# Comparing `tmp/pydora-2.2.0.tar.gz` & `tmp/pydora-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydora-2.2.0.tar", last modified: Sat Sep  2 17:10:47 2023, max compression
+gzip compressed data, was "pydora-2.3.0.tar", last modified: Mon May 20 18:55:38 2024, max compression
```

## Comparing `pydora-2.2.0.tar` & `pydora-2.3.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 17:10:47.575909 pydora-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (999)     1057 2023-09-02 17:10:20.000000 pydora-2.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (999)    11327 2023-09-02 17:10:47.579908 pydora-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)    10408 2023-09-02 17:10:20.000000 pydora-2.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 17:10:47.567908 pydora-2.2.0/pandora/
--rw-r--r--   0 runner    (1001) docker     (999)       22 2023-09-02 17:10:20.000000 pydora-2.2.0/pandora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     9878 2023-09-02 17:10:20.000000 pydora-2.2.0/pandora/client.py
--rw-r--r--   0 runner    (1001) docker     (999)     7233 2023-09-02 17:10:20.000000 pydora-2.2.0/pandora/clientbuilder.py
--rw-r--r--   0 runner    (1001) docker     (999)     3269 2023-09-02 17:10:20.000000 pydora-2.2.0/pandora/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 17:10:47.571908 pydora-2.2.0/pandora/models/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-02 17:10:20.000000 pydora-2.2.0/pandora/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     9927 2023-09-02 17:10:20.000000 pydora-2.2.0/pandora/models/_base.py
--rw-r--r--   0 runner    (1001) docker     (999)     1279 2023-09-02 17:10:20.000000 pydora-2.2.0/pandora/models/ad.py
--rw-r--r--   0 runner    (1001) docker     (999)      867 2023-09-02 17:10:20.000000 pydora-2.2.0/pandora/models/bookmark.py
--rw-r--r--   0 runner    (1001) docker     (999)     6071 2023-09-02 17:10:20.000000 pydora-2.2.0/pandora/models/playlist.py
--rw-r--r--   0 runner    (1001) docker     (999)     2836 2023-09-02 17:10:20.000000 pydora-2.2.0/pandora/models/search.py
--rw-r--r--   0 runner    (1001) docker     (999)     3540 2023-09-02 17:10:20.000000 pydora-2.2.0/pandora/models/station.py
--rw-r--r--   0 runner    (1001) docker     (999)     9703 2023-09-02 17:10:20.000000 pydora-2.2.0/pandora/transport.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 17:10:47.575909 pydora-2.2.0/pydora/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-02 17:10:20.000000 pydora-2.2.0/pydora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     9718 2023-09-02 17:10:20.000000 pydora-2.2.0/pydora/audio_backend.py
--rw-r--r--   0 runner    (1001) docker     (999)     5163 2023-09-02 17:10:20.000000 pydora-2.2.0/pydora/configure.py
--rw-r--r--   0 runner    (1001) docker     (999)     9403 2023-09-02 17:10:20.000000 pydora-2.2.0/pydora/player.py
--rw-r--r--   0 runner    (1001) docker     (999)     5542 2023-09-02 17:10:20.000000 pydora-2.2.0/pydora/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 17:10:47.575909 pydora-2.2.0/pydora.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)    11327 2023-09-02 17:10:47.000000 pydora-2.2.0/pydora.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      598 2023-09-02 17:10:47.000000 pydora-2.2.0/pydora.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-02 17:10:47.000000 pydora-2.2.0/pydora.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       87 2023-09-02 17:10:47.000000 pydora-2.2.0/pydora.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (999)       36 2023-09-02 17:10:47.000000 pydora-2.2.0/pydora.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       15 2023-09-02 17:10:47.000000 pydora-2.2.0/pydora.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)     1859 2023-09-02 17:10:47.579908 pydora-2.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (999)       62 2023-09-02 17:10:20.000000 pydora-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:55:38.604909 pydora-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-20 18:55:21.000000 pydora-2.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11393 2024-05-20 18:55:38.604909 pydora-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10408 2024-05-20 18:55:21.000000 pydora-2.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:55:38.600909 pydora-2.3.0/pandora/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-20 18:55:21.000000 pydora-2.3.0/pandora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9879 2024-05-20 18:55:21.000000 pydora-2.3.0/pandora/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7234 2024-05-20 18:55:21.000000 pydora-2.3.0/pandora/clientbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-20 18:55:21.000000 pydora-2.3.0/pandora/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:55:38.604909 pydora-2.3.0/pandora/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 18:55:21.000000 pydora-2.3.0/pandora/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9927 2024-05-20 18:55:21.000000 pydora-2.3.0/pandora/models/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-20 18:55:21.000000 pydora-2.3.0/pandora/models/ad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-20 18:55:21.000000 pydora-2.3.0/pandora/models/bookmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6071 2024-05-20 18:55:21.000000 pydora-2.3.0/pandora/models/playlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-20 18:55:21.000000 pydora-2.3.0/pandora/models/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-05-20 18:55:21.000000 pydora-2.3.0/pandora/models/station.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9704 2024-05-20 18:55:21.000000 pydora-2.3.0/pandora/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:55:38.604909 pydora-2.3.0/pydora/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 18:55:21.000000 pydora-2.3.0/pydora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9718 2024-05-20 18:55:21.000000 pydora-2.3.0/pydora/audio_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5163 2024-05-20 18:55:21.000000 pydora-2.3.0/pydora/configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9403 2024-05-20 18:55:21.000000 pydora-2.3.0/pydora/player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-05-20 18:55:21.000000 pydora-2.3.0/pydora/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:55:38.604909 pydora-2.3.0/pydora.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11393 2024-05-20 18:55:38.000000 pydora-2.3.0/pydora.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-20 18:55:38.000000 pydora-2.3.0/pydora.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 18:55:38.000000 pydora-2.3.0/pydora.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-20 18:55:38.000000 pydora-2.3.0/pydora.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-20 18:55:38.000000 pydora-2.3.0/pydora.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-20 18:55:38.000000 pydora-2.3.0/pydora.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-20 18:55:38.604909 pydora-2.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       62 2024-05-20 18:55:21.000000 pydora-2.3.0/setup.py
```

### Comparing `pydora-2.2.0/LICENSE.txt` & `pydora-2.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydora-2.2.0/PKG-INFO` & `pydora-2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydora
-Version: 2.2.0
+Version: 2.3.0
 Summary: Python wrapper for Pandora API
 Home-page: https://github.com/mcrute/pydora
 Author: Mike Crute
 Author-email: mike@crute.us
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -15,16 +15,18 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Multimedia :: Sound/Audio :: Players
-Requires-Python: >=3.5
+Requires-Python: >=3.8
 License-File: LICENSE.txt
+Requires-Dist: requests<3,>=2
+Requires-Dist: blowfish<1.0,>=0.6.1
 
 ==================
 Pandora API Client
 ==================
 
 .. image:: https://img.shields.io/pypi/v/pydora.svg
     :target: https://pypi.python.org/pypi/pydora
@@ -54,15 +56,15 @@
 
 If you run into a problem, file an issue and we'll respond. Pull requests for
 new features and fixes will be reviewed and accepted if they meet our criteria
 for stability, see below for contributing instructions.
 
 Compatibility
 =============
-This is the ``2.x`` series which supports only Python 3.5+. For older versions
+This is the ``2.x`` series which supports only Python 3.8+. For older versions
 of Python please use the |1.x|_ series. The |1.x|_ series is no longer
 maintained but pull requests to fix bugs are still welcomed.
 
 This package uses semantic versioning. The API is guaranteed to be stable
 within a major version release. Please constrain your dependencies to major
 versions. For example, to depend on version ``2.x`` use this line in your
 setup.py ``install_requires``::
```

### Comparing `pydora-2.2.0/README.rst` & `pydora-2.3.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 If you run into a problem, file an issue and we'll respond. Pull requests for
 new features and fixes will be reviewed and accepted if they meet our criteria
 for stability, see below for contributing instructions.
 
 Compatibility
 =============
-This is the ``2.x`` series which supports only Python 3.5+. For older versions
+This is the ``2.x`` series which supports only Python 3.8+. For older versions
 of Python please use the |1.x|_ series. The |1.x|_ series is no longer
 maintained but pull requests to fix bugs are still welcomed.
 
 This package uses semantic versioning. The API is guaranteed to be stable
 within a major version release. Please constrain your dependencies to major
 versions. For example, to depend on version ``2.x`` use this line in your
 setup.py ``install_requires``::
```

### Comparing `pydora-2.2.0/pandora/client.py` & `pydora-2.3.0/pandora/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 The high level API client is what most clients should use and provides API
 calls that map directly to the Pandora API and return model objects with
 mappings from the raw JSON structures to Python objects.
 
 For simplicity use a client builder from pandora.clientbuilder to create an
 instance of a client.
 """
+
 from . import errors
 
 
 class BaseAPIClient:
     """Base Pandora API Client
 
     The base API client has lower level methods that are composed together to
```

### Comparing `pydora-2.2.0/pandora/clientbuilder.py` & `pydora-2.3.0/pandora/clientbuilder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Pandora API Client Builders
 
 This module provides a set of builder classes that can turn various
 configuration formats into a fully built APIClient.
 """
+
 import os.path
 
 from configparser import ConfigParser
 from .client import APIClient
 from .transport import Encryptor, APITransport, DEFAULT_API_HOST
```

### Comparing `pydora-2.2.0/pandora/errors.py` & `pydora-2.3.0/pandora/errors.py`

 * *Files identical despite different names*

### Comparing `pydora-2.2.0/pandora/models/_base.py` & `pydora-2.3.0/pandora/models/_base.py`

 * *Files identical despite different names*

### Comparing `pydora-2.2.0/pandora/models/ad.py` & `pydora-2.3.0/pandora/models/ad.py`

 * *Files identical despite different names*

### Comparing `pydora-2.2.0/pandora/models/bookmark.py` & `pydora-2.3.0/pandora/models/bookmark.py`

 * *Files identical despite different names*

### Comparing `pydora-2.2.0/pandora/models/playlist.py` & `pydora-2.3.0/pandora/models/playlist.py`

 * *Files identical despite different names*

### Comparing `pydora-2.2.0/pandora/models/search.py` & `pydora-2.3.0/pandora/models/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 class SongSearchResultItem(SearchResultItem):
     score = Field("score")
     token = Field("musicToken")
     artist = Field("artistName")
     song_name = Field("songName")
 
     def create_station(self):
-        return self._api_client.create_station(track_token=self.token)
+        return self._api_client.create_station(song_token=self.token)
 
     @classmethod
     def from_json(cls, api_client, data):
         return super(SearchResultItem, cls).from_json(api_client, data)
 
 
 class GenreStationSearchResultItem(SearchResultItem):
```

### Comparing `pydora-2.2.0/pandora/models/station.py` & `pydora-2.3.0/pandora/models/station.py`

 * *Files identical despite different names*

### Comparing `pydora-2.2.0/pandora/transport.py` & `pydora-2.3.0/pandora/transport.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 The transport is concerned with the details of a raw HTTP call to the Pandora
 API along with the request and response encryption by way of an Encyrpytor
 object. The result from a transport is a JSON object for the API or an
 exception.
 
 API consumers should use one of the API clients in the pandora.client package.
 """
+
 import random
 import time
 import json
 import base64
 import blowfish
 import requests
 from requests.adapters import HTTPAdapter
```

### Comparing `pydora-2.2.0/pydora/audio_backend.py` & `pydora-2.3.0/pydora/audio_backend.py`

 * *Files identical despite different names*

### Comparing `pydora-2.2.0/pydora/configure.py` & `pydora-2.3.0/pydora/configure.py`

 * *Files identical despite different names*

### Comparing `pydora-2.2.0/pydora/player.py` & `pydora-2.3.0/pydora/player.py`

 * *Files identical despite different names*

### Comparing `pydora-2.2.0/pydora/utils.py` & `pydora-2.3.0/pydora/utils.py`

 * *Files identical despite different names*

### Comparing `pydora-2.2.0/pydora.egg-info/PKG-INFO` & `pydora-2.3.0/pydora.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydora
-Version: 2.2.0
+Version: 2.3.0
 Summary: Python wrapper for Pandora API
 Home-page: https://github.com/mcrute/pydora
 Author: Mike Crute
 Author-email: mike@crute.us
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -15,16 +15,18 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Multimedia :: Sound/Audio :: Players
-Requires-Python: >=3.5
+Requires-Python: >=3.8
 License-File: LICENSE.txt
+Requires-Dist: requests<3,>=2
+Requires-Dist: blowfish<1.0,>=0.6.1
 
 ==================
 Pandora API Client
 ==================
 
 .. image:: https://img.shields.io/pypi/v/pydora.svg
     :target: https://pypi.python.org/pypi/pydora
@@ -54,15 +56,15 @@
 
 If you run into a problem, file an issue and we'll respond. Pull requests for
 new features and fixes will be reviewed and accepted if they meet our criteria
 for stability, see below for contributing instructions.
 
 Compatibility
 =============
-This is the ``2.x`` series which supports only Python 3.5+. For older versions
+This is the ``2.x`` series which supports only Python 3.8+. For older versions
 of Python please use the |1.x|_ series. The |1.x|_ series is no longer
 maintained but pull requests to fix bugs are still welcomed.
 
 This package uses semantic versioning. The API is guaranteed to be stable
 within a major version release. Please constrain your dependencies to major
 versions. For example, to depend on version ``2.x`` use this line in your
 setup.py ``install_requires``::
```

### Comparing `pydora-2.2.0/pydora.egg-info/SOURCES.txt` & `pydora-2.3.0/pydora.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydora-2.2.0/setup.cfg` & `pydora-2.3.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3 :: Only
 	Topic :: Internet :: WWW/HTTP
 	Topic :: Multimedia :: Sound/Audio :: Players
 
 [options]
 packages = find:
-python_requires = >=3.5
+python_requires = >=3.8
 install_requires = 
 	requests >=2, <3
 	blowfish >=0.6.1, <1.0
 
 [options.packages.find]
 exclude = 
 	tests
@@ -39,37 +39,38 @@
 	pydora = pydora.player:main
 	pydora-configure = pydora.configure:main
 
 [tox:tox]
 
 [testenv:format]
 deps = 
-	black
+	black ==24.4.2
 commands = 
 	black -l 79 -t py311 pandora/ pydora/ tests/ setup.py
 
 [testenv:tests]
 deps = 
 	pytest
-	black
+	black ==24.4.2
 	flake8 >=3.3
 	coverage >=7
 commands = 
 	black --check -l 79 -t py311 pandora/ pydora/ tests/ setup.py
 	flake8 --statistics --ignore=E231 pandora/ pydora/ tests/ setup.py
 	coverage run --source='pandora/,pydora/' -m pytest
 	coverage report --fail-under 100 -m --include='pandora/*'
 	coverage report -m --include='pydora/*'
 	coverage html --include='pandora/*,pydora/*'
 
 [testenv:release]
 deps = 
-	wheel
+	build
 commands = 
-	python setup.py sdist bdist_wheel
+	python -m build --sdist
+	python -m build --wheel
 
 [testenv:upload]
 skip_install = true
 deps = 
 	twine
 passenv = 
 	TWINE_PASSWORD
```

