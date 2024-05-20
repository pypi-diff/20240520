# Comparing `tmp/lbtool-1.3.4.tar.gz` & `tmp/lbtool-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lbtool-1.3.4.tar", last modified: Thu May 16 11:14:04 2024, max compression
+gzip compressed data, was "lbtool-1.3.5.tar", last modified: Mon May 20 14:05:02 2024, max compression
```

## Comparing `lbtool-1.3.4.tar` & `lbtool-1.3.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 11:14:04.351777 lbtool-1.3.4/
--rw-rw-rw-   0        0        0     5915 2024-05-16 11:14:04.350780 lbtool-1.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     5402 2024-01-17 07:02:08.000000 lbtool-1.3.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 11:14:04.343798 lbtool-1.3.4/lbTool/
--rw-rw-rw-   0        0        0     4492 2023-12-04 07:29:53.000000 lbtool-1.3.4/lbTool/Common.py
--rw-rw-rw-   0        0        0     1075 2023-11-08 02:54:21.000000 lbtool-1.3.4/lbTool/ConfigManager.py
--rw-rw-rw-   0        0        0    10446 2024-05-16 08:08:55.000000 lbtool-1.3.4/lbTool/Db.py
--rw-rw-rw-   0        0        0    18181 2024-05-15 16:26:28.000000 lbtool-1.3.4/lbTool/DmDb.py
--rw-rw-rw-   0        0        0     4063 2023-07-14 07:59:22.000000 lbtool-1.3.4/lbTool/EnCipher.py
--rw-rw-rw-   0        0        0     2280 2023-08-22 15:07:22.000000 lbtool-1.3.4/lbTool/FileUtil.py
--rw-rw-rw-   0        0        0     3140 2024-05-16 11:06:24.000000 lbtool-1.3.4/lbTool/Logging.py
--rw-rw-rw-   0        0        0        0 2023-07-25 07:51:14.000000 lbtool-1.3.4/lbTool/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 11:14:04.349782 lbtool-1.3.4/lbTool.egg-info/
--rw-rw-rw-   0        0        0     5915 2024-05-16 11:14:04.000000 lbtool-1.3.4/lbTool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2024-05-16 11:14:04.000000 lbtool-1.3.4/lbTool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 11:14:04.000000 lbtool-1.3.4/lbTool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      148 2024-05-16 11:14:04.000000 lbtool-1.3.4/lbTool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-16 11:14:04.000000 lbtool-1.3.4/lbTool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 11:14:04.351777 lbtool-1.3.4/setup.cfg
--rw-rw-rw-   0        0        0     1064 2024-05-16 11:11:01.000000 lbtool-1.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:05:02.861041 lbtool-1.3.5/
+-rw-rw-rw-   0        0        0     6018 2024-05-20 14:05:02.859086 lbtool-1.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5505 2024-05-20 14:03:32.000000 lbtool-1.3.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 14:05:02.847308 lbtool-1.3.5/lbTool/
+-rw-rw-rw-   0        0        0     4492 2024-01-25 15:49:04.000000 lbtool-1.3.5/lbTool/Common.py
+-rw-rw-rw-   0        0        0     1075 2024-01-25 15:49:04.000000 lbtool-1.3.5/lbTool/ConfigManager.py
+-rw-rw-rw-   0        0        0    10446 2024-05-16 15:08:28.000000 lbtool-1.3.5/lbTool/Db.py
+-rw-rw-rw-   0        0        0    18181 2024-05-16 15:08:28.000000 lbtool-1.3.5/lbTool/DmDb.py
+-rw-rw-rw-   0        0        0     4063 2024-01-25 15:49:04.000000 lbtool-1.3.5/lbTool/EnCipher.py
+-rw-rw-rw-   0        0        0     2280 2024-01-25 15:49:04.000000 lbtool-1.3.5/lbTool/FileUtil.py
+-rw-rw-rw-   0        0        0     3140 2024-05-16 15:08:28.000000 lbtool-1.3.5/lbTool/Logging.py
+-rw-rw-rw-   0        0        0        0 2024-01-25 15:49:04.000000 lbtool-1.3.5/lbTool/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:05:02.858108 lbtool-1.3.5/lbTool.egg-info/
+-rw-rw-rw-   0        0        0     6018 2024-05-20 14:05:02.000000 lbtool-1.3.5/lbTool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2024-05-20 14:05:02.000000 lbtool-1.3.5/lbTool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 14:05:02.000000 lbtool-1.3.5/lbTool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      148 2024-05-20 14:05:02.000000 lbtool-1.3.5/lbTool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-20 14:05:02.000000 lbtool-1.3.5/lbTool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 14:05:02.861041 lbtool-1.3.5/setup.cfg
+-rw-rw-rw-   0        0        0     1064 2024-05-20 14:03:32.000000 lbtool-1.3.5/setup.py
```

### Comparing `lbtool-1.3.4/PKG-INFO` & `lbtool-1.3.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbTool
-Version: 1.3.4
+Version: 1.3.5
 Summary: Multifunctional Toolset
 Author: lb
 Author-email: lcoolb@163.com
 Requires-Python: >=3.6, <3.11
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: gmSsl==3.2.2
@@ -140,19 +140,19 @@
 print("SM4解密后===", sm4_plaintext)
 ```
 ### 文件操作模块 lbTool.FileUtil
 内含：数据流写文件，合并PDF，Word转PDF
 ### 日志操作模块 lbTool.Logging
 默认在程序所在目录新建 Log/app_yyyymmdd.log 日志文件
 ```python
-from lbTool.Logging import Logger
+from lbTool.Logging import get_logger
 
 # 依靠log.yml配置文件获取参数，可查看下方配置文件区域
-# 获取日志处理器 默认fileLogger文件输出,为空则控制台输出
-logger = Logger()
+# 获取日志处理器 默认root文件,控制台输出,可单独指定
+logger = get_logger()
 logger.info("xxx")
 ```
 ## 配置文件
 ### 放在项目根路径config目录中 config.yml、log.yml
 config/config.yml
 <details>
 <summary>点击查看具体代码</summary>
@@ -181,35 +181,37 @@
 
 ```yaml
 # DEBUG->INFO->WARNING->ERROR->CRITICAL
 version: 1
 disable_existing_loggers: False
 formatters:
   simple:
-    format: "%(asctime)s[%(levelname)s] - %(message)s"
+    format: "%(asctime)s %(levelname)s %(filename)s|%(lineno)d - %(message)s"
   full:
-    format: "%(asctime)s[%(levelname)s]%(filename)s->%(funcName)s|%(lineno)d - %(message)s"
+    format: "%(asctime)s %(levelname)s %(filename)s|%(funcName)s|%(lineno)d - %(message)s"
 #    datefmt: "%F %T"
 handlers:
   console:
     class: logging.StreamHandler
     level: DEBUG
     formatter: full
+    stream: ext://sys.stdout
   file_handler:
     class: logging.handlers.RotatingFileHandler
     level: DEBUG
     formatter: simple
     filename: "app.log"
     maxBytes: 5242880
     backupCount: 1
     encoding: "utf8"
 loggers:
   fileLogger:
     level: DEBUG
     handlers: [file_handler]
+    propagate: yes
+  root:
+    level: DEBUG
+    handlers: [console,file_handler]
+#    handlers: [console]
     propagate: no
-root:
-  level: DEBUG
-  handlers: [console]
-  propagate: no
 ```
 </details>
```

### Comparing `lbtool-1.3.4/README.md` & `lbtool-1.3.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -121,19 +121,19 @@
 print("SM4解密后===", sm4_plaintext)
 ```
 ### 文件操作模块 lbTool.FileUtil
 内含：数据流写文件，合并PDF，Word转PDF
 ### 日志操作模块 lbTool.Logging
 默认在程序所在目录新建 Log/app_yyyymmdd.log 日志文件
 ```python
-from lbTool.Logging import Logger
+from lbTool.Logging import get_logger
 
 # 依靠log.yml配置文件获取参数，可查看下方配置文件区域
-# 获取日志处理器 默认fileLogger文件输出,为空则控制台输出
-logger = Logger()
+# 获取日志处理器 默认root文件,控制台输出,可单独指定
+logger = get_logger()
 logger.info("xxx")
 ```
 ## 配置文件
 ### 放在项目根路径config目录中 config.yml、log.yml
 config/config.yml
 <details>
 <summary>点击查看具体代码</summary>
@@ -162,35 +162,37 @@
 
 ```yaml
 # DEBUG->INFO->WARNING->ERROR->CRITICAL
 version: 1
 disable_existing_loggers: False
 formatters:
   simple:
-    format: "%(asctime)s[%(levelname)s] - %(message)s"
+    format: "%(asctime)s %(levelname)s %(filename)s|%(lineno)d - %(message)s"
   full:
-    format: "%(asctime)s[%(levelname)s]%(filename)s->%(funcName)s|%(lineno)d - %(message)s"
+    format: "%(asctime)s %(levelname)s %(filename)s|%(funcName)s|%(lineno)d - %(message)s"
 #    datefmt: "%F %T"
 handlers:
   console:
     class: logging.StreamHandler
     level: DEBUG
     formatter: full
+    stream: ext://sys.stdout
   file_handler:
     class: logging.handlers.RotatingFileHandler
     level: DEBUG
     formatter: simple
     filename: "app.log"
     maxBytes: 5242880
     backupCount: 1
     encoding: "utf8"
 loggers:
   fileLogger:
     level: DEBUG
     handlers: [file_handler]
+    propagate: yes
+  root:
+    level: DEBUG
+    handlers: [console,file_handler]
+#    handlers: [console]
     propagate: no
-root:
-  level: DEBUG
-  handlers: [console]
-  propagate: no
 ```
 </details>
```

### Comparing `lbtool-1.3.4/lbTool/Common.py` & `lbtool-1.3.5/lbTool/Common.py`

 * *Files identical despite different names*

### Comparing `lbtool-1.3.4/lbTool/ConfigManager.py` & `lbtool-1.3.5/lbTool/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `lbtool-1.3.4/lbTool/Db.py` & `lbtool-1.3.5/lbTool/Db.py`

 * *Files identical despite different names*

### Comparing `lbtool-1.3.4/lbTool/DmDb.py` & `lbtool-1.3.5/lbTool/DmDb.py`

 * *Files identical despite different names*

### Comparing `lbtool-1.3.4/lbTool/EnCipher.py` & `lbtool-1.3.5/lbTool/EnCipher.py`

 * *Files identical despite different names*

### Comparing `lbtool-1.3.4/lbTool/FileUtil.py` & `lbtool-1.3.5/lbTool/FileUtil.py`

 * *Files identical despite different names*

### Comparing `lbtool-1.3.4/lbTool/Logging.py` & `lbtool-1.3.5/lbTool/Logging.py`

 * *Files identical despite different names*

### Comparing `lbtool-1.3.4/lbTool.egg-info/PKG-INFO` & `lbtool-1.3.5/lbTool.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbTool
-Version: 1.3.4
+Version: 1.3.5
 Summary: Multifunctional Toolset
 Author: lb
 Author-email: lcoolb@163.com
 Requires-Python: >=3.6, <3.11
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: gmSsl==3.2.2
@@ -140,19 +140,19 @@
 print("SM4解密后===", sm4_plaintext)
 ```
 ### 文件操作模块 lbTool.FileUtil
 内含：数据流写文件，合并PDF，Word转PDF
 ### 日志操作模块 lbTool.Logging
 默认在程序所在目录新建 Log/app_yyyymmdd.log 日志文件
 ```python
-from lbTool.Logging import Logger
+from lbTool.Logging import get_logger
 
 # 依靠log.yml配置文件获取参数，可查看下方配置文件区域
-# 获取日志处理器 默认fileLogger文件输出,为空则控制台输出
-logger = Logger()
+# 获取日志处理器 默认root文件,控制台输出,可单独指定
+logger = get_logger()
 logger.info("xxx")
 ```
 ## 配置文件
 ### 放在项目根路径config目录中 config.yml、log.yml
 config/config.yml
 <details>
 <summary>点击查看具体代码</summary>
@@ -181,35 +181,37 @@
 
 ```yaml
 # DEBUG->INFO->WARNING->ERROR->CRITICAL
 version: 1
 disable_existing_loggers: False
 formatters:
   simple:
-    format: "%(asctime)s[%(levelname)s] - %(message)s"
+    format: "%(asctime)s %(levelname)s %(filename)s|%(lineno)d - %(message)s"
   full:
-    format: "%(asctime)s[%(levelname)s]%(filename)s->%(funcName)s|%(lineno)d - %(message)s"
+    format: "%(asctime)s %(levelname)s %(filename)s|%(funcName)s|%(lineno)d - %(message)s"
 #    datefmt: "%F %T"
 handlers:
   console:
     class: logging.StreamHandler
     level: DEBUG
     formatter: full
+    stream: ext://sys.stdout
   file_handler:
     class: logging.handlers.RotatingFileHandler
     level: DEBUG
     formatter: simple
     filename: "app.log"
     maxBytes: 5242880
     backupCount: 1
     encoding: "utf8"
 loggers:
   fileLogger:
     level: DEBUG
     handlers: [file_handler]
+    propagate: yes
+  root:
+    level: DEBUG
+    handlers: [console,file_handler]
+#    handlers: [console]
     propagate: no
-root:
-  level: DEBUG
-  handlers: [console]
-  propagate: no
 ```
 </details>
```

### Comparing `lbtool-1.3.4/setup.py` & `lbtool-1.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='lbTool',  # 包的名称
-    version='1.3.4',  # 版本号
+    version='1.3.5',  # 版本号
     author='lb',  # 作者名
     author_email='lcoolb@163.com',
     description='Multifunctional Toolset',  # 包的描述信息
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),  # 包含的所有包
     install_requires=[  # 依赖的其他包
```

