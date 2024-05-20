# Comparing `tmp/verifyvoice-0.1.31.tar.gz` & `tmp/verifyvoice-0.1.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verifyvoice-0.1.31.tar", last modified: Mon May 20 10:50:57 2024, max compression
+gzip compressed data, was "verifyvoice-0.1.32.tar", last modified: Mon May 20 18:32:31 2024, max compression
```

## Comparing `verifyvoice-0.1.31.tar` & `verifyvoice-0.1.32.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 thejan    (1000) thejan    (1000)        0 2024-05-20 10:50:57.294019 verifyvoice-0.1.31/
--rw-r--r--   0 thejan    (1000) thejan    (1000)      979 2024-05-20 10:50:57.294019 verifyvoice-0.1.31/PKG-INFO
--rw-rw-r--   0 thejan    (1000) thejan    (1000)      127 2024-05-01 09:13:01.000000 verifyvoice-0.1.31/README.md
--rw-rw-r--   0 thejan    (1000) thejan    (1000)       38 2024-05-20 10:50:57.294019 verifyvoice-0.1.31/setup.cfg
--rw-rw-r--   0 thejan    (1000) thejan    (1000)     1369 2024-05-20 10:50:46.000000 verifyvoice-0.1.31/setup.py
-drwxrwxr-x   0 thejan    (1000) thejan    (1000)        0 2024-05-20 10:50:57.290019 verifyvoice-0.1.31/verifyvoice/
--rw-rw-r--   0 thejan    (1000) thejan    (1000)     3667 2024-05-20 10:48:03.000000 verifyvoice-0.1.31/verifyvoice/DataLoader.py
--rw-rw-r--   0 thejan    (1000) thejan    (1000)     4943 2024-05-20 10:48:32.000000 verifyvoice-0.1.31/verifyvoice/ModelLoader.py
--rw-rw-r--   0 thejan    (1000) thejan    (1000)      719 2024-05-20 10:08:16.000000 verifyvoice-0.1.31/verifyvoice/Similarity.py
--rw-rw-r--   0 thejan    (1000) thejan    (1000)     2765 2024-05-20 10:13:08.000000 verifyvoice-0.1.31/verifyvoice/SpeakerNet.py
--rw-rw-r--   0 thejan    (1000) thejan    (1000)     3656 2024-05-20 10:50:17.000000 verifyvoice-0.1.31/verifyvoice/Spk_Encoder.py
--rw-rw-r--   0 thejan    (1000) thejan    (1000)    28893 2024-05-20 09:15:36.000000 verifyvoice-0.1.31/verifyvoice/WavLM.py
--rw-rw-r--   0 thejan    (1000) thejan    (1000)      106 2024-05-20 09:57:43.000000 verifyvoice-0.1.31/verifyvoice/__init__.py
--rw-rw-r--   0 thejan    (1000) thejan    (1000)     2082 2024-05-13 14:54:41.000000 verifyvoice-0.1.31/verifyvoice/aamsoftmax.py
--rw-rw-r--   0 thejan    (1000) thejan    (1000)     1330 2024-05-20 10:12:39.000000 verifyvoice-0.1.31/verifyvoice/deepInfoMaxLoss.py
--rw-rw-r--   0 thejan    (1000) thejan    (1000)     1935 2024-05-11 14:54:52.000000 verifyvoice-0.1.31/verifyvoice/mine.py
--rw-rw-r--   0 thejan    (1000) thejan    (1000)     2760 2024-05-20 10:49:54.000000 verifyvoice-0.1.31/verifyvoice/model_args.py
--rw-rw-r--   0 thejan    (1000) thejan    (1000)    31946 2024-05-18 09:38:55.000000 verifyvoice-0.1.31/verifyvoice/modules.py
--rw-rw-r--   0 thejan    (1000) thejan    (1000)     1285 2024-05-20 09:16:02.000000 verifyvoice-0.1.31/verifyvoice/utils.py
-drwxrwxr-x   0 thejan    (1000) thejan    (1000)        0 2024-05-20 10:50:57.294019 verifyvoice-0.1.31/verifyvoice.egg-info/
--rw-r--r--   0 thejan    (1000) thejan    (1000)      979 2024-05-20 10:50:57.000000 verifyvoice-0.1.31/verifyvoice.egg-info/PKG-INFO
--rw-rw-r--   0 thejan    (1000) thejan    (1000)      516 2024-05-20 10:50:57.000000 verifyvoice-0.1.31/verifyvoice.egg-info/SOURCES.txt
--rw-rw-r--   0 thejan    (1000) thejan    (1000)        1 2024-05-20 10:50:57.000000 verifyvoice-0.1.31/verifyvoice.egg-info/dependency_links.txt
--rw-rw-r--   0 thejan    (1000) thejan    (1000)       55 2024-05-20 10:50:57.000000 verifyvoice-0.1.31/verifyvoice.egg-info/requires.txt
--rw-rw-r--   0 thejan    (1000) thejan    (1000)       12 2024-05-20 10:50:57.000000 verifyvoice-0.1.31/verifyvoice.egg-info/top_level.txt
+drwxrwxr-x   0 thejan    (1000) thejan    (1000)        0 2024-05-20 18:32:31.296938 verifyvoice-0.1.32/
+-rw-r--r--   0 thejan    (1000) thejan    (1000)      979 2024-05-20 18:32:31.296938 verifyvoice-0.1.32/PKG-INFO
+-rw-rw-r--   0 thejan    (1000) thejan    (1000)      127 2024-05-01 09:13:01.000000 verifyvoice-0.1.32/README.md
+-rw-rw-r--   0 thejan    (1000) thejan    (1000)       38 2024-05-20 18:32:31.296938 verifyvoice-0.1.32/setup.cfg
+-rw-rw-r--   0 thejan    (1000) thejan    (1000)     1369 2024-05-20 18:32:04.000000 verifyvoice-0.1.32/setup.py
+drwxrwxr-x   0 thejan    (1000) thejan    (1000)        0 2024-05-20 18:32:31.292938 verifyvoice-0.1.32/verifyvoice/
+-rw-rw-r--   0 thejan    (1000) thejan    (1000)     3667 2024-05-20 10:48:03.000000 verifyvoice-0.1.32/verifyvoice/DataLoader.py
+-rw-rw-r--   0 thejan    (1000) thejan    (1000)     4943 2024-05-20 10:48:32.000000 verifyvoice-0.1.32/verifyvoice/ModelLoader.py
+-rw-rw-r--   0 thejan    (1000) thejan    (1000)      719 2024-05-20 10:08:16.000000 verifyvoice-0.1.32/verifyvoice/Similarity.py
+-rw-rw-r--   0 thejan    (1000) thejan    (1000)     2765 2024-05-20 10:13:08.000000 verifyvoice-0.1.32/verifyvoice/SpeakerNet.py
+-rw-rw-r--   0 thejan    (1000) thejan    (1000)     3656 2024-05-20 10:50:17.000000 verifyvoice-0.1.32/verifyvoice/Spk_Encoder.py
+-rw-rw-r--   0 thejan    (1000) thejan    (1000)    28893 2024-05-20 09:15:36.000000 verifyvoice-0.1.32/verifyvoice/WavLM.py
+-rw-rw-r--   0 thejan    (1000) thejan    (1000)      106 2024-05-20 09:57:43.000000 verifyvoice-0.1.32/verifyvoice/__init__.py
+-rw-rw-r--   0 thejan    (1000) thejan    (1000)     2082 2024-05-13 14:54:41.000000 verifyvoice-0.1.32/verifyvoice/aamsoftmax.py
+-rw-rw-r--   0 thejan    (1000) thejan    (1000)     1330 2024-05-20 10:12:39.000000 verifyvoice-0.1.32/verifyvoice/deepInfoMaxLoss.py
+-rw-rw-r--   0 thejan    (1000) thejan    (1000)     1935 2024-05-11 14:54:52.000000 verifyvoice-0.1.32/verifyvoice/mine.py
+-rw-rw-r--   0 thejan    (1000) thejan    (1000)     2760 2024-05-20 10:49:54.000000 verifyvoice-0.1.32/verifyvoice/model_args.py
+-rw-rw-r--   0 thejan    (1000) thejan    (1000)    31946 2024-05-18 09:38:55.000000 verifyvoice-0.1.32/verifyvoice/modules.py
+-rw-rw-r--   0 thejan    (1000) thejan    (1000)     1285 2024-05-20 09:16:02.000000 verifyvoice-0.1.32/verifyvoice/utils.py
+drwxrwxr-x   0 thejan    (1000) thejan    (1000)        0 2024-05-20 18:32:31.292938 verifyvoice-0.1.32/verifyvoice.egg-info/
+-rw-r--r--   0 thejan    (1000) thejan    (1000)      979 2024-05-20 18:32:31.000000 verifyvoice-0.1.32/verifyvoice.egg-info/PKG-INFO
+-rw-rw-r--   0 thejan    (1000) thejan    (1000)      516 2024-05-20 18:32:31.000000 verifyvoice-0.1.32/verifyvoice.egg-info/SOURCES.txt
+-rw-rw-r--   0 thejan    (1000) thejan    (1000)        1 2024-05-20 18:32:31.000000 verifyvoice-0.1.32/verifyvoice.egg-info/dependency_links.txt
+-rw-rw-r--   0 thejan    (1000) thejan    (1000)       55 2024-05-20 18:32:31.000000 verifyvoice-0.1.32/verifyvoice.egg-info/requires.txt
+-rw-rw-r--   0 thejan    (1000) thejan    (1000)       12 2024-05-20 18:32:31.000000 verifyvoice-0.1.32/verifyvoice.egg-info/top_level.txt
```

### Comparing `verifyvoice-0.1.31/PKG-INFO` & `verifyvoice-0.1.32/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verifyvoice
-Version: 0.1.31
+Version: 0.1.32
 Summary: A package for verifying the voice of a person
 Home-page: https://github.com/NirmalSankalana/VerifiVoice
 Author: Nirmal Sankalana, Nipun Thejan
 Author-email: sankalana.nirmal@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `verifyvoice-0.1.31/setup.py` & `verifyvoice-0.1.32/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="verifyvoice",
-    version="0.1.31",
+    version="0.1.32",
     description="A package for verifying the voice of a person",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/NirmalSankalana/VerifiVoice",
     author="Nirmal Sankalana, Nipun Thejan",
     author_email="sankalana.nirmal@gmail.com",
     license="MIT",
```

### Comparing `verifyvoice-0.1.31/verifyvoice/DataLoader.py` & `verifyvoice-0.1.32/verifyvoice/DataLoader.py`

 * *Files identical despite different names*

### Comparing `verifyvoice-0.1.31/verifyvoice/ModelLoader.py` & `verifyvoice-0.1.32/verifyvoice/ModelLoader.py`

 * *Files identical despite different names*

### Comparing `verifyvoice-0.1.31/verifyvoice/Similarity.py` & `verifyvoice-0.1.32/verifyvoice/Similarity.py`

 * *Files identical despite different names*

### Comparing `verifyvoice-0.1.31/verifyvoice/SpeakerNet.py` & `verifyvoice-0.1.32/verifyvoice/SpeakerNet.py`

 * *Files identical despite different names*

### Comparing `verifyvoice-0.1.31/verifyvoice/Spk_Encoder.py` & `verifyvoice-0.1.32/verifyvoice/Spk_Encoder.py`

 * *Files identical despite different names*

### Comparing `verifyvoice-0.1.31/verifyvoice/WavLM.py` & `verifyvoice-0.1.32/verifyvoice/WavLM.py`

 * *Files identical despite different names*

### Comparing `verifyvoice-0.1.31/verifyvoice/aamsoftmax.py` & `verifyvoice-0.1.32/verifyvoice/aamsoftmax.py`

 * *Files identical despite different names*

### Comparing `verifyvoice-0.1.31/verifyvoice/deepInfoMaxLoss.py` & `verifyvoice-0.1.32/verifyvoice/deepInfoMaxLoss.py`

 * *Files identical despite different names*

### Comparing `verifyvoice-0.1.31/verifyvoice/mine.py` & `verifyvoice-0.1.32/verifyvoice/mine.py`

 * *Files identical despite different names*

### Comparing `verifyvoice-0.1.31/verifyvoice/model_args.py` & `verifyvoice-0.1.32/verifyvoice/model_args.py`

 * *Files identical despite different names*

### Comparing `verifyvoice-0.1.31/verifyvoice/modules.py` & `verifyvoice-0.1.32/verifyvoice/modules.py`

 * *Files identical despite different names*

### Comparing `verifyvoice-0.1.31/verifyvoice/utils.py` & `verifyvoice-0.1.32/verifyvoice/utils.py`

 * *Files identical despite different names*

### Comparing `verifyvoice-0.1.31/verifyvoice.egg-info/PKG-INFO` & `verifyvoice-0.1.32/verifyvoice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verifyvoice
-Version: 0.1.31
+Version: 0.1.32
 Summary: A package for verifying the voice of a person
 Home-page: https://github.com/NirmalSankalana/VerifiVoice
 Author: Nirmal Sankalana, Nipun Thejan
 Author-email: sankalana.nirmal@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `verifyvoice-0.1.31/verifyvoice.egg-info/SOURCES.txt` & `verifyvoice-0.1.32/verifyvoice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

