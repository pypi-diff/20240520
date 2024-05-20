# Comparing `tmp/calculate_mean-0.0.1.tar.gz` & `tmp/calculate_mean-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calculate_mean-0.0.1.tar", last modified: Mon May 20 02:55:29 2024, max compression
+gzip compressed data, was "calculate_mean-0.1.tar", last modified: Mon May 20 12:48:07 2024, max compression
```

## Comparing `calculate_mean-0.0.1.tar` & `calculate_mean-0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 02:55:29.956203 calculate_mean-0.0.1/
--rw-rw-rw-   0        0        0     1083 2024-05-18 13:06:21.000000 calculate_mean-0.0.1/LICENCE
--rw-rw-rw-   0        0        0      761 2024-05-20 02:55:29.956203 calculate_mean-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      107 2024-05-18 13:16:20.000000 calculate_mean-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 02:55:29.956203 calculate_mean-0.0.1/calculate_mean.egg-info/
--rw-rw-rw-   0        0        0      761 2024-05-20 02:55:29.000000 calculate_mean-0.0.1/calculate_mean.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2024-05-20 02:55:29.000000 calculate_mean-0.0.1/calculate_mean.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 02:55:29.000000 calculate_mean-0.0.1/calculate_mean.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-05-20 02:55:29.000000 calculate_mean-0.0.1/calculate_mean.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 02:55:29.000000 calculate_mean-0.0.1/calculate_mean.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 02:55:29.956203 calculate_mean-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1156 2024-05-18 14:01:23.000000 calculate_mean-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 12:48:07.695042 calculate_mean-0.1/
+-rw-rw-rw-   0        0        0     1083 2024-05-18 13:06:21.000000 calculate_mean-0.1/LICENCE
+-rw-rw-rw-   0        0        0      829 2024-05-20 12:48:07.693041 calculate_mean-0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      153 2024-05-20 12:44:21.000000 calculate_mean-0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 12:48:07.691039 calculate_mean-0.1/calculate_mean.egg-info/
+-rw-rw-rw-   0        0        0      829 2024-05-20 12:48:07.000000 calculate_mean-0.1/calculate_mean.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2024-05-20 12:48:07.000000 calculate_mean-0.1/calculate_mean.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 12:48:07.000000 calculate_mean-0.1/calculate_mean.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-05-20 12:48:07.000000 calculate_mean-0.1/calculate_mean.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 12:48:07.000000 calculate_mean-0.1/calculate_mean.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 12:48:07.695435 calculate_mean-0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1162 2024-05-20 12:45:24.000000 calculate_mean-0.1/setup.py
```

### Comparing `calculate_mean-0.0.1/LICENCE` & `calculate_mean-0.1/LICENCE`

 * *Files identical despite different names*

### Comparing `calculate_mean-0.0.1/PKG-INFO` & `calculate_mean-0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: calculate_mean
-Version: 0.0.1
+Version: 0.1
 Summary: Calculates the Mean of given Values
 Author: kunaalg
 Author-email: <kunaal@runcode.com>
 Keywords: python,mean,calculate,calculate mean,numbers,math
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENCE
-Requires-Dist: opencv-python
+Requires-Dist: virtualenv
 Requires-Dist: datetime
 Requires-Dist: numpy
+Requires-Dist: requests
 
 
 You can use this function like this:
 
 Python
 
+from calculate_mean import calculate_mean 
+
 values = [1, 2, 3, 4, 5]
 
 print(calculate_mean(values))
```

### Comparing `calculate_mean-0.0.1/calculate_mean.egg-info/PKG-INFO` & `calculate_mean-0.1/calculate_mean.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: calculate_mean
-Version: 0.0.1
+Version: 0.1
 Summary: Calculates the Mean of given Values
 Author: kunaalg
 Author-email: <kunaal@runcode.com>
 Keywords: python,mean,calculate,calculate mean,numbers,math
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENCE
-Requires-Dist: opencv-python
+Requires-Dist: virtualenv
 Requires-Dist: datetime
 Requires-Dist: numpy
+Requires-Dist: requests
 
 
 You can use this function like this:
 
 Python
 
+from calculate_mean import calculate_mean 
+
 values = [1, 2, 3, 4, 5]
 
 print(calculate_mean(values))
```

### Comparing `calculate_mean-0.0.1/setup.py` & `calculate_mean-0.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.1'
 DESCRIPTION = 'Calculates the Mean of given Values'
 LONG_DESCRIPTION = 'A package that defines a function to calculate the mean of n number of values'
 
 # Setting up
 setup(
     name="calculate_mean",
     version=VERSION,
     author="kunaalg",
     author_email="<kunaal@runcode.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=['opencv-python', 'datetime', 'numpy'],
+    install_requires=['virtualenv', 'datetime', 'numpy','requests'],
     keywords=['python', 'mean', 'calculate', 'calculate mean', 'numbers', 'math'],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

