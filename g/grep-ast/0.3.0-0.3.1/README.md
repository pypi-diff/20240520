# Comparing `tmp/grep_ast-0.3.0.tar.gz` & `tmp/grep_ast-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grep_ast-0.3.0.tar", last modified: Fri May 17 21:41:13 2024, max compression
+gzip compressed data, was "grep_ast-0.3.1.tar", last modified: Sun May 19 22:05:28 2024, max compression
```

## Comparing `grep_ast-0.3.0.tar` & `grep_ast-0.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 gauthier   (501) staff       (20)        0 2024-05-17 21:41:13.083300 grep_ast-0.3.0/
--rw-r--r--   0 gauthier   (501) staff       (20)    11358 2023-07-28 21:17:34.000000 grep_ast-0.3.0/LICENSE.txt
--rw-r--r--   0 gauthier   (501) staff       (20)       25 2023-10-19 17:15:21.000000 grep_ast-0.3.0/MANIFEST.in
--rw-r--r--   0 gauthier   (501) staff       (20)     2552 2024-05-17 21:41:13.082416 grep_ast-0.3.0/PKG-INFO
--rw-r--r--   0 gauthier   (501) staff       (20)     2255 2023-12-10 15:48:41.000000 grep_ast-0.3.0/README.md
-drwxr-xr-x   0 gauthier   (501) staff       (20)        0 2024-05-17 21:41:13.076687 grep_ast-0.3.0/grep_ast/
--rw-r--r--   0 gauthier   (501) staff       (20)       86 2023-10-19 16:59:55.000000 grep_ast-0.3.0/grep_ast/__init__.py
--rw-r--r--   0 gauthier   (501) staff       (20)      653 2023-07-29 19:09:18.000000 grep_ast-0.3.0/grep_ast/dump.py
--rwxr-xr-x   0 gauthier   (501) staff       (20)     9049 2024-05-17 21:18:06.000000 grep_ast-0.3.0/grep_ast/grep_ast.py
--rwxr-xr-x   0 gauthier   (501) staff       (20)     3377 2024-01-25 20:59:41.000000 grep_ast-0.3.0/grep_ast/main.py
--rw-r--r--   0 gauthier   (501) staff       (20)     1378 2024-05-17 21:40:39.000000 grep_ast-0.3.0/grep_ast/parsers.py
-drwxr-xr-x   0 gauthier   (501) staff       (20)        0 2024-05-17 21:41:13.081726 grep_ast-0.3.0/grep_ast.egg-info/
--rw-r--r--   0 gauthier   (501) staff       (20)     2552 2024-05-17 21:41:13.000000 grep_ast-0.3.0/grep_ast.egg-info/PKG-INFO
--rw-r--r--   0 gauthier   (501) staff       (20)      371 2024-05-17 21:41:13.000000 grep_ast-0.3.0/grep_ast.egg-info/SOURCES.txt
--rw-r--r--   0 gauthier   (501) staff       (20)        1 2024-05-17 21:41:13.000000 grep_ast-0.3.0/grep_ast.egg-info/dependency_links.txt
--rw-r--r--   0 gauthier   (501) staff       (20)       74 2024-05-17 21:41:13.000000 grep_ast-0.3.0/grep_ast.egg-info/entry_points.txt
--rw-r--r--   0 gauthier   (501) staff       (20)       38 2024-05-17 21:41:13.000000 grep_ast-0.3.0/grep_ast.egg-info/requires.txt
--rw-r--r--   0 gauthier   (501) staff       (20)        9 2024-05-17 21:41:13.000000 grep_ast-0.3.0/grep_ast.egg-info/top_level.txt
--rw-r--r--   0 gauthier   (501) staff       (20)       38 2023-12-10 15:44:50.000000 grep_ast-0.3.0/requirements.txt
--rw-r--r--   0 gauthier   (501) staff       (20)       38 2024-05-17 21:41:13.083438 grep_ast-0.3.0/setup.cfg
--rw-r--r--   0 gauthier   (501) staff       (20)      765 2024-05-17 21:40:20.000000 grep_ast-0.3.0/setup.py
-drwxr-xr-x   0 gauthier   (501) staff       (20)        0 2024-05-17 21:41:13.080761 grep_ast-0.3.0/tests/
--rw-r--r--   0 gauthier   (501) staff       (20)      247 2023-12-10 15:44:50.000000 grep_ast-0.3.0/tests/test_parsers.py
+drwxr-xr-x   0 gauthier   (501) staff       (20)        0 2024-05-19 22:05:28.407718 grep_ast-0.3.1/
+-rw-r--r--   0 gauthier   (501) staff       (20)    11358 2023-07-28 21:17:34.000000 grep_ast-0.3.1/LICENSE.txt
+-rw-r--r--   0 gauthier   (501) staff       (20)       25 2023-10-19 17:15:21.000000 grep_ast-0.3.1/MANIFEST.in
+-rw-r--r--   0 gauthier   (501) staff       (20)     2552 2024-05-19 22:05:28.407207 grep_ast-0.3.1/PKG-INFO
+-rw-r--r--   0 gauthier   (501) staff       (20)     2255 2023-12-10 15:48:41.000000 grep_ast-0.3.1/README.md
+drwxr-xr-x   0 gauthier   (501) staff       (20)        0 2024-05-19 22:05:28.402908 grep_ast-0.3.1/grep_ast/
+-rw-r--r--   0 gauthier   (501) staff       (20)       86 2023-10-19 16:59:55.000000 grep_ast-0.3.1/grep_ast/__init__.py
+-rw-r--r--   0 gauthier   (501) staff       (20)      653 2023-07-29 19:09:18.000000 grep_ast-0.3.1/grep_ast/dump.py
+-rwxr-xr-x   0 gauthier   (501) staff       (20)     9236 2024-05-19 02:51:37.000000 grep_ast-0.3.1/grep_ast/grep_ast.py
+-rwxr-xr-x   0 gauthier   (501) staff       (20)     3377 2024-01-25 20:59:41.000000 grep_ast-0.3.1/grep_ast/main.py
+-rw-r--r--   0 gauthier   (501) staff       (20)     1378 2024-05-17 21:40:39.000000 grep_ast-0.3.1/grep_ast/parsers.py
+drwxr-xr-x   0 gauthier   (501) staff       (20)        0 2024-05-19 22:05:28.406718 grep_ast-0.3.1/grep_ast.egg-info/
+-rw-r--r--   0 gauthier   (501) staff       (20)     2552 2024-05-19 22:05:28.000000 grep_ast-0.3.1/grep_ast.egg-info/PKG-INFO
+-rw-r--r--   0 gauthier   (501) staff       (20)      371 2024-05-19 22:05:28.000000 grep_ast-0.3.1/grep_ast.egg-info/SOURCES.txt
+-rw-r--r--   0 gauthier   (501) staff       (20)        1 2024-05-19 22:05:28.000000 grep_ast-0.3.1/grep_ast.egg-info/dependency_links.txt
+-rw-r--r--   0 gauthier   (501) staff       (20)       74 2024-05-19 22:05:28.000000 grep_ast-0.3.1/grep_ast.egg-info/entry_points.txt
+-rw-r--r--   0 gauthier   (501) staff       (20)       38 2024-05-19 22:05:28.000000 grep_ast-0.3.1/grep_ast.egg-info/requires.txt
+-rw-r--r--   0 gauthier   (501) staff       (20)        9 2024-05-19 22:05:28.000000 grep_ast-0.3.1/grep_ast.egg-info/top_level.txt
+-rw-r--r--   0 gauthier   (501) staff       (20)       38 2023-12-10 15:44:50.000000 grep_ast-0.3.1/requirements.txt
+-rw-r--r--   0 gauthier   (501) staff       (20)       38 2024-05-19 22:05:28.407813 grep_ast-0.3.1/setup.cfg
+-rw-r--r--   0 gauthier   (501) staff       (20)      765 2024-05-19 22:05:08.000000 grep_ast-0.3.1/setup.py
+drwxr-xr-x   0 gauthier   (501) staff       (20)        0 2024-05-19 22:05:28.405923 grep_ast-0.3.1/tests/
+-rw-r--r--   0 gauthier   (501) staff       (20)      247 2023-12-10 15:44:50.000000 grep_ast-0.3.1/tests/test_parsers.py
```

### Comparing `grep_ast-0.3.0/LICENSE.txt` & `grep_ast-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `grep_ast-0.3.0/PKG-INFO` & `grep_ast-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grep-ast
-Version: 0.3.0
+Version: 0.3.1
 Summary: A tool to grep through the AST of a source file
 Home-page: https://github.com/paul-gauthier/grep-ast
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: tree-sitter-languages>=1.8.0
 Requires-Dist: pathspec
```

### Comparing `grep_ast-0.3.0/README.md` & `grep_ast-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `grep_ast-0.3.0/grep_ast/dump.py` & `grep_ast-0.3.1/grep_ast/dump.py`

 * *Files identical despite different names*

### Comparing `grep_ast-0.3.0/grep_ast/grep_ast.py` & `grep_ast-0.3.1/grep_ast/grep_ast.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,16 +113,21 @@
         self.done_parent_scopes = set()
 
         self.show_lines = set(self.lines_of_interest)
 
         if self.loi_pad:
             for line in list(self.show_lines):
                 for new_line in range(line - self.loi_pad, line + self.loi_pad + 1):
-                    if self.scopes[line].intersection(self.scopes[new_line]):
-                        self.show_lines.add(new_line)
+                    if not self.scopes[line].intersection(self.scopes[new_line]):
+                        continue
+                    if new_line >= self.num_lines:
+                        continue
+                    if new_line < 0:
+                        continue
+                    self.show_lines.add(new_line)
 
         if self.last_line:
             # add the bottom line (plus parent context)
             bottom_line = self.num_lines - 2
             self.show_lines.add(bottom_line)
             self.add_parent_scopes(bottom_line)
```

### Comparing `grep_ast-0.3.0/grep_ast/main.py` & `grep_ast-0.3.1/grep_ast/main.py`

 * *Files identical despite different names*

### Comparing `grep_ast-0.3.0/grep_ast/parsers.py` & `grep_ast-0.3.1/grep_ast/parsers.py`

 * *Files identical despite different names*

### Comparing `grep_ast-0.3.0/grep_ast.egg-info/PKG-INFO` & `grep_ast-0.3.1/grep_ast.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grep-ast
-Version: 0.3.0
+Version: 0.3.1
 Summary: A tool to grep through the AST of a source file
 Home-page: https://github.com/paul-gauthier/grep-ast
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: tree-sitter-languages>=1.8.0
 Requires-Dist: pathspec
```

### Comparing `grep_ast-0.3.0/setup.py` & `grep_ast-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
     long_description = re.sub(r"\n!\[.*\]\(.*\)", "", long_description)
 
 setup(
     name="grep-ast",
-    version="0.3.0",
+    version="0.3.1",
     description="A tool to grep through the AST of a source file",
     url="https://github.com/paul-gauthier/grep-ast",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=requirements,
     entry_points={
```

