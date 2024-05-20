# Comparing `tmp/funkai-1.0.tar.gz` & `tmp/funkai-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funkai-1.0.tar", last modified: Thu May 16 04:42:27 2024, max compression
+gzip compressed data, was "funkai-1.1.tar", last modified: Mon May 20 06:37:58 2024, max compression
```

## Comparing `funkai-1.0.tar` & `funkai-1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 sameer     (502) staff       (20)        0 2024-05-16 04:42:27.339614 funkai-1.0/
--rw-r--r--   0 sameer     (502) staff       (20)     4901 2024-05-16 04:42:27.339399 funkai-1.0/PKG-INFO
--rw-r--r--   0 sameer     (502) staff       (20)     4486 2024-05-14 06:00:28.000000 funkai-1.0/README.md
-drwxr-xr-x   0 sameer     (502) staff       (20)        0 2024-05-16 04:42:27.338410 funkai-1.0/funkai/
--rw-r--r--   0 sameer     (502) staff       (20)       61 2024-05-14 06:00:28.000000 funkai-1.0/funkai/__init__.py
--rw-r--r--   0 sameer     (502) staff       (20)      199 2024-05-14 06:00:28.000000 funkai-1.0/funkai/claude.py
--rw-r--r--   0 sameer     (502) staff       (20)    10838 2024-03-01 12:09:36.000000 funkai-1.0/funkai/examples.py
--rw-r--r--   0 sameer     (502) staff       (20)     6471 2024-05-14 06:00:28.000000 funkai-1.0/funkai/funk.py
--rw-r--r--   0 sameer     (502) staff       (20)     1639 2024-05-14 06:00:28.000000 funkai-1.0/funkai/manager.py
--rw-r--r--   0 sameer     (502) staff       (20)      190 2024-05-14 06:00:28.000000 funkai-1.0/funkai/openai.py
-drwxr-xr-x   0 sameer     (502) staff       (20)        0 2024-05-16 04:42:27.339108 funkai-1.0/funkai.egg-info/
--rw-r--r--   0 sameer     (502) staff       (20)     4901 2024-05-16 04:42:27.000000 funkai-1.0/funkai.egg-info/PKG-INFO
--rw-r--r--   0 sameer     (502) staff       (20)      272 2024-05-16 04:42:27.000000 funkai-1.0/funkai.egg-info/SOURCES.txt
--rw-r--r--   0 sameer     (502) staff       (20)        1 2024-05-16 04:42:27.000000 funkai-1.0/funkai.egg-info/dependency_links.txt
--rw-r--r--   0 sameer     (502) staff       (20)       27 2024-05-16 04:42:27.000000 funkai-1.0/funkai.egg-info/requires.txt
--rw-r--r--   0 sameer     (502) staff       (20)        7 2024-05-16 04:42:27.000000 funkai-1.0/funkai.egg-info/top_level.txt
--rw-r--r--   0 sameer     (502) staff       (20)       38 2024-05-16 04:42:27.339661 funkai-1.0/setup.cfg
--rw-r--r--   0 sameer     (502) staff       (20)      570 2024-05-16 04:42:20.000000 funkai-1.0/setup.py
+drwxr-xr-x   0 sameer     (502) staff       (20)        0 2024-05-20 06:37:58.019744 funkai-1.1/
+-rw-r--r--   0 sameer     (502) staff       (20)     5349 2024-05-20 06:37:58.019513 funkai-1.1/PKG-INFO
+-rw-r--r--   0 sameer     (502) staff       (20)     4911 2024-05-20 06:34:38.000000 funkai-1.1/README.md
+drwxr-xr-x   0 sameer     (502) staff       (20)        0 2024-05-20 06:37:58.018181 funkai-1.1/funkai/
+-rw-r--r--   0 sameer     (502) staff       (20)       61 2024-05-14 06:00:28.000000 funkai-1.1/funkai/__init__.py
+-rw-r--r--   0 sameer     (502) staff       (20)      199 2024-05-14 06:00:28.000000 funkai-1.1/funkai/claude.py
+-rw-r--r--   0 sameer     (502) staff       (20)    10838 2024-03-01 12:09:36.000000 funkai-1.1/funkai/examples.py
+-rw-r--r--   0 sameer     (502) staff       (20)     6471 2024-05-14 06:00:28.000000 funkai-1.1/funkai/funk.py
+-rw-r--r--   0 sameer     (502) staff       (20)     1639 2024-05-14 06:00:28.000000 funkai-1.1/funkai/manager.py
+-rw-r--r--   0 sameer     (502) staff       (20)      190 2024-05-14 06:00:28.000000 funkai-1.1/funkai/openai.py
+drwxr-xr-x   0 sameer     (502) staff       (20)        0 2024-05-20 06:37:58.019092 funkai-1.1/funkai.egg-info/
+-rw-r--r--   0 sameer     (502) staff       (20)     5349 2024-05-20 06:37:57.000000 funkai-1.1/funkai.egg-info/PKG-INFO
+-rw-r--r--   0 sameer     (502) staff       (20)      272 2024-05-20 06:37:57.000000 funkai-1.1/funkai.egg-info/SOURCES.txt
+-rw-r--r--   0 sameer     (502) staff       (20)        1 2024-05-20 06:37:57.000000 funkai-1.1/funkai.egg-info/dependency_links.txt
+-rw-r--r--   0 sameer     (502) staff       (20)       27 2024-05-20 06:37:57.000000 funkai-1.1/funkai.egg-info/requires.txt
+-rw-r--r--   0 sameer     (502) staff       (20)        7 2024-05-20 06:37:57.000000 funkai-1.1/funkai.egg-info/top_level.txt
+-rw-r--r--   0 sameer     (502) staff       (20)       38 2024-05-20 06:37:58.019797 funkai-1.1/setup.cfg
+-rw-r--r--   0 sameer     (502) staff       (20)      593 2024-05-20 06:35:47.000000 funkai-1.1/setup.py
```

### Comparing `funkai-1.0/PKG-INFO` & `funkai-1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,15 @@
-Metadata-Version: 2.1
-Name: funkai
-Version: 1.0
-Summary: Easily create and deploy placeholder functions powered by OpenAI for rapid prototyping, diverse linguistic tasks, and quick insights.
-Home-page: https://github.com/ciaraadkins/funkai
-Author: Ciara Adkins
-Author-email: adkins.ciara@gmail.com.com
-Description-Content-Type: text/markdown
-Requires-Dist: openai
-Requires-Dist: llmonitor
-Requires-Dist: anthropic
-
 # Funkai Library
 
-Funkai is a Python library that encapsulates linguistic operations and uses OpenAI to perform them based on user inputs.
+Funkai is a Python library that encapsulates linguistic operations and uses OpenAI or Claude to perform them based on user inputs.
 
 ## Features
 
 - Diverse Operations: Easily define linguistic tasks that can process various data types.
-- Interaction with OpenAI: Seamlessly connect and utilize the OpenAI API to run operations.
+- Interaction with LLM: Seamlessly connect and utilize the LLM (OpenAI or Claude) API to run operations.
 - Dynamic Management: Add, remove, and run operations on-the-fly with the FunkManager.
 
 ## Funkai Setup
 
 Install via pip:
 
 ```python
@@ -33,51 +21,63 @@
 ```python
 git clone https://github.com/ciaraadkins/funkai.git
 pip install ./funkai/
 ```
 
 Once installed, import the necessary modules:
 
-```python
-from funkai import FunkManager
-```
-
 ## OpenAI Setup
 
 For the OpenAI functionality to work, you need to set up your OpenAI API key with init of FunkManager
 
 ```python
-funk = FunkManager(
+from funkai import OpenAIFunk
+
+funk = OpenAIFunk(
         model="gpt-4-turbo-preview",
         api_key='OPEN_API_KEY'
     )
 ```
 
 Additionally, if you want to monitor your llm usage, we recommend using llmonitor (you will need to also set up an account and get an app id on [llmonitor.com](https://llmonitor.com/)):
 
 ```python
 pip install openai llmonitor
 os.environ["LLMONITOR_APP_ID"] = "YOUR_LLMONITOR_APP_ID"
 ```
 
+## Claude Setup
+
+For the Claude functionality to work, you need to set up your Claude API key with init of FunkManager
+
+```python
+from funkai import ClaudeFunk
+
+funk = ClaudeFunk(
+        model="claude-3-opus-20240229",
+        api_key='CLAUDE_API_KEY'
+    )
+```
+
 # Methods
 
-###### `add(name, operation, api_key=None, model=None, retry_count=0, input_dtype=str, output_dtype=str)`
+###### `add(name, operation, api_key=None, model=None, retry_count=0, input_dtype=str, output_dtype=str, options={'temperature': int, 'max_tokens': int})`
 
 Add a new Funk instance to the manager.
 
 #### Parameters:
 
 - `name`: Unique identifier for the Funk instance.
 - `operation`: Description of the operation or task performed by the Funk instance.
-- `api_key`: API key for accessing the OpenAI GPT API. If not provided, the API key from FunkManager will be used.
+- `api_key`: API key for accessing the LLM API. If not provided, the API key from FunkManager will be used.
 - `model`: Model to be used for the Funk instance. If not provided, the default model from FunkManager will be used.
 - `retry_count`: Number of retries allowed if there's an error during execution (default is 0).
 - `input_dtype`: Data type expected for input to the Funk instance (default is `str`).
 - `output_dtype`: Data type expected for output from the Funk instance (default is `str`).
+- `options`: Allows you to pass parameters such as `temperate` and `max_tokens` to each jobs.
 
 #### Raises:
 
 - `ValueError`: If a Funk with the same name already exists or if the parameters are invalid.
 
 ###### `update(name, **kwargs)`
 
@@ -112,15 +112,15 @@
 
 - `ValueError`: If no Funk with the specified name is found.
 
 ## Example Usage
 
 ```python
 # Initialize FunkManager
-manager = FunkManager(model="gpt-4-turbo-preview", api_key="YOUR_OPENAI_API_KEY")
+manager = OpenAIFunk(model="gpt-4-turbo-preview", api_key="YOUR_OPENAI_API_KEY")
 
 # Add a new Funk instance
 manager.add(name="example_funk", operation="Perform a sample task")
 
 # Update parameters of the Funk instance
 manager.update("example_funk", retry_count=3, output_dtype=int)
 
@@ -139,15 +139,15 @@
 
 my_funks.run("find fruit", items)
 # should return something like: ['apple','date','fig','grape','jackfruit','lemon','mango','strawberry','watermelon']
 ```
 
 ## Prerequisites
 
-This library is built on top of the OpenAI API. Ensure you have the OpenAI Python client installed and configured.
+This library is built on top of the OpenAI & Claude API. Ensure you have the OpenAI or Claude Python client installed and configured.
 
 ## Contributing
 
 If you find any bugs or want to propose enhancements, feel free to create issues and pull requests on [GitHub](https://github.com/ciaraadkins/funkai).
 
 ## License
```

### Comparing `funkai-1.0/README.md` & `funkai-1.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,27 @@
+Metadata-Version: 2.1
+Name: funkai
+Version: 1.1
+Summary: Easily create and deploy placeholder functions powered by OpenAI and Anthropic (Claude) for rapid prototyping, diverse linguistic tasks, and quick insights.
+Home-page: https://github.com/ciaraadkins/funkai
+Author: Ciara Adkins
+Author-email: adkins.ciara@gmail.com.com
+Description-Content-Type: text/markdown
+Requires-Dist: openai
+Requires-Dist: llmonitor
+Requires-Dist: anthropic
+
 # Funkai Library
 
-Funkai is a Python library that encapsulates linguistic operations and uses OpenAI to perform them based on user inputs.
+Funkai is a Python library that encapsulates linguistic operations and uses OpenAI or Claude to perform them based on user inputs.
 
 ## Features
 
 - Diverse Operations: Easily define linguistic tasks that can process various data types.
-- Interaction with OpenAI: Seamlessly connect and utilize the OpenAI API to run operations.
+- Interaction with LLM: Seamlessly connect and utilize the LLM (OpenAI or Claude) API to run operations.
 - Dynamic Management: Add, remove, and run operations on-the-fly with the FunkManager.
 
 ## Funkai Setup
 
 Install via pip:
 
 ```python
@@ -21,51 +33,63 @@
 ```python
 git clone https://github.com/ciaraadkins/funkai.git
 pip install ./funkai/
 ```
 
 Once installed, import the necessary modules:
 
-```python
-from funkai import FunkManager
-```
-
 ## OpenAI Setup
 
 For the OpenAI functionality to work, you need to set up your OpenAI API key with init of FunkManager
 
 ```python
-funk = FunkManager(
+from funkai import OpenAIFunk
+
+funk = OpenAIFunk(
         model="gpt-4-turbo-preview",
         api_key='OPEN_API_KEY'
     )
 ```
 
 Additionally, if you want to monitor your llm usage, we recommend using llmonitor (you will need to also set up an account and get an app id on [llmonitor.com](https://llmonitor.com/)):
 
 ```python
 pip install openai llmonitor
 os.environ["LLMONITOR_APP_ID"] = "YOUR_LLMONITOR_APP_ID"
 ```
 
+## Claude Setup
+
+For the Claude functionality to work, you need to set up your Claude API key with init of FunkManager
+
+```python
+from funkai import ClaudeFunk
+
+funk = ClaudeFunk(
+        model="claude-3-opus-20240229",
+        api_key='CLAUDE_API_KEY'
+    )
+```
+
 # Methods
 
-###### `add(name, operation, api_key=None, model=None, retry_count=0, input_dtype=str, output_dtype=str)`
+###### `add(name, operation, api_key=None, model=None, retry_count=0, input_dtype=str, output_dtype=str, options={'temperature': int, 'max_tokens': int})`
 
 Add a new Funk instance to the manager.
 
 #### Parameters:
 
 - `name`: Unique identifier for the Funk instance.
 - `operation`: Description of the operation or task performed by the Funk instance.
-- `api_key`: API key for accessing the OpenAI GPT API. If not provided, the API key from FunkManager will be used.
+- `api_key`: API key for accessing the LLM API. If not provided, the API key from FunkManager will be used.
 - `model`: Model to be used for the Funk instance. If not provided, the default model from FunkManager will be used.
 - `retry_count`: Number of retries allowed if there's an error during execution (default is 0).
 - `input_dtype`: Data type expected for input to the Funk instance (default is `str`).
 - `output_dtype`: Data type expected for output from the Funk instance (default is `str`).
+- `options`: Allows you to pass parameters such as `temperate` and `max_tokens` to each jobs.
 
 #### Raises:
 
 - `ValueError`: If a Funk with the same name already exists or if the parameters are invalid.
 
 ###### `update(name, **kwargs)`
 
@@ -100,15 +124,15 @@
 
 - `ValueError`: If no Funk with the specified name is found.
 
 ## Example Usage
 
 ```python
 # Initialize FunkManager
-manager = FunkManager(model="gpt-4-turbo-preview", api_key="YOUR_OPENAI_API_KEY")
+manager = OpenAIFunk(model="gpt-4-turbo-preview", api_key="YOUR_OPENAI_API_KEY")
 
 # Add a new Funk instance
 manager.add(name="example_funk", operation="Perform a sample task")
 
 # Update parameters of the Funk instance
 manager.update("example_funk", retry_count=3, output_dtype=int)
 
@@ -127,15 +151,15 @@
 
 my_funks.run("find fruit", items)
 # should return something like: ['apple','date','fig','grape','jackfruit','lemon','mango','strawberry','watermelon']
 ```
 
 ## Prerequisites
 
-This library is built on top of the OpenAI API. Ensure you have the OpenAI Python client installed and configured.
+This library is built on top of the OpenAI & Claude API. Ensure you have the OpenAI or Claude Python client installed and configured.
 
 ## Contributing
 
 If you find any bugs or want to propose enhancements, feel free to create issues and pull requests on [GitHub](https://github.com/ciaraadkins/funkai).
 
 ## License
```

### Comparing `funkai-1.0/funkai/examples.py` & `funkai-1.1/funkai/examples.py`

 * *Files identical despite different names*

### Comparing `funkai-1.0/funkai/funk.py` & `funkai-1.1/funkai/funk.py`

 * *Files identical despite different names*

### Comparing `funkai-1.0/funkai/manager.py` & `funkai-1.1/funkai/manager.py`

 * *Files identical despite different names*

### Comparing `funkai-1.0/funkai.egg-info/PKG-INFO` & `funkai-1.1/funkai.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: funkai
-Version: 1.0
-Summary: Easily create and deploy placeholder functions powered by OpenAI for rapid prototyping, diverse linguistic tasks, and quick insights.
+Version: 1.1
+Summary: Easily create and deploy placeholder functions powered by OpenAI and Anthropic (Claude) for rapid prototyping, diverse linguistic tasks, and quick insights.
 Home-page: https://github.com/ciaraadkins/funkai
 Author: Ciara Adkins
 Author-email: adkins.ciara@gmail.com.com
 Description-Content-Type: text/markdown
 Requires-Dist: openai
 Requires-Dist: llmonitor
 Requires-Dist: anthropic
 
 # Funkai Library
 
-Funkai is a Python library that encapsulates linguistic operations and uses OpenAI to perform them based on user inputs.
+Funkai is a Python library that encapsulates linguistic operations and uses OpenAI or Claude to perform them based on user inputs.
 
 ## Features
 
 - Diverse Operations: Easily define linguistic tasks that can process various data types.
-- Interaction with OpenAI: Seamlessly connect and utilize the OpenAI API to run operations.
+- Interaction with LLM: Seamlessly connect and utilize the LLM (OpenAI or Claude) API to run operations.
 - Dynamic Management: Add, remove, and run operations on-the-fly with the FunkManager.
 
 ## Funkai Setup
 
 Install via pip:
 
 ```python
@@ -33,51 +33,63 @@
 ```python
 git clone https://github.com/ciaraadkins/funkai.git
 pip install ./funkai/
 ```
 
 Once installed, import the necessary modules:
 
-```python
-from funkai import FunkManager
-```
-
 ## OpenAI Setup
 
 For the OpenAI functionality to work, you need to set up your OpenAI API key with init of FunkManager
 
 ```python
-funk = FunkManager(
+from funkai import OpenAIFunk
+
+funk = OpenAIFunk(
         model="gpt-4-turbo-preview",
         api_key='OPEN_API_KEY'
     )
 ```
 
 Additionally, if you want to monitor your llm usage, we recommend using llmonitor (you will need to also set up an account and get an app id on [llmonitor.com](https://llmonitor.com/)):
 
 ```python
 pip install openai llmonitor
 os.environ["LLMONITOR_APP_ID"] = "YOUR_LLMONITOR_APP_ID"
 ```
 
+## Claude Setup
+
+For the Claude functionality to work, you need to set up your Claude API key with init of FunkManager
+
+```python
+from funkai import ClaudeFunk
+
+funk = ClaudeFunk(
+        model="claude-3-opus-20240229",
+        api_key='CLAUDE_API_KEY'
+    )
+```
+
 # Methods
 
-###### `add(name, operation, api_key=None, model=None, retry_count=0, input_dtype=str, output_dtype=str)`
+###### `add(name, operation, api_key=None, model=None, retry_count=0, input_dtype=str, output_dtype=str, options={'temperature': int, 'max_tokens': int})`
 
 Add a new Funk instance to the manager.
 
 #### Parameters:
 
 - `name`: Unique identifier for the Funk instance.
 - `operation`: Description of the operation or task performed by the Funk instance.
-- `api_key`: API key for accessing the OpenAI GPT API. If not provided, the API key from FunkManager will be used.
+- `api_key`: API key for accessing the LLM API. If not provided, the API key from FunkManager will be used.
 - `model`: Model to be used for the Funk instance. If not provided, the default model from FunkManager will be used.
 - `retry_count`: Number of retries allowed if there's an error during execution (default is 0).
 - `input_dtype`: Data type expected for input to the Funk instance (default is `str`).
 - `output_dtype`: Data type expected for output from the Funk instance (default is `str`).
+- `options`: Allows you to pass parameters such as `temperate` and `max_tokens` to each jobs.
 
 #### Raises:
 
 - `ValueError`: If a Funk with the same name already exists or if the parameters are invalid.
 
 ###### `update(name, **kwargs)`
 
@@ -112,15 +124,15 @@
 
 - `ValueError`: If no Funk with the specified name is found.
 
 ## Example Usage
 
 ```python
 # Initialize FunkManager
-manager = FunkManager(model="gpt-4-turbo-preview", api_key="YOUR_OPENAI_API_KEY")
+manager = OpenAIFunk(model="gpt-4-turbo-preview", api_key="YOUR_OPENAI_API_KEY")
 
 # Add a new Funk instance
 manager.add(name="example_funk", operation="Perform a sample task")
 
 # Update parameters of the Funk instance
 manager.update("example_funk", retry_count=3, output_dtype=int)
 
@@ -139,15 +151,15 @@
 
 my_funks.run("find fruit", items)
 # should return something like: ['apple','date','fig','grape','jackfruit','lemon','mango','strawberry','watermelon']
 ```
 
 ## Prerequisites
 
-This library is built on top of the OpenAI API. Ensure you have the OpenAI Python client installed and configured.
+This library is built on top of the OpenAI & Claude API. Ensure you have the OpenAI or Claude Python client installed and configured.
 
 ## Contributing
 
 If you find any bugs or want to propose enhancements, feel free to create issues and pull requests on [GitHub](https://github.com/ciaraadkins/funkai).
 
 ## License
```

### Comparing `funkai-1.0/setup.py` & `funkai-1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name="funkai",
-    version="1.0",
+    version="1.1",
     packages=find_packages(),
     install_requires=[
         "openai",  'llmonitor', 'anthropic'
     ],
     author="Ciara Adkins",
     author_email="adkins.ciara@gmail.com.com",
-    description="Easily create and deploy placeholder functions powered by OpenAI for rapid prototyping, diverse linguistic tasks, and quick insights.",
+    description="Easily create and deploy placeholder functions powered by OpenAI and Anthropic (Claude) for rapid prototyping, diverse linguistic tasks, and quick insights.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/ciaraadkins/funkai",
 )
```

