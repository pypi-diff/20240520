# Comparing `tmp/anycrc-0.7.3.tar.gz` & `tmp/anycrc-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anycrc-0.7.3.tar", last modified: Sun May 19 17:46:08 2024, max compression
+gzip compressed data, was "anycrc-0.7.4.tar", last modified: Mon May 20 03:36:56 2024, max compression
```

## Comparing `anycrc-0.7.3.tar` & `anycrc-0.7.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:46:08.896280 anycrc-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-19 17:46:03.000000 anycrc-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-19 17:46:08.896280 anycrc-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-19 17:46:03.000000 anycrc-0.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:46:08.892279 anycrc-0.7.3/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:46:08.892279 anycrc-0.7.3/lib/crcany/
--rw-r--r--   0 runner    (1001) docker     (127)    25358 2024-05-19 17:46:03.000000 anycrc-0.7.3/lib/crcany/crc.c
--rw-r--r--   0 runner    (1001) docker     (127)     7268 2024-05-19 17:46:03.000000 anycrc-0.7.3/lib/crcany/crcdbl.c
--rw-r--r--   0 runner    (1001) docker     (127)    18969 2024-05-19 17:46:03.000000 anycrc-0.7.3/lib/crcany/model.c
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-19 17:46:03.000000 anycrc-0.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 17:46:08.896280 anycrc-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-19 17:46:03.000000 anycrc-0.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:46:08.892279 anycrc-0.7.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:46:08.896280 anycrc-0.7.3/src/anycrc/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-19 17:46:03.000000 anycrc-0.7.3/src/anycrc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-19 17:46:03.000000 anycrc-0.7.3/src/anycrc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-05-19 17:46:03.000000 anycrc-0.7.3/src/anycrc/anycrc.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    17836 2024-05-19 17:46:03.000000 anycrc-0.7.3/src/anycrc/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:46:08.896280 anycrc-0.7.3/src/anycrc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-19 17:46:08.000000 anycrc-0.7.3/src/anycrc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-19 17:46:08.000000 anycrc-0.7.3/src/anycrc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 17:46:08.000000 anycrc-0.7.3/src/anycrc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-19 17:46:08.000000 anycrc-0.7.3/src/anycrc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:36:56.009386 anycrc-0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-20 03:36:50.000000 anycrc-0.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-05-20 03:36:56.009386 anycrc-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-20 03:36:50.000000 anycrc-0.7.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:36:56.005386 anycrc-0.7.4/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:36:56.005386 anycrc-0.7.4/lib/crcany/
+-rw-r--r--   0 runner    (1001) docker     (127)    25358 2024-05-20 03:36:50.000000 anycrc-0.7.4/lib/crcany/crc.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7268 2024-05-20 03:36:50.000000 anycrc-0.7.4/lib/crcany/crcdbl.c
+-rw-r--r--   0 runner    (1001) docker     (127)    18969 2024-05-20 03:36:50.000000 anycrc-0.7.4/lib/crcany/model.c
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-20 03:36:50.000000 anycrc-0.7.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 03:36:56.009386 anycrc-0.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-20 03:36:50.000000 anycrc-0.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:36:56.005386 anycrc-0.7.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:36:56.005386 anycrc-0.7.4/src/anycrc/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-20 03:36:50.000000 anycrc-0.7.4/src/anycrc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-20 03:36:50.000000 anycrc-0.7.4/src/anycrc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-05-20 03:36:50.000000 anycrc-0.7.4/src/anycrc/anycrc.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    17836 2024-05-20 03:36:50.000000 anycrc-0.7.4/src/anycrc/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:36:56.009386 anycrc-0.7.4/src/anycrc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-05-20 03:36:55.000000 anycrc-0.7.4/src/anycrc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-20 03:36:56.000000 anycrc-0.7.4/src/anycrc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 03:36:56.000000 anycrc-0.7.4/src/anycrc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 03:36:56.000000 anycrc-0.7.4/src/anycrc.egg-info/top_level.txt
```

### Comparing `anycrc-0.7.3/LICENSE` & `anycrc-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `anycrc-0.7.3/PKG-INFO` & `anycrc-0.7.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anycrc
-Version: 0.7.3
+Version: 0.7.4
 Summary: Python CRC Computation Library
 Project-URL: Homepage, https://github.com/marzooqy/anycrc
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This is a Cython module with bindings to the [crcany](https://github.com/madler/crcany) library. It supports calculating CRC hashes of arbitary sizes as well as updating a crc hash over time. It takes advantage of crcany's ability to efficiently combine multiple CRCs to parallelize the CRC's calculation.
@@ -96,10 +96,12 @@
 | fastcrc | 0.67 | 0.62 | 39.75 |
 | crcmod-plus | 0.67 | 0.62 | 39.73 |
 
 Tested on a 10th generation Intel i7 processor. Parallel performance will depend on your system.
 
 #### Notes
 
-Parallelism is disabled when the length of the input data is under 200k, as the serial method is faster in that case.
+1- Parallelism is disabled when the length of the input data is under 200k, as the serial method is faster in that case.
 
-The input needs to be very large in order to notice the speed advantage of the parallel algorithm.
+2- The input needs to be very large in order to notice the speed advantage of the parallel algorithm.
+
+3- CRCs with a width larger than 64 bits use the slower byte-by-byte algorithm.
```

### Comparing `anycrc-0.7.3/README.md` & `anycrc-0.7.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -87,10 +87,12 @@
 | fastcrc | 0.67 | 0.62 | 39.75 |
 | crcmod-plus | 0.67 | 0.62 | 39.73 |
 
 Tested on a 10th generation Intel i7 processor. Parallel performance will depend on your system.
 
 #### Notes
 
-Parallelism is disabled when the length of the input data is under 200k, as the serial method is faster in that case.
+1- Parallelism is disabled when the length of the input data is under 200k, as the serial method is faster in that case.
 
-The input needs to be very large in order to notice the speed advantage of the parallel algorithm.
+2- The input needs to be very large in order to notice the speed advantage of the parallel algorithm.
+
+3- CRCs with a width larger than 64 bits use the slower byte-by-byte algorithm.
```

### Comparing `anycrc-0.7.3/lib/crcany/crc.c` & `anycrc-0.7.4/lib/crcany/crc.c`

 * *Files identical despite different names*

### Comparing `anycrc-0.7.3/lib/crcany/crcdbl.c` & `anycrc-0.7.4/lib/crcany/crcdbl.c`

 * *Files identical despite different names*

### Comparing `anycrc-0.7.3/lib/crcany/model.c` & `anycrc-0.7.4/lib/crcany/model.c`

 * *Files identical despite different names*

### Comparing `anycrc-0.7.3/setup.py` & `anycrc-0.7.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         
 else:
     compile_args = ['-fopenmp', '-O2']
     link_args = ['-fopenmp', '-O2']
     
 setup(
     name = 'anycrc',
-    version = '0.7.3',
+    version = '0.7.4',
     package_dir = {"": "src"},
     cmdclass={"build_ext": Build},
     ext_modules = [
         Extension(
             name='anycrc.anycrc',
             extra_compile_args=compile_args,
             extra_link_args=link_args,
```

### Comparing `anycrc-0.7.3/src/anycrc/anycrc.pyx` & `anycrc-0.7.4/src/anycrc/anycrc.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     
 cdef extern from '../../lib/crcany/crcdbl.h':
     cdef int crc_table_bytewise_dbl(model_t *model)
     cdef void crc_bytewise_dbl(model_t *model, word_t *crc_hi, word_t *crc_lo, const unsigned char *buf, size_t len)
     
 cdef bint parallel = True
 cdef word_t MASK = -1
-word_bits = WORDBITS
+word_bits = WORDBITS #accessible from python
 
 cdef class CRC:
     cdef model_t model
     cdef word_t reg, reg_hi
     
     def __cinit__(self, width, poly, init, ref_in, ref_out, xor_out, check=0, residue=0):
         cdef unsigned endian = 1 if sys.byteorder == 'little' else 0
@@ -115,52 +115,55 @@
         self.reg = crc & MASK
         self.reg_hi = crc >> WORDBITS
         
     def reset(self):
         self.reg = self.model.init
         self.reg_hi = self.model.init_hi
         
-    cdef word_t _calc(self, const unsigned char *data, word_t length):
-        cdef word_t crc
-        cdef int error = 0
-        
+    cdef word_t _calc(self, const unsigned char *data, word_t length, int *error):
         if parallel and length >= 200000:
-            crc = crc_parallel(&self.model, self.reg, data, length, &error)
-            
-            if error == 1:
-                raise MemoryError('Out of memory error')
-                
-            return crc
-            
+            return crc_parallel(&self.model, self.reg, data, length, error)
         else:
             return crc_slice16(&self.model, self.reg, data, length)
             
     def calc(self, data):
         if isinstance(data, str):
             data = (<unicode> data).encode('utf-8')
             
         cdef word_t crc_lo = self.reg
         cdef word_t crc_hi = self.reg_hi
+        cdef int error = 0;
         
         if self.model.width <= WORDBITS:
-            return self._calc(data, len(data))
+            crc_lo = self._calc(data, len(data), &error)
+            
+            if error == 1:
+                raise MemoryError('Out of memory error')
+                
+            return crc_lo
             
         else:
             crc_bytewise_dbl(&self.model, &crc_hi, &crc_lo, data, len(data))
             crc = crc_hi
             crc <<= WORDBITS
             crc += crc_lo
             return crc
             
     def update(self, data):
         if isinstance(data, str):
             data = (<unicode> data).encode('utf-8')
             
+        cdef int error = 0
+        
         if self.model.width <= WORDBITS:
-            self.reg = self._calc(data, len(data))
+            self.reg = self._calc(data, len(data), &error)
+            
+            if error == 1:
+                raise MemoryError('Out of memory error')
+                
             return self.reg
             
         else:
             crc_bytewise_dbl(&self.model, &self.reg_hi, &self.reg, data, len(data))
             crc = self.reg_hi
             crc <<= WORDBITS
             crc += self.reg
```

### Comparing `anycrc-0.7.3/src/anycrc/models.py` & `anycrc-0.7.4/src/anycrc/models.py`

 * *Files identical despite different names*

### Comparing `anycrc-0.7.3/src/anycrc.egg-info/PKG-INFO` & `anycrc-0.7.4/src/anycrc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anycrc
-Version: 0.7.3
+Version: 0.7.4
 Summary: Python CRC Computation Library
 Project-URL: Homepage, https://github.com/marzooqy/anycrc
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This is a Cython module with bindings to the [crcany](https://github.com/madler/crcany) library. It supports calculating CRC hashes of arbitary sizes as well as updating a crc hash over time. It takes advantage of crcany's ability to efficiently combine multiple CRCs to parallelize the CRC's calculation.
@@ -96,10 +96,12 @@
 | fastcrc | 0.67 | 0.62 | 39.75 |
 | crcmod-plus | 0.67 | 0.62 | 39.73 |
 
 Tested on a 10th generation Intel i7 processor. Parallel performance will depend on your system.
 
 #### Notes
 
-Parallelism is disabled when the length of the input data is under 200k, as the serial method is faster in that case.
+1- Parallelism is disabled when the length of the input data is under 200k, as the serial method is faster in that case.
 
-The input needs to be very large in order to notice the speed advantage of the parallel algorithm.
+2- The input needs to be very large in order to notice the speed advantage of the parallel algorithm.
+
+3- CRCs with a width larger than 64 bits use the slower byte-by-byte algorithm.
```

