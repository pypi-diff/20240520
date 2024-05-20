# Comparing `tmp/alita_sdk-0.1.7.tar.gz` & `tmp/alita_sdk-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alita_sdk-0.1.7.tar", last modified: Thu May 16 11:43:14 2024, max compression
+gzip compressed data, was "alita_sdk-0.1.8.tar", last modified: Mon May 20 06:53:15 2024, max compression
```

## Comparing `alita_sdk-0.1.7.tar` & `alita_sdk-0.1.8.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-16 11:43:14.303975 alita_sdk-0.1.7/
--rw-r--r--   0 arozumenko   (501) staff       (20)    11357 2024-03-08 11:24:37.000000 alita_sdk-0.1.7/LICENSE
--rw-r--r--   0 arozumenko   (501) staff       (20)     4063 2024-05-16 11:43:14.303714 alita_sdk-0.1.7/PKG-INFO
--rw-r--r--   0 arozumenko   (501) staff       (20)     3200 2024-03-10 12:01:09.000000 alita_sdk-0.1.7/README.md
--rw-r--r--   0 arozumenko   (501) staff       (20)      705 2024-05-16 11:43:11.000000 alita_sdk-0.1.7/pyproject.toml
--rw-r--r--   0 arozumenko   (501) staff       (20)      175 2024-05-08 13:44:16.000000 alita_sdk-0.1.7/requirements.txt
--rw-r--r--   0 arozumenko   (501) staff       (20)       38 2024-05-16 11:43:14.304037 alita_sdk-0.1.7/setup.cfg
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-16 11:43:14.295579 alita_sdk-0.1.7/src/
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-08 11:25:38.000000 alita_sdk-0.1.7/src/__init__.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-16 11:43:14.295672 alita_sdk-0.1.7/src/alita_sdk/
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-08 11:25:50.000000 alita_sdk-0.1.7/src/alita_sdk/__init__.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-16 11:43:14.299044 alita_sdk-0.1.7/src/alita_sdk/agents/
--rw-r--r--   0 arozumenko   (501) staff       (20)     2412 2024-03-18 10:31:52.000000 alita_sdk-0.1.7/src/alita_sdk/agents/__init__.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     3122 2024-04-30 17:52:10.000000 alita_sdk-0.1.7/src/alita_sdk/agents/alita_openai.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     3135 2024-05-16 11:42:35.000000 alita_sdk-0.1.7/src/alita_sdk/agents/mixedAgentParser.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     2380 2024-05-09 09:15:40.000000 alita_sdk-0.1.7/src/alita_sdk/agents/mixedAgentRenderes.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     1151 2024-05-16 11:35:26.000000 alita_sdk-0.1.7/src/alita_sdk/agents/utils.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-16 11:43:14.299819 alita_sdk-0.1.7/src/alita_sdk/clients/
--rw-r--r--   0 arozumenko   (501) staff       (20)       31 2024-03-09 15:53:40.000000 alita_sdk-0.1.7/src/alita_sdk/clients/__init__.py
--rw-r--r--   0 arozumenko   (501) staff       (20)    21757 2024-05-08 13:31:09.000000 alita_sdk-0.1.7/src/alita_sdk/clients/client.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-16 11:43:14.300124 alita_sdk-0.1.7/src/alita_sdk/llms/
--rw-r--r--   0 arozumenko   (501) staff       (20)       33 2024-03-09 14:45:23.000000 alita_sdk-0.1.7/src/alita_sdk/llms/__init__.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     8851 2024-05-02 10:28:32.000000 alita_sdk-0.1.7/src/alita_sdk/llms/alita.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-16 11:43:14.300657 alita_sdk-0.1.7/src/alita_sdk/toolkits/
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-04-12 11:47:05.000000 alita_sdk-0.1.7/src/alita_sdk/toolkits/__init__.py
--rw-r--r--   0 arozumenko   (501) staff       (20)      798 2024-05-08 13:59:31.000000 alita_sdk-0.1.7/src/alita_sdk/toolkits/application.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     1985 2024-04-12 12:00:03.000000 alita_sdk-0.1.7/src/alita_sdk/toolkits/datasource.py
--rw-r--r--   0 arozumenko   (501) staff       (20)      734 2024-04-12 11:47:16.000000 alita_sdk-0.1.7/src/alita_sdk/toolkits/prompt.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-16 11:43:14.301104 alita_sdk-0.1.7/src/alita_sdk/tools/
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-11 07:45:42.000000 alita_sdk-0.1.7/src/alita_sdk/tools/__init__.py
--rw-r--r--   0 arozumenko   (501) staff       (20)      530 2024-05-08 13:59:34.000000 alita_sdk-0.1.7/src/alita_sdk/tools/application.py
--rw-r--r--   0 arozumenko   (501) staff       (20)      743 2024-04-12 14:28:55.000000 alita_sdk-0.1.7/src/alita_sdk/tools/datasource.py
--rw-r--r--   0 arozumenko   (501) staff       (20)      281 2024-05-14 06:19:04.000000 alita_sdk-0.1.7/src/alita_sdk/tools/prompt.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-16 11:43:14.301318 alita_sdk-0.1.7/src/alita_sdk/utils/
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-13 15:14:37.000000 alita_sdk-0.1.7/src/alita_sdk/utils/__init__.py
--rw-r--r--   0 arozumenko   (501) staff       (20)    10148 2024-04-04 04:14:44.000000 alita_sdk-0.1.7/src/alita_sdk/utils/streamlit.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-16 11:43:14.303341 alita_sdk-0.1.7/src/alita_sdk.egg-info/
--rw-r--r--   0 arozumenko   (501) staff       (20)     4063 2024-05-16 11:43:14.000000 alita_sdk-0.1.7/src/alita_sdk.egg-info/PKG-INFO
--rw-r--r--   0 arozumenko   (501) staff       (20)      923 2024-05-16 11:43:14.000000 alita_sdk-0.1.7/src/alita_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 arozumenko   (501) staff       (20)        1 2024-05-16 11:43:14.000000 alita_sdk-0.1.7/src/alita_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 arozumenko   (501) staff       (20)      176 2024-05-16 11:43:14.000000 alita_sdk-0.1.7/src/alita_sdk.egg-info/requires.txt
--rw-r--r--   0 arozumenko   (501) staff       (20)       19 2024-05-16 11:43:14.000000 alita_sdk-0.1.7/src/alita_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-20 06:53:15.563035 alita_sdk-0.1.8/
+-rw-r--r--   0 arozumenko   (501) staff       (20)    11357 2024-03-08 11:24:37.000000 alita_sdk-0.1.8/LICENSE
+-rw-r--r--   0 arozumenko   (501) staff       (20)     4063 2024-05-20 06:53:15.562800 alita_sdk-0.1.8/PKG-INFO
+-rw-r--r--   0 arozumenko   (501) staff       (20)     3200 2024-03-10 12:01:09.000000 alita_sdk-0.1.8/README.md
+-rw-r--r--   0 arozumenko   (501) staff       (20)      705 2024-05-20 06:53:10.000000 alita_sdk-0.1.8/pyproject.toml
+-rw-r--r--   0 arozumenko   (501) staff       (20)      175 2024-05-08 13:44:16.000000 alita_sdk-0.1.8/requirements.txt
+-rw-r--r--   0 arozumenko   (501) staff       (20)       38 2024-05-20 06:53:15.563084 alita_sdk-0.1.8/setup.cfg
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-20 06:53:15.558320 alita_sdk-0.1.8/src/
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-08 11:25:38.000000 alita_sdk-0.1.8/src/__init__.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-20 06:53:15.558419 alita_sdk-0.1.8/src/alita_sdk/
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-08 11:25:50.000000 alita_sdk-0.1.8/src/alita_sdk/__init__.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-20 06:53:15.559883 alita_sdk-0.1.8/src/alita_sdk/agents/
+-rw-r--r--   0 arozumenko   (501) staff       (20)     2412 2024-03-18 10:31:52.000000 alita_sdk-0.1.8/src/alita_sdk/agents/__init__.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     3122 2024-04-30 17:52:10.000000 alita_sdk-0.1.8/src/alita_sdk/agents/alita_openai.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     3135 2024-05-16 11:42:35.000000 alita_sdk-0.1.8/src/alita_sdk/agents/mixedAgentParser.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     2380 2024-05-09 09:15:40.000000 alita_sdk-0.1.8/src/alita_sdk/agents/mixedAgentRenderes.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     1151 2024-05-16 11:35:26.000000 alita_sdk-0.1.8/src/alita_sdk/agents/utils.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-20 06:53:15.560287 alita_sdk-0.1.8/src/alita_sdk/clients/
+-rw-r--r--   0 arozumenko   (501) staff       (20)       31 2024-03-09 15:53:40.000000 alita_sdk-0.1.8/src/alita_sdk/clients/__init__.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)    21902 2024-05-20 06:52:53.000000 alita_sdk-0.1.8/src/alita_sdk/clients/client.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-20 06:53:15.560825 alita_sdk-0.1.8/src/alita_sdk/llms/
+-rw-r--r--   0 arozumenko   (501) staff       (20)       33 2024-03-09 14:45:23.000000 alita_sdk-0.1.8/src/alita_sdk/llms/__init__.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     8851 2024-05-02 10:28:32.000000 alita_sdk-0.1.8/src/alita_sdk/llms/alita.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-20 06:53:15.561405 alita_sdk-0.1.8/src/alita_sdk/toolkits/
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-04-12 11:47:05.000000 alita_sdk-0.1.8/src/alita_sdk/toolkits/__init__.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)      798 2024-05-08 13:59:31.000000 alita_sdk-0.1.8/src/alita_sdk/toolkits/application.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     1985 2024-04-12 12:00:03.000000 alita_sdk-0.1.8/src/alita_sdk/toolkits/datasource.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)      734 2024-04-12 11:47:16.000000 alita_sdk-0.1.8/src/alita_sdk/toolkits/prompt.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-20 06:53:15.561957 alita_sdk-0.1.8/src/alita_sdk/tools/
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-11 07:45:42.000000 alita_sdk-0.1.8/src/alita_sdk/tools/__init__.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)      530 2024-05-08 13:59:34.000000 alita_sdk-0.1.8/src/alita_sdk/tools/application.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)      743 2024-04-12 14:28:55.000000 alita_sdk-0.1.8/src/alita_sdk/tools/datasource.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)      281 2024-05-14 06:19:04.000000 alita_sdk-0.1.8/src/alita_sdk/tools/prompt.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-20 06:53:15.562181 alita_sdk-0.1.8/src/alita_sdk/utils/
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-13 15:14:37.000000 alita_sdk-0.1.8/src/alita_sdk/utils/__init__.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)    10148 2024-04-04 04:14:44.000000 alita_sdk-0.1.8/src/alita_sdk/utils/streamlit.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-20 06:53:15.562518 alita_sdk-0.1.8/src/alita_sdk.egg-info/
+-rw-r--r--   0 arozumenko   (501) staff       (20)     4063 2024-05-20 06:53:15.000000 alita_sdk-0.1.8/src/alita_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 arozumenko   (501) staff       (20)      923 2024-05-20 06:53:15.000000 alita_sdk-0.1.8/src/alita_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 arozumenko   (501) staff       (20)        1 2024-05-20 06:53:15.000000 alita_sdk-0.1.8/src/alita_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 arozumenko   (501) staff       (20)      176 2024-05-20 06:53:15.000000 alita_sdk-0.1.8/src/alita_sdk.egg-info/requires.txt
+-rw-r--r--   0 arozumenko   (501) staff       (20)       19 2024-05-20 06:53:15.000000 alita_sdk-0.1.8/src/alita_sdk.egg-info/top_level.txt
```

### Comparing `alita_sdk-0.1.7/LICENSE` & `alita_sdk-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.7/PKG-INFO` & `alita_sdk-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alita_sdk
-Version: 0.1.7
+Version: 0.1.8
 Summary: SDK for building langchain agents using resouces from Alita
 Author-email: Artem Rozumenko <support@analysta.ai>
 Project-URL: Homepage, https://projectalita.ai
 Project-URL: Issues, https://github.com/ProjectAlita/alita-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `alita_sdk-0.1.7/README.md` & `alita_sdk-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.7/pyproject.toml` & `alita_sdk-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alita_sdk"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   { name="Artem Rozumenko", email="support@analysta.ai" },
 ]
 description = "SDK for building langchain agents using resouces from Alita"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `alita_sdk-0.1.7/src/alita_sdk/agents/__init__.py` & `alita_sdk-0.1.8/src/alita_sdk/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.7/src/alita_sdk/agents/alita_openai.py` & `alita_sdk-0.1.8/src/alita_sdk/agents/alita_openai.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.7/src/alita_sdk/agents/mixedAgentParser.py` & `alita_sdk-0.1.8/src/alita_sdk/agents/mixedAgentParser.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.7/src/alita_sdk/agents/mixedAgentRenderes.py` & `alita_sdk-0.1.8/src/alita_sdk/agents/mixedAgentRenderes.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.7/src/alita_sdk/agents/utils.py` & `alita_sdk-0.1.8/src/alita_sdk/agents/utils.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.7/src/alita_sdk/clients/client.py` & `alita_sdk-0.1.8/src/alita_sdk/clients/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,15 +274,17 @@
                 ).get_tools())
             elif tool['type'] == 'github':
                 github_toolkit = AlitaGitHubToolkit().get_toolkit(
                     selected_tools=tool['settings'].get('selected_tools', []),
                     github_repository=tool['settings']['repository'],
                     active_branch=tool['settings']['active_branch'],
                     github_base_branch=tool['settings']['base_branch'],
-                    github_access_token=tool['settings'].get('access_token', None),
+                    github_access_token=tool['settings'].get('access_token', ''),
+                    github_username=tool['settings'].get('username', ''),
+                    github_password=tool['settings'].get('password', '')
                 )
                 tools.extend(github_toolkit.get_tools())
             elif tool['type'] == 'jira':
                 jira_tools = JiraToolkit().get_toolkit(
                     selected_tools=tool['settings'].get('selected_tools', []),
                     base_url=tool['settings']['base_url'], 
                     cloud=tool['settings'].get('cloud', True),
```

### Comparing `alita_sdk-0.1.7/src/alita_sdk/llms/alita.py` & `alita_sdk-0.1.8/src/alita_sdk/llms/alita.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.7/src/alita_sdk/toolkits/application.py` & `alita_sdk-0.1.8/src/alita_sdk/toolkits/application.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.7/src/alita_sdk/toolkits/datasource.py` & `alita_sdk-0.1.8/src/alita_sdk/toolkits/datasource.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.7/src/alita_sdk/toolkits/prompt.py` & `alita_sdk-0.1.8/src/alita_sdk/toolkits/prompt.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.7/src/alita_sdk/tools/application.py` & `alita_sdk-0.1.8/src/alita_sdk/tools/application.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.7/src/alita_sdk/tools/datasource.py` & `alita_sdk-0.1.8/src/alita_sdk/tools/datasource.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.7/src/alita_sdk/utils/streamlit.py` & `alita_sdk-0.1.8/src/alita_sdk/utils/streamlit.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.7/src/alita_sdk.egg-info/PKG-INFO` & `alita_sdk-0.1.8/src/alita_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alita_sdk
-Version: 0.1.7
+Version: 0.1.8
 Summary: SDK for building langchain agents using resouces from Alita
 Author-email: Artem Rozumenko <support@analysta.ai>
 Project-URL: Homepage, https://projectalita.ai
 Project-URL: Issues, https://github.com/ProjectAlita/alita-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `alita_sdk-0.1.7/src/alita_sdk.egg-info/SOURCES.txt` & `alita_sdk-0.1.8/src/alita_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

