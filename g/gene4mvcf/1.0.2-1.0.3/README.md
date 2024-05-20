# Comparing `tmp/gene4mvcf-1.0.2.tar.gz` & `tmp/gene4mvcf-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gene4mvcf-1.0.2.tar", last modified: Mon May 20 10:10:52 2024, max compression
+gzip compressed data, was "gene4mvcf-1.0.3.tar", last modified: Mon May 20 10:22:42 2024, max compression
```

## Comparing `gene4mvcf-1.0.2.tar` & `gene4mvcf-1.0.3.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 10:10:52.780564 gene4mvcf-1.0.2/
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1586 2024-05-20 10:10:52.780564 gene4mvcf-1.0.2/PKG-INFO
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1289 2024-05-20 10:09:20.000000 gene4mvcf-1.0.2/README.md
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 10:10:52.780564 gene4mvcf-1.0.2/gene4mvcf.egg-info/
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)     1586 2024-05-20 10:10:52.000000 gene4mvcf-1.0.2/gene4mvcf.egg-info/PKG-INFO
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      182 2024-05-20 10:10:52.000000 gene4mvcf-1.0.2/gene4mvcf.egg-info/SOURCES.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-05-20 10:10:52.000000 gene4mvcf-1.0.2/gene4mvcf.egg-info/dependency_links.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       78 2024-05-20 10:10:52.000000 gene4mvcf-1.0.2/gene4mvcf.egg-info/requires.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-05-20 10:10:52.000000 gene4mvcf-1.0.2/gene4mvcf.egg-info/top_level.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       38 2024-05-20 10:10:52.780564 gene4mvcf-1.0.2/setup.cfg
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1148 2024-05-20 10:10:43.000000 gene4mvcf-1.0.2/setup.py
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 10:22:42.038113 gene4mvcf-1.0.3/
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     1739 2024-05-20 10:22:42.038113 gene4mvcf-1.0.3/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1289 2024-05-20 10:22:01.000000 gene4mvcf-1.0.3/README.md
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 10:22:42.038113 gene4mvcf-1.0.3/gene4mVCF/
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        0 2024-05-17 19:50:34.000000 gene4mvcf-1.0.3/gene4mVCF/__init__.py
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     4665 2024-05-20 10:22:02.000000 gene4mvcf-1.0.3/gene4mVCF/gene4mvcf.py
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 10:22:42.038113 gene4mvcf-1.0.3/gene4mvcf.egg-info/
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     1739 2024-05-20 10:22:42.000000 gene4mvcf-1.0.3/gene4mvcf.egg-info/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      227 2024-05-20 10:22:42.000000 gene4mvcf-1.0.3/gene4mvcf.egg-info/SOURCES.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-05-20 10:22:42.000000 gene4mvcf-1.0.3/gene4mvcf.egg-info/dependency_links.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       78 2024-05-20 10:22:42.000000 gene4mvcf-1.0.3/gene4mvcf.egg-info/requires.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       10 2024-05-20 10:22:42.000000 gene4mvcf-1.0.3/gene4mvcf.egg-info/top_level.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       38 2024-05-20 10:22:42.038113 gene4mvcf-1.0.3/setup.cfg
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1148 2024-05-20 10:21:52.000000 gene4mvcf-1.0.3/setup.py
```

### Comparing `gene4mvcf-1.0.2/PKG-INFO` & `gene4mvcf-1.0.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 Metadata-Version: 2.1
 Name: gene4mvcf
-Version: 1.0.2
+Version: 1.0.3
 Summary: Description of your package
 Home-page: https://github.com/VJ-Ulaganathan/gene4mVCF
 Author: Pr (France). Dr. rer. nat. Vijay K. ULAGANATHAN
 Author-email: vijay-kumar.ulaganathan@uni-tuebingen.de
 Description-Content-Type: text/markdown
+Requires-Dist: pysam>=0.16.0.1
+Requires-Dist: pandas>=1.0.0
+Requires-Dist: pybedtools>=0.8.0
+Requires-Dist: tqdm>=4.47.0
+Requires-Dist: gffutils>=0.10.1
 
 # gene4mVCF
 
 ## Introduction
 `gene4mVCF` is a Python package that allows you to extract variant entries for specific genes or a list of genes from a VCF (Variant Call Format) file. It utilizes tools like `bcftools`, `tabix`, and Python libraries like `pysam`, `pandas`, `pybedtools`, `tqdm`, and `gffutils` to efficiently parse and extract variants.
 
 ## Installation
```

### Comparing `gene4mvcf-1.0.2/README.md` & `gene4mvcf-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `gene4mvcf-1.0.2/gene4mvcf.egg-info/PKG-INFO` & `gene4mvcf-1.0.3/gene4mvcf.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 Metadata-Version: 2.1
 Name: gene4mvcf
-Version: 1.0.2
+Version: 1.0.3
 Summary: Description of your package
 Home-page: https://github.com/VJ-Ulaganathan/gene4mVCF
 Author: Pr (France). Dr. rer. nat. Vijay K. ULAGANATHAN
 Author-email: vijay-kumar.ulaganathan@uni-tuebingen.de
 Description-Content-Type: text/markdown
+Requires-Dist: pysam>=0.16.0.1
+Requires-Dist: pandas>=1.0.0
+Requires-Dist: pybedtools>=0.8.0
+Requires-Dist: tqdm>=4.47.0
+Requires-Dist: gffutils>=0.10.1
 
 # gene4mVCF
 
 ## Introduction
 `gene4mVCF` is a Python package that allows you to extract variant entries for specific genes or a list of genes from a VCF (Variant Call Format) file. It utilizes tools like `bcftools`, `tabix`, and Python libraries like `pysam`, `pandas`, `pybedtools`, `tqdm`, and `gffutils` to efficiently parse and extract variants.
 
 ## Installation
```

### Comparing `gene4mvcf-1.0.2/setup.py` & `gene4mvcf-1.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # Check if all required commands exist
 if not all(command_exists(cmd) for cmd in required_commands):
     raise RuntimeError("Please install the following dependencies: bcftools, bgzip, tabix")
 
 setup(
     name='gene4mvcf',
-    version='1.0.2',
+    version='1.0.3',
     description='Description of your package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Pr (France). Dr. rer. nat. Vijay K. ULAGANATHAN',
     author_email='vijay-kumar.ulaganathan@uni-tuebingen.de',
     url='https://github.com/VJ-Ulaganathan/gene4mVCF',
     packages=find_packages(),
```

