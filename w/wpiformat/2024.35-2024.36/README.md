# Comparing `tmp/wpiformat-2024.35.tar.gz` & `tmp/wpiformat-2024.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wpiformat-2024.35.tar", last modified: Wed May  8 22:14:59 2024, max compression
+gzip compressed data, was "wpiformat-2024.36.tar", last modified: Mon May 20 20:01:51 2024, max compression
```

## Comparing `wpiformat-2024.35.tar` & `wpiformat-2024.36.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:14:59.763043 wpiformat-2024.35/
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-08 22:14:54.000000 wpiformat-2024.35/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-05-08 22:14:59.763043 wpiformat-2024.35/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-05-08 22:14:54.000000 wpiformat-2024.35/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-08 22:14:54.000000 wpiformat-2024.35/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 22:14:59.763043 wpiformat-2024.35/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:14:59.755044 wpiformat-2024.35/wpiformat/
--rw-r--r--   0 runner    (1001) docker     (127)    18048 2024-05-08 22:14:54.000000 wpiformat-2024.35/wpiformat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-08 22:14:54.000000 wpiformat-2024.35/wpiformat/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-05-08 22:14:54.000000 wpiformat-2024.35/wpiformat/bracecomment.py
--rw-r--r--   0 runner    (1001) docker     (127)     7217 2024-05-08 22:14:54.000000 wpiformat-2024.35/wpiformat/cidentlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-08 22:14:54.000000 wpiformat-2024.35/wpiformat/clangformat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-08 22:14:54.000000 wpiformat-2024.35/wpiformat/clangtidy.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-08 22:14:54.000000 wpiformat-2024.35/wpiformat/cmakeformat.py
--rw-r--r--   0 runner    (1001) docker     (127)     7325 2024-05-08 22:14:54.000000 wpiformat-2024.35/wpiformat/config.py
--rw-r--r--   0 runner    (1001) docker     (127)   144327 2024-05-08 22:14:54.000000 wpiformat-2024.35/wpiformat/cpplint.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-08 22:14:54.000000 wpiformat-2024.35/wpiformat/eofnewline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-05-08 22:14:54.000000 wpiformat-2024.35/wpiformat/gtestname.py
--rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-05-08 22:14:54.000000 wpiformat-2024.35/wpiformat/includeguard.py
--rw-r--r--   0 runner    (1001) docker     (127)    16396 2024-05-08 22:14:54.000000 wpiformat-2024.35/wpiformat/includeorder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-08 22:14:54.000000 wpiformat-2024.35/wpiformat/javaclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-05-08 22:14:54.000000 wpiformat-2024.35/wpiformat/jni.py
--rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-05-08 22:14:54.000000 wpiformat-2024.35/wpiformat/licenseupdate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-08 22:14:54.000000 wpiformat-2024.35/wpiformat/lint.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-08 22:14:54.000000 wpiformat-2024.35/wpiformat/pyformat.py
--rw-r--r--   0 runner    (1001) docker     (127)    12685 2024-05-08 22:14:54.000000 wpiformat-2024.35/wpiformat/stdlib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-08 22:14:54.000000 wpiformat-2024.35/wpiformat/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:14:59.759044 wpiformat-2024.35/wpiformat/test/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-08 22:14:54.000000 wpiformat-2024.35/wpiformat/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-05-08 22:14:54.000000 wpiformat-2024.35/wpiformat/test/test_bracecomment.py
--rw-r--r--   0 runner    (1001) docker     (127)    12499 2024-05-08 22:14:54.000000 wpiformat-2024.35/wpiformat/test/test_cidentlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-08 22:14:54.000000 wpiformat-2024.35/wpiformat/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-08 22:14:54.000000 wpiformat-2024.35/wpiformat/test/test_eofnewline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-08 22:14:54.000000 wpiformat-2024.35/wpiformat/test/test_gtestname.py
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-08 22:14:54.000000 wpiformat-2024.35/wpiformat/test/test_includeguard.py
--rw-r--r--   0 runner    (1001) docker     (127)    23206 2024-05-08 22:14:54.000000 wpiformat-2024.35/wpiformat/test/test_includeorder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-05-08 22:14:54.000000 wpiformat-2024.35/wpiformat/test/test_javaclass.py
--rw-r--r--   0 runner    (1001) docker     (127)    29622 2024-05-08 22:14:54.000000 wpiformat-2024.35/wpiformat/test/test_jni.py
--rw-r--r--   0 runner    (1001) docker     (127)    13433 2024-05-08 22:14:54.000000 wpiformat-2024.35/wpiformat/test/test_licenseupdate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-05-08 22:14:54.000000 wpiformat-2024.35/wpiformat/test/test_stdlib.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-05-08 22:14:54.000000 wpiformat-2024.35/wpiformat/test/test_tasktest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-08 22:14:54.000000 wpiformat-2024.35/wpiformat/test/test_usingdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-08 22:14:54.000000 wpiformat-2024.35/wpiformat/test/test_usingnamespacestd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-08 22:14:54.000000 wpiformat-2024.35/wpiformat/test/test_whitespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-08 22:14:54.000000 wpiformat-2024.35/wpiformat/usingdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-08 22:14:54.000000 wpiformat-2024.35/wpiformat/usingnamespacestd.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-08 22:14:54.000000 wpiformat-2024.35/wpiformat/version.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-08 22:14:54.000000 wpiformat-2024.35/wpiformat/whitespace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:14:59.759044 wpiformat-2024.35/wpiformat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-05-08 22:14:59.000000 wpiformat-2024.35/wpiformat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-08 22:14:59.000000 wpiformat-2024.35/wpiformat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 22:14:59.000000 wpiformat-2024.35/wpiformat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-08 22:14:59.000000 wpiformat-2024.35/wpiformat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-08 22:14:59.000000 wpiformat-2024.35/wpiformat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 22:14:59.000000 wpiformat-2024.35/wpiformat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:01:51.041997 wpiformat-2024.36/
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-20 20:01:45.000000 wpiformat-2024.36/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-05-20 20:01:51.041997 wpiformat-2024.36/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-05-20 20:01:45.000000 wpiformat-2024.36/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-20 20:01:45.000000 wpiformat-2024.36/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 20:01:51.041997 wpiformat-2024.36/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:01:51.033997 wpiformat-2024.36/wpiformat/
+-rw-r--r--   0 runner    (1001) docker     (127)    18048 2024-05-20 20:01:45.000000 wpiformat-2024.36/wpiformat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-20 20:01:45.000000 wpiformat-2024.36/wpiformat/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-05-20 20:01:45.000000 wpiformat-2024.36/wpiformat/bracecomment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7217 2024-05-20 20:01:45.000000 wpiformat-2024.36/wpiformat/cidentlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-20 20:01:45.000000 wpiformat-2024.36/wpiformat/clangformat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-20 20:01:45.000000 wpiformat-2024.36/wpiformat/clangtidy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-20 20:01:45.000000 wpiformat-2024.36/wpiformat/cmakeformat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7325 2024-05-20 20:01:45.000000 wpiformat-2024.36/wpiformat/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)   144327 2024-05-20 20:01:45.000000 wpiformat-2024.36/wpiformat/cpplint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-20 20:01:45.000000 wpiformat-2024.36/wpiformat/eofnewline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-05-20 20:01:45.000000 wpiformat-2024.36/wpiformat/gtestname.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-05-20 20:01:45.000000 wpiformat-2024.36/wpiformat/includeguard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16396 2024-05-20 20:01:45.000000 wpiformat-2024.36/wpiformat/includeorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-20 20:01:45.000000 wpiformat-2024.36/wpiformat/javaclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-05-20 20:01:45.000000 wpiformat-2024.36/wpiformat/jni.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-05-20 20:01:45.000000 wpiformat-2024.36/wpiformat/licenseupdate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-20 20:01:45.000000 wpiformat-2024.36/wpiformat/lint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-20 20:01:45.000000 wpiformat-2024.36/wpiformat/pyformat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12685 2024-05-20 20:01:45.000000 wpiformat-2024.36/wpiformat/stdlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-20 20:01:45.000000 wpiformat-2024.36/wpiformat/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:01:51.037997 wpiformat-2024.36/wpiformat/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-20 20:01:45.000000 wpiformat-2024.36/wpiformat/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-05-20 20:01:45.000000 wpiformat-2024.36/wpiformat/test/test_bracecomment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12499 2024-05-20 20:01:45.000000 wpiformat-2024.36/wpiformat/test/test_cidentlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-20 20:01:45.000000 wpiformat-2024.36/wpiformat/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-20 20:01:45.000000 wpiformat-2024.36/wpiformat/test/test_eofnewline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-20 20:01:45.000000 wpiformat-2024.36/wpiformat/test/test_gtestname.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-20 20:01:45.000000 wpiformat-2024.36/wpiformat/test/test_includeguard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23206 2024-05-20 20:01:45.000000 wpiformat-2024.36/wpiformat/test/test_includeorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-05-20 20:01:45.000000 wpiformat-2024.36/wpiformat/test/test_javaclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29622 2024-05-20 20:01:45.000000 wpiformat-2024.36/wpiformat/test/test_jni.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13433 2024-05-20 20:01:45.000000 wpiformat-2024.36/wpiformat/test/test_licenseupdate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-05-20 20:01:45.000000 wpiformat-2024.36/wpiformat/test/test_stdlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-05-20 20:01:45.000000 wpiformat-2024.36/wpiformat/test/test_tasktest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-20 20:01:45.000000 wpiformat-2024.36/wpiformat/test/test_usingdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-20 20:01:45.000000 wpiformat-2024.36/wpiformat/test/test_usingnamespacestd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-20 20:01:45.000000 wpiformat-2024.36/wpiformat/test/test_whitespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-20 20:01:45.000000 wpiformat-2024.36/wpiformat/usingdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-20 20:01:45.000000 wpiformat-2024.36/wpiformat/usingnamespacestd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-20 20:01:45.000000 wpiformat-2024.36/wpiformat/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-20 20:01:45.000000 wpiformat-2024.36/wpiformat/whitespace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:01:51.041997 wpiformat-2024.36/wpiformat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-05-20 20:01:51.000000 wpiformat-2024.36/wpiformat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-20 20:01:51.000000 wpiformat-2024.36/wpiformat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 20:01:51.000000 wpiformat-2024.36/wpiformat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-20 20:01:51.000000 wpiformat-2024.36/wpiformat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-20 20:01:51.000000 wpiformat-2024.36/wpiformat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 20:01:51.000000 wpiformat-2024.36/wpiformat.egg-info/top_level.txt
```

### Comparing `wpiformat-2024.35/LICENSE.txt` & `wpiformat-2024.36/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wpiformat-2024.35/PKG-INFO` & `wpiformat-2024.36/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wpiformat
-Version: 2024.35
+Version: 2024.36
 Summary: Linters and formatters for ensuring WPILib's source code conforms to its style guide
 Maintainer-email: Tyler Veness <calcmogul@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/wpilibsuite/styleguide
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `wpiformat-2024.35/README.rst` & `wpiformat-2024.36/README.rst`

 * *Files identical despite different names*

### Comparing `wpiformat-2024.35/pyproject.toml` & `wpiformat-2024.36/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wpiformat-2024.35/wpiformat/__init__.py` & `wpiformat-2024.36/wpiformat/__init__.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2024.35/wpiformat/bracecomment.py` & `wpiformat-2024.36/wpiformat/bracecomment.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2024.35/wpiformat/cidentlist.py` & `wpiformat-2024.36/wpiformat/cidentlist.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2024.35/wpiformat/clangformat.py` & `wpiformat-2024.36/wpiformat/clangformat.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2024.35/wpiformat/clangtidy.py` & `wpiformat-2024.36/wpiformat/clangtidy.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2024.35/wpiformat/cmakeformat.py` & `wpiformat-2024.36/wpiformat/cmakeformat.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2024.35/wpiformat/config.py` & `wpiformat-2024.36/wpiformat/config.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2024.35/wpiformat/cpplint.py` & `wpiformat-2024.36/wpiformat/cpplint.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2024.35/wpiformat/gtestname.py` & `wpiformat-2024.36/wpiformat/gtestname.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2024.35/wpiformat/includeguard.py` & `wpiformat-2024.36/wpiformat/includeguard.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2024.35/wpiformat/includeorder.py` & `wpiformat-2024.36/wpiformat/includeorder.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2024.35/wpiformat/javaclass.py` & `wpiformat-2024.36/wpiformat/javaclass.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2024.35/wpiformat/jni.py` & `wpiformat-2024.36/wpiformat/jni.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2024.35/wpiformat/licenseupdate.py` & `wpiformat-2024.36/wpiformat/licenseupdate.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2024.35/wpiformat/lint.py` & `wpiformat-2024.36/wpiformat/lint.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2024.35/wpiformat/pyformat.py` & `wpiformat-2024.36/wpiformat/pyformat.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2024.35/wpiformat/stdlib.py` & `wpiformat-2024.36/wpiformat/stdlib.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2024.35/wpiformat/task.py` & `wpiformat-2024.36/wpiformat/task.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2024.35/wpiformat/test/test_bracecomment.py` & `wpiformat-2024.36/wpiformat/test/test_bracecomment.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2024.35/wpiformat/test/test_cidentlist.py` & `wpiformat-2024.36/wpiformat/test/test_cidentlist.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2024.35/wpiformat/test/test_config.py` & `wpiformat-2024.36/wpiformat/test/test_config.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2024.35/wpiformat/test/test_eofnewline.py` & `wpiformat-2024.36/wpiformat/test/test_eofnewline.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2024.35/wpiformat/test/test_gtestname.py` & `wpiformat-2024.36/wpiformat/test/test_gtestname.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2024.35/wpiformat/test/test_includeguard.py` & `wpiformat-2024.36/wpiformat/test/test_includeguard.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2024.35/wpiformat/test/test_includeorder.py` & `wpiformat-2024.36/wpiformat/test/test_includeorder.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2024.35/wpiformat/test/test_javaclass.py` & `wpiformat-2024.36/wpiformat/test/test_javaclass.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2024.35/wpiformat/test/test_jni.py` & `wpiformat-2024.36/wpiformat/test/test_jni.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2024.35/wpiformat/test/test_licenseupdate.py` & `wpiformat-2024.36/wpiformat/test/test_licenseupdate.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2024.35/wpiformat/test/test_stdlib.py` & `wpiformat-2024.36/wpiformat/test/test_stdlib.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2024.35/wpiformat/test/test_tasktest.py` & `wpiformat-2024.36/wpiformat/test/test_tasktest.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2024.35/wpiformat/test/test_usingdeclaration.py` & `wpiformat-2024.36/wpiformat/test/test_usingdeclaration.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2024.35/wpiformat/test/test_usingnamespacestd.py` & `wpiformat-2024.36/wpiformat/test/test_usingnamespacestd.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2024.35/wpiformat/test/test_whitespace.py` & `wpiformat-2024.36/wpiformat/test/test_whitespace.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2024.35/wpiformat/usingdeclaration.py` & `wpiformat-2024.36/wpiformat/usingdeclaration.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2024.35/wpiformat/usingnamespacestd.py` & `wpiformat-2024.36/wpiformat/usingnamespacestd.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2024.35/wpiformat/version.py` & `wpiformat-2024.36/wpiformat/version.py`

 * *Files identical despite different names*

### Comparing `wpiformat-2024.35/wpiformat.egg-info/PKG-INFO` & `wpiformat-2024.36/wpiformat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wpiformat
-Version: 2024.35
+Version: 2024.36
 Summary: Linters and formatters for ensuring WPILib's source code conforms to its style guide
 Maintainer-email: Tyler Veness <calcmogul@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/wpilibsuite/styleguide
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `wpiformat-2024.35/wpiformat.egg-info/SOURCES.txt` & `wpiformat-2024.36/wpiformat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

