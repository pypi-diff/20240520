# Comparing `tmp/rst2dep-1.3.0.0.tar.gz` & `tmp/rst2dep-1.3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rst2dep-1.3.0.0.tar", last modified: Tue May 14 18:11:23 2024, max compression
+gzip compressed data, was "rst2dep-1.3.0.1.tar", last modified: Sun May 19 22:22:32 2024, max compression
```

## Comparing `rst2dep-1.3.0.0.tar` & `rst2dep-1.3.0.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 18:11:23.987525 rst2dep-1.3.0.0/
--rw-rw-rw-   0        0        0    10763 2023-06-30 21:19:28.000000 rst2dep-1.3.0.0/LICENSE
--rw-rw-rw-   0        0        0      762 2024-05-14 18:11:23.986526 rst2dep-1.3.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     7757 2024-05-14 15:42:10.000000 rst2dep-1.3.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 18:11:23.979640 rst2dep-1.3.0.0/rst2dep/
--rw-rw-rw-   0        0        0    34921 2023-07-20 15:05:40.000000 rst2dep-1.3.0.0/rst2dep/GUM_academic_census.rs4
--rw-rw-rw-   0        0        0      127 2023-07-05 13:43:17.000000 rst2dep-1.3.0.0/rst2dep/__init__.py
--rw-rw-rw-   0        0        0     3249 2024-05-14 15:39:31.000000 rst2dep-1.3.0.0/rst2dep/__main__.py
--rw-rw-rw-   0        0        0    24779 2024-05-14 15:35:46.000000 rst2dep-1.3.0.0/rst2dep/classes.py
--rw-rw-rw-   0        0        0    16339 2023-07-05 13:43:13.000000 rst2dep-1.3.0.0/rst2dep/dep2rst.py
--rw-rw-rw-   0        0        0    13395 2021-10-21 19:46:30.000000 rst2dep-1.3.0.0/rst2dep/example.conllu
--rw-rw-rw-   0        0        0     2902 2021-10-21 20:26:06.000000 rst2dep-1.3.0.0/rst2dep/example.rs3
--rw-rw-rw-   0        0        0     1368 2021-10-21 20:24:03.000000 rst2dep-1.3.0.0/rst2dep/example.rsd
--rw-rw-rw-   0        0        0     3234 2023-07-05 14:04:58.000000 rst2dep-1.3.0.0/rst2dep/feature_extraction.py
--rw-rw-rw-   0        0        0     3897 2024-04-09 14:58:00.000000 rst2dep-1.3.0.0/rst2dep/four_units.rs4
--rw-rw-rw-   0        0        0      178 2024-02-26 15:37:50.000000 rst2dep-1.3.0.0/rst2dep/four_units.rsd
--rw-rw-rw-   0        0        0       58 2024-02-26 15:22:18.000000 rst2dep-1.3.0.0/rst2dep/four_units.txt
--rw-rw-rw-   0        0        0    18783 2024-05-14 18:08:13.000000 rst2dep-1.3.0.0/rst2dep/rst2dep.py
--rw-rw-rw-   0        0        0      497 2023-06-30 21:52:58.000000 rst2dep-1.3.0.0/rst2dep/run_tests.py
--rw-rw-rw-   0        0        0    13806 2024-02-27 14:57:34.000000 rst2dep-1.3.0.0/rst2dep/salinity_chain.rsd
--rw-rw-rw-   0        0        0    13803 2024-02-27 14:57:25.000000 rst2dep-1.3.0.0/rst2dep/salinity_li.rsd
-drwxrwxrwx   0        0        0        0 2024-05-14 18:11:23.985526 rst2dep-1.3.0.0/rst2dep.egg-info/
--rw-rw-rw-   0        0        0      762 2024-05-14 18:11:23.000000 rst2dep-1.3.0.0/rst2dep.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      513 2024-05-14 18:11:23.000000 rst2dep-1.3.0.0/rst2dep.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 18:11:23.000000 rst2dep-1.3.0.0/rst2dep.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-14 18:11:23.000000 rst2dep-1.3.0.0/rst2dep.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 18:11:23.987525 rst2dep-1.3.0.0/setup.cfg
--rw-rw-rw-   0        0        0      934 2024-05-14 15:41:35.000000 rst2dep-1.3.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 22:22:32.835482 rst2dep-1.3.0.1/
+-rw-rw-rw-   0        0        0    10763 2023-06-30 21:19:28.000000 rst2dep-1.3.0.1/LICENSE
+-rw-rw-rw-   0        0        0      762 2024-05-19 22:22:32.833483 rst2dep-1.3.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7757 2024-05-14 15:42:10.000000 rst2dep-1.3.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 22:22:32.818113 rst2dep-1.3.0.1/rst2dep/
+-rw-rw-rw-   0        0        0    34921 2023-07-20 15:05:40.000000 rst2dep-1.3.0.1/rst2dep/GUM_academic_census.rs4
+-rw-rw-rw-   0        0        0      127 2023-07-05 13:43:17.000000 rst2dep-1.3.0.1/rst2dep/__init__.py
+-rw-rw-rw-   0        0        0     3249 2024-05-14 15:39:31.000000 rst2dep-1.3.0.1/rst2dep/__main__.py
+-rw-rw-rw-   0        0        0    24779 2024-05-14 15:35:46.000000 rst2dep-1.3.0.1/rst2dep/classes.py
+-rw-rw-rw-   0        0        0    16339 2023-07-05 13:43:13.000000 rst2dep-1.3.0.1/rst2dep/dep2rst.py
+-rw-rw-rw-   0        0        0    13395 2021-10-21 19:46:30.000000 rst2dep-1.3.0.1/rst2dep/example.conllu
+-rw-rw-rw-   0        0        0     2902 2021-10-21 20:26:06.000000 rst2dep-1.3.0.1/rst2dep/example.rs3
+-rw-rw-rw-   0        0        0     1368 2021-10-21 20:24:03.000000 rst2dep-1.3.0.1/rst2dep/example.rsd
+-rw-rw-rw-   0        0        0     3234 2023-07-05 14:04:58.000000 rst2dep-1.3.0.1/rst2dep/feature_extraction.py
+-rw-rw-rw-   0        0        0     3897 2024-04-09 14:58:00.000000 rst2dep-1.3.0.1/rst2dep/four_units.rs4
+-rw-rw-rw-   0        0        0      178 2024-02-26 15:37:50.000000 rst2dep-1.3.0.1/rst2dep/four_units.rsd
+-rw-rw-rw-   0        0        0       58 2024-02-26 15:22:18.000000 rst2dep-1.3.0.1/rst2dep/four_units.txt
+-rw-rw-rw-   0        0        0    19789 2024-05-19 22:18:43.000000 rst2dep-1.3.0.1/rst2dep/rst2dep.py
+-rw-rw-rw-   0        0        0      497 2023-06-30 21:52:58.000000 rst2dep-1.3.0.1/rst2dep/run_tests.py
+-rw-rw-rw-   0        0        0    13806 2024-02-27 14:57:34.000000 rst2dep-1.3.0.1/rst2dep/salinity_chain.rsd
+-rw-rw-rw-   0        0        0    13803 2024-02-27 14:57:25.000000 rst2dep-1.3.0.1/rst2dep/salinity_li.rsd
+drwxrwxrwx   0        0        0        0 2024-05-19 22:22:32.830484 rst2dep-1.3.0.1/rst2dep.egg-info/
+-rw-rw-rw-   0        0        0      762 2024-05-19 22:22:32.000000 rst2dep-1.3.0.1/rst2dep.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      513 2024-05-19 22:22:32.000000 rst2dep-1.3.0.1/rst2dep.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 22:22:32.000000 rst2dep-1.3.0.1/rst2dep.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-19 22:22:32.000000 rst2dep-1.3.0.1/rst2dep.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 22:22:32.836481 rst2dep-1.3.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      934 2024-05-17 19:59:52.000000 rst2dep-1.3.0.1/setup.py
```

### Comparing `rst2dep-1.3.0.0/LICENSE` & `rst2dep-1.3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rst2dep-1.3.0.0/PKG-INFO` & `rst2dep-1.3.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: rst2dep
-Version: 1.3.0.0
+Version: 1.3.0.1
 Summary: RST (Rhetorical Structure Theory) constituent and dependency converter for discourse parses
 Home-page: https://github.com/amir-zeldes/rst2dep
-Download-URL: https://github.com/amir-zeldes/rst2dep/releases/tag/v1.3.0.0
+Download-URL: https://github.com/amir-zeldes/rst2dep/releases/tag/v1.3.0.1
 Author: Amir Zeldes
 Author-email: amir.zeldes@georgetown.edu
 License: Apache License, Version 2.0
 Keywords: NLP,RST,discourse,dependencies,converter,conversion,Rhetorical Structure Theory,parsing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rst2dep-1.3.0.0/README.md` & `rst2dep-1.3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `rst2dep-1.3.0.0/rst2dep/GUM_academic_census.rs4` & `rst2dep-1.3.0.1/rst2dep/GUM_academic_census.rs4`

 * *Files identical despite different names*

### Comparing `rst2dep-1.3.0.0/rst2dep/__main__.py` & `rst2dep-1.3.0.1/rst2dep/__main__.py`

 * *Files identical despite different names*

### Comparing `rst2dep-1.3.0.0/rst2dep/classes.py` & `rst2dep-1.3.0.1/rst2dep/classes.py`

 * *Files identical despite different names*

### Comparing `rst2dep-1.3.0.0/rst2dep/dep2rst.py` & `rst2dep-1.3.0.1/rst2dep/dep2rst.py`

 * *Files identical despite different names*

### Comparing `rst2dep-1.3.0.0/rst2dep/example.conllu` & `rst2dep-1.3.0.1/rst2dep/example.conllu`

 * *Files identical despite different names*

### Comparing `rst2dep-1.3.0.0/rst2dep/example.rs3` & `rst2dep-1.3.0.1/rst2dep/example.rs3`

 * *Files identical despite different names*

### Comparing `rst2dep-1.3.0.0/rst2dep/example.rsd` & `rst2dep-1.3.0.1/rst2dep/example.rsd`

 * *Files identical despite different names*

### Comparing `rst2dep-1.3.0.0/rst2dep/feature_extraction.py` & `rst2dep-1.3.0.1/rst2dep/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `rst2dep-1.3.0.0/rst2dep/four_units.rs4` & `rst2dep-1.3.0.1/rst2dep/four_units.rs4`

 * *Files identical despite different names*

### Comparing `rst2dep-1.3.0.0/rst2dep/rst2dep.py` & `rst2dep-1.3.0.1/rst2dep/rst2dep.py`

 * *Files 6% similar despite different names*

```diff
@@ -294,31 +294,42 @@
                     dep_rel = node.dep_rel = "ROOT"
                 else:
                     dep_rel = node.dep_rel = nodes[node.dep_parent].dep_rel
                     node.dep_parent = nodes[node.dep_parent].dep_parent
 
     # Get head EDU and height per node
     node2head_edu = {}
+    target_node2head_edu = {}  # Only distinct for chain algorithm
     for edu in edus:
         edu.height = 0
         node = edu
         edu_id = edu.id
-        node2head_edu[node.id] = edu_id
+        target_node2head_edu[node.id] = node2head_edu[node.id] = edu_id
         while node.parent != "0":
             this_height = node.height + 1
+            span_parent = node.relname == "span"
+            multinuc_parent = nodes[node.parent].kind == "multinuc" and (nodes[node.parent].leftmost_child == node.id or (node.relname.endswith("_m") and not node.relname.startswith("same")))
             node = nodes[node.parent]
             if node.kind == "edu":
                 edu_id = node.id
             if node.id not in node2head_edu:
-                node2head_edu[node.id] = edu_id
+                if span_parent or multinuc_parent:
+                    target_node2head_edu[node.id] = node2head_edu[node.id] = edu_id
                 node.height = this_height
             else:
                 if int(edu_id) < int(node2head_edu[node.id]):  # Prefer left most child as head
-                    node2head_edu[node.id] = edu_id
+                    if span_parent or multinuc_parent:
+                        node2head_edu[node.id] = edu_id
                     node.height = this_height
+                if int(edu_id) > int(target_node2head_edu[node.id]):  # Prefer right most child as head for chain target
+                    if span_parent or multinuc_parent:
+                        target_node2head_edu[node.id] = edu_id
+
+            if not span_parent and not multinuc_parent:
+                break  # A satellite relation has been traversed, stop looking for nodes headed by this
 
     # Get height distance from dependency parent to child's attachment point in the phrase structure (number of spans)
     for nid in nodes:
         node = nodes[nid]
         if node.dep_rel == "ROOT":
             node.dist = "0"
             continue
@@ -337,15 +348,18 @@
             output.append(node.out_malt())
 
     # Insert secedges if any
     src2secedges = collections.defaultdict(set)
     secedge_mapping = {}
     for secedge in secedges:
         dep_src = node2head_edu[nodes[secedge.source].id]
-        dep_trg = node2head_edu[nodes[secedge.target].id]
+        if algorithm == "chain":
+            dep_trg = target_node2head_edu[nodes[secedge.target].id]
+        else:
+            dep_trg = node2head_edu[nodes[secedge.target].id]
         src_dist = str(nodes[secedge.source].height)
         trg_dist = str(nodes[secedge.target].height)
         signals = []
         for sig in secedge.signals:
             signals.append(sig.pretty_print(tokens=document_tokens))
         signals = ";".join(sorted(signals)) if len(signals)>0 else "_"
         src2secedges[dep_src].add(":".join([dep_trg,secedge.relname,src_dist,trg_dist,signals]))
```

### Comparing `rst2dep-1.3.0.0/rst2dep/salinity_chain.rsd` & `rst2dep-1.3.0.1/rst2dep/salinity_chain.rsd`

 * *Files identical despite different names*

### Comparing `rst2dep-1.3.0.0/rst2dep/salinity_li.rsd` & `rst2dep-1.3.0.1/rst2dep/salinity_li.rsd`

 * *Files identical despite different names*

### Comparing `rst2dep-1.3.0.0/rst2dep.egg-info/PKG-INFO` & `rst2dep-1.3.0.1/rst2dep.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: rst2dep
-Version: 1.3.0.0
+Version: 1.3.0.1
 Summary: RST (Rhetorical Structure Theory) constituent and dependency converter for discourse parses
 Home-page: https://github.com/amir-zeldes/rst2dep
-Download-URL: https://github.com/amir-zeldes/rst2dep/releases/tag/v1.3.0.0
+Download-URL: https://github.com/amir-zeldes/rst2dep/releases/tag/v1.3.0.1
 Author: Amir Zeldes
 Author-email: amir.zeldes@georgetown.edu
 License: Apache License, Version 2.0
 Keywords: NLP,RST,discourse,dependencies,converter,conversion,Rhetorical Structure Theory,parsing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rst2dep-1.3.0.0/rst2dep.egg-info/SOURCES.txt` & `rst2dep-1.3.0.1/rst2dep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rst2dep-1.3.0.0/setup.py` & `rst2dep-1.3.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'rst2dep',
   packages = find_packages(),
-  version = '1.3.0.0',
+  version = '1.3.0.1',
   description = 'RST (Rhetorical Structure Theory) constituent and dependency converter for discourse parses',
   author = 'Amir Zeldes',
   author_email = 'amir.zeldes@georgetown.edu',
   package_data = {'':['README.md','LICENSE','requirements.txt'],'rst2dep':['*']},
   install_requires=[],
   url = 'https://github.com/amir-zeldes/rst2dep',
   license='Apache License, Version 2.0',
-  download_url = 'https://github.com/amir-zeldes/rst2dep/releases/tag/v1.3.0.0',
+  download_url = 'https://github.com/amir-zeldes/rst2dep/releases/tag/v1.3.0.1',
   keywords = ['NLP', 'RST', 'discourse', 'dependencies', 'converter', 'conversion','Rhetorical Structure Theory','parsing'],
   classifiers = ['Programming Language :: Python',
 'Programming Language :: Python :: 2',
 'Programming Language :: Python :: 3',
 'License :: OSI Approved :: Apache Software License',
 'Operating System :: OS Independent'],
 )
```

