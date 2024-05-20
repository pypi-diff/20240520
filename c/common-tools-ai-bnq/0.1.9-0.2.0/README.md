# Comparing `tmp/common-tools-ai-bnq-0.1.9.tar.gz` & `tmp/common-tools-ai-bnq-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common-tools-ai-bnq-0.1.9.tar", last modified: Fri May 17 09:07:34 2024, max compression
+gzip compressed data, was "common-tools-ai-bnq-0.2.0.tar", last modified: Mon May 20 09:14:57 2024, max compression
```

## Comparing `common-tools-ai-bnq-0.1.9.tar` & `common-tools-ai-bnq-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 09:07:34.495803 common-tools-ai-bnq-0.1.9/
--rw-rw-rw-   0        0        0     3204 2024-05-17 09:07:34.494801 common-tools-ai-bnq-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     2977 2024-05-17 08:21:09.000000 common-tools-ai-bnq-0.1.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 09:07:34.478725 common-tools-ai-bnq-0.1.9/bnq_py_core/
--rw-rw-rw-   0        0        0      412 2024-05-14 03:05:23.000000 common-tools-ai-bnq-0.1.9/bnq_py_core/__init__.py
--rw-rw-rw-   0        0        0     1088 2024-05-06 07:47:07.000000 common-tools-ai-bnq-0.1.9/bnq_py_core/cos_connect.py
--rw-rw-rw-   0        0        0     7552 2024-05-17 08:45:24.000000 common-tools-ai-bnq-0.1.9/bnq_py_core/logger_record.py
--rw-rw-rw-   0        0        0     3218 2024-05-06 09:03:26.000000 common-tools-ai-bnq-0.1.9/bnq_py_core/nacos_connect.py
--rw-rw-rw-   0        0        0     2076 2024-05-13 11:48:35.000000 common-tools-ai-bnq-0.1.9/bnq_py_core/read_conf_from_ini.py
--rw-rw-rw-   0        0        0      716 2024-03-27 09:35:48.000000 common-tools-ai-bnq-0.1.9/bnq_py_core/singleton.py
-drwxrwxrwx   0        0        0        0 2024-05-17 09:07:34.494801 common-tools-ai-bnq-0.1.9/common_tools_ai_bnq.egg-info/
--rw-rw-rw-   0        0        0     3204 2024-05-17 09:07:34.000000 common-tools-ai-bnq-0.1.9/common_tools_ai_bnq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      400 2024-05-17 09:07:34.000000 common-tools-ai-bnq-0.1.9/common_tools_ai_bnq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 09:07:34.000000 common-tools-ai-bnq-0.1.9/common_tools_ai_bnq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      131 2024-05-17 09:07:34.000000 common-tools-ai-bnq-0.1.9/common_tools_ai_bnq.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-17 09:07:34.000000 common-tools-ai-bnq-0.1.9/common_tools_ai_bnq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-17 09:07:34.495803 common-tools-ai-bnq-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0      856 2024-05-17 09:07:27.000000 common-tools-ai-bnq-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:14:57.232147 common-tools-ai-bnq-0.2.0/
+-rw-rw-rw-   0        0        0     3204 2024-05-20 09:14:57.232040 common-tools-ai-bnq-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2977 2024-05-17 08:21:09.000000 common-tools-ai-bnq-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 09:14:57.209214 common-tools-ai-bnq-0.2.0/bnq_py_core/
+-rw-rw-rw-   0        0        0      412 2024-05-14 03:05:23.000000 common-tools-ai-bnq-0.2.0/bnq_py_core/__init__.py
+-rw-rw-rw-   0        0        0     1088 2024-05-06 07:47:07.000000 common-tools-ai-bnq-0.2.0/bnq_py_core/cos_connect.py
+-rw-rw-rw-   0        0        0     7687 2024-05-20 09:13:46.000000 common-tools-ai-bnq-0.2.0/bnq_py_core/logger_record.py
+-rw-rw-rw-   0        0        0     3218 2024-05-06 09:03:26.000000 common-tools-ai-bnq-0.2.0/bnq_py_core/nacos_connect.py
+-rw-rw-rw-   0        0        0     1574 2024-05-20 08:46:33.000000 common-tools-ai-bnq-0.2.0/bnq_py_core/read_conf_from_ini.py
+-rw-rw-rw-   0        0        0      716 2024-03-27 09:35:48.000000 common-tools-ai-bnq-0.2.0/bnq_py_core/singleton.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:14:57.209214 common-tools-ai-bnq-0.2.0/bnq_py_core/util/
+-rw-rw-rw-   0        0        0      122 2024-05-20 08:34:05.000000 common-tools-ai-bnq-0.2.0/bnq_py_core/util/__init__.py
+-rw-rw-rw-   0        0        0      662 2024-05-20 08:39:57.000000 common-tools-ai-bnq-0.2.0/bnq_py_core/util/time_zone.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:14:57.229497 common-tools-ai-bnq-0.2.0/common_tools_ai_bnq.egg-info/
+-rw-rw-rw-   0        0        0     3204 2024-05-20 09:14:57.000000 common-tools-ai-bnq-0.2.0/common_tools_ai_bnq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      459 2024-05-20 09:14:57.000000 common-tools-ai-bnq-0.2.0/common_tools_ai_bnq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 09:14:57.000000 common-tools-ai-bnq-0.2.0/common_tools_ai_bnq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2024-05-20 09:14:57.000000 common-tools-ai-bnq-0.2.0/common_tools_ai_bnq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-20 09:14:57.000000 common-tools-ai-bnq-0.2.0/common_tools_ai_bnq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 09:14:57.232147 common-tools-ai-bnq-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      881 2024-05-20 09:14:51.000000 common-tools-ai-bnq-0.2.0/setup.py
```

### Comparing `common-tools-ai-bnq-0.1.9/PKG-INFO` & `common-tools-ai-bnq-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-tools-ai-bnq
-Version: 0.1.9
+Version: 0.2.0
 Summary: Common tools of AI module for BNQ
 Home-page: UNKNOWN
 Author: BNQ
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `common-tools-ai-bnq-0.1.9/README.md` & `common-tools-ai-bnq-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `common-tools-ai-bnq-0.1.9/bnq_py_core/cos_connect.py` & `common-tools-ai-bnq-0.2.0/bnq_py_core/cos_connect.py`

 * *Files identical despite different names*

### Comparing `common-tools-ai-bnq-0.1.9/bnq_py_core/logger_record.py` & `common-tools-ai-bnq-0.2.0/bnq_py_core/logger_record.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import os
 import pathlib
 import sys
 import time
 
 from structlog import configure, processors, stdlib
 from termcolor import colored
+from util.time_zone import BeijingFormatter
 
 
 class _LoggingF(object):
     """
     日志记录父类
     """
 
@@ -36,17 +37,19 @@
         :return:
         """
         return {
             "version": 1,
             "disable_existing_loggers": False,
             "formatters": {
                 "default": {
+                    "()": BeijingFormatter,
                     "format": '%(asctime)s - %(levelname)s - %(name)s - %(message)s'
                 },
                 "console": {
+                    "()": BeijingFormatter,
                     "format": colored(f'[%(asctime)s][%(levelname)1.1s][%(process)d][%(name)s]', 'green') + colored(
                         f'(%(filename)s %(lineno)d)', 'yellow') + ': %(message)s'
                 }
             },
             "handlers": {
                 "console_handler": {
                     "class": "logging.StreamHandler",
```

### Comparing `common-tools-ai-bnq-0.1.9/bnq_py_core/nacos_connect.py` & `common-tools-ai-bnq-0.2.0/bnq_py_core/nacos_connect.py`

 * *Files identical despite different names*

### Comparing `common-tools-ai-bnq-0.1.9/bnq_py_core/singleton.py` & `common-tools-ai-bnq-0.2.0/bnq_py_core/singleton.py`

 * *Files identical despite different names*

### Comparing `common-tools-ai-bnq-0.1.9/common_tools_ai_bnq.egg-info/PKG-INFO` & `common-tools-ai-bnq-0.2.0/common_tools_ai_bnq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-tools-ai-bnq
-Version: 0.1.9
+Version: 0.2.0
 Summary: Common tools of AI module for BNQ
 Home-page: UNKNOWN
 Author: BNQ
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `common-tools-ai-bnq-0.1.9/setup.py` & `common-tools-ai-bnq-0.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,24 +7,25 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='common-tools-ai-bnq',
-    version='0.1.9',
+    version='0.2.0',
     packages=find_packages(),
     install_requires=[
         # 依赖项列表
         'structlog==23.1.0',
         'concurrent-log-handler==0.9.25',
         'nacos-sdk-python==0.1.12',
         'PyYAML==6.0.1',
         'cos-python-sdk-v5==1.9.28',
-        'termcolor==2.4.0'
+        'termcolor==2.4.0',
+        'pytz==2024.1'
     ],
     # 其他元数据，如作者、描述等
     author='BNQ',
     description='Common tools of AI module for BNQ',
     long_description=long_description,
     long_description_content_type="text/markdown",  # 指明内容类型为markdown
 )
```

