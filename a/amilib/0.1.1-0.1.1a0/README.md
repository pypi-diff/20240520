# Comparing `tmp/amilib-0.1.1.tar.gz` & `tmp/amilib-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/amilib-0.1.1.tar", last modified: Fri May 17 22:04:55 2024, max compression
+gzip compressed data, was "dist/amilib-0.1.1a0.tar", last modified: Mon May 20 07:48:16 2024, max compression
```

## Comparing `amilib-0.1.1.tar` & `amilib-0.1.1a0.tar`

### file list

```diff
@@ -1,40 +1,51 @@
-drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-05-17 22:04:55.424171 amilib-0.1.1/
--rw-r--r--   0 pm286      (503) staff       (20)      850 2024-05-17 22:04:55.424246 amilib-0.1.1/PKG-INFO
-drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-05-17 22:04:55.421061 amilib-0.1.1/amilib/
--rw-r--r--   0 pm286      (503) staff       (20)        0 2024-04-16 00:05:01.830761 amilib-0.1.1/amilib/__init__.py
--rw-r--r--   0 pm286      (503) staff       (20)     9811 2024-05-17 15:11:52.431271 amilib-0.1.1/amilib/ami_args.py
--rw-r--r--   0 pm286      (503) staff       (20)     5132 2024-05-10 07:45:14.848226 amilib-0.1.1/amilib/ami_bib.py
--rw-r--r--   0 pm286      (503) staff       (20)      287 2024-04-17 21:43:55.251516 amilib-0.1.1/amilib/ami_csv.py
--rw-r--r--   0 pm286      (503) staff       (20)   164403 2024-05-17 15:11:52.432392 amilib-0.1.1/amilib/ami_html.py
--rw-r--r--   0 pm286      (503) staff       (20)    16407 2024-05-15 10:50:48.747796 amilib-0.1.1/amilib/ami_integrate.py
--rw-r--r--   0 pm286      (503) staff       (20)     8542 2024-05-15 11:22:11.902271 amilib-0.1.1/amilib/ami_nlp.py
--rw-r--r--   0 pm286      (503) staff       (20)    81770 2024-05-15 10:50:48.748320 amilib-0.1.1/amilib/ami_pdf_libs.py
--rw-r--r--   0 pm286      (503) staff       (20)     5001 2024-05-15 10:50:48.748476 amilib-0.1.1/amilib/ami_svg.py
--rw-r--r--   0 pm286      (503) staff       (20)    10651 2024-04-16 00:05:01.831984 amilib-0.1.1/amilib/ami_util.py
--rw-r--r--   0 pm286      (503) staff       (20)     8422 2024-04-16 00:05:01.832063 amilib-0.1.1/amilib/amidriver.py
--rw-r--r--   0 pm286      (503) staff       (20)    17098 2024-05-17 21:28:55.457223 amilib-0.1.1/amilib/amix.py
--rw-r--r--   0 pm286      (503) staff       (20)    19721 2024-05-10 07:45:14.850101 amilib-0.1.1/amilib/bbox.py
--rw-r--r--   0 pm286      (503) staff       (20)    14824 2024-05-15 10:50:48.748870 amilib-0.1.1/amilib/file_lib.py
--rw-r--r--   0 pm286      (503) staff       (20)    19595 2024-05-10 07:45:14.850551 amilib-0.1.1/amilib/headless_lib.py
--rw-r--r--   0 pm286      (503) staff       (20)     4440 2024-05-17 15:11:52.432782 amilib-0.1.1/amilib/html_args.py
--rw-r--r--   0 pm286      (503) staff       (20)     1334 2024-04-23 06:25:16.187949 amilib-0.1.1/amilib/html_extra.py
--rw-r--r--   0 pm286      (503) staff       (20)    16556 2024-05-10 07:45:14.851089 amilib-0.1.1/amilib/html_generator.py
--rw-r--r--   0 pm286      (503) staff       (20)    48083 2024-05-10 07:45:14.851370 amilib-0.1.1/amilib/html_marker.py
--rw-r--r--   0 pm286      (503) staff       (20)    26450 2024-05-17 15:11:52.433165 amilib-0.1.1/amilib/pdf_args.py
--rw-r--r--   0 pm286      (503) staff       (20)    27640 2024-05-17 15:11:52.433562 amilib-0.1.1/amilib/util.py
--rw-r--r--   0 pm286      (503) staff       (20)    33690 2024-05-10 07:45:14.851892 amilib-0.1.1/amilib/wikimedia.py
--rw-r--r--   0 pm286      (503) staff       (20)    54474 2024-05-10 07:45:14.852158 amilib-0.1.1/amilib/xml_lib.py
--rw-r--r--   0 pm286      (503) staff       (20)     1666 2024-05-17 21:30:15.093611 amilib-0.1.1/setup.py
-drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-05-17 22:04:55.424106 amilib-0.1.1/test/
--rw-r--r--   0 pm286      (503) staff       (20)     2679 2024-04-17 00:12:33.325481 amilib-0.1.1/test/test_all.py
--rw-r--r--   0 pm286      (503) staff       (20)     3941 2024-04-18 07:09:52.218257 amilib-0.1.1/test/test_file.py
--rw-r--r--   0 pm286      (503) staff       (20)    21468 2024-05-10 08:49:13.862850 amilib-0.1.1/test/test_headless.py
--rw-r--r--   0 pm286      (503) staff       (20)   120399 2024-05-17 15:11:52.445559 amilib-0.1.1/test/test_html.py
--rw-r--r--   0 pm286      (503) staff       (20)      733 2024-04-16 00:05:02.394994 amilib-0.1.1/test/test_nlp.py
--rw-r--r--   0 pm286      (503) staff       (20)    80476 2024-05-17 15:11:52.445978 amilib-0.1.1/test/test_pdf.py
--rw-r--r--   0 pm286      (503) staff       (20)       92 2024-05-17 15:11:52.446099 amilib-0.1.1/test/test_pytest.py
--rw-r--r--   0 pm286      (503) staff       (20)     1087 2024-04-23 06:34:10.071353 amilib-0.1.1/test/test_stat.py
--rw-r--r--   0 pm286      (503) staff       (20)     1065 2024-04-16 00:05:02.395346 amilib-0.1.1/test/test_svg.py
--rw-r--r--   0 pm286      (503) staff       (20)    10568 2024-05-17 15:11:52.446284 amilib-0.1.1/test/test_util.py
--rw-r--r--   0 pm286      (503) staff       (20)    35765 2024-04-16 00:05:02.395578 amilib-0.1.1/test/test_wikidata.py
--rw-r--r--   0 pm286      (503) staff       (20)     4824 2024-04-23 06:34:10.078244 amilib-0.1.1/test/test_xml.py
+drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-05-20 07:48:16.112351 amilib-0.1.1a0/
+-rw-r--r--   0 pm286      (503) staff       (20)    11357 2024-04-16 00:05:01.000000 amilib-0.1.1a0/LICENSE
+-rw-r--r--   0 pm286      (503) staff       (20)     1179 2024-05-20 07:48:16.112139 amilib-0.1.1a0/PKG-INFO
+-rw-r--r--   0 pm286      (503) staff       (20)       76 2024-04-16 00:05:01.000000 amilib-0.1.1a0/README.md
+drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-05-20 07:48:16.106570 amilib-0.1.1a0/amilib/
+-rw-r--r--   0 pm286      (503) staff       (20)        0 2024-04-16 00:05:01.000000 amilib-0.1.1a0/amilib/__init__.py
+-rw-r--r--   0 pm286      (503) staff       (20)     9811 2024-05-17 15:11:52.000000 amilib-0.1.1a0/amilib/ami_args.py
+-rw-r--r--   0 pm286      (503) staff       (20)     5132 2024-05-10 07:45:14.000000 amilib-0.1.1a0/amilib/ami_bib.py
+-rw-r--r--   0 pm286      (503) staff       (20)      287 2024-04-17 21:43:55.000000 amilib-0.1.1a0/amilib/ami_csv.py
+-rw-r--r--   0 pm286      (503) staff       (20)   164403 2024-05-17 15:11:52.000000 amilib-0.1.1a0/amilib/ami_html.py
+-rw-r--r--   0 pm286      (503) staff       (20)    16407 2024-05-15 10:50:48.000000 amilib-0.1.1a0/amilib/ami_integrate.py
+-rw-r--r--   0 pm286      (503) staff       (20)     8542 2024-05-15 11:22:11.000000 amilib-0.1.1a0/amilib/ami_nlp.py
+-rw-r--r--   0 pm286      (503) staff       (20)    81770 2024-05-15 10:50:48.000000 amilib-0.1.1a0/amilib/ami_pdf_libs.py
+-rw-r--r--   0 pm286      (503) staff       (20)     5001 2024-05-15 10:50:48.000000 amilib-0.1.1a0/amilib/ami_svg.py
+-rw-r--r--   0 pm286      (503) staff       (20)    10651 2024-04-16 00:05:01.000000 amilib-0.1.1a0/amilib/ami_util.py
+-rw-r--r--   0 pm286      (503) staff       (20)     8422 2024-04-16 00:05:01.000000 amilib-0.1.1a0/amilib/amidriver.py
+-rw-r--r--   0 pm286      (503) staff       (20)    17166 2024-05-20 07:46:59.000000 amilib-0.1.1a0/amilib/amix.py
+-rw-r--r--   0 pm286      (503) staff       (20)    19721 2024-05-10 07:45:14.000000 amilib-0.1.1a0/amilib/bbox.py
+-rw-r--r--   0 pm286      (503) staff       (20)    14824 2024-05-15 10:50:48.000000 amilib-0.1.1a0/amilib/file_lib.py
+-rw-r--r--   0 pm286      (503) staff       (20)    19595 2024-05-10 07:45:14.000000 amilib-0.1.1a0/amilib/headless_lib.py
+-rw-r--r--   0 pm286      (503) staff       (20)     4440 2024-05-17 15:11:52.000000 amilib-0.1.1a0/amilib/html_args.py
+-rw-r--r--   0 pm286      (503) staff       (20)     1334 2024-04-23 06:25:16.000000 amilib-0.1.1a0/amilib/html_extra.py
+-rw-r--r--   0 pm286      (503) staff       (20)    16556 2024-05-10 07:45:14.000000 amilib-0.1.1a0/amilib/html_generator.py
+-rw-r--r--   0 pm286      (503) staff       (20)    48083 2024-05-10 07:45:14.000000 amilib-0.1.1a0/amilib/html_marker.py
+-rw-r--r--   0 pm286      (503) staff       (20)    26450 2024-05-17 15:11:52.000000 amilib-0.1.1a0/amilib/pdf_args.py
+-rw-r--r--   0 pm286      (503) staff       (20)    27640 2024-05-17 15:11:52.000000 amilib-0.1.1a0/amilib/util.py
+-rw-r--r--   0 pm286      (503) staff       (20)    33690 2024-05-10 07:45:14.000000 amilib-0.1.1a0/amilib/wikimedia.py
+-rw-r--r--   0 pm286      (503) staff       (20)    54508 2024-05-17 22:21:11.000000 amilib-0.1.1a0/amilib/xml_lib.py
+drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-05-20 07:48:16.111884 amilib-0.1.1a0/amilib.egg-info/
+-rw-r--r--   0 pm286      (503) staff       (20)     1179 2024-05-20 07:48:15.000000 amilib-0.1.1a0/amilib.egg-info/PKG-INFO
+-rw-r--r--   0 pm286      (503) staff       (20)      905 2024-05-20 07:48:15.000000 amilib-0.1.1a0/amilib.egg-info/SOURCES.txt
+-rw-r--r--   0 pm286      (503) staff       (20)        1 2024-05-20 07:48:15.000000 amilib-0.1.1a0/amilib.egg-info/dependency_links.txt
+-rw-r--r--   0 pm286      (503) staff       (20)       44 2024-05-20 07:48:15.000000 amilib-0.1.1a0/amilib.egg-info/entry_points.txt
+-rw-r--r--   0 pm286      (503) staff       (20)        1 2024-05-17 21:30:27.000000 amilib-0.1.1a0/amilib.egg-info/not-zip-safe
+-rw-r--r--   0 pm286      (503) staff       (20)      136 2024-05-20 07:48:15.000000 amilib-0.1.1a0/amilib.egg-info/requires.txt
+-rw-r--r--   0 pm286      (503) staff       (20)        7 2024-05-20 07:48:15.000000 amilib-0.1.1a0/amilib.egg-info/top_level.txt
+-rw-r--r--   0 pm286      (503) staff       (20)       38 2024-05-20 07:48:16.112399 amilib-0.1.1a0/setup.cfg
+-rw-r--r--   0 pm286      (503) staff       (20)     1667 2024-05-20 07:47:32.000000 amilib-0.1.1a0/setup.py
+drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-05-20 07:48:16.111562 amilib-0.1.1a0/test/
+-rw-r--r--   0 pm286      (503) staff       (20)     2679 2024-04-17 00:12:33.000000 amilib-0.1.1a0/test/test_all.py
+-rw-r--r--   0 pm286      (503) staff       (20)     3941 2024-04-18 07:09:52.000000 amilib-0.1.1a0/test/test_file.py
+-rw-r--r--   0 pm286      (503) staff       (20)    21468 2024-05-10 08:49:13.000000 amilib-0.1.1a0/test/test_headless.py
+-rw-r--r--   0 pm286      (503) staff       (20)   120399 2024-05-17 15:11:52.000000 amilib-0.1.1a0/test/test_html.py
+-rw-r--r--   0 pm286      (503) staff       (20)      733 2024-04-16 00:05:02.000000 amilib-0.1.1a0/test/test_nlp.py
+-rw-r--r--   0 pm286      (503) staff       (20)    80476 2024-05-17 15:11:52.000000 amilib-0.1.1a0/test/test_pdf.py
+-rw-r--r--   0 pm286      (503) staff       (20)       92 2024-05-17 15:11:52.000000 amilib-0.1.1a0/test/test_pytest.py
+-rw-r--r--   0 pm286      (503) staff       (20)     1087 2024-04-23 06:34:10.000000 amilib-0.1.1a0/test/test_stat.py
+-rw-r--r--   0 pm286      (503) staff       (20)     1065 2024-04-16 00:05:02.000000 amilib-0.1.1a0/test/test_svg.py
+-rw-r--r--   0 pm286      (503) staff       (20)    10568 2024-05-17 15:11:52.000000 amilib-0.1.1a0/test/test_util.py
+-rw-r--r--   0 pm286      (503) staff       (20)    35765 2024-04-16 00:05:02.000000 amilib-0.1.1a0/test/test_wikidata.py
+-rw-r--r--   0 pm286      (503) staff       (20)     4824 2024-04-23 06:34:10.000000 amilib-0.1.1a0/test/test_xml.py
```

### Comparing `amilib-0.1.1/amilib/ami_args.py` & `amilib-0.1.1a0/amilib/ami_args.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.1/amilib/ami_bib.py` & `amilib-0.1.1a0/amilib/ami_bib.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.1/amilib/ami_html.py` & `amilib-0.1.1a0/amilib/ami_html.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.1/amilib/ami_integrate.py` & `amilib-0.1.1a0/amilib/ami_integrate.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.1/amilib/ami_nlp.py` & `amilib-0.1.1a0/amilib/ami_nlp.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.1/amilib/ami_pdf_libs.py` & `amilib-0.1.1a0/amilib/ami_pdf_libs.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.1/amilib/ami_svg.py` & `amilib-0.1.1a0/amilib/ami_svg.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.1/amilib/ami_util.py` & `amilib-0.1.1a0/amilib/ami_util.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.1/amilib/amidriver.py` & `amilib-0.1.1a0/amilib/amidriver.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.1/amilib/amix.py` & `amilib-0.1.1a0/amilib/amix.py`

 * *Files 1% similar despite different names*

```diff
@@ -369,15 +369,16 @@
         # had to revert here I think
         version = '0.0.6'  # 2024-04-19
         version = '0.0.7'  # 2024-04-23
         version = '0.0.8'  # 2024-04-23
         version = '0.0.9'  # 2024-05-09
         version = '0.0.10'  # 2024-05-09
         version = '0.1.0'  # 2024-05-10 # fixed absolute imports and mended tests
-        version = '0.1.1'  # 2024-05-11 # fixed subclassig of AmiLibArgs
+        version = '0.1.1'  # 2024-05-11 # fixed subclassing of AmiLibArgs
+        version = '0.1.1a'  # 2024-05-11 # simple requirements.txt
 
         # logging.warn(f"VERSION {version}")
         return version
 
 
 class AmiLibArgs(AbstractArgs):
     """Parse args to analyze, edit and annotate HTML"""
```

### Comparing `amilib-0.1.1/amilib/bbox.py` & `amilib-0.1.1a0/amilib/bbox.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.1/amilib/file_lib.py` & `amilib-0.1.1a0/amilib/file_lib.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.1/amilib/headless_lib.py` & `amilib-0.1.1a0/amilib/headless_lib.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.1/amilib/html_args.py` & `amilib-0.1.1a0/amilib/html_args.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.1/amilib/html_extra.py` & `amilib-0.1.1a0/amilib/html_extra.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.1/amilib/html_generator.py` & `amilib-0.1.1a0/amilib/html_generator.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.1/amilib/html_marker.py` & `amilib-0.1.1a0/amilib/html_marker.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.1/amilib/pdf_args.py` & `amilib-0.1.1a0/amilib/pdf_args.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.1/amilib/util.py` & `amilib-0.1.1a0/amilib/util.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.1/amilib/wikimedia.py` & `amilib-0.1.1a0/amilib/wikimedia.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.1/amilib/xml_lib.py` & `amilib-0.1.1a0/amilib/xml_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 from pathlib import Path
 from urllib.request import urlopen
 
 import chardet
 import lxml
 import lxml.etree
 import requests
-import tkinterweb
+# import tkinterweb
 from lxml import etree as ET
 from lxml.etree import _Element, _ElementTree
 from lxml.html import HTMLParser
-import tkinter as tk
+# import tkinter as tk
 
 from amilib.file_lib import FileLib
 
 logging.debug("loading xml_lib")
 
 # make leafnodes and copy remaning content as XML
 TERMINAL_COPY = {
@@ -1500,30 +1500,30 @@
         # print(f" div_content {div_content[:maxchar]}")
         templater = Templater.create_template(template, regex)
         id = templater.match_template(div_content, template_type=ID_TEMPLATE)
         print(f">>id {id}")
         return id
 
 
-class Web:
-    def __init__(self):
-        root = tk.Tk()
-        site = "http://google.com"
-        self.display_html(root, site)
-        root.mainloop()
-
-    @classmethod
-    def display_html(cls, master, site):
-        frame = tkinterweb.HtmlFrame(master)
-        frame.load_website(site)
-        frame.pack(fill="both", expand=True)
-
-    @classmethod
-    def tkinterweb_demo(cls):
-        tkinterweb.Demo()
+# class Web:
+#     def __init__(self):
+#         root = tk.Tk()
+#         site = "http://google.com"
+#         self.display_html(root, site)
+#         root.mainloop()
+#
+#     @classmethod
+#     def display_html(cls, master, site):
+#         frame = tkinterweb.HtmlFrame(master)
+#         frame.load_website(site)
+#         frame.pack(fill="both", expand=True)
+#
+#     @classmethod
+#     def tkinterweb_demo(cls):
+#         tkinterweb.Demo()
 
 
 def main():
     XmlLib().test_recurse_sections()  # recursively list sections
 
 
 #    test_data_table()
```

### Comparing `amilib-0.1.1/setup.py` & `amilib-0.1.1a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
  'scikit-learn',
 
 ]
 
 setup(
     name='amilib',
     url='https://github.com/petermr/amilib',
-    version='0.1.1',
+    version='0.1.1a',
     description='document download, cleaning, management',
     long_description_content_type='text/markdown',
     long_description=readme,
     author="Peter Murray-Rust",
     author_email='petermurrayrust@googlemail.com',
     license='Apache2',
     install_requires=requirements,
```

### Comparing `amilib-0.1.1/test/test_all.py` & `amilib-0.1.1a0/test/test_all.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.1/test/test_file.py` & `amilib-0.1.1a0/test/test_file.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.1/test/test_headless.py` & `amilib-0.1.1a0/test/test_headless.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.1/test/test_html.py` & `amilib-0.1.1a0/test/test_html.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.1/test/test_nlp.py` & `amilib-0.1.1a0/test/test_nlp.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.1/test/test_pdf.py` & `amilib-0.1.1a0/test/test_pdf.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.1/test/test_stat.py` & `amilib-0.1.1a0/test/test_stat.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.1/test/test_svg.py` & `amilib-0.1.1a0/test/test_svg.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.1/test/test_util.py` & `amilib-0.1.1a0/test/test_util.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.1/test/test_wikidata.py` & `amilib-0.1.1a0/test/test_wikidata.py`

 * *Files identical despite different names*

### Comparing `amilib-0.1.1/test/test_xml.py` & `amilib-0.1.1a0/test/test_xml.py`

 * *Files identical despite different names*

