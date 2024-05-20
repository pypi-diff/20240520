# Comparing `tmp/italian_ats_evaluator-2.0.1.tar.gz` & `tmp/italian_ats_evaluator-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "italian_ats_evaluator-2.0.1.tar", last modified: Mon May 20 15:55:02 2024, max compression
+gzip compressed data, was "italian_ats_evaluator-2.0.2.tar", last modified: Mon May 20 16:04:44 2024, max compression
```

## Comparing `italian_ats_evaluator-2.0.1.tar` & `italian_ats_evaluator-2.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:55:02.304635 italian_ats_evaluator-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-20 15:54:55.000000 italian_ats_evaluator-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-20 15:55:02.304635 italian_ats_evaluator-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-20 15:54:55.000000 italian_ats_evaluator-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:55:02.300635 italian_ats_evaluator-2.0.1/italian_ats_evaluator/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-20 15:54:55.000000 italian_ats_evaluator-2.0.1/italian_ats_evaluator/SimplificationAnalyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-20 15:54:55.000000 italian_ats_evaluator-2.0.1/italian_ats_evaluator/TextAnalyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-20 15:54:55.000000 italian_ats_evaluator-2.0.1/italian_ats_evaluator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:55:02.304635 italian_ats_evaluator-2.0.1/italian_ats_evaluator/analyzers/
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-20 15:54:55.000000 italian_ats_evaluator-2.0.1/italian_ats_evaluator/analyzers/BasicAnalyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-20 15:54:55.000000 italian_ats_evaluator-2.0.1/italian_ats_evaluator/analyzers/DiffAnalyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-20 15:54:55.000000 italian_ats_evaluator-2.0.1/italian_ats_evaluator/analyzers/PosAnalyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-20 15:54:55.000000 italian_ats_evaluator-2.0.1/italian_ats_evaluator/analyzers/ReadabilityAnalyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-20 15:54:55.000000 italian_ats_evaluator-2.0.1/italian_ats_evaluator/analyzers/SimilarityAnalyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-20 15:54:55.000000 italian_ats_evaluator-2.0.1/italian_ats_evaluator/analyzers/VdbAnalyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-20 15:54:55.000000 italian_ats_evaluator-2.0.1/italian_ats_evaluator/analyzers/VerbsAnalyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 15:54:55.000000 italian_ats_evaluator-2.0.1/italian_ats_evaluator/analyzers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:55:02.304635 italian_ats_evaluator-2.0.1/italian_ats_evaluator/nvdb/
--rw-r--r--   0 runner    (1001) docker     (127)    20485 2024-05-20 15:54:55.000000 italian_ats_evaluator-2.0.1/italian_ats_evaluator/nvdb/AD.txt
--rw-r--r--   0 runner    (1001) docker     (127)    27630 2024-05-20 15:54:55.000000 italian_ats_evaluator-2.0.1/italian_ats_evaluator/nvdb/AU.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16107 2024-05-20 15:54:55.000000 italian_ats_evaluator-2.0.1/italian_ats_evaluator/nvdb/FO.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:55:02.304635 italian_ats_evaluator-2.0.1/italian_ats_evaluator/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:54:55.000000 italian_ats_evaluator-2.0.1/italian_ats_evaluator/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-20 15:54:55.000000 italian_ats_evaluator-2.0.1/italian_ats_evaluator/utils/nlp_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:55:02.304635 italian_ats_evaluator-2.0.1/italian_ats_evaluator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-20 15:55:02.000000 italian_ats_evaluator-2.0.1/italian_ats_evaluator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-20 15:55:02.000000 italian_ats_evaluator-2.0.1/italian_ats_evaluator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 15:55:02.000000 italian_ats_evaluator-2.0.1/italian_ats_evaluator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-20 15:55:02.000000 italian_ats_evaluator-2.0.1/italian_ats_evaluator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-20 15:55:02.000000 italian_ats_evaluator-2.0.1/italian_ats_evaluator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-20 15:54:55.000000 italian_ats_evaluator-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 15:55:02.304635 italian_ats_evaluator-2.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:04:44.890204 italian_ats_evaluator-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-20 16:04:38.000000 italian_ats_evaluator-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-20 16:04:44.890204 italian_ats_evaluator-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-20 16:04:38.000000 italian_ats_evaluator-2.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:04:44.886204 italian_ats_evaluator-2.0.2/italian_ats_evaluator/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-20 16:04:38.000000 italian_ats_evaluator-2.0.2/italian_ats_evaluator/SimplificationAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-20 16:04:38.000000 italian_ats_evaluator-2.0.2/italian_ats_evaluator/TextAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-20 16:04:38.000000 italian_ats_evaluator-2.0.2/italian_ats_evaluator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:04:44.890204 italian_ats_evaluator-2.0.2/italian_ats_evaluator/analyzers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-20 16:04:38.000000 italian_ats_evaluator-2.0.2/italian_ats_evaluator/analyzers/BasicAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-20 16:04:38.000000 italian_ats_evaluator-2.0.2/italian_ats_evaluator/analyzers/DiffAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-20 16:04:38.000000 italian_ats_evaluator-2.0.2/italian_ats_evaluator/analyzers/PosAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-20 16:04:38.000000 italian_ats_evaluator-2.0.2/italian_ats_evaluator/analyzers/ReadabilityAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-20 16:04:38.000000 italian_ats_evaluator-2.0.2/italian_ats_evaluator/analyzers/SimilarityAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-20 16:04:38.000000 italian_ats_evaluator-2.0.2/italian_ats_evaluator/analyzers/VdbAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-20 16:04:38.000000 italian_ats_evaluator-2.0.2/italian_ats_evaluator/analyzers/VerbsAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 16:04:38.000000 italian_ats_evaluator-2.0.2/italian_ats_evaluator/analyzers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:04:44.890204 italian_ats_evaluator-2.0.2/italian_ats_evaluator/nvdb/
+-rw-r--r--   0 runner    (1001) docker     (127)    20485 2024-05-20 16:04:38.000000 italian_ats_evaluator-2.0.2/italian_ats_evaluator/nvdb/AD.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    27630 2024-05-20 16:04:38.000000 italian_ats_evaluator-2.0.2/italian_ats_evaluator/nvdb/AU.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16107 2024-05-20 16:04:38.000000 italian_ats_evaluator-2.0.2/italian_ats_evaluator/nvdb/FO.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:04:44.890204 italian_ats_evaluator-2.0.2/italian_ats_evaluator/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 16:04:38.000000 italian_ats_evaluator-2.0.2/italian_ats_evaluator/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-20 16:04:38.000000 italian_ats_evaluator-2.0.2/italian_ats_evaluator/utils/nlp_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:04:44.890204 italian_ats_evaluator-2.0.2/italian_ats_evaluator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-20 16:04:44.000000 italian_ats_evaluator-2.0.2/italian_ats_evaluator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-20 16:04:44.000000 italian_ats_evaluator-2.0.2/italian_ats_evaluator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 16:04:44.000000 italian_ats_evaluator-2.0.2/italian_ats_evaluator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-20 16:04:44.000000 italian_ats_evaluator-2.0.2/italian_ats_evaluator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-20 16:04:44.000000 italian_ats_evaluator-2.0.2/italian_ats_evaluator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-20 16:04:38.000000 italian_ats_evaluator-2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 16:04:44.890204 italian_ats_evaluator-2.0.2/setup.cfg
```

### Comparing `italian_ats_evaluator-2.0.1/LICENSE` & `italian_ats_evaluator-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-2.0.1/PKG-INFO` & `italian_ats_evaluator-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: italian-ats-evaluator
-Version: 2.0.1
+Version: 2.0.2
 Summary: Italian ATS Evaluator
 Author-email: RedHitMark <russodivito.marco@gmail.com>
 Maintainer-email: RedHitMark <russodivito.marco@gmail.com>
 License: MIT License
 Project-URL: Repository, https://github.com/RedHitMark/italian-ats-evaluator
 Project-URL: Issues, https://github.com/RedHitMark/italian-ats-evaluator/issues
 Keywords: ats,text,simplification,italian,nlp
```

### Comparing `italian_ats_evaluator-2.0.1/README.md` & `italian_ats_evaluator-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-2.0.1/italian_ats_evaluator/SimplificationAnalyzer.py` & `italian_ats_evaluator-2.0.2/italian_ats_evaluator/SimplificationAnalyzer.py`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-2.0.1/italian_ats_evaluator/TextAnalyzer.py` & `italian_ats_evaluator-2.0.2/italian_ats_evaluator/TextAnalyzer.py`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-2.0.1/italian_ats_evaluator/analyzers/BasicAnalyzer.py` & `italian_ats_evaluator-2.0.2/italian_ats_evaluator/analyzers/BasicAnalyzer.py`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-2.0.1/italian_ats_evaluator/analyzers/DiffAnalyzer.py` & `italian_ats_evaluator-2.0.2/italian_ats_evaluator/analyzers/DiffAnalyzer.py`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-2.0.1/italian_ats_evaluator/analyzers/PosAnalyzer.py` & `italian_ats_evaluator-2.0.2/italian_ats_evaluator/analyzers/PosAnalyzer.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,56 +7,58 @@
     "NOUN": "nouns",
     "AUX": "verbs",
     "VERB": "verbs",
     "NUM": "number",
     "SYM": "symbols",
     "ADV": "adverbs",
     "DET": "articles",
-    "PART": "particle",
     "PRON": "pronouns",
+    "PART": "particles",
     "ADJ": "adjectives",
     "ADP": "prepositions",
-    "INTJ": "interjection",
     "PROPN": "proper_nouns",
     "PUNCT": "punctuations",
-    "CCONJ": "coordinating_conjunction",
-    "SCONJ": "subordinating_conjunction",
+    "INTJ": "interjections",
+    "CCONJ": "coordinating_conjunctions",
+    "SCONJ": "subordinating_conjunctions",
 }
 
 
 class PosAnalyzer:
     other: List[str] = []
     nouns: List[str] = []
     verbs: List[str] = []
     number: List[str] = []
     symbols: List[str] = []
     adverbs: List[str] = []
     articles: List[str] = []
-    particle: List[str] = []
     pronouns: List[str] = []
+    particles: List[str] = []
     adjectives: List[str] = []
     prepositions: List[str] = []
     proper_nouns: List[str] = []
-    interjection: List[str] = []
     punctuations: List[str] = []
-    coordinating_conjunction: List[str] = []
-    subordinating_conjunction: List[str] = []
+    interjections: List[str] = []
+    coordinating_conjunctions: List[str] = []
+    subordinating_conjunctions: List[str] = []
 
     def __init__(self, processed_text: Doc):
         for token in processed_text:
             if token.pos_ in POS_MAP:
                 getattr(self, POS_MAP[token.pos_]).append(token.text)
 
         self.n_other = len(self.other)
         self.n_nouns = len(self.nouns)
         self.n_verbs = len(self.verbs)
         self.n_number = len(self.number)
         self.n_symbols = len(self.symbols)
         self.n_adverbs = len(self.adverbs)
         self.n_articles = len(self.articles)
         self.n_pronouns = len(self.pronouns)
+        self.n_particles = len(self.particles)
         self.n_adjectives = len(self.adjectives)
         self.n_prepositions = len(self.prepositions)
         self.n_proper_nouns = len(self.proper_nouns)
         self.n_punctuations = len(self.punctuations)
-        self.n_coordinating_conjunction = len(self.coordinating_conjunction)
-        self.n_subordinating_conjunction = len(self.subordinating_conjunction)
+        self.n_interjections = len(self.interjections)
+        self.n_coordinating_conjunctions = len(self.coordinating_conjunctions)
+        self.n_subordinating_conjunctions = len(self.subordinating_conjunctions)
```

### Comparing `italian_ats_evaluator-2.0.1/italian_ats_evaluator/analyzers/ReadabilityAnalyzer.py` & `italian_ats_evaluator-2.0.2/italian_ats_evaluator/analyzers/ReadabilityAnalyzer.py`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-2.0.1/italian_ats_evaluator/analyzers/SimilarityAnalyzer.py` & `italian_ats_evaluator-2.0.2/italian_ats_evaluator/analyzers/SimilarityAnalyzer.py`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-2.0.1/italian_ats_evaluator/analyzers/VdbAnalyzer.py` & `italian_ats_evaluator-2.0.2/italian_ats_evaluator/analyzers/VdbAnalyzer.py`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-2.0.1/italian_ats_evaluator/analyzers/VerbsAnalyzer.py` & `italian_ats_evaluator-2.0.2/italian_ats_evaluator/analyzers/VerbsAnalyzer.py`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-2.0.1/italian_ats_evaluator/nvdb/AD.txt` & `italian_ats_evaluator-2.0.2/italian_ats_evaluator/nvdb/AD.txt`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-2.0.1/italian_ats_evaluator/nvdb/AU.txt` & `italian_ats_evaluator-2.0.2/italian_ats_evaluator/nvdb/AU.txt`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-2.0.1/italian_ats_evaluator/nvdb/FO.txt` & `italian_ats_evaluator-2.0.2/italian_ats_evaluator/nvdb/FO.txt`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-2.0.1/italian_ats_evaluator/utils/nlp_utils.py` & `italian_ats_evaluator-2.0.2/italian_ats_evaluator/utils/nlp_utils.py`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-2.0.1/italian_ats_evaluator.egg-info/PKG-INFO` & `italian_ats_evaluator-2.0.2/italian_ats_evaluator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: italian-ats-evaluator
-Version: 2.0.1
+Version: 2.0.2
 Summary: Italian ATS Evaluator
 Author-email: RedHitMark <russodivito.marco@gmail.com>
 Maintainer-email: RedHitMark <russodivito.marco@gmail.com>
 License: MIT License
 Project-URL: Repository, https://github.com/RedHitMark/italian-ats-evaluator
 Project-URL: Issues, https://github.com/RedHitMark/italian-ats-evaluator/issues
 Keywords: ats,text,simplification,italian,nlp
```

### Comparing `italian_ats_evaluator-2.0.1/italian_ats_evaluator.egg-info/SOURCES.txt` & `italian_ats_evaluator-2.0.2/italian_ats_evaluator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-2.0.1/pyproject.toml` & `italian_ats_evaluator-2.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "italian-ats-evaluator"
-version = "2.0.1"
+version = "2.0.2"
 description = "Italian ATS Evaluator"
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {text = "MIT License"}
 authors = [{"name" = "RedHitMark", "email"= "russodivito.marco@gmail.com"}]
 maintainers = [{"name" = "RedHitMark", "email"= "russodivito.marco@gmail.com"}]
 keywords = ["ats", 'text', 'simplification', 'italian', 'nlp']
 classifiers=[
```

