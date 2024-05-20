# Comparing `tmp/opmentis-0.1.0.tar.gz` & `tmp/opmentis-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opmentis-0.1.0.tar", last modified: Mon May  6 18:41:56 2024, max compression
+gzip compressed data, was "opmentis-0.1.1.tar", last modified: Mon May 20 03:34:38 2024, max compression
```

## Comparing `opmentis-0.1.0.tar` & `opmentis-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:41:56.024934 opmentis-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-06 18:41:56.024934 opmentis-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-06 18:41:50.000000 opmentis-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:41:56.020934 opmentis-0.1.0/opmentis/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-06 18:41:50.000000 opmentis-0.1.0/opmentis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-06 18:41:50.000000 opmentis-0.1.0/opmentis/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:41:56.024934 opmentis-0.1.0/opmentis/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 18:41:50.000000 opmentis-0.1.0/opmentis/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-06 18:41:50.000000 opmentis-0.1.0/opmentis/tests/test_core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:41:56.024934 opmentis-0.1.0/opmentis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-06 18:41:55.000000 opmentis-0.1.0/opmentis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-06 18:41:56.000000 opmentis-0.1.0/opmentis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 18:41:55.000000 opmentis-0.1.0/opmentis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-06 18:41:55.000000 opmentis-0.1.0/opmentis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-06 18:41:55.000000 opmentis-0.1.0/opmentis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 18:41:56.024934 opmentis-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-06 18:41:50.000000 opmentis-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:34:38.443430 opmentis-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-20 03:34:38.443430 opmentis-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-20 03:34:33.000000 opmentis-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:34:38.443430 opmentis-0.1.1/opmentis/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-20 03:34:33.000000 opmentis-0.1.1/opmentis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-20 03:34:33.000000 opmentis-0.1.1/opmentis/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:34:38.443430 opmentis-0.1.1/opmentis/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 03:34:33.000000 opmentis-0.1.1/opmentis/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-05-20 03:34:33.000000 opmentis-0.1.1/opmentis/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:34:38.443430 opmentis-0.1.1/opmentis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-20 03:34:38.000000 opmentis-0.1.1/opmentis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-20 03:34:38.000000 opmentis-0.1.1/opmentis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 03:34:38.000000 opmentis-0.1.1/opmentis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-20 03:34:38.000000 opmentis-0.1.1/opmentis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-20 03:34:38.000000 opmentis-0.1.1/opmentis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 03:34:38.443430 opmentis-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-20 03:34:33.000000 opmentis-0.1.1/setup.py
```

### Comparing `opmentis-0.1.0/PKG-INFO` & `opmentis-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: opmentis
-Version: 0.1.0
-Summary: Library to register opmentis miners.
+Version: 0.1.1
+Summary: Library to register opmentis miners and check data
 Home-page: https://github.com/OpMentis-Ai
 Author: opmentis
 Author-email: opmentisai@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: requests>=2.25.1
 
 # Opmentis
 
 Opmentis is a Python package designed to manage user registrations within a decentralized application, allowing users to register as miners or validators with AWS DynamoDB. This package simplifies the process of user registration by providing a single function that can handle different user roles based on the presence of a stake.
 
 ## Features
 
@@ -41,18 +40,27 @@
 
 # Example: Registering a miner
 miner_wallet_address = "miner_wallet_address"
 miner = register_miners(wallet_address=miner_wallet_address)
 print("Miner Registered:", miner)
 
 ```
+### Check your data
+To register a new user as a miner:
+
+```python
+from opmentis import userdata
+
+# Example: Registering a miner
+miner_wallet_address = "miner_wallet_address"
+userdata(wallet_address=miner_wallet_address)
+
+```
 
 ### Contributing
 Contributions to Opmentis are welcome. Please fork the repository, make your changes, and submit a pull request.
 
 ### License
 
 
 For more information and updates, visit GitHub repository URL or contact the project maintainers.
 
-
-
```

### Comparing `opmentis-0.1.0/README.md` & `opmentis-0.1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -26,14 +26,25 @@
 
 # Example: Registering a miner
 miner_wallet_address = "miner_wallet_address"
 miner = register_miners(wallet_address=miner_wallet_address)
 print("Miner Registered:", miner)
 
 ```
+### Check your data
+To register a new user as a miner:
+
+```python
+from opmentis import userdata
+
+# Example: Registering a miner
+miner_wallet_address = "miner_wallet_address"
+userdata(wallet_address=miner_wallet_address)
+
+```
 
 ### Contributing
 Contributions to Opmentis are welcome. Please fork the repository, make your changes, and submit a pull request.
 
 ### License
```

### Comparing `opmentis-0.1.0/opmentis/core.py` & `opmentis-0.1.1/opmentis/core.py`

 * *Files 19% similar despite different names*

```diff
@@ -35,9 +35,33 @@
             return {"error": "Failed to register user.", "status_code": response.status_code}
 
         # Handle unexpected conditions or server messages
         unexpected_response_message = "Unexpected server response: {}".format(response.json())
         print(unexpected_response_message)
         return {"error": unexpected_response_message}
 
+    
+def userdata(wallet_address: str):
+    """Fetch user data from the central API endpoint and return as a formatted table."""
+    endpoint = "http://54.74.133.71/user_data/table"
+    payload = {"wallet_address": wallet_address}
+
+    with requests.Session() as session:
+        response = session.post(endpoint, json=payload)
+        if response.status_code == 200:
+            user_table = response.json().get("user_table", "")
+            return user_table
+        else:
+            # General error handling for unsuccessful attempts
+            error_message = f"Failed to fetch user data. Status code: {response.status_code}, Response: {response.json()}"
+            print(error_message)  # Print error message to console or log
+            return {"error": "Failed to fetch user data.", "status_code": response.status_code}
+
+        # Handle unexpected conditions or server messages
+        unexpected_response_message = "Unexpected server response: {}".format(response.json())
+        print(unexpected_response_message)
+        return {"error": unexpected_response_message}
+
+
+
```

### Comparing `opmentis-0.1.0/opmentis/tests/test_core.py` & `opmentis-0.1.1/opmentis/tests/test_core.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 import requests_mock
-from opmentis import register_miners
+from opmentis import register_miners, userdata
 
 def test_register_miners_success():
     wallet_address = "0x42C584058fA2a01622D09827EF688dD33d9643Dc"
     endpoint = "http://54.74.133.71/register_user"
     expected_response = f"Miner registered successfully with wallet address: {wallet_address}"
 
     # Setup mock
@@ -54,7 +54,48 @@
     # Setup mock
     with requests_mock.Mocker() as m:
         m.post(endpoint, json={"error": "Failed to register user."}, status_code=400)
         response = register_miners(wallet_address)
         assert response == {"error": "Failed to register user.", "status_code": 400}
         assert m.last_request.json() == {"wallet_address": wallet_address}
 
+def test_userdata_success():
+    wallet_address = "0x42C584058fA2a01622D09827EF688dD33d9643Dc"
+    endpoint = "http://54.74.133.71/user_data/table"
+
+    # Define sample user data
+    user_data = {
+        "Point": 100,
+        "Incentive": 50,
+        "Daily Attempt": 5,
+        "Broken": 2,
+        "Stake": 500,
+        "Total Attempt": 50
+    }
+
+    # Setup mock
+    with requests_mock.Mocker() as m:
+        m.post(endpoint, json={"user_table": "Mocked table data"}, status_code=200)
+        response = userdata(wallet_address)
+        
+        # Assert response
+        assert response == "Mocked table data"
+        
+        # Assert last request payload
+        assert m.last_request.json() == {"wallet_address": wallet_address}
+
+
+def test_userdata_failure():
+    wallet_address = "0x42C584058fA2a01622D09827EF688dD33d9643Dc"
+    endpoint = "http://54.74.133.71/user_data/table"
+
+    # Setup mock
+    with requests_mock.Mocker() as m:
+        m.post(endpoint, json={"error": "Failed to fetch user data."}, status_code=500)
+        response = userdata(wallet_address)
+        
+        # Assert response
+        assert response == {"error": "Failed to fetch user data.", "status_code": 500}
+        
+        # Assert last request payload
+        assert m.last_request.json() == {"wallet_address": wallet_address}
+
```

### Comparing `opmentis-0.1.0/opmentis.egg-info/PKG-INFO` & `opmentis-0.1.1/opmentis.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: opmentis
-Version: 0.1.0
-Summary: Library to register opmentis miners.
+Version: 0.1.1
+Summary: Library to register opmentis miners and check data
 Home-page: https://github.com/OpMentis-Ai
 Author: opmentis
 Author-email: opmentisai@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: requests>=2.25.1
 
 # Opmentis
 
 Opmentis is a Python package designed to manage user registrations within a decentralized application, allowing users to register as miners or validators with AWS DynamoDB. This package simplifies the process of user registration by providing a single function that can handle different user roles based on the presence of a stake.
 
 ## Features
 
@@ -41,18 +40,27 @@
 
 # Example: Registering a miner
 miner_wallet_address = "miner_wallet_address"
 miner = register_miners(wallet_address=miner_wallet_address)
 print("Miner Registered:", miner)
 
 ```
+### Check your data
+To register a new user as a miner:
+
+```python
+from opmentis import userdata
+
+# Example: Registering a miner
+miner_wallet_address = "miner_wallet_address"
+userdata(wallet_address=miner_wallet_address)
+
+```
 
 ### Contributing
 Contributions to Opmentis are welcome. Please fork the repository, make your changes, and submit a pull request.
 
 ### License
 
 
 For more information and updates, visit GitHub repository URL or contact the project maintainers.
 
-
-
```

### Comparing `opmentis-0.1.0/setup.py` & `opmentis-0.1.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='opmentis',
-    version='0.1.0',
+    version='0.1.1',
     author='opmentis',
     author_email='opmentisai@gmail.com',
     packages=find_packages(),
     install_requires=[
         'requests>=2.25.1',  # Ensure you include all necessary dependencies
     ],
     python_requires='>=3.6',
-    description='Library to register opmentis miners.',
+    description='Library to register opmentis miners and check data',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/OpMentis-Ai',  # Replace with the URL to your project
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

