# Comparing `tmp/desktop_env-0.1.8.tar.gz` & `tmp/desktop_env-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "desktop_env-0.1.8.tar", last modified: Fri May 10 08:27:17 2024, max compression
+gzip compressed data, was "desktop_env-0.1.9.tar", last modified: Fri May 10 08:42:20 2024, max compression
```

## Comparing `desktop_env-0.1.8.tar` & `desktop_env-0.1.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 08:27:17.374360 desktop_env-0.1.8/
--rw-rw-rw-   0        0        0    11358 2024-02-24 15:43:05.000000 desktop_env-0.1.8/LICENSE
--rw-rw-rw-   0        0        0     9260 2024-05-10 08:27:17.373851 desktop_env-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     7324 2024-04-21 11:49:28.000000 desktop_env-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 08:27:17.187383 desktop_env-0.1.8/desktop_env/
--rw-rw-rw-   0        0        0        2 2023-12-24 03:12:41.000000 desktop_env-0.1.8/desktop_env/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 08:27:17.217018 desktop_env-0.1.8/desktop_env/controllers/
--rw-rw-rw-   0        0        0        0 2023-11-21 09:05:29.000000 desktop_env-0.1.8/desktop_env/controllers/__init__.py
--rw-rw-rw-   0        0        0    15393 2024-03-21 03:16:56.000000 desktop_env-0.1.8/desktop_env/controllers/python.py
--rw-rw-rw-   0        0        0    29975 2024-04-13 14:40:47.000000 desktop_env-0.1.8/desktop_env/controllers/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-10 08:27:17.228084 desktop_env-0.1.8/desktop_env/envs/
--rw-rw-rw-   0        0        0    14491 2024-05-09 13:59:30.000000 desktop_env-0.1.8/desktop_env/envs/__init__.py
--rw-rw-rw-   0        0        0     7377 2024-01-14 13:22:15.000000 desktop_env-0.1.8/desktop_env/envs/actions.py
--rw-rw-rw-   0        0        0    14634 2024-04-21 11:31:18.000000 desktop_env-0.1.8/desktop_env/envs/desktop_env.py
-drwxrwxrwx   0        0        0        0 2024-05-10 08:27:17.231104 desktop_env-0.1.8/desktop_env/evaluators/
--rw-rw-rw-   0        0        0      113 2023-12-24 05:57:07.000000 desktop_env-0.1.8/desktop_env/evaluators/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 08:27:17.293202 desktop_env-0.1.8/desktop_env/evaluators/getters/
--rw-rw-rw-   0        0        0     1504 2024-04-13 14:50:54.000000 desktop_env-0.1.8/desktop_env/evaluators/getters/__init__.py
--rw-rw-rw-   0        0        0      537 2024-04-13 14:50:54.000000 desktop_env-0.1.8/desktop_env/evaluators/getters/calc.py
--rw-rw-rw-   0        0        0    62483 2024-04-01 11:46:38.000000 desktop_env-0.1.8/desktop_env/evaluators/getters/chrome.py
--rw-rw-rw-   0        0        0     4746 2024-03-10 07:16:40.000000 desktop_env-0.1.8/desktop_env/evaluators/getters/file.py
--rw-rw-rw-   0        0        0     1269 2024-03-08 12:39:20.000000 desktop_env-0.1.8/desktop_env/evaluators/getters/general.py
--rw-rw-rw-   0        0        0     1144 2024-01-30 18:56:45.000000 desktop_env-0.1.8/desktop_env/evaluators/getters/gimp.py
--rw-rw-rw-   0        0        0     7156 2024-03-08 11:36:11.000000 desktop_env-0.1.8/desktop_env/evaluators/getters/impress.py
--rw-rw-rw-   0        0        0      660 2024-01-26 05:22:46.000000 desktop_env-0.1.8/desktop_env/evaluators/getters/info.py
--rw-rw-rw-   0        0        0     7985 2024-03-08 12:47:17.000000 desktop_env-0.1.8/desktop_env/evaluators/getters/misc.py
--rw-rw-rw-   0        0        0      729 2024-01-13 16:57:53.000000 desktop_env-0.1.8/desktop_env/evaluators/getters/replay.py
--rw-rw-rw-   0        0        0     3768 2024-01-30 07:42:11.000000 desktop_env-0.1.8/desktop_env/evaluators/getters/vlc.py
--rw-rw-rw-   0        0        0     1113 2024-01-30 07:42:11.000000 desktop_env-0.1.8/desktop_env/evaluators/getters/vscode.py
-drwxrwxrwx   0        0        0        0 2024-05-10 08:27:17.371296 desktop_env-0.1.8/desktop_env/evaluators/metrics/
--rw-rw-rw-   0        0        0     4083 2024-04-13 14:50:54.000000 desktop_env-0.1.8/desktop_env/evaluators/metrics/__init__.py
--rw-rw-rw-   0        0        0     1877 2024-03-14 04:54:10.000000 desktop_env-0.1.8/desktop_env/evaluators/metrics/basic_os.py
--rw-rw-rw-   0        0        0    13473 2024-03-10 16:02:05.000000 desktop_env-0.1.8/desktop_env/evaluators/metrics/chrome.py
--rw-rw-rw-   0        0        0    28929 2024-04-02 06:37:07.000000 desktop_env-0.1.8/desktop_env/evaluators/metrics/docs.py
--rw-rw-rw-   0        0        0    17228 2024-04-01 06:53:32.000000 desktop_env-0.1.8/desktop_env/evaluators/metrics/general.py
--rw-rw-rw-   0        0        0    20366 2024-03-19 10:44:27.000000 desktop_env-0.1.8/desktop_env/evaluators/metrics/gimp.py
--rw-rw-rw-   0        0        0     1242 2024-03-14 04:54:10.000000 desktop_env-0.1.8/desktop_env/evaluators/metrics/libreoffice.py
--rw-rw-rw-   0        0        0     3316 2024-03-14 04:54:10.000000 desktop_env-0.1.8/desktop_env/evaluators/metrics/others.py
--rw-rw-rw-   0        0        0      832 2024-03-14 04:54:10.000000 desktop_env-0.1.8/desktop_env/evaluators/metrics/pdf.py
--rw-rw-rw-   0        0        0    22385 2024-03-21 14:05:41.000000 desktop_env-0.1.8/desktop_env/evaluators/metrics/slides.py
--rw-rw-rw-   0        0        0    23931 2024-03-14 04:54:10.000000 desktop_env-0.1.8/desktop_env/evaluators/metrics/table.py
--rw-rw-rw-   0        0        0     6801 2024-03-14 04:54:10.000000 desktop_env-0.1.8/desktop_env/evaluators/metrics/thunderbird.py
--rw-rw-rw-   0        0        0    29419 2024-03-08 12:47:17.000000 desktop_env-0.1.8/desktop_env/evaluators/metrics/utils.py
--rw-rw-rw-   0        0        0    14582 2024-01-25 04:36:46.000000 desktop_env-0.1.8/desktop_env/evaluators/metrics/vlc.py
--rw-rw-rw-   0        0        0     8034 2024-03-18 12:33:10.000000 desktop_env-0.1.8/desktop_env/evaluators/metrics/vscode.py
-drwxrwxrwx   0        0        0        0 2024-05-10 08:27:17.372802 desktop_env-0.1.8/desktop_env.egg-info/
--rw-rw-rw-   0        0        0     9260 2024-05-10 08:27:17.000000 desktop_env-0.1.8/desktop_env.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1552 2024-05-10 08:27:17.000000 desktop_env-0.1.8/desktop_env.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 08:27:17.000000 desktop_env-0.1.8/desktop_env.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      567 2024-05-10 08:27:17.000000 desktop_env-0.1.8/desktop_env.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-10 08:27:17.000000 desktop_env-0.1.8/desktop_env.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 08:27:17.374360 desktop_env-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     2805 2024-05-10 08:25:39.000000 desktop_env-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:42:20.181458 desktop_env-0.1.9/
+-rw-rw-rw-   0        0        0    11358 2024-02-24 15:43:05.000000 desktop_env-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0     9260 2024-05-10 08:42:20.181458 desktop_env-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     7324 2024-04-21 11:49:28.000000 desktop_env-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 08:42:19.664944 desktop_env-0.1.9/desktop_env/
+-rw-rw-rw-   0        0        0        2 2023-12-24 03:12:41.000000 desktop_env-0.1.9/desktop_env/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:42:19.789477 desktop_env-0.1.9/desktop_env/controllers/
+-rw-rw-rw-   0        0        0        0 2023-11-21 09:05:29.000000 desktop_env-0.1.9/desktop_env/controllers/__init__.py
+-rw-rw-rw-   0        0        0    15393 2024-03-21 03:16:56.000000 desktop_env-0.1.9/desktop_env/controllers/python.py
+-rw-rw-rw-   0        0        0    29975 2024-04-13 14:40:47.000000 desktop_env-0.1.9/desktop_env/controllers/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:42:19.809775 desktop_env-0.1.9/desktop_env/envs/
+-rw-rw-rw-   0        0        0    14615 2024-05-10 08:40:37.000000 desktop_env-0.1.9/desktop_env/envs/__init__.py
+-rw-rw-rw-   0        0        0     7377 2024-01-14 13:22:15.000000 desktop_env-0.1.9/desktop_env/envs/actions.py
+-rw-rw-rw-   0        0        0    14634 2024-04-21 11:31:18.000000 desktop_env-0.1.9/desktop_env/envs/desktop_env.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:42:19.818906 desktop_env-0.1.9/desktop_env/evaluators/
+-rw-rw-rw-   0        0        0      113 2023-12-24 05:57:07.000000 desktop_env-0.1.9/desktop_env/evaluators/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:42:19.917205 desktop_env-0.1.9/desktop_env/evaluators/getters/
+-rw-rw-rw-   0        0        0     1504 2024-04-13 14:50:54.000000 desktop_env-0.1.9/desktop_env/evaluators/getters/__init__.py
+-rw-rw-rw-   0        0        0      537 2024-04-13 14:50:54.000000 desktop_env-0.1.9/desktop_env/evaluators/getters/calc.py
+-rw-rw-rw-   0        0        0    62483 2024-04-01 11:46:38.000000 desktop_env-0.1.9/desktop_env/evaluators/getters/chrome.py
+-rw-rw-rw-   0        0        0     4746 2024-03-10 07:16:40.000000 desktop_env-0.1.9/desktop_env/evaluators/getters/file.py
+-rw-rw-rw-   0        0        0     1269 2024-03-08 12:39:20.000000 desktop_env-0.1.9/desktop_env/evaluators/getters/general.py
+-rw-rw-rw-   0        0        0     1144 2024-01-30 18:56:45.000000 desktop_env-0.1.9/desktop_env/evaluators/getters/gimp.py
+-rw-rw-rw-   0        0        0     7156 2024-03-08 11:36:11.000000 desktop_env-0.1.9/desktop_env/evaluators/getters/impress.py
+-rw-rw-rw-   0        0        0      660 2024-01-26 05:22:46.000000 desktop_env-0.1.9/desktop_env/evaluators/getters/info.py
+-rw-rw-rw-   0        0        0     7985 2024-03-08 12:47:17.000000 desktop_env-0.1.9/desktop_env/evaluators/getters/misc.py
+-rw-rw-rw-   0        0        0      729 2024-01-13 16:57:53.000000 desktop_env-0.1.9/desktop_env/evaluators/getters/replay.py
+-rw-rw-rw-   0        0        0     3768 2024-01-30 07:42:11.000000 desktop_env-0.1.9/desktop_env/evaluators/getters/vlc.py
+-rw-rw-rw-   0        0        0     1113 2024-01-30 07:42:11.000000 desktop_env-0.1.9/desktop_env/evaluators/getters/vscode.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:42:20.162662 desktop_env-0.1.9/desktop_env/evaluators/metrics/
+-rw-rw-rw-   0        0        0     4083 2024-04-13 14:50:54.000000 desktop_env-0.1.9/desktop_env/evaluators/metrics/__init__.py
+-rw-rw-rw-   0        0        0     1877 2024-03-14 04:54:10.000000 desktop_env-0.1.9/desktop_env/evaluators/metrics/basic_os.py
+-rw-rw-rw-   0        0        0    13473 2024-03-10 16:02:05.000000 desktop_env-0.1.9/desktop_env/evaluators/metrics/chrome.py
+-rw-rw-rw-   0        0        0    28929 2024-04-02 06:37:07.000000 desktop_env-0.1.9/desktop_env/evaluators/metrics/docs.py
+-rw-rw-rw-   0        0        0    17228 2024-04-01 06:53:32.000000 desktop_env-0.1.9/desktop_env/evaluators/metrics/general.py
+-rw-rw-rw-   0        0        0    20366 2024-03-19 10:44:27.000000 desktop_env-0.1.9/desktop_env/evaluators/metrics/gimp.py
+-rw-rw-rw-   0        0        0     1242 2024-03-14 04:54:10.000000 desktop_env-0.1.9/desktop_env/evaluators/metrics/libreoffice.py
+-rw-rw-rw-   0        0        0     3316 2024-03-14 04:54:10.000000 desktop_env-0.1.9/desktop_env/evaluators/metrics/others.py
+-rw-rw-rw-   0        0        0      832 2024-03-14 04:54:10.000000 desktop_env-0.1.9/desktop_env/evaluators/metrics/pdf.py
+-rw-rw-rw-   0        0        0    22385 2024-03-21 14:05:41.000000 desktop_env-0.1.9/desktop_env/evaluators/metrics/slides.py
+-rw-rw-rw-   0        0        0    23931 2024-03-14 04:54:10.000000 desktop_env-0.1.9/desktop_env/evaluators/metrics/table.py
+-rw-rw-rw-   0        0        0     6801 2024-03-14 04:54:10.000000 desktop_env-0.1.9/desktop_env/evaluators/metrics/thunderbird.py
+-rw-rw-rw-   0        0        0    29419 2024-03-08 12:47:17.000000 desktop_env-0.1.9/desktop_env/evaluators/metrics/utils.py
+-rw-rw-rw-   0        0        0    14582 2024-01-25 04:36:46.000000 desktop_env-0.1.9/desktop_env/evaluators/metrics/vlc.py
+-rw-rw-rw-   0        0        0     8034 2024-03-18 12:33:10.000000 desktop_env-0.1.9/desktop_env/evaluators/metrics/vscode.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:42:20.172347 desktop_env-0.1.9/desktop_env.egg-info/
+-rw-rw-rw-   0        0        0     9260 2024-05-10 08:42:19.000000 desktop_env-0.1.9/desktop_env.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1552 2024-05-10 08:42:19.000000 desktop_env-0.1.9/desktop_env.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 08:42:19.000000 desktop_env-0.1.9/desktop_env.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      567 2024-05-10 08:42:19.000000 desktop_env-0.1.9/desktop_env.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-10 08:42:19.000000 desktop_env-0.1.9/desktop_env.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 08:42:20.190553 desktop_env-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     2805 2024-05-10 08:40:37.000000 desktop_env-0.1.9/setup.py
```

### Comparing `desktop_env-0.1.8/LICENSE` & `desktop_env-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.8/PKG-INFO` & `desktop_env-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: desktop_env
-Version: 0.1.8
+Version: 0.1.9
 Summary: The package provides a desktop environment for setting and evaluating desktop automation tasks.
 Home-page: https://github.com/xlang-ai/desktop_env
 Author: Tianbao Xie, Danyang Zhang,  Jixuan Chen, Xiaochuan Li, Siheng Zhao, Ruisheng Cao, Toh Jing Hua, etc.
 Author-email: tianbaoxiexxx@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: desktop_env Version: 0.1.8 Summary: The package
+Metadata-Version: 2.1 Name: desktop_env Version: 0.1.9 Summary: The package
 provides a desktop environment for setting and evaluating desktop automation
 tasks. Home-page: https://github.com/xlang-ai/desktop_env Author: Tianbao Xie,
 Danyang Zhang, Jixuan Chen, Xiaochuan Li, Siheng Zhao, Ruisheng Cao, Toh Jing
 Hua, etc. Author-email: tianbaoxiexxx@gmail.com Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.9
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
```

### Comparing `desktop_env-0.1.8/README.md` & `desktop_env-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.8/desktop_env/controllers/python.py` & `desktop_env-0.1.9/desktop_env/controllers/python.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.8/desktop_env/controllers/setup.py` & `desktop_env-0.1.9/desktop_env/controllers/setup.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.8/desktop_env/envs/__init__.py` & `desktop_env-0.1.9/desktop_env/envs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import zipfile
 from time import sleep
 import shutil
 import psutil
 import requests
 from tqdm import tqdm
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 
 MAX_RETRY_TIMES = 10
 UBUNTU_ARM_URL = "https://huggingface.co/datasets/xlangai/ubuntu_arm/resolve/main/Ubuntu.zip"
 UBUNTU_X86_URL = "https://huggingface.co/datasets/xlangai/ubuntu_x86/resolve/main/Ubuntu.zip"
 DOWNLOADED_FILE_NAME = "Ubuntu.zip"
 REGISTRY_PATH = '.vms'
 VMS_DIR = "./vm_data"
@@ -96,14 +96,18 @@
 
             # Check and clean on the files inside vms_dir, delete the unregistered ones
             vm_names = os.listdir(vms_dir)
             for vm_name in vm_names:
                 # skip the downloaded .zip file
                 if vm_name == DOWNLOADED_FILE_NAME:
                     continue
+                # Skip the .DS_Store file on macOS
+                if vm_name == ".DS_Store":
+                    continue
+
                 flag = True
                 for vm_path in vm_paths:
                     if vm_name + ".vmx" in vm_path:
                         flag = False
                 if flag:
                     shutil.rmtree(os.path.join(vms_dir, vm_name))
```

### Comparing `desktop_env-0.1.8/desktop_env/envs/actions.py` & `desktop_env-0.1.9/desktop_env/envs/actions.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.8/desktop_env/envs/desktop_env.py` & `desktop_env-0.1.9/desktop_env/envs/desktop_env.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.8/desktop_env/evaluators/getters/__init__.py` & `desktop_env-0.1.9/desktop_env/evaluators/getters/__init__.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.8/desktop_env/evaluators/getters/calc.py` & `desktop_env-0.1.9/desktop_env/evaluators/getters/calc.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.8/desktop_env/evaluators/getters/chrome.py` & `desktop_env-0.1.9/desktop_env/evaluators/getters/chrome.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.8/desktop_env/evaluators/getters/file.py` & `desktop_env-0.1.9/desktop_env/evaluators/getters/file.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.8/desktop_env/evaluators/getters/general.py` & `desktop_env-0.1.9/desktop_env/evaluators/getters/general.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.8/desktop_env/evaluators/getters/gimp.py` & `desktop_env-0.1.9/desktop_env/evaluators/getters/gimp.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.8/desktop_env/evaluators/getters/impress.py` & `desktop_env-0.1.9/desktop_env/evaluators/getters/impress.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.8/desktop_env/evaluators/getters/info.py` & `desktop_env-0.1.9/desktop_env/evaluators/getters/info.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.8/desktop_env/evaluators/getters/misc.py` & `desktop_env-0.1.9/desktop_env/evaluators/getters/misc.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.8/desktop_env/evaluators/getters/replay.py` & `desktop_env-0.1.9/desktop_env/evaluators/getters/replay.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.8/desktop_env/evaluators/getters/vlc.py` & `desktop_env-0.1.9/desktop_env/evaluators/getters/vlc.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.8/desktop_env/evaluators/getters/vscode.py` & `desktop_env-0.1.9/desktop_env/evaluators/getters/vscode.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.8/desktop_env/evaluators/metrics/__init__.py` & `desktop_env-0.1.9/desktop_env/evaluators/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.8/desktop_env/evaluators/metrics/basic_os.py` & `desktop_env-0.1.9/desktop_env/evaluators/metrics/basic_os.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.8/desktop_env/evaluators/metrics/chrome.py` & `desktop_env-0.1.9/desktop_env/evaluators/metrics/chrome.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.8/desktop_env/evaluators/metrics/docs.py` & `desktop_env-0.1.9/desktop_env/evaluators/metrics/docs.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.8/desktop_env/evaluators/metrics/general.py` & `desktop_env-0.1.9/desktop_env/evaluators/metrics/general.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.8/desktop_env/evaluators/metrics/gimp.py` & `desktop_env-0.1.9/desktop_env/evaluators/metrics/gimp.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.8/desktop_env/evaluators/metrics/libreoffice.py` & `desktop_env-0.1.9/desktop_env/evaluators/metrics/libreoffice.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.8/desktop_env/evaluators/metrics/others.py` & `desktop_env-0.1.9/desktop_env/evaluators/metrics/others.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.8/desktop_env/evaluators/metrics/pdf.py` & `desktop_env-0.1.9/desktop_env/evaluators/metrics/pdf.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.8/desktop_env/evaluators/metrics/slides.py` & `desktop_env-0.1.9/desktop_env/evaluators/metrics/slides.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.8/desktop_env/evaluators/metrics/table.py` & `desktop_env-0.1.9/desktop_env/evaluators/metrics/table.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.8/desktop_env/evaluators/metrics/thunderbird.py` & `desktop_env-0.1.9/desktop_env/evaluators/metrics/thunderbird.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.8/desktop_env/evaluators/metrics/utils.py` & `desktop_env-0.1.9/desktop_env/evaluators/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.8/desktop_env/evaluators/metrics/vlc.py` & `desktop_env-0.1.9/desktop_env/evaluators/metrics/vlc.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.8/desktop_env/evaluators/metrics/vscode.py` & `desktop_env-0.1.9/desktop_env/evaluators/metrics/vscode.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.8/desktop_env.egg-info/PKG-INFO` & `desktop_env-0.1.9/desktop_env.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: desktop_env
-Version: 0.1.8
+Version: 0.1.9
 Summary: The package provides a desktop environment for setting and evaluating desktop automation tasks.
 Home-page: https://github.com/xlang-ai/desktop_env
 Author: Tianbao Xie, Danyang Zhang,  Jixuan Chen, Xiaochuan Li, Siheng Zhao, Ruisheng Cao, Toh Jing Hua, etc.
 Author-email: tianbaoxiexxx@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: desktop_env Version: 0.1.8 Summary: The package
+Metadata-Version: 2.1 Name: desktop_env Version: 0.1.9 Summary: The package
 provides a desktop environment for setting and evaluating desktop automation
 tasks. Home-page: https://github.com/xlang-ai/desktop_env Author: Tianbao Xie,
 Danyang Zhang, Jixuan Chen, Xiaochuan Li, Siheng Zhao, Ruisheng Cao, Toh Jing
 Hua, etc. Author-email: tianbaoxiexxx@gmail.com Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.9
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
```

### Comparing `desktop_env-0.1.8/desktop_env.egg-info/SOURCES.txt` & `desktop_env-0.1.9/desktop_env.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.8/desktop_env.egg-info/requires.txt` & `desktop_env-0.1.9/desktop_env.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.8/setup.py` & `desktop_env-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         except subprocess.CalledProcessError as e:
             print("Failed to run 'playwright install'. Please run 'playwright install' manually.")
             print(e)
 
 
 setup(
     name="desktop_env",
-    version="0.1.8",
+    version="0.1.9",
     author="Tianbao Xie, Danyang Zhang,  Jixuan Chen, Xiaochuan Li, Siheng Zhao, Ruisheng Cao, Toh Jing Hua, etc.",
     author_email="tianbaoxiexxx@gmail.com",
     description="The package provides a desktop environment for setting and evaluating desktop automation tasks.",
     long_description=open('README.md', encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/xlang-ai/desktop_env",
     packages=find_packages(),
```

