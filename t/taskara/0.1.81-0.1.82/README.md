# Comparing `tmp/taskara-0.1.81.tar.gz` & `tmp/taskara-0.1.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskara-0.1.81.tar", max compression
+gzip compressed data, was "taskara-0.1.82.tar", max compression
```

## Comparing `taskara-0.1.81.tar` & `taskara-0.1.82.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1069 2024-04-17 17:09:32.374116 taskara-0.1.81/LICENSE
--rw-r--r--   0        0        0     2060 2024-05-18 03:15:36.175112 taskara-0.1.81/README.md
--rw-r--r--   0        0        0     1149 2024-05-20 19:16:30.781156 taskara-0.1.81/pyproject.toml
--rw-r--r--   0        0        0       81 2024-04-30 21:36:12.359132 taskara-0.1.81/taskara/__init__.py
--rw-r--r--   0        0        0     1725 2024-04-30 21:35:45.162984 taskara-0.1.81/taskara/agent.py
--rw-r--r--   0        0        0       23 2024-04-25 16:52:45.140876 taskara-0.1.81/taskara/auth/default.py
--rw-r--r--   0        0        0     2548 2024-05-18 03:15:36.178446 taskara-0.1.81/taskara/auth/key.py
--rw-r--r--   0        0        0     3106 2024-05-18 03:15:36.178774 taskara-0.1.81/taskara/auth/provider.py
--rw-r--r--   0        0        0     1446 2024-05-18 03:15:36.179051 taskara-0.1.81/taskara/auth/transport.py
--rw-r--r--   0        0        0     3250 2024-05-18 03:15:36.179410 taskara-0.1.81/taskara/cli/main.py
--rw-r--r--   0        0        0      672 2024-05-18 03:15:36.179529 taskara-0.1.81/taskara/config.py
--rw-r--r--   0        0        0     2517 2024-05-18 03:15:36.179872 taskara-0.1.81/taskara/db/conn.py
--rw-r--r--   0        0        0     1639 2024-05-18 03:15:36.180173 taskara-0.1.81/taskara/db/models.py
--rw-r--r--   0        0        0      195 2024-04-30 21:35:42.361364 taskara-0.1.81/taskara/env.py
--rw-r--r--   0        0        0     1520 2024-04-30 21:35:40.978077 taskara-0.1.81/taskara/metrics.py
--rw-r--r--   0        0        0    11573 2024-05-18 03:15:36.180417 taskara-0.1.81/taskara/runtime/base.py
--rw-r--r--   0        0        0    11091 2024-05-18 03:15:36.180578 taskara-0.1.81/taskara/runtime/docker.py
--rw-r--r--   0        0        0    28338 2024-05-18 03:15:36.180876 taskara-0.1.81/taskara/runtime/kube.py
--rw-r--r--   0        0        0     1983 2024-05-18 03:15:36.181027 taskara-0.1.81/taskara/runtime/load.py
--rw-r--r--   0        0        0    13524 2024-05-18 03:15:36.181232 taskara-0.1.81/taskara/runtime/process.py
--rw-r--r--   0        0        0     2243 2024-05-18 03:15:36.181763 taskara-0.1.81/taskara/server/app.py
--rw-r--r--   0        0        0     2747 2024-05-18 03:15:36.182016 taskara-0.1.81/taskara/server/models.py
--rw-r--r--   0        0        0     8468 2024-05-18 03:15:36.182433 taskara-0.1.81/taskara/server/router/tasks.py
--rw-r--r--   0        0        0    35236 2024-05-20 19:16:35.335676 taskara-0.1.81/taskara/task.py
--rw-r--r--   0        0        0     1810 2024-05-18 03:15:36.183189 taskara-0.1.81/taskara/util.py
--rw-r--r--   0        0        0     3314 1970-01-01 00:00:00.000000 taskara-0.1.81/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-17 17:09:32.374116 taskara-0.1.82/LICENSE
+-rw-r--r--   0        0        0     2060 2024-05-18 03:15:36.175112 taskara-0.1.82/README.md
+-rw-r--r--   0        0        0     1149 2024-05-20 19:30:07.725248 taskara-0.1.82/pyproject.toml
+-rw-r--r--   0        0        0       81 2024-04-30 21:36:12.359132 taskara-0.1.82/taskara/__init__.py
+-rw-r--r--   0        0        0     1725 2024-04-30 21:35:45.162984 taskara-0.1.82/taskara/agent.py
+-rw-r--r--   0        0        0       23 2024-04-25 16:52:45.140876 taskara-0.1.82/taskara/auth/default.py
+-rw-r--r--   0        0        0     2548 2024-05-18 03:15:36.178446 taskara-0.1.82/taskara/auth/key.py
+-rw-r--r--   0        0        0     3106 2024-05-18 03:15:36.178774 taskara-0.1.82/taskara/auth/provider.py
+-rw-r--r--   0        0        0     1446 2024-05-18 03:15:36.179051 taskara-0.1.82/taskara/auth/transport.py
+-rw-r--r--   0        0        0     3250 2024-05-18 03:15:36.179410 taskara-0.1.82/taskara/cli/main.py
+-rw-r--r--   0        0        0      672 2024-05-18 03:15:36.179529 taskara-0.1.82/taskara/config.py
+-rw-r--r--   0        0        0     2517 2024-05-18 03:15:36.179872 taskara-0.1.82/taskara/db/conn.py
+-rw-r--r--   0        0        0     1639 2024-05-18 03:15:36.180173 taskara-0.1.82/taskara/db/models.py
+-rw-r--r--   0        0        0      195 2024-04-30 21:35:42.361364 taskara-0.1.82/taskara/env.py
+-rw-r--r--   0        0        0     1520 2024-04-30 21:35:40.978077 taskara-0.1.82/taskara/metrics.py
+-rw-r--r--   0        0        0    11573 2024-05-18 03:15:36.180417 taskara-0.1.82/taskara/runtime/base.py
+-rw-r--r--   0        0        0    11912 2024-05-20 19:30:07.725603 taskara-0.1.82/taskara/runtime/docker.py
+-rw-r--r--   0        0        0    28338 2024-05-18 03:15:36.180876 taskara-0.1.82/taskara/runtime/kube.py
+-rw-r--r--   0        0        0     1983 2024-05-18 03:15:36.181027 taskara-0.1.82/taskara/runtime/load.py
+-rw-r--r--   0        0        0    13524 2024-05-18 03:15:36.181232 taskara-0.1.82/taskara/runtime/process.py
+-rw-r--r--   0        0        0     2243 2024-05-18 03:15:36.181763 taskara-0.1.82/taskara/server/app.py
+-rw-r--r--   0        0        0     2747 2024-05-18 03:15:36.182016 taskara-0.1.82/taskara/server/models.py
+-rw-r--r--   0        0        0     8468 2024-05-18 03:15:36.182433 taskara-0.1.82/taskara/server/router/tasks.py
+-rw-r--r--   0        0        0    35236 2024-05-20 19:16:35.335676 taskara-0.1.82/taskara/task.py
+-rw-r--r--   0        0        0     1810 2024-05-18 03:15:36.183189 taskara-0.1.82/taskara/util.py
+-rw-r--r--   0        0        0     3314 1970-01-01 00:00:00.000000 taskara-0.1.82/PKG-INFO
```

### Comparing `taskara-0.1.81/LICENSE` & `taskara-0.1.82/LICENSE`

 * *Files identical despite different names*

### Comparing `taskara-0.1.81/README.md` & `taskara-0.1.82/README.md`

 * *Files identical despite different names*

### Comparing `taskara-0.1.81/pyproject.toml` & `taskara-0.1.82/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taskara"
-version = "0.1.81"
+version = "0.1.82"
 description = "Task management for AI agents"
 authors = ["Patrick Barker <patrickbarkerco@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `taskara-0.1.81/taskara/agent.py` & `taskara-0.1.82/taskara/agent.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.81/taskara/auth/key.py` & `taskara-0.1.82/taskara/auth/key.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.81/taskara/auth/provider.py` & `taskara-0.1.82/taskara/auth/provider.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.81/taskara/auth/transport.py` & `taskara-0.1.82/taskara/auth/transport.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.81/taskara/cli/main.py` & `taskara-0.1.82/taskara/cli/main.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.81/taskara/config.py` & `taskara-0.1.82/taskara/config.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.81/taskara/db/conn.py` & `taskara-0.1.82/taskara/db/conn.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.81/taskara/db/models.py` & `taskara-0.1.82/taskara/db/models.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.81/taskara/metrics.py` & `taskara-0.1.82/taskara/metrics.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.81/taskara/runtime/base.py` & `taskara-0.1.82/taskara/runtime/base.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.81/taskara/runtime/docker.py` & `taskara-0.1.82/taskara/runtime/docker.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import List, Optional, Type, Union, Iterator, Dict, Tuple
 import signal
 import sys
 import urllib.request
 import urllib.error
 import urllib.parse
 import json
+import os
 
 import docker
 from docker.errors import NotFound
 from taskara.util import find_open_port
 from pydantic import BaseModel
 
 from taskara.server.models import (
@@ -25,25 +26,42 @@
     timeout: Optional[int] = None
     image: str = "us-central1-docker.pkg.dev/agentsea-dev/taskara/api:latest"
 
 
 class DockerTrackerRuntime(TrackerRuntime["DockerTrackerRuntime", DockerConnectConfig]):
 
     def __init__(self, cfg: Optional[DockerConnectConfig] = None) -> None:
+        self._configure_docker_socket()
         if not cfg:
             cfg = DockerConnectConfig()
 
         self.img = cfg.image
 
         self._cfg = cfg
         if cfg.timeout:
             self.client = docker.from_env(timeout=cfg.timeout)
         else:
             self.client = docker.from_env()
 
+    def _configure_docker_socket(self):
+        if os.path.exists("/var/run/docker.sock"):
+            docker_socket = "unix:///var/run/docker.sock"
+        else:
+            user = os.environ.get("USER")
+            if os.path.exists(f"/Users/{user}/.docker/run/docker.sock"):
+                docker_socket = f"unix:///Users/{user}/.docker/run/docker.sock"
+            else:
+                raise FileNotFoundError(
+                    (
+                        "Neither '/var/run/docker.sock' nor '/Users/<USER>/.docker/run/docker.sock' are available."
+                        "Please make sure you have Docker installed and running."
+                    )
+                )
+        os.environ["DOCKER_HOST"] = docker_socket
+
     @classmethod
     def name(cls) -> str:
         return "docker"
 
     @classmethod
     def connect_config_type(cls) -> Type[DockerConnectConfig]:
         return DockerConnectConfig
@@ -113,14 +131,16 @@
         env_vars: Optional[dict] = None,
         owner_id: Optional[str] = None,
         labels: Optional[Dict[str, str]] = None,
         resource_requests: V1ResourceRequests = V1ResourceRequests(),
         resource_limits: V1ResourceLimits = V1ResourceLimits(),
         auth_enabled: bool = True,
     ) -> Tracker:
+
+        self.client.images.pull(self.img)
         _labels = {
             "provisioner": "taskara",
             "server_name": name,
         }
         if labels:
             _labels.update(labels)
```

### Comparing `taskara-0.1.81/taskara/runtime/kube.py` & `taskara-0.1.82/taskara/runtime/kube.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.81/taskara/runtime/load.py` & `taskara-0.1.82/taskara/runtime/load.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.81/taskara/runtime/process.py` & `taskara-0.1.82/taskara/runtime/process.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.81/taskara/server/app.py` & `taskara-0.1.82/taskara/server/app.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.81/taskara/server/models.py` & `taskara-0.1.82/taskara/server/models.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.81/taskara/server/router/tasks.py` & `taskara-0.1.82/taskara/server/router/tasks.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.81/taskara/task.py` & `taskara-0.1.82/taskara/task.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.81/taskara/util.py` & `taskara-0.1.82/taskara/util.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.81/PKG-INFO` & `taskara-0.1.82/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskara
-Version: 0.1.81
+Version: 0.1.82
 Summary: Task management for AI agents
 License: MIT
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: taskara Version: 0.1.81 Summary: Task management
+Metadata-Version: 2.1 Name: taskara Version: 0.1.82 Summary: Task management
 for AI agents License: MIT Author: Patrick Barker Author-email:
 patrickbarkerco@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Provides-Extra: all Provides-Extra: cli Provides-
 Extra: runtime Requires-Dist: devicebay (>=0.1.21,<0.2.0) Requires-Dist: docker
 (>=7.0.0,<8.0.0) ; extra == "runtime" or extra == "all" Requires-Dist: google-
```

