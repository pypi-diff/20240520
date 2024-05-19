# Comparing `tmp/roofai-4.15.1.tar.gz` & `tmp/roofai-4.16.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roofai-4.15.1.tar", last modified: Sun May 19 23:07:59 2024, max compression
+gzip compressed data, was "roofai-4.16.1.tar", last modified: Sun May 19 23:08:40 2024, max compression
```

## Comparing `roofai-4.15.1.tar` & `roofai-4.16.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 23:07:59.076399 roofai-4.15.1/
--rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-10-03 04:10:45.000000 roofai-4.15.1/LICENSE
--rw-r--r--   0 kamangir   (502) staff       (20)     3616 2024-05-19 23:07:59.075866 roofai-4.15.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     3137 2024-04-23 03:27:00.000000 roofai-4.15.1/README.md
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 23:07:59.073069 roofai-4.15.1/roofAI/
--rw-r--r--   0 kamangir   (502) staff       (20)      106 2024-05-19 23:07:54.000000 roofai-4.15.1/roofAI/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      751 2024-03-04 07:11:52.000000 roofai-4.15.1/roofAI/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)       87 2024-03-24 00:16:41.000000 roofai-4.15.1/roofAI/logger.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-10-03 04:10:45.000000 roofai-4.15.1/roofAI/urls.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 23:07:59.075299 roofai-4.15.1/roofAI.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)     3616 2024-05-19 23:07:59.000000 roofai-4.15.1/roofAI.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      216 2024-05-19 23:07:59.000000 roofai-4.15.1/roofAI.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-19 23:07:59.000000 roofai-4.15.1/roofAI.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        7 2024-05-19 23:07:59.000000 roofai-4.15.1/roofAI.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-19 23:07:59.076505 roofai-4.15.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      493 2024-05-19 23:02:29.000000 roofai-4.15.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 23:08:40.536372 roofai-4.16.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-10-03 04:10:45.000000 roofai-4.16.1/LICENSE
+-rw-r--r--   0 kamangir   (502) staff       (20)     3554 2024-05-19 23:08:40.535041 roofai-4.16.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     3117 2024-05-19 23:08:32.000000 roofai-4.16.1/README.md
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 23:08:40.530576 roofai-4.16.1/roofAI/
+-rw-r--r--   0 kamangir   (502) staff       (20)      106 2024-05-19 23:08:35.000000 roofai-4.16.1/roofAI/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      751 2024-03-04 07:11:52.000000 roofai-4.16.1/roofAI/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       87 2024-03-24 00:16:41.000000 roofai-4.16.1/roofAI/logger.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-10-03 04:10:45.000000 roofai-4.16.1/roofAI/urls.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 23:08:40.532960 roofai-4.16.1/roofAI.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     3554 2024-05-19 23:08:40.000000 roofai-4.16.1/roofAI.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      216 2024-05-19 23:08:40.000000 roofai-4.16.1/roofAI.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-19 23:08:40.000000 roofai-4.16.1/roofAI.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        7 2024-05-19 23:08:40.000000 roofai-4.16.1/roofAI.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-19 23:08:40.536611 roofai-4.16.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      493 2024-05-19 23:02:29.000000 roofai-4.16.1/setup.py
```

### Comparing `roofai-4.15.1/LICENSE` & `roofai-4.16.1/LICENSE`

 * *Files identical despite different names*

### Comparing `roofai-4.15.1/PKG-INFO` & `roofai-4.16.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roofAI
-Version: 4.15.1
+Version: 4.16.1
 Summary: 🏛️ everything AI about roofs.
 Author: arash@kamangir.net
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # roofAI 🏛️
 
@@ -96,12 +96,12 @@
 	[~download,dryrun,list,~log,plugin=<plugin-name>,warning] \
 	[filename.py|filename.py::test]
  . pytest roofAI.
 roofAI test [~dataset,dryrun,~semseg]
  . test roofAI.
 ```
 
-[![image](https://github.com/kamangir/assets/blob/main/roofAI/2023-11-12-20-30-49-02592-predict.gif?raw=true)](https://github.com/kamangir/roofAI/raw/main/roofAI/semseg/)
+![image](https://github.com/kamangir/assets/blob/main/roofAI/2023-11-12-20-30-49-02592-predict.gif?raw=true)
 
 ---
 
 To use on [AWS SageMaker](https://aws.amazon.com/sagemaker/) replace `<plugin-name>` with `roofAI` and follow [these instructions](https://github.com/kamangir/blue-plugin/blob/main/SageMaker.md).
```

### Comparing `roofai-4.15.1/README.md` & `roofai-4.16.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -88,12 +88,12 @@
 	[~download,dryrun,list,~log,plugin=<plugin-name>,warning] \
 	[filename.py|filename.py::test]
  . pytest roofAI.
 roofAI test [~dataset,dryrun,~semseg]
  . test roofAI.
 ```
 
-[![image](https://github.com/kamangir/assets/blob/main/roofAI/2023-11-12-20-30-49-02592-predict.gif?raw=true)](./roofAI/semseg/)
+![image](https://github.com/kamangir/assets/blob/main/roofAI/2023-11-12-20-30-49-02592-predict.gif?raw=true)
 
 ---
 
 To use on [AWS SageMaker](https://aws.amazon.com/sagemaker/) replace `<plugin-name>` with `roofAI` and follow [these instructions](https://github.com/kamangir/blue-plugin/blob/main/SageMaker.md).
```

### Comparing `roofai-4.15.1/roofAI/__main__.py` & `roofai-4.16.1/roofAI/__main__.py`

 * *Files identical despite different names*

### Comparing `roofai-4.15.1/roofAI.egg-info/PKG-INFO` & `roofai-4.16.1/roofAI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roofAI
-Version: 4.15.1
+Version: 4.16.1
 Summary: 🏛️ everything AI about roofs.
 Author: arash@kamangir.net
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # roofAI 🏛️
 
@@ -96,12 +96,12 @@
 	[~download,dryrun,list,~log,plugin=<plugin-name>,warning] \
 	[filename.py|filename.py::test]
  . pytest roofAI.
 roofAI test [~dataset,dryrun,~semseg]
  . test roofAI.
 ```
 
-[![image](https://github.com/kamangir/assets/blob/main/roofAI/2023-11-12-20-30-49-02592-predict.gif?raw=true)](https://github.com/kamangir/roofAI/raw/main/roofAI/semseg/)
+![image](https://github.com/kamangir/assets/blob/main/roofAI/2023-11-12-20-30-49-02592-predict.gif?raw=true)
 
 ---
 
 To use on [AWS SageMaker](https://aws.amazon.com/sagemaker/) replace `<plugin-name>` with `roofAI` and follow [these instructions](https://github.com/kamangir/blue-plugin/blob/main/SageMaker.md).
```

