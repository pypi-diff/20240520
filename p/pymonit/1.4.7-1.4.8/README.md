# Comparing `tmp/pymonit-1.4.7.tar.gz` & `tmp/pymonit-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymonit-1.4.7.tar", last modified: Sun May 19 13:06:09 2024, max compression
+gzip compressed data, was "pymonit-1.4.8.tar", last modified: Mon May 20 10:10:18 2024, max compression
```

## Comparing `pymonit-1.4.7.tar` & `pymonit-1.4.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-19 13:06:09.436823 pymonit-1.4.7/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)       76 2024-05-18 17:42:33.000000 pymonit-1.4.7/.gitignore
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1064 2024-04-22 01:06:10.000000 pymonit-1.4.7/LICENSE
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1803 2024-05-19 13:06:09.436823 pymonit-1.4.7/PKG-INFO
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1168 2024-05-18 19:09:33.000000 pymonit-1.4.7/README.md
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-19 13:06:09.436823 pymonit-1.4.7/monit/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:06:10.000000 pymonit-1.4.7/monit/__init__.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      977 2024-05-18 17:24:00.000000 pymonit-1.4.7/monit/config.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      730 2024-05-18 18:44:31.000000 pymonit-1.4.7/monit/core.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2020 2024-05-19 13:04:31.000000 pymonit-1.4.7/monit/func.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1180 2024-05-18 17:24:34.000000 pymonit-1.4.7/monit/http.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      441 2024-05-18 18:04:46.000000 pymonit-1.4.7/monit/init.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      950 2024-05-18 17:25:03.000000 pymonit-1.4.7/monit/log2file.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1698 2024-05-18 17:25:39.000000 pymonit-1.4.7/monit/logger.py
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-19 13:06:09.436823 pymonit-1.4.7/pymonit.egg-info/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1803 2024-05-19 13:06:09.000000 pymonit-1.4.7/pymonit.egg-info/PKG-INFO
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      359 2024-05-19 13:06:09.000000 pymonit-1.4.7/pymonit.egg-info/SOURCES.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        1 2024-05-19 13:06:09.000000 pymonit-1.4.7/pymonit.egg-info/dependency_links.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-05-19 13:06:09.000000 pymonit-1.4.7/pymonit.egg-info/requires.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        6 2024-05-19 13:06:09.000000 pymonit-1.4.7/pymonit.egg-info/top_level.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-04-22 01:06:10.000000 pymonit-1.4.7/requirements.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      542 2024-05-19 12:44:37.000000 pymonit-1.4.7/sample.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      320 2024-05-18 17:14:22.000000 pymonit-1.4.7/sample_static.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)       38 2024-05-19 13:06:09.436823 pymonit-1.4.7/setup.cfg
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      865 2024-05-19 13:05:37.000000 pymonit-1.4.7/setup.py
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-20 10:10:18.589273 pymonit-1.4.8/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       86 2024-05-19 13:06:25.000000 pymonit-1.4.8/.gitignore
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1064 2024-04-22 01:06:10.000000 pymonit-1.4.8/LICENSE
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1820 2024-05-20 10:10:18.589273 pymonit-1.4.8/PKG-INFO
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1185 2024-05-20 10:09:51.000000 pymonit-1.4.8/README.md
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-20 10:10:18.589273 pymonit-1.4.8/monit/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:06:10.000000 pymonit-1.4.8/monit/__init__.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      977 2024-05-18 17:24:00.000000 pymonit-1.4.8/monit/config.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      730 2024-05-18 18:44:31.000000 pymonit-1.4.8/monit/core.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2020 2024-05-19 13:04:31.000000 pymonit-1.4.8/monit/func.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1180 2024-05-18 17:24:34.000000 pymonit-1.4.8/monit/http.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      441 2024-05-18 18:04:46.000000 pymonit-1.4.8/monit/init.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      950 2024-05-18 17:25:03.000000 pymonit-1.4.8/monit/log2file.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1698 2024-05-18 17:25:39.000000 pymonit-1.4.8/monit/logger.py
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-20 10:10:18.589273 pymonit-1.4.8/pymonit.egg-info/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1820 2024-05-20 10:10:18.000000 pymonit-1.4.8/pymonit.egg-info/PKG-INFO
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      359 2024-05-20 10:10:18.000000 pymonit-1.4.8/pymonit.egg-info/SOURCES.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        1 2024-05-20 10:10:18.000000 pymonit-1.4.8/pymonit.egg-info/dependency_links.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-05-20 10:10:18.000000 pymonit-1.4.8/pymonit.egg-info/requires.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        6 2024-05-20 10:10:18.000000 pymonit-1.4.8/pymonit.egg-info/top_level.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-04-22 01:06:10.000000 pymonit-1.4.8/requirements.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      542 2024-05-19 12:44:37.000000 pymonit-1.4.8/sample.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      320 2024-05-18 17:14:22.000000 pymonit-1.4.8/sample_static.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       38 2024-05-20 10:10:18.592606 pymonit-1.4.8/setup.cfg
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      865 2024-05-20 10:10:15.000000 pymonit-1.4.8/setup.py
```

### Comparing `pymonit-1.4.7/LICENSE` & `pymonit-1.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.7/PKG-INFO` & `pymonit-1.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymonit
-Version: 1.4.7
+Version: 1.4.8
 Summary: Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados
 Home-page: https://github.com/arktnld/monit
 Author: arktnld
 Author-email: arktnld@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -49,14 +49,16 @@
     try:
         time.sleep(5)
         raise ValueError("This is a sample error.")
 
     except Exception as e:
         monit.notify_and_exit(e)
 
+    monit.end()
+
 
 if __name__ == "__main__":
     main()
 ```
 
 **Utilização avançada**
```

### Comparing `pymonit-1.4.7/README.md` & `pymonit-1.4.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -30,14 +30,16 @@
     try:
         time.sleep(5)
         raise ValueError("This is a sample error.")
 
     except Exception as e:
         monit.notify_and_exit(e)
 
+    monit.end()
+
 
 if __name__ == "__main__":
     main()
 ```
 
 **Utilização avançada**
```

### Comparing `pymonit-1.4.7/monit/config.py` & `pymonit-1.4.8/monit/config.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.7/monit/core.py` & `pymonit-1.4.8/monit/core.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.7/monit/func.py` & `pymonit-1.4.8/monit/func.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.7/monit/http.py` & `pymonit-1.4.8/monit/http.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.7/monit/log2file.py` & `pymonit-1.4.8/monit/log2file.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.7/monit/logger.py` & `pymonit-1.4.8/monit/logger.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.7/pymonit.egg-info/PKG-INFO` & `pymonit-1.4.8/pymonit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymonit
-Version: 1.4.7
+Version: 1.4.8
 Summary: Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados
 Home-page: https://github.com/arktnld/monit
 Author: arktnld
 Author-email: arktnld@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -49,14 +49,16 @@
     try:
         time.sleep(5)
         raise ValueError("This is a sample error.")
 
     except Exception as e:
         monit.notify_and_exit(e)
 
+    monit.end()
+
 
 if __name__ == "__main__":
     main()
 ```
 
 **Utilização avançada**
```

### Comparing `pymonit-1.4.7/sample.py` & `pymonit-1.4.8/sample.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.7/setup.py` & `pymonit-1.4.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import pathlib
 
 setup(
     name='pymonit',
-    version='1.4.7',
+    version='1.4.8',
     description='Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados',
     long_description=pathlib.Path('README.md').read_text(),
     long_description_content_type='text/markdown',
     author='arktnld',
     author_email='arktnld@gmail.com',
     url='https://github.com/arktnld/monit',
     license='MIT',
```

