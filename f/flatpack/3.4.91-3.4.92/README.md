# Comparing `tmp/flatpack-3.4.91.tar.gz` & `tmp/flatpack-3.4.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatpack-3.4.91.tar", last modified: Mon May 20 15:23:46 2024, max compression
+gzip compressed data, was "flatpack-3.4.92.tar", last modified: Mon May 20 15:26:40 2024, max compression
```

## Comparing `flatpack-3.4.91.tar` & `flatpack-3.4.92.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-20 15:23:46.340071 flatpack-3.4.91/
--rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.4.91/LICENSE
--rw-r--r--   0 romlingroup   (501) staff       (20)     6253 2024-05-20 15:23:46.339762 flatpack-3.4.91/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)     5422 2024-05-18 05:22:15.000000 flatpack-3.4.91/README.md
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-20 15:23:46.336606 flatpack-3.4.91/flatpack/
--rw-r--r--   0 romlingroup   (501) staff       (20)      138 2024-05-02 14:39:05.000000 flatpack-3.4.91/flatpack/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     2494 2024-05-02 07:38:12.000000 flatpack-3.4.91/flatpack/agent_manager.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.4.91/flatpack/config.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.4.91/flatpack/datasets.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-20 15:23:46.338214 flatpack-3.4.91/flatpack/engines/
--rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:17:03.000000 flatpack-3.4.91/flatpack/engines/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     2079 2024-05-20 15:23:39.000000 flatpack-3.4.91/flatpack/engines/engine_llama_cpp.py
--rw-rw-r--   0 romlingroup   (501) staff       (20)     1057 2023-09-28 21:46:27.000000 flatpack-3.4.91/flatpack/instructions.py
--rw-r--r--   0 romlingroup   (501) staff       (20)       52 2024-05-18 04:12:26.000000 flatpack-3.4.91/flatpack/load_engines.py
--rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-01-31 06:56:56.000000 flatpack-3.4.91/flatpack/load_modules.py
--rw-r--r--   0 romlingroup   (501) staff       (20)    34886 2024-05-20 14:53:14.000000 flatpack-3.4.91/flatpack/main.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-20 15:23:46.338940 flatpack-3.4.91/flatpack/modules/
--rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.4.91/flatpack/modules/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.4.91/flatpack/modules/lstm.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.4.91/flatpack/modules/rnn.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     6983 2024-05-14 17:52:21.000000 flatpack-3.4.91/flatpack/parsers.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      290 2024-04-27 11:31:48.000000 flatpack-3.4.91/flatpack/session_manager.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.4.91/flatpack/utils.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     8543 2024-05-20 15:16:59.000000 flatpack-3.4.91/flatpack/vector_manager.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-20 15:23:46.339309 flatpack-3.4.91/flatpack.egg-info/
--rw-r--r--   0 romlingroup   (501) staff       (20)     6253 2024-05-20 15:23:46.000000 flatpack-3.4.91/flatpack.egg-info/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)      636 2024-05-20 15:23:46.000000 flatpack-3.4.91/flatpack.egg-info/SOURCES.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-05-20 15:23:46.000000 flatpack-3.4.91/flatpack.egg-info/dependency_links.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-05-20 15:23:46.000000 flatpack-3.4.91/flatpack.egg-info/entry_points.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)      313 2024-05-20 15:23:46.000000 flatpack-3.4.91/flatpack.egg-info/requires.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-05-20 15:23:46.000000 flatpack-3.4.91/flatpack.egg-info/top_level.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-05-20 15:23:46.340133 flatpack-3.4.91/setup.cfg
--rw-r--r--   0 romlingroup   (501) staff       (20)     1090 2024-05-20 15:23:41.000000 flatpack-3.4.91/setup.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-20 15:26:40.268031 flatpack-3.4.92/
+-rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.4.92/LICENSE
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6253 2024-05-20 15:26:40.267730 flatpack-3.4.92/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)     5422 2024-05-18 05:22:15.000000 flatpack-3.4.92/README.md
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-20 15:26:40.264545 flatpack-3.4.92/flatpack/
+-rw-r--r--   0 romlingroup   (501) staff       (20)      138 2024-05-02 14:39:05.000000 flatpack-3.4.92/flatpack/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     2494 2024-05-02 07:38:12.000000 flatpack-3.4.92/flatpack/agent_manager.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.4.92/flatpack/config.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.4.92/flatpack/datasets.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-20 15:26:40.266210 flatpack-3.4.92/flatpack/engines/
+-rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:17:03.000000 flatpack-3.4.92/flatpack/engines/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1593 2024-05-20 15:26:27.000000 flatpack-3.4.92/flatpack/engines/engine_llama_cpp.py
+-rw-rw-r--   0 romlingroup   (501) staff       (20)     1057 2023-09-28 21:46:27.000000 flatpack-3.4.92/flatpack/instructions.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)       52 2024-05-18 04:12:26.000000 flatpack-3.4.92/flatpack/load_engines.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-01-31 06:56:56.000000 flatpack-3.4.92/flatpack/load_modules.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)    34886 2024-05-20 14:53:14.000000 flatpack-3.4.92/flatpack/main.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-20 15:26:40.266989 flatpack-3.4.92/flatpack/modules/
+-rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.4.92/flatpack/modules/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.4.92/flatpack/modules/lstm.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.4.92/flatpack/modules/rnn.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6983 2024-05-14 17:52:21.000000 flatpack-3.4.92/flatpack/parsers.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      290 2024-04-27 11:31:48.000000 flatpack-3.4.92/flatpack/session_manager.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.4.92/flatpack/utils.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     8543 2024-05-20 15:16:59.000000 flatpack-3.4.92/flatpack/vector_manager.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-20 15:26:40.267341 flatpack-3.4.92/flatpack.egg-info/
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6253 2024-05-20 15:26:40.000000 flatpack-3.4.92/flatpack.egg-info/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)      636 2024-05-20 15:26:40.000000 flatpack-3.4.92/flatpack.egg-info/SOURCES.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-05-20 15:26:40.000000 flatpack-3.4.92/flatpack.egg-info/dependency_links.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-05-20 15:26:40.000000 flatpack-3.4.92/flatpack.egg-info/entry_points.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)      313 2024-05-20 15:26:40.000000 flatpack-3.4.92/flatpack.egg-info/requires.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-05-20 15:26:40.000000 flatpack-3.4.92/flatpack.egg-info/top_level.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-05-20 15:26:40.268092 flatpack-3.4.92/setup.cfg
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1090 2024-05-20 15:26:35.000000 flatpack-3.4.92/setup.py
```

### Comparing `flatpack-3.4.91/LICENSE` & `flatpack-3.4.92/LICENSE`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.91/PKG-INFO` & `flatpack-3.4.92/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.4.91
+Version: 3.4.92
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
```

### Comparing `flatpack-3.4.91/README.md` & `flatpack-3.4.92/README.md`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.91/flatpack/agent_manager.py` & `flatpack-3.4.92/flatpack/agent_manager.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.91/flatpack/datasets.py` & `flatpack-3.4.92/flatpack/datasets.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.91/flatpack/engines/engine_llama_cpp.py` & `flatpack-3.4.92/flatpack/engines/engine_llama_cpp.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,12 @@
-import time
-
 from llama_cpp import Llama
 
 
 class LlamaCPPEngine:
     def __init__(self, repo_id=None, filename=None, n_ctx=4096, n_threads=8, verbose=False):
-        start_time = time.time()
-        print("Initializing LlamaCPPEngine...")
-
         if repo_id:
             print(f"Loading model from repo_id: {repo_id}")
             self.model = Llama.from_pretrained(
                 echo=False,
                 filename=filename,
                 n_ctx=n_ctx,
                 n_threads=n_threads,
@@ -32,38 +27,28 @@
                 repeat_penalty=1.0,
                 seed=-1,
                 streaming=True,
                 temp=1.0,
                 verbose=verbose
             )
 
-        print(f"Model loaded in {time.time() - start_time:.2f} seconds")
-
     def generate_response(self, context, question, max_tokens):
         prompt = f"""
         Context: {context}\n
         Question: {question}\n
         """
 
         messages = [
             {"role": "user", "content": prompt}
         ]
 
-        start_time = time.time()
-        print("Generating response...")
-
         response_chunks = self.model.create_chat_completion(
             max_tokens=max_tokens,
             messages=messages,
-            stop=[""],
+            stop=["<|end|>"],
             stream=True
         )
 
-        print(f"Response generation started in {time.time() - start_time:.2f} seconds")
-
         for chunk in response_chunks:
             delta = chunk['choices'][0]['delta']
             if 'content' in delta:
-                print(f"Yielding response chunk: {delta['content']}")
                 yield delta['content']
-
-        print(f"Response generation completed in {time.time() - start_time:.2f} seconds")
```

### Comparing `flatpack-3.4.91/flatpack/instructions.py` & `flatpack-3.4.92/flatpack/instructions.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.91/flatpack/main.py` & `flatpack-3.4.92/flatpack/main.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.91/flatpack/modules/lstm.py` & `flatpack-3.4.92/flatpack/modules/lstm.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.91/flatpack/modules/rnn.py` & `flatpack-3.4.92/flatpack/modules/rnn.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.91/flatpack/parsers.py` & `flatpack-3.4.92/flatpack/parsers.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.91/flatpack/vector_manager.py` & `flatpack-3.4.92/flatpack/vector_manager.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.91/flatpack.egg-info/PKG-INFO` & `flatpack-3.4.92/flatpack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.4.91
+Version: 3.4.92
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
```

### Comparing `flatpack-3.4.91/flatpack.egg-info/SOURCES.txt` & `flatpack-3.4.92/flatpack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.91/setup.py` & `flatpack-3.4.92/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="flatpack",
-    version="3.4.91",
+    version="3.4.92",
     license="Apache Software License (Apache-2.0)",
     packages=find_packages(),
     install_requires=[
         "beautifulsoup4==4.12.3",
         "cryptography==42.0.6",
         "faiss-cpu==1.8.0",
         "fastapi==0.110.2",
```

