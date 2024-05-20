# Comparing `tmp/api-management-local-0.0.8.tar.gz` & `tmp/api-management-local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api-management-local-0.0.8.tar", last modified: Wed Oct  4 09:04:12 2023, max compression
+gzip compressed data, was "api-management-local-0.0.9.tar", last modified: Wed Oct  4 09:55:47 2023, max compression
```

## Comparing `api-management-local-0.0.8.tar` & `api-management-local-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 09:04:12.963475 api-management-local-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     3800 2023-10-04 09:04:12.963475 api-management-local-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2023-10-04 09:03:27.000000 api-management-local-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 09:04:12.963475 api-management-local-0.0.8/api_management_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 09:04:12.963475 api-management-local-0.0.8/api_management_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 09:03:27.000000 api-management-local-0.0.8/api_management_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4268 2023-10-04 09:03:27.000000 api-management-local-0.0.8/api_management_local/src/api_management_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 09:04:12.963475 api-management-local-0.0.8/api_management_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3800 2023-10-04 09:04:12.000000 api-management-local-0.0.8/api_management_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      338 2023-10-04 09:04:12.000000 api-management-local-0.0.8/api_management_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-04 09:04:12.000000 api-management-local-0.0.8/api_management_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2023-10-04 09:04:12.000000 api-management-local-0.0.8/api_management_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-10-04 09:04:12.000000 api-management-local-0.0.8/api_management_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      732 2023-10-04 09:03:27.000000 api-management-local-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-04 09:04:12.963475 api-management-local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2023-10-04 09:03:27.000000 api-management-local-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 09:55:47.051212 api-management-local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2023-10-04 09:55:47.051212 api-management-local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2023-10-04 09:55:20.000000 api-management-local-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 09:55:47.043212 api-management-local-0.0.9/api_management_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 09:55:47.051212 api-management-local-0.0.9/api_management_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 09:55:20.000000 api-management-local-0.0.9/api_management_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2023-10-04 09:55:20.000000 api-management-local-0.0.9/api_management_local/src/api_management_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 09:55:47.051212 api-management-local-0.0.9/api_management_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2023-10-04 09:55:47.000000 api-management-local-0.0.9/api_management_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2023-10-04 09:55:47.000000 api-management-local-0.0.9/api_management_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-04 09:55:47.000000 api-management-local-0.0.9/api_management_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2023-10-04 09:55:47.000000 api-management-local-0.0.9/api_management_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2023-10-04 09:55:47.000000 api-management-local-0.0.9/api_management_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2023-10-04 09:55:20.000000 api-management-local-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-04 09:55:47.051212 api-management-local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2023-10-04 09:55:20.000000 api-management-local-0.0.9/setup.py
```

### Comparing `api-management-local-0.0.8/PKG-INFO` & `api-management-local-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api-management-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles <short-project-name-with-dash> Python
 Home-page: https://github.com/circles
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `api-management-local-0.0.8/README.md` & `api-management-local-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `api-management-local-0.0.8/api_management_local/src/api_management_local.py` & `api-management-local-0.0.9/api_management_local/src/api_management_local.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 from logger_local.LoggerComponentEnum import LoggerComponentEnum
 from circles_local_database_python.connector import Connector
 from circles_local_database_python.generic_crud import GenericCRUD
 
 API_MANAGEMENT_LOCAL_PYTHON_COMPONENT_ID = 212  
 API_MANAGEMENT_LOCAL_PYTHON_COMPONENT_NAME = "api-management-local-python-package"
 DEVELOPER_EMAIL = "heba.a@circ.zone"
-# TODO Why so we need it?
-API_Type_ID=1
+
 object1 = {
     'component_id': API_MANAGEMENT_LOCAL_PYTHON_COMPONENT_ID,
     'component_name': API_MANAGEMENT_LOCAL_PYTHON_COMPONENT_NAME,
     'component_category': LoggerComponentEnum.ComponentCategory.Code.value,
     'developer_email': DEVELOPER_EMAIL
 }
 load_dotenv()
@@ -55,26 +54,26 @@
            return list 
         except Exception as exception:
             logger.exception(object=exception)
             logger.end()
             raise
             
     @staticmethod
-    def get_actual_by_api_type_id( hours: int) -> int:
-        logger.start(object={'hours':str(hours)})
+    def get_actual_by_api_type_id( api_type_id:int, hours: int) -> int:
+        logger.start(object={'api_type_id':str(api_type_id),'hours':str(hours)})
         connection = Connector.connect("api_call")
         cursor = connection.cursor()
         try:
             # TODO: We should count only successful API calls
             cursor.execute("""
                   SELECT COUNT(*)
                   FROM api_call_view
                   WHERE api_type_id = %s
                   AND TIMESTAMPDIFF(HOUR, created_timestamp, NOW()) <= %s
-                  """.format(API_Type_ID, hours))
+                  """.format(api_type_id, hours))
             count_result = cursor.fetchone()[0]
             logger.end(object={'count_result':count_result})
             return count_result
         except Exception as exception:
             logger.exception(object=exception)
             logger.end()
             raise
```

### Comparing `api-management-local-0.0.8/api_management_local.egg-info/PKG-INFO` & `api-management-local-0.0.9/api_management_local.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api-management-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles <short-project-name-with-dash> Python
 Home-page: https://github.com/circles
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `api-management-local-0.0.8/pyproject.toml` & `api-management-local-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `api-management-local-0.0.8/setup.py` & `api-management-local-0.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 with open('README.md') as f:
     readme = f.read()
     
 setuptools.setup(
     # TODO: Please update the name and delete this line i.e. XXX-local or XXX-remote (without the -python-package suffix). Only lowercase, no underlines.
     name=PACKAGE_NAME,
-    version='0.0.8',  # update each time
+    version='0.0.9',  # update each time
     author="Circles",
     author_email="info@circlez.ai",
     # TODO: Please update the description and delete this line
     description="PyPI Package for Circles <short-project-name-with-dash> Python",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     # TODO: Please update the URL below
```

