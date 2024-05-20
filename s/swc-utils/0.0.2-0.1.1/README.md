# Comparing `tmp/swc_utils-0.0.2.tar.gz` & `tmp/swc_utils-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swc_utils-0.0.2.tar", last modified: Sun May 19 13:06:06 2024, max compression
+gzip compressed data, was "swc_utils-0.1.1.tar", last modified: Mon May 20 13:17:58 2024, max compression
```

## Comparing `swc_utils-0.0.2.tar` & `swc_utils-0.1.1.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 13:06:06.810676 swc_utils-0.0.2/
--rw-rw-rw-   0        0        0     1090 2024-05-18 12:05:04.000000 swc_utils-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      711 2024-05-19 13:06:06.809675 swc_utils-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       85 2024-05-18 12:04:37.000000 swc_utils-0.0.2/README.md
--rw-rw-rw-   0        0        0      704 2024-05-19 13:05:37.000000 swc_utils-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-19 13:06:06.810676 swc_utils-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-19 13:06:06.787674 swc_utils-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-19 13:06:06.791676 swc_utils-0.0.2/src/swc_utils/
--rw-rw-rw-   0        0        0        0 2024-05-18 12:00:49.000000 swc_utils-0.0.2/src/swc_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 13:06:06.800676 swc_utils-0.0.2/src/swc_utils/database/
--rw-rw-rw-   0        0        0      105 2024-05-18 12:15:55.000000 swc_utils-0.0.2/src/swc_utils/database/__init__.py
--rw-rw-rw-   0        0        0     1068 2024-04-27 15:30:53.000000 swc_utils-0.0.2/src/swc_utils/database/connection_profile.py
--rw-rw-rw-   0        0        0      493 2024-05-18 12:01:51.000000 swc_utils-0.0.2/src/swc_utils/database/database_connection.py
-drwxrwxrwx   0        0        0        0 2024-05-19 13:06:06.802676 swc_utils-0.0.2/src/swc_utils/other/
--rw-rw-rw-   0        0        0       63 2024-05-18 12:34:45.000000 swc_utils-0.0.2/src/swc_utils/other/__init__.py
--rw-rw-rw-   0        0        0      619 2024-04-25 14:33:38.000000 swc_utils-0.0.2/src/swc_utils/other/generator_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-19 13:06:06.804675 swc_utils-0.0.2/src/swc_utils/tools/
--rw-rw-rw-   0        0        0       67 2024-05-18 12:34:45.000000 swc_utils-0.0.2/src/swc_utils/tools/__init__.py
--rw-rw-rw-   0        0        0      914 2023-06-03 18:25:42.000000 swc_utils-0.0.2/src/swc_utils/tools/config.py
--rw-rw-rw-   0        0        0      512 2024-04-25 14:07:54.000000 swc_utils-0.0.2/src/swc_utils/tools/route_loader.py
-drwxrwxrwx   0        0        0        0 2024-05-19 13:06:06.806676 swc_utils-0.0.2/src/swc_utils/web/
--rw-rw-rw-   0        0        0      186 2024-05-18 12:34:45.000000 swc_utils-0.0.2/src/swc_utils/web/__init__.py
--rw-rw-rw-   0        0        0      542 2024-05-18 12:34:45.000000 swc_utils-0.0.2/src/swc_utils/web/adv_responses.py
--rw-rw-rw-   0        0        0     1044 2024-05-18 12:34:45.000000 swc_utils-0.0.2/src/swc_utils/web/auth_manager.py
--rw-rw-rw-   0        0        0     2524 2023-02-28 00:29:50.000000 swc_utils-0.0.2/src/swc_utils/web/request_codes.py
-drwxrwxrwx   0        0        0        0 2024-05-19 13:06:06.808678 swc_utils-0.0.2/src/swc_utils/wsl/
--rw-rw-rw-   0        0        0       87 2024-05-18 12:34:45.000000 swc_utils-0.0.2/src/swc_utils/wsl/__init__.py
--rw-rw-rw-   0        0        0      663 2024-05-18 12:34:45.000000 swc_utils-0.0.2/src/swc_utils/wsl/wsl_compatability.py
-drwxrwxrwx   0        0        0        0 2024-05-19 13:06:06.809675 swc_utils-0.0.2/src/swc_utils.egg-info/
--rw-rw-rw-   0        0        0      711 2024-05-19 13:06:06.000000 swc_utils-0.0.2/src/swc_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      740 2024-05-19 13:06:06.000000 swc_utils-0.0.2/src/swc_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 13:06:06.000000 swc_utils-0.0.2/src/swc_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-05-19 13:06:06.000000 swc_utils-0.0.2/src/swc_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-19 13:06:06.000000 swc_utils-0.0.2/src/swc_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-20 13:17:58.301604 swc_utils-0.1.1/
+-rw-rw-rw-   0        0        0     1090 2024-05-18 12:05:04.000000 swc_utils-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      711 2024-05-20 13:17:58.300604 swc_utils-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       85 2024-05-18 12:04:37.000000 swc_utils-0.1.1/README.md
+-rw-rw-rw-   0        0        0      704 2024-05-20 13:17:50.000000 swc_utils-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-20 13:17:58.301604 swc_utils-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 13:17:58.282606 swc_utils-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-20 13:17:58.285604 swc_utils-0.1.1/src/swc_utils/
+-rw-rw-rw-   0        0        0        0 2024-05-18 12:00:49.000000 swc_utils-0.1.1/src/swc_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 13:17:58.292604 swc_utils-0.1.1/src/swc_utils/database/
+-rw-rw-rw-   0        0        0      105 2024-05-18 12:15:55.000000 swc_utils-0.1.1/src/swc_utils/database/__init__.py
+-rw-rw-rw-   0        0        0     1068 2024-04-27 15:30:53.000000 swc_utils-0.1.1/src/swc_utils/database/connection_profile.py
+-rw-rw-rw-   0        0        0      493 2024-05-18 12:01:51.000000 swc_utils-0.1.1/src/swc_utils/database/database_connection.py
+-rw-rw-rw-   0        0        0     3275 2024-05-20 13:10:50.000000 swc_utils-0.1.1/src/swc_utils/database/db_table_care.py
+drwxrwxrwx   0        0        0        0 2024-05-20 13:17:58.293604 swc_utils-0.1.1/src/swc_utils/other/
+-rw-rw-rw-   0        0        0       63 2024-05-18 12:34:45.000000 swc_utils-0.1.1/src/swc_utils/other/__init__.py
+-rw-rw-rw-   0        0        0      619 2024-04-25 14:33:38.000000 swc_utils-0.1.1/src/swc_utils/other/generator_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-20 13:17:58.295604 swc_utils-0.1.1/src/swc_utils/tools/
+-rw-rw-rw-   0        0        0       67 2024-05-18 12:34:45.000000 swc_utils-0.1.1/src/swc_utils/tools/__init__.py
+-rw-rw-rw-   0        0        0      914 2023-06-03 18:25:42.000000 swc_utils-0.1.1/src/swc_utils/tools/config.py
+-rw-rw-rw-   0        0        0      512 2024-04-25 14:07:54.000000 swc_utils-0.1.1/src/swc_utils/tools/route_loader.py
+drwxrwxrwx   0        0        0        0 2024-05-20 13:17:58.298604 swc_utils-0.1.1/src/swc_utils/web/
+-rw-rw-rw-   0        0        0      186 2024-05-18 12:34:45.000000 swc_utils-0.1.1/src/swc_utils/web/__init__.py
+-rw-rw-rw-   0        0        0      542 2024-05-18 12:34:45.000000 swc_utils-0.1.1/src/swc_utils/web/adv_responses.py
+-rw-rw-rw-   0        0        0     1044 2024-05-18 12:34:45.000000 swc_utils-0.1.1/src/swc_utils/web/auth_manager.py
+-rw-rw-rw-   0        0        0     2524 2023-02-28 00:29:50.000000 swc_utils-0.1.1/src/swc_utils/web/request_codes.py
+drwxrwxrwx   0        0        0        0 2024-05-20 13:17:58.299604 swc_utils-0.1.1/src/swc_utils/wsl/
+-rw-rw-rw-   0        0        0       87 2024-05-18 12:34:45.000000 swc_utils-0.1.1/src/swc_utils/wsl/__init__.py
+-rw-rw-rw-   0        0        0      663 2024-05-18 12:34:45.000000 swc_utils-0.1.1/src/swc_utils/wsl/wsl_compatability.py
+drwxrwxrwx   0        0        0        0 2024-05-20 13:17:58.300604 swc_utils-0.1.1/src/swc_utils.egg-info/
+-rw-rw-rw-   0        0        0      711 2024-05-20 13:17:58.000000 swc_utils-0.1.1/src/swc_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      780 2024-05-20 13:17:58.000000 swc_utils-0.1.1/src/swc_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 13:17:58.000000 swc_utils-0.1.1/src/swc_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-05-20 13:17:58.000000 swc_utils-0.1.1/src/swc_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-20 13:17:58.000000 swc_utils-0.1.1/src/swc_utils.egg-info/top_level.txt
```

### Comparing `swc_utils-0.0.2/LICENSE` & `swc_utils-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `swc_utils-0.0.2/PKG-INFO` & `swc_utils-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swc_utils
-Version: 0.0.2
+Version: 0.1.1
 Summary: Provides utility functions for SWC projects
 Author-email: Davis_Software <davissoftware6@gmail.com>
 Project-URL: Homepage, https://gitlab.software-city.org/root/swc_utils
 Project-URL: Issues, https://gitlab.software-city.org/root/swc_utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `swc_utils-0.0.2/pyproject.toml` & `swc_utils-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "swc_utils"
-version = "0.0.2"
+version = "0.1.1"
 authors = [
   { name="Davis_Software", email="davissoftware6@gmail.com" },
 ]
 description = "Provides utility functions for SWC projects"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `swc_utils-0.0.2/src/swc_utils/database/connection_profile.py` & `swc_utils-0.1.1/src/swc_utils/database/connection_profile.py`

 * *Files identical despite different names*

### Comparing `swc_utils-0.0.2/src/swc_utils/other/generator_utils.py` & `swc_utils-0.1.1/src/swc_utils/other/generator_utils.py`

 * *Files identical despite different names*

### Comparing `swc_utils-0.0.2/src/swc_utils/tools/config.py` & `swc_utils-0.1.1/src/swc_utils/tools/config.py`

 * *Files identical despite different names*

### Comparing `swc_utils-0.0.2/src/swc_utils/tools/route_loader.py` & `swc_utils-0.1.1/src/swc_utils/tools/route_loader.py`

 * *Files identical despite different names*

### Comparing `swc_utils-0.0.2/src/swc_utils/web/adv_responses.py` & `swc_utils-0.1.1/src/swc_utils/web/adv_responses.py`

 * *Files identical despite different names*

### Comparing `swc_utils-0.0.2/src/swc_utils/web/auth_manager.py` & `swc_utils-0.1.1/src/swc_utils/web/auth_manager.py`

 * *Files identical despite different names*

### Comparing `swc_utils-0.0.2/src/swc_utils/web/request_codes.py` & `swc_utils-0.1.1/src/swc_utils/web/request_codes.py`

 * *Files identical despite different names*

### Comparing `swc_utils-0.0.2/src/swc_utils/wsl/wsl_compatability.py` & `swc_utils-0.1.1/src/swc_utils/wsl/wsl_compatability.py`

 * *Files identical despite different names*

### Comparing `swc_utils-0.0.2/src/swc_utils.egg-info/PKG-INFO` & `swc_utils-0.1.1/src/swc_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swc_utils
-Version: 0.0.2
+Version: 0.1.1
 Summary: Provides utility functions for SWC projects
 Author-email: Davis_Software <davissoftware6@gmail.com>
 Project-URL: Homepage, https://gitlab.software-city.org/root/swc_utils
 Project-URL: Issues, https://gitlab.software-city.org/root/swc_utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `swc_utils-0.0.2/src/swc_utils.egg-info/SOURCES.txt` & `swc_utils-0.1.1/src/swc_utils.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 src/swc_utils.egg-info/SOURCES.txt
 src/swc_utils.egg-info/dependency_links.txt
 src/swc_utils.egg-info/requires.txt
 src/swc_utils.egg-info/top_level.txt
 src/swc_utils/database/__init__.py
 src/swc_utils/database/connection_profile.py
 src/swc_utils/database/database_connection.py
+src/swc_utils/database/db_table_care.py
 src/swc_utils/other/__init__.py
 src/swc_utils/other/generator_utils.py
 src/swc_utils/tools/__init__.py
 src/swc_utils/tools/config.py
 src/swc_utils/tools/route_loader.py
 src/swc_utils/web/__init__.py
 src/swc_utils/web/adv_responses.py
```

