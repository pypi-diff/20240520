# Comparing `tmp/DjangoSharepointStorage-1.0.0.tar.gz` & `tmp/DjangoSharepointStorage-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DjangoSharepointStorage-1.0.0.tar", last modified: Tue Nov 21 10:34:45 2023, max compression
+gzip compressed data, was "DjangoSharepointStorage-1.0.1.tar", last modified: Mon May 20 19:21:43 2024, max compression
```

## Comparing `DjangoSharepointStorage-1.0.0.tar` & `DjangoSharepointStorage-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 melihsunbul   (501) staff       (20)        0 2023-11-21 10:34:45.733226 DjangoSharepointStorage-1.0.0/
-drwxr-xr-x   0 melihsunbul   (501) staff       (20)        0 2023-11-21 10:34:45.731825 DjangoSharepointStorage-1.0.0/DjangoSharepointStorage.egg-info/
--rw-r--r--   0 melihsunbul   (501) staff       (20)     1711 2023-11-21 10:34:45.000000 DjangoSharepointStorage-1.0.0/DjangoSharepointStorage.egg-info/PKG-INFO
--rw-r--r--   0 melihsunbul   (501) staff       (20)      485 2023-11-21 10:34:45.000000 DjangoSharepointStorage-1.0.0/DjangoSharepointStorage.egg-info/SOURCES.txt
--rw-r--r--   0 melihsunbul   (501) staff       (20)        1 2023-11-21 10:34:45.000000 DjangoSharepointStorage-1.0.0/DjangoSharepointStorage.egg-info/dependency_links.txt
--rw-r--r--   0 melihsunbul   (501) staff       (20)       36 2023-11-21 10:34:45.000000 DjangoSharepointStorage-1.0.0/DjangoSharepointStorage.egg-info/requires.txt
--rw-r--r--   0 melihsunbul   (501) staff       (20)       26 2023-11-21 10:34:45.000000 DjangoSharepointStorage-1.0.0/DjangoSharepointStorage.egg-info/top_level.txt
--rw-r--r--   0 melihsunbul   (501) staff       (20)     1711 2023-11-21 10:34:45.733127 DjangoSharepointStorage-1.0.0/PKG-INFO
--rw-r--r--   0 melihsunbul   (501) staff       (20)      928 2023-11-21 10:32:47.000000 DjangoSharepointStorage-1.0.0/README.md
-drwxr-xr-x   0 melihsunbul   (501) staff       (20)        0 2023-11-21 10:34:45.733000 DjangoSharepointStorage-1.0.0/django_sharepoint_storage/
--rw-r--r--   0 melihsunbul   (501) staff       (20)      493 2023-11-21 10:32:47.000000 DjangoSharepointStorage-1.0.0/django_sharepoint_storage/SharePointClients.py
--rw-r--r--   0 melihsunbul   (501) staff       (20)      592 2023-11-21 10:32:47.000000 DjangoSharepointStorage-1.0.0/django_sharepoint_storage/SharePointCloudStorageUtils.py
--rw-r--r--   0 melihsunbul   (501) staff       (20)      735 2023-11-16 09:06:38.000000 DjangoSharepointStorage-1.0.0/django_sharepoint_storage/SharePointFile.py
--rw-r--r--   0 melihsunbul   (501) staff       (20)     2734 2023-11-21 10:32:47.000000 DjangoSharepointStorage-1.0.0/django_sharepoint_storage/SharePointStorage.py
--rw-r--r--   0 melihsunbul   (501) staff       (20)        0 2023-10-30 10:29:18.000000 DjangoSharepointStorage-1.0.0/django_sharepoint_storage/__init__.py
--rw-r--r--   0 melihsunbul   (501) staff       (20)       38 2023-11-21 10:34:45.733266 DjangoSharepointStorage-1.0.0/setup.cfg
--rw-r--r--   0 melihsunbul   (501) staff       (20)      853 2023-11-21 10:21:35.000000 DjangoSharepointStorage-1.0.0/setup.py
+drwxr-xr-x   0 melihsunbul   (501) staff       (20)        0 2024-05-20 19:21:43.145701 DjangoSharepointStorage-1.0.1/
+drwxr-xr-x   0 melihsunbul   (501) staff       (20)        0 2024-05-20 19:21:43.145352 DjangoSharepointStorage-1.0.1/DjangoSharepointStorage.egg-info/
+-rw-r--r--   0 melihsunbul   (501) staff       (20)     1507 2024-05-20 19:21:43.000000 DjangoSharepointStorage-1.0.1/DjangoSharepointStorage.egg-info/PKG-INFO
+-rw-r--r--   0 melihsunbul   (501) staff       (20)      497 2024-05-20 19:21:43.000000 DjangoSharepointStorage-1.0.1/DjangoSharepointStorage.egg-info/SOURCES.txt
+-rw-r--r--   0 melihsunbul   (501) staff       (20)        1 2024-05-20 19:21:43.000000 DjangoSharepointStorage-1.0.1/DjangoSharepointStorage.egg-info/dependency_links.txt
+-rw-r--r--   0 melihsunbul   (501) staff       (20)       36 2024-05-20 19:21:43.000000 DjangoSharepointStorage-1.0.1/DjangoSharepointStorage.egg-info/requires.txt
+-rw-r--r--   0 melihsunbul   (501) staff       (20)       26 2024-05-20 19:21:43.000000 DjangoSharepointStorage-1.0.1/DjangoSharepointStorage.egg-info/top_level.txt
+-rw-r--r--   0 melihsunbul   (501) staff       (20)     1071 2023-11-09 16:23:47.000000 DjangoSharepointStorage-1.0.1/LICENSE.txt
+-rw-r--r--   0 melihsunbul   (501) staff       (20)     1507 2024-05-20 19:21:43.145523 DjangoSharepointStorage-1.0.1/PKG-INFO
+-rw-r--r--   0 melihsunbul   (501) staff       (20)      928 2023-11-21 10:32:47.000000 DjangoSharepointStorage-1.0.1/README.md
+drwxr-xr-x   0 melihsunbul   (501) staff       (20)        0 2024-05-20 19:21:43.145208 DjangoSharepointStorage-1.0.1/django_sharepoint_storage/
+-rw-r--r--   0 melihsunbul   (501) staff       (20)      493 2023-11-21 10:32:47.000000 DjangoSharepointStorage-1.0.1/django_sharepoint_storage/SharePointClients.py
+-rw-r--r--   0 melihsunbul   (501) staff       (20)      592 2023-11-21 10:32:47.000000 DjangoSharepointStorage-1.0.1/django_sharepoint_storage/SharePointCloudStorageUtils.py
+-rw-r--r--   0 melihsunbul   (501) staff       (20)      735 2023-11-16 09:06:38.000000 DjangoSharepointStorage-1.0.1/django_sharepoint_storage/SharePointFile.py
+-rw-r--r--   0 melihsunbul   (501) staff       (20)     3277 2024-05-20 19:18:56.000000 DjangoSharepointStorage-1.0.1/django_sharepoint_storage/SharePointStorage.py
+-rw-r--r--   0 melihsunbul   (501) staff       (20)        0 2023-10-30 10:29:18.000000 DjangoSharepointStorage-1.0.1/django_sharepoint_storage/__init__.py
+-rw-r--r--   0 melihsunbul   (501) staff       (20)       38 2024-05-20 19:21:43.145739 DjangoSharepointStorage-1.0.1/setup.cfg
+-rw-r--r--   0 melihsunbul   (501) staff       (20)      853 2024-05-20 19:21:27.000000 DjangoSharepointStorage-1.0.1/setup.py
```

### Comparing `DjangoSharepointStorage-1.0.0/README.md` & `DjangoSharepointStorage-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `DjangoSharepointStorage-1.0.0/django_sharepoint_storage/SharePointCloudStorageUtils.py` & `DjangoSharepointStorage-1.0.1/django_sharepoint_storage/SharePointCloudStorageUtils.py`

 * *Files identical despite different names*

### Comparing `DjangoSharepointStorage-1.0.0/django_sharepoint_storage/SharePointFile.py` & `DjangoSharepointStorage-1.0.1/django_sharepoint_storage/SharePointFile.py`

 * *Files identical despite different names*

### Comparing `DjangoSharepointStorage-1.0.0/django_sharepoint_storage/SharePointStorage.py` & `DjangoSharepointStorage-1.0.1/django_sharepoint_storage/SharePointStorage.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,41 +15,46 @@
     client_id = getattr(settings, 'SHAREPOINT_APP_CLIENT_ID', 'client_id')
     client_secret = getattr(settings, 'SHAREPOINT_APP_CLIENT_SECRET', 'client_secret')
 
     def __init__(self, location='uploads', *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.location = location
 
+    @classmethod
+    @staticmethod
+    def print_failure(retry_number, ex):
+        Logger.logger_msg(f"{retry_number}: {ex}")
+
     def _open(self, name, mode='rb'):
         from django_sharepoint_storage.SharePointCloudStorageUtils import get_server_relative_path
         if mode in ['r', 'rb']:
             file_url = self.url(name)
-            file = ctx.web.get_file_by_server_relative_path(get_server_relative_path(file_url)).execute_query()
+            file = ctx.web.get_file_by_server_relative_path(get_server_relative_path(file_url)).execute_query_retry(max_retry=5, timeout_secs=5, failure_callback=SharePointStorage.print_failure)
             binary_file = file.open_binary(ctx, get_server_relative_path(file_url))
             bytesio_object = BytesIO(binary_file.content)
             return bytesio_object
         elif mode in ['w', 'wb']:
             return SharePointFile(name, mode, self)
         else:
             raise ValueError(f"Unsupported file mode: {mode}")
 
     def _save(self, name, content):
         # Here, name will have the format 'upload_to/filename.ext'
         folder_path = f"Shared Documents/{os.getenv('DEPLOYMENT_ENVIRONMENT', 'LOCAL')}-{os.getenv('K8S_NAMESPACE', 'ENV')}/{os.getenv('KEYCLOAK_INTERNAL_CLIENT_ID', 'Local')}/{os.getenv('INSTANCE_RESOURCE_IDENTIFIER', f'{platform.node()}/{DB_NAME}')}/{self.location}/{os.path.dirname(name)}"
-        target_folder = ctx.web.ensure_folder_path(folder_path).get().select(["ServerRelativePath"]).execute_query()
+        target_folder = ctx.web.ensure_folder_path(folder_path).get().select(["ServerRelativePath"]).execute_query_retry(max_retry=5, timeout_secs=5, failure_callback=SharePointStorage.print_failure)
 
         file_content = content.read()
 
-        target_folder.upload_file(os.path.basename(name), file_content).execute_query()
+        target_folder.upload_file(os.path.basename(name), file_content).execute_query_retry(max_retry=5, timeout_secs=5, failure_callback=SharePointStorage.print_failure)
 
         return name
 
     def delete(self, name):
-        file = File.from_url(self.url(name)).with_credentials(client_credentials).execute_query()
-        file.delete_object().execute_query()
+        file = File.from_url(self.url(name)).with_credentials(client_credentials).execute_query_retry(max_retry=5, timeout_secs=5, failure_callback=SharePointStorage.print_failure)
+        file.delete_object().execute_query_retry(max_retry=5, timeout_secs=5, failure_callback=SharePointStorage.print_failure)
 
     def exists(self, name):
         return False
 
     def url(self, name):
         # Use the dirname of name as your upload_to equivalent
         return f"{self.sharepoint_url}/Shared Documents/{os.getenv('DEPLOYMENT_ENVIRONMENT', 'LOCAL')}-{os.getenv('K8S_NAMESPACE', 'ENV')}/{os.getenv('KEYCLOAK_INTERNAL_CLIENT_ID', 'Local')}/{os.getenv('INSTANCE_RESOURCE_IDENTIFIER', f'{platform.node()}/{DB_NAME}')}/{self.location}/{name}"
```

### Comparing `DjangoSharepointStorage-1.0.0/setup.py` & `DjangoSharepointStorage-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as readme_file:
     long_description = readme_file.read()
 
 setup(
     name="DjangoSharepointStorage",
-    version="1.0.0",
+    version="1.0.1",
     author="Melih Sünbül",
     author_email="m.sunbul@lund-it.com",
     description="A Python library to use SharePoint as storage backend for your Django application",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LundIT/DjangoSharepointStorage",
     packages=find_packages(),
```

