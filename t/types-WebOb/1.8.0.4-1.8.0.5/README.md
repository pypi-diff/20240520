# Comparing `tmp/types-WebOb-1.8.0.4.tar.gz` & `tmp/types-WebOb-1.8.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-WebOb-1.8.0.4.tar", last modified: Sat Nov 11 02:45:51 2023, max compression
+gzip compressed data, was "types-WebOb-1.8.0.5.tar", last modified: Fri Nov 24 02:18:15 2023, max compression
```

## Comparing `types-WebOb-1.8.0.4.tar` & `types-WebOb-1.8.0.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-11 02:45:51.441253 types-WebOb-1.8.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2023-11-11 02:45:50.000000 types-WebOb-1.8.0.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-11-11 02:45:50.000000 types-WebOb-1.8.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2023-11-11 02:45:51.441253 types-WebOb-1.8.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-11 02:45:51.441253 types-WebOb-1.8.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2023-11-11 02:45:50.000000 types-WebOb-1.8.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-11 02:45:51.437253 types-WebOb-1.8.0.4/types_WebOb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2023-11-11 02:45:51.000000 types-WebOb-1.8.0.4/types_WebOb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      617 2023-11-11 02:45:51.000000 types-WebOb-1.8.0.4/types_WebOb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-11 02:45:51.000000 types-WebOb-1.8.0.4/types_WebOb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-11-11 02:45:51.000000 types-WebOb-1.8.0.4/types_WebOb.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-11 02:45:51.441253 types-WebOb-1.8.0.4/webob-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-11-11 02:45:50.000000 types-WebOb-1.8.0.4/webob-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)      362 2023-11-11 02:45:29.000000 types-WebOb-1.8.0.4/webob-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    21980 2023-11-11 02:45:29.000000 types-WebOb-1.8.0.4/webob-stubs/acceptparse.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      951 2023-11-11 02:45:29.000000 types-WebOb-1.8.0.4/webob-stubs/byterange.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2023-11-11 02:45:29.000000 types-WebOb-1.8.0.4/webob-stubs/cachecontrol.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      519 2023-11-11 02:45:29.000000 types-WebOb-1.8.0.4/webob-stubs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6702 2023-11-11 02:45:29.000000 types-WebOb-1.8.0.4/webob-stubs/cookies.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      629 2023-11-11 02:45:29.000000 types-WebOb-1.8.0.4/webob-stubs/datetime_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2023-11-11 02:45:29.000000 types-WebOb-1.8.0.4/webob-stubs/dec.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2023-11-11 02:45:29.000000 types-WebOb-1.8.0.4/webob-stubs/descriptors.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2023-11-11 02:45:29.000000 types-WebOb-1.8.0.4/webob-stubs/etag.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4939 2023-11-11 02:45:29.000000 types-WebOb-1.8.0.4/webob-stubs/exc.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      684 2023-11-11 02:45:29.000000 types-WebOb-1.8.0.4/webob-stubs/headers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4504 2023-11-11 02:45:29.000000 types-WebOb-1.8.0.4/webob-stubs/multidict.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8774 2023-11-11 02:45:29.000000 types-WebOb-1.8.0.4/webob-stubs/request.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6578 2023-11-11 02:45:29.000000 types-WebOb-1.8.0.4/webob-stubs/response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2023-11-11 02:45:29.000000 types-WebOb-1.8.0.4/webob-stubs/static.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      493 2023-11-11 02:45:29.000000 types-WebOb-1.8.0.4/webob-stubs/util.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 02:18:15.224090 types-WebOb-1.8.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2023-11-24 02:18:14.000000 types-WebOb-1.8.0.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2023-11-24 02:18:14.000000 types-WebOb-1.8.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2023-11-24 02:18:15.224090 types-WebOb-1.8.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-24 02:18:15.228090 types-WebOb-1.8.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2023-11-24 02:18:14.000000 types-WebOb-1.8.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 02:18:15.224090 types-WebOb-1.8.0.5/types_WebOb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2023-11-24 02:18:15.000000 types-WebOb-1.8.0.5/types_WebOb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2023-11-24 02:18:15.000000 types-WebOb-1.8.0.5/types_WebOb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-24 02:18:15.000000 types-WebOb-1.8.0.5/types_WebOb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2023-11-24 02:18:15.000000 types-WebOb-1.8.0.5/types_WebOb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 02:18:15.224090 types-WebOb-1.8.0.5/webob-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2023-11-24 02:18:14.000000 types-WebOb-1.8.0.5/webob-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2023-11-24 02:17:58.000000 types-WebOb-1.8.0.5/webob-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    21980 2023-11-24 02:17:58.000000 types-WebOb-1.8.0.5/webob-stubs/acceptparse.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2023-11-24 02:17:58.000000 types-WebOb-1.8.0.5/webob-stubs/byterange.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2023-11-24 02:17:58.000000 types-WebOb-1.8.0.5/webob-stubs/cachecontrol.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2023-11-24 02:17:58.000000 types-WebOb-1.8.0.5/webob-stubs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6703 2023-11-24 02:17:58.000000 types-WebOb-1.8.0.5/webob-stubs/cookies.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2023-11-24 02:17:58.000000 types-WebOb-1.8.0.5/webob-stubs/datetime_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2023-11-24 02:17:58.000000 types-WebOb-1.8.0.5/webob-stubs/dec.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2023-11-24 02:17:58.000000 types-WebOb-1.8.0.5/webob-stubs/descriptors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2023-11-24 02:17:58.000000 types-WebOb-1.8.0.5/webob-stubs/etag.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4939 2023-11-24 02:17:58.000000 types-WebOb-1.8.0.5/webob-stubs/exc.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2023-11-24 02:17:58.000000 types-WebOb-1.8.0.5/webob-stubs/headers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2023-11-24 02:17:58.000000 types-WebOb-1.8.0.5/webob-stubs/multidict.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8774 2023-11-24 02:17:58.000000 types-WebOb-1.8.0.5/webob-stubs/request.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6578 2023-11-24 02:17:58.000000 types-WebOb-1.8.0.5/webob-stubs/response.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2023-11-24 02:17:58.000000 types-WebOb-1.8.0.5/webob-stubs/static.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2023-11-24 02:17:58.000000 types-WebOb-1.8.0.5/webob-stubs/util.pyi
```

### Comparing `types-WebOb-1.8.0.4/PKG-INFO` & `types-WebOb-1.8.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-WebOb
-Version: 1.8.0.4
+Version: 1.8.0.5
 Summary: Typing stubs for WebOb
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/WebOb.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-WebOb` aims to provide accurate annotations
 for `WebOb==1.8.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/WebOb. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `571cc6d77ad85c6b3c12f546f8b62c69f37da402` and was tested
-with mypy 1.7.0, pyright 1.1.334, and
-pytype 2023.10.17.
+This package was generated from typeshed commit `81633e27097228a8a7eb0f963c62916ecea78abc` and was tested
+with mypy 1.7.1, pyright 1.1.334, and
+pytype 2023.11.21.
```

### Comparing `types-WebOb-1.8.0.4/setup.py` & `types-WebOb-1.8.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 This version of `types-WebOb` aims to provide accurate annotations
 for `WebOb==1.8.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/WebOb. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `571cc6d77ad85c6b3c12f546f8b62c69f37da402` and was tested
-with mypy 1.7.0, pyright 1.1.334, and
-pytype 2023.10.17.
+This package was generated from typeshed commit `81633e27097228a8a7eb0f963c62916ecea78abc` and was tested
+with mypy 1.7.1, pyright 1.1.334, and
+pytype 2023.11.21.
 '''.lstrip()
 
 setup(name=name,
-      version="1.8.0.4",
+      version="1.8.0.5",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/WebOb.md",
```

### Comparing `types-WebOb-1.8.0.4/types_WebOb.egg-info/PKG-INFO` & `types-WebOb-1.8.0.5/types_WebOb.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-WebOb
-Version: 1.8.0.4
+Version: 1.8.0.5
 Summary: Typing stubs for WebOb
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/WebOb.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-WebOb` aims to provide accurate annotations
 for `WebOb==1.8.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/WebOb. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `571cc6d77ad85c6b3c12f546f8b62c69f37da402` and was tested
-with mypy 1.7.0, pyright 1.1.334, and
-pytype 2023.10.17.
+This package was generated from typeshed commit `81633e27097228a8a7eb0f963c62916ecea78abc` and was tested
+with mypy 1.7.1, pyright 1.1.334, and
+pytype 2023.11.21.
```

### Comparing `types-WebOb-1.8.0.4/types_WebOb.egg-info/SOURCES.txt` & `types-WebOb-1.8.0.5/types_WebOb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `types-WebOb-1.8.0.4/webob-stubs/acceptparse.pyi` & `types-WebOb-1.8.0.5/webob-stubs/acceptparse.pyi`

 * *Files identical despite different names*

### Comparing `types-WebOb-1.8.0.4/webob-stubs/byterange.pyi` & `types-WebOb-1.8.0.5/webob-stubs/byterange.pyi`

 * *Files identical despite different names*

### Comparing `types-WebOb-1.8.0.4/webob-stubs/cachecontrol.pyi` & `types-WebOb-1.8.0.5/webob-stubs/cachecontrol.pyi`

 * *Files identical despite different names*

### Comparing `types-WebOb-1.8.0.4/webob-stubs/client.pyi` & `types-WebOb-1.8.0.5/webob-stubs/client.pyi`

 * *Files identical despite different names*

### Comparing `types-WebOb-1.8.0.4/webob-stubs/cookies.pyi` & `types-WebOb-1.8.0.5/webob-stubs/cookies.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from webob.descriptors import _AsymmetricProperty
 from webob.request import Request
 from webob.response import Response
 
 _T = TypeVar("_T")
 # we accept both the official spelling and the one used in the WebOb docs
 # the implementation compares after lower() so technically there are more
-# valid spellings, but it seems mor natural to support these two spellings
+# valid spellings, but it seems more natural to support these two spellings
 _SameSitePolicy: TypeAlias = Literal["Strict", "Lax", "None", "strict", "lax", "none"]
 
 class _Serializer(Protocol):
     def loads(self, __appstruct: Any) -> bytes: ...
     def dumps(self, __bstruct: bytes) -> Any: ...
 
 class RequestCookies(MutableMapping[str, str]):
```

### Comparing `types-WebOb-1.8.0.4/webob-stubs/datetime_utils.pyi` & `types-WebOb-1.8.0.5/webob-stubs/datetime_utils.pyi`

 * *Files identical despite different names*

### Comparing `types-WebOb-1.8.0.4/webob-stubs/dec.pyi` & `types-WebOb-1.8.0.5/webob-stubs/dec.pyi`

 * *Files identical despite different names*

### Comparing `types-WebOb-1.8.0.4/webob-stubs/descriptors.pyi` & `types-WebOb-1.8.0.5/webob-stubs/descriptors.pyi`

 * *Files identical despite different names*

### Comparing `types-WebOb-1.8.0.4/webob-stubs/etag.pyi` & `types-WebOb-1.8.0.5/webob-stubs/etag.pyi`

 * *Files identical despite different names*

### Comparing `types-WebOb-1.8.0.4/webob-stubs/exc.pyi` & `types-WebOb-1.8.0.5/webob-stubs/exc.pyi`

 * *Files identical despite different names*

### Comparing `types-WebOb-1.8.0.4/webob-stubs/headers.pyi` & `types-WebOb-1.8.0.5/webob-stubs/headers.pyi`

 * *Files identical despite different names*

### Comparing `types-WebOb-1.8.0.4/webob-stubs/multidict.pyi` & `types-WebOb-1.8.0.5/webob-stubs/multidict.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     def dict_of_lists(self) -> dict[_KT, list[_VT]]: ...
     def __delitem__(self, key: _KT) -> None: ...
     def __contains__(self, key: object) -> bool: ...
     has_key = __contains__
     def clear(self) -> None: ...
     def copy(self) -> Self: ...
     @overload
-    def setdefault(self, key: _KT, default: None = None) -> _VT | None: ...  # type:ignore[misc]
+    def setdefault(self, key: _KT, default: None = None) -> _VT | None: ...
     @overload
     def setdefault(self, key: _KT, default: _VT) -> _VT: ...
     @overload
     def pop(self, key: _KT) -> _VT: ...
     @overload
     def pop(self, key: _KT, default: _T) -> _VT | _T: ...
     def popitem(self) -> tuple[_KT, _VT]: ...
```

### Comparing `types-WebOb-1.8.0.4/webob-stubs/request.pyi` & `types-WebOb-1.8.0.5/webob-stubs/request.pyi`

 * *Files identical despite different names*

### Comparing `types-WebOb-1.8.0.4/webob-stubs/response.pyi` & `types-WebOb-1.8.0.5/webob-stubs/response.pyi`

 * *Files identical despite different names*

### Comparing `types-WebOb-1.8.0.4/webob-stubs/static.pyi` & `types-WebOb-1.8.0.5/webob-stubs/static.pyi`

 * *Files identical despite different names*

