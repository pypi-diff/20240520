# Comparing `tmp/stac_asset-0.3.1.tar.gz` & `tmp/stac_asset-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac_asset-0.3.1.tar", last modified: Mon May 13 14:33:06 2024, max compression
+gzip compressed data, was "stac_asset-0.3.2.tar", last modified: Mon May 20 12:30:56 2024, max compression
```

## Comparing `stac_asset-0.3.1.tar` & `stac_asset-0.3.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:33:06.182827 stac_asset-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-13 14:33:02.000000 stac_asset-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-13 14:33:02.000000 stac_asset-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-13 14:33:02.000000 stac_asset-0.3.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     8293 2024-05-13 14:33:06.182827 stac_asset-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-05-13 14:33:02.000000 stac_asset-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-13 14:33:02.000000 stac_asset-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 14:33:06.182827 stac_asset-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:33:06.174827 stac_asset-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:33:06.178827 stac_asset-0.3.1/src/stac_asset/
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-13 14:33:02.000000 stac_asset-0.3.1/src/stac_asset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15367 2024-05-13 14:33:02.000000 stac_asset-0.3.1/src/stac_asset/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    18954 2024-05-13 14:33:02.000000 stac_asset-0.3.1/src/stac_asset/_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-05-13 14:33:02.000000 stac_asset-0.3.1/src/stac_asset/blocking.py
--rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-05-13 14:33:02.000000 stac_asset-0.3.1/src/stac_asset/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-05-13 14:33:02.000000 stac_asset-0.3.1/src/stac_asset/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-13 14:33:02.000000 stac_asset-0.3.1/src/stac_asset/earthdata_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-13 14:33:02.000000 stac_asset-0.3.1/src/stac_asset/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-13 14:33:02.000000 stac_asset-0.3.1/src/stac_asset/filesystem_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-05-13 14:33:02.000000 stac_asset-0.3.1/src/stac_asset/http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-13 14:33:02.000000 stac_asset-0.3.1/src/stac_asset/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-05-13 14:33:02.000000 stac_asset-0.3.1/src/stac_asset/planetary_computer_client.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 14:33:02.000000 stac_asset-0.3.1/src/stac_asset/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-05-13 14:33:02.000000 stac_asset-0.3.1/src/stac_asset/s3_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-13 14:33:02.000000 stac_asset-0.3.1/src/stac_asset/strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-13 14:33:02.000000 stac_asset-0.3.1/src/stac_asset/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-13 14:33:02.000000 stac_asset-0.3.1/src/stac_asset/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:33:06.182827 stac_asset-0.3.1/src/stac_asset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8293 2024-05-13 14:33:06.000000 stac_asset-0.3.1/src/stac_asset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-13 14:33:06.000000 stac_asset-0.3.1/src/stac_asset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 14:33:06.000000 stac_asset-0.3.1/src/stac_asset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-13 14:33:06.000000 stac_asset-0.3.1/src/stac_asset.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-13 14:33:06.000000 stac_asset-0.3.1/src/stac_asset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-13 14:33:06.000000 stac_asset-0.3.1/src/stac_asset.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:33:06.182827 stac_asset-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-13 14:33:02.000000 stac_asset-0.3.1/tests/test_blocking.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-13 14:33:02.000000 stac_asset-0.3.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-13 14:33:02.000000 stac_asset-0.3.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-13 14:33:02.000000 stac_asset-0.3.1/tests/test_earthdata_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-13 14:33:02.000000 stac_asset-0.3.1/tests/test_filesystem_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8722 2024-05-13 14:33:02.000000 stac_asset-0.3.1/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-13 14:33:02.000000 stac_asset-0.3.1/tests/test_http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-13 14:33:02.000000 stac_asset-0.3.1/tests/test_planetary_computer_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-13 14:33:02.000000 stac_asset-0.3.1/tests/test_s3_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-13 14:33:02.000000 stac_asset-0.3.1/tests/test_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:30:56.833710 stac_asset-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-20 12:30:53.000000 stac_asset-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-20 12:30:53.000000 stac_asset-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-20 12:30:53.000000 stac_asset-0.3.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-05-20 12:30:56.833710 stac_asset-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-05-20 12:30:53.000000 stac_asset-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-20 12:30:53.000000 stac_asset-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 12:30:56.833710 stac_asset-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:30:56.825710 stac_asset-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:30:56.829710 stac_asset-0.3.2/src/stac_asset/
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-20 12:30:53.000000 stac_asset-0.3.2/src/stac_asset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15367 2024-05-20 12:30:53.000000 stac_asset-0.3.2/src/stac_asset/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19461 2024-05-20 12:30:53.000000 stac_asset-0.3.2/src/stac_asset/_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-05-20 12:30:53.000000 stac_asset-0.3.2/src/stac_asset/blocking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-05-20 12:30:53.000000 stac_asset-0.3.2/src/stac_asset/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-05-20 12:30:53.000000 stac_asset-0.3.2/src/stac_asset/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-20 12:30:53.000000 stac_asset-0.3.2/src/stac_asset/earthdata_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-20 12:30:53.000000 stac_asset-0.3.2/src/stac_asset/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-20 12:30:53.000000 stac_asset-0.3.2/src/stac_asset/filesystem_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-20 12:30:53.000000 stac_asset-0.3.2/src/stac_asset/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-20 12:30:53.000000 stac_asset-0.3.2/src/stac_asset/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-05-20 12:30:53.000000 stac_asset-0.3.2/src/stac_asset/planetary_computer_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 12:30:53.000000 stac_asset-0.3.2/src/stac_asset/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-05-20 12:30:53.000000 stac_asset-0.3.2/src/stac_asset/s3_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-20 12:30:53.000000 stac_asset-0.3.2/src/stac_asset/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-20 12:30:53.000000 stac_asset-0.3.2/src/stac_asset/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-20 12:30:53.000000 stac_asset-0.3.2/src/stac_asset/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:30:56.833710 stac_asset-0.3.2/src/stac_asset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-05-20 12:30:56.000000 stac_asset-0.3.2/src/stac_asset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-20 12:30:56.000000 stac_asset-0.3.2/src/stac_asset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 12:30:56.000000 stac_asset-0.3.2/src/stac_asset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-20 12:30:56.000000 stac_asset-0.3.2/src/stac_asset.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-20 12:30:56.000000 stac_asset-0.3.2/src/stac_asset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-20 12:30:56.000000 stac_asset-0.3.2/src/stac_asset.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:30:56.833710 stac_asset-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-20 12:30:53.000000 stac_asset-0.3.2/tests/test_blocking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-20 12:30:53.000000 stac_asset-0.3.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-20 12:30:53.000000 stac_asset-0.3.2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-20 12:30:53.000000 stac_asset-0.3.2/tests/test_earthdata_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-20 12:30:53.000000 stac_asset-0.3.2/tests/test_filesystem_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8722 2024-05-20 12:30:53.000000 stac_asset-0.3.2/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-20 12:30:53.000000 stac_asset-0.3.2/tests/test_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-20 12:30:53.000000 stac_asset-0.3.2/tests/test_planetary_computer_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-20 12:30:53.000000 stac_asset-0.3.2/tests/test_s3_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-20 12:30:53.000000 stac_asset-0.3.2/tests/test_validate.py
```

### Comparing `stac_asset-0.3.1/LICENSE` & `stac_asset-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.1/NOTICE` & `stac_asset-0.3.2/NOTICE`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.1/PKG-INFO` & `stac_asset-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-asset
-Version: 0.3.1
+Version: 0.3.2
 Summary: Read and download STAC assets across platforms and providers
 Author-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: Github, https://github.com/stac-utils/stac-asset
 Project-URL: CHANGELOG, https://github.com/stac-utils/stac-asset/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/stac-utils/stac-asset/issues
 Keywords: stac,async
@@ -30,26 +30,27 @@
 Requires-Dist: click-logging~=1.0.1; extra == "cli"
 Requires-Dist: tabulate~=0.9.0; extra == "cli"
 Requires-Dist: tqdm~=4.66.1; extra == "cli"
 Provides-Extra: dev
 Requires-Dist: mypy~=1.3; extra == "dev"
 Requires-Dist: pre-commit~=3.3; extra == "dev"
 Requires-Dist: pystac[validation]>=1.8.4; extra == "dev"
-Requires-Dist: pytest~=7.3; extra == "dev"
+Requires-Dist: pytest~=8.2; extra == "dev"
 Requires-Dist: pytest-asyncio~=0.21; extra == "dev"
 Requires-Dist: pytest-cov>=5.0; extra == "dev"
+Requires-Dist: pytest-recording~=0.13.1; extra == "dev"
 Requires-Dist: ruff==0.4.4; extra == "dev"
 Requires-Dist: types-aiofiles~=23.1; extra == "dev"
 Requires-Dist: types-python-dateutil~=2.9; extra == "dev"
 Requires-Dist: types-tqdm~=4.66.0; extra == "dev"
 Requires-Dist: types-tabulate~=0.9.0; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: pydata-sphinx-theme~=0.13; extra == "docs"
 Requires-Dist: sphinx~=7.3; extra == "docs"
-Requires-Dist: sphinx-click~=5.0; extra == "docs"
+Requires-Dist: sphinx-click~=6.0; extra == "docs"
 
 # stac-asset
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/stac-utils/stac-asset/ci.yaml?style=for-the-badge)](https://github.com/stac-utils/stac-asset/actions/workflows/ci.yaml)
 [![Read the Docs](https://img.shields.io/readthedocs/stac-asset?style=for-the-badge)](https://stac-asset.readthedocs.io/en/stable/)
 [![PyPI](https://img.shields.io/pypi/v/stac-asset?style=for-the-badge)](https://pypi.org/project/stac-asset)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg?style=for-the-badge)](./CODE_OF_CONDUCT)
@@ -175,16 +176,16 @@
 cd stac-asset
 pip install '.[dev]'
 pre-commit install
 ```
 
 ### Testing
 
-All network-touching tests are disabled by default, because we can't use [pytest-vcr](https://pytest-vcr.readthedocs.io/en/latest/) (<https://github.com/kevin1024/vcrpy/issues/597>), and repeatedly hitting the network during testing and CI is bad behavior.
-To enable network-touching tests:
+Some network-touching tests are disabled by default.
+To enable these tests:
 
 ```shell
 pytest --network-access
 ```
 
 Some tests are client-specific and need your environment to be configured correctly.
 See [each client's documentation](#clients) for instructions on setting up your environment for each client.
```

### Comparing `stac_asset-0.3.1/README.md` & `stac_asset-0.3.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -126,16 +126,16 @@
 cd stac-asset
 pip install '.[dev]'
 pre-commit install
 ```
 
 ### Testing
 
-All network-touching tests are disabled by default, because we can't use [pytest-vcr](https://pytest-vcr.readthedocs.io/en/latest/) (<https://github.com/kevin1024/vcrpy/issues/597>), and repeatedly hitting the network during testing and CI is bad behavior.
-To enable network-touching tests:
+Some network-touching tests are disabled by default.
+To enable these tests:
 
 ```shell
 pytest --network-access
 ```
 
 Some tests are client-specific and need your environment to be configured correctly.
 See [each client's documentation](#clients) for instructions on setting up your environment for each client.
```

### Comparing `stac_asset-0.3.1/pyproject.toml` & `stac_asset-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "stac-asset"
-version = "0.3.1"
+version = "0.3.2"
 description = "Read and download STAC assets across platforms and providers"
 authors = [{ name = "Pete Gadomski", email = "pete.gadomski@gmail.com" }]
 readme = "README.md"
 keywords = ["stac", "async"]
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
@@ -32,24 +32,25 @@
     "tabulate~=0.9.0",
     "tqdm~=4.66.1",
 ]
 dev = [
     "mypy~=1.3",
     "pre-commit~=3.3",
     "pystac[validation]>=1.8.4",
-    "pytest~=7.3",
+    "pytest~=8.2",
     "pytest-asyncio~=0.21",
     "pytest-cov>=5.0",
+    "pytest-recording~=0.13.1",
     "ruff==0.4.4",
     "types-aiofiles~=23.1",
     "types-python-dateutil~=2.9",
     "types-tqdm~=4.66.0",
     "types-tabulate~=0.9.0",
 ]
-docs = ["pydata-sphinx-theme~=0.13", "sphinx~=7.3", "sphinx-click~=5.0"]
+docs = ["pydata-sphinx-theme~=0.13", "sphinx~=7.3", "sphinx-click~=6.0"]
 
 [project.scripts]
 stac-asset = "stac_asset._cli:cli"
 
 [project.urls]
 Github = "https://github.com/stac-utils/stac-asset"
 CHANGELOG = "https://github.com/stac-utils/stac-asset/blob/main/CHANGELOG.md"
```

### Comparing `stac_asset-0.3.1/src/stac_asset/__init__.py` & `stac_asset-0.3.2/src/stac_asset/__init__.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.1/src/stac_asset/_cli.py` & `stac_asset-0.3.2/src/stac_asset/_cli.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.1/src/stac_asset/_functions.py` & `stac_asset-0.3.2/src/stac_asset/_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import asyncio
 import json
 import os.path
 import warnings
-from asyncio import Task
+from asyncio import Semaphore, Task
 from dataclasses import dataclass
 from pathlib import Path
 from types import TracebackType
 from typing import (
     AsyncIterator,
     List,
     Optional,
@@ -70,20 +70,27 @@
         return self
 
 
 class Downloads:
     clients: Clients
     config: Config
     downloads: List[Download]
+    semaphore: Semaphore
 
-    def __init__(self, config: Config, clients: Optional[List[Client]] = None) -> None:
+    def __init__(
+        self,
+        config: Config,
+        clients: Optional[List[Client]] = None,
+        max_concurrent_downloads: int = 500,
+    ) -> None:
         config.validate()
         self.config = config
         self.downloads = list()
         self.clients = Clients(config, clients)
+        self.semaphore = Semaphore(max_concurrent_downloads)
 
     async def add(
         self,
         stac_object: Union[Item, Collection],
         root: Path,
         file_name: Optional[str],
         keep_non_downloaded: bool,
@@ -132,19 +139,17 @@
             stac_object.assets.update(assets)
         else:
             stac_object.assets = assets
 
     async def download(self, messages: Optional[MessageQueue]) -> None:
         tasks: Set[Task[Union[Download, WrappedError]]] = set()
         for download in self.downloads:
-            task = asyncio.create_task(
-                download.download(
-                    messages=messages,
-                )
-            )
+            # wait to acquire the semaphore before starting a new download task
+            await self.semaphore.acquire()
+            task = asyncio.create_task(self._download_with_release(download, messages))
             tasks.add(task)
             task.add_done_callback(tasks.discard)
 
         try:
             results = await asyncio.gather(*tasks)
         except Exception as error:
             # We failed fast
@@ -167,14 +172,22 @@
                 if self.config.warn:
                     warnings.warn(str(result.error), DownloadWarning)
                 else:
                     exceptions.append(result.error)
         if exceptions:
             raise DownloadError(exceptions)
 
+    async def _download_with_release(
+        self, download: Download, messages: Optional[MessageQueue]
+    ) -> Download | WrappedError:
+        try:
+            return await download.download(messages=messages)
+        finally:
+            self.semaphore.release()
+
     async def __aenter__(self) -> Downloads:
         return self
 
     async def __aexit__(
         self,
         exc_type: Optional[Type[BaseException]],
         exc_val: Optional[BaseException],
```

### Comparing `stac_asset-0.3.1/src/stac_asset/blocking.py` & `stac_asset-0.3.2/src/stac_asset/blocking.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.1/src/stac_asset/client.py` & `stac_asset-0.3.2/src/stac_asset/client.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.1/src/stac_asset/config.py` & `stac_asset-0.3.2/src/stac_asset/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from .errors import ConfigError
 from .strategy import ErrorStrategy, FileNameStrategy
 
 DEFAULT_S3_REGION_NAME = "us-west-2"
 DEFAULT_S3_RETRY_MODE = "adaptive"
 DEFAULT_S3_MAX_ATTEMPTS = 10
+DEFAULT_HTTP_CLIENT_TIMEOUT = 300
 
 
 @dataclass
 class Config:
     """Configuration for downloading items and their assets."""
 
     alternate_assets: List[str] = field(default_factory=list)
@@ -55,14 +56,17 @@
 
     clean: bool = True
     """If true, clean up the downloaded file if it errors."""
 
     overwrite: bool = False
     """Download files even if they already exist locally."""
 
+    http_client_timeout: Optional[float] = DEFAULT_HTTP_CLIENT_TIMEOUT
+    """Total number of seconds for the whole request."""
+
     earthdata_token: Optional[str] = None
     """A token for logging in to Earthdata."""
 
     s3_region_name: str = DEFAULT_S3_REGION_NAME
     """Default s3 region."""
 
     s3_requester_pays: bool = False
```

### Comparing `stac_asset-0.3.1/src/stac_asset/earthdata_client.py` & `stac_asset-0.3.2/src/stac_asset/earthdata_client.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.1/src/stac_asset/errors.py` & `stac_asset-0.3.2/src/stac_asset/errors.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.1/src/stac_asset/filesystem_client.py` & `stac_asset-0.3.2/src/stac_asset/filesystem_client.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.1/src/stac_asset/http_client.py` & `stac_asset-0.3.2/src/stac_asset/http_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from types import TracebackType
 from typing import AsyncIterator, Optional, Type, TypeVar
 
-from aiohttp import ClientSession
+from aiohttp import ClientSession, ClientTimeout
 from yarl import URL
 
 from . import validate
 from .client import Client
 from .config import Config
 from .messages import OpenUrl
 from .types import MessageQueue
@@ -18,35 +18,34 @@
 class HttpClient(Client):
     """A simple client for making HTTP requests.
 
     By default, doesn't do any authentication.
     Configure the session to customize its behavior.
     """
 
-    check_content_type: bool
-    """If true, check the asset's content type against the response from the server.
-
-    See :py:func:`stac_asset.validate.content_type` for more information about
-    hte content type check.
-    """
-
-    session: ClientSession
-    """A atiohttp session that will be used for all requests."""
-
     @classmethod
     async def from_config(cls: Type[T], config: Config) -> T:
         """Creates the default http client with a vanilla session object."""
         # TODO add basic auth
-        session = ClientSession()
+        timeout = ClientTimeout(total=config.http_client_timeout)
+        session = ClientSession(timeout=timeout)
         return cls(session)
 
     def __init__(self, session: ClientSession, check_content_type: bool = True) -> None:
         super().__init__()
-        self.session = session
-        self.check_content_type = check_content_type
+
+        self.session: ClientSession = session
+        """A aiohttp session that will be used for all requests."""
+
+        self.check_content_type: bool = check_content_type
+        """If true, check the asset's content type against the response from the server.
+
+        See :py:func:`stac_asset.validate.content_type` for more information about
+        the content type check.
+        """
 
     async def open_url(
         self,
         url: URL,
         content_type: Optional[str] = None,
         messages: Optional[MessageQueue] = None,
     ) -> AsyncIterator[bytes]:
```

### Comparing `stac_asset-0.3.1/src/stac_asset/messages.py` & `stac_asset-0.3.2/src/stac_asset/messages.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.1/src/stac_asset/planetary_computer_client.py` & `stac_asset-0.3.2/src/stac_asset/planetary_computer_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,27 +48,25 @@
     """Open and download assets from Microsoft's Planetary Computer.
 
     Heavily cribbed from
     https://github.com/microsoft/planetary-computer-sdk-for-python/blob/main/planetary_computer/sas.py,
     thanks Tom Augspurger!
     """
 
-    _cache: Dict[URL, _Token]
-    _cache_lock: Lock
-    token_request_url: URL
-
     def __init__(
         self,
         session: ClientSession,
         sas_token_endpoint: str = DEFAULT_SAS_TOKEN_ENDPOINT,
     ) -> None:
         super().__init__(session)
-        self._cache = dict()
-        self._cache_lock = Lock()
-        self.sas_token_endpoint = URL(sas_token_endpoint)
+        self._cache: Dict[URL, _Token] = dict()
+        self._cache_lock: Lock = Lock()
+
+        self.sas_token_endpoint: URL = URL(sas_token_endpoint)
+        """The endpoint that will be used to fetch a SAS token for reading."""
 
     async def open_url(
         self,
         url: URL,
         content_type: Optional[str] = None,
         messages: Optional[Queue[Any]] = None,
     ) -> AsyncIterator[bytes]:
```

### Comparing `stac_asset-0.3.1/src/stac_asset/s3_client.py` & `stac_asset-0.3.2/src/stac_asset/s3_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,35 +26,14 @@
 
     To use the ``requester_pays`` option, you need to configure your AWS
     credentials. See `the AWS documentation
     <https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-files.html>`_
     for instructions.
     """
 
-    session: AioSession
-    """The session that will be used for all s3 requests."""
-
-    region_name: str
-    """The region that all clients will be rooted in."""
-
-    requester_pays: bool
-    """If True, enable access to `requester pays buckets
-    <https://docs.aws.amazon.com/AmazonS3/latest/userguide/RequesterPaysBuckets.html>`_."""
-
-    retry_mode: str
-    """The retry mode, one of "adaptive", "legacy", or "standard".
-
-    See `the boto3 docs
-    <https://boto3.amazonaws.com/v1/documentation/api/latest/guide/retries.html>`_
-    for more information on the available modes.
-    """
-
-    max_attempts: int
-    """The maximum number of attempts."""
-
     @classmethod
     async def from_config(cls, config: Config) -> S3Client:
         """Creates an s3 client from a config.
 
         Args:
             config: The config object
 
@@ -72,19 +51,35 @@
         self,
         requester_pays: bool = False,
         region_name: str = DEFAULT_S3_REGION_NAME,
         retry_mode: str = DEFAULT_S3_RETRY_MODE,
         max_attempts: int = DEFAULT_S3_MAX_ATTEMPTS,
     ) -> None:
         super().__init__()
-        self.session = aiobotocore.session.get_session()
-        self.region_name = region_name
-        self.requester_pays = requester_pays
-        self.retry_mode = retry_mode
-        self.max_attempts = max_attempts
+
+        self.session: AioSession = aiobotocore.session.get_session()
+        """The session that will be used for all s3 requests."""
+
+        self.region_name: str = region_name
+        """The region that all clients will be rooted in."""
+
+        self.requester_pays: bool = requester_pays
+        """If True, enable access to `requester pays buckets
+        <https://docs.aws.amazon.com/AmazonS3/latest/userguide/RequesterPaysBuckets.html>`_."""
+
+        self.retry_mode: str = retry_mode
+        """The retry mode, one of "adaptive", "legacy", or "standard".
+
+        See `the boto3 docs
+        <https://boto3.amazonaws.com/v1/documentation/api/latest/guide/retries.html>`_
+        for more information on the available modes.
+        """
+
+        self.max_attempts: int = max_attempts
+        """The maximum number of attempts."""
 
     async def open_url(
         self,
         url: URL,
         content_type: Optional[str] = None,
         messages: Optional[MessageQueue] = None,
     ) -> AsyncIterator[bytes]:
```

### Comparing `stac_asset-0.3.1/src/stac_asset/strategy.py` & `stac_asset-0.3.2/src/stac_asset/strategy.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.1/src/stac_asset/types.py` & `stac_asset-0.3.2/src/stac_asset/types.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.1/src/stac_asset/validate.py` & `stac_asset-0.3.2/src/stac_asset/validate.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.1/src/stac_asset.egg-info/PKG-INFO` & `stac_asset-0.3.2/src/stac_asset.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-asset
-Version: 0.3.1
+Version: 0.3.2
 Summary: Read and download STAC assets across platforms and providers
 Author-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: Github, https://github.com/stac-utils/stac-asset
 Project-URL: CHANGELOG, https://github.com/stac-utils/stac-asset/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/stac-utils/stac-asset/issues
 Keywords: stac,async
@@ -30,26 +30,27 @@
 Requires-Dist: click-logging~=1.0.1; extra == "cli"
 Requires-Dist: tabulate~=0.9.0; extra == "cli"
 Requires-Dist: tqdm~=4.66.1; extra == "cli"
 Provides-Extra: dev
 Requires-Dist: mypy~=1.3; extra == "dev"
 Requires-Dist: pre-commit~=3.3; extra == "dev"
 Requires-Dist: pystac[validation]>=1.8.4; extra == "dev"
-Requires-Dist: pytest~=7.3; extra == "dev"
+Requires-Dist: pytest~=8.2; extra == "dev"
 Requires-Dist: pytest-asyncio~=0.21; extra == "dev"
 Requires-Dist: pytest-cov>=5.0; extra == "dev"
+Requires-Dist: pytest-recording~=0.13.1; extra == "dev"
 Requires-Dist: ruff==0.4.4; extra == "dev"
 Requires-Dist: types-aiofiles~=23.1; extra == "dev"
 Requires-Dist: types-python-dateutil~=2.9; extra == "dev"
 Requires-Dist: types-tqdm~=4.66.0; extra == "dev"
 Requires-Dist: types-tabulate~=0.9.0; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: pydata-sphinx-theme~=0.13; extra == "docs"
 Requires-Dist: sphinx~=7.3; extra == "docs"
-Requires-Dist: sphinx-click~=5.0; extra == "docs"
+Requires-Dist: sphinx-click~=6.0; extra == "docs"
 
 # stac-asset
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/stac-utils/stac-asset/ci.yaml?style=for-the-badge)](https://github.com/stac-utils/stac-asset/actions/workflows/ci.yaml)
 [![Read the Docs](https://img.shields.io/readthedocs/stac-asset?style=for-the-badge)](https://stac-asset.readthedocs.io/en/stable/)
 [![PyPI](https://img.shields.io/pypi/v/stac-asset?style=for-the-badge)](https://pypi.org/project/stac-asset)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg?style=for-the-badge)](./CODE_OF_CONDUCT)
@@ -175,16 +176,16 @@
 cd stac-asset
 pip install '.[dev]'
 pre-commit install
 ```
 
 ### Testing
 
-All network-touching tests are disabled by default, because we can't use [pytest-vcr](https://pytest-vcr.readthedocs.io/en/latest/) (<https://github.com/kevin1024/vcrpy/issues/597>), and repeatedly hitting the network during testing and CI is bad behavior.
-To enable network-touching tests:
+Some network-touching tests are disabled by default.
+To enable these tests:
 
 ```shell
 pytest --network-access
 ```
 
 Some tests are client-specific and need your environment to be configured correctly.
 See [each client's documentation](#clients) for instructions on setting up your environment for each client.
```

### Comparing `stac_asset-0.3.1/src/stac_asset.egg-info/SOURCES.txt` & `stac_asset-0.3.2/src/stac_asset.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.1/tests/test_blocking.py` & `stac_asset-0.3.2/tests/test_blocking.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.1/tests/test_cli.py` & `stac_asset-0.3.2/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,15 @@
             "https://landsatlook.usgs.gov/stac-server/collections/landsat-c2l2-sr/items/LC09_L2SP_092068_20230607_20230609_02_T1_SR",
             str(tmp_path),
             "--s3-requester-pays",
             "-i",
             "thumbnail",
             "--alternate-assets",
             "s3",
+            "--fail-fast",
         ],
     )
     assert result.exit_code == 0
 
 
 def test_info(item_path: Path) -> None:
     runner = CliRunner()
```

### Comparing `stac_asset-0.3.1/tests/test_earthdata_client.py` & `stac_asset-0.3.2/tests/test_earthdata_client.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.1/tests/test_filesystem_client.py` & `stac_asset-0.3.2/tests/test_filesystem_client.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.1/tests/test_functions.py` & `stac_asset-0.3.2/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.1/tests/test_planetary_computer_client.py` & `stac_asset-0.3.2/tests/test_planetary_computer_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import os.path
 from pathlib import Path
 
 import pytest
 from stac_asset import Config, PlanetaryComputerClient
 
 pytestmark = [
-    pytest.mark.network_access,
     pytest.mark.asyncio,
 ]
 
 
 @pytest.fixture
 def asset_href() -> str:
     return "https://sentinel2l2a01.blob.core.windows.net/sentinel2-l2/48/X/VR/2023/05/24/S2B_MSIL2A_20230524T084609_N0509_R107_T48XVR_20230524T120352.SAFE/GRANULE/L2A_T48XVR_A032451_20230524T084603/QI_DATA/T48XVR_20230524T084609_PVI.tif"
 
 
+@pytest.mark.network_access
 async def test_download(tmp_path: Path, asset_href: str) -> None:
     async with await PlanetaryComputerClient.from_config(Config()) as client:
         await client.download_href(asset_href, tmp_path / "out.tif")
 
     assert os.path.getsize(tmp_path / "out.tif") == 4096
 
 
+@pytest.mark.vcr
 async def test_href_exists(tmp_path: Path, asset_href: str) -> None:
     async with await PlanetaryComputerClient.from_config(Config()) as client:
         assert await client.href_exists(asset_href)
```

### Comparing `stac_asset-0.3.1/tests/test_s3_client.py` & `stac_asset-0.3.2/tests/test_s3_client.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.1/tests/test_validate.py` & `stac_asset-0.3.2/tests/test_validate.py`

 * *Files identical despite different names*

