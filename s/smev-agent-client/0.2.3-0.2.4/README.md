# Comparing `tmp/smev-agent-client-0.2.3.tar.gz` & `tmp/smev-agent-client-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smev-agent-client-0.2.3.tar", last modified: Thu Sep 28 07:03:37 2023, max compression
+gzip compressed data, was "smev-agent-client-0.2.4.tar", last modified: Mon May 20 09:27:08 2024, max compression
```

## Comparing `smev-agent-client-0.2.3.tar` & `smev-agent-client-0.2.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-09-28 07:03:37.219936 smev-agent-client-0.2.3/
--rw-r--r--   0 toor      (1000) toor      (1000)      290 2022-12-16 09:04:21.000000 smev-agent-client-0.2.3/MANIFEST.in
--rw-r--r--   0 toor      (1000) toor      (1000)     2836 2023-09-28 07:03:37.218936 smev-agent-client-0.2.3/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)     1802 2022-12-16 09:04:21.000000 smev-agent-client-0.2.3/README.md
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-09-28 07:03:37.211936 smev-agent-client-0.2.3/requirements/
--rw-r--r--   0 toor      (1000) toor      (1000)       87 2023-09-28 07:03:28.000000 smev-agent-client-0.2.3/requirements/base.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       12 2022-12-16 09:04:21.000000 smev-agent-client-0.2.3/requirements/prod.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-09-28 07:03:37.219936 smev-agent-client-0.2.3/setup.cfg
--rw-r--r--   0 toor      (1000) toor      (1000)     2415 2022-12-16 09:04:21.000000 smev-agent-client-0.2.3/setup.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-09-28 07:03:37.208936 smev-agent-client-0.2.3/src/
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-09-28 07:03:37.212936 smev-agent-client-0.2.3/src/smev_agent_client/
--rw-r--r--   0 toor      (1000) toor      (1000)      593 2022-12-16 09:04:21.000000 smev-agent-client-0.2.3/src/smev_agent_client/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1032 2022-12-16 09:04:21.000000 smev-agent-client-0.2.3/src/smev_agent_client/adapters.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1337 2022-12-16 09:04:21.000000 smev-agent-client-0.2.3/src/smev_agent_client/configuration.py
--rw-r--r--   0 toor      (1000) toor      (1000)      280 2022-12-16 09:04:21.000000 smev-agent-client-0.2.3/src/smev_agent_client/const.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-09-28 07:03:37.213936 smev-agent-client-0.2.3/src/smev_agent_client/contrib/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-12-16 09:04:21.000000 smev-agent-client-0.2.3/src/smev_agent_client/contrib/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-09-28 07:03:37.214936 smev-agent-client-0.2.3/src/smev_agent_client/contrib/my_edu/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-12-16 09:04:21.000000 smev-agent-client-0.2.3/src/smev_agent_client/contrib/my_edu/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-09-28 07:03:37.215937 smev-agent-client-0.2.3/src/smev_agent_client/contrib/my_edu/interfaces/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-12-16 09:04:21.000000 smev-agent-client-0.2.3/src/smev_agent_client/contrib/my_edu/interfaces/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5461 2022-12-16 09:04:21.000000 smev-agent-client-0.2.3/src/smev_agent_client/contrib/my_edu/interfaces/myedu.json
--rw-r--r--   0 toor      (1000) toor      (1000)     2345 2022-12-16 09:04:21.000000 smev-agent-client-0.2.3/src/smev_agent_client/contrib/my_edu/interfaces/rest.py
--rw-r--r--   0 toor      (1000) toor      (1000)      905 2022-12-16 09:04:21.000000 smev-agent-client-0.2.3/src/smev_agent_client/contrib/my_edu/interfaces/utils.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1530 2022-12-16 09:04:21.000000 smev-agent-client-0.2.3/src/smev_agent_client/contrib/my_edu/interfaces/validation.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-09-28 07:03:37.216936 smev-agent-client-0.2.3/src/smev_agent_client/interfaces/
--rw-r--r--   0 toor      (1000) toor      (1000)      242 2022-12-16 09:04:21.000000 smev-agent-client-0.2.3/src/smev_agent_client/interfaces/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      622 2022-12-16 09:04:21.000000 smev-agent-client-0.2.3/src/smev_agent_client/interfaces/base.py
--rw-r--r--   0 toor      (1000) toor      (1000)     7396 2022-12-16 09:04:21.000000 smev-agent-client-0.2.3/src/smev_agent_client/interfaces/rest.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-09-28 07:03:37.217936 smev-agent-client-0.2.3/src/smev_agent_client/logging/
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2022-12-16 09:04:21.000000 smev-agent-client-0.2.3/src/smev_agent_client/logging/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1174 2022-12-16 09:04:21.000000 smev-agent-client-0.2.3/src/smev_agent_client/logging/base.py
--rw-r--r--   0 toor      (1000) toor      (1000)      386 2022-12-16 09:04:21.000000 smev-agent-client-0.2.3/src/smev_agent_client/logging/db.py
--rw-r--r--   0 toor      (1000) toor      (1000)      441 2022-12-16 09:04:21.000000 smev-agent-client-0.2.3/src/smev_agent_client/logging/stdlib.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-09-28 07:03:37.217936 smev-agent-client-0.2.3/src/smev_agent_client/migrations/
--rw-r--r--   0 toor      (1000) toor      (1000)     1034 2022-12-16 09:04:21.000000 smev-agent-client-0.2.3/src/smev_agent_client/migrations/0001_initial.py
--rw-r--r--   0 toor      (1000) toor      (1000)      419 2022-12-22 13:47:00.000000 smev-agent-client-0.2.3/src/smev_agent_client/migrations/0002_auto_20220714_0650.py
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-12-16 09:04:21.000000 smev-agent-client-0.2.3/src/smev_agent_client/migrations/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      902 2022-12-22 13:33:39.000000 smev-agent-client-0.2.3/src/smev_agent_client/models.py
--rw-r--r--   0 toor      (1000) toor      (1000)      706 2022-12-16 09:04:21.000000 smev-agent-client-0.2.3/src/smev_agent_client/utils.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-09-28 07:03:37.213936 smev-agent-client-0.2.3/src/smev_agent_client.egg-info/
--rw-r--r--   0 toor      (1000) toor      (1000)     2836 2023-09-28 07:03:37.000000 smev-agent-client-0.2.3/src/smev_agent_client.egg-info/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)     1334 2023-09-28 07:03:37.000000 smev-agent-client-0.2.3/src/smev_agent_client.egg-info/SOURCES.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       44 2023-09-28 07:03:37.000000 smev-agent-client-0.2.3/src/smev_agent_client.egg-info/dependency_links.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       87 2023-09-28 07:03:37.000000 smev-agent-client-0.2.3/src/smev_agent_client.egg-info/requires.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       18 2023-09-28 07:03:37.000000 smev-agent-client-0.2.3/src/smev_agent_client.egg-info/top_level.txt
--rw-r--r--   0 toor      (1000) toor      (1000)      448 2023-09-28 07:03:37.000000 smev-agent-client-0.2.3/version.conf
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-20 09:27:08.183514 smev-agent-client-0.2.4/
+-rw-r--r--   0 toor      (1000) toor      (1000)      290 2022-12-16 09:04:21.000000 smev-agent-client-0.2.4/MANIFEST.in
+-rw-r--r--   0 toor      (1000) toor      (1000)     2831 2024-05-20 09:27:08.182515 smev-agent-client-0.2.4/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)     1802 2022-12-16 09:04:21.000000 smev-agent-client-0.2.4/README.md
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-20 09:27:08.150514 smev-agent-client-0.2.4/requirements/
+-rw-r--r--   0 toor      (1000) toor      (1000)       82 2024-05-20 09:27:02.000000 smev-agent-client-0.2.4/requirements/base.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       12 2022-12-16 09:04:21.000000 smev-agent-client-0.2.4/requirements/prod.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       38 2024-05-20 09:27:08.183514 smev-agent-client-0.2.4/setup.cfg
+-rw-r--r--   0 toor      (1000) toor      (1000)     2415 2022-12-16 09:04:21.000000 smev-agent-client-0.2.4/setup.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-20 09:27:08.146515 smev-agent-client-0.2.4/src/
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-20 09:27:08.156515 smev-agent-client-0.2.4/src/smev_agent_client/
+-rw-r--r--   0 toor      (1000) toor      (1000)      593 2022-12-16 09:04:21.000000 smev-agent-client-0.2.4/src/smev_agent_client/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1032 2022-12-16 09:04:21.000000 smev-agent-client-0.2.4/src/smev_agent_client/adapters.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1337 2022-12-16 09:04:21.000000 smev-agent-client-0.2.4/src/smev_agent_client/configuration.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      280 2022-12-16 09:04:21.000000 smev-agent-client-0.2.4/src/smev_agent_client/const.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-20 09:27:08.160514 smev-agent-client-0.2.4/src/smev_agent_client/contrib/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-12-16 09:04:21.000000 smev-agent-client-0.2.4/src/smev_agent_client/contrib/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-20 09:27:08.160514 smev-agent-client-0.2.4/src/smev_agent_client/contrib/my_edu/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-12-16 09:04:21.000000 smev-agent-client-0.2.4/src/smev_agent_client/contrib/my_edu/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-20 09:27:08.168515 smev-agent-client-0.2.4/src/smev_agent_client/contrib/my_edu/interfaces/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-12-16 09:04:21.000000 smev-agent-client-0.2.4/src/smev_agent_client/contrib/my_edu/interfaces/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5461 2022-12-16 09:04:21.000000 smev-agent-client-0.2.4/src/smev_agent_client/contrib/my_edu/interfaces/myedu.json
+-rw-r--r--   0 toor      (1000) toor      (1000)     2345 2022-12-16 09:04:21.000000 smev-agent-client-0.2.4/src/smev_agent_client/contrib/my_edu/interfaces/rest.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      905 2022-12-16 09:04:21.000000 smev-agent-client-0.2.4/src/smev_agent_client/contrib/my_edu/interfaces/utils.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1530 2022-12-16 09:04:21.000000 smev-agent-client-0.2.4/src/smev_agent_client/contrib/my_edu/interfaces/validation.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-20 09:27:08.171514 smev-agent-client-0.2.4/src/smev_agent_client/interfaces/
+-rw-r--r--   0 toor      (1000) toor      (1000)      242 2022-12-16 09:04:21.000000 smev-agent-client-0.2.4/src/smev_agent_client/interfaces/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      622 2022-12-16 09:04:21.000000 smev-agent-client-0.2.4/src/smev_agent_client/interfaces/base.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     7396 2022-12-16 09:04:21.000000 smev-agent-client-0.2.4/src/smev_agent_client/interfaces/rest.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-20 09:27:08.176514 smev-agent-client-0.2.4/src/smev_agent_client/logging/
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2022-12-16 09:04:21.000000 smev-agent-client-0.2.4/src/smev_agent_client/logging/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1174 2022-12-16 09:04:21.000000 smev-agent-client-0.2.4/src/smev_agent_client/logging/base.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      386 2022-12-16 09:04:21.000000 smev-agent-client-0.2.4/src/smev_agent_client/logging/db.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      441 2022-12-16 09:04:21.000000 smev-agent-client-0.2.4/src/smev_agent_client/logging/stdlib.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-20 09:27:08.181515 smev-agent-client-0.2.4/src/smev_agent_client/migrations/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1034 2022-12-16 09:04:21.000000 smev-agent-client-0.2.4/src/smev_agent_client/migrations/0001_initial.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      419 2022-12-22 13:47:00.000000 smev-agent-client-0.2.4/src/smev_agent_client/migrations/0002_auto_20220714_0650.py
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-12-16 09:04:21.000000 smev-agent-client-0.2.4/src/smev_agent_client/migrations/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      902 2022-12-22 13:33:39.000000 smev-agent-client-0.2.4/src/smev_agent_client/models.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      706 2022-12-16 09:04:21.000000 smev-agent-client-0.2.4/src/smev_agent_client/utils.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-20 09:27:08.182515 smev-agent-client-0.2.4/src/smev_agent_client.egg-info/
+-rw-r--r--   0 toor      (1000) toor      (1000)     2831 2024-05-20 09:27:08.000000 smev-agent-client-0.2.4/src/smev_agent_client.egg-info/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)     1334 2024-05-20 09:27:08.000000 smev-agent-client-0.2.4/src/smev_agent_client.egg-info/SOURCES.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       44 2024-05-20 09:27:08.000000 smev-agent-client-0.2.4/src/smev_agent_client.egg-info/dependency_links.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       82 2024-05-20 09:27:08.000000 smev-agent-client-0.2.4/src/smev_agent_client.egg-info/requires.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       18 2024-05-20 09:27:08.000000 smev-agent-client-0.2.4/src/smev_agent_client.egg-info/top_level.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)      450 2024-05-20 09:27:08.000000 smev-agent-client-0.2.4/version.conf
```

### Comparing `smev-agent-client-0.2.3/PKG-INFO` & `smev-agent-client-0.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smev-agent-client
-Version: 0.2.3
+Version: 0.2.4
 Summary: Клиент для взаимодействия с Агентом ПОДД СМЭВ
 Author: BARS Group
 Author-email: education_dev@bars-open.ru
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
 Classifier: Natural Language :: Russian
@@ -17,15 +17,15 @@
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic<1.10.0,>=1.9.0
-Requires-Dist: requests<2.28.0,>=1.1.0
+Requires-Dist: requests<3,>=1.1.0
 Requires-Dist: django<4.1,>=1.11
 Requires-Dist: openapi-core==0.14.5
 
 # Клиент для взаимодействия со СМЭВ3 посредством Адаптера
 ## Подключение
 settings:
```

### Comparing `smev-agent-client-0.2.3/README.md` & `smev-agent-client-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `smev-agent-client-0.2.3/setup.py` & `smev-agent-client-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `smev-agent-client-0.2.3/src/smev_agent_client/__init__.py` & `smev-agent-client-0.2.4/src/smev_agent_client/__init__.py`

 * *Files identical despite different names*

### Comparing `smev-agent-client-0.2.3/src/smev_agent_client/adapters.py` & `smev-agent-client-0.2.4/src/smev_agent_client/adapters.py`

 * *Files identical despite different names*

### Comparing `smev-agent-client-0.2.3/src/smev_agent_client/configuration.py` & `smev-agent-client-0.2.4/src/smev_agent_client/configuration.py`

 * *Files identical despite different names*

### Comparing `smev-agent-client-0.2.3/src/smev_agent_client/contrib/my_edu/interfaces/myedu.json` & `smev-agent-client-0.2.4/src/smev_agent_client/contrib/my_edu/interfaces/myedu.json`

 * *Files identical despite different names*

### Comparing `smev-agent-client-0.2.3/src/smev_agent_client/contrib/my_edu/interfaces/rest.py` & `smev-agent-client-0.2.4/src/smev_agent_client/contrib/my_edu/interfaces/rest.py`

 * *Files identical despite different names*

### Comparing `smev-agent-client-0.2.3/src/smev_agent_client/contrib/my_edu/interfaces/utils.py` & `smev-agent-client-0.2.4/src/smev_agent_client/contrib/my_edu/interfaces/utils.py`

 * *Files identical despite different names*

### Comparing `smev-agent-client-0.2.3/src/smev_agent_client/contrib/my_edu/interfaces/validation.py` & `smev-agent-client-0.2.4/src/smev_agent_client/contrib/my_edu/interfaces/validation.py`

 * *Files identical despite different names*

### Comparing `smev-agent-client-0.2.3/src/smev_agent_client/interfaces/base.py` & `smev-agent-client-0.2.4/src/smev_agent_client/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `smev-agent-client-0.2.3/src/smev_agent_client/interfaces/rest.py` & `smev-agent-client-0.2.4/src/smev_agent_client/interfaces/rest.py`

 * *Files identical despite different names*

### Comparing `smev-agent-client-0.2.3/src/smev_agent_client/logging/base.py` & `smev-agent-client-0.2.4/src/smev_agent_client/logging/base.py`

 * *Files identical despite different names*

### Comparing `smev-agent-client-0.2.3/src/smev_agent_client/migrations/0001_initial.py` & `smev-agent-client-0.2.4/src/smev_agent_client/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `smev-agent-client-0.2.3/src/smev_agent_client/models.py` & `smev-agent-client-0.2.4/src/smev_agent_client/models.py`

 * *Files identical despite different names*

### Comparing `smev-agent-client-0.2.3/src/smev_agent_client/utils.py` & `smev-agent-client-0.2.4/src/smev_agent_client/utils.py`

 * *Files identical despite different names*

### Comparing `smev-agent-client-0.2.3/src/smev_agent_client.egg-info/PKG-INFO` & `smev-agent-client-0.2.4/src/smev_agent_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smev-agent-client
-Version: 0.2.3
+Version: 0.2.4
 Summary: Клиент для взаимодействия с Агентом ПОДД СМЭВ
 Author: BARS Group
 Author-email: education_dev@bars-open.ru
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
 Classifier: Natural Language :: Russian
@@ -17,15 +17,15 @@
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic<1.10.0,>=1.9.0
-Requires-Dist: requests<2.28.0,>=1.1.0
+Requires-Dist: requests<3,>=1.1.0
 Requires-Dist: django<4.1,>=1.11
 Requires-Dist: openapi-core==0.14.5
 
 # Клиент для взаимодействия со СМЭВ3 посредством Адаптера
 ## Подключение
 settings:
```

### Comparing `smev-agent-client-0.2.3/src/smev_agent_client.egg-info/SOURCES.txt` & `smev-agent-client-0.2.4/src/smev_agent_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

