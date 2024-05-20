# Comparing `tmp/annotated_types-0.5.0.tar.gz` & `tmp/annotated_types-0.6.0.tar.gz`

## Comparing `annotated_types-0.5.0.tar` & `annotated_types-0.6.0.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 annotated_types-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 annotated_types-0.5.0/Makefile
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 annotated_types-0.5.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     9375 2020-02-02 00:00:00.000000 annotated_types-0.5.0/annotated_types/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 annotated_types-0.5.0/annotated_types/py.typed
--rw-r--r--   0        0        0     5680 2020-02-02 00:00:00.000000 annotated_types-0.5.0/annotated_types/test_cases.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 annotated_types-0.5.0/requirements/all.txt
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 annotated_types-0.5.0/requirements/linting.in
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 annotated_types-0.5.0/requirements/linting.txt
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 annotated_types-0.5.0/requirements/testing.in
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 annotated_types-0.5.0/requirements/testing.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 annotated_types-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 annotated_types-0.5.0/tests/test_grouped_metadata.py
--rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 annotated_types-0.5.0/tests/test_main.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 annotated_types-0.5.0/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 annotated_types-0.5.0/LICENSE
--rw-r--r--   0        0        0    10505 2020-02-02 00:00:00.000000 annotated_types-0.5.0/README.md
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 annotated_types-0.5.0/pyproject.toml
--rw-r--r--   0        0        0    11685 2020-02-02 00:00:00.000000 annotated_types-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 annotated_types-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 annotated_types-0.6.0/Makefile
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 annotated_types-0.6.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0    12151 2020-02-02 00:00:00.000000 annotated_types-0.6.0/annotated_types/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 annotated_types-0.6.0/annotated_types/py.typed
+-rw-r--r--   0        0        0     6327 2020-02-02 00:00:00.000000 annotated_types-0.6.0/annotated_types/test_cases.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 annotated_types-0.6.0/requirements/all.in
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 annotated_types-0.6.0/requirements/all.txt
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 annotated_types-0.6.0/requirements/linting.in
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 annotated_types-0.6.0/requirements/testing.in
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 annotated_types-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 annotated_types-0.6.0/tests/test_grouped_metadata.py
+-rw-r--r--   0        0        0     4595 2020-02-02 00:00:00.000000 annotated_types-0.6.0/tests/test_main.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 annotated_types-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 annotated_types-0.6.0/LICENSE
+-rw-r--r--   0        0        0    11698 2020-02-02 00:00:00.000000 annotated_types-0.6.0/README.md
+-rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 annotated_types-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    12879 2020-02-02 00:00:00.000000 annotated_types-0.6.0/PKG-INFO
```

### Comparing `annotated_types-0.5.0/.pre-commit-config.yaml` & `annotated_types-0.6.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `annotated_types-0.5.0/.github/workflows/ci.yml` & `annotated_types-0.6.0/.github/workflows/ci.yml`

 * *Files 10% similar despite different names*

```diff
@@ -11,30 +11,30 @@
 
 jobs:
   test:
     name: test py-${{ matrix.python-version }}
     strategy:
       fail-fast: false
       matrix:
-        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11-dev']
+        python-version: ['3.8', '3.9', '3.10', '3.11', '3.12-dev']
 
     runs-on: ubuntu-latest
 
     env:
       PYTHON: ${{ matrix.python-version }}
 
     steps:
     - uses: actions/checkout@v3
 
     - name: set up python
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
 
-    - run: pip install -r requirements/testing.txt
+    - run: pip install -r requirements/all.txt
 
     - run: pip install .
 
     - run: make test
 
     - run: coverage xml
 
@@ -49,15 +49,15 @@
     steps:
     - uses: actions/checkout@v3
 
     - uses: actions/setup-python@v4
       with:
         python-version: '3.10'
 
-    - run: pip install -r requirements/linting.txt
+    - run: pip install -r requirements/all.txt
 
     - uses: pre-commit/action@v3.0.0
       with:
         extra_args: --all-files --verbose
 
   deploy:
     needs:
```

### Comparing `annotated_types-0.5.0/annotated_types/__init__.py` & `annotated_types-0.6.0/annotated_types/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+import math
 import sys
 from dataclasses import dataclass
 from datetime import timezone
-from typing import TYPE_CHECKING, Any, Callable, Iterator, Optional, TypeVar, Union
+from typing import TYPE_CHECKING, Any, Callable, Iterator, Optional, SupportsFloat, SupportsIndex, TypeVar, Union
 
 if sys.version_info < (3, 8):
     from typing_extensions import Protocol, runtime_checkable
 else:
     from typing import Protocol, runtime_checkable
 
 if sys.version_info < (3, 9):
@@ -37,18 +38,26 @@
     'MaxLen',
     'Len',
     'Timezone',
     'Predicate',
     'LowerCase',
     'UpperCase',
     'IsDigits',
+    'IsFinite',
+    'IsNotFinite',
+    'IsNan',
+    'IsNotNan',
+    'IsInfinite',
+    'IsNotInfinite',
+    'doc',
+    'DocInfo',
     '__version__',
 )
 
-__version__ = '0.5.0'
+__version__ = '0.6.0'
 
 
 T = TypeVar('T')
 
 
 # arguments that start with __ are considered
 # positional only
@@ -307,13 +316,81 @@
     skip invalid constraints, or statically raise an error; or it might try calling it
     and then propogate or discard the resulting exception.
     """
 
     func: Callable[[Any], bool]
 
 
-StrType = TypeVar("StrType", bound=str)
+@dataclass
+class Not:
+    func: Callable[[Any], bool]
+
+    def __call__(self, __v: Any) -> bool:
+        return not self.func(__v)
+
+
+_StrType = TypeVar("_StrType", bound=str)
 
-LowerCase = Annotated[StrType, Predicate(str.islower)]
-UpperCase = Annotated[StrType, Predicate(str.isupper)]
-IsDigits = Annotated[StrType, Predicate(str.isdigit)]
-IsAscii = Annotated[StrType, Predicate(str.isascii)]
+LowerCase = Annotated[_StrType, Predicate(str.islower)]
+"""
+Return True if the string is a lowercase string, False otherwise.
+
+A string is lowercase if all cased characters in the string are lowercase and there is at least one cased character in the string.
+"""  # noqa: E501
+UpperCase = Annotated[_StrType, Predicate(str.isupper)]
+"""
+Return True if the string is an uppercase string, False otherwise.
+
+A string is uppercase if all cased characters in the string are uppercase and there is at least one cased character in the string.
+"""  # noqa: E501
+IsDigits = Annotated[_StrType, Predicate(str.isdigit)]
+"""
+Return True if the string is a digit string, False otherwise.
+
+A string is a digit string if all characters in the string are digits and there is at least one character in the string.
+"""  # noqa: E501
+IsAscii = Annotated[_StrType, Predicate(str.isascii)]
+"""
+Return True if all characters in the string are ASCII, False otherwise.
+
+ASCII characters have code points in the range U+0000-U+007F. Empty string is ASCII too.
+"""
+
+_NumericType = TypeVar('_NumericType', bound=Union[SupportsFloat, SupportsIndex])
+IsFinite = Annotated[_NumericType, Predicate(math.isfinite)]
+"""Return True if x is neither an infinity nor a NaN, and False otherwise."""
+IsNotFinite = Annotated[_NumericType, Predicate(Not(math.isfinite))]
+"""Return True if x is one of infinity or NaN, and False otherwise"""
+IsNan = Annotated[_NumericType, Predicate(math.isnan)]
+"""Return True if x is a NaN (not a number), and False otherwise."""
+IsNotNan = Annotated[_NumericType, Predicate(Not(math.isnan))]
+"""Return True if x is anything but NaN (not a number), and False otherwise."""
+IsInfinite = Annotated[_NumericType, Predicate(math.isinf)]
+"""Return True if x is a positive or negative infinity, and False otherwise."""
+IsNotInfinite = Annotated[_NumericType, Predicate(Not(math.isinf))]
+"""Return True if x is neither a positive or negative infinity, and False otherwise."""
+
+try:
+    from typing_extensions import DocInfo, doc  # type: ignore [attr-defined]
+except ImportError:
+
+    @dataclass(frozen=True, **SLOTS)
+    class DocInfo:  # type: ignore [no-redef]
+        """ "
+        The return value of doc(), mainly to be used by tools that want to extract the
+        Annotated documentation at runtime.
+        """
+
+        documentation: str
+        """The documentation string passed to doc()."""
+
+    def doc(
+        documentation: str,
+    ) -> DocInfo:
+        """
+        Add documentation to a type annotation inside of Annotated.
+
+        For example:
+
+        >>> def hi(name: Annotated[int, doc("The name of the user")]) -> None: ...
+        """
+        return DocInfo(documentation)
```

### Comparing `annotated_types-0.5.0/annotated_types/test_cases.py` & `annotated_types-0.6.0/annotated_types/test_cases.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import math
 import sys
 from datetime import date, datetime, timedelta, timezone
 from decimal import Decimal
 from typing import Any, Dict, Iterable, Iterator, List, NamedTuple, Set, Tuple
 
 if sys.version_info < (3, 9):
     from typing_extensions import Annotated
@@ -121,13 +122,26 @@
     yield Case(at.LowerCase[str], ['abc', 'foobar'], ['', 'A', 'Boom'])
     yield Case(at.UpperCase[str], ['ABC', 'DEFO'], ['', 'a', 'abc', 'AbC'])
     yield Case(at.IsDigits[str], ['123'], ['', 'ab', 'a1b2'])
     yield Case(at.IsAscii[str], ['123', 'foo bar'], ['£100', '😊', 'whatever 👀'])
 
     yield Case(Annotated[int, at.Predicate(lambda x: x % 2 == 0)], [0, 2, 4], [1, 3, 5])
 
+    yield Case(at.IsFinite[float], [1.23], [math.nan, math.inf, -math.inf])
+    yield Case(at.IsNotFinite[float], [math.nan, math.inf], [1.23])
+    yield Case(at.IsNan[float], [math.nan], [1.23, math.inf])
+    yield Case(at.IsNotNan[float], [1.23, math.inf], [math.nan])
+    yield Case(at.IsInfinite[float], [math.inf], [math.nan, 1.23])
+    yield Case(at.IsNotInfinite[float], [math.nan, 1.23], [math.inf])
+
+    # check stacked predicates
+    yield Case(at.IsInfinite[Annotated[float, at.Predicate(lambda x: x > 0)]], [math.inf], [-math.inf, 1.23, math.nan])
+
+    # doc
+    yield Case(Annotated[int, at.doc("A number")], [1, 2], [])
+
     # custom GroupedMetadata
     class MyCustomGroupedMetadata(at.GroupedMetadata):
         def __iter__(self) -> Iterator[at.Predicate]:
             yield at.Predicate(lambda x: float(x).is_integer())
 
     yield Case(Annotated[float, MyCustomGroupedMetadata()], [0, 2.0], [0.01, 1.5])
```

### Comparing `annotated_types-0.5.0/requirements/linting.txt` & `annotated_types-0.6.0/requirements/all.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,77 +1,79 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --output-file=requirements/linting.txt --resolver=backtracking requirements/linting.in
+#    pip-compile --output-file=requirements/all.txt requirements/all.in
 #
-black==22.8.0
-    # via -r requirements/linting.in
-cfgv==3.3.1
+black==23.7.0
+    # via -r requirements/./linting.in
+cfgv==3.4.0
     # via pre-commit
-click==8.1.3
+click==8.1.7
     # via black
-colorama==0.4.5
+colorama==0.4.6
     # via isort
-distlib==0.3.6
+coverage==7.3.0
+    # via -r requirements/./testing.in
+distlib==0.3.7
     # via virtualenv
-exceptiongroup==1.1.1
-    # via pytest
-filelock==3.8.0
+filelock==3.12.2
     # via virtualenv
-flake8==5.0.4
+flake8==6.1.0
     # via
-    #   -r requirements/linting.in
+    #   -r requirements/./linting.in
     #   flake8-pyproject
-flake8-pyproject==1.1.0.post0
-    # via -r requirements/linting.in
-identify==2.5.5
+flake8-pyproject==1.2.3
+    # via -r requirements/./linting.in
+identify==2.5.27
     # via pre-commit
 iniconfig==2.0.0
     # via pytest
-isort[colors]==5.10.1
-    # via -r requirements/linting.in
+isort[colors]==5.12.0
+    # via -r requirements/./linting.in
 mccabe==0.7.0
     # via flake8
-mypy==0.971
-    # via -r requirements/linting.in
-mypy-extensions==0.4.3
+mypy==1.5.1
+    # via -r requirements/./linting.in
+mypy-extensions==1.0.0
     # via
     #   black
     #   mypy
-nodeenv==1.7.0
+nodeenv==1.8.0
     # via pre-commit
 packaging==23.1
-    # via pytest
-pathspec==0.10.1
+    # via
+    #   black
+    #   pytest
+    #   pytest-sugar
+pathspec==0.11.2
     # via black
-platformdirs==2.5.2
+platformdirs==3.10.0
     # via
     #   black
     #   virtualenv
-pluggy==1.0.0
+pluggy==1.3.0
     # via pytest
-pre-commit==2.20.0
-    # via -r requirements/linting.in
-pycodestyle==2.9.1
+pre-commit==3.3.3
+    # via -r requirements/./linting.in
+pycodestyle==2.11.0
     # via flake8
-pyflakes==2.5.0
+pyflakes==3.1.0
     # via flake8
-pytest==7.3.1
-    # via -r requirements/linting.in
-pyyaml==6.0
-    # via pre-commit
-toml==0.10.2
-    # via pre-commit
-tomli==2.0.1
+pytest==7.4.0
     # via
-    #   black
-    #   flake8-pyproject
-    #   mypy
-    #   pytest
-typing-extensions==4.3.0
+    #   -r requirements/./linting.in
+    #   -r requirements/./testing.in
+    #   pytest-sugar
+pytest-sugar==0.9.7
+    # via -r requirements/./testing.in
+pyyaml==6.0.1
+    # via pre-commit
+termcolor==2.3.0
+    # via pytest-sugar
+typing-extensions==4.7.1
     # via mypy
-virtualenv==20.16.5
+virtualenv==20.24.3
     # via pre-commit
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `annotated_types-0.5.0/tests/test_grouped_metadata.py` & `annotated_types-0.6.0/tests/test_grouped_metadata.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     with pytest.raises(TypeError):
 
         class Foo1(GroupedMetadata):
             pass
 
     class Foo2(GroupedMetadata):
         def __iter__(self) -> Iterator[BaseMetadata]:
-            return super().__iter__()
+            raise NotImplementedError
 
     with pytest.raises(NotImplementedError):
         for _ in Foo2():
             pass
 
 
 def test_non_subclass_implementer() -> None:
```

### Comparing `annotated_types-0.5.0/tests/test_main.py` & `annotated_types-0.6.0/tests/test_main.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,14 +51,19 @@
 def check_max_len(constraint: Constraint, val: Any) -> bool:
     assert isinstance(constraint, annotated_types.MaxLen)
     return len(val) <= constraint.max_length
 
 
 def check_predicate(constraint: Constraint, val: Any) -> bool:
     assert isinstance(constraint, annotated_types.Predicate)
+    # this is a relatively pointless branch since Not is itself callable
+    # but it serves to demonstrate that Not can be introspected
+    # and the wrapped predicate can be extracted / matched
+    if isinstance(constraint.func, annotated_types.Not):
+        return not constraint.func.func(val)
     return constraint.func(val)
 
 
 def check_timezone(constraint: Constraint, val: Any) -> bool:
     assert isinstance(constraint, annotated_types.Timezone)
     assert isinstance(val, datetime)
     if isinstance(constraint.tz, str):
```

### Comparing `annotated_types-0.5.0/LICENSE` & `annotated_types-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `annotated_types-0.5.0/README.md` & `annotated_types-0.6.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -124,29 +124,50 @@
 ### Predicate
 
 `Predicate(func: Callable)` expresses that `func(value)` is truthy for valid values.
 Users should prefer the statically inspectable metadata above, but if you need
 the full power and flexibility of arbitrary runtime predicates... here it is.
 
 We provide a few predefined predicates for common string constraints:
-`IsLower = Predicate(str.islower)`, `IsUpper = Predicate(str.isupper)`, and
-`IsDigit = Predicate(str.isdigit)`.
+
+* `IsLower = Predicate(str.islower)`
+* `IsUpper = Predicate(str.isupper)`
+* `IsDigit = Predicate(str.isdigit)`
+* `IsFinite = Predicate(math.isfinite)`
+* `IsNotFinite = Predicate(Not(math.isfinite))`
+* `IsNan = Predicate(math.isnan)`
+* `IsNotNan = Predicate(Not(math.isnan))`
+* `IsInfinite = Predicate(math.isinf)`
+* `IsNotInfinite = Predicate(Not(math.isinf))`
+
 Some libraries might have special logic to handle known or understandable predicates,
 for example by checking for `str.isdigit` and using its presence to both call custom
 logic to enforce digit-only strings, and customise some generated external schema.
 Users are therefore encouraged to avoid indirection like `lambda s: s.lower()`, in
 favor of introspectable methods such as `str.lower` or `re.compile("pattern").search`.
 
+To enable basic negation of commonly used predicates like `math.isnan` without introducing introspection that makes it impossible for implementers to introspect the predicate we provide a `Not` wrapper that simply negates the predicate in an introspectable manner. Several of the predicates listed above are created in this manner.
+
 We do not specify what behaviour should be expected for predicates that raise
 an exception.  For example `Annotated[int, Predicate(str.isdigit)]` might silently
 skip invalid constraints, or statically raise an error; or it might try calling it
 and then propogate or discard the resulting
 `TypeError: descriptor 'isdigit' for 'str' objects doesn't apply to a 'int' object`
 exception.  We encourage libraries to document the behaviour they choose.
 
+### Doc
+
+`doc()` can be used to add documentation information in `Annotated`, for function and method parameters, variables, class attributes, return types, and any place where `Annotated` can be used.
+
+It expects a value that can be statically analyzed, as the main use case is for static analysis, editors, documentation generators, and similar tools.
+
+It returns a `DocInfo` class with a single attribute `documentation` containing the value passed to `doc()`.
+
+This is the early adopter's alternative form of the [`typing-doc` proposal](https://github.com/tiangolo/fastapi/blob/typing-doc/typing_doc.md).
+
 ### Integrating downstream types with `GroupedMetadata`
 
 Implementers may choose to provide a convenience wrapper that groups multiple pieces of metadata.
 This can help reduce verbosity and cognitive overhead for users.
 For example, an implementer like Pydantic might provide a `Field` or `Meta` type that accepts keyword arguments and transforms these into low-level metadata:
 
 ```python
@@ -173,15 +194,15 @@
 
 Libraries consuming annotated-types should also ignore any metadata they do not recongize that came from unpacking a `GroupedMetadata`, just like they ignore unrecognized metadata in `Annotated` itself.
 
 Our own `annotated_types.Interval` class is a `GroupedMetadata` which unpacks itself into `Gt`, `Lt`, etc., so this is not an abstract concern.  Similarly, `annotated_types.Len` is a `GroupedMetadata` which unpacks itself into `MinLen` (optionally) and `MaxLen`.
 
 ### Consuming metadata
 
-We intend to not be perspcriptive as to _how_ the metadata and constraints are used, but as an example of how one might parse constraints from types annotations see our [implementation in `test_main.py`](https://github.com/annotated-types/annotated-types/blob/f59cf6d1b5255a0fe359b93896759a180bec30ae/tests/test_main.py#L94-L103).
+We intend to not be prescriptive as to _how_ the metadata and constraints are used, but as an example of how one might parse constraints from types annotations see our [implementation in `test_main.py`](https://github.com/annotated-types/annotated-types/blob/f59cf6d1b5255a0fe359b93896759a180bec30ae/tests/test_main.py#L94-L103).
 
 It is up to the implementer to determine how this metadata is used.
 You could use the metadata for runtime type checking, for generating schemas or to generate example data, amongst other use cases.
 
 ## Design & History
 
 This package was designed at the PyCon 2022 sprints by the maintainers of Pydantic
```

### Comparing `annotated_types-0.5.0/pyproject.toml` & `annotated_types-0.6.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -15,24 +15,24 @@
     "Intended Audience :: Information Technology",
     "Operating System :: Unix",
     "Operating System :: POSIX :: Linux",
     "Environment :: Console",
     "Environment :: MacOS X",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
 ]
 
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dependencies = ["typing-extensions>=4.0.0; python_version<'3.9'"]
 dynamic = ["version"]
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
```

### Comparing `annotated_types-0.5.0/PKG-INFO` & `annotated_types-0.6.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: annotated-types
-Version: 0.5.0
+Version: 0.6.0
 Summary: Reusable constraint types to use with typing.Annotated
 Author-email: Samuel Colvin <s@muelcolvin.com>, Adrian Garcia Badaracco <1755071+adriangb@users.noreply.github.com>, Zac Hatfield-Dodds <zac@zhd.dev>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: typing-extensions>=4.0.0; python_version < '3.9'
 Description-Content-Type: text/markdown
 
 # annotated-types
 
 [![CI](https://github.com/annotated-types/annotated-types/workflows/CI/badge.svg?event=push)](https://github.com/annotated-types/annotated-types/actions?query=event%3Apush+branch%3Amain+workflow%3ACI)
 [![pypi](https://img.shields.io/pypi/v/annotated-types.svg)](https://pypi.python.org/pypi/annotated-types)
@@ -150,29 +150,50 @@
 ### Predicate
 
 `Predicate(func: Callable)` expresses that `func(value)` is truthy for valid values.
 Users should prefer the statically inspectable metadata above, but if you need
 the full power and flexibility of arbitrary runtime predicates... here it is.
 
 We provide a few predefined predicates for common string constraints:
-`IsLower = Predicate(str.islower)`, `IsUpper = Predicate(str.isupper)`, and
-`IsDigit = Predicate(str.isdigit)`.
+
+* `IsLower = Predicate(str.islower)`
+* `IsUpper = Predicate(str.isupper)`
+* `IsDigit = Predicate(str.isdigit)`
+* `IsFinite = Predicate(math.isfinite)`
+* `IsNotFinite = Predicate(Not(math.isfinite))`
+* `IsNan = Predicate(math.isnan)`
+* `IsNotNan = Predicate(Not(math.isnan))`
+* `IsInfinite = Predicate(math.isinf)`
+* `IsNotInfinite = Predicate(Not(math.isinf))`
+
 Some libraries might have special logic to handle known or understandable predicates,
 for example by checking for `str.isdigit` and using its presence to both call custom
 logic to enforce digit-only strings, and customise some generated external schema.
 Users are therefore encouraged to avoid indirection like `lambda s: s.lower()`, in
 favor of introspectable methods such as `str.lower` or `re.compile("pattern").search`.
 
+To enable basic negation of commonly used predicates like `math.isnan` without introducing introspection that makes it impossible for implementers to introspect the predicate we provide a `Not` wrapper that simply negates the predicate in an introspectable manner. Several of the predicates listed above are created in this manner.
+
 We do not specify what behaviour should be expected for predicates that raise
 an exception.  For example `Annotated[int, Predicate(str.isdigit)]` might silently
 skip invalid constraints, or statically raise an error; or it might try calling it
 and then propogate or discard the resulting
 `TypeError: descriptor 'isdigit' for 'str' objects doesn't apply to a 'int' object`
 exception.  We encourage libraries to document the behaviour they choose.
 
+### Doc
+
+`doc()` can be used to add documentation information in `Annotated`, for function and method parameters, variables, class attributes, return types, and any place where `Annotated` can be used.
+
+It expects a value that can be statically analyzed, as the main use case is for static analysis, editors, documentation generators, and similar tools.
+
+It returns a `DocInfo` class with a single attribute `documentation` containing the value passed to `doc()`.
+
+This is the early adopter's alternative form of the [`typing-doc` proposal](https://github.com/tiangolo/fastapi/blob/typing-doc/typing_doc.md).
+
 ### Integrating downstream types with `GroupedMetadata`
 
 Implementers may choose to provide a convenience wrapper that groups multiple pieces of metadata.
 This can help reduce verbosity and cognitive overhead for users.
 For example, an implementer like Pydantic might provide a `Field` or `Meta` type that accepts keyword arguments and transforms these into low-level metadata:
 
 ```python
@@ -199,15 +220,15 @@
 
 Libraries consuming annotated-types should also ignore any metadata they do not recongize that came from unpacking a `GroupedMetadata`, just like they ignore unrecognized metadata in `Annotated` itself.
 
 Our own `annotated_types.Interval` class is a `GroupedMetadata` which unpacks itself into `Gt`, `Lt`, etc., so this is not an abstract concern.  Similarly, `annotated_types.Len` is a `GroupedMetadata` which unpacks itself into `MinLen` (optionally) and `MaxLen`.
 
 ### Consuming metadata
 
-We intend to not be perspcriptive as to _how_ the metadata and constraints are used, but as an example of how one might parse constraints from types annotations see our [implementation in `test_main.py`](https://github.com/annotated-types/annotated-types/blob/f59cf6d1b5255a0fe359b93896759a180bec30ae/tests/test_main.py#L94-L103).
+We intend to not be prescriptive as to _how_ the metadata and constraints are used, but as an example of how one might parse constraints from types annotations see our [implementation in `test_main.py`](https://github.com/annotated-types/annotated-types/blob/f59cf6d1b5255a0fe359b93896759a180bec30ae/tests/test_main.py#L94-L103).
 
 It is up to the implementer to determine how this metadata is used.
 You could use the metadata for runtime type checking, for generating schemas or to generate example data, amongst other use cases.
 
 ## Design & History
 
 This package was designed at the PyCon 2022 sprints by the maintainers of Pydantic
```

