# Comparing `tmp/imas_tools-0.3.0.tar.gz` & `tmp/imas_tools-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imas_tools-0.3.0.tar", max compression
+gzip compressed data, was "imas_tools-0.4.0.tar", max compression
```

## Comparing `imas_tools-0.3.0.tar` & `imas_tools-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,11 @@
--rw-r--r--   0        0        0        0 2024-04-13 09:02:36.035606 imas_tools-0.3.0/imas_tools/__init__.py
--rw-r--r--   0        0        0        0 2024-04-15 13:36:34.820658 imas_tools-0.3.0/imas_tools/portal/__init__.py
--rw-r--r--   0        0        0     4772 2024-04-19 15:23:32.617350 imas_tools-0.3.0/imas_tools/portal/article.py
--rw-r--r--   0        0        0     2363 2024-04-18 15:56:10.247192 imas_tools-0.3.0/imas_tools/portal/interfaces.py
--rw-r--r--   0        0        0     4126 2024-04-13 12:27:59.670781 imas_tools-0.3.0/imas_tools/recochoku.py
--rw-r--r--   0        0        0      465 2024-04-19 15:24:31.529598 imas_tools-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-13 09:02:36.044152 imas_tools-0.3.0/README.md
--rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 imas_tools-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-13 09:02:36.035606 imas_tools-0.4.0/imas_tools/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 13:36:34.820658 imas_tools-0.4.0/imas_tools/portal/__init__.py
+-rw-r--r--   0        0        0     4772 2024-04-19 15:23:32.617350 imas_tools-0.4.0/imas_tools/portal/article.py
+-rw-r--r--   0        0        0     2363 2024-04-18 15:56:10.247192 imas_tools-0.4.0/imas_tools/portal/interfaces.py
+-rw-r--r--   0        0        0     4126 2024-04-13 12:27:59.670781 imas_tools-0.4.0/imas_tools/recochoku.py
+-rw-r--r--   0        0        0        0 2024-05-20 16:09:08.603881 imas_tools-0.4.0/imas_tools/story/__init__.py
+-rw-r--r--   0        0        0      579 2024-05-20 16:09:28.637319 imas_tools-0.4.0/imas_tools/story/adapter.py
+-rw-r--r--   0        0        0     3061 2024-05-20 16:08:35.466738 imas_tools-0.4.0/imas_tools/story/gakuen_parser.py
+-rw-r--r--   0        0        0      465 2024-05-20 16:17:21.451486 imas_tools-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-13 09:02:36.044152 imas_tools-0.4.0/README.md
+-rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 imas_tools-0.4.0/PKG-INFO
```

### Comparing `imas_tools-0.3.0/imas_tools/portal/article.py` & `imas_tools-0.4.0/imas_tools/portal/article.py`

 * *Files identical despite different names*

### Comparing `imas_tools-0.3.0/imas_tools/portal/interfaces.py` & `imas_tools-0.4.0/imas_tools/portal/interfaces.py`

 * *Files identical despite different names*

### Comparing `imas_tools-0.3.0/imas_tools/recochoku.py` & `imas_tools-0.4.0/imas_tools/recochoku.py`

 * *Files identical despite different names*

### Comparing `imas_tools-0.3.0/PKG-INFO` & `imas_tools-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imas-tools
-Version: 0.3.0
+Version: 0.4.0
 Summary: 
 Author: darwintree
 Author-email: 17946284+darwintree@users.noreply.github.com
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

