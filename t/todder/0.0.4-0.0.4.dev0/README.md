# Comparing `tmp/todder-0.0.4.tar.gz` & `tmp/todder-0.0.4.dev0.tar.gz`

## Comparing `todder-0.0.4.tar` & `todder-0.0.4.dev0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 todder-0.0.4/.codecov.yml
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 todder-0.0.4/.coveragerc
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 todder-0.0.4/.flake8
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 todder-0.0.4/.gitattributes
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 todder-0.0.4/.isort.cfg
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 todder-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 todder-0.0.4/pytest.ini
--rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 todder-0.0.4/.github/workflows/docs.yml
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 todder-0.0.4/.github/workflows/pre-commit.yml
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 todder-0.0.4/.github/workflows/publish-pypi.yml
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 todder-0.0.4/.github/workflows/testing.yml
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 todder-0.0.4/docs/Makefile
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 todder-0.0.4/docs/make.bat
--rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 todder-0.0.4/docs/source/conf.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 todder-0.0.4/docs/source/index.rst
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 todder-0.0.4/docs/source/installation.rst
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 todder-0.0.4/docs/source/release-history.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 todder-0.0.4/docs/source/_static/.placeholder
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 todder-0.0.4/todder/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 todder-0.0.4/todder/_version.py
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 todder-0.0.4/todder/signal.py
--rw-r--r--   0        0        0     8255 2020-02-02 00:00:00.000000 todder-0.0.4/todder/tod.py
--rw-r--r--   0        0        0    11662 2020-02-02 00:00:00.000000 todder-0.0.4/todder/coords/__init__.py
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 todder-0.0.4/todder/coords/transforms.py
--rw-r--r--   0        0        0    25325 2020-02-02 00:00:00.000000 todder-0.0.4/todder/instruments/__init__.py
--rw-r--r--   0        0        0     4678 2020-02-02 00:00:00.000000 todder-0.0.4/todder/instruments/act/__init__.py
--rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 todder-0.0.4/todder/instruments/act/della.py
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 todder-0.0.4/todder/instruments/atlast/__init__.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 todder-0.0.4/todder/instruments/mustang2/__init__.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 todder-0.0.4/todder/sim/__init__.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 todder-0.0.4/todder/sim/noise.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 todder-0.0.4/todder/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 todder-0.0.4/todder/tests/conftest.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 todder-0.0.4/todder/tests/test_tod.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 todder-0.0.4/.gitignore
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 todder-0.0.4/LICENSE
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 todder-0.0.4/README.rst
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 todder-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 todder-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 todder-0.0.4.dev0/.codecov.yml
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 todder-0.0.4.dev0/.coveragerc
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 todder-0.0.4.dev0/.flake8
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 todder-0.0.4.dev0/.gitattributes
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 todder-0.0.4.dev0/.isort.cfg
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 todder-0.0.4.dev0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 todder-0.0.4.dev0/pytest.ini
+-rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 todder-0.0.4.dev0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 todder-0.0.4.dev0/.github/workflows/pre-commit.yml
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 todder-0.0.4.dev0/.github/workflows/publish-pypi.yml
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 todder-0.0.4.dev0/.github/workflows/testing.yml
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 todder-0.0.4.dev0/docs/Makefile
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 todder-0.0.4.dev0/docs/make.bat
+-rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 todder-0.0.4.dev0/docs/source/conf.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 todder-0.0.4.dev0/docs/source/index.rst
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 todder-0.0.4.dev0/docs/source/installation.rst
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 todder-0.0.4.dev0/docs/source/release-history.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 todder-0.0.4.dev0/docs/source/_static/.placeholder
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 todder-0.0.4.dev0/todder/__init__.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 todder-0.0.4.dev0/todder/_version.py
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 todder-0.0.4.dev0/todder/signal.py
+-rw-r--r--   0        0        0     8255 2020-02-02 00:00:00.000000 todder-0.0.4.dev0/todder/tod.py
+-rw-r--r--   0        0        0    11662 2020-02-02 00:00:00.000000 todder-0.0.4.dev0/todder/coords/__init__.py
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 todder-0.0.4.dev0/todder/coords/transforms.py
+-rw-r--r--   0        0        0    25325 2020-02-02 00:00:00.000000 todder-0.0.4.dev0/todder/instruments/__init__.py
+-rw-r--r--   0        0        0     4678 2020-02-02 00:00:00.000000 todder-0.0.4.dev0/todder/instruments/act/__init__.py
+-rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 todder-0.0.4.dev0/todder/instruments/act/della.py
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 todder-0.0.4.dev0/todder/instruments/atlast/__init__.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 todder-0.0.4.dev0/todder/instruments/mustang2/__init__.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 todder-0.0.4.dev0/todder/sim/__init__.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 todder-0.0.4.dev0/todder/sim/noise.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 todder-0.0.4.dev0/todder/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 todder-0.0.4.dev0/todder/tests/conftest.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 todder-0.0.4.dev0/todder/tests/test_tod.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 todder-0.0.4.dev0/.gitignore
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 todder-0.0.4.dev0/LICENSE
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 todder-0.0.4.dev0/README.rst
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 todder-0.0.4.dev0/pyproject.toml
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 todder-0.0.4.dev0/PKG-INFO
```

### Comparing `todder-0.0.4/.pre-commit-config.yaml` & `todder-0.0.4.dev0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `todder-0.0.4/.github/workflows/docs.yml` & `todder-0.0.4.dev0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `todder-0.0.4/.github/workflows/publish-pypi.yml` & `todder-0.0.4.dev0/.github/workflows/publish-pypi.yml`

 * *Files identical despite different names*

### Comparing `todder-0.0.4/.github/workflows/testing.yml` & `todder-0.0.4.dev0/.github/workflows/testing.yml`

 * *Files identical despite different names*

### Comparing `todder-0.0.4/docs/Makefile` & `todder-0.0.4.dev0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `todder-0.0.4/docs/make.bat` & `todder-0.0.4.dev0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `todder-0.0.4/docs/source/conf.py` & `todder-0.0.4.dev0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `todder-0.0.4/todder/signal.py` & `todder-0.0.4.dev0/todder/signal.py`

 * *Files identical despite different names*

### Comparing `todder-0.0.4/todder/tod.py` & `todder-0.0.4.dev0/todder/tod.py`

 * *Files identical despite different names*

### Comparing `todder-0.0.4/todder/coords/__init__.py` & `todder-0.0.4.dev0/todder/coords/__init__.py`

 * *Files identical despite different names*

### Comparing `todder-0.0.4/todder/coords/transforms.py` & `todder-0.0.4.dev0/todder/coords/transforms.py`

 * *Files identical despite different names*

### Comparing `todder-0.0.4/todder/instruments/__init__.py` & `todder-0.0.4.dev0/todder/instruments/__init__.py`

 * *Files identical despite different names*

### Comparing `todder-0.0.4/todder/instruments/act/__init__.py` & `todder-0.0.4.dev0/todder/instruments/act/__init__.py`

 * *Files identical despite different names*

### Comparing `todder-0.0.4/todder/instruments/act/della.py` & `todder-0.0.4.dev0/todder/instruments/act/della.py`

 * *Files identical despite different names*

### Comparing `todder-0.0.4/todder/instruments/atlast/__init__.py` & `todder-0.0.4.dev0/todder/instruments/atlast/__init__.py`

 * *Files identical despite different names*

### Comparing `todder-0.0.4/todder/instruments/mustang2/__init__.py` & `todder-0.0.4.dev0/todder/instruments/mustang2/__init__.py`

 * *Files identical despite different names*

### Comparing `todder-0.0.4/todder/sim/__init__.py` & `todder-0.0.4.dev0/todder/sim/__init__.py`

 * *Files identical despite different names*

### Comparing `todder-0.0.4/todder/sim/noise.py` & `todder-0.0.4.dev0/todder/sim/noise.py`

 * *Files identical despite different names*

### Comparing `todder-0.0.4/todder/tests/test_tod.py` & `todder-0.0.4.dev0/todder/tests/test_tod.py`

 * *Files identical despite different names*

### Comparing `todder-0.0.4/.gitignore` & `todder-0.0.4.dev0/.gitignore`

 * *Files identical despite different names*

### Comparing `todder-0.0.4/LICENSE` & `todder-0.0.4.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `todder-0.0.4/pyproject.toml` & `todder-0.0.4.dev0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `todder-0.0.4/PKG-INFO` & `todder-0.0.4.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: todder
-Version: 0.0.4
+Version: 0.0.4.dev0
 Summary: Beamline optimization with machine learning
 Project-URL: Homepage, https://github.com/thomaswmorris/todder
 Project-URL: Bug Reports, https://github.com/thomaswmorris/todder/issues
 Author-email: "Thomas W. Morris" <thomas.w.morris@yale.edu>
 Maintainer-email: "Thomas W. Morris" <thomas.w.morris@yale.edu>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
@@ -45,8 +45,8 @@
 Requires-Dist: sphinx-rtd-theme; extra == 'dev'
 Requires-Dist: twine; extra == 'dev'
 Description-Content-Type: text/x-rst
 
 maria
 =====
 
-``maria`` is a package for manipulating time-ordered astronomical data.
+``maria`` is a package for manipulating time-ordered astronomical data.
```

