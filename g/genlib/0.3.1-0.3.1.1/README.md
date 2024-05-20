# Comparing `tmp/genlib-0.3.1.tar.gz` & `tmp/genlib-0.3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genlib-0.3.1.tar", last modified: Tue Apr  2 08:04:54 2024, max compression
+gzip compressed data, was "genlib-0.3.1.1.tar", last modified: Mon May 20 07:27:13 2024, max compression
```

## Comparing `genlib-0.3.1.tar` & `genlib-0.3.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 08:04:54.633262 genlib-0.3.1/
--rw-rw-rw-   0        0        0     1088 2024-01-30 04:45:17.000000 genlib-0.3.1/LICENSE
--rw-rw-rw-   0        0        0     6127 2024-04-02 08:04:54.631260 genlib-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     5669 2024-04-02 07:40:52.000000 genlib-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 08:04:54.604722 genlib-0.3.1/genlib/
--rw-rw-rw-   0        0        0       21 2024-04-02 08:04:41.000000 genlib-0.3.1/genlib/__init__.py
--rw-rw-rw-   0        0        0     1876 2024-02-06 01:28:54.000000 genlib-0.3.1/genlib/ansiec.py
--rw-rw-rw-   0        0        0     1961 2024-01-31 03:40:22.000000 genlib-0.3.1/genlib/slip.py
--rw-rw-rw-   0        0        0    10280 2024-03-14 23:41:14.000000 genlib-0.3.1/genlib/udp.py
-drwxrwxrwx   0        0        0        0 2024-04-02 08:04:54.630258 genlib-0.3.1/genlib.egg-info/
--rw-rw-rw-   0        0        0     6127 2024-04-02 08:04:54.000000 genlib-0.3.1/genlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2024-04-02 08:04:54.000000 genlib-0.3.1/genlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 08:04:54.000000 genlib-0.3.1/genlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-02 08:04:54.000000 genlib-0.3.1/genlib.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2024-04-02 08:04:54.000000 genlib-0.3.1/genlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 08:04:54.633262 genlib-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      800 2024-04-02 08:04:16.000000 genlib-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:27:13.050958 genlib-0.3.1.1/
+-rw-rw-rw-   0        0        0     1088 2024-01-30 04:45:17.000000 genlib-0.3.1.1/LICENSE
+-rw-rw-rw-   0        0        0     6128 2024-05-20 07:27:13.049958 genlib-0.3.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5669 2024-04-02 07:40:52.000000 genlib-0.3.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 07:27:13.020961 genlib-0.3.1.1/genlib/
+-rw-rw-rw-   0        0        0       21 2024-04-02 08:04:41.000000 genlib-0.3.1.1/genlib/__init__.py
+-rw-rw-rw-   0        0        0     1876 2024-02-06 01:28:54.000000 genlib-0.3.1.1/genlib/ansiec.py
+-rw-rw-rw-   0        0        0     1961 2024-01-31 03:40:22.000000 genlib-0.3.1.1/genlib/slip.py
+-rw-rw-rw-   0        0        0    10280 2024-03-14 23:41:14.000000 genlib-0.3.1.1/genlib/udp.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:27:13.048959 genlib-0.3.1.1/genlib.egg-info/
+-rw-rw-rw-   0        0        0     6128 2024-05-20 07:27:12.000000 genlib-0.3.1.1/genlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2024-05-20 07:27:12.000000 genlib-0.3.1.1/genlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 07:27:12.000000 genlib-0.3.1.1/genlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-20 07:27:12.000000 genlib-0.3.1.1/genlib.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2024-05-20 07:27:12.000000 genlib-0.3.1.1/genlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 07:27:13.050958 genlib-0.3.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      801 2024-05-20 07:26:39.000000 genlib-0.3.1.1/setup.py
```

### Comparing `genlib-0.3.1/LICENSE` & `genlib-0.3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `genlib-0.3.1/PKG-INFO` & `genlib-0.3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: genlib
-Version: 0.3.1
+Version: 0.3.1.1
 Summary: This is the basic library for xkit.
 Home-page: https://github.com/planxstudio/xkit
 Author: chanmin.park
 Author-email: devcamp@gmail.com
 Keywords: xkit
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This is the basic library for xkit.
 
 ### History
 - V0.3.0
```

### Comparing `genlib-0.3.1/README.md` & `genlib-0.3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `genlib-0.3.1/genlib/ansiec.py` & `genlib-0.3.1.1/genlib/ansiec.py`

 * *Files identical despite different names*

### Comparing `genlib-0.3.1/genlib/slip.py` & `genlib-0.3.1.1/genlib/slip.py`

 * *Files identical despite different names*

### Comparing `genlib-0.3.1/genlib/udp.py` & `genlib-0.3.1.1/genlib/udp.py`

 * *Files identical despite different names*

### Comparing `genlib-0.3.1/genlib.egg-info/PKG-INFO` & `genlib-0.3.1.1/genlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: genlib
-Version: 0.3.1
+Version: 0.3.1.1
 Summary: This is the basic library for xkit.
 Home-page: https://github.com/planxstudio/xkit
 Author: chanmin.park
 Author-email: devcamp@gmail.com
 Keywords: xkit
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This is the basic library for xkit.
 
 ### History
 - V0.3.0
```

### Comparing `genlib-0.3.1/setup.py` & `genlib-0.3.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
     
 setup(
     name='genlib',
-    version='0.3.1',
+    version='0.3.1.1',
     description='This is the basic library for xkit.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='chanmin.park',
     author_email='devcamp@gmail.com',
     url='https://github.com/planxstudio/xkit',
     install_requires=[],
     packages=find_packages(exclude=[]),    
     keywords=['xkit'],
-    python_requires='>=3.11',
+    python_requires='>=3.8',
     package_data={}, 
     zip_safe=False,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

