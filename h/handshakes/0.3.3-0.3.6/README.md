# Comparing `tmp/handshakes-0.3.3.tar.gz` & `tmp/handshakes-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "handshakes-0.3.3.tar", max compression
+gzip compressed data, was "handshakes-0.3.6.tar", max compression
```

## Comparing `handshakes-0.3.3.tar` & `handshakes-0.3.6.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0      749 2024-05-06 19:29:28.744154 handshakes-0.3.3/README.md
--rw-r--r--   0        0        0      448 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/.version
--rw-r--r--   0        0        0       22 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/CommandLine/__init__.py
--rw-r--r--   0        0        0     8485 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/CommandLine/_init.py
--rw-r--r--   0        0        0     4326 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/CommandLine/center.py
--rw-r--r--   0        0        0       15 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/DBService/__init__.py
--rw-r--r--   0        0        0     3107 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/DBService/lifecycle.py
--rw-r--r--   0        0        0     4234 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/DBService/migrator.py
--rw-r--r--   0        0        0      570 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/DBService/models/__init__.py
--rw-r--r--   0        0        0      939 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/DBService/models/attachmentBase.py
--rw-r--r--   0        0        0     2034 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/DBService/models/config_base.py
--rw-r--r--   0        0        0     1618 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/DBService/models/dynamic_base.py
--rw-r--r--   0        0        0     1010 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/DBService/models/enums.py
--rw-r--r--   0        0        0     5894 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/DBService/models/result_base.py
--rw-r--r--   0        0        0     1167 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/DBService/models/static_base.py
--rw-r--r--   0        0        0     2102 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/DBService/models/types.py
--rw-r--r--   0        0        0       50 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/DBService/sanic_free_shared.py
--rw-r--r--   0        0        0      221 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/DBService/scripts/bump-v5.sql
--rw-r--r--   0        0        0      369 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/DBService/scripts/bump-v6.sql
--rw-r--r--   0        0        0      407 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/DBService/scripts/revert-v4.sql
--rw-r--r--   0        0        0       99 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/DBService/scripts/revert-v6.sql
--rw-r--r--   0        0        0      452 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/DBService/scripts/revert-v7.sql
--rw-r--r--   0        0        0      753 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/DBService/shared.py
--rw-r--r--   0        0        0        0 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/Endpoints/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/Endpoints/blueprints/__init__.py
--rw-r--r--   0        0        0     7967 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/Endpoints/blueprints/coreEndpoints.py
--rw-r--r--   0        0        0     1434 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/Endpoints/blueprints/utils.py
--rw-r--r--   0        0        0     1934 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/Endpoints/blueprints/writeServices.py
--rw-r--r--   0        0        0      431 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/Endpoints/center.py
--rw-r--r--   0        0        0     1055 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/Endpoints/core.py
--rw-r--r--   0        0        0      278 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/Endpoints/errorHandling.py
--rw-r--r--   0        0        0      954 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/Endpoints/internalEndpoints.py
--rw-r--r--   0        0        0      128 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/Endpoints/static_server.py
--rw-r--r--   0        0        0     2587 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/SchedularService/README.md
--rw-r--r--   0        0        0        0 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/SchedularService/__init__.py
--rw-r--r--   0        0        0     9654 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/SchedularService/completeTestRun.py
--rw-r--r--   0        0        0      591 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/SchedularService/constants.py
--rw-r--r--   0        0        0     4562 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/SchedularService/handlePending.py
--rw-r--r--   0        0        0     1635 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/SchedularService/handleTestResults.py
--rw-r--r--   0        0        0     8216 2024-05-06 19:29:28.760154 handshakes-0.3.3/handshake/services/SchedularService/modifySuites.py
--rw-r--r--   0        0        0     1867 2024-05-06 19:29:28.764154 handshakes-0.3.3/handshake/services/SchedularService/pruneTasks.py
--rw-r--r--   0        0        0      666 2024-05-06 19:29:28.764154 handshakes-0.3.3/handshake/services/SchedularService/refer_types.py
--rw-r--r--   0        0        0     1653 2024-05-06 19:29:28.764154 handshakes-0.3.3/handshake/services/SchedularService/register.py
--rw-r--r--   0        0        0    13922 2024-05-06 19:29:28.764154 handshakes-0.3.3/handshake/services/SchedularService/start.py
--rw-r--r--   0        0        0        0 2024-05-06 19:29:28.764154 handshakes-0.3.3/handshake/services/__init__.py
--rw-r--r--   0        0        0      193 2024-05-06 19:29:28.764154 handshakes-0.3.3/handshake/services/starter.py
--rw-r--r--   0        0        0     1576 2024-05-06 19:29:28.764154 handshakes-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     1861 1970-01-01 00:00:00.000000 handshakes-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0      749 2024-05-20 21:17:45.312587 handshakes-0.3.6/README.md
+-rw-r--r--   0        0        0      448 2024-05-20 21:17:45.328587 handshakes-0.3.6/handshake/.version
+-rw-r--r--   0        0        0       22 2024-05-20 21:17:45.328587 handshakes-0.3.6/handshake/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-20 21:17:45.328587 handshakes-0.3.6/handshake/services/CommandLine/__init__.py
+-rw-r--r--   0        0        0     8485 2024-05-20 21:17:45.328587 handshakes-0.3.6/handshake/services/CommandLine/_init.py
+-rw-r--r--   0        0        0     4326 2024-05-20 21:17:45.328587 handshakes-0.3.6/handshake/services/CommandLine/center.py
+-rw-r--r--   0        0        0       15 2024-05-20 21:17:45.328587 handshakes-0.3.6/handshake/services/DBService/__init__.py
+-rw-r--r--   0        0        0     3107 2024-05-20 21:17:45.328587 handshakes-0.3.6/handshake/services/DBService/lifecycle.py
+-rw-r--r--   0        0        0     4234 2024-05-20 21:17:45.328587 handshakes-0.3.6/handshake/services/DBService/migrator.py
+-rw-r--r--   0        0        0      570 2024-05-20 21:17:45.328587 handshakes-0.3.6/handshake/services/DBService/models/__init__.py
+-rw-r--r--   0        0        0      939 2024-05-20 21:17:45.328587 handshakes-0.3.6/handshake/services/DBService/models/attachmentBase.py
+-rw-r--r--   0        0        0     2034 2024-05-20 21:17:45.328587 handshakes-0.3.6/handshake/services/DBService/models/config_base.py
+-rw-r--r--   0        0        0     1618 2024-05-20 21:17:45.328587 handshakes-0.3.6/handshake/services/DBService/models/dynamic_base.py
+-rw-r--r--   0        0        0     1010 2024-05-20 21:17:45.328587 handshakes-0.3.6/handshake/services/DBService/models/enums.py
+-rw-r--r--   0        0        0     5833 2024-05-20 21:17:45.328587 handshakes-0.3.6/handshake/services/DBService/models/result_base.py
+-rw-r--r--   0        0        0     1167 2024-05-20 21:17:45.328587 handshakes-0.3.6/handshake/services/DBService/models/static_base.py
+-rw-r--r--   0        0        0     2102 2024-05-20 21:17:45.332587 handshakes-0.3.6/handshake/services/DBService/models/types.py
+-rw-r--r--   0        0        0       50 2024-05-20 21:17:45.332587 handshakes-0.3.6/handshake/services/DBService/sanic_free_shared.py
+-rw-r--r--   0        0        0      221 2024-05-20 21:17:45.332587 handshakes-0.3.6/handshake/services/DBService/scripts/bump-v5.sql
+-rw-r--r--   0        0        0      369 2024-05-20 21:17:45.332587 handshakes-0.3.6/handshake/services/DBService/scripts/bump-v6.sql
+-rw-r--r--   0        0        0      407 2024-05-20 21:17:45.332587 handshakes-0.3.6/handshake/services/DBService/scripts/revert-v4.sql
+-rw-r--r--   0        0        0       99 2024-05-20 21:17:45.332587 handshakes-0.3.6/handshake/services/DBService/scripts/revert-v6.sql
+-rw-r--r--   0        0        0      452 2024-05-20 21:17:45.332587 handshakes-0.3.6/handshake/services/DBService/scripts/revert-v7.sql
+-rw-r--r--   0        0        0      753 2024-05-20 21:17:45.332587 handshakes-0.3.6/handshake/services/DBService/shared.py
+-rw-r--r--   0        0        0        0 2024-05-20 21:17:45.332587 handshakes-0.3.6/handshake/services/Endpoints/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-20 21:17:45.332587 handshakes-0.3.6/handshake/services/Endpoints/blueprints/__init__.py
+-rw-r--r--   0        0        0     7967 2024-05-20 21:17:45.332587 handshakes-0.3.6/handshake/services/Endpoints/blueprints/coreEndpoints.py
+-rw-r--r--   0        0        0     1434 2024-05-20 21:17:45.332587 handshakes-0.3.6/handshake/services/Endpoints/blueprints/utils.py
+-rw-r--r--   0        0        0     1956 2024-05-20 21:17:45.332587 handshakes-0.3.6/handshake/services/Endpoints/blueprints/writeServices.py
+-rw-r--r--   0        0        0      431 2024-05-20 21:17:45.332587 handshakes-0.3.6/handshake/services/Endpoints/center.py
+-rw-r--r--   0        0        0     1055 2024-05-20 21:17:45.332587 handshakes-0.3.6/handshake/services/Endpoints/core.py
+-rw-r--r--   0        0        0      278 2024-05-20 21:17:45.332587 handshakes-0.3.6/handshake/services/Endpoints/errorHandling.py
+-rw-r--r--   0        0        0      954 2024-05-20 21:17:45.332587 handshakes-0.3.6/handshake/services/Endpoints/internalEndpoints.py
+-rw-r--r--   0        0        0      128 2024-05-20 21:17:45.332587 handshakes-0.3.6/handshake/services/Endpoints/static_server.py
+-rw-r--r--   0        0        0     2587 2024-05-20 21:17:45.332587 handshakes-0.3.6/handshake/services/SchedularService/README.md
+-rw-r--r--   0        0        0        0 2024-05-20 21:17:45.332587 handshakes-0.3.6/handshake/services/SchedularService/__init__.py
+-rw-r--r--   0        0        0     9654 2024-05-20 21:17:45.332587 handshakes-0.3.6/handshake/services/SchedularService/completeTestRun.py
+-rw-r--r--   0        0        0      875 2024-05-20 21:17:45.332587 handshakes-0.3.6/handshake/services/SchedularService/constants.py
+-rw-r--r--   0        0        0     4562 2024-05-20 21:17:45.332587 handshakes-0.3.6/handshake/services/SchedularService/handlePending.py
+-rw-r--r--   0        0        0     1635 2024-05-20 21:17:45.332587 handshakes-0.3.6/handshake/services/SchedularService/handleTestResults.py
+-rw-r--r--   0        0        0     8216 2024-05-20 21:17:45.332587 handshakes-0.3.6/handshake/services/SchedularService/modifySuites.py
+-rw-r--r--   0        0        0     1867 2024-05-20 21:17:45.332587 handshakes-0.3.6/handshake/services/SchedularService/pruneTasks.py
+-rw-r--r--   0        0        0      666 2024-05-20 21:17:45.332587 handshakes-0.3.6/handshake/services/SchedularService/refer_types.py
+-rw-r--r--   0        0        0     1653 2024-05-20 21:17:45.332587 handshakes-0.3.6/handshake/services/SchedularService/register.py
+-rw-r--r--   0        0        0    19394 2024-05-20 21:17:45.332587 handshakes-0.3.6/handshake/services/SchedularService/start.py
+-rw-r--r--   0        0        0        0 2024-05-20 21:17:45.332587 handshakes-0.3.6/handshake/services/__init__.py
+-rw-r--r--   0        0        0      193 2024-05-20 21:17:45.332587 handshakes-0.3.6/handshake/services/starter.py
+-rw-r--r--   0        0        0     1576 2024-05-20 21:17:45.332587 handshakes-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     1861 1970-01-01 00:00:00.000000 handshakes-0.3.6/PKG-INFO
```

### Comparing `handshakes-0.3.3/README.md` & `handshakes-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.3/handshake/services/CommandLine/_init.py` & `handshakes-0.3.6/handshake/services/CommandLine/_init.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.3/handshake/services/CommandLine/center.py` & `handshakes-0.3.6/handshake/services/CommandLine/center.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.3/handshake/services/DBService/lifecycle.py` & `handshakes-0.3.6/handshake/services/DBService/lifecycle.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.3/handshake/services/DBService/migrator.py` & `handshakes-0.3.6/handshake/services/DBService/migrator.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.3/handshake/services/DBService/models/__init__.py` & `handshakes-0.3.6/handshake/services/DBService/models/__init__.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.3/handshake/services/DBService/models/attachmentBase.py` & `handshakes-0.3.6/handshake/services/DBService/models/attachmentBase.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.3/handshake/services/DBService/models/config_base.py` & `handshakes-0.3.6/handshake/services/DBService/models/config_base.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.3/handshake/services/DBService/models/dynamic_base.py` & `handshakes-0.3.6/handshake/services/DBService/models/dynamic_base.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.3/handshake/services/DBService/models/enums.py` & `handshakes-0.3.6/handshake/services/DBService/models/enums.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.3/handshake/services/DBService/models/result_base.py` & `handshakes-0.3.6/handshake/services/DBService/models/result_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     CharField,
     ReverseRelation,
     ForeignKeyField,
     BooleanField,
     ForeignKeyRelation,
     TextField,
 )
-from tortoise.contrib.pydantic import pydantic_model_creator
 from handshake.services.DBService.models.enums import Status, SuiteType, LogType
 
 
 class CommandReportFields(Model):
     started = DatetimeField(descrption="Start Datetime field")
     ended = DatetimeField(null=True, description="End Datetime field")
     tests = IntField(default=0, null=False, description="No. of the test entries")
```

### Comparing `handshakes-0.3.3/handshake/services/DBService/models/static_base.py` & `handshakes-0.3.6/handshake/services/DBService/models/static_base.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.3/handshake/services/DBService/models/types.py` & `handshakes-0.3.6/handshake/services/DBService/models/types.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.3/handshake/services/DBService/shared.py` & `handshakes-0.3.6/handshake/services/DBService/shared.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.3/handshake/services/Endpoints/blueprints/coreEndpoints.py` & `handshakes-0.3.6/handshake/services/Endpoints/blueprints/coreEndpoints.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.3/handshake/services/Endpoints/blueprints/utils.py` & `handshakes-0.3.6/handshake/services/Endpoints/blueprints/utils.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.3/handshake/services/Endpoints/blueprints/writeServices.py` & `handshakes-0.3.6/handshake/services/Endpoints/blueprints/writeServices.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,17 @@
         return response
 
     payload = extractPayload(request, response)
     await attachWarn(payload, request.url)
     return JSONResponse(body=payload, status=response.status)
 
 
+# NOTE: depreciated
+
+
 @writeServices.put("/addAttachmentForEntity", error_format="json")
 async def saveImage(request: Request) -> HTTPResponse:
     attachment = AddAttachmentForEntity.model_validate(request.json)
 
     record = await StaticBase.create(
         entity_id=attachment.entityID,
         description=attachment.description,
```

### Comparing `handshakes-0.3.3/handshake/services/Endpoints/core.py` & `handshakes-0.3.6/handshake/services/Endpoints/core.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.3/handshake/services/Endpoints/internalEndpoints.py` & `handshakes-0.3.6/handshake/services/Endpoints/internalEndpoints.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.3/handshake/services/SchedularService/README.md` & `handshakes-0.3.6/handshake/services/SchedularService/README.md`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.3/handshake/services/SchedularService/completeTestRun.py` & `handshakes-0.3.6/handshake/services/SchedularService/completeTestRun.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.3/handshake/services/SchedularService/constants.py` & `handshakes-0.3.6/handshake/services/SchedularService/constants.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,10 +12,16 @@
 
 
 writtenAttachmentFolderName = "Attachments"
 exportAttachmentFolderName = "Import"
 
 EXPORT_RUNS_PAGE_FILE_NAME = "runs.json"
 EXPORT_RUN_PAGE_FILE_NAME = "run.json"
+EXPORT_SUITE_PAGE_FILE_NAME = "suite.json"
 EXPORT_PROJECTS_FILE_NAME = "projects.json"
 EXPORT_OVERVIEW_PAGE = "overview.json"
 EXPORT_ALL_SUITES = "suites.json"
+EXPORT_SUITE_TESTS_PAGE = "tests.json"
+EXPORT_TEST_ASSERTIONS = "assertions.json"
+EXPORT_TEST_ENTITY_ATTACHMENTS = "entity-attachments.json"
+EXPORT_TEST_RUN_ATTACHMENTS = "test-run-attachments.json"
+EXPORT_SUITE_RETRIED_MAP = "retries.json"
```

### Comparing `handshakes-0.3.3/handshake/services/SchedularService/handlePending.py` & `handshakes-0.3.6/handshake/services/SchedularService/handlePending.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.3/handshake/services/SchedularService/handleTestResults.py` & `handshakes-0.3.6/handshake/services/SchedularService/handleTestResults.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.3/handshake/services/SchedularService/modifySuites.py` & `handshakes-0.3.6/handshake/services/SchedularService/modifySuites.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.3/handshake/services/SchedularService/pruneTasks.py` & `handshakes-0.3.6/handshake/services/SchedularService/pruneTasks.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.3/handshake/services/SchedularService/refer_types.py` & `handshakes-0.3.6/handshake/services/SchedularService/refer_types.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.3/handshake/services/SchedularService/register.py` & `handshakes-0.3.6/handshake/services/SchedularService/register.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.3/handshake/services/SchedularService/start.py` & `handshakes-0.3.6/handshake/services/SchedularService/start.py`

 * *Files 22% similar despite different names*

```diff
@@ -26,18 +26,25 @@
     writtenAttachmentFolderName,
     exportAttachmentFolderName,
     EXPORT_RUN_PAGE_FILE_NAME,
     EXPORT_PROJECTS_FILE_NAME,
     EXPORT_RUNS_PAGE_FILE_NAME,
     EXPORT_OVERVIEW_PAGE,
     EXPORT_ALL_SUITES,
+    EXPORT_SUITE_PAGE_FILE_NAME,
+    EXPORT_SUITE_TESTS_PAGE,
+    EXPORT_TEST_ASSERTIONS,
+    EXPORT_TEST_ENTITY_ATTACHMENTS,
+    EXPORT_SUITE_RETRIED_MAP,
 )
 from handshake.services.DBService.models.dynamic_base import TaskBase, JobType
 from handshake.services.SchedularService.pruneTasks import pruneTasks
 from handshake.services.SchedularService.handleTestResults import delete_test_attachment
+from handshake.services.DBService.models.attachmentBase import AssertBase
+from handshake.services.DBService.models.static_base import StaticBase
 from handshake.services.SchedularService.handlePending import patch_jobs
 from handshake.services.SchedularService.refer_types import (
     SubSetOfRunBaseRequiredForProjectExport,
     SuiteSummary,
 )
 
 
@@ -246,15 +253,16 @@
                     )
                 )
 
                 (self.import_dir / str(test_run.testID)).mkdir(exist_ok=True)
 
                 exporter.create_task(
                     to_thread(
-                        self.save_run_query,
+                        self.save_test_run_level_files,
+                        EXPORT_RUN_PAGE_FILE_NAME,
                         str(test_run.testID),
                         json.dumps(run),
                     ),
                     name="export-run-page",
                 )
 
                 exporter.create_task(
@@ -308,15 +316,16 @@
             await SessionBase.filter(test_id=run_id)
             .only("entityName", "entityVersion", "simplified")
             .distinct()
             .values("entityName", "entityVersion", "simplified")
         )
 
         await to_thread(
-            self.save_overview_query,
+            self.save_test_run_level_files,
+            EXPORT_OVERVIEW_PAGE,
             run_id,
             json.dumps(
                 dict(
                     recentSuites=recent_suites,
                     aggregated=aggregated,
                     platforms=platforms,
                 )
@@ -331,34 +340,49 @@
             .annotate(
                 numberOfErrors=RawSQL("json_array_length(errors)"),
                 id=RawSQL("suiteID"),
                 p_id=RawSQL("parent"),
                 s=RawSQL("suitebase.started"),
                 e=RawSQL("suitebase.ended"),
                 error=RawSQL("errors ->> '[0]'"),
+                nextSuite=RawSQL(
+                    "(select suiteID from suitebase sb join sessionbase ssb on sb.session_id = ssb.sessionID"
+                    " where sb.suiteType = 'SUITE' AND sb.standing <> 'RETRIED' "
+                    " and suitebase.started <= sb.started and sb.suiteID <> suitebase.suiteID"
+                    " and 'suitebase__session'.'test_id' = ssb.test_id order by sb.started)"
+                ),
+                prevSuite=RawSQL(
+                    "(select suiteID from suitebase sb join sessionbase ssb on sb.session_id = ssb.sessionID"
+                    " where sb.suiteType = 'SUITE' AND sb.standing <> 'RETRIED' "
+                    " and suitebase.started >= sb.started and sb.suiteID <> suitebase.suiteID"
+                    " and 'suitebase__session'.'test_id' = ssb.test_id order by sb.started)"
+                ),
                 hasChildSuite=RawSQL(
                     "(select count(*) from suitebase sb where sb.parent=suitebase.suiteID "
                     "and sb.suiteType='SUITE' LIMIT 1)"
                 ),
             )
             .values(
                 "title",
                 "passed",
                 "failed",
                 "standing",
+                "tests",
                 "skipped",
                 "duration",
                 "file",
                 "retried",
                 "tags",
                 "description",
                 "errors",
                 "error",
                 "numberOfErrors",
                 "hasChildSuite",
+                "nextSuite",
+                "prevSuite",
                 suiteID="id",
                 parent="p_id",
                 started="s",
                 ended="e",
                 entityName="session__entityName",
                 entityVersion="session__entityVersion",
                 hooks="session__hooks",
@@ -369,15 +393,131 @@
                 rollup_tests="rollup__tests",
             )
         )
 
         await to_thread(
             self.save_all_suites_query,
             run_id,
-            json.dumps(all_suites),
+            all_suites,
+        )
+
+        await gather(
+            *[
+                self.export_suite(run_id, str(suite))
+                for suite in await SuiteBase.filter(
+                    Q(session__test_id=run_id) & Q(suiteType=SuiteType.SUITE)
+                ).values_list("suiteID", flat=True)
+            ]
+        )
+
+    async def export_suite(self, run_id: str, suite_id: str):
+        tests = await (
+            SuiteBase.filter(Q(parent=suite_id))
+            .order_by("started")
+            .prefetch_related("rollup")
+            .annotate(
+                numberOfErrors=RawSQL("json_array_length(errors)"),
+                id=RawSQL("suiteID"),
+                s=RawSQL("suitebase.started"),
+                e=RawSQL("suitebase.ended"),
+                error=RawSQL("errors ->> '[0]'"),
+                assertions=RawSQL(
+                    "(select count(ab.entity_id) from assertbase ab where ab.entity_id=suitebase.suiteID)"
+                ),
+            )
+            .values(
+                "title",
+                "standing",
+                "assertions",
+                "duration",
+                "file",
+                "retried",
+                "tags",
+                "suiteType",
+                "description",
+                "errors",
+                "error",
+                "numberOfErrors",
+                suiteID="id",
+                started="s",
+                ended="e",
+                hooks="session__hooks",
+                rollup_passed="rollup__passed",
+                rollup_failed="rollup__failed",
+                rollup_skipped="rollup__skipped",
+                rollup_tests="rollup__tests",
+            )
+        )
+
+        assertions = (
+            await AssertBase.filter(entity__parent=suite_id)
+            .annotate(id=RawSQL("entity_id"))
+            .all()
+            .values("title", "message", "interval", "passed", "wait", entity_id="id")
+        )
+
+        written_records = {}
+        written = (
+            await StaticBase.filter(entity__parent=suite_id)
+            .annotate(
+                id=RawSQL("entity_id"),
+                title=RawSQL("attachmentValue ->> 'title'"),
+                file=RawSQL("attachmentValue ->> 'value'"),
+            )
+            .all()
+            .values("type", "title", "description", "file", entity_id="id")
+        )
+
+        for record in written:
+            records = written_records.get(record["entity_id"], [])
+            records.append(record)
+            written_records[record["entity_id"]] = records
+
+        retried_map = {}
+
+        _, rows = await connections.get("default").execute_query(
+            "select key, value as suite, rb.tests, length, suite_id"
+            " from retriedbase rb join json_each(rb.tests)"
+            " join suitebase sb on suite = sb.suiteID"
+            " join sessionbase ssb on ssb.sessionID = sb.session_id"
+            " where ssb.test_id = ?",
+            (run_id,),
+        )
+
+        for row in rows:
+            retried_map[row["suite"]] = dict(row)
+
+        await to_thread(
+            self.save_under_suite_folder,
+            EXPORT_SUITE_TESTS_PAGE,
+            run_id,
+            suite_id,
+            json.dumps(tests),
+        )
+        await to_thread(
+            self.save_under_suite_folder,
+            EXPORT_TEST_ASSERTIONS,
+            run_id,
+            suite_id,
+            json.dumps(assertions),
+        )
+        await to_thread(
+            self.save_under_suite_folder,
+            EXPORT_TEST_ENTITY_ATTACHMENTS,
+            run_id,
+            suite_id,
+            json.dumps(dict(written=written_records)),
+        )
+
+        await to_thread(
+            self.save_under_suite_folder,
+            EXPORT_SUITE_RETRIED_MAP,
+            run_id,
+            suite_id,
+            json.dumps(retried_map),
         )
 
     def export_files(self):
         # we reset entire export folder
         if self.export_dir.exists():
             logger.debug("removing previous results")
             rmtree(self.export_dir)
@@ -387,15 +527,23 @@
         with open(self.dashboard_build, "r:bz2") as tar_file:
             tar_file.extractall(self.export_dir)
 
     def save_runs_query(self, feed: str, projectsFeed: str):
         (self.import_dir / EXPORT_RUNS_PAGE_FILE_NAME).write_text(feed)
         (self.import_dir / EXPORT_PROJECTS_FILE_NAME).write_text(projectsFeed)
 
-    def save_run_query(self, testID: str, feed: str):
-        (self.import_dir / testID / EXPORT_RUN_PAGE_FILE_NAME).write_text(feed)
+    def save_test_run_level_files(self, file_name: str, testID: str, feed: str):
+        (self.import_dir / testID / file_name).write_text(feed)
 
-    def save_overview_query(self, testID: str, feed: str):
-        (self.import_dir / testID / EXPORT_OVERVIEW_PAGE).write_text(feed)
+    def save_all_suites_query(self, testID: str, feed: dict):
+        (self.import_dir / testID / EXPORT_ALL_SUITES).write_text(json.dumps(feed))
+        for suite in feed:
+            suite_id = suite["suiteID"]
+            (self.import_dir / testID / suite_id).mkdir(exist_ok=True)
+            self.save_under_suite_folder(
+                EXPORT_SUITE_PAGE_FILE_NAME, testID, suite_id, json.dumps(suite)
+            )
 
-    def save_all_suites_query(self, testID: str, feed: str):
-        (self.import_dir / testID / EXPORT_ALL_SUITES).write_text(feed)
+    def save_under_suite_folder(
+        self, file_name: str, testID: str, suiteID: str, feed: str
+    ):
+        (self.import_dir / testID / suiteID / file_name).write_text(feed)
```

### Comparing `handshakes-0.3.3/pyproject.toml` & `handshakes-0.3.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "handshakes"
-version = "0.3.3"
+version = "0.3.6"
 description = "A service that's keen to process your test results"
 authors = ["Rahul <saihanumarahul66@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "handshake"}]
 maintainers = [
     "Rahul <saihanumarahul66@gmail.com>"
```

### Comparing `handshakes-0.3.3/PKG-INFO` & `handshakes-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: handshakes
-Version: 0.3.3
+Version: 0.3.6
 Summary: A service that's keen to process your test results
 License: MIT
 Author: Rahul
 Author-email: saihanumarahul66@gmail.com
 Maintainer: Rahul
 Maintainer-email: saihanumarahul66@gmail.com
 Requires-Python: >=3.11,<3.13
```

