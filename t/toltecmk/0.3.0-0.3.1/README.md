# Comparing `tmp/toltecmk-0.3.0.tar.gz` & `tmp/toltecmk-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toltecmk-0.3.0.tar", last modified: Wed Jan  3 02:53:03 2024, max compression
+gzip compressed data, was "toltecmk-0.3.1.tar", last modified: Mon May 20 19:20:54 2024, max compression
```

## Comparing `toltecmk-0.3.0.tar` & `toltecmk-0.3.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 02:53:03.397889 toltecmk-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-01-03 02:52:44.000000 toltecmk-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-01-03 02:53:03.397889 toltecmk-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-01-03 02:52:44.000000 toltecmk-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-01-03 02:52:44.000000 toltecmk-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-01-03 02:52:44.000000 toltecmk-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-03 02:53:03.397889 toltecmk-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 02:53:03.393889 toltecmk-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-01-03 02:52:44.000000 toltecmk-0.3.0/tests/test_ipk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-01-03 02:52:44.000000 toltecmk-0.3.0/tests/test_recipe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-01-03 02:52:44.000000 toltecmk-0.3.0/tests/test_strip.py
--rw-r--r--   0 runner    (1001) docker     (127)     6112 2024-01-03 02:52:44.000000 toltecmk-0.3.0/tests/test_toltec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9862 2024-01-03 02:52:44.000000 toltecmk-0.3.0/tests/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 02:53:03.397889 toltecmk-0.3.0/toltec/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-01-03 02:52:44.000000 toltecmk-0.3.0/toltec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-01-03 02:52:44.000000 toltecmk-0.3.0/toltec/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13255 2024-01-03 02:52:44.000000 toltecmk-0.3.0/toltec/bash.py
--rw-r--r--   0 runner    (1001) docker     (127)    16023 2024-01-03 02:52:44.000000 toltecmk-0.3.0/toltec/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 02:53:03.397889 toltecmk-0.3.0/toltec/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-01-03 02:52:44.000000 toltecmk-0.3.0/toltec/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-01-03 02:52:44.000000 toltecmk-0.3.0/toltec/hooks/install_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-01-03 02:52:44.000000 toltecmk-0.3.0/toltec/hooks/patch_rm2fb.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-03 02:52:44.000000 toltecmk-0.3.0/toltec/hooks/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-01-03 02:52:44.000000 toltecmk-0.3.0/toltec/hooks/reload_oxide_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-01-03 02:52:44.000000 toltecmk-0.3.0/toltec/hooks/strip.py
--rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-01-03 02:52:44.000000 toltecmk-0.3.0/toltec/ipk.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-03 02:52:44.000000 toltecmk-0.3.0/toltec/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-01-03 02:52:44.000000 toltecmk-0.3.0/toltec/recipe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 02:53:03.397889 toltecmk-0.3.0/toltec/recipe_parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-01-03 02:52:44.000000 toltecmk-0.3.0/toltec/recipe_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13185 2024-01-03 02:52:44.000000 toltecmk-0.3.0/toltec/recipe_parsers/bash.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-03 02:52:44.000000 toltecmk-0.3.0/toltec/recipe_parsers/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-01-03 02:52:44.000000 toltecmk-0.3.0/toltec/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)    10931 2024-01-03 02:52:44.000000 toltecmk-0.3.0/toltec/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    12758 2024-01-03 02:52:44.000000 toltecmk-0.3.0/toltec/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 02:53:03.397889 toltecmk-0.3.0/toltecmk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-01-03 02:53:03.000000 toltecmk-0.3.0/toltecmk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-01-03 02:53:03.000000 toltecmk-0.3.0/toltecmk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-03 02:53:03.000000 toltecmk-0.3.0/toltecmk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-01-03 02:53:03.000000 toltecmk-0.3.0/toltecmk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-01-03 02:53:03.000000 toltecmk-0.3.0/toltecmk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-03 02:53:03.000000 toltecmk-0.3.0/toltecmk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:20:54.916532 toltecmk-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-20 19:20:36.000000 toltecmk-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6537 2024-05-20 19:20:54.916532 toltecmk-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-05-20 19:20:36.000000 toltecmk-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-20 19:20:36.000000 toltecmk-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-20 19:20:36.000000 toltecmk-0.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 19:20:54.916532 toltecmk-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:20:54.912532 toltecmk-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-05-20 19:20:36.000000 toltecmk-0.3.1/tests/test_ipk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-20 19:20:36.000000 toltecmk-0.3.1/tests/test_recipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-05-20 19:20:36.000000 toltecmk-0.3.1/tests/test_strip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6112 2024-05-20 19:20:36.000000 toltecmk-0.3.1/tests/test_toltec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9862 2024-05-20 19:20:36.000000 toltecmk-0.3.1/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:20:54.916532 toltecmk-0.3.1/toltec/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-20 19:20:36.000000 toltecmk-0.3.1/toltec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-05-20 19:20:36.000000 toltecmk-0.3.1/toltec/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13255 2024-05-20 19:20:36.000000 toltecmk-0.3.1/toltec/bash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16023 2024-05-20 19:20:36.000000 toltecmk-0.3.1/toltec/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:20:54.916532 toltecmk-0.3.1/toltec/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-20 19:20:36.000000 toltecmk-0.3.1/toltec/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-05-20 19:20:36.000000 toltecmk-0.3.1/toltec/hooks/install_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-20 19:20:36.000000 toltecmk-0.3.1/toltec/hooks/patch_rm2fb.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:20:36.000000 toltecmk-0.3.1/toltec/hooks/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-20 19:20:36.000000 toltecmk-0.3.1/toltec/hooks/reload_oxide_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-05-20 19:20:36.000000 toltecmk-0.3.1/toltec/hooks/strip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-05-20 19:20:36.000000 toltecmk-0.3.1/toltec/ipk.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:20:36.000000 toltecmk-0.3.1/toltec/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-05-20 19:20:36.000000 toltecmk-0.3.1/toltec/recipe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:20:54.916532 toltecmk-0.3.1/toltec/recipe_parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-20 19:20:36.000000 toltecmk-0.3.1/toltec/recipe_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13185 2024-05-20 19:20:36.000000 toltecmk-0.3.1/toltec/recipe_parsers/bash.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:20:36.000000 toltecmk-0.3.1/toltec/recipe_parsers/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-20 19:20:36.000000 toltecmk-0.3.1/toltec/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10931 2024-05-20 19:20:36.000000 toltecmk-0.3.1/toltec/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12758 2024-05-20 19:20:36.000000 toltecmk-0.3.1/toltec/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:20:54.916532 toltecmk-0.3.1/toltecmk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6537 2024-05-20 19:20:54.000000 toltecmk-0.3.1/toltecmk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-20 19:20:54.000000 toltecmk-0.3.1/toltecmk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 19:20:54.000000 toltecmk-0.3.1/toltecmk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-20 19:20:54.000000 toltecmk-0.3.1/toltecmk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-20 19:20:54.000000 toltecmk-0.3.1/toltecmk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 19:20:54.000000 toltecmk-0.3.1/toltecmk.egg-info/top_level.txt
```

### Comparing `toltecmk-0.3.0/LICENSE` & `toltecmk-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `toltecmk-0.3.0/PKG-INFO` & `toltecmk-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toltecmk
-Version: 0.3.0
+Version: 0.3.1
 Summary: Build system used for the Toltec community repository
 Author-email: Mattéo Delabre <git.matteo@delab.re>, Eeems <eeems@eeems.email>
 Project-URL: Homepage, https://github.com/toltec-dev/build
 Project-URL: Bug Tracker, https://github.com/toltec-dev/build/issues
 Keywords: build-tooling,packaging,distribution
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -14,17 +14,18 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: System :: Archiving :: Packaging
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: docker==6.1.3
+Requires-Dist: docker==7.0.0
 Requires-Dist: python-dateutil==2.8.2
 Requires-Dist: pyelftools==0.30
+Requires-Dist: requests==2.31.0
 
 ## toltecmk
 
 [![toltecmk on PyPI](https://img.shields.io/pypi/v/toltecmk)](https://pypi.org/project/toltecmk)
 ![Status of the main branch](https://github.com/toltec-dev/build/actions/workflows/checks.yml/badge.svg)
 
 `toltecmk` is a Python tool used to build software packages for the [Toltec repository](https://github.com/toltec-dev/toltec) from _[PKGBUILD](https://wiki.archlinux.org/index.php/PKGBUILD)-like build recipes_.
```

#### html2text {}

```diff
@@ -1,31 +1,32 @@
-Metadata-Version: 2.1 Name: toltecmk Version: 0.3.0 Summary: Build system used
+Metadata-Version: 2.1 Name: toltecmk Version: 0.3.1 Summary: Build system used
 for the Toltec community repository Author-email: MattÃ©o Delabre
 delab.re>, Eeems
 eeems.email> Project-URL: Homepage, https://github.com/toltec-dev/build
 Project-URL: Bug Tracker, https://github.com/toltec-dev/build/issues Keywords:
 build-tooling,packaging,distribution Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: POSIX :: Linux Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Topic :: Software Development :: Build Tools Classifier: Topic :: System ::
 Archiving :: Packaging Requires-Python: >=3.11 Description-Content-Type: text/
-markdown License-File: LICENSE Requires-Dist: docker==6.1.3 Requires-Dist:
-python-dateutil==2.8.2 Requires-Dist: pyelftools==0.30 ## toltecmk [![toltecmk
-on PyPI](https://img.shields.io/pypi/v/toltecmk)](https://pypi.org/project/
-toltecmk) ![Status of the main branch](https://github.com/toltec-dev/build/
-actions/workflows/checks.yml/badge.svg) `toltecmk` is a Python tool used to
-build software packages for the [Toltec repository](https://github.com/toltec-
-dev/toltec) from _[PKGBUILD](https://wiki.archlinux.org/index.php/PKGBUILD)-
-like build recipes_. It automates common tasks such as fetching sources,
-building artifacts in a reproducible environment, and creating [Opkg-compatible
-archives](docs/ipk.md). **Disclaimer: This is beta-quality software. The recipe
-format may change at any time in future releases. If you use `toltecmk` in
-other projects, it is advised to pin to a specific version.**
+markdown License-File: LICENSE Requires-Dist: docker==7.0.0 Requires-Dist:
+python-dateutil==2.8.2 Requires-Dist: pyelftools==0.30 Requires-Dist:
+requests==2.31.0 ## toltecmk [![toltecmk on PyPI](https://img.shields.io/pypi/
+v/toltecmk)](https://pypi.org/project/toltecmk) ![Status of the main branch]
+(https://github.com/toltec-dev/build/actions/workflows/checks.yml/badge.svg)
+`toltecmk` is a Python tool used to build software packages for the [Toltec
+repository](https://github.com/toltec-dev/toltec) from _[PKGBUILD](https://
+wiki.archlinux.org/index.php/PKGBUILD)-like build recipes_. It automates common
+tasks such as fetching sources, building artifacts in a reproducible
+environment, and creating [Opkg-compatible archives](docs/ipk.md).
+**Disclaimer: This is beta-quality software. The recipe format may change at
+any time in future releases. If you use `toltecmk` in other projects, it is
+advised to pin to a specific version.**
       [toltecmk input: recipe; output: packages. Fetches sources based on
                          instructions in the recipe.]
 ### Setup `toltecmk` is available as a Python package on PyPI. ```sh pip
 install toltecmk ``` There are a few system requirements to use this tool: *
 Linux-based operating system * Python â©¾Â 3.11 * Docker ### Basic Usage To
 build a recipe located in the current directory, simply run: ```sh toltecmk ```
 This will process the recipe in a subfolder called `build` (which can be
```

### Comparing `toltecmk-0.3.0/README.md` & `toltecmk-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `toltecmk-0.3.0/pyproject.toml` & `toltecmk-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "toltecmk"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
   { name="Mattéo Delabre", email="git.matteo@delab.re" },
   { name="Eeems", email="eeems@eeems.email" },
 ]
 description = "Build system used for the Toltec community repository"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `toltecmk-0.3.0/tests/test_ipk.py` & `toltecmk-0.3.1/tests/test_ipk.py`

 * *Files identical despite different names*

### Comparing `toltecmk-0.3.0/tests/test_recipe.py` & `toltecmk-0.3.1/tests/test_recipe.py`

 * *Files identical despite different names*

### Comparing `toltecmk-0.3.0/tests/test_strip.py` & `toltecmk-0.3.1/tests/test_strip.py`

 * *Files identical despite different names*

### Comparing `toltecmk-0.3.0/tests/test_toltec.py` & `toltecmk-0.3.1/tests/test_toltec.py`

 * *Files identical despite different names*

### Comparing `toltecmk-0.3.0/tests/test_version.py` & `toltecmk-0.3.1/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `toltecmk-0.3.0/toltec/__main__.py` & `toltecmk-0.3.1/toltec/__main__.py`

 * *Files identical despite different names*

### Comparing `toltecmk-0.3.0/toltec/bash.py` & `toltecmk-0.3.1/toltec/bash.py`

 * *Files identical despite different names*

### Comparing `toltecmk-0.3.0/toltec/builder.py` & `toltecmk-0.3.1/toltec/builder.py`

 * *Files identical despite different names*

### Comparing `toltecmk-0.3.0/toltec/hooks/install_lib.py` & `toltecmk-0.3.1/toltec/hooks/install_lib.py`

 * *Files identical despite different names*

### Comparing `toltecmk-0.3.0/toltec/hooks/patch_rm2fb.py` & `toltecmk-0.3.1/toltec/hooks/patch_rm2fb.py`

 * *Files identical despite different names*

### Comparing `toltecmk-0.3.0/toltec/hooks/reload_oxide_apps.py` & `toltecmk-0.3.1/toltec/hooks/reload_oxide_apps.py`

 * *Files identical despite different names*

### Comparing `toltecmk-0.3.0/toltec/hooks/strip.py` & `toltecmk-0.3.1/toltec/hooks/strip.py`

 * *Files identical despite different names*

### Comparing `toltecmk-0.3.0/toltec/ipk.py` & `toltecmk-0.3.1/toltec/ipk.py`

 * *Files identical despite different names*

### Comparing `toltecmk-0.3.0/toltec/recipe.py` & `toltecmk-0.3.1/toltec/recipe.py`

 * *Files identical despite different names*

### Comparing `toltecmk-0.3.0/toltec/recipe_parsers/__init__.py` & `toltecmk-0.3.1/toltec/recipe_parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `toltecmk-0.3.0/toltec/recipe_parsers/bash.py` & `toltecmk-0.3.1/toltec/recipe_parsers/bash.py`

 * *Files identical despite different names*

### Comparing `toltecmk-0.3.0/toltec/repo.py` & `toltecmk-0.3.1/toltec/repo.py`

 * *Files identical despite different names*

### Comparing `toltecmk-0.3.0/toltec/util.py` & `toltecmk-0.3.1/toltec/util.py`

 * *Files identical despite different names*

### Comparing `toltecmk-0.3.0/toltec/version.py` & `toltecmk-0.3.1/toltec/version.py`

 * *Files identical despite different names*

### Comparing `toltecmk-0.3.0/toltecmk.egg-info/PKG-INFO` & `toltecmk-0.3.1/toltecmk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toltecmk
-Version: 0.3.0
+Version: 0.3.1
 Summary: Build system used for the Toltec community repository
 Author-email: Mattéo Delabre <git.matteo@delab.re>, Eeems <eeems@eeems.email>
 Project-URL: Homepage, https://github.com/toltec-dev/build
 Project-URL: Bug Tracker, https://github.com/toltec-dev/build/issues
 Keywords: build-tooling,packaging,distribution
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -14,17 +14,18 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: System :: Archiving :: Packaging
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: docker==6.1.3
+Requires-Dist: docker==7.0.0
 Requires-Dist: python-dateutil==2.8.2
 Requires-Dist: pyelftools==0.30
+Requires-Dist: requests==2.31.0
 
 ## toltecmk
 
 [![toltecmk on PyPI](https://img.shields.io/pypi/v/toltecmk)](https://pypi.org/project/toltecmk)
 ![Status of the main branch](https://github.com/toltec-dev/build/actions/workflows/checks.yml/badge.svg)
 
 `toltecmk` is a Python tool used to build software packages for the [Toltec repository](https://github.com/toltec-dev/toltec) from _[PKGBUILD](https://wiki.archlinux.org/index.php/PKGBUILD)-like build recipes_.
```

#### html2text {}

```diff
@@ -1,31 +1,32 @@
-Metadata-Version: 2.1 Name: toltecmk Version: 0.3.0 Summary: Build system used
+Metadata-Version: 2.1 Name: toltecmk Version: 0.3.1 Summary: Build system used
 for the Toltec community repository Author-email: MattÃ©o Delabre
 delab.re>, Eeems
 eeems.email> Project-URL: Homepage, https://github.com/toltec-dev/build
 Project-URL: Bug Tracker, https://github.com/toltec-dev/build/issues Keywords:
 build-tooling,packaging,distribution Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: POSIX :: Linux Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Topic :: Software Development :: Build Tools Classifier: Topic :: System ::
 Archiving :: Packaging Requires-Python: >=3.11 Description-Content-Type: text/
-markdown License-File: LICENSE Requires-Dist: docker==6.1.3 Requires-Dist:
-python-dateutil==2.8.2 Requires-Dist: pyelftools==0.30 ## toltecmk [![toltecmk
-on PyPI](https://img.shields.io/pypi/v/toltecmk)](https://pypi.org/project/
-toltecmk) ![Status of the main branch](https://github.com/toltec-dev/build/
-actions/workflows/checks.yml/badge.svg) `toltecmk` is a Python tool used to
-build software packages for the [Toltec repository](https://github.com/toltec-
-dev/toltec) from _[PKGBUILD](https://wiki.archlinux.org/index.php/PKGBUILD)-
-like build recipes_. It automates common tasks such as fetching sources,
-building artifacts in a reproducible environment, and creating [Opkg-compatible
-archives](docs/ipk.md). **Disclaimer: This is beta-quality software. The recipe
-format may change at any time in future releases. If you use `toltecmk` in
-other projects, it is advised to pin to a specific version.**
+markdown License-File: LICENSE Requires-Dist: docker==7.0.0 Requires-Dist:
+python-dateutil==2.8.2 Requires-Dist: pyelftools==0.30 Requires-Dist:
+requests==2.31.0 ## toltecmk [![toltecmk on PyPI](https://img.shields.io/pypi/
+v/toltecmk)](https://pypi.org/project/toltecmk) ![Status of the main branch]
+(https://github.com/toltec-dev/build/actions/workflows/checks.yml/badge.svg)
+`toltecmk` is a Python tool used to build software packages for the [Toltec
+repository](https://github.com/toltec-dev/toltec) from _[PKGBUILD](https://
+wiki.archlinux.org/index.php/PKGBUILD)-like build recipes_. It automates common
+tasks such as fetching sources, building artifacts in a reproducible
+environment, and creating [Opkg-compatible archives](docs/ipk.md).
+**Disclaimer: This is beta-quality software. The recipe format may change at
+any time in future releases. If you use `toltecmk` in other projects, it is
+advised to pin to a specific version.**
       [toltecmk input: recipe; output: packages. Fetches sources based on
                          instructions in the recipe.]
 ### Setup `toltecmk` is available as a Python package on PyPI. ```sh pip
 install toltecmk ``` There are a few system requirements to use this tool: *
 Linux-based operating system * Python â©¾Â 3.11 * Docker ### Basic Usage To
 build a recipe located in the current directory, simply run: ```sh toltecmk ```
 This will process the recipe in a subfolder called `build` (which can be
```

### Comparing `toltecmk-0.3.0/toltecmk.egg-info/SOURCES.txt` & `toltecmk-0.3.1/toltecmk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

