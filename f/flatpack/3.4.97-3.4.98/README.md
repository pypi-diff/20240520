# Comparing `tmp/flatpack-3.4.97.tar.gz` & `tmp/flatpack-3.4.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatpack-3.4.97.tar", last modified: Mon May 20 19:08:11 2024, max compression
+gzip compressed data, was "flatpack-3.4.98.tar", last modified: Mon May 20 19:20:53 2024, max compression
```

## Comparing `flatpack-3.4.97.tar` & `flatpack-3.4.98.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-20 19:08:11.479733 flatpack-3.4.97/
--rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.4.97/LICENSE
--rw-r--r--   0 romlingroup   (501) staff       (20)     6058 2024-05-20 19:08:11.479538 flatpack-3.4.97/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)     5267 2024-05-20 17:36:41.000000 flatpack-3.4.97/README.md
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-20 19:08:11.477717 flatpack-3.4.97/flatpack/
--rw-r--r--   0 romlingroup   (501) staff       (20)      138 2024-05-02 14:39:05.000000 flatpack-3.4.97/flatpack/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     2494 2024-05-02 07:38:12.000000 flatpack-3.4.97/flatpack/agent_manager.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.4.97/flatpack/config.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.4.97/flatpack/datasets.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-20 19:08:11.478741 flatpack-3.4.97/flatpack/engines/
--rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:17:03.000000 flatpack-3.4.97/flatpack/engines/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     3995 2024-05-20 19:05:21.000000 flatpack-3.4.97/flatpack/engines/engine_llama_cpp.py
--rw-rw-r--   0 romlingroup   (501) staff       (20)     1057 2023-09-28 21:46:27.000000 flatpack-3.4.97/flatpack/instructions.py
--rw-r--r--   0 romlingroup   (501) staff       (20)       52 2024-05-18 04:12:26.000000 flatpack-3.4.97/flatpack/load_engines.py
--rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-01-31 06:56:56.000000 flatpack-3.4.97/flatpack/load_modules.py
--rw-r--r--   0 romlingroup   (501) staff       (20)    35257 2024-05-20 16:30:51.000000 flatpack-3.4.97/flatpack/main.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-20 19:08:11.479095 flatpack-3.4.97/flatpack/modules/
--rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.4.97/flatpack/modules/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.4.97/flatpack/modules/lstm.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.4.97/flatpack/modules/rnn.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     6983 2024-05-14 17:52:21.000000 flatpack-3.4.97/flatpack/parsers.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      290 2024-04-27 11:31:48.000000 flatpack-3.4.97/flatpack/session_manager.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.4.97/flatpack/utils.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     8543 2024-05-20 15:16:59.000000 flatpack-3.4.97/flatpack/vector_manager.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-20 19:08:11.479287 flatpack-3.4.97/flatpack.egg-info/
--rw-r--r--   0 romlingroup   (501) staff       (20)     6058 2024-05-20 19:08:11.000000 flatpack-3.4.97/flatpack.egg-info/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)      636 2024-05-20 19:08:11.000000 flatpack-3.4.97/flatpack.egg-info/SOURCES.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-05-20 19:08:11.000000 flatpack-3.4.97/flatpack.egg-info/dependency_links.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-05-20 19:08:11.000000 flatpack-3.4.97/flatpack.egg-info/entry_points.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)      288 2024-05-20 19:08:11.000000 flatpack-3.4.97/flatpack.egg-info/requires.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-05-20 19:08:11.000000 flatpack-3.4.97/flatpack.egg-info/top_level.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-05-20 19:08:11.479776 flatpack-3.4.97/setup.cfg
--rw-r--r--   0 romlingroup   (501) staff       (20)     1054 2024-05-20 19:07:58.000000 flatpack-3.4.97/setup.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-20 19:20:53.897662 flatpack-3.4.98/
+-rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.4.98/LICENSE
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6058 2024-05-20 19:20:53.897460 flatpack-3.4.98/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)     5267 2024-05-20 19:20:44.000000 flatpack-3.4.98/README.md
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-20 19:20:53.895863 flatpack-3.4.98/flatpack/
+-rw-r--r--   0 romlingroup   (501) staff       (20)      138 2024-05-02 14:39:05.000000 flatpack-3.4.98/flatpack/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     2494 2024-05-02 07:38:12.000000 flatpack-3.4.98/flatpack/agent_manager.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.4.98/flatpack/config.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.4.98/flatpack/datasets.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-20 19:20:53.896749 flatpack-3.4.98/flatpack/engines/
+-rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:17:03.000000 flatpack-3.4.98/flatpack/engines/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     3995 2024-05-20 19:05:21.000000 flatpack-3.4.98/flatpack/engines/engine_llama_cpp.py
+-rw-rw-r--   0 romlingroup   (501) staff       (20)     1057 2023-09-28 21:46:27.000000 flatpack-3.4.98/flatpack/instructions.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)       52 2024-05-18 04:12:26.000000 flatpack-3.4.98/flatpack/load_engines.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-01-31 06:56:56.000000 flatpack-3.4.98/flatpack/load_modules.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)    35257 2024-05-20 16:30:51.000000 flatpack-3.4.98/flatpack/main.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-20 19:20:53.897067 flatpack-3.4.98/flatpack/modules/
+-rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.4.98/flatpack/modules/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.4.98/flatpack/modules/lstm.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.4.98/flatpack/modules/rnn.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6983 2024-05-14 17:52:21.000000 flatpack-3.4.98/flatpack/parsers.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      290 2024-04-27 11:31:48.000000 flatpack-3.4.98/flatpack/session_manager.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.4.98/flatpack/utils.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     8543 2024-05-20 15:16:59.000000 flatpack-3.4.98/flatpack/vector_manager.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-20 19:20:53.897227 flatpack-3.4.98/flatpack.egg-info/
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6058 2024-05-20 19:20:53.000000 flatpack-3.4.98/flatpack.egg-info/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)      636 2024-05-20 19:20:53.000000 flatpack-3.4.98/flatpack.egg-info/SOURCES.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-05-20 19:20:53.000000 flatpack-3.4.98/flatpack.egg-info/dependency_links.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-05-20 19:20:53.000000 flatpack-3.4.98/flatpack.egg-info/entry_points.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)      288 2024-05-20 19:20:53.000000 flatpack-3.4.98/flatpack.egg-info/requires.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-05-20 19:20:53.000000 flatpack-3.4.98/flatpack.egg-info/top_level.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-05-20 19:20:53.897701 flatpack-3.4.98/setup.cfg
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1054 2024-05-20 19:20:30.000000 flatpack-3.4.98/setup.py
```

### Comparing `flatpack-3.4.97/LICENSE` & `flatpack-3.4.98/LICENSE`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.97/PKG-INFO` & `flatpack-3.4.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.4.97
+Version: 3.4.98
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
@@ -128,8 +128,8 @@
 
 - **[toml](https://pypi.org/project/toml/)**\
   MIT License (MIT) ([LICENSE](https://github.com/uiri/toml/blob/master/LICENSE))
 
 - **[uvicorn](https://pypi.org/project/uvicorn/)**\
   BSD License ([LICENSE](https://github.com/encode/uvicorn/blob/master/LICENSE.md))
 
-Last updated: 2024-04-27
+Last updated: 2024-05-20
```

### Comparing `flatpack-3.4.97/README.md` & `flatpack-3.4.98/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -101,8 +101,8 @@
 
 - **[toml](https://pypi.org/project/toml/)**\
   MIT License (MIT) ([LICENSE](https://github.com/uiri/toml/blob/master/LICENSE))
 
 - **[uvicorn](https://pypi.org/project/uvicorn/)**\
   BSD License ([LICENSE](https://github.com/encode/uvicorn/blob/master/LICENSE.md))
 
-Last updated: 2024-04-27
+Last updated: 2024-05-20
```

### Comparing `flatpack-3.4.97/flatpack/agent_manager.py` & `flatpack-3.4.98/flatpack/agent_manager.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.97/flatpack/datasets.py` & `flatpack-3.4.98/flatpack/datasets.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.97/flatpack/engines/engine_llama_cpp.py` & `flatpack-3.4.98/flatpack/engines/engine_llama_cpp.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.97/flatpack/instructions.py` & `flatpack-3.4.98/flatpack/instructions.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.97/flatpack/main.py` & `flatpack-3.4.98/flatpack/main.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.97/flatpack/modules/lstm.py` & `flatpack-3.4.98/flatpack/modules/lstm.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.97/flatpack/modules/rnn.py` & `flatpack-3.4.98/flatpack/modules/rnn.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.97/flatpack/parsers.py` & `flatpack-3.4.98/flatpack/parsers.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.97/flatpack/vector_manager.py` & `flatpack-3.4.98/flatpack/vector_manager.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.97/flatpack.egg-info/PKG-INFO` & `flatpack-3.4.98/flatpack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.4.97
+Version: 3.4.98
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
@@ -128,8 +128,8 @@
 
 - **[toml](https://pypi.org/project/toml/)**\
   MIT License (MIT) ([LICENSE](https://github.com/uiri/toml/blob/master/LICENSE))
 
 - **[uvicorn](https://pypi.org/project/uvicorn/)**\
   BSD License ([LICENSE](https://github.com/encode/uvicorn/blob/master/LICENSE.md))
 
-Last updated: 2024-04-27
+Last updated: 2024-05-20
```

### Comparing `flatpack-3.4.97/flatpack.egg-info/SOURCES.txt` & `flatpack-3.4.98/flatpack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.97/setup.py` & `flatpack-3.4.98/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="flatpack",
-    version="3.4.97",
+    version="3.4.98",
     license="Apache Software License (Apache-2.0)",
     packages=find_packages(),
     install_requires=[
         "beautifulsoup4==4.12.3",
         "cryptography==42.0.6",
         "faiss-cpu==1.8.0",
         "fastapi==0.110.2",
```

