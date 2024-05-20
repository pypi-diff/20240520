# Comparing `tmp/spam_util-0.51.tar.gz` & `tmp/spam_util-0.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spam_util-0.51.tar", last modified: Mon Apr 22 21:16:29 2024, max compression
+gzip compressed data, was "spam_util-0.52.tar", last modified: Mon May 20 21:13:15 2024, max compression
```

## Comparing `spam_util-0.51.tar` & `spam_util-0.52.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 mgmiller  (1000) mgmiller  (1000)        0 2024-04-22 21:16:29.993878 spam_util-0.51/
--rw-r--r--   0 mgmiller  (1000) mgmiller  (1000)    35146 2024-04-22 20:50:13.000000 spam_util-0.51/LICENSE
--rw-r--r--   0 mgmiller  (1000) mgmiller  (1000)     2068 2024-04-22 21:16:29.993878 spam_util-0.51/PKG-INFO
--rw-r--r--   0 mgmiller  (1000) mgmiller  (1000)     1294 2024-04-22 21:09:45.000000 spam_util-0.51/README.md
--rw-r--r--   0 mgmiller  (1000) mgmiller  (1000)      969 2024-04-22 21:15:49.000000 spam_util-0.51/pyproject.toml
--rw-r--r--   0 mgmiller  (1000) mgmiller  (1000)       38 2024-04-22 21:16:29.993878 spam_util-0.51/setup.cfg
--rwxr-xr-x   0 mgmiller  (1000) mgmiller  (1000)     4582 2024-04-22 21:14:53.000000 spam_util-0.51/spam
-drwxr-xr-x   0 mgmiller  (1000) mgmiller  (1000)        0 2024-04-22 21:16:29.992878 spam_util-0.51/spam_util.egg-info/
--rw-r--r--   0 mgmiller  (1000) mgmiller  (1000)     2068 2024-04-22 21:16:29.000000 spam_util-0.51/spam_util.egg-info/PKG-INFO
--rw-r--r--   0 mgmiller  (1000) mgmiller  (1000)      169 2024-04-22 21:16:29.000000 spam_util-0.51/spam_util.egg-info/SOURCES.txt
--rw-r--r--   0 mgmiller  (1000) mgmiller  (1000)        1 2024-04-22 21:16:29.000000 spam_util-0.51/spam_util.egg-info/dependency_links.txt
--rw-r--r--   0 mgmiller  (1000) mgmiller  (1000)        1 2024-04-22 21:16:29.000000 spam_util-0.51/spam_util.egg-info/top_level.txt
+drwxr-xr-x   0 mgmiller  (1000) mgmiller  (1000)        0 2024-05-20 21:13:15.075399 spam_util-0.52/
+-rw-r--r--   0 mgmiller  (1000) mgmiller  (1000)    35146 2024-04-18 02:22:15.000000 spam_util-0.52/LICENSE
+-rw-r--r--   0 mgmiller  (1000) mgmiller  (1000)     2067 2024-05-20 21:13:15.074399 spam_util-0.52/PKG-INFO
+-rw-r--r--   0 mgmiller  (1000) mgmiller  (1000)     1293 2024-04-23 03:02:40.000000 spam_util-0.52/README.md
+-rw-r--r--   0 mgmiller  (1000) mgmiller  (1000)      969 2024-05-20 21:10:32.000000 spam_util-0.52/pyproject.toml
+-rw-r--r--   0 mgmiller  (1000) mgmiller  (1000)       38 2024-05-20 21:13:15.075399 spam_util-0.52/setup.cfg
+-rwxr-xr-x   0 mgmiller  (1000) mgmiller  (1000)     5545 2024-05-20 21:10:37.000000 spam_util-0.52/spam
+drwxr-xr-x   0 mgmiller  (1000) mgmiller  (1000)        0 2024-05-20 21:13:15.074399 spam_util-0.52/spam_util.egg-info/
+-rw-r--r--   0 mgmiller  (1000) mgmiller  (1000)     2067 2024-05-20 21:13:15.000000 spam_util-0.52/spam_util.egg-info/PKG-INFO
+-rw-r--r--   0 mgmiller  (1000) mgmiller  (1000)      169 2024-05-20 21:13:15.000000 spam_util-0.52/spam_util.egg-info/SOURCES.txt
+-rw-r--r--   0 mgmiller  (1000) mgmiller  (1000)        1 2024-05-20 21:13:15.000000 spam_util-0.52/spam_util.egg-info/dependency_links.txt
+-rw-r--r--   0 mgmiller  (1000) mgmiller  (1000)        1 2024-05-20 21:13:15.000000 spam_util-0.52/spam_util.egg-info/top_level.txt
```

### Comparing `spam_util-0.51/LICENSE` & `spam_util-0.52/LICENSE`

 * *Files identical despite different names*

### Comparing `spam_util-0.51/PKG-INFO` & `spam_util-0.52/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spam-util
-Version: 0.51
+Version: 0.52
 Summary: A Software PAckage Manager interface utility for Linux.
 Author-email: Foo McBar <mixmastamyk@bitbucket.org>
 Project-URL: Homepage, https://bitbucket.org/mixmastamyk/spam/
 Project-URL: Issues, https://bitbucket.org/mixmastamyk/spam/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -16,16 +16,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # SPAM - A <u>S</u>oftware <u>PA</u>ckage <u>M</u>anager #
 
-To be honest,
-it's not really a package manager,
+To be honest it's not *really* a package manager,
 but merely a wrapper that presents a uniform command-line interface
 across Linux distros.
 
 
 ## Usage & Features ##
 
 👉  Easy to type and use every day.
@@ -51,15 +50,15 @@
 👉  It knows when to invoke sudo,
 so you rarely need to worry about it.
 
 👉  It prints the command it runs,
 so you can learn how to do it on a package manager you may not be as familiar
 with.
 Also, if it wasn't able to do what you want,
-it is easy to recover.
+it is easy to tweak.
 
 
 ## Support ##
 
 Currently supports Debian `apt` and Fedora `dnf`,
 with hopefully more to come as time allows.
```

### Comparing `spam_util-0.51/README.md` & `spam_util-0.52/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 
 # SPAM - A <u>S</u>oftware <u>PA</u>ckage <u>M</u>anager #
 
-To be honest,
-it's not really a package manager,
+To be honest it's not *really* a package manager,
 but merely a wrapper that presents a uniform command-line interface
 across Linux distros.
 
 
 ## Usage & Features ##
 
 👉  Easy to type and use every day.
@@ -32,15 +31,15 @@
 👉  It knows when to invoke sudo,
 so you rarely need to worry about it.
 
 👉  It prints the command it runs,
 so you can learn how to do it on a package manager you may not be as familiar
 with.
 Also, if it wasn't able to do what you want,
-it is easy to recover.
+it is easy to tweak.
 
 
 ## Support ##
 
 Currently supports Debian `apt` and Fedora `dnf`,
 with hopefully more to come as time allows.
```

### Comparing `spam_util-0.51/pyproject.toml` & `spam_util-0.52/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "spam-util"
-version = "0.51"
+version = "0.52"
 authors = [
   { name="Foo McBar", email="mixmastamyk@bitbucket.org" },
 ]
 description = "A Software PAckage Manager interface utility for Linux."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `spam_util-0.51/spam_util.egg-info/PKG-INFO` & `spam_util-0.52/spam_util.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spam-util
-Version: 0.51
+Version: 0.52
 Summary: A Software PAckage Manager interface utility for Linux.
 Author-email: Foo McBar <mixmastamyk@bitbucket.org>
 Project-URL: Homepage, https://bitbucket.org/mixmastamyk/spam/
 Project-URL: Issues, https://bitbucket.org/mixmastamyk/spam/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -16,16 +16,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # SPAM - A <u>S</u>oftware <u>PA</u>ckage <u>M</u>anager #
 
-To be honest,
-it's not really a package manager,
+To be honest it's not *really* a package manager,
 but merely a wrapper that presents a uniform command-line interface
 across Linux distros.
 
 
 ## Usage & Features ##
 
 👉  Easy to type and use every day.
@@ -51,15 +50,15 @@
 👉  It knows when to invoke sudo,
 so you rarely need to worry about it.
 
 👉  It prints the command it runs,
 so you can learn how to do it on a package manager you may not be as familiar
 with.
 Also, if it wasn't able to do what you want,
-it is easy to recover.
+it is easy to tweak.
 
 
 ## Support ##
 
 Currently supports Debian `apt` and Fedora `dnf`,
 with hopefully more to come as time allows.
```

