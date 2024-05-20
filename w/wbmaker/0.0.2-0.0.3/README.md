# Comparing `tmp/wbmaker-0.0.2.tar.gz` & `tmp/wbmaker-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wbmaker-0.0.2.tar", max compression
+gzip compressed data, was "wbmaker-0.0.3.tar", max compression
```

## Comparing `wbmaker-0.0.2.tar` & `wbmaker-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2024-05-10 22:05:47.248777 wbmaker-0.0.2/LICENSE
--rw-r--r--   0        0        0      492 2024-05-10 22:11:14.772671 wbmaker-0.0.2/README.md
--rw-r--r--   0        0        0      475 2024-05-13 18:16:58.427663 wbmaker-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-10 22:05:47.250351 wbmaker-0.0.2/wbmaker/__init__.py
--rw-r--r--   0        0        0     4663 2024-05-13 18:16:48.198894 wbmaker-0.0.2/wbmaker/wb.py
--rw-r--r--   0        0        0     1145 1970-01-01 00:00:00.000000 wbmaker-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-10 22:05:47.248777 wbmaker-0.0.3/LICENSE
+-rw-r--r--   0        0        0      492 2024-05-10 22:11:14.772671 wbmaker-0.0.3/README.md
+-rw-r--r--   0        0        0      475 2024-05-20 18:43:57.046710 wbmaker-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-10 22:05:47.250351 wbmaker-0.0.3/wbmaker/__init__.py
+-rw-r--r--   0        0        0     4797 2024-05-20 18:43:52.999122 wbmaker-0.0.3/wbmaker/wb.py
+-rw-r--r--   0        0        0     1145 1970-01-01 00:00:00.000000 wbmaker-0.0.3/PKG-INFO
```

### Comparing `wbmaker-0.0.2/LICENSE` & `wbmaker-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wbmaker-0.0.2/wbmaker/wb.py` & `wbmaker-0.0.3/wbmaker/wb.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,25 +99,27 @@
                 df['identifier'] = df.iloc[:, 0].apply(lambda x: x.split('/')[-1])
                 return df[['lookup_value','identifier']].set_index('lookup_value').to_dict()['identifier']
             else:
                 return data_records
     
     def property_map(self):
         q_props = """
-        SELECT ?property ?propertyLabel WHERE {
-        ?property a wikibase:Property .
-        SERVICE wikibase:label { bd:serviceParam wikibase:language "[AUTO_LANGUAGE],en". }
+        SELECT ?property ?propertyLabel ?dataType
+        WHERE {
+        ?property a wikibase:Property ;
+                  wikibase:propertyType ?dataType .
+        SERVICE wikibase:label { bd:serviceParam wikibase:language "en". }
         }
         """
 
         props = self.sparql_query(q_props)
-        props['pid'] = props['property'].str.split('/').str[-1]
-
-        return props.set_index('propertyLabel')['pid'].to_dict()
+        props['property'] = props['property'].str.split('/').str[-1]
+        props['dataType'] = props['dataType'].str.split('#').str[-1]
 
+        return props.set_index('propertyLabel').to_dict(orient='index')
 
     def wb_dt(self, dt=datetime.now()):
         '''
         Converts a string (or datetime object) to a proper Wikibase datetime string
         '''
         if not isinstance(dt, datetime):
             try:
```

### Comparing `wbmaker-0.0.2/PKG-INFO` & `wbmaker-0.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbmaker
-Version: 0.0.2
+Version: 0.0.3
 Summary: Establishes a connection to a Wikibase instance and provides methods for interacting with it.
 Author: Sky Bristol
 Author-email: skybristol@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

