# Comparing `tmp/pdmcontext-0.1.4.tar.gz` & `tmp/pdmcontext-0.1.5.tar.gz`

## Comparing `pdmcontext-0.1.4.tar` & `pdmcontext-0.1.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0    26047 2020-02-02 00:00:00.000000 pdmcontext-0.1.4/Documentation/PdmContext/ContextClustering.html
--rw-r--r--   0        0        0   136382 2020-02-02 00:00:00.000000 pdmcontext-0.1.4/Documentation/PdmContext/ContextGeneration.html
--rw-r--r--   0        0        0    28792 2020-02-02 00:00:00.000000 pdmcontext-0.1.4/Documentation/PdmContext/Pipelines.html
--rw-r--r--   0        0        0  1238528 2020-02-02 00:00:00.000000 pdmcontext-0.1.4/Documentation/PdmContext/index.html
--rw-r--r--   0        0        0     7227 2020-02-02 00:00:00.000000 pdmcontext-0.1.4/Documentation/PdmContext/index_old.html
--rw-r--r--   0        0        0     8957 2020-02-02 00:00:00.000000 pdmcontext-0.1.4/Documentation/PdmContext/utils/causal_discovery_functions.html
--rw-r--r--   0        0        0    54557 2020-02-02 00:00:00.000000 pdmcontext-0.1.4/Documentation/PdmContext/utils/dbconnector.html
--rw-r--r--   0        0        0    41393 2020-02-02 00:00:00.000000 pdmcontext-0.1.4/Documentation/PdmContext/utils/distances.html
--rw-r--r--   0        0        0     8085 2020-02-02 00:00:00.000000 pdmcontext-0.1.4/Documentation/PdmContext/utils/index.html
--rw-r--r--   0        0        0    20025 2020-02-02 00:00:00.000000 pdmcontext-0.1.4/Documentation/PdmContext/utils/showcontext.html
--rw-r--r--   0        0        0    17227 2020-02-02 00:00:00.000000 pdmcontext-0.1.4/Documentation/PdmContext/utils/simulate_stream.html
--rw-r--r--   0        0        0    21819 2020-02-02 00:00:00.000000 pdmcontext-0.1.4/Documentation/PdmContext/utils/structure.html
--rw-r--r--   0        0        0   570434 2020-02-02 00:00:00.000000 pdmcontext-0.1.4/src/Example.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pdmcontext-0.1.4/src/__init__.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 pdmcontext-0.1.4/src/dummy_data.csv
--rw-r--r--   0        0        0    11537 2020-02-02 00:00:00.000000 pdmcontext-0.1.4/src/test_main.py
--rw-r--r--   0        0        0   570434 2020-02-02 00:00:00.000000 pdmcontext-0.1.4/src/.ipynb_checkpoints/Example-checkpoint.ipynb
--rw-r--r--   0        0        0     8610 2020-02-02 00:00:00.000000 pdmcontext-0.1.4/src/.ipynb_checkpoints/test_main-checkpoint.py
--rw-r--r--   0        0        0     5371 2020-02-02 00:00:00.000000 pdmcontext-0.1.4/src/PdmContext/ContextClustering.py
--rw-r--r--   0        0        0    36219 2020-02-02 00:00:00.000000 pdmcontext-0.1.4/src/PdmContext/ContextGeneration.py
--rw-r--r--   0        0        0     5607 2020-02-02 00:00:00.000000 pdmcontext-0.1.4/src/PdmContext/Pipelines.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pdmcontext-0.1.4/src/PdmContext/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pdmcontext-0.1.4/src/PdmContext/utils/__init__.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 pdmcontext-0.1.4/src/PdmContext/utils/causal_discovery_functions.py
--rw-r--r--   0        0        0    11063 2020-02-02 00:00:00.000000 pdmcontext-0.1.4/src/PdmContext/utils/dbconnector.py
--rw-r--r--   0        0        0    13720 2020-02-02 00:00:00.000000 pdmcontext-0.1.4/src/PdmContext/utils/distances.py
--rw-r--r--   0        0        0     5146 2020-02-02 00:00:00.000000 pdmcontext-0.1.4/src/PdmContext/utils/showcontext.py
--rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 pdmcontext-0.1.4/src/PdmContext/utils/simulate_stream.py
--rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 pdmcontext-0.1.4/src/PdmContext/utils/structure.py
--rw-r--r--   0        0        0    68806 2020-02-02 00:00:00.000000 pdmcontext-0.1.4/src/images/CDextraction.png
--rw-r--r--   0        0        0    68806 2020-02-02 00:00:00.000000 pdmcontext-0.1.4/src/images/.ipynb_checkpoints/CDextraction-checkpoint.png
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 pdmcontext-0.1.4/.gitignore
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 pdmcontext-0.1.4/README.md
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 pdmcontext-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 pdmcontext-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    26047 2020-02-02 00:00:00.000000 pdmcontext-0.1.5/Documentation/PdmContext/ContextClustering.html
+-rw-r--r--   0        0        0   136382 2020-02-02 00:00:00.000000 pdmcontext-0.1.5/Documentation/PdmContext/ContextGeneration.html
+-rw-r--r--   0        0        0    28792 2020-02-02 00:00:00.000000 pdmcontext-0.1.5/Documentation/PdmContext/Pipelines.html
+-rw-r--r--   0        0        0  1238528 2020-02-02 00:00:00.000000 pdmcontext-0.1.5/Documentation/PdmContext/index.html
+-rw-r--r--   0        0        0     7227 2020-02-02 00:00:00.000000 pdmcontext-0.1.5/Documentation/PdmContext/index_old.html
+-rw-r--r--   0        0        0     8957 2020-02-02 00:00:00.000000 pdmcontext-0.1.5/Documentation/PdmContext/utils/causal_discovery_functions.html
+-rw-r--r--   0        0        0    54557 2020-02-02 00:00:00.000000 pdmcontext-0.1.5/Documentation/PdmContext/utils/dbconnector.html
+-rw-r--r--   0        0        0    41393 2020-02-02 00:00:00.000000 pdmcontext-0.1.5/Documentation/PdmContext/utils/distances.html
+-rw-r--r--   0        0        0     8085 2020-02-02 00:00:00.000000 pdmcontext-0.1.5/Documentation/PdmContext/utils/index.html
+-rw-r--r--   0        0        0    20025 2020-02-02 00:00:00.000000 pdmcontext-0.1.5/Documentation/PdmContext/utils/showcontext.html
+-rw-r--r--   0        0        0    17227 2020-02-02 00:00:00.000000 pdmcontext-0.1.5/Documentation/PdmContext/utils/simulate_stream.html
+-rw-r--r--   0        0        0    21819 2020-02-02 00:00:00.000000 pdmcontext-0.1.5/Documentation/PdmContext/utils/structure.html
+-rw-r--r--   0        0        0   570434 2020-02-02 00:00:00.000000 pdmcontext-0.1.5/src/Example.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pdmcontext-0.1.5/src/__init__.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 pdmcontext-0.1.5/src/dummy_data.csv
+-rw-r--r--   0        0        0    11537 2020-02-02 00:00:00.000000 pdmcontext-0.1.5/src/test_main.py
+-rw-r--r--   0        0        0   570434 2020-02-02 00:00:00.000000 pdmcontext-0.1.5/src/.ipynb_checkpoints/Example-checkpoint.ipynb
+-rw-r--r--   0        0        0     8610 2020-02-02 00:00:00.000000 pdmcontext-0.1.5/src/.ipynb_checkpoints/test_main-checkpoint.py
+-rw-r--r--   0        0        0     5371 2020-02-02 00:00:00.000000 pdmcontext-0.1.5/src/PdmContext/ContextClustering.py
+-rw-r--r--   0        0        0    36495 2020-02-02 00:00:00.000000 pdmcontext-0.1.5/src/PdmContext/ContextGeneration.py
+-rw-r--r--   0        0        0     5607 2020-02-02 00:00:00.000000 pdmcontext-0.1.5/src/PdmContext/Pipelines.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pdmcontext-0.1.5/src/PdmContext/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pdmcontext-0.1.5/src/PdmContext/utils/__init__.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 pdmcontext-0.1.5/src/PdmContext/utils/causal_discovery_functions.py
+-rw-r--r--   0        0        0    11063 2020-02-02 00:00:00.000000 pdmcontext-0.1.5/src/PdmContext/utils/dbconnector.py
+-rw-r--r--   0        0        0    13720 2020-02-02 00:00:00.000000 pdmcontext-0.1.5/src/PdmContext/utils/distances.py
+-rw-r--r--   0        0        0     5146 2020-02-02 00:00:00.000000 pdmcontext-0.1.5/src/PdmContext/utils/showcontext.py
+-rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 pdmcontext-0.1.5/src/PdmContext/utils/simulate_stream.py
+-rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 pdmcontext-0.1.5/src/PdmContext/utils/structure.py
+-rw-r--r--   0        0        0    68806 2020-02-02 00:00:00.000000 pdmcontext-0.1.5/src/images/CDextraction.png
+-rw-r--r--   0        0        0    68806 2020-02-02 00:00:00.000000 pdmcontext-0.1.5/src/images/.ipynb_checkpoints/CDextraction-checkpoint.png
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 pdmcontext-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 pdmcontext-0.1.5/README.md
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 pdmcontext-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 pdmcontext-0.1.5/PKG-INFO
```

### Comparing `pdmcontext-0.1.4/Documentation/PdmContext/ContextClustering.html` & `pdmcontext-0.1.5/Documentation/PdmContext/ContextClustering.html`

 * *Files identical despite different names*

### Comparing `pdmcontext-0.1.4/Documentation/PdmContext/ContextGeneration.html` & `pdmcontext-0.1.5/Documentation/PdmContext/ContextGeneration.html`

 * *Files identical despite different names*

### Comparing `pdmcontext-0.1.4/Documentation/PdmContext/Pipelines.html` & `pdmcontext-0.1.5/Documentation/PdmContext/Pipelines.html`

 * *Files identical despite different names*

### Comparing `pdmcontext-0.1.4/Documentation/PdmContext/index.html` & `pdmcontext-0.1.5/Documentation/PdmContext/index.html`

 * *Files identical despite different names*

### Comparing `pdmcontext-0.1.4/Documentation/PdmContext/index_old.html` & `pdmcontext-0.1.5/Documentation/PdmContext/index_old.html`

 * *Files identical despite different names*

### Comparing `pdmcontext-0.1.4/Documentation/PdmContext/utils/causal_discovery_functions.html` & `pdmcontext-0.1.5/Documentation/PdmContext/utils/causal_discovery_functions.html`

 * *Files identical despite different names*

### Comparing `pdmcontext-0.1.4/Documentation/PdmContext/utils/dbconnector.html` & `pdmcontext-0.1.5/Documentation/PdmContext/utils/dbconnector.html`

 * *Files identical despite different names*

### Comparing `pdmcontext-0.1.4/Documentation/PdmContext/utils/distances.html` & `pdmcontext-0.1.5/Documentation/PdmContext/utils/distances.html`

 * *Files identical despite different names*

### Comparing `pdmcontext-0.1.4/Documentation/PdmContext/utils/index.html` & `pdmcontext-0.1.5/Documentation/PdmContext/utils/index.html`

 * *Files identical despite different names*

### Comparing `pdmcontext-0.1.4/Documentation/PdmContext/utils/showcontext.html` & `pdmcontext-0.1.5/Documentation/PdmContext/utils/showcontext.html`

 * *Files identical despite different names*

### Comparing `pdmcontext-0.1.4/Documentation/PdmContext/utils/simulate_stream.html` & `pdmcontext-0.1.5/Documentation/PdmContext/utils/simulate_stream.html`

 * *Files identical despite different names*

### Comparing `pdmcontext-0.1.4/Documentation/PdmContext/utils/structure.html` & `pdmcontext-0.1.5/Documentation/PdmContext/utils/structure.html`

 * *Files identical despite different names*

### Comparing `pdmcontext-0.1.4/src/Example.ipynb` & `pdmcontext-0.1.5/src/Example.ipynb`

 * *Files identical despite different names*

### Comparing `pdmcontext-0.1.4/src/dummy_data.csv` & `pdmcontext-0.1.5/src/dummy_data.csv`

 * *Files identical despite different names*

### Comparing `pdmcontext-0.1.4/src/test_main.py` & `pdmcontext-0.1.5/src/test_main.py`

 * *Files identical despite different names*

### Comparing `pdmcontext-0.1.4/src/.ipynb_checkpoints/Example-checkpoint.ipynb` & `pdmcontext-0.1.5/src/.ipynb_checkpoints/Example-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `pdmcontext-0.1.4/src/.ipynb_checkpoints/test_main-checkpoint.py` & `pdmcontext-0.1.5/src/.ipynb_checkpoints/test_main-checkpoint.py`

 * *Files identical despite different names*

### Comparing `pdmcontext-0.1.4/src/PdmContext/ContextClustering.py` & `pdmcontext-0.1.5/src/PdmContext/ContextClustering.py`

 * *Files identical despite different names*

### Comparing `pdmcontext-0.1.4/src/PdmContext/ContextGeneration.py` & `pdmcontext-0.1.5/src/PdmContext/ContextGeneration.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,38 +118,40 @@
         storing["timestamp"] = timestamp
 
         alldata_names = [nn[0] for nn in alldata]
         alldata_data = [nn[1] for nn in alldata]
 
         for namedd, datadd in zip(alldata_names, alldata_data):
             storing[namedd] = datadd
-
+        alldata_names = [nn[0] for nn in alldata if nn[1] is not None and len(set(nn[1])) > 1]
+        alldata_data = [nn[1] for nn in alldata if nn[1] is not None and len(set(nn[1])) > 1]
         # For context with more than two series calculate PC casualities
         count = len([1 for lista in alldata_data if lista is not None])
-        if count > 1 and len(alldata[0][1]) > 5:
-            alldata_names = [nn[0] for nn in alldata if nn[1] is not None and len(set(nn[1]))>1]
-            alldata_data = [nn[1] for nn in alldata if nn[1] is not None and len(set(nn[1]))>1]
-
-            #end = time.time()
-            #print(f"before {end - start}")
-            #start=time.time()
-
-            if len(alldata) <= 1:
-                edges = []
-            else:
-                edges = self.calculate_causality(np.column_stack(alldata_data), alldata_names)
-            #end=time.time()
-            #print(f"actual edge calculation {end-start}")
-            if edges is None:
-                singleedges = []
-            else:
-                singleedges = edges
-            # print(edges)
-            storing["edges"] = singleedges
-            return storing
+        if count > 1:
+            if len(alldata[0][1]) > 5:
+                # alldata_names = [nn[0] for nn in alldata if nn[1] is not None and len(set(nn[1]))>1]
+                # alldata_data = [nn[1] for nn in alldata if nn[1] is not None and len(set(nn[1]))>1]
+
+                #end = time.time()
+                #print(f"before {end - start}")
+                #start=time.time()
+
+                if len(alldata) <= 1:
+                    edges = []
+                else:
+                    edges = self.calculate_causality(np.column_stack(alldata_data), alldata_names)
+                #end=time.time()
+                #print(f"actual edge calculation {end-start}")
+                if edges is None:
+                    singleedges = []
+                else:
+                    singleedges = edges
+                # print(edges)
+                storing["edges"] = singleedges
+                return storing
         storing["edges"] = []
         return storing
 
     def calculate_causality(self, dataor, names):
         num_time_series = len(dataor)
         data = np.array(dataor)
         edges = self.causality_discovery(names, data)
```

### Comparing `pdmcontext-0.1.4/src/PdmContext/Pipelines.py` & `pdmcontext-0.1.5/src/PdmContext/Pipelines.py`

 * *Files identical despite different names*

### Comparing `pdmcontext-0.1.4/src/PdmContext/utils/causal_discovery_functions.py` & `pdmcontext-0.1.5/src/PdmContext/utils/causal_discovery_functions.py`

 * *Files identical despite different names*

### Comparing `pdmcontext-0.1.4/src/PdmContext/utils/dbconnector.py` & `pdmcontext-0.1.5/src/PdmContext/utils/dbconnector.py`

 * *Files identical despite different names*

### Comparing `pdmcontext-0.1.4/src/PdmContext/utils/distances.py` & `pdmcontext-0.1.5/src/PdmContext/utils/distances.py`

 * *Files identical despite different names*

### Comparing `pdmcontext-0.1.4/src/PdmContext/utils/showcontext.py` & `pdmcontext-0.1.5/src/PdmContext/utils/showcontext.py`

 * *Files identical despite different names*

### Comparing `pdmcontext-0.1.4/src/PdmContext/utils/simulate_stream.py` & `pdmcontext-0.1.5/src/PdmContext/utils/simulate_stream.py`

 * *Files identical despite different names*

### Comparing `pdmcontext-0.1.4/src/PdmContext/utils/structure.py` & `pdmcontext-0.1.5/src/PdmContext/utils/structure.py`

 * *Files identical despite different names*

### Comparing `pdmcontext-0.1.4/src/images/CDextraction.png` & `pdmcontext-0.1.5/src/images/CDextraction.png`

 * *Files identical despite different names*

### Comparing `pdmcontext-0.1.4/src/images/.ipynb_checkpoints/CDextraction-checkpoint.png` & `pdmcontext-0.1.5/src/images/.ipynb_checkpoints/CDextraction-checkpoint.png`

 * *Files identical despite different names*

### Comparing `pdmcontext-0.1.4/README.md` & `pdmcontext-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pdmcontext-0.1.4/pyproject.toml` & `pdmcontext-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "PdmContext"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="Apostolos Giannoulidis", email="agiannous@csd.auth.gr" },
 ]
 description = "Context is used here to provide a better understanding of how changes in data affect anomaly detection task. Essentially, Context represent the data (CD), existing in a time window, and their relationships (CR), where the relationships are extracted using causal discovery between the data (the causal discovery method can be user defiend)."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `pdmcontext-0.1.4/PKG-INFO` & `pdmcontext-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: PdmContext
-Version: 0.1.4
+Version: 0.1.5
 Summary: Context is used here to provide a better understanding of how changes in data affect anomaly detection task. Essentially, Context represent the data (CD), existing in a time window, and their relationships (CR), where the relationships are extracted using causal discovery between the data (the causal discovery method can be user defiend).
 Project-URL: Homepage, https://github.com/agiannoul/PdMContext
 Project-URL: Issues, https://github.com/agiannoul/PdMContext/issues
 Project-URL: documentation, https://pd-m-context.vercel.app/
 Author-email: Apostolos Giannoulidis <agiannous@csd.auth.gr>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

