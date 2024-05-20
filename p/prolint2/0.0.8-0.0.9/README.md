# Comparing `tmp/prolint2-0.0.8.tar.gz` & `tmp/prolint2-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prolint2-0.0.8.tar", last modified: Mon Mar 27 21:45:22 2023, max compression
+gzip compressed data, was "prolint2-0.0.9.tar", last modified: Wed Jun 14 16:55:08 2023, max compression
```

## Comparing `prolint2-0.0.8.tar` & `prolint2-0.0.9.tar`

### file list

```diff
@@ -1,61 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:45:22.390018 prolint2-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-03-27 21:45:12.000000 prolint2-0.0.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-03-27 21:45:12.000000 prolint2-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-27 21:45:12.000000 prolint2-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-03-27 21:45:22.390018 prolint2-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-03-27 21:45:12.000000 prolint2-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:45:22.374018 prolint2-0.0.8/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3209 2023-03-27 21:45:12.000000 prolint2-0.0.8/bin/prolint2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:45:22.390018 prolint2-0.0.8/prolint2/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-27 21:45:22.390018 prolint2-0.0.8/prolint2/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/config.ini
--rw-r--r--   0 runner    (1001) docker     (123)    16840 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/contacts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:45:22.378018 prolint2-0.0.8/prolint2/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/data/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)  1643625 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/data/coordinates.gro
--rw-r--r--   0 runner    (1001) docker     (123)   966276 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/data/trajectory.xtc
--rw-r--r--   0 runner    (1001) docker     (123)    13222 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/interactive_sel.py
--rw-r--r--   0 runner    (1001) docker     (123)    12908 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/prolint2.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/sampledata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:45:22.382018 prolint2-0.0.8/prolint2/server/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/server/app.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     9469 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/server/chord_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/server/get_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    71086 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/server/girk.json
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/server/home.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/server/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    12153 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:45:22.374018 prolint2-0.0.8/prolint2/server/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:45:22.382018 prolint2-0.0.8/prolint2/server/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/server/static/css/main.css
--rw-r--r--   0 runner    (1001) docker     (123)    66916 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/server/static/css/pdbe-molstar-3.1.0_vendor.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:45:22.382018 prolint2-0.0.8/prolint2/server/static/images/
--rwxr-xr-x   0 runner    (1001) docker     (123)    12211 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/server/static/images/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:45:22.386018 prolint2-0.0.8/prolint2/server/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/server/static/js/app.js
--rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/server/static/js/ganttApp.js
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/server/static/js/heatmapApp.js
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/server/static/js/mol.js
--rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/server/static/js/network.js
--rw-r--r--   0 runner    (1001) docker     (123)  4346110 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/server/static/js/pdbe-molstar-plugin-3.1.0_vendor.js
--rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/server/static/js/pie.js
--rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/server/static/js/radialApp.js
--rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/server/static/js/table.js
--rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/server/static/js/timeseries.js
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/server/static/js/utils.js
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/server/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:45:22.390018 prolint2-0.0.8/prolint2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/tests/test_contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/tests/test_prolint2.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/tests/test_sampledata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:45:22.374018 prolint2-0.0.8/prolint2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-03-27 21:45:22.000000 prolint2-0.0.8/prolint2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-03-27 21:45:22.000000 prolint2-0.0.8/prolint2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 21:45:22.000000 prolint2-0.0.8/prolint2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-27 21:45:22.000000 prolint2-0.0.8/prolint2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-27 21:45:22.000000 prolint2-0.0.8/prolint2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-03-27 21:45:22.390018 prolint2-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-03-27 21:45:12.000000 prolint2-0.0.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68277 2023-03-27 21:45:12.000000 prolint2-0.0.8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:55:08.064166 prolint2-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-06-14 16:54:57.000000 prolint2-0.0.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-14 16:54:57.000000 prolint2-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-14 16:54:57.000000 prolint2-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-06-14 16:55:08.064166 prolint2-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-06-14 16:54:57.000000 prolint2-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:55:08.040166 prolint2-0.0.9/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3273 2023-06-14 16:54:57.000000 prolint2-0.0.9/bin/prolint2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:55:08.064166 prolint2-0.0.9/prolint2/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-14 16:55:08.064166 prolint2-0.0.9/prolint2/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:55:08.044166 prolint2-0.0.9/prolint2/computers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/computers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/computers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/computers/contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/computers/distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/computers/payload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:55:08.044166 prolint2-0.0.9/prolint2/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/config/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/config.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:55:08.044166 prolint2-0.0.9/prolint2/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/core/contact_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/core/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/core/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/core/universe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:55:08.048166 prolint2-0.0.9/prolint2/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/data/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1643625 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/data/coordinates.gro
+-rw-r--r--   0 runner    (1001) docker     (123)   966276 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/data/trajectory.xtc
+-rw-r--r--   0 runner    (1001) docker     (123)    13222 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/interactive_sel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:55:08.052166 prolint2-0.0.9/prolint2/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/metrics/aprox_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/metrics/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/metrics/exact_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/metrics/fitters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/metrics/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/metrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/metrics/registries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/metrics/restime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/metrics/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/sampledata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:55:08.052166 prolint2-0.0.9/prolint2/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/server/chord_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/server/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14943 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:55:08.040166 prolint2-0.0.9/prolint2/server/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:55:08.052166 prolint2-0.0.9/prolint2/server/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/server/static/css/main.css
+-rw-r--r--   0 runner    (1001) docker     (123)    66916 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/server/static/css/pdbe-molstar-3.1.0_vendor.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:55:08.052166 prolint2-0.0.9/prolint2/server/static/images/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12211 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/server/static/images/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:55:08.060166 prolint2-0.0.9/prolint2/server/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/server/static/js/app.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/server/static/js/ganttApp.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/server/static/js/heatmapApp.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/server/static/js/mol.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/server/static/js/network.js
+-rw-r--r--   0 runner    (1001) docker     (123)  4346110 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/server/static/js/pdbe-molstar-plugin-3.1.0_vendor.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/server/static/js/pie.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/server/static/js/radialApp.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/server/static/js/table.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/server/static/js/timeseries.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/server/static/js/utils.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/server/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:55:08.060166 prolint2-0.0.9/prolint2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/tests/test_sampledata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:55:08.060166 prolint2-0.0.9/prolint2/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-14 16:54:57.000000 prolint2-0.0.9/prolint2/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:55:08.044166 prolint2-0.0.9/prolint2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-06-14 16:55:08.000000 prolint2-0.0.9/prolint2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-14 16:55:08.000000 prolint2-0.0.9/prolint2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 16:55:08.000000 prolint2-0.0.9/prolint2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-14 16:55:08.000000 prolint2-0.0.9/prolint2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-14 16:55:08.000000 prolint2-0.0.9/prolint2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-14 16:55:08.064166 prolint2-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-14 16:54:57.000000 prolint2-0.0.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68277 2023-06-14 16:54:57.000000 prolint2-0.0.9/versioneer.py
```

### Comparing `prolint2-0.0.8/CODE_OF_CONDUCT.md` & `prolint2-0.0.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.8/LICENSE` & `prolint2-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.8/PKG-INFO` & `prolint2-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prolint2
-Version: 0.0.8
+Version: 0.0.9
 Summary: ProLint2: Lipid-Protein Interaction Analysis.
 Home-page: https://github.com/ProLint/prolint2
 Author: Daniel P. Ramirez & Besian I. Sejdiu
 Author-email: daniel.ramirezecheme@ucalgary.ca
 License: MIT
 Platform: Linux
 Platform: Mac OS-X
```

### Comparing `prolint2-0.0.8/README.md` & `prolint2-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.8/bin/prolint2` & `prolint2-0.0.9/bin/prolint2`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 r"""Argument parser to use prolint2 from the command-line
 ======================================================
 :Authors: Daniel P. Ramirez & Besian I. Sejdiu
 :Year: 2022
 :Copyright: MIT License
 """
 
+import os
 import argparse
-import prolint2._version as vers
-from prolint2.server.server import start_server
 import configparser
+
 from prolint2 import get_config
-import os
+import prolint2._version as vers
+from prolint2.server.server import ProLintDashboard
+
 
 # Getting the config file
 config = configparser.ConfigParser(allow_no_value=True)
 config.read(get_config())
 parameters_config = config["Parameters"]
 
 # Creating the parser
@@ -114,11 +116,13 @@
     dest="e_file",
 )
 
 # Executing the parse_args() method
 args = prolint2_parser.parse_args()
 
 # Starting the server
-start_server(payload=args, reloader=False, i_bool=args.i_bool, e_file=args.e_file)
+# start_server(payload=args, reloader=False, i_bool=args.i_bool, e_file=args.e_file)
+app = ProLintDashboard()
+app.start_server(payload=args)
 import sys
 
 sys.exit()
```

### Comparing `prolint2-0.0.8/prolint2/__init__.py` & `prolint2-0.0.9/prolint2/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 """ProLint2: Lipid-Protein Interaction Analysis"""
 
 # Add imports here
 import os
-from .prolint2 import *
+from .core import Universe
+
 from .interactive_sel import *
 
 # Handle versioneer
 from ._version import get_versions
 
 versions = get_versions()
 __version__ = versions["version"]
 __git_revision__ = versions["full-revisionid"]
 del get_versions, versions
 
 # to get the paths relative to the root of the package
 _ROOT = os.path.abspath(os.path.dirname(__file__))
 
-
 def get_data():
     return os.path.join(_ROOT, "data")
 
-
 # to get the path to the config file
 def get_config():
     return os.path.join(_ROOT, "config.ini")
```

### Comparing `prolint2-0.0.8/prolint2/config.ini` & `prolint2-0.0.9/prolint2/config.ini`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.8/prolint2/data/README.md` & `prolint2-0.0.9/prolint2/data/README.md`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.8/prolint2/data/coordinates.gro` & `prolint2-0.0.9/prolint2/data/coordinates.gro`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.8/prolint2/data/trajectory.xtc` & `prolint2-0.0.9/prolint2/data/trajectory.xtc`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.8/prolint2/interactive_sel.py` & `prolint2-0.0.9/prolint2/interactive_sel.py`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.8/prolint2/sampledata.py` & `prolint2-0.0.9/prolint2/sampledata.py`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.8/prolint2/server/chord_utils.py` & `prolint2-0.0.9/prolint2/server/chord_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,46 @@
 #!/usr/bin/env python
 
 from inspect import ArgSpec
 import numpy as np
 from itertools import combinations
-from .utils import calculate_contact_intervals
+from prolint2.server.utils import calculate_contact_intervals
 
-def per_lipid_contacts(ts, lipids, frame_cutoff=10):
-    """
-    Given a list of lipid IDs, returns a dict with these lipid IDs
-    as keys, and values set to a dict containing the residues these lipids
-    interact with as keys and the corresponding number of contacts as values.
-    These contacts can be filtered using the `frame_cutoff` option.
+# def per_lipid_contacts(ts, lipids, frame_cutoff=10):
+#     """
+#     Given a list of lipid IDs, returns a dict with these lipid IDs
+#     as keys, and values set to a dict containing the residues these lipids
+#     interact with as keys and the corresponding number of contacts as values.
+#     These contacts can be filtered using the `frame_cutoff` option.
+
+#     TODO:
+#     `frame_cutoff` should operate on a percentage of trajectory length.
+#     """
+#     results = {k: {} for k in lipids}
+#     for k, v in ts.contacts.contact_frames.items():
+#         if len(v) < frame_cutoff:
+#             continue
+#         # r, l = [int(x) for x in k.split(',')] # k used to be a string formatted as 'residue,lipid'
+#         # k now is a tuple of (residue, lipid)
+#         r, l = k
+#         if l in lipids:
+#             results[l][r] = len(v)
+#     return results
 
-    TODO:
-    `frame_cutoff` should operate on a percentage of trajectory length.
-    """
+def per_lipid_contacts(ts, lipids, frame_cutoff=10):
     results = {k: {} for k in lipids}
-    for k, v in ts.contacts.contact_frames.items():
-        if len(v) < frame_cutoff:
-            continue
-        r, l = [int(x) for x in k.split(',')]
-        if l in lipids:
-            results[l][r] = len(v)
+    for residue_id, lipid_dict in ts.contacts.contact_frames.items():
+        for lipid_id, frames in lipid_dict.items():
+            if len(frames) < frame_cutoff:
+                continue
+            if lipid_id in lipids:
+                results[lipid_id][residue_id] = len(frames)
     return results
 
+
 def sort_dict(d, cutoff=None):
     """
     Takes a dictionary as input, and sorts it according to values.
     The purpose of this function is to order residue:contacts dicts build
     by `per_lipid_contacts` function according to the number of contacts.
 
     The `cutoff` value returns only a subsection of this dict. The cutoff
@@ -94,25 +107,25 @@
             if key in ordered_combinations:
                 ordered_combinations[key] = ordered_combinations[key] + value
             else:
                 ordered_combinations[key] = value
 
     return ordered_combinations
 
-def shared_contacts(ts, top_lipids, lipid_contact_frames, *args, **kwargs):
+def shared_contacts(contacts, top_lipids, lipid_contact_frames, *args, **kwargs):
     """
     Aim: improve the shortcomings outlined in `get_ordered_combinations`.
     """
     lipid_shared_contacts = {}
     for lipid in top_lipids:
-        contact_intervals = calculate_contact_intervals(ts, lipid_contact_frames, lipid, *args, **kwargs)
+        contact_intervals = calculate_contact_intervals(contacts, lipid_contact_frames, lipid, *args, **kwargs)
         residue_contacts = {}
         for res1, res2 in combinations(contact_intervals.keys(), 2):
-            contacts = residue_pair_matching_contacts(contact_intervals[res1], contact_intervals[res2])
-            residue_contacts[f'{res1},{res2}'] = contacts
+            pair_contacts = residue_pair_matching_contacts(contact_intervals[res1], contact_intervals[res2])
+            residue_contacts[f'{res1},{res2}'] = pair_contacts
         lipid_shared_contacts[lipid] = residue_contacts
 
     shared_contacts_all = {}
     for residue_pair_contacts in lipid_shared_contacts.values():
         for residue_pair, pair_contacts in residue_pair_contacts.items():
             if residue_pair in shared_contacts_all:
                 shared_contacts_all[residue_pair] += pair_contacts
@@ -163,16 +176,16 @@
     The output is a simple list of dicts. Each entry containing info for
     one link. We also add residue ID and residue name information which is
     important to link node data with other apps.
     """
     node_links = list(combinations(nodes, 2))
     position_node_links = [x for x in node_links if x[0] == 0]
 
-    resnums = ts.query.selected.residues.resnums
-    resnames = ts.query.selected.residues.resnames
+    resnums = ts.query.residues.resnums
+    resnames = ts.query.residues.resnames
     node_names = {x[0]: f'{x[0]} {x[1]}' for x in list(zip(resnums, resnames))}
 
     chord_elements = []
     for res1, res2 in position_node_links:
         chord_elements.append({
             "from": 0,
             "to": node_names[res2],
@@ -192,37 +205,37 @@
             "to": node_names[int(res2)],
             "value": v,
             "valueWidth": float(v) / contact_max
         })
 
     return chord_elements
 
-def contact_chord(ts, top_lipid_ids, lipid_contact_frames, cutoff=100):
+def contact_chord(ts, contacts, top_lipid_ids, lipid_contact_frames, cutoff=100):
     """
     We call all functions here. We return the chord elements (these are the data
     amCharts needs to render nodes and links), we also return information on which
     nodes to hide, and which nodes correspond to which lipid ID.
 
     TODO:
     `per_lipid_nodes` can be further refined.
     """
     # lipid_contacts = per_lipid_contacts(ts, top_lipid_ids)
     lipid_shared_contacts, ordered_combinations = shared_contacts(
-        ts,
+        contacts,
         top_lipid_ids,
         lipid_contact_frames,
         residues_to_show=30,
         intervals_to_filter_out=10
         )
     # ordered_combinations = get_ordered_combinations(lipid_contacts)
     linked_nodes = get_linked_nodes(ordered_combinations, cutoff=cutoff)
-    nodes, hidden_node_indices = get_node_list(ts.query.selected.n_residues, linked_nodes)
+    nodes, hidden_node_indices = get_node_list(ts.query.n_residues, linked_nodes)
     chord_elements = get_chord_elements(ts, nodes, ordered_combinations, cutoff=cutoff)
 
     per_lipid_nodes = {}
     for lipid, pair_contacts in lipid_shared_contacts.items():
         lipid_nodes = get_linked_nodes(pair_contacts, cutoff=None)
         all_lipid_nodes = [x for x in lipid_nodes if x in linked_nodes]
         if all_lipid_nodes:
             per_lipid_nodes[lipid] = all_lipid_nodes
 
-    return chord_elements, hidden_node_indices, per_lipid_nodes
+    return chord_elements, hidden_node_indices, per_lipid_nodes
```

### Comparing `prolint2-0.0.8/prolint2/server/index.html` & `prolint2-0.0.9/prolint2/server/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,27 @@
                 <div id="chartdiv3"></div>
             </div>
             <div class="col-sm-5" style="background-color: white;">
                 <div id="chartdiv4"></div>
             </div>
         </div>
         <div class="row">
+            <div class="col-sm-7" style="background-color: white; position: relative; height: 50px; margin-top: 20px">
+                <div class="dropdown-wrapper">
+                    <span class="dropdown-label">Select contact metric</span>
+                    <select id="metric_button" class="custom-dropdown">
+                      <option value="sum" selected>Sum of all contacts</option>
+                      <option value="mean">Mean of contacts</option>
+                      <option value="max">Longest contact</option>
+                    </select>
+                  </div>
+            </div>
+        </div>
+
+        <div class="row">
             <div id="chartdiv" class="col-sm-7" style="background-color: white; position: relative;">
               <div id="chartdiv_z" style="width: 100%; height: 100%; position: absolute; padding-top: 30px;"></div>
               <div id="chartdiv_y" style="width: 100%; height: 100%; position: absolute; padding-top: 20px"></div>
               <div id="chartdiv_x" style="width: 100%; height: 100%; position: absolute; padding-top: 15px;"></div>
               <button id="button_x" style="position: absolute; top: 20; left: 45%; --c: #373B44; --s:3px" data-app="app_x">Radial App</button>
               <button id="button_y" style="position: absolute; top: 20; right: 0; --c: #373B44; --s:3px" data-app="app_y">Shared Contacts</button>
               <button id="button_z" style="position: absolute; top: 20; left: 0; --c: #373B44; --s:3px" data-app="app_z">Time Series</button>
```

#### html2text {}

```diff
@@ -1,3 +1,5 @@
 [ProLint Logo]
 ************ PPrrooLLiinntt22 DDaasshhbbooaarrdd ************
+Select contact metric[One of: Sum of all contacts/Mean of contacts/Longest
+contact]
 Radial App Shared Contacts Time Series
```

### Comparing `prolint2-0.0.8/prolint2/server/server.py` & `prolint2-0.0.9/prolint2/server/server.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,424 +1,410 @@
-from collections import Counter
-from prolint2.interactive_sel import interactive_selection
 import os
 import ast
-import json
-
-from bottle import route, run, template, debug, static_file, request
-from prolint2.contacts import SerialDistances
+from io import StringIO
+from collections import Counter
 
 import MDAnalysis as mda
-from prolint2.prolint2 import PL2
-from io import StringIO
+from bottle import Bottle, redirect, static_file
 
-from .chord_utils import contact_chord
+from prolint2.core.universe import Universe
+from prolint2.server.chord_utils import contact_chord
+from prolint2.interactive_sel import interactive_selection
+from prolint2.computers.payload import ServerPayload
+from prolint2.computers.distances import SerialDistances
 
 SERVER_PATH = os.path.abspath(os.path.dirname(__file__))
 
-BACKEND_DATA = None
-TS = None
-ARGS = None
-data = None
-data_loaded = False
-
-
-def sort_lipids(ts):
+class ProLintDashboard:
     """
-    Sort lipid contacts according to their contact frequency, all the while keeping track
-    of residue IDs, and number of contacts with each residue.
-
-    Returns:
-        t (dict): Stores lipid IDs and their contact frequency, sorted in descending order
-        g (dict): For each lipid ID, stores the residues in contact and the corresponding
-                  frequency.
+    A dashboard for ProLint2. It is a fully functional web application that can be used to
+    visualize the results of the ProLint2 analysis.
     """
-
-    def sort_tuple(tup):
-        tup.sort(key=lambda x: x[1], reverse=True)
-        return tup
-
-    # TODO:
-    # top lipid number should be put in the config.
-    contact_threshold = ts.n_frames * 0.05
-
-    # initialize dictionary to store values:
-    t = {k: {} for k in ts.database_unique}
-    g = {}
-    for ix, (residue, lipid_contacts) in enumerate(ts.contacts.contacts.items()):
-        for lipid, contact_counter in lipid_contacts.items():
-            top10_counter = contact_counter.most_common()
-            for (lipid_id, lipid_counter) in top10_counter:
-                # Exclude short-lived contacts
-                if lipid_counter <= contact_threshold:
+    def __init__(self, port=8351, debug_bool=False, reloader=False):
+        self.backend_data = None
+        self.ts = None
+        self.contacts = None
+        self.payload = None
+        self.args = None
+        self.data = None
+        self.data_loaded = False
+        self.port = port
+        self.debug_bool = debug_bool
+        self.reloader = reloader
+        self.response = None
+        self.app = Bottle()
+        self.setup_routes()
+
+    def setup_routes(self):
+        """
+            Setup the routes for the dashboard.
+        """
+        self.app.route("/", method="GET", callback=self.redirect_to_app)
+        self.app.route("/app", method="GET", callback=self.serve_app)
+        self.app.route("/static/<filepath:path>", method="GET", callback=self.server_static)
+        self.app.route("/data/<metadata>", method="GET", callback=self.serve_data)
+        self.app.route("/pdb/<metadata>", method="GET", callback=self.serve_pdb)
+        self.app.route("/network/<metadata>", method="GET", callback=self.serve_network)
+        self.app.route("/tabledata/<metadata>", method="GET", callback=self.serve_table_data)
+        self.app.route("/toplipids/<metadata>", method="GET", callback=self.serve_top_lipids)
+        self.app.route("/distance/<metadata>", method="GET", callback=self.serve_distance_array)
+        self.app.route("/metric/<metadata>", method="GET", callback=self.update_metric)
+
+    def serve_app(self):
+        """
+            Serve the main application.
+        """
+        return static_file("index.html", root=SERVER_PATH)
+
+    def server_static(self, filepath):
+        """
+            Serve static files.
+        """
+        return static_file(filepath, root=os.path.join(SERVER_PATH, "static"))
+
+    def redirect_to_app(self):
+        """
+            Redirect to the main application.
+        """
+        redirect("/app")
+
+    def serve_pdb(self, metadata):
+        """
+            Serve the PDB file to the client for use with Mol*.
+        """
+        u = mda.Universe(self.args.structure, self.args.trajectory)
+        protein = u.select_atoms("protein")
+        pstream = mda.lib.util.NamedStream(StringIO(), "dummy.pdb")
+        with mda.Writer(pstream, format="PDB") as w:
+            w.write(protein)
+
+        return pstream.read()
+
+    def get_gantt_app_data(self, g, lipid_id, residues_to_show=15, intervals_to_filter_out=10):
+        """
+        Get the data for the Gantt chart in the application.
+
+        Args:
+            g (dict): For each lipid ID, stores the residues in contact and the corresponding
+                    frequency.
+            lipid_id (str): The lipid ID to use.
+            residues_to_show (int): The number of residues to show in the Gantt chart.
+            intervals_to_filter_out (int): The number of frames to filter out.
+
+        Returns:
+            gantt_data (list): A list of dictionaries containing the data for the Gantt chart.
+            categories (list): A list of residue IDs.
+        """
+
+        gantt_data = []
+        for res, _ in g[lipid_id][:residues_to_show]:
+            frame_numbers = self.contacts.contact_frames[res][lipid_id]
+            frame_intervals = self.get_frame_contact_intervals(frame_numbers)
+            for start, end in frame_intervals:
+                if end - start < intervals_to_filter_out:
                     continue
-                if lipid_id in t[lipid]:
-                    t[lipid][lipid_id] += lipid_counter
-                    g[lipid_id].append((residue, lipid_counter))
-                else:
-                    t[lipid][lipid_id] = lipid_counter
-                    g[lipid_id] = [(residue, lipid_counter)]
-
-    for lipid, values in t.items():
-        t[lipid] = Counter(values).most_common()
+                gantt_data.append(
+                    {
+                        "category": res,
+                        "startFrame": start,
+                        "endFrame": end,
+                        "lipid_id": lipid_id,
+                    }
+                )
+
+        # TODO:
+        # `categories` is now just the `gantt_data` keys.
+        # replace with: `list(gantt_data.keys())` or remove entirely
+        categories = []
+        for y in [x["category"] for x in gantt_data]:
+            if y not in categories:
+                categories.append(y)
+        return gantt_data, categories
+
+    def sort_lipids(self):
+        """
+        Sort lipid contacts according to their contact frequency, all the while keeping track
+        of residue IDs, and number of contacts with each residue.
+
+        Args:
+            ts (PL2): The ProLint2 object.
+
+        Returns:
+            lipid_frequency (dict): Stores lipid IDs and their contact frequency, sorted in descending order
+            residue_contact_freq (dict): For each lipid ID, stores the residues in contact and the corresponding
+                    frequency.
+                    
+        """
+
+        def sort_by_frequency(contact_list):
+            contact_list.sort(key=lambda x: x[1], reverse=True)
+            return contact_list
+
+        # TODO:
+        # top lipid number should be put in the config.
+        # contact_threshold = self.ts.trajectory.n_frames * 0.05
+        contact_threshold = 0
+
+        # Initialize dictionaries to store values:
+        lipid_frequency = {lipid: {} for lipid in self.ts.database.unique_resnames}
+        residue_contact_freq = {}
+
+        for residue, lipid_contacts in self.contacts.compute_metric('sum').items():
+            for lipid, contact_counter in lipid_contacts.items():
+                # Sort the contact_counter dictionary by its values
+                sorted_contacts = sorted(contact_counter.items(), key=lambda x: x[1], reverse=True)
+
+                for lipid_id, freq in sorted_contacts:
+                    # Exclude short-lived contacts
+                    if freq <= contact_threshold:
+                        continue
+
+                    # Update lipid_frequency
+                    if lipid_id in lipid_frequency[lipid]:
+                        lipid_frequency[lipid][int(lipid_id)] += freq
+                    else:
+                        lipid_frequency[lipid][int(lipid_id)] = freq
+
+                    # Update residue_contact_freq
+                    if int(lipid_id) in residue_contact_freq:
+                        residue_contact_freq[int(lipid_id)].append((int(residue), freq))
+                    else:
+                        residue_contact_freq[int(lipid_id)] = [(int(residue), freq)]
+
+        for lipid, values in lipid_frequency.items():
+            lipid_frequency[lipid] = Counter(values).most_common()
+
+        for lipid_id, vals in residue_contact_freq.items():
+            residue_contact_freq[lipid_id] = sort_by_frequency(vals)
+
+        return lipid_frequency, residue_contact_freq
+
+
+    @staticmethod
+    def get_frame_contact_intervals(frames, tolerance=6):
+        """
+        Get the intervals of frames in which a contact is present.
+
+        Args:
+            frames (list): A list of frames in which a contact is present.
+            tolerance (int): The number of frames to tolerate before considering a new interval.
+
+        Returns:
+            ranges_collect (list): A list of tuples containing the start and end frames of each
+                interval.
+
+        """
+        ranges_collect = []
+        range_start = 0
+        for ix, el in enumerate(frames):
+            if ix == 0:
+                range_start = el
+                continue
 
-    # for lipid, values in g.items():
-    for lipid_id, vals in g.items():
-        g[lipid_id] = sort_tuple(vals)
+            prev_el = frames[ix - 1]
+            if not el - tolerance <= prev_el:
+                ranges_collect.append((range_start, prev_el))
+                range_start = el
+            if ix == len(frames) - 1:
+                ranges_collect.append((range_start, el))
+        return ranges_collect
+
+    def serve_data(self, metadata):
+        """
+            Serve the data to the client for use with the application.
+        """
+
+        metadata = ast.literal_eval(metadata)
+
+        lipid = metadata["lipid"]
+        protein = metadata["protein"]
+        metric = metadata.get('metric', '')
+
+        if lipid == "" and protein == "":
+            # Starting setup:
+            lipid = self.backend_data["lipids"][0]
+            protein = self.backend_data["proteins"][0]
+
+        table_data = []
+        for ix, (lipid_id, freq) in enumerate(self.backend_data["top_lipids"][lipid]):
+            table_data.append({"id": ix, "lipidID": lipid_id, "contactFrequency": freq})
+
+        # Initiate ganttApp with the top lipid data
+        lipid_id = self.backend_data["top_lipids"][lipid][0][0]
+        gantt_data, categories = self.get_gantt_app_data(
+            self.backend_data["lipid_contact_frames"], lipid_id
+        )
 
-    return t, g
+        # Initiate heatmapApp with the top residue
+        residue_id = self.backend_data["lipid_contact_frames"][lipid_id][0][0]
+        ri = SerialDistances(
+            self.ts.query.universe,
+            self.ts.query,
+            self.ts.database,
+            lipid_id,
+            residue_id,
+            self.contacts.contact_frames[residue_id][lipid_id],
+        )
+        ri.run(verbose=False)
 
+        hm_data, la_data = [], []
+        for lx, la in enumerate(ri.lipid_atomnames):
+            la_data.append({"LipidAtoms": la})
+            for rx, ra in enumerate(ri.resid_atomnames):
+                v = ri.distance_array[lx, rx]
+                hm_data.append({"LipidAtoms": la, "ResidueAtoms": ra, "value": float(v)})
+        ra_data = [{"ResidueAtoms": x} for x in ri.resid_atomnames]
+
+        # TODO:
+        # Possibly, avoid single point of failure on these dictionary lookups?
+        response = {
+            "data": self.backend_data["data"][protein][lipid],
+            "proteins": self.backend_data["proteins"],
+            "lipids": self.backend_data["lipids"],
+            "pieData": self.backend_data["pie_data"],
+            "ganttData": gantt_data,
+            "topLipids": categories,
+            "globalTopLipids": self.backend_data["top_lipids"],
+            "lipidContactFrames": self.backend_data["lipid_contact_frames"],
+            "tableData": table_data,
+            "heatmapData": hm_data,
+            "lipidAtomsData": la_data,
+            "residueAtomsData": ra_data,
+            "frameNumber": self.ts.trajectory.n_frames,
+        }
+        self.response = response
+        return response
 
-def get_frame_contact_intervals(frames, tolerance=6):
-    """
-    Get frame ranges
-    """
-    ranges_collect = []
-    range_start = 0
-    for ix, el in enumerate(frames):
-        if ix == 0:
-            range_start = el
-            continue
-
-        prev_el = frames[ix - 1]
-        if not el - tolerance <= prev_el:
-            ranges_collect.append((range_start, prev_el))
-            range_start = el
-        if ix == len(frames) - 1:
-            ranges_collect.append((range_start, el))
-    return ranges_collect
-
-
-def get_gantt_app_data(g, lipid_id, residues_to_show=15, intervals_to_filter_out=10):
-    gantt_data = []
-    for res, _ in g[lipid_id][:residues_to_show]:
-        frame_numbers = TS.contacts.contact_frames[f"{res},{lipid_id}"]
-        frame_intervals = get_frame_contact_intervals(frame_numbers)
-        for start, end in frame_intervals:
-            if end - start < intervals_to_filter_out:
-                continue
-            gantt_data.append(
-                {
-                    # "category": f'{res}',
-                    "category": res,
-                    "startFrame": start,
-                    "endFrame": end,
-                    "lipid_id": lipid_id,
-                }
+    def update_metric(self, metadata):
+        """
+            Update the metric used for the backend data.
+        """
+        metadata = ast.literal_eval(metadata)
+        
+        lipid = metadata["lipid"]
+        metric = metadata["metric"]
+
+        residue_contacts = self.payload.residue_contacts(lipid_type=lipid, metric=metric)
+        
+        self.response['data'] = residue_contacts[lipid]
+        return self.response
+
+
+    def serve_network(self, metadata):
+        """
+            Serve the data to the client for use with the network application.
+        """
+        metadata = ast.literal_eval(metadata)
+        lipid = metadata['lipid']
+
+        top_lipid_ids = [x[0] for x in self.backend_data['top_lipids'][lipid]]
+        chord_elements, hidden_node_indices, per_lipid_nodes = contact_chord(
+            self.ts,
+            self.contacts,
+            top_lipid_ids,
+            self.backend_data['lipid_contact_frames'],
+            cutoff=100
             )
 
-    # TODO:
-    # `categories` is now just the `gantt_data` keys.
-    # replace with: `list(gantt_data.keys())` or remove entirely
-    categories = []
-    for y in [x["category"] for x in gantt_data]:
-        if y not in categories:
-            categories.append(y)
-    return gantt_data, categories
-
-
-@route("/static/<filepath:path>")
-def server_static(filepath):
-    return static_file(filepath, root=os.path.join(SERVER_PATH, "static"))
-
-
-@route("/")
-def index():
-    return template(os.path.join(SERVER_PATH, "home.tpl"))
-
-
-@route("/app")
-def app():
-    return static_file("index.html", root=SERVER_PATH)
-
-
-@route("/prolint2")
-def prolint2():
-    import sys
-
-    print(request.body.getvalue().decode("utf-8"), file=sys.stdout)
-    return request.body
-
-
-@route("/toplipids/:metadata")
-def top_lipid_listener(metadata):
-    global BACKEND_DATA
-
-    metadata = ast.literal_eval(metadata)
-    lipid_id = metadata["lipidID"]
-
-    gantt_data, categories = get_gantt_app_data(
-        BACKEND_DATA["lipid_contact_frames"], lipid_id
-    )
-    # This will sort the residues
-    # sorted_gantt_data = sorted(gantt_data, key=lambda d: d['category'])
-
-    # ags = TS.query.selected.select_atoms(f'resid {" ".join([str(x) for x in categories])}')
-    # labeled_categories = [[int(x.resid), x.resname] for x in ags]
-    return {
-        "ganttData": gantt_data,
-        "topLipids": categories,
-    }
-
-
-@route("/distance/:metadata")
-def distance_array_listener(metadata):
-    global BACKEND_DATA
-    global TS
-
-    metadata = ast.literal_eval(metadata)
-    lipid_id = metadata["lipidID"]
-    residue_id = int(metadata["residueID"])
-
-    ri = SerialDistances(
-        TS.query.selected.universe,
-        TS.query.selected,
-        TS.database.selected,
-        lipid_id,
-        residue_id,
-        TS.contacts.contact_frames[f"{residue_id},{lipid_id}"],
-    )
-    ri.run(verbose=False)
-
-    hm_data, la_data = [], []
-    for lx, la in enumerate(ri.lipid_atomnames):
-        la_data.append({"LipidAtoms": la})
-        for rx, ra in enumerate(ri.resid_atomnames):
-            v = ri.distance_array[lx, rx]
-            hm_data.append({"LipidAtoms": la, "ResidueAtoms": ra, "value": float(v)})
-    ra_data = [{"ResidueAtoms": x} for x in ri.resid_atomnames]
-
-    return {
-        "heatmapData": hm_data,
-        "lipidAtomsData": la_data,
-        "residueAtomsData": ra_data,
-    }
-
-
-@route("/tabledata/:metadata")
-def table_listener(metadata):
-    global BACKEND_DATA
-
-    metadata = ast.literal_eval(metadata)
-    lipid = metadata["lipid"]
-
-    table_data = []
-    for ix, (lipid_id, freq) in enumerate(BACKEND_DATA["top_lipids"][lipid]):
-        table_data.append({"id": ix, "lipidID": lipid_id, "contactFrequency": freq})
-
-    return {
-        "tableData": table_data,
-    }
-
-
-@route("/pdb/:metadata")
-def blob(metadata):
-
-    global ARGS
-    u = mda.Universe(ARGS.structure, ARGS.trajectory)
-    protein = u.select_atoms("protein")
-    pstream = mda.lib.util.NamedStream(StringIO(), "dummy.pdb")
-    with mda.Writer(pstream, format="PDB") as w:
-        w.write(protein)
-
-    return pstream.read()
-
-@route('/network/:metadata')
-def network_listener(metadata):
-    global BACKEND_DATA
-    global TS
-
-    metadata = ast.literal_eval(metadata)
-    lipid = metadata['lipid']
-
-    top_lipid_ids = [x[0] for x in BACKEND_DATA['top_lipids'][lipid]]
-    chord_elements, hidden_node_indices, per_lipid_nodes = contact_chord(
-        TS,
-        top_lipid_ids,
-        BACKEND_DATA['lipid_contact_frames'],
-        cutoff=100
-        )
+        return {
+            "chordElements": chord_elements,
+            "positionResidues": hidden_node_indices,
+            "lipidNodes": per_lipid_nodes
+        }
+
+    def serve_table_data(self, metadata):
+        """
+            Serve the data to the client for use with the table application.
+        """
+        metadata = ast.literal_eval(metadata)
+        lipid = metadata["lipid"]
+
+        table_data = []
+        for ix, (lipid_id, freq) in enumerate(self.backend_data["top_lipids"][lipid]):
+            table_data.append({"id": ix, "lipidID": lipid_id, "contactFrequency": freq})
 
-    return {
-        "chordElements": chord_elements,
-        "positionResidues": hidden_node_indices,
-        "lipidNodes": per_lipid_nodes
-    }
-
-@route('/data/:metadata')
-def listener(metadata):
-
-    global data_loaded
-    global data
-    global BACKEND_DATA
-    global TS
-
-    # TODO:
-    # Bottle should provide the metadata already,
-    # perhaps via the following:
-    # from bottle import response, request
-    metadata = ast.literal_eval(metadata)
-
-    lipid = metadata["lipid"]
-    protein = metadata["protein"]
-
-    if lipid == "" and protein == "":
-        # Starting setup:
-        try:
-            lipid = BACKEND_DATA["lipids"][0]
-            protein = BACKEND_DATA["proteins"][0]
-        except:
-            print("Detached EXECUTION")
-            print("This is currently meant for testing only. Not guaranteed to work!")
-            BACKEND_DATA = independent_execution()
-            lipid = BACKEND_DATA["lipids"][0]
-            protein = BACKEND_DATA["proteins"][0]
-
-    table_data = []
-    for ix, (lipid_id, freq) in enumerate(BACKEND_DATA["top_lipids"][lipid]):
-        table_data.append({"id": ix, "lipidID": lipid_id, "contactFrequency": freq})
-
-    # Initiate ganttApp with the top lipid
-    lipid_id = BACKEND_DATA["top_lipids"][lipid][0][0]
-    gantt_data, categories = get_gantt_app_data(
-        BACKEND_DATA["lipid_contact_frames"], lipid_id
-    )
-
-    # Initiate heatmapApp with the top residue
-    residue_id = BACKEND_DATA["lipid_contact_frames"][lipid_id][0][0]
-    ri = SerialDistances(
-        TS.query.selected.universe,
-        TS.query.selected,
-        TS.database.selected,
-        lipid_id,
-        residue_id,
-        TS.contacts.contact_frames[f"{residue_id},{lipid_id}"],
-    )
-    ri.run(verbose=False)
-
-    hm_data, la_data = [], []
-    for lx, la in enumerate(ri.lipid_atomnames):
-        la_data.append({"LipidAtoms": la})
-        for rx, ra in enumerate(ri.resid_atomnames):
-            v = ri.distance_array[lx, rx]
-            hm_data.append({"LipidAtoms": la, "ResidueAtoms": ra, "value": float(v)})
-    ra_data = [{"ResidueAtoms": x} for x in ri.resid_atomnames]
-
-    # TODO:
-    # Possibly, avoid single point of failure on these dictionary lookups?
-    response = {
-        "data": BACKEND_DATA["data"][protein][lipid],
-        "proteins": BACKEND_DATA["proteins"],
-        "lipids": BACKEND_DATA["lipids"],
-        "pieData": BACKEND_DATA["pie_data"],
-        "ganttData": gantt_data,
-        "topLipids": categories,
-        "globalTopLipids": BACKEND_DATA["top_lipids"],
-        "lipidContactFrames": BACKEND_DATA["lipid_contact_frames"],
-        "tableData": table_data,
-        "heatmapData": hm_data,
-        "lipidAtomsData": la_data,
-        "residueAtomsData": ra_data,
-        "frameNumber": TS.n_frames,
-    }
-    return response
-
-
-def start_server(
-    payload=None, debug_bool=False, reloader=True, port=8351, i_bool=True, e_file=False
-):
-
-    global ARGS
-    # ProLint2 calls:
-    args = payload
-    ARGS = args
-    ts = PL2(args.structure, args.trajectory, add_lipid_types=args.other_lipids)
-    # For interactive selection of the groups for the contacts calculation
-    if i_bool:
-        ts = interactive_selection(ts)
-    ts.contacts.compute(cutoff=args.cutoff)
-
-    # for exporting the data
-    if e_file:
-        ts.contacts.export(args.e_file)
-
-    payload = ts.contacts.server_payload()
-
-    t, g = sort_lipids(ts)
-    payload["top_lipids"] = t
-    payload["lipid_contact_frames"] = g
-
-    # Make data accessible globally
-    global BACKEND_DATA
-    global TS
-    BACKEND_DATA = payload
-    TS = ts
+        return {
+            "tableData": table_data,
+        }
 
-    debug(debug_bool)
-    run(reloader=reloader, host="localhost", port=port)
+    def serve_top_lipids(self, metadata):
+        """
+            Serve the data to the client for use with the gantt application.
+        """
+        metadata = ast.literal_eval(metadata)
+        lipid_id = metadata["lipidID"]
 
+        gantt_data, categories = self.get_gantt_app_data(
+            self.backend_data["lipid_contact_frames"], lipid_id
+        )
 
-def independent_execution():
-    """
-    If we are not calling the server through the prolint2 executable, but
-    independently, locally for testing purposes, we will load local data file
-    and serve that to the dashboard.
-    """
-    with open(os.path.join(SERVER_PATH, "girk.json"), "r") as fp:
-        data = json.load(fp)
+        return {
+            "ganttData": gantt_data,
+            "topLipids": categories,
+        }
+
+    def serve_distance_array(self, metadata):
+        """
+            Serve the data to the client for use with the heatmap application.
+        """
+        metadata = ast.literal_eval(metadata)
+        lipid_id = metadata["lipidID"]
+        residue_id = int(metadata["residueID"])
+
+        ri = SerialDistances(
+            self.ts.query.universe,
+            self.ts.query,
+            self.ts.database,
+            lipid_id,
+            residue_id,
+            self.contacts.contact_frames[residue_id][lipid_id],
+        )
+        ri.run(verbose=False)
 
-    pie_data = [
-        {
-            "category": "LocalGirk",
-            "value": 500,
-            "subData": [
-                {"category": "CHOL", "value": 300},
-                {"category": "POPE", "value": 150},
-                {"category": "POPS", "value": 50},
-            ],
+        hm_data, la_data = [], []
+        for lx, la in enumerate(ri.lipid_atomnames):
+            la_data.append({"LipidAtoms": la})
+            for rx, ra in enumerate(ri.resid_atomnames):
+                v = ri.distance_array[lx, rx]
+                hm_data.append({"LipidAtoms": la, "ResidueAtoms": ra, "value": float(v)})
+        ra_data = [{"ResidueAtoms": x} for x in ri.resid_atomnames]
+
+        return {
+            "heatmapData": hm_data,
+            "lipidAtomsData": la_data,
+            "residueAtomsData": ra_data,
         }
-    ]
 
-    # ganttApp data input requirement
-    gantt_data = [
-        {
-            "category": "Lipid 1",
-            "startFrame": 0,
-            "endFrame": 10,
-        },
-        {
-            "category": "Lipid 1",
-            "startFrame": 45,
-            "endFrame": 75,
-        },
-        {
-            "category": "Lipid 1",
-            "startFrame": 90,
-            "endFrame": 100,
-        },
-        {
-            "category": "Lipid 2",
-            "startFrame": 10,
-            "endFrame": 35,
-        },
-        {
-            "category": "Lipid 2",
-            "startFrame": 45,
-            "endFrame": 60,
-        },
-    ]
-    top_10_lipids = ["Lipid 1", "Lipid 2"]
-
-    payload = {
-        "data": data,
-        "proteins": ["LocalGirk"],
-        "lipids": list(data["LocalGirk"].keys()),
-        "pie_data": pie_data,
-        "gantt_data": gantt_data,
-        "top_10_lipids": top_10_lipids,
-    }
+    def start_server(self, payload=None):
+        """
+            Start the server.
+        """
+        if payload is None:
+            import sys # pylint: disable=import-outside-toplevel
+            print ("Please provide a payload")
+            sys.exit(1)
+
+        self.args = payload
+        self.ts = Universe(self.args.structure, self.args.trajectory)
+
+        if self.args.i_bool:
+            self.ts = interactive_selection(self.ts)
+        self.contacts = self.ts.compute_contacts(cutoff=self.args.cutoff)
+
+        if self.args.e_file:
+            self.contacts.export(self.args.e_file)
+
+        # payload = self.contacts.server_payload()
+        self.payload = ServerPayload(self.contacts, self.ts)
+        payload = self.payload.payload
+
+        lipid_frequency, residue_contact_freq = self.sort_lipids()
+        payload["top_lipids"] = lipid_frequency
+        payload["lipid_contact_frames"] = residue_contact_freq
 
-    return payload
+        self.backend_data = payload
 
+        self.app.run(reloader=self.reloader, host="localhost", port=self.port, debug=self.debug_bool)
 
 if __name__ == "__main__":
-    start_server(debug_bool=True)
+    app = ProLintDashboard(debug_bool=True)
+    app.start_server()
```

### Comparing `prolint2-0.0.8/prolint2/server/static/css/main.css` & `prolint2-0.0.9/prolint2/server/static/css/main.css`

 * *Files 12% similar despite different names*

```diff
@@ -72,15 +72,36 @@
 display: grid;
 grid-template-columns: auto auto;
 gap: 20px;
 place-content: center;
 background: #DAEDFB;
 } */
 
-button {
+.dropdown-wrapper {
+  display: flex;
+  align-items: center;
+  top: 15px; 
+}
+
+.dropdown-label {
+  margin-right: 0.5em;
+  font-family: system-ui, sans-serif;
+  font-weight: bold;
+  font-size: 1.5rem;
+  color: var(--c);
+}
+
+.custom-dropdown {
+  width: 250px;
+  appearance: none;
+  /* Add the remaining styles from your previous custom-select rule */
+}
+
+
+button, select {
   --b: 1.5px; /* border thickness */
   --s: 0.02em; /* size of the corner */
   --c: #bd5532;
 
   padding: calc(0.05em + var(--s)) calc(0.3em + var(--s));
   color: var(--c);
   --_p: var(--s);
@@ -92,25 +113,41 @@
     var(--_p) var(--_p) / calc(100% - var(--b) - 2 * var(--_p))
     calc(100% - var(--b) - 2 * var(--_p));
   transition: 0.3s linear, color 0s, background-color 0s;
   outline: var(--b) solid #0000;
   outline-offset: 0.2em;
 }
 button:hover,
-button:focus-visible {
+button:focus-visible,
+select:hover,
+select:focus-visible {
   --_p: 0px;
   outline-color: var(--c);
   outline-offset: 0.05em;
 }
 button:active {
   background: var(--c);
   color: #fff;
 }
 
-button {
+button, select {
   font-family: system-ui, sans-serif;
   font-weight: bold;
   font-size: 1.5rem;
   cursor: pointer;
   border: none;
   margin: 0.1em;
 }
+
+select option {
+  background-color: #ffffff;
+  color: var(--c);
+  font-family: system-ui, sans-serif;
+  font-weight: bold;
+  font-size: 1.5rem;
+  padding: 0.1em 0.3em;
+}
+
+select option:hover {
+  background-color: var(--c);
+  color: #ffffff;
+}
```

### Comparing `prolint2-0.0.8/prolint2/server/static/css/pdbe-molstar-3.1.0_vendor.css` & `prolint2-0.0.9/prolint2/server/static/css/pdbe-molstar-3.1.0_vendor.css`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.8/prolint2/server/static/images/logo.png` & `prolint2-0.0.9/prolint2/server/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.8/prolint2/server/static/js/ganttApp.js` & `prolint2-0.0.9/prolint2/server/static/js/ganttApp.js`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.8/prolint2/server/static/js/heatmapApp.js` & `prolint2-0.0.9/prolint2/server/static/js/heatmapApp.js`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.8/prolint2/server/static/js/mol.js` & `prolint2-0.0.9/prolint2/server/static/js/mol.js`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.8/prolint2/server/static/js/network.js` & `prolint2-0.0.9/prolint2/server/static/js/network.js`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.8/prolint2/server/static/js/pdbe-molstar-plugin-3.1.0_vendor.js` & `prolint2-0.0.9/prolint2/server/static/js/pdbe-molstar-plugin-3.1.0_vendor.js`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.8/prolint2/server/static/js/pie.js` & `prolint2-0.0.9/prolint2/server/static/js/pie.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -161,15 +161,16 @@
         if (lipid != rootReferenceObjects["axisRange"].get("label").get('text')) {
             sameLipid = false;
             // TODO:
             // get correct protein
             // Update Circular App Data
             obj.protein = "Protein"
             obj.lipid = lipid
-            fetch('/data/' + JSON.stringify(obj))
+            obj.metric = document.getElementById("metric_button").value;
+            fetch('/metric/' + JSON.stringify(obj))
                 .then(response => response.json())
                 .then(responseData => {
 
                     var updateData = responseData['data'];
 
                     rootReferenceObjects["series"].data.setAll(updateData);
                     rootReferenceObjects["categoryAxis"].data.setAll(updateData);
```

### Comparing `prolint2-0.0.8/prolint2/server/static/js/radialApp.js` & `prolint2-0.0.9/prolint2/server/static/js/radialApp.js`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.8/prolint2/server/static/js/table.js` & `prolint2-0.0.9/prolint2/server/static/js/table.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -31,14 +31,18 @@
             }, {
                 title: "f",
                 field: "contactFrequency",
                 // width: 120,
                 hozAlign: "center",
                 headerSort: false,
                 resizable: false,
+                formatter: function(cell) {
+                    return parseFloat(cell.getValue()).toFixed(2);
+                },
+
             }, ]
         }],
         headerVisible: true,
     });
 
     table.on("rowClick", function(e, row) {
```

### Comparing `prolint2-0.0.8/prolint2/server/static/js/timeseries.js` & `prolint2-0.0.9/prolint2/server/static/js/timeseries.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -136,15 +136,15 @@
         return am5.Bullet.new(root, {
             sprite: bulletCircle,
             locationY: 1,
             // radius: 5
         });
     });
 
-    series.children.moveValue(series.bulletsContainer, 0);
+    series.children.moveValue(series.bulletsContainer, series.children.length + 1);
 
 
     series.on("tooltipDataItem", function(tooltipDataItem) {
 
         var residueID = tooltipDataItem.dataContext.category.split(' ')[1]
         residueID = parseInt(residueID)
```

### Comparing `prolint2-0.0.8/prolint2/server/static/js/utils.js` & `prolint2-0.0.9/prolint2/server/static/js/utils.js`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.8/prolint2/server/utils.py` & `prolint2-0.0.9/prolint2/server/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,42 +18,42 @@
         if not el-tolerance <= prev_el:
             ranges_collect.append((range_start, prev_el))
             range_start = el
         if ix == len(frames) - 1:
             ranges_collect.append((range_start, el))
     return ranges_collect
 
-def calculate_contact_intervals(TS, g, lipid_id, residues_to_show=15, intervals_to_filter_out=10):
+def calculate_contact_intervals(contacts, g, lipid_id, residues_to_show=15, intervals_to_filter_out=10):
     """
     TODO:
     write doc
     """
     contact_intervals = {}
     for res, _ in g[lipid_id][:residues_to_show]:
-        frame_numbers = TS.contacts.contact_frames[f'{res},{lipid_id}']
+        frame_numbers = contacts.contact_frames[res][lipid_id]
         frame_intervals = get_frame_contact_intervals(frame_numbers)
         for start, end in frame_intervals:
             if end - start < intervals_to_filter_out:
                 continue
 
             if res in contact_intervals:
                 contact_intervals[res].append((start, end))
             else:
                 contact_intervals[res] = [(start, end)]
 
     return contact_intervals
 
-def amCharts_contact_intervals(TS, g, lipid_id, residues_to_show=15, intervals_to_filter_out=10):
+def amCharts_contact_intervals(contacts, g, lipid_id, residues_to_show=15, intervals_to_filter_out=10):
     """
     TODO:
     write doc
     """
     contact_intervals = []
     for res, _ in g[lipid_id][:residues_to_show]:
-        frame_numbers = TS.contacts.contact_frames[f'{res},{lipid_id}']
+        frame_numbers = contacts.contact_frames[res][lipid_id]
         frame_intervals = get_frame_contact_intervals(frame_numbers)
         for start, end in frame_intervals:
             if end - start < intervals_to_filter_out:
                 continue
 
             d = {
             "category": res,
```

### Comparing `prolint2-0.0.8/prolint2.egg-info/PKG-INFO` & `prolint2-0.0.9/prolint2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prolint2
-Version: 0.0.8
+Version: 0.0.9
 Summary: ProLint2: Lipid-Protein Interaction Analysis.
 Home-page: https://github.com/ProLint/prolint2
 Author: Daniel P. Ramirez & Besian I. Sejdiu
 Author-email: daniel.ramirezecheme@ucalgary.ca
 License: MIT
 Platform: Linux
 Platform: Mac OS-X
```

### Comparing `prolint2-0.0.8/setup.py` & `prolint2-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.8/versioneer.py` & `prolint2-0.0.9/versioneer.py`

 * *Files identical despite different names*

