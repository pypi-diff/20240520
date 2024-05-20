# Comparing `tmp/codedepot_ai-0.1.0.tar.gz` & `tmp/codedepot_ai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codedepot_ai-0.1.0.tar", last modified: Mon May 20 10:10:14 2024, max compression
+gzip compressed data, was "codedepot_ai-0.1.1.tar", last modified: Mon May 20 11:10:46 2024, max compression
```

## Comparing `codedepot_ai-0.1.0.tar` & `codedepot_ai-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       48 2024-05-19 13:16:34.101892 codedepot_ai-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-19 13:16:34.102035 codedepot_ai-0.1.0/ai/__init__.py
--rw-r--r--   0        0        0    15523 2024-05-20 07:04:50.516845 codedepot_ai-0.1.0/ai/api.py
--rw-r--r--   0        0        0      624 2024-05-19 13:16:34.102856 codedepot_ai-0.1.0/ai/cluster_spec.py
--rw-r--r--   0        0        0     4006 2024-05-20 06:44:09.258505 codedepot_ai-0.1.0/ai/config.py
--rw-r--r--   0        0        0      507 2024-05-19 13:16:34.103249 codedepot_ai-0.1.0/ai/jobfile.py
--rw-r--r--   0        0        0     5413 2024-05-20 10:09:03.613552 codedepot_ai-0.1.0/ai/main.py
--rw-r--r--   0        0        0      616 2024-05-19 13:16:34.112642 codedepot_ai-0.1.0/ai/provider_spec.py
--rw-r--r--   0        0        0      769 2024-05-20 10:10:14.053544 codedepot_ai-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-19 13:16:34.113271 codedepot_ai-0.1.0/test/__init__.py
--rw-r--r--   0        0        0       86 2024-05-19 13:16:34.113562 codedepot_ai-0.1.0/test/resources/cluster_test.yaml
--rw-r--r--   0        0        0       87 2024-05-19 13:16:34.113676 codedepot_ai-0.1.0/test/resources/config.json
--rw-r--r--   0        0        0       80 2024-05-19 13:16:34.113777 codedepot_ai-0.1.0/test/resources/local_cred.json
--rw-r--r--   0        0        0       94 2024-05-19 13:16:34.113889 codedepot_ai-0.1.0/test/resources/provider_test.yaml
--rw-r--r--   0        0        0        0 2024-05-19 13:16:34.114215 codedepot_ai-0.1.0/test/test_client.py
--rw-r--r--   0        0        0      405 2024-05-19 13:16:34.114473 codedepot_ai-0.1.0/test/test_provider.py
--rw-r--r--   0        0        0      654 2024-05-19 13:16:34.114624 codedepot_ai-0.1.0/test/utils.py
--rw-r--r--   0        0        0      727 1970-01-01 00:00:00.000000 codedepot_ai-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       48 2024-05-19 13:16:34.101892 codedepot_ai-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-19 13:16:34.102035 codedepot_ai-0.1.1/ai/__init__.py
+-rw-r--r--   0        0        0    15509 2024-05-20 10:52:01.501968 codedepot_ai-0.1.1/ai/api.py
+-rw-r--r--   0        0        0      624 2024-05-19 13:16:34.102856 codedepot_ai-0.1.1/ai/cluster_spec.py
+-rw-r--r--   0        0        0     4051 2024-05-20 10:53:20.520567 codedepot_ai-0.1.1/ai/config.py
+-rw-r--r--   0        0        0      507 2024-05-19 13:16:34.103249 codedepot_ai-0.1.1/ai/jobfile.py
+-rw-r--r--   0        0        0     5413 2024-05-20 10:51:12.781449 codedepot_ai-0.1.1/ai/main.py
+-rw-r--r--   0        0        0      616 2024-05-19 13:16:34.112642 codedepot_ai-0.1.1/ai/provider_spec.py
+-rw-r--r--   0        0        0      769 2024-05-20 11:10:46.800521 codedepot_ai-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-19 13:16:34.113271 codedepot_ai-0.1.1/test/__init__.py
+-rw-r--r--   0        0        0       86 2024-05-19 13:16:34.113562 codedepot_ai-0.1.1/test/resources/cluster_test.yaml
+-rw-r--r--   0        0        0       87 2024-05-19 13:16:34.113676 codedepot_ai-0.1.1/test/resources/config.json
+-rw-r--r--   0        0        0       80 2024-05-19 13:16:34.113777 codedepot_ai-0.1.1/test/resources/local_cred.json
+-rw-r--r--   0        0        0       94 2024-05-19 13:16:34.113889 codedepot_ai-0.1.1/test/resources/provider_test.yaml
+-rw-r--r--   0        0        0        0 2024-05-19 13:16:34.114215 codedepot_ai-0.1.1/test/test_client.py
+-rw-r--r--   0        0        0      405 2024-05-19 13:16:34.114473 codedepot_ai-0.1.1/test/test_provider.py
+-rw-r--r--   0        0        0      654 2024-05-19 13:16:34.114624 codedepot_ai-0.1.1/test/utils.py
+-rw-r--r--   0        0        0      727 1970-01-01 00:00:00.000000 codedepot_ai-0.1.1/PKG-INFO
```

### Comparing `codedepot_ai-0.1.0/ai/api.py` & `codedepot_ai-0.1.1/ai/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
 def list_clusters(config: AIConfig):
     response = config.api().list_clusters_clusters_get()
     table = PrettyTable()
     table.field_names = ['Name', 'Provider', 'Type', 'Status']
     for cluster in response:
         table.add_row([cluster.name, cluster.provider.name,
-                      cluster.provider.provider_type.name, 'Reachable'])
+                      cluster.provider.provider_type.name, cluster.status])
     print(table)
 
 
 def list_provider_types(config: AIConfig):
     response = config.api().list_providers_types_provider_types_get()
     table = PrettyTable()
     table.field_names = ['Name', 'Module']
@@ -349,15 +349,14 @@
         response = config.api().create_provider_providers_post(ProviderIn(
             name=spec.name,
             provider_type=provider_type.name,
             credentials=credentials,
             userlogin=config.login))
         return 0
     except Exception as e:
-        print(e)
         print(f"Error creating provider.")
         return 1
 
 
 def create_cluster(config: AIConfig, spec_file: str) -> int:
     try:
         try:
```

### Comparing `codedepot_ai-0.1.0/ai/cluster_spec.py` & `codedepot_ai-0.1.1/ai/cluster_spec.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai-0.1.0/ai/config.py` & `codedepot_ai-0.1.1/ai/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from email.policy import default
 import json
 import os
 from prompt_toolkit import prompt
 
 from ai_api.api.default_api import DefaultApi
-from ai_api.api_client import ApiClient, Configuration
+from ai_api.api_client import ApiClient
+from ai_api.configuration import Configuration
 
 
 class AIConfig(object):
-    DEFAULT_CONFIG_FOLDER = '.api'
+    DEFAULT_CONFIG_FOLDER = '.ai'
     DEFAULT_CONFIG_FILE = 'config.json'
 
     def __init__(self, login: str, token: str, endpoint: str, email: str):
         config = Configuration(host=endpoint)
         config.access_token = token
         self.default_api = DefaultApi(ApiClient(config))
 
@@ -112,10 +113,10 @@
             f'Enter the password for {username}: ', is_password=True)
         default_api = DefaultApi(ApiClient(Configuration(host=endpoint)))
 
         response = default_api.login_token_post(
             username=email, password=password)
 
         config = AIConfig(
-            token=response['token'], endpoint=endpoint, login=username, email=email)
+            token=response['token'], endpoint=endpoint, login=username, email=email) # type: ignore
         config.save()
-        print('The user is logged in, the token is stored at ~/.api/config.json')
+        print('The user is logged in, the token is stored at ~/.ai/config.json')
```

### Comparing `codedepot_ai-0.1.0/ai/main.py` & `codedepot_ai-0.1.1/ai/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     return parser.parse_args()
 
 
 
 def main():
     args = parse_args()
     if args.version:
-        print("0.1.0")
+        print("0.1.1")
         return
 
     if args.command == 'login':
         AIConfig.create()
         return
 
     config = AIConfig.default()
```

### Comparing `codedepot_ai-0.1.0/ai/provider_spec.py` & `codedepot_ai-0.1.1/ai/provider_spec.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai-0.1.0/pyproject.toml` & `codedepot_ai-0.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.pdm]
 
 [project]
 name = "codedepot-ai"
-version = "0.1.0"
+version = "0.1.1"
 description = "Job run support for Git AI"
 readme = "README.md"
 authors = [
     { name = "CodeDepot", email = "contact@codedepot.ai" },
 ]
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -19,15 +19,15 @@
     "prompt-toolkit",
     "py",
     "pyaml",
     "pydantic",
     "pygit2",
     "requests",
     "inquirer",
-    "codedepot-ai-api>=1.1.0",
+    "codedepot-ai-api>=1.1.1",
     "codedepot-git-ai>=0.1.0",
 ]
 
 [project.urls]
 Homepage = "https://github.com/codedepotai/git-ai"
 
 [project.scripts]
```

### Comparing `codedepot_ai-0.1.0/test/utils.py` & `codedepot_ai-0.1.1/test/utils.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai-0.1.0/PKG-INFO` & `codedepot_ai-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codedepot-ai
-Version: 0.1.0
+Version: 0.1.1
 Summary: Job run support for Git AI
 Author-Email: CodeDepot <contact@codedepot.ai>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Homepage, https://github.com/codedepotai/git-ai
 Requires-Python: >=3.10
@@ -12,14 +12,14 @@
 Requires-Dist: prompt-toolkit
 Requires-Dist: py
 Requires-Dist: pyaml
 Requires-Dist: pydantic
 Requires-Dist: pygit2
 Requires-Dist: requests
 Requires-Dist: inquirer
-Requires-Dist: codedepot-ai-api>=1.1.0
+Requires-Dist: codedepot-ai-api>=1.1.1
 Requires-Dist: codedepot-git-ai>=0.1.0
 Description-Content-Type: text/markdown
 
 # AI
 
 This is the ai client. More docs to come.
```

