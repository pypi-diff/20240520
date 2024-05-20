# Comparing `tmp/sentrifyai-0.1.1.tar.gz` & `tmp/sentrifyai-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentrifyai-0.1.1.tar", last modified: Mon May 20 19:33:15 2024, max compression
+gzip compressed data, was "sentrifyai-0.1.2.tar", last modified: Mon May 20 19:56:29 2024, max compression
```

## Comparing `sentrifyai-0.1.1.tar` & `sentrifyai-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,12 @@
-drwxr-xr-x   0 railendemoss   (501) staff       (20)        0 2024-05-20 19:33:15.317947 sentrifyai-0.1.1/
--rw-r--r--   0 railendemoss   (501) staff       (20)     1056 2024-05-20 19:18:13.000000 sentrifyai-0.1.1/LICENSE
--rw-r--r--   0 railendemoss   (501) staff       (20)     1272 2024-05-20 19:33:15.317363 sentrifyai-0.1.1/PKG-INFO
--rw-r--r--   0 railendemoss   (501) staff       (20)      843 2024-05-20 19:29:13.000000 sentrifyai-0.1.1/README.md
-drwxr-xr-x   0 railendemoss   (501) staff       (20)        0 2024-05-20 19:33:15.316992 sentrifyai-0.1.1/sentrifyai.egg-info/
--rw-r--r--   0 railendemoss   (501) staff       (20)     1272 2024-05-20 19:33:15.000000 sentrifyai-0.1.1/sentrifyai.egg-info/PKG-INFO
--rw-r--r--   0 railendemoss   (501) staff       (20)      213 2024-05-20 19:33:15.000000 sentrifyai-0.1.1/sentrifyai.egg-info/SOURCES.txt
--rw-r--r--   0 railendemoss   (501) staff       (20)        1 2024-05-20 19:33:15.000000 sentrifyai-0.1.1/sentrifyai.egg-info/dependency_links.txt
--rw-r--r--   0 railendemoss   (501) staff       (20)        9 2024-05-20 19:33:15.000000 sentrifyai-0.1.1/sentrifyai.egg-info/requires.txt
--rw-r--r--   0 railendemoss   (501) staff       (20)        1 2024-05-20 19:33:15.000000 sentrifyai-0.1.1/sentrifyai.egg-info/top_level.txt
--rw-r--r--   0 railendemoss   (501) staff       (20)       38 2024-05-20 19:33:15.317993 sentrifyai-0.1.1/setup.cfg
--rw-r--r--   0 railendemoss   (501) staff       (20)      638 2024-05-20 19:33:11.000000 sentrifyai-0.1.1/setup.py
-drwxr-xr-x   0 railendemoss   (501) staff       (20)        0 2024-05-20 19:33:15.317113 sentrifyai-0.1.1/tests/
--rw-r--r--   0 railendemoss   (501) staff       (20)      599 2024-05-20 19:12:58.000000 sentrifyai-0.1.1/tests/test_api.py
+drwxr-xr-x   0 railendemoss   (501) staff       (20)        0 2024-05-20 19:56:29.573652 sentrifyai-0.1.2/
+-rw-r--r--   0 railendemoss   (501) staff       (20)     1056 2024-05-20 19:45:42.000000 sentrifyai-0.1.2/LICENSE
+-rw-r--r--   0 railendemoss   (501) staff       (20)     1238 2024-05-20 19:56:29.573177 sentrifyai-0.1.2/PKG-INFO
+-rw-r--r--   0 railendemoss   (501) staff       (20)      808 2024-05-20 19:47:19.000000 sentrifyai-0.1.2/README.md
+drwxr-xr-x   0 railendemoss   (501) staff       (20)        0 2024-05-20 19:56:29.573013 sentrifyai-0.1.2/sentrifyai.egg-info/
+-rw-r--r--   0 railendemoss   (501) staff       (20)     1238 2024-05-20 19:56:29.000000 sentrifyai-0.1.2/sentrifyai.egg-info/PKG-INFO
+-rw-r--r--   0 railendemoss   (501) staff       (20)      195 2024-05-20 19:56:29.000000 sentrifyai-0.1.2/sentrifyai.egg-info/SOURCES.txt
+-rw-r--r--   0 railendemoss   (501) staff       (20)        1 2024-05-20 19:56:29.000000 sentrifyai-0.1.2/sentrifyai.egg-info/dependency_links.txt
+-rw-r--r--   0 railendemoss   (501) staff       (20)        9 2024-05-20 19:56:29.000000 sentrifyai-0.1.2/sentrifyai.egg-info/requires.txt
+-rw-r--r--   0 railendemoss   (501) staff       (20)        1 2024-05-20 19:56:29.000000 sentrifyai-0.1.2/sentrifyai.egg-info/top_level.txt
+-rw-r--r--   0 railendemoss   (501) staff       (20)       38 2024-05-20 19:56:29.573818 sentrifyai-0.1.2/setup.cfg
+-rw-r--r--   0 railendemoss   (501) staff       (20)      638 2024-05-20 19:56:25.000000 sentrifyai-0.1.2/setup.py
```

### Comparing `sentrifyai-0.1.1/LICENSE` & `sentrifyai-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sentrifyai-0.1.1/PKG-INFO` & `sentrifyai-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentrifyai
-Version: 0.1.1
+Version: 0.1.2
 Summary: SentrifyAI API client
 Home-page: https://github.com/sentrifybot/sentrifyai-python
 Author: SentrifyAI
 Author-email: admin@sentrify.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,26 +25,26 @@
 ```
 
 ## Usage
 
 ```
 from sentrifyai import SentrifyAI
 
-# Initialize the client with your API key
-client = SentrifyAI(api_key='your_api_key')
+# Initialize the client
+client = SentrifyAI()
 
 # List models available on SentrifyAI
 models = client.list_models()
 print(models)
 
 # Classify a message using a specific model
 result = client.classify_message(model_slug='model_slug', message='Your message here')
 print(result)
 ```
 
 ## Documentation
 
-For more detailed usage instructions and API reference, please refer to the [documentation](https://github.com/yourusername/sentrifyai).
+For more detailed usage instructions and API reference, please refer to the [documentation](https://github.com/sentrifybot/sentrifyai-python).
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

### Comparing `sentrifyai-0.1.1/README.md` & `sentrifyai-0.1.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 ```
 
 ## Usage
 
 ```
 from sentrifyai import SentrifyAI
 
-# Initialize the client with your API key
-client = SentrifyAI(api_key='your_api_key')
+# Initialize the client
+client = SentrifyAI()
 
 # List models available on SentrifyAI
 models = client.list_models()
 print(models)
 
 # Classify a message using a specific model
 result = client.classify_message(model_slug='model_slug', message='Your message here')
 print(result)
 ```
 
 ## Documentation
 
-For more detailed usage instructions and API reference, please refer to the [documentation](https://github.com/yourusername/sentrifyai).
+For more detailed usage instructions and API reference, please refer to the [documentation](https://github.com/sentrifybot/sentrifyai-python).
 
 ## License
 
-This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
+This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

### Comparing `sentrifyai-0.1.1/sentrifyai.egg-info/PKG-INFO` & `sentrifyai-0.1.2/sentrifyai.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentrifyai
-Version: 0.1.1
+Version: 0.1.2
 Summary: SentrifyAI API client
 Home-page: https://github.com/sentrifybot/sentrifyai-python
 Author: SentrifyAI
 Author-email: admin@sentrify.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,26 +25,26 @@
 ```
 
 ## Usage
 
 ```
 from sentrifyai import SentrifyAI
 
-# Initialize the client with your API key
-client = SentrifyAI(api_key='your_api_key')
+# Initialize the client
+client = SentrifyAI()
 
 # List models available on SentrifyAI
 models = client.list_models()
 print(models)
 
 # Classify a message using a specific model
 result = client.classify_message(model_slug='model_slug', message='Your message here')
 print(result)
 ```
 
 ## Documentation
 
-For more detailed usage instructions and API reference, please refer to the [documentation](https://github.com/yourusername/sentrifyai).
+For more detailed usage instructions and API reference, please refer to the [documentation](https://github.com/sentrifybot/sentrifyai-python).
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

### Comparing `sentrifyai-0.1.1/setup.py` & `sentrifyai-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sentrifyai',
-    version='0.1.1',
+    version='0.1.2',
     description='SentrifyAI API client',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='SentrifyAI',
     author_email='admin@sentrify.org',
     url='https://github.com/sentrifybot/sentrifyai-python',
     packages=find_packages(),
```

