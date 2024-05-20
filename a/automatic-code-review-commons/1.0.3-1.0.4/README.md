# Comparing `tmp/automatic-code-review-commons-1.0.3.tar.gz` & `tmp/automatic-code-review-commons-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automatic-code-review-commons-1.0.3.tar", last modified: Mon May 20 16:24:23 2024, max compression
+gzip compressed data, was "automatic-code-review-commons-1.0.4.tar", last modified: Mon May 20 16:30:05 2024, max compression
```

## Comparing `automatic-code-review-commons-1.0.3.tar` & `automatic-code-review-commons-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 kielsondasilva  (1001) kielsonzinn  (1001)        0 2024-05-20 16:24:23.086134 automatic-code-review-commons-1.0.3/
--rw-r--r--   0 kielsondasilva  (1001) kielsonzinn  (1001)      935 2024-05-20 16:24:23.086134 automatic-code-review-commons-1.0.3/PKG-INFO
--rw-r--r--   0 kielsondasilva  (1001) kielsonzinn  (1001)      358 2024-05-20 16:19:34.000000 automatic-code-review-commons-1.0.3/README.md
-drwxr-xr-x   0 kielsondasilva  (1001) kielsonzinn  (1001)        0 2024-05-20 16:24:23.086134 automatic-code-review-commons-1.0.3/automatic_code_review_commons/
--rw-r--r--   0 kielsondasilva  (1001) kielsonzinn  (1001)       50 2024-05-20 16:23:55.000000 automatic-code-review-commons-1.0.3/automatic_code_review_commons/__init__.py
--rw-r--r--   0 kielsondasilva  (1001) kielsonzinn  (1001)      685 2024-05-20 16:23:41.000000 automatic-code-review-commons-1.0.3/automatic_code_review_commons/comment.py
--rw-r--r--   0 kielsondasilva  (1001) kielsonzinn  (1001)      372 2024-05-20 16:23:06.000000 automatic-code-review-commons-1.0.3/automatic_code_review_commons/review.py
-drwxr-xr-x   0 kielsondasilva  (1001) kielsonzinn  (1001)        0 2024-05-20 16:24:23.086134 automatic-code-review-commons-1.0.3/automatic_code_review_commons.egg-info/
--rw-r--r--   0 kielsondasilva  (1001) kielsonzinn  (1001)      935 2024-05-20 16:24:23.000000 automatic-code-review-commons-1.0.3/automatic_code_review_commons.egg-info/PKG-INFO
--rw-r--r--   0 kielsondasilva  (1001) kielsonzinn  (1001)      353 2024-05-20 16:24:23.000000 automatic-code-review-commons-1.0.3/automatic_code_review_commons.egg-info/SOURCES.txt
--rw-r--r--   0 kielsondasilva  (1001) kielsonzinn  (1001)        1 2024-05-20 16:24:23.000000 automatic-code-review-commons-1.0.3/automatic_code_review_commons.egg-info/dependency_links.txt
--rw-r--r--   0 kielsondasilva  (1001) kielsonzinn  (1001)       30 2024-05-20 16:24:23.000000 automatic-code-review-commons-1.0.3/automatic_code_review_commons.egg-info/top_level.txt
--rw-r--r--   0 kielsondasilva  (1001) kielsonzinn  (1001)       38 2024-05-20 16:24:23.086134 automatic-code-review-commons-1.0.3/setup.cfg
--rw-r--r--   0 kielsondasilva  (1001) kielsonzinn  (1001)      721 2024-05-20 16:24:01.000000 automatic-code-review-commons-1.0.3/setup.py
+drwxr-xr-x   0 kielsondasilva  (1001) kielsonzinn  (1001)        0 2024-05-20 16:30:05.766121 automatic-code-review-commons-1.0.4/
+-rw-r--r--   0 kielsondasilva  (1001) kielsonzinn  (1001)      935 2024-05-20 16:30:05.766121 automatic-code-review-commons-1.0.4/PKG-INFO
+-rw-r--r--   0 kielsondasilva  (1001) kielsonzinn  (1001)      358 2024-05-20 16:19:34.000000 automatic-code-review-commons-1.0.4/README.md
+drwxr-xr-x   0 kielsondasilva  (1001) kielsonzinn  (1001)        0 2024-05-20 16:30:05.766121 automatic-code-review-commons-1.0.4/automatic_code_review_commons/
+-rw-r--r--   0 kielsondasilva  (1001) kielsonzinn  (1001)      120 2024-05-20 16:29:32.000000 automatic-code-review-commons-1.0.4/automatic_code_review_commons/__init__.py
+-rw-r--r--   0 kielsondasilva  (1001) kielsonzinn  (1001)      685 2024-05-20 16:23:41.000000 automatic-code-review-commons-1.0.4/automatic_code_review_commons/comment.py
+-rw-r--r--   0 kielsondasilva  (1001) kielsonzinn  (1001)      372 2024-05-20 16:23:06.000000 automatic-code-review-commons-1.0.4/automatic_code_review_commons/review.py
+drwxr-xr-x   0 kielsondasilva  (1001) kielsonzinn  (1001)        0 2024-05-20 16:30:05.766121 automatic-code-review-commons-1.0.4/automatic_code_review_commons.egg-info/
+-rw-r--r--   0 kielsondasilva  (1001) kielsonzinn  (1001)      935 2024-05-20 16:30:05.000000 automatic-code-review-commons-1.0.4/automatic_code_review_commons.egg-info/PKG-INFO
+-rw-r--r--   0 kielsondasilva  (1001) kielsonzinn  (1001)      353 2024-05-20 16:30:05.000000 automatic-code-review-commons-1.0.4/automatic_code_review_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 kielsondasilva  (1001) kielsonzinn  (1001)        1 2024-05-20 16:30:05.000000 automatic-code-review-commons-1.0.4/automatic_code_review_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 kielsondasilva  (1001) kielsonzinn  (1001)       30 2024-05-20 16:30:05.000000 automatic-code-review-commons-1.0.4/automatic_code_review_commons.egg-info/top_level.txt
+-rw-r--r--   0 kielsondasilva  (1001) kielsonzinn  (1001)       38 2024-05-20 16:30:05.766121 automatic-code-review-commons-1.0.4/setup.cfg
+-rw-r--r--   0 kielsondasilva  (1001) kielsonzinn  (1001)      721 2024-05-20 16:29:57.000000 automatic-code-review-commons-1.0.4/setup.py
```

### Comparing `automatic-code-review-commons-1.0.3/PKG-INFO` & `automatic-code-review-commons-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automatic-code-review-commons
-Version: 1.0.3
+Version: 1.0.4
 Summary: Biblioteca com funções genéricas para revisões automáticas de código do projeto ACR
 Home-page: https://github.com/automatic-code-review/automatic-code-review-commons
 Author: Kielson Zinn da Silva
 Author-email: automatic.code.review@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `automatic-code-review-commons-1.0.3/automatic_code_review_commons/comment.py` & `automatic-code-review-commons-1.0.4/automatic_code_review_commons/comment.py`

 * *Files identical despite different names*

### Comparing `automatic-code-review-commons-1.0.3/automatic_code_review_commons.egg-info/PKG-INFO` & `automatic-code-review-commons-1.0.4/automatic_code_review_commons.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automatic-code-review-commons
-Version: 1.0.3
+Version: 1.0.4
 Summary: Biblioteca com funções genéricas para revisões automáticas de código do projeto ACR
 Home-page: https://github.com/automatic-code-review/automatic-code-review-commons
 Author: Kielson Zinn da Silva
 Author-email: automatic.code.review@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `automatic-code-review-commons-1.0.3/setup.py` & `automatic-code-review-commons-1.0.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='automatic-code-review-commons',
-    version='1.0.3',
+    version='1.0.4',
     packages=find_packages(),
     description='Biblioteca com funções genéricas para revisões automáticas de código do projeto ACR',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Kielson Zinn da Silva',
     author_email='automatic.code.review@gmail.com',
     url='https://github.com/automatic-code-review/automatic-code-review-commons',
```

