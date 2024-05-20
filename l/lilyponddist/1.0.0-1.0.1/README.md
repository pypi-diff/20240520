# Comparing `tmp/lilyponddist-1.0.0.tar.gz` & `tmp/lilyponddist-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lilyponddist-1.0.0.tar", last modified: Thu Apr 25 22:03:34 2024, max compression
+gzip compressed data, was "lilyponddist-1.0.1.tar", last modified: Mon May 20 21:29:07 2024, max compression
```

## Comparing `lilyponddist-1.0.0.tar` & `lilyponddist-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-25 22:03:34.434795 lilyponddist-1.0.0/
--rw-r--r--   0 em        (1000) em        (1000)     2079 2023-04-17 21:56:53.000000 lilyponddist-1.0.0/LICENSE
--rw-r--r--   0 em        (1000) em        (1000)     2510 2024-04-25 22:03:34.434795 lilyponddist-1.0.0/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)     2183 2024-04-22 11:07:32.000000 lilyponddist-1.0.0/README.rst
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-25 22:03:34.432795 lilyponddist-1.0.0/lilyponddist/
--rw-rw-r--   0 em        (1000) em        (1000)    19316 2024-04-22 10:34:24.000000 lilyponddist-1.0.0/lilyponddist/__init__.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-25 22:03:34.433795 lilyponddist-1.0.0/lilyponddist.egg-info/
--rw-r--r--   0 em        (1000) em        (1000)     2510 2024-04-25 22:03:34.000000 lilyponddist-1.0.0/lilyponddist.egg-info/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)      245 2024-04-25 22:03:34.000000 lilyponddist-1.0.0/lilyponddist.egg-info/SOURCES.txt
--rw-rw-r--   0 em        (1000) em        (1000)        1 2024-04-25 22:03:34.000000 lilyponddist-1.0.0/lilyponddist.egg-info/dependency_links.txt
--rw-rw-r--   0 em        (1000) em        (1000)       20 2024-04-25 22:03:34.000000 lilyponddist-1.0.0/lilyponddist.egg-info/requires.txt
--rw-rw-r--   0 em        (1000) em        (1000)       13 2024-04-25 22:03:34.000000 lilyponddist-1.0.0/lilyponddist.egg-info/top_level.txt
--rw-rw-r--   0 em        (1000) em        (1000)       38 2024-04-25 22:03:34.434795 lilyponddist-1.0.0/setup.cfg
--rwxrwxr-x   0 em        (1000) em        (1000)      721 2023-12-19 01:17:01.000000 lilyponddist-1.0.0/setup.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-25 22:03:34.433795 lilyponddist-1.0.0/test/
--rw-r--r--   0 em        (1000) em        (1000)      328 2024-02-19 10:20:09.000000 lilyponddist-1.0.0/test/test1.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-05-20 21:29:07.909459 lilyponddist-1.0.1/
+-rw-r--r--   0 em        (1000) em        (1000)     2079 2023-04-17 21:56:53.000000 lilyponddist-1.0.1/LICENSE
+-rw-r--r--   0 em        (1000) em        (1000)     2510 2024-05-20 21:29:07.909459 lilyponddist-1.0.1/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)     2183 2024-04-22 11:07:32.000000 lilyponddist-1.0.1/README.rst
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-05-20 21:29:07.907459 lilyponddist-1.0.1/lilyponddist/
+-rw-rw-r--   0 em        (1000) em        (1000)    19414 2024-05-20 21:26:20.000000 lilyponddist-1.0.1/lilyponddist/__init__.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-05-20 21:29:07.909459 lilyponddist-1.0.1/lilyponddist.egg-info/
+-rw-r--r--   0 em        (1000) em        (1000)     2510 2024-05-20 21:29:07.000000 lilyponddist-1.0.1/lilyponddist.egg-info/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)      245 2024-05-20 21:29:07.000000 lilyponddist-1.0.1/lilyponddist.egg-info/SOURCES.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        1 2024-05-20 21:29:07.000000 lilyponddist-1.0.1/lilyponddist.egg-info/dependency_links.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       20 2024-05-20 21:29:07.000000 lilyponddist-1.0.1/lilyponddist.egg-info/requires.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       13 2024-05-20 21:29:07.000000 lilyponddist-1.0.1/lilyponddist.egg-info/top_level.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       38 2024-05-20 21:29:07.909459 lilyponddist-1.0.1/setup.cfg
+-rwxrwxr-x   0 em        (1000) em        (1000)      721 2023-12-19 01:17:01.000000 lilyponddist-1.0.1/setup.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-05-20 21:29:07.908459 lilyponddist-1.0.1/test/
+-rw-r--r--   0 em        (1000) em        (1000)      328 2024-02-19 10:20:09.000000 lilyponddist-1.0.1/test/test1.py
```

### Comparing `lilyponddist-1.0.0/LICENSE` & `lilyponddist-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lilyponddist-1.0.0/PKG-INFO` & `lilyponddist-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lilyponddist
-Version: 1.0.0
+Version: 1.0.1
 Summary: Distribute lilypond as a pypi package
 Home-page: https://github.com/gesellkammer/lilyponddist
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 Requires-Dist: appdirs
 Requires-Dist: progressbar
```

### Comparing `lilyponddist-1.0.0/README.rst` & `lilyponddist-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `lilyponddist-1.0.0/lilyponddist/__init__.py` & `lilyponddist-1.0.1/lilyponddist/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 import sys
 
 
-__VERSION__ = "1.0.0"
+__VERSION__ = "1.0.1"
 
 
 if __name__ == '__main__':
     if len(sys.argv) > 1 and sys.argv[1] == '--version':
         print(__VERSION__)
     sys.exit(0)
 
@@ -499,14 +499,18 @@
         return 'lilypond.exe'
     else:
         return 'lilypond'
 
 
 def _find_lilypond(version='') -> Path | None:
     installed = installed_versions()
+    if not installed:
+        logger.debug("No lilypond installation found")
+        return None
+
     if version:
         versiontup = _parse_versionstr(version)
     else:
         versiontup = max(installed.keys())
     root = installed.get(versiontup)
     if not root:
         logger.debug("No lilypond installation found for version {versiontup}")
```

### Comparing `lilyponddist-1.0.0/lilyponddist.egg-info/PKG-INFO` & `lilyponddist-1.0.1/lilyponddist.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lilyponddist
-Version: 1.0.0
+Version: 1.0.1
 Summary: Distribute lilypond as a pypi package
 Home-page: https://github.com/gesellkammer/lilyponddist
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 Requires-Dist: appdirs
 Requires-Dist: progressbar
```

### Comparing `lilyponddist-1.0.0/setup.py` & `lilyponddist-1.0.1/setup.py`

 * *Files identical despite different names*

