# Comparing `tmp/betterschema-0.1.8.tar.gz` & `tmp/betterschema-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betterschema-0.1.8.tar", last modified: Sun May 19 21:18:33 2024, max compression
+gzip compressed data, was "betterschema-0.1.9.tar", last modified: Sun May 19 21:25:06 2024, max compression
```

## Comparing `betterschema-0.1.8.tar` & `betterschema-0.1.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:18:33.100341 betterschema-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-19 21:18:27.000000 betterschema-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-05-19 21:18:33.100341 betterschema-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-19 21:18:27.000000 betterschema-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:18:33.092341 betterschema-0.1.8/baselib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:18:33.096341 betterschema-0.1.8/baselib/src/
--rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-05-19 21:18:27.000000 betterschema-0.1.8/baselib/src/attr.c
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-05-19 21:18:27.000000 betterschema-0.1.8/baselib/src/init.c
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-19 21:18:27.000000 betterschema-0.1.8/baselib/src/module.c
--rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-05-19 21:18:27.000000 betterschema-0.1.8/baselib/src/schema.c
--rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-05-19 21:18:27.000000 betterschema-0.1.8/baselib/src/utils.c
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-19 21:18:27.000000 betterschema-0.1.8/baselib/src/watch.c
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-19 21:18:27.000000 betterschema-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 21:18:33.100341 betterschema-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-19 21:18:27.000000 betterschema-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:18:33.092341 betterschema-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:18:33.096341 betterschema-0.1.8/src/betterschema/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-19 21:18:27.000000 betterschema-0.1.8/src/betterschema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-19 21:18:27.000000 betterschema-0.1.8/src/betterschema/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-19 21:18:27.000000 betterschema-0.1.8/src/betterschema/render.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:18:33.096341 betterschema-0.1.8/src/betterschema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-05-19 21:18:33.000000 betterschema-0.1.8/src/betterschema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-19 21:18:33.000000 betterschema-0.1.8/src/betterschema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 21:18:33.000000 betterschema-0.1.8/src/betterschema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-19 21:18:33.000000 betterschema-0.1.8/src/betterschema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-19 21:18:33.000000 betterschema-0.1.8/src/betterschema.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:18:33.096341 betterschema-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-19 21:18:27.000000 betterschema-0.1.8/tests/testlib.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-19 21:18:27.000000 betterschema-0.1.8/tests/testrender.py
--rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-05-19 21:18:27.000000 betterschema-0.1.8/tests/testschema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:25:06.188799 betterschema-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-19 21:25:00.000000 betterschema-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-05-19 21:25:06.188799 betterschema-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-19 21:25:00.000000 betterschema-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:25:06.184799 betterschema-0.1.9/baselib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:25:06.184799 betterschema-0.1.9/baselib/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-05-19 21:25:00.000000 betterschema-0.1.9/baselib/src/attr.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-05-19 21:25:00.000000 betterschema-0.1.9/baselib/src/init.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-19 21:25:00.000000 betterschema-0.1.9/baselib/src/module.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-05-19 21:25:00.000000 betterschema-0.1.9/baselib/src/schema.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-05-19 21:25:00.000000 betterschema-0.1.9/baselib/src/utils.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-19 21:25:00.000000 betterschema-0.1.9/baselib/src/watch.c
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-19 21:25:00.000000 betterschema-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 21:25:06.188799 betterschema-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-19 21:25:00.000000 betterschema-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:25:06.184799 betterschema-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:25:06.184799 betterschema-0.1.9/src/betterschema/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-19 21:25:00.000000 betterschema-0.1.9/src/betterschema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-19 21:25:00.000000 betterschema-0.1.9/src/betterschema/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-19 21:25:00.000000 betterschema-0.1.9/src/betterschema/render.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:25:06.188799 betterschema-0.1.9/src/betterschema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-05-19 21:25:06.000000 betterschema-0.1.9/src/betterschema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-19 21:25:06.000000 betterschema-0.1.9/src/betterschema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 21:25:06.000000 betterschema-0.1.9/src/betterschema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-19 21:25:06.000000 betterschema-0.1.9/src/betterschema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-19 21:25:06.000000 betterschema-0.1.9/src/betterschema.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:25:06.188799 betterschema-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-19 21:25:00.000000 betterschema-0.1.9/tests/testlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-19 21:25:00.000000 betterschema-0.1.9/tests/testrender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-05-19 21:25:00.000000 betterschema-0.1.9/tests/testschema.py
```

### Comparing `betterschema-0.1.8/LICENSE` & `betterschema-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `betterschema-0.1.8/PKG-INFO` & `betterschema-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betterschema
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python schema library that supports type checking and validation
 Author: Wilson Wang
 Author-email: wilsonny371@gmail.com
 Project-URL: Source, https://github.com/wilsonwang371/betterschema
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `betterschema-0.1.8/README.md` & `betterschema-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `betterschema-0.1.8/baselib/src/attr.c` & `betterschema-0.1.9/baselib/src/attr.c`

 * *Files identical despite different names*

### Comparing `betterschema-0.1.8/baselib/src/init.c` & `betterschema-0.1.9/baselib/src/init.c`

 * *Files identical despite different names*

### Comparing `betterschema-0.1.8/baselib/src/module.c` & `betterschema-0.1.9/baselib/src/module.c`

 * *Files identical despite different names*

### Comparing `betterschema-0.1.8/baselib/src/schema.c` & `betterschema-0.1.9/baselib/src/schema.c`

 * *Files identical despite different names*

### Comparing `betterschema-0.1.8/baselib/src/utils.c` & `betterschema-0.1.9/baselib/src/utils.c`

 * *Files identical despite different names*

### Comparing `betterschema-0.1.8/baselib/src/watch.c` & `betterschema-0.1.9/baselib/src/watch.c`

 * *Files identical despite different names*

### Comparing `betterschema-0.1.8/setup.py` & `betterschema-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `betterschema-0.1.8/src/betterschema/core.py` & `betterschema-0.1.9/src/betterschema/core.py`

 * *Files identical despite different names*

### Comparing `betterschema-0.1.8/src/betterschema/render.py` & `betterschema-0.1.9/src/betterschema/render.py`

 * *Files identical despite different names*

### Comparing `betterschema-0.1.8/src/betterschema.egg-info/PKG-INFO` & `betterschema-0.1.9/src/betterschema.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betterschema
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python schema library that supports type checking and validation
 Author: Wilson Wang
 Author-email: wilsonny371@gmail.com
 Project-URL: Source, https://github.com/wilsonwang371/betterschema
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `betterschema-0.1.8/tests/testlib.py` & `betterschema-0.1.9/tests/testlib.py`

 * *Files identical despite different names*

### Comparing `betterschema-0.1.8/tests/testrender.py` & `betterschema-0.1.9/tests/testrender.py`

 * *Files identical despite different names*

### Comparing `betterschema-0.1.8/tests/testschema.py` & `betterschema-0.1.9/tests/testschema.py`

 * *Files identical despite different names*

