# Comparing `tmp/kapoorlabs_lightning-5.3.7.tar.gz` & `tmp/kapoorlabs_lightning-5.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kapoorlabs_lightning-5.3.7.tar", last modified: Fri May 17 20:18:54 2024, max compression
+gzip compressed data, was "kapoorlabs_lightning-5.3.8.tar", last modified: Mon May 20 17:23:54 2024, max compression
```

## Comparing `kapoorlabs_lightning-5.3.7.tar` & `kapoorlabs_lightning-5.3.8.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-17 20:18:54.343373 kapoorlabs_lightning-5.3.7/
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-17 20:18:54.335373 kapoorlabs_lightning-5.3.7/.github/
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-17 20:18:54.339373 kapoorlabs_lightning-5.3.7/.github/workflows/
--rw-r--r--   0 debian    (1000) debian    (1000)     1068 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/.github/workflows/deploy.yml
--rw-r--r--   0 debian    (1000) debian    (1000)     1963 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 debian    (1000) debian    (1000)      991 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/.gitignore
--rw-r--r--   0 debian    (1000) debian    (1000)     1008 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/.pre-commit-config.yaml
--rw-r--r--   0 debian    (1000) debian    (1000)     1487 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/LICENSE
--rw-r--r--   0 debian    (1000) debian    (1000)       96 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/MANIFEST.in
--rw-r--r--   0 debian    (1000) debian    (1000)     4108 2024-05-17 20:18:54.343373 kapoorlabs_lightning-5.3.7/PKG-INFO
--rw-r--r--   0 debian    (1000) debian    (1000)     2435 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/README.md
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-17 20:18:54.339373 kapoorlabs_lightning-5.3.7/licenses/
--rw-r--r--   0 debian    (1000) debian    (1000)    11358 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/licenses/Apache-2
--rw-r--r--   0 debian    (1000) debian    (1000)     1487 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/licenses/BSD-3
--rw-r--r--   0 debian    (1000) debian    (1000)    35148 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/licenses/GPL-3
--rw-r--r--   0 debian    (1000) debian    (1000)     7653 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/licenses/LGPL-3
--rw-r--r--   0 debian    (1000) debian    (1000)     1080 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/licenses/MIT
--rw-r--r--   0 debian    (1000) debian    (1000)    16726 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/licenses/MPL-2
--rw-r--r--   0 debian    (1000) debian    (1000)      116 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/pyproject.toml
--rw-r--r--   0 debian    (1000) debian    (1000)     1766 2024-05-17 20:18:54.343373 kapoorlabs_lightning-5.3.7/setup.cfg
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-17 20:18:54.335373 kapoorlabs_lightning-5.3.7/src/
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-17 20:18:54.343373 kapoorlabs_lightning-5.3.7/src/KapoorLabs_Lightning.egg-info/
--rw-r--r--   0 debian    (1000) debian    (1000)     4108 2024-05-17 20:18:54.000000 kapoorlabs_lightning-5.3.7/src/KapoorLabs_Lightning.egg-info/PKG-INFO
--rw-r--r--   0 debian    (1000) debian    (1000)     1269 2024-05-17 20:18:54.000000 kapoorlabs_lightning-5.3.7/src/KapoorLabs_Lightning.egg-info/SOURCES.txt
--rw-r--r--   0 debian    (1000) debian    (1000)        1 2024-05-17 20:18:54.000000 kapoorlabs_lightning-5.3.7/src/KapoorLabs_Lightning.egg-info/dependency_links.txt
--rw-r--r--   0 debian    (1000) debian    (1000)      102 2024-05-17 20:18:54.000000 kapoorlabs_lightning-5.3.7/src/KapoorLabs_Lightning.egg-info/requires.txt
--rw-r--r--   0 debian    (1000) debian    (1000)       21 2024-05-17 20:18:54.000000 kapoorlabs_lightning-5.3.7/src/KapoorLabs_Lightning.egg-info/top_level.txt
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-17 20:18:54.343373 kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/
--rw-r--r--   0 debian    (1000) debian    (1000)     1603 2024-05-17 14:55:57.000000 kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/__init__.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-17 20:18:54.343373 kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/_tests/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/_tests/__init__.py
--rw-r--r--   0 debian    (1000) debian    (1000)     3106 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/_tests/test_pytorch_models.py
--rw-r--r--   0 debian    (1000) debian    (1000)       78 2024-05-17 20:17:46.000000 kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/_version.py
--rw-r--r--   0 debian    (1000) debian    (1000)       75 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/caped.yaml
--rw-r--r--   0 debian    (1000) debian    (1000)     2065 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/graph_functions.py
--rw-r--r--   0 debian    (1000) debian    (1000)       68 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/kapoorlabs.yaml
--rw-r--r--   0 debian    (1000) debian    (1000)    65851 2024-05-17 20:17:40.000000 kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/lightning_trainer.py
--rw-r--r--   0 debian    (1000) debian    (1000)    13629 2024-05-13 15:18:01.000000 kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/metrics.py
--rw-r--r--   0 debian    (1000) debian    (1000)     4658 2024-05-13 15:11:51.000000 kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/optimizers.py
--rw-r--r--   0 debian    (1000) debian    (1000)    10230 2024-05-13 17:03:42.000000 kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/pytorch_callbacks.py
--rw-r--r--   0 debian    (1000) debian    (1000)    16235 2024-05-13 15:11:52.000000 kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/pytorch_datasets.py
--rw-r--r--   0 debian    (1000) debian    (1000)     2680 2024-02-23 15:21:15.000000 kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/pytorch_loggers.py
--rw-r--r--   0 debian    (1000) debian    (1000)      762 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/pytorch_losses.py
--rw-r--r--   0 debian    (1000) debian    (1000)    22962 2024-05-13 20:10:57.000000 kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/pytorch_models.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1809 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/pytorch_transforms.py
--rw-r--r--   0 debian    (1000) debian    (1000)     6283 2024-05-13 15:11:52.000000 kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/schedulers.py
--rw-r--r--   0 debian    (1000) debian    (1000)     2497 2024-05-17 18:55:38.000000 kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/utils.py
--rw-r--r--   0 debian    (1000) debian    (1000)      615 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/tox.ini
--rw-r--r--   0 debian    (1000) debian    (1000)      623 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/update_version.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-20 17:23:54.267281 kapoorlabs_lightning-5.3.8/
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-20 17:23:54.255281 kapoorlabs_lightning-5.3.8/.github/
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-20 17:23:54.255281 kapoorlabs_lightning-5.3.8/.github/workflows/
+-rw-r--r--   0 debian    (1000) debian    (1000)     1068 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/.github/workflows/deploy.yml
+-rw-r--r--   0 debian    (1000) debian    (1000)     1963 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 debian    (1000) debian    (1000)      991 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/.gitignore
+-rw-r--r--   0 debian    (1000) debian    (1000)     1008 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/.pre-commit-config.yaml
+-rw-r--r--   0 debian    (1000) debian    (1000)     1487 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/LICENSE
+-rw-r--r--   0 debian    (1000) debian    (1000)       96 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/MANIFEST.in
+-rw-r--r--   0 debian    (1000) debian    (1000)     4108 2024-05-20 17:23:54.267281 kapoorlabs_lightning-5.3.8/PKG-INFO
+-rw-r--r--   0 debian    (1000) debian    (1000)     2435 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/README.md
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-20 17:23:54.259281 kapoorlabs_lightning-5.3.8/licenses/
+-rw-r--r--   0 debian    (1000) debian    (1000)    11358 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/licenses/Apache-2
+-rw-r--r--   0 debian    (1000) debian    (1000)     1487 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/licenses/BSD-3
+-rw-r--r--   0 debian    (1000) debian    (1000)    35148 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/licenses/GPL-3
+-rw-r--r--   0 debian    (1000) debian    (1000)     7653 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/licenses/LGPL-3
+-rw-r--r--   0 debian    (1000) debian    (1000)     1080 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/licenses/MIT
+-rw-r--r--   0 debian    (1000) debian    (1000)    16726 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/licenses/MPL-2
+-rw-r--r--   0 debian    (1000) debian    (1000)      116 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/pyproject.toml
+-rw-r--r--   0 debian    (1000) debian    (1000)     1766 2024-05-20 17:23:54.267281 kapoorlabs_lightning-5.3.8/setup.cfg
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-20 17:23:54.255281 kapoorlabs_lightning-5.3.8/src/
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-20 17:23:54.267281 kapoorlabs_lightning-5.3.8/src/KapoorLabs_Lightning.egg-info/
+-rw-r--r--   0 debian    (1000) debian    (1000)     4108 2024-05-20 17:23:54.000000 kapoorlabs_lightning-5.3.8/src/KapoorLabs_Lightning.egg-info/PKG-INFO
+-rw-r--r--   0 debian    (1000) debian    (1000)     1269 2024-05-20 17:23:54.000000 kapoorlabs_lightning-5.3.8/src/KapoorLabs_Lightning.egg-info/SOURCES.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)        1 2024-05-20 17:23:54.000000 kapoorlabs_lightning-5.3.8/src/KapoorLabs_Lightning.egg-info/dependency_links.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)      102 2024-05-20 17:23:54.000000 kapoorlabs_lightning-5.3.8/src/KapoorLabs_Lightning.egg-info/requires.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)       21 2024-05-20 17:23:54.000000 kapoorlabs_lightning-5.3.8/src/KapoorLabs_Lightning.egg-info/top_level.txt
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-20 17:23:54.267281 kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/
+-rw-r--r--   0 debian    (1000) debian    (1000)     1603 2024-05-17 14:55:57.000000 kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/__init__.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-20 17:23:54.267281 kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/_tests/
+-rw-r--r--   0 debian    (1000) debian    (1000)        0 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/_tests/__init__.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     3106 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/_tests/test_pytorch_models.py
+-rw-r--r--   0 debian    (1000) debian    (1000)       78 2024-05-20 17:22:56.000000 kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/_version.py
+-rw-r--r--   0 debian    (1000) debian    (1000)       75 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/caped.yaml
+-rw-r--r--   0 debian    (1000) debian    (1000)     2065 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/graph_functions.py
+-rw-r--r--   0 debian    (1000) debian    (1000)       68 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/kapoorlabs.yaml
+-rw-r--r--   0 debian    (1000) debian    (1000)    65805 2024-05-18 20:51:03.000000 kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/lightning_trainer.py
+-rw-r--r--   0 debian    (1000) debian    (1000)    13532 2024-05-20 17:22:52.000000 kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/metrics.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     4658 2024-05-13 15:11:51.000000 kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/optimizers.py
+-rw-r--r--   0 debian    (1000) debian    (1000)    10230 2024-05-13 17:03:42.000000 kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/pytorch_callbacks.py
+-rw-r--r--   0 debian    (1000) debian    (1000)    16120 2024-05-20 11:14:56.000000 kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/pytorch_datasets.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     2680 2024-02-23 15:21:15.000000 kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/pytorch_loggers.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      762 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/pytorch_losses.py
+-rw-r--r--   0 debian    (1000) debian    (1000)    23059 2024-05-18 20:48:11.000000 kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/pytorch_models.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     1809 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/pytorch_transforms.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     6283 2024-05-13 15:11:52.000000 kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/schedulers.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     2504 2024-05-17 21:13:17.000000 kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/utils.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      615 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/tox.ini
+-rw-r--r--   0 debian    (1000) debian    (1000)      623 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/update_version.py
```

### Comparing `kapoorlabs_lightning-5.3.7/.github/workflows/deploy.yml` & `kapoorlabs_lightning-5.3.8/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.7/.github/workflows/test_and_deploy.yml` & `kapoorlabs_lightning-5.3.8/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.7/.gitignore` & `kapoorlabs_lightning-5.3.8/.gitignore`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.7/.pre-commit-config.yaml` & `kapoorlabs_lightning-5.3.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.7/LICENSE` & `kapoorlabs_lightning-5.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.7/PKG-INFO` & `kapoorlabs_lightning-5.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KapoorLabs-Lightning
-Version: 5.3.7
+Version: 5.3.8
 Summary: Lightning modules for KapoorLabs specific projects
 Home-page: https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning
 Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning#README.md
```

### Comparing `kapoorlabs_lightning-5.3.7/README.md` & `kapoorlabs_lightning-5.3.8/README.md`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.7/licenses/Apache-2` & `kapoorlabs_lightning-5.3.8/licenses/Apache-2`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.7/licenses/BSD-3` & `kapoorlabs_lightning-5.3.8/licenses/BSD-3`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.7/licenses/GPL-3` & `kapoorlabs_lightning-5.3.8/licenses/GPL-3`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.7/licenses/LGPL-3` & `kapoorlabs_lightning-5.3.8/licenses/LGPL-3`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.7/licenses/MIT` & `kapoorlabs_lightning-5.3.8/licenses/MIT`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.7/licenses/MPL-2` & `kapoorlabs_lightning-5.3.8/licenses/MPL-2`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.7/setup.cfg` & `kapoorlabs_lightning-5.3.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.7/src/KapoorLabs_Lightning.egg-info/PKG-INFO` & `kapoorlabs_lightning-5.3.8/src/KapoorLabs_Lightning.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KapoorLabs-Lightning
-Version: 5.3.7
+Version: 5.3.8
 Summary: Lightning modules for KapoorLabs specific projects
 Home-page: https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning
 Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning#README.md
```

### Comparing `kapoorlabs_lightning-5.3.7/src/KapoorLabs_Lightning.egg-info/SOURCES.txt` & `kapoorlabs_lightning-5.3.8/src/KapoorLabs_Lightning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/__init__.py` & `kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/__init__.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/_tests/test_pytorch_models.py` & `kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/_tests/test_pytorch_models.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/graph_functions.py` & `kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/graph_functions.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/lightning_trainer.py` & `kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/lightning_trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         self,
         npz_file: str,
         num_classes,
         growth_rate: int = 32,
         block_config: tuple = (6, 12, 24, 16),
         num_init_features: int = 32,
         bottleneck_size: int = 4,
-        kernel_size: int = 3,
+        kernel_size: int = 7,
         num_workers: int = 1,
         epochs: int = 1,
         log_path="log_path",
         batch_size: int = 1,
         accelerator="cuda",
         devices=1,
         loss_function: str = "cross_entropy",
@@ -211,15 +211,15 @@
 
     def setup_checkpoint(self):
         self.ckpt_path = load_checkpoint_model(self.log_path)
         self.modelcheckpoint = CheckpointModel(save_dir=self.log_path)
 
     def setup_adam(self):
         self.optimizer = Adam(
-            lr=self.learning_rate, weight_decay=self.weight_decay, eps=self.eps
+            lr=self.learning_rate
         )
 
     def setup_rmsprop(self):
         self.optimizer = RMSprop(
             lr=self.learning_rate,
             momentum=self.momentum,
             weight_decay=self.decay,
```

### Comparing `kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/metrics.py` & `kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 from natsort import natsorted
 import seaborn as sns
 
 
 def extract_metrics_from_model(lightning_model, after_final_validation=True):
 
     if after_final_validation:
-        extra_validation_runs = (
-            1  # to account for the last additional validation run done by the trainer
-        )
+        extra_validation_runs = 1
         val_losses = lightning_model.val_losses[:-extra_validation_runs]
         val_accuracies = lightning_model.val_accuracies[:-extra_validation_runs]
         extra_val_loss = lightning_model.val_losses[-1]  # extra run
         extra_val_accuracy = lightning_model.val_accuracies[-1]  # extra run
     else:
         extra_validation_runs = 0
         val_losses = lightning_model.val_losses
```

### Comparing `kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/optimizers.py` & `kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/optimizers.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/pytorch_callbacks.py` & `kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/pytorch_callbacks.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/pytorch_datasets.py` & `kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/pytorch_datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,23 +133,22 @@
 
 
 class MitosisDataset(Dataset):
     def __init__(self, arrays, labels):
         self.arrays = arrays
         self.labels = labels
         self.input_channels = arrays.shape[2]
-        self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
     def __len__(self):
         return len(self.arrays)
 
     def __getitem__(self, idx):
         array = self.arrays[idx]
-        array = torch.tensor(array).permute(1, 0).float().to(self.device)
-        label = torch.tensor(self.labels[idx]).to(self.device)
+        array = torch.tensor(array).permute(1, 0).float()
+        label = torch.tensor(self.labels[idx])
         return array, label
 
 
 class GefGapDataset(Dataset):
     def __init__(
         self,
         annotations_file,
```

### Comparing `kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/pytorch_loggers.py` & `kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/pytorch_loggers.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/pytorch_losses.py` & `kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/pytorch_losses.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/pytorch_models.py` & `kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/pytorch_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,23 +13,23 @@
     """ """
 
     def __init__(self, input_channels, growth_rate, bottleneck_size, kernel_size):
         super().__init__()
         self.use_bottleneck = bottleneck_size > 0
         self.num_bottleneck_output_filters = growth_rate * bottleneck_size
         if self.use_bottleneck:
-            self.bn2 = nn.GroupNorm(1, input_channels)
+            self.bn2 = nn.BatchNorm1d(input_channels)
             self.act2 = nn.ReLU(inplace=True)
             self.conv2 = nn.Conv1d(
                 input_channels,
                 self.num_bottleneck_output_filters,
                 kernel_size=1,
                 stride=1,
             )
-        self.bn1 = nn.GroupNorm(1, self.num_bottleneck_output_filters)
+        self.bn1 = nn.BatchNorm1d(self.num_bottleneck_output_filters)
         self.act1 = nn.ReLU(inplace=True)
         self.conv1 = nn.Conv1d(
             self.num_bottleneck_output_filters,
             growth_rate,
             kernel_size=kernel_size,
             stride=1,
             dilation=1,
@@ -76,15 +76,15 @@
 
 
 class TransitionBlock(nn.Module):
     """ """
 
     def __init__(self, input_channels, out_channels):
         super().__init__()
-        self.bn = nn.GroupNorm(1, input_channels)
+        self.bn = nn.BatchNorm1d(input_channels)
         self.act = nn.ReLU(inplace=True)
         self.conv = nn.Conv1d(
             input_channels, out_channels, kernel_size=1, stride=1, dilation=1
         )
         self.pool = nn.AvgPool1d(kernel_size=2, stride=2)
 
     def forward(self, x):
@@ -105,21 +105,24 @@
         num_init_features: int = 32,
         bottleneck_size: int = 4,
         kernel_size: int = 3,
     ):
 
         super().__init__()
         self._initialize_weights()
-
+        
         self.features = nn.Sequential(
-            nn.Conv1d(input_channels, num_init_features, kernel_size=1),
-            nn.GroupNorm(1, num_init_features),
+            nn.Conv1d(
+                input_channels, num_init_features, 
+                kernel_size=7, stride=2, padding=3, dilation=1),
+            nn.BatchNorm1d(num_init_features),
             nn.ReLU(inplace=True),
-            nn.MaxPool1d(kernel_size=1),
+            nn.MaxPool1d(kernel_size=3, stride=2, padding=1),
         )
+     
 
         num_features = num_init_features
         for i, num_layers in enumerate(block_config):
             block = DenseBlock(
                 num_layers=num_layers,
                 input_channels=num_features,
                 growth_rate=growth_rate,
@@ -131,15 +134,15 @@
             if i != len(block_config) - 1:
                 trans = TransitionBlock(
                     input_channels=num_features, out_channels=num_features // 2
                 )
                 self.features.add_module(f"transition{i}", trans)
                 num_features = num_features // 2
 
-        self.final_bn = nn.GroupNorm(1, num_features)
+        self.final_bn = nn.BatchNorm1d(num_features)
         self.final_act = nn.ReLU(inplace=True)
         self.final_pool = nn.AdaptiveAvgPool1d(1)
         self.classifier_1 = nn.Linear(num_features, num_classes)
 
     def _initialize_weights(self):
         for m in self.modules():
             if isinstance(m, nn.Conv1d):
```

### Comparing `kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/pytorch_transforms.py` & `kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/pytorch_transforms.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/schedulers.py` & `kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/schedulers.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/utils.py` & `kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             data = np.load(str(filepath), allow_pickle=True)
         except pickle.UnpicklingError:
             # print(f"Error loading data from {filepath}. Skipping this file.")
             continue
 
         keys = data.files
         keys = sorted(keys, key=lambda x: ("epoch" in x, x), reverse=True)
-        unwanted_substrings = ["gpu", "memory"]
+        unwanted_substrings = ["step","gpu", "memory"]
         for idx, key in enumerate(keys):
             if not any(substring in key for substring in unwanted_substrings):
                 data_values = data[key].tolist()
                 if key not in all_data:
                     all_data[key] = data_values
                 else:
                     all_data[key]["steps"].extend(data_values["steps"])
```

### Comparing `kapoorlabs_lightning-5.3.7/tox.ini` & `kapoorlabs_lightning-5.3.8/tox.ini`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.7/update_version.py` & `kapoorlabs_lightning-5.3.8/update_version.py`

 * *Files identical despite different names*

