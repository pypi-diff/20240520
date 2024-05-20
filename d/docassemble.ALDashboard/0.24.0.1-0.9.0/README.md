# Comparing `tmp/docassemble_aldashboard-0.24.0.1.tar.gz` & `tmp/docassemble.ALDashboard-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docassemble_aldashboard-0.24.0.1.tar", last modified: Mon May 20 15:09:13 2024, max compression
+gzip compressed data, was "dist/docassemble.ALDashboard-0.9.0.tar", last modified: Tue Oct 26 18:13:40 2021, max compression
```

## Comparing `docassemble_aldashboard-0.24.0.1.tar` & `docassemble.ALDashboard-0.9.0.tar`

### file list

```diff
@@ -1,64 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:09:13.685213 docassemble_aldashboard-0.24.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-05-20 15:09:13.685213 docassemble_aldashboard-0.24.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:09:13.681213 docassemble_aldashboard-0.24.0.1/docassemble/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:09:13.681213 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15060 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/aldashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    12036 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/create_package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:09:13.677213 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:09:13.685213 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/data/questions/
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/data/questions/api_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/data/questions/browse_interviews.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/data/questions/compile_bootstrap.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/data/questions/docx_wrangling.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/data/questions/generate_translation.yml
--rw-r--r--   0 runner    (1001) docker     (127)    24386 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/data/questions/install_assembly_line.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/data/questions/install_fonts.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/data/questions/install_packages.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5151 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/data/questions/list_sessions.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/data/questions/manage_answer_viewers.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/data/questions/manage_users.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/data/questions/menu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/data/questions/nav.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7514 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/data/questions/package_scanner.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/data/questions/pdf_wrangling.yml
--rw-r--r--   0 runner    (1001) docker     (127)    10064 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/data/questions/review_screen_generator.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/data/questions/update_packages.yml
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/data/questions/validate_attachment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/data/questions/validate_docx.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/data/questions/validate_translation.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:09:13.685213 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/data/sources/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/data/sources/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:09:13.685213 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/data/static/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/data/static/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/data/static/al_dashboard.css
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/data/static/bootstrap.svg
--rw-r--r--   0 runner    (1001) docker     (127)    78321 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/data/static/test_html.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:09:13.685213 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/data/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/data/templates/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7493 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/data/templates/pkg_scanner_report.docx
--rw-r--r--   0 runner    (1001) docker     (127)    10640 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/docx_wrangling.py
--rw-r--r--   0 runner    (1001) docker     (127)     8255 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/package_scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:09:13.685213 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/test/
--rw-r--r--   0 runner    (1001) docker     (127)    12223 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/test/made_up_variables.docx
--rw-r--r--   0 runner    (1001) docker     (127)    11900 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/test/valid_word_invalid_jinja.docx
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/test_validate_docx.py
--rw-r--r--   0 runner    (1001) docker     (127)    24597 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/translation.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/validate_attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/validate_docx.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/docassemble/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:09:13.685213 docassemble_aldashboard-0.24.0.1/docassemble.ALDashboard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-05-20 15:09:13.000000 docassemble_aldashboard-0.24.0.1/docassemble.ALDashboard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-20 15:09:13.000000 docassemble_aldashboard-0.24.0.1/docassemble.ALDashboard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 15:09:13.000000 docassemble_aldashboard-0.24.0.1/docassemble.ALDashboard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-20 15:09:13.000000 docassemble_aldashboard-0.24.0.1/docassemble.ALDashboard.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 15:09:13.000000 docassemble_aldashboard-0.24.0.1/docassemble.ALDashboard.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-20 15:09:13.000000 docassemble_aldashboard-0.24.0.1/docassemble.ALDashboard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-20 15:09:13.000000 docassemble_aldashboard-0.24.0.1/docassemble.ALDashboard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-20 15:09:13.685213 docassemble_aldashboard-0.24.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-05-20 15:09:10.000000 docassemble_aldashboard-0.24.0.1/setup.py
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2021-10-26 18:13:40.849167 docassemble.ALDashboard-0.9.0/
+-rw-r--r--   0 www-data    (33) www-data    (33)       18 2021-10-26 18:13:40.000000 docassemble.ALDashboard-0.9.0/MANIFEST.in
+-rw-r--r--   0 www-data    (33) www-data    (33)     2933 2021-10-26 18:13:40.849167 docassemble.ALDashboard-0.9.0/PKG-INFO
+-rw-r--r--   0 www-data    (33) www-data    (33)     2195 2021-10-26 18:13:40.000000 docassemble.ALDashboard-0.9.0/README.md
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2021-10-26 18:13:40.845167 docassemble.ALDashboard-0.9.0/docassemble/
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2021-10-26 18:13:40.849167 docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/
+-rw-r--r--   0 www-data    (33) www-data    (33)       22 2021-10-26 18:13:40.000000 docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/__init__.py
+-rw-r--r--   0 www-data    (33) www-data    (33)     4889 2021-10-26 16:03:52.000000 docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/aldashboard.py
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2021-10-26 18:13:40.845167 docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/data/
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2021-10-26 18:13:40.849167 docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/data/questions/
+-rw-r--r--   0 www-data    (33) www-data    (33)     2791 2021-10-26 15:39:12.000000 docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/data/questions/install_assembly_line.yml
+-rw-r--r--   0 www-data    (33) www-data    (33)     2685 2021-10-26 15:01:33.000000 docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/data/questions/install_packages.yml
+-rw-r--r--   0 www-data    (33) www-data    (33)     1563 2021-07-31 17:09:32.000000 docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/data/questions/list_sessions.yml
+-rw-r--r--   0 www-data    (33) www-data    (33)     2542 2021-10-18 16:49:09.000000 docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/data/questions/manage_users.yml
+-rw-r--r--   0 www-data    (33) www-data    (33)     1120 2021-10-26 15:37:24.000000 docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/data/questions/menu.yml
+-rw-r--r--   0 www-data    (33) www-data    (33)      143 2021-07-31 17:13:17.000000 docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/data/questions/nav.yml
+-rw-r--r--   0 www-data    (33) www-data    (33)     2087 2021-10-26 15:01:33.000000 docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/data/questions/update_packages.yml
+-rw-r--r--   0 www-data    (33) www-data    (33)     4402 2021-07-31 17:11:53.000000 docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/data/questions/validate_translation.yml
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2021-10-26 18:13:40.849167 docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/data/sources/
+-rw-r--r--   0 www-data    (33) www-data    (33)      134 2021-10-26 18:13:40.000000 docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/data/sources/README.md
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2021-10-26 18:13:40.849167 docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/data/static/
+-rw-r--r--   0 www-data    (33) www-data    (33)      105 2021-10-26 18:13:40.000000 docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/data/static/README.md
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2021-10-26 18:13:40.849167 docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/data/templates/
+-rw-r--r--   0 www-data    (33) www-data    (33)      102 2021-10-26 18:13:40.000000 docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/data/templates/README.md
+-rw-r--r--   0 www-data    (33) www-data    (33)      155 2021-10-26 18:13:40.000000 docassemble.ALDashboard-0.9.0/docassemble/__init__.py
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2021-10-26 18:13:40.849167 docassemble.ALDashboard-0.9.0/docassemble.ALDashboard.egg-info/
+-rw-r--r--   0 www-data    (33) www-data    (33)     2933 2021-10-26 18:13:40.000000 docassemble.ALDashboard-0.9.0/docassemble.ALDashboard.egg-info/PKG-INFO
+-rw-r--r--   0 www-data    (33) www-data    (33)     1027 2021-10-26 18:13:40.000000 docassemble.ALDashboard-0.9.0/docassemble.ALDashboard.egg-info/SOURCES.txt
+-rw-r--r--   0 www-data    (33) www-data    (33)        1 2021-10-26 18:13:40.000000 docassemble.ALDashboard-0.9.0/docassemble.ALDashboard.egg-info/dependency_links.txt
+-rw-r--r--   0 www-data    (33) www-data    (33)       12 2021-10-26 18:13:40.000000 docassemble.ALDashboard-0.9.0/docassemble.ALDashboard.egg-info/namespace_packages.txt
+-rw-r--r--   0 www-data    (33) www-data    (33)        1 2021-10-26 18:13:40.000000 docassemble.ALDashboard-0.9.0/docassemble.ALDashboard.egg-info/not-zip-safe
+-rw-r--r--   0 www-data    (33) www-data    (33)       12 2021-10-26 18:13:40.000000 docassemble.ALDashboard-0.9.0/docassemble.ALDashboard.egg-info/top_level.txt
+-rw-r--r--   0 www-data    (33) www-data    (33)       79 2021-10-26 18:13:40.849167 docassemble.ALDashboard-0.9.0/setup.cfg
+-rw-r--r--   0 www-data    (33) www-data    (33)     4667 2021-10-26 18:13:40.000000 docassemble.ALDashboard-0.9.0/setup.py
```

### Comparing `docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/data/questions/install_packages.yml` & `docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/data/questions/update_packages.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,105 +1,80 @@
+---
+include:
+  - nav.yml
+---
 metadata:
-  title: Bulk Package Install
+  title: Bulk Package Update
   sessions are unique: True
   required privileges:
     - admin
     - developer
   temporary session: True
 ---
-modules:
-  - .aldashboard
----
 objects:
-  - packages: DAList.using(object_type=DAObject, there_are_any=True, complete_attribute="github_url")
+  - daREST: DAWeb.using(base_url=get_config('url root',"https://" + get_config('external hostname',"")) + "/api" )
+  - packages: DAList.using(object_type=DAObject, there_are_any=True, complete_attribute="package_name")
+---
+code: |
+  installed_packages = daREST.get('package',{"key": install_packages_api_key })
+---
+code: |
+  install_packages_api_key = get_config('install packages api key')
 ---
 mandatory: True
 id: interview order
 code: |
+  if not install_packages_api_key:
+    exit_no_api_key
   packages.gather()
   if install_packages_task.ready():
     ending_screen
   else:
     waiting_screen
 ---
+event: exit_no_api_key
+question: |
+  Please add an API key!
+subquestion: |
+  This interview requires an API key to work.
+  
+  You can create an API key by going to your profile. Please
+  create an API key with either IP restrictions or no restrictions.
+  
+  Then add it to the [configuration file](${ url_of('config') }) like this:
+  
+  ```
+  install packages api key: x7123aG...
+  ```
+---
 question: |
-  What packages do you want to install?
-list collect: True
+  What packages do you want to update?
 fields:
-  - Github URL: packages[i].github_url
-  - This is a private GitHub repo: packages[i].is_private
-    datatype: yesno
-  - Github [Personal Access Token](https://docassemble.org/docs/packages.html#github_install): packages[i].github_token
-    show if: packages[i].is_private
-    default: |
-      ${ get_config('assembly line',{}).get("github install token", "") }
-  - Also add an alias: packages[i].add_alias
-    datatype: yesno
-  - YAML filename: packages[i].yaml_name
-    show if: packages[i].add_alias
-  - Short name or alias (no spaces): packages[i].alias
-    validate: |
-      lambda y: y.isidentifier()
-    show if: packages[i].add_alias
+  - no label: packages
+    required: False
+    datatype: checkboxes
+    code: |
+      [[package.get('name'),f"{package.get('name','')} ({package.get('version')})",True] for package in installed_packages if 'docassemble.' in package.get('name') and package.get('name') not in ['docassemble.demo','docassemble.webapp','docassemble.base']]
 ---
 code: |
   install_packages_task = background_action('install_packages_event')
 ---
 event: install_packages_event
 code: |
-  background_error_action("bg_failure")
   for package in packages:
-    pkgname = install_from_github_url(package.github_url, pat=package.github_token if package.is_private else None)
-    reset(pkgname)
-
-  if any((package.add_alias for package in packages)):
-    the_config = da_get_config()
-    if not the_config.get("dispatch"):
-      the_config["dispatch"] = {}
-    for package in packages:
-      if package.add_alias:
-        package_regex = r"https:\/\/github\.com\/.*\/docassemble-([\w]*)"
-        match = re.search(package_regex, package.github_url)
-        if match:
-          package_path = f"docassemble.{ match.groups()[0] }:data/questions/{ package.yaml_name }"
-          the_config["dispatch"][package.alias] = package_path
-    results = da_write_config(the_config)
-
-  background_response_action("bg_success")
----
-event: bg_success
-code: |
-  it_worked = True
+    data = {"key": install_packages_api_key,
+            "update": package
+            }
+    # This won't persist after backround task completes
+    package.status = daREST.post("package",data=data)
   background_response()
 ---  
 event: waiting_screen
 question: |
-  Wait here while we start the installation process
+  Wait here
 reload: True
 ---
-event: bg_failure
-code: |
-  it_worked = False
-  background_response()
----
 event: ending_screen
 question: |
   All done
-subquestion: |
-  % if it_worked:
-  It may take a few minutes for the installation process to complete.
-
-  % if any((package.add_alias for package in packages)):
-  You can now use these links to reach your interviews:
-  
-  % for package in packages:
-  % if package.add_alias:
-  * [${package.alias}](/start/${package.alias})
-  % endif
-  % endfor
-  % endif
-  % else:
-  Something went wrong. Check the [worker.log](/logs?file=worker.log) to learn what.
-  % endif
-
 buttons:
   - Restart: restart
```

### Comparing `docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/data/questions/manage_users.yml` & `docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/data/questions/manage_users.yml`

 * *Files 19% similar despite different names*

```diff
@@ -3,74 +3,47 @@
   - nav.yml
 ---
 metadata:
   title: Manage users
   sessions are unique: True
   required privileges:
     - admin
-    - al_manage_users
   temporary session: True
 ---
 modules:
   - .aldashboard
-  - .create_package
 ---
 mandatory: True
 id: interview order
 code: |
   chosen_user
   if user_task == 'reset_password':
     do_update_password
   elif user_task == 'elevate_permissions':
     do_update_privileges
-  elif user_task == 'download_playground':
-    do_download_playground
   ending_screen    
 ---
-code: |
-  user_lookup = {}
-  for user in get_users_and_name():
-    user_lookup[user[0]] = user[3]
----
 id: select user
 question: |
   Manage users
-subquestion: |
-  % if not user_has_privilege(["admin"]):
-  **Note**: make sure the role `al_manage_users` any of the the following desired [permissions](https://docassemble.org/docs/config.html#permissions)
-  in the global configuration:
-
-  ```
-  permissions:
-    al_manage_users:
-      - access_user_info
-      - edit_user_active_status
-      - edit_user_password
-      - delete_user
-      - edit_sessions
-      - access_sessions
-      - access_privileges 
-      - edit_user_privileges
-  ```
-  % endif
 fields:
   - User: chosen_user
     datatype: integer
     input type: combobox
     code: |
-      [{user[0]: f"{user[1]} {user[2]} {user[3]}"} for user in get_users_and_name()]
+      [{user[0]: f"{user['first_name']} {user['last_name']} {user['email']}"} for user in get_users_and_name()]      
     exclude:
       - "2"
     # User ID 2 is the "cron" user and should not be managed here        
   - What do you want to do?: user_task
     datatype: radio
     choices:
       - Reset password: reset_password
-      - Download playground files: download_playground
-      - Change user permissions: elevate_permissions      
+      # - Download playground files: download_playground
+      - Change user permissions: elevate_permissions
   - New password: new_user_password
     datatype: password
     show if:
       variable: user_task
       is: reset_password
     validate: valid_password      
   - Verify new password: new_user_password_2
@@ -99,26 +72,17 @@
   set_user_info(user_id=chosen_user, password=new_user_password)
   do_update_password = True
 ---
 code: |
   set_user_info(user_id=chosen_user, privileges=new_permission_level.true_values().elements )
   do_update_privileges = True
 ---
-id: download playground
-question: |
-  Playground download for ${ user_lookup[chosen_user] }
-subquestion: |
-  % for project in get_list_of_projects(chosen_user) + ['default']:
-  [${project}]( ${ create_user_playground_zip(chosen_user, space_to_underscore(user_lookup[chosen_user]), project).url_for() })
-  % endfor
-event: do_download_playground
----
 code: |
   def valid_password(pword):
-    if not re.match(r"^(?=.*[a-z])(?=.*[A-Z])(?=.*\d)[a-zA-Z\d!@#$%^&*()_+\-=\[\]{};:\'\"\\|,.<>\/?]{6,}$", pword):
+    if not re.match(r"^(?=.*[a-z])(?=.*[A-Z])(?=.*\d)[a-zA-Z\d]{6,}$", pword):
       validation_error(word("Password must have at least 6 characters with one lowercase letter, one uppercase letter and one number"))
     return True      
 ---
 event: ending_screen
 question: |
   Task is done
 subquestion: |
```

### Comparing `docassemble_aldashboard-0.24.0.1/docassemble/ALDashboard/data/questions/validate_translation.yml` & `docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/data/questions/validate_translation.yml`

 * *Files identical despite different names*

