# Comparing `tmp/slot_can-0.1.0.tar.gz` & `tmp/slot_can-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slot_can-0.1.0.tar", last modified: Mon May 20 14:10:44 2024, max compression
+gzip compressed data, was "slot_can-0.2.0.tar", last modified: Mon May 20 14:17:30 2024, max compression
```

## Comparing `slot_can-0.1.0.tar` & `slot_can-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 yi        (1000) yi        (1000)        0 2024-05-20 14:10:44.767199 slot_can-0.1.0/
--rw-rw-r--   0 yi        (1000) yi        (1000)      225 2024-05-20 14:10:44.767199 slot_can-0.1.0/PKG-INFO
--rw-rw-r--   0 yi        (1000) yi        (1000)      131 2024-05-20 14:06:15.000000 slot_can-0.1.0/README.md
--rw-rw-r--   0 yi        (1000) yi        (1000)       38 2024-05-20 14:10:44.767199 slot_can-0.1.0/setup.cfg
--rw-rw-r--   0 yi        (1000) yi        (1000)      247 2024-05-20 14:10:25.000000 slot_can-0.1.0/setup.py
-drwxrwxr-x   0 yi        (1000) yi        (1000)        0 2024-05-20 14:10:44.767199 slot_can-0.1.0/slot_can.egg-info/
--rw-rw-r--   0 yi        (1000) yi        (1000)      225 2024-05-20 14:10:44.000000 slot_can-0.1.0/slot_can.egg-info/PKG-INFO
--rw-rw-r--   0 yi        (1000) yi        (1000)      146 2024-05-20 14:10:44.000000 slot_can-0.1.0/slot_can.egg-info/SOURCES.txt
--rw-rw-r--   0 yi        (1000) yi        (1000)        1 2024-05-20 14:10:44.000000 slot_can-0.1.0/slot_can.egg-info/dependency_links.txt
--rw-rw-r--   0 yi        (1000) yi        (1000)        1 2024-05-20 14:10:44.000000 slot_can-0.1.0/slot_can.egg-info/top_level.txt
+drwxrwxr-x   0 yi        (1000) yi        (1000)        0 2024-05-20 14:17:30.995123 slot_can-0.2.0/
+-rw-r--r--   0 yi        (1000) yi        (1000)      225 2024-05-20 14:17:30.995123 slot_can-0.2.0/PKG-INFO
+-rw-rw-r--   0 yi        (1000) yi        (1000)      131 2024-05-20 14:06:15.000000 slot_can-0.2.0/README.md
+-rw-rw-r--   0 yi        (1000) yi        (1000)       38 2024-05-20 14:17:30.995123 slot_can-0.2.0/setup.cfg
+-rw-rw-r--   0 yi        (1000) yi        (1000)      247 2024-05-20 14:17:22.000000 slot_can-0.2.0/setup.py
+drwxrwxr-x   0 yi        (1000) yi        (1000)        0 2024-05-20 14:17:30.995123 slot_can-0.2.0/slot_can.egg-info/
+-rw-r--r--   0 yi        (1000) yi        (1000)      225 2024-05-20 14:17:30.000000 slot_can-0.2.0/slot_can.egg-info/PKG-INFO
+-rw-rw-r--   0 yi        (1000) yi        (1000)      146 2024-05-20 14:17:30.000000 slot_can-0.2.0/slot_can.egg-info/SOURCES.txt
+-rw-rw-r--   0 yi        (1000) yi        (1000)        1 2024-05-20 14:17:30.000000 slot_can-0.2.0/slot_can.egg-info/dependency_links.txt
+-rw-rw-r--   0 yi        (1000) yi        (1000)        1 2024-05-20 14:17:30.000000 slot_can-0.2.0/slot_can.egg-info/top_level.txt
```

