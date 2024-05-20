# Comparing `tmp/js_flask_install-0.1.tar.gz` & `tmp/js_flask_install-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "js_flask_install-0.1.tar", last modified: Mon May 20 07:17:50 2024, max compression
+gzip compressed data, was "js_flask_install-0.1.1.tar", last modified: Mon May 20 08:17:10 2024, max compression
```

## Comparing `js_flask_install-0.1.tar` & `js_flask_install-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 07:17:50.349401 js_flask_install-0.1/
-drwxrwxrwx   0        0        0        0 2024-05-20 07:17:50.322701 js_flask_install-0.1/JS_Flask_Install.egg-info/
--rw-rw-rw-   0        0        0      925 2024-05-20 07:17:49.000000 js_flask_install-0.1/JS_Flask_Install.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2024-05-20 07:17:50.000000 js_flask_install-0.1/JS_Flask_Install.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 07:17:49.000000 js_flask_install-0.1/JS_Flask_Install.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       99 2024-05-20 07:17:49.000000 js_flask_install-0.1/JS_Flask_Install.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-20 07:17:49.000000 js_flask_install-0.1/JS_Flask_Install.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1083 2024-05-18 13:06:21.000000 js_flask_install-0.1/LICENCE
--rw-rw-rw-   0        0        0      925 2024-05-20 07:17:50.336654 js_flask_install-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       75 2024-05-20 07:06:24.000000 js_flask_install-0.1/README.md
--rw-rw-rw-   0        0        0      402 2024-05-20 07:04:25.000000 js_flask_install-0.1/run.sh
--rw-rw-rw-   0        0        0       42 2024-05-20 07:17:50.350403 js_flask_install-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1321 2024-05-20 07:15:52.000000 js_flask_install-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-20 07:17:50.311413 js_flask_install-0.1/src/
--rw-rw-rw-   0        0        0       39 2024-05-20 07:07:06.000000 js_flask_install-0.1/src/__init__.py
--rw-rw-rw-   0        0        0      541 2024-05-20 07:03:52.000000 js_flask_install-0.1/src/writefile_js.py
+drwxrwxrwx   0        0        0        0 2024-05-20 08:17:10.811744 js_flask_install-0.1.1/
+drwxrwxrwx   0        0        0        0 2024-05-20 08:17:10.782690 js_flask_install-0.1.1/JS_Flask_Install.egg-info/
+-rw-rw-rw-   0        0        0      911 2024-05-20 08:17:10.000000 js_flask_install-0.1.1/JS_Flask_Install.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2024-05-20 08:17:10.000000 js_flask_install-0.1.1/JS_Flask_Install.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 08:17:10.000000 js_flask_install-0.1.1/JS_Flask_Install.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2024-05-20 08:17:10.000000 js_flask_install-0.1.1/JS_Flask_Install.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-20 08:17:10.000000 js_flask_install-0.1.1/JS_Flask_Install.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1083 2024-05-18 13:06:21.000000 js_flask_install-0.1.1/LICENCE
+-rw-rw-rw-   0        0        0      911 2024-05-20 08:17:10.797243 js_flask_install-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       75 2024-05-20 07:06:24.000000 js_flask_install-0.1.1/README.md
+-rw-rw-rw-   0        0        0      406 2024-05-20 08:06:15.000000 js_flask_install-0.1.1/run.sh
+-rw-rw-rw-   0        0        0       42 2024-05-20 08:17:10.813612 js_flask_install-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1307 2024-05-20 08:16:32.000000 js_flask_install-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 08:17:10.767416 js_flask_install-0.1.1/src/
+-rw-rw-rw-   0        0        0       39 2024-05-20 07:07:06.000000 js_flask_install-0.1.1/src/__init__.py
+-rw-rw-rw-   0        0        0      541 2024-05-20 07:03:52.000000 js_flask_install-0.1.1/src/writefile_js.py
```

### Comparing `js_flask_install-0.1/JS_Flask_Install.egg-info/PKG-INFO` & `js_flask_install-0.1.1/JS_Flask_Install.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JS_Flask_Install
-Version: 0.1
+Version: 0.1.1
 Summary: Sets up a basic Javascript Boilerplate and Directory Structure for a Flask App.
 Author: kunaalg
 Author-email: <kunaal@runcode.in>
 Keywords: python,Flask,App,Javascript,Function,math
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -14,16 +14,16 @@
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
-Requires-Dist: JS_Flask_Install.writefile_js
+Requires-Dist: JS_Flask_Install
 
 
 Install the Package:
 
 Update your Scripts.js file in the static folder.
```

### Comparing `js_flask_install-0.1/LICENCE` & `js_flask_install-0.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `js_flask_install-0.1/PKG-INFO` & `js_flask_install-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JS_Flask_Install
-Version: 0.1
+Version: 0.1.1
 Summary: Sets up a basic Javascript Boilerplate and Directory Structure for a Flask App.
 Author: kunaalg
 Author-email: <kunaal@runcode.in>
 Keywords: python,Flask,App,Javascript,Function,math
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -14,16 +14,16 @@
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
-Requires-Dist: JS_Flask_Install.writefile_js
+Requires-Dist: JS_Flask_Install
 
 
 Install the Package:
 
 Update your Scripts.js file in the static folder.
```

### Comparing `js_flask_install-0.1/setup.py` & `js_flask_install-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1'
+VERSION = '0.1.1'
 DESCRIPTION = 'Sets up a basic Javascript Boilerplate and Directory Structure for a Flask App.'
 LONG_DESCRIPTION = 'A package that sets up a basic Javascript Boilerplate and Directory Structure for a Flask App.'
 
 # Setting up
 setup(
     name="JS_Flask_Install",
     version=VERSION,
     author="kunaalg",
     author_email="<kunaal@runcode.in>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
     scripts=['run.sh'],
-    install_requires=['datetime', 'pandas', 'requests', 'numpy', 'flask', 'python-dotenv', 'pipreqs', 'pip-tools', 'JS_Flask_Install.writefile_js'],
+    install_requires=['datetime', 'pandas', 'requests', 'numpy', 'flask', 'virtualenv', 'pipreqs', 'pip-tools', 'JS_Flask_Install'],
     keywords=['python', 'Flask', 'App', 'Javascript', 'Function', 'math'],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

### Comparing `js_flask_install-0.1/src/writefile_js.py` & `js_flask_install-0.1.1/src/writefile_js.py`

 * *Files identical despite different names*

