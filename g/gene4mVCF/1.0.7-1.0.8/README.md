# Comparing `tmp/gene4mvcf-1.0.7.tar.gz` & `tmp/gene4mVCF-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gene4mvcf-1.0.7.tar", last modified: Mon May 20 10:42:54 2024, max compression
+gzip compressed data, was "gene4mVCF-1.0.8.tar", last modified: Mon May 20 10:50:19 2024, max compression
```

## Comparing `gene4mvcf-1.0.7.tar` & `gene4mVCF-1.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 10:42:54.535939 gene4mvcf-1.0.7/
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)     1762 2024-05-20 10:42:54.535939 gene4mvcf-1.0.7/PKG-INFO
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1312 2024-05-20 10:42:40.000000 gene4mvcf-1.0.7/README.md
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 10:42:54.535939 gene4mvcf-1.0.7/gene4mVCF/
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        0 2024-05-17 19:50:34.000000 gene4mvcf-1.0.7/gene4mVCF/__init__.py
--rwxrwxr-x   0 ws2024    (1000) ws2024    (1000)     4665 2024-05-20 10:22:02.000000 gene4mvcf-1.0.7/gene4mVCF/gene4mvcf.py
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 10:42:54.535939 gene4mvcf-1.0.7/gene4mVCF.egg-info/
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)     1762 2024-05-20 10:42:54.000000 gene4mvcf-1.0.7/gene4mVCF.egg-info/PKG-INFO
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      263 2024-05-20 10:42:54.000000 gene4mvcf-1.0.7/gene4mVCF.egg-info/SOURCES.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-05-20 10:42:54.000000 gene4mvcf-1.0.7/gene4mVCF.egg-info/dependency_links.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       55 2024-05-20 10:42:54.000000 gene4mvcf-1.0.7/gene4mVCF.egg-info/entry_points.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       78 2024-05-20 10:42:54.000000 gene4mvcf-1.0.7/gene4mVCF.egg-info/requires.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       10 2024-05-20 10:42:54.000000 gene4mvcf-1.0.7/gene4mVCF.egg-info/top_level.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       38 2024-05-20 10:42:54.535939 gene4mvcf-1.0.7/setup.cfg
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1222 2024-05-20 10:42:38.000000 gene4mvcf-1.0.7/setup.py
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 10:50:19.552696 gene4mVCF-1.0.8/
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1606 2024-05-20 10:50:19.552696 gene4mVCF-1.0.8/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1309 2024-05-20 10:48:17.000000 gene4mVCF-1.0.8/README.md
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 10:50:19.552696 gene4mVCF-1.0.8/gene4mVCF/
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        0 2024-05-17 19:50:34.000000 gene4mVCF-1.0.8/gene4mVCF/__init__.py
+-rwxrwxr-x   0 ws2024    (1000) ws2024    (1000)     4665 2024-05-20 10:22:02.000000 gene4mVCF-1.0.8/gene4mVCF/gene4mvcf.py
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 10:50:19.552696 gene4mVCF-1.0.8/gene4mVCF.egg-info/
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1606 2024-05-20 10:50:19.000000 gene4mVCF-1.0.8/gene4mVCF.egg-info/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      263 2024-05-20 10:50:19.000000 gene4mVCF-1.0.8/gene4mVCF.egg-info/SOURCES.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-05-20 10:50:19.000000 gene4mVCF-1.0.8/gene4mVCF.egg-info/dependency_links.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       55 2024-05-20 10:50:19.000000 gene4mVCF-1.0.8/gene4mVCF.egg-info/entry_points.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       78 2024-05-20 10:50:19.000000 gene4mVCF-1.0.8/gene4mVCF.egg-info/requires.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       10 2024-05-20 10:50:19.000000 gene4mVCF-1.0.8/gene4mVCF.egg-info/top_level.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       38 2024-05-20 10:50:19.552696 gene4mVCF-1.0.8/setup.cfg
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1222 2024-05-20 10:48:15.000000 gene4mVCF-1.0.8/setup.py
```

### Comparing `gene4mvcf-1.0.7/PKG-INFO` & `gene4mVCF-1.0.8/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: gene4mVCF
-Version: 1.0.7
-Summary: Description of your package
-Home-page: https://github.com/VJ-Ulaganathan/gene4mVCF
-Author: Pr (France). Dr. rer. nat. Vijay K. ULAGANATHAN
-Author-email: vijay-kumar.ulaganathan@uni-tuebingen.de
-Description-Content-Type: text/markdown
-Requires-Dist: pysam>=0.16.0.1
-Requires-Dist: pandas>=1.0.0
-Requires-Dist: pybedtools>=0.8.0
-Requires-Dist: tqdm>=4.47.0
-Requires-Dist: gffutils>=0.10.1
-
 # gene4mVCF
 
 ## Introduction
 `gene4mVCF` is a Python package that allows you to extract variant entries for specific genes or a list of genes from a VCF (Variant Call Format) file. It utilizes tools like `bcftools`, `tabix`, and Python libraries like `pysam`, `pandas`, `pybedtools`, `tqdm`, and `gffutils` to efficiently parse and extract variants.
 
 ## Installation
 
@@ -41,15 +27,15 @@
 
 Extract variants for multiple genes listed in a file:
 `$ python3 gene4mVCF -i input.vcf.gz -g genes.txt`
 
 For more options and details, refer to the help message.
 
 ## Support
-For any issues or inquiries, please open an issue on the GitHub repository `https://github.com/VJ-Ulaganathan/gene4mVCF` 
+For any issues or inquiries, please open an issue on the GitHub repository https://github.com/VJ-Ulaganathan/gene4mVCF
 
 
 ## Installation
 
 Installation via pip:
 
 `$ pip install gene4mVCF`
```

### Comparing `gene4mvcf-1.0.7/gene4mVCF/gene4mvcf.py` & `gene4mVCF-1.0.8/gene4mVCF/gene4mvcf.py`

 * *Files identical despite different names*

### Comparing `gene4mvcf-1.0.7/gene4mVCF.egg-info/PKG-INFO` & `gene4mVCF-1.0.8/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 Metadata-Version: 2.1
 Name: gene4mVCF
-Version: 1.0.7
+Version: 1.0.8
 Summary: Description of your package
 Home-page: https://github.com/VJ-Ulaganathan/gene4mVCF
 Author: Pr (France). Dr. rer. nat. Vijay K. ULAGANATHAN
 Author-email: vijay-kumar.ulaganathan@uni-tuebingen.de
 Description-Content-Type: text/markdown
-Requires-Dist: pysam>=0.16.0.1
-Requires-Dist: pandas>=1.0.0
-Requires-Dist: pybedtools>=0.8.0
-Requires-Dist: tqdm>=4.47.0
-Requires-Dist: gffutils>=0.10.1
 
 # gene4mVCF
 
 ## Introduction
 `gene4mVCF` is a Python package that allows you to extract variant entries for specific genes or a list of genes from a VCF (Variant Call Format) file. It utilizes tools like `bcftools`, `tabix`, and Python libraries like `pysam`, `pandas`, `pybedtools`, `tqdm`, and `gffutils` to efficiently parse and extract variants.
 
 ## Installation
@@ -41,15 +36,15 @@
 
 Extract variants for multiple genes listed in a file:
 `$ python3 gene4mVCF -i input.vcf.gz -g genes.txt`
 
 For more options and details, refer to the help message.
 
 ## Support
-For any issues or inquiries, please open an issue on the GitHub repository `https://github.com/VJ-Ulaganathan/gene4mVCF` 
+For any issues or inquiries, please open an issue on the GitHub repository https://github.com/VJ-Ulaganathan/gene4mVCF
 
 
 ## Installation
 
 Installation via pip:
 
 `$ pip install gene4mVCF`
```

### Comparing `gene4mvcf-1.0.7/setup.py` & `gene4mVCF-1.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # Check if all required commands exist
 if not all(command_exists(cmd) for cmd in required_commands):
     raise RuntimeError("Please install the following dependencies: bcftools, bgzip, tabix")
 
 setup(
     name='gene4mVCF',
-    version='1.0.7',
+    version='1.0.8',
     description='Description of your package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Pr (France). Dr. rer. nat. Vijay K. ULAGANATHAN',
     author_email='vijay-kumar.ulaganathan@uni-tuebingen.de',
     url='https://github.com/VJ-Ulaganathan/gene4mVCF',
     packages=find_packages(),
```

