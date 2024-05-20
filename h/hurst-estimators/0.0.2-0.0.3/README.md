# Comparing `tmp/hurst_estimators-0.0.2.tar.gz` & `tmp/hurst_estimators-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hurst_estimators-0.0.2.tar", max compression
+gzip compressed data, was "hurst_estimators-0.0.3.tar", max compression
```

## Comparing `hurst_estimators-0.0.2.tar` & `hurst_estimators-0.0.3.tar`

### file list

```diff
@@ -1,5 +1,18 @@
--rw-r--r--   0        0        0        0 2024-05-15 13:03:21.357769 hurst_estimators-0.0.2/hurst_estimators/__init__.py
--rw-r--r--   0        0        0        0 2024-05-15 13:13:27.716123 hurst_estimators-0.0.2/hurst_estimators/wavelet_estimator.py
--rw-r--r--   0        0        0      387 2024-05-15 13:34:59.320493 hurst_estimators-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-15 13:14:05.657123 hurst_estimators-0.0.2/README.md
--rw-r--r--   0        0        0      614 1970-01-01 00:00:00.000000 hurst_estimators-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      441 2024-05-20 14:46:53.353076 hurst_estimators-0.0.3/hurst_estimators/__init__.py
+-rw-r--r--   0        0        0      523 2024-05-20 14:36:07.131260 hurst_estimators-0.0.3/hurst_estimators/estimators/__init__.py
+-rw-r--r--   0        0        0     2614 2024-05-15 20:26:54.174240 hurst_estimators-0.0.3/hurst_estimators/estimators/central_estimator.py
+-rw-r--r--   0        0        0     2029 2024-05-20 14:16:02.389121 hurst_estimators-0.0.3/hurst_estimators/estimators/dfa_estimator.py
+-rw-r--r--   0        0        0     1138 2024-05-20 12:58:38.289273 hurst_estimators-0.0.3/hurst_estimators/estimators/ghe_estimator.py
+-rw-r--r--   0        0        0     2946 2024-05-15 20:26:54.175240 hurst_estimators-0.0.3/hurst_estimators/estimators/higuchi_estimator.py
+-rw-r--r--   0        0        0     1513 2024-05-20 12:54:32.368846 hurst_estimators-0.0.3/hurst_estimators/estimators/periodogram_estimator.py
+-rw-r--r--   0        0        0     1784 2024-05-20 14:41:22.980973 hurst_estimators-0.0.3/hurst_estimators/estimators/rs_estimator.py
+-rw-r--r--   0        0        0     1904 2024-05-20 11:25:43.287066 hurst_estimators-0.0.3/hurst_estimators/estimators/wavelet_estimator.py
+-rw-r--r--   0        0        0       70 2024-05-20 11:40:10.069703 hurst_estimators-0.0.3/hurst_estimators/simulators/__init__.py
+-rw-r--r--   0        0        0     1668 2024-05-20 11:40:10.069703 hurst_estimators-0.0.3/hurst_estimators/simulators/generate_fgn.py
+-rw-r--r--   0        0        0      149 2024-05-20 12:46:55.610520 hurst_estimators-0.0.3/hurst_estimators/utils/__init__.py
+-rw-r--r--   0        0        0      415 2024-05-20 12:45:24.843110 hurst_estimators-0.0.3/hurst_estimators/utils/_gen_sbpf.py
+-rw-r--r--   0        0        0      677 2024-05-20 12:46:32.502711 hurst_estimators-0.0.3/hurst_estimators/utils/search_opt_seq_len.py
+-rw-r--r--   0        0        0     1088 2024-05-15 20:26:54.173235 hurst_estimators-0.0.3/LICENSE
+-rw-r--r--   0        0        0      698 2024-05-20 19:42:45.469790 hurst_estimators-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1396 2024-05-20 19:40:15.154660 hurst_estimators-0.0.3/README.md
+-rw-r--r--   0        0        0     1950 1970-01-01 00:00:00.000000 hurst_estimators-0.0.3/PKG-INFO
```

