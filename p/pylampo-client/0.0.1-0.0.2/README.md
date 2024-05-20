# Comparing `tmp/pylampo_client-0.0.1.tar.gz` & `tmp/pylampo_client-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylampo_client-0.0.1.tar", max compression
+gzip compressed data, was "pylampo_client-0.0.2.tar", max compression
```

## Comparing `pylampo_client-0.0.1.tar` & `pylampo_client-0.0.2.tar`

### file list

```diff
@@ -1,3 +1,4 @@
--rw-r--r--   0        0        0     1559 2024-04-07 17:18:33.992142 pylampo_client-0.0.1/pylampo_client/client.py
--rw-r--r--   0        0        0      306 2024-04-07 17:18:33.992921 pylampo_client-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      505 1970-01-01 00:00:00.000000 pylampo_client-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       55 2024-05-20 10:12:25.816454 pylampo_client-0.0.2/pylampo_client/__init__.py
+-rw-r--r--   0        0        0     2266 2024-05-20 10:12:25.816683 pylampo_client-0.0.2/pylampo_client/client.py
+-rw-r--r--   0        0        0      324 2024-05-20 10:12:51.127759 pylampo_client-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 pylampo_client-0.0.2/PKG-INFO
```

