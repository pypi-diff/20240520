# Comparing `tmp/nightingalejsonadapter-3.0.0.tar.gz` & `tmp/nightingalejsonadapter-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nightingalejsonadapter-3.0.0.tar", last modified: Thu May 16 15:29:32 2024, max compression
+gzip compressed data, was "nightingalejsonadapter-3.1.0.tar", last modified: Mon May 20 19:18:51 2024, max compression
```

## Comparing `nightingalejsonadapter-3.0.0.tar` & `nightingalejsonadapter-3.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 dtitestsystem  (1000) dtitestsystem  (1001)        0 2024-05-16 15:29:32.502914 nightingalejsonadapter-3.0.0/
--rw-r--r--   0 dtitestsystem  (1000) dtitestsystem  (1001)      270 2024-05-16 15:29:32.502914 nightingalejsonadapter-3.0.0/PKG-INFO
-drwxr-xr-x   0 dtitestsystem  (1000) dtitestsystem  (1001)        0 2024-05-16 15:29:32.502914 nightingalejsonadapter-3.0.0/nightingalejsonadapter/
--rw-r--r--   0 dtitestsystem  (1000) dtitestsystem  (1001)        0 2024-05-13 08:50:47.000000 nightingalejsonadapter-3.0.0/nightingalejsonadapter/__init__.py
--rw-r--r--   0 dtitestsystem  (1000) dtitestsystem  (1001)      452 2024-05-13 08:50:47.000000 nightingalejsonadapter-3.0.0/nightingalejsonadapter/intervention_adapter.py
--rw-r--r--   0 dtitestsystem  (1000) dtitestsystem  (1001)      700 2024-05-13 08:50:47.000000 nightingalejsonadapter-3.0.0/nightingalejsonadapter/patient_info_adapter.py
--rw-r--r--   0 dtitestsystem  (1000) dtitestsystem  (1001)      434 2024-05-13 08:50:47.000000 nightingalejsonadapter-3.0.0/nightingalejsonadapter/trigger_adapter.py
--rw-r--r--   0 dtitestsystem  (1000) dtitestsystem  (1001)      516 2024-05-13 08:50:47.000000 nightingalejsonadapter-3.0.0/nightingalejsonadapter/uuid_generator.py
--rw-r--r--   0 dtitestsystem  (1000) dtitestsystem  (1001)      776 2024-05-16 13:43:19.000000 nightingalejsonadapter-3.0.0/nightingalejsonadapter/vital_kafka_adapter.py
--rw-r--r--   0 dtitestsystem  (1000) dtitestsystem  (1001)      601 2024-05-13 08:50:47.000000 nightingalejsonadapter-3.0.0/nightingalejsonadapter/vitals_adapter.py
--rw-r--r--   0 dtitestsystem  (1000) dtitestsystem  (1001)     1019 2024-05-13 08:50:47.000000 nightingalejsonadapter-3.0.0/nightingalejsonadapter/vitals_response.py
-drwxr-xr-x   0 dtitestsystem  (1000) dtitestsystem  (1001)        0 2024-05-16 15:29:32.502914 nightingalejsonadapter-3.0.0/nightingalejsonadapter.egg-info/
--rw-r--r--   0 dtitestsystem  (1000) dtitestsystem  (1001)      270 2024-05-16 15:29:32.000000 nightingalejsonadapter-3.0.0/nightingalejsonadapter.egg-info/PKG-INFO
--rw-r--r--   0 dtitestsystem  (1000) dtitestsystem  (1001)      578 2024-05-16 15:29:32.000000 nightingalejsonadapter-3.0.0/nightingalejsonadapter.egg-info/SOURCES.txt
--rw-r--r--   0 dtitestsystem  (1000) dtitestsystem  (1001)        1 2024-05-16 15:29:32.000000 nightingalejsonadapter-3.0.0/nightingalejsonadapter.egg-info/dependency_links.txt
--rw-r--r--   0 dtitestsystem  (1000) dtitestsystem  (1001)        9 2024-05-16 15:29:32.000000 nightingalejsonadapter-3.0.0/nightingalejsonadapter.egg-info/requires.txt
--rw-r--r--   0 dtitestsystem  (1000) dtitestsystem  (1001)       23 2024-05-16 15:29:32.000000 nightingalejsonadapter-3.0.0/nightingalejsonadapter.egg-info/top_level.txt
--rw-r--r--   0 dtitestsystem  (1000) dtitestsystem  (1001)       38 2024-05-16 15:29:32.502914 nightingalejsonadapter-3.0.0/setup.cfg
--rw-r--r--   0 dtitestsystem  (1000) dtitestsystem  (1001)      774 2024-05-16 15:27:08.000000 nightingalejsonadapter-3.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 19:18:51.310287 nightingalejsonadapter-3.1.0/
+-rw-rw-rw-   0        0        0      280 2024-05-20 19:18:51.310287 nightingalejsonadapter-3.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-20 19:18:51.302286 nightingalejsonadapter-3.1.0/nightingalejsonadapter/
+-rw-rw-rw-   0        0        0        0 2024-05-03 01:38:22.000000 nightingalejsonadapter-3.1.0/nightingalejsonadapter/__init__.py
+-rw-rw-rw-   0        0        0      481 2024-05-03 01:38:22.000000 nightingalejsonadapter-3.1.0/nightingalejsonadapter/intervention_adapter.py
+-rw-rw-rw-   0        0        0      740 2024-05-03 14:52:50.000000 nightingalejsonadapter-3.1.0/nightingalejsonadapter/patient_info_adapter.py
+-rw-rw-rw-   0        0        0      455 2024-05-03 01:38:23.000000 nightingalejsonadapter-3.1.0/nightingalejsonadapter/trigger_adapter.py
+-rw-rw-rw-   0        0        0      533 2024-05-03 01:38:23.000000 nightingalejsonadapter-3.1.0/nightingalejsonadapter/uuid_generator.py
+-rw-rw-rw-   0        0        0      809 2024-05-20 09:22:44.000000 nightingalejsonadapter-3.1.0/nightingalejsonadapter/vital_kafka_adapter.py
+-rw-rw-rw-   0        0        0      629 2024-05-03 01:38:23.000000 nightingalejsonadapter-3.1.0/nightingalejsonadapter/vitals_adapter.py
+-rw-rw-rw-   0        0        0     1885 2024-05-20 19:15:09.000000 nightingalejsonadapter-3.1.0/nightingalejsonadapter/vitals_response.py
+drwxrwxrwx   0        0        0        0 2024-05-20 19:18:51.309287 nightingalejsonadapter-3.1.0/nightingalejsonadapter.egg-info/
+-rw-rw-rw-   0        0        0      280 2024-05-20 19:18:51.000000 nightingalejsonadapter-3.1.0/nightingalejsonadapter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      578 2024-05-20 19:18:51.000000 nightingalejsonadapter-3.1.0/nightingalejsonadapter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 19:18:51.000000 nightingalejsonadapter-3.1.0/nightingalejsonadapter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-20 19:18:51.000000 nightingalejsonadapter-3.1.0/nightingalejsonadapter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-20 19:18:51.000000 nightingalejsonadapter-3.1.0/nightingalejsonadapter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 19:18:51.311287 nightingalejsonadapter-3.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      797 2024-05-20 10:39:06.000000 nightingalejsonadapter-3.1.0/setup.py
```

### Comparing `nightingalejsonadapter-3.0.0/nightingalejsonadapter.egg-info/SOURCES.txt` & `nightingalejsonadapter-3.1.0/nightingalejsonadapter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nightingalejsonadapter-3.0.0/setup.py` & `nightingalejsonadapter-3.1.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from setuptools import setup, find_packages
-
-VERSION = '3.0.0' 
-DESCRIPTION = 'JSON adapter'
-LONG_DESCRIPTION = 'JSON adapters and validators for Nightingale Communication and Integration'
-
-# Setting up
-setup(
-       # the name must match the folder name 'verysimplemodule'
-        name="nightingalejsonadapter", 
-        version=VERSION,
-        author="Nuno Antunes",
-        author_email="<nuno.f.antunes@inov.pt>",
-        description=DESCRIPTION,
-        long_description=LONG_DESCRIPTION,
-        packages=find_packages(),
-        install_requires=['pydantic'], # add any additional packages that 
-        # needs to be installed along with your package. Eg: 'caer'
-        
-        keywords=['jsonadapter']
-)
-
-# python setup.py sdist bdist_wheel
+from setuptools import setup, find_packages
+
+VERSION = '3.1.0' 
+DESCRIPTION = 'JSON adapter'
+LONG_DESCRIPTION = 'JSON adapters and validators for Nightingale Communication and Integration'
+
+# Setting up
+setup(
+       # the name must match the folder name 'verysimplemodule'
+        name="nightingalejsonadapter", 
+        version=VERSION,
+        author="Nuno Antunes",
+        author_email="<nuno.f.antunes@inov.pt>",
+        description=DESCRIPTION,
+        long_description=LONG_DESCRIPTION,
+        packages=find_packages(),
+        install_requires=['pydantic'], # add any additional packages that 
+        # needs to be installed along with your package. Eg: 'caer'
+        
+        keywords=['jsonadapter']
+)
+
+# python setup.py sdist bdist_wheel
 # twine upload dist/*
```

