# Comparing `tmp/gene4mvcf-1.1.1.tar.gz` & `tmp/gene4mvcf-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gene4mvcf-1.1.1.tar", last modified: Mon May 20 12:23:28 2024, max compression
+gzip compressed data, was "gene4mvcf-1.1.2.tar", last modified: Mon May 20 12:38:01 2024, max compression
```

## Comparing `gene4mvcf-1.1.1.tar` & `gene4mvcf-1.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 12:23:28.126169 gene4mvcf-1.1.1/
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)     1843 2024-05-20 12:23:28.126169 gene4mvcf-1.1.1/PKG-INFO
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1393 2024-05-20 11:47:55.000000 gene4mvcf-1.1.1/README.md
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 12:23:28.126169 gene4mvcf-1.1.1/gene4mVCF/
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 11:07:18.000000 gene4mvcf-1.1.1/gene4mVCF/__init__.py
--rwxrwxr-x   0 ws2024    (1000) ws2024    (1000)     4379 2024-05-20 12:13:50.000000 gene4mvcf-1.1.1/gene4mVCF/fetchgenes.py
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 12:23:28.126169 gene4mvcf-1.1.1/gene4mVCF.egg-info/
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)     1843 2024-05-20 12:23:28.000000 gene4mvcf-1.1.1/gene4mVCF.egg-info/PKG-INFO
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      264 2024-05-20 12:23:28.000000 gene4mvcf-1.1.1/gene4mVCF.egg-info/SOURCES.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-05-20 12:23:28.000000 gene4mvcf-1.1.1/gene4mVCF.egg-info/dependency_links.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       56 2024-05-20 12:23:28.000000 gene4mvcf-1.1.1/gene4mVCF.egg-info/entry_points.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       78 2024-05-20 12:23:28.000000 gene4mvcf-1.1.1/gene4mVCF.egg-info/requires.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       10 2024-05-20 12:23:28.000000 gene4mvcf-1.1.1/gene4mVCF.egg-info/top_level.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       38 2024-05-20 12:23:28.126169 gene4mvcf-1.1.1/setup.cfg
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1343 2024-05-20 11:48:03.000000 gene4mvcf-1.1.1/setup.py
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 12:38:01.007881 gene4mvcf-1.1.2/
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     2417 2024-05-20 12:38:01.003881 gene4mvcf-1.1.2/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1967 2024-05-20 12:34:41.000000 gene4mvcf-1.1.2/README.md
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 12:38:00.999881 gene4mvcf-1.1.2/gene4mVCF/
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 11:07:18.000000 gene4mvcf-1.1.2/gene4mVCF/__init__.py
+-rwxrwxr-x   0 ws2024    (1000) ws2024    (1000)     4379 2024-05-20 12:13:50.000000 gene4mvcf-1.1.2/gene4mVCF/fetchgenes.py
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 12:38:01.003881 gene4mvcf-1.1.2/gene4mVCF.egg-info/
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     2417 2024-05-20 12:38:00.000000 gene4mvcf-1.1.2/gene4mVCF.egg-info/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      264 2024-05-20 12:38:00.000000 gene4mvcf-1.1.2/gene4mVCF.egg-info/SOURCES.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-05-20 12:38:00.000000 gene4mvcf-1.1.2/gene4mVCF.egg-info/dependency_links.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       56 2024-05-20 12:38:00.000000 gene4mvcf-1.1.2/gene4mVCF.egg-info/entry_points.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       78 2024-05-20 12:38:00.000000 gene4mvcf-1.1.2/gene4mVCF.egg-info/requires.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       10 2024-05-20 12:38:00.000000 gene4mvcf-1.1.2/gene4mVCF.egg-info/top_level.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       38 2024-05-20 12:38:01.007881 gene4mvcf-1.1.2/setup.cfg
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1343 2024-05-20 12:37:50.000000 gene4mvcf-1.1.2/setup.py
```

### Comparing `gene4mvcf-1.1.1/PKG-INFO` & `gene4mvcf-1.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gene4mVCF
-Version: 1.1.1
+Version: 1.1.2
 Summary: Description of your package
 Home-page: https://github.com/VJ-Ulaganathan/gene4mVCF
 Author: Pr (France). Dr. rer. nat. Vijay K. ULAGANATHAN
 Author-email: vijay-kumar.ulaganathan@uni-tuebingen.de
 Description-Content-Type: text/markdown
 Requires-Dist: pysam>=0.16.0.1
 Requires-Dist: pandas>=1.0.0
@@ -19,14 +19,20 @@
 
 ## Installation
 
 You can install `gene4mVCF` via pip:
 
 `$ pip install gene4mVCF`
 
+After installation please download the four required bed files and place inside the folder /gene4mVCF
+<br>'hg19.ensGene.bed' --> https://hgdownload.soe.ucsc.edu/goldenPath/hg19/bigZips/genes/hg19.ensGene.gtf.gz </br>
+<br>'hg19.ncbiRefSeq.bed' --> https://hgdownload.soe.ucsc.edu/goldenPath/hg19/bigZips/genes/hg19.ncbiRefSeq.gtf.gz </br>
+<br>'hg38.ensGene.bed' --> https://hgdownload.soe.ucsc.edu/goldenPath/hg38/bigZips/genes/hg38.ensGene.gtf.gz </br>
+<br>'hg38.ncbiRefSeq.bed'--> https://hgdownload.soe.ucsc.edu/goldenPath/hg38/bigZips/genes/hg38.ncbiRefSeq.gtf.gz </br>
+
 ## Usage
 usage: `$ gene4mVCF [-h] -i INPUT -g GENE`
 
 Extract variant entries for a specific gene or list of genes from a VCF file.
 
 optional arguments:
   -h, --help            show this help message and exit
```

### Comparing `gene4mvcf-1.1.1/gene4mVCF/fetchgenes.py` & `gene4mvcf-1.1.2/gene4mVCF/fetchgenes.py`

 * *Files identical despite different names*

### Comparing `gene4mvcf-1.1.1/gene4mVCF.egg-info/PKG-INFO` & `gene4mvcf-1.1.2/gene4mVCF.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gene4mVCF
-Version: 1.1.1
+Version: 1.1.2
 Summary: Description of your package
 Home-page: https://github.com/VJ-Ulaganathan/gene4mVCF
 Author: Pr (France). Dr. rer. nat. Vijay K. ULAGANATHAN
 Author-email: vijay-kumar.ulaganathan@uni-tuebingen.de
 Description-Content-Type: text/markdown
 Requires-Dist: pysam>=0.16.0.1
 Requires-Dist: pandas>=1.0.0
@@ -19,14 +19,20 @@
 
 ## Installation
 
 You can install `gene4mVCF` via pip:
 
 `$ pip install gene4mVCF`
 
+After installation please download the four required bed files and place inside the folder /gene4mVCF
+<br>'hg19.ensGene.bed' --> https://hgdownload.soe.ucsc.edu/goldenPath/hg19/bigZips/genes/hg19.ensGene.gtf.gz </br>
+<br>'hg19.ncbiRefSeq.bed' --> https://hgdownload.soe.ucsc.edu/goldenPath/hg19/bigZips/genes/hg19.ncbiRefSeq.gtf.gz </br>
+<br>'hg38.ensGene.bed' --> https://hgdownload.soe.ucsc.edu/goldenPath/hg38/bigZips/genes/hg38.ensGene.gtf.gz </br>
+<br>'hg38.ncbiRefSeq.bed'--> https://hgdownload.soe.ucsc.edu/goldenPath/hg38/bigZips/genes/hg38.ncbiRefSeq.gtf.gz </br>
+
 ## Usage
 usage: `$ gene4mVCF [-h] -i INPUT -g GENE`
 
 Extract variant entries for a specific gene or list of genes from a VCF file.
 
 optional arguments:
   -h, --help            show this help message and exit
```

### Comparing `gene4mvcf-1.1.1/setup.py` & `gene4mvcf-1.1.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # Check if all required commands exist
 if not all(command_exists(cmd) for cmd in required_commands):
     raise RuntimeError("Please install the following dependencies: bcftools, bgzip, tabix")
 
 setup(
     name='gene4mVCF',
-    version='1.1.1',
+    version='1.1.2',
     description='Description of your package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Pr (France). Dr. rer. nat. Vijay K. ULAGANATHAN',
     author_email='vijay-kumar.ulaganathan@uni-tuebingen.de',
     url='https://github.com/VJ-Ulaganathan/gene4mVCF',
     packages=find_packages(),
```

