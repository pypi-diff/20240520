# Comparing `tmp/pyflyde-0.0.6.tar.gz` & `tmp/pyflyde-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyflyde-0.0.6.tar", last modified: Thu May  9 19:42:20 2024, max compression
+gzip compressed data, was "pyflyde-0.0.7.tar", last modified: Mon May 20 18:18:08 2024, max compression
```

## Comparing `pyflyde-0.0.6.tar` & `pyflyde-0.0.7.tar`

### file list

```diff
@@ -1,60 +1,72 @@
-drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 19:42:20.630336 pyflyde-0.0.6/
--rw-r--r--   0 trustmaster   (501) staff       (20)       31 2024-05-09 18:42:24.000000 pyflyde-0.0.6/.flake8
-drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 19:42:20.487418 pyflyde-0.0.6/.github/
-drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 19:42:20.513145 pyflyde-0.0.6/.github/workflows/
--rw-r--r--   0 trustmaster   (501) staff       (20)      984 2024-05-09 11:09:26.000000 pyflyde-0.0.6/.github/workflows/python-package.yml
--rw-r--r--   0 trustmaster   (501) staff       (20)     3197 2024-05-09 10:46:21.000000 pyflyde-0.0.6/.gitignore
--rw-r--r--   0 trustmaster   (501) staff       (20)    11345 2024-04-09 17:14:23.000000 pyflyde-0.0.6/LICENSE
--rw-r--r--   0 trustmaster   (501) staff       (20)     1047 2024-05-09 19:01:54.000000 pyflyde-0.0.6/Makefile
--rw-r--r--   0 trustmaster   (501) staff       (20)    16114 2024-05-09 19:42:20.628943 pyflyde-0.0.6/PKG-INFO
--rw-r--r--   0 trustmaster   (501) staff       (20)     1887 2024-05-09 16:21:19.000000 pyflyde-0.0.6/README.md
--rw-r--r--   0 trustmaster   (501) staff       (20)   265919 2024-05-09 10:46:21.000000 pyflyde-0.0.6/clustering_example.png
-drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 19:42:20.526363 pyflyde-0.0.6/examples/
--rw-r--r--   0 trustmaster   (501) staff       (20)     4489 2024-05-09 10:46:21.000000 pyflyde-0.0.6/examples/Clustering.flyde
--rw-r--r--   0 trustmaster   (501) staff       (20)      991 2024-04-09 17:14:23.000000 pyflyde-0.0.6/examples/HelloPy.flyde
-drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 19:42:20.527595 pyflyde-0.0.6/examples/datasets/
--rw-r--r--   0 trustmaster   (501) staff       (20)    11089 2024-04-09 17:14:23.000000 pyflyde-0.0.6/examples/datasets/wine-clustering.csv
-drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 19:42:20.546914 pyflyde-0.0.6/examples/mylib/
--rw-r--r--   0 trustmaster   (501) staff       (20)        0 2024-04-09 17:14:23.000000 pyflyde-0.0.6/examples/mylib/__init__.py
--rw-r--r--   0 trustmaster   (501) staff       (20)      560 2024-04-21 06:51:36.000000 pyflyde-0.0.6/examples/mylib/components.flyde.ts
--rw-r--r--   0 trustmaster   (501) staff       (20)      725 2024-04-13 14:14:04.000000 pyflyde-0.0.6/examples/mylib/components.py
--rw-r--r--   0 trustmaster   (501) staff       (20)      684 2024-05-09 10:46:21.000000 pyflyde-0.0.6/examples/mylib/dataframe.flyde.ts
--rw-r--r--   0 trustmaster   (501) staff       (20)     1353 2024-05-09 10:46:21.000000 pyflyde-0.0.6/examples/mylib/dataframe.py
--rw-r--r--   0 trustmaster   (501) staff       (20)     1619 2024-04-09 17:14:23.000000 pyflyde-0.0.6/examples/mylib/kmeans.flyde.ts
--rw-r--r--   0 trustmaster   (501) staff       (20)     6171 2024-05-06 19:18:33.000000 pyflyde-0.0.6/examples/mylib/kmeans.py
--rw-r--r--   0 trustmaster   (501) staff       (20)      216 2024-04-09 17:14:23.000000 pyflyde-0.0.6/examples/pyproject.toml
-drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 19:42:20.574730 pyflyde-0.0.6/flyde/
--rw-r--r--   0 trustmaster   (501) staff       (20)        0 2024-04-09 17:14:23.000000 pyflyde-0.0.6/flyde/__init__.py
--rw-r--r--   0 trustmaster   (501) staff       (20)        0 2024-05-09 19:01:16.000000 pyflyde-0.0.6/flyde/__init__.pyi
--rw-r--r--   0 trustmaster   (501) staff       (20)     2202 2024-05-09 19:40:24.000000 pyflyde-0.0.6/flyde/cli.py
--rw-r--r--   0 trustmaster   (501) staff       (20)      221 2024-05-09 19:42:12.000000 pyflyde-0.0.6/flyde/cli.pyi
--rw-r--r--   0 trustmaster   (501) staff       (20)     4559 2024-05-09 10:46:21.000000 pyflyde-0.0.6/flyde/flow.py
--rw-r--r--   0 trustmaster   (501) staff       (20)      679 2024-05-09 19:42:12.000000 pyflyde-0.0.6/flyde/flow.pyi
--rw-r--r--   0 trustmaster   (501) staff       (20)     9925 2024-05-09 10:46:21.000000 pyflyde-0.0.6/flyde/io.py
--rw-r--r--   0 trustmaster   (501) staff       (20)     2182 2024-05-09 19:42:12.000000 pyflyde-0.0.6/flyde/io.pyi
--rw-r--r--   0 trustmaster   (501) staff       (20)    17280 2024-05-09 10:46:21.000000 pyflyde-0.0.6/flyde/node.py
--rw-r--r--   0 trustmaster   (501) staff       (20)     2115 2024-05-09 19:42:12.000000 pyflyde-0.0.6/flyde/node.pyi
--rw-r--r--   0 trustmaster   (501) staff       (20)     1670 2024-05-09 10:46:21.000000 pyflyde-0.0.6/flyde/stdlib.py
--rw-r--r--   0 trustmaster   (501) staff       (20)      500 2024-05-09 19:42:12.000000 pyflyde-0.0.6/flyde/stdlib.pyi
--rwxr-xr-x   0 trustmaster   (501) staff       (20)       89 2024-05-09 19:40:47.000000 pyflyde-0.0.6/flyde.py
-drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 19:42:20.624007 pyflyde-0.0.6/pyflyde.egg-info/
--rw-r--r--   0 trustmaster   (501) staff       (20)    16114 2024-05-09 19:42:20.000000 pyflyde-0.0.6/pyflyde.egg-info/PKG-INFO
--rw-r--r--   0 trustmaster   (501) staff       (20)     1064 2024-05-09 19:42:20.000000 pyflyde-0.0.6/pyflyde.egg-info/SOURCES.txt
--rw-r--r--   0 trustmaster   (501) staff       (20)        1 2024-05-09 19:42:20.000000 pyflyde-0.0.6/pyflyde.egg-info/dependency_links.txt
--rw-r--r--   0 trustmaster   (501) staff       (20)       44 2024-05-09 19:42:20.000000 pyflyde-0.0.6/pyflyde.egg-info/entry_points.txt
--rw-r--r--   0 trustmaster   (501) staff       (20)       64 2024-05-09 19:42:20.000000 pyflyde-0.0.6/pyflyde.egg-info/requires.txt
--rw-r--r--   0 trustmaster   (501) staff       (20)        6 2024-05-09 19:42:20.000000 pyflyde-0.0.6/pyflyde.egg-info/top_level.txt
--rw-r--r--   0 trustmaster   (501) staff       (20)     1322 2024-05-09 19:41:45.000000 pyflyde-0.0.6/pyproject.toml
--rw-r--r--   0 trustmaster   (501) staff       (20)       38 2024-05-09 19:42:20.630585 pyflyde-0.0.6/setup.cfg
-drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 19:42:20.622556 pyflyde-0.0.6/tests/
--rw-r--r--   0 trustmaster   (501) staff       (20)     1744 2024-05-09 10:46:21.000000 pyflyde-0.0.6/tests/Repeat3Times.flyde
--rw-r--r--   0 trustmaster   (501) staff       (20)      782 2024-04-25 19:45:07.000000 pyflyde-0.0.6/tests/TestInOutFlow.flyde
--rw-r--r--   0 trustmaster   (501) staff       (20)      820 2024-04-24 22:56:30.000000 pyflyde-0.0.6/tests/TestIsolatedFlow.flyde
--rw-r--r--   0 trustmaster   (501) staff       (20)     1798 2024-05-09 10:46:21.000000 pyflyde-0.0.6/tests/TestNestedFlow.flyde
--rw-r--r--   0 trustmaster   (501) staff       (20)        0 2024-04-09 17:26:09.000000 pyflyde-0.0.6/tests/__init.py__
--rw-r--r--   0 trustmaster   (501) staff       (20)      914 2024-05-09 10:46:21.000000 pyflyde-0.0.6/tests/components.flyde.ts
--rw-r--r--   0 trustmaster   (501) staff       (20)     1185 2024-05-09 10:46:21.000000 pyflyde-0.0.6/tests/components.py
--rw-r--r--   0 trustmaster   (501) staff       (20)     1933 2024-05-09 10:46:21.000000 pyflyde-0.0.6/tests/test_flow.py
--rw-r--r--   0 trustmaster   (501) staff       (20)    10544 2024-05-09 10:46:21.000000 pyflyde-0.0.6/tests/test_io.py
--rw-r--r--   0 trustmaster   (501) staff       (20)    11312 2024-05-09 10:46:21.000000 pyflyde-0.0.6/tests/test_node.py
--rw-r--r--   0 trustmaster   (501) staff       (20)     3754 2024-05-09 10:46:21.000000 pyflyde-0.0.6/tests/test_stdlib.py
+drwxr-xr-x   0 trustmaster  (1000) trustmaster  (1000)        0 2024-05-20 18:18:08.929855 pyflyde-0.0.7/
+-rw-rw-r--   0 trustmaster  (1000) trustmaster  (1000)       31 2024-05-13 16:07:18.000000 pyflyde-0.0.7/.flake8
+drwxr-xr-x   0 trustmaster  (1000) trustmaster  (1000)        0 2024-05-20 18:18:08.769841 pyflyde-0.0.7/.github/
+drwxr-xr-x   0 trustmaster  (1000) trustmaster  (1000)        0 2024-05-20 18:18:08.825846 pyflyde-0.0.7/.github/workflows/
+-rw-rw-r--   0 trustmaster  (1000) trustmaster  (1000)      984 2024-05-13 16:07:18.000000 pyflyde-0.0.7/.github/workflows/python-package.yml
+-rw-rw-r--   0 trustmaster  (1000) trustmaster  (1000)     3197 2024-05-13 16:07:18.000000 pyflyde-0.0.7/.gitignore
+-rw-r--r--   0 trustmaster  (1000) trustmaster  (1000)      816 2024-05-19 14:55:39.000000 pyflyde-0.0.7/.readthedocs.yaml
+-rw-r--r--   0 trustmaster  (1000) trustmaster  (1000)    11345 2024-04-01 20:24:29.000000 pyflyde-0.0.7/LICENSE
+-rw-r--r--   0 trustmaster  (1000) trustmaster  (1000)     1229 2024-05-20 18:17:53.000000 pyflyde-0.0.7/Makefile
+-rw-r--r--   0 trustmaster  (1000) trustmaster  (1000)    16766 2024-05-20 18:18:08.928855 pyflyde-0.0.7/PKG-INFO
+-rw-rw-r--   0 trustmaster  (1000) trustmaster  (1000)     2501 2024-05-18 16:33:30.000000 pyflyde-0.0.7/README.md
+-rw-rw-r--   0 trustmaster  (1000) trustmaster  (1000)   265919 2024-05-13 16:07:18.000000 pyflyde-0.0.7/clustering_example.png
+drwxr-xr-x   0 trustmaster  (1000) trustmaster  (1000)        0 2024-05-20 18:18:08.850848 pyflyde-0.0.7/docs/
+-rw-r--r--   0 trustmaster  (1000) trustmaster  (1000)      311 2024-05-19 14:55:39.000000 pyflyde-0.0.7/docs/index.md
+drwxr-xr-x   0 trustmaster  (1000) trustmaster  (1000)        0 2024-05-20 18:18:08.853848 pyflyde-0.0.7/docs/package/
+-rw-r--r--   0 trustmaster  (1000) trustmaster  (1000)       29 2024-05-19 14:55:39.000000 pyflyde-0.0.7/docs/package/flyde.flow.md
+-rw-r--r--   0 trustmaster  (1000) trustmaster  (1000)       25 2024-05-19 14:55:39.000000 pyflyde-0.0.7/docs/package/flyde.io.md
+-rw-r--r--   0 trustmaster  (1000) trustmaster  (1000)       29 2024-05-19 14:55:39.000000 pyflyde-0.0.7/docs/package/flyde.node.md
+-rw-r--r--   0 trustmaster  (1000) trustmaster  (1000)      239 2024-05-19 14:55:39.000000 pyflyde-0.0.7/docs/reference.md
+-rw-r--r--   0 trustmaster  (1000) trustmaster  (1000)       45 2024-05-19 14:55:39.000000 pyflyde-0.0.7/docs/requirements.in
+-rw-r--r--   0 trustmaster  (1000) trustmaster  (1000)     1528 2024-05-19 14:55:39.000000 pyflyde-0.0.7/docs/requirements.txt
+-rw-r--r--   0 trustmaster  (1000) trustmaster  (1000)      927 2024-05-19 14:55:39.000000 pyflyde-0.0.7/docs/usage.md
+drwxr-xr-x   0 trustmaster  (1000) trustmaster  (1000)        0 2024-05-20 18:18:08.855849 pyflyde-0.0.7/examples/
+-rw-rw-r--   0 trustmaster  (1000) trustmaster  (1000)     4489 2024-05-13 16:07:18.000000 pyflyde-0.0.7/examples/Clustering.flyde
+-rw-r--r--   0 trustmaster  (1000) trustmaster  (1000)      991 2024-05-19 13:50:08.000000 pyflyde-0.0.7/examples/HelloPy.flyde
+drwxr-xr-x   0 trustmaster  (1000) trustmaster  (1000)        0 2024-05-20 18:18:08.855849 pyflyde-0.0.7/examples/datasets/
+-rw-r--r--   0 trustmaster  (1000) trustmaster  (1000)    11089 2024-04-06 12:45:53.000000 pyflyde-0.0.7/examples/datasets/wine-clustering.csv
+drwxr-xr-x   0 trustmaster  (1000) trustmaster  (1000)        0 2024-05-20 18:18:08.915854 pyflyde-0.0.7/examples/mylib/
+-rw-r--r--   0 trustmaster  (1000) trustmaster  (1000)        0 2024-04-05 15:20:17.000000 pyflyde-0.0.7/examples/mylib/__init__.py
+-rw-r--r--   0 trustmaster  (1000) trustmaster  (1000)      560 2024-04-05 15:32:45.000000 pyflyde-0.0.7/examples/mylib/components.flyde.ts
+-rw-rw-r--   0 trustmaster  (1000) trustmaster  (1000)      725 2024-05-13 16:07:18.000000 pyflyde-0.0.7/examples/mylib/components.py
+-rw-rw-r--   0 trustmaster  (1000) trustmaster  (1000)      684 2024-05-13 16:07:18.000000 pyflyde-0.0.7/examples/mylib/dataframe.flyde.ts
+-rw-rw-r--   0 trustmaster  (1000) trustmaster  (1000)     1353 2024-05-13 16:07:18.000000 pyflyde-0.0.7/examples/mylib/dataframe.py
+-rw-r--r--   0 trustmaster  (1000) trustmaster  (1000)     1619 2024-04-06 14:46:34.000000 pyflyde-0.0.7/examples/mylib/kmeans.flyde.ts
+-rw-rw-r--   0 trustmaster  (1000) trustmaster  (1000)     6171 2024-05-13 16:07:18.000000 pyflyde-0.0.7/examples/mylib/kmeans.py
+-rw-r--r--   0 trustmaster  (1000) trustmaster  (1000)      216 2024-04-06 13:35:54.000000 pyflyde-0.0.7/examples/pyproject.toml
+drwxr-xr-x   0 trustmaster  (1000) trustmaster  (1000)        0 2024-05-20 18:18:08.919854 pyflyde-0.0.7/flyde/
+-rw-r--r--   0 trustmaster  (1000) trustmaster  (1000)        0 2024-03-25 20:32:10.000000 pyflyde-0.0.7/flyde/__init__.py
+-rw-r--r--   0 trustmaster  (1000) trustmaster  (1000)        0 2024-05-20 18:18:02.000000 pyflyde-0.0.7/flyde/__init__.pyi
+-rw-rw-r--   0 trustmaster  (1000) trustmaster  (1000)     2202 2024-05-13 16:07:18.000000 pyflyde-0.0.7/flyde/cli.py
+-rw-r--r--   0 trustmaster  (1000) trustmaster  (1000)      267 2024-05-20 18:18:02.000000 pyflyde-0.0.7/flyde/cli.pyi
+-rw-rw-r--   0 trustmaster  (1000) trustmaster  (1000)     4559 2024-05-13 16:07:18.000000 pyflyde-0.0.7/flyde/flow.py
+-rw-r--r--   0 trustmaster  (1000) trustmaster  (1000)     1531 2024-05-20 18:18:02.000000 pyflyde-0.0.7/flyde/flow.pyi
+-rw-rw-r--   0 trustmaster  (1000) trustmaster  (1000)     9925 2024-05-13 16:07:18.000000 pyflyde-0.0.7/flyde/io.py
+-rw-r--r--   0 trustmaster  (1000) trustmaster  (1000)     5616 2024-05-20 18:18:02.000000 pyflyde-0.0.7/flyde/io.pyi
+-rw-r--r--   0 trustmaster  (1000) trustmaster  (1000)    17183 2024-05-20 18:13:37.000000 pyflyde-0.0.7/flyde/node.py
+-rw-r--r--   0 trustmaster  (1000) trustmaster  (1000)     4226 2024-05-20 18:18:02.000000 pyflyde-0.0.7/flyde/node.pyi
+-rw-r--r--   0 trustmaster  (1000) trustmaster  (1000)     9243 2024-05-20 18:13:37.000000 pyflyde-0.0.7/flyde/stdlib.py
+-rw-r--r--   0 trustmaster  (1000) trustmaster  (1000)     2212 2024-05-20 18:18:02.000000 pyflyde-0.0.7/flyde/stdlib.pyi
+-rw-r--r--   0 trustmaster  (1000) trustmaster  (1000)      384 2024-05-19 14:55:39.000000 pyflyde-0.0.7/mkdocs.yml
+-rwxrwxr-x   0 trustmaster  (1000) trustmaster  (1000)       89 2024-05-13 16:07:18.000000 pyflyde-0.0.7/pyflyde
+drwxr-xr-x   0 trustmaster  (1000) trustmaster  (1000)        0 2024-05-20 18:18:08.925855 pyflyde-0.0.7/pyflyde.egg-info/
+-rw-r--r--   0 trustmaster  (1000) trustmaster  (1000)    16766 2024-05-20 18:18:08.000000 pyflyde-0.0.7/pyflyde.egg-info/PKG-INFO
+-rw-r--r--   0 trustmaster  (1000) trustmaster  (1000)     1260 2024-05-20 18:18:08.000000 pyflyde-0.0.7/pyflyde.egg-info/SOURCES.txt
+-rw-r--r--   0 trustmaster  (1000) trustmaster  (1000)        1 2024-05-20 18:18:08.000000 pyflyde-0.0.7/pyflyde.egg-info/dependency_links.txt
+-rw-r--r--   0 trustmaster  (1000) trustmaster  (1000)       43 2024-05-20 18:18:08.000000 pyflyde-0.0.7/pyflyde.egg-info/entry_points.txt
+-rw-r--r--   0 trustmaster  (1000) trustmaster  (1000)       71 2024-05-20 18:18:08.000000 pyflyde-0.0.7/pyflyde.egg-info/requires.txt
+-rw-r--r--   0 trustmaster  (1000) trustmaster  (1000)        6 2024-05-20 18:18:08.000000 pyflyde-0.0.7/pyflyde.egg-info/top_level.txt
+-rw-r--r--   0 trustmaster  (1000) trustmaster  (1000)     1331 2024-05-20 18:13:37.000000 pyflyde-0.0.7/pyproject.toml
+-rw-r--r--   0 trustmaster  (1000) trustmaster  (1000)       38 2024-05-20 18:18:08.929855 pyflyde-0.0.7/setup.cfg
+drwxr-xr-x   0 trustmaster  (1000) trustmaster  (1000)        0 2024-05-20 18:18:08.924855 pyflyde-0.0.7/tests/
+-rw-rw-r--   0 trustmaster  (1000) trustmaster  (1000)     1744 2024-05-13 16:07:18.000000 pyflyde-0.0.7/tests/Repeat3Times.flyde
+-rw-r--r--   0 trustmaster  (1000) trustmaster  (1000)     2280 2024-05-20 18:13:37.000000 pyflyde-0.0.7/tests/TestInOutFlow.flyde
+-rw-rw-r--   0 trustmaster  (1000) trustmaster  (1000)      820 2024-05-13 16:07:18.000000 pyflyde-0.0.7/tests/TestIsolatedFlow.flyde
+-rw-rw-r--   0 trustmaster  (1000) trustmaster  (1000)     1798 2024-05-20 18:03:49.000000 pyflyde-0.0.7/tests/TestNestedFlow.flyde
+-rw-r--r--   0 trustmaster  (1000) trustmaster  (1000)        0 2024-04-12 19:21:25.000000 pyflyde-0.0.7/tests/__init.py__
+-rw-r--r--   0 trustmaster  (1000) trustmaster  (1000)     1256 2024-05-20 18:13:37.000000 pyflyde-0.0.7/tests/components.flyde.ts
+-rw-r--r--   0 trustmaster  (1000) trustmaster  (1000)     1673 2024-05-20 18:13:37.000000 pyflyde-0.0.7/tests/components.py
+-rw-r--r--   0 trustmaster  (1000) trustmaster  (1000)     1958 2024-05-20 18:13:37.000000 pyflyde-0.0.7/tests/test_flow.py
+-rw-rw-r--   0 trustmaster  (1000) trustmaster  (1000)    10544 2024-05-13 16:07:18.000000 pyflyde-0.0.7/tests/test_io.py
+-rw-r--r--   0 trustmaster  (1000) trustmaster  (1000)    11312 2024-05-20 18:13:37.000000 pyflyde-0.0.7/tests/test_node.py
+-rw-r--r--   0 trustmaster  (1000) trustmaster  (1000)    36595 2024-05-20 18:13:37.000000 pyflyde-0.0.7/tests/test_stdlib.py
```

### Comparing `pyflyde-0.0.6/.github/workflows/python-package.yml` & `pyflyde-0.0.7/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.6/.gitignore` & `pyflyde-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.6/LICENSE` & `pyflyde-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.6/Makefile` & `pyflyde-0.0.7/Makefile`

 * *Files 9% similar despite different names*

```diff
@@ -17,14 +17,19 @@
 	done
 
 lint:
 	@echo "Running linters..."
 	@black $(LIB_DIR) $(TEST_DIR);
 	@flake8 $(LIB_DIR) $(TEST_DIR);
 
+stubgen:
+	@echo "Generating type stubs..."
+	@rm -f $(SRC_DIR)/*.pyi;
+	@stubgen $(SRC_DIR) --include-docstrings --include-private -o .;
+
 test:
 	@echo "Running tests..."
 	@$(PYTHON) -m unittest discover -s $(TEST_DIR) -p "test_$(if $(mod),$(mod),*).py";
 
 cover:
 	@echo "Running tests with coverage..."
 	@coverage run -m unittest discover -s $(TEST_DIR) -p "test_*.py" ;
@@ -34,13 +39,15 @@
 
 venv-activate:
 	@echo "Activating virtual environment..."
 	@source .venv/bin/activate;
 
 builddist:
 	@echo "Building the project for distribution..."
-	@stubgen $(SRC_DIR) -o .;
 	@$(PYTHON) -m build;
 
+release: lint test stubgen builddist
+	@echo "Releasing the project...";
+
 upload:
 	@echo "Uploading the project to PyPI..."
 	@twine upload dist/*;
```

### Comparing `pyflyde-0.0.6/PKG-INFO` & `pyflyde-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyflyde
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python SDK and runtime for Flyde - a visual flow-based programming language and IDE.
 Author: Vladimir Sibirov
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -226,53 +226,58 @@
 Requires-Dist: setuptools; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: twine; extra == "dev"
+Requires-Dist: mkdocs; extra == "dev"
 
 # PyFlyde
 
 ![Build](https://github.com/trustmaster/pyflyde/actions/workflows/python-package.yml/badge.svg)
+[<img src="https://readthedocs.org/projects/pyflyde/badge/">](https://pyflyde.readthedocs.io/en/latest/)
 
 Python runtime for [Flyde](https://github.com/flydelabs/flyde) with Data Engineering emphasis.
 
 ![Example graph running K-means clustering with Pandas and Scikit-learn](https://github.com/trustmaster/pyflyde/blob/main/clustering_example.png?raw=true)
 
-## PoC warning
-
-This is a proof-of-concept and not a final implementation. Structure and API may change drastically before public release.
-
 ## Getting started
 
 You need Python 3.9+ installed on your machine to run PyFlyde.
 
-First, you need to install its dependencies:
+Then you can install PyFlyde using pip:
 
 ```bash
-pip install .
+pip install pyflyde
 ```
 
-Then you can run the Hello World example:
+### Running the examples
+
+You can copy `examples` folder from this repository to your local project to give it a try. Then you can run the example flow with:
 
 ```bash
-./flyde.py examples/HelloPy.flyde
+pyflyde examples/HelloWorld.flyde
 ```
 
+
 ### Using the visual editor
 
-Install Flyde VSCode extension from the [marketplace](https://marketplace.visualstudio.com/items?itemName=flyde.flyde-vscode).
+Install Flyde VSCode extension from the [marketplace](https://marketplace.visualstudio.com/items?itemName=flyde.flyde-vscode). It will open existing `.flyde` files in the visual editor. You can call `Flyde: New Visual Flow` command in VSCode to create a new flow file.
+
+You can browse the component library in the panel on the right. To see your local components click the "View all" button. They will appear under the "Current project". Note that PyFlyde doesn't implement all of the Flyde's stdlib components, only a few essential ones.
 
-Whenever you change your component library classes or their interfaces, use flyde.py gen command to generate .flyde.ts definitions, e.g.:
+Whenever you change your component library classes or their interfaces, use `pyflyde gen` command to generate `.flyde.ts` definitions, e.g.:
 
 ```bash
-./flyde.py gen examples/mylib/components.py
+pyflyde gen examples/mylib/components.py
 ```
 
+Flyde editor needs `.flyde.ts` files in order to "see" your components.
+
 ## Running a Machine Learning example
 
 `Clustering.flyde` is a more complex example which uses Pandas and Scikit-Learn to run K-means clustering on a [wine clustering dataset from Kaggle](https://www.kaggle.com/harrywang/wine-dataset-for-clustering). It's a PyFlyde version of https://github.com/Shivangi0503/Wine_Clustering_KMeans.
 
 To run this example, you need to install its dependencies first:
 
 ```bash
@@ -280,31 +285,37 @@
 pip install .
 cd ..
 ```
 
 After going back to the main folder you can run it with:
 
 ```bash
-./flyde.py examples/Clustering.flyde
+pyflyde examples/Clustering.flyde
 ```
 
 ## Contributing
 
 ### Install dev dependencies
 
 ```bash
 pip install .\[dev\]
 ```
 
-### Run tests and coverage reports
+### Run tests, linters and coverage reports
 
 To run tests only:
 
 ```bash
 make test
 ```
 
-TO run tests with coverage and see report:
+To run tests with coverage and see report:
 
 ```bash
 make cover report
 ```
+
+To run linters:
+
+```bash
+make lint
+```
```

### Comparing `pyflyde-0.0.6/README.md` & `pyflyde-0.0.7/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 # PyFlyde
 
 ![Build](https://github.com/trustmaster/pyflyde/actions/workflows/python-package.yml/badge.svg)
+[<img src="https://readthedocs.org/projects/pyflyde/badge/">](https://pyflyde.readthedocs.io/en/latest/)
 
 Python runtime for [Flyde](https://github.com/flydelabs/flyde) with Data Engineering emphasis.
 
 ![Example graph running K-means clustering with Pandas and Scikit-learn](https://github.com/trustmaster/pyflyde/blob/main/clustering_example.png?raw=true)
 
-## PoC warning
-
-This is a proof-of-concept and not a final implementation. Structure and API may change drastically before public release.
-
 ## Getting started
 
 You need Python 3.9+ installed on your machine to run PyFlyde.
 
-First, you need to install its dependencies:
+Then you can install PyFlyde using pip:
 
 ```bash
-pip install .
+pip install pyflyde
 ```
 
-Then you can run the Hello World example:
+### Running the examples
+
+You can copy `examples` folder from this repository to your local project to give it a try. Then you can run the example flow with:
 
 ```bash
-./flyde.py examples/HelloPy.flyde
+pyflyde examples/HelloWorld.flyde
 ```
 
+
 ### Using the visual editor
 
-Install Flyde VSCode extension from the [marketplace](https://marketplace.visualstudio.com/items?itemName=flyde.flyde-vscode).
+Install Flyde VSCode extension from the [marketplace](https://marketplace.visualstudio.com/items?itemName=flyde.flyde-vscode). It will open existing `.flyde` files in the visual editor. You can call `Flyde: New Visual Flow` command in VSCode to create a new flow file.
+
+You can browse the component library in the panel on the right. To see your local components click the "View all" button. They will appear under the "Current project". Note that PyFlyde doesn't implement all of the Flyde's stdlib components, only a few essential ones.
 
-Whenever you change your component library classes or their interfaces, use flyde.py gen command to generate .flyde.ts definitions, e.g.:
+Whenever you change your component library classes or their interfaces, use `pyflyde gen` command to generate `.flyde.ts` definitions, e.g.:
 
 ```bash
-./flyde.py gen examples/mylib/components.py
+pyflyde gen examples/mylib/components.py
 ```
 
+Flyde editor needs `.flyde.ts` files in order to "see" your components.
+
 ## Running a Machine Learning example
 
 `Clustering.flyde` is a more complex example which uses Pandas and Scikit-Learn to run K-means clustering on a [wine clustering dataset from Kaggle](https://www.kaggle.com/harrywang/wine-dataset-for-clustering). It's a PyFlyde version of https://github.com/Shivangi0503/Wine_Clustering_KMeans.
 
 To run this example, you need to install its dependencies first:
 
 ```bash
@@ -47,31 +51,37 @@
 pip install .
 cd ..
 ```
 
 After going back to the main folder you can run it with:
 
 ```bash
-./flyde.py examples/Clustering.flyde
+pyflyde examples/Clustering.flyde
 ```
 
 ## Contributing
 
 ### Install dev dependencies
 
 ```bash
 pip install .\[dev\]
 ```
 
-### Run tests and coverage reports
+### Run tests, linters and coverage reports
 
 To run tests only:
 
 ```bash
 make test
 ```
 
-TO run tests with coverage and see report:
+To run tests with coverage and see report:
 
 ```bash
 make cover report
 ```
+
+To run linters:
+
+```bash
+make lint
+```
```

### Comparing `pyflyde-0.0.6/clustering_example.png` & `pyflyde-0.0.7/clustering_example.png`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.6/examples/Clustering.flyde` & `pyflyde-0.0.7/examples/Clustering.flyde`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.6/examples/HelloPy.flyde` & `pyflyde-0.0.7/examples/HelloPy.flyde`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.6/examples/datasets/wine-clustering.csv` & `pyflyde-0.0.7/examples/datasets/wine-clustering.csv`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.6/examples/mylib/components.flyde.ts` & `pyflyde-0.0.7/examples/mylib/components.flyde.ts`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.6/examples/mylib/components.py` & `pyflyde-0.0.7/examples/mylib/components.py`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.6/examples/mylib/dataframe.flyde.ts` & `pyflyde-0.0.7/examples/mylib/dataframe.flyde.ts`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.6/examples/mylib/dataframe.py` & `pyflyde-0.0.7/examples/mylib/dataframe.py`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.6/examples/mylib/kmeans.flyde.ts` & `pyflyde-0.0.7/examples/mylib/kmeans.flyde.ts`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.6/examples/mylib/kmeans.py` & `pyflyde-0.0.7/examples/mylib/kmeans.py`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.6/flyde/cli.py` & `pyflyde-0.0.7/flyde/cli.py`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.6/flyde/flow.py` & `pyflyde-0.0.7/flyde/flow.py`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.6/flyde/io.py` & `pyflyde-0.0.7/flyde/io.py`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.6/flyde/io.pyi` & `pyflyde-0.0.7/flyde/stdlib.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-from _typeshed import Incomplete as Incomplete
+from _typeshed import Incomplete
 from enum import Enum
-from queue import Queue
+from flyde.io import Input as Input, InputMode as InputMode, Output as Output
+from flyde.node import Component as Component
 from typing import Any
 
-EOF: Incomplete
-
-def is_EOF(value: Any) -> bool: ...
-
-class InputMode(Enum):
-    QUEUE: str
-    STICKY: str
-    STATIC: str
-
-class Requiredness(Enum):
-    REQUIRED: str
-    OPTIONAL: str
-    REQUIRED_IF_CONNECTED: str
-
-class OutputMode(Enum):
-    REF: str
-    VALUE: str
-    CIRCLE: str
-
-class Input:
-    id: Incomplete
-    description: Incomplete
-    type: Incomplete
-    required: Incomplete
-    def __init__(self, /, id: str = '', description: str = '', mode: InputMode = ..., type: type | None = None, value: Any = None, required: Requiredness = ...) -> None: ...
-    @property
-    def queue(self) -> Queue: ...
-    @property
-    def value(self) -> Any: ...
-    @value.setter
-    def value(self, value: Any): ...
-    def get(self) -> Any: ...
-    def empty(self) -> bool: ...
-    def count(self) -> int: ...
-
-class Output:
-    id: Incomplete
-    description: Incomplete
-    type: Incomplete
-    delayed: Incomplete
-    def __init__(self, /, id: str = '', description: str = '', mode: OutputMode = ..., type: type | None = None, delayed: bool = False) -> None: ...
-    def connect(self, queue: Queue): ...
-    @property
-    def connected(self) -> bool: ...
-    def send(self, value: Any): ...
-
-class RedirectQueue:
-    def __init__(self, output: Output) -> None: ...
-    def put(self, item: Any, block: bool = True, timeout: Incomplete | None = None): ...
-
-class GraphPort(Input, Output):
-    def __init__(self, id: str = '', description: str = '', type: type | None = None, value: Any = None, required: Requiredness = ..., output_mode: OutputMode = ..., delayed: bool = False) -> None: ...
-
-class ConnectionNode:
-    ins_id: Incomplete
-    pin_id: Incomplete
-    def __init__(self, ins_id: str, pin_id: str) -> None: ...
-
-class Connection:
-    from_node: Incomplete
-    to_node: Incomplete
-    delayed: Incomplete
-    hidden: Incomplete
-    def __init__(self, from_node: ConnectionNode, to_node: ConnectionNode, delayed: bool = False, hidden: bool = False) -> None: ...
-    @classmethod
-    def from_yaml(cls, yml: dict): ...
-    def to_dict(self) -> dict: ...
+class InlineValue(Component):
+    """InlineValue sends a constant value to output."""
+    outputs: Incomplete
+    value: Incomplete
+    def __init__(self, macro_data: dict, **kwargs) -> None: ...
+    def process(self) -> None: ...
+
+class _ConditionType(Enum):
+    """Condition type enumeration."""
+    Equal: str
+    NotEqual: str
+    GreaterThan: str
+    GreaterThanOrEqual: str
+    LessThan: str
+    LessThanOrEqual: str
+    Contains: str
+    NotContains: str
+    RegexMatches: str
+    IsEmpty: str
+    IsNotEmpty: str
+    IsNull: str
+    IsNotNull: str
+    IsUndefined: str
+    IsNotUndefined: str
+    HasProperty: str
+    LengthEqual: str
+    LengthNotEqual: str
+    LengthGreaterThan: str
+    LengthLessThan: str
+    TypeEquals: str
+    Expression: str
+
+class _ConditionalConfig:
+    """Conditional configuration."""
+    property_path: Incomplete
+    condition_type: Incomplete
+    condition_data: Incomplete
+    compare_to_mode: Incomplete
+    compare_to_value: Incomplete
+    compare_to_type: Incomplete
+    compare_to_property_path: str
+    true_value_type: Incomplete
+    true_value_expression: Incomplete
+    false_value_type: Incomplete
+    false_value_expression: Incomplete
+    def __init__(self, yml: dict) -> None: ...
+
+def _get_attribute_by_path(obj: Any, path: str) -> Any:
+    """Gets nested attribute by property path."""
+
+class Conditional(Component):
+    """Conditional component evaluates a condition against the input and sends the result to output."""
+    inputs: Incomplete
+    outputs: Incomplete
+    _config: Incomplete
+    def __init__(self, macro_data: dict, **kwargs) -> None: ...
+    def _evaluate(self, value: Any, compareTo: Any) -> bool: ...
+    def process(self, value: Any, compareTo: Any): ...
+
+class GetAttribute(Component):
+    """Get an attribute from an object or dictionary."""
+    inputs: Incomplete
+    outputs: Incomplete
+    value: Incomplete
+    def __init__(self, macro_data: dict, **kwargs) -> None: ...
+    def process(self, object: Any, attribute: str): ...
```

### Comparing `pyflyde-0.0.6/flyde/node.py` & `pyflyde-0.0.7/flyde/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import Any, Callable
 from uuid import uuid4
 
 from flyde.io import GraphPort, InputMode, Input, Output, EOF, Requiredness, is_EOF, Connection
 
 logger = logging.getLogger(__name__)
 
+SUPPORTED_MACROS = ["InlineValue", "Conditional", "GetAttribute"]
 
 # InstanceFactory is a function that creates a new instance of a node.
 # It can create instances dynamically based on the node ID.
 InstanceFactory = Callable[[str, dict], Any]
 
 
 class Node(ABC):
@@ -124,18 +125,15 @@
             "id": yml["id"],
             "input_config": yml.get("inputConfig", {}),
             "display_name": yml.get("displayName", ""),
             "stopped": yml.get("stopped", None),  # It's a hacky way to pass the stopped event to the constructor
         }
         # If macro parameters are present, pass them to the constructor
         if "macroData" in yml:
-            if "value" in yml["macroData"]:
-                args["value"] = yml["macroData"]["value"]
-            if "key" in yml["macroData"]:
-                args["key"] = yml["macroData"]["key"]
+            args["macro_data"] = yml["macroData"]
         return create(node_class_name, args)
 
     def to_dict(self) -> dict:
         return {
             "id": self._id,
             "nodeId": self._node_type,
             "inputConfig": self._input_config,
@@ -406,15 +404,15 @@
         # Load instances and macros
         instances = {}
         instances_stopped = {}
         for ins in yml.get("instances", []):
             ins_id = ins["id"]
             if "macroId" in ins:
                 # Only InlineValue macros are supported for now
-                if ins["macroId"] not in ["InlineValue", "GetAttribute"]:
+                if ins["macroId"] not in SUPPORTED_MACROS:
                     raise ValueError(f'Unsupported macro: {ins["macroId"]}')
                 ins["nodeId"] = ins["macroId"]
             stopped = Event()
             ins["stopped"] = stopped
             logger.debug(f"Creating instance {ins_id}")
             instances[ins_id] = Node.from_yaml(create, ins)
             instances_stopped[ins_id] = stopped
```

### Comparing `pyflyde-0.0.6/pyflyde.egg-info/PKG-INFO` & `pyflyde-0.0.7/pyflyde.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyflyde
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python SDK and runtime for Flyde - a visual flow-based programming language and IDE.
 Author: Vladimir Sibirov
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -226,53 +226,58 @@
 Requires-Dist: setuptools; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: twine; extra == "dev"
+Requires-Dist: mkdocs; extra == "dev"
 
 # PyFlyde
 
 ![Build](https://github.com/trustmaster/pyflyde/actions/workflows/python-package.yml/badge.svg)
+[<img src="https://readthedocs.org/projects/pyflyde/badge/">](https://pyflyde.readthedocs.io/en/latest/)
 
 Python runtime for [Flyde](https://github.com/flydelabs/flyde) with Data Engineering emphasis.
 
 ![Example graph running K-means clustering with Pandas and Scikit-learn](https://github.com/trustmaster/pyflyde/blob/main/clustering_example.png?raw=true)
 
-## PoC warning
-
-This is a proof-of-concept and not a final implementation. Structure and API may change drastically before public release.
-
 ## Getting started
 
 You need Python 3.9+ installed on your machine to run PyFlyde.
 
-First, you need to install its dependencies:
+Then you can install PyFlyde using pip:
 
 ```bash
-pip install .
+pip install pyflyde
 ```
 
-Then you can run the Hello World example:
+### Running the examples
+
+You can copy `examples` folder from this repository to your local project to give it a try. Then you can run the example flow with:
 
 ```bash
-./flyde.py examples/HelloPy.flyde
+pyflyde examples/HelloWorld.flyde
 ```
 
+
 ### Using the visual editor
 
-Install Flyde VSCode extension from the [marketplace](https://marketplace.visualstudio.com/items?itemName=flyde.flyde-vscode).
+Install Flyde VSCode extension from the [marketplace](https://marketplace.visualstudio.com/items?itemName=flyde.flyde-vscode). It will open existing `.flyde` files in the visual editor. You can call `Flyde: New Visual Flow` command in VSCode to create a new flow file.
+
+You can browse the component library in the panel on the right. To see your local components click the "View all" button. They will appear under the "Current project". Note that PyFlyde doesn't implement all of the Flyde's stdlib components, only a few essential ones.
 
-Whenever you change your component library classes or their interfaces, use flyde.py gen command to generate .flyde.ts definitions, e.g.:
+Whenever you change your component library classes or their interfaces, use `pyflyde gen` command to generate `.flyde.ts` definitions, e.g.:
 
 ```bash
-./flyde.py gen examples/mylib/components.py
+pyflyde gen examples/mylib/components.py
 ```
 
+Flyde editor needs `.flyde.ts` files in order to "see" your components.
+
 ## Running a Machine Learning example
 
 `Clustering.flyde` is a more complex example which uses Pandas and Scikit-Learn to run K-means clustering on a [wine clustering dataset from Kaggle](https://www.kaggle.com/harrywang/wine-dataset-for-clustering). It's a PyFlyde version of https://github.com/Shivangi0503/Wine_Clustering_KMeans.
 
 To run this example, you need to install its dependencies first:
 
 ```bash
@@ -280,31 +285,37 @@
 pip install .
 cd ..
 ```
 
 After going back to the main folder you can run it with:
 
 ```bash
-./flyde.py examples/Clustering.flyde
+pyflyde examples/Clustering.flyde
 ```
 
 ## Contributing
 
 ### Install dev dependencies
 
 ```bash
 pip install .\[dev\]
 ```
 
-### Run tests and coverage reports
+### Run tests, linters and coverage reports
 
 To run tests only:
 
 ```bash
 make test
 ```
 
-TO run tests with coverage and see report:
+To run tests with coverage and see report:
 
 ```bash
 make cover report
 ```
+
+To run linters:
+
+```bash
+make lint
+```
```

### Comparing `pyflyde-0.0.6/pyproject.toml` & `pyflyde-0.0.7/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyflyde"
-version = "0.0.6"
+version = "0.0.7"
 requires-python = ">= 3.9"
 authors = [
     {name = "Vladimir Sibirov"}
 ]
 description="Python SDK and runtime for Flyde - a visual flow-based programming language and IDE."
 readme="README.md"
 classifiers = [
@@ -30,23 +30,24 @@
 license = { file = "LICENSE" }
 
 dependencies = [
     "pyyaml",
 ]
 
 [project.scripts]
-flyde-py = "flyde.cli:main"
+pyflyde = "flyde.cli:main"
 
-# [tool.setuptools]
+[tool.setuptools]
 # package-dir = { "" = "flyde" }
-# packages = ["flyde"]
+packages = ["flyde"]
 
 [project.optional-dependencies]
 dev = [
     "setuptools",
     "build",
     "black",
     "coverage",
     "flake8",
     "mypy",
     "twine",
+    "mkdocs",
 ]
```

### Comparing `pyflyde-0.0.6/tests/Repeat3Times.flyde` & `pyflyde-0.0.7/tests/Repeat3Times.flyde`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.6/tests/TestIsolatedFlow.flyde` & `pyflyde-0.0.7/tests/TestIsolatedFlow.flyde`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.6/tests/TestNestedFlow.flyde` & `pyflyde-0.0.7/tests/TestNestedFlow.flyde`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.6/tests/components.flyde.ts` & `pyflyde-0.0.7/tests/components.flyde.ts`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,22 @@
 import { CodeNode } from "@flyde/core";
 
+export const Format: CodeNode = {
+  id: "Format",
+  description: "Formats the input value with a given format string and sends it to out.",
+  inputs: {
+    inp: { description: "The input" },
+    format: { description: "The format string" }
+  },
+  outputs: {
+    out: { description: "The formatted output" }
+  },
+  run: () => { return; },
+};
+
 export const Echo: CodeNode = {
   id: "Echo",
   description: "A simple component that echoes the input.",
   inputs: {
     inp: { description: "The input" }
   },
   outputs: {
```

### Comparing `pyflyde-0.0.6/tests/components.py` & `pyflyde-0.0.7/tests/components.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,28 @@
 from flyde.io import Input, InputMode, Output
 from flyde.node import Component
 
 
+class Format(Component):
+    """Formats the input value with a given format string and sends it to out."""
+
+    inputs = {
+        "inp": Input(description="The input"),
+        "format": Input(
+            description="The format string", type=str, mode=InputMode.STICKY
+        ),
+    }
+    outputs = {
+        "out": Output(description="The formatted output", type=str),
+    }
+
+    def process(self, inp: str, format: str = "{inp}"):
+        self.send("out", format.format(inp=inp))
+
+
 class Echo(Component):
     """A simple component that echoes the input."""
 
     inputs = {"inp": Input(description="The input", type=str)}
     outputs = {"out": Output(description="The output", type=str)}
 
     def process(self, inp: str) -> dict[str, str]:
```

### Comparing `pyflyde-0.0.6/tests/test_flow.py` & `pyflyde-0.0.7/tests/test_flow.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,16 @@
         flow.stopped.wait()
         self.assertTrue(flow.stopped.is_set())
 
 
 class TestInOutFlow(unittest.TestCase):
     def test_flow(self):
         test_case = {
-            "inputs": ["Hello", "World", EOF],
-            "outputs": ["Hello", "World", EOF],
+            "inputs": ["Hello", "World", "", EOF],
+            "outputs": ["Hello", "World", "ERR: msg is empty", EOF],
         }
         flow = Flow.from_file("tests/TestInOutFlow.flyde")
 
         in_q = flow.node.inputs["inMsg"].queue
         out_q = Queue()
         flow.node.outputs["outMsg"].connect(out_q)
```

### Comparing `pyflyde-0.0.6/tests/test_io.py` & `pyflyde-0.0.7/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.6/tests/test_node.py` & `pyflyde-0.0.7/tests/test_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,20 +167,19 @@
             "nodeId": "RepeatWordNTimes",
             "inputConfig": {},
             "displayName": "Repeat",
             "macroData": {"value": 100, "key": "foo"},
         }
 
         def factory(class_name: str, args: dict):
-            self.assertEqual(args["value"], yaml["macroData"]["value"])
-            self.assertEqual(args["key"], yaml["macroData"]["key"])
-            # Drop value and key from the args, otherwise there will be an exception
-            # because the constructor doesn't support them.
-            del args["value"]
-            del args["key"]
+            self.assertEqual(args["macro_data"]["value"], yaml["macroData"]["value"])
+            self.assertEqual(args["macro_data"]["key"], yaml["macroData"]["key"])
+            # Drop macro_data from the args, otherwise there will be an exception
+            # because the constructor doesn't support it.
+            del args["macro_data"]
             return RepeatWordNTimes(**args)
 
         node = Component.from_yaml(factory, yaml)
         self.assertEqual(node._id, "repeat")
         self.assertEqual(node._display_name, "Repeat")
         self.assertEqual(node._node_type, "RepeatWordNTimes")
         self.assertEqual(len(node.inputs), 2)
```

