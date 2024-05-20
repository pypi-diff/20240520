# Comparing `tmp/fao56-1.1.0.tar.gz` & `tmp/fao56-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fao56-1.1.0.tar", last modified: Wed Mar 29 09:11:16 2023, max compression
+gzip compressed data, was "fao56-1.2.0.tar", last modified: Mon May 20 07:27:34 2024, max compression
```

## Comparing `fao56-1.1.0.tar` & `fao56-1.2.0.tar`

### file list

```diff
@@ -1,53 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-03-29 09:11:16.319718 fao56-1.1.0/
--rw-rw-rw-   0        0        0      316 2023-03-29 08:46:00.000000 fao56-1.1.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3273 2023-03-29 08:46:00.000000 fao56-1.1.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0      106 2023-03-29 08:46:00.000000 fao56-1.1.0/HISTORY.rst
--rw-rw-rw-   0        0        0    20838 2023-03-29 08:46:00.000000 fao56-1.1.0/LICENSE
--rw-rw-rw-   0        0        0      433 2023-03-29 08:46:00.000000 fao56-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1954 2023-03-29 09:11:16.320718 fao56-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1151 2023-03-29 08:46:00.000000 fao56-1.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-29 09:11:16.152596 fao56-1.1.0/doc/
--rw-rw-rw-   0        0        0     6967 2023-03-29 08:46:00.000000 fao56-1.1.0/doc/Makefile
--rw-rw-rw-   0        0        0       29 2023-03-29 08:46:00.000000 fao56-1.1.0/doc/authors.rst
-drwxrwxrwx   0        0        0        0 2023-03-29 09:11:16.155642 fao56-1.1.0/doc/badges/
--rw-rw-rw-   0        0        0      282 2023-03-29 08:46:00.000000 fao56-1.1.0/doc/badges/listing.rst
-drwxrwxrwx   0        0        0        0 2023-03-29 09:11:16.167644 fao56-1.1.0/doc/biblio/
--rw-rw-rw-   0        0        0      513 2023-03-29 08:46:00.000000 fao56-1.1.0/doc/biblio/biblio.rst
--rw-rw-rw-   0        0        0     5072 2023-03-29 08:46:00.000000 fao56-1.1.0/doc/conf.py
--rw-rw-rw-   0        0        0       34 2023-03-29 08:46:00.000000 fao56-1.1.0/doc/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-03-29 08:46:00.000000 fao56-1.1.0/doc/history.rst
--rw-rw-rw-   0        0        0      585 2023-03-29 08:46:00.000000 fao56-1.1.0/doc/index.rst
--rw-rw-rw-   0        0        0      215 2023-03-29 08:46:00.000000 fao56-1.1.0/doc/installation.rst
--rwxrwxrwx   0        0        0     6731 2023-03-29 08:46:00.000000 fao56-1.1.0/doc/make.bat
--rw-rw-rw-   0        0        0      133 2023-03-29 08:46:00.000000 fao56-1.1.0/doc/management.rst
--rw-rw-rw-   0        0        0     1021 2023-03-29 08:46:00.000000 fao56-1.1.0/doc/readme.rst
--rw-rw-rw-   0        0        0       21 2023-03-29 08:46:00.000000 fao56-1.1.0/doc/usage.rst
-drwxrwxrwx   0        0        0        0 2023-03-29 09:11:16.180645 fao56-1.1.0/doc/user/
--rw-rw-rw-   0        0        0       86 2023-03-29 08:46:00.000000 fao56-1.1.0/doc/user/index.rst
--rw-rw-rw-   0        0        0       66 2023-03-29 08:46:00.000000 fao56-1.1.0/doc/user/overview.rst
--rw-rw-rw-   0        0        0      286 2023-03-29 08:46:00.000000 fao56-1.1.0/requirements.txt
--rw-rw-rw-   0        0        0       29 2023-03-29 08:46:00.000000 fao56-1.1.0/requirements_minimal.txt
--rw-rw-rw-   0        0        0      187 2023-03-29 09:11:16.330721 fao56-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1886 2023-03-29 08:46:00.000000 fao56-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-29 09:11:16.051509 fao56-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-03-29 09:11:16.214644 fao56-1.1.0/src/fao56/
--rw-rw-rw-   0        0        0      287 2023-03-29 08:46:00.000000 fao56-1.1.0/src/fao56/__init__.py
--rw-rw-rw-   0        0        0      824 2021-12-10 15:38:21.000000 fao56-1.1.0/src/fao56/chap2.py
--rw-rw-rw-   0        0        0     5812 2021-12-13 11:56:03.000000 fao56-1.1.0/src/fao56/chap3.py
--rw-rw-rw-   0        0        0     1091 2021-12-10 15:55:43.000000 fao56-1.1.0/src/fao56/chap4.py
--rw-rw-rw-   0        0        0     6662 2023-03-29 08:42:19.000000 fao56-1.1.0/src/fao56/clean.py
--rw-rw-rw-   0        0        0      367 2023-03-29 08:46:00.000000 fao56-1.1.0/src/fao56/version.py
-drwxrwxrwx   0        0        0        0 2023-03-29 09:11:16.266719 fao56-1.1.0/src/fao56.egg-info/
--rw-rw-rw-   0        0        0     1954 2023-03-29 09:11:15.000000 fao56-1.1.0/src/fao56.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      826 2023-03-29 09:11:16.000000 fao56-1.1.0/src/fao56.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-29 09:11:15.000000 fao56-1.1.0/src/fao56.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-12-10 15:16:45.000000 fao56-1.1.0/src/fao56.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2023-03-29 09:11:15.000000 fao56-1.1.0/src/fao56.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-29 09:11:16.313754 fao56-1.1.0/test/
--rw-rw-rw-   0        0        0     1680 2019-01-29 08:24:00.000000 fao56-1.1.0/test/climate.csv
--rw-rw-rw-   0        0        0      969 2023-03-29 08:46:00.000000 fao56-1.1.0/test/conftest.py
--rw-rw-rw-   0        0        0      557 2017-08-24 15:50:14.000000 fao56-1.1.0/test/etp_table_chap4_fig18.txt
--rw-rw-rw-   0        0        0     1519 2019-01-29 08:24:00.000000 fao56-1.1.0/test/retrieve_weather.py
--rw-rw-rw-   0        0        0     2512 2021-12-13 10:22:08.000000 fao56-1.1.0/test/test_chap3.py
--rw-rw-rw-   0        0        0     4622 2021-12-14 09:13:38.000000 fao56-1.1.0/test/test_clean.py
--rw-rw-rw-   0        0        0       76 2023-03-29 08:46:00.000000 fao56-1.1.0/test/test_packaging.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:27:34.030409 fao56-1.2.0/
+-rw-rw-rw-   0        0        0      316 2024-05-20 07:24:00.000000 fao56-1.2.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3273 2024-05-20 07:24:00.000000 fao56-1.2.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0      106 2024-05-20 07:24:00.000000 fao56-1.2.0/HISTORY.rst
+-rw-rw-rw-   0        0        0    20838 2024-05-20 07:24:00.000000 fao56-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     2687 2024-05-20 07:27:34.030409 fao56-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1097 2024-05-20 07:24:00.000000 fao56-1.2.0/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-20 07:27:33.999189 fao56-1.2.0/doc/
+-rw-rw-rw-   0        0        0     6967 2024-05-20 07:24:00.000000 fao56-1.2.0/doc/Makefile
+-rw-rw-rw-   0        0        0       29 2024-05-20 07:24:00.000000 fao56-1.2.0/doc/authors.rst
+drwxrwxrwx   0        0        0        0 2024-05-20 07:27:33.999189 fao56-1.2.0/doc/badges/
+-rw-rw-rw-   0        0        0      282 2024-05-20 07:24:00.000000 fao56-1.2.0/doc/badges/listing.rst
+drwxrwxrwx   0        0        0        0 2024-05-20 07:27:34.004198 fao56-1.2.0/doc/biblio/
+-rw-rw-rw-   0        0        0      513 2024-05-20 07:24:00.000000 fao56-1.2.0/doc/biblio/biblio.rst
+-rw-rw-rw-   0        0        0     5072 2024-05-20 07:24:00.000000 fao56-1.2.0/doc/conf.py
+-rw-rw-rw-   0        0        0       34 2024-05-20 07:24:00.000000 fao56-1.2.0/doc/contributing.rst
+-rw-rw-rw-   0        0        0       29 2024-05-20 07:24:00.000000 fao56-1.2.0/doc/history.rst
+-rw-rw-rw-   0        0        0      585 2024-05-20 07:24:00.000000 fao56-1.2.0/doc/index.rst
+-rw-rw-rw-   0        0        0      215 2024-05-20 07:24:00.000000 fao56-1.2.0/doc/installation.rst
+-rwxrwxrwx   0        0        0     6731 2024-05-20 07:24:00.000000 fao56-1.2.0/doc/make.bat
+-rw-rw-rw-   0        0        0      133 2024-05-20 07:24:00.000000 fao56-1.2.0/doc/management.rst
+-rw-rw-rw-   0        0        0     1029 2024-05-20 07:24:00.000000 fao56-1.2.0/doc/readme.rst
+-rw-rw-rw-   0        0        0       21 2024-05-20 07:24:00.000000 fao56-1.2.0/doc/usage.rst
+drwxrwxrwx   0        0        0        0 2024-05-20 07:27:34.004198 fao56-1.2.0/doc/user/
+-rw-rw-rw-   0        0        0       86 2024-05-20 07:24:00.000000 fao56-1.2.0/doc/user/index.rst
+-rw-rw-rw-   0        0        0       66 2024-05-20 07:24:00.000000 fao56-1.2.0/doc/user/overview.rst
+-rw-rw-rw-   0        0        0     2207 2024-05-20 07:24:00.000000 fao56-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0      286 2024-05-20 07:24:00.000000 fao56-1.2.0/requirements.txt
+-rw-rw-rw-   0        0        0       29 2024-05-20 07:24:00.000000 fao56-1.2.0/requirements_minimal.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 07:27:34.030409 fao56-1.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 07:27:33.964502 fao56-1.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-20 07:27:34.013762 fao56-1.2.0/src/fao56/
+-rw-rw-rw-   0        0        0      287 2024-05-20 07:24:00.000000 fao56-1.2.0/src/fao56/__init__.py
+-rw-rw-rw-   0        0        0      824 2021-12-10 15:38:21.000000 fao56-1.2.0/src/fao56/chap2.py
+-rw-rw-rw-   0        0        0     5812 2021-12-13 11:56:03.000000 fao56-1.2.0/src/fao56/chap3.py
+-rw-rw-rw-   0        0        0     1091 2021-12-10 15:55:43.000000 fao56-1.2.0/src/fao56/chap4.py
+-rw-rw-rw-   0        0        0     6662 2023-03-29 08:42:19.000000 fao56-1.2.0/src/fao56/clean.py
+-rw-rw-rw-   0        0        0      367 2024-05-20 07:24:00.000000 fao56-1.2.0/src/fao56/version.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:27:34.030409 fao56-1.2.0/src/fao56.egg-info/
+-rw-rw-rw-   0        0        0     2687 2024-05-20 07:27:33.000000 fao56-1.2.0/src/fao56.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      810 2024-05-20 07:27:33.000000 fao56-1.2.0/src/fao56.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 07:27:33.000000 fao56-1.2.0/src/fao56.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2024-05-20 07:27:33.000000 fao56-1.2.0/src/fao56.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-20 07:27:33.000000 fao56-1.2.0/src/fao56.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-20 07:27:34.030409 fao56-1.2.0/test/
+-rw-rw-rw-   0        0        0     1680 2019-01-29 08:24:00.000000 fao56-1.2.0/test/climate.csv
+-rw-rw-rw-   0        0        0      981 2024-05-20 07:24:00.000000 fao56-1.2.0/test/conftest.py
+-rw-rw-rw-   0        0        0      557 2017-08-24 15:50:14.000000 fao56-1.2.0/test/etp_table_chap4_fig18.txt
+-rw-rw-rw-   0        0        0     1519 2019-01-29 08:24:00.000000 fao56-1.2.0/test/retrieve_weather.py
+-rw-rw-rw-   0        0        0     2512 2021-12-13 10:22:08.000000 fao56-1.2.0/test/test_chap3.py
+-rw-rw-rw-   0        0        0     4622 2021-12-14 09:13:38.000000 fao56-1.2.0/test/test_clean.py
+-rw-rw-rw-   0        0        0      110 2024-05-20 07:24:00.000000 fao56-1.2.0/test/test_packaging.py
```

### Comparing `fao56-1.1.0/CONTRIBUTING.rst` & `fao56-1.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `fao56-1.1.0/LICENSE` & `fao56-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fao56-1.1.0/README.rst` & `fao56-1.2.0/doc/readme.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-========================
-fao56
-========================
+Overview
+========
 
-.. {# pkglts, doc
+.. {# pkglts, glabpkg_dev
 
 .. image:: https://b326.gitlab.io/fao56/_images/badge_pkging_pip.svg
     :alt: PyPI version
-    :target: https://pypi.org/project/fao56/1.1.0/
+    :target: https://pypi.org/project/fao56/1.2.0/
+
 
 .. image:: https://b326.gitlab.io/fao56/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/fao56
 
+
 .. image:: https://b326.gitlab.io/fao56/_images/badge_doc.svg
     :alt: Documentation status
     :target: https://b326.gitlab.io/fao56/
 
+
 .. image:: https://badge.fury.io/py/fao56.svg
     :alt: PyPI version
     :target: https://badge.fury.io/py/fao56
 
-.. #}
-.. {# pkglts, glabpkg_dev, after doc
+
+
 
 main: |main_build|_ |main_coverage|_
 
 .. |main_build| image:: https://gitlab.com/b326/fao56/badges/main/pipeline.svg
 .. _main_build: https://gitlab.com/b326/fao56/commits/main
 
 .. |main_coverage| image:: https://gitlab.com/b326/fao56/badges/main/coverage.svg
 .. _main_coverage: https://gitlab.com/b326/fao56/commits/main
 .. #}
 
 Data and formalisms from FAO56 related to crop evapotranspiration
-
-Reference: https://www.fao.org/3/x0490e/x0490e00.htm
```

### Comparing `fao56-1.1.0/doc/Makefile` & `fao56-1.2.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `fao56-1.1.0/doc/biblio/biblio.rst` & `fao56-1.2.0/doc/biblio/biblio.rst`

 * *Files identical despite different names*

### Comparing `fao56-1.1.0/doc/conf.py` & `fao56-1.2.0/doc/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,17 +85,17 @@
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 
 # The short X.Y version.
-version = "1.1.0"
+version = "1.2.0"
 # The full version, including alpha/beta/rc tags.
-release = "1.1.0"
+release = "1.2.0"
 
 
 exclude_patterns = ['build', 'dist']
 
 pygments_style = 'sphinx'
 
 # -- Options for HTML output -------------------------------------------
```

### Comparing `fao56-1.1.0/doc/index.rst` & `fao56-1.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `fao56-1.1.0/doc/make.bat` & `fao56-1.2.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `fao56-1.1.0/doc/readme.rst` & `fao56-1.2.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,36 @@
-Overview
-========
+========================
+fao56
+========================
 
-.. {# pkglts, glabpkg_dev
+.. {# pkglts, doc
 
 .. image:: https://b326.gitlab.io/fao56/_images/badge_pkging_pip.svg
     :alt: PyPI version
-    :target: https://pypi.org/project/fao56/1.1.0/
+    :target: https://pypi.org/project/fao56/1.2.0/
 
 .. image:: https://b326.gitlab.io/fao56/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/fao56
 
 .. image:: https://b326.gitlab.io/fao56/_images/badge_doc.svg
     :alt: Documentation status
     :target: https://b326.gitlab.io/fao56/
 
 .. image:: https://badge.fury.io/py/fao56.svg
     :alt: PyPI version
     :target: https://badge.fury.io/py/fao56
 
-
+.. #}
+.. {# pkglts, glabpkg_dev, after doc
 
 main: |main_build|_ |main_coverage|_
 
 .. |main_build| image:: https://gitlab.com/b326/fao56/badges/main/pipeline.svg
 .. _main_build: https://gitlab.com/b326/fao56/commits/main
 
 .. |main_coverage| image:: https://gitlab.com/b326/fao56/badges/main/coverage.svg
 .. _main_coverage: https://gitlab.com/b326/fao56/commits/main
 .. #}
 
 Data and formalisms from FAO56 related to crop evapotranspiration
+
```

### Comparing `fao56-1.1.0/setup.py` & `fao56-1.2.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,72 +1,86 @@
-# {# pkglts, pysetup.kwds
-# format setup arguments
-from pathlib import Path
-from setuptools import setup, find_packages
-
-short_descr = "Data and formalisms from FAO56 related to crop evapotranspiration"
-readme = open('README.rst').read()
-history = open('HISTORY.rst').read()
-
-# find packages
-pkgs = find_packages('src')
-
-src_dir = Path("src/fao56")
-
-data_files = []
-for pth in src_dir.rglob("*"):
-    if not pth.is_dir() and "__pycache__" not in pth.parts:
-        if pth.suffix in ['.json', '.ini', '.csv', '.rst', '.svg']:
-            data_files.append(str(pth.relative_to(src_dir)))
-
-pkg_data = {'fao56': data_files}
-
-setup_kwds = dict(
-    name='fao56',
-    version="1.1.0",
-    description=short_descr,
-    long_description=readme + '\n\n' + history,
-    author="revesansparole",
-    author_email="revesansparole@gmail.com",
-    url='https://gitlab.com/b326/fao56',
-    license='cc_by_nc',
-    zip_safe=False,
-
-    packages=pkgs,
-    
-    package_dir={'': 'src'},
-    
-    
-    package_data=pkg_data,
-    setup_requires=[
-        "pytest-runner",
-        ],
-    install_requires=[
-        ],
-    tests_require=[
-        "coverage",
-        "pandas",
-        "pytest",
-        "pytest-cov",
-        "pytest-mock",
-        ],
-    entry_points={},
-    keywords='',
-    
-    classifiers=[
-        "Development Status :: 2 - Pre-Alpha",
-        "Intended Audience :: Developers",
-        "License :: OSI Approved :: BSD License",
-        "Natural Language :: English",
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.9",
-    ],
-    )
+# {# pkglts, pyproject.build
+[build-system]
+# Minimum requirements for the build system to execute.
+requires = ["setuptools", "wheel"]  # , "setuptools-scm"]  # PEP 508 specifications.
+build-backend = "setuptools.build_meta"  # we don't know if we need it
 # #}
-# change setup_kwds below before the next pkglts tag
 
-# do not change things below
-# {# pkglts, pysetup.call
-setup(**setup_kwds)
+# {# pkglts, pyproject.project
+[project]  # https://packaging.python.org/en/latest/specifications/pyproject-toml/
+name = "fao56"
+version = "1.2.0"
+description = "Data and formalisms from FAO56 related to crop evapotranspiration"
+readme = "README.rst"
+requires-python = ">= 3.9"
+license = {text = "cc_by_nc"}
+authors = [
+    {name = "revesansparole", email = "revesansparole@gmail.com"},
+]
+maintainers = [
+    {name = "revesansparole", email = "revesansparole@gmail.com"},
+    {name = "Jerome Chopard", email = "revesansparole@gmail.com"},
+]
+keywords = [
+]
+classifiers = [
+    "Development Status :: 2 - Pre-Alpha",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: BSD License",
+    "Natural Language :: English",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: 3.9",
+]
+dependencies = [
+]
+
+[project.optional-dependencies]
+doc = [
+    "sphinx",
+    "sphinx-gallery",
+    "sphinx_rtd_theme",
+]
+dvlpt = [
+    "twine",
+]
+test = [
+    "coverage",
+    "pandas",
+    "pytest",
+    "pytest-cov",
+    "pytest-mock",
+]
+
+
+[project.urls]
+repository = "https://gitlab.com/b326/fao56"
+pip = "https://pypi.org/project/fao56/1.2.0/"
+conda = "https://anaconda.org/revesansparole/fao56"
+doc = "https://b326.gitlab.io/fao56/"
+pypi = "https://badge.fury.io/py/fao56"
+
+
+[tool.setuptools]
+include-package-data = true
+
+[tool.setuptools.packages.find]
+where = ["src"]
+
+[tool.setuptools.package-data]
+"*" = ['*.json', '*.ini', '*.csv', '*.rst', '*.svg', ]
+
+# #}
+# {# pkglts, test, after pyproject.project
+[tool.pytest.ini_options]
+addopts = "--maxfail=2 -rf --cov=fao56"
+# #}
+
+# {# pkglts, pyproject.scripts
+[project.scripts]
+# #}
+
+# {# pkglts, pyproject.gui_scripts
+[project.gui-scripts]
 # #}
```

### Comparing `fao56-1.1.0/src/fao56/chap2.py` & `fao56-1.2.0/src/fao56/chap2.py`

 * *Files identical despite different names*

### Comparing `fao56-1.1.0/src/fao56/chap3.py` & `fao56-1.2.0/src/fao56/chap3.py`

 * *Files identical despite different names*

### Comparing `fao56-1.1.0/src/fao56/chap4.py` & `fao56-1.2.0/src/fao56/chap4.py`

 * *Files identical despite different names*

### Comparing `fao56-1.1.0/src/fao56/clean.py` & `fao56-1.2.0/src/fao56/clean.py`

 * *Files identical despite different names*

### Comparing `fao56-1.1.0/src/fao56.egg-info/SOURCES.txt` & `fao56-1.2.0/src/fao56.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 AUTHORS.rst
 CONTRIBUTING.rst
 HISTORY.rst
 LICENSE
-MANIFEST.in
 README.rst
+pyproject.toml
 requirements.txt
 requirements_minimal.txt
-setup.cfg
-setup.py
 doc/Makefile
 doc/authors.rst
 doc/conf.py
 doc/contributing.rst
 doc/history.rst
 doc/index.rst
 doc/installation.rst
@@ -28,15 +26,15 @@
 src/fao56/chap3.py
 src/fao56/chap4.py
 src/fao56/clean.py
 src/fao56/version.py
 src/fao56.egg-info/PKG-INFO
 src/fao56.egg-info/SOURCES.txt
 src/fao56.egg-info/dependency_links.txt
-src/fao56.egg-info/not-zip-safe
+src/fao56.egg-info/requires.txt
 src/fao56.egg-info/top_level.txt
 test/climate.csv
 test/conftest.py
 test/etp_table_chap4_fig18.txt
 test/retrieve_weather.py
 test/test_chap3.py
 test/test_clean.py
```

### Comparing `fao56-1.1.0/test/climate.csv` & `fao56-1.2.0/test/climate.csv`

 * *Files identical despite different names*

### Comparing `fao56-1.1.0/test/conftest.py` & `fao56-1.2.0/test/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 import os
 
 import pytest
 # #}
 
 
 # {# pkglts, test.pytest_cmdline_preparse
-def pytest_cmdline_preparse(args):
-    if 'PYCHARM_HOSTED' not in os.environ:
-        args.append("--cov=fao56")
+# def pytest_cmdline_preparse(args):
+#
+#     if 'PYCHARM_HOSTED' not in os.environ:
+#         args.append("--cov=fao56")
+#
 # #}
 
 
 # {# pkglts, test.pytest_addoption
 def pytest_addoption(parser):
     parser.addoption("--runslow", action="store_true",
                      default=False, help="run slow tests")
```

### Comparing `fao56-1.1.0/test/etp_table_chap4_fig18.txt` & `fao56-1.2.0/test/etp_table_chap4_fig18.txt`

 * *Files identical despite different names*

### Comparing `fao56-1.1.0/test/retrieve_weather.py` & `fao56-1.2.0/test/retrieve_weather.py`

 * *Files identical despite different names*

### Comparing `fao56-1.1.0/test/test_chap3.py` & `fao56-1.2.0/test/test_chap3.py`

 * *Files identical despite different names*

### Comparing `fao56-1.1.0/test/test_clean.py` & `fao56-1.2.0/test/test_clean.py`

 * *Files identical despite different names*

