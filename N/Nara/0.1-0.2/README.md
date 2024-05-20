# Comparing `tmp/nara-0.1.tar.gz` & `tmp/nara-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nara-0.1.tar", last modified: Sun May 19 19:54:36 2024, max compression
+gzip compressed data, was "nara-0.2.tar", last modified: Mon May 20 06:01:32 2024, max compression
```

## Comparing `nara-0.1.tar` & `nara-0.2.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 19:54:36.776708 nara-0.1/
--rw-rw-rw-   0        0        0     1099 2024-05-19 11:22:20.000000 nara-0.1/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2024-05-19 19:54:36.747747 nara-0.1/Nara/
-drwxrwxrwx   0        0        0        0 2024-05-19 19:54:36.757484 nara-0.1/Nara/Extra/
-drwxrwxrwx   0        0        0        0 2024-05-19 19:54:36.767022 nara-0.1/Nara/Extra/Json/
--rw-rw-rw-   0        0        0     4079 2024-05-19 10:15:08.000000 nara-0.1/Nara/Extra/Json/Cache.py
--rw-rw-rw-   0        0        0     3156 2024-05-19 08:59:50.000000 nara-0.1/Nara/Extra/Json/LoadJson.py
--rw-rw-rw-   0        0        0     4313 2024-05-19 10:17:44.000000 nara-0.1/Nara/Extra/Json/Save.py
--rw-rw-rw-   0        0        0     5148 2024-05-19 07:25:39.000000 nara-0.1/Nara/Extra/Json/TestingTools.py
-drwxrwxrwx   0        0        0        0 2024-05-19 19:54:36.770526 nara-0.1/Nara/Extra/TempMail/
--rw-rw-rw-   0        0        0     1618 2024-05-19 05:08:02.000000 nara-0.1/Nara/Extra/TempMail/retry.py
--rw-rw-rw-   0        0        0     7378 2024-05-19 14:01:26.000000 nara-0.1/Nara/Extra/TempMail/tempmail.py
--rw-rw-rw-   0        0        0      295 2024-05-19 14:51:46.000000 nara-0.1/Nara/Extra/__init__.py
--rw-rw-rw-   0        0        0      776 2024-05-19 17:49:53.000000 nara-0.1/Nara/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 19:54:36.772524 nara-0.1/Nara/nara/
--rw-rw-rw-   0        0        0     4359 2024-05-19 19:35:19.000000 nara-0.1/Nara/nara/GenFunc.py
--rw-rw-rw-   0        0        0     3562 2024-05-19 17:50:13.000000 nara-0.1/Nara/nara/GenTemplate.py
-drwxrwxrwx   0        0        0        0 2024-05-19 19:54:36.773526 nara-0.1/Nara.egg-info/
--rw-rw-rw-   0        0        0     8635 2024-05-19 19:54:36.000000 nara-0.1/Nara.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      425 2024-05-19 19:54:36.000000 nara-0.1/Nara.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 19:54:36.000000 nara-0.1/Nara.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-05-19 19:54:36.000000 nara-0.1/Nara.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-19 19:54:36.000000 nara-0.1/Nara.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     8635 2024-05-19 19:54:36.774525 nara-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     6005 2024-05-19 19:31:10.000000 nara-0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-19 19:54:36.776708 nara-0.1/setup.cfg
--rw-rw-rw-   0        0        0     3064 2024-05-19 14:50:16.000000 nara-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 06:01:32.436663 nara-0.2/
+-rw-rw-rw-   0        0        0     1099 2024-05-19 11:22:20.000000 nara-0.2/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2024-05-20 06:01:32.321154 nara-0.2/Nara/
+drwxrwxrwx   0        0        0        0 2024-05-20 06:01:32.381611 nara-0.2/Nara/Extra/
+drwxrwxrwx   0        0        0        0 2024-05-20 06:01:32.399819 nara-0.2/Nara/Extra/Json/
+-rw-rw-rw-   0        0        0     4079 2024-05-19 10:15:08.000000 nara-0.2/Nara/Extra/Json/Cache.py
+-rw-rw-rw-   0        0        0     3156 2024-05-19 08:59:50.000000 nara-0.2/Nara/Extra/Json/LoadJson.py
+-rw-rw-rw-   0        0        0     4313 2024-05-19 10:17:44.000000 nara-0.2/Nara/Extra/Json/Save.py
+-rw-rw-rw-   0        0        0     5148 2024-05-19 07:25:39.000000 nara-0.2/Nara/Extra/Json/TestingTools.py
+drwxrwxrwx   0        0        0        0 2024-05-20 06:01:32.410363 nara-0.2/Nara/Extra/TempMail/
+-rw-rw-rw-   0        0        0     1618 2024-05-19 05:08:02.000000 nara-0.2/Nara/Extra/TempMail/retry.py
+-rw-rw-rw-   0        0        0     7378 2024-05-19 14:01:26.000000 nara-0.2/Nara/Extra/TempMail/tempmail.py
+-rw-rw-rw-   0        0        0      295 2024-05-19 14:51:46.000000 nara-0.2/Nara/Extra/__init__.py
+-rw-rw-rw-   0        0        0      269 2024-05-20 04:52:48.000000 nara-0.2/Nara/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 06:01:32.426587 nara-0.2/Nara/nara/
+-rw-rw-rw-   0        0        0     3892 2024-05-20 05:28:11.000000 nara-0.2/Nara/nara/GenFunc.py
+-rw-rw-rw-   0        0        0     3093 2024-05-20 05:28:40.000000 nara-0.2/Nara/nara/GenTemplate.py
+-rw-rw-rw-   0        0        0     1682 2024-05-20 05:51:28.000000 nara-0.2/Nara/nara/init.py
+drwxrwxrwx   0        0        0        0 2024-05-20 06:01:32.430600 nara-0.2/Nara.egg-info/
+-rw-rw-rw-   0        0        0     8635 2024-05-20 06:01:31.000000 nara-0.2/Nara.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      443 2024-05-20 06:01:32.000000 nara-0.2/Nara.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 06:01:31.000000 nara-0.2/Nara.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-05-20 06:01:31.000000 nara-0.2/Nara.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-20 06:01:31.000000 nara-0.2/Nara.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8635 2024-05-20 06:01:32.433183 nara-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6005 2024-05-19 19:31:10.000000 nara-0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-20 06:01:32.436663 nara-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     3064 2024-05-20 05:57:53.000000 nara-0.2/setup.py
```

### Comparing `nara-0.1/LICENSE.txt` & `nara-0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nara-0.1/Nara/Extra/Json/Cache.py` & `nara-0.2/Nara/Extra/Json/Cache.py`

 * *Files identical despite different names*

### Comparing `nara-0.1/Nara/Extra/Json/LoadJson.py` & `nara-0.2/Nara/Extra/Json/LoadJson.py`

 * *Files identical despite different names*

### Comparing `nara-0.1/Nara/Extra/Json/Save.py` & `nara-0.2/Nara/Extra/Json/Save.py`

 * *Files identical despite different names*

### Comparing `nara-0.1/Nara/Extra/Json/TestingTools.py` & `nara-0.2/Nara/Extra/Json/TestingTools.py`

 * *Files identical despite different names*

### Comparing `nara-0.1/Nara/Extra/TempMail/retry.py` & `nara-0.2/Nara/Extra/TempMail/retry.py`

 * *Files identical despite different names*

### Comparing `nara-0.1/Nara/Extra/TempMail/tempmail.py` & `nara-0.2/Nara/Extra/TempMail/tempmail.py`

 * *Files identical despite different names*

### Comparing `nara-0.1/Nara/nara/GenFunc.py` & `nara-0.2/Nara/nara/GenFunc.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,49 @@
 import re
 from groq import Groq
 import functools
 import inspect
 import os
 from dotenv import load_dotenv
 from rich.console import Console
+from Nara.nara.init import init
+
 
 current_dir = os.path.dirname(__file__)
 file_path = os.path.join(current_dir, '.env')
 
 load_dotenv(dotenv_path=file_path)
 
 System = [
     {"role": "system", "content": "write code in ```python\n<code>\n``` format"},
     {"role": "system", "content": "you are a Ai which create funcs src in python whatever user instruct and if any imports of module is needed then write import <module> inside the function."},
     {"role": "system", "content": "only provide func code DO not run it."},
     {"role": "user", "content": "# Instruction Create This function\n\ndef add(a: int = 0, b: int = 0) -> int:"},
     {"role": "user", "content": "Sure, here's the Python function code for the add function as per your instructions:\n\n```python\ndef add(a: int = 0, b: int = 0) -> int:\n    return a + b\n```"},
 ]
 
-API = os.getenv("GROQ_API")
-
-if not API:
-    # Get the directory of the current script
-    current_dir = os.path.dirname(__file__)
-
-    # Get the full path of a file in the same directory
-    file_path = os.path.join(current_dir, '.env')
-    
-    console = Console()
-    API = console.input("[bold #e6a330]Let Begin with Groq [/bold #e6a330][green]API[/green][bold #0b7ce6] (https://console.groq.com/keys): [/bold #0b7ce6]")
-    with open(file_path, "w") as f:
-        f.write(f"GROQ_API = {API}")
-    console.print("\nYOU CAN CHANGE YOUR API USING init() from Nara")
-
-client = Groq(api_key=API)
 
 def Filter(txt:str) -> str|None:
     pattern = r"```python(.*?)```"
     matches = re.findall(pattern, txt, re.DOTALL)
 
     if matches:
         python_code = matches[0].strip()
         return python_code
     else:
         return None
 
 def GroqGen(Prompt:str):
+    API = os.getenv("GROQ_API")
+
+    if not API:
+        API = init()
+
+    client = Groq(api_key=API)
+
     completion = client.chat.completions.create(
     model="llama3-70b-8192",
     messages = System + [{ "role": "user", "content": Prompt }],
     temperature=0.1,
     max_tokens=4096,
     top_p=1,
     stream=True,
```

### Comparing `nara-0.1/Nara/nara/GenTemplate.py` & `nara-0.2/Nara/nara/GenTemplate.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,54 +1,44 @@
 import re
 from groq import Groq
 import inspect
 import os
 from dotenv import load_dotenv
 from rich.console import Console
+from Nara.nara.init import init
 
 current_dir = os.path.dirname(__file__)
 file_path = os.path.join(current_dir, '.env')
 
 load_dotenv(dotenv_path=file_path)
 
 System = [
     {"role": "system", "content": "write code in ```python\n<code>\n``` format"},
     {"role": "system", "content": "you are a Ai which create templates src in python whatever user instruct and if any imports of module is needed then write import <module>."},
     {"role": "user", "content": "# Instruction Create Flask Template"},
     {"role": "user", "content": "Sure, here's the Python template code for the flask template as per your instructions:\n\n```python\nfrom flask import Flask, render_template\napp = Flask(__name__)\n\n@app.route('/')\ndef index():\n    return 'Hello World'\n\nif __name__ == '__main__':\n    app.run(debug=True)\n```"},
 ]
 
-API = os.getenv("GROQ_API")
-
-if not API:
-    # Get the directory of the current script
-    current_dir = os.path.dirname(__file__)
-
-    # Get the full path of a file in the same directory
-    file_path = os.path.join(current_dir, '.env')
-    
-    console = Console()
-    API = console.input("[bold #e6a330]Let Begin with Groq [/bold #e6a330][green]API[/green][bold #0b7ce6] (https://console.groq.com/keys): [/bold #0b7ce6]")
-    with open(file_path, "w") as f:
-        f.write(f"GROQ_API = {API}")
-    console.print("\nYOU CAN CHANGE YOUR API USING init() from Nara")
-
-client = Groq(api_key=API)
 
 def Filter(txt:str) -> str|None:
     pattern = r"```python(.*?)```"
     matches = re.findall(pattern, txt, re.DOTALL)
 
     if matches:
         python_code = matches[0].strip()
         return python_code
     else:
         return None
 
 def GroqGen(Prompt:str):
+    API = os.getenv("GROQ_API")
+    if not API:
+        API = init()
+    client = Groq(api_key=API)
+    
     completion = client.chat.completions.create(
     model="llama3-70b-8192",
     messages = System + [{ "role": "user", "content": Prompt }],
     temperature=0.1,
     max_tokens=4096,
     top_p=1,
     stream=True,
```

### Comparing `nara-0.1/Nara.egg-info/PKG-INFO` & `nara-0.2/Nara.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Nara
-Version: 0.1
+Version: 0.2
 Summary: A versatile package for AI-based real-time information and chatbot interactions, creating temporary emails, generating random data, caching, and JSON manipulation.
 Home-page: https://github.com/subh-sk/Nara
 Author: Subhash Kumar, Divyansh Shukla, Yateesh Reddy
 Maintainer: Nara Developers
 Maintainer-email: naravirtualai@gmail.com
 License: MIT
 Project-URL: Homepage, https://github.com/subh-sk/Nara
```

### Comparing `nara-0.1/PKG-INFO` & `nara-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Nara
-Version: 0.1
+Version: 0.2
 Summary: A versatile package for AI-based real-time information and chatbot interactions, creating temporary emails, generating random data, caching, and JSON manipulation.
 Home-page: https://github.com/subh-sk/Nara
 Author: Subhash Kumar, Divyansh Shukla, Yateesh Reddy
 Maintainer: Nara Developers
 Maintainer-email: naravirtualai@gmail.com
 License: MIT
 Project-URL: Homepage, https://github.com/subh-sk/Nara
```

### Comparing `nara-0.1/README.md` & `nara-0.2/README.md`

 * *Files identical despite different names*

### Comparing `nara-0.1/setup.py` & `nara-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1'
+VERSION = '0.2'
 
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Education',
     'Intended Audience :: Developers',
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Testing",
```

