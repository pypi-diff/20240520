# Comparing `tmp/urlgenie-1.1.0.tar.gz` & `tmp/urlgenie-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "urlgenie-1.1.0.tar", last modified: Sun May 19 18:02:06 2024, max compression
+gzip compressed data, was "urlgenie-1.1.1.tar", last modified: Mon May 20 09:17:08 2024, max compression
```

## Comparing `urlgenie-1.1.0.tar` & `urlgenie-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 18:02:06.607731 urlgenie-1.1.0/
--rw-rw-rw-   0        0        0     1088 2024-05-18 06:21:54.000000 urlgenie-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     9334 2024-05-19 18:02:06.607731 urlgenie-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     7964 2024-05-19 17:57:10.000000 urlgenie-1.1.0/README.md
--rw-rw-rw-   0        0        0       86 2024-05-19 18:02:06.611471 urlgenie-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1945 2024-05-19 17:58:36.000000 urlgenie-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-19 18:02:06.547512 urlgenie-1.1.0/urlgenie/
--rw-rw-rw-   0        0        0       85 2024-05-19 17:58:42.000000 urlgenie-1.1.0/urlgenie/__init__.py
--rw-rw-rw-   0        0        0     2595 2024-05-18 17:09:45.000000 urlgenie-1.1.0/urlgenie/constants.py
--rw-rw-rw-   0        0        0     6157 2024-05-18 06:17:28.000000 urlgenie-1.1.0/urlgenie/social_gens.py
--rw-rw-rw-   0        0        0    11801 2024-05-19 09:01:26.000000 urlgenie-1.1.0/urlgenie/urlgenie.py
-drwxrwxrwx   0        0        0        0 2024-05-19 18:02:06.607157 urlgenie-1.1.0/urlgenie.egg-info/
--rw-rw-rw-   0        0        0     9334 2024-05-19 18:02:06.000000 urlgenie-1.1.0/urlgenie.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2024-05-19 18:02:06.000000 urlgenie-1.1.0/urlgenie.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 18:02:06.000000 urlgenie-1.1.0/urlgenie.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-19 18:02:06.000000 urlgenie-1.1.0/urlgenie.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-19 18:02:06.000000 urlgenie-1.1.0/urlgenie.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-20 09:17:08.689791 urlgenie-1.1.1/
+-rw-rw-rw-   0        0        0     1088 2024-05-18 06:21:54.000000 urlgenie-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     9387 2024-05-20 09:17:08.689791 urlgenie-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8017 2024-05-20 09:02:54.000000 urlgenie-1.1.1/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-20 09:17:08.692890 urlgenie-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1945 2024-05-20 09:16:35.000000 urlgenie-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:17:08.644557 urlgenie-1.1.1/urlgenie/
+-rw-rw-rw-   0        0        0       85 2024-05-20 09:16:47.000000 urlgenie-1.1.1/urlgenie/__init__.py
+-rw-rw-rw-   0        0        0     2595 2024-05-18 17:09:45.000000 urlgenie-1.1.1/urlgenie/constants.py
+-rw-rw-rw-   0        0        0     6157 2024-05-18 06:17:28.000000 urlgenie-1.1.1/urlgenie/social_gens.py
+-rw-rw-rw-   0        0        0    11801 2024-05-19 09:01:26.000000 urlgenie-1.1.1/urlgenie/urlgenie.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:17:08.687472 urlgenie-1.1.1/urlgenie.egg-info/
+-rw-rw-rw-   0        0        0     9387 2024-05-20 09:17:08.000000 urlgenie-1.1.1/urlgenie.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2024-05-20 09:17:08.000000 urlgenie-1.1.1/urlgenie.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 09:17:08.000000 urlgenie-1.1.1/urlgenie.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-20 09:17:08.000000 urlgenie-1.1.1/urlgenie.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-20 09:17:08.000000 urlgenie-1.1.1/urlgenie.egg-info/top_level.txt
```

### Comparing `urlgenie-1.1.0/LICENSE` & `urlgenie-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `urlgenie-1.1.0/PKG-INFO` & `urlgenie-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urlgenie
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python package to make URL extraction, generalization, validation, and filtration easy.
 Author: Ahmed Khatib
 Author-email: ahmedkhatib99@gmail.com
 Maintainer: Ahmed Khatib
 Maintainer-email: ahmedkhatib99@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/bluestero/urlgenie/blob/main/README.md
@@ -38,17 +38,18 @@
 ## 🚀 About URL Genie
 It is a python package based on research involving over 2 million URLs, designed to handle URLs in a flexible manner for data-driven projects.
 
 ## 💡 How it works
 It checks the given URL input, validates it against the URL regex, identifies each component of the URL and processes it according to the set flags.
 
 ## ✨ Features
-- Handle both encoded and decoded URLs.
+- Handles both encoded and decoded URLs.
+- Handles comma separated URLs using recursion.
 - Filter out valid, invalid URLs and also bad socials with ease.
-- Extract Email and Socials from a given text and validate them.
+- Email and Socials extraction from a given text and validate them.
 - URL validation using regex and over 1400 TLDs (off by default).
 - Duplicate reduction by minimizing the general and social URL patterns.
 - Domain mismatch by just extracting the domain along with the TLD and match against the email domain.
 - Researched and refined social regexes to recognize different social patterns and generalizes them to the standardized format.
 
 ## ⚙️ Installation
 First things first, you need to install URL Genie by running the following command in your terminal:
```

### Comparing `urlgenie-1.1.0/README.md` & `urlgenie-1.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 ## 🚀 About URL Genie
 It is a python package based on research involving over 2 million URLs, designed to handle URLs in a flexible manner for data-driven projects.
 
 ## 💡 How it works
 It checks the given URL input, validates it against the URL regex, identifies each component of the URL and processes it according to the set flags.
 
 ## ✨ Features
-- Handle both encoded and decoded URLs.
+- Handles both encoded and decoded URLs.
+- Handles comma separated URLs using recursion.
 - Filter out valid, invalid URLs and also bad socials with ease.
-- Extract Email and Socials from a given text and validate them.
+- Email and Socials extraction from a given text and validate them.
 - URL validation using regex and over 1400 TLDs (off by default).
 - Duplicate reduction by minimizing the general and social URL patterns.
 - Domain mismatch by just extracting the domain along with the TLD and match against the email domain.
 - Researched and refined social regexes to recognize different social patterns and generalizes them to the standardized format.
 
 ## ⚙️ Installation
 First things first, you need to install URL Genie by running the following command in your terminal:
```

### Comparing `urlgenie-1.1.0/setup.py` & `urlgenie-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         return long_description
     except:
         return None
 
 setup(
     license = "MIT",
     name = "urlgenie",
-    version = "1.1.0",
+    version = "1.1.1",
     packages = ["urlgenie"],
     author = "Ahmed Khatib",
     python_requires = ">=3.7",
     maintainer = "Ahmed Khatib",
     install_requires = ["tldextract"],
     long_description = get_description(),
     author_email = "ahmedkhatib99@gmail.com",
```

### Comparing `urlgenie-1.1.0/urlgenie/constants.py` & `urlgenie-1.1.1/urlgenie/constants.py`

 * *Files identical despite different names*

### Comparing `urlgenie-1.1.0/urlgenie/social_gens.py` & `urlgenie-1.1.1/urlgenie/social_gens.py`

 * *Files identical despite different names*

### Comparing `urlgenie-1.1.0/urlgenie/urlgenie.py` & `urlgenie-1.1.1/urlgenie/urlgenie.py`

 * *Files identical despite different names*

### Comparing `urlgenie-1.1.0/urlgenie.egg-info/PKG-INFO` & `urlgenie-1.1.1/urlgenie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urlgenie
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python package to make URL extraction, generalization, validation, and filtration easy.
 Author: Ahmed Khatib
 Author-email: ahmedkhatib99@gmail.com
 Maintainer: Ahmed Khatib
 Maintainer-email: ahmedkhatib99@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/bluestero/urlgenie/blob/main/README.md
@@ -38,17 +38,18 @@
 ## 🚀 About URL Genie
 It is a python package based on research involving over 2 million URLs, designed to handle URLs in a flexible manner for data-driven projects.
 
 ## 💡 How it works
 It checks the given URL input, validates it against the URL regex, identifies each component of the URL and processes it according to the set flags.
 
 ## ✨ Features
-- Handle both encoded and decoded URLs.
+- Handles both encoded and decoded URLs.
+- Handles comma separated URLs using recursion.
 - Filter out valid, invalid URLs and also bad socials with ease.
-- Extract Email and Socials from a given text and validate them.
+- Email and Socials extraction from a given text and validate them.
 - URL validation using regex and over 1400 TLDs (off by default).
 - Duplicate reduction by minimizing the general and social URL patterns.
 - Domain mismatch by just extracting the domain along with the TLD and match against the email domain.
 - Researched and refined social regexes to recognize different social patterns and generalizes them to the standardized format.
 
 ## ⚙️ Installation
 First things first, you need to install URL Genie by running the following command in your terminal:
```

