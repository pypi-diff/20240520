# Comparing `tmp/codedepot_ai-0.0.26.tar.gz` & `tmp/codedepot_ai-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codedepot_ai-0.0.26.tar", last modified: Tue May 14 16:48:34 2024, max compression
+gzip compressed data, was "codedepot_ai-0.1.0.tar", last modified: Mon May 20 10:10:14 2024, max compression
```

## Comparing `codedepot_ai-0.0.26.tar` & `codedepot_ai-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       48 2024-05-13 13:26:24.698707 codedepot_ai-0.0.26/README.md
--rw-r--r--   0        0        0        0 2024-05-13 13:14:58.280759 codedepot_ai-0.0.26/ai/__init__.py
--rw-r--r--   0        0        0    15093 2024-05-14 16:47:35.661693 codedepot_ai-0.0.26/ai/api.py
--rw-r--r--   0        0        0      624 2024-05-13 13:14:58.281422 codedepot_ai-0.0.26/ai/cluster_spec.py
--rw-r--r--   0        0        0     3947 2024-05-13 13:28:42.697260 codedepot_ai-0.0.26/ai/config.py
--rw-r--r--   0        0        0      507 2024-05-13 13:14:58.282241 codedepot_ai-0.0.26/ai/jobfile.py
--rw-r--r--   0        0        0     5553 2024-05-14 16:47:55.946487 codedepot_ai-0.0.26/ai/main.py
--rw-r--r--   0        0        0      616 2024-05-13 13:14:58.283186 codedepot_ai-0.0.26/ai/provider_spec.py
--rw-r--r--   0        0        0      771 2024-05-14 16:48:34.507972 codedepot_ai-0.0.26/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-13 13:14:58.284442 codedepot_ai-0.0.26/test/__init__.py
--rw-r--r--   0        0        0       86 2024-05-13 13:14:58.284960 codedepot_ai-0.0.26/test/resources/cluster_test.yaml
--rw-r--r--   0        0        0       87 2024-05-13 13:14:58.285531 codedepot_ai-0.0.26/test/resources/config.json
--rw-r--r--   0        0        0       80 2024-05-13 13:14:58.285845 codedepot_ai-0.0.26/test/resources/local_cred.json
--rw-r--r--   0        0        0       94 2024-05-13 13:30:47.773285 codedepot_ai-0.0.26/test/resources/provider_test.yaml
--rw-r--r--   0        0        0        0 2024-05-13 13:14:58.286084 codedepot_ai-0.0.26/test/test_client.py
--rw-r--r--   0        0        0      405 2024-05-13 13:25:27.013607 codedepot_ai-0.0.26/test/test_provider.py
--rw-r--r--   0        0        0      654 2024-05-13 13:28:42.702562 codedepot_ai-0.0.26/test/utils.py
--rw-r--r--   0        0        0      729 1970-01-01 00:00:00.000000 codedepot_ai-0.0.26/PKG-INFO
+-rw-r--r--   0        0        0       48 2024-05-19 13:16:34.101892 codedepot_ai-0.1.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-19 13:16:34.102035 codedepot_ai-0.1.0/ai/__init__.py
+-rw-r--r--   0        0        0    15523 2024-05-20 07:04:50.516845 codedepot_ai-0.1.0/ai/api.py
+-rw-r--r--   0        0        0      624 2024-05-19 13:16:34.102856 codedepot_ai-0.1.0/ai/cluster_spec.py
+-rw-r--r--   0        0        0     4006 2024-05-20 06:44:09.258505 codedepot_ai-0.1.0/ai/config.py
+-rw-r--r--   0        0        0      507 2024-05-19 13:16:34.103249 codedepot_ai-0.1.0/ai/jobfile.py
+-rw-r--r--   0        0        0     5413 2024-05-20 10:09:03.613552 codedepot_ai-0.1.0/ai/main.py
+-rw-r--r--   0        0        0      616 2024-05-19 13:16:34.112642 codedepot_ai-0.1.0/ai/provider_spec.py
+-rw-r--r--   0        0        0      769 2024-05-20 10:10:14.053544 codedepot_ai-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-19 13:16:34.113271 codedepot_ai-0.1.0/test/__init__.py
+-rw-r--r--   0        0        0       86 2024-05-19 13:16:34.113562 codedepot_ai-0.1.0/test/resources/cluster_test.yaml
+-rw-r--r--   0        0        0       87 2024-05-19 13:16:34.113676 codedepot_ai-0.1.0/test/resources/config.json
+-rw-r--r--   0        0        0       80 2024-05-19 13:16:34.113777 codedepot_ai-0.1.0/test/resources/local_cred.json
+-rw-r--r--   0        0        0       94 2024-05-19 13:16:34.113889 codedepot_ai-0.1.0/test/resources/provider_test.yaml
+-rw-r--r--   0        0        0        0 2024-05-19 13:16:34.114215 codedepot_ai-0.1.0/test/test_client.py
+-rw-r--r--   0        0        0      405 2024-05-19 13:16:34.114473 codedepot_ai-0.1.0/test/test_provider.py
+-rw-r--r--   0        0        0      654 2024-05-19 13:16:34.114624 codedepot_ai-0.1.0/test/utils.py
+-rw-r--r--   0        0        0      727 1970-01-01 00:00:00.000000 codedepot_ai-0.1.0/PKG-INFO
```

### Comparing `codedepot_ai-0.0.26/ai/api.py` & `codedepot_ai-0.1.0/ai/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from urllib import response
 
 from ai_api.models import provider
+from ai_api.models.provider_in import ProviderIn
 from ai_api.models.repository_in import RepositoryIn
 from ai_api.models.ssh_key_out import SshKeyOut
 import inquirer
 from ai.config import AIConfig
 from ai_api.exceptions import ApiException
 from ai_api.models.ssh_key_in import SshKeyIn
 from prettytable import PrettyTable
 from ai.cluster_spec import ClusterSpec
 from ai.jobfile import JobSpec
 from ai.provider_spec import ProviderSpec
 from ai_api.api import default_api
 from ai_api.api.default_api import DefaultApi
 from ai_api.models.job_instance_in import JobInstanceIn
 from ai_api.models.cluster_in import ClusterIn
-from ai_api.models.provider import Provider
+from ai_api.models.provider_in import ProviderIn
 from git_ai.metrics.experiment import get_new_exp_name
 from git_ai.cmd.ai_repo import AIRepo
 import pygit2
 import os
 from urllib.parse import urlparse
 
 
@@ -89,15 +90,14 @@
     print(table)
 
 
 def list_jobs(config: AIConfig):
     response = config.api().list_job_instances_job_instances_get()
     table = PrettyTable()
     table.field_names = ['Name', 'Status', 'Repository', 'Cluster']
-    # table._max_width = {"Name": 10, "Repository": 20}
     for job in response:
         table.add_row([job.name, job.status,
                       job.repository_url, job.cluster_name])
     print(table)
 
 
 def stop_job(config: AIConfig, job_name: str):
@@ -110,16 +110,15 @@
         instance = config.api().read_job_instance_by_name_job_instances_by_name_get(
             repo_url, job_name)
     except:
         print(f"Error reading job {job_name}.")
         return 1
 
     try:
-        config.api().delete_job_instance_job_instances_job_instance_id_delete(
-            instance.id)
+        config.api().delete_job_instance_job_instances_job_instance_id_delete(instance.id)
     except:
         print(f"Error stopping job {job_name}.")
         return 1
 
     print(f"Job {job_name} stopped.")
 
 
@@ -195,18 +194,18 @@
         repository_key=key_name,
         userlogin=config.login
     )
 
     try:
         response = config.api().create_repository_repositories_post(repo)
     except ApiException as e:
-        if 'detail' in e.body and 'already exists' in e.body:
+        if 'detail' in e.body and 'already exists' in e.body:  # type: ignore
             print(f"Repository {repo_url} already exists.")
             return None
-        if 'detail' in e.body and 'Key not found' in e.body:
+        if 'detail' in e.body and 'Key not found' in e.body:  # type: ignore
             print(f"Key {key_name} was not found.")
             return None
         else:
             print(f"Error registering repository.")
             return None
 
     return response
@@ -299,21 +298,26 @@
 
 def log(config: AIConfig, job_name: str):
     repo, repo_url = __get_repo()
     if not repo or not repo_url:
         print("Error: Cannot find a git repository in the current folder. Please run this command from a git repository.")
         return 1
 
-    instance = config.api().read_job_instance_by_name_job_instances_by_name_get(
-        repo_url, job_name)
-    if not instance:
+    try:
+        instance = config.api().read_job_instance_by_name_job_instances_by_name_get(
+            repo_url, job_name)
+    except Exception as e:
         print(f"Job {job_name} does not exist.")
         return 1
 
-    response = config.api().read_log_logs_job_instance_id_get(instance.id)
+    try:
+        response = config.api().read_log_logs_job_instance_id_get(instance.id)
+    except Exception as e:
+        print(f"Cannot read log for {job_name}.")
+        return 1
     print(response.log)
 
 
 def create_provider(config: AIConfig, spec_file: str) -> int:
     try:
         try:
             spec = ProviderSpec.from_file(spec_file)
@@ -321,60 +325,69 @@
             print(f"Error reading provider spec file.")
             return 1
 
         try:
             with open(spec.credentials, 'r') as file:
                 credentials = file.read()
         except Exception as e:
-            print(f"Error reading credentials file.")
+            print(f"Error reading credentials file {spec_file}.")
             return 1
 
-        try: 
+        try:
             provider_type = (
                 config.api().read_provider_type_by_name_provider_types_by_name_get(spec.provider_type))
         except Exception as e:
             print(f"Provider type {spec.provider_type} is not supported")
             return 1
 
         try:
             config.api().read_provider_by_name_providers_by_name_get(spec.name)
             print(f"Provider {spec.name} already exists.")
             return 1
         except ApiException as e:
             pass
 
-        response = config.api().create_provider_providers_post(Provider(
+        response = config.api().create_provider_providers_post(ProviderIn(
             name=spec.name,
-            provider_type_id=provider_type.id,  # type: ignore
+            provider_type=provider_type.name,
             credentials=credentials,
             userlogin=config.login))
         return 0
     except Exception as e:
+        print(e)
         print(f"Error creating provider.")
         return 1
 
 
 def create_cluster(config: AIConfig, spec_file: str) -> int:
     try:
         try:
             spec = ClusterSpec.from_file(spec_file)
         except Exception as e:
-            print(f"Error reading cluster spec file.")
+            print(f"Error reading cluster spec file {spec_file}.")
+            return 1
+
+        try:
+            with open(spec.key_file, 'r') as file:
+                private_key = file.read()
+        except Exception as e:
+            print(f"Error reading key file {spec.key_file}.")
             return 1
         try:
             provider = config.api().read_provider_by_name_providers_by_name_get(spec.provider)
         except ApiException as e:
             print(f"Provider {spec.provider} does not exist.")
             return 1
 
         response = config.api().create_cluster_clusters_post(ClusterIn(
             name=spec.name,
             provider_id=provider.id,
             nodes=spec.nodes,
-            userlogin=config.login))
+            userlogin=config.login,
+            cluster_key=private_key))
         return 0
     except Exception as e:
         print(f"Error creating cluster.")
         return 1
 
 
 def __register_ssh_key(config: AIConfig, name: str, path: str) -> SshKeyOut | None:
```

### Comparing `codedepot_ai-0.0.26/ai/cluster_spec.py` & `codedepot_ai-0.1.0/ai/cluster_spec.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai-0.0.26/ai/config.py` & `codedepot_ai-0.1.0/ai/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             os.path.expanduser('~'),
             AIConfig.DEFAULT_CONFIG_FOLDER,
             AIConfig.DEFAULT_CONFIG_FILE)
 
     @classmethod
     def from_file(cls, filename: str) -> 'AIConfig':
         if not os.path.exists(filename):
-            return None
+            raise FileNotFoundError(f'File {filename} does not exist')            
 
         with open(filename, 'r') as file:
             y = json.load(file)
             return cls(**y)
 
     @classmethod
     def default(cls) -> 'AIConfig':
```

### Comparing `codedepot_ai-0.0.26/ai/main.py` & `codedepot_ai-0.1.0/ai/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse
 
 from ai.config import AIConfig
-from ai.api import create_provider, create_cluster, create_ssh_key, delete_ssh_key, list_clusters, list_jobs, list_provider_types, list_providers, list_ssh_keys, refresh_managed_ssh_key, start_job, log, stop_job
+import ai.api as api
 
 
 def parse_args():
     # Create the top-level parser
     parser = argparse.ArgumentParser(
         description="Command line tool for managing jobs, clusters, and providers.")
     parser.add_argument('--version', action='store_true',
@@ -73,56 +73,56 @@
     return parser.parse_args()
 
 
 
 def main():
     args = parse_args()
     if args.version:
-        print("0.0.26")
+        print("0.1.0")
         return
 
     if args.command == 'login':
         AIConfig.create()
         return
 
     config = AIConfig.default()
     if not config:
         print("Please log in by running `ai login` first.")
         return
 
     if args.command == 'job':
         if args.job_command == 'run':
-            start_job(config, args.cluster_name)
+            api.start_job(config, args.cluster_name)
         elif args.job_command == 'list':
-            list_jobs(config)
+            api.list_jobs(config)
         elif args.job_command == 'stop':
             print(f"Stopping job {args.name}...")
-            stop_job(config, args.name)
+            api.stop_job(config, args.name)
         elif args.job_command == 'log':
             print(f"Getting log for job {args.name}...")
-            log(config, args.name)
+            api.log(config, args.name)
     elif args.command == 'cluster':
         if args.cluster_command == 'create':
             print(f"Creating cluster from {args.spec}...")
-            create_cluster(config, args.spec)
+            api.create_cluster(config, args.spec)
         elif args.cluster_command == 'list':
-            list_clusters(config)
+            api.list_clusters(config)
     elif args.command == 'provider':
         if args.provider_command == 'create':
             print(f"Creating provider from spec {args.spec}...")
-            create_provider(config, args.spec)
+            api.create_provider(config, args.spec)
         elif args.provider_command == 'list':
-            list_providers(config)
+            api.list_providers(config)
         elif args.provider_command == 'list_types':
-            list_provider_types(config)
+            api.list_provider_types(config)
     elif args.command == 'key':
         if args.key_command == 'create':
-            create_ssh_key(config, args.name, args.path)
+            api.create_ssh_key(config, args.name, args.path)
         elif args.key_command == 'delete':
             print(f"Deleting key {args.name}...")
-            delete_ssh_key(config, args.name)
+            api.delete_ssh_key(config, args.name)
         elif args.key_command == 'list':
-            list_ssh_keys(config)
+            api.list_ssh_keys(config)
         elif args.key_command == 'refresh_managed':
-            refresh_managed_ssh_key(config)
+            api.refresh_managed_ssh_key(config)
 if __name__ == "__main__":
     main()
```

### Comparing `codedepot_ai-0.0.26/ai/provider_spec.py` & `codedepot_ai-0.1.0/ai/provider_spec.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai-0.0.26/pyproject.toml` & `codedepot_ai-0.1.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.pdm]
 
 [project]
 name = "codedepot-ai"
-version = "0.0.26"
+version = "0.1.0"
 description = "Job run support for Git AI"
 readme = "README.md"
 authors = [
     { name = "CodeDepot", email = "contact@codedepot.ai" },
 ]
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -19,16 +19,16 @@
     "prompt-toolkit",
     "py",
     "pyaml",
     "pydantic",
     "pygit2",
     "requests",
     "inquirer",
-    "codedepot-git-ai>=0.0.25",
-    "codedepot-ai-api>=1.0.9",
+    "codedepot-ai-api>=1.1.0",
+    "codedepot-git-ai>=0.1.0",
 ]
 
 [project.urls]
 Homepage = "https://github.com/codedepotai/git-ai"
 
 [project.scripts]
 ai = "ai.main:main"
```

### Comparing `codedepot_ai-0.0.26/test/utils.py` & `codedepot_ai-0.1.0/test/utils.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai-0.0.26/PKG-INFO` & `codedepot_ai-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codedepot-ai
-Version: 0.0.26
+Version: 0.1.0
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
-Requires-Dist: codedepot-git-ai>=0.0.25
-Requires-Dist: codedepot-ai-api>=1.0.9
+Requires-Dist: codedepot-ai-api>=1.1.0
+Requires-Dist: codedepot-git-ai>=0.1.0
 Description-Content-Type: text/markdown
 
 # AI
 
 This is the ai client. More docs to come.
```

