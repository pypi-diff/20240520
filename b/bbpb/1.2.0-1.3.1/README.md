# Comparing `tmp/bbpb-1.2.0.tar.gz` & `tmp/bbpb-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbpb-1.2.0.tar", max compression
+gzip compressed data, was "bbpb-1.3.1.tar", max compression
```

## Comparing `bbpb-1.2.0.tar` & `bbpb-1.3.1.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0    11001 2024-05-13 04:43:10.974932 bbpb-1.2.0/README.md
--rw-r--r--   0        0        0     1577 2024-05-13 04:43:10.974932 bbpb-1.2.0/blackboxprotobuf/__init__.py
--rw-r--r--   0        0        0     8896 2024-05-13 04:43:10.974932 bbpb-1.2.0/blackboxprotobuf/__main__.py
--rw-r--r--   0        0        0     1382 2024-05-13 04:43:10.974932 bbpb-1.2.0/blackboxprotobuf/lib/__init__.py
--rw-r--r--   0        0        0    27799 2024-05-13 04:43:10.974932 bbpb-1.2.0/blackboxprotobuf/lib/api.py
--rw-r--r--   0        0        0     2265 2024-05-13 04:43:10.974932 bbpb-1.2.0/blackboxprotobuf/lib/config.py
--rw-r--r--   0        0        0     3760 2024-05-13 04:43:10.974932 bbpb-1.2.0/blackboxprotobuf/lib/exceptions.py
--rw-r--r--   0        0        0     2798 2024-05-13 04:43:10.974932 bbpb-1.2.0/blackboxprotobuf/lib/payloads/__init__.py
--rw-r--r--   0        0        0     3469 2024-05-13 04:43:10.974932 bbpb-1.2.0/blackboxprotobuf/lib/payloads/grpc.py
--rw-r--r--   0        0        0     1695 2024-05-13 04:43:10.974932 bbpb-1.2.0/blackboxprotobuf/lib/payloads/gzip.py
--rw-r--r--   0        0        0    16052 2024-05-13 04:43:10.974932 bbpb-1.2.0/blackboxprotobuf/lib/protofile.py
--rw-r--r--   0        0        0     1296 2024-05-13 04:43:10.974932 bbpb-1.2.0/blackboxprotobuf/lib/types/__init__.py
--rw-r--r--   0        0        0     3911 2024-05-13 04:43:10.974932 bbpb-1.2.0/blackboxprotobuf/lib/types/fixed.py
--rw-r--r--   0        0        0    26259 2024-05-13 04:43:10.974932 bbpb-1.2.0/blackboxprotobuf/lib/types/length_delim.py
--rw-r--r--   0        0        0     5089 2024-05-13 04:43:10.974932 bbpb-1.2.0/blackboxprotobuf/lib/types/type_maps.py
--rw-r--r--   0        0        0     5889 2024-05-13 04:43:10.974932 bbpb-1.2.0/blackboxprotobuf/lib/types/varint.py
--rw-r--r--   0        0        0     1217 2024-05-13 04:43:10.974932 bbpb-1.2.0/blackboxprotobuf/lib/types/wiretypes.py
--rw-r--r--   0        0        0      660 2024-05-13 04:43:10.974932 bbpb-1.2.0/pyproject.toml
--rw-r--r--   0        0        0    11819 1970-01-01 00:00:00.000000 bbpb-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    10909 2024-05-20 00:25:00.829196 bbpb-1.3.1/README.md
+-rw-r--r--   0        0        0     1577 2024-05-20 00:13:10.602735 bbpb-1.3.1/blackboxprotobuf/__init__.py
+-rw-r--r--   0        0        0    10922 2024-05-20 00:13:10.606738 bbpb-1.3.1/blackboxprotobuf/__main__.py
+-rw-r--r--   0        0        0     1382 2024-05-20 00:13:10.606738 bbpb-1.3.1/blackboxprotobuf/lib/__init__.py
+-rw-r--r--   0        0        0    30964 2024-05-20 00:13:10.606738 bbpb-1.3.1/blackboxprotobuf/lib/api.py
+-rw-r--r--   0        0        0     2756 2024-05-20 00:13:10.606738 bbpb-1.3.1/blackboxprotobuf/lib/config.py
+-rw-r--r--   0        0        0     4208 2024-05-20 00:13:10.606738 bbpb-1.3.1/blackboxprotobuf/lib/exceptions.py
+-rw-r--r--   0        0        0     3192 2024-05-20 00:13:10.606738 bbpb-1.3.1/blackboxprotobuf/lib/payloads/__init__.py
+-rw-r--r--   0        0        0     3614 2024-05-20 00:13:10.606738 bbpb-1.3.1/blackboxprotobuf/lib/payloads/grpc.py
+-rw-r--r--   0        0        0     1846 2024-05-20 00:13:10.606738 bbpb-1.3.1/blackboxprotobuf/lib/payloads/gzip.py
+-rw-r--r--   0        0        0    17601 2024-05-20 00:13:10.606738 bbpb-1.3.1/blackboxprotobuf/lib/protofile.py
+-rw-r--r--   0        0        0     1911 2024-05-20 00:13:10.606738 bbpb-1.3.1/blackboxprotobuf/lib/pytypes.py
+-rw-r--r--   0        0        0     1296 2024-05-20 00:13:10.606738 bbpb-1.3.1/blackboxprotobuf/lib/types/__init__.py
+-rw-r--r--   0        0        0     4696 2024-05-20 00:13:10.606738 bbpb-1.3.1/blackboxprotobuf/lib/types/fixed.py
+-rw-r--r--   0        0        0    28482 2024-05-20 00:13:10.606738 bbpb-1.3.1/blackboxprotobuf/lib/types/length_delim.py
+-rw-r--r--   0        0        0     5324 2024-05-20 00:13:10.606738 bbpb-1.3.1/blackboxprotobuf/lib/types/type_maps.py
+-rw-r--r--   0        0        0     6597 2024-05-20 00:13:10.606738 bbpb-1.3.1/blackboxprotobuf/lib/types/varint.py
+-rw-r--r--   0        0        0     1217 2024-05-20 00:13:10.606738 bbpb-1.3.1/blackboxprotobuf/lib/types/wiretypes.py
+-rw-r--r--   0        0        0        0 2024-05-20 00:13:10.606738 bbpb-1.3.1/blackboxprotobuf/py.typed
+-rw-r--r--   0        0        0      778 2024-05-20 00:25:00.829196 bbpb-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0    11727 1970-01-01 00:00:00.000000 bbpb-1.3.1/PKG-INFO
```

### Comparing `bbpb-1.2.0/README.md` & `bbpb-1.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -38,32 +38,30 @@
 re-encode the data. In general, most fields of interest are likely to be parsed
 into a usable form. Users can optionally pass in custom type definitions that
 override the guessed type. Custom type definitions also allow naming of fields to
 improve user friendliness.
 
 # Usage
 ## Installation    
-This library depends on internal functions of Google's protobuf Python library
-to do some encoding/decoding of individual fields and six for python 2
-compatibility.
-
 The package can be installed from source with:
 
 ```
 poetry install
 ```
 
 BlackBox Protobuf is also available on PyPi at <https://pypi.org/project/bbpb>.
 It can be installed with:
 
 ```
 pip install bbpb
 ```
 
 ## CLI
+The package defines a `bbpb` command for command line encoding/decoding.
+
 For command line usage see [CLI.md](./CLI.md).
 
 ## Interface
 The main `blackboxprotobuf` module defines an API with the core encode/decode
 message functions, along with several convenience functions to make it easier
 to use blackboxprotobuf with a user interface, such as encoding/decoding
 directly to JSON and validating modified type definitions.
```

### Comparing `bbpb-1.2.0/blackboxprotobuf/__init__.py` & `bbpb-1.3.1/blackboxprotobuf/__init__.py`

 * *Files identical despite different names*

### Comparing `bbpb-1.2.0/blackboxprotobuf/__main__.py` & `bbpb-1.3.1/blackboxprotobuf/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,20 +20,25 @@
 
 import sys
 import json
 import base64
 import logging
 import argparse
 
+import typing
+from typing import Any, Dict, Optional, Tuple
+
 from .lib.exceptions import BlackboxProtobufException
 from .lib import api
 from .lib import payloads
+from .lib.pytypes import TypeDef, Message
 
 
 def main():
+    # type: () -> int
     parser = argparse.ArgumentParser(description="Decode/Encode Protobuf Messages")
     parser.add_argument(
         "-e",
         "--encode",
         action="store_true",
         help="Switch to encode mode. Command decodes by default",
     )
@@ -71,15 +76,17 @@
         "--raw-decode",
         action="store_true",
         help="(Decoding) Output just the decoded JSON and no type information.",
     )
 
     args = parser.parse_args()
 
-    message, typedef, payload_encoding = None, None, None
+    message = None  # type:  str | bytes | Message | None
+    typedef = None  # type: TypeDef | None
+    payload_encoding = None  # type: str | None
 
     if args.input_type:
         typedef, payload_encoding = _read_input_typedef_arg(args)
 
     if args.payload_encoding:
         payload_encoding = args.payload_encoding
 
@@ -98,152 +105,181 @@
         message = input_data
 
     if payload_encoding is None:
         payload_encoding = "none"
 
     # Start basic, raw protobuf decoding
     if args.encode:
+        if not isinstance(message, dict):
+            sys.stderr.write("Error did not get a valid message to encode")
+            return 1
+        if typedef is None:
+            sys.stderr.write("Encoding requires a valid type definition")
+            return 1
         return _encode(args, message, typedef, payload_encoding)
     else:
+        if isinstance(message, str):
+            message = message.encode("utf-8")
+        if not isinstance(message, bytes):
+            sys.stderr.write("Error did not get a valid message to decode")
+            return 1
         return _decode(args, message, typedef, payload_encoding)
 
 
 # Reads input from the location from args
 # Does not handle any JSON decoding
 def _read_input(args):
+    # type: (argparse.Namespace) -> str | bytes
     if args.encode or args.json_protobuf:
         # Text
-        data = sys.stdin.read()
+        return sys.stdin.read()
     else:
         # Binary
-        data = sys.stdin.buffer.read()
-
-    return data
+        return sys.stdin.buffer.read()
 
 
 # Writes output to the location from args
 # Does not handle any JSON encoding
 def _write_output(args, data):
-    if not args.encode or args.json_protobuf:
+    # type: (argparse.Namespace, str | bytes) -> None
+    if isinstance(data, str):
         # Text
         sys.stdout.write(data)
     else:
         # Binary
         sys.stdout.buffer.write(data)
 
 
 def _read_input_typedef_arg(args):
+    # type: (argparse.Namespace) -> Tuple[TypeDef, Optional[str]]
     with open(args.input_type, "r") as f:
         input_json = json.load(f)
     if "typedef" in input_json:
         return input_json.get("typedef"), input_json.get("payload_encoding")
     else:
         # Return whole paylaod as typedef, no encoding
         return input_json, None
 
 
 def _write_output_typedef_arg(args, typedef):
+    # type: (argparse.Namespace, Dict[str, str | TypeDef]) -> None
     with open(args.output_type, "w") as f:
         f.write(_to_json(args, typedef))
 
 
 def _to_json(args, data):
+    # type: (argparse.Namespace, Dict[str, Any]) -> str
     if args.compact:
         return json.dumps(data)
     else:
         return json.dumps(data, indent=2)
 
 
 def _read_input_json_encoding(args, input_json, typedef, payload_encoding):
+    # type: (argparse.Namespace, Message | Dict[str, str | Message | TypeDef], Optional[TypeDef], Optional[str]) -> Tuple[Message, Optional[TypeDef], Optional[str]]
     if typedef is None and "typedef" not in input_json:
         sys.stderr.write(
             "Error: Did not get a typedef from --input-type or stdin. A typedef is required for encoding\n"
         )
         sys.exit(1)
 
-    message = input_json.get("message")
+    message = typing.cast(Message | None, input_json.get("message"))
     if message is None:
         # Whole input is message. We already checked to make sure we have a typedef, so we can ditch it
-        return input_json, typedef, None
+        return typing.cast(Message, input_json), typedef, None
 
     if typedef is None:
-        typedef = input_json.get("typedef")
+        typedef = typing.cast(TypeDef | None, input_json.get("typedef"))
 
     if payload_encoding is None:
-        payload_encoding = input_json.get("payload_encoding")
+        json_payload_encoding = input_json.get("payload_encoding")
+        if isinstance(json_payload_encoding, str):
+            payload_encoding = json_payload_encoding
+        elif json_payload_encoding is None:
+            payload_encoding = None
+        else:
+            sys.stderr.write(
+                "Warn: Payload encoding must be a string value: %r" % payload_encoding
+            )
+            payload_encoding = None
 
     return message, typedef, payload_encoding
 
 
 def _read_input_json_decoding(args, input_json, typedef, payload_encoding):
+    # type: (argparse.Namespace, Dict[str, TypeDef | str], Optional[TypeDef], Optional[str]) -> Tuple[bytes, Optional[TypeDef], Optional[str]]
     # Return message, typedef, payload_encoding
-    message = input_json.get("protobuf_data")
+    message = typing.cast(str | None, input_json.get("protobuf_data"))
     if message is None:
         sys.stderr.write('Error: Did not get a "protobuf_data" attribute in input JSON')
         sys.exit(1)
 
     if typedef is None:
-        typedef = input_json.get("typedef")
+        typedef = typing.cast(TypeDef | None, input_json.get("typedef"))
 
     if payload_encoding is None:
-        payload_encoding = input_json.get("payload_encoding")
+        payload_encoding = typing.cast(str | None, input_json.get("payload_encoding"))
 
     # base64 decode if protobuf_json when decoding
-    message = base64.b64decode(message)
+    protobuf_data = base64.b64decode(message)
 
-    return message, typedef, payload_encoding
+    return protobuf_data, typedef, payload_encoding
 
 
-def _encode(args, data, typedef, payload_encoding):
+def _encode(args, message, typedef, payload_encoding):
+    # type: (argparse.Namespace, Message, TypeDef, Optional[str]) -> int
     if typedef is None:
         sys.stderr.write("Error: Cannot encode without a valid typedef")
         return 1
 
     if not payload_encoding:
         payload_encoding = "none"
 
     # Re jsonify so that bbpb can fix bytes
-    message_json = json.dumps(data)
+    message_json = json.dumps(message)
 
     protobuf_data = api.protobuf_from_json(message_json, typedef)
 
     data = payloads.encode_payload(protobuf_data, payload_encoding)
 
     if args.json_protobuf:
-        data = {
+        json_out = {
             "protobuf_data": base64.b64encode(data).decode("ascii"),
             "typedef": typedef,  # Typedef is a bit redundant here
         }
         if payload_encoding != "none":
-            data["payload_encoding"] = payload_encoding
-        data = _to_json(args, data)
-    _write_output(args, data)
+            json_out["payload_encoding"] = payload_encoding
+
+        _write_output(args, _to_json(args, json_out))
+    else:
+        _write_output(args, data)
     return 0
 
 
-def _decode(args, message, typedef, payload_encoding):
-    if len(message) == 0:
+def _decode(args, data, typedef, payload_encoding):
+    # type: (argparse.Namespace, bytes, Optional[TypeDef], str) -> int
+    if len(data) == 0:
         sys.stderr.write("Error: Input data cannot be empty\n")
         return 1
 
     # args.protobuf_json is already handled
 
     if payload_encoding:
         # Use provided payload encoding algorithm
         protobuf_data, payload_encoding = payloads.decode_payload(
-            message, payload_encoding
+            data, payload_encoding
         )
         message_json, output_typedef = api.protobuf_to_json(protobuf_data, typedef)
     else:
         # Have to guess the decoding algorithm
-        decoders = payloads.find_decoders(message)
+        decoders = payloads.find_decoders(data)
 
         for decode in decoders:
             try:
-                protobuf_data, encoding_alg = decode(message)
+                protobuf_data, encoding_alg = decode(data)
             except BlackboxProtobufException:
                 # The "none" algorithm should always succeed
                 continue
 
             try:
                 message_json, output_typedef = api.protobuf_to_json(
                     protobuf_data, typedef
@@ -252,17 +288,16 @@
             except BlackboxProtobufException as exc:
                 if encoding_alg == "none":
                     raise exc
 
     message = json.loads(message_json)
 
     if args.output_type:
-        output_typedef_data = {
-            "typedef": output_typedef,
-        }
+        output_typedef_data = {}  # type: Dict[str, TypeDef | str]
+        output_typedef_data["typedef"] = output_typedef
         if payload_encoding != "none":
             output_typedef_data["payload_encoding"] = payload_encoding
         _write_output_typedef_arg(args, output_typedef_data)
 
     if args.raw_decode:
         output = message
     else:
```

### Comparing `bbpb-1.2.0/blackboxprotobuf/lib/__init__.py` & `bbpb-1.3.1/blackboxprotobuf/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `bbpb-1.2.0/blackboxprotobuf/lib/api.py` & `bbpb-1.3.1/blackboxprotobuf/lib/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,19 +40,29 @@
 import re
 import six
 import json
 import collections
 import blackboxprotobuf.lib.protofile
 import blackboxprotobuf.lib.types.length_delim
 import blackboxprotobuf.lib.types.type_maps
-import blackboxprotobuf.lib.config
+from blackboxprotobuf.lib.config import default as default_config
 from blackboxprotobuf.lib.exceptions import TypedefException, EncoderException
 
+if six.PY3:
+    import typing
+
+    # Circular imports on Config if we don't check here
+    if typing.TYPE_CHECKING:
+        from typing import Dict, List, Optional
+        from blackboxprotobuf.lib.pytypes import Message, TypeDef, FieldDef
+        from blackboxprotobuf.lib.config import Config
+
 
 def decode_message(buf, message_type=None, config=None):
+    # type: (bytes, Optional[str | TypeDef], Optional[Config]) -> tuple[Message, TypeDef]
     """Decode a protobuf message and return a python dictionary representing
     the message.
 
     Args:
         buf: Bytes representing an encoded protobuf message
         message_type: Optional type to use as the base for decoding. Allows for
             customizing field types or names. Can be a python dictionary or a
@@ -68,34 +78,35 @@
 
         The type definition is based on the `message_type` argument if one was
         provided, but may add additional fields if new fields were encountered
         during decoding.
     """
 
     if config is None:
-        config = blackboxprotobuf.lib.config.default
+        config = default_config
 
     if isinstance(buf, bytearray):
         buf = bytes(buf)
     buf = six.ensure_binary(buf)
     if message_type is None:
         message_type = {}
-    elif isinstance(message_type, str):
+    elif isinstance(message_type, six.text_type):
         if message_type not in config.known_types:
             message_type = {}
         else:
             message_type = config.known_types[message_type]
 
     value, typedef, _, _ = blackboxprotobuf.lib.types.length_delim.decode_message(
         buf, config, message_type
     )
     return value, typedef
 
 
 def encode_message(value, message_type, config=None):
+    # type: (Message, str | TypeDef, Optional[Config]) -> bytes
     """Re-encode a python dictionary as a binary protobuf message.
 
     Args:
         value: Python dictionary to re-encode to bytes. This should usually be
             a modified version of the dictionary returned by `decode_message`.
         message_type: Type definition to use to re-encode the message. This
             will should generally be the type definition returned from the
@@ -105,37 +116,38 @@
             `known_types` array. Defaults to
             `blackboxprotobuf.lib.config.default` if not provided.
     Returns:
         A bytearray containing the encoded protobuf message.
     """
 
     if config is None:
-        config = blackboxprotobuf.lib.config.default
+        config = default_config
 
     if message_type is None:
         raise EncoderException(
             "Encode message must have valid type definition. message_type cannot be None"
         )
 
-    if isinstance(message_type, str):
+    if isinstance(message_type, six.text_type):
         if message_type not in config.known_types:
             raise EncoderException(
                 "The provided message type name (%s) is not known. Encoding requires a valid type definition"
                 % message_type
             )
         message_type = config.known_types[message_type]
 
     return bytes(
         blackboxprotobuf.lib.types.length_delim.encode_message(
             value, config, message_type
         )
     )
 
 
-def protobuf_to_json(*args, **kwargs):
+def protobuf_to_json(buf, message_type=None, config=None):
+    # type: (bytes, Optional[str | TypeDef], Optional[Config]) -> tuple[str, TypeDef]
     """Decode a protobuf message and return a JSON string representing the
     message.
 
     Args:
         buf: Bytes representing an encoded protobuf message
         message_type: Optional type to use as the base for decoding. Allows for
             customizing field types or names. Can be a python dictionary or a
@@ -152,25 +164,24 @@
         The JSON string and type definition are annotated and sorted for
         readability.
 
         The type definition is based on the `message_type` argument if one was
         provided, but may add additional fields if new fields were encountered
         during decoding.
     """
-    value, message_type = decode_message(*args, **kwargs)
-    value = _json_safe_transform(
-        value, message_type, False, config=kwargs.get("config", None)
-    )
-    value = _sort_output(value, message_type, config=kwargs.get("config", None))
+    value, message_type = decode_message(buf, message_type, config)
+    value = _json_safe_transform(value, message_type, False, config=config)
+    value = _sort_output(value, message_type, config=config)
     _annotate_typedef(message_type, value)
     message_type = sort_typedef(message_type)
     return json.dumps(value, indent=2), message_type
 
 
-def protobuf_from_json(json_str, message_type, *args, **kwargs):
+def protobuf_from_json(json_str, message_type, config=None):
+    # type: (str, str | TypeDef, Optional[Config]) -> bytes
     """Re-encode a JSON string as a binary protobuf message.
 
     Args:
         json_str: JSON string to re-encode to protobuf message bytes. This
             should usually be a modified version of the value returned by
             `protobuf_to_json`.
         message_type: Type definition to use to re-encode the message. This
@@ -179,21 +190,31 @@
         config: `blackboxprotobuf.lib.config.Config` object which allows
             customizing default types for wire types and holds the
             `known_types` array. Defaults to
             `blackboxprotobuf.lib.config.default` if not provided.
     Returns:
         A bytearray containing the encoded protobuf message.
     """
+    if config is None:
+        config = default_config
+    if isinstance(message_type, six.text_type):
+        if message_type not in config.known_types:
+            raise EncoderException(
+                'protobuf_from_json must have valid type definition. message_type "%s" is not known'
+                % message_type
+            )
+        message_type = config.known_types[message_type]
     value = json.loads(json_str)
     _strip_typedef_annotations(message_type)
     value = _json_safe_transform(value, message_type, True)
-    return encode_message(value, message_type, *args, **kwargs)
+    return encode_message(value, message_type, config)
 
 
 def export_protofile(message_types, output_filename):
+    # type: (Dict[str, TypeDef], str) -> None
     """This function attempts to export a set of message type definitions to a
     `.proto` file for use with other tools.
 
     Args:
         message_types: Python dictionary containing the type definitions to
             export. The dictionary should contain the message type name as the
             key and the type definition as the value.
@@ -202,14 +223,15 @@
     """
     blackboxprotobuf.lib.protofile.export_proto(
         message_types, output_filename=output_filename
     )
 
 
 def import_protofile(input_filename, save_to_known=True, config=None):
+    # type: (str, bool, Optional[Config]) -> Dict[str, TypeDef] | None
     """This function attempts to import a set of message type definitions from a
     `.proto` file.
 
     This is a convenience function for `blackboxprotobuf.lib.protofile`. The
     protobuf file import support is not complete and may fail for some type
     definitions.
 
@@ -222,29 +244,31 @@
             Defaults to `blackboxprotobuf.lib.config.default`.
     Returns:
         If `save_to_known` is False, then the type definitions read from the
         file are returned as a dictionary, with the type names as the keys and
         type definitions as the values.
     """
     if config is None:
-        config = blackboxprotobuf.lib.config.default
+        config = default_config
 
     new_typedefs = blackboxprotobuf.lib.protofile.import_proto(
         config, input_filename=input_filename
     )
     if save_to_known:
         config.known_types.update(new_typedefs)
+        return None
     else:
         return new_typedefs
 
 
 NAME_REGEX = re.compile(r"\A[a-zA-Z][a-zA-Z0-9_]*\Z")
 
 
 def validate_typedef(typedef, old_typedef=None, config=None, _path=None):
+    # type: (TypeDef, Optional[TypeDef], Optional[Config], Optional[List[str]]) -> None
     """Attempt to validate a type definition object is valid.
 
     This function attempts to ensure a type definition is valid before it is
     used to encode/decode a message. This will make sure the field names are
     valid and field names/numbers are consistent. It is intended to be called
     after a user has edited the type definition to ensure the edits are valid.
 
@@ -262,27 +286,27 @@
     Raises:
         TypedefException: Raises a TypedefException if the provided type
             definition is not valid.
     """
     if _path is None:
         _path = []
     if config is None:
-        config = blackboxprotobuf.lib.config.default
+        config = default_config
 
     int_keys = set()
     field_names = set()
     for field_number, field_typedef in typedef.items():
         alt_field_number = None
         if "-" in str(field_number):
             field_number, alt_field_number = field_number.split("-")
 
         # Validate field_number is a number
         if not str(field_number).isdigit():
             raise TypedefException("Field number must be a digit: %s" % field_number)
-        field_number = str(field_number)
+        field_number = six.ensure_text(str(field_number))
 
         field_path = _path[:]
         field_path.append(field_number)
 
         # Check for duplicate field numbers
         if field_number in int_keys:
             raise TypedefException(
@@ -338,15 +362,24 @@
             if key == "type":
                 if value not in blackboxprotobuf.lib.types.type_maps.WIRETYPES:
                     raise TypedefException(
                         'Invalid type "%s" for field number %s' % (value, field_number),
                         field_path,
                     )
             # Check for duplicate names
-            if key == "name" and value.strip() != "":
+            if key == "name":
+                if not isinstance(value, six.text_type):
+                    raise TypedefException(
+                        "Invalid type for name field in typedef: %r. Field number %s"
+                        % (value, field_number),
+                        field_path,
+                    )
+                if value.strip() == "":
+                    continue
+
                 if value.lower() in field_names:
                     raise TypedefException(
                         ('Duplicate field name "%s" for field ' "number %s")
                         % (value, field_number),
                         field_path,
                     )
                 if not NAME_REGEX.match(value):
@@ -354,47 +387,48 @@
                         (
                             'Invalid field name "%s" for field '
                             "number %s. Should match %s"
                         )
                         % (value, field_number, "[a-zA-Z_][a-zA-Z0-9_]*"),
                         field_path,
                     )
-                if value != "":
-                    field_names.add(value.lower())
+                field_names.add(value.lower())
 
             # Check if message type name is known
             if key == "message_type_name":
                 if value not in config.known_types:
                     raise TypedefException(
                         (
                             'Message type "%s" for field number'
                             " %s is not known. Known types: %s"
                         )
                         % (value, field_number, config.known_types.keys()),
                         field_path,
                     )
 
             # Recursively validate inner typedefs
-            if key in ["message_typedef", "group_typedef"]:
+            if key == "message_typedef":
                 if isinstance(value, dict):
                     if (
                         old_typedef is not None
                         and field_number in old_typedef
                         and key in old_typedef[field_number]
                     ):
                         validate_typedef(
                             value,
-                            old_typedef=old_typedef[field_number][key],
+                            old_typedef=old_typedef[field_number]["message_typedef"],
                             _path=field_path,
                             config=config,
                         )
                     else:
                         validate_typedef(value, _path=field_path, config=config)
             if key == "alt_typedefs":
-                for alt_field_number, alt_typedef in value.items():
+                for alt_field_number, alt_typedef in field_typedef[
+                    "alt_typedefs"
+                ].items():
                     if isinstance(alt_typedef, dict):
                         validate_typedef(alt_typedef, _path=field_path, config=config)
 
     if old_typedef is not None:
         wiretype_map = {}
         for field_number, value in old_typedef.items():
             wiretype_map[
@@ -416,14 +450,15 @@
                         )
                         % field_number,
                         field_path,
                     )
 
 
 def _json_safe_transform(values, typedef, toBytes, config=None):
+    # type: (Message, TypeDef, bool, Optional[Config]) -> Message
     # Python's JSON doesn't have a default way to handle 'bytes' types. To
     # handle this, we want some string like encoding which JSON can handle but
     # can also handle arbitrary bytes. This method get's more complicated than
     # just converting all bytes since on re-encoding we need to know which ones
     # were transformed and which are supposed to actually be strings
 
     # A built-for binary encoding method like hex or base64 would be 'proper',
@@ -434,28 +469,30 @@
     # This uses latin1 encoding because it can handle arbitrary bytes, prints
     # ASCII characters and can be decoded back to the same exact byte string.
     # It's possible I missed another encoding method that matches these
     # properties across python2.7 and python3.9, but had issues with some other
     # backslash escape mechanisms parsing back to bytes.
 
     if config is None:
-        config = blackboxprotobuf.lib.config.default
+        config = default_config
     name_map = {
         item["name"]: number
         for number, item in typedef.items()
         if ("name" in item and item["name"] != "")
     }
     if not isinstance(values, dict):
         # this function should only ever be called on a message, error out if
         # it is not one. This usually means a type got swapped around
         raise EncoderException(
             "Error performing _json_safe_transform on message. Field was expected to be a message but was not: %r"
             % values
         )
     for name, value in values.items():
+        if isinstance(name, int):
+            name = six.ensure_text(str(name))
         alt_number = None
         base_name = name
         if "-" in name:
             base_name, alt_number = name.split("-")
 
         if base_name in name_map:
             field_number = name_map[base_name]
@@ -464,15 +501,15 @@
 
         if field_number not in typedef or "type" not in typedef[field_number]:
             raise EncoderException(
                 "Field %r not found in typedef or does not have type attribute."
                 % field_number
             )
 
-        field_type = typedef[field_number]["type"]
+        field_type = typedef[field_number]["type"]  # type: str | TypeDef
         if field_type == "message":
             field_typedef = _get_typedef_for_message(typedef[field_number], config)
             if alt_number is not None:
                 # if we have an alt type, then let's look that up instead
                 if alt_number not in typedef[field_number].get("alt_typedefs", {}):
                     raise TypedefException(
                         (
@@ -507,14 +544,15 @@
             values[name] = field_values[0]
         else:
             values[name] = field_values
     return values
 
 
 def _get_typedef_for_message(field_typedef, config):
+    # type: (FieldDef, Config) -> TypeDef
     assert field_typedef["type"] == "message"
     if "message_typedef" in field_typedef:
         return field_typedef["message_typedef"]
     elif field_typedef.get("message_type_name"):
         if field_typedef["message_type_name"] not in config.known_types:
             raise TypedefException(
                 "Got 'message_type_name' not in known_messages: %s"
@@ -524,32 +562,35 @@
     else:
         raise TypedefException(
             "Got 'message' type without typedef or type name: %s" % field_typedef
         )
 
 
 def _sort_output(value, typedef, config=None):
+    # type: (Message, TypeDef, Optional[Config]) -> Message
     # Sort output by the field number in the typedef. Helps with readability in
     # a JSON dump
-    output_dict = collections.OrderedDict()
+    output_dict = collections.OrderedDict()  # type: Message
     if config is None:
-        config = blackboxprotobuf.lib.config.default
+        config = default_config
 
     # Make a list of all the field names we have, aggregate together the alt fields as well
-    field_names = {}
+    field_names = {}  # type: Dict[str, List[tuple[str, str | None]]]
     for field_name in value.keys():
+        if isinstance(field_name, int):
+            field_name = six.ensure_text(str(field_name))
         if "-" in field_name:
             field_name_base, alt_number = field_name.split("-")
         else:
             field_name_base = field_name
             alt_number = None
         field_names.setdefault(field_name_base, []).append((field_name, alt_number))
 
     for field_number, field_def in sorted(typedef.items(), key=lambda t: int(t[0])):
-        field_number = str(field_number)
+        field_number = six.ensure_text(str(field_number))
         seen_field_names = field_names.get(field_number, [])
 
         # Try getting matching fields by name as well
         if field_def.get("name", "") != "":
             field_name = field_def["name"]
             seen_field_names.extend(field_names.get(field_name, []))
 
@@ -564,37 +605,55 @@
                     raise TypedefException(
                         (
                             "Provided alt field name/number "
                             "%s is not valid for field_number %s"
                         )
                         % (alt_number, field_number)
                     )
-                field_type = field_def["alt_typedefs"][alt_number]
-                if isinstance(field_type, dict):
-                    field_message_typedef = field_type
+                alt_field_type = field_def["alt_typedefs"][alt_number]
+                if isinstance(alt_field_type, dict):
+                    field_message_typedef = alt_field_type
                     field_type = "message"
+                else:
+                    field_type = alt_field_type
 
             if field_type == "message":
-                if not isinstance(value[field_name], list):
-                    output_dict[field_name] = _sort_output(
-                        value[field_name], field_message_typedef
+                if field_message_typedef is None:
+                    raise TypedefException(
+                        'Message does not have an associated typedef: "%s"' % field_name
                     )
-                else:
+                field_value = value.get(field_name)
+                if isinstance(field_value, list):
                     output_dict[field_name] = []
-                    for field_value in value[field_name]:
+                    for field_value_item in field_value:
+                        if not isinstance(field_value_item, dict):
+                            raise TypedefException(
+                                'Message values must be a dictionary type. Field name: "%s"'
+                                % field_name
+                            )
                         output_dict[field_name].append(
-                            _sort_output(field_value, field_message_typedef)
+                            _sort_output(field_value_item, field_message_typedef)
+                        )
+                else:
+                    if not isinstance(field_value, dict):
+                        raise TypedefException(
+                            'Message values must be a dictionary type. Field name: "%s"'
+                            % field_name
                         )
+                    output_dict[field_name] = _sort_output(
+                        field_value, field_message_typedef
+                    )
             else:
                 output_dict[field_name] = value[field_name]
 
     return output_dict
 
 
 def sort_typedef(typedef):
+    # type: (TypeDef) -> TypeDef
     """Apply special sorting rules to the type definition to improve readability.
 
     Sorts the fields of a type definition so that important fields such as the
     'type' or 'name' are at the top and don't get buried beneath longer fields
     like 'message_typedef'. This will also sort the keys of the
     'message_typedef' based on the field number.
     Args:
@@ -608,40 +667,48 @@
 
     TYPEDEF_KEY_ORDER = [
         "name",
         "type",
         "message_type_name",
         "example_value_ignored",
         "field_order",
+        "seen_repeated",
+        "message_typedef",
+        "alt_typedefs",
     ]
     output_dict = collections.OrderedDict()
 
-    for field_number, field_def in sorted(typedef.items(), key=lambda t: int(t[0])):
+    for field_number, field_def in sorted(
+        typedef.items(), key=lambda t: int(t[0])
+    ):  # Sort by type number
         output_field_def = collections.OrderedDict()
-        field_def = field_def.copy()
-        for key in TYPEDEF_KEY_ORDER:
-            if key in field_def:
-                output_field_def[key] = field_def[key]
-                del field_def[key]
-        for key, value in field_def.items():
+        for key, value in sorted(
+            field_def.items(), key=lambda t: (TYPEDEF_KEY_ORDER.index(t[0]), t[1])
+        ):  # sort by special keys, then value
             if key == "message_typedef":
-                output_field_def[key] = sort_typedef(value)
+                output_field_def[key] = sort_typedef(value)  # type: ignore
             else:
-                output_field_def[key] = value
+                output_field_def[key] = value  # type: ignore
+
         output_dict[field_number] = output_field_def
+    if six.PY3 and typing.TYPE_CHECKING:
+        return typing.cast(
+            TypeDef, output_dict
+        )  # Cast because typing doesn't like the ordered dict
     return output_dict
 
 
 def _annotate_typedef(typedef, message):
+    # type: (TypeDef, Message) -> None
     # Add values from message into the typedef so it's easier to figure out
     # which field when you're editing manually
 
     for field_number, field_def in typedef.items():
         field_value = None
-        field_name = str(field_number)
+        field_name = six.ensure_text(str(field_number))
         if field_name not in message and field_def.get("name", "") != "":
             field_name = field_def["name"]
 
         if field_name in message:
             field_value = message[field_name]
 
             if field_def["type"] == "message":
@@ -652,17 +719,18 @@
                     _annotate_typedef(field_def["message_typedef"], field_value)
             else:
                 field_def["example_value_ignored"] = field_value
 
         # Add a blank name field if the field doesn't have one, so it's easier
         # to add
         if "name" not in field_def:
-            field_def["name"] = ""
+            field_def["name"] = six.u("")
 
 
 def _strip_typedef_annotations(typedef):
+    # type: (TypeDef) -> None
     # Remove example values placed by _annotate_typedef
     for _, field_def in typedef.items():
         if "example_value_ignored" in field_def:
             del field_def["example_value_ignored"]
         if "message_typedef" in field_def:
             _strip_typedef_annotations(field_def["message_typedef"])
```

### Comparing `bbpb-1.2.0/blackboxprotobuf/lib/config.py` & `bbpb-1.3.1/blackboxprotobuf/lib/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,38 +16,56 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from .types import type_maps
 
+import six
+from blackboxprotobuf.lib.exceptions import (
+    DecoderException,
+)
+
+if six.PY3:
+    import typing
+
+    if typing.TYPE_CHECKING:
+        from typing import Dict
+        from .pytypes import TypeDef
+
 
 class Config:
     def __init__(self):
+        # type: (Config) -> None
         # Map of message type names to typedefs, previously stored at
         # `blackboxprotobuf.known_messages`
-        self.known_types = {}
+        self.known_types = {}  # type: Dict[str, TypeDef]
 
         # Default type for "bytes" like objects that aren't messages or strings
         # Other option is currently just 'bytes_hex'
         self.default_binary_type = "bytes"
 
         # Change the default type for a wiretype (eg. change ints to be signed
         # by default or fixed fields to always be float)
-        self.default_types = {}
+        self.default_types = {}  # type: Dict[int, str]
 
         # Configure whether bbpb should try to re-encode fields in the same
         # order they decoded
         # Field order shouldn't matter for real protobufs, but is there to ensure
         # that bytes/string are accidentally valid protobufs don't get scrambled
         # by decoding/re-encoding
         self.preserve_field_order = True
 
     def get_default_type(self, wiretype):
+        # type: (Config, int) -> str
         default_type = self.default_types.get(wiretype, None)
         if default_type is None:
             default_type = type_maps.WIRE_TYPE_DEFAULTS.get(wiretype, None)
 
+        if default_type is None:
+            raise DecoderException(
+                "Could not find default type for wire type %d" % wiretype
+            )
         return default_type
 
 
 default = Config()
```

### Comparing `bbpb-1.2.0/blackboxprotobuf/lib/exceptions.py` & `bbpb-1.3.1/blackboxprotobuf/lib/exceptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,32 +16,40 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
+import six
+
+if six.PY3:
+    from typing import Any, Optional, List
+
 
 class BlackboxProtobufException(Exception):
     """Base class for excepions raised by Blackbox Protobuf"""
 
     def __init__(self, message, path=None, *args):
+        # type: (str, Optional[List[str]], Any) -> None
         self.path = path
         super(BlackboxProtobufException, self).__init__(message, *args)
 
     def set_path(self, path):
+        # type: (BlackboxProtobufException, List[str]) -> None
         if self.path is None:
             self.path = path
 
 
 class TypedefException(BlackboxProtobufException):
     """Thrown when an error is identified in the type definition, such as
     conflicting or inconsistent values."""
 
     def __str__(self):
+        # type: (TypedefException) -> str
         message = super(TypedefException, self).__str__()
         if self.path is not None:
             message = (
                 "Encountered error within typedef for field %s: "
                 % "->".join(map(str, self.path))
             ) + message
         else:
@@ -49,44 +57,48 @@
         return message
 
 
 class EncoderException(BlackboxProtobufException, ValueError):
     """Thrown when there is an error encoding a dictionary to a type definition"""
 
     def __str__(self):
+        # type: (EncoderException) -> str
         message = super(EncoderException, self).__str__()
         if self.path is not None:
             message = (
                 "Encountered error encoding field %s: " % "->".join(map(str, self.path))
             ) + message
         else:
             message = ("Encountered error encoding message: ") + message
         return message
 
 
 class DecoderException(BlackboxProtobufException, ValueError):
     """Thrown when there is an error decoding a bytestring to a dictionary"""
 
     def __str__(self):
+        # type: (DecoderException) -> str
         message = super(DecoderException, self).__str__()
         if self.path is not None:
             message = (
                 "Encountered error decoding field %s: " % "->".join(map(str, self.path))
             ) + message
         else:
             message = ("Encountered error decoding message: ") + message
         return message
 
 
 class ProtofileException(BlackboxProtobufException):
     def __init__(self, message, path=None, filename=None, *args):
+        # type: (ProtofileException, str, Optional[List[str]], Optional[str], Any) -> None
         self.filename = filename
         super(BlackboxProtobufException, self).__init__(message, path, *args)
 
     def __str__(self):
+        # type: (ProtofileException) -> str
         message = super(ProtofileException, self).__str__()
         if self.path is not None:
             message = (
                 "Encountered error within protofile %s for field %s: "
                 % (self.filename, "->".join(map(str, self.path)))
             ) + message
         else:
```

### Comparing `bbpb-1.2.0/blackboxprotobuf/lib/payloads/__init__.py` & `bbpb-1.3.1/blackboxprotobuf/lib/payloads/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,58 +18,70 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """ The payloads module is intended to handle different encodings of the
     protobuf data, such as compression and grpc header. """
 
 from blackboxprotobuf.lib.exceptions import BlackboxProtobufException
-
 from . import gzip, grpc
 
+import six
+
+if six.PY3:
+    from typing import List, Callable, Tuple, Optional
+
 
 # Returns an ordered list of potential decoders, from most specific to least specific
 # The consumer should loop through each decoder, try to decode it and then try
 # to decode as a protobuf. This should minimize the chance of a false positive
 # on any decoders
 def find_decoders(buf):
+    # type: (bytes) -> List[Callable[[bytes], Tuple[bytes, str]]]
     # In the future, we can take into account content-type too, such as for
     # grpc, but we risk false negatives
-    decoders = []
+    decoders = []  # type: List[Callable[[bytes], Tuple[bytes, str]]]
 
     if gzip.is_gzip(buf):
         decoders.append(gzip.decode_gzip)
 
     if grpc.is_grpc(buf):
         decoders.append(grpc.decode_grpc)
 
     decoders.append(_none_decoder)
     return decoders
 
 
 def _none_decoder(buf):
+    # type: (bytes) -> Tuple[bytes, str]
     return buf, "none"
 
 
 # Decoder by name
 def decode_payload(buf, decoder):
+    # type: (bytes, Optional[str]) -> Tuple[bytes, str]
+    if decoder is None:
+        return buf, "none"
     decoder = decoder.lower()
-    if decoder is None or decoder == "none":
+    if decoder == "none":
         return buf, "none"
     elif decoder.startswith("grpc"):
         return grpc.decode_grpc(buf)
     elif decoder == "gzip":
         return gzip.decode_gzip(buf)
     else:
         raise BlackboxProtobufException("Unknown decoder: " + decoder)
 
 
 # Encode by name, should pass in the results from the decode function
 def encode_payload(buf, encoder):
+    # type: (bytes, Optional[str]) -> bytes
+    if encoder is None:
+        return buf
     encoder = encoder.lower()
-    if encoder is None or encoder == "none":
+    if encoder == "none":
         return buf
     elif encoder.startswith("grpc"):
         return grpc.encode_grpc(buf, encoder)
     elif encoder == "gzip":
         return gzip.encode_gzip(buf)
     else:
         raise BlackboxProtobufException("Unknown encoder: " + encoder)
```

### Comparing `bbpb-1.2.0/blackboxprotobuf/lib/payloads/grpc.py` & `bbpb-1.3.1/blackboxprotobuf/lib/payloads/grpc.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,20 +18,24 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import six
 import struct
 from blackboxprotobuf.lib.exceptions import BlackboxProtobufException
 
+if six.PY3:
+    from typing import Tuple
+
 # gRPC over HTTP2 spec: https://github.com/grpc/grpc/blob/master/doc/PROTOCOL-HTTP2.md
 
 HEADER_LEN = 1 + 4
 
 
 def is_grpc(payload):
+    # type: (bytes) -> bool
     if len(payload) < HEADER_LEN:
         return False
     if six.PY2 and isinstance(payload, bytearray):
         payload = bytes(payload)
     compression_byte = six.indexbytes(payload, 0)
     # Change this to support 0x1 once we support compression
     if compression_byte != 0:
@@ -39,14 +43,15 @@
     message_length = struct.unpack_from(">I", payload[1:])[0]
     if len(payload) != HEADER_LEN + message_length:
         return False
     return True
 
 
 def decode_grpc(payload):
+    # type: (bytes) -> Tuple[bytes, str]
     """Decode GRPC. Return the protobuf data"""
     if six.PY2 and isinstance(payload, bytearray):
         payload = bytes(payload)
     if len(payload) < HEADER_LEN:
         raise BlackboxProtobufException(
             "Error decoding GRPC, payload is not long enough: %d" % len(payload)
         )
@@ -74,14 +79,15 @@
 
     data = payload[HEADER_LEN:]
 
     return data, "grpc"
 
 
 def encode_grpc(data, encoding="grpc"):
+    # type: (bytes, str) -> bytes
     if encoding != "grpc":
         raise BlackboxProtobufException(
             "Error encoding GRPC with encoding %s. GRPC is only supported with no compression"
             % encoding
         )
 
     payload = bytearray()
```

### Comparing `bbpb-1.2.0/blackboxprotobuf/lib/payloads/gzip.py` & `bbpb-1.3.1/blackboxprotobuf/lib/payloads/gzip.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,28 +16,35 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import zlib
 
-
 from blackboxprotobuf.lib.exceptions import BlackboxProtobufException
 
+import six
+
+if six.PY3:
+    from typing import Tuple
+
 
 def is_gzip(buf):
+    # type: (bytes) -> bool
     return buf.startswith(bytearray([0x1F, 0x8B, 0x08]))
 
 
 def decode_gzip(buf):
+    # type: (bytes) -> Tuple[bytes, str]
     if buf.startswith(bytearray([0x1F, 0x8B, 0x08])):
         decompressor = zlib.decompressobj(31)
         return decompressor.decompress(buf), "gzip"
     else:
         raise BlackboxProtobufException(
             "Cannot decode as gzip: magic bytes don't match"
         )
 
 
 def encode_gzip(buf):
+    # type: (bytes) -> bytes
     compressor = zlib.compressobj(-1, zlib.DEFLATED, 31)
     return compressor.compress(buf) + compressor.flush()
```

### Comparing `bbpb-1.2.0/blackboxprotobuf/lib/protofile.py` & `bbpb-1.3.1/blackboxprotobuf/lib/protofile.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,17 +21,28 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import io
 import re
 import logging
+import re
+import six
+
 from blackboxprotobuf.lib.exceptions import TypedefException, ProtofileException
 import blackboxprotobuf.lib.api
 
+if six.PY3:
+    import typing
+
+    if typing.TYPE_CHECKING:
+        from blackboxprotobuf.lib.config import Config
+        from typing import Any, TextIO, Tuple, Dict, Optional, List
+        from blackboxprotobuf.lib.pytypes import TypeDef, FieldDef
+
 PROTO_FILE_TYPE_MAP = {
     "uint": "uint64",
     "int": "int64",
     "sint": "sint64",
     "fixed32": "fixed32",
     "sfixed32": "sfixed32",
     "float": "float",
@@ -80,14 +91,15 @@
 # add packed types to the list
 for packable_type in PACKABLE_TYPES:
     packed_type = "packed_" + packable_type
     PROTO_FILE_TYPE_MAP[packed_type] = PROTO_FILE_TYPE_MAP[packable_type]
 
 
 def _print_message(message_name, typedef, output_file, depth=0):
+    # type: (str, TypeDef, TextIO, int) -> None
     indent = "  " * depth
     if not NAME_REGEX.match(message_name):
         raise TypedefException("Message name: %s is not valid" % message_name)
 
     # sort typedef for better looking output
     typedef = blackboxprotobuf.lib.api.sort_typedef(typedef)
 
@@ -108,15 +120,15 @@
 
         if "name" in field_typedef and field_typedef["name"] != "":
             field_name = field_typedef["name"]
             field_name = field_name.strip()
             if not NAME_REGEX.match(field_name):
                 field_name = None
         if field_name is None:
-            field_name = "field%s" % field_number
+            field_name = six.ensure_text("field%s" % field_number)
 
         if field_typedef["type"] == "message":
             # If we have multiple typedefs, this means is something like the Any
             # message, and has to be manually reparsed to each type
             if "alt_typedefs" in field_typedef:
                 proto_type = "bytes"
             else:
@@ -154,37 +166,36 @@
         )
 
     output_file.write(indent)
     output_file.write("}\n\n")
 
 
 def export_proto(typedef_map, output_filename=None, output_file=None, package=None):
+    # type: (Dict[str, TypeDef], Optional[str], Optional[TextIO], Optional[str]) -> str | None
     """Export the given type definitons as a '.proto' file. Typedefs are
     expected as a dictionary of {'message_name': typedef }
 
     Write to output_file or output_filename if provided, otherwise return a string
     output_filename will be overwritten if it exists
     """
-    return_string = False
     if output_filename is not None:
         output_file = io.open(output_filename, "w+")
 
     if output_file is None:
-        return_string = True
         output_file = io.StringIO()
 
     # preamble
     output_file.write('syntax = "proto3";\n\n')
     if package:
         output_file.write("package %s;\n\n" % package)
 
     for typedef_name, typedef in typedef_map.items():
         _print_message(typedef_name, typedef, output_file)
 
-    if return_string:
+    if isinstance(output_file, io.StringIO):
         return output_file.getvalue()
     # close the file if we opened it
     elif output_filename is not None:
         output_file.close()
     return None
 
 
@@ -194,15 +205,16 @@
 )
 SYNTAX_REGEX = re.compile(r'^ *syntax += +"(proto\d)" *;.*')
 ENUM_REGEX = re.compile(r"^ *enum +([a-zA-Z0-9_]+) *{.*")
 PACKAGE_REGEX = re.compile(r"^ *package +([a-zA-Z0-9_.]+) *;.*")
 
 
 def import_proto(config, input_string=None, input_filename=None, input_file=None):
-    typedef_map = {}
+    # type: (Config, Optional[str], Optional[str], Optional[TextIO]) -> Dict[str, TypeDef]
+    typedef_map = {}  # type: Dict[str, TypeDef]
     if input_string is not None:
         input_file = io.StringIO(input_string)
     if input_file is None and input_filename is not None:
         input_file = io.open(input_filename, "r")
     if input_file is None:
         raise ProtofileException(
             "No file provided to import_proto", filename=input_filename
@@ -214,34 +226,42 @@
     message_trees = []
     message_names = []
 
     line = input_file.readline()
     while line:
         line = line.strip()
 
-        if line.startswith("syntax") and SYNTAX_REGEX.match(line):
-            syntax_version = SYNTAX_REGEX.match(line).group(1)
-
-        elif line.startswith("package") and PACKAGE_REGEX.match(line):
-            package_prefix = PACKAGE_REGEX.match(line).group(1) + "."
+        if line.startswith("syntax"):
+            syntax_match = SYNTAX_REGEX.match(line)
+            if syntax_match:
+                syntax_version = syntax_match.group(1)
+
+        elif line.startswith("package"):
+            package_match = PACKAGE_REGEX.match(line)
+            if package_match:
+                package_prefix = package_match.group(1) + "."
 
         elif line.startswith("import"):
             logging.warning(
                 "Proto file has import which is not supported "
                 "by the parser. Ensure the imported files are "
                 "processed first: %s",
                 line,
             )
-        elif line.startswith("enum") and ENUM_REGEX.match(line):
-            enum_name = _parse_enum(line, input_file)
-            enum_names.append(enum_name)
-
-        elif line.startswith("message") and MESSAGE_START_REGEX.match(line):
-            message_tree = _preparse_message(line, input_file)
-            message_trees.append(message_tree)
+        elif line.startswith("enum"):
+            enum_match = ENUM_REGEX.match(line)
+            if enum_match:
+                enum_name = _parse_enum(enum_match, line, input_file)
+                enum_names.append(enum_name)
+
+        elif line.startswith("message"):
+            message_start_match = MESSAGE_START_REGEX.match(line)
+            if message_start_match:
+                message_tree = _preparse_message(message_start_match, line, input_file)
+                message_trees.append(message_tree)
 
         line = input_file.readline()
 
     for tree in message_trees:
         new_message_names, new_enum_names = _collect_names(package_prefix, tree)
         enum_names += new_enum_names
         message_names += new_message_names
@@ -259,60 +279,71 @@
             syntax_version == "proto3",
             config,
         )
 
     return typedef_map
 
 
-def _parse_enum(line, input_file):
+def _parse_enum(enum_match, line, input_file):
+    # type: (re.Match[str], str, TextIO) -> str
     """Parse an enum out of the file. Goes from enum declaration to next }
     Returns the enum's name
     """
-    enum_name = ENUM_REGEX.match(line).group(1)
+    enum_name = enum_match.group(1)
     # parse until the next '}'
     while "}" not in line:
         line = input_file.readline()
         if not line:
             raise ProtofileException("Did not find close of enum")
     return enum_name
 
 
-def _preparse_message(line, input_file):
+def _preparse_message(message_start_match, line, input_file):
+    # type: (re.Match[str], str, TextIO) -> Dict[str, Any]
+    # TODO Should put together better types than Any, but we'll stick with this
+    # for now
     """Parse out a message name and the lines that make it up"""
-    message_name = MESSAGE_START_REGEX.match(line).group(1)
+    message_name = message_start_match.group(1)
     message_lines = []
     inner_enums = []
     inner_messages = []
 
     while "}" not in line:
         line = input_file.readline()
         if not line:
             raise ProtofileException("Did not find close of message")
 
         line = line.strip()
-        if line.startswith("enum") and ENUM_REGEX.match(line):
-            enum_name = _parse_enum(line, input_file)
-            inner_enums.append(enum_name)
-
-        elif line.startswith("message") and MESSAGE_START_REGEX.match(line):
-            message_tree = _preparse_message(line, input_file)
-            inner_messages.append(message_tree)
+        if line.startswith("enum"):
+            enum_match = ENUM_REGEX.match(line)
+            if enum_match:
+                enum_name = _parse_enum(enum_match, line, input_file)
+                inner_enums.append(enum_name)
+
+        elif line.startswith("message"):
+            inner_message_start_match = MESSAGE_START_REGEX.match(line)
+            if inner_message_start_match:
+                message_tree = _preparse_message(
+                    inner_message_start_match, line, input_file
+                )
+                inner_messages.append(message_tree)
         # not an inner enum or message
         else:
             message_lines.append(line)
 
     return {
         "name": message_name,
         "data": message_lines,
         "enums": inner_enums,
         "inner_messages": inner_messages,
     }
 
 
 def _collect_names(prefix, message_tree):
+    # type: (str, Dict[str, Any]) -> Tuple[List[str], List[str]]
     message_names = []
     enum_names = []
 
     name = prefix + message_tree["name"]
     message_names.append(name)
     for enum_name in message_tree["enums"]:
         enum_names.append(prefix + enum_name)
@@ -320,26 +351,27 @@
         new_message_names, new_enum_names = _collect_names(name + ".", inner_message)
         message_names += new_message_names
         enum_names += new_enum_names
     return message_names, enum_names
 
 
 def _check_message_name(current_path, name, known_message_names, config):
+    # type: (str, str, List[str], Config) -> str | None
     # Verify message name against preparsed message names and global
     # known_messages
     # For example, if we have:
     #   Message.InnerMesage
     # referenced from:
     #    PackageA.Message2
     # we would look up:
     # PackageA.Message2.Message.InnerMessage
     # PackageA.Message.InnerMessage
     # should also work for enums
     if name in config.known_types:
-        return True
+        return name
     # search for anything under a common prefix in known_message_names
     logging.debug("Testing message name: %s", name)
 
     prefix_options = [""]
     for part in current_path.split("."):
         if part:
             prefix_options = [prefix_options[0] + part + "."] + prefix_options
@@ -361,14 +393,15 @@
     )
     return None
 
 
 def _parse_message(
     message_tree, typdef_map, known_message_names, enum_names, prefix, is_proto3, config
 ):
+    # type: (Dict[str, Any], Dict[str, TypeDef], List[str], List[str], str, bool, Config) -> None
     message_typedef = {}
     message_name = prefix + message_tree["name"]
     prefix = message_name + "."
     # parse the actual message fields
     for line in message_tree["data"]:
         # lines should already be stripped and should not have messages or enums
         # logging.debug("Line before assert: %s", line)
@@ -395,20 +428,21 @@
             is_proto3,
             config,
         )
 
 
 # parse a field into a dictionary for the typedef
 def _parse_field(match, known_message_names, enum_names, prefix, is_proto3, config):
-    typedef = {}
+    # type: (re.Match[str], List[str], List[str], str, bool, Config) -> Tuple[str, FieldDef]
+    typedef = {}  # type: FieldDef
 
     field_name = match.group(3)
     if not field_name:
         raise ProtofileException("Could not parse field name from line: %s" % match)
-    typedef["name"] = field_name
+    typedef["name"] = six.ensure_text(field_name)
     field_number = match.group(4)
     if not field_number:
         raise ProtofileException("Could not parse field number from line: %s" % match)
 
     # figure out repeated
     field_rule = match.group(1)
     is_repeated = False
```

### Comparing `bbpb-1.2.0/blackboxprotobuf/lib/types/__init__.py` & `bbpb-1.3.1/blackboxprotobuf/lib/types/__init__.py`

 * *Files identical despite different names*

### Comparing `bbpb-1.2.0/blackboxprotobuf/lib/types/fixed.py` & `bbpb-1.3.1/blackboxprotobuf/lib/types/fixed.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,113 +21,136 @@
 # SOFTWARE.
 
 import struct
 import binascii
 import six
 from blackboxprotobuf.lib.exceptions import DecoderException, EncoderException
 
+import six
+
+if six.PY3:
+    from typing import Any, Tuple
+
 
 # Generic functions for encoding/decoding structs based on the "struct" format
 def encode_struct(fmt, value):
+    # type: (str, Any) -> bytes
     """Generic method for encoding arbitrary python "struct" values"""
     try:
         return struct.pack(fmt, value)
     except struct.error as exc:
         six.raise_from(
             EncoderException(
                 "Error encoding value %r with format string %s" % (value, fmt)
             ),
             exc,
         )
 
 
 def decode_struct(fmt, buf, pos):
+    # type: (str, bytes, int) -> Tuple[Any, int]
     """Generic method for decoding arbitrary python "struct" values"""
     new_pos = pos + struct.calcsize(fmt)
     try:
         return struct.unpack(fmt, buf[pos:new_pos])[0], new_pos
     except struct.error as exc:
         six.raise_from(
             DecoderException(
-                "Error deocding format string %s from bytes: %s"
+                "Error deocding format string %s from bytes: %r"
                 % (fmt, binascii.hexlify(buf[pos:new_pos]))
             ),
             exc,
         )
 
 
 _fixed32_fmt = "<I"
 
+# Note on types: We use Any here for decoded objects. While we could manually
+# enforce individual types, we would have to do so via `typing.cast` anyway
+# because of `struct`. The Message type also has `Any` anyways.
+
 
 def encode_fixed32(value):
+    # type: (Any) -> bytes
     """Encode a single 32 bit fixed-size value"""
     return encode_struct(_fixed32_fmt, value)
 
 
 def decode_fixed32(buf, pos):
+    # type: (bytes, int) -> Tuple[Any, int]
     """Decode a single 32 bit fixed-size value"""
     return decode_struct(_fixed32_fmt, buf, pos)
 
 
 _sfixed32_fmt = "<i"
 
 
 def encode_sfixed32(value):
+    # type: (Any) -> bytes
     """Encode a single signed 32 bit fixed-size value"""
     return encode_struct(_sfixed32_fmt, value)
 
 
 def decode_sfixed32(buf, pos):
+    # type: (bytes, int) -> Tuple[Any, int]
     """Decode a single signed 32 bit fixed-size value"""
     return decode_struct(_sfixed32_fmt, buf, pos)
 
 
 _float_fmt = "<f"
 
 
 def encode_float(value):
+    # type: (Any) -> bytes
     """Encode a single 32 bit floating point value"""
     return encode_struct(_float_fmt, value)
 
 
 def decode_float(buf, pos):
+    # type: (bytes, int) -> Tuple[Any, int]
     """Decode a single 32 bit floating point value"""
     return decode_struct(_float_fmt, buf, pos)
 
 
 _fixed64_fmt = "<Q"
 
 
 def encode_fixed64(value):
+    # type: (Any) -> bytes
     """Encode a single 64 bit fixed-size value"""
     return encode_struct(_fixed64_fmt, value)
 
 
 def decode_fixed64(buf, pos):
+    # type: (bytes, int) -> Tuple[Any, int]
     """Decode a single 64 bit fixed-size value"""
     return decode_struct(_fixed64_fmt, buf, pos)
 
 
 _sfixed64_fmt = "<q"
 
 
 def encode_sfixed64(value):
+    # type: (Any) -> bytes
     """Encode a single signed 64 bit fixed-size value"""
     return encode_struct(_sfixed64_fmt, value)
 
 
 def decode_sfixed64(buf, pos):
+    # type: (bytes, int) -> Tuple[Any, int]
     """Decode a single signed 64 bit fixed-size value"""
     return decode_struct(_sfixed64_fmt, buf, pos)
 
 
 _double_fmt = "<d"
 
 
 def encode_double(value):
+    # type: (Any) -> bytes
     """Encode a single 64 bit floating point value"""
     return encode_struct(_double_fmt, value)
 
 
 def decode_double(buf, pos):
+    # type: (bytes, int) -> Tuple[Any, int]
     """Decode a single 64 bit floating point value"""
     return decode_struct(_double_fmt, buf, pos)
```

### Comparing `bbpb-1.2.0/blackboxprotobuf/lib/types/length_delim.py` & `bbpb-1.3.1/blackboxprotobuf/lib/types/length_delim.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,49 +22,67 @@
 
 import binascii
 import copy
 import sys
 import six
 import logging
 
+
 import blackboxprotobuf.lib
 from blackboxprotobuf.lib.types import varint, wiretypes
 from blackboxprotobuf.lib.exceptions import (
     EncoderException,
     DecoderException,
     TypedefException,
 )
 
+if six.PY3:
+    import typing
+
+    if typing.TYPE_CHECKING:
+        from blackboxprotobuf.lib.config import Config
+        from typing import Any, Callable, Dict, Tuple, Optional, List
+        from blackboxprotobuf.lib.pytypes import Message, TypeDef, FieldDef
+
 
 def encode_string(value):
+    # type: (Any) -> bytes
     """Encode a string as a length delimited byte array"""
     try:
         value = six.ensure_text(value)
     except TypeError as exc:
         six.raise_from(
             EncoderException("Error encoding string to message: %r" % value), exc
         )
     return encode_bytes(value)
 
 
 def encode_bytes(value):
+    # type: (Any) -> bytes
     """Encode a length delimited byte array"""
     if isinstance(value, bytearray):
         value = bytes(value)
     try:
         value = six.ensure_binary(value)
     except TypeError as exc:
         six.raise_from(
             EncoderException("Error encoding bytes to message: %r" % value), exc
         )
+
+    if not isinstance(value, bytes):
+        raise EncoderException(
+            "encode_bytes must receive a bytes or bytearray value: %s %r"
+            % (type(value), value)
+        )
     encoded_length = varint.encode_varint(len(value))
     return encoded_length + value
 
 
 def decode_bytes(buf, pos):
+    # type: (bytes, int) -> Tuple[bytes, int]
     """Decode a length delimited bytes array from buf"""
     length, pos = varint.decode_varint(buf, pos)
     end = pos + length
     try:
         return buf[pos:end], end
     except IndexError as exc:
         six.raise_from(
@@ -76,63 +94,69 @@
                 % (length, len(buf) - pos)
             ),
             exc,
         )
 
 
 def encode_bytes_hex(value):
+    # type: (Any) -> bytes
     """Encode a length delimited byte array represented by a hex string"""
     try:
         return encode_bytes(binascii.unhexlify(value))
     except (TypeError, binascii.Error) as exc:
         six.raise_from(
             EncoderException("Error encoding hex bytestring %s" % value), exc
         )
 
 
 def decode_bytes_hex(buf, pos):
+    # type: (bytes, int) -> Tuple[bytes, int]
     """Decode a length delimited byte array from buf and return a hex encoded string"""
     value, pos = decode_bytes(buf, pos)
     return binascii.hexlify(value), pos
 
 
 def decode_string(value, pos):
+    # type: (bytes, int) -> Tuple[str, int]
     """Decode a length delimited byte array as a string"""
     length, pos = varint.decode_varint(value, pos)
     end = pos + length
     try:
         # backslash escaping isn't reversible easily
         return value[pos:end].decode("utf-8"), end
     except (TypeError, UnicodeDecodeError) as exc:
         six.raise_from(
-            DecoderException("Error decoding UTF-8 string %s" % value[pos:end]), exc
+            DecoderException("Error decoding UTF-8 string %r" % value[pos:end]), exc
         )
 
 
 def encode_tag(field_number, wire_type):
+    # type: (int, int) -> bytes
     # Not checking bounds here, should be check before
     tag_number = (field_number << 3) | wire_type
     return varint.encode_uvarint(tag_number)
 
 
 def decode_tag(buf, pos):
+    # type: (bytes, int) -> Tuple[int, int, int]
     tag_number, pos = varint.decode_uvarint(buf, pos)
     field_number = tag_number >> 3
     wire_type = tag_number & 0x7
     return field_number, wire_type, pos
 
 
 def encode_message(data, config, typedef, path=None, field_order=None):
+    # type: (Message, Config, TypeDef, Optional[List[str]], Optional[List[str]]) -> bytes
     """Encode a Python dictionary to a binary protobuf message"""
     output = bytearray()
     if path is None:
         path = []
 
     output_len = 0
-    field_outputs = {}
+    field_outputs = {}  # type: Dict[str, List[bytes]]
     for field_id, value in data.items():
         field_number, outputs = _encode_message_field(
             config, typedef, path, field_id, value
         )
 
         # In case the field number is represented in multiple locations in data
         # (eg. as an int, as name, as a string with an int)
@@ -174,49 +198,45 @@
             for value in values:
                 output += value
 
     return output
 
 
 def _encode_message_field(config, typedef, path, field_id, value):
+    # type: (Config, TypeDef, List[str], str | int, Any) -> Tuple[str, List[bytes]]
     # Get the field number convert it as necessary
     alt_field_number = None
 
-    if six.PY2:
-        string_types = (str, unicode)
-    else:
-        string_types = str
-
     field_number = None
     # Convert the field_id, which could be a number or a name, into a field number
     # From a correctness standpoint, field_number should probably be an int
     # type, but IIRC that leads to headaches elsewhere
-    if isinstance(field_id, string_types):
+    if isinstance(field_id, six.text_type):
         if "-" in field_id:
             field_id, alt_field_number = field_id.split("-")
         if field_id.isdigit():
             field_number = field_id
         else:
             for number, info in typedef.items():
                 if (
                     info.get("name", "") != ""
                     and info["name"] == field_id
                     and field_id != ""
                 ):
                     field_number = number
                     break
     else:
-        field_number = str(field_id)
+        field_number = six.ensure_text(str(field_id))
 
     field_path = path[:]
-    field_path.append(field_id)
+    field_path.append(str(field_number))
 
     if field_number is None or field_number not in typedef:
         raise EncoderException(
-            "Provided field name/number %s / $s is not valid"
+            "Provided field name/number %s / %s is not valid"
             % (field_id, field_number),
             field_path,
         )
 
     field_typedef = typedef[field_number]
 
     # Get encoder
@@ -224,35 +244,34 @@
         raise TypedefException(
             "Field %s does not have a defined type." % field_number, field_path
         )
 
     field_type = field_typedef["type"]
     field_order = field_typedef.get("field_order", None)
 
-    field_encoder = None
+    field_encoder = None  # type: Callable[[Any], bytes] | None
     if alt_field_number is not None:
         if alt_field_number not in field_typedef["alt_typedefs"]:
             raise EncoderException(
                 "Provided alt field name/number %s is not valid for field_number %s"
                 % (alt_field_number, field_number),
                 field_path,
             )
-        if isinstance(field_typedef["alt_typedefs"][alt_field_number], dict):
-            innertypedef = field_typedef["alt_typedefs"][alt_field_number]
+        alt_field_type = field_typedef["alt_typedefs"][alt_field_number]
+        if isinstance(alt_field_type, six.text_type):
+            # just let the field
+            field_type = alt_field_type
+        else:
+            innertypedef = alt_field_type
             field_encoder = lambda data: encode_lendelim_message(
                 data, config, innertypedef, path=field_path, field_order=field_order
             )
 
-        else:
-            # just let the field
-            field_type = field_typedef["alt_typedefs"][alt_field_number]
-
     if field_encoder is None:
         if field_type == "message":
-            innertypedef = None
             if "message_typedef" in field_typedef:
                 innertypedef = field_typedef["message_typedef"]
             elif "message_type_name" in field_typedef:
                 message_type_name = field_typedef["message_type_name"]
                 if message_type_name not in config.known_types:
                     raise TypedefException(
                         "Message type (%s) has not been defined"
@@ -298,28 +317,29 @@
         exc.set_path(field_path)
         six.reraise(*sys.exc_info())
 
     return field_number, outputs
 
 
 def decode_message(buf, config, typedef=None, pos=0, end=None, depth=0, path=None):
+    # type: (bytes, Config, Optional[TypeDef], int, Optional[int], int, Optional[List[str]]) -> Tuple[Message, TypeDef, List[str], int]
     """Decode a protobuf message with no length prefix"""
     if end is None:
         end = len(buf)
 
     if typedef is None:
         typedef = {}
     else:
         # Don't want to accidentally modify the original
         typedef = copy.deepcopy(typedef)
 
     if path is None:
         path = []
 
-    output = {}
+    output = {}  # type: Message
 
     grouped_fields, field_order, pos = _group_by_number(buf, pos, end, path)
     for field_number, (wire_type, buffers) in grouped_fields.items():
         # wire_type should already be validated by _group_by_number
 
         path = path[:] + [field_number]
         field_outputs = None
@@ -385,40 +405,41 @@
         # Save the field typedef/type back to the typedef
         typedef[field_number] = field_typedef
 
     return output, typedef, field_order, pos
 
 
 def _group_by_number(buf, pos, end, path):
+    # type: (bytes, int, int, List[str]) -> Tuple[Dict[str, Tuple[int, List[bytes]]], List[str], int]
     # Parse through the whole message and split into buffers based on wire
     # type and organized by field number. This forces us to parse the whole
     # message at once, but I think we're doing that anyway. This catches size
     # errors early as well, which is usually the best indicator of if it's a
     # protobuf message or not.
     # Returns a dictionary like:
     #     {
     #         "2": (<wiretype>, [<data>])
     #     }
 
-    output_map = {}
+    output_map = {}  # type: Dict[str, Tuple[int, List[bytes]]]
     field_order = []
     while pos < end:
         # Read in a field
         field_number, wire_type, pos = decode_tag(buf, pos)
 
         # We want field numbers as strings everywhere
-        field_number = str(field_number)
+        field_id = six.ensure_text(str(field_number))
 
-        field_path = path[:] + [field_number]
+        field_path = path[:] + [field_id]
 
-        if field_number in output_map and output_map[field_number][0] != wire_type:
+        if field_id in output_map and output_map[field_id][0] != wire_type:
             # This should never happen
             raise DecoderException(
                 "Field %s has mistmatched wiretypes. Previous: %s Now: %s"
-                % (field_number, output_map[field_number][0], wire_type),
+                % (field_id, output_map[field_id][0], wire_type),
                 path=field_path,
             )
 
         length = None
         if wire_type == wiretypes.VARINT:
             # We actually have to read in the whole varint to figure out it's size
             _, new_pos = varint.decode_uvarint(buf, pos)
@@ -440,35 +461,36 @@
         else:
             raise DecoderException(
                 "Got unknown wire type: %d" % wire_type, path=field_path
             )
         if pos + length > end:
             raise DecoderException(
                 "Decoded length for field %s goes over end: %d > %d"
-                % (field_number, pos + length, end),
+                % (field_id, pos + length, end),
                 path=field_path,
             )
 
         field_buf = buf[pos : pos + length]
 
-        if field_number in output_map:
-            output_map[field_number][1].append(field_buf)
+        if field_id in output_map:
+            output_map[field_id][1].append(field_buf)
         else:
-            output_map[field_number] = (wire_type, [field_buf])
-        field_order.append(field_number)
+            output_map[field_id] = (wire_type, [field_buf])
+        field_order.append(field_id)
         pos += length
     return output_map, field_order, pos
 
 
 def _get_field_key(field_number, typedef, path):
+    # type: (str | int, TypeDef, List[str]) -> str
     # Translate a field_number into a name if one is available in the typedef
-    if not isinstance(field_number, (int, str)):
+    if not isinstance(field_number, (int, six.text_type)):
         raise EncoderException("Field key in message must be a str or int", path=path)
     if isinstance(field_number, int):
-        field_number = str(field_number)
+        field_number = six.ensure_text(str(field_number))
 
     # handle an alt_typedef by transforming 1-1 to name-1
     # I don't think should actually be used with the current uses of
     # _get_field_key
     alt_field_number = None
     if "-" in field_number:
         field_number, alt_field_number = field_number.split("-")
@@ -480,14 +502,17 @@
     # Return the new field_name + alt_field_number
     return field_key + ("" if alt_field_number is None else "-" + alt_field_number)
 
 
 def _try_decode_lendelim_fields(
     buffers, field_key, field_typedef, message_output, config
 ):
+    # type: (List[bytes], str, FieldDef, Message, Config) -> None
+    # Mutates message_output
+
     # This is where things get weird
     # To start, since we want to decode messages and not treat every
     # embedded message as bytes, we have to guess if it's a message or
     # not.
     # Unlike other types, we can't assume our message types are
     # consistent across the tree or even within the same message.
     # A field could be a bytes type that that decodes to multiple different
@@ -498,30 +523,30 @@
     # and we can enforce that across a single message, but not multiple
     # messages.
     # This is going to change the definition of "alt_typedefs" a bit from just
     # alternate message type definitions to also allowing downgrading to
     # 'bytes' or string with an 'alt_type' if it doesn't parse
 
     try:
-        outputs_map = {}
-        field_order = []
+        outputs_map = {}  # type: Dict[str, Any]
+        field_order = []  # type: List[str]
         # grab all dictonary alt_typedefs
         all_typedefs = {
             # we don't want this to modify in-place if it fails
             key: copy.deepcopy(value)
             for key, value in field_typedef.get("alt_typedefs", {}).items()
             if isinstance(value, dict)
-        }
+        }  # type: Dict[str, TypeDef]
         all_typedefs["1"] = copy.deepcopy(field_typedef.get("message_typedef", {}))
 
         for buf in buffers:
             output = None
             output_typedef = None
             output_typedef_num = None
-            new_field_order = []
+            new_field_order = []  # type: List[str]
             for alt_typedef_num, alt_typedef in sorted(
                 all_typedefs.items(), key=lambda x: int(x[0])
             ):
                 try:
                     (
                         output,
                         output_typedef,
@@ -534,18 +559,22 @@
                 break
             # try an anonymous type
             # let the error propogate up if we fail this
             if output is None:
                 output, output_typedef, new_field_order, _ = decode_lendelim_message(
                     buf, config, {}
                 )
-                output_typedef_num = str(
-                    max([int(i) for i in ["0"] + list(all_typedefs.keys())]) + 1
+                output_typedef_num = six.ensure_text(
+                    str(max([int(i) for i in ["0"] + list(all_typedefs.keys())]) + 1)
                 )
 
+            if output_typedef is None or output_typedef_num is None:
+                raise DecoderException(
+                    "Could not find an output_typedef or output_typedef_num. This should not happen under any circumstances."
+                )
             # save the output or typedef we found
             all_typedefs[output_typedef_num] = output_typedef
             output_list = outputs_map.get(output_typedef_num, [])
             output_list.append(output)
             outputs_map[output_typedef_num] = output_list
 
             # we should technically have a different field order for each instance of the data
@@ -595,26 +624,28 @@
 
             # all outputs worked, this is our type
             # check if there is a message type already in the typedef
             if "type" in field_typedef and "message" == field_typedef["type"]:
                 # we already had a message type. save it as an alt_typedef
 
                 # check if we already have this type as an alt_typedef
-                output_typedef_nums = {
-                    key: value
+                output_typedef_nums = [
+                    key
                     for key, value in field_typedef.setdefault(
                         "alt_typedefs", {}
                     ).items()
                     if value == target_type
-                }.keys()
+                ]
                 output_typedef_num = None
                 if len(output_typedef_nums) == 0:
                     # find the next largest alt typedef number to put this type as
-                    output_typedef_num = str(
-                        max([int(i) for i in ["0"] + all_typedefs.keys()]) + 1
+                    output_typedef_num = six.ensure_text(
+                        str(
+                            max([int(i) for i in ["0"] + list(all_typedefs.keys())]) + 1
+                        )
                     )
                     field_typedef.setdefault("alt_typedefs", {})[
                         output_typedef_num
                     ] = target_type
                 else:
                     # we already have an alt typedef with this number
                     output_typedef_num = output_typedef_nums[0]
@@ -626,50 +657,56 @@
                 message_output[field_key] = outputs if len(outputs) > 1 else outputs[0]
             return
         except DecoderException:
             continue
 
 
 def encode_lendelim_message(data, config, typedef, path=None, field_order=None):
+    # type: (Message, Config, TypeDef, Optional[List[str]], Optional[List[str]]) -> bytes
     """Encode data as a length delimited protobuf message"""
     message_out = encode_message(
         data, config, typedef, path=path, field_order=field_order
     )
     length = varint.encode_varint(len(message_out))
     logging.debug("Message length encoded: %d", len(length) + len(message_out))
     return length + message_out
 
 
 def decode_lendelim_message(buf, config, typedef=None, pos=0, depth=0, path=None):
+    # type: (bytes, Config, Optional[TypeDef], int, int, Optional[List[str]]) -> Tuple[Message, TypeDef, List[str], int]
     """Deocde a length delimited protobuf message from buf"""
     length, pos = varint.decode_varint(buf, pos)
     ret = decode_message(
         buf, config, typedef, pos, pos + length, depth=depth, path=path
     )
     return ret
 
 
 def generate_packed_encoder(wrapped_encoder):
+    # type: (Callable[[Any], bytes]) -> Callable[[List[Any]], bytes]
     """Generate an encoder for a packed type based on a base type encoder"""
 
     def length_wrapper(values):
+        # type: (List[Any]) -> bytes
         # Encode repeat values and prefix with the length
         output = bytearray()
         for value in values:
             output += wrapped_encoder(value)
         length = varint.encode_varint(len(output))
         return length + output
 
     return length_wrapper
 
 
 def generate_packed_decoder(wrapped_decoder):
+    # type: (Callable[[bytes, int], Tuple[Any, int]]) -> Callable[[bytes, int], Tuple[List[Any], int]]
     """Generate an decoder for a packed type based on a base type decoder"""
 
     def length_wrapper(buf, pos):
+        # type: (bytes, int) -> Tuple[List[Any], int]
         # Decode repeat values prefixed with the length
         length, pos = varint.decode_varint(buf, pos)
         end = pos + length
         output = []
         while pos < end:
             value, pos = wrapped_decoder(buf, pos)
             output.append(value)
```

### Comparing `bbpb-1.2.0/blackboxprotobuf/lib/types/type_maps.py` & `bbpb-1.3.1/blackboxprotobuf/lib/types/type_maps.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,19 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from blackboxprotobuf.lib.types import varint, fixed, length_delim, wiretypes
 
+import six
+
+if six.PY3:
+    from typing import Any, Callable, Dict, Tuple
+
 # Map a blackboxprotobuf type to specific encoder
 ENCODERS = {
     "uint": varint.encode_uvarint,
     "int": varint.encode_varint,
     "sint": varint.encode_svarint,
     "fixed32": fixed.encode_fixed32,
     "sfixed32": fixed.encode_sfixed32,
@@ -43,15 +48,15 @@
     "packed_sint": length_delim.generate_packed_encoder(varint.encode_svarint),
     "packed_fixed32": length_delim.generate_packed_encoder(fixed.encode_fixed32),
     "packed_sfixed32": length_delim.generate_packed_encoder(fixed.encode_sfixed32),
     "packed_float": length_delim.generate_packed_encoder(fixed.encode_float),
     "packed_fixed64": length_delim.generate_packed_encoder(fixed.encode_fixed64),
     "packed_sfixed64": length_delim.generate_packed_encoder(fixed.encode_sfixed64),
     "packed_double": length_delim.generate_packed_encoder(fixed.encode_double),
-}
+}  # type: Dict[str, Callable[[Any], bytes]]
 
 # Map a blackboxprotobuf type to specific decoder
 DECODERS = {
     "uint": varint.decode_uvarint,
     "int": varint.decode_varint,
     "sint": varint.decode_svarint,
     "fixed32": fixed.decode_fixed32,
@@ -68,15 +73,15 @@
     "packed_sint": length_delim.generate_packed_decoder(varint.decode_svarint),
     "packed_fixed32": length_delim.generate_packed_decoder(fixed.decode_fixed32),
     "packed_sfixed32": length_delim.generate_packed_decoder(fixed.decode_sfixed32),
     "packed_float": length_delim.generate_packed_decoder(fixed.decode_float),
     "packed_fixed64": length_delim.generate_packed_decoder(fixed.decode_fixed64),
     "packed_sfixed64": length_delim.generate_packed_decoder(fixed.decode_sfixed64),
     "packed_double": length_delim.generate_packed_decoder(fixed.decode_double),
-}
+}  # type: Dict[str, Callable[[bytes, int], Tuple[Any, int]  ]]
 
 WIRETYPES = {
     "uint": wiretypes.VARINT,
     "int": wiretypes.VARINT,
     "sint": wiretypes.VARINT,
     "fixed32": wiretypes.FIXED32,
     "sfixed32": wiretypes.FIXED32,
@@ -94,19 +99,19 @@
     "packed_sint": wiretypes.LENGTH_DELIMITED,
     "packed_fixed32": wiretypes.LENGTH_DELIMITED,
     "packed_sfixed32": wiretypes.LENGTH_DELIMITED,
     "packed_float": wiretypes.LENGTH_DELIMITED,
     "packed_fixed64": wiretypes.LENGTH_DELIMITED,
     "packed_sfixed64": wiretypes.LENGTH_DELIMITED,
     "packed_double": wiretypes.LENGTH_DELIMITED,
-}
+}  # type: Dict[str, int]
 
 # Default values to use when decoding each wire type
 # length delimited is special and handled in the length_delim module
 WIRE_TYPE_DEFAULTS = {
     wiretypes.VARINT: "int",
     wiretypes.FIXED32: "fixed32",
     wiretypes.FIXED64: "fixed64",
     wiretypes.LENGTH_DELIMITED: None,
     wiretypes.START_GROUP: None,
     wiretypes.END_GROUP: None,
-}
+}  # type: Dict[int, str | None]
```

### Comparing `bbpb-1.2.0/blackboxprotobuf/lib/types/varint.py` & `bbpb-1.3.1/blackboxprotobuf/lib/types/varint.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,25 +22,31 @@
 
 import binascii
 import struct
 import six
 
 from blackboxprotobuf.lib.exceptions import EncoderException, DecoderException
 
+if six.PY3:
+    from typing import Any, Tuple
+
 # These are set in decoder.py
 # In theory, uvarints and zigzag varints shouldn't have a max
 # But this is enforced by protobuf
 MAX_UVARINT = (1 << 64) - 1
 MIN_UVARINT = 0
 MAX_SVARINT = (1 << 63) - 1
 MIN_SVARINT = -(1 << 63)
 
 
 def encode_uvarint(value):
+    # type: (Any) -> bytes
     """Encode a long or int into a bytearray."""
+    if not isinstance(value, six.integer_types):
+        raise EncoderException("Got non-int type for uvarint encoding: %s" % value)
     output = bytearray()
     if value < MIN_UVARINT:
         raise EncoderException(
             "Error encoding %d as uvarint. Value must be positive" % value
         )
     if value > MAX_UVARINT:
         raise EncoderException(
@@ -58,14 +64,15 @@
                 next_byte |= 0x80
             output.append(next_byte)
 
     return output
 
 
 def decode_uvarint(buf, pos):
+    # type: (bytes, int) -> Tuple[int, int]
     """Decode bytearray into a long."""
     pos_start = pos
     # Convert buffer to string
     if six.PY2:
         buf = bytes(buf)
 
     try:
@@ -88,23 +95,26 @@
     except EncoderException as ex:
         raise DecoderException(
             "Error decoding uvarint: value (%s) was not able to be re-encoded: %s"
             % (value, ex)
         )
     if buf[pos_start:pos] != test_encode:
         raise DecoderException(
-            "Error decoding uvarint: Encoding is not standard:\noriginal:  %s\nstandard: %s"
+            "Error decoding uvarint: Encoding is not standard:\noriginal:  %r\nstandard: %r"
             % (buf[pos_start:pos], test_encode)
         )
 
     return (value, pos)
 
 
 def encode_varint(value):
+    # type: (Any) -> bytes
     """Encode a long or int into a bytearray."""
+    if not isinstance(value, six.integer_types):
+        raise EncoderException("Got non-int type for varint encoding: %s" % value)
     if value > MAX_SVARINT:
         raise EncoderException(
             "Error encoding %d as varint. Value must be <= %s" % (value, MAX_SVARINT)
         )
     if value < MIN_SVARINT:
         raise EncoderException(
             "Error encoding %d as varint. Value must be >= %s" % (value, MIN_SVARINT)
@@ -112,14 +122,15 @@
     if value < 0:
         value += 1 << 64
     output = encode_uvarint(value)
     return output
 
 
 def decode_varint(buf, pos):
+    # type: (bytes, int) -> Tuple[int, int]
     """Decode bytearray into a long."""
     # Convert buffer to string
     pos_start = pos
     if six.PY2:
         buf = bytes(buf)
 
     value, pos = decode_uvarint(buf, pos)
@@ -133,56 +144,62 @@
         raise DecoderException(
             "Error decoding varint: value (%s) was not able to be re-encoded: %s"
             % (value, ex)
         )
 
     if buf[pos_start:pos] != test_encode:
         raise DecoderException(
-            "Error decoding varint: Encoding is not standard:\noriginal:  %s\nstandard: %s"
+            "Error decoding varint: Encoding is not standard:\noriginal:  %r\nstandard: %r"
             % (buf[pos_start:pos], test_encode)
         )
     return (value, pos)
 
 
 def encode_zig_zag(value):
+    # type: (int) -> int
     if value < 0:
         return (abs(value) << 1) - 1
     return value << 1
 
 
 def decode_zig_zag(value):
+    # type: (int) -> int
     if value & 0x1:
         # negative
         return -((value + 1) >> 1)
     return value >> 1
 
 
 def encode_svarint(value):
+    # type: (Any) -> bytes
     """Zigzag encode the potentially signed value prior to encoding"""
+    if not isinstance(value, six.integer_types):
+        raise EncoderException("Got non-int type for svarint encoding: %s" % value)
     # zigzag encode value
     if value > MAX_SVARINT:
         raise EncoderException(
             "Error encoding %d as svarint. Value must be <= %s" % (value, MAX_SVARINT)
         )
     if value < MIN_SVARINT:
         raise EncoderException(
             "Error encoding %d as svarint. Value must be >= %s" % (value, MIN_SVARINT)
         )
     return encode_uvarint(encode_zig_zag(value))
 
 
 def decode_svarint(buf, pos):
+    # type: (bytes, int) -> Tuple[int, int]
     """Decode bytearray into a long."""
     pos_start = pos
 
     output, pos = decode_uvarint(buf, pos)
     value = decode_zig_zag(output)
 
     # Validate that this is a cononical encoding by re-encoding the value
     test_encode = encode_svarint(value)
     if buf[pos_start:pos] != test_encode:
         raise DecoderException(
-            "Error decoding svarint: Encoding is not standard:\noriginal:  %s\nstandard: %s"
+            "Error decoding svarint: Encoding is not standard:\noriginal:  %r\nstandard: %r"
             % (buf[pos_start:pos], test_encode)
         )
 
     return value, pos
```

### Comparing `bbpb-1.2.0/blackboxprotobuf/lib/types/wiretypes.py` & `bbpb-1.3.1/blackboxprotobuf/lib/types/wiretypes.py`

 * *Files identical despite different names*

### Comparing `bbpb-1.2.0/pyproject.toml` & `bbpb-1.3.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bbpb"
-version = "1.2.0"
+version = "1.3.1"
 description = "Library for working with protobuf messages without a protobuf type definition."
 authors = ["Ryan Winkelmaier <ryan.winkelmaier@nccgroup.com>"]
 license = "MIT"
 repository = "https://github.com/nccgroup/blackboxprotobuf"
 readme = "README.md"
 keywords = ["protobuf"]
 exclude = ["./tests"]
@@ -19,10 +19,16 @@
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.4.2"
 hypothesis = "^6.31.6"
 black = "^23.9.1"
 protobuf = "^3.20"
 
+[tool.poetry.group.dev.dependencies]
+mypy = "^1.10.0"
+
+[tool.poetry.scripts]
+bbpb = "blackboxprotobuf.__main__:main"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `bbpb-1.2.0/PKG-INFO` & `bbpb-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbpb
-Version: 1.2.0
+Version: 1.3.1
 Summary: Library for working with protobuf messages without a protobuf type definition.
 Home-page: https://github.com/nccgroup/blackboxprotobuf
 License: MIT
 Keywords: protobuf
 Author: Ryan Winkelmaier
 Author-email: ryan.winkelmaier@nccgroup.com
 Requires-Python: >=3.8,<4.0
@@ -59,32 +59,30 @@
 re-encode the data. In general, most fields of interest are likely to be parsed
 into a usable form. Users can optionally pass in custom type definitions that
 override the guessed type. Custom type definitions also allow naming of fields to
 improve user friendliness.
 
 # Usage
 ## Installation    
-This library depends on internal functions of Google's protobuf Python library
-to do some encoding/decoding of individual fields and six for python 2
-compatibility.
-
 The package can be installed from source with:
 
 ```
 poetry install
 ```
 
 BlackBox Protobuf is also available on PyPi at <https://pypi.org/project/bbpb>.
 It can be installed with:
 
 ```
 pip install bbpb
 ```
 
 ## CLI
+The package defines a `bbpb` command for command line encoding/decoding.
+
 For command line usage see [CLI.md](./CLI.md).
 
 ## Interface
 The main `blackboxprotobuf` module defines an API with the core encode/decode
 message functions, along with several convenience functions to make it easier
 to use blackboxprotobuf with a user interface, such as encoding/decoding
 directly to JSON and validating modified type definitions.
```

