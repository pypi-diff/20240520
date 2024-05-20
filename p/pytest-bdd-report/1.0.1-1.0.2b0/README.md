# Comparing `tmp/pytest_bdd_report-1.0.1.tar.gz` & `tmp/pytest_bdd_report-1.0.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_bdd_report-1.0.1.tar", last modified: Mon Feb 19 16:37:41 2024, max compression
+gzip compressed data, was "pytest_bdd_report-1.0.2b0.tar", last modified: Mon May 20 14:51:59 2024, max compression
```

## Comparing `pytest_bdd_report-1.0.1.tar` & `pytest_bdd_report-1.0.2b0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 mattia     (501) staff       (20)        0 2024-02-19 16:37:41.546045 pytest_bdd_report-1.0.1/
--rw-r--r--   0 mattia     (501) staff       (20)     1080 2024-02-16 09:03:02.000000 pytest_bdd_report-1.0.1/LICENSE
--rw-r--r--   0 mattia     (501) staff       (20)      214 2024-02-16 09:03:02.000000 pytest_bdd_report-1.0.1/MANIFEST.in
--rw-r--r--   0 mattia     (501) staff       (20)     4642 2024-02-19 16:37:41.545873 pytest_bdd_report-1.0.1/PKG-INFO
--rw-r--r--   0 mattia     (501) staff       (20)     3968 2024-02-19 14:45:01.000000 pytest_bdd_report-1.0.1/README.rst
--rw-r--r--   0 mattia     (501) staff       (20)      828 2024-02-19 16:34:51.000000 pytest_bdd_report-1.0.1/pyproject.toml
--rw-r--r--   0 mattia     (501) staff       (20)       38 2024-02-19 16:37:41.546080 pytest_bdd_report-1.0.1/setup.cfg
-drwxr-xr-x   0 mattia     (501) staff       (20)        0 2024-02-19 16:37:41.540151 pytest_bdd_report-1.0.1/src/
-drwxr-xr-x   0 mattia     (501) staff       (20)        0 2024-02-19 16:37:41.541916 pytest_bdd_report-1.0.1/src/pytest_bdd_report/
--rw-r--r--   0 mattia     (501) staff       (20)        0 2024-02-16 09:03:02.000000 pytest_bdd_report-1.0.1/src/pytest_bdd_report/__init__.py
-drwxr-xr-x   0 mattia     (501) staff       (20)        0 2024-02-19 16:37:41.542903 pytest_bdd_report-1.0.1/src/pytest_bdd_report/components/
--rw-r--r--   0 mattia     (501) staff       (20)        0 2024-02-16 09:03:02.000000 pytest_bdd_report-1.0.1/src/pytest_bdd_report/components/__init__.py
--rw-r--r--   0 mattia     (501) staff       (20)     2154 2024-02-19 16:34:51.000000 pytest_bdd_report-1.0.1/src/pytest_bdd_report/components/feature.py
--rw-r--r--   0 mattia     (501) staff       (20)      742 2024-02-19 16:34:51.000000 pytest_bdd_report-1.0.1/src/pytest_bdd_report/components/scenario.py
--rw-r--r--   0 mattia     (501) staff       (20)      166 2024-02-16 09:03:02.000000 pytest_bdd_report-1.0.1/src/pytest_bdd_report/components/step.py
--rw-r--r--   0 mattia     (501) staff       (20)     4200 2024-02-19 16:34:51.000000 pytest_bdd_report-1.0.1/src/pytest_bdd_report/extractor.py
--rw-r--r--   0 mattia     (501) staff       (20)      751 2024-02-19 16:34:51.000000 pytest_bdd_report-1.0.1/src/pytest_bdd_report/interfaces.py
--rw-r--r--   0 mattia     (501) staff       (20)      350 2024-02-19 16:34:51.000000 pytest_bdd_report-1.0.1/src/pytest_bdd_report/json_loader.py
--rw-r--r--   0 mattia     (501) staff       (20)     2528 2024-02-19 16:34:51.000000 pytest_bdd_report-1.0.1/src/pytest_bdd_report/pytest_bdd_report.py
--rw-r--r--   0 mattia     (501) staff       (20)     2399 2024-02-19 16:34:51.000000 pytest_bdd_report-1.0.1/src/pytest_bdd_report/renderer.py
--rw-r--r--   0 mattia     (501) staff       (20)      597 2024-02-19 16:34:51.000000 pytest_bdd_report-1.0.1/src/pytest_bdd_report/report.py
--rw-r--r--   0 mattia     (501) staff       (20)     1235 2024-02-19 16:34:51.000000 pytest_bdd_report-1.0.1/src/pytest_bdd_report/report_composer.py
--rw-r--r--   0 mattia     (501) staff       (20)     3107 2024-02-19 16:34:51.000000 pytest_bdd_report-1.0.1/src/pytest_bdd_report/report_file_generator.py
--rw-r--r--   0 mattia     (501) staff       (20)     1680 2024-02-16 09:03:02.000000 pytest_bdd_report-1.0.1/src/pytest_bdd_report/setup.py
-drwxr-xr-x   0 mattia     (501) staff       (20)        0 2024-02-19 16:37:41.543198 pytest_bdd_report-1.0.1/src/pytest_bdd_report/summary/
--rw-r--r--   0 mattia     (501) staff       (20)        0 2024-02-16 09:03:02.000000 pytest_bdd_report-1.0.1/src/pytest_bdd_report/summary/__init__.py
--rw-r--r--   0 mattia     (501) staff       (20)      457 2024-02-19 16:34:51.000000 pytest_bdd_report-1.0.1/src/pytest_bdd_report/summary/summary.py
--rw-r--r--   0 mattia     (501) staff       (20)     2524 2024-02-19 16:34:51.000000 pytest_bdd_report-1.0.1/src/pytest_bdd_report/summary/summary_generator.py
-drwxr-xr-x   0 mattia     (501) staff       (20)        0 2024-02-19 16:37:41.544119 pytest_bdd_report-1.0.1/src/pytest_bdd_report/templates/
--rw-r--r--   0 mattia     (501) staff       (20)        0 2024-02-16 09:03:02.000000 pytest_bdd_report-1.0.1/src/pytest_bdd_report/templates/__init__.py
--rw-r--r--   0 mattia     (501) staff       (20)      984 2024-02-19 16:34:51.000000 pytest_bdd_report-1.0.1/src/pytest_bdd_report/templates/feature_statistics_template.py
--rw-r--r--   0 mattia     (501) staff       (20)     1073 2024-02-19 16:34:51.000000 pytest_bdd_report-1.0.1/src/pytest_bdd_report/templates/feature_template.py
-drwxr-xr-x   0 mattia     (501) staff       (20)        0 2024-02-19 16:37:41.544861 pytest_bdd_report-1.0.1/src/pytest_bdd_report/templates/html_templates/
-drwxr-xr-x   0 mattia     (501) staff       (20)        0 2024-02-19 16:37:41.545544 pytest_bdd_report-1.0.1/src/pytest_bdd_report/templates/html_templates/components/
--rw-r--r--   0 mattia     (501) staff       (20)      846 2024-02-16 09:03:02.000000 pytest_bdd_report-1.0.1/src/pytest_bdd_report/templates/html_templates/components/badge.html
--rw-r--r--   0 mattia     (501) staff       (20)      740 2024-02-16 09:03:02.000000 pytest_bdd_report-1.0.1/src/pytest_bdd_report/templates/html_templates/components/duration.html
--rw-r--r--   0 mattia     (501) staff       (20)      281 2024-02-16 09:03:02.000000 pytest_bdd_report-1.0.1/src/pytest_bdd_report/templates/html_templates/components/feature_statistics_link.html
--rw-r--r--   0 mattia     (501) staff       (20)      919 2024-02-16 09:03:02.000000 pytest_bdd_report-1.0.1/src/pytest_bdd_report/templates/html_templates/components/filters.html
--rw-r--r--   0 mattia     (501) staff       (20)     4987 2024-02-16 09:03:02.000000 pytest_bdd_report-1.0.1/src/pytest_bdd_report/templates/html_templates/components/icon.html
--rw-r--r--   0 mattia     (501) staff       (20)      862 2024-02-16 09:03:02.000000 pytest_bdd_report-1.0.1/src/pytest_bdd_report/templates/html_templates/components/test_file_uri.html
--rw-r--r--   0 mattia     (501) staff       (20)     1890 2024-02-16 09:03:02.000000 pytest_bdd_report-1.0.1/src/pytest_bdd_report/templates/html_templates/feature.html
--rw-r--r--   0 mattia     (501) staff       (20)     1098 2024-02-16 09:03:02.000000 pytest_bdd_report-1.0.1/src/pytest_bdd_report/templates/html_templates/feature_statistics.html
--rw-r--r--   0 mattia     (501) staff       (20)     3502 2024-02-16 09:03:02.000000 pytest_bdd_report-1.0.1/src/pytest_bdd_report/templates/html_templates/report.html
--rw-r--r--   0 mattia     (501) staff       (20)     4181 2024-02-16 09:03:02.000000 pytest_bdd_report-1.0.1/src/pytest_bdd_report/templates/html_templates/scenario.html
--rw-r--r--   0 mattia     (501) staff       (20)      850 2024-02-16 09:03:02.000000 pytest_bdd_report-1.0.1/src/pytest_bdd_report/templates/html_templates/step.html
--rw-r--r--   0 mattia     (501) staff       (20)     6313 2024-02-16 09:03:02.000000 pytest_bdd_report-1.0.1/src/pytest_bdd_report/templates/html_templates/summary.html
--rw-r--r--   0 mattia     (501) staff       (20)     1949 2024-02-19 16:34:51.000000 pytest_bdd_report-1.0.1/src/pytest_bdd_report/templates/report_template.py
--rw-r--r--   0 mattia     (501) staff       (20)     1341 2024-02-19 16:34:51.000000 pytest_bdd_report-1.0.1/src/pytest_bdd_report/templates/scenario_template.py
--rw-r--r--   0 mattia     (501) staff       (20)      487 2024-02-19 16:34:51.000000 pytest_bdd_report-1.0.1/src/pytest_bdd_report/templates/step_template.py
--rw-r--r--   0 mattia     (501) staff       (20)      678 2024-02-19 16:34:51.000000 pytest_bdd_report-1.0.1/src/pytest_bdd_report/templates/summary_template.py
--rw-r--r--   0 mattia     (501) staff       (20)      941 2024-02-19 16:34:51.000000 pytest_bdd_report-1.0.1/src/pytest_bdd_report/templates/template.py
-drwxr-xr-x   0 mattia     (501) staff       (20)        0 2024-02-19 16:37:41.545699 pytest_bdd_report-1.0.1/src/pytest_bdd_report.egg-info/
--rw-r--r--   0 mattia     (501) staff       (20)     4642 2024-02-19 16:37:41.000000 pytest_bdd_report-1.0.1/src/pytest_bdd_report.egg-info/PKG-INFO
--rw-r--r--   0 mattia     (501) staff       (20)     2216 2024-02-19 16:37:41.000000 pytest_bdd_report-1.0.1/src/pytest_bdd_report.egg-info/SOURCES.txt
--rw-r--r--   0 mattia     (501) staff       (20)        1 2024-02-19 16:37:41.000000 pytest_bdd_report-1.0.1/src/pytest_bdd_report.egg-info/dependency_links.txt
--rw-r--r--   0 mattia     (501) staff       (20)       60 2024-02-19 16:37:41.000000 pytest_bdd_report-1.0.1/src/pytest_bdd_report.egg-info/entry_points.txt
--rw-r--r--   0 mattia     (501) staff       (20)       46 2024-02-19 16:37:41.000000 pytest_bdd_report-1.0.1/src/pytest_bdd_report.egg-info/requires.txt
--rw-r--r--   0 mattia     (501) staff       (20)       18 2024-02-19 16:37:41.000000 pytest_bdd_report-1.0.1/src/pytest_bdd_report.egg-info/top_level.txt
+drwxr-xr-x   0 mattia     (501) staff       (20)        0 2024-05-20 14:51:59.356599 pytest_bdd_report-1.0.2b0/
+-rw-r--r--   0 mattia     (501) staff       (20)     1080 2024-05-20 14:45:06.000000 pytest_bdd_report-1.0.2b0/LICENSE
+-rw-r--r--   0 mattia     (501) staff       (20)      214 2024-05-20 14:45:06.000000 pytest_bdd_report-1.0.2b0/MANIFEST.in
+-rw-r--r--   0 mattia     (501) staff       (20)     5258 2024-05-20 14:51:59.356407 pytest_bdd_report-1.0.2b0/PKG-INFO
+-rw-r--r--   0 mattia     (501) staff       (20)     4575 2024-05-20 14:45:06.000000 pytest_bdd_report-1.0.2b0/README.rst
+-rw-r--r--   0 mattia     (501) staff       (20)      840 2024-05-20 14:47:52.000000 pytest_bdd_report-1.0.2b0/pyproject.toml
+-rw-r--r--   0 mattia     (501) staff       (20)       38 2024-05-20 14:51:59.356638 pytest_bdd_report-1.0.2b0/setup.cfg
+drwxr-xr-x   0 mattia     (501) staff       (20)        0 2024-05-20 14:51:59.350837 pytest_bdd_report-1.0.2b0/src/
+drwxr-xr-x   0 mattia     (501) staff       (20)        0 2024-05-20 14:51:59.352665 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/
+-rw-r--r--   0 mattia     (501) staff       (20)        0 2024-05-20 14:45:06.000000 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/__init__.py
+drwxr-xr-x   0 mattia     (501) staff       (20)        0 2024-05-20 14:51:59.353711 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/components/
+-rw-r--r--   0 mattia     (501) staff       (20)        0 2024-05-20 14:45:06.000000 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/components/__init__.py
+-rw-r--r--   0 mattia     (501) staff       (20)     2154 2024-05-20 14:45:06.000000 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/components/feature.py
+-rw-r--r--   0 mattia     (501) staff       (20)      742 2024-05-20 14:45:06.000000 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/components/scenario.py
+-rw-r--r--   0 mattia     (501) staff       (20)      166 2024-05-20 14:45:06.000000 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/components/step.py
+-rw-r--r--   0 mattia     (501) staff       (20)     4200 2024-05-20 14:45:06.000000 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/extractor.py
+-rw-r--r--   0 mattia     (501) staff       (20)      751 2024-05-20 14:45:06.000000 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/interfaces.py
+-rw-r--r--   0 mattia     (501) staff       (20)      350 2024-05-20 14:45:06.000000 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/json_loader.py
+-rw-r--r--   0 mattia     (501) staff       (20)     2528 2024-05-20 14:45:06.000000 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/pytest_bdd_report.py
+-rw-r--r--   0 mattia     (501) staff       (20)     2208 2024-05-20 14:45:06.000000 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/renderer.py
+-rw-r--r--   0 mattia     (501) staff       (20)      597 2024-05-20 14:45:06.000000 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/report.py
+-rw-r--r--   0 mattia     (501) staff       (20)     1235 2024-05-20 14:45:06.000000 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/report_composer.py
+-rw-r--r--   0 mattia     (501) staff       (20)     3107 2024-05-20 14:45:06.000000 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/report_file_generator.py
+-rw-r--r--   0 mattia     (501) staff       (20)     1680 2024-05-20 14:45:06.000000 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/setup.py
+drwxr-xr-x   0 mattia     (501) staff       (20)        0 2024-05-20 14:51:59.354008 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/summary/
+-rw-r--r--   0 mattia     (501) staff       (20)        0 2024-05-20 14:45:06.000000 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/summary/__init__.py
+-rw-r--r--   0 mattia     (501) staff       (20)      457 2024-05-20 14:45:06.000000 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/summary/summary.py
+-rw-r--r--   0 mattia     (501) staff       (20)     2524 2024-05-20 14:45:06.000000 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/summary/summary_generator.py
+drwxr-xr-x   0 mattia     (501) staff       (20)        0 2024-05-20 14:51:59.354822 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/templates/
+-rw-r--r--   0 mattia     (501) staff       (20)        0 2024-05-20 14:45:06.000000 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/templates/__init__.py
+-rw-r--r--   0 mattia     (501) staff       (20)      984 2024-05-20 14:45:06.000000 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/templates/feature_statistics_template.py
+-rw-r--r--   0 mattia     (501) staff       (20)     1073 2024-05-20 14:45:06.000000 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/templates/feature_template.py
+drwxr-xr-x   0 mattia     (501) staff       (20)        0 2024-05-20 14:51:59.355469 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/templates/html_templates/
+drwxr-xr-x   0 mattia     (501) staff       (20)        0 2024-05-20 14:51:59.356094 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/templates/html_templates/components/
+-rw-r--r--   0 mattia     (501) staff       (20)      846 2024-05-20 14:45:06.000000 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/templates/html_templates/components/badge.html
+-rw-r--r--   0 mattia     (501) staff       (20)      740 2024-05-20 14:45:06.000000 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/templates/html_templates/components/duration.html
+-rw-r--r--   0 mattia     (501) staff       (20)      281 2024-05-20 14:45:06.000000 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/templates/html_templates/components/feature_statistics_link.html
+-rw-r--r--   0 mattia     (501) staff       (20)      919 2024-05-20 14:45:06.000000 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/templates/html_templates/components/filters.html
+-rw-r--r--   0 mattia     (501) staff       (20)     4987 2024-05-20 14:45:06.000000 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/templates/html_templates/components/icon.html
+-rw-r--r--   0 mattia     (501) staff       (20)      862 2024-05-20 14:45:06.000000 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/templates/html_templates/components/test_file_uri.html
+-rw-r--r--   0 mattia     (501) staff       (20)     1890 2024-05-20 14:45:06.000000 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/templates/html_templates/feature.html
+-rw-r--r--   0 mattia     (501) staff       (20)     1098 2024-05-20 14:45:06.000000 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/templates/html_templates/feature_statistics.html
+-rw-r--r--   0 mattia     (501) staff       (20)     3502 2024-05-20 14:45:06.000000 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/templates/html_templates/report.html
+-rw-r--r--   0 mattia     (501) staff       (20)     4181 2024-05-20 14:45:06.000000 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/templates/html_templates/scenario.html
+-rw-r--r--   0 mattia     (501) staff       (20)      850 2024-05-20 14:45:06.000000 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/templates/html_templates/step.html
+-rw-r--r--   0 mattia     (501) staff       (20)     6313 2024-05-20 14:45:06.000000 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/templates/html_templates/summary.html
+-rw-r--r--   0 mattia     (501) staff       (20)     1949 2024-05-20 14:45:06.000000 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/templates/report_template.py
+-rw-r--r--   0 mattia     (501) staff       (20)     1341 2024-05-20 14:45:06.000000 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/templates/scenario_template.py
+-rw-r--r--   0 mattia     (501) staff       (20)      487 2024-05-20 14:45:06.000000 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/templates/step_template.py
+-rw-r--r--   0 mattia     (501) staff       (20)      678 2024-05-20 14:45:06.000000 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/templates/summary_template.py
+-rw-r--r--   0 mattia     (501) staff       (20)      941 2024-05-20 14:45:06.000000 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/templates/template.py
+drwxr-xr-x   0 mattia     (501) staff       (20)        0 2024-05-20 14:51:59.356232 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report.egg-info/
+-rw-r--r--   0 mattia     (501) staff       (20)     5258 2024-05-20 14:51:59.000000 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report.egg-info/PKG-INFO
+-rw-r--r--   0 mattia     (501) staff       (20)     2216 2024-05-20 14:51:59.000000 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report.egg-info/SOURCES.txt
+-rw-r--r--   0 mattia     (501) staff       (20)        1 2024-05-20 14:51:59.000000 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report.egg-info/dependency_links.txt
+-rw-r--r--   0 mattia     (501) staff       (20)       60 2024-05-20 14:51:59.000000 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report.egg-info/entry_points.txt
+-rw-r--r--   0 mattia     (501) staff       (20)       53 2024-05-20 14:51:59.000000 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report.egg-info/requires.txt
+-rw-r--r--   0 mattia     (501) staff       (20)       18 2024-05-20 14:51:59.000000 pytest_bdd_report-1.0.2b0/src/pytest_bdd_report.egg-info/top_level.txt
```

### Comparing `pytest_bdd_report-1.0.1/LICENSE` & `pytest_bdd_report-1.0.2b0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_bdd_report-1.0.1/PKG-INFO` & `pytest_bdd_report-1.0.2b0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 Metadata-Version: 2.1
 Name: pytest_bdd_report
-Version: 1.0.1
+Version: 1.0.2b0
 Summary: A pytest-bdd plugin for generating useful and informative BDD test reports
 Author-email: Mattia Monti <mattiamonti2001@gmail.com>
 Project-URL: Homepage, https://github.com/mattiamonti/pytest-bdd-report
 Project-URL: Bug Tracker, https://github.com/mattiamonti/pytest-bdd-report/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: pytest>=7.1.3
-Requires-Dist: pytest-bdd>=6.1.1
+Requires-Dist: pytest-bdd<7.0.0,>=5.0.0
 Requires-Dist: Jinja2>=3.1.2
 
 =================
 pytest-bdd-report
 =================
 
-|python| |pypi| |formatting| |tests|
+|python| |pypi| |formatting| |tests| |ui_tests|
 
-|dstats| |mstats|
+|mstats| |total|
 
+.. |total| image:: https://static.pepy.tech/badge/pytest-bdd-report
+    :target: https://pepy.tech/project/pytest-bdd-report
+    :alt: PePy total downloads
 
 .. |pypi| image:: https://img.shields.io/pypi/v/pytest-bdd-report.svg
     :target: https://pypi.org/project/pytest-bdd-report
     :alt: PyPI version
 
 .. |python| image:: https://img.shields.io/pypi/pyversions/pytest-bdd-report.svg
     :target: https://pypi.org/project/pytest-bdd-report
@@ -34,26 +37,31 @@
 
 .. |formatting| image:: https://img.shields.io/github/actions/workflow/status/mattiamonti/pytest-bdd-report/automated%20tests.yml?logo=GitHub%20actions&label=Formatting
     :alt: GitHub Workflow Status (with event)
 
 .. |tests| image:: https://img.shields.io/github/actions/workflow/status/mattiamonti/pytest-bdd-report/automated%20tests.yml?logo=pytest&label=Tests
     :alt: GitHub Workflow Status (with event)
 
+.. |ui_tests| image:: https://img.shields.io/github/actions/workflow/status/mattiamonti/pytest-bdd-report/ui%20automated%20tests.yml?logo=robotframework&label=UI%20Tests
+    :alt: GitHub Workflow Status (with event)
+
 .. |mstats| image:: https://img.shields.io/pypi/dm/pytest-bdd-report
    :alt: PyPI - Downloads
 
 .. |dstats| image:: https://img.shields.io/pypi/dd/pytest-bdd-report
    :alt: PyPI - Downloads
 
 
 
-The `pytest-bdd-report` plugin is a useful extension for the `pytest-bdd`_ library that allows you to generate 
+The `pytest-bdd-report` plugin is a useful extension for the `pytest-bdd`_ library that allows you to generate
 useful and informative reports for BDD (Behavior-Driven Development) tests developed using the pytest-bdd framework.
 This plugin facilitates the generation of clear and effective HTML reports, providing a comprehensible view of BDD test executions within the project.
 
+For more, check out the `Documentation`_
+
 ----
 
 This `pytest`_ plugin was generated with `Cookiecutter`_ along with `@hackebrot`_'s `cookiecutter-pytest-plugin`_ template.
 
 
 Features
 --------
@@ -109,20 +117,27 @@
 3. Install the plugin locally:
 
 ::
 
     $ pip install -e .
 
 
-4. Run the tests:
+4. Run the unit tests:
 
 ::
 
     $ python -m pytest
 
+5. Run the UI tests with Robot Framework:
+
+::
+
+    $ cd tests/ui_testing
+    $ ./execute_all_ui_tests.sh
+
 
 Contributing
 ------------
 Contributions are very welcome. Tests can be run with `pytest`_ as shown.
 
 License
 -------
@@ -144,7 +159,8 @@
 .. _`cookiecutter-pytest-plugin`: https://github.com/pytest-dev/cookiecutter-pytest-plugin
 .. _`file an issue`: https://github.com/mattiamonti/pytest-bdd-report/issues
 .. _`pytest`: https://github.com/pytest-dev/pytest
 .. _`tox`: https://tox.readthedocs.io/en/latest/
 .. _`pip`: https://pypi.org/project/pip/
 .. _`PyPI`: https://pypi.org/project
 .. _`pytest-bdd`: https://github.com/pytest-dev/pytest-bdd
+.. _`Documentation`: https://mattia-monti.gitbook.io/pytest-bdd-report/
```

### Comparing `pytest_bdd_report-1.0.1/README.rst` & `pytest_bdd_report-1.0.2b0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 =================
 pytest-bdd-report
 =================
 
-|python| |pypi| |formatting| |tests|
+|python| |pypi| |formatting| |tests| |ui_tests|
 
-|dstats| |mstats|
+|mstats| |total|
 
+.. |total| image:: https://static.pepy.tech/badge/pytest-bdd-report
+    :target: https://pepy.tech/project/pytest-bdd-report
+    :alt: PePy total downloads
 
 .. |pypi| image:: https://img.shields.io/pypi/v/pytest-bdd-report.svg
     :target: https://pypi.org/project/pytest-bdd-report
     :alt: PyPI version
 
 .. |python| image:: https://img.shields.io/pypi/pyversions/pytest-bdd-report.svg
     :target: https://pypi.org/project/pytest-bdd-report
@@ -17,26 +20,31 @@
 
 .. |formatting| image:: https://img.shields.io/github/actions/workflow/status/mattiamonti/pytest-bdd-report/automated%20tests.yml?logo=GitHub%20actions&label=Formatting
     :alt: GitHub Workflow Status (with event)
 
 .. |tests| image:: https://img.shields.io/github/actions/workflow/status/mattiamonti/pytest-bdd-report/automated%20tests.yml?logo=pytest&label=Tests
     :alt: GitHub Workflow Status (with event)
 
+.. |ui_tests| image:: https://img.shields.io/github/actions/workflow/status/mattiamonti/pytest-bdd-report/ui%20automated%20tests.yml?logo=robotframework&label=UI%20Tests
+    :alt: GitHub Workflow Status (with event)
+
 .. |mstats| image:: https://img.shields.io/pypi/dm/pytest-bdd-report
    :alt: PyPI - Downloads
 
 .. |dstats| image:: https://img.shields.io/pypi/dd/pytest-bdd-report
    :alt: PyPI - Downloads
 
 
 
-The `pytest-bdd-report` plugin is a useful extension for the `pytest-bdd`_ library that allows you to generate 
+The `pytest-bdd-report` plugin is a useful extension for the `pytest-bdd`_ library that allows you to generate
 useful and informative reports for BDD (Behavior-Driven Development) tests developed using the pytest-bdd framework.
 This plugin facilitates the generation of clear and effective HTML reports, providing a comprehensible view of BDD test executions within the project.
 
+For more, check out the `Documentation`_
+
 ----
 
 This `pytest`_ plugin was generated with `Cookiecutter`_ along with `@hackebrot`_'s `cookiecutter-pytest-plugin`_ template.
 
 
 Features
 --------
@@ -92,20 +100,27 @@
 3. Install the plugin locally:
 
 ::
 
     $ pip install -e .
 
 
-4. Run the tests:
+4. Run the unit tests:
 
 ::
 
     $ python -m pytest
 
+5. Run the UI tests with Robot Framework:
+
+::
+
+    $ cd tests/ui_testing
+    $ ./execute_all_ui_tests.sh
+
 
 Contributing
 ------------
 Contributions are very welcome. Tests can be run with `pytest`_ as shown.
 
 License
 -------
@@ -127,7 +142,8 @@
 .. _`cookiecutter-pytest-plugin`: https://github.com/pytest-dev/cookiecutter-pytest-plugin
 .. _`file an issue`: https://github.com/mattiamonti/pytest-bdd-report/issues
 .. _`pytest`: https://github.com/pytest-dev/pytest
 .. _`tox`: https://tox.readthedocs.io/en/latest/
 .. _`pip`: https://pypi.org/project/pip/
 .. _`PyPI`: https://pypi.org/project
 .. _`pytest-bdd`: https://github.com/pytest-dev/pytest-bdd
+.. _`Documentation`: https://mattia-monti.gitbook.io/pytest-bdd-report/
```

### Comparing `pytest_bdd_report-1.0.1/pyproject.toml` & `pytest_bdd_report-1.0.2b0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytest_bdd_report"
-version = "1.0.1"
+version = "1.0.2-beta"
 authors = [
   { name="Mattia Monti", email="mattiamonti2001@gmail.com" },
 ]
 description = "A pytest-bdd plugin for generating useful and informative BDD test reports"
 readme = "README.rst"
 requires-python = ">=3.5"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
 	'pytest >= 7.1.3',
-	'pytest-bdd >= 6.1.1',
+	'pytest-bdd >= 5.0.0,<7.0.0',
 	'Jinja2 >= 3.1.2',
 ]
 
 [project.entry-points.pytest11]
 bdd-report = "pytest_bdd_report.pytest_bdd_report"
 
 [project.urls]
```

### Comparing `pytest_bdd_report-1.0.1/src/pytest_bdd_report/components/feature.py` & `pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/components/feature.py`

 * *Files identical despite different names*

### Comparing `pytest_bdd_report-1.0.1/src/pytest_bdd_report/components/scenario.py` & `pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/components/scenario.py`

 * *Files identical despite different names*

### Comparing `pytest_bdd_report-1.0.1/src/pytest_bdd_report/extractor.py` & `pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/extractor.py`

 * *Files identical despite different names*

### Comparing `pytest_bdd_report-1.0.1/src/pytest_bdd_report/interfaces.py` & `pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/interfaces.py`

 * *Files identical despite different names*

### Comparing `pytest_bdd_report-1.0.1/src/pytest_bdd_report/pytest_bdd_report.py` & `pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/pytest_bdd_report.py`

 * *Files identical despite different names*

### Comparing `pytest_bdd_report-1.0.1/src/pytest_bdd_report/report.py` & `pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/report.py`

 * *Files identical despite different names*

### Comparing `pytest_bdd_report-1.0.1/src/pytest_bdd_report/report_composer.py` & `pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/report_composer.py`

 * *Files identical despite different names*

### Comparing `pytest_bdd_report-1.0.1/src/pytest_bdd_report/report_file_generator.py` & `pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/report_file_generator.py`

 * *Files identical despite different names*

### Comparing `pytest_bdd_report-1.0.1/src/pytest_bdd_report/setup.py` & `pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/setup.py`

 * *Files identical despite different names*

### Comparing `pytest_bdd_report-1.0.1/src/pytest_bdd_report/summary/summary_generator.py` & `pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/summary/summary_generator.py`

 * *Files identical despite different names*

### Comparing `pytest_bdd_report-1.0.1/src/pytest_bdd_report/templates/feature_statistics_template.py` & `pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/templates/feature_statistics_template.py`

 * *Files identical despite different names*

### Comparing `pytest_bdd_report-1.0.1/src/pytest_bdd_report/templates/feature_template.py` & `pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/templates/feature_template.py`

 * *Files identical despite different names*

### Comparing `pytest_bdd_report-1.0.1/src/pytest_bdd_report/templates/html_templates/components/badge.html` & `pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/templates/html_templates/components/badge.html`

 * *Files identical despite different names*

### Comparing `pytest_bdd_report-1.0.1/src/pytest_bdd_report/templates/html_templates/components/duration.html` & `pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/templates/html_templates/components/duration.html`

 * *Files identical despite different names*

### Comparing `pytest_bdd_report-1.0.1/src/pytest_bdd_report/templates/html_templates/components/filters.html` & `pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/templates/html_templates/components/filters.html`

 * *Files identical despite different names*

### Comparing `pytest_bdd_report-1.0.1/src/pytest_bdd_report/templates/html_templates/components/icon.html` & `pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/templates/html_templates/components/icon.html`

 * *Files identical despite different names*

### Comparing `pytest_bdd_report-1.0.1/src/pytest_bdd_report/templates/html_templates/components/test_file_uri.html` & `pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/templates/html_templates/components/test_file_uri.html`

 * *Files identical despite different names*

### Comparing `pytest_bdd_report-1.0.1/src/pytest_bdd_report/templates/html_templates/feature.html` & `pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/templates/html_templates/feature.html`

 * *Files identical despite different names*

### Comparing `pytest_bdd_report-1.0.1/src/pytest_bdd_report/templates/html_templates/feature_statistics.html` & `pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/templates/html_templates/feature_statistics.html`

 * *Files identical despite different names*

### Comparing `pytest_bdd_report-1.0.1/src/pytest_bdd_report/templates/html_templates/report.html` & `pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/templates/html_templates/report.html`

 * *Files identical despite different names*

### Comparing `pytest_bdd_report-1.0.1/src/pytest_bdd_report/templates/html_templates/scenario.html` & `pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/templates/html_templates/scenario.html`

 * *Files identical despite different names*

### Comparing `pytest_bdd_report-1.0.1/src/pytest_bdd_report/templates/html_templates/step.html` & `pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/templates/html_templates/step.html`

 * *Files identical despite different names*

### Comparing `pytest_bdd_report-1.0.1/src/pytest_bdd_report/templates/html_templates/summary.html` & `pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/templates/html_templates/summary.html`

 * *Files identical despite different names*

### Comparing `pytest_bdd_report-1.0.1/src/pytest_bdd_report/templates/report_template.py` & `pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/templates/report_template.py`

 * *Files identical despite different names*

### Comparing `pytest_bdd_report-1.0.1/src/pytest_bdd_report/templates/scenario_template.py` & `pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/templates/scenario_template.py`

 * *Files identical despite different names*

### Comparing `pytest_bdd_report-1.0.1/src/pytest_bdd_report/templates/summary_template.py` & `pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/templates/summary_template.py`

 * *Files identical despite different names*

### Comparing `pytest_bdd_report-1.0.1/src/pytest_bdd_report/templates/template.py` & `pytest_bdd_report-1.0.2b0/src/pytest_bdd_report/templates/template.py`

 * *Files identical despite different names*

### Comparing `pytest_bdd_report-1.0.1/src/pytest_bdd_report.egg-info/PKG-INFO` & `pytest_bdd_report-1.0.2b0/src/pytest_bdd_report.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 Metadata-Version: 2.1
 Name: pytest_bdd_report
-Version: 1.0.1
+Version: 1.0.2b0
 Summary: A pytest-bdd plugin for generating useful and informative BDD test reports
 Author-email: Mattia Monti <mattiamonti2001@gmail.com>
 Project-URL: Homepage, https://github.com/mattiamonti/pytest-bdd-report
 Project-URL: Bug Tracker, https://github.com/mattiamonti/pytest-bdd-report/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: pytest>=7.1.3
-Requires-Dist: pytest-bdd>=6.1.1
+Requires-Dist: pytest-bdd<7.0.0,>=5.0.0
 Requires-Dist: Jinja2>=3.1.2
 
 =================
 pytest-bdd-report
 =================
 
-|python| |pypi| |formatting| |tests|
+|python| |pypi| |formatting| |tests| |ui_tests|
 
-|dstats| |mstats|
+|mstats| |total|
 
+.. |total| image:: https://static.pepy.tech/badge/pytest-bdd-report
+    :target: https://pepy.tech/project/pytest-bdd-report
+    :alt: PePy total downloads
 
 .. |pypi| image:: https://img.shields.io/pypi/v/pytest-bdd-report.svg
     :target: https://pypi.org/project/pytest-bdd-report
     :alt: PyPI version
 
 .. |python| image:: https://img.shields.io/pypi/pyversions/pytest-bdd-report.svg
     :target: https://pypi.org/project/pytest-bdd-report
@@ -34,26 +37,31 @@
 
 .. |formatting| image:: https://img.shields.io/github/actions/workflow/status/mattiamonti/pytest-bdd-report/automated%20tests.yml?logo=GitHub%20actions&label=Formatting
     :alt: GitHub Workflow Status (with event)
 
 .. |tests| image:: https://img.shields.io/github/actions/workflow/status/mattiamonti/pytest-bdd-report/automated%20tests.yml?logo=pytest&label=Tests
     :alt: GitHub Workflow Status (with event)
 
+.. |ui_tests| image:: https://img.shields.io/github/actions/workflow/status/mattiamonti/pytest-bdd-report/ui%20automated%20tests.yml?logo=robotframework&label=UI%20Tests
+    :alt: GitHub Workflow Status (with event)
+
 .. |mstats| image:: https://img.shields.io/pypi/dm/pytest-bdd-report
    :alt: PyPI - Downloads
 
 .. |dstats| image:: https://img.shields.io/pypi/dd/pytest-bdd-report
    :alt: PyPI - Downloads
 
 
 
-The `pytest-bdd-report` plugin is a useful extension for the `pytest-bdd`_ library that allows you to generate 
+The `pytest-bdd-report` plugin is a useful extension for the `pytest-bdd`_ library that allows you to generate
 useful and informative reports for BDD (Behavior-Driven Development) tests developed using the pytest-bdd framework.
 This plugin facilitates the generation of clear and effective HTML reports, providing a comprehensible view of BDD test executions within the project.
 
+For more, check out the `Documentation`_
+
 ----
 
 This `pytest`_ plugin was generated with `Cookiecutter`_ along with `@hackebrot`_'s `cookiecutter-pytest-plugin`_ template.
 
 
 Features
 --------
@@ -109,20 +117,27 @@
 3. Install the plugin locally:
 
 ::
 
     $ pip install -e .
 
 
-4. Run the tests:
+4. Run the unit tests:
 
 ::
 
     $ python -m pytest
 
+5. Run the UI tests with Robot Framework:
+
+::
+
+    $ cd tests/ui_testing
+    $ ./execute_all_ui_tests.sh
+
 
 Contributing
 ------------
 Contributions are very welcome. Tests can be run with `pytest`_ as shown.
 
 License
 -------
@@ -144,7 +159,8 @@
 .. _`cookiecutter-pytest-plugin`: https://github.com/pytest-dev/cookiecutter-pytest-plugin
 .. _`file an issue`: https://github.com/mattiamonti/pytest-bdd-report/issues
 .. _`pytest`: https://github.com/pytest-dev/pytest
 .. _`tox`: https://tox.readthedocs.io/en/latest/
 .. _`pip`: https://pypi.org/project/pip/
 .. _`PyPI`: https://pypi.org/project
 .. _`pytest-bdd`: https://github.com/pytest-dev/pytest-bdd
+.. _`Documentation`: https://mattia-monti.gitbook.io/pytest-bdd-report/
```

### Comparing `pytest_bdd_report-1.0.1/src/pytest_bdd_report.egg-info/SOURCES.txt` & `pytest_bdd_report-1.0.2b0/src/pytest_bdd_report.egg-info/SOURCES.txt`

 * *Files identical despite different names*

