# Comparing `tmp/surrogates_interface-4.0.1.tar.gz` & `tmp/surrogates_interface-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surrogates_interface-4.0.1.tar", max compression
+gzip compressed data, was "surrogates_interface-4.0.2.tar", max compression
```

## Comparing `surrogates_interface-4.0.1.tar` & `surrogates_interface-4.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1216 2023-12-07 09:21:40.491435 surrogates_interface-4.0.1/LICENSE
--rw-r--r--   0        0        0     1116 2023-12-02 14:41:25.303916 surrogates_interface-4.0.1/README.md
--rw-r--r--   0        0        0     3997 2024-03-06 15:21:21.017036 surrogates_interface-4.0.1/pyproject.toml
--rw-r--r--   0        0        0       78 2023-12-02 14:41:25.303916 surrogates_interface-4.0.1/surrogates_interface/__init__.py
--rw-r--r--   0        0        0     3030 2023-12-02 14:41:25.303916 surrogates_interface-4.0.1/surrogates_interface/domains.py
--rw-r--r--   0        0        0    15656 2024-03-19 14:36:15.132939 surrogates_interface-4.0.1/surrogates_interface/openmdao.py
--rw-r--r--   0        0        0    39224 2024-03-19 14:36:15.132939 surrogates_interface-4.0.1/surrogates_interface/surrogates.py
--rw-r--r--   0        0        0        0 2024-05-16 14:05:51.285549 surrogates_interface-4.0.1/surrogates_interface/test/__init__.py
--rw-r--r--   0        0        0     1253 2023-12-02 14:41:25.303916 surrogates_interface-4.0.1/surrogates_interface/test/test_domains.py
--rw-r--r--   0        0        0      335 2023-12-02 14:41:25.303916 surrogates_interface-4.0.1/surrogates_interface/test/test_init.py
--rw-r--r--   0        0        0     4831 2024-01-31 07:42:59.693005 surrogates_interface-4.0.1/surrogates_interface/test/test_pca_jacobian.py
--rw-r--r--   0        0        0     7294 2023-12-02 14:41:25.303916 surrogates_interface-4.0.1/surrogates_interface/test/test_smt.py
--rw-r--r--   0        0        0      560 2023-12-02 14:41:25.303916 surrogates_interface-4.0.1/surrogates_interface/test/test_surrogates.py
--rw-r--r--   0        0        0    43482 2024-02-06 15:01:57.159128 surrogates_interface-4.0.1/surrogates_interface/test/test_tensorflow_and_openmdao.py
--rw-r--r--   0        0        0    22766 2023-12-18 15:41:08.368739 surrogates_interface-4.0.1/surrogates_interface/test/test_transformers.py
--rw-r--r--   0        0        0    29506 2024-03-19 14:36:15.132939 surrogates_interface-4.0.1/surrogates_interface/transformers.py
--rw-r--r--   0        0        0     4374 1970-01-01 00:00:00.000000 surrogates_interface-4.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1216 2023-12-07 09:21:40.491435 surrogates_interface-4.0.2/LICENSE
+-rw-r--r--   0        0        0     1116 2023-12-02 14:41:25.303916 surrogates_interface-4.0.2/README.md
+-rw-r--r--   0        0        0     2858 2024-05-20 09:50:37.854339 surrogates_interface-4.0.2/pyproject.toml
+-rw-r--r--   0        0        0       78 2023-12-02 14:41:25.303916 surrogates_interface-4.0.2/surrogates_interface/__init__.py
+-rw-r--r--   0        0        0     3030 2023-12-02 14:41:25.303916 surrogates_interface-4.0.2/surrogates_interface/domains.py
+-rw-r--r--   0        0        0    15656 2024-03-19 14:36:15.132939 surrogates_interface-4.0.2/surrogates_interface/openmdao.py
+-rw-r--r--   0        0        0    39224 2024-03-19 14:36:15.132939 surrogates_interface-4.0.2/surrogates_interface/surrogates.py
+-rw-r--r--   0        0        0        0 2024-05-20 12:11:13.044710 surrogates_interface-4.0.2/surrogates_interface/test/__init__.py
+-rw-r--r--   0        0        0     1253 2023-12-02 14:41:25.303916 surrogates_interface-4.0.2/surrogates_interface/test/test_domains.py
+-rw-r--r--   0        0        0      335 2023-12-02 14:41:25.303916 surrogates_interface-4.0.2/surrogates_interface/test/test_init.py
+-rw-r--r--   0        0        0     4831 2024-01-31 07:42:59.693005 surrogates_interface-4.0.2/surrogates_interface/test/test_pca_jacobian.py
+-rw-r--r--   0        0        0     7294 2023-12-02 14:41:25.303916 surrogates_interface-4.0.2/surrogates_interface/test/test_smt.py
+-rw-r--r--   0        0        0      560 2023-12-02 14:41:25.303916 surrogates_interface-4.0.2/surrogates_interface/test/test_surrogates.py
+-rw-r--r--   0        0        0    43482 2024-02-06 15:01:57.159128 surrogates_interface-4.0.2/surrogates_interface/test/test_tensorflow_and_openmdao.py
+-rw-r--r--   0        0        0    22766 2023-12-18 15:41:08.368739 surrogates_interface-4.0.2/surrogates_interface/test/test_transformers.py
+-rw-r--r--   0        0        0    29506 2024-03-19 14:36:15.132939 surrogates_interface-4.0.2/surrogates_interface/transformers.py
+-rw-r--r--   0        0        0     3659 1970-01-01 00:00:00.000000 surrogates_interface-4.0.2/PKG-INFO
```

### Comparing `surrogates_interface-4.0.1/LICENSE` & `surrogates_interface-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `surrogates_interface-4.0.1/README.md` & `surrogates_interface-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `surrogates_interface-4.0.1/surrogates_interface/domains.py` & `surrogates_interface-4.0.2/surrogates_interface/domains.py`

 * *Files identical despite different names*

### Comparing `surrogates_interface-4.0.1/surrogates_interface/openmdao.py` & `surrogates_interface-4.0.2/surrogates_interface/openmdao.py`

 * *Files identical despite different names*

### Comparing `surrogates_interface-4.0.1/surrogates_interface/surrogates.py` & `surrogates_interface-4.0.2/surrogates_interface/surrogates.py`

 * *Files identical despite different names*

### Comparing `surrogates_interface-4.0.1/surrogates_interface/test/test_domains.py` & `surrogates_interface-4.0.2/surrogates_interface/test/test_domains.py`

 * *Files identical despite different names*

### Comparing `surrogates_interface-4.0.1/surrogates_interface/test/test_pca_jacobian.py` & `surrogates_interface-4.0.2/surrogates_interface/test/test_pca_jacobian.py`

 * *Files identical despite different names*

### Comparing `surrogates_interface-4.0.1/surrogates_interface/test/test_smt.py` & `surrogates_interface-4.0.2/surrogates_interface/test/test_smt.py`

 * *Files identical despite different names*

### Comparing `surrogates_interface-4.0.1/surrogates_interface/test/test_surrogates.py` & `surrogates_interface-4.0.2/surrogates_interface/test/test_surrogates.py`

 * *Files identical despite different names*

### Comparing `surrogates_interface-4.0.1/surrogates_interface/test/test_tensorflow_and_openmdao.py` & `surrogates_interface-4.0.2/surrogates_interface/test/test_tensorflow_and_openmdao.py`

 * *Files identical despite different names*

### Comparing `surrogates_interface-4.0.1/surrogates_interface/test/test_transformers.py` & `surrogates_interface-4.0.2/surrogates_interface/test/test_transformers.py`

 * *Files identical despite different names*

### Comparing `surrogates_interface-4.0.1/surrogates_interface/transformers.py` & `surrogates_interface-4.0.2/surrogates_interface/transformers.py`

 * *Files identical despite different names*

### Comparing `surrogates_interface-4.0.1/PKG-INFO` & `surrogates_interface-4.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,52 @@
 Metadata-Version: 2.1
 Name: surrogates_interface
-Version: 4.0.1
+Version: 4.0.2
 Summary: Interface for surrogate models.
 Home-page: https://gitlab.windenergy.dtu.dk/surrogate-models/surrogate-models-interface
 License: MIT
 Author: DTU Wind and Energy Systems
 Maintainer: Riccardo Riva
 Maintainer-email: ricriv@dtu.dk
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: all
 Provides-Extra: code-style
 Provides-Extra: docs
 Provides-Extra: om
 Provides-Extra: smt
 Provides-Extra: test
 Provides-Extra: tf
-Requires-Dist: black ; extra == "all" or extra == "code-style"
-Requires-Dist: codespell ; extra == "all" or extra == "code-style"
-Requires-Dist: flake8 ; extra == "all" or extra == "code-style"
+Requires-Dist: black ; extra == "code-style"
+Requires-Dist: codespell ; extra == "code-style"
+Requires-Dist: flake8 ; extra == "code-style"
 Requires-Dist: h5py
-Requires-Dist: isort ; extra == "all" or extra == "code-style"
-Requires-Dist: matplotlib ; extra == "all" or extra == "test" or extra == "smt"
+Requires-Dist: isort ; extra == "code-style"
+Requires-Dist: matplotlib ; extra == "test" or extra == "smt"
 Requires-Dist: numpy (>=1.10.0)
-Requires-Dist: numpydoc ; extra == "all" or extra == "docs"
-Requires-Dist: openmdao (>=3.25,<4.0) ; extra == "all" or extra == "docs" or extra == "test" or extra == "om"
-Requires-Dist: pydata-sphinx-theme ; extra == "all" or extra == "docs"
-Requires-Dist: pytest ; extra == "all" or extra == "test"
-Requires-Dist: pytest-cov ; extra == "all" or extra == "test"
-Requires-Dist: pytest-testmon ; extra == "all" or extra == "test"
-Requires-Dist: scikit-learn ; extra == "all" or extra == "test" or extra == "smt" or extra == "tf"
-Requires-Dist: smt (>=2.0.1,<3.0.0) ; extra == "all" or extra == "test" or extra == "smt"
-Requires-Dist: sphinx ; extra == "all" or extra == "docs"
-Requires-Dist: sphinx-copybutton ; extra == "all" or extra == "docs"
-Requires-Dist: sphinx-sitemap ; extra == "all" or extra == "docs"
-Requires-Dist: tensorflow (>=2.10.0,<2.11) ; (platform_system == "Windows") and (extra == "all" or extra == "test" or extra == "tf")
-Requires-Dist: tensorflow (>=2.10.0,<3.0.0) ; (platform_system != "Windows") and (extra == "all" or extra == "test" or extra == "tf")
-Requires-Dist: tensorflow-cpu (>=2.10.0,<3.0.0) ; (platform_machine != "arm64" and platform_machine != "aarch64") and sys_platform == "darwin"
-Requires-Dist: tensorflow-cpu (>=2.10.0,<3.0.0) ; (platform_machine != "arm64" and platform_machine != "aarch64") and sys_platform == "linux"
-Requires-Dist: tensorflow-cpu-aws (>=2.10.0,<3.0.0) ; (platform_machine == "arm64" or platform_machine == "aarch64") and sys_platform == "linux"
-Requires-Dist: tensorflow-intel (>=2.10.0,<3.0.0) ; sys_platform == "win32"
-Requires-Dist: tensorflow-io-gcs-filesystem (<0.32.0) ; platform_system == "Windows"
-Requires-Dist: tensorflow-io-gcs-filesystem (>=0.23.1) ; platform_machine != "arm64" or platform_system != "Darwin"
-Requires-Dist: tensorflow-macos (>=2.10.0,<3.0.0) ; platform_machine == "arm64" and sys_platform == "darwin"
-Requires-Dist: tomli (>=2.0.1,<3.0.0) ; (python_version < "3.11") and (extra == "all" or extra == "test")
+Requires-Dist: numpydoc ; extra == "docs"
+Requires-Dist: openmdao (>=3.25,<4.0) ; extra == "docs" or extra == "test" or extra == "om"
+Requires-Dist: pydata-sphinx-theme ; extra == "docs"
+Requires-Dist: pytest ; extra == "test"
+Requires-Dist: pytest-cov ; extra == "test"
+Requires-Dist: pytest-testmon ; extra == "test"
+Requires-Dist: scikit-learn ; extra == "test" or extra == "smt" or extra == "tf"
+Requires-Dist: smt (>=2.0.1,<3.0.0) ; extra == "test" or extra == "smt"
+Requires-Dist: sphinx ; extra == "docs"
+Requires-Dist: sphinx-copybutton ; extra == "docs"
+Requires-Dist: sphinx-sitemap ; extra == "docs"
+Requires-Dist: sphinx_design ; extra == "docs"
+Requires-Dist: tensorflow (>=2.10.0,<3.0.0) ; extra == "test" or extra == "tf"
+Requires-Dist: tensorflow-intel (>=2.10.0,<3.0.0) ; (sys_platform == "win32") and (extra == "test" or extra == "tf")
+Requires-Dist: tensorflow-io-gcs-filesystem (<0.32.0) ; (python_version >= "3.9" and python_version < "3.12" and platform_system == "Windows") and (extra == "test" or extra == "tf")
+Requires-Dist: tensorflow-io-gcs-filesystem (>=0.23.1) ; (platform_machine != "arm64" and python_version >= "3.9" and python_version < "3.12" or platform_system != "Darwin" and python_version >= "3.9" and python_version < "3.12") and (extra == "test" or extra == "tf")
+Requires-Dist: tomli (>=2.0.1,<3.0.0) ; (python_version < "3.11") and (extra == "test")
 Project-URL: Repository, https://gitlab.windenergy.dtu.dk/surrogate-models/surrogate-models-interface
 Description-Content-Type: text/markdown
 
 # Surrogate Models Interface
 
 [![pipeline status](https://gitlab.windenergy.dtu.dk/surrogate-models/surrogate-models-interface/badges/main/pipeline.svg)](https://gitlab.windenergy.dtu.dk/surrogate-models/surrogate-models-interface/-/commits/main)
 [![coverage report](https://gitlab.windenergy.dtu.dk/surrogate-models/surrogate-models-interface/badges/main/coverage.svg)](https://gitlab.windenergy.dtu.dk/surrogate-models/surrogate-models-interface/-/commits/main)
```

