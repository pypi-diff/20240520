# Comparing `tmp/pinecone_notebooks-0.1.0rc1.tar.gz` & `tmp/pinecone_notebooks-0.1.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinecone_notebooks-0.1.0rc1.tar", max compression
+gzip compressed data, was "pinecone_notebooks-0.1.1rc1.tar", max compression
```

## Comparing `pinecone_notebooks-0.1.0rc1.tar` & `pinecone_notebooks-0.1.1rc1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11352 2024-04-23 17:34:44.118422 pinecone_notebooks-0.1.0rc1/LICENSE
--rw-r--r--   0        0        0     1341 2024-04-23 17:34:44.118422 pinecone_notebooks-0.1.0rc1/README.md
--rw-r--r--   0        0        0       31 2024-04-23 17:34:44.118422 pinecone_notebooks-0.1.0rc1/pinecone_notebooks/__init__.py
--rw-r--r--   0        0        0        9 2024-04-23 17:34:51.146410 pinecone_notebooks-0.1.0rc1/pinecone_notebooks/__version__
--rw-r--r--   0        0        0      646 2024-04-23 17:34:44.118422 pinecone_notebooks-0.1.0rc1/pinecone_notebooks/colab/__init__.py
--rw-r--r--   0        0        0      151 2024-04-23 17:34:44.118422 pinecone_notebooks-0.1.0rc1/pinecone_notebooks/utils.py
--rw-r--r--   0        0        0     1376 2024-04-23 17:35:11.738380 pinecone_notebooks-0.1.0rc1/pyproject.toml
--rw-r--r--   0        0        0     2619 1970-01-01 00:00:00.000000 pinecone_notebooks-0.1.0rc1/PKG-INFO
+-rw-r--r--   0        0        0    11352 2024-05-20 17:09:37.102167 pinecone_notebooks-0.1.1rc1/LICENSE
+-rw-r--r--   0        0        0     1341 2024-05-20 17:09:37.102167 pinecone_notebooks-0.1.1rc1/README.md
+-rw-r--r--   0        0        0       31 2024-05-20 17:09:37.102167 pinecone_notebooks-0.1.1rc1/pinecone_notebooks/__init__.py
+-rw-r--r--   0        0        0        9 2024-05-20 17:09:41.774161 pinecone_notebooks-0.1.1rc1/pinecone_notebooks/__version__
+-rw-r--r--   0        0        0      656 2024-05-20 17:09:37.102167 pinecone_notebooks-0.1.1rc1/pinecone_notebooks/colab/__init__.py
+-rw-r--r--   0        0        0      151 2024-05-20 17:09:37.102167 pinecone_notebooks-0.1.1rc1/pinecone_notebooks/utils.py
+-rw-r--r--   0        0        0     1376 2024-05-20 17:09:58.258159 pinecone_notebooks-0.1.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     2619 1970-01-01 00:00:00.000000 pinecone_notebooks-0.1.1rc1/PKG-INFO
```

### Comparing `pinecone_notebooks-0.1.0rc1/LICENSE` & `pinecone_notebooks-0.1.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `pinecone_notebooks-0.1.0rc1/README.md` & `pinecone_notebooks-0.1.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `pinecone_notebooks-0.1.0rc1/pinecone_notebooks/colab/__init__.py` & `pinecone_notebooks-0.1.1rc1/pinecone_notebooks/colab/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 
   def SetApiKey(val):
     os.environ['PINECONE_API_KEY'] = val
 
   def Authenticate(source_tag: Optional[str] = None):
     output.register_callback('pinecone.SetApiKey', SetApiKey)
     display(HTML(data='<script type="text/javascript" src="https://connect.pinecone.io/embed.js"></script>'))
-    output.eval_js('connectToPinecone((val) => google.colab.kernel.invokeFunction("pinecone.SetApiKey", [val], {}), {integrationId: "colab"})')
+    output.eval_js('const x = connectToPinecone((val) => google.colab.kernel.invokeFunction("pinecone.SetApiKey", [val], {}), {integrationId: "colab"})')
```

### Comparing `pinecone_notebooks-0.1.0rc1/pyproject.toml` & `pinecone_notebooks-0.1.1rc1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pinecone-notebooks"
-version = "0.1.0.rc1"
+version = "0.1.1.rc1"
 packages = [
     { include="pinecone_notebooks" },
 ]
 description = "Helpers for using Pinecone with notebooks"
 authors = ["Pinecone Systems, Inc. <support@pinecone.io>"]
 license = "Apache-2.0"
 readme = "README.md"
```

### Comparing `pinecone_notebooks-0.1.0rc1/PKG-INFO` & `pinecone_notebooks-0.1.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinecone-notebooks
-Version: 0.1.0rc1
+Version: 0.1.1rc1
 Summary: Helpers for using Pinecone with notebooks
 Home-page: https://www.pinecone.io
 License: Apache-2.0
 Keywords: Pinecone,vector,database,cloud,jupyter,colab,notebooks
 Author: Pinecone Systems, Inc.
 Author-email: support@pinecone.io
 Requires-Python: >=3.10,<4.0
```

