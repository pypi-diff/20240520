# Comparing `tmp/my_scrcpy-0.1.tar.gz` & `tmp/my_scrcpy-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_scrcpy-0.1.tar", last modified: Mon May 20 14:31:02 2024, max compression
+gzip compressed data, was "my_scrcpy-0.2.tar", last modified: Mon May 20 14:46:04 2024, max compression
```

## Comparing `my_scrcpy-0.1.tar` & `my_scrcpy-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 14:31:02.763106 my_scrcpy-0.1/
--rw-rw-rw-   0        0        0      363 2024-05-20 14:31:02.762116 my_scrcpy-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-20 14:31:02.761543 my_scrcpy-0.1/my_scrcpy.egg-info/
--rw-rw-rw-   0        0        0      363 2024-05-20 14:31:02.000000 my_scrcpy-0.1/my_scrcpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2024-05-20 14:31:02.000000 my_scrcpy-0.1/my_scrcpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 14:31:02.000000 my_scrcpy-0.1/my_scrcpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-20 14:31:02.000000 my_scrcpy-0.1/my_scrcpy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-20 14:31:02.760546 my_scrcpy-0.1/scrcpy/
--rw-rw-rw-   0        0        0       90 2023-08-17 05:07:04.000000 my_scrcpy-0.1/scrcpy/__init__.py
--rw-rw-rw-   0        0        0     7478 2023-08-17 05:07:04.000000 my_scrcpy-0.1/scrcpy/const.py
--rw-rw-rw-   0        0        0     6935 2023-08-17 05:07:04.000000 my_scrcpy-0.1/scrcpy/control.py
--rw-rw-rw-   0        0        0    10229 2023-08-17 05:07:04.000000 my_scrcpy-0.1/scrcpy/core.py
--rw-rw-rw-   0        0        0       42 2024-05-20 14:31:02.763106 my_scrcpy-0.1/setup.cfg
--rw-rw-rw-   0        0        0      588 2024-05-20 14:30:38.000000 my_scrcpy-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:46:04.518215 my_scrcpy-0.2/
+-rw-rw-rw-   0        0        0      363 2024-05-20 14:46:04.517217 my_scrcpy-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-20 14:46:04.517217 my_scrcpy-0.2/my_scrcpy.egg-info/
+-rw-rw-rw-   0        0        0      363 2024-05-20 14:46:04.000000 my_scrcpy-0.2/my_scrcpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2024-05-20 14:46:04.000000 my_scrcpy-0.2/my_scrcpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 14:46:04.000000 my_scrcpy-0.2/my_scrcpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-20 14:46:04.000000 my_scrcpy-0.2/my_scrcpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-20 14:46:04.517217 my_scrcpy-0.2/scrcpy/
+-rw-rw-rw-   0        0        0       90 2023-08-17 05:07:04.000000 my_scrcpy-0.2/scrcpy/__init__.py
+-rw-rw-rw-   0        0        0     7478 2023-08-17 05:07:04.000000 my_scrcpy-0.2/scrcpy/const.py
+-rw-rw-rw-   0        0        0     6935 2023-08-17 05:07:04.000000 my_scrcpy-0.2/scrcpy/control.py
+-rw-rw-rw-   0        0        0    10191 2024-05-20 14:45:46.000000 my_scrcpy-0.2/scrcpy/core.py
+-rw-rw-rw-   0        0        0       42 2024-05-20 14:46:04.518215 my_scrcpy-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      588 2024-05-20 14:46:02.000000 my_scrcpy-0.2/setup.py
```

### Comparing `my_scrcpy-0.1/scrcpy/const.py` & `my_scrcpy-0.2/scrcpy/const.py`

 * *Files identical despite different names*

### Comparing `my_scrcpy-0.1/scrcpy/control.py` & `my_scrcpy-0.2/scrcpy/control.py`

 * *Files identical despite different names*

### Comparing `my_scrcpy-0.1/scrcpy/core.py` & `my_scrcpy-0.2/scrcpy/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -132,22 +132,20 @@
         if not len(self.device_name):
             raise ConnectionError("Did not receive Device Name!")
 
         res = self.__video_socket.recv(4)
         self.resolution = struct.unpack(">HH", res)
         self.__video_socket.setblocking(False)
 
-    def __deploy_server(self) -> None:
+    def __deploy_server(self, file_path) -> None:
         """
         Deploy server to android device
         """
         jar_name = "scrcpy-server.jar"
-        server_file_path = os.path.join(
-            os.path.abspath(os.path.dirname(__file__)), jar_name
-        )
+        server_file_path = file_path
         self.device.sync.push(server_file_path, f"/data/local/tmp/{jar_name}")
         commands = [
             f"CLASSPATH=/data/local/tmp/{jar_name}",
             "app_process",
             "/",
             "com.genymobile.scrcpy.Server",
             "1.20",  # Scrcpy server version
@@ -172,25 +170,25 @@
             commands,
             stream=True,
         )
 
         # Wait for server to start
         self.__server_stream.read(10)
 
-    def start(self, threaded: bool = False, daemon_threaded: bool = False) -> None:
+    def start(self, threaded: bool = False, daemon_threaded: bool = False, file_path: str = "") -> None:
         """
         Start listening video stream
 
         Args:
             threaded: Run stream loop in a different thread to avoid blocking
             daemon_threaded: Run stream loop in a daemon thread to avoid blocking
         """
         assert self.alive is False
 
-        self.__deploy_server()
+        self.__deploy_server(file_path)
         self.__init_server_connection()
         self.alive = True
         self.__send_to_listeners(EVENT_INIT)
 
         if threaded or daemon_threaded:
             self.stream_loop_thread = threading.Thread(
                 target=self.__stream_loop, daemon=daemon_threaded
```

### Comparing `my_scrcpy-0.1/setup.py` & `my_scrcpy-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='my_scrcpy',
-    version='0.1',
+    version='0.2',
     packages=find_packages(),
     install_requires=[],  # Các package phụ thuộc nếu có
     description='Screen copy android',
     author='NamHV4',
     author_email='namhoang2110@gmail.com',
     url='https://github.com/NamHV4/scrcpy_namhv4',  # URL đến repo của bạn
     classifiers=[
```

