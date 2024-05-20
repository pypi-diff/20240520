# Comparing `tmp/enchante-0.1.0.tar.gz` & `tmp/enchante-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enchante-0.1.0.tar", max compression
+gzip compressed data, was "enchante-0.1.1.tar", max compression
```

## Comparing `enchante-0.1.0.tar` & `enchante-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1065 2023-07-28 04:07:22.481576 enchante-0.1.0/LICENSE
--rw-r--r--   0        0        0     1284 2024-05-15 16:52:02.490446 enchante-0.1.0/README.md
--rw-r--r--   0        0        0      588 2024-05-15 16:10:41.472817 enchante-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-28 05:22:58.672964 enchante-0.1.0/src/enchante/__init__.py
--rw-r--r--   0        0        0       60 2023-08-09 17:31:33.464907 enchante-0.1.0/src/enchante/__main__.py
--rw-r--r--   0        0        0     1703 2024-05-15 16:43:56.822682 enchante-0.1.0/src/enchante/main.py
--rw-r--r--   0        0        0       23 2023-05-30 08:32:53.162623 enchante-0.1.0/src/enchante/templates/table/__init__.py
--rw-r--r--   0        0        0      460 2024-05-15 15:33:09.063245 enchante-0.1.0/src/enchante/templates/table/crud.py.jinja
--rw-r--r--   0        0        0      547 2024-05-15 16:44:47.198089 enchante-0.1.0/src/enchante/templates/table/model.py.jinja
--rw-r--r--   0        0        0      222 2024-05-15 15:32:46.321803 enchante-0.1.0/src/enchante/templates/table/schema.py.jinja
--rw-r--r--   0        0        0       46 2024-05-15 12:25:49.515202 enchante-0.1.0/src/enchante/utils/__init__.py
--rw-r--r--   0        0        0      232 2024-05-15 10:43:51.273324 enchante-0.1.0/src/enchante/utils/base.py
--rw-r--r--   0        0        0     6868 2024-05-20 06:16:54.641795 enchante-0.1.0/src/enchante/utils/crud.py
--rw-r--r--   0        0        0      141 2024-05-15 15:49:37.705454 enchante-0.1.0/src/enchante/utils/types.py
--rw-r--r--   0        0        0     1981 1970-01-01 00:00:00.000000 enchante-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-28 04:07:22.481576 enchante-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1260 2024-05-20 06:44:55.449904 enchante-0.1.1/README.md
+-rw-r--r--   0        0        0      587 2024-05-20 06:44:55.451964 enchante-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-28 05:22:58.672964 enchante-0.1.1/src/enchante/__init__.py
+-rw-r--r--   0        0        0       60 2023-08-09 17:31:33.464907 enchante-0.1.1/src/enchante/__main__.py
+-rw-r--r--   0        0        0     1703 2024-05-15 16:43:56.822682 enchante-0.1.1/src/enchante/main.py
+-rw-r--r--   0        0        0       23 2023-05-30 08:32:53.162623 enchante-0.1.1/src/enchante/templates/table/__init__.py
+-rw-r--r--   0        0        0      460 2024-05-15 15:33:09.063245 enchante-0.1.1/src/enchante/templates/table/crud.py.jinja
+-rw-r--r--   0        0        0      547 2024-05-15 16:44:47.198089 enchante-0.1.1/src/enchante/templates/table/model.py.jinja
+-rw-r--r--   0        0        0      222 2024-05-15 15:32:46.321803 enchante-0.1.1/src/enchante/templates/table/schema.py.jinja
+-rw-r--r--   0        0        0       46 2024-05-15 12:25:49.515202 enchante-0.1.1/src/enchante/utils/__init__.py
+-rw-r--r--   0        0        0      232 2024-05-15 10:43:51.273324 enchante-0.1.1/src/enchante/utils/base.py
+-rw-r--r--   0        0        0     6868 2024-05-20 06:16:54.641795 enchante-0.1.1/src/enchante/utils/crud.py
+-rw-r--r--   0        0        0      141 2024-05-15 15:49:37.705454 enchante-0.1.1/src/enchante/utils/types.py
+-rw-r--r--   0        0        0     2041 1970-01-01 00:00:00.000000 enchante-0.1.1/PKG-INFO
```

### Comparing `enchante-0.1.0/LICENSE` & `enchante-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `enchante-0.1.0/README.md` & `enchante-0.1.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -24,16 +24,20 @@
 <details>
   <summary>
     Why not <a href="https://sqlmodel.tiangolo.com/">SQLModel</a> instead of
     Pydantic + SQLALchemy?
   </summary>
   SQLModel still has a long way to go
   <a href="https://github.com/tiangolo/sqlmodel/issues/654">
-    with their current roadmap
-  </a>, but they're making good progress!
+    with their current roadmap </a
+  >, but they're making good progress!
 </details>
-## How to use 1. First run `enchante init
-<root_dir
-  >` 2. Now you can run `enchante create <object_name>` </object_name></root_dir
->
-## Development ---
+
+
+## How to use
+1. First run `enchante init <root_dir>`
+2. Now you can run `enchante create <object_name>`
+
+## Development 
+
+---
 License: [MIT](https://github.com/StevenJPx2/enchante/blob/main/LICENSE)
```

### Comparing `enchante-0.1.0/pyproject.toml` & `enchante-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "enchante"
-version = "0.1.0"
+version = "0.1.1"
 description = "CLI tool to help scaffolding relational DB architecture as code"
 authors = ["Steven John <steven@stevenjohn.co>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "enchante", from = "src" }]
 
 [tool.poetry.dependencies]
-python = "^3.12"
+python = ">=3.10"
 pydantic = "^2.1.1"
-SQLAlchemy = "^2.0.19"
+SQLAlchemy = "^2.0"
 alembic = "^1.11.1"
-typer = "^0.9.0"
+typer = ">=0.9.0"
 pyyaml = "^6.0.1"
 jinja2 = "^3.1.4"
 pyhumps = "^3.8.0"
 
 [tool.poetry.scripts]
 enchante = "enchante.main:app"
```

### Comparing `enchante-0.1.0/src/enchante/main.py` & `enchante-0.1.1/src/enchante/main.py`

 * *Files identical despite different names*

### Comparing `enchante-0.1.0/src/enchante/templates/table/model.py.jinja` & `enchante-0.1.1/src/enchante/templates/table/model.py.jinja`

 * *Files identical despite different names*

### Comparing `enchante-0.1.0/src/enchante/utils/crud.py` & `enchante-0.1.1/src/enchante/utils/crud.py`

 * *Files identical despite different names*

### Comparing `enchante-0.1.0/PKG-INFO` & `enchante-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: enchante
-Version: 0.1.0
+Version: 0.1.1
 Summary: CLI tool to help scaffolding relational DB architecture as code
 License: MIT
 Author: Steven John
 Author-email: steven@stevenjohn.co
-Requires-Python: >=3.12,<4.0
+Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: SQLAlchemy (>=2.0.19,<3.0.0)
+Requires-Dist: SQLAlchemy (>=2.0,<3.0)
 Requires-Dist: alembic (>=1.11.1,<2.0.0)
 Requires-Dist: jinja2 (>=3.1.4,<4.0.0)
 Requires-Dist: pydantic (>=2.1.1,<3.0.0)
 Requires-Dist: pyhumps (>=3.8.0,<4.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
-Requires-Dist: typer (>=0.9.0,<0.10.0)
+Requires-Dist: typer (>=0.9.0)
 Description-Content-Type: text/markdown
 
 # enchante
 Simplify your DB management
 
 ---
 ## Motivation
@@ -44,17 +46,21 @@
 <details>
   <summary>
     Why not <a href="https://sqlmodel.tiangolo.com/">SQLModel</a> instead of
     Pydantic + SQLALchemy?
   </summary>
   SQLModel still has a long way to go
   <a href="https://github.com/tiangolo/sqlmodel/issues/654">
-    with their current roadmap
-  </a>, but they're making good progress!
+    with their current roadmap </a
+  >, but they're making good progress!
 </details>
-## How to use 1. First run `enchante init
-<root_dir
-  >` 2. Now you can run `enchante create <object_name>` </object_name></root_dir
->
-## Development ---
+
+
+## How to use
+1. First run `enchante init <root_dir>`
+2. Now you can run `enchante create <object_name>`
+
+## Development 
+
+---
 License: [MIT](https://github.com/StevenJPx2/enchante/blob/main/LICENSE)
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
-Metadata-Version: 2.1 Name: enchante Version: 0.1.0 Summary: CLI tool to help
+Metadata-Version: 2.1 Name: enchante Version: 0.1.1 Summary: CLI tool to help
 scaffolding relational DB architecture as code License: MIT Author: Steven John
-Author-email: steven@stevenjohn.co Requires-Python: >=3.12,<4.0 Classifier:
-License :: OSI Approved :: MIT License Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.12 Requires-Dist:
-SQLAlchemy (>=2.0.19,<3.0.0) Requires-Dist: alembic (>=1.11.1,<2.0.0) Requires-
-Dist: jinja2 (>=3.1.4,<4.0.0) Requires-Dist: pydantic (>=2.1.1,<3.0.0)
+Author-email: steven@stevenjohn.co Requires-Python: >=3.10 Classifier: License
+:: OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: SQLAlchemy (>=2.0,<3.0) Requires-Dist: alembic (>=1.11.1,<2.0.0)
+Requires-Dist: jinja2 (>=3.1.4,<4.0.0) Requires-Dist: pydantic (>=2.1.1,<3.0.0)
 Requires-Dist: pyhumps (>=3.8.0,<4.0.0) Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
-Requires-Dist: typer (>=0.9.0,<0.10.0) Description-Content-Type: text/markdown
-# enchante Simplify your DB management --- ## Motivation Imagine you're
-creating an API that connects to your SQL DB via SQLAlchemy. One of the biggest
-pain points is to create a structure that makes logical sense along with being
-easy to scale (as in add more tables easily). Well, that's where `enchante`
-comes in! Using the power of Pydantic, SQLAlchemy and Alembic, it'll be much
-easier to initialise and make changes to your database. This CLI helps with
-creating and scaffolding the structure of your db architecture as python code.
-### Folder structure ``` db/ ââ migrations/ ââ [table_name]/ â ââ
+Requires-Dist: typer (>=0.9.0) Description-Content-Type: text/markdown #
+enchante Simplify your DB management --- ## Motivation Imagine you're creating
+an API that connects to your SQL DB via SQLAlchemy. One of the biggest pain
+points is to create a structure that makes logical sense along with being easy
+to scale (as in add more tables easily). Well, that's where `enchante` comes
+in! Using the power of Pydantic, SQLAlchemy and Alembic, it'll be much easier
+to initialise and make changes to your database. This CLI helps with creating
+and scaffolding the structure of your db architecture as python code. ###
+Folder structure ``` db/ ââ migrations/ ââ [table_name]/ â ââ
 __init__.py â ââ crud.py â ââ model.py â ââ schema.py
 enchante.toml ``` ## Why not `...`? Why not _S_Q_L_M_o_d_e_l instead of Pydantic +
 SQLALchemy? SQLModel still has a long way to go _w_i_t_h_ _t_h_e_i_r_ _c_u_r_r_e_n_t_ _r_o_a_d_m_a_p_ ,
 but they're making good progress! ## How to use 1. First run `enchante init `
 2. Now you can run `enchante create ` ## Development --- License: [MIT](https:/
 /github.com/StevenJPx2/enchante/blob/main/LICENSE)
```

