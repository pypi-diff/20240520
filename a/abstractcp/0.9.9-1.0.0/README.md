# Comparing `tmp/abstractcp-0.9.9.tar.gz` & `tmp/abstractcp-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstractcp-0.9.9.tar", last modified: Thu Feb 10 12:42:31 2022, max compression
+gzip compressed data, was "abstractcp-1.0.0.tar", last modified: Mon May 20 07:59:36 2024, max compression
```

## Comparing `abstractcp-0.9.9.tar` & `abstractcp-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-10 12:42:31.919729 abstractcp-0.9.9/
--rw-r--r--   0 runner    (1001) docker     (121)     1053 2022-02-10 12:42:12.000000 abstractcp-0.9.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     9136 2022-02-10 12:42:31.919729 abstractcp-0.9.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8669 2022-02-10 12:42:12.000000 abstractcp-0.9.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-10 12:42:31.915729 abstractcp-0.9.9/abstractcp/
--rw-r--r--   0 runner    (1001) docker     (121)     4765 2022-02-10 12:42:12.000000 abstractcp-0.9.9/abstractcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-10 12:42:12.000000 abstractcp-0.9.9/abstractcp/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-10 12:42:31.919729 abstractcp-0.9.9/abstractcp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9136 2022-02-10 12:42:31.000000 abstractcp-0.9.9/abstractcp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      205 2022-02-10 12:42:31.000000 abstractcp-0.9.9/abstractcp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-10 12:42:31.000000 abstractcp-0.9.9/abstractcp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-02-10 12:42:31.000000 abstractcp-0.9.9/abstractcp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-10 12:42:31.919729 abstractcp-0.9.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      728 2022-02-10 12:42:12.000000 abstractcp-0.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:59:36.218158 abstractcp-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-20 07:59:28.000000 abstractcp-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9026 2024-05-20 07:59:36.218158 abstractcp-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8596 2024-05-20 07:59:28.000000 abstractcp-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:59:36.218158 abstractcp-1.0.0/abstractcp/
+-rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-05-20 07:59:28.000000 abstractcp-1.0.0/abstractcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 07:59:28.000000 abstractcp-1.0.0/abstractcp/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:59:36.218158 abstractcp-1.0.0/abstractcp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9026 2024-05-20 07:59:36.000000 abstractcp-1.0.0/abstractcp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-20 07:59:36.000000 abstractcp-1.0.0/abstractcp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 07:59:36.000000 abstractcp-1.0.0/abstractcp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-20 07:59:36.000000 abstractcp-1.0.0/abstractcp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 07:59:36.218158 abstractcp-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-20 07:59:28.000000 abstractcp-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:59:36.218158 abstractcp-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-05-20 07:59:28.000000 abstractcp-1.0.0/tests/test_define.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-20 07:59:28.000000 abstractcp-1.0.0/tests/test_use.py
```

### Comparing `abstractcp-0.9.9/LICENSE` & `abstractcp-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `abstractcp-0.9.9/PKG-INFO` & `abstractcp-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 Metadata-Version: 2.1
 Name: abstractcp
-Version: 0.9.9
+Version: 1.0.0
 Summary: Create abstract class variables
 Home-page: https://github.com/reinhrst/abstractcp
 Author: Claude El
 Author-email: abstractcp@claude.nl
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # AbstractCP -- Abstract Class Property
 
 ![Tox tests](https://github.com/reinhrst/abstractcp/workflows/Tox%20tests/badge.svg)
 
 
 This package allows one to create classes with abstract class properties.
 The initial code was inspired by [this question][1] (and accepted answer) -- in
-addition to me strugling many time with the same issue in the past.
-I firtst wanted to just post this as separate answer, however since it includes quite
+addition to me struggling many time with the same issue in the past.
+I first wanted to just post this as separate answer, however since it includes quite
 some python magic, and I would like to include quite some tests (and possibly update
 the code in the future), I made it into a package (even though I'm not a big fan of
 small packages that hardly do anything).
 
-The package is python3.6 and higher. I could consider creating a version for pre-3.6;
-if you want that, please create an [issue on github][2].
+The package is python3.8 and higher (version 0.9.9 runs on 3.6-3.11).
 
 ## TL;DR Examples
 Note: the examples use [PEP-526 type hints][3]; this is obviously optional.
 
 All examples assume the following imports:
 ```python
 import tying as t
@@ -194,9 +191,7 @@
 
 If you do this, I would appreciate if you drop me a line, since it probably means you've found a novel use for the package that I'd be happy to learn about (and possibly document).
 
 
 [1]: https://stackoverflow.com/questions/45248243/most-pythonic-way-to-declare-an-abstract-class-property
 [2]: https://github.com/reinhrst/abstractcp/issues/
 [3]: https://www.python.org/dev/peps/pep-0526/
-
-
```

### Comparing `abstractcp-0.9.9/README.md` & `abstractcp-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # AbstractCP -- Abstract Class Property
 
 ![Tox tests](https://github.com/reinhrst/abstractcp/workflows/Tox%20tests/badge.svg)
 
 
 This package allows one to create classes with abstract class properties.
 The initial code was inspired by [this question][1] (and accepted answer) -- in
-addition to me strugling many time with the same issue in the past.
-I firtst wanted to just post this as separate answer, however since it includes quite
+addition to me struggling many time with the same issue in the past.
+I first wanted to just post this as separate answer, however since it includes quite
 some python magic, and I would like to include quite some tests (and possibly update
 the code in the future), I made it into a package (even though I'm not a big fan of
 small packages that hardly do anything).
 
-The package is python3.6 and higher. I could consider creating a version for pre-3.6;
-if you want that, please create an [issue on github][2].
+The package is python3.8 and higher (version 0.9.9 runs on 3.6-3.11).
 
 ## TL;DR Examples
 Note: the examples use [PEP-526 type hints][3]; this is obviously optional.
 
 All examples assume the following imports:
 ```python
 import tying as t
```

### Comparing `abstractcp-0.9.9/abstractcp/__init__.py` & `abstractcp-1.0.0/abstractcp/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-import inspect
 import typing as t
 import warnings
-from pkg_resources import get_distribution, DistributionNotFound
+from importlib.metadata import version
 
 __project__ = __name__
 try:
-    __version__ = get_distribution(__project__).version
-except DistributionNotFound:
-    VERSION = __project__ + '-' + '(local)'
+    __version__ = version(__project__)
+except ImportError:
+    __version__ = __project__ + '-' + '(local)'
 
 T = t.TypeVar('T')
 
+
 class AbstractClassWithoutAbstractPropertiesWarning(Warning):
     pass
 
+
 class _AbstractClassProperty(t.Generic[T]):
     """
     Defines a class property as abstract
     """
     __name__: str
     __containg_klass_name__: str
     __propertytype_name__: str
@@ -67,18 +68,19 @@
 
     # next we override some of the default methods on an object that could
     # possibly be used accidentally (and give a non-error result):
 
     # compare
     __eq__ = __ne__ = __lt__ = __le__ = __gt__ = __ge__ = raise_use_compare
 
-    # We only need to take care of __bool__ and __str__ since they give a result
-    # on object()
+    # We only need to take care of __bool__ and __str__ since they give a
+    # result on object()
     __bool__ = __str__ = raise_use
 
+
 def abstract_class_property(propertytype: t.Type[T]) -> T:
     """
     Define an abstract class property of the given type
     """
     # Note that t.cast doesn't actually do anything at runtime
     return t.cast(T, _AbstractClassProperty(propertytype))
 
@@ -99,29 +101,29 @@
     def __init_subclass__(cls, **kwargs):
         super().__init_subclass__(**kwargs)
         if Abstract in cls.__bases__:
             # Direct descendant. Make sure that at least one property is
             # actually abstract
             for name in dir(cls):
                 if name.startswith("__") and name.endswith("__"):
-                    # internal names are ignored since they may have magic attached
-                    # when accessing
+                    # internal names are ignored since they may have magic
+                    # attached when accessing
                     continue
                 if isinstance(getattr(cls, name), _AbstractClassProperty):
                     break
             else:
                 warnings.warn(AbstractClassWithoutAbstractPropertiesWarning(
-                    f"Class {cls.__name__} is defined as abstract but does not "
-                    "have any abstract class properties defined."))
+                    f"Class {cls.__name__} is defined as abstract but does "
+                    "not have any abstract class properties defined."))
         else:
             # Any class that does not have Abstract as direct parent, is
             # assumed to be non-abstract, and therefore should have all
             # properties defined
             for name in dir(cls):
                 if name.startswith("__") and name.endswith("__"):
-                    # internal names are ignored since they may have magic attached
-                    # when accessing
+                    # internal names are ignored since they may have magic
+                    # attached when accessing
                     continue
                 if isinstance(getattr(cls, name), _AbstractClassProperty):
                     raise TypeError(
                         f"Class {cls.__name__} must define abstract class "
                         f"property {name}, or have Abstract as direct parent.")
```

### Comparing `abstractcp-0.9.9/abstractcp.egg-info/PKG-INFO` & `abstractcp-1.0.0/abstractcp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 Metadata-Version: 2.1
 Name: abstractcp
-Version: 0.9.9
+Version: 1.0.0
 Summary: Create abstract class variables
 Home-page: https://github.com/reinhrst/abstractcp
 Author: Claude El
 Author-email: abstractcp@claude.nl
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # AbstractCP -- Abstract Class Property
 
 ![Tox tests](https://github.com/reinhrst/abstractcp/workflows/Tox%20tests/badge.svg)
 
 
 This package allows one to create classes with abstract class properties.
 The initial code was inspired by [this question][1] (and accepted answer) -- in
-addition to me strugling many time with the same issue in the past.
-I firtst wanted to just post this as separate answer, however since it includes quite
+addition to me struggling many time with the same issue in the past.
+I first wanted to just post this as separate answer, however since it includes quite
 some python magic, and I would like to include quite some tests (and possibly update
 the code in the future), I made it into a package (even though I'm not a big fan of
 small packages that hardly do anything).
 
-The package is python3.6 and higher. I could consider creating a version for pre-3.6;
-if you want that, please create an [issue on github][2].
+The package is python3.8 and higher (version 0.9.9 runs on 3.6-3.11).
 
 ## TL;DR Examples
 Note: the examples use [PEP-526 type hints][3]; this is obviously optional.
 
 All examples assume the following imports:
 ```python
 import tying as t
@@ -194,9 +191,7 @@
 
 If you do this, I would appreciate if you drop me a line, since it probably means you've found a novel use for the package that I'd be happy to learn about (and possibly document).
 
 
 [1]: https://stackoverflow.com/questions/45248243/most-pythonic-way-to-declare-an-abstract-class-property
 [2]: https://github.com/reinhrst/abstractcp/issues/
 [3]: https://www.python.org/dev/peps/pep-0526/
-
-
```

### Comparing `abstractcp-0.9.9/setup.py` & `abstractcp-1.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools  # type: ignore
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-VERSION = "0.9.9"
+VERSION = "1.0.0"
 
 setuptools.setup(
     name="abstractcp",
     version=VERSION,
     author="Claude El",
     author_email="abstractcp@claude.nl",
     description="Create abstract class variables",
@@ -17,9 +17,9 @@
     packages=setuptools.find_packages(),
     package_data={"abstractcp": ["py.typed"]},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.6',
+    python_requires='>=3.8',
 )
```

