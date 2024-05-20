# Comparing `tmp/napari-tomodl-0.1.8.tar.gz` & `tmp/napari-tomodl-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-tomodl-0.1.8.tar", last modified: Tue Sep 26 02:52:22 2023, max compression
+gzip compressed data, was "napari-tomodl-0.1.9.tar", last modified: Tue Sep 26 02:56:56 2023, max compression
```

## Comparing `napari-tomodl-0.1.8.tar` & `napari-tomodl-0.1.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 obanmarcos  (1000) obanmarcos  (1000)        0 2023-09-26 02:52:22.577159 napari-tomodl-0.1.8/
--rw-rw-r--   0 obanmarcos  (1000) obanmarcos  (1000)     1089 2023-09-03 22:16:12.000000 napari-tomodl-0.1.8/LICENSE
--rw-rw-r--   0 obanmarcos  (1000) obanmarcos  (1000)       96 2023-09-03 22:16:12.000000 napari-tomodl-0.1.8/MANIFEST.in
--rw-r--r--   0 obanmarcos  (1000) obanmarcos  (1000)     5969 2023-09-26 02:52:22.577159 napari-tomodl-0.1.8/PKG-INFO
--rw-rw-r--   0 obanmarcos  (1000) obanmarcos  (1000)     4568 2023-09-21 14:31:45.000000 napari-tomodl-0.1.8/README.md
--rw-rw-r--   0 obanmarcos  (1000) obanmarcos  (1000)      178 2023-09-03 22:16:12.000000 napari-tomodl-0.1.8/pyproject.toml
--rw-rw-r--   0 obanmarcos  (1000) obanmarcos  (1000)     1460 2023-09-26 02:52:22.577159 napari-tomodl-0.1.8/setup.cfg
-drwxrwxr-x   0 obanmarcos  (1000) obanmarcos  (1000)        0 2023-09-26 02:52:22.521155 napari-tomodl-0.1.8/src/
-drwxrwxr-x   0 obanmarcos  (1000) obanmarcos  (1000)        0 2023-09-26 02:52:22.549157 napari-tomodl-0.1.8/src/napari_tomodl/
--rw-rw-r--   0 obanmarcos  (1000) obanmarcos  (1000)      275 2023-09-03 22:16:12.000000 napari-tomodl-0.1.8/src/napari_tomodl/__init__.py
--rw-rw-r--   0 obanmarcos  (1000) obanmarcos  (1000)    11437 2023-09-24 13:34:43.000000 napari-tomodl-0.1.8/src/napari_tomodl/_reconstruction_widget.py
-drwxrwxr-x   0 obanmarcos  (1000) obanmarcos  (1000)        0 2023-09-26 02:52:22.557157 napari-tomodl-0.1.8/src/napari_tomodl/_tests/
--rw-rw-r--   0 obanmarcos  (1000) obanmarcos  (1000)        0 2023-09-03 22:16:12.000000 napari-tomodl-0.1.8/src/napari_tomodl/_tests/__init__.py
--rw-rw-r--   0 obanmarcos  (1000) obanmarcos  (1000)      357 2023-09-03 22:16:12.000000 napari-tomodl-0.1.8/src/napari_tomodl/napari.yaml
-drwxrwxr-x   0 obanmarcos  (1000) obanmarcos  (1000)        0 2023-09-26 02:52:22.573158 napari-tomodl-0.1.8/src/napari_tomodl/processors/
--rw-rw-r--   0 obanmarcos  (1000) obanmarcos  (1000)    11914 2023-09-26 02:37:22.000000 napari-tomodl-0.1.8/src/napari_tomodl/processors/OPTProcessor.py
--rw-rw-r--   0 obanmarcos  (1000) obanmarcos  (1000)        0 2023-09-03 22:16:12.000000 napari-tomodl-0.1.8/src/napari_tomodl/processors/__init__.py
--rw-rw-r--   0 obanmarcos  (1000) obanmarcos  (1000)    21696 2023-09-03 22:59:31.000000 napari-tomodl-0.1.8/src/napari_tomodl/processors/alternating.py
--rw-rw-r--   0 obanmarcos  (1000) obanmarcos  (1000)    12878 2023-09-26 02:50:25.000000 napari-tomodl-0.1.8/src/napari_tomodl/processors/modl.py
--rw-rw-r--   0 obanmarcos  (1000) obanmarcos  (1000)     5099 2023-09-26 02:31:42.000000 napari-tomodl-0.1.8/src/napari_tomodl/processors/unet.py
--rw-rw-r--   0 obanmarcos  (1000) obanmarcos  (1000)     8523 2023-09-03 22:16:12.000000 napari-tomodl-0.1.8/src/napari_tomodl/widget_settings.py
-drwxrwxr-x   0 obanmarcos  (1000) obanmarcos  (1000)        0 2023-09-26 02:52:22.573158 napari-tomodl-0.1.8/src/napari_tomodl/workshop/
--rw-rw-r--   0 obanmarcos  (1000) obanmarcos  (1000)      117 2023-09-04 16:34:28.000000 napari-tomodl-0.1.8/src/napari_tomodl/workshop/segmentation.py
-drwxrwxr-x   0 obanmarcos  (1000) obanmarcos  (1000)        0 2023-09-26 02:52:22.553157 napari-tomodl-0.1.8/src/napari_tomodl.egg-info/
--rw-r--r--   0 obanmarcos  (1000) obanmarcos  (1000)     5969 2023-09-26 02:52:22.000000 napari-tomodl-0.1.8/src/napari_tomodl.egg-info/PKG-INFO
--rw-rw-r--   0 obanmarcos  (1000) obanmarcos  (1000)      727 2023-09-26 02:52:22.000000 napari-tomodl-0.1.8/src/napari_tomodl.egg-info/SOURCES.txt
--rw-rw-r--   0 obanmarcos  (1000) obanmarcos  (1000)        1 2023-09-26 02:52:22.000000 napari-tomodl-0.1.8/src/napari_tomodl.egg-info/dependency_links.txt
--rw-rw-r--   0 obanmarcos  (1000) obanmarcos  (1000)       60 2023-09-26 02:52:22.000000 napari-tomodl-0.1.8/src/napari_tomodl.egg-info/entry_points.txt
--rw-rw-r--   0 obanmarcos  (1000) obanmarcos  (1000)      129 2023-09-26 02:52:22.000000 napari-tomodl-0.1.8/src/napari_tomodl.egg-info/requires.txt
--rw-rw-r--   0 obanmarcos  (1000) obanmarcos  (1000)       14 2023-09-26 02:52:22.000000 napari-tomodl-0.1.8/src/napari_tomodl.egg-info/top_level.txt
+drwxrwxr-x   0 obanmarcos  (1000) obanmarcos  (1000)        0 2023-09-26 02:56:56.955773 napari-tomodl-0.1.9/
+-rw-rw-r--   0 obanmarcos  (1000) obanmarcos  (1000)     1089 2023-09-03 22:16:12.000000 napari-tomodl-0.1.9/LICENSE
+-rw-rw-r--   0 obanmarcos  (1000) obanmarcos  (1000)       96 2023-09-03 22:16:12.000000 napari-tomodl-0.1.9/MANIFEST.in
+-rw-r--r--   0 obanmarcos  (1000) obanmarcos  (1000)     5967 2023-09-26 02:56:56.951773 napari-tomodl-0.1.9/PKG-INFO
+-rw-rw-r--   0 obanmarcos  (1000) obanmarcos  (1000)     4568 2023-09-21 14:31:45.000000 napari-tomodl-0.1.9/README.md
+-rw-rw-r--   0 obanmarcos  (1000) obanmarcos  (1000)      178 2023-09-03 22:16:12.000000 napari-tomodl-0.1.9/pyproject.toml
+-rw-r--r--   0 obanmarcos  (1000) obanmarcos  (1000)     1458 2023-09-26 02:56:56.959773 napari-tomodl-0.1.9/setup.cfg
+drwxrwxr-x   0 obanmarcos  (1000) obanmarcos  (1000)        0 2023-09-26 02:56:56.887770 napari-tomodl-0.1.9/src/
+drwxrwxr-x   0 obanmarcos  (1000) obanmarcos  (1000)        0 2023-09-26 02:56:56.911771 napari-tomodl-0.1.9/src/napari_tomodl/
+-rw-rw-r--   0 obanmarcos  (1000) obanmarcos  (1000)      275 2023-09-03 22:16:12.000000 napari-tomodl-0.1.9/src/napari_tomodl/__init__.py
+-rw-rw-r--   0 obanmarcos  (1000) obanmarcos  (1000)    11437 2023-09-24 13:34:43.000000 napari-tomodl-0.1.9/src/napari_tomodl/_reconstruction_widget.py
+drwxrwxr-x   0 obanmarcos  (1000) obanmarcos  (1000)        0 2023-09-26 02:56:56.927772 napari-tomodl-0.1.9/src/napari_tomodl/_tests/
+-rw-rw-r--   0 obanmarcos  (1000) obanmarcos  (1000)        0 2023-09-03 22:16:12.000000 napari-tomodl-0.1.9/src/napari_tomodl/_tests/__init__.py
+-rw-rw-r--   0 obanmarcos  (1000) obanmarcos  (1000)      357 2023-09-03 22:16:12.000000 napari-tomodl-0.1.9/src/napari_tomodl/napari.yaml
+drwxrwxr-x   0 obanmarcos  (1000) obanmarcos  (1000)        0 2023-09-26 02:56:56.943773 napari-tomodl-0.1.9/src/napari_tomodl/processors/
+-rw-rw-r--   0 obanmarcos  (1000) obanmarcos  (1000)    11914 2023-09-26 02:37:22.000000 napari-tomodl-0.1.9/src/napari_tomodl/processors/OPTProcessor.py
+-rw-rw-r--   0 obanmarcos  (1000) obanmarcos  (1000)        0 2023-09-03 22:16:12.000000 napari-tomodl-0.1.9/src/napari_tomodl/processors/__init__.py
+-rw-rw-r--   0 obanmarcos  (1000) obanmarcos  (1000)    21696 2023-09-03 22:59:31.000000 napari-tomodl-0.1.9/src/napari_tomodl/processors/alternating.py
+-rw-rw-r--   0 obanmarcos  (1000) obanmarcos  (1000)    12878 2023-09-26 02:50:25.000000 napari-tomodl-0.1.9/src/napari_tomodl/processors/modl.py
+-rw-rw-r--   0 obanmarcos  (1000) obanmarcos  (1000)     5094 2023-09-26 02:56:34.000000 napari-tomodl-0.1.9/src/napari_tomodl/processors/unet.py
+-rw-rw-r--   0 obanmarcos  (1000) obanmarcos  (1000)     8523 2023-09-03 22:16:12.000000 napari-tomodl-0.1.9/src/napari_tomodl/widget_settings.py
+drwxrwxr-x   0 obanmarcos  (1000) obanmarcos  (1000)        0 2023-09-26 02:56:56.947773 napari-tomodl-0.1.9/src/napari_tomodl/workshop/
+-rw-rw-r--   0 obanmarcos  (1000) obanmarcos  (1000)      117 2023-09-04 16:34:28.000000 napari-tomodl-0.1.9/src/napari_tomodl/workshop/segmentation.py
+drwxrwxr-x   0 obanmarcos  (1000) obanmarcos  (1000)        0 2023-09-26 02:56:56.923772 napari-tomodl-0.1.9/src/napari_tomodl.egg-info/
+-rw-r--r--   0 obanmarcos  (1000) obanmarcos  (1000)     5967 2023-09-26 02:56:56.000000 napari-tomodl-0.1.9/src/napari_tomodl.egg-info/PKG-INFO
+-rw-rw-r--   0 obanmarcos  (1000) obanmarcos  (1000)      727 2023-09-26 02:56:56.000000 napari-tomodl-0.1.9/src/napari_tomodl.egg-info/SOURCES.txt
+-rw-rw-r--   0 obanmarcos  (1000) obanmarcos  (1000)        1 2023-09-26 02:56:56.000000 napari-tomodl-0.1.9/src/napari_tomodl.egg-info/dependency_links.txt
+-rw-rw-r--   0 obanmarcos  (1000) obanmarcos  (1000)       60 2023-09-26 02:56:56.000000 napari-tomodl-0.1.9/src/napari_tomodl.egg-info/entry_points.txt
+-rw-rw-r--   0 obanmarcos  (1000) obanmarcos  (1000)      129 2023-09-26 02:56:56.000000 napari-tomodl-0.1.9/src/napari_tomodl.egg-info/requires.txt
+-rw-rw-r--   0 obanmarcos  (1000) obanmarcos  (1000)       14 2023-09-26 02:56:56.000000 napari-tomodl-0.1.9/src/napari_tomodl.egg-info/top_level.txt
```

### Comparing `napari-tomodl-0.1.8/LICENSE` & `napari-tomodl-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-tomodl-0.1.8/PKG-INFO` & `napari-tomodl-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: napari-tomodl
-Version: 0.1.8
+Version: 0.1.9
 Summary: A plugin for optical projection tomography reconstruction with model-based neural networks.
-Author: [Marcos Antonio Obando, Germán Mato, Teresa Correia]
+Author: Marcos Antonio Obando, Germán Mato, Teresa Correia
 Author-email: marcos.obando@ib.edu.ar
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `napari-tomodl-0.1.8/README.md` & `napari-tomodl-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `napari-tomodl-0.1.8/setup.cfg` & `napari-tomodl-0.1.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = napari-tomodl
-version = 0.1.8
+version = 0.1.9
 description = A plugin for optical projection tomography reconstruction with model-based neural networks.
 long_description = file: README.md
 long_description_content_type = text/markdown
-author = [Marcos Antonio Obando, Germán Mato, Teresa Correia]
+author = Marcos Antonio Obando, Germán Mato, Teresa Correia
 author_email = marcos.obando@ib.edu.ar
 license = MIT
 license_files = LICENSE
 classifiers = 
 	Development Status :: 2 - Pre-Alpha
 	Framework :: napari
 	Intended Audience :: Developers
```

### Comparing `napari-tomodl-0.1.8/src/napari_tomodl/_reconstruction_widget.py` & `napari-tomodl-0.1.9/src/napari_tomodl/_reconstruction_widget.py`

 * *Files identical despite different names*

### Comparing `napari-tomodl-0.1.8/src/napari_tomodl/processors/OPTProcessor.py` & `napari-tomodl-0.1.9/src/napari_tomodl/processors/OPTProcessor.py`

 * *Files identical despite different names*

### Comparing `napari-tomodl-0.1.8/src/napari_tomodl/processors/alternating.py` & `napari-tomodl-0.1.9/src/napari_tomodl/processors/alternating.py`

 * *Files identical despite different names*

### Comparing `napari-tomodl-0.1.8/src/napari_tomodl/processors/modl.py` & `napari-tomodl-0.1.9/src/napari_tomodl/processors/modl.py`

 * *Files identical despite different names*

### Comparing `napari-tomodl-0.1.8/src/napari_tomodl/processors/unet.py` & `napari-tomodl-0.1.9/src/napari_tomodl/processors/unet.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 
 try:
     # Modify for multi-gpu
     device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
 
 except:
     print('Torch not available!')
-    
 # U-Net
 
 class double_conv(nn.Module):
     '''(conv => BN => ReLU) * 2'''
     def __init__(self, in_ch, out_ch, batch_norm = False):
         super(double_conv, self).__init__()
```

### Comparing `napari-tomodl-0.1.8/src/napari_tomodl/widget_settings.py` & `napari-tomodl-0.1.9/src/napari_tomodl/widget_settings.py`

 * *Files identical despite different names*

### Comparing `napari-tomodl-0.1.8/src/napari_tomodl.egg-info/PKG-INFO` & `napari-tomodl-0.1.9/src/napari_tomodl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: napari-tomodl
-Version: 0.1.8
+Version: 0.1.9
 Summary: A plugin for optical projection tomography reconstruction with model-based neural networks.
-Author: [Marcos Antonio Obando, Germán Mato, Teresa Correia]
+Author: Marcos Antonio Obando, Germán Mato, Teresa Correia
 Author-email: marcos.obando@ib.edu.ar
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `napari-tomodl-0.1.8/src/napari_tomodl.egg-info/SOURCES.txt` & `napari-tomodl-0.1.9/src/napari_tomodl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

