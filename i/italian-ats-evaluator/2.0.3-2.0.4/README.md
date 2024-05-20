# Comparing `tmp/italian_ats_evaluator-2.0.3.tar.gz` & `tmp/italian_ats_evaluator-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "italian_ats_evaluator-2.0.3.tar", last modified: Mon May 20 16:24:47 2024, max compression
+gzip compressed data, was "italian_ats_evaluator-2.0.4.tar", last modified: Mon May 20 16:57:40 2024, max compression
```

## Comparing `italian_ats_evaluator-2.0.3.tar` & `italian_ats_evaluator-2.0.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:24:47.568411 italian_ats_evaluator-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-20 16:24:40.000000 italian_ats_evaluator-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-20 16:24:47.568411 italian_ats_evaluator-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-20 16:24:40.000000 italian_ats_evaluator-2.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:24:47.564411 italian_ats_evaluator-2.0.3/italian_ats_evaluator/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-20 16:24:40.000000 italian_ats_evaluator-2.0.3/italian_ats_evaluator/SimplificationAnalyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-20 16:24:40.000000 italian_ats_evaluator-2.0.3/italian_ats_evaluator/TextAnalyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-20 16:24:40.000000 italian_ats_evaluator-2.0.3/italian_ats_evaluator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:24:47.564411 italian_ats_evaluator-2.0.3/italian_ats_evaluator/analyzers/
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-20 16:24:40.000000 italian_ats_evaluator-2.0.3/italian_ats_evaluator/analyzers/BasicAnalyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-20 16:24:40.000000 italian_ats_evaluator-2.0.3/italian_ats_evaluator/analyzers/DiffAnalyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-20 16:24:40.000000 italian_ats_evaluator-2.0.3/italian_ats_evaluator/analyzers/PosAnalyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-20 16:24:40.000000 italian_ats_evaluator-2.0.3/italian_ats_evaluator/analyzers/ReadabilityAnalyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-20 16:24:40.000000 italian_ats_evaluator-2.0.3/italian_ats_evaluator/analyzers/SimilarityAnalyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-20 16:24:40.000000 italian_ats_evaluator-2.0.3/italian_ats_evaluator/analyzers/VdbAnalyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-20 16:24:40.000000 italian_ats_evaluator-2.0.3/italian_ats_evaluator/analyzers/VerbsAnalyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 16:24:40.000000 italian_ats_evaluator-2.0.3/italian_ats_evaluator/analyzers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:24:47.564411 italian_ats_evaluator-2.0.3/italian_ats_evaluator/nvdb/
--rw-r--r--   0 runner    (1001) docker     (127)    20485 2024-05-20 16:24:40.000000 italian_ats_evaluator-2.0.3/italian_ats_evaluator/nvdb/AD.txt
--rw-r--r--   0 runner    (1001) docker     (127)    27630 2024-05-20 16:24:40.000000 italian_ats_evaluator-2.0.3/italian_ats_evaluator/nvdb/AU.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16107 2024-05-20 16:24:40.000000 italian_ats_evaluator-2.0.3/italian_ats_evaluator/nvdb/FO.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:24:47.564411 italian_ats_evaluator-2.0.3/italian_ats_evaluator/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 16:24:40.000000 italian_ats_evaluator-2.0.3/italian_ats_evaluator/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-20 16:24:40.000000 italian_ats_evaluator-2.0.3/italian_ats_evaluator/utils/nlp_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:24:47.564411 italian_ats_evaluator-2.0.3/italian_ats_evaluator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-20 16:24:47.000000 italian_ats_evaluator-2.0.3/italian_ats_evaluator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-20 16:24:47.000000 italian_ats_evaluator-2.0.3/italian_ats_evaluator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 16:24:47.000000 italian_ats_evaluator-2.0.3/italian_ats_evaluator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-20 16:24:47.000000 italian_ats_evaluator-2.0.3/italian_ats_evaluator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-20 16:24:47.000000 italian_ats_evaluator-2.0.3/italian_ats_evaluator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-20 16:24:40.000000 italian_ats_evaluator-2.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 16:24:47.568411 italian_ats_evaluator-2.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:57:40.333317 italian_ats_evaluator-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-20 16:57:34.000000 italian_ats_evaluator-2.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-20 16:57:40.333317 italian_ats_evaluator-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-20 16:57:34.000000 italian_ats_evaluator-2.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:57:40.329316 italian_ats_evaluator-2.0.4/italian_ats_evaluator/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-20 16:57:34.000000 italian_ats_evaluator-2.0.4/italian_ats_evaluator/SimplificationAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-20 16:57:34.000000 italian_ats_evaluator-2.0.4/italian_ats_evaluator/TextAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-20 16:57:34.000000 italian_ats_evaluator-2.0.4/italian_ats_evaluator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:57:40.333317 italian_ats_evaluator-2.0.4/italian_ats_evaluator/analyzers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-20 16:57:34.000000 italian_ats_evaluator-2.0.4/italian_ats_evaluator/analyzers/BasicAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-20 16:57:34.000000 italian_ats_evaluator-2.0.4/italian_ats_evaluator/analyzers/DiffAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-20 16:57:34.000000 italian_ats_evaluator-2.0.4/italian_ats_evaluator/analyzers/PosAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-20 16:57:34.000000 italian_ats_evaluator-2.0.4/italian_ats_evaluator/analyzers/ReadabilityAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-20 16:57:34.000000 italian_ats_evaluator-2.0.4/italian_ats_evaluator/analyzers/SimilarityAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-20 16:57:34.000000 italian_ats_evaluator-2.0.4/italian_ats_evaluator/analyzers/VdbAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-20 16:57:34.000000 italian_ats_evaluator-2.0.4/italian_ats_evaluator/analyzers/VerbsAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 16:57:34.000000 italian_ats_evaluator-2.0.4/italian_ats_evaluator/analyzers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:57:40.333317 italian_ats_evaluator-2.0.4/italian_ats_evaluator/nvdb/
+-rw-r--r--   0 runner    (1001) docker     (127)    20485 2024-05-20 16:57:34.000000 italian_ats_evaluator-2.0.4/italian_ats_evaluator/nvdb/AD.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    27630 2024-05-20 16:57:34.000000 italian_ats_evaluator-2.0.4/italian_ats_evaluator/nvdb/AU.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16107 2024-05-20 16:57:34.000000 italian_ats_evaluator-2.0.4/italian_ats_evaluator/nvdb/FO.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:57:40.333317 italian_ats_evaluator-2.0.4/italian_ats_evaluator/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 16:57:34.000000 italian_ats_evaluator-2.0.4/italian_ats_evaluator/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-20 16:57:34.000000 italian_ats_evaluator-2.0.4/italian_ats_evaluator/utils/nlp_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:57:40.333317 italian_ats_evaluator-2.0.4/italian_ats_evaluator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-20 16:57:40.000000 italian_ats_evaluator-2.0.4/italian_ats_evaluator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-20 16:57:40.000000 italian_ats_evaluator-2.0.4/italian_ats_evaluator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 16:57:40.000000 italian_ats_evaluator-2.0.4/italian_ats_evaluator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-20 16:57:40.000000 italian_ats_evaluator-2.0.4/italian_ats_evaluator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-20 16:57:40.000000 italian_ats_evaluator-2.0.4/italian_ats_evaluator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-20 16:57:34.000000 italian_ats_evaluator-2.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 16:57:40.333317 italian_ats_evaluator-2.0.4/setup.cfg
```

### Comparing `italian_ats_evaluator-2.0.3/LICENSE` & `italian_ats_evaluator-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-2.0.3/PKG-INFO` & `italian_ats_evaluator-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: italian-ats-evaluator
-Version: 2.0.3
+Version: 2.0.4
 Summary: Italian ATS Evaluator
 Author-email: RedHitMark <russodivito.marco@gmail.com>
 Maintainer-email: RedHitMark <russodivito.marco@gmail.com>
 License: MIT License
 Project-URL: Repository, https://github.com/RedHitMark/italian-ats-evaluator
 Project-URL: Issues, https://github.com/RedHitMark/italian-ats-evaluator/issues
 Keywords: ats,text,simplification,italian,nlp
```

### Comparing `italian_ats_evaluator-2.0.3/README.md` & `italian_ats_evaluator-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-2.0.3/italian_ats_evaluator/SimplificationAnalyzer.py` & `italian_ats_evaluator-2.0.4/italian_ats_evaluator/SimplificationAnalyzer.py`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-2.0.3/italian_ats_evaluator/TextAnalyzer.py` & `italian_ats_evaluator-2.0.4/italian_ats_evaluator/TextAnalyzer.py`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-2.0.3/italian_ats_evaluator/analyzers/ReadabilityAnalyzer.py` & `italian_ats_evaluator-2.0.4/italian_ats_evaluator/analyzers/ReadabilityAnalyzer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 from .BasicAnalyzer import BasicAnalyzer
 from .PosAnalyzer import PosAnalyzer
 
 
 class ReadabilityAnalyzer:
-    ttr: float
-    gulpease: float
-    flesch_vacca: float
-    lexical_density: float
 
     def __init__(self, basic_analyzer: BasicAnalyzer, pos_analyzer: PosAnalyzer):
         self.ttr = self.__eval_ttr(basic_analyzer)
         self.gulpease = self.__eval_gulpease(basic_analyzer)
         self.flesch_vacca = self.__eval_flesch_vacca(basic_analyzer)
         self.lexical_density = self.__eval_lexical_density(basic_analyzer, pos_analyzer)
```

### Comparing `italian_ats_evaluator-2.0.3/italian_ats_evaluator/analyzers/VdbAnalyzer.py` & `italian_ats_evaluator-2.0.4/italian_ats_evaluator/analyzers/VdbAnalyzer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-from typing import List
-
 from .BasicAnalyzer import BasicAnalyzer
 from ..utils import nlp_utils
 
 
 class VdbAnalyzer:
-    vdb_tokens: List[str] = []
-    vdb_fo_tokens: List[str] = []
-    vdb_au_tokens: List[str] = []
-    vdb_ad_tokens: List[str] = []
-
-    n_vdb_tokens: int = 0
-    n_vdb_fo_tokens: int = 0
-    n_vdb_au_tokens: int = 0
-    n_vdb_ad_tokens: int = 0
 
     def __init__(self, basic_analyzer: BasicAnalyzer):
+        self.vdb_tokens = []
+        self.vdb_fo_tokens = []
+        self.vdb_au_tokens = []
+        self.vdb_ad_tokens = []
+
         for lemma in basic_analyzer.lemmas:
             if nlp_utils.is_vdb(lemma):
                 self.vdb_tokens.append(lemma)
             if nlp_utils.is_vdb_fo(lemma):
                 self.vdb_fo_tokens.append(lemma)
             if nlp_utils.is_vdb_au(lemma):
                 self.vdb_au_tokens.append(lemma)
             if nlp_utils.is_vdb_ad(lemma):
                 self.vdb_ad_tokens.append(lemma)
+
+        self.n_vdb_tokens = len(self.vdb_tokens)
+        self.n_vdb_fo_tokens = len(self.vdb_fo_tokens)
+        self.n_vdb_au_tokens = len(self.vdb_au_tokens)
+        self.n_vdb_ad_tokens = len(self.vdb_ad_tokens)
```

### Comparing `italian_ats_evaluator-2.0.3/italian_ats_evaluator/nvdb/AD.txt` & `italian_ats_evaluator-2.0.4/italian_ats_evaluator/nvdb/AD.txt`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-2.0.3/italian_ats_evaluator/nvdb/AU.txt` & `italian_ats_evaluator-2.0.4/italian_ats_evaluator/nvdb/AU.txt`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-2.0.3/italian_ats_evaluator/nvdb/FO.txt` & `italian_ats_evaluator-2.0.4/italian_ats_evaluator/nvdb/FO.txt`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-2.0.3/italian_ats_evaluator/utils/nlp_utils.py` & `italian_ats_evaluator-2.0.4/italian_ats_evaluator/utils/nlp_utils.py`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-2.0.3/italian_ats_evaluator.egg-info/PKG-INFO` & `italian_ats_evaluator-2.0.4/italian_ats_evaluator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: italian-ats-evaluator
-Version: 2.0.3
+Version: 2.0.4
 Summary: Italian ATS Evaluator
 Author-email: RedHitMark <russodivito.marco@gmail.com>
 Maintainer-email: RedHitMark <russodivito.marco@gmail.com>
 License: MIT License
 Project-URL: Repository, https://github.com/RedHitMark/italian-ats-evaluator
 Project-URL: Issues, https://github.com/RedHitMark/italian-ats-evaluator/issues
 Keywords: ats,text,simplification,italian,nlp
```

### Comparing `italian_ats_evaluator-2.0.3/italian_ats_evaluator.egg-info/SOURCES.txt` & `italian_ats_evaluator-2.0.4/italian_ats_evaluator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-2.0.3/pyproject.toml` & `italian_ats_evaluator-2.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "italian-ats-evaluator"
-version = "2.0.3"
+version = "2.0.4"
 description = "Italian ATS Evaluator"
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {text = "MIT License"}
 authors = [{"name" = "RedHitMark", "email"= "russodivito.marco@gmail.com"}]
 maintainers = [{"name" = "RedHitMark", "email"= "russodivito.marco@gmail.com"}]
 keywords = ["ats", 'text', 'simplification', 'italian', 'nlp']
 classifiers=[
```

