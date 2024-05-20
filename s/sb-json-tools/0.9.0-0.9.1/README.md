# Comparing `tmp/sb-json-tools-0.9.0.tar.gz` & `tmp/sb-json-tools-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sb-json-tools-0.9.0.tar", last modified: Tue May 18 08:22:33 2021, max compression
+gzip compressed data, was "dist/sb-json-tools-0.9.1.tar", last modified: Wed May 19 08:55:06 2021, max compression
```

## Comparing `sb-json-tools-0.9.0.tar` & `sb-json-tools-0.9.1.tar`

### file list

```diff
@@ -1,93 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-18 08:22:33.000000 sb-json-tools-0.9.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-18 08:22:33.000000 sb-json-tools-0.9.0/sb_json_tools/
--rw-r--r--   0 runner    (1001) docker     (121)       41 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/sb_json_tools/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      129 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/sb_json_tools/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/sb_json_tools/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-18 08:22:33.000000 sb-json-tools-0.9.0/sb_json_tools/jt_val/
--rw-r--r--   0 runner    (1001) docker     (121)      233 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/sb_json_tools/jt_val/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      284 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/sb_json_tools/jt_val/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      678 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/sb_json_tools/jt_val/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2308 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/sb_json_tools/jt_val/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/sb_json_tools/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      588 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/sb_json_tools/jsondiff.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1176 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/sb_json_tools/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      466 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/sb_json_tools/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      334 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/sb_json_tools/cli.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/sb_json_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/sb_json_tools/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     4518 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/sb_json_tools/jsondiff.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-18 08:22:33.000000 sb-json-tools-0.9.0/sb_json_tools/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     3444 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/sb_json_tools/tests/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-18 08:22:33.000000 sb-json-tools-0.9.0/sb_json_tools/tests/jt_val/
--rw-r--r--   0 runner    (1001) docker     (121)      700 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/sb_json_tools/tests/jt_val/test_numeric_types.py
--rw-r--r--   0 runner    (1001) docker     (121)      266 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/sb_json_tools/tests/jt_val/test_streaming_validate.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1166 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/sb_json_tools/tests/jt_val/test_streaming_validate.py
--rw-r--r--   0 runner    (1001) docker     (121)      143 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/sb_json_tools/tests/jt_val/test_numeric_types.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      225 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/sb_json_tools/tests/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/sb_json_tools/tests/conftest.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      203 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/sb_json_tools/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/sb_json_tools/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2002 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/sb_json_tools/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       59 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/sb_json_tools/tests/test_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1918 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/sb_json_tools/tests/test_jsondiff.py
--rw-r--r--   0 runner    (1001) docker     (121)      566 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/sb_json_tools/tests/test_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      343 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/sb_json_tools/tests/test_jsondiff.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-18 08:22:33.000000 sb-json-tools-0.9.0/sb_json_tools/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)      158 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/sb_json_tools/tests/data/schema_default.json
--rw-r--r--   0 runner    (1001) docker     (121)       25 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/sb_json_tools/tests/data/valid_object.json
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/sb_json_tools/tests/data/invalid_type.json
--rw-r--r--   0 runner    (1001) docker     (121)       48 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/sb_json_tools/tests/data/valid_array.json
--rw-r--r--   0 runner    (1001) docker     (121)       68 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/sb_json_tools/tests/data/validated.json
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/sb_json_tools/tests/data/invalid.json
--rw-r--r--   0 runner    (1001) docker     (121)       26 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/sb_json_tools/tests/data/invalid_property.json
--rw-r--r--   0 runner    (1001) docker     (121)       64 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/sb_json_tools/tests/data/validated.jsonl
--rw-r--r--   0 runner    (1001) docker     (121)      100 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/sb_json_tools/tests/data/array.jsonl
--rw-r--r--   0 runner    (1001) docker     (121)      208 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/sb_json_tools/tests/data/array.json
--rw-r--r--   0 runner    (1001) docker     (121)       62 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/sb_json_tools/tests/data/invalid_many.json
--rw-r--r--   0 runner    (1001) docker     (121)      337 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/sb_json_tools/tests/data/schema_test.json
--rw-r--r--   0 runner    (1001) docker     (121)       50 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/sb_json_tools/tests/data/dict.json
--rw-r--r--   0 runner    (1001) docker     (121)     3096 2021-05-18 08:22:33.000000 sb-json-tools-0.9.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-18 08:22:33.000000 sb-json-tools-0.9.0/benches/
--rw-r--r--   0 runner    (1001) docker     (121)      423 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/benches/update_doc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-18 08:22:33.000000 sb-json-tools-0.9.0/benches/data/
--rw-r--r--   0 runner    (1001) docker     (121) 17178958 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/benches/data/skbl.json
--rw-r--r--   0 runner    (1001) docker     (121)      225 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1514 2021-05-18 08:22:33.000000 sb-json-tools-0.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-18 08:22:33.000000 sb-json-tools-0.9.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-18 08:22:33.000000 sb-json-tools-0.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1693 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)     4208 2021-05-18 08:22:32.000000 sb-json-tools-0.9.0/ChangeLog
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-18 08:22:33.000000 sb-json-tools-0.9.0/sb_json_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3096 2021-05-18 08:22:32.000000 sb-json-tools-0.9.0/sb_json_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-18 08:22:32.000000 sb-json-tools-0.9.0/sb_json_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)     2255 2021-05-18 08:22:32.000000 sb-json-tools-0.9.0/sb_json_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)      187 2021-05-18 08:22:32.000000 sb-json-tools-0.9.0/sb_json_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2021-05-18 08:22:32.000000 sb-json-tools-0.9.0/sb_json_tools.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-18 08:22:32.000000 sb-json-tools-0.9.0/sb_json_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2021-05-18 08:22:32.000000 sb-json-tools-0.9.0/sb_json_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2021-05-18 08:22:32.000000 sb-json-tools-0.9.0/sb_json_tools.egg-info/entry_points.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-18 08:22:33.000000 sb-json-tools-0.9.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      453 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-18 08:22:33.000000 sb-json-tools-0.9.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/docs/_static/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-18 08:22:33.000000 sb-json-tools-0.9.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/docs/_templates/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (121)       26 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/docs/readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-18 08:22:33.000000 sb-json-tools-0.9.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (121)      363 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/docs/source/json_tools.diff.rst
--rw-r--r--   0 runner    (1001) docker     (121)      542 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/docs/source/json_tools.iter.rst
--rw-r--r--   0 runner    (1001) docker     (121)      586 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/docs/source/json_tools.rst
--rw-r--r--   0 runner    (1001) docker     (121)      511 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/docs/source/json_tools.val.rst
--rw-r--r--   0 runner    (1001) docker     (121)       67 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (121)      787 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)      580 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     2092 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       65 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       51 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/pyrightconfig.json
--rw-r--r--   0 runner    (1001) docker     (121)      336 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (121)    17763 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)     1430 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      259 2021-05-18 08:22:32.000000 sb-json-tools-0.9.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)     1576 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      104 2021-05-18 08:22:20.000000 sb-json-tools-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-19 08:55:06.000000 sb-json-tools-0.9.1/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-19 08:55:06.000000 sb-json-tools-0.9.1/sb_json_tools/
+-rw-r--r--   0 runner    (1001) docker     (121)      129 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/sb_json_tools/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-19 08:55:06.000000 sb-json-tools-0.9.1/sb_json_tools/jt_val/
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/sb_json_tools/jt_val/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2308 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/sb_json_tools/jt_val/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1176 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/sb_json_tools/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)      466 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/sb_json_tools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/sb_json_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/sb_json_tools/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)     4518 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/sb_json_tools/jsondiff.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-19 08:55:06.000000 sb-json-tools-0.9.1/sb_json_tools/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     3444 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/sb_json_tools/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-19 08:55:06.000000 sb-json-tools-0.9.1/sb_json_tools/tests/jt_val/
+-rw-r--r--   0 runner    (1001) docker     (121)      700 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/sb_json_tools/tests/jt_val/test_numeric_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)      266 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/sb_json_tools/tests/jt_val/test_streaming_validate.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1166 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/sb_json_tools/tests/jt_val/test_streaming_validate.py
+-rw-r--r--   0 runner    (1001) docker     (121)      143 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/sb_json_tools/tests/jt_val/test_numeric_types.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/sb_json_tools/tests/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/sb_json_tools/tests/conftest.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      203 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/sb_json_tools/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/sb_json_tools/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2002 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/sb_json_tools/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/sb_json_tools/tests/test_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1918 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/sb_json_tools/tests/test_jsondiff.py
+-rw-r--r--   0 runner    (1001) docker     (121)      566 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/sb_json_tools/tests/test_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      343 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/sb_json_tools/tests/test_jsondiff.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-19 08:55:06.000000 sb-json-tools-0.9.1/sb_json_tools/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (121)      158 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/sb_json_tools/tests/data/schema_default.json
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/sb_json_tools/tests/data/valid_object.json
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/sb_json_tools/tests/data/invalid_type.json
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/sb_json_tools/tests/data/valid_array.json
+-rw-r--r--   0 runner    (1001) docker     (121)       68 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/sb_json_tools/tests/data/validated.json
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/sb_json_tools/tests/data/invalid.json
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/sb_json_tools/tests/data/invalid_property.json
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/sb_json_tools/tests/data/validated.jsonl
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/sb_json_tools/tests/data/array.jsonl
+-rw-r--r--   0 runner    (1001) docker     (121)      208 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/sb_json_tools/tests/data/array.json
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/sb_json_tools/tests/data/invalid_many.json
+-rw-r--r--   0 runner    (1001) docker     (121)      337 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/sb_json_tools/tests/data/schema_test.json
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/sb_json_tools/tests/data/dict.json
+-rw-r--r--   0 runner    (1001) docker     (121)     3096 2021-05-19 08:55:06.000000 sb-json-tools-0.9.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-19 08:55:06.000000 sb-json-tools-0.9.1/benches/
+-rw-r--r--   0 runner    (1001) docker     (121)      423 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/benches/update_doc.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-19 08:55:06.000000 sb-json-tools-0.9.1/benches/data/
+-rw-r--r--   0 runner    (1001) docker     (121) 17178958 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/benches/data/skbl.json
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1514 2021-05-19 08:55:06.000000 sb-json-tools-0.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-19 08:55:06.000000 sb-json-tools-0.9.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-19 08:55:06.000000 sb-json-tools-0.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2563 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2021-05-19 08:55:06.000000 sb-json-tools-0.9.1/ChangeLog
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-19 08:55:06.000000 sb-json-tools-0.9.1/sb_json_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3096 2021-05-19 08:55:06.000000 sb-json-tools-0.9.1/sb_json_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-19 08:55:06.000000 sb-json-tools-0.9.1/sb_json_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)     2056 2021-05-19 08:55:06.000000 sb-json-tools-0.9.1/sb_json_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      187 2021-05-19 08:55:06.000000 sb-json-tools-0.9.1/sb_json_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2021-05-19 08:55:06.000000 sb-json-tools-0.9.1/sb_json_tools.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-19 08:55:06.000000 sb-json-tools-0.9.1/sb_json_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2021-05-19 08:55:06.000000 sb-json-tools-0.9.1/sb_json_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2021-05-19 08:55:06.000000 sb-json-tools-0.9.1/sb_json_tools.egg-info/entry_points.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-19 08:55:06.000000 sb-json-tools-0.9.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)      453 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-19 08:55:06.000000 sb-json-tools-0.9.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/docs/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-19 08:55:06.000000 sb-json-tools-0.9.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/docs/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/docs/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-19 08:55:06.000000 sb-json-tools-0.9.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (121)      363 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/docs/source/json_tools.diff.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      542 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/docs/source/json_tools.iter.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      586 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/docs/source/json_tools.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      511 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/docs/source/json_tools.val.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       67 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      787 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (121)      580 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)     2092 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1069 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       51 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/pyrightconfig.json
+-rw-r--r--   0 runner    (1001) docker     (121)      336 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (121)    17763 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)     1430 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2021-05-19 08:55:06.000000 sb-json-tools-0.9.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (121)     1874 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2021-05-19 08:54:58.000000 sb-json-tools-0.9.1/setup.py
```

### Comparing `sb-json-tools-0.9.0/sb_json_tools/jt_val/__init__.py` & `sb-json-tools-0.9.1/sb_json_tools/jt_val/__init__.py`

 * *Files identical despite different names*

### Comparing `sb-json-tools-0.9.0/sb_json_tools/cli.py` & `sb-json-tools-0.9.1/sb_json_tools/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typer
 
 import json_streams
 from json_streams import jsonlib
 from sb_json_tools import jt_val
 
 
-__version__ = "0.9.0"
+__version__ = "0.9.1"
 
 
 cli = typer.Typer()
 
 
 @cli.command()
 def validate(
```

### Comparing `sb-json-tools-0.9.0/sb_json_tools/jsondiff.py` & `sb-json-tools-0.9.1/sb_json_tools/jsondiff.py`

 * *Files identical despite different names*

### Comparing `sb-json-tools-0.9.0/sb_json_tools/tests/test_cli.py` & `sb-json-tools-0.9.1/sb_json_tools/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `sb-json-tools-0.9.0/sb_json_tools/tests/jt_val/test_numeric_types.py` & `sb-json-tools-0.9.1/sb_json_tools/tests/jt_val/test_numeric_types.py`

 * *Files identical despite different names*

### Comparing `sb-json-tools-0.9.0/sb_json_tools/tests/jt_val/test_streaming_validate.py` & `sb-json-tools-0.9.1/sb_json_tools/tests/jt_val/test_streaming_validate.py`

 * *Files identical despite different names*

### Comparing `sb-json-tools-0.9.0/sb_json_tools/tests/utils.py` & `sb-json-tools-0.9.1/sb_json_tools/tests/utils.py`

 * *Files identical despite different names*

### Comparing `sb-json-tools-0.9.0/sb_json_tools/tests/test_jsondiff.py` & `sb-json-tools-0.9.1/sb_json_tools/tests/test_jsondiff.py`

 * *Files identical despite different names*

### Comparing `sb-json-tools-0.9.0/sb_json_tools/tests/test_cli.pyi` & `sb-json-tools-0.9.1/sb_json_tools/tests/test_cli.pyi`

 * *Files identical despite different names*

### Comparing `sb-json-tools-0.9.0/PKG-INFO` & `sb-json-tools-0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sb-json-tools
-Version: 0.9.0
+Version: 0.9.1
 Summary: Tools for working with JSON files.
 Home-page: https://github.com/spraakbanken/python-json-tools
 Author: Språkbanken at the University of Gothenburg
 Author-email: sb-info@svenska.gu.se
 Maintainer: Språkbanken
 Maintainer-email: sb-info@svenska.gu.se
 License: MIT
```

### Comparing `sb-json-tools-0.9.0/benches/data/skbl.json` & `sb-json-tools-0.9.1/benches/data/skbl.json`

 * *Files identical despite different names*

### Comparing `sb-json-tools-0.9.0/setup.cfg` & `sb-json-tools-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `sb-json-tools-0.9.0/.github/workflows/build.yml` & `sb-json-tools-0.9.1/.github/workflows/build.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,64 @@
 name: Build
 
 on: [push]
 
 jobs:
+  lint:
+    runs-on: ${{ matrix.os }}
+    name: Lint with pylint py-${{ matrix.python-version }} (${{ matrix.os}})
+    strategy:
+      matrix:
+        os: [ubuntu-latest]
+        python-version: [3.6]
+    steps:
+      - uses: actions/checkout@v2
+      - name: Set up Python ${{ matrix.python-version }}
+        uses: actions/setup-python@v1
+        with:
+          python-version: ${{ matrix.python-version }}
+      - name: Install dependencies
+        run: make install-dev
+      - name: Lint with pylint
+        run: make check-pylint
+        continue-on-error: true
+
   build:
-    runs-on: ubuntu-latest
+    runs-on: ${{ matrix.os }}
+    name: ${{ matrix.task.name }} py-${{ matrix.python-version }} (${{ matrix.os }})
     strategy:
       max-parallel: 4
       matrix:
+        os: [ubuntu-latest, macos-latest]
         python-version: [3.6, 3.7, 3.8, 3.9]
+        task:
+          - name: Check types with mypy
+            run: make check-mypy
+            allow-error: true
+          - name: Run tests
+            run: make test-w-coverage
+            allow-error: false
 
     steps:
-      - uses: actions/checkout@v1
+      - uses: actions/checkout@v2
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v1
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
-        run: |
-          python -m pip install --upgrade pip
-          make install-dev
-      - name: Lint with pylint
-        run: make lint-no-fail
-      - name: Test with pytest
-        run: make test-w-coverage
+        run: make install-dev
+      - name: ${{ matrix.task.name }}
+        run: ${{ matrix.task.run }}
+        continue-on-error: ${{ matrix.task.allow-error }}
+
   publish:
-    needs: build
+    needs: [build, lint]
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v1
+      - uses: actions/checkout@v2
       - name: Set up Python 3.6
         uses: actions/setup-python@v1
         with:
           python-version: 3.6
       - name: Build distribution
         run: |
           pip install --upgrade setuptools twine wheel pbr
```

### Comparing `sb-json-tools-0.9.0/sb_json_tools.egg-info/PKG-INFO` & `sb-json-tools-0.9.1/sb_json_tools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sb-json-tools
-Version: 0.9.0
+Version: 0.9.1
 Summary: Tools for working with JSON files.
 Home-page: https://github.com/spraakbanken/python-json-tools
 Author: Språkbanken at the University of Gothenburg
 Author-email: sb-info@svenska.gu.se
 Maintainer: Språkbanken
 Maintainer-email: sb-info@svenska.gu.se
 License: MIT
```

### Comparing `sb-json-tools-0.9.0/sb_json_tools.egg-info/SOURCES.txt` & `sb-json-tools-0.9.1/sb_json_tools.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -22,36 +22,29 @@
 docs/_templates/.gitkeep
 docs/source/json_tools.diff.rst
 docs/source/json_tools.iter.rst
 docs/source/json_tools.rst
 docs/source/json_tools.val.rst
 docs/source/modules.rst
 sb_json_tools/__init__.py
-sb_json_tools/__init__.pyi
 sb_json_tools/cli.py
-sb_json_tools/cli.pyi
 sb_json_tools/exceptions.py
-sb_json_tools/exceptions.pyi
 sb_json_tools/jsondiff.py
-sb_json_tools/jsondiff.pyi
 sb_json_tools/py.typed
 sb_json_tools/utils.py
-sb_json_tools/utils.pyi
 sb_json_tools.egg-info/PKG-INFO
 sb_json_tools.egg-info/SOURCES.txt
 sb_json_tools.egg-info/dependency_links.txt
 sb_json_tools.egg-info/entry_points.txt
 sb_json_tools.egg-info/not-zip-safe
 sb_json_tools.egg-info/pbr.json
 sb_json_tools.egg-info/requires.txt
 sb_json_tools.egg-info/top_level.txt
 sb_json_tools/jt_val/__init__.py
-sb_json_tools/jt_val/__init__.pyi
 sb_json_tools/jt_val/exceptions.py
-sb_json_tools/jt_val/exceptions.pyi
 sb_json_tools/tests/conftest.py
 sb_json_tools/tests/conftest.pyi
 sb_json_tools/tests/test_cli.py
 sb_json_tools/tests/test_cli.pyi
 sb_json_tools/tests/test_jsondiff.py
 sb_json_tools/tests/test_jsondiff.pyi
 sb_json_tools/tests/test_utils.py
```

### Comparing `sb-json-tools-0.9.0/docs/source/json_tools.iter.rst` & `sb-json-tools-0.9.1/docs/source/json_tools.iter.rst`

 * *Files identical despite different names*

### Comparing `sb-json-tools-0.9.0/docs/source/json_tools.rst` & `sb-json-tools-0.9.1/docs/source/json_tools.rst`

 * *Files identical despite different names*

### Comparing `sb-json-tools-0.9.0/docs/make.bat` & `sb-json-tools-0.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sb-json-tools-0.9.0/docs/Makefile` & `sb-json-tools-0.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sb-json-tools-0.9.0/docs/conf.py` & `sb-json-tools-0.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sb-json-tools-0.9.0/LICENSE` & `sb-json-tools-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sb-json-tools-0.9.0/.pylintrc` & `sb-json-tools-0.9.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `sb-json-tools-0.9.0/README.md` & `sb-json-tools-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `sb-json-tools-0.9.0/Makefile` & `sb-json-tools-0.9.1/Makefile`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.PHONY: venv help test bumpversion-minor bumpversion-major bumpversion-patch
+.PHONY: venv help test test-w-coverage bumpversion-minor bumpversion-major bumpversion-patch check-pylint check-mypy check-pylint-refactorings
 
 .default: help
 
 help:
 	@echo "usage:"
 PLATFORM := ${shell uname -o}
 INVENV_PATH = ${shell which invenv}
@@ -53,14 +53,23 @@
 
 lint: install-dev
 	${INVENV} pylint --rcfile=.pylintrc sb_json_tools
 
 lint-no-fail: install-dev
 	${INVENV} pylint --rcfile=.pylintrc --exit-zero sb_json_tools
 
+check-pylint: install-dev
+	${INVENV} pylint --rcfile=.pylintrc sb_json_tools
+
+check-mypy: install-dev
+	${INVENV} mypy sb_json_tools
+
+check-pylint-refactorings: install-dev
+	${INVENV} pylint --disable=C,W,E --enable=R sb_json_tools
+
 bumpversion: install-dev
 	${INVENV} bump2version patch
 
 bumpversion-minor: install-dev
 	${INVENV} bump2version minor
 
 bumpversion-major: install-dev
```

