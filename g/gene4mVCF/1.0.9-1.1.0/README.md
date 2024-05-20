# Comparing `tmp/gene4mvcf-1.0.9.tar.gz` & `tmp/gene4mvcf-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gene4mvcf-1.0.9.tar", last modified: Mon May 20 11:10:10 2024, max compression
+gzip compressed data, was "gene4mvcf-1.1.0.tar", last modified: Mon May 20 11:33:24 2024, max compression
```

## Comparing `gene4mvcf-1.0.9.tar` & `gene4mvcf-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 11:10:10.507081 gene4mvcf-1.0.9/
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)     1805 2024-05-20 11:10:10.507081 gene4mvcf-1.0.9/PKG-INFO
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1355 2024-05-20 11:06:57.000000 gene4mvcf-1.0.9/README.md
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 11:10:10.503081 gene4mvcf-1.0.9/gene4mVCF/
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 11:07:18.000000 gene4mvcf-1.0.9/gene4mVCF/__init__.py
--rwxrwxr-x   0 ws2024    (1000) ws2024    (1000)     4665 2024-05-20 10:22:02.000000 gene4mvcf-1.0.9/gene4mVCF/fetchgenes.py
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 11:10:10.507081 gene4mvcf-1.0.9/gene4mVCF.egg-info/
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)     1805 2024-05-20 11:10:10.000000 gene4mvcf-1.0.9/gene4mVCF.egg-info/PKG-INFO
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      264 2024-05-20 11:10:10.000000 gene4mvcf-1.0.9/gene4mVCF.egg-info/SOURCES.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-05-20 11:10:10.000000 gene4mvcf-1.0.9/gene4mVCF.egg-info/dependency_links.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       56 2024-05-20 11:10:10.000000 gene4mvcf-1.0.9/gene4mVCF.egg-info/entry_points.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       78 2024-05-20 11:10:10.000000 gene4mvcf-1.0.9/gene4mVCF.egg-info/requires.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       10 2024-05-20 11:10:10.000000 gene4mvcf-1.0.9/gene4mVCF.egg-info/top_level.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       38 2024-05-20 11:10:10.507081 gene4mvcf-1.0.9/setup.cfg
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1223 2024-05-20 11:06:59.000000 gene4mvcf-1.0.9/setup.py
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 11:33:24.065985 gene4mvcf-1.1.0/
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     1773 2024-05-20 11:33:24.065985 gene4mvcf-1.1.0/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1323 2024-05-20 11:33:00.000000 gene4mvcf-1.1.0/README.md
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 11:33:24.065985 gene4mvcf-1.1.0/gene4mVCF/
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 11:07:18.000000 gene4mvcf-1.1.0/gene4mVCF/__init__.py
+-rwxrwxr-x   0 ws2024    (1000) ws2024    (1000)     4665 2024-05-20 10:22:02.000000 gene4mvcf-1.1.0/gene4mVCF/fetchgenes.py
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 11:33:24.065985 gene4mvcf-1.1.0/gene4mVCF.egg-info/
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     1773 2024-05-20 11:33:24.000000 gene4mvcf-1.1.0/gene4mVCF.egg-info/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      264 2024-05-20 11:33:24.000000 gene4mvcf-1.1.0/gene4mVCF.egg-info/SOURCES.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-05-20 11:33:24.000000 gene4mvcf-1.1.0/gene4mVCF.egg-info/dependency_links.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       56 2024-05-20 11:33:24.000000 gene4mvcf-1.1.0/gene4mVCF.egg-info/entry_points.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       78 2024-05-20 11:33:24.000000 gene4mvcf-1.1.0/gene4mVCF.egg-info/requires.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       10 2024-05-20 11:33:24.000000 gene4mvcf-1.1.0/gene4mVCF.egg-info/top_level.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       38 2024-05-20 11:33:24.065985 gene4mvcf-1.1.0/setup.cfg
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1343 2024-05-20 11:32:51.000000 gene4mvcf-1.1.0/setup.py
```

### Comparing `gene4mvcf-1.0.9/PKG-INFO` & `gene4mvcf-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gene4mVCF
-Version: 1.0.9
+Version: 1.1.0
 Summary: Description of your package
 Home-page: https://github.com/VJ-Ulaganathan/gene4mVCF
 Author: Pr (France). Dr. rer. nat. Vijay K. ULAGANATHAN
 Author-email: vijay-kumar.ulaganathan@uni-tuebingen.de
 Description-Content-Type: text/markdown
 Requires-Dist: pysam>=0.16.0.1
 Requires-Dist: pandas>=1.0.0
@@ -20,32 +20,32 @@
 ## Installation
 
 You can install `gene4mVCF` via pip:
 
 `$ pip install gene4mVCF`
 
 ## Usage
-usage: `$ python3 gene4mVCF [-h] -i INPUT -g GENE`
+usage: `$ gene4mVCF [-h] -i INPUT -g GENE`
 
 Extract variant entries for a specific gene or list of genes from a VCF file.
 
 optional arguments:
   -h, --help            show this help message and exit
   -i INPUT, --input INPUT
                         Input bgzip compressed VCF file
   -g GENES, --genes GENES
                         Gene name, Ensembl gene ID, or path to a gene list file
 
 ## Examples
 Extract variants for a single gene:
-`$ python3 gene4mVCF -i input.vcf.gz -g EGFR`
-`$ python3 gene4mVCF -i input.vcf.gz -g ENSG00000168878`
+`$ gene4mVCF -i input.vcf.gz -g EGFR`
+`$ gene4mVCF -i input.vcf.gz -g ENSG00000168878`
 
 Extract variants for multiple genes listed in a file:
-`$ python3 gene4mVCF -i input.vcf.gz -g genes.txt`
+`$ gene4mVCF -i input.vcf.gz -g genes.txt`
 
 For more options and details, refer to the help message.
 
 ## Support
 For any issues or inquiries, please open an issue on the GitHub repository https://github.com/VJ-Ulaganathan/gene4mVCF
```

### Comparing `gene4mvcf-1.0.9/README.md` & `gene4mvcf-1.1.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -6,32 +6,32 @@
 ## Installation
 
 You can install `gene4mVCF` via pip:
 
 `$ pip install gene4mVCF`
 
 ## Usage
-usage: `$ python3 gene4mVCF [-h] -i INPUT -g GENE`
+usage: `$ gene4mVCF [-h] -i INPUT -g GENE`
 
 Extract variant entries for a specific gene or list of genes from a VCF file.
 
 optional arguments:
   -h, --help            show this help message and exit
   -i INPUT, --input INPUT
                         Input bgzip compressed VCF file
   -g GENES, --genes GENES
                         Gene name, Ensembl gene ID, or path to a gene list file
 
 ## Examples
 Extract variants for a single gene:
-`$ python3 gene4mVCF -i input.vcf.gz -g EGFR`
-`$ python3 gene4mVCF -i input.vcf.gz -g ENSG00000168878`
+`$ gene4mVCF -i input.vcf.gz -g EGFR`
+`$ gene4mVCF -i input.vcf.gz -g ENSG00000168878`
 
 Extract variants for multiple genes listed in a file:
-`$ python3 gene4mVCF -i input.vcf.gz -g genes.txt`
+`$ gene4mVCF -i input.vcf.gz -g genes.txt`
 
 For more options and details, refer to the help message.
 
 ## Support
 For any issues or inquiries, please open an issue on the GitHub repository https://github.com/VJ-Ulaganathan/gene4mVCF
```

### Comparing `gene4mvcf-1.0.9/gene4mVCF/fetchgenes.py` & `gene4mvcf-1.1.0/gene4mVCF/fetchgenes.py`

 * *Files identical despite different names*

### Comparing `gene4mvcf-1.0.9/gene4mVCF.egg-info/PKG-INFO` & `gene4mvcf-1.1.0/gene4mVCF.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gene4mVCF
-Version: 1.0.9
+Version: 1.1.0
 Summary: Description of your package
 Home-page: https://github.com/VJ-Ulaganathan/gene4mVCF
 Author: Pr (France). Dr. rer. nat. Vijay K. ULAGANATHAN
 Author-email: vijay-kumar.ulaganathan@uni-tuebingen.de
 Description-Content-Type: text/markdown
 Requires-Dist: pysam>=0.16.0.1
 Requires-Dist: pandas>=1.0.0
@@ -20,32 +20,32 @@
 ## Installation
 
 You can install `gene4mVCF` via pip:
 
 `$ pip install gene4mVCF`
 
 ## Usage
-usage: `$ python3 gene4mVCF [-h] -i INPUT -g GENE`
+usage: `$ gene4mVCF [-h] -i INPUT -g GENE`
 
 Extract variant entries for a specific gene or list of genes from a VCF file.
 
 optional arguments:
   -h, --help            show this help message and exit
   -i INPUT, --input INPUT
                         Input bgzip compressed VCF file
   -g GENES, --genes GENES
                         Gene name, Ensembl gene ID, or path to a gene list file
 
 ## Examples
 Extract variants for a single gene:
-`$ python3 gene4mVCF -i input.vcf.gz -g EGFR`
-`$ python3 gene4mVCF -i input.vcf.gz -g ENSG00000168878`
+`$ gene4mVCF -i input.vcf.gz -g EGFR`
+`$ gene4mVCF -i input.vcf.gz -g ENSG00000168878`
 
 Extract variants for multiple genes listed in a file:
-`$ python3 gene4mVCF -i input.vcf.gz -g genes.txt`
+`$ gene4mVCF -i input.vcf.gz -g genes.txt`
 
 For more options and details, refer to the help message.
 
 ## Support
 For any issues or inquiries, please open an issue on the GitHub repository https://github.com/VJ-Ulaganathan/gene4mVCF
```

### Comparing `gene4mvcf-1.0.9/setup.py` & `gene4mvcf-1.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,22 +10,23 @@
 
 # Check if all required commands exist
 if not all(command_exists(cmd) for cmd in required_commands):
     raise RuntimeError("Please install the following dependencies: bcftools, bgzip, tabix")
 
 setup(
     name='gene4mVCF',
-    version='1.0.9',
+    version='1.1.0',
     description='Description of your package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Pr (France). Dr. rer. nat. Vijay K. ULAGANATHAN',
     author_email='vijay-kumar.ulaganathan@uni-tuebingen.de',
     url='https://github.com/VJ-Ulaganathan/gene4mVCF',
     packages=find_packages(),
+    package_data={'gene4mVCF': ['hg19.ensGene.bed', 'hg19.ncbiRefSeq.bed', 'hg38.ensGene.bed', 'hg38.ncbiRefSeq.bed']},
     install_requires=[
         'pysam>=0.16.0.1',
         'pandas>=1.0.0',
         'pybedtools>=0.8.0',
         'tqdm>=4.47.0',
         'gffutils>=0.10.1'
     ],
```

