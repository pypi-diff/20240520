# Comparing `tmp/alibabacloud_dm20151123-1.1.1.tar.gz` & `tmp/alibabacloud_dm20151123-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dm20151123-1.1.1.tar", last modified: Wed May 15 02:02:23 2024, max compression
+gzip compressed data, was "dist/alibabacloud_dm20151123-1.1.2.tar", last modified: Mon May 20 03:20:16 2024, max compression
```

## Comparing `alibabacloud_dm20151123-1.1.1.tar` & `alibabacloud_dm20151123-1.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 02:02:23.000000 alibabacloud_dm20151123-1.1.1/
--rw-r--r--   0 root         (0) root         (0)     2195 2024-05-15 02:02:23.000000 alibabacloud_dm20151123-1.1.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-05-15 02:02:23.000000 alibabacloud_dm20151123-1.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-05-15 02:02:23.000000 alibabacloud_dm20151123-1.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2394 2024-05-15 02:02:23.000000 alibabacloud_dm20151123-1.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1091 2024-05-15 02:02:23.000000 alibabacloud_dm20151123-1.1.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1176 2024-05-15 02:02:23.000000 alibabacloud_dm20151123-1.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 02:02:23.000000 alibabacloud_dm20151123-1.1.1/alibabacloud_dm20151123/
--rw-r--r--   0 root         (0) root         (0)       21 2024-05-15 02:02:23.000000 alibabacloud_dm20151123-1.1.1/alibabacloud_dm20151123/__init__.py
--rw-r--r--   0 root         (0) root         (0)   198476 2024-05-15 02:02:23.000000 alibabacloud_dm20151123-1.1.1/alibabacloud_dm20151123/client.py
--rw-r--r--   0 root         (0) root         (0)   247209 2024-05-15 02:02:23.000000 alibabacloud_dm20151123-1.1.1/alibabacloud_dm20151123/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 02:02:23.000000 alibabacloud_dm20151123-1.1.1/alibabacloud_dm20151123.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2394 2024-05-15 02:02:23.000000 alibabacloud_dm20151123-1.1.1/alibabacloud_dm20151123.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      412 2024-05-15 02:02:23.000000 alibabacloud_dm20151123-1.1.1/alibabacloud_dm20151123.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 02:02:23.000000 alibabacloud_dm20151123-1.1.1/alibabacloud_dm20151123.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-05-15 02:02:23.000000 alibabacloud_dm20151123-1.1.1/alibabacloud_dm20151123.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2024-05-15 02:02:23.000000 alibabacloud_dm20151123-1.1.1/alibabacloud_dm20151123.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-05-15 02:02:23.000000 alibabacloud_dm20151123-1.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2606 2024-05-15 02:02:23.000000 alibabacloud_dm20151123-1.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 03:20:16.000000 alibabacloud_dm20151123-1.1.2/
+-rw-r--r--   0 root         (0) root         (0)     2260 2024-05-20 03:20:15.000000 alibabacloud_dm20151123-1.1.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-20 03:20:15.000000 alibabacloud_dm20151123-1.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-20 03:20:15.000000 alibabacloud_dm20151123-1.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2394 2024-05-20 03:20:16.000000 alibabacloud_dm20151123-1.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1091 2024-05-20 03:20:15.000000 alibabacloud_dm20151123-1.1.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1176 2024-05-20 03:20:15.000000 alibabacloud_dm20151123-1.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 03:20:16.000000 alibabacloud_dm20151123-1.1.2/alibabacloud_dm20151123/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-20 03:20:15.000000 alibabacloud_dm20151123-1.1.2/alibabacloud_dm20151123/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   198476 2024-05-20 03:20:15.000000 alibabacloud_dm20151123-1.1.2/alibabacloud_dm20151123/client.py
+-rw-r--r--   0 root         (0) root         (0)   247209 2024-05-20 03:20:15.000000 alibabacloud_dm20151123-1.1.2/alibabacloud_dm20151123/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 03:20:16.000000 alibabacloud_dm20151123-1.1.2/alibabacloud_dm20151123.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2394 2024-05-20 03:20:16.000000 alibabacloud_dm20151123-1.1.2/alibabacloud_dm20151123.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      412 2024-05-20 03:20:16.000000 alibabacloud_dm20151123-1.1.2/alibabacloud_dm20151123.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 03:20:16.000000 alibabacloud_dm20151123-1.1.2/alibabacloud_dm20151123.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-20 03:20:16.000000 alibabacloud_dm20151123-1.1.2/alibabacloud_dm20151123.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2024-05-20 03:20:16.000000 alibabacloud_dm20151123-1.1.2/alibabacloud_dm20151123.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-20 03:20:16.000000 alibabacloud_dm20151123-1.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2606 2024-05-20 03:20:15.000000 alibabacloud_dm20151123-1.1.2/setup.py
```

### Comparing `alibabacloud_dm20151123-1.1.1/ChangeLog.md` & `alibabacloud_dm20151123-1.1.2/ChangeLog.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2024-05-15 Version: 1.1.1
+- Generated python 2015-11-23 for Dm.
+
 2024-04-22 Version: 1.1.0
 - Support API CreateUserSuppression.
 - Support API GetSuppressionListLevel.
 - Support API ListUserSuppression.
 - Support API RemoveUserSuppression.
 - Support API SetSuppressionListLevel.
 - Update API BatchSendMail: add param UnSubscribeFilterLevel.
```

### Comparing `alibabacloud_dm20151123-1.1.1/LICENSE` & `alibabacloud_dm20151123-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dm20151123-1.1.1/PKG-INFO` & `alibabacloud_dm20151123-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dm20151123
-Version: 1.1.1
+Version: 1.1.2
 Summary: Alibaba Cloud Dm (20151123) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dm20151123-1.1.1/README-CN.md` & `alibabacloud_dm20151123-1.1.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dm20151123-1.1.1/README.md` & `alibabacloud_dm20151123-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dm20151123-1.1.1/alibabacloud_dm20151123/client.py` & `alibabacloud_dm20151123-1.1.2/alibabacloud_dm20151123/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dm20151123-1.1.1/alibabacloud_dm20151123/models.py` & `alibabacloud_dm20151123-1.1.2/alibabacloud_dm20151123/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dm20151123-1.1.1/alibabacloud_dm20151123.egg-info/PKG-INFO` & `alibabacloud_dm20151123-1.1.2/alibabacloud_dm20151123.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dm20151123
-Version: 1.1.1
+Version: 1.1.2
 Summary: Alibaba Cloud Dm (20151123) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dm20151123-1.1.1/setup.py` & `alibabacloud_dm20151123-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dm20151123.
 
-Created on 14/05/2024
+Created on 20/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dm20151123"
 NAME = "alibabacloud_dm20151123" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dm (20151123) SDK Library for Python"
```

