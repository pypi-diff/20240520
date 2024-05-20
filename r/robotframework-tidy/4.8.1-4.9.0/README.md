# Comparing `tmp/robotframework-tidy-4.8.1.tar.gz` & `tmp/robotframework-tidy-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-tidy-4.8.1.tar", last modified: Fri Jan 12 08:46:19 2024, max compression
+gzip compressed data, was "robotframework-tidy-4.9.0.tar", last modified: Sat Feb  3 11:33:05 2024, max compression
```

## Comparing `robotframework-tidy-4.8.1.tar` & `robotframework-tidy-4.9.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 08:46:19.679260 robotframework-tidy-4.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-01-12 08:46:19.679260 robotframework-tidy-4.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 08:46:19.675260 robotframework-tidy-4.8.1/robotframework_tidy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-01-12 08:46:19.000000 robotframework-tidy-4.8.1/robotframework_tidy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-01-12 08:46:19.000000 robotframework-tidy-4.8.1/robotframework_tidy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-12 08:46:19.000000 robotframework-tidy-4.8.1/robotframework_tidy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-01-12 08:46:19.000000 robotframework-tidy-4.8.1/robotframework_tidy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-01-12 08:46:19.000000 robotframework-tidy-4.8.1/robotframework_tidy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-12 08:46:19.000000 robotframework-tidy-4.8.1/robotframework_tidy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 08:46:19.671260 robotframework-tidy-4.8.1/robotidy/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 08:46:19.671260 robotframework-tidy-4.8.1/robotidy/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-01-12 08:46:19.000000 robotframework-tidy-4.8.1/robotidy/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-01-12 08:46:19.000000 robotframework-tidy-4.8.1/robotidy/__pycache__/version.cpython-312.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/app.py
--rw-r--r--   0 runner    (1001) docker     (127)    16307 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    15692 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/disablers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/files.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/rich_console.py
--rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/skip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 08:46:19.675260 robotframework-tidy-4.8.1/robotidy/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/transformers/AddMissingEnd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/transformers/AlignKeywordsSection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/transformers/AlignSettingsSection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/transformers/AlignTemplatedTestCases.py
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/transformers/AlignTestCasesSection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/transformers/AlignVariablesSection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/transformers/DiscardEmptySections.py
--rw-r--r--   0 runner    (1001) docker     (127)     6903 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/transformers/GenerateDocumentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9724 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/transformers/IndentNestedKeywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    12568 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/transformers/InlineIf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7889 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/transformers/MergeAndOrderSections.py
--rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/transformers/NormalizeAssignments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/transformers/NormalizeComments.py
--rw-r--r--   0 runner    (1001) docker     (127)     5760 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/transformers/NormalizeNewLines.py
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/transformers/NormalizeSectionHeaderName.py
--rw-r--r--   0 runner    (1001) docker     (127)     8539 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/transformers/NormalizeSeparators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/transformers/NormalizeSettingName.py
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/transformers/NormalizeTags.py
--rw-r--r--   0 runner    (1001) docker     (127)     8471 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/transformers/OrderSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)     8834 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/transformers/OrderSettingsSection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/transformers/OrderTags.py
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/transformers/RemoveEmptySettings.py
--rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/transformers/RenameKeywords.py
--rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/transformers/RenameTestCases.py
--rw-r--r--   0 runner    (1001) docker     (127)    20317 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/transformers/RenameVariables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/transformers/ReplaceBreakContinue.py
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/transformers/ReplaceEmptyValues.py
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/transformers/ReplaceReturns.py
--rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/transformers/ReplaceRunKeywordIf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/transformers/SmartSortKeywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    12254 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/transformers/SplitTooLongLine.py
--rw-r--r--   0 runner    (1001) docker     (127)    10310 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/transformers/Translate.py
--rw-r--r--   0 runner    (1001) docker     (127)    19689 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23078 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/transformers/aligners_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/transformers/run_keywords.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 08:46:19.675260 robotframework-tidy-4.8.1/robotidy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    13963 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/utils/variable_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/robotidy/version.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-12 08:46:19.679260 robotframework-tidy-4.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-01-12 08:46:10.000000 robotframework-tidy-4.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 11:33:05.796443 robotframework-tidy-4.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-02-03 11:33:05.796443 robotframework-tidy-4.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 11:33:05.792443 robotframework-tidy-4.9.0/robotframework_tidy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-02-03 11:33:05.000000 robotframework-tidy-4.9.0/robotframework_tidy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-02-03 11:33:05.000000 robotframework-tidy-4.9.0/robotframework_tidy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-03 11:33:05.000000 robotframework-tidy-4.9.0/robotframework_tidy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-03 11:33:05.000000 robotframework-tidy-4.9.0/robotframework_tidy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-02-03 11:33:05.000000 robotframework-tidy-4.9.0/robotframework_tidy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-03 11:33:05.000000 robotframework-tidy-4.9.0/robotframework_tidy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 11:33:05.784443 robotframework-tidy-4.9.0/robotidy/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 11:33:05.784443 robotframework-tidy-4.9.0/robotidy/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-02-03 11:33:05.000000 robotframework-tidy-4.9.0/robotidy/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-02-03 11:33:05.000000 robotframework-tidy-4.9.0/robotidy/__pycache__/version.cpython-312.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16307 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15692 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/disablers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/rich_console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/skip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 11:33:05.792443 robotframework-tidy-4.9.0/robotidy/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/transformers/AddMissingEnd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/transformers/AlignKeywordsSection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6839 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/transformers/AlignSettingsSection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/transformers/AlignTemplatedTestCases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/transformers/AlignTestCasesSection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/transformers/AlignVariablesSection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/transformers/DiscardEmptySections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/transformers/GenerateDocumentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9724 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/transformers/IndentNestedKeywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12568 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/transformers/InlineIf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7889 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/transformers/MergeAndOrderSections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/transformers/NormalizeAssignments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/transformers/NormalizeComments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5760 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/transformers/NormalizeNewLines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/transformers/NormalizeSectionHeaderName.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8539 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/transformers/NormalizeSeparators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/transformers/NormalizeSettingName.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/transformers/NormalizeTags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8471 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/transformers/OrderSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8834 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/transformers/OrderSettingsSection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/transformers/OrderTags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/transformers/RemoveEmptySettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/transformers/RenameKeywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/transformers/RenameTestCases.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20317 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/transformers/RenameVariables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/transformers/ReplaceBreakContinue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/transformers/ReplaceEmptyValues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/transformers/ReplaceReturns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/transformers/ReplaceRunKeywordIf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/transformers/SmartSortKeywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12254 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/transformers/SplitTooLongLine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10310 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/transformers/Translate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19689 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23078 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/transformers/aligners_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/transformers/run_keywords.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 11:33:05.792443 robotframework-tidy-4.9.0/robotidy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    13963 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/utils/variable_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/robotidy/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-03 11:33:05.796443 robotframework-tidy-4.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-02-03 11:32:54.000000 robotframework-tidy-4.9.0/setup.py
```

### Comparing `robotframework-tidy-4.8.1/LICENSE` & `robotframework-tidy-4.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/PKG-INFO` & `robotframework-tidy-4.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-tidy
-Version: 4.8.1
+Version: 4.9.0
 Summary: Code autoformatter for Robot Framework
 Home-page: https://github.com/MarketSquare/robotframework-tidy
 Author: MarketSquare - Robot Framework community
 Author-email: bartek.hirsz@gmail.com
 License: Apache License 2.0
 Keywords: robotframework
 Platform: any
@@ -22,15 +22,15 @@
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: robotframework>=4.0
+Requires-Dist: robotframework<8.0,>=4.0
 Requires-Dist: click==8.1.*
 Requires-Dist: colorama<0.4.7,>=0.4.3
 Requires-Dist: pathspec<0.12.2,>=0.9.0
 Requires-Dist: tomli==2.0.*
 Requires-Dist: rich_click<1.7.4,>=1.4
 Requires-Dist: jinja2<4.0,>=3.1.3
 Provides-Extra: dev
```

### Comparing `robotframework-tidy-4.8.1/README.md` & `robotframework-tidy-4.9.0/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotframework_tidy.egg-info/PKG-INFO` & `robotframework-tidy-4.9.0/robotframework_tidy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-tidy
-Version: 4.8.1
+Version: 4.9.0
 Summary: Code autoformatter for Robot Framework
 Home-page: https://github.com/MarketSquare/robotframework-tidy
 Author: MarketSquare - Robot Framework community
 Author-email: bartek.hirsz@gmail.com
 License: Apache License 2.0
 Keywords: robotframework
 Platform: any
@@ -22,15 +22,15 @@
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: robotframework>=4.0
+Requires-Dist: robotframework<8.0,>=4.0
 Requires-Dist: click==8.1.*
 Requires-Dist: colorama<0.4.7,>=0.4.3
 Requires-Dist: pathspec<0.12.2,>=0.9.0
 Requires-Dist: tomli==2.0.*
 Requires-Dist: rich_click<1.7.4,>=1.4
 Requires-Dist: jinja2<4.0,>=3.1.3
 Provides-Extra: dev
```

### Comparing `robotframework-tidy-4.8.1/robotframework_tidy.egg-info/SOURCES.txt` & `robotframework-tidy-4.9.0/robotframework_tidy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotidy/api.py` & `robotframework-tidy-4.9.0/robotidy/api.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotidy/app.py` & `robotframework-tidy-4.9.0/robotidy/app.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotidy/cli.py` & `robotframework-tidy-4.9.0/robotidy/cli.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotidy/config.py` & `robotframework-tidy-4.9.0/robotidy/config.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotidy/decorators.py` & `robotframework-tidy-4.9.0/robotidy/decorators.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotidy/disablers.py` & `robotframework-tidy-4.9.0/robotidy/disablers.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotidy/exceptions.py` & `robotframework-tidy-4.9.0/robotidy/exceptions.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotidy/files.py` & `robotframework-tidy-4.9.0/robotidy/files.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotidy/skip.py` & `robotframework-tidy-4.9.0/robotidy/skip.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotidy/transformers/AddMissingEnd.py` & `robotframework-tidy-4.9.0/robotidy/transformers/AddMissingEnd.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotidy/transformers/AlignKeywordsSection.py` & `robotframework-tidy-4.9.0/robotidy/transformers/AlignKeywordsSection.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotidy/transformers/AlignSettingsSection.py` & `robotframework-tidy-4.9.0/robotidy/transformers/AlignSettingsSection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from collections import defaultdict
 
-from robot.api.parsing import Token
+from robot.api.parsing import Documentation, Token
 from robot.parsing.model import Statement
 
 from robotidy.disablers import skip_section_if_disabled
+from robotidy.skip import Skip
 from robotidy.transformers import Transformer
 from robotidy.utils import misc
 
 
 class AlignSettingsSection(Transformer):
     """
     Align statements in ``*** Settings ***`` section to columns.
@@ -65,39 +66,52 @@
         Token.SUITE_SETUP,
         Token.SUITE_TEARDOWN,
         Token.TEST_SETUP,
         Token.TEST_TEARDOWN,
         Token.LIBRARY,
         Token.VARIABLES,
     }
+    HANDLES_SKIP = frozenset({"skip_documentation"})
 
-    def __init__(self, up_to_column: int = 2, argument_indent: int = 4, min_width: int = None, fixed_width: int = None):
-        super().__init__()
+    def __init__(
+        self,
+        up_to_column: int = 2,
+        argument_indent: int = 4,
+        min_width: int = None,
+        fixed_width: int = None,
+        skip: Skip = None,
+    ):
+        super().__init__(skip=skip)
         self.up_to_column = up_to_column - 1
         self.argument_indent = argument_indent
         self.min_width = min_width
         self.fixed_width = fixed_width
 
     @skip_section_if_disabled
     def visit_SettingSection(self, node):  # noqa
         statements = []
         for child in node.body:
-            if self.disablers.is_node_disabled(child):
+            if self.disablers.is_node_disabled(child) or self.is_node_skip(child):
                 statements.append(child)
             elif child.type in (Token.EOL, Token.COMMENT):
                 statements.append(misc.left_align(child))
             else:
                 statements.append(list(misc.tokens_by_lines(child)))
         nodes_to_be_aligned = [st for st in statements if isinstance(st, list)]
         if not nodes_to_be_aligned:
             return node
         look_up = self.create_look_up(nodes_to_be_aligned)  # for every col find longest value
         node.body = self.align_rows(statements, look_up)
         return node
 
+    def is_node_skip(self, node):
+        if isinstance(node, Documentation) and self.skip.documentation:
+            return True
+        return False
+
     def should_indent_arguments(self, statement):
         statement_type = statement[0][0].type
         is_library = statement_type == Token.LIBRARY
         if is_library:
             return is_library, True
         return is_library, statement_type in self.TOKENS_WITH_ARGUMENTS
```

### Comparing `robotframework-tidy-4.8.1/robotidy/transformers/AlignTemplatedTestCases.py` & `robotframework-tidy-4.9.0/robotidy/transformers/AlignTemplatedTestCases.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotidy/transformers/AlignTestCasesSection.py` & `robotframework-tidy-4.9.0/robotidy/transformers/AlignTestCasesSection.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotidy/transformers/AlignVariablesSection.py` & `robotframework-tidy-4.9.0/robotidy/transformers/AlignVariablesSection.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotidy/transformers/DiscardEmptySections.py` & `robotframework-tidy-4.9.0/robotidy/transformers/DiscardEmptySections.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotidy/transformers/GenerateDocumentation.py` & `robotframework-tidy-4.9.0/robotidy/transformers/GenerateDocumentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,14 +131,19 @@
 
     def __init__(self, overwrite: bool = False, doc_template: str = "google", template_directory: Optional[str] = None):
         self.overwrite = overwrite
         self.doc_template = self.load_template(doc_template, template_directory)
         self.args_returns_finder = ArgumentsAndReturnsVisitor()
         super().__init__()
 
+    def visit_TestCaseSection(self, node):  # noqa
+        return node
+
+    visit_SettingSection = visit_TestCaseSection
+
     def load_template(self, template: str, template_directory: Optional[str] = None) -> str:
         try:
             return Template(self.get_template(template, template_directory))
         except TemplateError as err:
             raise InvalidParameterValueError(
                 self.__class__.__name__,
                 "doc_template",
```

### Comparing `robotframework-tidy-4.8.1/robotidy/transformers/IndentNestedKeywords.py` & `robotframework-tidy-4.9.0/robotidy/transformers/IndentNestedKeywords.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotidy/transformers/InlineIf.py` & `robotframework-tidy-4.9.0/robotidy/transformers/InlineIf.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotidy/transformers/MergeAndOrderSections.py` & `robotframework-tidy-4.9.0/robotidy/transformers/MergeAndOrderSections.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotidy/transformers/NormalizeAssignments.py` & `robotframework-tidy-4.9.0/robotidy/transformers/NormalizeAssignments.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotidy/transformers/NormalizeComments.py` & `robotframework-tidy-4.9.0/robotidy/transformers/NormalizeComments.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotidy/transformers/NormalizeNewLines.py` & `robotframework-tidy-4.9.0/robotidy/transformers/NormalizeNewLines.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotidy/transformers/NormalizeSectionHeaderName.py` & `robotframework-tidy-4.9.0/robotidy/transformers/NormalizeSectionHeaderName.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotidy/transformers/NormalizeSeparators.py` & `robotframework-tidy-4.9.0/robotidy/transformers/NormalizeSeparators.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotidy/transformers/NormalizeSettingName.py` & `robotframework-tidy-4.9.0/robotidy/transformers/NormalizeSettingName.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotidy/transformers/NormalizeTags.py` & `robotframework-tidy-4.9.0/robotidy/transformers/NormalizeTags.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotidy/transformers/OrderSettings.py` & `robotframework-tidy-4.9.0/robotidy/transformers/OrderSettings.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotidy/transformers/OrderSettingsSection.py` & `robotframework-tidy-4.9.0/robotidy/transformers/OrderSettingsSection.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotidy/transformers/OrderTags.py` & `robotframework-tidy-4.9.0/robotidy/transformers/OrderTags.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotidy/transformers/RemoveEmptySettings.py` & `robotframework-tidy-4.9.0/robotidy/transformers/RemoveEmptySettings.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotidy/transformers/RenameKeywords.py` & `robotframework-tidy-4.9.0/robotidy/transformers/RenameKeywords.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotidy/transformers/RenameTestCases.py` & `robotframework-tidy-4.9.0/robotidy/transformers/RenameTestCases.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotidy/transformers/RenameVariables.py` & `robotframework-tidy-4.9.0/robotidy/transformers/RenameVariables.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotidy/transformers/ReplaceBreakContinue.py` & `robotframework-tidy-4.9.0/robotidy/transformers/ReplaceBreakContinue.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotidy/transformers/ReplaceEmptyValues.py` & `robotframework-tidy-4.9.0/robotidy/transformers/ReplaceEmptyValues.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotidy/transformers/ReplaceReturns.py` & `robotframework-tidy-4.9.0/robotidy/transformers/ReplaceReturns.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotidy/transformers/ReplaceRunKeywordIf.py` & `robotframework-tidy-4.9.0/robotidy/transformers/ReplaceRunKeywordIf.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotidy/transformers/SmartSortKeywords.py` & `robotframework-tidy-4.9.0/robotidy/transformers/SmartSortKeywords.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotidy/transformers/SplitTooLongLine.py` & `robotframework-tidy-4.9.0/robotidy/transformers/SplitTooLongLine.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotidy/transformers/Translate.py` & `robotframework-tidy-4.9.0/robotidy/transformers/Translate.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotidy/transformers/__init__.py` & `robotframework-tidy-4.9.0/robotidy/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotidy/transformers/aligners_core.py` & `robotframework-tidy-4.9.0/robotidy/transformers/aligners_core.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotidy/transformers/run_keywords.py` & `robotframework-tidy-4.9.0/robotidy/transformers/run_keywords.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotidy/utils/misc.py` & `robotframework-tidy-4.9.0/robotidy/utils/misc.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/robotidy/utils/variable_matcher.py` & `robotframework-tidy-4.9.0/robotidy/utils/variable_matcher.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.8.1/setup.py` & `robotframework-tidy-4.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     platforms="any",
     classifiers=CLASSIFIERS,
     keywords="robotframework",
     packages=["robotidy"],
     include_package_data=True,
     python_requires=">=3.7",
     install_requires=[
-        "robotframework>=4.0",
+        "robotframework>=4.0,<8.0",
         "click==8.1.*",
         "colorama>=0.4.3,<0.4.7",
         "pathspec>=0.9.0,<0.12.2",
         "tomli==2.0.*",
         "rich_click>=1.4,<1.7.4",
         "jinja2>=3.1.3,<4.0",
     ],
```

