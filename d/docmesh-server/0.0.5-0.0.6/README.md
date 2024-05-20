# Comparing `tmp/docmesh_server-0.0.5.tar.gz` & `tmp/docmesh_server-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docmesh_server-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "docmesh_server-0.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `docmesh_server-0.0.5.tar` & `docmesh_server-0.0.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       16 2024-05-14 04:58:32.409536 docmesh_server-0.0.5/README.md
--rw-r--r--   0        0        0       64 2024-05-18 04:25:07.075131 docmesh_server-0.0.5/docmesh_server/__init__.py
--rw-r--r--   0        0        0     6899 2024-05-18 04:15:24.263777 docmesh_server-0.0.5/docmesh_server/main.py
--rw-r--r--   0        0        0      673 2024-05-17 06:29:59.531015 docmesh_server-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 docmesh_server-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       16 2024-05-14 04:58:32.409536 docmesh_server-0.0.6/README.md
+-rw-r--r--   0        0        0       64 2024-05-20 09:08:24.619547 docmesh_server-0.0.6/docmesh_server/__init__.py
+-rw-r--r--   0        0        0    10156 2024-05-20 09:06:56.477538 docmesh_server-0.0.6/docmesh_server/main.py
+-rw-r--r--   0        0        0      673 2024-05-20 09:08:34.267768 docmesh_server-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 docmesh_server-0.0.6/PKG-INFO
```

### Comparing `docmesh_server-0.0.5/docmesh_server/main.py` & `docmesh_server-0.0.6/docmesh_server/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from fastapi import status, Depends, HTTPException, Response, FastAPI
 from fastapi.responses import StreamingResponse
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.security import HTTPBearer, HTTPAuthorizationCredentials
 
 from docmesh_core.utils.semantic_scholar import get_paper_id
 from docmesh_core.db.neo import add_entity, _add_paper, mark_paper_read, DuplicateEntity
+from docmesh_core.db.neo import add_collection, add_paper_to_collection
 from docmesh_core.db.auth import get_entity_from_auth, add_auth_for_entity
 from docmesh_agent.agent import execute_docmesh_agent, aexecute_docmesh_agnet
 from docmesh_agent.embeddings.embeddings import update_paper_embeddings
 
 if (neo4j_url := os.getenv("NEO4J_URL")) is None:
     raise ValueError("You have not set neo4j database url using environment `NEO4J_URL`.")
 else:
@@ -45,22 +46,35 @@
 auth_scheme = HTTPBearer()
 
 
 class AddEntityBody(BaseModel):
     entity_name: str
 
 
+class AddCollectionBody(BaseModel):
+    collection_name: str
+
+
+class AddCollectionPaperBody(BaseModel):
+    collection_name: str
+    paper: str
+
+
 class AddPaperBody(BaseModel):
     paper: str
 
 
-class ReadPaperBody(BaseModel):
+class MarkPaperBody(BaseModel):
     paper_id: str
 
 
+class AddAndMarkPaperBody(BaseModel):
+    paper: str
+
+
 class AgentBody(BaseModel):
     session_id: str
     query: str
 
 
 def _check_access_token(access_token: str) -> str:
     if (entity_name := get_entity_from_auth(engine, access_token)) is None:
@@ -120,14 +134,65 @@
         data = {
             "msg": f"Failed to add a new entity {body.entity_name}, with error {e}.",
         }
 
     return {"data": data}
 
 
+@app.post("/add_collection")
+def add_collection_api(
+    body: AddCollectionBody,
+    response: Response,
+    token: HTTPAuthorizationCredentials = Depends(auth_scheme),
+) -> dict[str, Any]:
+    _check_admin_access_token(token.credentials)
+
+    try:
+        add_collection(collection_name=body.collection_name)
+        data = {
+            "msg": f"Successfully add a new collection {body.collection_name}.",
+        }
+    except Exception as e:
+        response.status_code = status.HTTP_500_INTERNAL_SERVER_ERROR
+        data = {"msg": f"Failed to add a new collection {body.collection_name}, with error: {e}."}
+
+    return {"data": data}
+
+
+@app.post("/add_collection_paper")
+def add_collection_paper_api(
+    body: AddCollectionPaperBody,
+    response: Response,
+    token: HTTPAuthorizationCredentials = Depends(auth_scheme),
+) -> dict[str, Any]:
+    _check_admin_access_token(token.credentials)
+
+    semantic_scholar_paper_id = get_paper_id(body.paper)
+
+    if semantic_scholar_paper_id is None:
+        response.status_code = status.HTTP_404_NOT_FOUND
+        data = {
+            "msg": f"Failed to add {body.paper} to collection, cannot find semantic scholar paper id.",
+        }
+    else:
+        try:
+            paper_id = _add_paper(paper_id=semantic_scholar_paper_id).paper_id
+            add_paper_to_collection(paper_id=paper_id, collection_name=body.collection_name)
+            data = {
+                "msg": f"Successfully add paper {body.paper} to collection {body.collection_name}.",
+            }
+        except Exception as e:
+            response.status_code = status.HTTP_500_INTERNAL_SERVER_ERROR
+            data = {
+                "msg": f"Failed to add paper {body.paper} to collection {body.collection_name} with error: {e}.",
+            }
+
+    return {"data": data}
+
+
 @app.post("/update_embeddings")
 def update_embeddings_api(
     response: Response,
     token: HTTPAuthorizationCredentials = Depends(auth_scheme),
 ) -> dict[str, Any]:
     _check_admin_access_token(token.credentials)
 
@@ -173,15 +238,15 @@
             }
 
     return {"data": data}
 
 
 @app.post("/mark_paper")
 def mark_paper_read_api(
-    body: ReadPaperBody,
+    body: MarkPaperBody,
     response: Response,
     token: HTTPAuthorizationCredentials = Depends(auth_scheme),
 ) -> dict[str, Any]:
     entity_name = _check_access_token(token.credentials)
 
     try:
         mark_paper_read(entity_name=entity_name, paper_id=body.paper_id)
@@ -193,14 +258,47 @@
         data = {
             "msg": f"Failed to mark paper {body.paper_id} with error: {e}.",
         }
 
     return {"data": data}
 
 
+@app.post("/add_and_mark_paper")
+def add_and_mark_paper_read_api(
+    body: AddAndMarkPaperBody,
+    response: Response,
+    token: HTTPAuthorizationCredentials = Depends(auth_scheme),
+) -> dict[str, Any]:
+    entity_name = _check_access_token(token.credentials)
+
+    semantic_scholar_paper_id = get_paper_id(body.paper)
+
+    if semantic_scholar_paper_id is None:
+        response.status_code = status.HTTP_404_NOT_FOUND
+        data = {
+            "msg": f"Failed to add and mark paper {body.paper}, cannot find semantic scholar paper id.",
+        }
+    else:
+        try:
+            paper_id = _add_paper(paper_id=semantic_scholar_paper_id).paper_id
+            mark_paper_read(entity_name=entity_name, paper_id=paper_id)
+            data = {
+                "msg": (
+                    f"Successfully add and mark paper {body.paper} read with paper id {paper_id} for {entity_name}."
+                ),
+            }
+        except Exception as e:
+            response.status_code = status.HTTP_500_INTERNAL_SERVER_ERROR
+            data = {
+                "msg": f"Failed to add and mark paper {body.paper} read with error: {e}.",
+            }
+
+    return {"data": data}
+
+
 @app.post("/agent")
 def execute_docmesh_agent_api(
     body: AgentBody,
     response: Response,
     token: HTTPAuthorizationCredentials = Depends(auth_scheme),
 ) -> dict[str, Any]:
     entity_name = _check_access_token(token.credentials)
```

### Comparing `docmesh_server-0.0.5/pyproject.toml` & `docmesh_server-0.0.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Operating System :: OS Independent"
 ]
 requires-python = ">=3.8"
 dependencies = [
-    "docmesh-core>=0.0.5",
+    "docmesh-core>=0.0.7",
     "docmesh-agent>=0.0.6",
     "fastapi==0.111.0",
     "uvicorn==0.29.0",
     "gunicorn==19.3.0",
 ]
 
 [tool.flake8]
```

### Comparing `docmesh_server-0.0.5/PKG-INFO` & `docmesh_server-0.0.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: docmesh_server
-Version: 0.0.5
+Version: 0.0.6
 Summary: Server of docmesh.
 Author-email: Zhengkai Yang <kyle.yang1995@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
-Requires-Dist: docmesh-core>=0.0.5
+Requires-Dist: docmesh-core>=0.0.7
 Requires-Dist: docmesh-agent>=0.0.6
 Requires-Dist: fastapi==0.111.0
 Requires-Dist: uvicorn==0.29.0
 Requires-Dist: gunicorn==19.3.0
 
 # docemsh server
```

