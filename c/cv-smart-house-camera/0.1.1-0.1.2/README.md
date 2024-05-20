# Comparing `tmp/cv_smart_house_camera-0.1.1.tar.gz` & `tmp/cv_smart_house_camera-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cv_smart_house_camera-0.1.1.tar", max compression
+gzip compressed data, was "cv_smart_house_camera-0.1.2.tar", max compression
```

## Comparing `cv_smart_house_camera-0.1.1.tar` & `cv_smart_house_camera-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     3991 2024-05-20 12:10:20.119846 cv_smart_house_camera-0.1.1/cv_smart_house_camera/__init__.py
--rw-r--r--   0        0        0      795 2024-05-20 12:12:45.499792 cv_smart_house_camera-0.1.1/cv_smart_house_camera/cam_capture.py
--rw-r--r--   0        0        0       48 2024-05-20 12:13:33.324485 cv_smart_house_camera-0.1.1/cv_smart_house_camera/constants.py
--rw-r--r--   0        0        0       85 2024-05-18 16:24:24.102931 cv_smart_house_camera-0.1.1/cv_smart_house_camera/data/frames.py
--rw-r--r--   0        0        0     1102 2024-05-20 12:10:21.242333 cv_smart_house_camera-0.1.1/cv_smart_house_camera/generate_code.py
--rw-r--r--   0        0        0      292 2024-05-20 12:05:00.597313 cv_smart_house_camera-0.1.1/cv_smart_house_camera/helpers/poetry_install.py
--rw-r--r--   0        0        0      761 2024-05-20 11:44:37.606982 cv_smart_house_camera-0.1.1/cv_smart_house_camera/modules/modules_list.py
--rw-r--r--   0        0        0     1772 2024-05-20 12:12:30.001708 cv_smart_house_camera-0.1.1/cv_smart_house_camera/modules/modules_processing.py
--rw-r--r--   0        0        0     3501 2024-05-20 11:57:48.195278 cv_smart_house_camera-0.1.1/cv_smart_house_camera/proto_services/camera_service_pb2.py
--rw-r--r--   0        0        0     5512 2024-05-20 11:57:48.195278 cv_smart_house_camera-0.1.1/cv_smart_house_camera/proto_services/camera_service_twirp.py
--rw-r--r--   0        0        0      141 2024-05-19 14:26:26.476002 cv_smart_house_camera-0.1.1/cv_smart_house_camera/utils/get_local_ip.py
--rw-r--r--   0        0        0      508 2024-05-19 13:22:30.480493 cv_smart_house_camera-0.1.1/cv_smart_house_camera/utils/get_modules_from_toml.py
--rw-r--r--   0        0        0      680 2024-05-20 12:14:27.187421 cv_smart_house_camera-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-05 13:48:56.985064 cv_smart_house_camera-0.1.1/README.md
--rw-r--r--   0        0        0      823 1970-01-01 00:00:00.000000 cv_smart_house_camera-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     4155 2024-05-20 17:14:19.319636 cv_smart_house_camera-0.1.2/cv_smart_house_camera/__init__.py
+-rw-r--r--   0        0        0      733 2024-05-20 13:14:13.260707 cv_smart_house_camera-0.1.2/cv_smart_house_camera/cam_capture.py
+-rw-r--r--   0        0        0       48 2024-05-20 12:13:33.324485 cv_smart_house_camera-0.1.2/cv_smart_house_camera/constants.py
+-rw-r--r--   0        0        0       85 2024-05-18 16:24:24.102931 cv_smart_house_camera-0.1.2/cv_smart_house_camera/data/frames.py
+-rw-r--r--   0        0        0     1102 2024-05-20 12:10:21.242333 cv_smart_house_camera-0.1.2/cv_smart_house_camera/generate_code.py
+-rw-r--r--   0        0        0      292 2024-05-20 12:05:00.597313 cv_smart_house_camera-0.1.2/cv_smart_house_camera/helpers/poetry_install.py
+-rw-r--r--   0        0        0      522 2024-05-20 17:15:58.713259 cv_smart_house_camera-0.1.2/cv_smart_house_camera/modules/modules_list.py
+-rw-r--r--   0        0        0     1772 2024-05-20 12:12:30.001708 cv_smart_house_camera-0.1.2/cv_smart_house_camera/modules/modules_processing.py
+-rw-r--r--   0        0        0     3501 2024-05-20 11:57:48.195278 cv_smart_house_camera-0.1.2/cv_smart_house_camera/proto_services/camera_service_pb2.py
+-rw-r--r--   0        0        0     5512 2024-05-20 11:57:48.195278 cv_smart_house_camera-0.1.2/cv_smart_house_camera/proto_services/camera_service_twirp.py
+-rw-r--r--   0        0        0      141 2024-05-19 14:26:26.476002 cv_smart_house_camera-0.1.2/cv_smart_house_camera/utils/get_local_ip.py
+-rw-r--r--   0        0        0      515 2024-05-20 12:20:23.424894 cv_smart_house_camera-0.1.2/cv_smart_house_camera/utils/get_modules_from_toml.py
+-rw-r--r--   0        0        0      683 2024-05-20 17:14:55.015162 cv_smart_house_camera-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-05 13:48:56.985064 cv_smart_house_camera-0.1.2/README.md
+-rw-r--r--   0        0        0      787 1970-01-01 00:00:00.000000 cv_smart_house_camera-0.1.2/PKG-INFO
```

### Comparing `cv_smart_house_camera-0.1.1/cv_smart_house_camera/__init__.py` & `cv_smart_house_camera-0.1.2/cv_smart_house_camera/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import uvicorn
 from threading import Thread
 from cv_smart_house_camera.cam_capture import cam_capture
 from twirp.asgi import TwirpASGIApp
 from  cv_smart_house_camera.proto_services.camera_service_twirp import CameraServiceServer
 import  cv_smart_house_camera.proto_services.camera_service_pb2 as camera_service
 from cv_smart_house_camera.data.frames import modules_result
-from cv_smart_house_camera.modules.modules_list import modules
+from cv_smart_house_camera.modules.modules_list import modules as modules_list
 from starlette.middleware.cors import CORSMiddleware
 
 from cv_smart_house_camera.helpers.poetry_install import poetry_install
 from cv_smart_house_camera.generate_code import generate_code
 from google.protobuf.empty_pb2 import Empty
 from cv_smart_house_camera.constants import PORT
 from cv_smart_house_camera.utils.get_local_ip import get_local_ip
@@ -38,15 +38,15 @@
     
     def UninstallModules(self, ctx, request):
         # Remove packages from array from the project.
         original_names = []
 
         #find original_name of the package
         for module in request.modules:
-            for installed_module in modules:
+            for installed_module in modules_list:
                 if installed_module.get("name") == module:
                     original_names.append(installed_module.get("package_name"))
 
         with open('pyproject.toml', 'r') as file:
             pyproject_data = toml.load(file)
 
         for package in original_names:
@@ -58,15 +58,15 @@
         generate_code()
 
         return Empty()
     
     def GetInstalledModules(self, ctx, request):
         formatted_modules = []
 
-        for module in modules:
+        for module in modules_list:
             formatted_modules.append(camera_service.InstalledModule(name = module.get("name"), options = module.get("options")))
 
         return camera_service.InstalledModules(modules=formatted_modules)
 
     def GetLastFrame(self, ctx, request):
         module_result = modules_result.get(request.module)
         if module_result is None or module_result.get("ok") == False:
@@ -88,22 +88,27 @@
     allow_headers=["*"],
 )
 
 def run_server():
     uvicorn.run(app=app, host=get_local_ip(), port=PORT)
 
 def configure_camera_server(services: list = [], 
-                            allow_origins=["*"],
-                            allow_methods=["*"],
-                            allow_headers=["*"]):
+                            modules: list = [],
+                            allow_origins=[],
+                            allow_methods=[],
+                            allow_headers=[]):
     logging.basicConfig()
 
     # Install packages.
     poetry_install()
 
+    # Add modules to the list
+    for module in modules:
+        modules_list.append(module)
+
     app = TwirpASGIApp()
     services.append(CameraServiceServer(service=CameraService()))
 
     for service in services:
         app.add_service(service)
```

### Comparing `cv_smart_house_camera-0.1.1/cv_smart_house_camera/cam_capture.py` & `cv_smart_house_camera-0.1.2/cv_smart_house_camera/cam_capture.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import cv2
-from cv_smart_house_camera.data.frames import modules_result
 from cv_smart_house_camera.modules.modules_processing import modules_processing
 
 def cam_capture():
     cap = cv2.VideoCapture(0)  # 0 for default webcam, change if necessary
     frame_number = 0
     while True:
         try:
```

### Comparing `cv_smart_house_camera-0.1.1/cv_smart_house_camera/generate_code.py` & `cv_smart_house_camera-0.1.2/cv_smart_house_camera/generate_code.py`

 * *Files identical despite different names*

### Comparing `cv_smart_house_camera-0.1.1/cv_smart_house_camera/modules/modules_processing.py` & `cv_smart_house_camera-0.1.2/cv_smart_house_camera/modules/modules_processing.py`

 * *Files identical despite different names*

### Comparing `cv_smart_house_camera-0.1.1/cv_smart_house_camera/proto_services/camera_service_pb2.py` & `cv_smart_house_camera-0.1.2/cv_smart_house_camera/proto_services/camera_service_pb2.py`

 * *Files identical despite different names*

### Comparing `cv_smart_house_camera-0.1.1/cv_smart_house_camera/proto_services/camera_service_twirp.py` & `cv_smart_house_camera-0.1.2/cv_smart_house_camera/proto_services/camera_service_twirp.py`

 * *Files identical despite different names*

### Comparing `cv_smart_house_camera-0.1.1/pyproject.toml` & `cv_smart_house_camera-0.1.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cv-smart-house-camera"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = [ "Your Name <you@example.com>",]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 flask = "^3.0.3"
@@ -19,12 +19,11 @@
 opencv-python = "^4.9.0.80"
 twirp = "^0.0.7"
 protobuf = "^5.26.1"
 uvicorn = "^0.29.0"
 starlette = "^0.37.2"
 aiohttp = "^3.9.5"
 aiortc = "^1.8.0"
-module_1st = "1.4.0"
 
 [tool.poetry.scripts]
-start = "camera_service.__init__:start"
+start = "cv_smart_house_camera.__init__:configure_camera_server"
 compile = "compile_proto:compile_proto_files"
```

### Comparing `cv_smart_house_camera-0.1.1/PKG-INFO` & `cv_smart_house_camera-0.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: cv-smart-house-camera
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9.5,<4.0.0)
 Requires-Dist: aiortc (>=1.8.0,<2.0.0)
 Requires-Dist: flask (>=3.0.3,<4.0.0)
 Requires-Dist: grpcio (>=1.63.0,<2.0.0)
 Requires-Dist: grpcio-tools (>=1.63.0,<2.0.0)
-Requires-Dist: module_1st (==1.4.0)
 Requires-Dist: opencv-python (>=4.9.0.80,<5.0.0.0)
 Requires-Dist: protobuf (>=5.26.1,<6.0.0)
 Requires-Dist: requests (==2.31.0)
 Requires-Dist: starlette (>=0.37.2,<0.38.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: twirp (>=0.0.7,<0.0.8)
 Requires-Dist: uvicorn (>=0.29.0,<0.30.0)
```

