# Comparing `tmp/svsa-0.0.6.tar.gz` & `tmp/svsa-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/svsa-0.0.6.tar", last modified: Wed Aug 28 20:59:14 2019, max compression
+gzip compressed data, was "svsa-0.0.8.tar", last modified: Mon May 20 16:11:48 2024, max compression
```

## Comparing `svsa-0.0.6.tar` & `svsa-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2019-08-28 20:59:14.000000 svsa-0.0.6/
--rw-r--r--   0 greg      (1000) greg      (1000)      484 2019-08-28 20:51:21.000000 svsa-0.0.6/README.md
--rw-r--r--   0 greg      (1000) greg      (1000)     1054 2019-08-28 20:59:14.000000 svsa-0.0.6/PKG-INFO
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2019-08-28 20:59:14.000000 svsa-0.0.6/svsa/
--rwxr-xr-x   0 greg      (1000) greg      (1000)     3222 2019-05-22 01:50:25.000000 svsa-0.0.6/svsa/crbs6.py
--rwxr-xr-x   0 greg      (1000) greg      (1000)     3770 2019-06-10 20:42:03.000000 svsa-0.0.6/svsa/crbs7.py
--rw-r--r--   0 greg      (1000) greg      (1000)     1033 2019-06-10 20:14:05.000000 svsa-0.0.6/svsa/gen_spectra.py
--rw-r--r--   0 greg      (1000) greg      (1000)     3329 2019-08-28 20:19:19.000000 svsa-0.0.6/svsa/support_vector_spectrum.py
--rw-r--r--   0 greg      (1000) greg      (1000)      146 2019-06-10 20:14:22.000000 svsa-0.0.6/svsa/__init__.py
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2019-08-28 20:59:14.000000 svsa-0.0.6/svsa.egg-info/
--rw-r--r--   0 greg      (1000) greg      (1000)     1054 2019-08-28 20:59:14.000000 svsa-0.0.6/svsa.egg-info/PKG-INFO
--rw-r--r--   0 greg      (1000) greg      (1000)       27 2019-08-28 20:59:14.000000 svsa-0.0.6/svsa.egg-info/requires.txt
--rw-r--r--   0 greg      (1000) greg      (1000)      277 2019-08-28 20:59:14.000000 svsa-0.0.6/svsa.egg-info/SOURCES.txt
--rw-r--r--   0 greg      (1000) greg      (1000)        1 2019-08-28 20:59:14.000000 svsa-0.0.6/svsa.egg-info/dependency_links.txt
--rw-r--r--   0 greg      (1000) greg      (1000)        5 2019-08-28 20:59:14.000000 svsa-0.0.6/svsa.egg-info/top_level.txt
--rw-r--r--   0 greg      (1000) greg      (1000)        1 2019-08-28 19:38:50.000000 svsa-0.0.6/svsa.egg-info/zip-safe
--rw-r--r--   0 greg      (1000) greg      (1000)       38 2019-08-28 20:59:14.000000 svsa-0.0.6/setup.cfg
--rw-r--r--   0 greg      (1000) greg      (1000)      878 2019-08-28 20:27:33.000000 svsa-0.0.6/setup.py
+drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2024-05-20 16:11:48.888291 svsa-0.0.8/
+-rw-rw-r--   0 greg      (1000) greg      (1000)     1633 2024-05-20 16:11:48.888291 svsa-0.0.8/PKG-INFO
+-rw-rw-r--   0 greg      (1000) greg      (1000)      951 2024-05-20 16:04:49.000000 svsa-0.0.8/README.md
+-rw-rw-r--   0 greg      (1000) greg      (1000)       38 2024-05-20 16:11:48.888291 svsa-0.0.8/setup.cfg
+-rw-r--r--   0 greg      (1000) greg      (1000)      883 2024-05-20 16:08:15.000000 svsa-0.0.8/setup.py
+drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2024-05-20 16:11:48.888291 svsa-0.0.8/svsa/
+-rw-rw-r--   0 greg      (1000) greg      (1000)      146 2024-05-20 16:04:49.000000 svsa-0.0.8/svsa/__init__.py
+-rwxrwxr-x   0 greg      (1000) greg      (1000)     3222 2024-05-20 16:04:49.000000 svsa-0.0.8/svsa/crbs6.py
+-rwxrwxr-x   0 greg      (1000) greg      (1000)     3770 2024-05-20 16:04:49.000000 svsa-0.0.8/svsa/crbs7.py
+-rw-rw-r--   0 greg      (1000) greg      (1000)     1033 2024-05-20 16:04:49.000000 svsa-0.0.8/svsa/gen_spectra.py
+-rw-rw-r--   0 greg      (1000) greg      (1000)     3329 2024-05-20 16:04:49.000000 svsa-0.0.8/svsa/support_vector_spectrum.py
+drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2024-05-20 16:11:48.888291 svsa-0.0.8/svsa.egg-info/
+-rw-rw-r--   0 greg      (1000) greg      (1000)     1633 2024-05-20 16:11:48.000000 svsa-0.0.8/svsa.egg-info/PKG-INFO
+-rw-rw-r--   0 greg      (1000) greg      (1000)      277 2024-05-20 16:11:48.000000 svsa-0.0.8/svsa.egg-info/SOURCES.txt
+-rw-rw-r--   0 greg      (1000) greg      (1000)        1 2024-05-20 16:11:48.000000 svsa-0.0.8/svsa.egg-info/dependency_links.txt
+-rw-rw-r--   0 greg      (1000) greg      (1000)       32 2024-05-20 16:11:48.000000 svsa-0.0.8/svsa.egg-info/requires.txt
+-rw-rw-r--   0 greg      (1000) greg      (1000)        5 2024-05-20 16:11:48.000000 svsa-0.0.8/svsa.egg-info/top_level.txt
+-rw-rw-r--   0 greg      (1000) greg      (1000)        1 2024-05-20 16:11:48.000000 svsa-0.0.8/svsa.egg-info/zip-safe
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `svsa-0.0.6/svsa/crbs6.py` & `svsa-0.0.8/svsa/crbs6.py`

 * *Files identical despite different names*

### Comparing `svsa-0.0.6/svsa/crbs7.py` & `svsa-0.0.8/svsa/crbs7.py`

 * *Files identical despite different names*

### Comparing `svsa-0.0.6/svsa/gen_spectra.py` & `svsa-0.0.8/svsa/gen_spectra.py`

 * *Files identical despite different names*

### Comparing `svsa-0.0.6/svsa/support_vector_spectrum.py` & `svsa-0.0.8/svsa/support_vector_spectrum.py`

 * *Files identical despite different names*

### Comparing `svsa-0.0.6/setup.py` & `svsa-0.0.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(name='svsa',
-      version='0.0.6',
+      version='0.0.8',
       url='https://gjhunt.github.io/svsa/',
       author='Gregory J. Hunt',
       author_email='ghunt@wm.edu',
       description='Fast approximations of scattering spectra with SVR.',
       long_description=long_description,
       long_description_content_type="text/markdown",
       license='GPL3',
       packages=setuptools.find_packages(),
       install_requires=[
           'pandas',
           'numpy',
           'scipy',
-          'sklearn'
+          'scikit-learn'
           ],
       classifiers=[
           "Programming Language :: Python :: 3",
           "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
           "Operating System :: OS Independent",
           'Topic :: Scientific/Engineering',
       ],
```

