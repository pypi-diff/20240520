# Comparing `tmp/gene4mvcf-1.0.0.tar.gz` & `tmp/gene4mvcf-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gene4mvcf-1.0.0.tar", last modified: Mon May 20 09:46:44 2024, max compression
+gzip compressed data, was "gene4mvcf-1.0.1.tar", last modified: Mon May 20 09:54:33 2024, max compression
```

## Comparing `gene4mvcf-1.0.0.tar` & `gene4mvcf-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 09:46:44.029299 gene4mvcf-1.0.0/
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      296 2024-05-20 09:46:44.025299 gene4mvcf-1.0.0/PKG-INFO
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 09:36:02.000000 gene4mvcf-1.0.0/README.md
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 09:46:44.025299 gene4mvcf-1.0.0/gene4mvcf.egg-info/
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      296 2024-05-20 09:46:43.000000 gene4mvcf-1.0.0/gene4mvcf.egg-info/PKG-INFO
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      182 2024-05-20 09:46:43.000000 gene4mvcf-1.0.0/gene4mvcf.egg-info/SOURCES.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-05-20 09:46:43.000000 gene4mvcf-1.0.0/gene4mvcf.egg-info/dependency_links.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       34 2024-05-20 09:46:43.000000 gene4mvcf-1.0.0/gene4mvcf.egg-info/requires.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-05-20 09:46:43.000000 gene4mvcf-1.0.0/gene4mvcf.egg-info/top_level.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       38 2024-05-20 09:46:44.029299 gene4mvcf-1.0.0/setup.cfg
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1104 2024-05-20 09:35:35.000000 gene4mvcf-1.0.0/setup.py
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 09:54:33.262079 gene4mvcf-1.0.1/
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     1822 2024-05-20 09:54:33.262079 gene4mvcf-1.0.1/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1476 2024-05-20 09:45:42.000000 gene4mvcf-1.0.1/README.md
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 09:54:33.262079 gene4mvcf-1.0.1/gene4mvcf.egg-info/
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     1822 2024-05-20 09:54:33.000000 gene4mvcf-1.0.1/gene4mvcf.egg-info/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      182 2024-05-20 09:54:33.000000 gene4mvcf-1.0.1/gene4mvcf.egg-info/SOURCES.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-05-20 09:54:33.000000 gene4mvcf-1.0.1/gene4mvcf.egg-info/dependency_links.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       34 2024-05-20 09:54:33.000000 gene4mvcf-1.0.1/gene4mvcf.egg-info/requires.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-05-20 09:54:33.000000 gene4mvcf-1.0.1/gene4mvcf.egg-info/top_level.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       38 2024-05-20 09:54:33.262079 gene4mvcf-1.0.1/setup.cfg
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1104 2024-05-20 09:53:53.000000 gene4mvcf-1.0.1/setup.py
```

### Comparing `gene4mvcf-1.0.0/setup.py` & `gene4mvcf-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # Check if all required commands exist
 if not all(command_exists(cmd) for cmd in required_commands):
     raise RuntimeError("Please install the following dependencies: bcftools, bgzip, tabix")
 
 setup(
     name='gene4mvcf',
-    version='1.0.0',
+    version='1.0.1',
     description='Description of your package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Pr (France). Dr. rer. nat. Vijay K. ULAGANATHAN',
     author_email='vijay-kumar.ulaganathan@uni-tuebingen.de',
     url='https://github.com/VJ-Ulaganathan/gene4mVCF',
     packages=find_packages(),
```

