# Comparing `tmp/dash_pydantic_form-0.1.5.tar.gz` & `tmp/dash_pydantic_form-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_pydantic_form-0.1.5.tar", last modified: Mon May 20 05:19:41 2024, max compression
+gzip compressed data, was "dash_pydantic_form-0.1.6.tar", last modified: Mon May 20 07:57:47 2024, max compression
```

## Comparing `dash_pydantic_form-0.1.5.tar` & `dash_pydantic_form-0.1.6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:19:41.340027 dash_pydantic_form-0.1.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:19:41.336027 dash_pydantic_form-0.1.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:19:41.336027 dash_pydantic_form-0.1.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:19:41.336027 dash_pydantic_form-0.1.5/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     8753 2024-05-20 05:19:41.340027 dash_pydantic_form-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8050 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:19:41.336027 dash_pydantic_form-0.1.5/dash_pydantic_form/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/dash_pydantic_form/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:19:41.340027 dash_pydantic_form-0.1.5/dash_pydantic_form/fields/
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/dash_pydantic_form/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/dash_pydantic_form/fields/all_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    21910 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/dash_pydantic_form/fields/base_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    18943 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/dash_pydantic_form/fields/editabletable_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/dash_pydantic_form/fields/markdown_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     8536 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/dash_pydantic_form/fields/model_field.py
--rw-r--r--   0 runner    (1001) docker     (127)    21436 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/dash_pydantic_form/fields/model_list_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/dash_pydantic_form/form_section.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/dash_pydantic_form/ids.py
--rw-r--r--   0 runner    (1001) docker     (127)    18872 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/dash_pydantic_form/model_form.py
--rw-r--r--   0 runner    (1001) docker     (127)     8662 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/dash_pydantic_form/pydantic_form_scripts.js
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/dash_pydantic_form/pydantic_form_styles.css
--rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/dash_pydantic_form/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:19:41.340027 dash_pydantic_form-0.1.5/dash_pydantic_form.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8753 2024-05-20 05:19:41.000000 dash_pydantic_form-0.1.5/dash_pydantic_form.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-20 05:19:41.000000 dash_pydantic_form-0.1.5/dash_pydantic_form.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 05:19:41.000000 dash_pydantic_form-0.1.5/dash_pydantic_form.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-20 05:19:41.000000 dash_pydantic_form-0.1.5/dash_pydantic_form.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-20 05:19:41.000000 dash_pydantic_form-0.1.5/dash_pydantic_form.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:19:41.340027 dash_pydantic_form-0.1.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/docs/_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:19:41.340027 dash_pydantic_form-0.1.5/images/
--rwxr-xr-x   0 runner    (1001) docker     (127)    47789 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/images/conditionnally-visible-field.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)    55763 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/images/discriminated-union.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)    15290 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/images/editable-table.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     4506 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/images/form-sections.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    12406 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/images/model-list.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     8028 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/images/nested-model.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    16764 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/images/simple-form.png
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 05:19:41.340027 dash_pydantic_form-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/usage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:57:47.720474 dash_pydantic_form-0.1.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:57:47.712473 dash_pydantic_form-0.1.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:57:47.712473 dash_pydantic_form-0.1.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:57:47.716474 dash_pydantic_form-0.1.6/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8753 2024-05-20 07:57:47.720474 dash_pydantic_form-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8050 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:57:47.716474 dash_pydantic_form-0.1.6/dash_pydantic_form/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/dash_pydantic_form/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:57:47.716474 dash_pydantic_form-0.1.6/dash_pydantic_form/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/dash_pydantic_form/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/dash_pydantic_form/fields/all_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21910 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/dash_pydantic_form/fields/base_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18943 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/dash_pydantic_form/fields/editabletable_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/dash_pydantic_form/fields/markdown_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8536 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/dash_pydantic_form/fields/model_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21436 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/dash_pydantic_form/fields/model_list_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/dash_pydantic_form/form_section.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/dash_pydantic_form/ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18810 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/dash_pydantic_form/model_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8662 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/dash_pydantic_form/pydantic_form_scripts.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/dash_pydantic_form/pydantic_form_styles.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/dash_pydantic_form/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:57:47.720474 dash_pydantic_form-0.1.6/dash_pydantic_form.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8753 2024-05-20 07:57:47.000000 dash_pydantic_form-0.1.6/dash_pydantic_form.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-20 07:57:47.000000 dash_pydantic_form-0.1.6/dash_pydantic_form.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 07:57:47.000000 dash_pydantic_form-0.1.6/dash_pydantic_form.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-20 07:57:47.000000 dash_pydantic_form-0.1.6/dash_pydantic_form.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-20 07:57:47.000000 dash_pydantic_form-0.1.6/dash_pydantic_form.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:57:47.716474 dash_pydantic_form-0.1.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/docs/_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:57:47.720474 dash_pydantic_form-0.1.6/images/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    47789 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/images/conditionnally-visible-field.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)    55763 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/images/discriminated-union.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15290 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/images/editable-table.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4506 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/images/form-sections.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12406 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/images/model-list.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8028 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/images/nested-model.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16764 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/images/simple-form.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 07:57:47.720474 dash_pydantic_form-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/usage.py
```

### Comparing `dash_pydantic_form-0.1.5/.github/workflows/publish.yaml` & `dash_pydantic_form-0.1.6/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.5/.gitignore` & `dash_pydantic_form-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.5/.vscode/launch.json` & `dash_pydantic_form-0.1.6/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.5/PKG-INFO` & `dash_pydantic_form-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-pydantic-form
-Version: 0.1.5
+Version: 0.1.6
 Summary: Create Dash forms from pydantic objects
 Author-email: Renaud Lainé <renaud.laine@enea-consulting.com>
 License: Copyright ENEA Australia Pty Ltd - All Rights Reserved. Proprietary and confidential
 Project-URL: Source, https://github.com/RenaudLN/dash-pydantic-form
 Requires-Python: <3.13,>=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: dash
```

### Comparing `dash_pydantic_form-0.1.5/README.md` & `dash_pydantic_form-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.5/dash_pydantic_form/__init__.py` & `dash_pydantic_form-0.1.6/dash_pydantic_form/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.5/dash_pydantic_form/fields/__init__.py` & `dash_pydantic_form-0.1.6/dash_pydantic_form/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.5/dash_pydantic_form/fields/all_fields.py` & `dash_pydantic_form-0.1.6/dash_pydantic_form/fields/all_fields.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.5/dash_pydantic_form/fields/base_fields.py` & `dash_pydantic_form-0.1.6/dash_pydantic_form/fields/base_fields.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.5/dash_pydantic_form/fields/editabletable_field.py` & `dash_pydantic_form-0.1.6/dash_pydantic_form/fields/editabletable_field.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.5/dash_pydantic_form/fields/markdown_field.py` & `dash_pydantic_form-0.1.6/dash_pydantic_form/fields/markdown_field.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.5/dash_pydantic_form/fields/model_field.py` & `dash_pydantic_form-0.1.6/dash_pydantic_form/fields/model_field.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.5/dash_pydantic_form/fields/model_list_field.py` & `dash_pydantic_form-0.1.6/dash_pydantic_form/fields/model_list_field.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.5/dash_pydantic_form/form_section.py` & `dash_pydantic_form-0.1.6/dash_pydantic_form/form_section.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.5/dash_pydantic_form/ids.py` & `dash_pydantic_form-0.1.6/dash_pydantic_form/ids.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.5/dash_pydantic_form/model_form.py` & `dash_pydantic_form-0.1.6/dash_pydantic_form/model_form.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,24 +200,23 @@
             if fields_repr
             else None
         )
         if not path:
             children.append(dcc.Store(id=self.ids.main(aio_id, form_id)))
             children.append(dcc.Store(data=str(item.__class__), id=self.ids.model_store(aio_id, form_id)))
 
-        if discriminator:
-            children.append(
-                dcc.Store(
-                    data={
-                        "sections": sections.model_dump(mode="json") if sections else None,
-                        "fields_repr": fields_repr_dicts,
-                    },
-                    id=self.ids.form_specs_store(aio_id, form_id, path),
-                )
+        children.append(
+            dcc.Store(
+                data={
+                    "sections": sections.model_dump(mode="json") if sections else None,
+                    "fields_repr": fields_repr_dicts,
+                },
+                id=self.ids.form_specs_store(aio_id, form_id, path),
             )
+        )
 
         super().__init__(
             children=children,
             **(
                 {
                     "id": self.ids.form(aio_id, form_id, path),
                     "data-entersubmits": submit_on_enter,
```

### Comparing `dash_pydantic_form-0.1.5/dash_pydantic_form/pydantic_form_scripts.js` & `dash_pydantic_form-0.1.6/dash_pydantic_form/pydantic_form_scripts.js`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.5/dash_pydantic_form/pydantic_form_styles.css` & `dash_pydantic_form-0.1.6/dash_pydantic_form/pydantic_form_styles.css`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.5/dash_pydantic_form/utils.py` & `dash_pydantic_form-0.1.6/dash_pydantic_form/utils.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.5/dash_pydantic_form.egg-info/PKG-INFO` & `dash_pydantic_form-0.1.6/dash_pydantic_form.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-pydantic-form
-Version: 0.1.5
+Version: 0.1.6
 Summary: Create Dash forms from pydantic objects
 Author-email: Renaud Lainé <renaud.laine@enea-consulting.com>
 License: Copyright ENEA Australia Pty Ltd - All Rights Reserved. Proprietary and confidential
 Project-URL: Source, https://github.com/RenaudLN/dash-pydantic-form
 Requires-Python: <3.13,>=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: dash
```

### Comparing `dash_pydantic_form-0.1.5/dash_pydantic_form.egg-info/SOURCES.txt` & `dash_pydantic_form-0.1.6/dash_pydantic_form.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.5/images/conditionnally-visible-field.gif` & `dash_pydantic_form-0.1.6/images/conditionnally-visible-field.gif`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.5/images/discriminated-union.gif` & `dash_pydantic_form-0.1.6/images/discriminated-union.gif`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.5/images/editable-table.png` & `dash_pydantic_form-0.1.6/images/editable-table.png`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.5/images/form-sections.png` & `dash_pydantic_form-0.1.6/images/form-sections.png`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.5/images/model-list.png` & `dash_pydantic_form-0.1.6/images/model-list.png`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.5/images/nested-model.png` & `dash_pydantic_form-0.1.6/images/nested-model.png`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.5/images/simple-form.png` & `dash_pydantic_form-0.1.6/images/simple-form.png`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.5/pyproject.toml` & `dash_pydantic_form-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.5/usage.py` & `dash_pydantic_form-0.1.6/usage.py`

 * *Files identical despite different names*

