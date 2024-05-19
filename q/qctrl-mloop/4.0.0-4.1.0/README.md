# Comparing `tmp/qctrl_mloop-4.0.0.tar.gz` & `tmp/qctrl_mloop-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qctrl_mloop-4.0.0.tar", max compression
+gzip compressed data, was "qctrl_mloop-4.1.0.tar", max compression
```

## Comparing `qctrl_mloop-4.0.0.tar` & `qctrl_mloop-4.1.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    36653 2023-10-17 00:41:56.814088 qctrl_mloop-4.0.0/LICENSE
--rw-r--r--   0        0        0      470 2023-10-17 00:41:56.814088 qctrl_mloop-4.0.0/README.md
--rw-r--r--   0        0        0     2632 2023-10-17 00:42:17.554761 qctrl_mloop-4.0.0/pyproject.toml
--rw-r--r--   0        0        0      862 2023-10-17 00:42:17.566761 qctrl_mloop-4.0.0/qctrlmloop/__init__.py
--rw-r--r--   0        0        0    13035 2023-10-17 00:41:56.814088 qctrl_mloop-4.0.0/qctrlmloop/controller.py
--rw-r--r--   0        0        0     2564 1970-01-01 00:00:00.000000 qctrl_mloop-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0    36587 2024-05-19 22:55:31.819425 qctrl_mloop-4.1.0/LICENSE
+-rw-r--r--   0        0        0      184 2024-05-19 22:55:31.819425 qctrl_mloop-4.1.0/README.md
+-rw-r--r--   0        0        0     2651 2024-05-19 22:55:55.339805 qctrl_mloop-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0      862 2024-05-19 22:55:55.347805 qctrl_mloop-4.1.0/qctrlmloop/__init__.py
+-rw-r--r--   0        0        0    13035 2024-05-19 22:55:31.823425 qctrl_mloop-4.1.0/qctrlmloop/controller.py
+-rw-r--r--   0        0        0     2278 1970-01-01 00:00:00.000000 qctrl_mloop-4.1.0/PKG-INFO
```

### Comparing `qctrl_mloop-4.0.0/LICENSE` & `qctrl_mloop-4.1.0/LICENSE`

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

### Comparing `qctrl_mloop-4.0.0/pyproject.toml` & `qctrl_mloop-4.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 [tool.poetry]
 name = "qctrl-mloop"
-version = "4.0.0"
+version = "4.1.0"
 description = "Q-CTRL M-LOOP Adapter"
 license = "https://q-ctrl.com/terms"
 authors = ["Q-CTRL <support@q-ctrl.com>"]
 maintainers = ["Q-CTRL <support@q-ctrl.com>"]
 readme = "README.md"
-repository = ""
 documentation = "https://docs.q-ctrl.com/boulder-opal/references/qctrl-mloop/"
 keywords = [
     "black opal",
     "boulder opal",
     "fire opal",
     "nisq",
     "open controls",
@@ -63,24 +62,25 @@
 python = ">=3.8, <3.12"
 M-LOOP = "~3.3.3"
 numpy = "^1.23.5"
 tensorflow = "^2.12.1"
 boulder-opal  = { version = "^1.0.0", source = "PyPI" }
 
 [tool.poetry.dev-dependencies]
-black = "^23.3.0"
+black = "^24.3.0"
 isort = "^5.12.0"
 mypy = "^1.4.1"
 pre-commit = "^3.3.3"
 pylint = "^2.17.1"
 pytest = "^7.4.0"
 pytest-mock = "^3.11.1"
-qctrl-sphinx-theme = "^2.1.3"
+qctrl-sphinx-theme = "^2.1.4"
 sphinx = "^5.0.0"
 tomli = "^2.0.1"
+sphinx-markdown-builder = "^0.6.6"
 
 [[tool.poetry.source]]
 name = "PyPI"
 priority = "supplemental"
 
 [[tool.poetry.source]]
 name = "Q-CTRL PyPI"
```

### Comparing `qctrl_mloop-4.0.0/qctrlmloop/__init__.py` & `qctrl_mloop-4.1.0/qctrlmloop/__init__.py`

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
@@ -10,15 +10,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS. See the
 # License for the specific language.
 
 """qctrlmloop - integration between Boulder Opal automated closed-loop optimizers and M-LOOP"""
 
 __author__ = "Q-CTRL <support@q-ctrl.com>"
-__version__ = "4.0.0"
+__version__ = "4.1.0"
 
 from .controller import (
     BoulderOpalController,
     boulder_opal_controller,
 )
 
 __all__ = ["BoulderOpalController", "boulder_opal_controller"]
```

### Comparing `qctrl_mloop-4.0.0/qctrlmloop/controller.py` & `qctrl_mloop-4.1.0/qctrlmloop/controller.py`

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

### Comparing `qctrl_mloop-4.0.0/PKG-INFO` & `qctrl_mloop-4.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qctrl-mloop
-Version: 4.0.0
+Version: 4.1.0
 Summary: Q-CTRL M-LOOP Adapter
 License: https://q-ctrl.com/terms
 Keywords: black opal,boulder opal,fire opal,nisq,open controls,q control,q ctrl,q-control,q-ctrl,qcontrol,qctrl,quantum,quantum algorithms,quantum circuits,quantum coding,quantum coding software,quantum computing,quantum control,quantum control software,quantum control theory,quantum engineering,quantum error correction,quantum firmware,quantum fundamentals,quantum sensing,qubit,qudit
 Author: Q-CTRL
 Author-email: support@q-ctrl.com
 Maintainer: Q-CTRL
 Maintainer-email: support@q-ctrl.com
@@ -35,13 +35,11 @@
 Project-URL: Facebook, https://www.facebook.com/qctrl
 Project-URL: GitHub, https://github.com/qctrl
 Project-URL: LinkedIn, https://www.linkedin.com/company/q-ctrl/
 Project-URL: Twitter, https://twitter.com/qctrlHQ
 Project-URL: YouTube, https://www.youtube.com/c/qctrl
 Description-Content-Type: text/markdown
 
-# Q-CTRL M-LOOP Adapter
+# ⚠️ (DEPRECATED) This package has been deprecated ⚠️
 
-The Q-CTRL M-LOOP Adapter package allows you to integrate Boulder Opal automated closed-loop optimizers with automated closed-loop optimizations managed by the open-source package M-LOOP.
-
-See how you can use M-LOOP with Boulder Opal in the user guide [How to manage automated closed-loop hardware optimization with M-LOOP](https://docs.q-ctrl.com/boulder-opal/user-guides/how-to-manage-automated-closed-loop-hardware-optimization-with-m-loop).
+Visit https://docs.q-ctrl.com/ for updated information about how to automate closed-loop optimization with Boulder Opal.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

