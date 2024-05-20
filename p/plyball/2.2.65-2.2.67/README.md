# Comparing `tmp/plyball-2.2.65.tar.gz` & `tmp/plyball-2.2.67.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plyball-2.2.65.tar", last modified: Mon May 20 01:17:02 2024, max compression
+gzip compressed data, was "plyball-2.2.67.tar", max compression
```

## Comparing `plyball-2.2.65.tar` & `plyball-2.2.67.tar`

### file list

```diff
@@ -1,43 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:17:02.451050 plyball-2.2.65/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-20 01:16:54.000000 plyball-2.2.65/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-20 01:16:54.000000 plyball-2.2.65/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-20 01:17:02.451050 plyball-2.2.65/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-20 01:16:54.000000 plyball-2.2.65/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:17:02.447050 plyball-2.2.65/plyball/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 01:16:54.000000 plyball-2.2.65/plyball/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:17:02.447050 plyball-2.2.65/plyball/baseballreference/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-20 01:16:54.000000 plyball-2.2.65/plyball/baseballreference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9610 2024-05-20 01:16:54.000000 plyball-2.2.65/plyball/baseballreference/baseballreference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:17:02.447050 plyball-2.2.65/plyball/fangraphs/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-20 01:16:54.000000 plyball-2.2.65/plyball/fangraphs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15578 2024-05-20 01:16:54.000000 plyball-2.2.65/plyball/fangraphs/fangraphs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:17:02.447050 plyball-2.2.65/plyball/lahman/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-20 01:16:54.000000 plyball-2.2.65/plyball/lahman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-05-20 01:16:54.000000 plyball-2.2.65/plyball/lahman/lahman.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:17:02.447050 plyball-2.2.65/plyball/mlb/
--rw-r--r--   0 runner    (1001) docker     (127)     6013 2024-05-20 01:16:54.000000 plyball-2.2.65/plyball/mlb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:17:02.447050 plyball-2.2.65/plyball/ottoneu/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-20 01:16:54.000000 plyball-2.2.65/plyball/ottoneu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13950 2024-05-20 01:16:54.000000 plyball-2.2.65/plyball/ottoneu/ottoneu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:17:02.447050 plyball-2.2.65/plyball/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 01:16:54.000000 plyball-2.2.65/plyball/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-20 01:16:54.000000 plyball-2.2.65/plyball/pipeline/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-05-20 01:16:54.000000 plyball-2.2.65/plyball/player_id_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-20 01:16:54.000000 plyball-2.2.65/plyball/player_map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:17:02.451050 plyball-2.2.65/plyball/retrosheet/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-20 01:16:54.000000 plyball-2.2.65/plyball/retrosheet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8085 2024-05-20 01:16:54.000000 plyball-2.2.65/plyball/retrosheet/retrosheet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:17:02.451050 plyball-2.2.65/plyball/statcast/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-20 01:16:54.000000 plyball-2.2.65/plyball/statcast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14792 2024-05-20 01:16:54.000000 plyball-2.2.65/plyball/statcast/statcast.py
--rw-r--r--   0 runner    (1001) docker     (127)     4433 2024-05-20 01:16:54.000000 plyball-2.2.65/plyball/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:17:02.451050 plyball-2.2.65/plyball.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-20 01:17:02.000000 plyball-2.2.65/plyball.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-20 01:17:02.000000 plyball-2.2.65/plyball.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 01:17:02.000000 plyball-2.2.65/plyball.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-20 01:17:02.000000 plyball-2.2.65/plyball.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-20 01:17:02.000000 plyball-2.2.65/plyball.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 01:17:02.451050 plyball-2.2.65/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-05-20 01:16:54.000000 plyball-2.2.65/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:17:02.451050 plyball-2.2.65/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-20 01:16:54.000000 plyball-2.2.65/tests/__init__.py
+-rw-r--r--   0        0        0     1076 2024-05-20 15:10:28.732353 plyball-2.2.67/LICENSE.txt
+-rw-r--r--   0        0        0      819 2024-05-20 15:10:28.732353 plyball-2.2.67/README.md
+-rw-r--r--   0        0        0       22 2024-05-20 15:10:28.732353 plyball-2.2.67/plyball/__init__.py
+-rw-r--r--   0        0        0       48 2024-05-20 15:10:28.732353 plyball-2.2.67/plyball/baseballreference/__init__.py
+-rw-r--r--   0        0        0     9610 2024-05-20 15:10:28.732353 plyball-2.2.67/plyball/baseballreference/baseballreference.py
+-rw-r--r--   0        0        0       33 2024-05-20 15:10:28.732353 plyball-2.2.67/plyball/fangraphs/__init__.py
+-rw-r--r--   0        0        0    15578 2024-05-20 15:10:28.732353 plyball-2.2.67/plyball/fangraphs/fangraphs.py
+-rw-r--r--   0        0        0       26 2024-05-20 15:10:28.732353 plyball-2.2.67/plyball/lahman/__init__.py
+-rw-r--r--   0        0        0    10203 2024-05-20 15:10:28.732353 plyball-2.2.67/plyball/lahman/lahman.py
+-rw-r--r--   0        0        0     6013 2024-05-20 15:10:28.732353 plyball-2.2.67/plyball/mlb/__init__.py
+-rw-r--r--   0        0        0       28 2024-05-20 15:10:28.732353 plyball-2.2.67/plyball/ottoneu/__init__.py
+-rw-r--r--   0        0        0    13950 2024-05-20 15:10:28.732353 plyball-2.2.67/plyball/ottoneu/ottoneu.py
+-rw-r--r--   0        0        0        0 2024-05-20 15:10:28.732353 plyball-2.2.67/plyball/pipeline/__init__.py
+-rw-r--r--   0        0        0     3019 2024-05-20 15:10:28.732353 plyball-2.2.67/plyball/pipeline/evaluation.py
+-rw-r--r--   0        0        0     3517 2024-05-20 15:10:28.732353 plyball-2.2.67/plyball/player_id_lookup.py
+-rw-r--r--   0        0        0      268 2024-05-20 15:10:28.732353 plyball-2.2.67/plyball/player_map.py
+-rw-r--r--   0        0        0       35 2024-05-20 15:10:28.732353 plyball-2.2.67/plyball/retrosheet/__init__.py
+-rw-r--r--   0        0        0     8085 2024-05-20 15:10:28.732353 plyball-2.2.67/plyball/retrosheet/retrosheet.py
+-rw-r--r--   0        0        0       30 2024-05-20 15:10:28.732353 plyball-2.2.67/plyball/statcast/__init__.py
+-rw-r--r--   0        0        0    14792 2024-05-20 15:10:28.732353 plyball-2.2.67/plyball/statcast/statcast.py
+-rw-r--r--   0        0        0     4433 2024-05-20 15:10:28.732353 plyball-2.2.67/plyball/utils.py
+-rw-r--r--   0        0        0     2875 2024-05-20 15:10:28.736353 plyball-2.2.67/pyproject.toml
+-rw-r--r--   0        0        0     2631 1970-01-01 00:00:00.000000 plyball-2.2.67/PKG-INFO
```

### Comparing `plyball-2.2.65/LICENSE.txt` & `plyball-2.2.67/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plyball-2.2.65/PKG-INFO` & `plyball-2.2.67/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,58 @@
 Metadata-Version: 2.1
 Name: plyball
-Version: 2.2.65
-Summary: A simple package for scraping baseball data from the most popular sites.
-Home-page: https://github.com/waaronmorris/plyball
+Version: 2.2.67
+Summary: 
 Author: W. Aaron Morris
-Author-email: w.aaron.morris@gmail.com
-License: MIT
-Keywords: baseball sabermetrics data statistics statcast web scraping
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 2.7
+Author-email: waaronmorris@gmail.com
+Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: alabaster (==0.7.13)
+Requires-Dist: babel (==2.12.1)
+Requires-Dist: beautifulsoup4 (==4.12.2)
+Requires-Dist: bleach (==6.0.0)
+Requires-Dist: bs4 (==0.0.1)
+Requires-Dist: certifi (==2022.12.7)
+Requires-Dist: chardet (==5.1.0)
+Requires-Dist: docutils (==0.19)
+Requires-Dist: flake8 (>=7.0.0,<8.0.0)
+Requires-Dist: idna (==3.4)
+Requires-Dist: imagesize (==1.4.1)
+Requires-Dist: jinja2 (==3.1.2)
+Requires-Dist: keyring (==23.13.1)
+Requires-Dist: lxml (==4.9.2)
+Requires-Dist: markupsafe (==2.1.2)
+Requires-Dist: numpy (==1.24.2)
+Requires-Dist: packaging (==23.1)
+Requires-Dist: pandas (==2.0.0)
+Requires-Dist: pkginfo (==1.9.6)
+Requires-Dist: pygments (==2.15.0)
+Requires-Dist: pyparsing (==3.0.9)
+Requires-Dist: python-dateutil (==2.8.2)
+Requires-Dist: readme-renderer (==37.3)
+Requires-Dist: requests (==2.31.0)
+Requires-Dist: requests-toolbelt (==0.10.1)
+Requires-Dist: six (==1.16.0)
+Requires-Dist: snowballstemmer (==2.2.0)
+Requires-Dist: soupsieve (==2.4.1)
+Requires-Dist: sphinx (>=6.1.3)
+Requires-Dist: sphinxcontrib-applehelp (>=1.0.4)
+Requires-Dist: sphinxcontrib-devhelp (>=1.0.2)
+Requires-Dist: sphinxcontrib-htmlhelp (>=2.0.1)
+Requires-Dist: sphinxcontrib-jsmath (>=1.0.1)
+Requires-Dist: sphinxcontrib-qthelp (>=1.0.2)
+Requires-Dist: sphinxcontrib-serializinghtml (>=1.1.3)
+Requires-Dist: structlog (==23.2.0)
+Requires-Dist: tqdm (==4.42.1)
+Requires-Dist: twine (==3.1.1)
+Requires-Dist: urllib3 (==1.26.5)
+Requires-Dist: webencodings (==0.5.1)
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: numpy>=1.24
-Requires-Dist: pandas>=2.0.0
-Requires-Dist: beautifulsoup4>=4.4.0
-Requires-Dist: requests>=2.31.0
-Requires-Dist: lxml>=4.2.1
-Requires-Dist: structlog>=23.2.0
 
 # Overview
 **plyball** is a Python package providing a extracting data from several of 
 the most popular baseball sources (Fangraphs, Statcast, etc...). A majority 
 of these sources are scraped. 
 
 ## Where to get it
```

### Comparing `plyball-2.2.65/README.md` & `plyball-2.2.67/README.md`

 * *Files identical despite different names*

### Comparing `plyball-2.2.65/plyball/baseballreference/baseballreference.py` & `plyball-2.2.67/plyball/baseballreference/baseballreference.py`

 * *Files identical despite different names*

### Comparing `plyball-2.2.65/plyball/fangraphs/fangraphs.py` & `plyball-2.2.67/plyball/fangraphs/fangraphs.py`

 * *Files identical despite different names*

### Comparing `plyball-2.2.65/plyball/lahman/lahman.py` & `plyball-2.2.67/plyball/lahman/lahman.py`

 * *Files identical despite different names*

### Comparing `plyball-2.2.65/plyball/mlb/__init__.py` & `plyball-2.2.67/plyball/mlb/__init__.py`

 * *Files identical despite different names*

### Comparing `plyball-2.2.65/plyball/ottoneu/ottoneu.py` & `plyball-2.2.67/plyball/ottoneu/ottoneu.py`

 * *Files identical despite different names*

### Comparing `plyball-2.2.65/plyball/pipeline/evaluation.py` & `plyball-2.2.67/plyball/pipeline/evaluation.py`

 * *Files identical despite different names*

### Comparing `plyball-2.2.65/plyball/player_id_lookup.py` & `plyball-2.2.67/plyball/player_id_lookup.py`

 * *Files identical despite different names*

### Comparing `plyball-2.2.65/plyball/retrosheet/retrosheet.py` & `plyball-2.2.67/plyball/retrosheet/retrosheet.py`

 * *Files identical despite different names*

### Comparing `plyball-2.2.65/plyball/statcast/statcast.py` & `plyball-2.2.67/plyball/statcast/statcast.py`

 * *Files identical despite different names*

### Comparing `plyball-2.2.65/plyball/utils.py` & `plyball-2.2.67/plyball/utils.py`

 * *Files identical despite different names*

