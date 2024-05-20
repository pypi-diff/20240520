# Comparing `tmp/fileformats_medimage_afni-0.2.2.post186034.tar.gz` & `tmp/fileformats_medimage_afni-0.3.1.tar.gz`

## Comparing `fileformats_medimage_afni-0.2.2.post186034.tar` & `fileformats_medimage_afni-0.3.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 fileformats_medimage_afni-0.2.2.post186034/fileformats/medimage_afni/__init__.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 fileformats_medimage_afni-0.2.2.post186034/fileformats/medimage_afni/_version.py
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 fileformats_medimage_afni-0.2.2.post186034/.gitignore
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fileformats_medimage_afni-0.2.2.post186034/LICENSE
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 fileformats_medimage_afni-0.2.2.post186034/README.rst
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 fileformats_medimage_afni-0.2.2.post186034/pyproject.toml
--rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 fileformats_medimage_afni-0.2.2.post186034/PKG-INFO
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 fileformats_medimage_afni-0.3.1/fileformats/medimage_afni/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fileformats_medimage_afni-0.3.1/fileformats/medimage_afni/_version.py
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 fileformats_medimage_afni-0.3.1/.gitignore
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fileformats_medimage_afni-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 fileformats_medimage_afni-0.3.1/README.rst
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 fileformats_medimage_afni-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3782 2020-02-02 00:00:00.000000 fileformats_medimage_afni-0.3.1/PKG-INFO
```

### Comparing `fileformats_medimage_afni-0.2.2.post186034/.gitignore` & `fileformats_medimage_afni-0.3.1/.gitignore`

 * *Files 19% similar despite different names*

```diff
@@ -127,20 +127,16 @@
 
 # Pyre type checker
 .pyre/
 
 # Pycharm
 .idea
 
-# Vim
-.*.sw[op]
-
 # VS Code
 .vscode
 
 # Mac garbarge
 .DS_store
 
 /pydra/tasks/afni/auto
 /pydra/tasks/afni/_version.py
-/related-packages/fileformats/fileformats/medimage_afni/_version.py
-/related-packages/fileformats-extras/fileformats/extras/medimage_afni/_version.py
+/related-packages/**/_version.py
```

### Comparing `fileformats_medimage_afni-0.2.2.post186034/LICENSE` & `fileformats_medimage_afni-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_afni-0.2.2.post186034/pyproject.toml` & `fileformats_medimage_afni-0.3.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "fileformats-medimage-afni"
 description = "Classes for representing different file formats in Python classes for use in type hinting in data workflows"
 readme = "README.rst"
 requires-python = ">=3.8"
-dependencies = ["fileformats", "fileformats-medimage"]
+dependencies = ["fileformats >= 0.4", "fileformats-medimage >= 0.2"]
 license = { file = "LICENSE" }
 authors = [{ name = "Thomas G. Close", email = "tom.g.close@gmail.com" }]
 maintainers = [{ name = "Thomas G. Close", email = "tom.g.close@gmail.com" }]
 keywords = ["file formats", "data"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
```

### Comparing `fileformats_medimage_afni-0.2.2.post186034/PKG-INFO` & `fileformats_medimage_afni-0.3.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fileformats-medimage-afni
-Version: 0.2.2.post186034
+Version: 0.3.1
 Summary: Classes for representing different file formats in Python classes for use in type hinting in data workflows
 Project-URL: repository, https://github.com/nipype/pydra-afni
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License:    Copyright 2021 Nipype developers
         
            Licensed under the Apache License, Version 2.0 (the "License");
@@ -29,47 +29,57 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
-Requires-Dist: fileformats
-Requires-Dist: fileformats-medimage
+Requires-Dist: fileformats-medimage>=0.2
+Requires-Dist: fileformats>=0.4
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: codespell; extra == 'dev'
 Requires-Dist: flake8; extra == 'dev'
 Requires-Dist: flake8-pyproject; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: codecov; extra == 'test'
 Requires-Dist: fileformats-medimage-afni-extras; extra == 'test'
 Requires-Dist: pytest-cov>=2.12.1; extra == 'test'
 Requires-Dist: pytest-env>=0.6.2; extra == 'test'
 Requires-Dist: pytest>=6.2.5; extra == 'test'
 Description-Content-Type: text/x-rst
 
-FileFormats Medimage/AFNI
-=========================
+How to customise this template
+==============================
 
-.. image:: https://github.com/nipype/pydra-afni/actions/workflows/ci-cd.yaml/badge.svg
-   :target: https://github.com/nipype/pydra-afni/actions/workflows/ci-cd.yaml
+#. Rename the `related-packages/fileformats/afni` directory to the name of the fileformats subpackage (e.g. `medimage_fsl`)
+#. Search and replace "afni" with the name of the fileformats subpackage the extras are to be added
+#. Replace name + email placeholders in `pyproject.toml` for developers and maintainers
+#. Add the extension file-format classes
+#. Ensure that all the extension file-format classes are imported into the extras package root, i.e. `fileformats/afni`
+#. Delete these instructions
+
+...
+
+FileFormats Extension - afni
+====================================
+.. image:: https://github.com/nipype/pydra-afni/actions/workflows/ci-cd.yml/badge.svg
+    :target: https://github.com/nipype/pydra-afni/actions/workflows/ci-cd.yml
 
-
-This is the AFNI extension module for the
-`fileformats <https://github.com/ArcanaFramework/fileformats>`__ package
+This is the "afni" extension module for the
+`fileformats <https://github.com/ArcanaFramework/fileformats-core>`__ package
 
 
 Quick Installation
 ------------------
 
 This extension can be installed for Python 3 using *pip*::
 
-    $ pip3 install fileformats-medimage-afni
+    $ pip3 install fileformats-afni
 
 This will install the core package and any other dependencies
 
 License
 -------
 
 This work is licensed under a
```

