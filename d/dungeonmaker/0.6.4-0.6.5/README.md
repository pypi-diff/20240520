# Comparing `tmp/dungeonmaker-0.6.4.tar.gz` & `tmp/dungeonmaker-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dungeonmaker-0.6.4.tar", last modified: Mon May 20 17:50:23 2024, max compression
+gzip compressed data, was "dungeonmaker-0.6.5.tar", last modified: Mon May 20 18:07:28 2024, max compression
```

## Comparing `dungeonmaker-0.6.4.tar` & `dungeonmaker-0.6.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:50:23.890358 dungeonmaker-0.6.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-20 17:50:19.000000 dungeonmaker-0.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-20 17:50:23.890358 dungeonmaker-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-20 17:50:19.000000 dungeonmaker-0.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:50:23.886358 dungeonmaker-0.6.4/dungeonmaker/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-20 17:50:19.000000 dungeonmaker-0.6.4/dungeonmaker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:50:23.886358 dungeonmaker-0.6.4/dungeonmaker/dm_backend/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-20 17:50:19.000000 dungeonmaker-0.6.4/dungeonmaker/dm_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16842 2024-05-20 17:50:19.000000 dungeonmaker-0.6.4/dungeonmaker/dm_backend/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:50:23.886358 dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-20 17:50:19.000000 dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:50:23.886358 dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/database/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-20 17:50:19.000000 dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-20 17:50:19.000000 dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/database/basetypes.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-20 17:50:19.000000 dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/database/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-05-20 17:50:19.000000 dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/database/dba.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:50:23.890358 dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/dm/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-20 17:50:19.000000 dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/dm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6205 2024-05-20 17:50:19.000000 dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/dm/dba.py
--rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-05-20 17:50:19.000000 dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/dm/dmtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-05-20 17:50:19.000000 dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/dm/dungeon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-20 17:50:19.000000 dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/dm/room.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-20 17:50:19.000000 dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/dm/selectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-05-20 17:50:19.000000 dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/dm/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-20 17:50:19.000000 dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/dm/user.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-20 17:50:19.000000 dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/dm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:50:23.890358 dungeonmaker-0.6.4/dungeonmaker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-20 17:50:23.000000 dungeonmaker-0.6.4/dungeonmaker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-20 17:50:23.000000 dungeonmaker-0.6.4/dungeonmaker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 17:50:23.000000 dungeonmaker-0.6.4/dungeonmaker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-20 17:50:23.000000 dungeonmaker-0.6.4/dungeonmaker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-20 17:50:23.000000 dungeonmaker-0.6.4/dungeonmaker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 17:50:23.890358 dungeonmaker-0.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-20 17:50:19.000000 dungeonmaker-0.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:07:28.903511 dungeonmaker-0.6.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-20 18:07:17.000000 dungeonmaker-0.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-20 18:07:28.903511 dungeonmaker-0.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-20 18:07:17.000000 dungeonmaker-0.6.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:07:28.899511 dungeonmaker-0.6.5/dungeonmaker/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-20 18:07:17.000000 dungeonmaker-0.6.5/dungeonmaker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:07:28.899511 dungeonmaker-0.6.5/dungeonmaker/dm_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-20 18:07:17.000000 dungeonmaker-0.6.5/dungeonmaker/dm_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16842 2024-05-20 18:07:17.000000 dungeonmaker-0.6.5/dungeonmaker/dm_backend/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:07:28.899511 dungeonmaker-0.6.5/dungeonmaker/dm_backend/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-20 18:07:17.000000 dungeonmaker-0.6.5/dungeonmaker/dm_backend/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:07:28.899511 dungeonmaker-0.6.5/dungeonmaker/dm_backend/modules/database/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-20 18:07:17.000000 dungeonmaker-0.6.5/dungeonmaker/dm_backend/modules/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-20 18:07:17.000000 dungeonmaker-0.6.5/dungeonmaker/dm_backend/modules/database/basetypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-20 18:07:17.000000 dungeonmaker-0.6.5/dungeonmaker/dm_backend/modules/database/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-05-20 18:07:17.000000 dungeonmaker-0.6.5/dungeonmaker/dm_backend/modules/database/dba.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:07:28.899511 dungeonmaker-0.6.5/dungeonmaker/dm_backend/modules/dm/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-20 18:07:17.000000 dungeonmaker-0.6.5/dungeonmaker/dm_backend/modules/dm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-05-20 18:07:17.000000 dungeonmaker-0.6.5/dungeonmaker/dm_backend/modules/dm/dba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-05-20 18:07:17.000000 dungeonmaker-0.6.5/dungeonmaker/dm_backend/modules/dm/dmtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-05-20 18:07:17.000000 dungeonmaker-0.6.5/dungeonmaker/dm_backend/modules/dm/dungeon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-20 18:07:17.000000 dungeonmaker-0.6.5/dungeonmaker/dm_backend/modules/dm/room.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-20 18:07:17.000000 dungeonmaker-0.6.5/dungeonmaker/dm_backend/modules/dm/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-05-20 18:07:17.000000 dungeonmaker-0.6.5/dungeonmaker/dm_backend/modules/dm/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-20 18:07:17.000000 dungeonmaker-0.6.5/dungeonmaker/dm_backend/modules/dm/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-20 18:07:17.000000 dungeonmaker-0.6.5/dungeonmaker/dm_backend/modules/dm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:07:28.903511 dungeonmaker-0.6.5/dungeonmaker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-20 18:07:28.000000 dungeonmaker-0.6.5/dungeonmaker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-20 18:07:28.000000 dungeonmaker-0.6.5/dungeonmaker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 18:07:28.000000 dungeonmaker-0.6.5/dungeonmaker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-20 18:07:28.000000 dungeonmaker-0.6.5/dungeonmaker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-20 18:07:28.000000 dungeonmaker-0.6.5/dungeonmaker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 18:07:28.903511 dungeonmaker-0.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-20 18:07:17.000000 dungeonmaker-0.6.5/setup.py
```

### Comparing `dungeonmaker-0.6.4/LICENSE` & `dungeonmaker-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.4/PKG-INFO` & `dungeonmaker-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dungeonmaker
-Version: 0.6.4
+Version: 0.6.5
 Summary: Dungeon maker backend and other things
 Home-page: https://github.com/thecommcraft/dungeon-maker-reinvented
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `dungeonmaker-0.6.4/dungeonmaker/dm_backend/backend.py` & `dungeonmaker-0.6.5/dungeonmaker/dm_backend/backend.py`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/database/basetypes.py` & `dungeonmaker-0.6.5/dungeonmaker/dm_backend/modules/database/basetypes.py`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/database/connection.py` & `dungeonmaker-0.6.5/dungeonmaker/dm_backend/modules/database/connection.py`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/database/dba.py` & `dungeonmaker-0.6.5/dungeonmaker/dm_backend/modules/database/dba.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 Submodule for Database Abstractions.
 """
 from typing import Literal
 from dataclasses import dataclass, field
 from .basetypes import BaseMongoDBAtlasSession
-from ..dm.dba import BaseDatabaseAbstraction
+from ..dm.dba import dba.BaseDatabaseAbstraction
 from ..dm.dmtypes import UserId, DungeonId, RoomId
 
 @dataclass(slots=True)
-class MongoDBDatabaseAbstraction(BaseDatabaseAbstraction):
+class MongoDBDatabaseAbstraction(dba.BaseDatabaseAbstraction):
     """
     Class for MongoDB database abstractions.
     """
     connection : BaseMongoDBAtlasSession = field(kw_only=True)
     
     def select_user(self, user_id : UserId = None, *, fields : dict = None) -> dict:
         """
```

### Comparing `dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/dm/dba.py` & `dungeonmaker-0.6.5/dungeonmaker/dm_backend/modules/dm/dba.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
 Submodule for database abstractions.
 """
-from .dmtypes import UserId, DungeonId, RoomId, BaseDatabaseAbstraction
+from .dmtypes import UserId, DungeonId, RoomId, dba.BaseDatabaseAbstraction
 
 
     
-class DatabaseAbstractionSelector(BaseDatabaseAbstraction):
+class DatabaseAbstractionSelector(dba.BaseDatabaseAbstraction):
     """
     Class for selecting a database abstraction.
     """
-    dbas : list[BaseDatabaseAbstraction]
+    dbas : list[dba.BaseDatabaseAbstraction]
     
-    def __init__(self, dbas : list[BaseDatabaseAbstraction]):
+    def __init__(self, dbas : list[dba.BaseDatabaseAbstraction]):
         self.dbas = dbas
         
     def select_user(self, user_id : UserId = None, *, fields : dict = None) -> dict:
         """
         Automatically selects an abstraction to select a user.
         """
         for dba in self.dbas:
```

### Comparing `dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/dm/dmtypes.py` & `dungeonmaker-0.6.5/dungeonmaker/dm_backend/modules/dm/dmtypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 Types used in the dm library
 """
 from typing import Literal, Any, Union
 from dataclasses import dataclass, field
 import secrets, time
-from . import session as _session
 
 
 
 RoomId = int
 
 DungeonId = int
 
@@ -140,15 +139,15 @@
     Base class for rooms.
     """
     room_id : RoomId = field(kw_only=True, default_factory=lambda : secrets.randbits(32))
     dungeon_id : DungeonId = field(kw_only=True)
     content : Any = field(kw_only=True, default=None)
     new : bool = field(kw_only=True, default=True)
     _id : Any = field(kw_only=True, default=None)
-    session : _session.DMSession = field(kw_only=True)
+    session : BaseDMSession = field(kw_only=True)
 
 
 
 
 @dataclass(slots=True)
 class BaseDungeon:
     """
@@ -164,15 +163,15 @@
     dungeon_id : DungeonId = field(kw_only=True, default_factory=lambda : secrets.randbits(32))
     name : str = field(kw_only=True)
     description : str = field(kw_only=True)
     creation_time : float = field(kw_only=True, default_factory=time.time)
     update_time : float = field(kw_only=True, default_factory=time.time)
     _id : Any = field(kw_only=True, default=None)
     score : Any = field(kw_only=True, default=None)
-    session : _session.DMSession = field(kw_only=True)
+    session : BaseDMSession = field(kw_only=True)
     stats : Stats = field(kw_only=True, default_factory=Stats)
     start : tuple = field(kw_only=True)
 
 
 
 
 @dataclass(slots=True)
@@ -195,24 +194,23 @@
     owned_dungeons : list[DungeonId] = field(kw_only=True, default_factory=list)
     recent_dungeons : list[DungeonId] = field(kw_only=True, default_factory=list)
     permitted_dungeons : list[DungeonId] = field(kw_only=True, default_factory=list)
     username : str = field(kw_only=True)
     admin_level : int = field(kw_only=True, default=0)
     new : bool = field(kw_only=True, default=True)
     _id : Any = field(kw_only=True, default=None)
-    session : _session.DMSession = field(kw_only=True)
+    session : BaseDMSession = field(kw_only=True)
     passdata : bytes = field(kw_only=True)
     linked_user : Union[str, None] = field(kw_only=True, default=None)
     stats : Stats = field(kw_only=True, default_factory=Stats)
 
 
 
 
 
 
 
-
```

### Comparing `dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/dm/dungeon.py` & `dungeonmaker-0.6.5/dungeonmaker/dm_backend/modules/dm/dungeon.py`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/dm/room.py` & `dungeonmaker-0.6.5/dungeonmaker/dm_backend/modules/dm/room.py`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/dm/session.py` & `dungeonmaker-0.6.5/dungeonmaker/dm_backend/modules/dm/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
 Submodule for database connection.
 """
 import random
 from typing import Literal, Union, assert_never, Sequence, Mapping
 
 from dataclasses import dataclass, field
-from .dba import BaseDatabaseAbstraction, DatabaseAbstractionSelector
 from . import dungeon, user, room
-from .dmtypes import DungeonId, RoomId, UserId
+from . import dba as _dba
+from .dmtypes import DungeonId, RoomId, UserId, BaseDatabaseAbstraction
 from .selectors import DUNGEON, ROOM, USER
 
 @dataclass
 class DMSession:
 
     def __init__(self, *, database_abstractions : list = None):
         self.database_abstractions = list(database_abstractions or ())
-        self.database_abstraction = DatabaseAbstractionSelector(self.database_abstractions)
+        self.database_abstraction = _dba.DatabaseAbstractionSelector(self.database_abstractions)
 
     def add_database_abstraction(self, dba : BaseDatabaseAbstraction):
         """
         Add a database abstraction.
         """
         assert isinstance(dba, BaseDatabaseAbstraction)
         self.database_abstractions.append(dba)
```

### Comparing `dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/dm/user.py` & `dungeonmaker-0.6.5/dungeonmaker/dm_backend/modules/dm/user.py`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.4/dungeonmaker.egg-info/PKG-INFO` & `dungeonmaker-0.6.5/dungeonmaker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dungeonmaker
-Version: 0.6.4
+Version: 0.6.5
 Summary: Dungeon maker backend and other things
 Home-page: https://github.com/thecommcraft/dungeon-maker-reinvented
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `dungeonmaker-0.6.4/dungeonmaker.egg-info/SOURCES.txt` & `dungeonmaker-0.6.5/dungeonmaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.4/setup.py` & `dungeonmaker-0.6.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='dungeonmaker',
-    version='0.6.4',
+    version='0.6.5',
     author='Simon Gilde',
     author_email='simon.c.gilde@gmail.com',
     description='Dungeon maker backend and other things',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/thecommcraft/dungeon-maker-reinvented',
     packages=find_packages(),
```

