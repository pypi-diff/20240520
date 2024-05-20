# Comparing `tmp/flask_tailwind_manager-0.0.3.tar.gz` & `tmp/flask_tailwind_manager-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_tailwind_manager-0.0.3.tar", last modified: Mon May 20 19:19:44 2024, max compression
+gzip compressed data, was "flask_tailwind_manager-0.0.4.tar", last modified: Mon May 20 19:26:24 2024, max compression
```

## Comparing `flask_tailwind_manager-0.0.3.tar` & `flask_tailwind_manager-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,33 @@
-drwxr-xr-x   0 thonder   (1000) thonder   (1000)        0 2024-05-20 19:19:44.956335 flask_tailwind_manager-0.0.3/
--rw-r--r--   0 thonder   (1000) thonder   (1000)     1081 2024-05-19 21:57:00.000000 flask_tailwind_manager-0.0.3/LICENSE
--rw-r--r--   0 thonder   (1000) thonder   (1000)     5099 2024-05-20 19:19:44.946335 flask_tailwind_manager-0.0.3/PKG-INFO
--rw-r--r--   0 thonder   (1000) thonder   (1000)     3295 2024-05-19 22:36:02.000000 flask_tailwind_manager-0.0.3/README.md
--rw-r--r--   0 thonder   (1000) thonder   (1000)      848 2024-05-20 19:19:25.000000 flask_tailwind_manager-0.0.3/pyproject.toml
--rw-r--r--   0 thonder   (1000) thonder   (1000)       38 2024-05-20 19:19:44.956335 flask_tailwind_manager-0.0.3/setup.cfg
--rw-r--r--   0 thonder   (1000) thonder   (1000)       54 2024-05-20 19:17:17.000000 flask_tailwind_manager-0.0.3/setup.py
-drwxr-xr-x   0 thonder   (1000) thonder   (1000)        0 2024-05-20 19:19:44.906335 flask_tailwind_manager-0.0.3/src/
-drwxr-xr-x   0 thonder   (1000) thonder   (1000)        0 2024-05-20 19:19:44.936335 flask_tailwind_manager-0.0.3/src/flask_tailwind/
--rw-r--r--   0 thonder   (1000) thonder   (1000)       62 2024-05-19 22:11:38.000000 flask_tailwind_manager-0.0.3/src/flask_tailwind/__init__.py
--rw-r--r--   0 thonder   (1000) thonder   (1000)     2365 2024-05-19 22:11:38.000000 flask_tailwind_manager-0.0.3/src/flask_tailwind/cli.py
--rw-r--r--   0 thonder   (1000) thonder   (1000)     1456 2024-05-19 22:11:38.000000 flask_tailwind_manager-0.0.3/src/flask_tailwind/console.py
--rw-r--r--   0 thonder   (1000) thonder   (1000)        0 2024-05-19 22:06:05.000000 flask_tailwind_manager-0.0.3/src/flask_tailwind/py.typed
--rw-r--r--   0 thonder   (1000) thonder   (1000)     3686 2024-05-19 22:11:38.000000 flask_tailwind_manager-0.0.3/src/flask_tailwind/tailwind.py
-drwxr-xr-x   0 thonder   (1000) thonder   (1000)        0 2024-05-20 19:19:44.946335 flask_tailwind_manager-0.0.3/src/flask_tailwind_manager.egg-info/
--rw-r--r--   0 thonder   (1000) thonder   (1000)     5099 2024-05-20 19:19:44.000000 flask_tailwind_manager-0.0.3/src/flask_tailwind_manager.egg-info/PKG-INFO
--rw-r--r--   0 thonder   (1000) thonder   (1000)      436 2024-05-20 19:19:44.000000 flask_tailwind_manager-0.0.3/src/flask_tailwind_manager.egg-info/SOURCES.txt
--rw-r--r--   0 thonder   (1000) thonder   (1000)        1 2024-05-20 19:19:44.000000 flask_tailwind_manager-0.0.3/src/flask_tailwind_manager.egg-info/dependency_links.txt
--rw-r--r--   0 thonder   (1000) thonder   (1000)       16 2024-05-20 19:19:44.000000 flask_tailwind_manager-0.0.3/src/flask_tailwind_manager.egg-info/requires.txt
--rw-r--r--   0 thonder   (1000) thonder   (1000)        1 2024-05-20 19:19:44.000000 flask_tailwind_manager-0.0.3/src/flask_tailwind_manager.egg-info/top_level.txt
+drwxr-xr-x   0 thonder   (1000) thonder   (1000)        0 2024-05-20 19:26:24.206352 flask_tailwind_manager-0.0.4/
+-rw-r--r--   0 thonder   (1000) thonder   (1000)     3098 2024-04-16 01:38:06.000000 flask_tailwind_manager-0.0.4/.gitignore
+-rw-r--r--   0 thonder   (1000) thonder   (1000)     1081 2024-05-19 21:57:00.000000 flask_tailwind_manager-0.0.4/LICENSE
+-rw-r--r--   0 thonder   (1000) thonder   (1000)     5099 2024-05-20 19:26:24.206352 flask_tailwind_manager-0.0.4/PKG-INFO
+-rw-r--r--   0 thonder   (1000) thonder   (1000)     3295 2024-05-19 22:36:02.000000 flask_tailwind_manager-0.0.4/README.md
+-rw-r--r--   0 thonder   (1000) thonder   (1000)      896 2024-05-20 19:26:03.000000 flask_tailwind_manager-0.0.4/pyproject.toml
+-rw-r--r--   0 thonder   (1000) thonder   (1000)       26 2024-05-19 21:19:37.000000 flask_tailwind_manager-0.0.4/requirements-dev.txt
+-rw-r--r--   0 thonder   (1000) thonder   (1000)        5 2024-05-19 21:19:33.000000 flask_tailwind_manager-0.0.4/requirements.txt
+-rw-r--r--   0 thonder   (1000) thonder   (1000)       38 2024-05-20 19:26:24.206352 flask_tailwind_manager-0.0.4/setup.cfg
+-rw-r--r--   0 thonder   (1000) thonder   (1000)       54 2024-05-20 19:17:17.000000 flask_tailwind_manager-0.0.4/setup.py
+drwxr-xr-x   0 thonder   (1000) thonder   (1000)        0 2024-05-20 19:26:24.136352 flask_tailwind_manager-0.0.4/src/
+drwxr-xr-x   0 thonder   (1000) thonder   (1000)        0 2024-05-20 19:26:24.176352 flask_tailwind_manager-0.0.4/src/flask_tailwind/
+-rw-r--r--   0 thonder   (1000) thonder   (1000)       62 2024-05-19 22:11:38.000000 flask_tailwind_manager-0.0.4/src/flask_tailwind/__init__.py
+-rw-r--r--   0 thonder   (1000) thonder   (1000)     2365 2024-05-19 22:11:38.000000 flask_tailwind_manager-0.0.4/src/flask_tailwind/cli.py
+-rw-r--r--   0 thonder   (1000) thonder   (1000)     1456 2024-05-19 22:11:38.000000 flask_tailwind_manager-0.0.4/src/flask_tailwind/console.py
+-rw-r--r--   0 thonder   (1000) thonder   (1000)        0 2024-05-19 22:06:05.000000 flask_tailwind_manager-0.0.4/src/flask_tailwind/py.typed
+drwxr-xr-x   0 thonder   (1000) thonder   (1000)        0 2024-05-20 19:26:24.186352 flask_tailwind_manager-0.0.4/src/flask_tailwind/starter/
+-rw-r--r--   0 thonder   (1000) thonder   (1000)        0 2024-05-19 00:12:17.000000 flask_tailwind_manager-0.0.4/src/flask_tailwind/starter/.gitignore
+-rw-r--r--   0 thonder   (1000) thonder   (1000)        0 2024-05-19 02:57:40.000000 flask_tailwind_manager-0.0.4/src/flask_tailwind/starter/package.json
+drwxr-xr-x   0 thonder   (1000) thonder   (1000)        0 2024-05-20 19:26:24.186352 flask_tailwind_manager-0.0.4/src/flask_tailwind/starter/src/
+-rw-r--r--   0 thonder   (1000) thonder   (1000)       58 2024-05-19 00:19:52.000000 flask_tailwind_manager-0.0.4/src/flask_tailwind/starter/src/input.css
+-rw-r--r--   0 thonder   (1000) thonder   (1000)        0 2024-05-19 18:03:15.000000 flask_tailwind_manager-0.0.4/src/flask_tailwind/starter/tailwind.config.js
+-rw-r--r--   0 thonder   (1000) thonder   (1000)     3686 2024-05-19 22:11:38.000000 flask_tailwind_manager-0.0.4/src/flask_tailwind/tailwind.py
+drwxr-xr-x   0 thonder   (1000) thonder   (1000)        0 2024-05-20 19:26:24.196352 flask_tailwind_manager-0.0.4/src/flask_tailwind/templates/
+-rw-r--r--   0 thonder   (1000) thonder   (1000)       73 2024-05-18 23:09:40.000000 flask_tailwind_manager-0.0.4/src/flask_tailwind/templates/load.jinja
+-rw-r--r--   0 thonder   (1000) thonder   (1000)       89 2024-05-19 18:30:33.000000 flask_tailwind_manager-0.0.4/src/flask_tailwind/templates/package.json.jinja
+-rw-r--r--   0 thonder   (1000) thonder   (1000)      497 2024-05-19 18:27:46.000000 flask_tailwind_manager-0.0.4/src/flask_tailwind/templates/tailwind.config.js.jinja
+drwxr-xr-x   0 thonder   (1000) thonder   (1000)        0 2024-05-20 19:26:24.206352 flask_tailwind_manager-0.0.4/src/flask_tailwind_manager.egg-info/
+-rw-r--r--   0 thonder   (1000) thonder   (1000)     5099 2024-05-20 19:26:23.000000 flask_tailwind_manager-0.0.4/src/flask_tailwind_manager.egg-info/PKG-INFO
+-rw-r--r--   0 thonder   (1000) thonder   (1000)      792 2024-05-20 19:26:24.000000 flask_tailwind_manager-0.0.4/src/flask_tailwind_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 thonder   (1000) thonder   (1000)        1 2024-05-20 19:26:23.000000 flask_tailwind_manager-0.0.4/src/flask_tailwind_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 thonder   (1000) thonder   (1000)       16 2024-05-20 19:26:23.000000 flask_tailwind_manager-0.0.4/src/flask_tailwind_manager.egg-info/requires.txt
+-rw-r--r--   0 thonder   (1000) thonder   (1000)        1 2024-05-20 19:26:23.000000 flask_tailwind_manager-0.0.4/src/flask_tailwind_manager.egg-info/top_level.txt
```

### Comparing `flask_tailwind_manager-0.0.3/LICENSE` & `flask_tailwind_manager-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_tailwind_manager-0.0.3/PKG-INFO` & `flask_tailwind_manager-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-tailwind-manager
-Version: 0.0.3
+Version: 0.0.4
 Summary: Easily use tailwind css with Flask projects
 Author-email: Sebastian Salinas <seba.salinas.delrio@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Sebastian Salinas Del Rio
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `flask_tailwind_manager-0.0.3/README.md` & `flask_tailwind_manager-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `flask_tailwind_manager-0.0.3/pyproject.toml` & `flask_tailwind_manager-0.0.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 [build-system]
-requires = ["setuptools>=61.0.0", "wheel"]
+requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
+[tool.setuptools]
+include-package-data = true
+
 [tool.setuptools.packages.find]
 where = ["src"]
 include = ["starter", "templates"]  # alternatively: `exclude = ["additional*"]`
 namespaces = false
 
 [project]
 name = "flask-tailwind-manager"
-version = "0.0.3"
+version = "0.0.4"
 description = "Easily use tailwind css with Flask projects"
 readme = "README.md"
 authors = [{ name = "Sebastian Salinas", email = "seba.salinas.delrio@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `flask_tailwind_manager-0.0.3/src/flask_tailwind/cli.py` & `flask_tailwind_manager-0.0.4/src/flask_tailwind/cli.py`

 * *Files identical despite different names*

### Comparing `flask_tailwind_manager-0.0.3/src/flask_tailwind/console.py` & `flask_tailwind_manager-0.0.4/src/flask_tailwind/console.py`

 * *Files identical despite different names*

### Comparing `flask_tailwind_manager-0.0.3/src/flask_tailwind/tailwind.py` & `flask_tailwind_manager-0.0.4/src/flask_tailwind/tailwind.py`

 * *Files identical despite different names*

### Comparing `flask_tailwind_manager-0.0.3/src/flask_tailwind_manager.egg-info/PKG-INFO` & `flask_tailwind_manager-0.0.4/src/flask_tailwind_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-tailwind-manager
-Version: 0.0.3
+Version: 0.0.4
 Summary: Easily use tailwind css with Flask projects
 Author-email: Sebastian Salinas <seba.salinas.delrio@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Sebastian Salinas Del Rio
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

