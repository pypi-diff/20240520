# Comparing `tmp/hermes_cai-0.0.2.tar.gz` & `tmp/hermes_cai-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hermes_cai-0.0.2.tar", last modified: Mon May 20 20:56:10 2024, max compression
+gzip compressed data, was "hermes_cai-0.0.3.tar", last modified: Mon May 20 20:59:08 2024, max compression
```

## Comparing `hermes_cai-0.0.2.tar` & `hermes_cai-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,13 @@
-drwxr-xr-x   0 jamesgroeneveld   (501) staff       (20)        0 2024-05-20 20:56:10.735803 hermes_cai-0.0.2/
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)     3563 2024-05-20 20:56:10.735650 hermes_cai-0.0.2/PKG-INFO
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)     3220 2024-05-20 20:22:55.000000 hermes_cai-0.0.2/README.md
-drwxr-xr-x   0 jamesgroeneveld   (501) staff       (20)        0 2024-05-20 20:56:10.735509 hermes_cai-0.0.2/hermes_cai.egg-info/
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)     3563 2024-05-20 20:56:10.000000 hermes_cai-0.0.2/hermes_cai.egg-info/PKG-INFO
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)      154 2024-05-20 20:56:10.000000 hermes_cai-0.0.2/hermes_cai.egg-info/SOURCES.txt
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)        1 2024-05-20 20:56:10.000000 hermes_cai-0.0.2/hermes_cai.egg-info/dependency_links.txt
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)        1 2024-05-20 20:56:10.000000 hermes_cai-0.0.2/hermes_cai.egg-info/top_level.txt
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)       38 2024-05-20 20:56:10.735838 hermes_cai-0.0.2/setup.cfg
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)      599 2024-05-20 20:56:07.000000 hermes_cai-0.0.2/setup.py
+drwxr-xr-x   0 jamesgroeneveld   (501) staff       (20)        0 2024-05-20 20:59:08.904085 hermes_cai-0.0.3/
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)     3563 2024-05-20 20:59:08.903880 hermes_cai-0.0.3/PKG-INFO
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)     3220 2024-05-20 20:22:55.000000 hermes_cai-0.0.3/README.md
+drwxr-xr-x   0 jamesgroeneveld   (501) staff       (20)        0 2024-05-20 20:59:08.902885 hermes_cai-0.0.3/hermes_cai/
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)        0 2024-05-20 20:22:55.000000 hermes_cai-0.0.3/hermes_cai/__init__.py
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)      556 2024-05-20 20:54:56.000000 hermes_cai-0.0.3/hermes_cai/constants.py
+drwxr-xr-x   0 jamesgroeneveld   (501) staff       (20)        0 2024-05-20 20:59:08.903707 hermes_cai-0.0.3/hermes_cai.egg-info/
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)     3563 2024-05-20 20:59:08.000000 hermes_cai-0.0.3/hermes_cai.egg-info/PKG-INFO
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)      201 2024-05-20 20:59:08.000000 hermes_cai-0.0.3/hermes_cai.egg-info/SOURCES.txt
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)        1 2024-05-20 20:59:08.000000 hermes_cai-0.0.3/hermes_cai.egg-info/dependency_links.txt
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)       11 2024-05-20 20:59:08.000000 hermes_cai-0.0.3/hermes_cai.egg-info/top_level.txt
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)       38 2024-05-20 20:59:08.904124 hermes_cai-0.0.3/setup.cfg
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)      613 2024-05-20 20:58:51.000000 hermes_cai-0.0.3/setup.py
```

### Comparing `hermes_cai-0.0.2/PKG-INFO` & `hermes_cai-0.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: hermes-cai
-Version: 0.0.2
-Summary: Defining and constructing production-grade prompts via an expressive templating engine.
-Home-page: https://github.com/character-tech/chat-stack
-Author: James Groeneveld
-Author-email: james@character.ai
-License: MIT
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-
 # Hermes
 Defining and constructing production-grade LLM prompts via rich structured templates.
 
 ### Goals & Requirements
 - Centralized: By centralizing the prompt construction into one place Hermes aims to simplify prompt the prompt construction mechanics.
 - Extensible: Make it as easy as possible to create new prompts for new use cases.
 - Experimentation: Must be easy to experiment with new prompt data and placements.
```

### Comparing `hermes_cai-0.0.2/README.md` & `hermes_cai-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: hermes-cai
+Version: 0.0.3
+Summary: Defining and constructing production-grade prompts via an expressive templating engine.
+Home-page: https://github.com/character-tech/chat-stack
+Author: James Groeneveld
+Author-email: james@character.ai
+License: MIT
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+
 # Hermes
 Defining and constructing production-grade LLM prompts via rich structured templates.
 
 ### Goals & Requirements
 - Centralized: By centralizing the prompt construction into one place Hermes aims to simplify prompt the prompt construction mechanics.
 - Extensible: Make it as easy as possible to create new prompts for new use cases.
 - Experimentation: Must be easy to experiment with new prompt data and placements.
```

### Comparing `hermes_cai-0.0.2/hermes_cai.egg-info/PKG-INFO` & `hermes_cai-0.0.3/hermes_cai.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hermes-cai
-Version: 0.0.2
+Version: 0.0.3
 Summary: Defining and constructing production-grade prompts via an expressive templating engine.
 Home-page: https://github.com/character-tech/chat-stack
 Author: James Groeneveld
 Author-email: james@character.ai
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

