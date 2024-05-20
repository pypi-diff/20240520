# Comparing `tmp/genewalk-1.6.1.tar.gz` & `tmp/genewalk-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/genewalk-1.6.1.tar", last modified: Fri May 19 20:12:18 2023, max compression
+gzip compressed data, was "dist/genewalk-1.6.2.tar", last modified: Mon May 20 15:01:56 2024, max compression
```

## Comparing `genewalk-1.6.1.tar` & `genewalk-1.6.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 horizon    (501) staff       (20)        0 2023-05-19 20:12:18.000000 genewalk-1.6.1/
--rw-r--r--   0 horizon    (501) staff       (20)       66 2021-01-27 21:08:32.000000 genewalk-1.6.1/MANIFEST.in
--rw-r--r--   0 horizon    (501) staff       (20)    23541 2023-05-19 20:12:18.000000 genewalk-1.6.1/PKG-INFO
--rw-r--r--   0 horizon    (501) staff       (20)    19851 2023-05-16 19:20:53.000000 genewalk-1.6.1/README.md
-drwxr-xr-x   0 horizon    (501) staff       (20)        0 2023-05-19 20:12:18.000000 genewalk-1.6.1/doc/
--rw-r--r--   0 horizon    (501) staff       (20)      606 2019-08-30 13:54:12.000000 genewalk-1.6.1/doc/Makefile
--rw-r--r--   0 horizon    (501) staff       (20)     5562 2023-05-19 20:09:59.000000 genewalk-1.6.1/doc/conf.py
--rw-r--r--   0 horizon    (501) staff       (20)      407 2019-08-30 13:54:12.000000 genewalk-1.6.1/doc/index.rst
--rw-r--r--   0 horizon    (501) staff       (20)      812 2019-08-30 13:54:12.000000 genewalk-1.6.1/doc/make.bat
-drwxr-xr-x   0 horizon    (501) staff       (20)        0 2023-05-19 20:12:18.000000 genewalk-1.6.1/doc/modules/
--rw-r--r--   0 horizon    (501) staff       (20)     1648 2021-01-27 21:08:32.000000 genewalk-1.6.1/doc/modules/genewalk.rst
--rw-r--r--   0 horizon    (501) staff       (20)      124 2019-08-30 13:54:12.000000 genewalk-1.6.1/doc/modules/index.rst
--rw-r--r--   0 horizon    (501) staff       (20)       83 2021-01-27 21:08:32.000000 genewalk-1.6.1/doc/requirements.txt
-drwxr-xr-x   0 horizon    (501) staff       (20)        0 2023-05-19 20:12:18.000000 genewalk-1.6.1/genewalk/
--rw-r--r--   0 horizon    (501) staff       (20)      478 2023-05-19 20:09:59.000000 genewalk-1.6.1/genewalk/__init__.py
--rw-r--r--   0 horizon    (501) staff       (20)    13352 2023-05-16 19:20:53.000000 genewalk-1.6.1/genewalk/cli.py
--rw-r--r--   0 horizon    (501) staff       (20)     8361 2023-05-16 19:20:53.000000 genewalk-1.6.1/genewalk/deepwalk.py
--rw-r--r--   0 horizon    (501) staff       (20)    16017 2021-02-21 02:50:54.000000 genewalk-1.6.1/genewalk/gene_lists.py
--rw-r--r--   0 horizon    (501) staff       (20)     7237 2020-09-21 20:38:26.000000 genewalk-1.6.1/genewalk/get_indra_stmts.py
--rw-r--r--   0 horizon    (501) staff       (20)     1613 2020-02-26 02:19:30.000000 genewalk-1.6.1/genewalk/null_distributions.py
--rw-r--r--   0 horizon    (501) staff       (20)    17380 2021-05-10 13:16:56.000000 genewalk-1.6.1/genewalk/nx_mg_assembler.py
--rw-r--r--   0 horizon    (501) staff       (20)    13295 2023-05-19 20:09:59.000000 genewalk-1.6.1/genewalk/perform_statistics.py
--rw-r--r--   0 horizon    (501) staff       (20)    18257 2021-02-21 02:50:54.000000 genewalk-1.6.1/genewalk/plot.py
--rw-r--r--   0 horizon    (501) staff       (20)     5406 2021-02-21 02:50:54.000000 genewalk-1.6.1/genewalk/resources.py
--rw-r--r--   0 horizon    (501) staff       (20)      442 2021-01-27 21:08:32.000000 genewalk-1.6.1/genewalk/results_template.html
-drwxr-xr-x   0 horizon    (501) staff       (20)        0 2023-05-19 20:12:18.000000 genewalk-1.6.1/genewalk/tests/
--rw-r--r--   0 horizon    (501) staff       (20)        0 2019-08-30 13:54:12.000000 genewalk-1.6.1/genewalk/tests/__init__.py
--rw-r--r--   0 horizon    (501) staff       (20)     6255 2021-02-21 02:50:54.000000 genewalk-1.6.1/genewalk/tests/test_cli.py
--rw-r--r--   0 horizon    (501) staff       (20)      735 2020-02-26 02:19:30.000000 genewalk-1.6.1/genewalk/tests/test_deepwalk.py
--rw-r--r--   0 horizon    (501) staff       (20)     3381 2021-02-21 02:50:54.000000 genewalk-1.6.1/genewalk/tests/test_gene_lists.py
--rw-r--r--   0 horizon    (501) staff       (20)      719 2021-02-21 02:50:54.000000 genewalk-1.6.1/genewalk/tests/test_indra_assembly.py
--rw-r--r--   0 horizon    (501) staff       (20)     5185 2021-02-21 02:50:54.000000 genewalk-1.6.1/genewalk/tests/test_sif_assembler.py
--rw-r--r--   0 horizon    (501) staff       (20)      988 2021-01-27 21:08:32.000000 genewalk-1.6.1/genewalk/tests/test_visualize.py
--rw-r--r--   0 horizon    (501) staff       (20)      815 2021-02-21 02:50:54.000000 genewalk-1.6.1/genewalk/tests/util.py
-drwxr-xr-x   0 horizon    (501) staff       (20)        0 2023-05-19 20:12:18.000000 genewalk-1.6.1/genewalk.egg-info/
--rw-r--r--   0 horizon    (501) staff       (20)    23541 2023-05-19 20:12:18.000000 genewalk-1.6.1/genewalk.egg-info/PKG-INFO
--rw-r--r--   0 horizon    (501) staff       (20)      874 2023-05-19 20:12:18.000000 genewalk-1.6.1/genewalk.egg-info/SOURCES.txt
--rw-r--r--   0 horizon    (501) staff       (20)        1 2023-05-19 20:12:18.000000 genewalk-1.6.1/genewalk.egg-info/dependency_links.txt
--rw-r--r--   0 horizon    (501) staff       (20)       48 2023-05-19 20:12:18.000000 genewalk-1.6.1/genewalk.egg-info/entry_points.txt
--rw-r--r--   0 horizon    (501) staff       (20)      111 2023-05-19 20:12:18.000000 genewalk-1.6.1/genewalk.egg-info/requires.txt
--rw-r--r--   0 horizon    (501) staff       (20)        9 2023-05-19 20:12:18.000000 genewalk-1.6.1/genewalk.egg-info/top_level.txt
--rw-r--r--   0 horizon    (501) staff       (20)       79 2023-05-19 20:12:18.000000 genewalk-1.6.1/setup.cfg
--rwxr-xr-x   0 horizon    (501) staff       (20)     1717 2023-05-19 20:09:59.000000 genewalk-1.6.1/setup.py
+drwxr-xr-x   0 horizon    (501) staff       (20)        0 2024-05-20 15:01:56.000000 genewalk-1.6.2/
+-rw-r--r--   0 horizon    (501) staff       (20)       66 2021-01-27 21:08:32.000000 genewalk-1.6.2/MANIFEST.in
+-rw-r--r--   0 horizon    (501) staff       (20)    23525 2024-05-20 15:01:56.000000 genewalk-1.6.2/PKG-INFO
+-rw-r--r--   0 horizon    (501) staff       (20)    19835 2024-05-20 14:34:17.000000 genewalk-1.6.2/README.md
+drwxr-xr-x   0 horizon    (501) staff       (20)        0 2024-05-20 15:01:56.000000 genewalk-1.6.2/doc/
+-rw-r--r--   0 horizon    (501) staff       (20)      606 2019-08-30 13:54:12.000000 genewalk-1.6.2/doc/Makefile
+-rw-r--r--   0 horizon    (501) staff       (20)     5562 2024-05-20 14:54:48.000000 genewalk-1.6.2/doc/conf.py
+-rw-r--r--   0 horizon    (501) staff       (20)      407 2019-08-30 13:54:12.000000 genewalk-1.6.2/doc/index.rst
+-rw-r--r--   0 horizon    (501) staff       (20)      812 2019-08-30 13:54:12.000000 genewalk-1.6.2/doc/make.bat
+drwxr-xr-x   0 horizon    (501) staff       (20)        0 2024-05-20 15:01:56.000000 genewalk-1.6.2/doc/modules/
+-rw-r--r--   0 horizon    (501) staff       (20)     1648 2021-01-27 21:08:32.000000 genewalk-1.6.2/doc/modules/genewalk.rst
+-rw-r--r--   0 horizon    (501) staff       (20)      124 2019-08-30 13:54:12.000000 genewalk-1.6.2/doc/modules/index.rst
+-rw-r--r--   0 horizon    (501) staff       (20)       83 2021-01-27 21:08:32.000000 genewalk-1.6.2/doc/requirements.txt
+drwxr-xr-x   0 horizon    (501) staff       (20)        0 2024-05-20 15:01:56.000000 genewalk-1.6.2/genewalk/
+-rw-r--r--   0 horizon    (501) staff       (20)      478 2024-05-20 14:54:28.000000 genewalk-1.6.2/genewalk/__init__.py
+-rw-r--r--   0 horizon    (501) staff       (20)    13352 2023-05-16 19:20:53.000000 genewalk-1.6.2/genewalk/cli.py
+-rw-r--r--   0 horizon    (501) staff       (20)     8361 2023-05-16 19:20:53.000000 genewalk-1.6.2/genewalk/deepwalk.py
+-rw-r--r--   0 horizon    (501) staff       (20)    16017 2021-02-21 02:50:54.000000 genewalk-1.6.2/genewalk/gene_lists.py
+-rw-r--r--   0 horizon    (501) staff       (20)     7237 2020-09-21 20:38:26.000000 genewalk-1.6.2/genewalk/get_indra_stmts.py
+-rw-r--r--   0 horizon    (501) staff       (20)     1613 2020-02-26 02:19:30.000000 genewalk-1.6.2/genewalk/null_distributions.py
+-rw-r--r--   0 horizon    (501) staff       (20)    17380 2021-05-10 13:16:56.000000 genewalk-1.6.2/genewalk/nx_mg_assembler.py
+-rw-r--r--   0 horizon    (501) staff       (20)    13295 2023-05-19 20:09:59.000000 genewalk-1.6.2/genewalk/perform_statistics.py
+-rw-r--r--   0 horizon    (501) staff       (20)    18257 2021-02-21 02:50:54.000000 genewalk-1.6.2/genewalk/plot.py
+-rw-r--r--   0 horizon    (501) staff       (20)     5410 2024-05-20 14:34:17.000000 genewalk-1.6.2/genewalk/resources.py
+-rw-r--r--   0 horizon    (501) staff       (20)      442 2021-01-27 21:08:32.000000 genewalk-1.6.2/genewalk/results_template.html
+drwxr-xr-x   0 horizon    (501) staff       (20)        0 2024-05-20 15:01:56.000000 genewalk-1.6.2/genewalk/tests/
+-rw-r--r--   0 horizon    (501) staff       (20)        0 2019-08-30 13:54:12.000000 genewalk-1.6.2/genewalk/tests/__init__.py
+-rw-r--r--   0 horizon    (501) staff       (20)     6255 2021-02-21 02:50:54.000000 genewalk-1.6.2/genewalk/tests/test_cli.py
+-rw-r--r--   0 horizon    (501) staff       (20)      735 2020-02-26 02:19:30.000000 genewalk-1.6.2/genewalk/tests/test_deepwalk.py
+-rw-r--r--   0 horizon    (501) staff       (20)     3381 2021-02-21 02:50:54.000000 genewalk-1.6.2/genewalk/tests/test_gene_lists.py
+-rw-r--r--   0 horizon    (501) staff       (20)      719 2021-02-21 02:50:54.000000 genewalk-1.6.2/genewalk/tests/test_indra_assembly.py
+-rw-r--r--   0 horizon    (501) staff       (20)     5185 2021-02-21 02:50:54.000000 genewalk-1.6.2/genewalk/tests/test_sif_assembler.py
+-rw-r--r--   0 horizon    (501) staff       (20)      988 2021-01-27 21:08:32.000000 genewalk-1.6.2/genewalk/tests/test_visualize.py
+-rw-r--r--   0 horizon    (501) staff       (20)      815 2021-02-21 02:50:54.000000 genewalk-1.6.2/genewalk/tests/util.py
+drwxr-xr-x   0 horizon    (501) staff       (20)        0 2024-05-20 15:01:56.000000 genewalk-1.6.2/genewalk.egg-info/
+-rw-r--r--   0 horizon    (501) staff       (20)    23525 2024-05-20 15:01:56.000000 genewalk-1.6.2/genewalk.egg-info/PKG-INFO
+-rw-r--r--   0 horizon    (501) staff       (20)      874 2024-05-20 15:01:56.000000 genewalk-1.6.2/genewalk.egg-info/SOURCES.txt
+-rw-r--r--   0 horizon    (501) staff       (20)        1 2024-05-20 15:01:56.000000 genewalk-1.6.2/genewalk.egg-info/dependency_links.txt
+-rw-r--r--   0 horizon    (501) staff       (20)       48 2024-05-20 15:01:56.000000 genewalk-1.6.2/genewalk.egg-info/entry_points.txt
+-rw-r--r--   0 horizon    (501) staff       (20)      111 2024-05-20 15:01:56.000000 genewalk-1.6.2/genewalk.egg-info/requires.txt
+-rw-r--r--   0 horizon    (501) staff       (20)        9 2024-05-20 15:01:56.000000 genewalk-1.6.2/genewalk.egg-info/top_level.txt
+-rw-r--r--   0 horizon    (501) staff       (20)       79 2024-05-20 15:01:56.000000 genewalk-1.6.2/setup.cfg
+-rwxr-xr-x   0 horizon    (501) staff       (20)     1717 2024-05-20 14:52:30.000000 genewalk-1.6.2/setup.py
```

### Comparing `genewalk-1.6.1/PKG-INFO` & `genewalk-1.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: genewalk
-Version: 1.6.1
+Version: 1.6.2
 Summary: Determine gene function based on network embeddings.
 Home-page: https://github.com/churchmanlab/genewalk
 Author: Robert Ietswaart
 Author-email: robert_ietswaart@hms.harvard.edu
 License: UNKNOWN
 Description: # GeneWalk
         
         [![License](https://img.shields.io/badge/License-BSD%202--Clause-orange.svg)](https://opensource.org/licenses/BSD-2-Clause)
         [![Documentation](https://readthedocs.org/projects/genewalk/badge/?version=latest)](https://genewalk.readthedocs.io/en/latest/?badge=latest)
         [![PyPI version](https://badge.fury.io/py/genewalk.svg)](https://badge.fury.io/py/genewalk)
-        [![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/genewalk/README.html)
+        [![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](https://anaconda.org/bioconda/genewalk)
         [![Python 3.8+](https://img.shields.io/pypi/pyversions/genewalk.svg)](https://www.python.org/downloads)
         
         GeneWalk determines for individual genes the functions that are relevant in a
         particular biological context and experimental condition. GeneWalk quantifies
         the similarity between vector representations of a gene and annotated GO terms
         through representation learning with random walks on a condition-specific gene
         regulatory network. Similarity significance is determined through comparison
```

### Comparing `genewalk-1.6.1/README.md` & `genewalk-1.6.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # GeneWalk
 
 [![License](https://img.shields.io/badge/License-BSD%202--Clause-orange.svg)](https://opensource.org/licenses/BSD-2-Clause)
 [![Documentation](https://readthedocs.org/projects/genewalk/badge/?version=latest)](https://genewalk.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/genewalk.svg)](https://badge.fury.io/py/genewalk)
-[![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/genewalk/README.html)
+[![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](https://anaconda.org/bioconda/genewalk)
 [![Python 3.8+](https://img.shields.io/pypi/pyversions/genewalk.svg)](https://www.python.org/downloads)
 
 GeneWalk determines for individual genes the functions that are relevant in a
 particular biological context and experimental condition. GeneWalk quantifies
 the similarity between vector representations of a gene and annotated GO terms
 through representation learning with random walks on a condition-specific gene
 regulatory network. Similarity significance is determined through comparison
```

### Comparing `genewalk-1.6.1/doc/Makefile` & `genewalk-1.6.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `genewalk-1.6.1/doc/conf.py` & `genewalk-1.6.2/doc/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 project = 'GeneWalk'
 copyright = '2019, GeneWalk Developers'
 author = 'GeneWalk Developers'
 
 # The short X.Y version
 version = '1.6'
 # The full version, including alpha/beta/rc tags
-release = '1.6.1'
+release = '1.6.2'
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
```

### Comparing `genewalk-1.6.1/doc/make.bat` & `genewalk-1.6.2/doc/make.bat`

 * *Files identical despite different names*

### Comparing `genewalk-1.6.1/doc/modules/genewalk.rst` & `genewalk-1.6.2/doc/modules/genewalk.rst`

 * *Files identical despite different names*

### Comparing `genewalk-1.6.1/genewalk/cli.py` & `genewalk-1.6.2/genewalk/cli.py`

 * *Files identical despite different names*

### Comparing `genewalk-1.6.1/genewalk/deepwalk.py` & `genewalk-1.6.2/genewalk/deepwalk.py`

 * *Files identical despite different names*

### Comparing `genewalk-1.6.1/genewalk/gene_lists.py` & `genewalk-1.6.2/genewalk/gene_lists.py`

 * *Files identical despite different names*

### Comparing `genewalk-1.6.1/genewalk/get_indra_stmts.py` & `genewalk-1.6.2/genewalk/get_indra_stmts.py`

 * *Files identical despite different names*

### Comparing `genewalk-1.6.1/genewalk/null_distributions.py` & `genewalk-1.6.2/genewalk/null_distributions.py`

 * *Files identical despite different names*

### Comparing `genewalk-1.6.1/genewalk/nx_mg_assembler.py` & `genewalk-1.6.2/genewalk/nx_mg_assembler.py`

 * *Files identical despite different names*

### Comparing `genewalk-1.6.1/genewalk/perform_statistics.py` & `genewalk-1.6.2/genewalk/perform_statistics.py`

 * *Files identical despite different names*

### Comparing `genewalk-1.6.1/genewalk/plot.py` & `genewalk-1.6.2/genewalk/plot.py`

 * *Files identical despite different names*

### Comparing `genewalk-1.6.1/genewalk/resources.py` & `genewalk-1.6.2/genewalk/resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,43 +16,43 @@
             os.path.join(os.path.expanduser('~'), 'genewalk')
         self.resource_folder = self._get_resource_folder()
         logger.info('Using %s as resource folder.' % self.resource_folder)
 
     def get_go_obo(self):
         fname = os.path.join(self.resource_folder, 'go.obo')
         if not os.path.exists(fname):
-            url = 'http://snapshot.geneontology.org/ontology/go.obo'
+            url = 'https://snapshot.geneontology.org/ontology/go.obo'
             download_url(url, fname)
         return fname
 
     def get_goa_gaf(self):
         fname = os.path.join(self.resource_folder, 'goa_human.gaf')
         if not os.path.exists(fname):
-            url_goa = ('http://geneontology.org/gene-associations/'
+            url_goa = ('https://geneontology.org/gene-associations/'
                        'goa_human.gaf.gz')
             download_gz(fname, url_goa)
         return fname
 
     def get_pc(self):
         fname_current = os.path.join(self.resource_folder,
                                      'PathwayCommons12.All.hgnc_current.sif')
         if not os.path.exists(fname_current):
             fname = os.path.join(self.resource_folder,
                                  'PathwayCommons12.All.hgnc.sif')
             if not os.path.exists(fname):
-                url_pc = ('http://www.pathwaycommons.org/archives/PC2/v12/'
+                url_pc = ('https://www.pathwaycommons.org/archives/PC2/v12/'
                           'PathwayCommons12.All.hgnc.sif.gz')
                 download_gz(fname, url_pc)
             self._replace_outdated_hgnc_symbols(fname,fname_current)
         return fname_current
 
     def get_mgi_entrez(self):
         fname = os.path.join(self.resource_folder, 'MGI_EntrezGene.rpt')
         if not os.path.exists(fname):
-            url = 'http://www.informatics.jax.org/downloads/reports/' \
+            url = 'https://www.informatics.jax.org/downloads/reports/' \
                   'MGI_EntrezGene.rpt'
             download_url(url, fname)
         return fname
 
     def get_hgnc(self):
         fname = os.path.join(self.resource_folder, 'hgnc_entries.tsv')
         if not os.path.exists(fname):
```

### Comparing `genewalk-1.6.1/genewalk/tests/test_cli.py` & `genewalk-1.6.2/genewalk/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `genewalk-1.6.1/genewalk/tests/test_deepwalk.py` & `genewalk-1.6.2/genewalk/tests/test_deepwalk.py`

 * *Files identical despite different names*

### Comparing `genewalk-1.6.1/genewalk/tests/test_gene_lists.py` & `genewalk-1.6.2/genewalk/tests/test_gene_lists.py`

 * *Files identical despite different names*

### Comparing `genewalk-1.6.1/genewalk/tests/test_indra_assembly.py` & `genewalk-1.6.2/genewalk/tests/test_indra_assembly.py`

 * *Files identical despite different names*

### Comparing `genewalk-1.6.1/genewalk/tests/test_sif_assembler.py` & `genewalk-1.6.2/genewalk/tests/test_sif_assembler.py`

 * *Files identical despite different names*

### Comparing `genewalk-1.6.1/genewalk/tests/test_visualize.py` & `genewalk-1.6.2/genewalk/tests/test_visualize.py`

 * *Files identical despite different names*

### Comparing `genewalk-1.6.1/genewalk/tests/util.py` & `genewalk-1.6.2/genewalk/tests/util.py`

 * *Files identical despite different names*

### Comparing `genewalk-1.6.1/genewalk.egg-info/PKG-INFO` & `genewalk-1.6.2/genewalk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: genewalk
-Version: 1.6.1
+Version: 1.6.2
 Summary: Determine gene function based on network embeddings.
 Home-page: https://github.com/churchmanlab/genewalk
 Author: Robert Ietswaart
 Author-email: robert_ietswaart@hms.harvard.edu
 License: UNKNOWN
 Description: # GeneWalk
         
         [![License](https://img.shields.io/badge/License-BSD%202--Clause-orange.svg)](https://opensource.org/licenses/BSD-2-Clause)
         [![Documentation](https://readthedocs.org/projects/genewalk/badge/?version=latest)](https://genewalk.readthedocs.io/en/latest/?badge=latest)
         [![PyPI version](https://badge.fury.io/py/genewalk.svg)](https://badge.fury.io/py/genewalk)
-        [![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/genewalk/README.html)
+        [![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](https://anaconda.org/bioconda/genewalk)
         [![Python 3.8+](https://img.shields.io/pypi/pyversions/genewalk.svg)](https://www.python.org/downloads)
         
         GeneWalk determines for individual genes the functions that are relevant in a
         particular biological context and experimental condition. GeneWalk quantifies
         the similarity between vector representations of a gene and annotated GO terms
         through representation learning with random walks on a condition-specific gene
         regulatory network. Similarity significance is determined through comparison
```

### Comparing `genewalk-1.6.1/genewalk.egg-info/SOURCES.txt` & `genewalk-1.6.2/genewalk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `genewalk-1.6.1/setup.py` & `genewalk-1.6.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 def main():
     install_list = ['numpy', 'pandas', 'networkx>=2.1', 'gensim>=4.0.0', 'goatools',
                     'scipy>=1.3.0', 'matplotlib', 'seaborn', 'plotly>=4.0.0']
 
     setup(name='genewalk',
-          version='1.6.1',
+          version='1.6.2',
           description='Determine gene function based on network embeddings.',
           long_description=long_description,
           long_description_content_type='text/markdown',
           author='Robert Ietswaart',
           author_email='robert_ietswaart@hms.harvard.edu',
           url='https://github.com/churchmanlab/genewalk',
           classifiers=[
```

