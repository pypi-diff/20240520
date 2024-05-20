# Comparing `tmp/ysfutils-1.0.15.tar.gz` & `tmp/ysfutils-1.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ysfutils-1.0.15.tar", last modified: Wed Mar 27 13:53:46 2024, max compression
+gzip compressed data, was "ysfutils-1.0.16.tar", last modified: Mon May 20 09:00:46 2024, max compression
```

## Comparing `ysfutils-1.0.15.tar` & `ysfutils-1.0.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 yingsf     (501) staff       (20)        0 2024-03-27 13:53:46.425974 ysfutils-1.0.15/
--rw-r--r--   0 yingsf     (501) staff       (20)     1068 2024-03-26 11:33:15.000000 ysfutils-1.0.15/LICENSE
--rw-r--r--   0 yingsf     (501) staff       (20)       69 2024-03-26 11:33:15.000000 ysfutils-1.0.15/MANIFEST.in
--rw-r--r--   0 yingsf     (501) staff       (20)     6700 2024-03-27 13:53:46.425873 ysfutils-1.0.15/PKG-INFO
--rw-r--r--   0 yingsf     (501) staff       (20)     5633 2024-03-26 11:33:15.000000 ysfutils-1.0.15/README.md
--rw-r--r--   0 yingsf     (501) staff       (20)      237 2024-03-27 13:53:46.426367 ysfutils-1.0.15/setup.cfg
--rw-r--r--   0 yingsf     (501) staff       (20)     4196 2024-03-26 11:49:23.000000 ysfutils-1.0.15/setup.py
-drwxr-xr-x   0 yingsf     (501) staff       (20)        0 2024-03-27 13:53:46.423585 ysfutils-1.0.15/ysfutils/
--rw-r--r--   0 yingsf     (501) staff       (20)      271 2024-03-27 13:53:32.000000 ysfutils-1.0.15/ysfutils/__init__.py
--rw-r--r--   0 yingsf     (501) staff       (20)    10775 2024-03-26 11:37:29.000000 ysfutils-1.0.15/ysfutils/config.py
--rw-r--r--   0 yingsf     (501) staff       (20)      808 2024-03-26 11:33:15.000000 ysfutils-1.0.15/ysfutils/dataframe.py
--rw-r--r--   0 yingsf     (501) staff       (20)      952 2024-03-26 11:33:15.000000 ysfutils-1.0.15/ysfutils/dingding.py
--rw-r--r--   0 yingsf     (501) staff       (20)      539 2024-03-27 13:53:19.000000 ysfutils-1.0.15/ysfutils/error.py
--rw-r--r--   0 yingsf     (501) staff       (20)     2735 2024-03-26 11:33:15.000000 ysfutils-1.0.15/ysfutils/github.py
--rw-r--r--   0 yingsf     (501) staff       (20)    18781 2024-03-26 11:33:15.000000 ysfutils-1.0.15/ysfutils/job.py
--rw-r--r--   0 yingsf     (501) staff       (20)     1986 2024-03-26 11:33:15.000000 ysfutils-1.0.15/ysfutils/list.py
--rw-r--r--   0 yingsf     (501) staff       (20)     7615 2024-03-26 11:33:15.000000 ysfutils-1.0.15/ysfutils/mongo.py
--rw-r--r--   0 yingsf     (501) staff       (20)      824 2024-03-26 11:33:15.000000 ysfutils-1.0.15/ysfutils/pid.py
--rw-r--r--   0 yingsf     (501) staff       (20)     2614 2024-03-26 11:33:15.000000 ysfutils-1.0.15/ysfutils/sqlites.py
--rw-r--r--   0 yingsf     (501) staff       (20)    39632 2022-09-26 11:19:00.000000 ysfutils-1.0.15/ysfutils/ths.js
--rw-r--r--   0 yingsf     (501) staff       (20)      859 2024-03-26 11:45:12.000000 ysfutils-1.0.15/ysfutils/ths.py
-drwxr-xr-x   0 yingsf     (501) staff       (20)        0 2024-03-27 13:53:46.425418 ysfutils-1.0.15/ysfutils.egg-info/
--rw-r--r--   0 yingsf     (501) staff       (20)     6700 2024-03-27 13:53:46.000000 ysfutils-1.0.15/ysfutils.egg-info/PKG-INFO
--rw-r--r--   0 yingsf     (501) staff       (20)      446 2024-03-27 13:53:46.000000 ysfutils-1.0.15/ysfutils.egg-info/SOURCES.txt
--rw-r--r--   0 yingsf     (501) staff       (20)        1 2024-03-27 13:53:46.000000 ysfutils-1.0.15/ysfutils.egg-info/dependency_links.txt
--rw-r--r--   0 yingsf     (501) staff       (20)      139 2024-03-27 13:53:46.000000 ysfutils-1.0.15/ysfutils.egg-info/requires.txt
--rw-r--r--   0 yingsf     (501) staff       (20)        9 2024-03-27 13:53:46.000000 ysfutils-1.0.15/ysfutils.egg-info/top_level.txt
+drwxr-xr-x   0 yingsf     (501) staff       (20)        0 2024-05-20 09:00:46.355339 ysfutils-1.0.16/
+-rw-r--r--   0 yingsf     (501) staff       (20)     1068 2024-05-20 08:39:02.000000 ysfutils-1.0.16/LICENSE
+-rw-r--r--   0 yingsf     (501) staff       (20)       69 2024-05-20 08:39:02.000000 ysfutils-1.0.16/MANIFEST.in
+-rw-r--r--   0 yingsf     (501) staff       (20)     6701 2024-05-20 09:00:46.355289 ysfutils-1.0.16/PKG-INFO
+-rw-r--r--   0 yingsf     (501) staff       (20)     5633 2024-05-20 08:39:02.000000 ysfutils-1.0.16/README.md
+-rw-r--r--   0 yingsf     (501) staff       (20)      238 2024-05-20 09:00:46.355524 ysfutils-1.0.16/setup.cfg
+-rw-r--r--   0 yingsf     (501) staff       (20)     4197 2024-05-20 08:58:05.000000 ysfutils-1.0.16/setup.py
+drwxr-xr-x   0 yingsf     (501) staff       (20)        0 2024-05-20 09:00:46.354400 ysfutils-1.0.16/ysfutils/
+-rw-r--r--   0 yingsf     (501) staff       (20)      271 2024-05-20 08:57:01.000000 ysfutils-1.0.16/ysfutils/__init__.py
+-rw-r--r--   0 yingsf     (501) staff       (20)    11004 2024-05-20 08:57:01.000000 ysfutils-1.0.16/ysfutils/config.py
+-rw-r--r--   0 yingsf     (501) staff       (20)      808 2024-05-20 08:39:02.000000 ysfutils-1.0.16/ysfutils/dataframe.py
+-rw-r--r--   0 yingsf     (501) staff       (20)      952 2024-05-20 08:39:02.000000 ysfutils-1.0.16/ysfutils/dingding.py
+-rw-r--r--   0 yingsf     (501) staff       (20)      539 2024-05-20 08:39:02.000000 ysfutils-1.0.16/ysfutils/error.py
+-rw-r--r--   0 yingsf     (501) staff       (20)     2735 2024-05-20 08:39:02.000000 ysfutils-1.0.16/ysfutils/github.py
+-rw-r--r--   0 yingsf     (501) staff       (20)    18781 2024-05-20 08:39:02.000000 ysfutils-1.0.16/ysfutils/job.py
+-rw-r--r--   0 yingsf     (501) staff       (20)     1986 2024-05-20 08:39:02.000000 ysfutils-1.0.16/ysfutils/list.py
+-rw-r--r--   0 yingsf     (501) staff       (20)     7615 2024-05-20 08:39:02.000000 ysfutils-1.0.16/ysfutils/mongo.py
+-rw-r--r--   0 yingsf     (501) staff       (20)      824 2024-05-20 08:39:02.000000 ysfutils-1.0.16/ysfutils/pid.py
+-rw-r--r--   0 yingsf     (501) staff       (20)     2614 2024-05-20 08:39:02.000000 ysfutils-1.0.16/ysfutils/sqlites.py
+-rw-r--r--   0 yingsf     (501) staff       (20)    39632 2024-05-20 08:39:02.000000 ysfutils-1.0.16/ysfutils/ths.js
+-rw-r--r--   0 yingsf     (501) staff       (20)      859 2024-05-20 08:39:02.000000 ysfutils-1.0.16/ysfutils/ths.py
+drwxr-xr-x   0 yingsf     (501) staff       (20)        0 2024-05-20 09:00:46.355079 ysfutils-1.0.16/ysfutils.egg-info/
+-rw-r--r--   0 yingsf     (501) staff       (20)     6701 2024-05-20 09:00:46.000000 ysfutils-1.0.16/ysfutils.egg-info/PKG-INFO
+-rw-r--r--   0 yingsf     (501) staff       (20)      446 2024-05-20 09:00:46.000000 ysfutils-1.0.16/ysfutils.egg-info/SOURCES.txt
+-rw-r--r--   0 yingsf     (501) staff       (20)        1 2024-05-20 09:00:46.000000 ysfutils-1.0.16/ysfutils.egg-info/dependency_links.txt
+-rw-r--r--   0 yingsf     (501) staff       (20)      140 2024-05-20 09:00:46.000000 ysfutils-1.0.16/ysfutils.egg-info/requires.txt
+-rw-r--r--   0 yingsf     (501) staff       (20)        9 2024-05-20 09:00:46.000000 ysfutils-1.0.16/ysfutils.egg-info/top_level.txt
```

### Comparing `ysfutils-1.0.15/LICENSE` & `ysfutils-1.0.16/LICENSE`

 * *Files identical despite different names*

### Comparing `ysfutils-1.0.15/PKG-INFO` & `ysfutils-1.0.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ysfutils
-Version: 1.0.15
+Version: 1.0.16
 Summary: My library of frequently used tools.
 Home-page: https://github.com/yingsf/ysfutils
 Download-URL: https://github.com/yingsf/ysfutils/tarball/master
 Author: ShuFeng Ying
 Author-email: me@yingsf.com
 Maintainer: ShuFeng Ying
 Maintainer-email: me@yingsf.com
@@ -19,18 +19,18 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: APScheduler~=3.10.4
-Requires-Dist: Cython~=3.0.9
+Requires-Dist: Cython~=3.0.10
 Requires-Dist: loguru~=0.7.2
 Requires-Dist: py-mini-racer~=0.6.0
-Requires-Dist: pymongo~=4.6.2
+Requires-Dist: pymongo~=4.7.2
 Requires-Dist: pysqlcipher3~=1.2.0
 Requires-Dist: python-box~=7.1.1
 Requires-Dist: requests~=2.31.0
 
 # utils - 我常用的工具类
 
 ## 1. mongo
```

### Comparing `ysfutils-1.0.15/README.md` & `ysfutils-1.0.16/README.md`

 * *Files identical despite different names*

### Comparing `ysfutils-1.0.15/setup.py` & `ysfutils-1.0.16/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,18 +108,18 @@
         "Operating System :: MacOS",
         "Operating System :: Unix",
         "Programming Language :: Python :: 3 :: Only"
     ]
 
     REQUIRES = [
         "APScheduler~=3.10.4",
-        "Cython~=3.0.9",
+        "Cython~=3.0.10",
         "loguru~=0.7.2",
         "py-mini-racer~=0.6.0",
-        "pymongo~=4.6.2",
+        "pymongo~=4.7.2",
         "pysqlcipher3~=1.2.0",
         "python-box~=7.1.1",
         "requests~=2.31.0"
     ]
 
     setup(
         name=PKG_NAME,
```

### Comparing `ysfutils-1.0.15/ysfutils/config.py` & `ysfutils-1.0.16/ysfutils/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,17 +31,25 @@
                 }
             }
         2. 所有配置都在sqlite数据库中名字以_config结尾的各个表中存储
         3. MongoDB的证书文件存放路径和sqlite数据库文件所在路径平级
 
     """
 
-    def __init__(self):
+    def __init__(self, env_name: str = "RUN_ENV", config_table_list: None | list = None):
+        """
+
+        Args:
+            env_name: 环境变量名
+            config_table_list: 不传该参数时, 获取所有名字以_config结尾的表
+
+        """
         # 获取运行时参数
-        self.__run_env_dict = eval(os.getenv("RUN_ENV")) if os.getenv("RUN_ENV") else {}
+        self.__run_env_dict = eval(os.getenv(f"{env_name}")) if os.getenv(f"{env_name}") else {}
+        self.__config_table_list = config_table_list
 
     @property
     def all_config(self):
         path_config = self.__makedirs(self.__run_env_dict.get("path", {}))
         db_config = self.__get_config_from_sqlite3()
         all_config = {**path_config, **db_config}
 
@@ -66,20 +74,17 @@
             for path in eval(path_list):
                 path_name = Path(path).stem
                 os.makedirs(path, exist_ok=True)
                 if is_show == "show":
                     result["path"][path_name] = path
         return result
 
-    def __get_config_from_sqlite3(self, config_table_list: None | list = None) -> dict:
+    def __get_config_from_sqlite3(self) -> dict:
         """ 从本地sqlite3数据库的配置表中获取配置
 
-        Args:
-            config_table_list: 不传该参数时, 获取所有名字以_config结尾的表
-
         Notes:
             sqlite数据库中各参数表的表结构只有value一个字段, 内容为json字符串
 
         """
         all_config_from_db = {}
 
         mongo_db_list = eval(self.__run_env_dict.get("mongo", "[]"))
@@ -88,18 +93,20 @@
         sqlite3_db_path = self.__run_env_dict.get("sqlite3", {}).get("path", "")
         sqlite3_db_file, sqlite3_db_passwd_file = self.__get_configdb(sqlite3_db_path)
         with open(sqlite3_db_passwd_file, "r", encoding="utf-8") as file:
             db_passwd = file.read().rstrip("\n")
         client = Sqlite3Client(sqlite3_db_file, db_passwd)
 
         # 如果config_table_list入参的值为None, 则以sqlite数据库中所有以_config结尾的表名作为值
-        if config_table_list is None:
+        if self.__config_table_list is None:
             get_table_name_sql = 'select name from sqlite_master where name like "%_config"'
             query_result = client.find(get_table_name_sql, multi=True)
             config_table_list = [table_set[0] for table_set in query_result]
+        else:
+            config_table_list = self.__config_table_list
 
         for table_name in config_table_list:
             sql = f'select value from {table_name}'
             config = json.loads(client.find(sql, multi=False)[0])
             if table_name == "mongodb_config" and mongo_db_list and isinstance(mongo_db_list, list):
                 mongo_config = {"mongo_client": self.__get_mongo_config(config, mongo_db_list)}
                 all_config_from_db = dict(**all_config_from_db, **mongo_config)
```

### Comparing `ysfutils-1.0.15/ysfutils/dataframe.py` & `ysfutils-1.0.16/ysfutils/dataframe.py`

 * *Files identical despite different names*

### Comparing `ysfutils-1.0.15/ysfutils/dingding.py` & `ysfutils-1.0.16/ysfutils/dingding.py`

 * *Files identical despite different names*

### Comparing `ysfutils-1.0.15/ysfutils/error.py` & `ysfutils-1.0.16/ysfutils/error.py`

 * *Files identical despite different names*

### Comparing `ysfutils-1.0.15/ysfutils/github.py` & `ysfutils-1.0.16/ysfutils/github.py`

 * *Files identical despite different names*

### Comparing `ysfutils-1.0.15/ysfutils/job.py` & `ysfutils-1.0.16/ysfutils/job.py`

 * *Files identical despite different names*

### Comparing `ysfutils-1.0.15/ysfutils/list.py` & `ysfutils-1.0.16/ysfutils/list.py`

 * *Files identical despite different names*

### Comparing `ysfutils-1.0.15/ysfutils/mongo.py` & `ysfutils-1.0.16/ysfutils/mongo.py`

 * *Files identical despite different names*

### Comparing `ysfutils-1.0.15/ysfutils/pid.py` & `ysfutils-1.0.16/ysfutils/pid.py`

 * *Files identical despite different names*

### Comparing `ysfutils-1.0.15/ysfutils/sqlites.py` & `ysfutils-1.0.16/ysfutils/sqlites.py`

 * *Files identical despite different names*

### Comparing `ysfutils-1.0.15/ysfutils/ths.js` & `ysfutils-1.0.16/ysfutils/ths.js`

 * *Files identical despite different names*

### Comparing `ysfutils-1.0.15/ysfutils/ths.py` & `ysfutils-1.0.16/ysfutils/ths.py`

 * *Files identical despite different names*

### Comparing `ysfutils-1.0.15/ysfutils.egg-info/PKG-INFO` & `ysfutils-1.0.16/ysfutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ysfutils
-Version: 1.0.15
+Version: 1.0.16
 Summary: My library of frequently used tools.
 Home-page: https://github.com/yingsf/ysfutils
 Download-URL: https://github.com/yingsf/ysfutils/tarball/master
 Author: ShuFeng Ying
 Author-email: me@yingsf.com
 Maintainer: ShuFeng Ying
 Maintainer-email: me@yingsf.com
@@ -19,18 +19,18 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: APScheduler~=3.10.4
-Requires-Dist: Cython~=3.0.9
+Requires-Dist: Cython~=3.0.10
 Requires-Dist: loguru~=0.7.2
 Requires-Dist: py-mini-racer~=0.6.0
-Requires-Dist: pymongo~=4.6.2
+Requires-Dist: pymongo~=4.7.2
 Requires-Dist: pysqlcipher3~=1.2.0
 Requires-Dist: python-box~=7.1.1
 Requires-Dist: requests~=2.31.0
 
 # utils - 我常用的工具类
 
 ## 1. mongo
```

