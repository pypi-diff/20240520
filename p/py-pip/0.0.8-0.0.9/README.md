# Comparing `tmp/py-pip-0.0.8.tar.gz` & `tmp/py-pip-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-pip-0.0.8.tar", last modified: Mon Dec 18 11:40:57 2023, max compression
+gzip compressed data, was "py-pip-0.0.9.tar", last modified: Mon Dec 18 12:26:29 2023, max compression
```

## Comparing `py-pip-0.0.8.tar` & `py-pip-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 11:40:57.412666 py-pip-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 11:40:57.408666 py-pip-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 11:40:57.412666 py-pip-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-12-18 11:40:47.000000 py-pip-0.0.8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2023-12-18 11:40:47.000000 py-pip-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2023-12-18 11:40:57.412666 py-pip-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2023-12-18 11:40:47.000000 py-pip-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 11:40:57.412666 py-pip-0.0.8/py_pip/
--rw-r--r--   0 runner    (1001) docker     (127)     7941 2023-12-18 11:40:47.000000 py-pip-0.0.8/py_pip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 11:40:57.412666 py-pip-0.0.8/py_pip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2023-12-18 11:40:57.000000 py-pip-0.0.8/py_pip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      240 2023-12-18 11:40:57.000000 py-pip-0.0.8/py_pip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-18 11:40:57.000000 py-pip-0.0.8/py_pip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-12-18 11:40:57.000000 py-pip-0.0.8/py_pip.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-18 11:40:57.000000 py-pip-0.0.8/py_pip.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      824 2023-12-18 11:40:47.000000 py-pip-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-18 11:40:57.412666 py-pip-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 12:26:29.066906 py-pip-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 12:26:29.062906 py-pip-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 12:26:29.066906 py-pip-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-12-18 12:26:15.000000 py-pip-0.0.9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2023-12-18 12:26:15.000000 py-pip-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2023-12-18 12:26:29.066906 py-pip-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2023-12-18 12:26:15.000000 py-pip-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 12:26:29.066906 py-pip-0.0.9/py_pip/
+-rw-r--r--   0 runner    (1001) docker     (127)     7990 2023-12-18 12:26:15.000000 py-pip-0.0.9/py_pip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 12:26:29.066906 py-pip-0.0.9/py_pip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2023-12-18 12:26:29.000000 py-pip-0.0.9/py_pip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2023-12-18 12:26:29.000000 py-pip-0.0.9/py_pip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-18 12:26:29.000000 py-pip-0.0.9/py_pip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2023-12-18 12:26:29.000000 py-pip-0.0.9/py_pip.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-18 12:26:29.000000 py-pip-0.0.9/py_pip.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2023-12-18 12:26:15.000000 py-pip-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-18 12:26:29.066906 py-pip-0.0.9/setup.cfg
```

### Comparing `py-pip-0.0.8/.github/workflows/python-publish.yml` & `py-pip-0.0.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `py-pip-0.0.8/.gitignore` & `py-pip-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `py-pip-0.0.8/PKG-INFO` & `py-pip-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-pip
-Version: 0.0.8
+Version: 0.0.9
 Summary: a PIP wrapper to install PyPI packages from inside Python
 Author: Hannes
 Project-URL: Homepage, https://github.com/hannesdelbeke/py-pip
 Project-URL: Source, https://github.com/hannesdelbeke/py-pip
 Keywords: manager,dcc,app
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.4
```

### Comparing `py-pip-0.0.8/README.md` & `py-pip-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `py-pip-0.0.8/py_pip/__init__.py` & `py-pip-0.0.9/py_pip/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,22 +13,27 @@
 
 _cached_installed_packages = []
 
 
 def _prep_env() -> dict:
     """Add custom python paths to the environment, to support dynamically added paths """
     my_env = os.environ.copy()
-    joined_paths = os.pathsep.join(sys.path)  # get all python paths
-    my_env["PYTHONPATH"] = joined_paths  # overwrite PYTHONPATH with all python paths, to avoid paths not in sys.path
+
+    # avoid paths not in sys.path passed to pip,
+    # e.g. paths set in PYTHONPATH, are ignored in apps like Blender. So shouldn't be passed to pip
+    my_env["PYTHONPATH"] = os.pathsep.join(sys.path)
 
     # clear paths, to avoid passing external python modules to pip
     for key in ["PATH", "PYTHONHOME", "PYTHONUSERBASE"]:
         if key in my_env:
             del my_env[key]
 
+    # prevent pip from using the user site
+    my_env["PYTHONNOUSERSITE"] = "1"
+
     return my_env
 
 
 def run_command_process(command) -> subprocess.Popen:
     """returns the subprocess, use to capture the output of the command while running"""
     my_env = _prep_env()
     return subprocess.Popen(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, env=my_env)
@@ -75,36 +80,35 @@
         packages = list()
     for name, version in packages:
         if name == package_name:
             return version
     return ""
     
 
-def get_location(package_name) -> str:
-    # TODO cleanup
-    def find_package_location(package_name):
+def get_location(package_name: str) -> "str|None":
+
+    # todo cleanup
+    def find_package_location(name: str) -> "str|None":
         try:
-            distribution = pkg_resources.get_distribution(package_name)
+            distribution = pkg_resources.get_distribution(name)
             return distribution.location
         except pkg_resources.DistributionNotFound:
-            return f"Package '{package_name}' not found."
-        
+            logging.warning(f"Package '{name}' not found.")
+            return None
+
     try:
         loader = pkgutil.get_loader(package_name)
         if loader is not None:
             package_location = os.path.dirname(loader.get_filename())
             return package_location
         else:
-            loc = find_package_location(package_name)
-            if loc:
-                return loc
-            else:
-                return f"Package '{package_name}' not found."
-    except ImportError:
-        return f"Error while trying to locate package '{package_name}'."
+            return find_package_location(package_name)
+    except ImportError as e:
+        logging.error(f"Error while trying to locate package '{package_name}'. Error: {e}")
+        return None
 
 
 def install_process(package_name: "str|List[str]"=None,
                     target_path: "str|pathlib.Path"=None,
                     force=False,
                     upgrade=False,
                     requirements=None,
```

### Comparing `py-pip-0.0.8/py_pip.egg-info/PKG-INFO` & `py-pip-0.0.9/py_pip.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-pip
-Version: 0.0.8
+Version: 0.0.9
 Summary: a PIP wrapper to install PyPI packages from inside Python
 Author: Hannes
 Project-URL: Homepage, https://github.com/hannesdelbeke/py-pip
 Project-URL: Source, https://github.com/hannesdelbeke/py-pip
 Keywords: manager,dcc,app
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.4
```

### Comparing `py-pip-0.0.8/pyproject.toml` & `py-pip-0.0.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3.7",
 ]
 #dynamic = ["dependencies"]
 dependencies = ['importlib-metadata; python_version<"3.7"']
 #dynamic = ["version"]
-version = "0.0.8"
+version = "0.0.9"
 
 #[project.optional-dependencies]
 #yaml = ["pyyaml"]
 
 #[project.scripts]
 #my-script = "my_package.module:function"
```

