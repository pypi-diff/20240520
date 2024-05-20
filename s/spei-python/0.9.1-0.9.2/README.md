# Comparing `tmp/spei_python-0.9.1.tar.gz` & `tmp/spei_python-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spei_python-0.9.1.tar", max compression
+gzip compressed data, was "spei_python-0.9.2.tar", max compression
```

## Comparing `spei_python-0.9.1.tar` & `spei_python-0.9.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      999 2023-02-15 18:15:34.283809 spei_python-0.9.1/README.md
--rw-r--r--   0        0        0      879 2023-08-18 17:38:14.811570 spei_python-0.9.1/pyproject.toml
--rw-r--r--   0        0        0       49 2022-07-27 23:08:37.464131 spei_python-0.9.1/spei/__init__.py
--rw-r--r--   0        0        0     1956 2023-08-18 16:39:35.648617 spei_python-0.9.1/spei/client.py
--rw-r--r--   0        0        0      126 2023-08-18 16:39:35.648617 spei_python-0.9.1/spei/requests/__init__.py
--rw-r--r--   0        0        0     1168 2023-08-18 16:39:35.648617 spei_python-0.9.1/spei/requests/orden.py
--rw-r--r--   0        0        0     1022 2023-08-18 17:38:14.811570 spei_python-0.9.1/spei/requests/respuesta.py
--rw-r--r--   0        0        0      114 2023-08-18 16:39:35.648617 spei_python-0.9.1/spei/resources/__init__.py
--rw-r--r--   0        0        0     3359 2023-08-18 16:39:35.648617 spei_python-0.9.1/spei/resources/orden.py
--rw-r--r--   0        0        0     1698 2023-08-18 16:39:35.648617 spei_python-0.9.1/spei/resources/respuesta.py
--rw-r--r--   0        0        0     2788 2023-08-17 22:19:32.277618 spei_python-0.9.1/spei/types.py
--rw-r--r--   0        0        0     2272 2023-06-08 21:05:13.625019 spei_python-0.9.1/spei/utils.py
--rw-r--r--   0        0        0      742 2023-08-17 22:19:32.277618 spei_python-0.9.1/spei/validators.py
--rw-r--r--   0        0        0     1643 1970-01-01 00:00:00.000000 spei_python-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0      999 2023-02-15 18:15:34.283809 spei_python-0.9.2/README.md
+-rw-r--r--   0        0        0      879 2023-08-18 18:35:40.200584 spei_python-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0       49 2022-07-27 23:08:37.464131 spei_python-0.9.2/spei/__init__.py
+-rw-r--r--   0        0        0     1956 2023-08-18 16:39:35.648617 spei_python-0.9.2/spei/client.py
+-rw-r--r--   0        0        0      126 2023-08-18 16:39:35.648617 spei_python-0.9.2/spei/requests/__init__.py
+-rw-r--r--   0        0        0     1168 2023-08-18 16:39:35.648617 spei_python-0.9.2/spei/requests/orden.py
+-rw-r--r--   0        0        0     1054 2023-08-18 18:35:02.975544 spei_python-0.9.2/spei/requests/respuesta.py
+-rw-r--r--   0        0        0      114 2023-08-18 16:39:35.648617 spei_python-0.9.2/spei/resources/__init__.py
+-rw-r--r--   0        0        0     3359 2023-08-18 16:39:35.648617 spei_python-0.9.2/spei/resources/orden.py
+-rw-r--r--   0        0        0     1698 2023-08-18 16:39:35.648617 spei_python-0.9.2/spei/resources/respuesta.py
+-rw-r--r--   0        0        0     2788 2023-08-17 22:19:32.277618 spei_python-0.9.2/spei/types.py
+-rw-r--r--   0        0        0     2272 2023-06-08 21:05:13.625019 spei_python-0.9.2/spei/utils.py
+-rw-r--r--   0        0        0      742 2023-08-17 22:19:32.277618 spei_python-0.9.2/spei/validators.py
+-rw-r--r--   0        0        0     1643 1970-01-01 00:00:00.000000 spei_python-0.9.2/PKG-INFO
```

### Comparing `spei_python-0.9.1/README.md` & `spei_python-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `spei_python-0.9.1/pyproject.toml` & `spei_python-0.9.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spei-python"
-version = "0.9.1"
+version = "0.9.2"
 description = ""
 authors = ["gonz <gonzasestopal@gmail.com>"]
 readme = "README.md"
 packages = [{include = "spei"}]
 
 [tool.poetry.dependencies]
 python = "^3.7"
@@ -28,13 +28,13 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.9.1"
+version = "0.9.2"
 tag_format = "v$version"
 bump_message = "bump: Semantic Release Bot: Release Version: $new_version 🤖🚀 [skip ci]"
 version_files = [
     "pyproject.toml:version",
 ]
```

### Comparing `spei_python-0.9.1/spei/client.py` & `spei_python-0.9.2/spei/client.py`

 * *Files identical despite different names*

### Comparing `spei_python-0.9.1/spei/requests/orden.py` & `spei_python-0.9.2/spei/requests/orden.py`

 * *Files identical despite different names*

### Comparing `spei_python-0.9.1/spei/requests/respuesta.py` & `spei_python-0.9.2/spei/requests/respuesta.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 SOAP_NS = 'http://schemas.xmlsoap.org/soap/envelope/'
 PRAXIS_NS = 'http://www.praxis.com.mx/'
 
 
 class Respuesta(object):
     def __new__(cls, mensaje_xml):
-        respuesta = etree.Element('respuesta', xlmns=PRAXIS_NS)
+        respuesta = etree.Element(etree.QName(PRAXIS_NS, 'respuesta'), nsmap={None: PRAXIS_NS})
         mensaje = etree.tostring(mensaje_xml, xml_declaration=True, encoding='cp850')
         respuesta.text = mensaje
         return respuesta
 
 
 class Body(object):
     def __new__(cls, respuesta):
```

### Comparing `spei_python-0.9.1/spei/resources/orden.py` & `spei_python-0.9.2/spei/resources/orden.py`

 * *Files identical despite different names*

### Comparing `spei_python-0.9.1/spei/resources/respuesta.py` & `spei_python-0.9.2/spei/resources/respuesta.py`

 * *Files identical despite different names*

### Comparing `spei_python-0.9.1/spei/types.py` & `spei_python-0.9.2/spei/types.py`

 * *Files identical despite different names*

### Comparing `spei_python-0.9.1/spei/utils.py` & `spei_python-0.9.2/spei/utils.py`

 * *Files identical despite different names*

### Comparing `spei_python-0.9.1/spei/validators.py` & `spei_python-0.9.2/spei/validators.py`

 * *Files identical despite different names*

### Comparing `spei_python-0.9.1/PKG-INFO` & `spei_python-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spei-python
-Version: 0.9.1
+Version: 0.9.2
 Summary: 
 Author: gonz
 Author-email: gonzasestopal@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

