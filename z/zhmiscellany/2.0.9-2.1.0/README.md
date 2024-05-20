# Comparing `tmp/zhmiscellany-2.0.9-py3-none-any.whl.zip` & `tmp/zhmiscellany-2.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 20142 bytes, number of entries: 18
+Zip file size: 20170 bytes, number of entries: 18
 -rw-rw-rw-  2.0 fat      236 b- defN 24-Apr-15 13:40 zhmiscellany/__init__.py
 -rw-rw-rw-  2.0 fat     6520 b- defN 23-Dec-08 14:13 zhmiscellany/_discord_supportfuncs.py
 -rw-rw-rw-  2.0 fat      673 b- defN 23-Nov-05 00:34 zhmiscellany/_misc_supportfuncs.py
 -rw-rw-rw-  2.0 fat       81 b- defN 23-Nov-01 22:45 zhmiscellany/dict.py
 -rw-rw-rw-  2.0 fat    15608 b- defN 24-Mar-07 15:37 zhmiscellany/discord.py
--rw-rw-rw-  2.0 fat     4256 b- defN 23-Nov-01 20:01 zhmiscellany/fileio.py
+-rw-rw-rw-  2.0 fat     4382 b- defN 24-May-20 17:12 zhmiscellany/fileio.py
 -rw-rw-rw-  2.0 fat      338 b- defN 23-Oct-31 21:16 zhmiscellany/image.py
 -rw-rw-rw-  2.0 fat      854 b- defN 23-Nov-14 14:55 zhmiscellany/list.py
 -rw-rw-rw-  2.0 fat      632 b- defN 23-Nov-18 07:12 zhmiscellany/math.py
 -rw-rw-rw-  2.0 fat     4531 b- defN 24-Apr-15 16:39 zhmiscellany/misc.py
 -rw-rw-rw-  2.0 fat     1687 b- defN 24-May-18 08:24 zhmiscellany/netio.py
 -rw-rw-rw-  2.0 fat     3795 b- defN 24-Apr-28 06:17 zhmiscellany/pipes.py
 -rw-rw-rw-  2.0 fat      761 b- defN 24-Feb-12 17:09 zhmiscellany/processing.py
 -rw-rw-rw-  2.0 fat     2412 b- defN 23-Nov-18 07:28 zhmiscellany/string.py
--rw-rw-rw-  2.0 fat    18861 b- defN 24-May-18 08:25 zhmiscellany-2.0.9.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-18 08:25 zhmiscellany-2.0.9.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 24-May-18 08:25 zhmiscellany-2.0.9.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1441 b- defN 24-May-18 08:25 zhmiscellany-2.0.9.dist-info/RECORD
-18 files, 62791 bytes uncompressed, 17794 bytes compressed:  71.7%
+-rw-rw-rw-  2.0 fat    18861 b- defN 24-May-20 17:12 zhmiscellany-2.1.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-20 17:12 zhmiscellany-2.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 24-May-20 17:12 zhmiscellany-2.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1441 b- defN 24-May-20 17:12 zhmiscellany-2.1.0.dist-info/RECORD
+18 files, 62917 bytes uncompressed, 17822 bytes compressed:  71.7%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: zhmiscellany/processing.py
 Comment: 
 
 Filename: zhmiscellany/string.py
 Comment: 
 
-Filename: zhmiscellany-2.0.9.dist-info/METADATA
+Filename: zhmiscellany-2.1.0.dist-info/METADATA
 Comment: 
 
-Filename: zhmiscellany-2.0.9.dist-info/WHEEL
+Filename: zhmiscellany-2.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: zhmiscellany-2.0.9.dist-info/top_level.txt
+Filename: zhmiscellany-2.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: zhmiscellany-2.0.9.dist-info/RECORD
+Filename: zhmiscellany-2.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zhmiscellany/fileio.py

```diff
@@ -122,8 +122,14 @@
 
 def read_bytes_section(file_path, section_start, section_end):
     with open(file_path, 'rb') as file:
         file.seek(section_start)  # Move the file pointer to the 'start' position
         bytes_to_read = section_end - section_start
         data = file.read(bytes_to_read)  # Read 'bytes_to_read' number of bytes
 
-    return data
+    return data
+
+
+def copy_file_with_overwrite(src, dst):
+    if os.path.exists(dst):
+        os.remove(dst)
+    shutil.copy2(src, dst)
```

## Comparing `zhmiscellany-2.0.9.dist-info/METADATA` & `zhmiscellany-2.1.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhmiscellany
-Version: 2.0.9
+Version: 2.1.0
 Summary: A collection of useful/interesting python libraries made by zh.
 Home-page: https://discord.gg/ThBBAuueVJ
 Author: zh
 Author-email: imnotgivingmyemailjustaddmeondiscordmydiscordisz_h_@zh.com
 Project-URL: Bug Tracker, https://github.com/zen-ham/zhmiscellany/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `zhmiscellany-2.0.9.dist-info/RECORD` & `zhmiscellany-2.1.0.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 zhmiscellany/__init__.py,sha256=B_bSZHCIbiiraewwok9mCtKJM2jzU9qomo5byh53z34,236
 zhmiscellany/_discord_supportfuncs.py,sha256=OIO40DDGgAPNCifP9VQsHH4p4P_NuLq-RC377k1LTW8,6520
 zhmiscellany/_misc_supportfuncs.py,sha256=H8VZ8vEhH5kC9df488j-MuQmxS8v5Xjc6RHBtE5UrKM,673
 zhmiscellany/dict.py,sha256=0BZJ5eK-MurAHYV1OPa0jdGTr-QEWos7ZM0npb-tN9I,81
 zhmiscellany/discord.py,sha256=Re-fUdc_OA-9tzvd3VX_w7lBNvFpg3Tg5mVyIQ83IKA,15608
-zhmiscellany/fileio.py,sha256=q5noOhvPxyHxSy56sawW0X91qwHM2xuU8CYzfJN5O08,4256
+zhmiscellany/fileio.py,sha256=ATfxWFvdYxsQ_aD2Er1UgMrEjlT4e1tg3Ev1kHRs2GQ,4382
 zhmiscellany/image.py,sha256=uOXFcGG1FhvNeCU7dm6DYxefh6suiL8qg8qtAVyezew,338
 zhmiscellany/list.py,sha256=2kqsscSFXEanmEdR1NuwWaf2l8nPTDUgRyrfL1snoRg,854
 zhmiscellany/math.py,sha256=v2WmHdKrwsrY08E6yUgb0nPHbTuyrljRdgUMw5uqu3U,632
 zhmiscellany/misc.py,sha256=JlibUEtNHc3nHDnlgyOE3050SIQkcMMedPK8WZookNU,4531
 zhmiscellany/netio.py,sha256=UiMQFsdpPx2Kst-YDxYrz_Ivsnq455LNTKQRCi-aZwY,1687
 zhmiscellany/pipes.py,sha256=PxO4aykFzC60xbTQuc66KzZYIxiW0KPebXZbncD2HcU,3795
 zhmiscellany/processing.py,sha256=pE2LVtaZwBvWgd6Xx0S_ZT0WhcKr6GtBhjAfbAflSYo,761
 zhmiscellany/string.py,sha256=2xL_rbJeiGH14k_JkXWUp-oBN30Ltl9-bZk0eHUPltA,2412
-zhmiscellany-2.0.9.dist-info/METADATA,sha256=vGFDjFDK2s6iINdYZPtEQYoh0jssms2t7YbRtsZC1JE,18861
-zhmiscellany-2.0.9.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-zhmiscellany-2.0.9.dist-info/top_level.txt,sha256=ioDtsrevCI52rTxZntMPljRIBsZs73tD0hI00HektiE,13
-zhmiscellany-2.0.9.dist-info/RECORD,,
+zhmiscellany-2.1.0.dist-info/METADATA,sha256=qT53LuyMeufbpQRp9tH7icNwv9QgNOPXSdEv8C7SqtA,18861
+zhmiscellany-2.1.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+zhmiscellany-2.1.0.dist-info/top_level.txt,sha256=ioDtsrevCI52rTxZntMPljRIBsZs73tD0hI00HektiE,13
+zhmiscellany-2.1.0.dist-info/RECORD,,
```

