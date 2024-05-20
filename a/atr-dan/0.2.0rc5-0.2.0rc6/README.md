# Comparing `tmp/atr-dan-0.2.0rc5.tar.gz` & `tmp/atr_dan-0.2.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atr-dan-0.2.0rc5.tar", last modified: Mon May  6 15:06:16 2024, max compression
+gzip compressed data, was "atr_dan-0.2.0rc6.tar", last modified: Mon May 20 15:30:38 2024, max compression
```

## Comparing `atr-dan-0.2.0rc5.tar` & `atr_dan-0.2.0rc6.tar`

### file list

```diff
@@ -1,83 +1,78 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 15:06:16.630738 atr-dan-0.2.0rc5/
--rw-rw-rw-   0 root         (0) root         (0)    23048 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/LICENCE
--rw-rw-rw-   0 root         (0) root         (0)    22135 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      152 2024-05-06 11:45:42.000000 atr-dan-0.2.0rc5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2318 2024-05-06 15:06:16.630738 atr-dan-0.2.0rc5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1980 2024-05-06 11:36:57.000000 atr-dan-0.2.0rc5/README.md
--rw-rw-rw-   0 root         (0) root         (0)        9 2024-05-06 14:47:02.000000 atr-dan-0.2.0rc5/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 15:06:16.622738 atr-dan-0.2.0rc5/atr_dan.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2318 2024-05-06 15:06:16.000000 atr-dan-0.2.0rc5/atr_dan.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1597 2024-05-06 15:06:16.000000 atr-dan-0.2.0rc5/atr_dan.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 15:06:16.000000 atr-dan-0.2.0rc5/atr_dan.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2024-05-06 15:06:16.000000 atr-dan-0.2.0rc5/atr_dan.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      597 2024-05-06 15:06:16.000000 atr-dan-0.2.0rc5/atr_dan.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-05-06 15:06:16.000000 atr-dan-0.2.0rc5/atr_dan.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 15:06:16.622738 atr-dan-0.2.0rc5/dan/
--rw-rw-rw-   0 root         (0) root         (0)      246 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/dan/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4416 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/dan/bio.py
--rw-rw-rw-   0 root         (0) root         (0)     1115 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/dan/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 15:06:16.622738 atr-dan-0.2.0rc5/dan/datasets/
--rw-rw-rw-   0 root         (0) root         (0)      830 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/dan/datasets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 15:06:16.622738 atr-dan-0.2.0rc5/dan/datasets/analyze/
--rw-rw-rw-   0 root         (0) root         (0)      988 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/dan/datasets/analyze/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5659 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/dan/datasets/analyze/statistics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 15:06:16.626738 atr-dan-0.2.0rc5/dan/datasets/download/
--rw-rw-rw-   0 root         (0) root         (0)     1330 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/dan/datasets/download/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      560 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/dan/datasets/download/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     9800 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/dan/datasets/download/images.py
--rw-rw-rw-   0 root         (0) root         (0)     2455 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/dan/datasets/download/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 15:06:16.626738 atr-dan-0.2.0rc5/dan/datasets/entities/
--rw-rw-rw-   0 root         (0) root         (0)      791 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/dan/datasets/entities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/dan/datasets/entities/extract.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 15:06:16.626738 atr-dan-0.2.0rc5/dan/datasets/extract/
--rw-rw-rw-   0 root         (0) root         (0)     3653 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/dan/datasets/extract/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12081 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/dan/datasets/extract/arkindex.py
--rw-rw-rw-   0 root         (0) root         (0)     3325 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/dan/datasets/extract/db.py
--rw-rw-rw-   0 root         (0) root         (0)     1030 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/dan/datasets/extract/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    10624 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/dan/datasets/extract/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 15:06:16.626738 atr-dan-0.2.0rc5/dan/datasets/tokens/
--rw-rw-rw-   0 root         (0) root         (0)      988 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/dan/datasets/tokens/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1061 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/dan/datasets/tokens/generate.py
--rw-rw-rw-   0 root         (0) root         (0)      324 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/dan/datasets/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 15:06:16.626738 atr-dan-0.2.0rc5/dan/ocr/
--rw-rw-rw-   0 root         (0) root         (0)      654 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/dan/ocr/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21260 2024-05-06 14:47:02.000000 atr-dan-0.2.0rc5/dan/ocr/decoder.py
--rw-rw-rw-   0 root         (0) root         (0)     5799 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/dan/ocr/encoder.py
--rw-rw-rw-   0 root         (0) root         (0)     6977 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/dan/ocr/evaluate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 15:06:16.626738 atr-dan-0.2.0rc5/dan/ocr/manager/
--rw-rw-rw-   0 root         (0) root         (0)       96 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/dan/ocr/manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5396 2024-05-06 14:47:02.000000 atr-dan-0.2.0rc5/dan/ocr/manager/dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     8217 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/dan/ocr/manager/metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     9648 2024-05-06 14:47:02.000000 atr-dan-0.2.0rc5/dan/ocr/manager/ocr.py
--rw-rw-rw-   0 root         (0) root         (0)    48049 2024-05-06 14:47:02.000000 atr-dan-0.2.0rc5/dan/ocr/manager/training.py
--rw-rw-rw-   0 root         (0) root         (0)     4948 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/dan/ocr/mlflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 15:06:16.626738 atr-dan-0.2.0rc5/dan/ocr/predict/
--rw-rw-rw-   0 root         (0) root         (0)     5242 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/dan/ocr/predict/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19081 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/dan/ocr/predict/attention.py
--rw-rw-rw-   0 root         (0) root         (0)    19531 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/dan/ocr/predict/inference.py
--rw-rw-rw-   0 root         (0) root         (0)     1446 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/dan/ocr/schedulers.py
--rw-rw-rw-   0 root         (0) root         (0)     4784 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/dan/ocr/train.py
--rw-rw-rw-   0 root         (0) root         (0)     7426 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/dan/ocr/transforms.py
--rw-rw-rw-   0 root         (0) root         (0)     3438 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/dan/ocr/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     6657 2024-05-06 14:47:02.000000 atr-dan-0.2.0rc5/dan/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      212 2024-05-06 11:36:57.000000 atr-dan-0.2.0rc5/doc-requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)       35 2024-05-06 11:36:57.000000 atr-dan-0.2.0rc5/mlflow-requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      570 2024-05-06 11:36:57.000000 atr-dan-0.2.0rc5/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      398 2024-05-06 11:36:57.000000 atr-dan-0.2.0rc5/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-06 15:06:16.630738 atr-dan-0.2.0rc5/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1961 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 15:06:16.630738 atr-dan-0.2.0rc5/tests/
--rw-rw-rw-   0 root         (0) root         (0)      200 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9196 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     3406 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/tests/test_analyze.py
--rw-rw-rw-   0 root         (0) root         (0)     3728 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/tests/test_attention.py
--rw-rw-rw-   0 root         (0) root         (0)     3229 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/tests/test_bio.py
--rw-rw-rw-   0 root         (0) root         (0)     4244 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/tests/test_db.py
--rw-rw-rw-   0 root         (0) root         (0)     7308 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/tests/test_download.py
--rw-rw-rw-   0 root         (0) root         (0)      421 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/tests/test_entities.py
--rw-rw-rw-   0 root         (0) root         (0)    16401 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/tests/test_evaluate.py
--rw-rw-rw-   0 root         (0) root         (0)    20055 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/tests/test_extract.py
--rw-rw-rw-   0 root         (0) root         (0)    28360 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/tests/test_prediction.py
--rw-rw-rw-   0 root         (0) root         (0)     2041 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/tests/test_tokens.py
--rw-rw-rw-   0 root         (0) root         (0)     5441 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/tests/test_training.py
--rw-rw-rw-   0 root         (0) root         (0)     2221 2024-05-06 13:02:12.000000 atr-dan-0.2.0rc5/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 15:30:38.531843 atr_dan-0.2.0rc6/
+-rw-rw-rw-   0 root         (0) root         (0)    23048 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/LICENCE
+-rw-rw-rw-   0 root         (0) root         (0)    22135 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4342 2024-05-20 15:30:38.527843 atr_dan-0.2.0rc6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2391 2024-05-20 13:41:43.000000 atr_dan-0.2.0rc6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 15:30:38.527843 atr_dan-0.2.0rc6/atr_dan.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4342 2024-05-20 15:30:38.000000 atr_dan-0.2.0rc6/atr_dan.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1518 2024-05-20 15:30:38.000000 atr_dan-0.2.0rc6/atr_dan.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 15:30:38.000000 atr_dan-0.2.0rc6/atr_dan.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2024-05-20 15:30:38.000000 atr_dan-0.2.0rc6/atr_dan.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      443 2024-05-20 15:30:38.000000 atr_dan-0.2.0rc6/atr_dan.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-20 15:30:38.000000 atr_dan-0.2.0rc6/atr_dan.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 15:30:38.519843 atr_dan-0.2.0rc6/dan/
+-rw-rw-rw-   0 root         (0) root         (0)      246 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/dan/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4416 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/dan/bio.py
+-rw-rw-rw-   0 root         (0) root         (0)     1115 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/dan/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 15:30:38.519843 atr_dan-0.2.0rc6/dan/datasets/
+-rw-rw-rw-   0 root         (0) root         (0)      830 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/dan/datasets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 15:30:38.519843 atr_dan-0.2.0rc6/dan/datasets/analyze/
+-rw-rw-rw-   0 root         (0) root         (0)      988 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/dan/datasets/analyze/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5659 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/dan/datasets/analyze/statistics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 15:30:38.519843 atr_dan-0.2.0rc6/dan/datasets/download/
+-rw-rw-rw-   0 root         (0) root         (0)     1330 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/dan/datasets/download/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      560 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/dan/datasets/download/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     9800 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/dan/datasets/download/images.py
+-rw-rw-rw-   0 root         (0) root         (0)     2455 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/dan/datasets/download/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 15:30:38.519843 atr_dan-0.2.0rc6/dan/datasets/entities/
+-rw-rw-rw-   0 root         (0) root         (0)      791 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/dan/datasets/entities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/dan/datasets/entities/extract.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 15:30:38.519843 atr_dan-0.2.0rc6/dan/datasets/extract/
+-rw-rw-rw-   0 root         (0) root         (0)     4040 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/dan/datasets/extract/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12603 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/dan/datasets/extract/arkindex.py
+-rw-rw-rw-   0 root         (0) root         (0)     4263 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/dan/datasets/extract/db.py
+-rw-rw-rw-   0 root         (0) root         (0)     1030 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/dan/datasets/extract/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    10692 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/dan/datasets/extract/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 15:30:38.519843 atr_dan-0.2.0rc6/dan/datasets/tokens/
+-rw-rw-rw-   0 root         (0) root         (0)      988 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/dan/datasets/tokens/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1061 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/dan/datasets/tokens/generate.py
+-rw-rw-rw-   0 root         (0) root         (0)      324 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/dan/datasets/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 15:30:38.523843 atr_dan-0.2.0rc6/dan/ocr/
+-rw-rw-rw-   0 root         (0) root         (0)      654 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/dan/ocr/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21260 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/dan/ocr/decoder.py
+-rw-rw-rw-   0 root         (0) root         (0)     5799 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/dan/ocr/encoder.py
+-rw-rw-rw-   0 root         (0) root         (0)     6977 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/dan/ocr/evaluate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 15:30:38.523843 atr_dan-0.2.0rc6/dan/ocr/manager/
+-rw-rw-rw-   0 root         (0) root         (0)       96 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/dan/ocr/manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5396 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/dan/ocr/manager/dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     8217 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/dan/ocr/manager/metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     9648 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/dan/ocr/manager/ocr.py
+-rw-rw-rw-   0 root         (0) root         (0)    48049 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/dan/ocr/manager/training.py
+-rw-rw-rw-   0 root         (0) root         (0)     4948 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/dan/ocr/mlflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 15:30:38.523843 atr_dan-0.2.0rc6/dan/ocr/predict/
+-rw-rw-rw-   0 root         (0) root         (0)     5242 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/dan/ocr/predict/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    19258 2024-05-20 13:27:37.000000 atr_dan-0.2.0rc6/dan/ocr/predict/attention.py
+-rw-rw-rw-   0 root         (0) root         (0)    20526 2024-05-20 14:52:18.000000 atr_dan-0.2.0rc6/dan/ocr/predict/inference.py
+-rw-rw-rw-   0 root         (0) root         (0)     1446 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/dan/ocr/schedulers.py
+-rw-rw-rw-   0 root         (0) root         (0)     4784 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/dan/ocr/train.py
+-rw-rw-rw-   0 root         (0) root         (0)     7426 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/dan/ocr/transforms.py
+-rw-rw-rw-   0 root         (0) root         (0)     3438 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/dan/ocr/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     6657 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/dan/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2561 2024-05-20 15:15:15.000000 atr_dan-0.2.0rc6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-20 15:30:38.531843 atr_dan-0.2.0rc6/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 15:30:38.527843 atr_dan-0.2.0rc6/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      200 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9796 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     3406 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/tests/test_analyze.py
+-rw-rw-rw-   0 root         (0) root         (0)     3728 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/tests/test_attention.py
+-rw-rw-rw-   0 root         (0) root         (0)     3229 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/tests/test_bio.py
+-rw-rw-rw-   0 root         (0) root         (0)     4917 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/tests/test_db.py
+-rw-rw-rw-   0 root         (0) root         (0)     7308 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/tests/test_download.py
+-rw-rw-rw-   0 root         (0) root         (0)      421 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/tests/test_entities.py
+-rw-rw-rw-   0 root         (0) root         (0)    16401 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/tests/test_evaluate.py
+-rw-rw-rw-   0 root         (0) root         (0)    20210 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/tests/test_extract.py
+-rw-rw-rw-   0 root         (0) root         (0)    32070 2024-05-20 13:41:43.000000 atr_dan-0.2.0rc6/tests/test_prediction.py
+-rw-rw-rw-   0 root         (0) root         (0)     2041 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/tests/test_tokens.py
+-rw-rw-rw-   0 root         (0) root         (0)     5441 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/tests/test_training.py
+-rw-rw-rw-   0 root         (0) root         (0)     2221 2024-05-20 12:52:52.000000 atr_dan-0.2.0rc6/tests/test_utils.py
```

### Comparing `atr-dan-0.2.0rc5/LICENCE` & `atr_dan-0.2.0rc6/LICENCE`

 * *Files identical despite different names*

### Comparing `atr-dan-0.2.0rc5/LICENSE` & `atr_dan-0.2.0rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `atr-dan-0.2.0rc5/PKG-INFO` & `atr_dan-0.2.0rc6/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,14 @@
-Metadata-Version: 2.1
-Name: atr-dan
-Version: 0.2.0rc5
-Summary: Teklia DAN
-Home-page: https://gitlab.teklia.com/atr/dan
-Author: Teklia
-Author-email: contact@teklia.com
-License: CeCILL-C
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: docs
-Provides-Extra: mlflow
-License-File: LICENSE
-License-File: LICENCE
-
 # DAN: a Segmentation-free Document Attention Network for Handwritten Document Recognition
 
 [![Python >= 3.10](https://img.shields.io/badge/Python-%3E%3D3.10-blue.svg)](https://www.python.org/downloads/release/python-3100/)
 
 For more details about this package, make sure to see the documentation available at <https://atr.pages.teklia.com/dan/>.
 
-This is an open-source project, licensed using [the MIT license](https://opensource.org/license/mit/).
+This is an open-source project, licensed using [the CeCILL-C license](https://cecill.info/index.en.html).
 
 ## Inference
 
 To apply DAN to an image, one needs to first add a few imports and to load an image. Note that the image should be in RGB.
 
 ```python
 import cv2
@@ -35,24 +20,43 @@
 Then one can initialize and load the trained model with the parameters used during training. The directory passed as parameter should have:
 
 - a `model.pt` file,
 - a `charset.pkl` file,
 - a `parameters.yml` file corresponding to the `inference_parameters.yml` file generated during training.
 
 ```python
-model_path = "models"
+from pathlib import Path
+
+model_path = Path("models")
 
 model = DAN("cpu")
 model.load(model_path, mode="eval")
 ```
 
 To run the inference on a GPU, one can replace `cpu` by the name of the GPU. In the end, one can run the prediction:
 
 ```python
-text, confidence_scores = model.predict(image, confidences=True)
+from pathlib import Path
+from dan.utils import parse_charset_pattern
+
+# Load image
+image_path = "images/page.jpg"
+_, image = dan_model.preprocess(str(image_path))
+
+input_tensor = image.unsqueeze(0)
+input_tensor = input_tensor.to("cpu")
+input_sizes = [image.shape[1:]]
+
+# Predict
+text, confidence_scores = model.predict(
+    input_tensor,
+    input_sizes,
+    char_separators=parse_charset_pattern(dan_model.charset),
+    confidences=True,
+)
 ```
 
 ## Training
 
 This package provides three subcommands. To get more information about any subcommand, use the `--help` option.
 
 ### Get started
```

### Comparing `atr-dan-0.2.0rc5/atr_dan.egg-info/SOURCES.txt` & `atr_dan-0.2.0rc6/atr_dan.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 LICENCE
 LICENSE
 MANIFEST.in
 README.md
-VERSION
-doc-requirements.txt
-mlflow-requirements.txt
 pyproject.toml
-requirements.txt
-setup.py
 atr_dan.egg-info/PKG-INFO
 atr_dan.egg-info/SOURCES.txt
 atr_dan.egg-info/dependency_links.txt
 atr_dan.egg-info/entry_points.txt
 atr_dan.egg-info/requires.txt
 atr_dan.egg-info/top_level.txt
 dan/__init__.py
```

### Comparing `atr-dan-0.2.0rc5/dan/bio.py` & `atr_dan-0.2.0rc6/dan/bio.py`

 * *Files identical despite different names*

### Comparing `atr-dan-0.2.0rc5/dan/cli.py` & `atr_dan-0.2.0rc6/dan/cli.py`

 * *Files identical despite different names*

### Comparing `atr-dan-0.2.0rc5/dan/datasets/__init__.py` & `atr_dan-0.2.0rc6/dan/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `atr-dan-0.2.0rc5/dan/datasets/analyze/__init__.py` & `atr_dan-0.2.0rc6/dan/datasets/analyze/__init__.py`

 * *Files identical despite different names*

### Comparing `atr-dan-0.2.0rc5/dan/datasets/analyze/statistics.py` & `atr_dan-0.2.0rc6/dan/datasets/analyze/statistics.py`

 * *Files identical despite different names*

### Comparing `atr-dan-0.2.0rc5/dan/datasets/download/__init__.py` & `atr_dan-0.2.0rc6/dan/datasets/download/__init__.py`

 * *Files identical despite different names*

### Comparing `atr-dan-0.2.0rc5/dan/datasets/download/exceptions.py` & `atr_dan-0.2.0rc6/dan/datasets/download/exceptions.py`

 * *Files identical despite different names*

### Comparing `atr-dan-0.2.0rc5/dan/datasets/download/images.py` & `atr_dan-0.2.0rc6/dan/datasets/download/images.py`

 * *Files identical despite different names*

### Comparing `atr-dan-0.2.0rc5/dan/datasets/download/utils.py` & `atr_dan-0.2.0rc6/dan/datasets/download/utils.py`

 * *Files identical despite different names*

### Comparing `atr-dan-0.2.0rc5/dan/datasets/entities/__init__.py` & `atr_dan-0.2.0rc6/dan/datasets/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `atr-dan-0.2.0rc5/dan/datasets/entities/extract.py` & `atr_dan-0.2.0rc6/dan/datasets/entities/extract.py`

 * *Files identical despite different names*

### Comparing `atr-dan-0.2.0rc5/dan/datasets/extract/__init__.py` & `atr_dan-0.2.0rc6/dan/datasets/extract/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 from uuid import UUID
 
 from dan.datasets.extract.arkindex import run
 
 MANUAL_SOURCE = "manual"
 
 
-def parse_worker_version(worker_version_id) -> str | bool:
-    if worker_version_id == MANUAL_SOURCE:
+def parse_source(source) -> str | bool:
+    if source == MANUAL_SOURCE:
         return False
 
     try:
-        UUID(worker_version_id)
+        UUID(source)
     except ValueError:
-        raise argparse.ArgumentTypeError(f"`{worker_version_id}` is not a valid UUID.")
+        raise argparse.ArgumentTypeError(f"`{source}` is not a valid UUID.")
 
-    return worker_version_id
+    return source
 
 
 def validate_char(char):
     if len(char) != 1:
         raise argparse.ArgumentTypeError(
             f"`{char}` (of length {len(char)}) is not a valid character. Must be a string of length 1."
         )
@@ -93,26 +93,40 @@
         type=pathlib.Path,
         help="Mapping between starting tokens and end tokens to extract text with their entities.",
         required=False,
     )
 
     parser.add_argument(
         "--transcription-worker-versions",
-        type=parse_worker_version,
+        type=parse_source,
         nargs="+",
         help=f"Filter transcriptions by worker_version. Use {MANUAL_SOURCE} for manual filtering.",
         default=[],
     )
     parser.add_argument(
         "--entity-worker-versions",
-        type=parse_worker_version,
+        type=parse_source,
         nargs="+",
         help=f"Filter transcriptions entities by worker_version. Use {MANUAL_SOURCE} for manual filtering.",
         default=[],
     )
+    parser.add_argument(
+        "--transcription-worker-runs",
+        type=parse_source,
+        nargs="+",
+        help=f"Filter transcriptions by worker_run. Use {MANUAL_SOURCE} for manual filtering.",
+        default=[],
+    )
+    parser.add_argument(
+        "--entity-worker-runs",
+        type=parse_source,
+        nargs="+",
+        help=f"Filter transcriptions entities by worker_run. Use {MANUAL_SOURCE} for manual filtering.",
+        default=[],
+    )
 
     parser.add_argument(
         "--subword-vocab-size",
         type=int,
         default=1000,
         help="Size of the vocabulary to train the sentencepiece subword tokenizer needed for language model.",
     )
```

### Comparing `atr-dan-0.2.0rc5/dan/datasets/extract/arkindex.py` & `atr_dan-0.2.0rc6/dan/datasets/extract/arkindex.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,26 +57,30 @@
         element_type: List[str] = [],
         output: Path | None = None,
         entity_separators: List[str] = ["\n", " "],
         unknown_token: str = "⁇",
         tokens: Path | None = None,
         transcription_worker_versions: List[str | bool] = [],
         entity_worker_versions: List[str | bool] = [],
+        transcription_worker_runs: List[str | bool] = [],
+        entity_worker_runs: List[str | bool] = [],
         keep_spaces: bool = False,
         allow_empty: bool = False,
         subword_vocab_size: int = 1000,
     ) -> None:
         self.dataset_ids = dataset_ids
         self.element_type = element_type
         self.output = output
         self.entity_separators = entity_separators
         self.unknown_token = unknown_token
         self.tokens = parse_tokens(tokens) if tokens else {}
         self.transcription_worker_versions = transcription_worker_versions
         self.entity_worker_versions = entity_worker_versions
+        self.transcription_worker_runs = transcription_worker_runs
+        self.entity_worker_runs = entity_worker_runs
         self.allow_empty = allow_empty
         self.mapping = LMTokenMapping()
         self.keep_spaces = keep_spaces
         self.subword_vocab_size = subword_vocab_size
 
         self.data: Dict = defaultdict(dict)
         self.charset = set()
@@ -97,15 +101,17 @@
 
     def extract_transcription(self, element: Element):
         """
         Extract the element's transcription.
         If the entities are needed, they are added to the transcription using tokens.
         """
         transcriptions = get_transcriptions(
-            element.id, self.transcription_worker_versions
+            element.id,
+            self.transcription_worker_versions,
+            self.transcription_worker_runs,
         )
         if len(transcriptions) == 0:
             if self.allow_empty:
                 return ""
             raise NoTranscriptionError(element.id)
 
         transcription = random.choice(transcriptions)
@@ -113,14 +119,15 @@
 
         if not self.tokens:
             return stripped_text
 
         entities = get_transcription_entities(
             transcription.id,
             self.entity_worker_versions,
+            self.entity_worker_runs,
             supported_types=list(self.tokens),
         )
 
         if not entities.count():
             return stripped_text
 
         return self.translate(
@@ -324,14 +331,16 @@
     element_type: List[str],
     output: Path,
     entity_separators: List[str],
     unknown_token: str,
     tokens: Path,
     transcription_worker_versions: List[str | bool],
     entity_worker_versions: List[str | bool],
+    transcription_worker_runs: List[str | bool],
+    entity_worker_runs: List[str | bool],
     keep_spaces: bool,
     allow_empty: bool,
     subword_vocab_size: int,
 ):
     assert database.exists(), f"No file found @ {database}"
     open_database(path=database)
 
@@ -343,11 +352,13 @@
         element_type=element_type,
         output=output,
         entity_separators=entity_separators,
         unknown_token=unknown_token,
         tokens=tokens,
         transcription_worker_versions=transcription_worker_versions,
         entity_worker_versions=entity_worker_versions,
+        transcription_worker_runs=transcription_worker_runs,
+        entity_worker_runs=entity_worker_runs,
         keep_spaces=keep_spaces,
         allow_empty=allow_empty,
         subword_vocab_size=subword_vocab_size,
     ).run()
```

### Comparing `atr-dan-0.2.0rc5/dan/datasets/extract/db.py` & `atr_dan-0.2.0rc6/dan/datasets/extract/db.py`

 * *Files 16% similar despite different names*

```diff
@@ -64,48 +64,77 @@
             ArkindexModel.worker_version == worker_version
             if worker_version
             else ArkindexModel.worker_version.is_null()
         )
     return condition
 
 
+def build_worker_run_filter(ArkindexModel, worker_runs: List[str | bool]):
+    """
+    `False` worker run means `manual` worker_run -> null field.
+    """
+    condition = None
+    for worker_run in worker_runs:
+        condition |= (
+            ArkindexModel.worker_run == worker_run
+            if worker_run
+            else ArkindexModel.worker_run.is_null()
+        )
+    return condition
+
+
 def get_transcriptions(
-    element_id: str, transcription_worker_versions: List[str | bool]
+    element_id: str,
+    transcription_worker_versions: List[str | bool],
+    transcription_worker_runs: List[str | bool],
 ) -> List[Transcription]:
     """
     Retrieve transcriptions from an SQLite export of an Arkindex corpus
     """
     query = Transcription.select(
-        Transcription.id, Transcription.text, Transcription.worker_version
+        Transcription.id,
+        Transcription.text,
+        Transcription.worker_version,
+        Transcription.worker_run,
     ).where((Transcription.element == element_id))
 
     if transcription_worker_versions:
         query = query.where(
             build_worker_version_filter(
                 Transcription, worker_versions=transcription_worker_versions
             )
         )
+
+    if transcription_worker_runs:
+        query = query.where(
+            build_worker_run_filter(
+                Transcription, worker_runs=transcription_worker_runs
+            )
+        )
+
     return query
 
 
 def get_transcription_entities(
     transcription_id: str,
     entity_worker_versions: List[str | bool],
+    entity_worker_runs: List[str | bool],
     supported_types: List[str],
 ) -> List[TranscriptionEntity]:
     """
     Retrieve transcription entities from an SQLite export of an Arkindex corpus
     """
     query = (
         TranscriptionEntity.select(
             EntityType.name.alias("type"),
             Entity.name.alias("name"),
             TranscriptionEntity.offset,
             TranscriptionEntity.length,
             TranscriptionEntity.worker_version,
+            TranscriptionEntity.worker_run,
         )
         .join(Entity, on=TranscriptionEntity.entity)
         .join(EntityType, on=Entity.type)
         .where(
             TranscriptionEntity.transcription == transcription_id,
             EntityType.name.in_(supported_types),
         )
@@ -114,10 +143,15 @@
     if entity_worker_versions:
         query = query.where(
             build_worker_version_filter(
                 TranscriptionEntity, worker_versions=entity_worker_versions
             )
         )
 
+    if entity_worker_runs:
+        query = query.where(
+            build_worker_run_filter(TranscriptionEntity, worker_runs=entity_worker_runs)
+        )
+
     return query.order_by(
         TranscriptionEntity.offset, TranscriptionEntity.length.desc()
     ).dicts()
```

### Comparing `atr-dan-0.2.0rc5/dan/datasets/extract/exceptions.py` & `atr_dan-0.2.0rc6/dan/datasets/extract/exceptions.py`

 * *Files identical despite different names*

### Comparing `atr-dan-0.2.0rc5/dan/datasets/extract/utils.py` & `atr_dan-0.2.0rc6/dan/datasets/extract/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,28 +205,30 @@
 @dataclass
 class XMLEntity:
     type: str
     name: str
     offset: int
     length: int
     worker_version: str
+    worker_run: str
     children: List["XMLEntity"] = field(default_factory=list)
 
     @property
     def end(self) -> int:
         return self.offset + self.length
 
     def add_child(self, child: TranscriptionEntity):
         self.children.append(
             XMLEntity(
                 type=child["type"],
                 name=child["name"],
                 offset=child["offset"] - self.offset,
                 length=child["length"],
                 worker_version=child["worker_version"],
+                worker_run=child["worker_run"],
             )
         )
 
     def insert(self, parent: Element):
         e = SubElement(parent, slugify(self.type))
 
         if not self.children:
```

### Comparing `atr-dan-0.2.0rc5/dan/datasets/tokens/__init__.py` & `atr_dan-0.2.0rc6/dan/datasets/tokens/__init__.py`

 * *Files identical despite different names*

### Comparing `atr-dan-0.2.0rc5/dan/datasets/tokens/generate.py` & `atr_dan-0.2.0rc6/dan/datasets/tokens/generate.py`

 * *Files identical despite different names*

### Comparing `atr-dan-0.2.0rc5/dan/ocr/__init__.py` & `atr_dan-0.2.0rc6/dan/ocr/__init__.py`

 * *Files identical despite different names*

### Comparing `atr-dan-0.2.0rc5/dan/ocr/decoder.py` & `atr_dan-0.2.0rc6/dan/ocr/decoder.py`

 * *Files identical despite different names*

### Comparing `atr-dan-0.2.0rc5/dan/ocr/encoder.py` & `atr_dan-0.2.0rc6/dan/ocr/encoder.py`

 * *Files identical despite different names*

### Comparing `atr-dan-0.2.0rc5/dan/ocr/evaluate.py` & `atr_dan-0.2.0rc6/dan/ocr/evaluate.py`

 * *Files identical despite different names*

### Comparing `atr-dan-0.2.0rc5/dan/ocr/manager/dataset.py` & `atr_dan-0.2.0rc6/dan/ocr/manager/dataset.py`

 * *Files identical despite different names*

### Comparing `atr-dan-0.2.0rc5/dan/ocr/manager/metrics.py` & `atr_dan-0.2.0rc6/dan/ocr/manager/metrics.py`

 * *Files identical despite different names*

### Comparing `atr-dan-0.2.0rc5/dan/ocr/manager/ocr.py` & `atr_dan-0.2.0rc6/dan/ocr/manager/ocr.py`

 * *Files identical despite different names*

### Comparing `atr-dan-0.2.0rc5/dan/ocr/manager/training.py` & `atr_dan-0.2.0rc6/dan/ocr/manager/training.py`

 * *Files identical despite different names*

### Comparing `atr-dan-0.2.0rc5/dan/ocr/mlflow.py` & `atr_dan-0.2.0rc6/dan/ocr/mlflow.py`

 * *Files identical despite different names*

### Comparing `atr-dan-0.2.0rc5/dan/ocr/predict/__init__.py` & `atr_dan-0.2.0rc6/dan/ocr/predict/__init__.py`

 * *Files identical despite different names*

### Comparing `atr-dan-0.2.0rc5/dan/ocr/predict/attention.py` & `atr_dan-0.2.0rc6/dan/ocr/predict/attention.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 # Copyright Teklia (contact@teklia.com) & Denis Coquenet
 # This code is licensed under CeCILL-C
 
 # -*- coding: utf-8 -*-
 import logging
 import re
 from enum import Enum
-from typing import Dict, List, Tuple
+from typing import List, Tuple
 
 import cv2
 import matplotlib.pyplot as plt
 import numpy as np
 import torch
 from PIL import Image
 from torchvision.transforms.functional import to_pil_image
 
-from dan.utils import EntityType
-
 logger = logging.getLogger(__name__)
 
 
 class Level(str, Enum):
     Char = "char"
     Word = "word"
     Line = "line"
@@ -436,42 +434,49 @@
     text: str,
     weights: np.ndarray,
     level: Level,
     scale: float,
     outname: str,
     alpha_factor: float,
     color_map: str,
+    char_separators: re.Pattern,
     max_object_height: int = 50,
     word_separators: re.Pattern = parse_delimiters(["\n", " "]),
     line_separators: re.Pattern = parse_delimiters(["\n"]),
-    tokens: Dict[str, EntityType] = {},
+    tokens_separators: re.Pattern | None = None,
     display_polygons: bool = False,
 ) -> None:
     """
     Create a gif by blending attention maps to the image for each text piece (char, word or line)
     :param image: Input image as torch.Tensor
     :param text: Text predicted by DAN
     :param weights: Attention weights of size (n_char, feature_height, feature_width)
     :param level: Level to display (must be in [char, word, line, ner])
     :param scale: Scaling factor for the output gif image
     :param outname: Name of the gif image
     :param alpha_factor: Alpha factor that controls how much the attention map is shown to the user during prediction. (higher value means more transparency for the attention map, commonly between 0.5 and 1.0)
     :param color_map: Colormap to use for the attention map
+    :param char_separators: Pattern used to find tokens of the charset
     :param max_object_height: Maximum height of predicted objects.
-    :param word_separators: List of word separators
-    :param line_separators: List of line separators
-    :param tokens: NER tokens used
+    :param word_separators: Pattern used to find words
+    :param line_separators: Pattern used to find lines
+    :param tokens_separators: Pattern used to find NER entities
     :param display_polygons: Whether to plot extracted polygons
     """
     image = to_pil_image(image)
     attention_map = []
 
     # Split text into characters, words or lines
     text_list, offsets = split_text(
-        text, level, word_separators, line_separators, tokens
+        text,
+        level,
+        char_separators,
+        word_separators,
+        line_separators,
+        tokens_separators,
     )
 
     # Iterate on characters, words or lines
     tot_len = 0
     max_value = weights.sum(0).max()
 
     for text_piece, offset in zip(text_list, offsets):
```

### Comparing `atr-dan-0.2.0rc5/dan/ocr/predict/inference.py` & `atr_dan-0.2.0rc6/dan/ocr/predict/inference.py`

 * *Files 4% similar despite different names*

```diff
@@ -166,32 +166,38 @@
 
         return preprocessed_image, normalized_image
 
     def predict(
         self,
         input_tensor: torch.Tensor,
         input_sizes: List[torch.Size],
+        char_separators: re.Pattern,
         confidences: bool = False,
         attentions: bool = False,
         attention_level: Level = Level.Line,
         extract_objects: bool = False,
         word_separators: re.Pattern = parse_delimiters(["\n", " "]),
         line_separators: re.Pattern = parse_delimiters(["\n"]),
-        tokens: Dict[str, EntityType] = {},
+        tokens_separators: re.Pattern | None = None,
         start_token: str | None = None,
         max_object_height: int = 50,
     ) -> dict:
         """
         Run prediction on an input image.
         :param input_tensor: A batch of images to predict.
         :param input_sizes: The original images sizes.
+        :param char_separators: The regular expression pattern to split characters.
         :param confidences: Return the characters probabilities.
         :param attentions: Return characters attention weights.
         :param attention_level: Level of text pieces (must be in [char, word, line, ner])
         :param extract_objects: Whether to extract polygons' coordinates.
+        :param word_separators: The regular expression pattern to split words.
+        :param line_separators: The regular expression pattern to split lines.
+        :param tokens_separators: The regular expression pattern to split NER tokens.
+        :param start_token: The starting token for the prediction.
         :param max_object_height: Maximum height of predicted objects.
         """
         input_tensor = input_tensor.to(self.device)
 
         start_token = (
             self.charset.index(start_token) if start_token else len(self.charset) + 1
         )
@@ -316,17 +322,18 @@
                     predicted_text[i],
                     attention_maps[i],
                     confidence_scores[i],
                     attention_level,
                     input_sizes[i][0],
                     input_sizes[i][1],
                     max_object_height=max_object_height,
+                    char_separators=char_separators,
                     word_separators=word_separators,
                     line_separators=line_separators,
-                    tokens=tokens,
+                    tokens_separators=tokens_separators,
                 )
                 for i in range(batch_size)
             ]
         return out
 
 
 def process_batch(
@@ -374,17 +381,18 @@
     prediction = dan_model.predict(
         input_tensor,
         input_sizes,
         confidences=confidence_score,
         attentions=attention_map,
         attention_level=attention_map_level,
         extract_objects=predict_objects,
+        char_separators=char_separators,
         word_separators=word_separators,
         line_separators=line_separators,
-        tokens=tokens,
+        tokens_separators=ner_separators,
         max_object_height=max_object_height,
         start_token=start_token,
     )
 
     logger.info("Prediction parsing...")
     for idx, image_path in enumerate(image_batch):
         predicted_text = prediction["text"][idx]
@@ -423,24 +431,27 @@
                         result["confidences"][level.value].append(
                             {"text": text, "confidence": conf}
                         )
 
             # Save gif with attention map
             if attention_map:
                 attentions = prediction["attentions"][idx]
-                gif_filename = f"{output}/{image_path.stem}_{attention_map_level}.gif"
+                gif_filename = (
+                    f"{output}/{image_path.stem}_{attention_map_level.value}.gif"
+                )
                 logger.info(f"Creating attention GIF in {gif_filename}")
                 plot_attention(
                     image=visu_tensor[idx],
                     text=predicted_text,
                     weights=attentions,
                     level=attention_map_level,
                     scale=attention_map_scale,
                     alpha_factor=alpha_factor,
                     color_map=color_map,
+                    char_separators=char_separators,
                     word_separators=word_separators,
                     line_separators=line_separators,
                     tokens_separators=ner_separators,
                     display_polygons=predict_objects,
                     max_object_height=max_object_height,
                     outname=gif_filename,
                 )
@@ -478,21 +489,26 @@
 ) -> None:
     """
     Predict a single image save the output
     :param image_dir: Path to the folder where the images to predict are stored.
     :param model: Path to the directory containing the model, the YAML parameters file and the charset file to use for prediction.
     :param output: Path to the output folder where the results will be saved.
     :param confidence_score: Whether to compute confidence score.
+    :param confidence_score_levels: Levels of objects to extract.
     :param attention_map: Whether to plot the attention map.
     :param attention_map_level: Level of objects to extract.
     :param attention_map_scale: Scaling factor for the attention map.
+    :param alpha_factor: Alpha factor for the attention map.
+    :param color_map: A matplotlib colormap to use for the attention maps.
     :param word_separators: List of word separators.
     :param line_separators: List of line separators.
+    :param temperature: Temperature scalar parameter.
     :param predict_objects: Whether to extract objects.
     :param max_object_height: Maximum height of predicted objects.
+    :param image_extension: Extension of the images to predict.
     :param gpu_device: Use a specific GPU if available.
     :param batch_size: Size of the batches for prediction.
     :param tokens: NER tokens used.
     :param start_token: Use a specific starting token at the beginning of the prediction. Useful when making predictions on different single pages.
     :param use_language_model: Whether to use an explicit language model to rescore text hypotheses.
     :param compile_model: Whether to compile the model.
     :param dynamic_mode: Whether to use the dynamic mode during model compilation.
```

### Comparing `atr-dan-0.2.0rc5/dan/ocr/schedulers.py` & `atr_dan-0.2.0rc6/dan/ocr/schedulers.py`

 * *Files identical despite different names*

### Comparing `atr-dan-0.2.0rc5/dan/ocr/train.py` & `atr_dan-0.2.0rc6/dan/ocr/train.py`

 * *Files identical despite different names*

### Comparing `atr-dan-0.2.0rc5/dan/ocr/transforms.py` & `atr_dan-0.2.0rc6/dan/ocr/transforms.py`

 * *Files identical despite different names*

### Comparing `atr-dan-0.2.0rc5/dan/ocr/utils.py` & `atr_dan-0.2.0rc6/dan/ocr/utils.py`

 * *Files identical despite different names*

### Comparing `atr-dan-0.2.0rc5/dan/utils.py` & `atr_dan-0.2.0rc6/dan/utils.py`

 * *Files identical despite different names*

### Comparing `atr-dan-0.2.0rc5/tests/conftest.py` & `atr_dan-0.2.0rc6/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,64 +29,74 @@
 
 
 @pytest.fixture()
 def mock_database(tmp_path_factory):
     def create_transcription_entity(
         transcription: Transcription,
         worker_version: str | None,
+        worker_run: str | None,
         type: str,
         name: str,
         offset: int,
     ) -> None:
         entity_type, _ = EntityType.get_or_create(
             name=type, defaults={"id": f"{type}_id"}
         )
         entity = Entity.create(
             id=str(uuid.uuid4()),
             name=name,
             type=entity_type,
             worker_version=worker_version,
+            worker_run=worker_run,
         )
         TranscriptionEntity.create(
             entity=entity,
             length=len(name),
             offset=offset,
             transcription=transcription,
             worker_version=worker_version,
+            worker_run=worker_run,
         )
 
     def create_transcriptions(element: Element, entities: List[dict]) -> None:
         if not entities:
             return
 
         # Add transcription with entities
         entities = sorted(entities, key=itemgetter("offset"))
 
         # We will add extra spaces to test the "keep_spaces" parameters of the "extract" command
         for offset, entity in enumerate(entities[1:], start=1):
             entity["offset"] += offset
 
-        for worker_version in [None, "worker_version_id"]:
+        for worker_version, worker_run in [
+            (None, None),
+            ("worker_version_id", "worker_run_id"),
+        ]:
+            transcription_suffix = ""
             # Use different transcriptions to filter by worker version
-            if worker_version == "worker_version_id":
+            if worker_version and worker_run:
+                transcription_suffix = "source"
                 for entity in entities:
                     entity["name"] = entity["name"].lower()
 
             transcription = Transcription.create(
-                id=element.id + (worker_version or ""),
+                id=element.id + transcription_suffix,
                 # Add extra spaces to test the "keep_spaces" parameters of the "extract" command
                 text="  ".join(map(itemgetter("name"), entities)),
                 element=element,
                 worker_version=worker_version,
+                worker_run=worker_run,
             )
 
             for entity in entities:
                 create_transcription_entity(
                     transcription=transcription,
                     worker_version=worker_version,
+                    worker_run=worker_run,
                     **entity,
                 )
 
     def create_element(id: str, parent: Element | None = None) -> None:
         element_path = (FIXTURES / "extraction" / "elements" / id).with_suffix(".json")
         element_json = json.loads(element_path.read_text())
 
@@ -179,14 +189,19 @@
         slug="worker_version",
         name="Worker version",
         repository_url="http://repository/url",
         revision="main",
         type="worker",
     )
 
+    WorkerRun.create(
+        id="worker_run_id",
+        worker_version="worker_version_id",
+    )
+
     # Create dataset
     split_names = [VAL_NAME, TEST_NAME, TRAIN_NAME]
     dataset = Dataset.create(
         id="dataset_id",
         name="Dataset",
         state="complete",
         sets=",".join(split_names),
@@ -212,90 +227,96 @@
     # Create transcription
     transcription = Transcription.create(
         id="tr-with-entities",
         text="The great king Charles III has eaten \nwith us.",
         element=Element.select().first(),
     )
 
-    # Create worker version
-    WorkerVersion.bulk_create(
-        [
-            WorkerVersion(
-                id=f"{nestation}-id",
-                slug=nestation,
-                name=nestation,
-                repository_url="http://repository/url",
-                revision="main",
-                type="worker",
-            )
-            for nestation in ("nested", "non-nested", "special-chars")
-        ]
-    )
+    # Create worker version and worker run
+    for nestation in ("nested", "non-nested", "special-chars"):
+        WorkerVersion.create(
+            id=f"worker-version-{nestation}-id",
+            slug=nestation,
+            name=nestation,
+            repository_url="http://repository/url",
+            revision="main",
+            type="worker",
+        )
+        WorkerRun.create(
+            id=f"worker-run-{nestation}-id",
+            worker_version=f"worker-version-{nestation}-id",
+        )
 
     # Create entities
     for entity in [
         # Non-nested entities
         {
-            "worker_version": "non-nested-id",
+            "source": "non-nested",
             "type": "adj",
             "name": "great",
             "offset": 4,
         },
         {
-            "worker_version": "non-nested-id",
+            "source": "non-nested",
             "type": "name",
             "name": "Charles",
             "offset": 15,
         },
         {
-            "worker_version": "non-nested-id",
+            "source": "non-nested",
             "type": "person",
             "name": "us",
             "offset": 43,
         },
         # Nested entities
         {
-            "worker_version": "nested-id",
+            "source": "nested",
             "type": "fullname",
             "name": "Charles III",
             "offset": 15,
         },
         {
-            "worker_version": "nested-id",
+            "source": "nested",
             "type": "name",
             "name": "Charles",
             "offset": 15,
         },
         {
-            "worker_version": "nested-id",
+            "source": "nested",
             "type": "person",
             "name": "us",
             "offset": 43,
         },
         # Special characters
         {
-            "worker_version": "special-chars-id",
+            "source": "special-chars",
             "type": "Arkindex's entity",
             "name": "great",
             "offset": 4,
         },
         {
-            "worker_version": "special-chars-id",
+            "source": "special-chars",
             "type": '"Name" (1)',
             "name": "Charles",
             "offset": 15,
         },
         {
-            "worker_version": "special-chars-id",
+            "source": "special-chars",
             "type": "Person /!\\",
             "name": "us",
             "offset": 43,
         },
     ]:
-        create_transcription_entity(transcription=transcription, **entity)
+        source = entity.pop("source")
+        create_transcription_entity(
+            transcription=transcription,
+            worker_version=f"worker-version-{source}-id",
+            worker_run=f"worker-run-{source}-id",
+            **entity,
+        )
 
     return database_path
 
 
 @pytest.fixture
 def training_config():
     return json.loads((FIXTURES.parent.parent / "configs" / "tests.json").read_text())
```

### Comparing `atr-dan-0.2.0rc5/tests/test_analyze.py` & `atr_dan-0.2.0rc6/tests/test_analyze.py`

 * *Files identical despite different names*

### Comparing `atr-dan-0.2.0rc5/tests/test_attention.py` & `atr_dan-0.2.0rc6/tests/test_attention.py`

 * *Files identical despite different names*

### Comparing `atr-dan-0.2.0rc5/tests/test_bio.py` & `atr_dan-0.2.0rc6/tests/test_bio.py`

 * *Files identical despite different names*

### Comparing `atr-dan-0.2.0rc5/tests/test_db.py` & `atr_dan-0.2.0rc6/tests/test_db.py`

 * *Files 15% similar despite different names*

```diff
@@ -53,70 +53,89 @@
         "train-page_1-line_2",
         "train-page_1-line_3",
         "train-page_1-line_4",
     ]
 
 
 @pytest.mark.parametrize(
-    "worker_versions",
-    ([False], ["worker_version_id"], [], [False, "worker_version_id"]),
+    "sources",
+    ([False], ["id"], [], [False, "id"]),
 )
-def test_get_transcriptions(worker_versions, mock_database):
+def test_get_transcriptions(sources, mock_database):
     """
     Assert transcriptions retrieval output against verified results
     """
+    worker_versions = [
+        f"worker_version_{source}" if isinstance(source, str) else source
+        for source in sources
+    ]
+    worker_runs = [
+        f"worker_run_{source}" if isinstance(source, str) else source
+        for source in sources
+    ]
+
     element_id = "train-page_1-line_1"
     transcriptions = get_transcriptions(
         element_id=element_id,
         transcription_worker_versions=worker_versions,
+        transcription_worker_runs=worker_runs,
     )
 
     expected_transcriptions = []
-    if not worker_versions or False in worker_versions:
+    if not sources or False in sources:
         expected_transcriptions.append(
             {
                 "text": "Caillet  Maurice  28.9.06",
                 "worker_version_id": None,
+                "worker_run_id": None,
             }
         )
 
-    if not worker_versions or "worker_version_id" in worker_versions:
+    if not sources or "id" in sources:
         expected_transcriptions.append(
             {
                 "text": "caillet  maurice  28.9.06",
                 "worker_version_id": "worker_version_id",
+                "worker_run_id": "worker_run_id",
             }
         )
 
     assert (
         sorted(
             [
                 {
                     "text": transcription.text,
                     "worker_version_id": transcription.worker_version.id
                     if transcription.worker_version
                     else None,
+                    "worker_run_id": transcription.worker_run.id
+                    if transcription.worker_run
+                    else None,
                 }
                 for transcription in transcriptions
             ],
             key=itemgetter("text"),
         )
         == expected_transcriptions
     )
 
 
-@pytest.mark.parametrize("worker_version", (False, "worker_version_id", None))
+@pytest.mark.parametrize("source", (False, "id", None))
 @pytest.mark.parametrize(
     "supported_types", (["surname"], ["surname", "firstname", "birthdate"])
 )
-def test_get_transcription_entities(worker_version, mock_database, supported_types):
-    transcription_id = "train-page_1-line_1" + (worker_version or "")
+def test_get_transcription_entities(source, mock_database, supported_types):
+    worker_version = f"worker_version_{source}" if isinstance(source, str) else source
+    worker_run = f"worker_run_{source}" if isinstance(source, str) else source
+
+    transcription_id = "train-page_1-line_1" + ("source" if source else "")
     entities = get_transcription_entities(
         transcription_id=transcription_id,
         entity_worker_versions=[worker_version],
+        entity_worker_runs=[worker_run],
         supported_types=supported_types,
     )
 
     expected_entities = [
         {
             "name": "Caillet",
             "type": "surname",
@@ -137,17 +156,18 @@
         },
     ]
 
     expected_entities = list(
         filter(lambda ent: ent["type"] in supported_types, expected_entities)
     )
     for entity in expected_entities:
-        if worker_version:
+        if source:
             entity["name"] = entity["name"].lower()
         entity["worker_version"] = worker_version or None
+        entity["worker_run"] = worker_run or None
 
     assert (
         sorted(
             entities,
             key=itemgetter("offset"),
         )
         == expected_entities
```

### Comparing `atr-dan-0.2.0rc5/tests/test_download.py` & `atr_dan-0.2.0rc6/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `atr-dan-0.2.0rc5/tests/test_evaluate.py` & `atr_dan-0.2.0rc6/tests/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `atr-dan-0.2.0rc5/tests/test_extract.py` & `atr_dan-0.2.0rc6/tests/test_extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -455,52 +455,53 @@
 
 
 @pytest.mark.parametrize(
     "nestation, xml_output, separators",
     (
         # Non-nested
         (
-            "non-nested-id",
+            "non-nested",
             "<root>The <adj>great</adj> king <name>Charles</name> III has eaten \nwith <person>us</person>.</root>",
             None,
         ),
         # Non-nested no text between entities
         (
-            "non-nested-id",
+            "non-nested",
             "<root><adj>great</adj> <name>Charles</name>\n<person>us</person></root>",
             ["\n", " "],
         ),
         # Nested
         (
-            "nested-id",
+            "nested",
             "<root>The great king <fullname><name>Charles</name> III</fullname> has eaten \nwith <person>us</person>.</root>",
             None,
         ),
         # Nested no text between entities
         (
-            "nested-id",
+            "nested",
             "<root><fullname><name>Charles</name> III</fullname>\n<person>us</person></root>",
             ["\n", " "],
         ),
         # Special characters in entities
         (
-            "special-chars-id",
+            "special-chars",
             "<root>The <Arkindex_s_entity>great</Arkindex_s_entity> king <_Name_1_>Charles</_Name_1_> III has eaten \nwith <Person_>us</Person_>.</root>",
             None,
         ),
     ),
 )
 def test_entities_to_xml(mock_database, nestation, xml_output, separators):
     transcription = Transcription.get_by_id("tr-with-entities")
     assert (
         entities_to_xml(
             text=transcription.text,
             predictions=get_transcription_entities(
                 transcription_id="tr-with-entities",
-                entity_worker_versions=[nestation],
+                entity_worker_versions=[f"worker-version-{nestation}-id"],
+                entity_worker_runs=[f"worker-run-{nestation}-id"],
                 supported_types=[
                     "name",
                     "fullname",
                     "person",
                     "adj",
                     "Arkindex's entity",
                     '"Name" (1)',
@@ -535,15 +536,16 @@
 ):
     transcription = Transcription.get_by_id("tr-with-entities")
     assert (
         entities_to_xml(
             text=transcription.text,
             predictions=get_transcription_entities(
                 transcription_id="tr-with-entities",
-                entity_worker_versions=["non-nested-id"],
+                entity_worker_versions=["worker-version-non-nested-id"],
+                entity_worker_runs=["worker-run-non-nested-id"],
                 supported_types=supported_entities,
             ),
             entity_separators=separators,
         )
         == xml_output
     )
```

### Comparing `atr-dan-0.2.0rc5/tests/test_prediction.py` & `atr_dan-0.2.0rc6/tests/test_prediction.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 # Copyright Teklia (contact@teklia.com) & Denis Coquenet
 # This code is licensed under CeCILL-C
 
 # -*- coding: utf-8 -*-
 
 import json
 import shutil
+from pathlib import Path
 
 import numpy as np
 import pytest
 import yaml
 
 from dan.ocr.predict.attention import Level
 from dan.ocr.predict.inference import DAN
 from dan.ocr.predict.inference import run as run_prediction
-from dan.utils import parse_tokens, read_yaml
+from dan.utils import (
+    parse_charset_pattern,
+    parse_tokens,
+    read_yaml,
+)
 from tests import FIXTURES
 
 PREDICTION_DATA_PATH = FIXTURES / "prediction"
 
 
 @pytest.mark.parametrize(
     "image_name, expected_prediction",
@@ -69,36 +74,42 @@
     image_path = PREDICTION_DATA_PATH / "images" / image_name
     _, image = dan_model.preprocess(str(image_path))
 
     input_tensor = image.unsqueeze(0)
     input_tensor = input_tensor.to(device)
     input_sizes = [image.shape[1:]]
 
-    prediction = dan_model.predict(input_tensor, input_sizes)
+    prediction = dan_model.predict(
+        input_tensor,
+        input_sizes,
+        char_separators=parse_charset_pattern(dan_model.charset),
+    )
 
     assert prediction == expected_prediction
 
 
 @pytest.mark.parametrize(
-    "image_name, confidence_score, temperature, expected_prediction",
+    "image_name, confidence_score, temperature, predict_objects, expected_prediction",
     (
         (
             "0a56e8b3-95cd-4fa5-a17b-5b0ff9e6ea84",
-            None,
-            1.0,
+            [],  # Confidence score
+            1.0,  # Temperature
+            False,  # Predict objects
             {
                 "text": "ⓈBellisson ⒻGeorges Ⓑ91 ⓁP ⒸM ⓀCh ⓄPlombier ⓅPatron?12241",
                 "language_model": {},
                 "confidences": {},
             },
         ),
         (
             "0a56e8b3-95cd-4fa5-a17b-5b0ff9e6ea84",
-            [Level.Word],
-            1.0,
+            [Level.Word],  # Confidence score
+            1.0,  # Temperature
+            True,  # Predict objects
             {
                 "text": "ⓈBellisson ⒻGeorges Ⓑ91 ⓁP ⒸM ⓀCh ⓄPlombier ⓅPatron?12241",
                 "language_model": {},
                 "confidences": {
                     "total": 1.0,
                     "word": [
                         {"text": "ⓈBellisson", "confidence": 1.0},
@@ -107,20 +118,72 @@
                         {"text": "ⓁP", "confidence": 1.0},
                         {"text": "ⒸM", "confidence": 1.0},
                         {"text": "ⓀCh", "confidence": 1.0},
                         {"text": "ⓄPlombier", "confidence": 1.0},
                         {"text": "ⓅPatron?12241", "confidence": 1.0},
                     ],
                 },
+                "objects": [
+                    {
+                        "confidence": 0.42,
+                        "polygon": [[0, 0], [144, 0], [144, 66], [0, 66]],
+                        "text": "ⓈBellisson",
+                        "text_confidence": 1.0,
+                    },
+                    {
+                        "confidence": 0.52,
+                        "polygon": [[184, 0], [269, 0], [269, 66], [184, 66]],
+                        "text": "ⒻGeorges",
+                        "text_confidence": 1.0,
+                    },
+                    {
+                        "confidence": 0.21,
+                        "polygon": [[294, 0], [371, 0], [371, 66], [294, 66]],
+                        "text": "Ⓑ91",
+                        "text_confidence": 1.0,
+                    },
+                    {
+                        "confidence": 0.23,
+                        "polygon": [[367, 0], [427, 0], [427, 66], [367, 66]],
+                        "text": "ⓁP",
+                        "text_confidence": 1.0,
+                    },
+                    {
+                        "confidence": 0.18,
+                        "polygon": [[535, 0], [619, 0], [619, 66], [535, 66]],
+                        "text": "ⒸM",
+                        "text_confidence": 1.0,
+                    },
+                    {
+                        "confidence": 0.23,
+                        "polygon": [[589, 0], [674, 0], [674, 66], [589, 66]],
+                        "text": "ⓀCh",
+                        "text_confidence": 1.0,
+                    },
+                    {
+                        "confidence": 0.31,
+                        "polygon": [[685, 0], [806, 0], [806, 66], [685, 66]],
+                        "text": "ⓄPlombier",
+                        "text_confidence": 1.0,
+                    },
+                    {
+                        "confidence": 0.91,
+                        "polygon": [[820, 0], [938, 0], [938, 66], [820, 66]],
+                        "text": "ⓅPatron?12241",
+                        "text_confidence": 1.0,
+                    },
+                ],
+                "attention_gif": "0a56e8b3-95cd-4fa5-a17b-5b0ff9e6ea84_word.gif",
             },
         ),
         (
             "0a56e8b3-95cd-4fa5-a17b-5b0ff9e6ea84",
-            [Level.NER, Level.Word],
-            3.5,
+            [Level.NER, Level.Word],  # Confidence score
+            3.5,  # Temperature
+            False,  # Predict objects
             {
                 "text": "ⓈBellisson ⒻGeorges Ⓑ91 ⓁP ⒸM ⓀCh ⓄPlombier ⓅPatron?12241",
                 "language_model": {},
                 "confidences": {
                     "total": 0.93,
                     "ner": [
                         {"text": "ⓈBellisson ", "confidence": 0.92},
@@ -143,16 +206,17 @@
                         {"text": "ⓅPatron?12241", "confidence": 0.93},
                     ],
                 },
             },
         ),
         (
             "0a56e8b3-95cd-4fa5-a17b-5b0ff9e6ea84",
-            [Level.Line],
-            1.0,
+            [Level.Line],  # Confidence score
+            1.0,  # Temperature
+            False,  # Predict objects
             {
                 "text": "ⓈBellisson ⒻGeorges Ⓑ91 ⓁP ⒸM ⓀCh ⓄPlombier ⓅPatron?12241",
                 "language_model": {},
                 "confidences": {
                     "total": 1.0,
                     "line": [
                         {
@@ -161,16 +225,17 @@
                         }
                     ],
                 },
             },
         ),
         (
             "0a56e8b3-95cd-4fa5-a17b-5b0ff9e6ea84",
-            [Level.NER, Level.Line],
-            3.5,
+            [Level.NER, Level.Line],  # Confidence score
+            3.5,  # Temperature
+            False,  # Predict objects
             {
                 "text": "ⓈBellisson ⒻGeorges Ⓑ91 ⓁP ⒸM ⓀCh ⓄPlombier ⓅPatron?12241",
                 "language_model": {},
                 "confidences": {
                     "total": 0.93,
                     "ner": [
                         {"text": "ⓈBellisson ", "confidence": 0.92},
@@ -189,26 +254,28 @@
                         }
                     ],
                 },
             },
         ),
         (
             "0dfe8bcd-ed0b-453e-bf19-cc697012296e",
-            None,
-            1.0,
+            [],  # Confidence score
+            1.0,  # Temperature
+            False,  # Predict objects
             {
                 "text": "ⓈTemplié ⒻMarcelle Ⓑ93 ⓁS Ⓚch ⓄE dactylo Ⓟ18376",
                 "language_model": {},
                 "confidences": {},
             },
         ),
         (
             "0dfe8bcd-ed0b-453e-bf19-cc697012296e",
-            [Level.NER, Level.Char, Level.Word, Level.Line],
-            1.0,
+            [Level.NER, Level.Char, Level.Word, Level.Line],  # Confidence score
+            1.0,  # Temperature
+            False,  # Predict objects
             {
                 "text": "ⓈTemplié ⒻMarcelle Ⓑ93 ⓁS Ⓚch ⓄE dactylo Ⓟ18376",
                 "language_model": {},
                 "confidences": {
                     "total": 1.0,
                     "ner": [
                         {"text": "ⓈTemplié ", "confidence": 0.98},
@@ -285,77 +352,95 @@
                         }
                     ],
                 },
             },
         ),
         (
             "2c242f5c-e979-43c4-b6f2-a6d4815b651d",
-            False,
-            1.0,
+            [],  # Confidence score
+            1.0,  # Temperature
+            False,  # Predict objects
             {
                 "text": "Ⓢd ⒻCharles Ⓑ11 ⓁP ⒸC ⓀF Ⓞd Ⓟ14 31",
                 "language_model": {},
                 "confidences": {},
             },
         ),
         (
             "ffdec445-7f14-4f5f-be44-68d0844d0df1",
-            False,
-            1.0,
+            [],  # Confidence score
+            1.0,  # Temperature
+            True,  # Predict objects
             {
                 "text": "ⓈNaudin ⒻMarie Ⓑ53 ⓁS Ⓒv ⓀBelle mère",
                 "language_model": {},
                 "confidences": {},
+                "objects": [
+                    {
+                        "confidence": 0.96,
+                        "polygon": [[546, 0], [715, 0], [715, 67], [546, 67]],
+                        "text": "ⓈNaudin ⒻMarie Ⓑ53 ⓁS Ⓒv ⓀBelle mère",
+                        "text_confidence": 1.0,
+                    }
+                ],
             },
         ),
     ),
 )
 def test_run_prediction(
     image_name,
     confidence_score,
     temperature,
+    predict_objects,
     expected_prediction,
     tmp_path,
 ):
+    if "attention_gif" in expected_prediction:
+        expected_prediction["attention_gif"] = str(
+            tmp_path / expected_prediction["attention_gif"]
+        )
+
     # Make tmpdir and copy needed image inside
     image_dir = tmp_path / "images"
     image_dir.mkdir()
     shutil.copyfile(
         (PREDICTION_DATA_PATH / "images" / image_name).with_suffix(".png"),
         (image_dir / image_name).with_suffix(".png"),
     )
 
     run_prediction(
         image_dir=image_dir,
         model=PREDICTION_DATA_PATH,
         output=tmp_path,
-        confidence_score=True if confidence_score else False,
-        confidence_score_levels=confidence_score if confidence_score else [],
-        attention_map=False,
-        attention_map_level=None,
+        confidence_score=bool(confidence_score),
+        confidence_score_levels=confidence_score,
+        attention_map=predict_objects and confidence_score,
+        attention_map_level=[Level.Line, *confidence_score].pop(),
         attention_map_scale=0.5,
         alpha_factor=0.9,
         color_map="nipy_spectral",
         word_separators=[" ", "\n"],
         line_separators=["\n"],
         temperature=temperature,
-        predict_objects=False,
+        predict_objects=predict_objects,
         max_object_height=None,
         image_extension=".png",
         gpu_device=None,
         batch_size=1,
         tokens=parse_tokens(PREDICTION_DATA_PATH / "tokens.yml"),
         start_token=None,
         use_language_model=False,
         compile_model=False,
         dynamic_mode=False,
     )
 
     prediction = json.loads((tmp_path / image_name).with_suffix(".json").read_text())
     assert prediction == expected_prediction
+    if "attention_gif" in expected_prediction:
+        assert Path(expected_prediction["attention_gif"]).exists()
 
 
 @pytest.mark.parametrize(
     "image_names, confidence_score, temperature, expected_predictions",
     (
         (
             ["0a56e8b3-95cd-4fa5-a17b-5b0ff9e6ea84"],
```

### Comparing `atr-dan-0.2.0rc5/tests/test_tokens.py` & `atr_dan-0.2.0rc6/tests/test_tokens.py`

 * *Files identical despite different names*

### Comparing `atr-dan-0.2.0rc5/tests/test_training.py` & `atr_dan-0.2.0rc6/tests/test_training.py`

 * *Files identical despite different names*

### Comparing `atr-dan-0.2.0rc5/tests/test_utils.py` & `atr_dan-0.2.0rc6/tests/test_utils.py`

 * *Files identical despite different names*

