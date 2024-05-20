# Comparing `tmp/djelm-0.8.0.tar.gz` & `tmp/djelm-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djelm-0.8.0.tar", max compression
+gzip compressed data, was "djelm-0.9.0.tar", max compression
```

## Comparing `djelm-0.8.0.tar` & `djelm-0.9.0.tar`

### file list

```diff
@@ -1,67 +1,65 @@
--rw-r--r--   0        0        0     1082 2024-04-08 08:39:45.980995 djelm-0.8.0/LICENSE.txt
--rw-r--r--   0        0        0    23839 2024-04-08 08:39:45.980995 djelm-0.8.0/README_pypi.md
--rw-r--r--   0        0        0     1360 2024-04-08 08:39:45.984995 djelm-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      254 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/__init__.py
--rw-r--r--   0        0        0       83 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/apps.py
--rw-r--r--   0        0        0     2234 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/codegen/annotation.py
--rw-r--r--   0        0        0     2332 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/codegen/compiler.py
--rw-r--r--   0        0        0     2128 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/codegen/elm.py
--rw-r--r--   0        0        0     5288 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/codegen/expression.py
--rw-r--r--   0        0        0      202 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/codegen/format.py
--rw-r--r--   0        0        0       98 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/codegen/module_name.py
--rw-r--r--   0        0        0     1325 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/codegen/op.py
--rw-r--r--   0        0        0      101 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/codegen/range.py
--rw-r--r--   0        0        0       88 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/codegen/utils.py
--rw-r--r--   0        0        0    11043 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/codegen/writer.py
--rw-r--r--   0        0        0     1291 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/cookiecutter.py
--rw-r--r--   0        0        0      345 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/effect.py
--rw-r--r--   0        0        0     1659 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/elm.py
--rw-r--r--   0        0        0     1739 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/flags/README.md
--rw-r--r--   0        0        0      199 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/flags/__init__.py
--rw-r--r--   0        0        0      514 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/flags/adapters.py
--rw-r--r--   0        0        0       65 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/flags/form/__init__.py
--rw-r--r--   0        0        0      813 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/flags/form/adapters.py
--rw-r--r--   0        0        0     2045 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/flags/form/helpers.py
--rw-r--r--   0        0        0      444 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/flags/form/primitives.py
--rw-r--r--   0        0        0      592 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/flags/form/serializer.py
--rw-r--r--   0        0        0    38411 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/flags/main.py
--rw-r--r--   0        0        0     1828 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/flags/primitives.py
--rw-r--r--   0        0        0       36 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/forms/widgets/main.py
--rw-r--r--   0        0        0    13914 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/generators.py
--rw-r--r--   0        0        0        0 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/management/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/management/commands/__init__.py
--rw-r--r--   0        0        0     3376 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/management/commands/djelm.py
--rw-r--r--   0        0        0      105 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/model_template/cookiecutter.json
--rw-r--r--   0        0        0      385 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/model_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.program_name}}.elmf
--rw-r--r--   0        0        0     1384 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/npm.py
--rw-r--r--   0        0        0      112 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/program_template/cookiecutter.json
--rw-r--r--   0        0        0     1464 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.program_name}}.elm
--rw-r--r--   0        0        0      791 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.program_name}}.ts
--rw-r--r--   0        0        0       99 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.tag_file}}.html
--rw-r--r--   0        0        0      375 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.tag_file}}.pyf
--rw-r--r--   0        0        0      603 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.tag_file}}_tags.py
--rw-r--r--   0        0        0       75 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/project_template/cookiecutter.json
--rw-r--r--   0        0        0      430 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/project_template/hooks/post_gen_project.py
--rw-r--r--   0        0        0      167 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/project_template/{{cookiecutter.app_name}}/apps.py
--rw-r--r--   0        0        0        0 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/project_template/{{cookiecutter.app_name}}/flags/.gitkeep
--rw-r--r--   0        0        0        0 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/project_template/{{cookiecutter.app_name}}/static/dist/.gitkeep
--rw-r--r--   0        0        0      446 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/project_template/{{cookiecutter.app_name}}/static_src/.gitignore
--rw-r--r--   0        0        0        0 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/project_template/{{cookiecutter.app_name}}/static_src/djelm_src/.gitkeep
--rw-r--r--   0        0        0      475 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/project_template/{{cookiecutter.app_name}}/static_src/elm.json
--rw-r--r--   0        0        0      384 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/project_template/{{cookiecutter.app_name}}/static_src/package.json
--rw-r--r--   0        0        0        0 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/project_template/{{cookiecutter.app_name}}/static_src/src/Models/.gitkeep
--rw-r--r--   0        0        0       92 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/project_template/{{cookiecutter.app_name}}/templates/include.html
--rw-r--r--   0        0        0        0 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/project_template/{{cookiecutter.app_name}}/templates/{{cookiecutter.app_name}}/.gitkeep
--rw-r--r--   0        0        0        0 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/project_template/{{cookiecutter.app_name}}/templatetags/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/project_template/{{cookiecutter.app_name}}/{{cookiecutter.app_name}}.djelm
--rw-r--r--   0        0        0    21257 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/strategy.py
--rw-r--r--   0        0        0     1010 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/subprocess.py
--rw-r--r--   0        0        0     3348 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/utils.py
--rw-r--r--   0        0        0    20835 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/validate.py
--rw-r--r--   0        0        0      112 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/widget_templates/cookiecutter.json
--rw-r--r--   0        0        0     3912 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/ModelChoiceField.elmw
--rw-r--r--   0        0        0      813 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/Widgets.{{cookiecutter.program_name}}.ts
--rw-r--r--   0        0        0      429 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/modelChoiceField.pyf
--rw-r--r--   0        0        0      753 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/modelChoiceField_tags.py
--rw-r--r--   0        0        0      105 2024-04-08 08:39:45.984995 djelm-0.8.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/{{cookiecutter.tag_file}}.html
--rw-r--r--   0        0        0    24682 1970-01-01 00:00:00.000000 djelm-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-04-10 10:38:35.807679 djelm-0.9.0/LICENSE.txt
+-rw-r--r--   0        0        0    23621 2024-04-10 10:38:35.807679 djelm-0.9.0/README_pypi.md
+-rw-r--r--   0        0        0     1360 2024-04-10 10:38:35.811679 djelm-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      254 2024-04-10 10:38:35.811679 djelm-0.9.0/src/djelm/__init__.py
+-rw-r--r--   0        0        0       83 2024-04-10 10:38:35.811679 djelm-0.9.0/src/djelm/apps.py
+-rw-r--r--   0        0        0     2234 2024-04-10 10:38:35.811679 djelm-0.9.0/src/djelm/codegen/annotation.py
+-rw-r--r--   0        0        0     2332 2024-04-10 10:38:35.811679 djelm-0.9.0/src/djelm/codegen/compiler.py
+-rw-r--r--   0        0        0     2128 2024-04-10 10:38:35.811679 djelm-0.9.0/src/djelm/codegen/elm.py
+-rw-r--r--   0        0        0     5288 2024-04-10 10:38:35.811679 djelm-0.9.0/src/djelm/codegen/expression.py
+-rw-r--r--   0        0        0      202 2024-04-10 10:38:35.811679 djelm-0.9.0/src/djelm/codegen/format.py
+-rw-r--r--   0        0        0       98 2024-04-10 10:38:35.811679 djelm-0.9.0/src/djelm/codegen/module_name.py
+-rw-r--r--   0        0        0     1325 2024-04-10 10:38:35.811679 djelm-0.9.0/src/djelm/codegen/op.py
+-rw-r--r--   0        0        0      101 2024-04-10 10:38:35.811679 djelm-0.9.0/src/djelm/codegen/range.py
+-rw-r--r--   0        0        0       88 2024-04-10 10:38:35.811679 djelm-0.9.0/src/djelm/codegen/utils.py
+-rw-r--r--   0        0        0    11043 2024-04-10 10:38:35.811679 djelm-0.9.0/src/djelm/codegen/writer.py
+-rw-r--r--   0        0        0     1291 2024-04-10 10:38:35.811679 djelm-0.9.0/src/djelm/cookiecutter.py
+-rw-r--r--   0        0        0      345 2024-04-10 10:38:35.811679 djelm-0.9.0/src/djelm/effect.py
+-rw-r--r--   0        0        0     1659 2024-04-10 10:38:35.811679 djelm-0.9.0/src/djelm/elm.py
+-rw-r--r--   0        0        0     1739 2024-04-10 10:38:35.811679 djelm-0.9.0/src/djelm/flags/README.md
+-rw-r--r--   0        0        0      199 2024-04-10 10:38:35.811679 djelm-0.9.0/src/djelm/flags/__init__.py
+-rw-r--r--   0        0        0      514 2024-04-10 10:38:35.811679 djelm-0.9.0/src/djelm/flags/adapters.py
+-rw-r--r--   0        0        0       65 2024-04-10 10:38:35.811679 djelm-0.9.0/src/djelm/flags/form/__init__.py
+-rw-r--r--   0        0        0      813 2024-04-10 10:38:35.811679 djelm-0.9.0/src/djelm/flags/form/adapters.py
+-rw-r--r--   0        0        0     2045 2024-04-10 10:38:35.811679 djelm-0.9.0/src/djelm/flags/form/helpers.py
+-rw-r--r--   0        0        0      444 2024-04-10 10:38:35.811679 djelm-0.9.0/src/djelm/flags/form/primitives.py
+-rw-r--r--   0        0        0      592 2024-04-10 10:38:35.811679 djelm-0.9.0/src/djelm/flags/form/serializer.py
+-rw-r--r--   0        0        0    38411 2024-04-10 10:38:35.811679 djelm-0.9.0/src/djelm/flags/main.py
+-rw-r--r--   0        0        0     1828 2024-04-10 10:38:35.815678 djelm-0.9.0/src/djelm/flags/primitives.py
+-rw-r--r--   0        0        0       36 2024-04-10 10:38:35.815678 djelm-0.9.0/src/djelm/forms/widgets/main.py
+-rw-r--r--   0        0        0    13708 2024-04-10 10:38:35.815678 djelm-0.9.0/src/djelm/generators.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:38:35.815678 djelm-0.9.0/src/djelm/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:38:35.815678 djelm-0.9.0/src/djelm/management/commands/__init__.py
+-rw-r--r--   0        0        0     3376 2024-04-10 10:38:35.815678 djelm-0.9.0/src/djelm/management/commands/djelm.py
+-rw-r--r--   0        0        0      105 2024-04-10 10:38:35.815678 djelm-0.9.0/src/djelm/model_template/cookiecutter.json
+-rw-r--r--   0        0        0      385 2024-04-10 10:38:35.815678 djelm-0.9.0/src/djelm/model_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.program_name}}.elmf
+-rw-r--r--   0        0        0     1384 2024-04-10 10:38:35.815678 djelm-0.9.0/src/djelm/npm.py
+-rw-r--r--   0        0        0      129 2024-04-10 10:38:35.815678 djelm-0.9.0/src/djelm/program_template/cookiecutter.json
+-rw-r--r--   0        0        0     1464 2024-04-10 10:38:35.815678 djelm-0.9.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.program_name}}.elm
+-rw-r--r--   0        0        0      791 2024-04-10 10:38:35.815678 djelm-0.9.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.program_name}}.ts
+-rw-r--r--   0        0        0      459 2024-04-10 10:38:35.815678 djelm-0.9.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.tag_file}}.pyf
+-rw-r--r--   0        0        0      584 2024-04-10 10:38:35.815678 djelm-0.9.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.tag_file}}_tags.py
+-rw-r--r--   0        0        0       75 2024-04-10 10:38:35.815678 djelm-0.9.0/src/djelm/project_template/cookiecutter.json
+-rw-r--r--   0        0        0      430 2024-04-10 10:38:35.815678 djelm-0.9.0/src/djelm/project_template/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      167 2024-04-10 10:38:35.815678 djelm-0.9.0/src/djelm/project_template/{{cookiecutter.app_name}}/apps.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:38:35.815678 djelm-0.9.0/src/djelm/project_template/{{cookiecutter.app_name}}/flags/.gitkeep
+-rw-r--r--   0        0        0        0 2024-04-10 10:38:35.815678 djelm-0.9.0/src/djelm/project_template/{{cookiecutter.app_name}}/static/dist/.gitkeep
+-rw-r--r--   0        0        0      446 2024-04-10 10:38:35.815678 djelm-0.9.0/src/djelm/project_template/{{cookiecutter.app_name}}/static_src/.gitignore
+-rw-r--r--   0        0        0        0 2024-04-10 10:38:35.815678 djelm-0.9.0/src/djelm/project_template/{{cookiecutter.app_name}}/static_src/djelm_src/.gitkeep
+-rw-r--r--   0        0        0      475 2024-04-10 10:38:35.815678 djelm-0.9.0/src/djelm/project_template/{{cookiecutter.app_name}}/static_src/elm.json
+-rw-r--r--   0        0        0      384 2024-04-10 10:38:35.815678 djelm-0.9.0/src/djelm/project_template/{{cookiecutter.app_name}}/static_src/package.json
+-rw-r--r--   0        0        0        0 2024-04-10 10:38:35.815678 djelm-0.9.0/src/djelm/project_template/{{cookiecutter.app_name}}/static_src/src/Models/.gitkeep
+-rw-r--r--   0        0        0        0 2024-04-10 10:38:35.815678 djelm-0.9.0/src/djelm/project_template/{{cookiecutter.app_name}}/templatetags/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:38:35.815678 djelm-0.9.0/src/djelm/project_template/{{cookiecutter.app_name}}/{{cookiecutter.app_name}}.djelm
+-rw-r--r--   0        0        0    21088 2024-04-10 10:38:35.815678 djelm-0.9.0/src/djelm/strategy.py
+-rw-r--r--   0        0        0     1010 2024-04-10 10:38:35.815678 djelm-0.9.0/src/djelm/subprocess.py
+-rw-r--r--   0        0        0       92 2024-04-10 10:38:35.815678 djelm-0.9.0/src/djelm/templates/djelm/include.html
+-rw-r--r--   0        0        0       45 2024-04-10 10:38:35.815678 djelm-0.9.0/src/djelm/templates/djelm/program.html
+-rw-r--r--   0        0        0     3208 2024-04-10 10:38:35.815678 djelm-0.9.0/src/djelm/utils.py
+-rw-r--r--   0        0        0    20835 2024-04-10 10:38:35.815678 djelm-0.9.0/src/djelm/validate.py
+-rw-r--r--   0        0        0      129 2024-04-10 10:38:35.815678 djelm-0.9.0/src/djelm/widget_templates/cookiecutter.json
+-rw-r--r--   0        0        0     3912 2024-04-10 10:38:35.815678 djelm-0.9.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/ModelChoiceField.elmw
+-rw-r--r--   0        0        0      813 2024-04-10 10:38:35.815678 djelm-0.9.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/Widgets.{{cookiecutter.program_name}}.ts
+-rw-r--r--   0        0        0      519 2024-04-10 10:38:35.815678 djelm-0.9.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/modelChoiceField.pyf
+-rw-r--r--   0        0        0      726 2024-04-10 10:38:35.815678 djelm-0.9.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/modelChoiceField_tags.py
+-rw-r--r--   0        0        0    24464 1970-01-01 00:00:00.000000 djelm-0.9.0/PKG-INFO
```

### Comparing `djelm-0.8.0/LICENSE.txt` & `djelm-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djelm-0.8.0/README_pypi.md` & `djelm-0.9.0/README_pypi.md`

 * *Files 4% similar despite different names*

```diff
@@ -204,17 +204,14 @@
 ├── static_src
 │   ├── .gitignore
 │   ├── djelm_src
 │   ├── elm.json
 │   ├── package.json
 │   └── src
 │       └── Models
-├── templates
-│   ├── include.html
-│   └── elm_programs
 └── templatetags
     └── __init__.py
 ```
 
 What you are seeing is the directory structure required for djelm to seamlessly work with both Django and Elm.
 
 Everything outside of the `static_src` directory should look like a typical Django app, and everything inside
@@ -253,18 +250,14 @@
 │   │   └── Main.ts *
 │   ├── elm.json
 │   ├── package.json
 │   └── src
 │       ├── Main.elm *
 │       └── Models
 │           └── Main.elm *
-├── templates
-│   ├── include.html
-│   └── elm_programs
-│       └── main.html *
 └── templatetags
     ├── __init__.py
     └── main_tags.py *
 ```
 
 Jump in to the `static_src/src/Main.elm` file in the `elm_programs` directory and what you will see is a simple Elm
 program. You
@@ -348,18 +341,14 @@
 │   │   └── Main.ts
 │   ├── elm.json
 │   ├── package.json
 │   └── src
 │       ├── Main.elm
 │       └── Models
 │           └── Main.elm
-├── templates
-│   ├── include.html
-│   └── elm_programs
-│       └── main.html
 └── templatetags
     ├── __init__.py
     └── main_tags.py
 
 ```
 
 Djelm compiled our `Main.elm` program and bundled it up for us in a place where Django can work with it, awesome!
@@ -388,17 +377,18 @@
 > don't want sitting on your Django production server taking up space.
 
 ## Template tags
 
 Let's now actually render something in the browser by adding our `Main` programs tags to a Django template.
 
 > [!NOTE]
-> I have added the following `base.html` and `main.html` templates to the `elm_programs/templates` directory for demonstration purposes.
+> I have added the following `base.html` and `main.html` templates to a `elm_programs/templates` directory for demonstration purposes.
+> You will need to create this directory if you havent done so already.
 >
-> if you already have a django project you can just add the tags into whatever templates you want to render the elm program.
+> If you already have a django project you can just add the tags into whatever templates you want to render the elm program.
 
 ```html
 <!-- base.html -->
 
 <!doctype html>
 <html lang="en">
   <head>
@@ -468,17 +458,17 @@
 This value actually comes bound to our render tag when we server render the template, and is passed to the Elm program
 when it is initialized on the client,
 as a flag value.
 
 Check out the `elm_programs/templatetags/main_tags.py` file that was generated for you:
 
 ```python
-@register.inclusion_tag("elm_programs/main.html", takes_context=True)
+@register.inclusion_tag("djelm/program.html", takes_context=True)
 def render_main(context):
-    return {"flags": MainFlags.parse(0)}
+    return {"key": key, "flags": MainFlags.parse(0)}
 ```
 
 Those experienced with Django might be having an 'Aha!' moment right now but don't worry if thats not the case,
 I'll explain everything.
 
 This `0` value is set from the `render_main` tag function as a default, the actual values you will want to pass your Elm
 programs are much more likely to originate in your Django views like the following example:
@@ -496,17 +486,17 @@
 
 The context that was set in the view is available to us from the `render_main` tag function which we can
 call `MainFlags` with:
 
 ```python
 # main_tags.py
 
-@register.inclusion_tag("elm_programs/main.html", takes_context=True)
+@register.inclusion_tag("djelm/program.html", takes_context=True)
 def render_main(context):
-    return {"flags": MainFlags.parse(context["counter_start"])}
+    return {"key": key, "flags": MainFlags.parse(context["counter_start"])}
 ```
 
 Whilst in this example we are hardcoding a value of `0`, you really can pass it any `int` you want, perhaps an ID from a
 database
 model or some other computed value.
 
 The one constraint you have is that it must be an `int`, which is perfect for our default Elm
@@ -517,17 +507,17 @@
 > docs [here](https://docs.djangoproject.com/en/5.0/howto/custom-template-tags/).
 
 Let's try passing something that isn't an `int` and see what happens:
 
 ```python
 # main_tags.py
 
-@register.inclusion_tag("elm_programs/main.html", takes_context=True)
+@register.inclusion_tag("djelm/program.html", takes_context=True)
 def render_main(context):
-    return {"flags": MainFlags.parse("Hello Elm!")}
+    return {"key": key, "flags": MainFlags.parse("Hello Elm!")}
 ```
 
 What you should be seeing is a server error, but why? Let's find out!
 
 ## Flag classes
 
 If we inspect the `MainFlags` function in `elm_programs/flags/main.py` we will see the following:
```

### Comparing `djelm-0.8.0/pyproject.toml` & `djelm-0.9.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.mypy]
 plugins = [ "mypy_django_plugin.main" ]
 
 [tool.poetry]
 name = "djelm"
-version = "0.8.0"
+version = "0.9.0"
 description = "A framework for using Elm programs in a Django project"
 authors = ["Confidenceman02"]
 readme = "README_pypi.md"
 keywords = ["django", "elm"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

### Comparing `djelm-0.8.0/src/djelm/codegen/annotation.py` & `djelm-0.9.0/src/djelm/codegen/annotation.py`

 * *Files identical despite different names*

### Comparing `djelm-0.8.0/src/djelm/codegen/compiler.py` & `djelm-0.9.0/src/djelm/codegen/compiler.py`

 * *Files identical despite different names*

### Comparing `djelm-0.8.0/src/djelm/codegen/elm.py` & `djelm-0.9.0/src/djelm/codegen/elm.py`

 * *Files identical despite different names*

### Comparing `djelm-0.8.0/src/djelm/codegen/expression.py` & `djelm-0.9.0/src/djelm/codegen/expression.py`

 * *Files identical despite different names*

### Comparing `djelm-0.8.0/src/djelm/codegen/op.py` & `djelm-0.9.0/src/djelm/codegen/op.py`

 * *Files identical despite different names*

### Comparing `djelm-0.8.0/src/djelm/codegen/writer.py` & `djelm-0.9.0/src/djelm/codegen/writer.py`

 * *Files identical despite different names*

### Comparing `djelm-0.8.0/src/djelm/cookiecutter.py` & `djelm-0.9.0/src/djelm/cookiecutter.py`

 * *Files identical despite different names*

### Comparing `djelm-0.8.0/src/djelm/elm.py` & `djelm-0.9.0/src/djelm/elm.py`

 * *Files identical despite different names*

### Comparing `djelm-0.8.0/src/djelm/flags/README.md` & `djelm-0.9.0/src/djelm/flags/README.md`

 * *Files identical despite different names*

### Comparing `djelm-0.8.0/src/djelm/flags/adapters.py` & `djelm-0.9.0/src/djelm/flags/adapters.py`

 * *Files identical despite different names*

### Comparing `djelm-0.8.0/src/djelm/flags/form/adapters.py` & `djelm-0.9.0/src/djelm/flags/form/adapters.py`

 * *Files identical despite different names*

### Comparing `djelm-0.8.0/src/djelm/flags/form/helpers.py` & `djelm-0.9.0/src/djelm/flags/form/helpers.py`

 * *Files identical despite different names*

### Comparing `djelm-0.8.0/src/djelm/flags/form/serializer.py` & `djelm-0.9.0/src/djelm/flags/form/serializer.py`

 * *Files identical despite different names*

### Comparing `djelm-0.8.0/src/djelm/flags/main.py` & `djelm-0.9.0/src/djelm/flags/main.py`

 * *Files identical despite different names*

### Comparing `djelm-0.8.0/src/djelm/flags/primitives.py` & `djelm-0.9.0/src/djelm/flags/primitives.py`

 * *Files identical despite different names*

### Comparing `djelm-0.8.0/src/djelm/generators.py` & `djelm-0.9.0/src/djelm/generators.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         Is is either going to be from a djelm app or a pre-built one.
         """
         ...
 
 
 class SupportsProgramCookieCutter(Protocol):
     def cookie_cutter(
-        self, app_name: str, program_name: str, src_path: str
+        self, app_name: str, program_name: str, src_path: str, version: str
     ) -> CookieCutter:
         """Generate a cookie cutter config"""
         ...
 
 
 class SupportsModelCookieCutter(Protocol):
     def cookie_cutter(
@@ -110,14 +110,15 @@
     {
         "tmp_dir": str,
         "program_name": str,
         "tag_file": str,
         "app_name": str,
         "scope": str,
         "view_name": str,
+        "version": str,
     },
 )
 
 ModelCookieExtra = TypedDict(
     "ModelCookieExtra",
     {
         "program_name": str,
@@ -133,32 +134,34 @@
     {
         "program_name": str,
         "view_name": str,
         "tmp_dir": str,
         "tag_file": str,
         "scope": str,
         "app_name": str,
+        "version": str,
     },
 )
 
 
 def widget_cookie_cutter(
-    app_name: str, src_path: str, program_name: str
+    app_name: str, src_path: str, program_name: str, version: str
 ) -> CookieCutter:
     return CookieCutter[WidgetProgramCookieExtra](
         file_dir=os.path.dirname(__file__),
         output_dir=os.path.join(src_path, *STUFF_NAMESPACE),
         cookie_dir_name="widget_templates",
         extra={
             "tmp_dir": "widgets",
             "program_name": program_name,
             "tag_file": tag_file_name(program_name),
             "app_name": app_name,
             "scope": widget_scope_name(app_name, program_name),
             "view_name": view_name(program_name),
+            "version": version,
         },
         overwrite=True,
     )
 
 
 def model_cookie_cutter(
     flags: Flags, program_name: str, tmp_dir: str, output_dir: str, module_path: str
@@ -246,17 +249,17 @@
         effect = NPM(raise_err=True).command(working_dir, args)
 
         if effect.tag != "Success":
             return ExitFailure(None, effect.err)
         return ExitSuccess(None)
 
     def cookie_cutter(
-        self, app_name: str, program_name: str, src_path: str
+        self, app_name: str, program_name: str, src_path: str, version: str
     ) -> CookieCutter:
-        return widget_cookie_cutter(app_name, src_path, program_name)
+        return widget_cookie_cutter(app_name, src_path, program_name, version)
 
     def applicators(
         self,
         template_dir: str,
         src_dir: str,
         app_dir: str,
         program_name: str,
@@ -287,18 +290,14 @@
                 os.path.join(
                     app_dir,
                     "templatetags",
                     f"{tag_file_name(program_name)}_widget_tags.py",
                 ),
             ),
             TemplateCopyer(
-                os.path.join(template_dir, f"{tag_file_name(program_name)}.html"),
-                os.path.join(app_dir, "templates", app_name, "widgets"),
-            ),
-            TemplateCopyer(
                 os.path.join(template_dir, f"Widgets.{module_name(program_name)}.ts"),
                 os.path.join(
                     src_dir,
                     "djelm_src",
                 ),
             ),
         ]
@@ -307,27 +306,28 @@
 class ProgramGenerator(ProgramBuilder):
     def install_elm_deps(
         self, working_dir: str, logger
     ) -> ExitSuccess[None] | ExitFailure[None, NPMError]:
         return ExitSuccess(None)
 
     def cookie_cutter(
-        self, app_name: str, program_name: str, src_path: str
+        self, app_name: str, program_name: str, src_path: str, version: str
     ) -> CookieCutter:
         return CookieCutter[ProgramCookieExtra](
             file_dir=os.path.dirname(__file__),
             output_dir=os.path.join(src_path, "elm-stuff"),
             cookie_dir_name="program_template",
             extra={
                 "program_name": module_name(program_name),
                 "view_name": view_name(program_name),
                 "tmp_dir": STUFF_NAMESPACE[1],
                 "tag_file": tag_file_name(program_name),
                 "scope": scope_name(app_name, program_name),
                 "app_name": app_name,
+                "version": version,
             },
             overwrite=True,
         )
 
     def applicators(
         self,
         template_dir: str,
@@ -350,18 +350,14 @@
                 os.path.join(app_dir, "templatetags"),
             ),
             TemplateCopyer(
                 os.path.join(template_dir, tag_file_name(program_name) + ".pyf"),
                 os.path.join(app_dir, "flags", tag_file_name(program_name) + ".py"),
             ),
             TemplateCopyer(
-                os.path.join(template_dir, tag_file_name(program_name) + ".html"),
-                os.path.join(app_dir, "templates", app_name),
-            ),
-            TemplateCopyer(
                 os.path.join(template_dir, module_name(program_name) + ".ts"),
                 os.path.join(src_dir, "djelm_src"),
             ),
         ]
 
 
 class ModelGenerator(ModelBuilder):
```

### Comparing `djelm-0.8.0/src/djelm/management/commands/djelm.py` & `djelm-0.9.0/src/djelm/management/commands/djelm.py`

 * *Files identical despite different names*

### Comparing `djelm-0.8.0/src/djelm/npm.py` & `djelm-0.9.0/src/djelm/npm.py`

 * *Files identical despite different names*

### Comparing `djelm-0.8.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.program_name}}.elm` & `djelm-0.9.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.program_name}}.elm`

 * *Files identical despite different names*

### Comparing `djelm-0.8.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.program_name}}.ts` & `djelm-0.9.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.program_name}}.ts`

 * *Files identical despite different names*

### Comparing `djelm-0.8.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.tag_file}}_tags.py` & `djelm-0.9.0/src/djelm/program_template/{{cookiecutter.tmp_dir}}/{{cookiecutter.tag_file}}_tags.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from django import template
-from ..flags.{{cookiecutter.tag_file}} import {{cookiecutter.program_name}}Flags
+from ..flags.{{cookiecutter.tag_file}} import key, {{cookiecutter.program_name}}Flags
 
 register = template.Library()
 
 
-@register.inclusion_tag("{{ cookiecutter.app_name }}/{{ cookiecutter.tag_file }}.html", takes_context=True)
+@register.inclusion_tag("djelm/program.html", takes_context=True)
 def render_{{ cookiecutter.tag_file }}(context):
-    return {"flags": {{cookiecutter.program_name}}Flags.parse(0)}
+    return {"key": key, "flags": {{cookiecutter.program_name}}Flags.parse(0)}
 
 
-@register.inclusion_tag("include.html")
+@register.inclusion_tag("djelm/include.html")
 def include_{{ cookiecutter.tag_file }}():
     # Generates the script tag for the {{cookiecutter.program_name}}.elm program
     return {"djelm_program": "dist/{{ cookiecutter.program_name }}.js"}
```

### Comparing `djelm-0.8.0/src/djelm/strategy.py` & `djelm-0.9.0/src/djelm/strategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,15 @@
     widget_name: str
     handler: ProgramBuilder
     no_deps: bool
 
     def run(self, logger) -> ExitSuccess[None] | ExitFailure[None, StrategyError]:
         src_path = get_app_src_path(self.app_name)
         app_path = get_app_path(self.app_name)
+        djelm_version = version("djelm")
 
         if src_path.tag != "Success":
             raise src_path.err
 
         if app_path.tag != "Success":
             raise app_path.err
 
@@ -98,30 +99,22 @@
 
         # Make flags dirs
         try:
             os.makedirs(os.path.join(app_path.value, "flags", "widgets"))
         except FileExistsError:
             pass
 
-        # Make templates.{self.app_name}.widgets dirs
-        try:
-            os.makedirs(
-                os.path.join(app_path.value, "templates", self.app_name, "widgets")
-            )
-        except FileExistsError:
-            pass
-
         # Make Widgets dirs
         try:
             os.makedirs(os.path.join(src_path.value, "src", "Widgets", "Models"))
         except FileExistsError:
             pass
 
         cookie = self.handler.cookie_cutter(
-            self.app_name, self.widget_name, src_path.value
+            self.app_name, self.widget_name, src_path.value, djelm_version
         )
 
         # Cut cookie
         ck_result = cookie.cut(logger)
 
         if ck_result.tag != "Success":
             raise ck_result.err
@@ -455,15 +448,15 @@
             os.makedirs(os.path.join(src_path.value, *stuff_namespace))
         except FileExistsError:
             pass
         except FileNotFoundError as err:
             raise err
 
         program_ck = self.handler.cookie_cutter(
-            self.app_name, self.prog_name, src_path.value
+            self.app_name, self.prog_name, src_path.value, djelm_version
         )
 
         program_ck_effect = program_ck.cut(logger)
 
         if program_ck_effect.tag != "Success":
             raise program_ck_effect.err
```

### Comparing `djelm-0.8.0/src/djelm/subprocess.py` & `djelm-0.9.0/src/djelm/subprocess.py`

 * *Files identical despite different names*

### Comparing `djelm-0.8.0/src/djelm/utils.py` & `djelm-0.9.0/src/djelm/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,21 +57,16 @@
     if path_exit.tag == "Success":
         tags = os.path.isdir(
             os.path.join(
                 path_exit.value,
                 "templatetags",
             )
         )
-        templates = os.path.isdir(
-            os.path.join(
-                path_exit.value,
-                "templates",
-            )
-        )
-        return templates and tags
+        if tags:
+            return True
     return False
 
 
 def is_init(app_name: str) -> bool:
     path_exit = get_app_path(app_name)
     if path_exit.tag == "Success":
         f = os.path.isfile(
```

### Comparing `djelm-0.8.0/src/djelm/validate.py` & `djelm-0.9.0/src/djelm/validate.py`

 * *Files identical despite different names*

### Comparing `djelm-0.8.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/ModelChoiceField.elmw` & `djelm-0.9.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/ModelChoiceField.elmw`

 * *Files identical despite different names*

### Comparing `djelm-0.8.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/Widgets.{{cookiecutter.program_name}}.ts` & `djelm-0.9.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/Widgets.{{cookiecutter.program_name}}.ts`

 * *Files identical despite different names*

### Comparing `djelm-0.8.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/modelChoiceField_tags.py` & `djelm-0.9.0/src/djelm/widget_templates/{{cookiecutter.tmp_dir}}/modelChoiceField_tags.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from django import template
-from ..flags.widgets.{{cookiecutter.tag_file}} import {{cookiecutter.program_name}}Flags
+from ..flags.widgets.{{cookiecutter.tag_file}} import key, {{cookiecutter.program_name}}Flags
 
 register = template.Library()
 
 
-@register.inclusion_tag("{{ cookiecutter.app_name }}/widgets/{{ cookiecutter.tag_file }}.html", takes_context=True, name="render_{{cookiecutter.program_name}}Widget")
+@register.inclusion_tag("djelm/program.html", takes_context=True, name="render_{{cookiecutter.program_name}}Widget")
 def render_{{ cookiecutter.tag_file }}(context):
-    return {"flags": {{cookiecutter.program_name}}Flags.parse(context["field"])}
+    return {"key": key, "flags": {{cookiecutter.program_name}}Flags.parse(context["field"])}
 
 
-@register.inclusion_tag("include.html", name="include_{{cookiecutter.program_name}}Widget")
+@register.inclusion_tag("djelm/include.html", name="include_{{cookiecutter.program_name}}Widget")
 def include_{{ cookiecutter.tag_file }}():
     # Generates the script tag for the Widgets/{{cookiecutter.program_name}}.elm program
     return {"djelm_program": "dist/Widgets.{{ cookiecutter.program_name }}.js"}
```

### Comparing `djelm-0.8.0/PKG-INFO` & `djelm-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djelm
-Version: 0.8.0
+Version: 0.9.0
 Summary: A framework for using Elm programs in a Django project
 Keywords: django,elm
 Author: Confidenceman02
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -227,17 +227,14 @@
 ├── static_src
 │   ├── .gitignore
 │   ├── djelm_src
 │   ├── elm.json
 │   ├── package.json
 │   └── src
 │       └── Models
-├── templates
-│   ├── include.html
-│   └── elm_programs
 └── templatetags
     └── __init__.py
 ```
 
 What you are seeing is the directory structure required for djelm to seamlessly work with both Django and Elm.
 
 Everything outside of the `static_src` directory should look like a typical Django app, and everything inside
@@ -276,18 +273,14 @@
 │   │   └── Main.ts *
 │   ├── elm.json
 │   ├── package.json
 │   └── src
 │       ├── Main.elm *
 │       └── Models
 │           └── Main.elm *
-├── templates
-│   ├── include.html
-│   └── elm_programs
-│       └── main.html *
 └── templatetags
     ├── __init__.py
     └── main_tags.py *
 ```
 
 Jump in to the `static_src/src/Main.elm` file in the `elm_programs` directory and what you will see is a simple Elm
 program. You
@@ -371,18 +364,14 @@
 │   │   └── Main.ts
 │   ├── elm.json
 │   ├── package.json
 │   └── src
 │       ├── Main.elm
 │       └── Models
 │           └── Main.elm
-├── templates
-│   ├── include.html
-│   └── elm_programs
-│       └── main.html
 └── templatetags
     ├── __init__.py
     └── main_tags.py
 
 ```
 
 Djelm compiled our `Main.elm` program and bundled it up for us in a place where Django can work with it, awesome!
@@ -411,17 +400,18 @@
 > don't want sitting on your Django production server taking up space.
 
 ## Template tags
 
 Let's now actually render something in the browser by adding our `Main` programs tags to a Django template.
 
 > [!NOTE]
-> I have added the following `base.html` and `main.html` templates to the `elm_programs/templates` directory for demonstration purposes.
+> I have added the following `base.html` and `main.html` templates to a `elm_programs/templates` directory for demonstration purposes.
+> You will need to create this directory if you havent done so already.
 >
-> if you already have a django project you can just add the tags into whatever templates you want to render the elm program.
+> If you already have a django project you can just add the tags into whatever templates you want to render the elm program.
 
 ```html
 <!-- base.html -->
 
 <!doctype html>
 <html lang="en">
   <head>
@@ -491,17 +481,17 @@
 This value actually comes bound to our render tag when we server render the template, and is passed to the Elm program
 when it is initialized on the client,
 as a flag value.
 
 Check out the `elm_programs/templatetags/main_tags.py` file that was generated for you:
 
 ```python
-@register.inclusion_tag("elm_programs/main.html", takes_context=True)
+@register.inclusion_tag("djelm/program.html", takes_context=True)
 def render_main(context):
-    return {"flags": MainFlags.parse(0)}
+    return {"key": key, "flags": MainFlags.parse(0)}
 ```
 
 Those experienced with Django might be having an 'Aha!' moment right now but don't worry if thats not the case,
 I'll explain everything.
 
 This `0` value is set from the `render_main` tag function as a default, the actual values you will want to pass your Elm
 programs are much more likely to originate in your Django views like the following example:
@@ -519,17 +509,17 @@
 
 The context that was set in the view is available to us from the `render_main` tag function which we can
 call `MainFlags` with:
 
 ```python
 # main_tags.py
 
-@register.inclusion_tag("elm_programs/main.html", takes_context=True)
+@register.inclusion_tag("djelm/program.html", takes_context=True)
 def render_main(context):
-    return {"flags": MainFlags.parse(context["counter_start"])}
+    return {"key": key, "flags": MainFlags.parse(context["counter_start"])}
 ```
 
 Whilst in this example we are hardcoding a value of `0`, you really can pass it any `int` you want, perhaps an ID from a
 database
 model or some other computed value.
 
 The one constraint you have is that it must be an `int`, which is perfect for our default Elm
@@ -540,17 +530,17 @@
 > docs [here](https://docs.djangoproject.com/en/5.0/howto/custom-template-tags/).
 
 Let's try passing something that isn't an `int` and see what happens:
 
 ```python
 # main_tags.py
 
-@register.inclusion_tag("elm_programs/main.html", takes_context=True)
+@register.inclusion_tag("djelm/program.html", takes_context=True)
 def render_main(context):
-    return {"flags": MainFlags.parse("Hello Elm!")}
+    return {"key": key, "flags": MainFlags.parse("Hello Elm!")}
 ```
 
 What you should be seeing is a server error, but why? Let's find out!
 
 ## Flag classes
 
 If we inspect the `MainFlags` function in `elm_programs/flags/main.py` we will see the following:
```

