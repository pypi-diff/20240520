# Comparing `tmp/printwizard-0.1.2.tar.gz` & `tmp/printwizard-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "printwizard-0.1.2.tar", last modified: Sun Oct 15 11:08:05 2023, max compression
+gzip compressed data, was "printwizard-1.0.0.tar", last modified: Sun May 19 16:17:21 2024, max compression
```

## Comparing `printwizard-0.1.2.tar` & `printwizard-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 neon      (1000) neon      (1000)        0 2023-10-15 11:08:05.299867 printwizard-0.1.2/
--rw-r--r--   0 neon      (1000) neon      (1000)     1068 2023-10-14 15:35:53.000000 printwizard-0.1.2/LICENSE
--rw-r--r--   0 neon      (1000) neon      (1000)     1391 2023-10-15 11:08:05.299867 printwizard-0.1.2/PKG-INFO
--rw-r--r--   0 neon      (1000) neon      (1000)      775 2023-10-14 15:33:13.000000 printwizard-0.1.2/README.md
--rw-r--r--   0 neon      (1000) neon      (1000)      691 2023-10-15 11:07:49.000000 printwizard-0.1.2/pyproject.toml
--rw-r--r--   0 neon      (1000) neon      (1000)       38 2023-10-15 11:08:05.299867 printwizard-0.1.2/setup.cfg
-drwxr-xr-x   0 neon      (1000) neon      (1000)        0 2023-10-15 11:08:05.299867 printwizard-0.1.2/src/
-drwxr-xr-x   0 neon      (1000) neon      (1000)        0 2023-10-15 11:08:05.299867 printwizard-0.1.2/src/printwizard/
--rw-r--r--   0 neon      (1000) neon      (1000)       76 2023-10-14 15:41:46.000000 printwizard-0.1.2/src/printwizard/__init__.py
--rw-r--r--   0 neon      (1000) neon      (1000)     4316 2023-10-15 11:06:23.000000 printwizard-0.1.2/src/printwizard/logger.py
--rw-r--r--   0 neon      (1000) neon      (1000)      629 2023-10-15 10:27:32.000000 printwizard-0.1.2/src/printwizard/set_wizard_config.py
-drwxr-xr-x   0 neon      (1000) neon      (1000)        0 2023-10-15 11:08:05.299867 printwizard-0.1.2/src/printwizard.egg-info/
--rw-r--r--   0 neon      (1000) neon      (1000)     1391 2023-10-15 11:08:05.000000 printwizard-0.1.2/src/printwizard.egg-info/PKG-INFO
--rw-r--r--   0 neon      (1000) neon      (1000)      279 2023-10-15 11:08:05.000000 printwizard-0.1.2/src/printwizard.egg-info/SOURCES.txt
--rw-r--r--   0 neon      (1000) neon      (1000)        1 2023-10-15 11:08:05.000000 printwizard-0.1.2/src/printwizard.egg-info/dependency_links.txt
--rw-r--r--   0 neon      (1000) neon      (1000)       12 2023-10-15 11:08:05.000000 printwizard-0.1.2/src/printwizard.egg-info/top_level.txt
+drwxr-xr-x   0 neon      (1000) neon      (1000)        0 2024-05-19 16:17:21.871969 printwizard-1.0.0/
+-rw-r--r--   0 neon      (1000) neon      (1000)     1068 2023-10-14 15:35:53.000000 printwizard-1.0.0/LICENSE
+-rw-r--r--   0 neon      (1000) neon      (1000)     1192 2024-05-19 16:17:21.871969 printwizard-1.0.0/PKG-INFO
+-rw-r--r--   0 neon      (1000) neon      (1000)      775 2023-10-14 15:33:13.000000 printwizard-1.0.0/README.md
+drwxr-xr-x   0 neon      (1000) neon      (1000)        0 2024-05-19 16:17:21.868635 printwizard-1.0.0/printwizard/
+-rw-r--r--   0 neon      (1000) neon      (1000)       98 2024-05-19 15:38:21.000000 printwizard-1.0.0/printwizard/__init__.py
+-rw-r--r--   0 neon      (1000) neon      (1000)     4910 2024-05-19 16:11:10.000000 printwizard-1.0.0/printwizard/logger.py
+-rw-r--r--   0 neon      (1000) neon      (1000)      629 2024-05-19 15:43:28.000000 printwizard-1.0.0/printwizard/set_wizard_config.py
+drwxr-xr-x   0 neon      (1000) neon      (1000)        0 2024-05-19 16:17:21.871969 printwizard-1.0.0/printwizard.egg-info/
+-rw-r--r--   0 neon      (1000) neon      (1000)     1192 2024-05-19 16:17:21.000000 printwizard-1.0.0/printwizard.egg-info/PKG-INFO
+-rw-r--r--   0 neon      (1000) neon      (1000)      284 2024-05-19 16:17:21.000000 printwizard-1.0.0/printwizard.egg-info/SOURCES.txt
+-rw-r--r--   0 neon      (1000) neon      (1000)        1 2024-05-19 16:17:21.000000 printwizard-1.0.0/printwizard.egg-info/dependency_links.txt
+-rw-r--r--   0 neon      (1000) neon      (1000)       18 2024-05-19 16:17:21.000000 printwizard-1.0.0/printwizard.egg-info/top_level.txt
+-rw-r--r--   0 neon      (1000) neon      (1000)       38 2024-05-19 16:17:21.871969 printwizard-1.0.0/setup.cfg
+-rw-r--r--   0 neon      (1000) neon      (1000)      613 2024-05-19 16:14:59.000000 printwizard-1.0.0/setup.py
+drwxr-xr-x   0 neon      (1000) neon      (1000)        0 2024-05-19 16:17:21.871969 printwizard-1.0.0/tests/
+-rw-r--r--   0 neon      (1000) neon      (1000)        0 2024-05-19 15:05:01.000000 printwizard-1.0.0/tests/__init__.py
+-rw-r--r--   0 neon      (1000) neon      (1000)      204 2024-05-19 16:11:26.000000 printwizard-1.0.0/tests/test_logger.py
```

### Comparing `printwizard-0.1.2/LICENSE` & `printwizard-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `printwizard-0.1.2/PKG-INFO` & `printwizard-1.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: printwizard
-Version: 0.1.2
-Summary: A minimal yet colorful alternative to the print() function in Python, with methods like success(), warn(), info() and error()
-Author-email: GoodBoyNeon <contact@neon.is-a.dev>
-Project-URL: Homepage, https://github.com/goodboyneon/print-wizard
-Project-URL: Bug Tracker, https://github.com/goodboyneon/print-wizard/issues
+Version: 1.0.0
+Summary: A minimal logger to make your print statements beautiful and functional
+Author: GoodBoyNeon (Sushant Ray)
+Author-email: <contact@neon.is-a.dev>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
 	<br />
 	<p>
     <h1 align="center">🌈 Print Wizard</h1>
```

#### html2text {}

```diff
@@ -1,16 +1,13 @@
-Metadata-Version: 2.1 Name: printwizard Version: 0.1.2 Summary: A minimal yet
-colorful alternative to the print() function in Python, with methods like
-success(), warn(), info() and error() Author-email: GoodBoyNeon
-neon.is-a.dev> Project-URL: Homepage, https://github.com/goodboyneon/print-
-wizard Project-URL: Bug Tracker, https://github.com/goodboyneon/print-wizard/
-issues Classifier: Programming Language :: Python :: 3 Classifier: License ::
-OSI Approved :: MIT License Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
-LICENSE
+Metadata-Version: 2.1 Name: printwizard Version: 1.0.0 Summary: A minimal
+logger to make your print statements beautiful and functional Author:
+GoodBoyNeon (Sushant Ray) Author-email:
+neon.is-a.dev> Classifier: Programming Language :: Python :: 3 Classifier:
+License :: OSI Approved :: MIT License Classifier: Operating System :: OS
+Independent Description-Content-Type: text/markdown License-File: LICENSE
 
                         ************ ?ð??? PPrriinntt WWiizzaarrdd ************
 ** ?ð??? AA mmiinniimmaall yyeett ccoolloorrffuull aanndd ccuussttoommiizzaabbllee aalltteerrnnaattiivvee ttoo ppyytthhoonn''ss ddeeffaauulltt
                                    llooggggeerr.. **
 
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_i_s_s_u_e_s_/_G_o_o_d_B_o_y_N_e_o_n_/_c_o_n_s_o_l_e_-_w_i_z_a_r_d_?_s_t_y_l_e_=_f_l_a_t_-
 _s_q_u_a_r_e_&_l_o_g_o_=_g_i_t_h_u_b_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_i_s_s_u_e_s_-_p_r_/_G_o_o_d_B_o_y_N_e_o_n_/
```

### Comparing `printwizard-0.1.2/README.md` & `printwizard-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `printwizard-0.1.2/src/printwizard/logger.py` & `printwizard-1.0.0/printwizard/logger.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from .set_wizard_config import user_config
 from datetime import datetime
 
 style_wrapper = {
     "reset": "\x1b[0m",
     # This lightens the color as a side-effect
     "bold": "\x1b[1m",
     "dim": "\x1b[2m",
@@ -28,26 +27,46 @@
     "bg_blue": "\x1b[44m",
     "bg_magenta": "\x1b[45m",
     "bg_cyan": "\x1b[46m",
     "bg_white": "\x1b[47m",
     "bg_gray": "\x1b[100m",
 }
 
+default_config = {
+    "include_timestamp": True,
+    "include_status": True,
+    "include_sn": True,
+    "table_border": {
+        "corner_tl": "┌",
+        "corner_tr": "┐",
+        "corner_bl": "└",
+        "corner_br": "┘",
+        "edge_vertical": "│",
+        "edge_horizontal": "─",
+        "intersection_tlr": "┴",
+        "intersection_blr": "┬",
+        "intersection_tbl": "├",
+        "intersection_tbr": "┤",
+        "intersection_center": "┼",
+    },
+}
+
 
 class Helpers:
     @staticmethod
     def get_timestamp():
         return datetime.now().strftime("%m/%d/%Y %H:%M:%S")
 
     @staticmethod
-    def get_config(override=None):
+    def get_config(user_config: dict, override=None):
         if override:
-            return {**user_config, **override}
+            return {**default_config, **user_config, **override}
+
         else:
-            return user_config
+            return {**default_config, **user_config}
 
     @staticmethod
     def get_logging_args(config: dict, options: dict):
         status_text = {
             "error": "ERROR ",
             "warn": "WARN ",
             "info": "INFO ",
@@ -92,18 +111,21 @@
         return args
 
 
 timestamp = f"[{Helpers.get_timestamp()}]"
 
 
 class Logger:
-    @staticmethod
-    def success(msg: str, config_override=None) -> str:
+
+    def __init__(self, config: dict = default_config):
+        self.config = config
+
+    def success(self, msg: str, config_override=None) -> str:
         status_type = "success"
-        config = Helpers.get_config(config_override)
+        config = Helpers.get_config(self.config, config_override)
         args_list = Helpers.get_logging_args(
             config,
             {
                 "status_type": status_type,
                 "msg": msg,
                 "timestamp": timestamp,
             },
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `printwizard-0.1.2/src/printwizard/set_wizard_config.py` & `printwizard-1.0.0/printwizard/set_wizard_config.py`

 * *Files identical despite different names*

### Comparing `printwizard-0.1.2/src/printwizard.egg-info/PKG-INFO` & `printwizard-1.0.0/printwizard.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: printwizard
-Version: 0.1.2
-Summary: A minimal yet colorful alternative to the print() function in Python, with methods like success(), warn(), info() and error()
-Author-email: GoodBoyNeon <contact@neon.is-a.dev>
-Project-URL: Homepage, https://github.com/goodboyneon/print-wizard
-Project-URL: Bug Tracker, https://github.com/goodboyneon/print-wizard/issues
+Version: 1.0.0
+Summary: A minimal logger to make your print statements beautiful and functional
+Author: GoodBoyNeon (Sushant Ray)
+Author-email: <contact@neon.is-a.dev>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
 	<br />
 	<p>
     <h1 align="center">🌈 Print Wizard</h1>
```

#### html2text {}

```diff
@@ -1,16 +1,13 @@
-Metadata-Version: 2.1 Name: printwizard Version: 0.1.2 Summary: A minimal yet
-colorful alternative to the print() function in Python, with methods like
-success(), warn(), info() and error() Author-email: GoodBoyNeon
-neon.is-a.dev> Project-URL: Homepage, https://github.com/goodboyneon/print-
-wizard Project-URL: Bug Tracker, https://github.com/goodboyneon/print-wizard/
-issues Classifier: Programming Language :: Python :: 3 Classifier: License ::
-OSI Approved :: MIT License Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
-LICENSE
+Metadata-Version: 2.1 Name: printwizard Version: 1.0.0 Summary: A minimal
+logger to make your print statements beautiful and functional Author:
+GoodBoyNeon (Sushant Ray) Author-email:
+neon.is-a.dev> Classifier: Programming Language :: Python :: 3 Classifier:
+License :: OSI Approved :: MIT License Classifier: Operating System :: OS
+Independent Description-Content-Type: text/markdown License-File: LICENSE
 
                         ************ ?ð??? PPrriinntt WWiizzaarrdd ************
 ** ?ð??? AA mmiinniimmaall yyeett ccoolloorrffuull aanndd ccuussttoommiizzaabbllee aalltteerrnnaattiivvee ttoo ppyytthhoonn''ss ddeeffaauulltt
                                    llooggggeerr.. **
 
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_i_s_s_u_e_s_/_G_o_o_d_B_o_y_N_e_o_n_/_c_o_n_s_o_l_e_-_w_i_z_a_r_d_?_s_t_y_l_e_=_f_l_a_t_-
 _s_q_u_a_r_e_&_l_o_g_o_=_g_i_t_h_u_b_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_i_s_s_u_e_s_-_p_r_/_G_o_o_d_B_o_y_N_e_o_n_/
```

