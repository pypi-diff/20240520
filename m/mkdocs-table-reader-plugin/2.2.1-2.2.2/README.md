# Comparing `tmp/mkdocs_table_reader_plugin-2.2.1.tar.gz` & `tmp/mkdocs_table_reader_plugin-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_table_reader_plugin-2.2.1.tar", last modified: Tue May  7 09:20:57 2024, max compression
+gzip compressed data, was "mkdocs_table_reader_plugin-2.2.2.tar", last modified: Mon May 20 11:19:14 2024, max compression
```

## Comparing `mkdocs_table_reader_plugin-2.2.1.tar` & `mkdocs_table_reader_plugin-2.2.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:20:57.381267 mkdocs_table_reader_plugin-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-07 09:20:21.000000 mkdocs_table_reader_plugin-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-05-07 09:20:57.381267 mkdocs_table_reader_plugin-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-05-07 09:20:21.000000 mkdocs_table_reader_plugin-2.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:20:57.381267 mkdocs_table_reader_plugin-2.2.1/mkdocs_table_reader_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 09:20:21.000000 mkdocs_table_reader_plugin-2.2.1/mkdocs_table_reader_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-07 09:20:21.000000 mkdocs_table_reader_plugin-2.2.1/mkdocs_table_reader_plugin/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-05-07 09:20:21.000000 mkdocs_table_reader_plugin-2.2.1/mkdocs_table_reader_plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-07 09:20:21.000000 mkdocs_table_reader_plugin-2.2.1/mkdocs_table_reader_plugin/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-05-07 09:20:21.000000 mkdocs_table_reader_plugin-2.2.1/mkdocs_table_reader_plugin/safe_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-07 09:20:21.000000 mkdocs_table_reader_plugin-2.2.1/mkdocs_table_reader_plugin/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:20:57.381267 mkdocs_table_reader_plugin-2.2.1/mkdocs_table_reader_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-05-07 09:20:57.000000 mkdocs_table_reader_plugin-2.2.1/mkdocs_table_reader_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-07 09:20:57.000000 mkdocs_table_reader_plugin-2.2.1/mkdocs_table_reader_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 09:20:57.000000 mkdocs_table_reader_plugin-2.2.1/mkdocs_table_reader_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-07 09:20:57.000000 mkdocs_table_reader_plugin-2.2.1/mkdocs_table_reader_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-07 09:20:57.000000 mkdocs_table_reader_plugin-2.2.1/mkdocs_table_reader_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-07 09:20:57.000000 mkdocs_table_reader_plugin-2.2.1/mkdocs_table_reader_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 09:20:57.381267 mkdocs_table_reader_plugin-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-07 09:20:21.000000 mkdocs_table_reader_plugin-2.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:20:57.381267 mkdocs_table_reader_plugin-2.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10979 2024-05-07 09:20:21.000000 mkdocs_table_reader_plugin-2.2.1/tests/test_build.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-07 09:20:21.000000 mkdocs_table_reader_plugin-2.2.1/tests/test_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-07 09:20:21.000000 mkdocs_table_reader_plugin-2.2.1/tests/test_markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-07 09:20:21.000000 mkdocs_table_reader_plugin-2.2.1/tests/test_safe_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:19:14.611761 mkdocs_table_reader_plugin-2.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-20 11:18:40.000000 mkdocs_table_reader_plugin-2.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-05-20 11:19:14.611761 mkdocs_table_reader_plugin-2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-05-20 11:18:40.000000 mkdocs_table_reader_plugin-2.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:19:14.607761 mkdocs_table_reader_plugin-2.2.2/mkdocs_table_reader_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:18:40.000000 mkdocs_table_reader_plugin-2.2.2/mkdocs_table_reader_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-20 11:18:40.000000 mkdocs_table_reader_plugin-2.2.2/mkdocs_table_reader_plugin/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-05-20 11:18:40.000000 mkdocs_table_reader_plugin-2.2.2/mkdocs_table_reader_plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-20 11:18:40.000000 mkdocs_table_reader_plugin-2.2.2/mkdocs_table_reader_plugin/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-05-20 11:18:40.000000 mkdocs_table_reader_plugin-2.2.2/mkdocs_table_reader_plugin/safe_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-20 11:18:40.000000 mkdocs_table_reader_plugin-2.2.2/mkdocs_table_reader_plugin/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:19:14.611761 mkdocs_table_reader_plugin-2.2.2/mkdocs_table_reader_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-05-20 11:19:14.000000 mkdocs_table_reader_plugin-2.2.2/mkdocs_table_reader_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-20 11:19:14.000000 mkdocs_table_reader_plugin-2.2.2/mkdocs_table_reader_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 11:19:14.000000 mkdocs_table_reader_plugin-2.2.2/mkdocs_table_reader_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-20 11:19:14.000000 mkdocs_table_reader_plugin-2.2.2/mkdocs_table_reader_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-20 11:19:14.000000 mkdocs_table_reader_plugin-2.2.2/mkdocs_table_reader_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-20 11:19:14.000000 mkdocs_table_reader_plugin-2.2.2/mkdocs_table_reader_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 11:19:14.611761 mkdocs_table_reader_plugin-2.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-20 11:18:40.000000 mkdocs_table_reader_plugin-2.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:19:14.611761 mkdocs_table_reader_plugin-2.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11416 2024-05-20 11:18:40.000000 mkdocs_table_reader_plugin-2.2.2/tests/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-20 11:18:40.000000 mkdocs_table_reader_plugin-2.2.2/tests/test_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-20 11:18:40.000000 mkdocs_table_reader_plugin-2.2.2/tests/test_markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-20 11:18:40.000000 mkdocs_table_reader_plugin-2.2.2/tests/test_safe_eval.py
```

### Comparing `mkdocs_table_reader_plugin-2.2.1/LICENSE` & `mkdocs_table_reader_plugin-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_table_reader_plugin-2.2.1/PKG-INFO` & `mkdocs_table_reader_plugin-2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-table-reader-plugin
-Version: 2.2.1
+Version: 2.2.2
 Summary: MkDocs plugin to directly insert tables from files into markdown.
 Home-page: https://github.com/timvink/mkdocs-table-reader-plugin
 Author: Tim Vink
 Author-email: vinktim@gmail.com
 License: MIT
 Keywords: mkdocs plugin
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocs_table_reader_plugin-2.2.1/README.md` & `mkdocs_table_reader_plugin-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_table_reader_plugin-2.2.1/mkdocs_table_reader_plugin/markdown.py` & `mkdocs_table_reader_plugin-2.2.2/mkdocs_table_reader_plugin/markdown.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 def convert_to_md_table(df: pd.DataFrame, markdown_kwargs: Dict) -> str:
     """
     Convert dataframe to markdown table using tabulate.
     """
     # Escape any pipe characters, | to \|
     # See https://github.com/astanin/python-tabulate/issues/241
-    df.columns = [replace_unescaped_pipes(c) for c in df.columns]
+    df.columns = [replace_unescaped_pipes(c) if isinstance(c, str) else c for c in df.columns]
 
     # Avoid deprecated applymap warning on pandas>=2.0
     # See https://github.com/timvink/mkdocs-table-reader-plugin/issues/55
     if pd.__version__ >= "2.1.0":
         df = df.map(lambda s: replace_unescaped_pipes(s) if isinstance(s, str) else s)
     else:
         df = df.applymap(lambda s: replace_unescaped_pipes(s) if isinstance(s, str) else s)
```

### Comparing `mkdocs_table_reader_plugin-2.2.1/mkdocs_table_reader_plugin/plugin.py` & `mkdocs_table_reader_plugin-2.2.2/mkdocs_table_reader_plugin/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,14 @@
                     else:
                         raise FileNotFoundError(msg)
                 
                 # Load the table
                 # note we use the first valid file paths,
                 # where we first search the 'data_path' and then the page's directory.
                 markdown_table = function(valid_file_paths[0], *pd_args, **pd_kwargs)
-
                 markdown_table = fix_indentation(leading_spaces, markdown_table)
 
                 # Insert markdown table
                 # By replacing only the first occurrence of the regex pattern
                 # You might insert multiple CSVs with a single reader like read_csv
                 # Because of the replacement, the next occurrence will be the first match for .sub() again.
                 # This is always why when allow_missing_files=True we replaced the input tag.
```

### Comparing `mkdocs_table_reader_plugin-2.2.1/mkdocs_table_reader_plugin/readers.py` & `mkdocs_table_reader_plugin-2.2.2/mkdocs_table_reader_plugin/readers.py`

 * *Files identical despite different names*

### Comparing `mkdocs_table_reader_plugin-2.2.1/mkdocs_table_reader_plugin/safe_eval.py` & `mkdocs_table_reader_plugin-2.2.2/mkdocs_table_reader_plugin/safe_eval.py`

 * *Files identical despite different names*

### Comparing `mkdocs_table_reader_plugin-2.2.1/mkdocs_table_reader_plugin/utils.py` & `mkdocs_table_reader_plugin-2.2.2/mkdocs_table_reader_plugin/utils.py`

 * *Files identical despite different names*

### Comparing `mkdocs_table_reader_plugin-2.2.1/mkdocs_table_reader_plugin.egg-info/PKG-INFO` & `mkdocs_table_reader_plugin-2.2.2/mkdocs_table_reader_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-table-reader-plugin
-Version: 2.2.1
+Version: 2.2.2
 Summary: MkDocs plugin to directly insert tables from files into markdown.
 Home-page: https://github.com/timvink/mkdocs-table-reader-plugin
 Author: Tim Vink
 Author-email: vinktim@gmail.com
 License: MIT
 Keywords: mkdocs plugin
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocs_table_reader_plugin-2.2.1/mkdocs_table_reader_plugin.egg-info/SOURCES.txt` & `mkdocs_table_reader_plugin-2.2.2/mkdocs_table_reader_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs_table_reader_plugin-2.2.1/setup.py` & `mkdocs_table_reader_plugin-2.2.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="mkdocs-table-reader-plugin",
-    version="2.2.1",
+    version="2.2.2",
     description="MkDocs plugin to directly insert tables from files into markdown.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="mkdocs plugin",
     url="https://github.com/timvink/mkdocs-table-reader-plugin",
     author="Tim Vink",
     author_email="vinktim@gmail.com",
```

### Comparing `mkdocs_table_reader_plugin-2.2.1/tests/test_build.py` & `mkdocs_table_reader_plugin-2.2.2/tests/test_build.py`

 * *Files 1% similar despite different names*

```diff
@@ -358,7 +358,19 @@
     result = build_docs_setup(tmp_proj)
     assert result.exit_code == 0, "'mkdocs build' command failed"
 
     # Make sure the file.csv is inserted
     page_with_tag = tmp_proj / "site/index.html"
     contents = page_with_tag.read_text()
     assert re.search(r"56", contents)
+
+def test_csv_with_no_string_headers(tmp_path):
+    tmp_proj = setup_clean_mkdocs_folder(
+        "tests/fixtures/nonstringheaders/mkdocs.yml", tmp_path
+    )
+    result = build_docs_setup(tmp_proj)
+    assert result.exit_code == 0, "'mkdocs build' command failed"
+
+    # Make sure the file.csv is inserted
+    page_with_tag = tmp_proj / "site/index.html"
+    contents = page_with_tag.read_text()
+    assert re.search(r"4242", contents)
```

### Comparing `mkdocs_table_reader_plugin-2.2.1/tests/test_kwargs.py` & `mkdocs_table_reader_plugin-2.2.2/tests/test_kwargs.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,7 +17,10 @@
 def test_parse_argkwarg():
 
     assert parse_argkwarg("sep=';'") == ([], {'sep': ';'})
     assert parse_argkwarg('"file.csv", usecols=["A", "B"]') == (['file.csv'], {'usecols': ['A', 'B']})
     assert parse_argkwarg('"file.csv", usecols=[\'A\',\'B\']') == (['file.csv'], {'usecols': ['A', 'B']})
     assert parse_argkwarg("'assets/tables/table_with_carriage_return.csv', sep = ','") == (['assets/tables/table_with_carriage_return.csv'], {'sep': ','})
     assert parse_argkwarg("'includes/statistics.csv', keep_default_na=False, colalign=('center','center','center','center','center','center','center')") == (['includes/statistics.csv'], {'keep_default_na': False, 'colalign': ('center','center','center','center','center','center','center')})
+    assert parse_argkwarg('"file.csv", header=None') == (['file.csv'], {'header': None})
+    assert parse_argkwarg("'Example.xlsx', sheet_name = 'test', header = None") == (['Example.xlsx'], {'sheet_name': 'test', 'header': None})
+    assert parse_argkwarg("'test.csv', header = None, names = ['a', 'b', 'c']") == (['test.csv'], {'header': None, 'names': ['a', 'b', 'c']})
```

### Comparing `mkdocs_table_reader_plugin-2.2.1/tests/test_markdown.py` & `mkdocs_table_reader_plugin-2.2.2/tests/test_markdown.py`

 * *Files identical despite different names*

### Comparing `mkdocs_table_reader_plugin-2.2.1/tests/test_safe_eval.py` & `mkdocs_table_reader_plugin-2.2.2/tests/test_safe_eval.py`

 * *Files identical despite different names*

