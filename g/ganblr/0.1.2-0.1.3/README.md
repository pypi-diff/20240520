# Comparing `tmp/ganblr-0.1.2.tar.gz` & `tmp/ganblr-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ganblr-0.1.2.tar", last modified: Thu May  9 02:49:57 2024, max compression
+gzip compressed data, was "ganblr-0.1.3.tar", last modified: Mon May 20 08:09:28 2024, max compression
```

## Comparing `ganblr-0.1.2.tar` & `ganblr-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 02:49:57.061464 ganblr-0.1.2/
--rw-rw-rw-   0        0        0     1099 2022-11-15 11:32:18.000000 ganblr-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     4309 2024-05-09 02:49:57.060963 ganblr-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3826 2024-05-09 02:37:42.000000 ganblr-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 02:49:57.044449 ganblr-0.1.2/ganblr/
--rw-rw-rw-   0        0        0      281 2024-05-09 02:39:42.000000 ganblr-0.1.2/ganblr/__init__.py
--rw-rw-rw-   0        0        0    12681 2024-05-03 06:06:11.000000 ganblr-0.1.2/ganblr/kdb.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:49:57.059462 ganblr-0.1.2/ganblr/models/
--rw-rw-rw-   0        0        0      167 2024-05-09 02:39:42.000000 ganblr-0.1.2/ganblr/models/__init__.py
--rw-rw-rw-   0        0        0    10654 2024-05-03 06:06:11.000000 ganblr-0.1.2/ganblr/models/ganblr.py
--rw-rw-rw-   0        0        0    12100 2024-05-09 02:39:42.000000 ganblr-0.1.2/ganblr/models/ganblrmug.py
--rw-rw-rw-   0        0        0    12395 2022-12-14 17:18:53.000000 ganblr-0.1.2/ganblr/models/ganblrpp.py
--rw-rw-rw-   0        0        0     5255 2024-05-03 06:06:11.000000 ganblr-0.1.2/ganblr/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:49:57.052456 ganblr-0.1.2/ganblr.egg-info/
--rw-rw-rw-   0        0        0     4309 2024-05-09 02:49:56.000000 ganblr-0.1.2/ganblr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      327 2024-05-09 02:49:56.000000 ganblr-0.1.2/ganblr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 02:49:56.000000 ganblr-0.1.2/ganblr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-05-09 02:49:56.000000 ganblr-0.1.2/ganblr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-09 02:49:56.000000 ganblr-0.1.2/ganblr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 02:49:57.061965 ganblr-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1089 2024-05-09 02:39:42.000000 ganblr-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 08:09:28.797342 ganblr-0.1.3/
+-rw-rw-rw-   0        0        0     1099 2022-11-15 11:32:18.000000 ganblr-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     4309 2024-05-20 08:09:28.797342 ganblr-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3826 2024-05-09 02:37:42.000000 ganblr-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 08:09:28.768728 ganblr-0.1.3/ganblr/
+-rw-rw-rw-   0        0        0      320 2024-05-20 08:03:03.000000 ganblr-0.1.3/ganblr/__init__.py
+-rw-rw-rw-   0        0        0    12680 2024-05-20 07:56:42.000000 ganblr-0.1.3/ganblr/kdb.py
+drwxrwxrwx   0        0        0        0 2024-05-20 08:09:28.785347 ganblr-0.1.3/ganblr/models/
+-rw-rw-rw-   0        0        0      167 2024-05-09 02:39:42.000000 ganblr-0.1.3/ganblr/models/__init__.py
+-rw-rw-rw-   0        0        0    10654 2024-05-03 06:06:11.000000 ganblr-0.1.3/ganblr/models/ganblr.py
+-rw-rw-rw-   0        0        0    12100 2024-05-09 02:39:42.000000 ganblr-0.1.3/ganblr/models/ganblrmug.py
+-rw-rw-rw-   0        0        0    12395 2022-12-14 17:18:53.000000 ganblr-0.1.3/ganblr/models/ganblrpp.py
+drwxrwxrwx   0        0        0        0 2024-05-20 08:09:28.787333 ganblr-0.1.3/ganblr/pyitlib/
+-rw-rw-rw-   0        0        0       87 2024-05-20 07:55:46.000000 ganblr-0.1.3/ganblr/pyitlib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 08:09:28.795340 ganblr-0.1.3/ganblr/pyitlib/pyitlib/
+-rw-rw-rw-   0        0        0     1137 2024-05-20 07:46:02.000000 ganblr-0.1.3/ganblr/pyitlib/pyitlib/__init__.py
+-rw-rw-rw-   0        0        0   232279 2024-05-20 07:46:02.000000 ganblr-0.1.3/ganblr/pyitlib/pyitlib/discrete_random_variable.py
+-rw-rw-rw-   0        0        0       79 2024-05-20 07:46:02.000000 ganblr-0.1.3/ganblr/pyitlib/pyitlib/pyitlib_version.py
+-rw-rw-rw-   0        0        0     1137 2024-05-20 07:46:02.000000 ganblr-0.1.3/ganblr/pyitlib/pyitlib/util.py
+-rw-rw-rw-   0        0        0     5255 2024-05-03 06:06:11.000000 ganblr-0.1.3/ganblr/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-20 08:09:28.778325 ganblr-0.1.3/ganblr.egg-info/
+-rw-rw-rw-   0        0        0     4309 2024-05-20 08:09:28.000000 ganblr-0.1.3/ganblr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      513 2024-05-20 08:09:28.000000 ganblr-0.1.3/ganblr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 08:09:28.000000 ganblr-0.1.3/ganblr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-20 08:09:28.000000 ganblr-0.1.3/ganblr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-20 08:09:28.000000 ganblr-0.1.3/ganblr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 08:09:28.798343 ganblr-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1078 2024-05-20 08:05:47.000000 ganblr-0.1.3/setup.py
```

### Comparing `ganblr-0.1.2/LICENSE` & `ganblr-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ganblr-0.1.2/PKG-INFO` & `ganblr-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ganblr
-Version: 0.1.2
+Version: 0.1.3
 Summary: Ganblr Toolbox
 Home-page: https://github.com/tulip-lab/ganblr
 Author: kae zhou
 Author-email: kaezhou@gmail.com
 License: MIT Licence
 Keywords: ganblr,tulip
 Platform: any
```

### Comparing `ganblr-0.1.2/README.md` & `ganblr-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ganblr-0.1.2/ganblr/kdb.py` & `ganblr-0.1.3/ganblr/kdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import numpy as np
 #import networkx as nx
-from pyitlib import discrete_random_variable as drv
-
+from .pyitlib import discrete_random_variable as drv
 def build_graph(X, y, k=2):
   '''
   kDB algorithm
 
   Param:
   ----------------------
```

### Comparing `ganblr-0.1.2/ganblr/models/ganblr.py` & `ganblr-0.1.3/ganblr/models/ganblr.py`

 * *Files identical despite different names*

### Comparing `ganblr-0.1.2/ganblr/models/ganblrmug.py` & `ganblr-0.1.3/ganblr/models/ganblrmug.py`

 * *Files identical despite different names*

### Comparing `ganblr-0.1.2/ganblr/models/ganblrpp.py` & `ganblr-0.1.3/ganblr/models/ganblrpp.py`

 * *Files identical despite different names*

### Comparing `ganblr-0.1.2/ganblr/utils.py` & `ganblr-0.1.3/ganblr/utils.py`

 * *Files identical despite different names*

### Comparing `ganblr-0.1.2/ganblr.egg-info/PKG-INFO` & `ganblr-0.1.3/ganblr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ganblr
-Version: 0.1.2
+Version: 0.1.3
 Summary: Ganblr Toolbox
 Home-page: https://github.com/tulip-lab/ganblr
 Author: kae zhou
 Author-email: kaezhou@gmail.com
 License: MIT Licence
 Keywords: ganblr,tulip
 Platform: any
```

### Comparing `ganblr-0.1.2/setup.py` & `ganblr-0.1.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,29 +7,29 @@
   with open(os.path.join(path, 'README.md')) as f:
     long_description = f.read()
 except Exception as e:
   long_description = "Ganblr Toolbox"
 
 setup(
     name = "ganblr",
-    version = "0.1.2",
+    version = "0.1.3",
     keywords = ["ganblr", "tulip"],
     description = "Ganblr Toolbox",
     long_description = long_description,
     long_description_content_type='text/markdown',
     python_requires=">=3.5.0",
     license = "MIT Licence",
 
     url = "https://github.com/tulip-lab/ganblr",
     author = "kae zhou",
     author_email = "kaezhou@gmail.com",
 
     packages = find_packages(),
     include_package_data = True,
-    install_requires = ["numpy", "pandas", "tensorflow>=2.3", "scikit-learn>=0.24", "pyitlib", "pgmpy"],
+    install_requires = ["numpy", "pandas", "tensorflow>=2.3", "scikit-learn>=0.24", "pgmpy"],
     platforms = "any",
 
     scripts = [],
     entry_points = {},
 
     classifiers=[
         "Programming Language :: Python :: 3",
```

