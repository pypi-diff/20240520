# Comparing `tmp/ncompass-0.0.8.tar.gz` & `tmp/ncompass-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncompass-0.0.8.tar", last modified: Mon Mar  4 20:30:09 2024, max compression
+gzip compressed data, was "ncompass-0.0.9.tar", last modified: Tue Mar  5 03:05:32 2024, max compression
```

## Comparing `ncompass-0.0.8.tar` & `ncompass-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 adi       (1000) users      (100)        0 2024-03-04 20:30:09.467743 ncompass-0.0.8/
--rw-r--r--   0 adi       (1000) users      (100)    35149 2024-02-22 19:30:10.000000 ncompass-0.0.8/LICENSE
--rw-r--r--   0 adi       (1000) users      (100)     7036 2024-03-04 20:30:09.467743 ncompass-0.0.8/PKG-INFO
--rw-r--r--   0 adi       (1000) users      (100)     6361 2024-03-04 20:25:15.000000 ncompass-0.0.8/README.md
-drwxr-xr-x   0 adi       (1000) users      (100)        0 2024-03-04 20:30:09.466742 ncompass-0.0.8/ncompass/
--rw-r--r--   0 adi       (1000) users      (100)        0 2024-02-22 19:30:10.000000 ncompass-0.0.8/ncompass/__init__.py
--rw-r--r--   0 adi       (1000) users      (100)      876 2024-03-04 20:25:08.000000 ncompass-0.0.8/ncompass/async_utils.py
-drwxr-xr-x   0 adi       (1000) users      (100)        0 2024-03-04 20:30:09.466742 ncompass-0.0.8/ncompass/cli/
--rw-r--r--   0 adi       (1000) users      (100)       74 2024-02-26 21:38:30.000000 ncompass-0.0.8/ncompass/cli/__init__.py
--rw-r--r--   0 adi       (1000) users      (100)      544 2024-02-26 21:38:30.000000 ncompass-0.0.8/ncompass/cli/help.py
--rw-r--r--   0 adi       (1000) users      (100)      209 2024-02-26 21:55:18.000000 ncompass-0.0.8/ncompass/cli/start_session.py
--rw-r--r--   0 adi       (1000) users      (100)      205 2024-02-26 21:55:18.000000 ncompass-0.0.8/ncompass/cli/stop_session.py
-drwxr-xr-x   0 adi       (1000) users      (100)        0 2024-03-04 20:30:09.467743 ncompass-0.0.8/ncompass/client/
--rw-r--r--   0 adi       (1000) users      (100)       43 2024-02-22 19:30:10.000000 ncompass-0.0.8/ncompass/client/__init__.py
--rw-r--r--   0 adi       (1000) users      (100)     6144 2024-03-04 20:25:15.000000 ncompass-0.0.8/ncompass/client/client.py
-drwxr-xr-x   0 adi       (1000) users      (100)        0 2024-03-04 20:30:09.467743 ncompass-0.0.8/ncompass/client/functional/
--rw-r--r--   0 adi       (1000) users      (100)      323 2024-03-04 20:25:15.000000 ncompass-0.0.8/ncompass/client/functional/__init__.py
--rw-r--r--   0 adi       (1000) users      (100)     3976 2024-03-04 20:25:15.000000 ncompass-0.0.8/ncompass/client/functional/client.py
--rw-r--r--   0 adi       (1000) users      (100)      221 2024-02-28 22:08:24.000000 ncompass-0.0.8/ncompass/client/functional/model_health.py
--rw-r--r--   0 adi       (1000) users      (100)     5756 2024-03-04 20:25:15.000000 ncompass-0.0.8/ncompass/client/functional/run_prompt.py
--rw-r--r--   0 adi       (1000) users      (100)      956 2024-03-04 20:25:08.000000 ncompass-0.0.8/ncompass/errors.py
--rw-r--r--   0 adi       (1000) users      (100)      668 2024-03-04 20:25:08.000000 ncompass-0.0.8/ncompass/network_utils.py
-drwxr-xr-x   0 adi       (1000) users      (100)        0 2024-03-04 20:30:09.467743 ncompass-0.0.8/ncompass.egg-info/
--rw-r--r--   0 adi       (1000) users      (100)     7036 2024-03-04 20:30:09.000000 ncompass-0.0.8/ncompass.egg-info/PKG-INFO
--rw-r--r--   0 adi       (1000) users      (100)      635 2024-03-04 20:30:09.000000 ncompass-0.0.8/ncompass.egg-info/SOURCES.txt
--rw-r--r--   0 adi       (1000) users      (100)        1 2024-03-04 20:30:09.000000 ncompass-0.0.8/ncompass.egg-info/dependency_links.txt
--rw-r--r--   0 adi       (1000) users      (100)      160 2024-03-04 20:30:09.000000 ncompass-0.0.8/ncompass.egg-info/entry_points.txt
--rw-r--r--   0 adi       (1000) users      (100)       29 2024-03-04 20:30:09.000000 ncompass-0.0.8/ncompass.egg-info/requires.txt
--rw-r--r--   0 adi       (1000) users      (100)        9 2024-03-04 20:30:09.000000 ncompass-0.0.8/ncompass.egg-info/top_level.txt
--rw-r--r--   0 adi       (1000) users      (100)      824 2024-03-04 20:26:07.000000 ncompass-0.0.8/pyproject.toml
--rw-r--r--   0 adi       (1000) users      (100)       38 2024-03-04 20:30:09.467743 ncompass-0.0.8/setup.cfg
+drwxr-xr-x   0 adi       (1000) users      (100)        0 2024-03-05 03:05:32.177469 ncompass-0.0.9/
+-rw-r--r--   0 adi       (1000) users      (100)    35149 2024-02-22 19:30:10.000000 ncompass-0.0.9/LICENSE
+-rw-r--r--   0 adi       (1000) users      (100)     7036 2024-03-05 03:05:32.177469 ncompass-0.0.9/PKG-INFO
+-rw-r--r--   0 adi       (1000) users      (100)     6361 2024-03-04 20:40:11.000000 ncompass-0.0.9/README.md
+drwxr-xr-x   0 adi       (1000) users      (100)        0 2024-03-05 03:05:32.176469 ncompass-0.0.9/ncompass/
+-rw-r--r--   0 adi       (1000) users      (100)        0 2024-02-22 19:30:10.000000 ncompass-0.0.9/ncompass/__init__.py
+-rw-r--r--   0 adi       (1000) users      (100)      876 2024-03-05 03:00:11.000000 ncompass-0.0.9/ncompass/async_utils.py
+drwxr-xr-x   0 adi       (1000) users      (100)        0 2024-03-05 03:05:32.176469 ncompass-0.0.9/ncompass/cli/
+-rw-r--r--   0 adi       (1000) users      (100)       74 2024-02-26 21:38:30.000000 ncompass-0.0.9/ncompass/cli/__init__.py
+-rw-r--r--   0 adi       (1000) users      (100)      544 2024-02-26 21:38:30.000000 ncompass-0.0.9/ncompass/cli/help.py
+-rw-r--r--   0 adi       (1000) users      (100)      209 2024-02-26 21:55:18.000000 ncompass-0.0.9/ncompass/cli/start_session.py
+-rw-r--r--   0 adi       (1000) users      (100)      205 2024-02-26 21:55:18.000000 ncompass-0.0.9/ncompass/cli/stop_session.py
+drwxr-xr-x   0 adi       (1000) users      (100)        0 2024-03-05 03:05:32.176469 ncompass-0.0.9/ncompass/client/
+-rw-r--r--   0 adi       (1000) users      (100)       43 2024-02-22 19:30:10.000000 ncompass-0.0.9/ncompass/client/__init__.py
+-rw-r--r--   0 adi       (1000) users      (100)     6144 2024-03-05 03:00:11.000000 ncompass-0.0.9/ncompass/client/client.py
+drwxr-xr-x   0 adi       (1000) users      (100)        0 2024-03-05 03:05:32.177469 ncompass-0.0.9/ncompass/client/functional/
+-rw-r--r--   0 adi       (1000) users      (100)      323 2024-03-05 03:00:11.000000 ncompass-0.0.9/ncompass/client/functional/__init__.py
+-rw-r--r--   0 adi       (1000) users      (100)     4537 2024-03-05 03:00:11.000000 ncompass-0.0.9/ncompass/client/functional/client.py
+-rw-r--r--   0 adi       (1000) users      (100)      221 2024-02-28 22:08:24.000000 ncompass-0.0.9/ncompass/client/functional/model_health.py
+-rw-r--r--   0 adi       (1000) users      (100)     5756 2024-03-05 03:00:11.000000 ncompass-0.0.9/ncompass/client/functional/run_prompt.py
+-rw-r--r--   0 adi       (1000) users      (100)      956 2024-03-05 03:00:11.000000 ncompass-0.0.9/ncompass/errors.py
+-rw-r--r--   0 adi       (1000) users      (100)      668 2024-03-05 03:00:11.000000 ncompass-0.0.9/ncompass/network_utils.py
+drwxr-xr-x   0 adi       (1000) users      (100)        0 2024-03-05 03:05:32.177469 ncompass-0.0.9/ncompass.egg-info/
+-rw-r--r--   0 adi       (1000) users      (100)     7036 2024-03-05 03:05:32.000000 ncompass-0.0.9/ncompass.egg-info/PKG-INFO
+-rw-r--r--   0 adi       (1000) users      (100)      635 2024-03-05 03:05:32.000000 ncompass-0.0.9/ncompass.egg-info/SOURCES.txt
+-rw-r--r--   0 adi       (1000) users      (100)        1 2024-03-05 03:05:32.000000 ncompass-0.0.9/ncompass.egg-info/dependency_links.txt
+-rw-r--r--   0 adi       (1000) users      (100)      160 2024-03-05 03:05:32.000000 ncompass-0.0.9/ncompass.egg-info/entry_points.txt
+-rw-r--r--   0 adi       (1000) users      (100)       29 2024-03-05 03:05:32.000000 ncompass-0.0.9/ncompass.egg-info/requires.txt
+-rw-r--r--   0 adi       (1000) users      (100)        9 2024-03-05 03:05:32.000000 ncompass-0.0.9/ncompass.egg-info/top_level.txt
+-rw-r--r--   0 adi       (1000) users      (100)      824 2024-03-05 03:00:55.000000 ncompass-0.0.9/pyproject.toml
+-rw-r--r--   0 adi       (1000) users      (100)       38 2024-03-05 03:05:32.177469 ncompass-0.0.9/setup.cfg
```

### Comparing `ncompass-0.0.8/LICENSE` & `ncompass-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ncompass-0.0.8/PKG-INFO` & `ncompass-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncompass
-Version: 0.0.8
+Version: 0.0.9
 Summary: An API built to enable one-line-of-code access to accelerated open-source and custom AI models. 
 Author-email: "nCompass Technologies Inc." <admin@ncompass.tech>
 Project-URL: Homepage, https://github.com/nCompass-tech/nCompass
 Project-URL: Issues, https://github.com/nCompass-tech/nCompass/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `ncompass-0.0.8/README.md` & `ncompass-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ncompass-0.0.8/ncompass/async_utils.py` & `ncompass-0.0.9/ncompass/async_utils.py`

 * *Files identical despite different names*

### Comparing `ncompass-0.0.8/ncompass/cli/help.py` & `ncompass-0.0.9/ncompass/cli/help.py`

 * *Files identical despite different names*

### Comparing `ncompass-0.0.8/ncompass/client/client.py` & `ncompass-0.0.9/ncompass/client/client.py`

 * *Files identical despite different names*

### Comparing `ncompass-0.0.8/ncompass/client/functional/client.py` & `ncompass-0.0.9/ncompass/client/functional/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,18 +17,32 @@
 
 async def close_session(session):
     return await session.close()
 
 async def create_session():
     return aiohttp.ClientSession()
 
+def warmup_prompt(session, url, api_key, event_loop):
+    wait_until_model_running(url, api_key, timeout=2)
+    for _ in complete_prompt(session
+                             , url
+                             , api_key
+                             , prompt=''
+                             , max_tokens=1
+                             , temperature=0.1
+                             , top_p=0.9
+                             , stream=True
+                             , event_loop=event_loop):
+        pass
+
 def start_session(url, api_key, event_loop=None):
     session = run_in_event_loop(create_session(), event_loop)
     try:
         start_stop_handler(get(f'{url}/start_session', {'Authorization': api_key}))
+        warmup_prompt(session, url, api_key, event_loop)
         return session
     except Exception as e:
         run_in_event_loop(close_session(session), event_loop)
         raise e
 
 def stop_session(url, api_key, session, event_loop=None):
     if session is not None: run_in_event_loop(close_session(session), event_loop)
```

### Comparing `ncompass-0.0.8/ncompass/client/functional/run_prompt.py` & `ncompass-0.0.9/ncompass/client/functional/run_prompt.py`

 * *Files identical despite different names*

### Comparing `ncompass-0.0.8/ncompass/errors.py` & `ncompass-0.0.9/ncompass/errors.py`

 * *Files identical despite different names*

### Comparing `ncompass-0.0.8/ncompass/network_utils.py` & `ncompass-0.0.9/ncompass/network_utils.py`

 * *Files identical despite different names*

### Comparing `ncompass-0.0.8/ncompass.egg-info/PKG-INFO` & `ncompass-0.0.9/ncompass.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncompass
-Version: 0.0.8
+Version: 0.0.9
 Summary: An API built to enable one-line-of-code access to accelerated open-source and custom AI models. 
 Author-email: "nCompass Technologies Inc." <admin@ncompass.tech>
 Project-URL: Homepage, https://github.com/nCompass-tech/nCompass
 Project-URL: Issues, https://github.com/nCompass-tech/nCompass/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `ncompass-0.0.8/ncompass.egg-info/SOURCES.txt` & `ncompass-0.0.9/ncompass.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ncompass-0.0.8/pyproject.toml` & `ncompass-0.0.9/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ncompass"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="nCompass Technologies Inc.", email="admin@ncompass.tech" },
 ]
 description = "An API built to enable one-line-of-code access to accelerated open-source and custom AI models. "
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

