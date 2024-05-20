# Comparing `tmp/lfg_llama-2.0.2.tar.gz` & `tmp/lfg_llama-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lfg_llama-2.0.2.tar", last modified: Mon May 13 18:51:29 2024, max compression
+gzip compressed data, was "lfg_llama-2.1.0.tar", last modified: Mon May 20 18:04:06 2024, max compression
```

## Comparing `lfg_llama-2.0.2.tar` & `lfg_llama-2.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-13 18:51:29.958538 lfg_llama-2.0.2/
--rw-r--r--   0 ob907      (502) staff       (20)     2132 2024-05-13 18:51:29.958334 lfg_llama-2.0.2/PKG-INFO
--rw-r--r--   0 ob907      (502) staff       (20)     1893 2024-05-13 18:45:42.000000 lfg_llama-2.0.2/README.md
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-13 18:51:29.956334 lfg_llama-2.0.2/lfg/
--rw-r--r--   0 ob907      (502) staff       (20)        0 2024-04-28 17:51:36.000000 lfg_llama-2.0.2/lfg/__init__.py
--rwxr-xr-x   0 ob907      (502) staff       (20)     3031 2024-05-13 18:46:49.000000 lfg_llama-2.0.2/lfg/cli.py
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-13 18:51:29.957946 lfg_llama-2.0.2/lfg_llama.egg-info/
--rw-r--r--   0 ob907      (502) staff       (20)     2132 2024-05-13 18:51:29.000000 lfg_llama-2.0.2/lfg_llama.egg-info/PKG-INFO
--rw-r--r--   0 ob907      (502) staff       (20)      245 2024-05-13 18:51:29.000000 lfg_llama-2.0.2/lfg_llama.egg-info/SOURCES.txt
--rw-r--r--   0 ob907      (502) staff       (20)        1 2024-05-13 18:51:29.000000 lfg_llama-2.0.2/lfg_llama.egg-info/dependency_links.txt
--rw-r--r--   0 ob907      (502) staff       (20)       37 2024-05-13 18:51:29.000000 lfg_llama-2.0.2/lfg_llama.egg-info/entry_points.txt
--rw-r--r--   0 ob907      (502) staff       (20)        7 2024-05-13 18:51:29.000000 lfg_llama-2.0.2/lfg_llama.egg-info/requires.txt
--rw-r--r--   0 ob907      (502) staff       (20)        4 2024-05-13 18:51:29.000000 lfg_llama-2.0.2/lfg_llama.egg-info/top_level.txt
--rw-r--r--   0 ob907      (502) staff       (20)       38 2024-05-13 18:51:29.958588 lfg_llama-2.0.2/setup.cfg
--rw-r--r--   0 ob907      (502) staff       (20)      464 2024-05-13 18:51:26.000000 lfg_llama-2.0.2/setup.py
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-20 18:04:06.711848 lfg_llama-2.1.0/
+-rw-r--r--   0 ob907      (502) staff       (20)     2329 2024-05-20 18:04:06.711636 lfg_llama-2.1.0/PKG-INFO
+-rw-r--r--   0 ob907      (502) staff       (20)     2090 2024-05-20 18:02:28.000000 lfg_llama-2.1.0/README.md
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-20 18:04:06.710467 lfg_llama-2.1.0/lfg/
+-rw-r--r--   0 ob907      (502) staff       (20)        0 2024-04-28 17:51:36.000000 lfg_llama-2.1.0/lfg/__init__.py
+-rwxr-xr-x   0 ob907      (502) staff       (20)     2981 2024-05-20 18:00:32.000000 lfg_llama-2.1.0/lfg/cli.py
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-20 18:04:06.711402 lfg_llama-2.1.0/lfg_llama.egg-info/
+-rw-r--r--   0 ob907      (502) staff       (20)     2329 2024-05-20 18:04:06.000000 lfg_llama-2.1.0/lfg_llama.egg-info/PKG-INFO
+-rw-r--r--   0 ob907      (502) staff       (20)      245 2024-05-20 18:04:06.000000 lfg_llama-2.1.0/lfg_llama.egg-info/SOURCES.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        1 2024-05-20 18:04:06.000000 lfg_llama-2.1.0/lfg_llama.egg-info/dependency_links.txt
+-rw-r--r--   0 ob907      (502) staff       (20)       37 2024-05-20 18:04:06.000000 lfg_llama-2.1.0/lfg_llama.egg-info/entry_points.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        7 2024-05-20 18:04:06.000000 lfg_llama-2.1.0/lfg_llama.egg-info/requires.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        4 2024-05-20 18:04:06.000000 lfg_llama-2.1.0/lfg_llama.egg-info/top_level.txt
+-rw-r--r--   0 ob907      (502) staff       (20)       38 2024-05-20 18:04:06.711905 lfg_llama-2.1.0/setup.cfg
+-rw-r--r--   0 ob907      (502) staff       (20)      464 2024-05-20 18:00:42.000000 lfg_llama-2.1.0/setup.py
```

### Comparing `lfg_llama-2.0.2/PKG-INFO` & `lfg_llama-2.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfg-llama
-Version: 2.0.2
+Version: 2.1.0
 Summary: LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙
 Author: Bjarne Oeverli
 Author-email: bjarneocodes@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: openai
 
 # LFG
@@ -44,50 +44,53 @@
 This executable is using OpenAI, that means you need and [API token](https://platform.openai.com/api-keys).
 
 [GPT-4o](https://platform.openai.com/docs/models/gpt-4o) is free to use.
 
 Add the token to your .bashrc/.zshrc and reload your terminal.
 
 ```
-OPENAI_API_KEY={replace_me}
+export OPENAI_API_KEY={replace_me}
 ```
 
 ```
 $ lfg query
 ```
 
 Now you can use the executable
 
 ```bash
-lfg "kill port 3000"
+fuser -k 3000/tcp
 
-# Kill process listening on port 3000
-lsof -i :3000 | xargs kill
+Explanation:
+The `fuser` command identifies processes using files or sockets. The `-k` option is used to kill th
+ose processes. Here, `3000/tcp` specifies the TCP port number 3000. This command effectively kills
+any process currently using port 3000.
 
 ```
 
 Change the LLM
 
 ```bash
-$ lfg "list ec2 pipe json jq get name" -m llama370b
+$ lfg list ec2 pipe json jq get name
 
-# List EC2 instances with name
+aws ec2 describe-instances --query "Reservations[].Instances[].{Name:Tags[?Key=='Name']|[0].Value}"
+ --output json | jq -r '.[].Name'
 
-aws ec2 describe-instances --query 'Reservations[].Instances[]|{Name:Tags[?Key==`Name`]|[0].Value,I
-nstanceId}' --output text | jq '.[] | {"Name", .Name, "InstanceId", .InstanceId}'
-
-This command uses the AWS CLI to describe EC2 instances, and then pipes the output to `jq` to format the output in a JSON-like format, showing the instance name and ID.
+Explanation:
+This command uses the AWS CLI to list EC2 instances and their corresponding 'Name' tag values in JS
+ON format. The `--query` option filters the output to only include the 'Name' tag for each instance
+, and `jq` is used to parse and extract the 'Name' values.%
 ```
 
 ### Development
 
 ```bash
 pip install --user pipenv
 pipenv --python 3.11
 pipenv install
 
-pipenv run lfg "kill port 3000"
+pipenv run lfg kill port 3000
 ```
 
 ### TODO
 
 - Fix the setup and pyproject file, including github workflow for releasing the package
```

### Comparing `lfg_llama-2.0.2/README.md` & `lfg_llama-2.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -35,50 +35,53 @@
 This executable is using OpenAI, that means you need and [API token](https://platform.openai.com/api-keys).
 
 [GPT-4o](https://platform.openai.com/docs/models/gpt-4o) is free to use.
 
 Add the token to your .bashrc/.zshrc and reload your terminal.
 
 ```
-OPENAI_API_KEY={replace_me}
+export OPENAI_API_KEY={replace_me}
 ```
 
 ```
 $ lfg query
 ```
 
 Now you can use the executable
 
 ```bash
-lfg "kill port 3000"
+fuser -k 3000/tcp
 
-# Kill process listening on port 3000
-lsof -i :3000 | xargs kill
+Explanation:
+The `fuser` command identifies processes using files or sockets. The `-k` option is used to kill th
+ose processes. Here, `3000/tcp` specifies the TCP port number 3000. This command effectively kills
+any process currently using port 3000.
 
 ```
 
 Change the LLM
 
 ```bash
-$ lfg "list ec2 pipe json jq get name" -m llama370b
+$ lfg list ec2 pipe json jq get name
 
-# List EC2 instances with name
+aws ec2 describe-instances --query "Reservations[].Instances[].{Name:Tags[?Key=='Name']|[0].Value}"
+ --output json | jq -r '.[].Name'
 
-aws ec2 describe-instances --query 'Reservations[].Instances[]|{Name:Tags[?Key==`Name`]|[0].Value,I
-nstanceId}' --output text | jq '.[] | {"Name", .Name, "InstanceId", .InstanceId}'
-
-This command uses the AWS CLI to describe EC2 instances, and then pipes the output to `jq` to format the output in a JSON-like format, showing the instance name and ID.
+Explanation:
+This command uses the AWS CLI to list EC2 instances and their corresponding 'Name' tag values in JS
+ON format. The `--query` option filters the output to only include the 'Name' tag for each instance
+, and `jq` is used to parse and extract the 'Name' values.%
 ```
 
 ### Development
 
 ```bash
 pip install --user pipenv
 pipenv --python 3.11
 pipenv install
 
-pipenv run lfg "kill port 3000"
+pipenv run lfg kill port 3000
 ```
 
 ### TODO
 
 - Fix the setup and pyproject file, including github workflow for releasing the package
```

### Comparing `lfg_llama-2.0.2/lfg/cli.py` & `lfg_llama-2.1.0/lfg/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 #!/usr/bin/python3
 
 import os
 import sys
-import argparse
 import openai
 from openai import OpenAI
 from openai.types.chat import ChatCompletion
 
 
 def get_openai_client() -> OpenAI:
     """Retrieves the OpenAI API key and creates a OpenAI client instance.
@@ -71,22 +70,24 @@
         print(e.status_code)
         print(e.response)
 
 
 def main():
     """Initializes the OpenAI client, and processes the query."""
 
-    parser = argparse.ArgumentParser()
-    parser.add_argument("query", type=str, help="The query sent to the LLM")
+    if len(sys.argv) < 2:
+        print("Usage: lfg <query>")
 
-    args = parser.parse_args()
+        sys.exit(1)
+
+    query = " ".join(sys.argv[1:])
 
     try:
         client = get_openai_client()
-        stream = send_chat_query(args.query, client)
+        stream = send_chat_query(query, client)
 
         handle_stream(stream)
     except ValueError as e:
         print(f"Error: {e}")
 
 
 if __name__ == "__main__":
```

### Comparing `lfg_llama-2.0.2/lfg_llama.egg-info/PKG-INFO` & `lfg_llama-2.1.0/lfg_llama.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfg-llama
-Version: 2.0.2
+Version: 2.1.0
 Summary: LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙
 Author: Bjarne Oeverli
 Author-email: bjarneocodes@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: openai
 
 # LFG
@@ -44,50 +44,53 @@
 This executable is using OpenAI, that means you need and [API token](https://platform.openai.com/api-keys).
 
 [GPT-4o](https://platform.openai.com/docs/models/gpt-4o) is free to use.
 
 Add the token to your .bashrc/.zshrc and reload your terminal.
 
 ```
-OPENAI_API_KEY={replace_me}
+export OPENAI_API_KEY={replace_me}
 ```
 
 ```
 $ lfg query
 ```
 
 Now you can use the executable
 
 ```bash
-lfg "kill port 3000"
+fuser -k 3000/tcp
 
-# Kill process listening on port 3000
-lsof -i :3000 | xargs kill
+Explanation:
+The `fuser` command identifies processes using files or sockets. The `-k` option is used to kill th
+ose processes. Here, `3000/tcp` specifies the TCP port number 3000. This command effectively kills
+any process currently using port 3000.
 
 ```
 
 Change the LLM
 
 ```bash
-$ lfg "list ec2 pipe json jq get name" -m llama370b
+$ lfg list ec2 pipe json jq get name
 
-# List EC2 instances with name
+aws ec2 describe-instances --query "Reservations[].Instances[].{Name:Tags[?Key=='Name']|[0].Value}"
+ --output json | jq -r '.[].Name'
 
-aws ec2 describe-instances --query 'Reservations[].Instances[]|{Name:Tags[?Key==`Name`]|[0].Value,I
-nstanceId}' --output text | jq '.[] | {"Name", .Name, "InstanceId", .InstanceId}'
-
-This command uses the AWS CLI to describe EC2 instances, and then pipes the output to `jq` to format the output in a JSON-like format, showing the instance name and ID.
+Explanation:
+This command uses the AWS CLI to list EC2 instances and their corresponding 'Name' tag values in JS
+ON format. The `--query` option filters the output to only include the 'Name' tag for each instance
+, and `jq` is used to parse and extract the 'Name' values.%
 ```
 
 ### Development
 
 ```bash
 pip install --user pipenv
 pipenv --python 3.11
 pipenv install
 
-pipenv run lfg "kill port 3000"
+pipenv run lfg kill port 3000
 ```
 
 ### TODO
 
 - Fix the setup and pyproject file, including github workflow for releasing the package
```

