# Comparing `tmp/urlgenie-1.0.0.tar.gz` & `tmp/urlgenie-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "urlgenie-1.0.0.tar", last modified: Sat May 18 10:00:51 2024, max compression
+gzip compressed data, was "urlgenie-1.1.0.tar", last modified: Sun May 19 18:02:06 2024, max compression
```

## Comparing `urlgenie-1.0.0.tar` & `urlgenie-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 10:00:51.423606 urlgenie-1.0.0/
--rw-rw-rw-   0        0        0     1088 2024-05-18 06:21:54.000000 urlgenie-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1625 2024-05-18 10:00:51.423606 urlgenie-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      179 2024-05-18 09:59:47.000000 urlgenie-1.0.0/README.md
--rw-rw-rw-   0        0        0       86 2024-05-18 10:00:51.431281 urlgenie-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     2027 2024-05-18 09:59:33.000000 urlgenie-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-18 10:00:51.369050 urlgenie-1.0.0/urlgenie/
--rw-rw-rw-   0        0        0       90 2024-05-18 06:31:13.000000 urlgenie-1.0.0/urlgenie/__init__.py
--rw-rw-rw-   0        0        0     6157 2024-05-18 06:17:28.000000 urlgenie-1.0.0/urlgenie/social_gens.py
--rw-rw-rw-   0        0        0     8315 2024-05-18 06:17:28.000000 urlgenie-1.0.0/urlgenie/url_gen.py
-drwxrwxrwx   0        0        0        0 2024-05-18 10:00:51.423606 urlgenie-1.0.0/urlgenie.egg-info/
--rw-rw-rw-   0        0        0     1625 2024-05-18 10:00:51.000000 urlgenie-1.0.0/urlgenie.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2024-05-18 10:00:51.000000 urlgenie-1.0.0/urlgenie.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 10:00:51.000000 urlgenie-1.0.0/urlgenie.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-18 10:00:51.000000 urlgenie-1.0.0/urlgenie.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-18 10:00:51.000000 urlgenie-1.0.0/urlgenie.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-19 18:02:06.607731 urlgenie-1.1.0/
+-rw-rw-rw-   0        0        0     1088 2024-05-18 06:21:54.000000 urlgenie-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     9334 2024-05-19 18:02:06.607731 urlgenie-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7964 2024-05-19 17:57:10.000000 urlgenie-1.1.0/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-19 18:02:06.611471 urlgenie-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1945 2024-05-19 17:58:36.000000 urlgenie-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 18:02:06.547512 urlgenie-1.1.0/urlgenie/
+-rw-rw-rw-   0        0        0       85 2024-05-19 17:58:42.000000 urlgenie-1.1.0/urlgenie/__init__.py
+-rw-rw-rw-   0        0        0     2595 2024-05-18 17:09:45.000000 urlgenie-1.1.0/urlgenie/constants.py
+-rw-rw-rw-   0        0        0     6157 2024-05-18 06:17:28.000000 urlgenie-1.1.0/urlgenie/social_gens.py
+-rw-rw-rw-   0        0        0    11801 2024-05-19 09:01:26.000000 urlgenie-1.1.0/urlgenie/urlgenie.py
+drwxrwxrwx   0        0        0        0 2024-05-19 18:02:06.607157 urlgenie-1.1.0/urlgenie.egg-info/
+-rw-rw-rw-   0        0        0     9334 2024-05-19 18:02:06.000000 urlgenie-1.1.0/urlgenie.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2024-05-19 18:02:06.000000 urlgenie-1.1.0/urlgenie.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 18:02:06.000000 urlgenie-1.1.0/urlgenie.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-19 18:02:06.000000 urlgenie-1.1.0/urlgenie.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-19 18:02:06.000000 urlgenie-1.1.0/urlgenie.egg-info/top_level.txt
```

### Comparing `urlgenie-1.0.0/LICENSE` & `urlgenie-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `urlgenie-1.0.0/setup.py` & `urlgenie-1.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,26 +8,25 @@
         return long_description
     except:
         return None
 
 setup(
     license = "MIT",
     name = "urlgenie",
-    version = "1.0.0",
+    version = "1.1.0",
     packages = ["urlgenie"],
     author = "Ahmed Khatib",
     python_requires = ">=3.7",
     maintainer = "Ahmed Khatib",
     install_requires = ["tldextract"],
     long_description = get_description(),
     author_email = "ahmedkhatib99@gmail.com",
     maintainer_email = "ahmedkhatib99@gmail.com",
     long_description_content_type = "text/markdown",
-    download_url = "https://github.com/bluestero/urlgenie/archive/refs/tags/1.0.0.tar.gz",
-    description = "Tool to make URL extraction, generalization, validation, and filtration easy.",
+    description = "Python package to make URL extraction, generalization, validation, and filtration easy.",
     project_urls={
         "Documentation": "https://github.com/bluestero/urlgenie/blob/main/README.md",
         "Source": "https://github.com/bluestero/urlgenie",
         "Tracker": "https://github.com/bluestero/urlgenie/issues",
     },
     keywords = [
         "url-parsing",
```

### Comparing `urlgenie-1.0.0/urlgenie/social_gens.py` & `urlgenie-1.1.0/urlgenie/social_gens.py`

 * *Files identical despite different names*

