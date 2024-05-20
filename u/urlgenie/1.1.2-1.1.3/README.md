# Comparing `tmp/urlgenie-1.1.2.tar.gz` & `tmp/urlgenie-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "urlgenie-1.1.2.tar", last modified: Mon May 20 09:21:55 2024, max compression
+gzip compressed data, was "urlgenie-1.1.3.tar", last modified: Mon May 20 18:08:09 2024, max compression
```

## Comparing `urlgenie-1.1.2.tar` & `urlgenie-1.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 09:21:55.355546 urlgenie-1.1.2/
--rw-rw-rw-   0        0        0     1088 2024-05-18 06:21:54.000000 urlgenie-1.1.2/LICENSE
--rw-rw-rw-   0        0        0     9445 2024-05-20 09:21:55.355546 urlgenie-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     8075 2024-05-20 09:18:41.000000 urlgenie-1.1.2/README.md
--rw-rw-rw-   0        0        0       86 2024-05-20 09:21:55.358577 urlgenie-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1945 2024-05-20 09:21:07.000000 urlgenie-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-20 09:21:55.321162 urlgenie-1.1.2/urlgenie/
--rw-rw-rw-   0        0        0       85 2024-05-20 09:21:07.000000 urlgenie-1.1.2/urlgenie/__init__.py
--rw-rw-rw-   0        0        0     2595 2024-05-18 17:09:45.000000 urlgenie-1.1.2/urlgenie/constants.py
--rw-rw-rw-   0        0        0     6157 2024-05-18 06:17:28.000000 urlgenie-1.1.2/urlgenie/social_gens.py
--rw-rw-rw-   0        0        0    11801 2024-05-19 09:01:26.000000 urlgenie-1.1.2/urlgenie/urlgenie.py
-drwxrwxrwx   0        0        0        0 2024-05-20 09:21:55.354619 urlgenie-1.1.2/urlgenie.egg-info/
--rw-rw-rw-   0        0        0     9445 2024-05-20 09:21:55.000000 urlgenie-1.1.2/urlgenie.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2024-05-20 09:21:55.000000 urlgenie-1.1.2/urlgenie.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 09:21:55.000000 urlgenie-1.1.2/urlgenie.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-20 09:21:55.000000 urlgenie-1.1.2/urlgenie.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-20 09:21:55.000000 urlgenie-1.1.2/urlgenie.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-20 18:08:09.157549 urlgenie-1.1.3/
+-rw-rw-rw-   0        0        0     1088 2024-05-20 16:51:49.000000 urlgenie-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0     9472 2024-05-20 18:08:09.157549 urlgenie-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     8075 2024-05-20 16:51:49.000000 urlgenie-1.1.3/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-20 18:08:09.158547 urlgenie-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1945 2024-05-20 16:55:09.000000 urlgenie-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 18:08:09.150549 urlgenie-1.1.3/urlgenie/
+-rw-rw-rw-   0        0        0      144 2024-05-20 16:56:08.000000 urlgenie-1.1.3/urlgenie/__init__.py
+-rw-rw-rw-   0        0        0     2755 2024-05-20 16:55:42.000000 urlgenie-1.1.3/urlgenie/constants.py
+-rw-rw-rw-   0        0        0     6157 2024-05-20 16:51:49.000000 urlgenie-1.1.3/urlgenie/social_gens.py
+-rw-rw-rw-   0        0        0    11841 2024-05-20 16:53:17.000000 urlgenie-1.1.3/urlgenie/urlgenie.py
+drwxrwxrwx   0        0        0        0 2024-05-20 18:08:09.156550 urlgenie-1.1.3/urlgenie.egg-info/
+-rw-rw-rw-   0        0        0     9472 2024-05-20 18:08:09.000000 urlgenie-1.1.3/urlgenie.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2024-05-20 18:08:09.000000 urlgenie-1.1.3/urlgenie.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 18:08:09.000000 urlgenie-1.1.3/urlgenie.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-20 18:08:09.000000 urlgenie-1.1.3/urlgenie.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-20 18:08:09.000000 urlgenie-1.1.3/urlgenie.egg-info/top_level.txt
```

### Comparing `urlgenie-1.1.2/LICENSE` & `urlgenie-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `urlgenie-1.1.2/PKG-INFO` & `urlgenie-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urlgenie
-Version: 1.1.2
+Version: 1.1.3
 Summary: Python package to make URL extraction, generalization, validation, and filtration easy.
 Author: Ahmed Khatib
 Author-email: ahmedkhatib99@gmail.com
 Maintainer: Ahmed Khatib
 Maintainer-email: ahmedkhatib99@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/bluestero/urlgenie/blob/main/README.md
@@ -22,14 +22,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: tldextract
 
 <p align = "center">
 <img src = "https://raw.githubusercontent.com/bluestero/urlgenie/master/images/mascot.png" alt = "urlgenie" /><div align = "center" style = "margin-top: 0;">
 <h1>🧞 URL Genie 🧞</h1>
 </div>
 <h3 align="center">
   URL extraction, generalization, validation, and filtration made easy.
```

### Comparing `urlgenie-1.1.2/README.md` & `urlgenie-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `urlgenie-1.1.2/setup.py` & `urlgenie-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         return long_description
     except:
         return None
 
 setup(
     license = "MIT",
     name = "urlgenie",
-    version = "1.1.2",
+    version = "1.1.3",
     packages = ["urlgenie"],
     author = "Ahmed Khatib",
     python_requires = ">=3.7",
     maintainer = "Ahmed Khatib",
     install_requires = ["tldextract"],
     long_description = get_description(),
     author_email = "ahmedkhatib99@gmail.com",
```

### Comparing `urlgenie-1.1.2/urlgenie/constants.py` & `urlgenie-1.1.3/urlgenie/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,16 +26,22 @@
     r"(?:(?:in/|company/|showcase/|school/|companies/|profile/view\?id=)"
     r"(?:acwaa[a-z0-9_-]{34}|[a-z0-9&%.~_-]{2,200})|"
     r"pub/[a-z0-9&%.~_-]{2,150}/[a-z0-9]{1,3}/[a-z0-9]{1,3}/[a-z0-9]{1,3})", flags = re.IGNORECASE)
 instagram_handle = re.compile(
     r"instagram.com(?:.br|.au)?/+(?:accounts/login/\?next=/)"
     r"?[a-z0-9_.]{1,30}", flags = re.IGNORECASE)
 
-#-A pattern dictionary for easy access-#
-patterns_dict = {
+#-A pattern dictionary for href mailto and tel search-#
+primary_patterns = {
+    "phone": [phone_pattern_loose],
+    "email": [email_pattern],
+}
+
+#-A pattern dictionary for universal search-#
+generic_patterns = {
     "phone": [phone_pattern_strict],
     "email": [email_pattern],
     "instagram": [instagram_handle],
     "facebook": [facebook_id, facebook_handle],
     "linkedin": [linkedin_id, linkedin_handle],
     "twitter": [twitter_handle_1, twitter_handle_2],
 }
```

### Comparing `urlgenie-1.1.2/urlgenie/social_gens.py` & `urlgenie-1.1.3/urlgenie/social_gens.py`

 * *Files identical despite different names*

### Comparing `urlgenie-1.1.2/urlgenie/urlgenie.py` & `urlgenie-1.1.3/urlgenie/urlgenie.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,28 +147,28 @@
             url = url[:-1]
 
         #--Returning the decoded url in lower if lower flag is on--#
         return unquote(url).lower() if lower else unquote(url)
 
 
     #-Function to extract emails and socials from the given text-#
-    def extract_from_text(self, text: str) -> dict:
+    def extract_from_text(self, text: str, patterns_dict: dict = constants.generic_patterns) -> dict:
 
         #-Base object-#
         all_info = {
             "phone": set(),
             "email": set(),
             "facebook": set(),
             "twitter": set(),
             "linkedin": set(),
             "instagram": set(),
         }
 
         #-Iterating the dictionary containing different list of patterns-#
-        for column, patterns in constants.patterns_dict.items():
+        for column, patterns in patterns_dict.items():
 
             #-Iterating the pattern list-#
             for pattern in patterns:
 
                 #-Adding the regex matches in the all_info dict-#
                 all_info[column] = all_info[column].union(set(pattern.findall(text)))
```

### Comparing `urlgenie-1.1.2/urlgenie.egg-info/PKG-INFO` & `urlgenie-1.1.3/urlgenie.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urlgenie
-Version: 1.1.2
+Version: 1.1.3
 Summary: Python package to make URL extraction, generalization, validation, and filtration easy.
 Author: Ahmed Khatib
 Author-email: ahmedkhatib99@gmail.com
 Maintainer: Ahmed Khatib
 Maintainer-email: ahmedkhatib99@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/bluestero/urlgenie/blob/main/README.md
@@ -22,14 +22,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: tldextract
 
 <p align = "center">
 <img src = "https://raw.githubusercontent.com/bluestero/urlgenie/master/images/mascot.png" alt = "urlgenie" /><div align = "center" style = "margin-top: 0;">
 <h1>🧞 URL Genie 🧞</h1>
 </div>
 <h3 align="center">
   URL extraction, generalization, validation, and filtration made easy.
```

