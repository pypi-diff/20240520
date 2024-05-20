# Comparing `tmp/dash_pydantic_form-0.1.4.tar.gz` & `tmp/dash_pydantic_form-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_pydantic_form-0.1.4.tar", last modified: Sat May 18 23:41:17 2024, max compression
+gzip compressed data, was "dash_pydantic_form-0.1.5.tar", last modified: Mon May 20 05:19:41 2024, max compression
```

## Comparing `dash_pydantic_form-0.1.4.tar` & `dash_pydantic_form-0.1.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 23:41:17.177666 dash_pydantic_form-0.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 23:41:17.169666 dash_pydantic_form-0.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 23:41:17.173666 dash_pydantic_form-0.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 23:41:17.173666 dash_pydantic_form-0.1.4/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     8672 2024-05-18 23:41:17.177666 dash_pydantic_form-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 23:41:17.173666 dash_pydantic_form-0.1.4/dash_pydantic_form/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/dash_pydantic_form/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 23:41:17.173666 dash_pydantic_form-0.1.4/dash_pydantic_form/fields/
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/dash_pydantic_form/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/dash_pydantic_form/fields/all_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    21910 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/dash_pydantic_form/fields/base_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    18943 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/dash_pydantic_form/fields/editabletable_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/dash_pydantic_form/fields/markdown_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     8536 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/dash_pydantic_form/fields/model_field.py
--rw-r--r--   0 runner    (1001) docker     (127)    21436 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/dash_pydantic_form/fields/model_list_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/dash_pydantic_form/form_section.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/dash_pydantic_form/ids.py
--rw-r--r--   0 runner    (1001) docker     (127)    18731 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/dash_pydantic_form/model_form.py
--rw-r--r--   0 runner    (1001) docker     (127)     8662 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/dash_pydantic_form/pydantic_form_scripts.js
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/dash_pydantic_form/pydantic_form_styles.css
--rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/dash_pydantic_form/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 23:41:17.177666 dash_pydantic_form-0.1.4/dash_pydantic_form.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8672 2024-05-18 23:41:17.000000 dash_pydantic_form-0.1.4/dash_pydantic_form.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-18 23:41:17.000000 dash_pydantic_form-0.1.4/dash_pydantic_form.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 23:41:17.000000 dash_pydantic_form-0.1.4/dash_pydantic_form.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-18 23:41:17.000000 dash_pydantic_form-0.1.4/dash_pydantic_form.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-18 23:41:17.000000 dash_pydantic_form-0.1.4/dash_pydantic_form.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 23:41:17.173666 dash_pydantic_form-0.1.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/docs/_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 23:41:17.177666 dash_pydantic_form-0.1.4/images/
--rwxr-xr-x   0 runner    (1001) docker     (127)    47789 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/images/conditionnally-visible-field.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)    55763 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/images/discriminated-union.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)    15290 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/images/editable-table.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     4506 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/images/form-sections.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    12406 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/images/model-list.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     8028 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/images/nested-model.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    16764 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/images/simple-form.png
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 23:41:17.177666 dash_pydantic_form-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/usage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:19:41.340027 dash_pydantic_form-0.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:19:41.336027 dash_pydantic_form-0.1.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:19:41.336027 dash_pydantic_form-0.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:19:41.336027 dash_pydantic_form-0.1.5/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8753 2024-05-20 05:19:41.340027 dash_pydantic_form-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8050 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:19:41.336027 dash_pydantic_form-0.1.5/dash_pydantic_form/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/dash_pydantic_form/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:19:41.340027 dash_pydantic_form-0.1.5/dash_pydantic_form/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/dash_pydantic_form/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/dash_pydantic_form/fields/all_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21910 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/dash_pydantic_form/fields/base_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18943 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/dash_pydantic_form/fields/editabletable_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/dash_pydantic_form/fields/markdown_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8536 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/dash_pydantic_form/fields/model_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21436 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/dash_pydantic_form/fields/model_list_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/dash_pydantic_form/form_section.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/dash_pydantic_form/ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18872 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/dash_pydantic_form/model_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8662 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/dash_pydantic_form/pydantic_form_scripts.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/dash_pydantic_form/pydantic_form_styles.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/dash_pydantic_form/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:19:41.340027 dash_pydantic_form-0.1.5/dash_pydantic_form.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8753 2024-05-20 05:19:41.000000 dash_pydantic_form-0.1.5/dash_pydantic_form.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-20 05:19:41.000000 dash_pydantic_form-0.1.5/dash_pydantic_form.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 05:19:41.000000 dash_pydantic_form-0.1.5/dash_pydantic_form.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-20 05:19:41.000000 dash_pydantic_form-0.1.5/dash_pydantic_form.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-20 05:19:41.000000 dash_pydantic_form-0.1.5/dash_pydantic_form.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:19:41.340027 dash_pydantic_form-0.1.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/docs/_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:19:41.340027 dash_pydantic_form-0.1.5/images/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    47789 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/images/conditionnally-visible-field.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)    55763 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/images/discriminated-union.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15290 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/images/editable-table.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4506 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/images/form-sections.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12406 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/images/model-list.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8028 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/images/nested-model.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16764 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/images/simple-form.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 05:19:41.340027 dash_pydantic_form-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-05-20 05:19:24.000000 dash_pydantic_form-0.1.5/usage.py
```

### Comparing `dash_pydantic_form-0.1.4/.github/workflows/publish.yaml` & `dash_pydantic_form-0.1.5/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.4/.gitignore` & `dash_pydantic_form-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.4/.vscode/launch.json` & `dash_pydantic_form-0.1.5/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.4/PKG-INFO` & `dash_pydantic_form-0.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-pydantic-form
-Version: 0.1.4
+Version: 0.1.5
 Summary: Create Dash forms from pydantic objects
 Author-email: Renaud Lainé <renaud.laine@enea-consulting.com>
 License: Copyright ENEA Australia Pty Ltd - All Rights Reserved. Proprietary and confidential
 Project-URL: Source, https://github.com/RenaudLN/dash-pydantic-form
 Requires-Python: <3.13,>=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: dash
@@ -18,14 +18,16 @@
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 
 # Dash pydantic form
 
 This package allows users to quickly create forms with Plotly Dash based on pydantic models.
 
+See the full docs at [dash-pydantic-form docs](https://pydf-docs.onrender.com).
+
 ## Getting started
 
 Install with pip
 
 ```sh
 pip install dash-pydantic-form
 ```
```

### Comparing `dash_pydantic_form-0.1.4/README.md` & `dash_pydantic_form-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Dash pydantic form
 
 This package allows users to quickly create forms with Plotly Dash based on pydantic models.
 
+See the full docs at [dash-pydantic-form docs](https://pydf-docs.onrender.com).
+
 ## Getting started
 
 Install with pip
 
 ```sh
 pip install dash-pydantic-form
 ```
```

### Comparing `dash_pydantic_form-0.1.4/dash_pydantic_form/__init__.py` & `dash_pydantic_form-0.1.5/dash_pydantic_form/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.4/dash_pydantic_form/fields/__init__.py` & `dash_pydantic_form-0.1.5/dash_pydantic_form/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.4/dash_pydantic_form/fields/all_fields.py` & `dash_pydantic_form-0.1.5/dash_pydantic_form/fields/all_fields.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.4/dash_pydantic_form/fields/base_fields.py` & `dash_pydantic_form-0.1.5/dash_pydantic_form/fields/base_fields.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.4/dash_pydantic_form/fields/editabletable_field.py` & `dash_pydantic_form-0.1.5/dash_pydantic_form/fields/editabletable_field.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.4/dash_pydantic_form/fields/markdown_field.py` & `dash_pydantic_form-0.1.5/dash_pydantic_form/fields/markdown_field.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.4/dash_pydantic_form/fields/model_field.py` & `dash_pydantic_form-0.1.5/dash_pydantic_form/fields/model_field.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.4/dash_pydantic_form/fields/model_list_field.py` & `dash_pydantic_form-0.1.5/dash_pydantic_form/fields/model_list_field.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.4/dash_pydantic_form/form_section.py` & `dash_pydantic_form-0.1.5/dash_pydantic_form/form_section.py`

 * *Files 24% similar despite different names*

```diff
@@ -38,28 +38,22 @@
     sections: list[FormSection]
         List of FormSection.
     remaining_fields_position: Literal["top", "bottom", "none"]
         Position of the fields not listed in the sections. Default "top".
     render: Literal["accordion", "tabs", "steps"]
         how the sections should be rendered. Possible values: "accordion", "tabs", "steps".
         Default "accordion".
-    excluded_fields: list[str] | None
-        List of field names to exclude from the form altogether, optional.
     render_kwargs: dict | None
         Additional render kwargs passed to the section render functions, optional.
         See `ModelForm.render_accordion_sections`, `ModelForm.render_tabs_sections` and
         `ModelForm.render_steps_sections`
     """
 
     sections: list[FormSection]
     remaining_fields_position: Position = "top"
     render: SectionRender = "accordion"
-    excluded_fields: list[str] | None = None
     render_kwargs: dict | None = None
 
     def model_post_init(self, _context):
         """Model post init."""
         if self.render_kwargs is None:
             self.render_kwargs = {}
-
-        if self.excluded_fields is None:
-            self.excluded_fields = []
```

### Comparing `dash_pydantic_form-0.1.4/dash_pydantic_form/ids.py` & `dash_pydantic_form-0.1.5/dash_pydantic_form/ids.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.4/dash_pydantic_form/model_form.py` & `dash_pydantic_form-0.1.5/dash_pydantic_form/model_form.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,16 @@
         representations will be used based on the field annotation.
         See `fields.get_default_repr`.
     sections: Sections | None
         List of form sections (optional). See `Sections`.
     submit_on_enter: bool
         Whether to submit the form on enter. Default False.
         Note: this may break the behaviour of some fields (e.g. editable table), use with caution.
+    excluded_fields: list[str] | None
+        List of field names to exclude from the form altogether, optional.
     """
 
     class ids:
         """Model form ids."""
 
         form = partial(form_base_id, "_pydf-form")
         main = partial(form_base_id, "_pydf-main")
@@ -95,14 +97,15 @@
         aio_id: str,
         form_id: str,
         path: str = "",
         fields_repr: dict[str, Union["BaseField", dict]] | None = None,
         sections: Sections | None = None,
         submit_on_enter: bool = False,
         discriminator: str | None = None,
+        excluded_fields: list[str] | None = None,
     ) -> None:
         from dash_pydantic_form.fields import get_default_repr
 
         with contextlib.suppress(Exception):
             if issubclass(item, BaseModel):
                 item = item.model_construct()
 
@@ -118,15 +121,15 @@
             discriminator_value = None if subitem is None else getattr(subitem, discriminator, None)
             subitem_cls, disc_vals = handle_discriminated(
                 item.__class__, path, subitem_cls, discriminator, discriminator_value
             )
 
         more_kwargs = {}
         for field_name, field_info in subitem_cls.model_fields.items():
-            if sections and field_name in sections.excluded_fields:
+            if field_name in excluded_fields:
                 continue
             # If discriminating field, ensure all discriminator values are shown
             # Also add required metadata for discriminator callback
             if disc_vals and field_name == discriminator:
                 field_info = deepcopy(field_info)  # noqa: PLW2901
                 field_info.annotation = Literal[disc_vals]
                 more_kwargs |= {"n_cols": 4, "field_id_meta": "discriminator"}
```

### Comparing `dash_pydantic_form-0.1.4/dash_pydantic_form/pydantic_form_scripts.js` & `dash_pydantic_form-0.1.5/dash_pydantic_form/pydantic_form_scripts.js`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.4/dash_pydantic_form/pydantic_form_styles.css` & `dash_pydantic_form-0.1.5/dash_pydantic_form/pydantic_form_styles.css`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.4/dash_pydantic_form/utils.py` & `dash_pydantic_form-0.1.5/dash_pydantic_form/utils.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.4/dash_pydantic_form.egg-info/PKG-INFO` & `dash_pydantic_form-0.1.5/dash_pydantic_form.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-pydantic-form
-Version: 0.1.4
+Version: 0.1.5
 Summary: Create Dash forms from pydantic objects
 Author-email: Renaud Lainé <renaud.laine@enea-consulting.com>
 License: Copyright ENEA Australia Pty Ltd - All Rights Reserved. Proprietary and confidential
 Project-URL: Source, https://github.com/RenaudLN/dash-pydantic-form
 Requires-Python: <3.13,>=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: dash
@@ -18,14 +18,16 @@
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 
 # Dash pydantic form
 
 This package allows users to quickly create forms with Plotly Dash based on pydantic models.
 
+See the full docs at [dash-pydantic-form docs](https://pydf-docs.onrender.com).
+
 ## Getting started
 
 Install with pip
 
 ```sh
 pip install dash-pydantic-form
 ```
```

### Comparing `dash_pydantic_form-0.1.4/dash_pydantic_form.egg-info/SOURCES.txt` & `dash_pydantic_form-0.1.5/dash_pydantic_form.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.4/images/conditionnally-visible-field.gif` & `dash_pydantic_form-0.1.5/images/conditionnally-visible-field.gif`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.4/images/discriminated-union.gif` & `dash_pydantic_form-0.1.5/images/discriminated-union.gif`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.4/images/editable-table.png` & `dash_pydantic_form-0.1.5/images/editable-table.png`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.4/images/form-sections.png` & `dash_pydantic_form-0.1.5/images/form-sections.png`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.4/images/model-list.png` & `dash_pydantic_form-0.1.5/images/model-list.png`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.4/images/nested-model.png` & `dash_pydantic_form-0.1.5/images/nested-model.png`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.4/images/simple-form.png` & `dash_pydantic_form-0.1.5/images/simple-form.png`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.4/pyproject.toml` & `dash_pydantic_form-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.4/usage.py` & `dash_pydantic_form-0.1.5/usage.py`

 * *Files identical despite different names*

