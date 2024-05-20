# Comparing `tmp/viewstate-0.5.3.tar.gz` & `tmp/viewstate-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/viewstate-0.5.3.tar", last modified: Sat Feb  1 12:45:38 2020, max compression
+gzip compressed data, was "viewstate-0.6.0.tar", max compression
```

## Comparing `viewstate-0.5.3.tar` & `viewstate-0.6.0.tar`

### file list

```diff
@@ -1,19 +1,10 @@
-drwxr-xr-x   0 yuval     (1000) yuval     (1000)        0 2020-02-01 12:45:38.072594 viewstate-0.5.3/
--rw-r--r--   0 yuval     (1000) yuval     (1000)     1068 2020-02-01 06:08:45.000000 viewstate-0.5.3/LICENSE
--rw-r--r--   0 yuval     (1000) yuval     (1000)       15 2020-02-01 06:08:45.000000 viewstate-0.5.3/MANIFEST.in
--rw-r--r--   0 yuval     (1000) yuval     (1000)     4738 2020-02-01 12:45:38.072594 viewstate-0.5.3/PKG-INFO
--rw-r--r--   0 yuval     (1000) yuval     (1000)     3154 2020-02-01 12:26:42.000000 viewstate-0.5.3/README.rst
--rw-r--r--   0 yuval     (1000) yuval     (1000)      102 2020-02-01 12:45:38.072594 viewstate-0.5.3/setup.cfg
--rw-r--r--   0 yuval     (1000) yuval     (1000)     1043 2020-02-01 12:44:51.000000 viewstate-0.5.3/setup.py
-drwxr-xr-x   0 yuval     (1000) yuval     (1000)        0 2020-02-01 12:45:38.072594 viewstate-0.5.3/viewstate/
--rw-r--r--   0 yuval     (1000) yuval     (1000)       76 2020-02-01 11:34:13.000000 viewstate-0.5.3/viewstate/__init__.py
--rw-r--r--   0 yuval     (1000) yuval     (1000)      387 2020-02-01 11:34:13.000000 viewstate-0.5.3/viewstate/__main__.py
--rw-r--r--   0 yuval     (1000) yuval     (1000)     3152 2020-02-01 12:37:53.000000 viewstate-0.5.3/viewstate/colors.py
--rw-r--r--   0 yuval     (1000) yuval     (1000)       46 2020-02-01 11:34:13.000000 viewstate-0.5.3/viewstate/exceptions.py
--rw-r--r--   0 yuval     (1000) yuval     (1000)     5660 2020-02-01 12:37:53.000000 viewstate-0.5.3/viewstate/parse.py
--rw-r--r--   0 yuval     (1000) yuval     (1000)     1498 2020-02-01 11:34:13.000000 viewstate-0.5.3/viewstate/viewstate.py
-drwxr-xr-x   0 yuval     (1000) yuval     (1000)        0 2020-02-01 12:45:38.072594 viewstate-0.5.3/viewstate.egg-info/
--rw-r--r--   0 yuval     (1000) yuval     (1000)     4738 2020-02-01 12:45:37.000000 viewstate-0.5.3/viewstate.egg-info/PKG-INFO
--rw-r--r--   0 yuval     (1000) yuval     (1000)      311 2020-02-01 12:45:38.000000 viewstate-0.5.3/viewstate.egg-info/SOURCES.txt
--rw-r--r--   0 yuval     (1000) yuval     (1000)        1 2020-02-01 12:45:37.000000 viewstate-0.5.3/viewstate.egg-info/dependency_links.txt
--rw-r--r--   0 yuval     (1000) yuval     (1000)       10 2020-02-01 12:45:37.000000 viewstate-0.5.3/viewstate.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1068 2020-12-15 07:26:25.384433 viewstate-0.6.0/LICENSE
+-rw-r--r--   0        0        0     3154 2021-04-28 08:09:24.684016 viewstate-0.6.0/README.rst
+-rw-r--r--   0        0        0      369 2024-05-20 10:30:21.213021 viewstate-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      120 2024-05-20 10:30:21.213021 viewstate-0.6.0/viewstate/__init__.py
+-rw-r--r--   0        0        0      387 2020-12-15 07:26:25.387766 viewstate-0.6.0/viewstate/__main__.py
+-rw-r--r--   0        0        0     3152 2021-04-28 08:09:24.684016 viewstate-0.6.0/viewstate/colors.py
+-rw-r--r--   0        0        0       46 2020-12-15 07:26:25.387766 viewstate-0.6.0/viewstate/exceptions.py
+-rw-r--r--   0        0        0     5886 2024-05-20 10:30:21.213021 viewstate-0.6.0/viewstate/parse.py
+-rw-r--r--   0        0        0     1480 2024-05-20 10:30:21.213021 viewstate-0.6.0/viewstate/viewstate.py
+-rw-r--r--   0        0        0     3717 1970-01-01 00:00:00.000000 viewstate-0.6.0/PKG-INFO
```

### Comparing `viewstate-0.5.3/LICENSE` & `viewstate-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `viewstate-0.5.3/README.rst` & `viewstate-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `viewstate-0.5.3/viewstate/colors.py` & `viewstate-0.6.0/viewstate/colors.py`

 * *Files identical despite different names*

### Comparing `viewstate-0.5.3/viewstate/parse.py` & `viewstate-0.6.0/viewstate/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,35 +177,35 @@
 
 class StringArray(Parser):
     marker = 0x15
 
     @staticmethod
     def parse(b):
         n, remain = Integer.parse(b)
-        l = []
+        lst = []
         for _ in range(n):
             if not remain[0]:
                 val, remain = "", remain[1:]
             else:
                 val, remain = String.parse(remain)
-            l.append(val)
-        return l, remain
+            lst.append(val)
+        return lst, remain
 
 
 class Array(Parser):
     marker = 0x16
 
     @staticmethod
     def parse(b):
         n, remain = Integer.parse(b)
-        l = []
+        lst = []
         for _ in range(n):
             val, remain = Parser.parse(remain)
-            l.append(val)
-        return l, remain
+            lst.append(val)
+        return lst, remain
 
 
 class StringRef(Parser):
     marker = 0x1F
 
     @staticmethod
     def parse(b):
@@ -227,20 +227,20 @@
     marker = 0x3C
 
     @staticmethod
     def parse(b):
         type, remain = Parser.parse(b)
         length, remain = Integer.parse(remain)
         n, remain = Integer.parse(remain)
-        l = [None] * length
+        lst = [None] * length
         for _ in range(n):
             idx, remain = Integer.parse(remain)
             val, remain = Parser.parse(remain)
-            l[idx] = val
-        return l, remain
+            lst[idx] = val
+        return lst, remain
 
 
 class Dict(Parser):
     marker = 0x18
 
     @staticmethod
     def parse(b):
@@ -257,12 +257,22 @@
 class TypedArray(Parser):
     marker = 0x14
 
     @staticmethod
     def parse(b):
         typeval, remain = Parser.parse(b)
         n, remain = Integer.parse(remain)
-        l = []
+        lst = []
         for _ in range(n):
             val, remain = Parser.parse(remain)
-            l.append(val)
-        return l, remain
+            lst.append(val)
+        return lst, remain
+
+
+class BinaryFormatted(Parser):
+    marker = 0x32
+
+    @staticmethod
+    def parse(b):
+        n, remain = Integer.parse(b)
+        val = remain[:n]
+        return "Binary: {}".format(val), remain[n:]
```

### Comparing `viewstate-0.5.3/viewstate/viewstate.py` & `viewstate-0.6.0/viewstate/viewstate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from base64 import b64decode, b64encode
+from base64 import b64decode
 from binascii import Error as BinAsciiError
 
 from .exceptions import ViewStateException
 from .parse import Parser
 
 
 class ViewState(object):
     def __init__(self, base64=None, raw=None):
         if base64:
             self.base64 = base64
             try:
                 self.raw = b64decode(self.base64)
-            except BinAsciiError as bae:
+            except BinAsciiError:
                 raise ViewStateException("Cannot decode base64 input")
         elif raw:
             self.raw = raw
         self.decoded = None
         self.mac = None
         self.signature = None
```

