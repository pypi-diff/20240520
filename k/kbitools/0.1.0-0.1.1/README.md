# Comparing `tmp/kbitools-0.1.0.tar.gz` & `tmp/kbitools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kbitools-0.1.0.tar", last modified: Sun May 19 21:07:36 2024, max compression
+gzip compressed data, was "kbitools-0.1.1.tar", last modified: Sun May 19 21:26:59 2024, max compression
```

## Comparing `kbitools-0.1.0.tar` & `kbitools-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 cam       (1000) cam       (1000)        0 2024-05-19 21:07:36.538305 kbitools-0.1.0/
--rw-r--r--   0 cam       (1000) cam       (1000)      342 2024-05-19 21:07:36.538305 kbitools-0.1.0/PKG-INFO
-drwxr-xr-x   0 cam       (1000) cam       (1000)        0 2024-05-19 21:07:36.538305 kbitools-0.1.0/kbitools/
--rw-r--r--   0 cam       (1000) cam       (1000)       70 2024-04-29 19:27:42.000000 kbitools-0.1.0/kbitools/__init__.py
--rw-r--r--   0 cam       (1000) cam       (1000)     1331 2024-05-19 21:06:54.000000 kbitools-0.1.0/kbitools/flags.py
--rw-r--r--   0 cam       (1000) cam       (1000)     3951 2024-05-02 16:52:55.000000 kbitools-0.1.0/kbitools/kbi_logger.py
--rw-r--r--   0 cam       (1000) cam       (1000)     8748 2024-05-16 22:16:56.000000 kbitools-0.1.0/kbitools/klient.py
-drwxr-xr-x   0 cam       (1000) cam       (1000)        0 2024-05-19 21:07:36.538305 kbitools-0.1.0/kbitools.egg-info/
--rw-r--r--   0 cam       (1000) cam       (1000)      342 2024-05-19 21:07:36.000000 kbitools-0.1.0/kbitools.egg-info/PKG-INFO
--rw-r--r--   0 cam       (1000) cam       (1000)      283 2024-05-19 21:07:36.000000 kbitools-0.1.0/kbitools.egg-info/SOURCES.txt
--rw-r--r--   0 cam       (1000) cam       (1000)        1 2024-05-19 21:07:36.000000 kbitools-0.1.0/kbitools.egg-info/dependency_links.txt
--rw-r--r--   0 cam       (1000) cam       (1000)       48 2024-05-19 21:07:36.000000 kbitools-0.1.0/kbitools.egg-info/entry_points.txt
--rw-r--r--   0 cam       (1000) cam       (1000)       16 2024-05-19 21:07:36.000000 kbitools-0.1.0/kbitools.egg-info/requires.txt
--rw-r--r--   0 cam       (1000) cam       (1000)        9 2024-05-19 21:07:36.000000 kbitools-0.1.0/kbitools.egg-info/top_level.txt
--rw-r--r--   0 cam       (1000) cam       (1000)       38 2024-05-19 21:07:36.538305 kbitools-0.1.0/setup.cfg
--rw-r--r--   0 cam       (1000) cam       (1000)      615 2024-05-19 21:04:59.000000 kbitools-0.1.0/setup.py
+drwxr-xr-x   0 cam       (1000) cam       (1000)        0 2024-05-19 21:26:59.723056 kbitools-0.1.1/
+-rw-r--r--   0 cam       (1000) cam       (1000)      374 2024-05-19 21:26:59.723056 kbitools-0.1.1/PKG-INFO
+-rw-r--r--   0 cam       (1000) cam       (1000)     1460 2024-05-19 21:20:53.000000 kbitools-0.1.1/README.md
+drwxr-xr-x   0 cam       (1000) cam       (1000)        0 2024-05-19 21:26:59.723056 kbitools-0.1.1/kbitools/
+-rw-r--r--   0 cam       (1000) cam       (1000)       70 2024-04-29 19:27:42.000000 kbitools-0.1.1/kbitools/__init__.py
+-rw-r--r--   0 cam       (1000) cam       (1000)     1331 2024-05-19 21:06:54.000000 kbitools-0.1.1/kbitools/flags.py
+-rw-r--r--   0 cam       (1000) cam       (1000)     3951 2024-05-02 16:52:55.000000 kbitools-0.1.1/kbitools/kbi_logger.py
+-rw-r--r--   0 cam       (1000) cam       (1000)     8748 2024-05-16 22:16:56.000000 kbitools-0.1.1/kbitools/klient.py
+drwxr-xr-x   0 cam       (1000) cam       (1000)        0 2024-05-19 21:26:59.723056 kbitools-0.1.1/kbitools.egg-info/
+-rw-r--r--   0 cam       (1000) cam       (1000)      374 2024-05-19 21:26:59.000000 kbitools-0.1.1/kbitools.egg-info/PKG-INFO
+-rw-r--r--   0 cam       (1000) cam       (1000)      293 2024-05-19 21:26:59.000000 kbitools-0.1.1/kbitools.egg-info/SOURCES.txt
+-rw-r--r--   0 cam       (1000) cam       (1000)        1 2024-05-19 21:26:59.000000 kbitools-0.1.1/kbitools.egg-info/dependency_links.txt
+-rw-r--r--   0 cam       (1000) cam       (1000)       48 2024-05-19 21:26:59.000000 kbitools-0.1.1/kbitools.egg-info/entry_points.txt
+-rw-r--r--   0 cam       (1000) cam       (1000)       33 2024-05-19 21:26:59.000000 kbitools-0.1.1/kbitools.egg-info/requires.txt
+-rw-r--r--   0 cam       (1000) cam       (1000)        9 2024-05-19 21:26:59.000000 kbitools-0.1.1/kbitools.egg-info/top_level.txt
+-rw-r--r--   0 cam       (1000) cam       (1000)       38 2024-05-19 21:26:59.723056 kbitools-0.1.1/setup.cfg
+-rw-r--r--   0 cam       (1000) cam       (1000)      643 2024-05-19 21:25:24.000000 kbitools-0.1.1/setup.py
```

### Comparing `kbitools-0.1.0/kbitools/flags.py` & `kbitools-0.1.1/kbitools/flags.py`

 * *Files identical despite different names*

### Comparing `kbitools-0.1.0/kbitools/kbi_logger.py` & `kbitools-0.1.1/kbitools/kbi_logger.py`

 * *Files identical despite different names*

### Comparing `kbitools-0.1.0/kbitools/klient.py` & `kbitools-0.1.1/kbitools/klient.py`

 * *Files identical despite different names*

### Comparing `kbitools-0.1.0/setup.py` & `kbitools-0.1.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name='kbitools',
-    version='0.1.0',
+    version='0.1.1',
     author='gizmokhan',
     description='Tools and rarely-changing modules for use with the kbi daemon.',
     packages=find_packages(),
     classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     ],
     install_requires=[
         'colorama>=0.4.4',  # And any other dependencies
+        'requests>=2.31.0',
     ],
     entry_points={
         'console_scripts': [
             'kbicli = kbitools.klient:main',
         ],
     },
     python_requires=">=3.7",
```

