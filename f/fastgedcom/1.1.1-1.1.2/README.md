# Comparing `tmp/fastgedcom-1.1.1.tar.gz` & `tmp/fastgedcom-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastgedcom-1.1.1.tar", last modified: Wed Mar 20 21:15:38 2024, max compression
+gzip compressed data, was "fastgedcom-1.1.2.tar", last modified: Mon May 20 12:42:49 2024, max compression
```

## Comparing `fastgedcom-1.1.1.tar` & `fastgedcom-1.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-03-20 21:15:38.254381 fastgedcom-1.1.1/
--rw-rw-rw-   0        0        0     1090 2023-05-22 23:10:18.000000 fastgedcom-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     8381 2024-03-20 21:15:38.243667 fastgedcom-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     7039 2024-03-20 21:14:52.000000 fastgedcom-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-20 21:15:38.206399 fastgedcom-1.1.1/fastgedcom/
--rw-rw-rw-   0        0        0        0 2023-06-09 22:40:35.000000 fastgedcom-1.1.1/fastgedcom/__init__.py
--rw-rw-rw-   0        0        0    11653 2024-03-20 20:32:56.000000 fastgedcom-1.1.1/fastgedcom/base.py
--rw-rw-rw-   0        0        0    13176 2024-03-20 18:49:22.000000 fastgedcom-1.1.1/fastgedcom/family_link.py
--rw-rw-rw-   0        0        0    11041 2024-03-20 20:32:56.000000 fastgedcom-1.1.1/fastgedcom/helpers.py
--rw-rw-rw-   0        0        0     6966 2024-03-19 22:31:57.000000 fastgedcom-1.1.1/fastgedcom/parser.py
--rw-rw-rw-   0        0        0        0 2023-05-25 13:48:45.000000 fastgedcom-1.1.1/fastgedcom/py.typed
-drwxrwxrwx   0        0        0        0 2024-03-20 21:15:38.243667 fastgedcom-1.1.1/fastgedcom.egg-info/
--rw-rw-rw-   0        0        0     8381 2024-03-20 21:15:38.000000 fastgedcom-1.1.1/fastgedcom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2024-03-20 21:15:38.000000 fastgedcom-1.1.1/fastgedcom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-20 21:15:38.000000 fastgedcom-1.1.1/fastgedcom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       93 2024-03-20 21:15:38.000000 fastgedcom-1.1.1/fastgedcom.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-20 21:15:38.000000 fastgedcom-1.1.1/fastgedcom.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1346 2024-03-20 20:53:36.000000 fastgedcom-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-20 21:15:38.254381 fastgedcom-1.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-20 21:15:38.243667 fastgedcom-1.1.1/test/
--rw-rw-rw-   0        0        0     2660 2024-03-20 20:32:56.000000 fastgedcom-1.1.1/test/test_base.py
--rw-rw-rw-   0        0        0     8290 2024-03-08 20:56:59.000000 fastgedcom-1.1.1/test/test_date_helpers.py
--rw-rw-rw-   0        0        0     5463 2024-03-08 20:56:59.000000 fastgedcom-1.1.1/test/test_family_link.py
--rw-rw-rw-   0        0        0     2107 2024-03-20 20:32:56.000000 fastgedcom-1.1.1/test/test_helpers.py
--rw-rw-rw-   0        0        0     5177 2024-03-20 20:32:56.000000 fastgedcom-1.1.1/test/test_parser.py
+drwxrwxrwx   0        0        0        0 2024-05-20 12:42:49.235151 fastgedcom-1.1.2/
+-rw-rw-rw-   0        0        0     1090 2023-05-22 23:10:18.000000 fastgedcom-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     8817 2024-05-20 12:42:49.233640 fastgedcom-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7468 2024-05-20 12:40:59.000000 fastgedcom-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 12:42:49.194853 fastgedcom-1.1.2/fastgedcom/
+-rw-rw-rw-   0        0        0        0 2023-06-09 22:40:35.000000 fastgedcom-1.1.2/fastgedcom/__init__.py
+-rw-rw-rw-   0        0        0    12178 2024-05-20 12:40:59.000000 fastgedcom-1.1.2/fastgedcom/base.py
+-rw-rw-rw-   0        0        0    13530 2024-05-20 12:40:59.000000 fastgedcom-1.1.2/fastgedcom/family_link.py
+-rw-rw-rw-   0        0        0    11041 2024-03-20 21:26:00.000000 fastgedcom-1.1.2/fastgedcom/helpers.py
+-rw-rw-rw-   0        0        0     7380 2024-05-20 12:40:59.000000 fastgedcom-1.1.2/fastgedcom/parser.py
+-rw-rw-rw-   0        0        0        0 2023-05-25 13:48:45.000000 fastgedcom-1.1.2/fastgedcom/py.typed
+drwxrwxrwx   0        0        0        0 2024-05-20 12:42:49.231638 fastgedcom-1.1.2/fastgedcom.egg-info/
+-rw-rw-rw-   0        0        0     8817 2024-05-20 12:42:49.000000 fastgedcom-1.1.2/fastgedcom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2024-05-20 12:42:49.000000 fastgedcom-1.1.2/fastgedcom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 12:42:49.000000 fastgedcom-1.1.2/fastgedcom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       93 2024-05-20 12:42:49.000000 fastgedcom-1.1.2/fastgedcom.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-20 12:42:49.000000 fastgedcom-1.1.2/fastgedcom.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1353 2024-05-20 12:40:59.000000 fastgedcom-1.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-20 12:42:49.235151 fastgedcom-1.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 12:42:49.229637 fastgedcom-1.1.2/test/
+-rw-rw-rw-   0        0        0     5960 2024-05-20 12:40:59.000000 fastgedcom-1.1.2/test/test_base.py
+-rw-rw-rw-   0        0        0     8290 2024-03-08 20:56:59.000000 fastgedcom-1.1.2/test/test_date_helpers.py
+-rw-rw-rw-   0        0        0     5463 2024-05-19 22:24:40.000000 fastgedcom-1.1.2/test/test_family_link.py
+-rw-rw-rw-   0        0        0     2107 2024-03-20 21:26:00.000000 fastgedcom-1.1.2/test/test_helpers.py
+-rw-rw-rw-   0        0        0     7684 2024-05-20 12:40:59.000000 fastgedcom-1.1.2/test/test_parser.py
```

### Comparing `fastgedcom-1.1.1/LICENSE` & `fastgedcom-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastgedcom-1.1.1/PKG-INFO` & `fastgedcom-1.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: fastgedcom
-Version: 1.1.1
-Summary: A lightweight tool to parse, browse and edit gedcom files.
+Version: 1.1.2
+Summary: A lightweight tool to easily parse, browse and edit gedcom files.
 Author-email: Gatien Bouyer <gatien.bouyer.dev@gmail.com>
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/GatienBouyer/fastgedcom/issues
 Project-URL: Source, https://github.com/GatienBouyer/fastgedcom
 Project-URL: Documentation, https://fastgedcom.readthedocs.io/en/latest/
 Keywords: fastgedcom,gedcom,parser,genealogy
 Classifier: License :: OSI Approved :: MIT License
@@ -28,32 +28,35 @@
 Requires-Dist: sphinx-rtd-theme; extra == "dev"
 Requires-Dist: sphinx-autoapi; extra == "dev"
 Provides-Extra: ansel
 Requires-Dist: ansel>=1.0.0; extra == "ansel"
 
 # FastGedcom
 
-A lightweight tool to parse, browse and edit gedcom files.
+A lightweight tool to easily parse, browse and edit gedcom files.
 
 Install FastGedcom using pip from [its PyPI page](https://pypi.org/project/fastgedcom/):
 ```bash
 pip install fastgedcom
 ```
-To install the Ansel codecs use the following command. It enables the use of the Ansel text encoding often used for gedcom files.
+To install the Ansel codec use the following command. It enables the use of the Ansel text encoding often used for gedcom files.
 ```bash
 pip install fastgedcom[ansel]
 ```
 
-## Why choosing FastGedcom?
+## Highlights of FastGedcom
 
-- FastGedcom is fast.
-- FastGedcom has type annotations.
-- FastGedcom has less methods than the alternatives, which make it easier to work with.
-- FastGedcom has a linear syntax, if/else and try/except blocks are less needed.
-- FastGedcom is shorter to write with the use of operator overloading. (optional)
+- FastGedcom is **easy** to write.
+- FastGedcom has **type annotations**.
+- FastGedcom has a **[documentation](https://fastgedcom.readthedocs.io/en/latest/)**, **[code examples](https://github.com/GatienBouyer/fastgedcom/tree/main/examples)**.
+- FastGedcom has **[unit tests](https://github.com/GatienBouyer/fastgedcom/tree/main/test)**.
+- FastGedcom has **less methods** than the alternatives, which make it easy to learn.
+- FastGedcom is **concise** thanks to operator overloads. (**optional**)
+- FastGedcom has a **linear** syntax, if/else and try/except blocks are less needed.
+- Last but not least, FastGedcom is **fast**. Go to [benchmarks](https://github.com/GatienBouyer/benchmark-python-gedcom).
 
 Comparison:
 <table>
 	<tr>
 		<th>Gedcom file</th>
 		<th>FastGedcom</th>
 		<th>python-gedcom</th>
@@ -145,15 +148,15 @@
     f.write(gedcom_without_uids)
 ```
 
 ### Typehints for salvation!
 Autocompletion and type checking make development so much easier.
 
 - There are only 3 main classes: [Document](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.Document), [TrueLine](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.TrueLine), and [FakeLine](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.FakeLine).
-- There are type aliases for code clarity: [Record](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.Record), [XRef](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.XRef), [IndiRef](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.IndiRef), [FamRef](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.FamRef), and more.
+- There are type aliases for code clarity and code documentation: [Record](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.Record), [XRef](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.XRef), [IndiRef](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.IndiRef), [FamRef](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.FamRef), and more.
 
 ```python
 from fastgedcom.base import Record, FakeLine
 from fastgedcom.family_link import FamilyLink
 
 # For fast and easy family lookups
 families = FamilyLink(document)
```

### Comparing `fastgedcom-1.1.1/README.md` & `fastgedcom-1.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 # FastGedcom
 
-A lightweight tool to parse, browse and edit gedcom files.
+A lightweight tool to easily parse, browse and edit gedcom files.
 
 Install FastGedcom using pip from [its PyPI page](https://pypi.org/project/fastgedcom/):
 ```bash
 pip install fastgedcom
 ```
-To install the Ansel codecs use the following command. It enables the use of the Ansel text encoding often used for gedcom files.
+To install the Ansel codec use the following command. It enables the use of the Ansel text encoding often used for gedcom files.
 ```bash
 pip install fastgedcom[ansel]
 ```
 
-## Why choosing FastGedcom?
+## Highlights of FastGedcom
 
-- FastGedcom is fast.
-- FastGedcom has type annotations.
-- FastGedcom has less methods than the alternatives, which make it easier to work with.
-- FastGedcom has a linear syntax, if/else and try/except blocks are less needed.
-- FastGedcom is shorter to write with the use of operator overloading. (optional)
+- FastGedcom is **easy** to write.
+- FastGedcom has **type annotations**.
+- FastGedcom has a **[documentation](https://fastgedcom.readthedocs.io/en/latest/)**, **[code examples](https://github.com/GatienBouyer/fastgedcom/tree/main/examples)**.
+- FastGedcom has **[unit tests](https://github.com/GatienBouyer/fastgedcom/tree/main/test)**.
+- FastGedcom has **less methods** than the alternatives, which make it easy to learn.
+- FastGedcom is **concise** thanks to operator overloads. (**optional**)
+- FastGedcom has a **linear** syntax, if/else and try/except blocks are less needed.
+- Last but not least, FastGedcom is **fast**. Go to [benchmarks](https://github.com/GatienBouyer/benchmark-python-gedcom).
 
 Comparison:
 <table>
 	<tr>
 		<th>Gedcom file</th>
 		<th>FastGedcom</th>
 		<th>python-gedcom</th>
@@ -113,15 +116,15 @@
     f.write(gedcom_without_uids)
 ```
 
 ### Typehints for salvation!
 Autocompletion and type checking make development so much easier.
 
 - There are only 3 main classes: [Document](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.Document), [TrueLine](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.TrueLine), and [FakeLine](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.FakeLine).
-- There are type aliases for code clarity: [Record](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.Record), [XRef](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.XRef), [IndiRef](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.IndiRef), [FamRef](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.FamRef), and more.
+- There are type aliases for code clarity and code documentation: [Record](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.Record), [XRef](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.XRef), [IndiRef](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.IndiRef), [FamRef](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.FamRef), and more.
 
 ```python
 from fastgedcom.base import Record, FakeLine
 from fastgedcom.family_link import FamilyLink
 
 # For fast and easy family lookups
 families = FamilyLink(document)
```

### Comparing `fastgedcom-1.1.1/fastgedcom/base.py` & `fastgedcom-1.1.2/fastgedcom/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,46 +51,51 @@
     @abstractmethod
     def payload(self) -> str:
         """See the description of :py:class:`.TrueLine` class."""
 
     @property
     @abstractmethod
     def payload_with_cont(self) -> str:
-        """The content of this gedcom field, namely the payload combined
-        with all CONT and CONC sub-lines."""
+        """Return the multi-line payload into a single string.
+
+        Multi-line payloads are split into several :py:class:`Line` as written
+        in the original gedcom file. The corresponding sub-lines are with the
+        tags CONC and CONT. There are gathered into a single string by
+        concatenation of the different payload of each line. A newline is
+        added for the concatenation of sub-lines with the CONT tag."""
 
     @property
     @abstractmethod
     def sub_lines(self) -> list['TrueLine']:
         """See the description of :py:class:`.TrueLine` class."""
 
     @abstractmethod
     def get_sub_lines(self, tag: str) -> list['TrueLine']:
         """Return all sub-lines having the given :any:`tag`.
-        An empty list if no line matches."""
+        Return an empty list if no line matches."""
 
     def __rshift__(self, tag: str) -> list['TrueLine']:
         """Alias for :py:meth:`get_sub_lines` to shorten the syntax
         by using the >> operator."""
         return self.get_sub_lines(tag)
 
     @abstractmethod
     def get_sub_line(self, tag: str) -> 'TrueLine | FakeLine':
         """Return the first sub-line having the given :any:`tag`.
-        A :py:class:`.FakeLine` if no line matches."""
+        Return a :py:class:`.FakeLine` if no line matches."""
 
     def __gt__(self, tag: str) -> 'TrueLine | FakeLine':
         """Alias for :py:meth:`get_sub_line` to shorten the syntax
         by using the > operator."""
         return self.get_sub_line(tag)
 
     @abstractmethod
     def get_sub_line_payload(self, tag: str) -> str:
         """Return the payload of the first sub-line having the given
-        :any:`tag`. An empty string if no line matches."""
+        :any:`tag`. Return an empty string if no line matches."""
 
     def __ge__(self, tag: str) -> str:
         """Alias for :py:meth:`get_sub_line_payload` to shorten the syntax
         by using the >= operator."""
         return self.get_sub_line_payload(tag)
 
     def get_all_sub_lines(self) -> Iterator['TrueLine']:
@@ -161,37 +166,42 @@
         return isinstance(value, FakeLine)
 
 
 @dataclass(slots=True)
 class TrueLine(Line):
     """Represent a line of a gedcom document.
 
-    Contain the :py:attr:`sub-lines` of the gedcom structure.
+    Contain the :py:attr:`sub-lines` of the gedcom structure to form a recursive
+    representation of the gedcom file.
+
+    This class uses the simplified format, instead of the normalized
+    ``Level [Xref] Tag [LineVal]`` format.
 
-    This class uses the simplified ``Level Tag Payload`` format, instead of
-    the normalized ``Level [Xref] Tag [LineVal]`` format. In the simplified
-    format, the :py:attr:`tag` is either the normalized Tag or the optional
+    The format of a gedcom line: ``Level Tag Payload``.
+
+    In the simplified format, the :py:attr:`tag` is either the normalized Tag or the optional
     Xref. Hence, the :py:attr:`payload` is the LineVal - when the Xref is not
     present - or the normalized Tag plus the LineVal (generally an empty
     string) - when the Xref is present. The Payload can be an empty string. As
     for the :py:attr:`level`, it matches the definition of the gedcom standard.
     """
 
     level: int
     """The line level defined by the gedcom standard."""
 
     tag: str | XRef
-    """The cross-reference identified if it is a :py:const:`Record`,
-    or the tag - as defined in the gedcom standard - defining the structure
-    type."""
+    """The cross-reference identifier for level 0 line (also called record identifier),
+    or the tag defining the information and the structure of the data."""
 
     payload: str
     """The payload of the structure, also called content or value.
-    Warning: Multi-line payloads are split into several lines according to the
-    gedcom standard. Use the :py:attr:`payload_with_cont` property to get the
+
+    Warning: Multi-line payloads are split into several :py:class:`Line` as
+    written in the original gedcom file. The corresponding sub-lines are with
+    the tags CONC and CONT. Use the :py:attr:`payload_with_cont` property to get the
     complete multi-line payloads."""
 
     sub_lines: list['TrueLine'] = field(default_factory=list)
     """List of the sub-lines, i.e. the next-level lines that are part
     of this structure."""
 
     def __bool__(self) -> Literal[True]:
@@ -247,38 +257,38 @@
 """A level 0 line referenced by an XRef in the document."""
 
 
 class Document():
     """Store all the information of the gedcom document.
 
     All records (level 0 lines) are directly accessible via the
-    :py:attr:`records` dictionnary and the other lines level are
+    :py:attr:`records` dictionnary and the other lines are
     accessible via :py:attr:`.TrueLine.sub_lines`."""
 
     records: dict[XRef, Record]
     """Dictionnary of records, accessible via :py:meth:`get_records` or
     :py:meth:`__getitem__`. Access it directly to raise KeyError instead
     of getting a :py:class:`.FakeLine`. Usefull when you a pretty sure of
     the Record existing in the document."""
 
     def __init__(self) -> None:
         self.records = dict()
 
     def __iter__(self) -> Iterator[Record]:
-        """Iterate on the lines of level 0
-        (the records, the header, and the TRLR line)."""
+        """Iterate on the lines of level 0:
+        the records, the header, and the TRLR line."""
         return iter(self.records.values())
 
     def __contains__(self, identifier: XRef) -> bool:
         """Return True if the identifier refers to an existing record."""
         return identifier in self.records
 
     def get_records(self, record_type: str) -> Iterator[Record]:
-        """Return an iterator over records of that ``record_type``
-        (i.e. the :py:attr:`~.TrueLine.payload` of level 0 lines)."""
+        """Return an iterator over records of that ``record_type``.
+        The type is the payload of level 0 lines: INDI, FAM, etc.."""
         for record in self.records.values():
             if record.payload == record_type:
                 yield record
 
     __rshift__ = get_records
     """Alias for :py:meth:`get_records` to shorten the syntax
     by using the >> operator."""
```

### Comparing `fastgedcom-1.1.1/fastgedcom/family_link.py` & `fastgedcom-1.1.2/fastgedcom/family_link.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,44 @@
-"""Define the :py:class:`.FamilyLink` class used to bypass family records."""
+"""Define the :py:class:`.FamilyLink` class used to bypass family records
+and ease the access to relatives."""
 
 from collections import defaultdict
 
 from .base import (
     Document, FakeLine, FamRef, IndiRef, Record, TrueLine, fake_line
 )
 
 
 class FamilyLink():
     """Class with methods to easily get relatives of someone.
 
-    Methods ending in _ref (such as :py:meth:`.get_parent_family_ref`)
+    Methods ending in _ref (such as :py:meth:`.get_children_ref`)
     are called by their non-_ref counterparts (such as
-    :py:meth:`.get_parent_family`). Use the first set of methods when
+    :py:meth:`.get_children`). Use the first set of methods when
     you need performance. Use the second set of methods for convenience.
 
-    The class uses 2 dictionnaries to speed up the process.
-    The `parents` dictionnary is used to get the parents of someone
+    The class uses 2 dictionnaries to store family relations:
+
+    - The `parents` dictionnary is used to get the parents of someone
     (via the FAMC of the person).
-    The `unions` dictionnary is used to get the spouses or children
+    - The `unions` dictionnary is used to get the spouses or children
     (via the FAMS of the person).
-    Not all methods use those dictionnaries.
+    Not all methods use those dictionnaries,
+    for example the get_parent_family_ref doesn't.
     """
 
     def __init__(self, document: Document) -> None:
         self.document = document
-        self.parents: dict[IndiRef, tuple[Record | FakeLine, Record | FakeLine]]
-        self.unions: defaultdict[IndiRef, list[Record]]
+        self.parents: dict[IndiRef, tuple[Record | FakeLine, Record | FakeLine]] = dict()
+        self.unions: defaultdict[IndiRef, list[Record]] = defaultdict(list)
         self._build_dicts()
 
     def _build_dicts(self) -> None:
-        self.parents = dict()
-        self.unions = defaultdict(list)
+        self.parents.clear()
+        self.unions.clear()
         for fam_record in self.document.records.values():
             if fam_record.payload != "FAM":
                 continue
             children: list[IndiRef] = []
             father: FakeLine | TrueLine = fake_line
             mother: FakeLine | TrueLine = fake_line
             for line in fam_record.sub_lines:
@@ -221,18 +224,20 @@
         parents = [indi]
         last_parents = [indi]
         for _ in range(ascent):
             last_parents = parents
             parents = [p.tag for i in parents for p in self.get_parents(i) if p]
         children = parents
         for k in range(descent):
-            children = [c for i in children for c in self.get_children_ref(i)
-                        if c not in last_parents]
-            if k == 0 and ascent == 1:  # remove duplicates
-                children = list(set(children))
+            children = [c for i in children for c in self.get_children_ref(i)]
+            if k == 0:
+                # prevent going back toward indi
+                children = [c for c in children if c not in last_parents]
+                if ascent == 1:  # prevent duplication of siblings
+                    children = list(set(children))
         return children
 
     def traverse(self, indi: IndiRef,
                  ascent: int = 0, descent: int = 0
                  ) -> list[Record]:
         """
         Recursively traverse the parents of the person and then their children.
@@ -269,15 +274,17 @@
         `collateral_diff` is used for same-generation difference:
 
         * 1 sibling, 2 cousins, 3 grand-counsins, ...
 
         The combinaison can be read as:
 
         * (when generation_diff > 0) `collateral_diff` of `generation_diff`
+            * examples: siblings of parents, cousings of grandparents
         * (when generation_diff < 0) `generation_diff` of `collateral_diff`
+            * examples: children of cousins, grand-children of siblings
 
         The `collateral_diff` must be strictly positive.
         This function is a wrapper around :py:meth:`traverse`.
         """
         if generation_diff >= 0:
             pos_gen = generation_diff
             neg_gen = 0
```

### Comparing `fastgedcom-1.1.1/fastgedcom/helpers.py` & `fastgedcom-1.1.2/fastgedcom/helpers.py`

 * *Files identical despite different names*

### Comparing `fastgedcom-1.1.1/fastgedcom/parser.py` & `fastgedcom-1.1.2/fastgedcom/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,22 +15,14 @@
 except ImportError:
     IS_ANSEL_INSTALLED = False
 else:
     IS_ANSEL_INSTALLED = True
     ansel.register()
 
 
-class ParsingError(Exception):
-    """Error raise by :py:func:`.strict_parse`."""
-
-
-class NothingParsed(ParsingError):
-    """Raised by :py:func:`.strict_parse` when the resulting document is empty."""
-
-
 class ParsingWarning():
     """Base warning class."""
 
 
 @dataclass
 class LineParsingWarning(ParsingWarning):
     """Warn about a line with a single word.
@@ -45,20 +37,22 @@
     xref: XRef
 
 
 @dataclass
 class LevelInconsistencyWarning(ParsingWarning):
     """Warn about a line without correct parent line."""
     line_number: int
+    line_content: str
 
 
 @dataclass
 class LevelParsingWarning(ParsingWarning):
-    """Warn about an unparsable line level."""
+    """Warn about an unparsable line level. Failed to parse it to an integer."""
     line_number: int
+    line_content: str
 
 
 @dataclass
 class EmptyLineWarning(ParsingWarning):
     """Warn about an empty line."""
     line_number: int
 
@@ -68,28 +62,26 @@
     """Warn about the presents of a 1-character-long line.
     This happens when the object parsed is an iterable on characters,
     whereas an iterable on lines is expected."""
     line_number: int
 
 
 def parse(lines: Iterable[str]) -> tuple[Document, list[ParsingWarning]]:
-    """Parse the text input to create the
+    """Parse the text input to create a
     :py:class:`.Document` object.
 
-    List of possible :py:class:`.ParsingWarning`:
-
-    * :py:class:`.LineParsingWarning`
-    * :py:class:`.DuplicateXRefWarning`
-    * :py:class:`.LevelInconsistencyWarning`
-    * :py:class:`.LevelParsingWarning`
-    * :py:class:`.EmptyLineWarning`
-    * :py:class:`.CharacterInsteadOfLineWarning`
-
+    When a malformed line is encountered, a warning is created
+    and we pass continue with the next line.
     Only :py:class:`.CharacterInsteadOfLineWarning` stops the parsing. If
     other warnings occur, the parsing continues with the next line.
+    For :py:class:`.LevelInconsistencyWarning`, the line is still inserted in the
+    tree.
+
+    Return the :py:class:`.Document` and the list of :py:class:`.ParsingWarning`
+    encountered.
     """
     document = Document()
     warnings: list[ParsingWarning] = []
     line_number = 0
     parent_lines: list[TrueLine] = []
     for line in lines:
         line_number += 1
@@ -105,69 +97,71 @@
             else:
                 if len(line) == 1:
                     warnings.append(CharacterInsteadOfLineWarning(line_number))
                     break
                 warnings.append(LineParsingWarning(line_number, line))
                 continue
         except ValueError:
-            warnings.append(LevelParsingWarning(line_number))
+            warnings.append(LevelParsingWarning(line_number, line))
             continue
         if parsed_line.level == 0:
             parent_lines = [parsed_line]
             if parsed_line.tag in document.records:
                 warnings.append(DuplicateXRefWarning(parsed_line.tag))
             document.records[parsed_line.tag] = parsed_line
         else:
             while parent_lines and parsed_line.level <= parent_lines[-1].level:
                 parent_lines.pop(-1)
             if len(parent_lines) == 0:
-                warnings.append(LevelInconsistencyWarning(line_number))
+                warnings.append(LevelInconsistencyWarning(line_number, line))
             else:
+                if (parent_lines[-1].level + 1 != parsed_line.level):
+                    warnings.append(LevelInconsistencyWarning(line_number, line))
                 parent_lines[-1].sub_lines.append(parsed_line)
                 parent_lines.append(parsed_line)
     return (document, warnings)
 
 
 def guess_encoding(file: str | Path) -> str | None:
     """Return the guessed encoding of the ``file``. None if unknown.
 
     A gedcom should precise its encoding in the header under the tag CHAR.
 
     However, indication of that field are often misleading or incomplete.
     For example:
     - ANSEL refers to the gedcom version of the ansel charset.
-    - The use of a BOM mark is recommended, but not stated,
+    - The use of a BOM mark is recommended but not stated,
     and not automatically handled by Python.
     - UNICODE refers to UTF-16.
     """
     # check BOM mark to deduce UTF family encodings
     # see http://unicode.org/faq/utf_bom.html#bom4
     with open(file, "rb") as f:
         first_bytes = f.read(4)
     if first_bytes[:3] == b"\xef\xbb\xbf":
         # UTF-8
         # The presence of the BOM mark must be specified.
         # With "utf-8-sig, Python removes the BOM mark when reading the file.
         return "utf-8-sig"
-    if first_bytes[:2] == b"\xff\xfe":
-        # UTF-16, little-endian
-        # With "utf_16", Python removes the BOM mark when reading the file.
-        return "utf_16"
-    if first_bytes[:2] == b"\xfe\xff":
-        # UTF-16, big-endian
-        # With "utf_16", Python removes the BOM mark when reading the file.
-        return "utf_16"
     if first_bytes == b"\xff\xfe\x00\x00":
         # UTF-32, little-endian
         # With "utf_32", Python removes the BOM mark when reading the file.
         return "utf_32"
     if first_bytes == b"\x00\x00\xfe\xff":
         # UTF-32, big-endian
         # With "utf_32", Python removes the BOM mark when reading the file.
         return "utf_32"
+    if first_bytes[:2] == b"\xff\xfe":
+        # UTF-16, little-endian
+        # With "utf_16", Python removes the BOM mark when reading the file.
+        return "utf_16"
+    if first_bytes[:2] == b"\xfe\xff":
+        # UTF-16, big-endian
+        # With "utf_16", Python removes the BOM mark when reading the file.
+        return "utf_16"
     # Try non-utf encodings and loog at the 0 HEAD > 1 CHAR gedcom field
     encodings = (
         "utf-8",
         "ansel" if IS_ANSEL_INSTALLED else None,
         "iso8859-1",
     )
     for encoding in encodings:
@@ -182,21 +176,35 @@
                             return "gedcom"
                         return stated_encoding
         except UnicodeError:
             pass
     return None
 
 
+class ParsingError(Exception):
+    """Error raise by :py:func:`.strict_parse`."""
+
+
+class NothingParsedError(ParsingError):
+    """Raised by :py:func:`.strict_parse` when the resulting document is empty."""
+
+
+@dataclass
+class MalformedError(ParsingError):
+    """Raised by :py:func:`.strict_parse` when there is warnings."""
+    warnings: list[ParsingWarning]
+
+
 def strict_parse(file: str | Path) -> Document:
     """Open and parse the gedcom file.
     Return the :py:class:`.Document` representing the gedcom file.
 
-    Raise :py:exc:`.ParsingError` when an error occurs in the parsing process.
     Raise :py:exc:`.NothingParsed` when the input is empty or isn't gedcom.
+    Raise :py:exc:`.MalformedError` when an error occurs in the parsing process.
     """
     with open(file, "r", encoding=guess_encoding(file)) as f:
         document, warnings = parse(f)
     if warnings:
-        raise ParsingError(warnings)
+        raise MalformedError(warnings)
     if len(document.records) == 0:
-        raise NothingParsed()
+        raise NothingParsedError()
     return document
```

### Comparing `fastgedcom-1.1.1/fastgedcom.egg-info/PKG-INFO` & `fastgedcom-1.1.2/fastgedcom.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: fastgedcom
-Version: 1.1.1
-Summary: A lightweight tool to parse, browse and edit gedcom files.
+Version: 1.1.2
+Summary: A lightweight tool to easily parse, browse and edit gedcom files.
 Author-email: Gatien Bouyer <gatien.bouyer.dev@gmail.com>
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/GatienBouyer/fastgedcom/issues
 Project-URL: Source, https://github.com/GatienBouyer/fastgedcom
 Project-URL: Documentation, https://fastgedcom.readthedocs.io/en/latest/
 Keywords: fastgedcom,gedcom,parser,genealogy
 Classifier: License :: OSI Approved :: MIT License
@@ -28,32 +28,35 @@
 Requires-Dist: sphinx-rtd-theme; extra == "dev"
 Requires-Dist: sphinx-autoapi; extra == "dev"
 Provides-Extra: ansel
 Requires-Dist: ansel>=1.0.0; extra == "ansel"
 
 # FastGedcom
 
-A lightweight tool to parse, browse and edit gedcom files.
+A lightweight tool to easily parse, browse and edit gedcom files.
 
 Install FastGedcom using pip from [its PyPI page](https://pypi.org/project/fastgedcom/):
 ```bash
 pip install fastgedcom
 ```
-To install the Ansel codecs use the following command. It enables the use of the Ansel text encoding often used for gedcom files.
+To install the Ansel codec use the following command. It enables the use of the Ansel text encoding often used for gedcom files.
 ```bash
 pip install fastgedcom[ansel]
 ```
 
-## Why choosing FastGedcom?
+## Highlights of FastGedcom
 
-- FastGedcom is fast.
-- FastGedcom has type annotations.
-- FastGedcom has less methods than the alternatives, which make it easier to work with.
-- FastGedcom has a linear syntax, if/else and try/except blocks are less needed.
-- FastGedcom is shorter to write with the use of operator overloading. (optional)
+- FastGedcom is **easy** to write.
+- FastGedcom has **type annotations**.
+- FastGedcom has a **[documentation](https://fastgedcom.readthedocs.io/en/latest/)**, **[code examples](https://github.com/GatienBouyer/fastgedcom/tree/main/examples)**.
+- FastGedcom has **[unit tests](https://github.com/GatienBouyer/fastgedcom/tree/main/test)**.
+- FastGedcom has **less methods** than the alternatives, which make it easy to learn.
+- FastGedcom is **concise** thanks to operator overloads. (**optional**)
+- FastGedcom has a **linear** syntax, if/else and try/except blocks are less needed.
+- Last but not least, FastGedcom is **fast**. Go to [benchmarks](https://github.com/GatienBouyer/benchmark-python-gedcom).
 
 Comparison:
 <table>
 	<tr>
 		<th>Gedcom file</th>
 		<th>FastGedcom</th>
 		<th>python-gedcom</th>
@@ -145,15 +148,15 @@
     f.write(gedcom_without_uids)
 ```
 
 ### Typehints for salvation!
 Autocompletion and type checking make development so much easier.
 
 - There are only 3 main classes: [Document](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.Document), [TrueLine](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.TrueLine), and [FakeLine](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.FakeLine).
-- There are type aliases for code clarity: [Record](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.Record), [XRef](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.XRef), [IndiRef](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.IndiRef), [FamRef](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.FamRef), and more.
+- There are type aliases for code clarity and code documentation: [Record](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.Record), [XRef](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.XRef), [IndiRef](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.IndiRef), [FamRef](https://fastgedcom.readthedocs.io/en/latest/autoapi/fastgedcom/base/index.html#fastgedcom.base.FamRef), and more.
 
 ```python
 from fastgedcom.base import Record, FakeLine
 from fastgedcom.family_link import FamilyLink
 
 # For fast and easy family lookups
 families = FamilyLink(document)
```

### Comparing `fastgedcom-1.1.1/pyproject.toml` & `fastgedcom-1.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "fastgedcom"
-version = "1.1.1"
-description = "A lightweight tool to parse, browse and edit gedcom files."
+version = "1.1.2"
+description = "A lightweight tool to easily parse, browse and edit gedcom files."
 keywords = ["fastgedcom", "gedcom", "parser", "genealogy"]
 authors = [
 	{name="Gatien Bouyer", email="gatien.bouyer.dev@gmail.com"},
 ]
 readme = "README.md"
 license = {text = "MIT License"}
 requires-python = ">=3.10"
```

### Comparing `fastgedcom-1.1.1/test/test_base.py` & `fastgedcom-1.1.2/test/test_helpers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,46 @@
 import unittest
-from pathlib import Path
+import warnings
 
 from fastgedcom.base import TrueLine
-from fastgedcom.parser import parse, strict_parse
-
-gedcom_file = Path(__file__).parent / "test_data" / "relatives.ged"
-
-
-class TestBase(unittest.TestCase):
-    def test_syntactic_sugar(self) -> None:
-        doc = strict_parse(gedcom_file)
-        self.assertTrue(doc["@I1@"])
-        self.assertFalse(doc["@I99@"])
-        self.assertTrue("@I1@" in doc)
-        self.assertFalse("@I99@" in doc)
-        self.assertTrue(doc["@I1@"] > "NAME")
-        self.assertFalse((doc["@I1@"] > "NAME") > "_ALIA")
-        self.assertFalse((doc["@I1@"] > "DEAT") > "DATE")
-        self.assertEqual((doc["@I1@"] > "NAME") >= "GIVN", "root")
-        self.assertEqual((doc["@I1@"] > "DEAT") >= "DATE", "")
-        self.assertListEqual(list(doc >> ""), [doc["HEAD"], doc["TRLR"]])
-        self.assertListEqual(list(doc["@F3@"] >> "CHIL"), [
-            TrueLine(1, "CHIL", "@I7@"), TrueLine(1, "CHIL", "@I41@")
-        ])
-        self.assertListEqual(list(doc["@F99@"] >> "CHIL"), [])
-
-    def test_payload_with_cont(self) -> None:
-        note_text1 = "This is a text\non several\nlines"
-        note_line1 = TrueLine(1, "NOTE", "This is a text", [
-            TrueLine(2, "CONT", "on several"),
-            TrueLine(2, "CONT", "lines"),
-        ])
-        self.assertEqual(note_line1.payload_with_cont, note_text1)
-        note_text2 = "This is a very long text that is split"
-        note_line2 = TrueLine(1, "NOTE", "This is a very", [
-            TrueLine(2, "CONC", " long text th"),
-            TrueLine(2, "CONC", "at is split"),
-        ])
-        self.assertEqual(note_line2.payload_with_cont, note_text2)
-        note_text3 = "This text is on several lines:\nTo present a very long text that is split.\n\nAnd a second one:\nAlso a very long sentence that is split."
-        note_line3 = TrueLine(1, "NOTE", "This text is on several lines:", [
-            TrueLine(2, "CONT", "To present a very long"),
-            TrueLine(2, "CONC", " text that is split."),
-            TrueLine(2, "CONT", ""),
-            TrueLine(2, "CONT", "And a second one:"),
-            TrueLine(2, "CONT", "Also a very long sent"),
-            TrueLine(2, "CONC", "ence that is split."),
-        ])
-        self.assertEqual(note_line3.payload_with_cont, note_text3)
-
-    def test_document_to_gedcom(self) -> None:
-        source = "0 HEAD\n1 GEDC\n2 VERS 5.5\n1 CHAR UTF-8\n0 TRLR\n"
-        doc, _ = parse(source.splitlines())
-        output = doc.get_source()
-        self.assertEqual(source, output)
+from fastgedcom.helpers import (
+    extract_name_parts, format_name, get_all_sub_lines, get_source
+)
+from fastgedcom.parser import parse
+
+
+class TestHelpers(unittest.TestCase):
+    def test_format_name(self) -> None:
+        self.assertEqual(format_name("Gatien /BOUYER/"), "Gatien BOUYER")
+        self.assertEqual(format_name(" /BOUYER/"), " BOUYER")
+        self.assertEqual(format_name("Gatien "), "Gatien ")
+        self.assertEqual(format_name("Gatien //"), "Gatien ")
+
+    def test_extract_name_parts(self) -> None:
+        self.assertEqual(extract_name_parts("Gatien /BOUYER/"), ("Gatien", "BOUYER"))
+        self.assertEqual(extract_name_parts(" /BOUYER/"), ("", "BOUYER"))
+        self.assertEqual(extract_name_parts("Gatien "), ("Gatien", ""))
+        self.assertEqual(extract_name_parts("Gatien //"), ("Gatien", ""))
+        self.assertEqual(extract_name_parts("Gatien ... /BOUYER / ***"), ("Gatien ... ***", "BOUYER"))
+
+    def test_sub_rec_recursive(self) -> None:
+        with warnings.catch_warnings(record=True) as w:
+            surn = TrueLine(2, "SURN", "BOUYER", [])
+            givn = TrueLine(2, "GIVN", "Gatien", [])
+            name = TrueLine(1, "NAME", "Gatien /BOUYER/", [surn, givn])
+            sex = TrueLine(1, "SEX", "M", [])
+            indi = TrueLine(0, "@I1@", "INDI", [name, sex])
+            all_recs = list(get_all_sub_lines(indi))
+            self.assertListEqual(all_recs, [name, surn, givn, sex])
+            self.assertTrue(issubclass(w[0].category, DeprecationWarning))
+
+    def test_get_source(self) -> None:
+        with warnings.catch_warnings(record=True) as w:
+            header = "0 HEAD\n1 GEDC\n2 VERS 5.5\n2 FORM LINEAGE-LINKED\n1 CHAR UTF-8\n"
+            doc, _ = parse(header.splitlines())
+            self.assertEqual(get_source(doc["HEAD"]), header)
+            self.assertEqual(get_source(doc["@@"]), "")
+            self.assertTrue(issubclass(w[0].category, DeprecationWarning))
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fastgedcom-1.1.1/test/test_date_helpers.py` & `fastgedcom-1.1.2/test/test_date_helpers.py`

 * *Files identical despite different names*

### Comparing `fastgedcom-1.1.1/test/test_family_link.py` & `fastgedcom-1.1.2/test/test_family_link.py`

 * *Files identical despite different names*

