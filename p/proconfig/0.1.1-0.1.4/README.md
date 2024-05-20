# Comparing `tmp/proconfig-0.1.1.tar.gz` & `tmp/proconfig-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proconfig-0.1.1.tar", last modified: Mon May 20 05:38:44 2024, max compression
+gzip compressed data, was "proconfig-0.1.4.tar", last modified: Mon May 20 08:00:17 2024, max compression
```

## Comparing `proconfig-0.1.1.tar` & `proconfig-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 I530319    (501) staff       (20)        0 2024-05-20 05:38:44.252510 proconfig-0.1.1/
--rw-r--r--   0 I530319    (501) staff       (20)     2670 2024-05-20 05:38:44.251788 proconfig-0.1.1/PKG-INFO
--rw-r--r--   0 I530319    (501) staff       (20)     2157 2024-05-10 15:38:45.000000 proconfig-0.1.1/README.md
-drwxr-xr-x   0 I530319    (501) staff       (20)        0 2024-05-20 05:38:44.239564 proconfig-0.1.1/proconfig/
--rw-r--r--   0 I530319    (501) staff       (20)        0 2024-05-20 05:13:59.000000 proconfig-0.1.1/proconfig/__init__.py
--rw-r--r--   0 I530319    (501) staff       (20)     4950 2024-05-20 05:24:14.000000 proconfig-0.1.1/proconfig/cli.py
-drwxr-xr-x   0 I530319    (501) staff       (20)        0 2024-05-20 05:38:44.251074 proconfig-0.1.1/proconfig.egg-info/
--rw-r--r--   0 I530319    (501) staff       (20)     2670 2024-05-20 05:38:44.000000 proconfig-0.1.1/proconfig.egg-info/PKG-INFO
--rw-r--r--   0 I530319    (501) staff       (20)      257 2024-05-20 05:38:44.000000 proconfig-0.1.1/proconfig.egg-info/SOURCES.txt
--rw-r--r--   0 I530319    (501) staff       (20)        1 2024-05-20 05:38:44.000000 proconfig-0.1.1/proconfig.egg-info/dependency_links.txt
--rw-r--r--   0 I530319    (501) staff       (20)       42 2024-05-20 05:38:44.000000 proconfig-0.1.1/proconfig.egg-info/entry_points.txt
--rw-r--r--   0 I530319    (501) staff       (20)       25 2024-05-20 05:38:44.000000 proconfig-0.1.1/proconfig.egg-info/requires.txt
--rw-r--r--   0 I530319    (501) staff       (20)       10 2024-05-20 05:38:44.000000 proconfig-0.1.1/proconfig.egg-info/top_level.txt
--rw-r--r--   0 I530319    (501) staff       (20)       38 2024-05-20 05:38:44.252665 proconfig-0.1.1/setup.cfg
--rw-r--r--   0 I530319    (501) staff       (20)      829 2024-05-20 05:38:26.000000 proconfig-0.1.1/setup.py
+drwxr-xr-x   0 I530319    (501) staff       (20)        0 2024-05-20 08:00:17.666299 proconfig-0.1.4/
+-rw-r--r--   0 I530319    (501) staff       (20)     2670 2024-05-20 08:00:17.665671 proconfig-0.1.4/PKG-INFO
+-rw-r--r--   0 I530319    (501) staff       (20)     2157 2024-05-10 15:38:45.000000 proconfig-0.1.4/README.md
+drwxr-xr-x   0 I530319    (501) staff       (20)        0 2024-05-20 08:00:17.652155 proconfig-0.1.4/proconfig/
+-rw-r--r--   0 I530319    (501) staff       (20)     1795 2024-05-20 06:03:08.000000 proconfig-0.1.4/proconfig/__init__.py
+-rw-r--r--   0 I530319    (501) staff       (20)       22 2024-05-20 06:02:26.000000 proconfig-0.1.4/proconfig/__version__.py
+-rw-r--r--   0 I530319    (501) staff       (20)     5755 2024-05-20 07:55:10.000000 proconfig-0.1.4/proconfig/cli.py
+drwxr-xr-x   0 I530319    (501) staff       (20)        0 2024-05-20 08:00:17.665066 proconfig-0.1.4/proconfig.egg-info/
+-rw-r--r--   0 I530319    (501) staff       (20)     2670 2024-05-20 08:00:17.000000 proconfig-0.1.4/proconfig.egg-info/PKG-INFO
+-rw-r--r--   0 I530319    (501) staff       (20)      282 2024-05-20 08:00:17.000000 proconfig-0.1.4/proconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 I530319    (501) staff       (20)        1 2024-05-20 08:00:17.000000 proconfig-0.1.4/proconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 I530319    (501) staff       (20)       42 2024-05-20 08:00:17.000000 proconfig-0.1.4/proconfig.egg-info/entry_points.txt
+-rw-r--r--   0 I530319    (501) staff       (20)       25 2024-05-20 08:00:17.000000 proconfig-0.1.4/proconfig.egg-info/requires.txt
+-rw-r--r--   0 I530319    (501) staff       (20)       10 2024-05-20 08:00:17.000000 proconfig-0.1.4/proconfig.egg-info/top_level.txt
+-rw-r--r--   0 I530319    (501) staff       (20)       38 2024-05-20 08:00:17.666412 proconfig-0.1.4/setup.cfg
+-rw-r--r--   0 I530319    (501) staff       (20)      829 2024-05-20 07:54:47.000000 proconfig-0.1.4/setup.py
```

### Comparing `proconfig-0.1.1/PKG-INFO` & `proconfig-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proconfig
-Version: 0.1.1
+Version: 0.1.4
 Summary: A CLI tool for simplify MyShell PorConfig programming.
 Home-page: https://github.com/cybernagle/proconfig-generator
 Author: cybernagle
 Author-email: zhang.nagle@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `proconfig-0.1.1/README.md` & `proconfig-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `proconfig-0.1.1/proconfig.egg-info/PKG-INFO` & `proconfig-0.1.4/proconfig.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proconfig
-Version: 0.1.1
+Version: 0.1.4
 Summary: A CLI tool for simplify MyShell PorConfig programming.
 Home-page: https://github.com/cybernagle/proconfig-generator
 Author: cybernagle
 Author-email: zhang.nagle@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `proconfig-0.1.1/setup.py` & `proconfig-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='proconfig',
-    version='0.1.1',
+    version='0.1.4',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'click',
         "tabulate",
         "termcolor",
     ],
```

