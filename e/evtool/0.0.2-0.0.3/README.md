# Comparing `tmp/evtool-0.0.2.tar.gz` & `tmp/evtool-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evtool-0.0.2.tar", last modified: Wed Oct 18 15:11:10 2023, max compression
+gzip compressed data, was "evtool-0.0.3.tar", last modified: Mon May 20 10:45:07 2024, max compression
```

## Comparing `evtool-0.0.2.tar` & `evtool-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 sluys     (1000) sluys     (1000)        0 2023-10-18 15:11:10.792080 evtool-0.0.2/
--rw-r--r--   0 sluys     (1000) sluys     (1000)    13827 2023-10-18 14:41:43.000000 evtool-0.0.2/LICENCE
--rw-r--r--   0 sluys     (1000) sluys     (1000)     2673 2023-10-18 15:11:10.791081 evtool-0.0.2/PKG-INFO
--rw-r--r--   0 sluys     (1000) sluys     (1000)     1607 2023-10-18 14:55:50.000000 evtool-0.0.2/README.md
-drwxr-xr-x   0 sluys     (1000) sluys     (1000)        0 2023-10-18 15:11:10.791081 evtool-0.0.2/evtool/
--rw-r--r--   0 sluys     (1000) sluys     (1000)     1597 2023-10-18 15:10:31.000000 evtool-0.0.2/evtool/__init__.py
--rw-r--r--   0 sluys     (1000) sluys     (1000)     4911 2023-10-18 15:08:40.000000 evtool-0.0.2/evtool/plt.py
-drwxr-xr-x   0 sluys     (1000) sluys     (1000)        0 2023-10-18 15:11:10.791081 evtool-0.0.2/evtool.egg-info/
--rw-r--r--   0 sluys     (1000) sluys     (1000)     2673 2023-10-18 15:11:10.000000 evtool-0.0.2/evtool.egg-info/PKG-INFO
--rw-r--r--   0 sluys     (1000) sluys     (1000)      214 2023-10-18 15:11:10.000000 evtool-0.0.2/evtool.egg-info/SOURCES.txt
--rw-r--r--   0 sluys     (1000) sluys     (1000)        1 2023-10-18 15:11:10.000000 evtool-0.0.2/evtool.egg-info/dependency_links.txt
--rw-r--r--   0 sluys     (1000) sluys     (1000)        7 2023-10-18 15:11:10.000000 evtool-0.0.2/evtool.egg-info/requires.txt
--rw-r--r--   0 sluys     (1000) sluys     (1000)        7 2023-10-18 15:11:10.000000 evtool-0.0.2/evtool.egg-info/top_level.txt
--rw-r--r--   0 sluys     (1000) sluys     (1000)     1225 2023-10-18 15:10:49.000000 evtool-0.0.2/pyproject.toml
--rw-r--r--   0 sluys     (1000) sluys     (1000)       38 2023-10-18 15:11:10.792080 evtool-0.0.2/setup.cfg
+drwxr-xr-x   0 sluys     (1000) sluys     (1000)        0 2024-05-20 10:45:07.772069 evtool-0.0.3/
+-rw-r--r--   0 sluys     (1000) sluys     (1000)    13827 2023-10-18 14:41:43.000000 evtool-0.0.3/LICENCE
+-rw-r--r--   0 sluys     (1000) sluys     (1000)     2673 2024-05-20 10:45:07.772069 evtool-0.0.3/PKG-INFO
+-rw-r--r--   0 sluys     (1000) sluys     (1000)     1607 2023-10-18 14:55:50.000000 evtool-0.0.3/README.md
+drwxr-xr-x   0 sluys     (1000) sluys     (1000)        0 2024-05-20 10:45:07.771069 evtool-0.0.3/evtool/
+-rw-r--r--   0 sluys     (1000) sluys     (1000)     1645 2024-05-20 10:43:50.000000 evtool-0.0.3/evtool/__init__.py
+-rw-r--r--   0 sluys     (1000) sluys     (1000)     4360 2024-05-20 10:43:50.000000 evtool-0.0.3/evtool/mdl.py
+-rw-r--r--   0 sluys     (1000) sluys     (1000)     4916 2024-05-20 10:43:50.000000 evtool-0.0.3/evtool/plt.py
+drwxr-xr-x   0 sluys     (1000) sluys     (1000)        0 2024-05-20 10:45:07.772069 evtool-0.0.3/evtool.egg-info/
+-rw-r--r--   0 sluys     (1000) sluys     (1000)     2673 2024-05-20 10:45:07.000000 evtool-0.0.3/evtool.egg-info/PKG-INFO
+-rw-r--r--   0 sluys     (1000) sluys     (1000)      249 2024-05-20 10:45:07.000000 evtool-0.0.3/evtool.egg-info/SOURCES.txt
+-rw-r--r--   0 sluys     (1000) sluys     (1000)        1 2024-05-20 10:45:07.000000 evtool-0.0.3/evtool.egg-info/dependency_links.txt
+-rw-r--r--   0 sluys     (1000) sluys     (1000)        7 2024-05-20 10:45:07.000000 evtool-0.0.3/evtool.egg-info/requires.txt
+-rw-r--r--   0 sluys     (1000) sluys     (1000)        7 2024-05-20 10:45:07.000000 evtool-0.0.3/evtool.egg-info/top_level.txt
+-rw-r--r--   0 sluys     (1000) sluys     (1000)     1225 2024-05-20 10:44:37.000000 evtool-0.0.3/pyproject.toml
+-rw-r--r--   0 sluys     (1000) sluys     (1000)       38 2024-05-20 10:45:07.772069 evtool-0.0.3/setup.cfg
+drwxr-xr-x   0 sluys     (1000) sluys     (1000)        0 2024-05-20 10:45:07.771069 evtool-0.0.3/test/
+-rwxr-xr-x   0 sluys     (1000) sluys     (1000)     1222 2023-10-18 14:37:52.000000 evtool-0.0.3/test/test_readplt.py
```

### Comparing `evtool-0.0.2/LICENCE` & `evtool-0.0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `evtool-0.0.2/PKG-INFO` & `evtool-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evtool
-Version: 0.0.2
+Version: 0.0.3
 Summary: Analyse and display output from the binary stellar-evolution code ev (a.k.a. STARS and TWIN).
 Author-email: Marc van der Sluys <git@vandersluys.nl>
 License: EUPL 1.2
 Project-URL: GitHub, https://github.com/MarcvdSluys/evTool
 Project-URL: ReadTheDocs, https://evtool.readthedocs.io
 Keywords: astrophysics,stellar evolution,binary evolution,stellar model,binary model
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `evtool-0.0.2/README.md` & `evtool-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `evtool-0.0.2/evtool/__init__.py` & `evtool-0.0.3/evtool/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # SPDX-License-Identifier: EUPL-1.2
 #  
-#  Copyright (c) 2023  Marc van der Sluys - Nikhef/Utrecht University - marc.vandersluys.nl
+#  Copyright (c) 2024  Marc van der Sluys - Nikhef/Utrecht University - marc.vandersluys.nl
 #   
 #  This file is part of the evTool Python package:
 #  Analyse and display output from the binary stellar-evolution code ev (a.k.a. STARS or TWIN).
 #  See: https://github.com/MarcvdSluys/evTool
 #   
 #  This is free software: you can redistribute it and/or modify it under the terms of the European Union
 #  Public Licence 1.2 (EUPL 1.2).  This software is distributed in the hope that it will be useful, but
@@ -26,7 +26,9 @@
 
 """
 
 
 name = 'evtool'
 __author__ = 'Marc van der Sluys - Nikhef/Utrecht University - marc.vandersluys.nl'
 
+from .plt      import *
+from .mdl      import *
```

### Comparing `evtool-0.0.2/evtool/plt.py` & `evtool-0.0.3/evtool/plt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # SPDX-License-Identifier: EUPL-1.2
 #  
-#  Copyright (c) 2023  Marc van der Sluys - Nikhef/Utrecht University - marc.vandersluys.nl
+#  Copyright (c) 2024  Marc van der Sluys - Nikhef/Utrecht University - marc.vandersluys.nl
 #  
 #  This file is part of the evTool Python package:
 #  Analyse and display output from the binary stellar-evolution code ev (a.k.a. STARS or TWIN).
 #  See: https://github.com/MarcvdSluys/evTool
 #  
 #  This is free software: you can redistribute it and/or modify it under the terms of the European Union
 #  Public Licence 1.2 (EUPL 1.2).  This software is distributed in the hope that it will be useful, but
@@ -15,16 +15,16 @@
 
 
 """ Code to deal with ev/STARS/TWIN plt files.
     2023-09-08, MvdS: initial version.
 """
 
 
-import pandas as pd
-import sluyspy.cli as scli
+import pandas as _pd
+import sluyspy.cli as _scli
 
 
 def read_plt(plt_name, verbosity=0):
     """Read an ev/STARS/TWIN .plt[12] file containing global/stellar-evolution variables and return a Pandas
     DataFrame.
     
     Args:
@@ -74,28 +74,28 @@
                      'O_srf','Ne_srf','Mg_srf','H_tmax','He_tmax','C_tmax','N_tmax','O_tmax','Ne_tmax',
                      'Mg_tmax','H_ctr','He_ctr','C_ctr','N_ctr','O_ctr','Ne_ctr','Mg_ctr','mcb_1s','mcb_1e',
                      'mcb_2s','mcb_2e','mcb_3s','mcb_3e','msb_1s','msb_1e','msb_2s','msb_2e','msb_3s','msb_3e',
                      'nuc_1s','nuc_1e','nuc_2s','nuc_2e','nuc_3s','nuc_3e','Qconv','Pc','Protc','BE0','BE1',
                      'BE2','BE3','Sc','ST1e5K','RHe','RCO','strmdl']
         
     else:
-        scli.error('read_plt(): unsupported number of columns for '+plt_name+': '+str(ncols))
+        _scli.error('read_plt(): unsupported number of columns for '+plt_name+': '+str(ncols))
         
     
     iline = 0
-    df = pd.DataFrame()
+    df = _pd.DataFrame()
     while True:
         iline += 1
         line = input_file.readline()
         # print(iline, line)
         if line=='': break  # EoF
         
         arr = format_body.read(line)
         if iline==1:
-            df = pd.DataFrame([arr])
+            df = _pd.DataFrame([arr])
         else:
             df.loc[len(df.index)] = arr
         
     df.columns = col_names
     
     return df
```

### Comparing `evtool-0.0.2/evtool.egg-info/PKG-INFO` & `evtool-0.0.3/evtool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evtool
-Version: 0.0.2
+Version: 0.0.3
 Summary: Analyse and display output from the binary stellar-evolution code ev (a.k.a. STARS and TWIN).
 Author-email: Marc van der Sluys <git@vandersluys.nl>
 License: EUPL 1.2
 Project-URL: GitHub, https://github.com/MarcvdSluys/evTool
 Project-URL: ReadTheDocs, https://evtool.readthedocs.io
 Keywords: astrophysics,stellar evolution,binary evolution,stellar model,binary model
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `evtool-0.0.2/pyproject.toml` & `evtool-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "evtool"
-version = "0.0.2"
+version = "0.0.3"
 authors = [ { name="Marc van der Sluys", email="git@vandersluys.nl" } ]
 description = "Analyse and display output from the binary stellar-evolution code ev (a.k.a. STARS and TWIN)."
 readme   = "README.md"
 license  = {text = "EUPL 1.2"}
 keywords = ["astrophysics","stellar evolution","binary evolution","stellar model","binary model"]
 dependencies = ["pandas"]
```

