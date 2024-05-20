# Comparing `tmp/prompeteer-0.3.2.tar.gz` & `tmp/prompeteer-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompeteer-0.3.2.tar", last modified: Sun May 19 13:47:11 2024, max compression
+gzip compressed data, was "prompeteer-0.3.3.tar", last modified: Mon May 20 11:02:50 2024, max compression
```

## Comparing `prompeteer-0.3.2.tar` & `prompeteer-0.3.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-19 13:47:11.395364 prompeteer-0.3.2/
--rw-r--r--   0 yoaz       (502) staff       (20)       42 2024-05-15 15:30:47.000000 prompeteer-0.3.2/MANIFEST.in
--rw-r--r--   0 yoaz       (502) staff       (20)     3883 2024-05-19 13:47:11.394972 prompeteer-0.3.2/PKG-INFO
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-19 13:47:11.385072 prompeteer-0.3.2/prompeteer/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.3.2/prompeteer/__init__.py
--rw-r--r--   0 yoaz       (502) staff       (20)     4142 2024-05-19 11:15:13.000000 prompeteer-0.3.2/prompeteer/prompeteer.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-19 13:47:11.387885 prompeteer-0.3.2/prompeteer/prompt/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.3.2/prompeteer/prompt/__init__.py
--rw-r--r--   0 yoaz       (502) staff       (20)      673 2024-05-19 12:43:18.000000 prompeteer-0.3.2/prompeteer/prompt/prompt.py
--rw-r--r--   0 yoaz       (502) staff       (20)     3171 2024-05-19 13:02:38.000000 prompeteer-0.3.2/prompeteer/prompt/prompt_config.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-19 13:47:11.388914 prompeteer-0.3.2/prompeteer/providers/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.3.2/prompeteer/providers/__init__.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-19 13:47:11.390392 prompeteer-0.3.2/prompeteer/providers/aws_bedrock/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.3.2/prompeteer/providers/aws_bedrock/__init__.py
--rw-r--r--   0 yoaz       (502) staff       (20)     2085 2024-05-19 13:43:20.000000 prompeteer-0.3.2/prompeteer/providers/aws_bedrock/aws_bedrock_client.py
--rw-r--r--   0 yoaz       (502) staff       (20)     1866 2024-05-19 12:41:47.000000 prompeteer-0.3.2/prompeteer/providers/aws_bedrock/aws_llm_request.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-19 13:47:11.391343 prompeteer-0.3.2/prompeteer/providers/azure_openai/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.3.2/prompeteer/providers/azure_openai/__init__.py
--rw-r--r--   0 yoaz       (502) staff       (20)     2070 2024-05-19 12:41:18.000000 prompeteer-0.3.2/prompeteer/providers/azure_openai/azure_llm_request.py
--rw-r--r--   0 yoaz       (502) staff       (20)     3074 2024-05-19 13:17:36.000000 prompeteer-0.3.2/prompeteer/providers/azure_openai/azure_openai_client.py
--rw-r--r--   0 yoaz       (502) staff       (20)     1445 2024-05-19 11:15:13.000000 prompeteer-0.3.2/prompeteer/providers/llm_client.py
--rw-r--r--   0 yoaz       (502) staff       (20)     3790 2024-05-19 13:43:20.000000 prompeteer-0.3.2/prompeteer/providers/llm_request.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-19 13:47:11.392095 prompeteer-0.3.2/prompeteer/utils/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.3.2/prompeteer/utils/__init__.py
--rw-r--r--   0 yoaz       (502) staff       (20)     1012 2024-05-19 12:43:51.000000 prompeteer-0.3.2/prompeteer/utils/utils.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-19 13:47:11.394412 prompeteer-0.3.2/prompeteer.egg-info/
--rw-r--r--   0 yoaz       (502) staff       (20)     3883 2024-05-19 13:47:11.000000 prompeteer-0.3.2/prompeteer.egg-info/PKG-INFO
--rw-r--r--   0 yoaz       (502) staff       (20)      816 2024-05-19 13:47:11.000000 prompeteer-0.3.2/prompeteer.egg-info/SOURCES.txt
--rw-r--r--   0 yoaz       (502) staff       (20)        1 2024-05-19 13:47:11.000000 prompeteer-0.3.2/prompeteer.egg-info/dependency_links.txt
--rw-r--r--   0 yoaz       (502) staff       (20)       52 2024-05-19 13:47:11.000000 prompeteer-0.3.2/prompeteer.egg-info/requires.txt
--rw-r--r--   0 yoaz       (502) staff       (20)       11 2024-05-19 13:47:11.000000 prompeteer-0.3.2/prompeteer.egg-info/top_level.txt
--rw-r--r--   0 yoaz       (502) staff       (20)     3414 2024-05-15 13:59:10.000000 prompeteer-0.3.2/public_README.md
--rw-r--r--   0 yoaz       (502) staff       (20)       38 2024-05-19 13:47:11.395418 prompeteer-0.3.2/setup.cfg
--rw-r--r--   0 yoaz       (502) staff       (20)      877 2024-05-19 13:47:11.000000 prompeteer-0.3.2/setup.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-20 11:02:50.246636 prompeteer-0.3.3/
+-rw-r--r--   0 yoaz       (502) staff       (20)       42 2024-05-15 15:30:47.000000 prompeteer-0.3.3/MANIFEST.in
+-rw-r--r--   0 yoaz       (502) staff       (20)     3883 2024-05-20 11:02:50.246312 prompeteer-0.3.3/PKG-INFO
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-20 11:02:50.236394 prompeteer-0.3.3/prompeteer/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.3.3/prompeteer/__init__.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     4142 2024-05-19 11:15:13.000000 prompeteer-0.3.3/prompeteer/prompeteer.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-20 11:02:50.240233 prompeteer-0.3.3/prompeteer/prompt/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.3.3/prompeteer/prompt/__init__.py
+-rw-r--r--   0 yoaz       (502) staff       (20)      673 2024-05-19 12:43:18.000000 prompeteer-0.3.3/prompeteer/prompt/prompt.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     3171 2024-05-19 13:02:38.000000 prompeteer-0.3.3/prompeteer/prompt/prompt_config.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-20 11:02:50.241404 prompeteer-0.3.3/prompeteer/providers/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.3.3/prompeteer/providers/__init__.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-20 11:02:50.243052 prompeteer-0.3.3/prompeteer/providers/aws_bedrock/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.3.3/prompeteer/providers/aws_bedrock/__init__.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     2193 2024-05-20 11:00:14.000000 prompeteer-0.3.3/prompeteer/providers/aws_bedrock/aws_bedrock_client.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     1866 2024-05-19 12:41:47.000000 prompeteer-0.3.3/prompeteer/providers/aws_bedrock/aws_llm_request.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-20 11:02:50.244424 prompeteer-0.3.3/prompeteer/providers/azure_openai/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.3.3/prompeteer/providers/azure_openai/__init__.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     2070 2024-05-19 12:41:18.000000 prompeteer-0.3.3/prompeteer/providers/azure_openai/azure_llm_request.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     3074 2024-05-19 13:17:36.000000 prompeteer-0.3.3/prompeteer/providers/azure_openai/azure_openai_client.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     1445 2024-05-19 11:15:13.000000 prompeteer-0.3.3/prompeteer/providers/llm_client.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     3790 2024-05-19 13:43:20.000000 prompeteer-0.3.3/prompeteer/providers/llm_request.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-20 11:02:50.245302 prompeteer-0.3.3/prompeteer/utils/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.3.3/prompeteer/utils/__init__.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     1012 2024-05-19 12:43:51.000000 prompeteer-0.3.3/prompeteer/utils/utils.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-20 11:02:50.245880 prompeteer-0.3.3/prompeteer.egg-info/
+-rw-r--r--   0 yoaz       (502) staff       (20)     3883 2024-05-20 11:02:50.000000 prompeteer-0.3.3/prompeteer.egg-info/PKG-INFO
+-rw-r--r--   0 yoaz       (502) staff       (20)      816 2024-05-20 11:02:50.000000 prompeteer-0.3.3/prompeteer.egg-info/SOURCES.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)        1 2024-05-20 11:02:50.000000 prompeteer-0.3.3/prompeteer.egg-info/dependency_links.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)       52 2024-05-20 11:02:50.000000 prompeteer-0.3.3/prompeteer.egg-info/requires.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)       11 2024-05-20 11:02:50.000000 prompeteer-0.3.3/prompeteer.egg-info/top_level.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)     3414 2024-05-15 13:59:10.000000 prompeteer-0.3.3/public_README.md
+-rw-r--r--   0 yoaz       (502) staff       (20)       38 2024-05-20 11:02:50.246698 prompeteer-0.3.3/setup.cfg
+-rw-r--r--   0 yoaz       (502) staff       (20)      877 2024-05-20 11:02:49.000000 prompeteer-0.3.3/setup.py
```

### Comparing `prompeteer-0.3.2/PKG-INFO` & `prompeteer-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompeteer
-Version: 0.3.2
+Version: 0.3.3
 Summary: Prompt Development and Evaluation tool
 Author: Yoaz Menda
 Author-email: yoazmenda@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `prompeteer-0.3.2/prompeteer/prompeteer.py` & `prompeteer-0.3.3/prompeteer/prompeteer.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.3.2/prompeteer/prompt/prompt.py` & `prompeteer-0.3.3/prompeteer/prompt/prompt.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.3.2/prompeteer/prompt/prompt_config.py` & `prompeteer-0.3.3/prompeteer/prompt/prompt_config.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.3.2/prompeteer/providers/aws_bedrock/aws_bedrock_client.py` & `prompeteer-0.3.3/prompeteer/providers/aws_bedrock/aws_bedrock_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -38,14 +38,16 @@
                 params['temperature'] = llm_request.temperature
             if llm_request.top_p is not None:
                 params['top_p'] = llm_request.top_p
             if llm_request.top_k is not None:
                 params['top_k'] = llm_request.top_k
             if llm_request.stop_sequence is not None:
                 params['stop_sequence'] = llm_request.stop_sequence
+            if llm_request.stop_sequence is not None:
+                params['system'] = llm_request.system
 
             response = self.client.invoke_model(body=json.dumps(params), modelId=llm_request.model)
             response_body = json.loads(response.get('body').read())
 
             if len(response_body['content']) == 0:
                 raise ValueError("Empty response content, retrying...")
```

### Comparing `prompeteer-0.3.2/prompeteer/providers/aws_bedrock/aws_llm_request.py` & `prompeteer-0.3.3/prompeteer/providers/aws_bedrock/aws_llm_request.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.3.2/prompeteer/providers/azure_openai/azure_llm_request.py` & `prompeteer-0.3.3/prompeteer/providers/azure_openai/azure_llm_request.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.3.2/prompeteer/providers/azure_openai/azure_openai_client.py` & `prompeteer-0.3.3/prompeteer/providers/azure_openai/azure_openai_client.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.3.2/prompeteer/providers/llm_client.py` & `prompeteer-0.3.3/prompeteer/providers/llm_client.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.3.2/prompeteer/providers/llm_request.py` & `prompeteer-0.3.3/prompeteer/providers/llm_request.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.3.2/prompeteer/utils/utils.py` & `prompeteer-0.3.3/prompeteer/utils/utils.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.3.2/prompeteer.egg-info/PKG-INFO` & `prompeteer-0.3.3/prompeteer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompeteer
-Version: 0.3.2
+Version: 0.3.3
 Summary: Prompt Development and Evaluation tool
 Author: Yoaz Menda
 Author-email: yoazmenda@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `prompeteer-0.3.2/prompeteer.egg-info/SOURCES.txt` & `prompeteer-0.3.3/prompeteer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prompeteer-0.3.2/public_README.md` & `prompeteer-0.3.3/public_README.md`

 * *Files identical despite different names*

### Comparing `prompeteer-0.3.2/setup.py` & `prompeteer-0.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your README file
 with open("public_README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='prompeteer',
-    version='0.3.2',
+    version='0.3.3',
     author='Yoaz Menda',
     author_email='yoazmenda@gmail.com',
     description='Prompt Development and Evaluation tool',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(exclude=['tests', 'tests.*', 'README.md']),  # Include all packages
     py_modules=['prompeteer'],
```

