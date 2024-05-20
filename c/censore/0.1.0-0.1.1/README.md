# Comparing `tmp/censore-0.1.0.tar.gz` & `tmp/censore-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "censore-0.1.0.tar", last modified: Mon May 20 18:13:13 2024, max compression
+gzip compressed data, was "censore-0.1.1.tar", last modified: Mon May 20 18:40:39 2024, max compression
```

## Comparing `censore-0.1.0.tar` & `censore-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:13:13.208781 censore-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-20 18:13:09.000000 censore-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-20 18:13:09.000000 censore-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-20 18:13:13.208781 censore-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 18:13:09.000000 censore-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:13:13.204781 censore-0.1.0/censore/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-20 18:13:09.000000 censore-0.1.0/censore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6322 2024-05-20 18:13:09.000000 censore-0.1.0/censore/censor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:13:13.208781 censore-0.1.0/censore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-20 18:13:13.000000 censore-0.1.0/censore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-20 18:13:13.000000 censore-0.1.0/censore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 18:13:13.000000 censore-0.1.0/censore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-20 18:13:13.000000 censore-0.1.0/censore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-20 18:13:13.208781 censore-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-20 18:13:09.000000 censore-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:40:39.669309 censore-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-20 18:40:35.000000 censore-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-20 18:40:35.000000 censore-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-20 18:40:39.669309 censore-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 18:40:35.000000 censore-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:40:39.669309 censore-0.1.1/censore/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-20 18:40:35.000000 censore-0.1.1/censore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6322 2024-05-20 18:40:35.000000 censore-0.1.1/censore/censor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:40:39.669309 censore-0.1.1/censore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-20 18:40:39.000000 censore-0.1.1/censore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-20 18:40:39.000000 censore-0.1.1/censore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 18:40:39.000000 censore-0.1.1/censore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-20 18:40:39.000000 censore-0.1.1/censore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-20 18:40:39.669309 censore-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-20 18:40:35.000000 censore-0.1.1/setup.py
```

### Comparing `censore-0.1.0/LICENSE` & `censore-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `censore-0.1.0/censore/censor.py` & `censore-0.1.1/censore/censor.py`

 * *Files identical despite different names*

### Comparing `censore-0.1.0/setup.py` & `censore-0.1.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name="censore",
-    version="0.1.0",
+    version="0.1.1",
     description="A package for censoring profanity in text",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Okinea Dev",
     url="https://github.com/okineadev/censore",
     packages=find_packages(),
+    package_data={'censore' :['censore/data/list/*.txt']},
     include_package_data=True,
     install_requires=[],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

