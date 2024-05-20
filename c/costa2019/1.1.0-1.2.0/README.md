# Comparing `tmp/costa2019-1.1.0.tar.gz` & `tmp/costa2019-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "costa2019-1.1.0.tar", last modified: Mon Jul 18 15:29:34 2022, max compression
+gzip compressed data, was "costa2019-1.2.0.tar", last modified: Mon May 20 06:51:15 2024, max compression
```

## Comparing `costa2019-1.1.0.tar` & `costa2019-1.2.0.tar`

### file list

```diff
@@ -1,52 +1,51 @@
-drwxrwxrwx   0        0        0        0 2022-07-18 15:29:34.416942 costa2019-1.1.0/
--rw-rw-rw-   0        0        0      316 2022-07-18 15:15:24.000000 costa2019-1.1.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3312 2022-07-18 15:15:24.000000 costa2019-1.1.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0      106 2022-07-18 15:15:24.000000 costa2019-1.1.0/HISTORY.rst
--rw-rw-rw-   0        0        0    20838 2022-07-18 15:15:24.000000 costa2019-1.1.0/LICENSE
--rw-rw-rw-   0        0        0      437 2022-07-18 15:15:24.000000 costa2019-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2305 2022-07-18 15:29:34.416942 costa2019-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1481 2022-07-18 15:15:24.000000 costa2019-1.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2022-07-18 15:29:34.344936 costa2019-1.1.0/doc/
--rw-rw-rw-   0        0        0     6967 2022-07-18 15:15:24.000000 costa2019-1.1.0/doc/Makefile
--rw-rw-rw-   0        0        0       29 2022-07-18 15:15:25.000000 costa2019-1.1.0/doc/authors.rst
-drwxrwxrwx   0        0        0        0 2022-07-18 15:29:34.348924 costa2019-1.1.0/doc/badges/
--rw-rw-rw-   0        0        0      227 2022-07-18 15:15:25.000000 costa2019-1.1.0/doc/badges/listing.rst
-drwxrwxrwx   0        0        0        0 2022-07-18 15:29:34.350924 costa2019-1.1.0/doc/biblio/
--rw-rw-rw-   0        0        0      513 2022-07-18 15:15:25.000000 costa2019-1.1.0/doc/biblio/biblio.rst
--rw-rw-rw-   0        0        0     5102 2022-07-18 15:15:24.000000 costa2019-1.1.0/doc/conf.py
--rw-rw-rw-   0        0        0       34 2022-07-18 15:15:25.000000 costa2019-1.1.0/doc/contributing.rst
--rw-rw-rw-   0        0        0       29 2022-07-18 15:15:25.000000 costa2019-1.1.0/doc/history.rst
--rw-rw-rw-   0        0        0      593 2022-07-18 15:15:25.000000 costa2019-1.1.0/doc/index.rst
--rw-rw-rw-   0        0        0      164 2022-07-18 15:15:25.000000 costa2019-1.1.0/doc/installation.rst
--rwxrwxrwx   0        0        0     6731 2022-07-18 15:15:24.000000 costa2019-1.1.0/doc/make.bat
--rw-rw-rw-   0        0        0      133 2022-07-18 15:15:25.000000 costa2019-1.1.0/doc/management.rst
--rw-rw-rw-   0        0        0     1401 2022-07-18 15:15:25.000000 costa2019-1.1.0/doc/readme.rst
--rw-rw-rw-   0        0        0       21 2022-07-18 15:15:25.000000 costa2019-1.1.0/doc/usage.rst
-drwxrwxrwx   0        0        0        0 2022-07-18 15:29:34.356924 costa2019-1.1.0/doc/user/
--rw-rw-rw-   0        0        0       86 2022-07-18 15:15:25.000000 costa2019-1.1.0/doc/user/index.rst
--rw-rw-rw-   0        0        0       66 2022-07-18 15:15:25.000000 costa2019-1.1.0/doc/user/overview.rst
--rw-rw-rw-   0        0        0      360 2022-07-18 15:15:24.000000 costa2019-1.1.0/requirements.txt
--rw-rw-rw-   0        0        0       29 2022-07-18 15:15:24.000000 costa2019-1.1.0/requirements_minimal.txt
--rw-rw-rw-   0        0        0      187 2022-07-18 15:29:34.419924 costa2019-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1892 2022-07-18 15:15:25.000000 costa2019-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-07-18 15:29:34.281928 costa2019-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2022-07-18 15:29:34.364924 costa2019-1.1.0/src/costa2019/
--rw-rw-rw-   0        0        0      271 2022-07-18 15:15:24.000000 costa2019-1.1.0/src/costa2019/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-18 15:29:34.407923 costa2019-1.1.0/src/costa2019/clean/
--rw-rw-rw-   0        0        0     7169 2022-07-18 13:29:26.000000 costa2019-1.1.0/src/costa2019/clean/fig1.csv
--rw-rw-rw-   0        0        0      904 2022-07-18 13:29:29.000000 costa2019-1.1.0/src/costa2019/clean/fig5.csv
--rw-rw-rw-   0        0        0      442 2022-07-18 13:29:33.000000 costa2019-1.1.0/src/costa2019/clean/info.json
--rw-rw-rw-   0        0        0      134 2022-07-18 15:15:25.000000 costa2019-1.1.0/src/costa2019/clean/readme.rst
--rw-rw-rw-   0        0        0     1802 2022-07-18 13:58:19.000000 costa2019-1.1.0/src/costa2019/clean/tab4.csv
--rw-rw-rw-   0        0        0      152 2022-07-18 15:15:25.000000 costa2019-1.1.0/src/costa2019/info.py
--rw-rw-rw-   0        0        0      367 2022-07-18 15:15:24.000000 costa2019-1.1.0/src/costa2019/version.py
-drwxrwxrwx   0        0        0        0 2022-07-18 15:29:34.393926 costa2019-1.1.0/src/costa2019.egg-info/
--rw-rw-rw-   0        0        0     2305 2022-07-18 15:29:33.000000 costa2019-1.1.0/src/costa2019.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      855 2022-07-18 15:29:33.000000 costa2019-1.1.0/src/costa2019.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-18 15:29:33.000000 costa2019-1.1.0/src/costa2019.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-08-02 07:39:16.000000 costa2019-1.1.0/src/costa2019.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2022-07-18 15:29:33.000000 costa2019-1.1.0/src/costa2019.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-07-18 15:29:34.414925 costa2019-1.1.0/test/
--rw-rw-rw-   0        0        0      973 2022-07-18 15:15:25.000000 costa2019-1.1.0/test/conftest.py
--rw-rw-rw-   0        0        0       84 2022-07-18 15:15:25.000000 costa2019-1.1.0/test/test_packaging.py
--rw-rw-rw-   0        0        0      286 2022-07-18 14:01:47.000000 costa2019-1.1.0/test/test_tab4.py
+drwxrwxrwx   0        0        0        0 2024-05-20 06:51:15.659579 costa2019-1.2.0/
+-rw-rw-rw-   0        0        0      316 2024-05-20 06:46:44.000000 costa2019-1.2.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3313 2024-05-20 06:46:44.000000 costa2019-1.2.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0      106 2024-05-20 06:46:44.000000 costa2019-1.2.0/HISTORY.rst
+-rw-rw-rw-   0        0        0    20838 2024-05-20 06:46:44.000000 costa2019-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     3307 2024-05-20 06:51:15.657559 costa2019-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1485 2024-05-20 06:46:44.000000 costa2019-1.2.0/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-20 06:51:15.631900 costa2019-1.2.0/doc/
+-rw-rw-rw-   0        0        0     6967 2024-05-20 06:46:44.000000 costa2019-1.2.0/doc/Makefile
+-rw-rw-rw-   0        0        0       29 2024-05-20 06:46:44.000000 costa2019-1.2.0/doc/authors.rst
+drwxrwxrwx   0        0        0        0 2024-05-20 06:51:15.634282 costa2019-1.2.0/doc/badges/
+-rw-rw-rw-   0        0        0      282 2024-05-20 06:46:44.000000 costa2019-1.2.0/doc/badges/listing.rst
+drwxrwxrwx   0        0        0        0 2024-05-20 06:51:15.634971 costa2019-1.2.0/doc/biblio/
+-rw-rw-rw-   0        0        0      513 2024-05-20 06:46:44.000000 costa2019-1.2.0/doc/biblio/biblio.rst
+-rw-rw-rw-   0        0        0     5102 2024-05-20 06:46:44.000000 costa2019-1.2.0/doc/conf.py
+-rw-rw-rw-   0        0        0       34 2024-05-20 06:46:44.000000 costa2019-1.2.0/doc/contributing.rst
+-rw-rw-rw-   0        0        0       29 2024-05-20 06:46:44.000000 costa2019-1.2.0/doc/history.rst
+-rw-rw-rw-   0        0        0      593 2024-05-20 06:46:44.000000 costa2019-1.2.0/doc/index.rst
+-rw-rw-rw-   0        0        0      219 2024-05-20 06:46:44.000000 costa2019-1.2.0/doc/installation.rst
+-rwxrwxrwx   0        0        0     6731 2024-05-20 06:46:44.000000 costa2019-1.2.0/doc/make.bat
+-rw-rw-rw-   0        0        0      133 2024-05-20 06:46:44.000000 costa2019-1.2.0/doc/management.rst
+-rw-rw-rw-   0        0        0     1413 2024-05-20 06:46:44.000000 costa2019-1.2.0/doc/readme.rst
+-rw-rw-rw-   0        0        0       21 2024-05-20 06:46:44.000000 costa2019-1.2.0/doc/usage.rst
+drwxrwxrwx   0        0        0        0 2024-05-20 06:51:15.637416 costa2019-1.2.0/doc/user/
+-rw-rw-rw-   0        0        0       86 2024-05-20 06:46:44.000000 costa2019-1.2.0/doc/user/index.rst
+-rw-rw-rw-   0        0        0       66 2024-05-20 06:46:44.000000 costa2019-1.2.0/doc/user/overview.rst
+-rw-rw-rw-   0        0        0     2293 2024-05-20 06:46:44.000000 costa2019-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0      360 2024-05-20 06:46:44.000000 costa2019-1.2.0/requirements.txt
+-rw-rw-rw-   0        0        0       29 2024-05-20 06:46:44.000000 costa2019-1.2.0/requirements_minimal.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 06:51:15.659579 costa2019-1.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 06:51:15.598520 costa2019-1.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-20 06:51:15.640902 costa2019-1.2.0/src/costa2019/
+-rw-rw-rw-   0        0        0      263 2024-05-20 06:46:44.000000 costa2019-1.2.0/src/costa2019/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 06:51:15.653560 costa2019-1.2.0/src/costa2019/clean/
+-rw-rw-rw-   0        0        0     7169 2024-05-20 06:42:38.000000 costa2019-1.2.0/src/costa2019/clean/fig1.csv
+-rw-rw-rw-   0        0        0      904 2024-05-20 06:43:34.000000 costa2019-1.2.0/src/costa2019/clean/fig5.csv
+-rw-rw-rw-   0        0        0      442 2024-05-20 06:45:16.000000 costa2019-1.2.0/src/costa2019/clean/info.json
+-rw-rw-rw-   0        0        0      134 2024-05-20 06:46:44.000000 costa2019-1.2.0/src/costa2019/clean/readme.rst
+-rw-rw-rw-   0        0        0     1802 2024-05-20 06:45:08.000000 costa2019-1.2.0/src/costa2019/clean/tab4.csv
+-rw-rw-rw-   0        0        0      379 2024-05-20 06:46:44.000000 costa2019-1.2.0/src/costa2019/info.py
+-rw-rw-rw-   0        0        0      367 2024-05-20 06:46:44.000000 costa2019-1.2.0/src/costa2019/version.py
+drwxrwxrwx   0        0        0        0 2024-05-20 06:51:15.657559 costa2019-1.2.0/src/costa2019.egg-info/
+-rw-rw-rw-   0        0        0     3307 2024-05-20 06:51:15.000000 costa2019-1.2.0/src/costa2019.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      839 2024-05-20 06:51:15.000000 costa2019-1.2.0/src/costa2019.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 06:51:15.000000 costa2019-1.2.0/src/costa2019.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      180 2024-05-20 06:51:15.000000 costa2019-1.2.0/src/costa2019.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-20 06:51:15.000000 costa2019-1.2.0/src/costa2019.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-20 06:51:15.655560 costa2019-1.2.0/test/
+-rw-rw-rw-   0        0        0      985 2024-05-20 06:46:44.000000 costa2019-1.2.0/test/conftest.py
+-rw-rw-rw-   0        0        0      377 2024-05-20 06:46:44.000000 costa2019-1.2.0/test/test_packaging.py
+-rw-rw-rw-   0        0        0      286 2022-07-18 14:01:47.000000 costa2019-1.2.0/test/test_tab4.py
```

### Comparing `costa2019-1.1.0/CONTRIBUTING.rst` & `costa2019-1.2.0/CONTRIBUTING.rst`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 
 Before you submit a pull request, check that it meets these guidelines:
 
   1. The pull request should include tests.
   2. If the pull request adds functionality, the docs should be updated. Put
      your new functionality into a function with a docstring, and add the
      feature to the list in README.rst.
-  3. The pull request should work for Python 39.
+  3. The pull request should work for Python 3.9.
      
 
 Tips
 ----
 
 
 To run a subset of tests::
```

### Comparing `costa2019-1.1.0/LICENSE` & `costa2019-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `costa2019-1.1.0/README.rst` & `costa2019-1.2.0/doc/readme.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,33 @@
-========================
-costa2019
-========================
+Overview
+========
 
-.. {# pkglts, doc
-
-.. image:: https://b326.gitlab.io/costa2019/_images/badge_doc.svg
-    :alt: Documentation status
-    :target: https://b326.gitlab.io/costa2019/
+.. {# pkglts, glabpkg_dev
 
 .. image:: https://b326.gitlab.io/costa2019/_images/badge_pkging_pip.svg
     :alt: PyPI version
-    :target: https://pypi.org/project/costa2019/1.1.0/
+    :target: https://pypi.org/project/costa2019/1.2.0/
+
 
 .. image:: https://b326.gitlab.io/costa2019/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/costa2019
 
+
+.. image:: https://b326.gitlab.io/costa2019/_images/badge_doc.svg
+    :alt: Documentation status
+    :target: https://b326.gitlab.io/costa2019/
+
+
 .. image:: https://badge.fury.io/py/costa2019.svg
     :alt: PyPI version
     :target: https://badge.fury.io/py/costa2019
 
-.. #}
-.. {# pkglts, glabpkg, after doc
+
+
 
 main: |main_build|_ |main_coverage|_
 
 .. |main_build| image:: https://gitlab.com/b326/costa2019/badges/main/pipeline.svg
 .. _main_build: https://gitlab.com/b326/costa2019/commits/main
 
 .. |main_coverage| image:: https://gitlab.com/b326/costa2019/badges/main/coverage.svg
@@ -37,8 +39,7 @@
 .. _prod_build: https://gitlab.com/b326/costa2019/commits/prod
 
 .. |prod_coverage| image:: https://gitlab.com/b326/costa2019/badges/prod/coverage.svg
 .. _prod_coverage: https://gitlab.com/b326/costa2019/commits/prod
 .. #}
 
 Data from canopy and soil thermal patterns in vineyards
-
```

### Comparing `costa2019-1.1.0/doc/Makefile` & `costa2019-1.2.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `costa2019-1.1.0/doc/biblio/biblio.rst` & `costa2019-1.2.0/doc/biblio/biblio.rst`

 * *Files identical despite different names*

### Comparing `costa2019-1.1.0/doc/conf.py` & `costa2019-1.2.0/doc/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,17 +85,17 @@
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 
 # The short X.Y version.
-version = "1.1.0"
+version = "1.2.0"
 # The full version, including alpha/beta/rc tags.
-release = "1.1.0"
+release = "1.2.0"
 
 
 exclude_patterns = ['build', 'dist']
 
 pygments_style = 'sphinx'
 
 # -- Options for HTML output -------------------------------------------
```

### Comparing `costa2019-1.1.0/doc/index.rst` & `costa2019-1.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `costa2019-1.1.0/doc/make.bat` & `costa2019-1.2.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `costa2019-1.1.0/doc/readme.rst` & `costa2019-1.2.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-Overview
-========
+========================
+costa2019
+========================
 
-.. {# pkglts, glabpkg
-
-.. image:: https://b326.gitlab.io/costa2019/_images/badge_doc.svg
-    :alt: Documentation status
-    :target: https://b326.gitlab.io/costa2019/
+.. {# pkglts, doc
 
 .. image:: https://b326.gitlab.io/costa2019/_images/badge_pkging_pip.svg
     :alt: PyPI version
-    :target: https://pypi.org/project/costa2019/1.1.0/
+    :target: https://pypi.org/project/costa2019/1.2.0/
 
 .. image:: https://b326.gitlab.io/costa2019/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/costa2019
 
+.. image:: https://b326.gitlab.io/costa2019/_images/badge_doc.svg
+    :alt: Documentation status
+    :target: https://b326.gitlab.io/costa2019/
+
 .. image:: https://badge.fury.io/py/costa2019.svg
     :alt: PyPI version
     :target: https://badge.fury.io/py/costa2019
 
-
+.. #}
+.. {# pkglts, glabpkg_dev, after doc
 
 main: |main_build|_ |main_coverage|_
 
 .. |main_build| image:: https://gitlab.com/b326/costa2019/badges/main/pipeline.svg
 .. _main_build: https://gitlab.com/b326/costa2019/commits/main
 
 .. |main_coverage| image:: https://gitlab.com/b326/costa2019/badges/main/coverage.svg
@@ -35,7 +37,8 @@
 .. _prod_build: https://gitlab.com/b326/costa2019/commits/prod
 
 .. |prod_coverage| image:: https://gitlab.com/b326/costa2019/badges/prod/coverage.svg
 .. _prod_coverage: https://gitlab.com/b326/costa2019/commits/prod
 .. #}
 
 Data from canopy and soil thermal patterns in vineyards
+
```

### Comparing `costa2019-1.1.0/src/costa2019/clean/fig1.csv` & `costa2019-1.2.0/src/costa2019/clean/fig1.csv`

 * *Files identical despite different names*

### Comparing `costa2019-1.1.0/src/costa2019/clean/fig5.csv` & `costa2019-1.2.0/src/costa2019/clean/fig5.csv`

 * *Files identical despite different names*

### Comparing `costa2019-1.1.0/src/costa2019/clean/tab4.csv` & `costa2019-1.2.0/src/costa2019/clean/tab4.csv`

 * *Files identical despite different names*

### Comparing `costa2019-1.1.0/src/costa2019.egg-info/SOURCES.txt` & `costa2019-1.2.0/src/costa2019.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

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
 src/costa2019/__init__.py
 src/costa2019/info.py
 src/costa2019/version.py
 src/costa2019.egg-info/PKG-INFO
 src/costa2019.egg-info/SOURCES.txt
 src/costa2019.egg-info/dependency_links.txt
-src/costa2019.egg-info/not-zip-safe
+src/costa2019.egg-info/requires.txt
 src/costa2019.egg-info/top_level.txt
 src/costa2019/clean/fig1.csv
 src/costa2019/clean/fig5.csv
 src/costa2019/clean/info.json
 src/costa2019/clean/readme.rst
 src/costa2019/clean/tab4.csv
 test/conftest.py
```

### Comparing `costa2019-1.1.0/test/conftest.py` & `costa2019-1.2.0/test/conftest.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 import os
 
 import pytest
 # #}
 
 
 # {# pkglts, test.pytest_cmdline_preparse
-def pytest_cmdline_preparse(args):
-    if 'PYCHARM_HOSTED' not in os.environ:
-        args.append("--cov=costa2019")
+# def pytest_cmdline_preparse(args):
+#
+#     if 'PYCHARM_HOSTED' not in os.environ:
+#         args.append("--cov=costa2019")
+#
 # #}
 
 
 # {# pkglts, test.pytest_addoption
 def pytest_addoption(parser):
     parser.addoption("--runslow", action="store_true",
                      default=False, help="run slow tests")
```

