# Comparing `tmp/dp-launching-app-0.0.4.tar.gz` & `tmp/dp-launching-app-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dp-launching-app-0.0.4.tar", last modified: Thu May 16 07:07:45 2024, max compression
+gzip compressed data, was "dp-launching-app-0.0.6.tar", last modified: Mon May 20 10:17:34 2024, max compression
```

## Comparing `dp-launching-app-0.0.4.tar` & `dp-launching-app-0.0.6.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-16 07:07:45.658682 dp-launching-app-0.0.4/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)       94 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/MANIFEST.in
--rw-r--r--   0 xiongyanfei   (502) staff       (20)      156 2024-05-16 07:07:45.658510 dp-launching-app-0.0.4/PKG-INFO
--rw-r--r--   0 xiongyanfei   (502) staff       (20)        0 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/README.md
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-16 07:07:45.649754 dp-launching-app-0.0.4/dp/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)      154 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/dp/__init__.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-16 07:07:45.650177 dp-launching-app-0.0.4/dp/launching/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)       22 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/dp/launching/__init__.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-16 07:07:45.650566 dp-launching-app-0.0.4/dp/launching/cli/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)    12682 2024-05-16 07:06:32.000000 dp-launching-app-0.0.4/dp/launching/cli/__init__.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-16 07:07:45.651572 dp-launching-app-0.0.4/dp/launching/cli/api/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)        0 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/dp/launching/cli/api/__init__.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)    21712 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/dp/launching/cli/api/model.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     5386 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/dp/launching/cli/api/persistent_service.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-16 07:07:45.652098 dp-launching-app-0.0.4/dp/launching/cli/commands/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)        0 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/dp/launching/cli/commands/__init__.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     1315 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/dp/launching/cli/commands/launching.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-16 07:07:45.648379 dp-launching-app-0.0.4/dp/launching/cli/commands/scaffold/
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-16 07:07:45.652463 dp-launching-app-0.0.4/dp/launching/cli/commands/scaffold/basic/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     1858 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/dp/launching/cli/commands/scaffold/basic/basic.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-16 07:07:45.652789 dp-launching-app-0.0.4/dp/launching/cli/commands/scaffold/bohrium/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     2595 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/dp/launching/cli/commands/scaffold/bohrium/bohrium.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-16 07:07:45.653083 dp-launching-app-0.0.4/dp/launching/cli/commands/scaffold/dflow/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     2606 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/dp/launching/cli/commands/scaffold/dflow/dflow.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-16 07:07:45.653660 dp-launching-app-0.0.4/dp/launching/cli/utils/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)        0 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/dp/launching/cli/utils/__init__.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)      147 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/dp/launching/cli/utils/random.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-16 07:07:45.653942 dp-launching-app-0.0.4/dp/launching/report/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     2940 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/dp/launching/report/__init__.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-16 07:07:45.655905 dp-launching-app-0.0.4/dp/launching/typing/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)      175 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/dp/launching/typing/__init__.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-16 07:07:45.656746 dp-launching-app-0.0.4/dp/launching/typing/addon/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)        0 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/dp/launching/typing/addon/__init__.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)      867 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/dp/launching/typing/addon/sysmbol.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     6866 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/dp/launching/typing/addon/ui.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     7379 2024-05-11 02:54:01.000000 dp-launching-app-0.0.4/dp/launching/typing/basic.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)      749 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/dp/launching/typing/benchmark.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     1774 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/dp/launching/typing/bio.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     9731 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/dp/launching/typing/bohrium.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     4908 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/dp/launching/typing/dflow.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     6371 2024-05-10 07:03:20.000000 dp-launching-app-0.0.4/dp/launching/typing/io.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-16 07:07:45.658292 dp-launching-app-0.0.4/dp_launching_app.egg-info/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)      156 2024-05-16 07:07:45.000000 dp-launching-app-0.0.4/dp_launching_app.egg-info/PKG-INFO
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     1092 2024-05-16 07:07:45.000000 dp-launching-app-0.0.4/dp_launching_app.egg-info/SOURCES.txt
--rw-r--r--   0 xiongyanfei   (502) staff       (20)        1 2024-05-16 07:07:45.000000 dp-launching-app-0.0.4/dp_launching_app.egg-info/dependency_links.txt
--rw-r--r--   0 xiongyanfei   (502) staff       (20)       75 2024-05-16 07:07:45.000000 dp-launching-app-0.0.4/dp_launching_app.egg-info/entry_points.txt
--rw-r--r--   0 xiongyanfei   (502) staff       (20)      108 2024-05-16 07:07:45.000000 dp-launching-app-0.0.4/dp_launching_app.egg-info/requires.txt
--rw-r--r--   0 xiongyanfei   (502) staff       (20)        3 2024-05-16 07:07:45.000000 dp-launching-app-0.0.4/dp_launching_app.egg-info/top_level.txt
--rw-r--r--   0 xiongyanfei   (502) staff       (20)       38 2024-05-16 07:07:45.658720 dp-launching-app-0.0.4/setup.cfg
--rw-r--r--   0 xiongyanfei   (502) staff       (20)      714 2024-05-16 07:06:59.000000 dp-launching-app-0.0.4/setup.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-20 10:17:34.144948 dp-launching-app-0.0.6/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)       94 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/MANIFEST.in
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)      156 2024-05-20 10:17:34.144800 dp-launching-app-0.0.6/PKG-INFO
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)        0 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/README.md
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-20 10:17:34.137121 dp-launching-app-0.0.6/dp/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)      154 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/dp/__init__.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-20 10:17:34.137426 dp-launching-app-0.0.6/dp/launching/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)       22 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/dp/launching/__init__.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-20 10:17:34.137724 dp-launching-app-0.0.6/dp/launching/cli/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)    12682 2024-05-16 07:06:32.000000 dp-launching-app-0.0.6/dp/launching/cli/__init__.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-20 10:17:34.138725 dp-launching-app-0.0.6/dp/launching/cli/api/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)        0 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/dp/launching/cli/api/__init__.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)    21712 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/dp/launching/cli/api/model.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     5386 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/dp/launching/cli/api/persistent_service.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-20 10:17:34.139260 dp-launching-app-0.0.6/dp/launching/cli/commands/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)        0 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/dp/launching/cli/commands/__init__.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     1315 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/dp/launching/cli/commands/launching.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-20 10:17:34.135382 dp-launching-app-0.0.6/dp/launching/cli/commands/scaffold/
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-20 10:17:34.139513 dp-launching-app-0.0.6/dp/launching/cli/commands/scaffold/basic/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     1858 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/dp/launching/cli/commands/scaffold/basic/basic.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-20 10:17:34.139767 dp-launching-app-0.0.6/dp/launching/cli/commands/scaffold/bohrium/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     2595 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/dp/launching/cli/commands/scaffold/bohrium/bohrium.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-20 10:17:34.140014 dp-launching-app-0.0.6/dp/launching/cli/commands/scaffold/dflow/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     2606 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/dp/launching/cli/commands/scaffold/dflow/dflow.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-20 10:17:34.140504 dp-launching-app-0.0.6/dp/launching/cli/utils/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)        0 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/dp/launching/cli/utils/__init__.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)      147 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/dp/launching/cli/utils/random.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-20 10:17:34.140762 dp-launching-app-0.0.6/dp/launching/report/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     2940 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/dp/launching/report/__init__.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-20 10:17:34.142812 dp-launching-app-0.0.6/dp/launching/typing/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)      175 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/dp/launching/typing/__init__.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-20 10:17:34.143476 dp-launching-app-0.0.6/dp/launching/typing/addon/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)        0 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/dp/launching/typing/addon/__init__.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)      867 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/dp/launching/typing/addon/sysmbol.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     6866 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/dp/launching/typing/addon/ui.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     7379 2024-05-11 02:54:01.000000 dp-launching-app-0.0.6/dp/launching/typing/basic.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)      749 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/dp/launching/typing/benchmark.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     1774 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/dp/launching/typing/bio.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)    10526 2024-05-20 09:36:59.000000 dp-launching-app-0.0.6/dp/launching/typing/bohrium.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)      944 2024-05-20 10:13:32.000000 dp-launching-app-0.0.6/dp/launching/typing/dataset.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     4908 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/dp/launching/typing/dflow.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     6371 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/dp/launching/typing/io.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-20 10:17:34.144611 dp-launching-app-0.0.6/dp_launching_app.egg-info/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)      156 2024-05-20 10:17:33.000000 dp-launching-app-0.0.6/dp_launching_app.egg-info/PKG-INFO
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     1123 2024-05-20 10:17:34.000000 dp-launching-app-0.0.6/dp_launching_app.egg-info/SOURCES.txt
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)        1 2024-05-20 10:17:33.000000 dp-launching-app-0.0.6/dp_launching_app.egg-info/dependency_links.txt
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)       75 2024-05-20 10:17:33.000000 dp-launching-app-0.0.6/dp_launching_app.egg-info/entry_points.txt
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)      108 2024-05-20 10:17:34.000000 dp-launching-app-0.0.6/dp_launching_app.egg-info/requires.txt
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)        3 2024-05-20 10:17:34.000000 dp-launching-app-0.0.6/dp_launching_app.egg-info/top_level.txt
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)       38 2024-05-20 10:17:34.144983 dp-launching-app-0.0.6/setup.cfg
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)      714 2024-05-20 10:17:23.000000 dp-launching-app-0.0.6/setup.py
```

### Comparing `dp-launching-app-0.0.4/dp/launching/cli/__init__.py` & `dp-launching-app-0.0.6/dp/launching/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.4/dp/launching/cli/api/model.py` & `dp-launching-app-0.0.6/dp/launching/cli/api/model.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.4/dp/launching/cli/api/persistent_service.py` & `dp-launching-app-0.0.6/dp/launching/cli/api/persistent_service.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.4/dp/launching/cli/commands/launching.py` & `dp-launching-app-0.0.6/dp/launching/cli/commands/launching.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.4/dp/launching/cli/commands/scaffold/basic/basic.py` & `dp-launching-app-0.0.6/dp/launching/cli/commands/scaffold/basic/basic.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.4/dp/launching/cli/commands/scaffold/bohrium/bohrium.py` & `dp-launching-app-0.0.6/dp/launching/cli/commands/scaffold/bohrium/bohrium.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.4/dp/launching/cli/commands/scaffold/dflow/dflow.py` & `dp-launching-app-0.0.6/dp/launching/cli/commands/scaffold/dflow/dflow.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.4/dp/launching/report/__init__.py` & `dp-launching-app-0.0.6/dp/launching/report/__init__.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.4/dp/launching/typing/addon/sysmbol.py` & `dp-launching-app-0.0.6/dp/launching/typing/addon/sysmbol.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.4/dp/launching/typing/addon/ui.py` & `dp-launching-app-0.0.6/dp/launching/typing/addon/ui.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.4/dp/launching/typing/basic.py` & `dp-launching-app-0.0.6/dp/launching/typing/basic.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.4/dp/launching/typing/benchmark.py` & `dp-launching-app-0.0.6/dp/launching/typing/benchmark.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.4/dp/launching/typing/bio.py` & `dp-launching-app-0.0.6/dp/launching/typing/bio.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.4/dp/launching/typing/bohrium.py` & `dp-launching-app-0.0.6/dp/launching/typing/bohrium.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     "BohriumPlatform",
     "BohriumUsername",
     "BohriumTicket",
     "BohriumImage",
     "BohriumInstanceType",
     "BohriumStreamEndpoint",
     "BohriumJobID",
+    "BohriumPassword",
 ]
 
 
 class BohriumUsername(str):
     def get_value(self):
         return str(self)
 
@@ -308,7 +309,31 @@
             return value
         elif isinstance(value, str):
             return BohriumStreamEndpoint(value)
         elif isinstance(value, (bytes, bytearray, memoryview)):
             return BohriumStreamEndpoint(base64.b64encode(value).decode())
         else:
             raise Exception(f"BohriumStreamEndpoint Wrong type: {type(value)}")
+
+class BohriumPassword(str):
+    def get_value(self):
+        return str(self)
+
+    @classmethod
+    def __modify_schema__(cls, field_schema: Dict[str, Any]) -> None:
+        field_schema.update(format="bohrium_password", scope="executor")
+
+    @classmethod
+    def __get_validators__(cls) -> Any:
+        yield cls.validate
+
+    @classmethod
+    def validate(cls, value: Any) -> "BohriumPassword":
+        if isinstance(value, BohriumPassword):
+            return value
+        elif isinstance(value, str):
+            return BohriumPassword(value)
+        elif isinstance(value, (bytes, bytearray, memoryview)):
+            return BohriumPassword(base64.b64encode(value).decode())
+        else:
+            raise Exception(f"BohriumPassword Wrong type: {type(value)}")
+
```

### Comparing `dp-launching-app-0.0.4/dp/launching/typing/dflow.py` & `dp-launching-app-0.0.6/dp/launching/typing/dflow.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.4/dp/launching/typing/io.py` & `dp-launching-app-0.0.6/dp/launching/typing/io.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.4/dp_launching_app.egg-info/SOURCES.txt` & `dp-launching-app-0.0.6/dp_launching_app.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 dp/launching/cli/utils/random.py
 dp/launching/report/__init__.py
 dp/launching/typing/__init__.py
 dp/launching/typing/basic.py
 dp/launching/typing/benchmark.py
 dp/launching/typing/bio.py
 dp/launching/typing/bohrium.py
+dp/launching/typing/dataset.py
 dp/launching/typing/dflow.py
 dp/launching/typing/io.py
 dp/launching/typing/addon/__init__.py
 dp/launching/typing/addon/sysmbol.py
 dp/launching/typing/addon/ui.py
 dp_launching_app.egg-info/PKG-INFO
 dp_launching_app.egg-info/SOURCES.txt
```

### Comparing `dp-launching-app-0.0.4/setup.py` & `dp-launching-app-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="dp-launching-app",
-    version="0.0.4",
+    version="0.0.6",
     author="",
     author_email="",
     description="",
     long_description="",
     long_description_content_type="text/plain",
     url="",
     entry_points={
```

