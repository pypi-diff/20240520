# Comparing `tmp/FastHPOCR-0.1.0.tar.gz` & `tmp/FastHPOCR-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FastHPOCR-0.1.0.tar", last modified: Wed May 15 13:43:38 2024, max compression
+gzip compressed data, was "FastHPOCR-0.1.1.tar", last modified: Mon May 20 10:59:05 2024, max compression
```

## Comparing `FastHPOCR-0.1.0.tar` & `FastHPOCR-0.1.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 tudor      (501) staff       (20)        0 2024-05-15 13:43:38.373817 FastHPOCR-0.1.0/
-drwxr-xr-x   0 tudor      (501) staff       (20)        0 2024-05-15 13:43:38.366516 FastHPOCR-0.1.0/FastHPOCR/
--rw-r--r--   0 tudor      (501) staff       (20)     1295 2024-05-15 11:08:04.000000 FastHPOCR-0.1.0/FastHPOCR/HPOAnnotator.py
--rw-r--r--   0 tudor      (501) staff       (20)     4837 2024-05-15 13:34:45.000000 FastHPOCR-0.1.0/FastHPOCR/IndexHPO.py
--rw-r--r--   0 tudor      (501) staff       (20)     3491 2024-05-15 11:09:02.000000 FastHPOCR-0.1.0/FastHPOCR/IndexORPHANET.py
--rw-r--r--   0 tudor      (501) staff       (20)     4492 2024-05-15 11:09:14.000000 FastHPOCR-0.1.0/FastHPOCR/IndexSNOMED.py
--rw-r--r--   0 tudor      (501) staff       (20)     3507 2024-05-06 04:11:34.000000 FastHPOCR-0.1.0/FastHPOCR/README.md
--rw-r--r--   0 tudor      (501) staff       (20)        0 2024-03-18 01:56:25.000000 FastHPOCR-0.1.0/FastHPOCR/__init__.py
-drwxr-xr-x   0 tudor      (501) staff       (20)        0 2024-05-15 13:43:38.368003 FastHPOCR-0.1.0/FastHPOCR/cr/
--rw-r--r--   0 tudor      (501) staff       (20)     3621 2024-05-15 11:06:19.000000 FastHPOCR-0.1.0/FastHPOCR/cr/CRIndexKB.py
--rw-r--r--   0 tudor      (501) staff       (20)     1051 2024-02-21 03:39:40.000000 FastHPOCR-0.1.0/FastHPOCR/cr/CandidateMatcher.py
--rw-r--r--   0 tudor      (501) staff       (20)     3642 2024-05-15 11:08:04.000000 FastHPOCR-0.1.0/FastHPOCR/cr/FormatResults.py
--rw-r--r--   0 tudor      (501) staff       (20)     1734 2024-03-02 08:55:02.000000 FastHPOCR-0.1.0/FastHPOCR/cr/SequenceCache.py
--rw-r--r--   0 tudor      (501) staff       (20)     3675 2024-05-15 11:08:04.000000 FastHPOCR-0.1.0/FastHPOCR/cr/TextProcessor.py
--rw-r--r--   0 tudor      (501) staff       (20)     3875 2024-05-15 11:06:36.000000 FastHPOCR-0.1.0/FastHPOCR/cr/TextSplitter.py
--rw-r--r--   0 tudor      (501) staff       (20)        0 2024-02-23 02:34:40.000000 FastHPOCR-0.1.0/FastHPOCR/cr/__init__.py
-drwxr-xr-x   0 tudor      (501) staff       (20)        0 2024-05-15 13:43:38.369438 FastHPOCR-0.1.0/FastHPOCR/index/
--rw-r--r--   0 tudor      (501) staff       (20)     1353 2024-05-15 13:43:03.000000 FastHPOCR-0.1.0/FastHPOCR/index/HPOLabelCollector.py
--rw-r--r--   0 tudor      (501) staff       (20)     2323 2024-05-15 11:06:42.000000 FastHPOCR-0.1.0/FastHPOCR/index/IndexTerms.py
--rw-r--r--   0 tudor      (501) staff       (20)     3564 2024-05-15 13:24:33.000000 FastHPOCR-0.1.0/FastHPOCR/index/LabelProcessor.py
--rw-r--r--   0 tudor      (501) staff       (20)     1062 2024-05-15 11:08:04.000000 FastHPOCR-0.1.0/FastHPOCR/index/ORPHALabelCollector.py
--rw-r--r--   0 tudor      (501) staff       (20)     2508 2024-05-15 13:24:25.000000 FastHPOCR-0.1.0/FastHPOCR/index/PreprocessHPOTerms.py
--rw-r--r--   0 tudor      (501) staff       (20)     2157 2024-05-15 11:08:04.000000 FastHPOCR-0.1.0/FastHPOCR/index/PreprocessORPHATerms.py
--rw-r--r--   0 tudor      (501) staff       (20)     2135 2024-05-15 11:08:04.000000 FastHPOCR-0.1.0/FastHPOCR/index/PreprocessSNOMEDTerms.py
--rw-r--r--   0 tudor      (501) staff       (20)     1703 2024-05-15 11:08:04.000000 FastHPOCR-0.1.0/FastHPOCR/index/SNOMEDLabelCollector.py
--rw-r--r--   0 tudor      (501) staff       (20)     3036 2024-05-02 09:49:49.000000 FastHPOCR-0.1.0/FastHPOCR/index/SNOMEDParser.py
--rw-r--r--   0 tudor      (501) staff       (20)     2556 2024-02-28 12:38:42.000000 FastHPOCR-0.1.0/FastHPOCR/index/SynonymExpader.py
--rw-r--r--   0 tudor      (501) staff       (20)        0 2024-02-23 02:34:32.000000 FastHPOCR-0.1.0/FastHPOCR/index/__init__.py
--rw-r--r--   0 tudor      (501) staff       (20)     1058 2024-03-18 01:51:44.000000 FastHPOCR-0.1.0/FastHPOCR/license.txt
-drwxr-xr-x   0 tudor      (501) staff       (20)        0 2024-05-15 13:43:38.369680 FastHPOCR-0.1.0/FastHPOCR/resources/
--rw-r--r--   0 tudor      (501) staff       (20)     1385 2024-05-13 14:33:20.000000 FastHPOCR-0.1.0/FastHPOCR/resources/base-synonyms
--rw-r--r--   0 tudor      (501) staff       (20)  6300038 2024-05-14 04:27:52.000000 FastHPOCR-0.1.0/FastHPOCR/resources/vocab.clusters.list
-drwxr-xr-x   0 tudor      (501) staff       (20)        0 2024-05-15 13:43:38.373534 FastHPOCR-0.1.0/FastHPOCR/util/
--rw-r--r--   0 tudor      (501) staff       (20)      828 2024-02-20 02:33:16.000000 FastHPOCR-0.1.0/FastHPOCR/util/AnnotationObject.py
--rw-r--r--   0 tudor      (501) staff       (20)     1123 2024-05-15 11:07:20.000000 FastHPOCR-0.1.0/FastHPOCR/util/AnnotationToken.py
--rw-r--r--   0 tudor      (501) staff       (20)     1511 2024-05-02 10:33:44.000000 FastHPOCR-0.1.0/FastHPOCR/util/CRConstants.py
--rw-r--r--   0 tudor      (501) staff       (20)     1196 2024-05-14 04:26:12.000000 FastHPOCR-0.1.0/FastHPOCR/util/ContentUtil.py
--rw-r--r--   0 tudor      (501) staff       (20)     4740 2024-05-15 11:07:31.000000 FastHPOCR-0.1.0/FastHPOCR/util/OntoReader.py
--rw-r--r--   0 tudor      (501) staff       (20)    42275 2024-03-02 08:55:57.000000 FastHPOCR-0.1.0/FastHPOCR/util/SequenceData.py
--rw-r--r--   0 tudor      (501) staff       (20)        0 2024-02-23 02:36:52.000000 FastHPOCR-0.1.0/FastHPOCR/util/__init__.py
-drwxr-xr-x   0 tudor      (501) staff       (20)        0 2024-05-15 13:43:38.367069 FastHPOCR-0.1.0/FastHPOCR.egg-info/
--rw-r--r--   0 tudor      (501) staff       (20)      206 2024-05-15 13:43:38.000000 FastHPOCR-0.1.0/FastHPOCR.egg-info/PKG-INFO
--rw-r--r--   0 tudor      (501) staff       (20)     1190 2024-05-15 13:43:38.000000 FastHPOCR-0.1.0/FastHPOCR.egg-info/SOURCES.txt
--rw-r--r--   0 tudor      (501) staff       (20)        1 2024-05-15 13:43:38.000000 FastHPOCR-0.1.0/FastHPOCR.egg-info/dependency_links.txt
--rw-r--r--   0 tudor      (501) staff       (20)       10 2024-05-15 13:43:38.000000 FastHPOCR-0.1.0/FastHPOCR.egg-info/top_level.txt
--rw-r--r--   0 tudor      (501) staff       (20)      206 2024-05-15 13:43:38.373690 FastHPOCR-0.1.0/PKG-INFO
--rw-r--r--   0 tudor      (501) staff       (20)       38 2024-05-15 13:43:38.373865 FastHPOCR-0.1.0/setup.cfg
--rw-r--r--   0 tudor      (501) staff       (20)      447 2024-05-15 13:43:25.000000 FastHPOCR-0.1.0/setup.py
+drwxr-xr-x   0 tudor      (501) staff       (20)        0 2024-05-20 10:59:05.212227 FastHPOCR-0.1.1/
+drwxr-xr-x   0 tudor      (501) staff       (20)        0 2024-05-20 10:59:05.204017 FastHPOCR-0.1.1/FastHPOCR/
+-rw-r--r--   0 tudor      (501) staff       (20)     1295 2024-05-15 11:08:04.000000 FastHPOCR-0.1.1/FastHPOCR/HPOAnnotator.py
+-rw-r--r--   0 tudor      (501) staff       (20)     5044 2024-05-20 10:46:20.000000 FastHPOCR-0.1.1/FastHPOCR/IndexHPO.py
+-rw-r--r--   0 tudor      (501) staff       (20)     3491 2024-05-15 11:09:02.000000 FastHPOCR-0.1.1/FastHPOCR/IndexORPHANET.py
+-rw-r--r--   0 tudor      (501) staff       (20)     4492 2024-05-15 11:09:14.000000 FastHPOCR-0.1.1/FastHPOCR/IndexSNOMED.py
+-rw-r--r--   0 tudor      (501) staff       (20)     3507 2024-05-06 04:11:34.000000 FastHPOCR-0.1.1/FastHPOCR/README.md
+-rw-r--r--   0 tudor      (501) staff       (20)        0 2024-03-18 01:56:25.000000 FastHPOCR-0.1.1/FastHPOCR/__init__.py
+drwxr-xr-x   0 tudor      (501) staff       (20)        0 2024-05-20 10:59:05.205680 FastHPOCR-0.1.1/FastHPOCR/cr/
+-rw-r--r--   0 tudor      (501) staff       (20)     3621 2024-05-15 11:06:19.000000 FastHPOCR-0.1.1/FastHPOCR/cr/CRIndexKB.py
+-rw-r--r--   0 tudor      (501) staff       (20)     1051 2024-02-21 03:39:40.000000 FastHPOCR-0.1.1/FastHPOCR/cr/CandidateMatcher.py
+-rw-r--r--   0 tudor      (501) staff       (20)     3642 2024-05-15 11:08:04.000000 FastHPOCR-0.1.1/FastHPOCR/cr/FormatResults.py
+-rw-r--r--   0 tudor      (501) staff       (20)     1734 2024-03-02 08:55:02.000000 FastHPOCR-0.1.1/FastHPOCR/cr/SequenceCache.py
+-rw-r--r--   0 tudor      (501) staff       (20)     3675 2024-05-15 11:08:04.000000 FastHPOCR-0.1.1/FastHPOCR/cr/TextProcessor.py
+-rw-r--r--   0 tudor      (501) staff       (20)     3875 2024-05-15 11:06:36.000000 FastHPOCR-0.1.1/FastHPOCR/cr/TextSplitter.py
+-rw-r--r--   0 tudor      (501) staff       (20)        0 2024-02-23 02:34:40.000000 FastHPOCR-0.1.1/FastHPOCR/cr/__init__.py
+drwxr-xr-x   0 tudor      (501) staff       (20)        0 2024-05-20 10:59:05.207309 FastHPOCR-0.1.1/FastHPOCR/index/
+-rw-r--r--   0 tudor      (501) staff       (20)     1858 2024-05-20 10:46:20.000000 FastHPOCR-0.1.1/FastHPOCR/index/HPOLabelCollector.py
+-rw-r--r--   0 tudor      (501) staff       (20)     2323 2024-05-15 11:06:42.000000 FastHPOCR-0.1.1/FastHPOCR/index/IndexTerms.py
+-rw-r--r--   0 tudor      (501) staff       (20)     3564 2024-05-15 13:22:03.000000 FastHPOCR-0.1.1/FastHPOCR/index/LabelProcessor.py
+-rw-r--r--   0 tudor      (501) staff       (20)     1062 2024-05-15 11:08:04.000000 FastHPOCR-0.1.1/FastHPOCR/index/ORPHALabelCollector.py
+-rw-r--r--   0 tudor      (501) staff       (20)     2668 2024-05-20 10:46:20.000000 FastHPOCR-0.1.1/FastHPOCR/index/PreprocessHPOTerms.py
+-rw-r--r--   0 tudor      (501) staff       (20)     2157 2024-05-15 11:08:04.000000 FastHPOCR-0.1.1/FastHPOCR/index/PreprocessORPHATerms.py
+-rw-r--r--   0 tudor      (501) staff       (20)     2135 2024-05-15 11:08:04.000000 FastHPOCR-0.1.1/FastHPOCR/index/PreprocessSNOMEDTerms.py
+-rw-r--r--   0 tudor      (501) staff       (20)     1703 2024-05-15 11:08:04.000000 FastHPOCR-0.1.1/FastHPOCR/index/SNOMEDLabelCollector.py
+-rw-r--r--   0 tudor      (501) staff       (20)     3036 2024-05-02 09:49:49.000000 FastHPOCR-0.1.1/FastHPOCR/index/SNOMEDParser.py
+-rw-r--r--   0 tudor      (501) staff       (20)     2556 2024-02-28 12:38:42.000000 FastHPOCR-0.1.1/FastHPOCR/index/SynonymExpader.py
+-rw-r--r--   0 tudor      (501) staff       (20)        0 2024-02-23 02:34:32.000000 FastHPOCR-0.1.1/FastHPOCR/index/__init__.py
+-rw-r--r--   0 tudor      (501) staff       (20)     1058 2024-03-18 01:51:44.000000 FastHPOCR-0.1.1/FastHPOCR/license.txt
+drwxr-xr-x   0 tudor      (501) staff       (20)        0 2024-05-20 10:59:05.207583 FastHPOCR-0.1.1/FastHPOCR/resources/
+-rw-r--r--   0 tudor      (501) staff       (20)     1385 2024-05-13 14:33:20.000000 FastHPOCR-0.1.1/FastHPOCR/resources/base-synonyms
+-rw-r--r--   0 tudor      (501) staff       (20)  6300038 2024-05-14 04:27:52.000000 FastHPOCR-0.1.1/FastHPOCR/resources/vocab.clusters.list
+drwxr-xr-x   0 tudor      (501) staff       (20)        0 2024-05-20 10:59:05.211912 FastHPOCR-0.1.1/FastHPOCR/util/
+-rw-r--r--   0 tudor      (501) staff       (20)      828 2024-02-20 02:33:16.000000 FastHPOCR-0.1.1/FastHPOCR/util/AnnotationObject.py
+-rw-r--r--   0 tudor      (501) staff       (20)     1123 2024-05-15 11:07:20.000000 FastHPOCR-0.1.1/FastHPOCR/util/AnnotationToken.py
+-rw-r--r--   0 tudor      (501) staff       (20)     1511 2024-05-02 10:33:44.000000 FastHPOCR-0.1.1/FastHPOCR/util/CRConstants.py
+-rw-r--r--   0 tudor      (501) staff       (20)     1196 2024-05-14 04:26:12.000000 FastHPOCR-0.1.1/FastHPOCR/util/ContentUtil.py
+-rw-r--r--   0 tudor      (501) staff       (20)     4740 2024-05-15 11:07:31.000000 FastHPOCR-0.1.1/FastHPOCR/util/OntoReader.py
+-rw-r--r--   0 tudor      (501) staff       (20)    42275 2024-03-02 08:55:57.000000 FastHPOCR-0.1.1/FastHPOCR/util/SequenceData.py
+-rw-r--r--   0 tudor      (501) staff       (20)        0 2024-02-23 02:36:52.000000 FastHPOCR-0.1.1/FastHPOCR/util/__init__.py
+drwxr-xr-x   0 tudor      (501) staff       (20)        0 2024-05-20 10:59:05.204618 FastHPOCR-0.1.1/FastHPOCR.egg-info/
+-rw-r--r--   0 tudor      (501) staff       (20)      206 2024-05-20 10:59:05.000000 FastHPOCR-0.1.1/FastHPOCR.egg-info/PKG-INFO
+-rw-r--r--   0 tudor      (501) staff       (20)     1190 2024-05-20 10:59:05.000000 FastHPOCR-0.1.1/FastHPOCR.egg-info/SOURCES.txt
+-rw-r--r--   0 tudor      (501) staff       (20)        1 2024-05-20 10:59:05.000000 FastHPOCR-0.1.1/FastHPOCR.egg-info/dependency_links.txt
+-rw-r--r--   0 tudor      (501) staff       (20)       10 2024-05-20 10:59:05.000000 FastHPOCR-0.1.1/FastHPOCR.egg-info/top_level.txt
+-rw-r--r--   0 tudor      (501) staff       (20)      206 2024-05-20 10:59:05.212085 FastHPOCR-0.1.1/PKG-INFO
+-rw-r--r--   0 tudor      (501) staff       (20)       38 2024-05-20 10:59:05.212288 FastHPOCR-0.1.1/setup.cfg
+-rw-r--r--   0 tudor      (501) staff       (20)      447 2024-05-20 10:58:13.000000 FastHPOCR-0.1.1/setup.py
```

### Comparing `FastHPOCR-0.1.0/FastHPOCR/HPOAnnotator.py` & `FastHPOCR-0.1.1/FastHPOCR/HPOAnnotator.py`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.1.0/FastHPOCR/IndexHPO.py` & `FastHPOCR-0.1.1/FastHPOCR/IndexHPO.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,39 +13,43 @@
 class IndexHPO:
     resFolder = None
     hpoLocation = None
     outputFolder = None
     externalSynFile = None
     valid = False
     allow3LetterAcronyms = False
+    rootConcepts = []
 
     clusters = {}
     synClusters = {}
     externalSynonyms = {}
     crIndexKB = None
 
-    def __init__(self, hpoLocation: str, outputFolder: str, externalSynFile=None, allow3LetterAcronyms=False):
+    def __init__(self, hpoLocation: str, outputFolder: str, rootConcepts=[], externalSynFile=None, allow3LetterAcronyms=False):
         self.resFolder = 'resources'
         self.hpoLocation = hpoLocation
         self.outputFolder = outputFolder
         self.externalSynFile = externalSynFile
+        self.rootConcepts = rootConcepts
         self.valid = False
         self.allow3LetterAcronyms = allow3LetterAcronyms
         self.crIndexKB = CRIndexKB()
         self.externalSynonyms = {}
 
     def index(self):
         start = time.time()
         self.checkPrerequisites()
         if not self.valid:
             return
 
         self.loadPrerequisites()
         print(' - Preprocessing HPO terms ...')
-        preprocessHPOTerms = PreprocessHPOTerms(self.hpoLocation, externalSynonyms=self.externalSynonyms,
+        preprocessHPOTerms = PreprocessHPOTerms(self.hpoLocation,
+                                                rootConcepts=self.rootConcepts,
+                                                externalSynonyms=self.externalSynonyms,
                                                 allow3LetterAcronyms=self.allow3LetterAcronyms)
         processedTerms = preprocessHPOTerms.getProcessedTerms()
 
         print(' - Indexing HPO terms ...')
         indexTerms = IndexTerms(processedTerms, self.clusters, self.crIndexKB)
         termsToIndex = indexTerms.getTermsToIndex()
         voidTokens = indexTerms.getVoidTokens()
@@ -112,15 +116,14 @@
             syn = segs[1].strip()
             lst = []
             if uri in self.externalSynonyms:
                 lst = self.externalSynonyms[uri]
             lst.append(syn)
             self.externalSynonyms[uri] = lst
 
-
     def checkPrerequisites(self):
         if not os.path.isfile(self.hpoLocation):
             print('ERROR: Ontology file provided [{}] does not exist!'.format(self.hpoLocation))
             self.valid = False
             return
         if not os.path.isdir(self.outputFolder):
             print('ERROR: Output folder provided [{}] does not exist!'.format(self.outputFolder))
```

### Comparing `FastHPOCR-0.1.0/FastHPOCR/IndexORPHANET.py` & `FastHPOCR-0.1.1/FastHPOCR/IndexORPHANET.py`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.1.0/FastHPOCR/IndexSNOMED.py` & `FastHPOCR-0.1.1/FastHPOCR/IndexSNOMED.py`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.1.0/FastHPOCR/README.md` & `FastHPOCR-0.1.1/FastHPOCR/README.md`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.1.0/FastHPOCR/cr/CRIndexKB.py` & `FastHPOCR-0.1.1/FastHPOCR/cr/CRIndexKB.py`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.1.0/FastHPOCR/cr/CandidateMatcher.py` & `FastHPOCR-0.1.1/FastHPOCR/cr/CandidateMatcher.py`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.1.0/FastHPOCR/cr/FormatResults.py` & `FastHPOCR-0.1.1/FastHPOCR/cr/FormatResults.py`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.1.0/FastHPOCR/cr/SequenceCache.py` & `FastHPOCR-0.1.1/FastHPOCR/cr/SequenceCache.py`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.1.0/FastHPOCR/cr/TextProcessor.py` & `FastHPOCR-0.1.1/FastHPOCR/cr/TextProcessor.py`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.1.0/FastHPOCR/cr/TextSplitter.py` & `FastHPOCR-0.1.1/FastHPOCR/cr/TextSplitter.py`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.1.0/FastHPOCR/index/HPOLabelCollector.py` & `FastHPOCR-0.1.1/FastHPOCR/index/HPOLabelCollector.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,37 @@
 from FastHPOCR.util.CRConstants import PHENOTYPIC_ABNORMALITY
 
 
 class HPOLabelCollector:
     terms = {}
     allow3LetterAcronyms = False
     externalSynonyms = {}
+    rootConcepts = []
 
-    def __init__(self, ontoReader, externalSynonyms={}, allow3LetterAcronyms=False):
+    def __init__(self, ontoReader, rootConcepts=[], externalSynonyms={}, allow3LetterAcronyms=False):
         self.terms = {}
         self.externalSynonyms = externalSynonyms
         self.allow3LetterAcronyms = allow3LetterAcronyms
+        self.rootConcepts = rootConcepts
         self.collectTerms(ontoReader)
 
     def collectTerms(self, ontoReader):
+        print('{} - {}'.format(self.externalSynonyms, self.allow3LetterAcronyms))
+
         for uri in ontoReader.terms:
             if PHENOTYPIC_ABNORMALITY in ontoReader.allSuperClasses[uri]:
+                if self.rootConcepts:
+                    found = False
+                    for ancestor in self.rootConcepts:
+                        if ancestor in ontoReader.allSuperClasses[uri]:
+                            found = True
+                            break
+                    if not found:
+                        continue
+
                 label = ontoReader.terms[uri]
                 syns = []
                 if uri in self.externalSynonyms:
                     syns.extend(self.externalSynonyms[uri])
 
                 if uri in ontoReader.synonyms:
                     for syn in ontoReader.synonyms[uri]:
```

### Comparing `FastHPOCR-0.1.0/FastHPOCR/index/IndexTerms.py` & `FastHPOCR-0.1.1/FastHPOCR/index/IndexTerms.py`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.1.0/FastHPOCR/index/LabelProcessor.py` & `FastHPOCR-0.1.1/FastHPOCR/index/LabelProcessor.py`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.1.0/FastHPOCR/index/ORPHALabelCollector.py` & `FastHPOCR-0.1.1/FastHPOCR/index/ORPHALabelCollector.py`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.1.0/FastHPOCR/index/PreprocessHPOTerms.py` & `FastHPOCR-0.1.1/FastHPOCR/index/PreprocessHPOTerms.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,19 +5,21 @@
 from FastHPOCR.util.OntoReader import OntoReader
 
 
 class PreprocessHPOTerms:
     processedTerms = {}
     terms = {}
 
-    def __init__(self, ontologyFile, externalSynonyms={}, allow3LetterAcronyms=False):
+    def __init__(self, ontologyFile, rootConcepts=[], externalSynonyms={}, allow3LetterAcronyms=False):
         ontoReader = OntoReader(ontologyFile)
         self.processedTerms = {}
 
-        labelProcessor = LabelProcessor(HPOLabelCollector(ontoReader, externalSynonyms=externalSynonyms,
+        labelProcessor = LabelProcessor(HPOLabelCollector(ontoReader,
+                                                          rootConcepts=rootConcepts,
+                                                          externalSynonyms=externalSynonyms,
                                                           allow3LetterAcronyms=allow3LetterAcronyms).getTerms(),
                                         allow3LetterAcronyms=allow3LetterAcronyms)
         self.terms = labelProcessor.getProcessedTerms()
 
         self.filterTerms()
 
     def filterTerms(self):
```

### Comparing `FastHPOCR-0.1.0/FastHPOCR/index/PreprocessORPHATerms.py` & `FastHPOCR-0.1.1/FastHPOCR/index/PreprocessORPHATerms.py`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.1.0/FastHPOCR/index/PreprocessSNOMEDTerms.py` & `FastHPOCR-0.1.1/FastHPOCR/index/PreprocessSNOMEDTerms.py`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.1.0/FastHPOCR/index/SNOMEDLabelCollector.py` & `FastHPOCR-0.1.1/FastHPOCR/index/SNOMEDLabelCollector.py`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.1.0/FastHPOCR/index/SNOMEDParser.py` & `FastHPOCR-0.1.1/FastHPOCR/index/SNOMEDParser.py`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.1.0/FastHPOCR/index/SynonymExpader.py` & `FastHPOCR-0.1.1/FastHPOCR/index/SynonymExpader.py`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.1.0/FastHPOCR/license.txt` & `FastHPOCR-0.1.1/FastHPOCR/license.txt`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.1.0/FastHPOCR/resources/base-synonyms` & `FastHPOCR-0.1.1/FastHPOCR/resources/base-synonyms`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.1.0/FastHPOCR/resources/vocab.clusters.list` & `FastHPOCR-0.1.1/FastHPOCR/resources/vocab.clusters.list`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.1.0/FastHPOCR/util/AnnotationObject.py` & `FastHPOCR-0.1.1/FastHPOCR/util/AnnotationObject.py`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.1.0/FastHPOCR/util/AnnotationToken.py` & `FastHPOCR-0.1.1/FastHPOCR/util/AnnotationToken.py`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.1.0/FastHPOCR/util/CRConstants.py` & `FastHPOCR-0.1.1/FastHPOCR/util/CRConstants.py`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.1.0/FastHPOCR/util/ContentUtil.py` & `FastHPOCR-0.1.1/FastHPOCR/util/ContentUtil.py`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.1.0/FastHPOCR/util/OntoReader.py` & `FastHPOCR-0.1.1/FastHPOCR/util/OntoReader.py`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.1.0/FastHPOCR/util/SequenceData.py` & `FastHPOCR-0.1.1/FastHPOCR/util/SequenceData.py`

 * *Files identical despite different names*

### Comparing `FastHPOCR-0.1.0/FastHPOCR.egg-info/SOURCES.txt` & `FastHPOCR-0.1.1/FastHPOCR.egg-info/SOURCES.txt`

 * *Files identical despite different names*

