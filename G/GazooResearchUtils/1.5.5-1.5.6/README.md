# Comparing `tmp/GazooResearchUtils-1.5.5.tar.gz` & `tmp/GazooResearchUtils-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GazooResearchUtils-1.5.5.tar", last modified: Sun May 19 23:38:17 2024, max compression
+gzip compressed data, was "GazooResearchUtils-1.5.6.tar", last modified: Sun May 19 23:49:05 2024, max compression
```

## Comparing `GazooResearchUtils-1.5.5.tar` & `GazooResearchUtils-1.5.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-19 23:38:17.578753 GazooResearchUtils-1.5.5/
--rw-r--r--   0 andrewlim   (501) staff       (20)      268 2024-05-19 23:38:17.578401 GazooResearchUtils-1.5.5/PKG-INFO
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-19 23:38:17.576404 GazooResearchUtils-1.5.5/app/
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-19 23:38:17.577052 GazooResearchUtils-1.5.5/app/GazooResearchUtils/
--rw-r--r--   0 andrewlim   (501) staff       (20)      193 2024-05-19 23:38:13.000000 GazooResearchUtils-1.5.5/app/GazooResearchUtils/__init__.py
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-19 23:38:17.578051 GazooResearchUtils-1.5.5/app/GazooResearchUtils/src/
--rw-r--r--   0 andrewlim   (501) staff       (20)     8724 2024-05-19 23:35:05.000000 GazooResearchUtils-1.5.5/app/GazooResearchUtils/src/Analysis.py
--rw-r--r--   0 andrewlim   (501) staff       (20)        0 2024-05-10 21:10:14.000000 GazooResearchUtils-1.5.5/app/GazooResearchUtils/src/__init__.py
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-19 23:38:17.577759 GazooResearchUtils-1.5.5/app/GazooResearchUtils.egg-info/
--rw-r--r--   0 andrewlim   (501) staff       (20)      268 2024-05-19 23:38:17.000000 GazooResearchUtils-1.5.5/app/GazooResearchUtils.egg-info/PKG-INFO
--rw-r--r--   0 andrewlim   (501) staff       (20)      350 2024-05-19 23:38:17.000000 GazooResearchUtils-1.5.5/app/GazooResearchUtils.egg-info/SOURCES.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)        1 2024-05-19 23:38:17.000000 GazooResearchUtils-1.5.5/app/GazooResearchUtils.egg-info/dependency_links.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)       18 2024-05-19 23:38:17.000000 GazooResearchUtils-1.5.5/app/GazooResearchUtils.egg-info/requires.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)       19 2024-05-19 23:38:17.000000 GazooResearchUtils-1.5.5/app/GazooResearchUtils.egg-info/top_level.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)       38 2024-05-19 23:38:17.578843 GazooResearchUtils-1.5.5/setup.cfg
--rw-r--r--   0 andrewlim   (501) staff       (20)      415 2024-05-19 23:38:04.000000 GazooResearchUtils-1.5.5/setup.py
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-19 23:49:05.530020 GazooResearchUtils-1.5.6/
+-rw-r--r--   0 andrewlim   (501) staff       (20)      268 2024-05-19 23:49:05.529780 GazooResearchUtils-1.5.6/PKG-INFO
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-19 23:49:05.527914 GazooResearchUtils-1.5.6/app/
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-19 23:49:05.528331 GazooResearchUtils-1.5.6/app/GazooResearchUtils/
+-rw-r--r--   0 andrewlim   (501) staff       (20)      193 2024-05-19 23:38:13.000000 GazooResearchUtils-1.5.6/app/GazooResearchUtils/__init__.py
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-19 23:49:05.529455 GazooResearchUtils-1.5.6/app/GazooResearchUtils/src/
+-rw-r--r--   0 andrewlim   (501) staff       (20)     8723 2024-05-19 23:48:43.000000 GazooResearchUtils-1.5.6/app/GazooResearchUtils/src/Analysis.py
+-rw-r--r--   0 andrewlim   (501) staff       (20)        0 2024-05-10 21:10:14.000000 GazooResearchUtils-1.5.6/app/GazooResearchUtils/src/__init__.py
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-19 23:49:05.529117 GazooResearchUtils-1.5.6/app/GazooResearchUtils.egg-info/
+-rw-r--r--   0 andrewlim   (501) staff       (20)      268 2024-05-19 23:49:05.000000 GazooResearchUtils-1.5.6/app/GazooResearchUtils.egg-info/PKG-INFO
+-rw-r--r--   0 andrewlim   (501) staff       (20)      350 2024-05-19 23:49:05.000000 GazooResearchUtils-1.5.6/app/GazooResearchUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)        1 2024-05-19 23:49:05.000000 GazooResearchUtils-1.5.6/app/GazooResearchUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)       18 2024-05-19 23:49:05.000000 GazooResearchUtils-1.5.6/app/GazooResearchUtils.egg-info/requires.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)       19 2024-05-19 23:49:05.000000 GazooResearchUtils-1.5.6/app/GazooResearchUtils.egg-info/top_level.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)       38 2024-05-19 23:49:05.530074 GazooResearchUtils-1.5.6/setup.cfg
+-rw-r--r--   0 andrewlim   (501) staff       (20)      415 2024-05-19 23:48:57.000000 GazooResearchUtils-1.5.6/setup.py
```

### Comparing `GazooResearchUtils-1.5.5/app/GazooResearchUtils/src/Analysis.py` & `GazooResearchUtils-1.5.6/app/GazooResearchUtils/src/Analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,15 +254,15 @@
     """
     Creates a Kaplan-Meier plot.
 
     Parameters:
     km (DataFrame): dataframe for kaplan meier
     """
 
-    durations = km.apply(lambda row: time_in_months(row['start-date'], row['end-date']), axis = 1).to_numpy();
+    durations = km.apply(lambda row: time_in_months(row['start-date'], row['end-date']), axis = 1).to_numpy()
     events = km['event'].to_numpy()
 
     kmf = KaplanMeierFitter()
     kmf.fit(durations, event_observed=events)
 
     kmf.plot()
```

