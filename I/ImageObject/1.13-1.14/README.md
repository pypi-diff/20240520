# Comparing `tmp/ImageObject-1.13.tar.gz` & `tmp/ImageObject-1.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ImageObject-1.13.tar", last modified: Mon May 20 19:14:03 2024, max compression
+gzip compressed data, was "ImageObject-1.14.tar", last modified: Mon May 20 19:16:06 2024, max compression
```

## Comparing `ImageObject-1.13.tar` & `ImageObject-1.14.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 19:14:03.592193 ImageObject-1.13/
--rw-rw-rw-   0        0        0    18213 2024-05-20 19:14:01.000000 ImageObject-1.13/ImageObject.cpp
-drwxrwxrwx   0        0        0        0 2024-05-20 19:14:03.592193 ImageObject-1.13/ImageObject.egg-info/
--rw-rw-rw-   0        0        0      324 2024-05-20 19:14:03.000000 ImageObject-1.13/ImageObject.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2024-05-20 19:14:03.000000 ImageObject-1.13/ImageObject.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 19:14:03.000000 ImageObject-1.13/ImageObject.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-20 19:14:03.000000 ImageObject-1.13/ImageObject.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3770 2024-05-20 17:33:33.000000 ImageObject-1.13/ImageObject.h
--rw-rw-rw-   0        0        0     4922 2024-05-20 17:33:33.000000 ImageObject-1.13/ImageObject_old.h
--rw-rw-rw-   0        0        0       15 2024-05-20 19:12:51.000000 ImageObject-1.13/MANIFEST.in
--rw-rw-rw-   0        0        0      324 2024-05-20 19:14:03.592193 ImageObject-1.13/PKG-INFO
--rw-rw-rw-   0        0        0     3922 2024-05-20 19:13:53.000000 ImageObject-1.13/pybind11.cpp
--rw-rw-rw-   0        0        0       42 2024-05-20 19:14:03.592193 ImageObject-1.13/setup.cfg
--rw-rw-rw-   0        0        0      935 2024-05-20 19:10:20.000000 ImageObject-1.13/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 19:16:06.422782 ImageObject-1.14/
+-rw-rw-rw-   0        0        0    18213 2024-05-20 19:14:01.000000 ImageObject-1.14/ImageObject.cpp
+drwxrwxrwx   0        0        0        0 2024-05-20 19:16:06.422782 ImageObject-1.14/ImageObject.egg-info/
+-rw-rw-rw-   0        0        0      324 2024-05-20 19:16:06.000000 ImageObject-1.14/ImageObject.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2024-05-20 19:16:06.000000 ImageObject-1.14/ImageObject.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 19:16:06.000000 ImageObject-1.14/ImageObject.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-20 19:16:06.000000 ImageObject-1.14/ImageObject.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3770 2024-05-20 17:33:33.000000 ImageObject-1.14/ImageObject.h
+-rw-rw-rw-   0        0        0     4922 2024-05-20 17:33:33.000000 ImageObject-1.14/ImageObject_old.h
+-rw-rw-rw-   0        0        0       15 2024-05-20 19:12:51.000000 ImageObject-1.14/MANIFEST.in
+-rw-rw-rw-   0        0        0      324 2024-05-20 19:16:06.422782 ImageObject-1.14/PKG-INFO
+-rw-rw-rw-   0        0        0     3921 2024-05-20 19:15:47.000000 ImageObject-1.14/pybind11.cpp
+-rw-rw-rw-   0        0        0       42 2024-05-20 19:16:06.422782 ImageObject-1.14/setup.cfg
+-rw-rw-rw-   0        0        0      935 2024-05-20 19:16:05.000000 ImageObject-1.14/setup.py
```

### Comparing `ImageObject-1.13/ImageObject.cpp` & `ImageObject-1.14/ImageObject.cpp`

 * *Files identical despite different names*

### Comparing `ImageObject-1.13/ImageObject.h` & `ImageObject-1.14/ImageObject.h`

 * *Files identical despite different names*

### Comparing `ImageObject-1.13/ImageObject_old.h` & `ImageObject-1.14/ImageObject_old.h`

 * *Files identical despite different names*

### Comparing `ImageObject-1.13/pybind11.cpp` & `ImageObject-1.14/pybind11.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 #include <pybind11/pybind11.h>
 #include <pybind11/stl.h>
 #include <Python.h>
 
 #include <pybind11/numpy.h>
 #include <iostream>
-#include "ImageObjects.h"
+#include "ImageObject.h"
 
 using namespace std;
 
 namespace py = pybind11;
 
 template <typename T>
 vector< vector<short> > createShort2DArrayFromNumpy(py::array_t<T> input_array)
```

### Comparing `ImageObject-1.13/setup.py` & `ImageObject-1.14/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     ],
     language='c++',
     extra_compile_args=cpp_args)
 
 
 setup(
     name='ImageObject',
-    version='1.13',
+    version='1.14',
     description='Python package for image object operations',
     ext_modules=[sfc_module],
     author='Lei Wang',
     author_email='leiwang@lsu.edu',
     packages=find_packages(),
     headers=['includes/ImageObject.h'],
     classifiers=[
```

