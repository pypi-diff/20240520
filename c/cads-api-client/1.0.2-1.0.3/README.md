# Comparing `tmp/cads_api_client-1.0.2.tar.gz` & `tmp/cads_api_client-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cads_api_client-1.0.2.tar", last modified: Mon May 13 12:26:19 2024, max compression
+gzip compressed data, was "cads_api_client-1.0.3.tar", last modified: Mon May 20 09:10:23 2024, max compression
```

## Comparing `cads_api_client-1.0.2.tar` & `cads_api_client-1.0.3.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:26:19.751149 cads_api_client-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/.cruft.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:26:19.743149 cads_api_client-1.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:26:19.747149 cads_api_client-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/.github/workflows/on-push.yml
--rw-r--r--   0 runner    (1001) docker     (127)     8827 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/.pre-commit-config-cruft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    16585 2024-05-13 12:26:19.751149 cads_api_client-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:26:19.747149 cads_api_client-1.0.2/cads_api_client/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/cads_api_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/cads_api_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/cads_api_client/catalogue.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/cads_api_client/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/cads_api_client/legacy_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    15581 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/cads_api_client/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/cads_api_client/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/cads_api_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-13 12:26:19.000000 cads_api_client-1.0.2/cads_api_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:26:19.751149 cads_api_client-1.0.2/cads_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16585 2024-05-13 12:26:19.000000 cads_api_client-1.0.2/cads_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-13 12:26:19.000000 cads_api_client-1.0.2/cads_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 12:26:19.000000 cads_api_client-1.0.2/cads_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-13 12:26:19.000000 cads_api_client-1.0.2/cads_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-13 12:26:19.000000 cads_api_client-1.0.2/cads_api_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:26:19.747149 cads_api_client-1.0.2/ci/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/ci/environment-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/ci/environment-integration.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:26:19.751149 cads_api_client-1.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:26:19.751149 cads_api_client-1.0.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/docs/_static/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:26:19.751149 cads_api_client-1.0.2/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/docs/_templates/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:26:19.751149 cads_api_client-1.0.2/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    15779 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/notebooks/cads_api_client_test.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    44415 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/notebooks/cads_api_constraints_test.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12254 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/notebooks/cads_api_filters_and_pagination_tests.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/notebooks/cads_api_licences_tests.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 12:26:19.751149 cads_api_client-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:26:19.751149 cads_api_client-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/tests/integration_test_10_catalogue.py
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/tests/integration_test_20_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/tests/integration_test_30_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/tests/integration_test_40_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/tests/integration_test_50_legacy_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/tests/test_00_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/tests/test_10_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14768 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/tests/test_10_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:10:23.422110 cads_api_client-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-20 09:10:11.000000 cads_api_client-1.0.3/.cruft.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:10:23.414110 cads_api_client-1.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:10:23.414110 cads_api_client-1.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-05-20 09:10:11.000000 cads_api_client-1.0.3/.github/workflows/on-push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     8827 2024-05-20 09:10:11.000000 cads_api_client-1.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-20 09:10:11.000000 cads_api_client-1.0.3/.pre-commit-config-cruft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-20 09:10:11.000000 cads_api_client-1.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-20 09:10:11.000000 cads_api_client-1.0.3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-05-20 09:10:11.000000 cads_api_client-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-20 09:10:11.000000 cads_api_client-1.0.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    16585 2024-05-20 09:10:23.422110 cads_api_client-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-05-20 09:10:11.000000 cads_api_client-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:10:23.418110 cads_api_client-1.0.3/cads_api_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-20 09:10:11.000000 cads_api_client-1.0.3/cads_api_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-05-20 09:10:11.000000 cads_api_client-1.0.3/cads_api_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-20 09:10:11.000000 cads_api_client-1.0.3/cads_api_client/catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-20 09:10:11.000000 cads_api_client-1.0.3/cads_api_client/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-05-20 09:10:11.000000 cads_api_client-1.0.3/cads_api_client/legacy_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15475 2024-05-20 09:10:11.000000 cads_api_client-1.0.3/cads_api_client/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-20 09:10:11.000000 cads_api_client-1.0.3/cads_api_client/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 09:10:11.000000 cads_api_client-1.0.3/cads_api_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-20 09:10:23.000000 cads_api_client-1.0.3/cads_api_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:10:23.422110 cads_api_client-1.0.3/cads_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16585 2024-05-20 09:10:23.000000 cads_api_client-1.0.3/cads_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-20 09:10:23.000000 cads_api_client-1.0.3/cads_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 09:10:23.000000 cads_api_client-1.0.3/cads_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-20 09:10:23.000000 cads_api_client-1.0.3/cads_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-20 09:10:23.000000 cads_api_client-1.0.3/cads_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:10:23.418110 cads_api_client-1.0.3/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-20 09:10:11.000000 cads_api_client-1.0.3/ci/environment-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-20 09:10:11.000000 cads_api_client-1.0.3/ci/environment-integration.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:10:23.418110 cads_api_client-1.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-20 09:10:11.000000 cads_api_client-1.0.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:10:23.418110 cads_api_client-1.0.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 09:10:11.000000 cads_api_client-1.0.3/docs/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:10:23.418110 cads_api_client-1.0.3/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 09:10:11.000000 cads_api_client-1.0.3/docs/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-20 09:10:11.000000 cads_api_client-1.0.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-20 09:10:11.000000 cads_api_client-1.0.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-20 09:10:11.000000 cads_api_client-1.0.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-20 09:10:11.000000 cads_api_client-1.0.3/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:10:23.418110 cads_api_client-1.0.3/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    15779 2024-05-20 09:10:11.000000 cads_api_client-1.0.3/notebooks/cads_api_client_test.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    44415 2024-05-20 09:10:11.000000 cads_api_client-1.0.3/notebooks/cads_api_constraints_test.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12254 2024-05-20 09:10:11.000000 cads_api_client-1.0.3/notebooks/cads_api_filters_and_pagination_tests.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-05-20 09:10:11.000000 cads_api_client-1.0.3/notebooks/cads_api_licences_tests.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-20 09:10:11.000000 cads_api_client-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 09:10:23.422110 cads_api_client-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:10:23.422110 cads_api_client-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-20 09:10:11.000000 cads_api_client-1.0.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-20 09:10:11.000000 cads_api_client-1.0.3/tests/integration_test_10_catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-20 09:10:11.000000 cads_api_client-1.0.3/tests/integration_test_20_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-20 09:10:11.000000 cads_api_client-1.0.3/tests/integration_test_30_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-20 09:10:11.000000 cads_api_client-1.0.3/tests/integration_test_40_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-20 09:10:11.000000 cads_api_client-1.0.3/tests/integration_test_50_legacy_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-20 09:10:11.000000 cads_api_client-1.0.3/tests/test_00_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-20 09:10:11.000000 cads_api_client-1.0.3/tests/test_10_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14717 2024-05-20 09:10:11.000000 cads_api_client-1.0.3/tests/test_10_processing.py
```

### Comparing `cads_api_client-1.0.2/.cruft.json` & `cads_api_client-1.0.3/.cruft.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'commit'": "'22f52dd88a2ec84dfa380d8e2c655e0b3752a10a'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "checkout": null,
-    "commit": "a95a988e0a6488f2bfa141ed1d9dd4221ff4eda9",
+    "commit": "22f52dd88a2ec84dfa380d8e2c655e0b3752a10a",
     "context": {
         "cookiecutter": {
             "_template": "https://github.com/ecmwf-projects/cookiecutter-conda-package",
             "copyright_holder": "European Union",
             "copyright_year": "2022",
             "integration_tests": "True",
             "mypy_strict": "True",
```

### Comparing `cads_api_client-1.0.2/.github/workflows/on-push.yml` & `cads_api_client-1.0.3/.github/workflows/on-push.yml`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.2/.gitignore` & `cads_api_client-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.2/.pre-commit-config.yaml` & `cads_api_client-1.0.3/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
   - id: mixed-line-ending
 - repo: https://github.com/keewis/blackdoc
   rev: v0.3.9
   hooks:
   - id: blackdoc
     additional_dependencies: [black==23.11.0]
 - repo: https://github.com/astral-sh/ruff-pre-commit
-  rev: v0.4.3
+  rev: v0.4.4
   hooks:
   - id: ruff
     args: [--fix, --show-fixes]
   - id: ruff-format
 - repo: https://github.com/executablebooks/mdformat
   rev: 0.7.17
   hooks:
```

### Comparing `cads_api_client-1.0.2/LICENSE` & `cads_api_client-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.2/Makefile` & `cads_api_client-1.0.3/Makefile`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.2/PKG-INFO` & `cads_api_client-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cads-api-client
-Version: 1.0.2
+Version: 1.0.3
 Summary: CADS API Python client
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `cads_api_client-1.0.2/README.md` & `cads_api_client-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.2/cads_api_client/__init__.py` & `cads_api_client-1.0.3/cads_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.2/cads_api_client/api_client.py` & `cads_api_client-1.0.3/cads_api_client/api_client.py`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.2/cads_api_client/catalogue.py` & `cads_api_client-1.0.3/cads_api_client/catalogue.py`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.2/cads_api_client/config.py` & `cads_api_client-1.0.3/cads_api_client/config.py`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.2/cads_api_client/legacy_api_client.py` & `cads_api_client-1.0.3/cads_api_client/legacy_api_client.py`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.2/cads_api_client/processing.py` & `cads_api_client-1.0.3/cads_api_client/processing.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,16 +31,14 @@
 
 def error_json_to_message(error_json: dict[str, Any]) -> str:
     error_messages = [
         str(error_json[key])
         for key in ("title", "traceback", "detail")
         if key in error_json
     ]
-    if trace_id := error_json.get("trace_id"):
-        error_messages.append(f"Trace ID is {trace_id}")
     return "\n".join(error_messages)
 
 
 def cads_raise_for_status(response: requests.Response) -> None:
     if response.status_code > 499:
         response.raise_for_status()
     if response.status_code > 399:
@@ -183,15 +181,15 @@
         session: requests.Session = requests.api,  # type: ignore
     ):
         self.url = url
         self.sleep_max = sleep_max
         self.headers = headers
         self.session = session
         self.log_start_time = None
-        logger.debug(f"Request UID is {self.request_uid}")
+        logger.info(f"Request ID is {self.request_uid}")
 
     def log_metadata(self, metadata: dict[str, Any]) -> None:
         logs = metadata.get("log", [])
         for self.log_start_time, message in sorted(logs):
             level = 20
             for severity in ("DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"):
                 if message.startswith(severity):
```

### Comparing `cads_api_client-1.0.2/cads_api_client/profile.py` & `cads_api_client-1.0.3/cads_api_client/profile.py`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.2/cads_api_client.egg-info/PKG-INFO` & `cads_api_client-1.0.3/cads_api_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cads-api-client
-Version: 1.0.2
+Version: 1.0.3
 Summary: CADS API Python client
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `cads_api_client-1.0.2/cads_api_client.egg-info/SOURCES.txt` & `cads_api_client-1.0.3/cads_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.2/docs/Makefile` & `cads_api_client-1.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.2/docs/conf.py` & `cads_api_client-1.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.2/docs/make.bat` & `cads_api_client-1.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.2/notebooks/cads_api_client_test.ipynb` & `cads_api_client-1.0.3/notebooks/cads_api_client_test.ipynb`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.2/notebooks/cads_api_constraints_test.ipynb` & `cads_api_client-1.0.3/notebooks/cads_api_constraints_test.ipynb`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.2/notebooks/cads_api_filters_and_pagination_tests.ipynb` & `cads_api_client-1.0.3/notebooks/cads_api_filters_and_pagination_tests.ipynb`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.2/notebooks/cads_api_licences_tests.ipynb` & `cads_api_client-1.0.3/notebooks/cads_api_licences_tests.ipynb`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.2/pyproject.toml` & `cads_api_client-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.2/tests/conftest.py` & `cads_api_client-1.0.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.2/tests/integration_test_10_catalogue.py` & `cads_api_client-1.0.3/tests/integration_test_10_catalogue.py`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.2/tests/integration_test_20_processing.py` & `cads_api_client-1.0.3/tests/integration_test_20_processing.py`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.2/tests/integration_test_30_remote.py` & `cads_api_client-1.0.3/tests/integration_test_30_remote.py`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.2/tests/integration_test_40_api_client.py` & `cads_api_client-1.0.3/tests/integration_test_40_api_client.py`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.2/tests/integration_test_50_legacy_api_client.py` & `cads_api_client-1.0.3/tests/integration_test_50_legacy_api_client.py`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.2/tests/test_10_config.py` & `cads_api_client-1.0.3/tests/test_10_config.py`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.2/tests/test_10_processing.py` & `cads_api_client-1.0.3/tests/test_10_processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -419,15 +419,15 @@
     responses_add()
 
     catalogue = cads_api_client.Catalogue(CATALOGUE_URL)
     collection = catalogue.collection(COLLECTION_ID)
     remote = collection.submit(variable="temperature", year="0000")
     with pytest.raises(
         cads_api_client.processing.ProcessingFailedError,
-        match="job failed\nThis is a traceback\nTrace ID is ca3e7170-1ce2-48fc-97f8-bbe64fafce44",
+        match="job failed\nThis is a traceback",
     ):
         remote.wait_on_result()
 
 
 @responses.activate
 def test_remote_logs(caplog: pytest.LogCaptureFixture) -> None:
     responses_add()
@@ -472,16 +472,16 @@
         (
             "cads_api_client.processing",
             10,
             f"REPLY {json.dumps(JOB_SUCCESSFUL_JSON)}",
         ),
         (
             "cads_api_client.processing",
-            10,
-            "Request UID is 9bfc1362-2832-48e1-a235-359267420bb2",
+            20,
+            "Request ID is 9bfc1362-2832-48e1-a235-359267420bb2",
         ),
         (
             "cads_api_client.processing",
             10,
             "GET http://localhost:8080/api/retrieve/v1/jobs/9bfc1362-2832-48e1-a235-359267420bb2",
         ),
         (
```

