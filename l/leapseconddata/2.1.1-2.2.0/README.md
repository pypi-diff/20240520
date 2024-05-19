# Comparing `tmp/leapseconddata-2.1.1.tar.gz` & `tmp/leapseconddata-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leapseconddata-2.1.1.tar", last modified: Tue Oct  3 14:29:14 2023, max compression
+gzip compressed data, was "leapseconddata-2.2.0.tar", last modified: Sun May 19 22:57:24 2024, max compression
```

## Comparing `leapseconddata-2.1.1.tar` & `leapseconddata-2.2.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 14:29:14.466702 leapseconddata-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2023-10-03 14:28:51.000000 leapseconddata-2.1.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 14:29:14.462701 leapseconddata-2.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 14:29:14.466702 leapseconddata-2.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      801 2023-10-03 14:28:51.000000 leapseconddata-2.1.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2023-10-03 14:28:51.000000 leapseconddata-2.1.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      161 2023-10-03 14:28:51.000000 leapseconddata-2.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      715 2023-10-03 14:28:51.000000 leapseconddata-2.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-10-03 14:28:51.000000 leapseconddata-2.1.1/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 14:29:14.466702 leapseconddata-2.1.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2023-10-03 14:28:51.000000 leapseconddata-2.1.1/LICENSES/CC0-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    34670 2023-10-03 14:28:51.000000 leapseconddata-2.1.1/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2023-10-03 14:28:51.000000 leapseconddata-2.1.1/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2023-10-03 14:28:51.000000 leapseconddata-2.1.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2023-10-03 14:29:14.466702 leapseconddata-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      865 2023-10-03 14:28:51.000000 leapseconddata-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 14:29:14.466702 leapseconddata-2.1.1/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-03 14:28:51.000000 leapseconddata-2.1.1/_static/.empty
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-03 14:28:51.000000 leapseconddata-2.1.1/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2023-10-03 14:28:51.000000 leapseconddata-2.1.1/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2023-10-03 14:28:51.000000 leapseconddata-2.1.1/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 14:29:14.466702 leapseconddata-2.1.1/leapseconddata/
--rwxr-xr-x   0 runner    (1001) docker     (127)    12900 2023-10-03 14:28:51.000000 leapseconddata-2.1.1/leapseconddata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2023-10-03 14:28:51.000000 leapseconddata-2.1.1/leapseconddata/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-03 14:28:51.000000 leapseconddata-2.1.1/leapseconddata/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 14:29:14.466702 leapseconddata-2.1.1/leapseconddata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2023-10-03 14:29:14.000000 leapseconddata-2.1.1/leapseconddata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      629 2023-10-03 14:29:14.000000 leapseconddata-2.1.1/leapseconddata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-03 14:29:14.000000 leapseconddata-2.1.1/leapseconddata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-10-03 14:29:14.000000 leapseconddata-2.1.1/leapseconddata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      245 2023-10-03 14:28:51.000000 leapseconddata-2.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      223 2023-10-03 14:28:51.000000 leapseconddata-2.1.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      916 2023-10-03 14:29:14.466702 leapseconddata-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2023-10-03 14:28:51.000000 leapseconddata-2.1.1/testleapseconddata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:57:24.157765 leapseconddata-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-19 22:57:06.000000 leapseconddata-2.2.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:57:24.149765 leapseconddata-2.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:57:24.153765 leapseconddata-2.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-19 22:57:06.000000 leapseconddata-2.2.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-19 22:57:06.000000 leapseconddata-2.2.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-19 22:57:06.000000 leapseconddata-2.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-19 22:57:06.000000 leapseconddata-2.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-19 22:57:06.000000 leapseconddata-2.2.0/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:57:24.153765 leapseconddata-2.2.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-05-19 22:57:06.000000 leapseconddata-2.2.0/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    34670 2024-05-19 22:57:06.000000 leapseconddata-2.2.0/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-19 22:57:06.000000 leapseconddata-2.2.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-19 22:57:06.000000 leapseconddata-2.2.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-19 22:57:24.157765 leapseconddata-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-19 22:57:06.000000 leapseconddata-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:57:24.153765 leapseconddata-2.2.0/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 22:57:06.000000 leapseconddata-2.2.0/_static/.empty
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 22:57:06.000000 leapseconddata-2.2.0/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-19 22:57:06.000000 leapseconddata-2.2.0/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-19 22:57:06.000000 leapseconddata-2.2.0/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:57:24.153765 leapseconddata-2.2.0/leapseconddata/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12903 2024-05-19 22:57:06.000000 leapseconddata-2.2.0/leapseconddata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-19 22:57:06.000000 leapseconddata-2.2.0/leapseconddata/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 22:57:06.000000 leapseconddata-2.2.0/leapseconddata/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:57:24.157765 leapseconddata-2.2.0/leapseconddata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-19 22:57:24.000000 leapseconddata-2.2.0/leapseconddata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-19 22:57:24.000000 leapseconddata-2.2.0/leapseconddata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 22:57:24.000000 leapseconddata-2.2.0/leapseconddata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-19 22:57:24.000000 leapseconddata-2.2.0/leapseconddata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-19 22:57:06.000000 leapseconddata-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-19 22:57:06.000000 leapseconddata-2.2.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-19 22:57:24.157765 leapseconddata-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-05-19 22:57:06.000000 leapseconddata-2.2.0/testleapseconddata.py
```

### Comparing `leapseconddata-2.1.1/.github/workflows/release.yml` & `leapseconddata-2.2.0/.github/workflows/release.yml`

 * *Files 14% similar despite different names*

```diff
@@ -14,18 +14,18 @@
     runs-on: ubuntu-latest
     steps:
     - name: Dump GitHub context
       env:
         GITHUB_CONTEXT: ${{ toJson(github) }}
       run: echo "$GITHUB_CONTEXT"
 
-    - uses: actions/checkout@v2.2.0
+    - uses: actions/checkout@v4
 
     - name: Set up Python
-      uses: actions/setup-python@v1
+      uses: actions/setup-python@v5
       with:
         python-version: "3.x"
 
     - name: Install deps
       run: python -mpip install -r requirements-dev.txt
 
     - name: Build release
```

### Comparing `leapseconddata-2.1.1/.github/workflows/test.yml` & `leapseconddata-2.2.0/.github/workflows/test.yml`

 * *Files 3% similar despite different names*

```diff
@@ -13,35 +13,35 @@
     types: [rerequested]
 
 jobs:
   docs:
     runs-on: ubuntu-latest
     steps:
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v5
       with:
         python-version: '3.10'
 
-    - uses: actions/checkout@v2.2.0
+    - uses: actions/checkout@v4
 
     - name: Install deps
       run: python -mpip install -r requirements-dev.txt
 
     - name: Build HTML docs
       run: make html
 
   test:
     strategy:
       matrix:
         python-version:
-        - '3.8'
         - '3.9'
         - '3.10'
         - '3.11'
-        - '3.12.0-alpha.0 - 3.12'
+        - '3.12'
+        - '3.13.0-alpha.0 - 3.13'
         - 'pypy-3.9'
         os-version:
         - 'ubuntu-latest'
         include:
           - os-version: 'macos-latest'
             python-version: '3.x'
           - os-version: 'windows-latest'
@@ -51,15 +51,15 @@
       PYTHON: ${{ matrix.python-version }}
 
     runs-on: ${{ matrix.os-version }}
     steps:
     - uses: actions/checkout@v4
 
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Install deps
       run: python -mpip install -r requirements-dev.txt
 
     - name: Check stubs
@@ -69,9 +69,8 @@
     - name: Test
       run: python -mcoverage run --branch -m unittest testleapseconddata.py && python -mcoverage report --fail-under=100 && python -mcoverage xml
 
   pre-commit:
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v4
-    - uses: actions/setup-python@v4
-    - uses: pre-commit/action@v3.0.0
+    - uses: pre-commit/action@v3.0.1
```

### Comparing `leapseconddata-2.1.1/LICENSES/CC0-1.0.txt` & `leapseconddata-2.2.0/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `leapseconddata-2.1.1/LICENSES/GPL-3.0-only.txt` & `leapseconddata-2.2.0/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `leapseconddata-2.1.1/LICENSES/Unlicense.txt` & `leapseconddata-2.2.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `leapseconddata-2.1.1/Makefile` & `leapseconddata-2.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `leapseconddata-2.1.1/PKG-INFO` & `leapseconddata-2.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: leapseconddata
-Version: 2.1.1
+Version: 2.2.0
 Summary: Use the list of known and scheduled leap seconds
 Home-page: https://github.com/jepler/leapseconddata
 Author: Jeff Epler
 Author-email: jepler@gmail.com
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 <!--
 SPDX-FileCopyrightText: 2021 Jeff Epler
 
 SPDX-License-Identifier: GPL-3.0-only
 -->
```

### Comparing `leapseconddata-2.1.1/README.md` & `leapseconddata-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `leapseconddata-2.1.1/conf.py` & `leapseconddata-2.2.0/conf.py`

 * *Files identical despite different names*

### Comparing `leapseconddata-2.1.1/index.rst` & `leapseconddata-2.2.0/index.rst`

 * *Files identical despite different names*

### Comparing `leapseconddata-2.1.1/leapseconddata/__init__.py` & `leapseconddata-2.2.0/leapseconddata/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     """The list is valid until this UTC time"""
 
     last_updated: Optional[datetime.datetime] = field(default=None)
     """The last time the list was updated to add a new upcoming leap second"""
 
     def _check_validity(self, when: Optional[datetime.datetime]) -> Optional[str]:
         if when is None:
-            when = datetime.datetime.utcnow().replace(tzinfo=datetime.timezone.utc)
+            when = datetime.datetime.now(datetime.timezone.utc)
         if not self.valid_until:
             return "Data validity unknown"
         if when > self.valid_until:
             return f"Data only valid until {self.valid_until:%Y-%m-%d}"
         return None
 
     def valid(self, when: Optional[datetime.datetime] = None) -> bool:
@@ -248,21 +248,21 @@
         """
         with open(filename, "rb") as open_file:  # pragma no cover
             return cls.from_open_file(open_file, check_hash)
 
     @classmethod
     def from_url(
         cls,
-        url: str = "https://www.ietf.org/timezones/data/leap-seconds.list",
+        url: str = "https://raw.githubusercontent.com/eggert/tz/main/leap-seconds.list",
         check_hash: bool = True,
     ) -> Optional[LeapSecondData]:
         """Retrieve the leap second list from a local file
 
         :param filename: URL to read leap second data from.  The
-            default is maintained by the IETF
+            default is maintained by the tzdata authors
         :param check_hash: Whether to check the embedded hash
         """
         try:
             with urllib.request.urlopen(url) as open_file:
                 return cls.from_open_file(open_file, check_hash)
         except urllib.error.URLError:  # pragma no cover
             return None
```

### Comparing `leapseconddata-2.1.1/leapseconddata/__main__.py` & `leapseconddata-2.2.0/leapseconddata/__main__.py`

 * *Files identical despite different names*

### Comparing `leapseconddata-2.1.1/leapseconddata.egg-info/PKG-INFO` & `leapseconddata-2.2.0/leapseconddata.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: leapseconddata
-Version: 2.1.1
+Version: 2.2.0
 Summary: Use the list of known and scheduled leap seconds
 Home-page: https://github.com/jepler/leapseconddata
 Author: Jeff Epler
 Author-email: jepler@gmail.com
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 <!--
 SPDX-FileCopyrightText: 2021 Jeff Epler
 
 SPDX-License-Identifier: GPL-3.0-only
 -->
```

### Comparing `leapseconddata-2.1.1/leapseconddata.egg-info/SOURCES.txt` & `leapseconddata-2.2.0/leapseconddata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `leapseconddata-2.1.1/setup.cfg` & `leapseconddata-2.2.0/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -4,28 +4,27 @@
 author_email = jepler@gmail.com
 description = Use the list of known and scheduled leap seconds
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jepler/leapseconddata
 classifiers = 
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3.12
 	Programming Language :: Python :: Implementation :: PyPy
 	Programming Language :: Python :: Implementation :: CPython
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	=.
-python_requires = >=3.8
+python_requires = >=3.9
 packages = leapseconddata
 
 [options.package_data]
 leapseconddata = py.typed
 
 [egg_info]
 tag_build =
```

### Comparing `leapseconddata-2.1.1/testleapseconddata.py` & `leapseconddata-2.2.0/testleapseconddata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 
 # SPDX-FileCopyrightText: 2021 Jeff Epler
 #
 # SPDX-License-Identifier: GPL-3.0-only
 
 """Test most leapseconddata functionality"""
+
 # pylint: disable=missing-class-docstring,missing-function-docstring
 import datetime
 import unittest
 
 import leapseconddata
 import leapseconddata.__main__
```

