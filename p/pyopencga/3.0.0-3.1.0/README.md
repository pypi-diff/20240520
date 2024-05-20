# Comparing `tmp/pyopencga-3.0.0.tar.gz` & `tmp/pyopencga-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyopencga-3.0.0.tar", last modified: Thu Mar  7 17:49:12 2024, max compression
+gzip compressed data, was "pyopencga-3.1.0.tar", last modified: Mon May 20 17:15:31 2024, max compression
```

## Comparing `pyopencga-3.0.0.tar` & `pyopencga-3.1.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 17:49:12.235914 pyopencga-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-07 17:46:26.000000 pyopencga-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-03-07 17:49:12.235914 pyopencga-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-03-07 17:46:26.000000 pyopencga-3.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 17:49:12.231914 pyopencga-3.0.0/pyopencga/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-07 17:46:28.000000 pyopencga-3.0.0/pyopencga/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13671 2024-03-07 17:46:28.000000 pyopencga-3.0.0/pyopencga/commons.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-07 17:46:28.000000 pyopencga-3.0.0/pyopencga/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13389 2024-03-07 17:46:28.000000 pyopencga-3.0.0/pyopencga/opencga_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-03-07 17:46:28.000000 pyopencga-3.0.0/pyopencga/opencga_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 17:49:12.235914 pyopencga-3.0.0/pyopencga/rest_clients/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 17:46:28.000000 pyopencga-3.0.0/pyopencga/rest_clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-03-07 17:46:29.000000 pyopencga-3.0.0/pyopencga/rest_clients/_parent_rest_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-03-07 17:46:29.000000 pyopencga-3.0.0/pyopencga/rest_clients/admin_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14511 2024-03-07 17:46:29.000000 pyopencga-3.0.0/pyopencga/rest_clients/alignment_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    59985 2024-03-07 17:46:29.000000 pyopencga-3.0.0/pyopencga/rest_clients/clinical_analysis_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    52556 2024-03-07 17:46:29.000000 pyopencga-3.0.0/pyopencga/rest_clients/clinical_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14689 2024-03-07 17:46:29.000000 pyopencga-3.0.0/pyopencga/rest_clients/cohort_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14182 2024-03-07 17:46:30.000000 pyopencga-3.0.0/pyopencga/rest_clients/disease_panel_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    15496 2024-03-07 17:46:30.000000 pyopencga-3.0.0/pyopencga/rest_clients/family_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    27172 2024-03-07 17:46:30.000000 pyopencga-3.0.0/pyopencga/rest_clients/file_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-03-07 17:46:30.000000 pyopencga-3.0.0/pyopencga/rest_clients/ga4gh_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    19110 2024-03-07 17:46:30.000000 pyopencga-3.0.0/pyopencga/rest_clients/individual_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12825 2024-03-07 17:46:30.000000 pyopencga-3.0.0/pyopencga/rest_clients/job_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-03-07 17:46:31.000000 pyopencga-3.0.0/pyopencga/rest_clients/meta_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-03-07 17:46:31.000000 pyopencga-3.0.0/pyopencga/rest_clients/organization_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-03-07 17:46:31.000000 pyopencga-3.0.0/pyopencga/rest_clients/project_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    19207 2024-03-07 17:46:31.000000 pyopencga-3.0.0/pyopencga/rest_clients/sample_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    15763 2024-03-07 17:46:31.000000 pyopencga-3.0.0/pyopencga/rest_clients/study_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-03-07 17:46:31.000000 pyopencga-3.0.0/pyopencga/rest_clients/user_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    61600 2024-03-07 17:46:31.000000 pyopencga-3.0.0/pyopencga/rest_clients/variant_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    25932 2024-03-07 17:46:31.000000 pyopencga-3.0.0/pyopencga/rest_clients/variant_operation_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8634 2024-03-07 17:46:28.000000 pyopencga-3.0.0/pyopencga/rest_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-03-07 17:46:29.000000 pyopencga-3.0.0/pyopencga/retry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 17:49:12.235914 pyopencga-3.0.0/pyopencga.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-03-07 17:49:12.000000 pyopencga-3.0.0/pyopencga.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-03-07 17:49:12.000000 pyopencga-3.0.0/pyopencga.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 17:49:12.000000 pyopencga-3.0.0/pyopencga.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-07 17:49:12.000000 pyopencga-3.0.0/pyopencga.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-07 17:49:12.000000 pyopencga-3.0.0/pyopencga.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 17:49:12.235914 pyopencga-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-03-07 17:46:26.000000 pyopencga-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:15:31.436223 pyopencga-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-20 17:15:18.000000 pyopencga-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-05-20 17:15:31.436223 pyopencga-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-05-20 17:15:18.000000 pyopencga-3.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:15:31.428223 pyopencga-3.1.0/pyopencga/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-20 17:15:18.000000 pyopencga-3.1.0/pyopencga/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13671 2024-05-20 17:15:18.000000 pyopencga-3.1.0/pyopencga/commons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-20 17:15:18.000000 pyopencga-3.1.0/pyopencga/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13389 2024-05-20 17:15:18.000000 pyopencga-3.1.0/pyopencga/opencga_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-20 17:15:18.000000 pyopencga-3.1.0/pyopencga/opencga_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:15:31.436223 pyopencga-3.1.0/pyopencga/rest_clients/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:15:18.000000 pyopencga-3.1.0/pyopencga/rest_clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-20 17:15:18.000000 pyopencga-3.1.0/pyopencga/rest_clients/_parent_rest_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-05-20 17:15:18.000000 pyopencga-3.1.0/pyopencga/rest_clients/admin_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14511 2024-05-20 17:15:18.000000 pyopencga-3.1.0/pyopencga/rest_clients/alignment_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59985 2024-05-20 17:15:18.000000 pyopencga-3.1.0/pyopencga/rest_clients/clinical_analysis_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52556 2024-05-20 17:15:18.000000 pyopencga-3.1.0/pyopencga/rest_clients/clinical_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14689 2024-05-20 17:15:18.000000 pyopencga-3.1.0/pyopencga/rest_clients/cohort_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14182 2024-05-20 17:15:18.000000 pyopencga-3.1.0/pyopencga/rest_clients/disease_panel_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15496 2024-05-20 17:15:18.000000 pyopencga-3.1.0/pyopencga/rest_clients/family_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27891 2024-05-20 17:15:18.000000 pyopencga-3.1.0/pyopencga/rest_clients/file_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-05-20 17:15:18.000000 pyopencga-3.1.0/pyopencga/rest_clients/ga4gh_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19110 2024-05-20 17:15:18.000000 pyopencga-3.1.0/pyopencga/rest_clients/individual_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12825 2024-05-20 17:15:18.000000 pyopencga-3.1.0/pyopencga/rest_clients/job_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-20 17:15:18.000000 pyopencga-3.1.0/pyopencga/rest_clients/meta_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-05-20 17:15:18.000000 pyopencga-3.1.0/pyopencga/rest_clients/organization_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-05-20 17:15:18.000000 pyopencga-3.1.0/pyopencga/rest_clients/project_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19207 2024-05-20 17:15:18.000000 pyopencga-3.1.0/pyopencga/rest_clients/sample_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19684 2024-05-20 17:15:18.000000 pyopencga-3.1.0/pyopencga/rest_clients/study_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-05-20 17:15:18.000000 pyopencga-3.1.0/pyopencga/rest_clients/user_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61600 2024-05-20 17:15:18.000000 pyopencga-3.1.0/pyopencga/rest_clients/variant_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25932 2024-05-20 17:15:18.000000 pyopencga-3.1.0/pyopencga/rest_clients/variant_operation_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8634 2024-05-20 17:15:18.000000 pyopencga-3.1.0/pyopencga/rest_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-20 17:15:18.000000 pyopencga-3.1.0/pyopencga/retry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:15:31.436223 pyopencga-3.1.0/pyopencga.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-05-20 17:15:31.000000 pyopencga-3.1.0/pyopencga.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-20 17:15:31.000000 pyopencga-3.1.0/pyopencga.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 17:15:31.000000 pyopencga-3.1.0/pyopencga.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-20 17:15:31.000000 pyopencga-3.1.0/pyopencga.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 17:15:31.000000 pyopencga-3.1.0/pyopencga.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 17:15:31.436223 pyopencga-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-20 17:15:18.000000 pyopencga-3.1.0/setup.py
```

### Comparing `pyopencga-3.0.0/LICENSE` & `pyopencga-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyopencga-3.0.0/PKG-INFO` & `pyopencga-3.1.0/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopencga
-Version: 3.0.0
+Version: 3.1.0
 Summary: A REST client for OpenCGA REST web services
 Home-page: https://github.com/opencb/opencga/tree/develop/opencga-client/src/main/python/pyopencga
 Author: David Gomez-Peregrina, Pablo Marin-Garcia, Daniel Perez-Gil
 Author-email: david.gomez@mgviz.org, pmarin@kanteron.com, dp529@cam.ac.uk
 License: Apache Software License
 Project-URL: Documentation, http://docs.opencb.org/display/opencga/Python
 Project-URL: Source, https://github.com/opencb/opencga/tree/develop/opencga-client/src/main/python/pyopencga
```

### Comparing `pyopencga-3.0.0/README.rst` & `pyopencga-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `pyopencga-3.0.0/pyopencga/commons.py` & `pyopencga-3.1.0/pyopencga/commons.py`

 * *Files identical despite different names*

### Comparing `pyopencga-3.0.0/pyopencga/opencga_client.py` & `pyopencga-3.1.0/pyopencga/opencga_client.py`

 * *Files identical despite different names*

### Comparing `pyopencga-3.0.0/pyopencga/opencga_config.py` & `pyopencga-3.1.0/pyopencga/opencga_config.py`

 * *Files identical despite different names*

### Comparing `pyopencga-3.0.0/pyopencga/rest_clients/_parent_rest_clients.py` & `pyopencga-3.1.0/pyopencga/rest_clients/_parent_rest_clients.py`

 * *Files identical despite different names*

### Comparing `pyopencga-3.0.0/pyopencga/rest_clients/admin_client.py` & `pyopencga-3.1.0/pyopencga/rest_clients/admin_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2024-03-06
+    Autogenerated on: 2024-04-10
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class Admin(_ParentRestClient):
     """
     This class contains methods for the 'Admin' webservices
-    Client version: 3.0.0-SNAPSHOT
+    Client version: 3.1.0-SNAPSHOT
     PATH: /{apiVersion}/admin
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(Admin, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def group_by_audit(self, fields, entity, **options):
         """
         Group by operation.
         PATH: /{apiVersion}/admin/audit/groupBy
 
         :param str entity: Entity to be grouped by. Allowed values: ['AUDIT
-            ORGANIZATION USER PROJECT STUDY FILE SAMPLE JOB INDIVIDUAL COHORT
-            DISEASE_PANEL FAMILY CLINICAL_ANALYSIS INTERPRETATION VARIANT
-            ALIGNMENT CLINICAL EXPRESSION RGA FUNCTIONAL'] (REQUIRED)
+            NOTE ORGANIZATION USER PROJECT STUDY FILE SAMPLE JOB INDIVIDUAL
+            COHORT DISEASE_PANEL FAMILY CLINICAL_ANALYSIS INTERPRETATION
+            VARIANT ALIGNMENT CLINICAL EXPRESSION RGA FUNCTIONAL'] (REQUIRED)
         :param str fields: Comma separated list of fields by which to group
             by. (REQUIRED)
         :param bool count: Count the number of elements matching the group.
         :param int limit: Maximum number of documents (groups) to be returned.
         :param str action: Action performed.
         :param str before: Object before update.
         :param str after: Object after update.
```

### Comparing `pyopencga-3.0.0/pyopencga/rest_clients/alignment_client.py` & `pyopencga-3.1.0/pyopencga/rest_clients/alignment_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2024-03-06
+    Autogenerated on: 2024-04-10
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class Alignment(_ParentRestClient):
     """
     This class contains methods for the 'Analysis - Alignment' webservices
-    Client version: 3.0.0-SNAPSHOT
+    Client version: 3.1.0-SNAPSHOT
     PATH: /{apiVersion}/analysis/alignment
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(Alignment, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def run_bwa(self, data=None, **options):
```

### Comparing `pyopencga-3.0.0/pyopencga/rest_clients/clinical_analysis_client.py` & `pyopencga-3.1.0/pyopencga/rest_clients/clinical_analysis_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2024-03-06
+    Autogenerated on: 2024-04-10
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class ClinicalAnalysis(_ParentRestClient):
     """
     This class contains methods for the 'Analysis - Clinical' webservices
-    Client version: 3.0.0-SNAPSHOT
+    Client version: 3.1.0-SNAPSHOT
     PATH: /{apiVersion}/analysis/clinical
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(ClinicalAnalysis, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def update_acl(self, members, action, data=None, **options):
```

### Comparing `pyopencga-3.0.0/pyopencga/rest_clients/clinical_client.py` & `pyopencga-3.1.0/pyopencga/rest_clients/clinical_client.py`

 * *Files identical despite different names*

### Comparing `pyopencga-3.0.0/pyopencga/rest_clients/cohort_client.py` & `pyopencga-3.1.0/pyopencga/rest_clients/cohort_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2024-03-06
+    Autogenerated on: 2024-04-10
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class Cohort(_ParentRestClient):
     """
     This class contains methods for the 'Cohorts' webservices
-    Client version: 3.0.0-SNAPSHOT
+    Client version: 3.1.0-SNAPSHOT
     PATH: /{apiVersion}/cohorts
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(Cohort, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def update_acl(self, members, action, data=None, **options):
```

### Comparing `pyopencga-3.0.0/pyopencga/rest_clients/disease_panel_client.py` & `pyopencga-3.1.0/pyopencga/rest_clients/disease_panel_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2024-03-06
+    Autogenerated on: 2024-04-10
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class DiseasePanel(_ParentRestClient):
     """
     This class contains methods for the 'Disease Panels' webservices
-    Client version: 3.0.0-SNAPSHOT
+    Client version: 3.1.0-SNAPSHOT
     PATH: /{apiVersion}/panels
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(DiseasePanel, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def update_acl(self, members, action, data=None, **options):
```

### Comparing `pyopencga-3.0.0/pyopencga/rest_clients/family_client.py` & `pyopencga-3.1.0/pyopencga/rest_clients/family_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2024-03-06
+    Autogenerated on: 2024-04-10
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class Family(_ParentRestClient):
     """
     This class contains methods for the 'Families' webservices
-    Client version: 3.0.0-SNAPSHOT
+    Client version: 3.1.0-SNAPSHOT
     PATH: /{apiVersion}/families
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(Family, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def update_acl(self, members, action, data=None, **options):
```

### Comparing `pyopencga-3.0.0/pyopencga/rest_clients/file_client.py` & `pyopencga-3.1.0/pyopencga/rest_clients/file_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2024-03-06
+    Autogenerated on: 2024-04-10
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class File(_ParentRestClient):
     """
     This class contains methods for the 'Files' webservices
-    Client version: 3.0.0-SNAPSHOT
+    Client version: 3.1.0-SNAPSHOT
     PATH: /{apiVersion}/files
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(File, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def update_acl(self, members, action, data=None, **options):
@@ -510,14 +510,31 @@
         :param str file: File ID. (REQUIRED)
         :param str study: Study [[organization@]project:]study where study and
             project can be either the ID or UUID.
         """
 
         return self._get(category='files', resource='image', query_id=file, **options)
 
+    def move(self, file, data=None, **options):
+        """
+        Move file to a different path.
+        PATH: /{apiVersion}/files/{file}/move
+
+        :param dict data: Parameters to modify. (REQUIRED)
+        :param str file: File id, UUID or name. (REQUIRED)
+        :param str include: Fields included in the response, whole JSON path
+            must be provided.
+        :param str exclude: Fields excluded in the response, whole JSON path
+            must be provided.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
+        """
+
+        return self._post(category='files', resource='move', query_id=file, data=data, **options)
+
     def refresh(self, file, **options):
         """
         Refresh metadata from the selected file or folder. Return updated
             files.
         PATH: /{apiVersion}/files/{file}/refresh
 
         :param str file: File id, name or path. Paths must be separated by :
```

### Comparing `pyopencga-3.0.0/pyopencga/rest_clients/ga4gh_client.py` & `pyopencga-3.1.0/pyopencga/rest_clients/ga4gh_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2024-03-06
+    Autogenerated on: 2024-04-10
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class GA4GH(_ParentRestClient):
     """
     This class contains methods for the 'GA4GH' webservices
-    Client version: 3.0.0-SNAPSHOT
+    Client version: 3.1.0-SNAPSHOT
     PATH: /{apiVersion}/ga4gh
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(GA4GH, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def search_reads(self, **options):
```

### Comparing `pyopencga-3.0.0/pyopencga/rest_clients/individual_client.py` & `pyopencga-3.1.0/pyopencga/rest_clients/individual_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2024-03-06
+    Autogenerated on: 2024-04-10
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class Individual(_ParentRestClient):
     """
     This class contains methods for the 'Individuals' webservices
-    Client version: 3.0.0-SNAPSHOT
+    Client version: 3.1.0-SNAPSHOT
     PATH: /{apiVersion}/individuals
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(Individual, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def update_acl(self, members, action, data=None, **options):
```

### Comparing `pyopencga-3.0.0/pyopencga/rest_clients/job_client.py` & `pyopencga-3.1.0/pyopencga/rest_clients/job_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2024-03-06
+    Autogenerated on: 2024-04-10
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class Job(_ParentRestClient):
     """
     This class contains methods for the 'Jobs' webservices
-    Client version: 3.0.0-SNAPSHOT
+    Client version: 3.1.0-SNAPSHOT
     PATH: /{apiVersion}/jobs
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(Job, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def update_acl(self, members, action, data=None, **options):
```

### Comparing `pyopencga-3.0.0/pyopencga/rest_clients/meta_client.py` & `pyopencga-3.1.0/pyopencga/rest_clients/meta_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2024-03-06
+    Autogenerated on: 2024-04-10
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class Meta(_ParentRestClient):
     """
     This class contains methods for the 'Meta' webservices
-    Client version: 3.0.0-SNAPSHOT
+    Client version: 3.1.0-SNAPSHOT
     PATH: /{apiVersion}/meta
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(Meta, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def about(self, **options):
```

### Comparing `pyopencga-3.0.0/pyopencga/rest_clients/project_client.py` & `pyopencga-3.1.0/pyopencga/rest_clients/project_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2024-03-06
+    Autogenerated on: 2024-04-10
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class Project(_ParentRestClient):
     """
     This class contains methods for the 'Projects' webservices
-    Client version: 3.0.0-SNAPSHOT
+    Client version: 3.1.0-SNAPSHOT
     PATH: /{apiVersion}/projects
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(Project, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def create(self, data=None, **options):
```

### Comparing `pyopencga-3.0.0/pyopencga/rest_clients/sample_client.py` & `pyopencga-3.1.0/pyopencga/rest_clients/sample_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2024-03-06
+    Autogenerated on: 2024-04-10
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class Sample(_ParentRestClient):
     """
     This class contains methods for the 'Samples' webservices
-    Client version: 3.0.0-SNAPSHOT
+    Client version: 3.1.0-SNAPSHOT
     PATH: /{apiVersion}/samples
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(Sample, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def update_acl(self, members, action, data=None, **options):
```

### Comparing `pyopencga-3.0.0/pyopencga/rest_clients/study_client.py` & `pyopencga-3.1.0/pyopencga/rest_clients/study_client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2024-03-06
+    Autogenerated on: 2024-04-10
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class Study(_ParentRestClient):
     """
     This class contains methods for the 'Studies' webservices
-    Client version: 3.0.0-SNAPSHOT
+    Client version: 3.1.0-SNAPSHOT
     PATH: /{apiVersion}/studies
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(Study, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def update_acl(self, members, action, data=None, **options):
@@ -134,15 +134,15 @@
         :param int limit: Number of results to be returned.
         :param int skip: Number of results to skip.
         :param bool count: Get the total number of results matching the query.
             Deactivated by default.
         :param str operation_id: Audit operation UUID.
         :param str user_id: User ID.
         :param str action: Action performed by the user.
-        :param str resource: Resource involved. Allowed values: ['AUDIT
+        :param str resource: Resource involved. Allowed values: ['AUDIT NOTE
             ORGANIZATION USER PROJECT STUDY FILE SAMPLE JOB INDIVIDUAL COHORT
             DISEASE_PANEL FAMILY CLINICAL_ANALYSIS INTERPRETATION VARIANT
             ALIGNMENT CLINICAL EXPRESSION RGA FUNCTIONAL']
         :param str resource_id: Resource ID.
         :param str resource_uuid: resource UUID.
         :param str status: Filter by status. Allowed values: ['SUCCESS ERROR']
         :param str date: Date. Format: yyyyMMddHHmmss. Examples: >2018,
@@ -193,14 +193,95 @@
             project can be either the ID or UUID. (REQUIRED)
         :param str action: Action to be performed: ADD, SET or REMOVE users
             to/from a group. Allowed values: ['ADD SET REMOVE']
         """
 
         return self._post(category='studies', resource='users/update', query_id=study, subcategory='groups', second_query_id=group, data=data, **options)
 
+    def create_notes(self, study, data=None, **options):
+        """
+        Create a new note.
+        PATH: /{apiVersion}/studies/{study}/notes/create
+
+        :param dict data: JSON containing the Note to be added. (REQUIRED)
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID. (REQUIRED)
+        :param str include: Fields included in the response, whole JSON path
+            must be provided.
+        :param str exclude: Fields excluded in the response, whole JSON path
+            must be provided.
+        :param bool include_result: Flag indicating to include the created or
+            updated document result in the response.
+        """
+
+        return self._post(category='studies', resource='create', query_id=study, subcategory='notes', data=data, **options)
+
+    def search_notes(self, study, **options):
+        """
+        Search for notes of scope STUDY.
+        PATH: /{apiVersion}/studies/{study}/notes/search
+
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID. (REQUIRED)
+        :param str include: Fields included in the response, whole JSON path
+            must be provided.
+        :param str exclude: Fields excluded in the response, whole JSON path
+            must be provided.
+        :param str creation_date: Creation date. Format: yyyyMMddHHmmss.
+            Examples: >2018, 2017-2018, <201805.
+        :param str modification_date: Modification date. Format:
+            yyyyMMddHHmmss. Examples: >2018, 2017-2018, <201805.
+        :param str id: Note unique identifier.
+        :param str uuid: Unique 32-character identifier assigned automatically
+            by OpenCGA.
+        :param str user_id: User that wrote that Note.
+        :param str tags: Note tags.
+        :param str visibility: Visibility of the Note.
+        :param str version: Autoincremental version assigned to the registered
+            entry. By default, updates does not create new versions. To enable
+            versioning, users must set the `incVersion` flag from the /update
+            web service when updating the document.
+        """
+
+        return self._get(category='studies', resource='search', query_id=study, subcategory='notes', **options)
+
+    def delete_notes(self, study, id, **options):
+        """
+        Delete note.
+        PATH: /{apiVersion}/studies/{study}/notes/{id}/delete
+
+        :param str id: Note unique identifier. (REQUIRED)
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID. (REQUIRED)
+        :param bool include_result: Flag indicating to include the created or
+            updated document result in the response.
+        """
+
+        return self._delete(category='studies', resource='delete', query_id=study, subcategory='notes', second_query_id=id, **options)
+
+    def update_notes(self, study, id, data=None, **options):
+        """
+        Update a note.
+        PATH: /{apiVersion}/studies/{study}/notes/{id}/update
+
+        :param dict data: JSON containing the Note fields to be updated.
+            (REQUIRED)
+        :param str id: Note unique identifier. (REQUIRED)
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID. (REQUIRED)
+        :param str include: Fields included in the response, whole JSON path
+            must be provided.
+        :param str exclude: Fields excluded in the response, whole JSON path
+            must be provided.
+        :param bool include_result: Flag indicating to include the created or
+            updated document result in the response.
+        """
+
+        return self._post(category='studies', resource='update', query_id=study, subcategory='notes', second_query_id=id, data=data, **options)
+
     def permission_rules(self, study, entity, **options):
         """
         Fetch permission rules.
         PATH: /{apiVersion}/studies/{study}/permissionRules
 
         :param str entity: Entity where the permission rules should be applied
             to. Allowed values: ['SAMPLES FILES COHORTS INDIVIDUALS FAMILIES
@@ -270,15 +351,15 @@
     def delete_templates(self, study, template_id, **options):
         """
         Delete template.
         PATH: /{apiVersion}/studies/{study}/templates/{templateId}/delete
 
         :param str template_id: Template id. (REQUIRED)
         :param str study: Study [[organization@]project:]study where study and
-            project can be either the ID or UUID.
+            project can be either the ID or UUID. (REQUIRED)
         """
 
         return self._delete(category='studies', resource='delete', query_id=study, subcategory='templates', second_query_id=template_id, **options)
 
     def update(self, study, data=None, **options):
         """
         Update some study attributes.
```

### Comparing `pyopencga-3.0.0/pyopencga/rest_clients/user_client.py` & `pyopencga-3.1.0/pyopencga/rest_clients/user_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2024-03-06
+    Autogenerated on: 2024-04-10
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class User(_ParentRestClient):
     """
     This class contains methods for the 'Users' webservices
-    Client version: 3.0.0-SNAPSHOT
+    Client version: 3.1.0-SNAPSHOT
     PATH: /{apiVersion}/users
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(User, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def anonymous(self, organization, **options):
```

### Comparing `pyopencga-3.0.0/pyopencga/rest_clients/variant_client.py` & `pyopencga-3.1.0/pyopencga/rest_clients/variant_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2024-03-06
+    Autogenerated on: 2024-04-10
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class Variant(_ParentRestClient):
     """
     This class contains methods for the 'Analysis - Variant' webservices
-    Client version: 3.0.0-SNAPSHOT
+    Client version: 3.1.0-SNAPSHOT
     PATH: /{apiVersion}/analysis/variant
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(Variant, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def aggregation_stats(self, **options):
```

### Comparing `pyopencga-3.0.0/pyopencga/rest_clients/variant_operation_client.py` & `pyopencga-3.1.0/pyopencga/rest_clients/variant_operation_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2024-03-06
+    Autogenerated on: 2024-04-10
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class VariantOperation(_ParentRestClient):
     """
     This class contains methods for the 'Operations - Variant Storage' webservices
-    Client version: 3.0.0-SNAPSHOT
+    Client version: 3.1.0-SNAPSHOT
     PATH: /{apiVersion}/operation
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(VariantOperation, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def configure_cellbase(self, data=None, **options):
```

### Comparing `pyopencga-3.0.0/pyopencga/rest_response.py` & `pyopencga-3.1.0/pyopencga/rest_response.py`

 * *Files identical despite different names*

### Comparing `pyopencga-3.0.0/pyopencga/retry.py` & `pyopencga-3.1.0/pyopencga/retry.py`

 * *Files identical despite different names*

### Comparing `pyopencga-3.0.0/pyopencga.egg-info/PKG-INFO` & `pyopencga-3.1.0/pyopencga.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopencga
-Version: 3.0.0
+Version: 3.1.0
 Summary: A REST client for OpenCGA REST web services
 Home-page: https://github.com/opencb/opencga/tree/develop/opencga-client/src/main/python/pyopencga
 Author: David Gomez-Peregrina, Pablo Marin-Garcia, Daniel Perez-Gil
 Author-email: david.gomez@mgviz.org, pmarin@kanteron.com, dp529@cam.ac.uk
 License: Apache Software License
 Project-URL: Documentation, http://docs.opencb.org/display/opencga/Python
 Project-URL: Source, https://github.com/opencb/opencga/tree/develop/opencga-client/src/main/python/pyopencga
```

### Comparing `pyopencga-3.0.0/pyopencga.egg-info/SOURCES.txt` & `pyopencga-3.1.0/pyopencga.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyopencga-3.0.0/setup.py` & `pyopencga-3.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='pyopencga',
-    version='3.0.0',
+    version='3.1.0',
     description='A REST client for OpenCGA REST web services',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     url='https://github.com/opencb/opencga/tree/develop/opencga-client/src/main/python/pyopencga',
     packages=['pyopencga', 'pyopencga.rest_clients'],
     license='Apache Software License',
     author='David Gomez-Peregrina, Pablo Marin-Garcia, Daniel Perez-Gil',
```

