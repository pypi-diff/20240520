# Comparing `tmp/ryvencore-0.4.0a9.tar.gz` & `tmp/ryvencore-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ryvencore-0.4.0a9.tar", last modified: Sat Oct 22 05:09:24 2022, max compression
+gzip compressed data, was "ryvencore-0.5.0.tar", last modified: Mon May 20 15:36:52 2024, max compression
```

## Comparing `ryvencore-0.4.0a9.tar` & `ryvencore-0.5.0.tar`

### file list

```diff
@@ -1,48 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 05:09:24.302629 ryvencore-0.4.0a9/
--rw-r--r--   0 runner    (1001) docker     (121)    26526 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2827 2022-10-22 05:09:24.302629 ryvencore-0.4.0a9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2284 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 05:09:24.298629 ryvencore-0.4.0a9/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      638 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 05:09:24.298629 ryvencore-0.4.0a9/docs/img/
--rw-r--r--   0 runner    (1001) docker     (121)    71305 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/docs/img/logo.png
--rw-r--r--   0 runner    (1001) docker     (121)      838 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 05:09:24.298629 ryvencore-0.4.0a9/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 05:09:24.298629 ryvencore-0.4.0a9/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/docs/source/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (121)     2488 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      409 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      594 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/docs/source/ryvencore.addons.default.rst
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/docs/source/ryvencore.addons.rst
--rw-r--r--   0 runner    (1001) docker     (121)      923 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/docs/source/ryvencore.rst
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 05:09:24.298629 ryvencore-0.4.0a9/ryvencore/
--rw-r--r--   0 runner    (1001) docker     (121)     3052 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/ryvencore/AddOn.py
--rw-r--r--   0 runner    (1001) docker     (121)     3610 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/ryvencore/Base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3336 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/ryvencore/Data.py
--rw-r--r--   0 runner    (1001) docker     (121)    14780 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/ryvencore/Flow.py
--rw-r--r--   0 runner    (1001) docker     (121)    11022 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/ryvencore/FlowExecutor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1350 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/ryvencore/InfoMsgs.py
--rw-r--r--   0 runner    (1001) docker     (121)    12873 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/ryvencore/Node.py
--rw-r--r--   0 runner    (1001) docker     (121)     1271 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/ryvencore/NodePort.py
--rw-r--r--   0 runner    (1001) docker     (121)      768 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/ryvencore/NodePortType.py
--rw-r--r--   0 runner    (1001) docker     (121)      896 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/ryvencore/RC.py
--rw-r--r--   0 runner    (1001) docker     (121)     2408 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/ryvencore/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     5707 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/ryvencore/Session.py
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/ryvencore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 05:09:24.302629 ryvencore-0.4.0a9/ryvencore/addons/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/ryvencore/addons/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 05:09:24.302629 ryvencore-0.4.0a9/ryvencore/addons/default/
--rw-r--r--   0 runner    (1001) docker     (121)     6651 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/ryvencore/addons/default/DTypes.py
--rw-r--r--   0 runner    (1001) docker     (121)     2881 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/ryvencore/addons/default/Logging.py
--rw-r--r--   0 runner    (1001) docker     (121)     6733 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/ryvencore/addons/default/Variables.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/ryvencore/addons/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2230 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/ryvencore/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 05:09:24.302629 ryvencore-0.4.0a9/ryvencore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2827 2022-10-22 05:09:24.000000 ryvencore-0.4.0a9/ryvencore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      874 2022-10-22 05:09:24.000000 ryvencore-0.4.0a9/ryvencore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-22 05:09:24.000000 ryvencore-0.4.0a9/ryvencore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-10-22 05:09:24.000000 ryvencore-0.4.0a9/ryvencore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      661 2022-10-22 05:09:24.302629 ryvencore-0.4.0a9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:36:52.017731 ryvencore-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-05-20 15:36:48.000000 ryvencore-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-20 15:36:48.000000 ryvencore-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-20 15:36:52.017731 ryvencore-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-20 15:36:48.000000 ryvencore-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:36:52.013731 ryvencore-0.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-20 15:36:48.000000 ryvencore-0.5.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-20 15:36:48.000000 ryvencore-0.5.0/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:36:52.013731 ryvencore-0.5.0/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    71305 2024-05-20 15:36:48.000000 ryvencore-0.5.0/docs/img/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-20 15:36:48.000000 ryvencore-0.5.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-20 15:36:48.000000 ryvencore-0.5.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:36:52.013731 ryvencore-0.5.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:36:52.013731 ryvencore-0.5.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-20 15:36:48.000000 ryvencore-0.5.0/docs/source/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-20 15:36:48.000000 ryvencore-0.5.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-20 15:36:48.000000 ryvencore-0.5.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-20 15:36:48.000000 ryvencore-0.5.0/docs/source/ryvencore.addons.default.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-20 15:36:48.000000 ryvencore-0.5.0/docs/source/ryvencore.addons.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-20 15:36:48.000000 ryvencore-0.5.0/docs/source/ryvencore.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-20 15:36:48.000000 ryvencore-0.5.0/docs/source/setup_cython.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:36:52.017731 ryvencore-0.5.0/ryvencore/
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-05-20 15:36:48.000000 ryvencore-0.5.0/ryvencore/AddOn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5977 2024-05-20 15:36:48.000000 ryvencore-0.5.0/ryvencore/Base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-05-20 15:36:48.000000 ryvencore-0.5.0/ryvencore/Data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18457 2024-05-20 15:36:48.000000 ryvencore-0.5.0/ryvencore/Flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11519 2024-05-20 15:36:48.000000 ryvencore-0.5.0/ryvencore/FlowExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-20 15:36:48.000000 ryvencore-0.5.0/ryvencore/InfoMsgs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14238 2024-05-20 15:36:48.000000 ryvencore-0.5.0/ryvencore/Node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-20 15:36:48.000000 ryvencore-0.5.0/ryvencore/NodePort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-20 15:36:48.000000 ryvencore-0.5.0/ryvencore/NodePortType.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-20 15:36:48.000000 ryvencore-0.5.0/ryvencore/RC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-20 15:36:48.000000 ryvencore-0.5.0/ryvencore/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-05-20 15:36:48.000000 ryvencore-0.5.0/ryvencore/Session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-20 15:36:48.000000 ryvencore-0.5.0/ryvencore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:36:52.017731 ryvencore-0.5.0/ryvencore/addons/
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-20 15:36:48.000000 ryvencore-0.5.0/ryvencore/addons/Logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10035 2024-05-20 15:36:48.000000 ryvencore-0.5.0/ryvencore/addons/Variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:36:48.000000 ryvencore-0.5.0/ryvencore/addons/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:36:52.017731 ryvencore-0.5.0/ryvencore/addons/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)     6746 2024-05-20 15:36:48.000000 ryvencore-0.5.0/ryvencore/addons/legacy/DTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:36:48.000000 ryvencore-0.5.0/ryvencore/addons/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:36:48.000000 ryvencore-0.5.0/ryvencore/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-05-20 15:36:48.000000 ryvencore-0.5.0/ryvencore/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:36:52.017731 ryvencore-0.5.0/ryvencore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-20 15:36:51.000000 ryvencore-0.5.0/ryvencore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-20 15:36:52.000000 ryvencore-0.5.0/ryvencore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 15:36:51.000000 ryvencore-0.5.0/ryvencore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-20 15:36:52.000000 ryvencore-0.5.0/ryvencore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-20 15:36:52.000000 ryvencore-0.5.0/ryvencore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-20 15:36:52.021731 ryvencore-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 15:36:48.000000 ryvencore-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:36:52.017731 ryvencore-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:36:48.000000 ryvencore-0.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-20 15:36:48.000000 ryvencore-0.5.0/tests/data_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-05-20 15:36:48.000000 ryvencore-0.5.0/tests/data_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-20 15:36:48.000000 ryvencore-0.5.0/tests/exec_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-20 15:36:48.000000 ryvencore-0.5.0/tests/logging-addon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-20 15:36:48.000000 ryvencore-0.5.0/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-20 15:36:48.000000 ryvencore-0.5.0/tests/variables-addon.py
```

### Comparing `ryvencore-0.4.0a9/LICENSE` & `ryvencore-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ryvencore-0.4.0a9/PKG-INFO` & `ryvencore-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: ryvencore
-Version: 0.4.0a9
+Version: 0.5.0
 Summary: Python backend for node editor-like graph-based processing
 Home-page: https://github.com/leon-thomm/ryvencore
 Author: Leon Thomm
 Author-email: l.thomm@mailbox.org
 Project-URL: Website, https://ryven.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: importlib_metadata; python_version < "3.8"
+Requires-Dist: packaging
 
 
 <p align="center">
   <img src="./docs/img/logo.png" alt="drawing" width="70%"/>
 </p>
 
 An experimental Python library for graph-based processing, designed for flow-based/node-based visual scripting editors. It is the backbone of the [Ryven](https://github.com/leon-thomm/Ryven) project, but it can very much be used in other contexts as well.
 
-While ryvencore is written purely in Python, it is very lightweight and highly compatible. It can be compiled with Cython, see the `setup_cython.py` file. The performance seems comparable so far, but the code hasn't been optimized for Cython yet, so there might be a lot of potential. Please consider contributing. [Pyodide](https://github.com/pyodide/pyodide) provides a WebAssembly port of ryvencore.
+While ryvencore is written purely in Python, it is very lightweight and highly compatible. It can be compiled with Cython, see the `setup_cython.py` file. The performance seems comparable so far, but the code hasn't been optimized for Cython yet, so there might be a lot of potential. Please consider contributing. ryvencore also seems compatible with most Python ports to WebAssembly, even the Cython compiled ryvencore.
 
 ### Installation
 
 ```
 pip install ryvencore
 ```
```

### Comparing `ryvencore-0.4.0a9/README.md` & `ryvencore-0.5.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <p align="center">
   <img src="./docs/img/logo.png" alt="drawing" width="70%"/>
 </p>
 
 An experimental Python library for graph-based processing, designed for flow-based/node-based visual scripting editors. It is the backbone of the [Ryven](https://github.com/leon-thomm/Ryven) project, but it can very much be used in other contexts as well.
 
-While ryvencore is written purely in Python, it is very lightweight and highly compatible. It can be compiled with Cython, see the `setup_cython.py` file. The performance seems comparable so far, but the code hasn't been optimized for Cython yet, so there might be a lot of potential. Please consider contributing. [Pyodide](https://github.com/pyodide/pyodide) provides a WebAssembly port of ryvencore.
+While ryvencore is written purely in Python, it is very lightweight and highly compatible. It can be compiled with Cython, see the `setup_cython.py` file. The performance seems comparable so far, but the code hasn't been optimized for Cython yet, so there might be a lot of potential. Please consider contributing. ryvencore also seems compatible with most Python ports to WebAssembly, even the Cython compiled ryvencore.
 
 ### Installation
 
 ```
 pip install ryvencore
 ```
```

### Comparing `ryvencore-0.4.0a9/docs/Makefile` & `ryvencore-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ryvencore-0.4.0a9/docs/img/logo.png` & `ryvencore-0.5.0/docs/img/logo.png`

 * *Files identical despite different names*

### Comparing `ryvencore-0.4.0a9/docs/make.bat` & `ryvencore-0.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ryvencore-0.4.0a9/docs/source/conf.py` & `ryvencore-0.5.0/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 import os
 import sys
 sys.path.insert(0, os.path.abspath('../..'))
 
 from ryvencore import *
+from setup_cython import *
 from importlib.metadata import metadata
 
 # -- Project information -----------------------------------------------------
 
 project = 'ryvencore'
 copyright = '2022, Leon Thomm'
 author = 'Leon Thomm'
@@ -32,14 +33,15 @@
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.napoleon',
     'sphinx.ext.viewcode',
+    'sphinx.ext.doctest',
 ]
 
 add_module_names = False
 
 # autodoc options
 autodoc_member_order = 'bysource'
```

### Comparing `ryvencore-0.4.0a9/docs/source/ryvencore.addons.default.rst` & `ryvencore-0.5.0/docs/source/ryvencore.addons.default.rst`

 * *Files identical despite different names*

### Comparing `ryvencore-0.4.0a9/ryvencore/Flow.py` & `ryvencore-0.5.0/ryvencore/Flow.py`

 * *Files 18% similar despite different names*

```diff
@@ -84,72 +84,89 @@
 is both efficient and easy to use.
 
 Assumptions:
 
     * no non-terminating feedback loops with exec connections
 
 """
-
 from .Base import Base, Event
 from .Data import Data
 from .FlowExecutor import DataFlowNaive, DataFlowOptimized, FlowExecutor, executor_from_flow_alg
 from .Node import Node
 from .NodePort import NodeOutput, NodeInput
 from .RC import FlowAlg, PortObjPos
-from .utils import node_from_identifier, serialize, deserialize
-from typing import List, Dict, Optional, Tuple
+from .utils import *
+from typing import List, Dict, Optional, Tuple, Type
 
 
 class Flow(Base):
     """
     Manages all abstract flow components (nodes, edges, executors, etc.)
     and exposes methods for modification.
     """
 
-    def __init__(self, session, title):
+    def __init__(self, session, title: str):
         Base.__init__(self)
 
         # events
         self.node_added = Event(Node)
         self.node_removed = Event(Node)
+        self.node_created = Event(Node)
         self.connection_added = Event((NodeOutput, NodeInput))        # Event(Connection)
         self.connection_removed = Event((NodeOutput, NodeInput))      # Event (Connection)
 
         self.connection_request_valid = Event(bool)
         self.nodes_created_from_data = Event(list)
         self.connections_created_from_data = Event(list)
 
         self.algorithm_mode_changed = Event(str)
 
+        # connect events to add-ons
+        for addon in session.addons.values():
+            addon.connect_flow_events(self)
+
         # general attributes
         self.session = session
         self.title = title
-        self.nodes: [Node] = []
+        self.nodes: List[Node] = []
+        self.load_data: Optional[Dict] = None
 
-        self.node_successors = {}   # additional data structure for executors
-        self.graph_adj = {}         # directed adjacency list relating node ports
-        self.graph_adj_rev = {}     # reverse adjacency; reverse of graph_adj
+        self.node_successors: Dict[Node, List[Node]] = {}   # additional data structure for executors
+        self.graph_adj: Dict[NodeOutput, List[NodeInput]] = {}         # directed adjacency list relating node ports
+        self.graph_adj_rev: Dict[NodeInput, Optional[NodeOutput]] = {}     # reverse adjacency; reverse of graph_adj
 
         self.alg_mode = FlowAlg.DATA
         self.executor: FlowExecutor = executor_from_flow_alg(self.alg_mode)(self)
 
-    def load(self, data: dict):
+    def load(self, data: Dict):
         """Loading a flow from data as previously returned by ``Flow.data()``."""
         super().load(data)
+        self.load_data = data
 
         # set algorithm mode
         self.alg_mode = FlowAlg.from_str(data['algorithm mode'])
 
         # build flow
+        self.load_components(data['nodes'], data['connections'], data['output data'])
+
 
-        new_nodes = self._create_nodes_from_data(data['nodes'])
+    def load_components(self, nodes_data, conns_data, output_data):
+        """Loading nodes and their connections from data as previously returned
+        by :code:`Flow.data()`. This method will call :code:`Node.rebuilt()` after
+        connections are established on all nodes.
+        Returns the new nodes and connections."""
 
-        self._set_output_values_from_data(new_nodes, data['output data'])
+        new_nodes = self._create_nodes_from_data(nodes_data)
+        self._set_output_values_from_data(new_nodes, output_data)
+        new_conns = self._connect_nodes_from_data(new_nodes, conns_data)
 
-        self._connect_nodes_from_data(new_nodes, data['connections'])
+        for n in new_nodes:
+            n.rebuilt()
+
+        return new_nodes, new_conns
 
 
     def _create_nodes_from_data(self, nodes_data: List):
         """create nodes from nodes_data as previously returned by data()"""
 
         nodes = []
 
@@ -170,81 +187,143 @@
 
 
     def _set_output_values_from_data(self, nodes: List[Node], data: List):
         for d in data:
             indices = d['dependent node outputs']
             indices_paired = zip(indices[0::2], indices[1::2])
             for node_index, output_index in indices_paired:
+
+                # find Data class
+                dt_id = d['data']['identifier']
+                if dt_id == 'Data':
+                    data_type = Data
+                else:
+                    data_type = self.session.data_types.get(dt_id)
+
+                    if data_type is None:
+                        print_err(f'Tried to use unregistered Data type '
+                                  f'{dt_id} while loading. Skipping. '
+                                  f'Please register data types before using them.')
+                        continue
+
                 nodes[node_index].outputs[output_index].val = \
-                    Data(load_from=deserialize(d['data']))
+                    data_type(load_from=d['data'])
 
 
-    def create_node(self, node_class, data=None):
+    def create_node(self, node_class: Type[Node], data=None):
         """Creates, adds and returns a new node object"""
 
-        node = node_class((self, self.session, data))
+        if node_class not in self.session.nodes:
+            print_err(f'Node class {node_class} not in session nodes')
+            return
+
+        # instantiate node
+        node = node_class((self, self.session))
+        # connect to node events
+        node.input_added.sub(lambda n, i, inp: self.add_node_input(n, inp), nice=-5)
+        node.output_added.sub(lambda n, i, out: self.add_node_output(n, out), nice=-5)
+        node.input_removed.sub(lambda n, i, inp: self.remove_node_input(n, inp), nice=-5)
+        node.output_removed.sub(lambda n, i, out: self.remove_node_output(n, out), nice=-5)
+        # initialize node ports
         node.initialize()
-        self.add_node(node)
+        # load node
+        if data is not None:
+            node.load(data)
 
-        # notify addons
-        for addon in self.session.addons.values():
-            addon._on_node_created(self, node)
+        self.node_created.emit(node)
+        self.add_node(node)
 
         return node
 
 
     def add_node(self, node: Node):
         """
         Places the node object in the graph, Stores it, and causes the node's
         ``Node.place_event()`` to be executed. ``Flow.create_node()`` automatically
         adds the node already, so no need to call this manually.
         """
 
         self.nodes.append(node)
 
         self.node_successors[node] = []
+
+        # catch up on node ports
+        # notice that add_node_output() and add_node_input() are called by Node.
+        # but it's ignored when the node is not currently placed in the flow
         for out in node.outputs:
-            self.graph_adj[out] = []
+            self.add_node_output(node, out, False)
+            # self.graph_adj[out] = []
         for inp in node.inputs:
-            self.graph_adj_rev[inp] = None
+            self.add_node_input(node, inp, False)
+            # self.graph_adj_rev[inp] = None
 
         node.after_placement()
         self._flow_changed()
 
-        # notify addons
-        for addon in self.session.addons.values():
-            addon._on_node_added(self, node)
-
         self.node_added.emit(node)
 
 
     def remove_node(self, node: Node):
         """
         Removes a node from the flow without deleting it. Can be added again
         with ``Flow.add_node()``.
         """
 
         node.prepare_removal()
         self.nodes.remove(node)
 
         del self.node_successors[node]
         for out in node.outputs:
-            del self.graph_adj[out]
+            self.remove_node_output(node, out, False)
+            # del self.graph_adj[out]
         for inp in node.inputs:
-            del self.graph_adj_rev[inp]
+            self.remove_node_input(node, inp, False)
+            # del self.graph_adj_rev[inp]
 
         self._flow_changed()
 
         # notify addons
         for addon in self.session.addons.values():
-            addon._on_node_removed(self, node)
+            addon.on_node_removed(node)
 
         self.node_removed.emit(node)
 
 
+    def add_node_input(self, node: Node, inp: NodeInput, _call_flow_changed=True):
+        """updates internal data structures"""
+        if node in self.node_successors:
+            self.graph_adj_rev[inp] = None
+            if _call_flow_changed:
+                self._flow_changed()
+
+
+    def add_node_output(self, node: Node, out: NodeOutput, _call_flow_changed=True):
+        """updates internal data structures."""
+        if node in self.node_successors:
+            self.graph_adj[out] = []
+            if _call_flow_changed:
+                self._flow_changed()
+
+
+    def remove_node_input(self, node: Node, inp: NodeInput, _call_flow_changed=True):
+        """updates internal data structures."""
+        if node in self.node_successors:
+            del self.graph_adj_rev[inp]
+            if _call_flow_changed:
+                self._flow_changed()
+
+
+    def remove_node_output(self, node: Node, out: NodeOutput, _call_flow_changed=True):
+        """updates internal data structures."""
+        if node in self.node_successors:
+            del self.graph_adj[out]
+            if _call_flow_changed:
+                self._flow_changed()
+
+
     def _connect_nodes_from_data(self, nodes: List[Node], data: List):
         connections = []
 
         for c in data:
 
             c_parent_node_index = c['parent node index']
             c_connected_node_index = c['connected node']
@@ -263,58 +342,70 @@
                     ))
 
         self.connections_created_from_data.emit(connections)
 
         return connections
 
 
-    def check_connection_validity(self, p1: NodeOutput, p2: NodeInput) -> bool:
+    def check_connection_validity(self, c: Tuple[NodeOutput, NodeInput]) -> bool:
         """
         Checks whether a considered connect action is legal.
         """
 
+        out, inp = c
+
         valid = True
 
-        if p1.node == p2.node:
+        if out.node == inp.node:
             valid = False
 
-        if p1.io_pos == p2.io_pos or p1.type_ != p2.type_:
+        if out.io_pos == inp.io_pos or out.type_ != inp.type_:
+            valid = False
+
+        if out.io_pos != PortObjPos.OUTPUT:
             valid = False
 
         self.connection_request_valid.emit(valid)
 
         return valid
 
 
-    def connect_nodes(self, p1: NodeOutput, p2: NodeInput, silent: bool = False) -> Optional[Tuple[NodeOutput, NodeInput]]:
+    def connect_nodes(self, out: NodeOutput, inp: NodeInput, silent=False) -> Optional[Tuple[NodeOutput, NodeInput]]:
         """
-        Connects nodes or disconnects them if they are already connected.
-
-        TODO: change this; rather introduce ``disconnect_nodes()`` instead
+        Connects two node ports. Returns the connection if successful, None otherwise.
         """
 
-        if not self.check_connection_validity(p1, p2):
+        if not self.check_connection_validity((out, inp)):
+            print_err('Invalid connect request.')
             return None
 
-        out = p1
-        inp = p2
-        if out.io_pos == PortObjPos.INPUT:
-            out, inp = inp, out
-
         if inp in self.graph_adj[out]:
-            # disconnect
-            self.remove_connection((out, inp))
             return None
 
         self.add_connection((out, inp), silent=silent)
 
         return out, inp
 
 
-    def add_connection(self, c: Tuple[NodeOutput, NodeInput], silent: bool = False):
+    def disconnect_nodes(self, out: NodeOutput, inp: NodeInput, silent=False):
+        """
+        Disconnects two node ports.
+        """
+
+        if not self.check_connection_validity((out, inp)):
+            print_err('Invalid disconnect request.')
+            return
+
+        if inp not in self.graph_adj[out]:
+            return
+
+        self.remove_connection((out, inp), silent=silent)
+
+
+    def add_connection(self, c: Tuple[NodeOutput, NodeInput], silent=False):
         """
         Adds an edge between two node ports.
         """
 
         out, inp = c
 
         self.graph_adj[out].append(inp)
@@ -325,43 +416,43 @@
 
 
         self.executor.conn_added(out, inp, silent=silent)
 
         self.connection_added.emit((out, inp))
 
 
-    def remove_connection(self, c: Tuple[NodeOutput, NodeInput]):
+    def remove_connection(self, c: Tuple[NodeOutput, NodeInput], silent=False):
         """
         Removes an edge.
         """
 
         out, inp = c
 
         self.graph_adj[out].remove(inp)
         self.graph_adj_rev[inp] = None
 
         self.node_successors[out.node].remove(inp.node)
         self._flow_changed()
 
-        self.executor.conn_removed(out, inp)
+        self.executor.conn_removed(out, inp, silent=silent)
 #
         self.connection_removed.emit((out, inp))
 
 
     def connected_inputs(self, out: NodeOutput) -> List[NodeInput]:
         """
         Returns a list of all connected inputs to the given output port.
         """
         return self.graph_adj[out]
 
 
     def connected_output(self, inp: NodeInput) -> Optional[NodeOutput]:
         """
         Returns the connected output port to the given input port, or
-        ``None`` if it is not connected.
+        :code:`None` if it is not connected.
         """
         return self.graph_adj_rev[inp]
 
 
     def algorithm_mode(self) -> str:
         """
         Returns the current algorithm mode of the flow as string.
@@ -392,22 +483,21 @@
 
 
     def data(self) -> dict:
         """
         Serializes the flow: returns a JSON compatible dict containing all
         data of the flow.
         """
-        d = super().data()
-        d.update({
+        return {
+            **super().data(),
             'algorithm mode': FlowAlg.str(self.alg_mode),
             'nodes': self._gen_nodes_data(self.nodes),
             'connections': self._gen_conns_data(self.nodes),
             'output data': self._gen_output_data(self.nodes),
-        })
-        return d
+        }
 
 
     def _gen_nodes_data(self, nodes: List[Node]) -> List[dict]:
         """Returns the data dicts of the nodes given"""
 
         return [n.data() for n in nodes]
 
@@ -433,21 +523,21 @@
 
         return data
 
 
     def _gen_output_data(self, nodes: List[Node]) -> List[Dict]:
         """Serializes output data of the nodes"""
 
-        outputs_data = {}
+        outputs_data: Dict[Data, Dict] = {}
 
         for i_n, n in enumerate(nodes):
             for i_o, out in enumerate(n.outputs):
                 d = out.val
                 if isinstance(d, Data) and d not in outputs_data:
                     outputs_data[d] = {
-                        'data': serialize(d.get_data()),
+                        'data': d.data(),
                         'dependent node outputs': [i_n, i_o],
                     }
                 elif isinstance(d, Data):
                     outputs_data[d]['dependent node outputs'] += [i_n, i_o]
 
         return list(outputs_data.values())
```

### Comparing `ryvencore-0.4.0a9/ryvencore/FlowExecutor.py` & `ryvencore-0.5.0/ryvencore/FlowExecutor.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 """
 The flow executors are responsible for executing the flow. They have access to
 the flow as well as the nodes' internals and are able to perform optimizations.
 """
+# prevent cyclic imports
+from __future__ import annotations
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    from .Flow import Flow
+    from .Node import Node
+
+from typing import Optional
+
 from .Data import Data
+from .NodePort import NodeOutput, NodeInput
 from .RC import FlowAlg
 
 
 """
 graph_adjacency = {
     node_output: [node_input],    
     node_input:  node_output | None
@@ -15,40 +25,40 @@
 
 
 class FlowExecutor:
     """
     Base class for special flow execution algorithms.
     """
 
-    def __init__(self, flow):
+    def __init__(self, flow: Flow):
         self.flow = flow
         self.flow_changed = True
         self.graph = self.flow.graph_adj
         self.graph_rev = self.flow.graph_adj_rev
 
     # Node.update() =>
-    def update_node(self, node, inp):
+    def update_node(self, node: Node, inp: int):
         pass
 
     # Node.input() =>
-    def input(self, node, index):
+    def input(self, node: Node, index: int) -> Optional[Data]:
         pass
 
     # Node.set_output_val() =>
-    def set_output_val(self, node, index, val):
+    def set_output_val(self, node: Node, index: int, val) -> None:
         pass
 
     # Node.exec_output() =>
-    def exec_output(self, node, index):
+    def exec_output(self, node: Node, index: int) -> None:
         pass
 
-    def conn_added(self, out, inp, silent=False):
+    def conn_added(self, out: NodeOutput, inp: NodeInput, silent=False) -> None:
         pass
 
-    def conn_removed(self, out, inp):
+    def conn_removed(self, out: NodeOutput, inp: NodeInput, silent=False) -> None:
         pass
 
 
 class DataFlowNaive(FlowExecutor):
     """
     The naive implementation of data-flow execution. Naive meaning setting a node output
     leads to an immediate update in all successors consecutively. No runtime optimization
@@ -56,78 +66,77 @@
     include "diamonds".
 
     Assumptions for the graph:
     - no non-terminating feedback loops
     """
 
     # Node.update() =>
-    def update_node(self, node, inp):
+    def update_node(self, node: Node, inp: int):
         try:
             node.update_event(inp)
         except Exception as e:
-            node.update_error(e)
+            node.update_err(e)
 
     # Node.input() =>
-    def input(self, node, index):
+    def input(self, node: Node, index: int):
         inp = node.inputs[index]
         conn_out = self.graph_rev[inp]
 
         if conn_out:
             return conn_out.val
         else:
-            return None
+            return inp.default
 
     # Node.set_output_val() =>
-    def set_output_val(self, node, index, data):
+    def set_output_val(self, node: Node, index: int, data):
         out = node.outputs[index]
         if not out.type_ == 'data':
             return
         out.val = data
 
         for inp in self.graph[out]:
             inp.node.update(inp=inp.node.inputs.index(inp))
 
     # Node.exec_output() =>
-    def exec_output(self, node, index):
+    def exec_output(self, node: Node, index: int):
         out = node.outputs[index]
         if not out.type_ == 'exec':
             return
 
         for inp in self.graph[out]:
             inp.node.update(inp=inp.node.inputs.index(inp))
 
-    def conn_added(self, out, inp, silent=False):
+    def conn_added(self, out: NodeOutput, inp: NodeInput, silent=False):
         if not silent:
             # update input
             inp.node.update(inp=inp.node.inputs.index(inp))
 
-    def conn_removed(self, out, inp):
-        # update input
-        inp.node.update(inp=inp.node.inputs.index(inp))
+    def conn_removed(self, out, inp, silent=False):
+        if not silent:
+            # update input
+            inp.node.update(inp=inp.node.inputs.index(inp))
 
 
 class DataFlowOptimized(DataFlowNaive):
     """
+    *(see also documentation in Flow)*
+
     A special flow executor which implements some node functions to optimise flow execution.
     Whenever a new execution is invoked somewhere (some node or output is updated), it
     analyses the graph's connected component (of successors) where the execution was invoked
     and creates a few data structures to reverse engineer how many input
     updates every node possibly receives in this execution. A node's outputs are
     propagated once no input can still receive new data from a predecessor node.
     Therefore, while a node gets updated every time an input receives some data,
     every OUTPUT is only updated ONCE.
     This implies that every connection is activated at most once in an execution.
     This can result in asymptotic speedup in large data flows compared to normal data flow
     execution where any two executed branches which merge again in the future result in two
     complete executions of everything that comes after the merge, which quickly produces
     exponential performance issues.
-
-    Assumptions for the graph:
-
-    - no feedback loops
     """
 
     def __init__(self, flow):
         super().__init__(flow)
 
         self.output_updated = {}
         self.waiting_count = {}
@@ -325,15 +334,15 @@
             self.updated_nodes = {node}
         else:
             self.updated_nodes.add(node)
 
         try:
             node.update_event(inp)
         except Exception as e:
-            node.update_error(e)
+            node.update_err(e)
 
         if execution_starter:
             self.updated_nodes = None
 
     # Node.input() =>
     def input(self, node, index):
         inp = node.inputs[index]
```

### Comparing `ryvencore-0.4.0a9/ryvencore/InfoMsgs.py` & `ryvencore-0.5.0/ryvencore/InfoMsgs.py`

 * *Files identical despite different names*

### Comparing `ryvencore-0.4.0a9/ryvencore/Node.py` & `ryvencore-0.5.0/ryvencore/Node.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,21 @@
+# prevent cyclic imports
+from __future__ import annotations
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    from .Flow import Flow
+    from .Session import Session
+
 import traceback
-from typing import List, Optional
+from typing import Optional, List, Tuple, Dict
 
-from .Base import Base
+from .Base import Base, Event
 
 from .NodePort import NodeInput, NodeOutput
 from .NodePortType import NodeInputType, NodeOutputType
-from .RC import FlowAlg
 from .Data import Data
 from .InfoMsgs import InfoMsgs
 from .utils import serialize, deserialize
 
 
 class Node(Base):
     """
@@ -20,31 +26,31 @@
 
     title = ''
     """the node's title"""
 
     tags: List[str] = []
     """a list of tag strings, often useful for searching etc."""
 
-    version: str = None
+    version: Optional[str] = None
     """version tag, use it!"""
 
     init_inputs: List[NodeInputType] = []
     """list of node input types determining the initial inputs"""
 
     init_outputs: List[NodeOutputType] = []
     """initial outputs list, see ``init_inputs``"""
 
-    identifier: str = None
+    identifier: str
     """unique node identifier string. if not given it will set it to the class name when registering in the session"""
 
     legacy_identifiers: List[str] = []
-    """a list of compatible identifiers, useful if you change the class name (and hence the identifier) to provide 
+    """a list of compatible identifiers, useful when you change the class name (and hence the identifier) to provide 
     backward compatibility to load old projects that rely on the old identifier"""
 
-    identifier_prefix: str = None
+    identifier_prefix: Optional[str] = None
     """becomes part of the identifier if set; can be useful for grouping nodes"""
 
     #
     # INITIALIZATION
     #
 
     @classmethod
@@ -54,104 +60,77 @@
         the identifier prefix is set.
         """
 
         prefix = ''
         if cls.identifier_prefix is not None:
             prefix = cls.identifier_prefix + '.'
 
-        if cls.identifier is None:
+        if not hasattr(cls, 'identifier') or cls.identifier is None:
             cls.identifier = cls.__name__
 
         cls.identifier = prefix + cls.identifier
 
         # notice that we do not touch the legacy identifier fields
 
-    def __init__(self, params):
+    def __init__(self, params: Tuple[Flow, Session]):
         Base.__init__(self)
 
-        self.flow, self.session, self.init_data = params
+        self.flow, self.session = params
         self.inputs: List[NodeInput] = []
         self.outputs: List[NodeOutput] = []
 
-        self.initialized = False
+        self.loaded = False
+        self.load_data = None
 
         self.block_init_updates = False
         self.block_updates = False
 
+        # events
+        self.updating = Event(int)
+        self.update_error = Event(Exception)
+        self.input_added = Event(Node, int, NodeInput)
+        self.input_removed = Event(Node, int, NodeInput)
+        self.output_added = Event(Node, int, NodeOutput)
+        self.output_removed = Event(Node, int, NodeOutput)
+
     def initialize(self):
         """
-        Called by the Flow. This method
-
-        - loads all default properties from initial data if it was provided
-        - sets up inputs and outputs
-        - loads user_data
-
-        It does not crash on exception when loading user_data,
-        as this is not uncommon when developing nodes.
+        Sets up the node ports.
         """
-
-        if self.init_data:  # load from data
-            # setup ports
-            self._setup_ports(self.init_data['inputs'], self.init_data['outputs'])
-
-            # set state
-            if 'additional data' in self.init_data:
-                add_data = self.init_data['additional data']
-            else:   # backwards compatibility
-                add_data = self.init_data
-            self.load_additional_data(add_data)
-
-            try:
-                if 'version' in self.init_data:
-                    version = self.init_data['version']
-                else:  # backwards compatibility
-                    version = None
-
-                self.set_state(deserialize(self.init_data['state data']), version)
-
-            except Exception as e:
-                InfoMsgs.write_err(
-                    'Exception while setting data in', self.title, 'node:', e, ' (was this intended?)')
-
-        else:   # default setup
-
-            # setup ports
-            self._setup_ports()
-
-        self.initialized = True
+        self._setup_ports()
 
     def _setup_ports(self, inputs_data=None, outputs_data=None):
 
         if not inputs_data and not outputs_data:
             # generate initial ports
 
             for i in range(len(self.init_inputs)):
                 inp = self.init_inputs[i]
 
-                self.create_input(inp.label, inp.type_, add_data=self.init_inputs[i].add_data)
+                self.create_input(label=inp.label, type_=inp.type_, default=inp.default)
 
             for o in range(len(self.init_outputs)):
                 out = self.init_outputs[o]
                 self.create_output(out.label, out.type_)
 
         else:
             # load from data
             # initial ports specifications are irrelevant then
 
             for inp in inputs_data:
-                self.create_input(label=inp['label'], type_=inp['type'], add_data=inp)
+                self.create_input(load_from=inp)
 
                 # if 'val' in inp:
                 #     # this means the input is 'data' and did not have any connections,
                 #     # so we saved its value which was probably represented by some widget
                 #     # in the front end which has probably overridden the Node.input() method
                 #     self.inputs[-1].val = deserialize(inp['val'])
 
             for out in outputs_data:
-                self.create_output(out['label'], out['type'])
+                self.create_output(load_from=out)
 
     def after_placement(self):
         """Called from Flow when the nodes gets added."""
 
         self.place_event()
 
     def prepare_removal(self):
@@ -180,18 +159,20 @@
         if self.block_updates:
             InfoMsgs.write('update blocked in', self.title, 'node')
             return
 
         InfoMsgs.write('update in', self.title, 'node on input', inp)
 
         # invoke update_event
+        self.updating.emit(inp)
         self.flow.executor.update_node(self, inp)
 
-    def update_error(self, e):
+    def update_err(self, e):
         InfoMsgs.write_err('EXCEPTION in', self.title, '\n', traceback.format_exc())
+        self.update_error.emit(e)
 
     def input(self, index: int) -> Optional[Data]:
         """
         Returns the data residing at the data input of given index.
 
         Do not call on exec inputs.
         """
@@ -207,15 +188,15 @@
         Do not call on data outputs.
         """
 
         InfoMsgs.write('executing output', index, 'in:', self.title)
 
         self.flow.executor.exec_output(self, index)
 
-    def set_output_val(self, index, data: Data):
+    def set_output_val(self, index: int, data: Data):
         """
         Sets the value of a data output causing activation of all connections in data mode.
         """
         assert isinstance(data, Data), "Output value must be of type ryvencore.Data"
 
         InfoMsgs.write('setting output', index, 'in', self.title)
 
@@ -240,94 +221,107 @@
         pass
 
     def place_event(self):
         """
         *VIRTUAL*
 
         Called once the node object has been fully initialized and placed in the flow.
-        When loading content, ``place_event()`` is executed *before* connections are built,
-        so updating output values here will not cause any other nodes to be updated during loading.
+        When loading content, :code:`place_event()` is executed *before* connections are built.
 
         Notice that this method gets executed *every time* the node is added to the flow, which can happen
-        multiple times for the same object (e.g. due to undo/redo operations).
+        more than once if the node was subsequently removed (e.g. due to undo/redo operations).
         """
 
         pass
 
     def remove_event(self):
         """
         *VIRTUAL*
 
         Called when the node is removed from the flow; useful for stopping threads and timers etc.
         """
 
         pass
 
-    def additional_data(self) -> dict:
+    def additional_data(self) -> Dict:
         """
         *VIRTUAL*
 
         ``additional_data()``/``load_additional_data()`` is almost equivalent to
         ``get_state()``/``set_state()``,
         but it turned out to be useful for frontends to have their own dedicated version,
         so ``get_state()``/``set_state()`` stays clean for all specific node subclasses.
         """
 
         return {}
 
-    def load_additional_data(self, data: dict):
+    def load_additional_data(self, data: Dict):
         """
         *VIRTUAL*
 
         For loading the data returned by ``additional_data()``.
         """
         pass
 
-    def get_state(self) -> dict:
+    def get_state(self) -> Dict:
         """
         *VIRTUAL*
 
         If your node is stateful, implement this method for serialization. It should return a JSON compatible
         dict that encodes your node's state. The dict will be passed to ``set_state()`` when the node is loaded.
         """
         return {}
 
-    def set_state(self, data: dict, version):
+    def set_state(self, data: Dict, version):
         """
         *VIRTUAL*
 
         Opposite of ``get_state()``, reconstruct any custom internal state here.
+        Notice, that add-ons might not yet be fully available here, but in
+        ``place_event()`` the should be.
+        """
+        pass
+
+    def rebuilt(self):
+        """
+        *VIRTUAL*
+
+        If the node was created by loading components in the flow (see :code:`Flow.load_components()`),
+        this method will be called after the node has been added to the graph and incident connections
+        are established.
         """
         pass
 
     """
     
     API
     
     """
 
     #   PORTS
 
-    def create_input(self, label: str = '', type_: str = 'data', add_data={}, insert: int = None):
+    def create_input(self, label: str = '', type_: str = 'data', default: Optional[Data] = None, load_from = None, insert: Optional[int] = None):
         """
         Creates and adds a new input at the end or index ``insert`` if specified.
         """
         # InfoMsgs.write('create_input called')
 
-        inp = NodeInput(
-            node=self,
-            type_=type_,
-            label_str=label,
-            add_data=add_data,
-        )
+        inp = NodeInput(node=self, type_=type_, label_str=label, default=default)
+
+        if load_from is not None:
+            inp.load(load_from)
 
         if insert is not None:
             self.inputs.insert(insert, inp)
+            index = insert
         else:
             self.inputs.append(inp)
+            index = len(self.inputs) - 1
+
+        self.input_added.emit(self, index, inp)
 
         return inp
 
     def rename_input(self, index: int, label: str):
         self.inputs[index].label_str = label
 
     def delete_input(self, index: int):
@@ -340,29 +334,38 @@
         # break all connections
         out = self.flow.connected_output(inp)
         if out is not None:
             self.flow.connect_nodes(out, inp)
 
         self.inputs.remove(inp)
 
-    def create_output(self, label: str = '', type_: str = 'data', insert: int = None):
+        self.input_removed.emit(self, index, inp)
+
+    def create_output(self, label: str = '', type_: str = 'data', load_from=None, insert: Optional[int] = None):
         """
         Creates and adds a new output at the end or index ``insert`` if specified.
         """
 
         out = NodeOutput(
-              node=self,
-              type_=type_,
-              label_str=label
+            node=self,
+            type_=type_,
+            label_str=label,
         )
 
+        if load_from is not None:
+            out.load(load_from)
+
         if insert is not None:
             self.outputs.insert(insert, out)
+            index = insert
         else:
             self.outputs.append(out)
+            index = len(self.outputs) - 1
+
+        self.output_added.emit(self, index, out)
 
         return out
 
     def rename_output(self, index: int, label: str):
         self.outputs[index].label_str = label
 
     def delete_output(self, index: int):
@@ -374,14 +377,16 @@
 
         # break all connections
         for inp in self.flow.connected_inputs(out):
             self.flow.connect_nodes(out, inp)
 
         self.outputs.remove(out)
 
+        self.output_removed.emit(self, index, out)
+
     #   VARIABLES
 
     def get_addon(self, name: str):
         """
         Returns an add-on registered in the session by name, or None if it wasn't found.
         """
         return self.session.addons.get(name)
@@ -406,31 +411,69 @@
 
     """
     
     SERIALIZATION
     
     """
 
-    def data(self) -> dict:
+    def load(self, data):
+        """
+        Initializes the node from the data dict returned by :code:`Node.data()`.
+        Called by the flow, before the node is added to it.
+        It does not crash on exception when loading user_data,
+        as this is not uncommon when developing nodes.
         """
-        Returns all metadata of the node in JSON-compatible dict, including custom state.
-        Used to rebuild the Flow when loading a project or pasting components.
+        super().load(data)
+
+        self.load_data = data
+
+        # setup ports
+        #   remove initial ports
+        self.inputs = []
+        self.outputs = []
+        #   load from data
+        self._setup_ports(data['inputs'], data['outputs'])
+
+        # additional data
+        if 'additional data' in data:
+            add_data = data['additional data']
+        else:   # backwards compatibility
+            add_data = data
+        self.load_additional_data(add_data)
+
+        # set use state
+        try:
+            version = data.get('version')
+            self.set_state(deserialize(data['state data']), version)
+        except Exception as e:
+            InfoMsgs.write_err(
+                f'Exception while setting data in {self.title} node:'
+                f'{e} (was this intended?)')
+
+        self.loaded = True
+
+    def data(self) -> Dict:
+        """
+        Serializes the node's metadata, current configuration, and user state into
+        a JSON-compatible dict, from which the node can be loaded later using
+        :code:`Node.load()`.
         """
 
-        d = super().data()
-        d.update({
+        d = {
+            **super().data(),
+
             'identifier': self.identifier,
-            'version': self.version,
+            'version': self.version,    # this overrides the version field from Base
 
             'state data': serialize(self.get_state()),
             'additional data': self.additional_data(),
 
             'inputs': [i.data() for i in self.inputs],
             'outputs': [o.data() for o in self.outputs],
-        })
+        }
 
         # extend with data from addons
         for name, addon in self.session.addons.items():
             # addons can modify anything, there is no isolation enforcement
-            addon._extend_node_data(self, d)
+            addon.extend_node_data(self, d)
 
         return d
```

### Comparing `ryvencore-0.4.0a9/ryvencore/NodePortType.py` & `ryvencore-0.5.0/ryvencore/NodePortType.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+from typing import Optional
+
+from .Data import Data
+
 
 # TODO: make this a dataclass
 class NodePortType:
     """
     The NodePortBP classes are only placeholders (BP = BluePrint) for the static init_input and
     init_outputs of custom Node classes.
     An instantiated Node's actual inputs and outputs will be of type NodeObjPort (NodeObjInput, NodeObjOutput).
@@ -10,16 +14,16 @@
     def __init__(self, label: str = '', type_: str = 'data'):
 
         self.type_: str = type_
         self.label: str = label
 
 
 class NodeInputType(NodePortType):
-    def __init__(self, label: str = '', type_: str = 'data', add_data={}):
+    def __init__(self, label: str = '', type_: str = 'data', default: Optional[Data] = None):
         super().__init__(label, type_)
 
-        self.add_data = add_data
+        self.default: Optional[Data] = default
 
 
 class NodeOutputType(NodePortType):
     def __init__(self, label: str = '', type_: str = 'data'):
         super().__init__(label, type_)
```

### Comparing `ryvencore-0.4.0a9/ryvencore/README.md` & `ryvencore-0.5.0/ryvencore/README.md`

 * *Files identical despite different names*

### Comparing `ryvencore-0.4.0a9/ryvencore/Session.py` & `ryvencore-0.5.0/ryvencore/Session.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,126 +1,169 @@
 import importlib
 import glob
-from typing import List, Dict
+import os.path
+from typing import List, Dict, Type, Optional, Any
 
+from .Data import Data
 from .Base import Base, Event
 from .Flow import Flow
 from .InfoMsgs import InfoMsgs
-from .utils import pkg_path, load_from_file
+from .utils import pkg_version, pkg_path, load_from_file, print_err
 from .Node import Node
 
 
 class Session(Base):
     """
     The Session is the top level interface to your project. It mainly manages flows, nodes, and add-ons and
     provides methods for serialization and deserialization of the project.
     """
 
+    version = pkg_version()
+
     def __init__(
             self,
             gui: bool = False,
+            load_addons: bool = False,
     ):
         Base.__init__(self)
 
         # events
-        self.new_flow_created = Event(Flow)
-        self.flow_renamed = Event(Flow)
+        self.flow_created = Event(Flow)
+        self.flow_renamed = Event(Flow, str)
         self.flow_deleted = Event(Flow)
 
         # ATTRIBUTES
-        self.addons = {}
-        self.flows: [Flow] = []
-        self.nodes = set()  # list of node CLASSES
-        self.invisible_nodes = set()
+        self.addons: Dict[str, Any] = {}
+        self.flows: List[Flow] = []
+        self.nodes: set[type[Node]] = set()      # list of node CLASSES
+        self.invisible_nodes: set[type[Node]] = set()
+        self.data_types: Dict[str, type[Data]] = {}
         self.gui: bool = gui
-        self.init_data = None
+        self.init_data: Optional[Dict] = None
 
-        self.load_addons(pkg_path('addons/default/'))
-        self.load_addons(pkg_path('addons/'))
+        # self.register_addons(pkg_path('addons/legacy/'))
+        # self.register_addons(pkg_path('addons/'))
+        if load_addons:
+            self.register_addons()
 
 
-    def load_addons(self, location: str):
+    def register_addons(self, location: Optional[str] = None):
         """
-        Loads all addons from the given location. ``location`` can be an absolute path to any readable directory.
-        See ``ryvencore.AddOn``.
+        Loads all addons from the given location, or from ryvencore's
+        *addons* directory if :code:`location` is :code:`None`.
+        :code:`location` can be an absolute path to any readable directory.
+        New addons can be registered at any time.
+        Addons cannot be de-registered.
+        See :code:`ryvencore.AddOn`.
         """
 
+        if location is None:
+            location = pkg_path('addons/')
+
         # discover all top-level modules in the given location
         addons = filter(lambda p: not p.endswith('__init__.py'), glob.glob(location + '/*.py'))
 
         for path in addons:
             # extract 'addon' object from module
             addon, = load_from_file(path, ['addon'])
 
             if addon is None:
                 continue
 
             # register addon
-            modname = path.split('/')[-1][:-3]
+            modname = os.path.split(path)[-1][:-3]
             self.addons[modname] = addon
 
             addon.register(self)
-            setattr(Node, addon.name, addon)
+            # setattr(Node, addon.name, addon)
+
+            # establish event connections
+            self.flow_created.sub(addon.on_flow_created, nice=-5)
+            self.flow_deleted.sub(addon.on_flow_destroyed, nice=-5)
+            for f in self.flows:
+                addon.connect_flow_events(f)
 
 
-    def register_nodes(self, node_classes: List):
+    def register_node_types(self, node_types: List[Type[Node]]):
         """
         Registers a list of Nodes which then become available in the flows.
         Do not attempt to place nodes in flows that haven't been registered in the session before.
         """
 
-        for n in node_classes:
-            self.register_node(n)
+        for n in node_types:
+            self.register_node_type(n)
 
 
-    def register_node(self, node_class):
+    def register_node_type(self, node_class: Type[Node]):
         """
         Registers a single node.
         """
 
-        # build node class identifier
         node_class._build_identifier()
-
         self.nodes.add(node_class)
 
 
-    def unregister_node(self, node_class):
+    def unregister_node(self, node_class: Type[Node]):
         """
         Unregisters a node which will then be removed from the available list.
         Existing instances won't be affected.
         """
 
         self.nodes.remove(node_class)
 
 
-    def all_node_objects(self) -> List:
+    def all_node_objects(self) -> List[Node]:
         """
         Returns a list of all node objects instantiated in any flow.
         """
 
-        nodes = []
-        for s in self.flows:
-            for n in s.flow.nodes:
-                nodes.append(n)
-        return nodes
+        return [n for f in self.flows for n in f.nodes]
 
 
-    def create_flow(self, title: str = None, data: Dict = None) -> Flow:
+    def register_data_type(self, data_type_class: Type[Data]):
+        """
+        Registers a new :code:`Data` subclass which will then be available
+        in the flows.
+        """
+
+        data_type_class._build_identifier()
+        id = data_type_class.identifier
+        if id == 'Data' or id in self.data_types:
+            print_err(
+                f'Data type identifier "{id}" is already registered. '
+                f'skipping. You can use the "identifier" attribute of '
+                f'your Data subclass.')
+            return
+
+        self.data_types[id] = data_type_class
+
+
+    def register_data_types(self, data_type_classes: List[Type[Data]]):
+        """
+        Registers a list of :code:`Data` subclasses which will then be available
+        in the flows.
+        """
+
+        for d in data_type_classes:
+            self.register_data_type(d)
+
+
+    def create_flow(self, title: str, data: Optional[Dict] = None) -> Flow:
         """
         Creates and returns a new flow.
         If data is provided the title parameter will be ignored.
         """
 
         flow = Flow(session=self, title=title)
         self.flows.append(flow)
 
-        if data:
-            flow.load(data)
+        self.flow_created.emit(flow)
 
-        self.new_flow_created.emit(flow)
+        if data is not None:
+            flow.load(data)
 
         return flow
 
 
     def rename_flow(self, flow: Flow, title: str) -> bool:
         """
         Renames an existing flow and returns success boolean.
@@ -128,15 +171,15 @@
 
         success = False
 
         if self.flow_title_valid(title):
             flow.title = title
             success = True
 
-        self.flow_renamed.emit(flow)
+        self.flow_renamed.emit(flow, title)
 
         return success
 
 
     def flow_title_valid(self, title: str) -> bool:
         """
         Checks whether a considered title for a new flow is valid (unique) or not.
@@ -167,59 +210,71 @@
         """
 
         return InfoMsgs
 
 
     def load(self, data: Dict) -> List[Flow]:
         """
-        Loads a project and raises an exception if required nodes are missing (not registered).
+        Loads a project and raises an exception if required nodes are missing
+        (not registered).
         """
 
         super().load(data)
 
         self.init_data = data
 
+        # load addons
+        for name, addon_data in data['addons'].items():
+            if name in self.addons:
+                self.addons[name].load(addon_data)
+            else:
+                print(f'found missing addon: {name}; attempting to load anyway')
+
         # load flows
         new_flows = []
 
         #   backward compatibility
         if 'scripts' in data:
             flows_data = {
                 title: script_data['flow']
                 for title, script_data in data['scripts'].items()
             }
+        elif isinstance(data['flows'], list):
+            flows_data = {
+                f'Flow {i}': flow_data
+                for i, flow_data in enumerate(data['flows'])
+            }
         else:
             flows_data = data['flows']
 
-        for fd in flows_data:
-            new_flows.append(self.create_flow(data=fd))
-
-        # load addons
-        for name, addon_data in data['addons'].items():
-            if name in self.addons:
-                self.addons[name].set_state(addon_data)
-            else:
-                print(f'found missing addon: {name}; attempting to load anyway')
+        for title, data in flows_data.items():
+            new_flows.append(self.create_flow(title=title, data=data))
 
         return new_flows
 
-    def serialize(self):
-        """Returns the project as JSON compatible dict to be saved and loaded again using load()"""
+    def serialize(self) -> Dict:
+        """
+        Returns the project as JSON compatible dict to be saved and
+        loaded again using load()
+        """
 
         return self.complete_data(self.data())
 
 
     def data(self) -> dict:
         """
-        Serializes the whole project into a JSON compatible dict. Pass to ``load()`` in a new session to restore.
+        Serializes the project's abstract state into a JSON compatible
+        dict. Pass to :code:`load()` in a new session to restore.
+        Don't use this function for saving, use :code:`serialize()` in
+        order to include the effects of :code:`Base.complete_data()`.
         """
 
-        d = super().data()
-        d.update({
-            'flows': [
-                s.data() for s in self.flows
-            ],
+        return {
+            **super().data(),
+            'flows': {
+                f.title: f.data()
+                for f in self.flows
+            },
             'addons': {
-                name: addon.get_state() for name, addon in self.addons.items()
+                name: addon.data() for name, addon in self.addons.items()
             }
-        })
-        return d
+        }
```

### Comparing `ryvencore-0.4.0a9/ryvencore/addons/default/DTypes.py` & `ryvencore-0.5.0/ryvencore/addons/legacy/DTypes.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,29 +5,35 @@
 These dtypes only store some information which might be used by the nodes, or by a frontend, etc.
 There is currently no type checking or something like that implemented, but might be added
 optionally in the future.
 
 This list may grow significantly over time.
 """
 
-from typing import Dict as t_Dict, List as t_List
+from typing import (
+    TypeVar,
+    Optional,
+    Dict as t_Dict, 
+    List as t_List, 
+    Tuple as t_Tuple,
+)
 
 
 class DType:
-    def __init__(self, default, bounds: tuple = None, doc: str = "", _load_state=None):
+    def __init__(self, default, bounds: Optional[t_Tuple] = None, doc: str = "", _load_state=None):
 
         self.default = default
         self.val = self.default
         self.doc = doc
         self.bounds = bounds
 
         if _load_state:
             self.set_state(_load_state)
 
-        self._data = ['default', 'val', 'doc', 'bounds']
+        self._data = ['legacy', 'val', 'doc', 'bounds']
 
     def __str__(self):
         return 'DType.'+self.__class__.__name__
 
     @staticmethod
     def from_str(s):
         for DTypeClass in dtypes:
@@ -58,32 +64,32 @@
         """
         self.size = size
         super().__init__(default=default, doc=doc, _load_state=_load_state)
         self.add_data('size')
 
 
 class Integer(DType):
-    def __init__(self, default: int = 0, bounds: tuple = None, doc: str = "", _load_state=None):
+    def __init__(self, default: int = 0, bounds: Optional[tuple] = None, doc: str = "", _load_state=None):
         super().__init__(default=default, bounds=bounds, doc=doc, _load_state=_load_state)
 
 
 class Float(DType):
-    def __init__(self, default: float = 0.0, bounds: tuple = None, decimals: int = 10, doc: str = "", _load_state=None):
+    def __init__(self, default: float = 0.0, bounds: Optional[tuple] = None, decimals: int = 10, doc: str = "", _load_state=None):
         self.decimals = decimals
         super().__init__(default=default, bounds=bounds, doc=doc, _load_state=_load_state)
         self.add_data('decimals')
 
 
 class Boolean(DType):
     def __init__(self, default: bool = False, doc: str = "", _load_state=None):
         super().__init__(default=default, doc=doc, _load_state=_load_state)
 
 
 class Char(DType):
-    def __init__(self, default: chr = '', doc: str = "", _load_state=None):
+    def __init__(self, default: str = '0', doc: str = "", _load_state=None):
         super().__init__(default=default, doc=doc, _load_state=_load_state)
 
 
 class String(DType):
     def __init__(self, default: str = "", size: str = 'm', doc: str = "", _load_state=None):
         """
         size: 's' / 'm' / 'l'
@@ -179,19 +185,19 @@
     Float = Float
     Boolean = Boolean
     Char = Char
     String = String
     Choice = Choice
     List = List
 
-    class NodeInputType(NodeInputType):
-        def __init__(self, dtype=None, *args, **kwargs):
-            super().__init__(*args, **kwargs)
+    # class NodeInputType(NodeInputType):
+    #     def __init__(self, dtype=None, *args, **kwargs):
+    #         super().__init__(**kwargs)
 
-            self.dtype = dtype
+    #         self.dtype = dtype
 
     def __init__(self):
         super().__init__()
 
         self.dtype_inputs = {}  # {NodeInput: DType}
         self.creating_dtype_input = False
 
@@ -207,26 +213,26 @@
         # dtypes are only on data inputs allowed
         if inp.type_ != 'data':
             node.delete_input(node.inputs.index(inp))
             return
 
         self.dtype_inputs[inp] = dtype
 
-    def _on_node_created(self, flow, node):
+    def on_node_created(self, flow, node):
         """
         Restores the node's dtypes.
         """
 
         for i, inp in enumerate(node.inputs):
-            if inp.type_ == 'data' and 'dtype' in node.init_data['inputs'][i]:
-                dtype = DType.from_str(node.init_data['inputs'][i]['dtype'])
-                dtype.set_state(node.init_data['inputs'][i]['dtype']['state'])
+            if inp.type_ == 'data' and 'dtype' in node.load_data['inputs'][i]:
+                dtype = DType.from_str(node.load_data['inputs'][i]['dtype'])
+                dtype.set_state(node.load_data['inputs'][i]['dtype']['state'])
                 self.dtype_inputs[inp] = dtype
 
-    def _extend_node_data(self, node, data: dict):
+    def extend_node_data(self, node, data: dict):
         for i, inp in enumerate(node.inputs):
             if inp in self.dtype_inputs:
                 data['inputs'][i]['dtype'] = {
                     'type': str(self.dtype_inputs[inp]),
                     'state': self.dtype_inputs[inp].get_state(),
                 }
```

### Comparing `ryvencore-0.4.0a9/ryvencore/addons/default/Logging.py` & `ryvencore-0.5.0/ryvencore/addons/Logging.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,105 +2,120 @@
 WIP
 """
 
 from logging import Logger as PyLogger
 from typing import Optional
 
 from ryvencore.AddOn import AddOn
+from ryvencore.Base import Event
 
 
 class Logger(PyLogger):
 
     def __init__(self, *args, **kwargs):
         PyLogger.__init__(self, *args, **kwargs)
     #     # events
-    #     self.sig_enabled = Event()
-    #     self.sig_disabled = Event()
+        self.sig_enabled = Event()
+        self.sig_disabled = Event()  # 'disabled' is reserved
 
     def enable(self):
-        # self.sig_enabled.emit()
-        pass
+        self.sig_enabled.emit()
 
     def disable(self):
-        # self.sig_disabled.emit()
-        pass
+        self.sig_disabled.emit()
 
 
 class LoggingAddon(AddOn):
     """
-    This addon implements very basic some logging functionality.
+    This addon implements some very basic logging functionality.
 
-    It provides an API to create and delete loggers that are owned
-    by a particular node. The logger gets enabled/disabled
+    It provides functions to create and delete loggers that are owned
+    by a particular node. The loggers get enabled/disabled
     automatically when the owning node is added to/removed from
-    the flow.
+    the flow. When a node is serialized, its loggers are saved in
+    the state dict of the flow, and when the node is deserialized,
+    the loggers get recreated.
 
     Ownership might eventually be expanded to any component that
     preserves its global ID throughout save and load.
 
     The contents of logs are currently not preserved. If a log's
-    content should be preserved, it should be saved in a file.
+    content should be preserved, it should be saved explicitly.
 
     Refer to Python's logging module documentation.
     """
 
     name = 'Logging'
     version = '0.0.1'
 
     def __init__(self):
         super().__init__()
 
         # logger_created = Event(Logger)
 
         self.loggers = {}   # {Node: {name: Logger}}
 
+        self.log_created = Event(Logger)
+        # TODO: support deletion of loggers?
+
     def new_logger(self, node, title: str) -> Optional[Logger]:
         """
         Creates a new logger owned by the node, returns None if
         one with the given name already exists.
         """
 
         if not self._node_is_registered(node):
             self.loggers[node] = {}
 
         elif title in self.loggers[node]:
             return None
 
         logger = Logger(name=title)
         self.loggers[node][title] = logger
-        # self.logger_created.emit(logger)
+        self.log_created.emit(logger)
         return logger
 
-    def _on_node_created(self, flow, node):
-        if node.init_data and 'Logging' in node.init_data:
-            for title in node.init_data['Logging']['loggers']:
+    def get(self, node, title: str) -> Optional[Logger]:
+        """
+        Returns the logger with the given name owned by the node,
+        or None if it doesn't exist.
+        """
+
+        if not self._node_is_registered(node):
+            return None
+
+        return self.loggers[node][title]
+
+    def on_node_created(self, node):
+        if node.load_data and 'Logging' in node.load_data:
+            for title in node.load_data['Logging']['loggers']:
                 self.new_logger(node, title)
                 # in case the node already created the logger,
                 # new_logger() will have no effect
 
     def _node_is_registered(self, node):
         return node in self.loggers
 
-    def _on_node_added(self, flow, node):
+    def on_node_added(self, node):
         if not self._node_is_registered(node):
             return
 
         # enable the node's loggers
         for logger in self.loggers[node].values():
             logger.enable()
 
-    def _on_node_removed(self, flow, node):
+    def on_node_removed(self, node):
         if not self._node_is_registered(node):
             return
 
         # disable the node's loggers
         for logger in self.loggers[node].values():
             logger.disable()
 
-    def _extend_node_data(self, node, data: dict):
+    def extend_node_data(self, node, data: dict):
         if not self._node_is_registered(node):
             return
 
         data['Logging'] = {
             'loggers': [name for name in self.loggers[node].keys()]
         }
```

### Comparing `ryvencore-0.4.0a9/ryvencore/addons/default/Variables.py` & `ryvencore-0.5.0/ryvencore/addons/Variables.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,48 @@
-from typing import Optional
+from typing import Optional, Union, Any, Dict, List, Tuple
+from packaging.version import parse as parse_version
 
-from ryvencore import Node
+from ryvencore import Node, Data, AddOn, Flow
 from ryvencore.Base import Base, Event
-from ryvencore.utils import serialize, deserialize
-from ryvencore import AddOn
+from ryvencore.utils import print_err
 
 
+ADDON_VERSION = '0.4'
+# TODO: replace print_err with InfoMsgs
+
 
 class Variable:
-    """Implementation of flow variables"""
+    """
+    Implementation of flow variables.
+    A Variable can currently only hold pickle serializable data.
+    Storing other data will break save&load.
+    """
 
-    def __init__(self, addon, flow, name='', val=None, data=None):
+    def __init__(self, addon: Any, flow: Flow, name='', val=None, data=None):
         self.addon = addon
         self.flow = flow
         self.name = name
-        self.val = val
-
-        if data and 'serialized' in data.keys():
-            self.val = deserialize(data['serialized'])
+        self.data: Data = Data(value=val, load_from=data)
 
     def get(self):
         """
         Returns the value of the variable
         """
-        return self.val
+        return self.data.payload
 
-    def set(self, val):
+    def set(self, val, silent=False):
         """
         Sets the value of the variable
         """
-        self.val = val
-        self.addon._var_updated(self.flow, self.name)
+        self.data = Data(val)
+        if not silent:
+            self.addon.update_subscribers(self.flow, self.name)
 
     def serialize(self):
-        return serialize(self.val)
+        return self.data.data()
 
 
 
 
 class VarsAddon(AddOn):
     """
     This addon provides a simple variable system.
@@ -69,159 +74,249 @@
     ...         self.var_val = self.Vars.var(self.flow, 'var1').get()
     ...
     ...     def var1_changed(self, val):
     ...         print('var1 changed!')
     ...         self.var_val = val
     >>>
     >>> s = rc.Session()
-    >>> s.register_node(MyNode)
+    >>> s.register_node_type(MyNode)
     >>> f = s.create_flow('main')
     >>>
     >>> Vars = s.addons['Variables']
     >>> v = Vars.create_var(f, 'var1', None)
     >>>
     >>> n1 = f.create_node(MyNode)
     >>> v.set(42)
     var1 changed!
     >>> print(n1.var_val)
     42
     """
 
     name = 'Variables'
-    version = '0.0.3'
+    version = ADDON_VERSION
 
-    def __init__(self):
+    def __init__(self) -> None:
         AddOn.__init__(self)
 
-        # {
-        #   Flow: {
-        #       'variable name': {
-        #           'var': Variable,
-        #           'subscriptions': [Node method]
-        #        },
-        # }
-        self.flow_variables = {}
+        # layout:
+        #   {
+        #       Flow: {
+        #           'variable name': {
+        #               'var': Variable,
+        #               'subscriptions': [(node, method)]
+        #           },
+        #   }
+        self.flow_variables: Dict[
+            Flow, Dict[
+                str, Dict[
+                    str,
+                    Union[Variable, List[Tuple[Node, Any]]]
+                 ]
+             ]
+         ] = {}
+
+        # nodes can be removed and re-added, so we need to keep track of the broken
+        # subscriptions when nodes get removed, because they might get re-added
+        # in which case we need to re-establish their subscriptions
+        # layout:
+        #   {
+        #       Node: {
+        #          'variable name': 'callback name'
+        #       }
+        #   }
+        self.removed_subscriptions: Dict[Node, Dict[str, str]] = {}
+
+        # state data of variables that need to be recreated once their flow is
+        # available, see :code:`on_flow_created()`
+        self.flow_vars__pending: Dict = {}
+
+        # events
+        self.var_created = Event(Flow, str, Variable)
+        self.var_deleted = Event(Flow, str)
+
+    """
+    flow management
+    """
+
+    def on_flow_created(self, flow):
+        self.flow_variables[flow] = {}
+
+    def on_flow_deleted(self, flow):
+        del self.flow_variables[flow]
+
+    """
+    subscription management
+    """
+
+    def on_node_created(self, node):
+        flow = node.flow
+
+        # is invoked *before* the node is added to the flow
+
+        # unfortunately, I cannot do this in on_flow_created because there
+        # the flow doesn't have it's prev_global_id yet, but here it does
+        if flow.prev_global_id in self.flow_vars__pending:
+            for name, data in self.flow_vars__pending[flow.prev_global_id].items():
+                self.create_var(flow, name, load_from=data)
+            del self.flow_vars__pending[flow.prev_global_id]
+
+    def on_node_added(self, node):
+        """
+        Reconstruction of subscriptions.
+        """
+
+        # if node had subscriptions previously (so it was removed)
+        if node in self.removed_subscriptions:
+            for name, cb in self.removed_subscriptions[node].items():
+                self.subscribe(node, name, cb)
+            del self.removed_subscriptions[node]
+
+        # otherwise, check if it has load data and reconstruct subscriptions
+        elif node.load_data and 'Variables' in node.load_data:
+            for name, cb_name in node.load_data['Variables']['subscriptions'].items():
+                self.subscribe(node, name, getattr(node, cb_name))
+
+    def on_node_removed(self, node):
+        """
+        Remove all subscriptions of the node.
+        """
+
+        # store subscription in removed_subscriptions
+        # because the node might get re-added later
+        self.removed_subscriptions[node] = {}
+
+        for name, var_info in self.flow_variables[node.flow].items():
+            for (n, cb) in var_info['subscriptions']:
+                if n == node:
+                    self.removed_subscriptions[node][name] = cb.__name__
+                    self.unsubscribe(node, name, cb)
+
+    """
+    variables api
+    """
 
     def var_name_valid(self, flow, name: str) -> bool:
         """
-        Checks if ``name`` is a valid variable identifier and hasn't been take yet.
+        Checks if :code:`name` is a valid variable identifier and hasn't been take yet.
         """
 
-        return name.isidentifier() and not self._var_exists(flow, name)
+        return name.isidentifier() and not self.var_exists(flow, name)
 
-    def create_var(self, flow, name: str, val=None, data=None) -> Optional[Variable]:
+    def create_var(self, flow: Flow, name: str, val=None, load_from=None) -> Optional[Variable]:
         """
         Creates and returns a new variable and None if the name isn't valid.
         """
 
-        if flow not in self.flow_variables:
-            self.flow_variables[flow] = {}
-
         if self.var_name_valid(flow, name):
-            v = Variable(self, flow, name, val, data)
+            v = Variable(self, flow, name, val, load_from)
             self.flow_variables[flow][name] = {
                 'var': v,
                 'subscriptions': []
             }
+            self.var_created.emit(flow, name, v)
             return v
-        else:
-            return None
+
+        return None
 
     def delete_var(self, flow, name: str):
         """
         Deletes a variable and causes subscription update. Subscriptions are preserved.
         """
-        if not self._var_exists(flow, name):
+        if not self.var_exists(flow, name):
+            # print_err(f'Variable {name} does not exist.')
             return
 
-        del self.flow_variables[flow][name]['var']
+        del self.flow_variables[flow][name]
+        self.var_deleted.emit(flow, name)
 
-    def _var_exists(self, flow, name: str) -> bool:
+    def var_exists(self, flow, name: str) -> bool:
         return flow in self.flow_variables and name in self.flow_variables[flow]
 
-    def var(self, flow, name: str):
+    def var(self, flow, name: str) -> Optional[Variable]:
         """
         Returns the variable with the given name or None if it doesn't exist.
         """
-        if not self._var_exists(flow, name):
+        if not self.var_exists(flow, name):
+            # print_err(f'Variable {name} does not exist.')
             return None
 
-        return self.flow_variables[flow][name]['var']
+        return self.flow_variables[flow][name]['var']  # type: ignore
 
-    def _var_updated(self, flow, name: str):
+    def update_subscribers(self, flow, name: str):
         """
         Called when a Variable object changes or when the var is created or deleted.
         """
 
         v = self.flow_variables[flow][name]['var']
 
-        for (node, cb) in self.flow_variables[flow][name]['subscriptions']:
-            cb(v.val)
+        for (node, cb) in self.flow_variables[flow][name]['subscriptions']:  # type: ignore
+            cb(v)
 
     def subscribe(self, node: Node, name: str, callback):
         """
         Subscribe to a variable. ``callback`` must be a method of the node.
         """
-        if not self._var_exists(node.flow, name):
+        if not self.var_exists(node.flow, name):
+            # print_err(f'Variable {name} does not exist.')
             return
 
-        self.flow_variables[node.flow][name]['subscriptions'].append((node, callback))
+        self.flow_variables[node.flow][name]['subscriptions'].append((node, callback))  # type: ignore
 
     def unsubscribe(self, node, name: str, callback):
         """
         Unsubscribe from a variable.
         """
-        if not self._var_exists(node.flow, name):
+        if not self.var_exists(node.flow, name):
+            # print_err(f'Variable {name} does not exist.')
             return
 
-        self.flow_variables[node.flow][name]['subscriptions'].remove((node, callback))
+        self.flow_variables[node.flow][name]['subscriptions'].remove((node, callback))  # type: ignore
+
+    """
+    serialization
+    """
 
-    def _extend_node_data(self, node, data: dict):
+    def extend_node_data(self, node, data: dict):
         """
         Extends the node data with the variable subscriptions.
         """
 
+        if self.flow_variables.get(node.flow) == {}:
+            return
+
         data['Variables'] = {
             'subscriptions': {
                 name: cb.__name__
                 for name, var in self.flow_variables[node.flow].items()
-                for (n, cb) in var['subscriptions']
+                for (n, cb) in var['subscriptions']  # type: ignore
                 if node == n
             }
         }
 
-        if data['Variables']['subscriptions'] == {}:
-            del data['Variables']
-
-    def _on_node_created(self, flow, node):
-        """
-        Reconstruction of subscriptions.
-        """
-        if node.init_data and 'Variables' in node.init_data:
-            for name, cb_name in node.init_data['Variables']['subscriptions'].items():
-                self.subscribe(node, name, getattr(node, cb_name))
-
     def get_state(self) -> dict:
+        """"""
+        
         return {
-            f.GLOBAL_ID: {
-                name: {
-                    'serialized': var['var'].serialize()
-                }
+            f.global_id: {
+                name: var['var'].serialize()  # type: ignore
                 for name, var in self.flow_variables[f].items()
             }
             for f in self.flow_variables.keys()
         }
 
-    def set_state(self, state: dict):
+    def set_state(self, state: dict, version: str):
+        """"""
 
-        for pref_flow_id, variables in state.items():
-            f = Base.obj_from_prev_id(pref_flow_id)
+        if parse_version(version) < parse_version('0.4'):
+            print_err('Variables addon state version too old, skipping')
+            return
+
+        # JSON converts int keys to strings, so we need to convert them back
+        state = {
+            int(flow_id): flow_vars
+            for flow_id, flow_vars in state.items()
+        }
 
-            # recreate variables
-            for name, var in variables.items():
-                if self._var_exists(f, name):
-                    self.var(f, name).set(deserialize(var['serialized']))
-                else:
-                    self.create_var(f, name, data=var)
+        self.flow_vars__pending = state
 
 
 addon = VarsAddon()
```

### Comparing `ryvencore-0.4.0a9/ryvencore/utils.py` & `ryvencore-0.5.0/ryvencore/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,56 @@
 """A collection of useful functions used by different components."""
 
 import base64
-import importlib.util
+import json
 import pickle
+import sys
 from os.path import dirname, abspath, join, basename
-from typing import List, Tuple
+from typing import List, Tuple, Optional, Dict
+from packaging.version import Version, parse as _parse_version
+import importlib.util
+
+if sys.version_info < (3, 8):
+    import importlib_metadata
+else:
+    import importlib.metadata as importlib_metadata
+
+def pkg_version() -> str:
+    return importlib_metadata.version('ryvencore')
+
+
+def pkg_path(subpath: Optional[str] = None):
+    """
+    Returns the path to the installed package root directory, optionally with a relative sub-path appended.
+    Notice that this returns the path to the ryvencore package (ryvencore/ryvencore/) not the repository (ryvencore/).
+    """
+
+    p = dirname(__file__)
+    if subpath is not None:
+        p = join(p, subpath)
+    return abspath(p)
 
 
 def serialize(data) -> str:
     return base64.b64encode(pickle.dumps(data)).decode('ascii')
 
 
 def deserialize(data):
     return pickle.loads(base64.b64decode(data))
 
 
+def print_err(*args, **kwargs):
+    print(*args, file=sys.stderr, **kwargs)
+
+
+def json_print(d: Dict):
+    # I just need this all the time
+    print(json.dumps(d, indent=4))
+
+
 def node_from_identifier(identifier: str, nodes: List):
 
     for nc in nodes:
         if nc.identifier == identifier:
             return nc
     else:  # couldn't find a node with this identifier => search for identifier_comp
         for nc in nodes:
@@ -28,39 +60,37 @@
             raise Exception(
                 f'could not find node class with identifier \'{identifier}\'. '
                 f'if you changed your node\'s class name, make sure to add the old '
                 f'identifier to the identifier_comp list attribute to provide '
                 f'backwards compatibility.'
             )
 
-def pkg_path(subpath: str = None):
-    """
-    Returns the path to the installed package root directory, optionally with a relative sub-path appended.
-    Notice that this returns the path to the ryvencore package (ryvencore/ryvencore/) not the repository (ryvencore/).
-    """
-
-    p = dirname(__file__)
-    if subpath is not None:
-        p = join(p, subpath)
-    return abspath(p)
-
 
 def load_from_file(file: str, comps: List[str]) -> Tuple:
     """
     Imports components with name in ``comps`` from a python module.
     """
     # https://stackoverflow.com/questions/67631/how-do-i-import-a-module-given-the-full-path
 
     name = basename(file).split('.')[0]
     spec = importlib.util.spec_from_file_location(name, file)
+
+    assert name is not None
+    assert spec is not None
+    assert spec.loader is not None
+    
     importlib.util.module_from_spec(spec)
+
+    # TODO
+    #  I'm using the deprecated load_module() instead of
+    #  exec_module() because I had issues with exec_module().
+    #  exec_module() somehow registers it as "built-in" which
+    #  is wrong and prevents features, such as inspecting
+    #  the source with inspect
     mod = spec.loader.load_module(name)
-    # using load_module(name) instead of exec_module(mod) here,
-    # because exec_module() somehow then registers it as "built-in"
-    # which is wrong and e.g. prevents inspect from parsing the source
 
     def get_comp(c):
         try:
             return getattr(mod, c)
         except AttributeError:
             return None
```

### Comparing `ryvencore-0.4.0a9/ryvencore.egg-info/PKG-INFO` & `ryvencore-0.5.0/ryvencore.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: ryvencore
-Version: 0.4.0a9
+Version: 0.5.0
 Summary: Python backend for node editor-like graph-based processing
 Home-page: https://github.com/leon-thomm/ryvencore
 Author: Leon Thomm
 Author-email: l.thomm@mailbox.org
 Project-URL: Website, https://ryven.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: importlib_metadata; python_version < "3.8"
+Requires-Dist: packaging
 
 
 <p align="center">
   <img src="./docs/img/logo.png" alt="drawing" width="70%"/>
 </p>
 
 An experimental Python library for graph-based processing, designed for flow-based/node-based visual scripting editors. It is the backbone of the [Ryven](https://github.com/leon-thomm/Ryven) project, but it can very much be used in other contexts as well.
 
-While ryvencore is written purely in Python, it is very lightweight and highly compatible. It can be compiled with Cython, see the `setup_cython.py` file. The performance seems comparable so far, but the code hasn't been optimized for Cython yet, so there might be a lot of potential. Please consider contributing. [Pyodide](https://github.com/pyodide/pyodide) provides a WebAssembly port of ryvencore.
+While ryvencore is written purely in Python, it is very lightweight and highly compatible. It can be compiled with Cython, see the `setup_cython.py` file. The performance seems comparable so far, but the code hasn't been optimized for Cython yet, so there might be a lot of potential. Please consider contributing. ryvencore also seems compatible with most Python ports to WebAssembly, even the Cython compiled ryvencore.
 
 ### Installation
 
 ```
 pip install ryvencore
 ```
```

### Comparing `ryvencore-0.4.0a9/setup.cfg` & `ryvencore-0.5.0/setup.cfg`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ryvencore
-version = v0.4.0a9
+version = v0.5.0
 author = Leon Thomm
 author_email = l.thomm@mailbox.org
 description = Python backend for node editor-like graph-based processing
 long_description = file: README.md
 long_description_content_type = text/markdown
 license_file = LICENSE
 url = https://github.com/leon-thomm/ryvencore
@@ -14,13 +14,19 @@
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 	Operating System :: OS Independent
 
 [options]
 packages = find:
 include_package_data = True
-python_requires = >=3.6
+python_requires = >=3.7
+install_requires = 
+	importlib_metadata; python_version<'3.8'
+	packaging
+
+[tool:pytest]
+testpaths = tests/*
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

