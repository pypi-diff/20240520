# Comparing `tmp/nora_lib-0.0.4.tar.gz` & `tmp/nora_lib-0.0.5.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nora_lib-0.0.4.tar", last modified: Tue May 14 16:13:39 2024, max compression
+gzip compressed data, was "nora_lib-0.0.5.dev0.tar", last modified: Mon May 20 21:13:04 2024, max compression
```

## Comparing `nora_lib-0.0.4.tar` & `nora_lib-0.0.5.dev0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 reganh     (502) staff       (20)        0 2024-05-14 16:13:39.274597 nora_lib-0.0.4/
--rw-r--r--   0 reganh     (502) staff       (20)      407 2024-05-14 16:13:39.274310 nora_lib-0.0.4/PKG-INFO
--rw-r--r--   0 reganh     (502) staff       (20)      887 2024-05-09 17:31:43.000000 nora_lib-0.0.4/README.md
-drwxr-xr-x   0 reganh     (502) staff       (20)        0 2024-05-14 16:13:39.265471 nora_lib-0.0.4/nora_lib/
--rw-r--r--   0 reganh     (502) staff       (20)        0 2024-05-03 17:18:14.000000 nora_lib-0.0.4/nora_lib/__init__.py
-drwxr-xr-x   0 reganh     (502) staff       (20)        0 2024-05-14 16:13:39.267147 nora_lib-0.0.4/nora_lib/context/
--rw-r--r--   0 reganh     (502) staff       (20)        0 2024-05-09 17:26:38.000000 nora_lib-0.0.4/nora_lib/context/__init__.py
--rw-r--r--   0 reganh     (502) staff       (20)     3390 2024-05-14 16:12:32.000000 nora_lib-0.0.4/nora_lib/context/context_service.py
--rw-r--r--   0 reganh     (502) staff       (20)      757 2024-05-09 17:26:38.000000 nora_lib-0.0.4/nora_lib/context/models.py
-drwxr-xr-x   0 reganh     (502) staff       (20)        0 2024-05-14 16:13:39.271911 nora_lib-0.0.4/nora_lib/interactions/
--rw-r--r--   0 reganh     (502) staff       (20)        0 2024-05-09 17:26:38.000000 nora_lib-0.0.4/nora_lib/interactions/__init__.py
--rw-r--r--   0 reganh     (502) staff       (20)     4731 2024-05-14 16:12:32.000000 nora_lib-0.0.4/nora_lib/interactions/interactions_service.py
--rw-r--r--   0 reganh     (502) staff       (20)     3381 2024-05-14 16:12:32.000000 nora_lib-0.0.4/nora_lib/interactions/models.py
--rw-r--r--   0 reganh     (502) staff       (20)        0 2024-05-03 17:18:14.000000 nora_lib-0.0.4/nora_lib/py.typed
-drwxr-xr-x   0 reganh     (502) staff       (20)        0 2024-05-14 16:13:39.272604 nora_lib-0.0.4/nora_lib/tasks/
--rw-r--r--   0 reganh     (502) staff       (20)        0 2024-05-03 17:18:14.000000 nora_lib-0.0.4/nora_lib/tasks/__init__.py
--rw-r--r--   0 reganh     (502) staff       (20)      925 2024-05-03 17:18:14.000000 nora_lib-0.0.4/nora_lib/tasks/models.py
--rw-r--r--   0 reganh     (502) staff       (20)     1793 2024-05-03 17:18:14.000000 nora_lib-0.0.4/nora_lib/tasks/state.py
-drwxr-xr-x   0 reganh     (502) staff       (20)        0 2024-05-14 16:13:39.273778 nora_lib-0.0.4/nora_lib.egg-info/
--rw-r--r--   0 reganh     (502) staff       (20)      407 2024-05-14 16:13:39.000000 nora_lib-0.0.4/nora_lib.egg-info/PKG-INFO
--rw-r--r--   0 reganh     (502) staff       (20)      587 2024-05-14 16:13:39.000000 nora_lib-0.0.4/nora_lib.egg-info/SOURCES.txt
--rw-r--r--   0 reganh     (502) staff       (20)        1 2024-05-14 16:13:39.000000 nora_lib-0.0.4/nora_lib.egg-info/dependency_links.txt
--rw-r--r--   0 reganh     (502) staff       (20)       64 2024-05-14 16:13:39.000000 nora_lib-0.0.4/nora_lib.egg-info/requires.txt
--rw-r--r--   0 reganh     (502) staff       (20)       15 2024-05-14 16:13:39.000000 nora_lib-0.0.4/nora_lib.egg-info/top_level.txt
--rw-r--r--   0 reganh     (502) staff       (20)       90 2024-05-03 17:18:14.000000 nora_lib-0.0.4/pyproject.toml
--rw-r--r--   0 reganh     (502) staff       (20)       38 2024-05-14 16:13:39.274659 nora_lib-0.0.4/setup.cfg
--rw-r--r--   0 reganh     (502) staff       (20)      600 2024-05-14 16:12:32.000000 nora_lib-0.0.4/setup.py
-drwxr-xr-x   0 reganh     (502) staff       (20)        0 2024-05-14 16:13:39.272794 nora_lib-0.0.4/tests/
-drwxr-xr-x   0 reganh     (502) staff       (20)        0 2024-05-14 16:13:39.273115 nora_lib-0.0.4/tests/tasks/
--rw-r--r--   0 reganh     (502) staff       (20)        0 2024-05-03 17:18:14.000000 nora_lib-0.0.4/tests/tasks/__init__.py
--rw-r--r--   0 reganh     (502) staff       (20)     2670 2024-05-03 17:18:14.000000 nora_lib-0.0.4/tests/tasks/test_state.py
--rw-r--r--   0 reganh     (502) staff       (20)      123 2024-05-03 17:18:14.000000 nora_lib-0.0.4/tests/test_placeholder.py
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 21:13:04.261158 nora_lib-0.0.5.dev0/
+-rw-r--r--   0 stefanc    (502) staff       (20)      412 2024-05-20 21:13:04.260002 nora_lib-0.0.5.dev0/PKG-INFO
+-rw-r--r--   0 stefanc    (502) staff       (20)      887 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev0/README.md
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 21:13:04.243296 nora_lib-0.0.5.dev0/nora_lib/
+-rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev0/nora_lib/__init__.py
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 21:13:04.248623 nora_lib-0.0.5.dev0/nora_lib/context/
+-rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev0/nora_lib/context/__init__.py
+-rw-r--r--   0 stefanc    (502) staff       (20)     1338 2024-05-17 21:59:16.000000 nora_lib-0.0.5.dev0/nora_lib/context/context_service.py
+-rw-r--r--   0 stefanc    (502) staff       (20)      356 2024-05-17 21:59:16.000000 nora_lib-0.0.5.dev0/nora_lib/context/models.py
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 21:13:04.251074 nora_lib-0.0.5.dev0/nora_lib/interactions/
+-rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev0/nora_lib/interactions/__init__.py
+-rw-r--r--   0 stefanc    (502) staff       (20)     5133 2024-05-20 21:12:03.000000 nora_lib-0.0.5.dev0/nora_lib/interactions/interactions_service.py
+-rw-r--r--   0 stefanc    (502) staff       (20)     4196 2024-05-20 21:09:30.000000 nora_lib-0.0.5.dev0/nora_lib/interactions/models.py
+-rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev0/nora_lib/py.typed
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 21:13:04.253691 nora_lib-0.0.5.dev0/nora_lib/tasks/
+-rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev0/nora_lib/tasks/__init__.py
+-rw-r--r--   0 stefanc    (502) staff       (20)      925 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev0/nora_lib/tasks/models.py
+-rw-r--r--   0 stefanc    (502) staff       (20)     1793 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev0/nora_lib/tasks/state.py
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 21:13:04.257581 nora_lib-0.0.5.dev0/nora_lib.egg-info/
+-rw-r--r--   0 stefanc    (502) staff       (20)      412 2024-05-20 21:13:04.000000 nora_lib-0.0.5.dev0/nora_lib.egg-info/PKG-INFO
+-rw-r--r--   0 stefanc    (502) staff       (20)      587 2024-05-20 21:13:04.000000 nora_lib-0.0.5.dev0/nora_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 stefanc    (502) staff       (20)        1 2024-05-20 21:13:04.000000 nora_lib-0.0.5.dev0/nora_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 stefanc    (502) staff       (20)       64 2024-05-20 21:13:04.000000 nora_lib-0.0.5.dev0/nora_lib.egg-info/requires.txt
+-rw-r--r--   0 stefanc    (502) staff       (20)       15 2024-05-20 21:13:04.000000 nora_lib-0.0.5.dev0/nora_lib.egg-info/top_level.txt
+-rw-r--r--   0 stefanc    (502) staff       (20)       90 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev0/pyproject.toml
+-rw-r--r--   0 stefanc    (502) staff       (20)       38 2024-05-20 21:13:04.261384 nora_lib-0.0.5.dev0/setup.cfg
+-rw-r--r--   0 stefanc    (502) staff       (20)      605 2024-05-20 21:09:30.000000 nora_lib-0.0.5.dev0/setup.py
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 21:13:04.254789 nora_lib-0.0.5.dev0/tests/
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 21:13:04.256176 nora_lib-0.0.5.dev0/tests/tasks/
+-rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev0/tests/tasks/__init__.py
+-rw-r--r--   0 stefanc    (502) staff       (20)     2670 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev0/tests/tasks/test_state.py
+-rw-r--r--   0 stefanc    (502) staff       (20)      123 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev0/tests/test_placeholder.py
```

### Comparing `nora_lib-0.0.4/README.md` & `nora_lib-0.0.5.dev0/README.md`

 * *Files identical despite different names*

### Comparing `nora_lib-0.0.4/nora_lib/interactions/interactions_service.py` & `nora_lib-0.0.5.dev0/nora_lib/interactions/interactions_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from datetime import datetime
 import requests
 from typing import List, Optional
 
 from nora_lib.interactions.models import (
     Event,
     EventType,
+    Message,
     ReturnedMessage,
     ThreadRelationsResponse,
     ThreadForkEventData,
     thread_message_lookup_request,
 )
 
 
@@ -18,14 +19,25 @@
     """
 
     def __init__(self, base_url, timeout, token):
         self.base_url = base_url
         self.timeout = timeout
         self.headers = {"Authorization": f"Bearer {token}"}
 
+    def save_message(self, message: Message) -> None:
+        """Save a message to the Interactions API"""
+        message_url = f"{self.base_url}/interaction/v1/message"
+        response = requests.post(
+            message_url,
+            json=message.model_dump(),
+            headers=self.headers,
+            timeout=int(self.timeout),
+        )
+        response.raise_for_status()
+
     def save_event(self, event: Event) -> None:
         """Save an event to the Interactions API"""
         event_url = f"{self.base_url}/interaction/v1/event"
         response = requests.post(
             event_url,
             json=event.model_dump(),
             headers=self.headers,
```

### Comparing `nora_lib-0.0.4/nora_lib/interactions/models.py` & `nora_lib-0.0.5.dev0/nora_lib/interactions/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,14 +6,48 @@
 from enum import Enum
 from typing import Dict, List, Optional, Tuple
 from uuid import UUID
 
 from pydantic import BaseModel, Field, field_serializer, ConfigDict
 
 
+class Surface(str, Enum):
+    SLACK = "Slack"
+    WEB = "NoraWebapp"
+
+
+class Annotation(BaseModel):
+    # Need this config to stringify numeric values in attributes.
+    # Otherwise, we'll get 'Input should be a valid string' error.
+    model_config = ConfigDict(coerce_numbers_to_str=True)
+
+    tag: str
+    span: Tuple[int, int]
+    attributes: Optional[Dict[str, str]] = None
+
+
+class Message(BaseModel):
+    message_id: str
+    actor_id: UUID
+    text: str
+    thread_id: Optional[str]
+    channel_id: str
+    surface: Surface
+    ts: datetime
+    annotations: Optional[List[Annotation]] = None
+
+    @field_serializer("actor_id")
+    def serialize_actor_id(self, actor_id: UUID):
+        return str(actor_id)
+
+    @field_serializer("ts")
+    def serialize_ts(self, ts: datetime):
+        return ts.isoformat()
+
+
 class EventType(str, Enum):
     """Event types for the interactions service"""
 
     AGENT_CONTEXT = "agent:message_context"
     THREAD_FORK = "thread_fork"
```

### Comparing `nora_lib-0.0.4/nora_lib/tasks/models.py` & `nora_lib-0.0.5.dev0/nora_lib/tasks/models.py`

 * *Files identical despite different names*

### Comparing `nora_lib-0.0.4/nora_lib/tasks/state.py` & `nora_lib-0.0.5.dev0/nora_lib/tasks/state.py`

 * *Files identical despite different names*

### Comparing `nora_lib-0.0.4/nora_lib.egg-info/SOURCES.txt` & `nora_lib-0.0.5.dev0/nora_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nora_lib-0.0.4/setup.py` & `nora_lib-0.0.5.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 runtime_requirements = ["pydantic>=2,<3", "requests"]
 
 # For running tests, linting, etc
 dev_requirements = ["mypy", "pytest", "black", "types-requests"]
 
 setuptools.setup(
     name="nora_lib",
-    version="0.0.4",
+    version="0.0.5.dev0",
     description="For making and coordinating agents and tools",
     url="https://github.com/allenai/nora_lib",
     packages=setuptools.find_packages(exclude=(["tests"])),
     install_requires=runtime_requirements,
     package_data={
         "nora_lib": ["py.typed"],
     },
```

### Comparing `nora_lib-0.0.4/tests/tasks/test_state.py` & `nora_lib-0.0.5.dev0/tests/tasks/test_state.py`

 * *Files identical despite different names*

