# Comparing `tmp/html_flask_install-0.0.1.tar.gz` & `tmp/html_flask_install-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html_flask_install-0.0.1.tar", last modified: Mon May 20 05:34:53 2024, max compression
+gzip compressed data, was "html_flask_install-0.1.1.tar", last modified: Mon May 20 08:29:48 2024, max compression
```

## Comparing `html_flask_install-0.0.1.tar` & `html_flask_install-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 05:34:53.087182 html_flask_install-0.0.1/
-drwxrwxrwx   0        0        0        0 2024-05-20 05:34:53.074133 html_flask_install-0.0.1/Html_Flask_Install.egg-info/
--rw-rw-rw-   0        0        0      884 2024-05-20 05:34:52.000000 html_flask_install-0.0.1/Html_Flask_Install.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2024-05-20 05:34:52.000000 html_flask_install-0.0.1/Html_Flask_Install.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 05:34:52.000000 html_flask_install-0.0.1/Html_Flask_Install.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2024-05-20 05:34:52.000000 html_flask_install-0.0.1/Html_Flask_Install.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-20 05:34:52.000000 html_flask_install-0.0.1/Html_Flask_Install.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1083 2024-05-18 13:06:21.000000 html_flask_install-0.0.1/LICENCE
--rw-rw-rw-   0        0        0      884 2024-05-20 05:34:53.074133 html_flask_install-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       78 2024-05-20 04:19:43.000000 html_flask_install-0.0.1/README.md
--rw-rw-rw-   0        0        0      171 2024-05-20 05:27:58.000000 html_flask_install-0.0.1/run.sh
--rw-rw-rw-   0        0        0       42 2024-05-20 05:34:53.087684 html_flask_install-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1284 2024-05-20 05:34:08.000000 html_flask_install-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-20 05:34:53.073081 html_flask_install-0.0.1/src/
--rw-rw-rw-   0        0        0       43 2024-05-20 04:51:25.000000 html_flask_install-0.0.1/src/__init__.py
--rw-rw-rw-   0        0        0      970 2024-05-20 04:50:04.000000 html_flask_install-0.0.1/src/writefile_html.py
+drwxrwxrwx   0        0        0        0 2024-05-20 08:29:48.384636 html_flask_install-0.1.1/
+drwxrwxrwx   0        0        0        0 2024-05-20 08:29:48.362394 html_flask_install-0.1.1/Html_Flask_Install.egg-info/
+-rw-rw-rw-   0        0        0      881 2024-05-20 08:29:47.000000 html_flask_install-0.1.1/Html_Flask_Install.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2024-05-20 08:29:47.000000 html_flask_install-0.1.1/Html_Flask_Install.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 08:29:47.000000 html_flask_install-0.1.1/Html_Flask_Install.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2024-05-20 08:29:47.000000 html_flask_install-0.1.1/Html_Flask_Install.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-20 08:29:47.000000 html_flask_install-0.1.1/Html_Flask_Install.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1083 2024-05-18 13:06:21.000000 html_flask_install-0.1.1/LICENCE
+-rw-rw-rw-   0        0        0      881 2024-05-20 08:29:48.374633 html_flask_install-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       78 2024-05-20 04:19:43.000000 html_flask_install-0.1.1/README.md
+-rw-rw-rw-   0        0        0      408 2024-05-20 08:28:51.000000 html_flask_install-0.1.1/run.sh
+-rw-rw-rw-   0        0        0       42 2024-05-20 08:29:48.385489 html_flask_install-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1281 2024-05-20 08:29:31.000000 html_flask_install-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 08:29:48.338211 html_flask_install-0.1.1/src/
+-rw-rw-rw-   0        0        0       43 2024-05-20 04:51:25.000000 html_flask_install-0.1.1/src/__init__.py
+-rw-rw-rw-   0        0        0      970 2024-05-20 04:50:04.000000 html_flask_install-0.1.1/src/writefile_html.py
```

### Comparing `html_flask_install-0.0.1/Html_Flask_Install.egg-info/PKG-INFO` & `html_flask_install-0.1.1/Html_Flask_Install.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Html_Flask_Install
-Version: 0.0.1
+Version: 0.1.1
 Summary: Sets up a basic HTML Boilerplate for a Flask App with Javascipt Functionality
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
 
 Update your Index.html file in the templates folder.
```

### Comparing `html_flask_install-0.0.1/LICENCE` & `html_flask_install-0.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `html_flask_install-0.0.1/PKG-INFO` & `html_flask_install-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Html_Flask_Install
-Version: 0.0.1
+Version: 0.1.1
 Summary: Sets up a basic HTML Boilerplate for a Flask App with Javascipt Functionality
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
 
 Update your Index.html file in the templates folder.
```

### Comparing `html_flask_install-0.0.1/setup.py` & `html_flask_install-0.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.1.1'
 DESCRIPTION = 'Sets up a basic HTML Boilerplate for a Flask App with Javascipt Functionality'
 LONG_DESCRIPTION = 'A package that sets up a basic HTML Boilerplate Flask App with Javascript Functionality.'
 
 # Setting up
 setup(
     name="Html_Flask_Install",
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

### Comparing `html_flask_install-0.0.1/src/writefile_html.py` & `html_flask_install-0.1.1/src/writefile_html.py`

 * *Files identical despite different names*

