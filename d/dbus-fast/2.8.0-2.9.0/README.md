# Comparing `tmp/dbus_fast-2.8.0.tar.gz` & `tmp/dbus_fast-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbus_fast-2.8.0.tar", max compression
+gzip compressed data, was "dbus_fast-2.9.0.tar", max compression
```

## Comparing `dbus_fast-2.8.0.tar` & `dbus_fast-2.9.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1083 2023-09-20 08:31:00.445248 dbus_fast-2.8.0/LICENSE
--rw-r--r--   0        0        0     9404 2023-09-20 08:31:00.445248 dbus_fast-2.8.0/README.md
--rw-r--r--   0        0        0     1313 2023-09-20 08:31:00.445248 dbus_fast-2.8.0/build_ext.py
--rw-r--r--   0        0        0     2551 2023-09-20 08:31:01.493252 dbus_fast-2.8.0/pyproject.toml
--rw-r--r--   0        0        0     1948 2023-09-20 08:31:00.449248 dbus_fast-2.8.0/src/dbus_fast/__init__.py
--rw-r--r--   0        0        0      400 2023-09-20 08:31:01.461252 dbus_fast-2.8.0/src/dbus_fast/__version__.py
--rw-r--r--   0        0        0        0 2023-09-20 08:31:00.449248 dbus_fast-2.8.0/src/dbus_fast/_private/__init__.py
--rw-r--r--   0        0        0      211 2023-09-20 08:31:00.449248 dbus_fast-2.8.0/src/dbus_fast/_private/_cython_compat.py
--rw-r--r--   0        0        0      287 2023-09-20 08:31:00.449248 dbus_fast-2.8.0/src/dbus_fast/_private/address.pxd
--rw-r--r--   0        0        0     4024 2023-09-20 08:31:00.449248 dbus_fast-2.8.0/src/dbus_fast/_private/address.py
--rw-r--r--   0        0        0      275 2023-09-20 08:31:00.449248 dbus_fast-2.8.0/src/dbus_fast/_private/constants.py
--rw-r--r--   0        0        0     2463 2023-09-20 08:31:00.449248 dbus_fast-2.8.0/src/dbus_fast/_private/marshaller.pxd
--rw-r--r--   0        0        0     7785 2023-09-20 08:31:00.449248 dbus_fast-2.8.0/src/dbus_fast/_private/marshaller.py
--rw-r--r--   0        0        0     6146 2023-09-20 08:31:00.449248 dbus_fast-2.8.0/src/dbus_fast/_private/unmarshaller.pxd
--rw-r--r--   0        0        0    29016 2023-09-20 08:31:00.449248 dbus_fast-2.8.0/src/dbus_fast/_private/unmarshaller.py
--rw-r--r--   0        0        0     5660 2023-09-20 08:31:00.449248 dbus_fast-2.8.0/src/dbus_fast/_private/util.py
--rw-r--r--   0        0        0       90 2023-09-20 08:31:00.449248 dbus_fast-2.8.0/src/dbus_fast/aio/__init__.py
--rw-r--r--   0        0        0    19831 2023-09-20 08:31:00.449248 dbus_fast-2.8.0/src/dbus_fast/aio/message_bus.py
--rw-r--r--   0        0        0      100 2023-09-20 08:31:00.449248 dbus_fast-2.8.0/src/dbus_fast/aio/message_reader.pxd
--rw-r--r--   0        0        0     1498 2023-09-20 08:31:00.449248 dbus_fast-2.8.0/src/dbus_fast/aio/message_reader.py
--rw-r--r--   0        0        0     7045 2023-09-20 08:31:00.449248 dbus_fast-2.8.0/src/dbus_fast/aio/proxy_object.py
--rw-r--r--   0        0        0     4408 2023-09-20 08:31:00.449248 dbus_fast-2.8.0/src/dbus_fast/auth.py
--rw-r--r--   0        0        0     5490 2023-09-20 08:31:00.449248 dbus_fast-2.8.0/src/dbus_fast/constants.py
--rw-r--r--   0        0        0     1982 2023-09-20 08:31:00.449248 dbus_fast-2.8.0/src/dbus_fast/errors.py
--rw-r--r--   0        0        0       90 2023-09-20 08:31:00.449248 dbus_fast-2.8.0/src/dbus_fast/glib/__init__.py
--rw-r--r--   0        0        0    16397 2023-09-20 08:31:00.449248 dbus_fast-2.8.0/src/dbus_fast/glib/message_bus.py
--rw-r--r--   0        0        0    10724 2023-09-20 08:31:00.449248 dbus_fast-2.8.0/src/dbus_fast/glib/proxy_object.py
--rw-r--r--   0        0        0    22597 2023-09-20 08:31:00.449248 dbus_fast-2.8.0/src/dbus_fast/introspection.py
--rw-r--r--   0        0        0       53 2023-09-20 08:31:00.449248 dbus_fast-2.8.0/src/dbus_fast/main.py
--rw-r--r--   0        0        0     1287 2023-09-20 08:31:00.449248 dbus_fast-2.8.0/src/dbus_fast/message.pxd
--rw-r--r--   0        0        0    12432 2023-09-20 08:31:00.449248 dbus_fast-2.8.0/src/dbus_fast/message.py
--rw-r--r--   0        0        0     1524 2023-09-20 08:31:00.449248 dbus_fast-2.8.0/src/dbus_fast/message_bus.pxd
--rw-r--r--   0        0        0    47135 2023-09-20 08:31:00.449248 dbus_fast-2.8.0/src/dbus_fast/message_bus.py
--rw-r--r--   0        0        0    14103 2023-09-20 08:31:00.449248 dbus_fast-2.8.0/src/dbus_fast/proxy_object.py
--rw-r--r--   0        0        0        0 2023-09-20 08:31:00.449248 dbus_fast-2.8.0/src/dbus_fast/py.typed
--rw-r--r--   0        0        0     1637 2023-09-20 08:31:00.453248 dbus_fast-2.8.0/src/dbus_fast/send_reply.py
--rw-r--r--   0        0        0      565 2023-09-20 08:31:00.453248 dbus_fast-2.8.0/src/dbus_fast/service.pxd
--rw-r--r--   0        0        0    22232 2023-09-20 08:31:00.453248 dbus_fast-2.8.0/src/dbus_fast/service.py
--rw-r--r--   0        0        0      352 2023-09-20 08:31:00.453248 dbus_fast-2.8.0/src/dbus_fast/signature.pxd
--rw-r--r--   0        0        0    16502 2023-09-20 08:31:00.453248 dbus_fast-2.8.0/src/dbus_fast/signature.py
--rw-r--r--   0        0        0      181 2023-09-20 08:31:00.453248 dbus_fast-2.8.0/src/dbus_fast/unpack.pxd
--rw-r--r--   0        0        0      622 2023-09-20 08:31:00.453248 dbus_fast-2.8.0/src/dbus_fast/unpack.py
--rw-r--r--   0        0        0     5239 2023-09-20 08:31:00.453248 dbus_fast-2.8.0/src/dbus_fast/validators.py
--rw-r--r--   0        0        0    10449 1970-01-01 00:00:00.000000 dbus_fast-2.8.0/setup.py
--rw-r--r--   0        0        0    10606 1970-01-01 00:00:00.000000 dbus_fast-2.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-09-20 09:18:55.771577 dbus_fast-2.9.0/LICENSE
+-rw-r--r--   0        0        0     9404 2023-09-20 09:18:55.771577 dbus_fast-2.9.0/README.md
+-rw-r--r--   0        0        0     1313 2023-09-20 09:18:55.771577 dbus_fast-2.9.0/build_ext.py
+-rw-r--r--   0        0        0     2551 2023-09-20 09:18:56.659573 dbus_fast-2.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1948 2023-09-20 09:18:55.775577 dbus_fast-2.9.0/src/dbus_fast/__init__.py
+-rw-r--r--   0        0        0      400 2023-09-20 09:18:56.627574 dbus_fast-2.9.0/src/dbus_fast/__version__.py
+-rw-r--r--   0        0        0        0 2023-09-20 09:18:55.775577 dbus_fast-2.9.0/src/dbus_fast/_private/__init__.py
+-rw-r--r--   0        0        0      211 2023-09-20 09:18:55.775577 dbus_fast-2.9.0/src/dbus_fast/_private/_cython_compat.py
+-rw-r--r--   0        0        0      287 2023-09-20 09:18:55.775577 dbus_fast-2.9.0/src/dbus_fast/_private/address.pxd
+-rw-r--r--   0        0        0     4024 2023-09-20 09:18:55.775577 dbus_fast-2.9.0/src/dbus_fast/_private/address.py
+-rw-r--r--   0        0        0      275 2023-09-20 09:18:55.775577 dbus_fast-2.9.0/src/dbus_fast/_private/constants.py
+-rw-r--r--   0        0        0     2463 2023-09-20 09:18:55.775577 dbus_fast-2.9.0/src/dbus_fast/_private/marshaller.pxd
+-rw-r--r--   0        0        0     7785 2023-09-20 09:18:55.775577 dbus_fast-2.9.0/src/dbus_fast/_private/marshaller.py
+-rw-r--r--   0        0        0     6211 2023-09-20 09:18:55.775577 dbus_fast-2.9.0/src/dbus_fast/_private/unmarshaller.pxd
+-rw-r--r--   0        0        0    29620 2023-09-20 09:18:55.775577 dbus_fast-2.9.0/src/dbus_fast/_private/unmarshaller.py
+-rw-r--r--   0        0        0     5660 2023-09-20 09:18:55.775577 dbus_fast-2.9.0/src/dbus_fast/_private/util.py
+-rw-r--r--   0        0        0       90 2023-09-20 09:18:55.775577 dbus_fast-2.9.0/src/dbus_fast/aio/__init__.py
+-rw-r--r--   0        0        0    19831 2023-09-20 09:18:55.775577 dbus_fast-2.9.0/src/dbus_fast/aio/message_bus.py
+-rw-r--r--   0        0        0      100 2023-09-20 09:18:55.775577 dbus_fast-2.9.0/src/dbus_fast/aio/message_reader.pxd
+-rw-r--r--   0        0        0     1498 2023-09-20 09:18:55.775577 dbus_fast-2.9.0/src/dbus_fast/aio/message_reader.py
+-rw-r--r--   0        0        0     7045 2023-09-20 09:18:55.775577 dbus_fast-2.9.0/src/dbus_fast/aio/proxy_object.py
+-rw-r--r--   0        0        0     4408 2023-09-20 09:18:55.775577 dbus_fast-2.9.0/src/dbus_fast/auth.py
+-rw-r--r--   0        0        0     5490 2023-09-20 09:18:55.775577 dbus_fast-2.9.0/src/dbus_fast/constants.py
+-rw-r--r--   0        0        0     1982 2023-09-20 09:18:55.775577 dbus_fast-2.9.0/src/dbus_fast/errors.py
+-rw-r--r--   0        0        0       90 2023-09-20 09:18:55.775577 dbus_fast-2.9.0/src/dbus_fast/glib/__init__.py
+-rw-r--r--   0        0        0    16397 2023-09-20 09:18:55.775577 dbus_fast-2.9.0/src/dbus_fast/glib/message_bus.py
+-rw-r--r--   0        0        0    10724 2023-09-20 09:18:55.775577 dbus_fast-2.9.0/src/dbus_fast/glib/proxy_object.py
+-rw-r--r--   0        0        0    22597 2023-09-20 09:18:55.775577 dbus_fast-2.9.0/src/dbus_fast/introspection.py
+-rw-r--r--   0        0        0       53 2023-09-20 09:18:55.775577 dbus_fast-2.9.0/src/dbus_fast/main.py
+-rw-r--r--   0        0        0     1287 2023-09-20 09:18:55.775577 dbus_fast-2.9.0/src/dbus_fast/message.pxd
+-rw-r--r--   0        0        0    12432 2023-09-20 09:18:55.775577 dbus_fast-2.9.0/src/dbus_fast/message.py
+-rw-r--r--   0        0        0     1524 2023-09-20 09:18:55.775577 dbus_fast-2.9.0/src/dbus_fast/message_bus.pxd
+-rw-r--r--   0        0        0    47135 2023-09-20 09:18:55.775577 dbus_fast-2.9.0/src/dbus_fast/message_bus.py
+-rw-r--r--   0        0        0    14103 2023-09-20 09:18:55.775577 dbus_fast-2.9.0/src/dbus_fast/proxy_object.py
+-rw-r--r--   0        0        0        0 2023-09-20 09:18:55.775577 dbus_fast-2.9.0/src/dbus_fast/py.typed
+-rw-r--r--   0        0        0     1637 2023-09-20 09:18:55.775577 dbus_fast-2.9.0/src/dbus_fast/send_reply.py
+-rw-r--r--   0        0        0      565 2023-09-20 09:18:55.775577 dbus_fast-2.9.0/src/dbus_fast/service.pxd
+-rw-r--r--   0        0        0    22232 2023-09-20 09:18:55.779577 dbus_fast-2.9.0/src/dbus_fast/service.py
+-rw-r--r--   0        0        0      352 2023-09-20 09:18:55.779577 dbus_fast-2.9.0/src/dbus_fast/signature.pxd
+-rw-r--r--   0        0        0    16502 2023-09-20 09:18:55.779577 dbus_fast-2.9.0/src/dbus_fast/signature.py
+-rw-r--r--   0        0        0      181 2023-09-20 09:18:55.779577 dbus_fast-2.9.0/src/dbus_fast/unpack.pxd
+-rw-r--r--   0        0        0      622 2023-09-20 09:18:55.779577 dbus_fast-2.9.0/src/dbus_fast/unpack.py
+-rw-r--r--   0        0        0     5239 2023-09-20 09:18:55.779577 dbus_fast-2.9.0/src/dbus_fast/validators.py
+-rw-r--r--   0        0        0    10449 1970-01-01 00:00:00.000000 dbus_fast-2.9.0/setup.py
+-rw-r--r--   0        0        0    10606 1970-01-01 00:00:00.000000 dbus_fast-2.9.0/PKG-INFO
```

### Comparing `dbus_fast-2.8.0/LICENSE` & `dbus_fast-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbus_fast-2.8.0/README.md` & `dbus_fast-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `dbus_fast-2.8.0/build_ext.py` & `dbus_fast-2.9.0/build_ext.py`

 * *Files identical despite different names*

### Comparing `dbus_fast-2.8.0/pyproject.toml` & `dbus_fast-2.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbus-fast"
-version = "2.8.0"
+version = "2.9.0"
 description = "A faster version of dbus-next"
 authors = ["Bluetooth Devices Authors <bluetooth@koston.org>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bluetooth-devices/dbus-fast"
 documentation = "https://dbus-fast.readthedocs.io"
 classifiers = [
```

### Comparing `dbus_fast-2.8.0/src/dbus_fast/__init__.py` & `dbus_fast-2.9.0/src/dbus_fast/__init__.py`

 * *Files identical despite different names*

### Comparing `dbus_fast-2.8.0/src/dbus_fast/_private/address.py` & `dbus_fast-2.9.0/src/dbus_fast/_private/address.py`

 * *Files identical despite different names*

### Comparing `dbus_fast-2.8.0/src/dbus_fast/_private/marshaller.pxd` & `dbus_fast-2.9.0/src/dbus_fast/_private/marshaller.pxd`

 * *Files identical despite different names*

### Comparing `dbus_fast-2.8.0/src/dbus_fast/_private/marshaller.py` & `dbus_fast-2.9.0/src/dbus_fast/_private/marshaller.py`

 * *Files identical despite different names*

### Comparing `dbus_fast-2.8.0/src/dbus_fast/_private/unmarshaller.pxd` & `dbus_fast-2.9.0/src/dbus_fast/_private/unmarshaller.pxd`

 * *Files 1% similar despite different names*

```diff
@@ -209,15 +209,17 @@
         protocol_version=cython.uint,
         key=cython.str,
     )
     cdef _read_header(self)
 
     @cython.locals(
         body=cython.list,
-        header_fields=cython.dict
+        header_fields=cython.dict,
+        token_as_int=cython.uint,
+        signature=cython.str,
     )
     cdef _read_body(self)
 
     cdef _unmarshall(self)
 
     cpdef unmarshall(self)
```

### Comparing `dbus_fast-2.8.0/src/dbus_fast/_private/unmarshaller.py` & `dbus_fast-2.9.0/src/dbus_fast/_private/unmarshaller.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
 SIGNATURE_TREE_A_OA_SA_SV = get_signature_tree("a{oa{sa{sv}}}")
 SIGNATURE_TREE_A_OA_SA_SV_TYPES_0 = SIGNATURE_TREE_A_OA_SA_SV.types[0]
 
 TOKEN_B_AS_INT = ord("b")
 TOKEN_U_AS_INT = ord("u")
 TOKEN_Y_AS_INT = ord("y")
-TOKEN_A_AS_INT = ord("o")
+TOKEN_A_AS_INT = ord("a")
 TOKEN_O_AS_INT = ord("o")
 TOKEN_S_AS_INT = ord("s")
 TOKEN_G_AS_INT = ord("g")
 TOKEN_N_AS_INT = ord("n")
 
 ARRAY = array.array
 SOL_SOCKET = socket.SOL_SOCKET
@@ -433,53 +433,55 @@
         return self._buf[o : o + signature_len].decode()
 
     def read_variant(self, type_: _SignatureType) -> Variant:
         return self._read_variant()
 
     def _read_variant(self) -> Variant:
         signature = self._read_signature()
-        token_as_int = signature[0]
+        token_as_int = ord(signature[0])
         # verify in Variant is only useful on construction not unmarshalling
-        if token_as_int == TOKEN_N_AS_INT:
-            return Variant(SIGNATURE_TREE_N, self._read_int16_unpack(), False)
-        elif token_as_int == TOKEN_A_AS_INT and signature == "ay":
-            return Variant(
-                SIGNATURE_TREE_AY, self.read_array(SIGNATURE_TREE_AY_TYPES_0), False
-            )
-        elif token_as_int == TOKEN_A_AS_INT and signature == "a{qv}":
-            return Variant(
-                SIGNATURE_TREE_A_QV,
-                self.read_array(SIGNATURE_TREE_A_QV_TYPES_0),
-                False,
-            )
-        elif token_as_int == TOKEN_S_AS_INT:
-            return Variant(SIGNATURE_TREE_S, self._read_string_unpack(), False)
-        elif token_as_int == TOKEN_B_AS_INT:
-            return Variant(SIGNATURE_TREE_B, self._read_boolean(), False)
-        elif token_as_int == TOKEN_O_AS_INT:
-            return Variant(SIGNATURE_TREE_O, self._read_string_unpack(), False)
-        elif token_as_int == TOKEN_A_AS_INT and signature == "as":
-            return Variant(
-                SIGNATURE_TREE_AS, self.read_array(SIGNATURE_TREE_AS_TYPES_0), False
-            )
-        elif token_as_int == TOKEN_A_AS_INT and signature == "a{sv}":
-            return Variant(
-                SIGNATURE_TREE_A_SV,
-                self.read_array(SIGNATURE_TREE_A_SV_TYPES_0),
-                False,
-            )
-        elif token_as_int == TOKEN_A_AS_INT and signature == "ao":
-            return Variant(
-                SIGNATURE_TREE_AO, self.read_array(SIGNATURE_TREE_AO_TYPES_0), False
-            )
-        elif token_as_int == TOKEN_U_AS_INT:
-            return Variant(SIGNATURE_TREE_U, self._read_uint32_unpack(), False)
-        elif token_as_int == TOKEN_Y_AS_INT:
-            self._pos += 1
-            return Variant(SIGNATURE_TREE_Y, self._buf[self._pos - 1], False)
+        if len(signature) == 1:
+            if token_as_int == TOKEN_N_AS_INT:
+                return Variant(SIGNATURE_TREE_N, self._read_int16_unpack(), False)
+            if token_as_int == TOKEN_S_AS_INT:
+                return Variant(SIGNATURE_TREE_S, self._read_string_unpack(), False)
+            if token_as_int == TOKEN_B_AS_INT:
+                return Variant(SIGNATURE_TREE_B, self._read_boolean(), False)
+            if token_as_int == TOKEN_O_AS_INT:
+                return Variant(SIGNATURE_TREE_O, self._read_string_unpack(), False)
+            if token_as_int == TOKEN_U_AS_INT:
+                return Variant(SIGNATURE_TREE_U, self._read_uint32_unpack(), False)
+            if token_as_int == TOKEN_Y_AS_INT:
+                self._pos += 1
+                return Variant(SIGNATURE_TREE_Y, self._buf[self._pos - 1], False)
+        elif token_as_int == TOKEN_A_AS_INT:
+            if signature == "ay":
+                return Variant(
+                    SIGNATURE_TREE_AY, self.read_array(SIGNATURE_TREE_AY_TYPES_0), False
+                )
+            if signature == "a{qv}":
+                return Variant(
+                    SIGNATURE_TREE_A_QV,
+                    self.read_array(SIGNATURE_TREE_A_QV_TYPES_0),
+                    False,
+                )
+            if signature == "as":
+                return Variant(
+                    SIGNATURE_TREE_AS, self.read_array(SIGNATURE_TREE_AS_TYPES_0), False
+                )
+            if signature == "a{sv}":
+                return Variant(
+                    SIGNATURE_TREE_A_SV,
+                    self.read_array(SIGNATURE_TREE_A_SV_TYPES_0),
+                    False,
+                )
+            if signature == "ao":
+                return Variant(
+                    SIGNATURE_TREE_AO, self.read_array(SIGNATURE_TREE_AO_TYPES_0), False
+                )
         tree = get_signature_tree(signature)
         signature_type = tree.types[0]
         return Variant(
             tree,
             self._readers[signature_type.token](self, signature_type),
             False,
         )
@@ -670,45 +672,51 @@
         self._pos = HEADER_ARRAY_OF_STRUCT_SIGNATURE_POSITION
         header_fields = self._header_fields(self._header_len)
         self._pos += -self._pos & 7  # align 8
         signature = header_fields.pop("signature", "")
         if not self._body_len:
             tree = SIGNATURE_TREE_EMPTY
             body: List[Any] = []
-        elif signature == "s":
-            tree = SIGNATURE_TREE_S
-            body = [self._read_string_unpack()]
-        elif signature == "sa{sv}as":
-            tree = SIGNATURE_TREE_SA_SV_AS
-            body = [
-                self._read_string_unpack(),
-                self.read_array(SIGNATURE_TREE_SA_SV_AS_TYPES_1),
-                self.read_array(SIGNATURE_TREE_SA_SV_AS_TYPES_2),
-            ]
-        elif signature == "oa{sa{sv}}":
-            tree = SIGNATURE_TREE_OA_SA_SV
-            body = [
-                self._read_string_unpack(),
-                self.read_array(SIGNATURE_TREE_OA_SA_SV_TYPES_1),
-            ]
-        elif signature == "oas":
-            tree = SIGNATURE_TREE_OAS
-            body = [
-                self._read_string_unpack(),
-                self.read_array(SIGNATURE_TREE_OAS_TYPES_1),
-            ]
-        elif signature == "a{oa{sa{sv}}}":
-            tree = SIGNATURE_TREE_A_OA_SA_SV
-            body = [self.read_array(SIGNATURE_TREE_A_OA_SA_SV_TYPES_0)]
-        elif signature == "o":
-            tree = SIGNATURE_TREE_O
-            body = [self._read_string_unpack()]
         else:
-            tree = get_signature_tree(signature)
-            body = [self._readers[t.token](self, t) for t in tree.types]
+            token_as_int = ord(signature[0])
+            if len(signature) == 1:
+                if token_as_int == TOKEN_O_AS_INT:
+                    tree = SIGNATURE_TREE_O
+                    body = [self._read_string_unpack()]
+                elif token_as_int == TOKEN_S_AS_INT:
+                    tree = SIGNATURE_TREE_S
+                    body = [self._read_string_unpack()]
+                else:
+                    tree = get_signature_tree(signature)
+                    body = [self._readers[t.token](self, t) for t in tree.types]
+            elif token_as_int == TOKEN_S_AS_INT and signature == "sa{sv}as":
+                tree = SIGNATURE_TREE_SA_SV_AS
+                body = [
+                    self._read_string_unpack(),
+                    self.read_array(SIGNATURE_TREE_SA_SV_AS_TYPES_1),
+                    self.read_array(SIGNATURE_TREE_SA_SV_AS_TYPES_2),
+                ]
+            elif token_as_int == TOKEN_O_AS_INT and signature == "oa{sa{sv}}":
+                tree = SIGNATURE_TREE_OA_SA_SV
+                body = [
+                    self._read_string_unpack(),
+                    self.read_array(SIGNATURE_TREE_OA_SA_SV_TYPES_1),
+                ]
+            elif token_as_int == TOKEN_O_AS_INT and signature == "oas":
+                tree = SIGNATURE_TREE_OAS
+                body = [
+                    self._read_string_unpack(),
+                    self.read_array(SIGNATURE_TREE_OAS_TYPES_1),
+                ]
+            elif token_as_int == TOKEN_A_AS_INT and signature == "a{oa{sa{sv}}}":
+                tree = SIGNATURE_TREE_A_OA_SA_SV
+                body = [self.read_array(SIGNATURE_TREE_A_OA_SA_SV_TYPES_0)]
+            else:
+                tree = get_signature_tree(signature)
+                body = [self._readers[t.token](self, t) for t in tree.types]
 
         flags = MESSAGE_FLAG_MAP.get(self._flag)
         if flags is None:
             flags = MESSAGE_FLAG_INTENUM(self._flag)
         self._message = Message(
             message_type=MESSAGE_TYPE_MAP[self._message_type],
             flags=flags,
```

### Comparing `dbus_fast-2.8.0/src/dbus_fast/_private/util.py` & `dbus_fast-2.9.0/src/dbus_fast/_private/util.py`

 * *Files identical despite different names*

### Comparing `dbus_fast-2.8.0/src/dbus_fast/aio/message_bus.py` & `dbus_fast-2.9.0/src/dbus_fast/aio/message_bus.py`

 * *Files identical despite different names*

### Comparing `dbus_fast-2.8.0/src/dbus_fast/aio/message_reader.py` & `dbus_fast-2.9.0/src/dbus_fast/aio/message_reader.py`

 * *Files identical despite different names*

### Comparing `dbus_fast-2.8.0/src/dbus_fast/aio/proxy_object.py` & `dbus_fast-2.9.0/src/dbus_fast/aio/proxy_object.py`

 * *Files identical despite different names*

### Comparing `dbus_fast-2.8.0/src/dbus_fast/auth.py` & `dbus_fast-2.9.0/src/dbus_fast/auth.py`

 * *Files identical despite different names*

### Comparing `dbus_fast-2.8.0/src/dbus_fast/constants.py` & `dbus_fast-2.9.0/src/dbus_fast/constants.py`

 * *Files identical despite different names*

### Comparing `dbus_fast-2.8.0/src/dbus_fast/errors.py` & `dbus_fast-2.9.0/src/dbus_fast/errors.py`

 * *Files identical despite different names*

### Comparing `dbus_fast-2.8.0/src/dbus_fast/glib/message_bus.py` & `dbus_fast-2.9.0/src/dbus_fast/glib/message_bus.py`

 * *Files identical despite different names*

### Comparing `dbus_fast-2.8.0/src/dbus_fast/glib/proxy_object.py` & `dbus_fast-2.9.0/src/dbus_fast/glib/proxy_object.py`

 * *Files identical despite different names*

### Comparing `dbus_fast-2.8.0/src/dbus_fast/introspection.py` & `dbus_fast-2.9.0/src/dbus_fast/introspection.py`

 * *Files identical despite different names*

### Comparing `dbus_fast-2.8.0/src/dbus_fast/message.pxd` & `dbus_fast-2.9.0/src/dbus_fast/message.pxd`

 * *Files identical despite different names*

### Comparing `dbus_fast-2.8.0/src/dbus_fast/message.py` & `dbus_fast-2.9.0/src/dbus_fast/message.py`

 * *Files identical despite different names*

### Comparing `dbus_fast-2.8.0/src/dbus_fast/message_bus.pxd` & `dbus_fast-2.9.0/src/dbus_fast/message_bus.pxd`

 * *Files identical despite different names*

### Comparing `dbus_fast-2.8.0/src/dbus_fast/message_bus.py` & `dbus_fast-2.9.0/src/dbus_fast/message_bus.py`

 * *Files identical despite different names*

### Comparing `dbus_fast-2.8.0/src/dbus_fast/proxy_object.py` & `dbus_fast-2.9.0/src/dbus_fast/proxy_object.py`

 * *Files identical despite different names*

### Comparing `dbus_fast-2.8.0/src/dbus_fast/send_reply.py` & `dbus_fast-2.9.0/src/dbus_fast/send_reply.py`

 * *Files identical despite different names*

### Comparing `dbus_fast-2.8.0/src/dbus_fast/service.pxd` & `dbus_fast-2.9.0/src/dbus_fast/service.pxd`

 * *Files identical despite different names*

### Comparing `dbus_fast-2.8.0/src/dbus_fast/service.py` & `dbus_fast-2.9.0/src/dbus_fast/service.py`

 * *Files identical despite different names*

### Comparing `dbus_fast-2.8.0/src/dbus_fast/signature.py` & `dbus_fast-2.9.0/src/dbus_fast/signature.py`

 * *Files identical despite different names*

### Comparing `dbus_fast-2.8.0/src/dbus_fast/unpack.py` & `dbus_fast-2.9.0/src/dbus_fast/unpack.py`

 * *Files identical despite different names*

### Comparing `dbus_fast-2.8.0/src/dbus_fast/validators.py` & `dbus_fast-2.9.0/src/dbus_fast/validators.py`

 * *Files identical despite different names*

### Comparing `dbus_fast-2.8.0/setup.py` & `dbus_fast-2.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ['dbus_fast', 'dbus_fast._private', 'dbus_fast.aio', 'dbus_fast.glib']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'dbus-fast',
-    'version': '2.8.0',
+    'version': '2.9.0',
     'description': 'A faster version of dbus-next',
     'long_description': '# dbus-fast\n\n<p align="center">\n  <a href="https://github.com/bluetooth-devices/dbus-fast/actions?query=workflow%3ACI">\n    <img src="https://img.shields.io/github/workflow/status/bluetooth-devices/dbus-fast/CI/main?label=CI&logo=github&style=flat-square" alt="CI Status" >\n  </a>\n  <a href="https://dbus-fast.readthedocs.io">\n    <img src="https://img.shields.io/readthedocs/dbus-fast.svg?logo=read-the-docs&logoColor=fff&style=flat-square" alt="Documentation Status">\n  </a>\n  <a href="https://codecov.io/gh/bluetooth-devices/dbus-fast">\n    <img src="https://img.shields.io/codecov/c/github/bluetooth-devices/dbus-fast.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">\n  </a>\n</p>\n<p align="center">\n  <a href="https://python-poetry.org/">\n    <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">\n  </a>\n  <a href="https://github.com/ambv/black">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">\n  </a>\n  <a href="https://github.com/pre-commit/pre-commit">\n    <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">\n  </a>\n</p>\n<p align="center">\n  <a href="https://pypi.org/project/dbus-fast/">\n    <img src="https://img.shields.io/pypi/v/dbus-fast.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">\n  </a>\n  <img src="https://img.shields.io/pypi/pyversions/dbus-fast.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">\n  <img src="https://img.shields.io/pypi/l/dbus-fast.svg?style=flat-square" alt="License">\n</p>\n\nA faster version of dbus-next originally from the [great DBus next library](https://github.com/altdesktop/python-dbus-next) ❤️\n\n## Installation\n\nInstall this via pip (or your favourite package manager):\n\n`pip install dbus-fast`\n\n[Documentation](https://dbus-fast.readthedocs.io/en/latest/)\n\ndbus-fast is a Python library for DBus that aims to be a performant fully featured high level library primarily geared towards integration of applications into Linux desktop and mobile environments.\n\nDesktop application developers can use this library for integrating their applications into desktop environments by implementing common DBus standard interfaces or creating custom plugin interfaces.\n\nDesktop users can use this library to create their own scripts and utilities to interact with those interfaces for customization of their desktop environment.\n\ndbus-fast plans to improve over other DBus libraries for Python in the following ways:\n\n- Zero dependencies and pure Python 3\n- An optional cython extension is available to speed up (un)marshalling\n- Focus on performance\n- Support for multiple IO backends including asyncio and the GLib main loop.\n- Nonblocking IO suitable for GUI development.\n- Target the latest language features of Python for beautiful services and clients.\n- Complete implementation of the DBus type system without ever guessing types.\n- Integration tests for all features of the library.\n- Completely documented public API.\n\n## Installing\n\nThis library is available on PyPi as [dbus-fast](https://pypi.org/project/dbus-fast/).\n\n```\npip3 install dbus-fast\n```\n\n## The Client Interface\n\nTo use a service on the bus, the library constructs a proxy object you can use to call methods, get and set properties, and listen to signals.\n\nFor more information, see the [overview for the high-level client](https://dbus-fast.readthedocs.io/en/latest/high-level-client/index.html).\n\nThis example connects to a media player and controls it with the [MPRIS](https://specifications.freedesktop.org/mpris-spec/latest/) DBus interface.\n\n```python\nfrom dbus_fast.aio import MessageBus\n\nimport asyncio\n\n\nasync def main():\n    bus = await MessageBus().connect()\n    # the introspection xml would normally be included in your project, but\n    # this is convenient for development\n    introspection = await bus.introspect(\'org.mpris.MediaPlayer2.vlc\', \'/org/mpris/MediaPlayer2\')\n\n    obj = bus.get_proxy_object(\'org.mpris.MediaPlayer2.vlc\', \'/org/mpris/MediaPlayer2\', introspection)\n    player = obj.get_interface(\'org.mpris.MediaPlayer2.Player\')\n    properties = obj.get_interface(\'org.freedesktop.DBus.Properties\')\n\n    # call methods on the interface (this causes the media player to play)\n    await player.call_play()\n\n    volume = await player.get_volume()\n    print(f\'current volume: {volume}, setting to 0.5\')\n\n    await player.set_volume(0.5)\n\n    # listen to signals\n    def on_properties_changed(interface_name, changed_properties, invalidated_properties):\n        for changed, variant in changed_properties.items():\n            print(f\'property changed: {changed} - {variant.value}\')\n\n    properties.on_properties_changed(on_properties_changed)\n\n    await asyncio.Event().wait()\n\nasyncio.run(main())\n```\n\n## The Service Interface\n\nTo define a service on the bus, use the `ServiceInterface` class and decorate class methods to specify DBus methods, properties, and signals with their type signatures.\n\nFor more information, see the [overview for the high-level service](https://python-dbus-fast.readthedocs.io/en/latest/high-level-service/index.html).\n\n```python\nfrom dbus_fast.service import ServiceInterface, method, dbus_property, signal, Variant\nfrom dbus_fast.aio MessageBus\n\nimport asyncio\n\nclass ExampleInterface(ServiceInterface):\n    def __init__(self, name):\n        super().__init__(name)\n        self._string_prop = \'kevin\'\n\n    @method()\n    def Echo(self, what: \'s\') -> \'s\':\n        return what\n\n    @method()\n    def GetVariantDict() -> \'a{sv}\':\n        return {\n            \'foo\': Variant(\'s\', \'bar\'),\n            \'bat\': Variant(\'x\', -55),\n            \'a_list\': Variant(\'as\', [\'hello\', \'world\'])\n        }\n\n    @dbus_property()\n    def string_prop(self) -> \'s\':\n        return self._string_prop\n\n    @string_prop.setter\n    def string_prop_setter(self, val: \'s\'):\n        self._string_prop = val\n\n    @signal()\n    def signal_simple(self) -> \'s\':\n        return \'hello\'\n\nasync def main():\n    bus = await MessageBus().connect()\n    interface = ExampleInterface(\'test.interface\')\n    bus.export(\'/test/path\', interface)\n    # now that we are ready to handle requests, we can request name from D-Bus\n    await bus.request_name(\'test.name\')\n    # wait indefinitely\n    await asyncio.Event().wait()\n\nasyncio.run(main())\n```\n\n## The Low-Level Interface\n\nThe low-level interface works with DBus messages directly.\n\nFor more information, see the [overview for the low-level interface](https://python-dbus-fast.readthedocs.io/en/latest/low-level-interface/index.html).\n\n```python\nfrom dbus_fast.message import Message, MessageType\nfrom dbus_fast.aio import MessageBus\n\nimport asyncio\nimport json\n\n\nasync def main():\n    bus = await MessageBus().connect()\n\n    reply = await bus.call(\n        Message(destination=\'org.freedesktop.DBus\',\n                path=\'/org/freedesktop/DBus\',\n                interface=\'org.freedesktop.DBus\',\n                member=\'ListNames\'))\n\n    if reply.message_type == MessageType.ERROR:\n        raise Exception(reply.body[0])\n\n    print(json.dumps(reply.body[0], indent=2))\n\n\nasyncio.run(main())\n```\n\n## Projects that use python-dbus-fast\n\n- [Bluetooth Adapters](https://github.com/bluetooth-devices/bluetooth-adapters)\n\n## Contributing\n\nContributions are welcome. Development happens on [Github](https://github.com/Bluetooth-Devices/dbus-fast).\n\nBefore you commit, run `pre-commit run --all-files` to run the linter, code formatter, and the test suite.\n\n## Copyright\n\nYou can use this code under an MIT license (see LICENSE).\n\n- © 2019, Tony Crisci\n- © 2022, Bluetooth Devices authors\n\n## Contributors ✨\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- prettier-ignore-start -->\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- markdownlint-disable -->\n<!-- markdownlint-enable -->\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n<!-- prettier-ignore-end -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n\n## Credits\n\nThis package was created with\n[Cookiecutter](https://github.com/audreyr/cookiecutter) and the\n[browniebroke/cookiecutter-pypackage](https://github.com/browniebroke/cookiecutter-pypackage)\nproject template.\n',
     'author': 'Bluetooth Devices Authors',
     'author_email': 'bluetooth@koston.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/bluetooth-devices/dbus-fast',
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['dbus_fast', 'dbus_fast._private', 'dbus_fast.aio',
 'dbus_fast.glib'] package_data = \ {'': ['*']} setup_kwargs = { 'name': 'dbus-
-fast', 'version': '2.8.0', 'description': 'A faster version of dbus-next',
+fast', 'version': '2.9.0', 'description': 'A faster version of dbus-next',
 'long_description': '# dbus-fast\n\n
     \n _\_n_ _[_C_I_ _S_t_a_t_u_s_]_\_n_ \n _\_n_ _[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_\_n_ \n _\_n_ _[_T_e_s_t_ _c_o_v_e_r_a_g_e
                                _p_e_r_c_e_n_t_a_g_e_]_\_n_ \n
 \n
            \n _\_n_ _[_P_o_e_t_r_y_]_\_n_ \n _\_n_ _[_b_l_a_c_k_]_\_n_ \n _\_n_ _[_p_r_e_-_c_o_m_m_i_t_]_\_n_ \n
 \n
       \n _\_n_ _[_P_y_P_I_ _V_e_r_s_i_o_n_]_\_n_ \n [Supported Python versions]\n [License]\n
```

### Comparing `dbus_fast-2.8.0/PKG-INFO` & `dbus_fast-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbus-fast
-Version: 2.8.0
+Version: 2.9.0
 Summary: A faster version of dbus-next
 Home-page: https://github.com/bluetooth-devices/dbus-fast
 License: MIT
 Author: Bluetooth Devices Authors
 Author-email: bluetooth@koston.org
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

