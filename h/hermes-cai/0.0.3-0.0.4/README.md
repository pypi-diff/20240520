# Comparing `tmp/hermes_cai-0.0.3.tar.gz` & `tmp/hermes_cai-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hermes_cai-0.0.3.tar", last modified: Mon May 20 20:59:08 2024, max compression
+gzip compressed data, was "hermes_cai-0.0.4.tar", last modified: Mon May 20 21:50:06 2024, max compression
```

## Comparing `hermes_cai-0.0.3.tar` & `hermes_cai-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jamesgroeneveld   (501) staff       (20)        0 2024-05-20 20:59:08.904085 hermes_cai-0.0.3/
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)     3563 2024-05-20 20:59:08.903880 hermes_cai-0.0.3/PKG-INFO
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)     3220 2024-05-20 20:22:55.000000 hermes_cai-0.0.3/README.md
-drwxr-xr-x   0 jamesgroeneveld   (501) staff       (20)        0 2024-05-20 20:59:08.902885 hermes_cai-0.0.3/hermes_cai/
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)        0 2024-05-20 20:22:55.000000 hermes_cai-0.0.3/hermes_cai/__init__.py
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)      556 2024-05-20 20:54:56.000000 hermes_cai-0.0.3/hermes_cai/constants.py
-drwxr-xr-x   0 jamesgroeneveld   (501) staff       (20)        0 2024-05-20 20:59:08.903707 hermes_cai-0.0.3/hermes_cai.egg-info/
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)     3563 2024-05-20 20:59:08.000000 hermes_cai-0.0.3/hermes_cai.egg-info/PKG-INFO
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)      201 2024-05-20 20:59:08.000000 hermes_cai-0.0.3/hermes_cai.egg-info/SOURCES.txt
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)        1 2024-05-20 20:59:08.000000 hermes_cai-0.0.3/hermes_cai.egg-info/dependency_links.txt
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)       11 2024-05-20 20:59:08.000000 hermes_cai-0.0.3/hermes_cai.egg-info/top_level.txt
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)       38 2024-05-20 20:59:08.904124 hermes_cai-0.0.3/setup.cfg
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)      613 2024-05-20 20:58:51.000000 hermes_cai-0.0.3/setup.py
+drwxr-xr-x   0 jamesgroeneveld   (501) staff       (20)        0 2024-05-20 21:50:06.250128 hermes_cai-0.0.4/
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)     3563 2024-05-20 21:50:06.249961 hermes_cai-0.0.4/PKG-INFO
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)     3220 2024-05-20 20:22:55.000000 hermes_cai-0.0.4/README.md
+drwxr-xr-x   0 jamesgroeneveld   (501) staff       (20)        0 2024-05-20 21:50:06.248967 hermes_cai-0.0.4/hermes_cai/
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)        0 2024-05-20 20:22:55.000000 hermes_cai-0.0.4/hermes_cai/__init__.py
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)      556 2024-05-20 20:54:56.000000 hermes_cai-0.0.4/hermes_cai/constants.py
+drwxr-xr-x   0 jamesgroeneveld   (501) staff       (20)        0 2024-05-20 21:50:06.249793 hermes_cai-0.0.4/hermes_cai.egg-info/
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)     3563 2024-05-20 21:50:06.000000 hermes_cai-0.0.4/hermes_cai.egg-info/PKG-INFO
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)      201 2024-05-20 21:50:06.000000 hermes_cai-0.0.4/hermes_cai.egg-info/SOURCES.txt
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)        1 2024-05-20 21:50:06.000000 hermes_cai-0.0.4/hermes_cai.egg-info/dependency_links.txt
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)       11 2024-05-20 21:50:06.000000 hermes_cai-0.0.4/hermes_cai.egg-info/top_level.txt
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)       38 2024-05-20 21:50:06.250175 hermes_cai-0.0.4/setup.cfg
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)      694 2024-05-20 21:28:43.000000 hermes_cai-0.0.4/setup.py
```

### Comparing `hermes_cai-0.0.3/PKG-INFO` & `hermes_cai-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hermes-cai
-Version: 0.0.3
+Version: 0.0.4
 Summary: Defining and constructing production-grade prompts via an expressive templating engine.
 Home-page: https://github.com/character-tech/chat-stack
 Author: James Groeneveld
 Author-email: james@character.ai
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `hermes_cai-0.0.3/README.md` & `hermes_cai-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `hermes_cai-0.0.3/hermes_cai/constants.py` & `hermes_cai-0.0.4/hermes_cai/constants.py`

 * *Files identical despite different names*

### Comparing `hermes_cai-0.0.3/hermes_cai.egg-info/PKG-INFO` & `hermes_cai-0.0.4/hermes_cai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hermes-cai
-Version: 0.0.3
+Version: 0.0.4
 Summary: Defining and constructing production-grade prompts via an expressive templating engine.
 Home-page: https://github.com/character-tech/chat-stack
 Author: James Groeneveld
 Author-email: james@character.ai
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `hermes_cai-0.0.3/setup.py` & `hermes_cai-0.0.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 """Setup file for the Hermes package."""
 
 from setuptools import find_packages, setup
 
+with open("VERSION") as version_file:
+    version = version_file.read().strip()
+
 setup(
     name="hermes-cai",
-    version="0.0.3",
+    version=version,
     packages=find_packages(include=["hermes_cai", "hermes_cai.*"]),
     install_requires=[],
     author="James Groeneveld",
     author_email="james@character.ai",
     description="Defining and constructing production-grade prompts via an expressive templating engine.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

