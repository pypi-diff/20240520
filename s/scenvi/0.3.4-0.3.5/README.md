# Comparing `tmp/scenvi-0.3.4.tar.gz` & `tmp/scenvi-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scenvi-0.3.4.tar", max compression
+gzip compressed data, was "scenvi-0.3.5.tar", max compression
```

## Comparing `scenvi-0.3.4.tar` & `scenvi-0.3.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2024-02-20 21:59:17.777592 scenvi-0.3.4/LICENSE
--rw-r--r--   0        0        0     1891 2024-04-24 20:57:47.624722 scenvi-0.3.4/README.md
--rw-r--r--   0        0        0      434 2024-05-20 16:09:50.650075 scenvi-0.3.4/pyproject.toml
--rw-r--r--   0        0        0    24665 2024-05-20 16:09:17.568896 scenvi-0.3.4/scenvi/ENVI.py
--rw-r--r--   0        0        0       96 2024-04-26 18:55:35.962102 scenvi-0.3.4/scenvi/__init__.py
--rw-r--r--   0        0        0     1289 2024-04-26 18:55:10.183296 scenvi-0.3.4/scenvi/_dists.py
--rw-r--r--   0        0        0     8810 2024-05-20 16:08:12.362394 scenvi-0.3.4/scenvi/utils.py
--rw-r--r--   0        0        0     2661 1970-01-01 00:00:00.000000 scenvi-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-02-20 21:59:17.777592 scenvi-0.3.5/LICENSE
+-rw-r--r--   0        0        0     1891 2024-04-24 20:57:47.624722 scenvi-0.3.5/README.md
+-rw-r--r--   0        0        0      434 2024-05-20 16:19:47.978601 scenvi-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0    24689 2024-05-20 16:15:33.607257 scenvi-0.3.5/scenvi/ENVI.py
+-rw-r--r--   0        0        0       96 2024-04-26 18:55:35.962102 scenvi-0.3.5/scenvi/__init__.py
+-rw-r--r--   0        0        0     1289 2024-04-26 18:55:10.183296 scenvi-0.3.5/scenvi/_dists.py
+-rw-r--r--   0        0        0     8810 2024-05-20 16:08:12.362394 scenvi-0.3.5/scenvi/utils.py
+-rw-r--r--   0        0        0     2661 1970-01-01 00:00:00.000000 scenvi-0.3.5/PKG-INFO
```

### Comparing `scenvi-0.3.4/LICENSE` & `scenvi-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scenvi-0.3.4/README.md` & `scenvi-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `scenvi-0.3.4/scenvi/ENVI.py` & `scenvi-0.3.5/scenvi/ENVI.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,22 +78,22 @@
     ):
 
         self.spatial_data = spatial_data[:, np.intersect1d(spatial_data.var_names, sc_data.var_names)]
         self.sc_data = sc_data
 
         if "highly_variable" not in self.sc_data.var.columns:
             if 'log' in self.sc_data.layers.keys():
-                sc.pp.highly_variable_genes(self.sc_data, n_top_genes=g, layer="log")
+                sc.pp.highly_variable_genes(self.sc_data, n_top_genes=num_HVG, layer="log")
             elif('log1p' in self.sc_data.layers.keys()):
-                sc.pp.highly_variable_genes(self.sc_data, n_top_genes=g, layer="log1p")
+                sc.pp.highly_variable_genes(self.sc_data, n_top_genes=num_HVG, layer="log1p")
             elif(self.sc_data.X.min() < 0):
-                sc.pp.highly_variable_genes(self.sc_data, n_top_genes=g)
+                sc.pp.highly_variable_genes(self.sc_data, n_top_genes=num_HVG)
             else:
                 sc_data.layers["log"] = np.log(self.sc_data.X + 1)
-                sc.pp.highly_variable_genes(self.sc_data, n_top_genes=g, layer="log")
+                sc.pp.highly_variable_genes(self.sc_data, n_top_genes=num_HVG, layer="log")
 
         sc_genes_keep = np.union1d(
             self.sc_data.var_names[self.sc_data.var.highly_variable], self.spatial_data.var_names
         )
         if len(sc_genes) > 0:
             sc_genes_keep = np.union1d(sc_genes_keep, sc_genes)
```

### Comparing `scenvi-0.3.4/scenvi/_dists.py` & `scenvi-0.3.5/scenvi/_dists.py`

 * *Files identical despite different names*

### Comparing `scenvi-0.3.4/scenvi/utils.py` & `scenvi-0.3.5/scenvi/utils.py`

 * *Files identical despite different names*

### Comparing `scenvi-0.3.4/PKG-INFO` & `scenvi-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scenvi
-Version: 0.3.4
+Version: 0.3.5
 Summary: Integration of scRNA-seq and spatial transcriptomics data
 License: MIT
 Author: Doron Haviv
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

