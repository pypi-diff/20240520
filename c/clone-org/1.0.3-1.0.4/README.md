# Comparing `tmp/clone_org-1.0.3.tar.gz` & `tmp/clone_org-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clone_org-1.0.3.tar", max compression
+gzip compressed data, was "clone_org-1.0.4.tar", max compression
```

## Comparing `clone_org-1.0.3.tar` & `clone_org-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    11357 2023-04-30 23:19:16.107692 clone_org-1.0.3/LICENSE.txt
--rw-r--r--   0        0        0     3965 2023-04-30 23:19:16.107944 clone_org-1.0.3/README.md
--rw-r--r--   0        0        0        0 2024-02-24 13:30:41.750276 clone_org-1.0.3/clone_org/__init__.py
--rw-r--r--   0        0        0        0 2024-02-24 13:30:41.750408 clone_org-1.0.3/clone_org/arg_parsing/__init__.py
--rw-r--r--   0        0        0     4955 2024-02-24 13:30:41.750772 clone_org-1.0.3/clone_org/arg_parsing/parse_cmd_line.py
--rw-r--r--   0        0        0        0 2024-02-24 13:30:41.750862 clone_org-1.0.3/clone_org/clone/__init__.py
--rw-r--r--   0        0        0      531 2024-02-24 13:30:41.751063 clone_org-1.0.3/clone_org/clone/shell_clone.py
--rw-r--r--   0        0        0      657 2024-02-24 13:30:41.751222 clone_org-1.0.3/clone_org/main.py
--rw-r--r--   0        0        0      386 2024-02-24 13:30:41.751400 clone_org-1.0.3/clone_org/query_github/.graphqlconfig
--rw-r--r--   0        0        0     2463 2024-02-24 13:30:41.751581 clone_org-1.0.3/clone_org/query_github/README.rst
--rw-r--r--   0        0        0        0 2024-02-24 13:30:41.751647 clone_org-1.0.3/clone_org/query_github/__init__.py
--rw-r--r--   0        0        0     4666 2024-02-24 13:30:41.752099 clone_org-1.0.3/clone_org/query_github/fetch_org_repos.py
--rw-r--r--   0        0        0   498734 2024-02-24 13:30:41.754232 clone_org-1.0.3/clone_org/query_github/github-schema.graphql
--rw-r--r--   0        0        0      119 2024-02-24 13:30:41.754635 clone_org-1.0.3/clone_org/query_github/org-repos-count.graphql
--rw-r--r--   0        0        0      412 2024-02-24 13:30:41.754830 clone_org-1.0.3/clone_org/query_github/org-repos.graphql
--rw-r--r--   0        0        0        0 2024-02-24 13:30:41.754916 clone_org-1.0.3/clone_org/utils/__init__.py
--rw-r--r--   0        0        0     1072 2024-02-24 13:30:41.755131 clone_org-1.0.3/clone_org/utils/check_dict.py
--rw-r--r--   0        0        0      703 2024-02-24 13:47:17.448545 clone_org-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     4738 1970-01-01 00:00:00.000000 clone_org-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-02-15 21:09:06.456400 clone_org-1.0.4/LICENSE.txt
+-rw-r--r--   0        0        0     4127 2024-05-19 22:40:19.204924 clone_org-1.0.4/README.md
+-rw-r--r--   0        0        0        0 2024-02-15 21:09:06.456400 clone_org-1.0.4/clone_org/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-15 21:09:06.456400 clone_org-1.0.4/clone_org/arg_parsing/__init__.py
+-rw-r--r--   0        0        0     4955 2024-02-17 15:28:57.462137 clone_org-1.0.4/clone_org/arg_parsing/parse_cmd_line.py
+-rw-r--r--   0        0        0        0 2024-02-15 21:09:06.456400 clone_org-1.0.4/clone_org/clone/__init__.py
+-rw-r--r--   0        0        0      531 2024-02-15 21:09:06.456400 clone_org-1.0.4/clone_org/clone/shell_clone.py
+-rw-r--r--   0        0        0      657 2024-02-15 21:09:06.456400 clone_org-1.0.4/clone_org/main.py
+-rw-r--r--   0        0        0      386 2024-02-15 21:09:06.456400 clone_org-1.0.4/clone_org/query_github/.graphqlconfig
+-rw-r--r--   0        0        0     2463 2024-02-15 21:09:06.456400 clone_org-1.0.4/clone_org/query_github/README.rst
+-rw-r--r--   0        0        0        0 2024-02-15 21:09:06.456400 clone_org-1.0.4/clone_org/query_github/__init__.py
+-rw-r--r--   0        0        0     4666 2024-02-15 21:09:06.456400 clone_org-1.0.4/clone_org/query_github/fetch_org_repos.py
+-rw-r--r--   0        0        0   498734 2024-02-15 21:09:06.456400 clone_org-1.0.4/clone_org/query_github/github-schema.graphql
+-rw-r--r--   0        0        0      119 2024-02-15 21:09:06.456400 clone_org-1.0.4/clone_org/query_github/org-repos-count.graphql
+-rw-r--r--   0        0        0      412 2024-02-15 21:09:06.456400 clone_org-1.0.4/clone_org/query_github/org-repos.graphql
+-rw-r--r--   0        0        0        0 2024-02-15 21:09:06.456400 clone_org-1.0.4/clone_org/utils/__init__.py
+-rw-r--r--   0        0        0     1072 2024-02-15 21:09:06.456400 clone_org-1.0.4/clone_org/utils/check_dict.py
+-rw-r--r--   0        0        0      721 2024-05-19 22:40:19.204924 clone_org-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4969 1970-01-01 00:00:00.000000 clone_org-1.0.4/PKG-INFO
```

### Comparing `clone_org-1.0.3/LICENSE.txt` & `clone_org-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `clone_org-1.0.3/README.md` & `clone_org-1.0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # Clone GitHub namespace
 
 ## Clone an organization's repos.
 
-Clone an organization's repos. A common situation that folks find themselves
+Clone an organization's repos. Clone all repos in an organization or some by 
+language used. 
+```shell
+    $ clone-org -o kubernetes-client -p https -f ~/dev/kub-client-repos -l python,go
+```
+
+A common situation that folks find themselves
 in when starting to work with an organization is the ability to check out all
 the code and essentially familiarize themselves with the code base and even
 grep the code base looking for things. clone-org is designed to lessen
 the pain and give you a one-stop clone the organization toolkit. This module
 queries the GitHub graphql endpoint.
 
 Clone-org uses the installed version of git on your machine and executes shell
```

### Comparing `clone_org-1.0.3/clone_org/arg_parsing/parse_cmd_line.py` & `clone_org-1.0.4/clone_org/arg_parsing/parse_cmd_line.py`

 * *Files identical despite different names*

### Comparing `clone_org-1.0.3/clone_org/clone/shell_clone.py` & `clone_org-1.0.4/clone_org/clone/shell_clone.py`

 * *Files identical despite different names*

### Comparing `clone_org-1.0.3/clone_org/main.py` & `clone_org-1.0.4/clone_org/main.py`

 * *Files identical despite different names*

### Comparing `clone_org-1.0.3/clone_org/query_github/README.rst` & `clone_org-1.0.4/clone_org/query_github/README.rst`

 * *Files identical despite different names*

### Comparing `clone_org-1.0.3/clone_org/query_github/fetch_org_repos.py` & `clone_org-1.0.4/clone_org/query_github/fetch_org_repos.py`

 * *Files identical despite different names*

### Comparing `clone_org-1.0.3/clone_org/query_github/github-schema.graphql` & `clone_org-1.0.4/clone_org/query_github/github-schema.graphql`

 * *Files identical despite different names*

### Comparing `clone_org-1.0.3/clone_org/utils/check_dict.py` & `clone_org-1.0.4/clone_org/utils/check_dict.py`

 * *Files identical despite different names*

### Comparing `clone_org-1.0.3/pyproject.toml` & `clone_org-1.0.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "clone-org"
-version = "1.0.3"
-description = "Clone all repos from a GitHub organization"
+version = "1.0.4"
+description = "Clone repos from an organization by languge used in the repo"
 authors = ["Glenn Hinks <ghinks@yahoo.com>"]
 license = "Apache License 2.0"
 readme = "README.md"
 packages = [{include = "clone_org"}]
 repository = "https://github.com/ghinks/clone-org"  # Add your GitHub repository URL here
 homepage = "https://github.com/ghinks/clone-org"  # Add your project homepage URL here
```

### Comparing `clone_org-1.0.3/PKG-INFO` & `clone_org-1.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 Metadata-Version: 2.1
 Name: clone-org
-Version: 1.0.3
-Summary: Clone all repos from a GitHub organization
+Version: 1.0.4
+Summary: Clone repos from an organization by languge used in the repo
 Home-page: https://github.com/ghinks/clone-org
 License: Apache-2.0
 Author: Glenn Hinks
 Author-email: ghinks@yahoo.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: flake8 (>=6.1,<8.0)
 Requires-Dist: pytest (>=7.4.3,<9.0.0)
 Requires-Dist: sgqlc (>=16.3,<17.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://github.com/ghinks/clone-org
 Description-Content-Type: text/markdown
 
 # Clone GitHub namespace
 
 ## Clone an organization's repos.
 
-Clone an organization's repos. A common situation that folks find themselves
+Clone an organization's repos. Clone all repos in an organization or some by 
+language used. 
+```shell
+    $ clone-org -o kubernetes-client -p https -f ~/dev/kub-client-repos -l python,go
+```
+
+A common situation that folks find themselves
 in when starting to work with an organization is the ability to check out all
 the code and essentially familiarize themselves with the code base and even
 grep the code base looking for things. clone-org is designed to lessen
 the pain and give you a one-stop clone the organization toolkit. This module
 queries the GitHub graphql endpoint.
 
 Clone-org uses the installed version of git on your machine and executes shell
```

