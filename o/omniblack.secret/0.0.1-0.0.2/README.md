# Comparing `tmp/omniblack_secret-0.0.1.tar.gz` & `tmp/omniblack_secret-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omniblack_secret-0.0.1.tar", last modified: Sat Apr 27 21:27:21 2024, max compression
+gzip compressed data, was "omniblack_secret-0.0.2.tar", last modified: Sun May 19 19:15:46 2024, max compression
```

## Comparing `omniblack_secret-0.0.1.tar` & `omniblack_secret-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,14 @@
-drwxr-xr-x   0 terryp    (1000) terryp    (1000)        0 2024-04-27 21:27:21.410056 omniblack_secret-0.0.1/
--rw-r--r--   0 terryp    (1000) terryp    (1000)     1099 2024-04-27 17:21:57.000000 omniblack_secret-0.0.1/LICENSE
--rw-r--r--   0 terryp    (1000) terryp    (1000)       56 2024-04-27 17:51:52.000000 omniblack_secret-0.0.1/MANIFEST.in
--rw-r--r--   0 terryp    (1000) terryp    (1000)      582 2024-04-27 21:27:21.410056 omniblack_secret-0.0.1/PKG-INFO
-drwxr-xr-x   0 terryp    (1000) terryp    (1000)        0 2024-04-27 21:27:21.408056 omniblack_secret-0.0.1/include/
--rw-r--r--   0 terryp    (1000) terryp    (1000)    18620 2024-04-27 17:09:33.000000 omniblack_secret-0.0.1/include/rpmalloc.h
--rw-r--r--   0 terryp    (1000) terryp    (1000)    18661 2024-04-27 17:09:33.000000 omniblack_secret-0.0.1/malloc.c
-drwxr-xr-x   0 terryp    (1000) terryp    (1000)        0 2024-04-27 21:27:21.409056 omniblack_secret-0.0.1/omniblack.secret.egg-info/
--rw-r--r--   0 terryp    (1000) terryp    (1000)      582 2024-04-27 21:27:21.000000 omniblack_secret-0.0.1/omniblack.secret.egg-info/PKG-INFO
--rw-r--r--   0 terryp    (1000) terryp    (1000)      251 2024-04-27 21:27:21.000000 omniblack_secret-0.0.1/omniblack.secret.egg-info/SOURCES.txt
--rw-r--r--   0 terryp    (1000) terryp    (1000)        1 2024-04-27 21:27:21.000000 omniblack_secret-0.0.1/omniblack.secret.egg-info/dependency_links.txt
--rw-r--r--   0 terryp    (1000) terryp    (1000)       10 2024-04-27 21:27:21.000000 omniblack_secret-0.0.1/omniblack.secret.egg-info/top_level.txt
--rw-r--r--   0 terryp    (1000) terryp    (1000)      675 2024-04-27 18:35:52.000000 omniblack_secret-0.0.1/pyproject.toml
--rw-r--r--   0 terryp    (1000) terryp    (1000)    71417 2024-04-27 17:09:33.000000 omniblack_secret-0.0.1/rpmalloc.c
--rw-r--r--   0 terryp    (1000) terryp    (1000)     7111 2024-04-27 20:59:35.000000 omniblack_secret-0.0.1/secret.c
--rw-r--r--   0 terryp    (1000) terryp    (1000)       38 2024-04-27 21:27:21.410056 omniblack_secret-0.0.1/setup.cfg
--rw-r--r--   0 terryp    (1000) terryp    (1000)      532 2024-04-27 18:24:09.000000 omniblack_secret-0.0.1/setup.py
+drwxr-xr-x   0 terryp    (1000) terryp    (1000)        0 2024-05-19 19:15:46.705006 omniblack_secret-0.0.2/
+-rw-r--r--   0 terryp    (1000) terryp    (1000)     1099 2024-04-27 17:21:57.000000 omniblack_secret-0.0.2/LICENSE
+-rw-r--r--   0 terryp    (1000) terryp    (1000)       18 2024-05-19 18:48:32.000000 omniblack_secret-0.0.2/MANIFEST.in
+-rw-r--r--   0 terryp    (1000) terryp    (1000)      582 2024-05-19 19:15:46.704006 omniblack_secret-0.0.2/PKG-INFO
+-rw-r--r--   0 terryp    (1000) terryp    (1000)     1997 2024-05-19 18:55:42.000000 omniblack_secret-0.0.2/cflags.py
+drwxr-xr-x   0 terryp    (1000) terryp    (1000)        0 2024-05-19 19:15:46.704006 omniblack_secret-0.0.2/omniblack.secret.egg-info/
+-rw-r--r--   0 terryp    (1000) terryp    (1000)      582 2024-05-19 19:15:46.000000 omniblack_secret-0.0.2/omniblack.secret.egg-info/PKG-INFO
+-rw-r--r--   0 terryp    (1000) terryp    (1000)      222 2024-05-19 19:15:46.000000 omniblack_secret-0.0.2/omniblack.secret.egg-info/SOURCES.txt
+-rw-r--r--   0 terryp    (1000) terryp    (1000)        1 2024-05-19 19:15:46.000000 omniblack_secret-0.0.2/omniblack.secret.egg-info/dependency_links.txt
+-rw-r--r--   0 terryp    (1000) terryp    (1000)       10 2024-05-19 19:15:46.000000 omniblack_secret-0.0.2/omniblack.secret.egg-info/top_level.txt
+-rw-r--r--   0 terryp    (1000) terryp    (1000)      675 2024-05-19 18:55:50.000000 omniblack_secret-0.0.2/pyproject.toml
+-rw-r--r--   0 terryp    (1000) terryp    (1000)    13166 2024-05-19 18:44:06.000000 omniblack_secret-0.0.2/secret.c
+-rw-r--r--   0 terryp    (1000) terryp    (1000)       38 2024-05-19 19:15:46.705006 omniblack_secret-0.0.2/setup.cfg
+-rw-r--r--   0 terryp    (1000) terryp    (1000)      224 2024-05-19 18:48:59.000000 omniblack_secret-0.0.2/setup.py
```

### Comparing `omniblack_secret-0.0.1/LICENSE` & `omniblack_secret-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `omniblack_secret-0.0.1/PKG-INFO` & `omniblack_secret-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniblack.secret
-Version: 0.0.1
+Version: 0.0.2
 Author-email: Terry Patterson <terryp@wegrok.net>
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
```

### Comparing `omniblack_secret-0.0.1/omniblack.secret.egg-info/PKG-INFO` & `omniblack_secret-0.0.2/omniblack.secret.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniblack.secret
-Version: 0.0.1
+Version: 0.0.2
 Author-email: Terry Patterson <terryp@wegrok.net>
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
```

### Comparing `omniblack_secret-0.0.1/pyproject.toml` & `omniblack_secret-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name='omniblack.secret'
-version='0.0.1'
+version='0.0.2'
 license={text='MIT License'}
 
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: MIT License',
     'Operating System :: POSIX :: Linux',
```

