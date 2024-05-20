# Comparing `tmp/fol_parser-0.2.0.tar.gz` & `tmp/fol_parser-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fol_parser-0.2.0.tar", max compression
+gzip compressed data, was "fol_parser-0.3.0.tar", max compression
```

## Comparing `fol_parser-0.2.0.tar` & `fol_parser-0.3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      102 2024-05-18 18:09:05.865684 fol_parser-0.2.0/README.md
--rw-r--r--   0        0        0     6148 2024-05-19 19:13:03.059664 fol_parser-0.2.0/fol_parser/ANTLR/.DS_Store
--rw-r--r--   0        0        0     4116 2024-05-18 18:48:59.529653 fol_parser-0.2.0/fol_parser/ANTLR/.antlr/FOL.interp
--rw-r--r--   0        0        0     1071 2024-05-18 18:48:59.729232 fol_parser-0.2.0/fol_parser/ANTLR/.antlr/FOL.tokens
--rw-r--r--   0        0        0     9023 2024-05-18 18:48:59.703534 fol_parser-0.2.0/fol_parser/ANTLR/.antlr/FOLBaseListener.java
--rw-r--r--   0        0        0    19908 2024-05-18 18:48:59.048272 fol_parser-0.2.0/fol_parser/ANTLR/.antlr/FOLLexer.interp
--rw-r--r--   0        0        0    32808 2024-05-18 18:48:59.309989 fol_parser-0.2.0/fol_parser/ANTLR/.antlr/FOLLexer.java
--rw-r--r--   0        0        0     1071 2024-05-18 18:48:59.357771 fol_parser-0.2.0/fol_parser/ANTLR/.antlr/FOLLexer.tokens
--rw-r--r--   0        0        0     9909 2024-05-18 18:48:59.699941 fol_parser-0.2.0/fol_parser/ANTLR/.antlr/FOLListener.java
--rw-r--r--   0        0        0    36403 2024-05-18 18:48:59.688741 fol_parser-0.2.0/fol_parser/ANTLR/.antlr/FOLParser.java
--rw-r--r--   0        0        0     6246 2024-05-18 17:10:27.451400 fol_parser-0.2.0/fol_parser/ANTLR/FOL.g4
--rw-r--r--   0        0        0     4116 2024-05-19 11:08:28.597752 fol_parser-0.2.0/fol_parser/ANTLR/FOL.interp
--rw-r--r--   0        0        0     1071 2024-05-19 11:08:28.758622 fol_parser-0.2.0/fol_parser/ANTLR/FOL.tokens
--rw-r--r--   0        0        0    19908 2024-05-19 11:08:28.327569 fol_parser-0.2.0/fol_parser/ANTLR/FOLLexer.interp
--rw-r--r--   0        0        0    19154 2024-05-19 11:08:28.465327 fol_parser-0.2.0/fol_parser/ANTLR/FOLLexer.py
--rw-r--r--   0        0        0     1071 2024-05-19 11:08:28.502961 fol_parser-0.2.0/fol_parser/ANTLR/FOLLexer.tokens
--rw-r--r--   0        0        0     7066 2024-05-19 11:08:28.736372 fol_parser-0.2.0/fol_parser/ANTLR/FOLListener.py
--rw-r--r--   0        0        0    38834 2024-05-19 11:08:28.729232 fol_parser-0.2.0/fol_parser/ANTLR/FOLParser.py
--rw-r--r--   0        0        0        0 2024-05-19 18:56:43.425438 fol_parser-0.2.0/fol_parser/ANTLR/__init__.py
--rw-r--r--   0        0        0    27641 2024-05-19 06:47:11.366337 fol_parser-0.2.0/fol_parser/ANTLR/__pycache__/FOLLexer.cpython-311.pyc
--rw-r--r--   0        0        0    29283 2024-05-19 11:08:33.568207 fol_parser-0.2.0/fol_parser/ANTLR/__pycache__/FOLLexer.cpython-312.pyc
--rw-r--r--   0        0        0    60825 2024-05-19 11:08:33.575144 fol_parser-0.2.0/fol_parser/ANTLR/__pycache__/FOLParser.cpython-312.pyc
--rw-r--r--   0        0        0        0 2024-05-19 18:56:25.661954 fol_parser-0.2.0/fol_parser/__init__.py
--rw-r--r--   0        0        0     2774 2024-05-19 11:08:33.615809 fol_parser-0.2.0/fol_parser/graphs/parse_tree.gv
--rw-r--r--   0        0        0    27068 2024-05-19 11:08:33.938900 fol_parser-0.2.0/fol_parser/graphs/parse_tree.gv.pdf
--rw-r--r--   0        0        0      965 2024-05-19 06:45:44.762505 fol_parser-0.2.0/fol_parser/main.py
--rw-r--r--   0        0        0      950 2024-05-19 19:02:27.797468 fol_parser-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 fol_parser-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      278 2024-05-20 15:44:39.469336 fol_parser-0.3.0/README.md
+-rw-r--r--   0        0        0     6148 2024-05-19 19:13:03.059664 fol_parser-0.3.0/fol_parser/ANTLR/.DS_Store
+-rw-r--r--   0        0        0     4116 2024-05-18 18:48:59.529653 fol_parser-0.3.0/fol_parser/ANTLR/.antlr/FOL.interp
+-rw-r--r--   0        0        0     1071 2024-05-18 18:48:59.729232 fol_parser-0.3.0/fol_parser/ANTLR/.antlr/FOL.tokens
+-rw-r--r--   0        0        0     9023 2024-05-18 18:48:59.703534 fol_parser-0.3.0/fol_parser/ANTLR/.antlr/FOLBaseListener.java
+-rw-r--r--   0        0        0    19908 2024-05-18 18:48:59.048272 fol_parser-0.3.0/fol_parser/ANTLR/.antlr/FOLLexer.interp
+-rw-r--r--   0        0        0    32808 2024-05-18 18:48:59.309989 fol_parser-0.3.0/fol_parser/ANTLR/.antlr/FOLLexer.java
+-rw-r--r--   0        0        0     1071 2024-05-18 18:48:59.357771 fol_parser-0.3.0/fol_parser/ANTLR/.antlr/FOLLexer.tokens
+-rw-r--r--   0        0        0     9909 2024-05-18 18:48:59.699941 fol_parser-0.3.0/fol_parser/ANTLR/.antlr/FOLListener.java
+-rw-r--r--   0        0        0    36403 2024-05-18 18:48:59.688741 fol_parser-0.3.0/fol_parser/ANTLR/.antlr/FOLParser.java
+-rw-r--r--   0        0        0     6246 2024-05-18 17:10:27.451400 fol_parser-0.3.0/fol_parser/ANTLR/FOL.g4
+-rw-r--r--   0        0        0     4116 2024-05-19 11:08:28.597752 fol_parser-0.3.0/fol_parser/ANTLR/FOL.interp
+-rw-r--r--   0        0        0     1071 2024-05-19 11:08:28.758622 fol_parser-0.3.0/fol_parser/ANTLR/FOL.tokens
+-rw-r--r--   0        0        0    19908 2024-05-19 11:08:28.327569 fol_parser-0.3.0/fol_parser/ANTLR/FOLLexer.interp
+-rw-r--r--   0        0        0    19154 2024-05-19 11:08:28.465327 fol_parser-0.3.0/fol_parser/ANTLR/FOLLexer.py
+-rw-r--r--   0        0        0     1071 2024-05-19 11:08:28.502961 fol_parser-0.3.0/fol_parser/ANTLR/FOLLexer.tokens
+-rw-r--r--   0        0        0     7066 2024-05-19 11:08:28.736372 fol_parser-0.3.0/fol_parser/ANTLR/FOLListener.py
+-rw-r--r--   0        0        0    38834 2024-05-19 11:08:28.729232 fol_parser-0.3.0/fol_parser/ANTLR/FOLParser.py
+-rw-r--r--   0        0        0        0 2024-05-19 18:56:43.425438 fol_parser-0.3.0/fol_parser/ANTLR/__init__.py
+-rw-r--r--   0        0        0    27641 2024-05-19 06:47:11.366337 fol_parser-0.3.0/fol_parser/ANTLR/__pycache__/FOLLexer.cpython-311.pyc
+-rw-r--r--   0        0        0    29283 2024-05-19 11:08:33.568207 fol_parser-0.3.0/fol_parser/ANTLR/__pycache__/FOLLexer.cpython-312.pyc
+-rw-r--r--   0        0        0    60825 2024-05-19 11:08:33.575144 fol_parser-0.3.0/fol_parser/ANTLR/__pycache__/FOLParser.cpython-312.pyc
+-rw-r--r--   0        0        0        0 2024-05-19 18:56:25.661954 fol_parser-0.3.0/fol_parser/__init__.py
+-rw-r--r--   0        0        0     2774 2024-05-19 11:08:33.615809 fol_parser-0.3.0/fol_parser/graphs/parse_tree.gv
+-rw-r--r--   0        0        0    27068 2024-05-19 11:08:33.938900 fol_parser-0.3.0/fol_parser/graphs/parse_tree.gv.pdf
+-rw-r--r--   0        0        0      965 2024-05-19 06:45:44.762505 fol_parser-0.3.0/fol_parser/main.py
+-rw-r--r--   0        0        0      950 2024-05-20 15:45:03.701353 fol_parser-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      674 1970-01-01 00:00:00.000000 fol_parser-0.3.0/PKG-INFO
```

### Comparing `fol_parser-0.2.0/fol_parser/ANTLR/.DS_Store` & `fol_parser-0.3.0/fol_parser/ANTLR/.DS_Store`

 * *Files identical despite different names*

### Comparing `fol_parser-0.2.0/fol_parser/ANTLR/.antlr/FOL.interp` & `fol_parser-0.3.0/fol_parser/ANTLR/.antlr/FOL.interp`

 * *Files identical despite different names*

### Comparing `fol_parser-0.2.0/fol_parser/ANTLR/.antlr/FOL.tokens` & `fol_parser-0.3.0/fol_parser/ANTLR/.antlr/FOL.tokens`

 * *Files identical despite different names*

### Comparing `fol_parser-0.2.0/fol_parser/ANTLR/.antlr/FOLBaseListener.java` & `fol_parser-0.3.0/fol_parser/ANTLR/.antlr/FOLBaseListener.java`

 * *Files identical despite different names*

### Comparing `fol_parser-0.2.0/fol_parser/ANTLR/.antlr/FOLLexer.interp` & `fol_parser-0.3.0/fol_parser/ANTLR/.antlr/FOLLexer.interp`

 * *Files identical despite different names*

### Comparing `fol_parser-0.2.0/fol_parser/ANTLR/.antlr/FOLLexer.java` & `fol_parser-0.3.0/fol_parser/ANTLR/.antlr/FOLLexer.java`

 * *Files identical despite different names*

### Comparing `fol_parser-0.2.0/fol_parser/ANTLR/.antlr/FOLLexer.tokens` & `fol_parser-0.3.0/fol_parser/ANTLR/.antlr/FOLLexer.tokens`

 * *Files identical despite different names*

### Comparing `fol_parser-0.2.0/fol_parser/ANTLR/.antlr/FOLListener.java` & `fol_parser-0.3.0/fol_parser/ANTLR/.antlr/FOLListener.java`

 * *Files identical despite different names*

### Comparing `fol_parser-0.2.0/fol_parser/ANTLR/.antlr/FOLParser.java` & `fol_parser-0.3.0/fol_parser/ANTLR/.antlr/FOLParser.java`

 * *Files identical despite different names*

### Comparing `fol_parser-0.2.0/fol_parser/ANTLR/FOL.g4` & `fol_parser-0.3.0/fol_parser/ANTLR/FOL.g4`

 * *Files identical despite different names*

### Comparing `fol_parser-0.2.0/fol_parser/ANTLR/FOL.interp` & `fol_parser-0.3.0/fol_parser/ANTLR/FOL.interp`

 * *Files identical despite different names*

### Comparing `fol_parser-0.2.0/fol_parser/ANTLR/FOL.tokens` & `fol_parser-0.3.0/fol_parser/ANTLR/FOL.tokens`

 * *Files identical despite different names*

### Comparing `fol_parser-0.2.0/fol_parser/ANTLR/FOLLexer.interp` & `fol_parser-0.3.0/fol_parser/ANTLR/FOLLexer.interp`

 * *Files identical despite different names*

### Comparing `fol_parser-0.2.0/fol_parser/ANTLR/FOLLexer.py` & `fol_parser-0.3.0/fol_parser/ANTLR/FOLLexer.py`

 * *Files identical despite different names*

### Comparing `fol_parser-0.2.0/fol_parser/ANTLR/FOLLexer.tokens` & `fol_parser-0.3.0/fol_parser/ANTLR/FOLLexer.tokens`

 * *Files identical despite different names*

### Comparing `fol_parser-0.2.0/fol_parser/ANTLR/FOLListener.py` & `fol_parser-0.3.0/fol_parser/ANTLR/FOLListener.py`

 * *Files identical despite different names*

### Comparing `fol_parser-0.2.0/fol_parser/ANTLR/FOLParser.py` & `fol_parser-0.3.0/fol_parser/ANTLR/FOLParser.py`

 * *Files identical despite different names*

### Comparing `fol_parser-0.2.0/fol_parser/ANTLR/__pycache__/FOLLexer.cpython-311.pyc` & `fol_parser-0.3.0/fol_parser/ANTLR/__pycache__/FOLLexer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fol_parser-0.2.0/fol_parser/ANTLR/__pycache__/FOLLexer.cpython-312.pyc` & `fol_parser-0.3.0/fol_parser/ANTLR/__pycache__/FOLLexer.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `fol_parser-0.2.0/fol_parser/ANTLR/__pycache__/FOLParser.cpython-312.pyc` & `fol_parser-0.3.0/fol_parser/ANTLR/__pycache__/FOLParser.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `fol_parser-0.2.0/fol_parser/graphs/parse_tree.gv` & `fol_parser-0.3.0/fol_parser/graphs/parse_tree.gv`

 * *Files identical despite different names*

### Comparing `fol_parser-0.2.0/fol_parser/graphs/parse_tree.gv.pdf` & `fol_parser-0.3.0/fol_parser/graphs/parse_tree.gv.pdf`

 * *Files identical despite different names*

### Comparing `fol_parser-0.2.0/fol_parser/main.py` & `fol_parser-0.3.0/fol_parser/main.py`

 * *Files identical despite different names*

### Comparing `fol_parser-0.2.0/pyproject.toml` & `fol_parser-0.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fol_parser"
-version = "0.2.0"
+version = "0.3.0"
 description = "FOL Parser"
 authors = ["Emre Kuru <emre.kuru@ozu.edu.tr>"]
 readme = "README.md"
 
 packages = [
     { include = "fol_parser" }
 ]
```

