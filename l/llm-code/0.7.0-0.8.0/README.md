# Comparing `tmp/llm_code-0.7.0.tar.gz` & `tmp/llm_code-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_code-0.7.0.tar", max compression
+gzip compressed data, was "llm_code-0.8.0.tar", max compression
```

## Comparing `llm_code-0.7.0.tar` & `llm_code-0.8.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1070 2023-05-19 17:20:49.716226 llm_code-0.7.0/LICENSE
--rw-r--r--   0        0        0     4800 2024-02-28 23:16:03.362991 llm_code-0.7.0/README.md
--rw-r--r--   0        0        0       75 2023-05-21 03:18:50.955110 llm_code-0.7.0/llm_code/__init__.py
--rw-r--r--   0        0        0     1938 2023-05-23 04:05:15.623074 llm_code-0.7.0/llm_code/db.py
--rw-r--r--   0        0        0     5403 2024-02-29 02:43:53.708061 llm_code-0.7.0/llm_code/llm_code.py
--rw-r--r--   0        0        0     3449 2024-02-29 02:33:39.039788 llm_code-0.7.0/llm_code/templates.py
--rw-r--r--   0        0        0      161 2023-05-21 02:14:00.117237 llm_code-0.7.0/prompts/coding/system.toml
--rw-r--r--   0        0        0      760 2024-02-29 02:20:20.760611 llm_code-0.7.0/prompts/coding/user/input.toml
--rw-r--r--   0        0        0      396 2023-05-21 02:14:00.117693 llm_code-0.7.0/prompts/coding/user/simple.toml
--rw-r--r--   0        0        0     1252 2024-02-29 02:50:02.095651 llm_code-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     5871 1970-01-01 00:00:00.000000 llm_code-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-19 17:20:49.716226 llm_code-0.8.0/LICENSE
+-rw-r--r--   0        0        0     4800 2024-02-28 23:16:03.362991 llm_code-0.8.0/README.md
+-rw-r--r--   0        0        0       75 2023-05-21 03:18:50.955110 llm_code-0.8.0/llm_code/__init__.py
+-rw-r--r--   0        0        0     1938 2023-05-23 04:05:15.623074 llm_code-0.8.0/llm_code/db.py
+-rw-r--r--   0        0        0     5396 2024-05-20 04:55:24.272183 llm_code-0.8.0/llm_code/llm_code.py
+-rw-r--r--   0        0        0     3449 2024-02-29 02:33:39.039788 llm_code-0.8.0/llm_code/templates.py
+-rw-r--r--   0        0        0      161 2023-05-21 02:14:00.117237 llm_code-0.8.0/prompts/coding/system.toml
+-rw-r--r--   0        0        0      760 2024-02-29 02:20:20.760611 llm_code-0.8.0/prompts/coding/user/input.toml
+-rw-r--r--   0        0        0      396 2023-05-21 02:14:00.117693 llm_code-0.8.0/prompts/coding/user/simple.toml
+-rw-r--r--   0        0        0     1252 2024-05-20 04:59:41.207146 llm_code-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     5871 1970-01-01 00:00:00.000000 llm_code-0.8.0/PKG-INFO
```

### Comparing `llm_code-0.7.0/LICENSE` & `llm_code-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_code-0.7.0/README.md` & `llm_code-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `llm_code-0.7.0/llm_code/db.py` & `llm_code-0.8.0/llm_code/db.py`

 * *Files identical despite different names*

### Comparing `llm_code-0.7.0/llm_code/llm_code.py` & `llm_code-0.8.0/llm_code/llm_code.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 
 from llm_code import __version__, db
 from llm_code.templates import Message, TemplateLibrary
 
 
 class Settings(BaseSettings):
     openai_api_key: str = ""
-    model: str = "gpt-3.5-turbo"
-    temperature: float = 0.8
+    model: str = "gpt-4o"
+    temperature: float = 0.2
     max_tokens: int = 1000
     config_dir: Path = Path("~/.llm_code").expanduser()
 
     class Config:
         env_file = Path("~/.llm_code").expanduser() / "env"
         env_file_encoding = "utf-8"
```

### Comparing `llm_code-0.7.0/llm_code/templates.py` & `llm_code-0.8.0/llm_code/templates.py`

 * *Files identical despite different names*

### Comparing `llm_code-0.7.0/prompts/coding/user/input.toml` & `llm_code-0.8.0/prompts/coding/user/input.toml`

 * *Files identical despite different names*

### Comparing `llm_code-0.7.0/pyproject.toml` & `llm_code-0.8.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llm-code"
-version = "0.7.0"
+version = "0.8.0"
 description = "An OpenAI LLM based CLI coding assistant."
 authors = ["Rushabh Doshi <radoshi+pypi@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "llm_code" }]
 homepage = "https://github.com/radoshi/llm-code"
 repository = "https://github.com/radoshi/llm-code"
```

### Comparing `llm_code-0.7.0/PKG-INFO` & `llm_code-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-code
-Version: 0.7.0
+Version: 0.8.0
 Summary: An OpenAI LLM based CLI coding assistant.
 Home-page: https://github.com/radoshi/llm-code
 License: MIT
 Keywords: openai,llm,cli,coding,assistant
 Author: Rushabh Doshi
 Author-email: radoshi+pypi@gmail.com
 Requires-Python: >=3.11,<4.0
```

