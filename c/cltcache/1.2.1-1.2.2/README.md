# Comparing `tmp/cltcache-1.2.1.tar.gz` & `tmp/cltcache-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cltcache-1.2.1.tar", last modified: Mon Feb 19 12:15:10 2024, max compression
+gzip compressed data, was "cltcache-1.2.2.tar", last modified: Mon May 20 12:20:34 2024, max compression
```

## Comparing `cltcache-1.2.1.tar` & `cltcache-1.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:15:10.957123 cltcache-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-02-19 12:15:02.000000 cltcache-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-02-19 12:15:10.957123 cltcache-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-02-19 12:15:02.000000 cltcache-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-19 12:15:02.000000 cltcache-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-02-19 12:15:10.957123 cltcache-1.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:15:10.953123 cltcache-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:15:10.957123 cltcache-1.2.1/src/cltcache/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 12:15:02.000000 cltcache-1.2.1/src/cltcache/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7261 2024-02-19 12:15:02.000000 cltcache-1.2.1/src/cltcache/cltcache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:15:10.957123 cltcache-1.2.1/src/cltcache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-02-19 12:15:10.000000 cltcache-1.2.1/src/cltcache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-02-19 12:15:10.000000 cltcache-1.2.1/src/cltcache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 12:15:10.000000 cltcache-1.2.1/src/cltcache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-19 12:15:10.000000 cltcache-1.2.1/src/cltcache.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-19 12:15:10.000000 cltcache-1.2.1/src/cltcache.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:20:34.182778 cltcache-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-20 12:20:27.000000 cltcache-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-05-20 12:20:34.182778 cltcache-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-05-20 12:20:27.000000 cltcache-1.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-20 12:20:27.000000 cltcache-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-20 12:20:34.182778 cltcache-1.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:20:34.182778 cltcache-1.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:20:34.182778 cltcache-1.2.2/src/cltcache/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 12:20:27.000000 cltcache-1.2.2/src/cltcache/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7273 2024-05-20 12:20:27.000000 cltcache-1.2.2/src/cltcache/cltcache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:20:34.182778 cltcache-1.2.2/src/cltcache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-05-20 12:20:34.000000 cltcache-1.2.2/src/cltcache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-20 12:20:34.000000 cltcache-1.2.2/src/cltcache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 12:20:34.000000 cltcache-1.2.2/src/cltcache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-20 12:20:34.000000 cltcache-1.2.2/src/cltcache.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-20 12:20:34.000000 cltcache-1.2.2/src/cltcache.egg-info/top_level.txt
```

### Comparing `cltcache-1.2.1/LICENSE` & `cltcache-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cltcache-1.2.1/PKG-INFO` & `cltcache-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cltcache
-Version: 1.2.1
+Version: 1.2.2
 Home-page: https://github.com/freedick/cltcache
 Author: Fredrik Nordin
 Author-email: freddan007@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.6
```

### Comparing `cltcache-1.2.1/README.md` & `cltcache-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `cltcache-1.2.1/setup.cfg` & `cltcache-1.2.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cltcache
-version = 1.2.1
+version = 1.2.2
 author = Fredrik Nordin
 author_email = freddan007@gmail.com
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/freedick/cltcache
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `cltcache-1.2.1/src/cltcache/cltcache.py` & `cltcache-1.2.2/src/cltcache/cltcache.py`

 * *Files 6% similar despite different names*

```diff
@@ -122,19 +122,19 @@
 
     preproc_hash = get_preproc_hash(compile_args, config)
 
     version_out = run_get_stdout([clang_tidy] + ["--version"])
     version = ",".join(re.findall(r'[0-9]+\.[0-9]+\.?[0-9]*', version_out))
     version_hash = sha256(version)
 
-    enabled_checks = run_get_stdout(
-        [clang_tidy] + clang_tidy_args + ["--list-checks"])
-    enabled_checks_hash = sha256(enabled_checks)
+    clang_tidy_config = run_get_stdout(
+        [clang_tidy] + clang_tidy_args + ["--dump-config"])
+    clang_tidy_config_hash = sha256(clang_tidy_config)
 
-    return sha256(preproc_hash + enabled_checks_hash + version_hash)[:-16]
+    return sha256(preproc_hash + clang_tidy_config_hash + version_hash)[:-16]
 
 
 def init_cltcache():
     cltcache_path = os.environ.get(
         "CLTCACHE_DIR", pathlib.Path().home() / ".cltcache")
     cltcache_path.mkdir(parents=True, exist_ok=True)
     config = configparser.ConfigParser()
```

### Comparing `cltcache-1.2.1/src/cltcache.egg-info/PKG-INFO` & `cltcache-1.2.2/src/cltcache.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cltcache
-Version: 1.2.1
+Version: 1.2.2
 Home-page: https://github.com/freedick/cltcache
 Author: Fredrik Nordin
 Author-email: freddan007@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.6
```

