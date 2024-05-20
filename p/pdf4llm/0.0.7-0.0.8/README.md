# Comparing `tmp/pdf4llm-0.0.7.tar.gz` & `tmp/pdf4llm-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf4llm-0.0.7.tar", last modified: Sat Apr 27 10:55:17 2024, max compression
+gzip compressed data, was "pdf4llm-0.0.8.tar", last modified: Mon May 20 17:49:34 2024, max compression
```

## Comparing `pdf4llm-0.0.7.tar` & `pdf4llm-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 10:55:17.601847 pdf4llm-0.0.7/
--rw-rw-rw-   0        0        0     1740 2024-04-27 10:55:17.600848 pdf4llm-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1226 2024-04-24 14:40:20.000000 pdf4llm-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-27 10:55:17.585338 pdf4llm-0.0.7/pdf4llm/
--rw-rw-rw-   0        0        0       46 2024-04-22 23:14:44.000000 pdf4llm-0.0.7/pdf4llm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 10:55:17.599848 pdf4llm-0.0.7/pdf4llm/helpers/
--rw-rw-rw-   0        0        0    14027 2024-04-27 10:43:44.000000 pdf4llm-0.0.7/pdf4llm/helpers/pymupdf_rag.py
-drwxrwxrwx   0        0        0        0 2024-04-27 10:55:17.600848 pdf4llm-0.0.7/pdf4llm.egg-info/
--rw-rw-rw-   0        0        0     1740 2024-04-27 10:55:17.000000 pdf4llm-0.0.7/pdf4llm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2024-04-27 10:55:17.000000 pdf4llm-0.0.7/pdf4llm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 10:55:17.000000 pdf4llm-0.0.7/pdf4llm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-27 10:55:17.000000 pdf4llm-0.0.7/pdf4llm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-27 10:55:17.000000 pdf4llm-0.0.7/pdf4llm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-27 10:55:17.601847 pdf4llm-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      967 2024-04-27 10:54:38.000000 pdf4llm-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:49:34.646766 pdf4llm-0.0.8/
+-rw-rw-rw-   0        0        0     3819 2024-05-20 17:49:34.645765 pdf4llm-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3309 2024-05-20 17:16:21.000000 pdf4llm-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 17:49:34.631770 pdf4llm-0.0.8/pdf4llm/
+-rw-rw-rw-   0        0        0      307 2024-05-12 15:22:14.000000 pdf4llm-0.0.8/pdf4llm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:49:34.644765 pdf4llm-0.0.8/pdf4llm.egg-info/
+-rw-rw-rw-   0        0        0     3819 2024-05-20 17:49:34.000000 pdf4llm-0.0.8/pdf4llm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2024-05-20 17:49:34.000000 pdf4llm-0.0.8/pdf4llm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 17:49:34.000000 pdf4llm-0.0.8/pdf4llm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-20 17:49:34.000000 pdf4llm-0.0.8/pdf4llm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-20 17:49:34.000000 pdf4llm-0.0.8/pdf4llm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 17:49:34.646766 pdf4llm-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      947 2024-05-12 13:48:05.000000 pdf4llm-0.0.8/setup.py
```

### Comparing `pdf4llm-0.0.7/setup.py` & `pdf4llm-0.0.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
     "Topic :: Utilities",
 ]
-requires = ["pymupdf>=1.24.2"]
+requires = ["pymupdf4llm"]
 
 setuptools.setup(
     name="pdf4llm",
-    version="0.0.7",
+    version="0.0.8",
     author="Artifex",
     author_email="support@artifex.com",
     description="PyMuPDF Utilities for LLM/RAG",
     packages=setuptools.find_packages(),
     long_description=readme,
     long_description_content_type="text/markdown",
     install_requires=requires,
     license="GNU AFFERO GPL 3.0",
     url="https://github.com/pymupdf/RAG",
     classifiers=classifiers,
     project_urls={},
     package_data={
-        "pdf4llm": ["LICENSE", "helpers/*.py"],
+        "pdf4llm": ["LICENSE"],
     },
 )
```

