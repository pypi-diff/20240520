# Comparing `tmp/qmio-0.1.2.tar.gz` & `tmp/qmio-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qmio-0.1.2.tar", last modified: Wed May 15 15:57:04 2024, max compression
+gzip compressed data, was "qmio-0.1.3.tar", last modified: Mon May 20 15:21:15 2024, max compression
```

## Comparing `qmio-0.1.2.tar` & `qmio-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 jlopez    (1000) jlopez    (1000)        0 2024-05-15 15:57:04.200924 qmio-0.1.2/
--rw-rw-r--   0 jlopez    (1000) jlopez    (1000)    11358 2024-05-08 07:55:18.000000 qmio-0.1.2/LICENSE
--rw-rw-r--   0 jlopez    (1000) jlopez    (1000)      828 2024-05-15 15:57:04.200924 qmio-0.1.2/PKG-INFO
--rw-rw-r--   0 jlopez    (1000) jlopez    (1000)      412 2024-05-15 15:53:18.000000 qmio-0.1.2/README.md
-drwxrwxr-x   0 jlopez    (1000) jlopez    (1000)        0 2024-05-15 15:57:04.200924 qmio-0.1.2/config/
--rw-rw-r--   0 jlopez    (1000) jlopez    (1000)       50 2024-05-08 10:14:51.000000 qmio-0.1.2/config/__init__.py
-drwxrwxr-x   0 jlopez    (1000) jlopez    (1000)        0 2024-05-15 15:57:04.200924 qmio-0.1.2/qmio/
--rw-rw-r--   0 jlopez    (1000) jlopez    (1000)       63 2024-05-15 15:55:44.000000 qmio-0.1.2/qmio/__init__.py
--rw-rw-r--   0 jlopez    (1000) jlopez    (1000)     2255 2024-05-08 09:56:22.000000 qmio-0.1.2/qmio/backends.py
--rw-rw-r--   0 jlopez    (1000) jlopez    (1000)      346 2024-05-08 09:53:14.000000 qmio-0.1.2/qmio/circuits.py
--rw-rw-r--   0 jlopez    (1000) jlopez    (1000)     1511 2024-05-08 10:12:16.000000 qmio-0.1.2/qmio/clients.py
--rw-rw-r--   0 jlopez    (1000) jlopez    (1000)     1092 2024-05-08 07:55:18.000000 qmio-0.1.2/qmio/qmio.py
--rw-rw-r--   0 jlopez    (1000) jlopez    (1000)      275 2024-05-08 07:55:18.000000 qmio-0.1.2/qmio/services.py
-drwxrwxr-x   0 jlopez    (1000) jlopez    (1000)        0 2024-05-15 15:57:04.200924 qmio-0.1.2/qmio.egg-info/
--rw-rw-r--   0 jlopez    (1000) jlopez    (1000)      828 2024-05-15 15:57:04.000000 qmio-0.1.2/qmio.egg-info/PKG-INFO
--rw-rw-r--   0 jlopez    (1000) jlopez    (1000)      380 2024-05-15 15:57:04.000000 qmio-0.1.2/qmio.egg-info/SOURCES.txt
--rw-rw-r--   0 jlopez    (1000) jlopez    (1000)        1 2024-05-15 15:57:04.000000 qmio-0.1.2/qmio.egg-info/dependency_links.txt
--rw-rw-r--   0 jlopez    (1000) jlopez    (1000)       21 2024-05-15 15:57:04.000000 qmio-0.1.2/qmio.egg-info/requires.txt
--rw-rw-r--   0 jlopez    (1000) jlopez    (1000)       18 2024-05-15 15:57:04.000000 qmio-0.1.2/qmio.egg-info/top_level.txt
--rw-rw-r--   0 jlopez    (1000) jlopez    (1000)      630 2024-05-15 15:57:04.200924 qmio-0.1.2/setup.cfg
--rw-rw-r--   0 jlopez    (1000) jlopez    (1000)       38 2024-05-08 07:55:18.000000 qmio-0.1.2/setup.py
-drwxrwxr-x   0 jlopez    (1000) jlopez    (1000)        0 2024-05-15 15:57:04.200924 qmio-0.1.2/tests/
--rw-rw-r--   0 jlopez    (1000) jlopez    (1000)        0 2024-05-08 07:55:18.000000 qmio-0.1.2/tests/__init__.py
--rw-rw-r--   0 jlopez    (1000) jlopez    (1000)      834 2024-05-08 07:55:18.000000 qmio-0.1.2/tests/test_backends.py
--rw-rw-r--   0 jlopez    (1000) jlopez    (1000)      412 2024-05-08 07:55:18.000000 qmio-0.1.2/tests/test_services.py
--rw-rw-r--   0 jlopez    (1000) jlopez    (1000)       35 2024-05-08 07:55:18.000000 qmio-0.1.2/tests/test_zmq_client.py
+drwxrwxr-x   0 jlopez    (1000) jlopez    (1000)        0 2024-05-20 15:21:15.012025 qmio-0.1.3/
+-rw-rw-r--   0 jlopez    (1000) jlopez    (1000)    11358 2024-05-08 07:55:18.000000 qmio-0.1.3/LICENSE
+-rw-rw-r--   0 jlopez    (1000) jlopez    (1000)      870 2024-05-20 15:21:15.012025 qmio-0.1.3/PKG-INFO
+-rw-rw-r--   0 jlopez    (1000) jlopez    (1000)      454 2024-05-15 16:10:48.000000 qmio-0.1.3/README.md
+drwxrwxr-x   0 jlopez    (1000) jlopez    (1000)        0 2024-05-20 15:21:15.008026 qmio-0.1.3/config/
+-rw-rw-r--   0 jlopez    (1000) jlopez    (1000)       50 2024-05-08 10:14:51.000000 qmio-0.1.3/config/__init__.py
+drwxrwxr-x   0 jlopez    (1000) jlopez    (1000)        0 2024-05-20 15:21:15.012025 qmio-0.1.3/qmio/
+-rw-rw-r--   0 jlopez    (1000) jlopez    (1000)       63 2024-05-20 15:20:28.000000 qmio-0.1.3/qmio/__init__.py
+-rw-rw-r--   0 jlopez    (1000) jlopez    (1000)     4714 2024-05-20 15:19:53.000000 qmio-0.1.3/qmio/backends.py
+-rw-rw-r--   0 jlopez    (1000) jlopez    (1000)      346 2024-05-08 09:53:14.000000 qmio-0.1.3/qmio/circuits.py
+-rw-rw-r--   0 jlopez    (1000) jlopez    (1000)     1511 2024-05-08 10:12:16.000000 qmio-0.1.3/qmio/clients.py
+-rw-rw-r--   0 jlopez    (1000) jlopez    (1000)     1092 2024-05-08 07:55:18.000000 qmio-0.1.3/qmio/qmio.py
+-rw-rw-r--   0 jlopez    (1000) jlopez    (1000)      275 2024-05-08 07:55:18.000000 qmio-0.1.3/qmio/services.py
+drwxrwxr-x   0 jlopez    (1000) jlopez    (1000)        0 2024-05-20 15:21:15.012025 qmio-0.1.3/qmio.egg-info/
+-rw-rw-r--   0 jlopez    (1000) jlopez    (1000)      870 2024-05-20 15:21:14.000000 qmio-0.1.3/qmio.egg-info/PKG-INFO
+-rw-rw-r--   0 jlopez    (1000) jlopez    (1000)      380 2024-05-20 15:21:14.000000 qmio-0.1.3/qmio.egg-info/SOURCES.txt
+-rw-rw-r--   0 jlopez    (1000) jlopez    (1000)        1 2024-05-20 15:21:14.000000 qmio-0.1.3/qmio.egg-info/dependency_links.txt
+-rw-rw-r--   0 jlopez    (1000) jlopez    (1000)       21 2024-05-20 15:21:14.000000 qmio-0.1.3/qmio.egg-info/requires.txt
+-rw-rw-r--   0 jlopez    (1000) jlopez    (1000)       18 2024-05-20 15:21:14.000000 qmio-0.1.3/qmio.egg-info/top_level.txt
+-rw-rw-r--   0 jlopez    (1000) jlopez    (1000)      630 2024-05-20 15:21:15.012025 qmio-0.1.3/setup.cfg
+-rw-rw-r--   0 jlopez    (1000) jlopez    (1000)       38 2024-05-08 07:55:18.000000 qmio-0.1.3/setup.py
+drwxrwxr-x   0 jlopez    (1000) jlopez    (1000)        0 2024-05-20 15:21:15.012025 qmio-0.1.3/tests/
+-rw-rw-r--   0 jlopez    (1000) jlopez    (1000)        0 2024-05-08 07:55:18.000000 qmio-0.1.3/tests/__init__.py
+-rw-rw-r--   0 jlopez    (1000) jlopez    (1000)      834 2024-05-08 07:55:18.000000 qmio-0.1.3/tests/test_backends.py
+-rw-rw-r--   0 jlopez    (1000) jlopez    (1000)      412 2024-05-08 07:55:18.000000 qmio-0.1.3/tests/test_services.py
+-rw-rw-r--   0 jlopez    (1000) jlopez    (1000)       35 2024-05-08 07:55:18.000000 qmio-0.1.3/tests/test_zmq_client.py
```

### Comparing `qmio-0.1.2/LICENSE` & `qmio-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qmio-0.1.2/PKG-INFO` & `qmio-0.1.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 Metadata-Version: 2.1
 Name: qmio
-Version: 0.1.2
+Version: 0.1.3
 Summary: Helper python module to interact with the different backends available in Qmio.
 Home-page: https://github.com/javicacheiro/qmio
 Author: 'Javier Cacheiro, Alvaro Caride'
 Author-email: 'javier.cacheiro@gmail.com, a.caride.sanchez@gmail.com'
 License: Apache
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # Qmio
 Python module to interact with the different backends available in the Qmio system at CESGA.
 
+## Installation
+```
+pip install qmio
+```
+
 ## Usage
 ```python
 from qmio import QmioRuntimeService
 
 circuit = 'OPENQASM 3.0;\ninclude "qelib1.inc";\nqreg q[32];\ncreg c[32];\nx q[0];\nmeasure q[0]->c[0];'
 
 service = QmioRuntimeService()
-with service.backend(name="qpu") as backend:
+with service.backend(name='qpu') as backend:
     result = backend.run(circuit=circuit, shots=1000)
 
 print(result)
 ```
```

### Comparing `qmio-0.1.2/qmio/clients.py` & `qmio-0.1.3/qmio/clients.py`

 * *Files identical despite different names*

### Comparing `qmio-0.1.2/qmio/qmio.py` & `qmio-0.1.3/qmio/qmio.py`

 * *Files identical despite different names*

### Comparing `qmio-0.1.2/qmio.egg-info/PKG-INFO` & `qmio-0.1.3/qmio.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 Metadata-Version: 2.1
 Name: qmio
-Version: 0.1.2
+Version: 0.1.3
 Summary: Helper python module to interact with the different backends available in Qmio.
 Home-page: https://github.com/javicacheiro/qmio
 Author: 'Javier Cacheiro, Alvaro Caride'
 Author-email: 'javier.cacheiro@gmail.com, a.caride.sanchez@gmail.com'
 License: Apache
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # Qmio
 Python module to interact with the different backends available in the Qmio system at CESGA.
 
+## Installation
+```
+pip install qmio
+```
+
 ## Usage
 ```python
 from qmio import QmioRuntimeService
 
 circuit = 'OPENQASM 3.0;\ninclude "qelib1.inc";\nqreg q[32];\ncreg c[32];\nx q[0];\nmeasure q[0]->c[0];'
 
 service = QmioRuntimeService()
-with service.backend(name="qpu") as backend:
+with service.backend(name='qpu') as backend:
     result = backend.run(circuit=circuit, shots=1000)
 
 print(result)
 ```
```

### Comparing `qmio-0.1.2/setup.cfg` & `qmio-0.1.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = qmio
-version = 0.1.2
+version = 0.1.3
 author = 'Javier Cacheiro, Alvaro Caride'
 author_email = 'javier.cacheiro@gmail.com, a.caride.sanchez@gmail.com'
 url = https://github.com/javicacheiro/qmio
 license = Apache
 description = Helper python module to interact with the different backends available in Qmio.
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `qmio-0.1.2/tests/test_backends.py` & `qmio-0.1.3/tests/test_backends.py`

 * *Files identical despite different names*

