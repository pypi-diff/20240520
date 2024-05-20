# Comparing `tmp/soupsavvy-0.1.4.tar.gz` & `tmp/soupsavvy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soupsavvy-0.1.4.tar", last modified: Mon Apr 15 15:46:49 2024, max compression
+gzip compressed data, was "soupsavvy-0.1.5.tar", last modified: Mon May 20 01:15:47 2024, max compression
```

## Comparing `soupsavvy-0.1.4.tar` & `soupsavvy-0.1.5.tar`

### file list

```diff
@@ -1,41 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:49.791740 soupsavvy-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8564 2024-04-15 15:46:49.791740 soupsavvy-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6068 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 15:46:49.791740 soupsavvy-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:49.787739 soupsavvy-0.1.4/soupsavvy/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 15:46:36.000000 soupsavvy-0.1.4/soupsavvy/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-15 15:46:36.000000 soupsavvy-0.1.4/soupsavvy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:49.787739 soupsavvy-0.1.4/soupsavvy/tags/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/soupsavvy/tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9419 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/soupsavvy/tags/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11288 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/soupsavvy/tags/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/soupsavvy/tags/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/soupsavvy/tags/namespace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:49.787739 soupsavvy-0.1.4/soupsavvy/testing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/soupsavvy/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:49.787739 soupsavvy-0.1.4/soupsavvy/testing/generators/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/soupsavvy/testing/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/soupsavvy/testing/generators/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/soupsavvy/testing/generators/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11025 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/soupsavvy/testing/generators/generators.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/soupsavvy/testing/generators/namespace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:49.791740 soupsavvy-0.1.4/soupsavvy/testing/generators/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/soupsavvy/testing/generators/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/soupsavvy/testing/generators/templates/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/soupsavvy/testing/generators/templates/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/soupsavvy/testing/generators/templates/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:49.791740 soupsavvy-0.1.4/soupsavvy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/soupsavvy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/soupsavvy/utils/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-15 15:46:33.000000 soupsavvy-0.1.4/soupsavvy/utils/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:46:49.791740 soupsavvy-0.1.4/soupsavvy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8564 2024-04-15 15:46:49.000000 soupsavvy-0.1.4/soupsavvy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-15 15:46:49.000000 soupsavvy-0.1.4/soupsavvy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 15:46:49.000000 soupsavvy-0.1.4/soupsavvy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-15 15:46:49.000000 soupsavvy-0.1.4/soupsavvy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-15 15:46:49.000000 soupsavvy-0.1.4/soupsavvy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:47.131610 soupsavvy-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8448 2024-05-20 01:15:47.131610 soupsavvy-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 01:15:47.131610 soupsavvy-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:47.127611 soupsavvy-0.1.5/soupsavvy/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-20 01:15:35.000000 soupsavvy-0.1.5/soupsavvy/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-20 01:15:35.000000 soupsavvy-0.1.5/soupsavvy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:47.127611 soupsavvy-0.1.5/soupsavvy/tags/
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/tags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20610 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/tags/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17316 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/tags/combinators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15556 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/tags/components.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:47.127611 soupsavvy-0.1.5/soupsavvy/tags/css/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/tags/css/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/tags/css/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18511 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/tags/css/tag_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/tags/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/tags/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/tags/tag_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:47.127611 soupsavvy-0.1.5/soupsavvy/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:47.131610 soupsavvy-0.1.5/soupsavvy/testing/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/testing/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/testing/generators/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/testing/generators/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11025 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/testing/generators/generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/testing/generators/namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:47.131610 soupsavvy-0.1.5/soupsavvy/testing/generators/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/testing/generators/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/testing/generators/templates/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/testing/generators/templates/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/testing/generators/templates/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:47.131610 soupsavvy-0.1.5/soupsavvy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/utils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:47.131610 soupsavvy-0.1.5/soupsavvy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8448 2024-05-20 01:15:47.000000 soupsavvy-0.1.5/soupsavvy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-20 01:15:47.000000 soupsavvy-0.1.5/soupsavvy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 01:15:47.000000 soupsavvy-0.1.5/soupsavvy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-20 01:15:47.000000 soupsavvy-0.1.5/soupsavvy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 01:15:47.000000 soupsavvy-0.1.5/soupsavvy.egg-info/top_level.txt
```

### Comparing `soupsavvy-0.1.4/LICENSE` & `soupsavvy-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `soupsavvy-0.1.4/PKG-INFO` & `soupsavvy-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soupsavvy
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python package for advanced web scraping
 Author: sewcio543
 License: MIT License
         
         Copyright (c) 2024 Wojciech Seweryn
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -56,15 +56,15 @@
 
 -----------------
 
 ## Python package that makes web-scraping more manageable
 
 | | |
 | --- | --- |
-| Package | ![Deployment PyPI](https://github.com/sewcio543/soupsavvy/actions/workflows/production_release.yml/badge.svg) ![Deployment test PyPI](https://github.com/sewcio543/soupsavvy/actions/workflows/development_release.yml/badge.svg) [![GitHub](https://img.shields.io/badge/GitHub-sewcio543-181717.svg?style=flat&logo=github)](https://github.com/sewcio543) [![PyPI](https://img.shields.io/pypi/v/soupsavvy?color=orange)](https://pypi.org/project/soupsavvy/) [![Python Versions](https://img.shields.io/pypi/pyversions/soupsavvy)](https://www.python.org/)|
+| Package | ![Deployment PyPI](https://github.com/sewcio543/soupsavvy/actions/workflows/production_release.yml/badge.svg) [![GitHub](https://img.shields.io/badge/GitHub-sewcio543-181717.svg?style=flat&logo=github)](https://github.com/sewcio543) [![PyPI](https://img.shields.io/pypi/v/soupsavvy?color=orange)](https://pypi.org/project/soupsavvy/) [![Python Versions](https://img.shields.io/pypi/pyversions/soupsavvy)](https://www.python.org/)|
 | Testing | ![Tests](https://github.com/sewcio543/soupsavvy/actions/workflows/tests.yml/badge.svg) [![Codecov](https://codecov.io/gh/sewcio543/soupsavvy/graph/badge.svg?token=RZ51VS3QLB)](https://codecov.io/gh/sewcio543/soupsavvy)|
 | Code Quality | ![Build](https://github.com/sewcio543/soupsavvy/actions/workflows/build_package.yml/badge.svg) ![Linting](https://github.com/sewcio543/soupsavvy/actions/workflows/linting.yml/badge.svg) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sewcio543/soupsavvy/main.svg)](https://results.pre-commit.ci/latest/github/sewcio543/soupsavvy/main)|
 | Documentation | [![readthedocs](https://img.shields.io/readthedocs/pip?logo=readthedocs)](https://github.com/sewcio543/soupsavvy/actions/workflows/documentation.yml/badge.svg) [![Docs link](https://img.shields.io/badge/docs-check_out-blue)](https://sewcio543.github.io/soupsavvy/)|
 
 ## Table of Contents
 
 - [About](#about)
```

### Comparing `soupsavvy-0.1.4/README.md` & `soupsavvy-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 -----------------
 
 ## Python package that makes web-scraping more manageable
 
 | | |
 | --- | --- |
-| Package | ![Deployment PyPI](https://github.com/sewcio543/soupsavvy/actions/workflows/production_release.yml/badge.svg) ![Deployment test PyPI](https://github.com/sewcio543/soupsavvy/actions/workflows/development_release.yml/badge.svg) [![GitHub](https://img.shields.io/badge/GitHub-sewcio543-181717.svg?style=flat&logo=github)](https://github.com/sewcio543) [![PyPI](https://img.shields.io/pypi/v/soupsavvy?color=orange)](https://pypi.org/project/soupsavvy/) [![Python Versions](https://img.shields.io/pypi/pyversions/soupsavvy)](https://www.python.org/)|
+| Package | ![Deployment PyPI](https://github.com/sewcio543/soupsavvy/actions/workflows/production_release.yml/badge.svg) [![GitHub](https://img.shields.io/badge/GitHub-sewcio543-181717.svg?style=flat&logo=github)](https://github.com/sewcio543) [![PyPI](https://img.shields.io/pypi/v/soupsavvy?color=orange)](https://pypi.org/project/soupsavvy/) [![Python Versions](https://img.shields.io/pypi/pyversions/soupsavvy)](https://www.python.org/)|
 | Testing | ![Tests](https://github.com/sewcio543/soupsavvy/actions/workflows/tests.yml/badge.svg) [![Codecov](https://codecov.io/gh/sewcio543/soupsavvy/graph/badge.svg?token=RZ51VS3QLB)](https://codecov.io/gh/sewcio543/soupsavvy)|
 | Code Quality | ![Build](https://github.com/sewcio543/soupsavvy/actions/workflows/build_package.yml/badge.svg) ![Linting](https://github.com/sewcio543/soupsavvy/actions/workflows/linting.yml/badge.svg) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sewcio543/soupsavvy/main.svg)](https://results.pre-commit.ci/latest/github/sewcio543/soupsavvy/main)|
 | Documentation | [![readthedocs](https://img.shields.io/readthedocs/pip?logo=readthedocs)](https://github.com/sewcio543/soupsavvy/actions/workflows/documentation.yml/badge.svg) [![Docs link](https://img.shields.io/badge/docs-check_out-blue)](https://sewcio543.github.io/soupsavvy/)|
 
 ## Table of Contents
 
 - [About](#about)
```

### Comparing `soupsavvy-0.1.4/pyproject.toml` & `soupsavvy-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `soupsavvy-0.1.4/soupsavvy/tags/exceptions.py` & `soupsavvy-0.1.5/soupsavvy/tags/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,12 +47,12 @@
 
     BeautifulSoup constructor always wraps NavigableString in <p> element.
     It is rather an unexpected behavior and should rather be avoided in SelectableSoup
     find method, thus this exception is raised.
     """
 
 
-class NotSelectableSoupException(SelectableSoupException):
+class NotSelectableSoupException(SelectableSoupException, TypeError):
     """
     Exception to be raised when function excepted SelectableSoup as input
     and got argument of the different, invalid type.
     """
```

### Comparing `soupsavvy-0.1.4/soupsavvy/testing/generators/base.py` & `soupsavvy-0.1.5/soupsavvy/testing/generators/base.py`

 * *Files identical despite different names*

### Comparing `soupsavvy-0.1.4/soupsavvy/testing/generators/exceptions.py` & `soupsavvy-0.1.5/soupsavvy/testing/generators/exceptions.py`

 * *Files identical despite different names*

### Comparing `soupsavvy-0.1.4/soupsavvy/testing/generators/generators.py` & `soupsavvy-0.1.5/soupsavvy/testing/generators/generators.py`

 * *Files identical despite different names*

### Comparing `soupsavvy-0.1.4/soupsavvy/testing/generators/templates/base.py` & `soupsavvy-0.1.5/soupsavvy/testing/generators/templates/base.py`

 * *Files identical despite different names*

### Comparing `soupsavvy-0.1.4/soupsavvy/testing/generators/templates/templates.py` & `soupsavvy-0.1.5/soupsavvy/testing/generators/templates/templates.py`

 * *Files identical despite different names*

### Comparing `soupsavvy-0.1.4/soupsavvy/utils/deprecation.py` & `soupsavvy-0.1.5/soupsavvy/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `soupsavvy-0.1.4/soupsavvy.egg-info/PKG-INFO` & `soupsavvy-0.1.5/soupsavvy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soupsavvy
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python package for advanced web scraping
 Author: sewcio543
 License: MIT License
         
         Copyright (c) 2024 Wojciech Seweryn
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -56,15 +56,15 @@
 
 -----------------
 
 ## Python package that makes web-scraping more manageable
 
 | | |
 | --- | --- |
-| Package | ![Deployment PyPI](https://github.com/sewcio543/soupsavvy/actions/workflows/production_release.yml/badge.svg) ![Deployment test PyPI](https://github.com/sewcio543/soupsavvy/actions/workflows/development_release.yml/badge.svg) [![GitHub](https://img.shields.io/badge/GitHub-sewcio543-181717.svg?style=flat&logo=github)](https://github.com/sewcio543) [![PyPI](https://img.shields.io/pypi/v/soupsavvy?color=orange)](https://pypi.org/project/soupsavvy/) [![Python Versions](https://img.shields.io/pypi/pyversions/soupsavvy)](https://www.python.org/)|
+| Package | ![Deployment PyPI](https://github.com/sewcio543/soupsavvy/actions/workflows/production_release.yml/badge.svg) [![GitHub](https://img.shields.io/badge/GitHub-sewcio543-181717.svg?style=flat&logo=github)](https://github.com/sewcio543) [![PyPI](https://img.shields.io/pypi/v/soupsavvy?color=orange)](https://pypi.org/project/soupsavvy/) [![Python Versions](https://img.shields.io/pypi/pyversions/soupsavvy)](https://www.python.org/)|
 | Testing | ![Tests](https://github.com/sewcio543/soupsavvy/actions/workflows/tests.yml/badge.svg) [![Codecov](https://codecov.io/gh/sewcio543/soupsavvy/graph/badge.svg?token=RZ51VS3QLB)](https://codecov.io/gh/sewcio543/soupsavvy)|
 | Code Quality | ![Build](https://github.com/sewcio543/soupsavvy/actions/workflows/build_package.yml/badge.svg) ![Linting](https://github.com/sewcio543/soupsavvy/actions/workflows/linting.yml/badge.svg) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sewcio543/soupsavvy/main.svg)](https://results.pre-commit.ci/latest/github/sewcio543/soupsavvy/main)|
 | Documentation | [![readthedocs](https://img.shields.io/readthedocs/pip?logo=readthedocs)](https://github.com/sewcio543/soupsavvy/actions/workflows/documentation.yml/badge.svg) [![Docs link](https://img.shields.io/badge/docs-check_out-blue)](https://sewcio543.github.io/soupsavvy/)|
 
 ## Table of Contents
 
 - [About](#about)
```

### Comparing `soupsavvy-0.1.4/soupsavvy.egg-info/SOURCES.txt` & `soupsavvy-0.1.5/soupsavvy.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -9,17 +9,22 @@
 soupsavvy.egg-info/PKG-INFO
 soupsavvy.egg-info/SOURCES.txt
 soupsavvy.egg-info/dependency_links.txt
 soupsavvy.egg-info/requires.txt
 soupsavvy.egg-info/top_level.txt
 soupsavvy/tags/__init__.py
 soupsavvy/tags/base.py
+soupsavvy/tags/combinators.py
 soupsavvy/tags/components.py
 soupsavvy/tags/exceptions.py
 soupsavvy/tags/namespace.py
+soupsavvy/tags/tag_utils.py
+soupsavvy/tags/css/__init__.py
+soupsavvy/tags/css/exceptions.py
+soupsavvy/tags/css/tag_selectors.py
 soupsavvy/testing/__init__.py
 soupsavvy/testing/generators/__init__.py
 soupsavvy/testing/generators/base.py
 soupsavvy/testing/generators/exceptions.py
 soupsavvy/testing/generators/generators.py
 soupsavvy/testing/generators/namespace.py
 soupsavvy/testing/generators/templates/__init__.py
```

