# Comparing `tmp/pih-auto-0.21.tar.gz` & `tmp/pih-auto-0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-auto-0.21.tar", last modified: Mon May 13 03:17:11 2024, max compression
+gzip compressed data, was "pih-auto-0.22.tar", last modified: Sun May 19 22:43:03 2024, max compression
```

## Comparing `pih-auto-0.21.tar` & `pih-auto-0.22.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 03:17:11.736954 pih-auto-0.21/
-drwxrwxrwx   0        0        0        0 2024-05-13 03:17:11.249475 pih-auto-0.21/AutomationService/
--rw-rw-rw-   0        0        0        0 2022-08-10 08:09:48.000000 pih-auto-0.21/AutomationService/__init__.py
--rw-rw-rw-   0        0        0      152 2024-02-14 02:13:48.000000 pih-auto-0.21/AutomationService/__main__.py
--rw-rw-rw-   0        0        0      632 2024-05-13 01:13:01.000000 pih-auto-0.21/AutomationService/const.py
--rw-rw-rw-   0        0        0    19210 2024-05-13 01:12:44.000000 pih-auto-0.21/AutomationService/service.py
--rw-rw-rw-   0        0        0      295 2024-05-13 03:17:11.705699 pih-auto-0.21/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-13 03:17:11.658823 pih-auto-0.21/pih_auto.egg-info/
--rw-rw-rw-   0        0        0      295 2024-05-13 03:17:10.000000 pih-auto-0.21/pih_auto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2024-05-13 03:17:11.000000 pih-auto-0.21/pih_auto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 03:17:10.000000 pih-auto-0.21/pih_auto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-05-13 03:17:10.000000 pih-auto-0.21/pih_auto.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       13 2024-05-13 03:17:10.000000 pih-auto-0.21/pih_auto.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-13 03:17:10.000000 pih-auto-0.21/pih_auto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 03:17:11.738986 pih-auto-0.21/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-19 22:43:03.223473 pih-auto-0.22/
+drwxrwxrwx   0        0        0        0 2024-05-19 22:43:02.836753 pih-auto-0.22/AutomationService/
+-rw-rw-rw-   0        0        0        0 2022-08-10 08:09:48.000000 pih-auto-0.22/AutomationService/__init__.py
+-rw-rw-rw-   0        0        0      152 2024-02-14 02:13:48.000000 pih-auto-0.22/AutomationService/__main__.py
+-rw-rw-rw-   0        0        0      632 2024-05-19 22:42:02.000000 pih-auto-0.22/AutomationService/const.py
+-rw-rw-rw-   0        0        0    18948 2024-05-16 00:51:34.000000 pih-auto-0.22/AutomationService/service.py
+-rw-rw-rw-   0        0        0      295 2024-05-19 22:43:03.207861 pih-auto-0.22/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-19 22:43:03.160968 pih-auto-0.22/pih_auto.egg-info/
+-rw-rw-rw-   0        0        0      295 2024-05-19 22:43:02.000000 pih-auto-0.22/pih_auto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2024-05-19 22:43:02.000000 pih-auto-0.22/pih_auto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 22:43:02.000000 pih-auto-0.22/pih_auto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-05-19 22:43:02.000000 pih-auto-0.22/pih_auto.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       13 2024-05-19 22:43:02.000000 pih-auto-0.22/pih_auto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-19 22:43:02.000000 pih-auto-0.22/pih_auto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 22:43:03.254726 pih-auto-0.22/setup.cfg
```

### Comparing `pih-auto-0.21/AutomationService/const.py` & `pih-auto-0.22/AutomationService/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pih.collections.service import ServiceDescription
 
 
 NAME: str = "Automation"
 
 HOST = Hosts.BACKUP_WORKER
 
-VERSION: str = "0.21"
+VERSION: str = "0.22"
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     description="Automation service",
     host=HOST.NAME,
     use_standalone=True,
     standalone_name="auto",
```

### Comparing `pih-auto-0.21/AutomationService/service.py` & `pih-auto-0.22/AutomationService/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,23 +18,14 @@
 ISOLATED: bool = False
 
 
 def start(as_standalone: bool = False) -> None:
 
     if A.U.for_service(SD, as_standalone=as_standalone):
 
-        from pih.collections import (
-            User,
-            ActionWasDone,
-            NewMailMessage,
-            PolibasePerson,
-            ResourceStatus,
-            EmailInformation,
-            ChillerIndicationsValueContainer,
-        )
         from MobileHelperService.client import Client as MIO
         from pih.collections.service import SubscribtionResult
         from MobileHelperService.api import MobileOutput, mio_command
         from MobileHelperService.const import COMMAND_KEYWORDS, FLAG_KEYWORDS
 
         from datetime import datetime
```

