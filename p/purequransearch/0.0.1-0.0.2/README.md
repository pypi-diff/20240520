# Comparing `tmp/purequransearch-0.0.1.tar.gz` & `tmp/purequransearch-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "purequransearch-0.0.1.tar", last modified: Sun May 19 19:55:25 2024, max compression
+gzip compressed data, was "purequransearch-0.0.2.tar", last modified: Sun May 19 21:16:07 2024, max compression
```

## Comparing `purequransearch-0.0.1.tar` & `purequransearch-0.0.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:55:25.164217 purequransearch-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-19 19:55:25.164217 purequransearch-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-19 19:55:20.000000 purequransearch-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-19 19:55:20.000000 purequransearch-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 19:55:25.164217 purequransearch-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:55:25.136217 purequransearch-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:55:25.136217 purequransearch-0.0.1/src/purequransearch/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-19 19:55:20.000000 purequransearch-0.0.1/src/purequransearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7047 2024-05-19 19:55:20.000000 purequransearch-0.0.1/src/purequransearch/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-05-19 19:55:20.000000 purequransearch-0.0.1/src/purequransearch/concordance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:55:25.160217 purequransearch-0.0.1/src/purequransearch/corpora/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 19:55:20.000000 purequransearch-0.0.1/src/purequransearch/corpora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   979878 2024-05-19 19:55:20.000000 purequransearch-0.0.1/src/purequransearch/corpora/en.ahmedali.xml
--rw-r--r--   0 runner    (1001) docker     (127)  1094455 2024-05-19 19:55:20.000000 purequransearch-0.0.1/src/purequransearch/corpora/en.ahmedraza.xml
--rw-r--r--   0 runner    (1001) docker     (127)   957588 2024-05-19 19:55:20.000000 purequransearch-0.0.1/src/purequransearch/corpora/en.arberry.xml
--rw-r--r--   0 runner    (1001) docker     (127)  1017859 2024-05-19 19:55:20.000000 purequransearch-0.0.1/src/purequransearch/corpora/en.daryabadi.xml
--rw-r--r--   0 runner    (1001) docker     (127)  1300831 2024-05-19 19:55:20.000000 purequransearch-0.0.1/src/purequransearch/corpora/en.hilali.xml
--rw-r--r--   0 runner    (1001) docker     (127)   933981 2024-05-19 19:55:20.000000 purequransearch-0.0.1/src/purequransearch/corpora/en.itani.xml
--rw-r--r--   0 runner    (1001) docker     (127)  1105236 2024-05-19 19:55:20.000000 purequransearch-0.0.1/src/purequransearch/corpora/en.maududi.xml
--rw-r--r--   0 runner    (1001) docker     (127)  1065247 2024-05-19 19:55:20.000000 purequransearch-0.0.1/src/purequransearch/corpora/en.mubarakpuri.xml
--rw-r--r--   0 runner    (1001) docker     (127)  1001665 2024-05-19 19:55:20.000000 purequransearch-0.0.1/src/purequransearch/corpora/en.pickthall.xml
--rw-r--r--   0 runner    (1001) docker     (127)  1003239 2024-05-19 19:55:20.000000 purequransearch-0.0.1/src/purequransearch/corpora/en.qarai.xml
--rw-r--r--   0 runner    (1001) docker     (127)   951906 2024-05-19 19:55:20.000000 purequransearch-0.0.1/src/purequransearch/corpora/en.qaribullah.xml
--rw-r--r--   0 runner    (1001) docker     (127)  1051586 2024-05-19 19:55:21.000000 purequransearch-0.0.1/src/purequransearch/corpora/en.sahih.xml
--rw-r--r--   0 runner    (1001) docker     (127)  1027340 2024-05-19 19:55:21.000000 purequransearch-0.0.1/src/purequransearch/corpora/en.sarwar.xml
--rw-r--r--   0 runner    (1001) docker     (127)  1019299 2024-05-19 19:55:21.000000 purequransearch-0.0.1/src/purequransearch/corpora/en.shakir.xml
--rw-r--r--   0 runner    (1001) docker     (127)  1846773 2024-05-19 19:55:21.000000 purequransearch-0.0.1/src/purequransearch/corpora/en.transliteration.xml
--rw-r--r--   0 runner    (1001) docker     (127)  1014282 2024-05-19 19:55:21.000000 purequransearch-0.0.1/src/purequransearch/corpora/en.wahiduddin.xml
--rw-r--r--   0 runner    (1001) docker     (127)  1095168 2024-05-19 19:55:21.000000 purequransearch-0.0.1/src/purequransearch/corpora/en.yusufali.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:55:25.164217 purequransearch-0.0.1/src/purequransearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-19 19:55:25.000000 purequransearch-0.0.1/src/purequransearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-19 19:55:25.000000 purequransearch-0.0.1/src/purequransearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:55:25.000000 purequransearch-0.0.1/src/purequransearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-19 19:55:25.000000 purequransearch-0.0.1/src/purequransearch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-19 19:55:25.000000 purequransearch-0.0.1/src/purequransearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-19 19:55:25.000000 purequransearch-0.0.1/src/purequransearch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:16:07.422396 purequransearch-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-19 21:16:07.422396 purequransearch-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-19 21:16:03.000000 purequransearch-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-19 21:16:03.000000 purequransearch-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 21:16:07.422396 purequransearch-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:16:07.394396 purequransearch-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:16:07.394396 purequransearch-0.0.2/src/purequransearch/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-19 21:16:03.000000 purequransearch-0.0.2/src/purequransearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7020 2024-05-19 21:16:03.000000 purequransearch-0.0.2/src/purequransearch/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-05-19 21:16:03.000000 purequransearch-0.0.2/src/purequransearch/concordance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:16:07.422396 purequransearch-0.0.2/src/purequransearch/corpora/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 21:16:03.000000 purequransearch-0.0.2/src/purequransearch/corpora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   979878 2024-05-19 21:16:03.000000 purequransearch-0.0.2/src/purequransearch/corpora/en.ahmedali.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  1094455 2024-05-19 21:16:03.000000 purequransearch-0.0.2/src/purequransearch/corpora/en.ahmedraza.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   957588 2024-05-19 21:16:03.000000 purequransearch-0.0.2/src/purequransearch/corpora/en.arberry.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  1017859 2024-05-19 21:16:03.000000 purequransearch-0.0.2/src/purequransearch/corpora/en.daryabadi.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  1300831 2024-05-19 21:16:03.000000 purequransearch-0.0.2/src/purequransearch/corpora/en.hilali.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   933981 2024-05-19 21:16:03.000000 purequransearch-0.0.2/src/purequransearch/corpora/en.itani.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  1105236 2024-05-19 21:16:03.000000 purequransearch-0.0.2/src/purequransearch/corpora/en.maududi.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  1065247 2024-05-19 21:16:03.000000 purequransearch-0.0.2/src/purequransearch/corpora/en.mubarakpuri.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  1001665 2024-05-19 21:16:03.000000 purequransearch-0.0.2/src/purequransearch/corpora/en.pickthall.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  1003239 2024-05-19 21:16:03.000000 purequransearch-0.0.2/src/purequransearch/corpora/en.qarai.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   951906 2024-05-19 21:16:03.000000 purequransearch-0.0.2/src/purequransearch/corpora/en.qaribullah.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  1051586 2024-05-19 21:16:03.000000 purequransearch-0.0.2/src/purequransearch/corpora/en.sahih.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  1027340 2024-05-19 21:16:03.000000 purequransearch-0.0.2/src/purequransearch/corpora/en.sarwar.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  1019299 2024-05-19 21:16:03.000000 purequransearch-0.0.2/src/purequransearch/corpora/en.shakir.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  1846773 2024-05-19 21:16:03.000000 purequransearch-0.0.2/src/purequransearch/corpora/en.transliteration.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  1014282 2024-05-19 21:16:03.000000 purequransearch-0.0.2/src/purequransearch/corpora/en.wahiduddin.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  1095168 2024-05-19 21:16:03.000000 purequransearch-0.0.2/src/purequransearch/corpora/en.yusufali.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:16:07.422396 purequransearch-0.0.2/src/purequransearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-19 21:16:07.000000 purequransearch-0.0.2/src/purequransearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-19 21:16:07.000000 purequransearch-0.0.2/src/purequransearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 21:16:07.000000 purequransearch-0.0.2/src/purequransearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-19 21:16:07.000000 purequransearch-0.0.2/src/purequransearch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-19 21:16:07.000000 purequransearch-0.0.2/src/purequransearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-19 21:16:07.000000 purequransearch-0.0.2/src/purequransearch.egg-info/top_level.txt
```

### Comparing `purequransearch-0.0.1/PKG-INFO` & `purequransearch-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: purequransearch
-Version: 0.0.1
+Version: 0.0.2
 Summary: Search the Quran (in English) for words and phrases.
 Author-email: Josiah Winslow <winslowjosiah@gmail.com>
 Project-URL: Homepage, https://github.com/winslowjosiah/pure-quran-search
 Project-URL: Issues, https://github.com/winslowjosiah/pure-quran-search/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -51,10 +51,14 @@
 
 Found 2 occurrence(s) in 2 verse(s).
 
 ```
 
 ## Changelog
 
+### v0.0.2 (2024-05-19)
+
+- Fixed CLI error that can happen with overlapping matches.
+
 ### v0.0.1 (2024-05-19)
 
 Initial release.
```

### Comparing `purequransearch-0.0.1/README.md` & `purequransearch-0.0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -37,10 +37,14 @@
 
 Found 2 occurrence(s) in 2 verse(s).
 
 ```
 
 ## Changelog
 
+### v0.0.2 (2024-05-19)
+
+- Fixed CLI error that can happen with overlapping matches.
+
 ### v0.0.1 (2024-05-19)
 
 Initial release.
```

### Comparing `purequransearch-0.0.1/pyproject.toml` & `purequransearch-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "purequransearch"
-version = "0.0.1"
+version = "0.0.2"
 dependencies = [
     "lxml >= 5.0.0",
 ]
 requires-python = ">=3.9"
 authors = [
     { name="Josiah Winslow", email="winslowjosiah@gmail.com" },
 ]
```

### Comparing `purequransearch-0.0.1/src/purequransearch/cli.py` & `purequransearch-0.0.2/src/purequransearch/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,24 +134,25 @@
         word_length = len(concordance.text_to_words(term))
         # For each search result
         for index in term_results:
             verse_index = concordance.word_index_to_verse(index)
             # Create mapping between verse index and search result
             verse_map[verse_index].append((index, word_length))
 
+        verse_map[verse_index].sort()
+
     occurrence_total = 0
     verse_total = 0
     # For each verse which is part of the results
     for (chapter, verse), verse_results in sorted(verse_map.items()):
         verse_total += 1
 
         # Get info for this verse
         verse_start = concordance.starts[chapter][verse]
         text = concordance.content[chapter][verse]
-        words = Concordance.text_to_words(text, alnum_only=False)
 
         # HACK What I want to do is surround each occurrence of a search
         # term with braces (like "In the name {{ of Allah }}"). The most
         # robust way I can think of to do this is to split the text into
         # words, make the replacement, then join the text together.
         text = text.split()
         # NOTE Making the text replacements in reverse ensures that they
```

### Comparing `purequransearch-0.0.1/src/purequransearch/concordance.py` & `purequransearch-0.0.2/src/purequransearch/concordance.py`

 * *Files identical despite different names*

### Comparing `purequransearch-0.0.1/src/purequransearch/corpora/en.ahmedali.xml` & `purequransearch-0.0.2/src/purequransearch/corpora/en.ahmedali.xml`

 * *Files identical despite different names*

### Comparing `purequransearch-0.0.1/src/purequransearch/corpora/en.ahmedraza.xml` & `purequransearch-0.0.2/src/purequransearch/corpora/en.ahmedraza.xml`

 * *Files identical despite different names*

### Comparing `purequransearch-0.0.1/src/purequransearch/corpora/en.arberry.xml` & `purequransearch-0.0.2/src/purequransearch/corpora/en.arberry.xml`

 * *Files identical despite different names*

### Comparing `purequransearch-0.0.1/src/purequransearch/corpora/en.daryabadi.xml` & `purequransearch-0.0.2/src/purequransearch/corpora/en.daryabadi.xml`

 * *Files identical despite different names*

### Comparing `purequransearch-0.0.1/src/purequransearch/corpora/en.hilali.xml` & `purequransearch-0.0.2/src/purequransearch/corpora/en.hilali.xml`

 * *Files identical despite different names*

### Comparing `purequransearch-0.0.1/src/purequransearch/corpora/en.itani.xml` & `purequransearch-0.0.2/src/purequransearch/corpora/en.itani.xml`

 * *Files identical despite different names*

### Comparing `purequransearch-0.0.1/src/purequransearch/corpora/en.maududi.xml` & `purequransearch-0.0.2/src/purequransearch/corpora/en.maududi.xml`

 * *Files identical despite different names*

### Comparing `purequransearch-0.0.1/src/purequransearch/corpora/en.mubarakpuri.xml` & `purequransearch-0.0.2/src/purequransearch/corpora/en.mubarakpuri.xml`

 * *Files identical despite different names*

### Comparing `purequransearch-0.0.1/src/purequransearch/corpora/en.pickthall.xml` & `purequransearch-0.0.2/src/purequransearch/corpora/en.pickthall.xml`

 * *Files identical despite different names*

### Comparing `purequransearch-0.0.1/src/purequransearch/corpora/en.qarai.xml` & `purequransearch-0.0.2/src/purequransearch/corpora/en.qarai.xml`

 * *Files identical despite different names*

### Comparing `purequransearch-0.0.1/src/purequransearch/corpora/en.qaribullah.xml` & `purequransearch-0.0.2/src/purequransearch/corpora/en.qaribullah.xml`

 * *Files identical despite different names*

### Comparing `purequransearch-0.0.1/src/purequransearch/corpora/en.sahih.xml` & `purequransearch-0.0.2/src/purequransearch/corpora/en.sahih.xml`

 * *Files identical despite different names*

### Comparing `purequransearch-0.0.1/src/purequransearch/corpora/en.sarwar.xml` & `purequransearch-0.0.2/src/purequransearch/corpora/en.sarwar.xml`

 * *Files identical despite different names*

### Comparing `purequransearch-0.0.1/src/purequransearch/corpora/en.shakir.xml` & `purequransearch-0.0.2/src/purequransearch/corpora/en.shakir.xml`

 * *Files identical despite different names*

### Comparing `purequransearch-0.0.1/src/purequransearch/corpora/en.transliteration.xml` & `purequransearch-0.0.2/src/purequransearch/corpora/en.transliteration.xml`

 * *Files identical despite different names*

### Comparing `purequransearch-0.0.1/src/purequransearch/corpora/en.wahiduddin.xml` & `purequransearch-0.0.2/src/purequransearch/corpora/en.wahiduddin.xml`

 * *Files identical despite different names*

### Comparing `purequransearch-0.0.1/src/purequransearch/corpora/en.yusufali.xml` & `purequransearch-0.0.2/src/purequransearch/corpora/en.yusufali.xml`

 * *Files identical despite different names*

### Comparing `purequransearch-0.0.1/src/purequransearch.egg-info/PKG-INFO` & `purequransearch-0.0.2/src/purequransearch.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: purequransearch
-Version: 0.0.1
+Version: 0.0.2
 Summary: Search the Quran (in English) for words and phrases.
 Author-email: Josiah Winslow <winslowjosiah@gmail.com>
 Project-URL: Homepage, https://github.com/winslowjosiah/pure-quran-search
 Project-URL: Issues, https://github.com/winslowjosiah/pure-quran-search/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -51,10 +51,14 @@
 
 Found 2 occurrence(s) in 2 verse(s).
 
 ```
 
 ## Changelog
 
+### v0.0.2 (2024-05-19)
+
+- Fixed CLI error that can happen with overlapping matches.
+
 ### v0.0.1 (2024-05-19)
 
 Initial release.
```

### Comparing `purequransearch-0.0.1/src/purequransearch.egg-info/SOURCES.txt` & `purequransearch-0.0.2/src/purequransearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

