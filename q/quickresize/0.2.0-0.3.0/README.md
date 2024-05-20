# Comparing `tmp/quickresize-0.2.0.tar.gz` & `tmp/quickresize-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickresize-0.2.0.tar", last modified: Thu May  9 11:53:49 2024, max compression
+gzip compressed data, was "quickresize-0.3.0.tar", last modified: Mon May 20 08:03:06 2024, max compression
```

## Comparing `quickresize-0.2.0.tar` & `quickresize-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:53:49.613890 quickresize-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-09 11:53:46.000000 quickresize-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-09 11:53:49.613890 quickresize-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-09 11:53:46.000000 quickresize-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:53:49.613890 quickresize-0.2.0/quickresize/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 11:53:46.000000 quickresize-0.2.0/quickresize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-09 11:53:46.000000 quickresize-0.2.0/quickresize/resize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:53:49.613890 quickresize-0.2.0/quickresize.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-09 11:53:49.000000 quickresize-0.2.0/quickresize.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-09 11:53:49.000000 quickresize-0.2.0/quickresize.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 11:53:49.000000 quickresize-0.2.0/quickresize.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-09 11:53:49.000000 quickresize-0.2.0/quickresize.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-09 11:53:49.000000 quickresize-0.2.0/quickresize.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 11:53:49.613890 quickresize-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-09 11:53:46.000000 quickresize-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:03:06.481969 quickresize-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-20 08:03:03.000000 quickresize-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-20 08:03:06.481969 quickresize-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-20 08:03:03.000000 quickresize-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:03:06.481969 quickresize-0.3.0/quickresize/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 08:03:03.000000 quickresize-0.3.0/quickresize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-20 08:03:03.000000 quickresize-0.3.0/quickresize/resize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:03:06.481969 quickresize-0.3.0/quickresize.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-20 08:03:06.000000 quickresize-0.3.0/quickresize.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-20 08:03:06.000000 quickresize-0.3.0/quickresize.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 08:03:06.000000 quickresize-0.3.0/quickresize.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-20 08:03:06.000000 quickresize-0.3.0/quickresize.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-20 08:03:06.000000 quickresize-0.3.0/quickresize.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-20 08:03:06.000000 quickresize-0.3.0/quickresize.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 08:03:06.481969 quickresize-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-20 08:03:03.000000 quickresize-0.3.0/setup.py
```

### Comparing `quickresize-0.2.0/LICENSE` & `quickresize-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quickresize-0.2.0/quickresize/resize.py` & `quickresize-0.3.0/quickresize/resize.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import argparse
 import os
-
+from tqdm import tqdm
 from PIL import Image
 
 
 def resize_images(folder:str = None, resolution:tuple[int] = None):
     '''
     In-place resizing of images present in a folder
 
     @Args:
         1. folder: path of the folder containing images.
         2. resolution: resolution of the images to be resized to.
     '''
     paths = os.listdir(folder)
-    for path in paths:
+    for path in tqdm(paths):
         f = Image.open(f'{folder}/{path}')
         f = f.resize(resolution)
         f.save(f'{folder}/{path}')
 
 def main():
     parser = argparse.ArgumentParser(prog='Name', description='Description of the program')
     parser.add_argument('--f', required=True, help='Path of the folder')
```

