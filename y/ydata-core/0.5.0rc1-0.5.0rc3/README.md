# Comparing `tmp/ydata_core-0.5.0rc1-py2.py3-none-any.whl.zip` & `tmp/ydata_core-0.5.0rc3-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,14 @@
-Zip file size: 4289 bytes, number of entries: 11
--rw-r--r--  2.0 unx        0 b- defN 23-Dec-14 18:53 ydata/core/__init__.py
--rw-r--r--  2.0 unx       59 b- defN 23-Dec-14 18:53 ydata/core/connectors/__init__.py
--rw-r--r--  2.0 unx      134 b- defN 23-Dec-14 18:53 ydata/core/connectors/write_mode.py
--rw-r--r--  2.0 unx       67 b- defN 23-Dec-14 18:53 ydata/core/enum/__init__.py
--rw-r--r--  2.0 unx      722 b- defN 23-Dec-14 18:53 ydata/core/enum/string_enum.py
--rw-r--r--  2.0 unx       70 b- defN 23-Dec-14 18:53 ydata/core/error/__init__.py
--rw-r--r--  2.0 unx     2076 b- defN 23-Dec-14 18:53 ydata/core/error/fabric_error.py
--rw-r--r--  2.0 unx     1482 b- defN 23-Dec-14 18:53 ydata_core-0.5.0rc1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Dec-14 18:53 ydata_core-0.5.0rc1.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Dec-14 18:53 ydata_core-0.5.0rc1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      917 b- defN 23-Dec-14 18:53 ydata_core-0.5.0rc1.dist-info/RECORD
-11 files, 5643 bytes uncompressed, 2713 bytes compressed:  51.9%
+Zip file size: 4615 bytes, number of entries: 12
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-16 23:41 ydata/core/__init__.py
+-rw-r--r--  2.0 unx      113 b- defN 24-Jan-16 23:41 ydata/core/datatype.py
+-rw-r--r--  2.0 unx       59 b- defN 24-Jan-16 23:41 ydata/core/connectors/__init__.py
+-rw-r--r--  2.0 unx      134 b- defN 24-Jan-16 23:41 ydata/core/connectors/write_mode.py
+-rw-r--r--  2.0 unx       67 b- defN 24-Jan-16 23:41 ydata/core/enum/__init__.py
+-rw-r--r--  2.0 unx      722 b- defN 24-Jan-16 23:41 ydata/core/enum/string_enum.py
+-rw-r--r--  2.0 unx       70 b- defN 24-Jan-16 23:41 ydata/core/error/__init__.py
+-rw-r--r--  2.0 unx     2210 b- defN 24-Jan-16 23:41 ydata/core/error/fabric_error.py
+-rw-r--r--  2.0 unx     1482 b- defN 24-Jan-16 23:41 ydata_core-0.5.0rc3.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-Jan-16 23:41 ydata_core-0.5.0rc3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 24-Jan-16 23:41 ydata_core-0.5.0rc3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      995 b- defN 24-Jan-16 23:41 ydata_core-0.5.0rc3.dist-info/RECORD
+12 files, 5968 bytes uncompressed, 2919 bytes compressed:  51.1%
```

## zipnote {}

```diff
@@ -1,10 +1,13 @@
 Filename: ydata/core/__init__.py
 Comment: 
 
+Filename: ydata/core/datatype.py
+Comment: 
+
 Filename: ydata/core/connectors/__init__.py
 Comment: 
 
 Filename: ydata/core/connectors/write_mode.py
 Comment: 
 
 Filename: ydata/core/enum/__init__.py
@@ -15,20 +18,20 @@
 
 Filename: ydata/core/error/__init__.py
 Comment: 
 
 Filename: ydata/core/error/fabric_error.py
 Comment: 
 
-Filename: ydata_core-0.5.0rc1.dist-info/METADATA
+Filename: ydata_core-0.5.0rc3.dist-info/METADATA
 Comment: 
 
-Filename: ydata_core-0.5.0rc1.dist-info/WHEEL
+Filename: ydata_core-0.5.0rc3.dist-info/WHEEL
 Comment: 
 
-Filename: ydata_core-0.5.0rc1.dist-info/top_level.txt
+Filename: ydata_core-0.5.0rc3.dist-info/top_level.txt
 Comment: 
 
-Filename: ydata_core-0.5.0rc1.dist-info/RECORD
+Filename: ydata_core-0.5.0rc3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ydata/core/error/fabric_error.py

```diff
@@ -4,15 +4,15 @@
 
 
 def _camelcased(value: str) -> str:
   capitalized = ''.join(x.capitalize() for x in value.split('_'))
   return capitalized[0].lower() + capitalized[1:]
 
 
-# pylint: disable=too-many-arguments
+# pylint: disable=too-many-arguments, import-outside-toplevel
 class FabricError(Exception):
   context: dict[str, str] | None
   description: str
   http_code: int = 500
   name: str | None
   return_value: int
 
@@ -39,22 +39,24 @@
       "context": self.context,
       "name": self.name if self.name else self.__class__.__name__,
       "description": self.description,
       "http_code": self.http_code,
       "return_value": self.return_value
     }.items()
 
-  def __str__(self) -> str:
-    return f'''
-      {self.__class__.__name__}(name={self.name}, context={self.context}, description={self.description}, \
-http_code={self.http_code}, return_value={self.return_value})
-    '''
-
   def __repr__(self) -> str:
-    return self.__str__()
+    from pprint import pformat
+    return f"{self.__class__.__name__}(\n{pformat(dict(self), width=120, sort_dicts=False)}\n)"
+
+  def __str__(self) -> str:
+    from pprint import pformat
+    string = f"{self.name} - {self.description}"
+    if self.context:
+      string += f"\ncontext: {pformat(self.context, width=160, sort_dicts=False)}"
+    return string
 
   def __sizeof__(self) -> int:
     context_size = getsizeof(self.context) if self.context else 0
     http_code_size = getsizeof(str(self.http_code)) if self.http_code else 0
     return_value_size = getsizeof(str(self.return_value)) if self.return_value else 0
 
     return context_size \
```

## Comparing `ydata_core-0.5.0rc1.dist-info/METADATA` & `ydata_core-0.5.0rc3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ydata-core
-Version: 0.5.0rc1
+Version: 0.5.0rc3
 Summary: Core functionality for all python packages at YData
 Home-page: https://github.com/ydataai/python-core
 Author: YData
 Author-email: developers@ydata.ai
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

## Comparing `ydata_core-0.5.0rc1.dist-info/RECORD` & `ydata_core-0.5.0rc3.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 ydata/core/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ydata/core/datatype.py,sha256=JpnRoHMtWyy5EbwCI8GoZaUONG06y4Jp-LR3q8QGQP4,113
 ydata/core/connectors/__init__.py,sha256=rsifccFDjMFl71_MOEzejh-4lOLbgHLdgtrHd8l6efw,59
 ydata/core/connectors/write_mode.py,sha256=uUZMVD6yx3GJLR7_dLJyIOHrVZO1WaSjpulZA23aN-M,134
 ydata/core/enum/__init__.py,sha256=R5LgZ-ZFiZJGW19f8ejDodDf6EZjSJ0a_LXxIyhkOdo,67
 ydata/core/enum/string_enum.py,sha256=gwSPIzkPJoKXNEe8hAnVUGReVmLIakWkcXD4Dqg6rxY,722
 ydata/core/error/__init__.py,sha256=tA7nd8DVnbFyTexySXzNXDhmloFjPKzjJ_Wmz2IBl-Y,70
-ydata/core/error/fabric_error.py,sha256=uubh_7_WCb4JfqYfGWvxlwiWnRk0HdapdElOsS0o86w,2076
-ydata_core-0.5.0rc1.dist-info/METADATA,sha256=qce6k3s_V6vN53FmeIsK8HbPYBRt_Ge8XpAlfAA4lnQ,1482
-ydata_core-0.5.0rc1.dist-info/WHEEL,sha256=-G_t0oGuE7UD0DrSpVZnq1hHMBV9DD2XkS5v7XpmTnk,110
-ydata_core-0.5.0rc1.dist-info/top_level.txt,sha256=s4ySCHuzMHwZ8NeXGj2CkDdJaGLv0YzfNsi3JW3V8gQ,6
-ydata_core-0.5.0rc1.dist-info/RECORD,,
+ydata/core/error/fabric_error.py,sha256=zslDH4krJvwI7SwazErCGHCEi8VyLGKP50fwJy-c3Ho,2210
+ydata_core-0.5.0rc3.dist-info/METADATA,sha256=rv0LqBwiO7KXrjK9pMwZpBba2tZ8Q2BYr8SFCATlii0,1482
+ydata_core-0.5.0rc3.dist-info/WHEEL,sha256=-G_t0oGuE7UD0DrSpVZnq1hHMBV9DD2XkS5v7XpmTnk,110
+ydata_core-0.5.0rc3.dist-info/top_level.txt,sha256=s4ySCHuzMHwZ8NeXGj2CkDdJaGLv0YzfNsi3JW3V8gQ,6
+ydata_core-0.5.0rc3.dist-info/RECORD,,
```

