# Comparing `tmp/ecom-utils-1.3.8.tar.gz` & `tmp/ecom-utils-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecom-utils-1.3.8.tar", last modified: Wed Nov 22 15:30:19 2023, max compression
+gzip compressed data, was "ecom-utils-1.3.9.tar", last modified: Fri Nov 24 12:30:58 2023, max compression
```

## Comparing `ecom-utils-1.3.8.tar` & `ecom-utils-1.3.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-11-22 15:30:19.428946 ecom-utils-1.3.8/
--rw-rw-rw-   0        0        0     1142 2023-11-22 15:30:19.428946 ecom-utils-1.3.8/PKG-INFO
--rw-rw-rw-   0        0        0      446 2023-11-22 15:29:38.000000 ecom-utils-1.3.8/README.md
-drwxrwxrwx   0        0        0        0 2023-11-22 15:30:19.390864 ecom-utils-1.3.8/ecom_utils/
--rw-rw-rw-   0        0        0        0 2023-02-28 14:35:48.000000 ecom-utils-1.3.8/ecom_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-22 15:30:19.415275 ecom-utils-1.3.8/ecom_utils/pon/
--rw-rw-rw-   0        0        0        0 2023-02-28 14:35:48.000000 ecom-utils-1.3.8/ecom_utils/pon/__init__.py
--rw-rw-rw-   0        0        0     4846 2023-11-22 15:22:51.000000 ecom-utils-1.3.8/ecom_utils/pon/core.py
-drwxrwxrwx   0        0        0        0 2023-11-22 15:30:19.384025 ecom-utils-1.3.8/ecom_utils/scient/
-drwxrwxrwx   0        0        0        0 2023-11-22 15:30:19.416251 ecom-utils-1.3.8/ecom_utils/scient/airflow/
-drwxrwxrwx   0        0        0        0 2023-11-22 15:30:19.417227 ecom-utils-1.3.8/ecom_utils/scient/airflow/core/
--rw-rw-rw-   0        0        0      190 2023-02-28 14:35:48.000000 ecom-utils-1.3.8/ecom_utils/scient/airflow/core/__init__.py
--rw-rw-rw-   0        0        0     6833 2023-02-28 14:35:48.000000 ecom-utils-1.3.8/ecom_utils/scient/airflow/functions.py
-drwxrwxrwx   0        0        0        0 2023-11-22 15:30:19.418205 ecom-utils-1.3.8/ecom_utils/scient/airflow/sql/
-drwxrwxrwx   0        0        0        0 2023-11-22 15:30:19.419184 ecom-utils-1.3.8/ecom_utils/scient/airflow/sql/core/
--rw-rw-rw-   0        0        0     4503 2023-02-28 14:35:48.000000 ecom-utils-1.3.8/ecom_utils/scient/airflow/sql/core/base.py
-drwxrwxrwx   0        0        0        0 2023-11-22 15:30:19.421136 ecom-utils-1.3.8/ecom_utils/scient/airflow/sql/mssql/
--rw-rw-rw-   0        0        0     2583 2023-02-28 14:35:48.000000 ecom-utils-1.3.8/ecom_utils/scient/airflow/sql/mssql/functions.py
--rw-rw-rw-   0        0        0     2098 2023-02-28 14:35:48.000000 ecom-utils-1.3.8/ecom_utils/scient/airflow/sql/mssql/operators.py
--rw-rw-rw-   0        0        0     5951 2023-02-28 14:35:48.000000 ecom-utils-1.3.8/ecom_utils/scient/airflow/sql/operators.py
-drwxrwxrwx   0        0        0        0 2023-11-22 15:30:19.423088 ecom-utils-1.3.8/ecom_utils/scient/airflow/sql/postgres/
--rw-rw-rw-   0        0        0     1083 2023-02-28 14:35:48.000000 ecom-utils-1.3.8/ecom_utils/scient/airflow/sql/postgres/functions.py
--rw-rw-rw-   0        0        0     1622 2023-02-28 14:35:48.000000 ecom-utils-1.3.8/ecom_utils/scient/airflow/sql/postgres/operators.py
-drwxrwxrwx   0        0        0        0 2023-11-22 15:30:19.426995 ecom-utils-1.3.8/ecom_utils/tgd/
--rw-rw-rw-   0        0        0        0 2023-02-28 14:35:48.000000 ecom-utils-1.3.8/ecom_utils/tgd/__init__.py
--rw-rw-rw-   0        0        0     2462 2023-03-16 11:25:12.000000 ecom-utils-1.3.8/ecom_utils/tgd/base.py
--rw-rw-rw-   0        0        0     9285 2023-03-16 11:25:12.000000 ecom-utils-1.3.8/ecom_utils/tgd/core.py
-drwxrwxrwx   0        0        0        0 2023-11-22 15:30:19.413322 ecom-utils-1.3.8/ecom_utils.egg-info/
--rw-rw-rw-   0        0        0     1142 2023-11-22 15:30:19.000000 ecom-utils-1.3.8/ecom_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      703 2023-11-22 15:30:19.000000 ecom-utils-1.3.8/ecom_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-22 15:30:19.000000 ecom-utils-1.3.8/ecom_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-11-22 15:30:19.000000 ecom-utils-1.3.8/ecom_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-11-22 15:30:19.000000 ecom-utils-1.3.8/ecom_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-22 15:30:19.428946 ecom-utils-1.3.8/setup.cfg
--rw-rw-rw-   0        0        0     1339 2023-11-22 15:28:48.000000 ecom-utils-1.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-11-24 12:30:58.714805 ecom-utils-1.3.9/
+-rw-rw-rw-   0        0        0     1223 2023-11-24 12:30:58.714805 ecom-utils-1.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0      519 2023-11-24 12:29:08.000000 ecom-utils-1.3.9/README.md
+drwxrwxrwx   0        0        0        0 2023-11-24 12:30:58.661583 ecom-utils-1.3.9/ecom_utils/
+-rw-rw-rw-   0        0        0        0 2023-02-28 14:35:48.000000 ecom-utils-1.3.9/ecom_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-11-24 12:30:58.698572 ecom-utils-1.3.9/ecom_utils/pon/
+-rw-rw-rw-   0        0        0        0 2023-02-28 14:35:48.000000 ecom-utils-1.3.9/ecom_utils/pon/__init__.py
+-rw-rw-rw-   0        0        0     4846 2023-11-22 15:22:51.000000 ecom-utils-1.3.9/ecom_utils/pon/core.py
+drwxrwxrwx   0        0        0        0 2023-11-24 12:30:58.654752 ecom-utils-1.3.9/ecom_utils/scient/
+drwxrwxrwx   0        0        0        0 2023-11-24 12:30:58.699548 ecom-utils-1.3.9/ecom_utils/scient/airflow/
+drwxrwxrwx   0        0        0        0 2023-11-24 12:30:58.701502 ecom-utils-1.3.9/ecom_utils/scient/airflow/core/
+-rw-rw-rw-   0        0        0      190 2023-02-28 14:35:48.000000 ecom-utils-1.3.9/ecom_utils/scient/airflow/core/__init__.py
+-rw-rw-rw-   0        0        0     6833 2023-02-28 14:35:48.000000 ecom-utils-1.3.9/ecom_utils/scient/airflow/functions.py
+drwxrwxrwx   0        0        0        0 2023-11-24 12:30:58.703455 ecom-utils-1.3.9/ecom_utils/scient/airflow/sql/
+drwxrwxrwx   0        0        0        0 2023-11-24 12:30:58.705046 ecom-utils-1.3.9/ecom_utils/scient/airflow/sql/core/
+-rw-rw-rw-   0        0        0     4503 2023-02-28 14:35:48.000000 ecom-utils-1.3.9/ecom_utils/scient/airflow/sql/core/base.py
+drwxrwxrwx   0        0        0        0 2023-11-24 12:30:58.707968 ecom-utils-1.3.9/ecom_utils/scient/airflow/sql/mssql/
+-rw-rw-rw-   0        0        0     2583 2023-02-28 14:35:48.000000 ecom-utils-1.3.9/ecom_utils/scient/airflow/sql/mssql/functions.py
+-rw-rw-rw-   0        0        0     2098 2023-02-28 14:35:48.000000 ecom-utils-1.3.9/ecom_utils/scient/airflow/sql/mssql/operators.py
+-rw-rw-rw-   0        0        0     5951 2023-02-28 14:35:48.000000 ecom-utils-1.3.9/ecom_utils/scient/airflow/sql/operators.py
+drwxrwxrwx   0        0        0        0 2023-11-24 12:30:58.709920 ecom-utils-1.3.9/ecom_utils/scient/airflow/sql/postgres/
+-rw-rw-rw-   0        0        0     1083 2023-02-28 14:35:48.000000 ecom-utils-1.3.9/ecom_utils/scient/airflow/sql/postgres/functions.py
+-rw-rw-rw-   0        0        0     1622 2023-02-28 14:35:48.000000 ecom-utils-1.3.9/ecom_utils/scient/airflow/sql/postgres/operators.py
+drwxrwxrwx   0        0        0        0 2023-11-24 12:30:58.713826 ecom-utils-1.3.9/ecom_utils/tgd/
+-rw-rw-rw-   0        0        0        0 2023-02-28 14:35:48.000000 ecom-utils-1.3.9/ecom_utils/tgd/__init__.py
+-rw-rw-rw-   0        0        0     2499 2023-11-24 12:30:26.000000 ecom-utils-1.3.9/ecom_utils/tgd/base.py
+-rw-rw-rw-   0        0        0     9285 2023-03-16 11:25:12.000000 ecom-utils-1.3.9/ecom_utils/tgd/core.py
+drwxrwxrwx   0        0        0        0 2023-11-24 12:30:58.695643 ecom-utils-1.3.9/ecom_utils.egg-info/
+-rw-rw-rw-   0        0        0     1223 2023-11-24 12:30:58.000000 ecom-utils-1.3.9/ecom_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      703 2023-11-24 12:30:58.000000 ecom-utils-1.3.9/ecom_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-11-24 12:30:58.000000 ecom-utils-1.3.9/ecom_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-11-24 12:30:58.000000 ecom-utils-1.3.9/ecom_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-11-24 12:30:58.000000 ecom-utils-1.3.9/ecom_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-11-24 12:30:58.715779 ecom-utils-1.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     1339 2023-11-24 12:29:22.000000 ecom-utils-1.3.9/setup.py
```

### Comparing `ecom-utils-1.3.8/PKG-INFO` & `ecom-utils-1.3.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ecom-utils
-Version: 1.3.8
+Version: 1.3.9
 Summary: Core de módulos para PyPI
 Home-page: https://git.ecom.com.ar/python-dev/ecom-utils
 Author: Ecom Developers
 Author-email: simono@ecom.com.ar
 License: BSD
 Description: # ECOM UTILS
         
@@ -16,14 +16,15 @@
         python setup.py sdist
         twine upload dist/*
         
         pip install --upgrade ecom-utils
         
         
         ## Versiones
+            1.3.9 - Modulo TGD - se modifico url base en stage (ENDPOINT_STAGE)
             1.3.8 - Modulo PON - Se agrego consulta de cargos de agente
             1.3.7 - Actualizacion endpoint prod modulo PON
             1.3.6 - Fix a conexiÃ³n al nuevo y quitando logs.
             1.3.0 - ActualizaciÃ³n a nueva versiÃ³n de TGD. Se mantiene llamada a versiÃ³n vieja.
             
 Keywords: ecom utils
 Platform: UNKNOWN
```

### Comparing `ecom-utils-1.3.8/ecom_utils/pon/core.py` & `ecom-utils-1.3.9/ecom_utils/pon/core.py`

 * *Files identical despite different names*

### Comparing `ecom-utils-1.3.8/ecom_utils/scient/airflow/functions.py` & `ecom-utils-1.3.9/ecom_utils/scient/airflow/functions.py`

 * *Files identical despite different names*

### Comparing `ecom-utils-1.3.8/ecom_utils/scient/airflow/sql/core/base.py` & `ecom-utils-1.3.9/ecom_utils/scient/airflow/sql/core/base.py`

 * *Files identical despite different names*

### Comparing `ecom-utils-1.3.8/ecom_utils/scient/airflow/sql/mssql/functions.py` & `ecom-utils-1.3.9/ecom_utils/scient/airflow/sql/mssql/functions.py`

 * *Files identical despite different names*

### Comparing `ecom-utils-1.3.8/ecom_utils/scient/airflow/sql/mssql/operators.py` & `ecom-utils-1.3.9/ecom_utils/scient/airflow/sql/mssql/operators.py`

 * *Files identical despite different names*

### Comparing `ecom-utils-1.3.8/ecom_utils/scient/airflow/sql/operators.py` & `ecom-utils-1.3.9/ecom_utils/scient/airflow/sql/operators.py`

 * *Files identical despite different names*

### Comparing `ecom-utils-1.3.8/ecom_utils/scient/airflow/sql/postgres/functions.py` & `ecom-utils-1.3.9/ecom_utils/scient/airflow/sql/postgres/functions.py`

 * *Files identical despite different names*

### Comparing `ecom-utils-1.3.8/ecom_utils/scient/airflow/sql/postgres/operators.py` & `ecom-utils-1.3.9/ecom_utils/scient/airflow/sql/postgres/operators.py`

 * *Files identical despite different names*

### Comparing `ecom-utils-1.3.8/ecom_utils/tgd/base.py` & `ecom-utils-1.3.9/ecom_utils/tgd/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
                        'get_token_application': '_endpointbase_/oauth/v2/token',
                        'get_persona_via_cuil': '_endpointbase_/api/v1/persona/cuil/_cuil_',
                        'get_persona_via_token': '_endpointbase_/api/v1/persona',
                        'Content-Type': 'application/json'
                    }
                    },
 
-            "V1.1": {"ENDPOINT_STAGE": 'https://core.tgdpruebas.chaco.gob.ar',
+            "V1.1": {"ENDPOINT_STAGE": "https://tgdpruebas.chaco.gob.ar", # 'https://core.tgdpruebas.chaco.gob.ar',
                      "ENDPOINT_PROD": 'https://gobiernodigital.chaco.gob.ar',
                      "API_ENDPOINTS": {
                          'oauth_base_uri': '_endpointbase_',
                          'get_token_via_authorization_code': '_endpointbase_/token',
                          'get_token_application': '_endpointbase_/token',
                          'get_persona_via_cuil': '_endpointbase_/api/v2/persona/cuil/_cuil_',
                          'get_persona_via_token': '_endpointbase_/api/v2/persona',
```

### Comparing `ecom-utils-1.3.8/ecom_utils/tgd/core.py` & `ecom-utils-1.3.9/ecom_utils/tgd/core.py`

 * *Files identical despite different names*

### Comparing `ecom-utils-1.3.8/ecom_utils.egg-info/PKG-INFO` & `ecom-utils-1.3.9/ecom_utils.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ecom-utils
-Version: 1.3.8
+Version: 1.3.9
 Summary: Core de módulos para PyPI
 Home-page: https://git.ecom.com.ar/python-dev/ecom-utils
 Author: Ecom Developers
 Author-email: simono@ecom.com.ar
 License: BSD
 Description: # ECOM UTILS
         
@@ -16,14 +16,15 @@
         python setup.py sdist
         twine upload dist/*
         
         pip install --upgrade ecom-utils
         
         
         ## Versiones
+            1.3.9 - Modulo TGD - se modifico url base en stage (ENDPOINT_STAGE)
             1.3.8 - Modulo PON - Se agrego consulta de cargos de agente
             1.3.7 - Actualizacion endpoint prod modulo PON
             1.3.6 - Fix a conexiÃ³n al nuevo y quitando logs.
             1.3.0 - ActualizaciÃ³n a nueva versiÃ³n de TGD. Se mantiene llamada a versiÃ³n vieja.
             
 Keywords: ecom utils
 Platform: UNKNOWN
```

### Comparing `ecom-utils-1.3.8/ecom_utils.egg-info/SOURCES.txt` & `ecom-utils-1.3.9/ecom_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ecom-utils-1.3.8/setup.py` & `ecom-utils-1.3.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     except Exception as e:
         print("Ha ocurrido un inconveniente: " + str(e))
     return readme_txt
 
 
 setup(
     name='ecom-utils',
-    version='1.3.8',
+    version='1.3.9',
     author='Ecom Developers',
     author_email='simono@ecom.com.ar',
     description=('Core de módulos para PyPI'),
     long_description=get_readme(),
     license='BSD',
     keywords='ecom utils',
     url='https://git.ecom.com.ar/python-dev/ecom-utils',
```

