# Comparing `tmp/euc2mqtt-0.0.3.tar.gz` & `tmp/euc2mqtt-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "euc2mqtt-0.0.3.tar", last modified: Sat May 18 21:24:03 2024, max compression
+gzip compressed data, was "euc2mqtt-1.0.0.tar", last modified: Mon May 20 13:45:45 2024, max compression
```

## Comparing `euc2mqtt-0.0.3.tar` & `euc2mqtt-1.0.0.tar`

### file list

```diff
@@ -1,35 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:24:03.869849 euc2mqtt-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:24:03.865849 euc2mqtt-0.0.3/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-18 21:23:52.000000 euc2mqtt-0.0.3/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-18 21:23:52.000000 euc2mqtt-0.0.3/.devcontainer/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:24:03.865849 euc2mqtt-0.0.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-18 21:23:52.000000 euc2mqtt-0.0.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:24:03.865849 euc2mqtt-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-18 21:23:52.000000 euc2mqtt-0.0.3/.github/workflows/build-win.yml
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-18 21:23:52.000000 euc2mqtt-0.0.3/.github/workflows/publish-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-18 21:23:52.000000 euc2mqtt-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-18 21:23:52.000000 euc2mqtt-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-05-18 21:24:03.869849 euc2mqtt-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-18 21:23:52.000000 euc2mqtt-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-18 21:23:52.000000 euc2mqtt-0.0.3/build.bat
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-18 21:23:52.000000 euc2mqtt-0.0.3/entry_point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-18 21:23:52.000000 euc2mqtt-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)    42774 2024-05-18 21:23:52.000000 euc2mqtt-0.0.3/scr.png
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 21:24:03.869849 euc2mqtt-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-18 21:23:52.000000 euc2mqtt-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:24:03.865849 euc2mqtt-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:24:03.869849 euc2mqtt-0.0.3/src/euc2mqtt/
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-18 21:23:52.000000 euc2mqtt-0.0.3/src/euc2mqtt/CLI.py
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-05-18 21:23:52.000000 euc2mqtt-0.0.3/src/euc2mqtt/EatonAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     5105 2024-05-18 21:23:52.000000 euc2mqtt-0.0.3/src/euc2mqtt/HassioAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-18 21:23:52.000000 euc2mqtt-0.0.3/src/euc2mqtt/InteropE2H.py
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-18 21:23:52.000000 euc2mqtt-0.0.3/src/euc2mqtt/Utility.py
--rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-05-18 21:23:52.000000 euc2mqtt-0.0.3/src/euc2mqtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-18 21:23:52.000000 euc2mqtt-0.0.3/src/euc2mqtt/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:24:03.869849 euc2mqtt-0.0.3/src/euc2mqtt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-05-18 21:24:03.000000 euc2mqtt-0.0.3/src/euc2mqtt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-18 21:24:03.000000 euc2mqtt-0.0.3/src/euc2mqtt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 21:24:03.000000 euc2mqtt-0.0.3/src/euc2mqtt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-18 21:24:03.000000 euc2mqtt-0.0.3/src/euc2mqtt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-18 21:24:03.000000 euc2mqtt-0.0.3/src/euc2mqtt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-18 21:24:03.000000 euc2mqtt-0.0.3/src/euc2mqtt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:45:45.542189 euc2mqtt-1.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:45:45.538189 euc2mqtt-1.0.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-20 13:45:41.000000 euc2mqtt-1.0.0/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-20 13:45:41.000000 euc2mqtt-1.0.0/.devcontainer/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:45:45.538189 euc2mqtt-1.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-20 13:45:41.000000 euc2mqtt-1.0.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:45:45.538189 euc2mqtt-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-20 13:45:41.000000 euc2mqtt-1.0.0/.github/workflows/build-win.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-20 13:45:41.000000 euc2mqtt-1.0.0/.github/workflows/publish-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-20 13:45:41.000000 euc2mqtt-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-20 13:45:41.000000 euc2mqtt-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7336 2024-05-20 13:45:45.542189 euc2mqtt-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-05-20 13:45:41.000000 euc2mqtt-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-20 13:45:41.000000 euc2mqtt-1.0.0/entry_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-20 13:45:41.000000 euc2mqtt-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    85344 2024-05-20 13:45:41.000000 euc2mqtt-1.0.0/scr.png
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 13:45:45.542189 euc2mqtt-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-20 13:45:41.000000 euc2mqtt-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:45:45.538189 euc2mqtt-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:45:45.538189 euc2mqtt-1.0.0/src/euc2mqtt/
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-20 13:45:41.000000 euc2mqtt-1.0.0/src/euc2mqtt/CLI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-05-20 13:45:41.000000 euc2mqtt-1.0.0/src/euc2mqtt/EatonAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5105 2024-05-20 13:45:41.000000 euc2mqtt-1.0.0/src/euc2mqtt/HassioAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-20 13:45:41.000000 euc2mqtt-1.0.0/src/euc2mqtt/InteropE2H.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-20 13:45:41.000000 euc2mqtt-1.0.0/src/euc2mqtt/Utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-05-20 13:45:41.000000 euc2mqtt-1.0.0/src/euc2mqtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-20 13:45:41.000000 euc2mqtt-1.0.0/src/euc2mqtt/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:45:45.542189 euc2mqtt-1.0.0/src/euc2mqtt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7336 2024-05-20 13:45:45.000000 euc2mqtt-1.0.0/src/euc2mqtt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-20 13:45:45.000000 euc2mqtt-1.0.0/src/euc2mqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 13:45:45.000000 euc2mqtt-1.0.0/src/euc2mqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-20 13:45:45.000000 euc2mqtt-1.0.0/src/euc2mqtt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-20 13:45:45.000000 euc2mqtt-1.0.0/src/euc2mqtt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-20 13:45:45.000000 euc2mqtt-1.0.0/src/euc2mqtt.egg-info/top_level.txt
```

### Comparing `euc2mqtt-0.0.3/.devcontainer/devcontainer.json` & `euc2mqtt-1.0.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `euc2mqtt-0.0.3/.devcontainer/docker-compose.yml` & `euc2mqtt-1.0.0/.devcontainer/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `euc2mqtt-0.0.3/.github/workflows/build-win.yml` & `euc2mqtt-1.0.0/.github/workflows/build-win.yml`

 * *Files identical despite different names*

### Comparing `euc2mqtt-0.0.3/.github/workflows/publish-pypi.yml` & `euc2mqtt-1.0.0/.github/workflows/publish-pypi.yml`

 * *Files identical despite different names*

### Comparing `euc2mqtt-0.0.3/.gitignore` & `euc2mqtt-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `euc2mqtt-0.0.3/LICENSE` & `euc2mqtt-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `euc2mqtt-0.0.3/PKG-INFO` & `euc2mqtt-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: euc2mqtt
-Version: 0.0.3
+Version: 1.0.0
 Summary: Eaton UPS Companion to MQTT Publisher
 Author: islandc_
 License: MIT License
         
         Copyright (c) 2024 islandc_
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -23,15 +23,15 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Repository, https://github.com/islandcontroller/euc2mqtt.git
 Project-URL: Issues, https://github.com/islandcontroller/euc2mqtt/issues/
-Project-URL: Documentation, https://github.com/islandcontroller/euc2mqtt/wiki/
+Project-URL: Documentation, https://github.com/islandcontroller/euc2mqtt?tab=readme-ov-file
 Keywords: eaton,ups,mqtt
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Communications
@@ -48,40 +48,43 @@
 
 # euc2mqtt
 
 [![License](https://img.shields.io/github/license/islandcontroller/euc2mqtt)](LICENSE) ![PyPI - Version](https://img.shields.io/pypi/v/euc2mqtt)
 
 A tool for publishing status data from a local Eaton UPS Companion service to Homeassistant.
 
-<p align="center"><img src="scr.png"/></p>
+<p align="center"><img src="https://raw.githubusercontent.com/islandcontroller/euc2mqtt/master/scr.png"/></p>
 
 ## Quick Start
 
 The following quick start guide should get you up and running from a blank Homeassistant installation. Feel free to skip a step if your system is already configured.
 
 ### Install mosquitto
 
 1. In Homeassistant, navigate to *Settings*, *Add-ons*
 2. Click the *Add-on store* button
 3. Search for *Mosquitto broker* and select the result
 4. Click on *Install*
 
+> [!NOTE]
+> When using the *Mosquitto broker* Add-on, your MQTT broker hostname will be the same as your Homeassistant's, e.g. "`homeassistant.local`".
+
 ### Create a new Homeassistant user for data ingest
 
 As mosquitto requires authentication, I heavily suggest creating a new user for data ingest.
 
 1. In Homeassistant, navigate to *Settings*, *People*
 2. Click on *Add person*, input a user name
 3. Check *Allow person to log in*
 4. Enter all required fields
 5. Check *Can only log in from local network*
 
 ### Get the application
 
-Windows binaries are provided on the [GitHub Releases](https://github.com/islandcontroller/euc2mqtt/releases) page.**
+Windows binaries are provided on the [GitHub Releases](https://github.com/islandcontroller/euc2mqtt/releases) page.
 
 If you prefer to use your own Python insallation, a pre-built package is hosted on [PyPI](https://pypi.org/project/euc2mqtt/) and can be installed and updated using the [`pip`](https://pip.pypa.io/en/stable/getting-started/) utility:
 
     pip install -U euc2mqtt
 
 ### Run it!
 
@@ -116,8 +119,49 @@
   --euc EUC             Eaton UPS Companion hostname and port (hostname[:port])
   --username USERNAME   Username for MQTT broker authentication
   --password PASSWORD   Password for MQTT broker authentication
   --interval INTERVAL   Update interval in seconds
   --full-update FULL_UPDATE
                         Number of incremental dataset fetches between full updates
   --logfile LOGFILE     Output log messages to a file
-  --verbose             Enable verbose logging```
+  --verbose             Enable verbose logging
+```
+
+## Running as a Windows Task
+
+1. Open *Task Scheduler* and select *Create New Task...*
+2. Select the following options on the *General* tab:
+    - Check *Run whether user is logged in or not*
+    - Uncheck *Do not store password*
+3. On the *Triggers* tab, create a "At startup" trigger
+4. On the *Actions* tab, add the standalone application as a program to run:
+    - Action: *Start a program*
+    - Program/Script: (Navigate to your `euc2mqtt.exe` here)
+    - Add arguments: `--mqtt <broker hostname> --username <user> --password <password>`
+5. On the *Settings* tab, select the following options:
+    - Check *Allow task to be run on demand*
+    - Select *If task fails, restart every: 1 minute*
+    - Uncheck *Stop the task if it runs longer than: ...*
+    - Select *If the task is already running: Do not start a new instance*
+6. Click *OK*. You will be prompted for a username and password to run the task as.
+
+## Configuring bind address for Eaton UPS Companion
+
+> [!WARNING]
+> Exposing the EUC service may pose a security risk.
+
+> [!NOTE]
+> When euc2mqtt is run on the same host as EUC, it is not required to expose the EUC service.
+
+1. Start a `notepad` instance with Admin privileges
+2. Open `C:\Program Files (x86)\Eaton\UPSCompanion\configs\config.js`
+3. Edit the "`httpServers`" line to listen on all interfaces:
+
+        "httpServers": {"http": {"port": 4679, "hostname": "0.0.0.0"}}, 
+
+## Legal Information
+
+The contents of this repository are licensed under the MIT License. The full license text is provided in the [`LICENSE`](LICENSE) file.
+
+    SPDX-License-Identifier: MIT
+
+"Eaton" is a trademark of Eaton Corporation. "Windows" is a trademark of Microsoft Corporation. All trademarks are property of their respective owners.
```

### Comparing `euc2mqtt-0.0.3/README.md` & `euc2mqtt-1.0.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 # euc2mqtt
 
 [![License](https://img.shields.io/github/license/islandcontroller/euc2mqtt)](LICENSE) ![PyPI - Version](https://img.shields.io/pypi/v/euc2mqtt)
 
 A tool for publishing status data from a local Eaton UPS Companion service to Homeassistant.
 
-<p align="center"><img src="scr.png"/></p>
+<p align="center"><img src="https://raw.githubusercontent.com/islandcontroller/euc2mqtt/master/scr.png"/></p>
 
 ## Quick Start
 
 The following quick start guide should get you up and running from a blank Homeassistant installation. Feel free to skip a step if your system is already configured.
 
 ### Install mosquitto
 
 1. In Homeassistant, navigate to *Settings*, *Add-ons*
 2. Click the *Add-on store* button
 3. Search for *Mosquitto broker* and select the result
 4. Click on *Install*
 
+> [!NOTE]
+> When using the *Mosquitto broker* Add-on, your MQTT broker hostname will be the same as your Homeassistant's, e.g. "`homeassistant.local`".
+
 ### Create a new Homeassistant user for data ingest
 
 As mosquitto requires authentication, I heavily suggest creating a new user for data ingest.
 
 1. In Homeassistant, navigate to *Settings*, *People*
 2. Click on *Add person*, input a user name
 3. Check *Allow person to log in*
 4. Enter all required fields
 5. Check *Can only log in from local network*
 
 ### Get the application
 
-Windows binaries are provided on the [GitHub Releases](https://github.com/islandcontroller/euc2mqtt/releases) page.**
+Windows binaries are provided on the [GitHub Releases](https://github.com/islandcontroller/euc2mqtt/releases) page.
 
 If you prefer to use your own Python insallation, a pre-built package is hosted on [PyPI](https://pypi.org/project/euc2mqtt/) and can be installed and updated using the [`pip`](https://pip.pypa.io/en/stable/getting-started/) utility:
 
     pip install -U euc2mqtt
 
 ### Run it!
 
@@ -68,8 +71,49 @@
   --euc EUC             Eaton UPS Companion hostname and port (hostname[:port])
   --username USERNAME   Username for MQTT broker authentication
   --password PASSWORD   Password for MQTT broker authentication
   --interval INTERVAL   Update interval in seconds
   --full-update FULL_UPDATE
                         Number of incremental dataset fetches between full updates
   --logfile LOGFILE     Output log messages to a file
-  --verbose             Enable verbose logging```
+  --verbose             Enable verbose logging
+```
+
+## Running as a Windows Task
+
+1. Open *Task Scheduler* and select *Create New Task...*
+2. Select the following options on the *General* tab:
+    - Check *Run whether user is logged in or not*
+    - Uncheck *Do not store password*
+3. On the *Triggers* tab, create a "At startup" trigger
+4. On the *Actions* tab, add the standalone application as a program to run:
+    - Action: *Start a program*
+    - Program/Script: (Navigate to your `euc2mqtt.exe` here)
+    - Add arguments: `--mqtt <broker hostname> --username <user> --password <password>`
+5. On the *Settings* tab, select the following options:
+    - Check *Allow task to be run on demand*
+    - Select *If task fails, restart every: 1 minute*
+    - Uncheck *Stop the task if it runs longer than: ...*
+    - Select *If the task is already running: Do not start a new instance*
+6. Click *OK*. You will be prompted for a username and password to run the task as.
+
+## Configuring bind address for Eaton UPS Companion
+
+> [!WARNING]
+> Exposing the EUC service may pose a security risk.
+
+> [!NOTE]
+> When euc2mqtt is run on the same host as EUC, it is not required to expose the EUC service.
+
+1. Start a `notepad` instance with Admin privileges
+2. Open `C:\Program Files (x86)\Eaton\UPSCompanion\configs\config.js`
+3. Edit the "`httpServers`" line to listen on all interfaces:
+
+        "httpServers": {"http": {"port": 4679, "hostname": "0.0.0.0"}}, 
+
+## Legal Information
+
+The contents of this repository are licensed under the MIT License. The full license text is provided in the [`LICENSE`](LICENSE) file.
+
+    SPDX-License-Identifier: MIT
+
+"Eaton" is a trademark of Eaton Corporation. "Windows" is a trademark of Microsoft Corporation. All trademarks are property of their respective owners.
```

### Comparing `euc2mqtt-0.0.3/pyproject.toml` & `euc2mqtt-1.0.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     "responses>=0.25",
     "ruff>=0.3"
 ]
 
 [project.urls]
 Repository = "https://github.com/islandcontroller/euc2mqtt.git"
 Issues = "https://github.com/islandcontroller/euc2mqtt/issues/"
-Documentation = "https://github.com/islandcontroller/euc2mqtt/wiki/"
+Documentation = "https://github.com/islandcontroller/euc2mqtt?tab=readme-ov-file"
 
 [project.scripts]
 euc2mqtt = "euc2mqtt.CLI:main"
 
 [tool.setuptools_scm]
 
 [tool.pytest.ini_options]
```

### Comparing `euc2mqtt-0.0.3/src/euc2mqtt/CLI.py` & `euc2mqtt-1.0.0/src/euc2mqtt/CLI.py`

 * *Files identical despite different names*

### Comparing `euc2mqtt-0.0.3/src/euc2mqtt/EatonAPI.py` & `euc2mqtt-1.0.0/src/euc2mqtt/EatonAPI.py`

 * *Files identical despite different names*

### Comparing `euc2mqtt-0.0.3/src/euc2mqtt/HassioAPI.py` & `euc2mqtt-1.0.0/src/euc2mqtt/HassioAPI.py`

 * *Files identical despite different names*

### Comparing `euc2mqtt-0.0.3/src/euc2mqtt/InteropE2H.py` & `euc2mqtt-1.0.0/src/euc2mqtt/InteropE2H.py`

 * *Files identical despite different names*

### Comparing `euc2mqtt-0.0.3/src/euc2mqtt/__init__.py` & `euc2mqtt-1.0.0/src/euc2mqtt/__init__.py`

 * *Files identical despite different names*

### Comparing `euc2mqtt-0.0.3/src/euc2mqtt.egg-info/PKG-INFO` & `euc2mqtt-1.0.0/src/euc2mqtt.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: euc2mqtt
-Version: 0.0.3
+Version: 1.0.0
 Summary: Eaton UPS Companion to MQTT Publisher
 Author: islandc_
 License: MIT License
         
         Copyright (c) 2024 islandc_
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -23,15 +23,15 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Repository, https://github.com/islandcontroller/euc2mqtt.git
 Project-URL: Issues, https://github.com/islandcontroller/euc2mqtt/issues/
-Project-URL: Documentation, https://github.com/islandcontroller/euc2mqtt/wiki/
+Project-URL: Documentation, https://github.com/islandcontroller/euc2mqtt?tab=readme-ov-file
 Keywords: eaton,ups,mqtt
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Communications
@@ -48,40 +48,43 @@
 
 # euc2mqtt
 
 [![License](https://img.shields.io/github/license/islandcontroller/euc2mqtt)](LICENSE) ![PyPI - Version](https://img.shields.io/pypi/v/euc2mqtt)
 
 A tool for publishing status data from a local Eaton UPS Companion service to Homeassistant.
 
-<p align="center"><img src="scr.png"/></p>
+<p align="center"><img src="https://raw.githubusercontent.com/islandcontroller/euc2mqtt/master/scr.png"/></p>
 
 ## Quick Start
 
 The following quick start guide should get you up and running from a blank Homeassistant installation. Feel free to skip a step if your system is already configured.
 
 ### Install mosquitto
 
 1. In Homeassistant, navigate to *Settings*, *Add-ons*
 2. Click the *Add-on store* button
 3. Search for *Mosquitto broker* and select the result
 4. Click on *Install*
 
+> [!NOTE]
+> When using the *Mosquitto broker* Add-on, your MQTT broker hostname will be the same as your Homeassistant's, e.g. "`homeassistant.local`".
+
 ### Create a new Homeassistant user for data ingest
 
 As mosquitto requires authentication, I heavily suggest creating a new user for data ingest.
 
 1. In Homeassistant, navigate to *Settings*, *People*
 2. Click on *Add person*, input a user name
 3. Check *Allow person to log in*
 4. Enter all required fields
 5. Check *Can only log in from local network*
 
 ### Get the application
 
-Windows binaries are provided on the [GitHub Releases](https://github.com/islandcontroller/euc2mqtt/releases) page.**
+Windows binaries are provided on the [GitHub Releases](https://github.com/islandcontroller/euc2mqtt/releases) page.
 
 If you prefer to use your own Python insallation, a pre-built package is hosted on [PyPI](https://pypi.org/project/euc2mqtt/) and can be installed and updated using the [`pip`](https://pip.pypa.io/en/stable/getting-started/) utility:
 
     pip install -U euc2mqtt
 
 ### Run it!
 
@@ -116,8 +119,49 @@
   --euc EUC             Eaton UPS Companion hostname and port (hostname[:port])
   --username USERNAME   Username for MQTT broker authentication
   --password PASSWORD   Password for MQTT broker authentication
   --interval INTERVAL   Update interval in seconds
   --full-update FULL_UPDATE
                         Number of incremental dataset fetches between full updates
   --logfile LOGFILE     Output log messages to a file
-  --verbose             Enable verbose logging```
+  --verbose             Enable verbose logging
+```
+
+## Running as a Windows Task
+
+1. Open *Task Scheduler* and select *Create New Task...*
+2. Select the following options on the *General* tab:
+    - Check *Run whether user is logged in or not*
+    - Uncheck *Do not store password*
+3. On the *Triggers* tab, create a "At startup" trigger
+4. On the *Actions* tab, add the standalone application as a program to run:
+    - Action: *Start a program*
+    - Program/Script: (Navigate to your `euc2mqtt.exe` here)
+    - Add arguments: `--mqtt <broker hostname> --username <user> --password <password>`
+5. On the *Settings* tab, select the following options:
+    - Check *Allow task to be run on demand*
+    - Select *If task fails, restart every: 1 minute*
+    - Uncheck *Stop the task if it runs longer than: ...*
+    - Select *If the task is already running: Do not start a new instance*
+6. Click *OK*. You will be prompted for a username and password to run the task as.
+
+## Configuring bind address for Eaton UPS Companion
+
+> [!WARNING]
+> Exposing the EUC service may pose a security risk.
+
+> [!NOTE]
+> When euc2mqtt is run on the same host as EUC, it is not required to expose the EUC service.
+
+1. Start a `notepad` instance with Admin privileges
+2. Open `C:\Program Files (x86)\Eaton\UPSCompanion\configs\config.js`
+3. Edit the "`httpServers`" line to listen on all interfaces:
+
+        "httpServers": {"http": {"port": 4679, "hostname": "0.0.0.0"}}, 
+
+## Legal Information
+
+The contents of this repository are licensed under the MIT License. The full license text is provided in the [`LICENSE`](LICENSE) file.
+
+    SPDX-License-Identifier: MIT
+
+"Eaton" is a trademark of Eaton Corporation. "Windows" is a trademark of Microsoft Corporation. All trademarks are property of their respective owners.
```

### Comparing `euc2mqtt-0.0.3/src/euc2mqtt.egg-info/SOURCES.txt` & `euc2mqtt-1.0.0/src/euc2mqtt.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 .gitignore
 LICENSE
 README.md
-build.bat
 entry_point.py
 pyproject.toml
 scr.png
 setup.py
 .devcontainer/devcontainer.json
 .devcontainer/docker-compose.yml
 .github/dependabot.yml
```

