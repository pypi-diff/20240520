# Comparing `tmp/audiostack-1.3.0.tar.gz` & `tmp/audiostack-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiostack-1.3.0.tar", last modified: Wed May  8 15:53:40 2024, max compression
+gzip compressed data, was "audiostack-1.3.1.tar", last modified: Mon May 20 08:16:31 2024, max compression
```

## Comparing `audiostack-1.3.0.tar` & `audiostack-1.3.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 15:53:40.317243 audiostack-1.3.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1061 2024-05-08 15:53:07.000000 audiostack-1.3.0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5458 2024-05-08 15:53:40.317243 audiostack-1.3.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4963 2024-05-08 15:53:07.000000 audiostack-1.3.0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 15:53:40.309243 audiostack-1.3.0/audiostack/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      441 2024-05-08 15:53:33.000000 audiostack-1.3.0/audiostack/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 15:53:40.313243 audiostack-1.3.0/audiostack/content/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      592 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/content/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6077 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/content/file.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2270 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/content/media.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2088 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/content/recommend.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      947 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/content/root_functions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4183 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/content/script.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 15:53:40.313243 audiostack-1.3.0/audiostack/delivery/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       92 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/delivery/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3462 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/delivery/encoder.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2078 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/delivery/video.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 15:53:40.313243 audiostack-1.3.0/audiostack/docs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       47 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/docs/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      631 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/docs/docs.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 15:53:40.313243 audiostack-1.3.0/audiostack/helpers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/helpers/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      715 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/helpers/api_item.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      972 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/helpers/api_list.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4732 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/helpers/request_interface.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      163 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/helpers/request_types.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      338 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/helpers/response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      227 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/helpers/util.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 15:53:40.313243 audiostack-1.3.0/audiostack/orchestrator/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       58 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/orchestrator/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 15:53:40.313243 audiostack-1.3.0/audiostack/production/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      134 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/production/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4801 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/production/mix.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4286 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/production/sound.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4265 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/production/suite.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 15:53:40.317243 audiostack-1.3.0/audiostack/speech/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/speech/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2979 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/speech/diction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1298 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/speech/predict.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7488 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/speech/tts.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2189 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/speech/voice.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 15:53:40.317243 audiostack-1.3.0/audiostack.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5458 2024-05-08 15:53:40.000000 audiostack-1.3.0/audiostack.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1074 2024-05-08 15:53:40.000000 audiostack-1.3.0/audiostack.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-08 15:53:40.000000 audiostack-1.3.0/audiostack.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       45 2024-05-08 15:53:40.000000 audiostack-1.3.0/audiostack.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       11 2024-05-08 15:53:40.000000 audiostack-1.3.0/audiostack.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-08 15:53:40.317243 audiostack-1.3.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1039 2024-05-08 15:53:07.000000 audiostack-1.3.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 08:16:31.350443 audiostack-1.3.1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1061 2024-05-20 08:16:07.000000 audiostack-1.3.1/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5458 2024-05-20 08:16:31.346442 audiostack-1.3.1/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4963 2024-05-20 08:16:07.000000 audiostack-1.3.1/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 08:16:31.342442 audiostack-1.3.1/audiostack/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2024-05-20 08:16:24.000000 audiostack-1.3.1/audiostack/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 08:16:31.342442 audiostack-1.3.1/audiostack/content/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      592 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/content/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6077 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/content/file.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2270 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/content/media.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2088 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/content/recommend.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      947 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/content/root_functions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4183 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/content/script.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 08:16:31.346442 audiostack-1.3.1/audiostack/delivery/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       92 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/delivery/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3462 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/delivery/encoder.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2078 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/delivery/video.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 08:16:31.346442 audiostack-1.3.1/audiostack/docs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       47 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/docs/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      631 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/docs/docs.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 08:16:31.346442 audiostack-1.3.1/audiostack/helpers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/helpers/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      715 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/helpers/api_item.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      972 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/helpers/api_list.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4732 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/helpers/request_interface.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      163 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/helpers/request_types.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      338 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/helpers/response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      227 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/helpers/util.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 08:16:31.346442 audiostack-1.3.1/audiostack/orchestrator/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       58 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/orchestrator/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 08:16:31.346442 audiostack-1.3.1/audiostack/production/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      134 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/production/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4801 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/production/mix.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4286 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/production/sound.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4265 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/production/suite.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 08:16:31.346442 audiostack-1.3.1/audiostack/speech/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/speech/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2979 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/speech/diction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1298 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/speech/predict.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7488 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/speech/tts.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2189 2024-05-20 08:16:07.000000 audiostack-1.3.1/audiostack/speech/voice.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 08:16:31.346442 audiostack-1.3.1/audiostack.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5458 2024-05-20 08:16:31.000000 audiostack-1.3.1/audiostack.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1074 2024-05-20 08:16:31.000000 audiostack-1.3.1/audiostack.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-20 08:16:31.000000 audiostack-1.3.1/audiostack.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       45 2024-05-20 08:16:31.000000 audiostack-1.3.1/audiostack.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       11 2024-05-20 08:16:31.000000 audiostack-1.3.1/audiostack.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-20 08:16:31.350443 audiostack-1.3.1/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1039 2024-05-20 08:16:07.000000 audiostack-1.3.1/setup.py
```

### Comparing `audiostack-1.3.0/LICENSE` & `audiostack-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `audiostack-1.3.0/PKG-INFO` & `audiostack-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiostack
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python SDK for Audiostack API
 Home-page: https://github.com/aflorithmic/audiostack-python
 Author: Aflorithmic
 Author-email: sam@aflorithmic.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: audiostack Version: 1.3.0 Summary: Python SDK for
+Metadata-Version: 2.1 Name: audiostack Version: 1.3.1 Summary: Python SDK for
 Audiostack API Home-page: https://github.com/aflorithmic/audiostack-python
 Author: Aflorithmic Author-email: sam@aflorithmic.ai Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 requests>=2.28.1; python_version >= "3.6"
                                _[_a_p_i_._a_u_d_i_o_ _l_o_g_o_]
```

### Comparing `audiostack-1.3.0/README.md` & `audiostack-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `audiostack-1.3.0/audiostack/content/__init__.py` & `audiostack-1.3.1/audiostack/content/__init__.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.3.0/audiostack/content/file.py` & `audiostack-1.3.1/audiostack/content/file.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.3.0/audiostack/content/media.py` & `audiostack-1.3.1/audiostack/content/media.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.3.0/audiostack/content/recommend.py` & `audiostack-1.3.1/audiostack/content/recommend.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.3.0/audiostack/content/root_functions.py` & `audiostack-1.3.1/audiostack/content/root_functions.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.3.0/audiostack/content/script.py` & `audiostack-1.3.1/audiostack/content/script.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.3.0/audiostack/delivery/encoder.py` & `audiostack-1.3.1/audiostack/delivery/encoder.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.3.0/audiostack/delivery/video.py` & `audiostack-1.3.1/audiostack/delivery/video.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.3.0/audiostack/docs/docs.py` & `audiostack-1.3.1/audiostack/docs/docs.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.3.0/audiostack/helpers/api_item.py` & `audiostack-1.3.1/audiostack/helpers/api_item.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.3.0/audiostack/helpers/api_list.py` & `audiostack-1.3.1/audiostack/helpers/api_list.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.3.0/audiostack/helpers/request_interface.py` & `audiostack-1.3.1/audiostack/helpers/request_interface.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.3.0/audiostack/production/mix.py` & `audiostack-1.3.1/audiostack/production/mix.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.3.0/audiostack/production/sound.py` & `audiostack-1.3.1/audiostack/production/sound.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.3.0/audiostack/production/suite.py` & `audiostack-1.3.1/audiostack/production/suite.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.3.0/audiostack/speech/diction.py` & `audiostack-1.3.1/audiostack/speech/diction.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.3.0/audiostack/speech/predict.py` & `audiostack-1.3.1/audiostack/speech/predict.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.3.0/audiostack/speech/tts.py` & `audiostack-1.3.1/audiostack/speech/tts.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.3.0/audiostack/speech/voice.py` & `audiostack-1.3.1/audiostack/speech/voice.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.3.0/audiostack.egg-info/PKG-INFO` & `audiostack-1.3.1/audiostack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiostack
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python SDK for Audiostack API
 Home-page: https://github.com/aflorithmic/audiostack-python
 Author: Aflorithmic
 Author-email: sam@aflorithmic.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: audiostack Version: 1.3.0 Summary: Python SDK for
+Metadata-Version: 2.1 Name: audiostack Version: 1.3.1 Summary: Python SDK for
 Audiostack API Home-page: https://github.com/aflorithmic/audiostack-python
 Author: Aflorithmic Author-email: sam@aflorithmic.ai Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 requests>=2.28.1; python_version >= "3.6"
                                _[_a_p_i_._a_u_d_i_o_ _l_o_g_o_]
```

### Comparing `audiostack-1.3.0/audiostack.egg-info/SOURCES.txt` & `audiostack-1.3.1/audiostack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audiostack-1.3.0/setup.py` & `audiostack-1.3.1/setup.py`

 * *Files identical despite different names*

