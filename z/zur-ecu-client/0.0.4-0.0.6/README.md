# Comparing `tmp/zur_ecu_client-0.0.4.tar.gz` & `tmp/zur_ecu_client-0.0.6.tar.gz`

## Comparing `zur_ecu_client-0.0.4.tar` & `zur_ecu_client-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,33 @@
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.4/requirements.txt
--rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.4/.github/workflows/publish-to-test-pypi.yaml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.4/.vscode/settings.json
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.4/src/zur_ecu_client/__init__.py
--rw-r--r--   0        0        0     4017 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.4/src/zur_ecu_client/ecu_client.py
--rw-r--r--   0        0        0     3607 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.4/src/zur_ecu_client/ecu_server.py
--rw-r--r--   0        0        0    12822 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.4/src/zur_ecu_client/messages.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.4/src/zur_ecu_client/senml/__init__.py
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.4/src/zur_ecu_client/senml/senml_base.py
--rw-r--r--   0        0        0    10020 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.4/src/zur_ecu_client/senml/senml_pack.py
--rw-r--r--   0        0        0     9445 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.4/src/zur_ecu_client/senml/senml_record.py
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.4/src/zur_ecu_client/senml/senml_unit.py
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.4/src/zur_ecu_client/senml/senml_zur_names.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.4/tests/test_sample.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.4/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.4/LICENSE.txt
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.4/README.md
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/requirements.txt
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/.github/workflows/black.yml
+-rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/.github/workflows/publish-to-test-pypi.yaml
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/.idea/.gitignore
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/.idea/ECU-Client.iml
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/.idea/misc.xml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/.idea/vcs.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/.idea/runConfigurations/pytest.xml
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/.vscode/settings.json
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/src/zur_ecu_client/__init__.py
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/src/zur_ecu_client/ecu_client.py
+-rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/src/zur_ecu_client/messages.py
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/src/zur_ecu_client/mock_ecu.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/src/zur_ecu_client/udp_server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/src/zur_ecu_client/senml/__init__.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/src/zur_ecu_client/senml/senml.py
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/src/zur_ecu_client/senml/senml_msg.py
+-rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/src/zur_ecu_client/senml/senml_msg_dv.py
+-rw-r--r--   0        0        0     5401 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/src/zur_ecu_client/senml/senml_msg_ecu.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/src/zur_ecu_client/senml/senml_unit.py
+-rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/src/zur_ecu_client/senml/senml_zur_names.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/src/zur_ecu_client/senml/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/tests/test_messages.py
+-rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/tests/test_sample.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/LICENSE.txt
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/README.md
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.6/PKG-INFO
```

### Comparing `zur_ecu_client-0.0.4/.github/workflows/publish-to-test-pypi.yaml` & `zur_ecu_client-0.0.6/.github/workflows/publish-to-test-pypi.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 name: Publish Python 🐍 distribution 📦 to PyPI and TestPyPI
 
 on:
   workflow_dispatch:
   push:
-
+    tags:
+       - '*.*.*'
+    branches:
+      - develop
+      - main
 jobs:
   build:
     name: Build distribution 📦
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python
       uses: actions/setup-python@v5
       with:
-        python-version: "3.x"
+        python-version: "3.10"
     - name: Install pypa/build
       run: >-
         python3 -m
         pip install
         build
         --user
     - name: Build a binary wheel and a source tarball
       run: python3 -m build
     - name: Store the distribution packages
-      uses: actions/upload-artifact@v3
+      uses: actions/upload-artifact@v4
       with:
         name: python-package-distributions
         path: dist/
 
   publish-to-pypi:
     name: >-
       Publish Python 🐍 distribution 📦 to PyPI
@@ -40,15 +44,15 @@
       name: pypi
       url: https://pypi.org/p/<package-name>  # Replace <package-name> with your PyPI project name
     permissions:
       id-token: write  # IMPORTANT: mandatory for trusted publishing
 
     steps:
     - name: Download all the dists
-      uses: actions/download-artifact@v3
+      uses: actions/download-artifact@v4
       with:
         name: python-package-distributions
         path: dist/
     - name: Publish distribution 📦 to PyPI
       uses: pypa/gh-action-pypi-publish@release/v1
 
   github-release:
@@ -61,15 +65,15 @@
 
     permissions:
       contents: write  # IMPORTANT: mandatory for making GitHub Releases
       id-token: write  # IMPORTANT: mandatory for sigstore
 
     steps:
     - name: Download all the dists
-      uses: actions/download-artifact@v3
+      uses: actions/download-artifact@v4
       with:
         name: python-package-distributions
         path: dist/
     - name: Sign the dists with Sigstore
       uses: sigstore/gh-action-sigstore-python@v2.1.1
       with:
         inputs: >-
@@ -105,15 +109,15 @@
       url: https://test.pypi.org/p/<package-name>
 
     permissions:
       id-token: write  # IMPORTANT: mandatory for trusted publishing
 
     steps:
     - name: Download all the dists
-      uses: actions/download-artifact@v3
+      uses: actions/download-artifact@v4
       with:
         name: python-package-distributions
         path: dist/
     - name: Publish distribution 📦 to TestPyPI
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
         repository-url: https://test.pypi.org/legacy/
```

### Comparing `zur_ecu_client-0.0.4/.gitignore` & `zur_ecu_client-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `zur_ecu_client-0.0.4/LICENSE.txt` & `zur_ecu_client-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zur_ecu_client-0.0.4/pyproject.toml` & `zur_ecu_client-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "zur_ecu_client" 
-version = "0.0.4" 
+version = "0.0.6"
 description = "Internal Python library which provides an interface to the ECU"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE.txt"}
 keywords = ["sample", "setuptools", "development"]
 authors = [
     {name = "ZUR Driverless", email = "driverless@zurichuasracing.ch" },
```

### Comparing `zur_ecu_client-0.0.4/PKG-INFO` & `zur_ecu_client-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: zur_ecu_client
-Version: 0.0.4
+Version: 0.0.6
 Summary: Internal Python library which provides an interface to the ECU
 Project-URL: Homepage, https://zurichuasracing.ch
 Project-URL: Bug Reports, https://github.com/zurich-uas-racing/issues
 Project-URL: Source, https://github.com/zurich-uas-racing/ecu-client
 Author-email: ZUR Driverless <driverless@zurichuasracing.ch>, Finn Scheller <finn.scheller@zurichuasracing.ch>, Cèline Brun <bruncel1@students.zhaw.ch>
 Maintainer-email: ZUR Driverless <driverless@zurichuasracing.ch>
 License: MIT License
```

