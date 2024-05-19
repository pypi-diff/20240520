# Comparing `tmp/notebooks_and_scripts-4.447.1.tar.gz` & `tmp/notebooks_and_scripts-4.448.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notebooks_and_scripts-4.447.1.tar", last modified: Sun May 19 22:58:02 2024, max compression
+gzip compressed data, was "notebooks_and_scripts-4.448.1.tar", last modified: Sun May 19 23:00:27 2024, max compression
```

## Comparing `notebooks_and_scripts-4.447.1.tar` & `notebooks_and_scripts-4.448.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 22:58:02.475972 notebooks_and_scripts-4.447.1/
--rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-09-26 02:32:46.000000 notebooks_and_scripts-4.447.1/LICENSE
--rw-r--r--   0 kamangir   (502) staff       (20)     5052 2024-05-19 22:58:02.475281 notebooks_and_scripts-4.447.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     4193 2024-05-08 05:19:48.000000 notebooks_and_scripts-4.447.1/README.md
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 22:58:02.470486 notebooks_and_scripts-4.447.1/notebooks_and_scripts/
--rw-r--r--   0 kamangir   (502) staff       (20)      153 2024-05-19 22:57:57.000000 notebooks_and_scripts-4.447.1/notebooks_and_scripts/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      898 2024-04-27 03:49:23.000000 notebooks_and_scripts-4.447.1/notebooks_and_scripts/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      279 2024-05-08 01:33:41.000000 notebooks_and_scripts-4.447.1/notebooks_and_scripts/config.env
--rw-r--r--   0 kamangir   (502) staff       (20)      443 2024-05-08 01:33:52.000000 notebooks_and_scripts-4.447.1/notebooks_and_scripts/env.py
--rw-r--r--   0 kamangir   (502) staff       (20)      102 2024-03-24 00:15:57.000000 notebooks_and_scripts-4.447.1/notebooks_and_scripts/logger.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 22:58:02.473923 notebooks_and_scripts-4.447.1/notebooks_and_scripts/sagemaker/
--rw-r--r--   0 kamangir   (502) staff       (20)      365 2024-03-04 07:47:37.000000 notebooks_and_scripts-4.447.1/notebooks_and_scripts/sagemaker/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-09-26 02:32:46.000000 notebooks_and_scripts-4.447.1/notebooks_and_scripts/urls.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 22:58:02.474555 notebooks_and_scripts-4.447.1/notebooks_and_scripts.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)     5052 2024-05-19 22:58:02.000000 notebooks_and_scripts-4.447.1/notebooks_and_scripts.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      442 2024-05-19 22:58:02.000000 notebooks_and_scripts-4.447.1/notebooks_and_scripts.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-19 22:58:02.000000 notebooks_and_scripts-4.447.1/notebooks_and_scripts.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       22 2024-05-19 22:58:02.000000 notebooks_and_scripts-4.447.1/notebooks_and_scripts.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-19 22:58:02.476165 notebooks_and_scripts-4.447.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      624 2024-05-19 22:57:54.000000 notebooks_and_scripts-4.447.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 23:00:27.451527 notebooks_and_scripts-4.448.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-09-26 02:32:46.000000 notebooks_and_scripts-4.448.1/LICENSE
+-rw-r--r--   0 kamangir   (502) staff       (20)     4943 2024-05-19 23:00:27.450955 notebooks_and_scripts-4.448.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     4141 2024-05-19 23:00:17.000000 notebooks_and_scripts-4.448.1/README.md
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 23:00:27.447555 notebooks_and_scripts-4.448.1/notebooks_and_scripts/
+-rw-r--r--   0 kamangir   (502) staff       (20)      153 2024-05-19 23:00:22.000000 notebooks_and_scripts-4.448.1/notebooks_and_scripts/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      898 2024-04-27 03:49:23.000000 notebooks_and_scripts-4.448.1/notebooks_and_scripts/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      279 2024-05-08 01:33:41.000000 notebooks_and_scripts-4.448.1/notebooks_and_scripts/config.env
+-rw-r--r--   0 kamangir   (502) staff       (20)      443 2024-05-08 01:33:52.000000 notebooks_and_scripts-4.448.1/notebooks_and_scripts/env.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      102 2024-03-24 00:15:57.000000 notebooks_and_scripts-4.448.1/notebooks_and_scripts/logger.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 23:00:27.449781 notebooks_and_scripts-4.448.1/notebooks_and_scripts/sagemaker/
+-rw-r--r--   0 kamangir   (502) staff       (20)      365 2024-03-04 07:47:37.000000 notebooks_and_scripts-4.448.1/notebooks_and_scripts/sagemaker/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-09-26 02:32:46.000000 notebooks_and_scripts-4.448.1/notebooks_and_scripts/urls.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 23:00:27.450333 notebooks_and_scripts-4.448.1/notebooks_and_scripts.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     4943 2024-05-19 23:00:27.000000 notebooks_and_scripts-4.448.1/notebooks_and_scripts.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      442 2024-05-19 23:00:27.000000 notebooks_and_scripts-4.448.1/notebooks_and_scripts.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-19 23:00:27.000000 notebooks_and_scripts-4.448.1/notebooks_and_scripts.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       22 2024-05-19 23:00:27.000000 notebooks_and_scripts-4.448.1/notebooks_and_scripts.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-19 23:00:27.451648 notebooks_and_scripts-4.448.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      624 2024-05-19 22:57:54.000000 notebooks_and_scripts-4.448.1/setup.py
```

### Comparing `notebooks_and_scripts-4.447.1/LICENSE` & `notebooks_and_scripts-4.448.1/LICENSE`

 * *Files identical despite different names*

### Comparing `notebooks_and_scripts-4.447.1/PKG-INFO` & `notebooks_and_scripts-4.448.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: notebooks_and_scripts
-Version: 4.447.1
+Version: 4.448.1
 Summary: 📜 notebooks and scripts for ai experiments and aws batch jobs.
 Author: arash@kamangir.net
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 📜 notebooks & [meta] scripts
 
-Repository of research [notebooks](https://github.com/kamangir/notebooks-and-scripts/raw/main/notebooks) and [[meta](https://github.com/kamangir/notebooks-and-scripts/raw/main/scripts#meta/)] [scripts](https://github.com/kamangir/notebooks-and-scripts/raw/main/scripts) for aws batch jobs and sagemaker serving.
+[notebooks](https://github.com/kamangir/notebooks-and-scripts/raw/main/notebooks) and [scripts](https://github.com/kamangir/notebooks-and-scripts/raw/main/scripts) for ai experiments and aws batch jobs.
 
 ---
 
 | ![image](https://github.com/kamangir/assets/blob/main/nbs/3x4.jpg?raw=true)                               | ![image](https://github.com/kamangir/assets/blob/main/nbs/mission-patch-00008.png?raw=true) | ![image](https://github.com/kamangir/assets/blob/main/nbs/train-summary.png?raw=true) ![image](https://github.com/kamangir/assets/blob/main/nbs/predict-00000.png?raw=true) |
 | --------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | [paint-a-sentence](https://github.com/kamangir/notebooks-and-scripts/raw/main/scripts/paint-a-sentence.sh)                                                         | [mission-patch](https://github.com/kamangir/notebooks-and-scripts/raw/main/scripts/mission-patch.sh)                                                 | [roofAI-train](https://github.com/kamangir/notebooks-and-scripts/raw/main/scripts/roofAI-train.sh)                                                                                                                                   |
 | https://medium.com/@arash-kamangir/a-cat-walking-under-apple-trees-style-by-stable-diffusion-ab60ece43e2a | https://medium.com/@arash-kamangir/private-mission-patch-%EF%B8%8F-1-0c2eddd79762           | https://arash-kamangir.medium.com/roofai-%EF%B8%8F-on-gpu-6-b02f8f67ed3f                                                                                                    |
```

### Comparing `notebooks_and_scripts-4.447.1/README.md` & `notebooks_and_scripts-4.448.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # 📜 notebooks & [meta] scripts
 
-Repository of research [notebooks](./notebooks) and [[meta](./scripts#meta/)] [scripts](./scripts) for aws batch jobs and sagemaker serving.
+[notebooks](./notebooks) and [scripts](./scripts) for ai experiments and aws batch jobs.
 
 ---
 
 | ![image](https://github.com/kamangir/assets/blob/main/nbs/3x4.jpg?raw=true)                               | ![image](https://github.com/kamangir/assets/blob/main/nbs/mission-patch-00008.png?raw=true) | ![image](https://github.com/kamangir/assets/blob/main/nbs/train-summary.png?raw=true) ![image](https://github.com/kamangir/assets/blob/main/nbs/predict-00000.png?raw=true) |
 | --------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | [paint-a-sentence](./scripts/paint-a-sentence.sh)                                                         | [mission-patch](./scripts/mission-patch.sh)                                                 | [roofAI-train](./scripts/roofAI-train.sh)                                                                                                                                   |
 | https://medium.com/@arash-kamangir/a-cat-walking-under-apple-trees-style-by-stable-diffusion-ab60ece43e2a | https://medium.com/@arash-kamangir/private-mission-patch-%EF%B8%8F-1-0c2eddd79762           | https://arash-kamangir.medium.com/roofai-%EF%B8%8F-on-gpu-6-b02f8f67ed3f                                                                                                    |
```

### Comparing `notebooks_and_scripts-4.447.1/notebooks_and_scripts/__main__.py` & `notebooks_and_scripts-4.448.1/notebooks_and_scripts/__main__.py`

 * *Files identical despite different names*

### Comparing `notebooks_and_scripts-4.447.1/notebooks_and_scripts.egg-info/PKG-INFO` & `notebooks_and_scripts-4.448.1/notebooks_and_scripts.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: notebooks_and_scripts
-Version: 4.447.1
+Version: 4.448.1
 Summary: 📜 notebooks and scripts for ai experiments and aws batch jobs.
 Author: arash@kamangir.net
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 📜 notebooks & [meta] scripts
 
-Repository of research [notebooks](https://github.com/kamangir/notebooks-and-scripts/raw/main/notebooks) and [[meta](https://github.com/kamangir/notebooks-and-scripts/raw/main/scripts#meta/)] [scripts](https://github.com/kamangir/notebooks-and-scripts/raw/main/scripts) for aws batch jobs and sagemaker serving.
+[notebooks](https://github.com/kamangir/notebooks-and-scripts/raw/main/notebooks) and [scripts](https://github.com/kamangir/notebooks-and-scripts/raw/main/scripts) for ai experiments and aws batch jobs.
 
 ---
 
 | ![image](https://github.com/kamangir/assets/blob/main/nbs/3x4.jpg?raw=true)                               | ![image](https://github.com/kamangir/assets/blob/main/nbs/mission-patch-00008.png?raw=true) | ![image](https://github.com/kamangir/assets/blob/main/nbs/train-summary.png?raw=true) ![image](https://github.com/kamangir/assets/blob/main/nbs/predict-00000.png?raw=true) |
 | --------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | [paint-a-sentence](https://github.com/kamangir/notebooks-and-scripts/raw/main/scripts/paint-a-sentence.sh)                                                         | [mission-patch](https://github.com/kamangir/notebooks-and-scripts/raw/main/scripts/mission-patch.sh)                                                 | [roofAI-train](https://github.com/kamangir/notebooks-and-scripts/raw/main/scripts/roofAI-train.sh)                                                                                                                                   |
 | https://medium.com/@arash-kamangir/a-cat-walking-under-apple-trees-style-by-stable-diffusion-ab60ece43e2a | https://medium.com/@arash-kamangir/private-mission-patch-%EF%B8%8F-1-0c2eddd79762           | https://arash-kamangir.medium.com/roofai-%EF%B8%8F-on-gpu-6-b02f8f67ed3f                                                                                                    |
```

### Comparing `notebooks_and_scripts-4.447.1/setup.py` & `notebooks_and_scripts-4.448.1/setup.py`

 * *Files identical despite different names*

