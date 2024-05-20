# Comparing `tmp/dash_pydantic_form-0.1.6.tar.gz` & `tmp/dash_pydantic_form-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_pydantic_form-0.1.6.tar", last modified: Mon May 20 07:57:47 2024, max compression
+gzip compressed data, was "dash_pydantic_form-0.1.7.tar", last modified: Mon May 20 08:30:58 2024, max compression
```

## Comparing `dash_pydantic_form-0.1.6.tar` & `dash_pydantic_form-0.1.7.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:57:47.720474 dash_pydantic_form-0.1.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:57:47.712473 dash_pydantic_form-0.1.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:57:47.712473 dash_pydantic_form-0.1.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:57:47.716474 dash_pydantic_form-0.1.6/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     8753 2024-05-20 07:57:47.720474 dash_pydantic_form-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8050 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:57:47.716474 dash_pydantic_form-0.1.6/dash_pydantic_form/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/dash_pydantic_form/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:57:47.716474 dash_pydantic_form-0.1.6/dash_pydantic_form/fields/
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/dash_pydantic_form/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/dash_pydantic_form/fields/all_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    21910 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/dash_pydantic_form/fields/base_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    18943 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/dash_pydantic_form/fields/editabletable_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/dash_pydantic_form/fields/markdown_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     8536 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/dash_pydantic_form/fields/model_field.py
--rw-r--r--   0 runner    (1001) docker     (127)    21436 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/dash_pydantic_form/fields/model_list_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/dash_pydantic_form/form_section.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/dash_pydantic_form/ids.py
--rw-r--r--   0 runner    (1001) docker     (127)    18810 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/dash_pydantic_form/model_form.py
--rw-r--r--   0 runner    (1001) docker     (127)     8662 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/dash_pydantic_form/pydantic_form_scripts.js
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/dash_pydantic_form/pydantic_form_styles.css
--rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/dash_pydantic_form/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:57:47.720474 dash_pydantic_form-0.1.6/dash_pydantic_form.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8753 2024-05-20 07:57:47.000000 dash_pydantic_form-0.1.6/dash_pydantic_form.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-20 07:57:47.000000 dash_pydantic_form-0.1.6/dash_pydantic_form.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 07:57:47.000000 dash_pydantic_form-0.1.6/dash_pydantic_form.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-20 07:57:47.000000 dash_pydantic_form-0.1.6/dash_pydantic_form.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-20 07:57:47.000000 dash_pydantic_form-0.1.6/dash_pydantic_form.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:57:47.716474 dash_pydantic_form-0.1.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/docs/_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:57:47.720474 dash_pydantic_form-0.1.6/images/
--rwxr-xr-x   0 runner    (1001) docker     (127)    47789 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/images/conditionnally-visible-field.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)    55763 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/images/discriminated-union.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)    15290 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/images/editable-table.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     4506 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/images/form-sections.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    12406 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/images/model-list.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     8028 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/images/nested-model.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    16764 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/images/simple-form.png
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 07:57:47.720474 dash_pydantic_form-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-05-20 07:57:33.000000 dash_pydantic_form-0.1.6/usage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:30:58.110286 dash_pydantic_form-0.1.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:30:58.102286 dash_pydantic_form-0.1.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:30:58.102286 dash_pydantic_form-0.1.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:30:58.102286 dash_pydantic_form-0.1.7/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8753 2024-05-20 08:30:58.110286 dash_pydantic_form-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8050 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:30:58.106286 dash_pydantic_form-0.1.7/dash_pydantic_form/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/dash_pydantic_form/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:30:58.106286 dash_pydantic_form-0.1.7/dash_pydantic_form/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/dash_pydantic_form/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/dash_pydantic_form/fields/all_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21910 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/dash_pydantic_form/fields/base_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18943 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/dash_pydantic_form/fields/editabletable_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/dash_pydantic_form/fields/markdown_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8536 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/dash_pydantic_form/fields/model_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21436 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/dash_pydantic_form/fields/model_list_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/dash_pydantic_form/form_section.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/dash_pydantic_form/ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18843 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/dash_pydantic_form/model_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8662 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/dash_pydantic_form/pydantic_form_scripts.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/dash_pydantic_form/pydantic_form_styles.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/dash_pydantic_form/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:30:58.110286 dash_pydantic_form-0.1.7/dash_pydantic_form.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8753 2024-05-20 08:30:58.000000 dash_pydantic_form-0.1.7/dash_pydantic_form.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-20 08:30:58.000000 dash_pydantic_form-0.1.7/dash_pydantic_form.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 08:30:58.000000 dash_pydantic_form-0.1.7/dash_pydantic_form.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-20 08:30:58.000000 dash_pydantic_form-0.1.7/dash_pydantic_form.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-20 08:30:58.000000 dash_pydantic_form-0.1.7/dash_pydantic_form.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:30:58.106286 dash_pydantic_form-0.1.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/docs/_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:30:58.110286 dash_pydantic_form-0.1.7/images/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    47789 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/images/conditionnally-visible-field.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)    55763 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/images/discriminated-union.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15290 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/images/editable-table.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4506 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/images/form-sections.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12406 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/images/model-list.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8028 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/images/nested-model.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16764 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/images/simple-form.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 08:30:58.110286 dash_pydantic_form-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-05-20 08:30:48.000000 dash_pydantic_form-0.1.7/usage.py
```

### Comparing `dash_pydantic_form-0.1.6/.github/workflows/publish.yaml` & `dash_pydantic_form-0.1.7/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.6/.gitignore` & `dash_pydantic_form-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.6/.vscode/launch.json` & `dash_pydantic_form-0.1.7/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.6/CHANGELOG.md` & `dash_pydantic_form-0.1.7/CHANGELOG.md`

 * *Files 21% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.1.7] - 2024-05-20
+### Changed
+- Use container query to ensure the columns shrink when the form container is small
+
 ## [0.1.6] - 2024-05-20
 ### Changed
 - Always store form specs in in a `ids.form_specs_store`, not just for discriminated unions
 
 ## [0.1.5] - 2024-05-20
 ### Changed
 - BREAKING: Moved `excluded_fields` from `Sections` to `ModelForm`
```

### Comparing `dash_pydantic_form-0.1.6/PKG-INFO` & `dash_pydantic_form-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-pydantic-form
-Version: 0.1.6
+Version: 0.1.7
 Summary: Create Dash forms from pydantic objects
 Author-email: Renaud Lainé <renaud.laine@enea-consulting.com>
 License: Copyright ENEA Australia Pty Ltd - All Rights Reserved. Proprietary and confidential
 Project-URL: Source, https://github.com/RenaudLN/dash-pydantic-form
 Requires-Python: <3.13,>=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: dash
```

### Comparing `dash_pydantic_form-0.1.6/README.md` & `dash_pydantic_form-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.6/dash_pydantic_form/__init__.py` & `dash_pydantic_form-0.1.7/dash_pydantic_form/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.6/dash_pydantic_form/fields/__init__.py` & `dash_pydantic_form-0.1.7/dash_pydantic_form/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.6/dash_pydantic_form/fields/all_fields.py` & `dash_pydantic_form-0.1.7/dash_pydantic_form/fields/all_fields.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.6/dash_pydantic_form/fields/base_fields.py` & `dash_pydantic_form-0.1.7/dash_pydantic_form/fields/base_fields.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.6/dash_pydantic_form/fields/editabletable_field.py` & `dash_pydantic_form-0.1.7/dash_pydantic_form/fields/editabletable_field.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.6/dash_pydantic_form/fields/markdown_field.py` & `dash_pydantic_form-0.1.7/dash_pydantic_form/fields/markdown_field.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.6/dash_pydantic_form/fields/model_field.py` & `dash_pydantic_form-0.1.7/dash_pydantic_form/fields/model_field.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.6/dash_pydantic_form/fields/model_list_field.py` & `dash_pydantic_form-0.1.7/dash_pydantic_form/fields/model_list_field.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.6/dash_pydantic_form/form_section.py` & `dash_pydantic_form-0.1.7/dash_pydantic_form/form_section.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.6/dash_pydantic_form/ids.py` & `dash_pydantic_form-0.1.7/dash_pydantic_form/ids.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.6/dash_pydantic_form/model_form.py` & `dash_pydantic_form-0.1.7/dash_pydantic_form/model_form.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
             discriminator_value = None if subitem is None else getattr(subitem, discriminator, None)
             subitem_cls, disc_vals = handle_discriminated(
                 item.__class__, path, subitem_cls, discriminator, discriminator_value
             )
 
         more_kwargs = {}
         for field_name, field_info in subitem_cls.model_fields.items():
-            if field_name in excluded_fields:
+            if field_name in (excluded_fields or []):
                 continue
             # If discriminating field, ensure all discriminator values are shown
             # Also add required metadata for discriminator callback
             if disc_vals and field_name == discriminator:
                 field_info = deepcopy(field_info)  # noqa: PLW2901
                 field_info.annotation = Literal[disc_vals]
                 more_kwargs |= {"n_cols": 4, "field_id_meta": "discriminator"}
@@ -212,28 +212,29 @@
                 },
                 id=self.ids.form_specs_store(aio_id, form_id, path),
             )
         )
 
         super().__init__(
             children=children,
+            style={"containerType": "inline-size"},
             **(
                 {
                     "id": self.ids.form(aio_id, form_id, path),
                     "data-entersubmits": submit_on_enter,
                 }
                 if not path
                 else {}
             ),
         )
 
     @classmethod
     def grid(cls, children: Children, **kwargs):
         """Create the responsive grid for a field."""
-        return dmc.SimpleGrid(children, cols={"base": 1, "sm": 4}, className="pydantic-form-grid", **kwargs)
+        return dmc.SimpleGrid(children, className="pydantic-form-grid", **kwargs)
 
     @classmethod
     def render_accordion_sections(  # noqa: PLR0913
         cls,
         *,
         aio_id: str,
         form_id: str,
```

### Comparing `dash_pydantic_form-0.1.6/dash_pydantic_form/pydantic_form_scripts.js` & `dash_pydantic_form-0.1.7/dash_pydantic_form/pydantic_form_scripts.js`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.6/dash_pydantic_form/pydantic_form_styles.css` & `dash_pydantic_form-0.1.7/dash_pydantic_form/pydantic_form_styles.css`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 .pydantic-form-grid {
     --col-1-4: 1;
     --col-2-4: 2;
     --col-3-4: 3;
     --col-4-4: 4;
+    grid-template-columns: repeat(4, minmax(0, 1fr));
 }
 
-@media (max-width: 48em) {
+@container (max-width: 48rem) {
     .pydantic-form-grid {
         --col-1-4: 1;
         --col-2-4: 1;
         --col-3-4: 1;
         --col-4-4: 1;
+        grid-template-columns: repeat(1, minmax(0, 1fr));
     }
 }
 
 [data-mantine-color-scheme="dark"] .ag-theme-alpine.ag-themed {
     color-scheme: dark;
     --ag-background-color: #181d1f;
     --ag-foreground-color: #fff;
```

### Comparing `dash_pydantic_form-0.1.6/dash_pydantic_form/utils.py` & `dash_pydantic_form-0.1.7/dash_pydantic_form/utils.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.6/dash_pydantic_form.egg-info/PKG-INFO` & `dash_pydantic_form-0.1.7/dash_pydantic_form.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-pydantic-form
-Version: 0.1.6
+Version: 0.1.7
 Summary: Create Dash forms from pydantic objects
 Author-email: Renaud Lainé <renaud.laine@enea-consulting.com>
 License: Copyright ENEA Australia Pty Ltd - All Rights Reserved. Proprietary and confidential
 Project-URL: Source, https://github.com/RenaudLN/dash-pydantic-form
 Requires-Python: <3.13,>=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: dash
```

### Comparing `dash_pydantic_form-0.1.6/dash_pydantic_form.egg-info/SOURCES.txt` & `dash_pydantic_form-0.1.7/dash_pydantic_form.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.6/images/conditionnally-visible-field.gif` & `dash_pydantic_form-0.1.7/images/conditionnally-visible-field.gif`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.6/images/discriminated-union.gif` & `dash_pydantic_form-0.1.7/images/discriminated-union.gif`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.6/images/editable-table.png` & `dash_pydantic_form-0.1.7/images/editable-table.png`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.6/images/form-sections.png` & `dash_pydantic_form-0.1.7/images/form-sections.png`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.6/images/model-list.png` & `dash_pydantic_form-0.1.7/images/model-list.png`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.6/images/nested-model.png` & `dash_pydantic_form-0.1.7/images/nested-model.png`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.6/images/simple-form.png` & `dash_pydantic_form-0.1.7/images/simple-form.png`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.6/pyproject.toml` & `dash_pydantic_form-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.6/usage.py` & `dash_pydantic_form-0.1.7/usage.py`

 * *Files identical despite different names*

