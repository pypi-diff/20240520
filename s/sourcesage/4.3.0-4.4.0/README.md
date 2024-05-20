# Comparing `tmp/sourcesage-4.3.0.tar.gz` & `tmp/sourcesage-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sourcesage-4.3.0.tar", last modified: Tue May 14 15:07:27 2024, max compression
+gzip compressed data, was "sourcesage-4.4.0.tar", last modified: Mon May 20 08:49:42 2024, max compression
```

## Comparing `sourcesage-4.3.0.tar` & `sourcesage-4.4.0.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:07:27.612118 sourcesage-4.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-14 15:07:22.000000 sourcesage-4.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19660 2024-05-14 15:07:27.612118 sourcesage-4.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19252 2024-05-14 15:07:22.000000 sourcesage-4.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 15:07:27.612118 sourcesage-4.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-14 15:07:23.000000 sourcesage-4.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:07:27.604118 sourcesage-4.3.0/sourcesage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:07:27.608118 sourcesage-4.3.0/sourcesage/config/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/config/.SourceSageignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:07:27.608118 sourcesage-4.3.0/sourcesage/config/ISSUES_RESOLVE/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/config/ISSUES_RESOLVE/ISSUES_RESOLVE_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:07:27.608118 sourcesage-4.3.0/sourcesage/config/STAGE_INFO/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/config/STAGE_INFO/STAGE_INFO_AND_ISSUES_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_EMOJI.md
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_GAIAH.md
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/config/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/config/language_map.json
--rw-r--r--   0 runner    (1001) docker     (127)     6334 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:07:27.608118 sourcesage-4.3.0/sourcesage/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/modules/ChangelogGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/modules/ChangelogUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/modules/DiffChangelogGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/modules/EnvFileHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/modules/GitHubIssueRetrieve.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/modules/GitHubUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/modules/IssuesToMarkdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/modules/ReleaseDiffReportGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/modules/StageInfoGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/modules/StagedDiffGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/modules/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/modules/markdown_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/modules/source_sage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:07:27.612118 sourcesage-4.3.0/sourcesage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19660 2024-05-14 15:07:27.000000 sourcesage-4.3.0/sourcesage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-14 15:07:27.000000 sourcesage-4.3.0/sourcesage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:07:27.000000 sourcesage-4.3.0/sourcesage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-14 15:07:27.000000 sourcesage-4.3.0/sourcesage.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-14 15:07:27.000000 sourcesage-4.3.0/sourcesage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 15:07:27.000000 sourcesage-4.3.0/sourcesage.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:07:27.612118 sourcesage-4.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-05-14 15:07:23.000000 sourcesage-4.3.0/tests/test_sourcesage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:49:42.348407 sourcesage-4.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-20 08:49:34.000000 sourcesage-4.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19660 2024-05-20 08:49:42.348407 sourcesage-4.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19252 2024-05-20 08:49:34.000000 sourcesage-4.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 08:49:42.348407 sourcesage-4.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-20 08:49:34.000000 sourcesage-4.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:49:42.340407 sourcesage-4.4.0/sourcesage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 08:49:34.000000 sourcesage-4.4.0/sourcesage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-05-20 08:49:34.000000 sourcesage-4.4.0/sourcesage/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:49:42.344407 sourcesage-4.4.0/sourcesage/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-20 08:49:34.000000 sourcesage-4.4.0/sourcesage/config/.SourceSageignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:49:42.344407 sourcesage-4.4.0/sourcesage/config/ISSUES_RESOLVE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-20 08:49:34.000000 sourcesage-4.4.0/sourcesage/config/ISSUES_RESOLVE/ISSUES_RESOLVE_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:49:42.344407 sourcesage-4.4.0/sourcesage/config/STAGE_INFO/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-20 08:49:34.000000 sourcesage-4.4.0/sourcesage/config/STAGE_INFO/STAGE_INFO_AND_ISSUES_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-20 08:49:34.000000 sourcesage-4.4.0/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-20 08:49:34.000000 sourcesage-4.4.0/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_EMOJI.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-20 08:49:34.000000 sourcesage-4.4.0/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_GAIAH.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-05-20 08:49:34.000000 sourcesage-4.4.0/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_GAIAH_B.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-20 08:49:34.000000 sourcesage-4.4.0/sourcesage/config/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-20 08:49:34.000000 sourcesage-4.4.0/sourcesage/config/language_map.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7034 2024-05-20 08:49:34.000000 sourcesage-4.4.0/sourcesage/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:49:42.348407 sourcesage-4.4.0/sourcesage/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-05-20 08:49:34.000000 sourcesage-4.4.0/sourcesage/modules/ChangelogGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-20 08:49:34.000000 sourcesage-4.4.0/sourcesage/modules/ChangelogUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-20 08:49:34.000000 sourcesage-4.4.0/sourcesage/modules/DiffChangelogGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-20 08:49:34.000000 sourcesage-4.4.0/sourcesage/modules/EnvFileHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-20 08:49:34.000000 sourcesage-4.4.0/sourcesage/modules/GitHubIssueRetrieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-20 08:49:34.000000 sourcesage-4.4.0/sourcesage/modules/GitHubUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-20 08:49:34.000000 sourcesage-4.4.0/sourcesage/modules/IssuesToMarkdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-05-20 08:49:34.000000 sourcesage-4.4.0/sourcesage/modules/ReleaseDiffReportGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-20 08:49:34.000000 sourcesage-4.4.0/sourcesage/modules/StageInfoGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-05-20 08:49:34.000000 sourcesage-4.4.0/sourcesage/modules/StagedDiffGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 08:49:34.000000 sourcesage-4.4.0/sourcesage/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-20 08:49:34.000000 sourcesage-4.4.0/sourcesage/modules/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-20 08:49:34.000000 sourcesage-4.4.0/sourcesage/modules/markdown_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-20 08:49:34.000000 sourcesage-4.4.0/sourcesage/modules/source_sage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:49:42.348407 sourcesage-4.4.0/sourcesage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19660 2024-05-20 08:49:42.000000 sourcesage-4.4.0/sourcesage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-20 08:49:42.000000 sourcesage-4.4.0/sourcesage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 08:49:42.000000 sourcesage-4.4.0/sourcesage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-20 08:49:42.000000 sourcesage-4.4.0/sourcesage.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-20 08:49:42.000000 sourcesage-4.4.0/sourcesage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-20 08:49:42.000000 sourcesage-4.4.0/sourcesage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:49:42.348407 sourcesage-4.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-05-20 08:49:34.000000 sourcesage-4.4.0/tests/test_sourcesage.py
```

### Comparing `sourcesage-4.3.0/LICENSE` & `sourcesage-4.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sourcesage-4.3.0/PKG-INFO` & `sourcesage-4.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sourcesage
-Version: 4.3.0
+Version: 4.4.0
 Home-page: https://github.com/Sunwood-ai-labs/SourceSage
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: loguru
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sourcesage Version: 4.3.0 Home-page: https://
+Metadata-Version: 2.1 Name: sourcesage Version: 4.4.0 Home-page: https://
 github.com/Sunwood-ai-labs/SourceSage Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 loguru Requires-Dist: GitPython Requires-Dist: requests Requires-Dist: art
 Requires-Dist: termcolor
  [https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/
                              SourceSage_icon4.png]
```

### Comparing `sourcesage-4.3.0/README.md` & `sourcesage-4.4.0/README.md`

 * *Files identical despite different names*

### Comparing `sourcesage-4.3.0/setup.py` & `sourcesage-4.4.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #    required = f.read().splitlines()
 
 setup(
     # パッケージの名前
     name='sourcesage',
     
     # パッケージのバージョン
-    version='4.3.0',
+    version='4.4.0',
     
     # パッケージに含めるモジュールを自動的に探す
     packages=find_packages(),
     
     # パッケージの分類情報
     classifiers=[
         "Development Status :: 4 - Beta",
```

### Comparing `sourcesage-4.3.0/sourcesage/cli.py` & `sourcesage-4.4.0/sourcesage/cli.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.3.0/sourcesage/config/ISSUES_RESOLVE/ISSUES_RESOLVE_TEMPLATE.md` & `sourcesage-4.4.0/sourcesage/config/ISSUES_RESOLVE/ISSUES_RESOLVE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `sourcesage-4.3.0/sourcesage/config/STAGE_INFO/STAGE_INFO_AND_ISSUES_TEMPLATE.md` & `sourcesage-4.4.0/sourcesage/config/STAGE_INFO/STAGE_INFO_AND_ISSUES_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `sourcesage-4.3.0/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE.md` & `sourcesage-4.4.0/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `sourcesage-4.3.0/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_EMOJI.md` & `sourcesage-4.4.0/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_EMOJI.md`

 * *Files identical despite different names*

### Comparing `sourcesage-4.3.0/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_GAIAH.md` & `sourcesage-4.4.0/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_GAIAH.md`

 * *Files identical despite different names*

### Comparing `sourcesage-4.3.0/sourcesage/config/constants.py` & `sourcesage-4.4.0/sourcesage/config/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,8 +34,10 @@
         self.STAGE_INFO_TEMPLATE_MD = "STAGE_INFO_AND_ISSUES_TEMPLATE.md"
 
         self.STAGE_INFO_SIMPLE_OUTPUT_MD = "STAGE_INFO_AND_PROMT.md"
         self.STAGE_INFO_SIMPLE_TEMPLATE_MD = "STAGE_INFO_TEMPLATE.md"
         self.STAGE_INFO_SIMPLE_OUTPUT_MD_EMOJI = "STAGE_INFO_AND_PROMT_EMOJI.md"
         self.STAGE_INFO_SIMPLE_TEMPLATE_MD_EMOJI = "STAGE_INFO_TEMPLATE_EMOJI.md"
         self.STAGE_INFO_SIMPLE_OUTPUT_MD_GAIAH = "STAGE_INFO_AND_PROMT_GAIAH.md"
-        self.STAGE_INFO_SIMPLE_TEMPLATE_MD_GAIAH = "STAGE_INFO_TEMPLATE_GAIAH.md"
+        self.STAGE_INFO_SIMPLE_TEMPLATE_MD_GAIAH = "STAGE_INFO_TEMPLATE_GAIAH.md"
+        self.STAGE_INFO_SIMPLE_OUTPUT_MD_GAIAH_B = "STAGE_INFO_AND_PROMT_GAIAH_B.md"
+        self.STAGE_INFO_SIMPLE_TEMPLATE_MD_GAIAH_B = "STAGE_INFO_TEMPLATE_GAIAH_B.md"
```

### Comparing `sourcesage-4.3.0/sourcesage/config/language_map.json` & `sourcesage-4.4.0/sourcesage/config/language_map.json`

 * *Files identical despite different names*

### Comparing `sourcesage-4.3.0/sourcesage/core.py` & `sourcesage-4.4.0/sourcesage/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,14 +75,20 @@
         stage_info_generator.run()
         stage_info_generator = StageInfoGenerator(issue_file_path=os.path.join(self.constants.ISSUE_LOG_DIR, self.constants.ISSUES_FILE_NAME),
                                                   stage_diff_file_path=os.path.join(self.constants.SOURCE_SAGE_ASSETS_DIR, self.constants.STAGED_DIFF_MD),
                                                   template_file_path=os.path.join(self.constants.DOCS_DIR, self.constants.TEMPLATE_STAGE_INFO_DIR, self.constants.STAGE_INFO_SIMPLE_TEMPLATE_MD_GAIAH),
                                                   output_file_path=os.path.join(self.constants.STAGE_INFO_DIR, self.constants.STAGE_INFO_SIMPLE_OUTPUT_MD_GAIAH))
         stage_info_generator.run()
 
+        stage_info_generator = StageInfoGenerator(issue_file_path=os.path.join(self.constants.ISSUE_LOG_DIR, self.constants.ISSUES_FILE_NAME),
+                                                  stage_diff_file_path=os.path.join(self.constants.SOURCE_SAGE_ASSETS_DIR, self.constants.STAGED_DIFF_MD),
+                                                  template_file_path=os.path.join(self.constants.DOCS_DIR, self.constants.TEMPLATE_STAGE_INFO_DIR, self.constants.STAGE_INFO_SIMPLE_TEMPLATE_MD_GAIAH_B),
+                                                  output_file_path=os.path.join(self.constants.STAGE_INFO_DIR, self.constants.STAGE_INFO_SIMPLE_OUTPUT_MD_GAIAH_B))
+        stage_info_generator.run()
+
         # Convert issues to markdown
         issues_to_markdown = IssuesToMarkdown(issues_file=os.path.join(self.constants.ISSUE_LOG_DIR, self.constants.ISSUES_FILE_NAME),
                                               sourcesage_file=os.path.join(self.constants.SOURCE_SAGE_ASSETS_DIR, self.constants.SOURCE_SAGE_MD),
                                               template_file=os.path.join(self.constants.DOCS_DIR, self.constants.TEMPLATE_ISSUES_RESOLVE_DIR, self.constants.ISSUES_RESOLVE_TEMPLATE_MD),
                                               output_folder=self.constants.ISSUES_RESOLVE_DIR)
         issues_to_markdown.load_data()
         issues_to_markdown.create_markdown_files()
```

### Comparing `sourcesage-4.3.0/sourcesage/modules/ChangelogGenerator.py` & `sourcesage-4.4.0/sourcesage/modules/ChangelogGenerator.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.3.0/sourcesage/modules/ChangelogUtils.py` & `sourcesage-4.4.0/sourcesage/modules/ChangelogUtils.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.3.0/sourcesage/modules/DiffChangelogGenerator.py` & `sourcesage-4.4.0/sourcesage/modules/DiffChangelogGenerator.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.3.0/sourcesage/modules/EnvFileHandler.py` & `sourcesage-4.4.0/sourcesage/modules/EnvFileHandler.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.3.0/sourcesage/modules/GitHubIssueRetrieve.py` & `sourcesage-4.4.0/sourcesage/modules/GitHubIssueRetrieve.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.3.0/sourcesage/modules/GitHubUtils.py` & `sourcesage-4.4.0/sourcesage/modules/GitHubUtils.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.3.0/sourcesage/modules/IssuesToMarkdown.py` & `sourcesage-4.4.0/sourcesage/modules/IssuesToMarkdown.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.3.0/sourcesage/modules/ReleaseDiffReportGenerator.py` & `sourcesage-4.4.0/sourcesage/modules/ReleaseDiffReportGenerator.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.3.0/sourcesage/modules/StageInfoGenerator.py` & `sourcesage-4.4.0/sourcesage/modules/StageInfoGenerator.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.3.0/sourcesage/modules/StagedDiffGenerator.py` & `sourcesage-4.4.0/sourcesage/modules/StagedDiffGenerator.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.3.0/sourcesage/modules/file_utils.py` & `sourcesage-4.4.0/sourcesage/modules/file_utils.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.3.0/sourcesage/modules/markdown_utils.py` & `sourcesage-4.4.0/sourcesage/modules/markdown_utils.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.3.0/sourcesage/modules/source_sage.py` & `sourcesage-4.4.0/sourcesage/modules/source_sage.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.3.0/sourcesage.egg-info/PKG-INFO` & `sourcesage-4.4.0/sourcesage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sourcesage
-Version: 4.3.0
+Version: 4.4.0
 Home-page: https://github.com/Sunwood-ai-labs/SourceSage
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: loguru
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sourcesage Version: 4.3.0 Home-page: https://
+Metadata-Version: 2.1 Name: sourcesage Version: 4.4.0 Home-page: https://
 github.com/Sunwood-ai-labs/SourceSage Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 loguru Requires-Dist: GitPython Requires-Dist: requests Requires-Dist: art
 Requires-Dist: termcolor
  [https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/
                              SourceSage_icon4.png]
```

### Comparing `sourcesage-4.3.0/sourcesage.egg-info/SOURCES.txt` & `sourcesage-4.4.0/sourcesage.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 sourcesage/config/constants.py
 sourcesage/config/language_map.json
 sourcesage/config/ISSUES_RESOLVE/ISSUES_RESOLVE_TEMPLATE.md
 sourcesage/config/STAGE_INFO/STAGE_INFO_AND_ISSUES_TEMPLATE.md
 sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE.md
 sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_EMOJI.md
 sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_GAIAH.md
+sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_GAIAH_B.md
 sourcesage/modules/ChangelogGenerator.py
 sourcesage/modules/ChangelogUtils.py
 sourcesage/modules/DiffChangelogGenerator.py
 sourcesage/modules/EnvFileHandler.py
 sourcesage/modules/GitHubIssueRetrieve.py
 sourcesage/modules/GitHubUtils.py
 sourcesage/modules/IssuesToMarkdown.py
```

### Comparing `sourcesage-4.3.0/tests/test_sourcesage.py` & `sourcesage-4.4.0/tests/test_sourcesage.py`

 * *Files identical despite different names*

