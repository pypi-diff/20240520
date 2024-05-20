# Comparing `tmp/restutil-1.0.7.tar.gz` & `tmp/restutil-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\agonzalez\Desktop\adonis\workspace\rest_util\dist\.tmp-q8yei22y\restutil-1.0.7.tar", last modified: Tue Jan 17 23:51:27 2023, max compression
+gzip compressed data, was "restutil-1.0.9.tar", last modified: Wed Mar  8 12:53:48 2023, max compression
```

## Comparing `restutil-1.0.7.tar` & `restutil-1.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-01-17 23:51:27.000000 restutil-1.0.7/
--rw-rw-rw-   0        0        0    11525 2022-12-07 01:13:20.000000 restutil-1.0.7/LICENSE
--rw-rw-rw-   0        0        0     1392 2023-01-17 23:51:27.000000 restutil-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      786 2023-01-17 23:47:17.000000 restutil-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-01-17 23:51:27.000000 restutil-1.0.7/restutil/
--rw-rw-rw-   0        0        0       87 2023-01-17 23:29:10.000000 restutil-1.0.7/restutil/__init__.py
--rw-rw-rw-   0        0        0     1538 2022-12-22 14:49:31.000000 restutil-1.0.7/restutil/decorators.py
--rw-rw-rw-   0        0        0     1279 2022-12-14 13:15:38.000000 restutil-1.0.7/restutil/dictionary.py
--rw-rw-rw-   0        0        0     1993 2023-01-17 23:33:09.000000 restutil-1.0.7/restutil/encoder.py
--rw-rw-rw-   0        0        0      531 2022-12-14 13:50:35.000000 restutil-1.0.7/restutil/operations.py
--rw-rw-rw-   0        0        0     1478 2022-12-26 19:53:07.000000 restutil-1.0.7/restutil/result.py
-drwxrwxrwx   0        0        0        0 2023-01-17 23:51:27.000000 restutil-1.0.7/restutil.egg-info/
--rw-rw-rw-   0        0        0     1392 2023-01-17 23:51:27.000000 restutil-1.0.7/restutil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-01-17 23:51:27.000000 restutil-1.0.7/restutil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-17 23:51:27.000000 restutil-1.0.7/restutil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-01-17 23:51:27.000000 restutil-1.0.7/restutil.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-17 23:51:27.000000 restutil-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1007 2023-01-17 23:34:00.000000 restutil-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-08 12:53:48.753734 restutil-1.0.9/
+-rw-rw-rw-   0        0        0    11525 2022-12-07 01:13:20.000000 restutil-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1297 2023-03-08 12:53:48.752734 restutil-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      791 2023-01-17 23:55:21.000000 restutil-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-03-08 12:53:48.747735 restutil-1.0.9/restutil/
+-rw-rw-rw-   0        0        0       87 2023-01-17 23:29:10.000000 restutil-1.0.9/restutil/__init__.py
+-rw-rw-rw-   0        0        0     1538 2022-12-22 14:49:31.000000 restutil-1.0.9/restutil/decorators.py
+-rw-rw-rw-   0        0        0     1279 2022-12-14 13:15:38.000000 restutil-1.0.9/restutil/dictionary.py
+-rw-rw-rw-   0        0        0     2077 2023-03-08 12:47:28.000000 restutil-1.0.9/restutil/encoder.py
+-rw-rw-rw-   0        0        0      531 2022-12-14 13:50:35.000000 restutil-1.0.9/restutil/operations.py
+-rw-rw-rw-   0        0        0     1478 2022-12-26 19:53:07.000000 restutil-1.0.9/restutil/result.py
+drwxrwxrwx   0        0        0        0 2023-03-08 12:53:48.752734 restutil-1.0.9/restutil.egg-info/
+-rw-rw-rw-   0        0        0     1297 2023-03-08 12:53:48.000000 restutil-1.0.9/restutil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-03-08 12:53:48.000000 restutil-1.0.9/restutil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-08 12:53:48.000000 restutil-1.0.9/restutil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-03-08 12:53:48.000000 restutil-1.0.9/restutil.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-03-08 12:53:48.753734 restutil-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      909 2023-03-08 12:47:43.000000 restutil-1.0.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `restutil-1.0.7/LICENSE` & `restutil-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `restutil-1.0.7/PKG-INFO` & `restutil-1.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 Metadata-Version: 2.1
 Name: restutil
-Version: 1.0.7
+Version: 1.0.9
 Summary: Rest Util Tools
 Home-page: https://github.com/adions025/restutil
 Download-URL: https://github.com/adions025/restutil
 Author: Adonis Gonzalez Godoy
 Author-email: adions025@gmail.com
 Keywords: Restful,Rest,Util,Tools
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Rest tool
-> > A curated list of awesome things related to microservices and computer vision.
+> A curated list of awesome things related to microservices and computer vision.
 
 This module contains interesting features for endpoint creation. It also includes some decorators.
 
 ## Details
 
-- Decorest [Decorator that allows implementing a general try_log function in the entire function, but it is necessary to use the ResData data model.]
+- Decorest - class decorator that allows implementing a general try_log function in the entire function, but it is necessary to use the ResData data model
 
 ## Installation
 
 Use the package manager pip to install restutil.
 
 ```bash
 pip install restutil
@@ -37,14 +35,15 @@
 ```python
 from restutil.decorators import Decorest
 
 # create deco object
 deco = Decorest()
 
 # wrap foo function
+
 @deco.try_log
 def foo():
     return None
 ```
 
 ## Author
```

### Comparing `restutil-1.0.7/README.md` & `restutil-1.0.9/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Rest tool
-> > A curated list of awesome things related to microservices and computer vision.
+> A curated list of awesome things related to microservices and computer vision.
 
 This module contains interesting features for endpoint creation. It also includes some decorators.
 
 ## Details
 
-- Decorest [Decorator that allows implementing a general try_log function in the entire function, but it is necessary to use the ResData data model.]
+- Decorest - class decorator that allows implementing a general try_log function in the entire function, but it is necessary to use the ResData data model
 
 ## Installation
 
 Use the package manager pip to install restutil.
 
 ```bash
 pip install restutil
@@ -20,14 +20,15 @@
 ```python
 from restutil.decorators import Decorest
 
 # create deco object
 deco = Decorest()
 
 # wrap foo function
+
 @deco.try_log
 def foo():
     return None
 ```
 
 ## Author
```

### Comparing `restutil-1.0.7/restutil/decorators.py` & `restutil-1.0.9/restutil/decorators.py`

 * *Files identical despite different names*

### Comparing `restutil-1.0.7/restutil/dictionary.py` & `restutil-1.0.9/restutil/dictionary.py`

 * *Files identical despite different names*

### Comparing `restutil-1.0.7/restutil/encoder.py` & `restutil-1.0.9/restutil/encoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,19 +8,21 @@
 from multiprocessing import Pool, cpu_count
 
 
 class Encoder(JSONEncoder):
     def default(self, obj):
         if hasattr(obj, 'to_json'):
             return obj.to_json()
-        if hasattr(obj, '__dict__'):
+        elif hasattr(obj, '__dict__'):
             return {key: val for key, val in getmembers(obj)
                     if not any((key.startswith('_'), callable(val), key == 'metadata'))}
-        if hasattr(obj, 'isoformat'):
+        elif hasattr(obj, 'isoformat'):
             return f"{obj.isoformat(timespec='milliseconds')}Z"
+        elif type(obj).__name__ == 'ndarray':
+            return obj.tolist()
         return super(Encoder, self).default(obj)
 
 
 def jsonize(data, rel=False):
     result = []
     data = tuple(data) if isinstance(data, list) else (data,)
     for entity in data:
```

### Comparing `restutil-1.0.7/restutil/operations.py` & `restutil-1.0.9/restutil/operations.py`

 * *Files identical despite different names*

### Comparing `restutil-1.0.7/restutil/result.py` & `restutil-1.0.9/restutil/result.py`

 * *Files identical despite different names*

### Comparing `restutil-1.0.7/restutil.egg-info/PKG-INFO` & `restutil-1.0.9/restutil.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 Metadata-Version: 2.1
 Name: restutil
-Version: 1.0.7
+Version: 1.0.9
 Summary: Rest Util Tools
 Home-page: https://github.com/adions025/restutil
 Download-URL: https://github.com/adions025/restutil
 Author: Adonis Gonzalez Godoy
 Author-email: adions025@gmail.com
 Keywords: Restful,Rest,Util,Tools
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Rest tool
-> > A curated list of awesome things related to microservices and computer vision.
+> A curated list of awesome things related to microservices and computer vision.
 
 This module contains interesting features for endpoint creation. It also includes some decorators.
 
 ## Details
 
-- Decorest [Decorator that allows implementing a general try_log function in the entire function, but it is necessary to use the ResData data model.]
+- Decorest - class decorator that allows implementing a general try_log function in the entire function, but it is necessary to use the ResData data model
 
 ## Installation
 
 Use the package manager pip to install restutil.
 
 ```bash
 pip install restutil
@@ -37,14 +35,15 @@
 ```python
 from restutil.decorators import Decorest
 
 # create deco object
 deco = Decorest()
 
 # wrap foo function
+
 @deco.try_log
 def foo():
     return None
 ```
 
 ## Author
```

### Comparing `restutil-1.0.7/setup.py` & `restutil-1.0.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,24 +10,22 @@
 
 root_dir = Path(__file__).parent
 long_description = (root_dir / "README.md").read_text()
 
 setup(
     name='restutil',
     packages=['restutil'],
-    version='1.0.7',
+    version='1.0.9',
     description='Rest Util Tools',
     author='Adonis Gonzalez Godoy',
     author_email='adions025@gmail.com',
     url='https://github.com/adions025/restutil',
     download_url='https://github.com/adions025/restutil',
     keywords=['Restful', 'Rest', 'Util', 'Tools'],
     classifiers=[
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
     ],
     long_description=long_description,
     long_description_content_type='text/markdown'
 )
```

