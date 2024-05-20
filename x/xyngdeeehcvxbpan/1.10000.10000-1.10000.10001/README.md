# Comparing `tmp/xyngdeeehcvxbpan-1.10000.10000.tar.gz` & `tmp/xyngdeeehcvxbpan-1.10000.10001.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon May 20 00:31:11 2024, max compression
+gzip compressed data, last modified: Mon May 20 00:32:50 2024, max compression
```

## Comparing `xyngdeeehcvxbpan-1.10000.10000.tar` & `xyngdeeehcvxbpan-1.10000.10001.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 1970-01-01 00:00:00.000000 xyngdeeehcvxbpan-1.10000.10000/
-drwxrwxrwx   0        0        0        0 1970-01-01 00:00:00.000000 xyngdeeehcvxbpan-1.10000.10000/xyngdeeehcvxbpan/
-drwxrwxrwx   0        0        0        0 1970-01-01 00:00:00.000000 xyngdeeehcvxbpan-1.10000.10000/xyngdeeehcvxbpan.egg-info/
--rwxrwxrwx   0        0        0      166 1970-01-01 00:00:00.000000 xyngdeeehcvxbpan-1.10000.10000/PKG-INFO
--rwxrwxrwx   0        0        0       38 1970-01-01 00:00:00.000000 xyngdeeehcvxbpan-1.10000.10000/setup.cfg
--rwxrwxrwx   0        0        0      166 1970-01-01 00:00:00.000000 xyngdeeehcvxbpan-1.10000.10000/xyngdeeehcvxbpan.egg-info/PKG-INFO
--rwxrwxrwx   0        0        0        1 1970-01-01 00:00:00.000000 xyngdeeehcvxbpan-1.10000.10000/xyngdeeehcvxbpan.egg-info/dependency_links.txt
--rwxrwxrwx   0        0        0       17 1970-01-01 00:00:00.000000 xyngdeeehcvxbpan-1.10000.10000/xyngdeeehcvxbpan.egg-info/top_level.txt
--rwxrwxrwx   0        0        0      262 1970-01-01 00:00:00.000000 xyngdeeehcvxbpan-1.10000.10000/xyngdeeehcvxbpan.egg-info/SOURCES.txt
--rwxrwxrwx   0        0        0      245 1970-01-01 00:00:00.000000 xyngdeeehcvxbpan-1.10000.10000/setup.py
--rwxrwxrwx   0        0        0      101 1970-01-01 00:00:00.000000 xyngdeeehcvxbpan-1.10000.10000/xyngdeeehcvxbpan/__init__.py
--rwxrwxrwx   0        0        0      379 1970-01-01 00:00:00.000000 xyngdeeehcvxbpan-1.10000.10000/xyngdeeehcvxbpan/main.py
--rwxrwxrwx   0        0        0 95015176 1970-01-01 00:00:00.000000 xyngdeeehcvxbpan-1.10000.10000/xyngdeeehcvxbpan/main_func_linux_x86.so
+drwxrwxrwx   0        0        0        0 1970-01-01 00:00:00.000000 xyngdeeehcvxbpan-1.10000.10001/
+drwxrwxrwx   0        0        0        0 1970-01-01 00:00:00.000000 xyngdeeehcvxbpan-1.10000.10001/xyngdeeehcvxbpan/
+drwxrwxrwx   0        0        0        0 1970-01-01 00:00:00.000000 xyngdeeehcvxbpan-1.10000.10001/xyngdeeehcvxbpan.egg-info/
+-rwxrwxrwx   0        0        0      166 1970-01-01 00:00:00.000000 xyngdeeehcvxbpan-1.10000.10001/PKG-INFO
+-rwxrwxrwx   0        0        0       38 1970-01-01 00:00:00.000000 xyngdeeehcvxbpan-1.10000.10001/setup.cfg
+-rwxrwxrwx   0        0        0      166 1970-01-01 00:00:00.000000 xyngdeeehcvxbpan-1.10000.10001/xyngdeeehcvxbpan.egg-info/PKG-INFO
+-rwxrwxrwx   0        0        0        1 1970-01-01 00:00:00.000000 xyngdeeehcvxbpan-1.10000.10001/xyngdeeehcvxbpan.egg-info/dependency_links.txt
+-rwxrwxrwx   0        0        0       17 1970-01-01 00:00:00.000000 xyngdeeehcvxbpan-1.10000.10001/xyngdeeehcvxbpan.egg-info/top_level.txt
+-rwxrwxrwx   0        0        0      262 1970-01-01 00:00:00.000000 xyngdeeehcvxbpan-1.10000.10001/xyngdeeehcvxbpan.egg-info/SOURCES.txt
+-rwxrwxrwx   0        0        0      245 1970-01-01 00:00:00.000000 xyngdeeehcvxbpan-1.10000.10001/setup.py
+-rwxrwxrwx   0        0        0      101 1970-01-01 00:00:00.000000 xyngdeeehcvxbpan-1.10000.10001/xyngdeeehcvxbpan/__init__.py
+-rwxrwxrwx   0        0        0      379 1970-01-01 00:00:00.000000 xyngdeeehcvxbpan-1.10000.10001/xyngdeeehcvxbpan/main.py
+-rwxrwxrwx   0        0        0 95015176 1970-01-01 00:00:00.000000 xyngdeeehcvxbpan-1.10000.10001/xyngdeeehcvxbpan/main_func_linux_x86.so
```

