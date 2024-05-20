# Comparing `tmp/markdown_convert-1.1.8.tar.gz` & `tmp/markdown_convert-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown_convert-1.1.8.tar", max compression
+gzip compressed data, was "markdown_convert-1.1.9.tar", max compression
```

## Comparing `markdown_convert-1.1.8.tar` & `markdown_convert-1.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    18092 2023-10-23 17:37:06.761873 markdown_convert-1.1.8/LICENSE
--rw-r--r--   0        0        0     2452 2024-04-18 14:09:49.066892 markdown_convert-1.1.8/README.md
--rw-r--r--   0        0        0      213 2024-04-10 10:59:42.869680 markdown_convert-1.1.8/markdown_convert/__init__.py
--rwxr-xr-x   0        0        0     2815 2024-04-09 12:12:31.637276 markdown_convert-1.1.8/markdown_convert/__main__.py
--rw-r--r--   0        0        0     4935 2024-04-08 12:12:18.468503 markdown_convert-1.1.8/markdown_convert/code.css
--rw-r--r--   0        0        0     5631 2024-05-17 15:38:38.453499 markdown_convert-1.1.8/markdown_convert/default.css
--rw-r--r--   0        0        0       65 2024-04-10 10:59:51.693837 markdown_convert-1.1.8/markdown_convert/modules/__init__.py
--rw-r--r--   0        0        0      429 2024-04-10 20:54:32.247070 markdown_convert-1.1.8/markdown_convert/modules/constants.py
--rw-r--r--   0        0        0     5711 2024-04-16 12:03:21.481233 markdown_convert-1.1.8/markdown_convert/modules/convert.py
--rw-r--r--   0        0        0     2258 2024-04-09 12:12:32.309271 markdown_convert-1.1.8/markdown_convert/modules/resources.py
--rw-r--r--   0        0        0      655 2024-04-10 10:56:40.081145 markdown_convert-1.1.8/markdown_convert/modules/utils.py
--rw-r--r--   0        0        0     1487 2024-04-08 14:48:42.000577 markdown_convert-1.1.8/markdown_convert/modules/validate.py
--rw-r--r--   0        0        0      680 2024-05-17 15:38:55.353788 markdown_convert-1.1.8/pyproject.toml
--rw-r--r--   0        0        0     3356 1970-01-01 00:00:00.000000 markdown_convert-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-10-23 17:37:06.761873 markdown_convert-1.1.9/LICENSE
+-rw-r--r--   0        0        0     2452 2024-04-18 14:09:49.066892 markdown_convert-1.1.9/README.md
+-rw-r--r--   0        0        0      213 2024-04-10 10:59:42.869680 markdown_convert-1.1.9/markdown_convert/__init__.py
+-rwxr-xr-x   0        0        0     2815 2024-04-09 12:12:31.637276 markdown_convert-1.1.9/markdown_convert/__main__.py
+-rw-r--r--   0        0        0     4935 2024-04-08 12:12:18.468503 markdown_convert-1.1.9/markdown_convert/code.css
+-rw-r--r--   0        0        0     5680 2024-05-20 09:30:39.806398 markdown_convert-1.1.9/markdown_convert/default.css
+-rw-r--r--   0        0        0       65 2024-04-10 10:59:51.693837 markdown_convert-1.1.9/markdown_convert/modules/__init__.py
+-rw-r--r--   0        0        0      429 2024-04-10 20:54:32.247070 markdown_convert-1.1.9/markdown_convert/modules/constants.py
+-rw-r--r--   0        0        0     5711 2024-04-16 12:03:21.481233 markdown_convert-1.1.9/markdown_convert/modules/convert.py
+-rw-r--r--   0        0        0     2258 2024-04-09 12:12:32.309271 markdown_convert-1.1.9/markdown_convert/modules/resources.py
+-rw-r--r--   0        0        0      655 2024-04-10 10:56:40.081145 markdown_convert-1.1.9/markdown_convert/modules/utils.py
+-rw-r--r--   0        0        0     1487 2024-04-08 14:48:42.000577 markdown_convert-1.1.9/markdown_convert/modules/validate.py
+-rw-r--r--   0        0        0      680 2024-05-20 10:11:09.842565 markdown_convert-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3356 1970-01-01 00:00:00.000000 markdown_convert-1.1.9/PKG-INFO
```

### Comparing `markdown_convert-1.1.8/LICENSE` & `markdown_convert-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.1.8/README.md` & `markdown_convert-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.1.8/markdown_convert/__main__.py` & `markdown_convert-1.1.9/markdown_convert/__main__.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.1.8/markdown_convert/code.css` & `markdown_convert-1.1.9/markdown_convert/code.css`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.1.8/markdown_convert/default.css` & `markdown_convert-1.1.9/markdown_convert/default.css`

 * *Files 2% similar despite different names*

```diff
@@ -272,10 +272,19 @@
   page-break-after: always;
 }
 
 .pagebreak + * {
   margin-top: 0;
 }
 
-* {
+li,
+table,
+blockquote,
+code,
+p,
+h1,
+h2,
+h3,
+h4,
+h5 {
   page-break-inside: avoid;
 }
```

### Comparing `markdown_convert-1.1.8/markdown_convert/modules/convert.py` & `markdown_convert-1.1.9/markdown_convert/modules/convert.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.1.8/markdown_convert/modules/resources.py` & `markdown_convert-1.1.9/markdown_convert/modules/resources.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.1.8/markdown_convert/modules/utils.py` & `markdown_convert-1.1.9/markdown_convert/modules/utils.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.1.8/markdown_convert/modules/validate.py` & `markdown_convert-1.1.9/markdown_convert/modules/validate.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.1.8/pyproject.toml` & `markdown_convert-1.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "markdown_convert"
-version = "1.1.8"
+version = "1.1.9"
 description = "Convert Markdown files to PDF from your command line."
 authors = ["Julio Cabria <juliocabria@tutanota.com>"]
 license = "GPL-2.0-only"
 readme = "README.md"
 homepage = "https://github.com/Julynx/markdown_convert"
 include = ["markdown_convert/default.css", "markdown_convert/code.css"]
```

### Comparing `markdown_convert-1.1.8/PKG-INFO` & `markdown_convert-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdown_convert
-Version: 1.1.8
+Version: 1.1.9
 Summary: Convert Markdown files to PDF from your command line.
 Home-page: https://github.com/Julynx/markdown_convert
 License: GPL-2.0-only
 Author: Julio Cabria
 Author-email: juliocabria@tutanota.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

