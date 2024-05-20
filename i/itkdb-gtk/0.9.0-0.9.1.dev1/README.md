# Comparing `tmp/itkdb_gtk-0.9.0.tar.gz` & `tmp/itkdb_gtk-0.9.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itkdb_gtk-0.9.0.tar", last modified: Thu Apr  4 08:12:35 2024, max compression
+gzip compressed data, was "itkdb_gtk-0.9.1.dev1.tar", last modified: Tue Apr  9 09:38:50 2024, max compression
```

## Comparing `itkdb_gtk-0.9.0.tar` & `itkdb_gtk-0.9.1.dev1.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxr-xr-x   0 lacasta    (501) staff       (20)        0 2024-04-04 08:12:35.518084 itkdb_gtk-0.9.0/
--rw-r--r--   0 lacasta    (501) staff       (20)     3148 2024-04-04 08:12:35.517901 itkdb_gtk-0.9.0/PKG-INFO
--rw-r--r--   0 lacasta    (501) staff       (20)     2443 2024-04-01 19:21:18.000000 itkdb_gtk-0.9.0/README.md
-drwxr-xr-x   0 lacasta    (501) staff       (20)        0 2024-04-04 08:12:35.516713 itkdb_gtk-0.9.0/itkdb_gtk/
--rw-r--r--   0 lacasta    (501) staff       (20)    13159 2024-04-03 15:10:25.000000 itkdb_gtk-0.9.0/itkdb_gtk/CreateShipments.py
--rw-r--r--   0 lacasta    (501) staff       (20)    18739 2024-04-03 15:10:34.000000 itkdb_gtk-0.9.0/itkdb_gtk/GetShipments.py
--rw-r--r--   0 lacasta    (501) staff       (20)    12247 2024-04-03 15:13:45.000000 itkdb_gtk-0.9.0/itkdb_gtk/GlueWeight.py
--rw-r--r--   0 lacasta    (501) staff       (20)     9214 2024-04-03 15:11:24.000000 itkdb_gtk-0.9.0/itkdb_gtk/GroundVITests.py
--rw-r--r--   0 lacasta    (501) staff       (20)      172 2023-04-21 15:44:09.000000 itkdb_gtk-0.9.0/itkdb_gtk/ITkDB.desktop
--rw-r--r--   0 lacasta    (501) staff       (20)    24242 2024-04-01 21:45:02.000000 itkdb_gtk-0.9.0/itkdb_gtk/ITkDB.svg
--rw-r--r--   0 lacasta    (501) staff       (20)     9916 2024-04-03 15:11:28.000000 itkdb_gtk-0.9.0/itkdb_gtk/ITkDBlogin.py
--rw-r--r--   0 lacasta    (501) staff       (20)    14862 2024-04-03 15:55:55.000000 itkdb_gtk-0.9.0/itkdb_gtk/ITkDButils.py
--rw-r--r--   0 lacasta    (501) staff       (20)     8407 2024-02-29 19:12:17.000000 itkdb_gtk-0.9.0/itkdb_gtk/ShowAttachments.py
--rw-r--r--   0 lacasta    (501) staff       (20)     3154 2024-02-29 19:16:49.000000 itkdb_gtk-0.9.0/itkdb_gtk/ShowComments.py
--rw-r--r--   0 lacasta    (501) staff       (20)     3533 2024-02-29 19:17:50.000000 itkdb_gtk-0.9.0/itkdb_gtk/ShowDefects.py
--rw-r--r--   0 lacasta    (501) staff       (20)    28135 2024-04-03 15:15:38.000000 itkdb_gtk-0.9.0/itkdb_gtk/UploadModuleIV.py
--rw-r--r--   0 lacasta    (501) staff       (20)    22120 2024-04-03 15:16:30.000000 itkdb_gtk-0.9.0/itkdb_gtk/UploadMultipleTests.py
--rw-r--r--   0 lacasta    (501) staff       (20)    22194 2024-04-03 15:16:49.000000 itkdb_gtk-0.9.0/itkdb_gtk/UploadPetalInformation.py
--rw-r--r--   0 lacasta    (501) staff       (20)    16511 2024-04-03 15:16:59.000000 itkdb_gtk-0.9.0/itkdb_gtk/UploadTest.py
--rw-r--r--   0 lacasta    (501) staff       (20)    25761 2024-04-03 15:17:14.000000 itkdb_gtk-0.9.0/itkdb_gtk/WireBondGui.py
--rw-r--r--   0 lacasta    (501) staff       (20)     1106 2024-04-04 08:12:34.000000 itkdb_gtk-0.9.0/itkdb_gtk/__init__.py
--rw-r--r--   0 lacasta    (501) staff       (20)     6321 2024-04-01 19:22:49.000000 itkdb_gtk-0.9.0/itkdb_gtk/dashBoard.py
--rw-r--r--   0 lacasta    (501) staff       (20)    25071 2024-04-03 15:12:56.000000 itkdb_gtk-0.9.0/itkdb_gtk/dbGtkUtils.py
--rw-r--r--   0 lacasta    (501) staff       (20)    19394 2024-04-03 15:15:12.000000 itkdb_gtk-0.9.0/itkdb_gtk/readAVSdata.py
--rw-r--r--   0 lacasta    (501) staff       (20)     2673 2024-04-03 15:15:17.000000 itkdb_gtk-0.9.0/itkdb_gtk/readGoogleSheet.py
--rw-r--r--   0 lacasta    (501) staff       (20)      757 2024-04-03 15:15:24.000000 itkdb_gtk-0.9.0/itkdb_gtk/untrash_component.py
-drwxr-xr-x   0 lacasta    (501) staff       (20)        0 2024-04-04 08:12:35.517701 itkdb_gtk-0.9.0/itkdb_gtk.egg-info/
--rw-r--r--   0 lacasta    (501) staff       (20)     3148 2024-04-04 08:12:35.000000 itkdb_gtk-0.9.0/itkdb_gtk.egg-info/PKG-INFO
--rw-r--r--   0 lacasta    (501) staff       (20)      821 2024-04-04 08:12:35.000000 itkdb_gtk-0.9.0/itkdb_gtk.egg-info/SOURCES.txt
--rw-r--r--   0 lacasta    (501) staff       (20)        1 2024-04-04 08:12:35.000000 itkdb_gtk-0.9.0/itkdb_gtk.egg-info/dependency_links.txt
--rw-r--r--   0 lacasta    (501) staff       (20)      433 2024-04-04 08:12:35.000000 itkdb_gtk-0.9.0/itkdb_gtk.egg-info/entry_points.txt
--rw-r--r--   0 lacasta    (501) staff       (20)       83 2024-04-04 08:12:35.000000 itkdb_gtk-0.9.0/itkdb_gtk.egg-info/requires.txt
--rw-r--r--   0 lacasta    (501) staff       (20)       10 2024-04-04 08:12:35.000000 itkdb_gtk-0.9.0/itkdb_gtk.egg-info/top_level.txt
--rw-r--r--   0 lacasta    (501) staff       (20)     1320 2024-04-04 08:09:10.000000 itkdb_gtk-0.9.0/pyproject.toml
--rw-r--r--   0 lacasta    (501) staff       (20)       38 2024-04-04 08:12:35.518119 itkdb_gtk-0.9.0/setup.cfg
-drwxr-xr-x   0 lacasta    (501) staff       (20)        0 2024-04-04 08:12:35.517392 itkdb_gtk-0.9.0/test/
--rw-r--r--   0 lacasta    (501) staff       (20)     4165 2024-04-03 15:09:05.000000 itkdb_gtk-0.9.0/test/test_holes.py
+drwxr-xr-x   0 lacasta    (501) staff       (20)        0 2024-04-09 09:38:50.452700 itkdb_gtk-0.9.1.dev1/
+-rw-r--r--   0 lacasta    (501) staff       (20)     3153 2024-04-09 09:38:50.452495 itkdb_gtk-0.9.1.dev1/PKG-INFO
+-rw-r--r--   0 lacasta    (501) staff       (20)     2443 2024-04-01 19:21:18.000000 itkdb_gtk-0.9.1.dev1/README.md
+drwxr-xr-x   0 lacasta    (501) staff       (20)        0 2024-04-09 09:38:50.451031 itkdb_gtk-0.9.1.dev1/itkdb_gtk/
+-rw-r--r--   0 lacasta    (501) staff       (20)    13159 2024-04-03 15:10:25.000000 itkdb_gtk-0.9.1.dev1/itkdb_gtk/CreateShipments.py
+-rw-r--r--   0 lacasta    (501) staff       (20)    18761 2024-04-05 08:07:21.000000 itkdb_gtk-0.9.1.dev1/itkdb_gtk/GetShipments.py
+-rw-r--r--   0 lacasta    (501) staff       (20)    12272 2024-04-05 08:08:00.000000 itkdb_gtk-0.9.1.dev1/itkdb_gtk/GlueWeight.py
+-rw-r--r--   0 lacasta    (501) staff       (20)      172 2023-04-21 15:44:09.000000 itkdb_gtk-0.9.1.dev1/itkdb_gtk/ITkDB.desktop
+-rw-r--r--   0 lacasta    (501) staff       (20)    24242 2024-04-01 21:45:02.000000 itkdb_gtk-0.9.1.dev1/itkdb_gtk/ITkDB.svg
+-rw-r--r--   0 lacasta    (501) staff       (20)     9916 2024-04-03 15:11:28.000000 itkdb_gtk-0.9.1.dev1/itkdb_gtk/ITkDBlogin.py
+-rw-r--r--   0 lacasta    (501) staff       (20)    14861 2024-04-05 13:57:10.000000 itkdb_gtk-0.9.1.dev1/itkdb_gtk/ITkDButils.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     9273 2024-04-05 08:08:36.000000 itkdb_gtk-0.9.1.dev1/itkdb_gtk/PetalReceptionTests.py
+-rw-r--r--   0 lacasta    (501) staff       (20)    15458 2024-04-05 16:55:28.000000 itkdb_gtk-0.9.1.dev1/itkdb_gtk/SensorUtils.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     8407 2024-02-29 19:12:17.000000 itkdb_gtk-0.9.1.dev1/itkdb_gtk/ShowAttachments.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     3154 2024-02-29 19:16:49.000000 itkdb_gtk-0.9.1.dev1/itkdb_gtk/ShowComments.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     3533 2024-02-29 19:17:50.000000 itkdb_gtk-0.9.1.dev1/itkdb_gtk/ShowDefects.py
+-rw-r--r--   0 lacasta    (501) staff       (20)    17749 2024-04-09 06:55:51.000000 itkdb_gtk-0.9.1.dev1/itkdb_gtk/UploadModuleIV.py
+-rw-r--r--   0 lacasta    (501) staff       (20)    22142 2024-04-05 08:09:55.000000 itkdb_gtk-0.9.1.dev1/itkdb_gtk/UploadMultipleTests.py
+-rw-r--r--   0 lacasta    (501) staff       (20)    22194 2024-04-03 15:16:49.000000 itkdb_gtk-0.9.1.dev1/itkdb_gtk/UploadPetalInformation.py
+-rw-r--r--   0 lacasta    (501) staff       (20)    16645 2024-04-05 08:10:18.000000 itkdb_gtk-0.9.1.dev1/itkdb_gtk/UploadTest.py
+-rw-r--r--   0 lacasta    (501) staff       (20)    25761 2024-04-03 15:17:14.000000 itkdb_gtk-0.9.1.dev1/itkdb_gtk/WireBondGui.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     1155 2024-04-09 09:37:56.000000 itkdb_gtk-0.9.1.dev1/itkdb_gtk/__init__.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     6536 2024-04-05 10:12:43.000000 itkdb_gtk-0.9.1.dev1/itkdb_gtk/dashBoard.py
+-rw-r--r--   0 lacasta    (501) staff       (20)    25629 2024-04-05 16:57:04.000000 itkdb_gtk-0.9.1.dev1/itkdb_gtk/dbGtkUtils.py
+-rw-r--r--   0 lacasta    (501) staff       (20)    19394 2024-04-03 15:15:12.000000 itkdb_gtk-0.9.1.dev1/itkdb_gtk/readAVSdata.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     2673 2024-04-03 15:15:17.000000 itkdb_gtk-0.9.1.dev1/itkdb_gtk/readGoogleSheet.py
+-rw-r--r--   0 lacasta    (501) staff       (20)      757 2024-04-03 15:15:24.000000 itkdb_gtk-0.9.1.dev1/itkdb_gtk/untrash_component.py
+drwxr-xr-x   0 lacasta    (501) staff       (20)        0 2024-04-09 09:38:50.452278 itkdb_gtk-0.9.1.dev1/itkdb_gtk.egg-info/
+-rw-r--r--   0 lacasta    (501) staff       (20)     3153 2024-04-09 09:38:50.000000 itkdb_gtk-0.9.1.dev1/itkdb_gtk.egg-info/PKG-INFO
+-rw-r--r--   0 lacasta    (501) staff       (20)      873 2024-04-09 09:38:50.000000 itkdb_gtk-0.9.1.dev1/itkdb_gtk.egg-info/SOURCES.txt
+-rw-r--r--   0 lacasta    (501) staff       (20)        1 2024-04-09 09:38:50.000000 itkdb_gtk-0.9.1.dev1/itkdb_gtk.egg-info/dependency_links.txt
+-rw-r--r--   0 lacasta    (501) staff       (20)      445 2024-04-09 09:38:50.000000 itkdb_gtk-0.9.1.dev1/itkdb_gtk.egg-info/entry_points.txt
+-rw-r--r--   0 lacasta    (501) staff       (20)       83 2024-04-09 09:38:50.000000 itkdb_gtk-0.9.1.dev1/itkdb_gtk.egg-info/requires.txt
+-rw-r--r--   0 lacasta    (501) staff       (20)       10 2024-04-09 09:38:50.000000 itkdb_gtk-0.9.1.dev1/itkdb_gtk.egg-info/top_level.txt
+-rw-r--r--   0 lacasta    (501) staff       (20)     1337 2024-04-09 09:37:56.000000 itkdb_gtk-0.9.1.dev1/pyproject.toml
+-rw-r--r--   0 lacasta    (501) staff       (20)       38 2024-04-09 09:38:50.452743 itkdb_gtk-0.9.1.dev1/setup.cfg
+drwxr-xr-x   0 lacasta    (501) staff       (20)        0 2024-04-09 09:38:50.452002 itkdb_gtk-0.9.1.dev1/test/
+-rw-r--r--   0 lacasta    (501) staff       (20)      670 2024-04-08 18:30:41.000000 itkdb_gtk-0.9.1.dev1/test/testAnimated.py
+-rw-r--r--   0 lacasta    (501) staff       (20)     4165 2024-04-03 15:09:05.000000 itkdb_gtk-0.9.1.dev1/test/test_holes.py
```

### Comparing `itkdb_gtk-0.9.0/PKG-INFO` & `itkdb_gtk-0.9.1.dev1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itkdb_gtk
-Version: 0.9.0
+Version: 0.9.1.dev1
 Summary: A collection of Gtk based GUI to access ITkDB.
 Author-email: Carlos Lacasta <carlos.lacasta@cern.ch>
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `itkdb_gtk-0.9.0/README.md` & `itkdb_gtk-0.9.1.dev1/README.md`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.9.0/itkdb_gtk/CreateShipments.py` & `itkdb_gtk-0.9.1.dev1/itkdb_gtk/CreateShipments.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.9.0/itkdb_gtk/GetShipments.py` & `itkdb_gtk-0.9.1.dev1/itkdb_gtk/GetShipments.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # Check if Gtk can be open
 gtk_runs, gtk_args = Gtk.init_check()
 
 
 class ReceiveShipments(dbGtkUtils.ITkDBWindow):
     """Find shipments related to given recipient."""
 
-    def __init__(self, session, recipient="IFIC"):
+    def __init__(self, session, recipient="IFIC", help=None):
         """Initialization.
 
         Args:
             session: ITkDB session.
             recipient: default recipient
 
         """
@@ -40,15 +40,15 @@
         self.store = None
         self.shipments = {}
 
         global gtk_runs
         if gtk_runs:
             super().__init__(session=session, title="Upload AVS Data",
                              show_search="Cliick to search shipments",
-                             gtk_runs=gtk_runs)
+                             gtk_runs=gtk_runs, help=help)
 
             self.init_window()
 
     def init_window(self):
         """Initialize window."""
         #
         self.set_border_width(10)
```

### Comparing `itkdb_gtk-0.9.0/itkdb_gtk/GlueWeight.py` & `itkdb_gtk-0.9.1.dev1/itkdb_gtk/GlueWeight.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
     return data
 
 
 class GlueWeight(Gtk.Window):
     """Upluead Glue Weight test."""
 
-    def __init__(self, session, ifile=None):
+    def __init__(self, session, ifile=None, help=None):
         """Initialization.
     
         Args:
             session: ITkDB session_
             ifile (optional): Input file. Defaults to None.
 
         """
@@ -109,15 +109,15 @@
                 "FINISH_DATE": ITkDButils.get_db_date()
             }
         }
         self.skeleton = ITkDButils.get_test_skeleton(
             session, "MODULE", "GLUE_WEIGHT", defaults)
 
         if gtk_runs:
-            super().__init__(title="Upload AVS Data")
+            super().__init__(title="Upload Glue Weight", help=help)
             self.init_window()
 
     def init_window(self):
         """Initialize window."""
         #
         # Prepare HeaderBar
         hb = Gtk.HeaderBar()
```

### Comparing `itkdb_gtk-0.9.0/itkdb_gtk/GroundVITests.py` & `itkdb_gtk-0.9.1.dev1/itkdb_gtk/PetalReceptionTests.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,22 +30,23 @@
 
     except Exception:
         return None
 
     return None
 
 
-class GroundingTest(dbGtkUtils.ITkDBWindow):
+class PetalReceptionTests(dbGtkUtils.ITkDBWindow):
     """Dashboard class."""
 
-    def __init__(self, session):
+    def __init__(self, session, help=None):
         """Initialization."""
         super().__init__(title="ITkDB Dashboard",
                          session=session,
-                         show_search="Find object with given SN.")
+                         show_search="Find object with given SN.",
+                         help=help)
 
         # Members
         self.dbObject = None
 
         # action button in header
         button = Gtk.Button()
         icon = Gio.ThemedIcon(name="document-send-symbolic")
@@ -263,15 +264,15 @@
     if client is None:
         print("Could not connect to DB with provided credentials.")
         dlg.die()
         sys.exit()
 
     client.user_gui = dlg
 
-    gTest = GroundingTest(client)
+    gTest = PetalReceptionTests(client)
 
     gTest.present()
     gTest.connect("destroy", Gtk.main_quit)
     try:
         Gtk.main()
 
     except KeyboardInterrupt:
```

### Comparing `itkdb_gtk-0.9.0/itkdb_gtk/ITkDB.svg` & `itkdb_gtk-0.9.1.dev1/itkdb_gtk/ITkDB.svg`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.9.0/itkdb_gtk/ITkDBlogin.py` & `itkdb_gtk-0.9.1.dev1/itkdb_gtk/ITkDBlogin.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.9.0/itkdb_gtk/ITkDButils.py` & `itkdb_gtk-0.9.1.dev1/itkdb_gtk/ITkDButils.py`

 * *Files 0% similar despite different names*

```diff
@@ -275,15 +275,15 @@
 
         return None
 
     except Exception as e:
         return (str(e))
 
 
-def create_shipment(session, sender, recipient, items, name=None, send=False, 
+def create_shipment(session, sender, recipient, items, name=None, send=False,
                     type="domestic", attachment=None, comments=None):
     """Create a chipment.
 
     Args:
         session : The itkdb session
         sender : The sender ID
         recipient : The recipient ID
```

### Comparing `itkdb_gtk-0.9.0/itkdb_gtk/ShowAttachments.py` & `itkdb_gtk-0.9.1.dev1/itkdb_gtk/ShowAttachments.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.9.0/itkdb_gtk/ShowComments.py` & `itkdb_gtk-0.9.1.dev1/itkdb_gtk/ShowComments.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.9.0/itkdb_gtk/ShowDefects.py` & `itkdb_gtk-0.9.1.dev1/itkdb_gtk/ShowDefects.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.9.0/itkdb_gtk/UploadModuleIV.py` & `itkdb_gtk-0.9.1.dev1/itkdb_gtk/UploadModuleIV.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,285 +6,69 @@
 SENSOR_IV_Analysis.py in
 https://gitlab.cern.ch/atlas-itk/sw/db/production_database_scripts.git
 
 webApp aqui:
 https://itk-pdb-webapps-strips.web.cern.ch
 
 """
+import sys
 import os
 import json
-import warnings
+import tempfile
+import copy
 from pathlib import Path
 import shutil
 
-import gi
-import tempfile
-
-gi.require_version("Gtk", "3.0")
-from gi.repository import Gtk, Gio
-
-
 from matplotlib.backends.backend_gtk3agg import FigureCanvasGTK3Agg as FigureCanvas
 from matplotlib.backends.backend_gtk3 import NavigationToolbar2GTK3 as NavigationToolbar
 import numpy as np
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 
+import gi
+
+gi.require_version("Gtk", "3.0")
+from gi.repository import Gtk, Gio
+
 try:
     import itkdb_gtk
-    
+
 except ImportError:
-    import sys
-    from pathlib import Path
-    cwd = Path(sys.argv[0]).parent.parent
+    cwd = Path(__file__).parent.parent
     sys.path.append(cwd.as_posix())
 
-from itkdb_gtk import dbGtkUtils, ITkDBlogin, ITkDButils, UploadTest
+from itkdb_gtk import dbGtkUtils, ITkDBlogin, ITkDButils, UploadTest, SensorUtils
 
 # Check if Gtk can be open
 gtk_runs, gtk_args = Gtk.init_check()
 
 
 def remove_files(W, flist):
-    for f in flist:
-        os.unlink(f)
-
-
-#
-#   The following is taken from
-#   https://gitlab.cern.ch/atlas-itk/sw/db/production_database_scripts.git
-#
-mm = 1e-3
-cm = 1e-2
-UpperV = 500  # For sensor to pass, I must be < Imax up until this voltage and no breakdown must be detected before then.
-StabilityV = 700  # Voltage with multiple current readings to check stability
-
-AreaDict = {
-    "Unknown": (97.621 - 0.450) * (97.950 - 0.550) * mm * mm,
-    #
-    "ATLAS12": 95.7 * 95.64 * mm * mm,
-    "ATLAS17LS": (97.621 - 0.450) * (97.950 - 0.550) * mm * mm,
-    #
-    "ATLAS18R0": 89.9031 * cm * cm,
-    "ATLAS18R1": 89.0575 * cm * cm,
-    "ATLAS18R2": 74.1855 * cm * cm,
-    "ATLAS18R3": 80.1679 * cm * cm,
-    "ATLAS18R4": 87.4507 * cm * cm,
-    "ATLAS18R5": 91.1268 * cm * cm,
-    #
-    "ATLAS18SS": 93.6269 * cm * cm,
-    "ATLAS18LS": 93.6269 * cm * cm,
-    #
-    "ATLASDUMMY18": (97.621 - 0.450) * (97.950 - 0.550) * mm * mm,
-}
-
-
-def LocateMicroDischarge(
-    I,
-    V,
-    sm_window=2,
-    bd_limit=5.5,
-    allow_running_bd=True,
-    use_additional_cond=False,
-    tolerence=0.05,
-    voltage_span=4,
-    fit_window=5,
-):
-    """
-    Function for BDV estimation - if questions please contact Vera Latonova (vera.latonova@cern.ch).
-    I,V must have same shape and voltages must be in ascending order,
-    same indexes of I&V arrays must correspond each other,
-    only invalid data or holdstep should be stripped before
-    but it is not necessary. Measurments U=0&I=0 are removed.
-    If there is same or higher amount of same voltages in row than
-    sm_window, from this sequence we cannot estimete dI/dV and
-    we have to remove this averaged point.
-
-    It is assumed that only parameter use_additional_cond would be
-    changed by caller. Changing of other parameters may affect
-    BDV unexpectedly.
-
-
-    @param[in] I                   - array of currents without any cut
-    @param[in] V                   - array of voltages, ascending order, without any cut
-    @param[in] sm_window           - size of smoothing window
-    @param[in] bd_limit            - BD limit for |U| < 500V
-    @param[in] allow_running_bd    - allow increase bd_limit for |U| > 500
-    @param[in] use_additional_cond - use additional BD contition
-    @param[in] tolerence           - configuration of additional condition
-    @param[in] voltage_span        - max width of hump on spectra which may be neglected
-                                     in voltage steps in additional contition
-    @param[in] fit_window          - number of points used for linear fit before BD voltage
-
-    @return BD voltage (always positive) or NO_BD_CONST = 9.99e99 if not found.
-    """
-    NO_BD_CONST = 9.99e99
-
-    # add nan to the end of array
-    V = np.abs(V)
-    I = np.abs(I)
-
-    # skip zeros
-    ind = np.where(np.logical_or(I != 0, V != 0))
-    V = V[ind]
-    I = I[ind]
-
-    V_ = np.append(V, np.nan * np.ones(sm_window - 1))
-    I_ = np.append(I, np.nan * np.ones(sm_window - 1))
-
-    # make 2D array of I's, V's each row_ind shifted by row_ind index
-    # i.e from array [1,3,5] we make (for sm_window=2) 2D array
-    # [  1,3,5,nan]
-    # [nan,5,1,3]
-    # than get average from each column -> I_avg, V_avg
-    r = np.arange(sm_window)
-
-    V2 = np.outer(np.ones(sm_window), V_)
-    row_ind, col_ind = np.ogrid[: V2.shape[0], : V2.shape[1]]
-    col_ind = col_ind - r[:, np.newaxis]
-    V2 = V2[row_ind, col_ind]
-    # strip fields with nans
-    V2 = np.transpose(V2[:, (sm_window - 1) : -(sm_window - 1)])
-
-    I2 = np.outer(np.ones(sm_window), I_)
-    row_ind, col_ind = np.ogrid[: I2.shape[0], : I2.shape[1]]
-    col_ind = col_ind - r[:, np.newaxis]
-    I2 = I2[row_ind, col_ind]
-    I2 = np.transpose(I2[:, (sm_window - 1) : -(sm_window - 1)])
-
-    # get V & I averages
-    try:
-        V_avg = np.average(V2, axis=1)
-        I_avg = np.average(I2, axis=1)
-    except ZeroDivisionError:
-        # not enough data
-        return NO_BD_CONST
-
-    # find dI / dV array
-    # I'm not able to write this without cycle
-    dIdV = np.array([])
-    for i in range(V2.shape[0]):
-        with warnings.catch_warnings():
-            warnings.filterwarnings("error")
-            try:
-                dIdV = np.append(dIdV, np.polyfit(V2[i, :], I2[i, :], 1)[0])
-            except (np.RankWarning, TypeError):
-                dIdV = np.append(dIdV, np.nan)
-
-    # stripping U[n] == U[n+1] (i.e. hodlsetp) => fit cannot be sucessful =>
-    # dIdV is nan @holdstep
-    ind = np.where(np.isfinite(dIdV))
-    I_avg = I_avg[ind]
-    V_avg = V_avg[ind]
-    dIdV = dIdV[ind]
-
-    # get running BDV limit & compare
-    bd_limit_running = bd_limit + np.where(
-        allow_running_bd and V_avg > 500, (V_avg - 500.0) / 100.0, 0
-    )
-    V_avg_BD_ind = dIdV / (I_avg / V_avg) > bd_limit_running
-    V_avg_BD = V_avg[V_avg_BD_ind]
-
-    # Estimate BDV
-    BDV = np.array([])
-
-    # no break-down
-    if V_avg_BD.shape == (0,):
-        return NO_BD_CONST
-
-    # if V_avg_BD_ind[0] == True ... BDV <- V[0]
-    # for others V_avg_BD_ind[n] == True BDV <- (V_avg[n] + V_avg[n-1])/2
-    if V_avg_BD_ind[0]:
-        BDV = np.append(BDV, V[0])
-    V_avg_BD_ind[0] = False
-
-    BDV = np.append(
-        BDV,
-        (V_avg[np.where(V_avg_BD_ind)] + V_avg[np.where(V_avg_BD_ind)[0] - 1]) / 2.0,
-    )
-
-    ###########################################################################
-    ## Application of additional condition ####################################
-    ###########################################################################
-    if not use_additional_cond:
-        return BDV[0]
-
-    # get index if V <= BDV
-    B = np.where(np.less.outer(BDV, V))
-    col_ind = np.mgrid[: BDV.shape[0], : V.shape[0]][1]
-    col_ind[B[0], B[1]] = 0
-    V_BDV_ind = np.max(col_ind, axis=1)
-
-    back_ok_v_ind = 0
-    while True:
-        with warnings.catch_warnings():
-            warnings.filterwarnings("error")
-            try:
-                a, b = np.polyfit(
-                    V[
-                        max(back_ok_v_ind, V_BDV_ind[0] - fit_window) : max(
-                            back_ok_v_ind, V_BDV_ind[0]
-                        )
-                    ],
-                    I[
-                        max(back_ok_v_ind, V_BDV_ind[0] - fit_window) : max(
-                            back_ok_v_ind, V_BDV_ind[0]
-                        )
-                    ],
-                    1,
-                )
-            except (np.RankWarning, TypeError):
-                return BDV[0]
-
-        ind = np.where(1 - (a * V + b) / I <= tolerence)[0]
-        try:
-            back_ok_v_ind = np.min(ind[ind > V_BDV_ind[0] + 1])
-        except ValueError:
-            # sensor is not going back
-            return BDV[0]
-        # hump is too long -- it cannot be skipped
-        if back_ok_v_ind - V_BDV_ind[0] > voltage_span:
-            return BDV[0]
-
-        # skip BDVs inside hump
-        ind = BDV >= V[back_ok_v_ind]
-        BDV = BDV[ind]
-        V_BDV_ind = V_BDV_ind[ind]
-        if V_avg_BD.shape == (0,):
-            return NO_BD_CONST
-    return NO_BD_CONST
-
-
-def scale_iv(I, T1, T2):
-    """Normalize corrent  to given temperature (T2)
+    """Remove files given in the input list.
 
     Args:
-        I (array): Current
-        T1 (float): Original temperature
-        T2 (float): New temperature.
-
-    Return:
-        Array with scaled currents.
+        flist (list): list of filenames.
 
     """
-    factor = (T2 / T1) ** 2 * np.exp((-1.21 / 8.62) * (1 / T2 - 1 / T1))
-    return factor * I
+    for f in flist:
+        os.unlink(f)
 
 
 class IVwindow(dbGtkUtils.ITkDBWindow):
     """GUI for IV file handling."""
 
-    def __init__(self, session, title="IV window", options=None):
+    def __init__(self, session, title="IV window", options=None, help=help):
         """Initialization."""
         super().__init__(
-            session=session, title=title, show_search=None, gtk_runs=gtk_runs
+            session=session, title=title, show_search=None, gtk_runs=gtk_runs, help=help
         )
         self.mdata = {}
         self.mod_type = {}
         self.mod_SN = {}
+        self.last_folder = None
         self.difference = None
         self.canvas = None
 
         self.init_window()
 
     def init_window(self):
         """Prepare the Gtk window."""
@@ -300,15 +84,15 @@
 
         # Button to upload
         button = Gtk.Button()
         icon = Gio.ThemedIcon(name="document-send-symbolic")
         image = Gtk.Image.new_from_gicon(icon, Gtk.IconSize.BUTTON)
         button.add(image)
         button.set_tooltip_text("Click to upload test")
-        button.connect("clicked", self.upload_test)
+        button.connect("clicked", self.do_upload)
         self.hb.pack_end(button)
 
         # File entry and search button
         self.single_file = Gtk.FileChooserButton()
         self.single_file.connect("file-set", self.on_single_file_set)
 
         self.double_file = Gtk.FileChooserButton()
@@ -326,20 +110,20 @@
         grid.attach(self.single_file, 1, 1, 1, 1)
         grid.attach(self.single_SN, 2, 1, 1, 1)
 
         grid.attach(Gtk.Label(label="Double Data File"), 0, 2, 1, 1)
         grid.attach(self.double_file, 1, 2, 1, 1)
         grid.attach(self.double_SN, 2, 2, 1, 1)
 
-        btn = Gtk.Button(label="Compute difference")
-        btn.connect("clicked", self.on_difference)
-        grid.attach(btn, 1, 3, 1, 1)
+        #btn = Gtk.Button(label="Compute difference")
+        #btn.connect("clicked", self.on_difference)
+        #grid.attach(btn, 1, 3, 1, 1)
 
         btn = Gtk.Button(label="Upload to DB")
-        btn.connect("clicked", self.upload_test)
+        btn.connect("clicked", self.do_upload)
         grid.attach(btn, 2, 3, 1, 1)
 
         self.mainBox.pack_start(grid, False, True, 0)
 
         self.fig = mpl.figure.Figure()
         self.fig.tight_layout()
         sw = Gtk.ScrolledWindow()  # Gtk.Box(orientation=Gtk.Orientation.VERTICAL)
@@ -354,253 +138,207 @@
         self.mainBox.pack_start(sw, True, True, 0)
 
         # Create toolbar
         try:
             toolbar = NavigationToolbar(self.canvas)
         except TypeError:
             toolbar = NavigationToolbar(self.canvas, self)
-            
+
         self.mainBox.pack_start(toolbar, False, False, 0)
 
         # The text view
         self.mainBox.pack_start(self.message_panel.frame, True, True, 5)
 
         self.show_all()
 
-    def upload_test(self, *args):
+    def get_difference_data(self):
+        """Returns the double data witht the difference."""
+        # Prepare the data
+        ddata = copy.deepcopy(self.mdata["double"])
+
+        ndata = len(self.difference)
+        ddata["curve"]["V"] = np.abs(ddata["curve"]["V"][:ndata])
+        ddata["curve"]["I"] = np.abs(self.difference)
+        ddata["curve"]["S"] = ddata["curve"]["S"][:ndata]
+        return ddata
+
+    def upload_test(self, mdata, mod_type):
         """Upload available tests."""
-        try:
-            mdata = self.mdata["double"]
-        except KeyError:
-            dbGtkUtils.complain("Cannot Upload to DB", "Data not yet ready.")
-            return
 
-        # Check if we are dealing with sensors or modules
-        is_module = "Module_SN" in mdata
+        # Get JSon skeleton filled
+        test = SensorUtils.sensor_data_to_json(self.session, mdata, mod_type, self)
 
-        if is_module:
-            test = ITkDButils.get_test_skeleton(
-                self.session, "MODULE", self.mdata["double"]["TestType"]
-            )
-            tp = "ATLAS18{}".format(self.mod_type["double"][0:2])
-            area = AreaDict[tp] / cm**2
+        # write attachment.
+        # First geet the fine name.
+        fnam = SensorUtils.build_file_name(mdata)
 
-        else:
-            test = ITkDButils.get_test_skeleton(
-                self.session, "SENSOR", self.mdata["double"]["TestType"]
-            )
-            area = AreaDict[self.mod_type["double"]] / cm**2
 
-        # The data arrays
-        V = np.abs(mdata["curve"]["V"])
-        I = np.abs(mdata["curve"]["I"])
-        passed = True
-
-        # Find Current @ 500V
-        indx = np.where(V == 500)[0]
-        i_500 = I[indx][0] / area
-        self.write_message("I @ 500V = {:.2f} nA/cm2\n".format(i_500))
-
-        # Compute current stability
-        IStability = abs(I[abs(V) == StabilityV])
-        IVariation = -1
-        if np.size(IStability) > 1:  # Maybe make == 4?
-            IVariation = abs(np.std(IStability) / np.mean(IStability))
-
-        self.write_message("I stability = {:.6f} nA\n".format(IVariation))
-
-        # Search for Micro discharges
-        # Check for micro-discharge in non-normalized current,
-        # removing duplicate Voltage entries (e.g. for stability measurements)
-        comments = []
-        defects = []
-        UniqueVs, UniqueIndices = np.unique(V, return_index=True)
-        MicroDischargeV = LocateMicroDischarge(I[UniqueIndices], UniqueVs)
-        if MicroDischargeV < np.max(V):
-            comments.append("Found micro discharge: {:.1f} V\n".format(MicroDischargeV))
-            self.write_message(comments[-1])
-
-            if MicroDischargeV < UpperV:
-                txt = "microdischarge happening before {:.1f}V.".format(UpperV)
-                defects.append({
-                            "name": "MicroDischarge",
-                            "description": txt,
-                            "properties": {}
-                        }
-                )
-                self.write_message("...{}. FAILED\n".format(txt))
-                passed = False
+        data_out = tempfile.NamedTemporaryFile("w", prefix=fnam, suffix=".dat", delete=False)
+        SensorUtils.save_sensor_data(data_out, mdata, name=fnam)
 
-        test["component"] = self.mod_SN["double"]
-        test["institution"] = mdata["Institute"]
-        test["runNumber"] = mdata["RunNumber"]
-        test["date"] = ITkDButils.get_db_date(
-            "{} {}".format(mdata["Date"], mdata["Time"])
-        )
-        test["passed"] = passed
-        test["problems"] = False
-        test["properties"]["VBIAS_SMU"] = mdata["Vbias_SMU"]
-        test["properties"]["RSERIES"] = mdata["Rseries"]
-        test["properties"]["TEST_DMM"] = mdata["Test_DMM"]
-        test["properties"]["RSHUNT"] = mdata["Rshunt"]
-        test["properties"]["RUNNUMBER"] = mdata["RunNumber"]
-        test["properties"]["COMMENTS"] = mdata["Comments"]
-        test["properties"]["ALGORITHM_VERSION"] = "0.0.0"
-        if is_module:
-            test["properties"]["SOFTWARE_TYPE_VERSION"] = "pyProbe"
-            test["properties"]["MODULE_STAGE"] = mdata["Module_Stage"]
-
-        test["results"]["TEMPERATURE"] = mdata["Temperature"]
-        test["results"]["HUMIDITY"] = mdata["Humidity"]
-        test["results"]["VBD"] = MicroDischargeV
-        test["results"]["I_500V"] = i_500
-        test["results"]["VOLTAGE"] = -np.abs(V)
-        test["results"]["CURRENT"] = -np.abs(I)
-        test["results"]["RMS_STABILITY"] = IVariation
-        test["results"]["SHUNT_VOLTAGE"] = np.zeros(V.shape)
-        test["defects"] = defects
-        test["comments"] = comments
+        js_out = tempfile.NamedTemporaryFile("w", prefix="payload-", suffix=".json", delete=False)
+        js_out.write(json.dumps(test, indent=3, cls=dbGtkUtils.MyEncoder))
+        js_out.close()
 
-        # write attachment.
-        if is_module:
-            items = [
-                "Type",
-                "Wafer",
-                "Module_SN",
-                "Module_Stage",
-                "Date",
-                "Time",
-                "Institute",
-                "TestType",
-                "Vbias_SMU",
-                "Rseries",
-                "Test_DMM",
-                "Rshunt",
-                "Software type and version, fw version",
-                "RunNumber",
-                "Temperature",
-                "Humidity",
-                "Comments",
-            ]
-        else:
-            items = [
-                "Type",
-                "Batch",
-                "Wafer",
-                "Component",
-                "Date",
-                "Time",
-                "Institute",
-                "TestType",
-                "Vbias_SMU",
-                "Rseries",
-                "Test_DMM",
-                "Rshunt",
-                "RunNumber",
-                "Temperature",
-                "Humidity",
-                "Comments",
-            ]
+        attachment = ITkDButils.Attachment(data_out.name, "resultsFile", fnam)
+        uploadW = UploadTest.UploadTest(self.session, js_out.name, attachment)
+        uploadW.connect("destroy", remove_files, [data_out.name, js_out.name])
 
-        try:
-            fnam = "{}_{}_IV_{}-".format(
-                self.mod_SN["double"], mdata["Module_Stage"], mdata["RunNumber"]
-            )
-        except KeyError:
-            fnam = "{}_W_IV_{}".format(self.mod_SN["double"], mdata["RunNumber"])
 
-        data_out = tempfile.NamedTemporaryFile(
-            "w", prefix=fnam, suffix=".dat", delete=False
-        )
-        data_out.write("{}\n".format(fnam))
-        for key in items:
-            if key == "Module_SN" or key == "Component":
-                data_out.write("{}: {}\n".format(key, self.mod_SN["double"]))
-            else:
-                data_out.write("{}: {}\n".format(key, mdata[key]))
-
-        for il, label in enumerate(mdata["curve"]["labels"]):
-            if il:
-                data_out.write("\t")
-            data_out.write(label)
-        data_out.write("\n")
+    def do_upload(self, *args):
+        """The upload button has been clicked.
 
-        ncol = len(mdata["curve"]["labels"])
-        ndata = len(self.difference)
-        for i in range(ndata):
-            v = -abs(V[i])
-            iv = -abs(self.difference[i])
-            if ncol > 2:
-                data_out.write("{:.2f}\t{:.2f}\t{:.2f}\n".format(v, iv, 0.0))
-            else:
-                data_out.write("{:.2f}\t{:.2f}\n".format(v, iv))
+        We present a dialog where we ask if the new data file should be stored
+        locally and if both (single and difference) tests should be uploaded.
+        """
+        if "single" not in self.mdata:
+            return
 
-        print(data_out.name)
-        data_out.close()
+        if "double" not in self.mdata:
+            # upload only the single test.
+            if dbGtkUtils.ask_for_confirmation(
+                "Uploading Single data",
+                "No data for double module/sensor.\nUpload single test ?."):
 
-        js_out = tempfile.NamedTemporaryFile(
-            "w", prefix="payload-", suffix=".json", delete=False
-        )
-        js_out.write(json.dumps(test, indent=3, cls=dbGtkUtils.MyEncoder))
-        js_out.close()
+                self.upload_test(self.mdata["single"], self.mod_type["single"])
 
-        if dbGtkUtils.ask_for_confirmation("Save Data File locally?", "Saves attached file also locally."):
+            return
+
+        # We create the dialog.
+        dlg = Gtk.Dialog(title="Add Attachment", parent=self, flags=0)
+        dlg.add_buttons(Gtk.STOCK_CANCEL, Gtk.ResponseType.CANCEL,
+                    Gtk.STOCK_OK, Gtk.ResponseType.OK)
+        area = dlg.get_content_area()
+        grid = Gtk.Grid(column_spacing=5, row_spacing=1)
+        area.add(grid)
+
+        label = Gtk.Label(label="Save locally new data file ?")
+        save_locally = Gtk.Switch()
+        grid.attach(label, 0, 0, 1, 1)
+        grid.attach(save_locally, 1, 0, 1, 1)
+
+        label = Gtk.Label(label="Upload both tests ?")
+        do_both = Gtk.Switch()
+        grid.attach(label, 0, 1, 1, 1)
+        grid.attach(do_both, 1, 1, 1, 1)
+
+        dlg.show_all()
+        rc = dlg.run()
+        dlg.hide()
+        if rc != Gtk.ResponseType.OK:
+            dlg.destroy()
+            return
+
+        mdata = self.get_difference_data()
+        if save_locally.get_active():
+            # Save locally.
+            fnam = SensorUtils.build_file_name(mdata)
             fc = Gtk.FileChooserDialog(title="Save data file", action=Gtk.FileChooserAction.SAVE)
             fc.add_buttons(
                 Gtk.STOCK_CANCEL,
                 Gtk.ResponseType.CANCEL,
                 Gtk.STOCK_OPEN,
                 Gtk.ResponseType.OK,
             )
 
+            if self.last_folder:
+                fc.set_current_folder(self.last_folder)
+
             fc.set_current_name("{}.dat".format(fnam))
             rc = fc.run()
             if rc == Gtk.ResponseType.OK:
-                shutil.copyfile(data_out.name, fc.get_filename())
-
+                SensorUtils.save_sensor_data(fc.get_filename(), mdata)
+                
             fc.hide()
             fc.destroy()
 
-        attachment = ITkDButils.Attachment(data_out.name, "resultsFile", fnam)
-        uploadW = UploadTest.UploadTest(self.session, js_out.name, attachment)
-        uploadW.connect("destroy", remove_files, [data_out.name, js_out.name])
+        # Upload double
+        self.upload_test(mdata, self.mod_type["double"])
+
+        if do_both.get_active():
+            self.upload_test(self.mdata["single"], self.mod_type["single"])
+            
+        dlg.destroy()
 
     def on_refresh(self, *args):
         """Refresh canvas."""
         if self.fig and self.canvas:
             self.fig.tight_layout()
             self.canvas.draw()
 
     def find_module(self, SN):
         """Find module (SN) on database
 
         Args:
             SN (str): Module Serial number.
-            
+
         """
         md = ITkDButils.get_DB_component(self.session, SN)
         if md is None:
             dbGtkUtils.complain(
                 "Could not find {}".format(SN), str(ITkDButils.get_db_response())
             )
 
         return md
 
+    def update_folder(self, fnam):
+        """Sets last folder."""
+
+        self.last_folder = Path(fnam).parent.as_posix()
+        self.single_file.set_current_folder(self.last_folder)
+        self.double_file.set_current_folder(self.last_folder)
+
+    def show_single_curve(self):
+        """Shows the single curve."""
+        try:
+            mdata = self.mdata["single"]
+        except KeyError:
+            return
+
+        is_module = is_module = "Module_SN" in mdata
+
+        self.show_curve(
+            131,
+            mdata["curve"]["V"],
+            mdata["curve"]["I"],
+            self.mod_type["single"][0:4] if is_module else "Single",
+            mdata["curve"]["labels"][0],
+            mdata["curve"]["labels"][1],
+        )
+
+    def show_double_curve(self):
+        """Shows the double curve."""
+        try:
+            mdata = self.mdata["double"]
+        except KeyError:
+            return
+
+        self.show_curve(
+            133,
+            mdata["curve"]["V"],
+            mdata["curve"]["I"],
+            "Double",
+            mdata["curve"]["labels"][0],
+            None,
+        )
+
     def on_single_file_set(self, *args):
-        """File chosen."""
+        """Single sensor file chosen."""
         obj_type = ["sensor", "module"]
         fnam = self.single_file.get_filename()
         if fnam is None or not Path(fnam).exists():
             dbGtkUtils.complain("Could not find data file", fnam, parent=self)
 
-        mdata = self.read_file(fnam)
+        mdata = SensorUtils.read_sensor_file(fnam)
+        self.update_folder(fnam)
 
         is_module = 1
         try:
             SN = mdata["Module_SN"]
+
         except KeyError:
             SN = mdata["Component"]
             is_module = 0
 
         self.write_message("Reading data for {} {}\n".format(obj_type[is_module], SN))
         md = self.find_module(SN)
         if md is None:
@@ -612,64 +350,54 @@
         self.mod_SN["single"] = SN
         self.mdata["single"] = mdata
         self.mod_type["single"] = md["type"]["code"]
         print(self.mod_type["single"])
 
         self.single_SN.set_text("{} - {}".format(SN, md["type"]["name"]))
         self.fig.clf()
-        self.show_curve(
-            131,
-            mdata["curve"]["V"],
-            mdata["curve"]["I"],
-            self.mod_type["single"][0:4] if is_module else "Single",
-            mdata["curve"]["labels"][0],
-            mdata["curve"]["labels"][1],
-        )
+        self.show_single_curve()
 
-    def on_double_file_set(self, *args):
-        "File chosen for the 'double module'"
-        obj_type = ["sensor", "module"]
-        fnam = self.double_file.get_filename()
-        if fnam is None or not Path(fnam).exists():
-            dbGtkUtils.complain("Could not find data file", fnam, parent=self)
-
-        mdata = self.read_file(fnam)
-        is_module = 1
-        # Check SN in data file
-        try:
-            SN = mdata["Module_SN"]
-        except KeyError:
-            is_module = 0
-            SN = mdata["Component"]
+        # Compute difference if single already available
+        if "double" in self.mdata:
+            self.show_double_curve()
+            self.on_difference()
 
-        halfM_SN = SN
+    def check_double_SN(self, SN, is_module):
+        """Check that the double SN is a good one."""
+        obj_type = ["sensor", "module"]
         if "single" in self.mod_SN:
             if self.mod_SN["single"] == SN:
                 dbGtkUtils.complain(
-                    "Wrong {}} SN", "{} already used.".format(obj_type[is_module], SN)
+                    "Wrong SN {}".format(SN),
+                    "{} already used.".format(obj_type[is_module])
                 )
                 self.double_file.unselect_all()
-                return
+                return None
 
         # Check that it exists in the DB
         if len(SN) != 14 or SN[0:4] != "20US":
             self.write_message("Invalid SN: {}\n".format(SN))
             SN = dbGtkUtils.get_a_value(
                 "Invalid SN", "Give Ring or corresponding Half Module SN"
             )
+            return None
 
-        self.write_message("Reading data for module {}\n".format(SN))
         md = self.find_module(SN)
         if md is None:
             self.write_message("...object does not exist.\n")
             self.double_file.unselect_all()
-            return
+            return None
 
+        return md
+
+    def get_true_SN(self, md):
+        """Get the actual SN of the 'double' object."""
         found_child = False
-        if md["type"]["name"].find("Ring") >= 0:
+        has_ring = md["type"]["name"].find("Ring")
+        if has_ring >= 0:
             self.write_message("...This is a Ring module. Searching children in DB\n")
             for child in md["children"]:
                 if child["component"]:
                     ctype = child["type"]["code"]
                     if ctype.find("MODULE") < 0:
                         continue
 
@@ -691,17 +419,47 @@
             md = ITkDButils.get_DB_component(self.session, halfM_SN)
             if md is None:
                 dbGtkUtils.complain(
                     "Could not find {}".format(halfM_SN),
                     str(ITkDButils.get_db_response()),
                 )
                 self.double_file.unselect_all()
-                return
+                return None
 
             self.write_message("... {}\n".format(halfM_SN))
+            return halfM_SN
+
+        return md["serialNumber"]
+
+    def on_double_file_set(self, *args):
+        "File chosen for the 'double module'"
+        obj_type = ["sensor", "module"]
+        fnam = self.double_file.get_filename()
+        if fnam is None or not Path(fnam).exists():
+            dbGtkUtils.complain("Could not find data file", fnam, parent=self)
+
+        mdata = SensorUtils.read_sensor_file(fnam)
+        self.update_folder(fnam)
+        is_module = 1
+        # Check SN in data file
+        try:
+            SN = mdata["Module_SN"]
+        except KeyError:
+            is_module = 0
+            SN = mdata["Component"]
+
+        halfM_SN = SN
+        md = self.check_double_SN(SN, is_module)
+        if md is None:
+            return
+
+        self.write_message("Reading data for {} {}\n".format(obj_type[is_module], SN))
+        halfM_SN = self.get_true_SN(md)
+        if halfM_SN is None:
+            return
 
         if "single" in self.mod_type:
             if is_module and self.mod_type["single"] == md["type"]["code"]:
                 dbGtkUtils.complain(
                     "Wrong module type.",
                     "Module type cannot be {}".format(self.mod_type["single"]),
                 )
@@ -710,22 +468,15 @@
                 return
 
         self.mod_SN["double"] = halfM_SN
         self.mod_type["double"] = md["type"]["code"]
         self.mdata["double"] = mdata
 
         self.double_SN.set_text("{} - {}".format(halfM_SN, md["type"]["name"]))
-        self.show_curve(
-            133,
-            mdata["curve"]["V"],
-            mdata["curve"]["I"],
-            "Double",
-            mdata["curve"]["labels"][0],
-            None,
-        )
+        self.show_double_curve()
 
         # Compute difference if single already available
         if "single" in self.mdata:
             self.on_difference()
 
     def on_difference(self, *args):
         """Compute difference."""
@@ -733,15 +484,15 @@
             dbGtkUtils.complain(
                 "Data needed", "Check if single oand doubel module data are available"
             )
             return
 
         is_module = "Module_SN" in self.mdata["double"]
         double_I = self.mdata["double"]["curve"]["I"]
-        single_I = scale_iv(
+        single_I = SensorUtils.scale_iv(
             self.mdata["single"]["curve"]["I"],
             self.mdata["single"]["Temperature"] + 273.0,
             self.mdata["double"]["Temperature"] + 273.0,
         )
 
         try:
             nmin = double_I.size
@@ -777,59 +528,17 @@
         if title:
             ax.set_title(title)
 
         ax.plot(X, Y)
         ax.grid()
         self.on_refresh()
 
-    @staticmethod
-    def read_file(fnam):
-        """Read a data file. Return dictionary with all teh data."""
-        labels = []
-        metadata = {}
-        with open(fnam, "r", encoding="utf-8") as ifile:
-            first = True
-            for line in ifile:
-                if first:
-                    first = False
-                    ipos = line.rfind(".")
-                    metadata["fname"] = line[:ipos]
-                    continue
-
-                if line.find("Voltage [V]") >= 0 or line.find("Voltage[V]") >= 0:
-                    labels = line.split("\t")
-                    break
-
-                rc = line.find(":")
-                if rc >= 0:
-                    key = line[:rc].strip()
-                    val = line[rc + 1 :].strip()
-                    if key in ["Temperature", "Humidity"]:
-                        metadata[key] = float(val)
-                    else:
-                        metadata[key] = val
-
-            V = []
-            I = []
-            for line in ifile:
-                data = [float(s) for s in line.split()]
-                V.append(data[0])
-                I.append(data[1])
-
-            metadata["curve"] = {
-                "V": np.abs(np.array(V)),
-                "I": np.abs(np.array(I)),
-                "labels": labels[0:2],
-            }
-            return metadata
-
 
 def main():
     """Main entryy."""
-    import sys
 
     # DB login
     dlg = ITkDBlogin.ITkDBlogin()
     client = dlg.get_client()
     if client is None:
         print("Could not connect to DB with provided credentials.")
         dlg.die()
```

### Comparing `itkdb_gtk-0.9.0/itkdb_gtk/UploadMultipleTests.py` & `itkdb_gtk-0.9.1.dev1/itkdb_gtk/UploadMultipleTests.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,22 +99,22 @@
 
     return errors, missing
 
 
 class UploadMultipleTests(dbGtkUtils.ITkDBWindow):
     """Collects information to upload a test and its attachments."""
 
-    def __init__(self, session):
+    def __init__(self, session, help=help):
         """Initialization.
 
         Args:
             session: ITkDB session
 
         """
-        super().__init__(session=session, title="Upload Tests", gtk_runs=gtk_runs)
+        super().__init__(session=session, title="Upload Tests", gtk_runs=gtk_runs, help=help)
         self.tests = []
 
         self.init_window()
 
     def init_window(self):
         """Creates the Gtk window."""
         # Initial tweaks
```

### Comparing `itkdb_gtk-0.9.0/itkdb_gtk/UploadPetalInformation.py` & `itkdb_gtk-0.9.1.dev1/itkdb_gtk/UploadPetalInformation.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.9.0/itkdb_gtk/UploadTest.py` & `itkdb_gtk-0.9.1.dev1/itkdb_gtk/UploadTest.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
     return errors, missing
 
 
 class UploadTest(dbGtkUtils.ITkDBWindow):
     """Collects information to upload a test and its attachments."""
 
-    def __init__(self, session, payload=None, attachment=None):
+    def __init__(self, session, payload=None, attachment=None, help=None):
         """Initialization.
 
         Args:
             session: ITkDB session
             payload: path of test file
             attachment: an Attachment object or list of attachments.
 
@@ -103,15 +103,15 @@
                         self.attachments.append(att)
 
                 except TypeError:
                     print("Wrong attachment: {}".format(attachment))
 
         global gtk_runs
         if gtk_runs:
-            super().__init__(session=session, title="Upload Test", gtk_runs=gtk_runs)
+            super().__init__(session=session, title="Upload Test", gtk_runs=gtk_runs, help=help)
             self.init_window()
 
     def init_window(self):
         """Creates the Gtk window."""
         # Initial tweaks
         self.set_border_width(10)
 
@@ -349,15 +349,17 @@
             self.data = value.values
 
         dlg.hide()
         dlg.destroy()
 
     def find_attachments(self):
         """Find Attachments in payload."""
-        self.attachments = []
+        # We used to clean the attachmetns, but this would remove the ones given
+        # in the contructor.
+        # self.attachments = []
         if "attachments" in self.data:
             for A in self.data["attachments"]:
                 if not Path(A["path"]).exists():
                     if self.folder:
                         the_path = self.folder.joinpath(A["path"])
                     else:
                         continue
```

### Comparing `itkdb_gtk-0.9.0/itkdb_gtk/WireBondGui.py` & `itkdb_gtk-0.9.1.dev1/itkdb_gtk/WireBondGui.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.9.0/itkdb_gtk/dashBoard.py` & `itkdb_gtk-0.9.1.dev1/itkdb_gtk/dashBoard.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,43 +9,44 @@
     from pathlib import Path
     cwd = Path(sys.argv[0]).parent.parent
     sys.path.append(cwd.as_posix())
     
     
 from itkdb_gtk import dbGtkUtils
 from itkdb_gtk import GetShipments
-from itkdb_gtk import GroundVITests
+from itkdb_gtk import PetalReceptionTests
 from itkdb_gtk import ITkDBlogin
 from itkdb_gtk import CreateShipments
 from itkdb_gtk import UploadTest
 from itkdb_gtk import UploadMultipleTests
 from itkdb_gtk import GlueWeight
 from itkdb_gtk import UploadModuleIV
 from itkdb_gtk import WireBondGui
 
 import gi
 
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk
 
+HELP_LINK="https://itkdb-gtk.docs.cern.ch"
 
 class DashWindow(dbGtkUtils.ITkDBWindow):
     """Dashboard class."""
     UPLOAD_TEST = 1
     UPLOAD_MANY_TESTS = 2
     CREATE_SHIPMNT = 3
     RECV_SHIPMNT = 4
     PETAL_GND = 5
     GLUE_WEIGHT = 6
     MOD_IV = 7
     WIRE_BOND = 8
     
     def __init__(self, session):
         """Initialization."""
-        super().__init__(title="ITkDB Dashboard", session=session)
+        super().__init__(title="ITkDB Dashboard", session=session, help=HELP_LINK)
         self.mask = 0
 
         # set border width
         self.set_border_width(10)
 
         # Prepare dashboard
         lbl = Gtk.Label()
@@ -67,24 +68,24 @@
         grid.attach(btnTest, 0, irow, 1, 1)
 
         btnTest = Gtk.Button(label="Upload Multiple Tests")
         btnTest.connect("clicked", self.upload_multiple_tests)
         grid.attach(btnTest, 1, irow, 1, 1)
 
         irow += 1
-        btnGnd = Gtk.Button(label="Petal VI/GND")
+        btnGnd = Gtk.Button(label="Petal Reception")
         btnGnd.connect("clicked", self.petal_gnd)
         grid.attach(btnGnd, 0, irow, 1, 1)
 
         btnWeight = Gtk.Button(label="GlueWeight")
         btnWeight.connect("clicked", self.glue_weight)
         grid.attach(btnWeight, 1, irow, 1, 1)
 
         irow += 1
-        btnModIV = Gtk.Button(label="Module IV")
+        btnModIV = Gtk.Button(label="Sensor/Module IV")
         btnModIV.connect("clicked", self.module_IV)
         grid.attach(btnModIV, 0, irow, 1, 1)
 
         btnWireBond = Gtk.Button(label="Wire Bond")
         btnWireBond.connect("clicked", self.wire_bond)
         grid.attach(btnWireBond, 1, irow, 1, 1)
 
@@ -116,92 +117,92 @@
         """Launch upload test."""
         bitn = DashWindow.UPLOAD_TEST
         bt = 1 << bitn
         if self.mask & bt:
             return
 
         self.mask |= bt
-        W = UploadTest.UploadTest(self.session)
+        W = UploadTest.UploadTest(self.session, help=HELP_LINK)
         W.connect("destroy", self.app_closed, bitn)
 
     def upload_multiple_tests(self, *args):
         """Launch upload multiple test."""
         bitn = DashWindow.UPLOAD_MANY_TESTS
         bt = 1 << bitn
         if self.mask & bt:
             return
 
         self.mask |= bt
-        W = UploadMultipleTests.UploadMultipleTests(self.session)
+        W = UploadMultipleTests.UploadMultipleTests(self.session, help=HELP_LINK)
         W.connect("destroy", self.app_closed, bitn)
 
     def create_shipment(self, *args):
         """Launch createShipment."""
         bitn = DashWindow.CREATE_SHIPMNT
         bt = 1 << bitn
         if self.mask & bt:
             return
 
         self.mask |= bt
-        W = CreateShipments.CreateShipments(self.session)
+        W = CreateShipments.CreateShipments(self.session, help=HELP_LINK)
         W.connect("destroy", self.app_closed, bitn)
 
     def receive_shipment(self, *args):
         """Launch getShipments."""
         bitn = DashWindow.RECV_SHIPMNT
         bt = 1 << bitn
         if self.mask & bt:
             return
 
         self.mask |= bt
-        W = GetShipments.ReceiveShipments(self.session)
+        W = GetShipments.ReceiveShipments(self.session, help=HELP_LINK)
         W.connect("destroy", self.app_closed, bitn)
 
     def petal_gnd(self, *args):
         """Petal GND/VI test."""
         bitn = DashWindow.PETAL_GND
         bt = 1 << bitn
         if self.mask & bt:
             return
 
         self.mask |= bt
-        W = GroundVITests.GroundingTest(self.session)
+        W = PetalReceptionTests.PetalReceptionTests(self.session, help=HELP_LINK)
         W.connect("destroy", self.app_closed, bitn)
 
     def glue_weight(self, *args):
         """Glue Weight test."""
         bitn = DashWindow.GLUE_WEIGHT
         bt = 1 << bitn
         if self.mask & bt:
             return
 
         self.mask |= bt
-        W = GlueWeight.GlueWeight(self.session)
+        W = GlueWeight.GlueWeight(self.session, help=HELP_LINK)
         W.connect("destroy", self.app_closed, bitn)
 
     def module_IV(self, *args):
         """Module IV tests."""
         bitn = DashWindow.MOD_IV
         bt = 1 << bitn
         if self.mask & bt:
             return
 
         self.mask |= bt
-        W = UploadModuleIV.IVwindow(self.session)
+        W = UploadModuleIV.IVwindow(self.session, help=HELP_LINK)
         W.connect("destroy", self.app_closed, bitn)
 
     def wire_bond(self, *args):
         """Module IV tests."""
         bitn = DashWindow.WIRE_BOND
         bt = 1 << bitn
         if self.mask & bt:
             return
 
         self.mask |= bt
-        W = WireBondGui.WireBond(session=self.session, title="Wirebond")
+        W = WireBondGui.WireBond(session=self.session, title="Wirebond", help=HELP_LINK)
         W.connect("destroy", self.app_closed, bitn)
 
     def app_closed(self, *args):
         """Application window closed. Clear mask."""
         bt = 1 << args[1]
         self.mask &= ~bt
         # print(bt, self.mask)
```

### Comparing `itkdb_gtk-0.9.0/itkdb_gtk/dbGtkUtils.py` & `itkdb_gtk-0.9.1.dev1/itkdb_gtk/dbGtkUtils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 """A set of GTK utilities for DB scripts."""
 import json
 import time
 from collections.abc import Iterable
 from copy import deepcopy
 from datetime import datetime
+import webbrowser
 
 import dateutil.parser
-import gi
 import numpy as np
 
 
+import gi
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk, GObject, Gio, GLib
 
 def parse_date(txt):
     """Parse a date."""
     try:
         return dateutil.parser.parse(txt, fuzzy=False)
 
     except Exception:
         return None
+    
 def parse_date_as_string(txt):
     """Parse data and return DB compatible string."""
     D = parse_date(txt)
     if D is None:
         return D
 
     out = D.isoformat(timespec='milliseconds')
@@ -435,15 +437,15 @@
         self.textbuffer.insert(end, msg)
         GLib.idle_add(self.scroll_to_end)
 
 
 class ITkDBWindow(Gtk.Window):
     """Base class for GUI main windows."""
 
-    def __init__(self, title="", session=None, show_search=None, gtk_runs=True, panel_size=100):
+    def __init__(self, title="", session=None, show_search=None, help=None, gtk_runs=True, panel_size=100):
         """Initialization.
 
         Args:
             title: The title of the window.
             session: ITkDB session.
             show_search: tooltip for search button in header (calls to query_db).
                          No search button if this is None.
@@ -451,14 +453,15 @@
                       terminal only.
 
         """
         self.session = session
         self.inst2code = {}
         self.code2inst = {}
         self.message_panel = None
+        self.help = help
 
         if gtk_runs:
             super().__init__(title=title)
             self.prepare_window(show_search, panel_size)
 
     def prepare_window(self, show_search, panel_size):
         """Inititalizes GUI."""
@@ -478,14 +481,23 @@
             button = Gtk.Button()
             icon = Gio.ThemedIcon(name="system-search-symbolic")
             image = Gtk.Image.new_from_gicon(icon, Gtk.IconSize.BUTTON)
             button.add(image)
             button.set_tooltip_text(show_search)
             button.connect("clicked", self.query_db)
             self.hb.pack_end(button)
+            
+        if self.help:
+            button = Gtk.Button()
+            icon = Gio.ThemedIcon(name="help-browser-symbolic")
+            image = Gtk.Image.new_from_gicon(icon, Gtk.IconSize.BUTTON)
+            button.add(image)
+            button.connect("clicked", self.show_help)
+            self.hb.pack_end(button)
+            
 
         # Create main content box
         self.mainBox = Gtk.Box(orientation=Gtk.Orientation.VERTICAL)
         self.mainBox.set_property("margin-left", 6)
         self.mainBox.set_property("margin-right", 6)
 
         self.add(self.mainBox)
@@ -503,24 +515,30 @@
         self.mainBox.pack_end(btnBox, False, True, 0)
 
     def quit(self, *args):
         """Quits the application."""
         self.hide()
         self.destroy()
 
+    def show_help(self, *args):
+        """Show help"""
+        webbrowser.open(self.help)
+    
     def query_db(self, *args):
         """Search button clicked."""
         pass
 
     def new_login(self, obj, msg):
         """A new user logged in."""
         if msg == "<OK>":
             if hasattr(self.session, "user_gui"):
                 self.session = self.session.user_gui.get_client()
-            self.userLabel.get_child().set_text(self.session.user.name)
+                
+            if self.userLabel.get_child():
+                self.userLabel.get_child().set_text(self.session.user.name)
 
         else:
             self.write_message("Could not login.\n{}".format(msg))
 
     def reconnect(self, *args):
         """Reconnects."""
         if hasattr(self.session, "user_gui"):
```

### Comparing `itkdb_gtk-0.9.0/itkdb_gtk/readAVSdata.py` & `itkdb_gtk-0.9.1.dev1/itkdb_gtk/readAVSdata.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.9.0/itkdb_gtk/readGoogleSheet.py` & `itkdb_gtk-0.9.1.dev1/itkdb_gtk/readGoogleSheet.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.9.0/itkdb_gtk/untrash_component.py` & `itkdb_gtk-0.9.1.dev1/itkdb_gtk/untrash_component.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.9.0/itkdb_gtk.egg-info/PKG-INFO` & `itkdb_gtk-0.9.1.dev1/itkdb_gtk.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itkdb_gtk
-Version: 0.9.0
+Version: 0.9.1.dev1
 Summary: A collection of Gtk based GUI to access ITkDB.
 Author-email: Carlos Lacasta <carlos.lacasta@cern.ch>
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `itkdb_gtk-0.9.0/itkdb_gtk.egg-info/SOURCES.txt` & `itkdb_gtk-0.9.1.dev1/itkdb_gtk.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 README.md
 pyproject.toml
 itkdb_gtk/CreateShipments.py
 itkdb_gtk/GetShipments.py
 itkdb_gtk/GlueWeight.py
-itkdb_gtk/GroundVITests.py
 itkdb_gtk/ITkDB.desktop
 itkdb_gtk/ITkDB.svg
 itkdb_gtk/ITkDBlogin.py
 itkdb_gtk/ITkDButils.py
+itkdb_gtk/PetalReceptionTests.py
+itkdb_gtk/SensorUtils.py
 itkdb_gtk/ShowAttachments.py
 itkdb_gtk/ShowComments.py
 itkdb_gtk/ShowDefects.py
 itkdb_gtk/UploadModuleIV.py
 itkdb_gtk/UploadMultipleTests.py
 itkdb_gtk/UploadPetalInformation.py
 itkdb_gtk/UploadTest.py
@@ -24,8 +25,9 @@
 itkdb_gtk/untrash_component.py
 itkdb_gtk.egg-info/PKG-INFO
 itkdb_gtk.egg-info/SOURCES.txt
 itkdb_gtk.egg-info/dependency_links.txt
 itkdb_gtk.egg-info/entry_points.txt
 itkdb_gtk.egg-info/requires.txt
 itkdb_gtk.egg-info/top_level.txt
+test/testAnimated.py
 test/test_holes.py
```

### Comparing `itkdb_gtk-0.9.0/pyproject.toml` & `itkdb_gtk-0.9.1.dev1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "itkdb_gtk"
-version = "0.9.0"
+version = "0.9.1.dev1"
 authors = [
   { name="Carlos Lacasta", email="carlos.lacasta@cern.ch" },
 ]
 description = "A collection of Gtk based GUI to access ITkDB."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
@@ -26,21 +26,21 @@
     "Operating System :: OS Independent",
 ]
 
 [project.gui-scripts]
 itkdb_dashBoard = "itkdb_gtk:dash_board"
 getShipments = "itkdb_gtk:getShipments"
 glueWeight = "itkdb_gtk:glueWeight"
-groundVITests = "itkdb_gtk:groundVITests"
+petalReceptionTests = "itkdb_gtk:petalReceptionTests"
 createShipments = "itkdb_gtk:createShipments"
 uploadTest = "itkdb_gtk:uploadTest"
 uploadMultipleTests = "itkdb_gtk:uploadMultipleTests"
 uploadModuleIV = "itkdb_gtk:uploadModuleIV"
 wirebondTest = "itkdb_gtk:wirebondTest"
-iploadPetalInformation = "itkdb_gtk:uploadPetalInformation"
+uploadPetalInformation = "itkdb_gtk:uploadPetalInformation"
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.package-data]
 itkdb_gtk = ["*.desktop", "*.svg"]
```

### Comparing `itkdb_gtk-0.9.0/test/test_holes.py` & `itkdb_gtk-0.9.1.dev1/test/test_holes.py`

 * *Files identical despite different names*

