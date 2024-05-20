# Comparing `tmp/italian_ats_evaluator-2.0.2.tar.gz` & `tmp/italian_ats_evaluator-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "italian_ats_evaluator-2.0.2.tar", last modified: Mon May 20 16:04:44 2024, max compression
+gzip compressed data, was "italian_ats_evaluator-2.0.3.tar", last modified: Mon May 20 16:24:47 2024, max compression
```

## Comparing `italian_ats_evaluator-2.0.2.tar` & `italian_ats_evaluator-2.0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:04:44.890204 italian_ats_evaluator-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-20 16:04:38.000000 italian_ats_evaluator-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-20 16:04:44.890204 italian_ats_evaluator-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-20 16:04:38.000000 italian_ats_evaluator-2.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:04:44.886204 italian_ats_evaluator-2.0.2/italian_ats_evaluator/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-20 16:04:38.000000 italian_ats_evaluator-2.0.2/italian_ats_evaluator/SimplificationAnalyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-20 16:04:38.000000 italian_ats_evaluator-2.0.2/italian_ats_evaluator/TextAnalyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-20 16:04:38.000000 italian_ats_evaluator-2.0.2/italian_ats_evaluator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:04:44.890204 italian_ats_evaluator-2.0.2/italian_ats_evaluator/analyzers/
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-20 16:04:38.000000 italian_ats_evaluator-2.0.2/italian_ats_evaluator/analyzers/BasicAnalyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-20 16:04:38.000000 italian_ats_evaluator-2.0.2/italian_ats_evaluator/analyzers/DiffAnalyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-20 16:04:38.000000 italian_ats_evaluator-2.0.2/italian_ats_evaluator/analyzers/PosAnalyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-20 16:04:38.000000 italian_ats_evaluator-2.0.2/italian_ats_evaluator/analyzers/ReadabilityAnalyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-20 16:04:38.000000 italian_ats_evaluator-2.0.2/italian_ats_evaluator/analyzers/SimilarityAnalyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-20 16:04:38.000000 italian_ats_evaluator-2.0.2/italian_ats_evaluator/analyzers/VdbAnalyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-20 16:04:38.000000 italian_ats_evaluator-2.0.2/italian_ats_evaluator/analyzers/VerbsAnalyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 16:04:38.000000 italian_ats_evaluator-2.0.2/italian_ats_evaluator/analyzers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:04:44.890204 italian_ats_evaluator-2.0.2/italian_ats_evaluator/nvdb/
--rw-r--r--   0 runner    (1001) docker     (127)    20485 2024-05-20 16:04:38.000000 italian_ats_evaluator-2.0.2/italian_ats_evaluator/nvdb/AD.txt
--rw-r--r--   0 runner    (1001) docker     (127)    27630 2024-05-20 16:04:38.000000 italian_ats_evaluator-2.0.2/italian_ats_evaluator/nvdb/AU.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16107 2024-05-20 16:04:38.000000 italian_ats_evaluator-2.0.2/italian_ats_evaluator/nvdb/FO.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:04:44.890204 italian_ats_evaluator-2.0.2/italian_ats_evaluator/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 16:04:38.000000 italian_ats_evaluator-2.0.2/italian_ats_evaluator/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-20 16:04:38.000000 italian_ats_evaluator-2.0.2/italian_ats_evaluator/utils/nlp_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:04:44.890204 italian_ats_evaluator-2.0.2/italian_ats_evaluator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-20 16:04:44.000000 italian_ats_evaluator-2.0.2/italian_ats_evaluator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-20 16:04:44.000000 italian_ats_evaluator-2.0.2/italian_ats_evaluator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 16:04:44.000000 italian_ats_evaluator-2.0.2/italian_ats_evaluator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-20 16:04:44.000000 italian_ats_evaluator-2.0.2/italian_ats_evaluator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-20 16:04:44.000000 italian_ats_evaluator-2.0.2/italian_ats_evaluator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-20 16:04:38.000000 italian_ats_evaluator-2.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 16:04:44.890204 italian_ats_evaluator-2.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:24:47.568411 italian_ats_evaluator-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-20 16:24:40.000000 italian_ats_evaluator-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-20 16:24:47.568411 italian_ats_evaluator-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-20 16:24:40.000000 italian_ats_evaluator-2.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:24:47.564411 italian_ats_evaluator-2.0.3/italian_ats_evaluator/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-20 16:24:40.000000 italian_ats_evaluator-2.0.3/italian_ats_evaluator/SimplificationAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-20 16:24:40.000000 italian_ats_evaluator-2.0.3/italian_ats_evaluator/TextAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-20 16:24:40.000000 italian_ats_evaluator-2.0.3/italian_ats_evaluator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:24:47.564411 italian_ats_evaluator-2.0.3/italian_ats_evaluator/analyzers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-20 16:24:40.000000 italian_ats_evaluator-2.0.3/italian_ats_evaluator/analyzers/BasicAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-20 16:24:40.000000 italian_ats_evaluator-2.0.3/italian_ats_evaluator/analyzers/DiffAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-20 16:24:40.000000 italian_ats_evaluator-2.0.3/italian_ats_evaluator/analyzers/PosAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-20 16:24:40.000000 italian_ats_evaluator-2.0.3/italian_ats_evaluator/analyzers/ReadabilityAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-20 16:24:40.000000 italian_ats_evaluator-2.0.3/italian_ats_evaluator/analyzers/SimilarityAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-20 16:24:40.000000 italian_ats_evaluator-2.0.3/italian_ats_evaluator/analyzers/VdbAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-20 16:24:40.000000 italian_ats_evaluator-2.0.3/italian_ats_evaluator/analyzers/VerbsAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 16:24:40.000000 italian_ats_evaluator-2.0.3/italian_ats_evaluator/analyzers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:24:47.564411 italian_ats_evaluator-2.0.3/italian_ats_evaluator/nvdb/
+-rw-r--r--   0 runner    (1001) docker     (127)    20485 2024-05-20 16:24:40.000000 italian_ats_evaluator-2.0.3/italian_ats_evaluator/nvdb/AD.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    27630 2024-05-20 16:24:40.000000 italian_ats_evaluator-2.0.3/italian_ats_evaluator/nvdb/AU.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16107 2024-05-20 16:24:40.000000 italian_ats_evaluator-2.0.3/italian_ats_evaluator/nvdb/FO.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:24:47.564411 italian_ats_evaluator-2.0.3/italian_ats_evaluator/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 16:24:40.000000 italian_ats_evaluator-2.0.3/italian_ats_evaluator/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-20 16:24:40.000000 italian_ats_evaluator-2.0.3/italian_ats_evaluator/utils/nlp_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:24:47.564411 italian_ats_evaluator-2.0.3/italian_ats_evaluator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-20 16:24:47.000000 italian_ats_evaluator-2.0.3/italian_ats_evaluator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-20 16:24:47.000000 italian_ats_evaluator-2.0.3/italian_ats_evaluator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 16:24:47.000000 italian_ats_evaluator-2.0.3/italian_ats_evaluator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-20 16:24:47.000000 italian_ats_evaluator-2.0.3/italian_ats_evaluator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-20 16:24:47.000000 italian_ats_evaluator-2.0.3/italian_ats_evaluator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-20 16:24:40.000000 italian_ats_evaluator-2.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 16:24:47.568411 italian_ats_evaluator-2.0.3/setup.cfg
```

### Comparing `italian_ats_evaluator-2.0.2/LICENSE` & `italian_ats_evaluator-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-2.0.2/PKG-INFO` & `italian_ats_evaluator-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: italian-ats-evaluator
-Version: 2.0.2
+Version: 2.0.3
 Summary: Italian ATS Evaluator
 Author-email: RedHitMark <russodivito.marco@gmail.com>
 Maintainer-email: RedHitMark <russodivito.marco@gmail.com>
 License: MIT License
 Project-URL: Repository, https://github.com/RedHitMark/italian-ats-evaluator
 Project-URL: Issues, https://github.com/RedHitMark/italian-ats-evaluator/issues
 Keywords: ats,text,simplification,italian,nlp
```

### Comparing `italian_ats_evaluator-2.0.2/README.md` & `italian_ats_evaluator-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-2.0.2/italian_ats_evaluator/SimplificationAnalyzer.py` & `italian_ats_evaluator-2.0.3/italian_ats_evaluator/SimplificationAnalyzer.py`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-2.0.2/italian_ats_evaluator/TextAnalyzer.py` & `italian_ats_evaluator-2.0.3/italian_ats_evaluator/TextAnalyzer.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,14 +18,14 @@
     verbs: VerbsAnalyzer
     vdb: VdbAnalyzer
     readability: ReadabilityAnalyzer
 
     def __init__(self, text: str):
         self.text = text
         self.text_cleaned = nlp_utils.clean_text(text)
-        self.text_processed = nlp_utils.get_model()(self.text_cleaned)
+        self.text_processed = nlp_utils.get_spacy_model()(self.text_cleaned)
 
         self.basic = BasicAnalyzer(self.text_processed)
         self.pos = PosAnalyzer(self.text_processed)
         self.verbs = VerbsAnalyzer(self.text_processed)
         self.vdb = VdbAnalyzer(self.basic)
         self.readability = ReadabilityAnalyzer(self.basic, self.pos)
```

### Comparing `italian_ats_evaluator-2.0.2/italian_ats_evaluator/analyzers/BasicAnalyzer.py` & `italian_ats_evaluator-2.0.3/italian_ats_evaluator/analyzers/BasicAnalyzer.py`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-2.0.2/italian_ats_evaluator/analyzers/DiffAnalyzer.py` & `italian_ats_evaluator-2.0.3/italian_ats_evaluator/analyzers/DiffAnalyzer.py`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-2.0.2/italian_ats_evaluator/analyzers/PosAnalyzer.py` & `italian_ats_evaluator-2.0.3/italian_ats_evaluator/analyzers/PosAnalyzer.py`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-2.0.2/italian_ats_evaluator/analyzers/ReadabilityAnalyzer.py` & `italian_ats_evaluator-2.0.3/italian_ats_evaluator/analyzers/ReadabilityAnalyzer.py`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-2.0.2/italian_ats_evaluator/analyzers/SimilarityAnalyzer.py` & `italian_ats_evaluator-2.0.3/italian_ats_evaluator/analyzers/SimilarityAnalyzer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,17 @@
+from ..utils import nlp_utils
 from sentence_transformers import SentenceTransformer, util
 
 
 class SimilarityAnalyzer:
-    __model: SentenceTransformer
-
     semantic_similarity: float
 
     def __init__(self, reference_text: str, simplified_text: str):
-        self.__model = SentenceTransformer('sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2')
+        model = nlp_utils.get_sentence_transformers_model()
 
-        embeddings1 = self.__model.encode([reference_text], convert_to_numpy=True)
-        embeddings2 = self.__model.encode([simplified_text], convert_to_numpy=True)
+        embeddings1 = model.encode([reference_text], convert_to_numpy=True)
+        embeddings2 = model.encode([simplified_text], convert_to_numpy=True)
         cosine_scores = util.cos_sim(embeddings1, embeddings2)
 
         self.semantic_similarity = float(cosine_scores[0][0]) * 100.0
```

### Comparing `italian_ats_evaluator-2.0.2/italian_ats_evaluator/analyzers/VdbAnalyzer.py` & `italian_ats_evaluator-2.0.3/italian_ats_evaluator/analyzers/VdbAnalyzer.py`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-2.0.2/italian_ats_evaluator/analyzers/VerbsAnalyzer.py` & `italian_ats_evaluator-2.0.3/italian_ats_evaluator/analyzers/VerbsAnalyzer.py`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-2.0.2/italian_ats_evaluator/nvdb/AD.txt` & `italian_ats_evaluator-2.0.3/italian_ats_evaluator/nvdb/AD.txt`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-2.0.2/italian_ats_evaluator/nvdb/AU.txt` & `italian_ats_evaluator-2.0.3/italian_ats_evaluator/nvdb/AU.txt`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-2.0.2/italian_ats_evaluator/nvdb/FO.txt` & `italian_ats_evaluator-2.0.3/italian_ats_evaluator/nvdb/FO.txt`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-2.0.2/italian_ats_evaluator/utils/nlp_utils.py` & `italian_ats_evaluator-2.0.3/italian_ats_evaluator/utils/nlp_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,40 @@
 import spacy
 import pyphen
 import pkgutil
+from sentence_transformers import SentenceTransformer
 
 dic = pyphen.Pyphen(lang='it')
 
 italian_vdb_fo = {a for a in pkgutil.get_data('italian_ats_evaluator', 'nvdb/FO.txt').decode('utf-8').split('\r\n')}
 italian_vdb_au = {a for a in pkgutil.get_data('italian_ats_evaluator', 'nvdb/AU.txt').decode('utf-8').split('\r\n')}
 italian_vdb_ad = {a for a in pkgutil.get_data('italian_ats_evaluator', 'nvdb/AD.txt').decode('utf-8').split('\r\n')}
 italian_vdb = italian_vdb_fo.union(italian_vdb_au).union(italian_vdb_ad)
 
 
-def get_model() -> spacy.language.Language:
-    try:
-        return spacy.load("it_core_news_lg")
-    except OSError:
-        spacy.cli.download("it_core_news_lg")
-        return spacy.load("it_core_news_lg")
+spacy_model = None
+sentence_transformers_model = None
+
+
+def get_spacy_model() -> spacy.language.Language:
+    global spacy_model
+    if spacy_model is None:
+        try:
+            spacy_model = spacy.load("it_core_news_lg")
+        except OSError:
+            spacy.cli.download("it_core_news_lg")
+            spacy_model = spacy.load("it_core_news_lg")
+    return spacy_model
+
+
+def get_sentence_transformers_model():
+    global sentence_transformers_model
+    if sentence_transformers_model is None:
+        sentence_transformers_model = SentenceTransformer('all-MiniLM-L6-v2')
+    return sentence_transformers_model
 
 
 def clean_text(text: str) -> str:
     text = text.strip()
     text = text.replace("\r\n", " ")
     text = text.replace("\n", " ")
     text = text.replace("\r", " ")
```

### Comparing `italian_ats_evaluator-2.0.2/italian_ats_evaluator.egg-info/PKG-INFO` & `italian_ats_evaluator-2.0.3/italian_ats_evaluator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: italian-ats-evaluator
-Version: 2.0.2
+Version: 2.0.3
 Summary: Italian ATS Evaluator
 Author-email: RedHitMark <russodivito.marco@gmail.com>
 Maintainer-email: RedHitMark <russodivito.marco@gmail.com>
 License: MIT License
 Project-URL: Repository, https://github.com/RedHitMark/italian-ats-evaluator
 Project-URL: Issues, https://github.com/RedHitMark/italian-ats-evaluator/issues
 Keywords: ats,text,simplification,italian,nlp
```

### Comparing `italian_ats_evaluator-2.0.2/italian_ats_evaluator.egg-info/SOURCES.txt` & `italian_ats_evaluator-2.0.3/italian_ats_evaluator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `italian_ats_evaluator-2.0.2/pyproject.toml` & `italian_ats_evaluator-2.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "italian-ats-evaluator"
-version = "2.0.2"
+version = "2.0.3"
 description = "Italian ATS Evaluator"
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {text = "MIT License"}
 authors = [{"name" = "RedHitMark", "email"= "russodivito.marco@gmail.com"}]
 maintainers = [{"name" = "RedHitMark", "email"= "russodivito.marco@gmail.com"}]
 keywords = ["ats", 'text', 'simplification', 'italian', 'nlp']
 classifiers=[
```

