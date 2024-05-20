# Comparing `tmp/hpo-toolkit-0.5.0.tar.gz` & `tmp/hpo_toolkit-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hpo-toolkit-0.5.0.tar", last modified: Wed Mar 13 14:53:36 2024, max compression
+gzip compressed data, was "hpo_toolkit-0.5.1.tar", last modified: Mon May 20 17:13:09 2024, max compression
```

## Comparing `hpo-toolkit-0.5.0.tar` & `hpo_toolkit-0.5.1.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2024-03-13 14:53:36.131795 hpo-toolkit-0.5.0/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)    35149 2022-12-16 17:20:05.000000 hpo-toolkit-0.5.0/LICENSE
--rw-r--r--   0 ielis     (1000) ielis     (1000)    43001 2024-03-13 14:53:36.131795 hpo-toolkit-0.5.0/PKG-INFO
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     1359 2024-03-13 13:11:58.000000 hpo-toolkit-0.5.0/README.md
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     1267 2024-02-09 20:27:10.000000 hpo-toolkit-0.5.0/pyproject.toml
--rw-rw-r--   0 ielis     (1000) ielis     (1000)       38 2024-03-13 14:53:36.131795 hpo-toolkit-0.5.0/setup.cfg
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2024-03-13 14:53:36.115794 hpo-toolkit-0.5.0/src/
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2024-03-13 14:53:36.131795 hpo-toolkit-0.5.0/src/hpo_toolkit.egg-info/
--rw-r--r--   0 ielis     (1000) ielis     (1000)    43001 2024-03-13 14:53:36.000000 hpo-toolkit-0.5.0/src/hpo_toolkit.egg-info/PKG-INFO
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     2731 2024-03-13 14:53:36.000000 hpo-toolkit-0.5.0/src/hpo_toolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 ielis     (1000) ielis     (1000)        1 2024-03-13 14:53:36.000000 hpo-toolkit-0.5.0/src/hpo_toolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 ielis     (1000) ielis     (1000)        1 2023-02-27 14:40:18.000000 hpo-toolkit-0.5.0/src/hpo_toolkit.egg-info/not-zip-safe
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      151 2024-03-13 14:53:36.000000 hpo-toolkit-0.5.0/src/hpo_toolkit.egg-info/requires.txt
--rw-rw-r--   0 ielis     (1000) ielis     (1000)        6 2024-03-13 14:53:36.000000 hpo-toolkit-0.5.0/src/hpo_toolkit.egg-info/top_level.txt
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2024-03-13 14:53:36.119794 hpo-toolkit-0.5.0/src/hpotk/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      638 2024-03-13 14:49:16.000000 hpo-toolkit-0.5.0/src/hpotk/__init__.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2024-03-13 14:53:36.119794 hpo-toolkit-0.5.0/src/hpotk/algorithm/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      213 2023-09-01 19:53:47.000000 hpo-toolkit-0.5.0/src/hpotk/algorithm/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     2696 2023-05-12 16:45:32.000000 hpo-toolkit-0.5.0/src/hpotk/algorithm/_augment.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     6205 2023-09-01 19:53:47.000000 hpo-toolkit-0.5.0/src/hpotk/algorithm/_traversal.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2024-03-13 14:53:36.119794 hpo-toolkit-0.5.0/src/hpotk/algorithm/similarity/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      393 2023-08-01 20:24:52.000000 hpo-toolkit-0.5.0/src/hpotk/algorithm/similarity/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     3772 2023-06-12 17:28:47.000000 hpo-toolkit-0.5.0/src/hpotk/algorithm/similarity/_ic.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     6489 2023-05-12 16:45:32.000000 hpo-toolkit-0.5.0/src/hpotk/algorithm/similarity/_model.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     2728 2023-05-12 16:45:32.000000 hpo-toolkit-0.5.0/src/hpotk/algorithm/similarity/_resnik.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2024-03-13 14:53:36.119794 hpo-toolkit-0.5.0/src/hpotk/annotations/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     1102 2023-10-13 15:29:10.000000 hpo-toolkit-0.5.0/src/hpotk/annotations/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     3025 2024-02-13 02:07:32.000000 hpo-toolkit-0.5.0/src/hpotk/annotations/_api.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     6648 2023-10-13 15:41:02.000000 hpo-toolkit-0.5.0/src/hpotk/annotations/_base.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     3970 2023-10-13 16:12:13.000000 hpo-toolkit-0.5.0/src/hpotk/annotations/_simple.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      449 2023-12-04 15:34:46.000000 hpo-toolkit-0.5.0/src/hpotk/annotations/_test__base.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      670 2023-12-04 15:34:46.000000 hpo-toolkit-0.5.0/src/hpotk/annotations/_test__simple.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2024-03-13 14:53:36.119794 hpo-toolkit-0.5.0/src/hpotk/annotations/load/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)       54 2023-03-08 21:00:13.000000 hpo-toolkit-0.5.0/src/hpotk/annotations/load/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      307 2023-03-08 21:00:13.000000 hpo-toolkit-0.5.0/src/hpotk/annotations/load/_api.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2024-03-13 14:53:36.119794 hpo-toolkit-0.5.0/src/hpotk/annotations/load/hpoa/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)       88 2023-11-28 22:01:25.000000 hpo-toolkit-0.5.0/src/hpotk/annotations/load/hpoa/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)    11192 2023-06-12 17:28:47.000000 hpo-toolkit-0.5.0/src/hpotk/annotations/load/hpoa/_impl.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     1519 2023-08-01 20:24:52.000000 hpo-toolkit-0.5.0/src/hpotk/annotations/load/hpoa/_test__impl.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2024-03-13 14:53:36.123794 hpo-toolkit-0.5.0/src/hpotk/constants/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)       87 2023-10-13 15:15:11.000000 hpo-toolkit-0.5.0/src/hpotk/constants/__init__.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2024-03-13 14:53:36.123794 hpo-toolkit-0.5.0/src/hpotk/constants/hpo/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      191 2023-10-13 15:15:11.000000 hpo-toolkit-0.5.0/src/hpotk/constants/hpo/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      703 2023-10-13 15:15:11.000000 hpo-toolkit-0.5.0/src/hpotk/constants/hpo/base.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     2428 2023-03-08 21:00:13.000000 hpo-toolkit-0.5.0/src/hpotk/constants/hpo/frequency.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     1925 2022-12-28 21:43:07.000000 hpo-toolkit-0.5.0/src/hpotk/constants/hpo/inheritance.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     1419 2022-12-28 21:43:07.000000 hpo-toolkit-0.5.0/src/hpotk/constants/hpo/onset.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     1989 2022-12-28 21:43:07.000000 hpo-toolkit-0.5.0/src/hpotk/constants/hpo/organ_system.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      376 2022-12-28 21:43:07.000000 hpo-toolkit-0.5.0/src/hpotk/constants/hpo/severity.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2024-03-13 14:53:36.123794 hpo-toolkit-0.5.0/src/hpotk/graph/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      439 2024-02-09 20:27:10.000000 hpo-toolkit-0.5.0/src/hpotk/graph/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)    17433 2024-02-13 04:24:30.000000 hpo-toolkit-0.5.0/src/hpotk/graph/_api.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     7614 2023-08-19 03:37:58.000000 hpo-toolkit-0.5.0/src/hpotk/graph/_csr_graph.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     3085 2024-02-09 20:27:10.000000 hpo-toolkit-0.5.0/src/hpotk/graph/_csr_idx_graph.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)    12430 2024-02-09 20:38:06.000000 hpo-toolkit-0.5.0/src/hpotk/graph/_factory.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)    15186 2024-02-13 04:28:06.000000 hpo-toolkit-0.5.0/src/hpotk/graph/_test__api.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     6774 2023-09-01 18:45:21.000000 hpo-toolkit-0.5.0/src/hpotk/graph/_test__csr_graph.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     6760 2024-02-09 20:27:10.000000 hpo-toolkit-0.5.0/src/hpotk/graph/_test__factory.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     5679 2024-02-09 20:27:10.000000 hpo-toolkit-0.5.0/src/hpotk/graph/_test_csr_idx_graph.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      871 2023-12-15 02:18:57.000000 hpo-toolkit-0.5.0/src/hpotk/graph/_test_data.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2024-03-13 14:53:36.123794 hpo-toolkit-0.5.0/src/hpotk/graph/csr/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)       90 2023-05-12 16:45:32.000000 hpo-toolkit-0.5.0/src/hpotk/graph/csr/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     7766 2023-05-26 17:21:12.000000 hpo-toolkit-0.5.0/src/hpotk/graph/csr/_csr.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     5587 2023-08-01 20:24:52.000000 hpo-toolkit-0.5.0/src/hpotk/graph/csr/_test__csr.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2024-03-13 14:53:36.127794 hpo-toolkit-0.5.0/src/hpotk/model/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      902 2024-03-13 14:06:38.000000 hpo-toolkit-0.5.0/src/hpotk/model/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     5606 2023-10-13 14:58:12.000000 hpo-toolkit-0.5.0/src/hpotk/model/_base.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)    16404 2024-03-13 14:06:38.000000 hpo-toolkit-0.5.0/src/hpotk/model/_term.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     5086 2023-08-14 02:11:52.000000 hpo-toolkit-0.5.0/src/hpotk/model/_term_id.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     1478 2023-08-01 20:24:52.000000 hpo-toolkit-0.5.0/src/hpotk/model/_test__term_id.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2024-03-13 14:53:36.127794 hpo-toolkit-0.5.0/src/hpotk/ontology/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      344 2023-08-18 21:40:37.000000 hpo-toolkit-0.5.0/src/hpotk/ontology/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     4485 2023-10-13 15:15:11.000000 hpo-toolkit-0.5.0/src/hpotk/ontology/_api.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     4997 2023-09-06 13:40:42.000000 hpo-toolkit-0.5.0/src/hpotk/ontology/_default.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2024-03-13 14:53:36.127794 hpo-toolkit-0.5.0/src/hpotk/ontology/load/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)       24 2023-02-27 15:19:11.000000 hpo-toolkit-0.5.0/src/hpotk/ontology/load/__init__.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2024-03-13 14:53:36.127794 hpo-toolkit-0.5.0/src/hpotk/ontology/load/obographs/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      211 2023-08-01 20:24:52.000000 hpo-toolkit-0.5.0/src/hpotk/ontology/load/obographs/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     6105 2024-03-13 14:06:38.000000 hpo-toolkit-0.5.0/src/hpotk/ontology/load/obographs/_factory.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     6951 2024-02-09 20:27:10.000000 hpo-toolkit-0.5.0/src/hpotk/ontology/load/obographs/_load.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     9853 2023-04-14 14:23:26.000000 hpo-toolkit-0.5.0/src/hpotk/ontology/load/obographs/_model.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      828 2023-08-01 20:24:52.000000 hpo-toolkit-0.5.0/src/hpotk/ontology/load/obographs/_test_load.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2024-03-13 14:53:36.127794 hpo-toolkit-0.5.0/src/hpotk/util/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      542 2024-03-13 13:11:58.000000 hpo-toolkit-0.5.0/src/hpotk/util/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     5374 2023-09-01 00:24:20.000000 hpo-toolkit-0.5.0/src/hpotk/util/_io.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      967 2023-09-01 00:32:25.000000 hpo-toolkit-0.5.0/src/hpotk/util/_log.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     1490 2023-09-01 00:28:55.000000 hpo-toolkit-0.5.0/src/hpotk/util/_validate.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2024-03-13 14:53:36.127794 hpo-toolkit-0.5.0/src/hpotk/util/sort/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      413 2023-12-15 16:24:39.000000 hpo-toolkit-0.5.0/src/hpotk/util/sort/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      614 2023-09-01 15:29:00.000000 hpo-toolkit-0.5.0/src/hpotk/util/sort/_api.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)    12575 2023-12-15 16:13:38.000000 hpo-toolkit-0.5.0/src/hpotk/util/sort/_hierarchical.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     6185 2023-12-15 16:05:24.000000 hpo-toolkit-0.5.0/src/hpotk/util/sort/_test__hierarchical.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2024-03-13 14:53:36.127794 hpo-toolkit-0.5.0/src/hpotk/util/store/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      225 2024-03-13 13:11:58.000000 hpo-toolkit-0.5.0/src/hpotk/util/store/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     3329 2024-03-13 13:11:58.000000 hpo-toolkit-0.5.0/src/hpotk/util/store/_api.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     1529 2024-03-13 13:11:58.000000 hpo-toolkit-0.5.0/src/hpotk/util/store/_config.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     4713 2024-03-13 13:11:58.000000 hpo-toolkit-0.5.0/src/hpotk/util/store/_github.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2024-03-13 14:53:36.127794 hpo-toolkit-0.5.0/src/hpotk/validate/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      517 2023-08-19 00:46:45.000000 hpo-toolkit-0.5.0/src/hpotk/validate/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     7782 2023-08-19 00:58:27.000000 hpo-toolkit-0.5.0/src/hpotk/validate/_hpo.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     3386 2023-12-05 04:09:32.000000 hpo-toolkit-0.5.0/src/hpotk/validate/_model.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     1909 2023-06-12 17:28:47.000000 hpo-toolkit-0.5.0/src/hpotk/validate/_util.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2024-03-13 14:53:36.131795 hpo-toolkit-0.5.0/tests/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     2311 2024-03-13 14:06:38.000000 hpo-toolkit-0.5.0/tests/test_obographs.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     1151 2024-03-13 13:11:58.000000 hpo-toolkit-0.5.0/tests/test_store.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     4582 2024-03-13 14:06:38.000000 hpo-toolkit-0.5.0/tests/test_term.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     2968 2023-12-04 15:57:34.000000 hpo-toolkit-0.5.0/tests/test_term_id.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     7854 2024-02-09 20:27:10.000000 hpo-toolkit-0.5.0/tests/test_validate.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2024-05-20 17:13:09.203904 hpo_toolkit-0.5.1/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)    35149 2022-12-16 17:20:05.000000 hpo_toolkit-0.5.1/LICENSE
+-rw-r--r--   0 ielis     (1000) ielis     (1000)    43296 2024-05-20 17:13:09.203904 hpo_toolkit-0.5.1/PKG-INFO
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     1442 2024-05-09 01:09:18.000000 hpo_toolkit-0.5.1/README.md
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     1474 2024-05-09 01:09:19.000000 hpo_toolkit-0.5.1/pyproject.toml
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)       38 2024-05-20 17:13:09.203904 hpo_toolkit-0.5.1/setup.cfg
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2024-05-20 17:13:09.187904 hpo_toolkit-0.5.1/src/
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2024-05-20 17:13:09.199904 hpo_toolkit-0.5.1/src/hpo_toolkit.egg-info/
+-rw-r--r--   0 ielis     (1000) ielis     (1000)    43296 2024-05-20 17:13:09.000000 hpo_toolkit-0.5.1/src/hpo_toolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     2711 2024-05-20 17:13:09.000000 hpo_toolkit-0.5.1/src/hpo_toolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)        1 2024-05-20 17:13:09.000000 hpo_toolkit-0.5.1/src/hpo_toolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)        1 2023-02-27 14:40:18.000000 hpo_toolkit-0.5.1/src/hpo_toolkit.egg-info/not-zip-safe
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      159 2024-05-20 17:13:09.000000 hpo_toolkit-0.5.1/src/hpo_toolkit.egg-info/requires.txt
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)        6 2024-05-20 17:13:09.000000 hpo_toolkit-0.5.1/src/hpo_toolkit.egg-info/top_level.txt
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2024-05-20 17:13:09.191903 hpo_toolkit-0.5.1/src/hpotk/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      653 2024-05-20 17:11:33.000000 hpo_toolkit-0.5.1/src/hpotk/__init__.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2024-05-20 17:13:09.191903 hpo_toolkit-0.5.1/src/hpotk/algorithm/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      213 2023-09-01 19:53:47.000000 hpo_toolkit-0.5.1/src/hpotk/algorithm/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     2696 2023-05-12 16:45:32.000000 hpo_toolkit-0.5.1/src/hpotk/algorithm/_augment.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     6205 2023-09-01 19:53:47.000000 hpo_toolkit-0.5.1/src/hpotk/algorithm/_traversal.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2024-05-20 17:13:09.191903 hpo_toolkit-0.5.1/src/hpotk/algorithm/similarity/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      393 2023-08-01 20:24:52.000000 hpo_toolkit-0.5.1/src/hpotk/algorithm/similarity/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     3772 2023-06-12 17:28:47.000000 hpo_toolkit-0.5.1/src/hpotk/algorithm/similarity/_ic.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     6489 2023-05-12 16:45:32.000000 hpo_toolkit-0.5.1/src/hpotk/algorithm/similarity/_model.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     2728 2023-05-12 16:45:32.000000 hpo_toolkit-0.5.1/src/hpotk/algorithm/similarity/_resnik.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2024-05-20 17:13:09.191903 hpo_toolkit-0.5.1/src/hpotk/annotations/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     1102 2023-10-13 15:29:10.000000 hpo_toolkit-0.5.1/src/hpotk/annotations/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     3025 2024-02-13 02:07:32.000000 hpo_toolkit-0.5.1/src/hpotk/annotations/_api.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     6648 2023-10-13 15:41:02.000000 hpo_toolkit-0.5.1/src/hpotk/annotations/_base.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     3970 2023-10-13 16:12:13.000000 hpo_toolkit-0.5.1/src/hpotk/annotations/_simple.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      449 2023-12-04 15:34:46.000000 hpo_toolkit-0.5.1/src/hpotk/annotations/_test__base.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      670 2023-12-04 15:34:46.000000 hpo_toolkit-0.5.1/src/hpotk/annotations/_test__simple.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2024-05-20 17:13:09.191903 hpo_toolkit-0.5.1/src/hpotk/annotations/load/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)       54 2023-03-08 21:00:13.000000 hpo_toolkit-0.5.1/src/hpotk/annotations/load/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      307 2023-03-08 21:00:13.000000 hpo_toolkit-0.5.1/src/hpotk/annotations/load/_api.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2024-05-20 17:13:09.191903 hpo_toolkit-0.5.1/src/hpotk/annotations/load/hpoa/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)       88 2023-11-28 22:01:25.000000 hpo_toolkit-0.5.1/src/hpotk/annotations/load/hpoa/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)    11192 2023-06-12 17:28:47.000000 hpo_toolkit-0.5.1/src/hpotk/annotations/load/hpoa/_impl.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     1519 2023-08-01 20:24:52.000000 hpo_toolkit-0.5.1/src/hpotk/annotations/load/hpoa/_test__impl.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2024-05-20 17:13:09.195904 hpo_toolkit-0.5.1/src/hpotk/constants/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)       87 2023-10-13 15:15:11.000000 hpo_toolkit-0.5.1/src/hpotk/constants/__init__.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2024-05-20 17:13:09.195904 hpo_toolkit-0.5.1/src/hpotk/constants/hpo/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      191 2023-10-13 15:15:11.000000 hpo_toolkit-0.5.1/src/hpotk/constants/hpo/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      703 2023-10-13 15:15:11.000000 hpo_toolkit-0.5.1/src/hpotk/constants/hpo/base.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     2428 2023-03-08 21:00:13.000000 hpo_toolkit-0.5.1/src/hpotk/constants/hpo/frequency.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     1925 2022-12-28 21:43:07.000000 hpo_toolkit-0.5.1/src/hpotk/constants/hpo/inheritance.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     1419 2022-12-28 21:43:07.000000 hpo_toolkit-0.5.1/src/hpotk/constants/hpo/onset.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     1989 2022-12-28 21:43:07.000000 hpo_toolkit-0.5.1/src/hpotk/constants/hpo/organ_system.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      376 2022-12-28 21:43:07.000000 hpo_toolkit-0.5.1/src/hpotk/constants/hpo/severity.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2024-05-20 17:13:09.195904 hpo_toolkit-0.5.1/src/hpotk/graph/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      439 2024-02-09 20:27:10.000000 hpo_toolkit-0.5.1/src/hpotk/graph/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)    17433 2024-02-13 04:24:30.000000 hpo_toolkit-0.5.1/src/hpotk/graph/_api.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     7614 2023-08-19 03:37:58.000000 hpo_toolkit-0.5.1/src/hpotk/graph/_csr_graph.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     3085 2024-02-09 20:27:10.000000 hpo_toolkit-0.5.1/src/hpotk/graph/_csr_idx_graph.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)    12430 2024-02-09 20:38:06.000000 hpo_toolkit-0.5.1/src/hpotk/graph/_factory.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)    15186 2024-02-13 04:28:06.000000 hpo_toolkit-0.5.1/src/hpotk/graph/_test__api.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     6774 2023-09-01 18:45:21.000000 hpo_toolkit-0.5.1/src/hpotk/graph/_test__csr_graph.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     6760 2024-02-09 20:27:10.000000 hpo_toolkit-0.5.1/src/hpotk/graph/_test__factory.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     5679 2024-02-09 20:27:10.000000 hpo_toolkit-0.5.1/src/hpotk/graph/_test_csr_idx_graph.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      871 2023-12-15 02:18:57.000000 hpo_toolkit-0.5.1/src/hpotk/graph/_test_data.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2024-05-20 17:13:09.195904 hpo_toolkit-0.5.1/src/hpotk/graph/csr/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)       90 2023-05-12 16:45:32.000000 hpo_toolkit-0.5.1/src/hpotk/graph/csr/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     7766 2023-05-26 17:21:12.000000 hpo_toolkit-0.5.1/src/hpotk/graph/csr/_csr.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     5587 2023-08-01 20:24:52.000000 hpo_toolkit-0.5.1/src/hpotk/graph/csr/_test__csr.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2024-05-20 17:13:09.195904 hpo_toolkit-0.5.1/src/hpotk/model/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      902 2024-03-13 14:06:38.000000 hpo_toolkit-0.5.1/src/hpotk/model/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     5606 2023-10-13 14:58:12.000000 hpo_toolkit-0.5.1/src/hpotk/model/_base.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)    16404 2024-03-13 14:06:38.000000 hpo_toolkit-0.5.1/src/hpotk/model/_term.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     5086 2023-08-14 02:11:52.000000 hpo_toolkit-0.5.1/src/hpotk/model/_term_id.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     1478 2023-08-01 20:24:52.000000 hpo_toolkit-0.5.1/src/hpotk/model/_test__term_id.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2024-05-20 17:13:09.195904 hpo_toolkit-0.5.1/src/hpotk/ontology/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      344 2023-08-18 21:40:37.000000 hpo_toolkit-0.5.1/src/hpotk/ontology/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     5091 2024-03-25 13:31:39.000000 hpo_toolkit-0.5.1/src/hpotk/ontology/_api.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     4997 2023-09-06 13:40:42.000000 hpo_toolkit-0.5.1/src/hpotk/ontology/_default.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2024-05-20 17:13:09.195904 hpo_toolkit-0.5.1/src/hpotk/ontology/load/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)       24 2023-02-27 15:19:11.000000 hpo_toolkit-0.5.1/src/hpotk/ontology/load/__init__.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2024-05-20 17:13:09.199904 hpo_toolkit-0.5.1/src/hpotk/ontology/load/obographs/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      211 2023-08-01 20:24:52.000000 hpo_toolkit-0.5.1/src/hpotk/ontology/load/obographs/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     6105 2024-03-13 14:06:38.000000 hpo_toolkit-0.5.1/src/hpotk/ontology/load/obographs/_factory.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     6951 2024-02-09 20:27:10.000000 hpo_toolkit-0.5.1/src/hpotk/ontology/load/obographs/_load.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     9853 2023-04-14 14:23:26.000000 hpo_toolkit-0.5.1/src/hpotk/ontology/load/obographs/_model.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      828 2023-08-01 20:24:52.000000 hpo_toolkit-0.5.1/src/hpotk/ontology/load/obographs/_test_load.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2024-05-20 17:13:09.199904 hpo_toolkit-0.5.1/src/hpotk/store/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      869 2024-05-20 16:38:01.000000 hpo_toolkit-0.5.1/src/hpotk/store/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     6500 2024-05-20 16:46:28.000000 hpo_toolkit-0.5.1/src/hpotk/store/_api.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     2213 2024-05-20 16:35:21.000000 hpo_toolkit-0.5.1/src/hpotk/store/_config.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     3840 2024-05-20 16:59:01.000000 hpo_toolkit-0.5.1/src/hpotk/store/_github.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2024-05-20 17:13:09.199904 hpo_toolkit-0.5.1/src/hpotk/util/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      510 2024-04-12 19:43:26.000000 hpo_toolkit-0.5.1/src/hpotk/util/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     5501 2024-04-12 20:11:21.000000 hpo_toolkit-0.5.1/src/hpotk/util/_io.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     1129 2024-03-21 19:39:52.000000 hpo_toolkit-0.5.1/src/hpotk/util/_log.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     1490 2023-09-01 00:28:55.000000 hpo_toolkit-0.5.1/src/hpotk/util/_validate.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2024-05-20 17:13:09.199904 hpo_toolkit-0.5.1/src/hpotk/util/sort/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      413 2023-12-15 16:24:39.000000 hpo_toolkit-0.5.1/src/hpotk/util/sort/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      614 2023-09-01 15:29:00.000000 hpo_toolkit-0.5.1/src/hpotk/util/sort/_api.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)    12575 2023-12-15 16:13:38.000000 hpo_toolkit-0.5.1/src/hpotk/util/sort/_hierarchical.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     6185 2023-12-15 16:05:24.000000 hpo_toolkit-0.5.1/src/hpotk/util/sort/_test__hierarchical.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2024-05-20 17:13:09.199904 hpo_toolkit-0.5.1/src/hpotk/validate/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      517 2023-08-19 00:46:45.000000 hpo_toolkit-0.5.1/src/hpotk/validate/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     7782 2023-08-19 00:58:27.000000 hpo_toolkit-0.5.1/src/hpotk/validate/_hpo.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     3386 2023-12-05 04:09:32.000000 hpo_toolkit-0.5.1/src/hpotk/validate/_model.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     1909 2023-06-12 17:28:47.000000 hpo_toolkit-0.5.1/src/hpotk/validate/_util.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2024-05-20 17:13:09.199904 hpo_toolkit-0.5.1/tests/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     2311 2024-03-13 14:06:38.000000 hpo_toolkit-0.5.1/tests/test_obographs.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     3460 2024-05-20 16:54:42.000000 hpo_toolkit-0.5.1/tests/test_store.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     4582 2024-03-13 14:06:38.000000 hpo_toolkit-0.5.1/tests/test_term.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     2968 2023-12-04 15:57:34.000000 hpo_toolkit-0.5.1/tests/test_term_id.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     7854 2024-02-09 20:27:10.000000 hpo_toolkit-0.5.1/tests/test_validate.py
```

### Comparing `hpo-toolkit-0.5.0/LICENSE` & `hpo_toolkit-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/PKG-INFO` & `hpo_toolkit-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpo-toolkit
-Version: 0.5.0
+Version: 0.5.1
 Summary: A toolkit for working with Human Phenotype Ontology in Python
 Author-email: Daniel Danis <daniel.gordon.danis@protonmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -674,41 +674,46 @@
           The GNU General Public License does not permit incorporating your program
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
-Project-URL: Repository, https://github.com/TheJacksonLaboratory/hpo-toolkit
+Project-URL: homepage, https://github.com/ielis/hpo-toolkit
+Project-URL: repository, https://github.com/ielis/hpo-toolkit.git
+Project-URL: documentation, https://ielis.github.io/hpo-toolkit/stable
+Project-URL: bugtracker, https://github.com/ielis/hpo-toolkit/issues
 Keywords: human phenotype ontology,HPO,library
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.23
+Requires-Dist: certifi
 Provides-Extra: test
 Requires-Dist: pytest<9.0.0,>=8.0.0; extra == "test"
 Requires-Dist: ddt>=1.6.0; extra == "test"
 Provides-Extra: docs
 Requires-Dist: sphinx>=7.0.0; extra == "docs"
 Requires-Dist: sphinx-copybutton>=0.5.0; extra == "docs"
 Requires-Dist: sphinx-rtd-theme>=1.3.0; extra == "docs"
 Provides-Extra: bench
 Requires-Dist: pandas<3.0,>=1.0.0; extra == "bench"
 
 # hpo-toolkit
 
-![Build status](https://img.shields.io/github/actions/workflow/status/TheJacksonLaboratory/hpo-toolkit/python_ci.yml)
-![PyPi downloads](https://img.shields.io/pypi/dm/hpo-toolkit.svg?label=Pypi%20downloads)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hpo-toolkit)
+![PyPi downloads](https://img.shields.io/pypi/dm/hpo-toolkit.svg?label=Pypi%20downloads)
+![Build status](https://img.shields.io/github/actions/workflow/status/ielis/hpo-toolkit/python_ci.yml)
+[![GitHub release](https://img.shields.io/github/release/ielis/hpo-toolkit.svg)](https://github.com/ielis/hpo-toolkit/releases)
 
 A toolkit for working with Human Phenotype Ontology (HPO) and HPO disease annotations in Python.
 
 ## Example
 
 Loading HPO is as simple as:
 
@@ -736,9 +741,9 @@
 
 You got yourself phenotype annotations of 12,468 rare diseases.
 
 ## Learn more
 
 Find more info in our detailed documentation:
 
-- [Stable documentation](https://thejacksonlaboratory.github.io/hpo-toolkit/stable) (last release on `main` branch)
-- [Latest documentation](https://thejacksonlaboratory.github.io/hpo-toolkit/latest) (bleeding edge, latest commit on `development` branch)
+- [Stable documentation](https://ielis.github.io/hpo-toolkit/stable) (last release on `main` branch)
+- [Latest documentation](https://ielis.github.io/hpo-toolkit/latest) (bleeding edge, latest commit on `development` branch)
```

### Comparing `hpo-toolkit-0.5.0/README.md` & `hpo_toolkit-0.5.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # hpo-toolkit
 
-![Build status](https://img.shields.io/github/actions/workflow/status/TheJacksonLaboratory/hpo-toolkit/python_ci.yml)
-![PyPi downloads](https://img.shields.io/pypi/dm/hpo-toolkit.svg?label=Pypi%20downloads)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hpo-toolkit)
+![PyPi downloads](https://img.shields.io/pypi/dm/hpo-toolkit.svg?label=Pypi%20downloads)
+![Build status](https://img.shields.io/github/actions/workflow/status/ielis/hpo-toolkit/python_ci.yml)
+[![GitHub release](https://img.shields.io/github/release/ielis/hpo-toolkit.svg)](https://github.com/ielis/hpo-toolkit/releases)
 
 A toolkit for working with Human Phenotype Ontology (HPO) and HPO disease annotations in Python.
 
 ## Example
 
 Loading HPO is as simple as:
 
@@ -34,9 +35,9 @@
 
 You got yourself phenotype annotations of 12,468 rare diseases.
 
 ## Learn more
 
 Find more info in our detailed documentation:
 
-- [Stable documentation](https://thejacksonlaboratory.github.io/hpo-toolkit/stable) (last release on `main` branch)
-- [Latest documentation](https://thejacksonlaboratory.github.io/hpo-toolkit/latest) (bleeding edge, latest commit on `development` branch)
+- [Stable documentation](https://ielis.github.io/hpo-toolkit/stable) (last release on `main` branch)
+- [Latest documentation](https://ielis.github.io/hpo-toolkit/latest) (bleeding edge, latest commit on `development` branch)
```

### Comparing `hpo-toolkit-0.5.0/pyproject.toml` & `hpo_toolkit-0.5.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -20,15 +20,16 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dynamic = ["version"]
 
 dependencies = [
-    "numpy >= 1.23"
+    "numpy >= 1.23",
+    "certifi", # The latest version is the best.
 ]
 
 [project.optional-dependencies]
 test = [
     "pytest>=8.0.0, <9.0.0",
     "ddt >= 1.6.0",  # TODO: remove after finishing the migration to `pytest`!
 ]
@@ -36,15 +37,18 @@
     "sphinx>=7.0.0", "sphinx-copybutton>=0.5.0", "sphinx-rtd-theme>=1.3.0",
 ]
 bench = [
     'pandas >= 1.0.0, <3.0',
 ]
 
 [project.urls]
-"Repository" = "https://github.com/TheJacksonLaboratory/hpo-toolkit"
+homepage = "https://github.com/ielis/hpo-toolkit"
+repository = "https://github.com/ielis/hpo-toolkit.git"
+documentation = "https://ielis.github.io/hpo-toolkit/stable"
+bugtracker = "https://github.com/ielis/hpo-toolkit/issues"
 
 [tool.setuptools]
 package-dir = { "" = "src" }
 zip-safe = false
 
 [tool.setuptools.dynamic]
 version = { attr = "hpotk.__version__" }
```

### Comparing `hpo-toolkit-0.5.0/src/hpo_toolkit.egg-info/PKG-INFO` & `hpo_toolkit-0.5.1/src/hpo_toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpo-toolkit
-Version: 0.5.0
+Version: 0.5.1
 Summary: A toolkit for working with Human Phenotype Ontology in Python
 Author-email: Daniel Danis <daniel.gordon.danis@protonmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -674,41 +674,46 @@
           The GNU General Public License does not permit incorporating your program
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
-Project-URL: Repository, https://github.com/TheJacksonLaboratory/hpo-toolkit
+Project-URL: homepage, https://github.com/ielis/hpo-toolkit
+Project-URL: repository, https://github.com/ielis/hpo-toolkit.git
+Project-URL: documentation, https://ielis.github.io/hpo-toolkit/stable
+Project-URL: bugtracker, https://github.com/ielis/hpo-toolkit/issues
 Keywords: human phenotype ontology,HPO,library
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.23
+Requires-Dist: certifi
 Provides-Extra: test
 Requires-Dist: pytest<9.0.0,>=8.0.0; extra == "test"
 Requires-Dist: ddt>=1.6.0; extra == "test"
 Provides-Extra: docs
 Requires-Dist: sphinx>=7.0.0; extra == "docs"
 Requires-Dist: sphinx-copybutton>=0.5.0; extra == "docs"
 Requires-Dist: sphinx-rtd-theme>=1.3.0; extra == "docs"
 Provides-Extra: bench
 Requires-Dist: pandas<3.0,>=1.0.0; extra == "bench"
 
 # hpo-toolkit
 
-![Build status](https://img.shields.io/github/actions/workflow/status/TheJacksonLaboratory/hpo-toolkit/python_ci.yml)
-![PyPi downloads](https://img.shields.io/pypi/dm/hpo-toolkit.svg?label=Pypi%20downloads)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hpo-toolkit)
+![PyPi downloads](https://img.shields.io/pypi/dm/hpo-toolkit.svg?label=Pypi%20downloads)
+![Build status](https://img.shields.io/github/actions/workflow/status/ielis/hpo-toolkit/python_ci.yml)
+[![GitHub release](https://img.shields.io/github/release/ielis/hpo-toolkit.svg)](https://github.com/ielis/hpo-toolkit/releases)
 
 A toolkit for working with Human Phenotype Ontology (HPO) and HPO disease annotations in Python.
 
 ## Example
 
 Loading HPO is as simple as:
 
@@ -736,9 +741,9 @@
 
 You got yourself phenotype annotations of 12,468 rare diseases.
 
 ## Learn more
 
 Find more info in our detailed documentation:
 
-- [Stable documentation](https://thejacksonlaboratory.github.io/hpo-toolkit/stable) (last release on `main` branch)
-- [Latest documentation](https://thejacksonlaboratory.github.io/hpo-toolkit/latest) (bleeding edge, latest commit on `development` branch)
+- [Stable documentation](https://ielis.github.io/hpo-toolkit/stable) (last release on `main` branch)
+- [Latest documentation](https://ielis.github.io/hpo-toolkit/latest) (bleeding edge, latest commit on `development` branch)
```

### Comparing `hpo-toolkit-0.5.0/src/hpo_toolkit.egg-info/SOURCES.txt` & `hpo_toolkit-0.5.1/src/hpo_toolkit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -57,26 +57,26 @@
 src/hpotk/ontology/_default.py
 src/hpotk/ontology/load/__init__.py
 src/hpotk/ontology/load/obographs/__init__.py
 src/hpotk/ontology/load/obographs/_factory.py
 src/hpotk/ontology/load/obographs/_load.py
 src/hpotk/ontology/load/obographs/_model.py
 src/hpotk/ontology/load/obographs/_test_load.py
+src/hpotk/store/__init__.py
+src/hpotk/store/_api.py
+src/hpotk/store/_config.py
+src/hpotk/store/_github.py
 src/hpotk/util/__init__.py
 src/hpotk/util/_io.py
 src/hpotk/util/_log.py
 src/hpotk/util/_validate.py
 src/hpotk/util/sort/__init__.py
 src/hpotk/util/sort/_api.py
 src/hpotk/util/sort/_hierarchical.py
 src/hpotk/util/sort/_test__hierarchical.py
-src/hpotk/util/store/__init__.py
-src/hpotk/util/store/_api.py
-src/hpotk/util/store/_config.py
-src/hpotk/util/store/_github.py
 src/hpotk/validate/__init__.py
 src/hpotk/validate/_hpo.py
 src/hpotk/validate/_model.py
 src/hpotk/validate/_util.py
 tests/test_obographs.py
 tests/test_store.py
 tests/test_term.py
```

### Comparing `hpo-toolkit-0.5.0/src/hpotk/__init__.py` & `hpo_toolkit-0.5.1/src/hpotk/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """
 HPO toolkit is a library for working with Human Phenotype Ontology and the HPO annotation data.
 """
 
-__version__ = "0.5.0"
+__version__ = '0.5.1'
 
 from . import algorithm
 from . import annotations
 from . import constants
 from . import graph
 from . import model
 from . import ontology
+from . import store
 from . import util
 from . import validate
 
 from .graph import OntologyGraph, GraphAware
 from .model import TermId, Term, MinimalTerm, Synonym, SynonymType, SynonymCategory
 from .ontology import Ontology, MinimalOntology
 
 from .ontology.load.obographs import load_minimal_ontology, load_ontology
-from .util.store import OntologyType, OntologyStore, configure_ontology_store
+from .store import OntologyType, OntologyStore, configure_ontology_store
```

### Comparing `hpo-toolkit-0.5.0/src/hpotk/algorithm/_augment.py` & `hpo_toolkit-0.5.1/src/hpotk/algorithm/_augment.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/algorithm/_traversal.py` & `hpo_toolkit-0.5.1/src/hpotk/algorithm/_traversal.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/algorithm/similarity/_ic.py` & `hpo_toolkit-0.5.1/src/hpotk/algorithm/similarity/_ic.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/algorithm/similarity/_model.py` & `hpo_toolkit-0.5.1/src/hpotk/algorithm/similarity/_model.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/algorithm/similarity/_resnik.py` & `hpo_toolkit-0.5.1/src/hpotk/algorithm/similarity/_resnik.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/annotations/__init__.py` & `hpo_toolkit-0.5.1/src/hpotk/annotations/__init__.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/annotations/_api.py` & `hpo_toolkit-0.5.1/src/hpotk/annotations/_api.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/annotations/_base.py` & `hpo_toolkit-0.5.1/src/hpotk/annotations/_base.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/annotations/_simple.py` & `hpo_toolkit-0.5.1/src/hpotk/annotations/_simple.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/annotations/_test__simple.py` & `hpo_toolkit-0.5.1/src/hpotk/annotations/_test__simple.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/annotations/load/hpoa/_impl.py` & `hpo_toolkit-0.5.1/src/hpotk/annotations/load/hpoa/_impl.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/annotations/load/hpoa/_test__impl.py` & `hpo_toolkit-0.5.1/src/hpotk/annotations/load/hpoa/_test__impl.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/constants/hpo/base.py` & `hpo_toolkit-0.5.1/src/hpotk/constants/hpo/base.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/constants/hpo/frequency.py` & `hpo_toolkit-0.5.1/src/hpotk/constants/hpo/frequency.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/constants/hpo/inheritance.py` & `hpo_toolkit-0.5.1/src/hpotk/constants/hpo/inheritance.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/constants/hpo/onset.py` & `hpo_toolkit-0.5.1/src/hpotk/constants/hpo/onset.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/constants/hpo/organ_system.py` & `hpo_toolkit-0.5.1/src/hpotk/constants/hpo/organ_system.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/graph/_api.py` & `hpo_toolkit-0.5.1/src/hpotk/graph/_api.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/graph/_csr_graph.py` & `hpo_toolkit-0.5.1/src/hpotk/graph/_csr_graph.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/graph/_csr_idx_graph.py` & `hpo_toolkit-0.5.1/src/hpotk/graph/_csr_idx_graph.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/graph/_factory.py` & `hpo_toolkit-0.5.1/src/hpotk/graph/_factory.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/graph/_test__api.py` & `hpo_toolkit-0.5.1/src/hpotk/graph/_test__api.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/graph/_test__csr_graph.py` & `hpo_toolkit-0.5.1/src/hpotk/graph/_test__csr_graph.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/graph/_test__factory.py` & `hpo_toolkit-0.5.1/src/hpotk/graph/_test__factory.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/graph/_test_csr_idx_graph.py` & `hpo_toolkit-0.5.1/src/hpotk/graph/_test_csr_idx_graph.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/graph/_test_data.py` & `hpo_toolkit-0.5.1/src/hpotk/graph/_test_data.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/graph/csr/_csr.py` & `hpo_toolkit-0.5.1/src/hpotk/graph/csr/_csr.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/graph/csr/_test__csr.py` & `hpo_toolkit-0.5.1/src/hpotk/graph/csr/_test__csr.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/model/__init__.py` & `hpo_toolkit-0.5.1/src/hpotk/model/__init__.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/model/_base.py` & `hpo_toolkit-0.5.1/src/hpotk/model/_base.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/model/_term.py` & `hpo_toolkit-0.5.1/src/hpotk/model/_term.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/model/_term_id.py` & `hpo_toolkit-0.5.1/src/hpotk/model/_term_id.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/model/_test__term_id.py` & `hpo_toolkit-0.5.1/src/hpotk/model/_test__term_id.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/ontology/_default.py` & `hpo_toolkit-0.5.1/src/hpotk/ontology/_default.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/ontology/load/obographs/_factory.py` & `hpo_toolkit-0.5.1/src/hpotk/ontology/load/obographs/_factory.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/ontology/load/obographs/_load.py` & `hpo_toolkit-0.5.1/src/hpotk/ontology/load/obographs/_load.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/ontology/load/obographs/_model.py` & `hpo_toolkit-0.5.1/src/hpotk/ontology/load/obographs/_model.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/ontology/load/obographs/_test_load.py` & `hpo_toolkit-0.5.1/src/hpotk/ontology/load/obographs/_test_load.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/util/_io.py` & `hpo_toolkit-0.5.1/src/hpotk/util/_io.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import gzip
 import io
 import logging
+import ssl
 import sys
 import typing
 import warnings
 from urllib.request import urlopen
 
+import certifi
+
 
 def looks_like_url(file: str) -> bool:
     """
    Checks if the `file` looks like a URL.
 
    :param file: file to check.
    :return: `True` if the `file` starts with `http://` or `https://`.
@@ -32,17 +35,19 @@
         encoding = sys.getdefaultencoding()
         logger.debug(f'Using default encoding \'{encoding}\'')
     else:
         logger.debug(f'Using provided encoding \'{encoding}\'')
     return encoding
 
 
-def open_text_io_handle_for_reading(fh: typing.Union[typing.IO, str],
-                                    timeout: int = 30,
-                                    encoding: str = None) -> typing.TextIO:
+def open_text_io_handle_for_reading(
+        fh: typing.Union[typing.IO, str],
+        timeout: int = 30,
+        encoding: str = None,
+) -> typing.TextIO:
     """
     Open a `io.TextIO` file handle based on `fh`.
 
     :param fh: a `str` or `typing.IO` to read from. If `str`, then it should be a path to a local file or a URL
       of a remote resource. Either `http` or `https` protocols are supported. The content will be uncompressed
       on the fly if the file name ends with `.gz`. If `fh` is an IO wrapper, the function ensures we get a text wrapper
       that uses given encoding.
@@ -53,19 +58,24 @@
     logger = logging.getLogger('hpotk.util')
     encoding = _parse_encoding(encoding, logger)
 
     logger.debug(f'Opening {fh}')
     if isinstance(fh, str):
         # Can be a path to local file or URL
         if looks_like_url(fh):
+            ctx = ssl.create_default_context(cafile=certifi.where())
             logger.debug(f'Looks like a URL: {fh}')
             if not isinstance(timeout, int) or timeout <= 0:
                 raise ValueError(f'If {fh} looks like URL then timeout {timeout} must be a positive `int`')
             logger.debug(f'Downloading with timeout={timeout}s')
-            handle = urlopen(fh, timeout=timeout)
+            handle = urlopen(
+                fh,
+                timeout=timeout,
+                context=ctx,
+            )
         else:
             logger.debug(f'Looks like a local file: {fh}')
             handle = open(fh, 'rb')
 
         if looks_gzipped(fh):
             logger.debug(f'Looks like a gzipped data, decompressing on the fly')
             return gzip.open(handle, mode='rt', newline='', encoding=encoding)
```

### Comparing `hpo-toolkit-0.5.0/src/hpotk/util/_log.py` & `hpo_toolkit-0.5.1/src/hpotk/util/_log.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 import logging
+import typing
 
 DEFAULT_LOG_FMT = '%(asctime)s %(name)-20s %(levelname)-3s : %(message)s'
 
 
-def setup_logging(level: int = logging.INFO,
-                  log_fmt: str = DEFAULT_LOG_FMT):
+def setup_logging(
+        level: int = logging.INFO,
+        log_fmt: str = DEFAULT_LOG_FMT,
+        stream: typing.Optional[typing.TextIO] = None,
+):
     """
     Create a basic configuration for the logging library. Set up console and file handler using provided `log_fmt`.
 
     The `level` signifies the desired verbosity.
     Use:
 
     - `10` for `DEBUG`
     - `20` for `INFO`
     - `30` for `WARNING`
     - `40` for `ERROR`
     - `50` for `CRITICAL`
 
     :param level: the verbosity to use, `INFO` by default.
     :param log_fmt: format string for logging.
+    :param stream: stream to write to. Will default to `sys.stderr` if `None`.
     """
     # create logger
     logger = logging.getLogger()
     logger.setLevel(level)
     # create console handler and set level to debug
-    ch = logging.StreamHandler()
+    ch = logging.StreamHandler(stream=stream)
     ch.setLevel(level)
     # create formatter
     formatter = logging.Formatter(log_fmt)
     # add formatter to ch
     ch.setFormatter(formatter)
     # add ch to logger
     logger.addHandler(ch)
```

### Comparing `hpo-toolkit-0.5.0/src/hpotk/util/_validate.py` & `hpo_toolkit-0.5.1/src/hpotk/util/_validate.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/util/sort/_api.py` & `hpo_toolkit-0.5.1/src/hpotk/util/sort/_api.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/util/sort/_hierarchical.py` & `hpo_toolkit-0.5.1/src/hpotk/util/sort/_hierarchical.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/util/sort/_test__hierarchical.py` & `hpo_toolkit-0.5.1/src/hpotk/util/sort/_test__hierarchical.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/validate/__init__.py` & `hpo_toolkit-0.5.1/src/hpotk/validate/__init__.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/validate/_hpo.py` & `hpo_toolkit-0.5.1/src/hpotk/validate/_hpo.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/validate/_model.py` & `hpo_toolkit-0.5.1/src/hpotk/validate/_model.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/src/hpotk/validate/_util.py` & `hpo_toolkit-0.5.1/src/hpotk/validate/_util.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/tests/test_obographs.py` & `hpo_toolkit-0.5.1/tests/test_obographs.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/tests/test_term.py` & `hpo_toolkit-0.5.1/tests/test_term.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/tests/test_term_id.py` & `hpo_toolkit-0.5.1/tests/test_term_id.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.5.0/tests/test_validate.py` & `hpo_toolkit-0.5.1/tests/test_validate.py`

 * *Files identical despite different names*

