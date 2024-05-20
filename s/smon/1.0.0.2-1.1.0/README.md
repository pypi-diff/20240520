# Comparing `tmp/smon-1.0.0.2.tar.gz` & `tmp/smon-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smon-1.0.0.2.tar", last modified: Tue Apr  2 15:32:54 2024, max compression
+gzip compressed data, was "smon-1.1.0.tar", last modified: Mon May 20 07:54:48 2024, max compression
```

## Comparing `smon-1.0.0.2.tar` & `smon-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 15:32:54.828167 smon-1.0.0.2/
--rw-rw-rw-   0        0        0     1088 2024-01-30 04:45:17.000000 smon-1.0.0.2/LICENSE
--rw-rw-rw-   0        0        0       18 2024-04-02 14:52:41.000000 smon-1.0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2134 2024-04-02 15:32:54.827169 smon-1.0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1511 2024-04-02 15:26:03.000000 smon-1.0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-02 15:32:54.828167 smon-1.0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1037 2024-04-02 15:32:44.000000 smon-1.0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-02 15:32:54.806162 smon-1.0.0.2/smon/
--rw-rw-rw-   0        0        0       21 2024-04-02 13:46:54.000000 smon-1.0.0.2/smon/__init__.py
--rw-rw-rw-   0        0        0    18955 2024-04-02 15:19:39.000000 smon-1.0.0.2/smon/oscilloscope.py
--rw-rw-rw-   0        0        0     3285 2024-04-02 15:32:22.000000 smon-1.0.0.2/smon/sampling.py
--rw-rw-rw-   0        0        0     1292 2021-01-03 05:08:18.000000 smon-1.0.0.2/smon/smon.png
--rw-rw-rw-   0        0        0     2321 2024-04-02 15:04:58.000000 smon-1.0.0.2/smon/smon.py
--rw-rw-rw-   0        0        0    32162 2024-04-02 15:20:42.000000 smon-1.0.0.2/smon/smon_xnode_code.png
-drwxrwxrwx   0        0        0        0 2024-04-02 15:32:54.827169 smon-1.0.0.2/smon.egg-info/
--rw-rw-rw-   0        0        0     2134 2024-04-02 15:32:54.000000 smon-1.0.0.2/smon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2024-04-02 15:32:54.000000 smon-1.0.0.2/smon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 15:32:54.000000 smon-1.0.0.2/smon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-04-02 15:32:54.000000 smon-1.0.0.2/smon.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-02 15:32:54.000000 smon-1.0.0.2/smon.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       51 2024-04-02 15:32:54.000000 smon-1.0.0.2/smon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-02 15:32:54.000000 smon-1.0.0.2/smon.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-20 07:54:48.419271 smon-1.1.0/
+-rw-rw-rw-   0        0        0     1088 2024-01-30 04:45:17.000000 smon-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0       18 2024-04-02 14:52:41.000000 smon-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2131 2024-05-20 07:54:48.418270 smon-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1511 2024-04-02 15:26:03.000000 smon-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-20 07:54:48.420272 smon-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1034 2024-05-20 07:54:28.000000 smon-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:54:48.377261 smon-1.1.0/smon/
+-rw-rw-rw-   0        0        0       21 2024-05-20 07:53:52.000000 smon-1.1.0/smon/__init__.py
+-rw-rw-rw-   0        0        0    18955 2024-04-02 15:19:39.000000 smon-1.1.0/smon/oscilloscope.py
+-rw-rw-rw-   0        0        0     3285 2024-04-02 15:32:22.000000 smon-1.1.0/smon/sampling.py
+-rw-rw-rw-   0        0        0     1292 2021-01-03 05:08:18.000000 smon-1.1.0/smon/smon.png
+-rw-rw-rw-   0        0        0     2321 2024-04-02 15:04:58.000000 smon-1.1.0/smon/smon.py
+-rw-rw-rw-   0        0        0    32162 2024-04-02 15:20:42.000000 smon-1.1.0/smon/smon_xnode_code.png
+drwxrwxrwx   0        0        0        0 2024-05-20 07:54:48.416269 smon-1.1.0/smon.egg-info/
+-rw-rw-rw-   0        0        0     2131 2024-05-20 07:54:48.000000 smon-1.1.0/smon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2024-05-20 07:54:48.000000 smon-1.1.0/smon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 07:54:48.000000 smon-1.1.0/smon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-05-20 07:54:48.000000 smon-1.1.0/smon.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-20 07:54:48.000000 smon-1.1.0/smon.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       51 2024-05-20 07:54:48.000000 smon-1.1.0/smon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-20 07:54:48.000000 smon-1.1.0/smon.egg-info/top_level.txt
```

### Comparing `smon-1.0.0.2/LICENSE` & `smon-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smon-1.0.0.2/PKG-INFO` & `smon-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: smon
-Version: 1.0.0.2
+Version: 1.1.0
 Summary: This is a sensor data oscilloscope for xkit.
 Home-page: https://github.com/planxstudio/xkit
 Author: chanmin.park
 Author-email: devcamp@gmail.com
 Keywords: xkit,genlib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: python-dotenv
 Requires-Dist: numpy
 Requires-Dist: pyside6
 Requires-Dist: pythonqwt
```

### Comparing `smon-1.0.0.2/README.md` & `smon-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `smon-1.0.0.2/setup.py` & `smon-1.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
     
 setup(
     name='smon',
-    version='1.0.0.2',
+    version='1.1.0',
     description='This is a sensor data oscilloscope for xkit.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='chanmin.park',
     author_email='devcamp@gmail.com',
     url='https://github.com/planxstudio/xkit',
     install_requires=['click', 'python-dotenv', 'numpy', 'pyside6', 'pythonqwt', 'genlib'],
     packages=find_packages(exclude=[]),
     keywords=['xkit', 'genlib'],
-    python_requires='>=3.11',
+    python_requires='>=3.8',
     package_data={},
     include_package_data=True,    
     zip_safe=False,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `smon-1.0.0.2/smon/oscilloscope.py` & `smon-1.1.0/smon/oscilloscope.py`

 * *Files identical despite different names*

### Comparing `smon-1.0.0.2/smon/sampling.py` & `smon-1.1.0/smon/sampling.py`

 * *Files identical despite different names*

### Comparing `smon-1.0.0.2/smon/smon.png` & `smon-1.1.0/smon/smon.png`

 * *Files identical despite different names*

### Comparing `smon-1.0.0.2/smon/smon.py` & `smon-1.1.0/smon/smon.py`

 * *Files identical despite different names*

### Comparing `smon-1.0.0.2/smon/smon_xnode_code.png` & `smon-1.1.0/smon/smon_xnode_code.png`

 * *Files identical despite different names*

### Comparing `smon-1.0.0.2/smon.egg-info/PKG-INFO` & `smon-1.1.0/smon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: smon
-Version: 1.0.0.2
+Version: 1.1.0
 Summary: This is a sensor data oscilloscope for xkit.
 Home-page: https://github.com/planxstudio/xkit
 Author: chanmin.park
 Author-email: devcamp@gmail.com
 Keywords: xkit,genlib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: python-dotenv
 Requires-Dist: numpy
 Requires-Dist: pyside6
 Requires-Dist: pythonqwt
```

