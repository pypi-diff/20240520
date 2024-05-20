# Comparing `tmp/matprops-1.0.3.tar.gz` & `tmp/matprops-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matprops-1.0.3.tar", last modified: Thu Jul 14 19:54:42 2022, max compression
+gzip compressed data, was "matprops-1.0.4.tar", last modified: Mon May 20 00:16:09 2024, max compression
```

## Comparing `matprops-1.0.3.tar` & `matprops-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 19:54:42.951426 matprops-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-07-14 19:54:33.000000 matprops-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2942 2022-07-14 19:54:42.947426 matprops-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2244 2022-07-14 19:54:33.000000 matprops-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-14 19:54:42.951426 matprops-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1196 2022-07-14 19:54:33.000000 matprops-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 19:54:42.947426 matprops-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 19:54:42.947426 matprops-1.0.3/src/matprops/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 19:54:33.000000 matprops-1.0.3/src/matprops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8718 2022-07-14 19:54:33.000000 matprops-1.0.3/src/matprops/props.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 19:54:42.947426 matprops-1.0.3/src/matprops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2942 2022-07-14 19:54:42.000000 matprops-1.0.3/src/matprops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      252 2022-07-14 19:54:42.000000 matprops-1.0.3/src/matprops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-14 19:54:42.000000 matprops-1.0.3/src/matprops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-07-14 19:54:42.000000 matprops-1.0.3/src/matprops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-07-14 19:54:42.000000 matprops-1.0.3/src/matprops.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:16:09.673164 matprops-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-20 00:15:49.000000 matprops-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-20 00:16:09.673164 matprops-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-20 00:15:49.000000 matprops-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 00:16:09.673164 matprops-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-20 00:15:49.000000 matprops-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:16:09.669163 matprops-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:16:09.673164 matprops-1.0.4/src/matprops/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 00:15:49.000000 matprops-1.0.4/src/matprops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-05-20 00:15:49.000000 matprops-1.0.4/src/matprops/props.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:16:09.673164 matprops-1.0.4/src/matprops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-20 00:16:09.000000 matprops-1.0.4/src/matprops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-20 00:16:09.000000 matprops-1.0.4/src/matprops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 00:16:09.000000 matprops-1.0.4/src/matprops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-20 00:16:09.000000 matprops-1.0.4/src/matprops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-20 00:16:09.000000 matprops-1.0.4/src/matprops.egg-info/top_level.txt
```

### Comparing `matprops-1.0.3/LICENSE` & `matprops-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `matprops-1.0.3/PKG-INFO` & `matprops-1.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: matprops
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python library written on top of matplotlib library for customizable proportional charts
 Home-page: https://github.com/shammeer-s/matprops
 Author: Mohammed Shammeer
 Author-email: mohammedshammeer.s@gmail.com
 Keywords: matplotlib,visualization,proportional charts
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: numpy>=1.22.0
+Requires-Dist: pandas>=1.3.5
+Requires-Dist: matplotlib>=3.5.1
+Provides-Extra: dev
+Requires-Dist: pytest>=6.2.5; extra == "dev"
 
 # Matprops
 **matprops** is a Python library for visualizing proportional data. It is build above matplotlib (the visualization library). Understanding proportional data is quite easy but when it comes to bigger picture we lack of seeing everything 
 
 ## Installation
 Binary installers for the latest released version are available at the [Python
 Package Index (PyPI)](https://pypi.org/project/matprops/)
```

### Comparing `matprops-1.0.3/README.md` & `matprops-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `matprops-1.0.3/setup.py` & `matprops-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name='matprops',
-    version='1.0.3',
+    version='1.0.4',
     packages=find_packages(where="src"),
     package_dir={'': 'src'},
     classifiers=[
         "Programming Language :: Python :: 3",
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
```

### Comparing `matprops-1.0.3/src/matprops.egg-info/PKG-INFO` & `matprops-1.0.4/src/matprops.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: matprops
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python library written on top of matplotlib library for customizable proportional charts
 Home-page: https://github.com/shammeer-s/matprops
 Author: Mohammed Shammeer
 Author-email: mohammedshammeer.s@gmail.com
 Keywords: matplotlib,visualization,proportional charts
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: numpy>=1.22.0
+Requires-Dist: pandas>=1.3.5
+Requires-Dist: matplotlib>=3.5.1
+Provides-Extra: dev
+Requires-Dist: pytest>=6.2.5; extra == "dev"
 
 # Matprops
 **matprops** is a Python library for visualizing proportional data. It is build above matplotlib (the visualization library). Understanding proportional data is quite easy but when it comes to bigger picture we lack of seeing everything 
 
 ## Installation
 Binary installers for the latest released version are available at the [Python
 Package Index (PyPI)](https://pypi.org/project/matprops/)
```

