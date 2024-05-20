# Comparing `tmp/stsci_image-2.3.7.tar.gz` & `tmp/stsci_image-2.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stsci_image-2.3.7.tar", last modified: Fri May 10 13:29:24 2024, max compression
+gzip compressed data, was "stsci_image-2.3.8.tar", last modified: Mon May 20 13:27:12 2024, max compression
```

## Comparing `stsci_image-2.3.7.tar` & `stsci_image-2.3.8.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:29:24.115718 stsci_image-2.3.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:29:24.107717 stsci_image-2.3.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:29:24.107717 stsci_image-2.3.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-10 13:29:11.000000 stsci_image-2.3.7/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-10 13:29:11.000000 stsci_image-2.3.7/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-10 13:29:11.000000 stsci_image-2.3.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-10 13:29:11.000000 stsci_image-2.3.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-10 13:29:24.115718 stsci_image-2.3.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:29:24.107717 stsci_image-2.3.7/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-10 13:29:11.000000 stsci_image-2.3.7/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-10 13:29:11.000000 stsci_image-2.3.7/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:29:24.111717 stsci_image-2.3.7/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-05-10 13:29:11.000000 stsci_image-2.3.7/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-10 13:29:11.000000 stsci_image-2.3.7/docs/source/image.rst
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-10 13:29:11.000000 stsci_image-2.3.7/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-10 13:29:11.000000 stsci_image-2.3.7/docs/source/numcombine.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-10 13:29:11.000000 stsci_image-2.3.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 13:29:24.115718 stsci_image-2.3.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      310 2024-05-10 13:29:11.000000 stsci_image-2.3.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:29:24.111717 stsci_image-2.3.7/src/
--rw-r--r--   0 runner    (1001) docker     (127)     9490 2024-05-10 13:29:11.000000 stsci_image-2.3.7/src/_combinemodule.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:29:24.111717 stsci_image-2.3.7/stsci/
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-10 13:29:11.000000 stsci_image-2.3.7/stsci/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:29:24.111717 stsci_image-2.3.7/stsci/image/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-10 13:29:11.000000 stsci_image-2.3.7/stsci/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-10 13:29:11.000000 stsci_image-2.3.7/stsci/image/_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    13448 2024-05-10 13:29:11.000000 stsci_image-2.3.7/stsci/image/combine.py
--rw-r--r--   0 runner    (1001) docker     (127)    16306 2024-05-10 13:29:11.000000 stsci_image-2.3.7/stsci/image/numcombine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:29:24.115718 stsci_image-2.3.7/stsci/image/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:29:11.000000 stsci_image-2.3.7/stsci/image/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-10 13:29:11.000000 stsci_image-2.3.7/stsci/image/test/test_average.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-10 13:29:11.000000 stsci_image-2.3.7/stsci/image/test/test_median.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-05-10 13:29:11.000000 stsci_image-2.3.7/stsci/image/test/test_minimum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-10 13:29:11.000000 stsci_image-2.3.7/stsci/image/test/test_threshold.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:29:24.115718 stsci_image-2.3.7/stsci.image.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-10 13:29:24.000000 stsci_image-2.3.7/stsci.image.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-10 13:29:24.000000 stsci_image-2.3.7/stsci.image.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 13:29:24.000000 stsci_image-2.3.7/stsci.image.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 13:29:23.000000 stsci_image-2.3.7/stsci.image.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-10 13:29:24.000000 stsci_image-2.3.7/stsci.image.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 13:29:24.000000 stsci_image-2.3.7/stsci.image.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:27:12.625613 stsci_image-2.3.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:27:12.617613 stsci_image-2.3.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:27:12.621613 stsci_image-2.3.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-20 13:27:01.000000 stsci_image-2.3.8/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-20 13:27:01.000000 stsci_image-2.3.8/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-20 13:27:01.000000 stsci_image-2.3.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-20 13:27:01.000000 stsci_image-2.3.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-20 13:27:12.625613 stsci_image-2.3.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:27:12.621613 stsci_image-2.3.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-20 13:27:01.000000 stsci_image-2.3.8/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-20 13:27:01.000000 stsci_image-2.3.8/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:27:12.621613 stsci_image-2.3.8/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-05-20 13:27:01.000000 stsci_image-2.3.8/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-20 13:27:01.000000 stsci_image-2.3.8/docs/source/image.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-20 13:27:01.000000 stsci_image-2.3.8/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-20 13:27:01.000000 stsci_image-2.3.8/docs/source/numcombine.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-20 13:27:01.000000 stsci_image-2.3.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 13:27:12.625613 stsci_image-2.3.8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      310 2024-05-20 13:27:01.000000 stsci_image-2.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:27:12.621613 stsci_image-2.3.8/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     9490 2024-05-20 13:27:01.000000 stsci_image-2.3.8/src/_combinemodule.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:27:12.621613 stsci_image-2.3.8/stsci/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 13:27:01.000000 stsci_image-2.3.8/stsci/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:27:12.625613 stsci_image-2.3.8/stsci/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-20 13:27:01.000000 stsci_image-2.3.8/stsci/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-20 13:27:01.000000 stsci_image-2.3.8/stsci/image/_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13448 2024-05-20 13:27:01.000000 stsci_image-2.3.8/stsci/image/combine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16306 2024-05-20 13:27:01.000000 stsci_image-2.3.8/stsci/image/numcombine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:27:12.625613 stsci_image-2.3.8/stsci/image/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 13:27:01.000000 stsci_image-2.3.8/stsci/image/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-20 13:27:01.000000 stsci_image-2.3.8/stsci/image/test/test_average.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-20 13:27:01.000000 stsci_image-2.3.8/stsci/image/test/test_median.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-05-20 13:27:01.000000 stsci_image-2.3.8/stsci/image/test/test_minimum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-20 13:27:01.000000 stsci_image-2.3.8/stsci/image/test/test_threshold.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:27:12.625613 stsci_image-2.3.8/stsci.image.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-20 13:27:12.000000 stsci_image-2.3.8/stsci.image.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-20 13:27:12.000000 stsci_image-2.3.8/stsci.image.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 13:27:12.000000 stsci_image-2.3.8/stsci.image.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 13:27:12.000000 stsci_image-2.3.8/stsci.image.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-20 13:27:12.000000 stsci_image-2.3.8/stsci.image.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-20 13:27:12.000000 stsci_image-2.3.8/stsci.image.egg-info/top_level.txt
```

### Comparing `stsci_image-2.3.7/.github/workflows/build.yml` & `stsci_image-2.3.8/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `stsci_image-2.3.7/.github/workflows/ci.yml` & `stsci_image-2.3.8/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `stsci_image-2.3.7/LICENSE.txt` & `stsci_image-2.3.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stsci_image-2.3.7/PKG-INFO` & `stsci_image-2.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stsci.image
-Version: 2.3.7
+Version: 2.3.8
 Summary: Image array manipulation functions
 Author-email: STScI <help@stsci.edu>
 Project-URL: repository, https://github.com/spacetelescope/stsci.image
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `stsci_image-2.3.7/docs/Makefile` & `stsci_image-2.3.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `stsci_image-2.3.7/docs/make.bat` & `stsci_image-2.3.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `stsci_image-2.3.7/docs/source/conf.py` & `stsci_image-2.3.8/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `stsci_image-2.3.7/docs/source/index.rst` & `stsci_image-2.3.8/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `stsci_image-2.3.7/pyproject.toml` & `stsci_image-2.3.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stsci_image-2.3.7/src/_combinemodule.c` & `stsci_image-2.3.8/src/_combinemodule.c`

 * *Files identical despite different names*

### Comparing `stsci_image-2.3.7/stsci/image/_image.py` & `stsci_image-2.3.8/stsci/image/_image.py`

 * *Files identical despite different names*

### Comparing `stsci_image-2.3.7/stsci/image/combine.py` & `stsci_image-2.3.8/stsci/image/combine.py`

 * *Files identical despite different names*

### Comparing `stsci_image-2.3.7/stsci/image/numcombine.py` & `stsci_image-2.3.8/stsci/image/numcombine.py`

 * *Files identical despite different names*

### Comparing `stsci_image-2.3.7/stsci/image/test/test_average.py` & `stsci_image-2.3.8/stsci/image/test/test_average.py`

 * *Files identical despite different names*

### Comparing `stsci_image-2.3.7/stsci/image/test/test_median.py` & `stsci_image-2.3.8/stsci/image/test/test_median.py`

 * *Files identical despite different names*

### Comparing `stsci_image-2.3.7/stsci/image/test/test_minimum.py` & `stsci_image-2.3.8/stsci/image/test/test_minimum.py`

 * *Files identical despite different names*

### Comparing `stsci_image-2.3.7/stsci/image/test/test_threshold.py` & `stsci_image-2.3.8/stsci/image/test/test_threshold.py`

 * *Files identical despite different names*

### Comparing `stsci_image-2.3.7/stsci.image.egg-info/PKG-INFO` & `stsci_image-2.3.8/stsci.image.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stsci.image
-Version: 2.3.7
+Version: 2.3.8
 Summary: Image array manipulation functions
 Author-email: STScI <help@stsci.edu>
 Project-URL: repository, https://github.com/spacetelescope/stsci.image
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `stsci_image-2.3.7/stsci.image.egg-info/SOURCES.txt` & `stsci_image-2.3.8/stsci.image.egg-info/SOURCES.txt`

 * *Files identical despite different names*

