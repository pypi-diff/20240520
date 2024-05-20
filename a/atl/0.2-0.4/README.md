# Comparing `tmp/atl-0.2.tar.gz` & `tmp/atl-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atl-0.2.tar", last modified: Mon Apr  8 16:20:39 2024, max compression
+gzip compressed data, was "atl-0.4.tar", last modified: Mon May 20 00:49:16 2024, max compression
```

## Comparing `atl-0.2.tar` & `atl-0.4.tar`

### file list

```diff
@@ -1,12 +1,20 @@
-drwxr-xr-x   0 tux        (501) staff       (20)        0 2024-04-08 16:20:39.129247 atl-0.2/
--rw-r--r--   0 tux        (501) staff       (20)      357 2024-04-08 16:03:39.000000 atl-0.2/LICENSE
--rw-r--r--   0 tux        (501) staff       (20)     2067 2024-04-08 16:20:39.129028 atl-0.2/PKG-INFO
--rw-r--r--   0 tux        (501) staff       (20)     1079 2024-04-08 16:20:27.000000 atl-0.2/README.md
-drwxr-xr-x   0 tux        (501) staff       (20)        0 2024-04-08 16:20:39.128797 atl-0.2/atl.egg-info/
--rw-r--r--   0 tux        (501) staff       (20)     2067 2024-04-08 16:20:39.000000 atl-0.2/atl.egg-info/PKG-INFO
--rw-r--r--   0 tux        (501) staff       (20)      160 2024-04-08 16:20:39.000000 atl-0.2/atl.egg-info/SOURCES.txt
--rw-r--r--   0 tux        (501) staff       (20)        1 2024-04-08 16:20:39.000000 atl-0.2/atl.egg-info/dependency_links.txt
--rw-r--r--   0 tux        (501) staff       (20)       31 2024-04-08 16:20:39.000000 atl-0.2/atl.egg-info/requires.txt
--rw-r--r--   0 tux        (501) staff       (20)        1 2024-04-08 16:20:39.000000 atl-0.2/atl.egg-info/top_level.txt
--rw-r--r--   0 tux        (501) staff       (20)       38 2024-04-08 16:20:39.129291 atl-0.2/setup.cfg
--rw-r--r--   0 tux        (501) staff       (20)      888 2024-04-08 16:19:36.000000 atl-0.2/setup.py
+drwxrwxr-x   0 tux       (1000) tux       (1000)        0 2024-05-20 00:49:16.883471 atl-0.4/
+-rwxrwxr-x   0 tux       (1000) tux       (1000)      357 2024-05-19 23:39:35.000000 atl-0.4/LICENSE
+-rw-r--r--   0 tux       (1000) tux       (1000)     2965 2024-05-20 00:49:16.883471 atl-0.4/PKG-INFO
+-rwxrwxr-x   0 tux       (1000) tux       (1000)     1753 2024-05-20 00:49:05.000000 atl-0.4/README.md
+drwxrwxr-x   0 tux       (1000) tux       (1000)        0 2024-05-20 00:49:16.879471 atl-0.4/atl/
+-rwxrwxr-x   0 tux       (1000) tux       (1000)        0 2024-05-19 23:39:35.000000 atl-0.4/atl/__init__.py
+drwxrwxr-x   0 tux       (1000) tux       (1000)        0 2024-05-20 00:49:16.883471 atl-0.4/atl/module1_example/
+-rwxrwxr-x   0 tux       (1000) tux       (1000)        0 2024-05-19 23:39:35.000000 atl-0.4/atl/module1_example/__init__.py
+-rwxrwxr-x   0 tux       (1000) tux       (1000)       97 2024-05-19 23:39:35.000000 atl-0.4/atl/module1_example/functions1.py
+drwxrwxr-x   0 tux       (1000) tux       (1000)        0 2024-05-20 00:49:16.883471 atl-0.4/atl/module2_example/
+-rwxrwxr-x   0 tux       (1000) tux       (1000)        0 2024-05-19 23:39:35.000000 atl-0.4/atl/module2_example/__init__.py
+-rwxrwxr-x   0 tux       (1000) tux       (1000)      102 2024-05-19 23:39:35.000000 atl-0.4/atl/module2_example/functions1.py
+drwxrwxr-x   0 tux       (1000) tux       (1000)        0 2024-05-20 00:49:16.883471 atl-0.4/atl.egg-info/
+-rw-r--r--   0 tux       (1000) tux       (1000)     2965 2024-05-20 00:49:16.000000 atl-0.4/atl.egg-info/PKG-INFO
+-rw-rw-r--   0 tux       (1000) tux       (1000)      308 2024-05-20 00:49:16.000000 atl-0.4/atl.egg-info/SOURCES.txt
+-rw-rw-r--   0 tux       (1000) tux       (1000)        1 2024-05-20 00:49:16.000000 atl-0.4/atl.egg-info/dependency_links.txt
+-rw-rw-r--   0 tux       (1000) tux       (1000)       31 2024-05-20 00:49:16.000000 atl-0.4/atl.egg-info/requires.txt
+-rw-rw-r--   0 tux       (1000) tux       (1000)        4 2024-05-20 00:49:16.000000 atl-0.4/atl.egg-info/top_level.txt
+-rw-rw-r--   0 tux       (1000) tux       (1000)       38 2024-05-20 00:49:16.883471 atl-0.4/setup.cfg
+-rwxrwxr-x   0 tux       (1000) tux       (1000)     1245 2024-05-20 00:48:27.000000 atl-0.4/setup.py
```

### Comparing `atl-0.2/setup.py` & `atl-0.4/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 from setuptools import setup, find_packages
 
-with open('README.md', 'r') as f:
+with open("/tmp/projdir.pwd", "r") as f:
+    project_path = f.read().strip()
+
+with open(f"{project_path}/README.md", "r") as f:
     long_description = f.read()
 
-with open('requirements.txt') as f:
+with open(f"{project_path}/requirements.txt", "r") as f:
     required_packages = f.read().splitlines()
 
-with open('LICENSE') as f:
+with open(f"{project_path}/LICENSE", "r") as f:
     license_text = f.read()
 
 setup(
-    name='atl',
-    version='0.2',
+    name="atl",
+    version="0.4",
     packages=find_packages(),
-    description='ambedded.ch ambedded-technology-lab python3 library',
+    description="ambedded.ch ambedded-technology-lab python3 library",
     long_description=long_description,
-    long_description_content_type='text/markdown',
-    author='ambedded.ch',
-    author_email='info@ambedded.ch',
+    long_description_content_type="text/markdown",
+    author="ambedded.ch",
+    author_email="info@ambedded.ch",
     classifiers=[
-        'Development Status :: 3 - Alpha',
+        'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
+        'License :: OSI Approved :: GNU General Public License v2 (GPLv2)',
         'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
     ],
     install_requires=required_packages,
     license=license_text,
-    url='https://gitlab.com/ambedded-labs/al-pypi-ambedded-atl',
+    url="https://gitlab.com/ambedded-labs/al-pypi-ambedded-atl",
 )
```

