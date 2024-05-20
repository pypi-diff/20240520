# Comparing `tmp/pybedlite-0.0.4.tar.gz` & `tmp/pybedlite-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybedlite-0.0.4.tar", max compression
+gzip compressed data, was "pybedlite-0.1.0.tar", max compression
```

## Comparing `pybedlite-0.0.4.tar` & `pybedlite-0.1.0.tar`

### file list

```diff
@@ -1,66 +1,63 @@
--rw-r--r--   0        0        0     1315 2023-09-08 18:37:07.536971 pybedlite-0.0.4/LICENSE
--rw-r--r--   0        0        0     3359 2023-09-11 17:03:04.967363 pybedlite-0.0.4/README.md
--rw-r--r--   0        0        0      621 2023-09-11 17:03:04.967510 pybedlite-0.0.4/build.py
--rw-r--r--   0        0        0       33 2023-09-08 18:53:00.540418 pybedlite-0.0.4/cgranges/.git
--rw-r--r--   0        0        0       28 2023-09-08 18:53:00.544878 pybedlite-0.0.4/cgranges/.gitignore
--rw-r--r--   0        0        0       37 2023-09-08 20:13:44.291082 pybedlite-0.0.4/cgranges/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2023-09-08 20:13:44.291138 pybedlite-0.0.4/cgranges/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2023-09-08 20:13:44.291008 pybedlite-0.0.4/cgranges/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2023-09-08 20:13:44.291206 pybedlite-0.0.4/cgranges/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2023-09-08 20:13:44.291285 pybedlite-0.0.4/cgranges/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0     1093 2023-09-08 18:53:00.544963 pybedlite-0.0.4/cgranges/LICENSE.txt
--rw-r--r--   0        0        0       65 2023-09-08 18:53:00.545027 pybedlite-0.0.4/cgranges/MANIFEST.in
--rw-r--r--   0        0        0      200 2023-09-08 18:53:00.545085 pybedlite-0.0.4/cgranges/Makefile
--rw-r--r--   0        0        0     6254 2023-09-08 18:53:00.545211 pybedlite-0.0.4/cgranges/README.md
--rw-r--r--   0        0        0     8537 2023-09-08 18:53:00.545330 pybedlite-0.0.4/cgranges/cgranges.c
--rw-r--r--   0        0        0     3259 2023-09-08 18:53:00.545404 pybedlite-0.0.4/cgranges/cgranges.h
--rw-r--r--   0        0        0     4945 2023-09-08 18:53:00.545519 pybedlite-0.0.4/cgranges/cpp/IITree.h
--rw-r--r--   0        0        0     3027 2023-09-08 18:53:00.545618 pybedlite-0.0.4/cgranges/cpp/IITreeBFS.h
--rw-r--r--   0        0        0      100 2023-09-08 18:53:00.545676 pybedlite-0.0.4/cgranges/cpp/Makefile
--rw-r--r--   0        0        0      340 2023-09-08 18:53:00.545743 pybedlite-0.0.4/cgranges/cpp/example.cpp
--rw-r--r--   0        0        0      691 2023-09-08 18:53:00.545808 pybedlite-0.0.4/cgranges/example.c
--rw-r--r--   0        0        0    21543 2023-09-08 18:53:00.545935 pybedlite-0.0.4/cgranges/khash.h
--rw-r--r--   0        0        0      196 2023-09-08 18:53:00.546126 pybedlite-0.0.4/cgranges/python/README.rst
--rw-r--r--   0        0        0   441785 2023-09-08 23:58:53.444321 pybedlite-0.0.4/cgranges/python/cgranges.c
--rw-r--r--   0        0        0     1865 2023-09-08 18:53:00.546233 pybedlite-0.0.4/cgranges/python/cgranges.pyx
--rw-r--r--   0        0        0     1335 2023-09-08 18:53:00.546302 pybedlite-0.0.4/cgranges/setup.py
--rw-r--r--   0        0        0    12872 2023-09-08 18:53:00.546521 pybedlite-0.0.4/cgranges/test/3rd-party/AIList/AIList.c
--rw-r--r--   0        0        0     1301 2023-09-08 18:53:00.546609 pybedlite-0.0.4/cgranges/test/3rd-party/AIList/AIList.h
--rw-r--r--   0        0        0     5143 2023-09-08 18:53:00.546743 pybedlite-0.0.4/cgranges/test/3rd-party/AITree/AITree.c
--rw-r--r--   0        0        0      490 2023-09-08 18:53:00.546820 pybedlite-0.0.4/cgranges/test/3rd-party/AITree/compiler.h
--rw-r--r--   0        0        0      302 2023-09-08 18:53:00.546880 pybedlite-0.0.4/cgranges/test/3rd-party/AITree/interval_tree.c
--rw-r--r--   0        0        0      751 2023-09-08 18:53:00.546945 pybedlite-0.0.4/cgranges/test/3rd-party/AITree/interval_tree.h
--rw-r--r--   0        0        0     7148 2023-09-08 18:53:00.547035 pybedlite-0.0.4/cgranges/test/3rd-party/AITree/interval_tree_generic.h
--rw-r--r--   0        0        0    15046 2023-09-08 18:53:00.547140 pybedlite-0.0.4/cgranges/test/3rd-party/AITree/rbtree.c
--rw-r--r--   0        0        0     3756 2023-09-08 18:53:00.547219 pybedlite-0.0.4/cgranges/test/3rd-party/AITree/rbtree.h
--rw-r--r--   0        0        0     7570 2023-09-08 18:53:00.547304 pybedlite-0.0.4/cgranges/test/3rd-party/AITree/rbtree_augmented.h
--rw-r--r--   0        0        0    20195 2023-09-08 18:53:00.547470 pybedlite-0.0.4/cgranges/test/3rd-party/NCList/intervaldb.c
--rw-r--r--   0        0        0     5353 2023-09-08 18:53:00.547572 pybedlite-0.0.4/cgranges/test/3rd-party/NCList/intervaldb.h
--rw-r--r--   0        0        0       39 2023-09-08 18:53:00.547643 pybedlite-0.0.4/cgranges/test/3rd-party/README.md
--rw-r--r--   0        0        0    11995 2023-09-08 18:53:00.547762 pybedlite-0.0.4/cgranges/test/IntervalTree.h
--rw-r--r--   0        0        0      719 2023-09-08 18:53:00.547838 pybedlite-0.0.4/cgranges/test/Makefile
--rw-r--r--   0        0        0     2554 2023-09-08 18:53:00.547932 pybedlite-0.0.4/cgranges/test/bedcov-cr.c
--rwxr-xr-x   0        0        0     2964 2023-09-08 18:53:00.548018 pybedlite-0.0.4/cgranges/test/bedcov-cr.js
--rwxr-xr-x   0        0        0      871 2023-09-08 18:53:00.548102 pybedlite-0.0.4/cgranges/test/bedcov-cr.py
--rwxr-xr-x   0        0        0     1124 2023-09-08 18:53:00.548156 pybedlite-0.0.4/cgranges/test/bedcov-cr1.py
--rwxr-xr-x   0        0        0      851 2023-09-08 18:53:00.548225 pybedlite-0.0.4/cgranges/test/bedcov-cr2.py
--rw-r--r--   0        0        0     2668 2023-09-08 18:53:00.548292 pybedlite-0.0.4/cgranges/test/bedcov-iitree.cpp
--rw-r--r--   0        0        0     2850 2023-09-08 18:53:00.548377 pybedlite-0.0.4/cgranges/test/bedcov-itree.cpp
--rwxr-xr-x   0        0        0     2842 2023-09-08 18:53:00.548461 pybedlite-0.0.4/cgranges/test/bedcov-naive.js
--rwxr-xr-x   0        0        0     1214 2023-09-08 18:53:00.548524 pybedlite-0.0.4/cgranges/test/bedcov-ncls.py
--rw-r--r--   0        0        0     6695 2023-09-08 18:53:00.548611 pybedlite-0.0.4/cgranges/test/bedcov-py-iitree.py
--rwxr-xr-x   0        0        0      902 2023-09-08 18:53:00.548684 pybedlite-0.0.4/cgranges/test/bedcov-qs.py
--rw-r--r--   0        0        0     4837 2023-09-08 18:53:00.548771 pybedlite-0.0.4/cgranges/test/kseq.h
--rw-r--r--   0        0        0       58 2023-09-08 18:53:00.548837 pybedlite-0.0.4/cgranges/test/test1.bed
--rw-r--r--   0        0        0       45 2023-09-08 18:53:00.548895 pybedlite-0.0.4/cgranges/test/test2.bed
--rw-r--r--   0        0        0     2709 2023-09-08 18:37:07.538474 pybedlite-0.0.4/pybedlite/__init__.py
--rw-r--r--   0        0        0     7536 2023-09-08 18:37:07.538582 pybedlite-0.0.4/pybedlite/bed_record.py
--rw-r--r--   0        0        0     6349 2023-09-08 18:37:07.538688 pybedlite-0.0.4/pybedlite/bed_source.py
--rw-r--r--   0        0        0     5727 2023-09-08 18:37:07.538811 pybedlite-0.0.4/pybedlite/bed_writer.py
--rw-r--r--   0        0        0     9413 2023-09-11 17:03:04.968448 pybedlite-0.0.4/pybedlite/overlap_detector.py
--rw-r--r--   0        0        0       42 2023-09-08 18:37:07.539047 pybedlite-0.0.4/pybedlite/tests/__init__.py
--rw-r--r--   0        0        0     4837 2023-09-08 18:37:07.539132 pybedlite-0.0.4/pybedlite/tests/test_overlap_detector.py
--rw-r--r--   0        0        0     7417 2023-09-11 17:03:04.968838 pybedlite-0.0.4/pybedlite/tests/test_pybedlite.py
--rw-r--r--   0        0        0     1436 2023-09-11 17:03:17.916650 pybedlite-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     4598 1970-01-01 00:00:00.000000 pybedlite-0.0.4/setup.py
--rw-r--r--   0        0        0     4601 1970-01-01 00:00:00.000000 pybedlite-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1315 2024-05-20 17:03:15.038174 pybedlite-0.1.0/LICENSE
+-rw-r--r--   0        0        0     3459 2024-05-20 17:03:15.038258 pybedlite-0.1.0/README.md
+-rw-r--r--   0        0        0      621 2024-05-20 17:03:15.038328 pybedlite-0.1.0/build.py
+-rw-r--r--   0        0        0       33 2024-05-20 17:03:16.348724 pybedlite-0.1.0/cgranges/.git
+-rw-r--r--   0        0        0       28 2024-05-20 17:03:16.391788 pybedlite-0.1.0/cgranges/.gitignore
+-rw-r--r--   0        0        0     1093 2024-05-20 17:03:16.391887 pybedlite-0.1.0/cgranges/LICENSE.txt
+-rw-r--r--   0        0        0       65 2024-05-20 17:03:16.391949 pybedlite-0.1.0/cgranges/MANIFEST.in
+-rw-r--r--   0        0        0      200 2024-05-20 17:03:16.392013 pybedlite-0.1.0/cgranges/Makefile
+-rw-r--r--   0        0        0     6254 2024-05-20 17:03:16.392171 pybedlite-0.1.0/cgranges/README.md
+-rw-r--r--   0        0        0     8537 2024-05-20 17:03:16.392343 pybedlite-0.1.0/cgranges/cgranges.c
+-rw-r--r--   0        0        0     3259 2024-05-20 17:03:16.392417 pybedlite-0.1.0/cgranges/cgranges.h
+-rw-r--r--   0        0        0     4945 2024-05-20 17:03:16.392554 pybedlite-0.1.0/cgranges/cpp/IITree.h
+-rw-r--r--   0        0        0     3027 2024-05-20 17:03:16.392653 pybedlite-0.1.0/cgranges/cpp/IITreeBFS.h
+-rw-r--r--   0        0        0      100 2024-05-20 17:03:16.392711 pybedlite-0.1.0/cgranges/cpp/Makefile
+-rw-r--r--   0        0        0      340 2024-05-20 17:03:16.392785 pybedlite-0.1.0/cgranges/cpp/example.cpp
+-rw-r--r--   0        0        0      691 2024-05-20 17:03:16.392851 pybedlite-0.1.0/cgranges/example.c
+-rw-r--r--   0        0        0    21543 2024-05-20 17:03:16.392953 pybedlite-0.1.0/cgranges/khash.h
+-rw-r--r--   0        0        0      196 2024-05-20 17:03:16.393070 pybedlite-0.1.0/cgranges/python/README.rst
+-rw-r--r--   0        0        0   447381 2024-05-20 17:04:03.127914 pybedlite-0.1.0/cgranges/python/cgranges.c
+-rw-r--r--   0        0        0     1865 2024-05-20 17:03:16.393140 pybedlite-0.1.0/cgranges/python/cgranges.pyx
+-rw-r--r--   0        0        0     1335 2024-05-20 17:03:16.393207 pybedlite-0.1.0/cgranges/setup.py
+-rw-r--r--   0        0        0    12872 2024-05-20 17:03:16.393490 pybedlite-0.1.0/cgranges/test/3rd-party/AIList/AIList.c
+-rw-r--r--   0        0        0     1301 2024-05-20 17:03:16.393634 pybedlite-0.1.0/cgranges/test/3rd-party/AIList/AIList.h
+-rw-r--r--   0        0        0     5143 2024-05-20 17:03:16.393789 pybedlite-0.1.0/cgranges/test/3rd-party/AITree/AITree.c
+-rw-r--r--   0        0        0      490 2024-05-20 17:03:16.393869 pybedlite-0.1.0/cgranges/test/3rd-party/AITree/compiler.h
+-rw-r--r--   0        0        0      302 2024-05-20 17:03:16.393937 pybedlite-0.1.0/cgranges/test/3rd-party/AITree/interval_tree.c
+-rw-r--r--   0        0        0      751 2024-05-20 17:03:16.394012 pybedlite-0.1.0/cgranges/test/3rd-party/AITree/interval_tree.h
+-rw-r--r--   0        0        0     7148 2024-05-20 17:03:16.394129 pybedlite-0.1.0/cgranges/test/3rd-party/AITree/interval_tree_generic.h
+-rw-r--r--   0        0        0    15046 2024-05-20 17:03:16.394245 pybedlite-0.1.0/cgranges/test/3rd-party/AITree/rbtree.c
+-rw-r--r--   0        0        0     3756 2024-05-20 17:03:16.394317 pybedlite-0.1.0/cgranges/test/3rd-party/AITree/rbtree.h
+-rw-r--r--   0        0        0     7570 2024-05-20 17:03:16.394416 pybedlite-0.1.0/cgranges/test/3rd-party/AITree/rbtree_augmented.h
+-rw-r--r--   0        0        0    20195 2024-05-20 17:03:16.394566 pybedlite-0.1.0/cgranges/test/3rd-party/NCList/intervaldb.c
+-rw-r--r--   0        0        0     5353 2024-05-20 17:03:16.394703 pybedlite-0.1.0/cgranges/test/3rd-party/NCList/intervaldb.h
+-rw-r--r--   0        0        0       39 2024-05-20 17:03:16.394763 pybedlite-0.1.0/cgranges/test/3rd-party/README.md
+-rw-r--r--   0        0        0    11995 2024-05-20 17:03:16.394895 pybedlite-0.1.0/cgranges/test/IntervalTree.h
+-rw-r--r--   0        0        0      719 2024-05-20 17:03:16.394960 pybedlite-0.1.0/cgranges/test/Makefile
+-rw-r--r--   0        0        0     2554 2024-05-20 17:03:16.395052 pybedlite-0.1.0/cgranges/test/bedcov-cr.c
+-rwxr-xr-x   0        0        0     2964 2024-05-20 17:03:16.395118 pybedlite-0.1.0/cgranges/test/bedcov-cr.js
+-rwxr-xr-x   0        0        0      871 2024-05-20 17:03:16.395195 pybedlite-0.1.0/cgranges/test/bedcov-cr.py
+-rwxr-xr-x   0        0        0     1124 2024-05-20 17:03:16.395251 pybedlite-0.1.0/cgranges/test/bedcov-cr1.py
+-rwxr-xr-x   0        0        0      851 2024-05-20 17:03:16.395310 pybedlite-0.1.0/cgranges/test/bedcov-cr2.py
+-rw-r--r--   0        0        0     2668 2024-05-20 17:03:16.395366 pybedlite-0.1.0/cgranges/test/bedcov-iitree.cpp
+-rw-r--r--   0        0        0     2850 2024-05-20 17:03:16.395443 pybedlite-0.1.0/cgranges/test/bedcov-itree.cpp
+-rwxr-xr-x   0        0        0     2842 2024-05-20 17:03:16.395506 pybedlite-0.1.0/cgranges/test/bedcov-naive.js
+-rwxr-xr-x   0        0        0     1214 2024-05-20 17:03:16.395563 pybedlite-0.1.0/cgranges/test/bedcov-ncls.py
+-rw-r--r--   0        0        0     6695 2024-05-20 17:03:16.395666 pybedlite-0.1.0/cgranges/test/bedcov-py-iitree.py
+-rwxr-xr-x   0        0        0      902 2024-05-20 17:03:16.395725 pybedlite-0.1.0/cgranges/test/bedcov-qs.py
+-rw-r--r--   0        0        0     4837 2024-05-20 17:03:16.395815 pybedlite-0.1.0/cgranges/test/kseq.h
+-rw-r--r--   0        0        0       58 2024-05-20 17:03:16.395871 pybedlite-0.1.0/cgranges/test/test1.bed
+-rw-r--r--   0        0        0       45 2024-05-20 17:03:16.395924 pybedlite-0.1.0/cgranges/test/test2.bed
+-rw-r--r--   0        0        0     2709 2024-05-20 17:03:15.039726 pybedlite-0.1.0/pybedlite/__init__.py
+-rw-r--r--   0        0        0     8752 2024-05-20 17:03:15.039894 pybedlite-0.1.0/pybedlite/bed_record.py
+-rw-r--r--   0        0        0     6350 2024-05-20 17:03:15.040020 pybedlite-0.1.0/pybedlite/bed_source.py
+-rw-r--r--   0        0        0     5726 2024-05-20 17:03:15.040125 pybedlite-0.1.0/pybedlite/bed_writer.py
+-rw-r--r--   0        0        0    10087 2024-05-20 17:03:15.040296 pybedlite-0.1.0/pybedlite/overlap_detector.py
+-rw-r--r--   0        0        0        0 2024-05-20 17:03:15.040330 pybedlite-0.1.0/pybedlite/py.typed
+-rw-r--r--   0        0        0       42 2024-05-20 17:03:15.040441 pybedlite-0.1.0/pybedlite/tests/__init__.py
+-rw-r--r--   0        0        0     1291 2024-05-20 17:03:15.040559 pybedlite-0.1.0/pybedlite/tests/conftest.py
+-rw-r--r--   0        0        0     6255 2024-05-20 17:03:15.040699 pybedlite-0.1.0/pybedlite/tests/test_overlap_detector.py
+-rw-r--r--   0        0        0     6465 2024-05-20 17:03:15.040823 pybedlite-0.1.0/pybedlite/tests/test_pybedlite.py
+-rw-r--r--   0        0        0     1454 2024-05-20 17:03:40.720875 pybedlite-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4615 1970-01-01 00:00:00.000000 pybedlite-0.1.0/setup.py
+-rw-r--r--   0        0        0     4701 1970-01-01 00:00:00.000000 pybedlite-0.1.0/PKG-INFO
```

### Comparing `pybedlite-0.0.4/LICENSE` & `pybedlite-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pybedlite-0.0.4/README.md` & `pybedlite-0.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -34,34 +34,38 @@
 [pypi-downloads-link]:  https://pypi.python.org/pypi/pybedlite
 
 # pybedlite
 
 See documentation on [pybedlite.readthedocs.org][rtd-link].
 
 ```
+pip install pybedlite
+```
+OR
+```
 conda install -c bioconda pybedlite
 ```
 OR
 ```
 conda create -n pybedlite pybedlite
 conda activate pybedlite
 ```
 
-Note that while there is a version of pybedlite on pypi versions of pybedlite >=
-0.0.2 cannot at present be installed via pypi because they have dependencies
-that preclude publishing to pypi. For this reason installation via conda is
-required.
-
 [rtd-link]:    http://pybedlite.readthedocs.org/en/stable
 
 **Requires python 3.8+** (for python < 3.8, please use pybedlite <= 0.0.3)
 
 # Getting Setup for Development Work
 
-[Poetry][poetry-link] is used to manage the python development environment. 
+Clone the repository to your local machine. Note that pybedlite >= 0.0.4 includes [cgranges][cgranges-link] as a submodule, so you must use the `--recurse-submodules` option:
+```
+git clone --recurse-submodules https://github.com/fulcrumgenomics/pybedlite.git
+```
+
+[Poetry][poetry-link] is used to manage the python development environment.
 
 A simple way to create an environment with the desired version of python and poetry is to use [conda][conda-link].  E.g.:
 
 ```bash
 conda create -n pybedlite python=3.8 poetry
 conda activate pybedlite
 poetry install
@@ -77,13 +81,14 @@
 If, during `poetry install` on Mac OS X errors are encountered running gcc/clang to build `pybedtools` or other packages with native code, try setting the following and re-running `poetry install`:
 ```bash
 export CFLAGS="-stdlib=libc++"
 ``` 
 
 [poetry-link]: https://github.com/python-poetry/poetry
 [conda-link]:  https://docs.conda.io/en/latest/miniconda.html
+[cgranges-link]: https://github.com/lh3/cgranges
 
 ## Checking the Build
 ### Run all checks with:
 ```bash
 ./ci/check.sh
 ```
```

### Comparing `pybedlite-0.0.4/build.py` & `pybedlite-0.1.0/build.py`

 * *Files identical despite different names*

### Comparing `pybedlite-0.0.4/cgranges/LICENSE.txt` & `pybedlite-0.1.0/cgranges/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pybedlite-0.0.4/cgranges/README.md` & `pybedlite-0.1.0/cgranges/README.md`

 * *Files identical despite different names*

### Comparing `pybedlite-0.0.4/cgranges/cgranges.c` & `pybedlite-0.1.0/cgranges/cgranges.c`

 * *Files identical despite different names*

### Comparing `pybedlite-0.0.4/cgranges/cgranges.h` & `pybedlite-0.1.0/cgranges/cgranges.h`

 * *Files identical despite different names*

### Comparing `pybedlite-0.0.4/cgranges/cpp/IITree.h` & `pybedlite-0.1.0/cgranges/cpp/IITree.h`

 * *Files identical despite different names*

### Comparing `pybedlite-0.0.4/cgranges/cpp/IITreeBFS.h` & `pybedlite-0.1.0/cgranges/cpp/IITreeBFS.h`

 * *Files identical despite different names*

### Comparing `pybedlite-0.0.4/cgranges/example.c` & `pybedlite-0.1.0/cgranges/example.c`

 * *Files identical despite different names*

### Comparing `pybedlite-0.0.4/cgranges/khash.h` & `pybedlite-0.1.0/cgranges/khash.h`

 * *Files identical despite different names*

### Comparing `pybedlite-0.0.4/cgranges/python/cgranges.c` & `pybedlite-0.1.0/cgranges/python/cgranges.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.2 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "cgranges/cgranges.h",
             "cgranges/khash.h",
@@ -36,23 +36,23 @@
 
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02070000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
-#if CYTHON_LIMITED_API
+#if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_2" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030002F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -136,14 +136,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -197,14 +199,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -258,60 +262,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
-#elif defined(PY_NOGIL)
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
+#elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -394,14 +421,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -585,25 +615,28 @@
 #if CYTHON_COMPILING_IN_LIMITED_API
     static CYTHON_INLINE PyObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
         PyObject *exception_table = NULL;
         PyObject *types_module=NULL, *code_type=NULL, *result=NULL;
-        PyObject *version_info; // borrowed
+        #if __PYX_LIMITED_VERSION_HEX < 0x030B0000
+        PyObject *version_info;
         PyObject *py_minor_version = NULL;
+        #endif
         long minor_version = 0;
         PyObject *type, *value, *traceback;
         PyErr_Fetch(&type, &value, &traceback);
         #if __PYX_LIMITED_VERSION_HEX >= 0x030B0000
-        minor_version = 11; // we don't yet need to distinguish between versions > 11
+        minor_version = 11;
         #else
         if (!(version_info = PySys_GetObject("version_info"))) goto end;
         if (!(py_minor_version = PySequence_GetItem(version_info, 1))) goto end;
         minor_version = PyLong_AsLong(py_minor_version);
+        Py_DECREF(py_minor_version);
         if (minor_version == -1 && PyErr_Occurred()) goto end;
         #endif
         if (!(types_module = PyImport_ImportModule("types"))) goto end;
         if (!(code_type = PyObject_GetAttrString(types_module, "CodeType"))) goto end;
         if (minor_version <= 7) {
             (void)p;
             result = PyObject_CallFunction(code_type, "iiiiiOOOOOOiOO", a, k, l, s, f, code,
@@ -616,15 +649,14 @@
             result = PyObject_CallFunction(code_type, "iiiiiiOOOOOOOiOO", a,p, k, l, s, f, code,
                           c, n, v, fn, name, name, fline, lnos, exception_table, fv, cell);
         }
     end:
         Py_XDECREF(code_type);
         Py_XDECREF(exception_table);
         Py_XDECREF(types_module);
-        Py_XDECREF(py_minor_version);
         if (type) {
             PyErr_Restore(type, value, traceback);
         }
         return result;
     }
     #ifndef CO_OPTIMIZED
     #define CO_OPTIMIZED 0x0001
@@ -649,15 +681,15 @@
     #endif
 #elif PY_VERSION_HEX >= 0x030B0000
   static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
     PyCodeObject *result;
-    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);  // we don't have access to __pyx_empty_bytes here
+    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);
     if (!empty_bytes) return NULL;
     result =
       #if PY_VERSION_HEX >= 0x030C0000
         PyUnstable_Code_NewWithPosOnlyArgs
       #else
         PyCode_NewWithPosOnlyArgs
       #endif
@@ -735,16 +767,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -760,14 +797,39 @@
                                             size_t nargsf, PyObject *kwnames);
   #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  ((size_t)1 << (8 * sizeof(size_t) - 1))
   #define __Pyx_PyVectorcall_NARGS(n)  ((Py_ssize_t)(((size_t)(n)) & ~__Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET))
 #else
   #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  0
   #define __Pyx_PyVectorcall_NARGS(n)  ((Py_ssize_t)(n))
 #endif
+#if PY_MAJOR_VERSION >= 0x030900B1
+#define __Pyx_PyCFunction_CheckExact(func)  PyCFunction_CheckExact(func)
+#else
+#define __Pyx_PyCFunction_CheckExact(func)  PyCFunction_Check(func)
+#endif
+#define __Pyx_CyOrPyCFunction_Check(func)  PyCFunction_Check(func)
+#if CYTHON_COMPILING_IN_CPYTHON
+#define __Pyx_CyOrPyCFunction_GET_FUNCTION(func)  (((PyCFunctionObject*)(func))->m_ml->ml_meth)
+#elif !CYTHON_COMPILING_IN_LIMITED_API
+#define __Pyx_CyOrPyCFunction_GET_FUNCTION(func)  PyCFunction_GET_FUNCTION(func)
+#endif
+#if CYTHON_COMPILING_IN_CPYTHON
+#define __Pyx_CyOrPyCFunction_GET_FLAGS(func)  (((PyCFunctionObject*)(func))->m_ml->ml_flags)
+static CYTHON_INLINE PyObject* __Pyx_CyOrPyCFunction_GET_SELF(PyObject *func) {
+    return (__Pyx_CyOrPyCFunction_GET_FLAGS(func) & METH_STATIC) ? NULL : ((PyCFunctionObject*)func)->m_self;
+}
+#endif
+static CYTHON_INLINE int __Pyx__IsSameCFunction(PyObject *func, void *cfunc) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+    return PyCFunction_Check(func) && PyCFunction_GetFunction(func) == (PyCFunction) cfunc;
+#else
+    return PyCFunction_Check(func) && PyCFunction_GET_FUNCTION(func) == (PyCFunction) cfunc;
+#endif
+}
+#define __Pyx_IsSameCFunction(func, cfunc)   __Pyx__IsSameCFunction(func, cfunc)
 #if __PYX_LIMITED_VERSION_HEX < 0x030900B1
   #define __Pyx_PyType_FromModuleAndSpec(m, s, b)  ((void)m, PyType_FromSpecWithBases(s, b))
   typedef PyObject *(*__Pyx_PyCMethod)(PyObject *, PyTypeObject *, PyObject *const *, size_t, PyObject *);
 #else
   #define __Pyx_PyType_FromModuleAndSpec(m, s, b)  PyType_FromModuleAndSpec(m, s, b)
   #define __Pyx_PyCMethod  PyCMethod
 #endif
@@ -786,14 +848,16 @@
   #define __Pyx_PyCode_HasFreeVars(co)  (PyCode_GetNumFree(co) > 0)
   #define __Pyx_PyFrame_SetLineNumber(frame, lineno)  (frame)->f_lineno = (lineno)
 #endif
 #if CYTHON_COMPILING_IN_LIMITED_API
   #define __Pyx_PyThreadState_Current PyThreadState_Get()
 #elif !CYTHON_FAST_THREAD_STATE
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
+#elif PY_VERSION_HEX >= 0x030d00A1
+  #define __Pyx_PyThreadState_Current PyThreadState_GetUnchecked()
 #elif PY_VERSION_HEX >= 0x03060000
   #define __Pyx_PyThreadState_Current _PyThreadState_UncheckedGet()
 #elif PY_VERSION_HEX >= 0x03000000
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
 #else
   #define __Pyx_PyThreadState_Current _PyThreadState_Current
 #endif
@@ -861,27 +925,27 @@
     #else
         static CYTHON_INLINE int PyGILState_Check(void) {
             PyThreadState * tstate = _PyThreadState_Current;
             return tstate && (tstate == PyGILState_GetThisThreadState());
         }
     #endif
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON || defined(_PyDict_NewPresized)
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030d0000 || defined(_PyDict_NewPresized)
 #define __Pyx_PyDict_NewPresized(n)  ((n <= 8) ? PyDict_New() : _PyDict_NewPresized(n))
 #else
 #define __Pyx_PyDict_NewPresized(n)  PyDict_New()
 #endif
 #if PY_MAJOR_VERSION >= 3 || CYTHON_FUTURE_DIVISION
   #define __Pyx_PyNumber_Divide(x,y)         PyNumber_TrueDivide(x,y)
   #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceTrueDivide(x,y)
 #else
   #define __Pyx_PyNumber_Divide(x,y)         PyNumber_Divide(x,y)
   #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceDivide(x,y)
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX > 0x030600B4 && CYTHON_USE_UNICODE_INTERNALS
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX > 0x030600B4 && PY_VERSION_HEX < 0x030d0000 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStrWithError(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 static CYTHON_INLINE PyObject * __Pyx_PyDict_GetItemStr(PyObject *dict, PyObject *name) {
     PyObject *res = __Pyx_PyDict_GetItemStrWithError(dict, name);
     if (res == NULL) PyErr_Clear();
     return res;
 }
 #elif PY_MAJOR_VERSION >= 3 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07020000)
@@ -917,15 +981,15 @@
 #if CYTHON_COMPILING_IN_LIMITED_API
   #define __Pyx_SetItemOnTypeDict(tp, k, v) PyObject_GenericSetAttr((PyObject*)tp, k, v)
 #else
   #define __Pyx_SetItemOnTypeDict(tp, k, v) PyDict_SetItem(tp->tp_dict, k, v)
 #endif
 #if CYTHON_USE_TYPE_SPECS && PY_VERSION_HEX >= 0x03080000
 #define __Pyx_PyHeapTypeObject_GC_Del(obj)  {\
-    PyTypeObject *type = Py_TYPE(obj);\
+    PyTypeObject *type = Py_TYPE((PyObject*)obj);\
     assert(__Pyx_PyType_HasFeature(type, Py_TPFLAGS_HEAPTYPE));\
     PyObject_GC_Del(obj);\
     Py_DECREF(type);\
 }
 #else
 #define __Pyx_PyHeapTypeObject_GC_Del(obj)  PyObject_GC_Del(obj)
 #endif
@@ -1061,14 +1125,23 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
+  #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
+#else
+  static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
+      PyObject *module = PyImport_AddModule(name);
+      Py_XINCREF(module);
+      return module;
+  }
+#endif
 #if PY_MAJOR_VERSION >= 3
   #define PyIntObject                  PyLongObject
   #define PyInt_Type                   PyLong_Type
   #define PyInt_Check(op)              PyLong_Check(op)
   #define PyInt_CheckExact(op)         PyLong_CheckExact(op)
   #define __Pyx_Py3Int_Check(op)       PyLong_Check(op)
   #define __Pyx_Py3Int_CheckExact(op)  PyLong_CheckExact(op)
@@ -1139,15 +1212,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1215,17 +1288,18 @@
 #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define __Pyx_sst_abs(value) llabs(value)
 #elif defined (__GNUC__)
     #define __Pyx_sst_abs(value) __builtin_llabs(value)
 #else
     #define __Pyx_sst_abs(value) ((value<0) ? -value : value)
 #endif
+static CYTHON_INLINE Py_ssize_t __Pyx_ssize_strlen(const char *s);
 static CYTHON_INLINE const char* __Pyx_PyObject_AsString(PyObject*);
 static CYTHON_INLINE const char* __Pyx_PyObject_AsStringAndSize(PyObject*, Py_ssize_t* length);
-#define __Pyx_PyByteArray_FromString(s) PyByteArray_FromStringAndSize((const char*)s, strlen((const char*)s))
+static CYTHON_INLINE PyObject* __Pyx_PyByteArray_FromString(const char*);
 #define __Pyx_PyByteArray_FromStringAndSize(s, l) PyByteArray_FromStringAndSize((const char*)s, l)
 #define __Pyx_PyBytes_FromString        PyBytes_FromString
 #define __Pyx_PyBytes_FromStringAndSize PyBytes_FromStringAndSize
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_FromString(const char*);
 #if PY_MAJOR_VERSION < 3
     #define __Pyx_PyStr_FromString        __Pyx_PyBytes_FromString
     #define __Pyx_PyStr_FromStringAndSize __Pyx_PyBytes_FromStringAndSize
@@ -1245,32 +1319,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -1312,15 +1369,15 @@
     #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue((PyLongObject*) x)
   #else
     #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
     #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
   #endif
   typedef Py_ssize_t  __Pyx_compact_pylong;
   typedef size_t  __Pyx_compact_upylong;
-  #else  // Py < 3.12
+  #else
   #define __Pyx_PyLong_IsNeg(x)  (Py_SIZE(x) < 0)
   #define __Pyx_PyLong_IsNonNeg(x)  (Py_SIZE(x) >= 0)
   #define __Pyx_PyLong_IsZero(x)  (Py_SIZE(x) == 0)
   #define __Pyx_PyLong_IsPos(x)  (Py_SIZE(x) > 0)
   #define __Pyx_PyLong_CompactValueUnsigned(x)  ((Py_SIZE(x) == 0) ? 0 : __Pyx_PyLong_Digits(x)[0])
   #define __Pyx_PyLong_DigitCount(x)  __Pyx_sst_abs(Py_SIZE(x))
   #define __Pyx_PyLong_SignedDigitCount(x)  Py_SIZE(x)
@@ -1333,14 +1390,15 @@
   #if PY_VERSION_HEX >= 0x030C00A5
   #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->long_value.ob_digit)
   #else
   #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->ob_digit)
   #endif
 #endif
 #if PY_MAJOR_VERSION < 3 && __PYX_DEFAULT_STRING_ENCODING_IS_ASCII
+#include <string.h>
 static int __Pyx_sys_getdefaultencoding_not_ascii;
 static int __Pyx_init_sys_getdefaultencoding_params(void) {
     PyObject* sys;
     PyObject* default_encoding = NULL;
     PyObject* ascii_chars_u = NULL;
     PyObject* ascii_chars_b = NULL;
     const char* default_encoding_c;
@@ -1383,14 +1441,15 @@
 }
 #endif
 #if __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT && PY_MAJOR_VERSION >= 3
 #define __Pyx_PyUnicode_FromStringAndSize(c_str, size) PyUnicode_DecodeUTF8(c_str, size, NULL)
 #else
 #define __Pyx_PyUnicode_FromStringAndSize(c_str, size) PyUnicode_Decode(c_str, size, __PYX_DEFAULT_STRING_ENCODING, NULL)
 #if __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT
+#include <string.h>
 static char* __PYX_DEFAULT_STRING_ENCODING;
 static int __Pyx_init_sys_getdefaultencoding_params(void) {
     PyObject* sys;
     PyObject* default_encoding = NULL;
     char* default_encoding_c;
     sys = PyImport_ImportModule("sys");
     if (!sys) goto bad;
@@ -1433,14 +1492,19 @@
 /* #### Code section: filename_table ### */
 
 static const char *__pyx_f[] = {
   "cgranges/python/cgranges.pyx",
   "<stringsource>",
 };
 /* #### Code section: utility_code_proto_before_types ### */
+/* ForceInitThreads.proto */
+#ifndef __PYX_FORCE_INIT_THREADS
+  #define __PYX_FORCE_INIT_THREADS 0
+#endif
+
 /* #### Code section: numeric_typedefs ### */
 /* #### Code section: complex_type_declarations ### */
 /* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
 struct __pyx_obj_8cgranges_cgranges;
 struct __pyx_obj_8cgranges___pyx_scope_struct__overlap;
@@ -1650,29 +1714,34 @@
 #else
     #define __Pyx_Arg_VARARGS(args, i) PyTuple_GetItem(args, i)
 #endif
 #if CYTHON_AVOID_BORROWED_REFS
     #define __Pyx_Arg_NewRef_VARARGS(arg) __Pyx_NewRef(arg)
     #define __Pyx_Arg_XDECREF_VARARGS(arg) Py_XDECREF(arg)
 #else
-    #define __Pyx_Arg_NewRef_VARARGS(arg) arg // no-op
-    #define __Pyx_Arg_XDECREF_VARARGS(arg) // no-op - arg is borrowed
+    #define __Pyx_Arg_NewRef_VARARGS(arg) arg
+    #define __Pyx_Arg_XDECREF_VARARGS(arg)
 #endif
 #define __Pyx_NumKwargs_VARARGS(kwds) PyDict_Size(kwds)
 #define __Pyx_KwValues_VARARGS(args, nargs) NULL
 #define __Pyx_GetKwValue_VARARGS(kw, kwvalues, s) __Pyx_PyDict_GetItemStrWithError(kw, s)
 #define __Pyx_KwargsAsDict_VARARGS(kw, kwvalues) PyDict_Copy(kw)
 #if CYTHON_METH_FASTCALL
     #define __Pyx_Arg_FASTCALL(args, i) args[i]
     #define __Pyx_NumKwargs_FASTCALL(kwds) PyTuple_GET_SIZE(kwds)
     #define __Pyx_KwValues_FASTCALL(args, nargs) ((args) + (nargs))
     static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s);
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
+    CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues);
+  #else
     #define __Pyx_KwargsAsDict_FASTCALL(kw, kwvalues) _PyStack_AsDict(kwvalues, kw)
-    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg // no-op, __Pyx_Arg_FASTCALL is direct and this needs
-    #define __Pyx_Arg_XDECREF_FASTCALL(arg)  // no-op - arg was returned from array
+  #endif
+    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg  /* no-op, __Pyx_Arg_FASTCALL is direct and this needs
+                                                   to have the same reference counting */
+    #define __Pyx_Arg_XDECREF_FASTCALL(arg)
 #else
     #define __Pyx_Arg_FASTCALL __Pyx_Arg_VARARGS
     #define __Pyx_NumKwargs_FASTCALL __Pyx_NumKwargs_VARARGS
     #define __Pyx_KwValues_FASTCALL __Pyx_KwValues_VARARGS
     #define __Pyx_GetKwValue_FASTCALL __Pyx_GetKwValue_VARARGS
     #define __Pyx_KwargsAsDict_FASTCALL __Pyx_KwargsAsDict_VARARGS
     #define __Pyx_Arg_NewRef_FASTCALL(arg) __Pyx_Arg_NewRef_VARARGS(arg)
@@ -1900,25 +1969,29 @@
     PyObject *func_code;
     PyObject *func_closure;
 #if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
     PyObject *func_classobj;
 #endif
     void *defaults;
     int defaults_pyobjects;
-    size_t defaults_size;  // used by FusedFunction for copying defaults
+    size_t defaults_size;
     int flags;
     PyObject *defaults_tuple;
     PyObject *defaults_kwdict;
     PyObject *(*defaults_getter)(PyObject *);
     PyObject *func_annotations;
     PyObject *func_is_coroutine;
 } __pyx_CyFunctionObject;
+#undef __Pyx_CyOrPyCFunction_Check
 #define __Pyx_CyFunction_Check(obj)  __Pyx_TypeCheck(obj, __pyx_CyFunctionType)
-#define __Pyx_IsCyOrPyCFunction(obj)  __Pyx_TypeCheck2(obj, __pyx_CyFunctionType, &PyCFunction_Type)
+#define __Pyx_CyOrPyCFunction_Check(obj)  __Pyx_TypeCheck2(obj, __pyx_CyFunctionType, &PyCFunction_Type)
 #define __Pyx_CyFunction_CheckExact(obj)  __Pyx_IS_TYPE(obj, __pyx_CyFunctionType)
+static CYTHON_INLINE int __Pyx__IsSameCyOrCFunction(PyObject *func, void *cfunc);
+#undef __Pyx_IsSameCFunction
+#define __Pyx_IsSameCFunction(func, cfunc)   __Pyx__IsSameCyOrCFunction(func, cfunc)
 static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject* op, PyMethodDef *ml,
                                       int flags, PyObject* qualname,
                                       PyObject *closure,
                                       PyObject *module, PyObject *globals,
                                       PyObject* code);
 static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj);
 static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *m,
@@ -2163,15 +2236,16 @@
 #define __Pyx_Generator_CheckExact(obj) __Pyx_IS_TYPE(obj, __pyx_GeneratorType)
 #define __Pyx_Generator_New(body, code, closure, name, qualname, module_name)\
     __Pyx__Coroutine_New(__pyx_GeneratorType, body, code, closure, name, qualname, module_name)
 static PyObject *__Pyx_Generator_Next(PyObject *self);
 static int __pyx_Generator_init(PyObject *module);
 
 /* CheckBinaryVersion.proto */
-static int __Pyx_check_binary_version(void);
+static unsigned long __Pyx_get_runtime_version(void);
+static int __Pyx_check_binary_version(unsigned long ct_version, unsigned long rt_version, int allow_newer);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 /* #### Code section: module_declarations ### */
 
 /* Module declarations from "libc.stdint" */
@@ -2685,49 +2759,36 @@
  */
 
 /* Python wrapper */
 static int __pyx_pw_8cgranges_8cgranges_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_pw_8cgranges_8cgranges_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__ (wrapper)", 0);
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 25, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return -1;
   #endif
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 0, 0, __pyx_nargs); return -1;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_VARARGS(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__cinit__", 0))) return -1;
-  goto __pyx_L4_argument_unpacking_done;
-  goto __pyx_L3_error;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("cgranges.cgranges.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return -1;
-  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8cgranges_8cgranges___cinit__(((struct __pyx_obj_8cgranges_cgranges *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static int __pyx_pf_8cgranges_8cgranges___cinit__(struct __pyx_obj_8cgranges_cgranges *__pyx_v_self) {
   CYTHON_UNUSED long __pyx_v_indexed;
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__cinit__", 0);
 
   /* "cgranges.pyx":26
  * 
  * 	def __cinit__(self):
  * 		self.cr = cr_init()             # <<<<<<<<<<<<<<
  * 		indexed = 0
  * 
@@ -2749,15 +2810,14 @@
  * 	def __cinit__(self):             # <<<<<<<<<<<<<<
  * 		self.cr = cr_init()
  * 		indexed = 0
  */
 
   /* function exit code */
   __pyx_r = 0;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cgranges.pyx":29
  * 		indexed = 0
  * 
  * 	def __dealloc__(self):             # <<<<<<<<<<<<<<
@@ -2775,16 +2835,14 @@
   __pyx_pf_8cgranges_8cgranges_2__dealloc__(((struct __pyx_obj_8cgranges_cgranges *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_pf_8cgranges_8cgranges_2__dealloc__(struct __pyx_obj_8cgranges_cgranges *__pyx_v_self) {
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__dealloc__", 0);
 
   /* "cgranges.pyx":30
  * 
  * 	def __dealloc__(self):
  * 		cr_destroy(self.cr)             # <<<<<<<<<<<<<<
  * 
  * 	def add(self, ctg, st, en, label=-1):
@@ -2796,15 +2854,14 @@
  * 
  * 	def __dealloc__(self):             # <<<<<<<<<<<<<<
  * 		cr_destroy(self.cr)
  * 
  */
 
   /* function exit code */
-  __Pyx_RefNannyFinishContext();
 }
 
 /* "cgranges.pyx":32
  * 		cr_destroy(self.cr)
  * 
  * 	def add(self, ctg, st, en, label=-1):             # <<<<<<<<<<<<<<
  * 		if not self.indexed:
@@ -2842,16 +2899,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("add (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 32, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_ctg,&__pyx_n_s_st,&__pyx_n_s_en,&__pyx_n_s_label,0};
     values[3] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)__pyx_int_neg_1));
     if (__pyx_kwds) {
@@ -2921,18 +2977,19 @@
       }
     }
     __pyx_v_ctg = values[0];
     __pyx_v_st = values[1];
     __pyx_v_en = values[2];
     __pyx_v_label = values[3];
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("add", 0, 3, 4, __pyx_nargs); __PYX_ERR(0, 32, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -2964,15 +3021,15 @@
   char const *__pyx_t_6;
   int32_t __pyx_t_7;
   int32_t __pyx_t_8;
   int32_t __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("add", 0);
+  __Pyx_RefNannySetupContext("add", 1);
 
   /* "cgranges.pyx":33
  * 
  * 	def add(self, ctg, st, en, label=-1):
  * 		if not self.indexed:             # <<<<<<<<<<<<<<
  * 			cr_add(self.cr, str.encode(ctg), st, en, label)
  * 
@@ -3074,51 +3131,40 @@
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("index (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 36, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("index", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "index", 0))) return NULL;
-  goto __pyx_L4_argument_unpacking_done;
-  goto __pyx_L3_error;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("cgranges.cgranges.index", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8cgranges_8cgranges_6index(((struct __pyx_obj_8cgranges_cgranges *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_8cgranges_8cgranges_6index(struct __pyx_obj_8cgranges_cgranges *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
-  __Pyx_RefNannySetupContext("index", 0);
+  __Pyx_RefNannySetupContext("index", 1);
 
   /* "cgranges.pyx":37
  * 
  * 	def index(self):
  * 		if not self.indexed:             # <<<<<<<<<<<<<<
  * 			cr_index(self.cr)
  * 			self.indexed = 1
@@ -3207,16 +3253,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("overlap (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 41, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_ctg,&__pyx_n_s_st,&__pyx_n_s_en,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -3271,18 +3316,19 @@
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
     }
     __pyx_v_ctg = values[0];
     __pyx_v_st = values[1];
     __pyx_v_en = values[2];
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("overlap", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 41, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -3579,16 +3625,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("coverage (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 51, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_ctg,&__pyx_n_s_st,&__pyx_n_s_en,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -3643,18 +3688,19 @@
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
     }
     __pyx_v_ctg = values[0];
     __pyx_v_st = values[1];
     __pyx_v_en = values[2];
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("coverage", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 51, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -3698,15 +3744,15 @@
   char const *__pyx_t_9;
   int64_t __pyx_t_10;
   int64_t __pyx_t_11;
   int64_t __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("coverage", 0);
+  __Pyx_RefNannySetupContext("coverage", 1);
 
   /* "cgranges.pyx":52
  * 
  * 	def coverage(self, ctg, st, en):
  * 		cdef int64_t *b = NULL             # <<<<<<<<<<<<<<
  * 		cdef int64_t m_b = 0
  * 		cdef int64_t n
@@ -3997,53 +4043,42 @@
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 1, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("__reduce_cython__", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce_cython__", 0))) return NULL;
-  goto __pyx_L4_argument_unpacking_done;
-  goto __pyx_L3_error;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("cgranges.cgranges.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8cgranges_8cgranges_13__reduce_cython__(((struct __pyx_obj_8cgranges_cgranges *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_8cgranges_8cgranges_13__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_8cgranges_cgranges *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__reduce_cython__", 0);
+  __Pyx_RefNannySetupContext("__reduce_cython__", 1);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
@@ -4100,16 +4135,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 3, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_state,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -4136,18 +4170,19 @@
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v___pyx_state = values[0];
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__setstate_cython__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 3, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -4170,15 +4205,15 @@
 
 static PyObject *__pyx_pf_8cgranges_8cgranges_15__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_8cgranges_cgranges *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__setstate_cython__", 0);
+  __Pyx_RefNannySetupContext("__setstate_cython__", 1);
 
   /* "(tree fragment)":4
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"             # <<<<<<<<<<<<<<
  */
   __Pyx_Raise(__pyx_builtin_TypeError, __pyx_kp_s_no_default___reduce___due_to_non, 0, 0);
@@ -4349,24 +4384,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_8cgranges___pyx_scope_struct__overlap *__pyx_freelist_8cgranges___pyx_scope_struct__overlap[8];
 static int __pyx_freecount_8cgranges___pyx_scope_struct__overlap = 0;
+#endif
 
 static PyObject *__pyx_tp_new_8cgranges___pyx_scope_struct__overlap(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_8cgranges___pyx_scope_struct__overlap > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_8cgranges___pyx_scope_struct__overlap)))) {
     o = (PyObject*)__pyx_freelist_8cgranges___pyx_scope_struct__overlap[--__pyx_freecount_8cgranges___pyx_scope_struct__overlap];
     memset(o, 0, sizeof(struct __pyx_obj_8cgranges___pyx_scope_struct__overlap));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -4388,15 +4425,15 @@
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_ctg);
   Py_CLEAR(p->__pyx_v_en);
   Py_CLEAR(p->__pyx_v_self);
   Py_CLEAR(p->__pyx_v_st);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_8cgranges___pyx_scope_struct__overlap < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_8cgranges___pyx_scope_struct__overlap)))) {
     __pyx_freelist_8cgranges___pyx_scope_struct__overlap[__pyx_freecount_8cgranges___pyx_scope_struct__overlap++] = ((struct __pyx_obj_8cgranges___pyx_scope_struct__overlap *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -4998,42 +5035,40 @@
   #if PY_MAJOR_VERSION < 3
   __pyx_m = Py_InitModule4("cgranges", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #elif CYTHON_USE_MODULE_STATE
   __pyx_t_1 = PyModule_Create(&__pyx_moduledef); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   {
     int add_module_result = PyState_AddModule(__pyx_t_1, &__pyx_moduledef);
-    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to cgranges pseudovariable */
+    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to "cgranges" pseudovariable */
     if (unlikely((add_module_result < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
     pystate_addmodule_run = 1;
   }
   #else
   __pyx_m = PyModule_Create(&__pyx_moduledef);
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #endif
   CYTHON_UNUSED_VAR(__pyx_t_1);
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
-  __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_b);
-  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_cython_runtime);
+  __pyx_b = __Pyx_PyImport_AddModuleRef(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_cython_runtime = __Pyx_PyImport_AddModuleRef((const char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if CYTHON_REFNANNY
 __Pyx_RefNanny = __Pyx_RefNannyImportAPI("refnanny");
 if (!__Pyx_RefNanny) {
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
       Py_FatalError("failed to import 'refnanny' module");
 }
 #endif
   __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit_cgranges(void)", 0);
-  if (__Pyx_check_binary_version() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_check_binary_version(__PYX_LIMITED_VERSION_HEX, __Pyx_get_runtime_version(), CYTHON_COMPILING_IN_LIMITED_API) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #ifdef __Pxy_PyFrame_Initialize_Offsets
   __Pxy_PyFrame_Initialize_Offsets();
   #endif
   __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(0, 1, __pyx_L1_error)
   #ifdef __Pyx_CyFunction_USED
@@ -5300,14 +5335,16 @@
         if (unlikely(((PyBaseExceptionObject*) value)->traceback != tb))
         #endif
             PyException_SetTraceback(value, tb);
     }
     tmp_value = tstate->current_exception;
     tstate->current_exception = value;
     Py_XDECREF(tmp_value);
+    Py_XDECREF(type);
+    Py_XDECREF(tb);
 #else
     PyObject *tmp_type, *tmp_value, *tmp_tb;
     tmp_type = tstate->curexc_type;
     tmp_value = tstate->curexc_value;
     tmp_tb = tstate->curexc_traceback;
     tstate->curexc_type = type;
     tstate->curexc_value = value;
@@ -5357,33 +5394,40 @@
         return tp->tp_getattr(obj, PyString_AS_STRING(attr_name));
 #endif
     return PyObject_GetAttr(obj, attr_name);
 }
 #endif
 
 /* PyObjectGetAttrStrNoError */
+#if __PYX_LIMITED_VERSION_HEX < 0x030d00A1
 static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     if (likely(__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
         __Pyx_PyErr_Clear();
 }
+#endif
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name) {
     PyObject *result;
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
+    (void) PyObject_GetOptionalAttr(obj, attr_name, &result);
+    return result;
+#else
 #if CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_TYPE_SLOTS && PY_VERSION_HEX >= 0x030700B1
     PyTypeObject* tp = Py_TYPE(obj);
     if (likely(tp->tp_getattro == PyObject_GenericGetAttr)) {
         return _PyObject_GenericGetAttrWithDict(obj, attr_name, NULL, 1);
     }
 #endif
     result = __Pyx_PyObject_GetAttrStr(obj, attr_name);
     if (unlikely(!result)) {
         __Pyx_PyObject_GetAttrStr_ClearAttributeError();
     }
     return result;
+#endif
 }
 
 /* GetBuiltinName */
 static PyObject *__Pyx_GetBuiltinName(PyObject *name) {
     PyObject* result = __Pyx_PyObject_GetAttrStrNoError(__pyx_b, name);
     if (unlikely(!result) && !PyErr_Occurred()) {
         PyErr_Format(PyExc_NameError,
@@ -5591,21 +5635,39 @@
     {
         if (s == PyTuple_GET_ITEM(kwnames, i)) return kwvalues[i];
     }
     for (i = 0; i < n; i++)
     {
         int eq = __Pyx_PyUnicode_Equals(s, PyTuple_GET_ITEM(kwnames, i), Py_EQ);
         if (unlikely(eq != 0)) {
-            if (unlikely(eq < 0)) return NULL;  // error
+            if (unlikely(eq < 0)) return NULL;
             return kwvalues[i];
         }
     }
-    return NULL;  // not found (no exception set)
+    return NULL;
+}
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
+CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues) {
+    Py_ssize_t i, nkwargs = PyTuple_GET_SIZE(kwnames);
+    PyObject *dict;
+    dict = PyDict_New();
+    if (unlikely(!dict))
+        return NULL;
+    for (i=0; i<nkwargs; i++) {
+        PyObject *key = PyTuple_GET_ITEM(kwnames, i);
+        if (unlikely(PyDict_SetItem(dict, key, kwvalues[i]) < 0))
+            goto bad;
+    }
+    return dict;
+bad:
+    Py_DECREF(dict);
+    return NULL;
 }
 #endif
+#endif
 
 /* RaiseArgTupleInvalid */
 static void __Pyx_RaiseArgtupleInvalid(
     const char* func_name,
     int exact,
     Py_ssize_t num_min,
     Py_ssize_t num_max,
@@ -5764,15 +5826,15 @@
 #endif
         }
         name = first_kw_arg;
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-            Py_INCREF(value); // transfer ownership of value to values
+            Py_INCREF(value);
             Py_DECREF(key);
 #endif
             key = NULL;
             value = NULL;
             continue;
         }
 #if !CYTHON_AVOID_BORROWED_REFS
@@ -5783,15 +5845,15 @@
         #if PY_MAJOR_VERSION < 3
         if (likely(PyString_Check(key))) {
             while (*name) {
                 if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
                         && _PyString_Eq(**name, key)) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL;  // ownership transferred to values
+                    value = NULL;
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -5815,15 +5877,15 @@
                 #endif
                     PyUnicode_Compare(**name, key)
                 );
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL; // ownership transferred to values
+                    value = NULL;
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -5914,17 +5976,23 @@
     PyObject *kwtuple, **k;
     PyObject **d;
     Py_ssize_t nd;
     Py_ssize_t nk;
     PyObject *result;
     assert(kwargs == NULL || PyDict_Check(kwargs));
     nk = kwargs ? PyDict_Size(kwargs) : 0;
+    #if PY_MAJOR_VERSION < 3
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object"))) {
         return NULL;
     }
+    #else
+    if (unlikely(Py_EnterRecursiveCall(" while calling a Python object"))) {
+        return NULL;
+    }
+    #endif
     if (
 #if PY_MAJOR_VERSION >= 3
             co->co_kwonlyargcount == 0 &&
 #endif
             likely(kwargs == NULL || nk == 0) &&
             co->co_flags == (CO_OPTIMIZED | CO_NEWLOCALS | CO_NOFREE)) {
         if (argdefs == NULL && co->co_argcount == nargs) {
@@ -5993,16 +6061,21 @@
 /* PyObjectCall */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
     PyObject *result;
     ternaryfunc call = Py_TYPE(func)->tp_call;
     if (unlikely(!call))
         return PyObject_Call(func, arg, kw);
+    #if PY_MAJOR_VERSION < 3
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
+    #else
+    if (unlikely(Py_EnterRecursiveCall(" while calling a Python object")))
+        return NULL;
+    #endif
     result = (*call)(func, arg, kw);
     Py_LeaveRecursiveCall();
     if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
         PyErr_SetString(
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
@@ -6011,30 +6084,36 @@
 #endif
 
 /* PyObjectCallMethO */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg) {
     PyObject *self, *result;
     PyCFunction cfunc;
-    cfunc = PyCFunction_GET_FUNCTION(func);
-    self = PyCFunction_GET_SELF(func);
+    cfunc = __Pyx_CyOrPyCFunction_GET_FUNCTION(func);
+    self = __Pyx_CyOrPyCFunction_GET_SELF(func);
+    #if PY_MAJOR_VERSION < 3
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
+    #else
+    if (unlikely(Py_EnterRecursiveCall(" while calling a Python object")))
+        return NULL;
+    #endif
     result = cfunc(self, arg);
     Py_LeaveRecursiveCall();
     if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
         PyErr_SetString(
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
     return result;
 }
 #endif
 
 /* PyObjectFastCall */
+#if PY_VERSION_HEX < 0x03090000 || CYTHON_COMPILING_IN_LIMITED_API
 static PyObject* __Pyx_PyObject_FastCall_fallback(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs) {
     PyObject *argstuple;
     PyObject *result = 0;
     size_t i;
     argstuple = PyTuple_New((Py_ssize_t)nargs);
     if (unlikely(!argstuple)) return NULL;
     for (i = 0; i < nargs; i++) {
@@ -6042,36 +6121,25 @@
         if (__Pyx_PyTuple_SET_ITEM(argstuple, (Py_ssize_t)i, args[i]) < 0) goto bad;
     }
     result = __Pyx_PyObject_Call(func, argstuple, kwargs);
   bad:
     Py_DECREF(argstuple);
     return result;
 }
+#endif
 static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t _nargs, PyObject *kwargs) {
     Py_ssize_t nargs = __Pyx_PyVectorcall_NARGS(_nargs);
 #if CYTHON_COMPILING_IN_CPYTHON
     if (nargs == 0 && kwargs == NULL) {
-#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
-        if (__Pyx_IsCyOrPyCFunction(func))
-#else
-        if (PyCFunction_Check(func))
-#endif
-        {
-            if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
-                return __Pyx_PyObject_CallMethO(func, NULL);
-            }
-        }
+        if (__Pyx_CyOrPyCFunction_Check(func) && likely( __Pyx_CyOrPyCFunction_GET_FLAGS(func) & METH_NOARGS))
+            return __Pyx_PyObject_CallMethO(func, NULL);
     }
     else if (nargs == 1 && kwargs == NULL) {
-        if (PyCFunction_Check(func))
-        {
-            if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
-                return __Pyx_PyObject_CallMethO(func, args[0]);
-            }
-        }
+        if (__Pyx_CyOrPyCFunction_Check(func) && likely( __Pyx_CyOrPyCFunction_GET_FLAGS(func) & METH_O))
+            return __Pyx_PyObject_CallMethO(func, args[0]);
     }
 #endif
     #if PY_VERSION_HEX < 0x030800B1
     #if CYTHON_FAST_PYCCALL
     if (PyCFunction_Check(func)) {
         if (kwargs) {
             return _PyCFunction_FastCallDict(func, args, nargs, kwargs);
@@ -6087,33 +6155,39 @@
     #endif
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs);
     }
     #endif
     #endif
-    #if CYTHON_VECTORCALL
-    #if Py_VERSION_HEX < 0x03090000
-    vectorcallfunc f = _PyVectorcall_Function(func);
-    #else
-    vectorcallfunc f = PyVectorcall_Function(func);
-    #endif
-    if (f) {
-        return f(func, args, (size_t)nargs, kwargs);
-    }
-    #elif defined(__Pyx_CyFunction_USED) && CYTHON_BACKPORT_VECTORCALL
-    if (__Pyx_CyFunction_CheckExact(func)) {
-        __pyx_vectorcallfunc f = __Pyx_CyFunction_func_vectorcall(func);
-        if (f) return f(func, args, (size_t)nargs, kwargs);
+    if (kwargs == NULL) {
+        #if CYTHON_VECTORCALL
+        #if PY_VERSION_HEX < 0x03090000
+        vectorcallfunc f = _PyVectorcall_Function(func);
+        #else
+        vectorcallfunc f = PyVectorcall_Function(func);
+        #endif
+        if (f) {
+            return f(func, args, (size_t)nargs, NULL);
+        }
+        #elif defined(__Pyx_CyFunction_USED) && CYTHON_BACKPORT_VECTORCALL
+        if (__Pyx_CyFunction_CheckExact(func)) {
+            __pyx_vectorcallfunc f = __Pyx_CyFunction_func_vectorcall(func);
+            if (f) return f(func, args, (size_t)nargs, NULL);
+        }
+        #endif
     }
-    #endif
     if (nargs == 0) {
         return __Pyx_PyObject_Call(func, __pyx_empty_tuple, kwargs);
     }
+    #if PY_VERSION_HEX >= 0x03090000 && !CYTHON_COMPILING_IN_LIMITED_API
+    return PyObject_VectorcallDict(func, args, (size_t)nargs, kwargs);
+    #else
     return __Pyx_PyObject_FastCall_fallback(func, args, (size_t)nargs, kwargs);
+    #endif
 }
 
 /* GetException */
 #if CYTHON_FAST_THREAD_STATE
 static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb)
 #else
 static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb)
@@ -6469,16 +6543,16 @@
 #endif
     return 0;
 }
 #endif
 
 /* PyObjectCallNoArg */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
-    PyObject *arg = NULL;
-    return __Pyx_PyObject_FastCall(func, (&arg)+1, 0 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
+    PyObject *arg[2] = {NULL, NULL};
+    return __Pyx_PyObject_FastCall(func, arg + 1, 0 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
 }
 
 /* PyObjectCallOneArg */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
     PyObject *args[2] = {NULL, arg};
     return __Pyx_PyObject_FastCall(func, args+1, 1 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
 }
@@ -6641,46 +6715,46 @@
                 "base class '" __Pyx_FMT_TYPENAME "' is not a heap type", b_name);
             __Pyx_DECREF_TypeName(b_name);
 #if CYTHON_AVOID_BORROWED_REFS
             Py_DECREF(b0);
 #endif
             return -1;
         }
-#if !CYTHON_USE_TYPE_SLOTS
-        if (dictoffset == 0) {
-            PyErr_Format(PyExc_TypeError,
-                "extension type '%s.200s': "
-                "unable to validate whether bases have a __dict__ "
-                "when CYTHON_USE_TYPE_SLOTS is off "
-                "(likely because you are building in the limited API). "
-                "Therefore, all extension types with multiple bases "
-                "must add 'cdef dict __dict__' in this compilation mode",
-                type_name);
-#if CYTHON_AVOID_BORROWED_REFS
-            Py_DECREF(b0);
-#endif
-            return -1;
-        }
-#else
-        if (dictoffset == 0 && b->tp_dictoffset)
+        if (dictoffset == 0)
         {
-            __Pyx_TypeName b_name = __Pyx_PyType_GetName(b);
-            PyErr_Format(PyExc_TypeError,
-                "extension type '%.200s' has no __dict__ slot, "
-                "but base type '" __Pyx_FMT_TYPENAME "' has: "
-                "either add 'cdef dict __dict__' to the extension type "
-                "or add '__slots__ = [...]' to the base type",
-                type_name, b_name);
-            __Pyx_DECREF_TypeName(b_name);
+            Py_ssize_t b_dictoffset = 0;
+#if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
+            b_dictoffset = b->tp_dictoffset;
+#else
+            PyObject *py_b_dictoffset = PyObject_GetAttrString((PyObject*)b, "__dictoffset__");
+            if (!py_b_dictoffset) goto dictoffset_return;
+            b_dictoffset = PyLong_AsSsize_t(py_b_dictoffset);
+            Py_DECREF(py_b_dictoffset);
+            if (b_dictoffset == -1 && PyErr_Occurred()) goto dictoffset_return;
+#endif
+            if (b_dictoffset) {
+                {
+                    __Pyx_TypeName b_name = __Pyx_PyType_GetName(b);
+                    PyErr_Format(PyExc_TypeError,
+                        "extension type '%.200s' has no __dict__ slot, "
+                        "but base type '" __Pyx_FMT_TYPENAME "' has: "
+                        "either add 'cdef dict __dict__' to the extension type "
+                        "or add '__slots__ = [...]' to the base type",
+                        type_name, b_name);
+                    __Pyx_DECREF_TypeName(b_name);
+                }
+#if !(CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY)
+              dictoffset_return:
+#endif
 #if CYTHON_AVOID_BORROWED_REFS
-            Py_DECREF(b0);
+                Py_DECREF(b0);
 #endif
-            return -1;
+                return -1;
+            }
         }
-#endif
 #if CYTHON_AVOID_BORROWED_REFS
         Py_DECREF(b0);
 #endif
     }
     return 0;
 }
 #endif
@@ -6928,18 +7002,15 @@
     Py_XDECREF(setstate_cython);
     return ret;
 }
 #endif
 
 /* FetchSharedCythonModule */
 static PyObject *__Pyx_FetchSharedCythonABIModule(void) {
-    PyObject *abi_module = PyImport_AddModule((char*) __PYX_ABI_MODULE_NAME);
-    if (unlikely(!abi_module)) return NULL;
-    Py_INCREF(abi_module);
-    return abi_module;
+    return __Pyx_PyImport_AddModuleRef((char*) __PYX_ABI_MODULE_NAME);
 }
 
 /* FetchCommonType */
 static int __Pyx_VerifyCachedType(PyObject *cached_type,
                                const char *name,
                                Py_ssize_t basicsize,
                                Py_ssize_t expected_basicsize) {
@@ -7092,14 +7163,28 @@
         return vc(func, args, nargs, NULL);
     }
     return __Pyx_PyVectorcall_FastCallDict_kw(func, vc, args, nargs, kw);
 }
 #endif
 
 /* CythonFunctionShared */
+#if CYTHON_COMPILING_IN_LIMITED_API
+static CYTHON_INLINE int __Pyx__IsSameCyOrCFunction(PyObject *func, void *cfunc) {
+    if (__Pyx_CyFunction_Check(func)) {
+        return PyCFunction_GetFunction(((__pyx_CyFunctionObject*)func)->func) == (PyCFunction) cfunc;
+    } else if (PyCFunction_Check(func)) {
+        return PyCFunction_GetFunction(func) == (PyCFunction) cfunc;
+    }
+    return 0;
+}
+#else
+static CYTHON_INLINE int __Pyx__IsSameCyOrCFunction(PyObject *func, void *cfunc) {
+    return __Pyx_CyOrPyCFunction_Check(func) && __Pyx_CyOrPyCFunction_GET_FUNCTION(func) == (PyCFunction) cfunc;
+}
+#endif
 static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj) {
 #if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
     __Pyx_Py_XDECREF_SET(
         __Pyx_CyFunction_GetClassObj(f),
             ((classobj) ? __Pyx_NewRef(classobj) : NULL));
 #else
     __Pyx_Py_XDECREF_SET(
@@ -7901,15 +7986,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
@@ -8266,16 +8351,16 @@
     replace = PyObject_GetAttrString(code, "replace");
     if (likely(replace)) {
         PyObject *result;
         result = PyObject_Call(replace, __pyx_empty_tuple, scratch_dict);
         Py_DECREF(replace);
         return result;
     }
-    #if __PYX_LIMITED_VERSION_HEX < 0x030780000
     PyErr_Clear();
+    #if __PYX_LIMITED_VERSION_HEX < 0x030780000
     {
         PyObject *compiled = NULL, *result = NULL;
         if (unlikely(PyDict_SetItemString(scratch_dict, "code", code))) return NULL;
         if (unlikely(PyDict_SetItemString(scratch_dict, "type", (PyObject*)(&PyType_Type)))) return NULL;
         compiled = Py_CompileString(
             "out = type(code)(\n"
             "  code.co_argcount, code.co_kwonlyargcount, code.co_nlocals, code.co_stacksize,\n"
@@ -8287,14 +8372,16 @@
         Py_DECREF(compiled);
         if (!result) PyErr_Print();
         Py_DECREF(result);
         result = PyDict_GetItemString(scratch_dict, "out");
         if (result) Py_INCREF(result);
         return result;
     }
+    #else
+    return NULL;
     #endif
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyObject *code_object = NULL, *py_py_line = NULL, *py_funcname = NULL, *dict = NULL;
     PyObject *replace = NULL, *getframe = NULL, *frame = NULL;
     PyObject *exc_type, *exc_value, *exc_traceback;
@@ -8384,15 +8471,15 @@
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
     #else
     py_code = PyCode_NewEmpty(filename, funcname, py_line);
     #endif
-    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
+    Py_XDECREF(py_funcname);
     return py_code;
 bad:
     Py_XDECREF(py_funcname);
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_srcfile);
     #endif
     return NULL;
@@ -8625,15 +8712,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -8761,38 +8848,40 @@
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-#if !CYTHON_COMPILING_IN_LIMITED_API
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
         return _PyLong_FromByteArray(bytes, sizeof(int64_t),
                                      little, !is_unsigned);
 #else
         PyObject *from_bytes, *result = NULL;
         PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
-        from_bytes = PyObject_GetAttrString((PyObject*)&PyInt_Type, "from_bytes");
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
         if (!from_bytes) return NULL;
         py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(int64_t));
         if (!py_bytes) goto limited_bad;
         order_str = PyUnicode_FromString(little ? "little" : "big");
         if (!order_str) goto limited_bad;
         arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
         if (!arg_tuple) goto limited_bad;
-        kwds = PyDict_New();
-        if (!kwds) goto limited_bad;
-        if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(!is_unsigned ? Py_True : Py_False))) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
         result = PyObject_Call(from_bytes, arg_tuple, kwds);
         limited_bad:
-        Py_XDECREF(from_bytes);
-        Py_XDECREF(py_bytes);
-        Py_XDECREF(order_str);
-        Py_XDECREF(arg_tuple);
         Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
         return result;
 #endif
     }
 }
 
 /* CIntFromPy */
 static CYTHON_INLINE int64_t __Pyx_PyInt_As_int64_t(PyObject *x) {
@@ -8960,15 +9049,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -9096,38 +9185,40 @@
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-#if !CYTHON_COMPILING_IN_LIMITED_API
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
         return _PyLong_FromByteArray(bytes, sizeof(int32_t),
                                      little, !is_unsigned);
 #else
         PyObject *from_bytes, *result = NULL;
         PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
-        from_bytes = PyObject_GetAttrString((PyObject*)&PyInt_Type, "from_bytes");
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
         if (!from_bytes) return NULL;
         py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(int32_t));
         if (!py_bytes) goto limited_bad;
         order_str = PyUnicode_FromString(little ? "little" : "big");
         if (!order_str) goto limited_bad;
         arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
         if (!arg_tuple) goto limited_bad;
-        kwds = PyDict_New();
-        if (!kwds) goto limited_bad;
-        if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(!is_unsigned ? Py_True : Py_False))) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
         result = PyObject_Call(from_bytes, arg_tuple, kwds);
         limited_bad:
-        Py_XDECREF(from_bytes);
-        Py_XDECREF(py_bytes);
-        Py_XDECREF(order_str);
-        Py_XDECREF(arg_tuple);
         Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
         return result;
 #endif
     }
 }
 
 /* FormatTypeName */
 #if CYTHON_COMPILING_IN_LIMITED_API
@@ -9174,38 +9265,40 @@
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-#if !CYTHON_COMPILING_IN_LIMITED_API
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
         return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
 #else
         PyObject *from_bytes, *result = NULL;
         PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
-        from_bytes = PyObject_GetAttrString((PyObject*)&PyInt_Type, "from_bytes");
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
         if (!from_bytes) return NULL;
         py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(long));
         if (!py_bytes) goto limited_bad;
         order_str = PyUnicode_FromString(little ? "little" : "big");
         if (!order_str) goto limited_bad;
         arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
         if (!arg_tuple) goto limited_bad;
-        kwds = PyDict_New();
-        if (!kwds) goto limited_bad;
-        if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(!is_unsigned ? Py_True : Py_False))) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
         result = PyObject_Call(from_bytes, arg_tuple, kwds);
         limited_bad:
-        Py_XDECREF(from_bytes);
-        Py_XDECREF(py_bytes);
-        Py_XDECREF(order_str);
-        Py_XDECREF(arg_tuple);
         Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
         return result;
 #endif
     }
 }
 
 /* CIntFromPy */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
@@ -9373,15 +9466,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -9646,15 +9739,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -10008,29 +10101,39 @@
 /* PyObjectCall2Args */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2) {
     PyObject *args[3] = {NULL, arg1, arg2};
     return __Pyx_PyObject_FastCall(function, args+1, 2 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
 }
 
 /* PyObjectCallMethod1 */
+#if !(CYTHON_VECTORCALL && __PYX_LIMITED_VERSION_HEX >= 0x030C00A2)
 static PyObject* __Pyx__PyObject_CallMethod1(PyObject* method, PyObject* arg) {
     PyObject *result = __Pyx_PyObject_CallOneArg(method, arg);
     Py_DECREF(method);
     return result;
 }
+#endif
 static PyObject* __Pyx_PyObject_CallMethod1(PyObject* obj, PyObject* method_name, PyObject* arg) {
+#if CYTHON_VECTORCALL && __PYX_LIMITED_VERSION_HEX >= 0x030C00A2
+    PyObject *args[2] = {obj, arg};
+    (void) __Pyx_PyObject_GetMethod;
+    (void) __Pyx_PyObject_CallOneArg;
+    (void) __Pyx_PyObject_Call2Args;
+    return PyObject_VectorcallMethod(method_name, args, 2 | PY_VECTORCALL_ARGUMENTS_OFFSET, NULL);
+#else
     PyObject *method = NULL, *result;
     int is_method = __Pyx_PyObject_GetMethod(obj, method_name, &method);
     if (likely(is_method)) {
         result = __Pyx_PyObject_Call2Args(method, obj, arg);
         Py_DECREF(method);
         return result;
     }
     if (unlikely(!method)) return NULL;
     return __Pyx__PyObject_CallMethod1(method, arg);
+#endif
 }
 
 /* CoroutineBase */
 #include <frameobject.h>
 #if PY_VERSION_HEX >= 0x030b00a6
   #ifndef Py_BUILD_CORE
     #define Py_BUILD_CORE 1
@@ -10310,17 +10413,30 @@
             assert(result == Py_None);
             PyErr_SetNone(PyExc_StopAsyncIteration);
         }
         else if (result == Py_None) {
             PyErr_SetNone(PyExc_StopIteration);
         }
         else {
+#if PY_VERSION_HEX < 0x030d00A1
             _PyGen_SetStopIterationValue(result);
+#else
+            if (!PyTuple_Check(result) && !PyExceptionInstance_Check(result)) {
+                PyErr_SetObject(PyExc_StopIteration, result);
+            } else {
+                PyObject *exc = __Pyx_PyObject_CallOneArg(PyExc_StopIteration, result);
+                if (likely(exc != NULL)) {
+                    PyErr_SetObject(PyExc_StopIteration, exc);
+                    Py_DECREF(exc);
+                }
+            }
+#endif
         }
-        Py_CLEAR(result);
+        Py_DECREF(result);
+        result = NULL;
     }
     return result;
 #endif
 }
 #endif
 static CYTHON_INLINE
 PyObject *__Pyx_Coroutine_FinishDelegation(__pyx_CoroutineObject *gen) {
@@ -11093,49 +11209,58 @@
     if (unlikely(!__pyx_GeneratorType)) {
         return -1;
     }
     return 0;
 }
 
 /* CheckBinaryVersion */
-static int __Pyx_check_binary_version(void) {
-    char ctversion[5];
-    int same=1, i, found_dot;
-    const char* rt_from_call = Py_GetVersion();
-    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    found_dot = 0;
-    for (i = 0; i < 4; i++) {
-        if (!ctversion[i]) {
-            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
-            break;
+static unsigned long __Pyx_get_runtime_version(void) {
+#if __PYX_LIMITED_VERSION_HEX >= 0x030B00A4
+    return Py_Version & ~0xFFUL;
+#else
+    const char* rt_version = Py_GetVersion();
+    unsigned long version = 0;
+    unsigned long factor = 0x01000000UL;
+    unsigned int digit = 0;
+    int i = 0;
+    while (factor) {
+        while ('0' <= rt_version[i] && rt_version[i] <= '9') {
+            digit = digit * 10 + (unsigned int) (rt_version[i] - '0');
+            ++i;
         }
-        if (rt_from_call[i] != ctversion[i]) {
-            same = 0;
+        version += factor * digit;
+        if (rt_version[i] != '.')
             break;
-        }
+        digit = 0;
+        factor >>= 8;
+        ++i;
     }
-    if (!same) {
-        char rtversion[5] = {'\0'};
+    return version;
+#endif
+}
+static int __Pyx_check_binary_version(unsigned long ct_version, unsigned long rt_version, int allow_newer) {
+    const unsigned long MAJOR_MINOR = 0xFFFF0000UL;
+    if ((rt_version & MAJOR_MINOR) == (ct_version & MAJOR_MINOR))
+        return 0;
+    if (likely(allow_newer && (rt_version & MAJOR_MINOR) > (ct_version & MAJOR_MINOR)))
+        return 1;
+    {
         char message[200];
-        for (i=0; i<4; ++i) {
-            if (rt_from_call[i] == '.') {
-                if (found_dot) break;
-                found_dot = 1;
-            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
-                break;
-            }
-            rtversion[i] = rt_from_call[i];
-        }
         PyOS_snprintf(message, sizeof(message),
-                      "compile time version %s of module '%.100s' "
-                      "does not match runtime version %s",
-                      ctversion, __Pyx_MODULE_NAME, rtversion);
+                      "compile time Python version %d.%d "
+                      "of module '%.100s' "
+                      "%s "
+                      "runtime version %d.%d",
+                       (int) (ct_version >> 24), (int) ((ct_version >> 16) & 0xFF),
+                       __Pyx_MODULE_NAME,
+                       (allow_newer) ? "was newer than" : "does not match",
+                       (int) (rt_version >> 24), (int) ((rt_version >> 16) & 0xFF)
+       );
         return PyErr_WarnEx(NULL, message, 1);
     }
-    return 0;
 }
 
 /* InitStrings */
 #if PY_MAJOR_VERSION >= 3
 static int __Pyx_InitString(__Pyx_StringTabEntry t, PyObject **str) {
     if (t.is_unicode | t.is_str) {
         if (t.intern) {
@@ -11173,16 +11298,32 @@
             return -1;
         #endif
         ++t;
     }
     return 0;
 }
 
+#include <string.h>
+static CYTHON_INLINE Py_ssize_t __Pyx_ssize_strlen(const char *s) {
+    size_t len = strlen(s);
+    if (unlikely(len > (size_t) PY_SSIZE_T_MAX)) {
+        PyErr_SetString(PyExc_OverflowError, "byte string is too long");
+        return -1;
+    }
+    return (Py_ssize_t) len;
+}
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_FromString(const char* c_str) {
-    return __Pyx_PyUnicode_FromStringAndSize(c_str, (Py_ssize_t)strlen(c_str));
+    Py_ssize_t len = __Pyx_ssize_strlen(c_str);
+    if (unlikely(len < 0)) return NULL;
+    return __Pyx_PyUnicode_FromStringAndSize(c_str, len);
+}
+static CYTHON_INLINE PyObject* __Pyx_PyByteArray_FromString(const char* c_str) {
+    Py_ssize_t len = __Pyx_ssize_strlen(c_str);
+    if (unlikely(len < 0)) return NULL;
+    return PyByteArray_FromStringAndSize(c_str, len);
 }
 static CYTHON_INLINE const char* __Pyx_PyObject_AsString(PyObject* o) {
     Py_ssize_t ignore;
     return __Pyx_PyObject_AsStringAndSize(o, &ignore);
 }
 #if __PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT
 #if !CYTHON_PEP393_ENABLED
```

### Comparing `pybedlite-0.0.4/cgranges/python/cgranges.pyx` & `pybedlite-0.1.0/cgranges/python/cgranges.pyx`

 * *Files identical despite different names*

### Comparing `pybedlite-0.0.4/cgranges/setup.py` & `pybedlite-0.1.0/cgranges/setup.py`

 * *Files identical despite different names*

### Comparing `pybedlite-0.0.4/cgranges/test/3rd-party/AIList/AIList.c` & `pybedlite-0.1.0/cgranges/test/3rd-party/AIList/AIList.c`

 * *Files identical despite different names*

### Comparing `pybedlite-0.0.4/cgranges/test/3rd-party/AIList/AIList.h` & `pybedlite-0.1.0/cgranges/test/3rd-party/AIList/AIList.h`

 * *Files identical despite different names*

### Comparing `pybedlite-0.0.4/cgranges/test/3rd-party/AITree/AITree.c` & `pybedlite-0.1.0/cgranges/test/3rd-party/AITree/AITree.c`

 * *Files identical despite different names*

### Comparing `pybedlite-0.0.4/cgranges/test/3rd-party/AITree/interval_tree.h` & `pybedlite-0.1.0/cgranges/test/3rd-party/AITree/interval_tree.h`

 * *Files identical despite different names*

### Comparing `pybedlite-0.0.4/cgranges/test/3rd-party/AITree/interval_tree_generic.h` & `pybedlite-0.1.0/cgranges/test/3rd-party/AITree/interval_tree_generic.h`

 * *Files identical despite different names*

### Comparing `pybedlite-0.0.4/cgranges/test/3rd-party/AITree/rbtree.c` & `pybedlite-0.1.0/cgranges/test/3rd-party/AITree/rbtree.c`

 * *Files identical despite different names*

### Comparing `pybedlite-0.0.4/cgranges/test/3rd-party/AITree/rbtree.h` & `pybedlite-0.1.0/cgranges/test/3rd-party/AITree/rbtree.h`

 * *Files identical despite different names*

### Comparing `pybedlite-0.0.4/cgranges/test/3rd-party/AITree/rbtree_augmented.h` & `pybedlite-0.1.0/cgranges/test/3rd-party/AITree/rbtree_augmented.h`

 * *Files identical despite different names*

### Comparing `pybedlite-0.0.4/cgranges/test/3rd-party/NCList/intervaldb.c` & `pybedlite-0.1.0/cgranges/test/3rd-party/NCList/intervaldb.c`

 * *Files identical despite different names*

### Comparing `pybedlite-0.0.4/cgranges/test/3rd-party/NCList/intervaldb.h` & `pybedlite-0.1.0/cgranges/test/3rd-party/NCList/intervaldb.h`

 * *Files identical despite different names*

### Comparing `pybedlite-0.0.4/cgranges/test/IntervalTree.h` & `pybedlite-0.1.0/cgranges/test/IntervalTree.h`

 * *Files identical despite different names*

### Comparing `pybedlite-0.0.4/cgranges/test/Makefile` & `pybedlite-0.1.0/cgranges/test/Makefile`

 * *Files identical despite different names*

### Comparing `pybedlite-0.0.4/cgranges/test/bedcov-cr.c` & `pybedlite-0.1.0/cgranges/test/bedcov-cr.c`

 * *Files identical despite different names*

### Comparing `pybedlite-0.0.4/cgranges/test/bedcov-cr.js` & `pybedlite-0.1.0/cgranges/test/bedcov-cr.js`

 * *Files identical despite different names*

### Comparing `pybedlite-0.0.4/cgranges/test/bedcov-cr.py` & `pybedlite-0.1.0/cgranges/test/bedcov-cr.py`

 * *Files identical despite different names*

### Comparing `pybedlite-0.0.4/cgranges/test/bedcov-cr1.py` & `pybedlite-0.1.0/cgranges/test/bedcov-cr1.py`

 * *Files identical despite different names*

### Comparing `pybedlite-0.0.4/cgranges/test/bedcov-cr2.py` & `pybedlite-0.1.0/cgranges/test/bedcov-cr2.py`

 * *Files identical despite different names*

### Comparing `pybedlite-0.0.4/cgranges/test/bedcov-iitree.cpp` & `pybedlite-0.1.0/cgranges/test/bedcov-iitree.cpp`

 * *Files identical despite different names*

### Comparing `pybedlite-0.0.4/cgranges/test/bedcov-itree.cpp` & `pybedlite-0.1.0/cgranges/test/bedcov-itree.cpp`

 * *Files identical despite different names*

### Comparing `pybedlite-0.0.4/cgranges/test/bedcov-naive.js` & `pybedlite-0.1.0/cgranges/test/bedcov-naive.js`

 * *Files identical despite different names*

### Comparing `pybedlite-0.0.4/cgranges/test/bedcov-ncls.py` & `pybedlite-0.1.0/cgranges/test/bedcov-ncls.py`

 * *Files identical despite different names*

### Comparing `pybedlite-0.0.4/cgranges/test/bedcov-py-iitree.py` & `pybedlite-0.1.0/cgranges/test/bedcov-py-iitree.py`

 * *Files identical despite different names*

### Comparing `pybedlite-0.0.4/cgranges/test/bedcov-qs.py` & `pybedlite-0.1.0/cgranges/test/bedcov-qs.py`

 * *Files identical despite different names*

### Comparing `pybedlite-0.0.4/cgranges/test/kseq.h` & `pybedlite-0.1.0/cgranges/test/kseq.h`

 * *Files identical despite different names*

### Comparing `pybedlite-0.0.4/pybedlite/__init__.py` & `pybedlite-0.1.0/pybedlite/__init__.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -49,19 +49,19 @@
     - :func:`pybedlite.reader` -- opens a BED file for reading.
     - :func:`pybedlite.writer` -- opens a BED file for writing.
 
 """
 
 from typing import Optional
 
-from pybedlite.bed_writer import BedWriter
-from pybedlite.bed_source import BedSource
-from pybedlite.bed_source import BedPath
 from pybedlite.bed_record import BedRecord
 from pybedlite.bed_record import BedStrand
+from pybedlite.bed_source import BedPath
+from pybedlite.bed_source import BedSource
+from pybedlite.bed_writer import BedWriter
 
 
 def reader(path: BedPath) -> "BedSource":
     """Returns BED file for reading. File handle will need to be opened with the
 
     Args:
         path: a file handle or path to the Bed to read.
```

### Comparing `pybedlite-0.0.4/pybedlite/bed_record.py` & `pybedlite-0.1.0/pybedlite/bed_record.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,31 +7,45 @@
 
 The module contains the following public classes:
 
     - :class:`~pybedtools.bed_record.BedStrand` -- Enumeration of possible strands for a bed record
     - :class:`~pybedtools.bed_record.BedRecord` -- Lightweight class for storing information
         pertaining to a BED record.
 """
-import attr
+
+from __future__ import annotations
+
 import enum
+from typing import TYPE_CHECKING
+from typing import ClassVar
+from typing import List
 from typing import Optional
 from typing import Tuple
-from typing import List
-from typing import ClassVar
+from typing import Type
+
+import attr
+
+if TYPE_CHECKING:
+    from pybedlite.overlap_detector import Interval
 
 
 """Maximum BED fields that can be present in a well formed BED file written to specification"""
 MAX_BED_FIELDS: int = 12
 
 
 @enum.unique
 class BedStrand(enum.Enum):
     Positive = "+"
     Negative = "-"
 
+    @property
+    def opposite(self) -> BedStrand:
+        """Return the opposite strand of the current strand."""
+        return BedStrand.Positive if self is BedStrand.Negative else BedStrand.Negative
+
 
 @attr.s(frozen=True, auto_attribs=True, kw_only=True, slots=True)
 class BedRecord:
     """Lightweight class for storing BED records. A more comprehensive description of BED format
     can be found at https://genome.ucsc.edu/FAQ/FAQformat.html#format1. Only `chrom`, `start`, and
     `end` are required.
 
@@ -184,7 +198,31 @@
         ), "BED records can only contain between 3 and 12 fields"
 
         number_of_output_fields = (
             self.bed_field_num if number_of_output_fields is None else number_of_output_fields
         )
         fields = self.bed_fields[:number_of_output_fields]
         return "\t".join(fields)
+
+    @classmethod
+    def from_interval(cls: Type["BedRecord"], interval: Interval) -> "BedRecord":
+        """
+        Construct a `BedRecord` from a `Interval` instance.
+
+        **Note that `Interval` cannot represent a `BedRecord` with a missing strand.**
+        Converting a record with no strand to `Interval` and then back to `BedRecord` will result in
+        a record with **positive strand**.
+
+        Args:
+            interval: The `Interval` instance to convert.
+
+        Returns:
+            A `BedRecord` corresponding to the same region specified in the interval.
+        """
+
+        return BedRecord(
+            chrom=interval.refname,
+            start=interval.start,
+            end=interval.end,
+            strand=BedStrand.Negative if interval.negative else BedStrand.Positive,
+            name=interval.name,
+        )
```

### Comparing `pybedlite-0.0.4/pybedlite/bed_source.py` & `pybedlite-0.1.0/pybedlite/bed_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,33 +6,34 @@
 ~~~~~~~~~~~~~~~
 
 The module contains the following public classes:
 
     - :class:`~pybedtools.bed_source.BedSource` -- Reader class for parsing BED files and iterate
         over their contained records
 """
+
 import io
-from typing import IO
-from typing import Optional
-from typing import TypeVar
-from typing import Union
-from typing import Type
-from typing import Tuple
-from typing import List
 from pathlib import Path
 from types import TracebackType
+from typing import IO
+from typing import Any
 from typing import Callable
 from typing import ContextManager
+from typing import Dict
 from typing import Iterable
 from typing import Iterator
-from typing import Dict
-from typing import Any
+from typing import List
+from typing import Optional
+from typing import Tuple
+from typing import Type
+from typing import TypeVar
+from typing import Union
 
-from pybedlite.bed_record import BedStrand
 from pybedlite.bed_record import BedRecord
+from pybedlite.bed_record import BedStrand
 
 """The classes that should be treated as file-like classes"""
 _IOClasses = (io.TextIOBase, io.BufferedIOBase, io.RawIOBase, io.IOBase)
 
 """The valid base classes for opening a BED file."""
 BedPath = Union[Path, str, IO[Any]]
```

### Comparing `pybedlite-0.0.4/pybedlite/bed_writer.py` & `pybedlite-0.1.0/pybedlite/bed_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,27 +6,26 @@
 ~~~~~~~~~~~~~~~
 
 The module contains the following public classes:
 
     - :class:`~pybedtools.bed_source.BedWriter` -- Writer class for writing BED files
 """
 
-from typing import IO
-from typing import Optional
-from typing import Type
 from pathlib import Path
 from types import TracebackType
+from typing import IO
 from typing import ContextManager
 from typing import Iterable
+from typing import Optional
+from typing import Type
 
 from pybedlite.bed_record import BedRecord
 from pybedlite.bed_source import BedPath
 from pybedlite.bed_source import _IOClasses
 
-
 """Maximum BED fields that can be present in a well formed BED file written to specification"""
 MAX_BED_FIELDS: int = 12
 
 
 class BedWriter(ContextManager):
     """Writer class for writing BED records to a file.
```

### Comparing `pybedlite-0.0.4/pybedlite/overlap_detector.py` & `pybedlite-0.1.0/pybedlite/overlap_detector.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,18 +42,20 @@
 from pathlib import Path
 from typing import Dict
 from typing import Iterable
 from typing import Iterator
 from typing import List
 from typing import Optional
 from typing import Set
+from typing import Type
 
 import attr
-import cgranges as cr
 
+import cgranges as cr
+from pybedlite.bed_record import BedRecord
 from pybedlite.bed_record import BedStrand
 from pybedlite.bed_source import BedSource
 
 
 @attr.s(frozen=True, auto_attribs=True)
 class Interval:
     """A region mapping to the genome that is 0-based and open-ended
@@ -96,19 +98,42 @@
         overlap = min(self.end, other.end) - max(self.start, other.start)
         return overlap if overlap > 0 else 0
 
     def length(self) -> int:
         """Returns the length of the interval."""
         return self.end - self.start
 
+    @classmethod
+    def from_bedrecord(cls: Type["Interval"], record: BedRecord) -> "Interval":
+        """
+        Construct an `Interval` from a `BedRecord` instance.
+
+        Note that when the `BedRecord` does not have a specified strand, the `Interval`'s negative
+        attribute is set to False. This mimics the behavior of `OverlapDetector.from_bed()` when
+        reading a record that does not have a specified strand.
+
+        Args:
+            record: The `BedRecord` instance to convert.
+
+        Returns:
+            An `Interval` corresponding to the same region specified in the record.
+        """
+        return cls(
+            refname=record.chrom,
+            start=record.start,
+            end=record.end,
+            negative=record.strand is BedStrand.Negative,
+            name=record.name,
+        )
+
 
 class OverlapDetector(Iterable[Interval]):
     """Detects and returns overlaps between a set of genomic regions and another genomic region.
 
-    Since :class:`~samwell.overlap_detector.Interval` objects are used both to populate the
+    Since :class:`~pybedlite.overlap_detector.Interval` objects are used both to populate the
     overlap detector and to query it, the coordinate system in use is also 0-based open-ended.
 
     The same interval may be added multiple times, but only a single instance will be returned
     when querying for overlaps.  Intervals with the same coordinates but different names are
     treated as different intervals.
 
     This detector is the most efficient when all intervals are added ahead of time.
@@ -232,24 +257,19 @@
               The intervals will be return in ascending genomic order.
         """
         results = self.get_overlaps(interval)
         return [i for i in results if i.start >= interval.start and i.end <= interval.end]
 
     @classmethod
     def from_bed(cls, path: Path) -> "OverlapDetector":
-        """Builds an :class:`~samwell.overlap_detector.OverlapDetector` from a BED file.
+        """Builds a :class:`~pybedlite.overlap_detector.OverlapDetector` from a BED file.
         Args:
             path: the path to the BED file
         Returns:
             An overlap detector for the regions in the BED file.
         """
         detector = OverlapDetector()
+
         for region in BedSource(path):
-            locatable = Interval(
-                refname=region.chrom,
-                start=region.start,
-                end=region.end,
-                negative=region.strand == BedStrand.Negative,
-                name=region.name,
-            )
-            detector.add(locatable)
+            detector.add(Interval.from_bedrecord(region))
+
         return detector
```

### Comparing `pybedlite-0.0.4/pybedlite/tests/test_pybedlite.py` & `pybedlite-0.1.0/pybedlite/tests/test_pybedlite.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,67 +1,20 @@
 """Tests for :py:mod:`~pybedlite.__init__.py`"""
 
-import pytest
 from pathlib import Path
 from typing import List
+
+import pytest
+
 import pybedlite as pybed
-from pybedlite.bed_writer import MAX_BED_FIELDS
-from pybedlite.bed_writer import BedWriter
-from pybedlite.bed_source import BedSource
 from pybedlite.bed_record import BedRecord
 from pybedlite.bed_record import BedStrand
-
-
-@pytest.fixture
-def bed_records() -> List[BedRecord]:
-    return [
-        BedRecord(
-            chrom="1",
-            start=100,
-            end=150,
-            name="test_record1",
-            score=100,
-            strand=BedStrand.Positive,
-            thick_start=100,
-            thick_end=100,
-            item_rgb=(0, 0, 0),
-            block_count=1,
-            block_sizes=[50],
-            block_starts=[0],
-        ),
-        BedRecord(
-            chrom="1",
-            start=200,
-            end=300,
-            name="test_record2",
-            score=100,
-            strand=BedStrand.Negative,
-            thick_start=210,
-            thick_end=290,
-            item_rgb=(0, 0, 0),
-            block_count=1,
-            block_sizes=[100],
-            block_starts=[0],
-        ),
-        BedRecord(
-            chrom="2",
-            start=200,
-            end=300,
-            name="test_record3",
-            score=None,
-            strand=None,
-            thick_start=None,
-            thick_end=None,
-            item_rgb=None,
-            block_count=None,
-            block_sizes=None,
-            block_starts=None,
-        ),
-    ]
-
+from pybedlite.bed_source import BedSource
+from pybedlite.bed_writer import MAX_BED_FIELDS
+from pybedlite.bed_writer import BedWriter
 
 SNIPPET_BED = """\
 # Test header, with a line with whitespace below it.
 
 # More header
 1	100	150	test_record1	100	+	100	100	0,0,0	1	50	0
 1	200	300	test_record2	100	-	210	290	0,0,0	1	100	0
@@ -248,7 +201,14 @@
         ):
             compare_bed_records(
                 record1=parsed_record,
                 record2=expected_record,
                 record_number=i,
                 num_fields=bed_field_number,
             )
+
+
+def test_bedstrand_opposite() -> None:
+    """Test that we can reverse a BedStrand."""
+
+    assert BedStrand.Positive.opposite is BedStrand.Negative
+    assert BedStrand.Negative.opposite is BedStrand.Positive
```

### Comparing `pybedlite-0.0.4/pyproject.toml` & `pybedlite-0.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybedlite"
-version = "0.0.4"
+version = "0.1.0"
 description = "Python classes for interfacing with bed intervals"
 authors = [
 	"Nils Homer <nils@fulcrumgenomics.com>",
 	"Tim Fennell <tim@fulcrumgenomics.com>",
 	"John Didion <john@fulcrumgenomics.com>",
 ]
 license = "MIT"
@@ -33,14 +33,15 @@
 sphinx = { version = "^7.0.0", optional = true }
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.0.0"
 mypy = "^1.5.0"
 flake8 = "^5.0.0"
 black = "^23.0.0"
+isort = "^5.13.0"
 pytest-cov = "^4.0.0"
 
 [tool.poetry.extras]
 docs = ["sphinx"]
 
 [tool.poetry.build]
 script = "build.py"
```

### Comparing `pybedlite-0.0.4/setup.py` & `pybedlite-0.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,34 +2,31 @@
 from setuptools import setup
 
 packages = \
 ['cgranges', 'cgranges.test', 'pybedlite', 'pybedlite.tests']
 
 package_data = \
 {'': ['*'],
- 'cgranges': ['.pytest_cache/*',
-              '.pytest_cache/v/cache/*',
-              'cpp/*',
-              'python/*'],
+ 'cgranges': ['cpp/*', 'python/*'],
  'cgranges.test': ['3rd-party/*',
                    '3rd-party/AIList/*',
                    '3rd-party/AITree/*',
                    '3rd-party/NCList/*']}
 
 install_requires = \
 ['attrs>=23.0.0,<24.0.0']
 
 extras_require = \
 {'docs': ['sphinx>=7.0.0,<8.0.0']}
 
 setup_kwargs = {
     'name': 'pybedlite',
-    'version': '0.0.4',
+    'version': '0.1.0',
     'description': 'Python classes for interfacing with bed intervals',
-    'long_description': '\n[![Language][language-badge]][language-link]\n[![Code Style][code-style-badge]][code-style-link]\n[![Type Checked][type-checking-badge]][type-checking-link]\n[![PEP8][pep-8-badge]][pep-8-link]\n[![Code Coverage][code-coverage-badge]][code-coverage-link]\n[![License][license-badge]][license-link]\n\n---\n\n[![Python package][python-package-badge]][python-package-link]\n[![PyPI version][pypi-badge]][pypi-link]\n[![PyPI download total][pypi-downloads-badge]][pypi-downloads-link]\n\n---\n\n[language-badge]:       http://img.shields.io/badge/language-python-brightgreen.svg\n[language-link]:        http://www.python.org/\n[code-style-badge]:     https://img.shields.io/badge/code%20style-black-000000.svg\n[code-style-link]:      https://black.readthedocs.io/en/stable/ \n[type-checking-badge]:  http://www.mypy-lang.org/static/mypy_badge.svg\n[type-checking-link]:   http://mypy-lang.org/\n[pep-8-badge]:          https://img.shields.io/badge/code%20style-pep8-brightgreen.svg\n[pep-8-link]:           https://www.python.org/dev/peps/pep-0008/\n[code-coverage-badge]:  https://codecov.io/gh/fulcrumgenomics/pybedlite/branch/main/graph/badge.svg\n[code-coverage-link]:   https://codecov.io/gh/fulcrumgenomics/pybedlite\n[license-badge]:        http://img.shields.io/badge/license-MIT-blue.svg\n[license-link]:         https://github.com/fulcrumgenomics/pybedlite/blob/main/LICENSE\n[python-package-badge]: https://github.com/fulcrumgenomics/pybedlite/workflows/Python%20package/badge.svg\n[python-package-link]:  https://github.com/fulcrumgenomics/pybedlite/actions?query=workflow%3A%22Python+package%22\n[pypi-badge]:           https://badge.fury.io/py/pybedlite.svg\n[pypi-link]:            https://pypi.python.org/pypi/pybedlite\n[pypi-downloads-badge]: https://img.shields.io/pypi/dm/pybedlite\n[pypi-downloads-link]:  https://pypi.python.org/pypi/pybedlite\n\n# pybedlite\n\nSee documentation on [pybedlite.readthedocs.org][rtd-link].\n\n```\nconda install -c bioconda pybedlite\n```\nOR\n```\nconda create -n pybedlite pybedlite\nconda activate pybedlite\n```\n\nNote that while there is a version of pybedlite on pypi versions of pybedlite >=\n0.0.2 cannot at present be installed via pypi because they have dependencies\nthat preclude publishing to pypi. For this reason installation via conda is\nrequired.\n\n[rtd-link]:    http://pybedlite.readthedocs.org/en/stable\n\n**Requires python 3.8+** (for python < 3.8, please use pybedlite <= 0.0.3)\n\n# Getting Setup for Development Work\n\n[Poetry][poetry-link] is used to manage the python development environment. \n\nA simple way to create an environment with the desired version of python and poetry is to use [conda][conda-link].  E.g.:\n\n```bash\nconda create -n pybedlite python=3.8 poetry\nconda activate pybedlite\npoetry install\n```\n\nIf the methods listed above do not work try the following:\n```bash\nmamba create -n pybedlite -c conda-forge "python=3.9.16" "poetry=1.6.1"\nmamba activate pybedlite\npoetry install\n```\n\nIf, during `poetry install` on Mac OS X errors are encountered running gcc/clang to build `pybedtools` or other packages with native code, try setting the following and re-running `poetry install`:\n```bash\nexport CFLAGS="-stdlib=libc++"\n``` \n\n[poetry-link]: https://github.com/python-poetry/poetry\n[conda-link]:  https://docs.conda.io/en/latest/miniconda.html\n\n## Checking the Build\n### Run all checks with:\n```bash\n./ci/check.sh\n```\n',
+    'long_description': '\n[![Language][language-badge]][language-link]\n[![Code Style][code-style-badge]][code-style-link]\n[![Type Checked][type-checking-badge]][type-checking-link]\n[![PEP8][pep-8-badge]][pep-8-link]\n[![Code Coverage][code-coverage-badge]][code-coverage-link]\n[![License][license-badge]][license-link]\n\n---\n\n[![Python package][python-package-badge]][python-package-link]\n[![PyPI version][pypi-badge]][pypi-link]\n[![PyPI download total][pypi-downloads-badge]][pypi-downloads-link]\n\n---\n\n[language-badge]:       http://img.shields.io/badge/language-python-brightgreen.svg\n[language-link]:        http://www.python.org/\n[code-style-badge]:     https://img.shields.io/badge/code%20style-black-000000.svg\n[code-style-link]:      https://black.readthedocs.io/en/stable/ \n[type-checking-badge]:  http://www.mypy-lang.org/static/mypy_badge.svg\n[type-checking-link]:   http://mypy-lang.org/\n[pep-8-badge]:          https://img.shields.io/badge/code%20style-pep8-brightgreen.svg\n[pep-8-link]:           https://www.python.org/dev/peps/pep-0008/\n[code-coverage-badge]:  https://codecov.io/gh/fulcrumgenomics/pybedlite/branch/main/graph/badge.svg\n[code-coverage-link]:   https://codecov.io/gh/fulcrumgenomics/pybedlite\n[license-badge]:        http://img.shields.io/badge/license-MIT-blue.svg\n[license-link]:         https://github.com/fulcrumgenomics/pybedlite/blob/main/LICENSE\n[python-package-badge]: https://github.com/fulcrumgenomics/pybedlite/workflows/Python%20package/badge.svg\n[python-package-link]:  https://github.com/fulcrumgenomics/pybedlite/actions?query=workflow%3A%22Python+package%22\n[pypi-badge]:           https://badge.fury.io/py/pybedlite.svg\n[pypi-link]:            https://pypi.python.org/pypi/pybedlite\n[pypi-downloads-badge]: https://img.shields.io/pypi/dm/pybedlite\n[pypi-downloads-link]:  https://pypi.python.org/pypi/pybedlite\n\n# pybedlite\n\nSee documentation on [pybedlite.readthedocs.org][rtd-link].\n\n```\npip install pybedlite\n```\nOR\n```\nconda install -c bioconda pybedlite\n```\nOR\n```\nconda create -n pybedlite pybedlite\nconda activate pybedlite\n```\n\n[rtd-link]:    http://pybedlite.readthedocs.org/en/stable\n\n**Requires python 3.8+** (for python < 3.8, please use pybedlite <= 0.0.3)\n\n# Getting Setup for Development Work\n\nClone the repository to your local machine. Note that pybedlite >= 0.0.4 includes [cgranges][cgranges-link] as a submodule, so you must use the `--recurse-submodules` option:\n```\ngit clone --recurse-submodules https://github.com/fulcrumgenomics/pybedlite.git\n```\n\n[Poetry][poetry-link] is used to manage the python development environment.\n\nA simple way to create an environment with the desired version of python and poetry is to use [conda][conda-link].  E.g.:\n\n```bash\nconda create -n pybedlite python=3.8 poetry\nconda activate pybedlite\npoetry install\n```\n\nIf the methods listed above do not work try the following:\n```bash\nmamba create -n pybedlite -c conda-forge "python=3.9.16" "poetry=1.6.1"\nmamba activate pybedlite\npoetry install\n```\n\nIf, during `poetry install` on Mac OS X errors are encountered running gcc/clang to build `pybedtools` or other packages with native code, try setting the following and re-running `poetry install`:\n```bash\nexport CFLAGS="-stdlib=libc++"\n``` \n\n[poetry-link]: https://github.com/python-poetry/poetry\n[conda-link]:  https://docs.conda.io/en/latest/miniconda.html\n[cgranges-link]: https://github.com/lh3/cgranges\n\n## Checking the Build\n### Run all checks with:\n```bash\n./ci/check.sh\n```\n',
     'author': 'Nils Homer',
     'author_email': 'nils@fulcrumgenomics.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/fulcrumgenomics/pybedlite',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pybedlite-0.0.4/PKG-INFO` & `pybedlite-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybedlite
-Version: 0.0.4
+Version: 0.1.0
 Summary: Python classes for interfacing with bed intervals
 Home-page: https://github.com/fulcrumgenomics/pybedlite
 License: MIT
 Keywords: bioinformatics
 Author: Nils Homer
 Author-email: nils@fulcrumgenomics.com
 Requires-Python: >=3.8.0,<4.0.0
@@ -64,34 +64,38 @@
 [pypi-downloads-link]:  https://pypi.python.org/pypi/pybedlite
 
 # pybedlite
 
 See documentation on [pybedlite.readthedocs.org][rtd-link].
 
 ```
+pip install pybedlite
+```
+OR
+```
 conda install -c bioconda pybedlite
 ```
 OR
 ```
 conda create -n pybedlite pybedlite
 conda activate pybedlite
 ```
 
-Note that while there is a version of pybedlite on pypi versions of pybedlite >=
-0.0.2 cannot at present be installed via pypi because they have dependencies
-that preclude publishing to pypi. For this reason installation via conda is
-required.
-
 [rtd-link]:    http://pybedlite.readthedocs.org/en/stable
 
 **Requires python 3.8+** (for python < 3.8, please use pybedlite <= 0.0.3)
 
 # Getting Setup for Development Work
 
-[Poetry][poetry-link] is used to manage the python development environment. 
+Clone the repository to your local machine. Note that pybedlite >= 0.0.4 includes [cgranges][cgranges-link] as a submodule, so you must use the `--recurse-submodules` option:
+```
+git clone --recurse-submodules https://github.com/fulcrumgenomics/pybedlite.git
+```
+
+[Poetry][poetry-link] is used to manage the python development environment.
 
 A simple way to create an environment with the desired version of python and poetry is to use [conda][conda-link].  E.g.:
 
 ```bash
 conda create -n pybedlite python=3.8 poetry
 conda activate pybedlite
 poetry install
@@ -107,14 +111,15 @@
 If, during `poetry install` on Mac OS X errors are encountered running gcc/clang to build `pybedtools` or other packages with native code, try setting the following and re-running `poetry install`:
 ```bash
 export CFLAGS="-stdlib=libc++"
 ``` 
 
 [poetry-link]: https://github.com/python-poetry/poetry
 [conda-link]:  https://docs.conda.io/en/latest/miniconda.html
+[cgranges-link]: https://github.com/lh3/cgranges
 
 ## Checking the Build
 ### Run all checks with:
 ```bash
 ./ci/check.sh
 ```
```

