# Comparing `tmp/revhubinterface-1.3.3.dev9.tar.gz` & `tmp/revhubinterface-1.3.4.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revhubinterface-1.3.3.dev9.tar", last modified: Wed May 15 03:09:43 2024, max compression
+gzip compressed data, was "revhubinterface-1.3.4.dev1.tar", last modified: Mon May 20 06:27:45 2024, max compression
```

## Comparing `revhubinterface-1.3.3.dev9.tar` & `revhubinterface-1.3.4.dev1.tar`

### file list

```diff
@@ -1,45 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:09:43.098067 revhubinterface-1.3.3.dev9/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:09:43.090067 revhubinterface-1.3.3.dev9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:09:43.094067 revhubinterface-1.3.3.dev9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/.github/workflows/pyinstaller.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-15 03:09:43.098067 revhubinterface-1.3.3.dev9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:09:43.098067 revhubinterface-1.3.3.dev9/REVHubInterface/
--rw-r--r--   0 runner    (1001) docker     (127)    20812 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/REVHubInterface/REV2mSensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/REVHubInterface/REVADC.py
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/REVHubInterface/REVColorSensorV3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/REVHubInterface/REVComPorts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/REVHubInterface/REVDIO.py
--rw-r--r--   0 runner    (1001) docker     (127)    15925 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/REVHubInterface/REVI2C.py
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/REVHubInterface/REVModule.py
--rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/REVHubInterface/REVMotor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/REVHubInterface/REVServo.py
--rw-r--r--   0 runner    (1001) docker     (127)    16892 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/REVHubInterface/REVcomm.py
--rw-r--r--   0 runner    (1001) docker     (127)    73523 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/REVHubInterface/REVmessages.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/REVHubInterface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    61367 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/REVHubInterface/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-15 03:09:43.000000 revhubinterface-1.3.3.dev9/REVHubInterface/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:09:43.098067 revhubinterface-1.3.3.dev9/REVHubInterface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-15 03:09:43.000000 revhubinterface-1.3.3.dev9/REVHubInterface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-15 03:09:43.000000 revhubinterface-1.3.3.dev9/REVHubInterface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 03:09:43.000000 revhubinterface-1.3.3.dev9/REVHubInterface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-15 03:09:43.000000 revhubinterface-1.3.3.dev9/REVHubInterface.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-15 03:09:43.000000 revhubinterface-1.3.3.dev9/REVHubInterface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-15 03:09:43.000000 revhubinterface-1.3.3.dev9/REVHubInterface.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/REVHubInterface.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/REVHubInterface.spec
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:09:43.098067 revhubinterface-1.3.3.dev9/flatpak/
--rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/flatpak/flatpak-pip-generator
--rwxr-xr-x   0 runner    (1001) docker     (127)      162 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/flatpak/org.unofficialrevport.REVHubInterface.desktop
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/flatpak/org.unofficialrevport.REVHubInterface.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/flatpak/python3-requirements.json
--rw-r--r--   0 runner    (1001) docker     (127)    23399 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/org.unofficialrevport.REVHubInterface.Devel.svg
--rw-r--r--   0 runner    (1001) docker     (127)   384626 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/org.unofficialrevport.REVHubInterface.Source.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/org.unofficialrevport.REVHubInterface.metainfo.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/org.unofficialrevport.REVHubInterface.svg
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-15 03:09:38.000000 revhubinterface-1.3.3.dev9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 03:09:43.098067 revhubinterface-1.3.3.dev9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:27:45.807108 revhubinterface-1.3.4.dev1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:27:45.799108 revhubinterface-1.3.4.dev1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:27:45.803108 revhubinterface-1.3.4.dev1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/.github/workflows/pyinstaller.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-20 06:27:45.807108 revhubinterface-1.3.4.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:27:45.807108 revhubinterface-1.3.4.dev1/REVHubInterface/
+-rw-r--r--   0 runner    (1001) docker     (127)    20812 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/REVHubInterface/REV2mSensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/REVHubInterface/REVADC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/REVHubInterface/REVColorSensorV3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/REVHubInterface/REVComPorts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/REVHubInterface/REVDIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15925 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/REVHubInterface/REVI2C.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/REVHubInterface/REVModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/REVHubInterface/REVMotor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/REVHubInterface/REVServo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16892 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/REVHubInterface/REVcomm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73523 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/REVHubInterface/REVmessages.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/REVHubInterface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61395 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/REVHubInterface/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-20 06:27:45.000000 revhubinterface-1.3.4.dev1/REVHubInterface/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:27:45.807108 revhubinterface-1.3.4.dev1/REVHubInterface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-20 06:27:45.000000 revhubinterface-1.3.4.dev1/REVHubInterface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-20 06:27:45.000000 revhubinterface-1.3.4.dev1/REVHubInterface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 06:27:45.000000 revhubinterface-1.3.4.dev1/REVHubInterface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-20 06:27:45.000000 revhubinterface-1.3.4.dev1/REVHubInterface.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-20 06:27:45.000000 revhubinterface-1.3.4.dev1/REVHubInterface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-20 06:27:45.000000 revhubinterface-1.3.4.dev1/REVHubInterface.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/REVHubInterface.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/REVHubInterface.spec
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:27:45.807108 revhubinterface-1.3.4.dev1/flatpak/
+-rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/flatpak/flatpak-pip-generator
+-rwxr-xr-x   0 runner    (1001) docker     (127)      162 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/flatpak/org.unofficialrevport.REVHubInterface.desktop
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/flatpak/org.unofficialrevport.REVHubInterface.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/flatpak/python3-requirements.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23399 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/org.unofficialrevport.REVHubInterface.Devel.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   384626 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/org.unofficialrevport.REVHubInterface.Source.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    99970 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/org.unofficialrevport.REVHubInterface.icns
+-rw-r--r--   0 runner    (1001) docker     (127)    33388 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/org.unofficialrevport.REVHubInterface.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/org.unofficialrevport.REVHubInterface.metainfo.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/org.unofficialrevport.REVHubInterface.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/pyinstaller-build-reqs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 06:27:45.807108 revhubinterface-1.3.4.dev1/setup.cfg
```

### Comparing `revhubinterface-1.3.3.dev9/.github/workflows/python-publish.yml` & `revhubinterface-1.3.4.dev1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev9/LICENSE.txt` & `revhubinterface-1.3.4.dev1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev9/PKG-INFO` & `revhubinterface-1.3.4.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: REVHubInterface
-Version: 1.3.3.dev9
+Version: 1.3.4.dev1
 Summary: GUI program for manual control of REV Robotics Expansion Hub from a PC. Unofficial "Community Edition". 
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyft232==0.12
 Requires-Dist: pyserial==3.5
 Requires-Dist: sv-ttk==2.6.0
```

### Comparing `revhubinterface-1.3.3.dev9/README.md` & `revhubinterface-1.3.4.dev1/README.md`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev9/REVHubInterface/REV2mSensor.py` & `revhubinterface-1.3.4.dev1/REVHubInterface/REV2mSensor.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev9/REVHubInterface/REVADC.py` & `revhubinterface-1.3.4.dev1/REVHubInterface/REVADC.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev9/REVHubInterface/REVColorSensorV3.py` & `revhubinterface-1.3.4.dev1/REVHubInterface/REVColorSensorV3.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev9/REVHubInterface/REVComPorts.py` & `revhubinterface-1.3.4.dev1/REVHubInterface/REVComPorts.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev9/REVHubInterface/REVDIO.py` & `revhubinterface-1.3.4.dev1/REVHubInterface/REVDIO.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev9/REVHubInterface/REVI2C.py` & `revhubinterface-1.3.4.dev1/REVHubInterface/REVI2C.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev9/REVHubInterface/REVModule.py` & `revhubinterface-1.3.4.dev1/REVHubInterface/REVModule.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev9/REVHubInterface/REVMotor.py` & `revhubinterface-1.3.4.dev1/REVHubInterface/REVMotor.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev9/REVHubInterface/REVServo.py` & `revhubinterface-1.3.4.dev1/REVHubInterface/REVServo.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev9/REVHubInterface/REVcomm.py` & `revhubinterface-1.3.4.dev1/REVHubInterface/REVcomm.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev9/REVHubInterface/REVmessages.py` & `revhubinterface-1.3.4.dev1/REVHubInterface/REVmessages.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev9/REVHubInterface/__main__.py` & `revhubinterface-1.3.4.dev1/REVHubInterface/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1126,16 +1126,16 @@
     except Exception as e:
         # Print error, then fall back to default ttk theme
         print(e)
         pass
 
     # Attempt to load version
     try:
-        import _version
-        version = _version.version
+        from REVHubInterface._version import __version__
+        version = __version__
     except ModuleNotFoundError:
         version = "DEV BUILD"
 
 
     xroot.title(f'REV Hub Interface - Community Edition - v{version}')
     try:
         xroot.iconbitmap('resource\\\\favicon.ico')
```

### Comparing `revhubinterface-1.3.3.dev9/REVHubInterface.egg-info/PKG-INFO` & `revhubinterface-1.3.4.dev1/REVHubInterface.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: REVHubInterface
-Version: 1.3.3.dev9
+Version: 1.3.4.dev1
 Summary: GUI program for manual control of REV Robotics Expansion Hub from a PC. Unofficial "Community Edition". 
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyft232==0.12
 Requires-Dist: pyserial==3.5
 Requires-Dist: sv-ttk==2.6.0
```

### Comparing `revhubinterface-1.3.3.dev9/REVHubInterface.egg-info/SOURCES.txt` & `revhubinterface-1.3.4.dev1/REVHubInterface.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 .gitignore
 LICENSE.txt
 README.md
 REVHubInterface.sh
 REVHubInterface.spec
 org.unofficialrevport.REVHubInterface.Devel.svg
 org.unofficialrevport.REVHubInterface.Source.svg
+org.unofficialrevport.REVHubInterface.icns
+org.unofficialrevport.REVHubInterface.ico
 org.unofficialrevport.REVHubInterface.metainfo.xml
 org.unofficialrevport.REVHubInterface.svg
+pyinstaller-build-reqs.txt
 pyproject.toml
 requirements.txt
 .github/workflows/pyinstaller.yml
 .github/workflows/python-publish.yml
 REVHubInterface/REV2mSensor.py
 REVHubInterface/REVADC.py
 REVHubInterface/REVColorSensorV3.py
```

### Comparing `revhubinterface-1.3.3.dev9/flatpak/flatpak-pip-generator` & `revhubinterface-1.3.4.dev1/flatpak/flatpak-pip-generator`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev9/flatpak/org.unofficialrevport.REVHubInterface.yml` & `revhubinterface-1.3.4.dev1/flatpak/org.unofficialrevport.REVHubInterface.yml`

 * *Files 5% similar despite different names*

```diff
@@ -53,16 +53,18 @@
               type: anitya
               project-id: 11426
               stable-only: true
               url-template: https://prdownloads.sourceforge.net/tcl/tk$version-src.tar.gz
   - name: revhubinterface
     buildsystem: simple
     build-commands:
+      - python -m setuptools_scm --force-write-version-files
       - pip3 install --verbose --exists-action=i --no-index --find-links="file://${PWD}" --prefix=${FLATPAK_DEST} . --no-build-isolation
       - install -Dm755 REVHubInterface.sh /app/bin/REVHubInterface.sh
       - install -Dm644 -t /app/share/applications flatpak/org.unofficialrevport.REVHubInterface.desktop
       - install -Dm644 -t /app/share/icons/hicolor/scalable/apps org.unofficialrevport.REVHubInterface.svg
+      - install -Dm644 -t /app/share/metainfo org.unofficialrevport.REVHubInterface.metainfo.xml
     sources:
       - type: git
         url: https://github.com/unofficial-rev-port/REVHubInterface.git
-        commit: 40ae8c18fe9dd6ab92e8945ca669ff37e087d1bf
+        commit: 1f759c2868fee59824def38c2946077fa29557c3
```

### Comparing `revhubinterface-1.3.3.dev9/flatpak/python3-requirements.json` & `revhubinterface-1.3.4.dev1/flatpak/python3-requirements.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'modules'": "{insert: [(3, OrderedDict([('name', 'python3-setuptools-scm'), ('buildsystem', "*

 * *              "'simple'), ('build-commands', ['pip3 install --verbose --exists-action=i --no-index "*

 * *              '--find-links="file://${PWD}" --prefix=${FLATPAK_DEST} "setuptools-scm==8.1.0" '*

 * *              "--no-build-isolation']), ('sources', [OrderedDict([('type', 'file'), ('url', "*

 * *              "'https://files.pythonhosted.org/packages/49/df/1fceb2f8900f8639e278b056416d49134fb8d84c5942ffaa01ad34782422/pac […]*

```diff
@@ -49,11 +49,30 @@
             "sources": [
                 {
                     "sha256": "4319c52edf2e14732fe84bdc9788e26f9e9a1ad79451ec0f89f0120ffc8105d9",
                     "type": "file",
                     "url": "https://files.pythonhosted.org/packages/0f/3d/be0abc3202e90f282ad465f4e7c6e41bc8dce810ce5d1611566a1e7dfba8/sv_ttk-2.6.0-py3-none-any.whl"
                 }
             ]
+        },
+        {
+            "build-commands": [
+                "pip3 install --verbose --exists-action=i --no-index --find-links=\"file://${PWD}\" --prefix=${FLATPAK_DEST} \"setuptools-scm==8.1.0\" --no-build-isolation"
+            ],
+            "buildsystem": "simple",
+            "name": "python3-setuptools-scm",
+            "sources": [
+                {
+                    "sha256": "2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5",
+                    "type": "file",
+                    "url": "https://files.pythonhosted.org/packages/49/df/1fceb2f8900f8639e278b056416d49134fb8d84c5942ffaa01ad34782422/packaging-24.0-py3-none-any.whl"
+                },
+                {
+                    "sha256": "897a3226a6fd4a6eb2f068745e49733261a21f70b1bb28fce0339feb978d9af3",
+                    "type": "file",
+                    "url": "https://files.pythonhosted.org/packages/a0/b9/1906bfeb30f2fc13bb39bf7ddb8749784c05faadbd18a21cf141ba37bff2/setuptools_scm-8.1.0-py3-none-any.whl"
+                }
+            ]
         }
     ],
     "name": "python3-requirements"
 }
```

### Comparing `revhubinterface-1.3.3.dev9/org.unofficialrevport.REVHubInterface.Devel.svg` & `revhubinterface-1.3.4.dev1/org.unofficialrevport.REVHubInterface.Devel.svg`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev9/org.unofficialrevport.REVHubInterface.Source.svg` & `revhubinterface-1.3.4.dev1/org.unofficialrevport.REVHubInterface.Source.svg`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev9/org.unofficialrevport.REVHubInterface.metainfo.xml` & `revhubinterface-1.3.4.dev1/org.unofficialrevport.REVHubInterface.metainfo.xml`

 * *Files 0% similar despite different names*

#### Comparing `revhubinterface-1.3.3.dev9/org.unofficialrevport.REVHubInterface.metainfo.xml` & `revhubinterface-1.3.4.dev1/org.unofficialrevport.REVHubInterface.metainfo.xml`

```diff
@@ -25,16 +25,16 @@
     <category>Science</category>
     <category>Education</category>
     <category>Robotics</category>
     <category>Monitor</category>
     <category>Electronics</category>
   </categories>
   <branding>
-    <color type="primary" scheme-preference="light">#f05a28</color>
-    <color type="primary" scheme-preference="dark">#f05a28</color>
+    <color type="primary" scheme_preference="light">#f05a28</color>
+    <color type="primary" scheme_preference="dark">#873000</color>
   </branding>
   <screenshots>
     <screenshot type="default">
       <caption>Controlling motors</caption>
       <image type="source" width="1382" height="1590">https://unofficialrevport.org/revhubinterface/motorcontrol.png</image>
     </screenshot>
     <screenshot>
```

### Comparing `revhubinterface-1.3.3.dev9/org.unofficialrevport.REVHubInterface.svg` & `revhubinterface-1.3.4.dev1/org.unofficialrevport.REVHubInterface.svg`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev9/pyproject.toml` & `revhubinterface-1.3.4.dev1/pyproject.toml`

 * *Files identical despite different names*

