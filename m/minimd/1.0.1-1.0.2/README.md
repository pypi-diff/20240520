# Comparing `tmp/minimd-1.0.1.tar.gz` & `tmp/minimd-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minimd-1.0.1.tar", last modified: Sun Feb  5 18:35:57 2023, max compression
+gzip compressed data, was "minimd-1.0.2.tar", last modified: Mon May 20 15:49:23 2024, max compression
```

## Comparing `minimd-1.0.1.tar` & `minimd-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 rozo_a    (1000) users      (100)        0 2023-02-05 18:35:57.214704 minimd-1.0.1/
--rw-r--r--   0 rozo_a    (1000) users      (100)     3197 2023-02-05 18:35:57.214704 minimd-1.0.1/PKG-INFO
--rw-r--r--   0 rozo_a    (1000) users      (100)     2785 2023-02-05 18:35:25.000000 minimd-1.0.1/README.md
-drwxr-xr-x   0 rozo_a    (1000) users      (100)        0 2023-02-05 18:35:57.214704 minimd-1.0.1/minimd/
--rw-r--r--   0 rozo_a    (1000) users      (100)      383 2023-02-05 18:25:35.000000 minimd-1.0.1/minimd/__init__.py
--rw-r--r--   0 rozo_a    (1000) users      (100)      428 2023-02-05 10:59:24.000000 minimd-1.0.1/minimd/__main__.py
--rw-r--r--   0 rozo_a    (1000) users      (100)      157 2023-02-05 18:35:25.000000 minimd-1.0.1/minimd/_about.py
--rw-r--r--   0 rozo_a    (1000) users      (100)     2218 2023-02-05 10:59:24.000000 minimd-1.0.1/minimd/tokenizer.py
--rw-r--r--   0 rozo_a    (1000) users      (100)      297 2023-02-05 10:59:24.000000 minimd-1.0.1/minimd/utils.py
-drwxr-xr-x   0 rozo_a    (1000) users      (100)        0 2023-02-05 18:35:57.214704 minimd-1.0.1/minimd.egg-info/
--rw-r--r--   0 rozo_a    (1000) users      (100)     3197 2023-02-05 18:35:57.000000 minimd-1.0.1/minimd.egg-info/PKG-INFO
--rw-r--r--   0 rozo_a    (1000) users      (100)      301 2023-02-05 18:35:57.000000 minimd-1.0.1/minimd.egg-info/SOURCES.txt
--rw-r--r--   0 rozo_a    (1000) users      (100)        1 2023-02-05 18:35:57.000000 minimd-1.0.1/minimd.egg-info/dependency_links.txt
--rw-r--r--   0 rozo_a    (1000) users      (100)       48 2023-02-05 18:35:57.000000 minimd-1.0.1/minimd.egg-info/entry_points.txt
--rw-r--r--   0 rozo_a    (1000) users      (100)       39 2023-02-05 18:35:57.000000 minimd-1.0.1/minimd.egg-info/requires.txt
--rw-r--r--   0 rozo_a    (1000) users      (100)        7 2023-02-05 18:35:57.000000 minimd-1.0.1/minimd.egg-info/top_level.txt
--rw-r--r--   0 rozo_a    (1000) users      (100)      306 2023-02-05 18:35:57.214704 minimd-1.0.1/setup.cfg
--rw-r--r--   0 rozo_a    (1000) users      (100)     1025 2023-02-05 18:25:35.000000 minimd-1.0.1/setup.py
+drwxr-xr-x   0 rozo_a    (1000) users      (100)        0 2024-05-20 15:49:23.339982 minimd-1.0.2/
+-rw-r--r--   0 rozo_a    (1000) users      (100)     3383 2024-05-20 15:49:23.339982 minimd-1.0.2/PKG-INFO
+-rw-r--r--   0 rozo_a    (1000) users      (100)     2801 2024-05-20 15:48:29.000000 minimd-1.0.2/README.md
+drwxr-xr-x   0 rozo_a    (1000) users      (100)        0 2024-05-20 15:49:23.336649 minimd-1.0.2/minimd/
+-rw-r--r--   0 rozo_a    (1000) users      (100)      142 2024-05-20 15:48:29.000000 minimd-1.0.2/minimd/__init__.py
+-rw-r--r--   0 rozo_a    (1000) users      (100)      428 2023-02-05 10:59:24.000000 minimd-1.0.2/minimd/__main__.py
+-rw-r--r--   0 rozo_a    (1000) users      (100)     2218 2023-02-05 10:59:24.000000 minimd-1.0.2/minimd/tokenizer.py
+-rw-r--r--   0 rozo_a    (1000) users      (100)      297 2023-02-05 10:59:24.000000 minimd-1.0.2/minimd/utils.py
+drwxr-xr-x   0 rozo_a    (1000) users      (100)        0 2024-05-20 15:49:23.336649 minimd-1.0.2/minimd.egg-info/
+-rw-r--r--   0 rozo_a    (1000) users      (100)     3383 2024-05-20 15:49:23.000000 minimd-1.0.2/minimd.egg-info/PKG-INFO
+-rw-r--r--   0 rozo_a    (1000) users      (100)      324 2024-05-20 15:49:23.000000 minimd-1.0.2/minimd.egg-info/SOURCES.txt
+-rw-r--r--   0 rozo_a    (1000) users      (100)        1 2024-05-20 15:49:23.000000 minimd-1.0.2/minimd.egg-info/dependency_links.txt
+-rw-r--r--   0 rozo_a    (1000) users      (100)       48 2024-05-20 15:49:23.000000 minimd-1.0.2/minimd.egg-info/entry_points.txt
+-rw-r--r--   0 rozo_a    (1000) users      (100)       39 2024-05-20 15:49:23.000000 minimd-1.0.2/minimd.egg-info/requires.txt
+-rw-r--r--   0 rozo_a    (1000) users      (100)        7 2024-05-20 15:49:23.000000 minimd-1.0.2/minimd.egg-info/top_level.txt
+-rw-r--r--   0 rozo_a    (1000) users      (100)      988 2024-05-20 15:48:29.000000 minimd-1.0.2/pyproject.toml
+-rw-r--r--   0 rozo_a    (1000) users      (100)       38 2024-05-20 15:49:23.339982 minimd-1.0.2/setup.cfg
+drwxr-xr-x   0 rozo_a    (1000) users      (100)        0 2024-05-20 15:49:23.336649 minimd-1.0.2/tests/
+-rw-r--r--   0 rozo_a    (1000) users      (100)     3092 2023-02-05 10:59:24.000000 minimd-1.0.2/tests/test_tokenizer.py
+-rw-r--r--   0 rozo_a    (1000) users      (100)      718 2023-02-05 11:56:05.000000 minimd-1.0.2/tests/test_utils.py
```

### Comparing `minimd-1.0.1/PKG-INFO` & `minimd-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: minimd
-Version: 1.0.1
+Version: 1.0.2
 Summary: Minimal markdown parser
-Home-page: https://github.com/entwanne/minimd
-Author: entwanne
-Author-email: antoine.rozo@gmail.com
-License: MIT
+Author-email: entwanne <antoine.rozo@gmail.com>
+License: MIT License
+Project-URL: homepage, https://github.com/entwanne/minimd
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-mock; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: isort; extra == "dev"
 
 Minimd
 ======
 
 Minimal markdown parser.
 
 https://pypi.org/project/minimd/
@@ -114,10 +117,10 @@
 
 Code of the project is managed on <https://github.com/entwanne/minimd/> git repository.
 
 ### Building & deploying a new version
 
 You need to install `twine` package (`pip install twine`) to be able to deploy a version of the library.
 
-You can use `python setup.py sdist` to build the current version of the package.
+You can use `python -m build` (`pip install build`) to build the current version of the package.
 
 Then you can deploy this version to PyPI by running `twine upload dist/*`.
```

### Comparing `minimd-1.0.1/README.md` & `minimd-1.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -100,10 +100,10 @@
 
 Code of the project is managed on <https://github.com/entwanne/minimd/> git repository.
 
 ### Building & deploying a new version
 
 You need to install `twine` package (`pip install twine`) to be able to deploy a version of the library.
 
-You can use `python setup.py sdist` to build the current version of the package.
+You can use `python -m build` (`pip install build`) to build the current version of the package.
 
 Then you can deploy this version to PyPI by running `twine upload dist/*`.
```

### Comparing `minimd-1.0.1/minimd/tokenizer.py` & `minimd-1.0.2/minimd/tokenizer.py`

 * *Files identical despite different names*

### Comparing `minimd-1.0.1/minimd.egg-info/PKG-INFO` & `minimd-1.0.2/minimd.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: minimd
-Version: 1.0.1
+Version: 1.0.2
 Summary: Minimal markdown parser
-Home-page: https://github.com/entwanne/minimd
-Author: entwanne
-Author-email: antoine.rozo@gmail.com
-License: MIT
+Author-email: entwanne <antoine.rozo@gmail.com>
+License: MIT License
+Project-URL: homepage, https://github.com/entwanne/minimd
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-mock; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: isort; extra == "dev"
 
 Minimd
 ======
 
 Minimal markdown parser.
 
 https://pypi.org/project/minimd/
@@ -114,10 +117,10 @@
 
 Code of the project is managed on <https://github.com/entwanne/minimd/> git repository.
 
 ### Building & deploying a new version
 
 You need to install `twine` package (`pip install twine`) to be able to deploy a version of the library.
 
-You can use `python setup.py sdist` to build the current version of the package.
+You can use `python -m build` (`pip install build`) to build the current version of the package.
 
 Then you can deploy this version to PyPI by running `twine upload dist/*`.
```

