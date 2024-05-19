# Comparing `tmp/hpp2plantuml-0.8.3-py2.py3-none-any.whl.zip` & `tmp/hpp2plantuml-0.8.4-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 17541 bytes, number of entries: 9
--rw-r--r--  2.0 unx     3822 b- defN 22-Mar-27 21:48 hpp2plantuml/__init__.py
--rw-r--r--  2.0 unx    51471 b- defN 22-Mar-27 21:48 hpp2plantuml/hpp2plantuml.py
--rw-r--r--  2.0 unx      736 b- defN 22-Mar-27 21:48 hpp2plantuml/templates/default.puml
--rw-r--r--  2.0 unx     1068 b- defN 22-Mar-27 21:50 hpp2plantuml-0.8.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     5178 b- defN 22-Mar-27 21:50 hpp2plantuml-0.8.3.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 22-Mar-27 21:50 hpp2plantuml-0.8.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       65 b- defN 22-Mar-27 21:50 hpp2plantuml-0.8.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       13 b- defN 22-Mar-27 21:50 hpp2plantuml-0.8.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      770 b- defN 22-Mar-27 21:50 hpp2plantuml-0.8.3.dist-info/RECORD
-9 files, 63233 bytes uncompressed, 16203 bytes compressed:  74.4%
+Zip file size: 17574 bytes, number of entries: 9
+-rw-r--r--  2.0 unx     3822 b- defN 24-May-19 21:48 hpp2plantuml/__init__.py
+-rw-r--r--  2.0 unx    51601 b- defN 24-May-19 21:48 hpp2plantuml/hpp2plantuml.py
+-rw-r--r--  2.0 unx      736 b- defN 24-May-19 21:48 hpp2plantuml/templates/default.puml
+-rw-r--r--  2.0 unx     1068 b- defN 24-May-19 21:49 hpp2plantuml-0.8.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5180 b- defN 24-May-19 21:49 hpp2plantuml-0.8.4.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-May-19 21:49 hpp2plantuml-0.8.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       64 b- defN 24-May-19 21:49 hpp2plantuml-0.8.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       13 b- defN 24-May-19 21:49 hpp2plantuml-0.8.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      770 b- defN 24-May-19 21:49 hpp2plantuml-0.8.4.dist-info/RECORD
+9 files, 63364 bytes uncompressed, 16236 bytes compressed:  74.4%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: hpp2plantuml/hpp2plantuml.py
 Comment: 
 
 Filename: hpp2plantuml/templates/default.puml
 Comment: 
 
-Filename: hpp2plantuml-0.8.3.dist-info/LICENSE
+Filename: hpp2plantuml-0.8.4.dist-info/LICENSE
 Comment: 
 
-Filename: hpp2plantuml-0.8.3.dist-info/METADATA
+Filename: hpp2plantuml-0.8.4.dist-info/METADATA
 Comment: 
 
-Filename: hpp2plantuml-0.8.3.dist-info/WHEEL
+Filename: hpp2plantuml-0.8.4.dist-info/WHEEL
 Comment: 
 
-Filename: hpp2plantuml-0.8.3.dist-info/entry_points.txt
+Filename: hpp2plantuml-0.8.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: hpp2plantuml-0.8.3.dist-info/top_level.txt
+Filename: hpp2plantuml-0.8.4.dist-info/top_level.txt
 Comment: 
 
-Filename: hpp2plantuml-0.8.3.dist-info/RECORD
+Filename: hpp2plantuml-0.8.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hpp2plantuml/__init__.py

```diff
@@ -102,18 +102,18 @@
 produce a string output instead of writing to a text file.  See the API
 documentation for more details.
 
 """
 
 __title__ = "hpp2plantuml"
 __description__ = "Convert C++ header files to PlantUML"
-__version__ = '0.8.3'
+__version__ = '0.8.4'
 __uri__ = "https://github.com/thibaultmarin/hpp2plantuml"
 __doc__ = __description__ + " <" + __uri__ + ">"
 __author__ = "Thibault Marin"
 __email__ = "thibault.marin@gmx.com"
 __license__ = "MIT"
-__copyright__ = "Copyright (c) 2021 Thibault Marin"
+__copyright__ = "Copyright (c) 2023 Thibault Marin"
 
 from .hpp2plantuml import CreatePlantUMLFile, Diagram
 
 __all__ = ['CreatePlantUMLFile', 'Diagram']
```

## hpp2plantuml/hpp2plantuml.py

```diff
@@ -397,20 +397,23 @@
         Parameters
         ----------
         class_variable : CppVariable
             Parsed class variable object
         member_scope : str
             Scope property to member variable
         """
-        assert(isinstance(class_variable,
-                          CppHeaderParser.CppHeaderParser.CppVariable))
+        assert isinstance(class_variable,
+                          CppHeaderParser.CppHeaderParser.CppVariable)
 
         super().__init__(class_variable, member_scope)
 
         self._type = _cleanup_type(class_variable['type'])
+        if class_variable.get('array', 0):
+            self._type += '[]'
+
 
     def get_type(self):
         """Variable type accessor
 
         Returns
         -------
         str
@@ -441,16 +444,16 @@
         ----------
         class_method : CppMethod
             Parsed class member method
         member_scope : str
             Scope of the member method
 
         """
-        assert(isinstance(class_method,
-                          CppHeaderParser.CppHeaderParser.CppMethod))
+        assert isinstance(class_method,
+                          CppHeaderParser.CppHeaderParser.CppMethod)
 
         super().__init__(class_method, member_scope)
 
         self._type = _cleanup_type(class_method['returns'])
         if class_method['returns_pointer']:
             self._type += '*'
         elif class_method['returns_reference']:
@@ -473,15 +476,15 @@
 
         Returns
         -------
         str
             The method name (prefixed with the ``abstract`` keyword when
             appropriate) and signature
         """
-        assert(not self._static or not self._abstract)
+        assert not self._static or not self._abstract
 
         method_str = ('{abstract} ' if self._abstract else '') + \
                      self._name + '(' + \
                      ', '.join(' '.join(it).strip()
                                for it in self._param_list) + ')'
 
         return method_str
@@ -637,15 +640,17 @@
             Namespace or None if the class is defined in the default namespace
 
         Returns
         -------
         str
             Class name with appropriate prefix for use with link rendering
         """
-        return get_namespace_link_name(class_namespace) + '.' + class_name
+        if class_namespace:
+            return get_namespace_link_name(class_namespace) + '.' + class_name
+        return class_name
 
     def render(self):
         """Render class relationship to string
 
         This method generically appends the parent name, a rendering of the
         link type (obtained from the :func:`_render_link_type` method) and the
         child object name.
@@ -1489,15 +1494,15 @@
                         required=False, default=False, action='store_true',
                         help='Extract dependency relationships from method ' +
                         'arguments')
     parser.add_argument('-t', '--template-file', dest='template_file',
                         required=False, default=None, metavar='JINJA-FILE',
                         help='path to jinja2 template file')
     parser.add_argument('--version', action='version',
-                        version='%(prog)s ' + '0.8.3')
+                        version='%(prog)s ' + '0.8.4')
     args = parser.parse_args()
     if len(args.input_files) > 0:
         CreatePlantUMLFile(args.input_files, args.output_file,
                            template_file=args.template_file,
                            flag_dep=args.flag_dep)
 
 # %% Standalone mode
```

## Comparing `hpp2plantuml-0.8.3.dist-info/LICENSE` & `hpp2plantuml-0.8.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `hpp2plantuml-0.8.3.dist-info/METADATA` & `hpp2plantuml-0.8.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: hpp2plantuml
-Version: 0.8.3
+Version: 0.8.4
 Summary: Convert C++ header files to PlantUML
 Home-page: https://github.com/thibaultmarin/hpp2plantuml
 Author: Thibault Marin
 Author-email: thibault.marin@gmx.com
 Maintainer: Thibault Marin
 Maintainer-email: thibault.marin@gmx.com
 License: MIT
 Keywords: class
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE
 Requires-Dist: argparse
 Requires-Dist: jinja2
 Requires-Dist: robotpy-cppheaderparser
 Requires-Dist: sphinx
 
 hpp2plantuml - Convert C++ header files to PlantUML
 ===================================================
@@ -173,9 +173,7 @@
     python setup.py test
 
 
 The full documentation is available via:
 
 - `This org-mode post <https://thibaultmarin.github.io/blog/posts/2016-11-30-hpp2plantuml_-_Convert_C++_header_files_to_PlantUML.html>`_
 - `Read the docs <http://hpp2plantuml.readthedocs.io/en/latest/>`_
-
-
```

