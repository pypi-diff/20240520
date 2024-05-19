# Comparing `tmp/RNAkinetics-0.1.tar.gz` & `tmp/RNAkinetics-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RNAkinetics-0.1.tar", last modified: Tue Oct 17 21:01:43 2023, max compression
+gzip compressed data, was "RNAkinetics-0.2.4.tar", last modified: Sun May 19 23:24:19 2024, max compression
```

## Comparing `RNAkinetics-0.1.tar` & `RNAkinetics-0.2.4.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxr-xr-x   0 chan       (501) staff       (20)        0 2023-10-17 21:01:43.869146 RNAkinetics-0.1/
--rw-r--r--   0 chan       (501) staff       (20)    35149 2023-10-17 20:48:44.000000 RNAkinetics-0.1/LICENSE
--rw-r--r--   0 chan       (501) staff       (20)      332 2023-10-17 21:01:43.868971 RNAkinetics-0.1/PKG-INFO
--rw-r--r--   0 chan       (501) staff       (20)       63 2023-10-17 20:48:44.000000 RNAkinetics-0.1/README.md
-drwxr-xr-x   0 chan       (501) staff       (20)        0 2023-10-17 21:01:43.867994 RNAkinetics-0.1/RNAkinetics/
--rw-r--r--   0 chan       (501) staff       (20)       69 2023-10-17 20:51:33.000000 RNAkinetics-0.1/RNAkinetics/__init__.py
--rw-r--r--   0 chan       (501) staff       (20)    11954 2023-10-17 20:32:29.000000 RNAkinetics-0.1/RNAkinetics/kinetics.py
--rw-r--r--   0 chan       (501) staff       (20)     6540 2023-10-17 18:58:59.000000 RNAkinetics-0.1/RNAkinetics/layers.py
-drwxr-xr-x   0 chan       (501) staff       (20)        0 2023-10-17 21:01:43.868719 RNAkinetics-0.1/RNAkinetics.egg-info/
--rw-r--r--   0 chan       (501) staff       (20)      332 2023-10-17 21:01:43.000000 RNAkinetics-0.1/RNAkinetics.egg-info/PKG-INFO
--rw-r--r--   0 chan       (501) staff       (20)      270 2023-10-17 21:01:43.000000 RNAkinetics-0.1/RNAkinetics.egg-info/SOURCES.txt
--rw-r--r--   0 chan       (501) staff       (20)        1 2023-10-17 21:01:43.000000 RNAkinetics-0.1/RNAkinetics.egg-info/dependency_links.txt
--rw-r--r--   0 chan       (501) staff       (20)      105 2023-10-17 21:01:43.000000 RNAkinetics-0.1/RNAkinetics.egg-info/requires.txt
--rw-r--r--   0 chan       (501) staff       (20)       12 2023-10-17 21:01:43.000000 RNAkinetics-0.1/RNAkinetics.egg-info/top_level.txt
--rw-r--r--   0 chan       (501) staff       (20)       38 2023-10-17 21:01:43.869204 RNAkinetics-0.1/setup.cfg
--rw-r--r--   0 chan       (501) staff       (20)      645 2023-10-17 21:01:38.000000 RNAkinetics-0.1/setup.py
+drwxr-xr-x   0 chan       (501) staff       (20)        0 2024-05-19 23:24:19.713410 RNAkinetics-0.2.4/
+-rw-r--r--   0 chan       (501) staff       (20)     1069 2024-01-29 00:05:20.000000 RNAkinetics-0.2.4/LICENSE
+-rw-r--r--   0 chan       (501) staff       (20)      325 2024-05-19 23:24:19.713276 RNAkinetics-0.2.4/PKG-INFO
+-rw-r--r--   0 chan       (501) staff       (20)     2369 2024-05-19 23:11:55.000000 RNAkinetics-0.2.4/README.md
+drwxr-xr-x   0 chan       (501) staff       (20)        0 2024-05-19 23:24:19.712781 RNAkinetics-0.2.4/RNAkinetics.egg-info/
+-rw-r--r--   0 chan       (501) staff       (20)      325 2024-05-19 23:24:19.000000 RNAkinetics-0.2.4/RNAkinetics.egg-info/PKG-INFO
+-rw-r--r--   0 chan       (501) staff       (20)      249 2024-05-19 23:24:19.000000 RNAkinetics-0.2.4/RNAkinetics.egg-info/SOURCES.txt
+-rw-r--r--   0 chan       (501) staff       (20)        1 2024-05-19 23:24:19.000000 RNAkinetics-0.2.4/RNAkinetics.egg-info/dependency_links.txt
+-rw-r--r--   0 chan       (501) staff       (20)       76 2024-05-19 23:24:19.000000 RNAkinetics-0.2.4/RNAkinetics.egg-info/requires.txt
+-rw-r--r--   0 chan       (501) staff       (20)       12 2024-05-19 23:24:19.000000 RNAkinetics-0.2.4/RNAkinetics.egg-info/top_level.txt
+drwxr-xr-x   0 chan       (501) staff       (20)        0 2024-05-19 23:24:19.713095 RNAkinetics-0.2.4/rnakinetics/
+-rw-r--r--   0 chan       (501) staff       (20)    21482 2024-01-26 20:10:17.000000 RNAkinetics-0.2.4/rnakinetics/ODEsolver.py
+-rw-r--r--   0 chan       (501) staff       (20)       41 2023-12-08 19:38:59.000000 RNAkinetics-0.2.4/rnakinetics/__init__.py
+-rw-r--r--   0 chan       (501) staff       (20)       38 2024-05-19 23:24:19.713494 RNAkinetics-0.2.4/setup.cfg
+-rw-r--r--   0 chan       (501) staff       (20)      615 2024-05-19 23:15:47.000000 RNAkinetics-0.2.4/setup.py
```

