# Comparing `tmp/matprops-1.0.4.tar.gz` & `tmp/matprops-1.0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matprops-1.0.4.tar", last modified: Mon May 20 00:16:09 2024, max compression
+gzip compressed data, was "matprops-1.0.4.1.tar", last modified: Mon May 20 00:26:44 2024, max compression
```

## Comparing `matprops-1.0.4.tar` & `matprops-1.0.4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:16:09.673164 matprops-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-20 00:15:49.000000 matprops-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-20 00:16:09.673164 matprops-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-20 00:15:49.000000 matprops-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 00:16:09.673164 matprops-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-20 00:15:49.000000 matprops-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:16:09.669163 matprops-1.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:16:09.673164 matprops-1.0.4/src/matprops/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 00:15:49.000000 matprops-1.0.4/src/matprops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-05-20 00:15:49.000000 matprops-1.0.4/src/matprops/props.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:16:09.673164 matprops-1.0.4/src/matprops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-20 00:16:09.000000 matprops-1.0.4/src/matprops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-20 00:16:09.000000 matprops-1.0.4/src/matprops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 00:16:09.000000 matprops-1.0.4/src/matprops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-20 00:16:09.000000 matprops-1.0.4/src/matprops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-20 00:16:09.000000 matprops-1.0.4/src/matprops.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:26:44.142047 matprops-1.0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-20 00:26:39.000000 matprops-1.0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-05-20 00:26:44.142047 matprops-1.0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-20 00:26:39.000000 matprops-1.0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 00:26:44.142047 matprops-1.0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-20 00:26:39.000000 matprops-1.0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:26:44.138047 matprops-1.0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:26:44.142047 matprops-1.0.4.1/src/matprops/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 00:26:39.000000 matprops-1.0.4.1/src/matprops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-05-20 00:26:39.000000 matprops-1.0.4.1/src/matprops/props.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:26:44.142047 matprops-1.0.4.1/src/matprops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-05-20 00:26:44.000000 matprops-1.0.4.1/src/matprops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-20 00:26:44.000000 matprops-1.0.4.1/src/matprops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 00:26:44.000000 matprops-1.0.4.1/src/matprops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-20 00:26:44.000000 matprops-1.0.4.1/src/matprops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-20 00:26:44.000000 matprops-1.0.4.1/src/matprops.egg-info/top_level.txt
```

### Comparing `matprops-1.0.4/LICENSE` & `matprops-1.0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `matprops-1.0.4/PKG-INFO` & `matprops-1.0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matprops
-Version: 1.0.4
+Version: 1.0.4.1
 Summary: Python library written on top of matplotlib library for customizable proportional charts
 Home-page: https://github.com/shammeer-s/matprops
 Author: Mohammed Shammeer
 Author-email: mohammedshammeer.s@gmail.com
 Keywords: matplotlib,visualization,proportional charts
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `matprops-1.0.4/README.md` & `matprops-1.0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `matprops-1.0.4/setup.py` & `matprops-1.0.4.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name='matprops',
-    version='1.0.4',
+    version='1.0.4.1',
     packages=find_packages(where="src"),
     package_dir={'': 'src'},
     classifiers=[
         "Programming Language :: Python :: 3",
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
```

### Comparing `matprops-1.0.4/src/matprops/props.py` & `matprops-1.0.4.1/src/matprops/props.py`

 * *Files identical despite different names*

### Comparing `matprops-1.0.4/src/matprops.egg-info/PKG-INFO` & `matprops-1.0.4.1/src/matprops.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matprops
-Version: 1.0.4
+Version: 1.0.4.1
 Summary: Python library written on top of matplotlib library for customizable proportional charts
 Home-page: https://github.com/shammeer-s/matprops
 Author: Mohammed Shammeer
 Author-email: mohammedshammeer.s@gmail.com
 Keywords: matplotlib,visualization,proportional charts
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
```

