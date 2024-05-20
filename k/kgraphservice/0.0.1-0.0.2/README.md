# Comparing `tmp/kgraphservice-0.0.1.tar.gz` & `tmp/kgraphservice-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kgraphservice-0.0.1.tar", last modified: Tue May  7 11:54:14 2024, max compression
+gzip compressed data, was "kgraphservice-0.0.2.tar", last modified: Mon May 20 21:32:55 2024, max compression
```

## Comparing `kgraphservice-0.0.1.tar` & `kgraphservice-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 11:54:14.355219 kgraphservice-0.0.1/
--rw-r--r--   0 hadfield   (501) staff       (20)    11357 2024-05-07 11:46:32.000000 kgraphservice-0.0.1/LICENSE
--rw-r--r--   0 hadfield   (501) staff       (20)      752 2024-05-07 11:54:14.355001 kgraphservice-0.0.1/PKG-INFO
--rw-r--r--   0 hadfield   (501) staff       (20)       15 2024-05-07 11:46:32.000000 kgraphservice-0.0.1/README.md
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 11:54:14.353977 kgraphservice-0.0.1/kgraphservice/
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-07 11:50:04.000000 kgraphservice-0.0.1/kgraphservice/__init__.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 11:54:14.354762 kgraphservice-0.0.1/kgraphservice.egg-info/
--rw-r--r--   0 hadfield   (501) staff       (20)      752 2024-05-07 11:54:14.000000 kgraphservice-0.0.1/kgraphservice.egg-info/PKG-INFO
--rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-07 11:54:14.000000 kgraphservice-0.0.1/kgraphservice.egg-info/SOURCES.txt
--rw-r--r--   0 hadfield   (501) staff       (20)        1 2024-05-07 11:54:14.000000 kgraphservice-0.0.1/kgraphservice.egg-info/dependency_links.txt
--rw-r--r--   0 hadfield   (501) staff       (20)      141 2024-05-07 11:54:14.000000 kgraphservice-0.0.1/kgraphservice.egg-info/requires.txt
--rw-r--r--   0 hadfield   (501) staff       (20)       14 2024-05-07 11:54:14.000000 kgraphservice-0.0.1/kgraphservice.egg-info/top_level.txt
--rw-r--r--   0 hadfield   (501) staff       (20)       38 2024-05-07 11:54:14.355270 kgraphservice-0.0.1/setup.cfg
--rw-r--r--   0 hadfield   (501) staff       (20)      947 2024-05-07 11:49:51.000000 kgraphservice-0.0.1/setup.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-20 21:32:55.871361 kgraphservice-0.0.2/
+-rw-r--r--   0 hadfield   (501) staff       (20)    11357 2024-05-07 11:46:32.000000 kgraphservice-0.0.2/LICENSE
+-rw-r--r--   0 hadfield   (501) staff       (20)      753 2024-05-20 21:32:55.871160 kgraphservice-0.0.2/PKG-INFO
+-rw-r--r--   0 hadfield   (501) staff       (20)       15 2024-05-07 11:46:32.000000 kgraphservice-0.0.2/README.md
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-20 21:32:55.870176 kgraphservice-0.0.2/kgraphservice/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-07 11:50:04.000000 kgraphservice-0.0.2/kgraphservice/__init__.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     3287 2024-05-20 21:31:52.000000 kgraphservice-0.0.2/kgraphservice/kgraph_service.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-20 21:32:55.870951 kgraphservice-0.0.2/kgraphservice.egg-info/
+-rw-r--r--   0 hadfield   (501) staff       (20)      753 2024-05-20 21:32:55.000000 kgraphservice-0.0.2/kgraphservice.egg-info/PKG-INFO
+-rw-r--r--   0 hadfield   (501) staff       (20)      268 2024-05-20 21:32:55.000000 kgraphservice-0.0.2/kgraphservice.egg-info/SOURCES.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)        1 2024-05-20 21:32:55.000000 kgraphservice-0.0.2/kgraphservice.egg-info/dependency_links.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-20 21:32:55.000000 kgraphservice-0.0.2/kgraphservice.egg-info/requires.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)       14 2024-05-20 21:32:55.000000 kgraphservice-0.0.2/kgraphservice.egg-info/top_level.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)       38 2024-05-20 21:32:55.871400 kgraphservice-0.0.2/setup.cfg
+-rw-r--r--   0 hadfield   (501) staff       (20)      948 2024-05-20 21:32:34.000000 kgraphservice-0.0.2/setup.py
```

### Comparing `kgraphservice-0.0.1/LICENSE` & `kgraphservice-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kgraphservice-0.0.1/PKG-INFO` & `kgraphservice-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: kgraphservice
-Version: 0.0.1
+Version: 0.0.2
 Summary: KGraph Service
 Home-page: https://github.com/vital-ai/kgraphservice
 Author: Marc Hadfield
 Author-email: marc@vital.ai
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: vital-ai-vitalsigns>=0.1.4
+Requires-Dist: vital-ai-vitalsigns>=0.1.12
 Requires-Dist: vital-ai-domain>=0.1.4
 Requires-Dist: six
 Requires-Dist: pyyaml
-Requires-Dist: vital-ai-haley-kg>=0.1.4
+Requires-Dist: vital-ai-haley-kg>=0.1.6
 Requires-Dist: rdflib==7.0.0
 Requires-Dist: SPARQLWrapper==2.0.0
 Requires-Dist: networkx
 Requires-Dist: matplotlib
 
 # kgraphservice
```

### Comparing `kgraphservice-0.0.1/kgraphservice.egg-info/PKG-INFO` & `kgraphservice-0.0.2/kgraphservice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: kgraphservice
-Version: 0.0.1
+Version: 0.0.2
 Summary: KGraph Service
 Home-page: https://github.com/vital-ai/kgraphservice
 Author: Marc Hadfield
 Author-email: marc@vital.ai
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: vital-ai-vitalsigns>=0.1.4
+Requires-Dist: vital-ai-vitalsigns>=0.1.12
 Requires-Dist: vital-ai-domain>=0.1.4
 Requires-Dist: six
 Requires-Dist: pyyaml
-Requires-Dist: vital-ai-haley-kg>=0.1.4
+Requires-Dist: vital-ai-haley-kg>=0.1.6
 Requires-Dist: rdflib==7.0.0
 Requires-Dist: SPARQLWrapper==2.0.0
 Requires-Dist: networkx
 Requires-Dist: matplotlib
 
 # kgraphservice
```

### Comparing `kgraphservice-0.0.1/setup.py` & `kgraphservice-0.0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
     name='kgraphservice',
-    version='0.0.1',
+    version='0.0.2',
     author='Marc Hadfield',
     author_email='marc@vital.ai',
     description='KGraph Service',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/vital-ai/kgraphservice',
     packages=find_packages(exclude=["test"]),
     license='Apache License 2.0',
     install_requires=[
-            'vital-ai-vitalsigns>=0.1.4',
+            'vital-ai-vitalsigns>=0.1.12',
             'vital-ai-domain>=0.1.4',
             'six',
             'pyyaml',
-            'vital-ai-haley-kg>=0.1.4',
+            'vital-ai-haley-kg>=0.1.6',
             'rdflib==7.0.0',
             'SPARQLWrapper==2.0.0',
             'networkx',
             'matplotlib',
     ],
     classifiers=[
         "Programming Language :: Python :: 3.10",
```

