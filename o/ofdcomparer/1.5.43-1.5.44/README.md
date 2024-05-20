# Comparing `tmp/ofdcomparer-1.5.43.tar.gz` & `tmp/ofdcomparer-1.5.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofdcomparer-1.5.43.tar", last modified: Tue May 14 05:55:24 2024, max compression
+gzip compressed data, was "ofdcomparer-1.5.44.tar", last modified: Mon May 20 14:41:46 2024, max compression
```

## Comparing `ofdcomparer-1.5.43.tar` & `ofdcomparer-1.5.44.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 05:55:24.976123 ofdcomparer-1.5.43/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-20 08:16:51.000000 ofdcomparer-1.5.43/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1567 2024-05-14 05:55:24.976123 ofdcomparer-1.5.43/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      975 2023-11-06 21:06:45.000000 ofdcomparer-1.5.43/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 05:55:24.974123 ofdcomparer-1.5.43/ofdcomparer/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-20 08:16:51.000000 ofdcomparer-1.5.43/ofdcomparer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      458 2024-01-12 07:39:03.000000 ofdcomparer-1.5.43/ofdcomparer/allure_helper.py
--rw-rw-rw-   0 root         (0) root         (0)    21905 2024-05-14 05:55:09.000000 ofdcomparer-1.5.43/ofdcomparer/compare_ffd.py
--rw-rw-rw-   0 root         (0) root         (0)      145 2024-04-11 05:15:32.000000 ofdcomparer-1.5.43/ofdcomparer/configs.py
--rw-rw-rw-   0 root         (0) root         (0)    13995 2024-04-11 05:15:32.000000 ofdcomparer-1.5.43/ofdcomparer/convert.py
--rw-rw-rw-   0 root         (0) root         (0)    39683 2024-05-14 05:55:09.000000 ofdcomparer-1.5.43/ofdcomparer/dto10.py
--rw-rw-rw-   0 root         (0) root         (0)    38192 2024-04-11 05:15:32.000000 ofdcomparer-1.5.43/ofdcomparer/dto_error_descriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8301 2024-01-25 10:39:56.000000 ofdcomparer-1.5.43/ofdcomparer/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     1562 2024-04-11 15:37:51.000000 ofdcomparer-1.5.43/ofdcomparer/ofd_cri_atol.py
--rw-rw-rw-   0 root         (0) root         (0)     2183 2024-01-12 14:13:15.000000 ofdcomparer-1.5.43/ofdcomparer/ofd_taxcom.py
--rw-rw-rw-   0 root         (0) root         (0)    40745 2024-05-14 05:55:09.000000 ofdcomparer-1.5.43/ofdcomparer/tags_fn.py
--rw-rw-rw-   0 root         (0) root         (0)    10168 2024-04-11 05:15:32.000000 ofdcomparer-1.5.43/ofdcomparer/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 05:55:24.976123 ofdcomparer-1.5.43/ofdcomparer.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1567 2024-05-14 05:55:24.000000 ofdcomparer-1.5.43/ofdcomparer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      516 2024-05-14 05:55:24.000000 ofdcomparer-1.5.43/ofdcomparer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 05:55:24.000000 ofdcomparer-1.5.43/ofdcomparer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       70 2024-05-14 05:55:24.000000 ofdcomparer-1.5.43/ofdcomparer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-05-14 05:55:24.000000 ofdcomparer-1.5.43/ofdcomparer.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-14 05:55:24.977123 ofdcomparer-1.5.43/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      886 2024-05-14 05:55:09.000000 ofdcomparer-1.5.43/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 14:41:46.390858 ofdcomparer-1.5.44/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-19 13:19:58.000000 ofdcomparer-1.5.44/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1567 2024-05-20 14:41:46.391858 ofdcomparer-1.5.44/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      975 2023-11-01 17:56:55.000000 ofdcomparer-1.5.44/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 14:41:46.389858 ofdcomparer-1.5.44/ofdcomparer/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-19 13:19:58.000000 ofdcomparer-1.5.44/ofdcomparer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      458 2024-01-12 13:37:12.000000 ofdcomparer-1.5.44/ofdcomparer/allure_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)    21904 2024-05-20 14:41:30.000000 ofdcomparer-1.5.44/ofdcomparer/compare_ffd.py
+-rw-rw-rw-   0 root         (0) root         (0)      145 2024-04-06 09:21:48.000000 ofdcomparer-1.5.44/ofdcomparer/configs.py
+-rw-rw-rw-   0 root         (0) root         (0)    13995 2024-04-06 09:21:48.000000 ofdcomparer-1.5.44/ofdcomparer/convert.py
+-rw-rw-rw-   0 root         (0) root         (0)    39683 2024-05-20 14:41:30.000000 ofdcomparer-1.5.44/ofdcomparer/dto10.py
+-rw-rw-rw-   0 root         (0) root         (0)    38192 2024-04-06 09:32:23.000000 ofdcomparer-1.5.44/ofdcomparer/dto_error_descriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8301 2024-01-23 20:47:59.000000 ofdcomparer-1.5.44/ofdcomparer/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1562 2024-05-20 14:41:30.000000 ofdcomparer-1.5.44/ofdcomparer/ofd_cri_atol.py
+-rw-rw-rw-   0 root         (0) root         (0)     2183 2024-01-12 14:45:58.000000 ofdcomparer-1.5.44/ofdcomparer/ofd_taxcom.py
+-rw-rw-rw-   0 root         (0) root         (0)    40745 2024-05-20 14:41:30.000000 ofdcomparer-1.5.44/ofdcomparer/tags_fn.py
+-rw-rw-rw-   0 root         (0) root         (0)    10168 2024-03-09 15:40:06.000000 ofdcomparer-1.5.44/ofdcomparer/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 14:41:46.390858 ofdcomparer-1.5.44/ofdcomparer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1567 2024-05-20 14:41:46.000000 ofdcomparer-1.5.44/ofdcomparer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      516 2024-05-20 14:41:46.000000 ofdcomparer-1.5.44/ofdcomparer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 14:41:46.000000 ofdcomparer-1.5.44/ofdcomparer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2024-05-20 14:41:46.000000 ofdcomparer-1.5.44/ofdcomparer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-05-20 14:41:46.000000 ofdcomparer-1.5.44/ofdcomparer.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-20 14:41:46.391858 ofdcomparer-1.5.44/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      886 2024-05-20 14:41:30.000000 ofdcomparer-1.5.44/setup.py
```

### Comparing `ofdcomparer-1.5.43/PKG-INFO` & `ofdcomparer-1.5.44/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofdcomparer
-Version: 1.5.43
+Version: 1.5.44
 Summary: Библиотека для сравнивания ФД из ФН и ОФД
 Home-page: UNKNOWN
 Author-email: k.kabisova@atol.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ofdcomparer-1.5.43/README.md` & `ofdcomparer-1.5.44/README.md`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.43/ofdcomparer/compare_ffd.py` & `ofdcomparer-1.5.44/ofdcomparer/compare_ffd.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         self.etalon_value = None
         self.comparable_value = None
 
     def compare(self, comparable: dict, etalon: dict) -> bool:
         """
         Сравнение по тегам ФД из ФН и ОФД
         """
-        logging.debug(f"{inspect.currentframe().f_code.co_name} < {comparable=} {etalon=}")
+        logging.info(f"{inspect.currentframe().f_code.co_name} < {comparable=} {etalon=}")
         for key in etalon:
             if key in comparable:
                 if key in self.__white_list:
                     continue
                 try:
                     self.etalon_value = etalon[key]
                     self.comparable_value = comparable[key]
```

### Comparing `ofdcomparer-1.5.43/ofdcomparer/convert.py` & `ofdcomparer-1.5.44/ofdcomparer/convert.py`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.43/ofdcomparer/dto10.py` & `ofdcomparer-1.5.44/ofdcomparer/dto10.py`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.43/ofdcomparer/dto_error_descriptions.py` & `ofdcomparer-1.5.44/ofdcomparer/dto_error_descriptions.py`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.43/ofdcomparer/helpers.py` & `ofdcomparer-1.5.44/ofdcomparer/helpers.py`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.43/ofdcomparer/ofd_cri_atol.py` & `ofdcomparer-1.5.44/ofdcomparer/ofd_cri_atol.py`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.43/ofdcomparer/ofd_taxcom.py` & `ofdcomparer-1.5.44/ofdcomparer/ofd_taxcom.py`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.43/ofdcomparer/tags_fn.py` & `ofdcomparer-1.5.44/ofdcomparer/tags_fn.py`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.43/ofdcomparer/utils.py` & `ofdcomparer-1.5.44/ofdcomparer/utils.py`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.43/ofdcomparer.egg-info/PKG-INFO` & `ofdcomparer-1.5.44/ofdcomparer.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofdcomparer
-Version: 1.5.43
+Version: 1.5.44
 Summary: Библиотека для сравнивания ФД из ФН и ОФД
 Home-page: UNKNOWN
 Author-email: k.kabisova@atol.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ofdcomparer-1.5.43/ofdcomparer.egg-info/SOURCES.txt` & `ofdcomparer-1.5.44/ofdcomparer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.43/setup.py` & `ofdcomparer-1.5.44/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="ofdcomparer",
-    version="1.5.43",
+    version="1.5.44",
     long_description=long_description,
     description="Библиотека для сравнивания ФД из ФН и ОФД",
     packages=["ofdcomparer"],
     author_email="k.kabisova@atol.ru",
     install_requires=[
         "requests==2.31.0",
         "requests-toolbelt==1.0.0",
```

