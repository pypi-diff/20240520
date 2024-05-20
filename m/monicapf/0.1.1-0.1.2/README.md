# Comparing `tmp/monicapf-0.1.1.tar.gz` & `tmp/monicapf-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monicapf-0.1.1.tar", last modified: Sun May 19 07:00:33 2024, max compression
+gzip compressed data, was "monicapf-0.1.2.tar", last modified: Sun May 19 07:53:07 2024, max compression
```

## Comparing `monicapf-0.1.1.tar` & `monicapf-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,16 @@
-drwxr-xr-x   0 bilol     (1000) bilol     (1000)        0 2024-05-19 07:00:33.731516 monicapf-0.1.1/
--rw-r--r--   0 bilol     (1000) bilol     (1000)     4337 2024-05-19 07:00:33.730516 monicapf-0.1.1/PKG-INFO
--rw-r--r--   0 bilol     (1000) bilol     (1000)     3678 2024-05-19 07:00:18.000000 monicapf-0.1.1/README.md
-drwxr-xr-x   0 bilol     (1000) bilol     (1000)        0 2024-05-19 07:00:33.729516 monicapf-0.1.1/monicapf.egg-info/
--rw-r--r--   0 bilol     (1000) bilol     (1000)     4337 2024-05-19 07:00:33.000000 monicapf-0.1.1/monicapf.egg-info/PKG-INFO
--rw-r--r--   0 bilol     (1000) bilol     (1000)      177 2024-05-19 07:00:33.000000 monicapf-0.1.1/monicapf.egg-info/SOURCES.txt
--rw-r--r--   0 bilol     (1000) bilol     (1000)        1 2024-05-19 07:00:33.000000 monicapf-0.1.1/monicapf.egg-info/dependency_links.txt
--rw-r--r--   0 bilol     (1000) bilol     (1000)      122 2024-05-19 07:00:33.000000 monicapf-0.1.1/monicapf.egg-info/requires.txt
--rw-r--r--   0 bilol     (1000) bilol     (1000)        1 2024-05-19 07:00:33.000000 monicapf-0.1.1/monicapf.egg-info/top_level.txt
--rw-r--r--   0 bilol     (1000) bilol     (1000)       38 2024-05-19 07:00:33.731516 monicapf-0.1.1/setup.cfg
--rw-r--r--   0 bilol     (1000) bilol     (1000)     3946 2024-05-19 07:00:09.000000 monicapf-0.1.1/setup.py
+drwxr-xr-x   0 bilol     (1000) bilol     (1000)        0 2024-05-19 07:53:07.829134 monicapf-0.1.2/
+-rw-r--r--   0 bilol     (1000) bilol     (1000)     4327 2024-05-19 07:53:07.825134 monicapf-0.1.2/PKG-INFO
+-rw-r--r--   0 bilol     (1000) bilol     (1000)     3668 2024-05-19 07:52:51.000000 monicapf-0.1.2/README.md
+drwxr-xr-x   0 bilol     (1000) bilol     (1000)        0 2024-05-19 07:53:07.821134 monicapf-0.1.2/monicapf/
+-rw-r--r--   0 bilol     (1000) bilol     (1000)        0 2024-05-19 07:52:48.000000 monicapf-0.1.2/monicapf/__init__.py
+-rw-r--r--   0 bilol     (1000) bilol     (1000)     3796 2024-05-17 14:48:32.000000 monicapf-0.1.2/monicapf/app.py
+-rw-r--r--   0 bilol     (1000) bilol     (1000)      686 2024-05-17 14:48:30.000000 monicapf-0.1.2/monicapf/middleware.py
+-rw-r--r--   0 bilol     (1000) bilol     (1000)      954 2024-05-17 14:48:29.000000 monicapf-0.1.2/monicapf/response.py
+drwxr-xr-x   0 bilol     (1000) bilol     (1000)        0 2024-05-19 07:53:07.824134 monicapf-0.1.2/monicapf.egg-info/
+-rw-r--r--   0 bilol     (1000) bilol     (1000)     4327 2024-05-19 07:53:07.000000 monicapf-0.1.2/monicapf.egg-info/PKG-INFO
+-rw-r--r--   0 bilol     (1000) bilol     (1000)      258 2024-05-19 07:53:07.000000 monicapf-0.1.2/monicapf.egg-info/SOURCES.txt
+-rw-r--r--   0 bilol     (1000) bilol     (1000)        1 2024-05-19 07:53:07.000000 monicapf-0.1.2/monicapf.egg-info/dependency_links.txt
+-rw-r--r--   0 bilol     (1000) bilol     (1000)      122 2024-05-19 07:53:07.000000 monicapf-0.1.2/monicapf.egg-info/requires.txt
+-rw-r--r--   0 bilol     (1000) bilol     (1000)        9 2024-05-19 07:53:07.000000 monicapf-0.1.2/monicapf.egg-info/top_level.txt
+-rw-r--r--   0 bilol     (1000) bilol     (1000)       38 2024-05-19 07:53:07.829134 monicapf-0.1.2/setup.cfg
+-rw-r--r--   0 bilol     (1000) bilol     (1000)     3946 2024-05-19 07:52:58.000000 monicapf-0.1.2/setup.py
```

### Comparing `monicapf-0.1.1/PKG-INFO` & `monicapf-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monicapf
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python Web Frmaework built for learning purposes. 
 Home-page: https://github.com/me/myproject
 Author: Abdumalikov Bilolbek
 Author-email: bilolabdumalikov1@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -16,16 +16,16 @@
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 
 
 # MonicaPF: Python Web Framework built for learning purposes
 
 
-![Purpose](https://img.shields.io/badge/:learning-green)
-![PyPI - Version](https://img.shields.io/pypi/v/:monicapf)
+![Purpose](https://img.shields.io/badge/learning-green)
+![PyPI - Version](https://img.shields.io/pypi/v/monicapf)
 
 
 MonicaPF it is python web framework
 
 It is WSGI Framework and can be used with any WSGI application server such as Gunicorn
 
 
@@ -106,15 +106,15 @@
         ) 
     ```       
 
 # Add Static Files
     Create "static" folder and save inside that folder static files
 
     
-    ```html
+```html
 <!DOCTYPE html>
 <html lang="en">
 
 <head>
     <meta charset="UTF-8">
     <title>{{title}}</title>
 
@@ -122,15 +122,15 @@
 </head>
 
 <body>
     <h1>{{body}}</h1>
     <p>This is a paragraph</p>
 </body>
 </html>
-    ```
+```
 
 
 
 # MiddleWare
 
 You can create custom middleware classes by inheriting from the monicapf.middleware.Middleware class and overriding its two methods that are called before and after each request:
```

### Comparing `monicapf-0.1.1/README.md` & `monicapf-0.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # MonicaPF: Python Web Framework built for learning purposes
 
 
-![Purpose](https://img.shields.io/badge/:learning-green)
-![PyPI - Version](https://img.shields.io/pypi/v/:monicapf)
+![Purpose](https://img.shields.io/badge/learning-green)
+![PyPI - Version](https://img.shields.io/pypi/v/monicapf)
 
 
 MonicaPF it is python web framework
 
 It is WSGI Framework and can be used with any WSGI application server such as Gunicorn
 
 
@@ -87,15 +87,15 @@
         ) 
     ```       
 
 # Add Static Files
     Create "static" folder and save inside that folder static files
 
     
-    ```html
+```html
 <!DOCTYPE html>
 <html lang="en">
 
 <head>
     <meta charset="UTF-8">
     <title>{{title}}</title>
 
@@ -103,15 +103,15 @@
 </head>
 
 <body>
     <h1>{{body}}</h1>
     <p>This is a paragraph</p>
 </body>
 </html>
-    ```
+```
 
 
 
 # MiddleWare
 
 You can create custom middleware classes by inheriting from the monicapf.middleware.Middleware class and overriding its two methods that are called before and after each request:
```

### Comparing `monicapf-0.1.1/monicapf.egg-info/PKG-INFO` & `monicapf-0.1.2/monicapf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monicapf
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python Web Frmaework built for learning purposes. 
 Home-page: https://github.com/me/myproject
 Author: Abdumalikov Bilolbek
 Author-email: bilolabdumalikov1@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -16,16 +16,16 @@
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 
 
 # MonicaPF: Python Web Framework built for learning purposes
 
 
-![Purpose](https://img.shields.io/badge/:learning-green)
-![PyPI - Version](https://img.shields.io/pypi/v/:monicapf)
+![Purpose](https://img.shields.io/badge/learning-green)
+![PyPI - Version](https://img.shields.io/pypi/v/monicapf)
 
 
 MonicaPF it is python web framework
 
 It is WSGI Framework and can be used with any WSGI application server such as Gunicorn
 
 
@@ -106,15 +106,15 @@
         ) 
     ```       
 
 # Add Static Files
     Create "static" folder and save inside that folder static files
 
     
-    ```html
+```html
 <!DOCTYPE html>
 <html lang="en">
 
 <head>
     <meta charset="UTF-8">
     <title>{{title}}</title>
 
@@ -122,15 +122,15 @@
 </head>
 
 <body>
     <h1>{{body}}</h1>
     <p>This is a paragraph</p>
 </body>
 </html>
-    ```
+```
 
 
 
 # MiddleWare
 
 You can create custom middleware classes by inheriting from the monicapf.middleware.Middleware class and overriding its two methods that are called before and after each request:
```

### Comparing `monicapf-0.1.1/setup.py` & `monicapf-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'monicapf'
 DESCRIPTION = 'Python Web Frmaework built for learning purposes. '
 URL = 'https://github.com/me/myproject'
 EMAIL = 'bilolabdumalikov1@gmail.com'
 AUTHOR = 'Abdumalikov Bilolbek'
 REQUIRES_PYTHON = '>=3.9.0'
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "gunicorn==19.9.0",
     "Jinja2==3.1.4",
     "whitenoise==6.6.0",
     "WebOb==1.8.5",
```

