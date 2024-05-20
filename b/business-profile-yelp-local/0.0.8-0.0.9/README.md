# Comparing `tmp/business-profile-yelp-local-0.0.8.tar.gz` & `tmp/business-profile-yelp-local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "business-profile-yelp-local-0.0.8.tar", last modified: Sun Nov 26 05:58:51 2023, max compression
+gzip compressed data, was "business-profile-yelp-local-0.0.9.tar", last modified: Sun Nov 26 06:04:38 2023, max compression
```

## Comparing `business-profile-yelp-local-0.0.8.tar` & `business-profile-yelp-local-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 05:58:51.952328 business-profile-yelp-local-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 05:58:51.952328 business-profile-yelp-local-0.0.8/LocalYelpPython/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 05:58:51.952328 business-profile-yelp-local-0.0.8/LocalYelpPython/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-26 05:58:15.000000 business-profile-yelp-local-0.0.8/LocalYelpPython/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5223 2023-11-26 05:58:15.000000 business-profile-yelp-local-0.0.8/LocalYelpPython/src/yelpImporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2023-11-26 05:58:51.952328 business-profile-yelp-local-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      315 2023-11-26 05:58:15.000000 business-profile-yelp-local-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 05:58:51.952328 business-profile-yelp-local-0.0.8/business_profile_yelp_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      589 2023-11-26 05:58:51.000000 business-profile-yelp-local-0.0.8/business_profile_yelp_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      340 2023-11-26 05:58:51.000000 business-profile-yelp-local-0.0.8/business_profile_yelp_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-26 05:58:51.000000 business-profile-yelp-local-0.0.8/business_profile_yelp_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2023-11-26 05:58:51.000000 business-profile-yelp-local-0.0.8/business_profile_yelp_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-11-26 05:58:51.000000 business-profile-yelp-local-0.0.8/business_profile_yelp_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-26 05:58:51.952328 business-profile-yelp-local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      964 2023-11-26 05:58:15.000000 business-profile-yelp-local-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 06:04:38.265751 business-profile-yelp-local-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 06:04:38.261751 business-profile-yelp-local-0.0.9/LocalYelpPython/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 06:04:38.261751 business-profile-yelp-local-0.0.9/LocalYelpPython/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-26 06:03:56.000000 business-profile-yelp-local-0.0.9/LocalYelpPython/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5275 2023-11-26 06:03:56.000000 business-profile-yelp-local-0.0.9/LocalYelpPython/src/yelpImporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2023-11-26 06:04:38.265751 business-profile-yelp-local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2023-11-26 06:03:56.000000 business-profile-yelp-local-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 06:04:38.261751 business-profile-yelp-local-0.0.9/business_profile_yelp_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2023-11-26 06:04:38.000000 business-profile-yelp-local-0.0.9/business_profile_yelp_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2023-11-26 06:04:38.000000 business-profile-yelp-local-0.0.9/business_profile_yelp_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-26 06:04:38.000000 business-profile-yelp-local-0.0.9/business_profile_yelp_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2023-11-26 06:04:38.000000 business-profile-yelp-local-0.0.9/business_profile_yelp_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2023-11-26 06:04:38.000000 business-profile-yelp-local-0.0.9/business_profile_yelp_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-26 06:04:38.265751 business-profile-yelp-local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2023-11-26 06:03:56.000000 business-profile-yelp-local-0.0.9/setup.py
```

### Comparing `business-profile-yelp-local-0.0.8/LocalYelpPython/src/yelpImporter.py` & `business-profile-yelp-local-0.0.9/LocalYelpPython/src/yelpImporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 LOCAL_YELP_COMPONENT_ID = 156
 
 
 class YelpImporter:
     def __init__(self):
         self.logger = Logger(object={'component_id': LOCAL_YELP_COMPONENT_ID})
 
-    def get_data(self, business_type: str, location: str, total_entries: int = 1000):
+    def get_data(self, business_type: str, location: str, total_entries: int = 10):
         self.logger.start("Fetching business data from Yelp GraphQL",
                           object={"component_id": LOCAL_YELP_COMPONENT_ID, "component_name": "Local yelp importer"})
 
         query = gql('''
           query ($term: String!, $location: String!, $limit: Int!, $offset: Int!) {
             search(term: $term, location: $location, limit: $limit, offset: $offset) {
               business {
@@ -117,13 +117,14 @@
     # def insert_profile_and_update_importer(self, conn = connect()):
     # entity_id = profile generic package
     #   my_importer = importer.Importer("Yelp.com GraphQL", 1)
 
     #   my_importer.insert_record_data_source(
     #           "United States", "Business Profile", entity_id, "https://api.yelp.com/v3/graphql")
 
+    # TODO Let's move this to python-sdk repo time.py
     @staticmethod
     def reformat_time_string(input_str: str) -> str:
         hours = input_str[:2]
         minutes = input_str[2:]
         time_format = f"{hours}:{minutes}:00:00"
         return time_format
```

### Comparing `business-profile-yelp-local-0.0.8/PKG-INFO` & `business-profile-yelp-local-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: business-profile-yelp-local
-Version: 0.0.8
+Version: 0.0.9
 Home-page: https://github.com/circles-zone/business-profile-yelp-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `business-profile-yelp-local-0.0.8/business_profile_yelp_local.egg-info/PKG-INFO` & `business-profile-yelp-local-0.0.9/business_profile_yelp_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: business-profile-yelp-local
-Version: 0.0.8
+Version: 0.0.9
 Home-page: https://github.com/circles-zone/business-profile-yelp-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `business-profile-yelp-local-0.0.8/setup.py` & `business-profile-yelp-local-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "business-profile-yelp-local"
 package_dir = "LocalYelpPython"
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/business-profile-yelp-local
-    version='0.0.8',
+    version='0.0.9',
     author="Circles",
     author_email="info@circles.life",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="This package is used to import business profiles from Yelp.com.",
```

