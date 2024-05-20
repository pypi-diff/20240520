# Comparing `tmp/pmb_py-0.4.3.0.tar.gz` & `tmp/pmb_py-0.4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pmb_py-0.4.3.0.tar", last modified: Sat Sep  3 03:31:39 2022, max compression
+gzip compressed data, was "pmb_py-0.4.4.0.tar", last modified: Mon May 20 08:15:10 2024, max compression
```

## Comparing `pmb_py-0.4.3.0.tar` & `pmb_py-0.4.4.0.tar`

### file list

```diff
@@ -1,24 +1,35 @@
-drwxrwxr-x   0 noflame   (1000) noflame   (1000)        0 2022-09-03 03:31:39.000000 pmb_py-0.4.3.0/
--rw-rw-r--   0 noflame   (1000) noflame   (1000)     4951 2022-09-03 03:31:39.000000 pmb_py-0.4.3.0/PKG-INFO
--rw-rw-r--   0 noflame   (1000) noflame   (1000)     3266 2022-09-03 03:31:00.000000 pmb_py-0.4.3.0/README.md
--rw-rw-r--   0 noflame   (1000) noflame   (1000)       38 2022-09-03 03:31:39.000000 pmb_py-0.4.3.0/setup.cfg
--rw-rw-r--   0 noflame   (1000) noflame   (1000)      702 2022-09-03 03:31:00.000000 pmb_py-0.4.3.0/setup.py
-drwxrwxr-x   0 noflame   (1000) noflame   (1000)        0 2022-09-03 03:31:39.000000 pmb_py-0.4.3.0/src/
-drwxrwxr-x   0 noflame   (1000) noflame   (1000)        0 2022-09-03 03:31:39.000000 pmb_py-0.4.3.0/src/pmb_py/
--rw-rw-r--   0 noflame   (1000) noflame   (1000)      510 2021-09-01 07:19:59.000000 pmb_py-0.4.3.0/src/pmb_py/__init__.py
-drwxrwxr-x   0 noflame   (1000) noflame   (1000)        0 2022-09-03 03:31:39.000000 pmb_py-0.4.3.0/src/pmb_py/adapter/
--rw-rw-r--   0 noflame   (1000) noflame   (1000)        0 2021-08-20 07:23:03.000000 pmb_py-0.4.3.0/src/pmb_py/adapter/__init__.py
--rw-rw-r--   0 noflame   (1000) noflame   (1000)     1562 2022-07-20 10:15:35.000000 pmb_py-0.4.3.0/src/pmb_py/adapter/pmb_convert.py
--rw-rw-r--   0 noflame   (1000) noflame   (1000)     6128 2022-07-20 10:15:35.000000 pmb_py-0.4.3.0/src/pmb_py/api.py
--rw-rw-r--   0 noflame   (1000) noflame   (1000)     5686 2022-09-03 03:31:00.000000 pmb_py-0.4.3.0/src/pmb_py/core.py
-drwxrwxr-x   0 noflame   (1000) noflame   (1000)        0 2022-09-03 03:31:39.000000 pmb_py-0.4.3.0/src/pmb_py/domain/
--rw-rw-r--   0 noflame   (1000) noflame   (1000)        0 2021-08-20 07:23:03.000000 pmb_py-0.4.3.0/src/pmb_py/domain/__init__.py
--rw-rw-r--   0 noflame   (1000) noflame   (1000)     5654 2022-09-03 03:31:00.000000 pmb_py-0.4.3.0/src/pmb_py/domain/model.py
--rw-rw-r--   0 noflame   (1000) noflame   (1000)     2419 2022-07-20 10:15:35.000000 pmb_py-0.4.3.0/src/pmb_py/domain/query_result.py
--rw-rw-r--   0 noflame   (1000) noflame   (1000)     1754 2021-11-02 09:47:24.000000 pmb_py-0.4.3.0/src/pmb_py/spec.py
-drwxrwxr-x   0 noflame   (1000) noflame   (1000)        0 2022-09-03 03:31:39.000000 pmb_py-0.4.3.0/src/pmb_py.egg-info/
--rw-rw-r--   0 noflame   (1000) noflame   (1000)     4951 2022-09-03 03:31:39.000000 pmb_py-0.4.3.0/src/pmb_py.egg-info/PKG-INFO
--rw-rw-r--   0 noflame   (1000) noflame   (1000)      422 2022-09-03 03:31:39.000000 pmb_py-0.4.3.0/src/pmb_py.egg-info/SOURCES.txt
--rw-rw-r--   0 noflame   (1000) noflame   (1000)        1 2022-09-03 03:31:39.000000 pmb_py-0.4.3.0/src/pmb_py.egg-info/dependency_links.txt
--rw-rw-r--   0 noflame   (1000) noflame   (1000)       20 2022-09-03 03:31:39.000000 pmb_py-0.4.3.0/src/pmb_py.egg-info/requires.txt
--rw-rw-r--   0 noflame   (1000) noflame   (1000)        7 2022-09-03 03:31:39.000000 pmb_py-0.4.3.0/src/pmb_py.egg-info/top_level.txt
+drwxr-xr-x   0 noflame   (1000) noflame   (1000)        0 2024-05-20 08:15:10.087462 pmb_py-0.4.4.0/
+-rw-r--r--   0 noflame   (1000) noflame   (1000)     1064 2024-05-20 05:03:55.000000 pmb_py-0.4.4.0/LICENSE.txt
+-rw-r--r--   0 noflame   (1000) noflame   (1000)     3743 2024-05-20 08:15:10.087462 pmb_py-0.4.4.0/PKG-INFO
+-rw-r--r--   0 noflame   (1000) noflame   (1000)     3309 2024-05-20 08:11:26.000000 pmb_py-0.4.4.0/README.md
+-rw-r--r--   0 noflame   (1000) noflame   (1000)       38 2024-05-20 08:15:10.087462 pmb_py-0.4.4.0/setup.cfg
+-rw-r--r--   0 noflame   (1000) noflame   (1000)      702 2024-05-20 08:10:11.000000 pmb_py-0.4.4.0/setup.py
+drwxr-xr-x   0 noflame   (1000) noflame   (1000)        0 2024-05-20 08:15:10.087462 pmb_py-0.4.4.0/src/
+drwxr-xr-x   0 noflame   (1000) noflame   (1000)        0 2024-05-20 08:15:10.087462 pmb_py-0.4.4.0/src/pmb_py/
+-rw-r--r--   0 noflame   (1000) noflame   (1000)      510 2024-05-20 07:02:13.000000 pmb_py-0.4.4.0/src/pmb_py/__init__.py
+drwxr-xr-x   0 noflame   (1000) noflame   (1000)        0 2024-05-20 08:15:10.087462 pmb_py-0.4.4.0/src/pmb_py/adapter/
+-rw-r--r--   0 noflame   (1000) noflame   (1000)        0 2024-05-20 05:03:55.000000 pmb_py-0.4.4.0/src/pmb_py/adapter/__init__.py
+-rw-r--r--   0 noflame   (1000) noflame   (1000)     1562 2024-05-20 05:03:55.000000 pmb_py-0.4.4.0/src/pmb_py/adapter/pmb_convert.py
+-rw-r--r--   0 noflame   (1000) noflame   (1000)     6128 2024-05-20 07:42:22.000000 pmb_py-0.4.4.0/src/pmb_py/api.py
+-rw-r--r--   0 noflame   (1000) noflame   (1000)     5686 2024-05-20 07:26:27.000000 pmb_py-0.4.4.0/src/pmb_py/core.py
+drwxr-xr-x   0 noflame   (1000) noflame   (1000)        0 2024-05-20 08:15:10.087462 pmb_py-0.4.4.0/src/pmb_py/domain/
+-rw-r--r--   0 noflame   (1000) noflame   (1000)        0 2024-05-20 05:03:55.000000 pmb_py-0.4.4.0/src/pmb_py/domain/__init__.py
+-rw-r--r--   0 noflame   (1000) noflame   (1000)     5745 2024-05-20 08:09:38.000000 pmb_py-0.4.4.0/src/pmb_py/domain/model.py
+-rw-r--r--   0 noflame   (1000) noflame   (1000)     2419 2024-05-20 05:03:55.000000 pmb_py-0.4.4.0/src/pmb_py/domain/query_result.py
+-rw-r--r--   0 noflame   (1000) noflame   (1000)     1754 2024-05-20 08:07:55.000000 pmb_py-0.4.4.0/src/pmb_py/spec.py
+drwxr-xr-x   0 noflame   (1000) noflame   (1000)        0 2024-05-20 08:15:10.087462 pmb_py-0.4.4.0/src/pmb_py.egg-info/
+-rw-r--r--   0 noflame   (1000) noflame   (1000)     3743 2024-05-20 08:15:10.000000 pmb_py-0.4.4.0/src/pmb_py.egg-info/PKG-INFO
+-rw-r--r--   0 noflame   (1000) noflame   (1000)      676 2024-05-20 08:15:10.000000 pmb_py-0.4.4.0/src/pmb_py.egg-info/SOURCES.txt
+-rw-r--r--   0 noflame   (1000) noflame   (1000)        1 2024-05-20 08:15:10.000000 pmb_py-0.4.4.0/src/pmb_py.egg-info/dependency_links.txt
+-rw-r--r--   0 noflame   (1000) noflame   (1000)       20 2024-05-20 08:15:10.000000 pmb_py-0.4.4.0/src/pmb_py.egg-info/requires.txt
+-rw-r--r--   0 noflame   (1000) noflame   (1000)        7 2024-05-20 08:15:10.000000 pmb_py-0.4.4.0/src/pmb_py.egg-info/top_level.txt
+drwxr-xr-x   0 noflame   (1000) noflame   (1000)        0 2024-05-20 08:15:10.087462 pmb_py-0.4.4.0/tests/
+-rw-r--r--   0 noflame   (1000) noflame   (1000)     1462 2024-05-20 05:03:55.000000 pmb_py-0.4.4.0/tests/test_block_curd.py
+-rw-r--r--   0 noflame   (1000) noflame   (1000)      973 2024-05-20 05:03:55.000000 pmb_py-0.4.4.0/tests/test_gantt_item_curd.py
+-rw-r--r--   0 noflame   (1000) noflame   (1000)      380 2024-05-20 05:03:55.000000 pmb_py-0.4.4.0/tests/test_member_curd.py
+-rw-r--r--   0 noflame   (1000) noflame   (1000)      529 2024-05-20 05:03:55.000000 pmb_py-0.4.4.0/tests/test_pmb_gantt_api.py
+-rw-r--r--   0 noflame   (1000) noflame   (1000)      146 2024-05-20 05:03:55.000000 pmb_py-0.4.4.0/tests/test_pmb_login.py
+-rw-r--r--   0 noflame   (1000) noflame   (1000)      707 2024-05-20 05:03:55.000000 pmb_py-0.4.4.0/tests/test_project_curd.py
+-rw-r--r--   0 noflame   (1000) noflame   (1000)      455 2024-05-20 05:03:55.000000 pmb_py-0.4.4.0/tests/test_project_params.py
+-rw-r--r--   0 noflame   (1000) noflame   (1000)     1001 2024-05-20 05:03:55.000000 pmb_py-0.4.4.0/tests/test_task_curd.py
+-rw-r--r--   0 noflame   (1000) noflame   (1000)     1113 2024-05-20 05:03:55.000000 pmb_py-0.4.4.0/tests/test_taskgroup_curd.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pmb_py-0.4.3.0/README.md` & `pmb_py-0.4.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -126,14 +126,17 @@
 
 ## Projects
 ### list
 - 當給予 `member_id` 引數時其他引數將會無效，會回傳指定的 `member_id` 所有專案
 
 ### 歷史更新紀錄
 
+V 0.4.4
+增加對 is_evaluation 的支援
+
 V 0.4.3.0
 增加對應 Project 的 total extra cost 欄位
 
 V 0.4.2.1
 修正 cookie 的更名, 修正 header
 
 V 0.4.2
```

### Comparing `pmb_py-0.4.3.0/setup.py` & `pmb_py-0.4.4.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pmb_py",
-    version="0.4.3.0",
+    version="0.4.4.0",
     author="Noflame.lin",
     author_email="linjuang@gmail.com",
     description="pmb restful api python wrap",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/MoonShineVFX/pmb_py_api",
     install_requires=['requests', 'simplejson'],
```

### Comparing `pmb_py-0.4.3.0/src/pmb_py/adapter/pmb_convert.py` & `pmb_py-0.4.4.0/src/pmb_py/adapter/pmb_convert.py`

 * *Files identical despite different names*

### Comparing `pmb_py-0.4.3.0/src/pmb_py/api.py` & `pmb_py-0.4.4.0/src/pmb_py/api.py`

 * *Files identical despite different names*

### Comparing `pmb_py-0.4.3.0/src/pmb_py/core.py` & `pmb_py-0.4.4.0/src/pmb_py/core.py`

 * *Files identical despite different names*

### Comparing `pmb_py-0.4.3.0/src/pmb_py/domain/model.py` & `pmb_py-0.4.4.0/src/pmb_py/domain/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,19 +44,21 @@
                  sg_project_id: int = None,
                  contracted: bool = None,
                  is_deleted: bool = None,
                  tank_name: str = None,
                  backup_unc: str = None,
                  type_id: int = None,
                  hour_type: int = None,
+                 is_evaluation: bool = False,
                  total_group_budgets: float = None,
                  total_hours: float = None,
                  total_cost: float = None,
                  total_deductions: float = None,
                  total_extra_cost: float = None):
+
         self.id = id
         self.name = name
         self.type_id = type_id
         self.budget = budget
         self.budget_tax = budget_tax
         self.cost = cost
         self.profit = profit
@@ -86,14 +88,16 @@
         self.company_id = company_id
         self.sg_project_id = sg_project_id
         self.contracted = contracted
         self.is_deleted = is_deleted
         self.tank_name = tank_name
         self.backup_unc = backup_unc
         self.hour_type = hour_type
+        self.is_evaluation = is_evaluation
+
         self.total_group_budgets = total_group_budgets
         self.total_hours = total_hours
         self.total_cost = total_cost
         self.total_deductions = total_deductions
         self.total_extra_cost = total_extra_cost
 
     def __eq__(self, obj_b):
```

### Comparing `pmb_py-0.4.3.0/src/pmb_py/domain/query_result.py` & `pmb_py-0.4.4.0/src/pmb_py/domain/query_result.py`

 * *Files identical despite different names*

### Comparing `pmb_py-0.4.3.0/src/pmb_py/spec.py` & `pmb_py-0.4.4.0/src/pmb_py/spec.py`

 * *Files identical despite different names*

