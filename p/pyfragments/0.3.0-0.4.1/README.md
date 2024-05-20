# Comparing `tmp/pyfragments-0.3.0.tar.gz` & `tmp/pyfragments-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfragments-0.3.0.tar", last modified: Tue Jan  9 09:59:26 2024, max compression
+gzip compressed data, was "pyfragments-0.4.1.tar", last modified: Mon May 20 15:34:03 2024, max compression
```

## Comparing `pyfragments-0.3.0.tar` & `pyfragments-0.4.1.tar`

### file list

```diff
@@ -1,32 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 09:59:26.185483 pyfragments-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-09 09:59:13.000000 pyfragments-0.3.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 09:59:26.181483 pyfragments-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 09:59:26.181483 pyfragments-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-01-09 09:59:13.000000 pyfragments-0.3.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-01-09 09:59:13.000000 pyfragments-0.3.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-01-09 09:59:13.000000 pyfragments-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-01-09 09:59:13.000000 pyfragments-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-01-09 09:59:13.000000 pyfragments-0.3.0/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-01-09 09:59:13.000000 pyfragments-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-01-09 09:59:26.185483 pyfragments-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-01-09 09:59:13.000000 pyfragments-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 09:59:26.185483 pyfragments-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)    43638 2024-01-09 09:59:13.000000 pyfragments-0.3.0/docs/animated_figure.gif
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-09 09:59:13.000000 pyfragments-0.3.0/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 09:59:26.185483 pyfragments-0.3.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-01-09 09:59:13.000000 pyfragments-0.3.0/examples/animated_figure.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-01-09 09:59:13.000000 pyfragments-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-09 09:59:13.000000 pyfragments-0.3.0/requirements.test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-09 09:59:13.000000 pyfragments-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-09 09:59:26.185483 pyfragments-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 09:59:26.181483 pyfragments-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 09:59:26.185483 pyfragments-0.3.0/src/pyfragments/
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-01-09 09:59:13.000000 pyfragments-0.3.0/src/pyfragments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 09:59:26.185483 pyfragments-0.3.0/src/pyfragments/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-01-09 09:59:13.000000 pyfragments-0.3.0/src/pyfragments/tests/test_warning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 09:59:26.185483 pyfragments-0.3.0/src/pyfragments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-01-09 09:59:26.000000 pyfragments-0.3.0/src/pyfragments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-01-09 09:59:26.000000 pyfragments-0.3.0/src/pyfragments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-09 09:59:26.000000 pyfragments-0.3.0/src/pyfragments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-09 09:59:26.000000 pyfragments-0.3.0/src/pyfragments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-09 09:59:26.000000 pyfragments-0.3.0/src/pyfragments.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:34:03.987287 pyfragments-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-20 15:33:59.000000 pyfragments-0.4.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:34:03.979287 pyfragments-0.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:34:03.983287 pyfragments-0.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-20 15:33:59.000000 pyfragments-0.4.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-20 15:33:59.000000 pyfragments-0.4.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-20 15:33:59.000000 pyfragments-0.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-20 15:33:59.000000 pyfragments-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-20 15:33:59.000000 pyfragments-0.4.1/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-20 15:33:59.000000 pyfragments-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-05-20 15:34:03.983287 pyfragments-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-20 15:33:59.000000 pyfragments-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:34:03.983287 pyfragments-0.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)    43638 2024-05-20 15:33:59.000000 pyfragments-0.4.1/docs/animated_figure.gif
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-20 15:33:59.000000 pyfragments-0.4.1/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:34:03.983287 pyfragments-0.4.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-20 15:33:59.000000 pyfragments-0.4.1/examples/animated_figure.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-20 15:33:59.000000 pyfragments-0.4.1/examples/animated_svg.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-20 15:33:59.000000 pyfragments-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-20 15:33:59.000000 pyfragments-0.4.1/requirements.test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-20 15:33:59.000000 pyfragments-0.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 15:34:03.987287 pyfragments-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:34:03.979287 pyfragments-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:34:03.983287 pyfragments-0.4.1/src/pyfragments/
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-05-20 15:33:59.000000 pyfragments-0.4.1/src/pyfragments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-20 15:33:59.000000 pyfragments-0.4.1/src/pyfragments/svg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:34:03.983287 pyfragments-0.4.1/src/pyfragments/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-20 15:33:59.000000 pyfragments-0.4.1/src/pyfragments/tests/test_svg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-20 15:33:59.000000 pyfragments-0.4.1/src/pyfragments/tests/test_warning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:34:03.983287 pyfragments-0.4.1/src/pyfragments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-05-20 15:34:03.000000 pyfragments-0.4.1/src/pyfragments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-20 15:34:03.000000 pyfragments-0.4.1/src/pyfragments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 15:34:03.000000 pyfragments-0.4.1/src/pyfragments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-20 15:34:03.000000 pyfragments-0.4.1/src/pyfragments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-20 15:34:03.000000 pyfragments-0.4.1/src/pyfragments.egg-info/top_level.txt
```

### Comparing `pyfragments-0.3.0/.github/workflows/publish.yml` & `pyfragments-0.4.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `pyfragments-0.3.0/.github/workflows/test.yml` & `pyfragments-0.4.1/.github/workflows/test.yml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
+        python-version: ["3.9", "3.10", "3.11", "3.12"]
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
```

### Comparing `pyfragments-0.3.0/.pre-commit-config.yaml` & `pyfragments-0.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyfragments-0.3.0/CHANGELOG` & `pyfragments-0.4.1/CHANGELOG`

 * *Files identical despite different names*

### Comparing `pyfragments-0.3.0/LICENSE` & `pyfragments-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfragments-0.3.0/docs/animated_figure.gif` & `pyfragments-0.4.1/docs/animated_figure.gif`

 * *Files identical despite different names*

### Comparing `pyfragments-0.3.0/pyproject.toml` & `pyfragments-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "pyfragments"
 authors = [
     { name="Mauro Silberberg", email="maurosilber@gmail.com" },
 ]
 description = "Add animations to revealjs presentations from Python code-blocks."
-requires-python = ">=3.7"
+requires-python = ">=3.9"
 keywords = [
     "quarto",
     "revealjs",
     "presentation",
     "fragments",
     "animations",
     "matplotlib",
```

### Comparing `pyfragments-0.3.0/src/pyfragments.egg-info/SOURCES.txt` & `pyfragments-0.4.1/src/pyfragments.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 pyproject.toml
 requirements.test.txt
 requirements.txt
 .github/workflows/publish.yml
 .github/workflows/test.yml
 docs/animated_figure.gif
 examples/animated_figure.qmd
+examples/animated_svg.qmd
 src/pyfragments/__init__.py
+src/pyfragments/svg.py
 src/pyfragments.egg-info/PKG-INFO
 src/pyfragments.egg-info/SOURCES.txt
 src/pyfragments.egg-info/dependency_links.txt
 src/pyfragments.egg-info/requires.txt
 src/pyfragments.egg-info/top_level.txt
+src/pyfragments/tests/test_svg.py
 src/pyfragments/tests/test_warning.py
```

