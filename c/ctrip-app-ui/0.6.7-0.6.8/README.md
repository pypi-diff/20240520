# Comparing `tmp/ctrip-app-ui-0.6.7.tar.gz` & `tmp/ctrip-app-ui-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-app-ui-0.6.7.tar", last modified: Mon May 20 03:44:23 2024, max compression
+gzip compressed data, was "ctrip-app-ui-0.6.8.tar", last modified: Mon May 20 06:05:30 2024, max compression
```

## Comparing `ctrip-app-ui-0.6.7.tar` & `ctrip-app-ui-0.6.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 03:44:23.301082 ctrip-app-ui-0.6.7/
--rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.6.7/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-20 03:44:23.299088 ctrip-app-ui-0.6.7/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.6.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 03:44:23.290106 ctrip-app-ui-0.6.7/capp_ui/
--rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.6.7/capp_ui/__init__.py
--rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.6.7/capp_ui/config.py
--rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.6.7/capp_ui/date_extend.py
--rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.6.7/capp_ui/device.py
--rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.6.7/capp_ui/dir.py
--rw-rw-rw-   0        0        0    52558 2024-05-20 03:43:59.000000 ctrip-app-ui-0.6.7/capp_ui/domain_service.py
--rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.6.7/capp_ui/fee.py
--rw-rw-rw-   0        0        0     5414 2024-05-18 14:39:38.000000 ctrip-app-ui-0.6.7/capp_ui/libs.py
--rw-rw-rw-   0        0        0    24821 2024-05-13 17:15:14.000000 ctrip-app-ui-0.6.7/capp_ui/mobile_terminals.py
--rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.6.7/capp_ui/platforms.py
--rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.6.7/capp_ui/test.py
--rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.6.7/capp_ui/utils.py
--rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.6.7/capp_ui/validators.py
-drwxrwxrwx   0        0        0        0 2024-05-20 03:44:23.298091 ctrip-app-ui-0.6.7/ctrip_app_ui.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-20 03:44:23.000000 ctrip-app-ui-0.6.7/ctrip_app_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      460 2024-05-20 03:44:23.000000 ctrip-app-ui-0.6.7/ctrip_app_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 03:44:23.000000 ctrip-app-ui-0.6.7/ctrip_app_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-20 03:44:23.000000 ctrip-app-ui-0.6.7/ctrip_app_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-20 03:44:23.000000 ctrip-app-ui-0.6.7/ctrip_app_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 03:44:23.301082 ctrip-app-ui-0.6.7/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-20 03:44:18.000000 ctrip-app-ui-0.6.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 06:05:30.292165 ctrip-app-ui-0.6.8/
+-rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.6.8/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-20 06:05:30.291168 ctrip-app-ui-0.6.8/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.6.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 06:05:30.282192 ctrip-app-ui-0.6.8/capp_ui/
+-rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.6.8/capp_ui/__init__.py
+-rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.6.8/capp_ui/config.py
+-rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.6.8/capp_ui/date_extend.py
+-rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.6.8/capp_ui/device.py
+-rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.6.8/capp_ui/dir.py
+-rw-rw-rw-   0        0        0    52611 2024-05-20 06:05:05.000000 ctrip-app-ui-0.6.8/capp_ui/domain_service.py
+-rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.6.8/capp_ui/fee.py
+-rw-rw-rw-   0        0        0     5414 2024-05-18 14:39:38.000000 ctrip-app-ui-0.6.8/capp_ui/libs.py
+-rw-rw-rw-   0        0        0    24821 2024-05-13 17:15:14.000000 ctrip-app-ui-0.6.8/capp_ui/mobile_terminals.py
+-rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.6.8/capp_ui/platforms.py
+-rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.6.8/capp_ui/test.py
+-rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.6.8/capp_ui/utils.py
+-rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.6.8/capp_ui/validators.py
+drwxrwxrwx   0        0        0        0 2024-05-20 06:05:30.290171 ctrip-app-ui-0.6.8/ctrip_app_ui.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-20 06:05:30.000000 ctrip-app-ui-0.6.8/ctrip_app_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      460 2024-05-20 06:05:30.000000 ctrip-app-ui-0.6.8/ctrip_app_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 06:05:30.000000 ctrip-app-ui-0.6.8/ctrip_app_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-20 06:05:30.000000 ctrip-app-ui-0.6.8/ctrip_app_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-20 06:05:30.000000 ctrip-app-ui-0.6.8/ctrip_app_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 06:05:30.293163 ctrip-app-ui-0.6.8/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-20 06:05:26.000000 ctrip-app-ui-0.6.8/setup.py
```

### Comparing `ctrip-app-ui-0.6.7/LICENSE` & `ctrip-app-ui-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.7/capp_ui/config.py` & `ctrip-app-ui-0.6.8/capp_ui/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.7/capp_ui/date_extend.py` & `ctrip-app-ui-0.6.8/capp_ui/date_extend.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.7/capp_ui/device.py` & `ctrip-app-ui-0.6.8/capp_ui/device.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.7/capp_ui/dir.py` & `ctrip-app-ui-0.6.8/capp_ui/dir.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.7/capp_ui/domain_service.py` & `ctrip-app-ui-0.6.8/capp_ui/domain_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -516,14 +516,15 @@
             file_name = join_path([get_images_dir(), "取消订单弹框_取消订单.png"])
             if is_exists(file_name):
                 temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
                 pos = self.device.exists(v=temp)
                 if pos:
                     return {"pos": pos}
             else:
+                # (729, 1189) Huawei Mate 20 坐标
                 logger.warning("文件{}，没找到".format(file_name))
         except (Exception,):
             pass
         try:
             cancel_order = self.device.poco(
                 type="android.widget.TextView", name="Button_Text_取消订单", text="取消订单"
             )
```

### Comparing `ctrip-app-ui-0.6.7/capp_ui/fee.py` & `ctrip-app-ui-0.6.8/capp_ui/fee.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.7/capp_ui/libs.py` & `ctrip-app-ui-0.6.8/capp_ui/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.7/capp_ui/mobile_terminals.py` & `ctrip-app-ui-0.6.8/capp_ui/mobile_terminals.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.7/capp_ui/platforms.py` & `ctrip-app-ui-0.6.8/capp_ui/platforms.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.7/capp_ui/test.py` & `ctrip-app-ui-0.6.8/capp_ui/test.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.7/capp_ui/utils.py` & `ctrip-app-ui-0.6.8/capp_ui/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.7/capp_ui/validators.py` & `ctrip-app-ui-0.6.8/capp_ui/validators.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.7/setup.py` & `ctrip-app-ui-0.6.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-app-ui',
-    version='0.6.7',
+    version='0.6.8',
     description='This is my ctrip app ui package',
     long_description='This is my ctrip app ui package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-app-ui',
     packages=find_packages(),
     install_requires=[
```

