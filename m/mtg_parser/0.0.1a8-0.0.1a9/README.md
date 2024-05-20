# Comparing `tmp/mtg_parser-0.0.1a8.tar.gz` & `tmp/mtg_parser-0.0.1a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mtg_parser-0.0.1a8.tar", last modified: Thu Apr 15 20:18:39 2021, max compression
+gzip compressed data, was "mtg_parser-0.0.1a9.tar", last modified: Fri Apr 16 21:02:32 2021, max compression
```

## Comparing `mtg_parser-0.0.1a8.tar` & `mtg_parser-0.0.1a9.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1074 2021-03-28 21:26:17.680739 mtg_parser-0.0.1a8/LICENSE
--rw-r--r--   0        0        0      388 2021-04-15 20:15:55.706041 mtg_parser-0.0.1a8/README.md
--rw-r--r--   0        0        0     1130 2021-04-15 20:04:27.862662 mtg_parser-0.0.1a8/pyproject.toml
--rw-r--r--   0        0        0      440 2021-04-15 20:18:38.482768 mtg_parser-0.0.1a8/src/mtg_parser/__init__.py
--rw-r--r--   0        0        0     1506 2021-04-15 19:38:10.417225 mtg_parser-0.0.1a8/src/mtg_parser/archidekt.py
--rw-r--r--   0        0        0     1261 2021-04-15 19:53:10.752637 mtg_parser-0.0.1a8/src/mtg_parser/decklist.py
--rw-r--r--   0        0        0     1183 2021-04-15 19:35:31.390554 mtg_parser-0.0.1a8/src/mtg_parser/deckstats.py
--rw-r--r--   0        0        0      473 2021-04-14 20:47:52.620302 mtg_parser-0.0.1a8/src/mtg_parser/diff.py
--rw-r--r--   0        0        0     1376 2021-04-02 15:57:58.761813 mtg_parser-0.0.1a8/src/mtg_parser/gramar.py
--rw-r--r--   0        0        0     1266 2021-04-15 19:49:32.027356 mtg_parser-0.0.1a8/src/mtg_parser/moxfield.py
--rw-r--r--   0        0        0      731 2021-04-15 19:27:00.084676 mtg_parser-0.0.1a8/src/mtg_parser/parser.py
--rw-r--r--   0        0        0      708 2021-04-15 19:50:35.960988 mtg_parser-0.0.1a8/src/mtg_parser/tappedout.py
--rw-r--r--   0        0        0     1042 2021-04-15 12:35:37.701946 mtg_parser-0.0.1a8/src/mtg_parser/utils.py
--rw-r--r--   0        0        0     1224 2021-04-15 20:18:39.594256 mtg_parser-0.0.1a8/setup.py
--rw-r--r--   0        0        0     1176 2021-04-15 20:18:39.594570 mtg_parser-0.0.1a8/PKG-INFO
+-rw-r--r--   0        0        0     1074 2021-03-28 21:26:17.680739 mtg_parser-0.0.1a9/LICENSE
+-rw-r--r--   0        0        0      388 2021-04-15 20:15:55.706041 mtg_parser-0.0.1a9/README.md
+-rw-r--r--   0        0        0     1156 2021-04-16 21:01:47.177888 mtg_parser-0.0.1a9/pyproject.toml
+-rw-r--r--   0        0        0      484 2021-04-16 21:02:31.791127 mtg_parser-0.0.1a9/src/mtg_parser/__init__.py
+-rw-r--r--   0        0        0     1506 2021-04-15 19:38:10.417225 mtg_parser-0.0.1a9/src/mtg_parser/archidekt.py
+-rw-r--r--   0        0        0     1261 2021-04-15 19:53:10.752637 mtg_parser-0.0.1a9/src/mtg_parser/decklist.py
+-rw-r--r--   0        0        0     1183 2021-04-15 19:35:31.390554 mtg_parser-0.0.1a9/src/mtg_parser/deckstats.py
+-rw-r--r--   0        0        0      473 2021-04-14 20:47:52.620302 mtg_parser-0.0.1a9/src/mtg_parser/diff.py
+-rw-r--r--   0        0        0     1376 2021-04-02 15:57:58.761813 mtg_parser-0.0.1a9/src/mtg_parser/gramar.py
+-rw-r--r--   0        0        0     1266 2021-04-15 19:49:32.027356 mtg_parser-0.0.1a9/src/mtg_parser/moxfield.py
+-rw-r--r--   0        0        0     1440 2021-04-16 20:43:47.600692 mtg_parser-0.0.1a9/src/mtg_parser/mtggoldfish.py
+-rw-r--r--   0        0        0      731 2021-04-15 19:27:00.084676 mtg_parser-0.0.1a9/src/mtg_parser/parser.py
+-rw-r--r--   0        0        0      708 2021-04-15 19:50:35.960988 mtg_parser-0.0.1a9/src/mtg_parser/tappedout.py
+-rw-r--r--   0        0        0     1042 2021-04-15 12:35:37.701946 mtg_parser-0.0.1a9/src/mtg_parser/utils.py
+-rw-r--r--   0        0        0     1258 2021-04-16 21:02:32.899379 mtg_parser-0.0.1a9/setup.py
+-rw-r--r--   0        0        0     1223 2021-04-16 21:02:32.899659 mtg_parser-0.0.1a9/PKG-INFO
```

### Comparing `mtg_parser-0.0.1a8/LICENSE` & `mtg_parser-0.0.1a9/LICENSE`

 * *Files identical despite different names*

### Comparing `mtg_parser-0.0.1a8/pyproject.toml` & `mtg_parser-0.0.1a9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "mtg_parser"
-version = "0.0.1-alpha.8"
+version = "0.0.1-alpha.9"
 license = "MIT"
 description = "Magic: the Gathering decklist parser"
 readme = "README.md"
 authors = ["Ludovic Heyberger <940408+lheyberger@users.noreply.github.com>"]
 homepage = "https://github.com/lheyberger/mtg-parser"
 repository = "https://github.com/lheyberger/mtg-parser"
 documentation = "https://github.com/lheyberger/mtg-parser"
 
 
 [tool.poetry.dependencies]
 python = "^3.7"
 pyparsing = "^2.4.7"
 requests = "^2.25.1"
+beautifulsoup4 = "^4.9.3"
 
 
 [tool.poetry.dev-dependencies]
 coverage = {extras = ["toml"], version = "^5.5"}
 pytest = "^6.2.2"
 check-wheel-contents = "^0.2.0"
 pylint = "^2.7.4"
```

### Comparing `mtg_parser-0.0.1a8/src/mtg_parser/archidekt.py` & `mtg_parser-0.0.1a9/src/mtg_parser/archidekt.py`

 * *Files identical despite different names*

### Comparing `mtg_parser-0.0.1a8/src/mtg_parser/decklist.py` & `mtg_parser-0.0.1a9/src/mtg_parser/decklist.py`

 * *Files identical despite different names*

### Comparing `mtg_parser-0.0.1a8/src/mtg_parser/deckstats.py` & `mtg_parser-0.0.1a9/src/mtg_parser/deckstats.py`

 * *Files identical despite different names*

### Comparing `mtg_parser-0.0.1a8/src/mtg_parser/gramar.py` & `mtg_parser-0.0.1a9/src/mtg_parser/gramar.py`

 * *Files identical despite different names*

### Comparing `mtg_parser-0.0.1a8/src/mtg_parser/moxfield.py` & `mtg_parser-0.0.1a9/src/mtg_parser/moxfield.py`

 * *Files identical despite different names*

### Comparing `mtg_parser-0.0.1a8/src/mtg_parser/parser.py` & `mtg_parser-0.0.1a9/src/mtg_parser/parser.py`

 * *Files identical despite different names*

### Comparing `mtg_parser-0.0.1a8/src/mtg_parser/tappedout.py` & `mtg_parser-0.0.1a9/src/mtg_parser/tappedout.py`

 * *Files identical despite different names*

### Comparing `mtg_parser-0.0.1a8/src/mtg_parser/utils.py` & `mtg_parser-0.0.1a9/src/mtg_parser/utils.py`

 * *Files identical despite different names*

### Comparing `mtg_parser-0.0.1a8/setup.py` & `mtg_parser-0.0.1a9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,19 +7,21 @@
 packages = \
 ['mtg_parser']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['pyparsing>=2.4.7,<3.0.0', 'requests>=2.25.1,<3.0.0']
+['beautifulsoup4>=4.9.3,<5.0.0',
+ 'pyparsing>=2.4.7,<3.0.0',
+ 'requests>=2.25.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'mtg-parser',
-    'version': '0.0.1a8',
+    'version': '0.0.1a9',
     'description': 'Magic: the Gathering decklist parser',
     'long_description': '# mtg-parser\n\n\n## How to install\n\n\tpip install mtg-parser\n\n\n## How to use\n\n\timport mtg_parser\n\t\n\tdecklist = """\n\t\t1 Atraxa, Praetors\' Voice\n\t\t1 Imperial Seal\n\t\t1 Lim-Dûl\'s Vault\n\t\t1 Jeweled Lotus (CMR) 319\n\t\t1 Llanowar Elves (M12) 182\n\t\t3 Brainstorm #Card Advantage #Draw\n\t"""\n\t\n\tcards = mtg_parser.parse_deck(decklist)\n\t\n\tfor card in cards:\n\t\tprint(card[\'quantity\'], card[\'card_name\'])\n',
     'author': 'Ludovic Heyberger',
     'author_email': '940408+lheyberger@users.noreply.github.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/lheyberger/mtg-parser',
```

### Comparing `mtg_parser-0.0.1a8/PKG-INFO` & `mtg_parser-0.0.1a9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: mtg-parser
-Version: 0.0.1a8
+Version: 0.0.1a9
 Summary: Magic: the Gathering decklist parser
 Home-page: https://github.com/lheyberger/mtg-parser
 License: MIT
 Author: Ludovic Heyberger
 Author-email: 940408+lheyberger@users.noreply.github.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: beautifulsoup4 (>=4.9.3,<5.0.0)
 Requires-Dist: pyparsing (>=2.4.7,<3.0.0)
 Requires-Dist: requests (>=2.25.1,<3.0.0)
 Project-URL: Documentation, https://github.com/lheyberger/mtg-parser
 Project-URL: Repository, https://github.com/lheyberger/mtg-parser
 Description-Content-Type: text/markdown
 
 # mtg-parser
```

