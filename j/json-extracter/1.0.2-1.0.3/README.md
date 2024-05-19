# Comparing `tmp/json_extracter-1.0.2.tar.gz` & `tmp/json_extracter-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_extracter-1.0.2.tar", last modified: Fri May 17 22:56:25 2024, max compression
+gzip compressed data, was "json_extracter-1.0.3.tar", last modified: Sun May 19 23:13:11 2024, max compression
```

## Comparing `json_extracter-1.0.2.tar` & `json_extracter-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxr-x   0 edy       (1000) edy       (1000)        0 2024-05-17 22:56:25.753949 json_extracter-1.0.2/
--rw-rw-r--   0 edy       (1000) edy       (1000)     1054 2024-05-17 22:46:04.000000 json_extracter-1.0.2/LICENSE
--rw-r--r--   0 edy       (1000) edy       (1000)     1879 2024-05-17 22:56:25.753949 json_extracter-1.0.2/PKG-INFO
--rw-rw-r--   0 edy       (1000) edy       (1000)     1375 2024-05-17 22:53:19.000000 json_extracter-1.0.2/README.md
--rw-rw-r--   0 edy       (1000) edy       (1000)      484 2024-05-17 22:56:22.000000 json_extracter-1.0.2/pyproject.toml
--rw-rw-r--   0 edy       (1000) edy       (1000)       38 2024-05-17 22:56:25.753949 json_extracter-1.0.2/setup.cfg
-drwxrwxr-x   0 edy       (1000) edy       (1000)        0 2024-05-17 22:56:25.753949 json_extracter-1.0.2/src/
--rw-rw-r--   0 edy       (1000) edy       (1000)       60 2024-05-17 22:47:05.000000 json_extracter-1.0.2/src/__init__.py
-drwxrwxr-x   0 edy       (1000) edy       (1000)        0 2024-05-17 22:56:25.753949 json_extracter-1.0.2/src/json_extracter.egg-info/
--rw-r--r--   0 edy       (1000) edy       (1000)     1879 2024-05-17 22:56:25.000000 json_extracter-1.0.2/src/json_extracter.egg-info/PKG-INFO
--rw-rw-r--   0 edy       (1000) edy       (1000)      258 2024-05-17 22:56:25.000000 json_extracter-1.0.2/src/json_extracter.egg-info/SOURCES.txt
--rw-rw-r--   0 edy       (1000) edy       (1000)        1 2024-05-17 22:56:25.000000 json_extracter-1.0.2/src/json_extracter.egg-info/dependency_links.txt
--rw-rw-r--   0 edy       (1000) edy       (1000)       15 2024-05-17 22:56:25.000000 json_extracter-1.0.2/src/json_extracter.egg-info/top_level.txt
-drwxrwxr-x   0 edy       (1000) edy       (1000)        0 2024-05-17 22:56:25.753949 json_extracter-1.0.2/src/jsonx/
--rw-rw-r--   0 edy       (1000) edy       (1000)        0 2024-05-07 03:57:52.000000 json_extracter-1.0.2/src/jsonx/__init__.py
--rw-rw-r--   0 edy       (1000) edy       (1000)     1462 2024-05-17 22:46:57.000000 json_extracter-1.0.2/src/jsonx/modulo.py
+drwxrwxr-x   0 edy       (1000) edy       (1000)        0 2024-05-19 23:13:11.923997 json_extracter-1.0.3/
+-rw-rw-r--   0 edy       (1000) edy       (1000)     1054 2024-05-17 22:46:04.000000 json_extracter-1.0.3/LICENSE
+-rw-r--r--   0 edy       (1000) edy       (1000)     1879 2024-05-19 23:13:11.923997 json_extracter-1.0.3/PKG-INFO
+-rw-rw-r--   0 edy       (1000) edy       (1000)     1375 2024-05-17 22:53:19.000000 json_extracter-1.0.3/README.md
+-rw-rw-r--   0 edy       (1000) edy       (1000)      484 2024-05-19 23:12:33.000000 json_extracter-1.0.3/pyproject.toml
+-rw-rw-r--   0 edy       (1000) edy       (1000)       38 2024-05-19 23:13:11.923997 json_extracter-1.0.3/setup.cfg
+drwxrwxr-x   0 edy       (1000) edy       (1000)        0 2024-05-19 23:13:11.923997 json_extracter-1.0.3/src/
+-rw-rw-r--   0 edy       (1000) edy       (1000)       38 2024-05-19 23:11:59.000000 json_extracter-1.0.3/src/__init__.py
+drwxrwxr-x   0 edy       (1000) edy       (1000)        0 2024-05-19 23:13:11.923997 json_extracter-1.0.3/src/json_extracter.egg-info/
+-rw-r--r--   0 edy       (1000) edy       (1000)     1879 2024-05-19 23:13:11.000000 json_extracter-1.0.3/src/json_extracter.egg-info/PKG-INFO
+-rw-rw-r--   0 edy       (1000) edy       (1000)      236 2024-05-19 23:13:11.000000 json_extracter-1.0.3/src/json_extracter.egg-info/SOURCES.txt
+-rw-rw-r--   0 edy       (1000) edy       (1000)        1 2024-05-19 23:13:11.000000 json_extracter-1.0.3/src/json_extracter.egg-info/dependency_links.txt
+-rw-rw-r--   0 edy       (1000) edy       (1000)       15 2024-05-19 23:13:11.000000 json_extracter-1.0.3/src/json_extracter.egg-info/top_level.txt
+drwxrwxr-x   0 edy       (1000) edy       (1000)        0 2024-05-19 23:13:11.923997 json_extracter-1.0.3/src/jsonx/
+-rw-rw-r--   0 edy       (1000) edy       (1000)     1464 2024-05-19 23:04:33.000000 json_extracter-1.0.3/src/jsonx/modulo.py
```

### Comparing `json_extracter-1.0.2/LICENSE` & `json_extracter-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `json_extracter-1.0.2/PKG-INFO` & `json_extracter-1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json_extracter
-Version: 1.0.2
+Version: 1.0.3
 Summary: A small example package
 Author-email: edyMartin <edgar.edgarroman@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `json_extracter-1.0.2/README.md` & `json_extracter-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `json_extracter-1.0.2/src/json_extracter.egg-info/PKG-INFO` & `json_extracter-1.0.3/src/json_extracter.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json_extracter
-Version: 1.0.2
+Version: 1.0.3
 Summary: A small example package
 Author-email: edyMartin <edgar.edgarroman@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `json_extracter-1.0.2/src/jsonx/modulo.py` & `json_extracter-1.0.3/src/jsonx/modulo.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     if key_close_bracket < key_close_square_bracket:
         return open_text_clean[:key_close_square_bracket] + open_text_clean[key_close_square_bracket]
 
     if key_close_bracket > key_close_square_bracket:
         return open_text_clean[:key_close_bracket] + open_text_clean[key_close_bracket]
 
 
-def json_parse(txt):
+def json_extract(txt):
     txt_2 = str(txt.replace("\n", ""))
     text = re.sub(r'\s+', '', txt_2)
 
     # when open is {
     key_open_bracket = text.find("{")
 
     # when open is [
```

