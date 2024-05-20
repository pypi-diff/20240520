# Comparing `tmp/pymonit-1.4.6.tar.gz` & `tmp/pymonit-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymonit-1.4.6.tar", last modified: Sat May 18 19:09:55 2024, max compression
+gzip compressed data, was "pymonit-1.4.7.tar", last modified: Sun May 19 13:06:09 2024, max compression
```

## Comparing `pymonit-1.4.6.tar` & `pymonit-1.4.7.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-18 19:09:55.566207 pymonit-1.4.6/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1064 2024-04-22 01:06:10.000000 pymonit-1.4.6/LICENSE
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1803 2024-05-18 19:09:55.566207 pymonit-1.4.6/PKG-INFO
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1168 2024-05-18 19:09:33.000000 pymonit-1.4.6/README.md
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-18 19:09:55.562874 pymonit-1.4.6/monit/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:06:10.000000 pymonit-1.4.6/monit/__init__.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      977 2024-05-18 17:24:00.000000 pymonit-1.4.6/monit/config.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      730 2024-05-18 18:44:31.000000 pymonit-1.4.6/monit/core.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2054 2024-05-18 18:45:14.000000 pymonit-1.4.6/monit/func.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1180 2024-05-18 17:24:34.000000 pymonit-1.4.6/monit/http.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      441 2024-05-18 18:04:46.000000 pymonit-1.4.6/monit/init.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      950 2024-05-18 17:25:03.000000 pymonit-1.4.6/monit/log2file.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1698 2024-05-18 17:25:39.000000 pymonit-1.4.6/monit/logger.py
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-18 19:09:55.566207 pymonit-1.4.6/pymonit.egg-info/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1803 2024-05-18 19:09:55.000000 pymonit-1.4.6/pymonit.egg-info/PKG-INFO
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      304 2024-05-18 19:09:55.000000 pymonit-1.4.6/pymonit.egg-info/SOURCES.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        1 2024-05-18 19:09:55.000000 pymonit-1.4.6/pymonit.egg-info/dependency_links.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-05-18 19:09:55.000000 pymonit-1.4.6/pymonit.egg-info/requires.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        6 2024-05-18 19:09:55.000000 pymonit-1.4.6/pymonit.egg-info/top_level.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)       38 2024-05-18 19:09:55.566207 pymonit-1.4.6/setup.cfg
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      865 2024-05-18 19:09:51.000000 pymonit-1.4.6/setup.py
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-19 13:06:09.436823 pymonit-1.4.7/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       76 2024-05-18 17:42:33.000000 pymonit-1.4.7/.gitignore
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1064 2024-04-22 01:06:10.000000 pymonit-1.4.7/LICENSE
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1803 2024-05-19 13:06:09.436823 pymonit-1.4.7/PKG-INFO
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1168 2024-05-18 19:09:33.000000 pymonit-1.4.7/README.md
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-19 13:06:09.436823 pymonit-1.4.7/monit/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:06:10.000000 pymonit-1.4.7/monit/__init__.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      977 2024-05-18 17:24:00.000000 pymonit-1.4.7/monit/config.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      730 2024-05-18 18:44:31.000000 pymonit-1.4.7/monit/core.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2020 2024-05-19 13:04:31.000000 pymonit-1.4.7/monit/func.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1180 2024-05-18 17:24:34.000000 pymonit-1.4.7/monit/http.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      441 2024-05-18 18:04:46.000000 pymonit-1.4.7/monit/init.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      950 2024-05-18 17:25:03.000000 pymonit-1.4.7/monit/log2file.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1698 2024-05-18 17:25:39.000000 pymonit-1.4.7/monit/logger.py
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-19 13:06:09.436823 pymonit-1.4.7/pymonit.egg-info/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1803 2024-05-19 13:06:09.000000 pymonit-1.4.7/pymonit.egg-info/PKG-INFO
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      359 2024-05-19 13:06:09.000000 pymonit-1.4.7/pymonit.egg-info/SOURCES.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        1 2024-05-19 13:06:09.000000 pymonit-1.4.7/pymonit.egg-info/dependency_links.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-05-19 13:06:09.000000 pymonit-1.4.7/pymonit.egg-info/requires.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        6 2024-05-19 13:06:09.000000 pymonit-1.4.7/pymonit.egg-info/top_level.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-04-22 01:06:10.000000 pymonit-1.4.7/requirements.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      542 2024-05-19 12:44:37.000000 pymonit-1.4.7/sample.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      320 2024-05-18 17:14:22.000000 pymonit-1.4.7/sample_static.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       38 2024-05-19 13:06:09.436823 pymonit-1.4.7/setup.cfg
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      865 2024-05-19 13:05:37.000000 pymonit-1.4.7/setup.py
```

### Comparing `pymonit-1.4.6/LICENSE` & `pymonit-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.6/PKG-INFO` & `pymonit-1.4.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymonit
-Version: 1.4.6
+Version: 1.4.7
 Summary: Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados
 Home-page: https://github.com/arktnld/monit
 Author: arktnld
 Author-email: arktnld@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pymonit-1.4.6/README.md` & `pymonit-1.4.7/README.md`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.6/monit/config.py` & `pymonit-1.4.7/monit/config.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.6/monit/core.py` & `pymonit-1.4.7/monit/core.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.6/monit/func.py` & `pymonit-1.4.7/monit/func.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 import datetime
 import traceback
 import platform
 from datetime import datetime
 
 from monit import config
 
+
 def build_json(err=None, init_time=None):
     data = {
         "project": config.project,
         "company": config.company,
         "location": config.location,
         "dev": config.dev,
         "stderr": bool(err),
         "phone": config.phone
     }
 
     if init_time:
         fim = datetime.now()
-        init_time = datetime.now()
         total_time = fim - init_time
         data["runtime"] = total_time.total_seconds()
         data["date_init"] = init_time.isoformat()
         data["date_end"] = fim.isoformat()
 
     data["cpu"] = _get_cpu_usage()
     data["mem"] = _get_memory_usage()
```

### Comparing `pymonit-1.4.6/monit/http.py` & `pymonit-1.4.7/monit/http.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.6/monit/log2file.py` & `pymonit-1.4.7/monit/log2file.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.6/monit/logger.py` & `pymonit-1.4.7/monit/logger.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.6/pymonit.egg-info/PKG-INFO` & `pymonit-1.4.7/pymonit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymonit
-Version: 1.4.6
+Version: 1.4.7
 Summary: Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados
 Home-page: https://github.com/arktnld/monit
 Author: arktnld
 Author-email: arktnld@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pymonit-1.4.6/setup.py` & `pymonit-1.4.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import pathlib
 
 setup(
     name='pymonit',
-    version='1.4.6',
+    version='1.4.7',
     description='Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados',
     long_description=pathlib.Path('README.md').read_text(),
     long_description_content_type='text/markdown',
     author='arktnld',
     author_email='arktnld@gmail.com',
     url='https://github.com/arktnld/monit',
     license='MIT',
```

