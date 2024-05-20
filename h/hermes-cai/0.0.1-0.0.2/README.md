# Comparing `tmp/hermes_cai-0.0.1.tar.gz` & `tmp/hermes_cai-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hermes_cai-0.0.1.tar", last modified: Mon May 20 20:44:42 2024, max compression
+gzip compressed data, was "hermes_cai-0.0.2.tar", last modified: Mon May 20 20:56:10 2024, max compression
```

## Comparing `hermes_cai-0.0.1.tar` & `hermes_cai-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,10 @@
-drwxr-xr-x   0 jamesgroeneveld   (501) staff       (20)        0 2024-05-20 20:44:42.054423 hermes_cai-0.0.1/
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)     3563 2024-05-20 20:44:42.054277 hermes_cai-0.0.1/PKG-INFO
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)     3220 2024-05-20 20:22:55.000000 hermes_cai-0.0.1/README.md
-drwxr-xr-x   0 jamesgroeneveld   (501) staff       (20)        0 2024-05-20 20:44:42.054139 hermes_cai-0.0.1/hermes_cai.egg-info/
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)     3563 2024-05-20 20:44:42.000000 hermes_cai-0.0.1/hermes_cai.egg-info/PKG-INFO
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)      187 2024-05-20 20:44:42.000000 hermes_cai-0.0.1/hermes_cai.egg-info/SOURCES.txt
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)        1 2024-05-20 20:44:42.000000 hermes_cai-0.0.1/hermes_cai.egg-info/dependency_links.txt
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)        4 2024-05-20 20:44:42.000000 hermes_cai-0.0.1/hermes_cai.egg-info/top_level.txt
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)       38 2024-05-20 20:44:42.054453 hermes_cai-0.0.1/setup.cfg
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)      599 2024-05-20 20:41:10.000000 hermes_cai-0.0.1/setup.py
-drwxr-xr-x   0 jamesgroeneveld   (501) staff       (20)        0 2024-05-20 20:44:42.053753 hermes_cai-0.0.1/src/
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)        0 2024-05-20 20:22:55.000000 hermes_cai-0.0.1/src/__init__.py
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)      556 2024-05-20 20:22:55.000000 hermes_cai-0.0.1/src/constants.py
+drwxr-xr-x   0 jamesgroeneveld   (501) staff       (20)        0 2024-05-20 20:56:10.735803 hermes_cai-0.0.2/
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)     3563 2024-05-20 20:56:10.735650 hermes_cai-0.0.2/PKG-INFO
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)     3220 2024-05-20 20:22:55.000000 hermes_cai-0.0.2/README.md
+drwxr-xr-x   0 jamesgroeneveld   (501) staff       (20)        0 2024-05-20 20:56:10.735509 hermes_cai-0.0.2/hermes_cai.egg-info/
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)     3563 2024-05-20 20:56:10.000000 hermes_cai-0.0.2/hermes_cai.egg-info/PKG-INFO
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)      154 2024-05-20 20:56:10.000000 hermes_cai-0.0.2/hermes_cai.egg-info/SOURCES.txt
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)        1 2024-05-20 20:56:10.000000 hermes_cai-0.0.2/hermes_cai.egg-info/dependency_links.txt
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)        1 2024-05-20 20:56:10.000000 hermes_cai-0.0.2/hermes_cai.egg-info/top_level.txt
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)       38 2024-05-20 20:56:10.735838 hermes_cai-0.0.2/setup.cfg
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)      599 2024-05-20 20:56:07.000000 hermes_cai-0.0.2/setup.py
```

### Comparing `hermes_cai-0.0.1/PKG-INFO` & `hermes_cai-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hermes-cai
-Version: 0.0.1
+Version: 0.0.2
 Summary: Defining and constructing production-grade prompts via an expressive templating engine.
 Home-page: https://github.com/character-tech/chat-stack
 Author: James Groeneveld
 Author-email: james@character.ai
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `hermes_cai-0.0.1/README.md` & `hermes_cai-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `hermes_cai-0.0.1/hermes_cai.egg-info/PKG-INFO` & `hermes_cai-0.0.2/hermes_cai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hermes-cai
-Version: 0.0.1
+Version: 0.0.2
 Summary: Defining and constructing production-grade prompts via an expressive templating engine.
 Home-page: https://github.com/character-tech/chat-stack
 Author: James Groeneveld
 Author-email: james@character.ai
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `hermes_cai-0.0.1/setup.py` & `hermes_cai-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Setup file for the Hermes package."""
 
 from setuptools import find_packages, setup
 
 setup(
     name="hermes-cai",
-    version="0.0.1",
+    version="0.0.2",
     packages=find_packages(include=["src", "src.*"]),
     install_requires=[],
     author="James Groeneveld",
     author_email="james@character.ai",
     description="Defining and constructing production-grade prompts via an expressive templating engine.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

