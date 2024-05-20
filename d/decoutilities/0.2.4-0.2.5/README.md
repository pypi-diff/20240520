# Comparing `tmp/decoutilities-0.2.4.tar.gz` & `tmp/decoutilities-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decoutilities-0.2.4.tar", last modified: Sat May 18 20:26:37 2024, max compression
+gzip compressed data, was "decoutilities-0.2.5.tar", last modified: Mon May 20 11:41:38 2024, max compression
```

## Comparing `decoutilities-0.2.4.tar` & `decoutilities-0.2.5.tar`

### file list

```diff
@@ -1,26 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 20:26:37.645125 decoutilities-0.2.4/
--rw-rw-rw-   0        0        0     1089 2024-05-08 22:21:06.000000 decoutilities-0.2.4/LICENSE
--rw-rw-rw-   0        0        0    12193 2024-05-18 20:26:37.643042 decoutilities-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0    11722 2024-05-18 20:24:49.000000 decoutilities-0.2.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 20:26:37.624572 decoutilities-0.2.4/decoutilities/
--rw-rw-rw-   0        0        0     4740 2024-05-08 22:21:06.000000 decoutilities-0.2.4/decoutilities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-18 20:26:37.632977 decoutilities-0.2.4/decoutilities/config/
--rw-rw-rw-   0        0        0      104 2024-05-08 22:21:06.000000 decoutilities-0.2.4/decoutilities/config/__init__.py
--rw-rw-rw-   0        0        0      994 2024-05-08 22:21:06.000000 decoutilities-0.2.4/decoutilities/config/config.py
--rw-rw-rw-   0        0        0     2736 2024-05-08 22:21:06.000000 decoutilities-0.2.4/decoutilities/config/configContainer.py
-drwxrwxrwx   0        0        0        0 2024-05-18 20:26:37.636711 decoutilities-0.2.4/decoutilities/data/
--rw-rw-rw-   0        0        0      104 2024-05-08 22:21:06.000000 decoutilities-0.2.4/decoutilities/data/__init__.py
--rw-rw-rw-   0        0        0     2154 2024-05-08 22:21:06.000000 decoutilities-0.2.4/decoutilities/data/dataEncryptor.py
--rw-rw-rw-   0        0        0     1671 2024-05-08 22:21:06.000000 decoutilities-0.2.4/decoutilities/data/keyManager.py
-drwxrwxrwx   0        0        0        0 2024-05-18 20:26:37.638817 decoutilities-0.2.4/decoutilities/inject/
--rw-rw-rw-   0        0        0       44 2024-05-08 22:21:06.000000 decoutilities-0.2.4/decoutilities/inject/__init__.py
--rw-rw-rw-   0        0        0      569 2024-05-18 20:23:23.000000 decoutilities-0.2.4/decoutilities/inject/injector.py
-drwxrwxrwx   0        0        0        0 2024-05-18 20:26:37.639876 decoutilities-0.2.4/decoutilities/queue/
--rw-rw-rw-   0        0        0     1043 2024-05-08 22:21:06.000000 decoutilities-0.2.4/decoutilities/queue/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-18 20:26:37.641983 decoutilities-0.2.4/decoutilities.egg-info/
--rw-rw-rw-   0        0        0    12193 2024-05-18 20:26:37.000000 decoutilities-0.2.4/decoutilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      502 2024-05-18 20:26:37.000000 decoutilities-0.2.4/decoutilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 20:26:37.000000 decoutilities-0.2.4/decoutilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-18 20:26:37.000000 decoutilities-0.2.4/decoutilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 20:26:37.645125 decoutilities-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0      729 2024-05-18 20:20:07.000000 decoutilities-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 11:41:38.395916 decoutilities-0.2.5/
+-rw-rw-rw-   0        0        0     1089 2024-05-08 11:01:18.000000 decoutilities-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0    12193 2024-05-20 11:41:38.351916 decoutilities-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0    11722 2024-05-20 10:37:54.000000 decoutilities-0.2.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 11:41:37.663917 decoutilities-0.2.5/decoutilities/
+-rw-rw-rw-   0        0        0     4740 2024-05-07 07:54:09.000000 decoutilities-0.2.5/decoutilities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 11:41:37.952917 decoutilities-0.2.5/decoutilities/config/
+-rw-rw-rw-   0        0        0      104 2024-04-29 13:15:34.000000 decoutilities-0.2.5/decoutilities/config/__init__.py
+-rw-rw-rw-   0        0        0      994 2024-04-26 08:33:42.000000 decoutilities-0.2.5/decoutilities/config/config.py
+-rw-rw-rw-   0        0        0     2736 2024-04-30 08:27:33.000000 decoutilities-0.2.5/decoutilities/config/configContainer.py
+drwxrwxrwx   0        0        0        0 2024-05-20 11:41:38.065916 decoutilities-0.2.5/decoutilities/data/
+-rw-rw-rw-   0        0        0      104 2024-05-08 07:57:21.000000 decoutilities-0.2.5/decoutilities/data/__init__.py
+-rw-rw-rw-   0        0        0     2154 2024-05-08 07:56:33.000000 decoutilities-0.2.5/decoutilities/data/dataEncryptor.py
+-rw-rw-rw-   0        0        0     1671 2024-05-08 07:52:43.000000 decoutilities-0.2.5/decoutilities/data/keyManager.py
+drwxrwxrwx   0        0        0        0 2024-05-20 11:41:38.108918 decoutilities-0.2.5/decoutilities/inject/
+-rw-rw-rw-   0        0        0       44 2024-04-29 13:15:19.000000 decoutilities-0.2.5/decoutilities/inject/__init__.py
+-rw-rw-rw-   0        0        0      569 2024-05-20 10:37:54.000000 decoutilities-0.2.5/decoutilities/inject/injector.py
+drwxrwxrwx   0        0        0        0 2024-05-20 11:41:38.136917 decoutilities-0.2.5/decoutilities/logger/
+-rw-rw-rw-   0        0        0     1212 2024-05-20 11:36:36.000000 decoutilities-0.2.5/decoutilities/logger/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 11:41:38.197917 decoutilities-0.2.5/decoutilities/queue/
+-rw-rw-rw-   0        0        0     1043 2024-05-07 08:05:33.000000 decoutilities-0.2.5/decoutilities/queue/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 11:41:38.223918 decoutilities-0.2.5/decoutilities/textUtils/
+-rw-rw-rw-   0        0        0     2427 2024-05-20 10:37:30.000000 decoutilities-0.2.5/decoutilities/textUtils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 11:41:38.249918 decoutilities-0.2.5/decoutilities.egg-info/
+-rw-rw-rw-   0        0        0    12193 2024-05-20 11:41:36.000000 decoutilities-0.2.5/decoutilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      571 2024-05-20 11:41:37.000000 decoutilities-0.2.5/decoutilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 11:41:36.000000 decoutilities-0.2.5/decoutilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-20 11:41:36.000000 decoutilities-0.2.5/decoutilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 11:41:38.396917 decoutilities-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      729 2024-05-20 10:38:59.000000 decoutilities-0.2.5/setup.py
```

### Comparing `decoutilities-0.2.4/LICENSE` & `decoutilities-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.4/PKG-INFO` & `decoutilities-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoutilities
-Version: 0.2.4
+Version: 0.2.5
 Summary: Enhance the readability of your code with decorators and simplify the creation of configuration files.
 Author: Hugo Torres
 Author-email: contact@redactado.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `decoutilities-0.2.4/README.md` & `decoutilities-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.4/decoutilities/__init__.py` & `decoutilities-0.2.5/decoutilities/__init__.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.4/decoutilities/config/config.py` & `decoutilities-0.2.5/decoutilities/config/config.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.4/decoutilities/config/configContainer.py` & `decoutilities-0.2.5/decoutilities/config/configContainer.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.4/decoutilities/data/dataEncryptor.py` & `decoutilities-0.2.5/decoutilities/data/dataEncryptor.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.4/decoutilities/data/keyManager.py` & `decoutilities-0.2.5/decoutilities/data/keyManager.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.4/decoutilities/inject/injector.py` & `decoutilities-0.2.5/decoutilities/inject/injector.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.4/decoutilities/queue/__init__.py` & `decoutilities-0.2.5/decoutilities/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.4/decoutilities.egg-info/PKG-INFO` & `decoutilities-0.2.5/decoutilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoutilities
-Version: 0.2.4
+Version: 0.2.5
 Summary: Enhance the readability of your code with decorators and simplify the creation of configuration files.
 Author: Hugo Torres
 Author-email: contact@redactado.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `decoutilities-0.2.4/setup.py` & `decoutilities-0.2.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
 name='decoutilities',
-version='0.2.4',
+version='0.2.5',
 author='Hugo Torres',
 author_email='contact@redactado.es',
 description='Enhance the readability of your code with decorators and simplify the creation of configuration files.',
 packages=find_packages(include=['decoutilities', 'decoutilities.*']),
 classifiers=[
 'Programming Language :: Python :: 3',
 'License :: OSI Approved :: MIT License',
```

