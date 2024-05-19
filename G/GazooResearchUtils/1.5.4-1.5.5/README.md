# Comparing `tmp/GazooResearchUtils-1.5.4.tar.gz` & `tmp/GazooResearchUtils-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GazooResearchUtils-1.5.4.tar", last modified: Sun May 19 23:36:51 2024, max compression
+gzip compressed data, was "GazooResearchUtils-1.5.5.tar", last modified: Sun May 19 23:38:17 2024, max compression
```

## Comparing `GazooResearchUtils-1.5.4.tar` & `GazooResearchUtils-1.5.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-19 23:36:51.808697 GazooResearchUtils-1.5.4/
--rw-r--r--   0 andrewlim   (501) staff       (20)      268 2024-05-19 23:36:51.808461 GazooResearchUtils-1.5.4/PKG-INFO
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-19 23:36:51.806529 GazooResearchUtils-1.5.4/app/
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-19 23:36:51.806933 GazooResearchUtils-1.5.4/app/GazooResearchUtils/
--rw-r--r--   0 andrewlim   (501) staff       (20)      187 2024-05-16 13:57:19.000000 GazooResearchUtils-1.5.4/app/GazooResearchUtils/__init__.py
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-19 23:36:51.808149 GazooResearchUtils-1.5.4/app/GazooResearchUtils/src/
--rw-r--r--   0 andrewlim   (501) staff       (20)     8724 2024-05-19 23:35:05.000000 GazooResearchUtils-1.5.4/app/GazooResearchUtils/src/Analysis.py
--rw-r--r--   0 andrewlim   (501) staff       (20)        0 2024-05-10 21:10:14.000000 GazooResearchUtils-1.5.4/app/GazooResearchUtils/src/__init__.py
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-19 23:36:51.807747 GazooResearchUtils-1.5.4/app/GazooResearchUtils.egg-info/
--rw-r--r--   0 andrewlim   (501) staff       (20)      268 2024-05-19 23:36:51.000000 GazooResearchUtils-1.5.4/app/GazooResearchUtils.egg-info/PKG-INFO
--rw-r--r--   0 andrewlim   (501) staff       (20)      350 2024-05-19 23:36:51.000000 GazooResearchUtils-1.5.4/app/GazooResearchUtils.egg-info/SOURCES.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)        1 2024-05-19 23:36:51.000000 GazooResearchUtils-1.5.4/app/GazooResearchUtils.egg-info/dependency_links.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)       18 2024-05-19 23:36:51.000000 GazooResearchUtils-1.5.4/app/GazooResearchUtils.egg-info/requires.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)       19 2024-05-19 23:36:51.000000 GazooResearchUtils-1.5.4/app/GazooResearchUtils.egg-info/top_level.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)       38 2024-05-19 23:36:51.808756 GazooResearchUtils-1.5.4/setup.cfg
--rw-r--r--   0 andrewlim   (501) staff       (20)      415 2024-05-19 23:36:19.000000 GazooResearchUtils-1.5.4/setup.py
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-19 23:38:17.578753 GazooResearchUtils-1.5.5/
+-rw-r--r--   0 andrewlim   (501) staff       (20)      268 2024-05-19 23:38:17.578401 GazooResearchUtils-1.5.5/PKG-INFO
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-19 23:38:17.576404 GazooResearchUtils-1.5.5/app/
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-19 23:38:17.577052 GazooResearchUtils-1.5.5/app/GazooResearchUtils/
+-rw-r--r--   0 andrewlim   (501) staff       (20)      193 2024-05-19 23:38:13.000000 GazooResearchUtils-1.5.5/app/GazooResearchUtils/__init__.py
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-19 23:38:17.578051 GazooResearchUtils-1.5.5/app/GazooResearchUtils/src/
+-rw-r--r--   0 andrewlim   (501) staff       (20)     8724 2024-05-19 23:35:05.000000 GazooResearchUtils-1.5.5/app/GazooResearchUtils/src/Analysis.py
+-rw-r--r--   0 andrewlim   (501) staff       (20)        0 2024-05-10 21:10:14.000000 GazooResearchUtils-1.5.5/app/GazooResearchUtils/src/__init__.py
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-19 23:38:17.577759 GazooResearchUtils-1.5.5/app/GazooResearchUtils.egg-info/
+-rw-r--r--   0 andrewlim   (501) staff       (20)      268 2024-05-19 23:38:17.000000 GazooResearchUtils-1.5.5/app/GazooResearchUtils.egg-info/PKG-INFO
+-rw-r--r--   0 andrewlim   (501) staff       (20)      350 2024-05-19 23:38:17.000000 GazooResearchUtils-1.5.5/app/GazooResearchUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)        1 2024-05-19 23:38:17.000000 GazooResearchUtils-1.5.5/app/GazooResearchUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)       18 2024-05-19 23:38:17.000000 GazooResearchUtils-1.5.5/app/GazooResearchUtils.egg-info/requires.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)       19 2024-05-19 23:38:17.000000 GazooResearchUtils-1.5.5/app/GazooResearchUtils.egg-info/top_level.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)       38 2024-05-19 23:38:17.578843 GazooResearchUtils-1.5.5/setup.cfg
+-rw-r--r--   0 andrewlim   (501) staff       (20)      415 2024-05-19 23:38:04.000000 GazooResearchUtils-1.5.5/setup.py
```

### Comparing `GazooResearchUtils-1.5.4/app/GazooResearchUtils/src/Analysis.py` & `GazooResearchUtils-1.5.5/app/GazooResearchUtils/src/Analysis.py`

 * *Files identical despite different names*

