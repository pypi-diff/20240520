# Comparing `tmp/sbsv-0.0.1.tar.gz` & `tmp/sbsv-0.0.2.tar.gz`

## Comparing `sbsv-0.0.1.tar` & `sbsv-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,11 @@
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 sbsv-0.0.1/sbsv/__init__.py
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 sbsv-0.0.1/sbsv/sbsv.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 sbsv-0.0.1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 sbsv-0.0.1/LICENSE
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 sbsv-0.0.1/README.md
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 sbsv-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 sbsv-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 sbsv-0.0.2/sbsv/__init__.py
+-rw-r--r--   0        0        0     7336 2020-02-02 00:00:00.000000 sbsv-0.0.2/sbsv/sbsv.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sbsv-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 sbsv-0.0.2/tests/test_schema.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 sbsv-0.0.2/tests/resources/test_schema.sbsv
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 sbsv-0.0.2/tests/resources/test_schema_sub.sbsv
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 sbsv-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 sbsv-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 sbsv-0.0.2/README.md
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 sbsv-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 sbsv-0.0.2/PKG-INFO
```

### Comparing `sbsv-0.0.1/LICENSE` & `sbsv-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sbsv-0.0.1/pyproject.toml` & `sbsv-0.0.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sbsv"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Seungheon Han", email="shhan814@gmail.com" },
 ]
 description = "SBSV: Square Brackets Separated Values"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 Homepage = "https://github.com/hsh814/sbsv"
-Issues = "https://github.com/hsh814/sbsv/issues"
+Issues = "https://github.com/hsh814/sbsv/issues"
+
+[tool.black]
+line-length = 88
+target-version = ['py38']
+include = '\.pyi?$'
```

### Comparing `sbsv-0.0.1/PKG-INFO` & `sbsv-0.0.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,28 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: sbsv
-Version: 0.0.1
+Version: 0.0.2
 Summary: SBSV: Square Brackets Separated Values
 Project-URL: Homepage, https://github.com/hsh814/sbsv
 Project-URL: Issues, https://github.com/hsh814/sbsv/issues
 Author-email: Seungheon Han <shhan814@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # SBSV: square bracket separated values
+A flexible, schema-based structured log data format.
 
 ## Install
 
 ```shell
-python3 -m pip install svsb
+python3 -m pip install sbsv
 ```
 
 ## Use
 You can read this log-like data:
 ```sbsv
 [meta-data] [id 1] [format string]
 [meta-data] [id 2] [format token]
@@ -70,22 +71,83 @@
 But if you add sub schema, you cannot add new schema with same schema name without sub schema.
 ```
 [my-schema] [no: int] [sub: str] [schema: str]
 # this will cause error
 ```
 
 ### Ignore
+- [ ] Not available yet
 ```
 [2024-03-04 13:22:56] [DEBUG] [necessary] [from] [this part]
 ```
 Regular log file may contain unnecessary data. You can specify parser to ignore `[2024-03-04 13:22:56] [DEBUG]` part.
 
 ```python
 parser.add_schema("[$ignore] [$ignore] [necessary] [from] [this: str]")
 ```
 
+### Duplicating names
+- [ ] Not available yet
+Sometimes, you may want to use same name multiple times.
+```
+[my-schema] [node 1] [node 2] [node 3]
+```
+You can distinguish them using index.
+```python
+parser.add_schema("[my-schema] [node$0: int] [node$1: int] [node$2: int]")
+```
+
 ### Primitive types
 Primitive types are `str`, `int`, `float`, `bool`, `null`.
 
 ### Complex types
-You can use `list`.
+- [ ] Not available yet
+#### list
+```
+[data] [token] [id 2] [actual [some] [multiple] [tokens]]
+```
+
+```python
+parser.add_schema("[data] [token] [id: int] [actual: list[str]]")
+```
+
+#### obj
+```
+[car] [id 1] [data [speed 100] [power 2] [price 20000]]
+```
+```python
+parser.add_schema("[car] [id: int] [data: obj[speed: int, power: int, price: int]])
+```
+
+#### map
+```
+[map-example] [mymap [id: 1, name: alice, email: wd@email.com]]
+```
+```python
+parser.add_schema("[map-example] [mymap: map]")
+```
+
+#### nullable
+```
+[car] [id 1] [data [speed 100] [power 2] [price]]
+[car] [id] [data [speed 120] [power 3] [price 33000]]
+```
+
+```python
+parser.add_schema("[car] [id?: int] [data: obj[speed: int, power: int, price?: int]]")
+```
+
 
+## Contribute
+```shell
+python3 -m pip install --upgrade pip
+python3 -m pip install black
+```
+You should run `black` linter before commit.
+```shell
+python3 -m black .
+```
+
+Before implementing new features or fixing bugs, add new tests in `tests/`.
+```shell
+python3 -m unittest
+```
```

