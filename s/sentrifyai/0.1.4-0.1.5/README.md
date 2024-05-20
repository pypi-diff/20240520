# Comparing `tmp/sentrifyai-0.1.4.tar.gz` & `tmp/sentrifyai-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentrifyai-0.1.4.tar", last modified: Mon May 20 20:34:50 2024, max compression
+gzip compressed data, was "sentrifyai-0.1.5.tar", last modified: Mon May 20 20:40:07 2024, max compression
```

## Comparing `sentrifyai-0.1.4.tar` & `sentrifyai-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-20 20:34:50.742580 sentrifyai-0.1.4/
--rw-r--r--   0 runner    (1000) runner    (1000)     1056 2024-05-20 20:23:25.000000 sentrifyai-0.1.4/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     1274 2024-05-20 20:34:50.742580 sentrifyai-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      808 2024-05-20 20:23:17.000000 sentrifyai-0.1.4/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-20 20:34:50.738580 sentrifyai-0.1.4/sentrifyai/
--rw-r--r--   0 runner    (1000) runner    (1000)      169 2024-05-20 20:30:02.000000 sentrifyai-0.1.4/sentrifyai/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1691 2024-05-20 20:23:52.000000 sentrifyai-0.1.4/sentrifyai/api.py
--rw-r--r--   0 runner    (1000) runner    (1000)       43 2024-05-20 20:23:52.000000 sentrifyai-0.1.4/sentrifyai/config.py
--rw-r--r--   0 runner    (1000) runner    (1000)      322 2024-05-20 20:23:52.000000 sentrifyai-0.1.4/sentrifyai/exceptions.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-20 20:34:50.738580 sentrifyai-0.1.4/sentrifyai.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1274 2024-05-20 20:34:50.000000 sentrifyai-0.1.4/sentrifyai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      325 2024-05-20 20:34:50.000000 sentrifyai-0.1.4/sentrifyai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-20 20:34:50.000000 sentrifyai-0.1.4/sentrifyai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       11 2024-05-20 20:34:50.000000 sentrifyai-0.1.4/sentrifyai.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        9 2024-05-20 20:34:50.000000 sentrifyai-0.1.4/sentrifyai.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       11 2024-05-20 20:34:50.000000 sentrifyai-0.1.4/sentrifyai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-20 20:34:50.742580 sentrifyai-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      676 2024-05-20 20:34:35.000000 sentrifyai-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-20 20:40:07.754106 sentrifyai-0.1.5/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1056 2024-05-20 20:23:25.000000 sentrifyai-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     1277 2024-05-20 20:40:07.754106 sentrifyai-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      811 2024-05-20 20:39:14.000000 sentrifyai-0.1.5/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-20 20:40:07.754106 sentrifyai-0.1.5/sentrifyai/
+-rw-r--r--   0 runner    (1000) runner    (1000)      169 2024-05-20 20:30:02.000000 sentrifyai-0.1.5/sentrifyai/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1691 2024-05-20 20:23:52.000000 sentrifyai-0.1.5/sentrifyai/api.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       43 2024-05-20 20:23:52.000000 sentrifyai-0.1.5/sentrifyai/config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      322 2024-05-20 20:23:52.000000 sentrifyai-0.1.5/sentrifyai/exceptions.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-20 20:40:07.754106 sentrifyai-0.1.5/sentrifyai.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1277 2024-05-20 20:40:07.000000 sentrifyai-0.1.5/sentrifyai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      325 2024-05-20 20:40:07.000000 sentrifyai-0.1.5/sentrifyai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-20 20:40:07.000000 sentrifyai-0.1.5/sentrifyai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       11 2024-05-20 20:40:07.000000 sentrifyai-0.1.5/sentrifyai.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        9 2024-05-20 20:40:07.000000 sentrifyai-0.1.5/sentrifyai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       11 2024-05-20 20:40:07.000000 sentrifyai-0.1.5/sentrifyai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-20 20:40:07.754106 sentrifyai-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      676 2024-05-20 20:39:54.000000 sentrifyai-0.1.5/setup.py
```

### Comparing `sentrifyai-0.1.4/LICENSE` & `sentrifyai-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sentrifyai-0.1.4/PKG-INFO` & `sentrifyai-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentrifyai
-Version: 0.1.4
+Version: 0.1.5
 Summary: SentrifyAI API client
 Home-page: https://github.com/sentrifybot/sentrifyai-python
 Author: SentrifyAI
 Author-email: admin@sentrify.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -25,25 +25,25 @@
 ```
 pip install sentrifyai
 ```
 
 ## Usage
 
 ```
-from sentrifyai import SentrifyAI
+from sentrifyai import api
 
 # Initialize the client
-client = SentrifyAI()
+client = api.SentrifyAI()
 
 # List models available on SentrifyAI
 models = client.list_models()
 print(models)
 
 # Classify a message using a specific model
-result = client.classify_message(model_slug='model_slug', message='Your message here')
+result = client.classify_message(model_slug='Sentrify-Mod-1.1', message='Your message here')
 print(result)
 ```
 
 ## Documentation
 
 For more detailed usage instructions and API reference, please refer to the [documentation](https://github.com/sentrifybot/sentrifyai-python).
```

### Comparing `sentrifyai-0.1.4/README.md` & `sentrifyai-0.1.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 ```
 pip install sentrifyai
 ```
 
 ## Usage
 
 ```
-from sentrifyai import SentrifyAI
+from sentrifyai import api
 
 # Initialize the client
-client = SentrifyAI()
+client = api.SentrifyAI()
 
 # List models available on SentrifyAI
 models = client.list_models()
 print(models)
 
 # Classify a message using a specific model
-result = client.classify_message(model_slug='model_slug', message='Your message here')
+result = client.classify_message(model_slug='Sentrify-Mod-1.1', message='Your message here')
 print(result)
 ```
 
 ## Documentation
 
 For more detailed usage instructions and API reference, please refer to the [documentation](https://github.com/sentrifybot/sentrifyai-python).
```

### Comparing `sentrifyai-0.1.4/sentrifyai/api.py` & `sentrifyai-0.1.5/sentrifyai/api.py`

 * *Files identical despite different names*

### Comparing `sentrifyai-0.1.4/sentrifyai.egg-info/PKG-INFO` & `sentrifyai-0.1.5/sentrifyai.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentrifyai
-Version: 0.1.4
+Version: 0.1.5
 Summary: SentrifyAI API client
 Home-page: https://github.com/sentrifybot/sentrifyai-python
 Author: SentrifyAI
 Author-email: admin@sentrify.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -25,25 +25,25 @@
 ```
 pip install sentrifyai
 ```
 
 ## Usage
 
 ```
-from sentrifyai import SentrifyAI
+from sentrifyai import api
 
 # Initialize the client
-client = SentrifyAI()
+client = api.SentrifyAI()
 
 # List models available on SentrifyAI
 models = client.list_models()
 print(models)
 
 # Classify a message using a specific model
-result = client.classify_message(model_slug='model_slug', message='Your message here')
+result = client.classify_message(model_slug='Sentrify-Mod-1.1', message='Your message here')
 print(result)
 ```
 
 ## Documentation
 
 For more detailed usage instructions and API reference, please refer to the [documentation](https://github.com/sentrifybot/sentrifyai-python).
```

### Comparing `sentrifyai-0.1.4/setup.py` & `sentrifyai-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sentrifyai',
-    version='0.1.4',
+    version='0.1.5',
     description='SentrifyAI API client',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='SentrifyAI',
     author_email='admin@sentrify.org',
     url='https://github.com/sentrifybot/sentrifyai-python',
     packages=find_packages(),
```

