# Comparing `tmp/aiodocker-0.8.5.tar.gz` & `tmp/aiodocker-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aiodocker-0.8.5.tar", last modified: Sun Nov 12 09:56:50 2017, max compression
+gzip compressed data, was "dist/aiodocker-0.9.0.tar", last modified: Sun Feb 11 16:10:27 2018, max compression
```

## Comparing `aiodocker-0.8.5.tar` & `aiodocker-0.9.0.tar`

### file list

```diff
@@ -1,57 +1,59 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-11-12 09:56:50.000000 aiodocker-0.8.5/
--rw-rw-r--   0 travis    (2000) travis    (2000)      179 2017-11-12 09:55:26.000000 aiodocker-0.8.5/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     2189 2017-11-12 09:55:26.000000 aiodocker-0.8.5/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-11-12 09:56:50.000000 aiodocker-0.8.5/aiodocker/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5470 2017-11-12 09:55:26.000000 aiodocker-0.8.5/aiodocker/services.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1401 2017-11-12 09:55:26.000000 aiodocker-0.8.5/aiodocker/jsonstream.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      928 2017-11-12 09:55:26.000000 aiodocker-0.8.5/aiodocker/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8186 2017-11-12 09:55:26.000000 aiodocker-0.8.5/aiodocker/containers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      566 2017-11-12 09:55:26.000000 aiodocker-0.8.5/aiodocker/channel.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8833 2017-11-12 09:55:26.000000 aiodocker-0.8.5/aiodocker/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       29 2017-11-12 09:55:26.000000 aiodocker-0.8.5/aiodocker/constants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6818 2017-11-12 09:55:26.000000 aiodocker-0.8.5/aiodocker/docker.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2873 2017-11-12 09:55:26.000000 aiodocker-0.8.5/aiodocker/events.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1139 2017-11-12 09:55:26.000000 aiodocker-0.8.5/aiodocker/tasks.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1895 2017-11-12 09:55:26.000000 aiodocker-0.8.5/aiodocker/swarm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1768 2017-11-12 09:55:26.000000 aiodocker-0.8.5/aiodocker/logs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       76 2017-11-12 09:55:26.000000 aiodocker-0.8.5/aiodocker/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2071 2017-11-12 09:55:26.000000 aiodocker-0.8.5/aiodocker/multiplexed.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      980 2017-11-12 09:55:26.000000 aiodocker-0.8.5/aiodocker/volumes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7749 2017-11-12 09:55:26.000000 aiodocker-0.8.5/aiodocker/images.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10177 2017-11-12 09:55:26.000000 aiodocker-0.8.5/LICENSE
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-11-12 09:56:50.000000 aiodocker-0.8.5/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4676 2017-11-12 09:55:26.000000 aiodocker-0.8.5/tests/test_images.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2079 2017-11-12 09:55:26.000000 aiodocker-0.8.5/tests/test_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      911 2017-11-12 09:55:26.000000 aiodocker-0.8.5/tests/test_events.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-11-12 09:56:50.000000 aiodocker-0.8.5/tests/certs/
--rw-rw-r--   0 travis    (2000) travis    (2000)       71 2017-11-12 09:55:26.000000 aiodocker-0.8.5/tests/certs/htpasswd
--rw-rw-r--   0 travis    (2000) travis    (2000)     4380 2017-11-12 09:55:26.000000 aiodocker-0.8.5/tests/certs/registry.crt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1679 2017-11-12 09:55:26.000000 aiodocker-0.8.5/tests/certs/registry.key
--rw-rw-r--   0 travis    (2000) travis    (2000)     2174 2017-11-12 09:55:26.000000 aiodocker-0.8.5/tests/test_containers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4093 2017-11-12 09:55:26.000000 aiodocker-0.8.5/tests/test_services.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-11-12 09:56:50.000000 aiodocker-0.8.5/tests/docker/
--rw-rw-r--   0 travis    (2000) travis    (2000)       76 2017-11-12 09:55:26.000000 aiodocker-0.8.5/tests/docker/Dockerfile
--rw-rw-r--   0 travis    (2000) travis    (2000)     3584 2017-11-12 09:55:26.000000 aiodocker-0.8.5/tests/docker/docker_context.tar
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-11-12 09:56:50.000000 aiodocker-0.8.5/tests/docker/tar/
--rw-rw-r--   0 travis    (2000) travis    (2000)      189 2017-11-12 09:55:26.000000 aiodocker-0.8.5/tests/docker/tar/app.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       99 2017-11-12 09:55:26.000000 aiodocker-0.8.5/tests/docker/tar/Dockerfile
--rw-rw-r--   0 travis    (2000) travis    (2000)      220 2017-11-12 09:55:26.000000 aiodocker-0.8.5/tests/docker/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     4673 2017-11-12 09:55:26.000000 aiodocker-0.8.5/tests/conftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7994 2017-11-12 09:55:26.000000 aiodocker-0.8.5/tests/test_integration.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2017-11-12 09:56:50.000000 aiodocker-0.8.5/setup.cfg
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1577 2017-11-12 09:55:26.000000 aiodocker-0.8.5/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-11-12 09:56:50.000000 aiodocker-0.8.5/aiodocker.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)       26 2017-11-12 09:56:50.000000 aiodocker-0.8.5/aiodocker.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1017 2017-11-12 09:56:50.000000 aiodocker-0.8.5/aiodocker.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2017-11-12 09:56:50.000000 aiodocker-0.8.5/aiodocker.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     4233 2017-11-12 09:56:50.000000 aiodocker-0.8.5/aiodocker.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)       10 2017-11-12 09:56:50.000000 aiodocker-0.8.5/aiodocker.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     4233 2017-11-12 09:56:50.000000 aiodocker-0.8.5/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      473 2017-11-12 09:55:26.000000 aiodocker-0.8.5/CHANGES.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-11-12 09:56:50.000000 aiodocker-0.8.5/requirements/
--rw-rw-r--   0 travis    (2000) travis    (2000)       80 2017-11-12 09:55:26.000000 aiodocker-0.8.5/requirements/test.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       26 2017-11-12 09:55:26.000000 aiodocker-0.8.5/requirements/base.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-11-12 09:56:50.000000 aiodocker-0.8.5/examples/
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1189 2017-11-12 09:55:26.000000 aiodocker-0.8.5/examples/info.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1888 2017-11-12 09:55:26.000000 aiodocker-0.8.5/examples/events.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1790 2017-11-12 09:55:26.000000 aiodocker-0.8.5/examples/stdio_stdout.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-11 16:10:27.000000 aiodocker-0.9.0/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-11 16:10:27.000000 aiodocker-0.9.0/aiodocker/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      980 2018-02-11 16:07:55.000000 aiodocker-0.9.0/aiodocker/volumes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2873 2018-02-11 16:07:55.000000 aiodocker-0.9.0/aiodocker/events.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       29 2018-02-11 16:07:55.000000 aiodocker-0.9.0/aiodocker/constants.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7113 2018-02-11 16:07:55.000000 aiodocker-0.9.0/aiodocker/docker.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1139 2018-02-11 16:07:55.000000 aiodocker-0.9.0/aiodocker/tasks.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      928 2018-02-11 16:07:55.000000 aiodocker-0.9.0/aiodocker/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7749 2018-02-11 16:07:55.000000 aiodocker-0.9.0/aiodocker/images.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1895 2018-02-11 16:07:55.000000 aiodocker-0.9.0/aiodocker/swarm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       76 2018-02-11 16:07:55.000000 aiodocker-0.9.0/aiodocker/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8186 2018-02-11 16:07:55.000000 aiodocker-0.9.0/aiodocker/containers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6710 2018-02-11 16:07:55.000000 aiodocker-0.9.0/aiodocker/services.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2071 2018-02-11 16:07:55.000000 aiodocker-0.9.0/aiodocker/multiplexed.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      566 2018-02-11 16:07:55.000000 aiodocker-0.9.0/aiodocker/channel.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1401 2018-02-11 16:07:55.000000 aiodocker-0.9.0/aiodocker/jsonstream.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2371 2018-02-11 16:07:55.000000 aiodocker-0.9.0/aiodocker/nodes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8679 2018-02-11 16:07:55.000000 aiodocker-0.9.0/aiodocker/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1768 2018-02-11 16:07:55.000000 aiodocker-0.9.0/aiodocker/logs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2189 2018-02-11 16:07:55.000000 aiodocker-0.9.0/README.rst
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1577 2018-02-11 16:07:55.000000 aiodocker-0.9.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-11 16:10:27.000000 aiodocker-0.9.0/examples/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1888 2018-02-11 16:07:55.000000 aiodocker-0.9.0/examples/events.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1189 2018-02-11 16:07:55.000000 aiodocker-0.9.0/examples/info.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1790 2018-02-11 16:07:55.000000 aiodocker-0.9.0/examples/stdio_stdout.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-11 16:10:27.000000 aiodocker-0.9.0/requirements/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       26 2018-02-11 16:07:55.000000 aiodocker-0.9.0/requirements/base.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       80 2018-02-11 16:07:55.000000 aiodocker-0.9.0/requirements/test.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10177 2018-02-11 16:07:55.000000 aiodocker-0.9.0/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2018-02-11 16:10:27.000000 aiodocker-0.9.0/setup.cfg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-11 16:10:27.000000 aiodocker-0.9.0/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6095 2018-02-11 16:07:55.000000 aiodocker-0.9.0/tests/test_services.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      911 2018-02-11 16:07:55.000000 aiodocker-0.9.0/tests/test_events.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-11 16:10:27.000000 aiodocker-0.9.0/tests/certs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4380 2018-02-11 16:07:55.000000 aiodocker-0.9.0/tests/certs/registry.crt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       71 2018-02-11 16:07:55.000000 aiodocker-0.9.0/tests/certs/htpasswd
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1679 2018-02-11 16:07:55.000000 aiodocker-0.9.0/tests/certs/registry.key
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1738 2018-02-11 16:07:55.000000 aiodocker-0.9.0/tests/test_nodes.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-11 16:10:27.000000 aiodocker-0.9.0/tests/docker/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      220 2018-02-11 16:07:55.000000 aiodocker-0.9.0/tests/docker/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-11 16:10:27.000000 aiodocker-0.9.0/tests/docker/tar/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      189 2018-02-11 16:07:55.000000 aiodocker-0.9.0/tests/docker/tar/app.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       99 2018-02-11 16:07:55.000000 aiodocker-0.9.0/tests/docker/tar/Dockerfile
+-rw-rw-r--   0 travis    (2000) travis    (2000)       76 2018-02-11 16:07:55.000000 aiodocker-0.9.0/tests/docker/Dockerfile
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3584 2018-02-11 16:07:55.000000 aiodocker-0.9.0/tests/docker/docker_context.tar
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2174 2018-02-11 16:07:55.000000 aiodocker-0.9.0/tests/test_containers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2079 2018-02-11 16:07:55.000000 aiodocker-0.9.0/tests/test_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7806 2018-02-11 16:07:55.000000 aiodocker-0.9.0/tests/test_integration.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4572 2018-02-11 16:07:55.000000 aiodocker-0.9.0/tests/test_images.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4060 2018-02-11 16:07:55.000000 aiodocker-0.9.0/tests/conftest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      179 2018-02-11 16:07:55.000000 aiodocker-0.9.0/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4233 2018-02-11 16:10:27.000000 aiodocker-0.9.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      473 2018-02-11 16:07:55.000000 aiodocker-0.9.0/CHANGES.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-11 16:10:27.000000 aiodocker-0.9.0/aiodocker.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       10 2018-02-11 16:10:27.000000 aiodocker-0.9.0/aiodocker.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       26 2018-02-11 16:10:27.000000 aiodocker-0.9.0/aiodocker.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4233 2018-02-11 16:10:27.000000 aiodocker-0.9.0/aiodocker.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2018-02-11 16:10:27.000000 aiodocker-0.9.0/aiodocker.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1056 2018-02-11 16:10:27.000000 aiodocker-0.9.0/aiodocker.egg-info/SOURCES.txt
```

### Comparing `aiodocker-0.8.5/README.rst` & `aiodocker-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `aiodocker-0.8.5/aiodocker/services.py` & `aiodocker-0.9.0/aiodocker/services.py`

 * *Files 12% similar despite different names*

```diff
@@ -83,19 +83,62 @@
         }
 
         data = json.dumps(clean_map(config))
 
         response = await self.docker._query_json(
             "services/create",
             method="POST",
-            headers={"Content-type": "application/json", },
             data=data,
         )
         return response
 
+    async def update(self,
+                     service_id: str,
+                     version: str,
+                     *,
+                     image: str=None,
+                     rollback: bool=False
+                     ) -> bool:
+        """
+        Update a service.
+        If rollback is True image will be ignored.
+
+        Args:
+            service_id: ID or name of the service.
+            version: Version of the service that you want to update.
+            rollback: Rollback the service to the previous service spec.
+
+        Returns:
+            True if successful.
+        """
+        if image is None and rollback is False:
+            raise ValueError("You need to specify an image.")
+
+        inspect_service = await self.inspect(service_id)
+        spec = inspect_service["Spec"]
+
+        if image is not None:
+            spec['TaskTemplate']['ContainerSpec']['Image'] = image
+
+        params = {
+            "version": version,
+        }
+        if rollback is True:
+            params["rollback"] = 'previous'
+
+        data = json.dumps(clean_map(spec))
+
+        await self.docker._query_json(
+            "services/{service_id}/update".format(service_id=service_id),
+            method="POST",
+            data=data,
+            params=params
+        )
+        return True
+
     async def delete(self, service_id: str) -> bool:
         """
         Remove a service
 
         Args:
             service_id: ID or name of the service
```

### Comparing `aiodocker-0.8.5/aiodocker/jsonstream.py` & `aiodocker-0.9.0/aiodocker/jsonstream.py`

 * *Files identical despite different names*

### Comparing `aiodocker-0.8.5/aiodocker/exceptions.py` & `aiodocker-0.9.0/aiodocker/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiodocker-0.8.5/aiodocker/containers.py` & `aiodocker-0.9.0/aiodocker/containers.py`

 * *Files identical despite different names*

### Comparing `aiodocker-0.8.5/aiodocker/channel.py` & `aiodocker-0.9.0/aiodocker/channel.py`

 * *Files identical despite different names*

### Comparing `aiodocker-0.8.5/aiodocker/utils.py` & `aiodocker-0.9.0/aiodocker/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,18 +261,14 @@
     if isinstance(auth, Mapping):
         # Validate the JSON format only.
         if 'identitytoken' in auth:
             pass
         elif 'auth' in auth:
             return compose_auth_header(auth['auth'], registry_addr)
         else:
-            assert 'username' in auth
-            assert 'password' in auth
-            assert 'email' in auth
-            assert 'serveraddress' in auth
             if registry_addr:
                 auth['serveraddress'] = registry_addr
         auth_json = json.dumps(auth).encode('utf-8')
         auth = base64.b64encode(auth_json).decode('ascii')
     elif isinstance(auth, (str, bytes)):
         # Parse simple "username:password"-formatted strings
         # and attach the server address specified.
```

### Comparing `aiodocker-0.8.5/aiodocker/docker.py` & `aiodocker-0.9.0/aiodocker/docker.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,26 +17,28 @@
 from .exceptions import DockerError
 from .images import DockerImages
 from .logs import DockerLog
 from .swarm import DockerSwarm
 from .services import DockerServices
 from .tasks import DockerTasks
 from .volumes import DockerVolumes, DockerVolume
+from .nodes import DockerSwarmNodes
 
 __all__ = (
     'Docker',
     'DockerContainers', 'DockerContainer',
     'DockerEvents',
     'DockerError',
     'DockerImages',
     'DockerLog',
     'DockerSwarm',
     'DockerServices',
     'DockerTasks',
     'DockerVolumes', 'DockerVolume',
+    'DockerSwarmNodes',
 )
 
 log = logging.getLogger(__name__)
 
 _sock_search_paths = [
     Path('/run/docker.sock'),
     Path('/var/run/docker.sock'),
@@ -48,15 +50,15 @@
 
 class Docker:
     def __init__(self,
                  url=None,
                  connector=None,
                  session=None,
                  ssl_context=None,
-                 api_version='v1.26'):
+                 api_version='v1.30'):
 
         docker_host = url  # rename
         if docker_host is None:
             docker_host = os.environ.get('DOCKER_HOST', None)
         if docker_host is None:
             for sockpath in _sock_search_paths:
                 if sockpath.is_socket():
@@ -64,14 +66,20 @@
                     break
         self.docker_host = docker_host
 
         assert _rx_version.search(api_version) is not None, \
             'Invalid API version format'
         self.api_version = api_version
 
+        if docker_host is None:
+            raise ValueError(
+                "Missing valid docker_host."
+                "Either DOCKER_HOST or local sockets are not available."
+                )
+
         if connector is None:
             if _rx_tcp_schemes.search(docker_host):
                 if os.environ.get('DOCKER_TLS_VERIFY', '0') == '1':
                     ssl_context = self._docker_machine_ssl_context()
                     docker_host = _rx_tcp_schemes.sub('https://', docker_host)
                 else:
                     ssl_context = None
@@ -91,14 +99,15 @@
         self.events = DockerEvents(self)
         self.containers = DockerContainers(self)
         self.swarm = DockerSwarm(self)
         self.services = DockerServices(self)
         self.tasks = DockerTasks(self)
         self.images = DockerImages(self)
         self.volumes = DockerVolumes(self)
+        self.nodes = DockerSwarmNodes(self)
 
         # legacy aliases
         self.pull = self.images.pull
         self.push = self.images.push
 
     async def close(self):
         await self.events.stop()
@@ -161,15 +170,15 @@
         headers['content-type'] = 'application/json'
         if not isinstance(data, (str, bytes)):
             data = json.dumps(data)
         response = await self._query(
             path, method,
             params=params, data=data, headers=headers,
             timeout=timeout)
-        data = await parse_result(response, 'json')
+        data = await parse_result(response)
         return data
 
     async def _websocket(self, path, **params):
         if not params:
             params = {
                 'stdin': True,
                 'stdout': True,
```

### Comparing `aiodocker-0.8.5/aiodocker/events.py` & `aiodocker-0.9.0/aiodocker/events.py`

 * *Files identical despite different names*

### Comparing `aiodocker-0.8.5/aiodocker/tasks.py` & `aiodocker-0.9.0/aiodocker/tasks.py`

 * *Files identical despite different names*

### Comparing `aiodocker-0.8.5/aiodocker/swarm.py` & `aiodocker-0.9.0/aiodocker/swarm.py`

 * *Files identical despite different names*

### Comparing `aiodocker-0.8.5/aiodocker/logs.py` & `aiodocker-0.9.0/aiodocker/logs.py`

 * *Files identical despite different names*

### Comparing `aiodocker-0.8.5/aiodocker/multiplexed.py` & `aiodocker-0.9.0/aiodocker/multiplexed.py`

 * *Files identical despite different names*

### Comparing `aiodocker-0.8.5/aiodocker/volumes.py` & `aiodocker-0.9.0/aiodocker/volumes.py`

 * *Files identical despite different names*

### Comparing `aiodocker-0.8.5/aiodocker/images.py` & `aiodocker-0.9.0/aiodocker/images.py`

 * *Files identical despite different names*

### Comparing `aiodocker-0.8.5/LICENSE` & `aiodocker-0.9.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2014-2017 aiodocker Team
+Copyright 2014-2018 aiodocker Team
 
 Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `aiodocker-0.8.5/tests/test_images.py` & `aiodocker-0.9.0/tests/test_images.py`

 * *Files 6% similar despite different names*

```diff
@@ -117,18 +117,15 @@
     name = "alpine:latest"
     await docker.images.pull(from_image=name)
     repository = "localhost:5001/image:latest"
     image, tag = repository.rsplit(':', 1)
     registry_addr, image_name = image.split('/', 1)
     await docker.images.tag(name=name, repo=image, tag=tag)
 
-    auth_config = {'username': "testuser",
-                   'password': "testpassword",
-                   'email': None,
-                   'serveraddress': registry_addr}
+    auth_config = {'username': "testuser", 'password': "testpassword"}
 
     await docker.images.push(name=repository, tag=tag, auth=auth_config)
 
     await docker.images.delete(name=repository)
     await docker.images.pull(repository,
                              auth={"auth": "dGVzdHVzZXI6dGVzdHBhc3N3b3Jk"})
```

### Comparing `aiodocker-0.8.5/tests/test_utils.py` & `aiodocker-0.9.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `aiodocker-0.8.5/tests/test_events.py` & `aiodocker-0.9.0/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `aiodocker-0.8.5/tests/certs/registry.crt` & `aiodocker-0.9.0/tests/certs/registry.crt`

 * *Files identical despite different names*

### Comparing `aiodocker-0.8.5/tests/certs/registry.key` & `aiodocker-0.9.0/tests/certs/registry.key`

 * *Files identical despite different names*

### Comparing `aiodocker-0.8.5/tests/test_containers.py` & `aiodocker-0.9.0/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `aiodocker-0.8.5/tests/test_services.py` & `aiodocker-0.9.0/tests/test_services.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import aiohttp
 import asyncio
 import pytest
-from distutils.version import StrictVersion
 
 
 TaskTemplate = {
     "ContainerSpec": {
         "Image": "redis",
-        },
-    }
+    },
+}
 
 
 async def _wait_service(swarm, service_id):
     for i in range(5):
         tasks = await swarm.tasks.list(filters={'service': service_id})
         if tasks:
             return
@@ -35,38 +34,42 @@
     name = docker_service['Spec']['Name']
     filters = {"name": name}
     filtered_list = await swarm.services.list(filters=filters)
     assert len(filtered_list) == 1
 
 
 @pytest.mark.asyncio
-async def test_service_tasks(swarm, tmp_service):
-    assert await swarm.tasks.list()
+async def test_service_tasks_list(swarm, tmp_service):
+    tasks = await swarm.tasks.list()
+    assert len(tasks) == 1
+    assert tasks[0]['ServiceID'] == tmp_service
+    assert await swarm.tasks.inspect(tasks[0]['ID'])
+
+
+@pytest.mark.asyncio
+async def test_service_tasks_list_with_filters(swarm, tmp_service):
     tasks = await swarm.tasks.list(filters={'service': tmp_service})
     assert len(tasks) == 1
     assert tasks[0]['ServiceID'] == tmp_service
     assert await swarm.tasks.inspect(tasks[0]['ID'])
 
 
 @pytest.mark.asyncio
 async def test_logs_services(swarm):
-    if StrictVersion(swarm.api_version[1:]) < StrictVersion("1.29"):
-        pytest.skip("The feature is experimental before API version 1.29")
-
     TaskTemplate = {
         "ContainerSpec": {
             "Image": "python:3.6.1-alpine",
             "Args": [
                 "python", "-c",
                 "for _ in range(10): print('Hello Python')"
-                ]
+            ]
         },
         "RestartPolicy": {
             "Condition": "none"
-            }
+        }
     }
     service = await swarm.services.create(
         task_template=TaskTemplate,
     )
     service_id = service['ID']
 
     filters = {"service": service_id}
@@ -78,36 +81,33 @@
             task = await swarm.tasks.list(filters=filters)
             if task:
                 status = task[0]['Status']['State']
                 if status == 'complete':
                     break
 
     logs = await swarm.services.logs(
-                            service_id, stdout=True)
+        service_id, stdout=True)
 
     assert len(logs) == 10
     assert logs[0] == "Hello Python"
 
 
 @pytest.mark.asyncio
 async def test_logs_services_stream(swarm):
-    if StrictVersion(swarm.api_version[1:]) < StrictVersion("1.29"):
-        pytest.skip("The feature is experimental before API version 1.29")
-
     TaskTemplate = {
         "ContainerSpec": {
             "Image": "python:3.6.1-alpine",
             "Args": [
                 "python", "-c",
                 "for _ in range(10): print('Hello Python')"
-                ]
+            ]
         },
         "RestartPolicy": {
             "Condition": "none"
-            }
+        }
     }
     service = await swarm.services.create(
         task_template=TaskTemplate,
     )
     service_id = service['ID']
 
     filters = {"service": service_id}
@@ -119,23 +119,102 @@
             task = await swarm.tasks.list(filters=filters)
             if task:
                 status = task[0]['Status']['State']
                 if status == 'complete':
                     break
 
     stream = await swarm.services.logs(
-                            service_id, stdout=True, follow=True
-                            )
+        service_id, stdout=True, follow=True
+    )
 
     # the service printed 10 `Hello Python`
     # let's check for them
     count = 0
     try:
         with aiohttp.Timeout(2):
             while True:
                 async for log in stream:
                     if "Hello Python\n" in log:
                         count += 1
     except asyncio.TimeoutError:
         pass
 
     assert count == 10
+
+
+@pytest.mark.asyncio
+async def test_service_update(swarm):
+    name = "service-update"
+    initial_image = "redis:3.0.2"
+    image_after_update = "redis:4.0"
+    TaskTemplate = {
+        "ContainerSpec": {
+            "Image": initial_image,
+        },
+    }
+
+    await swarm.services.create(
+        name=name,
+        task_template=TaskTemplate,
+    )
+    service = await swarm.services.inspect(name)
+    current_image = service["Spec"]["TaskTemplate"]["ContainerSpec"]["Image"]
+    version = service['Version']['Index']
+    assert initial_image in current_image
+
+    # update the service
+    await swarm.services.update(
+        service_id=name, version=version, image=image_after_update
+    )
+    # wait a few to complete the update of the service
+    await asyncio.sleep(1)
+
+    service = await swarm.services.inspect(name)
+    current_image = service["Spec"]["TaskTemplate"]["ContainerSpec"]["Image"]
+    version = service['Version']['Index']
+    assert image_after_update in current_image
+
+    # rollback to the previous one
+    await swarm.services.update(
+        service_id=name, version=version, rollback=True
+    )
+    service = await swarm.services.inspect(name)
+    current_image = service["Spec"]["TaskTemplate"]["ContainerSpec"]["Image"]
+    assert initial_image in current_image
+
+    await swarm.services.delete(name)
+
+
+@pytest.mark.asyncio
+async def test_service_update_error(swarm):
+    name = "service-update"
+    TaskTemplate = {
+        "ContainerSpec": {
+            "Image": "redis:3.0.2",
+        },
+    }
+    await swarm.services.create(
+        name=name,
+        task_template=TaskTemplate,
+    )
+    await asyncio.sleep(1)
+    service = await swarm.services.inspect(name)
+    version = service['Version']['Index']
+
+    with pytest.raises(ValueError):
+        await swarm.services.update(service_id=name, version=version)
+
+    await swarm.services.delete(name)
+
+
+@pytest.mark.asyncio
+async def test_service_create_error(swarm):
+    name = "service-test-error"
+    TaskTemplate = {
+        "ContainerSpec": {
+        },
+    }
+    with pytest.raises(KeyError):
+        await swarm.services.create(
+            name=name,
+            task_template=TaskTemplate,
+        )
```

### Comparing `aiodocker-0.8.5/tests/docker/docker_context.tar` & `aiodocker-0.9.0/tests/docker/docker_context.tar`

 * *Files identical despite different names*

### Comparing `aiodocker-0.8.5/tests/conftest.py` & `aiodocker-0.9.0/tests/conftest.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,17 +8,14 @@
 
 from aiodocker.docker import Docker
 from aiodocker.exceptions import DockerError
 
 
 _api_versions = {
     "17.06": "v1.30",
-    "17.05": "v1.29",
-    "17.04": "v1.28",
-    "17.03": "v1.27",
 }
 
 
 def _random_name():
     return "aiodocker-" + uuid.uuid4().hex[:7]
 
 
@@ -54,15 +51,19 @@
 def testing_images():
     # Prepare a small Linux image shared by most test cases.
     event_loop = asyncio.get_event_loop()
 
     async def _pull():
         docker = Docker()
         required_images = [
-            'alpine:latest', 'redis:latest', 'python:3.6.1-alpine',
+            'alpine:latest',
+            'redis:latest',
+            'redis:3.0.2',
+            'redis:4.0',
+            'python:3.6.1-alpine',
         ]
         for img in required_images:
             try:
                 await docker.images.get(img)
             except DockerError as e:
                 assert e.status == 404
                 print('Pulling "{img}" for the testing session...'
@@ -94,29 +95,17 @@
             pytest.skip(reason)
 
     yield check
 
 
 @pytest.fixture
 def swarm(event_loop, docker):
-    if StrictVersion(docker.api_version[1:]) < StrictVersion("1.28"):
-        pytest.skip("The feature is experimental before API version 1.28")
     assert event_loop.run_until_complete(docker.swarm.init())
     yield docker
-    try:
-        assert event_loop.run_until_complete(docker.swarm.leave(force=True))
-    except DockerError as exc:
-        if StrictVersion(docker.api_version[1:]) >= StrictVersion("1.30"):
-            raise
-        else:
-            # NOTE: in Docker version 1.28 and 1.29, it is possible that Docker
-            #       refuses to leave the Swarm cleanly. Reducing the number
-            #       of service ran seems to solve the issue. More at #53
-            assert event_loop.run_until_complete(
-                docker.swarm.leave(force=True))
+    assert event_loop.run_until_complete(docker.swarm.leave(force=True))
 
 
 @pytest.fixture
 def shell_container(event_loop, docker):
     container = None
     config = {
         "Cmd": ["/bin/ash"],
```

### Comparing `aiodocker-0.8.5/tests/test_integration.py` & `aiodocker-0.9.0/tests/test_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import asyncio
 import datetime
 import io
 import os
 import sys
 import tarfile
 import time
-from distutils.version import StrictVersion
 
 import aiohttp
 import pytest
 
 from aiodocker.docker import Docker
 
 
@@ -101,17 +100,14 @@
     assert len(containers) == orig_count
 
 
 @pytest.mark.asyncio
 @pytest.mark.skipif(sys.platform == 'darwin',
                     reason="Docker for Mac has a bug with websocket")
 async def test_stdio_stdin(docker, testing_images, shell_container):
-    if StrictVersion(docker.api_version[1:]) < StrictVersion("1.28"):
-        pytest.skip("The WebSocket return text before API version 1.28")
-
     # echo of the input.
     ws = await shell_container.websocket(stdin=True, stdout=True, stream=True)
     await ws.send_str('echo hello world\n')
     output = b''
     found = False
     try:
         # collect the websocket outputs for at most 2 secs until we see the
```

### Comparing `aiodocker-0.8.5/setup.py` & `aiodocker-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `aiodocker-0.8.5/aiodocker.egg-info/SOURCES.txt` & `aiodocker-0.9.0/aiodocker.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 aiodocker/docker.py
 aiodocker/events.py
 aiodocker/exceptions.py
 aiodocker/images.py
 aiodocker/jsonstream.py
 aiodocker/logs.py
 aiodocker/multiplexed.py
+aiodocker/nodes.py
 aiodocker/services.py
 aiodocker/swarm.py
 aiodocker/tasks.py
 aiodocker/utils.py
 aiodocker/volumes.py
 aiodocker.egg-info/PKG-INFO
 aiodocker.egg-info/SOURCES.txt
@@ -30,14 +31,15 @@
 requirements/base.txt
 requirements/test.txt
 tests/conftest.py
 tests/test_containers.py
 tests/test_events.py
 tests/test_images.py
 tests/test_integration.py
+tests/test_nodes.py
 tests/test_services.py
 tests/test_utils.py
 tests/certs/htpasswd
 tests/certs/registry.crt
 tests/certs/registry.key
 tests/docker/Dockerfile
 tests/docker/README.md
```

### Comparing `aiodocker-0.8.5/aiodocker.egg-info/PKG-INFO` & `aiodocker-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: aiodocker
-Version: 0.8.5
+Version: 0.9.0
 Summary: Docker API client for asyncio
 Home-page: https://github.com/aio-libs/aiodocker
 Author: Paul Tagliamonte
 Author-email: paultag@debian.org
 License: Apache 2
 Description-Content-Type: UNKNOWN
 Description: ==============================
```

### Comparing `aiodocker-0.8.5/PKG-INFO` & `aiodocker-0.9.0/aiodocker.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: aiodocker
-Version: 0.8.5
+Version: 0.9.0
 Summary: Docker API client for asyncio
 Home-page: https://github.com/aio-libs/aiodocker
 Author: Paul Tagliamonte
 Author-email: paultag@debian.org
 License: Apache 2
 Description-Content-Type: UNKNOWN
 Description: ==============================
```

### Comparing `aiodocker-0.8.5/examples/info.py` & `aiodocker-0.9.0/examples/info.py`

 * *Files identical despite different names*

### Comparing `aiodocker-0.8.5/examples/events.py` & `aiodocker-0.9.0/examples/events.py`

 * *Files identical despite different names*

### Comparing `aiodocker-0.8.5/examples/stdio_stdout.py` & `aiodocker-0.9.0/examples/stdio_stdout.py`

 * *Files identical despite different names*

