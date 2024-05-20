# Comparing `tmp/purequransearch-0.0.2.tar.gz` & `tmp/purequransearch-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "purequransearch-0.0.2.tar", last modified: Sun May 19 21:16:07 2024, max compression
+gzip compressed data, was "purequransearch-0.0.3.tar", last modified: Mon May 20 00:35:46 2024, max compression
```

## Comparing `purequransearch-0.0.2.tar` & `purequransearch-0.0.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:16:07.422396 purequransearch-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-19 21:16:07.422396 purequransearch-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-19 21:16:03.000000 purequransearch-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-19 21:16:03.000000 purequransearch-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 21:16:07.422396 purequransearch-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:16:07.394396 purequransearch-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:16:07.394396 purequransearch-0.0.2/src/purequransearch/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-19 21:16:03.000000 purequransearch-0.0.2/src/purequransearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7020 2024-05-19 21:16:03.000000 purequransearch-0.0.2/src/purequransearch/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-05-19 21:16:03.000000 purequransearch-0.0.2/src/purequransearch/concordance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:16:07.422396 purequransearch-0.0.2/src/purequransearch/corpora/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 21:16:03.000000 purequransearch-0.0.2/src/purequransearch/corpora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   979878 2024-05-19 21:16:03.000000 purequransearch-0.0.2/src/purequransearch/corpora/en.ahmedali.xml
--rw-r--r--   0 runner    (1001) docker     (127)  1094455 2024-05-19 21:16:03.000000 purequransearch-0.0.2/src/purequransearch/corpora/en.ahmedraza.xml
--rw-r--r--   0 runner    (1001) docker     (127)   957588 2024-05-19 21:16:03.000000 purequransearch-0.0.2/src/purequransearch/corpora/en.arberry.xml
--rw-r--r--   0 runner    (1001) docker     (127)  1017859 2024-05-19 21:16:03.000000 purequransearch-0.0.2/src/purequransearch/corpora/en.daryabadi.xml
--rw-r--r--   0 runner    (1001) docker     (127)  1300831 2024-05-19 21:16:03.000000 purequransearch-0.0.2/src/purequransearch/corpora/en.hilali.xml
--rw-r--r--   0 runner    (1001) docker     (127)   933981 2024-05-19 21:16:03.000000 purequransearch-0.0.2/src/purequransearch/corpora/en.itani.xml
--rw-r--r--   0 runner    (1001) docker     (127)  1105236 2024-05-19 21:16:03.000000 purequransearch-0.0.2/src/purequransearch/corpora/en.maududi.xml
--rw-r--r--   0 runner    (1001) docker     (127)  1065247 2024-05-19 21:16:03.000000 purequransearch-0.0.2/src/purequransearch/corpora/en.mubarakpuri.xml
--rw-r--r--   0 runner    (1001) docker     (127)  1001665 2024-05-19 21:16:03.000000 purequransearch-0.0.2/src/purequransearch/corpora/en.pickthall.xml
--rw-r--r--   0 runner    (1001) docker     (127)  1003239 2024-05-19 21:16:03.000000 purequransearch-0.0.2/src/purequransearch/corpora/en.qarai.xml
--rw-r--r--   0 runner    (1001) docker     (127)   951906 2024-05-19 21:16:03.000000 purequransearch-0.0.2/src/purequransearch/corpora/en.qaribullah.xml
--rw-r--r--   0 runner    (1001) docker     (127)  1051586 2024-05-19 21:16:03.000000 purequransearch-0.0.2/src/purequransearch/corpora/en.sahih.xml
--rw-r--r--   0 runner    (1001) docker     (127)  1027340 2024-05-19 21:16:03.000000 purequransearch-0.0.2/src/purequransearch/corpora/en.sarwar.xml
--rw-r--r--   0 runner    (1001) docker     (127)  1019299 2024-05-19 21:16:03.000000 purequransearch-0.0.2/src/purequransearch/corpora/en.shakir.xml
--rw-r--r--   0 runner    (1001) docker     (127)  1846773 2024-05-19 21:16:03.000000 purequransearch-0.0.2/src/purequransearch/corpora/en.transliteration.xml
--rw-r--r--   0 runner    (1001) docker     (127)  1014282 2024-05-19 21:16:03.000000 purequransearch-0.0.2/src/purequransearch/corpora/en.wahiduddin.xml
--rw-r--r--   0 runner    (1001) docker     (127)  1095168 2024-05-19 21:16:03.000000 purequransearch-0.0.2/src/purequransearch/corpora/en.yusufali.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:16:07.422396 purequransearch-0.0.2/src/purequransearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-19 21:16:07.000000 purequransearch-0.0.2/src/purequransearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-19 21:16:07.000000 purequransearch-0.0.2/src/purequransearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 21:16:07.000000 purequransearch-0.0.2/src/purequransearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-19 21:16:07.000000 purequransearch-0.0.2/src/purequransearch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-19 21:16:07.000000 purequransearch-0.0.2/src/purequransearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-19 21:16:07.000000 purequransearch-0.0.2/src/purequransearch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:35:46.444779 purequransearch-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-20 00:35:46.444779 purequransearch-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-20 00:35:28.000000 purequransearch-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-20 00:35:28.000000 purequransearch-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 00:35:46.444779 purequransearch-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:35:46.416780 purequransearch-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:35:46.416780 purequransearch-0.0.3/src/purequransearch/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-20 00:35:28.000000 purequransearch-0.0.3/src/purequransearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7316 2024-05-20 00:35:28.000000 purequransearch-0.0.3/src/purequransearch/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10604 2024-05-20 00:35:28.000000 purequransearch-0.0.3/src/purequransearch/concordance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:35:46.444779 purequransearch-0.0.3/src/purequransearch/corpora/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 00:35:28.000000 purequransearch-0.0.3/src/purequransearch/corpora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   979878 2024-05-20 00:35:28.000000 purequransearch-0.0.3/src/purequransearch/corpora/en.ahmedali.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  1094455 2024-05-20 00:35:28.000000 purequransearch-0.0.3/src/purequransearch/corpora/en.ahmedraza.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   957588 2024-05-20 00:35:28.000000 purequransearch-0.0.3/src/purequransearch/corpora/en.arberry.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  1017859 2024-05-20 00:35:28.000000 purequransearch-0.0.3/src/purequransearch/corpora/en.daryabadi.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  1300831 2024-05-20 00:35:28.000000 purequransearch-0.0.3/src/purequransearch/corpora/en.hilali.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   933981 2024-05-20 00:35:28.000000 purequransearch-0.0.3/src/purequransearch/corpora/en.itani.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  1105236 2024-05-20 00:35:28.000000 purequransearch-0.0.3/src/purequransearch/corpora/en.maududi.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  1065247 2024-05-20 00:35:28.000000 purequransearch-0.0.3/src/purequransearch/corpora/en.mubarakpuri.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  1001665 2024-05-20 00:35:28.000000 purequransearch-0.0.3/src/purequransearch/corpora/en.pickthall.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  1003239 2024-05-20 00:35:28.000000 purequransearch-0.0.3/src/purequransearch/corpora/en.qarai.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   951906 2024-05-20 00:35:28.000000 purequransearch-0.0.3/src/purequransearch/corpora/en.qaribullah.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  1051586 2024-05-20 00:35:28.000000 purequransearch-0.0.3/src/purequransearch/corpora/en.sahih.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  1027340 2024-05-20 00:35:28.000000 purequransearch-0.0.3/src/purequransearch/corpora/en.sarwar.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  1019299 2024-05-20 00:35:28.000000 purequransearch-0.0.3/src/purequransearch/corpora/en.shakir.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  1846773 2024-05-20 00:35:28.000000 purequransearch-0.0.3/src/purequransearch/corpora/en.transliteration.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  1014282 2024-05-20 00:35:28.000000 purequransearch-0.0.3/src/purequransearch/corpora/en.wahiduddin.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  1095168 2024-05-20 00:35:28.000000 purequransearch-0.0.3/src/purequransearch/corpora/en.yusufali.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:35:46.444779 purequransearch-0.0.3/src/purequransearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-20 00:35:46.000000 purequransearch-0.0.3/src/purequransearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-20 00:35:46.000000 purequransearch-0.0.3/src/purequransearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 00:35:46.000000 purequransearch-0.0.3/src/purequransearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-20 00:35:46.000000 purequransearch-0.0.3/src/purequransearch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-20 00:35:46.000000 purequransearch-0.0.3/src/purequransearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-20 00:35:46.000000 purequransearch-0.0.3/src/purequransearch.egg-info/top_level.txt
```

### Comparing `purequransearch-0.0.2/PKG-INFO` & `purequransearch-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: purequransearch
-Version: 0.0.2
+Version: 0.0.3
 Summary: Search the Quran (in English) for words and phrases.
 Author-email: Josiah Winslow <winslowjosiah@gmail.com>
 Project-URL: Homepage, https://github.com/winslowjosiah/pure-quran-search
 Project-URL: Issues, https://github.com/winslowjosiah/pure-quran-search/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -51,14 +51,19 @@
 
 Found 2 occurrence(s) in 2 verse(s).
 
 ```
 
 ## Changelog
 
+### v0.0.3 (2024-05-19)
+
+- Fixed CLI error when searching past end of Quran.
+- Improved display of braces on CLI.
+
 ### v0.0.2 (2024-05-19)
 
 - Fixed CLI error that can happen with overlapping matches.
 
 ### v0.0.1 (2024-05-19)
 
 Initial release.
```

### Comparing `purequransearch-0.0.2/README.md` & `purequransearch-0.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -37,14 +37,19 @@
 
 Found 2 occurrence(s) in 2 verse(s).
 
 ```
 
 ## Changelog
 
+### v0.0.3 (2024-05-19)
+
+- Fixed CLI error when searching past end of Quran.
+- Improved display of braces on CLI.
+
 ### v0.0.2 (2024-05-19)
 
 - Fixed CLI error that can happen with overlapping matches.
 
 ### v0.0.1 (2024-05-19)
 
 Initial release.
```

### Comparing `purequransearch-0.0.2/pyproject.toml` & `purequransearch-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "purequransearch"
-version = "0.0.2"
+version = "0.0.3"
 dependencies = [
     "lxml >= 5.0.0",
 ]
 requires-python = ">=3.9"
 authors = [
     { name="Josiah Winslow", email="winslowjosiah@gmail.com" },
 ]
```

### Comparing `purequransearch-0.0.2/src/purequransearch/cli.py` & `purequransearch-0.0.3/src/purequransearch/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -149,19 +149,19 @@
         # Get info for this verse
         verse_start = concordance.starts[chapter][verse]
         text = concordance.content[chapter][verse]
 
         # HACK What I want to do is surround each occurrence of a search
         # term with braces (like "In the name {{ of Allah }}"). The most
         # robust way I can think of to do this is to split the text into
-        # words, make the replacement, then join the text together.
+        # words, position the braces, then join the text together.
         text = text.split()
-        # NOTE Making the text replacements in reverse ensures that they
-        # don't affect the positions of the other terms in the text.
-        for index, length in reversed(verse_results):
+        left_braces = ["" for _ in text]
+        right_braces = ["" for _ in text]
+        for verse_result_i, (index, length) in enumerate(verse_results, 1):
             occurrence_total += 1
 
             # Find the starting index of the term
             term_start = 0
             i = index - verse_start
             while i > 0:
                 if Concordance.normalize_word(text[term_start]):
@@ -181,26 +181,33 @@
                 if Concordance.normalize_word(text[term_end]):
                     i -= 1
                 term_end += 1
 
             if overflow:
                 # If there is overflow, surround in braces and display
                 # ellipsis at end
-                text[term_start:] = [
-                    "{{" + " ".join(text[term_start:]) + " ...}}"
-                ]
+                left_braces[term_start] += "{" * verse_result_i + " "
+                right_braces[term_end - 1] = (
+                    " ..." + "}" * verse_result_i + right_braces[term_end - 1]
+                )
                 # TODO Display part of next verse if there is overflow
             else:
                 # If there is no overflow, surround in braces
-                text[term_start:term_end] = [
-                    "{{" + " ".join(text[term_start:term_end]) + "}}"
-                ]
+                left_braces[term_start] += "{" * verse_result_i + " "
+                right_braces[term_end - 1] = (
+                    " " + "}" * verse_result_i + right_braces[term_end - 1]
+                )
 
         # Rejoin and display the text
-        text = " ".join(text)
+        text = " ".join(
+            left_brace + word + right_brace
+            for word, left_brace, right_brace in zip(
+                text, left_braces, right_braces
+            )
+        )
         print(f"{chapter + 1}:{verse + 1}\t{text}")
         print(f"Occurrences: {occurrence_total}; Verses: {verse_total}")
         print()
 
     # Report total occurrence and verse count
     print(
         f"Found {occurrence_total} occurrence(s) in {verse_total} "
```

### Comparing `purequransearch-0.0.2/src/purequransearch/concordance.py` & `purequransearch-0.0.3/src/purequransearch/concordance.py`

 * *Files 1% similar despite different names*

```diff
@@ -319,14 +319,19 @@
                     preserve_case=case_sensitive,
                 ):
                     continue
 
             found_result = True
             # Check that all other words match
             for offset, other_word in enumerate(other_words, 1):
+                # If word is past end of Quran
+                if word_index + offset >= len(self.words):
+                    found_result = False
+                    break
+
                 next_word = self.normalize_word(
                     self.words[word_index + offset],
                     preserve_case=case_sensitive,
                 )
 
                 if other_word != next_word:
                     found_result = False
```

### Comparing `purequransearch-0.0.2/src/purequransearch/corpora/en.ahmedali.xml` & `purequransearch-0.0.3/src/purequransearch/corpora/en.ahmedali.xml`

 * *Files identical despite different names*

### Comparing `purequransearch-0.0.2/src/purequransearch/corpora/en.ahmedraza.xml` & `purequransearch-0.0.3/src/purequransearch/corpora/en.ahmedraza.xml`

 * *Files identical despite different names*

### Comparing `purequransearch-0.0.2/src/purequransearch/corpora/en.arberry.xml` & `purequransearch-0.0.3/src/purequransearch/corpora/en.arberry.xml`

 * *Files identical despite different names*

### Comparing `purequransearch-0.0.2/src/purequransearch/corpora/en.daryabadi.xml` & `purequransearch-0.0.3/src/purequransearch/corpora/en.daryabadi.xml`

 * *Files identical despite different names*

### Comparing `purequransearch-0.0.2/src/purequransearch/corpora/en.hilali.xml` & `purequransearch-0.0.3/src/purequransearch/corpora/en.hilali.xml`

 * *Files identical despite different names*

### Comparing `purequransearch-0.0.2/src/purequransearch/corpora/en.itani.xml` & `purequransearch-0.0.3/src/purequransearch/corpora/en.itani.xml`

 * *Files identical despite different names*

### Comparing `purequransearch-0.0.2/src/purequransearch/corpora/en.maududi.xml` & `purequransearch-0.0.3/src/purequransearch/corpora/en.maududi.xml`

 * *Files identical despite different names*

### Comparing `purequransearch-0.0.2/src/purequransearch/corpora/en.mubarakpuri.xml` & `purequransearch-0.0.3/src/purequransearch/corpora/en.mubarakpuri.xml`

 * *Files identical despite different names*

### Comparing `purequransearch-0.0.2/src/purequransearch/corpora/en.pickthall.xml` & `purequransearch-0.0.3/src/purequransearch/corpora/en.pickthall.xml`

 * *Files identical despite different names*

### Comparing `purequransearch-0.0.2/src/purequransearch/corpora/en.qarai.xml` & `purequransearch-0.0.3/src/purequransearch/corpora/en.qarai.xml`

 * *Files identical despite different names*

### Comparing `purequransearch-0.0.2/src/purequransearch/corpora/en.qaribullah.xml` & `purequransearch-0.0.3/src/purequransearch/corpora/en.qaribullah.xml`

 * *Files identical despite different names*

### Comparing `purequransearch-0.0.2/src/purequransearch/corpora/en.sahih.xml` & `purequransearch-0.0.3/src/purequransearch/corpora/en.sahih.xml`

 * *Files identical despite different names*

### Comparing `purequransearch-0.0.2/src/purequransearch/corpora/en.sarwar.xml` & `purequransearch-0.0.3/src/purequransearch/corpora/en.sarwar.xml`

 * *Files identical despite different names*

### Comparing `purequransearch-0.0.2/src/purequransearch/corpora/en.shakir.xml` & `purequransearch-0.0.3/src/purequransearch/corpora/en.shakir.xml`

 * *Files identical despite different names*

### Comparing `purequransearch-0.0.2/src/purequransearch/corpora/en.transliteration.xml` & `purequransearch-0.0.3/src/purequransearch/corpora/en.transliteration.xml`

 * *Files identical despite different names*

### Comparing `purequransearch-0.0.2/src/purequransearch/corpora/en.wahiduddin.xml` & `purequransearch-0.0.3/src/purequransearch/corpora/en.wahiduddin.xml`

 * *Files identical despite different names*

### Comparing `purequransearch-0.0.2/src/purequransearch/corpora/en.yusufali.xml` & `purequransearch-0.0.3/src/purequransearch/corpora/en.yusufali.xml`

 * *Files identical despite different names*

### Comparing `purequransearch-0.0.2/src/purequransearch.egg-info/PKG-INFO` & `purequransearch-0.0.3/src/purequransearch.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: purequransearch
-Version: 0.0.2
+Version: 0.0.3
 Summary: Search the Quran (in English) for words and phrases.
 Author-email: Josiah Winslow <winslowjosiah@gmail.com>
 Project-URL: Homepage, https://github.com/winslowjosiah/pure-quran-search
 Project-URL: Issues, https://github.com/winslowjosiah/pure-quran-search/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -51,14 +51,19 @@
 
 Found 2 occurrence(s) in 2 verse(s).
 
 ```
 
 ## Changelog
 
+### v0.0.3 (2024-05-19)
+
+- Fixed CLI error when searching past end of Quran.
+- Improved display of braces on CLI.
+
 ### v0.0.2 (2024-05-19)
 
 - Fixed CLI error that can happen with overlapping matches.
 
 ### v0.0.1 (2024-05-19)
 
 Initial release.
```

### Comparing `purequransearch-0.0.2/src/purequransearch.egg-info/SOURCES.txt` & `purequransearch-0.0.3/src/purequransearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

