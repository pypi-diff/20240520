# Comparing `tmp/LogTranslate-1.4.0.tar.gz` & `tmp/LogTranslate-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LogTranslate-1.4.0.tar", last modified: Fri May 17 13:10:13 2024, max compression
+gzip compressed data, was "LogTranslate-1.4.1.tar", last modified: Mon May 20 12:31:10 2024, max compression
```

## Comparing `LogTranslate-1.4.0.tar` & `LogTranslate-1.4.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 13:10:13.318383 LogTranslate-1.4.0/
--rw-rw-rw-   0        0        0     1079 2023-06-28 15:23:37.000000 LogTranslate-1.4.0/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2024-05-17 13:10:13.300499 LogTranslate-1.4.0/LogTranslate.egg-info/
--rw-rw-rw-   0        0        0     3183 2024-05-17 13:10:13.000000 LogTranslate-1.4.0/LogTranslate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      623 2024-05-17 13:10:13.000000 LogTranslate-1.4.0/LogTranslate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 13:10:13.000000 LogTranslate-1.4.0/LogTranslate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-05-17 13:10:13.000000 LogTranslate-1.4.0/LogTranslate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-17 13:10:13.000000 LogTranslate-1.4.0/LogTranslate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3183 2024-05-17 13:10:13.318383 LogTranslate-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     2474 2023-06-28 15:23:37.000000 LogTranslate-1.4.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 13:10:13.311267 LogTranslate-1.4.0/log_translate/
--rw-rw-rw-   0        0        0        0 2023-06-28 15:23:37.000000 LogTranslate-1.4.0/log_translate/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:10:13.314356 LogTranslate-1.4.0/log_translate/business/
--rw-rw-rw-   0        0        0     5681 2024-05-17 12:02:02.000000 LogTranslate-1.4.0/log_translate/business/AndroidCrashPattern_translator.py
--rw-rw-rw-   0        0        0        0 2023-06-28 15:23:37.000000 LogTranslate-1.4.0/log_translate/business/__init__.py
--rw-rw-rw-   0        0        0    19076 2024-03-22 14:56:47.000000 LogTranslate-1.4.0/log_translate/business/bluetooth_translator.py
--rw-rw-rw-   0        0        0      729 2023-11-30 07:50:48.000000 LogTranslate-1.4.0/log_translate/config_default.py
--rw-rw-rw-   0        0        0     2115 2023-09-25 05:24:56.000000 LogTranslate-1.4.0/log_translate/data_struct.py
--rw-rw-rw-   0        0        0     4730 2024-05-17 12:24:36.000000 LogTranslate-1.4.0/log_translate/globals.py
--rw-rw-rw-   0        0        0     6914 2024-02-22 13:36:10.000000 LogTranslate-1.4.0/log_translate/log_translator.py
--rw-rw-rw-   0        0        0     4722 2024-05-17 12:29:31.000000 LogTranslate-1.4.0/log_translate/read_log_file.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:10:13.315781 LogTranslate-1.4.0/log_translate/res/
--rw-rw-rw-   0        0        0    10687 2023-06-28 15:23:37.000000 LogTranslate-1.4.0/log_translate/res/log_logo.ico
--rw-rw-rw-   0        0        0     9014 2024-05-17 12:59:45.000000 LogTranslate-1.4.0/log_translate/ui_pyqt6.py
--rw-rw-rw-   0        0        0     7718 2024-05-17 12:44:57.000000 LogTranslate-1.4.0/log_translate/ui_pyside2.py
--rw-rw-rw-   0        0        0      393 2023-06-28 15:23:37.000000 LogTranslate-1.4.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-17 13:10:13.319382 LogTranslate-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0     2708 2024-05-17 12:54:05.000000 LogTranslate-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 12:31:10.684395 LogTranslate-1.4.1/
+-rw-rw-rw-   0        0        0     1079 2023-06-28 15:23:37.000000 LogTranslate-1.4.1/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2024-05-20 12:31:10.665949 LogTranslate-1.4.1/LogTranslate.egg-info/
+-rw-rw-rw-   0        0        0     3183 2024-05-20 12:31:10.000000 LogTranslate-1.4.1/LogTranslate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      623 2024-05-20 12:31:10.000000 LogTranslate-1.4.1/LogTranslate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 12:31:10.000000 LogTranslate-1.4.1/LogTranslate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-05-20 12:31:10.000000 LogTranslate-1.4.1/LogTranslate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-20 12:31:10.000000 LogTranslate-1.4.1/LogTranslate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3183 2024-05-20 12:31:10.683349 LogTranslate-1.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2474 2023-06-28 15:23:37.000000 LogTranslate-1.4.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 12:31:10.676747 LogTranslate-1.4.1/log_translate/
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:23:37.000000 LogTranslate-1.4.1/log_translate/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 12:31:10.680940 LogTranslate-1.4.1/log_translate/business/
+-rw-rw-rw-   0        0        0     5681 2024-05-17 12:02:02.000000 LogTranslate-1.4.1/log_translate/business/AndroidCrashPattern_translator.py
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:23:37.000000 LogTranslate-1.4.1/log_translate/business/__init__.py
+-rw-rw-rw-   0        0        0    19076 2024-03-22 14:56:47.000000 LogTranslate-1.4.1/log_translate/business/bluetooth_translator.py
+-rw-rw-rw-   0        0        0      729 2023-11-30 07:50:48.000000 LogTranslate-1.4.1/log_translate/config_default.py
+-rw-rw-rw-   0        0        0     2115 2023-09-25 05:24:56.000000 LogTranslate-1.4.1/log_translate/data_struct.py
+-rw-rw-rw-   0        0        0     4730 2024-05-17 12:24:36.000000 LogTranslate-1.4.1/log_translate/globals.py
+-rw-rw-rw-   0        0        0     6914 2024-02-22 13:36:10.000000 LogTranslate-1.4.1/log_translate/log_translator.py
+-rw-rw-rw-   0        0        0     4727 2024-05-20 12:26:30.000000 LogTranslate-1.4.1/log_translate/read_log_file.py
+drwxrwxrwx   0        0        0        0 2024-05-20 12:31:10.682329 LogTranslate-1.4.1/log_translate/res/
+-rw-rw-rw-   0        0        0    10687 2023-06-28 15:23:37.000000 LogTranslate-1.4.1/log_translate/res/log_logo.ico
+-rw-rw-rw-   0        0        0     9014 2024-05-17 12:59:45.000000 LogTranslate-1.4.1/log_translate/ui_pyqt6.py
+-rw-rw-rw-   0        0        0     7718 2024-05-17 12:44:57.000000 LogTranslate-1.4.1/log_translate/ui_pyside2.py
+-rw-rw-rw-   0        0        0      393 2023-06-28 15:23:37.000000 LogTranslate-1.4.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-20 12:31:10.684395 LogTranslate-1.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     2880 2024-05-20 12:28:44.000000 LogTranslate-1.4.1/setup.py
```

### Comparing `LogTranslate-1.4.0/LICENSE.txt` & `LogTranslate-1.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.4.0/LogTranslate.egg-info/PKG-INFO` & `LogTranslate-1.4.1/LogTranslate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LogTranslate
-Version: 1.4.0
+Version: 1.4.1
 Summary: A Python library for translate log from log files
 Home-page: https://github.com/5hmlA/PyTools
 Author: 5hmlA
 Author-email: jonas.jzy@gmail.com
 License: MIT Licence
 Keywords: tools log translate
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `LogTranslate-1.4.0/LogTranslate.egg-info/SOURCES.txt` & `LogTranslate-1.4.1/LogTranslate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.4.0/PKG-INFO` & `LogTranslate-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LogTranslate
-Version: 1.4.0
+Version: 1.4.1
 Summary: A Python library for translate log from log files
 Home-page: https://github.com/5hmlA/PyTools
 Author: 5hmlA
 Author-email: jonas.jzy@gmail.com
 License: MIT Licence
 Keywords: tools log translate
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `LogTranslate-1.4.0/README.md` & `LogTranslate-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.4.0/log_translate/business/AndroidCrashPattern_translator.py` & `LogTranslate-1.4.1/log_translate/business/AndroidCrashPattern_translator.py`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.4.0/log_translate/business/bluetooth_translator.py` & `LogTranslate-1.4.1/log_translate/business/bluetooth_translator.py`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.4.0/log_translate/config_default.py` & `LogTranslate-1.4.1/log_translate/config_default.py`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.4.0/log_translate/data_struct.py` & `LogTranslate-1.4.1/log_translate/data_struct.py`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.4.0/log_translate/globals.py` & `LogTranslate-1.4.1/log_translate/globals.py`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.4.0/log_translate/log_translator.py` & `LogTranslate-1.4.1/log_translate/log_translator.py`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.4.0/log_translate/read_log_file.py` & `LogTranslate-1.4.1/log_translate/read_log_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,19 +33,19 @@
             config = importlib.import_module("config")
             try:
                 self.log_translators = getattr(config, "translators")
             except:
                 self.log_translators = translators
                 traceback.print_exc()
             try:
-                self.global_keys = getattr(config, "global_keys")
+                self.global_keys = set(getattr(config, "global_keys"))
             except:
                 self.global_keys = None
         except:
-            self.global_keys = log_translate.globals.sys_log_keys
+            self.global_keys = set(log_translate.globals.sys_log_keys)
             self.log_translators = translators
             traceback.print_exc()
         # 要在读取了配置之后设置
         self.log_stream._subscribe_core(AutoDetachObserver(on_next=log_translate.globals.log_watcher))
 
     @staticmethod
     def readFile(path="."):
@@ -61,15 +61,15 @@
             # 对日志进行翻译
             try:
                 str = datas.decode('ISO-8859-1').strip()
                 if self.global_keys is None:
                     self.do_translate_one_by_one(str)
                 else:
                     # 将字符数组转换为集合：char_set = set(char_array)。这样可以提高字符查找的效率，因为集合的查找操作为 $O(1)$。
-                    key_set = set(self.global_keys)
+                    key_set = self.global_keys
                     if any(key in str for key in key_set):
                         self.do_translate_one_by_one(str)
             except Exception as e:
                 print('文件解析发生异常：', e)
                 traceback.print_exc()
                 self.log_stream.on_next(Log(translated="文件解析发生异常：%s" % traceback.format_exc(), level=Level.e))
         self.log_stream.on_next(Log(translated=None))
```

### Comparing `LogTranslate-1.4.0/log_translate/res/log_logo.ico` & `LogTranslate-1.4.1/log_translate/res/log_logo.ico`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.4.0/log_translate/ui_pyqt6.py` & `LogTranslate-1.4.1/log_translate/ui_pyqt6.py`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.4.0/log_translate/ui_pyside2.py` & `LogTranslate-1.4.1/log_translate/ui_pyside2.py`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.4.0/setup.py` & `LogTranslate-1.4.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # PACKAGE_NAME主要在使用的时候用到 pkg_resources.resource_filename('log_translate', 'res/log_logo.ico')
 PACKAGE_NAME = 'log_translate'
 # 需要写清楚路径
 ICON_PATH = 'res/*'
 
 setup(
     name='LogTranslate',
-    version='1.4.0',
+    version='1.4.1',
     author='5hmlA',
     author_email='jonas.jzy@gmail.com',
     # 指定运行时需要的Python版本
     python_requires='>=3.6',
     # 找到当前目录下有哪些包 当前(setup.py)目录下的文件夹 当前目录的py不包含 打包的是把所有代码放一个文件夹下文件名为库名字
     packages=find_packages(),
     # 配置readme
@@ -60,9 +60,9 @@
 
 # 发布到测试地址
 # twine upload --repository testpypi dist/*
 # twine upload dist/*
 
 # [pypi]
 #   username = __token__
-#   password = pypi-AgEIcHlwaS5vcmcCJDM1MzcxMjcyLTRlMjY
+#   password = pypi-AgEIcHlwaS5vcmcCJDM1MzcxMjcyLTRlMjYtNDAxZi05MWZlLTI3NzZkZTE5MGI1MAACFFsxLFsibG9ndHJhbnNsYXRlIl1dAAIsWzIsWyJlMzExZmU4MC0wNjdhLTQ3YjAtYTYyNS0wNTU5ODAzODZhMmIiXV0AAAYgmsU-X81dIECmBzOwxMjBP0hgFSLIO2Fc6Ra4tR91tfg
```

