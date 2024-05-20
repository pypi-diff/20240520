# Comparing `tmp/git_migrator-1.0.0.tar.gz` & `tmp/git_migrator-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_migrator-1.0.0.tar", last modified: Mon May 20 18:01:57 2024, max compression
+gzip compressed data, was "git_migrator-1.0.1.tar", last modified: Mon May 20 18:03:54 2024, max compression
```

## Comparing `git_migrator-1.0.0.tar` & `git_migrator-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxr-x   0 n4n5      (1000) n4n5      (1000)        0 2024-05-20 18:01:57.285489 git_migrator-1.0.0/
--rw-rw-r--   0 n4n5      (1000) n4n5      (1000)     1061 2024-05-20 15:28:59.000000 git_migrator-1.0.0/LICENSE
--rw-r--r--   0 n4n5      (1000) n4n5      (1000)     2066 2024-05-20 18:01:57.285489 git_migrator-1.0.0/PKG-INFO
--rw-rw-r--   0 n4n5      (1000) n4n5      (1000)      245 2024-05-20 18:00:00.000000 git_migrator-1.0.0/README.md
-drwxrwxr-x   0 n4n5      (1000) n4n5      (1000)        0 2024-05-20 18:01:57.285489 git_migrator-1.0.0/git_migrator/
--rw-rw-r--   0 n4n5      (1000) n4n5      (1000)     6403 2024-05-20 17:58:06.000000 git_migrator-1.0.0/git_migrator/__init__.py
--rw-rw-r--   0 n4n5      (1000) n4n5      (1000)      187 2024-05-20 17:46:26.000000 git_migrator-1.0.0/git_migrator/__main__.py
-drwxrwxr-x   0 n4n5      (1000) n4n5      (1000)        0 2024-05-20 18:01:57.285489 git_migrator-1.0.0/git_migrator.egg-info/
--rw-r--r--   0 n4n5      (1000) n4n5      (1000)     2066 2024-05-20 18:01:57.000000 git_migrator-1.0.0/git_migrator.egg-info/PKG-INFO
--rw-rw-r--   0 n4n5      (1000) n4n5      (1000)      261 2024-05-20 18:01:57.000000 git_migrator-1.0.0/git_migrator.egg-info/SOURCES.txt
--rw-rw-r--   0 n4n5      (1000) n4n5      (1000)        1 2024-05-20 18:01:57.000000 git_migrator-1.0.0/git_migrator.egg-info/dependency_links.txt
--rw-rw-r--   0 n4n5      (1000) n4n5      (1000)       17 2024-05-20 18:01:57.000000 git_migrator-1.0.0/git_migrator.egg-info/requires.txt
--rw-rw-r--   0 n4n5      (1000) n4n5      (1000)       13 2024-05-20 18:01:57.000000 git_migrator-1.0.0/git_migrator.egg-info/top_level.txt
--rw-rw-r--   0 n4n5      (1000) n4n5      (1000)      719 2024-05-20 18:01:27.000000 git_migrator-1.0.0/pyproject.toml
--rw-rw-r--   0 n4n5      (1000) n4n5      (1000)       38 2024-05-20 18:01:57.285489 git_migrator-1.0.0/setup.cfg
+drwxrwxr-x   0 n4n5      (1000) n4n5      (1000)        0 2024-05-20 18:03:54.436440 git_migrator-1.0.1/
+-rw-rw-r--   0 n4n5      (1000) n4n5      (1000)     1061 2024-05-20 15:28:59.000000 git_migrator-1.0.1/LICENSE
+-rw-r--r--   0 n4n5      (1000) n4n5      (1000)     2019 2024-05-20 18:03:54.436440 git_migrator-1.0.1/PKG-INFO
+-rw-rw-r--   0 n4n5      (1000) n4n5      (1000)      245 2024-05-20 18:00:00.000000 git_migrator-1.0.1/README.md
+drwxrwxr-x   0 n4n5      (1000) n4n5      (1000)        0 2024-05-20 18:03:54.436440 git_migrator-1.0.1/git_migrator/
+-rw-rw-r--   0 n4n5      (1000) n4n5      (1000)     6403 2024-05-20 17:58:06.000000 git_migrator-1.0.1/git_migrator/__init__.py
+-rw-rw-r--   0 n4n5      (1000) n4n5      (1000)      187 2024-05-20 17:46:26.000000 git_migrator-1.0.1/git_migrator/__main__.py
+drwxrwxr-x   0 n4n5      (1000) n4n5      (1000)        0 2024-05-20 18:03:54.436440 git_migrator-1.0.1/git_migrator.egg-info/
+-rw-r--r--   0 n4n5      (1000) n4n5      (1000)     2019 2024-05-20 18:03:54.000000 git_migrator-1.0.1/git_migrator.egg-info/PKG-INFO
+-rw-rw-r--   0 n4n5      (1000) n4n5      (1000)      226 2024-05-20 18:03:54.000000 git_migrator-1.0.1/git_migrator.egg-info/SOURCES.txt
+-rw-rw-r--   0 n4n5      (1000) n4n5      (1000)        1 2024-05-20 18:03:54.000000 git_migrator-1.0.1/git_migrator.egg-info/dependency_links.txt
+-rw-rw-r--   0 n4n5      (1000) n4n5      (1000)       13 2024-05-20 18:03:54.000000 git_migrator-1.0.1/git_migrator.egg-info/top_level.txt
+-rw-rw-r--   0 n4n5      (1000) n4n5      (1000)      698 2024-05-20 18:03:31.000000 git_migrator-1.0.1/pyproject.toml
+-rw-rw-r--   0 n4n5      (1000) n4n5      (1000)       38 2024-05-20 18:03:54.436440 git_migrator-1.0.1/setup.cfg
```

### Comparing `git_migrator-1.0.0/LICENSE` & `git_migrator-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `git_migrator-1.0.0/PKG-INFO` & `git_migrator-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git_migrator
-Version: 1.0.0
+Version: 1.0.1
 Summary: Migrate git repositories
 Author-email: n4n5 <its.just.n4n5@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 n4n5
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,16 +30,14 @@
 Keywords: png,tools,cli
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: dotenv
-Requires-Dist: gitpython
 
 # git-migrator
 
 ## Usage
 
 ```bash
 python -m pip install git_migrator
```

### Comparing `git_migrator-1.0.0/git_migrator/__init__.py` & `git_migrator-1.0.1/git_migrator/__init__.py`

 * *Files identical despite different names*

### Comparing `git_migrator-1.0.0/git_migrator.egg-info/PKG-INFO` & `git_migrator-1.0.1/git_migrator.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git_migrator
-Version: 1.0.0
+Version: 1.0.1
 Summary: Migrate git repositories
 Author-email: n4n5 <its.just.n4n5@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 n4n5
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,16 +30,14 @@
 Keywords: png,tools,cli
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: dotenv
-Requires-Dist: gitpython
 
 # git-migrator
 
 ## Usage
 
 ```bash
 python -m pip install git_migrator
```

### Comparing `git_migrator-1.0.0/pyproject.toml` & `git_migrator-1.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "git_migrator"
-version = "1.0.0"
+version = "1.0.1"
 description = "Migrate git repositories"
 readme = "README.md"
 authors = [{ name = "n4n5", email = "its.just.n4n5@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["png", "tools", "cli"]
 requires-python = ">=3.6"
 
-dependencies = ["dotenv", "gitpython"]
+dependencies = []
 
 
 [project.urls]
 Homepage = "https://github.com/its-just-nans/git-migrator"
 "Bug Tracker" = "https://github.com/its-just-nans/git-migrator/issues"
```

