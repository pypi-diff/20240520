# Comparing `tmp/dropboxdrivefs-1.3.1.tar.gz` & `tmp/dropboxdrivefs-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dropboxdrivefs-1.3.1.tar", last modified: Fri Jan 28 11:12:04 2022, max compression
+gzip compressed data, was "dropboxdrivefs-1.4.0.tar", last modified: Mon May 20 18:59:11 2024, max compression
```

## Comparing `dropboxdrivefs-1.3.1.tar` & `dropboxdrivefs-1.4.0.tar`

### file list

```diff
@@ -1,19 +1,17 @@
-drwxrwxr-x   0 chaputmarine  (1000) chaputmarine  (1000)        0 2022-01-28 11:12:04.000000 dropboxdrivefs-1.3.1/
--rw-rw-r--   0 chaputmarine  (1000) chaputmarine  (1000)     1528 2022-01-24 17:34:25.000000 dropboxdrivefs-1.3.1/LICENSE
--rw-rw-r--   0 chaputmarine  (1000) chaputmarine  (1000)       35 2022-01-24 17:34:25.000000 dropboxdrivefs-1.3.1/MANIFEST.in
--rw-rw-r--   0 chaputmarine  (1000) chaputmarine  (1000)     1861 2022-01-28 11:12:04.000000 dropboxdrivefs-1.3.1/PKG-INFO
--rw-rw-r--   0 chaputmarine  (1000) chaputmarine  (1000)      889 2022-01-24 17:34:25.000000 dropboxdrivefs-1.3.1/README.md
-drwxrwxr-x   0 chaputmarine  (1000) chaputmarine  (1000)        0 2022-01-28 11:12:04.000000 dropboxdrivefs-1.3.1/dropboxdrivefs/
--rw-rw-r--   0 chaputmarine  (1000) chaputmarine  (1000)       57 2022-01-24 17:34:25.000000 dropboxdrivefs-1.3.1/dropboxdrivefs/__init__.py
--rw-rw-r--   0 chaputmarine  (1000) chaputmarine  (1000)     6586 2022-01-24 17:34:25.000000 dropboxdrivefs-1.3.1/dropboxdrivefs/core.py
-drwxrwxr-x   0 chaputmarine  (1000) chaputmarine  (1000)        0 2022-01-28 11:12:04.000000 dropboxdrivefs-1.3.1/dropboxdrivefs.egg-info/
--rw-rw-r--   0 chaputmarine  (1000) chaputmarine  (1000)     1861 2022-01-28 11:12:04.000000 dropboxdrivefs-1.3.1/dropboxdrivefs.egg-info/PKG-INFO
--rw-rw-r--   0 chaputmarine  (1000) chaputmarine  (1000)      327 2022-01-28 11:12:04.000000 dropboxdrivefs-1.3.1/dropboxdrivefs.egg-info/SOURCES.txt
--rw-rw-r--   0 chaputmarine  (1000) chaputmarine  (1000)        1 2022-01-28 11:12:04.000000 dropboxdrivefs-1.3.1/dropboxdrivefs.egg-info/dependency_links.txt
--rw-rw-r--   0 chaputmarine  (1000) chaputmarine  (1000)        1 2022-01-24 17:34:46.000000 dropboxdrivefs-1.3.1/dropboxdrivefs.egg-info/not-zip-safe
--rw-rw-r--   0 chaputmarine  (1000) chaputmarine  (1000)       24 2022-01-28 11:12:04.000000 dropboxdrivefs-1.3.1/dropboxdrivefs.egg-info/requires.txt
--rw-rw-r--   0 chaputmarine  (1000) chaputmarine  (1000)       15 2022-01-28 11:12:04.000000 dropboxdrivefs-1.3.1/dropboxdrivefs.egg-info/top_level.txt
--rw-rw-r--   0 chaputmarine  (1000) chaputmarine  (1000)       38 2022-01-28 11:12:04.000000 dropboxdrivefs-1.3.1/setup.cfg
--rw-rw-r--   0 chaputmarine  (1000) chaputmarine  (1000)     1135 2022-01-28 11:12:02.000000 dropboxdrivefs-1.3.1/setup.py
-drwxrwxr-x   0 chaputmarine  (1000) chaputmarine  (1000)        0 2022-01-28 11:12:04.000000 dropboxdrivefs-1.3.1/test/
--rw-rw-r--   0 chaputmarine  (1000) chaputmarine  (1000)     3067 2022-01-24 17:34:25.000000 dropboxdrivefs-1.3.1/test/test.py
+drwxrwxr-x   0 marine    (1000) marine    (1000)        0 2024-05-20 18:59:11.564527 dropboxdrivefs-1.4.0/
+-rw-rw-r--   0 marine    (1000) marine    (1000)     1528 2024-01-18 18:26:56.000000 dropboxdrivefs-1.4.0/LICENSE
+-rw-rw-r--   0 marine    (1000) marine    (1000)       35 2024-01-18 18:26:56.000000 dropboxdrivefs-1.4.0/MANIFEST.in
+-rw-r--r--   0 marine    (1000) marine    (1000)     2221 2024-05-20 18:59:11.564527 dropboxdrivefs-1.4.0/PKG-INFO
+-rw-rw-r--   0 marine    (1000) marine    (1000)     1383 2024-01-18 18:26:56.000000 dropboxdrivefs-1.4.0/README.md
+drwxrwxr-x   0 marine    (1000) marine    (1000)        0 2024-05-20 18:59:11.564527 dropboxdrivefs-1.4.0/dropboxdrivefs/
+drwxrwxr-x   0 marine    (1000) marine    (1000)        0 2024-05-20 18:59:11.564527 dropboxdrivefs-1.4.0/dropboxdrivefs/dropboxdrivefs.egg-info/
+-rw-r--r--   0 marine    (1000) marine    (1000)     2221 2024-05-20 18:59:11.000000 dropboxdrivefs-1.4.0/dropboxdrivefs/dropboxdrivefs.egg-info/PKG-INFO
+-rw-rw-r--   0 marine    (1000) marine    (1000)      339 2024-05-20 18:59:11.000000 dropboxdrivefs-1.4.0/dropboxdrivefs/dropboxdrivefs.egg-info/SOURCES.txt
+-rw-rw-r--   0 marine    (1000) marine    (1000)        1 2024-05-20 18:59:11.000000 dropboxdrivefs-1.4.0/dropboxdrivefs/dropboxdrivefs.egg-info/dependency_links.txt
+-rw-rw-r--   0 marine    (1000) marine    (1000)       24 2024-05-20 18:59:11.000000 dropboxdrivefs-1.4.0/dropboxdrivefs/dropboxdrivefs.egg-info/requires.txt
+-rw-rw-r--   0 marine    (1000) marine    (1000)        1 2024-05-20 18:59:11.000000 dropboxdrivefs-1.4.0/dropboxdrivefs/dropboxdrivefs.egg-info/top_level.txt
+-rw-rw-r--   0 marine    (1000) marine    (1000)      963 2024-05-20 18:58:57.000000 dropboxdrivefs-1.4.0/pyproject.toml
+-rw-rw-r--   0 marine    (1000) marine    (1000)       38 2024-05-20 18:59:11.564527 dropboxdrivefs-1.4.0/setup.cfg
+drwxrwxr-x   0 marine    (1000) marine    (1000)        0 2024-05-20 18:59:11.564527 dropboxdrivefs-1.4.0/test/
+-rw-rw-r--   0 marine    (1000) marine    (1000)     5615 2024-05-20 18:38:25.000000 dropboxdrivefs-1.4.0/test/test.py
+-rw-rw-r--   0 marine    (1000) marine    (1000)     2990 2024-05-20 18:38:25.000000 dropboxdrivefs-1.4.0/test/test_copy.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dropboxdrivefs-1.3.1/LICENSE` & `dropboxdrivefs-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dropboxdrivefs-1.3.1/PKG-INFO` & `dropboxdrivefs-1.4.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,47 +1,62 @@
 Metadata-Version: 2.1
 Name: dropboxdrivefs
-Version: 1.3.1
+Version: 1.4.0
 Summary: Dropbox implementation for fsspec module
-Home-page: https://github.com/fsspec/dropboxdrivefs
-Author: Marine Chaput
-Author-email: marine.chaput@hotmail.fr
-License: BSD
-Description: # Description
-        
-        This package is one of the implementation available in the fsspec module. It can be used with alone, or dask and intake by indicating the  protocol in the path file:
-        ```
-        dropbox://file_path
-        ```
-        
-        It can also be used directly from the fsspec module to download and upload files in the github account.
-        
-        The upload part is using the dropbox API.
-        
-        The download part is using the dropbox API to create a temporary link and then used the already existing https implementation.
-        Caching (see fsspec module) is available in that case.
-        
-        Documentation of the fsspec module : https://github.com/intake/filesystem_spec/blob/master/docs/source/features.rst
-        
-        ## Install
-        
-        ```
-        pip install dropboxdrivefs
-        ```
-        
-        ## Thanks
-        
-        Thanks to martindurant and TomAugspurger for the help to developping this implementation
-        see info about the development: https://github.com/intake/filesystem_spec/pull/207
-        
-Platform: UNKNOWN
+Author-email: Marine Chaput <marine.chaput@hotmail.fr>
+License: BSD License
+Project-URL: Homepage, https://github.com/fsspec/dropboxdrivefs
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: fsspec
+Requires-Dist: requests
+Requires-Dist: dropbox
+
+# Description
+
+This package is one of the implementation available in the fsspec module. 
+
+It can be used alone, or dask and intake by indicating the  protocol in the path file:
+```
+dropbox://file_path
+```
+Small nicety : file_path in dropbox needs to start at the root "/folder1/folder2/etc." which means your path when using the
+protocol identifier should look like this : 
+```
+dropbox:///folder1/folder2/etc
+```
+Yes, with three /// ! What happen if not, for some reasons the dropbox api will remove everything before the first / 
+in the path keep only what is after.
+
+It can also be used directly from the fsspec module to download and upload files in the github account.
+
+The upload part is using the dropbox API.
+
+The download part is using the dropbox API to create a temporary link and then used the already existing webhdfs implementation.
+Caching (see fsspec module) is available in that case.
+
+Documentation of the fsspec module : https://github.com/intake/filesystem_spec/blob/master/docs/source/features.rst
+
+## Install
+
+```
+pip install dropboxdrivefs
+```
+
+### How to obtain your access token? 
+
+https://blogs.dropbox.com/developers/2014/05/generate-an-access-token-for-your-own-account/
+
+## Thanks
+
+Thanks to martindurant and TomAugspurger for the help to developping this implementation
+see info about the development: https://github.com/intake/filesystem_spec/pull/207
```

### Comparing `dropboxdrivefs-1.3.1/dropboxdrivefs.egg-info/PKG-INFO` & `dropboxdrivefs-1.4.0/dropboxdrivefs/dropboxdrivefs.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,47 +1,62 @@
 Metadata-Version: 2.1
 Name: dropboxdrivefs
-Version: 1.3.1
+Version: 1.4.0
 Summary: Dropbox implementation for fsspec module
-Home-page: https://github.com/fsspec/dropboxdrivefs
-Author: Marine Chaput
-Author-email: marine.chaput@hotmail.fr
-License: BSD
-Description: # Description
-        
-        This package is one of the implementation available in the fsspec module. It can be used with alone, or dask and intake by indicating the  protocol in the path file:
-        ```
-        dropbox://file_path
-        ```
-        
-        It can also be used directly from the fsspec module to download and upload files in the github account.
-        
-        The upload part is using the dropbox API.
-        
-        The download part is using the dropbox API to create a temporary link and then used the already existing https implementation.
-        Caching (see fsspec module) is available in that case.
-        
-        Documentation of the fsspec module : https://github.com/intake/filesystem_spec/blob/master/docs/source/features.rst
-        
-        ## Install
-        
-        ```
-        pip install dropboxdrivefs
-        ```
-        
-        ## Thanks
-        
-        Thanks to martindurant and TomAugspurger for the help to developping this implementation
-        see info about the development: https://github.com/intake/filesystem_spec/pull/207
-        
-Platform: UNKNOWN
+Author-email: Marine Chaput <marine.chaput@hotmail.fr>
+License: BSD License
+Project-URL: Homepage, https://github.com/fsspec/dropboxdrivefs
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: fsspec
+Requires-Dist: requests
+Requires-Dist: dropbox
+
+# Description
+
+This package is one of the implementation available in the fsspec module. 
+
+It can be used alone, or dask and intake by indicating the  protocol in the path file:
+```
+dropbox://file_path
+```
+Small nicety : file_path in dropbox needs to start at the root "/folder1/folder2/etc." which means your path when using the
+protocol identifier should look like this : 
+```
+dropbox:///folder1/folder2/etc
+```
+Yes, with three /// ! What happen if not, for some reasons the dropbox api will remove everything before the first / 
+in the path keep only what is after.
+
+It can also be used directly from the fsspec module to download and upload files in the github account.
+
+The upload part is using the dropbox API.
+
+The download part is using the dropbox API to create a temporary link and then used the already existing webhdfs implementation.
+Caching (see fsspec module) is available in that case.
+
+Documentation of the fsspec module : https://github.com/intake/filesystem_spec/blob/master/docs/source/features.rst
+
+## Install
+
+```
+pip install dropboxdrivefs
+```
+
+### How to obtain your access token? 
+
+https://blogs.dropbox.com/developers/2014/05/generate-an-access-token-for-your-own-account/
+
+## Thanks
+
+Thanks to martindurant and TomAugspurger for the help to developping this implementation
+see info about the development: https://github.com/intake/filesystem_spec/pull/207
```

