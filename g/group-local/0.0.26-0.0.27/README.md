# Comparing `tmp/group_local-0.0.26.tar.gz` & `tmp/group_local-0.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "group_local-0.0.26.tar", last modified: Tue May 14 13:17:56 2024, max compression
+gzip compressed data, was "group_local-0.0.27.tar", last modified: Sun May 19 15:57:06 2024, max compression
```

## Comparing `group_local-0.0.26.tar` & `group_local-0.0.27.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:56.081808 group_local-0.0.26/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-14 13:17:56.081808 group_local-0.0.26/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:56.081808 group_local-0.0.26/group_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:56.081808 group_local-0.0.26/group_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:39.000000 group_local-0.0.26/group_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20135 2024-05-14 13:17:39.000000 group_local-0.0.26/group_local/src/group_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-14 13:17:39.000000 group_local-0.0.26/group_local/src/group_local_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:17:56.081808 group_local-0.0.26/group_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-14 13:17:56.000000 group_local-0.0.26/group_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-14 13:17:56.000000 group_local-0.0.26/group_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 13:17:56.000000 group_local-0.0.26/group_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-14 13:17:56.000000 group_local-0.0.26/group_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 13:17:56.000000 group_local-0.0.26/group_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-14 13:17:39.000000 group_local-0.0.26/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 13:17:56.081808 group_local-0.0.26/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-14 13:17:39.000000 group_local-0.0.26/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 15:57:06.449213 group_local-0.0.27/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-19 15:57:06.449213 group_local-0.0.27/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 15:57:06.445213 group_local-0.0.27/group_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 15:57:06.449213 group_local-0.0.27/group_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 15:56:48.000000 group_local-0.0.27/group_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20959 2024-05-19 15:56:48.000000 group_local-0.0.27/group_local/src/group_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-19 15:56:48.000000 group_local-0.0.27/group_local/src/group_local_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 15:57:06.449213 group_local-0.0.27/group_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-19 15:57:06.000000 group_local-0.0.27/group_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-19 15:57:06.000000 group_local-0.0.27/group_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 15:57:06.000000 group_local-0.0.27/group_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-19 15:57:06.000000 group_local-0.0.27/group_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-19 15:57:06.000000 group_local-0.0.27/group_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-19 15:56:48.000000 group_local-0.0.27/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 15:57:06.449213 group_local-0.0.27/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-19 15:56:48.000000 group_local-0.0.27/setup.py
```

### Comparing `group_local-0.0.26/PKG-INFO` & `group_local-0.0.27/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: group-local
-Version: 0.0.26
+Version: 0.0.27
 Summary: PyPI Package for Circles group-local Python
 Home-page: https://github.com/circles-zone/group-main-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `group_local-0.0.26/group_local/src/group_local.py` & `group_local-0.0.27/group_local/src/group_local.py`

 * *Files 3% similar despite different names*

```diff
@@ -367,7 +367,27 @@
             view_table_name="group_ml_also_not_approved_view", id_column_value=group_title, id_column_name="title",
             select_clause_value="group_id, group_ml_id")
         for group_ids_dict in group_ids_dicts_list:
             group_dict = self.get_group_dict_by_group_id(group_ids_dict.get('group_id'), group_ids_dict.get('group_ml_id'))
             groups.append(group_dict)
         logger.end(object={'groups': str(groups)})
         return groups
+
+    def get_all_groups_names(self, view_table_name: str = "group_ml_also_not_approved_view") -> list[str]:
+        logger.start()
+        if "ml" in view_table_name:
+            select_clause_value = "title"
+        else:
+            select_clause_value = "name"
+        groups_names_dict = self.select_multi_dict_by_where(
+            view_table_name="group_ml_also_not_approved_view",
+            where="end_timestamp IS NOT %s",
+            params=(None,),
+            distinct=True,
+            select_clause_value=select_clause_value
+        )
+        groups_names = []
+        for group_name_dict in groups_names_dict:
+            groups_name = group_name_dict.get(select_clause_value)
+            groups_names.append(groups_name)
+        logger.end(object={'groups_names': groups_names})
+        return groups_names
```

### Comparing `group_local-0.0.26/group_local/src/group_local_constants.py` & `group_local-0.0.27/group_local/src/group_local_constants.py`

 * *Files identical despite different names*

### Comparing `group_local-0.0.26/group_local.egg-info/PKG-INFO` & `group_local-0.0.27/group_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: group-local
-Version: 0.0.26
+Version: 0.0.27
 Summary: PyPI Package for Circles group-local Python
 Home-page: https://github.com/circles-zone/group-main-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `group_local-0.0.26/setup.py` & `group_local-0.0.27/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "group-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/group-local
-    version='0.0.26',
+    version='0.0.27',
     author="Circles",
     author_email="info@circles.life",
     description="PyPI Package for Circles group-local Python",
     long_description="PyPI Package for Circles group-local Python",
     long_description_content_type='text/markdown',
     url="https://github.com/circles-zone/group-main-local-python-package",
     packages=[package_dir],
```

