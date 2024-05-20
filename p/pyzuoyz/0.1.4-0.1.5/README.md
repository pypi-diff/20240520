# Comparing `tmp/pyzuoyz-0.1.4.tar.gz` & `tmp/pyzuoyz-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyzuoyz-0.1.4.tar", last modified: Mon Apr  1 11:49:23 2024, max compression
+gzip compressed data, was "pyzuoyz-0.1.5.tar", last modified: Mon May 20 03:19:48 2024, max compression
```

## Comparing `pyzuoyz-0.1.4.tar` & `pyzuoyz-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 aaazuoyz   (501) staff       (20)        0 2024-04-01 11:49:23.980746 pyzuoyz-0.1.4/
--rw-r--r--   0 aaazuoyz   (501) staff       (20)     1068 2024-04-01 04:24:56.000000 pyzuoyz-0.1.4/LICENSE
--rw-r--r--   0 aaazuoyz   (501) staff       (20)      948 2024-04-01 11:49:23.980548 pyzuoyz-0.1.4/PKG-INFO
--rw-r--r--   0 aaazuoyz   (501) staff       (20)       96 2024-04-01 04:54:26.000000 pyzuoyz-0.1.4/README.rst
-drwxr-xr-x   0 aaazuoyz   (501) staff       (20)        0 2024-04-01 11:49:23.979511 pyzuoyz-0.1.4/pyzuoyz/
--rw-r--r--   0 aaazuoyz   (501) staff       (20)       17 2024-04-01 11:48:21.000000 pyzuoyz-0.1.4/pyzuoyz/__init__.py
--rw-r--r--   0 aaazuoyz   (501) staff       (20)      129 2024-04-01 05:07:13.000000 pyzuoyz-0.1.4/pyzuoyz/help.py
-drwxr-xr-x   0 aaazuoyz   (501) staff       (20)        0 2024-04-01 11:49:23.980262 pyzuoyz-0.1.4/pyzuoyz.egg-info/
--rw-r--r--   0 aaazuoyz   (501) staff       (20)      948 2024-04-01 11:49:23.000000 pyzuoyz-0.1.4/pyzuoyz.egg-info/PKG-INFO
--rw-r--r--   0 aaazuoyz   (501) staff       (20)      217 2024-04-01 11:49:23.000000 pyzuoyz-0.1.4/pyzuoyz.egg-info/SOURCES.txt
--rw-r--r--   0 aaazuoyz   (501) staff       (20)        1 2024-04-01 11:49:23.000000 pyzuoyz-0.1.4/pyzuoyz.egg-info/dependency_links.txt
--rw-r--r--   0 aaazuoyz   (501) staff       (20)       17 2024-04-01 11:49:23.000000 pyzuoyz-0.1.4/pyzuoyz.egg-info/requires.txt
--rw-r--r--   0 aaazuoyz   (501) staff       (20)        8 2024-04-01 11:49:23.000000 pyzuoyz-0.1.4/pyzuoyz.egg-info/top_level.txt
--rw-r--r--   0 aaazuoyz   (501) staff       (20)       38 2024-04-01 11:49:23.980788 pyzuoyz-0.1.4/setup.cfg
--rw-r--r--   0 aaazuoyz   (501) staff       (20)     4053 2024-04-01 11:48:58.000000 pyzuoyz-0.1.4/setup.py
+drwxr-xr-x   0 aaazuoyz   (501) staff       (20)        0 2024-05-20 03:19:48.510582 pyzuoyz-0.1.5/
+-rw-r--r--   0 aaazuoyz   (501) staff       (20)     1068 2024-04-01 04:24:56.000000 pyzuoyz-0.1.5/LICENSE
+-rw-r--r--   0 aaazuoyz   (501) staff       (20)      948 2024-05-20 03:19:48.510241 pyzuoyz-0.1.5/PKG-INFO
+-rw-r--r--   0 aaazuoyz   (501) staff       (20)       96 2024-04-01 04:54:26.000000 pyzuoyz-0.1.5/README.rst
+drwxr-xr-x   0 aaazuoyz   (501) staff       (20)        0 2024-05-20 03:19:48.508296 pyzuoyz-0.1.5/pyzuoyz/
+-rw-r--r--   0 aaazuoyz   (501) staff       (20)      195 2024-05-20 03:17:24.000000 pyzuoyz-0.1.5/pyzuoyz/__init__.py
+-rw-r--r--   0 aaazuoyz   (501) staff       (20)      783 2024-04-01 05:54:33.000000 pyzuoyz-0.1.5/pyzuoyz/metrics.py
+-rw-r--r--   0 aaazuoyz   (501) staff       (20)     2236 2024-04-01 05:44:58.000000 pyzuoyz-0.1.5/pyzuoyz/prompt.py
+-rw-r--r--   0 aaazuoyz   (501) staff       (20)     2773 2024-05-20 03:18:29.000000 pyzuoyz-0.1.5/pyzuoyz/scaled_rope.py
+drwxr-xr-x   0 aaazuoyz   (501) staff       (20)        0 2024-05-20 03:19:48.509818 pyzuoyz-0.1.5/pyzuoyz.egg-info/
+-rw-r--r--   0 aaazuoyz   (501) staff       (20)      948 2024-05-20 03:19:48.000000 pyzuoyz-0.1.5/pyzuoyz.egg-info/PKG-INFO
+-rw-r--r--   0 aaazuoyz   (501) staff       (20)      261 2024-05-20 03:19:48.000000 pyzuoyz-0.1.5/pyzuoyz.egg-info/SOURCES.txt
+-rw-r--r--   0 aaazuoyz   (501) staff       (20)        1 2024-05-20 03:19:48.000000 pyzuoyz-0.1.5/pyzuoyz.egg-info/dependency_links.txt
+-rw-r--r--   0 aaazuoyz   (501) staff       (20)       17 2024-05-20 03:19:48.000000 pyzuoyz-0.1.5/pyzuoyz.egg-info/requires.txt
+-rw-r--r--   0 aaazuoyz   (501) staff       (20)        8 2024-05-20 03:19:48.000000 pyzuoyz-0.1.5/pyzuoyz.egg-info/top_level.txt
+-rw-r--r--   0 aaazuoyz   (501) staff       (20)       38 2024-05-20 03:19:48.510652 pyzuoyz-0.1.5/setup.cfg
+-rw-r--r--   0 aaazuoyz   (501) staff       (20)     4053 2024-05-20 03:18:35.000000 pyzuoyz-0.1.5/setup.py
```

### Comparing `pyzuoyz-0.1.4/LICENSE` & `pyzuoyz-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyzuoyz-0.1.4/PKG-INFO` & `pyzuoyz-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyzuoyz
-Version: 0.1.4
+Version: 0.1.5
 Summary: Packages for zyz.
 Author: Yuezhong Zuo
 Author-email: z80179030@163.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyzuoyz-0.1.4/pyzuoyz.egg-info/PKG-INFO` & `pyzuoyz-0.1.5/pyzuoyz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyzuoyz
-Version: 0.1.4
+Version: 0.1.5
 Summary: Packages for zyz.
 Author: Yuezhong Zuo
 Author-email: z80179030@163.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyzuoyz-0.1.4/setup.py` & `pyzuoyz-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'pyzuoyz'
 DESCRIPTION = 'Packages for zyz.'
 URL = 'https://github.com/me/myproject'
 EMAIL = 'z80179030@163.com'
 AUTHOR = 'Yuezhong Zuo'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.4'
+VERSION = '0.1.5'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'nltk', 'jieba', 'rouge',
 ]
 
 # What packages are optional?
```

