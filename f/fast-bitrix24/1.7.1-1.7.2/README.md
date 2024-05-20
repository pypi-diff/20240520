# Comparing `tmp/fast_bitrix24-1.7.1.tar.gz` & `tmp/fast_bitrix24-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_bitrix24-1.7.1.tar", last modified: Wed Apr  3 19:42:18 2024, max compression
+gzip compressed data, was "fast_bitrix24-1.7.2.tar", last modified: Mon May 20 10:39:36 2024, max compression
```

## Comparing `fast_bitrix24-1.7.1.tar` & `fast_bitrix24-1.7.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:42:18.739182 fast_bitrix24-1.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-03 19:42:00.000000 fast_bitrix24-1.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    21752 2024-04-03 19:42:18.739182 fast_bitrix24-1.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20848 2024-04-03 19:42:00.000000 fast_bitrix24-1.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:42:18.735182 fast_bitrix24-1.7.1/fast_bitrix24/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-03 19:42:00.000000 fast_bitrix24-1.7.1/fast_bitrix24/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 19:42:00.000000 fast_bitrix24-1.7.1/fast_bitrix24/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11212 2024-04-03 19:42:00.000000 fast_bitrix24-1.7.1/fast_bitrix24/bitrix.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-03 19:42:00.000000 fast_bitrix24-1.7.1/fast_bitrix24/correct_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-03 19:42:00.000000 fast_bitrix24-1.7.1/fast_bitrix24/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-04-03 19:42:00.000000 fast_bitrix24-1.7.1/fast_bitrix24/mult_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-03 19:42:00.000000 fast_bitrix24-1.7.1/fast_bitrix24/server_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10273 2024-04-03 19:42:00.000000 fast_bitrix24-1.7.1/fast_bitrix24/srh.py
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-04-03 19:42:00.000000 fast_bitrix24-1.7.1/fast_bitrix24/throttle.py
--rw-r--r--   0 runner    (1001) docker     (127)    15253 2024-04-03 19:42:00.000000 fast_bitrix24-1.7.1/fast_bitrix24/user_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-03 19:42:00.000000 fast_bitrix24-1.7.1/fast_bitrix24/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:42:18.739182 fast_bitrix24-1.7.1/fast_bitrix24.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21752 2024-04-03 19:42:18.000000 fast_bitrix24-1.7.1/fast_bitrix24.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-03 19:42:18.000000 fast_bitrix24-1.7.1/fast_bitrix24.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:42:18.000000 fast_bitrix24-1.7.1/fast_bitrix24.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-03 19:42:18.000000 fast_bitrix24-1.7.1/fast_bitrix24.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 19:42:18.000000 fast_bitrix24-1.7.1/fast_bitrix24.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:42:18.739182 fast_bitrix24-1.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-03 19:42:00.000000 fast_bitrix24-1.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:42:18.739182 fast_bitrix24-1.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-03 19:42:00.000000 fast_bitrix24-1.7.1/tests/test_async.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-03 19:42:00.000000 fast_bitrix24-1.7.1/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-03 19:42:00.000000 fast_bitrix24-1.7.1/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-04-03 19:42:00.000000 fast_bitrix24-1.7.1/tests/test_server_responses.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-03 19:42:00.000000 fast_bitrix24-1.7.1/tests/test_srh.py
--rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-04-03 19:42:00.000000 fast_bitrix24-1.7.1/tests/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-03 19:42:00.000000 fast_bitrix24-1.7.1/tests/test_throttle.py
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-04-03 19:42:00.000000 fast_bitrix24-1.7.1/tests/test_warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:39:36.694682 fast_bitrix24-1.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-20 10:39:25.000000 fast_bitrix24-1.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    21752 2024-05-20 10:39:36.694682 fast_bitrix24-1.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20848 2024-05-20 10:39:25.000000 fast_bitrix24-1.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:39:36.690682 fast_bitrix24-1.7.2/fast_bitrix24/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-20 10:39:25.000000 fast_bitrix24-1.7.2/fast_bitrix24/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-20 10:39:25.000000 fast_bitrix24-1.7.2/fast_bitrix24/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11212 2024-05-20 10:39:25.000000 fast_bitrix24-1.7.2/fast_bitrix24/bitrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-20 10:39:25.000000 fast_bitrix24-1.7.2/fast_bitrix24/correct_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-20 10:39:25.000000 fast_bitrix24-1.7.2/fast_bitrix24/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-05-20 10:39:25.000000 fast_bitrix24-1.7.2/fast_bitrix24/mult_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-20 10:39:25.000000 fast_bitrix24-1.7.2/fast_bitrix24/server_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10273 2024-05-20 10:39:25.000000 fast_bitrix24-1.7.2/fast_bitrix24/srh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-20 10:39:25.000000 fast_bitrix24-1.7.2/fast_bitrix24/throttle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15389 2024-05-20 10:39:25.000000 fast_bitrix24-1.7.2/fast_bitrix24/user_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-20 10:39:25.000000 fast_bitrix24-1.7.2/fast_bitrix24/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:39:36.694682 fast_bitrix24-1.7.2/fast_bitrix24.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21752 2024-05-20 10:39:36.000000 fast_bitrix24-1.7.2/fast_bitrix24.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-20 10:39:36.000000 fast_bitrix24-1.7.2/fast_bitrix24.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 10:39:36.000000 fast_bitrix24-1.7.2/fast_bitrix24.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-20 10:39:36.000000 fast_bitrix24-1.7.2/fast_bitrix24.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-20 10:39:36.000000 fast_bitrix24-1.7.2/fast_bitrix24.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 10:39:36.694682 fast_bitrix24-1.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-20 10:39:25.000000 fast_bitrix24-1.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:39:36.694682 fast_bitrix24-1.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-20 10:39:25.000000 fast_bitrix24-1.7.2/tests/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-20 10:39:25.000000 fast_bitrix24-1.7.2/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-20 10:39:25.000000 fast_bitrix24-1.7.2/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-05-20 10:39:25.000000 fast_bitrix24-1.7.2/tests/test_server_responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-20 10:39:25.000000 fast_bitrix24-1.7.2/tests/test_srh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-05-20 10:39:25.000000 fast_bitrix24-1.7.2/tests/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-05-20 10:39:25.000000 fast_bitrix24-1.7.2/tests/test_throttle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-05-20 10:39:25.000000 fast_bitrix24-1.7.2/tests/test_warnings.py
```

### Comparing `fast_bitrix24-1.7.1/LICENSE` & `fast_bitrix24-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.1/PKG-INFO` & `fast_bitrix24-1.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast_bitrix24
-Version: 1.7.1
+Version: 1.7.2
 Summary: API wrapper для быстрого получения данных от Битрикс24 через REST API. Параллельные запросы к серверу, упаковка запросов в батчи, контроль скорости запросов, есть синхронный и асинхронный клиенты.
 Home-page: https://github.com/leshchenko1979/fast_bitrix24
 Author: Alexey Leshchenko
 Author-email: leshchenko@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fast_bitrix24-1.7.1/README.md` & `fast_bitrix24-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.1/fast_bitrix24/bitrix.py` & `fast_bitrix24-1.7.2/fast_bitrix24/bitrix.py`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.1/fast_bitrix24/logger.py` & `fast_bitrix24-1.7.2/fast_bitrix24/logger.py`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.1/fast_bitrix24/mult_request.py` & `fast_bitrix24-1.7.2/fast_bitrix24/mult_request.py`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.1/fast_bitrix24/server_response.py` & `fast_bitrix24-1.7.2/fast_bitrix24/server_response.py`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.1/fast_bitrix24/srh.py` & `fast_bitrix24-1.7.2/fast_bitrix24/srh.py`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.1/fast_bitrix24/throttle.py` & `fast_bitrix24-1.7.2/fast_bitrix24/throttle.py`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.1/fast_bitrix24/user_request.py` & `fast_bitrix24-1.7.2/fast_bitrix24/user_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,18 +25,19 @@
     "fast_bitrix24/logger",
 ]
 
 # методы, возвращающие только списки
 GET_ALL_ENDINGS = (".list", ".getlist", ".fields", ".getavaliableforpayment", ".types")
 
 # методы, возвращающие как списки, так и отдельные сущности
-AMBIGUOUS_ENDINGS = (".get", )
+AMBIGUOUS_ENDINGS = (".get",)
 
 ALL_ENDINGS = (*GET_ALL_ENDINGS, *AMBIGUOUS_ENDINGS)
 
+
 class UserRequestAbstract:
     @beartype
     @icontract.require(lambda method: method, "Method cannot be empty")
     def __init__(
         self,
         bitrix,
         method: str,
@@ -146,17 +147,18 @@
                 stacklevel=get_warning_stack_level(TOP_MOST_LIBRARY_MODULES),
             )
 
         if (
             self.st_params
             and "SELECT" in self.st_params
             and "*" in self.st_params["SELECT"]
+            and "filter" not in self.st_params
         ):
             warnings.warn(
-                "You are selecting all fields. Beware that this is time-consuming and "
+                "You are selecting all fields and no filter. Beware that this is time-consuming and "
                 "may lead to penalties from the Bitrix server.",
                 UserWarning,
                 stacklevel=get_warning_stack_level(TOP_MOST_LIBRARY_MODULES),
             )
 
         return True
 
@@ -172,17 +174,21 @@
         return self.results
 
     def add_order_parameter(self):
         # необходимо установить порядок сортировки, иначе сортировка
         # будет рандомная и сущности будут повторяться на разных страницах
 
         # ряд методов не признают параметра "order", для таких ничего не делаем
-        excluded_methods = {"crm.address.list", "documentgenerator.template.list"}
+        EXCLUDED_METHODS = {
+            "crm.address.list",
+            "documentgenerator.template.list",
+            "userfieldconfig.list",
+        }
 
-        if self.method in excluded_methods:
+        if self.st_method in EXCLUDED_METHODS:
             return
 
         order_clause = {"order": {"ID": "ASC"}}
 
         if self.params:
             if "ORDER" not in self.st_params:
                 self.params.update(order_clause)
@@ -342,14 +348,15 @@
         # как ключ словаря с результатами.
 
         self.item_list = [
             ChainMap(item, {self.ID_field_name: f"order{i:010}"})
             for i, item in enumerate(self.item_list)
         ]
 
+
 class RawCallUserRequest:
     """Отправляем на сервер один элемент, не обрабатывая его и не заворачивая в батчи.
 
     Нужно для устревших методов, которые принимают на вход список
     (https://github.com/leshchenko1979/fast_bitrix24/issues/157),
     а также для отправки на сервер значений None, которые преобразуются
     в строку при заворачивании в батч
```

### Comparing `fast_bitrix24-1.7.1/fast_bitrix24/utils.py` & `fast_bitrix24-1.7.2/fast_bitrix24/utils.py`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.1/fast_bitrix24.egg-info/PKG-INFO` & `fast_bitrix24-1.7.2/fast_bitrix24.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast_bitrix24
-Version: 1.7.1
+Version: 1.7.2
 Summary: API wrapper для быстрого получения данных от Битрикс24 через REST API. Параллельные запросы к серверу, упаковка запросов в батчи, контроль скорости запросов, есть синхронный и асинхронный клиенты.
 Home-page: https://github.com/leshchenko1979/fast_bitrix24
 Author: Alexey Leshchenko
 Author-email: leshchenko@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fast_bitrix24-1.7.1/fast_bitrix24.egg-info/SOURCES.txt` & `fast_bitrix24-1.7.2/fast_bitrix24.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.1/setup.py` & `fast_bitrix24-1.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.1/tests/test_async.py` & `fast_bitrix24-1.7.2/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.1/tests/test_exceptions.py` & `fast_bitrix24-1.7.2/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.1/tests/test_helpers.py` & `fast_bitrix24-1.7.2/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.1/tests/test_server_responses.py` & `fast_bitrix24-1.7.2/tests/test_server_responses.py`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.1/tests/test_srh.py` & `fast_bitrix24-1.7.2/tests/test_srh.py`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.1/tests/test_sync.py` & `fast_bitrix24-1.7.2/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.1/tests/test_throttle.py` & `fast_bitrix24-1.7.2/tests/test_throttle.py`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.1/tests/test_warnings.py` & `fast_bitrix24-1.7.2/tests/test_warnings.py`

 * *Files identical despite different names*

