# Comparing `tmp/file_crusher-0.2.0.tar.gz` & `tmp/file_crusher-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "file_crusher-0.2.0.tar", last modified: Mon May 20 08:17:41 2024, max compression
+gzip compressed data, was "file_crusher-0.2.1.tar", last modified: Mon May 20 10:46:46 2024, max compression
```

## Comparing `file_crusher-0.2.0.tar` & `file_crusher-0.2.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-20 08:17:41.390332 file_crusher-0.2.0/
--rw-rw-r--   0 user      (1000) user      (1000)     1054 2024-03-16 11:34:40.000000 file_crusher-0.2.0/LICENSE.md
--rw-rw-r--   0 user      (1000) user      (1000)       50 2024-03-16 18:15:51.000000 file_crusher-0.2.0/MANIFEST.in
--rw-r--r--   0 user      (1000) user      (1000)     3581 2024-05-20 08:17:41.390332 file_crusher-0.2.0/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     2695 2024-05-20 08:16:56.000000 file_crusher-0.2.0/README.md
--rw-rw-r--   0 user      (1000) user      (1000)       98 2024-03-16 12:15:12.000000 file_crusher-0.2.0/pyproject.toml
--rw-rw-r--   0 user      (1000) user      (1000)     1003 2024-05-20 08:17:41.390332 file_crusher-0.2.0/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)       37 2024-03-16 12:24:32.000000 file_crusher-0.2.0/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-20 08:17:41.382332 file_crusher-0.2.0/src/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-20 08:17:41.386332 file_crusher-0.2.0/src/file_crusher/
--rw-rw-r--   0 user      (1000) user      (1000)      329 2024-05-20 06:06:40.000000 file_crusher-0.2.0/src/file_crusher/CompressionPostprocessor.py
--rw-rw-r--   0 user      (1000) user      (1000)      639 2024-05-20 07:16:41.000000 file_crusher-0.2.0/src/file_crusher/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1922 2024-05-20 07:23:55.000000 file_crusher-0.2.0/src/file_crusher/__main__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3408 2024-05-20 05:45:05.000000 file_crusher-0.2.0/src/file_crusher/advpng_compressor.py
--rw-rw-r--   0 user      (1000) user      (1000)      515 2024-03-16 17:30:20.000000 file_crusher-0.2.0/src/file_crusher/batch_processor.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-20 08:17:41.382332 file_crusher-0.2.0/src/file_crusher/compressor_lib/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-20 08:17:41.386332 file_crusher-0.2.0/src/file_crusher/compressor_lib/advpng/
--rw-rw-r--   0 user      (1000) user      (1000)    35147 2023-09-05 14:50:18.000000 file_crusher-0.2.0/src/file_crusher/compressor_lib/advpng/LICENCE.txt
--rw-rw-r--   0 user      (1000) user      (1000)   942592 2023-09-05 14:50:18.000000 file_crusher-0.2.0/src/file_crusher/compressor_lib/advpng/advpng.exe
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-20 08:17:41.386332 file_crusher-0.2.0/src/file_crusher/compressor_lib/cpdfsqueeze/
--rw-rw-r--   0 user      (1000) user      (1000)    26726 2023-09-05 14:50:18.000000 file_crusher-0.2.0/src/file_crusher/compressor_lib/cpdfsqueeze/LICENCE.txt
--rw-rw-r--   0 user      (1000) user      (1000)  3735784 2023-09-05 14:50:18.000000 file_crusher-0.2.0/src/file_crusher/compressor_lib/cpdfsqueeze/cpdfsqueeze.exe
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-20 08:17:41.386332 file_crusher-0.2.0/src/file_crusher/compressor_lib/pngcrush/
--rw-rw-r--   0 user      (1000) user      (1000)     3207 2023-09-05 14:50:18.000000 file_crusher-0.2.0/src/file_crusher/compressor_lib/pngcrush/LICENCE.txt
--rw-rw-r--   0 user      (1000) user      (1000)   447488 2023-09-05 14:50:18.000000 file_crusher-0.2.0/src/file_crusher/compressor_lib/pngcrush/pngcrush.exe
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-20 08:17:41.390332 file_crusher-0.2.0/src/file_crusher/compressor_lib/pngquant/
--rw-rw-r--   0 user      (1000) user      (1000)    35621 2023-09-05 14:50:18.000000 file_crusher-0.2.0/src/file_crusher/compressor_lib/pngquant/LICENCE.txt
--rw-rw-r--   0 user      (1000) user      (1000)   743424 2023-09-05 14:50:18.000000 file_crusher-0.2.0/src/file_crusher/compressor_lib/pngquant/pngquant.exe
--rw-rw-r--   0 user      (1000) user      (1000)     2356 2024-02-29 13:58:38.000000 file_crusher-0.2.0/src/file_crusher/config.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-20 08:17:41.390332 file_crusher-0.2.0/src/file_crusher/converter/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2024-02-28 12:16:17.000000 file_crusher-0.2.0/src/file_crusher/converter/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3774 2024-03-16 17:32:01.000000 file_crusher-0.2.0/src/file_crusher/converter/image_to_pdf_converter.py
--rw-rw-r--   0 user      (1000) user      (1000)      487 2024-02-29 18:27:44.000000 file_crusher-0.2.0/src/file_crusher/converter/pdf_merger.py
--rw-rw-r--   0 user      (1000) user      (1000)     2322 2024-03-16 17:32:13.000000 file_crusher-0.2.0/src/file_crusher/converter/pdf_to_image_converter.py
--rw-rw-r--   0 user      (1000) user      (1000)     2202 2024-05-20 07:50:33.000000 file_crusher-0.2.0/src/file_crusher/cpdfsqueeze_compressor.py
--rw-rw-r--   0 user      (1000) user      (1000)     2291 2024-05-20 06:14:13.000000 file_crusher-0.2.0/src/file_crusher/file_operations.py
--rw-rw-r--   0 user      (1000) user      (1000)     4667 2024-05-20 07:56:35.000000 file_crusher-0.2.0/src/file_crusher/pdf_compressor.py
--rw-rw-r--   0 user      (1000) user      (1000)     2224 2024-05-20 06:57:58.000000 file_crusher-0.2.0/src/file_crusher/pipeline_processor.py
--rw-rw-r--   0 user      (1000) user      (1000)     4246 2024-05-20 07:50:57.000000 file_crusher-0.2.0/src/file_crusher/png_compressor.py
--rw-rw-r--   0 user      (1000) user      (1000)     1891 2024-05-20 07:50:41.000000 file_crusher-0.2.0/src/file_crusher/pngcrush_compressor.py
--rw-rw-r--   0 user      (1000) user      (1000)     2894 2024-05-20 07:50:44.000000 file_crusher-0.2.0/src/file_crusher/pngquant_compressor.py
--rw-rw-r--   0 user      (1000) user      (1000)      637 2024-05-20 07:33:54.000000 file_crusher-0.2.0/src/file_crusher/processor.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-20 08:17:41.390332 file_crusher-0.2.0/src/file_crusher.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     3581 2024-05-20 08:17:41.000000 file_crusher-0.2.0/src/file_crusher.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1507 2024-05-20 08:17:41.000000 file_crusher-0.2.0/src/file_crusher.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-05-20 08:17:41.000000 file_crusher-0.2.0/src/file_crusher.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       65 2024-05-20 08:17:41.000000 file_crusher-0.2.0/src/file_crusher.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       13 2024-05-20 08:17:41.000000 file_crusher-0.2.0/src/file_crusher.egg-info/top_level.txt
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-20 08:17:41.390332 file_crusher-0.2.0/tests/
--rw-rw-r--   0 user      (1000) user      (1000)     1093 2024-03-17 17:08:42.000000 file_crusher-0.2.0/tests/test_batch_processing.py
--rw-rw-r--   0 user      (1000) user      (1000)     9044 2024-05-20 03:40:56.000000 file_crusher-0.2.0/tests/test_cpdf_compressor.py
--rw-rw-r--   0 user      (1000) user      (1000)     4202 2024-05-20 05:27:31.000000 file_crusher-0.2.0/tests/test_pipeline_processor.py
--rw-rw-r--   0 user      (1000) user      (1000)     1473 2024-05-20 05:51:01.000000 file_crusher-0.2.0/tests/test_png_compressor.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-20 10:46:46.797987 file_crusher-0.2.1/
+-rw-rw-r--   0 user      (1000) user      (1000)     1054 2024-03-16 11:34:40.000000 file_crusher-0.2.1/LICENSE.md
+-rw-rw-r--   0 user      (1000) user      (1000)       50 2024-03-16 18:15:51.000000 file_crusher-0.2.1/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)     3581 2024-05-20 10:46:46.797987 file_crusher-0.2.1/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     2695 2024-05-20 10:46:08.000000 file_crusher-0.2.1/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)       98 2024-03-16 12:15:12.000000 file_crusher-0.2.1/pyproject.toml
+-rw-rw-r--   0 user      (1000) user      (1000)     1003 2024-05-20 10:46:46.797987 file_crusher-0.2.1/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)       37 2024-03-16 12:24:32.000000 file_crusher-0.2.1/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-20 10:46:46.785987 file_crusher-0.2.1/src/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-20 10:46:46.789987 file_crusher-0.2.1/src/file_crusher/
+-rw-rw-r--   0 user      (1000) user      (1000)      329 2024-05-20 06:06:40.000000 file_crusher-0.2.1/src/file_crusher/CompressionPostprocessor.py
+-rw-rw-r--   0 user      (1000) user      (1000)      639 2024-05-20 07:16:41.000000 file_crusher-0.2.1/src/file_crusher/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1922 2024-05-20 07:23:55.000000 file_crusher-0.2.1/src/file_crusher/__main__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3408 2024-05-20 05:45:05.000000 file_crusher-0.2.1/src/file_crusher/advpng_compressor.py
+-rw-rw-r--   0 user      (1000) user      (1000)      515 2024-03-16 17:30:20.000000 file_crusher-0.2.1/src/file_crusher/batch_processor.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-20 10:46:46.785987 file_crusher-0.2.1/src/file_crusher/compressor_lib/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-20 10:46:46.789987 file_crusher-0.2.1/src/file_crusher/compressor_lib/advpng/
+-rw-rw-r--   0 user      (1000) user      (1000)    35147 2023-09-05 14:50:18.000000 file_crusher-0.2.1/src/file_crusher/compressor_lib/advpng/LICENCE.txt
+-rw-rw-r--   0 user      (1000) user      (1000)   942592 2023-09-05 14:50:18.000000 file_crusher-0.2.1/src/file_crusher/compressor_lib/advpng/advpng.exe
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-20 10:46:46.789987 file_crusher-0.2.1/src/file_crusher/compressor_lib/cpdfsqueeze/
+-rw-rw-r--   0 user      (1000) user      (1000)    26726 2023-09-05 14:50:18.000000 file_crusher-0.2.1/src/file_crusher/compressor_lib/cpdfsqueeze/LICENCE.txt
+-rw-rw-r--   0 user      (1000) user      (1000)  3735784 2023-09-05 14:50:18.000000 file_crusher-0.2.1/src/file_crusher/compressor_lib/cpdfsqueeze/cpdfsqueeze.exe
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-20 10:46:46.793987 file_crusher-0.2.1/src/file_crusher/compressor_lib/pngcrush/
+-rw-rw-r--   0 user      (1000) user      (1000)     3207 2023-09-05 14:50:18.000000 file_crusher-0.2.1/src/file_crusher/compressor_lib/pngcrush/LICENCE.txt
+-rw-rw-r--   0 user      (1000) user      (1000)   447488 2023-09-05 14:50:18.000000 file_crusher-0.2.1/src/file_crusher/compressor_lib/pngcrush/pngcrush.exe
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-20 10:46:46.797987 file_crusher-0.2.1/src/file_crusher/compressor_lib/pngquant/
+-rw-rw-r--   0 user      (1000) user      (1000)    35621 2023-09-05 14:50:18.000000 file_crusher-0.2.1/src/file_crusher/compressor_lib/pngquant/LICENCE.txt
+-rw-rw-r--   0 user      (1000) user      (1000)   743424 2023-09-05 14:50:18.000000 file_crusher-0.2.1/src/file_crusher/compressor_lib/pngquant/pngquant.exe
+-rw-rw-r--   0 user      (1000) user      (1000)     2356 2024-02-29 13:58:38.000000 file_crusher-0.2.1/src/file_crusher/config.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-20 10:46:46.797987 file_crusher-0.2.1/src/file_crusher/converter/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2024-02-28 12:16:17.000000 file_crusher-0.2.1/src/file_crusher/converter/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3774 2024-03-16 17:32:01.000000 file_crusher-0.2.1/src/file_crusher/converter/image_to_pdf_converter.py
+-rw-rw-r--   0 user      (1000) user      (1000)      487 2024-02-29 18:27:44.000000 file_crusher-0.2.1/src/file_crusher/converter/pdf_merger.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2322 2024-03-16 17:32:13.000000 file_crusher-0.2.1/src/file_crusher/converter/pdf_to_image_converter.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2202 2024-05-20 07:50:33.000000 file_crusher-0.2.1/src/file_crusher/cpdfsqueeze_compressor.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2291 2024-05-20 06:14:13.000000 file_crusher-0.2.1/src/file_crusher/file_operations.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4667 2024-05-20 07:56:35.000000 file_crusher-0.2.1/src/file_crusher/pdf_compressor.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2224 2024-05-20 06:57:58.000000 file_crusher-0.2.1/src/file_crusher/pipeline_processor.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4246 2024-05-20 07:50:57.000000 file_crusher-0.2.1/src/file_crusher/png_compressor.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1891 2024-05-20 07:50:41.000000 file_crusher-0.2.1/src/file_crusher/pngcrush_compressor.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2894 2024-05-20 07:50:44.000000 file_crusher-0.2.1/src/file_crusher/pngquant_compressor.py
+-rw-rw-r--   0 user      (1000) user      (1000)      637 2024-05-20 07:33:54.000000 file_crusher-0.2.1/src/file_crusher/processor.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-20 10:46:46.797987 file_crusher-0.2.1/src/file_crusher.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     3581 2024-05-20 10:46:46.000000 file_crusher-0.2.1/src/file_crusher.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1507 2024-05-20 10:46:46.000000 file_crusher-0.2.1/src/file_crusher.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-05-20 10:46:46.000000 file_crusher-0.2.1/src/file_crusher.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       65 2024-05-20 10:46:46.000000 file_crusher-0.2.1/src/file_crusher.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       13 2024-05-20 10:46:46.000000 file_crusher-0.2.1/src/file_crusher.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-20 10:46:46.797987 file_crusher-0.2.1/tests/
+-rw-rw-r--   0 user      (1000) user      (1000)     1093 2024-03-17 17:08:42.000000 file_crusher-0.2.1/tests/test_batch_processing.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9044 2024-05-20 03:40:56.000000 file_crusher-0.2.1/tests/test_cpdf_compressor.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4202 2024-05-20 05:27:31.000000 file_crusher-0.2.1/tests/test_pipeline_processor.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1473 2024-05-20 05:51:01.000000 file_crusher-0.2.1/tests/test_png_compressor.py
```

### Comparing `file_crusher-0.2.0/LICENSE.md` & `file_crusher-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `file_crusher-0.2.0/PKG-INFO` & `file_crusher-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: file-crusher
-Version: 0.2.0
+Version: 0.2.1
 Summary: Compresses PDFs with PNG compression.
 Home-page: https://github.com/pilip-d/FileCrusher.git
 Author: Philip Dell
 Project-URL: Bug Reports, https://github.com/pIlIp-d/FileCrusher/issues
 Project-URL: Source, https://github.com/pilip-d/FileCrusher.git
 Keywords: compression pdf png GoodNotes file crusher crunch compress size limit
 Classifier: Development Status :: 4 - Beta
@@ -75,19 +75,19 @@
 ```
 
 ## Usage
 
 ### CLI Usage
 ```bash
 # for pdfs
-python3 -m file-crusher input.pdf output.pdf --pdfcompressor
+python3 -m file_crusher input.pdf output.pdf --pdfcompressor
 # or for pngs
-python3 -m file-crusher input.png output.png --pngcompressor
+python3 -m file_crusher input.png output.png --pngcompressor
 # for other processors see
-python3 -m file-crusher --help
+python3 -m file_crusher --help
 ```
 
 ### Python Usage
 ```python3
 from file_crusher import PNGCompressor, PDFCompressor
 
 compressor = PNGCompressor()
```

### Comparing `file_crusher-0.2.0/README.md` & `file_crusher-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -52,19 +52,19 @@
 ```
 
 ## Usage
 
 ### CLI Usage
 ```bash
 # for pdfs
-python3 -m file-crusher input.pdf output.pdf --pdfcompressor
+python3 -m file_crusher input.pdf output.pdf --pdfcompressor
 # or for pngs
-python3 -m file-crusher input.png output.png --pngcompressor
+python3 -m file_crusher input.png output.png --pngcompressor
 # for other processors see
-python3 -m file-crusher --help
+python3 -m file_crusher --help
 ```
 
 ### Python Usage
 ```python3
 from file_crusher import PNGCompressor, PDFCompressor
 
 compressor = PNGCompressor()
```

### Comparing `file_crusher-0.2.0/setup.cfg` & `file_crusher-0.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = file-crusher
-version = 0.2.0
+version = 0.2.1
 description = Compresses PDFs with PNG compression.
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8
 license_file = file: LICENSE.md
 author = Philip Dell
 url = https://github.com/pilip-d/FileCrusher.git
 project_urls =
```

### Comparing `file_crusher-0.2.0/src/file_crusher/__init__.py` & `file_crusher-0.2.1/src/file_crusher/__init__.py`

 * *Files identical despite different names*

### Comparing `file_crusher-0.2.0/src/file_crusher/__main__.py` & `file_crusher-0.2.1/src/file_crusher/__main__.py`

 * *Files identical despite different names*

### Comparing `file_crusher-0.2.0/src/file_crusher/advpng_compressor.py` & `file_crusher-0.2.1/src/file_crusher/advpng_compressor.py`

 * *Files identical despite different names*

### Comparing `file_crusher-0.2.0/src/file_crusher/batch_processor.py` & `file_crusher-0.2.1/src/file_crusher/batch_processor.py`

 * *Files identical despite different names*

### Comparing `file_crusher-0.2.0/src/file_crusher/compressor_lib/advpng/LICENCE.txt` & `file_crusher-0.2.1/src/file_crusher/compressor_lib/advpng/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `file_crusher-0.2.0/src/file_crusher/compressor_lib/advpng/advpng.exe` & `file_crusher-0.2.1/src/file_crusher/compressor_lib/advpng/advpng.exe`

 * *Files identical despite different names*

### Comparing `file_crusher-0.2.0/src/file_crusher/compressor_lib/cpdfsqueeze/LICENCE.txt` & `file_crusher-0.2.1/src/file_crusher/compressor_lib/cpdfsqueeze/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `file_crusher-0.2.0/src/file_crusher/compressor_lib/cpdfsqueeze/cpdfsqueeze.exe` & `file_crusher-0.2.1/src/file_crusher/compressor_lib/cpdfsqueeze/cpdfsqueeze.exe`

 * *Files identical despite different names*

### Comparing `file_crusher-0.2.0/src/file_crusher/compressor_lib/pngcrush/LICENCE.txt` & `file_crusher-0.2.1/src/file_crusher/compressor_lib/pngcrush/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `file_crusher-0.2.0/src/file_crusher/compressor_lib/pngcrush/pngcrush.exe` & `file_crusher-0.2.1/src/file_crusher/compressor_lib/pngcrush/pngcrush.exe`

 * *Files identical despite different names*

### Comparing `file_crusher-0.2.0/src/file_crusher/compressor_lib/pngquant/LICENCE.txt` & `file_crusher-0.2.1/src/file_crusher/compressor_lib/pngquant/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `file_crusher-0.2.0/src/file_crusher/compressor_lib/pngquant/pngquant.exe` & `file_crusher-0.2.1/src/file_crusher/compressor_lib/pngquant/pngquant.exe`

 * *Files identical despite different names*

### Comparing `file_crusher-0.2.0/src/file_crusher/config.py` & `file_crusher-0.2.1/src/file_crusher/config.py`

 * *Files identical despite different names*

### Comparing `file_crusher-0.2.0/src/file_crusher/converter/image_to_pdf_converter.py` & `file_crusher-0.2.1/src/file_crusher/converter/image_to_pdf_converter.py`

 * *Files identical despite different names*

### Comparing `file_crusher-0.2.0/src/file_crusher/converter/pdf_to_image_converter.py` & `file_crusher-0.2.1/src/file_crusher/converter/pdf_to_image_converter.py`

 * *Files identical despite different names*

### Comparing `file_crusher-0.2.0/src/file_crusher/cpdfsqueeze_compressor.py` & `file_crusher-0.2.1/src/file_crusher/cpdfsqueeze_compressor.py`

 * *Files identical despite different names*

### Comparing `file_crusher-0.2.0/src/file_crusher/file_operations.py` & `file_crusher-0.2.1/src/file_crusher/file_operations.py`

 * *Files identical despite different names*

### Comparing `file_crusher-0.2.0/src/file_crusher/pdf_compressor.py` & `file_crusher-0.2.1/src/file_crusher/pdf_compressor.py`

 * *Files identical despite different names*

### Comparing `file_crusher-0.2.0/src/file_crusher/pipeline_processor.py` & `file_crusher-0.2.1/src/file_crusher/pipeline_processor.py`

 * *Files identical despite different names*

### Comparing `file_crusher-0.2.0/src/file_crusher/png_compressor.py` & `file_crusher-0.2.1/src/file_crusher/png_compressor.py`

 * *Files identical despite different names*

### Comparing `file_crusher-0.2.0/src/file_crusher/pngcrush_compressor.py` & `file_crusher-0.2.1/src/file_crusher/pngcrush_compressor.py`

 * *Files identical despite different names*

### Comparing `file_crusher-0.2.0/src/file_crusher/pngquant_compressor.py` & `file_crusher-0.2.1/src/file_crusher/pngquant_compressor.py`

 * *Files identical despite different names*

### Comparing `file_crusher-0.2.0/src/file_crusher/processor.py` & `file_crusher-0.2.1/src/file_crusher/processor.py`

 * *Files identical despite different names*

### Comparing `file_crusher-0.2.0/src/file_crusher.egg-info/PKG-INFO` & `file_crusher-0.2.1/src/file_crusher.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: file-crusher
-Version: 0.2.0
+Version: 0.2.1
 Summary: Compresses PDFs with PNG compression.
 Home-page: https://github.com/pilip-d/FileCrusher.git
 Author: Philip Dell
 Project-URL: Bug Reports, https://github.com/pIlIp-d/FileCrusher/issues
 Project-URL: Source, https://github.com/pilip-d/FileCrusher.git
 Keywords: compression pdf png GoodNotes file crusher crunch compress size limit
 Classifier: Development Status :: 4 - Beta
@@ -75,19 +75,19 @@
 ```
 
 ## Usage
 
 ### CLI Usage
 ```bash
 # for pdfs
-python3 -m file-crusher input.pdf output.pdf --pdfcompressor
+python3 -m file_crusher input.pdf output.pdf --pdfcompressor
 # or for pngs
-python3 -m file-crusher input.png output.png --pngcompressor
+python3 -m file_crusher input.png output.png --pngcompressor
 # for other processors see
-python3 -m file-crusher --help
+python3 -m file_crusher --help
 ```
 
 ### Python Usage
 ```python3
 from file_crusher import PNGCompressor, PDFCompressor
 
 compressor = PNGCompressor()
```

### Comparing `file_crusher-0.2.0/src/file_crusher.egg-info/SOURCES.txt` & `file_crusher-0.2.1/src/file_crusher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `file_crusher-0.2.0/tests/test_batch_processing.py` & `file_crusher-0.2.1/tests/test_batch_processing.py`

 * *Files identical despite different names*

### Comparing `file_crusher-0.2.0/tests/test_cpdf_compressor.py` & `file_crusher-0.2.1/tests/test_cpdf_compressor.py`

 * *Files identical despite different names*

### Comparing `file_crusher-0.2.0/tests/test_pipeline_processor.py` & `file_crusher-0.2.1/tests/test_pipeline_processor.py`

 * *Files identical despite different names*

### Comparing `file_crusher-0.2.0/tests/test_png_compressor.py` & `file_crusher-0.2.1/tests/test_png_compressor.py`

 * *Files identical despite different names*

