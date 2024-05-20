# Comparing `tmp/sdkfabric_notion-0.1.0.tar.gz` & `tmp/sdkfabric_notion-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdkfabric_notion-0.1.0.tar", last modified: Sat May 18 10:28:19 2024, max compression
+gzip compressed data, was "sdkfabric_notion-0.1.2.tar", last modified: Mon May 20 06:41:48 2024, max compression
```

## Comparing `sdkfabric_notion-0.1.0.tar` & `sdkfabric_notion-0.1.2.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:28:19.706908 sdkfabric_notion-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-18 10:28:13.000000 sdkfabric_notion-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-18 10:28:19.706908 sdkfabric_notion-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-18 10:28:13.000000 sdkfabric_notion-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-18 10:28:13.000000 sdkfabric_notion-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 10:28:19.706908 sdkfabric_notion-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 10:28:13.000000 sdkfabric_notion-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:28:19.702908 sdkfabric_notion-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:28:19.702908 sdkfabric_notion-0.1.0/src/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-18 10:28:13.000000 sdkfabric_notion-0.1.0/src/sdk/block.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-18 10:28:13.000000 sdkfabric_notion-0.1.0/src/sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-18 10:28:13.000000 sdkfabric_notion-0.1.0/src/sdk/database.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-18 10:28:13.000000 sdkfabric_notion-0.1.0/src/sdk/database_annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-18 10:28:13.000000 sdkfabric_notion-0.1.0/src/sdk/database_cover.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-18 10:28:13.000000 sdkfabric_notion-0.1.0/src/sdk/database_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-18 10:28:13.000000 sdkfabric_notion-0.1.0/src/sdk/database_text.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-18 10:28:13.000000 sdkfabric_notion-0.1.0/src/sdk/database_title.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-18 10:28:13.000000 sdkfabric_notion-0.1.0/src/sdk/databases_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-18 10:28:13.000000 sdkfabric_notion-0.1.0/src/sdk/page.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-18 10:28:13.000000 sdkfabric_notion-0.1.0/src/sdk/person.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-18 10:28:13.000000 sdkfabric_notion-0.1.0/src/sdk/user.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-18 10:28:13.000000 sdkfabric_notion-0.1.0/src/sdk/user_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-18 10:28:13.000000 sdkfabric_notion-0.1.0/src/sdk/users_tag.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:28:19.706908 sdkfabric_notion-0.1.0/src/sdkfabric_notion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-18 10:28:19.000000 sdkfabric_notion-0.1.0/src/sdkfabric_notion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-18 10:28:19.000000 sdkfabric_notion-0.1.0/src/sdkfabric_notion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 10:28:19.000000 sdkfabric_notion-0.1.0/src/sdkfabric_notion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-18 10:28:19.000000 sdkfabric_notion-0.1.0/src/sdkfabric_notion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-18 10:28:19.000000 sdkfabric_notion-0.1.0/src/sdkfabric_notion.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:41:48.664296 sdkfabric_notion-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-20 06:41:42.000000 sdkfabric_notion-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-20 06:41:48.664296 sdkfabric_notion-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-20 06:41:42.000000 sdkfabric_notion-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-20 06:41:42.000000 sdkfabric_notion-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 06:41:48.664296 sdkfabric_notion-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 06:41:42.000000 sdkfabric_notion-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:41:48.660296 sdkfabric_notion-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:41:48.664296 sdkfabric_notion-0.1.2/src/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-20 06:41:42.000000 sdkfabric_notion-0.1.2/src/sdk/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-20 06:41:42.000000 sdkfabric_notion-0.1.2/src/sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-20 06:41:42.000000 sdkfabric_notion-0.1.2/src/sdk/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-20 06:41:42.000000 sdkfabric_notion-0.1.2/src/sdk/database_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-20 06:41:42.000000 sdkfabric_notion-0.1.2/src/sdk/database_cover.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-20 06:41:42.000000 sdkfabric_notion-0.1.2/src/sdk/database_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-20 06:41:42.000000 sdkfabric_notion-0.1.2/src/sdk/database_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-20 06:41:42.000000 sdkfabric_notion-0.1.2/src/sdk/database_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-20 06:41:42.000000 sdkfabric_notion-0.1.2/src/sdk/database_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-20 06:41:42.000000 sdkfabric_notion-0.1.2/src/sdk/database_title.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-20 06:41:42.000000 sdkfabric_notion-0.1.2/src/sdk/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-20 06:41:42.000000 sdkfabric_notion-0.1.2/src/sdk/page_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-20 06:41:42.000000 sdkfabric_notion-0.1.2/src/sdk/page_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-20 06:41:42.000000 sdkfabric_notion-0.1.2/src/sdk/person.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-20 06:41:42.000000 sdkfabric_notion-0.1.2/src/sdk/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-20 06:41:42.000000 sdkfabric_notion-0.1.2/src/sdk/user_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-20 06:41:42.000000 sdkfabric_notion-0.1.2/src/sdk/user_tag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:41:48.664296 sdkfabric_notion-0.1.2/src/sdkfabric_notion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-20 06:41:48.000000 sdkfabric_notion-0.1.2/src/sdkfabric_notion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-20 06:41:48.000000 sdkfabric_notion-0.1.2/src/sdkfabric_notion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 06:41:48.000000 sdkfabric_notion-0.1.2/src/sdkfabric_notion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-20 06:41:48.000000 sdkfabric_notion-0.1.2/src/sdkfabric_notion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-20 06:41:48.000000 sdkfabric_notion-0.1.2/src/sdkfabric_notion.egg-info/top_level.txt
```

### Comparing `sdkfabric_notion-0.1.0/LICENSE` & `sdkfabric_notion-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sdkfabric_notion-0.1.0/PKG-INFO` & `sdkfabric_notion-0.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkfabric-notion
-Version: 0.1.0
+Version: 0.1.2
 Summary: Notion Python SDK managed by SDK Fabric
 Author-email: Christoph Kappestein <christoph.kappestein@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/sdk-fabric/notion-python
 Project-URL: Issues, https://github.com/sdk-fabric/notion-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -29,15 +29,19 @@
 please register at the [TypeHub](https://typehub.cloud/) platform and create
 a pull request at the [Notion](https://app.typehub.cloud/d/sdkfabric/notion)
 specification. The system will then automatically create a GIT commit and update
 the code.
 
 ## Usage
 
-The following example shows how you can use the client:
+The following example shows how you initialize the client:
 
 ```python
-const credentials = new HttpBearer('[access_token]');
-const client = Client::build(credentials);
+from sdk.client import Client
+
+client = Client.build("[access_token]")
 
 // @TODO use the client
 ```
+
+You can find all available operations and types at:
+https://app.typehub.cloud/d/sdkfabric/notion
```

### Comparing `sdkfabric_notion-0.1.0/pyproject.toml` & `sdkfabric_notion-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sdkfabric-notion"
-version = "0.1.0"
+version = "0.1.2"
 authors = [
   { name="Christoph Kappestein", email="christoph.kappestein@gmail.com" },
 ]
 description = "Notion Python SDK managed by SDK Fabric"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
```

### Comparing `sdkfabric_notion-0.1.0/src/sdk/block.py` & `sdkfabric_notion-0.1.2/src/sdk/block.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_notion-0.1.0/src/sdk/client.py` & `sdkfabric_notion-0.1.2/src/sdk/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,29 +4,36 @@
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 from typing import List
 
-from .users_tag import UsersTag
-from .databases_tag import DatabasesTag
+from .user_tag import UserTag
+from .database_tag import DatabaseTag
+from .page_tag import PageTag
 
 class Client(sdkgen.ClientAbstract):
     def __init__(self, base_url: str, credentials: sdkgen.CredentialsInterface):
         super().__init__(base_url, credentials)
 
-    def users(self) -> UsersTag:
-        return UsersTag(
+    def user(self) -> UserTag:
+        return UserTag(
             self.http_client,
             self.parser
         )
 
-    def databases(self) -> DatabasesTag:
-        return DatabasesTag(
+    def database(self) -> DatabaseTag:
+        return DatabaseTag(
+            self.http_client,
+            self.parser
+        )
+
+    def page(self) -> PageTag:
+        return PageTag(
             self.http_client,
             self.parser
         )
 
 
 
     @staticmethod
```

### Comparing `sdkfabric_notion-0.1.0/src/sdk/database.py` & `sdkfabric_notion-0.1.2/src/sdk/database.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_notion-0.1.0/src/sdk/database_annotations.py` & `sdkfabric_notion-0.1.2/src/sdk/database_annotations.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_notion-0.1.0/src/sdk/database_title.py` & `sdkfabric_notion-0.1.2/src/sdk/database_title.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_notion-0.1.0/src/sdk/databases_tag.py` & `sdkfabric_notion-0.1.2/src/sdk/database_tag.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
-DatabasesTag automatically generated by SDKgen please do not edit this file manually
+DatabaseTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 from typing import List
 
 from .database import Database
 
-class DatabasesTag(sdkgen.TagAbstract):
+class DatabaseTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
 
     def get(self, database_id: str) -> Database:
         try:
             path_params = {}
```

### Comparing `sdkfabric_notion-0.1.0/src/sdk/page.py` & `sdkfabric_notion-0.1.2/src/sdk/page.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,24 @@
 """
 
 from pydantic import BaseModel, Field, GetCoreSchemaHandler
 from pydantic_core import CoreSchema, core_schema
 from typing import Any, Dict, Generic, List, Optional, TypeVar, Union
 import datetime
 from .user import User
+from .database_id import DatabaseId
+from .page_id import PageId
 class Page(BaseModel):
     object: Optional[str] = Field(default=None, alias="object")
     id: Optional[str] = Field(default=None, alias="id")
     created_time: Optional[datetime.datetime] = Field(default=None, alias="created_time")
     last_edited_time: Optional[datetime.datetime] = Field(default=None, alias="last_edited_time")
     created_by: Optional[User] = Field(default=None, alias="created_by")
     last_edited_by: Optional[User] = Field(default=None, alias="last_edited_by")
     cover: Optional[str] = Field(default=None, alias="cover")
     icon: Optional[str] = Field(default=None, alias="icon")
-    parent: Optional[str] = Field(default=None, alias="parent")
+    parent: Optional[Union[DatabaseId, PageId]] = Field(default=None, alias="parent")
     in_trash: Optional[bool] = Field(default=None, alias="in_trash")
     properties: Optional[Dict[str, Any]] = Field(default=None, alias="properties")
+    url: Optional[str] = Field(default=None, alias="url")
+    public_url: Optional[str] = Field(default=None, alias="public_url")
     pass
```

### Comparing `sdkfabric_notion-0.1.0/src/sdk/user.py` & `sdkfabric_notion-0.1.2/src/sdk/user.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_notion-0.1.0/src/sdk/user_collection.py` & `sdkfabric_notion-0.1.2/src/sdk/user_collection.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_notion-0.1.0/src/sdk/users_tag.py` & `sdkfabric_notion-0.1.2/src/sdk/user_tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
-UsersTag automatically generated by SDKgen please do not edit this file manually
+UserTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 from typing import List
 
 from .user import User
 from .user_collection import UserCollection
 
-class UsersTag(sdkgen.TagAbstract):
+class UserTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
 
     def get_all(self, start_cursor: str, page_size: int) -> UserCollection:
         """
         Returns a paginated list of Users for the workspace. The response may contain fewer than page_size of results.
```

### Comparing `sdkfabric_notion-0.1.0/src/sdkfabric_notion.egg-info/PKG-INFO` & `sdkfabric_notion-0.1.2/src/sdkfabric_notion.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkfabric-notion
-Version: 0.1.0
+Version: 0.1.2
 Summary: Notion Python SDK managed by SDK Fabric
 Author-email: Christoph Kappestein <christoph.kappestein@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/sdk-fabric/notion-python
 Project-URL: Issues, https://github.com/sdk-fabric/notion-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -29,15 +29,19 @@
 please register at the [TypeHub](https://typehub.cloud/) platform and create
 a pull request at the [Notion](https://app.typehub.cloud/d/sdkfabric/notion)
 specification. The system will then automatically create a GIT commit and update
 the code.
 
 ## Usage
 
-The following example shows how you can use the client:
+The following example shows how you initialize the client:
 
 ```python
-const credentials = new HttpBearer('[access_token]');
-const client = Client::build(credentials);
+from sdk.client import Client
+
+client = Client.build("[access_token]")
 
 // @TODO use the client
 ```
+
+You can find all available operations and types at:
+https://app.typehub.cloud/d/sdkfabric/notion
```

