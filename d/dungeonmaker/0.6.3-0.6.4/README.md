# Comparing `tmp/dungeonmaker-0.6.3.tar.gz` & `tmp/dungeonmaker-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dungeonmaker-0.6.3.tar", last modified: Fri Apr 12 17:50:07 2024, max compression
+gzip compressed data, was "dungeonmaker-0.6.4.tar", last modified: Mon May 20 17:50:23 2024, max compression
```

## Comparing `dungeonmaker-0.6.3.tar` & `dungeonmaker-0.6.4.tar`

### file list

```diff
@@ -1,38 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:50:07.962245 dungeonmaker-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-12 17:50:07.962245 dungeonmaker-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:50:07.958245 dungeonmaker-0.6.3/dungeonmaker/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/dungeonmaker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:50:07.958245 dungeonmaker-0.6.3/dungeonmaker/dm_backend/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/dungeonmaker/dm_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12200 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/dungeonmaker/dm_backend/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:50:07.958245 dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:50:07.958245 dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/database/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/database/basetypes.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/database/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/database/dba.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:50:07.962245 dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/dm/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/dm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8254 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/dm/dba.py
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/dm/dmtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/dm/dungeon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/dm/room.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/dm/selectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/dm/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/dm/user.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/dm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:50:07.962245 dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/scratchcomms/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/scratchcomms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/scratchcomms/basetypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8305 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/scratchcomms/requests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:50:07.962245 dungeonmaker-0.6.3/dungeonmaker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-12 17:50:07.000000 dungeonmaker-0.6.3/dungeonmaker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-12 17:50:07.000000 dungeonmaker-0.6.3/dungeonmaker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 17:50:07.000000 dungeonmaker-0.6.3/dungeonmaker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-12 17:50:07.000000 dungeonmaker-0.6.3/dungeonmaker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-12 17:50:07.000000 dungeonmaker-0.6.3/dungeonmaker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 17:50:07.962245 dungeonmaker-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:50:23.890358 dungeonmaker-0.6.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-20 17:50:19.000000 dungeonmaker-0.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-20 17:50:23.890358 dungeonmaker-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-20 17:50:19.000000 dungeonmaker-0.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:50:23.886358 dungeonmaker-0.6.4/dungeonmaker/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-20 17:50:19.000000 dungeonmaker-0.6.4/dungeonmaker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:50:23.886358 dungeonmaker-0.6.4/dungeonmaker/dm_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-20 17:50:19.000000 dungeonmaker-0.6.4/dungeonmaker/dm_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16842 2024-05-20 17:50:19.000000 dungeonmaker-0.6.4/dungeonmaker/dm_backend/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:50:23.886358 dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-20 17:50:19.000000 dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:50:23.886358 dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/database/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-20 17:50:19.000000 dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-20 17:50:19.000000 dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/database/basetypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-20 17:50:19.000000 dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/database/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-05-20 17:50:19.000000 dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/database/dba.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:50:23.890358 dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/dm/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-20 17:50:19.000000 dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/dm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6205 2024-05-20 17:50:19.000000 dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/dm/dba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-05-20 17:50:19.000000 dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/dm/dmtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-05-20 17:50:19.000000 dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/dm/dungeon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-20 17:50:19.000000 dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/dm/room.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-20 17:50:19.000000 dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/dm/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-05-20 17:50:19.000000 dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/dm/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-20 17:50:19.000000 dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/dm/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-20 17:50:19.000000 dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/dm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:50:23.890358 dungeonmaker-0.6.4/dungeonmaker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-20 17:50:23.000000 dungeonmaker-0.6.4/dungeonmaker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-20 17:50:23.000000 dungeonmaker-0.6.4/dungeonmaker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 17:50:23.000000 dungeonmaker-0.6.4/dungeonmaker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-20 17:50:23.000000 dungeonmaker-0.6.4/dungeonmaker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-20 17:50:23.000000 dungeonmaker-0.6.4/dungeonmaker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 17:50:23.890358 dungeonmaker-0.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-20 17:50:19.000000 dungeonmaker-0.6.4/setup.py
```

### Comparing `dungeonmaker-0.6.3/LICENSE` & `dungeonmaker-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.3/PKG-INFO` & `dungeonmaker-0.6.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dungeonmaker
-Version: 0.6.3
+Version: 0.6.4
 Summary: Dungeon maker backend and other things
 Home-page: https://github.com/thecommcraft/dungeon-maker-reinvented
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/database/basetypes.py` & `dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/database/basetypes.py`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/database/connection.py` & `dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/database/connection.py`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/database/dba.py` & `dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/database/dba.py`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/dm/dba.py` & `dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/dm/dba.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,89 +1,13 @@
 """
 Submodule for database abstractions.
 """
-from .dmtypes import UserId, DungeonId, RoomId
+from .dmtypes import UserId, DungeonId, RoomId, BaseDatabaseAbstraction
 
 
-class BaseDatabaseAbstraction:
-    """
-    Base class for database abstractions.
-    """
-    def select_user(self, user_id : UserId = None, *, fields : dict = None) -> dict:
-        """
-        Do not use.
-        """
-        raise NotImplementedError
-    
-    def select_dungeon(self, dungeon_id : DungeonId = None, *, fields : dict = None) -> dict:
-        """
-        Do not use.
-        """
-        raise NotImplementedError
-    
-    def select_room(self, room_id : RoomId = None, *, fields : dict = None) -> dict:
-        """
-        Do not use.
-        """
-        raise NotImplementedError
-    
-    def update_user(self, user_id : UserId = None, *, fields : dict = None, updator : dict = None):
-        """
-        Do not use.
-        """
-        raise NotImplementedError
-    
-    def update_dungeon(self, dungeon_id : DungeonId = None, *, fields : dict = None, updator : dict = None):
-        """
-        Do not use.
-        """
-        raise NotImplementedError
-    
-    def update_room(self, room_id : RoomId = None, *, fields : dict = None, updator : dict = None):
-        """
-        Do not use.
-        """
-        raise NotImplementedError
-    
-    def insert_user(self, *, data : dict = None):
-        """
-        Do not use.
-        """
-        raise NotImplementedError
-    
-    def insert_dungeon(self, *, data : dict = None):
-        """
-        Do not use.
-        """
-        raise NotImplementedError
-    
-    def insert_room(self, *, data : dict = None):
-        """
-        Do not use.
-        """
-        raise NotImplementedError
-    
-    def random_dungeons(self, *, amount : int = 1) -> list[dict]:
-        """
-        Do not use.
-        """
-        raise NotImplementedError
-    
-    def sorted_dungeons(
-        self, 
-        *, 
-        amount : int = 20, 
-        offset : int = 0,
-        field : str = "score", 
-        aggregation : list[dict] = [{"$addFields":{"score": {"$add": [{"$multiply": [20,{"$size": "$likers"},]},"$views"]}}}]
-    ) -> list[dict]:
-        """
-        Do not use.
-        """
-        raise NotImplementedError
     
 class DatabaseAbstractionSelector(BaseDatabaseAbstraction):
     """
     Class for selecting a database abstraction.
     """
     dbas : list[BaseDatabaseAbstraction]
```

### Comparing `dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/dm/dungeon.py` & `dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/dm/dungeon.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 """
 Submodule for dungeons.
 """
-import time, copy
+import time, copy, secrets
 from typing import Self
 from .dmtypes import (
     DungeonId, 
     BaseDungeon, 
     BaseRoom, 
     UserId, 
+    RoomId, 
     Permition, 
     BaseDungeonUser, 
     Permitions
 )
 from .room import Room
 from .user import User
 from . import room
 from . import session as _session
 from .utils import s_vars
+from .selectors import ROOM
 
 class Dungeon(BaseDungeon):
     """
     Class for dungeons.
     """
     def __init__(self, *args, **kwargs):
-        kwargs["permitions"] = kwargs.get("permitions", {})
+        kwargs.setdefault("permitions", {})
         kwargs["permitions"][kwargs["owner"]] = Permitions([
             Permition(type="read", value=True),
             Permition(type="edit_rooms", value=True),
             Permition(type="edit_infos", value=True),
             Permition(type="edit_permitions", value=True),
             Permition(type="permition_level", value=999),
         ])
@@ -77,24 +79,49 @@
             perms[:] = [{"type": perm.type, "value": perm.value} for perm in perms]
         if self.new:
             self.new = False
             self.session.database_abstraction.insert_dungeon(data=data)
             return
         self.session.database_abstraction.update_dungeon(dungeon_id=self.dungeon_id, updator={"$set": data})
         
-    def new_room(self, content : str = None) -> Room:
+    def new_room(self, *, content : str = None, room_id : RoomId = None) -> Room:
         """
         Method for creating a new room.
         """
-        new_room = Room(content=content, dungeon_id=self.dungeon_id, new=True, session=self.session)
+        new_room = self.session.create(ROOM, kwargs={"content": content, "dungeon_id": self.dungeon_id, "room_id": room_id or secrets.randbits(32)})
         self.rooms.append(new_room.room_id)
         return new_room
     
     def log_update(self):
+        """
+        Log an update.
+        """
         self.update_time = time.time()
+        
+    def like(self, user : User):
+        """
+        Register a like.
+        """
+        if user.user_id in self.likers:
+            return
+        self.likers.append(user.user_id)
+        
+    def unlike(self, user : User):
+        """
+        Register an unlike.
+        """
+        if not user.user_id in self.likers:
+            return
+        self.likers.remove(user.user_id)
+        
+    def view(self):
+        """
+        Register a view.
+        """
+        self.views += 1
 
 class DungeonUser(BaseDungeonUser):
     """
     Class for handling users in the context of a dungeon.
     """
```

### Comparing `dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/dm/room.py` & `dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/dm/room.py`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/dm/session.py` & `dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/dm/session.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,18 +8,16 @@
 from .dba import BaseDatabaseAbstraction, DatabaseAbstractionSelector
 from . import dungeon, user, room
 from .dmtypes import DungeonId, RoomId, UserId
 from .selectors import DUNGEON, ROOM, USER
 
 @dataclass
 class DMSession:
-    database_abstractions : list[BaseDatabaseAbstraction] = field(default_factory=list, kw_only=True)
-    database_abstraction : DatabaseAbstractionSelector = field(init=False)
 
-    def __init__(self, database_abstractions : list = None):
+    def __init__(self, *, database_abstractions : list = None):
         self.database_abstractions = list(database_abstractions or ())
         self.database_abstraction = DatabaseAbstractionSelector(self.database_abstractions)
 
     def add_database_abstraction(self, dba : BaseDatabaseAbstraction):
         """
         Add a database abstraction.
         """
@@ -97,15 +95,15 @@
             return dungeon.Dungeon.read(dungeon_id=id, session=self)
         if type == ROOM:
             return room.Room.read(id, session=self)
         if type == USER:
             return user.User.lookup_user(user_id=id, username=name, session=self)
         assert_never(type)
 
-    def create(self, type : Literal["dungeon", "room", "user"], *, args : Sequence = (), kwargs : Mapping = {}):
+    def create(self, type : Literal["dungeon", "room", "user"], *, args : Sequence = (), kwargs : Mapping = {}) -> Union[dungeon.Dungeon, room.Room, user.User]:
         """
         Creates something.
         """
         args = list(args)
         kwargs = dict(kwargs)
         if type == DUNGEON:
             return dungeon.Dungeon(*args, session=self, **kwargs)
```

### Comparing `dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/dm/user.py` & `dungeonmaker-0.6.4/dungeonmaker/dm_backend/modules/dm/user.py`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.3/dungeonmaker.egg-info/PKG-INFO` & `dungeonmaker-0.6.4/dungeonmaker.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dungeonmaker
-Version: 0.6.3
+Version: 0.6.4
 Summary: Dungeon maker backend and other things
 Home-page: https://github.com/thecommcraft/dungeon-maker-reinvented
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `dungeonmaker-0.6.3/setup.py` & `dungeonmaker-0.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='dungeonmaker',
-    version='0.6.3',
+    version='0.6.4',
     author='Simon Gilde',
     author_email='simon.c.gilde@gmail.com',
     description='Dungeon maker backend and other things',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/thecommcraft/dungeon-maker-reinvented',
     packages=find_packages(),
```

