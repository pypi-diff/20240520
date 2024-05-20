# Comparing `tmp/classnotation-1.2.tar.gz` & `tmp/classnotation-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classnotation-1.2.tar", last modified: Thu May  2 19:43:37 2024, max compression
+gzip compressed data, was "classnotation-1.2.1.tar", last modified: Mon May 20 04:11:43 2024, max compression
```

## Comparing `classnotation-1.2.tar` & `classnotation-1.2.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 19:43:37.474299 classnotation-1.2/
--rw-r--r--   0 root         (0) root         (0)      281 2024-05-02 19:43:37.474299 classnotation-1.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 19:43:37.470299 classnotation-1.2/classnotation/
--rw-rw-rw-   0 root         (0) root         (0)      148 2024-05-02 14:45:56.000000 classnotation-1.2/classnotation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8517 2024-05-02 14:45:56.000000 classnotation-1.2/classnotation/dumper.py
--rw-rw-rw-   0 root         (0) root         (0)      235 2024-04-15 05:55:22.000000 classnotation-1.2/classnotation/json_types.py
--rw-rw-rw-   0 root         (0) root         (0)    13140 2024-05-02 19:41:55.000000 classnotation-1.2/classnotation/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 19:43:37.470299 classnotation-1.2/classnotation.egg-info/
--rw-r--r--   0 root         (0) root         (0)      116 2024-05-02 19:43:37.000000 classnotation-1.2/classnotation.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)      465 2024-05-02 19:43:13.000000 classnotation-1.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-02 19:43:37.474299 classnotation-1.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 04:11:43.928415 classnotation-1.2.1/
+-rw-r--r--   0 root         (0) root         (0)      283 2024-05-20 04:11:43.928415 classnotation-1.2.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 04:11:43.928415 classnotation-1.2.1/classnotation/
+-rw-rw-rw-   0 root         (0) root         (0)      148 2024-05-02 14:45:56.000000 classnotation-1.2.1/classnotation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8517 2024-05-02 14:45:56.000000 classnotation-1.2.1/classnotation/dumper.py
+-rw-rw-rw-   0 root         (0) root         (0)      235 2024-04-15 05:55:22.000000 classnotation-1.2.1/classnotation/json_types.py
+-rw-rw-rw-   0 root         (0) root         (0)    13159 2024-05-20 04:11:20.000000 classnotation-1.2.1/classnotation/loader.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 04:11:37.000000 classnotation-1.2.1/classnotation/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 04:11:43.928415 classnotation-1.2.1/classnotation.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      139 2024-05-20 04:11:43.000000 classnotation-1.2.1/classnotation.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)      467 2024-05-20 04:11:20.000000 classnotation-1.2.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-20 04:11:43.928415 classnotation-1.2.1/setup.cfg
```

### Comparing `classnotation-1.2/classnotation/dumper.py` & `classnotation-1.2.1/classnotation/dumper.py`

 * *Files identical despite different names*

### Comparing `classnotation-1.2/classnotation/loader.py` & `classnotation-1.2.1/classnotation/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
                     json_key=json_key,
                     stack=".".join(_stack),
                     dataclass=data_class,
                 )
                 if not self.strict:
                     logging.warning(error_message)
                 else:
-                    raise ValueError(error_message)
+                    raise TypeError(error_message)
 
         try:
             return data_class(**validated_data)
         except TypeError as e:
             print("Error found at", ".".join(_stack)) # TODO: this should be incorporated into the message somehow
             raise e
 
@@ -171,22 +171,22 @@
                 try:
                     return self.validate_field(value, arg, _stack=_stack)
                 except TypeError as e:
                     all_errors.append(e)
 
             if len(all_errors) > 0:
                 # Build an error message that contains the errors from parsing each of the possible types in the union
-                combined_message = "Expected one of union type `{}` at `{}`\n".format(field_type, ".".join(_stack))
+                combined_message: List[str] = ["Expected one of union type `{}` at `{}`".format(field_type, ".".join(_stack))]
                 for i, error in enumerate(all_errors):
                     prefix: str = "  {}: ".format(i)
                     for line in error.args[0].split("\n"):
-                        combined_message += prefix + line + "\n"
+                        combined_message.append(prefix + line)
                         prefix = " " * len(prefix)
 
-                raise TypeError(combined_message)
+                raise TypeError("\n".join(combined_message))
 
         # Literal[]
         elif field_origin == Literal:
             arg_value = get_args(field_type)[0]
             if type(value) is str and type(arg_value) is bytes:
                 value = value.encode("utf-8")
```

