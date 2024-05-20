# Comparing `tmp/fluke_fl-0.0.2.tar.gz` & `tmp/fluke_fl-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluke_fl-0.0.2.tar", last modified: Fri May 17 15:57:55 2024, max compression
+gzip compressed data, was "fluke_fl-0.0.3.tar", last modified: Mon May 20 07:51:21 2024, max compression
```

## Comparing `fluke_fl-0.0.2.tar` & `fluke_fl-0.0.3.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 mirko      (501) staff       (20)        0 2024-05-17 15:57:55.823469 fluke_fl-0.0.2/
--rw-r--r--   0 mirko      (501) staff       (20)    26083 2024-05-16 12:16:36.000000 fluke_fl-0.0.2/LICENSE
--rw-r--r--   0 mirko      (501) staff       (20)    34254 2024-05-17 15:57:55.823192 fluke_fl-0.0.2/PKG-INFO
--rw-r--r--   0 mirko      (501) staff       (20)     3023 2024-05-17 15:39:28.000000 fluke_fl-0.0.2/README.md
-drwxr-xr-x   0 mirko      (501) staff       (20)        0 2024-05-17 15:57:55.814308 fluke_fl-0.0.2/fluke/
--rw-r--r--   0 mirko      (501) staff       (20)     8675 2024-05-16 11:01:26.000000 fluke_fl-0.0.2/fluke/__init__.py
-drwxr-xr-x   0 mirko      (501) staff       (20)        0 2024-05-17 15:57:55.818832 fluke_fl-0.0.2/fluke/algorithms/
--rw-r--r--   0 mirko      (501) staff       (20)     9448 2024-05-16 13:37:43.000000 fluke_fl-0.0.2/fluke/algorithms/__init__.py
--rw-r--r--   0 mirko      (501) staff       (20)     3711 2024-05-16 11:01:26.000000 fluke_fl-0.0.2/fluke/algorithms/apfl.py
--rw-r--r--   0 mirko      (501) staff       (20)     5907 2024-05-17 07:28:01.000000 fluke_fl-0.0.2/fluke/algorithms/ccvr.py
--rw-r--r--   0 mirko      (501) staff       (20)     3250 2024-05-16 11:01:26.000000 fluke_fl-0.0.2/fluke/algorithms/ditto.py
--rw-r--r--   0 mirko      (501) staff       (20)     5018 2024-05-16 11:01:26.000000 fluke_fl-0.0.2/fluke/algorithms/fedamp.py
--rw-r--r--   0 mirko      (501) staff       (20)      496 2024-04-23 11:33:36.000000 fluke_fl-0.0.2/fluke/algorithms/fedavg.py
--rw-r--r--   0 mirko      (501) staff       (20)     1893 2024-05-16 11:01:26.000000 fluke_fl-0.0.2/fluke/algorithms/fedavgm.py
--rw-r--r--   0 mirko      (501) staff       (20)     4089 2024-05-17 07:29:44.000000 fluke_fl-0.0.2/fluke/algorithms/fedbabu.py
--rw-r--r--   0 mirko      (501) staff       (20)     1333 2024-05-16 11:01:26.000000 fluke_fl-0.0.2/fluke/algorithms/fedbn.py
--rwxr-xr-x   0 mirko      (501) staff       (20)     7466 2024-05-17 07:32:27.000000 fluke_fl-0.0.2/fluke/algorithms/feddyn.py
--rw-r--r--   0 mirko      (501) staff       (20)     1931 2024-05-16 11:01:26.000000 fluke_fl-0.0.2/fluke/algorithms/fedexp.py
--rw-r--r--   0 mirko      (501) staff       (20)     6855 2024-05-16 11:01:26.000000 fluke_fl-0.0.2/fluke/algorithms/fedhp.py
--rw-r--r--   0 mirko      (501) staff       (20)     1746 2024-05-16 11:01:26.000000 fluke_fl-0.0.2/fluke/algorithms/fedlc.py
--rw-r--r--   0 mirko      (501) staff       (20)     9164 2024-05-16 11:01:26.000000 fluke_fl-0.0.2/fluke/algorithms/fednh.py
--rw-r--r--   0 mirko      (501) staff       (20)     2723 2024-05-16 11:01:26.000000 fluke_fl-0.0.2/fluke/algorithms/fednova.py
--rw-r--r--   0 mirko      (501) staff       (20)     3536 2024-05-16 12:28:24.000000 fluke_fl-0.0.2/fluke/algorithms/fedopt.py
--rw-r--r--   0 mirko      (501) staff       (20)     1968 2024-05-16 11:01:26.000000 fluke_fl-0.0.2/fluke/algorithms/fedper.py
--rw-r--r--   0 mirko      (501) staff       (20)     7053 2024-05-16 11:01:26.000000 fluke_fl-0.0.2/fluke/algorithms/fedproto.py
--rw-r--r--   0 mirko      (501) staff       (20)     2075 2024-05-16 11:01:26.000000 fluke_fl-0.0.2/fluke/algorithms/fedprox.py
--rw-r--r--   0 mirko      (501) staff       (20)     4047 2024-05-16 11:01:26.000000 fluke_fl-0.0.2/fluke/algorithms/fedrep.py
--rw-r--r--   0 mirko      (501) staff       (20)      870 2024-05-16 11:01:26.000000 fluke_fl-0.0.2/fluke/algorithms/fedsgd.py
--rw-r--r--   0 mirko      (501) staff       (20)     2235 2024-05-16 11:01:26.000000 fluke_fl-0.0.2/fluke/algorithms/lg_fedavg.py
--rw-r--r--   0 mirko      (501) staff       (20)     3233 2024-05-16 11:01:26.000000 fluke_fl-0.0.2/fluke/algorithms/moon.py
--rw-r--r--   0 mirko      (501) staff       (20)     5686 2024-05-17 10:05:44.000000 fluke_fl-0.0.2/fluke/algorithms/per_fedavg.py
--rw-r--r--   0 mirko      (501) staff       (20)     5090 2024-05-16 11:01:26.000000 fluke_fl-0.0.2/fluke/algorithms/pfedme.py
--rw-r--r--   0 mirko      (501) staff       (20)     7374 2024-05-16 11:01:26.000000 fluke_fl-0.0.2/fluke/algorithms/scaffold.py
--rw-r--r--   0 mirko      (501) staff       (20)     5580 2024-05-16 11:01:26.000000 fluke_fl-0.0.2/fluke/algorithms/superfed.py
--rw-r--r--   0 mirko      (501) staff       (20)    11592 2024-05-16 11:01:26.000000 fluke_fl-0.0.2/fluke/client.py
--rw-r--r--   0 mirko      (501) staff       (20)    10376 2024-05-16 11:01:26.000000 fluke_fl-0.0.2/fluke/comm.py
-drwxr-xr-x   0 mirko      (501) staff       (20)        0 2024-05-17 15:57:55.819323 fluke_fl-0.0.2/fluke/data/
--rw-r--r--   0 mirko      (501) staff       (20)    34120 2024-05-16 12:25:40.000000 fluke_fl-0.0.2/fluke/data/__init__.py
--rw-r--r--   0 mirko      (501) staff       (20)    32234 2024-05-16 11:01:26.000000 fluke_fl-0.0.2/fluke/data/datasets.py
--rw-r--r--   0 mirko      (501) staff       (20)     6875 2024-05-17 12:07:25.000000 fluke_fl-0.0.2/fluke/data/support.py
--rw-r--r--   0 mirko      (501) staff       (20)     7167 2024-05-16 11:01:26.000000 fluke_fl-0.0.2/fluke/evaluation.py
--rw-r--r--   0 mirko      (501) staff       (20)    43792 2024-05-17 08:15:27.000000 fluke_fl-0.0.2/fluke/nets.py
--rw-r--r--   0 mirko      (501) staff       (20)     7075 2024-05-16 12:56:17.000000 fluke_fl-0.0.2/fluke/run.py
--rw-r--r--   0 mirko      (501) staff       (20)    15016 2024-05-16 11:01:26.000000 fluke_fl-0.0.2/fluke/server.py
-drwxr-xr-x   0 mirko      (501) staff       (20)        0 2024-05-17 15:57:55.819634 fluke_fl-0.0.2/fluke/utils/
--rw-r--r--   0 mirko      (501) staff       (20)    22022 2024-05-17 07:33:13.000000 fluke_fl-0.0.2/fluke/utils/__init__.py
--rw-r--r--   0 mirko      (501) staff       (20)    23035 2024-05-17 12:17:19.000000 fluke_fl-0.0.2/fluke/utils/model.py
-drwxr-xr-x   0 mirko      (501) staff       (20)        0 2024-05-17 15:57:55.822826 fluke_fl-0.0.2/fluke_fl.egg-info/
--rw-r--r--   0 mirko      (501) staff       (20)    34254 2024-05-17 15:57:55.000000 fluke_fl-0.0.2/fluke_fl.egg-info/PKG-INFO
--rw-r--r--   0 mirko      (501) staff       (20)     1385 2024-05-17 15:57:55.000000 fluke_fl-0.0.2/fluke_fl.egg-info/SOURCES.txt
--rw-r--r--   0 mirko      (501) staff       (20)        1 2024-05-17 15:57:55.000000 fluke_fl-0.0.2/fluke_fl.egg-info/dependency_links.txt
--rw-r--r--   0 mirko      (501) staff       (20)       41 2024-05-17 15:57:55.000000 fluke_fl-0.0.2/fluke_fl.egg-info/entry_points.txt
--rw-r--r--   0 mirko      (501) staff       (20)       96 2024-05-17 15:57:55.000000 fluke_fl-0.0.2/fluke_fl.egg-info/requires.txt
--rw-r--r--   0 mirko      (501) staff       (20)        6 2024-05-17 15:57:55.000000 fluke_fl-0.0.2/fluke_fl.egg-info/top_level.txt
--rw-r--r--   0 mirko      (501) staff       (20)     1699 2024-05-17 15:57:40.000000 fluke_fl-0.0.2/pyproject.toml
--rw-r--r--   0 mirko      (501) staff       (20)       38 2024-05-17 15:57:55.823528 fluke_fl-0.0.2/setup.cfg
-drwxr-xr-x   0 mirko      (501) staff       (20)        0 2024-05-17 15:57:55.822610 fluke_fl-0.0.2/tests/
--rw-r--r--   0 mirko      (501) staff       (20)    10293 2024-05-17 10:06:41.000000 fluke_fl-0.0.2/tests/test_alg.py
--rw-r--r--   0 mirko      (501) staff       (20)     4397 2024-05-16 11:01:26.000000 fluke_fl-0.0.2/tests/test_client.py
--rw-r--r--   0 mirko      (501) staff       (20)     3331 2024-05-16 11:01:26.000000 fluke_fl-0.0.2/tests/test_comm.py
--rw-r--r--   0 mirko      (501) staff       (20)     2130 2024-05-16 11:01:26.000000 fluke_fl-0.0.2/tests/test_core.py
--rw-r--r--   0 mirko      (501) staff       (20)    11108 2024-05-16 11:01:26.000000 fluke_fl-0.0.2/tests/test_data.py
--rw-r--r--   0 mirko      (501) staff       (20)    12738 2024-05-17 12:09:41.000000 fluke_fl-0.0.2/tests/test_datasets.py
--rw-r--r--   0 mirko      (501) staff       (20)     2895 2024-05-16 11:01:26.000000 fluke_fl-0.0.2/tests/test_eval.py
--rw-r--r--   0 mirko      (501) staff       (20)     4620 2024-05-16 11:01:26.000000 fluke_fl-0.0.2/tests/test_nets.py
--rw-r--r--   0 mirko      (501) staff       (20)     3716 2024-05-16 11:01:26.000000 fluke_fl-0.0.2/tests/test_server.py
--rw-r--r--   0 mirko      (501) staff       (20)    13910 2024-05-17 12:13:40.000000 fluke_fl-0.0.2/tests/test_utils.py
+drwxr-xr-x   0 mirko      (501) staff       (20)        0 2024-05-20 07:51:21.499642 fluke_fl-0.0.3/
+-rw-r--r--   0 mirko      (501) staff       (20)    26083 2024-05-16 12:16:36.000000 fluke_fl-0.0.3/LICENSE
+-rw-r--r--   0 mirko      (501) staff       (20)    34816 2024-05-20 07:51:21.499360 fluke_fl-0.0.3/PKG-INFO
+-rw-r--r--   0 mirko      (501) staff       (20)     3585 2024-05-20 06:05:54.000000 fluke_fl-0.0.3/README.md
+drwxr-xr-x   0 mirko      (501) staff       (20)        0 2024-05-20 07:51:21.490369 fluke_fl-0.0.3/fluke/
+-rw-r--r--   0 mirko      (501) staff       (20)     8675 2024-05-16 11:01:26.000000 fluke_fl-0.0.3/fluke/__init__.py
+drwxr-xr-x   0 mirko      (501) staff       (20)        0 2024-05-20 07:51:21.495194 fluke_fl-0.0.3/fluke/algorithms/
+-rw-r--r--   0 mirko      (501) staff       (20)     9448 2024-05-16 13:37:43.000000 fluke_fl-0.0.3/fluke/algorithms/__init__.py
+-rw-r--r--   0 mirko      (501) staff       (20)     3711 2024-05-16 11:01:26.000000 fluke_fl-0.0.3/fluke/algorithms/apfl.py
+-rw-r--r--   0 mirko      (501) staff       (20)     5907 2024-05-17 07:28:01.000000 fluke_fl-0.0.3/fluke/algorithms/ccvr.py
+-rw-r--r--   0 mirko      (501) staff       (20)     3250 2024-05-16 11:01:26.000000 fluke_fl-0.0.3/fluke/algorithms/ditto.py
+-rw-r--r--   0 mirko      (501) staff       (20)     5018 2024-05-16 11:01:26.000000 fluke_fl-0.0.3/fluke/algorithms/fedamp.py
+-rw-r--r--   0 mirko      (501) staff       (20)      496 2024-04-23 11:33:36.000000 fluke_fl-0.0.3/fluke/algorithms/fedavg.py
+-rw-r--r--   0 mirko      (501) staff       (20)     1893 2024-05-16 11:01:26.000000 fluke_fl-0.0.3/fluke/algorithms/fedavgm.py
+-rw-r--r--   0 mirko      (501) staff       (20)     4089 2024-05-17 07:29:44.000000 fluke_fl-0.0.3/fluke/algorithms/fedbabu.py
+-rw-r--r--   0 mirko      (501) staff       (20)     1333 2024-05-16 11:01:26.000000 fluke_fl-0.0.3/fluke/algorithms/fedbn.py
+-rwxr-xr-x   0 mirko      (501) staff       (20)     7466 2024-05-17 07:32:27.000000 fluke_fl-0.0.3/fluke/algorithms/feddyn.py
+-rw-r--r--   0 mirko      (501) staff       (20)     1914 2024-05-19 10:47:03.000000 fluke_fl-0.0.3/fluke/algorithms/fedexp.py
+-rw-r--r--   0 mirko      (501) staff       (20)     6855 2024-05-16 11:01:26.000000 fluke_fl-0.0.3/fluke/algorithms/fedhp.py
+-rw-r--r--   0 mirko      (501) staff       (20)     1746 2024-05-16 11:01:26.000000 fluke_fl-0.0.3/fluke/algorithms/fedlc.py
+-rw-r--r--   0 mirko      (501) staff       (20)     9164 2024-05-16 11:01:26.000000 fluke_fl-0.0.3/fluke/algorithms/fednh.py
+-rw-r--r--   0 mirko      (501) staff       (20)     2723 2024-05-16 11:01:26.000000 fluke_fl-0.0.3/fluke/algorithms/fednova.py
+-rw-r--r--   0 mirko      (501) staff       (20)     3536 2024-05-16 12:28:24.000000 fluke_fl-0.0.3/fluke/algorithms/fedopt.py
+-rw-r--r--   0 mirko      (501) staff       (20)     1968 2024-05-16 11:01:26.000000 fluke_fl-0.0.3/fluke/algorithms/fedper.py
+-rw-r--r--   0 mirko      (501) staff       (20)     7053 2024-05-16 11:01:26.000000 fluke_fl-0.0.3/fluke/algorithms/fedproto.py
+-rw-r--r--   0 mirko      (501) staff       (20)     2075 2024-05-16 11:01:26.000000 fluke_fl-0.0.3/fluke/algorithms/fedprox.py
+-rw-r--r--   0 mirko      (501) staff       (20)     4047 2024-05-16 11:01:26.000000 fluke_fl-0.0.3/fluke/algorithms/fedrep.py
+-rw-r--r--   0 mirko      (501) staff       (20)      870 2024-05-16 11:01:26.000000 fluke_fl-0.0.3/fluke/algorithms/fedsgd.py
+-rw-r--r--   0 mirko      (501) staff       (20)     2235 2024-05-16 11:01:26.000000 fluke_fl-0.0.3/fluke/algorithms/lg_fedavg.py
+-rw-r--r--   0 mirko      (501) staff       (20)     3233 2024-05-16 11:01:26.000000 fluke_fl-0.0.3/fluke/algorithms/moon.py
+-rw-r--r--   0 mirko      (501) staff       (20)     5686 2024-05-17 10:05:44.000000 fluke_fl-0.0.3/fluke/algorithms/per_fedavg.py
+-rw-r--r--   0 mirko      (501) staff       (20)     5090 2024-05-16 11:01:26.000000 fluke_fl-0.0.3/fluke/algorithms/pfedme.py
+-rw-r--r--   0 mirko      (501) staff       (20)     7374 2024-05-16 11:01:26.000000 fluke_fl-0.0.3/fluke/algorithms/scaffold.py
+-rw-r--r--   0 mirko      (501) staff       (20)     5580 2024-05-16 11:01:26.000000 fluke_fl-0.0.3/fluke/algorithms/superfed.py
+-rw-r--r--   0 mirko      (501) staff       (20)    11592 2024-05-16 11:01:26.000000 fluke_fl-0.0.3/fluke/client.py
+-rw-r--r--   0 mirko      (501) staff       (20)    10376 2024-05-16 11:01:26.000000 fluke_fl-0.0.3/fluke/comm.py
+drwxr-xr-x   0 mirko      (501) staff       (20)        0 2024-05-20 07:51:21.495759 fluke_fl-0.0.3/fluke/data/
+-rw-r--r--   0 mirko      (501) staff       (20)    34120 2024-05-16 12:25:40.000000 fluke_fl-0.0.3/fluke/data/__init__.py
+-rw-r--r--   0 mirko      (501) staff       (20)    32234 2024-05-16 11:01:26.000000 fluke_fl-0.0.3/fluke/data/datasets.py
+-rw-r--r--   0 mirko      (501) staff       (20)     6875 2024-05-17 12:07:25.000000 fluke_fl-0.0.3/fluke/data/support.py
+-rw-r--r--   0 mirko      (501) staff       (20)     7167 2024-05-16 11:01:26.000000 fluke_fl-0.0.3/fluke/evaluation.py
+-rw-r--r--   0 mirko      (501) staff       (20)    43792 2024-05-17 08:15:27.000000 fluke_fl-0.0.3/fluke/nets.py
+-rw-r--r--   0 mirko      (501) staff       (20)     7075 2024-05-16 12:56:17.000000 fluke_fl-0.0.3/fluke/run.py
+-rw-r--r--   0 mirko      (501) staff       (20)    15016 2024-05-16 11:01:26.000000 fluke_fl-0.0.3/fluke/server.py
+drwxr-xr-x   0 mirko      (501) staff       (20)        0 2024-05-20 07:51:21.496135 fluke_fl-0.0.3/fluke/utils/
+-rw-r--r--   0 mirko      (501) staff       (20)    22022 2024-05-17 07:33:13.000000 fluke_fl-0.0.3/fluke/utils/__init__.py
+-rw-r--r--   0 mirko      (501) staff       (20)    23035 2024-05-17 12:17:19.000000 fluke_fl-0.0.3/fluke/utils/model.py
+drwxr-xr-x   0 mirko      (501) staff       (20)        0 2024-05-20 07:51:21.498950 fluke_fl-0.0.3/fluke_fl.egg-info/
+-rw-r--r--   0 mirko      (501) staff       (20)    34816 2024-05-20 07:51:21.000000 fluke_fl-0.0.3/fluke_fl.egg-info/PKG-INFO
+-rw-r--r--   0 mirko      (501) staff       (20)     1385 2024-05-20 07:51:21.000000 fluke_fl-0.0.3/fluke_fl.egg-info/SOURCES.txt
+-rw-r--r--   0 mirko      (501) staff       (20)        1 2024-05-20 07:51:21.000000 fluke_fl-0.0.3/fluke_fl.egg-info/dependency_links.txt
+-rw-r--r--   0 mirko      (501) staff       (20)       41 2024-05-20 07:51:21.000000 fluke_fl-0.0.3/fluke_fl.egg-info/entry_points.txt
+-rw-r--r--   0 mirko      (501) staff       (20)       96 2024-05-20 07:51:21.000000 fluke_fl-0.0.3/fluke_fl.egg-info/requires.txt
+-rw-r--r--   0 mirko      (501) staff       (20)        6 2024-05-20 07:51:21.000000 fluke_fl-0.0.3/fluke_fl.egg-info/top_level.txt
+-rw-r--r--   0 mirko      (501) staff       (20)     1699 2024-05-20 07:51:16.000000 fluke_fl-0.0.3/pyproject.toml
+-rw-r--r--   0 mirko      (501) staff       (20)       38 2024-05-20 07:51:21.499689 fluke_fl-0.0.3/setup.cfg
+drwxr-xr-x   0 mirko      (501) staff       (20)        0 2024-05-20 07:51:21.498676 fluke_fl-0.0.3/tests/
+-rw-r--r--   0 mirko      (501) staff       (20)    10293 2024-05-17 10:06:41.000000 fluke_fl-0.0.3/tests/test_alg.py
+-rw-r--r--   0 mirko      (501) staff       (20)     4397 2024-05-16 11:01:26.000000 fluke_fl-0.0.3/tests/test_client.py
+-rw-r--r--   0 mirko      (501) staff       (20)     3331 2024-05-16 11:01:26.000000 fluke_fl-0.0.3/tests/test_comm.py
+-rw-r--r--   0 mirko      (501) staff       (20)     2130 2024-05-16 11:01:26.000000 fluke_fl-0.0.3/tests/test_core.py
+-rw-r--r--   0 mirko      (501) staff       (20)    11108 2024-05-16 11:01:26.000000 fluke_fl-0.0.3/tests/test_data.py
+-rw-r--r--   0 mirko      (501) staff       (20)    12738 2024-05-17 12:09:41.000000 fluke_fl-0.0.3/tests/test_datasets.py
+-rw-r--r--   0 mirko      (501) staff       (20)     2895 2024-05-16 11:01:26.000000 fluke_fl-0.0.3/tests/test_eval.py
+-rw-r--r--   0 mirko      (501) staff       (20)     4620 2024-05-16 11:01:26.000000 fluke_fl-0.0.3/tests/test_nets.py
+-rw-r--r--   0 mirko      (501) staff       (20)     3716 2024-05-16 11:01:26.000000 fluke_fl-0.0.3/tests/test_server.py
+-rw-r--r--   0 mirko      (501) staff       (20)    13910 2024-05-17 12:13:40.000000 fluke_fl-0.0.3/tests/test_utils.py
```

### Comparing `fluke_fl-0.0.2/LICENSE` & `fluke_fl-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/PKG-INFO` & `fluke_fl-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluke-fl
-Version: 0.0.2
+Version: 0.0.3
 Summary: Federated Learning Utility framework for Experimentation and research.
 Author-email: Mirko Polato <mirko.polato@unito.it>
 License:                   GNU LESSER GENERAL PUBLIC LICENSE
                                Version 2.1, February 1999
         
          Copyright (C) 1991, 1999 Free Software Foundation, Inc.
          51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
@@ -519,20 +519,21 @@
 Requires-Dist: torchvision
 Requires-Dist: rich
 Requires-Dist: typer
 Requires-Dist: wandb
 Requires-Dist: datasets
 Requires-Dist: psutil
 
+![Coveralls](https://img.shields.io/coverallsCoverage/github/makgyver/fluke?style=for-the-badge&logo=coveralls)
 <a href="https://makgyver.github.io/fluke"><img src="https://img.shields.io/github/actions/workflow/status/makgyver/fluke/doc-publish.yml?style=for-the-badge&label=DOCUMENTATION"/></a>
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/fluke-fl?style=for-the-badge&logo=python&logoColor=yellow)
 ![GitHub License](https://img.shields.io/github/license/makgyver/fluke?style=for-the-badge)
 
 
-# **``fluke``**: **f**ederated **l**earning **u**tility framewor**k** for **e**xperimentation and research
+# **fluke**: **f**ederated **l**earning **u**tility framewor**k** for **e**xperimentation and research
 
 ``fluke`` is a Python package that provides a framework for federated learning research. It is designed to be modular and extensible, allowing researchers to easily implement and test new federated learning algorithms. ``fluke`` provides a set of pre-implemented state-of-the-art federated learning algorithms that can be used as a starting point for research or as a benchmark for comparison.
 
 ## Installation
 
 ``fluke`` is a Python package that can be installed via pip. To install it, you can run the following command:
 
@@ -554,28 +555,38 @@
 
 You can find some examples of these files in the [configs](https://github.com/makgyver/fluke/tree/main/configs) folder of the repository.
 
 ### Example
 Let say you want to run the classic `FedAvg` algorithm on the `MNIST` dataset. Then, using the configuration files [exp.yaml](https://github.com/makgyver/fluke/blob/main/configs/exp.yaml) and [fedavg.yaml](https://github.com/makgyver/fluke/blob/main/configs/fedavg.yaml), you can run the following command:
 
 ```bash
-fluke --config=configs/exp.yaml federation ./configs/fedavg.yaml
+fluke --config=path_to_folder/exp.yaml federation path_to_folder/fedavg.yaml
 ```
 
+where `path_to_folder` is the path to the folder containing the configuration files.
+
 
 ## Documentation
 
 The documentation for ``fluke`` can be found [here](https://makgyver.github.io/fluke). It contains detailed information about the package, including how to install it, how to run an experiment, and how to implement new algorithms.
 
-## Tutorial
+## Tutorials
+
+Tutorials on how to use ``fluke`` can be found [here](https://makgyver.github.io/fluke/tutorials.html). In the following, you can find some quick tutorials to get started with ``fluke``:
+
+- Getting started with `fluke` API [![Open in Colab](https://img.shields.io/badge/Open_in_Colab-blue?style=flat-square&logo=google-colab&logoColor=yellow&labelColor=gray)
+](https://colab.research.google.com/github/makgyver/fluke/blob/main/tutorials/fluke_quick_api.ipynb)
+- Run your algorithm in ``fluke`` [![Open in Colab](https://img.shields.io/badge/Open_in_Colab-blue?style=flat-square&logo=google-colab&logoColor=yellow&labelColor=gray)
+](https://colab.research.google.com/github/makgyver/fluke/blob/main/tutorials/fluke_custom_alg.ipynb)
+
+## Contributing
 
-Tutorials on how to use ``fluke`` can be found [here](https://makgyver.github.io/fluke/tutorial.html). In the following, you can find some quick tutorials to get started with ``fluke``:
+If you have suggestions for how ``fluke`` could be improved, or want to report a bug, open an issue! We'd love all and any contributions.
 
-- Getting started with `fluke` API [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/makgyver/fluke/blob/main/tutorials/fluke_quick_api.ipynb)
-- Run your algorithm in `fluke` [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/makgyver/fluke/blob/main/tutorials/fluke_custom_alg.ipynb)
+For more, check out the [Contributing Guide](CONTRIBUTING.md).
 
 
 ## Authors
 
-- [**Mirko Polato**](https://makgyver.github.io) - *Idealization*, *Development*, *Testing*, and *Documentation*
+- [**Mirko Polato**](https://makgyver.github.io) - *Idealization*, *Design*, *Development*, *Testing*, and *Documentation*
 - [**Roberto Esposito**]() - *Testing*
 - [**Samuele Fonio**]() - *Testing*
```

### Comparing `fluke_fl-0.0.2/README.md` & `fluke_fl-0.0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+![Coveralls](https://img.shields.io/coverallsCoverage/github/makgyver/fluke?style=for-the-badge&logo=coveralls)
 <a href="https://makgyver.github.io/fluke"><img src="https://img.shields.io/github/actions/workflow/status/makgyver/fluke/doc-publish.yml?style=for-the-badge&label=DOCUMENTATION"/></a>
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/fluke-fl?style=for-the-badge&logo=python&logoColor=yellow)
 ![GitHub License](https://img.shields.io/github/license/makgyver/fluke?style=for-the-badge)
 
 
-# **``fluke``**: **f**ederated **l**earning **u**tility framewor**k** for **e**xperimentation and research
+# **fluke**: **f**ederated **l**earning **u**tility framewor**k** for **e**xperimentation and research
 
 ``fluke`` is a Python package that provides a framework for federated learning research. It is designed to be modular and extensible, allowing researchers to easily implement and test new federated learning algorithms. ``fluke`` provides a set of pre-implemented state-of-the-art federated learning algorithms that can be used as a starting point for research or as a benchmark for comparison.
 
 ## Installation
 
 ``fluke`` is a Python package that can be installed via pip. To install it, you can run the following command:
 
@@ -29,28 +30,38 @@
 
 You can find some examples of these files in the [configs](https://github.com/makgyver/fluke/tree/main/configs) folder of the repository.
 
 ### Example
 Let say you want to run the classic `FedAvg` algorithm on the `MNIST` dataset. Then, using the configuration files [exp.yaml](https://github.com/makgyver/fluke/blob/main/configs/exp.yaml) and [fedavg.yaml](https://github.com/makgyver/fluke/blob/main/configs/fedavg.yaml), you can run the following command:
 
 ```bash
-fluke --config=configs/exp.yaml federation ./configs/fedavg.yaml
+fluke --config=path_to_folder/exp.yaml federation path_to_folder/fedavg.yaml
 ```
 
+where `path_to_folder` is the path to the folder containing the configuration files.
+
 
 ## Documentation
 
 The documentation for ``fluke`` can be found [here](https://makgyver.github.io/fluke). It contains detailed information about the package, including how to install it, how to run an experiment, and how to implement new algorithms.
 
-## Tutorial
+## Tutorials
+
+Tutorials on how to use ``fluke`` can be found [here](https://makgyver.github.io/fluke/tutorials.html). In the following, you can find some quick tutorials to get started with ``fluke``:
+
+- Getting started with `fluke` API [![Open in Colab](https://img.shields.io/badge/Open_in_Colab-blue?style=flat-square&logo=google-colab&logoColor=yellow&labelColor=gray)
+](https://colab.research.google.com/github/makgyver/fluke/blob/main/tutorials/fluke_quick_api.ipynb)
+- Run your algorithm in ``fluke`` [![Open in Colab](https://img.shields.io/badge/Open_in_Colab-blue?style=flat-square&logo=google-colab&logoColor=yellow&labelColor=gray)
+](https://colab.research.google.com/github/makgyver/fluke/blob/main/tutorials/fluke_custom_alg.ipynb)
+
+## Contributing
 
-Tutorials on how to use ``fluke`` can be found [here](https://makgyver.github.io/fluke/tutorial.html). In the following, you can find some quick tutorials to get started with ``fluke``:
+If you have suggestions for how ``fluke`` could be improved, or want to report a bug, open an issue! We'd love all and any contributions.
 
-- Getting started with `fluke` API [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/makgyver/fluke/blob/main/tutorials/fluke_quick_api.ipynb)
-- Run your algorithm in `fluke` [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/makgyver/fluke/blob/main/tutorials/fluke_custom_alg.ipynb)
+For more, check out the [Contributing Guide](CONTRIBUTING.md).
 
 
 ## Authors
 
-- [**Mirko Polato**](https://makgyver.github.io) - *Idealization*, *Development*, *Testing*, and *Documentation*
+- [**Mirko Polato**](https://makgyver.github.io) - *Idealization*, *Design*, *Development*, *Testing*, and *Documentation*
 - [**Roberto Esposito**]() - *Testing*
 - [**Samuele Fonio**]() - *Testing*
```

#### html2text {}

```diff
@@ -1,41 +1,47 @@
-_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_/_s_t_a_t_u_s_/_m_a_k_g_y_v_e_r_/_f_l_u_k_e_/_d_o_c_-
-_p_u_b_l_i_s_h_._y_m_l_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_a_b_e_l_=_D_O_C_U_M_E_N_T_A_T_I_O_N_]![PyPI - Python Version]
-(https://img.shields.io/pypi/pyversions/fluke-fl?style=for-the-
-badge&logo=python&logoColor=yellow) ![GitHub License](https://img.shields.io/
-github/license/makgyver/fluke?style=for-the-badge) # **``fluke``**:
-**f**ederated **l**earning **u**tility framewor**k** for **e**xperimentation
-and research ``fluke`` is a Python package that provides a framework for
-federated learning research. It is designed to be modular and extensible,
-allowing researchers to easily implement and test new federated learning
-algorithms. ``fluke`` provides a set of pre-implemented state-of-the-art
-federated learning algorithms that can be used as a starting point for research
-or as a benchmark for comparison. ## Installation ``fluke`` is a Python package
-that can be installed via pip. To install it, you can run the following
-command: ```bash pip install fluke-fl ``` ## Run a federated algorithm To run
-an algorithm in ``fluke`` you need to create two configuration files: -
-`EXP_CONFIG`: the experiment configuration file (independent from the
+![Coveralls](https://img.shields.io/coverallsCoverage/github/makgyver/
+fluke?style=for-the-badge&logo=coveralls) _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/
+_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_/_s_t_a_t_u_s_/_m_a_k_g_y_v_e_r_/_f_l_u_k_e_/_d_o_c_-_p_u_b_l_i_s_h_._y_m_l_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-
+_b_a_d_g_e_&_l_a_b_e_l_=_D_O_C_U_M_E_N_T_A_T_I_O_N_]![PyPI - Python Version](https://img.shields.io/pypi/
+pyversions/fluke-fl?style=for-the-badge&logo=python&logoColor=yellow) ![GitHub
+License](https://img.shields.io/github/license/makgyver/fluke?style=for-the-
+badge) # **fluke**: **f**ederated **l**earning **u**tility framewor**k** for
+**e**xperimentation and research ``fluke`` is a Python package that provides a
+framework for federated learning research. It is designed to be modular and
+extensible, allowing researchers to easily implement and test new federated
+learning algorithms. ``fluke`` provides a set of pre-implemented state-of-the-
+art federated learning algorithms that can be used as a starting point for
+research or as a benchmark for comparison. ## Installation ``fluke`` is a
+Python package that can be installed via pip. To install it, you can run the
+following command: ```bash pip install fluke-fl ``` ## Run a federated
+algorithm To run an algorithm in ``fluke`` you need to create two configuration
+files: - `EXP_CONFIG`: the experiment configuration file (independent from the
 algorithm); - `ALG_CONFIG`: the algorithm configuration file; Then, you can run
 the following command: ```bash fluke --config=EXP_CONFIG federation ALG_CONFIG
 ``` You can find some examples of these files in the [configs](https://
 github.com/makgyver/fluke/tree/main/configs) folder of the repository. ###
 Example Let say you want to run the classic `FedAvg` algorithm on the `MNIST`
 dataset. Then, using the configuration files [exp.yaml](https://github.com/
 makgyver/fluke/blob/main/configs/exp.yaml) and [fedavg.yaml](https://
 github.com/makgyver/fluke/blob/main/configs/fedavg.yaml), you can run the
-following command: ```bash fluke --config=configs/exp.yaml federation ./
-configs/fedavg.yaml ``` ## Documentation The documentation for ``fluke`` can be
-found [here](https://makgyver.github.io/fluke). It contains detailed
-information about the package, including how to install it, how to run an
-experiment, and how to implement new algorithms. ## Tutorial Tutorials on how
-to use ``fluke`` can be found [here](https://makgyver.github.io/fluke/
-tutorial.html). In the following, you can find some quick tutorials to get
-started with ``fluke``: - Getting started with `fluke` API [![Open In Colab]
-(https://colab.research.google.com/assets/colab-badge.svg)](https://
-colab.research.google.com/github/makgyver/fluke/blob/main/tutorials/
-fluke_quick_api.ipynb) - Run your algorithm in `fluke` [![Open In Colab](https:
-//colab.research.google.com/assets/colab-badge.svg)](https://
-colab.research.google.com/github/makgyver/fluke/blob/main/tutorials/
-fluke_custom_alg.ipynb) ## Authors - [**Mirko Polato**](https://
-makgyver.github.io) - *Idealization*, *Development*, *Testing*, and
-*Documentation* - [**Roberto Esposito**]() - *Testing* - [**Samuele Fonio**]()
-- *Testing*
+following command: ```bash fluke --config=path_to_folder/exp.yaml federation
+path_to_folder/fedavg.yaml ``` where `path_to_folder` is the path to the folder
+containing the configuration files. ## Documentation The documentation for
+``fluke`` can be found [here](https://makgyver.github.io/fluke). It contains
+detailed information about the package, including how to install it, how to run
+an experiment, and how to implement new algorithms. ## Tutorials Tutorials on
+how to use ``fluke`` can be found [here](https://makgyver.github.io/fluke/
+tutorials.html). In the following, you can find some quick tutorials to get
+started with ``fluke``: - Getting started with `fluke` API [![Open in Colab]
+(https://img.shields.io/badge/Open_in_Colab-blue?style=flat-square&logo=google-
+colab&logoColor=yellow&labelColor=gray) ](https://colab.research.google.com/
+github/makgyver/fluke/blob/main/tutorials/fluke_quick_api.ipynb) - Run your
+algorithm in ``fluke`` [![Open in Colab](https://img.shields.io/badge/
+Open_in_Colab-blue?style=flat-square&logo=google-
+colab&logoColor=yellow&labelColor=gray) ](https://colab.research.google.com/
+github/makgyver/fluke/blob/main/tutorials/fluke_custom_alg.ipynb) ##
+Contributing If you have suggestions for how ``fluke`` could be improved, or
+want to report a bug, open an issue! We'd love all and any contributions. For
+more, check out the [Contributing Guide](CONTRIBUTING.md). ## Authors -
+[**Mirko Polato**](https://makgyver.github.io) - *Idealization*, *Design*,
+*Development*, *Testing*, and *Documentation* - [**Roberto Esposito**]() -
+*Testing* - [**Samuele Fonio**]() - *Testing*
```

### Comparing `fluke_fl-0.0.2/fluke/__init__.py` & `fluke_fl-0.0.3/fluke/__init__.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/fluke/algorithms/__init__.py` & `fluke_fl-0.0.3/fluke/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/fluke/algorithms/apfl.py` & `fluke_fl-0.0.3/fluke/algorithms/apfl.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/fluke/algorithms/ccvr.py` & `fluke_fl-0.0.3/fluke/algorithms/ccvr.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/fluke/algorithms/ditto.py` & `fluke_fl-0.0.3/fluke/algorithms/ditto.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/fluke/algorithms/fedamp.py` & `fluke_fl-0.0.3/fluke/algorithms/fedamp.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/fluke/algorithms/fedavgm.py` & `fluke_fl-0.0.3/fluke/algorithms/fedavgm.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/fluke/algorithms/fedbabu.py` & `fluke_fl-0.0.3/fluke/algorithms/fedbabu.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/fluke/algorithms/fedbn.py` & `fluke_fl-0.0.3/fluke/algorithms/fedbn.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/fluke/algorithms/feddyn.py` & `fluke_fl-0.0.3/fluke/algorithms/feddyn.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/fluke/algorithms/fedexp.py` & `fluke_fl-0.0.3/fluke/algorithms/fedexp.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,16 +36,15 @@
         mu_diff = {}
         eta = {}
         M = len(clients_diff)
 
         for key in clients_diff[0].keys():
             if key.endswith(STATE_DICT_KEYS_TO_IGNORE):
                 continue
-            num[key] = torch.sum(torch.FloatTensor(
-                [torch.norm(c[key])**2 for c in clients_diff]))
+            num[key] = torch.sum(torch.FloatTensor([torch.norm(c[key])**2 for c in clients_diff]))
             mu_diff[key] = torch.mean(torch.stack([c[key] for c in clients_diff]), dim=0)
             den[key] = 2 * M * (torch.norm(mu_diff[key])**2 + eps)
             eta[key] = torch.max(num[key] / den[key], torch.FloatTensor([1.0]))
 
         return eta, mu_diff
```

### Comparing `fluke_fl-0.0.2/fluke/algorithms/fedhp.py` & `fluke_fl-0.0.3/fluke/algorithms/fedhp.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/fluke/algorithms/fedlc.py` & `fluke_fl-0.0.3/fluke/algorithms/fedlc.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/fluke/algorithms/fednh.py` & `fluke_fl-0.0.3/fluke/algorithms/fednh.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/fluke/algorithms/fednova.py` & `fluke_fl-0.0.3/fluke/algorithms/fednova.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/fluke/algorithms/fedopt.py` & `fluke_fl-0.0.3/fluke/algorithms/fedopt.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/fluke/algorithms/fedper.py` & `fluke_fl-0.0.3/fluke/algorithms/fedper.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/fluke/algorithms/fedproto.py` & `fluke_fl-0.0.3/fluke/algorithms/fedproto.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/fluke/algorithms/fedprox.py` & `fluke_fl-0.0.3/fluke/algorithms/fedprox.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/fluke/algorithms/fedrep.py` & `fluke_fl-0.0.3/fluke/algorithms/fedrep.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/fluke/algorithms/fedsgd.py` & `fluke_fl-0.0.3/fluke/algorithms/fedsgd.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/fluke/algorithms/lg_fedavg.py` & `fluke_fl-0.0.3/fluke/algorithms/lg_fedavg.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/fluke/algorithms/moon.py` & `fluke_fl-0.0.3/fluke/algorithms/moon.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/fluke/algorithms/per_fedavg.py` & `fluke_fl-0.0.3/fluke/algorithms/per_fedavg.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/fluke/algorithms/pfedme.py` & `fluke_fl-0.0.3/fluke/algorithms/pfedme.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/fluke/algorithms/scaffold.py` & `fluke_fl-0.0.3/fluke/algorithms/scaffold.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/fluke/algorithms/superfed.py` & `fluke_fl-0.0.3/fluke/algorithms/superfed.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/fluke/client.py` & `fluke_fl-0.0.3/fluke/client.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/fluke/comm.py` & `fluke_fl-0.0.3/fluke/comm.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/fluke/data/__init__.py` & `fluke_fl-0.0.3/fluke/data/__init__.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/fluke/data/datasets.py` & `fluke_fl-0.0.3/fluke/data/datasets.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/fluke/data/support.py` & `fluke_fl-0.0.3/fluke/data/support.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/fluke/evaluation.py` & `fluke_fl-0.0.3/fluke/evaluation.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/fluke/nets.py` & `fluke_fl-0.0.3/fluke/nets.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/fluke/run.py` & `fluke_fl-0.0.3/fluke/run.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/fluke/server.py` & `fluke_fl-0.0.3/fluke/server.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/fluke/utils/__init__.py` & `fluke_fl-0.0.3/fluke/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/fluke/utils/model.py` & `fluke_fl-0.0.3/fluke/utils/model.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/fluke_fl.egg-info/PKG-INFO` & `fluke_fl-0.0.3/fluke_fl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluke-fl
-Version: 0.0.2
+Version: 0.0.3
 Summary: Federated Learning Utility framework for Experimentation and research.
 Author-email: Mirko Polato <mirko.polato@unito.it>
 License:                   GNU LESSER GENERAL PUBLIC LICENSE
                                Version 2.1, February 1999
         
          Copyright (C) 1991, 1999 Free Software Foundation, Inc.
          51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
@@ -519,20 +519,21 @@
 Requires-Dist: torchvision
 Requires-Dist: rich
 Requires-Dist: typer
 Requires-Dist: wandb
 Requires-Dist: datasets
 Requires-Dist: psutil
 
+![Coveralls](https://img.shields.io/coverallsCoverage/github/makgyver/fluke?style=for-the-badge&logo=coveralls)
 <a href="https://makgyver.github.io/fluke"><img src="https://img.shields.io/github/actions/workflow/status/makgyver/fluke/doc-publish.yml?style=for-the-badge&label=DOCUMENTATION"/></a>
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/fluke-fl?style=for-the-badge&logo=python&logoColor=yellow)
 ![GitHub License](https://img.shields.io/github/license/makgyver/fluke?style=for-the-badge)
 
 
-# **``fluke``**: **f**ederated **l**earning **u**tility framewor**k** for **e**xperimentation and research
+# **fluke**: **f**ederated **l**earning **u**tility framewor**k** for **e**xperimentation and research
 
 ``fluke`` is a Python package that provides a framework for federated learning research. It is designed to be modular and extensible, allowing researchers to easily implement and test new federated learning algorithms. ``fluke`` provides a set of pre-implemented state-of-the-art federated learning algorithms that can be used as a starting point for research or as a benchmark for comparison.
 
 ## Installation
 
 ``fluke`` is a Python package that can be installed via pip. To install it, you can run the following command:
 
@@ -554,28 +555,38 @@
 
 You can find some examples of these files in the [configs](https://github.com/makgyver/fluke/tree/main/configs) folder of the repository.
 
 ### Example
 Let say you want to run the classic `FedAvg` algorithm on the `MNIST` dataset. Then, using the configuration files [exp.yaml](https://github.com/makgyver/fluke/blob/main/configs/exp.yaml) and [fedavg.yaml](https://github.com/makgyver/fluke/blob/main/configs/fedavg.yaml), you can run the following command:
 
 ```bash
-fluke --config=configs/exp.yaml federation ./configs/fedavg.yaml
+fluke --config=path_to_folder/exp.yaml federation path_to_folder/fedavg.yaml
 ```
 
+where `path_to_folder` is the path to the folder containing the configuration files.
+
 
 ## Documentation
 
 The documentation for ``fluke`` can be found [here](https://makgyver.github.io/fluke). It contains detailed information about the package, including how to install it, how to run an experiment, and how to implement new algorithms.
 
-## Tutorial
+## Tutorials
+
+Tutorials on how to use ``fluke`` can be found [here](https://makgyver.github.io/fluke/tutorials.html). In the following, you can find some quick tutorials to get started with ``fluke``:
+
+- Getting started with `fluke` API [![Open in Colab](https://img.shields.io/badge/Open_in_Colab-blue?style=flat-square&logo=google-colab&logoColor=yellow&labelColor=gray)
+](https://colab.research.google.com/github/makgyver/fluke/blob/main/tutorials/fluke_quick_api.ipynb)
+- Run your algorithm in ``fluke`` [![Open in Colab](https://img.shields.io/badge/Open_in_Colab-blue?style=flat-square&logo=google-colab&logoColor=yellow&labelColor=gray)
+](https://colab.research.google.com/github/makgyver/fluke/blob/main/tutorials/fluke_custom_alg.ipynb)
+
+## Contributing
 
-Tutorials on how to use ``fluke`` can be found [here](https://makgyver.github.io/fluke/tutorial.html). In the following, you can find some quick tutorials to get started with ``fluke``:
+If you have suggestions for how ``fluke`` could be improved, or want to report a bug, open an issue! We'd love all and any contributions.
 
-- Getting started with `fluke` API [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/makgyver/fluke/blob/main/tutorials/fluke_quick_api.ipynb)
-- Run your algorithm in `fluke` [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/makgyver/fluke/blob/main/tutorials/fluke_custom_alg.ipynb)
+For more, check out the [Contributing Guide](CONTRIBUTING.md).
 
 
 ## Authors
 
-- [**Mirko Polato**](https://makgyver.github.io) - *Idealization*, *Development*, *Testing*, and *Documentation*
+- [**Mirko Polato**](https://makgyver.github.io) - *Idealization*, *Design*, *Development*, *Testing*, and *Documentation*
 - [**Roberto Esposito**]() - *Testing*
 - [**Samuele Fonio**]() - *Testing*
```

### Comparing `fluke_fl-0.0.2/fluke_fl.egg-info/SOURCES.txt` & `fluke_fl-0.0.3/fluke_fl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/pyproject.toml` & `fluke_fl-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 where = ["."]  # list of folders that contain the packages (["."] by default)
 include = ["fluke", "fluke.data", "fluke.utils", "fluke.algorithms"]  # package names should match these glob patterns (["*"] by default)
 exclude = []  # exclude packages matching these glob patterns (empty by default)
 namespaces = false  # to disable scanning PEP 420 namespaces (true by default)
 
 [project]
 name = "fluke-fl"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Mirko Polato", email="mirko.polato@unito.it" },
 ]
 description = "Federated Learning Utility framework for Experimentation and research."
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
```

### Comparing `fluke_fl-0.0.2/tests/test_alg.py` & `fluke_fl-0.0.3/tests/test_alg.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/tests/test_client.py` & `fluke_fl-0.0.3/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/tests/test_comm.py` & `fluke_fl-0.0.3/tests/test_comm.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/tests/test_core.py` & `fluke_fl-0.0.3/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/tests/test_data.py` & `fluke_fl-0.0.3/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/tests/test_datasets.py` & `fluke_fl-0.0.3/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/tests/test_eval.py` & `fluke_fl-0.0.3/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/tests/test_nets.py` & `fluke_fl-0.0.3/tests/test_nets.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/tests/test_server.py` & `fluke_fl-0.0.3/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.2/tests/test_utils.py` & `fluke_fl-0.0.3/tests/test_utils.py`

 * *Files identical despite different names*

