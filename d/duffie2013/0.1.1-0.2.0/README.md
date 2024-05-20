# Comparing `tmp/duffie2013-0.1.1.tar.gz` & `tmp/duffie2013-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duffie2013-0.1.1.tar", last modified: Wed Jul  7 16:00:04 2021, max compression
+gzip compressed data, was "duffie2013-0.2.0.tar", last modified: Mon May 20 07:09:50 2024, max compression
```

## Comparing `duffie2013-0.1.1.tar` & `duffie2013-0.2.0.tar`

### file list

```diff
@@ -1,52 +1,51 @@
-drwxrwxrwx   0        0        0        0 2021-07-07 16:00:04.411375 duffie2013-0.1.1/
--rw-rw-rw-   0        0        0      316 2021-07-07 15:55:59.000000 duffie2013-0.1.1/AUTHORS.rst
--rw-rw-rw-   0        0        0     3332 2021-07-07 15:55:59.000000 duffie2013-0.1.1/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0      106 2021-07-07 15:55:59.000000 duffie2013-0.1.1/HISTORY.rst
--rw-rw-rw-   0        0        0    20838 2021-07-07 15:55:59.000000 duffie2013-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      438 2021-07-07 15:55:59.000000 duffie2013-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3016 2021-07-07 16:00:04.412368 duffie2013-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1668 2021-07-07 15:55:59.000000 duffie2013-0.1.1/README.rst
-drwxrwxrwx   0        0        0        0 2021-07-07 16:00:04.346391 duffie2013-0.1.1/doc/
--rw-rw-rw-   0        0        0     6967 2021-07-07 15:55:59.000000 duffie2013-0.1.1/doc/Makefile
--rw-rw-rw-   0        0        0       29 2021-07-07 15:55:59.000000 duffie2013-0.1.1/doc/authors.rst
-drwxrwxrwx   0        0        0        0 2021-07-07 16:00:04.349362 duffie2013-0.1.1/doc/badges/
--rw-rw-rw-   0        0        0      227 2021-07-07 15:55:59.000000 duffie2013-0.1.1/doc/badges/listing.rst
-drwxrwxrwx   0        0        0        0 2021-07-07 16:00:04.351363 duffie2013-0.1.1/doc/biblio/
--rw-rw-rw-   0        0        0      640 2021-07-07 15:55:59.000000 duffie2013-0.1.1/doc/biblio/biblio.rst
--rw-rw-rw-   0        0        0     5123 2021-07-07 15:55:59.000000 duffie2013-0.1.1/doc/conf.py
--rw-rw-rw-   0        0        0       34 2021-07-07 15:55:59.000000 duffie2013-0.1.1/doc/contributing.rst
--rw-rw-rw-   0        0        0       29 2021-07-07 15:55:59.000000 duffie2013-0.1.1/doc/history.rst
--rw-rw-rw-   0        0        0      512 2021-07-07 15:55:59.000000 duffie2013-0.1.1/doc/index.rst
--rw-rw-rw-   0        0        0      165 2021-07-07 15:55:59.000000 duffie2013-0.1.1/doc/installation.rst
--rwxrwxrwx   0        0        0     6731 2021-07-07 15:55:59.000000 duffie2013-0.1.1/doc/make.bat
--rw-rw-rw-   0        0        0      128 2021-07-07 15:55:59.000000 duffie2013-0.1.1/doc/management.rst
--rw-rw-rw-   0        0        0     1587 2021-07-07 15:55:59.000000 duffie2013-0.1.1/doc/readme.rst
--rw-rw-rw-   0        0        0       21 2021-07-07 15:55:59.000000 duffie2013-0.1.1/doc/usage.rst
-drwxrwxrwx   0        0        0        0 2021-07-07 16:00:04.356366 duffie2013-0.1.1/doc/user/
--rw-rw-rw-   0        0        0       83 2021-07-07 15:55:59.000000 duffie2013-0.1.1/doc/user/index.rst
--rw-rw-rw-   0        0        0       66 2021-07-07 15:55:59.000000 duffie2013-0.1.1/doc/user/overview.rst
--rw-rw-rw-   0        0        0      318 2021-07-07 15:55:59.000000 duffie2013-0.1.1/requirements.txt
--rw-rw-rw-   0        0        0       29 2021-07-07 15:55:59.000000 duffie2013-0.1.1/requirements_minimal.txt
--rw-rw-rw-   0        0        0      187 2021-07-07 16:00:04.416363 duffie2013-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1998 2021-07-07 15:55:59.000000 duffie2013-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2021-07-07 16:00:04.266369 duffie2013-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2021-07-07 16:00:04.375371 duffie2013-0.1.1/src/duffie2013/
--rw-rw-rw-   0        0        0      209 2021-07-07 15:55:59.000000 duffie2013-0.1.1/src/duffie2013/__init__.py
--rw-rw-rw-   0        0        0     2353 2021-07-07 13:12:42.000000 duffie2013-0.1.1/src/duffie2013/clear_sky.py
--rw-rw-rw-   0        0        0      721 2021-07-07 13:12:42.000000 duffie2013-0.1.1/src/duffie2013/diffuse.py
--rw-rw-rw-   0        0        0     4885 2021-07-07 15:22:00.000000 duffie2013-0.1.1/src/duffie2013/extraterrestrial.py
--rw-rw-rw-   0        0        0     4230 2021-07-06 17:48:26.000000 duffie2013-0.1.1/src/duffie2013/sun.py
--rw-rw-rw-   0        0        0      367 2021-07-07 15:55:59.000000 duffie2013-0.1.1/src/duffie2013/version.py
-drwxrwxrwx   0        0        0        0 2021-07-07 16:00:04.391361 duffie2013-0.1.1/src/duffie2013.egg-info/
--rw-rw-rw-   0        0        0     3016 2021-07-07 16:00:03.000000 duffie2013-0.1.1/src/duffie2013.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      876 2021-07-07 16:00:04.000000 duffie2013-0.1.1/src/duffie2013.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-07-07 16:00:03.000000 duffie2013-0.1.1/src/duffie2013.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-07-06 14:24:47.000000 duffie2013-0.1.1/src/duffie2013.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2021-07-07 16:00:03.000000 duffie2013-0.1.1/src/duffie2013.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2021-07-07 16:00:04.408361 duffie2013-0.1.1/test/
--rw-rw-rw-   0        0        0      974 2021-07-07 15:55:59.000000 duffie2013-0.1.1/test/conftest.py
--rw-rw-rw-   0        0        0     1755 2021-07-07 13:12:42.000000 duffie2013-0.1.1/test/test_clear_sky.py
--rw-rw-rw-   0        0        0      240 2021-07-07 13:12:42.000000 duffie2013-0.1.1/test/test_diffuse.py
--rw-rw-rw-   0        0        0     2739 2021-07-07 15:22:00.000000 duffie2013-0.1.1/test/test_extraterrestrial.py
--rw-rw-rw-   0        0        0       86 2021-07-07 15:55:59.000000 duffie2013-0.1.1/test/test_packaging.py
--rw-rw-rw-   0        0        0     1911 2021-07-06 17:48:26.000000 duffie2013-0.1.1/test/test_sun.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:09:50.015964 duffie2013-0.2.0/
+-rw-rw-rw-   0        0        0      316 2024-05-20 06:58:25.000000 duffie2013-0.2.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3333 2024-05-20 06:58:25.000000 duffie2013-0.2.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0      106 2024-05-20 06:58:25.000000 duffie2013-0.2.0/HISTORY.rst
+-rw-rw-rw-   0        0        0    20838 2024-05-20 06:58:25.000000 duffie2013-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     3003 2024-05-20 07:09:50.015964 duffie2013-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1163 2024-05-20 06:58:25.000000 duffie2013-0.2.0/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-20 07:09:49.972813 duffie2013-0.2.0/doc/
+-rw-rw-rw-   0        0        0     6967 2024-05-20 06:58:25.000000 duffie2013-0.2.0/doc/Makefile
+-rw-rw-rw-   0        0        0       29 2024-05-20 06:58:25.000000 duffie2013-0.2.0/doc/authors.rst
+drwxrwxrwx   0        0        0        0 2024-05-20 07:09:49.981533 duffie2013-0.2.0/doc/badges/
+-rw-rw-rw-   0        0        0      282 2024-05-20 06:58:25.000000 duffie2013-0.2.0/doc/badges/listing.rst
+drwxrwxrwx   0        0        0        0 2024-05-20 07:09:49.983534 duffie2013-0.2.0/doc/biblio/
+-rw-rw-rw-   0        0        0      513 2024-05-20 06:58:25.000000 duffie2013-0.2.0/doc/biblio/biblio.rst
+-rw-rw-rw-   0        0        0     5123 2024-05-20 06:58:25.000000 duffie2013-0.2.0/doc/conf.py
+-rw-rw-rw-   0        0        0       34 2024-05-20 06:58:25.000000 duffie2013-0.2.0/doc/contributing.rst
+-rw-rw-rw-   0        0        0       29 2024-05-20 06:58:25.000000 duffie2013-0.2.0/doc/history.rst
+-rw-rw-rw-   0        0        0      595 2024-05-20 06:58:25.000000 duffie2013-0.2.0/doc/index.rst
+-rw-rw-rw-   0        0        0      220 2024-05-20 06:58:25.000000 duffie2013-0.2.0/doc/installation.rst
+-rwxrwxrwx   0        0        0     6731 2024-05-20 06:58:25.000000 duffie2013-0.2.0/doc/make.bat
+-rw-rw-rw-   0        0        0      133 2024-05-20 06:58:25.000000 duffie2013-0.2.0/doc/management.rst
+-rw-rw-rw-   0        0        0     1090 2024-05-20 06:58:25.000000 duffie2013-0.2.0/doc/readme.rst
+-rw-rw-rw-   0        0        0       21 2024-05-20 06:58:25.000000 duffie2013-0.2.0/doc/usage.rst
+drwxrwxrwx   0        0        0        0 2024-05-20 07:09:49.983534 duffie2013-0.2.0/doc/user/
+-rw-rw-rw-   0        0        0       86 2024-05-20 06:58:25.000000 duffie2013-0.2.0/doc/user/index.rst
+-rw-rw-rw-   0        0        0       66 2024-05-20 06:58:25.000000 duffie2013-0.2.0/doc/user/overview.rst
+-rw-rw-rw-   0        0        0     2384 2024-05-20 06:58:25.000000 duffie2013-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0      318 2024-05-20 06:58:25.000000 duffie2013-0.2.0/requirements.txt
+-rw-rw-rw-   0        0        0       29 2024-05-20 06:58:25.000000 duffie2013-0.2.0/requirements_minimal.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 07:09:50.015964 duffie2013-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 07:09:49.934465 duffie2013-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-20 07:09:49.992925 duffie2013-0.2.0/src/duffie2013/
+-rw-rw-rw-   0        0        0      209 2024-05-20 06:58:25.000000 duffie2013-0.2.0/src/duffie2013/__init__.py
+-rw-rw-rw-   0        0        0     2353 2021-07-08 15:32:41.000000 duffie2013-0.2.0/src/duffie2013/clear_sky.py
+-rw-rw-rw-   0        0        0      721 2021-07-07 13:12:42.000000 duffie2013-0.2.0/src/duffie2013/diffuse.py
+-rw-rw-rw-   0        0        0     4885 2021-07-07 15:22:00.000000 duffie2013-0.2.0/src/duffie2013/extraterrestrial.py
+-rw-rw-rw-   0        0        0     4230 2021-07-06 17:48:26.000000 duffie2013-0.2.0/src/duffie2013/sun.py
+-rw-rw-rw-   0        0        0      367 2024-05-20 06:58:25.000000 duffie2013-0.2.0/src/duffie2013/version.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:09:50.014925 duffie2013-0.2.0/src/duffie2013.egg-info/
+-rw-rw-rw-   0        0        0     3003 2024-05-20 07:09:49.000000 duffie2013-0.2.0/src/duffie2013.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      860 2024-05-20 07:09:49.000000 duffie2013-0.2.0/src/duffie2013.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 07:09:49.000000 duffie2013-0.2.0/src/duffie2013.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      143 2024-05-20 07:09:49.000000 duffie2013-0.2.0/src/duffie2013.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-20 07:09:49.000000 duffie2013-0.2.0/src/duffie2013.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-20 07:09:50.003263 duffie2013-0.2.0/test/
+-rw-rw-rw-   0        0        0      986 2024-05-20 06:58:25.000000 duffie2013-0.2.0/test/conftest.py
+-rw-rw-rw-   0        0        0     1755 2021-07-07 13:12:42.000000 duffie2013-0.2.0/test/test_clear_sky.py
+-rw-rw-rw-   0        0        0      240 2021-07-07 13:12:42.000000 duffie2013-0.2.0/test/test_diffuse.py
+-rw-rw-rw-   0        0        0     2739 2021-07-07 15:22:00.000000 duffie2013-0.2.0/test/test_extraterrestrial.py
+-rw-rw-rw-   0        0        0      120 2024-05-20 06:58:25.000000 duffie2013-0.2.0/test/test_packaging.py
+-rw-rw-rw-   0        0        0     1911 2021-07-06 17:48:26.000000 duffie2013-0.2.0/test/test_sun.py
```

### Comparing `duffie2013-0.1.1/CONTRIBUTING.rst` & `duffie2013-0.2.0/CONTRIBUTING.rst`

 * *Files 2% similar despite different names*

```diff
@@ -102,24 +102,24 @@
 
 Before you submit a pull request, check that it meets these guidelines:
 
   1. The pull request should include tests.
   2. If the pull request adds functionality, the docs should be updated. Put
      your new functionality into a function with a docstring, and add the
      feature to the list in README.rst.
-  3. The pull request should work for Python 39.
+  3. The pull request should work for Python 3.7, 3.8, 3.9.
      
 
 Tips
 ----
 
 
 To run a subset of tests::
 
     $ pytest test/test_XXX
 
 
 
 
-.. _issues: https://gitlab.com/revesansparole/duffie2013/issues
+.. _issues: https://gitlab.com/b326/duffie2013/issues
 
 .. _virtualenv: https://pypi.python.org/pypi/virtualenv
```

### Comparing `duffie2013-0.1.1/LICENSE` & `duffie2013-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `duffie2013-0.1.1/doc/Makefile` & `duffie2013-0.2.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `duffie2013-0.1.1/doc/biblio/biblio.rst` & `duffie2013-0.2.0/doc/biblio/biblio.rst`

 * *Files 20% similar despite different names*

```diff
@@ -10,9 +10,7 @@
         .. include:: ../biblio/biblio.rst
         """
         def myfunc():
         """does something
         Reference:
         - `Allen et al. (1998)`_
         """
-
-.. _`Duffie et al. (2013)`: https://www.wiley.com/en-us/Solar+Engineering+of+Thermal+Processes%2C+4th+Edition-p-9780470873663
```

### Comparing `duffie2013-0.1.1/doc/conf.py` & `duffie2013-0.2.0/doc/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,17 +85,17 @@
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 
 # The short X.Y version.
-version = "0.1.1"
+version = "0.2.0"
 # The full version, including alpha/beta/rc tags.
-release = "0.1.1"
+release = "0.2.0"
 
 
 exclude_patterns = ['build', 'dist']
 
 pygments_style = 'sphinx'
 
 # -- Options for HTML output -------------------------------------------
```

### Comparing `duffie2013-0.1.1/doc/index.rst` & `duffie2013-0.2.0/doc/index.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Welcome to duffie2013's documentation!
 ====================================================
 
 .. toctree::
-   :caption: Contents
-   :maxdepth: 2
+    :caption: Contents
+    :maxdepth: 2
 
-   readme
-   installation
-   usage
-   management
+    readme
+    installation
+    usage
 
 .. toctree::
-   :caption: User's documentation
-   :maxdepth: 2
+    :caption: User's documentation
+    :maxdepth: 2
 
-   user/index
-   _gallery/index
+    user/index
+    _gallery/index
 
 .. toctree::
-   :caption: Developer's documentation
-   :maxdepth: 4
+    :caption: Developer's documentation
+    :maxdepth: 4
 
-   Sources <_dvlpt/modules>
+    Sources <_dvlpt/modules>
 
-Indices and tables
-==================
+.. toctree::
+    :caption: Annexe
+    :maxdepth: 2
+
+    gitlab home <https://gitlab.com/b326/duffie2013>
+    management
 
 * :ref:`genindex`
 * :ref:`modindex`
 * :ref:`search`
```

### Comparing `duffie2013-0.1.1/doc/make.bat` & `duffie2013-0.2.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `duffie2013-0.1.1/src/duffie2013/clear_sky.py` & `duffie2013-0.2.0/src/duffie2013/clear_sky.py`

 * *Files identical despite different names*

### Comparing `duffie2013-0.1.1/src/duffie2013/diffuse.py` & `duffie2013-0.2.0/src/duffie2013/diffuse.py`

 * *Files identical despite different names*

### Comparing `duffie2013-0.1.1/src/duffie2013/extraterrestrial.py` & `duffie2013-0.2.0/src/duffie2013/extraterrestrial.py`

 * *Files identical despite different names*

### Comparing `duffie2013-0.1.1/src/duffie2013/sun.py` & `duffie2013-0.2.0/src/duffie2013/sun.py`

 * *Files identical despite different names*

### Comparing `duffie2013-0.1.1/src/duffie2013.egg-info/SOURCES.txt` & `duffie2013-0.2.0/src/duffie2013.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

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
@@ -28,15 +26,15 @@
 src/duffie2013/diffuse.py
 src/duffie2013/extraterrestrial.py
 src/duffie2013/sun.py
 src/duffie2013/version.py
 src/duffie2013.egg-info/PKG-INFO
 src/duffie2013.egg-info/SOURCES.txt
 src/duffie2013.egg-info/dependency_links.txt
-src/duffie2013.egg-info/not-zip-safe
+src/duffie2013.egg-info/requires.txt
 src/duffie2013.egg-info/top_level.txt
 test/conftest.py
 test/test_clear_sky.py
 test/test_diffuse.py
 test/test_extraterrestrial.py
 test/test_packaging.py
 test/test_sun.py
```

### Comparing `duffie2013-0.1.1/test/conftest.py` & `duffie2013-0.2.0/test/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 import os
 
 import pytest
 # #}
 
 
 # {# pkglts, test.pytest_cmdline_preparse
-def pytest_cmdline_preparse(args):
-    if 'PYCHARM_HOSTED' not in os.environ:
-        args.append("--cov=duffie2013")
+# def pytest_cmdline_preparse(args):
+#
+#     if 'PYCHARM_HOSTED' not in os.environ:
+#         args.append("--cov=duffie2013")
+#
 # #}
 
 
 # {# pkglts, test.pytest_addoption
 def pytest_addoption(parser):
     parser.addoption("--runslow", action="store_true",
                      default=False, help="run slow tests")
```

### Comparing `duffie2013-0.1.1/test/test_clear_sky.py` & `duffie2013-0.2.0/test/test_clear_sky.py`

 * *Files identical despite different names*

### Comparing `duffie2013-0.1.1/test/test_extraterrestrial.py` & `duffie2013-0.2.0/test/test_extraterrestrial.py`

 * *Files identical despite different names*

### Comparing `duffie2013-0.1.1/test/test_sun.py` & `duffie2013-0.2.0/test/test_sun.py`

 * *Files identical despite different names*

