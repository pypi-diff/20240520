# Comparing `tmp/qctrl_qua-0.4.1.tar.gz` & `tmp/qctrl_qua-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qctrl_qua-0.4.1.tar", max compression
+gzip compressed data, was "qctrl_qua-0.5.0.tar", max compression
```

## Comparing `qctrl_qua-0.4.1.tar` & `qctrl_qua-0.5.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    36653 2023-09-18 06:44:08.861829 qctrl_qua-0.4.1/LICENSE
--rw-r--r--   0        0        0      349 2023-09-18 06:44:08.861829 qctrl_qua-0.4.1/README.md
--rw-r--r--   0        0        0     2731 2023-09-18 06:44:31.530053 qctrl_qua-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      818 2023-09-18 06:44:31.538053 qctrl_qua-0.4.1/qctrlqua/__init__.py
--rw-r--r--   0        0        0     3978 2023-09-18 06:44:08.861829 qctrl_qua-0.4.1/qctrlqua/qua_config_gen.py
--rw-r--r--   0        0        0     2387 1970-01-01 00:00:00.000000 qctrl_qua-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    36587 2024-05-19 22:55:30.280188 qctrl_qua-0.5.0/LICENSE
+-rw-r--r--   0        0        0      164 2024-05-19 22:55:30.280188 qctrl_qua-0.5.0/README.md
+-rw-r--r--   0        0        0     2750 2024-05-19 22:55:54.480268 qctrl_qua-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      818 2024-05-19 22:55:54.484268 qctrl_qua-0.5.0/qctrlqua/__init__.py
+-rw-r--r--   0        0        0     3978 2024-05-19 22:55:30.284188 qctrl_qua-0.5.0/qctrlqua/qua_config_gen.py
+-rw-r--r--   0        0        0     2151 1970-01-01 00:00:00.000000 qctrl_qua-0.5.0/PKG-INFO
```

### Comparing `qctrl_qua-0.4.1/LICENSE` & `qctrl_qua-0.5.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
                             Q-CTRL Terms of service
-                            Updated August 8, 2022
+                            Updated November 8, 2023
                             https://q-ctrl.com/terms
 
 BY ACCEPTING THESE TERMS OF SERVICE YOU ARE ENTERING INTO A BINDING AGREEMENT
 THAT APPLIES TO ANY USE OF THE PLATFORM. WE HAVE ENDEAVORED TO MAKE THE TERMS
 SIMPLE AND CLEAR. YOU ACKNOWLEDGE THAT YOU HAVE READ AND UNDERSTOOD THIS
 AGREEMENT, AND REPRESENT THAT YOU HAVE THE AUTHORITY TO ENTER INTO THIS
 AGREEMENT ON BEHALF OF ANY ORGANIZATION OR PERSON FOR WHOM YOU ARE USING THE
@@ -106,17 +106,16 @@
 
 "Platform" shall mean the software made available by us from time to time via
 the access method, as may be changed or updated from time to time by us. The
 features of the platform available to you will depend on the plan you have
 subscribed to and whether the platform is hosted by us, hosted on-premises, or
 installed locally.
 
-"Q-CTRL" shall mean Q-CTRL Pty Ltd (ABN 78 622 325 535) of ℅ Scendar, Suite 1,
-Level 18, 219-227 Elizabeth Street, SYDNEY NSW 2000, Australia (also referred to
-as "we", "us" or "our").
+"Q-CTRL" shall mean Q-CTRL Pty Ltd (ABN 78 622 325 535) - Sydney, Australia
+(also referred to as "we", "us" or "our").
 
 "Subscriber" shall mean the person who registers to use the platform and, where
 the context permits, includes any entity on whose behalf that person registers
 to use the platform.
 
 "Support" shall mean the support services offered to you by us, the nature and
 extent of such are determined by your plan.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `qctrl_qua-0.4.1/pyproject.toml` & `qctrl_qua-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 [tool.poetry]
 name = "qctrl-qua"
-version = "0.4.1"
+version = "0.5.0"
 description = "Q-CTRL QUA Adapter"
 license = "https://q-ctrl.com/terms"
 authors = ["Q-CTRL <support@q-ctrl.com>"]
 maintainers = ["Q-CTRL <support@q-ctrl.com>"]
 readme = "README.md"
 homepage = "https://q-ctrl.com"
-repository = ""
 documentation = "https://docs.q-ctrl.com/boulder-opal/references/qctrl-qua/"
 keywords = [
     "black opal",
     "boulder opal",
     "fire opal",
     "nisq",
     "open controls",
@@ -59,26 +58,27 @@
 packages = [
     { include = "qctrlqua" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.12"
 numpy = "^1.23.5"
-qctrl-sphinx-theme = "^2.1.1"
 
 [tool.poetry.dev-dependencies]
-black = "^23.3.0"
+black = "^24.3.0"
 isort = "^5.12.0"
 mypy = "^1.2.0"
 pylint = "^2.17.1"
 pytest = "^7.3.1"
 pre-commit = "^3.2.2"
-qualang_tools = "~0.14.0"
+qualang_tools = "~0.16.0"
+qctrl-sphinx-theme = "^2.1.4"
 sphinx = "^5.3.0"
 tomli = "^2.0.1"
+sphinx-markdown-builder = "^0.6.6"
 
 [[tool.poetry.source]]
 name = "PyPI"
 priority = "supplemental"
 
 [[tool.poetry.source]]
 name = "Q-CTRL PyPI"
```

### Comparing `qctrl_qua-0.4.1/qctrlqua/__init__.py` & `qctrl_qua-0.5.0/qctrlqua/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 Q-CTRL. All rights reserved.
+# Copyright 2024 Q-CTRL. All rights reserved.
 #
 # Licensed under the Q-CTRL Terms of service (the "License"). Unauthorized
 # copying or use of this file, via any medium, is strictly prohibited.
 # Proprietary and confidential. You may not use this file except in compliance
 # with the License. You may obtain a copy of the License at
 #
 #    https://q-ctrl.com/terms
@@ -13,12 +13,12 @@
 
 """
 The Q-CTRL QUA Adapter package allows you to integrate Boulder Opal with the QUA
 quantum computing language.
 """
 
 __author__ = "Q-CTRL <support@q-ctrl.com>"
-__version__ = "0.4.1"
+__version__ = "0.5.0"
 
 from .qua_config_gen import add_pulse_to_config
 
 __all__ = ["add_pulse_to_config"]
```

### Comparing `qctrl_qua-0.4.1/qctrlqua/qua_config_gen.py` & `qctrl_qua-0.5.0/qctrlqua/qua_config_gen.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 Q-CTRL. All rights reserved.
+# Copyright 2024 Q-CTRL. All rights reserved.
 #
 # Licensed under the Q-CTRL Terms of service (the "License"). Unauthorized
 # copying or use of this file, via any medium, is strictly prohibited.
 # Proprietary and confidential. You may not use this file except in compliance
 # with the License. You may obtain a copy of the License at
 #
 #    https://q-ctrl.com/terms
```

### Comparing `qctrl_qua-0.4.1/PKG-INFO` & `qctrl_qua-0.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qctrl-qua
-Version: 0.4.1
+Version: 0.5.0
 Summary: Q-CTRL QUA Adapter
 Home-page: https://q-ctrl.com
 License: https://q-ctrl.com/terms
 Keywords: black opal,boulder opal,fire opal,nisq,open controls,q control,q ctrl,q-control,q-ctrl,qcontrol,qctrl,quantum,quantum algorithms,quantum circuits,quantum coding,quantum coding software,quantum computing,quantum control,quantum control software,quantum control theory,quantum engineering,quantum error correction,quantum firmware,quantum fundamentals,quantum sensing,qubit,qudit
 Author: Q-CTRL
 Author-email: support@q-ctrl.com
 Maintainer: Q-CTRL
@@ -25,22 +25,19 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Distributed Computing
 Requires-Dist: numpy (>=1.23.5,<2.0.0)
-Requires-Dist: qctrl-sphinx-theme (>=2.1.1,<3.0.0)
 Project-URL: Documentation, https://docs.q-ctrl.com/boulder-opal/references/qctrl-qua/
 Project-URL: Facebook, https://www.facebook.com/qctrl
 Project-URL: GitHub, https://github.com/qctrl
 Project-URL: LinkedIn, https://www.linkedin.com/company/q-ctrl/
 Project-URL: Twitter, https://twitter.com/qctrlHQ
 Project-URL: YouTube, https://www.youtube.com/qctrl
 Description-Content-Type: text/markdown
 
-# Q-CTRL QUA Adapter
+# ⚠️ (DEPRECATED) This package has been deprecated ⚠️
 
-The Q-CTRL QUA Adapter package allows you to integrate Boulder Opal with the QUA quantum computing language.
-
-See how you can do that in the user guide [How to integrate Boulder Opal with QUA from Quantum Machines](https://docs.q-ctrl.com/boulder-opal/user-guides/how-to-integrate-boulder-opal-with-qua-from-quantum-machines).
+Visit https://docs.q-ctrl.com/ for updated information about how to integrate Boulder Opal with QUA.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

