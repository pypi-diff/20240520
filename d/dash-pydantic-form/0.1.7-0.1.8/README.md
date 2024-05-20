# Comparing `tmp/dash_pydantic_form-0.1.7.tar.gz` & `tmp/dash_pydantic_form-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_pydantic_form-0.1.7.tar", last modified: Mon May 20 08:30:58 2024, max compression
+gzip compressed data, was "dash_pydantic_form-0.1.8.tar", last modified: Mon May 20 10:08:17 2024, max compression
```

## Comparing `dash_pydantic_form-0.1.7.tar` & `dash_pydantic_form-0.1.8.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:30:58.110286 dash_pydantic_form-0.1.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:30:58.102286 dash_pydantic_form-0.1.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:30:58.102286 dash_pydantic_form-0.1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:30:58.102286 dash_pydantic_form-0.1.7/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     8753 2024-05-20 08:30:58.110286 dash_pydantic_form-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8050 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:30:58.106286 dash_pydantic_form-0.1.7/dash_pydantic_form/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/dash_pydantic_form/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:30:58.106286 dash_pydantic_form-0.1.7/dash_pydantic_form/fields/
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/dash_pydantic_form/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/dash_pydantic_form/fields/all_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    21910 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/dash_pydantic_form/fields/base_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    18943 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/dash_pydantic_form/fields/editabletable_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/dash_pydantic_form/fields/markdown_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     8536 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/dash_pydantic_form/fields/model_field.py
--rw-r--r--   0 runner    (1001) docker     (127)    21436 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/dash_pydantic_form/fields/model_list_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/dash_pydantic_form/form_section.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/dash_pydantic_form/ids.py
--rw-r--r--   0 runner    (1001) docker     (127)    18843 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/dash_pydantic_form/model_form.py
--rw-r--r--   0 runner    (1001) docker     (127)     8662 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/dash_pydantic_form/pydantic_form_scripts.js
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/dash_pydantic_form/pydantic_form_styles.css
--rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/dash_pydantic_form/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:30:58.110286 dash_pydantic_form-0.1.7/dash_pydantic_form.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8753 2024-05-20 08:30:58.000000 dash_pydantic_form-0.1.7/dash_pydantic_form.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-20 08:30:58.000000 dash_pydantic_form-0.1.7/dash_pydantic_form.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 08:30:58.000000 dash_pydantic_form-0.1.7/dash_pydantic_form.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-20 08:30:58.000000 dash_pydantic_form-0.1.7/dash_pydantic_form.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-20 08:30:58.000000 dash_pydantic_form-0.1.7/dash_pydantic_form.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:30:58.106286 dash_pydantic_form-0.1.7/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/docs/_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:30:58.110286 dash_pydantic_form-0.1.7/images/
--rwxr-xr-x   0 runner    (1001) docker     (127)    47789 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/images/conditionnally-visible-field.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)    55763 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/images/discriminated-union.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)    15290 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/images/editable-table.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     4506 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/images/form-sections.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    12406 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/images/model-list.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     8028 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/images/nested-model.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    16764 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/images/simple-form.png
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 08:30:58.110286 dash_pydantic_form-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/usage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:08:17.421362 dash_pydantic_form-0.1.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:08:17.413362 dash_pydantic_form-0.1.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:08:17.413362 dash_pydantic_form-0.1.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:08:17.413362 dash_pydantic_form-0.1.8/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8753 2024-05-20 10:08:17.421362 dash_pydantic_form-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8050 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:08:17.417362 dash_pydantic_form-0.1.8/dash_pydantic_form/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/dash_pydantic_form/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:08:17.417362 dash_pydantic_form-0.1.8/dash_pydantic_form/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/dash_pydantic_form/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/dash_pydantic_form/fields/all_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21910 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/dash_pydantic_form/fields/base_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18943 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/dash_pydantic_form/fields/editabletable_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/dash_pydantic_form/fields/markdown_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8536 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/dash_pydantic_form/fields/model_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21436 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/dash_pydantic_form/fields/model_list_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/dash_pydantic_form/form_section.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/dash_pydantic_form/ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18843 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/dash_pydantic_form/model_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8662 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/dash_pydantic_form/pydantic_form_scripts.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/dash_pydantic_form/pydantic_form_styles.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/dash_pydantic_form/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:08:17.421362 dash_pydantic_form-0.1.8/dash_pydantic_form.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8753 2024-05-20 10:08:17.000000 dash_pydantic_form-0.1.8/dash_pydantic_form.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-20 10:08:17.000000 dash_pydantic_form-0.1.8/dash_pydantic_form.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 10:08:17.000000 dash_pydantic_form-0.1.8/dash_pydantic_form.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-20 10:08:17.000000 dash_pydantic_form-0.1.8/dash_pydantic_form.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-20 10:08:17.000000 dash_pydantic_form-0.1.8/dash_pydantic_form.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:08:17.417362 dash_pydantic_form-0.1.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/docs/_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:08:17.421362 dash_pydantic_form-0.1.8/images/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    47789 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/images/conditionnally-visible-field.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)    55763 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/images/discriminated-union.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15290 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/images/editable-table.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4506 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/images/form-sections.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12406 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/images/model-list.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8028 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/images/nested-model.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16764 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/images/simple-form.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 10:08:17.421362 dash_pydantic_form-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-05-20 10:08:04.000000 dash_pydantic_form-0.1.8/usage.py
```

### Comparing `dash_pydantic_form-0.1.7/.github/workflows/publish.yaml` & `dash_pydantic_form-0.1.8/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.7/.gitignore` & `dash_pydantic_form-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.7/.vscode/launch.json` & `dash_pydantic_form-0.1.8/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.7/CHANGELOG.md` & `dash_pydantic_form-0.1.8/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.7/PKG-INFO` & `dash_pydantic_form-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-pydantic-form
-Version: 0.1.7
+Version: 0.1.8
 Summary: Create Dash forms from pydantic objects
 Author-email: Renaud Lainé <renaud.laine@enea-consulting.com>
 License: Copyright ENEA Australia Pty Ltd - All Rights Reserved. Proprietary and confidential
 Project-URL: Source, https://github.com/RenaudLN/dash-pydantic-form
 Requires-Python: <3.13,>=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: dash
```

### Comparing `dash_pydantic_form-0.1.7/README.md` & `dash_pydantic_form-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.7/dash_pydantic_form/__init__.py` & `dash_pydantic_form-0.1.8/dash_pydantic_form/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.7/dash_pydantic_form/fields/__init__.py` & `dash_pydantic_form-0.1.8/dash_pydantic_form/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.7/dash_pydantic_form/fields/all_fields.py` & `dash_pydantic_form-0.1.8/dash_pydantic_form/fields/all_fields.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.7/dash_pydantic_form/fields/base_fields.py` & `dash_pydantic_form-0.1.8/dash_pydantic_form/fields/base_fields.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.7/dash_pydantic_form/fields/editabletable_field.py` & `dash_pydantic_form-0.1.8/dash_pydantic_form/fields/editabletable_field.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.7/dash_pydantic_form/fields/markdown_field.py` & `dash_pydantic_form-0.1.8/dash_pydantic_form/fields/markdown_field.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.7/dash_pydantic_form/fields/model_field.py` & `dash_pydantic_form-0.1.8/dash_pydantic_form/fields/model_field.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.7/dash_pydantic_form/fields/model_list_field.py` & `dash_pydantic_form-0.1.8/dash_pydantic_form/fields/model_list_field.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.7/dash_pydantic_form/form_section.py` & `dash_pydantic_form-0.1.8/dash_pydantic_form/form_section.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.7/dash_pydantic_form/ids.py` & `dash_pydantic_form-0.1.8/dash_pydantic_form/ids.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.7/dash_pydantic_form/model_form.py` & `dash_pydantic_form-0.1.8/dash_pydantic_form/model_form.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.7/dash_pydantic_form/pydantic_form_scripts.js` & `dash_pydantic_form-0.1.8/dash_pydantic_form/pydantic_form_scripts.js`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.7/dash_pydantic_form/pydantic_form_styles.css` & `dash_pydantic_form-0.1.8/dash_pydantic_form/pydantic_form_styles.css`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 .pydantic-form-grid {
     --col-1-4: 1;
     --col-2-4: 2;
     --col-3-4: 3;
     --col-4-4: 4;
-    grid-template-columns: repeat(4, minmax(0, 1fr));
+    --sg-cols: 4 !important;
 }
 
 @container (max-width: 48rem) {
     .pydantic-form-grid {
         --col-1-4: 1;
         --col-2-4: 1;
         --col-3-4: 1;
         --col-4-4: 1;
-        grid-template-columns: repeat(1, minmax(0, 1fr));
+        --sg-cols: 1 !important;
     }
 }
 
 [data-mantine-color-scheme="dark"] .ag-theme-alpine.ag-themed {
     color-scheme: dark;
     --ag-background-color: #181d1f;
     --ag-foreground-color: #fff;
```

### Comparing `dash_pydantic_form-0.1.7/dash_pydantic_form/utils.py` & `dash_pydantic_form-0.1.8/dash_pydantic_form/utils.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.7/dash_pydantic_form.egg-info/PKG-INFO` & `dash_pydantic_form-0.1.8/dash_pydantic_form.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-pydantic-form
-Version: 0.1.7
+Version: 0.1.8
 Summary: Create Dash forms from pydantic objects
 Author-email: Renaud Lainé <renaud.laine@enea-consulting.com>
 License: Copyright ENEA Australia Pty Ltd - All Rights Reserved. Proprietary and confidential
 Project-URL: Source, https://github.com/RenaudLN/dash-pydantic-form
 Requires-Python: <3.13,>=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: dash
```

### Comparing `dash_pydantic_form-0.1.7/dash_pydantic_form.egg-info/SOURCES.txt` & `dash_pydantic_form-0.1.8/dash_pydantic_form.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.7/images/conditionnally-visible-field.gif` & `dash_pydantic_form-0.1.8/images/conditionnally-visible-field.gif`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.7/images/discriminated-union.gif` & `dash_pydantic_form-0.1.8/images/discriminated-union.gif`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.7/images/editable-table.png` & `dash_pydantic_form-0.1.8/images/editable-table.png`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.7/images/form-sections.png` & `dash_pydantic_form-0.1.8/images/form-sections.png`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.7/images/model-list.png` & `dash_pydantic_form-0.1.8/images/model-list.png`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.7/images/nested-model.png` & `dash_pydantic_form-0.1.8/images/nested-model.png`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.7/images/simple-form.png` & `dash_pydantic_form-0.1.8/images/simple-form.png`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.7/pyproject.toml` & `dash_pydantic_form-0.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.7/usage.py` & `dash_pydantic_form-0.1.8/usage.py`

 * *Files identical despite different names*

