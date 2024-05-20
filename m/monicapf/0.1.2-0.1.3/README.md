# Comparing `tmp/monicapf-0.1.2.tar.gz` & `tmp/monicapf-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monicapf-0.1.2.tar", last modified: Sun May 19 07:53:07 2024, max compression
+gzip compressed data, was "monicapf-0.1.3.tar", last modified: Mon May 20 06:27:31 2024, max compression
```

## Comparing `monicapf-0.1.2.tar` & `monicapf-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 bilol     (1000) bilol     (1000)        0 2024-05-19 07:53:07.829134 monicapf-0.1.2/
--rw-r--r--   0 bilol     (1000) bilol     (1000)     4327 2024-05-19 07:53:07.825134 monicapf-0.1.2/PKG-INFO
--rw-r--r--   0 bilol     (1000) bilol     (1000)     3668 2024-05-19 07:52:51.000000 monicapf-0.1.2/README.md
-drwxr-xr-x   0 bilol     (1000) bilol     (1000)        0 2024-05-19 07:53:07.821134 monicapf-0.1.2/monicapf/
--rw-r--r--   0 bilol     (1000) bilol     (1000)        0 2024-05-19 07:52:48.000000 monicapf-0.1.2/monicapf/__init__.py
--rw-r--r--   0 bilol     (1000) bilol     (1000)     3796 2024-05-17 14:48:32.000000 monicapf-0.1.2/monicapf/app.py
--rw-r--r--   0 bilol     (1000) bilol     (1000)      686 2024-05-17 14:48:30.000000 monicapf-0.1.2/monicapf/middleware.py
--rw-r--r--   0 bilol     (1000) bilol     (1000)      954 2024-05-17 14:48:29.000000 monicapf-0.1.2/monicapf/response.py
-drwxr-xr-x   0 bilol     (1000) bilol     (1000)        0 2024-05-19 07:53:07.824134 monicapf-0.1.2/monicapf.egg-info/
--rw-r--r--   0 bilol     (1000) bilol     (1000)     4327 2024-05-19 07:53:07.000000 monicapf-0.1.2/monicapf.egg-info/PKG-INFO
--rw-r--r--   0 bilol     (1000) bilol     (1000)      258 2024-05-19 07:53:07.000000 monicapf-0.1.2/monicapf.egg-info/SOURCES.txt
--rw-r--r--   0 bilol     (1000) bilol     (1000)        1 2024-05-19 07:53:07.000000 monicapf-0.1.2/monicapf.egg-info/dependency_links.txt
--rw-r--r--   0 bilol     (1000) bilol     (1000)      122 2024-05-19 07:53:07.000000 monicapf-0.1.2/monicapf.egg-info/requires.txt
--rw-r--r--   0 bilol     (1000) bilol     (1000)        9 2024-05-19 07:53:07.000000 monicapf-0.1.2/monicapf.egg-info/top_level.txt
--rw-r--r--   0 bilol     (1000) bilol     (1000)       38 2024-05-19 07:53:07.829134 monicapf-0.1.2/setup.cfg
--rw-r--r--   0 bilol     (1000) bilol     (1000)     3946 2024-05-19 07:52:58.000000 monicapf-0.1.2/setup.py
+drwxr-xr-x   0 bilol     (1000) bilol     (1000)        0 2024-05-20 06:27:31.783743 monicapf-0.1.3/
+-rw-r--r--   0 bilol     (1000) bilol     (1000)     4172 2024-05-20 06:27:31.779743 monicapf-0.1.3/PKG-INFO
+-rw-r--r--   0 bilol     (1000) bilol     (1000)     3513 2024-05-20 06:26:16.000000 monicapf-0.1.3/README.md
+drwxr-xr-x   0 bilol     (1000) bilol     (1000)        0 2024-05-20 06:27:31.775743 monicapf-0.1.3/monicapf/
+-rw-r--r--   0 bilol     (1000) bilol     (1000)        0 2024-05-19 07:52:48.000000 monicapf-0.1.3/monicapf/__init__.py
+-rw-r--r--   0 bilol     (1000) bilol     (1000)     3796 2024-05-17 14:48:32.000000 monicapf-0.1.3/monicapf/app.py
+-rw-r--r--   0 bilol     (1000) bilol     (1000)      686 2024-05-17 14:48:30.000000 monicapf-0.1.3/monicapf/middleware.py
+-rw-r--r--   0 bilol     (1000) bilol     (1000)      954 2024-05-17 14:48:29.000000 monicapf-0.1.3/monicapf/response.py
+drwxr-xr-x   0 bilol     (1000) bilol     (1000)        0 2024-05-20 06:27:31.778743 monicapf-0.1.3/monicapf.egg-info/
+-rw-r--r--   0 bilol     (1000) bilol     (1000)     4172 2024-05-20 06:27:31.000000 monicapf-0.1.3/monicapf.egg-info/PKG-INFO
+-rw-r--r--   0 bilol     (1000) bilol     (1000)      258 2024-05-20 06:27:31.000000 monicapf-0.1.3/monicapf.egg-info/SOURCES.txt
+-rw-r--r--   0 bilol     (1000) bilol     (1000)        1 2024-05-20 06:27:31.000000 monicapf-0.1.3/monicapf.egg-info/dependency_links.txt
+-rw-r--r--   0 bilol     (1000) bilol     (1000)      122 2024-05-20 06:27:31.000000 monicapf-0.1.3/monicapf.egg-info/requires.txt
+-rw-r--r--   0 bilol     (1000) bilol     (1000)        9 2024-05-20 06:27:31.000000 monicapf-0.1.3/monicapf.egg-info/top_level.txt
+-rw-r--r--   0 bilol     (1000) bilol     (1000)       38 2024-05-20 06:27:31.783743 monicapf-0.1.3/setup.cfg
+-rw-r--r--   0 bilol     (1000) bilol     (1000)     3946 2024-05-20 06:26:14.000000 monicapf-0.1.3/setup.py
```

### Comparing `monicapf-0.1.2/PKG-INFO` & `monicapf-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monicapf
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python Web Frmaework built for learning purposes. 
 Home-page: https://github.com/me/myproject
 Author: Abdumalikov Bilolbek
 Author-email: bilolabdumalikov1@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -35,80 +35,81 @@
 ```
 
 # How To Use It:
 
 
 ### Basic Usage:
 
-    ```python
-    from monicapf.app import Monica
+```python
+from monicapf.app import Monica
 
 
-    app = Monica()      
+app = Monica()      
 
 
 # Add Allowed Methods:
-    @app.route('/home', allowed_methods=['get'])
-    def home(request, response):
-        if request.method == 'GET':
-            response.text = 'Hello this is home page'
-        elif request.method == 'POST':
-            response.text = 'POST '
+@app.route('/home', allowed_methods=['get'])
+def home(request, response):
+    if request.method == 'GET':
+        response.text = 'Hello this is home page'
+    elif request.method == 'POST':
+        response.text = 'POST '
 
 
 # Simple Route:
-    @app.route('/about')
-    def about(request, response):
-        response.text = 'Hello this is about page'    
-        
+@app.route('/about')
+def about(request, response):
+    response.text = 'Hello this is about page'    
+    
 
 # Parametrize Route:
-    @app.route('/hello/{name}')
-    def hello(request, response, name):
-        response.text = f"Just say hello. Hello {name}"    
+@app.route('/hello/{name}')
+def hello(request, response, name):
+    response.text = f"Just say hello. Hello {name}"    
 
 
 # Class Based Handlers:
-    @app.route('/books')
-    class Book:
-        def get(self, request, response):
-            response.text = 'Books GET request'
+@app.route('/books')
+class Book:
+    def get(self, request, response):
+        response.text = 'Books GET request'
 
-        def post(self, request, response):
-            response.text = 'Books POST request'
+    def post(self, request, response):
+        response.text = 'Books POST request'
 
 
-    def new_handler(req, res):
-        res.text = 'New handler'
+def new_handler(req, res):
+    res.text = 'New handler'
 
-    app.add_route('/new-handler', new_handler)
+app.add_route('/new-handler', new_handler)
 
 
 
 
 # Json data:
-    @app.route('/json')
-    def json(req, res):
-        res.json = {
-            'name': 'Request',
-            'Body': 'Json response',
-        }
-    ```
+@app.route('/json')
+def json(req, res):
+    res.json = {
+        'name': 'Request',
+        'Body': 'Json response',
+    }
+```
 
 # Add Template
     Create "templates" folder and save inside that folder htmls
 
-    ```python
-    @app.route('/template')
-    def template(req, res):
-        res.body = app.template(
-            'home.html',
-            context={'name': 'Bilol', 'title': 'Template working'}
-        ) 
-    ```       
+```python
+@app.route('/template')
+def template(req, res):
+    res.body = app.template(
+        'home.html',
+        context={'name': 'Bilol', 'title': 'Template working'}
+    ) 
+    
+```       
 
 # Add Static Files
     Create "static" folder and save inside that folder static files
 
     
 ```html
 <!DOCTYPE html>
```

### Comparing `monicapf-0.1.2/README.md` & `monicapf-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -16,80 +16,81 @@
 ```
 
 # How To Use It:
 
 
 ### Basic Usage:
 
-    ```python
-    from monicapf.app import Monica
+```python
+from monicapf.app import Monica
 
 
-    app = Monica()      
+app = Monica()      
 
 
 # Add Allowed Methods:
-    @app.route('/home', allowed_methods=['get'])
-    def home(request, response):
-        if request.method == 'GET':
-            response.text = 'Hello this is home page'
-        elif request.method == 'POST':
-            response.text = 'POST '
+@app.route('/home', allowed_methods=['get'])
+def home(request, response):
+    if request.method == 'GET':
+        response.text = 'Hello this is home page'
+    elif request.method == 'POST':
+        response.text = 'POST '
 
 
 # Simple Route:
-    @app.route('/about')
-    def about(request, response):
-        response.text = 'Hello this is about page'    
-        
+@app.route('/about')
+def about(request, response):
+    response.text = 'Hello this is about page'    
+    
 
 # Parametrize Route:
-    @app.route('/hello/{name}')
-    def hello(request, response, name):
-        response.text = f"Just say hello. Hello {name}"    
+@app.route('/hello/{name}')
+def hello(request, response, name):
+    response.text = f"Just say hello. Hello {name}"    
 
 
 # Class Based Handlers:
-    @app.route('/books')
-    class Book:
-        def get(self, request, response):
-            response.text = 'Books GET request'
+@app.route('/books')
+class Book:
+    def get(self, request, response):
+        response.text = 'Books GET request'
 
-        def post(self, request, response):
-            response.text = 'Books POST request'
+    def post(self, request, response):
+        response.text = 'Books POST request'
 
 
-    def new_handler(req, res):
-        res.text = 'New handler'
+def new_handler(req, res):
+    res.text = 'New handler'
 
-    app.add_route('/new-handler', new_handler)
+app.add_route('/new-handler', new_handler)
 
 
 
 
 # Json data:
-    @app.route('/json')
-    def json(req, res):
-        res.json = {
-            'name': 'Request',
-            'Body': 'Json response',
-        }
-    ```
+@app.route('/json')
+def json(req, res):
+    res.json = {
+        'name': 'Request',
+        'Body': 'Json response',
+    }
+```
 
 # Add Template
     Create "templates" folder and save inside that folder htmls
 
-    ```python
-    @app.route('/template')
-    def template(req, res):
-        res.body = app.template(
-            'home.html',
-            context={'name': 'Bilol', 'title': 'Template working'}
-        ) 
-    ```       
+```python
+@app.route('/template')
+def template(req, res):
+    res.body = app.template(
+        'home.html',
+        context={'name': 'Bilol', 'title': 'Template working'}
+    ) 
+    
+```       
 
 # Add Static Files
     Create "static" folder and save inside that folder static files
 
     
 ```html
 <!DOCTYPE html>
```

### Comparing `monicapf-0.1.2/monicapf/app.py` & `monicapf-0.1.3/monicapf/app.py`

 * *Files identical despite different names*

### Comparing `monicapf-0.1.2/monicapf/middleware.py` & `monicapf-0.1.3/monicapf/middleware.py`

 * *Files identical despite different names*

### Comparing `monicapf-0.1.2/monicapf/response.py` & `monicapf-0.1.3/monicapf/response.py`

 * *Files identical despite different names*

### Comparing `monicapf-0.1.2/monicapf.egg-info/PKG-INFO` & `monicapf-0.1.3/monicapf.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monicapf
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python Web Frmaework built for learning purposes. 
 Home-page: https://github.com/me/myproject
 Author: Abdumalikov Bilolbek
 Author-email: bilolabdumalikov1@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -35,80 +35,81 @@
 ```
 
 # How To Use It:
 
 
 ### Basic Usage:
 
-    ```python
-    from monicapf.app import Monica
+```python
+from monicapf.app import Monica
 
 
-    app = Monica()      
+app = Monica()      
 
 
 # Add Allowed Methods:
-    @app.route('/home', allowed_methods=['get'])
-    def home(request, response):
-        if request.method == 'GET':
-            response.text = 'Hello this is home page'
-        elif request.method == 'POST':
-            response.text = 'POST '
+@app.route('/home', allowed_methods=['get'])
+def home(request, response):
+    if request.method == 'GET':
+        response.text = 'Hello this is home page'
+    elif request.method == 'POST':
+        response.text = 'POST '
 
 
 # Simple Route:
-    @app.route('/about')
-    def about(request, response):
-        response.text = 'Hello this is about page'    
-        
+@app.route('/about')
+def about(request, response):
+    response.text = 'Hello this is about page'    
+    
 
 # Parametrize Route:
-    @app.route('/hello/{name}')
-    def hello(request, response, name):
-        response.text = f"Just say hello. Hello {name}"    
+@app.route('/hello/{name}')
+def hello(request, response, name):
+    response.text = f"Just say hello. Hello {name}"    
 
 
 # Class Based Handlers:
-    @app.route('/books')
-    class Book:
-        def get(self, request, response):
-            response.text = 'Books GET request'
+@app.route('/books')
+class Book:
+    def get(self, request, response):
+        response.text = 'Books GET request'
 
-        def post(self, request, response):
-            response.text = 'Books POST request'
+    def post(self, request, response):
+        response.text = 'Books POST request'
 
 
-    def new_handler(req, res):
-        res.text = 'New handler'
+def new_handler(req, res):
+    res.text = 'New handler'
 
-    app.add_route('/new-handler', new_handler)
+app.add_route('/new-handler', new_handler)
 
 
 
 
 # Json data:
-    @app.route('/json')
-    def json(req, res):
-        res.json = {
-            'name': 'Request',
-            'Body': 'Json response',
-        }
-    ```
+@app.route('/json')
+def json(req, res):
+    res.json = {
+        'name': 'Request',
+        'Body': 'Json response',
+    }
+```
 
 # Add Template
     Create "templates" folder and save inside that folder htmls
 
-    ```python
-    @app.route('/template')
-    def template(req, res):
-        res.body = app.template(
-            'home.html',
-            context={'name': 'Bilol', 'title': 'Template working'}
-        ) 
-    ```       
+```python
+@app.route('/template')
+def template(req, res):
+    res.body = app.template(
+        'home.html',
+        context={'name': 'Bilol', 'title': 'Template working'}
+    ) 
+    
+```       
 
 # Add Static Files
     Create "static" folder and save inside that folder static files
 
     
 ```html
 <!DOCTYPE html>
```

### Comparing `monicapf-0.1.2/setup.py` & `monicapf-0.1.3/setup.py`

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
-VERSION = '0.1.2'
+VERSION = '0.1.3'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "gunicorn==19.9.0",
     "Jinja2==3.1.4",
     "whitenoise==6.6.0",
     "WebOb==1.8.5",
```

