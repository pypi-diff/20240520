# Comparing `tmp/pymenu_cli-1.0.5.tar.gz` & `tmp/pymenu_cli-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymenu_cli-1.0.5.tar", last modified: Sun May 19 18:13:25 2024, max compression
+gzip compressed data, was "pymenu_cli-1.0.6.tar", last modified: Sun May 19 22:57:04 2024, max compression
```

## Comparing `pymenu_cli-1.0.5.tar` & `pymenu_cli-1.0.6.tar`

### file list

```diff
@@ -1,14 +1,22 @@
-drwxr-xr-x   0 moraneus   (501) staff       (20)        0 2024-05-19 18:13:25.783700 pymenu_cli-1.0.5/
--rw-r--r--   0 moraneus   (501) staff       (20)     3013 2024-05-19 18:13:25.783496 pymenu_cli-1.0.5/PKG-INFO
--rw-r--r--   0 moraneus   (501) staff       (20)     2743 2024-05-19 18:11:26.000000 pymenu_cli-1.0.5/README.md
-drwxr-xr-x   0 moraneus   (501) staff       (20)        0 2024-05-19 18:13:25.782007 pymenu_cli-1.0.5/pymenu_cli/
--rw-r--r--   0 moraneus   (501) staff       (20)        0 2024-05-17 18:45:03.000000 pymenu_cli-1.0.5/pymenu_cli/__init__.py
--rw-r--r--   0 moraneus   (501) staff       (20)     5117 2024-05-17 18:51:29.000000 pymenu_cli-1.0.5/pymenu_cli/menu.py
-drwxr-xr-x   0 moraneus   (501) staff       (20)        0 2024-05-19 18:13:25.783280 pymenu_cli-1.0.5/pymenu_cli.egg-info/
--rw-r--r--   0 moraneus   (501) staff       (20)     3013 2024-05-19 18:13:25.000000 pymenu_cli-1.0.5/pymenu_cli.egg-info/PKG-INFO
--rw-r--r--   0 moraneus   (501) staff       (20)      233 2024-05-19 18:13:25.000000 pymenu_cli-1.0.5/pymenu_cli.egg-info/SOURCES.txt
--rw-r--r--   0 moraneus   (501) staff       (20)        1 2024-05-19 18:13:25.000000 pymenu_cli-1.0.5/pymenu_cli.egg-info/dependency_links.txt
--rw-r--r--   0 moraneus   (501) staff       (20)       52 2024-05-19 18:13:25.000000 pymenu_cli-1.0.5/pymenu_cli.egg-info/entry_points.txt
--rw-r--r--   0 moraneus   (501) staff       (20)       11 2024-05-19 18:13:25.000000 pymenu_cli-1.0.5/pymenu_cli.egg-info/top_level.txt
--rw-r--r--   0 moraneus   (501) staff       (20)       38 2024-05-19 18:13:25.783743 pymenu_cli-1.0.5/setup.cfg
--rw-r--r--   0 moraneus   (501) staff       (20)      644 2024-05-19 18:12:37.000000 pymenu_cli-1.0.5/setup.py
+drwxr-xr-x   0 moraneus   (501) staff       (20)        0 2024-05-19 22:57:04.602573 pymenu_cli-1.0.6/
+-rw-r--r--   0 moraneus   (501) staff       (20)     9017 2024-05-19 22:57:04.602240 pymenu_cli-1.0.6/PKG-INFO
+-rw-r--r--   0 moraneus   (501) staff       (20)     8704 2024-05-19 22:51:14.000000 pymenu_cli-1.0.6/README.md
+drwxr-xr-x   0 moraneus   (501) staff       (20)        0 2024-05-19 22:57:04.598620 pymenu_cli-1.0.6/pymenu_cli/
+drwxr-xr-x   0 moraneus   (501) staff       (20)        0 2024-05-19 22:57:04.600438 pymenu_cli-1.0.6/pymenu_cli/UI/
+-rw-r--r--   0 moraneus   (501) staff       (20)        0 2024-05-19 20:13:04.000000 pymenu_cli-1.0.6/pymenu_cli/UI/__init__.py
+-rw-r--r--   0 moraneus   (501) staff       (20)     1477 2024-05-19 21:10:34.000000 pymenu_cli-1.0.6/pymenu_cli/UI/styles.py
+-rw-r--r--   0 moraneus   (501) staff       (20)        0 2024-05-17 18:45:03.000000 pymenu_cli-1.0.6/pymenu_cli/__init__.py
+drwxr-xr-x   0 moraneus   (501) staff       (20)        0 2024-05-19 22:57:04.601309 pymenu_cli-1.0.6/pymenu_cli/models/
+-rw-r--r--   0 moraneus   (501) staff       (20)        0 2024-05-19 20:12:17.000000 pymenu_cli-1.0.6/pymenu_cli/models/__init__.py
+-rw-r--r--   0 moraneus   (501) staff       (20)     3916 2024-05-19 22:28:27.000000 pymenu_cli-1.0.6/pymenu_cli/models/menu.py
+-rw-r--r--   0 moraneus   (501) staff       (20)     1464 2024-05-19 22:06:18.000000 pymenu_cli-1.0.6/pymenu_cli/models/menu_item.py
+-rw-r--r--   0 moraneus   (501) staff       (20)     3271 2024-05-19 22:02:24.000000 pymenu_cli-1.0.6/pymenu_cli/pymenu.py
+drwxr-xr-x   0 moraneus   (501) staff       (20)        0 2024-05-19 22:57:04.601842 pymenu_cli-1.0.6/pymenu_cli.egg-info/
+-rw-r--r--   0 moraneus   (501) staff       (20)     9017 2024-05-19 22:57:04.000000 pymenu_cli-1.0.6/pymenu_cli.egg-info/PKG-INFO
+-rw-r--r--   0 moraneus   (501) staff       (20)      405 2024-05-19 22:57:04.000000 pymenu_cli-1.0.6/pymenu_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 moraneus   (501) staff       (20)        1 2024-05-19 22:57:04.000000 pymenu_cli-1.0.6/pymenu_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 moraneus   (501) staff       (20)       54 2024-05-19 22:57:04.000000 pymenu_cli-1.0.6/pymenu_cli.egg-info/entry_points.txt
+-rw-r--r--   0 moraneus   (501) staff       (20)       13 2024-05-19 22:57:04.000000 pymenu_cli-1.0.6/pymenu_cli.egg-info/requires.txt
+-rw-r--r--   0 moraneus   (501) staff       (20)       11 2024-05-19 22:57:04.000000 pymenu_cli-1.0.6/pymenu_cli.egg-info/top_level.txt
+-rw-r--r--   0 moraneus   (501) staff       (20)       38 2024-05-19 22:57:04.602616 pymenu_cli-1.0.6/setup.cfg
+-rw-r--r--   0 moraneus   (501) staff       (20)      701 2024-05-19 22:56:39.000000 pymenu_cli-1.0.6/setup.py
```

### Comparing `pymenu_cli-1.0.5/setup.py` & `pymenu_cli-1.0.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,27 @@
+import colorama
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pymenu-cli',
-    version='1.0.5',
+    version='1.0.6',
     description='A Python library for creating interactive CLI menus',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Moraneus',
     author_email='moraneus@gmail.com',
     url='https://github.com/moraneus/pymenu-cli',
     packages=find_packages(),
-    install_requires=[],
+    install_requires=[
+        "colorama",
+        "art"
+    ],
     entry_points={
         'console_scripts': [
-            'pymenu-cli = pymenu_cli.menu:main'
+            'pymenu-cli = pymenu_cli.pymenu:main'
         ]
     },
     license='MIT',
 )
```

