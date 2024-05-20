# Comparing `tmp/urlgenie-1.1.1.tar.gz` & `tmp/urlgenie-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "urlgenie-1.1.1.tar", last modified: Mon May 20 09:17:08 2024, max compression
+gzip compressed data, was "urlgenie-1.1.2.tar", last modified: Mon May 20 09:21:55 2024, max compression
```

## Comparing `urlgenie-1.1.1.tar` & `urlgenie-1.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 09:17:08.689791 urlgenie-1.1.1/
--rw-rw-rw-   0        0        0     1088 2024-05-18 06:21:54.000000 urlgenie-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     9387 2024-05-20 09:17:08.689791 urlgenie-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     8017 2024-05-20 09:02:54.000000 urlgenie-1.1.1/README.md
--rw-rw-rw-   0        0        0       86 2024-05-20 09:17:08.692890 urlgenie-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1945 2024-05-20 09:16:35.000000 urlgenie-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-20 09:17:08.644557 urlgenie-1.1.1/urlgenie/
--rw-rw-rw-   0        0        0       85 2024-05-20 09:16:47.000000 urlgenie-1.1.1/urlgenie/__init__.py
--rw-rw-rw-   0        0        0     2595 2024-05-18 17:09:45.000000 urlgenie-1.1.1/urlgenie/constants.py
--rw-rw-rw-   0        0        0     6157 2024-05-18 06:17:28.000000 urlgenie-1.1.1/urlgenie/social_gens.py
--rw-rw-rw-   0        0        0    11801 2024-05-19 09:01:26.000000 urlgenie-1.1.1/urlgenie/urlgenie.py
-drwxrwxrwx   0        0        0        0 2024-05-20 09:17:08.687472 urlgenie-1.1.1/urlgenie.egg-info/
--rw-rw-rw-   0        0        0     9387 2024-05-20 09:17:08.000000 urlgenie-1.1.1/urlgenie.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2024-05-20 09:17:08.000000 urlgenie-1.1.1/urlgenie.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 09:17:08.000000 urlgenie-1.1.1/urlgenie.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-20 09:17:08.000000 urlgenie-1.1.1/urlgenie.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-20 09:17:08.000000 urlgenie-1.1.1/urlgenie.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-20 09:21:55.355546 urlgenie-1.1.2/
+-rw-rw-rw-   0        0        0     1088 2024-05-18 06:21:54.000000 urlgenie-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     9445 2024-05-20 09:21:55.355546 urlgenie-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8075 2024-05-20 09:18:41.000000 urlgenie-1.1.2/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-20 09:21:55.358577 urlgenie-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1945 2024-05-20 09:21:07.000000 urlgenie-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:21:55.321162 urlgenie-1.1.2/urlgenie/
+-rw-rw-rw-   0        0        0       85 2024-05-20 09:21:07.000000 urlgenie-1.1.2/urlgenie/__init__.py
+-rw-rw-rw-   0        0        0     2595 2024-05-18 17:09:45.000000 urlgenie-1.1.2/urlgenie/constants.py
+-rw-rw-rw-   0        0        0     6157 2024-05-18 06:17:28.000000 urlgenie-1.1.2/urlgenie/social_gens.py
+-rw-rw-rw-   0        0        0    11801 2024-05-19 09:01:26.000000 urlgenie-1.1.2/urlgenie/urlgenie.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:21:55.354619 urlgenie-1.1.2/urlgenie.egg-info/
+-rw-rw-rw-   0        0        0     9445 2024-05-20 09:21:55.000000 urlgenie-1.1.2/urlgenie.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2024-05-20 09:21:55.000000 urlgenie-1.1.2/urlgenie.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 09:21:55.000000 urlgenie-1.1.2/urlgenie.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-20 09:21:55.000000 urlgenie-1.1.2/urlgenie.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-20 09:21:55.000000 urlgenie-1.1.2/urlgenie.egg-info/top_level.txt
```

### Comparing `urlgenie-1.1.1/LICENSE` & `urlgenie-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `urlgenie-1.1.1/PKG-INFO` & `urlgenie-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urlgenie
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python package to make URL extraction, generalization, validation, and filtration easy.
 Author: Ahmed Khatib
 Author-email: ahmedkhatib99@gmail.com
 Maintainer: Ahmed Khatib
 Maintainer-email: ahmedkhatib99@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/bluestero/urlgenie/blob/main/README.md
@@ -24,15 +24,15 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align = "center">
-<img src = "./images/mascot.png" alt = "urlgenie" /><div align = "center" style = "margin-top: 0;">
+<img src = "https://raw.githubusercontent.com/bluestero/urlgenie/master/images/mascot.png" alt = "urlgenie" /><div align = "center" style = "margin-top: 0;">
 <h1>🧞 URL Genie 🧞</h1>
 </div>
 <h3 align="center">
   URL extraction, generalization, validation, and filtration made easy.
 </h3>
 
 ## 🚀 About URL Genie
```

### Comparing `urlgenie-1.1.1/README.md` & `urlgenie-1.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <p align = "center">
-<img src = "./images/mascot.png" alt = "urlgenie" /><div align = "center" style = "margin-top: 0;">
+<img src = "https://raw.githubusercontent.com/bluestero/urlgenie/master/images/mascot.png" alt = "urlgenie" /><div align = "center" style = "margin-top: 0;">
 <h1>🧞 URL Genie 🧞</h1>
 </div>
 <h3 align="center">
   URL extraction, generalization, validation, and filtration made easy.
 </h3>
 
 ## 🚀 About URL Genie
```

### Comparing `urlgenie-1.1.1/setup.py` & `urlgenie-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         return long_description
     except:
         return None
 
 setup(
     license = "MIT",
     name = "urlgenie",
-    version = "1.1.1",
+    version = "1.1.2",
     packages = ["urlgenie"],
     author = "Ahmed Khatib",
     python_requires = ">=3.7",
     maintainer = "Ahmed Khatib",
     install_requires = ["tldextract"],
     long_description = get_description(),
     author_email = "ahmedkhatib99@gmail.com",
```

### Comparing `urlgenie-1.1.1/urlgenie/constants.py` & `urlgenie-1.1.2/urlgenie/constants.py`

 * *Files identical despite different names*

### Comparing `urlgenie-1.1.1/urlgenie/social_gens.py` & `urlgenie-1.1.2/urlgenie/social_gens.py`

 * *Files identical despite different names*

### Comparing `urlgenie-1.1.1/urlgenie/urlgenie.py` & `urlgenie-1.1.2/urlgenie/urlgenie.py`

 * *Files identical despite different names*

### Comparing `urlgenie-1.1.1/urlgenie.egg-info/PKG-INFO` & `urlgenie-1.1.2/urlgenie.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urlgenie
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python package to make URL extraction, generalization, validation, and filtration easy.
 Author: Ahmed Khatib
 Author-email: ahmedkhatib99@gmail.com
 Maintainer: Ahmed Khatib
 Maintainer-email: ahmedkhatib99@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/bluestero/urlgenie/blob/main/README.md
@@ -24,15 +24,15 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align = "center">
-<img src = "./images/mascot.png" alt = "urlgenie" /><div align = "center" style = "margin-top: 0;">
+<img src = "https://raw.githubusercontent.com/bluestero/urlgenie/master/images/mascot.png" alt = "urlgenie" /><div align = "center" style = "margin-top: 0;">
 <h1>🧞 URL Genie 🧞</h1>
 </div>
 <h3 align="center">
   URL extraction, generalization, validation, and filtration made easy.
 </h3>
 
 ## 🚀 About URL Genie
```

