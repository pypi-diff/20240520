# Comparing `tmp/hydrobot-0.6.1.tar.gz` & `tmp/hydrobot-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydrobot-0.6.1.tar", last modified: Fri May 17 03:59:47 2024, max compression
+gzip compressed data, was "hydrobot-0.6.2.tar", last modified: Mon May 20 01:58:05 2024, max compression
```

## Comparing `hydrobot-0.6.1.tar` & `hydrobot-0.6.2.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-17 03:59:47.736144 hydrobot-0.6.1/
--rw-r--r--   0 nic       (1000) nic       (1000)      292 2023-09-27 02:03:08.000000 hydrobot-0.6.1/.editorconfig
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-17 03:59:47.576144 hydrobot-0.6.1/.github/
--rw-r--r--   0 nic       (1000) nic       (1000)      333 2023-09-27 02:03:08.000000 hydrobot-0.6.1/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 nic       (1000) nic       (1000)     1207 2023-10-16 02:52:42.000000 hydrobot-0.6.1/.gitignore
--rw-r--r--   0 nic       (1000) nic       (1000)      514 2024-04-03 19:58:45.000000 hydrobot-0.6.1/.pre-commit-config.yaml
--rw-r--r--   0 nic       (1000) nic       (1000)     1068 2024-03-11 01:19:58.000000 hydrobot-0.6.1/.readthedocs.yaml
--rw-r--r--   0 nic       (1000) nic       (1000)      212 2023-10-16 02:52:42.000000 hydrobot-0.6.1/AUTHORS.rst
--rw-r--r--   0 nic       (1000) nic       (1000)     7309 2024-04-10 20:37:44.000000 hydrobot-0.6.1/CONTRIBUTING.rst
--rw-r--r--   0 nic       (1000) nic       (1000)     2559 2024-05-17 03:46:05.000000 hydrobot-0.6.1/HISTORY.rst
--rw-r--r--   0 nic       (1000) nic       (1000)     1610 2023-10-16 02:47:23.000000 hydrobot-0.6.1/LICENSE
--rw-r--r--   0 nic       (1000) nic       (1000)      298 2024-03-11 01:19:58.000000 hydrobot-0.6.1/MANIFEST.in
--rw-r--r--   0 nic       (1000) nic       (1000)     2336 2024-03-11 01:19:58.000000 hydrobot-0.6.1/Makefile
--rw-r--r--   0 nic       (1000) nic       (1000)     7090 2024-05-17 03:59:47.736144 hydrobot-0.6.1/PKG-INFO
--rw-r--r--   0 nic       (1000) nic       (1000)     5295 2024-05-17 03:57:33.000000 hydrobot-0.6.1/README.rst
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-17 03:59:47.586144 hydrobot-0.6.1/docs/
--rw-r--r--   0 nic       (1000) nic       (1000)      609 2023-11-02 03:51:37.000000 hydrobot-0.6.1/docs/Makefile
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-17 03:59:47.576144 hydrobot-0.6.1/docs/_build/
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-17 03:59:47.576144 hydrobot-0.6.1/docs/_build/html/
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-17 03:59:47.606144 hydrobot-0.6.1/docs/_build/html/_static/
--rw-r--r--   0 nic       (1000) nic       (1000)      286 2023-12-12 21:10:33.000000 hydrobot-0.6.1/docs/_build/html/_static/file.png
--rw-r--r--   0 nic       (1000) nic       (1000)       90 2023-12-12 21:10:33.000000 hydrobot-0.6.1/docs/_build/html/_static/minus.png
--rw-r--r--   0 nic       (1000) nic       (1000)       90 2023-12-12 21:10:33.000000 hydrobot-0.6.1/docs/_build/html/_static/plus.png
--rw-r--r--   0 nic       (1000) nic       (1000)       28 2023-09-27 02:03:08.000000 hydrobot-0.6.1/docs/authors.rst
--rwxr-xr-x   0 nic       (1000) nic       (1000)     5087 2024-04-10 21:52:59.000000 hydrobot-0.6.1/docs/conf.py
--rw-r--r--   0 nic       (1000) nic       (1000)       33 2023-09-27 02:03:08.000000 hydrobot-0.6.1/docs/contributing.rst
--rw-r--r--   0 nic       (1000) nic       (1000)       28 2023-09-27 02:03:08.000000 hydrobot-0.6.1/docs/history.rst
--rw-r--r--   0 nic       (1000) nic       (1000)     1190 2024-03-11 01:19:58.000000 hydrobot-0.6.1/docs/hydrobot.rst
--rw-r--r--   0 nic       (1000) nic       (1000)      305 2023-11-02 03:51:37.000000 hydrobot-0.6.1/docs/index.rst
--rw-r--r--   0 nic       (1000) nic       (1000)     1555 2024-03-11 01:19:58.000000 hydrobot-0.6.1/docs/installation.rst
--rw-r--r--   0 nic       (1000) nic       (1000)      806 2023-11-02 03:51:37.000000 hydrobot-0.6.1/docs/make.bat
--rw-r--r--   0 nic       (1000) nic       (1000)       61 2023-12-12 21:10:41.000000 hydrobot-0.6.1/docs/modules.rst
--rw-r--r--   0 nic       (1000) nic       (1000)       27 2023-09-27 02:03:08.000000 hydrobot-0.6.1/docs/readme.rst
--rw-r--r--   0 nic       (1000) nic       (1000)       71 2023-11-02 03:51:37.000000 hydrobot-0.6.1/docs/usage.rst
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-17 03:59:47.616144 hydrobot-0.6.1/hydrobot/
--rw-r--r--   0 nic       (1000) nic       (1000)      153 2024-05-17 03:57:33.000000 hydrobot-0.6.1/hydrobot/__init__.py
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-17 03:59:47.616144 hydrobot-0.6.1/hydrobot/config/
--rw-r--r--   0 nic       (1000) nic       (1000)       77 2024-05-17 03:46:05.000000 hydrobot-0.6.1/hydrobot/config/DissolvedOxygenQualityCodeEvaluator_QC_config.csv
--rw-r--r--   0 nic       (1000) nic       (1000)      105 2024-03-11 01:19:58.000000 hydrobot-0.6.1/hydrobot/config/QualityCodeEvaluator_QC_config.csv
--rw-r--r--   0 nic       (1000) nic       (1000)       55 2024-03-11 01:19:58.000000 hydrobot-0.6.1/hydrobot/config/TwoLevelQualityCodeEvaluator_QC_config.csv
--rw-r--r--   0 nic       (1000) nic       (1000)     7562 2024-05-17 02:21:16.000000 hydrobot-0.6.1/hydrobot/data_acquisition.py
--rw-r--r--   0 nic       (1000) nic       (1000)    11004 2024-05-17 03:46:05.000000 hydrobot-0.6.1/hydrobot/data_sources.py
--rw-r--r--   0 nic       (1000) nic       (1000)    31712 2024-05-14 03:54:49.000000 hydrobot-0.6.1/hydrobot/data_structure.py
--rw-r--r--   0 nic       (1000) nic       (1000)    14127 2024-05-17 03:46:05.000000 hydrobot-0.6.1/hydrobot/do_processor.py
--rw-r--r--   0 nic       (1000) nic       (1000)    21191 2024-05-17 03:55:04.000000 hydrobot-0.6.1/hydrobot/evaluator.py
--rw-r--r--   0 nic       (1000) nic       (1000)     8425 2024-05-17 03:24:49.000000 hydrobot-0.6.1/hydrobot/filters.py
--rw-r--r--   0 nic       (1000) nic       (1000)    19993 2024-05-14 02:24:50.000000 hydrobot-0.6.1/hydrobot/plotter.py
--rw-r--r--   0 nic       (1000) nic       (1000)    67823 2024-05-17 03:46:05.000000 hydrobot-0.6.1/hydrobot/processor.py
--rw-r--r--   0 nic       (1000) nic       (1000)    10239 2024-05-17 03:46:05.000000 hydrobot-0.6.1/hydrobot/utils.py
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-17 03:59:47.736144 hydrobot-0.6.1/hydrobot.egg-info/
--rw-r--r--   0 nic       (1000) nic       (1000)     7090 2024-05-17 03:59:47.000000 hydrobot-0.6.1/hydrobot.egg-info/PKG-INFO
--rw-r--r--   0 nic       (1000) nic       (1000)     2708 2024-05-17 03:59:47.000000 hydrobot-0.6.1/hydrobot.egg-info/SOURCES.txt
--rw-r--r--   0 nic       (1000) nic       (1000)        1 2024-05-17 03:59:47.000000 hydrobot-0.6.1/hydrobot.egg-info/dependency_links.txt
--rw-r--r--   0 nic       (1000) nic       (1000)      343 2024-05-17 03:59:47.000000 hydrobot-0.6.1/hydrobot.egg-info/requires.txt
--rw-r--r--   0 nic       (1000) nic       (1000)        9 2024-05-17 03:59:47.000000 hydrobot-0.6.1/hydrobot.egg-info/top_level.txt
--rw-r--r--   0 nic       (1000) nic       (1000)      422 2024-03-11 01:19:58.000000 hydrobot-0.6.1/old_setup.cfg
--rw-r--r--   0 nic       (1000) nic       (1000)     1571 2024-03-11 01:19:58.000000 hydrobot-0.6.1/old_setup.py
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-17 03:59:47.616144 hydrobot-0.6.1/prototypes/
--rw-r--r--   0 nic       (1000) nic       (1000)     4257 2024-04-08 04:10:48.000000 hydrobot-0.6.1/prototypes/Class_script.py
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-17 03:59:47.706144 hydrobot-0.6.1/prototypes/example_script/
--rw-r--r--   0 nic       (1000) nic       (1000)       22 2024-05-14 02:24:50.000000 hydrobot-0.6.1/prototypes/example_script/.gitignore
--rwxr-xr-x   0 nic       (1000) nic       (1000)   450560 2024-05-03 01:38:55.000000 hydrobot-0.6.1/prototypes/example_script/40X_XXX_WaterTemperature.accdb
--rwxr-xr-x   0 nic       (1000) nic       (1000)  2998240 2024-05-14 03:54:49.000000 hydrobot-0.6.1/prototypes/example_script/40X_XXX_WaterTemperature.hts
--rw-r--r--   0 nic       (1000) nic       (1000)     9598 2024-05-17 02:46:12.000000 hydrobot-0.6.1/prototypes/example_script/AP_CheckData.R
--rw-r--r--   0 nic       (1000) nic       (1000)      832 2024-05-14 02:24:50.000000 hydrobot-0.6.1/prototypes/example_script/AP_config.yaml
--rw-r--r--   0 nic       (1000) nic       (1000)    10505 2024-05-14 02:24:50.000000 hydrobot-0.6.1/prototypes/example_script/WaterTemp_CheckData.R
--rw-r--r--   0 nic       (1000) nic       (1000)     1380 2024-05-17 03:57:33.000000 hydrobot-0.6.1/prototypes/example_script/config.yaml
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-17 03:59:47.706144 hydrobot-0.6.1/prototypes/example_script/diss_ox/
--rw-r--r--   0 nic       (1000) nic       (1000)    10348 2024-05-17 03:46:05.000000 hydrobot-0.6.1/prototypes/example_script/diss_ox/DO_CheckData.R
--rw-r--r--   0 nic       (1000) nic       (1000)     1318 2024-05-17 03:46:05.000000 hydrobot-0.6.1/prototypes/example_script/diss_ox/DO_config.yaml
--rw-r--r--   0 nic       (1000) nic       (1000)     5011 2024-05-17 03:46:05.000000 hydrobot-0.6.1/prototypes/example_script/diss_ox/do_script.py
--rw-r--r--   0 nic       (1000) nic       (1000)     4781 2024-05-17 03:57:33.000000 hydrobot-0.6.1/prototypes/example_script/script.py
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-17 03:59:47.706144 hydrobot-0.6.1/prototypes/output_dump/
--rw-r--r--   0 nic       (1000) nic       (1000)      144 2023-11-02 01:24:43.000000 hydrobot-0.6.1/prototypes/output_dump/.gitignore
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-17 03:59:47.706144 hydrobot-0.6.1/prototypes/py_scripts/
--rw-r--r--   0 nic       (1000) nic       (1000)     1515 2024-03-11 01:19:58.000000 hydrobot-0.6.1/prototypes/py_scripts/atmospheric_spike_removal.py
--rw-r--r--   0 nic       (1000) nic       (1000)     1051 2024-03-11 01:19:58.000000 hydrobot-0.6.1/prototypes/py_scripts/example_plot_script.py
--rw-r--r--   0 nic       (1000) nic       (1000)     1581 2024-04-03 02:25:29.000000 hydrobot-0.6.1/prototypes/py_scripts/gap_finder.py
--rw-r--r--   0 nic       (1000) nic       (1000)     1319 2024-03-11 01:19:58.000000 hydrobot-0.6.1/prototypes/py_scripts/new_ws_plot_with_check_data.py
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-17 03:59:47.706144 hydrobot-0.6.1/prototypes/py_scripts/output_dump/
--rw-r--r--   0 nic       (1000) nic       (1000)      144 2023-11-02 01:24:43.000000 hydrobot-0.6.1/prototypes/py_scripts/output_dump/.gitignore
--rw-r--r--   0 nic       (1000) nic       (1000)     1001 2024-03-11 01:19:58.000000 hydrobot-0.6.1/prototypes/py_scripts/plot_with_check_data.py
--rw-r--r--   0 nic       (1000) nic       (1000)     4222 2024-03-11 01:19:58.000000 hydrobot-0.6.1/prototypes/py_scripts/process_script.py
--rw-r--r--   0 nic       (1000) nic       (1000)      933 2023-12-03 22:14:39.000000 hydrobot-0.6.1/prototypes/py_scripts/spike_removal_util.py
--rw-r--r--   0 nic       (1000) nic       (1000)     3509 2024-03-11 01:19:58.000000 hydrobot-0.6.1/prototypes/py_scripts/stage_full_process.py
--rw-r--r--   0 nic       (1000) nic       (1000)     3627 2024-03-11 01:19:58.000000 hydrobot-0.6.1/prototypes/py_scripts/water_temp_full_process.py
--rw-r--r--   0 nic       (1000) nic       (1000)     1927 2023-11-02 02:57:00.000000 hydrobot-0.6.1/prototypes/py_scripts/water_temp_spike_removal.py
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-17 03:59:47.706144 hydrobot-0.6.1/prototypes/script_dump/
--rw-r--r--   0 nic       (1000) nic       (1000)      144 2024-03-11 01:19:58.000000 hydrobot-0.6.1/prototypes/script_dump/.gitignore
--rw-r--r--   0 nic       (1000) nic       (1000)     1419 2024-03-11 01:19:58.000000 hydrobot-0.6.1/prototypes/site_list_reader.py
--rw-r--r--   0 nic       (1000) nic       (1000)      443 2024-03-11 01:19:58.000000 hydrobot-0.6.1/prototypes/site_parameters.json
--rw-r--r--   0 nic       (1000) nic       (1000)     3507 2024-05-17 03:57:33.000000 hydrobot-0.6.1/pyproject.toml
--rw-r--r--   0 nic       (1000) nic       (1000)     3430 2024-05-03 01:38:55.000000 hydrobot-0.6.1/requirements_dev.txt
--rw-r--r--   0 nic       (1000) nic       (1000)      506 2024-03-11 01:19:58.000000 hydrobot-0.6.1/requirements_test.txt
--rw-r--r--   0 nic       (1000) nic       (1000)       38 2024-05-17 03:59:47.736144 hydrobot-0.6.1/setup.cfg
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-17 03:59:47.736144 hydrobot-0.6.1/tests/
--rw-r--r--   0 nic       (1000) nic       (1000)    53248 2024-02-26 00:40:14.000000 hydrobot-0.6.1/tests/.coverage
--rw-r--r--   0 nic       (1000) nic       (1000)       38 2023-11-02 02:57:00.000000 hydrobot-0.6.1/tests/__init__.py
--rw-r--r--   0 nic       (1000) nic       (1000)     1017 2024-04-10 21:52:59.000000 hydrobot-0.6.1/tests/conftest.py
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-17 03:59:47.736144 hydrobot-0.6.1/tests/test_data/
--rw-r--r--   0 nic       (1000) nic       (1000)      245 2024-04-10 21:52:59.000000 hydrobot-0.6.1/tests/test_data/site_list_response.xml
--rw-r--r--   0 nic       (1000) nic       (1000)      728 2024-05-17 03:46:05.000000 hydrobot-0.6.1/tests/test_data/test_config.yaml
--rw-r--r--   0 nic       (1000) nic       (1000)    74114 2024-05-14 03:24:14.000000 hydrobot-0.6.1/tests/test_data/xml_test_data_file.xml
--rw-r--r--   0 nic       (1000) nic       (1000)     6584 2024-05-03 01:38:55.000000 hydrobot-0.6.1/tests/test_data/xml_test_data_no_check.xml
--rw-r--r--   0 nic       (1000) nic       (1000)    12469 2024-05-03 01:38:55.000000 hydrobot-0.6.1/tests/test_data/xml_test_data_no_qual.xml
--rw-r--r--   0 nic       (1000) nic       (1000)     3624 2024-05-17 03:46:05.000000 hydrobot-0.6.1/tests/test_data_sources.py
--rw-r--r--   0 nic       (1000) nic       (1000)     9736 2024-05-03 01:38:55.000000 hydrobot-0.6.1/tests/test_data_structure.py
--rw-r--r--   0 nic       (1000) nic       (1000)    19438 2024-05-17 03:46:05.000000 hydrobot-0.6.1/tests/test_evaluator.py
--rw-r--r--   0 nic       (1000) nic       (1000)    11873 2024-05-14 02:24:50.000000 hydrobot-0.6.1/tests/test_filters.py
--rw-r--r--   0 nic       (1000) nic       (1000)    48996 2024-05-17 03:46:05.000000 hydrobot-0.6.1/tests/test_processor.py
--rw-r--r--   0 nic       (1000) nic       (1000)     4525 2024-05-17 03:46:05.000000 hydrobot-0.6.1/tests/test_utils.py
--rw-r--r--   0 nic       (1000) nic       (1000)    27025 2024-05-17 03:46:05.000000 hydrobot-0.6.1/tests/test_web_integration.py
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-20 01:58:05.305781 hydrobot-0.6.2/
+-rw-r--r--   0 nic       (1000) nic       (1000)      292 2023-09-27 02:03:08.000000 hydrobot-0.6.2/.editorconfig
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-20 01:58:05.285781 hydrobot-0.6.2/.github/
+-rw-r--r--   0 nic       (1000) nic       (1000)      333 2023-09-27 02:03:08.000000 hydrobot-0.6.2/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 nic       (1000) nic       (1000)     1207 2023-10-16 02:52:42.000000 hydrobot-0.6.2/.gitignore
+-rw-r--r--   0 nic       (1000) nic       (1000)      514 2024-04-03 19:58:45.000000 hydrobot-0.6.2/.pre-commit-config.yaml
+-rw-r--r--   0 nic       (1000) nic       (1000)     1068 2024-03-11 01:19:58.000000 hydrobot-0.6.2/.readthedocs.yaml
+-rw-r--r--   0 nic       (1000) nic       (1000)      212 2023-10-16 02:52:42.000000 hydrobot-0.6.2/AUTHORS.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)     7309 2024-04-10 20:37:44.000000 hydrobot-0.6.2/CONTRIBUTING.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)     2676 2024-05-20 01:51:34.000000 hydrobot-0.6.2/HISTORY.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)     1610 2023-10-16 02:47:23.000000 hydrobot-0.6.2/LICENSE
+-rw-r--r--   0 nic       (1000) nic       (1000)      298 2024-03-11 01:19:58.000000 hydrobot-0.6.2/MANIFEST.in
+-rw-r--r--   0 nic       (1000) nic       (1000)     2336 2024-03-11 01:19:58.000000 hydrobot-0.6.2/Makefile
+-rw-r--r--   0 nic       (1000) nic       (1000)     7090 2024-05-20 01:58:05.305781 hydrobot-0.6.2/PKG-INFO
+-rw-r--r--   0 nic       (1000) nic       (1000)     5295 2024-05-20 01:56:25.000000 hydrobot-0.6.2/README.rst
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-20 01:58:05.285781 hydrobot-0.6.2/docs/
+-rw-r--r--   0 nic       (1000) nic       (1000)      609 2023-11-02 03:51:37.000000 hydrobot-0.6.2/docs/Makefile
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-20 01:58:05.275781 hydrobot-0.6.2/docs/_build/
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-20 01:58:05.275781 hydrobot-0.6.2/docs/_build/html/
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-20 01:58:05.285781 hydrobot-0.6.2/docs/_build/html/_static/
+-rw-r--r--   0 nic       (1000) nic       (1000)      286 2023-12-12 21:10:33.000000 hydrobot-0.6.2/docs/_build/html/_static/file.png
+-rw-r--r--   0 nic       (1000) nic       (1000)       90 2023-12-12 21:10:33.000000 hydrobot-0.6.2/docs/_build/html/_static/minus.png
+-rw-r--r--   0 nic       (1000) nic       (1000)       90 2023-12-12 21:10:33.000000 hydrobot-0.6.2/docs/_build/html/_static/plus.png
+-rw-r--r--   0 nic       (1000) nic       (1000)       28 2023-09-27 02:03:08.000000 hydrobot-0.6.2/docs/authors.rst
+-rwxr-xr-x   0 nic       (1000) nic       (1000)     5087 2024-04-10 21:52:59.000000 hydrobot-0.6.2/docs/conf.py
+-rw-r--r--   0 nic       (1000) nic       (1000)       33 2023-09-27 02:03:08.000000 hydrobot-0.6.2/docs/contributing.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)       28 2023-09-27 02:03:08.000000 hydrobot-0.6.2/docs/history.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)     1190 2024-03-11 01:19:58.000000 hydrobot-0.6.2/docs/hydrobot.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)      305 2023-11-02 03:51:37.000000 hydrobot-0.6.2/docs/index.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)     1555 2024-03-11 01:19:58.000000 hydrobot-0.6.2/docs/installation.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)      806 2023-11-02 03:51:37.000000 hydrobot-0.6.2/docs/make.bat
+-rw-r--r--   0 nic       (1000) nic       (1000)       61 2023-12-12 21:10:41.000000 hydrobot-0.6.2/docs/modules.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)       27 2023-09-27 02:03:08.000000 hydrobot-0.6.2/docs/readme.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)       71 2023-11-02 03:51:37.000000 hydrobot-0.6.2/docs/usage.rst
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-20 01:58:05.285781 hydrobot-0.6.2/hydrobot/
+-rw-r--r--   0 nic       (1000) nic       (1000)      153 2024-05-20 01:56:25.000000 hydrobot-0.6.2/hydrobot/__init__.py
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-20 01:58:05.295781 hydrobot-0.6.2/hydrobot/config/
+-rw-r--r--   0 nic       (1000) nic       (1000)       77 2024-05-17 03:46:05.000000 hydrobot-0.6.2/hydrobot/config/DissolvedOxygenQualityCodeEvaluator_QC_config.csv
+-rw-r--r--   0 nic       (1000) nic       (1000)      105 2024-03-11 01:19:58.000000 hydrobot-0.6.2/hydrobot/config/QualityCodeEvaluator_QC_config.csv
+-rw-r--r--   0 nic       (1000) nic       (1000)       55 2024-03-11 01:19:58.000000 hydrobot-0.6.2/hydrobot/config/TwoLevelQualityCodeEvaluator_QC_config.csv
+-rw-r--r--   0 nic       (1000) nic       (1000)     7562 2024-05-17 02:21:16.000000 hydrobot-0.6.2/hydrobot/data_acquisition.py
+-rw-r--r--   0 nic       (1000) nic       (1000)    11004 2024-05-17 03:46:05.000000 hydrobot-0.6.2/hydrobot/data_sources.py
+-rw-r--r--   0 nic       (1000) nic       (1000)    31712 2024-05-14 03:54:49.000000 hydrobot-0.6.2/hydrobot/data_structure.py
+-rw-r--r--   0 nic       (1000) nic       (1000)    14210 2024-05-20 01:51:34.000000 hydrobot-0.6.2/hydrobot/do_processor.py
+-rw-r--r--   0 nic       (1000) nic       (1000)    21191 2024-05-17 03:55:04.000000 hydrobot-0.6.2/hydrobot/evaluator.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     8425 2024-05-17 03:24:49.000000 hydrobot-0.6.2/hydrobot/filters.py
+-rw-r--r--   0 nic       (1000) nic       (1000)    19993 2024-05-14 02:24:50.000000 hydrobot-0.6.2/hydrobot/plotter.py
+-rw-r--r--   0 nic       (1000) nic       (1000)    67823 2024-05-17 03:46:05.000000 hydrobot-0.6.2/hydrobot/processor.py
+-rw-r--r--   0 nic       (1000) nic       (1000)    10239 2024-05-17 03:46:05.000000 hydrobot-0.6.2/hydrobot/utils.py
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-20 01:58:05.305781 hydrobot-0.6.2/hydrobot.egg-info/
+-rw-r--r--   0 nic       (1000) nic       (1000)     7090 2024-05-20 01:58:05.000000 hydrobot-0.6.2/hydrobot.egg-info/PKG-INFO
+-rw-r--r--   0 nic       (1000) nic       (1000)     2708 2024-05-20 01:58:05.000000 hydrobot-0.6.2/hydrobot.egg-info/SOURCES.txt
+-rw-r--r--   0 nic       (1000) nic       (1000)        1 2024-05-20 01:58:05.000000 hydrobot-0.6.2/hydrobot.egg-info/dependency_links.txt
+-rw-r--r--   0 nic       (1000) nic       (1000)      343 2024-05-20 01:58:05.000000 hydrobot-0.6.2/hydrobot.egg-info/requires.txt
+-rw-r--r--   0 nic       (1000) nic       (1000)        9 2024-05-20 01:58:05.000000 hydrobot-0.6.2/hydrobot.egg-info/top_level.txt
+-rw-r--r--   0 nic       (1000) nic       (1000)      422 2024-03-11 01:19:58.000000 hydrobot-0.6.2/old_setup.cfg
+-rw-r--r--   0 nic       (1000) nic       (1000)     1571 2024-03-11 01:19:58.000000 hydrobot-0.6.2/old_setup.py
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-20 01:58:05.295781 hydrobot-0.6.2/prototypes/
+-rw-r--r--   0 nic       (1000) nic       (1000)     4257 2024-04-08 04:10:48.000000 hydrobot-0.6.2/prototypes/Class_script.py
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-20 01:58:05.295781 hydrobot-0.6.2/prototypes/example_script/
+-rw-r--r--   0 nic       (1000) nic       (1000)       22 2024-05-14 02:24:50.000000 hydrobot-0.6.2/prototypes/example_script/.gitignore
+-rwxr-xr-x   0 nic       (1000) nic       (1000)   450560 2024-05-03 01:38:55.000000 hydrobot-0.6.2/prototypes/example_script/40X_XXX_WaterTemperature.accdb
+-rwxr-xr-x   0 nic       (1000) nic       (1000)  2998240 2024-05-14 03:54:49.000000 hydrobot-0.6.2/prototypes/example_script/40X_XXX_WaterTemperature.hts
+-rw-r--r--   0 nic       (1000) nic       (1000)     9598 2024-05-17 02:46:12.000000 hydrobot-0.6.2/prototypes/example_script/AP_CheckData.R
+-rw-r--r--   0 nic       (1000) nic       (1000)      832 2024-05-14 02:24:50.000000 hydrobot-0.6.2/prototypes/example_script/AP_config.yaml
+-rw-r--r--   0 nic       (1000) nic       (1000)    10505 2024-05-14 02:24:50.000000 hydrobot-0.6.2/prototypes/example_script/WaterTemp_CheckData.R
+-rw-r--r--   0 nic       (1000) nic       (1000)     1380 2024-05-20 01:56:25.000000 hydrobot-0.6.2/prototypes/example_script/config.yaml
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-20 01:58:05.295781 hydrobot-0.6.2/prototypes/example_script/diss_ox/
+-rw-r--r--   0 nic       (1000) nic       (1000)    10348 2024-05-17 03:46:05.000000 hydrobot-0.6.2/prototypes/example_script/diss_ox/DO_CheckData.R
+-rw-r--r--   0 nic       (1000) nic       (1000)     1328 2024-05-20 01:51:34.000000 hydrobot-0.6.2/prototypes/example_script/diss_ox/DO_config.yaml
+-rw-r--r--   0 nic       (1000) nic       (1000)     5011 2024-05-17 03:46:05.000000 hydrobot-0.6.2/prototypes/example_script/diss_ox/do_script.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     4781 2024-05-20 01:56:25.000000 hydrobot-0.6.2/prototypes/example_script/script.py
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-20 01:58:05.295781 hydrobot-0.6.2/prototypes/output_dump/
+-rw-r--r--   0 nic       (1000) nic       (1000)      144 2023-11-02 01:24:43.000000 hydrobot-0.6.2/prototypes/output_dump/.gitignore
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-20 01:58:05.295781 hydrobot-0.6.2/prototypes/py_scripts/
+-rw-r--r--   0 nic       (1000) nic       (1000)     1515 2024-03-11 01:19:58.000000 hydrobot-0.6.2/prototypes/py_scripts/atmospheric_spike_removal.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     1051 2024-03-11 01:19:58.000000 hydrobot-0.6.2/prototypes/py_scripts/example_plot_script.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     1581 2024-04-03 02:25:29.000000 hydrobot-0.6.2/prototypes/py_scripts/gap_finder.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     1319 2024-03-11 01:19:58.000000 hydrobot-0.6.2/prototypes/py_scripts/new_ws_plot_with_check_data.py
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-20 01:58:05.295781 hydrobot-0.6.2/prototypes/py_scripts/output_dump/
+-rw-r--r--   0 nic       (1000) nic       (1000)      144 2023-11-02 01:24:43.000000 hydrobot-0.6.2/prototypes/py_scripts/output_dump/.gitignore
+-rw-r--r--   0 nic       (1000) nic       (1000)     1001 2024-03-11 01:19:58.000000 hydrobot-0.6.2/prototypes/py_scripts/plot_with_check_data.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     4222 2024-03-11 01:19:58.000000 hydrobot-0.6.2/prototypes/py_scripts/process_script.py
+-rw-r--r--   0 nic       (1000) nic       (1000)      933 2023-12-03 22:14:39.000000 hydrobot-0.6.2/prototypes/py_scripts/spike_removal_util.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     3509 2024-03-11 01:19:58.000000 hydrobot-0.6.2/prototypes/py_scripts/stage_full_process.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     3627 2024-03-11 01:19:58.000000 hydrobot-0.6.2/prototypes/py_scripts/water_temp_full_process.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     1927 2023-11-02 02:57:00.000000 hydrobot-0.6.2/prototypes/py_scripts/water_temp_spike_removal.py
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-20 01:58:05.295781 hydrobot-0.6.2/prototypes/script_dump/
+-rw-r--r--   0 nic       (1000) nic       (1000)      144 2024-03-11 01:19:58.000000 hydrobot-0.6.2/prototypes/script_dump/.gitignore
+-rw-r--r--   0 nic       (1000) nic       (1000)     1419 2024-03-11 01:19:58.000000 hydrobot-0.6.2/prototypes/site_list_reader.py
+-rw-r--r--   0 nic       (1000) nic       (1000)      443 2024-03-11 01:19:58.000000 hydrobot-0.6.2/prototypes/site_parameters.json
+-rw-r--r--   0 nic       (1000) nic       (1000)     3507 2024-05-20 01:56:25.000000 hydrobot-0.6.2/pyproject.toml
+-rw-r--r--   0 nic       (1000) nic       (1000)     3430 2024-05-03 01:38:55.000000 hydrobot-0.6.2/requirements_dev.txt
+-rw-r--r--   0 nic       (1000) nic       (1000)      506 2024-03-11 01:19:58.000000 hydrobot-0.6.2/requirements_test.txt
+-rw-r--r--   0 nic       (1000) nic       (1000)       38 2024-05-20 01:58:05.305781 hydrobot-0.6.2/setup.cfg
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-20 01:58:05.305781 hydrobot-0.6.2/tests/
+-rw-r--r--   0 nic       (1000) nic       (1000)    53248 2024-02-26 00:40:14.000000 hydrobot-0.6.2/tests/.coverage
+-rw-r--r--   0 nic       (1000) nic       (1000)       38 2023-11-02 02:57:00.000000 hydrobot-0.6.2/tests/__init__.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     1017 2024-04-10 21:52:59.000000 hydrobot-0.6.2/tests/conftest.py
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-20 01:58:05.305781 hydrobot-0.6.2/tests/test_data/
+-rw-r--r--   0 nic       (1000) nic       (1000)      245 2024-04-10 21:52:59.000000 hydrobot-0.6.2/tests/test_data/site_list_response.xml
+-rw-r--r--   0 nic       (1000) nic       (1000)      728 2024-05-17 03:46:05.000000 hydrobot-0.6.2/tests/test_data/test_config.yaml
+-rw-r--r--   0 nic       (1000) nic       (1000)    74114 2024-05-14 03:24:14.000000 hydrobot-0.6.2/tests/test_data/xml_test_data_file.xml
+-rw-r--r--   0 nic       (1000) nic       (1000)     6584 2024-05-03 01:38:55.000000 hydrobot-0.6.2/tests/test_data/xml_test_data_no_check.xml
+-rw-r--r--   0 nic       (1000) nic       (1000)    12469 2024-05-03 01:38:55.000000 hydrobot-0.6.2/tests/test_data/xml_test_data_no_qual.xml
+-rw-r--r--   0 nic       (1000) nic       (1000)     3624 2024-05-17 03:46:05.000000 hydrobot-0.6.2/tests/test_data_sources.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     9736 2024-05-03 01:38:55.000000 hydrobot-0.6.2/tests/test_data_structure.py
+-rw-r--r--   0 nic       (1000) nic       (1000)    19438 2024-05-17 03:46:05.000000 hydrobot-0.6.2/tests/test_evaluator.py
+-rw-r--r--   0 nic       (1000) nic       (1000)    11873 2024-05-14 02:24:50.000000 hydrobot-0.6.2/tests/test_filters.py
+-rw-r--r--   0 nic       (1000) nic       (1000)    48996 2024-05-17 03:46:05.000000 hydrobot-0.6.2/tests/test_processor.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     4525 2024-05-17 03:46:05.000000 hydrobot-0.6.2/tests/test_utils.py
+-rw-r--r--   0 nic       (1000) nic       (1000)    27025 2024-05-17 03:46:05.000000 hydrobot-0.6.2/tests/test_web_integration.py
```

### Comparing `hydrobot-0.6.1/.gitignore` & `hydrobot-0.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/.pre-commit-config.yaml` & `hydrobot-0.6.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/.readthedocs.yaml` & `hydrobot-0.6.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/CONTRIBUTING.rst` & `hydrobot-0.6.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/HISTORY.rst` & `hydrobot-0.6.2/HISTORY.rst`

 * *Files 6% similar despite different names*

```diff
@@ -94,7 +94,12 @@
 * DO semi-supported, but things are a little hairy rn
 * Gonna officially support DO next minor release with more testing
 * DO evaluator supported
 * 100% 500 qc cap supported
 * Support WT + AP QCs
 * AP VM adjustment supported
 * Nic promises the check data hilltop import thing is fixed this time
+
+0.6.2 (2024-05-20)
+----------------------------------
+
+* Fixed bug that meant that different data sources would not
```

### Comparing `hydrobot-0.6.1/LICENSE` & `hydrobot-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/Makefile` & `hydrobot-0.6.2/Makefile`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/PKG-INFO` & `hydrobot-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrobot
-Version: 0.6.1
+Version: 0.6.2
 Summary: A suite of processing tools for Hilltop hydrological data.
 Author-email: Nic Mostert <nicolas.mostert@horizons.govt.nz>, Sam Irvine <sam.irvine@horizons.govt.nz>
 License: GNU General Public License v3
 Project-URL: Homepage, https://github.com/HorizonsRC/hydrobot
 Project-URL: Issues, https://github.com/HorizonsRC/hydrobot/issues
 Project-URL: Documentation, https://hydrobot.readthedocs.io
 Project-URL: Package, https://pypi.org/project/hydrobot
@@ -82,27 +82,27 @@
   * Visualizing check points from various sources.
 
 Usage (Alpha)
 -------------
 
 The Alpha release of Hydrobot supports a "hybrid" workflow. This means that some external tools are still required to do a full processing. Importantly, the hybrid workflow relies on some R scripts to obtain check data from sources other than Hilltop. Further processing using Hilltop manager is also supported.
 
-NOTE: Hydrobot 0.6.1 supports only Water Temperature processing at the moment, but more measurements will be supported in patches as the processing progresses.
+NOTE: Hydrobot 0.6.2 supports only Water Temperature processing at the moment, but more measurements will be supported in patches as the processing progresses.
 
 Initial Setup (Repeat for each release)
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 #. Install a Python 3.11 interpreter. Note that 3.12 is not supported just yet.
-#. In your favourite shell, create a new virtual environment using this python interpreter and name it "hydrobot0.6.1". It's important that this is stored somewhere locally. I suggest creating a folder for virtual environments in your home folder::
+#. In your favourite shell, create a new virtual environment using this python interpreter and name it "hydrobot0.6.2". It's important that this is stored somewhere locally. I suggest creating a folder for virtual environments in your home folder::
 
-    python -m venv path/to/venv/hydrobot0.6.1/
+    python -m venv path/to/venv/hydrobot0.6.2/
 
 #. Activate this virtual environment. In powershell this should be something like::
 
-    ./path/to/venv/hydrobot0.6.1/Scripts/Activate.ps1
+    ./path/to/venv/hydrobot0.6.2/Scripts/Activate.ps1
 
 #. If you're sure your venv is active (ensure with `which python` and confirm that you're using the interpreter in your venv folder), install the latest version of Hydrobot using pip::
 
     pip install hydrobot
 
 #. Record which version of dependencies you have installed. The following pip freeze records which dependencies are
 installed by the hydrobot install process for if auditing/reprocessing is required later::
@@ -117,17 +117,17 @@
 Processing Steps
 ^^^^^^^^^^^^^^^^
 
 #. Open Logsheet Loader. Fill it as normal, and note the start date of your processing period (i.e. end date of the previous period).
 #. Navigate to the data source and site folder, and create your processing folder.
 #. Copy all the processing files in this folder into your processing folder::
 
-    \\ares\Environmental Data Validation\Water Temperature\Documents\Hydrobot_0.6.1_Files\
+    \\ares\Environmental Data Validation\Water Temperature\Documents\Hydrobot_0.6.2_Files\
 
-    //ares/Environmental\ Data\ Validation/Water\ Temperature/Documents/Hydrobot_0.6.1_Files/
+    //ares/Environmental\ Data\ Validation/Water\ Temperature/Documents/Hydrobot_0.6.2_Files/
 
 #. In your processing folder, open the `config.yaml` file and change the fields `site`, `from_date`, `to_date`, `analyst_name`. Feel free to mess with the other values once you get the hang of it. No one will die.
 
 #. Run the R script. I'm not an R guy so I'm not sure how to do this other than to open it in R studio, highlighting all the code, and hitting `Ctrl+Enter`. This should create a bunch of `.csv` files containing the check data from various sources. This is a good reasource for perusal during processing, but will be imbibed by hydrobot to for QC encoding.
 
 #. Make sure your virtual environment is set up and active. Ensure with `which python` and confirm that your python interpreter is running from your venv folder.
```

### Comparing `hydrobot-0.6.1/README.rst` & `hydrobot-0.6.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -39,27 +39,27 @@
   * Visualizing check points from various sources.
 
 Usage (Alpha)
 -------------
 
 The Alpha release of Hydrobot supports a "hybrid" workflow. This means that some external tools are still required to do a full processing. Importantly, the hybrid workflow relies on some R scripts to obtain check data from sources other than Hilltop. Further processing using Hilltop manager is also supported.
 
-NOTE: Hydrobot 0.6.1 supports only Water Temperature processing at the moment, but more measurements will be supported in patches as the processing progresses.
+NOTE: Hydrobot 0.6.2 supports only Water Temperature processing at the moment, but more measurements will be supported in patches as the processing progresses.
 
 Initial Setup (Repeat for each release)
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 #. Install a Python 3.11 interpreter. Note that 3.12 is not supported just yet.
-#. In your favourite shell, create a new virtual environment using this python interpreter and name it "hydrobot0.6.1". It's important that this is stored somewhere locally. I suggest creating a folder for virtual environments in your home folder::
+#. In your favourite shell, create a new virtual environment using this python interpreter and name it "hydrobot0.6.2". It's important that this is stored somewhere locally. I suggest creating a folder for virtual environments in your home folder::
 
-    python -m venv path/to/venv/hydrobot0.6.1/
+    python -m venv path/to/venv/hydrobot0.6.2/
 
 #. Activate this virtual environment. In powershell this should be something like::
 
-    ./path/to/venv/hydrobot0.6.1/Scripts/Activate.ps1
+    ./path/to/venv/hydrobot0.6.2/Scripts/Activate.ps1
 
 #. If you're sure your venv is active (ensure with `which python` and confirm that you're using the interpreter in your venv folder), install the latest version of Hydrobot using pip::
 
     pip install hydrobot
 
 #. Record which version of dependencies you have installed. The following pip freeze records which dependencies are
 installed by the hydrobot install process for if auditing/reprocessing is required later::
@@ -74,17 +74,17 @@
 Processing Steps
 ^^^^^^^^^^^^^^^^
 
 #. Open Logsheet Loader. Fill it as normal, and note the start date of your processing period (i.e. end date of the previous period).
 #. Navigate to the data source and site folder, and create your processing folder.
 #. Copy all the processing files in this folder into your processing folder::
 
-    \\ares\Environmental Data Validation\Water Temperature\Documents\Hydrobot_0.6.1_Files\
+    \\ares\Environmental Data Validation\Water Temperature\Documents\Hydrobot_0.6.2_Files\
 
-    //ares/Environmental\ Data\ Validation/Water\ Temperature/Documents/Hydrobot_0.6.1_Files/
+    //ares/Environmental\ Data\ Validation/Water\ Temperature/Documents/Hydrobot_0.6.2_Files/
 
 #. In your processing folder, open the `config.yaml` file and change the fields `site`, `from_date`, `to_date`, `analyst_name`. Feel free to mess with the other values once you get the hang of it. No one will die.
 
 #. Run the R script. I'm not an R guy so I'm not sure how to do this other than to open it in R studio, highlighting all the code, and hitting `Ctrl+Enter`. This should create a bunch of `.csv` files containing the check data from various sources. This is a good reasource for perusal during processing, but will be imbibed by hydrobot to for QC encoding.
 
 #. Make sure your virtual environment is set up and active. Ensure with `which python` and confirm that your python interpreter is running from your venv folder.
```

### Comparing `hydrobot-0.6.1/docs/Makefile` & `hydrobot-0.6.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/docs/conf.py` & `hydrobot-0.6.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/docs/hydrobot.rst` & `hydrobot-0.6.2/docs/hydrobot.rst`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/docs/installation.rst` & `hydrobot-0.6.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/docs/make.bat` & `hydrobot-0.6.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/hydrobot/data_acquisition.py` & `hydrobot-0.6.2/hydrobot/data_acquisition.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/hydrobot/data_sources.py` & `hydrobot-0.6.2/hydrobot/data_sources.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/hydrobot/data_structure.py` & `hydrobot-0.6.2/hydrobot/data_structure.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/hydrobot/do_processor.py` & `hydrobot-0.6.2/hydrobot/do_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,17 @@
             raise ValueError(
                 f"Atmospheric Pressure site '{site}' not found for both base_url and hts combos."
                 f"Available sites in {atmospheric_pressure_hts} are: "
                 f"{[s for s in ap_hilltop.available_sites]}"
             )
 
         # Atmospheric Pressure
-        available_ap_measurements = ap_hilltop.get_measurement_list(site)
+        available_ap_measurements = ap_hilltop.get_measurement_list(
+            atmospheric_pressure_site
+        )
         self.atmospheric_pressure_measurement_name = (
             atmospheric_pressure_measurement_name
         )
         matches = re.search(
             r"([^\[\n]+)(\[(.+)\])?", atmospheric_pressure_measurement_name
         )
 
@@ -110,15 +112,17 @@
                 f"'{atmospheric_pressure_measurement_name}' not found at"
                 f" site '{site}'. "
                 "Available measurements are "
                 f"{list(available_ap_measurements.MeasurementName)}"
             )
 
         # Water Temperature
-        available_wt_measurements = wt_hilltop.get_measurement_list(site)
+        available_wt_measurements = wt_hilltop.get_measurement_list(
+            water_temperature_site
+        )
         self.water_temperature_measurement_name = water_temperature_measurement_name
         matches = re.search(
             r"([^\[\n]+)(\[(.+)\])?", water_temperature_measurement_name
         )
 
         if matches is not None:
             self.wt_item_name = matches.groups()[0].strip(" ")
```

### Comparing `hydrobot-0.6.1/hydrobot/evaluator.py` & `hydrobot-0.6.2/hydrobot/evaluator.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/hydrobot/filters.py` & `hydrobot-0.6.2/hydrobot/filters.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/hydrobot/plotter.py` & `hydrobot-0.6.2/hydrobot/plotter.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/hydrobot/processor.py` & `hydrobot-0.6.2/hydrobot/processor.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/hydrobot/utils.py` & `hydrobot-0.6.2/hydrobot/utils.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/hydrobot.egg-info/PKG-INFO` & `hydrobot-0.6.2/hydrobot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrobot
-Version: 0.6.1
+Version: 0.6.2
 Summary: A suite of processing tools for Hilltop hydrological data.
 Author-email: Nic Mostert <nicolas.mostert@horizons.govt.nz>, Sam Irvine <sam.irvine@horizons.govt.nz>
 License: GNU General Public License v3
 Project-URL: Homepage, https://github.com/HorizonsRC/hydrobot
 Project-URL: Issues, https://github.com/HorizonsRC/hydrobot/issues
 Project-URL: Documentation, https://hydrobot.readthedocs.io
 Project-URL: Package, https://pypi.org/project/hydrobot
@@ -82,27 +82,27 @@
   * Visualizing check points from various sources.
 
 Usage (Alpha)
 -------------
 
 The Alpha release of Hydrobot supports a "hybrid" workflow. This means that some external tools are still required to do a full processing. Importantly, the hybrid workflow relies on some R scripts to obtain check data from sources other than Hilltop. Further processing using Hilltop manager is also supported.
 
-NOTE: Hydrobot 0.6.1 supports only Water Temperature processing at the moment, but more measurements will be supported in patches as the processing progresses.
+NOTE: Hydrobot 0.6.2 supports only Water Temperature processing at the moment, but more measurements will be supported in patches as the processing progresses.
 
 Initial Setup (Repeat for each release)
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 #. Install a Python 3.11 interpreter. Note that 3.12 is not supported just yet.
-#. In your favourite shell, create a new virtual environment using this python interpreter and name it "hydrobot0.6.1". It's important that this is stored somewhere locally. I suggest creating a folder for virtual environments in your home folder::
+#. In your favourite shell, create a new virtual environment using this python interpreter and name it "hydrobot0.6.2". It's important that this is stored somewhere locally. I suggest creating a folder for virtual environments in your home folder::
 
-    python -m venv path/to/venv/hydrobot0.6.1/
+    python -m venv path/to/venv/hydrobot0.6.2/
 
 #. Activate this virtual environment. In powershell this should be something like::
 
-    ./path/to/venv/hydrobot0.6.1/Scripts/Activate.ps1
+    ./path/to/venv/hydrobot0.6.2/Scripts/Activate.ps1
 
 #. If you're sure your venv is active (ensure with `which python` and confirm that you're using the interpreter in your venv folder), install the latest version of Hydrobot using pip::
 
     pip install hydrobot
 
 #. Record which version of dependencies you have installed. The following pip freeze records which dependencies are
 installed by the hydrobot install process for if auditing/reprocessing is required later::
@@ -117,17 +117,17 @@
 Processing Steps
 ^^^^^^^^^^^^^^^^
 
 #. Open Logsheet Loader. Fill it as normal, and note the start date of your processing period (i.e. end date of the previous period).
 #. Navigate to the data source and site folder, and create your processing folder.
 #. Copy all the processing files in this folder into your processing folder::
 
-    \\ares\Environmental Data Validation\Water Temperature\Documents\Hydrobot_0.6.1_Files\
+    \\ares\Environmental Data Validation\Water Temperature\Documents\Hydrobot_0.6.2_Files\
 
-    //ares/Environmental\ Data\ Validation/Water\ Temperature/Documents/Hydrobot_0.6.1_Files/
+    //ares/Environmental\ Data\ Validation/Water\ Temperature/Documents/Hydrobot_0.6.2_Files/
 
 #. In your processing folder, open the `config.yaml` file and change the fields `site`, `from_date`, `to_date`, `analyst_name`. Feel free to mess with the other values once you get the hang of it. No one will die.
 
 #. Run the R script. I'm not an R guy so I'm not sure how to do this other than to open it in R studio, highlighting all the code, and hitting `Ctrl+Enter`. This should create a bunch of `.csv` files containing the check data from various sources. This is a good reasource for perusal during processing, but will be imbibed by hydrobot to for QC encoding.
 
 #. Make sure your virtual environment is set up and active. Ensure with `which python` and confirm that your python interpreter is running from your venv folder.
```

### Comparing `hydrobot-0.6.1/hydrobot.egg-info/SOURCES.txt` & `hydrobot-0.6.2/hydrobot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/old_setup.py` & `hydrobot-0.6.2/old_setup.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/prototypes/Class_script.py` & `hydrobot-0.6.2/prototypes/Class_script.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/prototypes/example_script/40X_XXX_WaterTemperature.accdb` & `hydrobot-0.6.2/prototypes/example_script/40X_XXX_WaterTemperature.accdb`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/prototypes/example_script/40X_XXX_WaterTemperature.hts` & `hydrobot-0.6.2/prototypes/example_script/40X_XXX_WaterTemperature.hts`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/prototypes/example_script/AP_CheckData.R` & `hydrobot-0.6.2/prototypes/example_script/AP_CheckData.R`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/prototypes/example_script/AP_config.yaml` & `hydrobot-0.6.2/prototypes/example_script/AP_config.yaml`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/prototypes/example_script/WaterTemp_CheckData.R` & `hydrobot-0.6.2/prototypes/example_script/WaterTemp_CheckData.R`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/prototypes/example_script/config.yaml` & `hydrobot-0.6.2/prototypes/example_script/config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #################################################################################
-# Hydrobot 0.6.1 Configuration File
+# Hydrobot 0.6.2 Configuration File
 #################################################################################
 
 # Hilltop Server Configuration
 base_url: "http://hilltopdev.horizons.govt.nz/"
 standard_hts_filename: "RawLoggerNet.hts"
 # check_hts_filename: "boo.hts"
```

### Comparing `hydrobot-0.6.1/prototypes/example_script/diss_ox/DO_CheckData.R` & `hydrobot-0.6.2/prototypes/example_script/diss_ox/DO_CheckData.R`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/prototypes/example_script/diss_ox/DO_config.yaml` & `hydrobot-0.6.2/prototypes/example_script/diss_ox/DO_config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # Hilltop Server Configuration
 base_url: "http://hilltopdev.horizons.govt.nz/"
 standard_hts_filename: "RawLoggerNet.hts"
 check_hts_filename: "HydrobotCheckData.hts"
 
 # Data Source Configuration
-site: "Rangitikei at Mangaweka"
+site: "Oroua at Almadale Slackline"
 standard_measurement_name: "DO Saturation [Dissolved Oxygen (%)]"
 check_measurement_name: "DO saturation check"
 frequency: "15min"
 site_altitude: 156
 
 # water_temperature_site: "Rangitikei at McKelvies"
 water_temperature_hts: "ProvisionalAuto.hts"
 water_temperature_frequency: "15min"
 water_temperature_measurement_name: "Water Temperature"
 
 
-# atmospheric_pressure_site: "Rangitikei at McKelvies"
+atmospheric_pressure_site: "Manawatu at Teachers College"
 atmospheric_pressure_hts: "ProvisionalAuto.hts"
 atmospheric_pressure_frequency: "15min"
 atmospheric_pressure_measurement_name: "Atmospheric Pressure"
 atmospheric_pressure_site_altitude: 143
 
 # Processing Configuration
-from_date: "2022-12-21 11:15"
+from_date: "2023-06-15 14:45:00"
 to_date: "2024-04-02 10:00"
 defaults:
   delta: 5
   gap_limit: 12
   high_clip: 200
   low_clip: 50
   max_qc: 600
```

### Comparing `hydrobot-0.6.1/prototypes/example_script/diss_ox/do_script.py` & `hydrobot-0.6.2/prototypes/example_script/diss_ox/do_script.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/prototypes/example_script/script.py` & `hydrobot-0.6.2/prototypes/example_script/script.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 #######################################################################################
 # Reading configuration from config.yaml
 #######################################################################################
 
 data, ann = Processor.from_config_yaml("config.yaml")
 
-st.set_page_config(page_title="Hydrobot0.6.1", layout="wide", page_icon="💦")
+st.set_page_config(page_title="Hydrobot0.6.2", layout="wide", page_icon="💦")
 st.title(f"{data.site}")
 st.header(f"{data.standard_measurement_name}")
 
 #######################################################################################
 # Importing all check data that is not obtainable from Hilltop
 # (So far Hydrobot only speaks to Hilltop)
 #######################################################################################
```

### Comparing `hydrobot-0.6.1/prototypes/py_scripts/atmospheric_spike_removal.py` & `hydrobot-0.6.2/prototypes/py_scripts/atmospheric_spike_removal.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/prototypes/py_scripts/example_plot_script.py` & `hydrobot-0.6.2/prototypes/py_scripts/example_plot_script.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/prototypes/py_scripts/gap_finder.py` & `hydrobot-0.6.2/prototypes/py_scripts/gap_finder.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/prototypes/py_scripts/new_ws_plot_with_check_data.py` & `hydrobot-0.6.2/prototypes/py_scripts/new_ws_plot_with_check_data.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/prototypes/py_scripts/plot_with_check_data.py` & `hydrobot-0.6.2/prototypes/py_scripts/plot_with_check_data.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/prototypes/py_scripts/process_script.py` & `hydrobot-0.6.2/prototypes/py_scripts/process_script.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/prototypes/py_scripts/spike_removal_util.py` & `hydrobot-0.6.2/prototypes/py_scripts/spike_removal_util.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/prototypes/py_scripts/stage_full_process.py` & `hydrobot-0.6.2/prototypes/py_scripts/stage_full_process.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/prototypes/py_scripts/water_temp_full_process.py` & `hydrobot-0.6.2/prototypes/py_scripts/water_temp_full_process.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/prototypes/py_scripts/water_temp_spike_removal.py` & `hydrobot-0.6.2/prototypes/py_scripts/water_temp_spike_removal.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/prototypes/site_list_reader.py` & `hydrobot-0.6.2/prototypes/site_list_reader.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/pyproject.toml` & `hydrobot-0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hydrobot"
 description = "A suite of processing tools for Hilltop hydrological data."
-version = "0.6.1"
+version = "0.6.2"
 authors = [
     { name = "Nic Mostert", email = "nicolas.mostert@horizons.govt.nz" },
     { name = "Sam Irvine", email = "sam.irvine@horizons.govt.nz" }
 ]
 requires-python = "==3.11.*"
 dependencies = [
     "hilltop-py>=2.3.1",
@@ -98,15 +98,15 @@
 
 [tool.ruff.per-file-ignores]
 "tests/*" = ["S311", "S101", "F841"]
 "docs/*" = ["I001"]
 "prototypes" = ["D"]
 
 [tool.bumpversion]
-current_version = "0.6.1"
+current_version = "0.6.2"
 commit = true
 tag = true
 tag_name = "{new_version}"
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = "{current_version}"
```

### Comparing `hydrobot-0.6.1/requirements_dev.txt` & `hydrobot-0.6.2/requirements_dev.txt`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/tests/.coverage` & `hydrobot-0.6.2/tests/.coverage`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/tests/conftest.py` & `hydrobot-0.6.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/tests/test_data/test_config.yaml` & `hydrobot-0.6.2/tests/test_data/test_config.yaml`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/tests/test_data/xml_test_data_file.xml` & `hydrobot-0.6.2/tests/test_data/xml_test_data_file.xml`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/tests/test_data/xml_test_data_no_check.xml` & `hydrobot-0.6.2/tests/test_data/xml_test_data_no_check.xml`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/tests/test_data/xml_test_data_no_qual.xml` & `hydrobot-0.6.2/tests/test_data/xml_test_data_no_qual.xml`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/tests/test_data_sources.py` & `hydrobot-0.6.2/tests/test_data_sources.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/tests/test_data_structure.py` & `hydrobot-0.6.2/tests/test_data_structure.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/tests/test_evaluator.py` & `hydrobot-0.6.2/tests/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/tests/test_filters.py` & `hydrobot-0.6.2/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/tests/test_processor.py` & `hydrobot-0.6.2/tests/test_processor.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/tests/test_utils.py` & `hydrobot-0.6.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.6.1/tests/test_web_integration.py` & `hydrobot-0.6.2/tests/test_web_integration.py`

 * *Files identical despite different names*

