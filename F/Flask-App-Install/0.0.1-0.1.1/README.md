# Comparing `tmp/flask_app_install-0.0.1.tar.gz` & `tmp/flask_app_install-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_app_install-0.0.1.tar", last modified: Mon May 20 07:41:26 2024, max compression
+gzip compressed data, was "flask_app_install-0.1.1.tar", last modified: Mon May 20 08:22:41 2024, max compression
```

## Comparing `flask_app_install-0.0.1.tar` & `flask_app_install-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 07:41:26.964112 flask_app_install-0.0.1/
-drwxrwxrwx   0        0        0        0 2024-05-20 07:41:26.937865 flask_app_install-0.0.1/Flask_App_Install.egg-info/
--rw-rw-rw-   0        0        0      870 2024-05-20 07:41:26.000000 flask_app_install-0.0.1/Flask_App_Install.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2024-05-20 07:41:26.000000 flask_app_install-0.0.1/Flask_App_Install.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 07:41:26.000000 flask_app_install-0.0.1/Flask_App_Install.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2024-05-20 07:41:26.000000 flask_app_install-0.0.1/Flask_App_Install.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-20 07:41:26.000000 flask_app_install-0.0.1/Flask_App_Install.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1083 2024-05-18 13:06:21.000000 flask_app_install-0.0.1/LICENCE
--rw-rw-rw-   0        0        0      870 2024-05-20 07:41:26.951604 flask_app_install-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       88 2024-05-20 07:39:14.000000 flask_app_install-0.0.1/README.md
--rw-rw-rw-   0        0        0      403 2024-05-20 07:30:10.000000 flask_app_install-0.0.1/run.sh
--rw-rw-rw-   0        0        0       42 2024-05-20 07:41:26.965205 flask_app_install-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1255 2024-05-20 07:39:38.000000 flask_app_install-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-20 07:41:26.924191 flask_app_install-0.0.1/src/
--rw-rw-rw-   0        0        0      106 2024-05-20 07:36:38.000000 flask_app_install-0.0.1/src/__init__.py
--rw-rw-rw-   0        0        0     1543 2024-05-20 07:37:47.000000 flask_app_install-0.0.1/src/app.py
--rw-rw-rw-   0        0        0      372 2024-05-20 07:38:30.000000 flask_app_install-0.0.1/src/writefile_app.py
+drwxrwxrwx   0        0        0        0 2024-05-20 08:22:41.139123 flask_app_install-0.1.1/
+drwxrwxrwx   0        0        0        0 2024-05-20 08:22:41.114059 flask_app_install-0.1.1/Flask_App_Install.egg-info/
+-rw-rw-rw-   0        0        0      867 2024-05-20 08:22:40.000000 flask_app_install-0.1.1/Flask_App_Install.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2024-05-20 08:22:40.000000 flask_app_install-0.1.1/Flask_App_Install.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 08:22:40.000000 flask_app_install-0.1.1/Flask_App_Install.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2024-05-20 08:22:40.000000 flask_app_install-0.1.1/Flask_App_Install.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-20 08:22:40.000000 flask_app_install-0.1.1/Flask_App_Install.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1083 2024-05-18 13:06:21.000000 flask_app_install-0.1.1/LICENCE
+-rw-rw-rw-   0        0        0      867 2024-05-20 08:22:41.127441 flask_app_install-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       88 2024-05-20 07:39:14.000000 flask_app_install-0.1.1/README.md
+-rw-rw-rw-   0        0        0      407 2024-05-20 08:21:58.000000 flask_app_install-0.1.1/run.sh
+-rw-rw-rw-   0        0        0       42 2024-05-20 08:22:41.140274 flask_app_install-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1252 2024-05-20 08:21:44.000000 flask_app_install-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 08:22:41.102753 flask_app_install-0.1.1/src/
+-rw-rw-rw-   0        0        0      106 2024-05-20 07:36:38.000000 flask_app_install-0.1.1/src/__init__.py
+-rw-rw-rw-   0        0        0     1836 2024-05-20 08:21:17.000000 flask_app_install-0.1.1/src/app.py
+-rw-rw-rw-   0        0        0      372 2024-05-20 07:38:30.000000 flask_app_install-0.1.1/src/writefile_app.py
```

### Comparing `flask_app_install-0.0.1/Flask_App_Install.egg-info/PKG-INFO` & `flask_app_install-0.1.1/Flask_App_Install.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask_App_Install
-Version: 0.0.1
+Version: 0.1.1
 Summary: Sets up a basic Flask App with Javascipt Functionality
 Author: kunaalg
 Author-email: <kunaal@runcode.in>
 Keywords: python,Flask,App,Javascript,Function,math
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -14,15 +14,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENCE
 Requires-Dist: datetime
 Requires-Dist: pandas
 Requires-Dist: requests
 Requires-Dist: numpy
 Requires-Dist: flask
-Requires-Dist: python-dotenv
+Requires-Dist: virtualenv
 Requires-Dist: pipreqs
 Requires-Dist: pip-tools
 
 
 Install the Package:
 
 Import the create_app() function, call the function and deploy
```

### Comparing `flask_app_install-0.0.1/LICENCE` & `flask_app_install-0.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `flask_app_install-0.0.1/PKG-INFO` & `flask_app_install-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask_App_Install
-Version: 0.0.1
+Version: 0.1.1
 Summary: Sets up a basic Flask App with Javascipt Functionality
 Author: kunaalg
 Author-email: <kunaal@runcode.in>
 Keywords: python,Flask,App,Javascript,Function,math
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -14,15 +14,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENCE
 Requires-Dist: datetime
 Requires-Dist: pandas
 Requires-Dist: requests
 Requires-Dist: numpy
 Requires-Dist: flask
-Requires-Dist: python-dotenv
+Requires-Dist: virtualenv
 Requires-Dist: pipreqs
 Requires-Dist: pip-tools
 
 
 Install the Package:
 
 Import the create_app() function, call the function and deploy
```

### Comparing `flask_app_install-0.0.1/setup.py` & `flask_app_install-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.1.1'
 DESCRIPTION = 'Sets up a basic Flask App with Javascipt Functionality'
 LONG_DESCRIPTION = 'A package that sets up a basic Flask App Boilerplate with Javascript Functionality.'
 
 # Setting up
 setup(
     name="Flask_App_Install",
     version=VERSION,
     author="kunaalg",
     author_email="<kunaal@runcode.in>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
     scripts=['run.sh'],
-    install_requires=['datetime', 'pandas', 'requests', 'numpy', 'flask', 'python-dotenv', 'pipreqs', 'pip-tools'],
+    install_requires=['datetime', 'pandas', 'requests', 'numpy', 'flask', 'virtualenv', 'pipreqs', 'pip-tools'],
     keywords=['python', 'Flask', 'App', 'Javascript', 'Function', 'math'],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

### Comparing `flask_app_install-0.0.1/src/app.py` & `flask_app_install-0.1.1/src/app.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 from flask import Flask, jsonify, render_template, request
 
 def create_index_html():
     html_content = """
     <!DOCTYPE html>
     <html>
     <head>
+        <meta charset="utf-8">
+        <meta http-equiv="X-UA-Compatible" content="IE=edge">
+        <title>FlaskApplication</title>
+        <meta name="description" content="">
+        <meta name="viewport" content="width=device-width, initial-scale=1">
+        <link rel="stylesheet" href="">
         <title>Flask App</title>
         <script src="{{ url_for('static', filename='js/script.js') }}"></script>
     </head>
     <body>
         <!-- rest of your HTML code -->
     </body>
     </html>
@@ -33,15 +39,15 @@
             });
         });
     });
     """
 
     with open(os.path.join('static', 'js', 'script.js'), 'w') as f:
         f.write(js_content)
-        
+
 def create_app():
     app = Flask(__name__)
 
     @app.route('/')
     def index():
         return render_template('index.html')
```

