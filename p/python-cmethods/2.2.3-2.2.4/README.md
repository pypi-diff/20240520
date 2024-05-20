# Comparing `tmp/python_cmethods-2.2.3.tar.gz` & `tmp/python_cmethods-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_cmethods-2.2.3.tar", last modified: Fri May 17 14:33:04 2024, max compression
+gzip compressed data, was "python_cmethods-2.2.4.tar", last modified: Mon May 20 08:48:08 2024, max compression
```

## Comparing `python_cmethods-2.2.3.tar` & `python_cmethods-2.2.4.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:33:04.589160 python_cmethods-2.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:33:04.581160 python_cmethods-2.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:33:04.581160 python_cmethods-2.2.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/.github/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/.github/dependabot.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:33:04.585160 python_cmethods-2.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/.github/workflows/_build.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/.github/workflows/_build_doc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/.github/workflows/_codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/.github/workflows/_codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/.github/workflows/_pre_commit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/.github/workflows/_pypi_publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/.github/workflows/_pypi_test_publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/.github/workflows/_test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/.github/workflows/cicd.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/.github/workflows/scorecard.yml
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13733 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    32891 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    54246 2024-05-17 14:33:04.589160 python_cmethods-2.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14083 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:33:04.585160 python_cmethods-2.2.3/cmethods/
--rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/cmethods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-17 14:33:04.000000 python_cmethods-2.2.3/cmethods/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6683 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/cmethods/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9253 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/cmethods/distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     4688 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/cmethods/scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/cmethods/static.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/cmethods/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7337 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/cmethods/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7502 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:33:04.585160 python_cmethods-2.2.3/python_cmethods.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    54246 2024-05-17 14:33:04.000000 python_cmethods-2.2.3/python_cmethods.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-17 14:33:04.000000 python_cmethods-2.2.3/python_cmethods.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 14:33:04.000000 python_cmethods-2.2.3/python_cmethods.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-17 14:33:04.000000 python_cmethods-2.2.3/python_cmethods.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-17 14:33:04.000000 python_cmethods-2.2.3/python_cmethods.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-17 14:33:04.000000 python_cmethods-2.2.3/python_cmethods.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 14:33:04.589160 python_cmethods-2.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:48:08.209335 python_cmethods-2.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:48:08.201335 python_cmethods-2.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:48:08.201335 python_cmethods-2.2.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/.github/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/.github/dependabot.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:48:08.201335 python_cmethods-2.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/.github/workflows/_build.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/.github/workflows/_build_doc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/.github/workflows/_codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/.github/workflows/_codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/.github/workflows/_pre_commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/.github/workflows/_pypi_publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/.github/workflows/_pypi_test_publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/.github/workflows/_test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/.github/workflows/cicd.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/.github/workflows/dependabot_auto_approve.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/.github/workflows/scorecard.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13733 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    32891 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    54246 2024-05-20 08:48:08.209335 python_cmethods-2.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14083 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:48:08.205335 python_cmethods-2.2.4/cmethods/
+-rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/cmethods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-20 08:48:08.000000 python_cmethods-2.2.4/cmethods/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6683 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/cmethods/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8989 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/cmethods/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4688 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/cmethods/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/cmethods/static.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/cmethods/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/cmethods/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7502 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:48:08.205335 python_cmethods-2.2.4/python_cmethods.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    54246 2024-05-20 08:48:08.000000 python_cmethods-2.2.4/python_cmethods.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-20 08:48:08.000000 python_cmethods-2.2.4/python_cmethods.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 08:48:08.000000 python_cmethods-2.2.4/python_cmethods.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-20 08:48:08.000000 python_cmethods-2.2.4/python_cmethods.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-20 08:48:08.000000 python_cmethods-2.2.4/python_cmethods.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-20 08:48:08.000000 python_cmethods-2.2.4/python_cmethods.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 08:48:08.209335 python_cmethods-2.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/setup.py
```

### Comparing `python_cmethods-2.2.3/.gitattributes` & `python_cmethods-2.2.4/.gitattributes`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.3/.github/ISSUE_TEMPLATE/bug_report.md` & `python_cmethods-2.2.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.3/.github/ISSUE_TEMPLATE/feature_request.md` & `python_cmethods-2.2.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.3/.github/codecov.yml` & `python_cmethods-2.2.4/.github/codecov.yml`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.3/.github/workflows/_build.yaml` & `python_cmethods-2.2.4/.github/workflows/_build.yaml`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.3/.github/workflows/_build_doc.yaml` & `python_cmethods-2.2.4/.github/workflows/_build_doc.yaml`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.3/.github/workflows/_codecov.yaml` & `python_cmethods-2.2.4/.github/workflows/_codecov.yaml`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.3/.github/workflows/_codeql.yaml` & `python_cmethods-2.2.4/.github/workflows/_codeql.yaml`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.3/.github/workflows/_pypi_publish.yaml` & `python_cmethods-2.2.4/.github/workflows/_pypi_publish.yaml`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.3/.github/workflows/_pypi_test_publish.yaml` & `python_cmethods-2.2.4/.github/workflows/_pypi_test_publish.yaml`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.3/.github/workflows/_test.yaml` & `python_cmethods-2.2.4/.github/workflows/_test.yaml`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.3/.github/workflows/cicd.yaml` & `python_cmethods-2.2.4/.github/workflows/cicd.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -57,14 +57,16 @@
 
   ##    Run the unit tests for Python 3.8 until 3.11
   ##
   Test:
     needs: [Pre-Commit]
     uses: ./.github/workflows/_test.yaml
     strategy:
+      # FIXME: fail-fast as soon as the tests are not flaky anymore
+      fail-fast: false
       matrix:
         os: [ubuntu-latest, windows-latest]
         python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
     with:
       os: ${{ matrix.os }}
       python-version: ${{ matrix.python-version }}
```

### Comparing `python_cmethods-2.2.3/.github/workflows/scorecard.yml` & `python_cmethods-2.2.4/.github/workflows/scorecard.yml`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.3/.gitignore` & `python_cmethods-2.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.3/.pre-commit-config.yaml` & `python_cmethods-2.2.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.3/CHANGELOG.md` & `python_cmethods-2.2.4/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.3/LICENSE` & `python_cmethods-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.3/Makefile` & `python_cmethods-2.2.4/Makefile`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.3/PKG-INFO` & `python_cmethods-2.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-cmethods
-Version: 2.2.3
+Version: 2.2.4
 Summary: A collection of bias correction techniques written in Python - for climate sciences.
 Author-email: Benjamin Thomas Schwertfeger <contact@b-schwertfeger.de>
 Maintainer-email: Benjamin Thomas Schwertfeger <contact@b-schwertfeger.de>
 License: GNU GENERAL PUBLIC LICENSE
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `python_cmethods-2.2.3/README.md` & `python_cmethods-2.2.4/README.md`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.3/SECURITY.md` & `python_cmethods-2.2.4/SECURITY.md`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.3/cmethods/__init__.py` & `python_cmethods-2.2.4/cmethods/__init__.py`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.3/cmethods/core.py` & `python_cmethods-2.2.4/cmethods/core.py`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.3/cmethods/distribution.py` & `python_cmethods-2.2.4/cmethods/distribution.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,19 +58,14 @@
         return simp
 
     wide = abs(global_max - global_min) / n_quantiles
     xbins = np.arange(global_min, global_max + wide, wide)
 
     cdf_obs = get_cdf(obs, xbins)
     cdf_simh = get_cdf(simh, xbins)
-    cdf_simh = np.interp(
-        cdf_simh,
-        (cdf_simh.min(), cdf_simh.max()),
-        (cdf_obs.min(), cdf_obs.max()),
-    )
 
     if kind in ADDITIVE:
         epsilon = np.interp(simp, xbins, cdf_simh)  # Eq. 1
         return get_inverse_of_cdf(cdf_obs, epsilon, xbins)  # Eq. 1
 
     if kind in MULTIPLICATIVE:
         epsilon = np.interp(  # Eq. 2
@@ -125,19 +120,14 @@
         return np.array(simp.values)
 
     wide = abs(global_max - global_min) / n_quantiles
     xbins = np.arange(global_min, global_max + wide, wide)
 
     cdf_obs = get_cdf(obs, xbins)
     cdf_simh = get_cdf(simh, xbins)
-    cdf_simh = np.interp(
-        cdf_simh,
-        (cdf_simh.min(), cdf_simh.max()),
-        (cdf_obs.min(), cdf_obs.max()),
-    )
 
     # detrended => shift mean of $X_{sim,p}$ to range of $X_{sim,h}$ to adjust extremes
     res = np.zeros(len(simp.values))
     max_scaling_factor: Final[float] = kwargs.get(
         "max_scaling_factor",
         MAX_SCALING_FACTOR,
     )
```

### Comparing `python_cmethods-2.2.3/cmethods/scaling.py` & `python_cmethods-2.2.4/cmethods/scaling.py`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.3/cmethods/static.py` & `python_cmethods-2.2.4/cmethods/static.py`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.3/cmethods/utils.py` & `python_cmethods-2.2.4/cmethods/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -145,19 +145,19 @@
     :return: The probability densitiy function of ``x``
     :rtype: np.ndarray
 
     .. code-block:: python
         :linenos:
         :caption: Compute the probability density function :math:`P(x)`
 
-        >>> from cmethods import CMethods as cm
+        >>> from cmethods get_pdf
 
         >>> x = [1, 2, 3, 4, 5, 5, 5, 6, 7, 8, 9, 10]
         >>> xbins = [0, 3, 6, 10]
-        >>> print(cm.get_pdf(x=x, xbins=xbins))
+        >>> print(get_pdf(x=x, xbins=xbins))
         [2, 5, 5]
     """
     pdf, _ = np.histogram(x, xbins)
     return pdf
 
 
 def get_cdf(
@@ -174,25 +174,26 @@
     :type xbins: list | np.ndarray
     :return: The cumulative distribution function of ``x``
     :rtype: np.ndarray
 
 
     .. code-block:: python
         :linenos:
-        :caption: Compute the cmmulative distribution function :math:`F(x)`
+        :caption: Compute the cumulative distribution function :math:`F(x)`
 
-        >>> from cmethods import CMethods as cm
+        >>> from cmethods.utils import get_cdf
 
         >>> x = [1, 2, 3, 4, 5, 5, 5, 6, 7, 8, 9, 10]
         >>> xbins = [0, 3, 6, 10]
-        >>> print(cm.get_cdf(x=x, xbins=xbins))
-        [0, 2, 7, 12]
+        >>> print(get_cdf(x=x, xbins=xbins))
+        [0.0, 0.16666667, 0.58333333, 1.]
     """
     pdf, _ = np.histogram(x, xbins)
-    return np.insert(np.cumsum(pdf), 0, 0.0)
+    cdf = np.insert(np.cumsum(pdf), 0, 0.0)
+    return cdf / cdf[-1]
 
 
 def get_inverse_of_cdf(
     base_cdf: Union[list, np.ndarray],
     insert_cdf: Union[list, np.ndarray],
     xbins: Union[list, np.ndarray],
 ) -> np.ndarray:
```

### Comparing `python_cmethods-2.2.3/pyproject.toml` & `python_cmethods-2.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.3/python_cmethods.egg-info/PKG-INFO` & `python_cmethods-2.2.4/python_cmethods.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-cmethods
-Version: 2.2.3
+Version: 2.2.4
 Summary: A collection of bias correction techniques written in Python - for climate sciences.
 Author-email: Benjamin Thomas Schwertfeger <contact@b-schwertfeger.de>
 Maintainer-email: Benjamin Thomas Schwertfeger <contact@b-schwertfeger.de>
 License: GNU GENERAL PUBLIC LICENSE
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `python_cmethods-2.2.3/python_cmethods.egg-info/SOURCES.txt` & `python_cmethods-2.2.4/python_cmethods.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 .github/workflows/_codecov.yaml
 .github/workflows/_codeql.yaml
 .github/workflows/_pre_commit.yaml
 .github/workflows/_pypi_publish.yaml
 .github/workflows/_pypi_test_publish.yaml
 .github/workflows/_test.yaml
 .github/workflows/cicd.yaml
+.github/workflows/dependabot_auto_approve.yaml
 .github/workflows/scorecard.yml
 cmethods/__init__.py
 cmethods/_version.py
 cmethods/core.py
 cmethods/distribution.py
 cmethods/scaling.py
 cmethods/static.py
```

