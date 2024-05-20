# Comparing `tmp/parameterframe-0.1.4.tar.gz` & `tmp/parameterframe-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parameterframe-0.1.4.tar", last modified: Thu May 16 01:51:27 2024, max compression
+gzip compressed data, was "parameterframe-0.1.5.tar", last modified: Mon May 20 02:44:10 2024, max compression
```

## Comparing `parameterframe-0.1.4.tar` & `parameterframe-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:51:27.315345 parameterframe-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-16 01:46:42.000000 parameterframe-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    43745 2024-05-16 01:51:27.315345 parameterframe-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-05-16 01:46:42.000000 parameterframe-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:51:27.315345 parameterframe-0.1.4/parameterframe/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-16 01:51:01.000000 parameterframe-0.1.4/parameterframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   100447 2024-05-16 01:51:01.000000 parameterframe-0.1.4/parameterframe/parameterframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-16 01:51:26.000000 parameterframe-0.1.4/parameterframe/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:51:27.315345 parameterframe-0.1.4/parameterframe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    43745 2024-05-16 01:51:27.000000 parameterframe-0.1.4/parameterframe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-16 01:51:27.000000 parameterframe-0.1.4/parameterframe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 01:51:27.000000 parameterframe-0.1.4/parameterframe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-16 01:51:27.000000 parameterframe-0.1.4/parameterframe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-16 01:51:27.000000 parameterframe-0.1.4/parameterframe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 01:51:27.315345 parameterframe-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:44:10.359867 parameterframe-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-20 02:40:31.000000 parameterframe-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    49146 2024-05-20 02:44:10.359867 parameterframe-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-05-20 02:40:31.000000 parameterframe-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:44:10.359867 parameterframe-0.1.5/parameterframe/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-20 02:43:42.000000 parameterframe-0.1.5/parameterframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   107294 2024-05-20 02:43:42.000000 parameterframe-0.1.5/parameterframe/parameterframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-20 02:44:09.000000 parameterframe-0.1.5/parameterframe/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:44:10.359867 parameterframe-0.1.5/parameterframe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    49146 2024-05-20 02:44:10.000000 parameterframe-0.1.5/parameterframe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-20 02:44:10.000000 parameterframe-0.1.5/parameterframe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 02:44:10.000000 parameterframe-0.1.5/parameterframe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-20 02:44:10.000000 parameterframe-0.1.5/parameterframe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-20 02:44:10.000000 parameterframe-0.1.5/parameterframe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 02:44:10.359867 parameterframe-0.1.5/setup.cfg
```

### Comparing `parameterframe-0.1.4/LICENSE` & `parameterframe-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `parameterframe-0.1.4/PKG-INFO` & `parameterframe-0.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parameterframe
-Version: 0.1.4
+Version: 0.1.5
 Summary: A tool to manage parameters in a form of files, process them, upload to param storage, pull and reconstrut as files.
 Author: Kyrylo Mordan
 Author-email: parachute.repo@gmail.com
 Keywords: ['python','parameter storage']
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -25,29 +25,34 @@
 
 
 ```python
 import sys
 import pandas as pd
 import os
 sys.path.append('../')
-from parameterframe import ParameterFrame, MockerDatabaseConnector, SqlAlchemyDatabaseManager
+from python_modules.parameterframe import ParameterFrame, MockerDatabaseConnector, SqlAlchemyDatabaseManager
 
 ```
 
+    /Users/insani_dei/miniconda3/envs/parameterframe/lib/python3.11/site-packages/tqdm/auto.py:21: TqdmWarning: IProgress not found. Please update jupyter and ipywidgets. See https://ipywidgets.readthedocs.io/en/stable/user_install.html
+      from .autonotebook import tqdm as notebook_tqdm
+
+
 ## Content
 
 1. Adding new solution and uploading it
 2. Processing new files and creating parameter set
 3. Adding parameter set to solution and commiting
 4. Uploading parameter sets
 5. Getting latest parameter set id for solution
 6. Changing parameter set status
 7. Pulling select parameter sets
 8. Reconstructing parameter se
 9. Structure of local commit tables
+10. Scores
 
 ### 1. Adding new solution and uploading it
 
 
 ```python
 # - with database connector for MockerDB
 pf = ParameterFrame(
@@ -801,14 +806,15 @@
       <th>solution_id</th>
       <th>solution_name</th>
       <th>solution_description</th>
       <th>deployment_date</th>
       <th>deprecation_date</th>
       <th>maintainers</th>
       <th>commited_parameter_sets</th>
+      <th>aos</th>
     </tr>
   </thead>
   <tbody>
   </tbody>
 </table>
 </div>
 
@@ -840,19 +846,17 @@
 
 ```python
 pf2.pull_solution(solution_id='b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca',
                   # optionally specify parameter_set_id
                  parameter_set_id=None)
 ```
 
-    HTTP Request: POST http://localhost:8001/search "HTTP/1.1 200 OK"
-    HTTP Request: POST http://localhost:8001/search "HTTP/1.1 200 OK"
-
-
-    HTTP Request: POST http://localhost:8001/search "HTTP/1.1 200 OK"
+    No solutions with b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca could be pulled!
+    No parameter sets were pulled for solution_id b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca
+    Nothing was pulled for b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca
 
 
 
 
 
     True
 
@@ -902,26 +906,30 @@
       <th>solution_id</th>
       <th>solution_name</th>
       <th>solution_description</th>
       <th>deployment_date</th>
       <th>deprecation_date</th>
       <th>maintainers</th>
       <th>commited_parameter_sets</th>
+      <th>aos</th>
+      <th>pos</th>
     </tr>
   </thead>
   <tbody>
     <tr>
       <th>0</th>
       <td>cec89c4cbb8c891d388407ea93d84a5cd4f996af6d5c1b0cc5fe1cb12101acf5</td>
       <td>new_example_solution</td>
       <td>Description of new example solution.</td>
       <td>2024-xx-xx</td>
       <td>None</td>
       <td>some text about maintainers credentials</td>
       <td>6</td>
+      <td>0.397157</td>
+      <td>0.428571</td>
     </tr>
   </tbody>
 </table>
 </div>
 
 
 
@@ -953,70 +961,147 @@
       <th></th>
       <th>parameter_set_id</th>
       <th>parameter_set_name</th>
       <th>parameter_set_description</th>
       <th>deployment_status</th>
       <th>insertion_datetime</th>
       <th>commited_parameters</th>
+      <th>aos</th>
+      <th>pos</th>
     </tr>
   </thead>
   <tbody>
     <tr>
       <th>0</th>
       <td>5779bbf896ebb8f09a6ea252b09f8adb1a416e8780cf1424fb9bb93dbec8deb5</td>
       <td>green_tiny_car_749</td>
       <td></td>
       <td>STAGING</td>
       <td>2024-05-15 01:36:09</td>
       <td>3</td>
+      <td>0.025744</td>
+      <td>0.285714</td>
     </tr>
     <tr>
       <th>1</th>
-      <td>3940d6dd4c0d817625a31141874c54cf0c8d88b24994f7915deb4096b3c8d0cf</td>
-      <td>blue_tiny_television_381</td>
+      <td>73ece98c90d4e0bcce8b523a8e8d2bd4290c68f2a783ea279b39fe4507e42de7</td>
+      <td>blue_fuzzy_refrigerator_297</td>
       <td></td>
       <td>STAGING</td>
-      <td>2024-05-15 00:37:50</td>
-      <td>2</td>
+      <td>2024-05-15 23:57:17</td>
+      <td>1</td>
+      <td>0.000000</td>
+      <td>0.000000</td>
     </tr>
     <tr>
       <th>2</th>
-      <td>2f3ee8e19d91a89298d40984df5e7bdd1f1a48008b2e61c88a7f6f81b4ab23f5</td>
-      <td>silver_happy_car_441</td>
+      <td>82b8c5340454adf83667e59092fedbee28213475fd58ab6b3d95b4fc60f4d45f</td>
+      <td>purple_giant_television_135</td>
       <td></td>
       <td>STAGING</td>
-      <td>2024-05-16 00:03:25</td>
+      <td>2024-05-16 00:05:43</td>
       <td>1</td>
+      <td>0.371413</td>
+      <td>0.142857</td>
     </tr>
     <tr>
       <th>3</th>
-      <td>82b8c5340454adf83667e59092fedbee28213475fd58ab6b3d95b4fc60f4d45f</td>
-      <td>purple_giant_television_135</td>
+      <td>3940d6dd4c0d817625a31141874c54cf0c8d88b24994f7915deb4096b3c8d0cf</td>
+      <td>blue_tiny_television_381</td>
       <td></td>
       <td>STAGING</td>
-      <td>2024-05-16 00:05:43</td>
-      <td>1</td>
+      <td>2024-05-15 00:37:50</td>
+      <td>2</td>
+      <td>0.025744</td>
+      <td>0.285714</td>
     </tr>
     <tr>
       <th>4</th>
       <td>dddc057bc151de9f8fb8caa834c8e13b789cf68cb53299b4c65c23f1e1310acd</td>
       <td>red_sad_scooter_769</td>
       <td></td>
       <td>STAGING</td>
       <td>2024-05-16 00:08:21</td>
       <td>2</td>
+      <td>0.371413</td>
+      <td>0.142857</td>
     </tr>
     <tr>
       <th>5</th>
-      <td>73ece98c90d4e0bcce8b523a8e8d2bd4290c68f2a783ea279b39fe4507e42de7</td>
-      <td>blue_fuzzy_refrigerator_297</td>
+      <td>2f3ee8e19d91a89298d40984df5e7bdd1f1a48008b2e61c88a7f6f81b4ab23f5</td>
+      <td>silver_happy_car_441</td>
       <td></td>
       <td>STAGING</td>
-      <td>2024-05-15 23:57:17</td>
+      <td>2024-05-16 00:03:25</td>
       <td>1</td>
+      <td>0.000000</td>
+      <td>0.000000</td>
+    </tr>
+  </tbody>
+</table>
+</div>
+
+
+
+
+```python
+pf2.show_parameters(solution_id='cec89c4cbb8c891d388407ea93d84a5cd4f996af6d5c1b0cc5fe1cb12101acf5',
+                    parameter_set_id='3940d6dd4c0d817625a31141874c54cf0c8d88b24994f7915deb4096b3c8d0cf')
+```
+
+
+
+
+<div>
+<style scoped>
+    .dataframe tbody tr th:only-of-type {
+        vertical-align: middle;
+    }
+
+    .dataframe tbody tr th {
+        vertical-align: top;
+    }
+
+    .dataframe thead th {
+        text-align: right;
+    }
+</style>
+<table border="1" class="dataframe">
+  <thead>
+    <tr style="text-align: right;">
+      <th></th>
+      <th>parameter_id</th>
+      <th>parameter_name</th>
+      <th>parameter_description</th>
+      <th>file_name</th>
+      <th>file_type</th>
+      <th>commited_attributes</th>
+      <th>aos</th>
+    </tr>
+  </thead>
+  <tbody>
+    <tr>
+      <th>0</th>
+      <td>3386ebc962b1c57745ca24320bf873df6eb84a2b9cb733607d72006347bf95b8</td>
+      <td>Screenshot 2024-05-04 at 02</td>
+      <td></td>
+      <td>Screenshot 2024-05-04 at 02.59.31.png</td>
+      <td>other</td>
+      <td>35</td>
+      <td>0.0</td>
+    </tr>
+    <tr>
+      <th>1</th>
+      <td>5afae3951544cd3736685a3b2daa31c00106191a799b96b0c636cd35e9a416ff</td>
+      <td>uploads</td>
+      <td></td>
+      <td>uploads.zip</td>
+      <td>other</td>
+      <td>61</td>
+      <td>0.0</td>
     </tr>
   </tbody>
 </table>
 </div>
 
 
 
@@ -1049,43 +1134,163 @@
       <th></th>
       <th>parameter_id</th>
       <th>parameter_name</th>
       <th>parameter_description</th>
       <th>file_name</th>
       <th>file_type</th>
       <th>commited_attributes</th>
+      <th>aos</th>
     </tr>
   </thead>
   <tbody>
     <tr>
       <th>0</th>
       <td>3386ebc962b1c57745ca24320bf873df6eb84a2b9cb733607d72006347bf95b8</td>
       <td>Screenshot 2024-05-04 at 02</td>
       <td></td>
       <td>Screenshot 2024-05-04 at 02.59.31.png</td>
       <td>other</td>
       <td>35</td>
+      <td>0.0</td>
     </tr>
     <tr>
       <th>1</th>
       <td>4d8ca206d9bd09296b69a95f0c3c62d233282025964c356811510cc074cc2c49</td>
       <td>1</td>
       <td></td>
       <td>1. AF - opis projektu.pdf</td>
       <td>other</td>
       <td>34</td>
+      <td>0.0</td>
     </tr>
     <tr>
       <th>2</th>
       <td>5afae3951544cd3736685a3b2daa31c00106191a799b96b0c636cd35e9a416ff</td>
       <td>uploads</td>
       <td></td>
       <td>uploads.zip</td>
       <td>other</td>
       <td>61</td>
+      <td>0.0</td>
+    </tr>
+  </tbody>
+</table>
+</div>
+
+
+
+
+```python
+pf2.show_parameters(solution_id='cec89c4cbb8c891d388407ea93d84a5cd4f996af6d5c1b0cc5fe1cb12101acf5',
+                    parameter_set_id='dddc057bc151de9f8fb8caa834c8e13b789cf68cb53299b4c65c23f1e1310acd')
+```
+
+
+
+
+<div>
+<style scoped>
+    .dataframe tbody tr th:only-of-type {
+        vertical-align: middle;
+    }
+
+    .dataframe tbody tr th {
+        vertical-align: top;
+    }
+
+    .dataframe thead th {
+        text-align: right;
+    }
+</style>
+<table border="1" class="dataframe">
+  <thead>
+    <tr style="text-align: right;">
+      <th></th>
+      <th>parameter_id</th>
+      <th>parameter_name</th>
+      <th>parameter_description</th>
+      <th>file_name</th>
+      <th>file_type</th>
+      <th>commited_attributes</th>
+      <th>aos</th>
+    </tr>
+  </thead>
+  <tbody>
+    <tr>
+      <th>0</th>
+      <td>e6ae9d10f3b4d69c1ef6ff8038d13e9f0b093fc3710f2fed0259204aac2fcba4</td>
+      <td>Geekbench 6</td>
+      <td></td>
+      <td>Geekbench 6.app.zip</td>
+      <td>other</td>
+      <td>1385</td>
+      <td>0.0</td>
+    </tr>
+    <tr>
+      <th>1</th>
+      <td>be0886c2f5d24aa5672bf84e355d9d4adb527a36e5e973413c555200d7f3fdb2</td>
+      <td>Ollama</td>
+      <td></td>
+      <td>Ollama.app.zip</td>
+      <td>other</td>
+      <td>1400</td>
+      <td>0.0</td>
+    </tr>
+  </tbody>
+</table>
+</div>
+
+
+
+
+```python
+pf2.show_parameters(solution_id='cec89c4cbb8c891d388407ea93d84a5cd4f996af6d5c1b0cc5fe1cb12101acf5',
+                    parameter_set_id='82b8c5340454adf83667e59092fedbee28213475fd58ab6b3d95b4fc60f4d45f')
+```
+
+
+
+
+<div>
+<style scoped>
+    .dataframe tbody tr th:only-of-type {
+        vertical-align: middle;
+    }
+
+    .dataframe tbody tr th {
+        vertical-align: top;
+    }
+
+    .dataframe thead th {
+        text-align: right;
+    }
+</style>
+<table border="1" class="dataframe">
+  <thead>
+    <tr style="text-align: right;">
+      <th></th>
+      <th>parameter_id</th>
+      <th>parameter_name</th>
+      <th>parameter_description</th>
+      <th>file_name</th>
+      <th>file_type</th>
+      <th>commited_attributes</th>
+      <th>aos</th>
+    </tr>
+  </thead>
+  <tbody>
+    <tr>
+      <th>0</th>
+      <td>e6ae9d10f3b4d69c1ef6ff8038d13e9f0b093fc3710f2fed0259204aac2fcba4</td>
+      <td>Geekbench 6</td>
+      <td></td>
+      <td>Geekbench 6.app.zip</td>
+      <td>other</td>
+      <td>1385</td>
+      <td>0.0</td>
     </tr>
   </tbody>
 </table>
 </div>
 
 
 
@@ -1833,7 +2038,28 @@
       <td>bytes</td>
     </tr>
   </tbody>
 </table>
 </div>
 
 
+
+### 10. Scores
+
+##### I. Attribute overlap ratio
+
+AOR represents an overlap ratio between attribute ids that:
+
+- belong to a parameter within parameter set
+- belong to a parameter sets within solution
+- belong to a solution within solutions
+
+The score is between $0$ and $1$, and the greater the score, the greater is an overlap between attribute ids within select group and non unique attribute ids.
+
+##### II. Parameter overlap ratio
+
+POR represents an overlap ratio between parameter ids that:
+
+- belong to a parameter sets within solution
+- belong to a solution within solutions
+
+The score is between $0$ and $1$, and the greater the score, the greater is an overlap between parameter ids within select group and non unique parameter ids.
```

### Comparing `parameterframe-0.1.4/README.md` & `parameterframe-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 [module](python_modules/shouterlog.py) | [usage](docs/shouterlog.md) | [![PyPiVersion](https://img.shields.io/pypi/v/shouterlog)](https://pypi.org/project/shouterlog/) - Shouter Log
 
 This class uses the logging module to create and manage a logger for displaying formatted messages.
 It provides a method to output various types of lines and headers, with customizable message and line lengths.
 The purpose is to be integrated into other classes that also use logger.
 
-[module](python_modules/gridlooper.py) | [usage](docs/gridlooper.md) | [drawio: -flow](docs/gridlooper-flow.png) | [![PyPiVersion](https://img.shields.io/pypi/v/gridlooper)](https://pypi.org/project/gridlooper/) - Grid Looper
+[module](python_modules/gridlooper.py) | [usage](docs/gridlooper.md) | [drawio: -flow](docs/gridlooper-flow.png) | [release notes](release_notes/gridlooper.md) | [![PyPiVersion](https://img.shields.io/pypi/v/gridlooper)](https://pypi.org/project/gridlooper/) - Grid Looper
 
 A tool to run experiments based on defined grid and function with single iteration.
 
 [module](python_modules/mocker_db.py) | [usage](docs/mocker_db.md) | [drawio: -flow](docs/mocker_db-flow.png) | [release notes](release_notes/mocker_db.md) | [![PyPiVersion](https://img.shields.io/pypi/v/mocker-db)](https://pypi.org/project/mocker-db/) - MockerDB
 
 A python module that contains mock vector database like solution built around
 dictionary data type. It contains methods necessary to interact with this 'database',
```

### Comparing `parameterframe-0.1.4/parameterframe/parameterframe.py` & `parameterframe-0.1.5/parameterframe/parameterframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -2470,14 +2470,162 @@
         self.database_connector.modify_parameter_set_status(
                 solution_id=solution_id,
                 parameter_set_ids = parameter_set_id,
                 current_deployment_status = "ARCHIVED",
                 new_deployment_status = "PRODUCTION"
             )
 
+    def _overlap_score(self,
+                        ids : list,
+                        id_dict : dict,
+                        group_ids : list) -> dict:
+
+        scores = {}
+
+        ids_value_counts = pd.Series(ids).value_counts()
+        ids_value_counts_norm = ids_value_counts - 1
+        pivc_freq = ids_value_counts_norm/len(ids_value_counts_norm)
+
+        for id in group_ids:
+            sc = pivc_freq[pivc_freq.index.isin(id_dict[id])]
+            score = sum(sc)
+            scores[id] = score
+
+        return scores
+
+
+    def _make_parameter_attribute_overlap_scores(self,
+                                                show_parameters,
+                                                solution_id : str,
+                                                parameter_set_id : str):
+
+        parameter_ids = show_parameters['parameter_id']
+
+        attribute_ids = []
+        attribute_id_dict = {}
+
+        for paramter_id in parameter_ids:
+            # extract attributes for parameters
+            atrids_dict = self.commited_tables[solution_id]['parameter_attribute'][parameter_set_id][paramter_id]
+
+
+            atrids = [atrid['attribute_id'] for atrid in atrids_dict]
+
+            attribute_id_dict[paramter_id] = atrids
+            attribute_ids = attribute_ids + atrids
+
+
+        scores = self._overlap_score(ids = attribute_ids,
+                                        id_dict = attribute_id_dict,
+                                        group_ids = parameter_ids)
+
+        return scores, attribute_ids
+
+    def _make_parameter_set_attribute_overlap_scores(self, solution_id : str, show_parameter_sets):
+
+        parameter_set_ids = show_parameter_sets['parameter_set_id']
+
+        ps_attribute_ids = []
+        ps_attribute_id_dict = {}
+
+
+        for parameter_set_id in parameter_set_ids:
+
+            show_parameters = self.show_parameters(solution_id=solution_id,
+                            parameter_set_id=parameter_set_id)
+
+            _, attribute_ids = self._make_parameter_attribute_overlap_scores(
+                show_parameters = show_parameters,
+                solution_id = solution_id,
+                parameter_set_id = parameter_set_id)
+
+            ps_attribute_id_dict[parameter_set_id] = attribute_ids
+            ps_attribute_ids = ps_attribute_ids + attribute_ids
+
+
+        scores = self._overlap_score(ids = ps_attribute_ids,
+                                        id_dict = ps_attribute_id_dict,
+                                        group_ids = parameter_set_ids)
+
+
+        return scores, ps_attribute_ids
+
+    def _make_parameter_set_parameter_overlap_scores(self, solution_id : str, show_parameter_sets):
+
+        parameter_set_ids = show_parameter_sets['parameter_set_id']
+
+        ps_parameter_ids = []
+        ps_parameter_id_dict = {}
+
+
+        for parameter_set_id in parameter_set_ids:
+
+            # extract attributes for parameters
+            prids_dict = self.commited_tables[solution_id]['parameter_attribute'][parameter_set_id]
+
+            prids = [parameter_id for parameter_id in prids_dict]
+
+            ps_parameter_id_dict[parameter_set_id] = prids
+            ps_parameter_ids = ps_parameter_ids + prids
+
+        scores = self._overlap_score(ids = ps_parameter_ids,
+                                        id_dict = ps_parameter_id_dict,
+                                        group_ids = parameter_set_ids)
+
+
+        return scores, ps_parameter_ids
+
+    def _make_solution_attribute_overlap_scores(self, show_solutions):
+
+        solution_ids = show_solutions['solution_id']
+
+        s_attribute_ids = []
+        s_attribute_id_dict = {}
+
+        for solution_id in solution_ids:
+
+            show_parameter_sets = self.show_parameter_sets(solution_id=solution_id)
+
+            _, attribute_ids = self._make_parameter_set_attribute_overlap_scores(
+                show_parameter_sets = show_parameter_sets,
+                solution_id = solution_id)
+
+            s_attribute_id_dict[solution_id] = attribute_ids
+            s_attribute_ids = s_attribute_ids + attribute_ids
+
+        scores = self._overlap_score(ids = s_attribute_ids,
+                                        id_dict = s_attribute_id_dict,
+                                        group_ids = solution_ids)
+
+        return scores
+
+    def _make_solution_parameter_overlap_scores(self, show_solutions):
+
+        solution_ids = show_solutions['solution_id']
+
+        s_parameter_ids = []
+        s_parameter_id_dict = {}
+
+        for solution_id in solution_ids:
+
+            show_parameter_sets = self.show_parameter_sets(solution_id=solution_id)
+
+            _, parameter_ids = self._make_parameter_set_parameter_overlap_scores(
+                show_parameter_sets = show_parameter_sets,
+                solution_id = solution_id)
+
+            s_parameter_id_dict[solution_id] = parameter_ids
+            s_parameter_ids = s_parameter_ids + parameter_ids
+
+        scores = self._overlap_score(ids = s_parameter_ids,
+                                        id_dict = s_parameter_id_dict,
+                                        group_ids = solution_ids)
+
+        return scores
+
     def show_solutions(self):
 
         """
         Show info on locally commited solutions
         """
 
         solution_descriptions = [self.commited_tables[sid]['solution_description'][0] \
@@ -2506,14 +2654,26 @@
         solution_descriptions_pd['commited_parameter_sets'] = [
                     len(self.commited_tables[sid]['solution_parameter_set']) \
                     if self.commited_tables[sid]['solution_parameter_set'] != {}\
                     else 0
                     for sid in self.commited_tables
                 ]
 
+        solution_attribute_overlap_scores = self._make_solution_attribute_overlap_scores(
+            show_solutions=solution_descriptions_pd)
+
+        solution_descriptions_pd['aos'] = [solution_attribute_overlap_scores[solution_id] \
+            for solution_id in solution_descriptions_pd['solution_id']]
+
+        solution_parameter_overlap_scores = self._make_solution_parameter_overlap_scores(
+            show_solutions=solution_descriptions_pd)
+
+        solution_descriptions_pd['pos'] = [solution_parameter_overlap_scores[solution_id] \
+            for solution_id in solution_descriptions_pd['solution_id']]
+
         return solution_descriptions_pd
 
     def show_parameter_sets(self, solution_id : str):
 
         """
         Show info on locally commited parameter_sets for solution_id
         """
@@ -2537,14 +2697,28 @@
 
         psdsp_id_pd = parameter_set_descriptions_pd.merge(
             solution_parameter_sets_pd, on = 'parameter_set_id')
         psdsp_id_pd['commited_parameters'] = [
             len(self.commited_tables[solution_id]['parameter_set'][pid_d['parameter_set_id']]) \
                 for pid_d in parameter_set_descriptions]
 
+        parameter_set_attribute_overlap_scores, _ = self._make_parameter_set_attribute_overlap_scores(
+            solution_id = solution_id,
+            show_parameter_sets = psdsp_id_pd)
+
+        psdsp_id_pd['aos'] = [parameter_set_attribute_overlap_scores[parameter_set_id] \
+            for parameter_set_id in psdsp_id_pd['parameter_set_id']]
+
+        parameter_set_parameter_overlap_scores, _ = self._make_parameter_set_parameter_overlap_scores(
+            solution_id = solution_id,
+            show_parameter_sets = psdsp_id_pd)
+
+        psdsp_id_pd['pos'] = [parameter_set_parameter_overlap_scores[parameter_set_id] \
+            for parameter_set_id in psdsp_id_pd['parameter_set_id']]
+
         return psdsp_id_pd
 
     def show_parameters(self, solution_id : str, parameter_set_id : str):
 
         """
         Show info on locally commited parameters for solution_id and parameter_set_id
         """
@@ -2554,13 +2728,22 @@
 
         parameter_descriptions = self.commited_tables[solution_id]['parameter_description'][parameter_set_id]
         parameter_descriptions_l = [parameter_descriptions[pid][0] for pid in parameter_descriptions]
         parameter_descriptions_pd = self.pd.DataFrame(parameter_descriptions_l)
         parameter_descriptions_pd['commited_attributes'] = [
             len(self.commited_tables[solution_id]['parameter_attribute'][parameter_set_id][parameter_id]) \
                 for parameter_id in parameter_descriptions]
+
+        parameter_attribute_overlap_scores, _ = self._make_parameter_attribute_overlap_scores(
+            show_parameters = parameter_descriptions_pd,
+            solution_id = solution_id,
+            parameter_set_id = parameter_set_id)
+
+        parameter_descriptions_pd['aos'] = [parameter_attribute_overlap_scores[parameter_id] \
+            for parameter_id in parameter_descriptions_pd['parameter_id']]
+
         return parameter_descriptions_pd
```

### Comparing `parameterframe-0.1.4/parameterframe/setup.py` & `parameterframe-0.1.5/parameterframe/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,14 @@
       long_description = fh.read()
 else:
   long_description = ''
 
 setup(
     name="parameterframe",
     packages=["parameterframe"],
-    install_requires=['### parameterframe.py', 'pandas', 'pyyaml', 'sqlalchemy', 'attrs', 'dill', 'cryptography', 'mocker_db==0.1.1'],
+    install_requires=['### parameterframe.py', 'pyyaml', 'pandas', 'cryptography', 'dill', 'mocker_db==0.1.1', 'sqlalchemy', 'attrs'],
     classifiers=['Development Status :: 3 - Alpha', 'Intended Audience :: Developers', 'Intended Audience :: Science/Research', 'Programming Language :: Python :: 3', 'Programming Language :: Python :: 3.9', 'Programming Language :: Python :: 3.10', 'Programming Language :: Python :: 3.11', 'License :: OSI Approved :: MIT License', 'Topic :: Scientific/Engineering'],
     long_description=long_description,
     long_description_content_type='text/markdown',
-    author="Kyrylo Mordan", author_email="parachute.repo@gmail.com", description="A tool to manage parameters in a form of files, process them, upload to param storage, pull and reconstrut as files.", keywords="['python', 'parameter storage']", version="0.1.4"
+    author="Kyrylo Mordan", author_email="parachute.repo@gmail.com", description="A tool to manage parameters in a form of files, process them, upload to param storage, pull and reconstrut as files.", keywords="['python', 'parameter storage']", version="0.1.5"
 )
```

### Comparing `parameterframe-0.1.4/parameterframe.egg-info/PKG-INFO` & `parameterframe-0.1.5/parameterframe.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parameterframe
-Version: 0.1.4
+Version: 0.1.5
 Summary: A tool to manage parameters in a form of files, process them, upload to param storage, pull and reconstrut as files.
 Author: Kyrylo Mordan
 Author-email: parachute.repo@gmail.com
 Keywords: ['python','parameter storage']
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -25,29 +25,34 @@
 
 
 ```python
 import sys
 import pandas as pd
 import os
 sys.path.append('../')
-from parameterframe import ParameterFrame, MockerDatabaseConnector, SqlAlchemyDatabaseManager
+from python_modules.parameterframe import ParameterFrame, MockerDatabaseConnector, SqlAlchemyDatabaseManager
 
 ```
 
+    /Users/insani_dei/miniconda3/envs/parameterframe/lib/python3.11/site-packages/tqdm/auto.py:21: TqdmWarning: IProgress not found. Please update jupyter and ipywidgets. See https://ipywidgets.readthedocs.io/en/stable/user_install.html
+      from .autonotebook import tqdm as notebook_tqdm
+
+
 ## Content
 
 1. Adding new solution and uploading it
 2. Processing new files and creating parameter set
 3. Adding parameter set to solution and commiting
 4. Uploading parameter sets
 5. Getting latest parameter set id for solution
 6. Changing parameter set status
 7. Pulling select parameter sets
 8. Reconstructing parameter se
 9. Structure of local commit tables
+10. Scores
 
 ### 1. Adding new solution and uploading it
 
 
 ```python
 # - with database connector for MockerDB
 pf = ParameterFrame(
@@ -801,14 +806,15 @@
       <th>solution_id</th>
       <th>solution_name</th>
       <th>solution_description</th>
       <th>deployment_date</th>
       <th>deprecation_date</th>
       <th>maintainers</th>
       <th>commited_parameter_sets</th>
+      <th>aos</th>
     </tr>
   </thead>
   <tbody>
   </tbody>
 </table>
 </div>
 
@@ -840,19 +846,17 @@
 
 ```python
 pf2.pull_solution(solution_id='b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca',
                   # optionally specify parameter_set_id
                  parameter_set_id=None)
 ```
 
-    HTTP Request: POST http://localhost:8001/search "HTTP/1.1 200 OK"
-    HTTP Request: POST http://localhost:8001/search "HTTP/1.1 200 OK"
-
-
-    HTTP Request: POST http://localhost:8001/search "HTTP/1.1 200 OK"
+    No solutions with b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca could be pulled!
+    No parameter sets were pulled for solution_id b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca
+    Nothing was pulled for b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca
 
 
 
 
 
     True
 
@@ -902,26 +906,30 @@
       <th>solution_id</th>
       <th>solution_name</th>
       <th>solution_description</th>
       <th>deployment_date</th>
       <th>deprecation_date</th>
       <th>maintainers</th>
       <th>commited_parameter_sets</th>
+      <th>aos</th>
+      <th>pos</th>
     </tr>
   </thead>
   <tbody>
     <tr>
       <th>0</th>
       <td>cec89c4cbb8c891d388407ea93d84a5cd4f996af6d5c1b0cc5fe1cb12101acf5</td>
       <td>new_example_solution</td>
       <td>Description of new example solution.</td>
       <td>2024-xx-xx</td>
       <td>None</td>
       <td>some text about maintainers credentials</td>
       <td>6</td>
+      <td>0.397157</td>
+      <td>0.428571</td>
     </tr>
   </tbody>
 </table>
 </div>
 
 
 
@@ -953,70 +961,147 @@
       <th></th>
       <th>parameter_set_id</th>
       <th>parameter_set_name</th>
       <th>parameter_set_description</th>
       <th>deployment_status</th>
       <th>insertion_datetime</th>
       <th>commited_parameters</th>
+      <th>aos</th>
+      <th>pos</th>
     </tr>
   </thead>
   <tbody>
     <tr>
       <th>0</th>
       <td>5779bbf896ebb8f09a6ea252b09f8adb1a416e8780cf1424fb9bb93dbec8deb5</td>
       <td>green_tiny_car_749</td>
       <td></td>
       <td>STAGING</td>
       <td>2024-05-15 01:36:09</td>
       <td>3</td>
+      <td>0.025744</td>
+      <td>0.285714</td>
     </tr>
     <tr>
       <th>1</th>
-      <td>3940d6dd4c0d817625a31141874c54cf0c8d88b24994f7915deb4096b3c8d0cf</td>
-      <td>blue_tiny_television_381</td>
+      <td>73ece98c90d4e0bcce8b523a8e8d2bd4290c68f2a783ea279b39fe4507e42de7</td>
+      <td>blue_fuzzy_refrigerator_297</td>
       <td></td>
       <td>STAGING</td>
-      <td>2024-05-15 00:37:50</td>
-      <td>2</td>
+      <td>2024-05-15 23:57:17</td>
+      <td>1</td>
+      <td>0.000000</td>
+      <td>0.000000</td>
     </tr>
     <tr>
       <th>2</th>
-      <td>2f3ee8e19d91a89298d40984df5e7bdd1f1a48008b2e61c88a7f6f81b4ab23f5</td>
-      <td>silver_happy_car_441</td>
+      <td>82b8c5340454adf83667e59092fedbee28213475fd58ab6b3d95b4fc60f4d45f</td>
+      <td>purple_giant_television_135</td>
       <td></td>
       <td>STAGING</td>
-      <td>2024-05-16 00:03:25</td>
+      <td>2024-05-16 00:05:43</td>
       <td>1</td>
+      <td>0.371413</td>
+      <td>0.142857</td>
     </tr>
     <tr>
       <th>3</th>
-      <td>82b8c5340454adf83667e59092fedbee28213475fd58ab6b3d95b4fc60f4d45f</td>
-      <td>purple_giant_television_135</td>
+      <td>3940d6dd4c0d817625a31141874c54cf0c8d88b24994f7915deb4096b3c8d0cf</td>
+      <td>blue_tiny_television_381</td>
       <td></td>
       <td>STAGING</td>
-      <td>2024-05-16 00:05:43</td>
-      <td>1</td>
+      <td>2024-05-15 00:37:50</td>
+      <td>2</td>
+      <td>0.025744</td>
+      <td>0.285714</td>
     </tr>
     <tr>
       <th>4</th>
       <td>dddc057bc151de9f8fb8caa834c8e13b789cf68cb53299b4c65c23f1e1310acd</td>
       <td>red_sad_scooter_769</td>
       <td></td>
       <td>STAGING</td>
       <td>2024-05-16 00:08:21</td>
       <td>2</td>
+      <td>0.371413</td>
+      <td>0.142857</td>
     </tr>
     <tr>
       <th>5</th>
-      <td>73ece98c90d4e0bcce8b523a8e8d2bd4290c68f2a783ea279b39fe4507e42de7</td>
-      <td>blue_fuzzy_refrigerator_297</td>
+      <td>2f3ee8e19d91a89298d40984df5e7bdd1f1a48008b2e61c88a7f6f81b4ab23f5</td>
+      <td>silver_happy_car_441</td>
       <td></td>
       <td>STAGING</td>
-      <td>2024-05-15 23:57:17</td>
+      <td>2024-05-16 00:03:25</td>
       <td>1</td>
+      <td>0.000000</td>
+      <td>0.000000</td>
+    </tr>
+  </tbody>
+</table>
+</div>
+
+
+
+
+```python
+pf2.show_parameters(solution_id='cec89c4cbb8c891d388407ea93d84a5cd4f996af6d5c1b0cc5fe1cb12101acf5',
+                    parameter_set_id='3940d6dd4c0d817625a31141874c54cf0c8d88b24994f7915deb4096b3c8d0cf')
+```
+
+
+
+
+<div>
+<style scoped>
+    .dataframe tbody tr th:only-of-type {
+        vertical-align: middle;
+    }
+
+    .dataframe tbody tr th {
+        vertical-align: top;
+    }
+
+    .dataframe thead th {
+        text-align: right;
+    }
+</style>
+<table border="1" class="dataframe">
+  <thead>
+    <tr style="text-align: right;">
+      <th></th>
+      <th>parameter_id</th>
+      <th>parameter_name</th>
+      <th>parameter_description</th>
+      <th>file_name</th>
+      <th>file_type</th>
+      <th>commited_attributes</th>
+      <th>aos</th>
+    </tr>
+  </thead>
+  <tbody>
+    <tr>
+      <th>0</th>
+      <td>3386ebc962b1c57745ca24320bf873df6eb84a2b9cb733607d72006347bf95b8</td>
+      <td>Screenshot 2024-05-04 at 02</td>
+      <td></td>
+      <td>Screenshot 2024-05-04 at 02.59.31.png</td>
+      <td>other</td>
+      <td>35</td>
+      <td>0.0</td>
+    </tr>
+    <tr>
+      <th>1</th>
+      <td>5afae3951544cd3736685a3b2daa31c00106191a799b96b0c636cd35e9a416ff</td>
+      <td>uploads</td>
+      <td></td>
+      <td>uploads.zip</td>
+      <td>other</td>
+      <td>61</td>
+      <td>0.0</td>
     </tr>
   </tbody>
 </table>
 </div>
 
 
 
@@ -1049,43 +1134,163 @@
       <th></th>
       <th>parameter_id</th>
       <th>parameter_name</th>
       <th>parameter_description</th>
       <th>file_name</th>
       <th>file_type</th>
       <th>commited_attributes</th>
+      <th>aos</th>
     </tr>
   </thead>
   <tbody>
     <tr>
       <th>0</th>
       <td>3386ebc962b1c57745ca24320bf873df6eb84a2b9cb733607d72006347bf95b8</td>
       <td>Screenshot 2024-05-04 at 02</td>
       <td></td>
       <td>Screenshot 2024-05-04 at 02.59.31.png</td>
       <td>other</td>
       <td>35</td>
+      <td>0.0</td>
     </tr>
     <tr>
       <th>1</th>
       <td>4d8ca206d9bd09296b69a95f0c3c62d233282025964c356811510cc074cc2c49</td>
       <td>1</td>
       <td></td>
       <td>1. AF - opis projektu.pdf</td>
       <td>other</td>
       <td>34</td>
+      <td>0.0</td>
     </tr>
     <tr>
       <th>2</th>
       <td>5afae3951544cd3736685a3b2daa31c00106191a799b96b0c636cd35e9a416ff</td>
       <td>uploads</td>
       <td></td>
       <td>uploads.zip</td>
       <td>other</td>
       <td>61</td>
+      <td>0.0</td>
+    </tr>
+  </tbody>
+</table>
+</div>
+
+
+
+
+```python
+pf2.show_parameters(solution_id='cec89c4cbb8c891d388407ea93d84a5cd4f996af6d5c1b0cc5fe1cb12101acf5',
+                    parameter_set_id='dddc057bc151de9f8fb8caa834c8e13b789cf68cb53299b4c65c23f1e1310acd')
+```
+
+
+
+
+<div>
+<style scoped>
+    .dataframe tbody tr th:only-of-type {
+        vertical-align: middle;
+    }
+
+    .dataframe tbody tr th {
+        vertical-align: top;
+    }
+
+    .dataframe thead th {
+        text-align: right;
+    }
+</style>
+<table border="1" class="dataframe">
+  <thead>
+    <tr style="text-align: right;">
+      <th></th>
+      <th>parameter_id</th>
+      <th>parameter_name</th>
+      <th>parameter_description</th>
+      <th>file_name</th>
+      <th>file_type</th>
+      <th>commited_attributes</th>
+      <th>aos</th>
+    </tr>
+  </thead>
+  <tbody>
+    <tr>
+      <th>0</th>
+      <td>e6ae9d10f3b4d69c1ef6ff8038d13e9f0b093fc3710f2fed0259204aac2fcba4</td>
+      <td>Geekbench 6</td>
+      <td></td>
+      <td>Geekbench 6.app.zip</td>
+      <td>other</td>
+      <td>1385</td>
+      <td>0.0</td>
+    </tr>
+    <tr>
+      <th>1</th>
+      <td>be0886c2f5d24aa5672bf84e355d9d4adb527a36e5e973413c555200d7f3fdb2</td>
+      <td>Ollama</td>
+      <td></td>
+      <td>Ollama.app.zip</td>
+      <td>other</td>
+      <td>1400</td>
+      <td>0.0</td>
+    </tr>
+  </tbody>
+</table>
+</div>
+
+
+
+
+```python
+pf2.show_parameters(solution_id='cec89c4cbb8c891d388407ea93d84a5cd4f996af6d5c1b0cc5fe1cb12101acf5',
+                    parameter_set_id='82b8c5340454adf83667e59092fedbee28213475fd58ab6b3d95b4fc60f4d45f')
+```
+
+
+
+
+<div>
+<style scoped>
+    .dataframe tbody tr th:only-of-type {
+        vertical-align: middle;
+    }
+
+    .dataframe tbody tr th {
+        vertical-align: top;
+    }
+
+    .dataframe thead th {
+        text-align: right;
+    }
+</style>
+<table border="1" class="dataframe">
+  <thead>
+    <tr style="text-align: right;">
+      <th></th>
+      <th>parameter_id</th>
+      <th>parameter_name</th>
+      <th>parameter_description</th>
+      <th>file_name</th>
+      <th>file_type</th>
+      <th>commited_attributes</th>
+      <th>aos</th>
+    </tr>
+  </thead>
+  <tbody>
+    <tr>
+      <th>0</th>
+      <td>e6ae9d10f3b4d69c1ef6ff8038d13e9f0b093fc3710f2fed0259204aac2fcba4</td>
+      <td>Geekbench 6</td>
+      <td></td>
+      <td>Geekbench 6.app.zip</td>
+      <td>other</td>
+      <td>1385</td>
+      <td>0.0</td>
     </tr>
   </tbody>
 </table>
 </div>
 
 
 
@@ -1833,7 +2038,28 @@
       <td>bytes</td>
     </tr>
   </tbody>
 </table>
 </div>
 
 
+
+### 10. Scores
+
+##### I. Attribute overlap ratio
+
+AOR represents an overlap ratio between attribute ids that:
+
+- belong to a parameter within parameter set
+- belong to a parameter sets within solution
+- belong to a solution within solutions
+
+The score is between $0$ and $1$, and the greater the score, the greater is an overlap between attribute ids within select group and non unique attribute ids.
+
+##### II. Parameter overlap ratio
+
+POR represents an overlap ratio between parameter ids that:
+
+- belong to a parameter sets within solution
+- belong to a solution within solutions
+
+The score is between $0$ and $1$, and the greater the score, the greater is an overlap between parameter ids within select group and non unique parameter ids.
```

