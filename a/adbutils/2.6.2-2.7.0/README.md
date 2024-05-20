# Comparing `tmp/adbutils-2.6.2.tar.gz` & `tmp/adbutils-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adbutils-2.6.2.tar", last modified: Thu May  9 04:58:25 2024, max compression
+gzip compressed data, was "adbutils-2.7.0.tar", last modified: Mon May 20 10:16:27 2024, max compression
```

## Comparing `adbutils-2.6.2.tar` & `adbutils-2.7.0.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:58:25.888897 adbutils-2.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-09 04:58:15.000000 adbutils-2.6.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:58:25.884897 adbutils-2.6.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-09 04:58:15.000000 adbutils-2.6.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:58:25.884897 adbutils-2.6.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-09 04:58:15.000000 adbutils-2.6.2/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-09 04:58:15.000000 adbutils-2.6.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-09 04:58:15.000000 adbutils-2.6.2/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-09 04:58:25.000000 adbutils-2.6.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-09 04:58:25.000000 adbutils-2.6.2/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-09 04:58:15.000000 adbutils-2.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-09 04:58:25.888897 adbutils-2.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14753 2024-05-09 04:58:15.000000 adbutils-2.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:58:25.884897 adbutils-2.6.2/adbutils/
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-05-09 04:58:15.000000 adbutils-2.6.2/adbutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11923 2024-05-09 04:58:15.000000 adbutils-2.6.2/adbutils/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12689 2024-05-09 04:58:15.000000 adbutils-2.6.2/adbutils/_adb.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-09 04:58:15.000000 adbutils-2.6.2/adbutils/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)    16953 2024-05-09 04:58:15.000000 adbutils-2.6.2/adbutils/_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-09 04:58:15.000000 adbutils-2.6.2/adbutils/_proto.py
--rw-r--r--   0 runner    (1001) docker     (127)     8433 2024-05-09 04:58:15.000000 adbutils-2.6.2/adbutils/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-09 04:58:15.000000 adbutils-2.6.2/adbutils/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:58:25.884897 adbutils-2.6.2/adbutils/binaries/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 04:58:15.000000 adbutils-2.6.2/adbutils/binaries/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-09 04:58:15.000000 adbutils-2.6.2/adbutils/binaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-09 04:58:15.000000 adbutils-2.6.2/adbutils/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-05-09 04:58:15.000000 adbutils-2.6.2/adbutils/install.py
--rw-r--r--   0 runner    (1001) docker     (127)    12853 2024-05-09 04:58:15.000000 adbutils-2.6.2/adbutils/pidcat.py
--rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-05-09 04:58:15.000000 adbutils-2.6.2/adbutils/screenrecord.py
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-09 04:58:15.000000 adbutils-2.6.2/adbutils/screenshot.py
--rw-r--r--   0 runner    (1001) docker     (127)    18032 2024-05-09 04:58:15.000000 adbutils-2.6.2/adbutils/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-05-09 04:58:15.000000 adbutils-2.6.2/adbutils/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:58:25.884897 adbutils-2.6.2/adbutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-09 04:58:25.000000 adbutils-2.6.2/adbutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-09 04:58:25.000000 adbutils-2.6.2/adbutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 04:58:25.000000 adbutils-2.6.2/adbutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 04:58:25.000000 adbutils-2.6.2/adbutils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-09 04:58:25.000000 adbutils-2.6.2/adbutils.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-09 04:58:25.000000 adbutils-2.6.2/adbutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-09 04:58:25.000000 adbutils-2.6.2/adbutils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:58:25.880897 adbutils-2.6.2/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:58:25.884897 adbutils-2.6.2/assets/images/
--rw-r--r--   0 runner    (1001) docker     (127)   127305 2024-05-09 04:58:15.000000 adbutils-2.6.2/assets/images/pidcat.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     6132 2024-05-09 04:58:15.000000 adbutils-2.6.2/build_wheel.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-09 04:58:15.000000 adbutils-2.6.2/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:58:25.884897 adbutils-2.6.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-05-09 04:58:15.000000 adbutils-2.6.2/docs/PROTOCOL.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:58:25.884897 adbutils-2.6.2/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-09 04:58:15.000000 adbutils-2.6.2/examples/reset-offline.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-09 04:58:15.000000 adbutils-2.6.2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-09 04:58:15.000000 adbutils-2.6.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-09 04:58:25.888897 adbutils-2.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-09 04:58:15.000000 adbutils-2.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:58:25.888897 adbutils-2.6.2/test_real_device/
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-09 04:58:15.000000 adbutils-2.6.2/test_real_device/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-09 04:58:15.000000 adbutils-2.6.2/test_real_device/test_adb.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-09 04:58:15.000000 adbutils-2.6.2/test_real_device/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-05-09 04:58:15.000000 adbutils-2.6.2/test_real_device/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-09 04:58:15.000000 adbutils-2.6.2/test_real_device/test_forward_reverse.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-09 04:58:15.000000 adbutils-2.6.2/test_real_device/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-09 04:58:15.000000 adbutils-2.6.2/test_real_device/test_record.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-09 04:58:15.000000 adbutils-2.6.2/test_real_device/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:58:25.888897 adbutils-2.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-05-09 04:58:15.000000 adbutils-2.6.2/tests/adb_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-09 04:58:15.000000 adbutils-2.6.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-09 04:58:15.000000 adbutils-2.6.2/tests/test_adb_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-09 04:58:15.000000 adbutils-2.6.2/tests/test_adb_shell.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-09 04:58:15.000000 adbutils-2.6.2/tests/test_forward.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:16:27.140951 adbutils-2.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-20 10:16:21.000000 adbutils-2.7.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:16:27.136951 adbutils-2.7.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-20 10:16:21.000000 adbutils-2.7.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:16:27.136951 adbutils-2.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-20 10:16:21.000000 adbutils-2.7.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-20 10:16:21.000000 adbutils-2.7.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-20 10:16:21.000000 adbutils-2.7.0/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-20 10:16:27.000000 adbutils-2.7.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-20 10:16:27.000000 adbutils-2.7.0/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-20 10:16:21.000000 adbutils-2.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-20 10:16:27.140951 adbutils-2.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15478 2024-05-20 10:16:21.000000 adbutils-2.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:16:27.140951 adbutils-2.7.0/adbutils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-05-20 10:16:21.000000 adbutils-2.7.0/adbutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11923 2024-05-20 10:16:21.000000 adbutils-2.7.0/adbutils/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12835 2024-05-20 10:16:21.000000 adbutils-2.7.0/adbutils/_adb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-20 10:16:21.000000 adbutils-2.7.0/adbutils/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16918 2024-05-20 10:16:21.000000 adbutils-2.7.0/adbutils/_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-20 10:16:21.000000 adbutils-2.7.0/adbutils/_proto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8433 2024-05-20 10:16:21.000000 adbutils-2.7.0/adbutils/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-20 10:16:21.000000 adbutils-2.7.0/adbutils/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:16:27.140951 adbutils-2.7.0/adbutils/binaries/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-20 10:16:21.000000 adbutils-2.7.0/adbutils/binaries/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-20 10:16:21.000000 adbutils-2.7.0/adbutils/binaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-20 10:16:21.000000 adbutils-2.7.0/adbutils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-05-20 10:16:21.000000 adbutils-2.7.0/adbutils/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12853 2024-05-20 10:16:21.000000 adbutils-2.7.0/adbutils/pidcat.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:16:21.000000 adbutils-2.7.0/adbutils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-05-20 10:16:21.000000 adbutils-2.7.0/adbutils/screenrecord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-05-20 10:16:21.000000 adbutils-2.7.0/adbutils/screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19829 2024-05-20 10:16:21.000000 adbutils-2.7.0/adbutils/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8962 2024-05-20 10:16:21.000000 adbutils-2.7.0/adbutils/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:16:27.140951 adbutils-2.7.0/adbutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-20 10:16:27.000000 adbutils-2.7.0/adbutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-20 10:16:27.000000 adbutils-2.7.0/adbutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 10:16:27.000000 adbutils-2.7.0/adbutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 10:16:27.000000 adbutils-2.7.0/adbutils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-20 10:16:27.000000 adbutils-2.7.0/adbutils.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-20 10:16:27.000000 adbutils-2.7.0/adbutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-20 10:16:27.000000 adbutils-2.7.0/adbutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:16:27.136951 adbutils-2.7.0/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:16:27.140951 adbutils-2.7.0/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   127305 2024-05-20 10:16:21.000000 adbutils-2.7.0/assets/images/pidcat.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6132 2024-05-20 10:16:21.000000 adbutils-2.7.0/build_wheel.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-20 10:16:21.000000 adbutils-2.7.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:16:27.140951 adbutils-2.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-05-20 10:16:21.000000 adbutils-2.7.0/docs/PROTOCOL.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:16:27.140951 adbutils-2.7.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-20 10:16:21.000000 adbutils-2.7.0/examples/reset-offline.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-20 10:16:21.000000 adbutils-2.7.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-20 10:16:21.000000 adbutils-2.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-20 10:16:27.144951 adbutils-2.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-20 10:16:21.000000 adbutils-2.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:16:27.140951 adbutils-2.7.0/test_real_device/
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-20 10:16:21.000000 adbutils-2.7.0/test_real_device/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-20 10:16:21.000000 adbutils-2.7.0/test_real_device/test_adb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-20 10:16:21.000000 adbutils-2.7.0/test_real_device/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9601 2024-05-20 10:16:21.000000 adbutils-2.7.0/test_real_device/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-20 10:16:21.000000 adbutils-2.7.0/test_real_device/test_forward_reverse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-20 10:16:21.000000 adbutils-2.7.0/test_real_device/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-20 10:16:21.000000 adbutils-2.7.0/test_real_device/test_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-20 10:16:21.000000 adbutils-2.7.0/test_real_device/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:16:27.140951 adbutils-2.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-05-20 10:16:21.000000 adbutils-2.7.0/tests/adb_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-20 10:16:21.000000 adbutils-2.7.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-20 10:16:21.000000 adbutils-2.7.0/tests/test_adb_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-20 10:16:21.000000 adbutils-2.7.0/tests/test_adb_shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-20 10:16:21.000000 adbutils-2.7.0/tests/test_forward.py
```

### Comparing `adbutils-2.6.2/.coveragerc` & `adbutils-2.7.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.2/.github/workflows/main.yml` & `adbutils-2.7.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.2/.github/workflows/publish-to-pypi.yml` & `adbutils-2.7.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.2/.travis.yml` & `adbutils-2.7.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.2/LICENSE` & `adbutils-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.2/PKG-INFO` & `adbutils-2.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: adbutils
-Version: 2.6.2
+Version: 2.7.0
 Summary: Pure Python Adb Library
 Home-page: https://github.com/openatx/adbutils
 Author: codeskyblue
 Author-email: codeskyblue@gmail.com
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `adbutils-2.6.2/README.md` & `adbutils-2.7.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -199,14 +199,19 @@
 ```
 
 Take screenshot
 
 ```python
 # Method 1 (Recommend)
 pil_image = d.screenshot()
+# default display_id=0, error_ok=True
+try:
+    pil_image = d.screenshot(display_id=1, error_ok=False)
+except AdbError:
+    print("failed to takeScreenshot")
 
 # Method 2
 # adb exec-out screencap -p p.png
 png_data = d.shell("screencap -p", encoding=None)
 pathlib.Path("p.png").write_bytes(png_data)
 ```
 
@@ -280,17 +285,20 @@
 # example output: 1
 # other possible valus: 0, 1, 2, 3
 
 d.app_info("com.github.uiautomator")
 # example output: {"version_name": "1.1.7", "version_code": "1007"}
 
 d.keyevent("HOME")
+
 d.volume_up()
 d.volume_down()
-d.volume_mute()
+# default times=1, If you want to adjust the volume multiple times, you can use：d.volume_up(times=xxx)
+
+d.volume_mute()  # device mute
 
 d.send_keys("hello world$%^&*") # simulate: adb shell input text "hello%sworld\%\^\&\*"
 
 d.open_browser("https://www.baidu.com") # 打开百度
 # There still too many functions, please see source codes
 
 # check if screen is on
@@ -298,16 +306,26 @@
 
 # adb root
 d.root()
 
 # adb tcpip <port>
 d.tcpip(5555)
 
-print(d.battery())
+print(d.battery())  # get battery info
 BatteryInfo(ac_powered=False, usb_powered=False, wireless_powered=False, dock_powered=False, max_charging_current=0, max_charging_voltage=0, charge_counter=10000, status=4, health=2, present=True, level=100, scale=100, voltage=5000, temperature=25.0, technology='Li-ion')
+
+print(d.brightness_value)  # get brightness value, return int value in 0-255
+d.brightness_value = 100  # set brightness value
+
+# you can also set brightness mode
+from adbutils import BrightnessMode
+print(d.brightness_mode)  # output BrightnessMode.AUTO or BrightnessMode.MANUAL
+d.brightness_mode = BrightnessMode.MANUAL  # set brightness mode is manual
+d.brightness_mode = BrightnessMode.AUTO  # set brightness mode is auto
+
 ```
 
 Screenrecord (mp4)
 
 ```python
 d.start_recording("video.mp4")
 time.sleep(5)
```

### Comparing `adbutils-2.6.2/adbutils/__init__.py` & `adbutils-2.7.0/adbutils/__init__.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.2/adbutils/__main__.py` & `adbutils-2.7.0/adbutils/__main__.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.2/adbutils/_adb.py` & `adbutils-2.7.0/adbutils/_adb.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,29 +47,30 @@
         self._finalizer = weakref.finalize(self, self.conn.close)
 
     def _create_socket(self):
         adb_host = self.__host
         adb_port = self.__port
         s = socket.socket()
         try:
-            s.settimeout(.1) # prevent socket hang
+            s.settimeout(3) # prevent socket hang
             s.connect((adb_host, adb_port))
             s.settimeout(None)
             return s
         except socket.timeout as e:
-            raise AdbTimeout("connect to adb server timeout")
+            raise AdbTimeout("connect to adb server timeout") # windows raise timeout, mac raise connection error
         except socket.error as e:
             raise AdbConnectionError("connect to adb server failed: %s" % e)
 
 
     def _safe_connect(self):
         try:
             return self._create_socket()
         except AdbConnectionError:
-            subprocess.run([adb_path(), "start-server"], timeout=20.0)  # 20s should enough for adb start
+            flags = subprocess.CREATE_NO_WINDOW if os.name == 'nt' else 0
+            subprocess.run([adb_path(), "start-server"], timeout=20.0, creationflags=flags)  # 20s should enough for adb start
             return self._create_socket()
 
     @property
     def closed(self) -> bool:
         return not self._finalizer.alive
 
     def close(self):
```

### Comparing `adbutils-2.6.2/adbutils/_deprecated.py` & `adbutils-2.7.0/adbutils/_deprecated.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.2/adbutils/_device.py` & `adbutils-2.7.0/adbutils/_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -338,15 +338,15 @@
             raise UnidentifiedImageError("framebuffer size not match", size, len(buffer))
         image = Image.frombytes(color_format, (width, height), buffer)
         return image
 
     @deprecated(deprecated_in="2.6.0", removed_in="3.0.0", current_version=__version__, details="use sync.push instead")
     def push(self, local: str, remote: str):
         """ alias for sync.push """
-        self.sync.push(local, remote)
+        return self.sync.push(local, remote)
 
     def create_connection(
         self, network: Network, address: Union[int, str]
     ) -> socket.socket:
         """
         Used to connect a socket (unix of tcp) on the device
 
@@ -503,8 +503,7 @@
     """provide custom functions for some complex operations"""
 
     def __init__(
         self, client: BaseClient, serial: str = None, transport_id: int = None
     ):
         BaseDevice.__init__(self, client, serial, transport_id)
         ScreenrecordExtension.__init__(self)
-        ScreenshotExtesion.__init__(self)
```

### Comparing `adbutils-2.6.2/adbutils/_proto.py` & `adbutils-2.7.0/adbutils/_proto.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """Created on Fri May 06 2022 11:39:40 by codeskyblue
 """
 from __future__ import annotations
 
 __all__ = [
-    "Network", "DeviceEvent", "ForwardItem", "ReverseItem", "FileInfo",
-    "WindowSize", "RunningAppInfo", "ShellReturn", "AdbDeviceInfo", "AppInfo"
+    "Network", "BrightnessMode", "DeviceEvent", "ForwardItem", "ReverseItem", "FileInfo",
+    "WindowSize", "RunningAppInfo", "ShellReturn", "AdbDeviceInfo", "AppInfo", "BatteryInfo"
 ]
 
 import enum
 import datetime
 import pathlib
 from typing import List, NamedTuple, Optional, Union
 from dataclasses import dataclass
@@ -23,14 +23,19 @@
     DEV = "dev"
     LOCAL = "local"
     LOCAL_RESERVED = "localreserved"
     LOCAL_FILESYSTEM = "localfilesystem"
     LOCAL_ABSTRACT = "localabstract"  # same as UNIX
 
 
+class BrightnessMode(int, enum.Enum):
+    AUTO = 1
+    MANUAL = 0
+
+
 @dataclass(frozen=True)
 class DeviceEvent:
     present: bool
     serial: str
     status: str
 
 
@@ -78,16 +83,16 @@
     max_charging_voltage: Optional[int]
     charge_counter: Optional[int]
     status: Optional[int]
     health: Optional[int]
     present: Optional[bool]
     level: Optional[int]
     scale: Optional[int]
-    voltage: Optional[int] # mV
-    temperature: Optional[float] # e.g. 25.0
+    voltage: Optional[int]  # mV
+    temperature: Optional[float]  # e.g. 25.0
     technology: Optional[str]
 
 
 class WindowSize(NamedTuple):
     width: int
     height: int
```

### Comparing `adbutils-2.6.2/adbutils/_utils.py` & `adbutils-2.7.0/adbutils/_utils.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.2/adbutils/errors.py` & `adbutils-2.7.0/adbutils/errors.py`

 * *Files 16% similar despite different names*

```diff
@@ -31,8 +31,12 @@
         Reference: https://github.com/mzlogin/awesome-adb
         """
         m = re.search(r"Failure \[([\w_]+)", output)
         self.reason = m.group(1) if m else "Unknown"
         self.output = output
 
     def __str__(self):
-        return self.output
+        return self.output
+
+
+class AdbSyncError(AdbError):
+    """ sync error """
```

### Comparing `adbutils-2.6.2/adbutils/install.py` & `adbutils-2.7.0/adbutils/install.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.2/adbutils/pidcat.py` & `adbutils-2.7.0/adbutils/pidcat.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.2/adbutils/screenrecord.py` & `adbutils-2.7.0/adbutils/screenrecord.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.2/adbutils/shell.py` & `adbutils-2.7.0/adbutils/shell.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,24 +3,27 @@
 
 """Created on Sun Apr 07 2024 18:44:52 by codeskyblue
 """
 
 import abc
 import datetime
 import json
+import logging
 import re
 import time
 from typing import List, Optional, Union
-from adbutils._proto import WindowSize, AppInfo, RunningAppInfo, BatteryInfo
+from adbutils._proto import WindowSize, AppInfo, RunningAppInfo, BatteryInfo, BrightnessMode
 from adbutils.errors import AdbError, AdbInstallError
 from adbutils._utils import escape_special_characters
 from retry import retry
 
 from adbutils.sync import Sync
 
+logger = logging.getLogger(__name__)
+
 _DISPLAY_RE = re.compile(
     r".*DisplayViewport{.*?valid=true, .*?orientation=(?P<orientation>\d+), .*?deviceWidth=(?P<width>\d+), deviceHeight=(?P<height>\d+).*"
 )
 
 
 def is_percent(v):
     return isinstance(v, float) and v <= 1.0
@@ -71,14 +74,63 @@
     def reboot(self):
         self.shell("reboot")
 
     def switch_screen(self, enable: bool):
         """turn screen on/off"""
         return self.keyevent(224 if enable else 223)
 
+    @property
+    def brightness_value(self) -> int:
+        """
+        Return screen brightness value, [0, 255]
+        
+        Examples:
+            print(d.brightness_value) output：128
+        """
+        value = self.shell('settings get system screen_brightness')
+        return int(value.strip())
+
+    @brightness_value.setter
+    def brightness_value(self, value: int):
+        """
+        Set screen brightness values
+        :param value: brightness value
+        eg: d.brightness_value = 128
+        """
+        if not isinstance(value, int):
+            raise ValueError("Brightness value must be an integer")
+        if not 0 <= value <= 255:
+            raise ValueError("Brightness value must be between 0 and 255")
+        self.shell(f"settings put system screen_brightness {value}")
+
+    @property
+    def brightness_mode(self) -> BrightnessMode:
+        """
+        Return screen brightness mode
+        :return: BrightnessMode.AUTO or BrightnessMode.MANUAL
+        """
+        value = int(self.shell('settings get system screen_brightness_mode'))
+        return BrightnessMode(value)
+
+    @brightness_mode.setter
+    def brightness_mode(self, mode: BrightnessMode):
+        """
+        Set screen brightness mode
+        
+        Args:
+            mode: BrightnessMode.AUTO or BrightnessMode.MANUAL
+
+        Example:
+            d.brightness_mode = BrightnessMode.AUTO
+        """
+        if isinstance(mode, BrightnessMode):
+            self.shell(f"settings put system screen_brightness_mode {mode.value}")
+        else:
+            raise ValueError("Brightness mode must be an instance of BrightnessMode")
+
     def switch_airplane(self, enable: bool):
         """turn airplane-mode on/off"""
         base_setting_cmd = ["settings", "put", "global", "airplane_mode_on"]
         base_am_cmd = [
             "am",
             "broadcast",
             "-a",
@@ -100,42 +152,53 @@
         """turn WiFi on/off"""
         arglast = "enable" if enable else "disable"
         cmdargs = ["svc", "wifi", arglast]
         self.shell(cmdargs)
 
     def window_size(self) -> WindowSize:
         """
-        Return screen (width, height)
+        Return screen (width, height) in pixel, width and height will be swapped if rotation is 90 or 270
 
-        Virtual keyborad may get small d.info['displayHeight']
+        Returns:
+            WindowSize
+        
+        Raises:
+            AdbError
         """
-        w, h = self._raw_window_size()
-        s, l = min(w, h), max(w, h)
-        horizontal = self.rotation() % 2 == 1
-        return WindowSize(l, s) if horizontal else WindowSize(s, l)
-
-    def _raw_window_size(self) -> WindowSize:
+        try:
+            logger.debug("get window size from 'dumpsys display'")
+            return self._dumpsys_window_size()
+        except AdbError:
+            logger.debug("get window size from 'wm size'")
+            wsize = self._wm_size()
+            horizontal = self.rotation() % 2 == 1
+            return WindowSize(wsize.height, wsize.width) if horizontal else wsize
+    
+    def _dumpsys_window_size(self) -> WindowSize:
+        output = self.shell("dumpsys display")
+        for line in output.splitlines():
+            m = _DISPLAY_RE.search(line, 0)
+            if not m:
+                continue
+            w = int(m.group("width"))
+            h = int(m.group("height"))
+            return WindowSize(w, h)
+        raise AdbError("get window size from 'dumpsys display' failed", output)
+    
+    def _wm_size(self) -> WindowSize:
         output = self.shell("wm size")
         o = re.search(r"Override size: (\d+)x(\d+)", output)
-        m = re.search(r"Physical size: (\d+)x(\d+)", output)
         if o:
             w, h = o.group(1), o.group(2)
             return WindowSize(int(w), int(h))
-        elif m:
+        m = re.search(r"Physical size: (\d+)x(\d+)", output)
+        if m:
             w, h = m.group(1), m.group(2)
             return WindowSize(int(w), int(h))
-
-        for line in self.shell("dumpsys display").splitlines():
-            m = _DISPLAY_RE.search(line, 0)
-            if not m:
-                continue
-            w = int(m.group("width"))
-            h = int(m.group("height"))
-            return WindowSize(w, h)
-        raise AdbError("get window size failed")
+        raise AdbError("wm size output unexpected", output)
 
     def swipe(self, sx, sy, ex, ey, duration: float = 1.0) -> None:
         """
         swipe from start point to end point
 
         Args:
             sx, sy: start point(x, y)
@@ -201,31 +264,19 @@
 
     def rotation(self) -> int:
         """
         Returns:
             int [0, 1, 2, 3]
         """
         for line in self.shell("dumpsys display").splitlines():
-            m = _DISPLAY_RE.search(line, 0)
+            m = re.search(r".*?orientation=(?P<orientation>\d+)", line)
             if not m:
                 continue
             o = int(m.group("orientation"))
             return int(o)
-
-        output = self.shell(
-            "LD_LIBRARY_PATH=/data/local/tmp /data/local/tmp/minicap -i"
-        )
-        try:
-            if output.startswith("INFO:"):
-                output = output[output.index("{"):]
-            data = json.loads(output)
-            return data["rotation"] / 90
-        except ValueError:
-            pass
-
         raise AdbError("rotation get failed")
 
     def remove(self, path: str):
         """rm device file"""
         self.shell(["rm", path])
 
     def rmtree(self, path: str):
@@ -443,15 +494,15 @@
 
     def battery(self) -> BatteryInfo:
         """
         Get battery info
 
         Returns:
             BatteryInfo
-        
+
         Details:
             AC powered - Indicates that the device is currently not powered by AC power. If true, it indicates that the device is connected to an AC power adapter.
             USB powered - Indicates that the device is currently being powered or charged through the USB interface.
             Wireless powered - Indicates that the device is not powered through wireless charging. If wireless charging is supported and currently in use, this will be true.
             Max charging current - The maximum charging current supported by the device, usually in microamperes（ μ A).
             Max charging voltage - The maximum charging voltage supported by the device may be in millivolts (mV).
             Charge counter - The cumulative charge count of a battery, usually measured in milliampere hours (mAh)
@@ -460,29 +511,30 @@
             Present  - indicates that the battery is currently detected and installed in the device.
             Level - The percentage of current battery level.
             Scale - The full scale of the percentage of battery charge, indicating that the battery level is measured using 100 as the standard for full charge.
             Voltage - The current voltage of the battery, usually measured in millivolts (mV).
             Temperature - Battery temperature, usually measured in degrees Celsius (° C)
             Technology - Battery type, like (Li-ion) battery
         """
+
         def to_bool(v: str) -> bool:
             return v == "true"
-        
+
         output = self.shell(["dumpsys", "battery"])
         shell_kvs = {}
         for line in output.splitlines():
             key, val = line.strip().split(':', 1)
             shell_kvs[key.strip()] = val.strip()
-        
+
         def get_key(k: str, map_function):
             v = shell_kvs.get(k)
             if v is not None:
                 return map_function(v)
             return None
-        
+
         ac_powered = get_key("AC powered", to_bool)
         usb_powered = get_key("USB powered", to_bool)
         wireless_powered = get_key("Wireless powered", to_bool)
         dock_powered = get_key("Dock powered", to_bool)
         max_charging_current = get_key("Max charging current", int)
         max_charging_voltage = get_key("Max charging voltage", int)
         charge_counter = get_key("Charge counter", int)
@@ -506,8 +558,8 @@
             health=health,
             present=present,
             level=level,
             scale=scale,
             voltage=voltage,
             temperature=temperature,
             technology=technology,
-        )
+        )
```

### Comparing `adbutils-2.6.2/adbutils/sync.py` & `adbutils-2.7.0/adbutils/sync.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """Created on Sun Apr 07 2024 19:38:48 by codeskyblue
 """
 
 
+import logging
 import struct
 import datetime
 import typing
 import os
 import io
 import stat
 import pathlib
 from contextlib import contextmanager
 
 from adbutils._adb import BaseClient, AdbError
 from adbutils._proto import FileInfo
 from adbutils._utils import append_path
+from adbutils.errors import AdbSyncError
 
-
+logger = logging.getLogger(__name__)
 
 _OKAY = "OKAY"
 _FAIL = "FAIL"
 _DENT = "DENT"  # Directory Entity
 _DONE = "DONE"
 _DATA = "DATA"
 
@@ -76,41 +78,65 @@
                 except OSError:  # bug in Python 3.6
                     mtime = datetime.datetime.now()
                 yield FileInfo(mode, size, mtime, name)
 
     def list(self, path: str) -> typing.List[str]:
         return list(self.iter_directory(path))
 
-    def push(
+    def push(self, src: typing.Union[pathlib.Path, str, bytes, bytearray, typing.BinaryIO],
+             dst: typing.Union[pathlib.Path, str],
+             mode: int = 0o755,
+             check: bool = False) -> int:
+        """
+        Push file from local:src to device:dst
+
+        Args:
+            src: source file path
+            dst: destination file path or directory path
+            mode: file mode
+            check: check if push size is correct
+        
+        Returns:
+            total file size pushed
+        """
+        if isinstance(dst, pathlib.Path):
+            dst = dst.as_posix()
+        finfo = self.stat(dst)
+        if finfo.mode & stat.S_IFDIR != 0:
+            if not isinstance(src, (pathlib.Path, str)):
+                raise AdbSyncError("src should be a file path when dst is a directory")
+            dst = append_path(dst, pathlib.Path(src).name)
+            logger.debug("dst is a directory, update dst to %s", dst)
+        return self._push_file(src, dst, mode, check)
+    
+    def _push_file(
             self,
             src: typing.Union[pathlib.Path, str, bytes, bytearray, typing.BinaryIO],
-            dst: typing.Union[pathlib.Path, str],
+            dst: str,
             mode: int = 0o755,
             check: bool = False) -> int:  # yapf: disable
         # IFREG: File Regular
         # IFDIR: File Directory
         if isinstance(src, pathlib.Path):
             src = src.open("rb")
         elif isinstance(src, str):
             src = pathlib.Path(src).open("rb")
         elif isinstance(src, (bytes, bytearray)):
             src = io.BytesIO(src)
         else:
             if not hasattr(src, "read"):
                 raise TypeError("Invalid src type: %s" % type(src))
 
-        if isinstance(dst, pathlib.Path):
-            dst = dst.as_posix()
         path = dst + "," + str(stat.S_IFREG | mode)
         total_size = 0
         with self._prepare_sync(path, "SEND") as c:
             r = src if hasattr(src, "read") else open(src, "rb")
             try:
                 while True:
-                    chunk = r.read(4096)
+                    chunk = r.read(4096) # should not >64k
                     if not chunk:
                         mtime = int(datetime.datetime.now().timestamp())
                         c.conn.send(b"DONE" + struct.pack("<I", mtime))
                         break
                     c.conn.send(b"DATA" + struct.pack("<I", len(chunk)))
                     c.conn.send(chunk)
                     total_size += len(chunk)
```

### Comparing `adbutils-2.6.2/adbutils.egg-info/PKG-INFO` & `adbutils-2.7.0/adbutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: adbutils
-Version: 2.6.2
+Version: 2.7.0
 Summary: Pure Python Adb Library
 Home-page: https://github.com/openatx/adbutils
 Author: codeskyblue
 Author-email: codeskyblue@gmail.com
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `adbutils-2.6.2/adbutils.egg-info/SOURCES.txt` & `adbutils-2.7.0/adbutils.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 adbutils/_device.py
 adbutils/_proto.py
 adbutils/_utils.py
 adbutils/_version.py
 adbutils/errors.py
 adbutils/install.py
 adbutils/pidcat.py
+adbutils/py.typed
 adbutils/screenrecord.py
 adbutils/screenshot.py
 adbutils/shell.py
 adbutils/sync.py
 adbutils.egg-info/PKG-INFO
 adbutils.egg-info/SOURCES.txt
 adbutils.egg-info/dependency_links.txt
```

### Comparing `adbutils-2.6.2/assets/images/pidcat.png` & `adbutils-2.7.0/assets/images/pidcat.png`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.2/build_wheel.py` & `adbutils-2.7.0/build_wheel.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.2/docs/PROTOCOL.md` & `adbutils-2.7.0/docs/PROTOCOL.md`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.2/examples/reset-offline.py` & `adbutils-2.7.0/examples/reset-offline.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.2/setup.cfg` & `adbutils-2.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.2/test_real_device/conftest.py` & `adbutils-2.7.0/test_real_device/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,23 @@
 
 @pytest.fixture
 def device_tmp_path(device: AdbDevice):
     tmp_path = "/data/local/tmp/Hi-世界.txt"
     yield tmp_path
     device.remove(tmp_path)
 
+
+@pytest.fixture
+def device_tmp_dir(device: AdbDevice):
+    tmp_path = "/data/local/tmp/adbutils-test"
+    device.shell("mkdir -p {}".format(tmp_path))
+    yield tmp_path
+    device.rmtree(tmp_path)
+
+
 @pytest.fixture
 def device_tmp_dir_path(device: AdbDevice):
     tmp_dir_path = "/sdcard/test_d"
     yield tmp_dir_path
     device.rmtree(tmp_dir_path)
 
 @pytest.fixture
```

### Comparing `adbutils-2.6.2/test_real_device/test_adb.py` & `adbutils-2.7.0/test_real_device/test_adb.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.2/test_real_device/test_deprecated.py` & `adbutils-2.7.0/test_real_device/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.2/test_real_device/test_device.py` & `adbutils-2.7.0/test_real_device/test_device.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,19 +6,21 @@
 
 import os
 import io
 import pathlib
 import re
 import time
 import filecmp
+import uuid
 
 import pytest
 
 import adbutils
-from adbutils import AdbDevice, Network
+from adbutils import AdbDevice, Network, BrightnessMode
+from adbutils.errors import AdbSyncError
 
 
 def test_shell(device: AdbDevice):
     for text in ("foo", "?", "&", "but    123"):
         output = device.shell(['echo', '-n', text])
         assert output == text
 
@@ -68,14 +70,30 @@
     # make sure no error raised
     device.keyevent(4)
     device.volume_up(2)
     device.volume_down(3)
     device.volume_mute()
 
 
+def test_brightness(device: AdbDevice):
+    current_brightness = device.brightness_value
+    device.brightness_value = 100
+    assert device.brightness_value == 100
+    device.brightness_value = current_brightness
+
+    current_mode = device.brightness_mode
+    if current_mode == BrightnessMode.AUTO:
+        device.brightness_mode = BrightnessMode.MANUAL
+        assert device.brightness_mode == BrightnessMode.MANUAL
+    elif current_mode == BrightnessMode.MANUAL:
+        device.brightness_mode = BrightnessMode.AUTO
+        assert device.brightness_mode == BrightnessMode.AUTO
+    device.brightness_mode = current_mode
+
+
 def test_switch_screen(device: AdbDevice):
     device.switch_screen(False)
     device.switch_screen(True)
 
 
 def test_switch_airplane(device: AdbDevice):
     device.switch_airplane(True)
@@ -164,14 +182,25 @@
 
     data = b""
     for chunk in device.sync.iter_content(device_tmp_path):
         data += chunk
     assert b"Hello Android" == data
 
 
+def test_sync_push_to_dir(device: AdbDevice, device_tmp_dir, tmp_path: pathlib.Path):
+    random_data = str(uuid.uuid4()).encode()
+    src = io.BytesIO(random_data)
+    with pytest.raises(AdbSyncError):
+        device.sync.push(src, device_tmp_dir)
+    src_path = tmp_path.joinpath("random.txt")
+    src_path.write_bytes(random_data)
+    assert device.sync.push(src_path, device_tmp_dir) == len(random_data)
+    assert random_data == device.sync.read_bytes(device_tmp_dir + "/random.txt")
+
+
 def test_screenshot(device: AdbDevice):
     im = device.screenshot()
     assert im.mode == "RGB"
 
 
 def test_framebuffer(device: AdbDevice):
     im = device.framebuffer()
@@ -223,16 +252,14 @@
     device.shell(["log", "-p", "i", "-t", "TAG", "hello"])
     time.sleep(.1)
     logcat.stop()
     assert logcat_path.exists()
     assert re.compile(r"I/TAG.*hello").search(logcat_path.read_text(encoding="utf-8"))
 
 
-
-
 # todo: make independent of already present stuff on the phone
 def test_pull_push_dirs(
         device: AdbDevice,
         device_tmp_dir_path: str,
         local_src_in_dir: pathlib.Path,
         tmp_path: pathlib.Path,
 ):
@@ -265,15 +292,17 @@
             if not are_dir_trees_equal(new_dir1, new_dir2):
                 return False
         return True
 
     local_src_out_dir1 = tmp_path / 'dir1'
     local_src_out_dir2 = tmp_path / 'dir2'
 
-    device.push(local_src_in_dir, device_tmp_dir_path)
+    # TODO: push src support dir
+    # device.push(local_src_in_dir, device_tmp_dir_path)
+    device.adb_output("push", str(local_src_in_dir), device_tmp_dir_path)
 
     device.sync.pull_dir(device_tmp_dir_path, local_src_out_dir1)
 
     assert local_src_out_dir1.exists()
     assert local_src_out_dir1.is_dir()
 
     are_dir_trees_equal(local_src_in_dir, local_src_out_dir1)
```

### Comparing `adbutils-2.6.2/test_real_device/test_forward_reverse.py` & `adbutils-2.7.0/test_real_device/test_forward_reverse.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.2/test_real_device/test_utils.py` & `adbutils-2.7.0/test_real_device/test_utils.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.2/tests/adb_server.py` & `adbutils-2.7.0/tests/adb_server.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.2/tests/conftest.py` & `adbutils-2.7.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.6.2/tests/test_adb_server.py` & `adbutils-2.7.0/tests/test_adb_server.py`

 * *Files identical despite different names*

