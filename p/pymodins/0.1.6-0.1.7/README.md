# Comparing `tmp/pymodins-0.1.6.tar.gz` & `tmp/pymodins-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Vimal\Desktop\pymodins\dist\.tmp-8pvfh7ue\pymodins-0.1.6.tar", last modified: Fri May 17 08:55:32 2024, max compression
+gzip compressed data, was "C:\Users\Vimal\Desktop\pymodins\dist\.tmp-yeku4cnn\pymodins-0.1.7.tar", last modified: Sun May 19 22:53:35 2024, max compression
```

## Comparing `pymodins-0.1.6.tar` & `pymodins-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 08:55:32.719318 pymodins-0.1.6/
--rw-rw-rw-   0        0        0     1085 2024-05-17 08:05:08.000000 pymodins-0.1.6/LICENSE
--rw-rw-rw-   0        0        0      483 2024-05-17 08:55:32.717314 pymodins-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-17 07:54:51.000000 pymodins-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 08:55:32.701317 pymodins-0.1.6/pymodins/
--rw-rw-rw-   0        0        0       66 2024-05-17 08:55:26.000000 pymodins-0.1.6/pymodins/__init__.py
--rw-rw-rw-   0        0        0     8126 2024-05-17 08:55:11.000000 pymodins-0.1.6/pymodins/installer.py
-drwxrwxrwx   0        0        0        0 2024-05-17 08:55:32.716317 pymodins-0.1.6/pymodins.egg-info/
--rw-rw-rw-   0        0        0      483 2024-05-17 08:55:32.000000 pymodins-0.1.6/pymodins.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      286 2024-05-17 08:55:32.000000 pymodins-0.1.6/pymodins.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 08:55:32.000000 pymodins-0.1.6/pymodins.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-05-17 08:55:32.000000 pymodins-0.1.6/pymodins.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-05-17 08:55:32.000000 pymodins-0.1.6/pymodins.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-17 08:55:32.000000 pymodins-0.1.6/pymodins.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-17 08:55:32.719318 pymodins-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      796 2024-05-17 08:55:26.000000 pymodins-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-17 08:55:32.713316 pymodins-0.1.6/test/
--rw-rw-rw-   0        0        0        0 2024-05-17 07:54:29.000000 pymodins-0.1.6/test/test-installer.py
+drwxrwxrwx   0        0        0        0 2024-05-19 22:53:35.428681 pymodins-0.1.7/
+-rw-rw-rw-   0        0        0     1085 2024-05-17 08:05:08.000000 pymodins-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     3746 2024-05-19 22:53:35.426700 pymodins-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3149 2024-05-19 19:56:43.000000 pymodins-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 22:53:35.410729 pymodins-0.1.7/pymodins/
+-rw-rw-rw-   0        0        0      335 2024-05-19 19:57:21.000000 pymodins-0.1.7/pymodins/__init__.py
+-rw-rw-rw-   0        0        0    44054 2024-05-19 22:53:08.000000 pymodins-0.1.7/pymodins/installer.py
+drwxrwxrwx   0        0        0        0 2024-05-19 22:53:35.424692 pymodins-0.1.7/pymodins.egg-info/
+-rw-rw-rw-   0        0        0     3746 2024-05-19 22:53:35.000000 pymodins-0.1.7/pymodins.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2024-05-19 22:53:35.000000 pymodins-0.1.7/pymodins.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 22:53:35.000000 pymodins-0.1.7/pymodins.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-05-19 22:53:35.000000 pymodins-0.1.7/pymodins.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-05-19 22:53:35.000000 pymodins-0.1.7/pymodins.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-19 22:53:35.000000 pymodins-0.1.7/pymodins.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 22:53:35.428681 pymodins-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      913 2024-05-19 19:59:41.000000 pymodins-0.1.7/setup.py
```

### Comparing `pymodins-0.1.6/LICENSE` & `pymodins-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodins-0.1.6/setup.py` & `pymodins-0.1.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pymodins",
-    version="0.1.6",
+    version="0.1.7",
     packages=find_packages(),
     install_requires=[
         "rich"
     ],
     entry_points={
         "console_scripts": [
             "pymodins=pymodins.installer:run",
         ],
     },
     author="Nandhan K",
     author_email="nandhan2003alamelu@gmail.com ",
     description="A module to install various Python packages.",
+    keywords="Python Module Installer, Python Package Installer, python modules installer, python package installer",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/Nandhan-KA/pymodins",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
 )
-
```

