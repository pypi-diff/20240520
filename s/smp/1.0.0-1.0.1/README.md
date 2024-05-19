# Comparing `tmp/smp-1.0.0.tar.gz` & `tmp/smp-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smp-1.0.0.tar", max compression
+gzip compressed data, was "smp-1.0.1.tar", max compression
```

## Comparing `smp-1.0.0.tar` & `smp-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11365 2024-04-27 18:16:42.546318 smp-1.0.0/LICENSE
--rw-r--r--   0        0        0     2243 2024-04-27 18:16:42.546318 smp-1.0.0/README.md
--rw-r--r--   0        0        0      953 2024-04-27 18:16:42.546318 smp-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-27 18:16:42.546318 smp-1.0.0/smp/__init__.py
--rw-r--r--   0        0        0      659 2024-04-27 18:16:42.546318 smp-1.0.0/smp/error.py
--rw-r--r--   0        0        0      471 2024-04-27 18:16:42.546318 smp-1.0.0/smp/exceptions.py
--rw-r--r--   0        0        0     4978 2024-04-27 18:16:42.546318 smp-1.0.0/smp/header.py
--rw-r--r--   0        0        0     6149 2024-04-27 18:16:42.546318 smp-1.0.0/smp/image_management.py
--rw-r--r--   0        0        0     4846 2024-04-27 18:16:42.546318 smp-1.0.0/smp/message.py
--rw-r--r--   0        0        0     6761 2024-04-27 18:16:42.546318 smp-1.0.0/smp/os_management.py
--rw-r--r--   0        0        0     3135 2024-04-27 18:16:42.546318 smp-1.0.0/smp/packet.py
--rw-r--r--   0        0        0        0 2024-04-27 18:16:42.546318 smp-1.0.0/smp/py.typed
--rw-r--r--   0        0        0     1071 2024-04-27 18:16:42.546318 smp-1.0.0/smp/shell_management.py
--rw-r--r--   0        0        0        0 2024-04-27 18:16:42.546318 smp-1.0.0/smp/user/__init__.py
--rw-r--r--   0        0        0     1371 2024-04-27 18:16:42.546318 smp-1.0.0/smp/user/intercreate.py
--rw-r--r--   0        0        0     2894 1970-01-01 00:00:00.000000 smp-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11365 2024-05-19 22:32:36.689672 smp-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2312 2024-05-19 22:32:36.689672 smp-1.0.1/README.md
+-rw-r--r--   0        0        0     1595 2024-05-19 22:32:36.689672 smp-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-19 22:32:36.689672 smp-1.0.1/smp/__init__.py
+-rw-r--r--   0        0        0      695 2024-05-19 22:32:36.689672 smp-1.0.1/smp/error.py
+-rw-r--r--   0        0        0      471 2024-05-19 22:32:36.689672 smp-1.0.1/smp/exceptions.py
+-rw-r--r--   0        0        0     5090 2024-05-19 22:32:36.689672 smp-1.0.1/smp/header.py
+-rw-r--r--   0        0        0     6286 2024-05-19 22:32:36.689672 smp-1.0.1/smp/image_management.py
+-rw-r--r--   0        0        0     4882 2024-05-19 22:32:36.689672 smp-1.0.1/smp/message.py
+-rw-r--r--   0        0        0     7153 2024-05-19 22:32:36.689672 smp-1.0.1/smp/os_management.py
+-rw-r--r--   0        0        0     3135 2024-05-19 22:32:36.689672 smp-1.0.1/smp/packet.py
+-rw-r--r--   0        0        0        0 2024-05-19 22:32:36.689672 smp-1.0.1/smp/py.typed
+-rw-r--r--   0        0        0     1022 2024-05-19 22:32:36.689672 smp-1.0.1/smp/shell_management.py
+-rw-r--r--   0        0        0        0 2024-05-19 22:32:36.689672 smp-1.0.1/smp/user/__init__.py
+-rw-r--r--   0        0        0     1321 2024-05-19 22:32:36.689672 smp-1.0.1/smp/user/intercreate.py
+-rw-r--r--   0        0        0     3087 1970-01-01 00:00:00.000000 smp-1.0.1/PKG-INFO
```

### Comparing `smp-1.0.0/LICENSE` & `smp-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `smp-1.0.0/README.md` & `smp-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -30,20 +30,24 @@
    ```
    poetry add <my_new_dependency>
    ```
 6. add test or other development dependencies using [poetry groups](https://python-poetry.org/docs/managing-dependencies#dependency-groups):
    ```
    poetry add -G dev <my_dev_dependency>
    ```
+7.  run tests for all supported python versions:
+   ```
+   tox
+   ```
 
 ## Development Environment Setup
 
 ### Install Dependencies
 
-- python >=3.10, <3.13
+- python >=3.8, <3.13
 - poetry: https://python-poetry.org/docs/#installation
 
 ### Create the venv
 
 ```
 poetry install
 ```
```

### Comparing `smp-1.0.0/smp/error.py` & `smp-1.0.1/smp/error.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """The Simple Management Protocol (SMP) error responses."""
 
+from __future__ import annotations
+
 from enum import IntEnum
 from typing import Generic, TypeVar
 
 from pydantic import BaseModel, ConfigDict
 
 from smp import message
 from smp.header import GroupId
```

### Comparing `smp-1.0.0/smp/header.py` & `smp-1.0.1/smp/header.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 """The Simple Management Protocol (SMP) header."""
 
+from __future__ import annotations
+
 import struct
 from dataclasses import dataclass
 from enum import IntEnum, IntFlag, auto, unique
-from typing import ClassVar, Dict, Type, TypeAlias
+from typing import ClassVar, Dict, Type, Union
+
+from typing_extensions import TypeAlias
 
 
 class CommandId:
     @unique
     class OSManagement(IntEnum):
         ECHO = 0
         ECHO_CONTROL = 1
@@ -33,15 +37,15 @@
         EXECUTE = 0
 
     @unique
     class Intercreate(IntEnum):
         UPLOAD = 1
 
 
-AnyCommandId: TypeAlias = IntEnum | int
+AnyCommandId: TypeAlias = Union[IntEnum, int]
 
 
 @unique
 class GroupId(IntEnum):
     OS_MANAGEMENT = 0
     IMAGE_MANAGEMENT = 1
     STATISTICS_MANAGEMENT = 2
@@ -59,15 +63,15 @@
     """Users may define their own Group IDs starting at 64.
 
     It is optional to register them here."""
 
     INTERCREATE = 64
 
 
-AnyGroupId: TypeAlias = IntEnum | int
+AnyGroupId: TypeAlias = Union[IntEnum, int]
 
 
 @unique
 class OP(IntEnum):
     READ = 0
     READ_RSP = 1
     WRITE = 2
@@ -97,31 +101,31 @@
 
 @dataclass(frozen=True)
 class Header:
     op: OP
     version: Version
     flags: Flag
     length: int
-    group_id: AnyGroupId | GroupId | UserGroupId
+    group_id: Union[AnyGroupId, GroupId, UserGroupId]
     sequence: int
-    command_id: (
-        AnyCommandId
-        | CommandId.OSManagement
-        | CommandId.ImageManagement
-        | CommandId.ShellManagement
-        | CommandId.Intercreate
-    )
+    command_id: Union[
+        AnyCommandId,
+        CommandId.OSManagement,
+        CommandId.ImageManagement,
+        CommandId.ShellManagement,
+        CommandId.Intercreate,
+    ]
 
     _MAP_GROUP_ID_TO_COMMAND_ID_ENUM: ClassVar[Dict[int, Type[IntEnum]]] = {
         GroupId.OS_MANAGEMENT: CommandId.OSManagement,
         GroupId.IMAGE_MANAGEMENT: CommandId.ImageManagement,
         GroupId.SHELL_MANAGEMENT: CommandId.ShellManagement,
     }
-    _STRUCT: ClassVar = struct.Struct("!BBHHBB")
-    SIZE: ClassVar = _STRUCT.size
+    _STRUCT: ClassVar[struct.Struct] = struct.Struct("!BBHHBB")
+    SIZE: ClassVar[int] = _STRUCT.size
 
     @staticmethod
     def _pack_op(op: OP) -> int:
         """The value to be packed into the byte."""
         return op << _OP_BIT.SHIFT
 
     @staticmethod
```

### Comparing `smp-1.0.0/smp/image_management.py` & `smp-1.0.1/smp/image_management.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 """The Simple Management Protocol (SMP) Image Management group."""
 
+from __future__ import annotations
+
 from enum import IntEnum, auto, unique
-from typing import ClassVar, Generator, List
+from typing import Generator, List
 
 from pydantic import BaseModel, ConfigDict, ValidationInfo, field_validator
 
 from smp import error, header, message
 
 
-class _ImageManagementGroup:
-    _GROUP_ID: ClassVar = header.GroupId.IMAGE_MANAGEMENT
-
-
 class HashBytes(bytes):  # pragma: no cover
     """Only to print something useful to the console."""
 
     def __rich_repr__(self) -> Generator[str, None, None]:
         yield self.hex().upper()
 
 
@@ -36,69 +34,77 @@
     @classmethod
     def cast_bytes(cls, v: bytes | None, _: ValidationInfo) -> HashBytes | None:
         if v is None:
             return None
         return HashBytes(v)
 
 
-class ImageStatesReadRequest(_ImageManagementGroup, message.ReadRequest):
+class ImageStatesReadRequest(message.ReadRequest):
+    _GROUP_ID = header.GroupId.IMAGE_MANAGEMENT
     _COMMAND_ID = header.CommandId.ImageManagement.STATE
 
 
-class ImageStatesReadResponse(_ImageManagementGroup, message.ReadResponse):
+class ImageStatesReadResponse(message.ReadResponse):
+    _GROUP_ID = header.GroupId.IMAGE_MANAGEMENT
     _COMMAND_ID = header.CommandId.ImageManagement.STATE
 
     images: List[ImageState]
     splitStatus: int | None = None
 
 
-class ImageStatesWriteRequest(_ImageManagementGroup, message.WriteRequest):
+class ImageStatesWriteRequest(message.WriteRequest):
+    _GROUP_ID = header.GroupId.IMAGE_MANAGEMENT
     _COMMAND_ID = header.CommandId.ImageManagement.STATE
 
     hash: bytes
     confirm: bool = False
 
 
 class ImageStatesWriteResponse(ImageStatesReadResponse):
     pass
 
 
-class ImageUploadWriteRequest(_ImageManagementGroup, message.WriteRequest):
+class ImageUploadWriteRequest(message.WriteRequest):
+    _GROUP_ID = header.GroupId.IMAGE_MANAGEMENT
     _COMMAND_ID = header.CommandId.ImageManagement.UPLOAD
 
     off: int
     data: bytes
     image: int | None = None  # 'required' when off == 0
     len: int | None = None  # required when off == 0
     sha: bytes | None = None  # should be sent when off == 0
     upgrade: bool | None = None  # allowed when off == 0
 
 
-class ImageUploadProgressWriteResponse(_ImageManagementGroup, message.WriteResponse):
+class ImageUploadProgressWriteResponse(message.WriteResponse):
+    _GROUP_ID = header.GroupId.IMAGE_MANAGEMENT
     _COMMAND_ID = header.CommandId.ImageManagement.UPLOAD
 
     rc: int | None = None
     off: int | None = None
 
 
-class ImageUploadFinalWriteResponse(_ImageManagementGroup, message.WriteResponse):
+class ImageUploadFinalWriteResponse(message.WriteResponse):
+    _GROUP_ID = header.GroupId.IMAGE_MANAGEMENT
     _COMMAND_ID = header.CommandId.ImageManagement.UPLOAD
 
     off: int | None = None
     match: bool | None = None
 
 
-class ImageEraseRequest(_ImageManagementGroup, message.WriteRequest):
+class ImageEraseRequest(message.WriteRequest):
+    _GROUP_ID = header.GroupId.IMAGE_MANAGEMENT
     _COMMAND_ID = header.CommandId.ImageManagement.ERASE
 
     slot: int | None = None
     """The slot to erase. If not provided, slot 1 will be erased."""
 
 
-class ImageEraseResponse(_ImageManagementGroup, message.WriteResponse):
+class ImageEraseResponse(message.WriteResponse):
+    _GROUP_ID = header.GroupId.IMAGE_MANAGEMENT
     _COMMAND_ID = header.CommandId.ImageManagement.ERASE
 
 
 @unique
 class IMG_MGMT_ERR(IntEnum):
     OK = 0
     """No error, this is implied if there is no ret value in the response"""
```

### Comparing `smp-1.0.0/smp/message.py` & `smp-1.0.1/smp/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """The Simple Management Protocol (SMP) Message base class."""
 
+from __future__ import annotations
+
 import itertools
 from abc import ABC
 from enum import IntEnum, unique
 from typing import ClassVar, Type, TypeVar, cast
 
 import cbor2
 from pydantic import BaseModel, ConfigDict
```

### Comparing `smp-1.0.0/smp/os_management.py` & `smp-1.0.1/smp/os_management.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 """The Simple Management Protocol (SMP) OS Management group."""
 
+from __future__ import annotations
 
 from enum import IntEnum, auto, unique
-from typing import Any, ClassVar, Dict
+from typing import Any, Dict
 
 from pydantic import BaseModel, ConfigDict, Field
 
 from smp import error, header, message
 
 
-class _OSManagementGroup:
-    _GROUP_ID: ClassVar = header.GroupId.OS_MANAGEMENT
-
-
-class EchoWriteRequest(_OSManagementGroup, message.WriteRequest):
+class EchoWriteRequest(message.WriteRequest):
+    _GROUP_ID = header.GroupId.OS_MANAGEMENT
     _COMMAND_ID = header.CommandId.OSManagement.ECHO
 
     d: str
 
 
-class EchoWriteResponse(_OSManagementGroup, message.WriteResponse):
+class EchoWriteResponse(message.WriteResponse):
+    _GROUP_ID = header.GroupId.OS_MANAGEMENT
     _COMMAND_ID = header.CommandId.OSManagement.ECHO
 
     r: str
 
 
-class ResetWriteRequest(_OSManagementGroup, message.WriteRequest):
+class ResetWriteRequest(message.WriteRequest):
+    _GROUP_ID = header.GroupId.OS_MANAGEMENT
     _COMMAND_ID = header.CommandId.OSManagement.RESET
 
 
-class ResetWriteResponse(_OSManagementGroup, message.WriteResponse):
+class ResetWriteResponse(message.WriteResponse):
+    _GROUP_ID = header.GroupId.OS_MANAGEMENT
     _COMMAND_ID = header.CommandId.OSManagement.RESET
 
 
-class TaskStatisticsReadRequest(_OSManagementGroup, message.ReadRequest):
+class TaskStatisticsReadRequest(message.ReadRequest):
+    _GROUP_ID = header.GroupId.OS_MANAGEMENT
     _COMMAND_ID = header.CommandId.OSManagement.TASK_STATS
 
 
 class TaskStatistics(BaseModel):
     model_config = ConfigDict(extra="forbid", frozen=True)
 
     prio: int
@@ -62,21 +64,23 @@
     """Runtime in ticks."""
     last_checkin: int
     """Set to 0 by Zephyr."""
     next_checkin: int
     """Set to 0 by Zephyr."""
 
 
-class TaskStatisticsReadResponse(_OSManagementGroup, message.ReadResponse):
+class TaskStatisticsReadResponse(message.ReadResponse):
+    _GROUP_ID = header.GroupId.OS_MANAGEMENT
     _COMMAND_ID = header.CommandId.OSManagement.TASK_STATS
 
     tasks: Dict[str, TaskStatistics]
 
 
-class MemoryPoolStatisticsReadRequest(_OSManagementGroup, message.ReadRequest):
+class MemoryPoolStatisticsReadRequest(message.ReadRequest):
+    _GROUP_ID = header.GroupId.OS_MANAGEMENT
     _COMMAND_ID = header.CommandId.OSManagement.MEMORY_POOL_STATS
 
 
 class MemoryPoolStatistics(BaseModel):
     model_config = ConfigDict(extra="forbid", frozen=True)
 
     blksize: int
@@ -85,54 +89,62 @@
     """Number of memory blocks in the pool."""
     nfree: int
     """Number of free memory blocks in the pool."""
     min: int
     """Lowest number of free blocks the pool reached during run-time."""
 
 
-class MemoryPoolStatisticsReadResponse(_OSManagementGroup, message.ReadResponse):
+class MemoryPoolStatisticsReadResponse(message.ReadResponse):
     """The memory pools are accessed by name."""
 
     model_config = ConfigDict(extra="allow", frozen=True)
 
+    _GROUP_ID = header.GroupId.OS_MANAGEMENT
     _COMMAND_ID = header.CommandId.OSManagement.MEMORY_POOL_STATS
 
 
-class DateTimeReadRequest(_OSManagementGroup, message.ReadRequest):
+class DateTimeReadRequest(message.ReadRequest):
+    _GROUP_ID = header.GroupId.OS_MANAGEMENT
     _COMMAND_ID = header.CommandId.OSManagement.DATETIME_STRING
 
 
-class DateTimeReadResponse(_OSManagementGroup, message.ReadResponse):
+class DateTimeReadResponse(message.ReadResponse):
+    _GROUP_ID = header.GroupId.OS_MANAGEMENT
     _COMMAND_ID = header.CommandId.OSManagement.DATETIME_STRING
 
     datetime: str
 
 
-class DateTimeWriteRequest(_OSManagementGroup, message.WriteRequest):
+class DateTimeWriteRequest(message.WriteRequest):
+    _GROUP_ID = header.GroupId.OS_MANAGEMENT
     _COMMAND_ID = header.CommandId.OSManagement.DATETIME_STRING
 
     datetime: str
 
 
-class DateTimeWriteResponse(_OSManagementGroup, message.WriteResponse):
+class DateTimeWriteResponse(message.WriteResponse):
+    _GROUP_ID = header.GroupId.OS_MANAGEMENT
     _COMMAND_ID = header.CommandId.OSManagement.DATETIME_STRING
 
 
-class MCUMgrParametersReadRequest(_OSManagementGroup, message.ReadRequest):
+class MCUMgrParametersReadRequest(message.ReadRequest):
+    _GROUP_ID = header.GroupId.OS_MANAGEMENT
     _COMMAND_ID = header.CommandId.OSManagement.MCUMGR_PARAMETERS
 
 
-class MCUMgrParametersReadResponse(_OSManagementGroup, message.ReadResponse):
+class MCUMgrParametersReadResponse(message.ReadResponse):
+    _GROUP_ID = header.GroupId.OS_MANAGEMENT
     _COMMAND_ID = header.CommandId.OSManagement.MCUMGR_PARAMETERS
 
     buf_size: int
     buf_count: int
 
 
-class OSApplicationInfoReadRequest(_OSManagementGroup, message.ReadRequest):
+class OSApplicationInfoReadRequest(message.ReadRequest):
+    _GROUP_ID = header.GroupId.OS_MANAGEMENT
     _COMMAND_ID = header.CommandId.OSManagement.OS_APPLICATION_INFO
 
     format: str | None = None
     """Format specifier of returned response.
 
     Fields are appended in their natural ascending index order, not the order
     of characters that are received by the command.
@@ -149,21 +161,23 @@
     * `o` Operating system
     * `a` All fields (shorthand for all above options)
 
     If this option is not provided, the `s` Kernel name option will be used.
     """
 
 
-class OSApplicationInfoReadResponse(_OSManagementGroup, message.ReadResponse):
+class OSApplicationInfoReadResponse(message.ReadResponse):
+    _GROUP_ID = header.GroupId.OS_MANAGEMENT
     _COMMAND_ID = header.CommandId.OSManagement.OS_APPLICATION_INFO
 
     output: str
 
 
-class BootloaderInformationReadRequest(_OSManagementGroup, message.ReadRequest):
+class BootloaderInformationReadRequest(message.ReadRequest):
+    _GROUP_ID = header.GroupId.OS_MANAGEMENT
     _COMMAND_ID = header.CommandId.OSManagement.BOOTLOADER_INFO
 
     query: str | None = None
     """Is string representing query for parameters.
 
     With no restrictions how the query looks like as processing of query is left
     for bootloader backend. If there is no query, then response will return string
@@ -189,15 +203,16 @@
 class MCUbootModeQueryResponse(BaseModel):
     model_config = ConfigDict(extra="forbid", frozen=True)
 
     mode: MCUbootMode
     no_downgrade: bool | None = Field(alias="no-downgrade", default=None)
 
 
-class BootloaderInformationReadResponse(_OSManagementGroup, message.ReadResponse):
+class BootloaderInformationReadResponse(message.ReadResponse):
+    _GROUP_ID = header.GroupId.OS_MANAGEMENT
     _COMMAND_ID = header.CommandId.OSManagement.BOOTLOADER_INFO
 
     bootloader: str
     """String identifying the bootloader.  For MCUboot it will be "MCUboot"."""
     response: MCUbootModeQueryResponse | Any | None = None
     """Response to “query”.
```

### Comparing `smp-1.0.0/smp/packet.py` & `smp-1.0.1/smp/packet.py`

 * *Files identical despite different names*

### Comparing `smp-1.0.0/smp/shell_management.py` & `smp-1.0.1/smp/shell_management.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 """The Simple Management Protocol (SMP) Shell Management group."""
 
 
 from enum import IntEnum, auto, unique
-from typing import ClassVar, List
+from typing import List
 
 from smp import error, header, message
 
 
-class _ShellManagementGroup:
-    _GROUP_ID: ClassVar = header.GroupId.SHELL_MANAGEMENT
-
-
-class ExecuteRequest(_ShellManagementGroup, message.WriteRequest):
+class ExecuteRequest(message.WriteRequest):
+    _GROUP_ID = header.GroupId.SHELL_MANAGEMENT
     _COMMAND_ID = header.CommandId.ShellManagement.EXECUTE
 
     argv: List[str]
 
 
-class ExecuteResponse(_ShellManagementGroup, message.WriteResponse):
+class ExecuteResponse(message.WriteResponse):
+    _GROUP_ID = header.GroupId.SHELL_MANAGEMENT
     _COMMAND_ID = header.CommandId.ShellManagement.EXECUTE
 
     o: str
     ret: int
 
 
 @unique
```

### Comparing `smp-1.0.0/smp/user/intercreate.py` & `smp-1.0.1/smp/user/intercreate.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 """The Simple Management Protocol (SMP) Intercreate Management group."""
 
+from __future__ import annotations
+
 from enum import IntEnum, auto, unique
-from typing import ClassVar
 
 from smp import error, header, message
 
 
-class _IntercreateManagementGroup:
-    _GROUP_ID: ClassVar = header.UserGroupId.INTERCREATE
-
-
-class ImageUploadWriteRequest(_IntercreateManagementGroup, message.WriteRequest):
+class ImageUploadWriteRequest(message.WriteRequest):
+    _GROUP_ID = header.UserGroupId.INTERCREATE
     _COMMAND_ID = header.CommandId.Intercreate.UPLOAD
 
     off: int
     """The offset in the image to write to."""
 
     data: bytes
     """The data to write to the image."""
@@ -25,15 +23,16 @@
     len: int | None = None
     """The length of the data to write; required when off == 0."""
 
     sha: bytes | None = None
     """The SHA-256 hash of the image; optional when off == 0, else ignored."""
 
 
-class ImageUploadWriteResponse(_IntercreateManagementGroup, message.WriteResponse):
+class ImageUploadWriteResponse(message.WriteResponse):
+    _GROUP_ID = header.UserGroupId.INTERCREATE
     _COMMAND_ID = header.CommandId.Intercreate.UPLOAD
 
     off: int
     """The offset in the image after the request was written."""
 
 
 @unique
```

### Comparing `smp-1.0.0/PKG-INFO` & `smp-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: smp
-Version: 1.0.0
+Version: 1.0.1
 Summary: Simple Management Protocol (SMP) for remotely managing MCU firmware
 License: Apache-2.0
 Author: J.P. Hutchins
 Author-email: jphutchins@gmail.com
-Requires-Python: >=3.10,<3.13
+Requires-Python: >=3.8.1,<3.13
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: cbor2 (>=5.5.1,<6.0.0)
 Requires-Dist: crcmod (>=1.7,<2.0)
-Requires-Dist: pydantic (>=2.4.2,<3.0.0)
+Requires-Dist: eval-type-backport (>=0.2.0,<0.3.0) ; python_version < "3.10"
+Requires-Dist: pydantic (>=2.6,<3.0)
 Description-Content-Type: text/markdown
 
 # Simple Management Protocol (SMP)
 
 `smp` implements serialization and deserialization of the Simple Management Protocol.
 
 The SMP specification can be found [here](https://docs.zephyrproject.org/latest/services/device_mgmt/smp_protocol.html).
@@ -48,20 +50,24 @@
    ```
    poetry add <my_new_dependency>
    ```
 6. add test or other development dependencies using [poetry groups](https://python-poetry.org/docs/managing-dependencies#dependency-groups):
    ```
    poetry add -G dev <my_dev_dependency>
    ```
+7.  run tests for all supported python versions:
+   ```
+   tox
+   ```
 
 ## Development Environment Setup
 
 ### Install Dependencies
 
-- python >=3.10, <3.13
+- python >=3.8, <3.13
 - poetry: https://python-poetry.org/docs/#installation
 
 ### Create the venv
 
 ```
 poetry install
 ```
```

