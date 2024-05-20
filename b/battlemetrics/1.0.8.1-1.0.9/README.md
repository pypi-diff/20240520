# Comparing `tmp/battlemetrics-1.0.8.1.tar.gz` & `tmp/battlemetrics-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "battlemetrics-1.0.8.1.tar", last modified: Sat May 18 08:36:16 2024, max compression
+gzip compressed data, was "battlemetrics-1.0.9.tar", last modified: Sat May 18 08:37:15 2024, max compression
```

## Comparing `battlemetrics-1.0.8.1.tar` & `battlemetrics-1.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 08:36:16.291317 battlemetrics-1.0.8.1/
--rw-rw-rw-   0        0        0     3652 2024-05-18 08:36:16.290317 battlemetrics-1.0.8.1/PKG-INFO
--rw-rw-rw-   0        0        0     2870 2024-02-18 07:17:58.000000 battlemetrics-1.0.8.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 08:36:16.240992 battlemetrics-1.0.8.1/battlemetrics/
--rw-rw-rw-   0        0        0     5446 2024-02-18 07:05:35.000000 battlemetrics-1.0.8.1/battlemetrics/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-18 08:36:16.285311 battlemetrics-1.0.8.1/battlemetrics/components/
--rw-rw-rw-   0        0        0    21143 2024-02-14 11:12:24.000000 battlemetrics-1.0.8.1/battlemetrics/components/banlist.py
--rw-rw-rw-   0        0        0     6054 2024-02-14 12:00:23.000000 battlemetrics-1.0.8.1/battlemetrics/components/bans.py
--rw-rw-rw-   0        0        0     4869 2024-02-13 09:08:30.000000 battlemetrics-1.0.8.1/battlemetrics/components/flags.py
--rw-rw-rw-   0        0        0     3074 2024-02-13 09:08:30.000000 battlemetrics-1.0.8.1/battlemetrics/components/gameinfo.py
--rw-rw-rw-   0        0        0    11749 2024-02-25 13:58:26.000000 battlemetrics-1.0.8.1/battlemetrics/components/helpers.py
--rw-rw-rw-   0        0        0     3962 2024-02-19 03:47:02.000000 battlemetrics-1.0.8.1/battlemetrics/components/notes.py
--rw-rw-rw-   0        0        0    13151 2024-04-21 13:00:34.000000 battlemetrics-1.0.8.1/battlemetrics/components/organization.py
--rw-rw-rw-   0        0        0    20573 2024-02-19 03:46:02.000000 battlemetrics-1.0.8.1/battlemetrics/components/player.py
--rw-rw-rw-   0        0        0    27136 2024-05-18 08:35:25.000000 battlemetrics-1.0.8.1/battlemetrics/components/server.py
--rw-rw-rw-   0        0        0     2505 2024-02-13 09:08:30.000000 battlemetrics-1.0.8.1/battlemetrics/components/session.py
-drwxrwxrwx   0        0        0        0 2024-05-18 08:36:16.288314 battlemetrics-1.0.8.1/battlemetrics.egg-info/
--rw-rw-rw-   0        0        0     3652 2024-05-18 08:36:16.000000 battlemetrics-1.0.8.1/battlemetrics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      591 2024-05-18 08:36:16.000000 battlemetrics-1.0.8.1/battlemetrics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 08:36:16.000000 battlemetrics-1.0.8.1/battlemetrics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-18 08:36:16.000000 battlemetrics-1.0.8.1/battlemetrics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-18 08:36:16.000000 battlemetrics-1.0.8.1/battlemetrics.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      873 2024-05-18 08:35:53.000000 battlemetrics-1.0.8.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-18 08:36:16.292317 battlemetrics-1.0.8.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-18 08:37:15.746771 battlemetrics-1.0.9/
+-rw-rw-rw-   0        0        0     3650 2024-05-18 08:37:15.745770 battlemetrics-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2870 2024-02-18 07:17:58.000000 battlemetrics-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 08:37:15.670300 battlemetrics-1.0.9/battlemetrics/
+-rw-rw-rw-   0        0        0     5446 2024-02-18 07:05:35.000000 battlemetrics-1.0.9/battlemetrics/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 08:37:15.741767 battlemetrics-1.0.9/battlemetrics/components/
+-rw-rw-rw-   0        0        0    21143 2024-02-14 11:12:24.000000 battlemetrics-1.0.9/battlemetrics/components/banlist.py
+-rw-rw-rw-   0        0        0     6054 2024-02-14 12:00:23.000000 battlemetrics-1.0.9/battlemetrics/components/bans.py
+-rw-rw-rw-   0        0        0     4869 2024-02-13 09:08:30.000000 battlemetrics-1.0.9/battlemetrics/components/flags.py
+-rw-rw-rw-   0        0        0     3074 2024-02-13 09:08:30.000000 battlemetrics-1.0.9/battlemetrics/components/gameinfo.py
+-rw-rw-rw-   0        0        0    11749 2024-02-25 13:58:26.000000 battlemetrics-1.0.9/battlemetrics/components/helpers.py
+-rw-rw-rw-   0        0        0     3962 2024-02-19 03:47:02.000000 battlemetrics-1.0.9/battlemetrics/components/notes.py
+-rw-rw-rw-   0        0        0    13151 2024-04-21 13:00:34.000000 battlemetrics-1.0.9/battlemetrics/components/organization.py
+-rw-rw-rw-   0        0        0    20573 2024-02-19 03:46:02.000000 battlemetrics-1.0.9/battlemetrics/components/player.py
+-rw-rw-rw-   0        0        0    27136 2024-05-18 08:35:25.000000 battlemetrics-1.0.9/battlemetrics/components/server.py
+-rw-rw-rw-   0        0        0     2505 2024-02-13 09:08:30.000000 battlemetrics-1.0.9/battlemetrics/components/session.py
+drwxrwxrwx   0        0        0        0 2024-05-18 08:37:15.743769 battlemetrics-1.0.9/battlemetrics.egg-info/
+-rw-rw-rw-   0        0        0     3650 2024-05-18 08:37:15.000000 battlemetrics-1.0.9/battlemetrics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      591 2024-05-18 08:37:15.000000 battlemetrics-1.0.9/battlemetrics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 08:37:15.000000 battlemetrics-1.0.9/battlemetrics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-18 08:37:15.000000 battlemetrics-1.0.9/battlemetrics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-18 08:37:15.000000 battlemetrics-1.0.9/battlemetrics.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      871 2024-05-18 08:36:56.000000 battlemetrics-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-18 08:37:15.747772 battlemetrics-1.0.9/setup.cfg
```

### Comparing `battlemetrics-1.0.8.1/PKG-INFO` & `battlemetrics-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: battlemetrics
-Version: 1.0.8.1
+Version: 1.0.9
 Summary: Battlemetrics API wrapper.
 Author-email: Gnomeslayer <declan.otten@live.com.au>
 Project-URL: Homepage, https://github.com/Gnomeslayer/battlemetrics
 Keywords: battlemetrics,battlemetricsapi,api,gaming
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `battlemetrics-1.0.8.1/README.md` & `battlemetrics-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `battlemetrics-1.0.8.1/battlemetrics/__init__.py` & `battlemetrics-1.0.9/battlemetrics/__init__.py`

 * *Files identical despite different names*

### Comparing `battlemetrics-1.0.8.1/battlemetrics/components/banlist.py` & `battlemetrics-1.0.9/battlemetrics/components/banlist.py`

 * *Files identical despite different names*

### Comparing `battlemetrics-1.0.8.1/battlemetrics/components/bans.py` & `battlemetrics-1.0.9/battlemetrics/components/bans.py`

 * *Files identical despite different names*

### Comparing `battlemetrics-1.0.8.1/battlemetrics/components/flags.py` & `battlemetrics-1.0.9/battlemetrics/components/flags.py`

 * *Files identical despite different names*

### Comparing `battlemetrics-1.0.8.1/battlemetrics/components/gameinfo.py` & `battlemetrics-1.0.9/battlemetrics/components/gameinfo.py`

 * *Files identical despite different names*

### Comparing `battlemetrics-1.0.8.1/battlemetrics/components/helpers.py` & `battlemetrics-1.0.9/battlemetrics/components/helpers.py`

 * *Files identical despite different names*

### Comparing `battlemetrics-1.0.8.1/battlemetrics/components/notes.py` & `battlemetrics-1.0.9/battlemetrics/components/notes.py`

 * *Files identical despite different names*

### Comparing `battlemetrics-1.0.8.1/battlemetrics/components/organization.py` & `battlemetrics-1.0.9/battlemetrics/components/organization.py`

 * *Files identical despite different names*

### Comparing `battlemetrics-1.0.8.1/battlemetrics/components/player.py` & `battlemetrics-1.0.9/battlemetrics/components/player.py`

 * *Files identical despite different names*

### Comparing `battlemetrics-1.0.8.1/battlemetrics/components/server.py` & `battlemetrics-1.0.9/battlemetrics/components/server.py`

 * *Files identical despite different names*

### Comparing `battlemetrics-1.0.8.1/battlemetrics/components/session.py` & `battlemetrics-1.0.9/battlemetrics/components/session.py`

 * *Files identical despite different names*

### Comparing `battlemetrics-1.0.8.1/battlemetrics.egg-info/PKG-INFO` & `battlemetrics-1.0.9/battlemetrics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: battlemetrics
-Version: 1.0.8.1
+Version: 1.0.9
 Summary: Battlemetrics API wrapper.
 Author-email: Gnomeslayer <declan.otten@live.com.au>
 Project-URL: Homepage, https://github.com/Gnomeslayer/battlemetrics
 Keywords: battlemetrics,battlemetricsapi,api,gaming
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `battlemetrics-1.0.8.1/battlemetrics.egg-info/SOURCES.txt` & `battlemetrics-1.0.9/battlemetrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `battlemetrics-1.0.8.1/pyproject.toml` & `battlemetrics-1.0.9/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "battlemetrics"
 description = "Battlemetrics API wrapper."
-version = "1.0.8.1"
+version = "1.0.9"
 authors = [{ name = "Gnomeslayer", email = "declan.otten@live.com.au" }]
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
```

