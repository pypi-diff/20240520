# Comparing `tmp/ydata_datascience-0.5.0rc1-py2.py3-none-any.whl.zip` & `tmp/ydata_datascience-0.5.0rc3-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
 Zip file size: 2680 bytes, number of entries: 7
--rw-r--r--  2.0 unx        0 b- defN 23-Dec-14 18:53 ydata/datascience/__init__.py
--rw-r--r--  2.0 unx       67 b- defN 23-Dec-14 18:53 ydata/datascience/common/__init__.py
--rw-r--r--  2.0 unx      660 b- defN 23-Dec-14 18:53 ydata/datascience/common/privacy.py
--rw-r--r--  2.0 unx     1499 b- defN 23-Dec-14 18:53 ydata_datascience-0.5.0rc1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Dec-14 18:53 ydata_datascience-0.5.0rc1.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Dec-14 18:53 ydata_datascience-0.5.0rc1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      615 b- defN 23-Dec-14 18:53 ydata_datascience-0.5.0rc1.dist-info/RECORD
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-16 23:41 ydata/datascience/__init__.py
+-rw-r--r--  2.0 unx       67 b- defN 24-Jan-16 23:41 ydata/datascience/common/__init__.py
+-rw-r--r--  2.0 unx      660 b- defN 24-Jan-16 23:41 ydata/datascience/common/privacy.py
+-rw-r--r--  2.0 unx     1499 b- defN 24-Jan-16 23:41 ydata_datascience-0.5.0rc3.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-Jan-16 23:41 ydata_datascience-0.5.0rc3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 24-Jan-16 23:41 ydata_datascience-0.5.0rc3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      615 b- defN 24-Jan-16 23:41 ydata_datascience-0.5.0rc3.dist-info/RECORD
 7 files, 2957 bytes uncompressed, 1566 bytes compressed:  47.0%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: ydata/datascience/common/__init__.py
 Comment: 
 
 Filename: ydata/datascience/common/privacy.py
 Comment: 
 
-Filename: ydata_datascience-0.5.0rc1.dist-info/METADATA
+Filename: ydata_datascience-0.5.0rc3.dist-info/METADATA
 Comment: 
 
-Filename: ydata_datascience-0.5.0rc1.dist-info/WHEEL
+Filename: ydata_datascience-0.5.0rc3.dist-info/WHEEL
 Comment: 
 
-Filename: ydata_datascience-0.5.0rc1.dist-info/top_level.txt
+Filename: ydata_datascience-0.5.0rc3.dist-info/top_level.txt
 Comment: 
 
-Filename: ydata_datascience-0.5.0rc1.dist-info/RECORD
+Filename: ydata_datascience-0.5.0rc3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ydata_datascience-0.5.0rc1.dist-info/METADATA` & `ydata_datascience-0.5.0rc3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ydata-datascience
-Version: 0.5.0rc1
+Version: 0.5.0rc3
 Summary: Data science functionalities for all python packages at YData
 Home-page: https://github.com/ydataai/python-core
 Author: YData
 Author-email: developers@ydata.ai
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

## Comparing `ydata_datascience-0.5.0rc1.dist-info/RECORD` & `ydata_datascience-0.5.0rc3.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 ydata/datascience/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ydata/datascience/common/__init__.py,sha256=446ZR8dqVUXB_73pBEt4-P5Z2ALFbut2wMSa9902D7I,67
 ydata/datascience/common/privacy.py,sha256=rJ6Ii4iAzcYbVmtmNxh7DaNgiz_GwRxQnOa6S281Hvg,660
-ydata_datascience-0.5.0rc1.dist-info/METADATA,sha256=chUoQByNqjkDahX-0sA0poaCr2bYsrX-9oI0IRUINnM,1499
-ydata_datascience-0.5.0rc1.dist-info/WHEEL,sha256=-G_t0oGuE7UD0DrSpVZnq1hHMBV9DD2XkS5v7XpmTnk,110
-ydata_datascience-0.5.0rc1.dist-info/top_level.txt,sha256=s4ySCHuzMHwZ8NeXGj2CkDdJaGLv0YzfNsi3JW3V8gQ,6
-ydata_datascience-0.5.0rc1.dist-info/RECORD,,
+ydata_datascience-0.5.0rc3.dist-info/METADATA,sha256=G6u4iDAOPJRB8eGhtzYuOJwvR5IhkYNtg2RUZHpc2fc,1499
+ydata_datascience-0.5.0rc3.dist-info/WHEEL,sha256=-G_t0oGuE7UD0DrSpVZnq1hHMBV9DD2XkS5v7XpmTnk,110
+ydata_datascience-0.5.0rc3.dist-info/top_level.txt,sha256=s4ySCHuzMHwZ8NeXGj2CkDdJaGLv0YzfNsi3JW3V8gQ,6
+ydata_datascience-0.5.0rc3.dist-info/RECORD,,
```

