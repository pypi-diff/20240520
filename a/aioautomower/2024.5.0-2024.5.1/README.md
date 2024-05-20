# Comparing `tmp/aioautomower-2024.5.0.tar.gz` & `tmp/aioautomower-2024.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioautomower-2024.5.0.tar", max compression
+gzip compressed data, was "aioautomower-2024.5.1.tar", max compression
```

## Comparing `aioautomower-2024.5.0.tar` & `aioautomower-2024.5.1.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     2001 2024-05-06 16:16:07.208152 aioautomower-2024.5.0/README.md
--rw-r--r--   0        0        0     8389 2024-05-06 16:16:18.016122 aioautomower-2024.5.0/pyproject.toml
--rw-r--r--   0        0        0      138 2024-05-06 16:16:07.208152 aioautomower-2024.5.0/src/aioautomower/__init__.py
--rw-r--r--   0        0        0      108 2024-05-06 16:16:07.208152 aioautomower-2024.5.0/src/aioautomower/_secrets.yaml
--rw-r--r--   0        0        0     7241 2024-05-06 16:16:07.208152 aioautomower-2024.5.0/src/aioautomower/auth.py
--rw-r--r--   0        0        0     5812 2024-05-06 16:16:07.208152 aioautomower-2024.5.0/src/aioautomower/const.py
--rw-r--r--   0        0        0     5123 2024-05-06 16:16:07.208152 aioautomower-2024.5.0/src/aioautomower/example.py
--rw-r--r--   0        0        0      970 2024-05-06 16:16:07.208152 aioautomower-2024.5.0/src/aioautomower/exceptions.py
--rw-r--r--   0        0        0    15474 2024-05-06 16:16:07.208152 aioautomower-2024.5.0/src/aioautomower/model.py
--rw-r--r--   0        0        0        0 2024-05-06 16:16:07.208152 aioautomower-2024.5.0/src/aioautomower/py.typed
--rw-r--r--   0        0        0    13861 2024-05-06 16:16:07.208152 aioautomower-2024.5.0/src/aioautomower/session.py
--rw-r--r--   0        0        0     3659 2024-05-06 16:16:07.208152 aioautomower-2024.5.0/src/aioautomower/utils.py
--rw-r--r--   0        0        0     2811 1970-01-01 00:00:00.000000 aioautomower-2024.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1984 2024-05-20 18:07:01.128114 aioautomower-2024.5.1/README.md
+-rw-r--r--   0        0        0     8398 2024-05-20 18:07:14.732231 aioautomower-2024.5.1/pyproject.toml
+-rw-r--r--   0        0        0      138 2024-05-20 18:07:01.128114 aioautomower-2024.5.1/src/aioautomower/__init__.py
+-rw-r--r--   0        0        0      108 2024-05-20 18:07:01.128114 aioautomower-2024.5.1/src/aioautomower/_secrets.yaml
+-rw-r--r--   0        0        0     7320 2024-05-20 18:07:01.128114 aioautomower-2024.5.1/src/aioautomower/auth.py
+-rw-r--r--   0        0        0     5812 2024-05-20 18:07:01.128114 aioautomower-2024.5.1/src/aioautomower/const.py
+-rw-r--r--   0        0        0     1093 2024-05-20 18:07:01.128114 aioautomower-2024.5.1/src/aioautomower/exceptions.py
+-rw-r--r--   0        0        0    15589 2024-05-20 18:07:01.128114 aioautomower-2024.5.1/src/aioautomower/model.py
+-rw-r--r--   0        0        0        0 2024-05-20 18:07:01.128114 aioautomower-2024.5.1/src/aioautomower/py.typed
+-rw-r--r--   0        0        0    15817 2024-05-20 18:07:01.128114 aioautomower-2024.5.1/src/aioautomower/session.py
+-rw-r--r--   0        0        0     3659 2024-05-20 18:07:01.128114 aioautomower-2024.5.1/src/aioautomower/utils.py
+-rw-r--r--   0        0        0     2794 1970-01-01 00:00:00.000000 aioautomower-2024.5.1/PKG-INFO
```

### Comparing `aioautomower-2024.5.0/README.md` & `aioautomower-2024.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 For a first start you can run the `example.py`, by doing the following steps
 
 - `git clone https://github.com/Thomas55555/aioautomower.git`
 - `cd aioautomower`
 - `poetry install`
 - Enter your personal `client_id` and `client_secret` in the `_secrets.yaml` and rename it to `secrets.yaml`
-- Run with `poetry run ./src/aioautomower/example.py`
+- Run with `poetry run ./example.py`
 
 ## Contributing
 
 This is an active open-source project. We are always open to people who want to use the code or contribute to it.
 This Python project is fully managed using the [Poetry][poetry] dependency manager.
 
 As this repository uses the [pre-commit][pre-commit] framework, all changes
```

### Comparing `aioautomower-2024.5.0/pyproject.toml` & `aioautomower-2024.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "aioautomower"
 # The version is set by GH action on release
-version = "2024.5.0"
+version = "2024.5.1"
 description = "MPython module to talk to Husqvarna Automower."
 authors = ["Thomas55555"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [
     { include = "aioautomower", from = "src" },
 ]
@@ -27,26 +27,26 @@
 PyJWT = "^2.8.0"
 
 [tool.poetry.group.dev.dependencies]
 codespell = "2.2.6"
 covdefaults = "2.3.0"
 coverage = {version = "7.5.1", extras = ["toml"]}
 mypy = "1.10.0"
-pre-commit = "3.7.0"
+pre-commit = "3.7.1"
 pre-commit-hooks = "4.6.0"
-pylint = "3.1.0"
+pylint = "3.2.1"
 pytest = "8.2.0"
 pytest-asyncio = "0.23.6"
 pytest-cov = "5.0.0"
-ruff = "0.4.3"
+ruff = "0.4.4"
 safety = "3.2.0"
 yamllint = "1.35.1"
 syrupy = "4.6.1"
 aioresponses = "0.7.6"
-freezegun = "1.5.0"
+freezegun = "1.5.1"
 pyyaml = "6.0.1"
 types-pyyaml = "^6.0.12.20240311"
 
 [tool.pytest.ini_options]
 addopts = "--cov"
 asyncio_mode = "auto"
 
@@ -183,15 +183,15 @@
     "RET501",
     "TRY002",
     "TRY301"
 ]
 
 [tool.ruff.lint.per-file-ignores]
 # Allow for main entry & scripts to write to stdout
-"src/aioautomower/example.py" = ["T201"]
+"example.py" = ["T201"]
 
 [tool.pylint.FORMAT]
 max-line-length = 88
 
 [tool.ruff.lint.flake8-annotations]
 allow-star-arg-any = true
 suppress-dummy-args = true
@@ -242,7 +242,8 @@
 
 [tool.coverage.report]
 show_missing = true
 fail_under = 50
 
 [tool.coverage.run]
 plugins = ["covdefaults"]
+source = ["aioautomower"]
```

### Comparing `aioautomower-2024.5.0/src/aioautomower/auth.py` & `aioautomower-2024.5.1/src/aioautomower/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     WSServerHandshakeError,
 )
 
 from .const import API_BASE_URL, AUTH_HEADER_FMT, WS_URL
 from .exceptions import (
     ApiException,
     ApiForbiddenException,
+    ApiUnauthorizedException,
     AuthException,
     HusqvarnaWSServerHandshakeError,
 )
 from .utils import structure_token
 
 ERROR = "error"
 STATUS = "status"
@@ -148,15 +149,17 @@
             resp.raise_for_status()
         except ClientResponseError as err:
             if err.status == HTTPStatus.FORBIDDEN:
                 raise ApiForbiddenException(
                     f"Forbidden response from API: {err}"
                 ) from err
             if err.status == HTTPStatus.UNAUTHORIZED:
-                raise AuthException(f"Unable to authenticate with API: {err}") from err
+                raise ApiUnauthorizedException(
+                    f"Unable to authenticate with API: {err}"
+                ) from err
             detail.append(err.message)
             raise ApiException(": ".join(detail)) from err
         except ClientError as err:
             raise ApiException(f"Error from API: {err}") from err
         return resp
 
     @staticmethod
```

### Comparing `aioautomower-2024.5.0/src/aioautomower/const.py` & `aioautomower-2024.5.1/src/aioautomower/const.py`

 * *Files identical despite different names*

### Comparing `aioautomower-2024.5.0/src/aioautomower/exceptions.py` & `aioautomower-2024.5.1/src/aioautomower/exceptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,14 +17,18 @@
     """Raised when the sync token is invalid."""
 
 
 class ApiForbiddenException(HusqvarnaAutomowerException):
     """Raised due to permission errors talking to API."""
 
 
+class ApiUnauthorizedException(HusqvarnaAutomowerException):
+    """Raised occasionally, mustn't harm the connection."""
+
+
 class NoDataAvailableException(HusqvarnaAutomowerException):
     """Raised due updating data, when no data is available."""
 
 
 class TimeoutException(HusqvarnaAutomowerException):
     """Raised due connecting the websocket."""
```

### Comparing `aioautomower-2024.5.0/src/aioautomower/model.py` & `aioautomower-2024.5.1/src/aioautomower/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -435,30 +435,37 @@
     """DataClass for WorkAreas values."""
 
     name: str
     cutting_height: int
 
 
 @dataclass
+class Settings(DataClassDictMixin):
+    """DataClass for WorkAreas values."""
+
+    headlight: Headlight
+    cutting_height: int | None = field(
+        metadata=field_options(alias="cuttingHeight"), default=None
+    )
+
+
+@dataclass
 class MowerAttributes(DataClassDictMixin):
     """DataClass for MowerAttributes."""
 
     system: System
     battery: Battery
     capabilities: Capabilities
     mower: Mower
     calendar: Tasks
     planner: Planner
     metadata: Metadata
     positions: list[Positions] | None
+    settings: Settings
     statistics: Statistics
-    headlight: Headlight
-    cutting_height: int | None = field(
-        metadata=field_options(alias="cuttingHeight"), default=None
-    )
     stay_out_zones: StayOutZones | None = field(
         metadata=field_options(alias="stayOutZones"), default=None
     )
     work_areas: dict[int, WorkArea] | None = field(
         metadata=field_options(
             deserialize=lambda workarea_list: {
                 area.work_area_id: WorkArea(
```

### Comparing `aioautomower-2024.5.0/src/aioautomower/session.py` & `aioautomower-2024.5.1/src/aioautomower/session.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """Module to connect to Automower with websocket."""
 
 import asyncio
 import contextlib
 import datetime
 import logging
 from dataclasses import dataclass
-from typing import Any, Literal, Mapping
+from typing import Any, Iterable, Literal, Mapping
 
 from aiohttp import WSMessage, WSMsgType
 
 from .auth import AbstractAuth
 from .const import EVENT_TYPES, REST_POLL_CYCLE
 from .exceptions import NoDataAvailableException, TimeoutException
 from .model import HeadlightModes, MowerAttributes
 from .utils import mower_list_to_dictionary_dataclass
 
 _LOGGER = logging.getLogger(__name__)
 
+logging.basicConfig(level=logging.DEBUG)
+
 
 @dataclass
 class AutomowerEndpoint:
     """Endpoint URLs for the AutomowerConnect API."""
 
     mowers = "mowers/"
     "List data for all mowers linked to a user."
@@ -212,15 +214,15 @@
         poll: bool = False,
     ) -> None:
         """Create a session.
 
         :param class auth: The AbstractAuth class from aioautomower.auth.
         :param bool poll: Poll data with rest if True.
         """
-        self._data: Mapping[Any, Any] | None = {}
+        self._data: dict[str, Iterable[Any]] | None = {}
         self.auth = auth
         self.commands = _MowerCommands(self.auth)
         self.pong_cbs: list = []
         self.data_update_cbs: list = []
         self.data: dict[str, MowerAttributes] = {}
         self.last_ws_message: datetime.datetime
         self.loop: asyncio.AbstractEventLoop = asyncio.get_running_loop()
@@ -285,24 +287,75 @@
         """
         self._schedule_data_callbacks()
 
         if self.poll:
             await self.get_status()
             self.rest_task = asyncio.create_task(self._rest_task())
 
-    def handle_text_message(self, msg: WSMessage) -> None:
-        """Send an empty message every 60s."""
+    def add_settigs_tree(self, msg_dict: dict) -> dict:
+        """Add settings key and ignore empty calendar tasks.
+
+        Needed, because when polling the API `headlight` and `cuttingHeight` are
+        nested under the `settings` key. But when receiving a websocket message,
+        the `settings` key is missing.
+        """
+        copy_msg_dict = dict(msg_dict)
+        current_data = self._data
+        if current_data is None:
+            raise NoDataAvailableException
+        dater_iter = current_data["data"]
+        for _, current_data_mower in enumerate(dater_iter):
+            if current_data_mower["id"] == copy_msg_dict["id"]:
+                current_attributes = current_data_mower["attributes"]
+                formated_msg = {
+                    "id": current_data_mower["id"],
+                    "type": "settings-event",
+                    "attributes": {
+                        "calendar": {"tasks": current_attributes["calendar"]["tasks"]},
+                        "settings": {
+                            "cuttingHeight": current_attributes["settings"][
+                                "cuttingHeight"
+                            ],
+                            "headlight": {
+                                "mode": current_attributes["settings"]["headlight"][
+                                    "mode"
+                                ]
+                            },
+                        },
+                    },
+                }
+                new_attributes = copy_msg_dict["attributes"]
+                if len(new_attributes["calendar"]["tasks"]) > 0:
+                    formated_msg["attributes"]["calendar"]["tasks"] = copy_msg_dict[
+                        "attributes"
+                    ]["calendar"]["tasks"]
+                if "cuttingHeight" in new_attributes:
+                    formated_msg["attributes"]["settings"]["cuttingHeight"] = (
+                        copy_msg_dict["attributes"]["cuttingHeight"]
+                    )
+                if "headlight" in new_attributes:
+                    formated_msg["attributes"]["settings"]["headlight"]["mode"] = (
+                        copy_msg_dict["attributes"]["headlight"]["mode"]
+                    )
+                return formated_msg
+        return copy_msg_dict
+
+    def _handle_text_message(self, msg: WSMessage) -> None:
+        """Process a text message to data."""
         if not msg.data:
             self.last_ws_message = datetime.datetime.now(tz=datetime.UTC)
             _LOGGER.debug("last_ws_message:%s", self.last_ws_message)
             self._schedule_pong_callbacks()
         if msg.data:
             msg_dict = msg.json()
             if "type" in msg_dict:
                 if msg_dict["type"] in EVENT_TYPES:
+                    if msg_dict["type"] == "settings-event":
+                        copy = dict(msg_dict)
+                        msg_dict = self.add_settigs_tree(copy)
                     _LOGGER.debug("Got %s, data: %s", msg_dict["type"], msg_dict)
                     self._update_data(msg_dict)
                 else:
                     _LOGGER.warning("Received unknown ws type %s", msg_dict["type"])
             elif "ready" in msg_dict and "connectionId" in msg_dict:
                 _LOGGER.debug(
                     "Websocket ready=%s (id='%s')",
@@ -318,15 +371,15 @@
                 if msg.type in (
                     WSMsgType.CLOSE,
                     WSMsgType.CLOSING,
                     WSMsgType.CLOSED,
                 ):
                     break
                 if msg.type == WSMsgType.TEXT:
-                    self.handle_text_message(msg)
+                    self._handle_text_message(msg)
                 elif msg.type == WSMsgType.ERROR:
                     continue
             except TimeoutError as exc:
                 raise TimeoutException from exc
 
     async def send_empty_message(self) -> None:
         """Send an empty message every 60s."""
@@ -334,43 +387,30 @@
             await asyncio.sleep(60)
             _LOGGER.debug("ping:%s", datetime.datetime.now(tz=datetime.UTC))
             await self.auth.ws.send_str("")
 
     async def get_status(self) -> dict[str, MowerAttributes]:
         """Get mower status via Rest."""
         mower_list = await self.auth.get_json(AutomowerEndpoint.mowers)
-        for idx, _ent in enumerate(mower_list["data"]):
-            mower_list["data"][idx]["attributes"].update(
-                mower_list["data"][idx]["attributes"]["settings"]
-            )
-            del mower_list["data"][idx]["attributes"]["settings"]
         self._data = mower_list
         self.data = mower_list_to_dictionary_dataclass(self._data)
         return self.data
 
     def _update_data(self, new_data) -> None:
-        """Update internal data, with new data from websocket.
-
-        Empty tasks are ignored, so we always know the tasks.
-        """
+        """Update internal data, with new data from websocket."""
         if self._data is None:
             raise NoDataAvailableException
 
-        for datum in self._data["data"]:
-            if datum["type"] == "mower" and datum["id"] == new_data["id"]:
+        data = self._data["data"]
+        for mower in data:
+            if mower["type"] == "mower" and mower["id"] == new_data["id"]:
                 new_attributes: Mapping[Any, Any] = new_data["attributes"]
                 value: Mapping[Any, Any]
                 for attrib, value in new_attributes.items():
-                    if attrib == "calendar":
-                        tasks = value.get("tasks", [])
-                        if tasks:
-                            datum["attributes"]["calendar"]["tasks"] = tasks
-                    else:
-                        datum["attributes"][attrib] = value
-
+                    mower["attributes"][attrib] = value
         self.data = mower_list_to_dictionary_dataclass(self._data)
         self._schedule_data_callbacks()
 
     async def _rest_task(self) -> None:
         """Poll data periodically via Rest."""
         while True:
             await self.get_status()
```

### Comparing `aioautomower-2024.5.0/src/aioautomower/utils.py` & `aioautomower-2024.5.1/src/aioautomower/utils.py`

 * *Files identical despite different names*

### Comparing `aioautomower-2024.5.0/PKG-INFO` & `aioautomower-2024.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioautomower
-Version: 2024.5.0
+Version: 2024.5.1
 Summary: MPython module to talk to Husqvarna Automower.
 Home-page: https://github.com/Thomas55555/aioautomower
 License: Apache 2.0
 Author: Thomas55555
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -42,15 +42,15 @@
 
 For a first start you can run the `example.py`, by doing the following steps
 
 - `git clone https://github.com/Thomas55555/aioautomower.git`
 - `cd aioautomower`
 - `poetry install`
 - Enter your personal `client_id` and `client_secret` in the `_secrets.yaml` and rename it to `secrets.yaml`
-- Run with `poetry run ./src/aioautomower/example.py`
+- Run with `poetry run ./example.py`
 
 ## Contributing
 
 This is an active open-source project. We are always open to people who want to use the code or contribute to it.
 This Python project is fully managed using the [Poetry][poetry] dependency manager.
 
 As this repository uses the [pre-commit][pre-commit] framework, all changes
```

