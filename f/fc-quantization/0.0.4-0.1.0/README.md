# Comparing `tmp/fc-quantization-0.0.4.tar.gz` & `tmp/fc-quantization-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fc-quantization-0.0.4.tar", last modified: Sun May 12 13:18:23 2024, max compression
+gzip compressed data, was "fc-quantization-0.1.0.tar", last modified: Mon May 20 21:17:36 2024, max compression
```

## Comparing `fc-quantization-0.0.4.tar` & `fc-quantization-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-05-12 13:18:23.946808 fc-quantization-0.0.4/
--rw-r--r--   0 aidamehammed   (501) staff       (20)    11352 2024-03-22 14:55:37.000000 fc-quantization-0.0.4/LICENSE
--rw-r--r--   0 aidamehammed   (501) staff       (20)     1920 2024-05-12 13:18:23.946705 fc-quantization-0.0.4/PKG-INFO
--rw-r--r--   0 aidamehammed   (501) staff       (20)     1354 2024-04-19 22:15:39.000000 fc-quantization-0.0.4/README.md
-drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-05-12 13:18:23.945021 fc-quantization-0.0.4/fc_quantization/
-drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-05-12 13:18:23.946409 fc-quantization-0.0.4/fc_quantization/Compress/
--rw-r--r--   0 aidamehammed   (501) staff       (20)       47 2024-05-11 18:45:51.000000 fc-quantization-0.0.4/fc_quantization/Compress/__init__.py
--rw-r--r--   0 aidamehammed   (501) staff       (20)     4870 2024-05-12 13:18:21.000000 fc-quantization-0.0.4/fc_quantization/Compress/compress.py
--rw-r--r--   0 aidamehammed   (501) staff       (20)     2201 2024-05-12 11:42:18.000000 fc-quantization-0.0.4/fc_quantization/Compress/utils.py
--rw-r--r--   0 aidamehammed   (501) staff       (20)        0 2024-05-11 18:43:51.000000 fc-quantization-0.0.4/fc_quantization/__init__.py
-drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-05-12 13:18:23.945683 fc-quantization-0.0.4/fc_quantization.egg-info/
--rw-r--r--   0 aidamehammed   (501) staff       (20)     1920 2024-05-12 13:18:23.000000 fc-quantization-0.0.4/fc_quantization.egg-info/PKG-INFO
--rw-r--r--   0 aidamehammed   (501) staff       (20)      356 2024-05-12 13:18:23.000000 fc-quantization-0.0.4/fc_quantization.egg-info/SOURCES.txt
--rw-r--r--   0 aidamehammed   (501) staff       (20)        1 2024-05-12 13:18:23.000000 fc-quantization-0.0.4/fc_quantization.egg-info/dependency_links.txt
--rw-r--r--   0 aidamehammed   (501) staff       (20)       19 2024-05-12 13:18:23.000000 fc-quantization-0.0.4/fc_quantization.egg-info/requires.txt
--rw-r--r--   0 aidamehammed   (501) staff       (20)       16 2024-05-12 13:18:23.000000 fc-quantization-0.0.4/fc_quantization.egg-info/top_level.txt
--rw-r--r--   0 aidamehammed   (501) staff       (20)       38 2024-05-12 13:18:23.946921 fc-quantization-0.0.4/setup.cfg
--rw-r--r--   0 aidamehammed   (501) staff       (20)     1230 2024-05-12 13:18:21.000000 fc-quantization-0.0.4/setup.py
+drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-05-20 21:17:36.484140 fc-quantization-0.1.0/
+-rw-r--r--   0 aidamehammed   (501) staff       (20)    11352 2024-03-22 14:55:37.000000 fc-quantization-0.1.0/LICENSE
+-rw-r--r--   0 aidamehammed   (501) staff       (20)     1843 2024-05-20 21:17:36.484038 fc-quantization-0.1.0/PKG-INFO
+-rw-r--r--   0 aidamehammed   (501) staff       (20)     1277 2024-05-20 19:59:37.000000 fc-quantization-0.1.0/README.md
+drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-05-20 21:17:36.482498 fc-quantization-0.1.0/fc_quantization/
+drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-05-20 21:17:36.483736 fc-quantization-0.1.0/fc_quantization/Compress/
+-rw-r--r--   0 aidamehammed   (501) staff       (20)       47 2024-05-11 18:45:51.000000 fc-quantization-0.1.0/fc_quantization/Compress/__init__.py
+-rw-r--r--   0 aidamehammed   (501) staff       (20)     4746 2024-05-20 18:22:06.000000 fc-quantization-0.1.0/fc_quantization/Compress/compress.py
+-rw-r--r--   0 aidamehammed   (501) staff       (20)     2196 2024-05-20 18:22:34.000000 fc-quantization-0.1.0/fc_quantization/Compress/utils.py
+-rw-r--r--   0 aidamehammed   (501) staff       (20)        0 2024-05-11 18:43:51.000000 fc-quantization-0.1.0/fc_quantization/__init__.py
+drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-05-20 21:17:36.483083 fc-quantization-0.1.0/fc_quantization.egg-info/
+-rw-r--r--   0 aidamehammed   (501) staff       (20)     1843 2024-05-20 21:17:36.000000 fc-quantization-0.1.0/fc_quantization.egg-info/PKG-INFO
+-rw-r--r--   0 aidamehammed   (501) staff       (20)      356 2024-05-20 21:17:36.000000 fc-quantization-0.1.0/fc_quantization.egg-info/SOURCES.txt
+-rw-r--r--   0 aidamehammed   (501) staff       (20)        1 2024-05-20 21:17:36.000000 fc-quantization-0.1.0/fc_quantization.egg-info/dependency_links.txt
+-rw-r--r--   0 aidamehammed   (501) staff       (20)       19 2024-05-20 21:17:36.000000 fc-quantization-0.1.0/fc_quantization.egg-info/requires.txt
+-rw-r--r--   0 aidamehammed   (501) staff       (20)       16 2024-05-20 21:17:36.000000 fc-quantization-0.1.0/fc_quantization.egg-info/top_level.txt
+-rw-r--r--   0 aidamehammed   (501) staff       (20)       38 2024-05-20 21:17:36.484185 fc-quantization-0.1.0/setup.cfg
+-rw-r--r--   0 aidamehammed   (501) staff       (20)     1230 2024-05-20 21:15:57.000000 fc-quantization-0.1.0/setup.py
```

### Comparing `fc-quantization-0.0.4/LICENSE` & `fc-quantization-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fc-quantization-0.0.4/PKG-INFO` & `fc-quantization-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fc-quantization
-Version: 0.0.4
+Version: 0.1.0
 Summary: FC Quantization
 Home-page: https://github.com/AidaMehammed/fc-quantization
 Author: Aida Mehammed
 Author-email: aida.mehammed@studium.uni-hamburg.de
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/AidaMehammed/fc-quantization/issues
 Platform: UNKNOWN
@@ -15,18 +15,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # [FeatureCloud Quantization](https://github.com/AidaMehammed/Quantization_CNN)
 ### Model Compression with Quantization
 
 The FC Quantization package provides a comprehensive solution for model compression through quantization techniques. Integrated with federated learning frameworks and built upon the capabilities of PyTorch's quantization functionalities, this package facilitates efficient distributed training suitable for various machine learning tasks.
-## Install FeatureCloud Quantization
-```shell
-pip install fc-quantization
-```
+
 
 1. Configure Quantization:
     - Set up initial quantization settings.
       ```python
         self.configure_quant(model, backend, quant_typ)
         ```
```

### Comparing `fc-quantization-0.0.4/README.md` & `fc-quantization-0.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 # [FeatureCloud Quantization](https://github.com/AidaMehammed/Quantization_CNN)
 ### Model Compression with Quantization
 
 The FC Quantization package provides a comprehensive solution for model compression through quantization techniques. Integrated with federated learning frameworks and built upon the capabilities of PyTorch's quantization functionalities, this package facilitates efficient distributed training suitable for various machine learning tasks.
-## Install FeatureCloud Quantization
-```shell
-pip install fc-quantization
-```
+
 
 1. Configure Quantization:
     - Set up initial quantization settings.
       ```python
         self.configure_quant(model, backend, quant_typ)
         ```
```

### Comparing `fc-quantization-0.0.4/fc_quantization/Compress/compress.py` & `fc-quantization-0.1.0/fc_quantization/Compress/compress.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,16 +67,14 @@
 
         data = super().gather_data(**kwargs)
         if use_quant:
 
             reference_model = self.load('reference_model')
             backend = self.load('backend')
 
-            print(data)
-            self.log(f'Size of model before rebuild: {pf.print_size_of_model(reference_model)} MB')
 
             reconstructed_models = []
             # reconstruct data after quantization
             for i in range(len(data)):
                 print('Reconstrucing Models')
 
                 # recreating client models by first quantizing reference model and loading quantized model after
```

### Comparing `fc-quantization-0.0.4/fc_quantization/Compress/utils.py` & `fc-quantization-0.1.0/fc_quantization/Compress/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,29 +39,28 @@
     with torch.no_grad():
         for data, target in train_loader:
             # temp(data)
             forward_quant(temp, data)
 
     return temp
 
+# essential for training and testing functions
 def forward_quant(model, x):
     # Add quantization stub
     x = model.quant(x)
 
     # Forward pass through the model
     x = model(x)
 
     # Add dequantization stub
     x = model.dequant(x)
 
     return x
 
 
-# works for convd and linear (and pooling layers )
-
 
 def revert_quantized_model(quantized_model, original_model):
 
     reverted_model = nn.Sequential()
 
     # Iterate through the named parameters of the original model
     for name, param in original_model.named_parameters():
```

### Comparing `fc-quantization-0.0.4/fc_quantization.egg-info/PKG-INFO` & `fc-quantization-0.1.0/fc_quantization.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fc-quantization
-Version: 0.0.4
+Version: 0.1.0
 Summary: FC Quantization
 Home-page: https://github.com/AidaMehammed/fc-quantization
 Author: Aida Mehammed
 Author-email: aida.mehammed@studium.uni-hamburg.de
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/AidaMehammed/fc-quantization/issues
 Platform: UNKNOWN
@@ -15,18 +15,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # [FeatureCloud Quantization](https://github.com/AidaMehammed/Quantization_CNN)
 ### Model Compression with Quantization
 
 The FC Quantization package provides a comprehensive solution for model compression through quantization techniques. Integrated with federated learning frameworks and built upon the capabilities of PyTorch's quantization functionalities, this package facilitates efficient distributed training suitable for various machine learning tasks.
-## Install FeatureCloud Quantization
-```shell
-pip install fc-quantization
-```
+
 
 1. Configure Quantization:
     - Set up initial quantization settings.
       ```python
         self.configure_quant(model, backend, quant_typ)
         ```
```

### Comparing `fc-quantization-0.0.4/setup.py` & `fc-quantization-0.1.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(name="fc-quantization",
-                 version="0.0.4",
+                 version="0.1.0",
                  author="Aida Mehammed",
                  author_email="aida.mehammed@studium.uni-hamburg.de",
                  description="FC Quantization",
                  long_description=long_description,
                  long_description_content_type="text/markdown",
                  url="https://github.com/AidaMehammed/fc-quantization",
                  project_urls={
```

