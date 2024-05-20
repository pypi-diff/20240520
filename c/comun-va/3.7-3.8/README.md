# Comparing `tmp/comun_va-3.7.tar.gz` & `tmp/comun_va-3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comun_va-3.7.tar", last modified: Mon May 20 14:36:48 2024, max compression
+gzip compressed data, was "comun_va-3.8.tar", last modified: Mon May 20 14:56:54 2024, max compression
```

## Comparing `comun_va-3.7.tar` & `comun_va-3.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 14:36:47.990530 comun_va-3.7/
--rw-rw-rw-   0        0        0      141 2024-05-20 14:36:47.989944 comun_va-3.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-20 14:36:47.988699 comun_va-3.7/comun_va.egg-info/
--rw-rw-rw-   0        0        0      141 2024-05-20 14:36:47.000000 comun_va-3.7/comun_va.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      179 2024-05-20 14:36:47.000000 comun_va-3.7/comun_va.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 14:36:47.000000 comun_va-3.7/comun_va.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-05-20 14:36:47.000000 comun_va-3.7/comun_va.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-20 14:36:47.000000 comun_va-3.7/comun_va.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     8931 2024-05-20 14:35:45.000000 comun_va-3.7/comun_va.py
--rw-rw-rw-   0        0        0       42 2024-05-20 14:36:47.990530 comun_va-3.7/setup.cfg
--rw-rw-rw-   0        0        0      216 2024-05-20 14:35:45.000000 comun_va-3.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:56:54.589523 comun_va-3.8/
+-rw-rw-rw-   0        0        0      141 2024-05-20 14:56:54.589018 comun_va-3.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-20 14:56:54.587868 comun_va-3.8/comun_va.egg-info/
+-rw-rw-rw-   0        0        0      141 2024-05-20 14:56:54.000000 comun_va-3.8/comun_va.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      179 2024-05-20 14:56:54.000000 comun_va-3.8/comun_va.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 14:56:54.000000 comun_va-3.8/comun_va.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-05-20 14:56:54.000000 comun_va-3.8/comun_va.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-20 14:56:54.000000 comun_va-3.8/comun_va.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8927 2024-05-20 14:56:50.000000 comun_va-3.8/comun_va.py
+-rw-rw-rw-   0        0        0       42 2024-05-20 14:56:54.589523 comun_va-3.8/setup.cfg
+-rw-rw-rw-   0        0        0      216 2024-05-20 14:56:50.000000 comun_va-3.8/setup.py
```

### Comparing `comun_va-3.7/comun_va.py` & `comun_va-3.8/comun_va.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,15 @@
                 for barcode in detected_barcodes:
                     if barcode.data != "":
                         # Convert the byte string to a string
                         decoded_barcode = barcode.data.decode("utf-8")
                         # A set cannot have repeated elements, so we don't need to check if already exist.
                         barcodes.add(decoded_barcode)
 
-            cap.release()
+        cap.release()
         return barcodes
 
     except Exception as e:
         raise Exception(f"Error durante el proceso de lectura de código de barras: {str(e)}")
 
 
 def run_model_with_frame(img_frame, class_names: dict, model, output=False, limit_gpu=False,
```

