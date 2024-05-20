# Comparing `tmp/ipython_args-1.0.2.tar.gz` & `tmp/ipython_args-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipython_args-1.0.2.tar", last modified: Wed Feb  7 04:20:19 2024, max compression
+gzip compressed data, was "ipython_args-1.0.3.tar", last modified: Mon May 20 06:17:49 2024, max compression
```

## Comparing `ipython_args-1.0.2.tar` & `ipython_args-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 qkatlehdrnf   (501) staff       (20)        0 2024-02-07 04:20:19.694105 ipython_args-1.0.2/
--rw-r--r--   0 qkatlehdrnf   (501) staff       (20)     9704 2024-02-07 04:20:19.693830 ipython_args-1.0.2/PKG-INFO
--rw-r--r--   0 qkatlehdrnf   (501) staff       (20)     8731 2024-02-07 04:04:10.000000 ipython_args-1.0.2/README.md
-drwxr-xr-x   0 qkatlehdrnf   (501) staff       (20)        0 2024-02-07 04:20:19.692722 ipython_args-1.0.2/ipython_args/
--rw-r--r--   0 qkatlehdrnf   (501) staff       (20)       87 2024-01-25 13:52:51.000000 ipython_args-1.0.2/ipython_args/__init__.py
--rw-r--r--   0 qkatlehdrnf   (501) staff       (20)      860 2024-01-25 12:34:32.000000 ipython_args-1.0.2/ipython_args/utils.py
-drwxr-xr-x   0 qkatlehdrnf   (501) staff       (20)        0 2024-02-07 04:20:19.693636 ipython_args-1.0.2/ipython_args.egg-info/
--rw-r--r--   0 qkatlehdrnf   (501) staff       (20)     9704 2024-02-07 04:20:19.000000 ipython_args-1.0.2/ipython_args.egg-info/PKG-INFO
--rw-r--r--   0 qkatlehdrnf   (501) staff       (20)      244 2024-02-07 04:20:19.000000 ipython_args-1.0.2/ipython_args.egg-info/SOURCES.txt
--rw-r--r--   0 qkatlehdrnf   (501) staff       (20)        1 2024-02-07 04:20:19.000000 ipython_args-1.0.2/ipython_args.egg-info/dependency_links.txt
--rw-r--r--   0 qkatlehdrnf   (501) staff       (20)       17 2024-02-07 04:20:19.000000 ipython_args-1.0.2/ipython_args.egg-info/requires.txt
--rw-r--r--   0 qkatlehdrnf   (501) staff       (20)       13 2024-02-07 04:20:19.000000 ipython_args-1.0.2/ipython_args.egg-info/top_level.txt
--rw-r--r--   0 qkatlehdrnf   (501) staff       (20)       38 2024-02-07 04:20:19.694150 ipython_args-1.0.2/setup.cfg
--rw-r--r--   0 qkatlehdrnf   (501) staff       (20)     1671 2024-02-07 04:19:49.000000 ipython_args-1.0.2/setup.py
+drwxrwxrwx   0 wj        (1000) wj        (1000)        0 2024-05-20 06:17:49.338547 ipython_args-1.0.3/
+-rwxrwxrwx   0 wj        (1000) wj        (1000)     9776 2024-05-20 06:17:49.306420 ipython_args-1.0.3/PKG-INFO
+-rwxrwxrwx   0 wj        (1000) wj        (1000)     8841 2024-05-20 05:48:04.000000 ipython_args-1.0.3/README.md
+drwxrwxrwx   0 wj        (1000) wj        (1000)        0 2024-05-20 06:17:48.954554 ipython_args-1.0.3/ipython_args/
+-rwxrwxrwx   0 wj        (1000) wj        (1000)       89 2024-05-20 05:48:04.000000 ipython_args-1.0.3/ipython_args/__init__.py
+-rwxrwxrwx   0 wj        (1000) wj        (1000)      885 2024-05-20 05:48:04.000000 ipython_args-1.0.3/ipython_args/utils.py
+drwxrwxrwx   0 wj        (1000) wj        (1000)        0 2024-05-20 06:17:49.252112 ipython_args-1.0.3/ipython_args.egg-info/
+-rwxrwxrwx   0 wj        (1000) wj        (1000)     9776 2024-05-20 06:17:48.000000 ipython_args-1.0.3/ipython_args.egg-info/PKG-INFO
+-rwxrwxrwx   0 wj        (1000) wj        (1000)      244 2024-05-20 06:17:48.000000 ipython_args-1.0.3/ipython_args.egg-info/SOURCES.txt
+-rwxrwxrwx   0 wj        (1000) wj        (1000)        1 2024-05-20 06:17:48.000000 ipython_args-1.0.3/ipython_args.egg-info/dependency_links.txt
+-rwxrwxrwx   0 wj        (1000) wj        (1000)       27 2024-05-20 06:17:48.000000 ipython_args-1.0.3/ipython_args.egg-info/requires.txt
+-rwxrwxrwx   0 wj        (1000) wj        (1000)       13 2024-05-20 06:17:48.000000 ipython_args-1.0.3/ipython_args.egg-info/top_level.txt
+-rwxrwxrwx   0 wj        (1000) wj        (1000)       38 2024-05-20 06:17:49.341543 ipython_args-1.0.3/setup.cfg
+-rwxrwxrwx   0 wj        (1000) wj        (1000)     1742 2024-05-20 05:56:14.000000 ipython_args-1.0.3/setup.py
```

### Comparing `ipython_args-1.0.2/PKG-INFO` & `ipython_args-1.0.3/ipython_args.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ipython_args
-Version: 1.0.2
+Name: ipython-args
+Version: 1.0.3
 Summary: A utility for seamless argument parsing in IPython notebooks and Python scripts.
 Home-page: https://github.com/qkaTlehdrnf/IpythonArguments
 Author: Kim, Won-Joong
 Author-email: wonjoong11@yonsei.ac.kr
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -16,14 +16,17 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: IPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
+Requires-Dist: easydict
+Requires-Dist: ipython
+Requires-Dist: ipykernel
 
 # Python Argument Parser for Notebooks and Scripts
 
 ## Introduction
 
 This Python module provides a versatile argument parsing solution that works seamlessly both in Jupyter notebooks (or similar environments) and standard Python scripts. It allows the same code to accept arguments in two different contexts, making it easier to write code that is flexible and easy to test.
```

### Comparing `ipython_args-1.0.2/README.md` & `ipython_args-1.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+Metadata-Version: 2.1
+Name: ipython_args
+Version: 1.0.3
+Summary: A utility for seamless argument parsing in IPython notebooks and Python scripts.
+Home-page: https://github.com/qkaTlehdrnf/IpythonArguments
+Author: Kim, Won-Joong
+Author-email: wonjoong11@yonsei.ac.kr
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Framework :: IPython
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.4
+Description-Content-Type: text/markdown
+Requires-Dist: easydict
+Requires-Dist: ipython
+Requires-Dist: ipykernel
+
 # Python Argument Parser for Notebooks and Scripts
 
 ## Introduction
 
 This Python module provides a versatile argument parsing solution that works seamlessly both in Jupyter notebooks (or similar environments) and standard Python scripts. It allows the same code to accept arguments in two different contexts, making it easier to write code that is flexible and easy to test.
 
 The document is helped by ChatGPT 4.0
```

### Comparing `ipython_args-1.0.2/ipython_args/utils.py` & `ipython_args-1.0.3/ipython_args/utils.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-import argparse, easydict
-
-
-def ipython_args(args_dict: dict):
-    if is_notebook():
-        args = easydict.EasyDict()
-        for key, value in args_dict.items():
-            args[key] = value
-        return args
-    else:
-        parser = argparse.ArgumentParser()
-        for key, value in args_dict.items():
-            parser.add_argument('--'+key, type=type(value), default=value)
-        return parser.parse_args()
-    
-def is_notebook() -> bool:
-    try:
-        shell = get_ipython().__class__.__name__
-        if shell == 'ZMQInteractiveShell':
-            return True   # Jupyter notebook or qtconsole
-        elif shell == 'TerminalInteractiveShell':
-            return False  # Terminal running IPython
-        else:
-            return False  # Other type (?)
-    except NameError:
+import argparse, easydict
+
+
+def ipython_args(args_dict: dict):
+    if is_notebook():
+        args = easydict.EasyDict()
+        for key, value in args_dict.items():
+            args[key] = value
+        return args
+    else:
+        parser = argparse.ArgumentParser()
+        for key, value in args_dict.items():
+            parser.add_argument('--'+key, type=type(value), default=value)
+        return parser.parse_args()
+    
+def is_notebook() -> bool:
+    try:
+        shell = get_ipython().__class__.__name__
+        if shell == 'ZMQInteractiveShell':
+            return True   # Jupyter notebook or qtconsole
+        elif shell == 'TerminalInteractiveShell':
+            return False  # Terminal running IPython
+        else:
+            return False  # Other type (?)
+    except NameError:
         return False      # Probably standard Python interpreter
```

### Comparing `ipython_args-1.0.2/ipython_args.egg-info/PKG-INFO` & `ipython_args-1.0.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,133 +1,110 @@
-Metadata-Version: 2.1
-Name: ipython-args
-Version: 1.0.2
-Summary: A utility for seamless argument parsing in IPython notebooks and Python scripts.
-Home-page: https://github.com/qkaTlehdrnf/IpythonArguments
-Author: Kim, Won-Joong
-Author-email: wonjoong11@yonsei.ac.kr
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Framework :: IPython
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.4
-Description-Content-Type: text/markdown
-
-# Python Argument Parser for Notebooks and Scripts
-
-## Introduction
-
-This Python module provides a versatile argument parsing solution that works seamlessly both in Jupyter notebooks (or similar environments) and standard Python scripts. It allows the same code to accept arguments in two different contexts, making it easier to write code that is flexible and easy to test.
-
-The document is helped by ChatGPT 4.0
-
-## Features
-
-* **Dual Compatibility** : Works with Jupyter notebooks and standard Python scripts.
-* **Easy Integration** : Simple to integrate into existing Python projects.
-* **Dynamic Argument Parsing** : Automatically switches between `easydict` and `argparse` depending on the execution environment.
-
-## Requirements
-
-* `easydict`
-* `argparse`
-
-## Installation
-
-Ensure that you have `easydict` installed. You can install it using pip:
-
-<pre><div class="bg-black rounded-md"><div class="flex items-center relative text-gray-200 bg-gray-800 dark:bg-token-surface-primary px-4 py-2 text-xs font-sans justify-between rounded-t-md"><span class="" data-state="closed"><button class="flex gap-1 items-center"><svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" class="icon-sm"><path fill-rule="evenodd" clip-rule="evenodd" d="M12 4C10.8954 4 10 4.89543 10 6H14C14 4.89543 13.1046 4 12 4ZM8.53513 4C9.22675 2.8044 10.5194 2 12 2C13.4806 2 14.7733 2.8044 15.4649 4H17C18.6569 4 20 5.34315 20 7V19C20 20.6569 18.6569 22 17 22H7C5.34315 22 4 20.6569 4 19V7C4 5.34315 5.34315 4 7 4H8.53513ZM8 6H7C6.44772 6 6 6.44772 6 7V19C6 19.5523 6.44772 20 7 20H17C17.5523 20 18 19.5523 18 19V7C18 6.44772 17.5523 6 17 6H16C16 7.10457 15.1046 8 14 8H10C8.89543 8 8 7.10457 8 6Z" fill="currentColor"></path></svg></button></span></div><div class="p-4 overflow-y-auto"><code class="!whitespace-pre hljs language-bash">pip install easydict
-</code></div></div></pre>
-
-## Usage
-
-### Defining Arguments
-
-First, define your arguments in a dictionary format. For example:
-
-<pre><div class="bg-black rounded-md"><div class="flex items-center relative text-gray-200 bg-gray-800 dark:bg-token-surface-primary px-4 py-2 text-xs font-sans justify-between rounded-t-md"><span class="" data-state="closed"><button class="flex gap-1 items-center"><svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" class="icon-sm"><path fill-rule="evenodd" clip-rule="evenodd" d="M12 4C10.8954 4 10 4.89543 10 6H14C14 4.89543 13.1046 4 12 4ZM8.53513 4C9.22675 2.8044 10.5194 2 12 2C13.4806 2 14.7733 2.8044 15.4649 4H17C18.6569 4 20 5.34315 20 7V19C20 20.6569 18.6569 22 17 22H7C5.34315 22 4 20.6569 4 19V7C4 5.34315 5.34315 4 7 4H8.53513ZM8 6H7C6.44772 6 6 6.44772 6 7V19C6 19.5523 6.44772 20 7 20H17C17.5523 20 18 19.5523 18 19V7C18 6.44772 17.5523 6 17 6H16C16 7.10457 15.1046 8 14 8H10C8.89543 8 8 7.10457 8 6Z" fill="currentColor"></path></svg></button></span></div><div class="p-4 overflow-y-auto"><code class="!whitespace-pre hljs language-python">args_dict = {
-    "arg1": value1,
-    "arg2": value2,
-    // Add more arguments as needed
-}
-</code></div></div></pre>
-
-### Parsing Arguments
-
-Then, simply call the `ipython_args` function with your arguments dictionary:
-
-<pre><div class="bg-black rounded-md"><div class="flex items-center relative text-gray-200 bg-gray-800 dark:bg-token-surface-primary px-4 py-2 text-xs font-sans justify-between rounded-t-md"><span class="" data-state="closed"><button class="flex gap-1 items-center"><svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" class="icon-sm"><path fill-rule="evenodd" clip-rule="evenodd" d="M12 4C10.8954 4 10 4.89543 10 6H14C14 4.89543 13.1046 4 12 4ZM8.53513 4C9.22675 2.8044 10.5194 2 12 2C13.4806 2 14.7733 2.8044 15.4649 4H17C18.6569 4 20 5.34315 20 7V19C20 20.6569 18.6569 22 17 22H7C5.34315 22 4 20.6569 4 19V7C4 5.34315 5.34315 4 7 4H8.53513ZM8 6H7C6.44772 6 6 6.44772 6 7V19C6 19.5523 6.44772 20 7 20H17C17.5523 20 18 19.5523 18 19V7C18 6.44772 17.5523 6 17 6H16C16 7.10457 15.1046 8 14 8H10C8.89543 8 8 7.10457 8 6Z" fill="currentColor"></path></svg></button></span></div><div class="p-4 overflow-y-auto"><code class="!whitespace-pre hljs language-python">args = ipython_args(args_dict)
-</code></div></div></pre>
-
-In a Jupyter notebook environment, `args` will be an `EasyDict` object, allowing you to access arguments using dot notation (`args.arg1`). In a standard script, `args` will be the usual `argparse.Namespace` object.
-
-### Checking Environment
-
-The `is_notebook` function can be used independently to check if the code is running in a Jupyter notebook environment.
-
-## Example
-
-Here's a simple example demonstrating how to use this module:
-
-<pre><div class="bg-black rounded-md"><div class="flex items-center relative text-gray-200 bg-gray-800 dark:bg-token-surface-primary px-4 py-2 text-xs font-sans justify-between rounded-t-md"><span class="" data-state="closed"><button class="flex gap-1 items-center"><svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" class="icon-sm"><path fill-rule="evenodd" clip-rule="evenodd" d="M12 4C10.8954 4 10 4.89543 10 6H14C14 4.89543 13.1046 4 12 4ZM8.53513 4C9.22675 2.8044 10.5194 2 12 2C13.4806 2 14.7733 2.8044 15.4649 4H17C18.6569 4 20 5.34315 20 7V19C20 20.6569 18.6569 22 17 22H7C5.34315 22 4 20.6569 4 19V7C4 5.34315 5.34315 4 7 4H8.53513ZM8 6H7C6.44772 6 6 6.44772 6 7V19C6 19.5523 6.44772 20 7 20H17C17.5523 20 18 19.5523 18 19V7C18 6.44772 17.5523 6 17 6H16C16 7.10457 15.1046 8 14 8H10C8.89543 8 8 7.10457 8 6Z" fill="currentColor"></path></svg></button></span></div><div class="p-4 overflow-y-auto"><code class="!whitespace-pre hljs language-python">from ipython_args import ipython_args
-
-# Define your arguments here
-args_dict = {
-    "epoch": 10,
-    "learning_rate": 0.001
-}
-
-# Parse arguments
-args = ipython_args(args_dict)
-
-# Accessing arguments
-print(args.epoch)
-print(args.learning_rate)
-</code></div></div></pre>
-
-You can use is_notebook function to check the environment is notebook or not
-
-<pre><div class="bg-black rounded-md"><div class="flex items-center relative text-gray-200 bg-gray-800 dark:bg-token-surface-primary px-4 py-2 text-xs font-sans justify-between rounded-t-md"><span class="" data-state="closed"><button class="flex gap-1 items-center"><svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" class="icon-sm"><path fill-rule="evenodd" clip-rule="evenodd" d="M12 4C10.8954 4 10 4.89543 10 6H14C14 4.89543 13.1046 4 12 4ZM8.53513 4C9.22675 2.8044 10.5194 2 12 2C13.4806 2 14.7733 2.8044 15.4649 4H17C18.6569 4 20 5.34315 20 7V19C20 20.6569 18.6569 22 17 22H7C5.34315 22 4 20.6569 4 19V7C4 5.34315 5.34315 4 7 4H8.53513ZM8 6H7C6.44772 6 6 6.44772 6 7V19C6 19.5523 6.44772 20 7 20H17C17.5523 20 18 19.5523 18 19V7C18 6.44772 17.5523 6 17 6H16C16 7.10457 15.1046 8 14 8H10C8.89543 8 8 7.10457 8 6Z" fill="currentColor"></path></svg></button></span></div><div class="p-4 overflow-y-auto"><code class="!whitespace-pre hljs language-python">from ipython_args import is_notebook
-
-# Check whether the current environment is notebook shell or not
-current_env_notebook = is_notebook())
-</code></div></div></pre>
-
-## Contributing & Acknowledgements
-
-Thanks for professor Dr. Lee, Soo-Hong who encourage me to upload the project.
-
-
-This projects are side-project of the National Research Foundation of Korea, ‘Development of a 2-axis ankle exoskeleton robot to identify intentions using deep learning-based EMG images’ (No.2021R1I1A205215811)
-
-## License
-
-This project is open-source and available under the [MIT License]().
-
-Copyright (c) 2018 The Python Packaging Authority
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+# Python Argument Parser for Notebooks and Scripts
+
+## Introduction
+
+This Python module provides a versatile argument parsing solution that works seamlessly both in Jupyter notebooks (or similar environments) and standard Python scripts. It allows the same code to accept arguments in two different contexts, making it easier to write code that is flexible and easy to test.
+
+The document is helped by ChatGPT 4.0
+
+## Features
+
+* **Dual Compatibility** : Works with Jupyter notebooks and standard Python scripts.
+* **Easy Integration** : Simple to integrate into existing Python projects.
+* **Dynamic Argument Parsing** : Automatically switches between `easydict` and `argparse` depending on the execution environment.
+
+## Requirements
+
+* `easydict`
+* `argparse`
+
+## Installation
+
+Ensure that you have `easydict` installed. You can install it using pip:
+
+<pre><div class="bg-black rounded-md"><div class="flex items-center relative text-gray-200 bg-gray-800 dark:bg-token-surface-primary px-4 py-2 text-xs font-sans justify-between rounded-t-md"><span class="" data-state="closed"><button class="flex gap-1 items-center"><svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" class="icon-sm"><path fill-rule="evenodd" clip-rule="evenodd" d="M12 4C10.8954 4 10 4.89543 10 6H14C14 4.89543 13.1046 4 12 4ZM8.53513 4C9.22675 2.8044 10.5194 2 12 2C13.4806 2 14.7733 2.8044 15.4649 4H17C18.6569 4 20 5.34315 20 7V19C20 20.6569 18.6569 22 17 22H7C5.34315 22 4 20.6569 4 19V7C4 5.34315 5.34315 4 7 4H8.53513ZM8 6H7C6.44772 6 6 6.44772 6 7V19C6 19.5523 6.44772 20 7 20H17C17.5523 20 18 19.5523 18 19V7C18 6.44772 17.5523 6 17 6H16C16 7.10457 15.1046 8 14 8H10C8.89543 8 8 7.10457 8 6Z" fill="currentColor"></path></svg></button></span></div><div class="p-4 overflow-y-auto"><code class="!whitespace-pre hljs language-bash">pip install easydict
+</code></div></div></pre>
+
+## Usage
+
+### Defining Arguments
+
+First, define your arguments in a dictionary format. For example:
+
+<pre><div class="bg-black rounded-md"><div class="flex items-center relative text-gray-200 bg-gray-800 dark:bg-token-surface-primary px-4 py-2 text-xs font-sans justify-between rounded-t-md"><span class="" data-state="closed"><button class="flex gap-1 items-center"><svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" class="icon-sm"><path fill-rule="evenodd" clip-rule="evenodd" d="M12 4C10.8954 4 10 4.89543 10 6H14C14 4.89543 13.1046 4 12 4ZM8.53513 4C9.22675 2.8044 10.5194 2 12 2C13.4806 2 14.7733 2.8044 15.4649 4H17C18.6569 4 20 5.34315 20 7V19C20 20.6569 18.6569 22 17 22H7C5.34315 22 4 20.6569 4 19V7C4 5.34315 5.34315 4 7 4H8.53513ZM8 6H7C6.44772 6 6 6.44772 6 7V19C6 19.5523 6.44772 20 7 20H17C17.5523 20 18 19.5523 18 19V7C18 6.44772 17.5523 6 17 6H16C16 7.10457 15.1046 8 14 8H10C8.89543 8 8 7.10457 8 6Z" fill="currentColor"></path></svg></button></span></div><div class="p-4 overflow-y-auto"><code class="!whitespace-pre hljs language-python">args_dict = {
+    "arg1": value1,
+    "arg2": value2,
+    // Add more arguments as needed
+}
+</code></div></div></pre>
+
+### Parsing Arguments
+
+Then, simply call the `ipython_args` function with your arguments dictionary:
+
+<pre><div class="bg-black rounded-md"><div class="flex items-center relative text-gray-200 bg-gray-800 dark:bg-token-surface-primary px-4 py-2 text-xs font-sans justify-between rounded-t-md"><span class="" data-state="closed"><button class="flex gap-1 items-center"><svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" class="icon-sm"><path fill-rule="evenodd" clip-rule="evenodd" d="M12 4C10.8954 4 10 4.89543 10 6H14C14 4.89543 13.1046 4 12 4ZM8.53513 4C9.22675 2.8044 10.5194 2 12 2C13.4806 2 14.7733 2.8044 15.4649 4H17C18.6569 4 20 5.34315 20 7V19C20 20.6569 18.6569 22 17 22H7C5.34315 22 4 20.6569 4 19V7C4 5.34315 5.34315 4 7 4H8.53513ZM8 6H7C6.44772 6 6 6.44772 6 7V19C6 19.5523 6.44772 20 7 20H17C17.5523 20 18 19.5523 18 19V7C18 6.44772 17.5523 6 17 6H16C16 7.10457 15.1046 8 14 8H10C8.89543 8 8 7.10457 8 6Z" fill="currentColor"></path></svg></button></span></div><div class="p-4 overflow-y-auto"><code class="!whitespace-pre hljs language-python">args = ipython_args(args_dict)
+</code></div></div></pre>
+
+In a Jupyter notebook environment, `args` will be an `EasyDict` object, allowing you to access arguments using dot notation (`args.arg1`). In a standard script, `args` will be the usual `argparse.Namespace` object.
+
+### Checking Environment
+
+The `is_notebook` function can be used independently to check if the code is running in a Jupyter notebook environment.
+
+## Example
+
+Here's a simple example demonstrating how to use this module:
+
+<pre><div class="bg-black rounded-md"><div class="flex items-center relative text-gray-200 bg-gray-800 dark:bg-token-surface-primary px-4 py-2 text-xs font-sans justify-between rounded-t-md"><span class="" data-state="closed"><button class="flex gap-1 items-center"><svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" class="icon-sm"><path fill-rule="evenodd" clip-rule="evenodd" d="M12 4C10.8954 4 10 4.89543 10 6H14C14 4.89543 13.1046 4 12 4ZM8.53513 4C9.22675 2.8044 10.5194 2 12 2C13.4806 2 14.7733 2.8044 15.4649 4H17C18.6569 4 20 5.34315 20 7V19C20 20.6569 18.6569 22 17 22H7C5.34315 22 4 20.6569 4 19V7C4 5.34315 5.34315 4 7 4H8.53513ZM8 6H7C6.44772 6 6 6.44772 6 7V19C6 19.5523 6.44772 20 7 20H17C17.5523 20 18 19.5523 18 19V7C18 6.44772 17.5523 6 17 6H16C16 7.10457 15.1046 8 14 8H10C8.89543 8 8 7.10457 8 6Z" fill="currentColor"></path></svg></button></span></div><div class="p-4 overflow-y-auto"><code class="!whitespace-pre hljs language-python">from ipython_args import ipython_args
+
+# Define your arguments here
+args_dict = {
+    "epoch": 10,
+    "learning_rate": 0.001
+}
+
+# Parse arguments
+args = ipython_args(args_dict)
+
+# Accessing arguments
+print(args.epoch)
+print(args.learning_rate)
+</code></div></div></pre>
+
+You can use is_notebook function to check the environment is notebook or not
+
+<pre><div class="bg-black rounded-md"><div class="flex items-center relative text-gray-200 bg-gray-800 dark:bg-token-surface-primary px-4 py-2 text-xs font-sans justify-between rounded-t-md"><span class="" data-state="closed"><button class="flex gap-1 items-center"><svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" class="icon-sm"><path fill-rule="evenodd" clip-rule="evenodd" d="M12 4C10.8954 4 10 4.89543 10 6H14C14 4.89543 13.1046 4 12 4ZM8.53513 4C9.22675 2.8044 10.5194 2 12 2C13.4806 2 14.7733 2.8044 15.4649 4H17C18.6569 4 20 5.34315 20 7V19C20 20.6569 18.6569 22 17 22H7C5.34315 22 4 20.6569 4 19V7C4 5.34315 5.34315 4 7 4H8.53513ZM8 6H7C6.44772 6 6 6.44772 6 7V19C6 19.5523 6.44772 20 7 20H17C17.5523 20 18 19.5523 18 19V7C18 6.44772 17.5523 6 17 6H16C16 7.10457 15.1046 8 14 8H10C8.89543 8 8 7.10457 8 6Z" fill="currentColor"></path></svg></button></span></div><div class="p-4 overflow-y-auto"><code class="!whitespace-pre hljs language-python">from ipython_args import is_notebook
+
+# Check whether the current environment is notebook shell or not
+current_env_notebook = is_notebook())
+</code></div></div></pre>
+
+## Contributing & Acknowledgements
+
+Thanks for professor Dr. Lee, Soo-Hong who encourage me to upload the project.
+
+
+This projects are side-project of the National Research Foundation of Korea, ‘Development of a 2-axis ankle exoskeleton robot to identify intentions using deep learning-based EMG images’ (No.2021R1I1A205215811)
+
+## License
+
+This project is open-source and available under the [MIT License]().
+
+Copyright (c) 2018 The Python Packaging Authority
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `ipython_args-1.0.2/setup.py` & `ipython_args-1.0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,34 @@
-from setuptools import setup, find_packages
-
-setup(
-    name='ipython_args',  # A suitable name for your package
-    version='1.0.2',              # Starting with version 1.0.0
-    author='Kim, Won-Joong',           # Replace with your name
-    author_email='wonjoong11@yonsei.ac.kr',  # Replace with your email
-    description='A utility for seamless argument parsing in IPython notebooks and Python scripts.',  # Short description
-    long_description=open('README.md').read(),
-    long_description_content_type='text/markdown',
-    url='https://github.com/qkaTlehdrnf/IpythonArguments',  # Replace with your repository URL
-    packages=find_packages(exclude=('tests', 'docs', 'upload_pypi_package.txt')),
-    install_requires=[
-        'easydict',  # The code depends on easydict
-        'ipython',   # Assuming IPython is a dependency, given the use of get_ipython
-    ],
-    classifiers=[
-        'Development Status :: 4 - Beta',   # Assuming the project is in a beta stage
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',  # Assuming MIT License
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Framework :: IPython',
-        'Topic :: Software Development :: Libraries :: Python Modules',
-    ],
-    python_requires='>=3.4',  # Specifying compatible Python versions
-)
+from setuptools import setup, find_packages
+
+setup(
+    name='ipython_args',  # A suitable name for your package
+    version='1.0.3',              # Starting with version 1.0.0
+    author='Kim, Won-Joong',           # Replace with your name
+    author_email='wonjoong11@yonsei.ac.kr',  # Replace with your email
+    description='A utility for seamless argument parsing in IPython notebooks and Python scripts.',  # Short description
+    long_description=open('README.md',encoding='utf-8').read(),
+    long_description_content_type='text/markdown',
+    url='https://github.com/qkaTlehdrnf/IpythonArguments',  # Replace with your repository URL
+    packages=find_packages(exclude=('tests', 'docs', 'upload_pypi_package.txt')),
+    install_requires=[
+        'easydict',  # The code depends on easydict
+        'ipython',   # Assuming IPython is a dependency, given the use of get_ipython
+        'ipykernel'
+    ],
+    classifiers=[
+        'Development Status :: 4 - Beta',   # Assuming the project is in a beta stage
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: MIT License',  # Assuming MIT License
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.4',
+        'Programming Language :: Python :: 3.5',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Framework :: IPython',
+        'Topic :: Software Development :: Libraries :: Python Modules',
+    ],
+    python_requires='>=3.4',  # Specifying compatible Python versions
+)
```

