# Comparing `tmp/docrx-0.0.110.tar.gz` & `tmp/docrx-0.0.111.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docrx-0.0.110.tar", last modified: Fri May 17 15:46:55 2024, max compression
+gzip compressed data, was "docrx-0.0.111.tar", last modified: Mon May 20 20:53:17 2024, max compression
```

## Comparing `docrx-0.0.110.tar` & `docrx-0.0.111.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-05-17 15:46:55.839737 docrx-0.0.110/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1072 2023-08-15 18:10:00.000000 docrx-0.0.110/LICENSE.txt
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       46 2022-02-09 16:00:43.000000 docrx-0.0.110/MANIFEST.in
--rw-r--r--   0 tiago     (1000) tiago     (1000)     2421 2024-05-17 15:46:55.839737 docrx-0.0.110/PKG-INFO
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      181 2024-01-25 19:19:24.000000 docrx-0.0.110/README.md
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       42 2024-04-03 16:42:12.000000 docrx-0.0.110/requirements-dev.txt
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      404 2024-05-16 18:22:18.000000 docrx-0.0.110/requirements.txt
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1271 2024-05-17 15:46:55.839737 docrx-0.0.110/setup.cfg
--rwxrwxr-x   0 tiago     (1000) tiago     (1000)     3348 2024-05-17 15:44:47.000000 docrx-0.0.110/setup.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-05-17 15:46:55.819737 docrx-0.0.110/src/
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-05-17 15:46:55.839737 docrx-0.0.110/src/docrx.egg-info/
--rw-r--r--   0 tiago     (1000) tiago     (1000)     2421 2024-05-17 15:46:55.000000 docrx-0.0.110/src/docrx.egg-info/PKG-INFO
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1094 2024-05-17 15:46:55.000000 docrx-0.0.110/src/docrx.egg-info/SOURCES.txt
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        1 2024-05-17 15:46:55.000000 docrx-0.0.110/src/docrx.egg-info/dependency_links.txt
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        1 2024-05-17 15:46:55.000000 docrx-0.0.110/src/docrx.egg-info/not-zip-safe
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      464 2024-05-17 15:46:55.000000 docrx-0.0.110/src/docrx.egg-info/requires.txt
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        8 2024-05-17 15:46:55.000000 docrx-0.0.110/src/docrx.egg-info/top_level.txt
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-05-17 15:46:55.827737 docrx-0.0.110/src/wrapper/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)   491184 2024-05-17 15:46:55.000000 docrx-0.0.110/src/wrapper/Process.c
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-08-15 18:18:13.000000 docrx-0.0.110/src/wrapper/__init__.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-05-17 15:46:55.835737 docrx-0.0.110/src/wrapper/core/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)   308838 2024-04-03 16:41:28.000000 docrx-0.0.110/src/wrapper/core/DocumentSearch.c
--rw-rw-r--   0 tiago     (1000) tiago     (1000)   479564 2024-05-17 15:45:55.000000 docrx-0.0.110/src/wrapper/core/DocumentSearchSB.c
--rw-rw-r--   0 tiago     (1000) tiago     (1000)   530365 2024-05-03 22:12:32.000000 docrx-0.0.110/src/wrapper/core/DocumentSearchTD.c
--rw-rw-r--   0 tiago     (1000) tiago     (1000)   368433 2024-05-17 15:45:55.000000 docrx-0.0.110/src/wrapper/core/File.c
--rw-rw-r--   0 tiago     (1000) tiago     (1000)   279948 2024-05-17 15:45:55.000000 docrx-0.0.110/src/wrapper/core/Image.c
--rw-rw-r--   0 tiago     (1000) tiago     (1000)   278026 2024-05-17 15:45:55.000000 docrx-0.0.110/src/wrapper/core/PDF.c
--rw-rw-r--   0 tiago     (1000) tiago     (1000)   315197 2024-05-17 15:45:55.000000 docrx-0.0.110/src/wrapper/core/SentenceTransformerVectorizer.c
--rw-rw-r--   0 tiago     (1000) tiago     (1000)   293392 2024-05-17 15:45:55.000000 docrx-0.0.110/src/wrapper/core/Vectorizer.c
--rw-rw-r--   0 tiago     (1000) tiago     (1000)   278997 2024-05-17 15:45:56.000000 docrx-0.0.110/src/wrapper/core/Video.c
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-08-15 18:18:13.000000 docrx-0.0.110/src/wrapper/core/__init__.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-05-17 15:46:55.839737 docrx-0.0.110/src/wrapper/infra/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)   249742 2023-08-16 20:21:24.000000 docrx-0.0.110/src/wrapper/infra/AbsctractGenerator.c
--rw-rw-r--   0 tiago     (1000) tiago     (1000)   277587 2024-05-17 15:45:56.000000 docrx-0.0.110/src/wrapper/infra/DocLanguage.c
--rw-rw-r--   0 tiago     (1000) tiago     (1000)   363239 2023-08-16 20:24:23.000000 docrx-0.0.110/src/wrapper/infra/ImageObjectsExtractor.c
--rw-rw-r--   0 tiago     (1000) tiago     (1000)   487999 2024-05-17 15:45:56.000000 docrx-0.0.110/src/wrapper/infra/LanguageDetector.c
--rw-rw-r--   0 tiago     (1000) tiago     (1000)   187001 2024-05-17 15:45:56.000000 docrx-0.0.110/src/wrapper/infra/ModelType.c
--rw-rw-r--   0 tiago     (1000) tiago     (1000)   246255 2024-05-03 22:12:32.000000 docrx-0.0.110/src/wrapper/infra/NERExtractor.c
--rw-rw-r--   0 tiago     (1000) tiago     (1000)   382373 2024-05-17 15:45:56.000000 docrx-0.0.110/src/wrapper/infra/PreProcessing.c
--rw-rw-r--   0 tiago     (1000) tiago     (1000)   476607 2024-05-17 15:45:56.000000 docrx-0.0.110/src/wrapper/infra/TextExtractor.c
--rw-rw-r--   0 tiago     (1000) tiago     (1000)   345115 2023-08-21 16:33:02.000000 docrx-0.0.110/src/wrapper/infra/VideoObjectsExtractor.c
--rw-rw-r--   0 tiago     (1000) tiago     (1000)   278651 2024-05-17 15:45:56.000000 docrx-0.0.110/src/wrapper/infra/WordFixer.c
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-08-15 18:18:13.000000 docrx-0.0.110/src/wrapper/infra/__init__.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-05-17 15:46:55.839737 docrx-0.0.110/src/wrapper/infra/res/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-08-15 18:18:13.000000 docrx-0.0.110/src/wrapper/infra/res/__init__.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-05-17 15:46:55.839737 docrx-0.0.110/tests/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3015 2024-05-16 18:46:42.000000 docrx-0.0.110/tests/test_TestProcessPDFImage.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-05-20 20:53:17.235263 docrx-0.0.111/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1072 2023-08-15 18:10:00.000000 docrx-0.0.111/LICENSE.txt
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       46 2022-02-09 16:00:43.000000 docrx-0.0.111/MANIFEST.in
+-rw-r--r--   0 tiago     (1000) tiago     (1000)     2421 2024-05-20 20:53:17.235263 docrx-0.0.111/PKG-INFO
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      181 2024-01-25 19:19:24.000000 docrx-0.0.111/README.md
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       42 2024-04-03 16:42:12.000000 docrx-0.0.111/requirements-dev.txt
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      404 2024-05-16 18:22:18.000000 docrx-0.0.111/requirements.txt
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1271 2024-05-20 20:53:17.235263 docrx-0.0.111/setup.cfg
+-rwxrwxr-x   0 tiago     (1000) tiago     (1000)     3348 2024-05-17 15:44:47.000000 docrx-0.0.111/setup.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-05-20 20:53:17.147263 docrx-0.0.111/src/
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-05-20 20:53:17.235263 docrx-0.0.111/src/docrx.egg-info/
+-rw-r--r--   0 tiago     (1000) tiago     (1000)     2421 2024-05-20 20:53:16.000000 docrx-0.0.111/src/docrx.egg-info/PKG-INFO
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1094 2024-05-20 20:53:17.000000 docrx-0.0.111/src/docrx.egg-info/SOURCES.txt
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        1 2024-05-20 20:53:16.000000 docrx-0.0.111/src/docrx.egg-info/dependency_links.txt
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        1 2024-05-20 20:53:16.000000 docrx-0.0.111/src/docrx.egg-info/not-zip-safe
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      464 2024-05-20 20:53:16.000000 docrx-0.0.111/src/docrx.egg-info/requires.txt
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        8 2024-05-20 20:53:16.000000 docrx-0.0.111/src/docrx.egg-info/top_level.txt
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-05-20 20:53:17.191263 docrx-0.0.111/src/wrapper/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)   488908 2024-05-20 20:53:16.000000 docrx-0.0.111/src/wrapper/Process.c
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-08-15 18:18:13.000000 docrx-0.0.111/src/wrapper/__init__.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-05-20 20:53:17.203263 docrx-0.0.111/src/wrapper/core/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)   308838 2024-04-03 16:41:28.000000 docrx-0.0.111/src/wrapper/core/DocumentSearch.c
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)   479564 2024-05-17 15:45:55.000000 docrx-0.0.111/src/wrapper/core/DocumentSearchSB.c
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)   530365 2024-05-03 22:12:32.000000 docrx-0.0.111/src/wrapper/core/DocumentSearchTD.c
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)   368433 2024-05-17 15:45:55.000000 docrx-0.0.111/src/wrapper/core/File.c
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)   279948 2024-05-17 15:45:55.000000 docrx-0.0.111/src/wrapper/core/Image.c
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)   278026 2024-05-17 15:45:55.000000 docrx-0.0.111/src/wrapper/core/PDF.c
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)   315900 2024-05-20 20:53:16.000000 docrx-0.0.111/src/wrapper/core/SentenceTransformerVectorizer.c
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)   293392 2024-05-17 15:45:55.000000 docrx-0.0.111/src/wrapper/core/Vectorizer.c
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)   278997 2024-05-17 15:45:56.000000 docrx-0.0.111/src/wrapper/core/Video.c
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-08-15 18:18:13.000000 docrx-0.0.111/src/wrapper/core/__init__.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-05-20 20:53:17.219263 docrx-0.0.111/src/wrapper/infra/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)   249742 2023-08-16 20:21:24.000000 docrx-0.0.111/src/wrapper/infra/AbsctractGenerator.c
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)   277587 2024-05-17 15:45:56.000000 docrx-0.0.111/src/wrapper/infra/DocLanguage.c
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)   363239 2023-08-16 20:24:23.000000 docrx-0.0.111/src/wrapper/infra/ImageObjectsExtractor.c
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)   487999 2024-05-17 15:45:56.000000 docrx-0.0.111/src/wrapper/infra/LanguageDetector.c
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)   187001 2024-05-17 15:45:56.000000 docrx-0.0.111/src/wrapper/infra/ModelType.c
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)   246255 2024-05-03 22:12:32.000000 docrx-0.0.111/src/wrapper/infra/NERExtractor.c
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)   382373 2024-05-17 15:45:56.000000 docrx-0.0.111/src/wrapper/infra/PreProcessing.c
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)   476607 2024-05-17 15:45:56.000000 docrx-0.0.111/src/wrapper/infra/TextExtractor.c
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)   345115 2023-08-21 16:33:02.000000 docrx-0.0.111/src/wrapper/infra/VideoObjectsExtractor.c
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)   278651 2024-05-17 15:45:56.000000 docrx-0.0.111/src/wrapper/infra/WordFixer.c
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-08-15 18:18:13.000000 docrx-0.0.111/src/wrapper/infra/__init__.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-05-20 20:53:17.219263 docrx-0.0.111/src/wrapper/infra/res/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-08-15 18:18:13.000000 docrx-0.0.111/src/wrapper/infra/res/__init__.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-05-20 20:53:17.223263 docrx-0.0.111/tests/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3103 2024-05-20 19:42:05.000000 docrx-0.0.111/tests/test_TestProcessPDFImage.py
```

### Comparing `docrx-0.0.110/LICENSE.txt` & `docrx-0.0.111/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `docrx-0.0.110/PKG-INFO` & `docrx-0.0.111/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docrx
-Version: 0.0.110
+Version: 0.0.111
 Summary: search in documents
 Author: Tiago Zamperini
 Author-email: tiagozamperini@live.com
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Education
```

### Comparing `docrx-0.0.110/setup.cfg` & `docrx-0.0.111/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = docrx
-version = 0.0.110
+version = 0.0.111
 description = search in documents
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 author = Tiago Zamperini
 author_email = tiagozamperini@live.com
 classifiers =
```

### Comparing `docrx-0.0.110/setup.py` & `docrx-0.0.111/setup.py`

 * *Files identical despite different names*

### Comparing `docrx-0.0.110/src/docrx.egg-info/PKG-INFO` & `docrx-0.0.111/src/docrx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docrx
-Version: 0.0.110
+Version: 0.0.111
 Summary: search in documents
 Author: Tiago Zamperini
 Author-email: tiagozamperini@live.com
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Education
```

### Comparing `docrx-0.0.110/src/docrx.egg-info/SOURCES.txt` & `docrx-0.0.111/src/docrx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docrx-0.0.110/src/wrapper/Process.c` & `docrx-0.0.111/src/wrapper/Process.c`

 * *Files 2% similar despite different names*

```diff
@@ -1356,20 +1356,15 @@
 /* #### Code section: numeric_typedefs ### */
 /* #### Code section: complex_type_declarations ### */
 /* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
 struct __pyx_defaults;
 typedef struct __pyx_defaults __pyx_defaults;
-struct __pyx_defaults1;
-typedef struct __pyx_defaults1 __pyx_defaults1;
 struct __pyx_defaults {
-  PyObject *__pyx_arg_type;
-};
-struct __pyx_defaults1 {
   PyObject *__pyx_arg_translate_to;
 };
 /* #### Code section: utility_code_proto ### */
 
 /* --- Runtime support code (head) --- */
 /* Refnanny.proto */
 #ifndef CYTHON_REFNANNY
@@ -1987,15 +1982,15 @@
 static const char __pyx_k_TD[] = "TD";
 static const char __pyx_k__3[] = "";
 static const char __pyx_k_id[] = "id";
 static const char __pyx_k_os[] = "os";
 static const char __pyx_k_PDF[] = "PDF";
 static const char __pyx_k__12[] = ".";
 static const char __pyx_k__13[] = "*";
-static const char __pyx_k__34[] = "?";
+static const char __pyx_k__35[] = "?";
 static const char __pyx_k_csv[] = ".csv";
 static const char __pyx_k_doc[] = "doc";
 static const char __pyx_k_jpg[] = ".jpg";
 static const char __pyx_k_mp4[] = ".mp4";
 static const char __pyx_k_pdf[] = ".pdf";
 static const char __pyx_k_png[] = ".png";
 static const char __pyx_k_str[] = "str";
@@ -2114,17 +2109,16 @@
 static const char __pyx_k_python3_m_spacy_download_xx_ent[] = "python3 -m spacy download xx_ent_wiki_sm";
 static const char __pyx_k_Not_supported_extension_for_docu[] = "Not supported extension for document ";
 static const char __pyx_k_Process_create_online_pipeline_m[] = "Process.create_online_pipeline_multilingual";
 static const char __pyx_k_Without_support_for_document_wit[] = "Without support for document with extension .txt, .csv or .docx.";
 static const char __pyx_k_create_online_pipeline_multiling[] = "create_online_pipeline_multilingual";
 static const char __pyx_k_python3_m_spacy_download_pt_core[] = "python3 -m spacy download pt_core_news_sm";
 /* #### Code section: decls ### */
-static PyObject *__pyx_pf_7wrapper_7Process___defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_7wrapper_7Process_7Process___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_base_path, PyObject *__pyx_v_is_detect_language, PyObject *__pyx_v_translate_to, PyObject *__pyx_v_type); /* proto */
-static PyObject *__pyx_pf_7wrapper_7Process_2__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_7wrapper_7Process___defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_7wrapper_7Process_7Process_2create_online_pipeline_multilingual(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_base_path, PyObject *__pyx_v_is_detect_language, PyObject *__pyx_v_translate_to); /* proto */
 static PyObject *__pyx_pf_7wrapper_7Process_7Process_4create_batch_pipeline(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_base_path, PyObject *__pyx_v_is_detect_language, PyObject *__pyx_v_translate_to); /* proto */
 static PyObject *__pyx_pf_7wrapper_7Process_7Process_6compile_and_train(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_complement_path, PyObject *__pyx_v_file_index); /* proto */
 static PyObject *__pyx_pf_7wrapper_7Process_7Process_8compile_doc(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_complement_path, PyObject *__pyx_v_file_index); /* proto */
 static PyObject *__pyx_pf_7wrapper_7Process_7Process_10train_doc(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_file); /* proto */
 static PyObject *__pyx_pf_7wrapper_7Process_7Process_12search(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_query, PyObject *__pyx_v_detected_language, PyObject *__pyx_v_page, PyObject *__pyx_v_results_per_page); /* proto */
 static PyObject *__pyx_pf_7wrapper_7Process_7Process_14compile(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_base_path, PyObject *__pyx_v_complement_path, PyObject *__pyx_v_is_detect_language, PyObject *__pyx_v_translate_to); /* proto */
@@ -2189,15 +2183,15 @@
   PyObject *__pyx_n_s_SB;
   PyObject *__pyx_n_s_TD;
   PyObject *__pyx_n_s_Video;
   PyObject *__pyx_kp_u_Without_support_for_document_wit;
   PyObject *__pyx_kp_u__12;
   PyObject *__pyx_n_s__13;
   PyObject *__pyx_kp_u__3;
-  PyObject *__pyx_n_s__34;
+  PyObject *__pyx_n_s__35;
   PyObject *__pyx_n_s_annotations;
   PyObject *__pyx_n_s_asyncio_coroutines;
   PyObject *__pyx_n_s_base_path;
   PyObject *__pyx_n_s_bool;
   PyObject *__pyx_n_s_cline_in_traceback;
   PyObject *__pyx_n_s_compile;
   PyObject *__pyx_n_s_compile_and_train;
@@ -2302,32 +2296,33 @@
   PyObject *__pyx_tuple__7;
   PyObject *__pyx_tuple__8;
   PyObject *__pyx_tuple__9;
   PyObject *__pyx_tuple__10;
   PyObject *__pyx_tuple__11;
   PyObject *__pyx_tuple__14;
   PyObject *__pyx_tuple__16;
-  PyObject *__pyx_tuple__19;
+  PyObject *__pyx_tuple__17;
   PyObject *__pyx_tuple__20;
-  PyObject *__pyx_tuple__23;
-  PyObject *__pyx_tuple__25;
-  PyObject *__pyx_tuple__27;
+  PyObject *__pyx_tuple__21;
+  PyObject *__pyx_tuple__24;
+  PyObject *__pyx_tuple__26;
   PyObject *__pyx_tuple__28;
-  PyObject *__pyx_tuple__30;
+  PyObject *__pyx_tuple__29;
   PyObject *__pyx_tuple__31;
-  PyObject *__pyx_tuple__33;
+  PyObject *__pyx_tuple__32;
+  PyObject *__pyx_tuple__34;
   PyObject *__pyx_codeobj__15;
-  PyObject *__pyx_codeobj__17;
   PyObject *__pyx_codeobj__18;
-  PyObject *__pyx_codeobj__21;
+  PyObject *__pyx_codeobj__19;
   PyObject *__pyx_codeobj__22;
-  PyObject *__pyx_codeobj__24;
-  PyObject *__pyx_codeobj__26;
-  PyObject *__pyx_codeobj__29;
-  PyObject *__pyx_codeobj__32;
+  PyObject *__pyx_codeobj__23;
+  PyObject *__pyx_codeobj__25;
+  PyObject *__pyx_codeobj__27;
+  PyObject *__pyx_codeobj__30;
+  PyObject *__pyx_codeobj__33;
 } __pyx_mstate;
 
 #if CYTHON_USE_MODULE_STATE
 #ifdef __cplusplus
 namespace {
   extern struct PyModuleDef __pyx_moduledef;
 } /* anonymous namespace */
@@ -2397,15 +2392,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_SB);
   Py_CLEAR(clear_module_state->__pyx_n_s_TD);
   Py_CLEAR(clear_module_state->__pyx_n_s_Video);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Without_support_for_document_wit);
   Py_CLEAR(clear_module_state->__pyx_kp_u__12);
   Py_CLEAR(clear_module_state->__pyx_n_s__13);
   Py_CLEAR(clear_module_state->__pyx_kp_u__3);
-  Py_CLEAR(clear_module_state->__pyx_n_s__34);
+  Py_CLEAR(clear_module_state->__pyx_n_s__35);
   Py_CLEAR(clear_module_state->__pyx_n_s_annotations);
   Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
   Py_CLEAR(clear_module_state->__pyx_n_s_base_path);
   Py_CLEAR(clear_module_state->__pyx_n_s_bool);
   Py_CLEAR(clear_module_state->__pyx_n_s_cline_in_traceback);
   Py_CLEAR(clear_module_state->__pyx_n_s_compile);
   Py_CLEAR(clear_module_state->__pyx_n_s_compile_and_train);
@@ -2510,32 +2505,33 @@
   Py_CLEAR(clear_module_state->__pyx_tuple__7);
   Py_CLEAR(clear_module_state->__pyx_tuple__8);
   Py_CLEAR(clear_module_state->__pyx_tuple__9);
   Py_CLEAR(clear_module_state->__pyx_tuple__10);
   Py_CLEAR(clear_module_state->__pyx_tuple__11);
   Py_CLEAR(clear_module_state->__pyx_tuple__14);
   Py_CLEAR(clear_module_state->__pyx_tuple__16);
-  Py_CLEAR(clear_module_state->__pyx_tuple__19);
+  Py_CLEAR(clear_module_state->__pyx_tuple__17);
   Py_CLEAR(clear_module_state->__pyx_tuple__20);
-  Py_CLEAR(clear_module_state->__pyx_tuple__23);
-  Py_CLEAR(clear_module_state->__pyx_tuple__25);
-  Py_CLEAR(clear_module_state->__pyx_tuple__27);
+  Py_CLEAR(clear_module_state->__pyx_tuple__21);
+  Py_CLEAR(clear_module_state->__pyx_tuple__24);
+  Py_CLEAR(clear_module_state->__pyx_tuple__26);
   Py_CLEAR(clear_module_state->__pyx_tuple__28);
-  Py_CLEAR(clear_module_state->__pyx_tuple__30);
+  Py_CLEAR(clear_module_state->__pyx_tuple__29);
   Py_CLEAR(clear_module_state->__pyx_tuple__31);
-  Py_CLEAR(clear_module_state->__pyx_tuple__33);
+  Py_CLEAR(clear_module_state->__pyx_tuple__32);
+  Py_CLEAR(clear_module_state->__pyx_tuple__34);
   Py_CLEAR(clear_module_state->__pyx_codeobj__15);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__17);
   Py_CLEAR(clear_module_state->__pyx_codeobj__18);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__21);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__19);
   Py_CLEAR(clear_module_state->__pyx_codeobj__22);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__24);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__26);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__29);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__32);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__23);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__25);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__27);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__30);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__33);
   return 0;
 }
 #endif
 /* #### Code section: module_state_traverse ### */
 #if CYTHON_USE_MODULE_STATE
 static int __pyx_m_traverse(PyObject *m, visitproc visit, void *arg) {
   __pyx_mstate *traverse_module_state = __pyx_mstate(m);
@@ -2583,15 +2579,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_SB);
   Py_VISIT(traverse_module_state->__pyx_n_s_TD);
   Py_VISIT(traverse_module_state->__pyx_n_s_Video);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Without_support_for_document_wit);
   Py_VISIT(traverse_module_state->__pyx_kp_u__12);
   Py_VISIT(traverse_module_state->__pyx_n_s__13);
   Py_VISIT(traverse_module_state->__pyx_kp_u__3);
-  Py_VISIT(traverse_module_state->__pyx_n_s__34);
+  Py_VISIT(traverse_module_state->__pyx_n_s__35);
   Py_VISIT(traverse_module_state->__pyx_n_s_annotations);
   Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
   Py_VISIT(traverse_module_state->__pyx_n_s_base_path);
   Py_VISIT(traverse_module_state->__pyx_n_s_bool);
   Py_VISIT(traverse_module_state->__pyx_n_s_cline_in_traceback);
   Py_VISIT(traverse_module_state->__pyx_n_s_compile);
   Py_VISIT(traverse_module_state->__pyx_n_s_compile_and_train);
@@ -2696,32 +2692,33 @@
   Py_VISIT(traverse_module_state->__pyx_tuple__7);
   Py_VISIT(traverse_module_state->__pyx_tuple__8);
   Py_VISIT(traverse_module_state->__pyx_tuple__9);
   Py_VISIT(traverse_module_state->__pyx_tuple__10);
   Py_VISIT(traverse_module_state->__pyx_tuple__11);
   Py_VISIT(traverse_module_state->__pyx_tuple__14);
   Py_VISIT(traverse_module_state->__pyx_tuple__16);
-  Py_VISIT(traverse_module_state->__pyx_tuple__19);
+  Py_VISIT(traverse_module_state->__pyx_tuple__17);
   Py_VISIT(traverse_module_state->__pyx_tuple__20);
-  Py_VISIT(traverse_module_state->__pyx_tuple__23);
-  Py_VISIT(traverse_module_state->__pyx_tuple__25);
-  Py_VISIT(traverse_module_state->__pyx_tuple__27);
+  Py_VISIT(traverse_module_state->__pyx_tuple__21);
+  Py_VISIT(traverse_module_state->__pyx_tuple__24);
+  Py_VISIT(traverse_module_state->__pyx_tuple__26);
   Py_VISIT(traverse_module_state->__pyx_tuple__28);
-  Py_VISIT(traverse_module_state->__pyx_tuple__30);
+  Py_VISIT(traverse_module_state->__pyx_tuple__29);
   Py_VISIT(traverse_module_state->__pyx_tuple__31);
-  Py_VISIT(traverse_module_state->__pyx_tuple__33);
+  Py_VISIT(traverse_module_state->__pyx_tuple__32);
+  Py_VISIT(traverse_module_state->__pyx_tuple__34);
   Py_VISIT(traverse_module_state->__pyx_codeobj__15);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__17);
   Py_VISIT(traverse_module_state->__pyx_codeobj__18);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__21);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__19);
   Py_VISIT(traverse_module_state->__pyx_codeobj__22);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__24);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__26);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__29);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__32);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__23);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__25);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__27);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__30);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__33);
   return 0;
 }
 #endif
 /* #### Code section: module_state_defines ### */
 #define __pyx_d __pyx_mstate_global->__pyx_d
 #define __pyx_b __pyx_mstate_global->__pyx_b
 #define __pyx_cython_runtime __pyx_mstate_global->__pyx_cython_runtime
@@ -2779,15 +2776,15 @@
 #define __pyx_n_s_SB __pyx_mstate_global->__pyx_n_s_SB
 #define __pyx_n_s_TD __pyx_mstate_global->__pyx_n_s_TD
 #define __pyx_n_s_Video __pyx_mstate_global->__pyx_n_s_Video
 #define __pyx_kp_u_Without_support_for_document_wit __pyx_mstate_global->__pyx_kp_u_Without_support_for_document_wit
 #define __pyx_kp_u__12 __pyx_mstate_global->__pyx_kp_u__12
 #define __pyx_n_s__13 __pyx_mstate_global->__pyx_n_s__13
 #define __pyx_kp_u__3 __pyx_mstate_global->__pyx_kp_u__3
-#define __pyx_n_s__34 __pyx_mstate_global->__pyx_n_s__34
+#define __pyx_n_s__35 __pyx_mstate_global->__pyx_n_s__35
 #define __pyx_n_s_annotations __pyx_mstate_global->__pyx_n_s_annotations
 #define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
 #define __pyx_n_s_base_path __pyx_mstate_global->__pyx_n_s_base_path
 #define __pyx_n_s_bool __pyx_mstate_global->__pyx_n_s_bool
 #define __pyx_n_s_cline_in_traceback __pyx_mstate_global->__pyx_n_s_cline_in_traceback
 #define __pyx_n_s_compile __pyx_mstate_global->__pyx_n_s_compile
 #define __pyx_n_s_compile_and_train __pyx_mstate_global->__pyx_n_s_compile_and_train
@@ -2892,96 +2889,52 @@
 #define __pyx_tuple__7 __pyx_mstate_global->__pyx_tuple__7
 #define __pyx_tuple__8 __pyx_mstate_global->__pyx_tuple__8
 #define __pyx_tuple__9 __pyx_mstate_global->__pyx_tuple__9
 #define __pyx_tuple__10 __pyx_mstate_global->__pyx_tuple__10
 #define __pyx_tuple__11 __pyx_mstate_global->__pyx_tuple__11
 #define __pyx_tuple__14 __pyx_mstate_global->__pyx_tuple__14
 #define __pyx_tuple__16 __pyx_mstate_global->__pyx_tuple__16
-#define __pyx_tuple__19 __pyx_mstate_global->__pyx_tuple__19
+#define __pyx_tuple__17 __pyx_mstate_global->__pyx_tuple__17
 #define __pyx_tuple__20 __pyx_mstate_global->__pyx_tuple__20
-#define __pyx_tuple__23 __pyx_mstate_global->__pyx_tuple__23
-#define __pyx_tuple__25 __pyx_mstate_global->__pyx_tuple__25
-#define __pyx_tuple__27 __pyx_mstate_global->__pyx_tuple__27
+#define __pyx_tuple__21 __pyx_mstate_global->__pyx_tuple__21
+#define __pyx_tuple__24 __pyx_mstate_global->__pyx_tuple__24
+#define __pyx_tuple__26 __pyx_mstate_global->__pyx_tuple__26
 #define __pyx_tuple__28 __pyx_mstate_global->__pyx_tuple__28
-#define __pyx_tuple__30 __pyx_mstate_global->__pyx_tuple__30
+#define __pyx_tuple__29 __pyx_mstate_global->__pyx_tuple__29
 #define __pyx_tuple__31 __pyx_mstate_global->__pyx_tuple__31
-#define __pyx_tuple__33 __pyx_mstate_global->__pyx_tuple__33
+#define __pyx_tuple__32 __pyx_mstate_global->__pyx_tuple__32
+#define __pyx_tuple__34 __pyx_mstate_global->__pyx_tuple__34
 #define __pyx_codeobj__15 __pyx_mstate_global->__pyx_codeobj__15
-#define __pyx_codeobj__17 __pyx_mstate_global->__pyx_codeobj__17
 #define __pyx_codeobj__18 __pyx_mstate_global->__pyx_codeobj__18
-#define __pyx_codeobj__21 __pyx_mstate_global->__pyx_codeobj__21
+#define __pyx_codeobj__19 __pyx_mstate_global->__pyx_codeobj__19
 #define __pyx_codeobj__22 __pyx_mstate_global->__pyx_codeobj__22
-#define __pyx_codeobj__24 __pyx_mstate_global->__pyx_codeobj__24
-#define __pyx_codeobj__26 __pyx_mstate_global->__pyx_codeobj__26
-#define __pyx_codeobj__29 __pyx_mstate_global->__pyx_codeobj__29
-#define __pyx_codeobj__32 __pyx_mstate_global->__pyx_codeobj__32
+#define __pyx_codeobj__23 __pyx_mstate_global->__pyx_codeobj__23
+#define __pyx_codeobj__25 __pyx_mstate_global->__pyx_codeobj__25
+#define __pyx_codeobj__27 __pyx_mstate_global->__pyx_codeobj__27
+#define __pyx_codeobj__30 __pyx_mstate_global->__pyx_codeobj__30
+#define __pyx_codeobj__33 __pyx_mstate_global->__pyx_codeobj__33
 /* #### Code section: module_code ### */
 
 /* "wrapper/Process.pyx":29
  *     document_search = None
  * 
- *     def __init__(self, base_path, is_detect_language=False, translate_to:DocLanguage=None, type:ModelType=ModelType.SB) -> None:             # <<<<<<<<<<<<<<
+ *     def __init__(self, base_path, is_detect_language=False, translate_to:DocLanguage=None, type:ModelType=None) -> None:             # <<<<<<<<<<<<<<
  *         """
  *         Initialize the pipeline
  */
 
-static PyObject *__pyx_pf_7wrapper_7Process___defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__defaults__", 0);
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 29, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_INCREF(((PyObject *)Py_False));
-  __Pyx_GIVEREF(((PyObject *)Py_False));
-  PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)Py_False));
-  __Pyx_INCREF(((PyObject *)Py_None));
-  __Pyx_GIVEREF(((PyObject *)Py_None));
-  PyTuple_SET_ITEM(__pyx_t_1, 1, ((PyObject *)Py_None));
-  __Pyx_INCREF(__Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_self)->__pyx_arg_type);
-  __Pyx_GIVEREF(__Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_self)->__pyx_arg_type);
-  PyTuple_SET_ITEM(__pyx_t_1, 2, __Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_self)->__pyx_arg_type);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 29, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
-  __Pyx_INCREF(Py_None);
-  __Pyx_GIVEREF(Py_None);
-  PyTuple_SET_ITEM(__pyx_t_2, 1, Py_None);
-  __pyx_t_1 = 0;
-  __pyx_r = __pyx_t_2;
-  __pyx_t_2 = 0;
-  goto __pyx_L0;
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_AddTraceback("wrapper.Process.__defaults__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
 /* Python wrapper */
 static PyObject *__pyx_pw_7wrapper_7Process_7Process_1__init__(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7wrapper_7Process_7Process___init__, "Process.__init__(self, base_path, is_detect_language=False, translate_to: DocLanguage = None, type: ModelType = ModelType.SB) -> None\n\n        Initialize the pipeline\n        Arguments:\n            base_path: the folder where the resouses are stored like files and compiled models\n            is_detect_language: if true, detect the document language for tokenization and stemmetization.\n            in this case, the compiled model for search in documents will be splitted by the language detected.\n            translate_to: the document text will be translated by one of the translated languages (pt, en or es)\n            type:sb or td\n        Returns:\n            None\n        ");
+PyDoc_STRVAR(__pyx_doc_7wrapper_7Process_7Process___init__, "Process.__init__(self, base_path, is_detect_language=False, translate_to: DocLanguage = None, type: ModelType = None) -> None\n\n        Initialize the pipeline\n        Arguments:\n            base_path: the folder where the resouses are stored like files and compiled models\n            is_detect_language: if true, detect the document language for tokenization and stemmetization.\n            in this case, the compiled model for search in documents will be splitted by the language detected.\n            translate_to: the document text will be translated by one of the translated languages (pt, en or es)\n            type:sb or td\n        Returns:\n            None\n        ");
 static PyMethodDef __pyx_mdef_7wrapper_7Process_7Process_1__init__ = {"__init__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7wrapper_7Process_7Process_1__init__, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7wrapper_7Process_7Process___init__};
 static PyObject *__pyx_pw_7wrapper_7Process_7Process_1__init__(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
@@ -3000,18 +2953,17 @@
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_base_path,&__pyx_n_s_is_detect_language,&__pyx_n_s_translate_to,&__pyx_n_s_type,0};
     PyObject* values[5] = {0,0,0,0,0};
-    __pyx_defaults *__pyx_dynamic_args = __Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_self);
     values[2] = ((PyObject *)((PyObject *)Py_False));
     values[3] = ((PyObject *)((PyObject *)Py_None));
-    values[4] = __pyx_dynamic_args->__pyx_arg_type;
+    values[4] = ((PyObject *)((PyObject *)Py_None));
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
         case  5: values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
@@ -3426,15 +3378,15 @@
     if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_document_search, Py_None) < 0) __PYX_ERR(0, 54, __pyx_L1_error)
   }
   __pyx_L4:;
 
   /* "wrapper/Process.pyx":29
  *     document_search = None
  * 
- *     def __init__(self, base_path, is_detect_language=False, translate_to:DocLanguage=None, type:ModelType=ModelType.SB) -> None:             # <<<<<<<<<<<<<<
+ *     def __init__(self, base_path, is_detect_language=False, translate_to:DocLanguage=None, type:ModelType=None) -> None:             # <<<<<<<<<<<<<<
  *         """
  *         Initialize the pipeline
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
@@ -3457,15 +3409,15 @@
  *             self.document_search = None
  * 
  *     @staticmethod             # <<<<<<<<<<<<<<
  *     def create_online_pipeline_multilingual(base_path, is_detect_language=True, translate_to:DocLanguage=DocLanguage.ENGLISH):
  *         return Process(base_path, is_detect_language, translate_to, ModelType.SB)
  */
 
-static PyObject *__pyx_pf_7wrapper_7Process_2__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_7wrapper_7Process___defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -3480,17 +3432,17 @@
  * 
  */
   __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 56, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(((PyObject *)Py_True));
   __Pyx_GIVEREF(((PyObject *)Py_True));
   PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)Py_True));
-  __Pyx_INCREF(__Pyx_CyFunction_Defaults(__pyx_defaults1, __pyx_self)->__pyx_arg_translate_to);
-  __Pyx_GIVEREF(__Pyx_CyFunction_Defaults(__pyx_defaults1, __pyx_self)->__pyx_arg_translate_to);
-  PyTuple_SET_ITEM(__pyx_t_1, 1, __Pyx_CyFunction_Defaults(__pyx_defaults1, __pyx_self)->__pyx_arg_translate_to);
+  __Pyx_INCREF(__Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_self)->__pyx_arg_translate_to);
+  __Pyx_GIVEREF(__Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_self)->__pyx_arg_translate_to);
+  PyTuple_SET_ITEM(__pyx_t_1, 1, __Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_self)->__pyx_arg_translate_to);
 
   /* "wrapper/Process.pyx":56
  *             self.document_search = None
  * 
  *     @staticmethod             # <<<<<<<<<<<<<<
  *     def create_online_pipeline_multilingual(base_path, is_detect_language=True, translate_to:DocLanguage=DocLanguage.ENGLISH):
  *         return Process(base_path, is_detect_language, translate_to, ModelType.SB)
@@ -3548,15 +3500,15 @@
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("create_online_pipeline_multilingual (wrapper)", 0);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_base_path,&__pyx_n_s_is_detect_language,&__pyx_n_s_translate_to,0};
     PyObject* values[3] = {0,0,0};
-    __pyx_defaults1 *__pyx_dynamic_args = __Pyx_CyFunction_Defaults(__pyx_defaults1, __pyx_self);
+    __pyx_defaults *__pyx_dynamic_args = __Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_self);
     values[1] = ((PyObject *)((PyObject *)Py_True));
     values[2] = __pyx_dynamic_args->__pyx_arg_translate_to;
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
         case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
@@ -6328,15 +6280,15 @@
     {&__pyx_n_s_SB, __pyx_k_SB, sizeof(__pyx_k_SB), 0, 0, 1, 1},
     {&__pyx_n_s_TD, __pyx_k_TD, sizeof(__pyx_k_TD), 0, 0, 1, 1},
     {&__pyx_n_s_Video, __pyx_k_Video, sizeof(__pyx_k_Video), 0, 0, 1, 1},
     {&__pyx_kp_u_Without_support_for_document_wit, __pyx_k_Without_support_for_document_wit, sizeof(__pyx_k_Without_support_for_document_wit), 0, 1, 0, 0},
     {&__pyx_kp_u__12, __pyx_k__12, sizeof(__pyx_k__12), 0, 1, 0, 0},
     {&__pyx_n_s__13, __pyx_k__13, sizeof(__pyx_k__13), 0, 0, 1, 1},
     {&__pyx_kp_u__3, __pyx_k__3, sizeof(__pyx_k__3), 0, 1, 0, 0},
-    {&__pyx_n_s__34, __pyx_k__34, sizeof(__pyx_k__34), 0, 0, 1, 1},
+    {&__pyx_n_s__35, __pyx_k__35, sizeof(__pyx_k__35), 0, 0, 1, 1},
     {&__pyx_n_s_annotations, __pyx_k_annotations, sizeof(__pyx_k_annotations), 0, 0, 1, 1},
     {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
     {&__pyx_n_s_base_path, __pyx_k_base_path, sizeof(__pyx_k_base_path), 0, 0, 1, 1},
     {&__pyx_n_s_bool, __pyx_k_bool, sizeof(__pyx_k_bool), 0, 0, 1, 1},
     {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
     {&__pyx_n_s_compile, __pyx_k_compile, sizeof(__pyx_k_compile), 0, 0, 1, 1},
     {&__pyx_n_s_compile_and_train, __pyx_k_compile_and_train, sizeof(__pyx_k_compile_and_train), 0, 0, 1, 1},
@@ -6547,124 +6499,127 @@
   __pyx_tuple__11 = PyTuple_Pack(1, __pyx_n_u_rslp); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 125, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__11);
   __Pyx_GIVEREF(__pyx_tuple__11);
 
   /* "wrapper/Process.pyx":29
  *     document_search = None
  * 
- *     def __init__(self, base_path, is_detect_language=False, translate_to:DocLanguage=None, type:ModelType=ModelType.SB) -> None:             # <<<<<<<<<<<<<<
+ *     def __init__(self, base_path, is_detect_language=False, translate_to:DocLanguage=None, type:ModelType=None) -> None:             # <<<<<<<<<<<<<<
  *         """
  *         Initialize the pipeline
  */
   __pyx_tuple__14 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_base_path, __pyx_n_s_is_detect_language, __pyx_n_s_translate_to, __pyx_n_s_type, __pyx_n_s_isExist); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 29, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__14);
   __Pyx_GIVEREF(__pyx_tuple__14);
   __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_wrapper_Process_pyx, __pyx_n_s_init, 29, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_tuple__16 = PyTuple_Pack(3, ((PyObject *)Py_False), ((PyObject *)Py_None), ((PyObject *)Py_None)); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__16);
+  __Pyx_GIVEREF(__pyx_tuple__16);
 
   /* "wrapper/Process.pyx":56
  *             self.document_search = None
  * 
  *     @staticmethod             # <<<<<<<<<<<<<<
  *     def create_online_pipeline_multilingual(base_path, is_detect_language=True, translate_to:DocLanguage=DocLanguage.ENGLISH):
  *         return Process(base_path, is_detect_language, translate_to, ModelType.SB)
  */
-  __pyx_tuple__16 = PyTuple_Pack(3, __pyx_n_s_base_path, __pyx_n_s_is_detect_language, __pyx_n_s_translate_to); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 56, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__16);
-  __Pyx_GIVEREF(__pyx_tuple__16);
-  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_wrapper_Process_pyx, __pyx_n_s_create_online_pipeline_multiling, 56, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(0, 56, __pyx_L1_error)
+  __pyx_tuple__17 = PyTuple_Pack(3, __pyx_n_s_base_path, __pyx_n_s_is_detect_language, __pyx_n_s_translate_to); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 56, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__17);
+  __Pyx_GIVEREF(__pyx_tuple__17);
+  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_wrapper_Process_pyx, __pyx_n_s_create_online_pipeline_multiling, 56, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(0, 56, __pyx_L1_error)
 
   /* "wrapper/Process.pyx":60
  *         return Process(base_path, is_detect_language, translate_to, ModelType.SB)
  * 
  *     @staticmethod             # <<<<<<<<<<<<<<
  *     def create_batch_pipeline(base_path, is_detect_language=False, translate_to=None):
  *         return Process(base_path, is_detect_language, translate_to, ModelType.TD)
  */
-  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_wrapper_Process_pyx, __pyx_n_s_create_batch_pipeline, 60, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(0, 60, __pyx_L1_error)
-  __pyx_tuple__19 = PyTuple_Pack(2, ((PyObject *)Py_False), ((PyObject *)Py_None)); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 60, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__19);
-  __Pyx_GIVEREF(__pyx_tuple__19);
+  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_wrapper_Process_pyx, __pyx_n_s_create_batch_pipeline, 60, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __pyx_tuple__20 = PyTuple_Pack(2, ((PyObject *)Py_False), ((PyObject *)Py_None)); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__20);
+  __Pyx_GIVEREF(__pyx_tuple__20);
 
   /* "wrapper/Process.pyx":64
  *         return Process(base_path, is_detect_language, translate_to, ModelType.TD)
  * 
  *     def compile_and_train(self, complement_path, file_index):             # <<<<<<<<<<<<<<
  *         file = self.compile_doc(complement_path, file_index)
  *         self.document_search.train_model(file)
  */
-  __pyx_tuple__20 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_complement_path, __pyx_n_s_file_index, __pyx_n_s_file); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 64, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__20);
-  __Pyx_GIVEREF(__pyx_tuple__20);
-  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_wrapper_Process_pyx, __pyx_n_s_compile_and_train, 64, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_tuple__21 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_complement_path, __pyx_n_s_file_index, __pyx_n_s_file); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__21);
+  __Pyx_GIVEREF(__pyx_tuple__21);
+  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_wrapper_Process_pyx, __pyx_n_s_compile_and_train, 64, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 64, __pyx_L1_error)
 
   /* "wrapper/Process.pyx":69
  *         return file
  * 
  *     def compile_doc(self, complement_path, file_index):             # <<<<<<<<<<<<<<
  *         file = Process.compile(self.base_path, complement_path, self.is_detect_language, self.translate_to)
  *         file.id = file_index
  */
-  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_wrapper_Process_pyx, __pyx_n_s_compile_doc, 69, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 69, __pyx_L1_error)
+  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_wrapper_Process_pyx, __pyx_n_s_compile_doc, 69, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 69, __pyx_L1_error)
 
   /* "wrapper/Process.pyx":74
  *         return file
  * 
  *     def train_doc(self, file):             # <<<<<<<<<<<<<<
  *         self.document_search.train_model(file)
  *         return file
  */
-  __pyx_tuple__23 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_file); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(0, 74, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__23);
-  __Pyx_GIVEREF(__pyx_tuple__23);
-  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_wrapper_Process_pyx, __pyx_n_s_train_doc, 74, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_tuple__24 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_file); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__24);
+  __Pyx_GIVEREF(__pyx_tuple__24);
+  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_wrapper_Process_pyx, __pyx_n_s_train_doc, 74, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 74, __pyx_L1_error)
 
   /* "wrapper/Process.pyx":78
  *         return file
  * 
  *     def search(self, query, detected_language:DocLanguage = None, page=1, results_per_page=10):             # <<<<<<<<<<<<<<
  *         detected_language, query = LanguageDetector.detect_lang(query, self.translate_to, detected_language)
  *         logging.info(f"Language detected: {detected_language} - Query: {query}")
  */
-  __pyx_tuple__25 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_query, __pyx_n_s_detected_language, __pyx_n_s_page, __pyx_n_s_results_per_page, __pyx_n_s_lang_to_search); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(0, 78, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__25);
-  __Pyx_GIVEREF(__pyx_tuple__25);
-  __pyx_codeobj__26 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_wrapper_Process_pyx, __pyx_n_s_search, 78, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__26)) __PYX_ERR(0, 78, __pyx_L1_error)
-  __pyx_tuple__27 = PyTuple_Pack(3, ((PyObject *)Py_None), ((PyObject *)__pyx_int_1), ((PyObject *)__pyx_int_10)); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(0, 78, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__27);
-  __Pyx_GIVEREF(__pyx_tuple__27);
+  __pyx_tuple__26 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_query, __pyx_n_s_detected_language, __pyx_n_s_page, __pyx_n_s_results_per_page, __pyx_n_s_lang_to_search); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__26);
+  __Pyx_GIVEREF(__pyx_tuple__26);
+  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_wrapper_Process_pyx, __pyx_n_s_search, 78, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_tuple__28 = PyTuple_Pack(3, ((PyObject *)Py_None), ((PyObject *)__pyx_int_1), ((PyObject *)__pyx_int_10)); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__28);
+  __Pyx_GIVEREF(__pyx_tuple__28);
 
   /* "wrapper/Process.pyx":88
  *         return self.document_search.search_documents(query, lang_to_search, page, results_per_page)
  * 
  *     @staticmethod             # <<<<<<<<<<<<<<
  *     def compile(base_path, complement_path, is_detect_language=False, translate_to:DocLanguage=None) -> File:
  *         doc = None
  */
-  __pyx_tuple__28 = PyTuple_Pack(7, __pyx_n_s_base_path, __pyx_n_s_complement_path, __pyx_n_s_is_detect_language, __pyx_n_s_translate_to, __pyx_n_s_doc, __pyx_n_s_file_path, __pyx_n_s_text); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 88, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__28);
-  __Pyx_GIVEREF(__pyx_tuple__28);
-  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_wrapper_Process_pyx, __pyx_n_s_compile, 88, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 88, __pyx_L1_error)
-  __pyx_tuple__30 = PyTuple_Pack(2, ((PyObject *)Py_False), ((PyObject *)Py_None)); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(0, 88, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__30);
-  __Pyx_GIVEREF(__pyx_tuple__30);
+  __pyx_tuple__29 = PyTuple_Pack(7, __pyx_n_s_base_path, __pyx_n_s_complement_path, __pyx_n_s_is_detect_language, __pyx_n_s_translate_to, __pyx_n_s_doc, __pyx_n_s_file_path, __pyx_n_s_text); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(0, 88, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__29);
+  __Pyx_GIVEREF(__pyx_tuple__29);
+  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_wrapper_Process_pyx, __pyx_n_s_compile, 88, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(0, 88, __pyx_L1_error)
+  __pyx_tuple__31 = PyTuple_Pack(2, ((PyObject *)Py_False), ((PyObject *)Py_None)); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(0, 88, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__31);
+  __Pyx_GIVEREF(__pyx_tuple__31);
 
   /* "wrapper/Process.pyx":115
  *         return doc
  * 
  *     @staticmethod             # <<<<<<<<<<<<<<
  *     def load(download_dir=None):
  *         logging.info("Downloading resources...")
  */
-  __pyx_tuple__31 = PyTuple_Pack(1, __pyx_n_s_download_dir); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(0, 115, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__31);
-  __Pyx_GIVEREF(__pyx_tuple__31);
-  __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__31, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_wrapper_Process_pyx, __pyx_n_s_load, 115, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(0, 115, __pyx_L1_error)
-  __pyx_tuple__33 = PyTuple_Pack(1, ((PyObject *)Py_None)); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(0, 115, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__33);
-  __Pyx_GIVEREF(__pyx_tuple__33);
+  __pyx_tuple__32 = PyTuple_Pack(1, __pyx_n_s_download_dir); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(0, 115, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__32);
+  __Pyx_GIVEREF(__pyx_tuple__32);
+  __pyx_codeobj__33 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__32, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_wrapper_Process_pyx, __pyx_n_s_load, 115, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__33)) __PYX_ERR(0, 115, __pyx_L1_error)
+  __pyx_tuple__34 = PyTuple_Pack(1, ((PyObject *)Py_None)); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(0, 115, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__34);
+  __Pyx_GIVEREF(__pyx_tuple__34);
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
@@ -7284,42 +7239,33 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "wrapper/Process.pyx":27
  *     is_detect_language:bool
  *     translate_to:DocLanguage
  *     document_search = None             # <<<<<<<<<<<<<<
  * 
- *     def __init__(self, base_path, is_detect_language=False, translate_to:DocLanguage=None, type:ModelType=ModelType.SB) -> None:
+ *     def __init__(self, base_path, is_detect_language=False, translate_to:DocLanguage=None, type:ModelType=None) -> None:
  */
   if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_document_search, Py_None) < 0) __PYX_ERR(0, 27, __pyx_L1_error)
 
   /* "wrapper/Process.pyx":29
  *     document_search = None
  * 
- *     def __init__(self, base_path, is_detect_language=False, translate_to:DocLanguage=None, type:ModelType=ModelType.SB) -> None:             # <<<<<<<<<<<<<<
+ *     def __init__(self, base_path, is_detect_language=False, translate_to:DocLanguage=None, type:ModelType=None) -> None:             # <<<<<<<<<<<<<<
  *         """
  *         Initialize the pipeline
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 29, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_translate_to, __pyx_n_s_DocLanguage) < 0) __PYX_ERR(0, 29, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_type, __pyx_n_s_ModelType) < 0) __PYX_ERR(0, 29, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_None) < 0) __PYX_ERR(0, 29, __pyx_L1_error)
   __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7wrapper_7Process_7Process_1__init__, 0, __pyx_n_s_Process___init, NULL, __pyx_n_s_wrapper_Process, __pyx_d, ((PyObject *)__pyx_codeobj__15)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 29, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_4, sizeof(__pyx_defaults), 1)) __PYX_ERR(0, 29, __pyx_L1_error)
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_ModelType); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 29, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_SB); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 29, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_t_4)->__pyx_arg_type = __pyx_t_6;
-  __Pyx_GIVEREF(__pyx_t_6);
-  __pyx_t_6 = 0;
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_4, __pyx_pf_7wrapper_7Process___defaults__);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_4, __pyx_tuple__16);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_init, __pyx_t_4) < 0) __PYX_ERR(0, 29, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "wrapper/Process.pyx":56
  *             self.document_search = None
@@ -7327,34 +7273,34 @@
  *     @staticmethod             # <<<<<<<<<<<<<<
  *     def create_online_pipeline_multilingual(base_path, is_detect_language=True, translate_to:DocLanguage=DocLanguage.ENGLISH):
  *         return Process(base_path, is_detect_language, translate_to, ModelType.SB)
  */
   __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 56, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_translate_to, __pyx_n_s_DocLanguage) < 0) __PYX_ERR(0, 56, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7wrapper_7Process_7Process_3create_online_pipeline_multilingual, __Pyx_CYFUNCTION_STATICMETHOD, __pyx_n_s_Process_create_online_pipeline_m, NULL, __pyx_n_s_wrapper_Process, __pyx_d, ((PyObject *)__pyx_codeobj__17)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 56, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7wrapper_7Process_7Process_3create_online_pipeline_multilingual, __Pyx_CYFUNCTION_STATICMETHOD, __pyx_n_s_Process_create_online_pipeline_m, NULL, __pyx_n_s_wrapper_Process, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 56, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_2, sizeof(__pyx_defaults1), 1)) __PYX_ERR(0, 56, __pyx_L1_error)
+  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_2, sizeof(__pyx_defaults), 1)) __PYX_ERR(0, 56, __pyx_L1_error)
 
   /* "wrapper/Process.pyx":57
  * 
  *     @staticmethod
  *     def create_online_pipeline_multilingual(base_path, is_detect_language=True, translate_to:DocLanguage=DocLanguage.ENGLISH):             # <<<<<<<<<<<<<<
  *         return Process(base_path, is_detect_language, translate_to, ModelType.SB)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_DocLanguage); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 57, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_ENGLISH); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 57, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_DocLanguage); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __Pyx_CyFunction_Defaults(__pyx_defaults1, __pyx_t_2)->__pyx_arg_translate_to = __pyx_t_5;
-  __Pyx_GIVEREF(__pyx_t_5);
-  __pyx_t_5 = 0;
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_2, __pyx_pf_7wrapper_7Process_2__defaults__);
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_ENGLISH); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 57, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_t_2)->__pyx_arg_translate_to = __pyx_t_6;
+  __Pyx_GIVEREF(__pyx_t_6);
+  __pyx_t_6 = 0;
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_2, __pyx_pf_7wrapper_7Process___defaults__);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_4);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "wrapper/Process.pyx":56
  *             self.document_search = None
  * 
  *     @staticmethod             # <<<<<<<<<<<<<<
@@ -7370,72 +7316,72 @@
   /* "wrapper/Process.pyx":60
  *         return Process(base_path, is_detect_language, translate_to, ModelType.SB)
  * 
  *     @staticmethod             # <<<<<<<<<<<<<<
  *     def create_batch_pipeline(base_path, is_detect_language=False, translate_to=None):
  *         return Process(base_path, is_detect_language, translate_to, ModelType.TD)
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7wrapper_7Process_7Process_5create_batch_pipeline, __Pyx_CYFUNCTION_STATICMETHOD, __pyx_n_s_Process_create_batch_pipeline, NULL, __pyx_n_s_wrapper_Process, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7wrapper_7Process_7Process_5create_batch_pipeline, __Pyx_CYFUNCTION_STATICMETHOD, __pyx_n_s_Process_create_batch_pipeline, NULL, __pyx_n_s_wrapper_Process, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 60, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_4, __pyx_tuple__19);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_4, __pyx_tuple__20);
   __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_staticmethod, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 60, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_create_batch_pipeline, __pyx_t_2) < 0) __PYX_ERR(0, 60, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "wrapper/Process.pyx":64
  *         return Process(base_path, is_detect_language, translate_to, ModelType.TD)
  * 
  *     def compile_and_train(self, complement_path, file_index):             # <<<<<<<<<<<<<<
  *         file = self.compile_doc(complement_path, file_index)
  *         self.document_search.train_model(file)
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7wrapper_7Process_7Process_7compile_and_train, 0, __pyx_n_s_Process_compile_and_train, NULL, __pyx_n_s_wrapper_Process, __pyx_d, ((PyObject *)__pyx_codeobj__21)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7wrapper_7Process_7Process_7compile_and_train, 0, __pyx_n_s_Process_compile_and_train, NULL, __pyx_n_s_wrapper_Process, __pyx_d, ((PyObject *)__pyx_codeobj__22)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_compile_and_train, __pyx_t_2) < 0) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "wrapper/Process.pyx":69
  *         return file
  * 
  *     def compile_doc(self, complement_path, file_index):             # <<<<<<<<<<<<<<
  *         file = Process.compile(self.base_path, complement_path, self.is_detect_language, self.translate_to)
  *         file.id = file_index
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7wrapper_7Process_7Process_9compile_doc, 0, __pyx_n_s_Process_compile_doc, NULL, __pyx_n_s_wrapper_Process, __pyx_d, ((PyObject *)__pyx_codeobj__22)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 69, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7wrapper_7Process_7Process_9compile_doc, 0, __pyx_n_s_Process_compile_doc, NULL, __pyx_n_s_wrapper_Process, __pyx_d, ((PyObject *)__pyx_codeobj__23)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 69, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_compile_doc, __pyx_t_2) < 0) __PYX_ERR(0, 69, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "wrapper/Process.pyx":74
  *         return file
  * 
  *     def train_doc(self, file):             # <<<<<<<<<<<<<<
  *         self.document_search.train_model(file)
  *         return file
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7wrapper_7Process_7Process_11train_doc, 0, __pyx_n_s_Process_train_doc, NULL, __pyx_n_s_wrapper_Process, __pyx_d, ((PyObject *)__pyx_codeobj__24)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7wrapper_7Process_7Process_11train_doc, 0, __pyx_n_s_Process_train_doc, NULL, __pyx_n_s_wrapper_Process, __pyx_d, ((PyObject *)__pyx_codeobj__25)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 74, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_train_doc, __pyx_t_2) < 0) __PYX_ERR(0, 74, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "wrapper/Process.pyx":78
  *         return file
  * 
  *     def search(self, query, detected_language:DocLanguage = None, page=1, results_per_page=10):             # <<<<<<<<<<<<<<
  *         detected_language, query = LanguageDetector.detect_lang(query, self.translate_to, detected_language)
  *         logging.info(f"Language detected: {detected_language} - Query: {query}")
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_detected_language, __pyx_n_s_DocLanguage) < 0) __PYX_ERR(0, 78, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7wrapper_7Process_7Process_13search, 0, __pyx_n_s_Process_search, NULL, __pyx_n_s_wrapper_Process, __pyx_d, ((PyObject *)__pyx_codeobj__26)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7wrapper_7Process_7Process_13search, 0, __pyx_n_s_Process_search, NULL, __pyx_n_s_wrapper_Process, __pyx_d, ((PyObject *)__pyx_codeobj__27)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_4, __pyx_tuple__27);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_4, __pyx_tuple__28);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_search, __pyx_t_4) < 0) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "wrapper/Process.pyx":88
  *         return self.document_search.search_documents(query, lang_to_search, page, results_per_page)
@@ -7444,17 +7390,17 @@
  *     def compile(base_path, complement_path, is_detect_language=False, translate_to:DocLanguage=None) -> File:
  *         doc = None
  */
   __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 88, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_translate_to, __pyx_n_s_DocLanguage) < 0) __PYX_ERR(0, 88, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_n_s_File) < 0) __PYX_ERR(0, 88, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7wrapper_7Process_7Process_15compile, __Pyx_CYFUNCTION_STATICMETHOD, __pyx_n_s_Process_compile, NULL, __pyx_n_s_wrapper_Process, __pyx_d, ((PyObject *)__pyx_codeobj__29)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 88, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7wrapper_7Process_7Process_15compile, __Pyx_CYFUNCTION_STATICMETHOD, __pyx_n_s_Process_compile, NULL, __pyx_n_s_wrapper_Process, __pyx_d, ((PyObject *)__pyx_codeobj__30)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 88, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__30);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__31);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_4);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_staticmethod, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 88, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_compile, __pyx_t_4) < 0) __PYX_ERR(0, 88, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
@@ -7462,17 +7408,17 @@
   /* "wrapper/Process.pyx":115
  *         return doc
  * 
  *     @staticmethod             # <<<<<<<<<<<<<<
  *     def load(download_dir=None):
  *         logging.info("Downloading resources...")
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7wrapper_7Process_7Process_17load, __Pyx_CYFUNCTION_STATICMETHOD, __pyx_n_s_Process_load, NULL, __pyx_n_s_wrapper_Process, __pyx_d, ((PyObject *)__pyx_codeobj__32)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 115, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7wrapper_7Process_7Process_17load, __Pyx_CYFUNCTION_STATICMETHOD, __pyx_n_s_Process_load, NULL, __pyx_n_s_wrapper_Process, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 115, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_4, __pyx_tuple__33);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_4, __pyx_tuple__34);
   __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_staticmethod, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 115, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_load, __pyx_t_2) < 0) __PYX_ERR(0, 115, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "wrapper/Process.pyx":22
@@ -10557,15 +10503,15 @@
 static __Pyx_TypeName
 __Pyx_PyType_GetName(PyTypeObject* tp)
 {
     PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
                                                __pyx_n_s_name);
     if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
         PyErr_Clear();
-        Py_XSETREF(name, __Pyx_NewRef(__pyx_n_s__34));
+        Py_XSETREF(name, __Pyx_NewRef(__pyx_n_s__35));
     }
     return name;
 }
 #endif
 
 /* CIntToPy */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
```

### Comparing `docrx-0.0.110/src/wrapper/core/DocumentSearch.c` & `docrx-0.0.111/src/wrapper/core/DocumentSearch.c`

 * *Files identical despite different names*

### Comparing `docrx-0.0.110/src/wrapper/core/DocumentSearchSB.c` & `docrx-0.0.111/src/wrapper/core/DocumentSearchSB.c`

 * *Files identical despite different names*

### Comparing `docrx-0.0.110/src/wrapper/core/DocumentSearchTD.c` & `docrx-0.0.111/src/wrapper/core/DocumentSearchTD.c`

 * *Files identical despite different names*

### Comparing `docrx-0.0.110/src/wrapper/core/File.c` & `docrx-0.0.111/src/wrapper/core/File.c`

 * *Files identical despite different names*

### Comparing `docrx-0.0.110/src/wrapper/core/Image.c` & `docrx-0.0.111/src/wrapper/core/Image.c`

 * *Files identical despite different names*

### Comparing `docrx-0.0.110/src/wrapper/core/PDF.c` & `docrx-0.0.111/src/wrapper/core/PDF.c`

 * *Files identical despite different names*

### Comparing `docrx-0.0.110/src/wrapper/core/SentenceTransformerVectorizer.c` & `docrx-0.0.111/src/wrapper/core/SentenceTransformerVectorizer.c`

 * *Files 0% similar despite different names*

```diff
@@ -1964,20 +1964,19 @@
 int __pyx_module_is_main_wrapper__core__SentenceTransformerVectorizer = 0;
 
 /* Implementation of "wrapper.core.SentenceTransformerVectorizer" */
 /* #### Code section: global_var ### */
 static PyObject *__pyx_builtin_super;
 /* #### Code section: string_decls ### */
 static const char __pyx_k_[] = ".";
-static const char __pyx_k__8[] = "?";
+static const char __pyx_k__9[] = "?";
 static const char __pyx_k_cls[] = "cls";
 static const char __pyx_k_doc[] = "__doc__";
 static const char __pyx_k_File[] = "File";
 static const char __pyx_k_dict[] = "__dict__";
-static const char __pyx_k_file[] = "file";
 static const char __pyx_k_init[] = "__init__";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_path[] = "path";
 static const char __pyx_k_self[] = "self";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_text[] = "text";
@@ -2019,15 +2018,15 @@
 static const char __pyx_k_src_wrapper_core_SentenceTransfo[] = "src/wrapper/core/SentenceTransformerVectorizer.pyx";
 static const char __pyx_k_wrapper_core_SentenceTransformer[] = "wrapper.core.SentenceTransformerVectorizer";
 /* #### Code section: decls ### */
 static PyObject *__pyx_pf_7wrapper_4core_29SentenceTransformerVectorizer___defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_7wrapper_4core_29SentenceTransformerVectorizer_29SentenceTransformerVectorizer___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_path, PyObject *__pyx_v_vect_lang, PyObject *__pyx_v_corpus_name); /* proto */
 static PyObject *__pyx_pf_7wrapper_4core_29SentenceTransformerVectorizer_2__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_7wrapper_4core_29SentenceTransformerVectorizer_29SentenceTransformerVectorizer_2instance(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_cls, PyObject *__pyx_v_path, PyObject *__pyx_v_vect_lang, PyObject *__pyx_v_corpus_name); /* proto */
-static PyObject *__pyx_pf_7wrapper_4core_29SentenceTransformerVectorizer_29SentenceTransformerVectorizer_4encode(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_file); /* proto */
+static PyObject *__pyx_pf_7wrapper_4core_29SentenceTransformerVectorizer_29SentenceTransformerVectorizer_4encode(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_text, PyObject *__pyx_v_convert_to_tensor); /* proto */
 /* #### Code section: late_includes ### */
 /* #### Code section: module_state ### */
 typedef struct {
   PyObject *__pyx_d;
   PyObject *__pyx_b;
   PyObject *__pyx_cython_runtime;
   PyObject *__pyx_empty_tuple;
@@ -2059,26 +2058,25 @@
   PyObject *__pyx_n_s_File;
   PyObject *__pyx_n_s_SentenceTransformer;
   PyObject *__pyx_n_s_SentenceTransformerVectorizer;
   PyObject *__pyx_n_s_SentenceTransformerVectorizer_2;
   PyObject *__pyx_n_s_SentenceTransformerVectorizer_en;
   PyObject *__pyx_n_s_SentenceTransformerVectorizer_in;
   PyObject *__pyx_n_s_Vectorizer;
-  PyObject *__pyx_n_s__8;
+  PyObject *__pyx_n_s__9;
   PyObject *__pyx_kp_u_all_MiniLM_L6_v2;
   PyObject *__pyx_n_s_asyncio_coroutines;
   PyObject *__pyx_n_s_cline_in_traceback;
   PyObject *__pyx_n_s_cls;
   PyObject *__pyx_n_s_convert_to_tensor;
   PyObject *__pyx_n_s_corpus;
   PyObject *__pyx_n_s_corpus_name;
   PyObject *__pyx_n_s_dict;
   PyObject *__pyx_n_s_doc;
   PyObject *__pyx_n_s_encode;
-  PyObject *__pyx_n_s_file;
   PyObject *__pyx_n_s_import;
   PyObject *__pyx_n_s_infra_DocLanguage;
   PyObject *__pyx_n_s_init;
   PyObject *__pyx_n_s_init_subclass;
   PyObject *__pyx_n_s_instance;
   PyObject *__pyx_n_s_instance_2;
   PyObject *__pyx_n_s_is_coroutine;
@@ -2103,14 +2101,15 @@
   PyObject *__pyx_n_s_test;
   PyObject *__pyx_n_s_text;
   PyObject *__pyx_n_s_vect_lang;
   PyObject *__pyx_n_s_wrapper_core_SentenceTransformer;
   PyObject *__pyx_tuple__2;
   PyObject *__pyx_tuple__4;
   PyObject *__pyx_tuple__6;
+  PyObject *__pyx_tuple__8;
   PyObject *__pyx_codeobj__3;
   PyObject *__pyx_codeobj__5;
   PyObject *__pyx_codeobj__7;
 } __pyx_mstate;
 
 #if CYTHON_USE_MODULE_STATE
 #ifdef __cplusplus
@@ -2158,26 +2157,25 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_File);
   Py_CLEAR(clear_module_state->__pyx_n_s_SentenceTransformer);
   Py_CLEAR(clear_module_state->__pyx_n_s_SentenceTransformerVectorizer);
   Py_CLEAR(clear_module_state->__pyx_n_s_SentenceTransformerVectorizer_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_SentenceTransformerVectorizer_en);
   Py_CLEAR(clear_module_state->__pyx_n_s_SentenceTransformerVectorizer_in);
   Py_CLEAR(clear_module_state->__pyx_n_s_Vectorizer);
-  Py_CLEAR(clear_module_state->__pyx_n_s__8);
+  Py_CLEAR(clear_module_state->__pyx_n_s__9);
   Py_CLEAR(clear_module_state->__pyx_kp_u_all_MiniLM_L6_v2);
   Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
   Py_CLEAR(clear_module_state->__pyx_n_s_cline_in_traceback);
   Py_CLEAR(clear_module_state->__pyx_n_s_cls);
   Py_CLEAR(clear_module_state->__pyx_n_s_convert_to_tensor);
   Py_CLEAR(clear_module_state->__pyx_n_s_corpus);
   Py_CLEAR(clear_module_state->__pyx_n_s_corpus_name);
   Py_CLEAR(clear_module_state->__pyx_n_s_dict);
   Py_CLEAR(clear_module_state->__pyx_n_s_doc);
   Py_CLEAR(clear_module_state->__pyx_n_s_encode);
-  Py_CLEAR(clear_module_state->__pyx_n_s_file);
   Py_CLEAR(clear_module_state->__pyx_n_s_import);
   Py_CLEAR(clear_module_state->__pyx_n_s_infra_DocLanguage);
   Py_CLEAR(clear_module_state->__pyx_n_s_init);
   Py_CLEAR(clear_module_state->__pyx_n_s_init_subclass);
   Py_CLEAR(clear_module_state->__pyx_n_s_instance);
   Py_CLEAR(clear_module_state->__pyx_n_s_instance_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_is_coroutine);
@@ -2202,14 +2200,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_test);
   Py_CLEAR(clear_module_state->__pyx_n_s_text);
   Py_CLEAR(clear_module_state->__pyx_n_s_vect_lang);
   Py_CLEAR(clear_module_state->__pyx_n_s_wrapper_core_SentenceTransformer);
   Py_CLEAR(clear_module_state->__pyx_tuple__2);
   Py_CLEAR(clear_module_state->__pyx_tuple__4);
   Py_CLEAR(clear_module_state->__pyx_tuple__6);
+  Py_CLEAR(clear_module_state->__pyx_tuple__8);
   Py_CLEAR(clear_module_state->__pyx_codeobj__3);
   Py_CLEAR(clear_module_state->__pyx_codeobj__5);
   Py_CLEAR(clear_module_state->__pyx_codeobj__7);
   return 0;
 }
 #endif
 /* #### Code section: module_state_traverse ### */
@@ -2235,26 +2234,25 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_File);
   Py_VISIT(traverse_module_state->__pyx_n_s_SentenceTransformer);
   Py_VISIT(traverse_module_state->__pyx_n_s_SentenceTransformerVectorizer);
   Py_VISIT(traverse_module_state->__pyx_n_s_SentenceTransformerVectorizer_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_SentenceTransformerVectorizer_en);
   Py_VISIT(traverse_module_state->__pyx_n_s_SentenceTransformerVectorizer_in);
   Py_VISIT(traverse_module_state->__pyx_n_s_Vectorizer);
-  Py_VISIT(traverse_module_state->__pyx_n_s__8);
+  Py_VISIT(traverse_module_state->__pyx_n_s__9);
   Py_VISIT(traverse_module_state->__pyx_kp_u_all_MiniLM_L6_v2);
   Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
   Py_VISIT(traverse_module_state->__pyx_n_s_cline_in_traceback);
   Py_VISIT(traverse_module_state->__pyx_n_s_cls);
   Py_VISIT(traverse_module_state->__pyx_n_s_convert_to_tensor);
   Py_VISIT(traverse_module_state->__pyx_n_s_corpus);
   Py_VISIT(traverse_module_state->__pyx_n_s_corpus_name);
   Py_VISIT(traverse_module_state->__pyx_n_s_dict);
   Py_VISIT(traverse_module_state->__pyx_n_s_doc);
   Py_VISIT(traverse_module_state->__pyx_n_s_encode);
-  Py_VISIT(traverse_module_state->__pyx_n_s_file);
   Py_VISIT(traverse_module_state->__pyx_n_s_import);
   Py_VISIT(traverse_module_state->__pyx_n_s_infra_DocLanguage);
   Py_VISIT(traverse_module_state->__pyx_n_s_init);
   Py_VISIT(traverse_module_state->__pyx_n_s_init_subclass);
   Py_VISIT(traverse_module_state->__pyx_n_s_instance);
   Py_VISIT(traverse_module_state->__pyx_n_s_instance_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_is_coroutine);
@@ -2279,14 +2277,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_test);
   Py_VISIT(traverse_module_state->__pyx_n_s_text);
   Py_VISIT(traverse_module_state->__pyx_n_s_vect_lang);
   Py_VISIT(traverse_module_state->__pyx_n_s_wrapper_core_SentenceTransformer);
   Py_VISIT(traverse_module_state->__pyx_tuple__2);
   Py_VISIT(traverse_module_state->__pyx_tuple__4);
   Py_VISIT(traverse_module_state->__pyx_tuple__6);
+  Py_VISIT(traverse_module_state->__pyx_tuple__8);
   Py_VISIT(traverse_module_state->__pyx_codeobj__3);
   Py_VISIT(traverse_module_state->__pyx_codeobj__5);
   Py_VISIT(traverse_module_state->__pyx_codeobj__7);
   return 0;
 }
 #endif
 /* #### Code section: module_state_defines ### */
@@ -2322,26 +2321,25 @@
 #define __pyx_n_s_File __pyx_mstate_global->__pyx_n_s_File
 #define __pyx_n_s_SentenceTransformer __pyx_mstate_global->__pyx_n_s_SentenceTransformer
 #define __pyx_n_s_SentenceTransformerVectorizer __pyx_mstate_global->__pyx_n_s_SentenceTransformerVectorizer
 #define __pyx_n_s_SentenceTransformerVectorizer_2 __pyx_mstate_global->__pyx_n_s_SentenceTransformerVectorizer_2
 #define __pyx_n_s_SentenceTransformerVectorizer_en __pyx_mstate_global->__pyx_n_s_SentenceTransformerVectorizer_en
 #define __pyx_n_s_SentenceTransformerVectorizer_in __pyx_mstate_global->__pyx_n_s_SentenceTransformerVectorizer_in
 #define __pyx_n_s_Vectorizer __pyx_mstate_global->__pyx_n_s_Vectorizer
-#define __pyx_n_s__8 __pyx_mstate_global->__pyx_n_s__8
+#define __pyx_n_s__9 __pyx_mstate_global->__pyx_n_s__9
 #define __pyx_kp_u_all_MiniLM_L6_v2 __pyx_mstate_global->__pyx_kp_u_all_MiniLM_L6_v2
 #define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
 #define __pyx_n_s_cline_in_traceback __pyx_mstate_global->__pyx_n_s_cline_in_traceback
 #define __pyx_n_s_cls __pyx_mstate_global->__pyx_n_s_cls
 #define __pyx_n_s_convert_to_tensor __pyx_mstate_global->__pyx_n_s_convert_to_tensor
 #define __pyx_n_s_corpus __pyx_mstate_global->__pyx_n_s_corpus
 #define __pyx_n_s_corpus_name __pyx_mstate_global->__pyx_n_s_corpus_name
 #define __pyx_n_s_dict __pyx_mstate_global->__pyx_n_s_dict
 #define __pyx_n_s_doc __pyx_mstate_global->__pyx_n_s_doc
 #define __pyx_n_s_encode __pyx_mstate_global->__pyx_n_s_encode
-#define __pyx_n_s_file __pyx_mstate_global->__pyx_n_s_file
 #define __pyx_n_s_import __pyx_mstate_global->__pyx_n_s_import
 #define __pyx_n_s_infra_DocLanguage __pyx_mstate_global->__pyx_n_s_infra_DocLanguage
 #define __pyx_n_s_init __pyx_mstate_global->__pyx_n_s_init
 #define __pyx_n_s_init_subclass __pyx_mstate_global->__pyx_n_s_init_subclass
 #define __pyx_n_s_instance __pyx_mstate_global->__pyx_n_s_instance
 #define __pyx_n_s_instance_2 __pyx_mstate_global->__pyx_n_s_instance_2
 #define __pyx_n_s_is_coroutine __pyx_mstate_global->__pyx_n_s_is_coroutine
@@ -2366,14 +2364,15 @@
 #define __pyx_n_s_test __pyx_mstate_global->__pyx_n_s_test
 #define __pyx_n_s_text __pyx_mstate_global->__pyx_n_s_text
 #define __pyx_n_s_vect_lang __pyx_mstate_global->__pyx_n_s_vect_lang
 #define __pyx_n_s_wrapper_core_SentenceTransformer __pyx_mstate_global->__pyx_n_s_wrapper_core_SentenceTransformer
 #define __pyx_tuple__2 __pyx_mstate_global->__pyx_tuple__2
 #define __pyx_tuple__4 __pyx_mstate_global->__pyx_tuple__4
 #define __pyx_tuple__6 __pyx_mstate_global->__pyx_tuple__6
+#define __pyx_tuple__8 __pyx_mstate_global->__pyx_tuple__8
 #define __pyx_codeobj__3 __pyx_mstate_global->__pyx_codeobj__3
 #define __pyx_codeobj__5 __pyx_mstate_global->__pyx_codeobj__5
 #define __pyx_codeobj__7 __pyx_mstate_global->__pyx_codeobj__7
 /* #### Code section: module_code ### */
 
 /* "wrapper/core/SentenceTransformerVectorizer.pyx":12
  *     _instance = None
@@ -3080,15 +3079,15 @@
   }
 
   /* "wrapper/core/SentenceTransformerVectorizer.pyx":29
  *         if cls._instance is None:
  *             cls._instance = cls(path, vect_lang, corpus_name)
  *         return cls._instance             # <<<<<<<<<<<<<<
  * 
- *     def encode(self, file:File):
+ *     def encode(self, text, convert_to_tensor=False):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_cls, __pyx_n_s_instance); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 29, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
@@ -3113,53 +3112,57 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "wrapper/core/SentenceTransformerVectorizer.pyx":31
  *         return cls._instance
  * 
- *     def encode(self, file:File):             # <<<<<<<<<<<<<<
- *         return self.model.encode(file.text, convert_to_tensor=False)
+ *     def encode(self, text, convert_to_tensor=False):             # <<<<<<<<<<<<<<
+ *         return self.model.encode(text, convert_to_tensor=convert_to_tensor)
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_7wrapper_4core_29SentenceTransformerVectorizer_29SentenceTransformerVectorizer_5encode(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7wrapper_4core_29SentenceTransformerVectorizer_29SentenceTransformerVectorizer_4encode, "SentenceTransformerVectorizer.encode(self, file: File)");
+PyDoc_STRVAR(__pyx_doc_7wrapper_4core_29SentenceTransformerVectorizer_29SentenceTransformerVectorizer_4encode, "SentenceTransformerVectorizer.encode(self, text, convert_to_tensor=False)");
 static PyMethodDef __pyx_mdef_7wrapper_4core_29SentenceTransformerVectorizer_29SentenceTransformerVectorizer_5encode = {"encode", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7wrapper_4core_29SentenceTransformerVectorizer_29SentenceTransformerVectorizer_5encode, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7wrapper_4core_29SentenceTransformerVectorizer_29SentenceTransformerVectorizer_4encode};
 static PyObject *__pyx_pw_7wrapper_4core_29SentenceTransformerVectorizer_29SentenceTransformerVectorizer_5encode(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
-  PyObject *__pyx_v_file = 0;
+  PyObject *__pyx_v_text = 0;
+  PyObject *__pyx_v_convert_to_tensor = 0;
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("encode (wrapper)", 0);
   {
-    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_file,0};
-    PyObject* values[2] = {0,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_text,&__pyx_n_s_convert_to_tensor,0};
+    PyObject* values[3] = {0,0,0};
+    values[2] = ((PyObject *)((PyObject *)Py_False));
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
         case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
@@ -3167,95 +3170,105 @@
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) kw_args--;
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 31, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_file)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_text)) != 0)) kw_args--;
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 31, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("encode", 1, 2, 2, 1); __PYX_ERR(0, 31, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("encode", 0, 2, 3, 1); __PYX_ERR(0, 31, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  2:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_convert_to_tensor);
+          if (value) { values[2] = value; kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 31, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "encode") < 0)) __PYX_ERR(0, 31, __pyx_L3_error)
       }
-    } else if (unlikely(__pyx_nargs != 2)) {
-      goto __pyx_L5_argtuple_error;
     } else {
-      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
-      values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+      switch (__pyx_nargs) {
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+        values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        break;
+        default: goto __pyx_L5_argtuple_error;
+      }
     }
     __pyx_v_self = values[0];
-    __pyx_v_file = values[1];
+    __pyx_v_text = values[1];
+    __pyx_v_convert_to_tensor = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("encode", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 31, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("encode", 0, 2, 3, __pyx_nargs); __PYX_ERR(0, 31, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("wrapper.core.SentenceTransformerVectorizer.SentenceTransformerVectorizer.encode", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7wrapper_4core_29SentenceTransformerVectorizer_29SentenceTransformerVectorizer_4encode(__pyx_self, __pyx_v_self, __pyx_v_file);
+  __pyx_r = __pyx_pf_7wrapper_4core_29SentenceTransformerVectorizer_29SentenceTransformerVectorizer_4encode(__pyx_self, __pyx_v_self, __pyx_v_text, __pyx_v_convert_to_tensor);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7wrapper_4core_29SentenceTransformerVectorizer_29SentenceTransformerVectorizer_4encode(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_file) {
+static PyObject *__pyx_pf_7wrapper_4core_29SentenceTransformerVectorizer_29SentenceTransformerVectorizer_4encode(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_text, PyObject *__pyx_v_convert_to_tensor) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("encode", 0);
 
   /* "wrapper/core/SentenceTransformerVectorizer.pyx":32
  * 
- *     def encode(self, file:File):
- *         return self.model.encode(file.text, convert_to_tensor=False)             # <<<<<<<<<<<<<<
+ *     def encode(self, text, convert_to_tensor=False):
+ *         return self.model.encode(text, convert_to_tensor=convert_to_tensor)             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_model); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 32, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 32, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_file, __pyx_n_s_text); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 32, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 32, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 32, __pyx_L1_error)
+  __Pyx_INCREF(__pyx_v_text);
+  __Pyx_GIVEREF(__pyx_v_text);
+  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_text);
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 32, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
-  __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 32, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_convert_to_tensor, Py_False) < 0) __PYX_ERR(0, 32, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 32, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_convert_to_tensor, __pyx_v_convert_to_tensor) < 0) __PYX_ERR(0, 32, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 32, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
   /* "wrapper/core/SentenceTransformerVectorizer.pyx":31
  *         return cls._instance
  * 
- *     def encode(self, file:File):             # <<<<<<<<<<<<<<
- *         return self.model.encode(file.text, convert_to_tensor=False)
+ *     def encode(self, text, convert_to_tensor=False):             # <<<<<<<<<<<<<<
+ *         return self.model.encode(text, convert_to_tensor=convert_to_tensor)
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
@@ -3290,26 +3303,25 @@
     {&__pyx_n_s_File, __pyx_k_File, sizeof(__pyx_k_File), 0, 0, 1, 1},
     {&__pyx_n_s_SentenceTransformer, __pyx_k_SentenceTransformer, sizeof(__pyx_k_SentenceTransformer), 0, 0, 1, 1},
     {&__pyx_n_s_SentenceTransformerVectorizer, __pyx_k_SentenceTransformerVectorizer, sizeof(__pyx_k_SentenceTransformerVectorizer), 0, 0, 1, 1},
     {&__pyx_n_s_SentenceTransformerVectorizer_2, __pyx_k_SentenceTransformerVectorizer_2, sizeof(__pyx_k_SentenceTransformerVectorizer_2), 0, 0, 1, 1},
     {&__pyx_n_s_SentenceTransformerVectorizer_en, __pyx_k_SentenceTransformerVectorizer_en, sizeof(__pyx_k_SentenceTransformerVectorizer_en), 0, 0, 1, 1},
     {&__pyx_n_s_SentenceTransformerVectorizer_in, __pyx_k_SentenceTransformerVectorizer_in, sizeof(__pyx_k_SentenceTransformerVectorizer_in), 0, 0, 1, 1},
     {&__pyx_n_s_Vectorizer, __pyx_k_Vectorizer, sizeof(__pyx_k_Vectorizer), 0, 0, 1, 1},
-    {&__pyx_n_s__8, __pyx_k__8, sizeof(__pyx_k__8), 0, 0, 1, 1},
+    {&__pyx_n_s__9, __pyx_k__9, sizeof(__pyx_k__9), 0, 0, 1, 1},
     {&__pyx_kp_u_all_MiniLM_L6_v2, __pyx_k_all_MiniLM_L6_v2, sizeof(__pyx_k_all_MiniLM_L6_v2), 0, 1, 0, 0},
     {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
     {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
     {&__pyx_n_s_cls, __pyx_k_cls, sizeof(__pyx_k_cls), 0, 0, 1, 1},
     {&__pyx_n_s_convert_to_tensor, __pyx_k_convert_to_tensor, sizeof(__pyx_k_convert_to_tensor), 0, 0, 1, 1},
     {&__pyx_n_s_corpus, __pyx_k_corpus, sizeof(__pyx_k_corpus), 0, 0, 1, 1},
     {&__pyx_n_s_corpus_name, __pyx_k_corpus_name, sizeof(__pyx_k_corpus_name), 0, 0, 1, 1},
     {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
     {&__pyx_n_s_doc, __pyx_k_doc, sizeof(__pyx_k_doc), 0, 0, 1, 1},
     {&__pyx_n_s_encode, __pyx_k_encode, sizeof(__pyx_k_encode), 0, 0, 1, 1},
-    {&__pyx_n_s_file, __pyx_k_file, sizeof(__pyx_k_file), 0, 0, 1, 1},
     {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
     {&__pyx_n_s_infra_DocLanguage, __pyx_k_infra_DocLanguage, sizeof(__pyx_k_infra_DocLanguage), 0, 0, 1, 1},
     {&__pyx_n_s_init, __pyx_k_init, sizeof(__pyx_k_init), 0, 0, 1, 1},
     {&__pyx_n_s_init_subclass, __pyx_k_init_subclass, sizeof(__pyx_k_init_subclass), 0, 0, 1, 1},
     {&__pyx_n_s_instance, __pyx_k_instance, sizeof(__pyx_k_instance), 0, 0, 1, 1},
     {&__pyx_n_s_instance_2, __pyx_k_instance_2, sizeof(__pyx_k_instance_2), 0, 0, 1, 1},
     {&__pyx_n_s_is_coroutine, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
@@ -3375,21 +3387,24 @@
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
   __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_wrapper_core_SentenceTransfo, __pyx_n_s_instance_2, 25, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 25, __pyx_L1_error)
 
   /* "wrapper/core/SentenceTransformerVectorizer.pyx":31
  *         return cls._instance
  * 
- *     def encode(self, file:File):             # <<<<<<<<<<<<<<
- *         return self.model.encode(file.text, convert_to_tensor=False)
+ *     def encode(self, text, convert_to_tensor=False):             # <<<<<<<<<<<<<<
+ *         return self.model.encode(text, convert_to_tensor=convert_to_tensor)
  */
-  __pyx_tuple__6 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_file); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __pyx_tuple__6 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_text, __pyx_n_s_convert_to_tensor); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
-  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_wrapper_core_SentenceTransfo, __pyx_n_s_encode, 31, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_wrapper_core_SentenceTransfo, __pyx_n_s_encode, 31, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __pyx_tuple__8 = PyTuple_Pack(1, ((PyObject *)Py_False)); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__8);
+  __Pyx_GIVEREF(__pyx_tuple__8);
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
@@ -3952,40 +3967,36 @@
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_instance_2, __pyx_t_7) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
   /* "wrapper/core/SentenceTransformerVectorizer.pyx":31
  *         return cls._instance
  * 
- *     def encode(self, file:File):             # <<<<<<<<<<<<<<
- *         return self.model.encode(file.text, convert_to_tensor=False)
+ *     def encode(self, text, convert_to_tensor=False):             # <<<<<<<<<<<<<<
+ *         return self.model.encode(text, convert_to_tensor=convert_to_tensor)
  */
-  __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_7wrapper_4core_29SentenceTransformerVectorizer_29SentenceTransformerVectorizer_5encode, 0, __pyx_n_s_SentenceTransformerVectorizer_en, NULL, __pyx_n_s_wrapper_core_SentenceTransformer, __pyx_d, ((PyObject *)__pyx_codeobj__7)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_file, __pyx_n_s_File) < 0) __PYX_ERR(0, 31, __pyx_L1_error)
-  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_7wrapper_4core_29SentenceTransformerVectorizer_29SentenceTransformerVectorizer_5encode, 0, __pyx_n_s_SentenceTransformerVectorizer_en, NULL, __pyx_n_s_wrapper_core_SentenceTransformer, __pyx_d, ((PyObject *)__pyx_codeobj__7)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 31, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_6, __pyx_t_7);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_7, __pyx_tuple__8);
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_encode, __pyx_t_7) < 0) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_encode, __pyx_t_6) < 0) __PYX_ERR(0, 31, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
   /* "wrapper/core/SentenceTransformerVectorizer.pyx":8
  * 
  * # singleton pattern
  * class SentenceTransformerVectorizer(Vectorizer):             # <<<<<<<<<<<<<<
  * 
  *     _instance = None
  */
-  __pyx_t_6 = __Pyx_Py3ClassCreate(__pyx_t_4, __pyx_n_s_SentenceTransformerVectorizer, __pyx_t_2, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 8, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  if (__Pyx_CyFunction_InitClassCell(__pyx_t_3, __pyx_t_6) < 0) __PYX_ERR(0, 8, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_Py3ClassCreate(__pyx_t_4, __pyx_n_s_SentenceTransformerVectorizer, __pyx_t_2, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 8, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  if (__Pyx_CyFunction_InitClassCell(__pyx_t_3, __pyx_t_7) < 0) __PYX_ERR(0, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SentenceTransformerVectorizer, __pyx_t_6) < 0) __PYX_ERR(0, 8, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SentenceTransformerVectorizer, __pyx_t_7) < 0) __PYX_ERR(0, 8, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "wrapper/core/SentenceTransformerVectorizer.pyx":2
  * 
  * from .Vectorizer import Vectorizer             # <<<<<<<<<<<<<<
@@ -6795,15 +6806,15 @@
 static __Pyx_TypeName
 __Pyx_PyType_GetName(PyTypeObject* tp)
 {
     PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
                                                __pyx_n_s_name);
     if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
         PyErr_Clear();
-        Py_XSETREF(name, __Pyx_NewRef(__pyx_n_s__8));
+        Py_XSETREF(name, __Pyx_NewRef(__pyx_n_s__9));
     }
     return name;
 }
 #endif
 
 /* CIntToPy */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
```

### Comparing `docrx-0.0.110/src/wrapper/core/Vectorizer.c` & `docrx-0.0.111/src/wrapper/core/Vectorizer.c`

 * *Files identical despite different names*

### Comparing `docrx-0.0.110/src/wrapper/core/Video.c` & `docrx-0.0.111/src/wrapper/core/Video.c`

 * *Files identical despite different names*

### Comparing `docrx-0.0.110/src/wrapper/infra/AbsctractGenerator.c` & `docrx-0.0.111/src/wrapper/infra/AbsctractGenerator.c`

 * *Files identical despite different names*

### Comparing `docrx-0.0.110/src/wrapper/infra/DocLanguage.c` & `docrx-0.0.111/src/wrapper/infra/DocLanguage.c`

 * *Files identical despite different names*

### Comparing `docrx-0.0.110/src/wrapper/infra/ImageObjectsExtractor.c` & `docrx-0.0.111/src/wrapper/infra/ImageObjectsExtractor.c`

 * *Files identical despite different names*

### Comparing `docrx-0.0.110/src/wrapper/infra/LanguageDetector.c` & `docrx-0.0.111/src/wrapper/infra/LanguageDetector.c`

 * *Files identical despite different names*

### Comparing `docrx-0.0.110/src/wrapper/infra/ModelType.c` & `docrx-0.0.111/src/wrapper/infra/ModelType.c`

 * *Files identical despite different names*

### Comparing `docrx-0.0.110/src/wrapper/infra/NERExtractor.c` & `docrx-0.0.111/src/wrapper/infra/NERExtractor.c`

 * *Files identical despite different names*

### Comparing `docrx-0.0.110/src/wrapper/infra/PreProcessing.c` & `docrx-0.0.111/src/wrapper/infra/PreProcessing.c`

 * *Files identical despite different names*

### Comparing `docrx-0.0.110/src/wrapper/infra/TextExtractor.c` & `docrx-0.0.111/src/wrapper/infra/TextExtractor.c`

 * *Files identical despite different names*

### Comparing `docrx-0.0.110/src/wrapper/infra/VideoObjectsExtractor.c` & `docrx-0.0.111/src/wrapper/infra/VideoObjectsExtractor.c`

 * *Files identical despite different names*

### Comparing `docrx-0.0.110/src/wrapper/infra/WordFixer.c` & `docrx-0.0.111/src/wrapper/infra/WordFixer.c`

 * *Files identical despite different names*

### Comparing `docrx-0.0.110/tests/test_TestProcessPDFImage.py` & `docrx-0.0.111/tests/test_TestProcessPDFImage.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,42 +29,43 @@
             file = p.compile_doc('res/onus/pag1.pdf', 'res/onus/pag1.pdf')
             assert file and file.text
             logging.info('Extracted text: ' + file.extracted_text)
             logging.info('File translated text: ' + file.text)
             logging.info('sentences from text:')
             for index, s in enumerate(file.sentences):
                 logging.info(f'Sentence number {index}.Text: {s}')
-            vectorizer = SentenceTransformerVectorizer.instance(self.base_path, DocLanguage.PORTUGUESE)
-            vector = vectorizer.encode(file)
-            if vector is not None:
-                assert True
-            else:
-                assert False
-            logging.info(f'Language detected {file.detected_language} translate to {file.translate_to} Vector: {vector} for text {file.text}')
+                vectorizer = SentenceTransformerVectorizer.instance(self.base_path, DocLanguage.PORTUGUESE)
+                vector = vectorizer.encode(s)
+                if vector is not None:
+                    assert True
+                else:
+                    assert False
+                logging.info(f'vectorized sentence: {vector}')            
+            
+            logging.info(f'Language detected {file.detected_language} translate to {file.translate_to}')
         except:
             logging.error(traceback.format_exc())
             assert False
 
-    def test_search_on_file_by_sb(self):       
-        assert False 
-        logging.info('test_search_on_file_by_sb')
-        try:
-            p = Process.create_online_pipeline_multilingual(self.base_path)
-            file = p.compile_and_train('res/onus/pag1.pdf', 'res/onus/pag1.pdf')
-            assert file and file.text
-            logging.info('File text: ' + file.text)
-            logging.info('searching for: "Tereza Almeida"')
-            query, result = p.search("tereza almeida", page=1, results_per_page=10)
-            assert query and result
-            logging.info('Query: ' + query)
-            logging.info('Result: ')
-            logging.info(result)
-            query = "206.424-ES"
-            logging.info(f'searching for: {query}')
-            query, result = p.search(query, DocLanguage.PORTUGUESE, page=1, results_per_page=10)
-            assert query and result
-            logging.info('Query: ' + query)
-            logging.info('Result: ')
-            logging.info(result)
-        except:
-            logging.error(traceback.format_exc())
-            assert False
+    # def test_search_on_file_by_sb(self):
+    #     logging.info('test_search_on_file_by_sb')
+    #     try:
+    #         p = Process.create_online_pipeline_multilingual(self.base_path)
+    #         file = p.compile_and_train('res/onus/pag1.pdf', 'res/onus/pag1.pdf')
+    #         assert file and file.text
+    #         logging.info('File text: ' + file.text)
+    #         logging.info('searching for: "Tereza Almeida"')
+    #         query, result = p.search("tereza almeida", page=1, results_per_page=10)
+    #         assert query and result
+    #         logging.info('Query: ' + query)
+    #         logging.info('Result: ')
+    #         logging.info(result)
+    #         query = "206.424-ES"
+    #         logging.info(f'searching for: {query}')
+    #         query, result = p.search(query, DocLanguage.PORTUGUESE, page=1, results_per_page=10)
+    #         assert query and result
+    #         logging.info('Query: ' + query)
+    #         logging.info('Result: ')
+    #         logging.info(result)
+    #     except:
+    #         logging.error(traceback.format_exc())
+    #         assert False
```

