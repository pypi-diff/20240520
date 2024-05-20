# Comparing `tmp/coverup-0.2.0.tar.gz` & `tmp/coverup-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coverup-0.2.0.tar", last modified: Wed May  1 18:55:42 2024, max compression
+gzip compressed data, was "coverup-0.3.0.tar", last modified: Mon May 20 15:30:00 2024, max compression
```

## Comparing `coverup-0.2.0.tar` & `coverup-0.3.0.tar`

### file list

```diff
@@ -1,88 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:55:42.747093 coverup-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-01 18:55:33.000000 coverup-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6442 2024-05-01 18:55:42.747093 coverup-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-01 18:55:33.000000 coverup-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-01 18:55:33.000000 coverup-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 18:55:42.747093 coverup-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-01 18:55:33.000000 coverup-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:55:42.727092 coverup-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:55:42.747093 coverup-0.2.0/src/CoverUp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6442 2024-05-01 18:55:42.000000 coverup-0.2.0/src/CoverUp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-01 18:55:42.000000 coverup-0.2.0/src/CoverUp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 18:55:42.000000 coverup-0.2.0/src/CoverUp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-01 18:55:42.000000 coverup-0.2.0/src/CoverUp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-01 18:55:42.000000 coverup-0.2.0/src/CoverUp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 18:55:42.000000 coverup-0.2.0/src/CoverUp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:55:42.731092 coverup-0.2.0/src/coverup/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-01 18:55:33.000000 coverup-0.2.0/src/coverup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-01 18:55:33.000000 coverup-0.2.0/src/coverup/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30526 2024-05-01 18:55:33.000000 coverup-0.2.0/src/coverup/coverup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-01 18:55:33.000000 coverup-0.2.0/src/coverup/delta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-05-01 18:55:33.000000 coverup-0.2.0/src/coverup/llm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-05-01 18:55:33.000000 coverup-0.2.0/src/coverup/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-05-01 18:55:33.000000 coverup-0.2.0/src/coverup/pytest_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-05-01 18:55:33.000000 coverup-0.2.0/src/coverup/segment.py
--rw-r--r--   0 runner    (1001) docker     (127)    10257 2024-05-01 18:55:33.000000 coverup-0.2.0/src/coverup/testrunner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-01 18:55:33.000000 coverup-0.2.0/src/coverup/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:55:42.747093 coverup-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_claude_coverup_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_claude_coverup_2.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_claude_coverup_4.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_claude_coverup_5.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_claude_coverup_6.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_claude_coverup_7.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_claude_coverup_8.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_claude_coverup_9.py
--rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_coverup.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_coverup_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_coverup_10.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_coverup_11.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_coverup_12.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_coverup_13.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_coverup_14.py
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_coverup_15.py
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_coverup_16.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_coverup_17.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_coverup_18.py
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_coverup_19.py
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_coverup_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_coverup_20.py
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_coverup_21.py
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_coverup_22.py
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_coverup_23.py
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_coverup_24.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_coverup_25.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_coverup_26.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_coverup_3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_coverup_4.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_coverup_5.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_coverup_6.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_coverup_7.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_coverup_8.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_coverup_9.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_delta.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_llm.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_openai_coverup_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_openai_coverup_10.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_openai_coverup_11.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_openai_coverup_12.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_openai_coverup_13.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_openai_coverup_14.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_openai_coverup_15.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_openai_coverup_18.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_openai_coverup_19.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_openai_coverup_2.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_openai_coverup_3.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_openai_coverup_4.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_openai_coverup_5.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_openai_coverup_6.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_openai_coverup_8.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_openai_coverup_9.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_openai_second_coverup_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_openai_second_coverup_2.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_openai_second_coverup_4.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_openai_second_coverup_5.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     7452 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_segment.py
--rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_testrunner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-01 18:55:33.000000 coverup-0.2.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:30:00.853088 coverup-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-20 15:29:53.000000 coverup-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-05-20 15:30:00.853088 coverup-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-20 15:29:53.000000 coverup-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-20 15:29:53.000000 coverup-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 15:30:00.853088 coverup-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-20 15:29:53.000000 coverup-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:30:00.837088 coverup-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:30:00.853088 coverup-0.3.0/src/CoverUp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-05-20 15:30:00.000000 coverup-0.3.0/src/CoverUp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-20 15:30:00.000000 coverup-0.3.0/src/CoverUp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 15:30:00.000000 coverup-0.3.0/src/CoverUp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-20 15:30:00.000000 coverup-0.3.0/src/CoverUp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-20 15:30:00.000000 coverup-0.3.0/src/CoverUp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-20 15:30:00.000000 coverup-0.3.0/src/CoverUp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:30:00.841088 coverup-0.3.0/src/coverup/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-20 15:29:53.000000 coverup-0.3.0/src/coverup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-20 15:29:53.000000 coverup-0.3.0/src/coverup/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30724 2024-05-20 15:29:53.000000 coverup-0.3.0/src/coverup/coverup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-20 15:29:53.000000 coverup-0.3.0/src/coverup/delta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-05-20 15:29:53.000000 coverup-0.3.0/src/coverup/llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-05-20 15:29:53.000000 coverup-0.3.0/src/coverup/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-05-20 15:29:53.000000 coverup-0.3.0/src/coverup/pytest_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-05-20 15:29:53.000000 coverup-0.3.0/src/coverup/segment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10281 2024-05-20 15:29:53.000000 coverup-0.3.0/src/coverup/testrunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-20 15:29:53.000000 coverup-0.3.0/src/coverup/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-20 15:29:53.000000 coverup-0.3.0/src/coverup/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:30:00.853088 coverup-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_claude_coverup_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_claude_coverup_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_claude_coverup_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_claude_coverup_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_claude_coverup_6.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_claude_coverup_7.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_claude_coverup_8.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_claude_coverup_9.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_coverup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_coverup_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_coverup_10.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_coverup_11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_coverup_12.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_coverup_13.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_coverup_14.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_coverup_15.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_coverup_16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_coverup_17.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_coverup_18.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_coverup_19.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_coverup_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_coverup_20.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_coverup_21.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_coverup_22.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_coverup_23.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_coverup_24.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_coverup_25.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_coverup_26.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_coverup_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_coverup_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_coverup_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_coverup_6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_coverup_7.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_coverup_8.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_coverup_9.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_delta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_openai_coverup_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_openai_coverup_10.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_openai_coverup_11.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_openai_coverup_12.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_openai_coverup_13.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_openai_coverup_14.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_openai_coverup_15.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_openai_coverup_18.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_openai_coverup_19.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_openai_coverup_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_openai_coverup_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_openai_coverup_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_openai_coverup_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_openai_coverup_6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_openai_coverup_8.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_openai_coverup_9.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_openai_second_coverup_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_openai_second_coverup_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_openai_second_coverup_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_openai_second_coverup_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7452 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_segment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_testrunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-20 15:29:53.000000 coverup-0.3.0/tests/test_utils.py
```

### Comparing `coverup-0.2.0/LICENSE` & `coverup-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/PKG-INFO` & `coverup-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoverUp
-Version: 0.2.0
+Version: 0.3.0
 Summary: LLM-powered test coverage improver
 Author-email: Juan Altmayer Pizzorno <juan@altmayer.com>, Emery Berger <emery.berger@gmail.com>
 Project-URL: Homepage, https://github.com/plasma-umass/coverup
 Project-URL: Repository, https://github.com/plasma-umass/coverup
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -15,23 +15,23 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: asyncio
 Requires-Dist: openai
 Requires-Dist: tiktoken
 Requires-Dist: aiolimiter
 Requires-Dist: tqdm
-Requires-Dist: slipcover>=1.0.10
-Requires-Dist: pytest-forked
+Requires-Dist: slipcover>=1.0.13
+Requires-Dist: pytest-cleanslate
 Requires-Dist: litellm>=1.33.1
 
 <!--
-<img src="https://github.com/plasma-umass/coverup/blob/v0.2.0/images/logo.png?raw=True" align="right" width="20%"/>
+<img src="https://github.com/plasma-umass/coverup/blob/v0.3.0/images/logo.png?raw=True" align="right" width="20%"/>
 # CoverUp: Automatically Generating Higher-Coverage Test Suites with AI !
 -->
-<img src="https://github.com/plasma-umass/coverup/blob/v0.2.0/images/logo-with-title.png?raw=True" align="right" width="100%"/>
+<img src="https://github.com/plasma-umass/coverup/blob/v0.3.0/images/logo-with-title.png?raw=True" align="right" width="100%"/>
 
 by [Juan Altmayer Pizzorno](https://jaltmayerpizzorno.github.io) and [Emery Berger](https://emeryberger.com)
 at UMass Amherst's [PLASMA lab](https://plasma-umass.org/).
 
 [![pypi](https://img.shields.io/pypi/v/coverup?color=blue)](https://pypi.org/project/coverup/)
 ![pyversions](https://img.shields.io/pypi/pyversions/coverup)
 
@@ -44,15 +44,15 @@
 CoverUp is designed to work closely with the [pytest](https://docs.pytest.org/en/latest/) test framework.
 To generate tests, it first measures your suite's coverage using [SlipCover](https://github.com/plasma-umass/slipcover), our state-of-the art coverage analyzer.
 It then selects portions of the code that need more testing (that is, code that is uncovered).
 CoverUp then engages in a conversation with an [LLM](https://en.wikipedia.org/wiki/Large_language_model),
 prompting for tests, checking the results to verify that they run and increase coverage (again using SlipCover), and re-prompting for adjustments as necessary.
 Finally, CoverUp optionally checks that the new tests integrate well, attempting to resolve any issues it finds.
 
-For technical details and a complete evaluation, see our arXiv paper, [_CoverUp: Coverage-Guided LLM-Based Test Generation_](https://arxiv.org/abs/2403.16218) ([PDF](https://github.com/plasma-umass/coverup/blob/v0.2.0/CoverUp-arxiv-2403.16218.pdf)).
+For technical details and a complete evaluation, see our arXiv paper, [_CoverUp: Coverage-Guided LLM-Based Test Generation_](https://arxiv.org/abs/2403.16218) ([PDF](https://github.com/plasma-umass/coverup/blob/v0.3.0/CoverUp-arxiv-2403.16218.pdf)).
 
 ## Installing CoverUp
 CoverUp is available from PyPI, so you can install simply with
 ```shell
 $ python3 -m pip install coverup
 ```
 
@@ -99,15 +99,15 @@
 
 To evaluate the tests generated by the LLM, CoverUp must execute them.
 For best security and to minimize the risk of damage to your system, we recommend
 running CoverUp with [Docker](https://www.docker.com/).
 
 ## Evaluation
 
-<img src="https://github.com/plasma-umass/coverup/blob/v0.2.0/images/comparison.png?raw=True" align="right" width="65%"/>
+<img src="https://github.com/plasma-umass/coverup/blob/v0.3.0/images/comparison.png?raw=True" align="right" width="65%"/>
 
 The graph shows CoverUp in comparison to the state-of-the-art [CodaMosa](https://www.carolemieux.com/codamosa_icse23.pdf),
 which itself uses LLM queries to improve on the [Pynguin](https://github.com/se2p/pynguin) test generator.
 For this experiment, both CoverUp and CodaMosa created tests "from scratch", that is, ignoring any existing test suite.
 The bars show the difference in coverage percentage between CoverUp and CodaMosa for various Python modules;
 green bars, above 0, indicate that CoverUp achieved a higher coverage.
```

### Comparing `coverup-0.2.0/README.md` & `coverup-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/pyproject.toml` & `coverup-0.3.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 [project]
 name = "CoverUp"
 description = "LLM-powered test coverage improver"
-dynamic = ["readme"]
-version = "0.2.0"
+dynamic = ["readme", "version"]
 authors = [
     { name="Juan Altmayer Pizzorno", email="juan@altmayer.com" },
     { name="Emery Berger", email="emery.berger@gmail.com" }
 ]
 classifiers = [
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
@@ -18,16 +17,16 @@
 requires-python = ">=3.10"
 dependencies = [
     "asyncio",
     "openai",
     "tiktoken",
     "aiolimiter",
     "tqdm",
-    "slipcover>=1.0.10",
-    "pytest-forked",
+    "slipcover>=1.0.13",
+    "pytest-cleanslate",
     "litellm>=1.33.1"
 ]
 
 [build-system]
 requires = [
     "setuptools>61",
     "wheel",
```

### Comparing `coverup-0.2.0/setup.py` & `coverup-0.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 
 try:
     import tomllib
 except ImportError:
     import tomli as tomllib
 
 def get_version():
-    return tomllib.loads(Path("pyproject.toml").read_text())['project']['version']
+    import re
+    v = re.findall(r"^__version__ *= *\"([^\"]+)\"", Path("src/coverup/version.py").read_text())[0]
+    return v
 
 def get_url():
     return tomllib.loads(Path("pyproject.toml").read_text())['project']['urls']['Repository']
 
 def long_description():
     text = Path("README.md").read_text(encoding="utf-8")
 
@@ -22,10 +24,11 @@
     text = re.sub(r'(src=")((?!https?://))', sub, text)
     text = re.sub(r'(\[.*?\]\()((?!https?://))', sub, text)
 
     return text
 
 if __name__ == "__main__":
     setuptools.setup(
+        version=get_version(),
         long_description=long_description(),
         long_description_content_type="text/markdown",
     )
```

### Comparing `coverup-0.2.0/src/CoverUp.egg-info/PKG-INFO` & `coverup-0.3.0/src/CoverUp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoverUp
-Version: 0.2.0
+Version: 0.3.0
 Summary: LLM-powered test coverage improver
 Author-email: Juan Altmayer Pizzorno <juan@altmayer.com>, Emery Berger <emery.berger@gmail.com>
 Project-URL: Homepage, https://github.com/plasma-umass/coverup
 Project-URL: Repository, https://github.com/plasma-umass/coverup
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -15,23 +15,23 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: asyncio
 Requires-Dist: openai
 Requires-Dist: tiktoken
 Requires-Dist: aiolimiter
 Requires-Dist: tqdm
-Requires-Dist: slipcover>=1.0.10
-Requires-Dist: pytest-forked
+Requires-Dist: slipcover>=1.0.13
+Requires-Dist: pytest-cleanslate
 Requires-Dist: litellm>=1.33.1
 
 <!--
-<img src="https://github.com/plasma-umass/coverup/blob/v0.2.0/images/logo.png?raw=True" align="right" width="20%"/>
+<img src="https://github.com/plasma-umass/coverup/blob/v0.3.0/images/logo.png?raw=True" align="right" width="20%"/>
 # CoverUp: Automatically Generating Higher-Coverage Test Suites with AI !
 -->
-<img src="https://github.com/plasma-umass/coverup/blob/v0.2.0/images/logo-with-title.png?raw=True" align="right" width="100%"/>
+<img src="https://github.com/plasma-umass/coverup/blob/v0.3.0/images/logo-with-title.png?raw=True" align="right" width="100%"/>
 
 by [Juan Altmayer Pizzorno](https://jaltmayerpizzorno.github.io) and [Emery Berger](https://emeryberger.com)
 at UMass Amherst's [PLASMA lab](https://plasma-umass.org/).
 
 [![pypi](https://img.shields.io/pypi/v/coverup?color=blue)](https://pypi.org/project/coverup/)
 ![pyversions](https://img.shields.io/pypi/pyversions/coverup)
 
@@ -44,15 +44,15 @@
 CoverUp is designed to work closely with the [pytest](https://docs.pytest.org/en/latest/) test framework.
 To generate tests, it first measures your suite's coverage using [SlipCover](https://github.com/plasma-umass/slipcover), our state-of-the art coverage analyzer.
 It then selects portions of the code that need more testing (that is, code that is uncovered).
 CoverUp then engages in a conversation with an [LLM](https://en.wikipedia.org/wiki/Large_language_model),
 prompting for tests, checking the results to verify that they run and increase coverage (again using SlipCover), and re-prompting for adjustments as necessary.
 Finally, CoverUp optionally checks that the new tests integrate well, attempting to resolve any issues it finds.
 
-For technical details and a complete evaluation, see our arXiv paper, [_CoverUp: Coverage-Guided LLM-Based Test Generation_](https://arxiv.org/abs/2403.16218) ([PDF](https://github.com/plasma-umass/coverup/blob/v0.2.0/CoverUp-arxiv-2403.16218.pdf)).
+For technical details and a complete evaluation, see our arXiv paper, [_CoverUp: Coverage-Guided LLM-Based Test Generation_](https://arxiv.org/abs/2403.16218) ([PDF](https://github.com/plasma-umass/coverup/blob/v0.3.0/CoverUp-arxiv-2403.16218.pdf)).
 
 ## Installing CoverUp
 CoverUp is available from PyPI, so you can install simply with
 ```shell
 $ python3 -m pip install coverup
 ```
 
@@ -99,15 +99,15 @@
 
 To evaluate the tests generated by the LLM, CoverUp must execute them.
 For best security and to minimize the risk of damage to your system, we recommend
 running CoverUp with [Docker](https://www.docker.com/).
 
 ## Evaluation
 
-<img src="https://github.com/plasma-umass/coverup/blob/v0.2.0/images/comparison.png?raw=True" align="right" width="65%"/>
+<img src="https://github.com/plasma-umass/coverup/blob/v0.3.0/images/comparison.png?raw=True" align="right" width="65%"/>
 
 The graph shows CoverUp in comparison to the state-of-the-art [CodaMosa](https://www.carolemieux.com/codamosa_icse23.pdf),
 which itself uses LLM queries to improve on the [Pynguin](https://github.com/se2p/pynguin) test generator.
 For this experiment, both CoverUp and CodaMosa created tests "from scratch", that is, ignoring any existing test suite.
 The bars show the difference in coverage percentage between CoverUp and CodaMosa for various Python modules;
 green bars, above 0, indicate that CoverUp achieved a higher coverage.
```

### Comparing `coverup-0.2.0/src/CoverUp.egg-info/SOURCES.txt` & `coverup-0.3.0/src/CoverUp.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 src/coverup/delta.py
 src/coverup/llm.py
 src/coverup/prompt.py
 src/coverup/pytest_plugin.py
 src/coverup/segment.py
 src/coverup/testrunner.py
 src/coverup/utils.py
+src/coverup/version.py
 tests/test_claude_coverup_1.py
 tests/test_claude_coverup_2.py
 tests/test_claude_coverup_4.py
 tests/test_claude_coverup_5.py
 tests/test_claude_coverup_6.py
 tests/test_claude_coverup_7.py
 tests/test_claude_coverup_8.py
```

### Comparing `coverup-0.2.0/src/coverup/coverup.py` & `coverup-0.3.0/src/coverup/coverup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 from pathlib import Path
 from datetime import datetime
 
 from .llm import *
 from .segment import *
 from .testrunner import *
+from .version import __version__
 from . import prompt
 
 
 # Turn off most logging
 litellm.set_verbose = False
 logging.getLogger().setLevel(logging.ERROR)
 # Ignore unavailable parameters
@@ -51,15 +52,15 @@
     ap.add_argument('--checkpoint', type=Path, 
                     help=f'path to save progress to (and to resume it from)')
     ap.add_argument('--no-checkpoint', action='store_const', const=None, dest='checkpoint', default=argparse.SUPPRESS,
                     help=f'disables checkpoint')
 
     def default_model():
         if 'OPENAI_API_KEY' in os.environ:
-            return "openai/gpt-4-1106-preview"
+            return "openai/gpt-4o-2024-05-13"
         if 'ANTHROPIC_API_KEY' in os.environ:
             return "anthropic/claude-3-sonnet-20240229"
         if 'AWS_ACCESS_KEY_ID' in os.environ:
             return "bedrock/anthropic.claude-3-sonnet-20240229-v1:0"
 
     ap.add_argument('--model', type=str, default=default_model(),
                     help='OpenAI model to use')
@@ -140,14 +141,17 @@
         ivalue = int(value)
         if ivalue < 0: raise argparse.ArgumentTypeError("must be a number >= 0")
         return ivalue
 
     ap.add_argument('--max-concurrency', type=positive_int, default=50,
                     help='maximum number of parallel requests; 0 means unlimited')
 
+    ap.add_argument('--version', action='version',
+                    version=f"%(prog)s v{__version__} (Python {'.'.join(map(str, sys.version_info[:3]))})")
+
     args = ap.parse_args(args)
 
     for i in range(len(args.source_files)):
         args.source_files[i] = args.source_files[i].resolve()
 
     if args.disable_failing and args.disable_polluting:
         ap.error('Specify only one of --disable-failing and --disable-polluting')
@@ -802,14 +806,14 @@
         if args.checkpoint:
             state.set_final_coverage(coverage)
             state.save_checkpoint(args.checkpoint)
 
         if required := get_required_modules():
             # Sometimes GPT outputs 'from your_module import XYZ', asking us to modify
             # FIXME move this to 'state'
-            print(f"Some modules seem missing:  {', '.join(str(m) for m in required)}")
+            print(f"Some modules seem to be missing:  {', '.join(str(m) for m in required)}")
             if args.write_requirements_to:
                 with args.write_requirements_to.open("a") as f:
                     for module in required:
                         f.write(f"{module}\n")
 
     return 0
```

### Comparing `coverup-0.2.0/src/coverup/delta.py` & `coverup-0.3.0/src/coverup/delta.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/src/coverup/llm.py` & `coverup-0.3.0/src/coverup/llm.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/src/coverup/prompt.py` & `coverup-0.3.0/src/coverup/prompt.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/src/coverup/pytest_plugin.py` & `coverup-0.3.0/src/coverup/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/src/coverup/segment.py` & `coverup-0.3.0/src/coverup/segment.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/src/coverup/testrunner.py` & `coverup-0.3.0/src/coverup/testrunner.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,21 +43,21 @@
     """Runs an entire test suite and returns the coverage obtained."""
 
     with tempfile.NamedTemporaryFile(suffix='.json', delete=False) as j:
         try:
             command = [sys.executable,
                        '-m', 'slipcover', '--source', source_dir] + (['--branch'] if branch_coverage else []) + \
                             ['--json', '--out', j.name] + \
-                            (['--isolate-tests'] if isolate_tests else []) + \
-                      ['-m', 'pytest'] + pytest_args.split() + ['--disable-warnings', '-x', tests_dir]
+                      ['-m', 'pytest'] + pytest_args.split() + (['--cleanslate'] if isolate_tests else []) + \
+                            ['--disable-warnings', '-x', tests_dir]
 
             if trace: trace(command)
             p = subprocess.run(command, check=False, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
             if p.returncode not in (pytest.ExitCode.OK, pytest.ExitCode.NO_TESTS_COLLECTED):
-                if trace: trace(f"tests rc={p.returncode}")
+                if trace: trace(f"tests rc={p.returncode}\n" + str(p.stdout, 'utf-8'))
                 p.check_returncode()
 
             try:
                 return json.load(j)
             except json.decoder.JSONDecodeError:
                 # The JSON is broken, so pytest's execution likely aborted (e.g. a Python unhandled exception).
                 p.check_returncode() # this will almost certainly raise an exception. If not, we do it ourselves:
```

### Comparing `coverup-0.2.0/src/coverup/utils.py` & `coverup-0.3.0/src/coverup/utils.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_claude_coverup_1.py` & `coverup-0.3.0/tests/test_claude_coverup_1.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_claude_coverup_4.py` & `coverup-0.3.0/tests/test_claude_coverup_4.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_claude_coverup_5.py` & `coverup-0.3.0/tests/test_claude_coverup_5.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_claude_coverup_6.py` & `coverup-0.3.0/tests/test_claude_coverup_6.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_claude_coverup_9.py` & `coverup-0.3.0/tests/test_claude_coverup_9.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_coverup.py` & `coverup-0.3.0/tests/test_coverup.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_coverup_1.py` & `coverup-0.3.0/tests/test_coverup_1.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_coverup_10.py` & `coverup-0.3.0/tests/test_coverup_10.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_coverup_11.py` & `coverup-0.3.0/tests/test_coverup_11.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_coverup_12.py` & `coverup-0.3.0/tests/test_coverup_12.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_coverup_13.py` & `coverup-0.3.0/tests/test_coverup_13.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_coverup_14.py` & `coverup-0.3.0/tests/test_coverup_14.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_coverup_15.py` & `coverup-0.3.0/tests/test_coverup_15.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_coverup_16.py` & `coverup-0.3.0/tests/test_coverup_16.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_coverup_17.py` & `coverup-0.3.0/tests/test_coverup_17.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_coverup_18.py` & `coverup-0.3.0/tests/test_coverup_18.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_coverup_19.py` & `coverup-0.3.0/tests/test_coverup_19.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_coverup_2.py` & `coverup-0.3.0/tests/test_coverup_2.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_coverup_20.py` & `coverup-0.3.0/tests/test_coverup_20.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_coverup_21.py` & `coverup-0.3.0/tests/test_coverup_21.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_coverup_22.py` & `coverup-0.3.0/tests/test_coverup_22.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_coverup_23.py` & `coverup-0.3.0/tests/test_coverup_23.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_coverup_24.py` & `coverup-0.3.0/tests/test_coverup_24.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_coverup_25.py` & `coverup-0.3.0/tests/test_coverup_25.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_coverup_26.py` & `coverup-0.3.0/tests/test_coverup_26.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_coverup_3.py` & `coverup-0.3.0/tests/test_coverup_3.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_coverup_4.py` & `coverup-0.3.0/tests/test_coverup_4.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_coverup_5.py` & `coverup-0.3.0/tests/test_coverup_5.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_coverup_6.py` & `coverup-0.3.0/tests/test_coverup_6.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_coverup_7.py` & `coverup-0.3.0/tests/test_coverup_7.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_coverup_8.py` & `coverup-0.3.0/tests/test_coverup_8.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_coverup_9.py` & `coverup-0.3.0/tests/test_coverup_9.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_delta.py` & `coverup-0.3.0/tests/test_delta.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_llm.py` & `coverup-0.3.0/tests/test_llm.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_openai_coverup_10.py` & `coverup-0.3.0/tests/test_openai_coverup_10.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_openai_coverup_11.py` & `coverup-0.3.0/tests/test_openai_coverup_11.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_openai_coverup_12.py` & `coverup-0.3.0/tests/test_openai_coverup_12.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_openai_coverup_13.py` & `coverup-0.3.0/tests/test_openai_coverup_13.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_openai_coverup_14.py` & `coverup-0.3.0/tests/test_openai_coverup_14.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_openai_coverup_15.py` & `coverup-0.3.0/tests/test_openai_coverup_15.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_openai_coverup_18.py` & `coverup-0.3.0/tests/test_openai_coverup_18.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_openai_coverup_19.py` & `coverup-0.3.0/tests/test_openai_coverup_19.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_openai_coverup_4.py` & `coverup-0.3.0/tests/test_openai_coverup_4.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_openai_coverup_5.py` & `coverup-0.3.0/tests/test_openai_coverup_5.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_openai_coverup_6.py` & `coverup-0.3.0/tests/test_openai_coverup_6.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_openai_coverup_8.py` & `coverup-0.3.0/tests/test_openai_coverup_8.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_openai_coverup_9.py` & `coverup-0.3.0/tests/test_openai_coverup_9.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_openai_second_coverup_1.py` & `coverup-0.3.0/tests/test_openai_second_coverup_1.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_openai_second_coverup_2.py` & `coverup-0.3.0/tests/test_openai_second_coverup_2.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_openai_second_coverup_4.py` & `coverup-0.3.0/tests/test_openai_second_coverup_4.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_openai_second_coverup_5.py` & `coverup-0.3.0/tests/test_openai_second_coverup_5.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_segment.py` & `coverup-0.3.0/tests/test_segment.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_testrunner.py` & `coverup-0.3.0/tests/test_testrunner.py`

 * *Files identical despite different names*

### Comparing `coverup-0.2.0/tests/test_utils.py` & `coverup-0.3.0/tests/test_utils.py`

 * *Files identical despite different names*

