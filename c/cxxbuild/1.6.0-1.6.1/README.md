# Comparing `tmp/cxxbuild-1.6.0.tar.gz` & `tmp/cxxbuild-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cxxbuild-1.6.0.tar", last modified: Sun May 19 23:21:37 2024, max compression
+gzip compressed data, was "cxxbuild-1.6.1.tar", last modified: Sun May 19 23:33:54 2024, max compression
```

## Comparing `cxxbuild-1.6.0.tar` & `cxxbuild-1.6.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-sr-x   0 root         (0) root         (0)        0 2024-05-19 23:21:37.231684 cxxbuild-1.6.0/
--rw-rw-r--   0 root         (0) root         (0)     1065 2023-11-07 22:41:49.000000 cxxbuild-1.6.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    14541 2024-05-19 23:21:37.231684 cxxbuild-1.6.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12505 2024-05-19 23:20:26.000000 cxxbuild-1.6.0/README.md
-drwxr-sr-x   0 root         (0) root         (0)        0 2024-05-19 23:21:37.227684 cxxbuild-1.6.0/cxxbuild/
--rw-r--r--   0 root         (0) root         (0)       27 2023-12-31 14:16:19.000000 cxxbuild-1.6.0/cxxbuild/__init__.py
--rw-r--r--   0 root         (0) root         (0)    49679 2024-05-19 23:20:26.000000 cxxbuild-1.6.0/cxxbuild/cxxbuild.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2024-05-19 23:21:37.227684 cxxbuild-1.6.0/cxxbuild.egg-info/
--rw-r--r--   0 root         (0) root         (0)    14541 2024-05-19 23:21:37.000000 cxxbuild-1.6.0/cxxbuild.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      277 2024-05-19 23:21:37.000000 cxxbuild-1.6.0/cxxbuild.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-19 23:21:37.000000 cxxbuild-1.6.0/cxxbuild.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-05-19 23:21:37.000000 cxxbuild-1.6.0/cxxbuild.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       49 2024-05-19 23:21:37.000000 cxxbuild-1.6.0/cxxbuild.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-19 23:21:37.000000 cxxbuild-1.6.0/cxxbuild.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      910 2024-05-19 23:20:26.000000 cxxbuild-1.6.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-19 23:21:37.231684 cxxbuild-1.6.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      227 2024-05-19 23:20:26.000000 cxxbuild-1.6.0/setup.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2024-05-19 23:33:54.642930 cxxbuild-1.6.1/
+-rw-rw-r--   0 root         (0) root         (0)     1065 2023-11-07 22:41:49.000000 cxxbuild-1.6.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    14566 2024-05-19 23:33:54.642930 cxxbuild-1.6.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12505 2024-05-19 23:27:19.000000 cxxbuild-1.6.1/README.md
+drwxr-sr-x   0 root         (0) root         (0)        0 2024-05-19 23:33:54.634930 cxxbuild-1.6.1/cxxbuild/
+-rw-r--r--   0 root         (0) root         (0)       27 2023-12-31 14:16:19.000000 cxxbuild-1.6.1/cxxbuild/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    49679 2024-05-19 23:27:19.000000 cxxbuild-1.6.1/cxxbuild/cxxbuild.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2024-05-19 23:33:54.642930 cxxbuild-1.6.1/cxxbuild.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    14566 2024-05-19 23:33:54.000000 cxxbuild-1.6.1/cxxbuild.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      277 2024-05-19 23:33:54.000000 cxxbuild-1.6.1/cxxbuild.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-19 23:33:54.000000 cxxbuild-1.6.1/cxxbuild.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-05-19 23:33:54.000000 cxxbuild-1.6.1/cxxbuild.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2024-05-19 23:33:54.000000 cxxbuild-1.6.1/cxxbuild.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-19 23:33:54.000000 cxxbuild-1.6.1/cxxbuild.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      923 2024-05-19 23:27:19.000000 cxxbuild-1.6.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-19 23:33:54.642930 cxxbuild-1.6.1/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      227 2024-05-19 23:27:19.000000 cxxbuild-1.6.1/setup.py
```

### Comparing `cxxbuild-1.6.0/LICENSE` & `cxxbuild-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cxxbuild-1.6.0/PKG-INFO` & `cxxbuild-1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cxxbuild
-Version: 1.6.0
+Version: 1.6.1
 Summary: CxxBuild is a python script to easily build C++ programs: just invoke 'cxxbuild' and it works!
 Author-email: Igor Machado Coelho <igormcoelho@proton.me>
 License: MIT License
         
         Copyright (c) 2023 manydeps
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,14 +30,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: toml
+Requires-Dist: packaging
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 
@@ -47,15 +48,15 @@
 
 ![C++11](https://img.shields.io/badge/std-c%2B%2B11-blue) ![C++14](https://img.shields.io/badge/std-c%2B%2B14-blue) ![C++17](https://img.shields.io/badge/std-c%2B%2B17-blue) ![C++20](https://img.shields.io/badge/std-c%2B%2B20-blue) ![C++23](https://img.shields.io/badge/std-c%2B%2B23-blue)
 
 [![DOI](https://zenodo.org/badge/715821683.svg)](https://zenodo.org/doi/10.5281/zenodo.10447208)
 
 _**cxxbuild** (or "cplusplusbuild") is a python script to easily generate C/C++ build files for cmake and bazel._
 
-- Version: `cxxbuild version=1.6.0`
+- Version: `cxxbuild version=1.6.1`
 - Installation: `pip install cxxbuild` (or `pipx install cxxbuild` for newer distributions)
 
 For basic introduction, read the post: [Using cxxbuild to easily build C++ project with tests and dependencies](https://igormcoelho.medium.com/using-cxxbuild-to-easily-build-c-project-with-tests-and-dependencies-a3726b453f75)
 
 We know it is very hard to start a C++ project and learn basics of build systems such as CMake and Bazel, and package managers like conan and vcpkg... so just type "cxxbuild" and be happy!
 But you MUST follow the canonical organization below:
```

### Comparing `cxxbuild-1.6.0/README.md` & `cxxbuild-1.6.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ![C++11](https://img.shields.io/badge/std-c%2B%2B11-blue) ![C++14](https://img.shields.io/badge/std-c%2B%2B14-blue) ![C++17](https://img.shields.io/badge/std-c%2B%2B17-blue) ![C++20](https://img.shields.io/badge/std-c%2B%2B20-blue) ![C++23](https://img.shields.io/badge/std-c%2B%2B23-blue)
 
 [![DOI](https://zenodo.org/badge/715821683.svg)](https://zenodo.org/doi/10.5281/zenodo.10447208)
 
 _**cxxbuild** (or "cplusplusbuild") is a python script to easily generate C/C++ build files for cmake and bazel._
 
-- Version: `cxxbuild version=1.6.0`
+- Version: `cxxbuild version=1.6.1`
 - Installation: `pip install cxxbuild` (or `pipx install cxxbuild` for newer distributions)
 
 For basic introduction, read the post: [Using cxxbuild to easily build C++ project with tests and dependencies](https://igormcoelho.medium.com/using-cxxbuild-to-easily-build-c-project-with-tests-and-dependencies-a3726b453f75)
 
 We know it is very hard to start a C++ project and learn basics of build systems such as CMake and Bazel, and package managers like conan and vcpkg... so just type "cxxbuild" and be happy!
 But you MUST follow the canonical organization below:
```

### Comparing `cxxbuild-1.6.0/cxxbuild/cxxbuild.py` & `cxxbuild-1.6.1/cxxbuild/cxxbuild.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import os
 import sys
 import json
 import subprocess
 
 def version():
-    v = "cxxbuild=1.6.0"
+    v = "cxxbuild=1.6.1"
     return v
 
 def usage():
     u=version()+"""
 Usage:
     cxxbuild [build] [ROOT_PATH] 
       builds with cxxbuild, examples:
```

### Comparing `cxxbuild-1.6.0/cxxbuild.egg-info/PKG-INFO` & `cxxbuild-1.6.1/cxxbuild.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cxxbuild
-Version: 1.6.0
+Version: 1.6.1
 Summary: CxxBuild is a python script to easily build C++ programs: just invoke 'cxxbuild' and it works!
 Author-email: Igor Machado Coelho <igormcoelho@proton.me>
 License: MIT License
         
         Copyright (c) 2023 manydeps
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,14 +30,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: toml
+Requires-Dist: packaging
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 
@@ -47,15 +48,15 @@
 
 ![C++11](https://img.shields.io/badge/std-c%2B%2B11-blue) ![C++14](https://img.shields.io/badge/std-c%2B%2B14-blue) ![C++17](https://img.shields.io/badge/std-c%2B%2B17-blue) ![C++20](https://img.shields.io/badge/std-c%2B%2B20-blue) ![C++23](https://img.shields.io/badge/std-c%2B%2B23-blue)
 
 [![DOI](https://zenodo.org/badge/715821683.svg)](https://zenodo.org/doi/10.5281/zenodo.10447208)
 
 _**cxxbuild** (or "cplusplusbuild") is a python script to easily generate C/C++ build files for cmake and bazel._
 
-- Version: `cxxbuild version=1.6.0`
+- Version: `cxxbuild version=1.6.1`
 - Installation: `pip install cxxbuild` (or `pipx install cxxbuild` for newer distributions)
 
 For basic introduction, read the post: [Using cxxbuild to easily build C++ project with tests and dependencies](https://igormcoelho.medium.com/using-cxxbuild-to-easily-build-c-project-with-tests-and-dependencies-a3726b453f75)
 
 We know it is very hard to start a C++ project and learn basics of build systems such as CMake and Bazel, and package managers like conan and vcpkg... so just type "cxxbuild" and be happy!
 But you MUST follow the canonical organization below:
```

### Comparing `cxxbuild-1.6.0/pyproject.toml` & `cxxbuild-1.6.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 
 [build-system]
 requires=["setuptools", "wheel"]
 build-backend="setuptools.build_meta"
 
 [project]
 name="cxxbuild"
-version="1.6.0"
+version="1.6.1"
 description="CxxBuild is a python script to easily build C++ programs: just invoke 'cxxbuild' and it works!"
 readme="README.md"
 authors=[{ name="Igor Machado Coelho", email="igormcoelho@proton.me" }]
 license={ file="LICENSE" }
 classifiers=[
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3"
 ]
 keywords=["build", "cplusplus", "dependencies", "cxxdeps", "cmake", "bazel"]
-dependencies=["toml"]
+dependencies=["toml", "packaging"]
 requires-python=">=3.9"
 
 [project.optional-dependencies]
 dev=["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage="https://github.com/manydeps/cxxbuild"
```

