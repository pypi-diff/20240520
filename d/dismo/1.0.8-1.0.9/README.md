# Comparing `tmp/dismo-1.0.8.tar.gz` & `tmp/dismo-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dismo-1.0.8.tar", max compression
+gzip compressed data, was "dismo-1.0.9.tar", max compression
```

## Comparing `dismo-1.0.8.tar` & `dismo-1.0.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35753 2024-01-01 02:07:02.029455 dismo-1.0.8/LICENSE
--rw-r--r--   0        0        0     2773 2024-01-01 02:07:02.029455 dismo-1.0.8/README.md
--rw-r--r--   0        0        0     1447 2024-01-01 02:07:02.031455 dismo-1.0.8/pyproject.toml
--rw-r--r--   0        0        0      381 2024-01-01 02:07:02.031455 dismo-1.0.8/src/dismo/__init__.py
--rw-r--r--   0        0        0    17601 2024-01-01 02:07:02.031455 dismo-1.0.8/src/dismo/coordinates.py
--rw-r--r--   0        0        0    12677 2024-01-01 02:07:02.031455 dismo-1.0.8/src/dismo/grids.py
--rw-r--r--   0        0        0    22763 2024-01-01 02:07:02.031455 dismo-1.0.8/src/dismo/models.py
--rw-r--r--   0        0        0     3594 1970-01-01 00:00:00.000000 dismo-1.0.8/setup.py
--rw-r--r--   0        0        0     3243 1970-01-01 00:00:00.000000 dismo-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0    35753 2024-01-08 02:06:21.656833 dismo-1.0.9/LICENSE
+-rw-r--r--   0        0        0     2773 2024-01-08 02:06:21.656833 dismo-1.0.9/README.md
+-rw-r--r--   0        0        0     1447 2024-01-08 02:06:21.657833 dismo-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0      381 2024-01-08 02:06:21.657833 dismo-1.0.9/src/dismo/__init__.py
+-rw-r--r--   0        0        0    17601 2024-01-08 02:06:21.658833 dismo-1.0.9/src/dismo/coordinates.py
+-rw-r--r--   0        0        0    12677 2024-01-08 02:06:21.658833 dismo-1.0.9/src/dismo/grids.py
+-rw-r--r--   0        0        0    22763 2024-01-08 02:06:21.658833 dismo-1.0.9/src/dismo/models.py
+-rw-r--r--   0        0        0     3594 1970-01-01 00:00:00.000000 dismo-1.0.9/setup.py
+-rw-r--r--   0        0        0     3243 1970-01-01 00:00:00.000000 dismo-1.0.9/PKG-INFO
```

### Comparing `dismo-1.0.8/LICENSE` & `dismo-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dismo-1.0.8/README.md` & `dismo-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dismo-1.0.8/pyproject.toml` & `dismo-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dismo"
-version = "1.0.8"
+version = "1.0.9"
 description = "A subpackage of modelbase that enables investigation of PDE models"
 authors = ["Marvin van Aalst <marvin.vanaalst@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "dismo", from = "src" }
 ]
```

### Comparing `dismo-1.0.8/src/dismo/coordinates.py` & `dismo-1.0.9/src/dismo/coordinates.py`

 * *Files identical despite different names*

### Comparing `dismo-1.0.8/src/dismo/grids.py` & `dismo-1.0.9/src/dismo/grids.py`

 * *Files identical despite different names*

### Comparing `dismo-1.0.8/src/dismo/models.py` & `dismo-1.0.9/src/dismo/models.py`

 * *Files identical despite different names*

### Comparing `dismo-1.0.8/setup.py` & `dismo-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.8,<4.0', 'numpy>=1.26,<2.0', 'pandas>=2.1,<3.0']
 
 setup_kwargs = {
     'name': 'dismo',
-    'version': '1.0.8',
+    'version': '1.0.9',
     'description': 'A subpackage of modelbase that enables investigation of PDE models',
     'long_description': '# DIscrete Spatial MOdels\n\n[![pipeline status](https://gitlab.com/qtb-hhu/dismo/badges/main/pipeline.svg)](https://gitlab.com/qtb-hhu/dismo/-/commits/main)\n[![coverage report](https://gitlab.com/qtb-hhu/dismo/badges/main/coverage.svg)](https://gitlab.com/qtb-hhu/dismo/-/commits/main)\n[![Documentation](https://img.shields.io/badge/Documentation-Gitlab-success)](https://qtb-hhu.gitlab.io/dismo/)\n[![PyPi](https://img.shields.io/pypi/v/dismo)](https://pypi.org/project/dismo/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)\n[![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)\n[![Downloads](https://pepy.tech/badge/dismo)](https://pepy.tech/project/dismo)\n\ndismo is a Python package for building and analysing discrete spatial models based on ordinary differential equations.\nIts primary purpose is to allow arbitrarily complex internal and transport processes to easily be mapped over multiple different regular grids.\nFor this it features one, two and three-dimensional layouts, with standard and non-standard (e.g. hexagonal or triangular) grids.\n\n\n## Installation\n\nIf you quickly want to test out dismo, or do not require assimulo support, install dismo via\n\n```bash\npip install dismo\n```\n\nTo enable assimulo support, the easiest way is to install it via mamba using the [mambaforge](https://github.com/conda-forge/miniforge#mambaforge) distribution\n\n```bash\nmamba create -n py311 python=3.11 assimulo\nmamba activate py311\npip install dismo\n```\n\n## License\n\n[GPL 3](https://gitlab.com/qtb-hhu/dismo/blob/main/LICENSE)\n\n## Documentation\n\nThe official documentation is hosted [here on gitlab](https://qtb-hhu.gitlab.io/dismo/).\n\n## Issues and support\n\nIf you experience issues using the software please contact us through our [issues](https://gitlab.com/qtb-hhu/dismo/issues) page.\n\n## Contributing to dismo\n\nAll contributions, bug reports, bug fixes, documentation improvements, enhancements and ideas are welcome.\nSee our [contribution guide](https://gitlab.com/qtb-hhu/dismo/blob/main/CONTRIBUTING.md) for more information.\n\n## How to cite\n\ndismo is currently in the publication process. You will find citing information here as soon as possible.\n\n<!-- If you use this software in your scientific work, please cite [this article](https://rdcu.be/ckOSa):\n\nvan Aalst, M., Ebenhöh, O. & Matuszyńska, A. Constructing and analysing dynamic models with dismo v1.2.3: a software update. BMC Bioinformatics 22, 203 (2021)\n\n- [doi](https://doi.org/10.1186/s12859-021-04122-7)\n- [bibtex file](https://gitlab.com/qtb-hhu/dismo/blob/main/citation.bibtex) -->\n',
     'author': 'Marvin van Aalst',
     'author_email': 'marvin.vanaalst@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `dismo-1.0.8/PKG-INFO` & `dismo-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dismo
-Version: 1.0.8
+Version: 1.0.9
 Summary: A subpackage of modelbase that enables investigation of PDE models
 Author: Marvin van Aalst
 Author-email: marvin.vanaalst@gmail.com
 Requires-Python: >=3.11,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: matplotlib (>=3.8,<4.0)
```

