# Comparing `tmp/sentrifyai-0.1.2.tar.gz` & `tmp/sentrifyai-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentrifyai-0.1.2.tar", last modified: Mon May 20 19:56:29 2024, max compression
+gzip compressed data, was "sentrifyai-0.1.3.tar", last modified: Mon May 20 20:07:01 2024, max compression
```

## Comparing `sentrifyai-0.1.2.tar` & `sentrifyai-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 railendemoss   (501) staff       (20)        0 2024-05-20 19:56:29.573652 sentrifyai-0.1.2/
--rw-r--r--   0 railendemoss   (501) staff       (20)     1056 2024-05-20 19:45:42.000000 sentrifyai-0.1.2/LICENSE
--rw-r--r--   0 railendemoss   (501) staff       (20)     1238 2024-05-20 19:56:29.573177 sentrifyai-0.1.2/PKG-INFO
--rw-r--r--   0 railendemoss   (501) staff       (20)      808 2024-05-20 19:47:19.000000 sentrifyai-0.1.2/README.md
-drwxr-xr-x   0 railendemoss   (501) staff       (20)        0 2024-05-20 19:56:29.573013 sentrifyai-0.1.2/sentrifyai.egg-info/
--rw-r--r--   0 railendemoss   (501) staff       (20)     1238 2024-05-20 19:56:29.000000 sentrifyai-0.1.2/sentrifyai.egg-info/PKG-INFO
--rw-r--r--   0 railendemoss   (501) staff       (20)      195 2024-05-20 19:56:29.000000 sentrifyai-0.1.2/sentrifyai.egg-info/SOURCES.txt
--rw-r--r--   0 railendemoss   (501) staff       (20)        1 2024-05-20 19:56:29.000000 sentrifyai-0.1.2/sentrifyai.egg-info/dependency_links.txt
--rw-r--r--   0 railendemoss   (501) staff       (20)        9 2024-05-20 19:56:29.000000 sentrifyai-0.1.2/sentrifyai.egg-info/requires.txt
--rw-r--r--   0 railendemoss   (501) staff       (20)        1 2024-05-20 19:56:29.000000 sentrifyai-0.1.2/sentrifyai.egg-info/top_level.txt
--rw-r--r--   0 railendemoss   (501) staff       (20)       38 2024-05-20 19:56:29.573818 sentrifyai-0.1.2/setup.cfg
--rw-r--r--   0 railendemoss   (501) staff       (20)      638 2024-05-20 19:56:25.000000 sentrifyai-0.1.2/setup.py
+drwxr-xr-x   0 railendemoss   (501) staff       (20)        0 2024-05-20 20:07:01.116598 sentrifyai-0.1.3/
+-rw-r--r--   0 railendemoss   (501) staff       (20)     1056 2024-05-20 19:45:42.000000 sentrifyai-0.1.3/LICENSE
+-rw-r--r--   0 railendemoss   (501) staff       (20)     1238 2024-05-20 20:07:01.116006 sentrifyai-0.1.3/PKG-INFO
+-rw-r--r--   0 railendemoss   (501) staff       (20)      808 2024-05-20 19:47:19.000000 sentrifyai-0.1.3/README.md
+drwxr-xr-x   0 railendemoss   (501) staff       (20)        0 2024-05-20 20:07:01.115708 sentrifyai-0.1.3/sentrifyai.egg-info/
+-rw-r--r--   0 railendemoss   (501) staff       (20)     1238 2024-05-20 20:07:01.000000 sentrifyai-0.1.3/sentrifyai.egg-info/PKG-INFO
+-rw-r--r--   0 railendemoss   (501) staff       (20)      195 2024-05-20 20:07:01.000000 sentrifyai-0.1.3/sentrifyai.egg-info/SOURCES.txt
+-rw-r--r--   0 railendemoss   (501) staff       (20)        1 2024-05-20 20:07:01.000000 sentrifyai-0.1.3/sentrifyai.egg-info/dependency_links.txt
+-rw-r--r--   0 railendemoss   (501) staff       (20)        9 2024-05-20 20:07:01.000000 sentrifyai-0.1.3/sentrifyai.egg-info/requires.txt
+-rw-r--r--   0 railendemoss   (501) staff       (20)        1 2024-05-20 20:07:01.000000 sentrifyai-0.1.3/sentrifyai.egg-info/top_level.txt
+-rw-r--r--   0 railendemoss   (501) staff       (20)       38 2024-05-20 20:07:01.116833 sentrifyai-0.1.3/setup.cfg
+-rw-r--r--   0 railendemoss   (501) staff       (20)      638 2024-05-20 20:06:58.000000 sentrifyai-0.1.3/setup.py
```

### Comparing `sentrifyai-0.1.2/LICENSE` & `sentrifyai-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sentrifyai-0.1.2/PKG-INFO` & `sentrifyai-0.1.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentrifyai
-Version: 0.1.2
+Version: 0.1.3
 Summary: SentrifyAI API client
 Home-page: https://github.com/sentrifybot/sentrifyai-python
 Author: SentrifyAI
 Author-email: admin@sentrify.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sentrifyai-0.1.2/README.md` & `sentrifyai-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `sentrifyai-0.1.2/sentrifyai.egg-info/PKG-INFO` & `sentrifyai-0.1.3/sentrifyai.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentrifyai
-Version: 0.1.2
+Version: 0.1.3
 Summary: SentrifyAI API client
 Home-page: https://github.com/sentrifybot/sentrifyai-python
 Author: SentrifyAI
 Author-email: admin@sentrify.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sentrifyai-0.1.2/setup.py` & `sentrifyai-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sentrifyai',
-    version='0.1.2',
+    version='0.1.3',
     description='SentrifyAI API client',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='SentrifyAI',
     author_email='admin@sentrify.org',
     url='https://github.com/sentrifybot/sentrifyai-python',
     packages=find_packages(),
```

