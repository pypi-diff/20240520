# Comparing `tmp/fc_pruning-0.0.8.tar.gz` & `tmp/fc_pruning-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fc_pruning-0.0.8.tar", last modified: Thu May 16 21:37:11 2024, max compression
+gzip compressed data, was "fc_pruning-0.0.9.tar", last modified: Thu May 16 21:51:56 2024, max compression
```

## Comparing `fc_pruning-0.0.8.tar` & `fc_pruning-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-05-16 21:37:11.310260 fc_pruning-0.0.8/
--rw-r--r--   0 aidamehammed   (501) staff       (20)    11352 2024-04-30 18:18:40.000000 fc_pruning-0.0.8/LICENSE
--rw-r--r--   0 aidamehammed   (501) staff       (20)     1102 2024-05-16 21:37:11.310165 fc_pruning-0.0.8/PKG-INFO
--rw-r--r--   0 aidamehammed   (501) staff       (20)      556 2024-04-30 18:18:40.000000 fc_pruning-0.0.8/README.md
-drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-05-16 21:37:11.308728 fc_pruning-0.0.8/fc_pruning/
-drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-05-16 21:37:11.309892 fc_pruning-0.0.8/fc_pruning/Compress/
--rw-r--r--   0 aidamehammed   (501) staff       (20)       49 2024-04-30 18:22:57.000000 fc_pruning-0.0.8/fc_pruning/Compress/__init__.py
--rw-r--r--   0 aidamehammed   (501) staff       (20)     5893 2024-05-16 21:05:08.000000 fc_pruning-0.0.8/fc_pruning/Compress/compress.py
--rw-r--r--   0 aidamehammed   (501) staff       (20)     4213 2024-05-11 17:52:26.000000 fc_pruning-0.0.8/fc_pruning/Compress/utils.py
--rw-r--r--   0 aidamehammed   (501) staff       (20)        0 2024-04-30 18:22:57.000000 fc_pruning-0.0.8/fc_pruning/__init__.py
-drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-05-16 21:37:11.309275 fc_pruning-0.0.8/fc_pruning.egg-info/
--rw-r--r--   0 aidamehammed   (501) staff       (20)     1102 2024-05-16 21:37:11.000000 fc_pruning-0.0.8/fc_pruning.egg-info/PKG-INFO
--rw-r--r--   0 aidamehammed   (501) staff       (20)      311 2024-05-16 21:37:11.000000 fc_pruning-0.0.8/fc_pruning.egg-info/SOURCES.txt
--rw-r--r--   0 aidamehammed   (501) staff       (20)        1 2024-05-16 21:37:11.000000 fc_pruning-0.0.8/fc_pruning.egg-info/dependency_links.txt
--rw-r--r--   0 aidamehammed   (501) staff       (20)       27 2024-05-16 21:37:11.000000 fc_pruning-0.0.8/fc_pruning.egg-info/requires.txt
--rw-r--r--   0 aidamehammed   (501) staff       (20)       11 2024-05-16 21:37:11.000000 fc_pruning-0.0.8/fc_pruning.egg-info/top_level.txt
--rw-r--r--   0 aidamehammed   (501) staff       (20)       38 2024-05-16 21:37:11.310314 fc_pruning-0.0.8/setup.cfg
--rw-r--r--   0 aidamehammed   (501) staff       (20)     1202 2024-05-16 21:37:07.000000 fc_pruning-0.0.8/setup.py
+drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-05-16 21:51:56.868572 fc_pruning-0.0.9/
+-rw-r--r--   0 aidamehammed   (501) staff       (20)    11352 2024-04-30 18:18:40.000000 fc_pruning-0.0.9/LICENSE
+-rw-r--r--   0 aidamehammed   (501) staff       (20)     1102 2024-05-16 21:51:56.868472 fc_pruning-0.0.9/PKG-INFO
+-rw-r--r--   0 aidamehammed   (501) staff       (20)      556 2024-04-30 18:18:40.000000 fc_pruning-0.0.9/README.md
+drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-05-16 21:51:56.867084 fc_pruning-0.0.9/fc_pruning/
+drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-05-16 21:51:56.868182 fc_pruning-0.0.9/fc_pruning/Compress/
+-rw-r--r--   0 aidamehammed   (501) staff       (20)       49 2024-04-30 18:22:57.000000 fc_pruning-0.0.9/fc_pruning/Compress/__init__.py
+-rw-r--r--   0 aidamehammed   (501) staff       (20)     5896 2024-05-16 21:51:47.000000 fc_pruning-0.0.9/fc_pruning/Compress/compress.py
+-rw-r--r--   0 aidamehammed   (501) staff       (20)     4213 2024-05-11 17:52:26.000000 fc_pruning-0.0.9/fc_pruning/Compress/utils.py
+-rw-r--r--   0 aidamehammed   (501) staff       (20)        0 2024-04-30 18:22:57.000000 fc_pruning-0.0.9/fc_pruning/__init__.py
+drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-05-16 21:51:56.867680 fc_pruning-0.0.9/fc_pruning.egg-info/
+-rw-r--r--   0 aidamehammed   (501) staff       (20)     1102 2024-05-16 21:51:56.000000 fc_pruning-0.0.9/fc_pruning.egg-info/PKG-INFO
+-rw-r--r--   0 aidamehammed   (501) staff       (20)      311 2024-05-16 21:51:56.000000 fc_pruning-0.0.9/fc_pruning.egg-info/SOURCES.txt
+-rw-r--r--   0 aidamehammed   (501) staff       (20)        1 2024-05-16 21:51:56.000000 fc_pruning-0.0.9/fc_pruning.egg-info/dependency_links.txt
+-rw-r--r--   0 aidamehammed   (501) staff       (20)       27 2024-05-16 21:51:56.000000 fc_pruning-0.0.9/fc_pruning.egg-info/requires.txt
+-rw-r--r--   0 aidamehammed   (501) staff       (20)       11 2024-05-16 21:51:56.000000 fc_pruning-0.0.9/fc_pruning.egg-info/top_level.txt
+-rw-r--r--   0 aidamehammed   (501) staff       (20)       38 2024-05-16 21:51:56.868618 fc_pruning-0.0.9/setup.cfg
+-rw-r--r--   0 aidamehammed   (501) staff       (20)     1202 2024-05-16 21:51:47.000000 fc_pruning-0.0.9/setup.py
```

### Comparing `fc_pruning-0.0.8/LICENSE` & `fc_pruning-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fc_pruning-0.0.8/PKG-INFO` & `fc_pruning-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fc_pruning
-Version: 0.0.8
+Version: 0.0.9
 Summary: FC Pruning
 Home-page: https://github.com/AidaMehammed/fc_pruning
 Author: Aida Mehammed
 Author-email: aida.mehammed@studium.uni-hamburg.de
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/AidaMehammed/fc_pruning/issues
 Platform: UNKNOWN
```

### Comparing `fc_pruning-0.0.8/README.md` & `fc_pruning-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `fc_pruning-0.0.8/fc_pruning/Compress/compress.py` & `fc_pruning-0.0.9/fc_pruning/Compress/compress.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,17 +145,17 @@
             reconstructed_clients = []
             for i in range(len(data)):
                 reconstructed_model = pf.reconstruct_model(data[i], binary_mask[i][0], reference_model)
                 reconstructed_clients.append(reconstructed_model)
             data = reconstructed_clients
         else:
             data = data_with_mask_list
-
         return data
- def send_data_to_coordinator(self, data, use_pruning= True, **kwargs):
+
+    def send_data_to_coordinator(self, data, use_pruning= True, **kwargs):
         '''
             Sends data to the coordinator, including pruning if enabled.
 
             Parameters
             ----------
             data : list
                 List of data to be sent to the coordinator.
```

### Comparing `fc_pruning-0.0.8/fc_pruning/Compress/utils.py` & `fc_pruning-0.0.9/fc_pruning/Compress/utils.py`

 * *Files identical despite different names*

### Comparing `fc_pruning-0.0.8/fc_pruning.egg-info/PKG-INFO` & `fc_pruning-0.0.9/fc_pruning.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fc-pruning
-Version: 0.0.8
+Version: 0.0.9
 Summary: FC Pruning
 Home-page: https://github.com/AidaMehammed/fc_pruning
 Author: Aida Mehammed
 Author-email: aida.mehammed@studium.uni-hamburg.de
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/AidaMehammed/fc_pruning/issues
 Platform: UNKNOWN
```

### Comparing `fc_pruning-0.0.8/setup.py` & `fc_pruning-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(name="fc_pruning",
-                 version="0.0.8",
+                 version="0.0.9",
                  author="Aida Mehammed",
                  author_email="aida.mehammed@studium.uni-hamburg.de",
                  description="FC Pruning",
                  long_description=long_description,
                  long_description_content_type="text/markdown",
                  url="https://github.com/AidaMehammed/fc_pruning",
                  project_urls={
```

