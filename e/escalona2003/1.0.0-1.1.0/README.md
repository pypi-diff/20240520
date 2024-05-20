# Comparing `tmp/escalona2003-1.0.0.tar.gz` & `tmp/escalona2003-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "escalona2003-1.0.0.tar", last modified: Thu Mar  9 18:01:32 2023, max compression
+gzip compressed data, was "escalona2003-1.1.0.tar", last modified: Mon May 20 07:11:59 2024, max compression
```

## Comparing `escalona2003-1.0.0.tar` & `escalona2003-1.1.0.tar`

### file list

```diff
@@ -1,51 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-03-09 18:01:32.057125 escalona2003-1.0.0/
--rw-rw-rw-   0        0        0      316 2023-03-09 17:45:35.000000 escalona2003-1.0.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3343 2023-03-09 17:45:35.000000 escalona2003-1.0.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0      106 2023-03-09 17:45:35.000000 escalona2003-1.0.0/HISTORY.rst
--rw-rw-rw-   0        0        0    20838 2023-03-09 17:45:35.000000 escalona2003-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      440 2023-03-09 17:45:35.000000 escalona2003-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2327 2023-03-09 18:01:32.057125 escalona2003-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1528 2023-03-09 17:45:35.000000 escalona2003-1.0.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-09 18:01:31.149832 escalona2003-1.0.0/doc/
--rw-rw-rw-   0        0        0     6967 2023-03-09 17:45:35.000000 escalona2003-1.0.0/doc/Makefile
--rw-rw-rw-   0        0        0       29 2023-03-09 17:45:35.000000 escalona2003-1.0.0/doc/authors.rst
-drwxrwxrwx   0        0        0        0 2023-03-09 18:01:31.180608 escalona2003-1.0.0/doc/badges/
--rw-rw-rw-   0        0        0      282 2023-03-09 17:45:35.000000 escalona2003-1.0.0/doc/badges/listing.rst
-drwxrwxrwx   0        0        0        0 2023-03-09 18:01:31.205027 escalona2003-1.0.0/doc/biblio/
--rw-rw-rw-   0        0        0      513 2023-03-09 17:45:35.000000 escalona2003-1.0.0/doc/biblio/biblio.rst
--rw-rw-rw-   0        0        0     5124 2023-03-09 17:45:35.000000 escalona2003-1.0.0/doc/conf.py
--rw-rw-rw-   0        0        0       34 2023-03-09 17:45:35.000000 escalona2003-1.0.0/doc/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-03-09 17:45:35.000000 escalona2003-1.0.0/doc/history.rst
--rw-rw-rw-   0        0        0      599 2023-03-09 17:45:35.000000 escalona2003-1.0.0/doc/index.rst
--rw-rw-rw-   0        0        0      222 2023-03-09 17:45:35.000000 escalona2003-1.0.0/doc/installation.rst
--rwxrwxrwx   0        0        0     6731 2023-03-09 17:45:35.000000 escalona2003-1.0.0/doc/make.bat
--rw-rw-rw-   0        0        0      133 2023-03-09 17:45:35.000000 escalona2003-1.0.0/doc/management.rst
--rw-rw-rw-   0        0        0     1445 2023-03-09 17:45:35.000000 escalona2003-1.0.0/doc/readme.rst
--rw-rw-rw-   0        0        0       21 2023-03-09 17:45:35.000000 escalona2003-1.0.0/doc/usage.rst
-drwxrwxrwx   0        0        0        0 2023-03-09 18:01:31.269718 escalona2003-1.0.0/doc/user/
--rw-rw-rw-   0        0        0       86 2023-03-09 17:45:35.000000 escalona2003-1.0.0/doc/user/index.rst
--rw-rw-rw-   0        0        0       66 2023-03-09 17:45:35.000000 escalona2003-1.0.0/doc/user/overview.rst
--rw-rw-rw-   0        0        0      353 2023-03-09 17:45:35.000000 escalona2003-1.0.0/requirements.txt
--rw-rw-rw-   0        0        0       29 2023-03-09 17:45:35.000000 escalona2003-1.0.0/requirements_minimal.txt
--rw-rw-rw-   0        0        0      187 2023-03-09 18:01:32.108425 escalona2003-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1896 2023-03-09 17:45:35.000000 escalona2003-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-09 18:01:30.447237 escalona2003-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-03-09 18:01:31.414952 escalona2003-1.0.0/src/escalona2003/
--rw-rw-rw-   0        0        0      263 2023-03-09 17:45:35.000000 escalona2003-1.0.0/src/escalona2003/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-09 18:01:31.780169 escalona2003-1.0.0/src/escalona2003/clean/
--rw-rw-rw-   0        0        0     1866 2023-03-09 15:56:46.000000 escalona2003-1.0.0/src/escalona2003/clean/daily_carbon_uptake.csv
--rw-rw-rw-   0        0        0     2157 2023-03-09 15:57:06.000000 escalona2003-1.0.0/src/escalona2003/clean/rce.csv
--rw-rw-rw-   0        0        0      134 2023-03-09 17:45:35.000000 escalona2003-1.0.0/src/escalona2003/clean/readme.rst
--rw-rw-rw-   0        0        0      152 2023-03-09 17:45:35.000000 escalona2003-1.0.0/src/escalona2003/info.py
--rw-rw-rw-   0        0        0      367 2023-03-09 17:45:35.000000 escalona2003-1.0.0/src/escalona2003/version.py
-drwxrwxrwx   0        0        0        0 2023-03-09 18:01:31.574998 escalona2003-1.0.0/src/escalona2003.egg-info/
--rw-rw-rw-   0        0        0     2327 2023-03-09 18:01:30.000000 escalona2003-1.0.0/src/escalona2003.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      875 2023-03-09 18:01:30.000000 escalona2003-1.0.0/src/escalona2003.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-09 18:01:30.000000 escalona2003-1.0.0/src/escalona2003.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-09 17:59:42.000000 escalona2003-1.0.0/src/escalona2003.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-03-09 18:01:30.000000 escalona2003-1.0.0/src/escalona2003.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-09 18:01:32.047007 escalona2003-1.0.0/test/
--rw-rw-rw-   0        0        0      976 2023-03-09 17:45:35.000000 escalona2003-1.0.0/test/conftest.py
--rw-rw-rw-   0        0        0      546 2023-03-09 15:57:37.000000 escalona2003-1.0.0/test/test_daily_carbon_uptake.py
--rw-rw-rw-   0        0        0       90 2023-03-09 17:45:35.000000 escalona2003-1.0.0/test/test_packaging.py
--rw-rw-rw-   0        0        0      544 2023-03-09 15:58:02.000000 escalona2003-1.0.0/test/test_rce.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:11:59.867468 escalona2003-1.1.0/
+-rw-rw-rw-   0        0        0      316 2024-05-20 07:07:59.000000 escalona2003-1.1.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3349 2024-05-20 07:07:59.000000 escalona2003-1.1.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0      106 2024-05-20 07:07:59.000000 escalona2003-1.1.0/HISTORY.rst
+-rw-rw-rw-   0        0        0    20838 2024-05-20 07:07:59.000000 escalona2003-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     3371 2024-05-20 07:11:59.867468 escalona2003-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1528 2024-05-20 07:07:59.000000 escalona2003-1.1.0/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-20 07:11:59.837336 escalona2003-1.1.0/doc/
+-rw-rw-rw-   0        0        0     6967 2024-05-20 07:07:59.000000 escalona2003-1.1.0/doc/Makefile
+-rw-rw-rw-   0        0        0       29 2024-05-20 07:07:59.000000 escalona2003-1.1.0/doc/authors.rst
+drwxrwxrwx   0        0        0        0 2024-05-20 07:11:59.839293 escalona2003-1.1.0/doc/badges/
+-rw-rw-rw-   0        0        0      282 2024-05-20 07:07:59.000000 escalona2003-1.1.0/doc/badges/listing.rst
+drwxrwxrwx   0        0        0        0 2024-05-20 07:11:59.842374 escalona2003-1.1.0/doc/biblio/
+-rw-rw-rw-   0        0        0      513 2024-05-20 07:07:59.000000 escalona2003-1.1.0/doc/biblio/biblio.rst
+-rw-rw-rw-   0        0        0     5124 2024-05-20 07:07:59.000000 escalona2003-1.1.0/doc/conf.py
+-rw-rw-rw-   0        0        0       34 2024-05-20 07:07:59.000000 escalona2003-1.1.0/doc/contributing.rst
+-rw-rw-rw-   0        0        0       29 2024-05-20 07:07:59.000000 escalona2003-1.1.0/doc/history.rst
+-rw-rw-rw-   0        0        0      599 2024-05-20 07:07:59.000000 escalona2003-1.1.0/doc/index.rst
+-rw-rw-rw-   0        0        0      222 2024-05-20 07:07:59.000000 escalona2003-1.1.0/doc/installation.rst
+-rwxrwxrwx   0        0        0     6731 2024-05-20 07:07:59.000000 escalona2003-1.1.0/doc/make.bat
+-rw-rw-rw-   0        0        0      133 2024-05-20 07:07:59.000000 escalona2003-1.1.0/doc/management.rst
+-rw-rw-rw-   0        0        0     1453 2024-05-20 07:07:59.000000 escalona2003-1.1.0/doc/readme.rst
+-rw-rw-rw-   0        0        0       21 2024-05-20 07:07:59.000000 escalona2003-1.1.0/doc/usage.rst
+drwxrwxrwx   0        0        0        0 2024-05-20 07:11:59.842374 escalona2003-1.1.0/doc/user/
+-rw-rw-rw-   0        0        0       86 2024-05-20 07:07:59.000000 escalona2003-1.1.0/doc/user/index.rst
+-rw-rw-rw-   0        0        0       66 2024-05-20 07:07:59.000000 escalona2003-1.1.0/doc/user/overview.rst
+-rw-rw-rw-   0        0        0     2339 2024-05-20 07:07:59.000000 escalona2003-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      353 2024-05-20 07:07:59.000000 escalona2003-1.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       29 2024-05-20 07:07:59.000000 escalona2003-1.1.0/requirements_minimal.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 07:11:59.867468 escalona2003-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 07:11:59.807493 escalona2003-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-20 07:11:59.847381 escalona2003-1.1.0/src/escalona2003/
+-rw-rw-rw-   0        0        0      255 2024-05-20 07:07:59.000000 escalona2003-1.1.0/src/escalona2003/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:11:59.857413 escalona2003-1.1.0/src/escalona2003/clean/
+-rw-rw-rw-   0        0        0     1866 2024-05-20 07:07:22.000000 escalona2003-1.1.0/src/escalona2003/clean/daily_carbon_uptake.csv
+-rw-rw-rw-   0        0        0     2157 2024-05-20 07:07:26.000000 escalona2003-1.1.0/src/escalona2003/clean/rce.csv
+-rw-rw-rw-   0        0        0      134 2024-05-20 07:07:59.000000 escalona2003-1.1.0/src/escalona2003/clean/readme.rst
+-rw-rw-rw-   0        0        0      379 2024-05-20 07:07:59.000000 escalona2003-1.1.0/src/escalona2003/info.py
+-rw-rw-rw-   0        0        0      367 2024-05-20 07:07:59.000000 escalona2003-1.1.0/src/escalona2003/version.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:11:59.862460 escalona2003-1.1.0/src/escalona2003.egg-info/
+-rw-rw-rw-   0        0        0     3371 2024-05-20 07:11:59.000000 escalona2003-1.1.0/src/escalona2003.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      859 2024-05-20 07:11:59.000000 escalona2003-1.1.0/src/escalona2003.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 07:11:59.000000 escalona2003-1.1.0/src/escalona2003.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      174 2024-05-20 07:11:59.000000 escalona2003-1.1.0/src/escalona2003.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-20 07:11:59.000000 escalona2003-1.1.0/src/escalona2003.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-20 07:11:59.862460 escalona2003-1.1.0/test/
+-rw-rw-rw-   0        0        0      988 2024-05-20 07:07:59.000000 escalona2003-1.1.0/test/conftest.py
+-rw-rw-rw-   0        0        0      546 2023-03-09 15:57:37.000000 escalona2003-1.1.0/test/test_daily_carbon_uptake.py
+-rw-rw-rw-   0        0        0      389 2024-05-20 07:07:59.000000 escalona2003-1.1.0/test/test_packaging.py
+-rw-rw-rw-   0        0        0      544 2023-03-09 15:58:02.000000 escalona2003-1.1.0/test/test_rce.py
```

### Comparing `escalona2003-1.0.0/CONTRIBUTING.rst` & `escalona2003-1.1.0/CONTRIBUTING.rst`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 
 Before you submit a pull request, check that it meets these guidelines:
 
   1. The pull request should include tests.
   2. If the pull request adds functionality, the docs should be updated. Put
      your new functionality into a function with a docstring, and add the
      feature to the list in README.rst.
-  3. The pull request should work for Python 310.
+  3. The pull request should work for Python 3.9, 3.12.
      
 
 Tips
 ----
 
 
 To run a subset of tests::
```

### Comparing `escalona2003-1.0.0/LICENSE` & `escalona2003-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `escalona2003-1.0.0/README.rst` & `escalona2003-1.1.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 escalona2003
 ========================
 
 .. {# pkglts, doc
 
 .. image:: https://b326.gitlab.io/escalona2003/_images/badge_pkging_pip.svg
     :alt: PyPI version
-    :target: https://pypi.org/project/escalona2003/1.0.0/
+    :target: https://pypi.org/project/escalona2003/1.1.0/
 
 .. image:: https://b326.gitlab.io/escalona2003/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/escalona2003
 
 .. image:: https://b326.gitlab.io/escalona2003/_images/badge_doc.svg
     :alt: Documentation status
```

### Comparing `escalona2003-1.0.0/doc/Makefile` & `escalona2003-1.1.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `escalona2003-1.0.0/doc/biblio/biblio.rst` & `escalona2003-1.1.0/doc/biblio/biblio.rst`

 * *Files identical despite different names*

### Comparing `escalona2003-1.0.0/doc/conf.py` & `escalona2003-1.1.0/doc/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,17 +85,17 @@
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 
 # The short X.Y version.
-version = "1.0.0"
+version = "1.1.0"
 # The full version, including alpha/beta/rc tags.
-release = "1.0.0"
+release = "1.1.0"
 
 
 exclude_patterns = ['build', 'dist']
 
 pygments_style = 'sphinx'
 
 # -- Options for HTML output -------------------------------------------
```

### Comparing `escalona2003-1.0.0/doc/index.rst` & `escalona2003-1.1.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `escalona2003-1.0.0/doc/make.bat` & `escalona2003-1.1.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `escalona2003-1.0.0/doc/readme.rst` & `escalona2003-1.1.0/doc/readme.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 Overview
 ========
 
 .. {# pkglts, glabpkg_dev
 
 .. image:: https://b326.gitlab.io/escalona2003/_images/badge_pkging_pip.svg
     :alt: PyPI version
-    :target: https://pypi.org/project/escalona2003/1.0.0/
+    :target: https://pypi.org/project/escalona2003/1.1.0/
+
 
 .. image:: https://b326.gitlab.io/escalona2003/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/escalona2003
 
+
 .. image:: https://b326.gitlab.io/escalona2003/_images/badge_doc.svg
     :alt: Documentation status
     :target: https://b326.gitlab.io/escalona2003/
 
+
 .. image:: https://badge.fury.io/py/escalona2003.svg
     :alt: PyPI version
     :target: https://badge.fury.io/py/escalona2003
 
 
 
+
 main: |main_build|_ |main_coverage|_
 
 .. |main_build| image:: https://gitlab.com/b326/escalona2003/badges/main/pipeline.svg
 .. _main_build: https://gitlab.com/b326/escalona2003/commits/main
 
 .. |main_coverage| image:: https://gitlab.com/b326/escalona2003/badges/main/coverage.svg
 .. _main_coverage: https://gitlab.com/b326/escalona2003/commits/main
```

### Comparing `escalona2003-1.0.0/src/escalona2003/clean/daily_carbon_uptake.csv` & `escalona2003-1.1.0/src/escalona2003/clean/daily_carbon_uptake.csv`

 * *Files identical despite different names*

### Comparing `escalona2003-1.0.0/src/escalona2003/clean/rce.csv` & `escalona2003-1.1.0/src/escalona2003/clean/rce.csv`

 * *Files identical despite different names*

### Comparing `escalona2003-1.0.0/src/escalona2003.egg-info/SOURCES.txt` & `escalona2003-1.1.0/src/escalona2003.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 AUTHORS.rst
 CONTRIBUTING.rst
 HISTORY.rst
 LICENSE
-MANIFEST.in
 README.rst
+pyproject.toml
 requirements.txt
 requirements_minimal.txt
-setup.cfg
-setup.py
 doc/Makefile
 doc/authors.rst
 doc/conf.py
 doc/contributing.rst
 doc/history.rst
 doc/index.rst
 doc/installation.rst
@@ -25,15 +23,15 @@
 doc/user/overview.rst
 src/escalona2003/__init__.py
 src/escalona2003/info.py
 src/escalona2003/version.py
 src/escalona2003.egg-info/PKG-INFO
 src/escalona2003.egg-info/SOURCES.txt
 src/escalona2003.egg-info/dependency_links.txt
-src/escalona2003.egg-info/not-zip-safe
+src/escalona2003.egg-info/requires.txt
 src/escalona2003.egg-info/top_level.txt
 src/escalona2003/clean/daily_carbon_uptake.csv
 src/escalona2003/clean/rce.csv
 src/escalona2003/clean/readme.rst
 test/conftest.py
 test/test_daily_carbon_uptake.py
 test/test_packaging.py
```

### Comparing `escalona2003-1.0.0/test/conftest.py` & `escalona2003-1.1.0/test/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 import os
 
 import pytest
 # #}
 
 
 # {# pkglts, test.pytest_cmdline_preparse
-def pytest_cmdline_preparse(args):
-    if 'PYCHARM_HOSTED' not in os.environ:
-        args.append("--cov=escalona2003")
+# def pytest_cmdline_preparse(args):
+#
+#     if 'PYCHARM_HOSTED' not in os.environ:
+#         args.append("--cov=escalona2003")
+#
 # #}
 
 
 # {# pkglts, test.pytest_addoption
 def pytest_addoption(parser):
     parser.addoption("--runslow", action="store_true",
                      default=False, help="run slow tests")
```

### Comparing `escalona2003-1.0.0/test/test_daily_carbon_uptake.py` & `escalona2003-1.1.0/test/test_daily_carbon_uptake.py`

 * *Files identical despite different names*

### Comparing `escalona2003-1.0.0/test/test_rce.py` & `escalona2003-1.1.0/test/test_rce.py`

 * *Files identical despite different names*

