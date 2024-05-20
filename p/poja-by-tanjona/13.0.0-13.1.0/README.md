# Comparing `tmp/poja-by-tanjona-13.0.0.tar.gz` & `tmp/poja-by-tanjona-13.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poja-by-tanjona-13.0.0.tar", last modified: Sat May 18 15:22:27 2024, max compression
+gzip compressed data, was "poja-by-tanjona-13.1.0.tar", last modified: Mon May 20 06:19:22 2024, max compression
```

## Comparing `poja-by-tanjona-13.0.0.tar` & `poja-by-tanjona-13.1.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:22:27.705960 poja-by-tanjona-13.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-18 15:22:13.000000 poja-by-tanjona-13.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-05-18 15:22:27.705960 poja-by-tanjona-13.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-05-18 15:22:13.000000 poja-by-tanjona-13.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:22:27.701960 poja-by-tanjona-13.0.0/poja/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-18 15:22:13.000000 poja-by-tanjona-13.0.0/poja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-18 15:22:13.000000 poja-by-tanjona-13.0.0/poja/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18864 2024-05-18 15:22:13.000000 poja-by-tanjona-13.0.0/poja/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:22:27.705960 poja-by-tanjona-13.0.0/poja/database/
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-05-18 15:22:13.000000 poja-by-tanjona-13.0.0/poja/database/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:22:27.705960 poja-by-tanjona-13.0.0/poja/genclients/
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-18 15:22:13.000000 poja-by-tanjona-13.0.0/poja/genclients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:22:27.705960 poja-by-tanjona-13.0.0/poja/mygit/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-18 15:22:13.000000 poja-by-tanjona-13.0.0/poja/mygit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:22:27.705960 poja-by-tanjona-13.0.0/poja/myos/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-18 15:22:13.000000 poja-by-tanjona-13.0.0/poja/myos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:22:27.705960 poja-by-tanjona-13.0.0/poja/myrich/
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-18 15:22:13.000000 poja-by-tanjona-13.0.0/poja/myrich/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:22:27.705960 poja-by-tanjona-13.0.0/poja/sed/
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-18 15:22:13.000000 poja-by-tanjona-13.0.0/poja/sed/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:22:27.705960 poja-by-tanjona-13.0.0/poja/sentry/
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-18 15:22:13.000000 poja-by-tanjona-13.0.0/poja/sentry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:22:27.705960 poja-by-tanjona-13.0.0/poja/sonar/
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-18 15:22:13.000000 poja-by-tanjona-13.0.0/poja/sonar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-18 15:22:13.000000 poja-by-tanjona-13.0.0/poja/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:22:27.705960 poja-by-tanjona-13.0.0/poja/vpcscoped/
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-05-18 15:22:13.000000 poja-by-tanjona-13.0.0/poja/vpcscoped/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:22:27.705960 poja-by-tanjona-13.0.0/poja_by_tanjona.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-05-18 15:22:27.000000 poja-by-tanjona-13.0.0/poja_by_tanjona.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-18 15:22:27.000000 poja-by-tanjona-13.0.0/poja_by_tanjona.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 15:22:27.000000 poja-by-tanjona-13.0.0/poja_by_tanjona.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-18 15:22:27.000000 poja-by-tanjona-13.0.0/poja_by_tanjona.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-18 15:22:27.000000 poja-by-tanjona-13.0.0/poja_by_tanjona.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 15:22:27.705960 poja-by-tanjona-13.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-18 15:22:13.000000 poja-by-tanjona-13.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:19:22.808298 poja-by-tanjona-13.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-20 06:19:06.000000 poja-by-tanjona-13.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-05-20 06:19:22.808298 poja-by-tanjona-13.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-05-20 06:19:06.000000 poja-by-tanjona-13.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:19:22.808298 poja-by-tanjona-13.1.0/poja/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-20 06:19:06.000000 poja-by-tanjona-13.1.0/poja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-20 06:19:06.000000 poja-by-tanjona-13.1.0/poja/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18897 2024-05-20 06:19:06.000000 poja-by-tanjona-13.1.0/poja/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:19:22.808298 poja-by-tanjona-13.1.0/poja/database/
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-05-20 06:19:06.000000 poja-by-tanjona-13.1.0/poja/database/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:19:22.808298 poja-by-tanjona-13.1.0/poja/genclients/
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-20 06:19:06.000000 poja-by-tanjona-13.1.0/poja/genclients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:19:22.808298 poja-by-tanjona-13.1.0/poja/mygit/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-20 06:19:06.000000 poja-by-tanjona-13.1.0/poja/mygit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:19:22.808298 poja-by-tanjona-13.1.0/poja/myos/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-20 06:19:06.000000 poja-by-tanjona-13.1.0/poja/myos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:19:22.808298 poja-by-tanjona-13.1.0/poja/myrich/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-20 06:19:06.000000 poja-by-tanjona-13.1.0/poja/myrich/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:19:22.808298 poja-by-tanjona-13.1.0/poja/sed/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-20 06:19:06.000000 poja-by-tanjona-13.1.0/poja/sed/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:19:22.808298 poja-by-tanjona-13.1.0/poja/sentry/
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-20 06:19:06.000000 poja-by-tanjona-13.1.0/poja/sentry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:19:22.808298 poja-by-tanjona-13.1.0/poja/sonar/
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-20 06:19:06.000000 poja-by-tanjona-13.1.0/poja/sonar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-20 06:19:06.000000 poja-by-tanjona-13.1.0/poja/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:19:22.808298 poja-by-tanjona-13.1.0/poja/vpcscoped/
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-05-20 06:19:06.000000 poja-by-tanjona-13.1.0/poja/vpcscoped/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:19:22.808298 poja-by-tanjona-13.1.0/poja_by_tanjona.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-05-20 06:19:22.000000 poja-by-tanjona-13.1.0/poja_by_tanjona.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-20 06:19:22.000000 poja-by-tanjona-13.1.0/poja_by_tanjona.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 06:19:22.000000 poja-by-tanjona-13.1.0/poja_by_tanjona.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-20 06:19:22.000000 poja-by-tanjona-13.1.0/poja_by_tanjona.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-20 06:19:22.000000 poja-by-tanjona-13.1.0/poja_by_tanjona.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 06:19:22.808298 poja-by-tanjona-13.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-20 06:19:06.000000 poja-by-tanjona-13.1.0/setup.py
```

### Comparing `poja-by-tanjona-13.0.0/LICENSE` & `poja-by-tanjona-13.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `poja-by-tanjona-13.0.0/PKG-INFO` & `poja-by-tanjona-13.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poja-by-tanjona
-Version: 13.0.0
+Version: 13.1.0
 Summary: Serverless Postgres+Java hosted on Github+AWS
 Home-page: https://github.com/hei-school/poja-cli
 Author: HEI
 Author-email: contact@hei.school
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `poja-by-tanjona-13.0.0/README.md` & `poja-by-tanjona-13.1.0/README.md`

 * *Files identical despite different names*

### Comparing `poja-by-tanjona-13.0.0/poja/core.py` & `poja-by-tanjona-13.1.0/poja/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import yaml
 from yaml.loader import BaseLoader
 import os
 from poja.myos import cd_then_exec
 from pathlib import Path
 
 GIT_URL = "https://github.com/tanjonaaa/poja"
-GIT_TAG_OR_COMMIT = "6d1233a"
+GIT_TAG_OR_COMMIT = "4abb7c825a0420052830cf11028fe2072420d75e"
 
 DEFAULT_GROUP_NAME = "school.hei"
 DEFAULT_PACKAGE_FULL_NAME = DEFAULT_GROUP_NAME + ".poja"
 
 
 def gen(
     poja_conf=None,
```

### Comparing `poja-by-tanjona-13.0.0/poja/database/__init__.py` & `poja-by-tanjona-13.1.0/poja/database/__init__.py`

 * *Files identical despite different names*

### Comparing `poja-by-tanjona-13.0.0/poja/genclients/__init__.py` & `poja-by-tanjona-13.1.0/poja/genclients/__init__.py`

 * *Files identical despite different names*

### Comparing `poja-by-tanjona-13.0.0/poja/sed/__init__.py` & `poja-by-tanjona-13.1.0/poja/sed/__init__.py`

 * *Files identical despite different names*

### Comparing `poja-by-tanjona-13.0.0/poja/sentry/__init__.py` & `poja-by-tanjona-13.1.0/poja/sentry/__init__.py`

 * *Files identical despite different names*

### Comparing `poja-by-tanjona-13.0.0/poja/sonar/__init__.py` & `poja-by-tanjona-13.1.0/poja/sonar/__init__.py`

 * *Files identical despite different names*

### Comparing `poja-by-tanjona-13.0.0/poja/vpcscoped/__init__.py` & `poja-by-tanjona-13.1.0/poja/vpcscoped/__init__.py`

 * *Files identical despite different names*

### Comparing `poja-by-tanjona-13.0.0/poja_by_tanjona.egg-info/PKG-INFO` & `poja-by-tanjona-13.1.0/poja_by_tanjona.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poja-by-tanjona
-Version: 13.0.0
+Version: 13.1.0
 Summary: Serverless Postgres+Java hosted on Github+AWS
 Home-page: https://github.com/hei-school/poja-cli
 Author: HEI
 Author-email: contact@hei.school
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `poja-by-tanjona-13.0.0/setup.py` & `poja-by-tanjona-13.1.0/setup.py`

 * *Files identical despite different names*

