# Comparing `tmp/flatpack-3.4.95.tar.gz` & `tmp/flatpack-3.4.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatpack-3.4.95.tar", last modified: Mon May 20 16:31:21 2024, max compression
+gzip compressed data, was "flatpack-3.4.96.tar", last modified: Mon May 20 18:52:02 2024, max compression
```

## Comparing `flatpack-3.4.95.tar` & `flatpack-3.4.96.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-20 16:31:21.135213 flatpack-3.4.95/
--rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.4.95/LICENSE
--rw-r--r--   0 romlingroup   (501) staff       (20)     6253 2024-05-20 16:31:21.134859 flatpack-3.4.95/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)     5422 2024-05-18 05:22:15.000000 flatpack-3.4.95/README.md
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-20 16:31:21.131778 flatpack-3.4.95/flatpack/
--rw-r--r--   0 romlingroup   (501) staff       (20)      138 2024-05-02 14:39:05.000000 flatpack-3.4.95/flatpack/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     2494 2024-05-02 07:38:12.000000 flatpack-3.4.95/flatpack/agent_manager.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.4.95/flatpack/config.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.4.95/flatpack/datasets.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-20 16:31:21.133406 flatpack-3.4.95/flatpack/engines/
--rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:17:03.000000 flatpack-3.4.95/flatpack/engines/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     1530 2024-05-20 15:52:07.000000 flatpack-3.4.95/flatpack/engines/engine_llama_cpp.py
--rw-rw-r--   0 romlingroup   (501) staff       (20)     1057 2023-09-28 21:46:27.000000 flatpack-3.4.95/flatpack/instructions.py
--rw-r--r--   0 romlingroup   (501) staff       (20)       52 2024-05-18 04:12:26.000000 flatpack-3.4.95/flatpack/load_engines.py
--rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-01-31 06:56:56.000000 flatpack-3.4.95/flatpack/load_modules.py
--rw-r--r--   0 romlingroup   (501) staff       (20)    35257 2024-05-20 16:30:51.000000 flatpack-3.4.95/flatpack/main.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-20 16:31:21.134140 flatpack-3.4.95/flatpack/modules/
--rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.4.95/flatpack/modules/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.4.95/flatpack/modules/lstm.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.4.95/flatpack/modules/rnn.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     6983 2024-05-14 17:52:21.000000 flatpack-3.4.95/flatpack/parsers.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      290 2024-04-27 11:31:48.000000 flatpack-3.4.95/flatpack/session_manager.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.4.95/flatpack/utils.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     8543 2024-05-20 15:16:59.000000 flatpack-3.4.95/flatpack/vector_manager.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-20 16:31:21.134476 flatpack-3.4.95/flatpack.egg-info/
--rw-r--r--   0 romlingroup   (501) staff       (20)     6253 2024-05-20 16:31:21.000000 flatpack-3.4.95/flatpack.egg-info/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)      636 2024-05-20 16:31:21.000000 flatpack-3.4.95/flatpack.egg-info/SOURCES.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-05-20 16:31:21.000000 flatpack-3.4.95/flatpack.egg-info/dependency_links.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-05-20 16:31:21.000000 flatpack-3.4.95/flatpack.egg-info/entry_points.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)      313 2024-05-20 16:31:21.000000 flatpack-3.4.95/flatpack.egg-info/requires.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-05-20 16:31:21.000000 flatpack-3.4.95/flatpack.egg-info/top_level.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-05-20 16:31:21.135306 flatpack-3.4.95/setup.cfg
--rw-r--r--   0 romlingroup   (501) staff       (20)     1090 2024-05-20 16:31:11.000000 flatpack-3.4.95/setup.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-20 18:52:02.418917 flatpack-3.4.96/
+-rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.4.96/LICENSE
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6058 2024-05-20 18:52:02.418642 flatpack-3.4.96/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)     5267 2024-05-20 17:36:41.000000 flatpack-3.4.96/README.md
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-20 18:52:02.416266 flatpack-3.4.96/flatpack/
+-rw-r--r--   0 romlingroup   (501) staff       (20)      138 2024-05-02 14:39:05.000000 flatpack-3.4.96/flatpack/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     2494 2024-05-02 07:38:12.000000 flatpack-3.4.96/flatpack/agent_manager.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.4.96/flatpack/config.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.4.96/flatpack/datasets.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-20 18:52:02.417541 flatpack-3.4.96/flatpack/engines/
+-rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:17:03.000000 flatpack-3.4.96/flatpack/engines/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4313 2024-05-20 18:46:04.000000 flatpack-3.4.96/flatpack/engines/engine_llama_cpp.py
+-rw-rw-r--   0 romlingroup   (501) staff       (20)     1057 2023-09-28 21:46:27.000000 flatpack-3.4.96/flatpack/instructions.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)       52 2024-05-18 04:12:26.000000 flatpack-3.4.96/flatpack/load_engines.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-01-31 06:56:56.000000 flatpack-3.4.96/flatpack/load_modules.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)    35257 2024-05-20 16:30:51.000000 flatpack-3.4.96/flatpack/main.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-20 18:52:02.418019 flatpack-3.4.96/flatpack/modules/
+-rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.4.96/flatpack/modules/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.4.96/flatpack/modules/lstm.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.4.96/flatpack/modules/rnn.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6983 2024-05-14 17:52:21.000000 flatpack-3.4.96/flatpack/parsers.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      290 2024-04-27 11:31:48.000000 flatpack-3.4.96/flatpack/session_manager.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.4.96/flatpack/utils.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     8543 2024-05-20 15:16:59.000000 flatpack-3.4.96/flatpack/vector_manager.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-20 18:52:02.418298 flatpack-3.4.96/flatpack.egg-info/
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6058 2024-05-20 18:52:02.000000 flatpack-3.4.96/flatpack.egg-info/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)      636 2024-05-20 18:52:02.000000 flatpack-3.4.96/flatpack.egg-info/SOURCES.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-05-20 18:52:02.000000 flatpack-3.4.96/flatpack.egg-info/dependency_links.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-05-20 18:52:02.000000 flatpack-3.4.96/flatpack.egg-info/entry_points.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)      288 2024-05-20 18:52:02.000000 flatpack-3.4.96/flatpack.egg-info/requires.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-05-20 18:52:02.000000 flatpack-3.4.96/flatpack.egg-info/top_level.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-05-20 18:52:02.418973 flatpack-3.4.96/setup.cfg
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1054 2024-05-20 17:36:51.000000 flatpack-3.4.96/setup.py
```

### Comparing `flatpack-3.4.95/LICENSE` & `flatpack-3.4.96/LICENSE`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.95/PKG-INFO` & `flatpack-3.4.96/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.4.95
+Version: 3.4.96
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
 Requires-Dist: cryptography==42.0.6
 Requires-Dist: faiss-cpu==1.8.0
 Requires-Dist: fastapi==0.110.2
 Requires-Dist: hnswlib==0.8.0
 Requires-Dist: httpx==0.27.0
 Requires-Dist: huggingface-hub==0.23.0
-Requires-Dist: llama-cpp-python==0.2.75
 Requires-Dist: ngrok==1.2.0
 Requires-Dist: nltk==3.8.1
 Requires-Dist: olefile==0.47
 Requires-Dist: psutil==5.9.5
 Requires-Dist: pydantic==2.7.1
 Requires-Dist: pypdf==4.2.0
 Requires-Dist: requests==2.31.0
@@ -99,17 +98,14 @@
 
 - **[httpx](https://pypi.org/project/httpx/)**\
   BSD License ([LICENSE](https://github.com/encode/httpx/blob/master/LICENSE.md))
 
 - **[huggingface-hub](https://pypi.org/project/huggingface-hub/)**\
   Apache Software License (Apache) ([LICENSE](https://github.com/huggingface/huggingface_hub/blob/main/LICENSE))
 
-- **[llama-cpp-python](https://pypi.org/project/llama-cpp-python/)**\
-  MIT ([LICENSE](https://github.com/abetlen/llama-cpp-python/blob/main/LICENSE.md))
-
 - **[ngrok](https://pypi.org/project/ngrok/)**\
   MIT License (MIT OR Apache-2.0) ([LICENSE](https://github.com/ngrok/ngrok-python/blob/main/LICENSE-APACHE))
 
 - **[nltk](https://pypi.org/project/nltk/)**\
   Apache Software License (Apache License, Version 2.0) ([LICENSE](https://github.com/nltk/nltk/blob/develop/LICENSE.txt))
 
 - **[olefile](https://pypi.org/project/olefile/)**\
```

### Comparing `flatpack-3.4.95/README.md` & `flatpack-3.4.96/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -71,17 +71,14 @@
 
 - **[httpx](https://pypi.org/project/httpx/)**\
   BSD License ([LICENSE](https://github.com/encode/httpx/blob/master/LICENSE.md))
 
 - **[huggingface-hub](https://pypi.org/project/huggingface-hub/)**\
   Apache Software License (Apache) ([LICENSE](https://github.com/huggingface/huggingface_hub/blob/main/LICENSE))
 
-- **[llama-cpp-python](https://pypi.org/project/llama-cpp-python/)**\
-  MIT ([LICENSE](https://github.com/abetlen/llama-cpp-python/blob/main/LICENSE.md))
-
 - **[ngrok](https://pypi.org/project/ngrok/)**\
   MIT License (MIT OR Apache-2.0) ([LICENSE](https://github.com/ngrok/ngrok-python/blob/main/LICENSE-APACHE))
 
 - **[nltk](https://pypi.org/project/nltk/)**\
   Apache Software License (Apache License, Version 2.0) ([LICENSE](https://github.com/nltk/nltk/blob/develop/LICENSE.txt))
 
 - **[olefile](https://pypi.org/project/olefile/)**\
```

### Comparing `flatpack-3.4.95/flatpack/agent_manager.py` & `flatpack-3.4.96/flatpack/agent_manager.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.95/flatpack/datasets.py` & `flatpack-3.4.96/flatpack/datasets.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.95/flatpack/instructions.py` & `flatpack-3.4.96/flatpack/instructions.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.95/flatpack/main.py` & `flatpack-3.4.96/flatpack/main.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.95/flatpack/modules/lstm.py` & `flatpack-3.4.96/flatpack/modules/lstm.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.95/flatpack/modules/rnn.py` & `flatpack-3.4.96/flatpack/modules/rnn.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.95/flatpack/parsers.py` & `flatpack-3.4.96/flatpack/parsers.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.95/flatpack/vector_manager.py` & `flatpack-3.4.96/flatpack/vector_manager.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.95/flatpack.egg-info/PKG-INFO` & `flatpack-3.4.96/flatpack.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.4.95
+Version: 3.4.96
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
 Requires-Dist: cryptography==42.0.6
 Requires-Dist: faiss-cpu==1.8.0
 Requires-Dist: fastapi==0.110.2
 Requires-Dist: hnswlib==0.8.0
 Requires-Dist: httpx==0.27.0
 Requires-Dist: huggingface-hub==0.23.0
-Requires-Dist: llama-cpp-python==0.2.75
 Requires-Dist: ngrok==1.2.0
 Requires-Dist: nltk==3.8.1
 Requires-Dist: olefile==0.47
 Requires-Dist: psutil==5.9.5
 Requires-Dist: pydantic==2.7.1
 Requires-Dist: pypdf==4.2.0
 Requires-Dist: requests==2.31.0
@@ -99,17 +98,14 @@
 
 - **[httpx](https://pypi.org/project/httpx/)**\
   BSD License ([LICENSE](https://github.com/encode/httpx/blob/master/LICENSE.md))
 
 - **[huggingface-hub](https://pypi.org/project/huggingface-hub/)**\
   Apache Software License (Apache) ([LICENSE](https://github.com/huggingface/huggingface_hub/blob/main/LICENSE))
 
-- **[llama-cpp-python](https://pypi.org/project/llama-cpp-python/)**\
-  MIT ([LICENSE](https://github.com/abetlen/llama-cpp-python/blob/main/LICENSE.md))
-
 - **[ngrok](https://pypi.org/project/ngrok/)**\
   MIT License (MIT OR Apache-2.0) ([LICENSE](https://github.com/ngrok/ngrok-python/blob/main/LICENSE-APACHE))
 
 - **[nltk](https://pypi.org/project/nltk/)**\
   Apache Software License (Apache License, Version 2.0) ([LICENSE](https://github.com/nltk/nltk/blob/develop/LICENSE.txt))
 
 - **[olefile](https://pypi.org/project/olefile/)**\
```

### Comparing `flatpack-3.4.95/flatpack.egg-info/SOURCES.txt` & `flatpack-3.4.96/flatpack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.95/setup.py` & `flatpack-3.4.96/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="flatpack",
-    version="3.4.95",
+    version="3.4.96",
     license="Apache Software License (Apache-2.0)",
     packages=find_packages(),
     install_requires=[
         "beautifulsoup4==4.12.3",
         "cryptography==42.0.6",
         "faiss-cpu==1.8.0",
         "fastapi==0.110.2",
         "hnswlib==0.8.0",
         "httpx==0.27.0",
         "huggingface-hub==0.23.0",
-        "llama-cpp-python==0.2.75",
         "ngrok==1.2.0",
         "nltk==3.8.1",
         "olefile==0.47",
         "psutil==5.9.5",
         "pydantic==2.7.1",
         "pypdf==4.2.0",
         "requests==2.31.0",
```

