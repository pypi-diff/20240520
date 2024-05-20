# Comparing `tmp/logger_aux-0.0.7.tar.gz` & `tmp/logger_aux-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logger_aux-0.0.7.tar", last modified: Sat Apr 27 12:28:01 2024, max compression
+gzip compressed data, was "logger_aux-0.0.8.tar", last modified: Mon May 20 11:41:42 2024, max compression
```

## Comparing `logger_aux-0.0.7.tar` & `logger_aux-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 12:28:01.557986 logger_aux-0.0.7/
--rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 logger_aux-0.0.7/LICENSE
--rw-rw-rw-   0        0        0    19842 2024-04-27 12:28:01.557986 logger_aux-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0    19042 2024-04-27 12:27:23.000000 logger_aux-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-27 12:28:01.552121 logger_aux-0.0.7/logger_aux/
--rw-rw-rw-   0        0        0       21 2024-01-15 06:52:12.000000 logger_aux-0.0.7/logger_aux/__init__.py
--rw-rw-rw-   0        0        0     6405 2024-04-27 11:57:41.000000 logger_aux-0.0.7/logger_aux/main.py
-drwxrwxrwx   0        0        0        0 2024-04-27 12:28:01.556988 logger_aux-0.0.7/logger_aux.egg-info/
--rw-rw-rw-   0        0        0    19842 2024-04-27 12:28:01.000000 logger_aux-0.0.7/logger_aux.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2024-04-27 12:28:01.000000 logger_aux-0.0.7/logger_aux.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 12:28:01.000000 logger_aux-0.0.7/logger_aux.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-27 12:28:01.000000 logger_aux-0.0.7/logger_aux.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-27 12:28:01.559002 logger_aux-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     2184 2024-04-26 07:47:41.000000 logger_aux-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 11:41:42.853786 logger_aux-0.0.8/
+-rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 logger_aux-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0    25194 2024-05-20 11:41:42.853105 logger_aux-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0    24394 2024-05-20 11:40:57.000000 logger_aux-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 11:41:42.843429 logger_aux-0.0.8/logger_aux/
+-rw-rw-rw-   0        0        0       21 2024-01-15 06:52:12.000000 logger_aux-0.0.8/logger_aux/__init__.py
+-rw-rw-rw-   0        0        0     6675 2024-05-20 11:40:57.000000 logger_aux-0.0.8/logger_aux/main.py
+drwxrwxrwx   0        0        0        0 2024-05-20 11:41:42.850626 logger_aux-0.0.8/logger_aux.egg-info/
+-rw-rw-rw-   0        0        0    25194 2024-05-20 11:41:42.000000 logger_aux-0.0.8/logger_aux.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2024-05-20 11:41:42.000000 logger_aux-0.0.8/logger_aux.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 11:41:42.000000 logger_aux-0.0.8/logger_aux.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-20 11:41:42.000000 logger_aux-0.0.8/logger_aux.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 11:41:42.855341 logger_aux-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-04-26 07:47:41.000000 logger_aux-0.0.8/setup.py
```

### Comparing `logger_aux-0.0.7/LICENSE` & `logger_aux-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `logger_aux-0.0.7/PKG-INFO` & `logger_aux-0.0.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logger_aux
-Version: 0.0.7
+Version: 0.0.8
 Summary: simple logging
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/logger_aux
 Keywords: logger
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# logger_aux (v0.0.7)
+# logger_aux (v0.0.8)
 
 ## DESCRIPTION_SHORT
 simple logging
 
 ## DESCRIPTION_LONG
 designed for DRY simple/easy usage logging
 
@@ -124,14 +124,18 @@
 2024-04-27 14:56:41,419[DEBUG]Example(main.py).__init__(line155)/thread31224::[Logger.Example] start STREAM
 2024-04-27 14:56:41,419[DEBUG]Example(main.py).__init__(line158)/thread31224::[Logger.Example] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__Example.log]
 2024-04-27 14:56:41,420[DEBUG]Example(example1.py).meth(line41)/thread31224::hello123
 2024-04-27 14:57:41,958[DEBUG]Example(main.py).__init__(line152)/thread32520::====================================================================================================
 2024-04-27 14:57:41,959[DEBUG]Example(main.py).__init__(line155)/thread32520::[Logger.Example] start STREAM
 2024-04-27 14:57:41,959[DEBUG]Example(main.py).__init__(line158)/thread32520::[Logger.Example] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__Example.log]
 2024-04-27 14:57:41,959[DEBUG]Example(example1.py).meth(line41)/thread32520::hello123
+2024-04-27 15:27:49,968[DEBUG]Example(main.py).__init__(line152)/thread28020::====================================================================================================
+2024-04-27 15:27:49,968[DEBUG]Example(main.py).__init__(line155)/thread28020::[Logger.Example] start STREAM
+2024-04-27 15:27:49,969[DEBUG]Example(main.py).__init__(line158)/thread28020::[Logger.Example] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__Example.log]
+2024-04-27 15:27:49,969[DEBUG]Example(example1.py).meth(line41)/thread28020::hello123
 ```
 
 ------------------------------
 ### 3. logger__logger_first.log
 ```
 2024-04-27 14:56:35,114[DEBUG]logger_first(main.py).__init__(line152)/thread39932::====================================================================================================
 2024-04-27 14:56:35,114[DEBUG]logger_first(main.py).__init__(line155)/thread39932::[Logger.logger_first] start STREAM
@@ -144,14 +148,19 @@
 2024-04-27 14:56:41,415[DEBUG]logger_first(example1.py).<module>(line16)/thread31224::hello1-1
 2024-04-27 14:56:41,417[DEBUG]logger_first(example1.py).<module>(line22)/thread31224::hello1-2
 2024-04-27 14:57:41,954[DEBUG]logger_first(main.py).__init__(line152)/thread32520::====================================================================================================
 2024-04-27 14:57:41,954[DEBUG]logger_first(main.py).__init__(line155)/thread32520::[Logger.logger_first] start STREAM
 2024-04-27 14:57:41,955[DEBUG]logger_first(main.py).__init__(line158)/thread32520::[Logger.logger_first] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__logger_first.log]
 2024-04-27 14:57:41,955[DEBUG]logger_first(example1.py).<module>(line16)/thread32520::hello1-1
 2024-04-27 14:57:41,957[DEBUG]logger_first(example1.py).<module>(line22)/thread32520::hello1-2
+2024-04-27 15:27:49,963[DEBUG]logger_first(main.py).__init__(line152)/thread28020::====================================================================================================
+2024-04-27 15:27:49,963[DEBUG]logger_first(main.py).__init__(line155)/thread28020::[Logger.logger_first] start STREAM
+2024-04-27 15:27:49,964[DEBUG]logger_first(main.py).__init__(line158)/thread28020::[Logger.logger_first] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__logger_first.log]
+2024-04-27 15:27:49,964[DEBUG]logger_first(example1.py).<module>(line16)/thread28020::hello1-1
+2024-04-27 15:27:49,966[DEBUG]logger_first(example1.py).<module>(line22)/thread28020::hello1-2
 ```
 
 ------------------------------
 ### 4. logger__logger_second.log
 ```
 2024-04-27 14:56:35,115[DEBUG]logger_second(main.py).__init__(line152)/thread39932::====================================================================================================
 2024-04-27 14:56:35,116[DEBUG]logger_second(main.py).__init__(line155)/thread39932::[Logger.logger_second] start STREAM
@@ -164,14 +173,19 @@
 2024-04-27 14:56:41,416[DEBUG]logger_second(example1.py).<module>(line19)/thread31224::hello2-1
 2024-04-27 14:56:41,417[DEBUG]logger_second(example1.py).<module>(line23)/thread31224::hello2-2
 2024-04-27 14:57:41,955[DEBUG]logger_second(main.py).__init__(line152)/thread32520::====================================================================================================
 2024-04-27 14:57:41,956[DEBUG]logger_second(main.py).__init__(line155)/thread32520::[Logger.logger_second] start STREAM
 2024-04-27 14:57:41,956[DEBUG]logger_second(main.py).__init__(line158)/thread32520::[Logger.logger_second] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__logger_second.log]
 2024-04-27 14:57:41,956[DEBUG]logger_second(example1.py).<module>(line19)/thread32520::hello2-1
 2024-04-27 14:57:41,957[DEBUG]logger_second(example1.py).<module>(line23)/thread32520::hello2-2
+2024-04-27 15:27:49,964[DEBUG]logger_second(main.py).__init__(line152)/thread28020::====================================================================================================
+2024-04-27 15:27:49,965[DEBUG]logger_second(main.py).__init__(line155)/thread28020::[Logger.logger_second] start STREAM
+2024-04-27 15:27:49,965[DEBUG]logger_second(main.py).__init__(line158)/thread28020::[Logger.logger_second] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__logger_second.log]
+2024-04-27 15:27:49,966[DEBUG]logger_second(example1.py).<module>(line19)/thread28020::hello2-1
+2024-04-27 15:27:49,966[DEBUG]logger_second(example1.py).<module>(line23)/thread28020::hello2-2
 ```
 
 ------------------------------
 ### 5. logger__root.log
 ```
 2024-04-27 14:56:35,111[DEBUG]root(main.py).__init__(line152)/thread39932::====================================================================================================
 2024-04-27 14:56:35,111[DEBUG]root(main.py).__init__(line155)/thread39932::[Logger.root] start STREAM
@@ -247,10 +261,36 @@
 2024-04-27 14:57:41,958[DEBUG]logger_dir(main.py).__init__(line155)/thread32520::[Logger.logger_dir] start STREAM
 2024-04-27 14:57:41,958[DEBUG]logger_dir(main.py).__init__(line158)/thread32520::[Logger.logger_dir] start FILE=[c:\1\logger__logger_dir.log]
 2024-04-27 14:57:41,958[DEBUG]logger_dir(example1.py).<module>(line27)/thread32520::hello_dir
 2024-04-27 14:57:41,958[DEBUG]Example(main.py).__init__(line152)/thread32520::====================================================================================================
 2024-04-27 14:57:41,959[DEBUG]Example(main.py).__init__(line155)/thread32520::[Logger.Example] start STREAM
 2024-04-27 14:57:41,959[DEBUG]Example(main.py).__init__(line158)/thread32520::[Logger.Example] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__Example.log]
 2024-04-27 14:57:41,959[DEBUG]Example(example1.py).meth(line41)/thread32520::hello123
+2024-04-27 15:27:49,962[DEBUG]root(main.py).__init__(line152)/thread28020::====================================================================================================
+2024-04-27 15:27:49,962[DEBUG]root(main.py).__init__(line155)/thread28020::[Logger.root] start STREAM
+2024-04-27 15:27:49,962[DEBUG]root(main.py).__init__(line158)/thread28020::[Logger.root] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__root.log]
+2024-04-27 15:27:49,962[DEBUG]root(example1.py).<module>(line10)/thread28020::None
+2024-04-27 15:27:49,963[DEBUG]root(example1.py).<module>(line11)/thread28020::True
+2024-04-27 15:27:49,963[DEBUG]root(example1.py).<module>(line12)/thread28020::
+2024-04-27 15:27:49,963[DEBUG]root(example1.py).<module>(line13)/thread28020::hello0-1
+2024-04-27 15:27:49,963[DEBUG]logger_first(main.py).__init__(line152)/thread28020::====================================================================================================
+2024-04-27 15:27:49,963[DEBUG]logger_first(main.py).__init__(line155)/thread28020::[Logger.logger_first] start STREAM
+2024-04-27 15:27:49,964[DEBUG]logger_first(main.py).__init__(line158)/thread28020::[Logger.logger_first] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__logger_first.log]
+2024-04-27 15:27:49,964[DEBUG]logger_first(example1.py).<module>(line16)/thread28020::hello1-1
+2024-04-27 15:27:49,964[DEBUG]logger_second(main.py).__init__(line152)/thread28020::====================================================================================================
+2024-04-27 15:27:49,965[DEBUG]logger_second(main.py).__init__(line155)/thread28020::[Logger.logger_second] start STREAM
+2024-04-27 15:27:49,965[DEBUG]logger_second(main.py).__init__(line158)/thread28020::[Logger.logger_second] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__logger_second.log]
+2024-04-27 15:27:49,966[DEBUG]logger_second(example1.py).<module>(line19)/thread28020::hello2-1
+2024-04-27 15:27:49,966[DEBUG]root(example1.py).<module>(line21)/thread28020::hello0-2
+2024-04-27 15:27:49,966[DEBUG]logger_first(example1.py).<module>(line22)/thread28020::hello1-2
+2024-04-27 15:27:49,966[DEBUG]logger_second(example1.py).<module>(line23)/thread28020::hello2-2
+2024-04-27 15:27:49,966[DEBUG]logger_dir(main.py).__init__(line152)/thread28020::====================================================================================================
+2024-04-27 15:27:49,967[DEBUG]logger_dir(main.py).__init__(line155)/thread28020::[Logger.logger_dir] start STREAM
+2024-04-27 15:27:49,968[DEBUG]logger_dir(main.py).__init__(line158)/thread28020::[Logger.logger_dir] start FILE=[c:\1\logger__logger_dir.log]
+2024-04-27 15:27:49,968[DEBUG]logger_dir(example1.py).<module>(line27)/thread28020::hello_dir
+2024-04-27 15:27:49,968[DEBUG]Example(main.py).__init__(line152)/thread28020::====================================================================================================
+2024-04-27 15:27:49,968[DEBUG]Example(main.py).__init__(line155)/thread28020::[Logger.Example] start STREAM
+2024-04-27 15:27:49,969[DEBUG]Example(main.py).__init__(line158)/thread28020::[Logger.Example] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__Example.log]
+2024-04-27 15:27:49,969[DEBUG]Example(example1.py).meth(line41)/thread28020::hello123
 ```
 
 ********************************************************************************
```

### Comparing `logger_aux-0.0.7/README.md` & `logger_aux-0.0.8/logger_aux.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,30 @@
-# logger_aux (v0.0.7)
+Metadata-Version: 2.1
+Name: logger_aux
+Version: 0.0.8
+Summary: simple logging
+Home-page: https://github.com/centroid457/
+Author: Andrei Starichenko
+Author-email: centroid@mail.ru
+Project-URL: Source, https://github.com/centroid457/logger_aux
+Keywords: logger
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Typing :: Typed
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# logger_aux (v0.0.8)
 
 ## DESCRIPTION_SHORT
 simple logging
 
 ## DESCRIPTION_LONG
 designed for DRY simple/easy usage logging
 
@@ -102,14 +124,18 @@
 2024-04-27 14:56:41,419[DEBUG]Example(main.py).__init__(line155)/thread31224::[Logger.Example] start STREAM
 2024-04-27 14:56:41,419[DEBUG]Example(main.py).__init__(line158)/thread31224::[Logger.Example] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__Example.log]
 2024-04-27 14:56:41,420[DEBUG]Example(example1.py).meth(line41)/thread31224::hello123
 2024-04-27 14:57:41,958[DEBUG]Example(main.py).__init__(line152)/thread32520::====================================================================================================
 2024-04-27 14:57:41,959[DEBUG]Example(main.py).__init__(line155)/thread32520::[Logger.Example] start STREAM
 2024-04-27 14:57:41,959[DEBUG]Example(main.py).__init__(line158)/thread32520::[Logger.Example] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__Example.log]
 2024-04-27 14:57:41,959[DEBUG]Example(example1.py).meth(line41)/thread32520::hello123
+2024-04-27 15:27:49,968[DEBUG]Example(main.py).__init__(line152)/thread28020::====================================================================================================
+2024-04-27 15:27:49,968[DEBUG]Example(main.py).__init__(line155)/thread28020::[Logger.Example] start STREAM
+2024-04-27 15:27:49,969[DEBUG]Example(main.py).__init__(line158)/thread28020::[Logger.Example] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__Example.log]
+2024-04-27 15:27:49,969[DEBUG]Example(example1.py).meth(line41)/thread28020::hello123
 ```
 
 ------------------------------
 ### 3. logger__logger_first.log
 ```
 2024-04-27 14:56:35,114[DEBUG]logger_first(main.py).__init__(line152)/thread39932::====================================================================================================
 2024-04-27 14:56:35,114[DEBUG]logger_first(main.py).__init__(line155)/thread39932::[Logger.logger_first] start STREAM
@@ -122,14 +148,19 @@
 2024-04-27 14:56:41,415[DEBUG]logger_first(example1.py).<module>(line16)/thread31224::hello1-1
 2024-04-27 14:56:41,417[DEBUG]logger_first(example1.py).<module>(line22)/thread31224::hello1-2
 2024-04-27 14:57:41,954[DEBUG]logger_first(main.py).__init__(line152)/thread32520::====================================================================================================
 2024-04-27 14:57:41,954[DEBUG]logger_first(main.py).__init__(line155)/thread32520::[Logger.logger_first] start STREAM
 2024-04-27 14:57:41,955[DEBUG]logger_first(main.py).__init__(line158)/thread32520::[Logger.logger_first] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__logger_first.log]
 2024-04-27 14:57:41,955[DEBUG]logger_first(example1.py).<module>(line16)/thread32520::hello1-1
 2024-04-27 14:57:41,957[DEBUG]logger_first(example1.py).<module>(line22)/thread32520::hello1-2
+2024-04-27 15:27:49,963[DEBUG]logger_first(main.py).__init__(line152)/thread28020::====================================================================================================
+2024-04-27 15:27:49,963[DEBUG]logger_first(main.py).__init__(line155)/thread28020::[Logger.logger_first] start STREAM
+2024-04-27 15:27:49,964[DEBUG]logger_first(main.py).__init__(line158)/thread28020::[Logger.logger_first] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__logger_first.log]
+2024-04-27 15:27:49,964[DEBUG]logger_first(example1.py).<module>(line16)/thread28020::hello1-1
+2024-04-27 15:27:49,966[DEBUG]logger_first(example1.py).<module>(line22)/thread28020::hello1-2
 ```
 
 ------------------------------
 ### 4. logger__logger_second.log
 ```
 2024-04-27 14:56:35,115[DEBUG]logger_second(main.py).__init__(line152)/thread39932::====================================================================================================
 2024-04-27 14:56:35,116[DEBUG]logger_second(main.py).__init__(line155)/thread39932::[Logger.logger_second] start STREAM
@@ -142,14 +173,19 @@
 2024-04-27 14:56:41,416[DEBUG]logger_second(example1.py).<module>(line19)/thread31224::hello2-1
 2024-04-27 14:56:41,417[DEBUG]logger_second(example1.py).<module>(line23)/thread31224::hello2-2
 2024-04-27 14:57:41,955[DEBUG]logger_second(main.py).__init__(line152)/thread32520::====================================================================================================
 2024-04-27 14:57:41,956[DEBUG]logger_second(main.py).__init__(line155)/thread32520::[Logger.logger_second] start STREAM
 2024-04-27 14:57:41,956[DEBUG]logger_second(main.py).__init__(line158)/thread32520::[Logger.logger_second] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__logger_second.log]
 2024-04-27 14:57:41,956[DEBUG]logger_second(example1.py).<module>(line19)/thread32520::hello2-1
 2024-04-27 14:57:41,957[DEBUG]logger_second(example1.py).<module>(line23)/thread32520::hello2-2
+2024-04-27 15:27:49,964[DEBUG]logger_second(main.py).__init__(line152)/thread28020::====================================================================================================
+2024-04-27 15:27:49,965[DEBUG]logger_second(main.py).__init__(line155)/thread28020::[Logger.logger_second] start STREAM
+2024-04-27 15:27:49,965[DEBUG]logger_second(main.py).__init__(line158)/thread28020::[Logger.logger_second] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__logger_second.log]
+2024-04-27 15:27:49,966[DEBUG]logger_second(example1.py).<module>(line19)/thread28020::hello2-1
+2024-04-27 15:27:49,966[DEBUG]logger_second(example1.py).<module>(line23)/thread28020::hello2-2
 ```
 
 ------------------------------
 ### 5. logger__root.log
 ```
 2024-04-27 14:56:35,111[DEBUG]root(main.py).__init__(line152)/thread39932::====================================================================================================
 2024-04-27 14:56:35,111[DEBUG]root(main.py).__init__(line155)/thread39932::[Logger.root] start STREAM
@@ -225,10 +261,36 @@
 2024-04-27 14:57:41,958[DEBUG]logger_dir(main.py).__init__(line155)/thread32520::[Logger.logger_dir] start STREAM
 2024-04-27 14:57:41,958[DEBUG]logger_dir(main.py).__init__(line158)/thread32520::[Logger.logger_dir] start FILE=[c:\1\logger__logger_dir.log]
 2024-04-27 14:57:41,958[DEBUG]logger_dir(example1.py).<module>(line27)/thread32520::hello_dir
 2024-04-27 14:57:41,958[DEBUG]Example(main.py).__init__(line152)/thread32520::====================================================================================================
 2024-04-27 14:57:41,959[DEBUG]Example(main.py).__init__(line155)/thread32520::[Logger.Example] start STREAM
 2024-04-27 14:57:41,959[DEBUG]Example(main.py).__init__(line158)/thread32520::[Logger.Example] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__Example.log]
 2024-04-27 14:57:41,959[DEBUG]Example(example1.py).meth(line41)/thread32520::hello123
+2024-04-27 15:27:49,962[DEBUG]root(main.py).__init__(line152)/thread28020::====================================================================================================
+2024-04-27 15:27:49,962[DEBUG]root(main.py).__init__(line155)/thread28020::[Logger.root] start STREAM
+2024-04-27 15:27:49,962[DEBUG]root(main.py).__init__(line158)/thread28020::[Logger.root] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__root.log]
+2024-04-27 15:27:49,962[DEBUG]root(example1.py).<module>(line10)/thread28020::None
+2024-04-27 15:27:49,963[DEBUG]root(example1.py).<module>(line11)/thread28020::True
+2024-04-27 15:27:49,963[DEBUG]root(example1.py).<module>(line12)/thread28020::
+2024-04-27 15:27:49,963[DEBUG]root(example1.py).<module>(line13)/thread28020::hello0-1
+2024-04-27 15:27:49,963[DEBUG]logger_first(main.py).__init__(line152)/thread28020::====================================================================================================
+2024-04-27 15:27:49,963[DEBUG]logger_first(main.py).__init__(line155)/thread28020::[Logger.logger_first] start STREAM
+2024-04-27 15:27:49,964[DEBUG]logger_first(main.py).__init__(line158)/thread28020::[Logger.logger_first] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__logger_first.log]
+2024-04-27 15:27:49,964[DEBUG]logger_first(example1.py).<module>(line16)/thread28020::hello1-1
+2024-04-27 15:27:49,964[DEBUG]logger_second(main.py).__init__(line152)/thread28020::====================================================================================================
+2024-04-27 15:27:49,965[DEBUG]logger_second(main.py).__init__(line155)/thread28020::[Logger.logger_second] start STREAM
+2024-04-27 15:27:49,965[DEBUG]logger_second(main.py).__init__(line158)/thread28020::[Logger.logger_second] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__logger_second.log]
+2024-04-27 15:27:49,966[DEBUG]logger_second(example1.py).<module>(line19)/thread28020::hello2-1
+2024-04-27 15:27:49,966[DEBUG]root(example1.py).<module>(line21)/thread28020::hello0-2
+2024-04-27 15:27:49,966[DEBUG]logger_first(example1.py).<module>(line22)/thread28020::hello1-2
+2024-04-27 15:27:49,966[DEBUG]logger_second(example1.py).<module>(line23)/thread28020::hello2-2
+2024-04-27 15:27:49,966[DEBUG]logger_dir(main.py).__init__(line152)/thread28020::====================================================================================================
+2024-04-27 15:27:49,967[DEBUG]logger_dir(main.py).__init__(line155)/thread28020::[Logger.logger_dir] start STREAM
+2024-04-27 15:27:49,968[DEBUG]logger_dir(main.py).__init__(line158)/thread28020::[Logger.logger_dir] start FILE=[c:\1\logger__logger_dir.log]
+2024-04-27 15:27:49,968[DEBUG]logger_dir(example1.py).<module>(line27)/thread28020::hello_dir
+2024-04-27 15:27:49,968[DEBUG]Example(main.py).__init__(line152)/thread28020::====================================================================================================
+2024-04-27 15:27:49,968[DEBUG]Example(main.py).__init__(line155)/thread28020::[Logger.Example] start STREAM
+2024-04-27 15:27:49,969[DEBUG]Example(main.py).__init__(line158)/thread28020::[Logger.Example] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__Example.log]
+2024-04-27 15:27:49,969[DEBUG]Example(example1.py).meth(line41)/thread28020::hello123
 ```
 
 ********************************************************************************
```

### Comparing `logger_aux-0.0.7/logger_aux/main.py` & `logger_aux-0.0.8/logger_aux/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,20 +45,20 @@
 
     LOG_FILE_STARTWITH: None | str = None
     LOG_FILE_EXTENTION: None | str = None
     LOG_FILE_MAXBYTES: int = 1024 * 1024 * 10
     LOG_FILE_BACKUPCOUNT: int = 3
 
     LOG_ENABLE: None | bool = False
-
     LOG_USE_STREAM: bool = True
-    LOG_USE_FILE: bool = True
+    LOG_USE_FILE: bool = False
 
     # AUX ---------------------------------------
     _formatter: logging.Formatter
+    LOGGER: Self = None
 
     @property
     def LOG_FILENAME(self) -> str:
         return f"{self.LOG_FILE_STARTWITH or 'logger'}__{self.LOG_NAME or 'root'}.{self.LOG_FILE_EXTENTION or 'log'}"
 
     @property
     def LOG_FILEPATH(self) -> pathlib.Path:
@@ -107,14 +107,19 @@
             if class_name == "Logger":
                 self.LOG_NAME = "root"
             else:
                 self.LOG_NAME = class_name
         elif not isinstance(self.LOG_NAME, str):
             self.LOG_NAME = self.LOG_NAME.__class__.__name__
 
+        # if not self.__class__.LOGGER:
+        #     # place here MRO name??? for classmethods???
+        #     # useful for methods starts after inited first instance
+        #     self.__class__.LOGGER = logging.getLogger(self.LOG_NAME)
+
         self.LOGGER = logging.getLogger(self.LOG_NAME)
 
         # DISABLE ------------------------------------------
         if self.LOG_NAME == "root" and log_enable:
             pass
 
         elif not self.LOG_ENABLE:
```

### Comparing `logger_aux-0.0.7/logger_aux.egg-info/PKG-INFO` & `logger_aux-0.0.8/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,8 @@
-Metadata-Version: 2.1
-Name: logger_aux
-Version: 0.0.7
-Summary: simple logging
-Home-page: https://github.com/centroid457/
-Author: Andrei Starichenko
-Author-email: centroid@mail.ru
-Project-URL: Source, https://github.com/centroid457/logger_aux
-Keywords: logger
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Typing :: Typed
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# logger_aux (v0.0.7)
+# logger_aux (v0.0.8)
 
 ## DESCRIPTION_SHORT
 simple logging
 
 ## DESCRIPTION_LONG
 designed for DRY simple/easy usage logging
 
@@ -124,14 +102,18 @@
 2024-04-27 14:56:41,419[DEBUG]Example(main.py).__init__(line155)/thread31224::[Logger.Example] start STREAM
 2024-04-27 14:56:41,419[DEBUG]Example(main.py).__init__(line158)/thread31224::[Logger.Example] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__Example.log]
 2024-04-27 14:56:41,420[DEBUG]Example(example1.py).meth(line41)/thread31224::hello123
 2024-04-27 14:57:41,958[DEBUG]Example(main.py).__init__(line152)/thread32520::====================================================================================================
 2024-04-27 14:57:41,959[DEBUG]Example(main.py).__init__(line155)/thread32520::[Logger.Example] start STREAM
 2024-04-27 14:57:41,959[DEBUG]Example(main.py).__init__(line158)/thread32520::[Logger.Example] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__Example.log]
 2024-04-27 14:57:41,959[DEBUG]Example(example1.py).meth(line41)/thread32520::hello123
+2024-04-27 15:27:49,968[DEBUG]Example(main.py).__init__(line152)/thread28020::====================================================================================================
+2024-04-27 15:27:49,968[DEBUG]Example(main.py).__init__(line155)/thread28020::[Logger.Example] start STREAM
+2024-04-27 15:27:49,969[DEBUG]Example(main.py).__init__(line158)/thread28020::[Logger.Example] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__Example.log]
+2024-04-27 15:27:49,969[DEBUG]Example(example1.py).meth(line41)/thread28020::hello123
 ```
 
 ------------------------------
 ### 3. logger__logger_first.log
 ```
 2024-04-27 14:56:35,114[DEBUG]logger_first(main.py).__init__(line152)/thread39932::====================================================================================================
 2024-04-27 14:56:35,114[DEBUG]logger_first(main.py).__init__(line155)/thread39932::[Logger.logger_first] start STREAM
@@ -144,14 +126,19 @@
 2024-04-27 14:56:41,415[DEBUG]logger_first(example1.py).<module>(line16)/thread31224::hello1-1
 2024-04-27 14:56:41,417[DEBUG]logger_first(example1.py).<module>(line22)/thread31224::hello1-2
 2024-04-27 14:57:41,954[DEBUG]logger_first(main.py).__init__(line152)/thread32520::====================================================================================================
 2024-04-27 14:57:41,954[DEBUG]logger_first(main.py).__init__(line155)/thread32520::[Logger.logger_first] start STREAM
 2024-04-27 14:57:41,955[DEBUG]logger_first(main.py).__init__(line158)/thread32520::[Logger.logger_first] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__logger_first.log]
 2024-04-27 14:57:41,955[DEBUG]logger_first(example1.py).<module>(line16)/thread32520::hello1-1
 2024-04-27 14:57:41,957[DEBUG]logger_first(example1.py).<module>(line22)/thread32520::hello1-2
+2024-04-27 15:27:49,963[DEBUG]logger_first(main.py).__init__(line152)/thread28020::====================================================================================================
+2024-04-27 15:27:49,963[DEBUG]logger_first(main.py).__init__(line155)/thread28020::[Logger.logger_first] start STREAM
+2024-04-27 15:27:49,964[DEBUG]logger_first(main.py).__init__(line158)/thread28020::[Logger.logger_first] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__logger_first.log]
+2024-04-27 15:27:49,964[DEBUG]logger_first(example1.py).<module>(line16)/thread28020::hello1-1
+2024-04-27 15:27:49,966[DEBUG]logger_first(example1.py).<module>(line22)/thread28020::hello1-2
 ```
 
 ------------------------------
 ### 4. logger__logger_second.log
 ```
 2024-04-27 14:56:35,115[DEBUG]logger_second(main.py).__init__(line152)/thread39932::====================================================================================================
 2024-04-27 14:56:35,116[DEBUG]logger_second(main.py).__init__(line155)/thread39932::[Logger.logger_second] start STREAM
@@ -164,14 +151,19 @@
 2024-04-27 14:56:41,416[DEBUG]logger_second(example1.py).<module>(line19)/thread31224::hello2-1
 2024-04-27 14:56:41,417[DEBUG]logger_second(example1.py).<module>(line23)/thread31224::hello2-2
 2024-04-27 14:57:41,955[DEBUG]logger_second(main.py).__init__(line152)/thread32520::====================================================================================================
 2024-04-27 14:57:41,956[DEBUG]logger_second(main.py).__init__(line155)/thread32520::[Logger.logger_second] start STREAM
 2024-04-27 14:57:41,956[DEBUG]logger_second(main.py).__init__(line158)/thread32520::[Logger.logger_second] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__logger_second.log]
 2024-04-27 14:57:41,956[DEBUG]logger_second(example1.py).<module>(line19)/thread32520::hello2-1
 2024-04-27 14:57:41,957[DEBUG]logger_second(example1.py).<module>(line23)/thread32520::hello2-2
+2024-04-27 15:27:49,964[DEBUG]logger_second(main.py).__init__(line152)/thread28020::====================================================================================================
+2024-04-27 15:27:49,965[DEBUG]logger_second(main.py).__init__(line155)/thread28020::[Logger.logger_second] start STREAM
+2024-04-27 15:27:49,965[DEBUG]logger_second(main.py).__init__(line158)/thread28020::[Logger.logger_second] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__logger_second.log]
+2024-04-27 15:27:49,966[DEBUG]logger_second(example1.py).<module>(line19)/thread28020::hello2-1
+2024-04-27 15:27:49,966[DEBUG]logger_second(example1.py).<module>(line23)/thread28020::hello2-2
 ```
 
 ------------------------------
 ### 5. logger__root.log
 ```
 2024-04-27 14:56:35,111[DEBUG]root(main.py).__init__(line152)/thread39932::====================================================================================================
 2024-04-27 14:56:35,111[DEBUG]root(main.py).__init__(line155)/thread39932::[Logger.root] start STREAM
@@ -247,10 +239,36 @@
 2024-04-27 14:57:41,958[DEBUG]logger_dir(main.py).__init__(line155)/thread32520::[Logger.logger_dir] start STREAM
 2024-04-27 14:57:41,958[DEBUG]logger_dir(main.py).__init__(line158)/thread32520::[Logger.logger_dir] start FILE=[c:\1\logger__logger_dir.log]
 2024-04-27 14:57:41,958[DEBUG]logger_dir(example1.py).<module>(line27)/thread32520::hello_dir
 2024-04-27 14:57:41,958[DEBUG]Example(main.py).__init__(line152)/thread32520::====================================================================================================
 2024-04-27 14:57:41,959[DEBUG]Example(main.py).__init__(line155)/thread32520::[Logger.Example] start STREAM
 2024-04-27 14:57:41,959[DEBUG]Example(main.py).__init__(line158)/thread32520::[Logger.Example] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__Example.log]
 2024-04-27 14:57:41,959[DEBUG]Example(example1.py).meth(line41)/thread32520::hello123
+2024-04-27 15:27:49,962[DEBUG]root(main.py).__init__(line152)/thread28020::====================================================================================================
+2024-04-27 15:27:49,962[DEBUG]root(main.py).__init__(line155)/thread28020::[Logger.root] start STREAM
+2024-04-27 15:27:49,962[DEBUG]root(main.py).__init__(line158)/thread28020::[Logger.root] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__root.log]
+2024-04-27 15:27:49,962[DEBUG]root(example1.py).<module>(line10)/thread28020::None
+2024-04-27 15:27:49,963[DEBUG]root(example1.py).<module>(line11)/thread28020::True
+2024-04-27 15:27:49,963[DEBUG]root(example1.py).<module>(line12)/thread28020::
+2024-04-27 15:27:49,963[DEBUG]root(example1.py).<module>(line13)/thread28020::hello0-1
+2024-04-27 15:27:49,963[DEBUG]logger_first(main.py).__init__(line152)/thread28020::====================================================================================================
+2024-04-27 15:27:49,963[DEBUG]logger_first(main.py).__init__(line155)/thread28020::[Logger.logger_first] start STREAM
+2024-04-27 15:27:49,964[DEBUG]logger_first(main.py).__init__(line158)/thread28020::[Logger.logger_first] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__logger_first.log]
+2024-04-27 15:27:49,964[DEBUG]logger_first(example1.py).<module>(line16)/thread28020::hello1-1
+2024-04-27 15:27:49,964[DEBUG]logger_second(main.py).__init__(line152)/thread28020::====================================================================================================
+2024-04-27 15:27:49,965[DEBUG]logger_second(main.py).__init__(line155)/thread28020::[Logger.logger_second] start STREAM
+2024-04-27 15:27:49,965[DEBUG]logger_second(main.py).__init__(line158)/thread28020::[Logger.logger_second] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__logger_second.log]
+2024-04-27 15:27:49,966[DEBUG]logger_second(example1.py).<module>(line19)/thread28020::hello2-1
+2024-04-27 15:27:49,966[DEBUG]root(example1.py).<module>(line21)/thread28020::hello0-2
+2024-04-27 15:27:49,966[DEBUG]logger_first(example1.py).<module>(line22)/thread28020::hello1-2
+2024-04-27 15:27:49,966[DEBUG]logger_second(example1.py).<module>(line23)/thread28020::hello2-2
+2024-04-27 15:27:49,966[DEBUG]logger_dir(main.py).__init__(line152)/thread28020::====================================================================================================
+2024-04-27 15:27:49,967[DEBUG]logger_dir(main.py).__init__(line155)/thread28020::[Logger.logger_dir] start STREAM
+2024-04-27 15:27:49,968[DEBUG]logger_dir(main.py).__init__(line158)/thread28020::[Logger.logger_dir] start FILE=[c:\1\logger__logger_dir.log]
+2024-04-27 15:27:49,968[DEBUG]logger_dir(example1.py).<module>(line27)/thread28020::hello_dir
+2024-04-27 15:27:49,968[DEBUG]Example(main.py).__init__(line152)/thread28020::====================================================================================================
+2024-04-27 15:27:49,968[DEBUG]Example(main.py).__init__(line155)/thread28020::[Logger.Example] start STREAM
+2024-04-27 15:27:49,969[DEBUG]Example(main.py).__init__(line158)/thread28020::[Logger.Example] start FILE=[C:\__STARICHENKO_Element\PROJECTS\abc=logger_aux\EXAMPLES\logger__Example.log]
+2024-04-27 15:27:49,969[DEBUG]Example(example1.py).meth(line41)/thread28020::hello123
 ```
 
 ********************************************************************************
```

### Comparing `logger_aux-0.0.7/setup.py` & `logger_aux-0.0.8/setup.py`

 * *Files identical despite different names*

