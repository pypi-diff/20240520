# Comparing `tmp/staging_cacao_accounting_desktop-2024.5.5.tar.gz` & `tmp/staging_cacao_accounting_desktop-2024.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "staging_cacao_accounting_desktop-2024.5.5.tar", last modified: Sun May  5 15:35:51 2024, max compression
+gzip compressed data, was "staging_cacao_accounting_desktop-2024.5.7.tar", last modified: Tue May  7 15:22:04 2024, max compression
```

## Comparing `staging_cacao_accounting_desktop-2024.5.5.tar` & `staging_cacao_accounting_desktop-2024.5.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 15:35:51.613078 staging_cacao_accounting_desktop-2024.5.5/
--rw-rw-rw-   0        0        0    11558 2024-03-23 22:22:54.000000 staging_cacao_accounting_desktop-2024.5.5/LICENSE
--rw-rw-rw-   0        0        0     3862 2024-05-05 15:35:51.613078 staging_cacao_accounting_desktop-2024.5.5/PKG-INFO
--rw-rw-rw-   0        0        0     2909 2024-04-30 17:08:02.000000 staging_cacao_accounting_desktop-2024.5.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-05 15:35:51.599730 staging_cacao_accounting_desktop-2024.5.5/cacao_accounting_desktop/
--rw-rw-rw-   0        0        0     3327 2024-04-30 18:44:13.000000 staging_cacao_accounting_desktop-2024.5.5/cacao_accounting_desktop/__init__.py
--rw-rw-rw-   0        0        0       61 2024-04-30 16:45:42.000000 staging_cacao_accounting_desktop-2024.5.5/cacao_accounting_desktop/__main__.py
--rw-rw-rw-   0        0        0     1183 2024-05-05 15:35:30.000000 staging_cacao_accounting_desktop-2024.5.5/pyproject.toml
--rw-rw-rw-   0        0        0       81 2024-05-05 15:27:05.000000 staging_cacao_accounting_desktop-2024.5.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-05 15:35:51.613078 staging_cacao_accounting_desktop-2024.5.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-05 15:35:51.611574 staging_cacao_accounting_desktop-2024.5.5/staging_cacao_accounting_desktop.egg-info/
--rw-rw-rw-   0        0        0     3862 2024-05-05 15:35:51.000000 staging_cacao_accounting_desktop-2024.5.5/staging_cacao_accounting_desktop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      461 2024-05-05 15:35:51.000000 staging_cacao_accounting_desktop-2024.5.5/staging_cacao_accounting_desktop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 15:35:51.000000 staging_cacao_accounting_desktop-2024.5.5/staging_cacao_accounting_desktop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2024-05-05 15:35:51.000000 staging_cacao_accounting_desktop-2024.5.5/staging_cacao_accounting_desktop.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       57 2024-05-05 15:35:51.000000 staging_cacao_accounting_desktop-2024.5.5/staging_cacao_accounting_desktop.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2024-05-05 15:35:51.000000 staging_cacao_accounting_desktop-2024.5.5/staging_cacao_accounting_desktop.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 15:22:04.894409 staging_cacao_accounting_desktop-2024.5.7/
+-rw-rw-rw-   0        0        0    11558 2024-03-23 22:22:54.000000 staging_cacao_accounting_desktop-2024.5.7/LICENSE
+-rw-rw-rw-   0        0        0     3876 2024-05-07 15:22:04.883697 staging_cacao_accounting_desktop-2024.5.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2923 2024-05-05 16:07:17.000000 staging_cacao_accounting_desktop-2024.5.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 15:22:04.704398 staging_cacao_accounting_desktop-2024.5.7/cacao_accounting_desktop/
+-rw-rw-rw-   0        0        0     3158 2024-05-06 22:59:26.000000 staging_cacao_accounting_desktop-2024.5.7/cacao_accounting_desktop/__init__.py
+-rw-rw-rw-   0        0        0       61 2024-04-30 16:45:42.000000 staging_cacao_accounting_desktop-2024.5.7/cacao_accounting_desktop/__main__.py
+-rw-rw-rw-   0        0        0     1183 2024-05-07 15:19:30.000000 staging_cacao_accounting_desktop-2024.5.7/pyproject.toml
+-rw-rw-rw-   0        0        0       81 2024-05-05 15:27:05.000000 staging_cacao_accounting_desktop-2024.5.7/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 15:22:04.894409 staging_cacao_accounting_desktop-2024.5.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-07 15:22:04.883697 staging_cacao_accounting_desktop-2024.5.7/staging_cacao_accounting_desktop.egg-info/
+-rw-rw-rw-   0        0        0     3876 2024-05-07 15:22:04.000000 staging_cacao_accounting_desktop-2024.5.7/staging_cacao_accounting_desktop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      461 2024-05-07 15:22:04.000000 staging_cacao_accounting_desktop-2024.5.7/staging_cacao_accounting_desktop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 15:22:04.000000 staging_cacao_accounting_desktop-2024.5.7/staging_cacao_accounting_desktop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2024-05-07 15:22:04.000000 staging_cacao_accounting_desktop-2024.5.7/staging_cacao_accounting_desktop.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       57 2024-05-07 15:22:04.000000 staging_cacao_accounting_desktop-2024.5.7/staging_cacao_accounting_desktop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2024-05-07 15:22:04.000000 staging_cacao_accounting_desktop-2024.5.7/staging_cacao_accounting_desktop.egg-info/top_level.txt
```

### Comparing `staging_cacao_accounting_desktop-2024.5.5/LICENSE` & `staging_cacao_accounting_desktop-2024.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting_desktop-2024.5.5/PKG-INFO` & `staging_cacao_accounting_desktop-2024.5.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: staging_cacao_accounting_desktop
-Version: 2024.5.5
+Version: 2024.5.7
 Summary: Cacao Accounting Desktop App.
 Author-email: BMO Soluciones <development@bmogroup.solutions>
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: Spanish
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
@@ -59,14 +59,15 @@
 ```
 pip install pyvan
 ```
 
 2. Create a Windows executable with:
 
 ```
+rm -rf dist/
 python van.py
 ```
 
 Doble click on the executable to verify it works.
 
 3. Create a Windows installer with [nsis](https://nsis.sourceforge.io/Main_Page) using the `setup.nsi`, this will create a installer that can be shared to final users.
```

### Comparing `staging_cacao_accounting_desktop-2024.5.5/README.md` & `staging_cacao_accounting_desktop-2024.5.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 ```
 pip install pyvan
 ```
 
 2. Create a Windows executable with:
 
 ```
+rm -rf dist/
 python van.py
 ```
 
 Doble click on the executable to verify it works.
 
 3. Create a Windows installer with [nsis](https://nsis.sourceforge.io/Main_Page) using the `setup.nsi`, this will create a installer that can be shared to final users.
```

### Comparing `staging_cacao_accounting_desktop-2024.5.5/cacao_accounting_desktop/__init__.py` & `staging_cacao_accounting_desktop-2024.5.7/cacao_accounting_desktop/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 # ---------------------------------------------------------------------------------------
 # Librerias de terceros
 # ---------------------------------------------------------------------------------------
 from appdirs import AppDirs
 from cacao_accounting import create_app
 from flaskwebgui import FlaskUI
 from PIL import Image
-import wx
 
 if TYPE_CHECKING:
     from flask import Flask
 
 
 # ---------------------------------------------------------------------------------------
 # Principales constantes
@@ -75,26 +74,25 @@
     if Path.exists(BACKUP_PATH_FILE):
         with open(BACKUP_PATH_FILE) as f:
             return Path(f.readline())
     else:
         return APP_BACKUP_DIR
 
 
-class HelloFrame(wx.Frame):
+import kivy
+from kivy.app import App
+from kivy.config import Config
+from kivy.uix.label import Label
 
-    def __init__(self, *args, **kw):
-        super(HelloFrame, self).__init__(*args, **kw)
 
-        panel = wx.Panel(self)
+Config.set("kivy", "window_icon", "assets\CacaoAccounting.png")
 
-        st = wx.StaticText(panel, label="Cacao Accounting Desktop")
-        font = st.GetFont()
-        font.PointSize += 10
-        font = font.Bold()
-        st.SetFont(font)
+
+class MyApp(App):
+    title = "Cacao Accounting Desktop"
+
+    def build(self):
+        pass
 
 
 def init_app():
-    app = wx.App()
-    frm = HelloFrame(None, title="Cacao Accounting")
-    frm.Show()
-    app.MainLoop()
+    MyApp().run()
```

### Comparing `staging_cacao_accounting_desktop-2024.5.5/pyproject.toml` & `staging_cacao_accounting_desktop-2024.5.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "staging_cacao_accounting_desktop"
 description = "Cacao Accounting Desktop App."
 readme = "README.md"
 requires-python = ">=3.8"
-version="2024.05.05"
+version="2024.05.07"
 authors = [
   {name = "BMO Soluciones", email = "development@bmogroup.solutions"},
 ]
 classifiers = [
   'License :: OSI Approved :: Apache Software License',
   'Natural Language :: Spanish',
   'Operating System :: OS Independent',
```

### Comparing `staging_cacao_accounting_desktop-2024.5.5/staging_cacao_accounting_desktop.egg-info/PKG-INFO` & `staging_cacao_accounting_desktop-2024.5.7/staging_cacao_accounting_desktop.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: staging_cacao_accounting_desktop
-Version: 2024.5.5
+Version: 2024.5.7
 Summary: Cacao Accounting Desktop App.
 Author-email: BMO Soluciones <development@bmogroup.solutions>
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: Spanish
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
@@ -59,14 +59,15 @@
 ```
 pip install pyvan
 ```
 
 2. Create a Windows executable with:
 
 ```
+rm -rf dist/
 python van.py
 ```
 
 Doble click on the executable to verify it works.
 
 3. Create a Windows installer with [nsis](https://nsis.sourceforge.io/Main_Page) using the `setup.nsi`, this will create a installer that can be shared to final users.
```

