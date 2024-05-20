# Comparing `tmp/termii_py-0.1.5.tar.gz` & `tmp/termii_py-0.1.6.tar.gz`

## Comparing `termii_py-0.1.5.tar` & `termii_py-0.1.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 termii_py-0.1.5/.flake8
--rw-r--r--   0        0        0     5222 2020-02-02 00:00:00.000000 termii_py-0.1.5/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 termii_py-0.1.5/CONTRIBUTING.md
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 termii_py-0.1.5/Makefile
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 termii_py-0.1.5/requirements.txt
--rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 termii_py-0.1.5/.github/workflows/ci.yml
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 termii_py-0.1.5/termii/__init__.py
--rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 termii_py-0.1.5/termii/auth.py
--rw-r--r--   0        0        0     7071 2020-02-02 00:00:00.000000 termii_py-0.1.5/termii/campaign.py
--rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 termii_py-0.1.5/termii/contacts.py
--rw-r--r--   0        0        0     7461 2020-02-02 00:00:00.000000 termii_py-0.1.5/termii/messaging.py
--rw-r--r--   0        0        0    12831 2020-02-02 00:00:00.000000 termii_py-0.1.5/termii/token.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 termii_py-0.1.5/termii/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 termii_py-0.1.5/termii/endpoints/__Init__.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 termii_py-0.1.5/termii/endpoints/campaign.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 termii_py-0.1.5/termii/endpoints/contacts.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 termii_py-0.1.5/termii/endpoints/messaging.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 termii_py-0.1.5/termii/endpoints/token.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 termii_py-0.1.5/termii/schemas/__init__.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 termii_py-0.1.5/termii/schemas/messaging.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 termii_py-0.1.5/termii/schemas/shared.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 termii_py-0.1.5/termii/schemas/token.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 termii_py-0.1.5/tests/__init__.py
--rw-r--r--   0        0        0     7338 2020-02-02 00:00:00.000000 termii_py-0.1.5/tests/conftest.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 termii_py-0.1.5/tests/test_auth.py
--rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 termii_py-0.1.5/tests/test_campaign.py
--rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 termii_py-0.1.5/tests/test_contacts.py
--rw-r--r--   0        0        0     5510 2020-02-02 00:00:00.000000 termii_py-0.1.5/tests/test_messaging.py
--rw-r--r--   0        0        0     5832 2020-02-02 00:00:00.000000 termii_py-0.1.5/tests/test_token.py
--rw-r--r--   0        0        0    10906 2020-02-02 00:00:00.000000 termii_py-0.1.5/tests/test_data/campaign.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 termii_py-0.1.5/tests/test_data/messaging.py
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 termii_py-0.1.5/tests/test_data/sender_id.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 termii_py-0.1.5/tests/test_data/token.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 termii_py-0.1.5/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 termii_py-0.1.5/LICENSE
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 termii_py-0.1.5/README.md
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 termii_py-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 termii_py-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 termii_py-0.1.6/.flake8
+-rw-r--r--   0        0        0     5222 2020-02-02 00:00:00.000000 termii_py-0.1.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 termii_py-0.1.6/CONTRIBUTING.md
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 termii_py-0.1.6/Makefile
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 termii_py-0.1.6/requirements.txt
+-rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 termii_py-0.1.6/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 termii_py-0.1.6/termii/__init__.py
+-rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 termii_py-0.1.6/termii/auth.py
+-rw-r--r--   0        0        0     7071 2020-02-02 00:00:00.000000 termii_py-0.1.6/termii/campaign.py
+-rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 termii_py-0.1.6/termii/contacts.py
+-rw-r--r--   0        0        0     7461 2020-02-02 00:00:00.000000 termii_py-0.1.6/termii/messaging.py
+-rw-r--r--   0        0        0    12831 2020-02-02 00:00:00.000000 termii_py-0.1.6/termii/token.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 termii_py-0.1.6/termii/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 termii_py-0.1.6/termii/endpoints/__Init__.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 termii_py-0.1.6/termii/endpoints/campaign.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 termii_py-0.1.6/termii/endpoints/contacts.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 termii_py-0.1.6/termii/endpoints/messaging.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 termii_py-0.1.6/termii/endpoints/token.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 termii_py-0.1.6/termii/schemas/__init__.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 termii_py-0.1.6/termii/schemas/messaging.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 termii_py-0.1.6/termii/schemas/shared.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 termii_py-0.1.6/termii/schemas/token.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 termii_py-0.1.6/tests/__init__.py
+-rw-r--r--   0        0        0     7338 2020-02-02 00:00:00.000000 termii_py-0.1.6/tests/conftest.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 termii_py-0.1.6/tests/test_auth.py
+-rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 termii_py-0.1.6/tests/test_campaign.py
+-rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 termii_py-0.1.6/tests/test_contacts.py
+-rw-r--r--   0        0        0     5510 2020-02-02 00:00:00.000000 termii_py-0.1.6/tests/test_messaging.py
+-rw-r--r--   0        0        0     5832 2020-02-02 00:00:00.000000 termii_py-0.1.6/tests/test_token.py
+-rw-r--r--   0        0        0    10906 2020-02-02 00:00:00.000000 termii_py-0.1.6/tests/test_data/campaign.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 termii_py-0.1.6/tests/test_data/messaging.py
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 termii_py-0.1.6/tests/test_data/sender_id.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 termii_py-0.1.6/tests/test_data/token.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 termii_py-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 termii_py-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 termii_py-0.1.6/README.md
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 termii_py-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 termii_py-0.1.6/PKG-INFO
```

### Comparing `termii_py-0.1.5/CODE_OF_CONDUCT.md` & `termii_py-0.1.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `termii_py-0.1.5/CONTRIBUTING.md` & `termii_py-0.1.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `termii_py-0.1.5/.github/workflows/ci.yml` & `termii_py-0.1.6/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `termii_py-0.1.5/termii/auth.py` & `termii_py-0.1.6/termii/auth.py`

 * *Files identical despite different names*

### Comparing `termii_py-0.1.5/termii/campaign.py` & `termii_py-0.1.6/termii/campaign.py`

 * *Files identical despite different names*

### Comparing `termii_py-0.1.5/termii/contacts.py` & `termii_py-0.1.6/termii/contacts.py`

 * *Files identical despite different names*

### Comparing `termii_py-0.1.5/termii/messaging.py` & `termii_py-0.1.6/termii/messaging.py`

 * *Files identical despite different names*

### Comparing `termii_py-0.1.5/termii/token.py` & `termii_py-0.1.6/termii/token.py`

 * *Files identical despite different names*

### Comparing `termii_py-0.1.5/termii/utils.py` & `termii_py-0.1.6/termii/utils.py`

 * *Files identical despite different names*

### Comparing `termii_py-0.1.5/termii/endpoints/campaign.py` & `termii_py-0.1.6/termii/endpoints/campaign.py`

 * *Files identical despite different names*

### Comparing `termii_py-0.1.5/tests/conftest.py` & `termii_py-0.1.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `termii_py-0.1.5/tests/test_auth.py` & `termii_py-0.1.6/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `termii_py-0.1.5/tests/test_campaign.py` & `termii_py-0.1.6/tests/test_campaign.py`

 * *Files identical despite different names*

### Comparing `termii_py-0.1.5/tests/test_contacts.py` & `termii_py-0.1.6/tests/test_contacts.py`

 * *Files identical despite different names*

### Comparing `termii_py-0.1.5/tests/test_messaging.py` & `termii_py-0.1.6/tests/test_messaging.py`

 * *Files identical despite different names*

### Comparing `termii_py-0.1.5/tests/test_token.py` & `termii_py-0.1.6/tests/test_token.py`

 * *Files identical despite different names*

### Comparing `termii_py-0.1.5/tests/test_data/campaign.py` & `termii_py-0.1.6/tests/test_data/campaign.py`

 * *Files identical despite different names*

### Comparing `termii_py-0.1.5/tests/test_data/sender_id.py` & `termii_py-0.1.6/tests/test_data/sender_id.py`

 * *Files identical despite different names*

### Comparing `termii_py-0.1.5/tests/test_data/token.py` & `termii_py-0.1.6/tests/test_data/token.py`

 * *Files identical despite different names*

### Comparing `termii_py-0.1.5/.gitignore` & `termii_py-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `termii_py-0.1.5/LICENSE` & `termii_py-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `termii_py-0.1.5/README.md` & `termii_py-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `termii_py-0.1.5/pyproject.toml` & `termii_py-0.1.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "termii-py"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="Unyime Etim", email="lordunyime@gmail.com" },
 ]
 description = "A beginner friendly SDK for Termii."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -20,13 +20,13 @@
 
 [tool.hatch.build.targets.wheel]
 packages = ["termii"]
 
 
 dependencies = [
   "requests>=2.23.0,<=2.32.0",
-  "pydantic>=1.10.4,<=2.7.0"
+  "pydantic>=1.10.4,<=2.8.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/unyime1/termii-py"
 "Bug Tracker" = "https://github.com/unyime1/termii-py/issues"
```

### Comparing `termii_py-0.1.5/PKG-INFO` & `termii_py-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: termii-py
-Version: 0.1.5
+Version: 0.1.6
 Summary: A beginner friendly SDK for Termii.
 Project-URL: Homepage, https://github.com/unyime1/termii-py
 Project-URL: Bug Tracker, https://github.com/unyime1/termii-py/issues
 Author-email: Unyime Etim <lordunyime@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

