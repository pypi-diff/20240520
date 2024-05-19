# Comparing `tmp/async_bakalari_api-0.3.tar.gz` & `tmp/async_bakalari_api-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_bakalari_api-0.3.tar", last modified: Sat May 18 15:17:48 2024, max compression
+gzip compressed data, was "async_bakalari_api-0.3.1.tar", last modified: Sun May 19 22:57:57 2024, max compression
```

## Comparing `async_bakalari_api-0.3.tar` & `async_bakalari_api-0.3.1.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:17:48.688350 async_bakalari_api-0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-18 15:17:43.000000 async_bakalari_api-0.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    16070 2024-05-18 15:17:48.688350 async_bakalari_api-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-18 15:17:43.000000 async_bakalari_api-0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7787 2024-05-18 15:17:43.000000 async_bakalari_api-0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 15:17:48.688350 async_bakalari_api-0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:17:48.684350 async_bakalari_api-0.3/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 15:17:43.000000 async_bakalari_api-0.3/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:17:48.688350 async_bakalari_api-0.3/src/async_bakalari_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16070 2024-05-18 15:17:48.000000 async_bakalari_api-0.3/src/async_bakalari_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-18 15:17:48.000000 async_bakalari_api-0.3/src/async_bakalari_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 15:17:48.000000 async_bakalari_api-0.3/src/async_bakalari_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-18 15:17:48.000000 async_bakalari_api-0.3/src/async_bakalari_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 15:17:48.000000 async_bakalari_api-0.3/src/async_bakalari_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-18 15:17:48.000000 async_bakalari_api-0.3/src/async_bakalari_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:17:48.688350 async_bakalari_api-0.3/src/bakalari_api/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-18 15:17:43.000000 async_bakalari_api-0.3/src/bakalari_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-18 15:17:43.000000 async_bakalari_api-0.3/src/bakalari_api/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14669 2024-05-18 15:17:43.000000 async_bakalari_api-0.3/src/bakalari_api/bakalari.py
--rw-r--r--   0 runner    (1001) docker     (127)     8670 2024-05-18 15:17:43.000000 async_bakalari_api-0.3/src/bakalari_api/bakalari_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-18 15:17:43.000000 async_bakalari_api-0.3/src/bakalari_api/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-05-18 15:17:43.000000 async_bakalari_api-0.3/src/bakalari_api/datastructure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-18 15:17:43.000000 async_bakalari_api-0.3/src/bakalari_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-18 15:17:43.000000 async_bakalari_api-0.3/src/bakalari_api/first_login.py
--rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-05-18 15:17:43.000000 async_bakalari_api-0.3/src/bakalari_api/komens.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-18 15:17:43.000000 async_bakalari_api-0.3/src/bakalari_api/logger_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:17:48.688350 async_bakalari_api-0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    19347 2024-05-18 15:17:43.000000 async_bakalari_api-0.3/tests/test_bakalari.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-18 15:17:43.000000 async_bakalari_api-0.3/tests/test_const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-05-18 15:17:43.000000 async_bakalari_api-0.3/tests/test_datastructure.py
--rw-r--r--   0 runner    (1001) docker     (127)     6279 2024-05-18 15:17:43.000000 async_bakalari_api-0.3/tests/test_komens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:57:57.291777 async_bakalari_api-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-19 22:57:52.000000 async_bakalari_api-0.3.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16439 2024-05-19 22:57:57.291777 async_bakalari_api-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-19 22:57:52.000000 async_bakalari_api-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7790 2024-05-19 22:57:52.000000 async_bakalari_api-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-19 22:57:52.000000 async_bakalari_api-0.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 22:57:57.291777 async_bakalari_api-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:57:57.287777 async_bakalari_api-0.3.1/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 22:57:52.000000 async_bakalari_api-0.3.1/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:57:57.287777 async_bakalari_api-0.3.1/src/async_bakalari_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16439 2024-05-19 22:57:57.000000 async_bakalari_api-0.3.1/src/async_bakalari_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-19 22:57:57.000000 async_bakalari_api-0.3.1/src/async_bakalari_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 22:57:57.000000 async_bakalari_api-0.3.1/src/async_bakalari_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-19 22:57:57.000000 async_bakalari_api-0.3.1/src/async_bakalari_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 22:57:57.000000 async_bakalari_api-0.3.1/src/async_bakalari_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-19 22:57:57.000000 async_bakalari_api-0.3.1/src/async_bakalari_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-19 22:57:57.000000 async_bakalari_api-0.3.1/src/async_bakalari_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:57:57.287777 async_bakalari_api-0.3.1/src/bakalari_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-19 22:57:52.000000 async_bakalari_api-0.3.1/src/bakalari_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-19 22:57:52.000000 async_bakalari_api-0.3.1/src/bakalari_api/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14669 2024-05-19 22:57:52.000000 async_bakalari_api-0.3.1/src/bakalari_api/bakalari.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8670 2024-05-19 22:57:52.000000 async_bakalari_api-0.3.1/src/bakalari_api/bakalari_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-19 22:57:52.000000 async_bakalari_api-0.3.1/src/bakalari_api/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6797 2024-05-19 22:57:52.000000 async_bakalari_api-0.3.1/src/bakalari_api/datastructure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-19 22:57:52.000000 async_bakalari_api-0.3.1/src/bakalari_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-19 22:57:52.000000 async_bakalari_api-0.3.1/src/bakalari_api/first_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-05-19 22:57:52.000000 async_bakalari_api-0.3.1/src/bakalari_api/komens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-19 22:57:52.000000 async_bakalari_api-0.3.1/src/bakalari_api/logger_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:57:57.287777 async_bakalari_api-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    19347 2024-05-19 22:57:52.000000 async_bakalari_api-0.3.1/tests/test_bakalari.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-19 22:57:52.000000 async_bakalari_api-0.3.1/tests/test_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7431 2024-05-19 22:57:52.000000 async_bakalari_api-0.3.1/tests/test_datastructure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-05-19 22:57:52.000000 async_bakalari_api-0.3.1/tests/test_komens.py
```

### Comparing `async_bakalari_api-0.3/LICENSE.md` & `async_bakalari_api-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `async_bakalari_api-0.3/PKG-INFO` & `async_bakalari_api-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async_bakalari_api
-Version: 0.3
+Version: 0.3.1
 Summary: Async API for Bakalari endpoint v3
 Author-email: "Lukas Svoboda (@schizza)" <opensource@schizza.cz>
 Maintainer-email: Lukas Svoboda <opensource@schizza.cz>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -215,14 +215,26 @@
 Keywords: bakalari,async
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: aiohttp==3.9.5
+Requires-Dist: aiosignal==1.3.1
+Requires-Dist: attrs==23.2.0
+Requires-Dist: frozenlist==1.4.1
+Requires-Dist: idna==3.7
+Requires-Dist: logger==1.4
+Requires-Dist: multidict==6.0.5
+Requires-Dist: orjson==3.10.3
+Requires-Dist: python-dateutil==2.9.0.post0
+Requires-Dist: six==1.16.0
+Requires-Dist: strenum==0.4.15
+Requires-Dist: yarl==1.9.4
 
 [![codecov](https://codecov.io/gh/schizza/async-bakalari-api3/graph/badge.svg?token=KC2WYAOLOP)](https://codecov.io/gh/schizza/async-bakalari-api3)
 
 # Changelog
 
 All notable changes to this project will be documented in this file.
```

### Comparing `async_bakalari_api-0.3/README.md` & `async_bakalari_api-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `async_bakalari_api-0.3/pyproject.toml` & `async_bakalari_api-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "async_bakalari_api"
-version = "0.3"
+version = "0.3.1"
 dynamic = ["dependencies"]
 
 
 requires-python = ">=3.12"
 authors = [
   {name = "Lukas Svoboda (@schizza)", email = "opensource@schizza.cz"}
 ]
@@ -22,15 +22,15 @@
 keywords = ["bakalari", "async"]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python"
 ]
 
 [tool.setuptools.dynamic]
-dependencies = { file = ["requirements.in"] }
+dependencies = { file = ["requirements.txt"] }
 
 [tool.setuptools]
 platforms = ["any"]
 zip-safe  = false
 include-package-data = true
 
 [project.urls]
```

### Comparing `async_bakalari_api-0.3/src/async_bakalari_api.egg-info/PKG-INFO` & `async_bakalari_api-0.3.1/src/async_bakalari_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async_bakalari_api
-Version: 0.3
+Version: 0.3.1
 Summary: Async API for Bakalari endpoint v3
 Author-email: "Lukas Svoboda (@schizza)" <opensource@schizza.cz>
 Maintainer-email: Lukas Svoboda <opensource@schizza.cz>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -215,14 +215,26 @@
 Keywords: bakalari,async
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: aiohttp==3.9.5
+Requires-Dist: aiosignal==1.3.1
+Requires-Dist: attrs==23.2.0
+Requires-Dist: frozenlist==1.4.1
+Requires-Dist: idna==3.7
+Requires-Dist: logger==1.4
+Requires-Dist: multidict==6.0.5
+Requires-Dist: orjson==3.10.3
+Requires-Dist: python-dateutil==2.9.0.post0
+Requires-Dist: six==1.16.0
+Requires-Dist: strenum==0.4.15
+Requires-Dist: yarl==1.9.4
 
 [![codecov](https://codecov.io/gh/schizza/async-bakalari-api3/graph/badge.svg?token=KC2WYAOLOP)](https://codecov.io/gh/schizza/async-bakalari-api3)
 
 # Changelog
 
 All notable changes to this project will be documented in this file.
```

### Comparing `async_bakalari_api-0.3/src/async_bakalari_api.egg-info/SOURCES.txt` & `async_bakalari_api-0.3.1/src/async_bakalari_api.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 LICENSE.md
 README.md
 pyproject.toml
+requirements.txt
 src/__init__.py
 src/async_bakalari_api.egg-info/PKG-INFO
 src/async_bakalari_api.egg-info/SOURCES.txt
 src/async_bakalari_api.egg-info/dependency_links.txt
 src/async_bakalari_api.egg-info/entry_points.txt
 src/async_bakalari_api.egg-info/not-zip-safe
+src/async_bakalari_api.egg-info/requires.txt
 src/async_bakalari_api.egg-info/top_level.txt
 src/bakalari_api/__init__.py
 src/bakalari_api/__main__.py
 src/bakalari_api/bakalari.py
 src/bakalari_api/bakalari_demo.py
 src/bakalari_api/const.py
 src/bakalari_api/datastructure.py
```

### Comparing `async_bakalari_api-0.3/src/bakalari_api/bakalari.py` & `async_bakalari_api-0.3.1/src/bakalari_api/bakalari.py`

 * *Files identical despite different names*

### Comparing `async_bakalari_api-0.3/src/bakalari_api/bakalari_demo.py` & `async_bakalari_api-0.3.1/src/bakalari_api/bakalari_demo.py`

 * *Files identical despite different names*

### Comparing `async_bakalari_api-0.3/src/bakalari_api/const.py` & `async_bakalari_api-0.3.1/src/bakalari_api/const.py`

 * *Files identical despite different names*

### Comparing `async_bakalari_api-0.3/src/bakalari_api/exceptions.py` & `async_bakalari_api-0.3.1/src/bakalari_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `async_bakalari_api-0.3/src/bakalari_api/komens.py` & `async_bakalari_api-0.3.1/src/bakalari_api/komens.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,17 +67,17 @@
         }
         return orjson.dumps(json_repr)
 
     def __str__(self) -> str:
         """Return string representation of data."""
         return f"""Message id: {self.mid}
             title: {self.title}
-            text: {self.text},
-            sent: {self.sent},
-            sender: {self.sender},
+            text: {self.text}
+            sent: {self.sent}
+            sender: {self.sender}
             attachments: {self.attachments}"""
 
 
 class Messages(list[MessageContainer]):
     """Messages class holds all messages."""
 
     def __init__(self) -> None:
```

### Comparing `async_bakalari_api-0.3/src/bakalari_api/logger_api.py` & `async_bakalari_api-0.3.1/src/bakalari_api/logger_api.py`

 * *Files identical despite different names*

### Comparing `async_bakalari_api-0.3/tests/test_bakalari.py` & `async_bakalari_api-0.3.1/tests/test_bakalari.py`

 * *Files identical despite different names*

### Comparing `async_bakalari_api-0.3/tests/test_datastructure.py` & `async_bakalari_api-0.3.1/tests/test_datastructure.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 import tempfile
 from unittest.mock import patch
 
 import orjson
 import pytest
 from src.bakalari_api.bakalari import Credentials, Schools
+from src.bakalari_api.datastructure import UniqueTowns
 
 
 @pytest.fixture
 def mocker_file(mocker):
     """Mock file for testing."""
     data = b'[{"name": "test_name","api_point": "test_api_point","town": "test_town"}]'
     mocked_file = mocker.mock_open(read_data=data)
     mocker.patch("builtins.open", mocked_file)
 
 
-@pytest.mark.asyncio
 async def test_school_list_from_file(mocker_file):
     """Test loading schools from file."""
 
     schools: Schools = await Schools().load_from_file("fakefile")
     assert isinstance(schools, Schools)
 
 
@@ -29,43 +29,40 @@
     """Mock file for testing."""
 
     data = b'[{"name": "test_name","api_point": "test_api_point","town": "test_town"}'
     mocked_file = mocker.mock_open(read_data=data)
     mocker.patch("builtins.open", mocked_file)
 
 
-@pytest.mark.asyncio
 async def test_school_list_from_file_bad_data(mocker_file_bad_data):
     """Test loading schools from file."""
 
     schools: Schools = await Schools().load_from_file("fakefile")
     assert not isinstance(schools, Schools)
 
 
-@pytest.mark.asyncio
 async def test_schools_list_from_file_no_file():
     """Test loading schools from file."""
 
     schools: Schools = await Schools().load_from_file("")
     assert schools is False
 
 
-@pytest.mark.asyncio
 async def test_school_append():
     """Test appending schools to the list."""
 
     schools = Schools()
 
     assert not schools.append_school("", "test_api_point", "test_town_in")
     assert not schools.append_school("test_school", "", "test_town_in")
     assert not schools.append_school("test_school", "test_api_point", "")
     assert schools.append_school("test_school", "test_api_point", "test_town_in")
+    assert len(schools) == 1
 
 
-@pytest.mark.asyncio
 async def test_school_by_name():
     """Test getting schools by name."""
 
     schools = Schools()
     schools.append_school("test_school", "test_api_point", "test_town_in")
     schools.append_school("test_school_2", "test_api_point", "test_town_another_town")
 
@@ -74,30 +71,28 @@
 
     assert len(schools.school_list) == 2
     assert len(test_town_in) == 1
     assert test_town_in[0].name == "test_school"
     assert len(test_town_out) == 0
 
 
-@pytest.mark.asyncio
 async def test_school_by_api_point():
     """Test getting schools by api point."""
 
     schools = Schools()
     schools.append_school("test_school", "test_api_point_in", "test_town_in")
 
     test_api_point = schools.get_school_name_by_api_point("test_api_point_in")
     test_non_exist = schools.get_school_name_by_api_point("non_existing_api_point")
 
     assert len(schools.school_list) == 1
     assert test_api_point == "test_school"
     assert test_non_exist is None
 
 
-@pytest.mark.asyncio
 async def test_get_url():
     """Test getting url by name or index."""
 
     schools = Schools()
     schools.append_school("test_school", "test_api_point_in", "test_town_in")
     schools.append_school("test_school2", "test_api_point_out", "test_town_in")
 
@@ -115,15 +110,14 @@
 
 
 def open_err(*args, **kwargs):
     """Raise OSError."""
     raise OSError
 
 
-@pytest.mark.asyncio
 async def test_write_file(monkeypatch):
     """Test writing to file."""
 
     schools = Schools()
     schools.append_school("test_school", "test_api_point_in", "test_town_in")
     schools.append_school("test_school2", "test_api_point_out", "test_town_in")
 
@@ -156,7 +150,109 @@
 
     credentials = Credentials.create_from_json(data_json)
 
     assert isinstance(credentials, Credentials)
     assert credentials.access_token == "test_token"
     assert credentials.refresh_token == "test_refresh_token"
     assert credentials.user_id == "test_user_id"
+
+
+def test_append_unique_town():
+    """Test appending unique towns."""
+
+    towns = UniqueTowns()
+    towns.append("Town A")
+    towns.append("Town B")
+    towns.append("Town C")
+    assert len(towns) == 3
+    assert "Town A" in towns
+    assert "Town B" in towns
+    assert "Town C" in towns
+
+
+def test_append_duplicate_town():
+    """Test appending duplicate towns."""
+    towns = UniqueTowns()
+    towns.append("Town A")
+    towns.append("Town B")
+    towns.append("Town A")
+    assert len(towns) == 2
+    assert "Town A" in towns
+    assert "Town B" in towns
+
+
+def test_remove_town():
+    """Test removing town."""
+
+    towns = UniqueTowns()
+    towns.append("Town A")
+    towns.append("Town B")
+    towns.append("Town C")
+    assert len(towns) == 3
+    del towns["Town B"]
+    assert len(towns) == 2
+    assert "Town A" in towns
+    assert "Town B" not in towns
+    assert "Town C" in towns
+
+
+def test_get_town_by_index():
+    """Test getting town by index."""
+    towns = UniqueTowns()
+    towns.append("Town A")
+    towns.append("Town B")
+    towns.append("Town C")
+    assert towns[0] == "Town A"
+    assert towns[1] == "Town B"
+    assert towns[2] == "Town C"
+
+
+def test_get_all_towns():
+    """Test getting all towns."""
+
+    towns = Schools()
+    towns.towns_list.append("Town A")
+    towns.towns_list.append("Town B")
+    towns.towns_list.append("Town C")
+    assert towns.get_all_towns() == ["Town A", "Town B", "Town C"]
+
+
+def test_iterate_towns():
+    """Test iterating over towns."""
+    towns = UniqueTowns()
+    towns.append("Town A")
+    towns.append("Town B")
+    towns.append("Town C")
+    assert list(towns) == ["Town A", "Town B", "Town C"]
+
+
+def test_count_towns():
+    """Test counting towns."""
+    towns = Schools()
+    towns.towns_list.append("Town A")
+    towns.towns_list.append("Town B")
+    towns.towns_list.append("Town C")
+    assert towns.count_towns() == 3
+
+
+def test_str_towns():
+    """Test counting towns."""
+    towns = Schools()
+    towns.towns_list.append("Town A")
+    assert str(towns.towns_list) == "['Town A']"
+
+
+def test_istown():
+    """Test checking if town is in the list."""
+    towns = Schools()
+    towns.towns_list.append("Town A")
+    assert towns.istown("Town A")
+
+
+def test_get_towns_partial_name():
+    """Test getting towns by partial name."""
+    towns = Schools()
+    towns.towns_list.append("Town A")
+    towns.towns_list.append("Town B")
+    towns.towns_list.append("Town C")
+    assert towns.get_towns_partial_name("own") == ["Town A", "Town B", "Town C"]
+    assert towns.get_towns_partial_name("own A") == ["Town A"]
```

### Comparing `async_bakalari_api-0.3/tests/test_komens.py` & `async_bakalari_api-0.3.1/tests/test_komens.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,23 +103,23 @@
         assert msg.text == "fake_text_id1"
         assert msg.title == ""
 
         assert (
             str(msgs)
             == """Message id: fake_id1
             title: 
-            text: fake_text_id1,
-            sent: 2024-01-01,
-            sender: fake_teacher_name1,
+            text: fake_text_id1
+            sent: 2024-01-01
+            sender: fake_teacher_name1
             attachments: [{'$type': 'AttachmentInfo', 'Id': 'fake_attachment_id1', 'Name': 'fake_atachement_name1', 'Type': 'fake_type', 'Size': 12345}]
 Message id: fake_id2
             title: 
-            text: fake_text_id2,
-            sent: 2024-01-05,
-            sender: fake_teacher_name2,
+            text: fake_text_id2
+            sent: 2024-01-05
+            sender: fake_teacher_name2
             attachments: []
 """
         )
         assert_msgs = [
             {
                 "mid": msg.mid,
                 "title": msg.title,
@@ -141,17 +141,17 @@
         assert isinstance(msg, list)
         assert len(msg) == 2
         assert msg[1].mid == "fake_id2"
         assert (
             str(msg[1])
             == """Message id: fake_id2
             title: 
-            text: fake_text_id2,
-            sent: 2024-01-05,
-            sender: fake_teacher_name2,
+            text: fake_text_id2
+            sent: 2024-01-05
+            sender: fake_teacher_name2
             attachments: []"""
         )
 
         assert (
             repr(msg[0])
             == "<MessageContainer message_id=fake_id1 title= sender=fake_teacher_name1>"
         )
```

