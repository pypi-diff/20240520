# Comparing `tmp/quivr-0.7.2a1.tar.gz` & `tmp/quivr-0.7.3a1.tar.gz`

## Comparing `quivr-0.7.2a1.tar` & `quivr-0.7.3a1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 quivr-0.7.2a1/quivr/__init__.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 quivr-0.7.2a1/quivr/__version__.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 quivr-0.7.2a1/quivr/_arrow_utils.py
--rw-r--r--   0        0        0     5675 2020-02-02 00:00:00.000000 quivr-0.7.2a1/quivr/attributes.py
--rw-r--r--   0        0        0    49428 2020-02-02 00:00:00.000000 quivr-0.7.2a1/quivr/columns.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 quivr-0.7.2a1/quivr/concat.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 quivr-0.7.2a1/quivr/defragment.py
--rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 quivr-0.7.2a1/quivr/errors.py
--rw-r--r--   0        0        0    18383 2020-02-02 00:00:00.000000 quivr-0.7.2a1/quivr/linkage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quivr-0.7.2a1/quivr/py.typed
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 quivr-0.7.2a1/quivr/schemagraph.py
--rw-r--r--   0        0        0    46922 2020-02-02 00:00:00.000000 quivr-0.7.2a1/quivr/tables.py
--rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 quivr-0.7.2a1/quivr/validators.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quivr-0.7.2a1/quivr/experimental/__init__.py
--rw-r--r--   0        0        0     8225 2020-02-02 00:00:00.000000 quivr-0.7.2a1/quivr/experimental/shmem.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 quivr-0.7.2a1/.gitignore
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 quivr-0.7.2a1/LICENSE
--rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 quivr-0.7.2a1/README.md
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 quivr-0.7.2a1/pyproject.toml
--rw-r--r--   0        0        0     9579 2020-02-02 00:00:00.000000 quivr-0.7.2a1/PKG-INFO
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 quivr-0.7.3a1/quivr/__init__.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 quivr-0.7.3a1/quivr/__version__.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 quivr-0.7.3a1/quivr/_arrow_utils.py
+-rw-r--r--   0        0        0     5675 2020-02-02 00:00:00.000000 quivr-0.7.3a1/quivr/attributes.py
+-rw-r--r--   0        0        0    48884 2020-02-02 00:00:00.000000 quivr-0.7.3a1/quivr/columns.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 quivr-0.7.3a1/quivr/concat.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 quivr-0.7.3a1/quivr/defragment.py
+-rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 quivr-0.7.3a1/quivr/errors.py
+-rw-r--r--   0        0        0    18351 2020-02-02 00:00:00.000000 quivr-0.7.3a1/quivr/linkage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quivr-0.7.3a1/quivr/py.typed
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 quivr-0.7.3a1/quivr/schemagraph.py
+-rw-r--r--   0        0        0    46924 2020-02-02 00:00:00.000000 quivr-0.7.3a1/quivr/tables.py
+-rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 quivr-0.7.3a1/quivr/validators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quivr-0.7.3a1/quivr/experimental/__init__.py
+-rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 quivr-0.7.3a1/quivr/experimental/shmem.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 quivr-0.7.3a1/.gitignore
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 quivr-0.7.3a1/LICENSE
+-rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 quivr-0.7.3a1/README.md
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 quivr-0.7.3a1/pyproject.toml
+-rw-r--r--   0        0        0     9579 2020-02-02 00:00:00.000000 quivr-0.7.3a1/PKG-INFO
```

### Comparing `quivr-0.7.2a1/quivr/__init__.py` & `quivr-0.7.3a1/quivr/__init__.py`

 * *Files identical despite different names*

### Comparing `quivr-0.7.2a1/quivr/_arrow_utils.py` & `quivr-0.7.3a1/quivr/_arrow_utils.py`

 * *Files identical despite different names*

### Comparing `quivr-0.7.2a1/quivr/attributes.py` & `quivr-0.7.3a1/quivr/attributes.py`

 * *Files identical despite different names*

### Comparing `quivr-0.7.2a1/quivr/columns.py` & `quivr-0.7.3a1/quivr/columns.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,20 +68,18 @@
             else:
                 try:
                     self._default_scalar = pa.scalar(self.default, self.dtype)
                 except (pa.ArrowInvalid, pa.ArrowTypeError, OverflowError) as e:
                     raise errors.InvalidColumnDefault(self.default, self.dtype) from e
 
     @overload
-    def __get__(self, obj: None, objtype: type) -> Self:
-        ...
+    def __get__(self, obj: None, objtype: type) -> Self: ...
 
     @overload
-    def __get__(self, obj: tables.Table, objtype: type) -> pa.Array:
-        ...
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.Array: ...
 
     def __get__(self, obj: Union[tables.Table, None], objtype: type) -> Union[Self, pa.Array]:
         """
 
         Gets the Column object from a Table class, or the associated data from a Table instance.
 
         This method is part of the `descriptor protocol <https://docs.python.org/3/howto/descriptor.html>`_.
@@ -222,20 +220,18 @@
                 fields.append(field.with_nullable(True))
             data = pa.StructArray.from_arrays(data.flatten(), fields=fields)
 
         table = table.set_column(idx, self.pyarrow_field(), data)
         return table
 
     @overload
-    def __get__(self, obj: None, objtype: type) -> Self:
-        ...
+    def __get__(self, obj: None, objtype: type) -> Self: ...
 
     @overload
-    def __get__(self, obj: tables.Table, objtype: type) -> T:
-        ...
+    def __get__(self, obj: tables.Table, objtype: type) -> T: ...
 
     def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, T]:
         if obj is None:
             return self
         array = obj.table.column(self.name)
 
         metadata = self.metadata
@@ -274,20 +270,18 @@
         default: Union[None, Callable[[], int], int] = None,
     ):
         super().__init__(
             pa.int8(), nullable=nullable, metadata=metadata, validator=validator, default=default
         )
 
     @overload
-    def __get__(self, obj: None, objtype: type) -> Self:
-        ...
+    def __get__(self, obj: None, objtype: type) -> Self: ...
 
     @overload
-    def __get__(self, obj: tables.Table, objtype: type) -> pa.Int8Array:
-        ...
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.Int8Array: ...
 
     def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.Int8Array]:
         if obj is None:
             return self
         return _fast_combine_chunks(obj.table[self.name])
 
 
@@ -306,20 +300,18 @@
         default: Union[None, Callable[[], int], int] = None,
     ):
         super().__init__(
             pa.int16(), nullable=nullable, metadata=metadata, validator=validator, default=default
         )
 
     @overload
-    def __get__(self, obj: None, objtype: type) -> Self:
-        ...
+    def __get__(self, obj: None, objtype: type) -> Self: ...
 
     @overload
-    def __get__(self, obj: tables.Table, objtype: type) -> pa.Int16Array:
-        ...
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.Int16Array: ...
 
     def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.Int16Array]:
         if obj is None:
             return self
         return _fast_combine_chunks(obj.table[self.name])
 
 
@@ -338,20 +330,18 @@
         default: Union[None, Callable[[], int], int] = None,
     ):
         super().__init__(
             pa.int32(), nullable=nullable, metadata=metadata, validator=validator, default=default
         )
 
     @overload
-    def __get__(self, obj: None, objtype: type) -> Self:
-        ...
+    def __get__(self, obj: None, objtype: type) -> Self: ...
 
     @overload
-    def __get__(self, obj: tables.Table, objtype: type) -> pa.Int32Array:
-        ...
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.Int32Array: ...
 
     def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.Int32Array]:
         if obj is None:
             return self
         return _fast_combine_chunks(obj.table[self.name])
 
 
@@ -370,20 +360,18 @@
         default: Union[None, Callable[[], int], int] = None,
     ):
         super().__init__(
             pa.int64(), nullable=nullable, metadata=metadata, validator=validator, default=default
         )
 
     @overload
-    def __get__(self, obj: None, objtype: type) -> Self:
-        ...
+    def __get__(self, obj: None, objtype: type) -> Self: ...
 
     @overload
-    def __get__(self, obj: tables.Table, objtype: type) -> pa.Int64Array:
-        ...
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.Int64Array: ...
 
     def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.Int64Array]:
         if obj is None:
             return self
         return _fast_combine_chunks(obj.table[self.name])
 
 
@@ -402,20 +390,18 @@
         default: Union[None, Callable[[], int], int] = None,
     ):
         super().__init__(
             pa.uint8(), nullable=nullable, metadata=metadata, validator=validator, default=default
         )
 
     @overload
-    def __get__(self, obj: None, objtype: type) -> Self:
-        ...
+    def __get__(self, obj: None, objtype: type) -> Self: ...
 
     @overload
-    def __get__(self, obj: tables.Table, objtype: type) -> pa.UInt8Array:
-        ...
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.UInt8Array: ...
 
     def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.UInt8Array]:
         if obj is None:
             return self
         return _fast_combine_chunks(obj.table[self.name])
 
 
@@ -434,20 +420,18 @@
         default: Union[None, Callable[[], int], int] = None,
     ):
         super().__init__(
             pa.uint16(), nullable=nullable, metadata=metadata, validator=validator, default=default
         )
 
     @overload
-    def __get__(self, obj: None, objtype: type) -> Self:
-        ...
+    def __get__(self, obj: None, objtype: type) -> Self: ...
 
     @overload
-    def __get__(self, obj: tables.Table, objtype: type) -> pa.UInt16Array:
-        ...
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.UInt16Array: ...
 
     def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.UInt16Array]:
         if obj is None:
             return self
         return _fast_combine_chunks(obj.table[self.name])
 
 
@@ -466,20 +450,18 @@
         default: Union[None, Callable[[], int], int] = None,
     ):
         super().__init__(
             pa.uint32(), nullable=nullable, metadata=metadata, validator=validator, default=default
         )
 
     @overload
-    def __get__(self, obj: None, objtype: type) -> Self:
-        ...
+    def __get__(self, obj: None, objtype: type) -> Self: ...
 
     @overload
-    def __get__(self, obj: tables.Table, objtype: type) -> pa.UInt32Array:
-        ...
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.UInt32Array: ...
 
     def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.UInt32Array]:
         if obj is None:
             return self
         return _fast_combine_chunks(obj.table[self.name])
 
 
@@ -498,20 +480,18 @@
         default: Union[None, Callable[[], int], int] = None,
     ):
         super().__init__(
             pa.uint64(), nullable=nullable, metadata=metadata, validator=validator, default=default
         )
 
     @overload
-    def __get__(self, obj: None, objtype: type) -> Self:
-        ...
+    def __get__(self, obj: None, objtype: type) -> Self: ...
 
     @overload
-    def __get__(self, obj: tables.Table, objtype: type) -> pa.UInt64Array:
-        ...
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.UInt64Array: ...
 
     def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.UInt64Array]:
         if obj is None:
             return self
         return _fast_combine_chunks(obj.table[self.name])
 
 
@@ -538,20 +518,18 @@
         nullable: bool = False,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.float16(), nullable=nullable, metadata=metadata, validator=validator)
 
     @overload
-    def __get__(self, obj: None, objtype: type) -> Self:
-        ...
+    def __get__(self, obj: None, objtype: type) -> Self: ...
 
     @overload
-    def __get__(self, obj: tables.Table, objtype: type) -> pa.lib.HalfFloatArray:
-        ...
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.lib.HalfFloatArray: ...
 
     def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.lib.HalfFloatArray]:
         if obj is None:
             return self
         return _fast_combine_chunks(obj.table[self.name])
 
 
@@ -570,20 +548,18 @@
         default: Union[None, Callable[[], float], float] = None,
     ):
         super().__init__(
             pa.float32(), nullable=nullable, metadata=metadata, validator=validator, default=default
         )
 
     @overload
-    def __get__(self, obj: None, objtype: type) -> Self:
-        ...
+    def __get__(self, obj: None, objtype: type) -> Self: ...
 
     @overload
-    def __get__(self, obj: tables.Table, objtype: type) -> pa.lib.FloatArray:
-        ...
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.lib.FloatArray: ...
 
     def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.lib.FloatArray]:
         if obj is None:
             return self
         return _fast_combine_chunks(obj.table[self.name])
 
 
@@ -602,20 +578,18 @@
         default: Union[None, Callable[[], float], float] = None,
     ):
         super().__init__(
             pa.float64(), nullable=nullable, metadata=metadata, validator=validator, default=default
         )
 
     @overload
-    def __get__(self, obj: None, objtype: type) -> Self:
-        ...
+    def __get__(self, obj: None, objtype: type) -> Self: ...
 
     @overload
-    def __get__(self, obj: tables.Table, objtype: type) -> pa.lib.DoubleArray:
-        ...
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.lib.DoubleArray: ...
 
     def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.lib.DoubleArray]:
         if obj is None:
             return self
         return _fast_combine_chunks(obj.table[self.name])
 
 
@@ -632,20 +606,18 @@
         default: Union[None, Callable[[], bool], bool] = None,
     ):
         super().__init__(
             pa.bool_(), nullable=nullable, metadata=metadata, validator=validator, default=default
         )
 
     @overload
-    def __get__(self, obj: None, objtype: type) -> Self:
-        ...
+    def __get__(self, obj: None, objtype: type) -> Self: ...
 
     @overload
-    def __get__(self, obj: tables.Table, objtype: type) -> pa.BooleanArray:
-        ...
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.BooleanArray: ...
 
     def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[pa.BooleanArray, Self]:
         if obj is None:
             return self
         return _fast_combine_chunks(obj.table[self.name])
 
 
@@ -668,20 +640,18 @@
         default: Union[None, str, Callable[[], str]] = None,
     ):
         super().__init__(
             pa.string(), nullable=nullable, metadata=metadata, validator=validator, default=default
         )
 
     @overload
-    def __get__(self, obj: None, objtype: type) -> Self:
-        ...
+    def __get__(self, obj: None, objtype: type) -> Self: ...
 
     @overload
-    def __get__(self, obj: tables.Table, objtype: type) -> pa.StringArray:
-        ...
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.StringArray: ...
 
     def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[pa.StringArray, Self]:
         if obj is None:
             return self
         return _fast_combine_chunks(obj.table[self.name])
 
 
@@ -699,20 +669,18 @@
         default: Union[None, bytes, Callable[[], bytes]] = None,
     ):
         super().__init__(
             pa.large_binary(), nullable=nullable, metadata=metadata, validator=validator, default=default
         )
 
     @overload
-    def __get__(self, obj: None, objtype: type) -> Self:
-        ...
+    def __get__(self, obj: None, objtype: type) -> Self: ...
 
     @overload
-    def __get__(self, obj: tables.Table, objtype: type) -> pa.LargeBinaryArray:
-        ...
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.LargeBinaryArray: ...
 
     def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.LargeBinaryArray]:
         if obj is None:
             return self
         return _fast_combine_chunks(obj.table[self.name])
 
 
@@ -730,20 +698,18 @@
         default: Union[None, str, Callable[[], str]] = None,
     ):
         super().__init__(
             pa.large_string(), nullable=nullable, metadata=metadata, validator=validator, default=default
         )
 
     @overload
-    def __get__(self, obj: None, objtype: type) -> Self:
-        ...
+    def __get__(self, obj: None, objtype: type) -> Self: ...
 
     @overload
-    def __get__(self, obj: tables.Table, objtype: type) -> pa.LargeStringArray:
-        ...
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.LargeStringArray: ...
 
     def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.LargeStringArray]:
         if obj is None:
             return self
         return _fast_combine_chunks(obj.table[self.name])
 
 
@@ -760,20 +726,18 @@
         nullable: bool = False,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.date32(), nullable=nullable, metadata=metadata, validator=validator)
 
     @overload
-    def __get__(self, obj: None, objtype: type) -> Self:
-        ...
+    def __get__(self, obj: None, objtype: type) -> Self: ...
 
     @overload
-    def __get__(self, obj: tables.Table, objtype: type) -> pa.Date32Array:
-        ...
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.Date32Array: ...
 
     def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.Date32Array]:
         if obj is None:
             return self
         return _fast_combine_chunks(obj.table[self.name])
 
 
@@ -790,20 +754,18 @@
         nullable: bool = False,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.date64(), nullable=nullable, metadata=metadata, validator=validator)
 
     @overload
-    def __get__(self, obj: None, objtype: type) -> Self:
-        ...
+    def __get__(self, obj: None, objtype: type) -> Self: ...
 
     @overload
-    def __get__(self, obj: tables.Table, objtype: type) -> pa.Date64Array:
-        ...
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.Date64Array: ...
 
     def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.Date64Array]:
         if obj is None:
             return self
         return _fast_combine_chunks(obj.table[self.name])
 
 
@@ -843,20 +805,18 @@
         default: Union[None, datetime.datetime, Callable[[], datetime.datetime]] = None,
     ):
         super().__init__(
             pa.timestamp(unit, tz), nullable=nullable, metadata=metadata, validator=validator, default=default
         )
 
     @overload
-    def __get__(self, obj: None, objtype: type) -> Self:
-        ...
+    def __get__(self, obj: None, objtype: type) -> Self: ...
 
     @overload
-    def __get__(self, obj: tables.Table, objtype: type) -> pa.TimestampArray:
-        ...
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.TimestampArray: ...
 
     def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.TimestampArray]:
         if obj is None:
             return self
         return _fast_combine_chunks(obj.table[self.name])
 
 
@@ -887,20 +847,18 @@
         default: Union[None, datetime.time, Callable[[], datetime.time]] = None,
     ):
         super().__init__(
             pa.time32(unit), nullable=nullable, metadata=metadata, validator=validator, default=default
         )
 
     @overload
-    def __get__(self, obj: None, objtype: type) -> Self:
-        ...
+    def __get__(self, obj: None, objtype: type) -> Self: ...
 
     @overload
-    def __get__(self, obj: tables.Table, objtype: type) -> pa.Time32Array:
-        ...
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.Time32Array: ...
 
     def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.Time32Array]:
         if obj is None:
             return self
         return _fast_combine_chunks(obj.table[self.name])
 
 
@@ -931,20 +889,18 @@
         default: Union[None, datetime.time, Callable[[], datetime.time]] = None,
     ):
         super().__init__(
             pa.time64(unit), nullable=nullable, metadata=metadata, validator=validator, default=default
         )
 
     @overload
-    def __get__(self, obj: None, objtype: type) -> Self:
-        ...
+    def __get__(self, obj: None, objtype: type) -> Self: ...
 
     @overload
-    def __get__(self, obj: tables.Table, objtype: type) -> pa.Time64Array:
-        ...
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.Time64Array: ...
 
     def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.Time64Array]:
         if obj is None:
             return self
         return _fast_combine_chunks(obj.table[self.name])
 
 
@@ -965,20 +921,18 @@
         nullable: bool = False,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.duration(unit), nullable=nullable, metadata=metadata, validator=validator)
 
     @overload
-    def __get__(self, obj: None, objtype: type) -> Self:
-        ...
+    def __get__(self, obj: None, objtype: type) -> Self: ...
 
     @overload
-    def __get__(self, obj: tables.Table, objtype: type) -> pa.DurationArray:
-        ...
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.DurationArray: ...
 
     def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.DurationArray]:
         if obj is None:
             return self
         return _fast_combine_chunks(obj.table[self.name])
 
 
@@ -1001,20 +955,18 @@
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(
             pa.month_day_nano_interval(), nullable=nullable, metadata=metadata, validator=validator
         )
 
     @overload
-    def __get__(self, obj: None, objtype: type) -> Self:
-        ...
+    def __get__(self, obj: None, objtype: type) -> Self: ...
 
     @overload
-    def __get__(self, obj: tables.Table, objtype: type) -> pa.MonthDayNanoIntervalArray:
-        ...
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.MonthDayNanoIntervalArray: ...
 
     def __get__(
         self, obj: Optional[tables.Table], objtype: type
     ) -> Union[Self, pa.MonthDayNanoIntervalArray]:
         if obj is None:
             return self
         return _fast_combine_chunks(obj.table[self.name])
@@ -1031,20 +983,18 @@
         default: Union[None, bytes, Callable[[], bytes]] = None,
     ):
         super().__init__(
             pa.binary(-1), nullable=nullable, metadata=metadata, validator=validator, default=default
         )
 
     @overload
-    def __get__(self, obj: None, objtype: type) -> Self:
-        ...
+    def __get__(self, obj: None, objtype: type) -> Self: ...
 
     @overload
-    def __get__(self, obj: tables.Table, objtype: type) -> pa.BinaryArray:
-        ...
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.BinaryArray: ...
 
     def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.BinaryArray]:
         if obj is None:
             return self
         return _fast_combine_chunks(obj.table[self.name])
 
 
@@ -1069,20 +1019,18 @@
     ):
         self.byte_width = byte_width
         super().__init__(
             pa.binary(byte_width), nullable=nullable, metadata=metadata, validator=validator, default=default
         )
 
     @overload
-    def __get__(self, obj: None, objtype: type) -> Self:
-        ...
+    def __get__(self, obj: None, objtype: type) -> Self: ...
 
     @overload
-    def __get__(self, obj: tables.Table, objtype: type) -> pa.FixedSizeBinaryArray:
-        ...
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.FixedSizeBinaryArray: ...
 
     def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.FixedSizeBinaryArray]:
         if obj is None:
             return self
         return _fast_combine_chunks(obj.table[self.name])
 
 
@@ -1123,20 +1071,18 @@
         default: Union[None, decimal.Decimal, Callable[[], decimal.Decimal]] = None,
     ):
         super().__init__(
             pa.decimal128(precision, scale), nullable=nullable, metadata=metadata, default=default
         )
 
     @overload
-    def __get__(self, obj: None, objtype: type) -> Self:
-        ...
+    def __get__(self, obj: None, objtype: type) -> Self: ...
 
     @overload
-    def __get__(self, obj: tables.Table, objtype: type) -> pa.Decimal128Array:
-        ...
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.Decimal128Array: ...
 
     def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.Decimal128Array]:
         if obj is None:
             return self
         return _fast_combine_chunks(obj.table[self.name])
 
 
@@ -1167,20 +1113,18 @@
         default: Union[None, decimal.Decimal, Callable[[], decimal.Decimal]] = None,
     ):
         super().__init__(
             pa.decimal256(precision, scale), nullable=nullable, metadata=metadata, default=default
         )
 
     @overload
-    def __get__(self, obj: None, objtype: type) -> Self:
-        ...
+    def __get__(self, obj: None, objtype: type) -> Self: ...
 
     @overload
-    def __get__(self, obj: tables.Table, objtype: type) -> pa.Decimal256Array:
-        ...
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.Decimal256Array: ...
 
     def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.Decimal256Array]:
         if obj is None:
             return self
         return _fast_combine_chunks(obj.table[self.name])
 
 
@@ -1196,20 +1140,18 @@
         self,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.null(), nullable=True, metadata=metadata, validator=validator)
 
     @overload
-    def __get__(self, obj: None, objtype: type) -> Self:
-        ...
+    def __get__(self, obj: None, objtype: type) -> Self: ...
 
     @overload
-    def __get__(self, obj: tables.Table, objtype: type) -> pa.NullArray:
-        ...
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.NullArray: ...
 
     def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.NullArray]:
         if obj is None:
             return self
         return _fast_combine_chunks(obj.table[self.name])
 
 
@@ -1239,20 +1181,18 @@
         validator: Optional[validators.Validator] = None,
     ):
         if isinstance(value_type, Column):
             value_type = value_type.dtype
         super().__init__(pa.list_(value_type, -1), nullable=nullable, metadata=metadata, validator=validator)
 
     @overload
-    def __get__(self, obj: None, objtype: type) -> Self:
-        ...
+    def __get__(self, obj: None, objtype: type) -> Self: ...
 
     @overload
-    def __get__(self, obj: tables.Table, objtype: type) -> pa.ListArray:
-        ...
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.ListArray: ...
 
     def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.ListArray]:
         if obj is None:
             return self
         return _fast_combine_chunks(obj.table[self.name])
 
 
@@ -1284,20 +1224,18 @@
         if isinstance(value_type, Column):
             value_type = value_type.dtype
         super().__init__(
             pa.list_(value_type, list_size), nullable=nullable, metadata=metadata, validator=validator
         )
 
     @overload
-    def __get__(self, obj: None, objtype: type) -> Self:
-        ...
+    def __get__(self, obj: None, objtype: type) -> Self: ...
 
     @overload
-    def __get__(self, obj: tables.Table, objtype: type) -> pa.FixedSizeListArray:
-        ...
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.FixedSizeListArray: ...
 
     def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.FixedSizeListArray]:
         if obj is None:
             return self
         return _fast_combine_chunks(obj.table[self.name])
 
 
@@ -1326,20 +1264,18 @@
         validator: Optional[validators.Validator] = None,
     ):
         if isinstance(value_type, Column):
             value_type = value_type.dtype
         super().__init__(pa.large_list(value_type), nullable=nullable, metadata=metadata, validator=validator)
 
     @overload
-    def __get__(self, obj: None, objtype: type) -> Self:
-        ...
+    def __get__(self, obj: None, objtype: type) -> Self: ...
 
     @overload
-    def __get__(self, obj: tables.Table, objtype: type) -> pa.LargeListArray:
-        ...
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.LargeListArray: ...
 
     def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.LargeListArray]:
         if obj is None:
             return self
         return _fast_combine_chunks(obj.table[self.name])
 
 
@@ -1369,20 +1305,18 @@
         if isinstance(item_type, Column):
             item_type = item_type.dtype
         super().__init__(
             pa.map_(key_type, item_type), nullable=nullable, metadata=metadata, validator=validator
         )
 
     @overload
-    def __get__(self, obj: None, objtype: type) -> Self:
-        ...
+    def __get__(self, obj: None, objtype: type) -> Self: ...
 
     @overload
-    def __get__(self, obj: tables.Table, objtype: type) -> pa.MapArray:
-        ...
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.MapArray: ...
 
     def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.MapArray]:
         if obj is None:
             return self
         return _fast_combine_chunks(obj.table[self.name])
 
 
@@ -1417,20 +1351,18 @@
             pa.dictionary(index_type, value_type, ordered=ordered),
             nullable=nullable,
             metadata=metadata,
             validator=validator,
         )
 
     @overload
-    def __get__(self, obj: None, objtype: type) -> Self:
-        ...
+    def __get__(self, obj: None, objtype: type) -> Self: ...
 
     @overload
-    def __get__(self, obj: tables.Table, objtype: type) -> pa.DictionaryArray:
-        ...
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.DictionaryArray: ...
 
     def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.DictionaryArray]:
         if obj is None:
             return self
         return _fast_combine_chunks(obj.table[self.name])
```

### Comparing `quivr-0.7.2a1/quivr/concat.py` & `quivr-0.7.3a1/quivr/concat.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from typing import Iterator
+from typing import Iterable, List
 
 import pyarrow as pa
 
 from . import defragment, errors, tables
 
 
-def concatenate(values: Iterator[tables.AnyTable], defrag: bool = True) -> tables.AnyTable:
+def concatenate(values: Iterable[tables.AnyTable], defrag: bool = True) -> tables.AnyTable:
     """Concatenate a collection of Tables into a single Table.
 
     All input Tables be of the same class, and have the same attribute
     values (if any).
 
     By default, results are compacted to be contiguous in memory,
     which involves a copy. In a tight loop, this can be very
@@ -18,32 +18,46 @@
     the result after the loop is complete.
 
     :param values: An iterator of :class:`Table` instances to concatenate.
     :param defrag: Whether to compact the result to be contiguous in
         memory. Defaults to True.
 
     """
+    values_list: List[tables.AnyTable] = list(values)
+
+    if len(values_list) == 0:
+        raise ValueError("No values to concatenate")
+
     batches = []
-    first = True
-    for v in values:
-        batches += v.table.to_batches()
-        if first:
+    first_full = False
+
+    # Find the first non-empty table to get the class
+    for v in values_list:
+        if not first_full and len(v) > 0:
             first_cls = v.__class__
             first_val = v
-            first = False
-        else:
-            if v.__class__ != first_cls:
-                raise errors.TablesNotCompatibleError("All tables must be the same class to concatenate")
-            if not first_val._attr_equal(v):
-                raise errors.TablesNotCompatibleError(
-                    "All tables must have the same attribute values to concatenate"
-                )
+            first_full = True
+            break
 
-    if first:
-        raise ValueError("No values to concatenate")
+    # No non-empty tables found so lets pick the first table
+    # to get the class and attributes
+    if not first_full:
+        first_cls = values_list[0].__class__
+        first_val = values_list[0]
+
+    # Scan the values and now make sure they are all the same class
+    # as the first non-empty table
+    for v in values_list:
+        batches += v.table.to_batches()
+        if v.__class__ != first_cls:
+            raise errors.TablesNotCompatibleError("All tables must be the same class to concatenate")
+        if not first_val._attr_equal(v) and len(v) > 0:
+            raise errors.TablesNotCompatibleError(
+                "All non-empty tables must have the same attribute values to concatenate"
+            )
 
     if len(batches) == 0:
         return first_cls.empty()
 
     table = pa.Table.from_batches(batches)
     result = first_cls.from_pyarrow(table=table)
     if defrag:
```

### Comparing `quivr-0.7.2a1/quivr/errors.py` & `quivr-0.7.3a1/quivr/errors.py`

 * *Files identical despite different names*

### Comparing `quivr-0.7.2a1/quivr/linkage.py` & `quivr-0.7.3a1/quivr/linkage.py`

 * *Files 0% similar despite different names*

```diff
@@ -418,20 +418,20 @@
 def _concatenate_linkage_components(
     left_tables: List[LeftTable],
     right_tables: List[RightTable],
     left_keys: List[pa.Array],
     right_keys: List[pa.Array],
 ) -> Tuple[LeftTable, RightTable, pa.Array, pa.Array]:
     try:
-        left_table: LeftTable = concat.concatenate(left_tables)  # type: ignore
+        left_table: LeftTable = concat.concatenate(left_tables)
     except errors.TablesNotCompatibleError as e:
         raise errors.LinkageCombinationError("Left tables are not compatible") from e
 
     try:
-        right_table: RightTable = concat.concatenate(right_tables)  # type: ignore
+        right_table: RightTable = concat.concatenate(right_tables)
     except errors.TablesNotCompatibleError as e:
         raise errors.LinkageCombinationError("Right tables are not compatible") from e
 
     try:
         left_keys = pa.concat_arrays(left_keys)
     except pa.lib.ArrowInvalid as e:
         raise errors.LinkageCombinationError("Left keys types are not all identical") from e
```

### Comparing `quivr-0.7.2a1/quivr/schemagraph.py` & `quivr-0.7.3a1/quivr/schemagraph.py`

 * *Files identical despite different names*

### Comparing `quivr-0.7.2a1/quivr/tables.py` & `quivr-0.7.3a1/quivr/tables.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,24 +40,24 @@
 
 
 class ArrowArrayProvider(Protocol):
     """
     A Protocol which describes objects that support the Arrow custom array extension protocol.
     """
 
-    def __arrow_array__(self, type: Optional[pa.DataType] = None) -> pa.Array:
-        ...
+    def __arrow_array__(self, type: Optional[pa.DataType] = None) -> pa.Array: ...
 
 
 AttributeValueType: TypeAlias = Union[int, float, str]
 DataSourceType: TypeAlias = Union[
-    pa.Array, list[Any], "Table", pd.Series, npt.NDArray[Any], ArrowArrayProvider
+    pa.Array, list[Any], "Table", "pd.Series[Any]", npt.NDArray[Any], "ArrowArrayProvider"
 ]
 AnyTable = TypeVar("AnyTable", bound="Table")
 
+
 # If a table uses any of the following names, it will break quivr
 # internals entirely, so they must be rejected.
 _FORBIDDEN_COLUMN_NAMES = {
     "table",
     "schema",
     "_quivr_subtables",
     "_quivr_attributes",
```

### Comparing `quivr-0.7.2a1/quivr/validators.py` & `quivr-0.7.3a1/quivr/validators.py`

 * *Files identical despite different names*

### Comparing `quivr-0.7.2a1/quivr/experimental/shmem.py` & `quivr-0.7.3a1/quivr/experimental/shmem.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,16 +90,15 @@
     """
     A partitioning strategy for executing a function in parallel on a Table.
 
     This class is abstract and should be subclassed to implement a particular partitioning strategy.
     """
 
     @abc.abstractmethod
-    def partition(self, table: T) -> Iterator[T]:
-        ...
+    def partition(self, table: T) -> Iterator[T]: ...
 
 
 def partition_func(f: Callable[[T], Iterator[T]]) -> Partitioning:
     """
     Defines a partitioning strategy by providing a function that partitions a
     Table into multiple Tables.
     """
```

### Comparing `quivr-0.7.2a1/LICENSE` & `quivr-0.7.3a1/LICENSE`

 * *Files identical despite different names*

### Comparing `quivr-0.7.2a1/README.md` & `quivr-0.7.3a1/README.md`

 * *Files identical despite different names*

### Comparing `quivr-0.7.2a1/pyproject.toml` & `quivr-0.7.3a1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
   "typecheck",
   "test",
 ]
 fix = [
   "ruff ./quivr ./test --fix"
 ]
 lint = [
-  "ruff ./quivr ./test",
+  "ruff check ./quivr ./test",
   "black --check ./quivr ./test",
   "isort --check-only ./quivr ./test"
 ]
 format = [
   "black ./quivr ./test",
   "isort ./quivr ./test"
 ]
```

### Comparing `quivr-0.7.2a1/PKG-INFO` & `quivr-0.7.3a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: quivr
-Version: 0.7.2a1
+Version: 0.7.3a1
 Summary: Container library for working with tabular Arrow data
 Project-URL: Source, https://github.com/spenczar/quivr
 Author-email: Spencer Nelson <spencer@spencerwnelson.com>
 License-File: LICENSE
 Requires-Python: >=3.9
 Requires-Dist: mmh3
 Requires-Dist: numpy
```

