# Comparing `tmp/notebooks_and_scripts-4.446.1.tar.gz` & `tmp/notebooks_and_scripts-4.447.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notebooks_and_scripts-4.446.1.tar", last modified: Sun May 19 22:56:39 2024, max compression
+gzip compressed data, was "notebooks_and_scripts-4.447.1.tar", last modified: Sun May 19 22:58:02 2024, max compression
```

## Comparing `notebooks_and_scripts-4.446.1.tar` & `notebooks_and_scripts-4.447.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 22:56:39.556861 notebooks_and_scripts-4.446.1/
--rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-09-26 02:32:46.000000 notebooks_and_scripts-4.446.1/LICENSE
--rw-r--r--   0 kamangir   (502) staff       (20)     5085 2024-05-19 22:56:39.556091 notebooks_and_scripts-4.446.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     4193 2024-05-08 05:19:48.000000 notebooks_and_scripts-4.446.1/README.md
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 22:56:39.552750 notebooks_and_scripts-4.446.1/notebooks_and_scripts/
--rw-r--r--   0 kamangir   (502) staff       (20)      153 2024-05-19 22:56:35.000000 notebooks_and_scripts-4.446.1/notebooks_and_scripts/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      898 2024-04-27 03:49:23.000000 notebooks_and_scripts-4.446.1/notebooks_and_scripts/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      279 2024-05-08 01:33:41.000000 notebooks_and_scripts-4.446.1/notebooks_and_scripts/config.env
--rw-r--r--   0 kamangir   (502) staff       (20)      443 2024-05-08 01:33:52.000000 notebooks_and_scripts-4.446.1/notebooks_and_scripts/env.py
--rw-r--r--   0 kamangir   (502) staff       (20)      102 2024-03-24 00:15:57.000000 notebooks_and_scripts-4.446.1/notebooks_and_scripts/logger.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 22:56:39.554799 notebooks_and_scripts-4.446.1/notebooks_and_scripts/sagemaker/
--rw-r--r--   0 kamangir   (502) staff       (20)      365 2024-03-04 07:47:37.000000 notebooks_and_scripts-4.446.1/notebooks_and_scripts/sagemaker/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-09-26 02:32:46.000000 notebooks_and_scripts-4.446.1/notebooks_and_scripts/urls.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 22:56:39.555468 notebooks_and_scripts-4.446.1/notebooks_and_scripts.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)     5085 2024-05-19 22:56:39.000000 notebooks_and_scripts-4.446.1/notebooks_and_scripts.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      442 2024-05-19 22:56:39.000000 notebooks_and_scripts-4.446.1/notebooks_and_scripts.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-19 22:56:39.000000 notebooks_and_scripts-4.446.1/notebooks_and_scripts.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       22 2024-05-19 22:56:39.000000 notebooks_and_scripts-4.446.1/notebooks_and_scripts.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-19 22:56:39.557377 notebooks_and_scripts-4.446.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      627 2024-05-19 22:56:26.000000 notebooks_and_scripts-4.446.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 22:58:02.475972 notebooks_and_scripts-4.447.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-09-26 02:32:46.000000 notebooks_and_scripts-4.447.1/LICENSE
+-rw-r--r--   0 kamangir   (502) staff       (20)     5052 2024-05-19 22:58:02.475281 notebooks_and_scripts-4.447.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     4193 2024-05-08 05:19:48.000000 notebooks_and_scripts-4.447.1/README.md
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 22:58:02.470486 notebooks_and_scripts-4.447.1/notebooks_and_scripts/
+-rw-r--r--   0 kamangir   (502) staff       (20)      153 2024-05-19 22:57:57.000000 notebooks_and_scripts-4.447.1/notebooks_and_scripts/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      898 2024-04-27 03:49:23.000000 notebooks_and_scripts-4.447.1/notebooks_and_scripts/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      279 2024-05-08 01:33:41.000000 notebooks_and_scripts-4.447.1/notebooks_and_scripts/config.env
+-rw-r--r--   0 kamangir   (502) staff       (20)      443 2024-05-08 01:33:52.000000 notebooks_and_scripts-4.447.1/notebooks_and_scripts/env.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      102 2024-03-24 00:15:57.000000 notebooks_and_scripts-4.447.1/notebooks_and_scripts/logger.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 22:58:02.473923 notebooks_and_scripts-4.447.1/notebooks_and_scripts/sagemaker/
+-rw-r--r--   0 kamangir   (502) staff       (20)      365 2024-03-04 07:47:37.000000 notebooks_and_scripts-4.447.1/notebooks_and_scripts/sagemaker/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-09-26 02:32:46.000000 notebooks_and_scripts-4.447.1/notebooks_and_scripts/urls.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 22:58:02.474555 notebooks_and_scripts-4.447.1/notebooks_and_scripts.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     5052 2024-05-19 22:58:02.000000 notebooks_and_scripts-4.447.1/notebooks_and_scripts.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      442 2024-05-19 22:58:02.000000 notebooks_and_scripts-4.447.1/notebooks_and_scripts.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-19 22:58:02.000000 notebooks_and_scripts-4.447.1/notebooks_and_scripts.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       22 2024-05-19 22:58:02.000000 notebooks_and_scripts-4.447.1/notebooks_and_scripts.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-19 22:58:02.476165 notebooks_and_scripts-4.447.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      624 2024-05-19 22:57:54.000000 notebooks_and_scripts-4.447.1/setup.py
```

### Comparing `notebooks_and_scripts-4.446.1/LICENSE` & `notebooks_and_scripts-4.447.1/LICENSE`

 * *Files identical despite different names*

### Comparing `notebooks_and_scripts-4.446.1/PKG-INFO` & `notebooks_and_scripts-4.447.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: notebooks_and_scripts
-Version: 4.446.1
+Version: 4.447.1
 Summary: 📜 notebooks and scripts for ai experiments and aws batch jobs.
 Author: arash@kamangir.net
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 📜 notebooks & [meta] scripts
 
-Repository of research [notebooks](https://github.com/kamangir/notebooks-and-scripts/raw/current/notebooks) and [[meta](https://github.com/kamangir/notebooks-and-scripts/raw/current/scripts#meta/)] [scripts](https://github.com/kamangir/notebooks-and-scripts/raw/current/scripts) for aws batch jobs and sagemaker serving.
+Repository of research [notebooks](https://github.com/kamangir/notebooks-and-scripts/raw/main/notebooks) and [[meta](https://github.com/kamangir/notebooks-and-scripts/raw/main/scripts#meta/)] [scripts](https://github.com/kamangir/notebooks-and-scripts/raw/main/scripts) for aws batch jobs and sagemaker serving.
 
 ---
 
 | ![image](https://github.com/kamangir/assets/blob/main/nbs/3x4.jpg?raw=true)                               | ![image](https://github.com/kamangir/assets/blob/main/nbs/mission-patch-00008.png?raw=true) | ![image](https://github.com/kamangir/assets/blob/main/nbs/train-summary.png?raw=true) ![image](https://github.com/kamangir/assets/blob/main/nbs/predict-00000.png?raw=true) |
 | --------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| [paint-a-sentence](https://github.com/kamangir/notebooks-and-scripts/raw/current/scripts/paint-a-sentence.sh)                                                         | [mission-patch](https://github.com/kamangir/notebooks-and-scripts/raw/current/scripts/mission-patch.sh)                                                 | [roofAI-train](https://github.com/kamangir/notebooks-and-scripts/raw/current/scripts/roofAI-train.sh)                                                                                                                                   |
+| [paint-a-sentence](https://github.com/kamangir/notebooks-and-scripts/raw/main/scripts/paint-a-sentence.sh)                                                         | [mission-patch](https://github.com/kamangir/notebooks-and-scripts/raw/main/scripts/mission-patch.sh)                                                 | [roofAI-train](https://github.com/kamangir/notebooks-and-scripts/raw/main/scripts/roofAI-train.sh)                                                                                                                                   |
 | https://medium.com/@arash-kamangir/a-cat-walking-under-apple-trees-style-by-stable-diffusion-ab60ece43e2a | https://medium.com/@arash-kamangir/private-mission-patch-%EF%B8%8F-1-0c2eddd79762           | https://arash-kamangir.medium.com/roofai-%EF%B8%8F-on-gpu-6-b02f8f67ed3f                                                                                                    |
 
-also: [`sagesemseg`](https://github.com/kamangir/notebooks-and-scripts/raw/current/scripts/sagesemseg/).
+also: [`sagesemseg`](https://github.com/kamangir/notebooks-and-scripts/raw/main/scripts/sagesemseg/).
 
 ---
 
-also home to [`workflow`](https://github.com/kamangir/notebooks-and-scripts/raw/current/notebooks_and_scripts/workflow/generic.py), an abstraction to run mixed-type (cpu/gpu/...) [DAG](https://networkx.org/documentation/stable/reference/classes/digraph.html)s of bash commands on aws batch.
+also home to [`workflow`](https://github.com/kamangir/notebooks-and-scripts/raw/main/notebooks_and_scripts/workflow/generic.py), an abstraction to run mixed-type (cpu/gpu/...) [DAG](https://networkx.org/documentation/stable/reference/classes/digraph.html)s of bash commands on aws batch.
 
 ```bash
  > workflow help
 workflow create \
 	pattern=a-bc-d|hourglass,~upload \
 	-|<job-name> \
 	<command-line>
@@ -45,14 +45,14 @@
 workflow create pattern=hourglass .
 workflow submit to=aws_batch
 @watch - @download
 ```
 
 from https://arash-kamangir.medium.com/%EF%B8%8F-openai-experiments-54-e49117dc69ef
 
-| [`a-bc-d`](https://github.com/kamangir/notebooks-and-scripts/raw/current/notebooks_and_scripts/workflow/patterns/a-bc-d.dot) [🔗](https://kamangir-public.s3.ca-central-1.amazonaws.com/a-bc-d/workflow.gif?raw=true) | [`hourglass`](https://github.com/kamangir/notebooks-and-scripts/raw/current/notebooks_and_scripts/workflow/patterns/hourglass.dot) [🔗](https://kamangir-public.s3.ca-central-1.amazonaws.com/hourglass/workflow.gif?raw=true) | [`map-reduce`](https://github.com/kamangir/notebooks-and-scripts/raw/current/notebooks_and_scripts/workflow/patterns/map-reduce.dot) [🔗](https://kamangir-public.s3.ca-central-1.amazonaws.com/map-reduce/workflow.gif?raw=true) |
+| [`a-bc-d`](https://github.com/kamangir/notebooks-and-scripts/raw/main/notebooks_and_scripts/workflow/patterns/a-bc-d.dot) [🔗](https://kamangir-public.s3.ca-central-1.amazonaws.com/a-bc-d/workflow.gif?raw=true) | [`hourglass`](https://github.com/kamangir/notebooks-and-scripts/raw/main/notebooks_and_scripts/workflow/patterns/hourglass.dot) [🔗](https://kamangir-public.s3.ca-central-1.amazonaws.com/hourglass/workflow.gif?raw=true) | [`map-reduce`](https://github.com/kamangir/notebooks-and-scripts/raw/main/notebooks_and_scripts/workflow/patterns/map-reduce.dot) [🔗](https://kamangir-public.s3.ca-central-1.amazonaws.com/map-reduce/workflow.gif?raw=true) |
 | --------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | ![image](https://kamangir-public.s3.ca-central-1.amazonaws.com/a-bc-d/workflow.gif?raw=true)                                                              | ![image](https://kamangir-public.s3.ca-central-1.amazonaws.com/hourglass/workflow.gif?raw=true)                                                                    | ![image](https://kamangir-public.s3.ca-central-1.amazonaws.com/map-reduce/workflow.gif?raw=true)                                                                      |
 
 ---
 
 To use on [AWS SageMaker](https://aws.amazon.com/sagemaker/) replace `<plugin-name>` with `nbs` and follow [these instructions](https://github.com/kamangir/blue-plugin/blob/main/SageMaker.md).
```

### Comparing `notebooks_and_scripts-4.446.1/README.md` & `notebooks_and_scripts-4.447.1/README.md`

 * *Files identical despite different names*

### Comparing `notebooks_and_scripts-4.446.1/notebooks_and_scripts/__main__.py` & `notebooks_and_scripts-4.447.1/notebooks_and_scripts/__main__.py`

 * *Files identical despite different names*

### Comparing `notebooks_and_scripts-4.446.1/notebooks_and_scripts.egg-info/PKG-INFO` & `notebooks_and_scripts-4.447.1/notebooks_and_scripts.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: notebooks_and_scripts
-Version: 4.446.1
+Version: 4.447.1
 Summary: 📜 notebooks and scripts for ai experiments and aws batch jobs.
 Author: arash@kamangir.net
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 📜 notebooks & [meta] scripts
 
-Repository of research [notebooks](https://github.com/kamangir/notebooks-and-scripts/raw/current/notebooks) and [[meta](https://github.com/kamangir/notebooks-and-scripts/raw/current/scripts#meta/)] [scripts](https://github.com/kamangir/notebooks-and-scripts/raw/current/scripts) for aws batch jobs and sagemaker serving.
+Repository of research [notebooks](https://github.com/kamangir/notebooks-and-scripts/raw/main/notebooks) and [[meta](https://github.com/kamangir/notebooks-and-scripts/raw/main/scripts#meta/)] [scripts](https://github.com/kamangir/notebooks-and-scripts/raw/main/scripts) for aws batch jobs and sagemaker serving.
 
 ---
 
 | ![image](https://github.com/kamangir/assets/blob/main/nbs/3x4.jpg?raw=true)                               | ![image](https://github.com/kamangir/assets/blob/main/nbs/mission-patch-00008.png?raw=true) | ![image](https://github.com/kamangir/assets/blob/main/nbs/train-summary.png?raw=true) ![image](https://github.com/kamangir/assets/blob/main/nbs/predict-00000.png?raw=true) |
 | --------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| [paint-a-sentence](https://github.com/kamangir/notebooks-and-scripts/raw/current/scripts/paint-a-sentence.sh)                                                         | [mission-patch](https://github.com/kamangir/notebooks-and-scripts/raw/current/scripts/mission-patch.sh)                                                 | [roofAI-train](https://github.com/kamangir/notebooks-and-scripts/raw/current/scripts/roofAI-train.sh)                                                                                                                                   |
+| [paint-a-sentence](https://github.com/kamangir/notebooks-and-scripts/raw/main/scripts/paint-a-sentence.sh)                                                         | [mission-patch](https://github.com/kamangir/notebooks-and-scripts/raw/main/scripts/mission-patch.sh)                                                 | [roofAI-train](https://github.com/kamangir/notebooks-and-scripts/raw/main/scripts/roofAI-train.sh)                                                                                                                                   |
 | https://medium.com/@arash-kamangir/a-cat-walking-under-apple-trees-style-by-stable-diffusion-ab60ece43e2a | https://medium.com/@arash-kamangir/private-mission-patch-%EF%B8%8F-1-0c2eddd79762           | https://arash-kamangir.medium.com/roofai-%EF%B8%8F-on-gpu-6-b02f8f67ed3f                                                                                                    |
 
-also: [`sagesemseg`](https://github.com/kamangir/notebooks-and-scripts/raw/current/scripts/sagesemseg/).
+also: [`sagesemseg`](https://github.com/kamangir/notebooks-and-scripts/raw/main/scripts/sagesemseg/).
 
 ---
 
-also home to [`workflow`](https://github.com/kamangir/notebooks-and-scripts/raw/current/notebooks_and_scripts/workflow/generic.py), an abstraction to run mixed-type (cpu/gpu/...) [DAG](https://networkx.org/documentation/stable/reference/classes/digraph.html)s of bash commands on aws batch.
+also home to [`workflow`](https://github.com/kamangir/notebooks-and-scripts/raw/main/notebooks_and_scripts/workflow/generic.py), an abstraction to run mixed-type (cpu/gpu/...) [DAG](https://networkx.org/documentation/stable/reference/classes/digraph.html)s of bash commands on aws batch.
 
 ```bash
  > workflow help
 workflow create \
 	pattern=a-bc-d|hourglass,~upload \
 	-|<job-name> \
 	<command-line>
@@ -45,14 +45,14 @@
 workflow create pattern=hourglass .
 workflow submit to=aws_batch
 @watch - @download
 ```
 
 from https://arash-kamangir.medium.com/%EF%B8%8F-openai-experiments-54-e49117dc69ef
 
-| [`a-bc-d`](https://github.com/kamangir/notebooks-and-scripts/raw/current/notebooks_and_scripts/workflow/patterns/a-bc-d.dot) [🔗](https://kamangir-public.s3.ca-central-1.amazonaws.com/a-bc-d/workflow.gif?raw=true) | [`hourglass`](https://github.com/kamangir/notebooks-and-scripts/raw/current/notebooks_and_scripts/workflow/patterns/hourglass.dot) [🔗](https://kamangir-public.s3.ca-central-1.amazonaws.com/hourglass/workflow.gif?raw=true) | [`map-reduce`](https://github.com/kamangir/notebooks-and-scripts/raw/current/notebooks_and_scripts/workflow/patterns/map-reduce.dot) [🔗](https://kamangir-public.s3.ca-central-1.amazonaws.com/map-reduce/workflow.gif?raw=true) |
+| [`a-bc-d`](https://github.com/kamangir/notebooks-and-scripts/raw/main/notebooks_and_scripts/workflow/patterns/a-bc-d.dot) [🔗](https://kamangir-public.s3.ca-central-1.amazonaws.com/a-bc-d/workflow.gif?raw=true) | [`hourglass`](https://github.com/kamangir/notebooks-and-scripts/raw/main/notebooks_and_scripts/workflow/patterns/hourglass.dot) [🔗](https://kamangir-public.s3.ca-central-1.amazonaws.com/hourglass/workflow.gif?raw=true) | [`map-reduce`](https://github.com/kamangir/notebooks-and-scripts/raw/main/notebooks_and_scripts/workflow/patterns/map-reduce.dot) [🔗](https://kamangir-public.s3.ca-central-1.amazonaws.com/map-reduce/workflow.gif?raw=true) |
 | --------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | ![image](https://kamangir-public.s3.ca-central-1.amazonaws.com/a-bc-d/workflow.gif?raw=true)                                                              | ![image](https://kamangir-public.s3.ca-central-1.amazonaws.com/hourglass/workflow.gif?raw=true)                                                                    | ![image](https://kamangir-public.s3.ca-central-1.amazonaws.com/map-reduce/workflow.gif?raw=true)                                                                      |
 
 ---
 
 To use on [AWS SageMaker](https://aws.amazon.com/sagemaker/) replace `<plugin-name>` with `nbs` and follow [these instructions](https://github.com/kamangir/blue-plugin/blob/main/SageMaker.md).
```

### Comparing `notebooks_and_scripts-4.446.1/setup.py` & `notebooks_and_scripts-4.447.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from notebooks_and_scripts import NAME, VERSION, DESCRIPTION
 
 
 with open(os.path.join(os.path.dirname(__file__), "README.md")) as f:
     long_description = f.read().replace(
         "./",
-        "https://github.com/kamangir/notebooks-and-scripts/raw/current/",
+        "https://github.com/kamangir/notebooks-and-scripts/raw/main/",
     )
 
 setup(
     name=NAME,
     author="arash@kamangir.net",
     version=VERSION,
     description=DESCRIPTION,
```

