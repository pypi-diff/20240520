# Comparing `tmp/greatbrowser-1.0.3.tar.gz` & `tmp/greatbrowser-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "greatbrowser-1.0.3.tar", last modified: Sun May 19 03:43:31 2024, max compression
+gzip compressed data, was "greatbrowser-1.0.4.tar", last modified: Mon May 20 19:00:29 2024, max compression
```

## Comparing `greatbrowser-1.0.3.tar` & `greatbrowser-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 03:43:31.375477 greatbrowser-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-19 03:43:19.000000 greatbrowser-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-19 03:43:31.375477 greatbrowser-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-19 03:43:19.000000 greatbrowser-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 03:43:31.375477 greatbrowser-1.0.3/greatbrowser/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-19 03:43:19.000000 greatbrowser-1.0.3/greatbrowser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16850 2024-05-19 03:43:19.000000 greatbrowser-1.0.3/greatbrowser/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13387 2024-05-19 03:43:19.000000 greatbrowser-1.0.3/greatbrowser/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 03:43:31.375477 greatbrowser-1.0.3/greatbrowser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-19 03:43:31.000000 greatbrowser-1.0.3/greatbrowser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-19 03:43:31.000000 greatbrowser-1.0.3/greatbrowser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 03:43:31.000000 greatbrowser-1.0.3/greatbrowser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-19 03:43:31.000000 greatbrowser-1.0.3/greatbrowser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-19 03:43:31.000000 greatbrowser-1.0.3/greatbrowser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 03:43:31.375477 greatbrowser-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-19 03:43:19.000000 greatbrowser-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:29.728119 greatbrowser-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-20 19:00:19.000000 greatbrowser-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-20 19:00:29.728119 greatbrowser-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-20 19:00:19.000000 greatbrowser-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:29.728119 greatbrowser-1.0.4/greatbrowser/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-20 19:00:19.000000 greatbrowser-1.0.4/greatbrowser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17115 2024-05-20 19:00:19.000000 greatbrowser-1.0.4/greatbrowser/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13482 2024-05-20 19:00:19.000000 greatbrowser-1.0.4/greatbrowser/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:29.728119 greatbrowser-1.0.4/greatbrowser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-20 19:00:29.000000 greatbrowser-1.0.4/greatbrowser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-20 19:00:29.000000 greatbrowser-1.0.4/greatbrowser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 19:00:29.000000 greatbrowser-1.0.4/greatbrowser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-20 19:00:29.000000 greatbrowser-1.0.4/greatbrowser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-20 19:00:29.000000 greatbrowser-1.0.4/greatbrowser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 19:00:29.728119 greatbrowser-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-20 19:00:19.000000 greatbrowser-1.0.4/setup.py
```

### Comparing `greatbrowser-1.0.3/LICENSE` & `greatbrowser-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `greatbrowser-1.0.3/PKG-INFO` & `greatbrowser-1.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: greatbrowser
-Version: 1.0.3
+Version: 1.0.4
 Summary: Automate Stanford's GREAT browser
 Author: Sam Anderson
 Author-email: sanderson01@wesleyan.edu
 Project-URL: Source, https://github.com/SamAndTheSun/greatbrowser
 Project-URL: Bug Reports, https://github.com/SamAndTheSun/greatbrowser/issues
 Keywords: python,genomics,genetics,greatbrowser,great,automated,analysis
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# greatbrowser v1.0.3
+# greatbrowser v1.0.4
 A selenium implementation in python for Stanford's GREAT browser, allowing for quick and easy genomic analysis.
 
 This repository can be installed as a module
 
 ```
 pip install greatbrowser
 ```
@@ -34,15 +34,15 @@
 
 The user experience is primarily built around a single function, great_analysis(), with the complementary functions great_get_options() and great_global_controls()
 providing context regarding some of the parameters for this function.
 
 The current version supports the ability to find gene associations using probe sets as well the ability to download any GREAT-generated table or plot in dataframe form. 
 UCSC genome browser implementation is also supported. Customizability is controlled through parameter tuning, some of which are specific, 
 while others are encapsulated within the "global_settings" dictionary parameter as key options. More specific information is available in the great_analysis() docstring. 
-Because the project uses switch statements, its requires python >= 3.10 to run.
+Because the project uses switch statements, its requires python >= 3.10 to run. Analysis is limited to <200,000 regions.
 
 This repository is ideal for individuals attempting to conduct many different analyses using GREAT across many different probe sets. 
 It is fully functional with regards to its ability to modify table output settings, 
 but is not ideal if one desires to perform highly custom visual modifications to specifically the raw barplot or hierarchy plots generated by GREAT. 
 
 This repository is not affiliated with the official GREAT browser and was developed solely for the sake of convenience.
```

### Comparing `greatbrowser-1.0.3/README.md` & `greatbrowser-1.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# greatbrowser v1.0.3
+# greatbrowser v1.0.4
 A selenium implementation in python for Stanford's GREAT browser, allowing for quick and easy genomic analysis.
 
 This repository can be installed as a module
 
 ```
 pip install greatbrowser
 ```
@@ -17,15 +17,15 @@
 
 The user experience is primarily built around a single function, great_analysis(), with the complementary functions great_get_options() and great_global_controls()
 providing context regarding some of the parameters for this function.
 
 The current version supports the ability to find gene associations using probe sets as well the ability to download any GREAT-generated table or plot in dataframe form. 
 UCSC genome browser implementation is also supported. Customizability is controlled through parameter tuning, some of which are specific, 
 while others are encapsulated within the "global_settings" dictionary parameter as key options. More specific information is available in the great_analysis() docstring. 
-Because the project uses switch statements, its requires python >= 3.10 to run.
+Because the project uses switch statements, its requires python >= 3.10 to run. Analysis is limited to <200,000 regions.
 
 This repository is ideal for individuals attempting to conduct many different analyses using GREAT across many different probe sets. 
 It is fully functional with regards to its ability to modify table output settings, 
 but is not ideal if one desires to perform highly custom visual modifications to specifically the raw barplot or hierarchy plots generated by GREAT. 
 
 This repository is not affiliated with the official GREAT browser and was developed solely for the sake of convenience.
```

### Comparing `greatbrowser-1.0.3/greatbrowser/functions.py` & `greatbrowser-1.0.4/greatbrowser/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,17 @@
     elif isinstance(bed_data, str):
         try: bed_data = pd.read_excel(bed_data)
         except: bed_data = pd.read_csv(bed_data)
 
     #format df
     if isinstance(bed_data, pd.DataFrame) or isinstance(bed_data, pl.DataFrame):
 
+        bed_data[df_start] = bed_data[df_start].astype(int)
+        bed_data[df_end] = bed_data[df_end].astype(int)
+
         n = 0
         if isinstance(bed_data, pd.DataFrame) or isinstance(bed_data, pl.DataFrame):
             while n < bed_data.shape[1]: #get appropriate columns
                 try: df_dict[potential_cols[n]] = bed_data[potential_cols[n]]
                 except: pass
                 n+=1
         elif isinstance(bed_data, np.ndarray):
@@ -81,14 +84,18 @@
         if potential_cols[0] not in df_dict: raise Exception(f'KeyError: "{df_chr}" not found in columns')
         if potential_cols[1] not in df_dict: raise Exception(f'KeyError: "{df_start}" not found in columns')
         if potential_cols[2] not in df_dict: raise Exception(f'KeyError: "{df_end}" not found in columns')
 
     else:
         print('Invalid file type detected. Must be either pandas dataframe, polars dataframe, list, numpy array, or path (str)')
 
+    #add _ to all indices to differentiate them from genes in parsing
+    bed_data[df_index] = bed_data[df_index].astype(str)   
+    bed_data[df_index] = bed_data[df_index] + '_'
+
     return bed_data
 
 def get_genes(driver):
     '''
     get the gene table for a given region set
         param driver: the driver focused on the webpage of interest
 
@@ -118,15 +125,15 @@
 
     #prepare to create list of genes from table
     gene_by_ids = []
     gene_list = []
 
     #Extract gene names / positions by id
     for tag in gene_tags:
-        if ('+' not in tag.text) and ('-' not in tag.text): #differentiate between indices and values
+        if '_' in tag.text: #differentiate between indices and values
             gene_by_ids.append(gene_list)
             gene_list = []
         else:
             gene_list.append(tag.text)
     
     return gene_by_ids
```

### Comparing `greatbrowser-1.0.3/greatbrowser/main.py` & `greatbrowser-1.0.4/greatbrowser/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,16 @@
         adjust_global_controls(driver, global_controls)
 
     #get desired data
     output = False #default output
     n_table = False #default table
     match get:
         case 'genes':
-            output = test_regions 
+            test_regions[df_index] = test_regions[df_index].str.slice(0, -1) #remove added '_'
+            output = test_regions
             output['associated_genes'] = get_genes(driver)
         case 'ucsc_browser': get_ucsc_browser(driver) 
         case 'genes_pivot': output = get_genes_pivot(driver)
         case 'n_genes_region': get_n_genes_region(driver, 0, file_name, get)
         case 'n_genes_TSS': get_n_genes_region(driver, 1, file_name, get)
         case 'n_genes_abs_TSS': get_n_genes_region(driver, 2, file_name, get)
         case 'ensembl_genes': n_table = 0; output = get_table(driver, n_table)
```

### Comparing `greatbrowser-1.0.3/greatbrowser.egg-info/PKG-INFO` & `greatbrowser-1.0.4/greatbrowser.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: greatbrowser
-Version: 1.0.3
+Version: 1.0.4
 Summary: Automate Stanford's GREAT browser
 Author: Sam Anderson
 Author-email: sanderson01@wesleyan.edu
 Project-URL: Source, https://github.com/SamAndTheSun/greatbrowser
 Project-URL: Bug Reports, https://github.com/SamAndTheSun/greatbrowser/issues
 Keywords: python,genomics,genetics,greatbrowser,great,automated,analysis
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# greatbrowser v1.0.3
+# greatbrowser v1.0.4
 A selenium implementation in python for Stanford's GREAT browser, allowing for quick and easy genomic analysis.
 
 This repository can be installed as a module
 
 ```
 pip install greatbrowser
 ```
@@ -34,15 +34,15 @@
 
 The user experience is primarily built around a single function, great_analysis(), with the complementary functions great_get_options() and great_global_controls()
 providing context regarding some of the parameters for this function.
 
 The current version supports the ability to find gene associations using probe sets as well the ability to download any GREAT-generated table or plot in dataframe form. 
 UCSC genome browser implementation is also supported. Customizability is controlled through parameter tuning, some of which are specific, 
 while others are encapsulated within the "global_settings" dictionary parameter as key options. More specific information is available in the great_analysis() docstring. 
-Because the project uses switch statements, its requires python >= 3.10 to run.
+Because the project uses switch statements, its requires python >= 3.10 to run. Analysis is limited to <200,000 regions.
 
 This repository is ideal for individuals attempting to conduct many different analyses using GREAT across many different probe sets. 
 It is fully functional with regards to its ability to modify table output settings, 
 but is not ideal if one desires to perform highly custom visual modifications to specifically the raw barplot or hierarchy plots generated by GREAT. 
 
 This repository is not affiliated with the official GREAT browser and was developed solely for the sake of convenience.
```

### Comparing `greatbrowser-1.0.3/setup.py` & `greatbrowser-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.3'
+VERSION = '1.0.4'
 DESCRIPTION = "Automate Stanford's GREAT browser"
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
```

