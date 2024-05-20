# Comparing `tmp/vizbeauty-0.0.1.tar.gz` & `tmp/vizbeauty-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vizbeauty-0.0.1.tar", last modified: Mon May 20 13:31:37 2024, max compression
+gzip compressed data, was "vizbeauty-0.0.2.tar", last modified: Mon May 20 13:54:38 2024, max compression
```

## Comparing `vizbeauty-0.0.1.tar` & `vizbeauty-0.0.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:31:37.423210 vizbeauty-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:31:37.415209 vizbeauty-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:31:37.415209 vizbeauty-0.0.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:31:37.419209 vizbeauty-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-20 13:31:37.423210 vizbeauty-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:31:37.419209 vizbeauty-0.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:31:37.419209 vizbeauty-0.0.1/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:31:37.419209 vizbeauty-0.0.1/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/docs/vizbeauty.md
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 13:31:37.423210 vizbeauty-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:31:37.419209 vizbeauty-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/tests/test_vizbeauty.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:31:37.419209 vizbeauty-0.0.1/vizbeauty/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/vizbeauty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/vizbeauty/common.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/vizbeauty/vizbeauty.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:31:37.419209 vizbeauty-0.0.1/vizbeauty.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-20 13:31:37.000000 vizbeauty-0.0.1/vizbeauty.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-20 13:31:37.000000 vizbeauty-0.0.1/vizbeauty.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 13:31:37.000000 vizbeauty-0.0.1/vizbeauty.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-20 13:31:37.000000 vizbeauty-0.0.1/vizbeauty.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-20 13:31:37.000000 vizbeauty-0.0.1/vizbeauty.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 13:31:37.000000 vizbeauty-0.0.1/vizbeauty.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:54:38.934539 vizbeauty-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-20 13:54:24.000000 vizbeauty-0.0.2/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:54:38.926539 vizbeauty-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:54:38.930539 vizbeauty-0.0.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-20 13:54:24.000000 vizbeauty-0.0.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-20 13:54:24.000000 vizbeauty-0.0.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-20 13:54:24.000000 vizbeauty-0.0.2/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:54:38.930539 vizbeauty-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-20 13:54:24.000000 vizbeauty-0.0.2/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-20 13:54:24.000000 vizbeauty-0.0.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-20 13:54:24.000000 vizbeauty-0.0.2/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-20 13:54:24.000000 vizbeauty-0.0.2/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-20 13:54:24.000000 vizbeauty-0.0.2/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-20 13:54:24.000000 vizbeauty-0.0.2/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-20 13:54:24.000000 vizbeauty-0.0.2/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-20 13:54:24.000000 vizbeauty-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-20 13:54:24.000000 vizbeauty-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-20 13:54:24.000000 vizbeauty-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-20 13:54:38.934539 vizbeauty-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-20 13:54:24.000000 vizbeauty-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:54:38.930539 vizbeauty-0.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-20 13:54:24.000000 vizbeauty-0.0.2/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-20 13:54:24.000000 vizbeauty-0.0.2/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-05-20 13:54:24.000000 vizbeauty-0.0.2/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:54:38.934539 vizbeauty-0.0.2/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-20 13:54:24.000000 vizbeauty-0.0.2/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-20 13:54:24.000000 vizbeauty-0.0.2/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-20 13:54:24.000000 vizbeauty-0.0.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-20 13:54:24.000000 vizbeauty-0.0.2/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:54:38.934539 vizbeauty-0.0.2/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-20 13:54:24.000000 vizbeauty-0.0.2/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-20 13:54:24.000000 vizbeauty-0.0.2/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-20 13:54:24.000000 vizbeauty-0.0.2/docs/vizbeauty.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-20 13:54:24.000000 vizbeauty-0.0.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-20 13:54:24.000000 vizbeauty-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-20 13:54:24.000000 vizbeauty-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-20 13:54:24.000000 vizbeauty-0.0.2/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 13:54:38.934539 vizbeauty-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:54:38.934539 vizbeauty-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-20 13:54:24.000000 vizbeauty-0.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-20 13:54:24.000000 vizbeauty-0.0.2/tests/test_vizbeauty.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:54:38.934539 vizbeauty-0.0.2/vizbeauty/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-20 13:54:24.000000 vizbeauty-0.0.2/vizbeauty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5001 2024-05-20 13:54:24.000000 vizbeauty-0.0.2/vizbeauty/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-20 13:54:24.000000 vizbeauty-0.0.2/vizbeauty/vizbeauty.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:54:38.934539 vizbeauty-0.0.2/vizbeauty.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-20 13:54:38.000000 vizbeauty-0.0.2/vizbeauty.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-20 13:54:38.000000 vizbeauty-0.0.2/vizbeauty.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 13:54:38.000000 vizbeauty-0.0.2/vizbeauty.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-20 13:54:38.000000 vizbeauty-0.0.2/vizbeauty.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-20 13:54:38.000000 vizbeauty-0.0.2/vizbeauty.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 13:54:38.000000 vizbeauty-0.0.2/vizbeauty.egg-info/top_level.txt
```

### Comparing `vizbeauty-0.0.1/.github/workflows/docs-build.yml` & `vizbeauty-0.0.2/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `vizbeauty-0.0.1/.github/workflows/docs.yml` & `vizbeauty-0.0.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `vizbeauty-0.0.1/.github/workflows/installation.yml` & `vizbeauty-0.0.2/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `vizbeauty-0.0.1/.github/workflows/macos.yml` & `vizbeauty-0.0.2/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `vizbeauty-0.0.1/.github/workflows/pypi.yml` & `vizbeauty-0.0.2/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `vizbeauty-0.0.1/.github/workflows/ubuntu.yml` & `vizbeauty-0.0.2/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `vizbeauty-0.0.1/.github/workflows/windows.yml` & `vizbeauty-0.0.2/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `vizbeauty-0.0.1/.gitignore` & `vizbeauty-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `vizbeauty-0.0.1/LICENSE` & `vizbeauty-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vizbeauty-0.0.1/PKG-INFO` & `vizbeauty-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vizbeauty
-Version: 0.0.1
+Version: 0.0.2
 Summary: VizBeauty is a Python package for beautiful and insightful visualizations, including descriptive statistics, bar plots, regression scatter plots, and hyperparameter tuning visualizations for machine learning models.
 Author-email: Cristian Del Gobbo <cristiandelgobbo87@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/cris1618/vizbeauty
 Keywords: vizbeauty
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `vizbeauty-0.0.1/README.md` & `vizbeauty-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `vizbeauty-0.0.1/docs/contributing.md` & `vizbeauty-0.0.2/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `vizbeauty-0.0.1/docs/installation.md` & `vizbeauty-0.0.2/docs/installation.md`

 * *Files identical despite different names*

### Comparing `vizbeauty-0.0.1/mkdocs.yml` & `vizbeauty-0.0.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `vizbeauty-0.0.1/pyproject.toml` & `vizbeauty-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "vizbeauty"
-version = "0.0.1"
+version = "0.0.2"
 dynamic = [
     "dependencies",
 ]
 description = "VizBeauty is a Python package for beautiful and insightful visualizations, including descriptive statistics, bar plots, regression scatter plots, and hyperparameter tuning visualizations for machine learning models."
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -48,15 +48,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.0.1"
+current_version = "0.0.2"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

### Comparing `vizbeauty-0.0.1/vizbeauty.egg-info/PKG-INFO` & `vizbeauty-0.0.2/vizbeauty.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vizbeauty
-Version: 0.0.1
+Version: 0.0.2
 Summary: VizBeauty is a Python package for beautiful and insightful visualizations, including descriptive statistics, bar plots, regression scatter plots, and hyperparameter tuning visualizations for machine learning models.
 Author-email: Cristian Del Gobbo <cristiandelgobbo87@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/cris1618/vizbeauty
 Keywords: vizbeauty
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `vizbeauty-0.0.1/vizbeauty.egg-info/SOURCES.txt` & `vizbeauty-0.0.2/vizbeauty.egg-info/SOURCES.txt`

 * *Files identical despite different names*

