# Comparing `tmp/vizbeauty-0.0.1.tar.gz` & `tmp/VizBeauty-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vizbeauty-0.0.1.tar", last modified: Mon May 20 13:31:37 2024, max compression
+gzip compressed data, was "VizBeauty-0.1.0.tar", last modified: Mon May  6 02:30:17 2024, max compression
```

## Comparing `vizbeauty-0.0.1.tar` & `VizBeauty-0.1.0.tar`

### file list

```diff
@@ -1,52 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:31:37.423210 vizbeauty-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:31:37.415209 vizbeauty-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:31:37.415209 vizbeauty-0.0.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:31:37.419209 vizbeauty-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-20 13:31:37.423210 vizbeauty-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:31:37.419209 vizbeauty-0.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:31:37.419209 vizbeauty-0.0.1/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:31:37.419209 vizbeauty-0.0.1/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/docs/vizbeauty.md
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 13:31:37.423210 vizbeauty-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:31:37.419209 vizbeauty-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/tests/test_vizbeauty.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:31:37.419209 vizbeauty-0.0.1/vizbeauty/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/vizbeauty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/vizbeauty/common.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-20 13:31:26.000000 vizbeauty-0.0.1/vizbeauty/vizbeauty.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:31:37.419209 vizbeauty-0.0.1/vizbeauty.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-20 13:31:37.000000 vizbeauty-0.0.1/vizbeauty.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-20 13:31:37.000000 vizbeauty-0.0.1/vizbeauty.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 13:31:37.000000 vizbeauty-0.0.1/vizbeauty.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-20 13:31:37.000000 vizbeauty-0.0.1/vizbeauty.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-20 13:31:37.000000 vizbeauty-0.0.1/vizbeauty.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 13:31:37.000000 vizbeauty-0.0.1/vizbeauty.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 02:30:17.745726 VizBeauty-0.1.0/
+-rw-rw-rw-   0        0        0      183 2024-05-05 21:20:19.000000 VizBeauty-0.1.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3889 2024-05-05 21:20:20.000000 VizBeauty-0.1.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2024-05-05 21:20:20.000000 VizBeauty-0.1.0/HISTORY.rst
+-rw-rw-rw-   0        0        0     1099 2024-05-05 21:20:20.000000 VizBeauty-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      273 2024-05-05 21:20:20.000000 VizBeauty-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2032 2024-05-06 02:30:17.744347 VizBeauty-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1090 2024-05-05 21:20:20.000000 VizBeauty-0.1.0/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-06 02:30:17.716705 VizBeauty-0.1.0/docs/
+-rw-rw-rw-   0        0        0      630 2024-05-05 21:20:20.000000 VizBeauty-0.1.0/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2024-05-05 21:20:20.000000 VizBeauty-0.1.0/docs/authors.rst
+-rw-rw-rw-   0        0        0     4984 2024-05-05 21:20:20.000000 VizBeauty-0.1.0/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2024-05-05 21:20:20.000000 VizBeauty-0.1.0/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2024-05-05 21:20:20.000000 VizBeauty-0.1.0/docs/history.rst
+-rw-rw-rw-   0        0        0      326 2024-05-05 21:20:20.000000 VizBeauty-0.1.0/docs/index.rst
+-rw-rw-rw-   0        0        0     1181 2024-05-05 21:20:20.000000 VizBeauty-0.1.0/docs/installation.rst
+-rwxrwxrwx   0        0        0      807 2024-05-05 21:20:20.000000 VizBeauty-0.1.0/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2024-05-05 21:20:20.000000 VizBeauty-0.1.0/docs/readme.rst
+-rw-rw-rw-   0        0        0       80 2024-05-05 21:20:20.000000 VizBeauty-0.1.0/docs/usage.rst
+-rw-rw-rw-   0        0        0     1410 2024-05-05 21:20:20.000000 VizBeauty-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-06 02:30:17.745726 VizBeauty-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      267 2024-05-06 02:27:55.000000 VizBeauty-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 02:30:17.649937 VizBeauty-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-06 02:30:17.742939 VizBeauty-0.1.0/src/VizBeauty.egg-info/
+-rw-rw-rw-   0        0        0     2032 2024-05-06 02:30:17.000000 VizBeauty-0.1.0/src/VizBeauty.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      444 2024-05-06 02:30:17.000000 VizBeauty-0.1.0/src/VizBeauty.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 02:30:17.000000 VizBeauty-0.1.0/src/VizBeauty.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-05-06 02:30:17.000000 VizBeauty-0.1.0/src/VizBeauty.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 02:30:17.000000 VizBeauty-0.1.0/src/VizBeauty.egg-info/top_level.txt
```

### Comparing `vizbeauty-0.0.1/LICENSE` & `VizBeauty-0.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-MIT License
-
-Copyright (c) 2024, Cristian Del Gobbo
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
+MIT License
+
+Copyright (c) 2024, Cristian Del Gobbo
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
```

