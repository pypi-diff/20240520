# Comparing `tmp/okn_py_updater-2.0.6.tar.gz` & `tmp/okn_py_updater-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "okn_py_updater-2.0.6.tar", last modified: Wed May 15 22:41:36 2024, max compression
+gzip compressed data, was "okn_py_updater-2.0.7.tar", last modified: Sun May 19 23:05:57 2024, max compression
```

## Comparing `okn_py_updater-2.0.6.tar` & `okn_py_updater-2.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 22:41:36.837449 okn_py_updater-2.0.6/
--rw-rw-rw-   0        0        0    11558 2024-05-06 22:12:10.000000 okn_py_updater-2.0.6/LICENSE
--rw-rw-rw-   0        0        0     3706 2024-05-15 22:41:36.837449 okn_py_updater-2.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3129 2024-05-06 22:12:10.000000 okn_py_updater-2.0.6/README.md
--rw-rw-rw-   0        0        0      657 2024-05-15 22:41:13.000000 okn_py_updater-2.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-15 22:41:36.837449 okn_py_updater-2.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-15 22:41:36.811091 okn_py_updater-2.0.6/src/
-drwxrwxrwx   0        0        0        0 2024-05-15 22:41:36.817475 okn_py_updater-2.0.6/src/okn_py_updater/
--rw-rw-rw-   0        0        0        0 2024-05-06 22:12:10.000000 okn_py_updater-2.0.6/src/okn_py_updater/__init__.py
--rw-rw-rw-   0        0        0    25716 2024-05-15 22:40:16.000000 okn_py_updater-2.0.6/src/okn_py_updater/okn_py_updater.py
-drwxrwxrwx   0        0        0        0 2024-05-15 22:41:36.835434 okn_py_updater-2.0.6/src/okn_py_updater.egg-info/
--rw-rw-rw-   0        0        0     3706 2024-05-15 22:41:36.000000 okn_py_updater-2.0.6/src/okn_py_updater.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2024-05-15 22:41:36.000000 okn_py_updater-2.0.6/src/okn_py_updater.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 22:41:36.000000 okn_py_updater-2.0.6/src/okn_py_updater.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-15 22:41:36.000000 okn_py_updater-2.0.6/src/okn_py_updater.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-19 23:05:57.366163 okn_py_updater-2.0.7/
+-rw-rw-rw-   0        0        0    11558 2024-05-06 22:12:10.000000 okn_py_updater-2.0.7/LICENSE
+-rw-rw-rw-   0        0        0     3706 2024-05-19 23:05:57.364168 okn_py_updater-2.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3129 2024-05-06 22:12:10.000000 okn_py_updater-2.0.7/README.md
+-rw-rw-rw-   0        0        0      657 2024-05-19 23:05:36.000000 okn_py_updater-2.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-19 23:05:57.366163 okn_py_updater-2.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-19 23:05:57.333250 okn_py_updater-2.0.7/src/
+drwxrwxrwx   0        0        0        0 2024-05-19 23:05:57.344221 okn_py_updater-2.0.7/src/okn_py_updater/
+-rw-rw-rw-   0        0        0        0 2024-05-06 22:12:10.000000 okn_py_updater-2.0.7/src/okn_py_updater/__init__.py
+-rw-rw-rw-   0        0        0    25476 2024-05-19 23:05:36.000000 okn_py_updater-2.0.7/src/okn_py_updater/okn_py_updater.py
+drwxrwxrwx   0        0        0        0 2024-05-19 23:05:57.363199 okn_py_updater-2.0.7/src/okn_py_updater.egg-info/
+-rw-rw-rw-   0        0        0     3706 2024-05-19 23:05:57.000000 okn_py_updater-2.0.7/src/okn_py_updater.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2024-05-19 23:05:57.000000 okn_py_updater-2.0.7/src/okn_py_updater.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 23:05:57.000000 okn_py_updater-2.0.7/src/okn_py_updater.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-19 23:05:57.000000 okn_py_updater-2.0.7/src/okn_py_updater.egg-info/top_level.txt
```

### Comparing `okn_py_updater-2.0.6/LICENSE` & `okn_py_updater-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `okn_py_updater-2.0.6/PKG-INFO` & `okn_py_updater-2.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okn_py_updater
-Version: 2.0.6
+Version: 2.0.7
 Summary: Python Library for OKN Data Updater
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/ZawLinTun16925410/okn_data_updater
 Project-URL: Bug Tracker, https://github.com/ZawLinTun16925410/okn_data_updater/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `okn_py_updater-2.0.6/README.md` & `okn_py_updater-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `okn_py_updater-2.0.6/pyproject.toml` & `okn_py_updater-2.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "okn_py_updater"
-version = "2.0.6"
+version = "2.0.7"
 authors = [
   { name="Zaw Lin Tun", email="zawlintun1511@gmail.com" },
 ]
 description = "Python Library for OKN Data Updater"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `okn_py_updater-2.0.6/src/okn_py_updater/okn_py_updater.py` & `okn_py_updater-2.0.7/src/okn_py_updater/okn_py_updater.py`

 * *Files 2% similar despite different names*

```diff
@@ -531,19 +531,16 @@
 
             first_data = self.circular_buffer[0]
             self.pre_x_nom = first_data["updated_x_nom"]
             self.pre_y_nom = first_data["updated_y_nom"]
             self.pre_time = first_data["record_timestamp"]
             n_data_index = int((self.n_value - 3) / 2) + 1
             n_related_data = self.circular_buffer[n_data_index]
-            first_data["x_nom"] = n_related_data["x_nom"]
-            first_data["y_nom"] = n_related_data["y_nom"]
-            first_data["record_timestamp"] = n_related_data["record_timestamp"]
-            first_data["sensor_timestamp"] = n_related_data["sensor_timestamp"]
-            first_data["direction"] = n_related_data["direction"]
+            for header in self.header_array:
+                first_data[header] = n_related_data[header]
             out_array = []
             for header in self.out_header_array:
                 out_array.append(first_data[header])
             return out_array
         else:
             if self.count == 0:
                 data_input.insert(0, self.data_id)
```

### Comparing `okn_py_updater-2.0.6/src/okn_py_updater.egg-info/PKG-INFO` & `okn_py_updater-2.0.7/src/okn_py_updater.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okn_py_updater
-Version: 2.0.6
+Version: 2.0.7
 Summary: Python Library for OKN Data Updater
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/ZawLinTun16925410/okn_data_updater
 Project-URL: Bug Tracker, https://github.com/ZawLinTun16925410/okn_data_updater/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

