# Comparing `tmp/linkedit-1.0.2.tar.gz` & `tmp/linkedit-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkedit-1.0.2.tar", last modified: Sun May 19 22:13:04 2024, max compression
+gzip compressed data, was "linkedit-1.0.3.tar", last modified: Sun May 19 22:48:10 2024, max compression
```

## Comparing `linkedit-1.0.2.tar` & `linkedit-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-19 22:13:04.287960 linkedit-1.0.2/
--rw-r--r--   0 khiat     (1000) khiat     (1000)    74013 2024-05-19 22:13:04.287960 linkedit-1.0.2/PKG-INFO
--rw-rw-r--   0 khiat     (1000) khiat     (1000)    73559 2024-05-19 15:00:32.000000 linkedit-1.0.2/README.md
-drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-19 22:13:04.287960 linkedit-1.0.2/linkedit/
--rw-rw-r--   0 khiat     (1000) khiat     (1000)      280 2024-05-19 17:39:14.000000 linkedit-1.0.2/linkedit/__init__.py
--rw-r--r--   0 khiat     (1000) khiat     (1000)   100702 2024-05-19 22:10:01.000000 linkedit-1.0.2/linkedit/linkedit.py
-drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-19 22:13:04.287960 linkedit-1.0.2/linkedit.egg-info/
--rw-r--r--   0 khiat     (1000) khiat     (1000)    74013 2024-05-19 22:13:04.000000 linkedit-1.0.2/linkedit.egg-info/PKG-INFO
--rw-r--r--   0 khiat     (1000) khiat     (1000)      219 2024-05-19 22:13:04.000000 linkedit-1.0.2/linkedit.egg-info/SOURCES.txt
--rw-r--r--   0 khiat     (1000) khiat     (1000)        1 2024-05-19 22:13:04.000000 linkedit-1.0.2/linkedit.egg-info/dependency_links.txt
--rw-r--r--   0 khiat     (1000) khiat     (1000)       16 2024-05-19 22:13:04.000000 linkedit-1.0.2/linkedit.egg-info/requires.txt
--rw-r--r--   0 khiat     (1000) khiat     (1000)        9 2024-05-19 22:13:04.000000 linkedit-1.0.2/linkedit.egg-info/top_level.txt
--rw-r--r--   0 khiat     (1000) khiat     (1000)       38 2024-05-19 22:13:04.287960 linkedit-1.0.2/setup.cfg
--rw-rw-r--   0 khiat     (1000) khiat     (1000)      721 2024-05-19 22:12:46.000000 linkedit-1.0.2/setup.py
+drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-19 22:48:10.583886 linkedit-1.0.3/
+-rw-r--r--   0 khiat     (1000) khiat     (1000)    74010 2024-05-19 22:48:10.583886 linkedit-1.0.3/PKG-INFO
+-rw-rw-r--   0 khiat     (1000) khiat     (1000)    73556 2024-05-19 22:43:18.000000 linkedit-1.0.3/README.md
+drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-19 22:48:10.583886 linkedit-1.0.3/linkedit/
+-rw-rw-r--   0 khiat     (1000) khiat     (1000)      280 2024-05-19 17:39:14.000000 linkedit-1.0.3/linkedit/__init__.py
+-rw-r--r--   0 khiat     (1000) khiat     (1000)   100702 2024-05-19 22:10:00.000000 linkedit-1.0.3/linkedit/linkedit.py
+drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-19 22:48:10.583886 linkedit-1.0.3/linkedit.egg-info/
+-rw-r--r--   0 khiat     (1000) khiat     (1000)    74010 2024-05-19 22:48:10.000000 linkedit-1.0.3/linkedit.egg-info/PKG-INFO
+-rw-r--r--   0 khiat     (1000) khiat     (1000)      219 2024-05-19 22:48:10.000000 linkedit-1.0.3/linkedit.egg-info/SOURCES.txt
+-rw-r--r--   0 khiat     (1000) khiat     (1000)        1 2024-05-19 22:48:10.000000 linkedit-1.0.3/linkedit.egg-info/dependency_links.txt
+-rw-r--r--   0 khiat     (1000) khiat     (1000)       16 2024-05-19 22:48:10.000000 linkedit-1.0.3/linkedit.egg-info/requires.txt
+-rw-r--r--   0 khiat     (1000) khiat     (1000)        9 2024-05-19 22:48:10.000000 linkedit-1.0.3/linkedit.egg-info/top_level.txt
+-rw-r--r--   0 khiat     (1000) khiat     (1000)       38 2024-05-19 22:48:10.583886 linkedit-1.0.3/setup.cfg
+-rw-rw-r--   0 khiat     (1000) khiat     (1000)      721 2024-05-19 22:47:33.000000 linkedit-1.0.3/setup.py
```

### Comparing `linkedit-1.0.2/PKG-INFO` & `linkedit-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkedit
-Version: 1.0.2
+Version: 1.0.3
 Summary: Sophisticate Linked List
 Home-page: https://pypi.org/project/linkedit/
 Author: khiat Mohammed Abderrezzak
 Author-email: khiat.abderrezzak@gmail.com
 License: MIT
 Keywords: linked list
 Classifier: Programming Language :: Python :: 3
@@ -699,15 +699,15 @@
 {6: {'current value @ddress': '0x7f2ffda139d0', 'next value': 3, 'next value @ddress': '0x7f2ffda13a90'}, 3: {'current value @ddress': '0x7f2ffda13a90', 'next value': 8, 'next value @ddress': '0x7f2ffda13990'}, 8: {'current value @ddress': '0x7f2ffda13990', 'next value': 1, 'next value @ddress': '0x7f2ffda3c1d0'}, 1: {'current value @ddress': '0x7f2ffda3c1d0', 'next value': 9, 'next value @ddress': '0x7f2ffd81bb90'}, 9: {'current value @ddress': '0x7f2ffd81bb90', 'next value': 5, 'next value @ddress': '0x7f2ffd81b9d0'}, 5: {'current value @ddress': '0x7f2ffd81b9d0', 'next value': 7, 'next value @ddress': '0x7f2ffd81bcd0'}, 7: {'current value @ddress': '0x7f2ffd81bcd0', 'next value': 6, 'next value @ddress': '0x7f2ffda139d0'}}
 ```
 
 
 #### Advanced Usage
 
 
-##### You Can Looping Over All Linked List Values With A Time Complexity Of O(n)
+##### You Can Loop Over All Linked List Values With A Time Complexity Of O(n)
 
 
 ```python
 from linkedit import singlyLinkedList
 
 
 x = singlyLinkedList([6, 3, 8, 1, 9, 5, 7])
```

### Comparing `linkedit-1.0.2/README.md` & `linkedit-1.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -684,15 +684,15 @@
 {6: {'current value @ddress': '0x7f2ffda139d0', 'next value': 3, 'next value @ddress': '0x7f2ffda13a90'}, 3: {'current value @ddress': '0x7f2ffda13a90', 'next value': 8, 'next value @ddress': '0x7f2ffda13990'}, 8: {'current value @ddress': '0x7f2ffda13990', 'next value': 1, 'next value @ddress': '0x7f2ffda3c1d0'}, 1: {'current value @ddress': '0x7f2ffda3c1d0', 'next value': 9, 'next value @ddress': '0x7f2ffd81bb90'}, 9: {'current value @ddress': '0x7f2ffd81bb90', 'next value': 5, 'next value @ddress': '0x7f2ffd81b9d0'}, 5: {'current value @ddress': '0x7f2ffd81b9d0', 'next value': 7, 'next value @ddress': '0x7f2ffd81bcd0'}, 7: {'current value @ddress': '0x7f2ffd81bcd0', 'next value': 6, 'next value @ddress': '0x7f2ffda139d0'}}
 ```
 
 
 #### Advanced Usage
 
 
-##### You Can Looping Over All Linked List Values With A Time Complexity Of O(n)
+##### You Can Loop Over All Linked List Values With A Time Complexity Of O(n)
 
 
 ```python
 from linkedit import singlyLinkedList
 
 
 x = singlyLinkedList([6, 3, 8, 1, 9, 5, 7])
```

### Comparing `linkedit-1.0.2/linkedit/linkedit.py` & `linkedit-1.0.3/linkedit/linkedit.py`

 * *Files identical despite different names*

### Comparing `linkedit-1.0.2/linkedit.egg-info/PKG-INFO` & `linkedit-1.0.3/linkedit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkedit
-Version: 1.0.2
+Version: 1.0.3
 Summary: Sophisticate Linked List
 Home-page: https://pypi.org/project/linkedit/
 Author: khiat Mohammed Abderrezzak
 Author-email: khiat.abderrezzak@gmail.com
 License: MIT
 Keywords: linked list
 Classifier: Programming Language :: Python :: 3
@@ -699,15 +699,15 @@
 {6: {'current value @ddress': '0x7f2ffda139d0', 'next value': 3, 'next value @ddress': '0x7f2ffda13a90'}, 3: {'current value @ddress': '0x7f2ffda13a90', 'next value': 8, 'next value @ddress': '0x7f2ffda13990'}, 8: {'current value @ddress': '0x7f2ffda13990', 'next value': 1, 'next value @ddress': '0x7f2ffda3c1d0'}, 1: {'current value @ddress': '0x7f2ffda3c1d0', 'next value': 9, 'next value @ddress': '0x7f2ffd81bb90'}, 9: {'current value @ddress': '0x7f2ffd81bb90', 'next value': 5, 'next value @ddress': '0x7f2ffd81b9d0'}, 5: {'current value @ddress': '0x7f2ffd81b9d0', 'next value': 7, 'next value @ddress': '0x7f2ffd81bcd0'}, 7: {'current value @ddress': '0x7f2ffd81bcd0', 'next value': 6, 'next value @ddress': '0x7f2ffda139d0'}}
 ```
 
 
 #### Advanced Usage
 
 
-##### You Can Looping Over All Linked List Values With A Time Complexity Of O(n)
+##### You Can Loop Over All Linked List Values With A Time Complexity Of O(n)
 
 
 ```python
 from linkedit import singlyLinkedList
 
 
 x = singlyLinkedList([6, 3, 8, 1, 9, 5, 7])
```

### Comparing `linkedit-1.0.2/setup.py` & `linkedit-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="linkedit",
-    version="1.0.2",
+    version="1.0.3",
     author="khiat Mohammed Abderrezzak",
     author_email="khiat.abderrezzak@gmail.com",
     license="MIT",
     description="Sophisticate Linked List",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://pypi.org/project/linkedit/",
```

