# Comparing `tmp/fordpip-0.0.1.tar.gz` & `tmp/fordpip-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fordpip-0.0.1.tar", last modified: Mon Apr 15 18:00:52 2024, max compression
+gzip compressed data, was "fordpip-0.1.0.tar", last modified: Mon Apr 15 17:49:44 2024, max compression
```

## Comparing `fordpip-0.0.1.tar` & `fordpip-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,9 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 18:00:52.249974 fordpip-0.0.1/
--rw-rw-rw-   0        0        0      483 2024-04-15 18:00:52.246976 fordpip-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      483 2024-04-15 17:58:14.000000 fordpip-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0        9 2024-04-15 17:12:39.000000 fordpip-0.0.1/readme.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 18:00:52.249974 fordpip-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-15 18:00:52.220975 fordpip-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-15 18:00:52.230037 fordpip-0.0.1/src/fordpip/
--rw-rw-rw-   0        0        0        0 2024-04-15 17:56:14.000000 fordpip-0.0.1/src/fordpip/__init__.py
--rw-rw-rw-   0        0        0      105 2024-04-15 17:17:04.000000 fordpip-0.0.1/src/fordpip/start.py
--rw-rw-rw-   0        0        0       40 2024-04-15 17:47:14.000000 fordpip-0.0.1/src/fordpip/test.py
-drwxrwxrwx   0        0        0        0 2024-04-15 18:00:52.243975 fordpip-0.0.1/src/fordpip.egg-info/
--rw-rw-rw-   0        0        0      483 2024-04-15 18:00:52.000000 fordpip-0.0.1/src/fordpip.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2024-04-15 18:00:52.000000 fordpip-0.0.1/src/fordpip.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 18:00:52.000000 fordpip-0.0.1/src/fordpip.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-15 18:00:52.000000 fordpip-0.0.1/src/fordpip.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 17:49:44.303443 fordpip-0.1.0/
+-rw-rw-rw-   0        0        0      304 2024-04-15 17:49:44.301445 fordpip-0.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-15 17:49:44.298455 fordpip-0.1.0/fordpip.egg-info/
+-rw-rw-rw-   0        0        0      304 2024-04-15 17:49:44.000000 fordpip-0.1.0/fordpip.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      132 2024-04-15 17:49:44.000000 fordpip-0.1.0/fordpip.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 17:49:44.000000 fordpip-0.1.0/fordpip.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 17:49:44.000000 fordpip-0.1.0/fordpip.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 17:49:44.304542 fordpip-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      370 2024-04-15 17:38:18.000000 fordpip-0.1.0/setup.py
```

