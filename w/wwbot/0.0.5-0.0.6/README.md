# Comparing `tmp/wwbot-0.0.5.tar.gz` & `tmp/wwbot-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwbot-0.0.5.tar", last modified: Sun May 19 09:43:38 2024, max compression
+gzip compressed data, was "wwbot-0.0.6.tar", last modified: Mon May 20 01:07:19 2024, max compression
```

## Comparing `wwbot-0.0.5.tar` & `wwbot-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0 uleo      (1000) uleo      (1000)        0 2024-05-19 09:43:38.388048 wwbot-0.0.5/
--rwxrwxrwx   0 uleo      (1000) uleo      (1000)      933 2024-05-19 09:43:38.387067 wwbot-0.0.5/PKG-INFO
--rwxrwxrwx   0 uleo      (1000) uleo      (1000)       38 2024-05-19 09:43:38.388048 wwbot-0.0.5/setup.cfg
--rwxrwxrwx   0 uleo      (1000) uleo      (1000)      949 2024-05-19 09:43:17.000000 wwbot-0.0.5/setup.py
-drwxrwxrwx   0 uleo      (1000) uleo      (1000)        0 2024-05-19 09:43:38.364113 wwbot-0.0.5/wwbot/
--rwxrwxrwx   0 uleo      (1000) uleo      (1000)    16313 2024-05-19 09:41:15.000000 wwbot-0.0.5/wwbot/__init__.py
-drwxrwxrwx   0 uleo      (1000) uleo      (1000)        0 2024-05-19 09:43:38.383085 wwbot-0.0.5/wwbot/lib/
--rwxrwxrwx   0 uleo      (1000) uleo      (1000)       53 2024-05-11 11:51:42.000000 wwbot-0.0.5/wwbot/lib/__init__.py
--rwxrwxrwx   0 uleo      (1000) uleo      (1000)     4497 2024-05-11 10:37:30.000000 wwbot-0.0.5/wwbot/lib/logger.py
-drwxrwxrwx   0 uleo      (1000) uleo      (1000)        0 2024-05-19 09:43:38.377077 wwbot-0.0.5/wwbot.egg-info/
--rwxrwxrwx   0 uleo      (1000) uleo      (1000)      933 2024-05-19 09:43:38.000000 wwbot-0.0.5/wwbot.egg-info/PKG-INFO
--rwxrwxrwx   0 uleo      (1000) uleo      (1000)      184 2024-05-19 09:43:38.000000 wwbot-0.0.5/wwbot.egg-info/SOURCES.txt
--rwxrwxrwx   0 uleo      (1000) uleo      (1000)        1 2024-05-19 09:43:38.000000 wwbot-0.0.5/wwbot.egg-info/dependency_links.txt
--rwxrwxrwx   0 uleo      (1000) uleo      (1000)        6 2024-05-19 09:43:38.000000 wwbot-0.0.5/wwbot.egg-info/top_level.txt
+drwxrwxrwx   0 uleo      (1000) uleo      (1000)        0 2024-05-20 01:07:19.581056 wwbot-0.0.6/
+-rwxrwxrwx   0 uleo      (1000) uleo      (1000)      933 2024-05-20 01:07:19.580092 wwbot-0.0.6/PKG-INFO
+-rwxrwxrwx   0 uleo      (1000) uleo      (1000)       38 2024-05-20 01:07:19.581056 wwbot-0.0.6/setup.cfg
+-rwxrwxrwx   0 uleo      (1000) uleo      (1000)      949 2024-05-20 01:06:39.000000 wwbot-0.0.6/setup.py
+drwxrwxrwx   0 uleo      (1000) uleo      (1000)        0 2024-05-20 01:07:19.557153 wwbot-0.0.6/wwbot/
+-rwxrwxrwx   0 uleo      (1000) uleo      (1000)    16313 2024-05-19 09:41:15.000000 wwbot-0.0.6/wwbot/__init__.py
+drwxrwxrwx   0 uleo      (1000) uleo      (1000)        0 2024-05-20 01:07:19.577068 wwbot-0.0.6/wwbot/lib/
+-rwxrwxrwx   0 uleo      (1000) uleo      (1000)       53 2024-05-11 11:51:42.000000 wwbot-0.0.6/wwbot/lib/__init__.py
+-rwxrwxrwx   0 uleo      (1000) uleo      (1000)     4505 2024-05-20 01:05:40.000000 wwbot-0.0.6/wwbot/lib/logger.py
+drwxrwxrwx   0 uleo      (1000) uleo      (1000)        0 2024-05-20 01:07:19.570087 wwbot-0.0.6/wwbot.egg-info/
+-rwxrwxrwx   0 uleo      (1000) uleo      (1000)      933 2024-05-20 01:07:19.000000 wwbot-0.0.6/wwbot.egg-info/PKG-INFO
+-rwxrwxrwx   0 uleo      (1000) uleo      (1000)      184 2024-05-20 01:07:19.000000 wwbot-0.0.6/wwbot.egg-info/SOURCES.txt
+-rwxrwxrwx   0 uleo      (1000) uleo      (1000)        1 2024-05-20 01:07:19.000000 wwbot-0.0.6/wwbot.egg-info/dependency_links.txt
+-rwxrwxrwx   0 uleo      (1000) uleo      (1000)        6 2024-05-20 01:07:19.000000 wwbot-0.0.6/wwbot.egg-info/top_level.txt
```

### Comparing `wwbot-0.0.5/PKG-INFO` & `wwbot-0.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwbot
-Version: 0.0.5
+Version: 0.0.6
 Summary: A library for dealing with messages in WeWork
 Home-page: https://github.com/tbbatbb/WeWorkBot
 Author: tbbatbb
 Author-email: 20682299+tbbatbb@users.noreply.github.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `wwbot-0.0.5/setup.py` & `wwbot-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 import setuptools
 
 setuptools.setup(
   name="wwbot",
-  version="0.0.5",
+  version="0.0.6",
   author="tbbatbb",
   author_email="20682299+tbbatbb@users.noreply.github.com",
   description="A library for dealing with messages in WeWork",
   url="https://github.com/tbbatbb/WeWorkBot",
   packages=setuptools.find_packages(),
   classifiers=[
     "Development Status :: 2 - Pre-Alpha",
```

### Comparing `wwbot-0.0.5/wwbot/__init__.py` & `wwbot-0.0.6/wwbot/__init__.py`

 * *Files identical despite different names*

### Comparing `wwbot-0.0.5/wwbot/lib/logger.py` & `wwbot-0.0.6/wwbot/lib/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,17 +44,17 @@
         ts = self.__now_time().strftime('%H:%M:%S')
         if with_stack: call_stack:str = '->'.join(map(lambda s: f'{s[2]}:{s[1]}', traceback.extract_stack()[:-2]))
         else:
             line, caller = traceback.extract_stack()[-3][1:3]
             call_stack:str = f'[{caller}:{line}]'
         print(color + symbol, ts, f'[{self.name}]', call_stack + Logger.C_DEFAULT, *args, **kwarg)
         sys.stdout.flush()
-        msg = ' '.join([str(a) for a in args])
-        self.__save(self.TOTAL_LOG_NAME, f'[{ts}] | {msg}{os.linesep}')
         if self.save_to_file:
+            msg = ' '.join([str(a) for a in args])
+            self.__save(self.TOTAL_LOG_NAME, f'[{ts}] | {msg}{os.linesep}')
             self.__save(self.name, f'{symbol}[{ts}] | {msg}{os.linesep}')
 
     def __save(self, file_name:str, msg:str):
         if not path.isdir(self.LOG_DIR):
             os.mkdir(self.LOG_DIR)
             self.info(f'Directory {self.LOG_DIR} For Log Files Created.')
         log_file:str = path.join(self.LOG_DIR, f'{file_name}.log')
```

### Comparing `wwbot-0.0.5/wwbot.egg-info/PKG-INFO` & `wwbot-0.0.6/wwbot.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwbot
-Version: 0.0.5
+Version: 0.0.6
 Summary: A library for dealing with messages in WeWork
 Home-page: https://github.com/tbbatbb/WeWorkBot
 Author: tbbatbb
 Author-email: 20682299+tbbatbb@users.noreply.github.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

