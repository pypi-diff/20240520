# Comparing `tmp/ctrip-app-ui-0.6.8.tar.gz` & `tmp/ctrip-app-ui-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-app-ui-0.6.8.tar", last modified: Mon May 20 06:05:30 2024, max compression
+gzip compressed data, was "ctrip-app-ui-0.6.9.tar", last modified: Mon May 20 07:18:40 2024, max compression
```

## Comparing `ctrip-app-ui-0.6.8.tar` & `ctrip-app-ui-0.6.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 06:05:30.292165 ctrip-app-ui-0.6.8/
--rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.6.8/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-20 06:05:30.291168 ctrip-app-ui-0.6.8/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.6.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 06:05:30.282192 ctrip-app-ui-0.6.8/capp_ui/
--rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.6.8/capp_ui/__init__.py
--rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.6.8/capp_ui/config.py
--rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.6.8/capp_ui/date_extend.py
--rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.6.8/capp_ui/device.py
--rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.6.8/capp_ui/dir.py
--rw-rw-rw-   0        0        0    52611 2024-05-20 06:05:05.000000 ctrip-app-ui-0.6.8/capp_ui/domain_service.py
--rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.6.8/capp_ui/fee.py
--rw-rw-rw-   0        0        0     5414 2024-05-18 14:39:38.000000 ctrip-app-ui-0.6.8/capp_ui/libs.py
--rw-rw-rw-   0        0        0    24821 2024-05-13 17:15:14.000000 ctrip-app-ui-0.6.8/capp_ui/mobile_terminals.py
--rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.6.8/capp_ui/platforms.py
--rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.6.8/capp_ui/test.py
--rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.6.8/capp_ui/utils.py
--rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.6.8/capp_ui/validators.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:05:30.290171 ctrip-app-ui-0.6.8/ctrip_app_ui.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-20 06:05:30.000000 ctrip-app-ui-0.6.8/ctrip_app_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      460 2024-05-20 06:05:30.000000 ctrip-app-ui-0.6.8/ctrip_app_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 06:05:30.000000 ctrip-app-ui-0.6.8/ctrip_app_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-20 06:05:30.000000 ctrip-app-ui-0.6.8/ctrip_app_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-20 06:05:30.000000 ctrip-app-ui-0.6.8/ctrip_app_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 06:05:30.293163 ctrip-app-ui-0.6.8/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-20 06:05:26.000000 ctrip-app-ui-0.6.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:18:40.917072 ctrip-app-ui-0.6.9/
+-rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.6.9/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-20 07:18:40.916086 ctrip-app-ui-0.6.9/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.6.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 07:18:40.905105 ctrip-app-ui-0.6.9/capp_ui/
+-rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.6.9/capp_ui/__init__.py
+-rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.6.9/capp_ui/config.py
+-rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.6.9/capp_ui/date_extend.py
+-rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.6.9/capp_ui/device.py
+-rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.6.9/capp_ui/dir.py
+-rw-rw-rw-   0        0        0    54996 2024-05-20 07:18:22.000000 ctrip-app-ui-0.6.9/capp_ui/domain_service.py
+-rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.6.9/capp_ui/fee.py
+-rw-rw-rw-   0        0        0     5414 2024-05-18 14:39:38.000000 ctrip-app-ui-0.6.9/capp_ui/libs.py
+-rw-rw-rw-   0        0        0    24821 2024-05-13 17:15:14.000000 ctrip-app-ui-0.6.9/capp_ui/mobile_terminals.py
+-rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.6.9/capp_ui/platforms.py
+-rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.6.9/capp_ui/test.py
+-rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.6.9/capp_ui/utils.py
+-rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.6.9/capp_ui/validators.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:18:40.915090 ctrip-app-ui-0.6.9/ctrip_app_ui.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-20 07:18:40.000000 ctrip-app-ui-0.6.9/ctrip_app_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      460 2024-05-20 07:18:40.000000 ctrip-app-ui-0.6.9/ctrip_app_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 07:18:40.000000 ctrip-app-ui-0.6.9/ctrip_app_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-20 07:18:40.000000 ctrip-app-ui-0.6.9/ctrip_app_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-20 07:18:40.000000 ctrip-app-ui-0.6.9/ctrip_app_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 07:18:40.917072 ctrip-app-ui-0.6.9/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-20 07:18:36.000000 ctrip-app-ui-0.6.9/setup.py
```

### Comparing `ctrip-app-ui-0.6.8/LICENSE` & `ctrip-app-ui-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.8/capp_ui/config.py` & `ctrip-app-ui-0.6.9/capp_ui/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.8/capp_ui/date_extend.py` & `ctrip-app-ui-0.6.9/capp_ui/date_extend.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.8/capp_ui/device.py` & `ctrip-app-ui-0.6.9/capp_ui/device.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.8/capp_ui/dir.py` & `ctrip-app-ui-0.6.9/capp_ui/dir.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.8/capp_ui/domain_service.py` & `ctrip-app-ui-0.6.9/capp_ui/domain_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from poco.exceptions import PocoNoSuchNodeException, PocoTargetTimeout
 
 from capp_ui.platforms import PlatformService
 from capp_ui.config import ctrip_soft_keyboard_position
 from capp_ui.mobile_terminals import stop_app, PocoProxy
 from capp_ui.date_extend import is_later_than_current_time
 from capp_ui.dir import get_images_dir, is_exists, join_path
-from capp_ui.libs import SleepWait, LoopFindElementSubmit, logger, LoopFindElementObject
+from capp_ui.libs import SleepWait, LoopFindElementSubmit, logger, LoopFindElementObject, LoopExcute
 
 
 class CtripAppService(object):
     """
     携程APP
     """
     IMAGE_DIR = get_images_dir()
@@ -900,14 +900,68 @@
         return dict()
 
     def __get_wallet_element(self) -> UIObjectProxy:
         return self.device.get_po(
             type="android.widget.TextView", name="android.widget.TextView", textMatches=r'^钱包.*'
         )
 
+    @LoopExcute(action="钱包支付完成，查找是否出现【完成】弹框，或者详情页", sleep=1, loop=20)
+    def get_wallet_payment_success(self) -> bool:
+        try:
+            order_detail_page_1 = self.device.poco(
+                type="android.widget.TextView", name="浮层标题", text="出行前必读"
+            )
+            if order_detail_page_1.exists() is True:
+                return True
+        except (PocoNoSuchNodeException, PocoTargetTimeout, Exception):
+            pass
+        try:
+            order_detail_page_2 = self.device.poco(
+                type="android.widget.TextView", name="header_Text_订单详情", text="订单详情"
+            )
+            if order_detail_page_2.exists() is True:
+                return True
+        except (PocoNoSuchNodeException, PocoTargetTimeout, Exception):
+            pass
+        try:
+            order_detail_page_3 = self.device.poco(
+                type="android.widget.TextView", name="operateBtnList_Text_我要退订", text="我要退订"
+            )
+            if order_detail_page_3.exists() is True:
+                return True
+        except (PocoNoSuchNodeException, PocoTargetTimeout, Exception):
+            pass
+        try:
+            order_detail_page_4 = self.device.poco(
+                type="android.view.ViewGroup", name="CusHeaderView_TouchableOpacity_leftIconWrap",
+                desc="CusHeaderView_TouchableOpacity_leftIconWrap"
+            )
+            if order_detail_page_4.exists() is True:
+                return True
+        except (PocoNoSuchNodeException, PocoTargetTimeout, Exception):
+            pass
+        try:
+            file_name = join_path([get_images_dir(), "钱包支付_完成.png"])
+            if is_exists(file_name):
+                temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
+                pos = self.device.exists(v=temp)
+                if pos:
+                    return True
+        except (Exception,):
+            pass
+        try:
+            payment_success = self.device.get_po(
+                type="android.widget.TextView", name="android.widget.TextView", text="完成"
+            )
+            if payment_success.exists() is True:
+                return True
+        except (Exception,):
+            pass
+        return False
+
     @SleepWait(wait_time=1)
     def is_wallet_usable(self) -> t.Tuple:
         """
         判断收银台界面，钱包支付是否可用，如果可用，还要判断钱包的余额是否够用
         """
         flag = False
         amount = 0.00
```

### Comparing `ctrip-app-ui-0.6.8/capp_ui/fee.py` & `ctrip-app-ui-0.6.9/capp_ui/fee.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.8/capp_ui/libs.py` & `ctrip-app-ui-0.6.9/capp_ui/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.8/capp_ui/mobile_terminals.py` & `ctrip-app-ui-0.6.9/capp_ui/mobile_terminals.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.8/capp_ui/platforms.py` & `ctrip-app-ui-0.6.9/capp_ui/platforms.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.8/capp_ui/test.py` & `ctrip-app-ui-0.6.9/capp_ui/test.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.8/capp_ui/utils.py` & `ctrip-app-ui-0.6.9/capp_ui/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.8/capp_ui/validators.py` & `ctrip-app-ui-0.6.9/capp_ui/validators.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.8/setup.py` & `ctrip-app-ui-0.6.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-app-ui',
-    version='0.6.8',
+    version='0.6.9',
     description='This is my ctrip app ui package',
     long_description='This is my ctrip app ui package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-app-ui',
     packages=find_packages(),
     install_requires=[
```

