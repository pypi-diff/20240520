# Comparing `tmp/microsoft-teams-0.1.0.tar.gz` & `tmp/microsoft-teams-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microsoft-teams-0.1.0.tar", last modified: Mon May 20 11:57:39 2024, max compression
+gzip compressed data, was "microsoft-teams-0.1.1.tar", last modified: Mon May 20 19:15:05 2024, max compression
```

## Comparing `microsoft-teams-0.1.0.tar` & `microsoft-teams-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 11:57:39.243045 microsoft-teams-0.1.0/
--rw-rw-rw-   0        0        0     1080 2024-05-20 11:53:56.000000 microsoft-teams-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      614 2024-05-20 11:57:39.241760 microsoft-teams-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-20 11:57:39.213158 microsoft-teams-0.1.0/microsoft_teams.egg-info/
--rw-rw-rw-   0        0        0      614 2024-05-20 11:57:39.000000 microsoft-teams-0.1.0/microsoft_teams.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2024-05-20 11:57:39.000000 microsoft-teams-0.1.0/microsoft_teams.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 11:57:39.000000 microsoft-teams-0.1.0/microsoft_teams.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-20 11:57:39.000000 microsoft-teams-0.1.0/microsoft_teams.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-20 11:57:39.000000 microsoft-teams-0.1.0/microsoft_teams.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-20 11:57:39.237715 microsoft-teams-0.1.0/modules/
--rw-rw-rw-   0        0        0       33 2024-05-20 11:51:10.000000 microsoft-teams-0.1.0/modules/__init__.py
--rw-rw-rw-   0        0        0     1119 2024-05-20 11:50:32.000000 microsoft-teams-0.1.0/modules/teams.py
--rw-rw-rw-   0        0        0       42 2024-05-20 11:57:39.243045 microsoft-teams-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      699 2024-05-20 11:52:04.000000 microsoft-teams-0.1.0/setup.py
+drwxrwxrwx   0 rashelle  (1000) rashelle  (1000)        0 2024-05-20 19:15:05.026016 microsoft-teams-0.1.1/
+-rwxrwxrwx   0 rashelle  (1000) rashelle  (1000)     1080 2024-05-20 11:53:56.000000 microsoft-teams-0.1.1/LICENSE
+-rwxrwxrwx   0 rashelle  (1000) rashelle  (1000)      631 2024-05-20 19:15:05.016033 microsoft-teams-0.1.1/PKG-INFO
+drwxrwxrwx   0 rashelle  (1000) rashelle  (1000)        0 2024-05-20 19:15:04.947488 microsoft-teams-0.1.1/microsoft_teams/
+-rwxrwxrwx   0 rashelle  (1000) rashelle  (1000)       33 2024-05-20 11:51:10.000000 microsoft-teams-0.1.1/microsoft_teams/__init__.py
+-rwxrwxrwx   0 rashelle  (1000) rashelle  (1000)     1119 2024-05-20 11:50:32.000000 microsoft-teams-0.1.1/microsoft_teams/teams.py
+drwxrwxrwx   0 rashelle  (1000) rashelle  (1000)        0 2024-05-20 19:15:05.012850 microsoft-teams-0.1.1/microsoft_teams.egg-info/
+-rwxrwxrwx   0 rashelle  (1000) rashelle  (1000)      631 2024-05-20 19:15:04.000000 microsoft-teams-0.1.1/microsoft_teams.egg-info/PKG-INFO
+-rwxrwxrwx   0 rashelle  (1000) rashelle  (1000)      263 2024-05-20 19:15:04.000000 microsoft-teams-0.1.1/microsoft_teams.egg-info/SOURCES.txt
+-rwxrwxrwx   0 rashelle  (1000) rashelle  (1000)        1 2024-05-20 19:15:04.000000 microsoft-teams-0.1.1/microsoft_teams.egg-info/dependency_links.txt
+-rwxrwxrwx   0 rashelle  (1000) rashelle  (1000)        9 2024-05-20 19:15:04.000000 microsoft-teams-0.1.1/microsoft_teams.egg-info/requires.txt
+-rwxrwxrwx   0 rashelle  (1000) rashelle  (1000)       16 2024-05-20 19:15:04.000000 microsoft-teams-0.1.1/microsoft_teams.egg-info/top_level.txt
+-rwxrwxrwx   0 rashelle  (1000) rashelle  (1000)       38 2024-05-20 19:15:05.026016 microsoft-teams-0.1.1/setup.cfg
+-rwxrwxrwx   0 rashelle  (1000) rashelle  (1000)      699 2024-05-20 19:12:05.000000 microsoft-teams-0.1.1/setup.py
```

### Comparing `microsoft-teams-0.1.0/LICENSE` & `microsoft-teams-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `microsoft-teams-0.1.0/modules/teams.py` & `microsoft-teams-0.1.1/microsoft_teams/teams.py`

 * *Files identical despite different names*

### Comparing `microsoft-teams-0.1.0/setup.py` & `microsoft-teams-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='microsoft-teams',
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(),
     install_requires=[
         'requests'
     ],
     author='Rashelle Woudberg',
     author_email='rashelle@al.co.za',
     description='A Python wrapper to send messages to Microsoft Teams.',
```

