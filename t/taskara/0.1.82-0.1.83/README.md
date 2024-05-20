# Comparing `tmp/taskara-0.1.82.tar.gz` & `tmp/taskara-0.1.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskara-0.1.82.tar", max compression
+gzip compressed data, was "taskara-0.1.83.tar", max compression
```

## Comparing `taskara-0.1.82.tar` & `taskara-0.1.83.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1069 2024-04-17 17:09:32.374116 taskara-0.1.82/LICENSE
--rw-r--r--   0        0        0     2060 2024-05-18 03:15:36.175112 taskara-0.1.82/README.md
--rw-r--r--   0        0        0     1149 2024-05-20 19:30:07.725248 taskara-0.1.82/pyproject.toml
--rw-r--r--   0        0        0       81 2024-04-30 21:36:12.359132 taskara-0.1.82/taskara/__init__.py
--rw-r--r--   0        0        0     1725 2024-04-30 21:35:45.162984 taskara-0.1.82/taskara/agent.py
--rw-r--r--   0        0        0       23 2024-04-25 16:52:45.140876 taskara-0.1.82/taskara/auth/default.py
--rw-r--r--   0        0        0     2548 2024-05-18 03:15:36.178446 taskara-0.1.82/taskara/auth/key.py
--rw-r--r--   0        0        0     3106 2024-05-18 03:15:36.178774 taskara-0.1.82/taskara/auth/provider.py
--rw-r--r--   0        0        0     1446 2024-05-18 03:15:36.179051 taskara-0.1.82/taskara/auth/transport.py
--rw-r--r--   0        0        0     3250 2024-05-18 03:15:36.179410 taskara-0.1.82/taskara/cli/main.py
--rw-r--r--   0        0        0      672 2024-05-18 03:15:36.179529 taskara-0.1.82/taskara/config.py
--rw-r--r--   0        0        0     2517 2024-05-18 03:15:36.179872 taskara-0.1.82/taskara/db/conn.py
--rw-r--r--   0        0        0     1639 2024-05-18 03:15:36.180173 taskara-0.1.82/taskara/db/models.py
--rw-r--r--   0        0        0      195 2024-04-30 21:35:42.361364 taskara-0.1.82/taskara/env.py
--rw-r--r--   0        0        0     1520 2024-04-30 21:35:40.978077 taskara-0.1.82/taskara/metrics.py
--rw-r--r--   0        0        0    11573 2024-05-18 03:15:36.180417 taskara-0.1.82/taskara/runtime/base.py
--rw-r--r--   0        0        0    11912 2024-05-20 19:30:07.725603 taskara-0.1.82/taskara/runtime/docker.py
--rw-r--r--   0        0        0    28338 2024-05-18 03:15:36.180876 taskara-0.1.82/taskara/runtime/kube.py
--rw-r--r--   0        0        0     1983 2024-05-18 03:15:36.181027 taskara-0.1.82/taskara/runtime/load.py
--rw-r--r--   0        0        0    13524 2024-05-18 03:15:36.181232 taskara-0.1.82/taskara/runtime/process.py
--rw-r--r--   0        0        0     2243 2024-05-18 03:15:36.181763 taskara-0.1.82/taskara/server/app.py
--rw-r--r--   0        0        0     2747 2024-05-18 03:15:36.182016 taskara-0.1.82/taskara/server/models.py
--rw-r--r--   0        0        0     8468 2024-05-18 03:15:36.182433 taskara-0.1.82/taskara/server/router/tasks.py
--rw-r--r--   0        0        0    35236 2024-05-20 19:16:35.335676 taskara-0.1.82/taskara/task.py
--rw-r--r--   0        0        0     1810 2024-05-18 03:15:36.183189 taskara-0.1.82/taskara/util.py
--rw-r--r--   0        0        0     3314 1970-01-01 00:00:00.000000 taskara-0.1.82/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-17 17:09:32.374116 taskara-0.1.83/LICENSE
+-rw-r--r--   0        0        0     2060 2024-05-18 03:15:36.175112 taskara-0.1.83/README.md
+-rw-r--r--   0        0        0     1149 2024-05-20 20:14:55.701697 taskara-0.1.83/pyproject.toml
+-rw-r--r--   0        0        0       81 2024-04-30 21:36:12.359132 taskara-0.1.83/taskara/__init__.py
+-rw-r--r--   0        0        0     1725 2024-04-30 21:35:45.162984 taskara-0.1.83/taskara/agent.py
+-rw-r--r--   0        0        0       23 2024-04-25 16:52:45.140876 taskara-0.1.83/taskara/auth/default.py
+-rw-r--r--   0        0        0     2548 2024-05-18 03:15:36.178446 taskara-0.1.83/taskara/auth/key.py
+-rw-r--r--   0        0        0     3106 2024-05-18 03:15:36.178774 taskara-0.1.83/taskara/auth/provider.py
+-rw-r--r--   0        0        0     1446 2024-05-18 03:15:36.179051 taskara-0.1.83/taskara/auth/transport.py
+-rw-r--r--   0        0        0     3250 2024-05-18 03:15:36.179410 taskara-0.1.83/taskara/cli/main.py
+-rw-r--r--   0        0        0      672 2024-05-18 03:15:36.179529 taskara-0.1.83/taskara/config.py
+-rw-r--r--   0        0        0     2517 2024-05-18 03:15:36.179872 taskara-0.1.83/taskara/db/conn.py
+-rw-r--r--   0        0        0     1639 2024-05-18 03:15:36.180173 taskara-0.1.83/taskara/db/models.py
+-rw-r--r--   0        0        0      195 2024-04-30 21:35:42.361364 taskara-0.1.83/taskara/env.py
+-rw-r--r--   0        0        0     1520 2024-04-30 21:35:40.978077 taskara-0.1.83/taskara/metrics.py
+-rw-r--r--   0        0        0    11573 2024-05-18 03:15:36.180417 taskara-0.1.83/taskara/runtime/base.py
+-rw-r--r--   0        0        0    11912 2024-05-20 19:30:07.725603 taskara-0.1.83/taskara/runtime/docker.py
+-rw-r--r--   0        0        0    28338 2024-05-18 03:15:36.180876 taskara-0.1.83/taskara/runtime/kube.py
+-rw-r--r--   0        0        0     1983 2024-05-18 03:15:36.181027 taskara-0.1.83/taskara/runtime/load.py
+-rw-r--r--   0        0        0    13524 2024-05-18 03:15:36.181232 taskara-0.1.83/taskara/runtime/process.py
+-rw-r--r--   0        0        0     2243 2024-05-18 03:15:36.181763 taskara-0.1.83/taskara/server/app.py
+-rw-r--r--   0        0        0     2753 2024-05-20 20:14:55.702101 taskara-0.1.83/taskara/server/models.py
+-rw-r--r--   0        0        0     8468 2024-05-18 03:15:36.182433 taskara-0.1.83/taskara/server/router/tasks.py
+-rw-r--r--   0        0        0    35495 2024-05-20 20:14:55.702609 taskara-0.1.83/taskara/task.py
+-rw-r--r--   0        0        0     1947 2024-05-20 20:14:55.702891 taskara-0.1.83/taskara/util.py
+-rw-r--r--   0        0        0     3314 1970-01-01 00:00:00.000000 taskara-0.1.83/PKG-INFO
```

### Comparing `taskara-0.1.82/LICENSE` & `taskara-0.1.83/LICENSE`

 * *Files identical despite different names*

### Comparing `taskara-0.1.82/README.md` & `taskara-0.1.83/README.md`

 * *Files identical despite different names*

### Comparing `taskara-0.1.82/pyproject.toml` & `taskara-0.1.83/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taskara"
-version = "0.1.82"
+version = "0.1.83"
 description = "Task management for AI agents"
 authors = ["Patrick Barker <patrickbarkerco@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `taskara-0.1.82/taskara/agent.py` & `taskara-0.1.83/taskara/agent.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.82/taskara/auth/key.py` & `taskara-0.1.83/taskara/auth/key.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.82/taskara/auth/provider.py` & `taskara-0.1.83/taskara/auth/provider.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.82/taskara/auth/transport.py` & `taskara-0.1.83/taskara/auth/transport.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.82/taskara/cli/main.py` & `taskara-0.1.83/taskara/cli/main.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.82/taskara/config.py` & `taskara-0.1.83/taskara/config.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.82/taskara/db/conn.py` & `taskara-0.1.83/taskara/db/conn.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.82/taskara/db/models.py` & `taskara-0.1.83/taskara/db/models.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.82/taskara/metrics.py` & `taskara-0.1.83/taskara/metrics.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.82/taskara/runtime/base.py` & `taskara-0.1.83/taskara/runtime/base.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.82/taskara/runtime/docker.py` & `taskara-0.1.83/taskara/runtime/docker.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.82/taskara/runtime/kube.py` & `taskara-0.1.83/taskara/runtime/kube.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.82/taskara/runtime/load.py` & `taskara-0.1.83/taskara/runtime/load.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.82/taskara/runtime/process.py` & `taskara-0.1.83/taskara/runtime/process.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.82/taskara/server/app.py` & `taskara-0.1.83/taskara/server/app.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.82/taskara/server/models.py` & `taskara-0.1.83/taskara/server/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     version: Optional[str] = None
 
 
 class V1Task(BaseModel):
     id: str = Field(default_factory=lambda: str(uuid.uuid4()))
     description: str
     max_steps: int = 30
-    device: Optional[V1Device] = None
+    device: Optional[V1Device | str] = None
     device_type: Optional[V1DeviceType] = None
     status: Optional[str] = None
     threads: Optional[List[V1RoleThread]] = None
     prompts: Optional[List[str]] = None
     assigned_to: Optional[str] = None
     assigned_type: Optional[str] = None
     created: float = Field(default_factory=time.time)
```

### Comparing `taskara-0.1.82/taskara/server/router/tasks.py` & `taskara-0.1.83/taskara/server/router/tasks.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.82/taskara/task.py` & `taskara-0.1.83/taskara/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,28 +14,29 @@
 from devicebay import V1Device, V1DeviceType
 from pydantic import BaseModel
 
 from .db.models import TaskRecord
 from .db.conn import WithDB
 from .server.models import V1Prompts, V1Task, V1TaskUpdate, V1Tasks
 from .env import HUB_API_KEY_ENV
+from .util import is_json
 
 T = TypeVar("T", bound="Task")
 logger = logging.getLogger(__name__)
 
 
 class Task(WithDB):
     """An agent task"""
 
     def __init__(
         self,
         description: Optional[str] = None,
         max_steps: int = 30,
         owner_id: Optional[str] = None,
-        device: Optional[V1Device] = None,
+        device: Optional[V1Device | str] = None,
         device_type: Optional[V1DeviceType] = None,
         id: Optional[str] = None,
         status: str = "defined",
         created: Optional[float] = None,
         started: float = 0.0,
         completed: float = 0.0,
         threads: List[RoleThread] = [],
@@ -115,15 +116,15 @@
         return self._max_steps
 
     @max_steps.setter
     def max_steps(self, value: int):
         self._max_steps = value
 
     @property
-    def device(self) -> Optional[V1Device]:
+    def device(self) -> Optional[V1Device | str]:
         return self._device
 
     @device.setter
     def device(self, value: Optional[V1Device]):
         self._device = value
 
     @property
@@ -254,15 +255,18 @@
     def to_record(self) -> TaskRecord:
         version = None
         if hasattr(self, "_version"):
             version = self._version
 
         device = None
         if self._device:
-            device = self._device.model_dump_json()
+            if isinstance(self._device, V1Device):
+                device = self._device.model_dump_json()
+            else:
+                device = self._device
 
         device_type = None
         if self._device_type:
             device_type = self._device_type.model_dump_json()
 
         if not hasattr(self, "_episode") or not self._episode:
             raise ValueError("episode not set")
@@ -302,15 +306,18 @@
         parameters = json.loads(str(record.parameters))
 
         episodes = Episode.find(id=record.episode_id)
         episode = episodes[0]
 
         device = None
         if record.device:  # type: ignore
-            device = V1Device.model_validate_json(str(record.device))
+            if is_json(str(record.device)):
+                device = V1Device.model_validate_json(str(record.device))
+            else:
+                device = str(record.device)
 
         device_type = None
         if record.device_type:  # type: ignore
             device_type = V1DeviceType.model_validate_json(str(record.device_type))
 
         obj = cls.__new__(cls)
         obj._id = record.id
```

### Comparing `taskara-0.1.82/taskara/util.py` & `taskara-0.1.83/taskara/util.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import random
 import string
 import subprocess
 from typing import Optional
 import socket
+import json
 
 
 def generate_random_string(length: int = 8):
     """Generate a random string of fixed length."""
     letters = string.ascii_letters + string.digits
     return "".join(random.choices(letters, k=length))
 
@@ -51,7 +52,15 @@
         with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
             try:
                 s.bind(("", port))
                 return port  # Port is open
             except socket.error:
                 continue  # Port is in use, try the next one
     return None  # No open port found
+
+
+def is_json(my_string):
+    try:
+        json.loads(my_string)
+    except ValueError:
+        return False
+    return True
```

### Comparing `taskara-0.1.82/PKG-INFO` & `taskara-0.1.83/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskara
-Version: 0.1.82
+Version: 0.1.83
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
-Metadata-Version: 2.1 Name: taskara Version: 0.1.82 Summary: Task management
+Metadata-Version: 2.1 Name: taskara Version: 0.1.83 Summary: Task management
 for AI agents License: MIT Author: Patrick Barker Author-email:
 patrickbarkerco@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Provides-Extra: all Provides-Extra: cli Provides-
 Extra: runtime Requires-Dist: devicebay (>=0.1.21,<0.2.0) Requires-Dist: docker
 (>=7.0.0,<8.0.0) ; extra == "runtime" or extra == "all" Requires-Dist: google-
```

