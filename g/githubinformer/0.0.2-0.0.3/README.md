# Comparing `tmp/githubinformer-0.0.2.tar.gz` & `tmp/githubinformer-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "githubinformer-0.0.2.tar", last modified: Fri May 17 14:29:49 2024, max compression
+gzip compressed data, was "githubinformer-0.0.3.tar", last modified: Mon May 20 13:12:17 2024, max compression
```

## Comparing `githubinformer-0.0.2.tar` & `githubinformer-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 saneksking  (1000) saneksking  (1000)        0 2024-05-17 14:29:49.363489 githubinformer-0.0.2/
--rw-r--r--   0 saneksking  (1000) saneksking  (1000)     1498 2024-05-17 12:12:34.000000 githubinformer-0.0.2/LICENSE
--rw-r--r--   0 saneksking  (1000) saneksking  (1000)       93 2024-05-17 13:55:15.000000 githubinformer-0.0.2/MANIFEST.in
--rw-r--r--   0 saneksking  (1000) saneksking  (1000)     3630 2024-05-17 14:29:49.363489 githubinformer-0.0.2/PKG-INFO
--rw-r--r--   0 saneksking  (1000) saneksking  (1000)     2417 2024-05-17 14:25:29.000000 githubinformer-0.0.2/README.md
-drwxr-xr-x   0 saneksking  (1000) saneksking  (1000)        0 2024-05-17 14:29:49.363489 githubinformer-0.0.2/githubinformer/
--rw-r--r--   0 saneksking  (1000) saneksking  (1000)      366 2024-05-17 14:23:05.000000 githubinformer-0.0.2/githubinformer/__init__.py
--rw-r--r--   0 saneksking  (1000) saneksking  (1000)      862 2024-05-17 14:23:05.000000 githubinformer-0.0.2/githubinformer/github_informer.py
-drwxr-xr-x   0 saneksking  (1000) saneksking  (1000)        0 2024-05-17 14:29:49.363489 githubinformer-0.0.2/githubinformer.egg-info/
--rw-r--r--   0 saneksking  (1000) saneksking  (1000)     3630 2024-05-17 14:29:49.000000 githubinformer-0.0.2/githubinformer.egg-info/PKG-INFO
--rw-r--r--   0 saneksking  (1000) saneksking  (1000)      352 2024-05-17 14:29:49.000000 githubinformer-0.0.2/githubinformer.egg-info/SOURCES.txt
--rw-r--r--   0 saneksking  (1000) saneksking  (1000)        1 2024-05-17 14:29:49.000000 githubinformer-0.0.2/githubinformer.egg-info/dependency_links.txt
--rw-r--r--   0 saneksking  (1000) saneksking  (1000)        1 2024-05-17 14:29:49.000000 githubinformer-0.0.2/githubinformer.egg-info/not-zip-safe
--rw-r--r--   0 saneksking  (1000) saneksking  (1000)       17 2024-05-17 14:29:49.000000 githubinformer-0.0.2/githubinformer.egg-info/requires.txt
--rw-r--r--   0 saneksking  (1000) saneksking  (1000)       15 2024-05-17 14:29:49.000000 githubinformer-0.0.2/githubinformer.egg-info/top_level.txt
--rw-r--r--   0 saneksking  (1000) saneksking  (1000)       17 2024-05-17 13:49:39.000000 githubinformer-0.0.2/requirements.txt
--rw-r--r--   0 saneksking  (1000) saneksking  (1000)     1254 2024-05-17 14:29:49.363489 githubinformer-0.0.2/setup.cfg
--rw-r--r--   0 saneksking  (1000) saneksking  (1000)      347 2024-05-17 13:53:39.000000 githubinformer-0.0.2/setup.py
+drwxr-xr-x   0 saneksking  (1000) saneksking  (1000)        0 2024-05-20 13:12:17.542363 githubinformer-0.0.3/
+-rw-r--r--   0 saneksking  (1000) saneksking  (1000)     1498 2024-05-17 12:12:34.000000 githubinformer-0.0.3/LICENSE
+-rw-r--r--   0 saneksking  (1000) saneksking  (1000)       93 2024-05-17 13:55:15.000000 githubinformer-0.0.3/MANIFEST.in
+-rw-r--r--   0 saneksking  (1000) saneksking  (1000)     3630 2024-05-20 13:12:17.542363 githubinformer-0.0.3/PKG-INFO
+-rw-r--r--   0 saneksking  (1000) saneksking  (1000)     2417 2024-05-20 13:10:44.000000 githubinformer-0.0.3/README.md
+drwxr-xr-x   0 saneksking  (1000) saneksking  (1000)        0 2024-05-20 13:12:17.542363 githubinformer-0.0.3/githubinformer/
+-rw-r--r--   0 saneksking  (1000) saneksking  (1000)      366 2024-05-20 13:10:44.000000 githubinformer-0.0.3/githubinformer/__init__.py
+-rw-r--r--   0 saneksking  (1000) saneksking  (1000)      875 2024-05-20 13:04:07.000000 githubinformer-0.0.3/githubinformer/github_informer.py
+drwxr-xr-x   0 saneksking  (1000) saneksking  (1000)        0 2024-05-20 13:12:17.542363 githubinformer-0.0.3/githubinformer.egg-info/
+-rw-r--r--   0 saneksking  (1000) saneksking  (1000)     3630 2024-05-20 13:12:17.000000 githubinformer-0.0.3/githubinformer.egg-info/PKG-INFO
+-rw-r--r--   0 saneksking  (1000) saneksking  (1000)      352 2024-05-20 13:12:17.000000 githubinformer-0.0.3/githubinformer.egg-info/SOURCES.txt
+-rw-r--r--   0 saneksking  (1000) saneksking  (1000)        1 2024-05-20 13:12:17.000000 githubinformer-0.0.3/githubinformer.egg-info/dependency_links.txt
+-rw-r--r--   0 saneksking  (1000) saneksking  (1000)        1 2024-05-20 13:12:17.000000 githubinformer-0.0.3/githubinformer.egg-info/not-zip-safe
+-rw-r--r--   0 saneksking  (1000) saneksking  (1000)       17 2024-05-20 13:12:17.000000 githubinformer-0.0.3/githubinformer.egg-info/requires.txt
+-rw-r--r--   0 saneksking  (1000) saneksking  (1000)       15 2024-05-20 13:12:17.000000 githubinformer-0.0.3/githubinformer.egg-info/top_level.txt
+-rw-r--r--   0 saneksking  (1000) saneksking  (1000)       17 2024-05-17 13:49:39.000000 githubinformer-0.0.3/requirements.txt
+-rw-r--r--   0 saneksking  (1000) saneksking  (1000)     1254 2024-05-20 13:12:17.542363 githubinformer-0.0.3/setup.cfg
+-rw-r--r--   0 saneksking  (1000) saneksking  (1000)      347 2024-05-17 13:53:39.000000 githubinformer-0.0.3/setup.py
```

### Comparing `githubinformer-0.0.2/LICENSE` & `githubinformer-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `githubinformer-0.0.2/PKG-INFO` & `githubinformer-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: githubinformer
-Version: 0.0.2
+Version: 0.0.3
 Summary: 'A library to get data of open users repositories GitHub.'
 Home-page: https://github.com/saneksking
 Author: A.A Suvorov
 Author-email: smartlegiondev@gmail.com
 License: BSD 3-Clause License
 Project-URL: Documentation, https://github.com/saneksking/githubinformer/blob/master/README.md
 Project-URL: Release notes, https://github.com/saneksking/githubinformer/releases
@@ -22,15 +22,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.31.0
 
-# GitHub Informer <sup>v 0.0.2</sup>
+# GitHub Informer <sup>v 0.0.3</sup>
 
 ***
 
 [![GitHub release (latest by date)](https://img.shields.io/github/v/release/saneksking/githubinformer)](https://github.com/saneksking/githubinformer/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/githubinformer?label=pypi%20downloads)](https://pypi.org/project/githubinformer/)
 ![GitHub top language](https://img.shields.io/github/languages/top/saneksking/githubinformer)
 [![PyPI](https://img.shields.io/pypi/v/githubinformer)](https://pypi.org/project/githubinformer)
```

### Comparing `githubinformer-0.0.2/README.md` & `githubinformer-0.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# GitHub Informer <sup>v 0.0.2</sup>
+# GitHub Informer <sup>v 0.0.3</sup>
 
 ***
 
 [![GitHub release (latest by date)](https://img.shields.io/github/v/release/saneksking/githubinformer)](https://github.com/saneksking/githubinformer/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/githubinformer?label=pypi%20downloads)](https://pypi.org/project/githubinformer/)
 ![GitHub top language](https://img.shields.io/github/languages/top/saneksking/githubinformer)
 [![PyPI](https://img.shields.io/pypi/v/githubinformer)](https://pypi.org/project/githubinformer)
```

### Comparing `githubinformer-0.0.2/githubinformer/github_informer.py` & `githubinformer-0.0.3/githubinformer/github_informer.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,14 @@
             github_data = response.json()
             return github_data
         else:
             return []
 
     @property
     def api_url(self):
-        return f'https://api.github.com/users/{self._user}/repos'
+        return f'https://api.github.com/users/{self._user}/repos?per_page=100'
 
     def get_all_info(self):
         return self._data
 
     def get_repositories_count(self):
         return len(self._data)
```

### Comparing `githubinformer-0.0.2/githubinformer.egg-info/PKG-INFO` & `githubinformer-0.0.3/githubinformer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: githubinformer
-Version: 0.0.2
+Version: 0.0.3
 Summary: 'A library to get data of open users repositories GitHub.'
 Home-page: https://github.com/saneksking
 Author: A.A Suvorov
 Author-email: smartlegiondev@gmail.com
 License: BSD 3-Clause License
 Project-URL: Documentation, https://github.com/saneksking/githubinformer/blob/master/README.md
 Project-URL: Release notes, https://github.com/saneksking/githubinformer/releases
@@ -22,15 +22,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.31.0
 
-# GitHub Informer <sup>v 0.0.2</sup>
+# GitHub Informer <sup>v 0.0.3</sup>
 
 ***
 
 [![GitHub release (latest by date)](https://img.shields.io/github/v/release/saneksking/githubinformer)](https://github.com/saneksking/githubinformer/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/githubinformer?label=pypi%20downloads)](https://pypi.org/project/githubinformer/)
 ![GitHub top language](https://img.shields.io/github/languages/top/saneksking/githubinformer)
 [![PyPI](https://img.shields.io/pypi/v/githubinformer)](https://pypi.org/project/githubinformer)
```

### Comparing `githubinformer-0.0.2/setup.cfg` & `githubinformer-0.0.3/setup.cfg`

 * *Files identical despite different names*

