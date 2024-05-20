# Comparing `tmp/create_redirect-0.2.0.tar.gz` & `tmp/create_redirect-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "create_redirect-0.2.0.tar", last modified: Wed Dec 13 14:39:52 2023, max compression
+gzip compressed data, was "create_redirect-0.2.1.tar", last modified: Mon May 20 16:44:00 2024, max compression
```

## Comparing `create_redirect-0.2.0.tar` & `create_redirect-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 14:39:52.879112 create_redirect-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-12-13 14:39:31.000000 create_redirect-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      135 2023-12-13 14:39:31.000000 create_redirect-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7402 2023-12-13 14:39:52.879112 create_redirect-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2023-12-13 14:39:31.000000 create_redirect-0.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 14:39:52.875112 create_redirect-0.2.0/create_redirect/
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2023-12-13 14:39:31.000000 create_redirect-0.2.0/create_redirect/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2301 2023-12-13 14:39:31.000000 create_redirect-0.2.0/create_redirect/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 14:39:52.879112 create_redirect-0.2.0/create_redirect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7402 2023-12-13 14:39:52.000000 create_redirect-0.2.0/create_redirect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      422 2023-12-13 14:39:52.000000 create_redirect-0.2.0/create_redirect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 14:39:52.000000 create_redirect-0.2.0/create_redirect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-13 14:39:52.000000 create_redirect-0.2.0/create_redirect.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 14:39:52.000000 create_redirect-0.2.0/create_redirect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-13 14:39:52.000000 create_redirect-0.2.0/create_redirect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4656 2023-12-13 14:39:31.000000 create_redirect-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 14:39:31.000000 create_redirect-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2023-12-13 14:39:52.879112 create_redirect-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      605 2023-12-13 14:39:31.000000 create_redirect-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 14:39:52.875112 create_redirect-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      950 2023-12-13 14:39:31.000000 create_redirect-0.2.0/tests/test_create_redirect.py
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2023-12-13 14:39:31.000000 create_redirect-0.2.0/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:44:00.198895 create_redirect-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-20 16:43:32.000000 create_redirect-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-20 16:43:32.000000 create_redirect-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7402 2024-05-20 16:44:00.198895 create_redirect-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-20 16:43:32.000000 create_redirect-0.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:44:00.194895 create_redirect-0.2.1/create_redirect/
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-20 16:43:32.000000 create_redirect-0.2.1/create_redirect/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2301 2024-05-20 16:43:32.000000 create_redirect-0.2.1/create_redirect/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:44:00.198895 create_redirect-0.2.1/create_redirect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7402 2024-05-20 16:44:00.000000 create_redirect-0.2.1/create_redirect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-20 16:44:00.000000 create_redirect-0.2.1/create_redirect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 16:44:00.000000 create_redirect-0.2.1/create_redirect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-20 16:44:00.000000 create_redirect-0.2.1/create_redirect.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 16:44:00.000000 create_redirect-0.2.1/create_redirect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-20 16:44:00.000000 create_redirect-0.2.1/create_redirect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-05-20 16:43:32.000000 create_redirect-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 16:43:32.000000 create_redirect-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-20 16:44:00.198895 create_redirect-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-20 16:43:32.000000 create_redirect-0.2.1/setup.py
```

### Comparing `create_redirect-0.2.0/LICENSE` & `create_redirect-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `create_redirect-0.2.0/PKG-INFO` & `create_redirect-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: create_redirect
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python script for creating HTML redirects.
 Home-page: https://github.com/domdfcoding/create_redirect
 Author: Dominic Davis-Foster
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: Copyright (c) 2020 Dominic Davis-Foster
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -141,23 +141,23 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/create_redirect
 	:target: https://github.com/domdfcoding/create_redirect/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/create_redirect
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/create_redirect/v0.2.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/create_redirect/v0.2.1
 	:target: https://github.com/domdfcoding/create_redirect/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/create_redirect
 	:target: https://github.com/domdfcoding/create_redirect/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2024
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/create_redirect
 	:target: https://pypi.org/project/create_redirect/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `create_redirect-0.2.0/README.rst` & `create_redirect-0.2.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -87,23 +87,23 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/create_redirect
 	:target: https://github.com/domdfcoding/create_redirect/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/create_redirect
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/create_redirect/v0.2.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/create_redirect/v0.2.1
 	:target: https://github.com/domdfcoding/create_redirect/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/create_redirect
 	:target: https://github.com/domdfcoding/create_redirect/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2024
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/create_redirect
 	:target: https://pypi.org/project/create_redirect/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `create_redirect-0.2.0/create_redirect/__init__.py` & `create_redirect-0.2.1/create_redirect/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from textwrap import dedent
 
 __all__ = ["create_redirect"]
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2015, 2019-2020 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "0.2.0"
+__version__: str = "0.2.1"
 __email__: str = "dominic@davis-foster.co.uk"
 
 
 def create_redirect(redirect_url: str) -> str:
 	"""
 	Generate HTML Redirect File.
```

### Comparing `create_redirect-0.2.0/create_redirect/__main__.py` & `create_redirect-0.2.1/create_redirect/__main__.py`

 * *Files identical despite different names*

### Comparing `create_redirect-0.2.0/create_redirect.egg-info/PKG-INFO` & `create_redirect-0.2.1/create_redirect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: create-redirect
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python script for creating HTML redirects.
 Home-page: https://github.com/domdfcoding/create_redirect
 Author: Dominic Davis-Foster
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: Copyright (c) 2020 Dominic Davis-Foster
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -141,23 +141,23 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/create_redirect
 	:target: https://github.com/domdfcoding/create_redirect/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/create_redirect
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/create_redirect/v0.2.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/create_redirect/v0.2.1
 	:target: https://github.com/domdfcoding/create_redirect/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/create_redirect
 	:target: https://github.com/domdfcoding/create_redirect/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2024
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/create_redirect
 	:target: https://pypi.org/project/create_redirect/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `create_redirect-0.2.0/pyproject.toml` & `create_redirect-0.2.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = [ "setuptools!=61.*,>=40.6.0", "wheel>=0.34.2",]
+requires = [ "setuptools!=61.*,<=67.1.0,>=40.6.0", "wheel>=0.34.2",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "create_redirect"
-version = "0.2.0"
+version = "0.2.1"
 description = "Python script for creating HTML redirects."
 readme = "README.rst"
 requires-python = ">=3.6.1"
 keywords = []
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
@@ -25,22 +25,21 @@
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Text Processing :: Markup :: HTML",
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
 Homepage = "https://github.com/domdfcoding/create_redirect"
 "Issue Tracker" = "https://github.com/domdfcoding/create_redirect/issues"
 "Source Code" = "https://github.com/domdfcoding/create_redirect"
 Documentation = "https://create-redirect.readthedocs.io/en/latest"
 
 [project.scripts]
@@ -66,24 +65,22 @@
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
 ]
-sphinxemoji_style = "twemoji"
 gitstamp_fmt = "%d %b %Y"
 templates_path = [ "_templates",]
 html_static_path = [ "_static",]
 source_suffix = ".rst"
 master_doc = "index"
 suppress_warnings = [ "image.nonlocal_uri",]
 pygments_style = "default"
@@ -152,27 +149,27 @@
 warn_unused_ignores = true
 no_implicit_optional = true
 show_error_codes = true
 
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
 [tool.dependency-dash."requirements.txt"]
 order = 10
 
 [tool.dependency-dash."doc-source/requirements.txt"]
 order = 30
 include = false
 
 [tool.dependency-dash."tests/requirements.txt"]
 order = 20
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

### Comparing `create_redirect-0.2.0/setup.cfg` & `create_redirect-0.2.1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = create_redirect
-version = 0.2.0
+version = 0.2.1
 author = Dominic Davis-Foster
 author_email = dominic@davis-foster.co.uk
 license = MIT License
 keywords = 
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 platforms = Windows, macOS, Linux
```

### Comparing `create_redirect-0.2.0/setup.py` & `create_redirect-0.2.1/setup.py`

 * *Files identical despite different names*

