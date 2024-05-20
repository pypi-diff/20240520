# Comparing `tmp/ctrip-app-ui-0.7.0.tar.gz` & `tmp/ctrip-app-ui-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-app-ui-0.7.0.tar", last modified: Mon May 20 07:33:48 2024, max compression
+gzip compressed data, was "ctrip-app-ui-0.7.1.tar", last modified: Mon May 20 12:06:13 2024, max compression
```

## Comparing `ctrip-app-ui-0.7.0.tar` & `ctrip-app-ui-0.7.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 07:33:48.505228 ctrip-app-ui-0.7.0/
--rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.7.0/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-20 07:33:48.503221 ctrip-app-ui-0.7.0/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.7.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 07:33:48.491252 ctrip-app-ui-0.7.0/capp_ui/
--rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.7.0/capp_ui/__init__.py
--rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.7.0/capp_ui/config.py
--rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.7.0/capp_ui/date_extend.py
--rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.7.0/capp_ui/device.py
--rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.7.0/capp_ui/dir.py
--rw-rw-rw-   0        0        0    54975 2024-05-20 07:33:35.000000 ctrip-app-ui-0.7.0/capp_ui/domain_service.py
--rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.7.0/capp_ui/fee.py
--rw-rw-rw-   0        0        0     5414 2024-05-18 14:39:38.000000 ctrip-app-ui-0.7.0/capp_ui/libs.py
--rw-rw-rw-   0        0        0    24821 2024-05-13 17:15:14.000000 ctrip-app-ui-0.7.0/capp_ui/mobile_terminals.py
--rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.7.0/capp_ui/platforms.py
--rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.7.0/capp_ui/test.py
--rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.7.0/capp_ui/utils.py
--rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.7.0/capp_ui/validators.py
-drwxrwxrwx   0        0        0        0 2024-05-20 07:33:48.502224 ctrip-app-ui-0.7.0/ctrip_app_ui.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-20 07:33:48.000000 ctrip-app-ui-0.7.0/ctrip_app_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      460 2024-05-20 07:33:48.000000 ctrip-app-ui-0.7.0/ctrip_app_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 07:33:48.000000 ctrip-app-ui-0.7.0/ctrip_app_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-20 07:33:48.000000 ctrip-app-ui-0.7.0/ctrip_app_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-20 07:33:48.000000 ctrip-app-ui-0.7.0/ctrip_app_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 07:33:48.505228 ctrip-app-ui-0.7.0/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-20 07:33:43.000000 ctrip-app-ui-0.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 12:06:13.295555 ctrip-app-ui-0.7.1/
+-rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.7.1/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-20 12:06:13.293561 ctrip-app-ui-0.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.7.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 12:06:13.282591 ctrip-app-ui-0.7.1/capp_ui/
+-rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.7.1/capp_ui/__init__.py
+-rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.7.1/capp_ui/config.py
+-rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.7.1/capp_ui/date_extend.py
+-rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.7.1/capp_ui/device.py
+-rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.7.1/capp_ui/dir.py
+-rw-rw-rw-   0        0        0    55970 2024-05-20 12:05:57.000000 ctrip-app-ui-0.7.1/capp_ui/domain_service.py
+-rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.7.1/capp_ui/fee.py
+-rw-rw-rw-   0        0        0     5414 2024-05-18 14:39:38.000000 ctrip-app-ui-0.7.1/capp_ui/libs.py
+-rw-rw-rw-   0        0        0    24821 2024-05-13 17:15:14.000000 ctrip-app-ui-0.7.1/capp_ui/mobile_terminals.py
+-rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.7.1/capp_ui/platforms.py
+-rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.7.1/capp_ui/test.py
+-rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.7.1/capp_ui/utils.py
+-rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.7.1/capp_ui/validators.py
+drwxrwxrwx   0        0        0        0 2024-05-20 12:06:13.292564 ctrip-app-ui-0.7.1/ctrip_app_ui.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-20 12:06:13.000000 ctrip-app-ui-0.7.1/ctrip_app_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      460 2024-05-20 12:06:13.000000 ctrip-app-ui-0.7.1/ctrip_app_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 12:06:13.000000 ctrip-app-ui-0.7.1/ctrip_app_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-20 12:06:13.000000 ctrip-app-ui-0.7.1/ctrip_app_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-20 12:06:13.000000 ctrip-app-ui-0.7.1/ctrip_app_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 12:06:13.295555 ctrip-app-ui-0.7.1/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-20 12:06:07.000000 ctrip-app-ui-0.7.1/setup.py
```

### Comparing `ctrip-app-ui-0.7.0/LICENSE` & `ctrip-app-ui-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.0/capp_ui/config.py` & `ctrip-app-ui-0.7.1/capp_ui/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.0/capp_ui/date_extend.py` & `ctrip-app-ui-0.7.1/capp_ui/date_extend.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.0/capp_ui/device.py` & `ctrip-app-ui-0.7.1/capp_ui/device.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.0/capp_ui/dir.py` & `ctrip-app-ui-0.7.1/capp_ui/dir.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.0/capp_ui/domain_service.py` & `ctrip-app-ui-0.7.1/capp_ui/domain_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -507,15 +507,15 @@
             if cancel_order.exists() is True:
                 return {"element": cancel_order}
         except (Exception,):
             pass
         return dict()
 
     @LoopFindElementObject(action="取消订单确认小弹框查找【取消订单】按钮", loop=20, sleep=1)
-    def get_submit_cancel_order(self):
+    def get_submit_cancel_order(self) -> dict:
         try:
             file_name = join_path([get_images_dir(), "取消订单弹框_取消订单.png"])
             if is_exists(file_name):
                 temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
                 pos = self.device.exists(v=temp)
                 if pos:
                     return {"pos": pos}
@@ -1214,7 +1214,30 @@
             payment_amount = payment_amount.get_text()
             logger.info("从支付成功界面获取到的实际支付金额是: {}".format(payment_amount))
             payment_amount = Decimal(payment_amount) if payment_amount and isinstance(
                 payment_amount, str) else Decimal(-9999999999.9999999999)
         except Exception as e:
             logger.error(str(e))
         return payment_amount
+
+    @LoopFindElementObject(action="取消订单确认小弹框查找【再想想】按钮", loop=20, sleep=1)
+    def get_submit_think_again(self) -> dict:
+        try:
+            file_name = join_path([get_images_dir(), "取消订单弹框_再想想.png"])
+            if is_exists(file_name):
+                temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
+                pos = self.device.exists(v=temp)
+                if pos:
+                    return {"pos": pos}
+            else:
+                logger.warning("文件{}，没找到".format(file_name))
+        except (Exception,):
+            pass
+        try:
+            cancel_order = self.device.poco(
+                type="android.widget.TextView", name="Button_Text_再想想", text="再想想"
+            )
+            if cancel_order.exists() is True:
+                return {"element": cancel_order}
+        except (Exception,):
+            pass
+        return dict()
```

### Comparing `ctrip-app-ui-0.7.0/capp_ui/fee.py` & `ctrip-app-ui-0.7.1/capp_ui/fee.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.0/capp_ui/libs.py` & `ctrip-app-ui-0.7.1/capp_ui/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.0/capp_ui/mobile_terminals.py` & `ctrip-app-ui-0.7.1/capp_ui/mobile_terminals.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.0/capp_ui/platforms.py` & `ctrip-app-ui-0.7.1/capp_ui/platforms.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.0/capp_ui/test.py` & `ctrip-app-ui-0.7.1/capp_ui/test.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.0/capp_ui/utils.py` & `ctrip-app-ui-0.7.1/capp_ui/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.0/capp_ui/validators.py` & `ctrip-app-ui-0.7.1/capp_ui/validators.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.7.0/setup.py` & `ctrip-app-ui-0.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-app-ui',
-    version='0.7.0',
+    version='0.7.1',
     description='This is my ctrip app ui package',
     long_description='This is my ctrip app ui package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-app-ui',
     packages=find_packages(),
     install_requires=[
```

