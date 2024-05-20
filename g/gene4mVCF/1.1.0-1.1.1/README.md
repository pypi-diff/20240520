# Comparing `tmp/gene4mvcf-1.1.0.tar.gz` & `tmp/gene4mvcf-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gene4mvcf-1.1.0.tar", last modified: Mon May 20 11:33:24 2024, max compression
+gzip compressed data, was "gene4mvcf-1.1.1.tar", last modified: Mon May 20 12:23:28 2024, max compression
```

## Comparing `gene4mvcf-1.1.0.tar` & `gene4mvcf-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 11:33:24.065985 gene4mvcf-1.1.0/
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)     1773 2024-05-20 11:33:24.065985 gene4mvcf-1.1.0/PKG-INFO
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1323 2024-05-20 11:33:00.000000 gene4mvcf-1.1.0/README.md
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 11:33:24.065985 gene4mvcf-1.1.0/gene4mVCF/
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 11:07:18.000000 gene4mvcf-1.1.0/gene4mVCF/__init__.py
--rwxrwxr-x   0 ws2024    (1000) ws2024    (1000)     4665 2024-05-20 10:22:02.000000 gene4mvcf-1.1.0/gene4mVCF/fetchgenes.py
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 11:33:24.065985 gene4mvcf-1.1.0/gene4mVCF.egg-info/
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)     1773 2024-05-20 11:33:24.000000 gene4mvcf-1.1.0/gene4mVCF.egg-info/PKG-INFO
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      264 2024-05-20 11:33:24.000000 gene4mvcf-1.1.0/gene4mVCF.egg-info/SOURCES.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-05-20 11:33:24.000000 gene4mvcf-1.1.0/gene4mVCF.egg-info/dependency_links.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       56 2024-05-20 11:33:24.000000 gene4mvcf-1.1.0/gene4mVCF.egg-info/entry_points.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       78 2024-05-20 11:33:24.000000 gene4mvcf-1.1.0/gene4mVCF.egg-info/requires.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       10 2024-05-20 11:33:24.000000 gene4mvcf-1.1.0/gene4mVCF.egg-info/top_level.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       38 2024-05-20 11:33:24.065985 gene4mvcf-1.1.0/setup.cfg
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1343 2024-05-20 11:32:51.000000 gene4mvcf-1.1.0/setup.py
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 12:23:28.126169 gene4mvcf-1.1.1/
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     1843 2024-05-20 12:23:28.126169 gene4mvcf-1.1.1/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1393 2024-05-20 11:47:55.000000 gene4mvcf-1.1.1/README.md
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 12:23:28.126169 gene4mvcf-1.1.1/gene4mVCF/
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 11:07:18.000000 gene4mvcf-1.1.1/gene4mVCF/__init__.py
+-rwxrwxr-x   0 ws2024    (1000) ws2024    (1000)     4379 2024-05-20 12:13:50.000000 gene4mvcf-1.1.1/gene4mVCF/fetchgenes.py
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 12:23:28.126169 gene4mvcf-1.1.1/gene4mVCF.egg-info/
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     1843 2024-05-20 12:23:28.000000 gene4mvcf-1.1.1/gene4mVCF.egg-info/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      264 2024-05-20 12:23:28.000000 gene4mvcf-1.1.1/gene4mVCF.egg-info/SOURCES.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-05-20 12:23:28.000000 gene4mvcf-1.1.1/gene4mVCF.egg-info/dependency_links.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       56 2024-05-20 12:23:28.000000 gene4mvcf-1.1.1/gene4mVCF.egg-info/entry_points.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       78 2024-05-20 12:23:28.000000 gene4mvcf-1.1.1/gene4mVCF.egg-info/requires.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       10 2024-05-20 12:23:28.000000 gene4mvcf-1.1.1/gene4mVCF.egg-info/top_level.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       38 2024-05-20 12:23:28.126169 gene4mvcf-1.1.1/setup.cfg
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1343 2024-05-20 11:48:03.000000 gene4mvcf-1.1.1/setup.py
```

### Comparing `gene4mvcf-1.1.0/PKG-INFO` & `gene4mvcf-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gene4mVCF
-Version: 1.1.0
+Version: 1.1.1
 Summary: Description of your package
 Home-page: https://github.com/VJ-Ulaganathan/gene4mVCF
 Author: Pr (France). Dr. rer. nat. Vijay K. ULAGANATHAN
 Author-email: vijay-kumar.ulaganathan@uni-tuebingen.de
 Description-Content-Type: text/markdown
 Requires-Dist: pysam>=0.16.0.1
 Requires-Dist: pandas>=1.0.0
@@ -32,16 +32,18 @@
   -h, --help            show this help message and exit
   -i INPUT, --input INPUT
                         Input bgzip compressed VCF file
   -g GENES, --genes GENES
                         Gene name, Ensembl gene ID, or path to a gene list file
 
 ## Examples
-Extract variants for a single gene:
+Extract variants for a single gene using gene name:
 `$ gene4mVCF -i input.vcf.gz -g EGFR`
+
+Extract variants for a single using ensembl gene id:
 `$ gene4mVCF -i input.vcf.gz -g ENSG00000168878`
 
 Extract variants for multiple genes listed in a file:
 `$ gene4mVCF -i input.vcf.gz -g genes.txt`
 
 For more options and details, refer to the help message.
```

### Comparing `gene4mvcf-1.1.0/README.md` & `gene4mvcf-1.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -18,16 +18,18 @@
   -h, --help            show this help message and exit
   -i INPUT, --input INPUT
                         Input bgzip compressed VCF file
   -g GENES, --genes GENES
                         Gene name, Ensembl gene ID, or path to a gene list file
 
 ## Examples
-Extract variants for a single gene:
+Extract variants for a single gene using gene name:
 `$ gene4mVCF -i input.vcf.gz -g EGFR`
+
+Extract variants for a single using ensembl gene id:
 `$ gene4mVCF -i input.vcf.gz -g ENSG00000168878`
 
 Extract variants for multiple genes listed in a file:
 `$ gene4mVCF -i input.vcf.gz -g genes.txt`
 
 For more options and details, refer to the help message.
```

### Comparing `gene4mvcf-1.1.0/gene4mVCF/fetchgenes.py` & `gene4mvcf-1.1.1/gene4mVCF/fetchgenes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python
-
 import argparse
 import subprocess
 import os
 import gzip
 from tqdm import tqdm
 
 def parse_bed_file(gene_identifier, genome_version):
@@ -14,16 +12,19 @@
             bed_file = "hg19.ncbiRefSeq.bed"
     elif "hg38" in genome_version:
         if gene_identifier.startswith("ENSG"):
             bed_file = "hg38.ensGene.bed"
         else:
             bed_file = "hg38.ncbiRefSeq.bed"
     else:
-        print("Warning: Genome version cannot be determined. Defaulting to hg19/GRCh37.")
-        bed_file = "hg19.ensGene.bed"  # Default to hg19 if genome version cannot be determined
+        # Default to hg19 if genome version cannot be determined
+        if gene_identifier.startswith("ENSG"):
+            bed_file = "hg19.ensGene.bed"
+        else:
+            bed_file = "hg19.ncbiRefSeq.bed"
 
     gene_regions = {}
     with open(bed_file, 'r') as file:
         for line in file:
             fields = line.strip().split('\t')
             chrom = fields[0].lstrip("chr")
             start = int(fields[1])
@@ -42,23 +43,19 @@
         raise ValueError(f"Gene {gene_identifier} not found in {bed_file}")
     return gene_regions
 
 def get_reference_genome(vcf_path):
     reference_genome = None
     with gzip.open(vcf_path, 'rt') as file:
         for line in file:
-            if line.startswith("##contig=<ID="):
-                if "hg19" in line:
-                    reference_genome = "hg19/GRCh37"
-                elif "hg38" in line:
-                    reference_genome = "hg38/GRCh38"
+            if line.startswith("#CHROM"):
+                reference_genome = line.strip()
                 break
     if reference_genome is None:
-        print("Warning: Genome version cannot be determined from the input file. Defaulting to hg19/GRCh37.")
-        reference_genome = "hg19/GRCh37"  # Default to hg19/GRCh37 if genome version cannot be determined
+        raise ValueError("No header line found in VCF file")
     return reference_genome
 
 def get_gene_info(chrom, pos, gene_regions):
     for (region_chrom, start, end), (gene_name, feature) in gene_regions.items():
         if region_chrom == chrom and start <= pos <= end:
             return gene_name, feature
     return "", ""
@@ -68,16 +65,16 @@
     parser.add_argument('-i', '--input', required=True, help='Input VCF file')
     parser.add_argument('-g', '--genes', required=True, help='Gene name, Ensembl gene ID, or path to a gene list file')
 
     args = parser.parse_args()
 
     genome_version = get_reference_genome(args.input)
 
-    if genome_version:
-        print(f"Detected reference genome version: {genome_version}")
+    #if genome_version:
+        #print(f"Detected reference genome version: {genome_version}")
 
     if args.genes.endswith('.txt'):
         with open(args.genes, 'r') as gene_list_file:
             gene_list = [line.strip() for line in gene_list_file]
     else:
         gene_list = [args.genes]
```

### Comparing `gene4mvcf-1.1.0/gene4mVCF.egg-info/PKG-INFO` & `gene4mvcf-1.1.1/gene4mVCF.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gene4mVCF
-Version: 1.1.0
+Version: 1.1.1
 Summary: Description of your package
 Home-page: https://github.com/VJ-Ulaganathan/gene4mVCF
 Author: Pr (France). Dr. rer. nat. Vijay K. ULAGANATHAN
 Author-email: vijay-kumar.ulaganathan@uni-tuebingen.de
 Description-Content-Type: text/markdown
 Requires-Dist: pysam>=0.16.0.1
 Requires-Dist: pandas>=1.0.0
@@ -32,16 +32,18 @@
   -h, --help            show this help message and exit
   -i INPUT, --input INPUT
                         Input bgzip compressed VCF file
   -g GENES, --genes GENES
                         Gene name, Ensembl gene ID, or path to a gene list file
 
 ## Examples
-Extract variants for a single gene:
+Extract variants for a single gene using gene name:
 `$ gene4mVCF -i input.vcf.gz -g EGFR`
+
+Extract variants for a single using ensembl gene id:
 `$ gene4mVCF -i input.vcf.gz -g ENSG00000168878`
 
 Extract variants for multiple genes listed in a file:
 `$ gene4mVCF -i input.vcf.gz -g genes.txt`
 
 For more options and details, refer to the help message.
```

### Comparing `gene4mvcf-1.1.0/setup.py` & `gene4mvcf-1.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # Check if all required commands exist
 if not all(command_exists(cmd) for cmd in required_commands):
     raise RuntimeError("Please install the following dependencies: bcftools, bgzip, tabix")
 
 setup(
     name='gene4mVCF',
-    version='1.1.0',
+    version='1.1.1',
     description='Description of your package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Pr (France). Dr. rer. nat. Vijay K. ULAGANATHAN',
     author_email='vijay-kumar.ulaganathan@uni-tuebingen.de',
     url='https://github.com/VJ-Ulaganathan/gene4mVCF',
     packages=find_packages(),
```

