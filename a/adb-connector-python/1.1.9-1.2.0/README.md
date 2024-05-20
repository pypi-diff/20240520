# Comparing `tmp/adb_connector_python-1.1.9-py3-none-any.whl.zip` & `tmp/adb_connector_python-1.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 11565 bytes, number of entries: 6
--rw-rw-r--  2.0 unx    39197 b- defN 24-May-08 07:33 adb_connector_python/connector.py
--rwxr-xr-x  2.0 unx     1088 b- defN 24-May-08 07:34 adb_connector_python-1.1.9.dist-info/LICENSE
--rw-rw-r--  2.0 unx     5452 b- defN 24-May-08 07:34 adb_connector_python-1.1.9.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-May-08 07:34 adb_connector_python-1.1.9.dist-info/WHEEL
--rwxr-xr-x  2.0 unx       21 b- defN 24-May-08 07:34 adb_connector_python-1.1.9.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      542 b- defN 24-May-08 07:34 adb_connector_python-1.1.9.dist-info/RECORD
-6 files, 46392 bytes uncompressed, 10573 bytes compressed:  77.2%
+Zip file size: 11513 bytes, number of entries: 6
+-rw-rw-r--  2.0 unx    39056 b- defN 24-May-20 07:31 adb_connector_python/connector.py
+-rwxr-xr-x  2.0 unx     1088 b- defN 24-May-20 07:34 adb_connector_python-1.2.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     5452 b- defN 24-May-20 07:34 adb_connector_python-1.2.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-20 07:34 adb_connector_python-1.2.0.dist-info/WHEEL
+-rwxr-xr-x  2.0 unx       21 b- defN 24-May-20 07:34 adb_connector_python-1.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      542 b- defN 24-May-20 07:34 adb_connector_python-1.2.0.dist-info/RECORD
+6 files, 46251 bytes uncompressed, 10521 bytes compressed:  77.3%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: adb_connector_python/connector.py
 Comment: 
 
-Filename: adb_connector_python-1.1.9.dist-info/LICENSE
+Filename: adb_connector_python-1.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: adb_connector_python-1.1.9.dist-info/METADATA
+Filename: adb_connector_python-1.2.0.dist-info/METADATA
 Comment: 
 
-Filename: adb_connector_python-1.1.9.dist-info/WHEEL
+Filename: adb_connector_python-1.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: adb_connector_python-1.1.9.dist-info/top_level.txt
+Filename: adb_connector_python-1.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: adb_connector_python-1.1.9.dist-info/RECORD
+Filename: adb_connector_python-1.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## adb_connector_python/connector.py

```diff
@@ -104,20 +104,14 @@
 def clear_cmd():
     match platform:
         case "win32":
             system("cls")
         case "linux" | "darwin":
             system("clear")
 
-try:
-    check_output("adb --version", shell=True)
-except:
-    raise CalledProcessError(127,"You have not adb installed on this pc")
-
-
 
 
 
 class Py_adb:
     """
 this is a simple low level ADB connector, you can use it for every task, such as
 debugging, automatism and even fun!
```

## Comparing `adb_connector_python-1.1.9.dist-info/LICENSE` & `adb_connector_python-1.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `adb_connector_python-1.1.9.dist-info/METADATA` & `adb_connector_python-1.2.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adb-connector-python
-Version: 1.1.9
+Version: 1.2.0
 Summary: A simple python package to interface with adb
 Author: Giuseppe Gravante
 License: MIT License
         
         Copyright (c) 2023 Giuseppe7887
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

## Comparing `adb_connector_python-1.1.9.dist-info/RECORD` & `adb_connector_python-1.2.0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-adb_connector_python/connector.py,sha256=huLeF0lFNvABonKFjE56xRQGiImhCHC9GLs1Dvu3MfQ,39197
-adb_connector_python-1.1.9.dist-info/LICENSE,sha256=I_ByMPSnNu3xgizHvEHpoes3YsmO8uQx80UpXk2oWGc,1088
-adb_connector_python-1.1.9.dist-info/METADATA,sha256=ka1Pg30YTevrWvFzvX5YGBLzzK05WXTS-mpSKHiWfhA,5452
-adb_connector_python-1.1.9.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-adb_connector_python-1.1.9.dist-info/top_level.txt,sha256=Lm728SyX737VLY8s8V37rYl62-Gs84c1b7py5lKl8Xc,21
-adb_connector_python-1.1.9.dist-info/RECORD,,
+adb_connector_python/connector.py,sha256=g6QCKQYOiOdatRPz2qLLgy73FySNK0m1fK72V3aNDqU,39056
+adb_connector_python-1.2.0.dist-info/LICENSE,sha256=I_ByMPSnNu3xgizHvEHpoes3YsmO8uQx80UpXk2oWGc,1088
+adb_connector_python-1.2.0.dist-info/METADATA,sha256=t-t2FEwi83Rlxv18T6DEFwZrZkKdPEhWrIcimw9nHpc,5452
+adb_connector_python-1.2.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+adb_connector_python-1.2.0.dist-info/top_level.txt,sha256=Lm728SyX737VLY8s8V37rYl62-Gs84c1b7py5lKl8Xc,21
+adb_connector_python-1.2.0.dist-info/RECORD,,
```

