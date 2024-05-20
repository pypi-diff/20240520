# Comparing `tmp/ctrip-app-ui-0.6.4.tar.gz` & `tmp/ctrip-app-ui-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-app-ui-0.6.4.tar", last modified: Sun May 19 10:55:51 2024, max compression
+gzip compressed data, was "ctrip-app-ui-0.6.5.tar", last modified: Sun May 19 11:05:12 2024, max compression
```

## Comparing `ctrip-app-ui-0.6.4.tar` & `ctrip-app-ui-0.6.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 10:55:51.527949 ctrip-app-ui-0.6.4/
--rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.6.4/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-19 10:55:51.526951 ctrip-app-ui-0.6.4/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.6.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-19 10:55:51.500051 ctrip-app-ui-0.6.4/capp_ui/
--rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.6.4/capp_ui/__init__.py
--rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.6.4/capp_ui/config.py
--rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.6.4/capp_ui/date_extend.py
--rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.6.4/capp_ui/device.py
--rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.6.4/capp_ui/dir.py
--rw-rw-rw-   0        0        0    52875 2024-05-19 10:50:18.000000 ctrip-app-ui-0.6.4/capp_ui/domain_service.py
--rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.6.4/capp_ui/fee.py
--rw-rw-rw-   0        0        0     5414 2024-05-18 14:39:38.000000 ctrip-app-ui-0.6.4/capp_ui/libs.py
--rw-rw-rw-   0        0        0    24821 2024-05-13 17:15:14.000000 ctrip-app-ui-0.6.4/capp_ui/mobile_terminals.py
--rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.6.4/capp_ui/platforms.py
--rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.6.4/capp_ui/test.py
--rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.6.4/capp_ui/utils.py
--rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.6.4/capp_ui/validators.py
-drwxrwxrwx   0        0        0        0 2024-05-19 10:55:51.524957 ctrip-app-ui-0.6.4/ctrip_app_ui.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-19 10:55:51.000000 ctrip-app-ui-0.6.4/ctrip_app_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      460 2024-05-19 10:55:51.000000 ctrip-app-ui-0.6.4/ctrip_app_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 10:55:51.000000 ctrip-app-ui-0.6.4/ctrip_app_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-19 10:55:51.000000 ctrip-app-ui-0.6.4/ctrip_app_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-19 10:55:51.000000 ctrip-app-ui-0.6.4/ctrip_app_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-19 10:55:51.527949 ctrip-app-ui-0.6.4/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-19 10:55:46.000000 ctrip-app-ui-0.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 11:05:12.055620 ctrip-app-ui-0.6.5/
+-rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.6.5/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-19 11:05:12.053625 ctrip-app-ui-0.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.6.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 11:05:12.025700 ctrip-app-ui-0.6.5/capp_ui/
+-rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.6.5/capp_ui/__init__.py
+-rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.6.5/capp_ui/config.py
+-rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.6.5/capp_ui/date_extend.py
+-rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.6.5/capp_ui/device.py
+-rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.6.5/capp_ui/dir.py
+-rw-rw-rw-   0        0        0    52999 2024-05-19 11:04:54.000000 ctrip-app-ui-0.6.5/capp_ui/domain_service.py
+-rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.6.5/capp_ui/fee.py
+-rw-rw-rw-   0        0        0     5414 2024-05-18 14:39:38.000000 ctrip-app-ui-0.6.5/capp_ui/libs.py
+-rw-rw-rw-   0        0        0    24821 2024-05-13 17:15:14.000000 ctrip-app-ui-0.6.5/capp_ui/mobile_terminals.py
+-rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.6.5/capp_ui/platforms.py
+-rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.6.5/capp_ui/test.py
+-rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.6.5/capp_ui/utils.py
+-rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.6.5/capp_ui/validators.py
+drwxrwxrwx   0        0        0        0 2024-05-19 11:05:12.052628 ctrip-app-ui-0.6.5/ctrip_app_ui.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-19 11:05:11.000000 ctrip-app-ui-0.6.5/ctrip_app_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      460 2024-05-19 11:05:11.000000 ctrip-app-ui-0.6.5/ctrip_app_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 11:05:11.000000 ctrip-app-ui-0.6.5/ctrip_app_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-19 11:05:11.000000 ctrip-app-ui-0.6.5/ctrip_app_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-19 11:05:11.000000 ctrip-app-ui-0.6.5/ctrip_app_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 11:05:12.055620 ctrip-app-ui-0.6.5/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-19 11:05:10.000000 ctrip-app-ui-0.6.5/setup.py
```

### Comparing `ctrip-app-ui-0.6.4/LICENSE` & `ctrip-app-ui-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.4/capp_ui/config.py` & `ctrip-app-ui-0.6.5/capp_ui/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.4/capp_ui/date_extend.py` & `ctrip-app-ui-0.6.5/capp_ui/date_extend.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.4/capp_ui/device.py` & `ctrip-app-ui-0.6.5/capp_ui/device.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.4/capp_ui/dir.py` & `ctrip-app-ui-0.6.5/capp_ui/dir.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.4/capp_ui/domain_service.py` & `ctrip-app-ui-0.6.5/capp_ui/domain_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1139,37 +1139,40 @@
             if limit_quotas.exists():
                 # logger.warning("银行卡支付成功，等待出票.")
                 flag = True
         except (PocoNoSuchNodeException, Exception):
             logger.warning("银行卡支付有异常，需要更新支付类型，重新支付.")
         return flag
 
-    @SleepWait(wait_time=1)
     def get_order_with_payment_amount(self) -> Decimal:
         """获取支付成功后的订单金额"""
-        payment_amount = -9999999999.9999999999
+        payment_amount = Decimal(-9999999999.9999999999)
         try:
             payment_amount = self.device.get_po_extend(
                 type="android.widget.TextView",
                 name="android.widget.TextView",
                 textMatches_inner=r"^\d+.\d*",
                 global_num=0,
                 local_num=5,
                 touchable=False,
             )[0]
             payment_amount = payment_amount.get_text()
             logger.info("从支付成功界面获取到的实际支付金额是: {}".format(payment_amount))
-            payment_amount = Decimal(payment_amount) if isinstance(payment_amount, str) else payment_amount
+            payment_amount = Decimal(payment_amount) if payment_amount and isinstance(
+                payment_amount, str) else Decimal(-9999999999.9999999999)
         except Exception as e:
             logger.error(str(e))
         return payment_amount
 
     @LoopFindElementSubmit(loop=3, action="支付完成")
     def touch_payment_complete(self):
         """在支付成功界面，点击【完成】"""
-        payment_complete_button = self.device.poco(
-            type="android.widget.TextView",
-            name="android.widget.TextView",
-            text="完成"
-        )
-        payment_complete_button.click()
-        logger.warning("点击支付成功界面的【完成】按钮.")
+        try:
+            payment_complete_button = self.device.poco(
+                type="android.widget.TextView",
+                name="android.widget.TextView",
+                text="完成"
+            )
+            payment_complete_button.click()
+            logger.warning("点击支付成功界面的【完成】按钮.")
+        except (Exception,):
+            pass
```

### Comparing `ctrip-app-ui-0.6.4/capp_ui/fee.py` & `ctrip-app-ui-0.6.5/capp_ui/fee.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.4/capp_ui/libs.py` & `ctrip-app-ui-0.6.5/capp_ui/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.4/capp_ui/mobile_terminals.py` & `ctrip-app-ui-0.6.5/capp_ui/mobile_terminals.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.4/capp_ui/platforms.py` & `ctrip-app-ui-0.6.5/capp_ui/platforms.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.4/capp_ui/test.py` & `ctrip-app-ui-0.6.5/capp_ui/test.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.4/capp_ui/utils.py` & `ctrip-app-ui-0.6.5/capp_ui/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.4/capp_ui/validators.py` & `ctrip-app-ui-0.6.5/capp_ui/validators.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.4/setup.py` & `ctrip-app-ui-0.6.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-app-ui',
-    version='0.6.4',
+    version='0.6.5',
     description='This is my ctrip app ui package',
     long_description='This is my ctrip app ui package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-app-ui',
     packages=find_packages(),
     install_requires=[
```

