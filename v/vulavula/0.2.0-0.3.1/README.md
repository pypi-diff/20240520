# Comparing `tmp/vulavula-0.2.0.tar.gz` & `tmp/vulavula-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vulavula-0.2.0.tar", last modified: Tue May 14 08:04:04 2024, max compression
+gzip compressed data, was "vulavula-0.3.1.tar", last modified: Mon May 20 10:04:53 2024, max compression
```

## Comparing `vulavula-0.2.0.tar` & `vulavula-0.3.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     5347 2024-05-14 08:02:22.995087 vulavula-0.2.0/README.md
--rw-r--r--   0        0        0      912 2024-05-14 08:04:04.815674 vulavula-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-16 06:16:28.668957 vulavula-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 15:37:52.520889 vulavula-0.2.0/tests/audio/test1.mp3
--rw-r--r--   0        0        0     3284 2024-05-01 17:41:53.376004 vulavula-0.2.0/tests/test_nlu.py
--rw-r--r--   0        0        0     2150 2024-05-01 17:41:53.376223 vulavula-0.2.0/tests/test_sentiment.py
--rw-r--r--   0        0        0     3435 2024-05-14 08:02:22.995802 vulavula-0.2.0/tests/test_transcribe.py
--rw-r--r--   0        0        0     1884 2024-05-01 17:41:53.376685 vulavula-0.2.0/tests/test_transport.py
--rw-r--r--   0        0        0       35 2024-05-01 17:41:53.376769 vulavula-0.2.0/vulavula/__init__.py
--rw-r--r--   0        0        0       35 2024-05-01 17:41:53.376848 vulavula-0.2.0/vulavula/client/__init__.py
--rw-r--r--   0        0        0     3901 2024-05-14 08:02:22.996329 vulavula-0.2.0/vulavula/client/client.py
--rw-r--r--   0        0        0     4555 2024-05-01 17:41:53.377242 vulavula-0.2.0/vulavula/client/nlu.py
--rw-r--r--   0        0        0     2704 2024-05-01 17:41:53.377347 vulavula-0.2.0/vulavula/client/sentiment.py
--rw-r--r--   0        0        0     5586 2024-05-14 08:02:22.996533 vulavula-0.2.0/vulavula/client/transcribe.py
--rw-r--r--   0        0        0     3633 2024-05-01 17:41:53.377741 vulavula-0.2.0/vulavula/client/transport.py
--rw-r--r--   0        0        0        1 2024-05-01 17:41:53.377828 vulavula-0.2.0/vulavula/common/__init__.py
--rw-r--r--   0        0        0      942 2024-05-01 17:41:53.378112 vulavula-0.2.0/vulavula/common/error_handler.py
--rw-r--r--   0        0        0     2748 2024-05-01 17:41:53.378366 vulavula-0.2.0/vulavula/common/response_handler.py
--rw-r--r--   0        0        0       29 2024-05-01 17:41:53.378448 vulavula-0.2.0/vulavula/config/__init__.py
--rw-r--r--   0        0        0      323 2024-05-01 17:41:53.378562 vulavula-0.2.0/vulavula/config/config.py
--rw-r--r--   0        0        0        1 2024-05-01 17:41:53.378636 vulavula-0.2.0/vulavula/models/__init__.py
--rw-r--r--   0        0        0      220 2024-05-01 17:41:53.378712 vulavula-0.2.0/vulavula/models/types/__init__.py
--rw-r--r--   0        0        0      105 2024-05-01 17:41:53.378800 vulavula-0.2.0/vulavula/models/types/entity_recognition.py
--rw-r--r--   0        0        0     1529 2024-05-01 17:41:53.378896 vulavula-0.2.0/vulavula/models/types/intent_classification.py
--rw-r--r--   0        0        0      105 2024-05-01 17:41:53.378976 vulavula-0.2.0/vulavula/models/types/sentiment_analysis.py
--rw-r--r--   0        0        0     5979 1970-01-01 00:00:00.000000 vulavula-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     5347 2024-05-14 08:02:22.995087 vulavula-0.3.1/README.md
+-rw-r--r--   0        0        0      912 2024-05-20 10:04:53.479219 vulavula-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-16 06:16:28.668957 vulavula-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 15:37:52.520889 vulavula-0.3.1/tests/audio/test1.mp3
+-rw-r--r--   0        0        0     3284 2024-05-01 17:41:53.376004 vulavula-0.3.1/tests/test_nlu.py
+-rw-r--r--   0        0        0     2150 2024-05-01 17:41:53.376223 vulavula-0.3.1/tests/test_sentiment.py
+-rw-r--r--   0        0        0     3435 2024-05-14 08:02:22.995802 vulavula-0.3.1/tests/test_transcribe.py
+-rw-r--r--   0        0        0     1884 2024-05-01 17:41:53.376685 vulavula-0.3.1/tests/test_transport.py
+-rw-r--r--   0        0        0       35 2024-05-01 17:41:53.376769 vulavula-0.3.1/vulavula/__init__.py
+-rw-r--r--   0        0        0       35 2024-05-01 17:41:53.376848 vulavula-0.3.1/vulavula/client/__init__.py
+-rw-r--r--   0        0        0     3901 2024-05-14 08:02:22.996329 vulavula-0.3.1/vulavula/client/client.py
+-rw-r--r--   0        0        0     4555 2024-05-01 17:41:53.377242 vulavula-0.3.1/vulavula/client/nlu.py
+-rw-r--r--   0        0        0     2704 2024-05-01 17:41:53.377347 vulavula-0.3.1/vulavula/client/sentiment.py
+-rw-r--r--   0        0        0     5586 2024-05-14 08:02:22.996533 vulavula-0.3.1/vulavula/client/transcribe.py
+-rw-r--r--   0        0        0     3633 2024-05-01 17:41:53.377741 vulavula-0.3.1/vulavula/client/transport.py
+-rw-r--r--   0        0        0        1 2024-05-01 17:41:53.377828 vulavula-0.3.1/vulavula/common/__init__.py
+-rw-r--r--   0        0        0      942 2024-05-01 17:41:53.378112 vulavula-0.3.1/vulavula/common/error_handler.py
+-rw-r--r--   0        0        0     2748 2024-05-01 17:41:53.378366 vulavula-0.3.1/vulavula/common/response_handler.py
+-rw-r--r--   0        0        0       29 2024-05-01 17:41:53.378448 vulavula-0.3.1/vulavula/config/__init__.py
+-rw-r--r--   0        0        0      347 2024-05-20 10:04:18.868694 vulavula-0.3.1/vulavula/config/config.py
+-rw-r--r--   0        0        0        1 2024-05-01 17:41:53.378636 vulavula-0.3.1/vulavula/models/__init__.py
+-rw-r--r--   0        0        0      220 2024-05-01 17:41:53.378712 vulavula-0.3.1/vulavula/models/types/__init__.py
+-rw-r--r--   0        0        0      105 2024-05-01 17:41:53.378800 vulavula-0.3.1/vulavula/models/types/entity_recognition.py
+-rw-r--r--   0        0        0     1529 2024-05-01 17:41:53.378896 vulavula-0.3.1/vulavula/models/types/intent_classification.py
+-rw-r--r--   0        0        0      105 2024-05-01 17:41:53.378976 vulavula-0.3.1/vulavula/models/types/sentiment_analysis.py
+-rw-r--r--   0        0        0     5979 1970-01-01 00:00:00.000000 vulavula-0.3.1/PKG-INFO
```

### Comparing `vulavula-0.2.0/README.md` & `vulavula-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `vulavula-0.2.0/pyproject.toml` & `vulavula-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "vulavula"
-version = "0.2.0"
+version = "0.3.1"
 description = "The vulavula Python SDK provides access to the Vulavula API."
 authors = [
     { name = "Raphael Karanja", email = "raphael.karanja@lelapa.ai" },
 ]
 dependencies = [
     "requests>=2.31.0",
     "pydantic[dotenv]>=2.7.1",
```

### Comparing `vulavula-0.2.0/tests/test_nlu.py` & `vulavula-0.3.1/tests/test_nlu.py`

 * *Files identical despite different names*

### Comparing `vulavula-0.2.0/tests/test_sentiment.py` & `vulavula-0.3.1/tests/test_sentiment.py`

 * *Files identical despite different names*

### Comparing `vulavula-0.2.0/tests/test_transcribe.py` & `vulavula-0.3.1/tests/test_transcribe.py`

 * *Files identical despite different names*

### Comparing `vulavula-0.2.0/tests/test_transport.py` & `vulavula-0.3.1/tests/test_transport.py`

 * *Files identical despite different names*

### Comparing `vulavula-0.2.0/vulavula/client/client.py` & `vulavula-0.3.1/vulavula/client/client.py`

 * *Files identical despite different names*

### Comparing `vulavula-0.2.0/vulavula/client/nlu.py` & `vulavula-0.3.1/vulavula/client/nlu.py`

 * *Files identical despite different names*

### Comparing `vulavula-0.2.0/vulavula/client/sentiment.py` & `vulavula-0.3.1/vulavula/client/sentiment.py`

 * *Files identical despite different names*

### Comparing `vulavula-0.2.0/vulavula/client/transcribe.py` & `vulavula-0.3.1/vulavula/client/transcribe.py`

 * *Files identical despite different names*

### Comparing `vulavula-0.2.0/vulavula/client/transport.py` & `vulavula-0.3.1/vulavula/client/transport.py`

 * *Files identical despite different names*

### Comparing `vulavula-0.2.0/vulavula/common/error_handler.py` & `vulavula-0.3.1/vulavula/common/error_handler.py`

 * *Files identical despite different names*

### Comparing `vulavula-0.2.0/vulavula/common/response_handler.py` & `vulavula-0.3.1/vulavula/common/response_handler.py`

 * *Files identical despite different names*

### Comparing `vulavula-0.2.0/vulavula/models/types/intent_classification.py` & `vulavula-0.3.1/vulavula/models/types/intent_classification.py`

 * *Files identical despite different names*

### Comparing `vulavula-0.2.0/PKG-INFO` & `vulavula-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulavula
-Version: 0.2.0
+Version: 0.3.1
 Summary: The vulavula Python SDK provides access to the Vulavula API.
 Keywords: lelapa,vulavula,nlp,intent,multilingual,transcription
 Author-Email: Raphael Karanja <raphael.karanja@lelapa.ai>
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

