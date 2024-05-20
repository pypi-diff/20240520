# Comparing `tmp/DPRED-1.0.2.tar.gz` & `tmp/DPRED-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DPRED-1.0.2.tar", last modified: Fri May 17 23:02:01 2024, max compression
+gzip compressed data, was "DPRED-1.0.3.tar", last modified: Mon May 20 14:17:48 2024, max compression
```

## Comparing `DPRED-1.0.2.tar` & `DPRED-1.0.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 23:02:01.304637 DPRED-1.0.2/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 23:01:59.761529 DPRED-1.0.2/DPRED/
--rwxrwxrwx   0 root         (0) root         (0)       52 2024-05-17 21:45:14.000000 DPRED-1.0.2/DPRED/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1166 2024-05-17 21:45:16.000000 DPRED-1.0.2/DPRED/blast.py
--rwxrwxrwx   0 root         (0) root         (0)     5980 2024-05-17 23:01:46.000000 DPRED-1.0.2/DPRED/get_pdb_data.py
--rwxrwxrwx   0 root         (0) root         (0)     2556 2024-05-17 23:01:44.000000 DPRED-1.0.2/DPRED/get_pdb_files.py
--rwxrwxrwx   0 root         (0) root         (0)     1257 2024-05-17 23:01:48.000000 DPRED-1.0.2/DPRED/get_uniprot_data.py
--rwxrwxrwx   0 root         (0) root         (0)      751 2024-05-17 22:48:50.000000 DPRED-1.0.2/DPRED/hmm.py
--rwxrwxrwx   0 root         (0) root         (0)     2993 2024-05-17 22:48:54.000000 DPRED-1.0.2/DPRED/main.py
--rwxrwxrwx   0 root         (0) root         (0)     3403 2024-05-17 22:49:26.000000 DPRED-1.0.2/DPRED/msa.py
--rwxrwxrwx   0 root         (0) root         (0)     1572 2024-05-17 22:49:31.000000 DPRED-1.0.2/DPRED/performance.py
--rwxrwxrwx   0 root         (0) root         (0)      271 2024-05-17 21:45:32.000000 DPRED-1.0.2/DPRED/remove.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 23:02:01.126357 DPRED-1.0.2/DPRED/src/
--rwxrwxrwx   0 root         (0) root         (0)    11686 2018-07-26 08:18:18.000000 DPRED-1.0.2/DPRED/src/Kabsch.h
--rwxrwxrwx   0 root         (0) root         (0)      109 2022-01-04 04:17:11.000000 DPRED-1.0.2/DPRED/src/Makefile
--rwxrwxrwx   0 root         (0) root         (0)     6006 2018-07-26 08:18:17.000000 DPRED-1.0.2/DPRED/src/NW.h
--rwxrwxrwx   0 root         (0) root         (0)    72079 2022-01-05 10:38:25.000000 DPRED-1.0.2/DPRED/src/TMM.cpp
--rwxrwxrwx   0 root         (0) root         (0)     3657 2022-01-04 06:07:35.000000 DPRED-1.0.2/DPRED/src/TMM.h
--rwxrwxrwx   0 root         (0) root         (0)    36346 2018-07-26 08:18:17.000000 DPRED-1.0.2/DPRED/src/TMalign.h
--rwxrwxrwx   0 root         (0) root         (0)    14228 2018-07-26 08:18:17.000000 DPRED-1.0.2/DPRED/src/TMalign_main.h
--rwxrwxrwx   0 root         (0) root         (0)    14694 2018-07-26 08:18:17.000000 DPRED-1.0.2/DPRED/src/UPGMA.cpp
--rwxrwxrwx   0 root         (0) root         (0)     1973 2018-07-26 08:18:17.000000 DPRED-1.0.2/DPRED/src/UPGMA.h
--rwxrwxrwx   0 root         (0) root         (0)    14990 2018-09-13 06:40:53.000000 DPRED-1.0.2/DPRED/src/basic_fun.h
--rwxrwxrwx   0 root         (0) root         (0)   347960 2024-04-30 10:42:08.000000 DPRED-1.0.2/DPRED/src/mTM-align
--rwxrwxrwx   0 root         (0) root         (0)     4179 2022-01-05 10:48:54.000000 DPRED-1.0.2/DPRED/src/main.cpp
--rwxrwxrwx   0 root         (0) root         (0)     7687 2024-05-17 21:45:34.000000 DPRED-1.0.2/DPRED/validation.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 23:02:00.093772 DPRED-1.0.2/DPRED.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      538 2024-05-17 23:01:58.000000 DPRED-1.0.2/DPRED.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      683 2024-05-17 23:01:58.000000 DPRED-1.0.2/DPRED.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-17 23:01:58.000000 DPRED-1.0.2/DPRED.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       42 2024-05-17 23:01:58.000000 DPRED-1.0.2/DPRED.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)       25 2024-05-17 23:01:58.000000 DPRED-1.0.2/DPRED.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        6 2024-05-17 23:01:58.000000 DPRED-1.0.2/DPRED.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:35:08.000000 DPRED-1.0.2/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)       19 2024-05-17 21:26:51.000000 DPRED-1.0.2/MANIFEST.in
--rwxrwxrwx   0 root         (0) root         (0)      538 2024-05-17 23:02:01.285634 DPRED-1.0.2/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:35:02.000000 DPRED-1.0.2/README.md
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-17 23:02:01.317490 DPRED-1.0.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      963 2024-05-17 23:01:34.000000 DPRED-1.0.2/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 23:02:01.229620 DPRED-1.0.2/tests/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:34:27.000000 DPRED-1.0.2/tests/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:34:35.000000 DPRED-1.0.2/tests/test_main.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-20 14:17:48.684698 DPRED-1.0.3/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-20 14:17:47.377428 DPRED-1.0.3/DPRED/
+-rwxrwxrwx   0 root         (0) root         (0)       52 2024-05-17 21:45:14.000000 DPRED-1.0.3/DPRED/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1166 2024-05-17 21:45:16.000000 DPRED-1.0.3/DPRED/blast.py
+-rwxrwxrwx   0 root         (0) root         (0)     5980 2024-05-17 23:01:46.000000 DPRED-1.0.3/DPRED/get_pdb_data.py
+-rwxrwxrwx   0 root         (0) root         (0)     2556 2024-05-17 23:01:44.000000 DPRED-1.0.3/DPRED/get_pdb_files.py
+-rwxrwxrwx   0 root         (0) root         (0)     1257 2024-05-17 23:01:48.000000 DPRED-1.0.3/DPRED/get_uniprot_data.py
+-rwxrwxrwx   0 root         (0) root         (0)      751 2024-05-17 22:48:50.000000 DPRED-1.0.3/DPRED/hmm.py
+-rwxrwxrwx   0 root         (0) root         (0)     2993 2024-05-17 22:48:54.000000 DPRED-1.0.3/DPRED/main.py
+-rwxrwxrwx   0 root         (0) root         (0)     3403 2024-05-17 22:49:26.000000 DPRED-1.0.3/DPRED/msa.py
+-rwxrwxrwx   0 root         (0) root         (0)     7455 2024-05-20 14:14:09.000000 DPRED-1.0.3/DPRED/performance.py
+-rwxrwxrwx   0 root         (0) root         (0)      271 2024-05-17 21:45:32.000000 DPRED-1.0.3/DPRED/remove.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-20 14:17:48.527576 DPRED-1.0.3/DPRED/src/
+-rwxrwxrwx   0 root         (0) root         (0)    11686 2018-07-26 08:18:18.000000 DPRED-1.0.3/DPRED/src/Kabsch.h
+-rwxrwxrwx   0 root         (0) root         (0)      109 2022-01-04 04:17:11.000000 DPRED-1.0.3/DPRED/src/Makefile
+-rwxrwxrwx   0 root         (0) root         (0)     6006 2018-07-26 08:18:17.000000 DPRED-1.0.3/DPRED/src/NW.h
+-rwxrwxrwx   0 root         (0) root         (0)    72079 2022-01-05 10:38:25.000000 DPRED-1.0.3/DPRED/src/TMM.cpp
+-rwxrwxrwx   0 root         (0) root         (0)     3657 2022-01-04 06:07:35.000000 DPRED-1.0.3/DPRED/src/TMM.h
+-rwxrwxrwx   0 root         (0) root         (0)    36346 2018-07-26 08:18:17.000000 DPRED-1.0.3/DPRED/src/TMalign.h
+-rwxrwxrwx   0 root         (0) root         (0)    14228 2018-07-26 08:18:17.000000 DPRED-1.0.3/DPRED/src/TMalign_main.h
+-rwxrwxrwx   0 root         (0) root         (0)    14694 2018-07-26 08:18:17.000000 DPRED-1.0.3/DPRED/src/UPGMA.cpp
+-rwxrwxrwx   0 root         (0) root         (0)     1973 2018-07-26 08:18:17.000000 DPRED-1.0.3/DPRED/src/UPGMA.h
+-rwxrwxrwx   0 root         (0) root         (0)    14990 2018-09-13 06:40:53.000000 DPRED-1.0.3/DPRED/src/basic_fun.h
+-rwxrwxrwx   0 root         (0) root         (0)   347960 2024-04-30 10:42:08.000000 DPRED-1.0.3/DPRED/src/mTM-align
+-rwxrwxrwx   0 root         (0) root         (0)     4179 2022-01-05 10:48:54.000000 DPRED-1.0.3/DPRED/src/main.cpp
+-rwxrwxrwx   0 root         (0) root         (0)     7687 2024-05-17 21:45:34.000000 DPRED-1.0.3/DPRED/validation.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-20 14:17:47.665615 DPRED-1.0.3/DPRED.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     3321 2024-05-20 14:17:45.000000 DPRED-1.0.3/DPRED.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      683 2024-05-20 14:17:46.000000 DPRED-1.0.3/DPRED.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-20 14:17:45.000000 DPRED-1.0.3/DPRED.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       42 2024-05-20 14:17:45.000000 DPRED-1.0.3/DPRED.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)       25 2024-05-20 14:17:45.000000 DPRED-1.0.3/DPRED.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        6 2024-05-20 14:17:45.000000 DPRED-1.0.3/DPRED.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:35:08.000000 DPRED-1.0.3/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)       19 2024-05-17 21:26:51.000000 DPRED-1.0.3/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)     3321 2024-05-20 14:17:48.669012 DPRED-1.0.3/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2831 2024-05-18 11:11:29.000000 DPRED-1.0.3/README.md
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-20 14:17:48.684698 DPRED-1.0.3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      965 2024-05-20 14:17:25.000000 DPRED-1.0.3/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-20 14:17:48.621313 DPRED-1.0.3/tests/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:34:27.000000 DPRED-1.0.3/tests/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:34:35.000000 DPRED-1.0.3/tests/test_main.py
```

### Comparing `DPRED-1.0.2/DPRED/blast.py` & `DPRED-1.0.3/DPRED/blast.py`

 * *Files identical despite different names*

### Comparing `DPRED-1.0.2/DPRED/get_pdb_data.py` & `DPRED-1.0.3/DPRED/get_pdb_data.py`

 * *Files identical despite different names*

### Comparing `DPRED-1.0.2/DPRED/get_pdb_files.py` & `DPRED-1.0.3/DPRED/get_pdb_files.py`

 * *Files identical despite different names*

### Comparing `DPRED-1.0.2/DPRED/get_uniprot_data.py` & `DPRED-1.0.3/DPRED/get_uniprot_data.py`

 * *Files identical despite different names*

### Comparing `DPRED-1.0.2/DPRED/hmm.py` & `DPRED-1.0.3/DPRED/hmm.py`

 * *Files identical despite different names*

### Comparing `DPRED-1.0.2/DPRED/main.py` & `DPRED-1.0.3/DPRED/main.py`

 * *Files identical despite different names*

### Comparing `DPRED-1.0.2/DPRED/msa.py` & `DPRED-1.0.3/DPRED/msa.py`

 * *Files identical despite different names*

### Comparing `DPRED-1.0.2/DPRED/src/Kabsch.h` & `DPRED-1.0.3/DPRED/src/Kabsch.h`

 * *Files identical despite different names*

### Comparing `DPRED-1.0.2/DPRED/src/NW.h` & `DPRED-1.0.3/DPRED/src/NW.h`

 * *Files identical despite different names*

### Comparing `DPRED-1.0.2/DPRED/src/TMM.cpp` & `DPRED-1.0.3/DPRED/src/TMM.cpp`

 * *Files identical despite different names*

### Comparing `DPRED-1.0.2/DPRED/src/TMM.h` & `DPRED-1.0.3/DPRED/src/TMM.h`

 * *Files identical despite different names*

### Comparing `DPRED-1.0.2/DPRED/src/TMalign.h` & `DPRED-1.0.3/DPRED/src/TMalign.h`

 * *Files identical despite different names*

### Comparing `DPRED-1.0.2/DPRED/src/TMalign_main.h` & `DPRED-1.0.3/DPRED/src/TMalign_main.h`

 * *Files identical despite different names*

### Comparing `DPRED-1.0.2/DPRED/src/UPGMA.cpp` & `DPRED-1.0.3/DPRED/src/UPGMA.cpp`

 * *Files identical despite different names*

### Comparing `DPRED-1.0.2/DPRED/src/UPGMA.h` & `DPRED-1.0.3/DPRED/src/UPGMA.h`

 * *Files identical despite different names*

### Comparing `DPRED-1.0.2/DPRED/src/basic_fun.h` & `DPRED-1.0.3/DPRED/src/basic_fun.h`

 * *Files identical despite different names*

### Comparing `DPRED-1.0.2/DPRED/src/mTM-align` & `DPRED-1.0.3/DPRED/src/mTM-align`

 * *Files identical despite different names*

### Comparing `DPRED-1.0.2/DPRED/src/main.cpp` & `DPRED-1.0.3/DPRED/src/main.cpp`

 * *Files identical despite different names*

### Comparing `DPRED-1.0.2/DPRED/validation.py` & `DPRED-1.0.3/DPRED/validation.py`

 * *Files identical despite different names*

### Comparing `DPRED-1.0.2/DPRED.egg-info/SOURCES.txt` & `DPRED-1.0.3/DPRED.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DPRED-1.0.2/setup.py` & `DPRED-1.0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='DPRED',
-    version='1.0.2',
+    version='1.0.3',
     packages=find_packages(include=['DPRED', 'DPRED.*']),
     install_requires=[
         'biopython',
         'requests',
         'numpy',
     ],
     entry_points={
@@ -26,8 +26,8 @@
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.6',
     include_package_data=True,
     package_data={
         'DPRED': ['src/*'],
     },
-)
+)
```

