# Comparing `tmp/italian_ats_evaluator-1.0.2.tar.gz` & `tmp/italian_ats_evaluator-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "italian_ats_evaluator-1.0.2.tar", last modified: Sat May 18 20:50:56 2024, max compression
+gzip compressed data, was "italian_ats_evaluator-2.0.0.tar", last modified: Mon May 20 15:46:02 2024, max compression
```

## Comparing `italian_ats_evaluator-1.0.2.tar` & `italian_ats_evaluator-2.0.0.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 20:50:56.255311 italian_ats_evaluator-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-18 20:50:50.000000 italian_ats_evaluator-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-18 20:50:56.255311 italian_ats_evaluator-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-18 20:50:50.000000 italian_ats_evaluator-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 20:50:56.251311 italian_ats_evaluator-1.0.2/italian_ats_evaluator/
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-18 20:50:50.000000 italian_ats_evaluator-1.0.2/italian_ats_evaluator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 20:50:56.255311 italian_ats_evaluator-1.0.2/italian_ats_evaluator/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 20:50:50.000000 italian_ats_evaluator-1.0.2/italian_ats_evaluator/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-18 20:50:50.000000 italian_ats_evaluator-1.0.2/italian_ats_evaluator/analysis/basic_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-18 20:50:50.000000 italian_ats_evaluator-1.0.2/italian_ats_evaluator/analysis/diff_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-18 20:50:50.000000 italian_ats_evaluator-1.0.2/italian_ats_evaluator/analysis/pos_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-18 20:50:50.000000 italian_ats_evaluator-1.0.2/italian_ats_evaluator/analysis/readability_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-18 20:50:50.000000 italian_ats_evaluator-1.0.2/italian_ats_evaluator/analysis/similarity_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-18 20:50:50.000000 italian_ats_evaluator-1.0.2/italian_ats_evaluator/analysis/vdb_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 20:50:56.255311 italian_ats_evaluator-1.0.2/italian_ats_evaluator/nvdb/
--rw-r--r--   0 runner    (1001) docker     (127)    20485 2024-05-18 20:50:50.000000 italian_ats_evaluator-1.0.2/italian_ats_evaluator/nvdb/AD.txt
--rw-r--r--   0 runner    (1001) docker     (127)    27630 2024-05-18 20:50:50.000000 italian_ats_evaluator-1.0.2/italian_ats_evaluator/nvdb/AU.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16107 2024-05-18 20:50:50.000000 italian_ats_evaluator-1.0.2/italian_ats_evaluator/nvdb/FO.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 20:50:56.255311 italian_ats_evaluator-1.0.2/italian_ats_evaluator/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 20:50:50.000000 italian_ats_evaluator-1.0.2/italian_ats_evaluator/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-18 20:50:50.000000 italian_ats_evaluator-1.0.2/italian_ats_evaluator/utils/nlp_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 20:50:56.255311 italian_ats_evaluator-1.0.2/italian_ats_evaluator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-18 20:50:56.000000 italian_ats_evaluator-1.0.2/italian_ats_evaluator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-18 20:50:56.000000 italian_ats_evaluator-1.0.2/italian_ats_evaluator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 20:50:56.000000 italian_ats_evaluator-1.0.2/italian_ats_evaluator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-18 20:50:56.000000 italian_ats_evaluator-1.0.2/italian_ats_evaluator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-18 20:50:56.000000 italian_ats_evaluator-1.0.2/italian_ats_evaluator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-18 20:50:50.000000 italian_ats_evaluator-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 20:50:56.255311 italian_ats_evaluator-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:46:02.237399 italian_ats_evaluator-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-20 15:45:56.000000 italian_ats_evaluator-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-20 15:46:02.237399 italian_ats_evaluator-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-20 15:45:56.000000 italian_ats_evaluator-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:46:02.233399 italian_ats_evaluator-2.0.0/italian_ats_evaluator/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-20 15:45:56.000000 italian_ats_evaluator-2.0.0/italian_ats_evaluator/SimplificationAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-20 15:45:56.000000 italian_ats_evaluator-2.0.0/italian_ats_evaluator/TextAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-20 15:45:56.000000 italian_ats_evaluator-2.0.0/italian_ats_evaluator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:46:02.233399 italian_ats_evaluator-2.0.0/italian_ats_evaluator/analyzers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-20 15:45:56.000000 italian_ats_evaluator-2.0.0/italian_ats_evaluator/analyzers/BasicAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-20 15:45:56.000000 italian_ats_evaluator-2.0.0/italian_ats_evaluator/analyzers/DiffAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-20 15:45:56.000000 italian_ats_evaluator-2.0.0/italian_ats_evaluator/analyzers/PosAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-20 15:45:56.000000 italian_ats_evaluator-2.0.0/italian_ats_evaluator/analyzers/ReadabilityAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-20 15:45:56.000000 italian_ats_evaluator-2.0.0/italian_ats_evaluator/analyzers/SimilarityAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-20 15:45:56.000000 italian_ats_evaluator-2.0.0/italian_ats_evaluator/analyzers/VdbAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-20 15:45:56.000000 italian_ats_evaluator-2.0.0/italian_ats_evaluator/analyzers/VerbsAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 15:45:56.000000 italian_ats_evaluator-2.0.0/italian_ats_evaluator/analyzers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:46:02.233399 italian_ats_evaluator-2.0.0/italian_ats_evaluator/nvdb/
+-rw-r--r--   0 runner    (1001) docker     (127)    20485 2024-05-20 15:45:56.000000 italian_ats_evaluator-2.0.0/italian_ats_evaluator/nvdb/AD.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    27630 2024-05-20 15:45:56.000000 italian_ats_evaluator-2.0.0/italian_ats_evaluator/nvdb/AU.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16107 2024-05-20 15:45:56.000000 italian_ats_evaluator-2.0.0/italian_ats_evaluator/nvdb/FO.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:46:02.233399 italian_ats_evaluator-2.0.0/italian_ats_evaluator/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:45:56.000000 italian_ats_evaluator-2.0.0/italian_ats_evaluator/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-20 15:45:56.000000 italian_ats_evaluator-2.0.0/italian_ats_evaluator/utils/nlp_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:46:02.237399 italian_ats_evaluator-2.0.0/italian_ats_evaluator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-20 15:46:02.000000 italian_ats_evaluator-2.0.0/italian_ats_evaluator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-20 15:46:02.000000 italian_ats_evaluator-2.0.0/italian_ats_evaluator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 15:46:02.000000 italian_ats_evaluator-2.0.0/italian_ats_evaluator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-20 15:46:02.000000 italian_ats_evaluator-2.0.0/italian_ats_evaluator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-20 15:46:02.000000 italian_ats_evaluator-2.0.0/italian_ats_evaluator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-20 15:45:56.000000 italian_ats_evaluator-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 15:46:02.237399 italian_ats_evaluator-2.0.0/setup.cfg
```

### Comparing `italian_ats_evaluator-1.0.2/LICENSE` & `italian_ats_evaluator-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-1.0.2/PKG-INFO` & `italian_ats_evaluator-2.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: italian-ats-evaluator
-Version: 1.0.2
+Version: 2.0.0
 Summary: Italian ATS Evaluator
 Author-email: RedHitMark <russodivito.marco@gmail.com>
 Maintainer-email: RedHitMark <russodivito.marco@gmail.com>
 License: MIT License
 Project-URL: Repository, https://github.com/RedHitMark/italian-ats-evaluator
 Project-URL: Issues, https://github.com/RedHitMark/italian-ats-evaluator/issues
 Keywords: ats,text,simplification,italian,nlp
@@ -55,15 +55,15 @@
   - Gulpease Index
   - Flesch-Vacca Index
   - Lexical Density
 - Part of Speech (POS) distribution
 - Verbs distribution
   - Active Verbs
   - Passive Verbs
-- Italian Basic Vocabulary (VdB) by [Tullio De Mauro](https://dizionario.internazionale.it/)
+- Italian Basic Vocabulary (NVdB) from [Il Nuovo vocabolario di base della lingua italiana, Tullio De Mauro](https://dizionario.internazionale.it/)
   - All
   - FO (Fundamentals)
   - AU (High Usage)
   - AD (High Availability)
 
 
 You can also compare two texts and get the following metrics:
@@ -82,25 +82,27 @@
 ```bash
 pip install italian-ats-evaluator
 ```
 
 ## Usage
 
 ```python
-import italian_ats_evaluator
+from italian_ats_evaluator import TextAnalyzer
 
-text_analyzed = italian_ats_evaluator.analyze_text("Il gatto mangia il topo")
+result = TextAnalyzer(
+  text="Il gatto mangia il topo"
+)
 ```
 
 ```python
-import italian_ats_evaluator
+from italian_ats_evaluator import SimplificationAnalyzer
 
-text_analyzed, simplified_analyzed, comparion =  italian_ats_evaluator.compare(
-    ref_text="Il felino mangia il roditore",
-    simplified_text="Il gatto mangia il topo",
+result =  SimplificationAnalyzer(
+    reference_text="Il felino mangia il roditore",
+    simplified_text="Il gatto mangia il topo"
 )
 ```
 
 ## Development
 Create a virtual environment
 ```bash
 python3 -m venv venv
```

### Comparing `italian_ats_evaluator-1.0.2/README.md` & `italian_ats_evaluator-2.0.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -16,15 +16,15 @@
   - Gulpease Index
   - Flesch-Vacca Index
   - Lexical Density
 - Part of Speech (POS) distribution
 - Verbs distribution
   - Active Verbs
   - Passive Verbs
-- Italian Basic Vocabulary (VdB) by [Tullio De Mauro](https://dizionario.internazionale.it/)
+- Italian Basic Vocabulary (NVdB) from [Il Nuovo vocabolario di base della lingua italiana, Tullio De Mauro](https://dizionario.internazionale.it/)
   - All
   - FO (Fundamentals)
   - AU (High Usage)
   - AD (High Availability)
 
 
 You can also compare two texts and get the following metrics:
@@ -43,25 +43,27 @@
 ```bash
 pip install italian-ats-evaluator
 ```
 
 ## Usage
 
 ```python
-import italian_ats_evaluator
+from italian_ats_evaluator import TextAnalyzer
 
-text_analyzed = italian_ats_evaluator.analyze_text("Il gatto mangia il topo")
+result = TextAnalyzer(
+  text="Il gatto mangia il topo"
+)
 ```
 
 ```python
-import italian_ats_evaluator
+from italian_ats_evaluator import SimplificationAnalyzer
 
-text_analyzed, simplified_analyzed, comparion =  italian_ats_evaluator.compare(
-    ref_text="Il felino mangia il roditore",
-    simplified_text="Il gatto mangia il topo",
+result =  SimplificationAnalyzer(
+    reference_text="Il felino mangia il roditore",
+    simplified_text="Il gatto mangia il topo"
 )
 ```
 
 ## Development
 Create a virtual environment
 ```bash
 python3 -m venv venv
```

### Comparing `italian_ats_evaluator-1.0.2/italian_ats_evaluator/analysis/vdb_analysis.py` & `italian_ats_evaluator-2.0.0/italian_ats_evaluator/utils/nlp_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,47 @@
+import spacy
+import pyphen
 import pkgutil
 
+dic = pyphen.Pyphen(lang='it')
+
 italian_vdb_fo = {a for a in pkgutil.get_data('italian_ats_evaluator', 'nvdb/FO.txt').decode('utf-8').split('\r\n')}
 italian_vdb_au = {a for a in pkgutil.get_data('italian_ats_evaluator', 'nvdb/AU.txt').decode('utf-8').split('\r\n')}
 italian_vdb_ad = {a for a in pkgutil.get_data('italian_ats_evaluator', 'nvdb/AD.txt').decode('utf-8').split('\r\n')}
 italian_vdb = italian_vdb_fo.union(italian_vdb_au).union(italian_vdb_ad)
 
 
+def get_model() -> spacy.language.Language:
+    try:
+        return spacy.load("it_core_news_lg")
+    except OSError:
+        spacy.cli.download("it_core_news_lg")
+        return spacy.load("it_core_news_lg")
+
+
+def clean_text(text: str) -> str:
+    text = text.strip()
+    text = text.replace("\r\n", " ")
+    text = text.replace("\n", " ")
+    text = text.replace("\r", " ")
+    text = text.replace("\t", " ")
+    return " ".join(text.split())
+
+
+def eval_syllables(token: str):
+    return dic.inserted(token).split('-')
+
+
 def is_vdb(lemma: str):
     return lemma in italian_vdb
 
 
 def is_vdb_fo(lemma: str):
     return lemma in italian_vdb_fo
 
 
 def is_vdb_au(lemma: str):
     return lemma in italian_vdb_au
 
 
 def is_vdb_ad(lemma: str):
-    return lemma in italian_vdb_ad
-
-
-def do_vdb_analysis(lemmas: list[str]):
-    return {
-        "all": [lemma for lemma in lemmas if is_vdb(lemma)],
-        "fo": [lemma for lemma in lemmas if is_vdb_fo(lemma)],
-        "au": [lemma for lemma in lemmas if is_vdb_au(lemma)],
-        "ad": [lemma for lemma in lemmas if is_vdb_ad(lemma)]
-    }
+    return lemma in italian_vdb_ad
```

### Comparing `italian_ats_evaluator-1.0.2/italian_ats_evaluator/nvdb/AD.txt` & `italian_ats_evaluator-2.0.0/italian_ats_evaluator/nvdb/AD.txt`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-1.0.2/italian_ats_evaluator/nvdb/AU.txt` & `italian_ats_evaluator-2.0.0/italian_ats_evaluator/nvdb/AU.txt`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-1.0.2/italian_ats_evaluator/nvdb/FO.txt` & `italian_ats_evaluator-2.0.0/italian_ats_evaluator/nvdb/FO.txt`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-1.0.2/italian_ats_evaluator.egg-info/PKG-INFO` & `italian_ats_evaluator-2.0.0/italian_ats_evaluator.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: italian-ats-evaluator
-Version: 1.0.2
+Version: 2.0.0
 Summary: Italian ATS Evaluator
 Author-email: RedHitMark <russodivito.marco@gmail.com>
 Maintainer-email: RedHitMark <russodivito.marco@gmail.com>
 License: MIT License
 Project-URL: Repository, https://github.com/RedHitMark/italian-ats-evaluator
 Project-URL: Issues, https://github.com/RedHitMark/italian-ats-evaluator/issues
 Keywords: ats,text,simplification,italian,nlp
@@ -55,15 +55,15 @@
   - Gulpease Index
   - Flesch-Vacca Index
   - Lexical Density
 - Part of Speech (POS) distribution
 - Verbs distribution
   - Active Verbs
   - Passive Verbs
-- Italian Basic Vocabulary (VdB) by [Tullio De Mauro](https://dizionario.internazionale.it/)
+- Italian Basic Vocabulary (NVdB) from [Il Nuovo vocabolario di base della lingua italiana, Tullio De Mauro](https://dizionario.internazionale.it/)
   - All
   - FO (Fundamentals)
   - AU (High Usage)
   - AD (High Availability)
 
 
 You can also compare two texts and get the following metrics:
@@ -82,25 +82,27 @@
 ```bash
 pip install italian-ats-evaluator
 ```
 
 ## Usage
 
 ```python
-import italian_ats_evaluator
+from italian_ats_evaluator import TextAnalyzer
 
-text_analyzed = italian_ats_evaluator.analyze_text("Il gatto mangia il topo")
+result = TextAnalyzer(
+  text="Il gatto mangia il topo"
+)
 ```
 
 ```python
-import italian_ats_evaluator
+from italian_ats_evaluator import SimplificationAnalyzer
 
-text_analyzed, simplified_analyzed, comparion =  italian_ats_evaluator.compare(
-    ref_text="Il felino mangia il roditore",
-    simplified_text="Il gatto mangia il topo",
+result =  SimplificationAnalyzer(
+    reference_text="Il felino mangia il roditore",
+    simplified_text="Il gatto mangia il topo"
 )
 ```
 
 ## Development
 Create a virtual environment
 ```bash
 python3 -m venv venv
```

### Comparing `italian_ats_evaluator-1.0.2/pyproject.toml` & `italian_ats_evaluator-2.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "italian-ats-evaluator"
-version = "1.0.2"
+version = "2.0.0"
 description = "Italian ATS Evaluator"
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {text = "MIT License"}
 authors = [{"name" = "RedHitMark", "email"= "russodivito.marco@gmail.com"}]
 maintainers = [{"name" = "RedHitMark", "email"= "russodivito.marco@gmail.com"}]
 keywords = ["ats", 'text', 'simplification', 'italian', 'nlp']
 classifiers=[
```

