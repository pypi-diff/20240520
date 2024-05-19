# Comparing `tmp/omniblack_secret-0.0.2.tar.gz` & `tmp/omniblack_secret-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omniblack_secret-0.0.2.tar", last modified: Sun May 19 19:15:46 2024, max compression
+gzip compressed data, was "omniblack_secret-0.0.3.tar", last modified: Sun May 19 22:36:05 2024, max compression
```

## Comparing `omniblack_secret-0.0.2.tar` & `omniblack_secret-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 terryp    (1000) terryp    (1000)        0 2024-05-19 19:15:46.705006 omniblack_secret-0.0.2/
--rw-r--r--   0 terryp    (1000) terryp    (1000)     1099 2024-04-27 17:21:57.000000 omniblack_secret-0.0.2/LICENSE
--rw-r--r--   0 terryp    (1000) terryp    (1000)       18 2024-05-19 18:48:32.000000 omniblack_secret-0.0.2/MANIFEST.in
--rw-r--r--   0 terryp    (1000) terryp    (1000)      582 2024-05-19 19:15:46.704006 omniblack_secret-0.0.2/PKG-INFO
--rw-r--r--   0 terryp    (1000) terryp    (1000)     1997 2024-05-19 18:55:42.000000 omniblack_secret-0.0.2/cflags.py
-drwxr-xr-x   0 terryp    (1000) terryp    (1000)        0 2024-05-19 19:15:46.704006 omniblack_secret-0.0.2/omniblack.secret.egg-info/
--rw-r--r--   0 terryp    (1000) terryp    (1000)      582 2024-05-19 19:15:46.000000 omniblack_secret-0.0.2/omniblack.secret.egg-info/PKG-INFO
--rw-r--r--   0 terryp    (1000) terryp    (1000)      222 2024-05-19 19:15:46.000000 omniblack_secret-0.0.2/omniblack.secret.egg-info/SOURCES.txt
--rw-r--r--   0 terryp    (1000) terryp    (1000)        1 2024-05-19 19:15:46.000000 omniblack_secret-0.0.2/omniblack.secret.egg-info/dependency_links.txt
--rw-r--r--   0 terryp    (1000) terryp    (1000)       10 2024-05-19 19:15:46.000000 omniblack_secret-0.0.2/omniblack.secret.egg-info/top_level.txt
--rw-r--r--   0 terryp    (1000) terryp    (1000)      675 2024-05-19 18:55:50.000000 omniblack_secret-0.0.2/pyproject.toml
--rw-r--r--   0 terryp    (1000) terryp    (1000)    13166 2024-05-19 18:44:06.000000 omniblack_secret-0.0.2/secret.c
--rw-r--r--   0 terryp    (1000) terryp    (1000)       38 2024-05-19 19:15:46.705006 omniblack_secret-0.0.2/setup.cfg
--rw-r--r--   0 terryp    (1000) terryp    (1000)      224 2024-05-19 18:48:59.000000 omniblack_secret-0.0.2/setup.py
+drwxr-xr-x   0 terryp    (1000) terryp    (1000)        0 2024-05-19 22:36:05.250706 omniblack_secret-0.0.3/
+-rw-r--r--   0 terryp    (1000) terryp    (1000)     1082 2024-05-19 22:32:52.000000 omniblack_secret-0.0.3/LICENSE
+-rw-r--r--   0 terryp    (1000) terryp    (1000)       18 2024-05-19 18:48:32.000000 omniblack_secret-0.0.3/MANIFEST.in
+-rw-r--r--   0 terryp    (1000) terryp    (1000)      582 2024-05-19 22:36:05.250706 omniblack_secret-0.0.3/PKG-INFO
+-rw-r--r--   0 terryp    (1000) terryp    (1000)     1997 2024-05-19 18:55:42.000000 omniblack_secret-0.0.3/cflags.py
+drwxr-xr-x   0 terryp    (1000) terryp    (1000)        0 2024-05-19 22:36:05.249706 omniblack_secret-0.0.3/omniblack.secret.egg-info/
+-rw-r--r--   0 terryp    (1000) terryp    (1000)      582 2024-05-19 22:36:05.000000 omniblack_secret-0.0.3/omniblack.secret.egg-info/PKG-INFO
+-rw-r--r--   0 terryp    (1000) terryp    (1000)      222 2024-05-19 22:36:05.000000 omniblack_secret-0.0.3/omniblack.secret.egg-info/SOURCES.txt
+-rw-r--r--   0 terryp    (1000) terryp    (1000)        1 2024-05-19 22:36:05.000000 omniblack_secret-0.0.3/omniblack.secret.egg-info/dependency_links.txt
+-rw-r--r--   0 terryp    (1000) terryp    (1000)       10 2024-05-19 22:36:05.000000 omniblack_secret-0.0.3/omniblack.secret.egg-info/top_level.txt
+-rw-r--r--   0 terryp    (1000) terryp    (1000)      675 2024-05-19 22:32:41.000000 omniblack_secret-0.0.3/pyproject.toml
+-rw-r--r--   0 terryp    (1000) terryp    (1000)    14196 2024-05-19 22:35:33.000000 omniblack_secret-0.0.3/secret.c
+-rw-r--r--   0 terryp    (1000) terryp    (1000)       38 2024-05-19 22:36:05.250706 omniblack_secret-0.0.3/setup.cfg
+-rw-r--r--   0 terryp    (1000) terryp    (1000)      224 2024-05-19 18:48:59.000000 omniblack_secret-0.0.3/setup.py
```

### Comparing `omniblack_secret-0.0.2/LICENSE` & `omniblack_secret-0.0.3/LICENSE`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2024 Mattias Jansson, Terry Patterson
+Copyright (c) 2024 Terry Patterson
 
 Permission is hereby granted, free of charge, to any person obtaining
 a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish,
 distribute, sublicense, and/or sell copies of the Software, and to
 permit persons to whom the Software is furnished to do so, subject to
```

### Comparing `omniblack_secret-0.0.2/PKG-INFO` & `omniblack_secret-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniblack.secret
-Version: 0.0.2
+Version: 0.0.3
 Author-email: Terry Patterson <terryp@wegrok.net>
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
```

### Comparing `omniblack_secret-0.0.2/cflags.py` & `omniblack_secret-0.0.3/cflags.py`

 * *Files identical despite different names*

### Comparing `omniblack_secret-0.0.2/omniblack.secret.egg-info/PKG-INFO` & `omniblack_secret-0.0.3/omniblack.secret.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniblack.secret
-Version: 0.0.2
+Version: 0.0.3
 Author-email: Terry Patterson <terryp@wegrok.net>
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
```

### Comparing `omniblack_secret-0.0.2/pyproject.toml` & `omniblack_secret-0.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name='omniblack.secret'
-version='0.0.2'
+version='0.0.3'
 license={text='MIT License'}
 
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: MIT License',
     'Operating System :: POSIX :: Linux',
```

### Comparing `omniblack_secret-0.0.2/secret.c` & `omniblack_secret-0.0.3/secret.c`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #include <string.h>
 
 PyModuleDef secret_mod;
 PyType_Spec SecretSpec;
 
 struct SecretRef {
     volatile int readers;
-    Py_ssize_t len;
+    Py_ssize_t bytes_len;
     char* data;
 };
 
 struct SecretModuleState{
     PyTypeObject* Secret;
 };
 
@@ -150,15 +150,15 @@
 
     if (secret == NULL) {
         return NULL;
     }
 
     PyObject* string = PyUnicode_DecodeUTF8(
         secret->data,
-        secret->len,
+        secret->bytes_len,
         "strict"
     );
 
     lock_secret(secret);
 
     if (string == NULL) {
         return NULL;
@@ -195,14 +195,31 @@
     return 0;
 }
 
 int tp_clear(PyObject* Py_UNUSED(self)) {
     return 0;
 }
 
+Py_ssize_t code_points_len(const char* data, Py_ssize_t bytes_len) {
+    Py_ssize_t len = 0;
+
+    // ASCII is only 7 bits so the highest bit will never be set
+    // For multibyte unicode codepoints the first byte's high bits
+    // will be set to `11`, and the high bits of continuation bytes
+    // will be set to `10`. Therefore (*data & 0xC0) will only be
+    // 0x80 for continuation bytes, and count all bytes not starting
+    // with `10` count all starting bytes and ASCII bytes
+    // .. the number of bytes.
+    for (int i = 0; i < bytes_len; i += 1) {
+        len += (data[i] & 0xC0) != 0x80;
+    }
+
+    return len;
+}
+
 PyObject* prepare_new_secret(
     PyTypeObject* cls,
     const char* data,
     Py_ssize_t len
 ) {
     allocfunc tp_alloc = PyType_GetSlot(cls, Py_tp_alloc);
     PyObject* new_self = tp_alloc(cls, 0);
@@ -227,15 +244,15 @@
         return PyErr_SetFromErrno(PyExc_MemoryError);
     }
 
     // Copy our secret into the new buffer
     strcpy(secret_buffer, data);
 
     // Copy the metadata into the new python object
-    new_self_slot->len = len;
+    new_self_slot->bytes_len = len;
     new_self_slot->data = secret_buffer;
 
     // We are the reader. Setting it one means lock_secret will
     // correctly Re-protect the memory.
     new_self_slot->readers = 1;
 
     // Re-protect the new and old secret
@@ -291,15 +308,15 @@
     PyTypeObject* subtype = Py_TYPE(self);
     // Get the data to copy
     struct SecretRef* old_secret = unlock_secret(self);
 
     PyObject* new_self = prepare_new_secret(
         subtype,
         old_secret->data,
-        old_secret->len
+        old_secret->bytes_len
     );
 
     lock_secret(old_secret);
     return new_self;
 }
 
 PyObject* verify_password_against(PyObject* self, PyObject* args) {
@@ -324,25 +341,25 @@
     if (other_secret == NULL) {
         lock_secret(self_secret);
         return NULL;
     }
 
     PyThreadState* _save = NULL;
 
-    if (self_secret->len >= 2000) {
+    if (self_secret->bytes_len >= 2000) {
         Py_UNBLOCK_THREADS;
     }
 
     const int verify_result = crypto_pwhash_str_verify(
         other_secret->data,
         self_secret->data,
-        (unsigned long long)self_secret->len
+        (unsigned long long)self_secret->bytes_len
     );
 
-    if (self_secret->len >= 2000) {
+    if (self_secret->bytes_len >= 2000) {
         Py_BLOCK_THREADS;
     }
 
     lock_secret(self_secret);
     lock_secret(other_secret);
 
     return PyBool_FromLong(!verify_result);
@@ -353,30 +370,30 @@
     if (secret == NULL) {
         return NULL;
     }
 
     PyTypeObject* cls = borrowSecretCls(self);
 
     PyThreadState* _save = NULL;
-    if (secret->len >= 2000) {
+    if (secret->bytes_len >= 2000) {
         Py_UNBLOCK_THREADS;
     }
 
     char out[crypto_pwhash_STRBYTES] = {};
 
-    unsigned long long len = (unsigned long long)secret->len;
+    unsigned long long len = (unsigned long long)secret->bytes_len;
     int hash_result = crypto_pwhash_str(
         (char*)&out,
         secret->data,
         len,
         crypto_pwhash_OPSLIMIT_INTERACTIVE,
         crypto_pwhash_MEMLIMIT_INTERACTIVE
     );
 
-    if (secret->len >= 2000) {
+    if (secret->bytes_len >= 2000) {
         Py_BLOCK_THREADS;
     }
 
     // We no longer need the secret
     lock_secret(secret);
 
     if (hash_result) {
@@ -419,15 +436,17 @@
     // should check to see if the cost of allocating and encoding
     // exceeds the cost of releasing and aquiring the GIL.
     PyThreadState* _save = NULL;
     if (py_size >= 2000) {
         Py_UNBLOCK_THREADS;
     }
 
-    size_t num_of_bytes = (size_t)py_size;
+    // Calculate the number of bytes needed
+    // to get a base64 string of N-characters
+    size_t num_of_bytes = (size_t)py_size / 4 * 3;
 
     unsigned char* new_data = sodium_malloc(num_of_bytes);
 
     if (new_data == NULL) {
         return PyErr_NoMemory();
     }
 
@@ -469,14 +488,26 @@
     );
 
     sodium_free(b64_data);
 
     return result;
 }
 
+Py_ssize_t sq_length(PyObject* self) {
+    struct SecretRef* secret = unlock_secret(self);
+
+    if (secret == NULL) {
+        return -1;
+    }
+
+    Py_ssize_t len = code_points_len(secret->data, secret->bytes_len);
+    lock_secret(secret);
+    return len;
+}
+
 PyMethodDef methods[] = {
     {
         .ml_name="__copy__",
         .ml_meth=(PyCFunction)copy,
         .ml_flags=METH_NOARGS,
         .ml_doc=PyDoc_STR("Return a copy of the secret."),
     },
@@ -520,18 +551,15 @@
             "stored password format."
         ),
     },
     {
         .ml_name="random_secret",
         .ml_meth=(PyCFunction)random_secret,
         .ml_flags=METH_VARARGS | METH_CLASS,
-        .ml_doc=PyDoc_STR(
-            "Return a new random secret `n` bytes long.\n"
-            "The secret will be encoded in url safe base64."
-        ),
+        .ml_doc=PyDoc_STR("Return a new random url safe base64 string."),
     },
     {.ml_name=NULL},
 };
 
 PyType_Slot type_slots[] = {
     {
         .slot=Py_tp_doc,
@@ -557,14 +585,18 @@
         .slot=Py_tp_traverse,
         .pfunc=tp_traverse,
     },
     {
         .slot=Py_tp_clear,
         .pfunc=tp_clear,
     },
+    {
+        .slot=Py_sq_length,
+        .pfunc=sq_length,
+    },
     {0, 0}
 };
 
 PyType_Spec SecretSpec = {
     .name="omniblack.secret.Secret",
     .basicsize=-(Py_ssize_t)sizeof(struct SecretRef),
     .flags=Py_TPFLAGS_IMMUTABLETYPE | Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC,
```

