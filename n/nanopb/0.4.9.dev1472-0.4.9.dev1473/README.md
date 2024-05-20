# Comparing `tmp/nanopb-0.4.9.dev1472.tar.gz` & `tmp/nanopb-0.4.9.dev1473.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanopb-0.4.9.dev1472.tar", max compression
+gzip compressed data, was "nanopb-0.4.9.dev1473.tar", max compression
```

## Comparing `nanopb-0.4.9.dev1472.tar` & `nanopb-0.4.9.dev1473.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     4461 2024-05-06 13:53:00.000000 nanopb-0.4.9.dev1472/README.md
--rw-r--r--   0        0        0        0 2024-05-13 02:09:03.941521 nanopb-0.4.9.dev1472/nanopb/__init__.py
--rw-r--r--   0        0        0        0 2024-05-13 02:09:03.941521 nanopb-0.4.9.dev1472/nanopb/generator/__init__.py
--rwxr-xr-x   0        0        0      235 2024-05-06 13:53:00.000000 nanopb-0.4.9.dev1472/nanopb/generator/nanopb_generator
--rw-r--r--   0        0        0      206 2024-05-06 13:53:00.000000 nanopb-0.4.9.dev1472/nanopb/generator/nanopb_generator.bat
--rwxr-xr-x   0        0        0   112055 2024-05-06 13:53:00.000000 nanopb-0.4.9.dev1472/nanopb/generator/nanopb_generator.py
--rwxr-xr-x   0        0        0      460 2024-05-06 13:53:00.000000 nanopb-0.4.9.dev1472/nanopb/generator/nanopb_generator.py2
--rw-r--r--   0        0        0     5839 2024-05-06 13:53:00.000000 nanopb-0.4.9.dev1472/nanopb/generator/platformio_generator.py
--rw-r--r--   0        0        0      126 2024-05-06 13:53:00.000000 nanopb-0.4.9.dev1472/nanopb/generator/proto/Makefile
--rw-r--r--   0        0        0     4629 2024-05-06 13:53:00.000000 nanopb-0.4.9.dev1472/nanopb/generator/proto/__init__.py
--rw-r--r--   0        0        0     3376 2024-05-13 02:09:03.961521 nanopb-0.4.9.dev1472/nanopb/generator/proto/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2804 2024-05-13 02:09:04.033520 nanopb-0.4.9.dev1472/nanopb/generator/proto/__pycache__/_utils.cpython-38.pyc
--rw-r--r--   0        0        0     2949 2024-05-06 13:53:00.000000 nanopb-0.4.9.dev1472/nanopb/generator/proto/_utils.py
--rw-r--r--   0        0        0    36277 2024-05-06 13:53:00.000000 nanopb-0.4.9.dev1472/nanopb/generator/proto/google/protobuf/descriptor.proto
--rw-r--r--   0        0        0     7139 2024-05-06 13:53:00.000000 nanopb-0.4.9.dev1472/nanopb/generator/proto/nanopb.proto
--rw-r--r--   0        0        0     4445 2024-05-13 02:09:04.045520 nanopb-0.4.9.dev1472/nanopb/generator/proto/nanopb_pb2.py
--rwxr-xr-x   0        0        0     1577 2024-05-06 13:53:00.000000 nanopb-0.4.9.dev1472/nanopb/generator/protoc
--rwxr-xr-x   0        0        0      374 2024-05-06 13:53:00.000000 nanopb-0.4.9.dev1472/nanopb/generator/protoc-gen-nanopb
--rwxr-xr-x   0        0        0      554 2024-05-06 13:53:00.000000 nanopb-0.4.9.dev1472/nanopb/generator/protoc-gen-nanopb-py2
--rw-r--r--   0        0        0      449 2024-05-06 13:53:00.000000 nanopb-0.4.9.dev1472/nanopb/generator/protoc-gen-nanopb.bat
--rw-r--r--   0        0        0      302 2024-05-06 13:53:00.000000 nanopb-0.4.9.dev1472/nanopb/generator/protoc.bat
--rw-r--r--   0        0        0     1065 2024-05-13 02:09:04.065520 nanopb-0.4.9.dev1472/pyproject.toml
--rw-r--r--   0        0        0     5848 1970-01-01 00:00:00.000000 nanopb-0.4.9.dev1472/PKG-INFO
+-rw-r--r--   0        0        0     4461 2024-05-15 16:50:13.000000 nanopb-0.4.9.dev1473/README.md
+-rw-r--r--   0        0        0        0 2024-05-20 02:08:22.397021 nanopb-0.4.9.dev1473/nanopb/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-20 02:08:22.397021 nanopb-0.4.9.dev1473/nanopb/generator/__init__.py
+-rwxr-xr-x   0        0        0      235 2024-05-15 16:50:13.000000 nanopb-0.4.9.dev1473/nanopb/generator/nanopb_generator
+-rw-r--r--   0        0        0      206 2024-05-15 16:50:13.000000 nanopb-0.4.9.dev1473/nanopb/generator/nanopb_generator.bat
+-rwxr-xr-x   0        0        0   112249 2024-05-15 16:50:13.000000 nanopb-0.4.9.dev1473/nanopb/generator/nanopb_generator.py
+-rwxr-xr-x   0        0        0      460 2024-05-15 16:50:13.000000 nanopb-0.4.9.dev1473/nanopb/generator/nanopb_generator.py2
+-rw-r--r--   0        0        0     5839 2024-05-15 16:50:13.000000 nanopb-0.4.9.dev1473/nanopb/generator/platformio_generator.py
+-rw-r--r--   0        0        0      126 2024-05-15 16:50:13.000000 nanopb-0.4.9.dev1473/nanopb/generator/proto/Makefile
+-rw-r--r--   0        0        0     4629 2024-05-15 16:50:13.000000 nanopb-0.4.9.dev1473/nanopb/generator/proto/__init__.py
+-rw-r--r--   0        0        0     3376 2024-05-20 02:08:22.413021 nanopb-0.4.9.dev1473/nanopb/generator/proto/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2804 2024-05-20 02:08:22.485020 nanopb-0.4.9.dev1473/nanopb/generator/proto/__pycache__/_utils.cpython-38.pyc
+-rw-r--r--   0        0        0     2949 2024-05-15 16:50:13.000000 nanopb-0.4.9.dev1473/nanopb/generator/proto/_utils.py
+-rw-r--r--   0        0        0    36277 2024-05-15 16:50:13.000000 nanopb-0.4.9.dev1473/nanopb/generator/proto/google/protobuf/descriptor.proto
+-rw-r--r--   0        0        0     7437 2024-05-15 16:50:13.000000 nanopb-0.4.9.dev1473/nanopb/generator/proto/nanopb.proto
+-rw-r--r--   0        0        0     4539 2024-05-20 02:08:22.497020 nanopb-0.4.9.dev1473/nanopb/generator/proto/nanopb_pb2.py
+-rwxr-xr-x   0        0        0     1577 2024-05-15 16:50:13.000000 nanopb-0.4.9.dev1473/nanopb/generator/protoc
+-rwxr-xr-x   0        0        0      374 2024-05-15 16:50:13.000000 nanopb-0.4.9.dev1473/nanopb/generator/protoc-gen-nanopb
+-rwxr-xr-x   0        0        0      554 2024-05-15 16:50:13.000000 nanopb-0.4.9.dev1473/nanopb/generator/protoc-gen-nanopb-py2
+-rw-r--r--   0        0        0      449 2024-05-15 16:50:13.000000 nanopb-0.4.9.dev1473/nanopb/generator/protoc-gen-nanopb.bat
+-rw-r--r--   0        0        0      302 2024-05-15 16:50:13.000000 nanopb-0.4.9.dev1473/nanopb/generator/protoc.bat
+-rw-r--r--   0        0        0     1065 2024-05-20 02:08:22.513020 nanopb-0.4.9.dev1473/pyproject.toml
+-rw-r--r--   0        0        0     5848 1970-01-01 00:00:00.000000 nanopb-0.4.9.dev1473/PKG-INFO
```

### Comparing `nanopb-0.4.9.dev1472/README.md` & `nanopb-0.4.9.dev1473/README.md`

 * *Files identical despite different names*

### Comparing `nanopb-0.4.9.dev1472/nanopb/generator/nanopb_generator.py` & `nanopb-0.4.9.dev1473/nanopb/generator/nanopb_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -611,37 +611,41 @@
         if field_options.HasField("max_count"):
             self.max_count = field_options.max_count
 
         if desc.HasField('default_value'):
             self.default = desc.default_value
 
         # Check field rules, i.e. required/optional/repeated.
+        if field_options.HasField("label_override"):
+            desc.label = field_options.label_override
+
         can_be_static = True
         if desc.label == FieldD.LABEL_REPEATED:
             self.rules = 'REPEATED'
             if self.max_count is None:
                 can_be_static = False
             else:
                 self.array_decl = '[%d]' % self.max_count
                 if field_options.fixed_count:
                   self.rules = 'FIXARRAY'
 
+        elif desc.label == FieldD.LABEL_REQUIRED:
+            # We allow LABEL_REQUIRED using label_override even for proto3 (see #962)
+            self.rules = 'REQUIRED'
         elif field_options.proto3:
             if desc.type == FieldD.TYPE_MESSAGE and not field_options.proto3_singular_msgs:
                 # In most other protobuf libraries proto3 submessages have
                 # "null" status. For nanopb, that is implemented as has_ field.
                 self.rules = 'OPTIONAL'
             elif hasattr(desc, "proto3_optional") and desc.proto3_optional:
                 # Protobuf 3.12 introduced optional fields for proto3 syntax
                 self.rules = 'OPTIONAL'
             else:
                 # Proto3 singular fields (without has_field)
                 self.rules = 'SINGULAR'
-        elif desc.label == FieldD.LABEL_REQUIRED:
-            self.rules = 'REQUIRED'
         elif desc.label == FieldD.LABEL_OPTIONAL:
             self.rules = 'OPTIONAL'
         else:
             raise NotImplementedError(desc.label)
 
         # Check if the field can be implemented with static allocation
         # i.e. whether the data size is known.
```

### Comparing `nanopb-0.4.9.dev1472/nanopb/generator/platformio_generator.py` & `nanopb-0.4.9.dev1473/nanopb/generator/platformio_generator.py`

 * *Files identical despite different names*

### Comparing `nanopb-0.4.9.dev1472/nanopb/generator/proto/__init__.py` & `nanopb-0.4.9.dev1473/nanopb/generator/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `nanopb-0.4.9.dev1472/nanopb/generator/proto/__pycache__/__init__.cpython-38.pyc` & `nanopb-0.4.9.dev1473/nanopb/generator/proto/__pycache__/__init__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon May  6 13:53:00 2024 UTC, .py size: 4629 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 bce0 3866 1512 0000  U.........8f....
+00000000: 550d 0d0a 0000 0000 c5e7 4466 1512 0000  U.........Df....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 a400 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a03 6401 6403 6c04 5a03 6401  d.l.Z.d.d.l.Z.d.
 00000050: 6403 6c05 5a05 6401 6403 6c06 5a06 6401  d.l.Z.d.d.l.Z.d.
 00000060: 6403 6c07 5a07 6401 6403 6c08 5a08 6401  d.l.Z.d.d.l.Z.d.
 00000070: 6403 6c09 5a09 6404 6405 6c0a 6d0b 5a0b  d.l.Z.d.d.l.m.Z.
```

### Comparing `nanopb-0.4.9.dev1472/nanopb/generator/proto/__pycache__/_utils.cpython-38.pyc` & `nanopb-0.4.9.dev1473/nanopb/generator/proto/__pycache__/_utils.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon May  6 13:53:00 2024 UTC, .py size: 2949 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 bce0 3866 850b 0000  U.........8f....
+00000000: 550d 0d0a 0000 0000 c5e7 4466 850b 0000  U.........Df....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a03 6400 6401 6c04 5a04 640c  d.l.Z.d.d.l.Z.d.
 00000050: 6403 6404 8401 5a05 6405 6406 8400 5a06  d.d...Z.d.d...Z.
 00000060: 6407 6408 8400 5a07 6409 640a 8400 5a08  d.d...Z.d.d...Z.
 00000070: 6509 640b 6b02 7250 6508 8300 0100 6401  e.d.k.rPe.....d.
```

### Comparing `nanopb-0.4.9.dev1472/nanopb/generator/proto/_utils.py` & `nanopb-0.4.9.dev1473/nanopb/generator/proto/_utils.py`

 * *Files identical despite different names*

### Comparing `nanopb-0.4.9.dev1472/nanopb/generator/proto/google/protobuf/descriptor.proto` & `nanopb-0.4.9.dev1473/nanopb/generator/proto/google/protobuf/descriptor.proto`

 * *Files identical despite different names*

### Comparing `nanopb-0.4.9.dev1472/nanopb/generator/proto/nanopb.proto` & `nanopb-0.4.9.dev1473/nanopb/generator/proto/nanopb.proto`

 * *Files 3% similar despite different names*

```diff
@@ -139,14 +139,19 @@
 
   // Package name that applies only for nanopb.
   optional string package = 25;
   
   // Override type of the field in generated C code. Only to be used with related field types
   optional google.protobuf.FieldDescriptorProto.Type type_override = 27;
 
+  // Override of the label of the field (see FieldDescriptorProto.Label). Can be used to create
+  // fields which nanopb considers required in proto3, or whether nanopb treats the field as
+  // optional/required/repeated.
+  optional google.protobuf.FieldDescriptorProto.Label label_override = 31;
+
   // Due to historical reasons, nanopb orders fields in structs by their tag number
   // instead of the order in .proto. Set this to false to keep the .proto order.
   // The default value will probably change to false in nanopb-0.5.0.
   optional bool sort_by_tag = 28 [default = true];
 
   // Set the FT_DEFAULT field conversion strategy.
   // A field that can become a static member of a c struct (e.g. int, bool, etc)
```

### Comparing `nanopb-0.4.9.dev1472/nanopb/generator/proto/nanopb_pb2.py` & `nanopb-0.4.9.dev1473/nanopb/generator/proto/nanopb_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import descriptor_pb2 as google_dot_protobuf_dot_descriptor__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0cnanopb.proto\x1a google/protobuf/descriptor.proto\"\xb9\x07\n\rNanoPBOptions\x12\x10\n\x08max_size\x18\x01 \x01(\x05\x12\x12\n\nmax_length\x18\x0e \x01(\x05\x12\x11\n\tmax_count\x18\x02 \x01(\x05\x12&\n\x08int_size\x18\x07 \x01(\x0e\x32\x08.IntSize:\nIS_DEFAULT\x12$\n\x04type\x18\x03 \x01(\x0e\x32\n.FieldType:\nFT_DEFAULT\x12\x18\n\nlong_names\x18\x04 \x01(\x08:\x04true\x12\x1c\n\rpacked_struct\x18\x05 \x01(\x08:\x05\x66\x61lse\x12\x1a\n\x0bpacked_enum\x18\n \x01(\x08:\x05\x66\x61lse\x12\x1b\n\x0cskip_message\x18\x06 \x01(\x08:\x05\x66\x61lse\x12\x18\n\tno_unions\x18\x08 \x01(\x08:\x05\x66\x61lse\x12\r\n\x05msgid\x18\t \x01(\r\x12\x1e\n\x0f\x61nonymous_oneof\x18\x0b \x01(\x08:\x05\x66\x61lse\x12\x15\n\x06proto3\x18\x0c \x01(\x08:\x05\x66\x61lse\x12#\n\x14proto3_singular_msgs\x18\x15 \x01(\x08:\x05\x66\x61lse\x12\x1d\n\x0e\x65num_to_string\x18\r \x01(\x08:\x05\x66\x61lse\x12\x1b\n\x0c\x66ixed_length\x18\x0f \x01(\x08:\x05\x66\x61lse\x12\x1a\n\x0b\x66ixed_count\x18\x10 \x01(\x08:\x05\x66\x61lse\x12\x1e\n\x0fsubmsg_callback\x18\x16 \x01(\x08:\x05\x66\x61lse\x12/\n\x0cmangle_names\x18\x11 \x01(\x0e\x32\x11.TypenameMangling:\x06M_NONE\x12(\n\x11\x63\x61llback_datatype\x18\x12 \x01(\t:\rpb_callback_t\x12\x34\n\x11\x63\x61llback_function\x18\x13 \x01(\t:\x19pb_default_field_callback\x12\x30\n\x0e\x64\x65scriptorsize\x18\x14 \x01(\x0e\x32\x0f.DescriptorSize:\x07\x44S_AUTO\x12\x1a\n\x0b\x64\x65\x66\x61ult_has\x18\x17 \x01(\x08:\x05\x66\x61lse\x12\x0f\n\x07include\x18\x18 \x03(\t\x12\x0f\n\x07\x65xclude\x18\x1a \x03(\t\x12\x0f\n\x07package\x18\x19 \x01(\t\x12\x41\n\rtype_override\x18\x1b \x01(\x0e\x32*.google.protobuf.FieldDescriptorProto.Type\x12\x19\n\x0bsort_by_tag\x18\x1c \x01(\x08:\x04true\x12.\n\rfallback_type\x18\x1d \x01(\x0e\x32\n.FieldType:\x0b\x46T_CALLBACK\x12\x13\n\x0binitializer\x18\x1e \x01(\t*i\n\tFieldType\x12\x0e\n\nFT_DEFAULT\x10\x00\x12\x0f\n\x0b\x46T_CALLBACK\x10\x01\x12\x0e\n\nFT_POINTER\x10\x04\x12\r\n\tFT_STATIC\x10\x02\x12\r\n\tFT_IGNORE\x10\x03\x12\r\n\tFT_INLINE\x10\x05*D\n\x07IntSize\x12\x0e\n\nIS_DEFAULT\x10\x00\x12\x08\n\x04IS_8\x10\x08\x12\t\n\x05IS_16\x10\x10\x12\t\n\x05IS_32\x10 \x12\t\n\x05IS_64\x10@*Z\n\x10TypenameMangling\x12\n\n\x06M_NONE\x10\x00\x12\x13\n\x0fM_STRIP_PACKAGE\x10\x01\x12\r\n\tM_FLATTEN\x10\x02\x12\x16\n\x12M_PACKAGE_INITIALS\x10\x03*E\n\x0e\x44\x65scriptorSize\x12\x0b\n\x07\x44S_AUTO\x10\x00\x12\x08\n\x04\x44S_1\x10\x01\x12\x08\n\x04\x44S_2\x10\x02\x12\x08\n\x04\x44S_4\x10\x04\x12\x08\n\x04\x44S_8\x10\x08:E\n\x0enanopb_fileopt\x12\x1c.google.protobuf.FileOptions\x18\xf2\x07 \x01(\x0b\x32\x0e.NanoPBOptions:G\n\rnanopb_msgopt\x12\x1f.google.protobuf.MessageOptions\x18\xf2\x07 \x01(\x0b\x32\x0e.NanoPBOptions:E\n\x0enanopb_enumopt\x12\x1c.google.protobuf.EnumOptions\x18\xf2\x07 \x01(\x0b\x32\x0e.NanoPBOptions:>\n\x06nanopb\x12\x1d.google.protobuf.FieldOptions\x18\xf2\x07 \x01(\x0b\x32\x0e.NanoPBOptionsB\x1a\n\x18\x66i.kapsi.koti.jpa.nanopb')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0cnanopb.proto\x1a google/protobuf/descriptor.proto\"\xfe\x07\n\rNanoPBOptions\x12\x10\n\x08max_size\x18\x01 \x01(\x05\x12\x12\n\nmax_length\x18\x0e \x01(\x05\x12\x11\n\tmax_count\x18\x02 \x01(\x05\x12&\n\x08int_size\x18\x07 \x01(\x0e\x32\x08.IntSize:\nIS_DEFAULT\x12$\n\x04type\x18\x03 \x01(\x0e\x32\n.FieldType:\nFT_DEFAULT\x12\x18\n\nlong_names\x18\x04 \x01(\x08:\x04true\x12\x1c\n\rpacked_struct\x18\x05 \x01(\x08:\x05\x66\x61lse\x12\x1a\n\x0bpacked_enum\x18\n \x01(\x08:\x05\x66\x61lse\x12\x1b\n\x0cskip_message\x18\x06 \x01(\x08:\x05\x66\x61lse\x12\x18\n\tno_unions\x18\x08 \x01(\x08:\x05\x66\x61lse\x12\r\n\x05msgid\x18\t \x01(\r\x12\x1e\n\x0f\x61nonymous_oneof\x18\x0b \x01(\x08:\x05\x66\x61lse\x12\x15\n\x06proto3\x18\x0c \x01(\x08:\x05\x66\x61lse\x12#\n\x14proto3_singular_msgs\x18\x15 \x01(\x08:\x05\x66\x61lse\x12\x1d\n\x0e\x65num_to_string\x18\r \x01(\x08:\x05\x66\x61lse\x12\x1b\n\x0c\x66ixed_length\x18\x0f \x01(\x08:\x05\x66\x61lse\x12\x1a\n\x0b\x66ixed_count\x18\x10 \x01(\x08:\x05\x66\x61lse\x12\x1e\n\x0fsubmsg_callback\x18\x16 \x01(\x08:\x05\x66\x61lse\x12/\n\x0cmangle_names\x18\x11 \x01(\x0e\x32\x11.TypenameMangling:\x06M_NONE\x12(\n\x11\x63\x61llback_datatype\x18\x12 \x01(\t:\rpb_callback_t\x12\x34\n\x11\x63\x61llback_function\x18\x13 \x01(\t:\x19pb_default_field_callback\x12\x30\n\x0e\x64\x65scriptorsize\x18\x14 \x01(\x0e\x32\x0f.DescriptorSize:\x07\x44S_AUTO\x12\x1a\n\x0b\x64\x65\x66\x61ult_has\x18\x17 \x01(\x08:\x05\x66\x61lse\x12\x0f\n\x07include\x18\x18 \x03(\t\x12\x0f\n\x07\x65xclude\x18\x1a \x03(\t\x12\x0f\n\x07package\x18\x19 \x01(\t\x12\x41\n\rtype_override\x18\x1b \x01(\x0e\x32*.google.protobuf.FieldDescriptorProto.Type\x12\x43\n\x0elabel_override\x18\x1f \x01(\x0e\x32+.google.protobuf.FieldDescriptorProto.Label\x12\x19\n\x0bsort_by_tag\x18\x1c \x01(\x08:\x04true\x12.\n\rfallback_type\x18\x1d \x01(\x0e\x32\n.FieldType:\x0b\x46T_CALLBACK\x12\x13\n\x0binitializer\x18\x1e \x01(\t*i\n\tFieldType\x12\x0e\n\nFT_DEFAULT\x10\x00\x12\x0f\n\x0b\x46T_CALLBACK\x10\x01\x12\x0e\n\nFT_POINTER\x10\x04\x12\r\n\tFT_STATIC\x10\x02\x12\r\n\tFT_IGNORE\x10\x03\x12\r\n\tFT_INLINE\x10\x05*D\n\x07IntSize\x12\x0e\n\nIS_DEFAULT\x10\x00\x12\x08\n\x04IS_8\x10\x08\x12\t\n\x05IS_16\x10\x10\x12\t\n\x05IS_32\x10 \x12\t\n\x05IS_64\x10@*Z\n\x10TypenameMangling\x12\n\n\x06M_NONE\x10\x00\x12\x13\n\x0fM_STRIP_PACKAGE\x10\x01\x12\r\n\tM_FLATTEN\x10\x02\x12\x16\n\x12M_PACKAGE_INITIALS\x10\x03*E\n\x0e\x44\x65scriptorSize\x12\x0b\n\x07\x44S_AUTO\x10\x00\x12\x08\n\x04\x44S_1\x10\x01\x12\x08\n\x04\x44S_2\x10\x02\x12\x08\n\x04\x44S_4\x10\x04\x12\x08\n\x04\x44S_8\x10\x08:E\n\x0enanopb_fileopt\x12\x1c.google.protobuf.FileOptions\x18\xf2\x07 \x01(\x0b\x32\x0e.NanoPBOptions:G\n\rnanopb_msgopt\x12\x1f.google.protobuf.MessageOptions\x18\xf2\x07 \x01(\x0b\x32\x0e.NanoPBOptions:E\n\x0enanopb_enumopt\x12\x1c.google.protobuf.EnumOptions\x18\xf2\x07 \x01(\x0b\x32\x0e.NanoPBOptions:>\n\x06nanopb\x12\x1d.google.protobuf.FieldOptions\x18\xf2\x07 \x01(\x0b\x32\x0e.NanoPBOptionsB\x1a\n\x18\x66i.kapsi.koti.jpa.nanopb')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'nanopb_pb2', _globals)
 if not _descriptor._USE_C_DESCRIPTORS:
   _globals['DESCRIPTOR']._loaded_options = None
   _globals['DESCRIPTOR']._serialized_options = b'\n\030fi.kapsi.koti.jpa.nanopb'
-  _globals['_FIELDTYPE']._serialized_start=1006
-  _globals['_FIELDTYPE']._serialized_end=1111
-  _globals['_INTSIZE']._serialized_start=1113
-  _globals['_INTSIZE']._serialized_end=1181
-  _globals['_TYPENAMEMANGLING']._serialized_start=1183
-  _globals['_TYPENAMEMANGLING']._serialized_end=1273
-  _globals['_DESCRIPTORSIZE']._serialized_start=1275
-  _globals['_DESCRIPTORSIZE']._serialized_end=1344
+  _globals['_FIELDTYPE']._serialized_start=1075
+  _globals['_FIELDTYPE']._serialized_end=1180
+  _globals['_INTSIZE']._serialized_start=1182
+  _globals['_INTSIZE']._serialized_end=1250
+  _globals['_TYPENAMEMANGLING']._serialized_start=1252
+  _globals['_TYPENAMEMANGLING']._serialized_end=1342
+  _globals['_DESCRIPTORSIZE']._serialized_start=1344
+  _globals['_DESCRIPTORSIZE']._serialized_end=1413
   _globals['_NANOPBOPTIONS']._serialized_start=51
-  _globals['_NANOPBOPTIONS']._serialized_end=1004
+  _globals['_NANOPBOPTIONS']._serialized_end=1073
 # @@protoc_insertion_point(module_scope)
```

### Comparing `nanopb-0.4.9.dev1472/nanopb/generator/protoc` & `nanopb-0.4.9.dev1473/nanopb/generator/protoc`

 * *Files identical despite different names*

### Comparing `nanopb-0.4.9.dev1472/nanopb/generator/protoc-gen-nanopb-py2` & `nanopb-0.4.9.dev1473/nanopb/generator/protoc-gen-nanopb-py2`

 * *Files identical despite different names*

### Comparing `nanopb-0.4.9.dev1472/pyproject.toml` & `nanopb-0.4.9.dev1473/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nanopb"
-version = "0.4.9-dev1472"
+version = "0.4.9-dev1473"
 description = "Nanopb is a small code-size Protocol Buffers implementation in ansi C. It is especially suitable for use in microcontrollers, but fits any memory restricted system."
 authors = ["Petteri Aimonen <jpa@npb.mail.kapsi.fi>"]
 license = "Zlib"
 repository = "https://github.com/nanopb/nanopb/"
 readme = "README.md"
 homepage = "https://jpa.kapsi.fi/nanopb/"
 documentation = "https://jpa.kapsi.fi/nanopb/docs/index.html"
```

### Comparing `nanopb-0.4.9.dev1472/PKG-INFO` & `nanopb-0.4.9.dev1473/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanopb
-Version: 0.4.9.dev1472
+Version: 0.4.9.dev1473
 Summary: Nanopb is a small code-size Protocol Buffers implementation in ansi C. It is especially suitable for use in microcontrollers, but fits any memory restricted system.
 Home-page: https://jpa.kapsi.fi/nanopb/
 License: Zlib
 Keywords: protobuf,protoc
 Author: Petteri Aimonen
 Author-email: jpa@npb.mail.kapsi.fi
 Requires-Python: >=2.7
```

