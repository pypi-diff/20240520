# Comparing `tmp/pymupdf4llm-0.0.1.tar.gz` & `tmp/pymupdf4llm-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymupdf4llm-0.0.1.tar", last modified: Wed Apr 24 21:16:57 2024, max compression
+gzip compressed data, was "pymupdf4llm-0.0.2.tar", last modified: Mon May 20 17:49:14 2024, max compression
```

## Comparing `pymupdf4llm-0.0.1.tar` & `pymupdf4llm-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 21:16:57.969547 pymupdf4llm-0.0.1/
--rw-rw-rw-   0        0        0     1748 2024-04-24 21:16:57.968547 pymupdf4llm-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2024-04-24 14:40:43.000000 pymupdf4llm-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 21:16:57.960547 pymupdf4llm-0.0.1/pymupdf4llm/
--rw-rw-rw-   0        0        0       23 2024-04-23 23:25:53.000000 pymupdf4llm-0.0.1/pymupdf4llm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 21:16:57.967548 pymupdf4llm-0.0.1/pymupdf4llm.egg-info/
--rw-rw-rw-   0        0        0     1748 2024-04-24 21:16:57.000000 pymupdf4llm-0.0.1/pymupdf4llm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2024-04-24 21:16:57.000000 pymupdf4llm-0.0.1/pymupdf4llm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 21:16:57.000000 pymupdf4llm-0.0.1/pymupdf4llm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-24 21:16:57.000000 pymupdf4llm-0.0.1/pymupdf4llm.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-24 21:16:57.000000 pymupdf4llm-0.0.1/pymupdf4llm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 21:16:57.969547 pymupdf4llm-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      951 2024-04-24 21:16:30.000000 pymupdf4llm-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:49:14.225876 pymupdf4llm-0.0.2/
+-rw-rw-rw-   0        0        0     3855 2024-05-20 17:49:14.224877 pymupdf4llm-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3337 2024-05-20 17:05:17.000000 pymupdf4llm-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 17:49:14.198456 pymupdf4llm-0.0.2/pymupdf4llm/
+-rw-rw-rw-   0        0        0      324 2024-05-20 15:12:18.000000 pymupdf4llm-0.0.2/pymupdf4llm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:49:14.221884 pymupdf4llm-0.0.2/pymupdf4llm/helpers/
+-rw-rw-rw-   0        0        0     7512 2024-05-19 10:51:18.000000 pymupdf4llm-0.0.2/pymupdf4llm/helpers/get_text_lines.py
+-rw-rw-rw-   0        0        0    12436 2024-05-18 13:33:50.000000 pymupdf4llm-0.0.2/pymupdf4llm/helpers/multi_column.py
+-rw-rw-rw-   0        0        0    18225 2024-05-20 16:58:12.000000 pymupdf4llm-0.0.2/pymupdf4llm/helpers/pymupdf_rag.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:49:14.222876 pymupdf4llm-0.0.2/pymupdf4llm/llama/
+-rw-rw-rw-   0        0        0     5048 2024-05-20 15:16:25.000000 pymupdf4llm-0.0.2/pymupdf4llm/llama/pdf_markdown_reader.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:49:14.223876 pymupdf4llm-0.0.2/pymupdf4llm.egg-info/
+-rw-rw-rw-   0        0        0     3855 2024-05-20 17:49:14.000000 pymupdf4llm-0.0.2/pymupdf4llm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2024-05-20 17:49:14.000000 pymupdf4llm-0.0.2/pymupdf4llm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 17:49:14.000000 pymupdf4llm-0.0.2/pymupdf4llm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-20 17:49:14.000000 pymupdf4llm-0.0.2/pymupdf4llm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-20 17:49:14.000000 pymupdf4llm-0.0.2/pymupdf4llm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 17:49:14.225876 pymupdf4llm-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      989 2024-05-12 11:59:16.000000 pymupdf4llm-0.0.2/setup.py
```

### Comparing `pymupdf4llm-0.0.1/setup.py` & `pymupdf4llm-0.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
     "Topic :: Utilities",
 ]
-requires = ["pdf4llm"]
+requires = ["pymupdf>=1.24.2"]
 
 setuptools.setup(
     name="pymupdf4llm",
-    version="0.0.1",
+    version="0.0.2",
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
-        "pymupdf4llm": ["LICENSE"],
+        "pymupdf4llm": ["LICENSE", "helpers/*.py", "llama/*.py"],
     },
 )
```

