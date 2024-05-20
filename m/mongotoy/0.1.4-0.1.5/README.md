# Comparing `tmp/mongotoy-0.1.4.tar.gz` & `tmp/mongotoy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongotoy-0.1.4.tar", max compression
+gzip compressed data, was "mongotoy-0.1.5.tar", max compression
```

## Comparing `mongotoy-0.1.4.tar` & `mongotoy-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11558 2024-02-23 16:52:07.516625 mongotoy-0.1.4/LICENSE
--rw-r--r--   0        0        0      151 2024-04-06 23:50:55.339800 mongotoy-0.1.4/mongotoy/__init__.py
--rw-r--r--   0        0        0     2342 2024-03-18 19:02:50.653179 mongotoy-0.1.4/mongotoy/cache.py
--rw-r--r--   0        0        0    49515 2024-04-17 16:33:55.586760 mongotoy-0.1.4/mongotoy/db.py
--rw-r--r--   0        0        0    16382 2024-04-04 16:29:46.366685 mongotoy-0.1.4/mongotoy/documents.py
--rw-r--r--   0        0        0     6693 2024-04-03 17:32:35.942331 mongotoy-0.1.4/mongotoy/errors.py
--rw-r--r--   0        0        0     7731 2024-04-15 16:35:24.067748 mongotoy-0.1.4/mongotoy/expressions.py
--rw-r--r--   0        0        0    11917 2024-04-04 15:54:56.024009 mongotoy-0.1.4/mongotoy/fields.py
--rw-r--r--   0        0        0     2231 2024-03-18 19:06:51.253634 mongotoy-0.1.4/mongotoy/geodata.py
--rw-r--r--   0        0        0    40200 2024-04-17 18:30:39.172399 mongotoy-0.1.4/mongotoy/mappers.py
--rw-r--r--   0        0        0     5415 2024-04-04 16:29:08.681600 mongotoy-0.1.4/mongotoy/references.py
--rw-r--r--   0        0        0     1813 2024-04-07 17:20:09.221000 mongotoy-0.1.4/mongotoy/sync.py
--rw-r--r--   0        0        0    11992 2024-04-17 17:44:47.007889 mongotoy-0.1.4/mongotoy/types.py
--rw-r--r--   0        0        0      715 2024-04-17 19:01:28.715731 mongotoy-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     6484 2024-04-14 05:31:35.928668 mongotoy-0.1.4/README.md
--rw-r--r--   0        0        0     7128 1970-01-01 00:00:00.000000 mongotoy-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11558 2024-02-23 16:52:07.516625 mongotoy-0.1.5/LICENSE
+-rw-r--r--   0        0        0      151 2024-04-06 23:50:55.339800 mongotoy-0.1.5/mongotoy/__init__.py
+-rw-r--r--   0        0        0     2342 2024-03-18 19:02:50.653179 mongotoy-0.1.5/mongotoy/cache.py
+-rw-r--r--   0        0        0    49525 2024-05-20 17:47:01.468567 mongotoy-0.1.5/mongotoy/db.py
+-rw-r--r--   0        0        0    16382 2024-04-04 16:29:46.366685 mongotoy-0.1.5/mongotoy/documents.py
+-rw-r--r--   0        0        0     6693 2024-04-03 17:32:35.942331 mongotoy-0.1.5/mongotoy/errors.py
+-rw-r--r--   0        0        0     7731 2024-04-15 16:35:24.067748 mongotoy-0.1.5/mongotoy/expressions.py
+-rw-r--r--   0        0        0    13701 2024-05-20 17:54:14.699669 mongotoy-0.1.5/mongotoy/fields.py
+-rw-r--r--   0        0        0     2231 2024-03-18 19:06:51.253634 mongotoy-0.1.5/mongotoy/geodata.py
+-rw-r--r--   0        0        0    41495 2024-05-20 18:10:48.581789 mongotoy-0.1.5/mongotoy/mappers.py
+-rw-r--r--   0        0        0     5415 2024-04-04 16:29:08.681600 mongotoy-0.1.5/mongotoy/references.py
+-rw-r--r--   0        0        0     1813 2024-04-07 17:20:09.221000 mongotoy-0.1.5/mongotoy/sync.py
+-rw-r--r--   0        0        0    11992 2024-04-17 17:44:47.007889 mongotoy-0.1.5/mongotoy/types.py
+-rw-r--r--   0        0        0      715 2024-05-20 18:16:56.043236 mongotoy-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     6484 2024-04-14 05:31:35.928668 mongotoy-0.1.5/README.md
+-rw-r--r--   0        0        0     7128 1970-01-01 00:00:00.000000 mongotoy-0.1.5/PKG-INFO
```

### Comparing `mongotoy-0.1.4/LICENSE` & `mongotoy-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mongotoy-0.1.4/mongotoy/cache.py` & `mongotoy-0.1.5/mongotoy/cache.py`

 * *Files identical despite different names*

### Comparing `mongotoy-0.1.4/mongotoy/db.py` & `mongotoy-0.1.5/mongotoy/db.py`

 * *Files 0% similar despite different names*

```diff
@@ -993,15 +993,15 @@
             value (typing.Any): The identifier value.
 
         Returns:
             T: The parsed document instance.
         """
         # noinspection PyProtectedMember
         return await self.filter(
-            self._document_cls.id == self._document_cls.id._field.mapper.validate(value)
+            self._document_cls.id == self._document_cls.id._field.mapper.__validate_value__(value)
         )._fetch_one()
 
     async def _count(self) -> int:
         """
         Counts the number of documents in the result set.
 
         Returns:
```

### Comparing `mongotoy-0.1.4/mongotoy/documents.py` & `mongotoy-0.1.5/mongotoy/documents.py`

 * *Files identical despite different names*

### Comparing `mongotoy-0.1.4/mongotoy/errors.py` & `mongotoy-0.1.5/mongotoy/errors.py`

 * *Files identical despite different names*

### Comparing `mongotoy-0.1.4/mongotoy/expressions.py` & `mongotoy-0.1.5/mongotoy/expressions.py`

 * *Files identical despite different names*

### Comparing `mongotoy-0.1.4/mongotoy/fields.py` & `mongotoy-0.1.5/mongotoy/fields.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,42 +37,80 @@
         alias: str = None,
         id_field: bool = False,
         default: typing.Any = expressions.EmptyValue,
         default_factory: typing.Callable[[], typing.Any] = None,
         index: expressions.IndexType = None,
         sparse: bool = False,
         unique: bool = False,
+        lt: typing.Any = None,
+        lte: typing.Any = None,
+        gt: typing.Any = None,
+        gte: typing.Any = None,
+        min_items: typing.Optional[int] = None,
+        max_items: typing.Optional[int] = None,
+        min_len: typing.Optional[int] = None,
+        max_len: typing.Optional[int] = None,
+        choices: typing.Optional[list[str]] = None,
         **extra
 ) -> FieldOptions:
     """
     Create a field descriptor for a document.
 
     Args:
         alias (str, optional): Alias for the field. Defaults to None.
         id_field (bool, optional): Indicates if the field is an ID field. Defaults to False.
         default (Any, optional): Default value for the field. Defaults to EmptyValue.
         default_factory (Callable[[], Any], optional): Factory function for generating default values. Defaults to None.
         index (IndexType, optional): Type of index for the field. Defaults to None.
         sparse (bool, optional): Whether the index should be sparse. Defaults to False.
         unique (bool, optional): Whether the index should be unique. Defaults to False.
+        lt (Any): Upper bound for the field value
+        lte (Any): Upper bound (inclusive) for the field value
+        gt (Any): Lower bound for the field value
+        gte (Any): Lower bound (inclusive) for the field value
+        min_items (int, optional): Minimum number of items for sequence fields
+        max_items (int, optional): Maximum  number of items for sequence fields
+        min_len (int, optional): Minimum length for string fields
+        max_len (int, optional): Maximum length for string fields
+        choices (list[str], optional): List of allowed choices for string fields
         extra: Extra configurations
 
     Returns:
         FieldOptions: Field descriptor.
 
     """
+    extra_configs = {**extra}
+    if lt is not None:
+        extra_configs['lt'] = lt
+    if lte is not None:
+        extra_configs['lte'] = lte
+    if gt is not None:
+        extra_configs['gt'] = gt
+    if gte is not None:
+        extra_configs['gte'] = gte
+    if min_items is not None:
+        extra_configs['min_items'] = min_items
+    if max_items is not None:
+        extra_configs['max_items'] = max_items
+    if min_len is not None:
+        extra_configs['min_len'] = min_len
+    if max_len is not None:
+        extra_configs['max_len'] = max_len
+    if choices:
+        extra_configs['choices'] = choices
+
     return FieldOptions(
         alias=alias,
         id_field=id_field,
         default=default,
         default_factory=default_factory,
         index=index,
         sparse=sparse,
         unique=unique,
-        extra=extra
+        extra=extra_configs
     )
 
 
 def reference(ref_field: str = 'id', key_name: str = None) -> FieldOptions:
     """
     Create a reference field descriptor for a document.
 
@@ -169,15 +207,18 @@
 
         Returns:
             Any: The value of the field.
 
         """
         if not instance:
             return FieldProxy(self)
-        return instance.__data__.get(self.name, expressions.EmptyValue)
+        value = instance.__data__.get(self.name, expressions.EmptyValue)
+        if value in (expressions.EmptyValue, None):
+            return value
+        return self.mapper.dump_value(value)
 
     def __set__(self, instance, value):
         """
         Set the value of the field.
 
         Args:
             instance: The instance of the owner class.
@@ -219,15 +260,17 @@
             Any: The validated value.
 
         Raises:
             ValidationError: If validation fails.
 
         """
         try:
+            # Validate value
             value = self.mapper(value)
+
             # Check id value
             if self.alias == '_id' and value is expressions.EmptyValue:
                 raise ValidationError([
                     ErrorWrapper(loc=tuple(), error=ValueError('Id field value required'))
                 ])
         except ValidationError as e:
             raise ValidationError(
```

### Comparing `mongotoy-0.1.4/mongotoy/geodata.py` & `mongotoy-0.1.5/mongotoy/geodata.py`

 * *Files identical despite different names*

### Comparing `mongotoy-0.1.4/mongotoy/mappers.py` & `mongotoy-0.1.5/mongotoy/mappers.py`

 * *Files 11% similar despite different names*

```diff
@@ -168,15 +168,15 @@
 
     def __init__(self, options: MapperOptions):
         self._options = options
         self._default_factory = options.default_factory if options.default_factory else lambda: options.default
 
     def __call__(self, value) -> typing.Any:
         """
-        Validate the value against the mapper.
+        Validate the value.
 
         Args:
             value (Any): The value to be validated.
 
         Raises:
             ValueError: If the value is invalid.
 
@@ -191,47 +191,60 @@
 
         try:
             if value is None:
                 if not self._options.nullable:
                     raise ValueError('Null value not allowed')
                 return value
 
-            value = self.validate(value)
+            value = self.__validate_value__(value)
         except (TypeError, ValueError) as e:
             raise ValidationError(errors=[ErrorWrapper(loc=tuple(), error=e)]) from None
 
         return value
 
     @abc.abstractmethod
-    def validate(self, value) -> typing.Any:
+    def __validate_value__(self, value) -> typing.Any:
         """
-        Validate the value.
+        Abstract validator to be implemented in child mappers.
 
         Args:
             value: The value to be validated.
 
         Returns:
             Any: The validated value.
 
         """
         raise NotImplementedError
 
+    def dump_value(self, value) -> typing.Any:
+        """
+        Dump the value to be access direct from object instance.
+
+        Args:
+            value: The value to be dumped.
+
+        Returns:
+            Any: The dumped value.
+
+        """
+        return value
+
     def dump_dict(self, value, **options) -> typing.Any:
         """
         Dump the value to be in a dictionary.
 
         Args:
             value: The value to be dumped.
             **options: Additional options.
 
         Returns:
             Any: The dumped value.
 
         """
-        return value
+        return self.dump_value(value)
 
     def dump_json(self, value, **options) -> typing.Any:
         """
         Dump the value to valid JSON.
 
         Args:
             value: The value to be dumped.
@@ -263,15 +276,15 @@
     Base mapper for data types supporting the following comparators:
     - lt (less than)
     - lte (less than or equal to)
     - gt (greater than)
     - gte (greater than or equal to)
     """
 
-    def validate(self, value) -> typing.Any:
+    def __validate_value__(self, value) -> typing.Any:
         """
         Validate the input value against the specified comparators.
         Args:
             value: The value to be validated.
         Returns:
             The validated value.
         Raises:
@@ -342,15 +355,15 @@
         """Get the innermost mapper that isn't a SequenceMapper"""
         mapper_ = self.mapper
         while isinstance(mapper_, SequenceMapper):
             mapper_ = mapper_.mapper
         return mapper_
 
     # noinspection PyTypeChecker
-    def validate(self, value) -> typing.Any:
+    def __validate_value__(self, value) -> typing.Any:
         """
         Validate the list value.
 
         Args:
             value: The list value to be validated.
 
         Returns:
@@ -386,15 +399,15 @@
         if errors:
             raise ValidationError(errors=errors)
 
         return self.__bind__(new_value)
 
     def dump_dict(self, value, **options) -> typing.Any:
         """
-        Dump the list value to a dictionary.
+        Dump the list value to be in a dictionary.
 
         Args:
             value: The list value to be dumped.
             **options: Additional options.
 
         Returns:
             Any: The dumped list value.
@@ -458,15 +471,15 @@
         Returns:
             Type['documents.BaseDocument']: The class of the embedded document.
 
         """
         from mongotoy import documents
         return documents.get_embedded_document_cls(self._document_cls)
 
-    def validate(self, value) -> typing.Any:
+    def __validate_value__(self, value) -> typing.Any:
         """
         Validate the embedded document value.
 
         Args:
             value: The value to be validated.
 
         Returns:
@@ -540,28 +553,28 @@
         document_cls: typing.Type['documents.BaseDocument'] | str,
         options: MapperOptions
     ):
         if not options.ref_field:
             options.ref_field = 'id'
         super().__init__(document_cls, options)
 
-    def validate(self, value) -> typing.Any:
+    def __validate_value__(self, value) -> typing.Any:
         """
         Validate the referenced document value.
 
         Args:
             value: The value to be validated.
 
         Returns:
             Any: The validated value.
 
         Raises:
             ValueError: If validation fails due to missing referenced field value.
         """
-        value = super().validate(value)
+        value = super().__validate_value__(value)
         if getattr(value, self.ref_field.name) is expressions.EmptyValue:
             raise ValueError(
                 f'Referenced field {self.document_cls.__name__}.{self.ref_field.name} value required'
             )
         return value
 
     @property
@@ -604,15 +617,15 @@
 
 
 class StrMapper(Mapper, bind=str):
     """
     Mapper for handling string values.
     """
 
-    def validate(self, value) -> typing.Any:
+    def __validate_value__(self, value) -> typing.Any:
         """
         Validate the string value.
 
         Args:
             value: The value to be validated.
 
         Returns:
@@ -659,15 +672,15 @@
 
 
 class DecimalMapper(ComparableMapper, bind=decimal.Decimal):
     """
     Mapper for handling decimal values.
     """
 
-    def validate(self, value) -> typing.Any:
+    def __validate_value__(self, value) -> typing.Any:
         """
         Validate the decimal value.
 
         Args:
             value: The value to be validated.
 
         Returns:
@@ -675,15 +688,15 @@
 
         Raises:
             TypeError: If validation fails due to incorrect data type.
 
         """
         if isinstance(value, bson.Decimal128):
             value = value.to_decimal()
-        value = super().validate(value)
+        value = super().__validate_value__(value)
         # Ensure decimal limits for MongoDB
         # https://www.mongodb.com/docs/upcoming/release-notes/3.4/#decimal-type
         ctx = decimal.Context(prec=34)
         return ctx.create_decimal(value)
 
     def dump_json(self, value, **options) -> typing.Any:
         """
@@ -715,15 +728,15 @@
 
 
 class BoolMapper(Mapper, bind=bool):
     """
     Mapper for handling boolean values.
     """
 
-    def validate(self, value) -> typing.Any:
+    def __validate_value__(self, value) -> typing.Any:
         """
         Validate the boolean value.
 
         Args:
             value: The value to be validated.
 
         Returns:
@@ -739,15 +752,15 @@
 
 
 class BinaryMapper(Mapper, bind=bytes):
     """
     Mapper for handling binary values.
     """
 
-    def validate(self, value) -> typing.Any:
+    def __validate_value__(self, value) -> typing.Any:
         """
         Validate the binary value.
 
         Args:
             value: The value to be validated.
 
         Returns:
@@ -778,15 +791,15 @@
 
 
 class UUIDMapper(Mapper, bind=uuid.UUID):
     """
     Mapper for handling UUID values.
     """
 
-    def validate(self, value) -> typing.Any:
+    def __validate_value__(self, value) -> typing.Any:
         """
         Validate the UUID value.
 
         Args:
             value: The value to be validated.
 
         Returns:
@@ -796,28 +809,38 @@
             TypeError: If validation fails due to incorrect data type.
 
         """
         if not isinstance(value, uuid.UUID):
             raise TypeError(f'Invalid data type {type(value)}, required is {uuid.UUID}')
         return value
 
+    def dump_value(self, value) -> typing.Any:
+        if self._options.extra.get('dump_as_str', False):
+            return str(value)
+        return value
+
     def dump_json(self, value, **options) -> typing.Any:
         """
         Dump the UUID value to a JSON-serializable format.
 
         Args:
             value: The value to be dumped.
             **options: Additional options.
 
         Returns:
             Any: The dumped value.
 
         """
         return str(value)
 
+    def dump_bson(self, value, **options) -> typing.Any:
+        if self._options.extra.get('dump_bson_as_str', False):
+            return str(value)
+        return value
+
 
 class DateTimeMapper(ComparableMapper, bind=datetime.datetime):
     """
     Mapper for handling datetime values.
     """
 
     def dump_json(self, value, **options) -> typing.Any:
@@ -836,15 +859,15 @@
 
 
 class DateMapper(ComparableMapper, bind=datetime.date):
     """
     Mapper for handling date values.
     """
 
-    def validate(self, value) -> typing.Any:
+    def __validate_value__(self, value) -> typing.Any:
         """
         Validate the date value.
 
         Args:
             value: The value to be validated.
 
         Returns:
@@ -852,15 +875,15 @@
 
         Raises:
             TypeError: If validation fails due to incorrect data type.
 
         """
         if isinstance(value, datetime.datetime):
             value = value.date()
-        return super().validate(value)
+        return super().__validate_value__(value)
 
     def dump_json(self, value, **options) -> typing.Any:
         """
         Dump the date value to a JSON-serializable format.
 
         Args:
             value: The value to be dumped.
@@ -888,15 +911,15 @@
 
 
 class TimeMapper(ComparableMapper, bind=datetime.time):
     """
     Mapper for handling time values.
     """
 
-    def validate(self, value) -> typing.Any:
+    def __validate_value__(self, value) -> typing.Any:
         """
         Validate the time value.
 
         Args:
             value: The value to be validated.
 
         Returns:
@@ -904,15 +927,15 @@
 
         Raises:
             TypeError: If validation fails due to incorrect data type.
 
         """
         if isinstance(value, datetime.datetime):
             value = value.time()
-        return super().validate(value)
+        return super().__validate_value__(value)
 
     def dump_json(self, value, **options) -> typing.Any:
         """
         Dump the time value to a JSON-serializable format.
 
         Args:
             value: The value to be dumped.
@@ -951,46 +974,46 @@
 class TupleMapper(SequenceMapper, bind=tuple):
     """
     Mapper for handling tuples.
 
     Inherits from ManyMapper and specifies 'tuple' as the binding type.
 
     """
-    def validate(self, value) -> typing.Any:
+    def __validate_value__(self, value) -> typing.Any:
         if isinstance(value, list):
             value = tuple(value)
-        return super().validate(value)
+        return super().__validate_value__(value)
 
 
 class SetMapper(SequenceMapper, bind=set):
     """
     Mapper for handling sets.
 
     Inherits from ManyMapper and specifies 'set' as the binding type.
 
     """
 
-    def validate(self, value) -> typing.Any:
+    def __validate_value__(self, value) -> typing.Any:
         if isinstance(value, list):
             value = set(value)
-        return super().validate(value)
+        return super().__validate_value__(value)
 
     def dump_json(self, value, **options) -> typing.Any:
         return list(value)
 
     def dump_bson(self, value, **options) -> typing.Any:
         return list(value)
 
 
 class ObjectIdMapper(Mapper, bind=bson.ObjectId):
     """
     Mapper for handling BSON ObjectId values.
     """
 
-    def validate(self, value) -> typing.Any:
+    def __validate_value__(self, value) -> typing.Any:
         """
         Validate the ObjectId value.
 
         Args:
             value: The value to be validated.
 
         Returns:
@@ -1000,14 +1023,19 @@
             TypeError: If validation fails due to incorrect data type.
 
         """
         if not bson.ObjectId.is_valid(value):
             raise TypeError(f'Invalid data type {type(value)}, required is {bson.ObjectId}')
         return bson.ObjectId(value)
 
+    def dump_value(self, value) -> typing.Any:
+        if self._options.extra.get('dump_as_str', False):
+            return str(value)
+        return value
+
     def dump_json(self, value, **options) -> typing.Any:
         """
         Dump the ObjectId value to a JSON-serializable format.
 
         Args:
             value: The value to be dumped.
             **options: Additional options.
@@ -1020,15 +1048,15 @@
 
 
 class Int64Mapper(Mapper, bind=bson.Int64):
     """
     Mapper for handling BSON Int64 values.
     """
 
-    def validate(self, value) -> typing.Any:
+    def __validate_value__(self, value) -> typing.Any:
         """
         Validate the Int64 value.
 
         Args:
             value: The value to be validated.
 
         Returns:
@@ -1058,15 +1086,15 @@
 
 
 class Decimal128Mapper(Mapper, bind=bson.Decimal128):
     """
     Mapper for handling BSON Decimal128 values.
     """
 
-    def validate(self, value) -> typing.Any:
+    def __validate_value__(self, value) -> typing.Any:
         """
         Validate the Decimal128 value.
 
         Args:
             value: The value to be validated.
 
         Returns:
@@ -1096,15 +1124,15 @@
 
 
 class RegexMapper(Mapper, bind=bson.Regex):
     """
     Mapper for handling BSON Regex values.
     """
 
-    def validate(self, value) -> typing.Any:
+    def __validate_value__(self, value) -> typing.Any:
         """
         Validate the Regex value.
 
         Args:
             value: The value to be validated.
 
         Returns:
@@ -1134,15 +1162,15 @@
 
 
 class CodeMapper(Mapper, bind=bson.Code):
     """
     Mapper for handling BSON Code values.
     """
 
-    def validate(self, value) -> typing.Any:
+    def __validate_value__(self, value) -> typing.Any:
         """
         Validate the Code value.
 
         Args:
             value: The value to be validated.
 
         Returns:
@@ -1172,26 +1200,31 @@
 
 
 class ConstrainedStrMapper(StrMapper):
     """
     Mapper for handling constrained string values.
     """
 
-    def validate(self, value) -> typing.Any:
+    def __validate_value__(self, value) -> typing.Any:
         """
         Validate the string value.
 
         Args:
             value: The value to be validated.
 
         Returns:
             Any: The validated value.
 
         """
-        return self.__bind__(super().validate(value))
+        return self.__bind__(super().__validate_value__(value))
+
+    def dump_value(self, value) -> typing.Any:
+        if self._options.extra.get('dump_as_str', False):
+            return str(value)
+        return value
 
     def dump_json(self, value, **options) -> typing.Any:
         """
         Dump the string value to JSON.
 
         Args:
             value: The value to be dumped.
@@ -1293,15 +1326,15 @@
 class GeometryMapper(Mapper):
     """
     Mapper for handling geometry data.
 
     This mapper validates and handles geometry data.
     """
 
-    def validate(self, value) -> typing.Any:
+    def __validate_value__(self, value) -> typing.Any:
         """
         Validate the geometry data.
 
         Args:
             value (Any): The value to be validated.
 
         Returns:
@@ -1385,15 +1418,15 @@
 class JsonMapper(Mapper, bind=types.Json):
     """
     Mapper for handling JSON data.
 
     This mapper validates and handles JSON data.
     """
 
-    def validate(self, value) -> typing.Any:
+    def __validate_value__(self, value) -> typing.Any:
         """
         Validate the JSON data.
 
         Args:
             value (Any): The JSON data to be validated.
 
         Returns:
@@ -1418,15 +1451,15 @@
 class BsonMapper(Mapper, bind=types.Bson):
     """
     Mapper for handling BSON data.
 
     This mapper validates and handles BSON data.
     """
 
-    def validate(self, value) -> typing.Any:
+    def __validate_value__(self, value) -> typing.Any:
         """
         Validate the BSON data.
 
         Args:
             value (Any): The BSON data to be validated.
 
         Returns:
```

### Comparing `mongotoy-0.1.4/mongotoy/references.py` & `mongotoy-0.1.5/mongotoy/references.py`

 * *Files identical despite different names*

### Comparing `mongotoy-0.1.4/mongotoy/sync.py` & `mongotoy-0.1.5/mongotoy/sync.py`

 * *Files identical despite different names*

### Comparing `mongotoy-0.1.4/mongotoy/types.py` & `mongotoy-0.1.5/mongotoy/types.py`

 * *Files identical despite different names*

### Comparing `mongotoy-0.1.4/README.md` & `mongotoy-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `mongotoy-0.1.4/PKG-INFO` & `mongotoy-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: mongotoy
-Version: 0.1.4
+Version: 0.1.5
 Summary: Comprehensive ODM for MongoDB
 Home-page: https://gurcuff91.github.io/mongotoy
 License: Apache-2.0
 Keywords: mapping,asyncio,odm,mongodb
 Author: gurcuff91
 Author-email: gf.meneses91@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.12,<4.0
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: motor (>=3.4.0,<4.0.0)
 Requires-Dist: pymongo (>=4.6.3,<5.0.0)
 Project-URL: Repository, https://github.com/gurcuff91/mongotoy
 Description-Content-Type: text/markdown
```

