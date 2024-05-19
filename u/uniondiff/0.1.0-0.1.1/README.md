# Comparing `tmp/uniondiff-0.1.0.tar.gz` & `tmp/uniondiff-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uniondiff-0.1.0.tar", last modified: Mon Feb 20 00:53:21 2023, max compression
+gzip compressed data, was "uniondiff-0.1.1.tar", last modified: Sun May 19 23:36:32 2024, max compression
```

## Comparing `uniondiff-0.1.0.tar` & `uniondiff-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 msg       (1000) msg       (1000)        0 2023-02-20 00:53:21.434343 uniondiff-0.1.0/
--rw-rw-r--   0 msg       (1000) msg       (1000)     1493 2023-01-07 23:43:42.000000 uniondiff-0.1.0/LICENSE
--rw-rw-r--   0 msg       (1000) msg       (1000)     2594 2023-02-20 00:53:21.434343 uniondiff-0.1.0/PKG-INFO
--rw-rw-r--   0 msg       (1000) msg       (1000)     1978 2023-02-20 00:45:03.000000 uniondiff-0.1.0/README.md
--rw-rw-r--   0 msg       (1000) msg       (1000)     1382 2023-02-19 22:35:44.000000 uniondiff-0.1.0/pyproject.toml
--rw-rw-r--   0 msg       (1000) msg       (1000)      820 2023-02-20 00:53:21.434343 uniondiff-0.1.0/setup.cfg
-drwxrwxr-x   0 msg       (1000) msg       (1000)        0 2023-02-20 00:53:21.430343 uniondiff-0.1.0/tests/
--rw-rw-r--   0 msg       (1000) msg       (1000)     2398 2023-02-20 00:40:24.000000 uniondiff-0.1.0/tests/test_e2e.py
--rw-rw-r--   0 msg       (1000) msg       (1000)     7017 2023-02-20 00:39:27.000000 uniondiff-0.1.0/tests/test_io_file.py
--rw-rw-r--   0 msg       (1000) msg       (1000)     5923 2023-02-20 00:39:40.000000 uniondiff-0.1.0/tests/test_io_tar.py
--rw-rw-r--   0 msg       (1000) msg       (1000)        0 2023-01-07 23:43:42.000000 uniondiff-0.1.0/tests/tests.py
-drwxrwxr-x   0 msg       (1000) msg       (1000)        0 2023-02-20 00:53:21.434343 uniondiff-0.1.0/uniondiff/
--rw-rw-r--   0 msg       (1000) msg       (1000)        0 2023-01-07 23:43:42.000000 uniondiff-0.1.0/uniondiff/__init__.py
--rw-rw-r--   0 msg       (1000) msg       (1000)      577 2023-02-20 00:45:22.000000 uniondiff-0.1.0/uniondiff/__main__.py
--rw-rw-r--   0 msg       (1000) msg       (1000)       22 2023-01-07 23:43:42.000000 uniondiff-0.1.0/uniondiff/_version.py
--rw-rw-r--   0 msg       (1000) msg       (1000)     6886 2023-02-20 00:42:38.000000 uniondiff-0.1.0/uniondiff/cli.py
--rw-rw-r--   0 msg       (1000) msg       (1000)    18084 2023-02-20 00:40:56.000000 uniondiff-0.1.0/uniondiff/differ.py
--rw-rw-r--   0 msg       (1000) msg       (1000)      666 2023-02-20 00:45:13.000000 uniondiff-0.1.0/uniondiff/exceptions.py
--rw-rw-r--   0 msg       (1000) msg       (1000)     7236 2023-02-19 23:41:07.000000 uniondiff-0.1.0/uniondiff/filelib.py
--rw-rw-r--   0 msg       (1000) msg       (1000)     5160 2023-02-20 00:41:22.000000 uniondiff-0.1.0/uniondiff/filelib_tar.py
--rw-rw-r--   0 msg       (1000) msg       (1000)     1077 2023-02-19 22:41:36.000000 uniondiff-0.1.0/uniondiff/osshim.py
--rw-rw-r--   0 msg       (1000) msg       (1000)     3546 2023-02-20 00:42:09.000000 uniondiff-0.1.0/uniondiff/output.py
--rw-rw-r--   0 msg       (1000) msg       (1000)     1811 2023-02-20 00:42:56.000000 uniondiff-0.1.0/uniondiff/output_aufs.py
--rw-rw-r--   0 msg       (1000) msg       (1000)     2734 2023-02-20 00:43:03.000000 uniondiff-0.1.0/uniondiff/output_file.py
--rw-rw-r--   0 msg       (1000) msg       (1000)     1416 2023-02-20 00:42:00.000000 uniondiff-0.1.0/uniondiff/output_overlay.py
--rw-rw-r--   0 msg       (1000) msg       (1000)     2400 2023-02-20 00:42:24.000000 uniondiff-0.1.0/uniondiff/output_tar.py
-drwxrwxr-x   0 msg       (1000) msg       (1000)        0 2023-02-20 00:53:21.434343 uniondiff-0.1.0/uniondiff.egg-info/
--rw-rw-r--   0 msg       (1000) msg       (1000)     2594 2023-02-20 00:53:21.000000 uniondiff-0.1.0/uniondiff.egg-info/PKG-INFO
--rw-rw-r--   0 msg       (1000) msg       (1000)      601 2023-02-20 00:53:21.000000 uniondiff-0.1.0/uniondiff.egg-info/SOURCES.txt
--rw-rw-r--   0 msg       (1000) msg       (1000)        1 2023-02-20 00:53:21.000000 uniondiff-0.1.0/uniondiff.egg-info/dependency_links.txt
--rw-rw-r--   0 msg       (1000) msg       (1000)       49 2023-02-20 00:53:21.000000 uniondiff-0.1.0/uniondiff.egg-info/entry_points.txt
--rw-rw-r--   0 msg       (1000) msg       (1000)       10 2023-02-20 00:53:21.000000 uniondiff-0.1.0/uniondiff.egg-info/top_level.txt
+drwxrwxr-x   0 msg       (1000) msg       (1000)        0 2024-05-19 23:36:32.765422 uniondiff-0.1.1/
+-rw-rw-r--   0 msg       (1000) msg       (1000)     1493 2023-01-07 23:43:42.000000 uniondiff-0.1.1/LICENSE
+-rw-r--r--   0 msg       (1000) msg       (1000)     2697 2024-05-19 23:36:32.765422 uniondiff-0.1.1/PKG-INFO
+-rw-rw-r--   0 msg       (1000) msg       (1000)     1979 2024-05-19 23:28:54.000000 uniondiff-0.1.1/README.md
+-rw-rw-r--   0 msg       (1000) msg       (1000)     1382 2023-02-19 22:35:44.000000 uniondiff-0.1.1/pyproject.toml
+-rw-rw-r--   0 msg       (1000) msg       (1000)      900 2024-05-19 23:36:32.765422 uniondiff-0.1.1/setup.cfg
+drwxrwxr-x   0 msg       (1000) msg       (1000)        0 2024-05-19 23:36:32.761422 uniondiff-0.1.1/tests/
+-rw-rw-r--   0 msg       (1000) msg       (1000)     2398 2023-02-20 00:40:24.000000 uniondiff-0.1.1/tests/test_e2e.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     7017 2023-02-20 00:39:27.000000 uniondiff-0.1.1/tests/test_io_file.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     5923 2023-02-20 00:39:40.000000 uniondiff-0.1.1/tests/test_io_tar.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)        0 2023-01-07 23:43:42.000000 uniondiff-0.1.1/tests/tests.py
+drwxrwxr-x   0 msg       (1000) msg       (1000)        0 2024-05-19 23:36:32.761422 uniondiff-0.1.1/uniondiff/
+-rw-rw-r--   0 msg       (1000) msg       (1000)        0 2023-01-07 23:43:42.000000 uniondiff-0.1.1/uniondiff/__init__.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)      577 2023-02-20 00:45:22.000000 uniondiff-0.1.1/uniondiff/__main__.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)       22 2024-05-19 23:33:25.000000 uniondiff-0.1.1/uniondiff/_version.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     6886 2023-02-20 00:42:38.000000 uniondiff-0.1.1/uniondiff/cli.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)    18084 2023-02-20 00:40:56.000000 uniondiff-0.1.1/uniondiff/differ.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)      666 2023-02-20 00:45:13.000000 uniondiff-0.1.1/uniondiff/exceptions.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     7236 2023-02-19 23:41:07.000000 uniondiff-0.1.1/uniondiff/filelib.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     5160 2023-02-20 00:41:22.000000 uniondiff-0.1.1/uniondiff/filelib_tar.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     1077 2023-02-19 22:41:36.000000 uniondiff-0.1.1/uniondiff/osshim.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     3546 2023-02-20 00:42:09.000000 uniondiff-0.1.1/uniondiff/output.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     1811 2023-02-20 00:42:56.000000 uniondiff-0.1.1/uniondiff/output_aufs.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     2734 2023-02-20 00:43:03.000000 uniondiff-0.1.1/uniondiff/output_file.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     1416 2023-02-20 00:42:00.000000 uniondiff-0.1.1/uniondiff/output_overlay.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     2400 2023-02-20 00:42:24.000000 uniondiff-0.1.1/uniondiff/output_tar.py
+drwxrwxr-x   0 msg       (1000) msg       (1000)        0 2024-05-19 23:36:32.765422 uniondiff-0.1.1/uniondiff.egg-info/
+-rw-r--r--   0 msg       (1000) msg       (1000)     2697 2024-05-19 23:36:32.000000 uniondiff-0.1.1/uniondiff.egg-info/PKG-INFO
+-rw-rw-r--   0 msg       (1000) msg       (1000)      601 2024-05-19 23:36:32.000000 uniondiff-0.1.1/uniondiff.egg-info/SOURCES.txt
+-rw-rw-r--   0 msg       (1000) msg       (1000)        1 2024-05-19 23:36:32.000000 uniondiff-0.1.1/uniondiff.egg-info/dependency_links.txt
+-rw-rw-r--   0 msg       (1000) msg       (1000)       49 2024-05-19 23:36:32.000000 uniondiff-0.1.1/uniondiff.egg-info/entry_points.txt
+-rw-rw-r--   0 msg       (1000) msg       (1000)       10 2024-05-19 23:36:32.000000 uniondiff-0.1.1/uniondiff.egg-info/top_level.txt
```

### Comparing `uniondiff-0.1.0/LICENSE` & `uniondiff-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `uniondiff-0.1.0/PKG-INFO` & `uniondiff-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: uniondiff
-Version: 0.1.0
+Version: 0.1.1
 Summary: Directory difference CLI tool
 Home-page: http://github.com/msg555/uniondiff/
 Author: Mark Gordon
 Author-email: msg555@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # uniondiff - Directory difference calculator
@@ -40,18 +42,18 @@
 
 ## Installation
 
 *uniondiff* can be installed through *pip*. This installs both the `uniondiff`
 CLI utility and the *uniondiff* Python library.
 
 ```sh
-pip install tplbuild
+pip install uniondiff
 ```
 
-*uniondiff* is supported and tested on Python 3.8-3.10
+*uniondiff* is supported and tested on Python 3.8-3.12
 
 ## Examples
 
 Compute the directory difference between the directory "data-day10" and
 "data-day9". By default the output will be written as a tar file.
 
 ```sh
```

### Comparing `uniondiff-0.1.0/README.md` & `uniondiff-0.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -22,18 +22,18 @@
 
 ## Installation
 
 *uniondiff* can be installed through *pip*. This installs both the `uniondiff`
 CLI utility and the *uniondiff* Python library.
 
 ```sh
-pip install tplbuild
+pip install uniondiff
 ```
 
-*uniondiff* is supported and tested on Python 3.8-3.10
+*uniondiff* is supported and tested on Python 3.8-3.12
 
 ## Examples
 
 Compute the directory difference between the directory "data-day10" and
 "data-day9". By default the output will be written as a tar file.
 
 ```sh
```

### Comparing `uniondiff-0.1.0/pyproject.toml` & `uniondiff-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `uniondiff-0.1.0/tests/test_e2e.py` & `uniondiff-0.1.1/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `uniondiff-0.1.0/tests/test_io_file.py` & `uniondiff-0.1.1/tests/test_io_file.py`

 * *Files identical despite different names*

### Comparing `uniondiff-0.1.0/tests/test_io_tar.py` & `uniondiff-0.1.1/tests/test_io_tar.py`

 * *Files identical despite different names*

### Comparing `uniondiff-0.1.0/uniondiff/__main__.py` & `uniondiff-0.1.1/uniondiff/__main__.py`

 * *Files identical despite different names*

### Comparing `uniondiff-0.1.0/uniondiff/cli.py` & `uniondiff-0.1.1/uniondiff/cli.py`

 * *Files identical despite different names*

### Comparing `uniondiff-0.1.0/uniondiff/differ.py` & `uniondiff-0.1.1/uniondiff/differ.py`

 * *Files identical despite different names*

### Comparing `uniondiff-0.1.0/uniondiff/exceptions.py` & `uniondiff-0.1.1/uniondiff/exceptions.py`

 * *Files identical despite different names*

### Comparing `uniondiff-0.1.0/uniondiff/filelib.py` & `uniondiff-0.1.1/uniondiff/filelib.py`

 * *Files identical despite different names*

### Comparing `uniondiff-0.1.0/uniondiff/filelib_tar.py` & `uniondiff-0.1.1/uniondiff/filelib_tar.py`

 * *Files identical despite different names*

### Comparing `uniondiff-0.1.0/uniondiff/osshim.py` & `uniondiff-0.1.1/uniondiff/osshim.py`

 * *Files identical despite different names*

### Comparing `uniondiff-0.1.0/uniondiff/output.py` & `uniondiff-0.1.1/uniondiff/output.py`

 * *Files identical despite different names*

### Comparing `uniondiff-0.1.0/uniondiff/output_aufs.py` & `uniondiff-0.1.1/uniondiff/output_aufs.py`

 * *Files identical despite different names*

### Comparing `uniondiff-0.1.0/uniondiff/output_file.py` & `uniondiff-0.1.1/uniondiff/output_file.py`

 * *Files identical despite different names*

### Comparing `uniondiff-0.1.0/uniondiff/output_overlay.py` & `uniondiff-0.1.1/uniondiff/output_overlay.py`

 * *Files identical despite different names*

### Comparing `uniondiff-0.1.0/uniondiff/output_tar.py` & `uniondiff-0.1.1/uniondiff/output_tar.py`

 * *Files identical despite different names*

### Comparing `uniondiff-0.1.0/uniondiff.egg-info/PKG-INFO` & `uniondiff-0.1.1/uniondiff.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: uniondiff
-Version: 0.1.0
+Version: 0.1.1
 Summary: Directory difference CLI tool
 Home-page: http://github.com/msg555/uniondiff/
 Author: Mark Gordon
 Author-email: msg555@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # uniondiff - Directory difference calculator
@@ -40,18 +42,18 @@
 
 ## Installation
 
 *uniondiff* can be installed through *pip*. This installs both the `uniondiff`
 CLI utility and the *uniondiff* Python library.
 
 ```sh
-pip install tplbuild
+pip install uniondiff
 ```
 
-*uniondiff* is supported and tested on Python 3.8-3.10
+*uniondiff* is supported and tested on Python 3.8-3.12
 
 ## Examples
 
 Compute the directory difference between the directory "data-day10" and
 "data-day9". By default the output will be written as a tar file.
 
 ```sh
```

### Comparing `uniondiff-0.1.0/uniondiff.egg-info/SOURCES.txt` & `uniondiff-0.1.1/uniondiff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

