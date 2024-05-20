# Comparing `tmp/data_prep_toolkit_kfp-0.0.1.dev9.tar.gz` & `tmp/data_prep_toolkit_kfp-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_prep_toolkit_kfp-0.0.1.dev9.tar", last modified: Sun May 12 13:30:25 2024, max compression
+gzip compressed data, was "data_prep_toolkit_kfp-0.1.0.tar", last modified: Thu May 16 11:57:59 2024, max compression
```

## Comparing `data_prep_toolkit_kfp-0.0.1.dev9.tar` & `data_prep_toolkit_kfp-0.1.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 13:30:25.632277 data_prep_toolkit_kfp-0.0.1.dev9/
--rw-r--r--   0 eres      (1000) eres      (1000)     2117 2024-05-12 07:01:53.000000 data_prep_toolkit_kfp-0.0.1.dev9/Makefile
--rw-r--r--   0 eres      (1000) eres      (1000)     2737 2024-05-12 13:30:25.632277 data_prep_toolkit_kfp-0.0.1.dev9/PKG-INFO
--rw-r--r--   0 eres      (1000) eres      (1000)     1889 2024-05-12 07:01:53.000000 data_prep_toolkit_kfp-0.0.1.dev9/README.md
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 13:30:25.612277 data_prep_toolkit_kfp-0.0.1.dev9/doc/
--rw-r--r--   0 eres      (1000) eres      (1000)      452 2024-04-30 07:31:27.000000 data_prep_toolkit_kfp-0.0.1.dev9/doc/kfp_support_library.md
--rw-r--r--   0 eres      (1000) eres      (1000)     1245 2024-05-12 13:27:47.000000 data_prep_toolkit_kfp-0.0.1.dev9/pyproject.toml
--rw-r--r--   0 eres      (1000) eres      (1000)       38 2024-05-12 13:30:25.632277 data_prep_toolkit_kfp-0.0.1.dev9/setup.cfg
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 13:30:25.602277 data_prep_toolkit_kfp-0.0.1.dev9/src/
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 13:30:25.622277 data_prep_toolkit_kfp-0.0.1.dev9/src/data_prep_toolkit_kfp.egg-info/
--rw-r--r--   0 eres      (1000) eres      (1000)     2737 2024-05-12 13:30:23.000000 data_prep_toolkit_kfp-0.0.1.dev9/src/data_prep_toolkit_kfp.egg-info/PKG-INFO
--rw-r--r--   0 eres      (1000) eres      (1000)     1226 2024-05-12 13:30:25.000000 data_prep_toolkit_kfp-0.0.1.dev9/src/data_prep_toolkit_kfp.egg-info/SOURCES.txt
--rw-r--r--   0 eres      (1000) eres      (1000)        1 2024-05-12 13:30:23.000000 data_prep_toolkit_kfp-0.0.1.dev9/src/data_prep_toolkit_kfp.egg-info/dependency_links.txt
--rw-r--r--   0 eres      (1000) eres      (1000)      189 2024-05-12 13:30:23.000000 data_prep_toolkit_kfp-0.0.1.dev9/src/data_prep_toolkit_kfp.egg-info/requires.txt
--rw-r--r--   0 eres      (1000) eres      (1000)       12 2024-05-12 13:30:23.000000 data_prep_toolkit_kfp-0.0.1.dev9/src/data_prep_toolkit_kfp.egg-info/top_level.txt
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 13:30:25.602277 data_prep_toolkit_kfp-0.0.1.dev9/src/kfp_support/
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 13:30:25.612277 data_prep_toolkit_kfp-0.0.1.dev9/src/kfp_support/api_server_client/
--rw-r--r--   0 eres      (1000) eres      (1000)      238 2024-04-30 07:31:27.000000 data_prep_toolkit_kfp-0.0.1.dev9/src/kfp_support/api_server_client/README.md
--rw-r--r--   0 eres      (1000) eres      (1000)       67 2024-04-30 07:31:27.000000 data_prep_toolkit_kfp-0.0.1.dev9/src/kfp_support/api_server_client/__init__.py
--rw-r--r--   0 eres      (1000) eres      (1000)    26996 2024-04-30 07:31:27.000000 data_prep_toolkit_kfp-0.0.1.dev9/src/kfp_support/api_server_client/kuberay_apis.py
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 13:30:25.622277 data_prep_toolkit_kfp-0.0.1.dev9/src/kfp_support/api_server_client/params/
--rw-r--r--   0 eres      (1000) eres      (1000)     1259 2024-04-30 07:31:27.000000 data_prep_toolkit_kfp-0.0.1.dev9/src/kfp_support/api_server_client/params/__init__.py
--rw-r--r--   0 eres      (1000) eres      (1000)    11445 2024-04-30 07:31:27.000000 data_prep_toolkit_kfp-0.0.1.dev9/src/kfp_support/api_server_client/params/cluster.py
--rw-r--r--   0 eres      (1000) eres      (1000)     5390 2024-04-30 07:31:27.000000 data_prep_toolkit_kfp-0.0.1.dev9/src/kfp_support/api_server_client/params/environmentvariables.py
--rw-r--r--   0 eres      (1000) eres      (1000)     7528 2024-04-30 07:31:27.000000 data_prep_toolkit_kfp-0.0.1.dev9/src/kfp_support/api_server_client/params/headnode.py
--rw-r--r--   0 eres      (1000) eres      (1000)     6367 2024-04-30 07:31:27.000000 data_prep_toolkit_kfp-0.0.1.dev9/src/kfp_support/api_server_client/params/jobsubmission.py
--rw-r--r--   0 eres      (1000) eres      (1000)     7491 2024-04-30 07:31:27.000000 data_prep_toolkit_kfp-0.0.1.dev9/src/kfp_support/api_server_client/params/templates.py
--rw-r--r--   0 eres      (1000) eres      (1000)    14921 2024-04-30 07:31:27.000000 data_prep_toolkit_kfp-0.0.1.dev9/src/kfp_support/api_server_client/params/volumes.py
--rw-r--r--   0 eres      (1000) eres      (1000)     7884 2024-04-30 07:31:27.000000 data_prep_toolkit_kfp-0.0.1.dev9/src/kfp_support/api_server_client/params/workernode.py
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 13:30:25.622277 data_prep_toolkit_kfp-0.0.1.dev9/src/kfp_support/workflow_support/
--rw-r--r--   0 eres      (1000) eres      (1000)     2698 2024-04-30 07:31:27.000000 data_prep_toolkit_kfp-0.0.1.dev9/src/kfp_support/workflow_support/README.md
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 13:30:25.622277 data_prep_toolkit_kfp-0.0.1.dev9/src/kfp_support/workflow_support/utils/
--rw-r--r--   0 eres      (1000) eres      (1000)      192 2024-04-30 07:31:27.000000 data_prep_toolkit_kfp-0.0.1.dev9/src/kfp_support/workflow_support/utils/__init__.py
--rw-r--r--   0 eres      (1000) eres      (1000)     3913 2024-05-09 06:08:06.000000 data_prep_toolkit_kfp-0.0.1.dev9/src/kfp_support/workflow_support/utils/pipelines_tests_utils.py
--rw-r--r--   0 eres      (1000) eres      (1000)    27816 2024-05-12 13:25:58.000000 data_prep_toolkit_kfp-0.0.1.dev9/src/kfp_support/workflow_support/utils/workflow_utils.py
-drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 13:30:25.622277 data_prep_toolkit_kfp-0.0.1.dev9/test/
--rw-r--r--   0 eres      (1000) eres      (1000)    14416 2024-04-30 07:31:27.000000 data_prep_toolkit_kfp-0.0.1.dev9/test/api_params_test.py
--rw-r--r--   0 eres      (1000) eres      (1000)     2319 2024-04-30 07:31:27.000000 data_prep_toolkit_kfp-0.0.1.dev9/test/configmaps.py
--rw-r--r--   0 eres      (1000) eres      (1000)     9967 2024-04-30 07:31:27.000000 data_prep_toolkit_kfp-0.0.1.dev9/test/kuberay_api_test.py
--rw-r--r--   0 eres      (1000) eres      (1000)     1401 2024-04-30 07:31:27.000000 data_prep_toolkit_kfp-0.0.1.dev9/test/pipeline_utils_test.py
--rw-r--r--   0 eres      (1000) eres      (1000)     3154 2024-04-30 07:31:27.000000 data_prep_toolkit_kfp-0.0.1.dev9/test/ray_remote_jobs_test.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-16 11:57:59.588148 data_prep_toolkit_kfp-0.1.0/
+-rw-r--r--   0 boris      (501) staff       (20)     2117 2024-05-11 12:34:39.000000 data_prep_toolkit_kfp-0.1.0/Makefile
+-rw-r--r--   0 boris      (501) staff       (20)     2697 2024-05-16 11:57:59.587280 data_prep_toolkit_kfp-0.1.0/PKG-INFO
+-rw-r--r--   0 boris      (501) staff       (20)     1890 2024-05-14 14:33:32.000000 data_prep_toolkit_kfp-0.1.0/README.md
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-16 11:57:59.568707 data_prep_toolkit_kfp-0.1.0/doc/
+-rw-r--r--   0 boris      (501) staff       (20)      452 2024-05-11 12:34:39.000000 data_prep_toolkit_kfp-0.1.0/doc/kfp_support_library.md
+-rw-r--r--   0 boris      (501) staff       (20)     1212 2024-05-16 11:56:24.000000 data_prep_toolkit_kfp-0.1.0/pyproject.toml
+-rw-r--r--   0 boris      (501) staff       (20)       38 2024-05-16 11:57:59.588354 data_prep_toolkit_kfp-0.1.0/setup.cfg
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-16 11:57:59.565975 data_prep_toolkit_kfp-0.1.0/src/
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-16 11:57:59.584607 data_prep_toolkit_kfp-0.1.0/src/data_prep_toolkit_kfp.egg-info/
+-rw-r--r--   0 boris      (501) staff       (20)     2697 2024-05-16 11:57:59.000000 data_prep_toolkit_kfp-0.1.0/src/data_prep_toolkit_kfp.egg-info/PKG-INFO
+-rw-r--r--   0 boris      (501) staff       (20)     1226 2024-05-16 11:57:59.000000 data_prep_toolkit_kfp-0.1.0/src/data_prep_toolkit_kfp.egg-info/SOURCES.txt
+-rw-r--r--   0 boris      (501) staff       (20)        1 2024-05-16 11:57:59.000000 data_prep_toolkit_kfp-0.1.0/src/data_prep_toolkit_kfp.egg-info/dependency_links.txt
+-rw-r--r--   0 boris      (501) staff       (20)      168 2024-05-16 11:57:59.000000 data_prep_toolkit_kfp-0.1.0/src/data_prep_toolkit_kfp.egg-info/requires.txt
+-rw-r--r--   0 boris      (501) staff       (20)       12 2024-05-16 11:57:59.000000 data_prep_toolkit_kfp-0.1.0/src/data_prep_toolkit_kfp.egg-info/top_level.txt
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-16 11:57:59.566596 data_prep_toolkit_kfp-0.1.0/src/kfp_support/
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-16 11:57:59.573253 data_prep_toolkit_kfp-0.1.0/src/kfp_support/api_server_client/
+-rw-r--r--   0 boris      (501) staff       (20)      238 2024-05-11 12:34:39.000000 data_prep_toolkit_kfp-0.1.0/src/kfp_support/api_server_client/README.md
+-rw-r--r--   0 boris      (501) staff       (20)       67 2024-05-11 12:34:39.000000 data_prep_toolkit_kfp-0.1.0/src/kfp_support/api_server_client/__init__.py
+-rw-r--r--   0 boris      (501) staff       (20)    27135 2024-05-16 11:46:39.000000 data_prep_toolkit_kfp-0.1.0/src/kfp_support/api_server_client/kuberay_apis.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-16 11:57:59.578667 data_prep_toolkit_kfp-0.1.0/src/kfp_support/api_server_client/params/
+-rw-r--r--   0 boris      (501) staff       (20)     1307 2024-05-16 11:46:39.000000 data_prep_toolkit_kfp-0.1.0/src/kfp_support/api_server_client/params/__init__.py
+-rw-r--r--   0 boris      (501) staff       (20)    17734 2024-05-16 11:46:39.000000 data_prep_toolkit_kfp-0.1.0/src/kfp_support/api_server_client/params/cluster.py
+-rw-r--r--   0 boris      (501) staff       (20)     5390 2024-05-11 12:34:39.000000 data_prep_toolkit_kfp-0.1.0/src/kfp_support/api_server_client/params/environmentvariables.py
+-rw-r--r--   0 boris      (501) staff       (20)     8063 2024-05-16 11:46:39.000000 data_prep_toolkit_kfp-0.1.0/src/kfp_support/api_server_client/params/headnode.py
+-rw-r--r--   0 boris      (501) staff       (20)     6367 2024-05-11 12:34:39.000000 data_prep_toolkit_kfp-0.1.0/src/kfp_support/api_server_client/params/jobsubmission.py
+-rw-r--r--   0 boris      (501) staff       (20)     7491 2024-05-11 12:34:39.000000 data_prep_toolkit_kfp-0.1.0/src/kfp_support/api_server_client/params/templates.py
+-rw-r--r--   0 boris      (501) staff       (20)    14921 2024-05-11 12:34:39.000000 data_prep_toolkit_kfp-0.1.0/src/kfp_support/api_server_client/params/volumes.py
+-rw-r--r--   0 boris      (501) staff       (20)     8441 2024-05-16 11:46:39.000000 data_prep_toolkit_kfp-0.1.0/src/kfp_support/api_server_client/params/workernode.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-16 11:57:59.579091 data_prep_toolkit_kfp-0.1.0/src/kfp_support/workflow_support/
+-rw-r--r--   0 boris      (501) staff       (20)     2698 2024-05-11 12:34:39.000000 data_prep_toolkit_kfp-0.1.0/src/kfp_support/workflow_support/README.md
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-16 11:57:59.581297 data_prep_toolkit_kfp-0.1.0/src/kfp_support/workflow_support/utils/
+-rw-r--r--   0 boris      (501) staff       (20)      192 2024-05-11 12:34:39.000000 data_prep_toolkit_kfp-0.1.0/src/kfp_support/workflow_support/utils/__init__.py
+-rw-r--r--   0 boris      (501) staff       (20)     3116 2024-05-15 14:10:05.000000 data_prep_toolkit_kfp-0.1.0/src/kfp_support/workflow_support/utils/pipelines_tests_utils.py
+-rw-r--r--   0 boris      (501) staff       (20)    30850 2024-05-16 11:46:39.000000 data_prep_toolkit_kfp-0.1.0/src/kfp_support/workflow_support/utils/workflow_utils.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-16 11:57:59.583973 data_prep_toolkit_kfp-0.1.0/test/
+-rw-r--r--   0 boris      (501) staff       (20)    15224 2024-05-16 11:46:39.000000 data_prep_toolkit_kfp-0.1.0/test/api_params_test.py
+-rw-r--r--   0 boris      (501) staff       (20)     2319 2024-05-11 12:34:39.000000 data_prep_toolkit_kfp-0.1.0/test/configmaps.py
+-rw-r--r--   0 boris      (501) staff       (20)    10486 2024-05-16 11:46:39.000000 data_prep_toolkit_kfp-0.1.0/test/kuberay_api_test.py
+-rw-r--r--   0 boris      (501) staff       (20)     1401 2024-05-11 12:34:39.000000 data_prep_toolkit_kfp-0.1.0/test/pipeline_utils_test.py
+-rw-r--r--   0 boris      (501) staff       (20)     3232 2024-05-16 11:46:39.000000 data_prep_toolkit_kfp-0.1.0/test/ray_remote_jobs_test.py
```

### Comparing `data_prep_toolkit_kfp-0.0.1.dev9/Makefile` & `data_prep_toolkit_kfp-0.1.0/Makefile`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev9/PKG-INFO` & `data_prep_toolkit_kfp-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: data_prep_toolkit_kfp
-Version: 0.0.1.dev9
+Version: 0.1.0
 Summary: Data Preparation Kit Library. KFP support
 Author-email: Boris Lublinsky <blublinsky@ibm.com>, Alexey Roytman <roytman@il.ibm.com>, Mohammad Nassar <Mohammad.Nassar@ibm.com>, Revital Eres <eres@il.ibm.com>
 License: Apache-2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: kfp==2.7.0
-Requires-Dist: kfp-kubernetes==1.2.0
+Requires-Dist: kfp==1.8.22
 Requires-Dist: requests
-Requires-Dist: data-prep-toolkit==0.0.1
+Requires-Dist: data-prep-toolkit==0.1.0
 Provides-Extra: dev
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: pytest>=7.3.2; extra == "dev"
 Requires-Dist: pytest-dotenv>=0.5.2; extra == "dev"
 Requires-Dist: pytest-env>=1.0.0; extra == "dev"
 Requires-Dist: pre-commit>=3.3.2; extra == "dev"
 Requires-Dist: pytest-cov>=4.1.0; extra == "dev"
 Requires-Dist: pytest-mock>=3.10.0; extra == "dev"
 
 # KFP support library
 
 This provides support for implementing KFP pipelines automating transform's execution.
 It comprises 2 main modules
+
 * [api server client](src/kfp_support/api_server_client/README.md) 
 * [workflow support](src/kfp_support/workflow_support/README.md)
 
 ## Development
 
 ### Requirements
 1. python 3.10 or later
```

### Comparing `data_prep_toolkit_kfp-0.0.1.dev9/README.md` & `data_prep_toolkit_kfp-0.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # KFP support library
 
 This provides support for implementing KFP pipelines automating transform's execution.
 It comprises 2 main modules
+
 * [api server client](src/kfp_support/api_server_client/README.md) 
 * [workflow support](src/kfp_support/workflow_support/README.md)
 
 ## Development
 
 ### Requirements
 1. python 3.10 or later
```

### Comparing `data_prep_toolkit_kfp-0.0.1.dev9/pyproject.toml` & `data_prep_toolkit_kfp-0.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 [project]
 name = "data_prep_toolkit_kfp"
-version = "0.0.1-dev9"
+version = "0.1.0"
 requires-python = ">=3.10"
 description = "Data Preparation Kit Library. KFP support"
 license = {text = "Apache-2.0"}
 readme = {file = "README.md", content-type = "text/markdown"}
 authors = [
     { name = "Boris Lublinsky", email = "blublinsky@ibm.com" },
     { name = "Alexey Roytman", email = "roytman@il.ibm.com" },
     { name = "Mohammad Nassar", email = "Mohammad.Nassar@ibm.com" },
     { name = "Revital Eres", email = "eres@il.ibm.com" },
 ]
 dependencies = [
-    "kfp==2.7.0",
-    "kfp-kubernetes==1.2.0",
+    "kfp==1.8.22",
     "requests",
-    "data-prep-toolkit==0.0.1",
+    "data-prep-toolkit==0.1.0",
 ]
 
 [build-system]
 requires = ["setuptools>=68.0.0", "wheel", "setuptools_scm[toml]>=7.1.0"]
 build-backend = "setuptools.build_meta"
 
 [project.optional-dependencies]
```

### Comparing `data_prep_toolkit_kfp-0.0.1.dev9/src/data_prep_toolkit_kfp.egg-info/PKG-INFO` & `data_prep_toolkit_kfp-0.1.0/src/data_prep_toolkit_kfp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: data_prep_toolkit_kfp
-Version: 0.0.1.dev9
+Version: 0.1.0
 Summary: Data Preparation Kit Library. KFP support
 Author-email: Boris Lublinsky <blublinsky@ibm.com>, Alexey Roytman <roytman@il.ibm.com>, Mohammad Nassar <Mohammad.Nassar@ibm.com>, Revital Eres <eres@il.ibm.com>
 License: Apache-2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: kfp==2.7.0
-Requires-Dist: kfp-kubernetes==1.2.0
+Requires-Dist: kfp==1.8.22
 Requires-Dist: requests
-Requires-Dist: data-prep-toolkit==0.0.1
+Requires-Dist: data-prep-toolkit==0.1.0
 Provides-Extra: dev
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: pytest>=7.3.2; extra == "dev"
 Requires-Dist: pytest-dotenv>=0.5.2; extra == "dev"
 Requires-Dist: pytest-env>=1.0.0; extra == "dev"
 Requires-Dist: pre-commit>=3.3.2; extra == "dev"
 Requires-Dist: pytest-cov>=4.1.0; extra == "dev"
 Requires-Dist: pytest-mock>=3.10.0; extra == "dev"
 
 # KFP support library
 
 This provides support for implementing KFP pipelines automating transform's execution.
 It comprises 2 main modules
+
 * [api server client](src/kfp_support/api_server_client/README.md) 
 * [workflow support](src/kfp_support/workflow_support/README.md)
 
 ## Development
 
 ### Requirements
 1. python 3.10 or later
```

### Comparing `data_prep_toolkit_kfp-0.0.1.dev9/src/data_prep_toolkit_kfp.egg-info/SOURCES.txt` & `data_prep_toolkit_kfp-0.1.0/src/data_prep_toolkit_kfp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev9/src/kfp_support/api_server_client/kuberay_apis.py` & `data_prep_toolkit_kfp-0.1.0/src/kfp_support/api_server_client/kuberay_apis.py`

 * *Files 0% similar despite different names*

```diff
@@ -455,15 +455,15 @@
                     )
                     status = response.status_code
                     message = response.json()["message"]
             except Exception as e:
                 logger.warning(f"Failed to submit job to the cluster {name} in namespace {ns}, exception : {e}")
                 status = 500
                 message = str(e)
-            time.sleep(1)
+            time.sleep(5)
         return status, message, None
 
     def get_job_info(self, ns: str, name: str, sid: str) -> tuple[int, str, RayJobInfo]:
         """
         get Ray job details
         :param ns: namespace of the cluster
         :param name: name of the cluster
@@ -511,27 +511,30 @@
         # Execute HTTP request
         url = self.server_url + self.api_base + f"namespaces/{ns}/jobsubmissions/{name}"
         for i in range(self.http_retries):
             try:
                 response = requests.get(url, headers=_headers, timeout=TIMEOUT)
                 if response.status_code // 100 == 2:
                     job_info_array = response.json().get("submissions", None)
-                    return response.status_code, None, [RayJobInfo(i) for i in job_info_array]
+                    if job_info_array is None:
+                        return response.status_code, None, []
+                    else:
+                        return response.status_code, None, [RayJobInfo(i) for i in job_info_array]
                 else:
                     logger.warning(
                         f"Failed to list jobs from the cluster {name} in namespace {ns}, "
                         f"status : {response.status_code}"
                     )
                     status = response.status_code
                     message = response.json()["message"]
             except Exception as e:
                 logger.warning(f"Failed to list jobs from the cluster {name} in namespace {ns}, exception : {e}")
                 status = 500
                 message = str(e)
-            time.sleep(1)
+            time.sleep(5)
         return status, message, []
 
     def get_job_log(self, ns: str, name: str, sid: str) -> tuple[int, str, str]:
         """
         get Ray job log
         :param ns: namespace of the cluster
         :param name: name of the cluster
```

### Comparing `data_prep_toolkit_kfp-0.0.1.dev9/src/kfp_support/api_server_client/params/__init__.py` & `data_prep_toolkit_kfp-0.1.0/src/kfp_support/api_server_client/params/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,17 @@
 from kfp_support.api_server_client.params.workernode import (
     WorkerNodeSpec,
     DEFAULT_WORKER_START_PARAMS,
     worker_node_spec_decoder,
 )
 from kfp_support.api_server_client.params.cluster import (
     Environment,
+    AutoscalerOptions,
     ClusterSpec,
     ClusterEvent,
     Cluster,
+    autoscaling_decoder,
     cluster_spec_decoder,
     cluster_decoder,
     clusters_decoder,
 )
 from kfp_support.api_server_client.params.jobsubmission import RayJobRequest, RayJobInfo
```

### Comparing `data_prep_toolkit_kfp-0.0.1.dev9/src/kfp_support/api_server_client/params/environmentvariables.py` & `data_prep_toolkit_kfp-0.1.0/src/kfp_support/api_server_client/params/environmentvariables.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev9/src/kfp_support/api_server_client/params/headnode.py` & `data_prep_toolkit_kfp-0.1.0/src/kfp_support/api_server_client/params/headnode.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,14 +48,15 @@
         enable_ingress - optional, allow to enable ingress for dashboard
         volumes - optional, a list of volumes to attach to head node
         service_account - optional, a service account (has to exist) to run head node
         image_pull_secret - optional, secret to pull head node image from registry
         environment - optional, environment variables for head pod
         annotations - optional, annotations for head node
         labels - optional, labels for head node
+        image_pull_policy - optional, head node pull image policy. Default IfNotPresent
     """
 
     def __init__(
         self,
         compute_template: str,
         image: str,
         ray_start_params: dict[str, str] = DEFAULT_HEAD_START_PARAMS,
@@ -63,42 +64,45 @@
         enable_ingress: bool = False,
         volumes: list[BaseVolume] = None,
         service_account: str = None,
         image_pull_secret: str = None,
         environment: EnvironmentVariables = None,
         annotations: dict[str, str] = None,
         labels: dict[str, str] = None,
+        image_pull_policy: str = None,
     ):
         """
         Initialization
         :param compute_template: compute template
         :param ray_start_params:  ray start parameters
         :param image: node image
         :param service_type: service type
         :param enable_ingress: enable ingress flag
         :param volumes:  volumes for head node
         :param service_account: service account
         :param image_pull_secret:  image pull secret
         :param environment: head node environment
         :param annotations: head node annotation
         :param labels: labels
+        :param image_pull_policy: image pull policy
         """
 
         self.compute_template = compute_template
         self.ray_start_params = ray_start_params
         self.ray_start_params.update(DEFAULT_HEAD_START_PARAMS)
         self.image = image
         self.service_type = service_type
         self.enable_ingress = enable_ingress
         self.volumes = volumes
         self.service_account = service_account
         self.image_pull_secret = image_pull_secret
         self.environment = environment
         self.annotations = annotations
         self.labels = labels
+        self.image_pull_policy = image_pull_policy
 
     def to_string(self) -> str:
         """
         Convert to string
         :return: string representation of the head node
         """
         val = f"compute template = {self.compute_template}, ray start params = {str(self.ray_start_params)}"
@@ -108,14 +112,16 @@
             val += f", service_type = {self.service_type.name}"
         if self.enable_ingress:
             val += ", enable_ingress = True"
         if self.service_account is not None:
             val += f", service_account = {self.service_account}"
         if self.image_pull_secret is not None:
             val += f", image_pull_secret = {self.image_pull_secret}"
+        if self.image_pull_policy is not None:
+            val += f", image_pull_policy = {self.image_pull_policy}"
         if self.volumes is not None:
             val = val + ",\n volumes = ["
             first = True
             for v in self.volumes:
                 if first:
                     first = False
                 else:
@@ -142,14 +148,16 @@
             dct["serviceType"] = self.service_type.value
         if self.enable_ingress:
             dct["enableIngress"] = True
         if self.service_account is not None:
             dct["service_account"] = self.service_account
         if self.image_pull_secret is not None:
             dct["image_pull_secret"] = self.image_pull_secret
+        if self.image_pull_policy is not None:
+            dct["imagePullPolicy"] = self.image_pull_policy
         if self.volumes is not None:
             dct["volumes"] = [v.to_dict() for v in self.volumes]
         if self.environment is not None:
             dct["environment"] = self.environment.to_dict()
         if self.annotations is not None:
             dct["annotations"] = self.annotations
         if self.labels is not None:
@@ -181,13 +189,14 @@
     return HeadNodeSpec(
         compute_template=dct.get("computeTemplate"),
         ray_start_params=dct.get("rayStartParams"),
         image=dct.get("image"),
         service_type=service_type,
         enable_ingress=dct.get("enableIngress", False),
         volumes=volumes,
-        service_account=dct.get("service_account"),
-        image_pull_secret=dct.get("image_pull_secret"),
+        service_account=dct.get("service_account", None),
+        image_pull_secret=dct.get("imagePullSecret", None),
+        image_pull_policy=dct.get("imagePullPolicy", None),
         environment=environments,
-        annotations=dct.get("annotations"),
-        labels=dct.get("labels"),
+        annotations=dct.get("annotations", None),
+        labels=dct.get("labels", None),
     )
```

### Comparing `data_prep_toolkit_kfp-0.0.1.dev9/src/kfp_support/api_server_client/params/jobsubmission.py` & `data_prep_toolkit_kfp-0.1.0/src/kfp_support/api_server_client/params/jobsubmission.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev9/src/kfp_support/api_server_client/params/templates.py` & `data_prep_toolkit_kfp-0.1.0/src/kfp_support/api_server_client/params/templates.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev9/src/kfp_support/api_server_client/params/volumes.py` & `data_prep_toolkit_kfp-0.1.0/src/kfp_support/api_server_client/params/volumes.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev9/src/kfp_support/api_server_client/params/workernode.py` & `data_prep_toolkit_kfp-0.1.0/src/kfp_support/api_server_client/params/workernode.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,26 +27,27 @@
     """
     WorkerNodeSpec is used to define Ray cluster worker node pool configuration.
     It provides APIs to create, stringify and convert to dict.
 
     Methods:
     - Create worker node pool specification: gets the following parameters:
         group_name - required, group name of the worker group
-        compute_template - required, the computeTemplate of head node group
+        compute_template - required, the computeTemplate of worker node group
         replicas - required, desired replicas of the worker group
         min_replicas - required Min replicas of the worker group, can't be greater than max_replicas
         max_replicas - required, max replicas of the worker group
         ray_start_params - required, Ray start parameters
-        image - optional, image used for head node
-        volumes - optional, a list of volumes to attach to head node
-        service_account - optional, a service account (has to exist) to run head node
-        image_pull_secret - optional, secret to pull head node image from registry
-        environment - optional, environment variables for head pod
-        annotations - optional, annotations for head node
-        labels - optional, labels for head node
+        image - optional, image used for worker node
+        volumes - optional, a list of volumes to attach to worker node
+        service_account - optional, a service account (has to exist) to run worker node
+        image_pull_secret - optional, secret to pull worker node image from registry
+        environment - optional, environment variables for worker pod
+        annotations - optional, annotations for worker node
+        labels - optional, labels for worker node
+        image_pull_policy - optional, worker node pull image policy. Default IfNotPresent
     """
 
     def __init__(
         self,
         group_name: str,
         compute_template: str,
         image: str,
@@ -56,14 +57,15 @@
         ray_start_params: dict[str, str] = DEFAULT_WORKER_START_PARAMS,
         volumes: list[BaseVolume] = None,
         service_account: str = None,
         image_pull_secret: str = None,
         environment: EnvironmentVariables = None,
         annotations: dict[str, str] = None,
         labels: dict[str, str] = None,
+        image_pull_policy: str = None,
     ):
         """
         Initialization
         :param group_name: name
         :param compute_template: compute template
         :param replicas: number of replicas
         :param min_replicas: min number of replicas
@@ -72,14 +74,15 @@
         :param image: image name
         :param volumes: volumes
         :param service_account: service account
         :param image_pull_secret: image pull secret
         :param environment: environment
         :param annotations: annotations
         :param labels: labels
+        :param image_pull_policy: image pull policy
         """
         # Validate replicas
         if min_replicas > replicas:
             raise RuntimeError(f"min_replicas {min_replicas} is can't be greater then replicas {replicas} ")
         if replicas > max_replicas:
             raise RuntimeError(f"replicas {replicas} is can't be greater then max_replicas {max_replicas} ")
 
@@ -93,14 +96,15 @@
         self.image = image
         self.volumes = volumes
         self.service_account = service_account
         self.image_pull_secret = image_pull_secret
         self.environment = environment
         self.annotations = annotations
         self.labels = labels
+        self.image_pull_policy = image_pull_policy
 
     def to_string(self) -> str:
         """
         Convert to string
         :return: string representation of worker node spec
         """
         val = (
@@ -110,14 +114,16 @@
         )
         if self.image is not None:
             val += f", image = {self.image}"
         if self.service_account is not None:
             val += f", service_account = {self.service_account}"
         if self.image_pull_secret is not None:
             val += f", image_pull_secret = {self.image_pull_secret}"
+        if self.image_pull_policy is not None:
+            val += f", image_pull_policy = {self.image_pull_policy}"
         if self.volumes is not None:
             val = val + ",\n volumes = ["
             first = True
             for v in self.volumes:
                 if first:
                     first = False
                 else:
@@ -147,27 +153,29 @@
         }
         if self.image is not None:
             dct["image"] = self.image
         if self.service_account is not None:
             dct["service_account"] = self.service_account
         if self.image_pull_secret is not None:
             dct["imagePullSecret"] = self.image_pull_secret
+        if self.image_pull_policy is not None:
+            dct["imagePullPolicy"] = self.image_pull_policy
         if self.volumes is not None:
             dct["volumes"] = [v.to_dict() for v in self.volumes]
         if self.environment is not None:
             dct["environment"] = self.environment.to_dict()
         if self.annotations is not None:
             dct["annotations"] = self.annotations
         if self.labels is not None:
             dct["labels"] = self.labels
         return dct
 
 
 """
-    Creates new head node from dictionary, used for unmarshalling json. Python does not
+    Creates new worker node from dictionary, used for unmarshalling json. Python does not
     support multiple constructors, so do it this way
 """
 
 
 def worker_node_spec_decoder(dct: dict[str, Any]) -> WorkerNodeSpec:
     """
     Create worker node spec from dictionary
@@ -185,13 +193,14 @@
         compute_template=dct.get("computeTemplate"),
         replicas=dct.get("replicas", 0),
         min_replicas=dct.get("minReplicas", 0),
         max_replicas=dct.get("maxReplicas", 0),
         ray_start_params=dct.get("rayStartParams"),
         image=dct.get("image"),
         volumes=volumes,
-        service_account=dct.get("service_account"),
-        image_pull_secret=dct.get("imagePullSecret"),
+        service_account=dct.get("service_account", None),
+        image_pull_secret=dct.get("imagePullSecret", None),
+        image_pull_policy=dct.get("imagePullPolicy", None),
         environment=environments,
-        annotations=dct.get("annotations"),
-        labels=dct.get("labels"),
+        annotations=dct.get("annotations", None),
+        labels=dct.get("labels", None),
     )
```

### Comparing `data_prep_toolkit_kfp-0.0.1.dev9/src/kfp_support/workflow_support/README.md` & `data_prep_toolkit_kfp-0.1.0/src/kfp_support/workflow_support/README.md`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev9/src/kfp_support/workflow_support/utils/workflow_utils.py` & `data_prep_toolkit_kfp-0.1.0/src/kfp_support/workflow_support/utils/workflow_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,27 +31,26 @@
     HeadNodeSpec,
     RayJobRequest,
     Template,
     WorkerNodeSpec,
     environment_variables_decoder,
     volume_decoder,
 )
+from kubernetes import client as k8s_client
 from ray.job_submission import JobStatus
 
-from kfp import Client, kubernetes
-from kubernetes import client as k8s_client
+from kfp import Client
 
 
 logger = get_logger(__name__)
 
 ONE_HOUR_SEC = 60 * 60
 ONE_DAY_SEC = ONE_HOUR_SEC * 24
 ONE_WEEK_SEC = ONE_DAY_SEC * 7
 
-RUN_NAME = "KFP_RUN_NAME"
 
 class KFPUtils:
     """
     Helper utilities for KFP implementations
     """
 
     @staticmethod
@@ -140,51 +139,101 @@
     def __init__(self, host: str = "http://localhost:8080"):
         """
         Initialization
         :param host: host to connect to
         """
         self.kfp_client = Client(host=host)
 
+    def upload_pipeline(
+        self,
+        pipeline_package_path: str = None,
+        pipeline_name: str = None,
+        overwrite: bool = False,
+        description: str = None,
+    ) -> models.api_pipeline.ApiPipeline:
+        """
+        Uploads the pipeline
+        :param pipeline_package_path: Local path to the pipeline package.
+        :param pipeline_name: Optional. Name of the pipeline to be shown in the UI
+        :param overwrite: Optional. If pipeline exists, delete it before creating a new one.
+        :param description: Optional. Description of the pipeline to be shown in the UI.
+        :return: Server response object containing pipeline id and other information.
+        """
+        pipeline = None
+        if overwrite:
+            pipeline = self.get_pipeline_by_name(name=pipeline_name)
+            if pipeline is not None:
+                try:
+                    logger.info(f"pipeline {pipeline_name} already exists. Trying to delete it.")
+                    self.kfp_client.delete_pipeline(pipeline_id=pipeline.id)
+                except Exception as e:
+                    logger.warning(f"Exception deleting pipeline {e} before uploading")
+                    return None
+        try:
+            pipeline = self.kfp_client.upload_pipeline(
+                pipeline_package_path=pipeline_package_path, pipeline_name=pipeline_name, description=description
+            )
+        except Exception as e:
+            logger.warning(f"Exception uploading pipeline {e}")
+            return None
+        if pipeline is None:
+            logger.warning(f"Failed to upload pipeline {pipeline_name}.")
+            return None
+        logger.info("Pipeline uploaded")
+        return pipeline
+
+    def delete_pipeline(self, pipeline_id):
+        """
+        Delete pipeline.
+        :param pipeline_id: id of the pipeline.
+        :return
+        Returns:
+          Object. If the method is called asynchronously, returns the request thread.
+        Raises:
+          kfp_server_api.ApiException: If pipeline is not found.
+        """
+        return self.kfp_client.delete_pipeline(pipeline_id)
+
     def start_pipeline(
         self,
-        pipeline: kfp_server_api.V2beta1Pipeline,
-        experiment: kfp_server_api.V2beta1Experiment,
+        pipeline: models.api_pipeline.ApiPipeline,
+        experiment: models.api_experiment.ApiExperiment,
         params: Optional[dict[str, Any]],
     ) -> str:
         """
         Start a specified pipeline.
         :param pipeline: pipeline definition
         :param experiment: experiment to use
         :param params: pipeline parameters
         :return: the id of the run object
         """
         job_name = pipeline.name + " " + datetime.datetime.now().strftime("%Y_%m_%d_%H_%M_%S")
         try:
             run_id = self.kfp_client.run_pipeline(
                 experiment_id=experiment.id, job_name=job_name, pipeline_id=pipeline.id, params=params
             )
-            logger.info("Pipeline submitted")
+            logger.info(f"Pipeline run {job_name} submitted")
             return run_id.id
         except Exception as e:
             logger.warning(f"Exception starting pipeline {e}")
             return None
 
-    def get_experiment_by_name(self, name: str = "Default") -> kfp_server_api.V2beta1Experiment:
+    def get_experiment_by_name(self, name: str = "Default") -> models.api_experiment.ApiExperiment:
         """
         Get experiment by name
         :param name: name
         :return: experiment
         """
         try:
             return self.kfp_client.get_experiment(experiment_name=name)
         except Exception as e:
             logger.warning(f"Exception getting experiment {e}")
             return None
 
-    def get_pipeline_by_name(self, name: str, np: int = 100) -> kfp_server_api.V2beta1Pipeline:
+    def get_pipeline_by_name(self, name: str, np: int = 100) -> models.api_pipeline.ApiPipeline:
         """
         Given pipeline name, return the pipeline
         :param name: pipeline name
         :param np: page size for pipeline query. For large clusters with many pipelines, you might need to
                    increase this number
         :return: pipeline
         """
@@ -282,14 +331,15 @@
                 image_pull_secret - image pull secret
                 ray_start_params - dictionary of ray start parameters
                 volumes - list of volumes for head node
                 service_account - service account to use (has to be created)
                 environment - dictionary of head node environment
                 annotations: dictionary of head node annotation
                 labels: dictionary of head node labels
+                image_pull_policy: image pull policy, default IfNotPresent
 
         :param worker_nodes: an array of worker node specification dictionary including the following:
             mandatory fields:
                 cpu - number of cpus
                 memory memory size (GB)
                 image - image to use
                 max_replicas - max replicas for this worker group
@@ -301,14 +351,16 @@
                 image_pull_secret - image pull secret
                 ray_start_params - dictionary of ray start parameters
                 volumes - list of volumes for this group
                 service_account - service account to use (has to be created)
                 environment - dictionary of node of this group environment
                 annotations: dictionary of node of this group annotation
                 labels: dictionary of node of this group labels
+                image_pull_policy: image pull policy, default IfNotPresent
+
         :param wait_cluster_ready - time to wait for cluster ready sec (-1 forever)
         :return:tuple containing
             http return code
             message - only returned if http return code is not equal to 200
         """
         # start with templates
         # head_node
@@ -351,14 +403,15 @@
             if status != 200:
                 return status, error
             worker_template_names[index] = worker_node_template_name
             index += 1
         # Build head node spec
         image = head_node.get("image", self.default_image)
         image_pull_secret = head_node.get("image_pull_secret", None)
+        image_pull_policy = head_node.get("image_pull_policy", None)
         ray_start_params = head_node.get("ray_start_params", DEFAULT_HEAD_START_PARAMS)
         volumes_dict = head_node.get("volumes", None)
         service_account = head_node.get("service_account", None)
         environment_dict = head_node.get("environment", None)
         annotations = head_node.get("annotations", None)
         labels = head_node.get("labels", None)
         if volumes_dict is None:
@@ -375,24 +428,26 @@
             ray_start_params=ray_start_params,
             volumes=volumes,
             service_account=service_account,
             image_pull_secret=image_pull_secret,
             environment=environment,
             annotations=annotations,
             labels=labels,
+            image_pull_policy=image_pull_policy,
         )
         # build worker nodes
         worker_groups = []
         index = 0
         for worker_node in worker_nodes:
             max_replicas = worker_node.get("max_replicas", 1)
             replicas = worker_node.get("replicas", 1)
             min_replicas = worker_node.get("min_replicas", 0)
             image = worker_node.get("image", self.default_image)
             image_pull_secret = worker_node.get("image_pull_secret", None)
+            image_pull_policy = head_node.get("image_pull_policy", None)
             ray_start_params = worker_node.get("ray_start_params", DEFAULT_WORKER_START_PARAMS)
             volumes_dict = worker_node.get("volumes", None)
             service_account = worker_node.get("service_account", None)
             environment_dict = worker_node.get("environment", None)
             annotations = worker_node.get("annotations", None)
             labels = worker_node.get("labels", None)
             if volumes_dict is None:
@@ -414,14 +469,15 @@
                     ray_start_params=ray_start_params,
                     volumes=volumes,
                     service_account=service_account,
                     image_pull_secret=image_pull_secret,
                     environment=environment,
                     annotations=annotations,
                     labels=labels,
+                    image_pull_policy=image_pull_policy,
                 )
             )
             index += 1
         # Build cluster spec
         cluster_spec = ClusterSpec(head_node=head_node_spec, worker_groups=worker_groups)
         # Build cluster
         cluster = Cluster(name=name, namespace=namespace, user="dataprep", version="2.9.3", cluster_spec=cluster_spec)
@@ -471,14 +527,19 @@
         :param runtime_env: runtime environment string
         :param executor: python file to execute
         :return:tuple containing
             http return code
             message - only returned if http return code is not equal to 200
             submission id - submission id
         """
+        # Although the cluster is ready, the service web server might not be ready yet at this point.
+        # To ensure that it is ready, trying to get jobs info from the cluster. Even if it fails
+        # couple of times, its harmless
+        _, _, _ = self.api_server_client.list_job_info(ns=namespace, name=name)
+        time.sleep(5)
         # Build job request
         job_request = RayJobRequest(entrypoint=KFPUtils.dict_to_req(d=request, executor=executor))
         if runtime_env is not None:
             job_request.runtime_env = runtime_env
         return self.api_server_client.submit_job(ns=namespace, name=name, job_request=job_request)
 
     def _get_job_status(self, name: str, namespace: str, submission_id: str) -> tuple[int, str, str]:
@@ -570,20 +631,22 @@
         # Print the final log and execution status
         # Sleep here to avoid racing conditions
         time.sleep(2)
         status, error, log = self.api_server_client.get_job_log(ns=namespace, name=name, sid=submission_id)
         if status // 100 != 2:
             sys.exit(1)
         self._print_log(log=log, previous_log_len=previous_log_len)
-        logger.info(f"Job completed with execution status {status}")
+        logger.info(f"Job completed with execution status {job_status}")
+        if job_status != JobStatus.SUCCEEDED:
+            sys.exit(1)
         if data_access is None:
             return
         # Here data access is either S3 or lakehouse both of which contain self.output_folder
         try:
-            output_folder = data_access.output_folder
+            output_folder = data_access.get_output_folder()
         except Exception as e:
             logger.warning(f"failed to get output folder {e}")
             return
         output_folder = output_folder if output_folder.endswith("/") else output_folder + "/"
         execution_log_path = f"{output_folder}execution.log"
         logger.info(f"saving execution log to {execution_log_path}")
         data_access.save_file(path=execution_log_path, data=bytes(log, "UTF-8"))
@@ -592,84 +655,88 @@
 class ComponentUtils:
     """
     Class containing methods supporting building pipelines
     """
 
     @staticmethod
     def add_settings_to_component(
-        task: dsl.PipelineTask,
+        component: dsl.ContainerOp,
         timeout: int,
         image_pull_policy: str = "IfNotPresent",
-        cache_strategy: bool = False,
+        cache_strategy: str = "P0D",
     ) -> None:
         """
-        Add settings to kfp task
-        :param task: kfp task
+        Add settings to kfp component
+        :param component: kfp component
         :param timeout: timeout to set to the component in seconds
         :param image_pull_policy: pull policy to set to the component
         :param cache_strategy: cache strategy
         """
-        
-        kubernetes.use_field_path_as_env(task, env_name=RUN_NAME, field_path="metadata.annotations['pipelines.kubeflow.org/run_name']")
         # Set cashing
-        task.set_caching_options(enable_caching=cache_strategy)
+        component.execution_options.caching_strategy.max_cache_staleness = cache_strategy
         # image pull policy
-        kubernetes.set_image_pull_policy(task, image_pull_policy)
-        # Set the timeout for the task to one day (in seconds)
-        kubernetes.set_timeout(task, seconds=timeout)
+        component.container.set_image_pull_policy(image_pull_policy)
+        # Set the timeout for the task
+        component.set_timeout(timeout)
 
     @staticmethod
     def set_s3_env_vars_to_component(
-        task: dsl.PipelineTask,
+        component: dsl.ContainerOp,
         secret: str,
-        env2key: dict[str, str] = {"s3-key": "S3_KEY",  "s3-secret": "S3_SECRET", "s3-endpoint": "ENDPOINT"},
+        env2key: dict[str, str] = {"S3_KEY": "s3-key", "S3_SECRET": "s3-secret", "ENDPOINT": "s3-endpoint"},
         prefix: str = None,
     ) -> None:
         """
         Set S3 env variables to KFP component
-        :param task: kfp task
+        :param component: kfp component
         :param secret: secret name with the S3 credentials
         :param env2key: dict with mapping each env variable to a key in the secret
         :param prefix: prefix to add to env name
         """
-        if prefix is not None:
-            for env_name, _ in env2key.items():    
-                env2key[prefix+"_"+env_name] = env2key.pop(env_name)    
-        
-        kubernetes.use_secret_as_env(task, secret_name=secret, secret_key_to_env=env2key)
+        for env_name, secret_key in env2key.items():
+            if prefix is not None:
+                env_name = f"{prefix}_{env_name}"
+            component = component.add_env_variable(
+                k8s_client.V1EnvVar(
+                    name=env_name,
+                    value_from=k8s_client.V1EnvVarSource(
+                        secret_key_ref=k8s_client.V1SecretKeySelector(name=secret, key=secret_key)
+                    ),
+                )
+            )
 
     @staticmethod
     def default_compute_execution_params(
         worker_options: str,  # ray worker configuration
         actor_options: str,  # cpus per actor
     ) -> str:
         """
         This is the most simplistic transform execution parameters computation
         :param worker_options: configuration of ray workers
         :param actor_options: actor request requirements
         :return: number of actors
         """
         import sys
 
-        from data_processing.utils import get_logger
+        from data_processing.utils import get_logger, GB
         from kfp_support.workflow_support.utils import KFPUtils
 
         logger = get_logger(__name__)
 
         # convert input
         w_options = KFPUtils.load_from_json(worker_options.replace("'", '"'))
         a_options = KFPUtils.load_from_json(actor_options.replace("'", '"'))
         # Compute available cluster resources
         cluster_cpu = w_options["replicas"] * w_options["cpu"]
         cluster_mem = w_options["replicas"] * w_options["memory"]
         cluster_gpu = w_options["replicas"] * w_options.get("gpu", 0.0)
         logger.info(f"Cluster available CPUs {cluster_cpu}, Memory {cluster_mem}, GPUs {cluster_gpu}")
         # compute number of actors
         n_actors_cpu = int(cluster_cpu * 0.85 / a_options.get("num_cpus", 0.5))
-        n_actors_memory = int(cluster_mem * 0.85 / a_options.get("memory", 1))
+        n_actors_memory = int(cluster_mem * 0.85 / (a_options.get("memory", GB) / GB))
         n_actors = min(n_actors_cpu, n_actors_memory)
         # Check if we need gpu calculations as well
         actor_gpu = a_options.get("num_gpus", 0)
         if actor_gpu > 0:
             n_actors_gpu = int(cluster_gpu / actor_gpu)
             n_actors = min(n_actors, n_actors_gpu)
         logger.info(f"Number of actors - {n_actors}")
```

### Comparing `data_prep_toolkit_kfp-0.0.1.dev9/test/api_params_test.py` & `data_prep_toolkit_kfp-0.1.0/test/api_params_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 import json
 
 from kfp_support.api_server_client.params import (
     DEFAULT_HEAD_START_PARAMS,
     DEFAULT_WORKER_START_PARAMS,
     AccessMode,
+    AutoscalerOptions,
     Cluster,
     ClusterEvent,
     ClusterSpec,
     ConfigMapVolume,
     EmptyDirVolume,
     Environment,
     EnvironmentVariables,
@@ -36,14 +37,15 @@
     SecretVolume,
     ServiceType,
     Template,
     Toleration,
     TolerationEffect,
     TolerationOperation,
     WorkerNodeSpec,
+    autoscaling_decoder,
     cluster_decoder,
     cluster_spec_decoder,
     env_var_from_decoder,
     environment_variables_decoder,
     head_node_spec_decoder,
     template_decoder,
     toleration_decoder,
@@ -193,14 +195,15 @@
         compute_template="template",
         image="rayproject/ray:2.9.0-py310",
         ray_start_params=DEFAULT_HEAD_START_PARAMS,
         enable_ingress=True,
         service_type=ServiceType.ClusterIP,
         volumes=volumes,
         environment=env_s,
+        image_pull_policy="Always",
     )
     print(f"\nhead node: {head.to_string()}")
     head_json = json.dumps(head.to_dict())
     print(f"head node JSON: {head_json}")
     assert head_node_spec_decoder(json.loads(head_json)).to_string() == head.to_string()
 
 
@@ -226,21 +229,36 @@
         replicas=2,
         min_replicas=2,
         max_replicas=2,
         volumes=volumes,
         ray_start_params=DEFAULT_WORKER_START_PARAMS,
         environment=env_s,
         labels={"key": "value"},
+        image_pull_policy="IfNotPresent",
     )
     print(f"\nworker node: {worker.to_string()}")
     worker_json = json.dumps(worker.to_dict())
     print(f"worker node JSON: {worker_json}")
     assert worker_node_spec_decoder(json.loads(worker_json)).to_string() == worker.to_string()
 
 
+def test_autoscaler_options():
+    options = AutoscalerOptions()
+    print(f"\nautoscaler options: {options.to_string()}")
+    options_json = json.dumps(options.to_dict())
+    print(f"autoscaler options JSON: {options_json}")
+    assert autoscaling_decoder(json.loads(options_json)).to_string() == options.to_string()
+
+    options = AutoscalerOptions(cpus="1.0", memory="64GB")
+    print(f"\nautoscaler options: {options.to_string()}")
+    options_json = json.dumps(options.to_dict())
+    print(f"autoscaler options JSON: {options_json}")
+    assert autoscaling_decoder(json.loads(options_json)).to_string() == options.to_string()
+
+
 def test_cluster_spec():
     env_s = EnvironmentVariables(
         key_value={"key": "val"},
         from_ref={"key_ref": EnvVarFrom(source=EnvVarSource.SECRET, name="my-secret", key="key")},
     )
     volumes = [
         PVCVolume(
@@ -284,14 +302,15 @@
                 image="rayproject/ray:2.9.0-py310",
                 ray_start_params=DEFAULT_WORKER_START_PARAMS,
                 volumes=volumes,
                 environment=env_s,
                 labels={"key": "value"},
             ),
         ],
+        autoscaling_options=AutoscalerOptions(),
     )
     print(f"\ncluster spec: {spec.to_string()}")
     spec_json = json.dumps(spec.to_dict())
     print(f"cluster spec JSON: {spec_json}")
     assert cluster_spec_decoder(json.loads(spec_json)).to_string() == spec.to_string()
```

### Comparing `data_prep_toolkit_kfp-0.0.1.dev9/test/configmaps.py` & `data_prep_toolkit_kfp-0.1.0/test/configmaps.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev9/test/kuberay_api_test.py` & `data_prep_toolkit_kfp-0.1.0/test/kuberay_api_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -101,29 +101,31 @@
         source="ray-job-code-sample",
         items={"sample_code.py": "sample_code.py"},
     )
     environment = EnvironmentVariables(key_value={"key": "value"})
     head = HeadNodeSpec(
         compute_template="default-template",
         ray_start_params={"metrics-export-port": "8080", "num-cpus": "0"},
-        image="rayproject/ray:2.9.0-py310",
+        image="rayproject/ray:2.9.3-py310",
         service_type=ServiceType.ClusterIP,
         volumes=[volume],
         environment=environment,
+        image_pull_policy="Always",
     )
     worker = WorkerNodeSpec(
         group_name="small",
         compute_template="default-template",
         replicas=1,
         min_replicas=1,
         max_replicas=1,
         ray_start_params=DEFAULT_WORKER_START_PARAMS,
-        image="rayproject/ray:2.9.0-py310",
+        image="rayproject/ray:2.9.3-py310",
         volumes=[volume],
         environment=environment,
+        image_pull_policy="Always",
     )
     t_cluster = Cluster(
         name="test",
         namespace="default",
         user="boris",
         version="2.9.0",
         cluster_spec=ClusterSpec(head_node=head, worker_groups=[worker]),
@@ -199,29 +201,31 @@
         source="ray-job-code-sample",
         items={"sample_code.py": "sample_code.py"},
     )
     environment = EnvironmentVariables(key_value={"key": "value"})
     head = HeadNodeSpec(
         compute_template="default-template",
         ray_start_params={"metrics-export-port": "8080", "num-cpus": "0"},
-        image="rayproject/ray:2.9.0-py310",
+        image="rayproject/ray:2.9.3-py310",
         service_type=ServiceType.ClusterIP,
         volumes=[volume],
         environment=environment,
+        image_pull_policy="IfNotPresent",
     )
     worker = WorkerNodeSpec(
         group_name="small",
         compute_template="default-template",
         replicas=1,
         min_replicas=1,
         max_replicas=1,
         ray_start_params=DEFAULT_WORKER_START_PARAMS,
-        image="rayproject/ray:2.9.0-py310",
+        image="rayproject/ray:2.9.3-py310",
         volumes=[volume],
         environment=environment,
+        image_pull_policy="IfNotPresent",
     )
     t_cluster = Cluster(
         name="test-job",
         namespace="default",
         user="boris",
         version="2.9.0",
         cluster_spec=ClusterSpec(head_node=head, worker_groups=[worker]),
@@ -241,17 +245,26 @@
       - pendulum==2.1.2
     env_vars:
       counter_name: test_counter    
     """
     job_request = RayJobRequest(
         entrypoint="python /home/ray/samples/sample_code.py", runtime_env=resource_yaml, num_cpu=0.5
     )
+    # To ensure that Ray cluster HTTP is ready try to get jobs info from the cluster
+    status, error, job_info_array = apis.list_job_info(ns="default", name="test-job")
+    assert status == 200
+    assert error is None
+    print("\n initial jobs info")
+    for inf in job_info_array:
+        print(f"    {inf.to_string()}")
+    time.sleep(5)
     status, error, sid = apis.submit_job(ns="default", name="test-job", job_request=job_request)
     assert status == 200
     assert error is None
+    time.sleep(10)
     # get Ray job info
     status, error, jinfo = apis.get_job_info(ns="default", name="test-job", sid=sid)
     assert status == 200
     assert error is None
     print(f"\njobs info {jinfo.to_string()}")
     # get Ray jobs info
     status, error, job_info_array = apis.list_job_info(ns="default", name="test-job")
```

### Comparing `data_prep_toolkit_kfp-0.0.1.dev9/test/pipeline_utils_test.py` & `data_prep_toolkit_kfp-0.1.0/test/pipeline_utils_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.0.1.dev9/test/ray_remote_jobs_test.py` & `data_prep_toolkit_kfp-0.1.0/test/ray_remote_jobs_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,26 +30,28 @@
         )
     ]
     dct_volumes = {"volumes": [v.to_dict() for v in volumes]}
 
     head_node = {
         "cpu": 2,
         "memory": 4,
-        "image": "rayproject/ray:2.9.0-py310",
+        "image": "rayproject/ray:2.9.3-py310",
         # Ray start params, just to show
         "ray_start_params": {"metrics-export-port": "8080", "num-cpus": "0", "dashboard-host": "0.0.0.0"},
+        "image_pull_policy": "Always",
     } | dct_volumes
 
     worker_node = {
         "cpu": 2,
         "memory": 4,
-        "image": "rayproject/ray:2.9.0-py310",
+        "image": "rayproject/ray:2.9.3-py310",
         "replicas": 1,
         "min_replicas": 1,
         "max_replicas": 1,
+        "image_pull_policy": "Always",
     } | dct_volumes
 
     # Create configmap for testing
     cm_manager = ConfigmapsManager()
     cm_manager.delete_code_map()
     cm_manager.create_code_map()
```

