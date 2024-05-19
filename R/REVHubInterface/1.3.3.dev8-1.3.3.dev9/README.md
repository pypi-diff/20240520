# Comparing `tmp/revhubinterface-1.3.3.dev8.tar.gz` & `tmp/revhubinterface-1.3.3.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revhubinterface-1.3.3.dev8.tar", last modified: Wed May 15 02:33:59 2024, max compression
+gzip compressed data, was "revhubinterface-1.3.3.dev9.tar", last modified: Wed May 15 03:09:43 2024, max compression
```

## Comparing `revhubinterface-1.3.3.dev8.tar` & `revhubinterface-1.3.3.dev9.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 02:33:59.898804 revhubinterface-1.3.3.dev8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 02:33:59.890804 revhubinterface-1.3.3.dev8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 02:33:59.890804 revhubinterface-1.3.3.dev8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/.github/workflows/pyinstaller.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-15 02:33:59.898804 revhubinterface-1.3.3.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 02:33:59.894804 revhubinterface-1.3.3.dev8/REVHubInterface/
--rw-r--r--   0 runner    (1001) docker     (127)    20812 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/REVHubInterface/REV2mSensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/REVHubInterface/REVADC.py
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/REVHubInterface/REVColorSensorV3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/REVHubInterface/REVComPorts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/REVHubInterface/REVDIO.py
--rw-r--r--   0 runner    (1001) docker     (127)    15925 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/REVHubInterface/REVI2C.py
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/REVHubInterface/REVModule.py
--rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/REVHubInterface/REVMotor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/REVHubInterface/REVServo.py
--rw-r--r--   0 runner    (1001) docker     (127)    16892 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/REVHubInterface/REVcomm.py
--rw-r--r--   0 runner    (1001) docker     (127)    73523 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/REVHubInterface/REVmessages.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/REVHubInterface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    61200 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/REVHubInterface/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 02:33:59.894804 revhubinterface-1.3.3.dev8/REVHubInterface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-15 02:33:59.000000 revhubinterface-1.3.3.dev8/REVHubInterface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-15 02:33:59.000000 revhubinterface-1.3.3.dev8/REVHubInterface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 02:33:59.000000 revhubinterface-1.3.3.dev8/REVHubInterface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-15 02:33:59.000000 revhubinterface-1.3.3.dev8/REVHubInterface.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-15 02:33:59.000000 revhubinterface-1.3.3.dev8/REVHubInterface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-15 02:33:59.000000 revhubinterface-1.3.3.dev8/REVHubInterface.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/REVHubInterface.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/REVHubInterface.spec
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 02:33:59.894804 revhubinterface-1.3.3.dev8/flatpak/
--rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/flatpak/flatpak-pip-generator
--rwxr-xr-x   0 runner    (1001) docker     (127)      162 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/flatpak/org.unofficialrevport.REVHubInterface.desktop
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/flatpak/org.unofficialrevport.REVHubInterface.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/flatpak/python3-requirements.json
--rw-r--r--   0 runner    (1001) docker     (127)    23399 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/org.unofficialrevport.REVHubInterface.Devel.svg
--rw-r--r--   0 runner    (1001) docker     (127)   384626 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/org.unofficialrevport.REVHubInterface.Source.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/org.unofficialrevport.REVHubInterface.metainfo.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/org.unofficialrevport.REVHubInterface.svg
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-15 02:33:55.000000 revhubinterface-1.3.3.dev8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 02:33:59.898804 revhubinterface-1.3.3.dev8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:09:43.098067 revhubinterface-1.3.3.dev9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:09:43.090067 revhubinterface-1.3.3.dev9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:09:43.094067 revhubinterface-1.3.3.dev9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/.github/workflows/pyinstaller.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-15 03:09:43.098067 revhubinterface-1.3.3.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:09:43.098067 revhubinterface-1.3.3.dev9/REVHubInterface/
+-rw-r--r--   0 runner    (1001) docker     (127)    20812 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/REVHubInterface/REV2mSensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/REVHubInterface/REVADC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/REVHubInterface/REVColorSensorV3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/REVHubInterface/REVComPorts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/REVHubInterface/REVDIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15925 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/REVHubInterface/REVI2C.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/REVHubInterface/REVModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/REVHubInterface/REVMotor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/REVHubInterface/REVServo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16892 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/REVHubInterface/REVcomm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73523 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/REVHubInterface/REVmessages.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/REVHubInterface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61367 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/REVHubInterface/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-15 03:09:43.000000 revhubinterface-1.3.3.dev9/REVHubInterface/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:09:43.098067 revhubinterface-1.3.3.dev9/REVHubInterface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-15 03:09:43.000000 revhubinterface-1.3.3.dev9/REVHubInterface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-15 03:09:43.000000 revhubinterface-1.3.3.dev9/REVHubInterface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 03:09:43.000000 revhubinterface-1.3.3.dev9/REVHubInterface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-15 03:09:43.000000 revhubinterface-1.3.3.dev9/REVHubInterface.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-15 03:09:43.000000 revhubinterface-1.3.3.dev9/REVHubInterface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-15 03:09:43.000000 revhubinterface-1.3.3.dev9/REVHubInterface.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/REVHubInterface.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/REVHubInterface.spec
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:09:43.098067 revhubinterface-1.3.3.dev9/flatpak/
+-rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/flatpak/flatpak-pip-generator
+-rwxr-xr-x   0 runner    (1001) docker     (127)      162 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/flatpak/org.unofficialrevport.REVHubInterface.desktop
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/flatpak/org.unofficialrevport.REVHubInterface.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/flatpak/python3-requirements.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23399 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/org.unofficialrevport.REVHubInterface.Devel.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   384626 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/org.unofficialrevport.REVHubInterface.Source.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/org.unofficialrevport.REVHubInterface.metainfo.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/org.unofficialrevport.REVHubInterface.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 03:09:43.098067 revhubinterface-1.3.3.dev9/setup.cfg
```

### Comparing `revhubinterface-1.3.3.dev8/.github/workflows/pyinstaller.yml` & `revhubinterface-1.3.3.dev9/.github/workflows/pyinstaller.yml`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev8/.github/workflows/python-publish.yml` & `revhubinterface-1.3.3.dev9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev8/LICENSE.txt` & `revhubinterface-1.3.3.dev9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev8/PKG-INFO` & `revhubinterface-1.3.3.dev9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: REVHubInterface
-Version: 1.3.3.dev8
+Version: 1.3.3.dev9
 Summary: GUI program for manual control of REV Robotics Expansion Hub from a PC. Unofficial "Community Edition". 
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyft232==0.12
 Requires-Dist: pyserial==3.5
 Requires-Dist: sv-ttk==2.6.0
```

### Comparing `revhubinterface-1.3.3.dev8/README.md` & `revhubinterface-1.3.3.dev9/README.md`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev8/REVHubInterface/REV2mSensor.py` & `revhubinterface-1.3.3.dev9/REVHubInterface/REV2mSensor.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev8/REVHubInterface/REVADC.py` & `revhubinterface-1.3.3.dev9/REVHubInterface/REVADC.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev8/REVHubInterface/REVColorSensorV3.py` & `revhubinterface-1.3.3.dev9/REVHubInterface/REVColorSensorV3.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev8/REVHubInterface/REVComPorts.py` & `revhubinterface-1.3.3.dev9/REVHubInterface/REVComPorts.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev8/REVHubInterface/REVDIO.py` & `revhubinterface-1.3.3.dev9/REVHubInterface/REVDIO.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev8/REVHubInterface/REVI2C.py` & `revhubinterface-1.3.3.dev9/REVHubInterface/REVI2C.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev8/REVHubInterface/REVModule.py` & `revhubinterface-1.3.3.dev9/REVHubInterface/REVModule.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev8/REVHubInterface/REVMotor.py` & `revhubinterface-1.3.3.dev9/REVHubInterface/REVMotor.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev8/REVHubInterface/REVServo.py` & `revhubinterface-1.3.3.dev9/REVHubInterface/REVServo.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev8/REVHubInterface/REVcomm.py` & `revhubinterface-1.3.3.dev9/REVHubInterface/REVcomm.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev8/REVHubInterface/REVmessages.py` & `revhubinterface-1.3.3.dev9/REVHubInterface/REVmessages.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev8/REVHubInterface/__main__.py` & `revhubinterface-1.3.3.dev9/REVHubInterface/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1124,15 +1124,23 @@
         sv_ttk.set_theme("dark")
         print('Loaded Tk theme: Sun Valley')
     except Exception as e:
         # Print error, then fall back to default ttk theme
         print(e)
         pass
 
-    xroot.title('REV Hub Interface - Community Edition - v1.3.1')
+    # Attempt to load version
+    try:
+        import _version
+        version = _version.version
+    except ModuleNotFoundError:
+        version = "DEV BUILD"
+
+
+    xroot.title(f'REV Hub Interface - Community Edition - v{version}')
     try:
         xroot.iconbitmap('resource\\\\favicon.ico')
     except:
         try:
             xroot.iconbitmap('favicon.ico')
         except:
             pass
```

### Comparing `revhubinterface-1.3.3.dev8/REVHubInterface.egg-info/PKG-INFO` & `revhubinterface-1.3.3.dev9/REVHubInterface.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: REVHubInterface
-Version: 1.3.3.dev8
+Version: 1.3.3.dev9
 Summary: GUI program for manual control of REV Robotics Expansion Hub from a PC. Unofficial "Community Edition". 
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyft232==0.12
 Requires-Dist: pyserial==3.5
 Requires-Dist: sv-ttk==2.6.0
```

### Comparing `revhubinterface-1.3.3.dev8/REVHubInterface.egg-info/SOURCES.txt` & `revhubinterface-1.3.3.dev9/REVHubInterface.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 REVHubInterface/REVModule.py
 REVHubInterface/REVMotor.py
 REVHubInterface/REVServo.py
 REVHubInterface/REVcomm.py
 REVHubInterface/REVmessages.py
 REVHubInterface/__init__.py
 REVHubInterface/__main__.py
+REVHubInterface/_version.py
 REVHubInterface.egg-info/PKG-INFO
 REVHubInterface.egg-info/SOURCES.txt
 REVHubInterface.egg-info/dependency_links.txt
 REVHubInterface.egg-info/entry_points.txt
 REVHubInterface.egg-info/requires.txt
 REVHubInterface.egg-info/top_level.txt
 flatpak/flatpak-pip-generator
```

### Comparing `revhubinterface-1.3.3.dev8/REVHubInterface.spec` & `revhubinterface-1.3.3.dev9/REVHubInterface.spec`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev8/flatpak/flatpak-pip-generator` & `revhubinterface-1.3.3.dev9/flatpak/flatpak-pip-generator`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev8/flatpak/org.unofficialrevport.REVHubInterface.yml` & `revhubinterface-1.3.3.dev9/flatpak/org.unofficialrevport.REVHubInterface.yml`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev8/flatpak/python3-requirements.json` & `revhubinterface-1.3.3.dev9/flatpak/python3-requirements.json`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev8/org.unofficialrevport.REVHubInterface.Devel.svg` & `revhubinterface-1.3.3.dev9/org.unofficialrevport.REVHubInterface.Devel.svg`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev8/org.unofficialrevport.REVHubInterface.Source.svg` & `revhubinterface-1.3.3.dev9/org.unofficialrevport.REVHubInterface.Source.svg`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev8/org.unofficialrevport.REVHubInterface.metainfo.xml` & `revhubinterface-1.3.3.dev9/org.unofficialrevport.REVHubInterface.metainfo.xml`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev8/org.unofficialrevport.REVHubInterface.svg` & `revhubinterface-1.3.3.dev9/org.unofficialrevport.REVHubInterface.svg`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev8/pyproject.toml` & `revhubinterface-1.3.3.dev9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -10,7 +10,8 @@
 dependencies = { file = ["requirements.txt"] }
 [tool.setuptools]
 packages = ["REVHubInterface"]
 [project.gui-scripts]
 revhubinterface = "REVHubInterface.__main__:initwindow"
 [tool.setuptools_scm]
 local_scheme = "no-local-version"
+version_file = "REVHubInterface/_version.py"
```

