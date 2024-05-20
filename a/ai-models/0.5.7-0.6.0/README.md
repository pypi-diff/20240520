# Comparing `tmp/ai_models-0.5.7.tar.gz` & `tmp/ai_models-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_models-0.5.7.tar", last modified: Tue May 14 14:18:51 2024, max compression
+gzip compressed data, was "ai_models-0.6.0.tar", last modified: Mon May 20 08:02:43 2024, max compression
```

## Comparing `ai_models-0.5.7.tar` & `ai_models-0.6.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:51.652944 ai_models-0.5.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:51.648944 ai_models-0.5.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:51.652944 ai_models-0.5.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-14 14:18:42.000000 ai_models-0.5.7/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-14 14:18:42.000000 ai_models-0.5.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-14 14:18:42.000000 ai_models-0.5.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-14 14:18:42.000000 ai_models-0.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14197 2024-05-14 14:18:51.652944 ai_models-0.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-05-14 14:18:42.000000 ai_models-0.5.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-14 14:18:42.000000 ai_models-0.5.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 14:18:51.652944 ai_models-0.5.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:51.648944 ai_models-0.5.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:51.652944 ai_models-0.5.7/src/ai_models/
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-14 14:18:42.000000 ai_models-0.5.7/src/ai_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9507 2024-05-14 14:18:42.000000 ai_models-0.5.7/src/ai_models/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-14 14:18:51.000000 ai_models-0.5.7/src/ai_models/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-14 14:18:42.000000 ai_models-0.5.7/src/ai_models/checkpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:51.652944 ai_models-0.5.7/src/ai_models/inputs/
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-05-14 14:18:42.000000 ai_models-0.5.7/src/ai_models/inputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16159 2024-05-14 14:18:42.000000 ai_models-0.5.7/src/ai_models/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:51.652944 ai_models-0.5.7/src/ai_models/outputs/
--rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-05-14 14:18:42.000000 ai_models-0.5.7/src/ai_models/outputs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:51.652944 ai_models-0.5.7/src/ai_models/remote/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-14 14:18:42.000000 ai_models-0.5.7/src/ai_models/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-14 14:18:42.000000 ai_models-0.5.7/src/ai_models/remote/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-14 14:18:42.000000 ai_models-0.5.7/src/ai_models/remote/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-14 14:18:42.000000 ai_models-0.5.7/src/ai_models/remote/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-14 14:18:42.000000 ai_models-0.5.7/src/ai_models/stepper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:51.652944 ai_models-0.5.7/src/ai_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14197 2024-05-14 14:18:51.000000 ai_models-0.5.7/src/ai_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-14 14:18:51.000000 ai_models-0.5.7/src/ai_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 14:18:51.000000 ai_models-0.5.7/src/ai_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-14 14:18:51.000000 ai_models-0.5.7/src/ai_models.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-14 14:18:51.000000 ai_models-0.5.7/src/ai_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 14:18:51.000000 ai_models-0.5.7/src/ai_models.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:51.652944 ai_models-0.5.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-14 14:18:42.000000 ai_models-0.5.7/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-14 14:18:42.000000 ai_models-0.5.7/tests/test_code.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:02:43.422384 ai_models-0.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:02:43.418384 ai_models-0.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:02:43.418384 ai_models-0.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-20 08:02:32.000000 ai_models-0.6.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-20 08:02:32.000000 ai_models-0.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-20 08:02:32.000000 ai_models-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-20 08:02:32.000000 ai_models-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14197 2024-05-20 08:02:43.422384 ai_models-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-05-20 08:02:32.000000 ai_models-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-20 08:02:32.000000 ai_models-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 08:02:43.422384 ai_models-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:02:43.418384 ai_models-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:02:43.418384 ai_models-0.6.0/src/ai_models/
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-20 08:02:32.000000 ai_models-0.6.0/src/ai_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9507 2024-05-20 08:02:32.000000 ai_models-0.6.0/src/ai_models/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-20 08:02:43.000000 ai_models-0.6.0/src/ai_models/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-20 08:02:32.000000 ai_models-0.6.0/src/ai_models/checkpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:02:43.422384 ai_models-0.6.0/src/ai_models/inputs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-05-20 08:02:32.000000 ai_models-0.6.0/src/ai_models/inputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16292 2024-05-20 08:02:32.000000 ai_models-0.6.0/src/ai_models/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:02:43.422384 ai_models-0.6.0/src/ai_models/outputs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-05-20 08:02:32.000000 ai_models-0.6.0/src/ai_models/outputs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:02:43.422384 ai_models-0.6.0/src/ai_models/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-20 08:02:32.000000 ai_models-0.6.0/src/ai_models/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-20 08:02:32.000000 ai_models-0.6.0/src/ai_models/remote/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-20 08:02:32.000000 ai_models-0.6.0/src/ai_models/remote/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-20 08:02:32.000000 ai_models-0.6.0/src/ai_models/remote/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-20 08:02:32.000000 ai_models-0.6.0/src/ai_models/stepper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:02:43.422384 ai_models-0.6.0/src/ai_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14197 2024-05-20 08:02:43.000000 ai_models-0.6.0/src/ai_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-20 08:02:43.000000 ai_models-0.6.0/src/ai_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 08:02:43.000000 ai_models-0.6.0/src/ai_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-20 08:02:43.000000 ai_models-0.6.0/src/ai_models.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-20 08:02:43.000000 ai_models-0.6.0/src/ai_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 08:02:43.000000 ai_models-0.6.0/src/ai_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:02:43.422384 ai_models-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-20 08:02:32.000000 ai_models-0.6.0/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-20 08:02:32.000000 ai_models-0.6.0/tests/test_code.py
```

### Comparing `ai_models-0.5.7/.github/workflows/python-publish.yml` & `ai_models-0.6.0/.github/workflows/python-publish.yml`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,17 @@
     steps:
     # - run: sudo apt-get install -y pandoc # Needed by sphinx for notebooks
     - uses: actions/checkout@v4
     - uses: actions/setup-python@v5
       with:
         python-version: 3.x
     - uses: pre-commit/action@v3.0.1
+      env:
+        SKIP: no-commit-to-branch
+
 
   checks:
     strategy:
       fail-fast: false
       matrix:
         platform: ["ubuntu-latest", "macos-latest"]
         python-version: ["3.10"]
```

### Comparing `ai_models-0.5.7/.gitignore` & `ai_models-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ai_models-0.5.7/.pre-commit-config.yaml` & `ai_models-0.6.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ai_models-0.5.7/LICENSE` & `ai_models-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ai_models-0.5.7/PKG-INFO` & `ai_models-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-models
-Version: 0.5.7
+Version: 0.6.0
 Summary: A package to run AI weather models.
 Author-email: "European Centre for Medium-Range Weather Forecasts (ECMWF)" <software.support@ecmwf.int>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `ai_models-0.5.7/README.md` & `ai_models-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ai_models-0.5.7/pyproject.toml` & `ai_models-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ai_models-0.5.7/src/ai_models/__main__.py` & `ai_models-0.6.0/src/ai_models/__main__.py`

 * *Files identical despite different names*

### Comparing `ai_models-0.5.7/src/ai_models/checkpoint.py` & `ai_models-0.6.0/src/ai_models/checkpoint.py`

 * *Files identical despite different names*

### Comparing `ai_models-0.5.7/src/ai_models/inputs/__init__.py` & `ai_models-0.6.0/src/ai_models/inputs/__init__.py`

 * *Files identical despite different names*

### Comparing `ai_models-0.5.7/src/ai_models/model.py` & `ai_models-0.6.0/src/ai_models/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -322,15 +322,20 @@
             print(file)
 
     def _print_request(self, verb, request, file=sys.stdout):
         r = [verb]
         for k, v in sorted(request.items()):
             if not isinstance(v, (list, tuple, set)):
                 v = [v]
-            v = [str(_) for _ in sorted(v)]
+
+            if k in ("area", "grid", "frame", "rotation", "bitmap"):
+                v = [str(_) for _ in v]
+            else:
+                v = [str(_) for _ in sorted(v)]
+
             v = "/".join(v)
             r.append(f"{k}={v}")
 
         r = ",\n   ".join(r)
         print(r, file=file)
         print(file=file)
```

### Comparing `ai_models-0.5.7/src/ai_models/outputs/__init__.py` & `ai_models-0.6.0/src/ai_models/outputs/__init__.py`

 * *Files identical despite different names*

### Comparing `ai_models-0.5.7/src/ai_models/remote/api.py` & `ai_models-0.6.0/src/ai_models/remote/api.py`

 * *Files identical despite different names*

### Comparing `ai_models-0.5.7/src/ai_models/remote/config.py` & `ai_models-0.6.0/src/ai_models/remote/config.py`

 * *Files identical despite different names*

### Comparing `ai_models-0.5.7/src/ai_models/remote/model.py` & `ai_models-0.6.0/src/ai_models/remote/model.py`

 * *Files identical despite different names*

### Comparing `ai_models-0.5.7/src/ai_models/stepper.py` & `ai_models-0.6.0/src/ai_models/stepper.py`

 * *Files identical despite different names*

### Comparing `ai_models-0.5.7/src/ai_models.egg-info/PKG-INFO` & `ai_models-0.6.0/src/ai_models.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-models
-Version: 0.5.7
+Version: 0.6.0
 Summary: A package to run AI weather models.
 Author-email: "European Centre for Medium-Range Weather Forecasts (ECMWF)" <software.support@ecmwf.int>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `ai_models-0.5.7/src/ai_models.egg-info/SOURCES.txt` & `ai_models-0.6.0/src/ai_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

