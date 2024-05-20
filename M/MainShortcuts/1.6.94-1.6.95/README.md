# Comparing `tmp/mainshortcuts-1.6.94.tar.gz` & `tmp/mainshortcuts-1.6.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mainshortcuts-1.6.94.tar", max compression
+gzip compressed data, was "mainshortcuts-1.6.95.tar", max compression
```

## Comparing `mainshortcuts-1.6.94.tar` & `mainshortcuts-1.6.95.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rwxr-xr-x   0        0        0     2788 2024-03-02 06:10:12.000000 mainshortcuts-1.6.94/README.md
--rwxr-xr-x   0        0        0      696 2024-05-16 11:08:56.000000 mainshortcuts-1.6.94/pyproject.toml
--rwxr-xr-x   0        0        0     5954 2024-05-08 16:40:54.000000 mainshortcuts-1.6.94/src/MainShortcuts/MainCore.py
--rwxr-xr-x   0        0        0     1025 2024-05-16 11:08:51.000000 mainshortcuts-1.6.94/src/MainShortcuts/__init__.py
--rwxr-xr-x   0        0        0      495 2024-05-08 16:41:02.000000 mainshortcuts-1.6.94/src/MainShortcuts/addon.py
--rwxr-xr-x   0        0        0     4958 2024-05-08 16:41:08.000000 mainshortcuts-1.6.94/src/MainShortcuts/cfg.py
--rwxr-xr-x   0        0        0     1057 2024-05-08 16:41:00.000000 mainshortcuts-1.6.94/src/MainShortcuts/dict.py
--rwxr-xr-x   0        0        0     1538 2024-05-08 16:41:02.000000 mainshortcuts-1.6.94/src/MainShortcuts/dictplus.py
--rwxr-xr-x   0        0        0     4189 2024-05-16 08:59:32.000000 mainshortcuts-1.6.94/src/MainShortcuts/dir.py
--rwxr-xr-x   0        0        0     3043 2024-05-08 16:40:46.000000 mainshortcuts-1.6.94/src/MainShortcuts/file.py
--rwxr-xr-x   0        0        0     6183 2024-05-08 16:41:04.000000 mainshortcuts-1.6.94/src/MainShortcuts/fileobj.py
--rwxr-xr-x   0        0        0     3659 2024-05-16 11:09:00.000000 mainshortcuts-1.6.94/src/MainShortcuts/imports.py
--rwxr-xr-x   0        0        0     3948 2024-05-09 14:07:38.000000 mainshortcuts-1.6.94/src/MainShortcuts/json.py
--rwxr-xr-x   0        0        0     2292 2024-05-08 16:41:06.000000 mainshortcuts-1.6.94/src/MainShortcuts/list.py
--rwxr-xr-x   0        0        0     1073 2024-05-08 16:40:46.000000 mainshortcuts-1.6.94/src/MainShortcuts/main.py
--rwxr-xr-x   0        0        0       93 2024-05-08 16:40:46.000000 mainshortcuts-1.6.94/src/MainShortcuts/os.py
--rwxr-xr-x   0        0        0     6585 2024-05-08 16:40:58.000000 mainshortcuts-1.6.94/src/MainShortcuts/path.py
--rwxr-xr-x   0        0        0      857 2024-05-08 16:41:06.000000 mainshortcuts-1.6.94/src/MainShortcuts/proc.py
--rwxr-xr-x   0        0        0     1507 2024-05-08 16:40:50.000000 mainshortcuts-1.6.94/src/MainShortcuts/script.py
--rwxr-xr-x   0        0        0     1047 2024-05-08 16:41:08.000000 mainshortcuts-1.6.94/src/MainShortcuts/str.py
--rwxr-xr-x   0        0        0    15238 2024-05-08 16:40:50.000000 mainshortcuts-1.6.94/src/MainShortcuts/values.py
--rwxr-xr-x   0        0        0     1327 2024-05-08 16:41:00.000000 mainshortcuts-1.6.94/src/MainShortcuts/win.py
--rw-r--r--   0        0        0     3510 1970-01-01 00:00:00.000000 mainshortcuts-1.6.94/PKG-INFO
+-rwxr-xr-x   0        0        0     2788 2024-03-02 06:10:12.000000 mainshortcuts-1.6.95/README.md
+-rwxr-xr-x   0        0        0      696 2024-05-20 12:11:57.000000 mainshortcuts-1.6.95/pyproject.toml
+-rwxr-xr-x   0        0        0     5954 2024-05-08 16:40:54.000000 mainshortcuts-1.6.95/src/MainShortcuts/MainCore.py
+-rwxr-xr-x   0        0        0     1025 2024-05-20 12:11:52.000000 mainshortcuts-1.6.95/src/MainShortcuts/__init__.py
+-rwxr-xr-x   0        0        0      495 2024-05-08 16:41:02.000000 mainshortcuts-1.6.95/src/MainShortcuts/addon.py
+-rwxr-xr-x   0        0        0     4975 2024-05-20 12:11:29.000000 mainshortcuts-1.6.95/src/MainShortcuts/cfg.py
+-rwxr-xr-x   0        0        0     1057 2024-05-08 16:41:00.000000 mainshortcuts-1.6.95/src/MainShortcuts/dict.py
+-rwxr-xr-x   0        0        0     1538 2024-05-08 16:41:02.000000 mainshortcuts-1.6.95/src/MainShortcuts/dictplus.py
+-rwxr-xr-x   0        0        0     4189 2024-05-16 08:59:32.000000 mainshortcuts-1.6.95/src/MainShortcuts/dir.py
+-rwxr-xr-x   0        0        0     3043 2024-05-08 16:40:46.000000 mainshortcuts-1.6.95/src/MainShortcuts/file.py
+-rwxr-xr-x   0        0        0     6183 2024-05-08 16:41:04.000000 mainshortcuts-1.6.95/src/MainShortcuts/fileobj.py
+-rwxr-xr-x   0        0        0     3659 2024-05-20 12:12:01.000000 mainshortcuts-1.6.95/src/MainShortcuts/imports.py
+-rwxr-xr-x   0        0        0     3948 2024-05-09 14:07:38.000000 mainshortcuts-1.6.95/src/MainShortcuts/json.py
+-rwxr-xr-x   0        0        0     2292 2024-05-08 16:41:06.000000 mainshortcuts-1.6.95/src/MainShortcuts/list.py
+-rwxr-xr-x   0        0        0     1073 2024-05-08 16:40:46.000000 mainshortcuts-1.6.95/src/MainShortcuts/main.py
+-rwxr-xr-x   0        0        0       93 2024-05-08 16:40:46.000000 mainshortcuts-1.6.95/src/MainShortcuts/os.py
+-rwxr-xr-x   0        0        0     6585 2024-05-08 16:40:58.000000 mainshortcuts-1.6.95/src/MainShortcuts/path.py
+-rwxr-xr-x   0        0        0      857 2024-05-08 16:41:06.000000 mainshortcuts-1.6.95/src/MainShortcuts/proc.py
+-rwxr-xr-x   0        0        0     1507 2024-05-08 16:40:50.000000 mainshortcuts-1.6.95/src/MainShortcuts/script.py
+-rwxr-xr-x   0        0        0     1047 2024-05-08 16:41:08.000000 mainshortcuts-1.6.95/src/MainShortcuts/str.py
+-rwxr-xr-x   0        0        0    15238 2024-05-08 16:40:50.000000 mainshortcuts-1.6.95/src/MainShortcuts/values.py
+-rwxr-xr-x   0        0        0     1327 2024-05-08 16:41:00.000000 mainshortcuts-1.6.95/src/MainShortcuts/win.py
+-rw-r--r--   0        0        0     3510 1970-01-01 00:00:00.000000 mainshortcuts-1.6.95/PKG-INFO
```

### Comparing `mainshortcuts-1.6.94/README.md` & `mainshortcuts-1.6.95/README.md`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.94/pyproject.toml` & `mainshortcuts-1.6.95/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tool.poetry]
-version = "1.6.94"
+version = "1.6.95"
 name = "MainShortcuts"
 description = "Simplifying Python Built-in Commands"
 authors = [ "MainPlay TG <xbox.roman6666666666@gmail.com>",]
 readme = "README.md"
 repository = "https://github.com/MainPlay-TG/MainShortcuts.py"
 packages = [
     { include = "MainShortcuts", from = "src" },
```

### Comparing `mainshortcuts-1.6.94/src/MainShortcuts/MainCore.py` & `mainshortcuts-1.6.95/src/MainShortcuts/MainCore.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.94/src/MainShortcuts/__init__.py` & `mainshortcuts-1.6.95/src/MainShortcuts/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """MainShortcuts - \u043D\u0435\u0431\u043E\u043B\u044C\u0448\u0430\u044F \u0431\u0438\u0431\u043B\u0438\u043E\u0442\u0435\u043A\u0430 \u0434\u043B\u044F \u0443\u043F\u0440\u043E\u0449\u0435\u043D\u0438\u044F \u043D\u0430\u043F\u0438\u0441\u0430\u043D\u0438\u044F \u043A\u043E\u0434\u0430
 \u0420\u0430\u0437\u0440\u0430\u0431\u043E\u0442\u0447\u0438\u043A: MainPlay TG
 https://t.me/MainPlay_InfoCh"""
 
-__version_tuple__ = (1, 6, 94)
+__version_tuple__ = (1, 6, 95)
 __depends__ = {
     "required": [
         "json",
         "os",
         "platform",
         "shutil",
         "subprocess",
```

### Comparing `mainshortcuts-1.6.94/src/MainShortcuts/cfg.py` & `mainshortcuts-1.6.95/src/MainShortcuts/cfg.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
   def __init__(self, path: str, data: dict = {}, default: dict = {}, type: str = "auto"):
     """Аргументы:
     path - путь к файлу, в котором нужно хранить данные
     data - заранее указанные данные
     default - значения по умолчанию
     type - тип хранения (по умолчанию от расширения файла)"""
-    self.path = path
+    self.path = os.path.abspath(path)
     self.data = data
     self.default = default
     self.type = _checkType(path, type)
     _checkImport(self.type)
 
   def __getitem__(self, k):
     return self.data[k]
```

### Comparing `mainshortcuts-1.6.94/src/MainShortcuts/dict.py` & `mainshortcuts-1.6.95/src/MainShortcuts/dict.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.94/src/MainShortcuts/dictplus.py` & `mainshortcuts-1.6.95/src/MainShortcuts/dictplus.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.94/src/MainShortcuts/dir.py` & `mainshortcuts-1.6.95/src/MainShortcuts/dir.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.94/src/MainShortcuts/file.py` & `mainshortcuts-1.6.95/src/MainShortcuts/file.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.94/src/MainShortcuts/fileobj.py` & `mainshortcuts-1.6.95/src/MainShortcuts/fileobj.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.94/src/MainShortcuts/imports.py` & `mainshortcuts-1.6.95/src/MainShortcuts/imports.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.94/src/MainShortcuts/json.py` & `mainshortcuts-1.6.95/src/MainShortcuts/json.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.94/src/MainShortcuts/list.py` & `mainshortcuts-1.6.95/src/MainShortcuts/list.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.94/src/MainShortcuts/main.py` & `mainshortcuts-1.6.95/src/MainShortcuts/main.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.94/src/MainShortcuts/path.py` & `mainshortcuts-1.6.95/src/MainShortcuts/path.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.94/src/MainShortcuts/proc.py` & `mainshortcuts-1.6.95/src/MainShortcuts/proc.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.94/src/MainShortcuts/script.py` & `mainshortcuts-1.6.95/src/MainShortcuts/script.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.94/src/MainShortcuts/str.py` & `mainshortcuts-1.6.95/src/MainShortcuts/str.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.94/src/MainShortcuts/values.py` & `mainshortcuts-1.6.95/src/MainShortcuts/values.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.94/src/MainShortcuts/win.py` & `mainshortcuts-1.6.95/src/MainShortcuts/win.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.94/PKG-INFO` & `mainshortcuts-1.6.95/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MainShortcuts
-Version: 1.6.94
+Version: 1.6.95
 Summary: Simplifying Python Built-in Commands
 Home-page: https://github.com/MainPlay-TG/MainShortcuts.py
 Author: MainPlay TG
 Author-email: xbox.roman6666666666@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

