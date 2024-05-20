# Comparing `tmp/ddeutil_model-0.0.3.tar.gz` & `tmp/ddeutil_model-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddeutil_model-0.0.3.tar", last modified: Sat May 18 12:23:40 2024, max compression
+gzip compressed data, was "ddeutil_model-0.0.4.tar", last modified: Mon May 20 04:44:09 2024, max compression
```

## Comparing `ddeutil_model-0.0.3.tar` & `ddeutil_model-0.0.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:23:40.788979 ddeutil_model-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-05-18 12:23:40.784979 ddeutil_model-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 12:23:40.788979 ddeutil_model-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:23:40.780979 ddeutil_model-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:23:40.780979 ddeutil_model-0.0.3/src/ddeutil/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:23:40.784979 ddeutil_model-0.0.3/src/ddeutil/model/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/src/ddeutil/model/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/src/ddeutil/model/__base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/src/ddeutil/model/__enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/src/ddeutil/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/src/ddeutil/model/__types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/src/ddeutil/model/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/src/ddeutil/model/conn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/src/ddeutil/model/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:23:40.784979 ddeutil_model-0.0.3/src/ddeutil/model/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/src/ddeutil/model/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6119 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/src/ddeutil/model/datasets/col.py
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/src/ddeutil/model/datasets/db.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/src/ddeutil/model/datasets/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/src/ddeutil/model/dtype.py
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/src/ddeutil/model/lineage.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/src/ddeutil/model/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/src/ddeutil/model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:23:40.784979 ddeutil_model-0.0.3/src/ddeutil_model.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-05-18 12:23:40.000000 ddeutil_model-0.0.3/src/ddeutil_model.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-18 12:23:40.000000 ddeutil_model-0.0.3/src/ddeutil_model.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 12:23:40.000000 ddeutil_model-0.0.3/src/ddeutil_model.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-18 12:23:40.000000 ddeutil_model-0.0.3/src/ddeutil_model.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-18 12:23:40.000000 ddeutil_model-0.0.3/src/ddeutil_model.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:23:40.784979 ddeutil_model-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/tests/test_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/tests/test_conn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/tests/test_const.py
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/tests/test_dataset_column.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/tests/test_dataset_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/tests/test_dataset_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/tests/test_dtype.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/tests/test_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/tests/test_lineage.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/tests/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:44:09.082885 ddeutil_model-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-20 04:44:04.000000 ddeutil_model-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-20 04:44:09.082885 ddeutil_model-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-20 04:44:04.000000 ddeutil_model-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-05-20 04:44:04.000000 ddeutil_model-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 04:44:09.082885 ddeutil_model-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:44:09.074885 ddeutil_model-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:44:09.074885 ddeutil_model-0.0.4/src/ddeutil/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:44:09.078884 ddeutil_model-0.0.4/src/ddeutil/model/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-20 04:44:04.000000 ddeutil_model-0.0.4/src/ddeutil/model/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-05-20 04:44:04.000000 ddeutil_model-0.0.4/src/ddeutil/model/__base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-20 04:44:04.000000 ddeutil_model-0.0.4/src/ddeutil/model/__enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-20 04:44:04.000000 ddeutil_model-0.0.4/src/ddeutil/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-20 04:44:04.000000 ddeutil_model-0.0.4/src/ddeutil/model/__types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-20 04:44:04.000000 ddeutil_model-0.0.4/src/ddeutil/model/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-05-20 04:44:04.000000 ddeutil_model-0.0.4/src/ddeutil/model/conn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-20 04:44:04.000000 ddeutil_model-0.0.4/src/ddeutil/model/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:44:09.078884 ddeutil_model-0.0.4/src/ddeutil/model/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-20 04:44:04.000000 ddeutil_model-0.0.4/src/ddeutil/model/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6119 2024-05-20 04:44:04.000000 ddeutil_model-0.0.4/src/ddeutil/model/datasets/col.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-05-20 04:44:04.000000 ddeutil_model-0.0.4/src/ddeutil/model/datasets/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-20 04:44:04.000000 ddeutil_model-0.0.4/src/ddeutil/model/datasets/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-05-20 04:44:04.000000 ddeutil_model-0.0.4/src/ddeutil/model/dtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-20 04:44:04.000000 ddeutil_model-0.0.4/src/ddeutil/model/lineage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-20 04:44:04.000000 ddeutil_model-0.0.4/src/ddeutil/model/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-20 04:44:04.000000 ddeutil_model-0.0.4/src/ddeutil/model/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:44:09.082885 ddeutil_model-0.0.4/src/ddeutil_model.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-20 04:44:09.000000 ddeutil_model-0.0.4/src/ddeutil_model.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-20 04:44:09.000000 ddeutil_model-0.0.4/src/ddeutil_model.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 04:44:09.000000 ddeutil_model-0.0.4/src/ddeutil_model.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-20 04:44:09.000000 ddeutil_model-0.0.4/src/ddeutil_model.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-20 04:44:09.000000 ddeutil_model-0.0.4/src/ddeutil_model.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:44:09.082885 ddeutil_model-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-20 04:44:04.000000 ddeutil_model-0.0.4/tests/test_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-20 04:44:04.000000 ddeutil_model-0.0.4/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-20 04:44:04.000000 ddeutil_model-0.0.4/tests/test_conn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-20 04:44:04.000000 ddeutil_model-0.0.4/tests/test_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-05-20 04:44:04.000000 ddeutil_model-0.0.4/tests/test_dataset_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-20 04:44:04.000000 ddeutil_model-0.0.4/tests/test_dataset_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-05-20 04:44:04.000000 ddeutil_model-0.0.4/tests/test_dataset_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-20 04:44:04.000000 ddeutil_model-0.0.4/tests/test_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-20 04:44:04.000000 ddeutil_model-0.0.4/tests/test_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-20 04:44:04.000000 ddeutil_model-0.0.4/tests/test_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-20 04:44:04.000000 ddeutil_model-0.0.4/tests/test_types.py
```

### Comparing `ddeutil_model-0.0.3/LICENSE` & `ddeutil_model-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ddeutil_model-0.0.3/PKG-INFO` & `ddeutil_model-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddeutil-model
-Version: 0.0.3
+Version: 0.0.4
 Summary: Data Developer & Engineer Model Utility Objects
 Author-email: ddeutils <korawich.anu@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/ddeutils/ddeutil-model/
 Project-URL: Source Code, https://github.com/ddeutils/ddeutil-model/
 Keywords: data,model,utility,pipeline
 Classifier: Topic :: Utilities
@@ -36,16 +36,21 @@
 - [Installation](#installation)
 - [Models](#models)
   - [Data Types](#data-types)
   - [Constraints](#constraints)
   - [Datasets](#datasets)
 - [Usecase](#usecase)
 
-This is **Model Utility**, implements any model objects for **Data Pipeline**
-or **Data Platform**. The Model objects was implemented from the [Pydantic V2](https://docs.pydantic.dev/latest/).
+This is **Utility Models**, it implements any models for **Data Pipeline**,
+or **Data Platform** frameworks. The Model objects was implemented from the [Pydantic V2](https://docs.pydantic.dev/latest/)
+which is the powerful parsing and serializing data model to the Python object.
+
+> [!NOTE]
+> So, I use this project to learn and implement a limit and trick of the Pydantic
+> package.
 
 The model able to handle common logic validations and able to adjust by custom code
 for your specific requirements (Yeah, it just inherits Sub-Class from `BaseModel`).
 
 ## Installation
 
 ```shell
```

### Comparing `ddeutil_model-0.0.3/README.md` & `ddeutil_model-0.0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -9,16 +9,21 @@
 - [Installation](#installation)
 - [Models](#models)
   - [Data Types](#data-types)
   - [Constraints](#constraints)
   - [Datasets](#datasets)
 - [Usecase](#usecase)
 
-This is **Model Utility**, implements any model objects for **Data Pipeline**
-or **Data Platform**. The Model objects was implemented from the [Pydantic V2](https://docs.pydantic.dev/latest/).
+This is **Utility Models**, it implements any models for **Data Pipeline**,
+or **Data Platform** frameworks. The Model objects was implemented from the [Pydantic V2](https://docs.pydantic.dev/latest/)
+which is the powerful parsing and serializing data model to the Python object.
+
+> [!NOTE]
+> So, I use this project to learn and implement a limit and trick of the Pydantic
+> package.
 
 The model able to handle common logic validations and able to adjust by custom code
 for your specific requirements (Yeah, it just inherits Sub-Class from `BaseModel`).
 
 ## Installation
 
 ```shell
```

### Comparing `ddeutil_model-0.0.3/pyproject.toml` & `ddeutil_model-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ddeutil_model-0.0.3/src/ddeutil/model/__enums.py` & `ddeutil_model-0.0.4/src/ddeutil/model/__enums.py`

 * *Files identical despite different names*

### Comparing `ddeutil_model-0.0.3/src/ddeutil/model/__types.py` & `ddeutil_model-0.0.4/src/ddeutil/model/__types.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     Url,
     UrlConstraints(
         host_required=True,
         default_port=1234,
     ),
 ]
 
-FileUrl = Annotated[
+LocalUrl = Annotated[
     Url,
     UrlConstraints(
         default_host="127.0.0.1",
         default_port=None,
     ),
 ]
```

### Comparing `ddeutil_model-0.0.3/src/ddeutil/model/action.py` & `ddeutil_model-0.0.4/src/ddeutil/model/action.py`

 * *Files identical despite different names*

### Comparing `ddeutil_model-0.0.3/src/ddeutil/model/conn.py` & `ddeutil_model-0.0.4/src/ddeutil/model/conn.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from pydantic import Field
 from pydantic.functional_validators import field_validator
 from pydantic.types import SecretStr
 from pydantic_core import Url
 
 from .__base import BaseUpdatableModel
-from .__types import CustomUrl, FileUrl
+from .__types import CustomUrl
 from .utils import unquote_str
 
 
 class BaseConn(BaseUpdatableModel):
     type: str = "base"
 
 
@@ -38,45 +38,41 @@
     options: Annotated[dict[str, Any], Field(default_factory=dict)]
 
     @classmethod
     def from_url(cls, url: Union[Url, str]) -> Conn:
         if isinstance(url, str):
             url = Url(url=url)
         elif not isinstance(url, Url):
-            raise ValueError("A url value must be string or `CustomUrl` object")
+            raise ValueError("A url value must be string or `Url` object")
         return cls(
             dialect=url.scheme,
             host=unquote_str(url.host),
             port=url.port,
             user=unquote_str(url.username),
             pwd=unquote_str(url.password),
             endpoint=url.path,
             options=dict(url.query_params()),
         )
 
-    @field_validator("endpoint")
-    def __check_endpoint_name(cls, v: str) -> str:
-        return v.lstrip("/")
-
 
 class FlConn(BaseConn):
     type: Literal["file"] = "file"
     sys: str
     pointer: Optional[str] = None
     port: Optional[int] = None
     user: Optional[str] = None
     pwd: Optional[SecretStr] = None
     path: str
     options: Annotated[dict[str, Any], Field(default_factory=dict)]
 
     @classmethod
-    def from_url(cls, url: Union[FileUrl, str]) -> FlConn:
+    def from_url(cls, url: Union[Url, str]) -> FlConn:
         if isinstance(url, str):
-            url = FileUrl(url=url)
-        elif not isinstance(url, FileUrl):
+            url = Url(url=url)
+        elif not isinstance(url, Url):
             raise ValueError("A url value must be string or `FileUrl` object")
         return cls(
             sys=url.scheme,
             pointer=unquote_str(url.password),
             port=url.port,
             user=unquote_str(url.username),
             pwd=unquote_str(url.password),
@@ -117,9 +113,19 @@
             user=unquote_str(url.username),
             pwd=unquote_str(url.password),
             db=url.path,
             options=dict(url.query_params()),
         )
 
     @field_validator("db")
-    def __check_db_name(cls, v: str) -> str:
-        return v.lstrip("/").split("/")[0]
+    def _remove_slash_on_db(cls, v: str) -> str:
+        v: str = v[1:] if v.startswith("/") else v
+        return v.split("/")[0]
+
+
+# @remove_validators('_check_db_name')
+class DbWithSlashConn(DbConn):
+    """"""
+
+    @field_validator("db")
+    def _remove_slash_on_db(cls, v: str) -> str:
+        return v
```

### Comparing `ddeutil_model-0.0.3/src/ddeutil/model/const.py` & `ddeutil_model-0.0.4/src/ddeutil/model/const.py`

 * *Files identical despite different names*

### Comparing `ddeutil_model-0.0.3/src/ddeutil/model/datasets/col.py` & `ddeutil_model-0.0.4/src/ddeutil/model/datasets/col.py`

 * *Files identical despite different names*

### Comparing `ddeutil_model-0.0.3/src/ddeutil/model/datasets/db.py` & `ddeutil_model-0.0.4/src/ddeutil/model/datasets/db.py`

 * *Files identical despite different names*

### Comparing `ddeutil_model-0.0.3/src/ddeutil/model/datasets/file.py` & `ddeutil_model-0.0.4/src/ddeutil/model/datasets/file.py`

 * *Files identical despite different names*

### Comparing `ddeutil_model-0.0.3/src/ddeutil/model/dtype.py` & `ddeutil_model-0.0.4/src/ddeutil/model/dtype.py`

 * *Files identical despite different names*

### Comparing `ddeutil_model-0.0.3/src/ddeutil/model/lineage.py` & `ddeutil_model-0.0.4/src/ddeutil/model/lineage.py`

 * *Files identical despite different names*

### Comparing `ddeutil_model-0.0.3/src/ddeutil/model/utils.py` & `ddeutil_model-0.0.4/src/ddeutil/model/utils.py`

 * *Files identical despite different names*

### Comparing `ddeutil_model-0.0.3/src/ddeutil_model.egg-info/PKG-INFO` & `ddeutil_model-0.0.4/src/ddeutil_model.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddeutil-model
-Version: 0.0.3
+Version: 0.0.4
 Summary: Data Developer & Engineer Model Utility Objects
 Author-email: ddeutils <korawich.anu@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/ddeutils/ddeutil-model/
 Project-URL: Source Code, https://github.com/ddeutils/ddeutil-model/
 Keywords: data,model,utility,pipeline
 Classifier: Topic :: Utilities
@@ -36,16 +36,21 @@
 - [Installation](#installation)
 - [Models](#models)
   - [Data Types](#data-types)
   - [Constraints](#constraints)
   - [Datasets](#datasets)
 - [Usecase](#usecase)
 
-This is **Model Utility**, implements any model objects for **Data Pipeline**
-or **Data Platform**. The Model objects was implemented from the [Pydantic V2](https://docs.pydantic.dev/latest/).
+This is **Utility Models**, it implements any models for **Data Pipeline**,
+or **Data Platform** frameworks. The Model objects was implemented from the [Pydantic V2](https://docs.pydantic.dev/latest/)
+which is the powerful parsing and serializing data model to the Python object.
+
+> [!NOTE]
+> So, I use this project to learn and implement a limit and trick of the Pydantic
+> package.
 
 The model able to handle common logic validations and able to adjust by custom code
 for your specific requirements (Yeah, it just inherits Sub-Class from `BaseModel`).
 
 ## Installation
 
 ```shell
```

### Comparing `ddeutil_model-0.0.3/src/ddeutil_model.egg-info/SOURCES.txt` & `ddeutil_model-0.0.4/src/ddeutil_model.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ddeutil_model-0.0.3/tests/test_action.py` & `ddeutil_model-0.0.4/tests/test_action.py`

 * *Files identical despite different names*

### Comparing `ddeutil_model-0.0.3/tests/test_base.py` & `ddeutil_model-0.0.4/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `ddeutil_model-0.0.3/tests/test_conn.py` & `ddeutil_model-0.0.4/tests/test_conn.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,34 +6,34 @@
         url=(
             "postgres+psycopg://demo:P%40ssw0rd@localhost/postgres"
             "?echo=True&timeout=10"
         )
     )
     assert t.port is None
     assert "postgres+psycopg" == t.dialect
-    assert "postgres" == t.endpoint
+    assert "/postgres" == t.endpoint
     assert "demo" == t.user
     assert "P@ssw0rd" == t.pwd.get_secret_value()
     assert "localhost" == t.host
 
     t = conn.Conn.from_url(url="sqlite:///foo.db")
 
     assert t.port is None
     assert t.user is None
     assert t.pwd is None
     assert t.host is None
-    assert "foo.db" == t.endpoint
+    assert "/foo.db" == t.endpoint
 
     t = conn.Conn.from_url(url="sqlite:////absolute/path/to/foo.db")
 
-    assert "absolute/path/to/foo.db" == t.endpoint
+    assert "//absolute/path/to/foo.db" == t.endpoint
 
     t = conn.Conn.from_url(url=r"sqlite:///C:\path\to\foo.db")
 
-    assert "C:\\path\\to\\foo.db" == t.endpoint
+    assert "/C:\\path\\to\\foo.db" == t.endpoint
 
 
 def test_db_conn_from_url():
     t = conn.DbConn.from_url(
         url=(
             "postgres+psycopg://demo:P%40ssw0rd@localhost:5432/db"
             "?echo=True&timeout=10"
@@ -60,20 +60,45 @@
             "db": "sales",
         }
     )
     assert "postgres" == t.driver
     assert "P@ssw0rd" == t.pwd.get_secret_value()
 
 
+def test_db_with_slash_conn():
+    t = conn.DbWithSlashConn(
+        **{
+            "driver": "postgres",
+            "host": "127.0.0.1",
+            "port": "5432",
+            "user": "postgres",
+            "pwd": "P@ssw0rd",
+            "db": "/sales",
+        }
+    )
+    assert "postgres" == t.driver
+    assert "P@ssw0rd" == t.pwd.get_secret_value()
+    assert "/sales" == t.db
+
+
 def test_fl_conn_from_url():
     t = conn.FlConn.from_url(
-        url="sqlite:///D:/data/warehouse/main.sqlite?echo=True"
+        url="sqlite:///data/warehouse/main.sqlite?echo=True"
+    )
+    assert "sqlite" == t.sys
+    assert "/data/warehouse/main.sqlite" == t.path
+    assert {"echo": "True"} == t.options
+
+
+def test_fl_conn_from_absolute_url():
+    t = conn.FlConn.from_url(
+        url="sqlite:////D:/data/warehouse/main.sqlite?echo=True"
     )
     assert "sqlite" == t.sys
-    assert "/D:/data/warehouse/main.sqlite" == t.path
+    assert "//D:/data/warehouse/main.sqlite" == t.path
     assert {"echo": "True"} == t.options
 
 
 def test_fl_conn():
     t = conn.FlConn(
         **{
             "sys": "file",
```

### Comparing `ddeutil_model-0.0.3/tests/test_const.py` & `ddeutil_model-0.0.4/tests/test_const.py`

 * *Files identical despite different names*

### Comparing `ddeutil_model-0.0.3/tests/test_dataset_column.py` & `ddeutil_model-0.0.4/tests/test_dataset_column.py`

 * *Files identical despite different names*

### Comparing `ddeutil_model-0.0.3/tests/test_dataset_schema.py` & `ddeutil_model-0.0.4/tests/test_dataset_schema.py`

 * *Files identical despite different names*

### Comparing `ddeutil_model-0.0.3/tests/test_dataset_table.py` & `ddeutil_model-0.0.4/tests/test_dataset_table.py`

 * *Files identical despite different names*

### Comparing `ddeutil_model-0.0.3/tests/test_dtype.py` & `ddeutil_model-0.0.4/tests/test_dtype.py`

 * *Files identical despite different names*

### Comparing `ddeutil_model-0.0.3/tests/test_lineage.py` & `ddeutil_model-0.0.4/tests/test_lineage.py`

 * *Files identical despite different names*

