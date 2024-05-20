# Comparing `tmp/lambkid-0.2.3.tar.gz` & `tmp/lambkid-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lambkid-0.2.3.tar", last modified: Fri May 17 02:19:59 2024, max compression
+gzip compressed data, was "lambkid-0.2.4.tar", last modified: Mon May 20 03:27:04 2024, max compression
```

## Comparing `lambkid-0.2.3.tar` & `lambkid-0.2.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 02:19:59.342147 lambkid-0.2.3/
--rw-rw-rw-   0        0        0     1089 2024-03-27 01:13:02.000000 lambkid-0.2.3/LICENSE
--rw-rw-rw-   0        0        0       27 2024-04-01 08:22:25.000000 lambkid-0.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2094 2024-05-17 02:19:59.340153 lambkid-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0      717 2024-04-24 02:44:24.000000 lambkid-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 02:19:59.284302 lambkid-0.2.3/docs/
--rw-rw-rw-   0        0        0      371 2024-04-08 03:30:43.000000 lambkid-0.2.3/docs/cli.md
--rw-rw-rw-   0        0        0      221 2024-04-24 02:42:57.000000 lambkid-0.2.3/docs/csv.md
--rw-rw-rw-   0        0        0       54 2024-03-31 06:58:42.000000 lambkid-0.2.3/docs/install.md
--rw-rw-rw-   0        0        0      778 2024-04-07 15:20:10.000000 lambkid-0.2.3/docs/log.md
--rw-rw-rw-   0        0        0     1878 2024-04-01 07:39:19.000000 lambkid-0.2.3/docs/sshclient.md
--rw-rw-rw-   0        0        0       36 2024-04-25 02:05:46.000000 lambkid-0.2.3/docs/utils.md
-drwxrwxrwx   0        0        0        0 2024-05-17 02:19:59.286297 lambkid-0.2.3/lambkid/
--rw-rw-rw-   0        0        0      188 2024-04-25 02:53:27.000000 lambkid-0.2.3/lambkid/__init__.py
--rw-rw-rw-   0        0        0      969 2024-04-08 15:55:58.000000 lambkid-0.2.3/lambkid/cli.py
-drwxrwxrwx   0        0        0        0 2024-05-17 02:19:59.337160 lambkid-0.2.3/lambkid/libs/
--rw-rw-rw-   0        0        0        0 2024-03-31 06:59:08.000000 lambkid-0.2.3/lambkid/libs/__init__.py
--rw-rw-rw-   0        0        0     1514 2024-04-29 07:44:19.000000 lambkid-0.2.3/lambkid/libs/log.py
--rw-rw-rw-   0        0        0     1825 2024-05-17 02:16:37.000000 lambkid-0.2.3/lambkid/libs/minio_client.py
--rw-rw-rw-   0        0        0     7346 2024-05-15 08:32:56.000000 lambkid-0.2.3/lambkid/libs/ssh.py
--rw-rw-rw-   0        0        0     2259 2024-04-28 05:47:19.000000 lambkid-0.2.3/lambkid/libs/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-17 02:19:59.339156 lambkid-0.2.3/lambkid.egg-info/
--rw-rw-rw-   0        0        0     2094 2024-05-17 02:19:59.000000 lambkid-0.2.3/lambkid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      461 2024-05-17 02:19:59.000000 lambkid-0.2.3/lambkid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 02:19:59.000000 lambkid-0.2.3/lambkid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-05-17 02:19:59.000000 lambkid-0.2.3/lambkid.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       43 2024-05-17 02:19:59.000000 lambkid-0.2.3/lambkid.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-17 02:19:59.000000 lambkid-0.2.3/lambkid.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-17 02:19:59.343144 lambkid-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1834 2024-05-17 02:16:46.000000 lambkid-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 03:27:04.881443 lambkid-0.2.4/
+-rw-rw-rw-   0        0        0     1089 2024-03-27 01:13:02.000000 lambkid-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0       27 2024-04-01 08:22:25.000000 lambkid-0.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2094 2024-05-20 03:27:04.880446 lambkid-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0      717 2024-04-24 02:44:24.000000 lambkid-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 03:27:04.780713 lambkid-0.2.4/docs/
+-rw-rw-rw-   0        0        0      371 2024-04-08 03:30:43.000000 lambkid-0.2.4/docs/cli.md
+-rw-rw-rw-   0        0        0      221 2024-04-24 02:42:57.000000 lambkid-0.2.4/docs/csv.md
+-rw-rw-rw-   0        0        0       54 2024-03-31 06:58:42.000000 lambkid-0.2.4/docs/install.md
+-rw-rw-rw-   0        0        0      778 2024-04-07 15:20:10.000000 lambkid-0.2.4/docs/log.md
+-rw-rw-rw-   0        0        0     1878 2024-04-01 07:39:19.000000 lambkid-0.2.4/docs/sshclient.md
+-rw-rw-rw-   0        0        0       36 2024-04-25 02:05:46.000000 lambkid-0.2.4/docs/utils.md
+drwxrwxrwx   0        0        0        0 2024-05-20 03:27:04.783706 lambkid-0.2.4/lambkid/
+-rw-rw-rw-   0        0        0      188 2024-04-25 02:53:27.000000 lambkid-0.2.4/lambkid/__init__.py
+-rw-rw-rw-   0        0        0      969 2024-04-08 15:55:58.000000 lambkid-0.2.4/lambkid/cli.py
+drwxrwxrwx   0        0        0        0 2024-05-20 03:27:04.875460 lambkid-0.2.4/lambkid/libs/
+-rw-rw-rw-   0        0        0        0 2024-03-31 06:59:08.000000 lambkid-0.2.4/lambkid/libs/__init__.py
+-rw-rw-rw-   0        0        0     1514 2024-04-29 07:44:19.000000 lambkid-0.2.4/lambkid/libs/log.py
+-rw-rw-rw-   0        0        0     1825 2024-05-17 02:16:37.000000 lambkid-0.2.4/lambkid/libs/minio_client.py
+-rw-rw-rw-   0        0        0     9707 2024-05-20 03:26:20.000000 lambkid-0.2.4/lambkid/libs/ssh.py
+-rw-rw-rw-   0        0        0     2259 2024-04-28 05:47:19.000000 lambkid-0.2.4/lambkid/libs/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-20 03:27:04.879449 lambkid-0.2.4/lambkid.egg-info/
+-rw-rw-rw-   0        0        0     2094 2024-05-20 03:27:04.000000 lambkid-0.2.4/lambkid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      461 2024-05-20 03:27:04.000000 lambkid-0.2.4/lambkid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 03:27:04.000000 lambkid-0.2.4/lambkid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-20 03:27:04.000000 lambkid-0.2.4/lambkid.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       43 2024-05-20 03:27:04.000000 lambkid-0.2.4/lambkid.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-20 03:27:04.000000 lambkid-0.2.4/lambkid.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 03:27:04.881443 lambkid-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1834 2024-05-20 03:26:35.000000 lambkid-0.2.4/setup.py
```

### Comparing `lambkid-0.2.3/LICENSE` & `lambkid-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lambkid-0.2.3/PKG-INFO` & `lambkid-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambkid
-Version: 0.2.3
+Version: 0.2.4
 Summary: lambkid is an advance abstract from some common pyton lib, it aim to make you write python more easily and more fewer code.
 Home-page: https://github.com/redrose2100/lambkid
 Author: redrose2100
 Author-email: hitredrose@163.com
 Maintainer: redrose2100
 Maintainer-email: hitredrose@163.com
 License: MIT
```

### Comparing `lambkid-0.2.3/README.md` & `lambkid-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `lambkid-0.2.3/docs/log.md` & `lambkid-0.2.4/docs/log.md`

 * *Files identical despite different names*

### Comparing `lambkid-0.2.3/docs/sshclient.md` & `lambkid-0.2.4/docs/sshclient.md`

 * *Files identical despite different names*

### Comparing `lambkid-0.2.3/lambkid/cli.py` & `lambkid-0.2.4/lambkid/cli.py`

 * *Files identical despite different names*

### Comparing `lambkid-0.2.3/lambkid/libs/log.py` & `lambkid-0.2.4/lambkid/libs/log.py`

 * *Files identical despite different names*

### Comparing `lambkid-0.2.3/lambkid/libs/minio_client.py` & `lambkid-0.2.4/lambkid/libs/minio_client.py`

 * *Files identical despite different names*

### Comparing `lambkid-0.2.3/lambkid/libs/ssh.py` & `lambkid-0.2.4/lambkid/libs/ssh.py`

 * *Files 18% similar despite different names*

```diff
@@ -141,14 +141,54 @@
             log.info(
                 f" {self.__ip}:{self.__port} | Success to copy file from local {local_path} to remote host{remote_path}: OK.")
         except Exception as e:
             log.error(
                 f"{self.__ip}:{self.__port} | Failed to copy file from local {local_path} to remote host {remote_path}: Error. err msg is:{str(e)}")
             raise e
 
+    def scp_file_to_remote(self, local_path, remote_path):
+        log.info(
+            f" {self.__ip}:{self.__port} | Begin to copy file from local {local_path} to remote host {remote_path} ...")
+        try:
+            if not self.__is_active():
+                self.__reconnect()
+            if not self.__sftp or not self.__scp:
+                self.__scp = paramiko.Transport((self.__ip, self.__port))
+                self.__scp.connect(username=self.__username, password=self.__password)
+                self.__sftp = paramiko.SFTPClient.from_transport(self.__scp)
+            if os.path.isfile(local_path):
+                self.__sftp.put(local_path, remote_path)
+            else:
+                log.error(f" {self.__ip}:{self.__port} | failed to copy file from local {local_path} to remote host{remote_path}: Error. for local file is not exist.")
+            log.info(
+                f" {self.__ip}:{self.__port} | Success to copy file from local {local_path} to remote host{remote_path}: OK.")
+        except Exception as e:
+            log.error(
+                f"{self.__ip}:{self.__port} | Failed to copy file from local {local_path} to remote host {remote_path}: Error. err msg is:{str(e)}")
+            raise e
+    def scp_file_to_local(self, remote_path, local_path):
+        log.info(
+            f" {self.__ip}:{self.__port} | Begin to copy file from remote {remote_path} to local host {local_path} ...")
+        try:
+            if not self.__is_active():
+                self.__reconnect()
+            if not self.__sftp or not self.__scp:
+                self.__scp = paramiko.Transport((self.__ip, self.__port))
+                self.__scp.connect(username=self.__username, password=self.__password)
+                self.__sftp = paramiko.SFTPClient.from_transport(self.__scp)
+            if os.path.isfile(local_path):
+                os.system(f"rm -rf {local_path}")
+            self.__sftp.get(remote_path,local_path)
+            log.info(
+                f" {self.__ip}:{self.__port} | Success to copy file from remote {remote_path} to local host{local_path}: OK.")
+        except Exception as e:
+            log.error(
+                f"{self.__ip}:{self.__port} | Failed to copy file from remote {remote_path} to local host {local_path}: Error. err msg is:{str(e)}")
+            raise e
+
     def __connect(self):
         log.info(f" {self.__ip}:{self.__port} | begin to create ssh connect...")
         try:
             self.__ssh = paramiko.SSHClient()
             self.__ssh.set_missing_host_key_policy(paramiko.AutoAddPolicy())
             self.__ssh.connect(hostname=self.__ip, port=self.__port, username=self.__username, password=self.__password,
                                timeout=self.__connect_timeout)
```

### Comparing `lambkid-0.2.3/lambkid/libs/utils.py` & `lambkid-0.2.4/lambkid/libs/utils.py`

 * *Files identical despite different names*

### Comparing `lambkid-0.2.3/lambkid.egg-info/PKG-INFO` & `lambkid-0.2.4/lambkid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambkid
-Version: 0.2.3
+Version: 0.2.4
 Summary: lambkid is an advance abstract from some common pyton lib, it aim to make you write python more easily and more fewer code.
 Home-page: https://github.com/redrose2100/lambkid
 Author: redrose2100
 Author-email: hitredrose@163.com
 Maintainer: redrose2100
 Maintainer-email: hitredrose@163.com
 License: MIT
```

### Comparing `lambkid-0.2.3/setup.py` & `lambkid-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         long_desc=f.read()
 except:
     long_desc=""
 
 
 setup(
     name="lambkid",
-    version="0.2.3",
+    version="0.2.4",
     description="lambkid is an advance abstract from some common pyton lib, it aim to make you write python more easily and more fewer code.",
     long_description=long_desc,
     long_description_content_type="text/markdown",
     author="redrose2100",
     author_email="hitredrose@163.com",
     maintainer="redrose2100",
     maintainer_email="hitredrose@163.com",
```

