# Comparing `tmp/gene4mvcf-1.0.6.tar.gz` & `tmp/gene4mvcf-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gene4mvcf-1.0.6.tar", last modified: Mon May 20 10:32:31 2024, max compression
+gzip compressed data, was "gene4mvcf-1.0.7.tar", last modified: Mon May 20 10:42:54 2024, max compression
```

## Comparing `gene4mvcf-1.0.6.tar` & `gene4mvcf-1.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 10:32:31.559127 gene4mvcf-1.0.6/
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)     1739 2024-05-20 10:32:31.559127 gene4mvcf-1.0.6/PKG-INFO
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1289 2024-05-20 10:22:01.000000 gene4mvcf-1.0.6/README.md
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 10:32:31.555127 gene4mvcf-1.0.6/gene4mVCF/
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        0 2024-05-17 19:50:34.000000 gene4mvcf-1.0.6/gene4mVCF/__init__.py
--rwxrwxr-x   0 ws2024    (1000) ws2024    (1000)     4665 2024-05-20 10:22:02.000000 gene4mvcf-1.0.6/gene4mVCF/gene4mvcf.py
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 10:32:31.559127 gene4mvcf-1.0.6/gene4mVCF.egg-info/
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)     1739 2024-05-20 10:32:31.000000 gene4mvcf-1.0.6/gene4mVCF.egg-info/PKG-INFO
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      263 2024-05-20 10:32:31.000000 gene4mvcf-1.0.6/gene4mVCF.egg-info/SOURCES.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-05-20 10:32:31.000000 gene4mvcf-1.0.6/gene4mVCF.egg-info/dependency_links.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       55 2024-05-20 10:32:31.000000 gene4mvcf-1.0.6/gene4mVCF.egg-info/entry_points.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       78 2024-05-20 10:32:31.000000 gene4mvcf-1.0.6/gene4mVCF.egg-info/requires.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       10 2024-05-20 10:32:31.000000 gene4mvcf-1.0.6/gene4mVCF.egg-info/top_level.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       38 2024-05-20 10:32:31.559127 gene4mvcf-1.0.6/setup.cfg
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1222 2024-05-20 10:32:23.000000 gene4mvcf-1.0.6/setup.py
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 10:42:54.535939 gene4mvcf-1.0.7/
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     1762 2024-05-20 10:42:54.535939 gene4mvcf-1.0.7/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1312 2024-05-20 10:42:40.000000 gene4mvcf-1.0.7/README.md
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 10:42:54.535939 gene4mvcf-1.0.7/gene4mVCF/
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        0 2024-05-17 19:50:34.000000 gene4mvcf-1.0.7/gene4mVCF/__init__.py
+-rwxrwxr-x   0 ws2024    (1000) ws2024    (1000)     4665 2024-05-20 10:22:02.000000 gene4mvcf-1.0.7/gene4mVCF/gene4mvcf.py
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 10:42:54.535939 gene4mvcf-1.0.7/gene4mVCF.egg-info/
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     1762 2024-05-20 10:42:54.000000 gene4mvcf-1.0.7/gene4mVCF.egg-info/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      263 2024-05-20 10:42:54.000000 gene4mvcf-1.0.7/gene4mVCF.egg-info/SOURCES.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-05-20 10:42:54.000000 gene4mvcf-1.0.7/gene4mVCF.egg-info/dependency_links.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       55 2024-05-20 10:42:54.000000 gene4mvcf-1.0.7/gene4mVCF.egg-info/entry_points.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       78 2024-05-20 10:42:54.000000 gene4mvcf-1.0.7/gene4mVCF.egg-info/requires.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       10 2024-05-20 10:42:54.000000 gene4mvcf-1.0.7/gene4mVCF.egg-info/top_level.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       38 2024-05-20 10:42:54.535939 gene4mvcf-1.0.7/setup.cfg
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1222 2024-05-20 10:42:38.000000 gene4mvcf-1.0.7/setup.py
```

### Comparing `gene4mvcf-1.0.6/PKG-INFO` & `gene4mvcf-1.0.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gene4mVCF
-Version: 1.0.6
+Version: 1.0.7
 Summary: Description of your package
 Home-page: https://github.com/VJ-Ulaganathan/gene4mVCF
 Author: Pr (France). Dr. rer. nat. Vijay K. ULAGANATHAN
 Author-email: vijay-kumar.ulaganathan@uni-tuebingen.de
 Description-Content-Type: text/markdown
 Requires-Dist: pysam>=0.16.0.1
 Requires-Dist: pandas>=1.0.0
@@ -27,24 +27,24 @@
 usage: `$ python3 gene4mVCF [-h] -i INPUT -g GENE`
 
 Extract variant entries for a specific gene or list of genes from a VCF file.
 
 optional arguments:
   -h, --help            show this help message and exit
   -i INPUT, --input INPUT
-                        Input VCF file
+                        Input bgzip compressed VCF file
   -g GENES, --genes GENES
                         Gene name, Ensembl gene ID, or path to a gene list file
 
 ## Examples
 Extract variants for a single gene:
-`$ python3 gene4mVCF -i input.vcf -g ENSG00000168878`
+`$ python3 gene4mVCF -i input.vcf.gz -g ENSG00000168878`
 
 Extract variants for multiple genes listed in a file:
-`$ python3 gene4mVCF -i input.vcf -g genes.txt`
+`$ python3 gene4mVCF -i input.vcf.gz -g genes.txt`
 
 For more options and details, refer to the help message.
 
 ## Support
 For any issues or inquiries, please open an issue on the GitHub repository `https://github.com/VJ-Ulaganathan/gene4mVCF`
```

### Comparing `gene4mvcf-1.0.6/README.md` & `gene4mvcf-1.0.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 usage: `$ python3 gene4mVCF [-h] -i INPUT -g GENE`
 
 Extract variant entries for a specific gene or list of genes from a VCF file.
 
 optional arguments:
   -h, --help            show this help message and exit
   -i INPUT, --input INPUT
-                        Input VCF file
+                        Input bgzip compressed VCF file
   -g GENES, --genes GENES
                         Gene name, Ensembl gene ID, or path to a gene list file
 
 ## Examples
 Extract variants for a single gene:
-`$ python3 gene4mVCF -i input.vcf -g ENSG00000168878`
+`$ python3 gene4mVCF -i input.vcf.gz -g ENSG00000168878`
 
 Extract variants for multiple genes listed in a file:
-`$ python3 gene4mVCF -i input.vcf -g genes.txt`
+`$ python3 gene4mVCF -i input.vcf.gz -g genes.txt`
 
 For more options and details, refer to the help message.
 
 ## Support
 For any issues or inquiries, please open an issue on the GitHub repository `https://github.com/VJ-Ulaganathan/gene4mVCF`
```

### Comparing `gene4mvcf-1.0.6/gene4mVCF/gene4mvcf.py` & `gene4mvcf-1.0.7/gene4mVCF/gene4mvcf.py`

 * *Files identical despite different names*

### Comparing `gene4mvcf-1.0.6/gene4mVCF.egg-info/PKG-INFO` & `gene4mvcf-1.0.7/gene4mVCF.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gene4mVCF
-Version: 1.0.6
+Version: 1.0.7
 Summary: Description of your package
 Home-page: https://github.com/VJ-Ulaganathan/gene4mVCF
 Author: Pr (France). Dr. rer. nat. Vijay K. ULAGANATHAN
 Author-email: vijay-kumar.ulaganathan@uni-tuebingen.de
 Description-Content-Type: text/markdown
 Requires-Dist: pysam>=0.16.0.1
 Requires-Dist: pandas>=1.0.0
@@ -27,24 +27,24 @@
 usage: `$ python3 gene4mVCF [-h] -i INPUT -g GENE`
 
 Extract variant entries for a specific gene or list of genes from a VCF file.
 
 optional arguments:
   -h, --help            show this help message and exit
   -i INPUT, --input INPUT
-                        Input VCF file
+                        Input bgzip compressed VCF file
   -g GENES, --genes GENES
                         Gene name, Ensembl gene ID, or path to a gene list file
 
 ## Examples
 Extract variants for a single gene:
-`$ python3 gene4mVCF -i input.vcf -g ENSG00000168878`
+`$ python3 gene4mVCF -i input.vcf.gz -g ENSG00000168878`
 
 Extract variants for multiple genes listed in a file:
-`$ python3 gene4mVCF -i input.vcf -g genes.txt`
+`$ python3 gene4mVCF -i input.vcf.gz -g genes.txt`
 
 For more options and details, refer to the help message.
 
 ## Support
 For any issues or inquiries, please open an issue on the GitHub repository `https://github.com/VJ-Ulaganathan/gene4mVCF`
```

### Comparing `gene4mvcf-1.0.6/setup.py` & `gene4mvcf-1.0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # Check if all required commands exist
 if not all(command_exists(cmd) for cmd in required_commands):
     raise RuntimeError("Please install the following dependencies: bcftools, bgzip, tabix")
 
 setup(
     name='gene4mVCF',
-    version='1.0.6',
+    version='1.0.7',
     description='Description of your package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Pr (France). Dr. rer. nat. Vijay K. ULAGANATHAN',
     author_email='vijay-kumar.ulaganathan@uni-tuebingen.de',
     url='https://github.com/VJ-Ulaganathan/gene4mVCF',
     packages=find_packages(),
```

