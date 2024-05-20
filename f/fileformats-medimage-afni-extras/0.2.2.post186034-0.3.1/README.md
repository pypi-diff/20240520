# Comparing `tmp/fileformats_medimage_afni_extras-0.2.2.post186034.tar.gz` & `tmp/fileformats_medimage_afni_extras-0.3.1.tar.gz`

## Comparing `fileformats_medimage_afni_extras-0.2.2.post186034.tar` & `fileformats_medimage_afni_extras-0.3.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 fileformats_medimage_afni_extras-0.2.2.post186034/fileformats/extras/medimage_afni/__init__.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 fileformats_medimage_afni_extras-0.2.2.post186034/fileformats/extras/medimage_afni/_version.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 fileformats_medimage_afni_extras-0.2.2.post186034/fileformats/extras/medimage_afni/tests/test_generate_sample_data.py
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 fileformats_medimage_afni_extras-0.2.2.post186034/.gitignore
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fileformats_medimage_afni_extras-0.2.2.post186034/LICENSE
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 fileformats_medimage_afni_extras-0.2.2.post186034/README.rst
--rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 fileformats_medimage_afni_extras-0.2.2.post186034/pyproject.toml
--rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 fileformats_medimage_afni_extras-0.2.2.post186034/PKG-INFO
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 fileformats_medimage_afni_extras-0.3.1/fileformats/extras/medimage_afni/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fileformats_medimage_afni_extras-0.3.1/fileformats/extras/medimage_afni/_version.py
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 fileformats_medimage_afni_extras-0.3.1/fileformats/extras/medimage_afni/tests/test_generate_sample_data.py
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 fileformats_medimage_afni_extras-0.3.1/.gitignore
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fileformats_medimage_afni_extras-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 fileformats_medimage_afni_extras-0.3.1/README.rst
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 fileformats_medimage_afni_extras-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 fileformats_medimage_afni_extras-0.3.1/PKG-INFO
```

### Comparing `fileformats_medimage_afni_extras-0.2.2.post186034/fileformats/extras/medimage_afni/__init__.py` & `fileformats_medimage_afni_extras-0.3.1/fileformats/extras/medimage_afni/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,61 +1,60 @@
-from ._version import __version__  # noqa: F401
-from pathlib import Path
 import typing as ty
-from random import Random
+from pathlib import Path
 from fileformats.core import FileSet, SampleFileGenerator
 from fileformats.medimage_afni import (
     OneD,
+    Dset,
+    ThreeD,
     Head,
-    All1,
+    NCorr,
     R1,
-    ThreeD,
-    Dset,
+    All1,
 )
+from ._version import __version__
 
 
 @FileSet.generate_sample_data.register
 def gen_sample_oned_data(
-    oned: OneD,
-    generator: SampleFileGenerator,
+    oned: OneD, generator: SampleFileGenerator
 ) -> ty.Iterable[Path]:
     raise NotImplementedError
 
 
 @FileSet.generate_sample_data.register
-def gen_sample_head_data(
-    head: Head,
-    generator: SampleFileGenerator,
+def gen_sample_dset_data(
+    dset: Dset, generator: SampleFileGenerator
 ) -> ty.Iterable[Path]:
     raise NotImplementedError
 
 
 @FileSet.generate_sample_data.register
-def gen_sample_all1_data(
-    all1: All1,
-    generator: SampleFileGenerator,
+def gen_sample_threed_data(
+    threed: ThreeD, generator: SampleFileGenerator
 ) -> ty.Iterable[Path]:
     raise NotImplementedError
 
 
 @FileSet.generate_sample_data.register
-def gen_sample_r1_data(
-    r1: R1,
-    generator: SampleFileGenerator,
+def gen_sample_head_data(
+    head: Head, generator: SampleFileGenerator
 ) -> ty.Iterable[Path]:
     raise NotImplementedError
 
 
 @FileSet.generate_sample_data.register
-def gen_sample_threed_data(
-    threed: ThreeD,
-    generator: SampleFileGenerator,
+def gen_sample_ncorr_data(
+    ncorr: NCorr, generator: SampleFileGenerator
 ) -> ty.Iterable[Path]:
     raise NotImplementedError
 
 
 @FileSet.generate_sample_data.register
-def gen_sample_dset_data(
-    dset: Dset,
-    generator: SampleFileGenerator,
+def gen_sample_r1_data(r1: R1, generator: SampleFileGenerator) -> ty.Iterable[Path]:
+    raise NotImplementedError
+
+
+@FileSet.generate_sample_data.register
+def gen_sample_all1_data(
+    all1: All1, generator: SampleFileGenerator
 ) -> ty.Iterable[Path]:
     raise NotImplementedError
```

### Comparing `fileformats_medimage_afni_extras-0.2.2.post186034/fileformats/extras/medimage_afni/tests/test_generate_sample_data.py` & `fileformats_medimage_afni_extras-0.3.1/fileformats/extras/medimage_afni/tests/test_generate_sample_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,45 @@
 import pytest
 from fileformats.medimage_afni import (
     OneD,
+    Dset,
     ThreeD,
+    Head,
+    NCorr,
     R1,
     All1,
-    Dset,
-    Head,
 )
 
 
 @pytest.mark.xfail(reason="generate_sample_data not implemented")
-def test_generate_sample_oned_data():
+def test_generate_one_d_data():
     assert isinstance(OneD.sample(), OneD)
 
 
 @pytest.mark.xfail(reason="generate_sample_data not implemented")
-def test_generate_sample_threed_data():
+def test_generate_three_d_data():
     assert isinstance(ThreeD.sample(), ThreeD)
 
 
 @pytest.mark.xfail(reason="generate_sample_data not implemented")
-def test_generate_sample_r1_data():
-    assert isinstance(R1.sample(), R1)
+def test_generate_dset_data():
+    assert isinstance(Dset.sample(), Dset)
 
 
 @pytest.mark.xfail(reason="generate_sample_data not implemented")
-def test_generate_sample_all1_data():
-    assert isinstance(All1.sample(), All1)
+def test_generate_head_data():
+    assert isinstance(Head.sample(), Head)
 
 
 @pytest.mark.xfail(reason="generate_sample_data not implemented")
-def test_generate_sample_dset_data():
-    assert isinstance(Dset.sample(), Dset)
+def test_generate_ncorr_data():
+    assert isinstance(NCorr.sample(), NCorr)
 
 
 @pytest.mark.xfail(reason="generate_sample_data not implemented")
-def test_generate_sample_head_data():
-    assert isinstance(Head.sample(), Head)
+def test_generate_r1_data():
+    assert isinstance(R1.sample(), R1)
+
+
+@pytest.mark.xfail(reason="generate_sample_data not implemented")
+def test_generate_all1_data():
+    assert isinstance(All1.sample(), All1)
```

### Comparing `fileformats_medimage_afni_extras-0.2.2.post186034/.gitignore` & `fileformats_medimage_afni_extras-0.3.1/.gitignore`

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

### Comparing `fileformats_medimage_afni_extras-0.2.2.post186034/LICENSE` & `fileformats_medimage_afni_extras-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_afni_extras-0.2.2.post186034/README.rst` & `fileformats_medimage_afni_extras-0.3.1/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-FileFormats Medimage/ANFI Extras
-================================
+FileFormats-afni Extras
+======================================
+.. image:: https://github.com/nipype/pydra-freesurfer/actions/workflows/ci-cd.yaml/badge.svg
+    :target: https://github.com/nipype/pydra-freesurfer/actions/workflows/ci-cd.yaml
 
-.. image:: https://github.com/nipype/pydra-afni/actions/workflows/ci-cd.yaml/badge.svg
-   :target: https://github.com/nipype/pydra-afni/actions/workflows/ci-cd.yaml
 
-
-This is a extras module for the `fileformats-medimage-afni <https://github.com/nipype/pydra-afni/>`__
+This is a extras module for the `fileformats-afni <https://github.com/nipype/pydra-freesurfer/>`__
 fileformats extension package, which provides additional functionality to format classes (i.e. aside
-from basic identification and validation), such as conversion tools, metadata parsers, sample data
-generators, etc...
+from basic identification and validation), such as conversion tools, metadata parsers, test data generators, etc...
 
 
 Quick Installation
 ------------------
 
 This extension can be installed for Python 3 using *pip*::
 
-    $ pip3 install fileformats-medimage-afni-extras
+    $ pip3 install fileformats-afni-extras
 
 This will install the core package and any other dependencies
 
 License
 -------
 
 This work is licensed under a
```

### Comparing `fileformats_medimage_afni_extras-0.2.2.post186034/pyproject.toml` & `fileformats_medimage_afni_extras-0.3.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
 [project]
 name = "fileformats-medimage-afni-extras"
 description = "Extensions to add functionality to tool-specific *fileformats* classes"
 readme = "README.rst"
 requires-python = ">=3.8"
 dependencies = [
-    "fileformats",
+    "fileformats >= 0.7",
     "fileformats-medimage-afni",
-    "pydra >= 0.23.0a"
+    "pydra >= 0.22.0"
 ]
 license = {file = "LICENSE"}
 authors = [
     {name = "Thomas G. Close", email = "tom.g.close@gmail.com"},
 ]
 maintainers = [
     {name = "Thomas G. Close", email = "tom.g.close@gmail.com"},
```

### Comparing `fileformats_medimage_afni_extras-0.2.2.post186034/PKG-INFO` & `fileformats_medimage_afni_extras-0.3.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fileformats-medimage-afni-extras
-Version: 0.2.2.post186034
+Version: 0.3.1
 Summary: Extensions to add functionality to tool-specific *fileformats* classes
 Project-URL: repository, https://github.com/nipype/pydra-afni
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License:    Copyright 2021 Nipype developers
         
            Licensed under the Apache License, Version 2.0 (the "License");
@@ -29,50 +29,48 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
-Requires-Dist: fileformats
 Requires-Dist: fileformats-medimage-afni
-Requires-Dist: pydra>=0.23.0a
+Requires-Dist: fileformats>=0.7
+Requires-Dist: pydra>=0.22.0
 Provides-Extra: converters
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: codespell; extra == 'dev'
 Requires-Dist: flake8; extra == 'dev'
 Requires-Dist: flake8-pyproject; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: codecov; extra == 'test'
 Requires-Dist: pytest-cov>=2.12.1; extra == 'test'
 Requires-Dist: pytest-env>=0.6.2; extra == 'test'
 Requires-Dist: pytest>=6.2.5; extra == 'test'
 Description-Content-Type: text/x-rst
 
-FileFormats Medimage/ANFI Extras
-================================
+FileFormats-afni Extras
+======================================
+.. image:: https://github.com/nipype/pydra-freesurfer/actions/workflows/ci-cd.yaml/badge.svg
+    :target: https://github.com/nipype/pydra-freesurfer/actions/workflows/ci-cd.yaml
 
-.. image:: https://github.com/nipype/pydra-afni/actions/workflows/ci-cd.yaml/badge.svg
-   :target: https://github.com/nipype/pydra-afni/actions/workflows/ci-cd.yaml
 
-
-This is a extras module for the `fileformats-medimage-afni <https://github.com/nipype/pydra-afni/>`__
+This is a extras module for the `fileformats-afni <https://github.com/nipype/pydra-freesurfer/>`__
 fileformats extension package, which provides additional functionality to format classes (i.e. aside
-from basic identification and validation), such as conversion tools, metadata parsers, sample data
-generators, etc...
+from basic identification and validation), such as conversion tools, metadata parsers, test data generators, etc...
 
 
 Quick Installation
 ------------------
 
 This extension can be installed for Python 3 using *pip*::
 
-    $ pip3 install fileformats-medimage-afni-extras
+    $ pip3 install fileformats-afni-extras
 
 This will install the core package and any other dependencies
 
 License
 -------
 
 This work is licensed under a
```

