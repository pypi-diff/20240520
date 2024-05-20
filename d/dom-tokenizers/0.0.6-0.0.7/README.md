# Comparing `tmp/dom_tokenizers-0.0.6.tar.gz` & `tmp/dom_tokenizers-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dom_tokenizers-0.0.6.tar", last modified: Fri May 17 22:40:33 2024, max compression
+gzip compressed data, was "dom_tokenizers-0.0.7.tar", last modified: Sun May 19 14:33:44 2024, max compression
```

## Comparing `dom_tokenizers-0.0.6.tar` & `dom_tokenizers-0.0.7.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:40:33.270717 dom_tokenizers-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-17 22:39:53.000000 dom_tokenizers-0.0.6/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-17 22:39:53.000000 dom_tokenizers-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-17 22:39:53.000000 dom_tokenizers-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-17 22:40:33.270717 dom_tokenizers-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-17 22:39:53.000000 dom_tokenizers-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-17 22:39:53.000000 dom_tokenizers-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 22:40:33.270717 dom_tokenizers-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:40:33.262717 dom_tokenizers-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:40:33.266718 dom_tokenizers-0.0.6/src/dom_tokenizers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 22:39:53.000000 dom_tokenizers-0.0.6/src/dom_tokenizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:40:33.266718 dom_tokenizers-0.0.6/src/dom_tokenizers/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 22:39:53.000000 dom_tokenizers-0.0.6/src/dom_tokenizers/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-17 22:39:53.000000 dom_tokenizers-0.0.6/src/dom_tokenizers/internal/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:40:33.266718 dom_tokenizers-0.0.6/src/dom_tokenizers/pre_tokenizers/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-17 22:39:53.000000 dom_tokenizers-0.0.6/src/dom_tokenizers/pre_tokenizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9570 2024-05-17 22:39:53.000000 dom_tokenizers-0.0.6/src/dom_tokenizers/pre_tokenizers/dom_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-05-17 22:39:53.000000 dom_tokenizers-0.0.6/src/dom_tokenizers/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:40:33.266718 dom_tokenizers-0.0.6/src/dom_tokenizers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-17 22:40:33.000000 dom_tokenizers-0.0.6/src/dom_tokenizers.egg-info/SOURCES.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:40:33.266718 dom_tokenizers-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 22:39:53.000000 dom_tokenizers-0.0.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-17 22:39:53.000000 dom_tokenizers-0.0.6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:40:33.266718 dom_tokenizers-0.0.6/tests/pre_tokenizers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 22:39:53.000000 dom_tokenizers-0.0.6/tests/pre_tokenizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:40:33.266718 dom_tokenizers-0.0.6/tests/pre_tokenizers/dom_snapshot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 22:39:53.000000 dom_tokenizers-0.0.6/tests/pre_tokenizers/dom_snapshot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-17 22:39:53.000000 dom_tokenizers-0.0.6/tests/pre_tokenizers/dom_snapshot/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-17 22:39:53.000000 dom_tokenizers-0.0.6/tests/pre_tokenizers/dom_snapshot/test_pre_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:40:33.266718 dom_tokenizers-0.0.6/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-17 22:39:53.000000 dom_tokenizers-0.0.6/tests/resources/raw-browser-response.html
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-17 22:39:53.000000 dom_tokenizers-0.0.6/tests/resources/raw-browser-response.json
--rw-r--r--   0 runner    (1001) docker     (127)    47499 2024-05-17 22:39:53.000000 dom_tokenizers-0.0.6/tests/resources/svg-in-base64.html
--rw-r--r--   0 runner    (1001) docker     (127)    48905 2024-05-17 22:39:53.000000 dom_tokenizers-0.0.6/tests/resources/svg-in-base64.json
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-17 22:39:53.000000 dom_tokenizers-0.0.6/tests/test_train_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-17 22:39:53.000000 dom_tokenizers-0.0.6/tests/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:33:44.354430 dom_tokenizers-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-19 14:33:44.354430 dom_tokenizers-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 14:33:44.354430 dom_tokenizers-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:33:44.350429 dom_tokenizers-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:33:44.350429 dom_tokenizers-0.0.7/src/dom_tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/src/dom_tokenizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/src/dom_tokenizers/dump.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:33:44.354430 dom_tokenizers-0.0.7/src/dom_tokenizers/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/src/dom_tokenizers/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/src/dom_tokenizers/internal/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:33:44.354430 dom_tokenizers-0.0.7/src/dom_tokenizers/pre_tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/src/dom_tokenizers/pre_tokenizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9570 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/src/dom_tokenizers/pre_tokenizers/dom_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/src/dom_tokenizers/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:33:44.354430 dom_tokenizers-0.0.7/src/dom_tokenizers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-19 14:33:44.000000 dom_tokenizers-0.0.7/src/dom_tokenizers.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:33:44.354430 dom_tokenizers-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:33:44.354430 dom_tokenizers-0.0.7/tests/pre_tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/tests/pre_tokenizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:33:44.354430 dom_tokenizers-0.0.7/tests/pre_tokenizers/dom_snapshot/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/tests/pre_tokenizers/dom_snapshot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/tests/pre_tokenizers/dom_snapshot/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/tests/pre_tokenizers/dom_snapshot/test_pre_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:33:44.354430 dom_tokenizers-0.0.7/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/tests/resources/raw-browser-response.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/tests/resources/raw-browser-response.json
+-rw-r--r--   0 runner    (1001) docker     (127)    47499 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/tests/resources/svg-in-base64.html
+-rw-r--r--   0 runner    (1001) docker     (127)    48905 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/tests/resources/svg-in-base64.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/tests/test_train_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/tests/util.py
```

### Comparing `dom_tokenizers-0.0.6/LICENSE` & `dom_tokenizers-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dom_tokenizers-0.0.6/PKG-INFO` & `dom_tokenizers-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dom-tokenizers
-Version: 0.0.6
+Version: 0.0.7
 Summary: DOM-aware tokenizers for 🤗 Hugging Face language models
 Author: Gary Benson
 License: Apache-2.0
 Project-URL: Source, https://github.com/gbenson/dom-tokenizers
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dom-tokenizers Version: 0.0.6 Summary: DOM-aware
+Metadata-Version: 2.1 Name: dom-tokenizers Version: 0.0.7 Summary: DOM-aware
 tokenizers for ð¤Â HuggingÂ Face language models Author: Gary Benson License:
 Apache-2.0 Project-URL: Source, https://github.com/gbenson/dom-tokenizers
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

### Comparing `dom_tokenizers-0.0.6/README.md` & `dom_tokenizers-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `dom_tokenizers-0.0.6/pyproject.toml` & `dom_tokenizers-0.0.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dom-tokenizers"
-version = "0.0.6"
+version = "0.0.7"
 authors = [{ name = "Gary Benson" }]
 description = "DOM-aware tokenizers for 🤗 Hugging Face language models"
 readme = "README.md"
 license = { text = "Apache-2.0" }
 requires-python = ">=3.10"  # match..case
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -26,15 +26,15 @@
 dependencies = [
     "python-magic",
     "tokenizers",
     "transformers",
 ]
 
 [project.urls]
-#Homepage = "https://github.com/gbenson/dom-tokenizers"
+#Homepage = f"https://huggingface.co/gbenson/dom-tokenizer-{size}"
 Source = "https://github.com/gbenson/dom-tokenizers"
 
 [project.optional-dependencies]
 dev = [
     "build",
     "datasets",
     "flake8",
@@ -44,14 +44,15 @@
 train = [
     "datasets",
     "pillow",
 ]
 
 [project.scripts]
 train-tokenizer = "dom_tokenizers.train:main"
+dump-tokenizations = "dom_tokenizers.dump:main"
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.pytest.ini_options]
 addopts = "--cov=dom_tokenizers"
```

### Comparing `dom_tokenizers-0.0.6/src/dom_tokenizers/internal/transformers.py` & `dom_tokenizers-0.0.7/src/dom_tokenizers/internal/transformers.py`

 * *Files identical despite different names*

### Comparing `dom_tokenizers-0.0.6/src/dom_tokenizers/pre_tokenizers/dom_snapshot.py` & `dom_tokenizers-0.0.7/src/dom_tokenizers/pre_tokenizers/dom_snapshot.py`

 * *Files identical despite different names*

### Comparing `dom_tokenizers-0.0.6/src/dom_tokenizers/train.py` & `dom_tokenizers-0.0.7/src/dom_tokenizers/train.py`

 * *Files 15% similar despite different names*

```diff
@@ -114,56 +114,56 @@
     unit_index, whole = divmod(floor(whole), 3)
     value = round(10 ** (whole + frac))
     unit = ([""] + list("kMBTQ"))[unit_index]
     return f"{value}{unit}"
 
 
 def main():
-    p = ArgumentParser(
+    parser = ArgumentParser(
         description="Train DOM-aware tokenizers.",
         epilog=f"Report bugs to: <{SEND_BUGS_TO}>.")
-    p.add_argument(
+    parser.add_argument(
         "dataset", metavar="DATASET",
         help="dataset containing the training corpus")
-    p.add_argument(
+    parser.add_argument(
         "--base-tokenizer", metavar="ID",
         default=DEFAULT_BASE_TOKENIZER,
         help=(f"tokenizer to train ours from"
               f" [default: {DEFAULT_BASE_TOKENIZER}]"))
-    p.add_argument(
-        "--split", default=DEFAULT_SPLIT, metavar="SPLIT", dest="split_name",
+    parser.add_argument(
+        "-s", "--split", metavar="SPLIT", default=DEFAULT_SPLIT,
         help=(f"split of the training dataset to use"
               f" [default: {DEFAULT_SPLIT}]"))
-    p.add_argument(
+    parser.add_argument(
         "-N", "--num-inputs", metavar="N", dest="corpus_size",
         type=int,
         help=("number of sequences in the training dataset, if known;"
               " this is used to provide meaningful progress tracking"))
-    p.add_argument(
+    parser.add_argument(
         "-n", "--num-tokens", metavar="N", dest="vocab_size", type=int,
         default=DEFAULT_SIZE,
         help=(f"desired vocabulary size, including all special tokens and"
               f" the initial alphabet [default: {DEFAULT_SIZE} tokens]"))
-    p.add_argument(
+    parser.add_argument(
         "-o", "--output", metavar="DIR", dest="save_directory",
         help=("directory to save the trained tokenizer into"
               " [default: something based on targeted vocabulary size]"))
-    args = p.parse_args()
+    args = parser.parse_args()
 
     save_directory = args.save_directory
     if save_directory is None:
         save_directory = _save_directory_for(vocab_size=args.vocab_size)
         print(f"Output directory: {save_directory}\n")
 
     warnings.filterwarnings("ignore", message=r".*resume_download.*")
 
     tokenizer = train_tokenizer(
         load_dataset(
             args.dataset,
-            split=args.split_name,
+            split=args.split,
             streaming=True),
         base_tokenizer=args.base_tokenizer,
         vocab_size=args.vocab_size,
         corpus_size=args.corpus_size)
     print(f'\n{tokenizer.tokenize("training complete")}')
 
     tokenizer.save_pretrained(save_directory)
```

### Comparing `dom_tokenizers-0.0.6/src/dom_tokenizers.egg-info/SOURCES.txt` & `dom_tokenizers-0.0.7/src/dom_tokenizers.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 .flake8
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 src/dom_tokenizers/__init__.py
+src/dom_tokenizers/dump.py
 src/dom_tokenizers/train.py
 src/dom_tokenizers/internal/__init__.py
 src/dom_tokenizers/internal/transformers.py
 src/dom_tokenizers/pre_tokenizers/__init__.py
 src/dom_tokenizers/pre_tokenizers/dom_snapshot.py
 tests/__init__.py
 tests/conftest.py
```

### Comparing `dom_tokenizers-0.0.6/tests/conftest.py` & `dom_tokenizers-0.0.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dom_tokenizers-0.0.6/tests/pre_tokenizers/dom_snapshot/conftest.py` & `dom_tokenizers-0.0.7/tests/pre_tokenizers/dom_snapshot/conftest.py`

 * *Files identical despite different names*

### Comparing `dom_tokenizers-0.0.6/tests/pre_tokenizers/dom_snapshot/test_pre_tokenizer.py` & `dom_tokenizers-0.0.7/tests/pre_tokenizers/dom_snapshot/test_pre_tokenizer.py`

 * *Files identical despite different names*

### Comparing `dom_tokenizers-0.0.6/tests/resources/raw-browser-response.json` & `dom_tokenizers-0.0.7/tests/resources/raw-browser-response.json`

 * *Files identical despite different names*

### Comparing `dom_tokenizers-0.0.6/tests/resources/svg-in-base64.html` & `dom_tokenizers-0.0.7/tests/resources/svg-in-base64.html`

 * *Files identical despite different names*

### Comparing `dom_tokenizers-0.0.6/tests/resources/svg-in-base64.json` & `dom_tokenizers-0.0.7/tests/resources/svg-in-base64.json`

 * *Files identical despite different names*

### Comparing `dom_tokenizers-0.0.6/tests/test_train_tokenizer.py` & `dom_tokenizers-0.0.7/tests/test_train_tokenizer.py`

 * *Files identical despite different names*

### Comparing `dom_tokenizers-0.0.6/tests/util.py` & `dom_tokenizers-0.0.7/tests/util.py`

 * *Files identical despite different names*

