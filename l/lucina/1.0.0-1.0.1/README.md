# Comparing `tmp/lucina-1.0.0.tar.gz` & `tmp/lucina-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lucina-1.0.0.tar", last modified: Sun Feb  5 18:52:38 2023, max compression
+gzip compressed data, was "lucina-1.0.1.tar", last modified: Mon May 20 16:13:03 2024, max compression
```

## Comparing `lucina-1.0.0.tar` & `lucina-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,24 @@
-drwxr-xr-x   0 rozo_a    (1000) users      (100)        0 2023-02-05 18:52:38.950037 lucina-1.0.0/
--rw-r--r--   0 rozo_a    (1000) users      (100)     1507 2023-02-05 18:52:38.950037 lucina-1.0.0/PKG-INFO
--rw-r--r--   0 rozo_a    (1000) users      (100)     1085 2023-02-05 18:52:24.000000 lucina-1.0.0/README.md
-drwxr-xr-x   0 rozo_a    (1000) users      (100)        0 2023-02-05 18:52:38.946704 lucina-1.0.0/lucina/
--rw-r--r--   0 rozo_a    (1000) users      (100)      430 2023-02-05 12:03:11.000000 lucina-1.0.0/lucina/__init__.py
--rw-r--r--   0 rozo_a    (1000) users      (100)     1221 2023-02-05 12:03:11.000000 lucina-1.0.0/lucina/__main__.py
--rw-r--r--   0 rozo_a    (1000) users      (100)      157 2023-02-05 18:52:24.000000 lucina-1.0.0/lucina/_about.py
--rw-r--r--   0 rozo_a    (1000) users      (100)      686 2023-02-05 10:30:37.000000 lucina-1.0.0/lucina/cell.py
--rw-r--r--   0 rozo_a    (1000) users      (100)     1547 2023-02-05 10:30:37.000000 lucina-1.0.0/lucina/format.py
--rw-r--r--   0 rozo_a    (1000) users      (100)     2489 2023-02-05 12:03:11.000000 lucina-1.0.0/lucina/parser.py
--rw-r--r--   0 rozo_a    (1000) users      (100)      112 2023-02-05 12:03:11.000000 lucina-1.0.0/lucina/utils.py
-drwxr-xr-x   0 rozo_a    (1000) users      (100)        0 2023-02-05 18:52:38.950037 lucina-1.0.0/lucina.egg-info/
--rw-r--r--   0 rozo_a    (1000) users      (100)     1507 2023-02-05 18:52:38.000000 lucina-1.0.0/lucina.egg-info/PKG-INFO
--rw-r--r--   0 rozo_a    (1000) users      (100)      330 2023-02-05 18:52:38.000000 lucina-1.0.0/lucina.egg-info/SOURCES.txt
--rw-r--r--   0 rozo_a    (1000) users      (100)        1 2023-02-05 18:52:38.000000 lucina-1.0.0/lucina.egg-info/dependency_links.txt
--rw-r--r--   0 rozo_a    (1000) users      (100)       48 2023-02-05 18:52:38.000000 lucina-1.0.0/lucina.egg-info/entry_points.txt
--rw-r--r--   0 rozo_a    (1000) users      (100)       51 2023-02-05 18:52:38.000000 lucina-1.0.0/lucina.egg-info/requires.txt
--rw-r--r--   0 rozo_a    (1000) users      (100)        7 2023-02-05 18:52:38.000000 lucina-1.0.0/lucina.egg-info/top_level.txt
--rw-r--r--   0 rozo_a    (1000) users      (100)      306 2023-02-05 18:52:38.950037 lucina-1.0.0/setup.cfg
--rw-r--r--   0 rozo_a    (1000) users      (100)     1063 2023-02-05 18:52:24.000000 lucina-1.0.0/setup.py
+drwxr-xr-x   0 rozo_a    (1000) users      (100)        0 2024-05-20 16:13:03.593898 lucina-1.0.1/
+-rw-r--r--   0 rozo_a    (1000) users      (100)     1730 2024-05-20 16:13:03.593898 lucina-1.0.1/PKG-INFO
+-rw-r--r--   0 rozo_a    (1000) users      (100)     1111 2024-05-20 16:11:52.000000 lucina-1.0.1/README.md
+drwxr-xr-x   0 rozo_a    (1000) users      (100)        0 2024-05-20 16:13:03.590565 lucina-1.0.1/lucina/
+-rw-r--r--   0 rozo_a    (1000) users      (100)      161 2024-05-20 16:11:52.000000 lucina-1.0.1/lucina/__init__.py
+-rw-r--r--   0 rozo_a    (1000) users      (100)     1221 2023-02-05 12:03:11.000000 lucina-1.0.1/lucina/__main__.py
+-rw-r--r--   0 rozo_a    (1000) users      (100)      686 2023-02-05 10:30:37.000000 lucina-1.0.1/lucina/cell.py
+-rw-r--r--   0 rozo_a    (1000) users      (100)     1547 2023-02-05 10:30:37.000000 lucina-1.0.1/lucina/format.py
+-rw-r--r--   0 rozo_a    (1000) users      (100)     2489 2023-02-05 12:03:11.000000 lucina-1.0.1/lucina/parser.py
+-rw-r--r--   0 rozo_a    (1000) users      (100)      112 2023-02-05 12:03:11.000000 lucina-1.0.1/lucina/utils.py
+drwxr-xr-x   0 rozo_a    (1000) users      (100)        0 2024-05-20 16:13:03.593898 lucina-1.0.1/lucina.egg-info/
+-rw-r--r--   0 rozo_a    (1000) users      (100)     1730 2024-05-20 16:13:03.000000 lucina-1.0.1/lucina.egg-info/PKG-INFO
+-rw-r--r--   0 rozo_a    (1000) users      (100)      390 2024-05-20 16:13:03.000000 lucina-1.0.1/lucina.egg-info/SOURCES.txt
+-rw-r--r--   0 rozo_a    (1000) users      (100)        1 2024-05-20 16:13:03.000000 lucina-1.0.1/lucina.egg-info/dependency_links.txt
+-rw-r--r--   0 rozo_a    (1000) users      (100)       48 2024-05-20 16:13:03.000000 lucina-1.0.1/lucina.egg-info/entry_points.txt
+-rw-r--r--   0 rozo_a    (1000) users      (100)       51 2024-05-20 16:13:03.000000 lucina-1.0.1/lucina.egg-info/requires.txt
+-rw-r--r--   0 rozo_a    (1000) users      (100)        7 2024-05-20 16:13:03.000000 lucina-1.0.1/lucina.egg-info/top_level.txt
+-rw-r--r--   0 rozo_a    (1000) users      (100)     1036 2024-05-20 16:11:52.000000 lucina-1.0.1/pyproject.toml
+-rw-r--r--   0 rozo_a    (1000) users      (100)       38 2024-05-20 16:13:03.593898 lucina-1.0.1/setup.cfg
+drwxr-xr-x   0 rozo_a    (1000) users      (100)        0 2024-05-20 16:13:03.593898 lucina-1.0.1/tests/
+-rw-r--r--   0 rozo_a    (1000) users      (100)      698 2023-02-05 10:30:37.000000 lucina-1.0.1/tests/test_cell.py
+-rw-r--r--   0 rozo_a    (1000) users      (100)     2047 2023-02-05 10:30:37.000000 lucina-1.0.1/tests/test_format.py
+-rw-r--r--   0 rozo_a    (1000) users      (100)     9521 2023-02-05 12:03:11.000000 lucina-1.0.1/tests/test_parser.py
+-rw-r--r--   0 rozo_a    (1000) users      (100)      288 2023-02-05 12:03:11.000000 lucina-1.0.1/tests/test_utils.py
```

### Comparing `lucina-1.0.0/PKG-INFO` & `lucina-1.0.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: lucina
-Version: 1.0.0
+Version: 1.0.1
 Summary: From markdown to Jupyter notebook
-Home-page: https://github.com/entwanne/lucina
-Author: entwanne
-Author-email: antoine.rozo@gmail.com
-License: MIT
+Author-email: entwanne <antoine.rozo@gmail.com>
+License: MIT License
+Project-URL: homepage, https://github.com/entwanne/lucina
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
+Requires-Dist: minimd==1.*
 Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-mock; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: isort; extra == "dev"
 
 Lucina
 ======
 
 From markdown to Jupyter notebook.
 
 https://pypi.org/project/lucina/
@@ -31,15 +35,15 @@
 
 ```shell
 lucina -o docs/output.ipynb docs/input.md
 ```
 
 It outputs file [output.ipynb](docs/output.ipynb) that looks like:
 
-![Screenshot](https://github.com/entwanne/lucina/tree/master/docs/screen.png)
+![Screenshot](https://raw.githubusercontent.com/entwanne/lucina/master/docs/screen.png)
 
 ## Development
 
 ### Environment
 
 Use `pip install -e '.[dev]'` to install `lucina` with development dependencies (tests & lint).
 
@@ -47,10 +51,10 @@
 
 Code of the project is managed on <https://github.com/entwanne/lucina/> git repository.
 
 ### Building & deploying a new version
 
 You need to install `twine` package (`pip install twine`) to be able to deploy a version of the library.
 
-You can use `python setup.py sdist` to build the current version of the package.
+You can use `python -m build` (`pip install build`) to build the current version of the package.
 
 Then you can deploy this version to PyPI by running `twine upload dist/*`.
```

### Comparing `lucina-1.0.0/README.md` & `lucina-1.0.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 ```shell
 lucina -o docs/output.ipynb docs/input.md
 ```
 
 It outputs file [output.ipynb](docs/output.ipynb) that looks like:
 
-![Screenshot](https://github.com/entwanne/lucina/tree/master/docs/screen.png)
+![Screenshot](https://raw.githubusercontent.com/entwanne/lucina/master/docs/screen.png)
 
 ## Development
 
 ### Environment
 
 Use `pip install -e '.[dev]'` to install `lucina` with development dependencies (tests & lint).
 
@@ -33,10 +33,10 @@
 
 Code of the project is managed on <https://github.com/entwanne/lucina/> git repository.
 
 ### Building & deploying a new version
 
 You need to install `twine` package (`pip install twine`) to be able to deploy a version of the library.
 
-You can use `python setup.py sdist` to build the current version of the package.
+You can use `python -m build` (`pip install build`) to build the current version of the package.
 
 Then you can deploy this version to PyPI by running `twine upload dist/*`.
```

### Comparing `lucina-1.0.0/lucina/__main__.py` & `lucina-1.0.1/lucina/__main__.py`

 * *Files identical despite different names*

### Comparing `lucina-1.0.0/lucina/cell.py` & `lucina-1.0.1/lucina/cell.py`

 * *Files identical despite different names*

### Comparing `lucina-1.0.0/lucina/format.py` & `lucina-1.0.1/lucina/format.py`

 * *Files identical despite different names*

### Comparing `lucina-1.0.0/lucina/parser.py` & `lucina-1.0.1/lucina/parser.py`

 * *Files identical despite different names*

### Comparing `lucina-1.0.0/lucina.egg-info/PKG-INFO` & `lucina-1.0.1/lucina.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: lucina
-Version: 1.0.0
+Version: 1.0.1
 Summary: From markdown to Jupyter notebook
-Home-page: https://github.com/entwanne/lucina
-Author: entwanne
-Author-email: antoine.rozo@gmail.com
-License: MIT
+Author-email: entwanne <antoine.rozo@gmail.com>
+License: MIT License
+Project-URL: homepage, https://github.com/entwanne/lucina
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
+Requires-Dist: minimd==1.*
 Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-mock; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: isort; extra == "dev"
 
 Lucina
 ======
 
 From markdown to Jupyter notebook.
 
 https://pypi.org/project/lucina/
@@ -31,15 +35,15 @@
 
 ```shell
 lucina -o docs/output.ipynb docs/input.md
 ```
 
 It outputs file [output.ipynb](docs/output.ipynb) that looks like:
 
-![Screenshot](https://github.com/entwanne/lucina/tree/master/docs/screen.png)
+![Screenshot](https://raw.githubusercontent.com/entwanne/lucina/master/docs/screen.png)
 
 ## Development
 
 ### Environment
 
 Use `pip install -e '.[dev]'` to install `lucina` with development dependencies (tests & lint).
 
@@ -47,10 +51,10 @@
 
 Code of the project is managed on <https://github.com/entwanne/lucina/> git repository.
 
 ### Building & deploying a new version
 
 You need to install `twine` package (`pip install twine`) to be able to deploy a version of the library.
 
-You can use `python setup.py sdist` to build the current version of the package.
+You can use `python -m build` (`pip install build`) to build the current version of the package.
 
 Then you can deploy this version to PyPI by running `twine upload dist/*`.
```

