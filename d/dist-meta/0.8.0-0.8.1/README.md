# Comparing `tmp/dist-meta-0.8.0.tar.gz` & `tmp/dist-meta-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist-meta-0.8.0.tar", last modified: Tue Apr 25 08:56:44 2023, max compression
+gzip compressed data, was "dist-meta-0.8.1.tar", last modified: Mon May 20 18:09:29 2024, max compression
```

## Comparing `dist-meta-0.8.0.tar` & `dist-meta-0.8.1.tar`

### file list

```diff
@@ -1,34 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:56:44.012237 dist-meta-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-04-25 08:56:05.000000 dist-meta-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      123 2023-04-25 08:56:05.000000 dist-meta-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     7935 2023-04-25 08:56:44.012237 dist-meta-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5116 2023-04-25 08:56:05.000000 dist-meta-0.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:56:44.008237 dist-meta-0.8.0/dist_meta/
--rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-04-25 08:56:05.000000 dist-meta-0.8.0/dist_meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3168 2023-04-25 08:56:05.000000 dist-meta-0.8.0/dist_meta/_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    18820 2023-04-25 08:56:05.000000 dist-meta-0.8.0/dist_meta/distributions.py
--rw-r--r--   0 runner    (1001) docker     (122)    10350 2023-04-25 08:56:05.000000 dist-meta-0.8.0/dist_meta/entry_points.py
--rw-r--r--   0 runner    (1001) docker     (122)     6810 2023-04-25 08:56:05.000000 dist-meta-0.8.0/dist_meta/metadata.py
--rw-r--r--   0 runner    (1001) docker     (122)     8649 2023-04-25 08:56:05.000000 dist-meta-0.8.0/dist_meta/metadata_mapping.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 08:56:05.000000 dist-meta-0.8.0/dist_meta/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     8678 2023-04-25 08:56:05.000000 dist-meta-0.8.0/dist_meta/record.py
--rw-r--r--   0 runner    (1001) docker     (122)     4541 2023-04-25 08:56:05.000000 dist-meta-0.8.0/dist_meta/wheel.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:56:44.008237 dist-meta-0.8.0/dist_meta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7935 2023-04-25 08:56:43.000000 dist-meta-0.8.0/dist_meta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      668 2023-04-25 08:56:44.000000 dist-meta-0.8.0/dist_meta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 08:56:43.000000 dist-meta-0.8.0/dist_meta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 08:56:43.000000 dist-meta-0.8.0/dist_meta.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-04-25 08:56:43.000000 dist-meta-0.8.0/dist_meta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-25 08:56:43.000000 dist-meta-0.8.0/dist_meta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4896 2023-04-25 08:56:05.000000 dist-meta-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-04-25 08:56:05.000000 dist-meta-0.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-04-25 08:56:44.012237 dist-meta-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      597 2023-04-25 08:56:05.000000 dist-meta-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:56:44.012237 dist-meta-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)    19121 2023-04-25 08:56:05.000000 dist-meta-0.8.0/tests/test_distributions.py
--rw-r--r--   0 runner    (1001) docker     (122)    10134 2023-04-25 08:56:05.000000 dist-meta-0.8.0/tests/test_entry_points.py
--rw-r--r--   0 runner    (1001) docker     (122)    10319 2023-04-25 08:56:05.000000 dist-meta-0.8.0/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (122)     3975 2023-04-25 08:56:05.000000 dist-meta-0.8.0/tests/test_metadata_mapping.py
--rw-r--r--   0 runner    (1001) docker     (122)     6189 2023-04-25 08:56:05.000000 dist-meta-0.8.0/tests/test_metadata_top_packages.py
--rw-r--r--   0 runner    (1001) docker     (122)     6993 2023-04-25 08:56:05.000000 dist-meta-0.8.0/tests/test_record.py
--rw-r--r--   0 runner    (1001) docker     (122)     4729 2023-04-25 08:56:05.000000 dist-meta-0.8.0/tests/test_wheel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:09:29.880940 dist-meta-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-20 18:09:06.000000 dist-meta-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-20 18:09:06.000000 dist-meta-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7986 2024-05-20 18:09:29.880940 dist-meta-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5116 2024-05-20 18:09:06.000000 dist-meta-0.8.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:09:29.880940 dist-meta-0.8.1/dist_meta/
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-20 18:09:06.000000 dist-meta-0.8.1/dist_meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-05-20 18:09:06.000000 dist-meta-0.8.1/dist_meta/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18820 2024-05-20 18:09:06.000000 dist-meta-0.8.1/dist_meta/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10350 2024-05-20 18:09:06.000000 dist-meta-0.8.1/dist_meta/entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-05-20 18:09:06.000000 dist-meta-0.8.1/dist_meta/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8649 2024-05-20 18:09:06.000000 dist-meta-0.8.1/dist_meta/metadata_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 18:09:06.000000 dist-meta-0.8.1/dist_meta/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8678 2024-05-20 18:09:06.000000 dist-meta-0.8.1/dist_meta/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-05-20 18:09:06.000000 dist-meta-0.8.1/dist_meta/wheel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:09:29.880940 dist-meta-0.8.1/dist_meta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7986 2024-05-20 18:09:29.000000 dist-meta-0.8.1/dist_meta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-20 18:09:29.000000 dist-meta-0.8.1/dist_meta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 18:09:29.000000 dist-meta-0.8.1/dist_meta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 18:09:29.000000 dist-meta-0.8.1/dist_meta.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-20 18:09:29.000000 dist-meta-0.8.1/dist_meta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 18:09:29.000000 dist-meta-0.8.1/dist_meta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-05-20 18:09:06.000000 dist-meta-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-20 18:09:06.000000 dist-meta-0.8.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-20 18:09:29.884940 dist-meta-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-20 18:09:06.000000 dist-meta-0.8.1/setup.py
```

### Comparing `dist-meta-0.8.0/LICENSE` & `dist-meta-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dist-meta-0.8.0/PKG-INFO` & `dist-meta-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dist-meta
-Version: 0.8.0
+Version: 0.8.1
 Summary: Parse and create Python distribution metadata.
 Home-page: https://github.com/repo-helper/dist-meta
 Author: Dominic Davis-Foster
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: Copyright (c) 2021 Dominic Davis-Foster
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -41,14 +41,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Typing :: Typed
 Requires-Python: >=3.6.1
 Description-Content-Type: text/x-rst
@@ -153,23 +154,23 @@
 .. |license| image:: https://img.shields.io/github/license/repo-helper/dist-meta
 	:target: https://github.com/repo-helper/dist-meta/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/repo-helper/dist-meta
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/dist-meta/v0.8.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/dist-meta/v0.8.1
 	:target: https://github.com/repo-helper/dist-meta/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/dist-meta
 	:target: https://github.com/repo-helper/dist-meta/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2024
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/dist-meta
 	:target: https://pypi.org/project/dist-meta/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `dist-meta-0.8.0/README.rst` & `dist-meta-0.8.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -97,23 +97,23 @@
 .. |license| image:: https://img.shields.io/github/license/repo-helper/dist-meta
 	:target: https://github.com/repo-helper/dist-meta/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/repo-helper/dist-meta
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/dist-meta/v0.8.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/dist-meta/v0.8.1
 	:target: https://github.com/repo-helper/dist-meta/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/dist-meta
 	:target: https://github.com/repo-helper/dist-meta/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2024
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/dist-meta
 	:target: https://pypi.org/project/dist-meta/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `dist-meta-0.8.0/dist_meta/__init__.py` & `dist-meta-0.8.1/dist_meta/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,9 +29,9 @@
 # this package
 from dist_meta.distributions import get_distribution, iter_distributions  # noqa: F401
 from dist_meta.entry_points import get_all_entry_points, get_entry_points  # noqa: F401
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2021 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "0.8.0"
+__version__: str = "0.8.1"
 __email__: str = "dominic@davis-foster.co.uk"
```

### Comparing `dist-meta-0.8.0/dist_meta/_utils.py` & `dist-meta-0.8.1/dist_meta/_utils.py`

 * *Files identical despite different names*

### Comparing `dist-meta-0.8.0/dist_meta/distributions.py` & `dist-meta-0.8.1/dist_meta/distributions.py`

 * *Files identical despite different names*

### Comparing `dist-meta-0.8.0/dist_meta/entry_points.py` & `dist-meta-0.8.1/dist_meta/entry_points.py`

 * *Files identical despite different names*

### Comparing `dist-meta-0.8.0/dist_meta/metadata.py` & `dist-meta-0.8.1/dist_meta/metadata.py`

 * *Files identical despite different names*

### Comparing `dist-meta-0.8.0/dist_meta/metadata_mapping.py` & `dist-meta-0.8.1/dist_meta/metadata_mapping.py`

 * *Files identical despite different names*

### Comparing `dist-meta-0.8.0/dist_meta/record.py` & `dist-meta-0.8.1/dist_meta/record.py`

 * *Files identical despite different names*

### Comparing `dist-meta-0.8.0/dist_meta/wheel.py` & `dist-meta-0.8.1/dist_meta/wheel.py`

 * *Files identical despite different names*

### Comparing `dist-meta-0.8.0/dist_meta.egg-info/PKG-INFO` & `dist-meta-0.8.1/dist_meta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dist-meta
-Version: 0.8.0
+Version: 0.8.1
 Summary: Parse and create Python distribution metadata.
 Home-page: https://github.com/repo-helper/dist-meta
 Author: Dominic Davis-Foster
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: Copyright (c) 2021 Dominic Davis-Foster
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -41,14 +41,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Typing :: Typed
 Requires-Python: >=3.6.1
 Description-Content-Type: text/x-rst
@@ -153,23 +154,23 @@
 .. |license| image:: https://img.shields.io/github/license/repo-helper/dist-meta
 	:target: https://github.com/repo-helper/dist-meta/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/repo-helper/dist-meta
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/dist-meta/v0.8.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/dist-meta/v0.8.1
 	:target: https://github.com/repo-helper/dist-meta/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/dist-meta
 	:target: https://github.com/repo-helper/dist-meta/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2024
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/dist-meta
 	:target: https://pypi.org/project/dist-meta/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `dist-meta-0.8.0/pyproject.toml` & `dist-meta-0.8.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = [ "setuptools!=61.*,>=40.6.0", "wheel>=0.34.2",]
+requires = [ "setuptools!=61.*,<=67.1.0,>=40.6.0", "wheel>=0.34.2",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dist-meta"
-version = "0.8.0"
+version = "0.8.1"
 description = "Parse and create Python distribution metadata."
 readme = "README.rst"
 requires-python = ">=3.6.1"
 keywords = [ "dist-info", "metadata", "packaging", "pypi",]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
@@ -18,30 +18,30 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: System :: Archiving :: Packaging",
     "Typing :: Typed",
 ]
 dynamic = [ "dependencies",]
 
+[project.license]
+file = "LICENSE"
+
 [[project.authors]]
 name = "Dominic Davis-Foster"
 email = "dominic@davis-foster.co.uk"
 
-
-[project.license]
-file = "LICENSE"
-
 [project.urls]
 Homepage = "https://github.com/repo-helper/dist-meta"
 "Issue Tracker" = "https://github.com/repo-helper/dist-meta/issues"
 "Source Code" = "https://github.com/repo-helper/dist-meta"
 Documentation = "https://dist-meta.readthedocs.io/en/latest"
 
 [tool.mkrecipe]
@@ -67,28 +67,26 @@
     "sphinxcontrib.toctree_plus",
     "sphinx_toolbox.tweaks.latex_layout",
     "sphinx_toolbox.tweaks.latex_toc",
     "sphinx.ext.intersphinx",
     "sphinx.ext.mathjax",
     "sphinxcontrib.extras_require",
     "sphinx.ext.todo",
-    "sphinxemoji.sphinxemoji",
     "notfound.extension",
     "sphinx_copybutton",
     "sphinxcontrib.default_values",
     "sphinx_debuginfo",
     "sphinx_licenseinfo",
     "seed_intersphinx_mapping",
     "html_section",
     "sphinx_toolbox.more_autosummary.column_widths",
     "sphinx_toolbox.latex.succinct_seealso",
     "sphinx_packaging.peps",
     "local_extension",
 ]
-sphinxemoji_style = "twemoji"
 gitstamp_fmt = "%d %b %Y"
 templates_path = [ "_templates",]
 html_static_path = [ "_static",]
 source_suffix = ".rst"
 master_doc = "index"
 suppress_warnings = [ "image.nonlocal_uri",]
 pygments_style = "default"
@@ -137,15 +135,15 @@
 base-classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: System :: Archiving :: Packaging",
     "Typing :: Typed",
 ]
-python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10", "3.11",]
+python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10", "3.11", "3.12",]
 python-implementations = [ "CPython", "PyPy",]
 platforms = [ "Windows", "macOS", "Linux",]
 license-key = "MIT"
 package = "dist_meta"
 
 [tool.mypy]
 python_version = "3.8"
@@ -155,14 +153,24 @@
 no_implicit_optional = true
 show_error_codes = true
 incremental = false
 
 [tool.snippet-fmt]
 directives = [ "code-block",]
 
+[tool.snippet-fmt.languages.python]
+reformat = true
+
+[tool.snippet-fmt.languages.TOML]
+reformat = true
+
+[tool.snippet-fmt.languages.ini]
+
+[tool.snippet-fmt.languages.json]
+
 [tool.setuptools]
 zip-safe = false
 include-package-data = true
 platforms = [ "Windows", "macOS", "Linux",]
 
 [tool.dependency-dash."requirements.txt"]
 order = 10
@@ -170,17 +178,7 @@
 [tool.dependency-dash."tests/requirements.txt"]
 order = 20
 include = false
 
 [tool.dependency-dash."doc-source/requirements.txt"]
 order = 30
 include = false
-
-[tool.snippet-fmt.languages.python]
-reformat = true
-
-[tool.snippet-fmt.languages.TOML]
-reformat = true
-
-[tool.snippet-fmt.languages.ini]
-
-[tool.snippet-fmt.languages.json]
```

### Comparing `dist-meta-0.8.0/setup.cfg` & `dist-meta-0.8.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dist-meta
-version = 0.8.0
+version = 0.8.1
 author = Dominic Davis-Foster
 author_email = dominic@davis-foster.co.uk
 license = MIT License
 keywords = packaging, dist-info, metadata, pypi
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 platforms = Windows, macOS, Linux
@@ -22,14 +22,15 @@
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 	Topic :: Software Development :: Libraries :: Python Modules
 	Topic :: System :: Archiving :: Packaging
 	Typing :: Typed
 
 [options]
```

### Comparing `dist-meta-0.8.0/setup.py` & `dist-meta-0.8.1/setup.py`

 * *Files identical despite different names*

