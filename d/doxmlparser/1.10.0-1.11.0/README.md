# Comparing `tmp/doxmlparser-1.10.0-py3-none-any.whl.zip` & `tmp/doxmlparser-1.11.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 136499 bytes, number of entries: 8
--rw-r--r--  2.0 unx       45 b- defN 23-Dec-25 10:53 doxmlparser/__init__.py
--rw-r--r--  2.0 unx  1284355 b- defN 23-Dec-25 10:53 doxmlparser/compound.py
--rw-r--r--  2.0 unx    64628 b- defN 23-Dec-25 10:53 doxmlparser/index.py
--rw-r--r--  2.0 unx     1058 b- defN 23-Dec-25 10:53 doxmlparser-1.10.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1937 b- defN 23-Dec-25 10:53 doxmlparser-1.10.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Dec-25 10:53 doxmlparser-1.10.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Dec-25 10:53 doxmlparser-1.10.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      650 b- defN 23-Dec-25 10:53 doxmlparser-1.10.0.dist-info/RECORD
-8 files, 1352777 bytes uncompressed, 135369 bytes compressed:  90.0%
+Zip file size: 138033 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       45 b- defN 24-May-20 09:40 doxmlparser/__init__.py
+-rw-r--r--  2.0 unx  1324076 b- defN 24-May-20 09:40 doxmlparser/compound.py
+-rw-r--r--  2.0 unx    64628 b- defN 24-May-20 09:40 doxmlparser/index.py
+-rw-r--r--  2.0 unx     1058 b- defN 24-May-20 09:40 doxmlparser-1.11.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1937 b- defN 24-May-20 09:40 doxmlparser-1.11.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-20 09:40 doxmlparser-1.11.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 24-May-20 09:40 doxmlparser-1.11.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      650 b- defN 24-May-20 09:40 doxmlparser-1.11.0.dist-info/RECORD
+8 files, 1392498 bytes uncompressed, 136903 bytes compressed:  90.2%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: doxmlparser/compound.py
 Comment: 
 
 Filename: doxmlparser/index.py
 Comment: 
 
-Filename: doxmlparser-1.10.0.dist-info/LICENSE
+Filename: doxmlparser-1.11.0.dist-info/LICENSE
 Comment: 
 
-Filename: doxmlparser-1.10.0.dist-info/METADATA
+Filename: doxmlparser-1.11.0.dist-info/METADATA
 Comment: 
 
-Filename: doxmlparser-1.10.0.dist-info/WHEEL
+Filename: doxmlparser-1.11.0.dist-info/WHEEL
 Comment: 
 
-Filename: doxmlparser-1.10.0.dist-info/top_level.txt
+Filename: doxmlparser-1.11.0.dist-info/top_level.txt
 Comment: 
 
-Filename: doxmlparser-1.10.0.dist-info/RECORD
+Filename: doxmlparser-1.11.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## doxmlparser/compound.py

```diff
@@ -985,14 +985,19 @@
 
 
 class DoxBool(str, Enum):
     YES='yes'
     NO='no'
 
 
+class DoxCheck(str, Enum):
+    CHECKED='checked'
+    UNCHECKED='unchecked'
+
+
 class DoxCompoundKind(str, Enum):
     CLASS='class'
     STRUCT='struct'
     UNION='union'
     INTERFACE='interface'
     PROTOCOL='protocol'
     CATEGORY='category'
@@ -1119,14 +1124,15 @@
     JSON='json'
     FLOW='flow'
     BOARD='board'
     GIT='git'
     HCL='hcl'
     REGEX='regex'
     EBNF='ebnf'
+    FILES='files'
 
 
 class DoxProtectionKind(str, Enum):
     PUBLIC='public'
     PROTECTED='protected'
     PRIVATE='private'
     PACKAGE='package'
@@ -1193,14 +1199,15 @@
     WARNING='warning'
     PRE='pre'
     POST='post'
     COPYRIGHT='copyright'
     INVARIANT='invariant'
     REMARK='remark'
     ATTENTION='attention'
+    IMPORTANT='important'
     PAR='par'
     RCS='rcs'
 
 
 class DoxVerticalAlign(str, Enum):
     BOTTOM='bottom'
     TOP='top'
@@ -3958,15 +3965,15 @@
 # end class sectiondefType
 
 
 class memberdefType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
-    def __init__(self, kind=None, id=None, prot=None, static=None, extern=None, strong=None, const=None, explicit=None, inline=None, refqual=None, virt=None, volatile=None, mutable=None, noexcept=None, constexpr=None, readable=None, writable=None, initonly=None, settable=None, privatesettable=None, protectedsettable=None, gettable=None, privategettable=None, protectedgettable=None, final=None, sealed=None, new=None, add=None, remove=None, raise_=None, optional=None, required=None, accessor=None, attribute=None, property=None, readonly=None, bound=None, removable=None, constrained=None, transient=None, maybevoid=None, maybedefault=None, maybeambiguous=None, templateparamlist=None, type_=None, definition=None, argsstring=None, name=None, qualifiedname=None, read=None, write=None, bitfield=None, reimplements=None, reimplementedby=None, qualifier=None, param=None, enumvalue=None, requiresclause=None, initializer=None, exceptions=None, briefdescription=None, detaileddescription=None, inbodydescription=None, location=None, references=None, referencedby=None, gds_collector_=None, **kwargs_):
+    def __init__(self, kind=None, id=None, prot=None, static=None, extern=None, strong=None, const=None, explicit=None, inline=None, refqual=None, virt=None, volatile=None, mutable=None, noexcept=None, noexceptexpression=None, nodiscard=None, constexpr=None, consteval=None, constinit=None, readable=None, writable=None, initonly=None, settable=None, privatesettable=None, protectedsettable=None, gettable=None, privategettable=None, protectedgettable=None, final=None, sealed=None, new=None, add=None, remove=None, raise_=None, optional=None, required=None, accessor=None, attribute=None, property=None, readonly=None, bound=None, removable=None, constrained=None, transient=None, maybevoid=None, maybedefault=None, maybeambiguous=None, templateparamlist=None, type_=None, definition=None, argsstring=None, name=None, qualifiedname=None, read=None, write=None, bitfield=None, reimplements=None, reimplementedby=None, qualifier=None, param=None, enumvalue=None, requiresclause=None, initializer=None, exceptions=None, briefdescription=None, detaileddescription=None, inbodydescription=None, location=None, references=None, referencedby=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
         self.parent_object_ = kwargs_.get('parent_object_')
         self.ns_prefix_ = None
         self.kind = _cast(None, kind)
         self.kind_nsprefix_ = None
@@ -3992,16 +3999,24 @@
         self.virt_nsprefix_ = None
         self.volatile = _cast(None, volatile)
         self.volatile_nsprefix_ = None
         self.mutable = _cast(None, mutable)
         self.mutable_nsprefix_ = None
         self.noexcept = _cast(None, noexcept)
         self.noexcept_nsprefix_ = None
+        self.noexceptexpression = _cast(None, noexceptexpression)
+        self.noexceptexpression_nsprefix_ = None
+        self.nodiscard = _cast(None, nodiscard)
+        self.nodiscard_nsprefix_ = None
         self.constexpr = _cast(None, constexpr)
         self.constexpr_nsprefix_ = None
+        self.consteval = _cast(None, consteval)
+        self.consteval_nsprefix_ = None
+        self.constinit = _cast(None, constinit)
+        self.constinit_nsprefix_ = None
         self.readable = _cast(None, readable)
         self.readable_nsprefix_ = None
         self.writable = _cast(None, writable)
         self.writable_nsprefix_ = None
         self.initonly = _cast(None, initonly)
         self.initonly_nsprefix_ = None
         self.settable = _cast(None, settable)
@@ -4322,18 +4337,34 @@
         return self.mutable
     def set_mutable(self, mutable):
         self.mutable = mutable
     def get_noexcept(self):
         return self.noexcept
     def set_noexcept(self, noexcept):
         self.noexcept = noexcept
+    def get_noexceptexpression(self):
+        return self.noexceptexpression
+    def set_noexceptexpression(self, noexceptexpression):
+        self.noexceptexpression = noexceptexpression
+    def get_nodiscard(self):
+        return self.nodiscard
+    def set_nodiscard(self, nodiscard):
+        self.nodiscard = nodiscard
     def get_constexpr(self):
         return self.constexpr
     def set_constexpr(self, constexpr):
         self.constexpr = constexpr
+    def get_consteval(self):
+        return self.consteval
+    def set_consteval(self, consteval):
+        self.consteval = consteval
+    def get_constinit(self):
+        return self.constinit
+    def set_constinit(self, constinit):
+        self.constinit = constinit
     def get_readable(self):
         return self.readable
     def set_readable(self, readable):
         self.readable = readable
     def get_writable(self):
         return self.writable
     def set_writable(self, writable):
@@ -4611,17 +4642,29 @@
             outfile.write(' volatile=%s' % (self.gds_encode(self.gds_format_string(quote_attrib(self.volatile), input_name='volatile')), ))
         if self.mutable is not None and 'mutable' not in already_processed:
             already_processed.add('mutable')
             outfile.write(' mutable=%s' % (self.gds_encode(self.gds_format_string(quote_attrib(self.mutable), input_name='mutable')), ))
         if self.noexcept is not None and 'noexcept' not in already_processed:
             already_processed.add('noexcept')
             outfile.write(' noexcept=%s' % (self.gds_encode(self.gds_format_string(quote_attrib(self.noexcept), input_name='noexcept')), ))
+        if self.noexceptexpression is not None and 'noexceptexpression' not in already_processed:
+            already_processed.add('noexceptexpression')
+            outfile.write(' noexceptexpression=%s' % (self.gds_encode(self.gds_format_string(quote_attrib(self.noexceptexpression), input_name='noexceptexpression')), ))
+        if self.nodiscard is not None and 'nodiscard' not in already_processed:
+            already_processed.add('nodiscard')
+            outfile.write(' nodiscard=%s' % (self.gds_encode(self.gds_format_string(quote_attrib(self.nodiscard), input_name='nodiscard')), ))
         if self.constexpr is not None and 'constexpr' not in already_processed:
             already_processed.add('constexpr')
             outfile.write(' constexpr=%s' % (self.gds_encode(self.gds_format_string(quote_attrib(self.constexpr), input_name='constexpr')), ))
+        if self.consteval is not None and 'consteval' not in already_processed:
+            already_processed.add('consteval')
+            outfile.write(' consteval=%s' % (self.gds_encode(self.gds_format_string(quote_attrib(self.consteval), input_name='consteval')), ))
+        if self.constinit is not None and 'constinit' not in already_processed:
+            already_processed.add('constinit')
+            outfile.write(' constinit=%s' % (self.gds_encode(self.gds_format_string(quote_attrib(self.constinit), input_name='constinit')), ))
         if self.readable is not None and 'readable' not in already_processed:
             already_processed.add('readable')
             outfile.write(' readable=%s' % (self.gds_encode(self.gds_format_string(quote_attrib(self.readable), input_name='readable')), ))
         if self.writable is not None and 'writable' not in already_processed:
             already_processed.add('writable')
             outfile.write(' writable=%s' % (self.gds_encode(self.gds_format_string(quote_attrib(self.writable), input_name='writable')), ))
         if self.initonly is not None and 'initonly' not in already_processed:
@@ -4861,19 +4904,38 @@
             self.mutable = value
             self.validate_DoxBool(self.mutable)    # validate type DoxBool
         value = find_attr_value_('noexcept', node)
         if value is not None and 'noexcept' not in already_processed:
             already_processed.add('noexcept')
             self.noexcept = value
             self.validate_DoxBool(self.noexcept)    # validate type DoxBool
+        value = find_attr_value_('noexceptexpression', node)
+        if value is not None and 'noexceptexpression' not in already_processed:
+            already_processed.add('noexceptexpression')
+            self.noexceptexpression = value
+        value = find_attr_value_('nodiscard', node)
+        if value is not None and 'nodiscard' not in already_processed:
+            already_processed.add('nodiscard')
+            self.nodiscard = value
+            self.validate_DoxBool(self.nodiscard)    # validate type DoxBool
         value = find_attr_value_('constexpr', node)
         if value is not None and 'constexpr' not in already_processed:
             already_processed.add('constexpr')
             self.constexpr = value
             self.validate_DoxBool(self.constexpr)    # validate type DoxBool
+        value = find_attr_value_('consteval', node)
+        if value is not None and 'consteval' not in already_processed:
+            already_processed.add('consteval')
+            self.consteval = value
+            self.validate_DoxBool(self.consteval)    # validate type DoxBool
+        value = find_attr_value_('constinit', node)
+        if value is not None and 'constinit' not in already_processed:
+            already_processed.add('constinit')
+            self.constinit = value
+            self.validate_DoxBool(self.constinit)    # validate type DoxBool
         value = find_attr_value_('readable', node)
         if value is not None and 'readable' not in already_processed:
             already_processed.add('readable')
             self.readable = value
             self.validate_DoxBool(self.readable)    # validate type DoxBool
         value = find_attr_value_('writable', node)
         if value is not None and 'writable' not in already_processed:
@@ -8957,29 +9019,34 @@
 # end class docSect3Type
 
 
 class docSect4Type(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
-    def __init__(self, id=None, title=None, para=None, internal=None, valueOf_=None, mixedclass_=None, content_=None, gds_collector_=None, **kwargs_):
+    def __init__(self, id=None, title=None, para=None, sect5=None, internal=None, valueOf_=None, mixedclass_=None, content_=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
         self.parent_object_ = kwargs_.get('parent_object_')
         self.ns_prefix_ = None
         self.id = _cast(None, id)
         self.id_nsprefix_ = None
         self.title = title
         self.title_nsprefix_ = None
         if para is None:
             self.para = []
         else:
             self.para = para
         self.para_nsprefix_ = None
+        if sect5 is None:
+            self.sect5 = []
+        else:
+            self.sect5 = sect5
+        self.sect5_nsprefix_ = None
         if internal is None:
             self.internal = []
         else:
             self.internal = internal
         self.internal_nsprefix_ = None
         self.valueOf_ = valueOf_
         if mixedclass_ is None:
@@ -9016,14 +9083,24 @@
         self.para = para
     def add_para(self, value):
         self.para.append(value)
     def insert_para_at(self, index, value):
         self.para.insert(index, value)
     def replace_para_at(self, index, value):
         self.para[index] = value
+    def get_sect5(self):
+        return self.sect5
+    def set_sect5(self, sect5):
+        self.sect5 = sect5
+    def add_sect5(self, value):
+        self.sect5.append(value)
+    def insert_sect5_at(self, index, value):
+        self.sect5.insert(index, value)
+    def replace_sect5_at(self, index, value):
+        self.sect5[index] = value
     def get_internal(self):
         return self.internal
     def set_internal(self, internal):
         self.internal = internal
     def add_internal(self, value):
         self.internal.append(value)
     def insert_internal_at(self, index, value):
@@ -9036,14 +9113,15 @@
         self.id = id
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
     def hasContent_(self):
         if (
             self.title is not None or
             self.para or
+            self.sect5 or
             self.internal or
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_) or
             self.content_
         ):
             return True
         else:
             return False
@@ -9084,14 +9162,17 @@
             eol_ = ''
         if self.title is not None:
             namespaceprefix_ = self.title_nsprefix_ + ':' if (UseCapturedNS_ and self.title_nsprefix_) else ''
             self.title.export(outfile, level, namespaceprefix_, namespacedef_='', name_='title', pretty_print=pretty_print)
         for para_ in self.para:
             namespaceprefix_ = self.para_nsprefix_ + ':' if (UseCapturedNS_ and self.para_nsprefix_) else ''
             para_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='para', pretty_print=pretty_print)
+        for sect5_ in self.sect5:
+            namespaceprefix_ = self.sect5_nsprefix_ + ':' if (UseCapturedNS_ and self.sect5_nsprefix_) else ''
+            sect5_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='sect5', pretty_print=pretty_print)
         for internal_ in self.internal:
             namespaceprefix_ = self.internal_nsprefix_ + ':' if (UseCapturedNS_ and self.internal_nsprefix_) else ''
             internal_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='internal', pretty_print=pretty_print)
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
             self.gds_elementtree_node_ = node
@@ -9129,14 +9210,24 @@
             obj_ = self.mixedclass_(MixedContainer.CategoryComplex,
                 MixedContainer.TypeNone, 'para', obj_)
             self.content_.append(obj_)
             if hasattr(self, 'add_para'):
                 self.add_para(obj_.value)
             elif hasattr(self, 'set_para'):
                 self.set_para(obj_.value)
+        elif nodeName_ == 'sect5':
+            obj_ = docSect5Type.factory(parent_object_=self)
+            obj_.build(child_, gds_collector_=gds_collector_)
+            obj_ = self.mixedclass_(MixedContainer.CategoryComplex,
+                MixedContainer.TypeNone, 'sect5', obj_)
+            self.content_.append(obj_)
+            if hasattr(self, 'add_sect5'):
+                self.add_sect5(obj_.value)
+            elif hasattr(self, 'set_sect5'):
+                self.set_sect5(obj_.value)
         elif nodeName_ == 'internal':
             obj_ = docInternalS4Type.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             obj_ = self.mixedclass_(MixedContainer.CategoryComplex,
                 MixedContainer.TypeNone, 'internal', obj_)
             self.content_.append(obj_)
             if hasattr(self, 'add_internal'):
@@ -9146,14 +9237,429 @@
         if not fromsubclass_ and child_.tail is not None:
             obj_ = self.mixedclass_(MixedContainer.CategoryText,
                 MixedContainer.TypeNone, '', child_.tail)
             self.content_.append(obj_)
 # end class docSect4Type
 
 
+class docSect5Type(GeneratedsSuper):
+    __hash__ = GeneratedsSuper.__hash__
+    subclass = None
+    superclass = None
+    def __init__(self, id=None, title=None, para=None, sect6=None, internal=None, valueOf_=None, mixedclass_=None, content_=None, gds_collector_=None, **kwargs_):
+        self.gds_collector_ = gds_collector_
+        self.gds_elementtree_node_ = None
+        self.original_tagname_ = None
+        self.parent_object_ = kwargs_.get('parent_object_')
+        self.ns_prefix_ = None
+        self.id = _cast(None, id)
+        self.id_nsprefix_ = None
+        self.title = title
+        self.title_nsprefix_ = None
+        if para is None:
+            self.para = []
+        else:
+            self.para = para
+        self.para_nsprefix_ = None
+        if sect6 is None:
+            self.sect6 = []
+        else:
+            self.sect6 = sect6
+        self.sect6_nsprefix_ = None
+        if internal is None:
+            self.internal = []
+        else:
+            self.internal = internal
+        self.internal_nsprefix_ = None
+        self.valueOf_ = valueOf_
+        if mixedclass_ is None:
+            self.mixedclass_ = MixedContainer
+        else:
+            self.mixedclass_ = mixedclass_
+        if content_ is None:
+            self.content_ = []
+        else:
+            self.content_ = content_
+        self.valueOf_ = valueOf_
+    def factory(*args_, **kwargs_):
+        if CurrentSubclassModule_ is not None:
+            subclass = getSubclassFromModule_(
+                CurrentSubclassModule_, docSect5Type)
+            if subclass is not None:
+                return subclass(*args_, **kwargs_)
+        if docSect5Type.subclass:
+            return docSect5Type.subclass(*args_, **kwargs_)
+        else:
+            return docSect5Type(*args_, **kwargs_)
+    factory = staticmethod(factory)
+    def get_ns_prefix_(self):
+        return self.ns_prefix_
+    def set_ns_prefix_(self, ns_prefix):
+        self.ns_prefix_ = ns_prefix
+    def get_title(self):
+        return self.title
+    def set_title(self, title):
+        self.title = title
+    def get_para(self):
+        return self.para
+    def set_para(self, para):
+        self.para = para
+    def add_para(self, value):
+        self.para.append(value)
+    def insert_para_at(self, index, value):
+        self.para.insert(index, value)
+    def replace_para_at(self, index, value):
+        self.para[index] = value
+    def get_sect6(self):
+        return self.sect6
+    def set_sect6(self, sect6):
+        self.sect6 = sect6
+    def add_sect6(self, value):
+        self.sect6.append(value)
+    def insert_sect6_at(self, index, value):
+        self.sect6.insert(index, value)
+    def replace_sect6_at(self, index, value):
+        self.sect6[index] = value
+    def get_internal(self):
+        return self.internal
+    def set_internal(self, internal):
+        self.internal = internal
+    def add_internal(self, value):
+        self.internal.append(value)
+    def insert_internal_at(self, index, value):
+        self.internal.insert(index, value)
+    def replace_internal_at(self, index, value):
+        self.internal[index] = value
+    def get_id(self):
+        return self.id
+    def set_id(self, id):
+        self.id = id
+    def get_valueOf_(self): return self.valueOf_
+    def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
+    def hasContent_(self):
+        if (
+            self.title is not None or
+            self.para or
+            self.sect6 or
+            self.internal or
+            (1 if type(self.valueOf_) in [int,float] else self.valueOf_) or
+            self.content_
+        ):
+            return True
+        else:
+            return False
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='docSect5Type', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('docSect5Type')
+        if imported_ns_def_ is not None:
+            namespacedef_ = imported_ns_def_
+        if pretty_print:
+            eol_ = '\n'
+        else:
+            eol_ = ''
+        if self.original_tagname_ is not None and name_ == 'docSect5Type':
+            name_ = self.original_tagname_
+        if UseCapturedNS_ and self.ns_prefix_:
+            namespaceprefix_ = self.ns_prefix_ + ':'
+        showIndent(outfile, level, pretty_print)
+        outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
+        already_processed = set()
+        self.exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='docSect5Type')
+        if self.hasContent_():
+            outfile.write('>%s' % (eol_, ))
+            self.exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='docSect5Type', pretty_print=pretty_print)
+            showIndent(outfile, level, pretty_print)
+            outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
+        else:
+            outfile.write('/>%s' % (eol_, ))
+    def exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='docSect5Type'):
+        if self.id is not None and 'id' not in already_processed:
+            already_processed.add('id')
+            outfile.write(' id=%s' % (self.gds_encode(self.gds_format_string(quote_attrib(self.id), input_name='id')), ))
+    def exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='docSect5Type', fromsubclass_=False, pretty_print=True):
+        if not fromsubclass_:
+            for item_ in self.content_:
+                item_.export(outfile, level, item_.name, namespaceprefix_, pretty_print=pretty_print)
+        if pretty_print:
+            eol_ = '\n'
+        else:
+            eol_ = ''
+        if self.title is not None:
+            namespaceprefix_ = self.title_nsprefix_ + ':' if (UseCapturedNS_ and self.title_nsprefix_) else ''
+            self.title.export(outfile, level, namespaceprefix_, namespacedef_='', name_='title', pretty_print=pretty_print)
+        for para_ in self.para:
+            namespaceprefix_ = self.para_nsprefix_ + ':' if (UseCapturedNS_ and self.para_nsprefix_) else ''
+            para_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='para', pretty_print=pretty_print)
+        for sect6_ in self.sect6:
+            namespaceprefix_ = self.sect6_nsprefix_ + ':' if (UseCapturedNS_ and self.sect6_nsprefix_) else ''
+            sect6_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='sect6', pretty_print=pretty_print)
+        for internal_ in self.internal:
+            namespaceprefix_ = self.internal_nsprefix_ + ':' if (UseCapturedNS_ and self.internal_nsprefix_) else ''
+            internal_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='internal', pretty_print=pretty_print)
+    def build(self, node, gds_collector_=None):
+        self.gds_collector_ = gds_collector_
+        if SaveElementTreeNode:
+            self.gds_elementtree_node_ = node
+        already_processed = set()
+        self.ns_prefix_ = node.prefix
+        self.buildAttributes(node, node.attrib, already_processed)
+        self.valueOf_ = get_all_text_(node)
+        if node.text is not None:
+            obj_ = self.mixedclass_(MixedContainer.CategoryText,
+                MixedContainer.TypeNone, '', node.text)
+            self.content_.append(obj_)
+        for child in node:
+            nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
+            self.buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
+        return self
+    def buildAttributes(self, node, attrs, already_processed):
+        value = find_attr_value_('id', node)
+        if value is not None and 'id' not in already_processed:
+            already_processed.add('id')
+            self.id = value
+    def buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
+        if nodeName_ == 'title':
+            obj_ = docTitleType.factory(parent_object_=self)
+            obj_.build(child_, gds_collector_=gds_collector_)
+            obj_ = self.mixedclass_(MixedContainer.CategoryComplex,
+                MixedContainer.TypeNone, 'title', obj_)
+            self.content_.append(obj_)
+            if hasattr(self, 'add_title'):
+                self.add_title(obj_.value)
+            elif hasattr(self, 'set_title'):
+                self.set_title(obj_.value)
+        elif nodeName_ == 'para':
+            obj_ = docParaType.factory(parent_object_=self)
+            obj_.build(child_, gds_collector_=gds_collector_)
+            obj_ = self.mixedclass_(MixedContainer.CategoryComplex,
+                MixedContainer.TypeNone, 'para', obj_)
+            self.content_.append(obj_)
+            if hasattr(self, 'add_para'):
+                self.add_para(obj_.value)
+            elif hasattr(self, 'set_para'):
+                self.set_para(obj_.value)
+        elif nodeName_ == 'sect6':
+            obj_ = docSect6Type.factory(parent_object_=self)
+            obj_.build(child_, gds_collector_=gds_collector_)
+            obj_ = self.mixedclass_(MixedContainer.CategoryComplex,
+                MixedContainer.TypeNone, 'sect6', obj_)
+            self.content_.append(obj_)
+            if hasattr(self, 'add_sect6'):
+                self.add_sect6(obj_.value)
+            elif hasattr(self, 'set_sect6'):
+                self.set_sect6(obj_.value)
+        elif nodeName_ == 'internal':
+            obj_ = docInternalS5Type.factory(parent_object_=self)
+            obj_.build(child_, gds_collector_=gds_collector_)
+            obj_ = self.mixedclass_(MixedContainer.CategoryComplex,
+                MixedContainer.TypeNone, 'internal', obj_)
+            self.content_.append(obj_)
+            if hasattr(self, 'add_internal'):
+                self.add_internal(obj_.value)
+            elif hasattr(self, 'set_internal'):
+                self.set_internal(obj_.value)
+        if not fromsubclass_ and child_.tail is not None:
+            obj_ = self.mixedclass_(MixedContainer.CategoryText,
+                MixedContainer.TypeNone, '', child_.tail)
+            self.content_.append(obj_)
+# end class docSect5Type
+
+
+class docSect6Type(GeneratedsSuper):
+    __hash__ = GeneratedsSuper.__hash__
+    subclass = None
+    superclass = None
+    def __init__(self, id=None, title=None, para=None, internal=None, valueOf_=None, mixedclass_=None, content_=None, gds_collector_=None, **kwargs_):
+        self.gds_collector_ = gds_collector_
+        self.gds_elementtree_node_ = None
+        self.original_tagname_ = None
+        self.parent_object_ = kwargs_.get('parent_object_')
+        self.ns_prefix_ = None
+        self.id = _cast(None, id)
+        self.id_nsprefix_ = None
+        self.title = title
+        self.title_nsprefix_ = None
+        if para is None:
+            self.para = []
+        else:
+            self.para = para
+        self.para_nsprefix_ = None
+        if internal is None:
+            self.internal = []
+        else:
+            self.internal = internal
+        self.internal_nsprefix_ = None
+        self.valueOf_ = valueOf_
+        if mixedclass_ is None:
+            self.mixedclass_ = MixedContainer
+        else:
+            self.mixedclass_ = mixedclass_
+        if content_ is None:
+            self.content_ = []
+        else:
+            self.content_ = content_
+        self.valueOf_ = valueOf_
+    def factory(*args_, **kwargs_):
+        if CurrentSubclassModule_ is not None:
+            subclass = getSubclassFromModule_(
+                CurrentSubclassModule_, docSect6Type)
+            if subclass is not None:
+                return subclass(*args_, **kwargs_)
+        if docSect6Type.subclass:
+            return docSect6Type.subclass(*args_, **kwargs_)
+        else:
+            return docSect6Type(*args_, **kwargs_)
+    factory = staticmethod(factory)
+    def get_ns_prefix_(self):
+        return self.ns_prefix_
+    def set_ns_prefix_(self, ns_prefix):
+        self.ns_prefix_ = ns_prefix
+    def get_title(self):
+        return self.title
+    def set_title(self, title):
+        self.title = title
+    def get_para(self):
+        return self.para
+    def set_para(self, para):
+        self.para = para
+    def add_para(self, value):
+        self.para.append(value)
+    def insert_para_at(self, index, value):
+        self.para.insert(index, value)
+    def replace_para_at(self, index, value):
+        self.para[index] = value
+    def get_internal(self):
+        return self.internal
+    def set_internal(self, internal):
+        self.internal = internal
+    def add_internal(self, value):
+        self.internal.append(value)
+    def insert_internal_at(self, index, value):
+        self.internal.insert(index, value)
+    def replace_internal_at(self, index, value):
+        self.internal[index] = value
+    def get_id(self):
+        return self.id
+    def set_id(self, id):
+        self.id = id
+    def get_valueOf_(self): return self.valueOf_
+    def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
+    def hasContent_(self):
+        if (
+            self.title is not None or
+            self.para or
+            self.internal or
+            (1 if type(self.valueOf_) in [int,float] else self.valueOf_) or
+            self.content_
+        ):
+            return True
+        else:
+            return False
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='docSect6Type', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('docSect6Type')
+        if imported_ns_def_ is not None:
+            namespacedef_ = imported_ns_def_
+        if pretty_print:
+            eol_ = '\n'
+        else:
+            eol_ = ''
+        if self.original_tagname_ is not None and name_ == 'docSect6Type':
+            name_ = self.original_tagname_
+        if UseCapturedNS_ and self.ns_prefix_:
+            namespaceprefix_ = self.ns_prefix_ + ':'
+        showIndent(outfile, level, pretty_print)
+        outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
+        already_processed = set()
+        self.exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='docSect6Type')
+        if self.hasContent_():
+            outfile.write('>%s' % (eol_, ))
+            self.exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='docSect6Type', pretty_print=pretty_print)
+            showIndent(outfile, level, pretty_print)
+            outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
+        else:
+            outfile.write('/>%s' % (eol_, ))
+    def exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='docSect6Type'):
+        if self.id is not None and 'id' not in already_processed:
+            already_processed.add('id')
+            outfile.write(' id=%s' % (self.gds_encode(self.gds_format_string(quote_attrib(self.id), input_name='id')), ))
+    def exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='docSect6Type', fromsubclass_=False, pretty_print=True):
+        if not fromsubclass_:
+            for item_ in self.content_:
+                item_.export(outfile, level, item_.name, namespaceprefix_, pretty_print=pretty_print)
+        if pretty_print:
+            eol_ = '\n'
+        else:
+            eol_ = ''
+        if self.title is not None:
+            namespaceprefix_ = self.title_nsprefix_ + ':' if (UseCapturedNS_ and self.title_nsprefix_) else ''
+            self.title.export(outfile, level, namespaceprefix_, namespacedef_='', name_='title', pretty_print=pretty_print)
+        for para_ in self.para:
+            namespaceprefix_ = self.para_nsprefix_ + ':' if (UseCapturedNS_ and self.para_nsprefix_) else ''
+            para_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='para', pretty_print=pretty_print)
+        for internal_ in self.internal:
+            namespaceprefix_ = self.internal_nsprefix_ + ':' if (UseCapturedNS_ and self.internal_nsprefix_) else ''
+            internal_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='internal', pretty_print=pretty_print)
+    def build(self, node, gds_collector_=None):
+        self.gds_collector_ = gds_collector_
+        if SaveElementTreeNode:
+            self.gds_elementtree_node_ = node
+        already_processed = set()
+        self.ns_prefix_ = node.prefix
+        self.buildAttributes(node, node.attrib, already_processed)
+        self.valueOf_ = get_all_text_(node)
+        if node.text is not None:
+            obj_ = self.mixedclass_(MixedContainer.CategoryText,
+                MixedContainer.TypeNone, '', node.text)
+            self.content_.append(obj_)
+        for child in node:
+            nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
+            self.buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
+        return self
+    def buildAttributes(self, node, attrs, already_processed):
+        value = find_attr_value_('id', node)
+        if value is not None and 'id' not in already_processed:
+            already_processed.add('id')
+            self.id = value
+    def buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
+        if nodeName_ == 'title':
+            obj_ = docTitleType.factory(parent_object_=self)
+            obj_.build(child_, gds_collector_=gds_collector_)
+            obj_ = self.mixedclass_(MixedContainer.CategoryComplex,
+                MixedContainer.TypeNone, 'title', obj_)
+            self.content_.append(obj_)
+            if hasattr(self, 'add_title'):
+                self.add_title(obj_.value)
+            elif hasattr(self, 'set_title'):
+                self.set_title(obj_.value)
+        elif nodeName_ == 'para':
+            obj_ = docParaType.factory(parent_object_=self)
+            obj_.build(child_, gds_collector_=gds_collector_)
+            obj_ = self.mixedclass_(MixedContainer.CategoryComplex,
+                MixedContainer.TypeNone, 'para', obj_)
+            self.content_.append(obj_)
+            if hasattr(self, 'add_para'):
+                self.add_para(obj_.value)
+            elif hasattr(self, 'set_para'):
+                self.set_para(obj_.value)
+        elif nodeName_ == 'internal':
+            obj_ = docInternalS6Type.factory(parent_object_=self)
+            obj_.build(child_, gds_collector_=gds_collector_)
+            obj_ = self.mixedclass_(MixedContainer.CategoryComplex,
+                MixedContainer.TypeNone, 'internal', obj_)
+            self.content_.append(obj_)
+            if hasattr(self, 'add_internal'):
+                self.add_internal(obj_.value)
+            elif hasattr(self, 'set_internal'):
+                self.set_internal(obj_.value)
+        if not fromsubclass_ and child_.tail is not None:
+            obj_ = self.mixedclass_(MixedContainer.CategoryText,
+                MixedContainer.TypeNone, '', child_.tail)
+            self.content_.append(obj_)
+# end class docSect6Type
+
+
 class docInternalType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, para=None, sect1=None, valueOf_=None, mixedclass_=None, content_=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
@@ -9636,30 +10142,30 @@
 # end class docInternalS2Type
 
 
 class docInternalS3Type(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
-    def __init__(self, para=None, sect3=None, valueOf_=None, mixedclass_=None, content_=None, gds_collector_=None, **kwargs_):
+    def __init__(self, para=None, sect4=None, valueOf_=None, mixedclass_=None, content_=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
         self.parent_object_ = kwargs_.get('parent_object_')
         self.ns_prefix_ = None
         if para is None:
             self.para = []
         else:
             self.para = para
         self.para_nsprefix_ = None
-        if sect3 is None:
-            self.sect3 = []
+        if sect4 is None:
+            self.sect4 = []
         else:
-            self.sect3 = sect3
-        self.sect3_nsprefix_ = None
+            self.sect4 = sect4
+        self.sect4_nsprefix_ = None
         self.valueOf_ = valueOf_
         if mixedclass_ is None:
             self.mixedclass_ = MixedContainer
         else:
             self.mixedclass_ = mixedclass_
         if content_ is None:
             self.content_ = []
@@ -9687,30 +10193,30 @@
         self.para = para
     def add_para(self, value):
         self.para.append(value)
     def insert_para_at(self, index, value):
         self.para.insert(index, value)
     def replace_para_at(self, index, value):
         self.para[index] = value
-    def get_sect3(self):
-        return self.sect3
-    def set_sect3(self, sect3):
-        self.sect3 = sect3
-    def add_sect3(self, value):
-        self.sect3.append(value)
-    def insert_sect3_at(self, index, value):
-        self.sect3.insert(index, value)
-    def replace_sect3_at(self, index, value):
-        self.sect3[index] = value
+    def get_sect4(self):
+        return self.sect4
+    def set_sect4(self, sect4):
+        self.sect4 = sect4
+    def add_sect4(self, value):
+        self.sect4.append(value)
+    def insert_sect4_at(self, index, value):
+        self.sect4.insert(index, value)
+    def replace_sect4_at(self, index, value):
+        self.sect4[index] = value
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
     def hasContent_(self):
         if (
             self.para or
-            self.sect3 or
+            self.sect4 or
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_) or
             self.content_
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='docInternalS3Type', pretty_print=True):
@@ -9745,17 +10251,17 @@
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for para_ in self.para:
             namespaceprefix_ = self.para_nsprefix_ + ':' if (UseCapturedNS_ and self.para_nsprefix_) else ''
             para_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='para', pretty_print=pretty_print)
-        for sect3_ in self.sect3:
-            namespaceprefix_ = self.sect3_nsprefix_ + ':' if (UseCapturedNS_ and self.sect3_nsprefix_) else ''
-            sect3_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='sect3', pretty_print=pretty_print)
+        for sect4_ in self.sect4:
+            namespaceprefix_ = self.sect4_nsprefix_ + ':' if (UseCapturedNS_ and self.sect4_nsprefix_) else ''
+            sect4_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='sect4', pretty_print=pretty_print)
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
             self.gds_elementtree_node_ = node
         already_processed = set()
         self.ns_prefix_ = node.prefix
         self.buildAttributes(node, node.attrib, already_processed)
@@ -9777,46 +10283,51 @@
             obj_ = self.mixedclass_(MixedContainer.CategoryComplex,
                 MixedContainer.TypeNone, 'para', obj_)
             self.content_.append(obj_)
             if hasattr(self, 'add_para'):
                 self.add_para(obj_.value)
             elif hasattr(self, 'set_para'):
                 self.set_para(obj_.value)
-        elif nodeName_ == 'sect3':
+        elif nodeName_ == 'sect4':
             obj_ = docSect4Type.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             obj_ = self.mixedclass_(MixedContainer.CategoryComplex,
-                MixedContainer.TypeNone, 'sect3', obj_)
+                MixedContainer.TypeNone, 'sect4', obj_)
             self.content_.append(obj_)
-            if hasattr(self, 'add_sect3'):
-                self.add_sect3(obj_.value)
-            elif hasattr(self, 'set_sect3'):
-                self.set_sect3(obj_.value)
+            if hasattr(self, 'add_sect4'):
+                self.add_sect4(obj_.value)
+            elif hasattr(self, 'set_sect4'):
+                self.set_sect4(obj_.value)
         if not fromsubclass_ and child_.tail is not None:
             obj_ = self.mixedclass_(MixedContainer.CategoryText,
                 MixedContainer.TypeNone, '', child_.tail)
             self.content_.append(obj_)
 # end class docInternalS3Type
 
 
 class docInternalS4Type(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
-    def __init__(self, para=None, valueOf_=None, mixedclass_=None, content_=None, gds_collector_=None, **kwargs_):
+    def __init__(self, para=None, sect5=None, valueOf_=None, mixedclass_=None, content_=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
         self.parent_object_ = kwargs_.get('parent_object_')
         self.ns_prefix_ = None
         if para is None:
             self.para = []
         else:
             self.para = para
         self.para_nsprefix_ = None
+        if sect5 is None:
+            self.sect5 = []
+        else:
+            self.sect5 = sect5
+        self.sect5_nsprefix_ = None
         self.valueOf_ = valueOf_
         if mixedclass_ is None:
             self.mixedclass_ = MixedContainer
         else:
             self.mixedclass_ = mixedclass_
         if content_ is None:
             self.content_ = []
@@ -9844,19 +10355,30 @@
         self.para = para
     def add_para(self, value):
         self.para.append(value)
     def insert_para_at(self, index, value):
         self.para.insert(index, value)
     def replace_para_at(self, index, value):
         self.para[index] = value
+    def get_sect5(self):
+        return self.sect5
+    def set_sect5(self, sect5):
+        self.sect5 = sect5
+    def add_sect5(self, value):
+        self.sect5.append(value)
+    def insert_sect5_at(self, index, value):
+        self.sect5.insert(index, value)
+    def replace_sect5_at(self, index, value):
+        self.sect5[index] = value
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
     def hasContent_(self):
         if (
             self.para or
+            self.sect5 or
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_) or
             self.content_
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='docInternalS4Type', pretty_print=True):
@@ -9891,14 +10413,17 @@
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for para_ in self.para:
             namespaceprefix_ = self.para_nsprefix_ + ':' if (UseCapturedNS_ and self.para_nsprefix_) else ''
             para_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='para', pretty_print=pretty_print)
+        for sect5_ in self.sect5:
+            namespaceprefix_ = self.sect5_nsprefix_ + ':' if (UseCapturedNS_ and self.sect5_nsprefix_) else ''
+            sect5_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='sect5', pretty_print=pretty_print)
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
             self.gds_elementtree_node_ = node
         already_processed = set()
         self.ns_prefix_ = node.prefix
         self.buildAttributes(node, node.attrib, already_processed)
@@ -9920,21 +10445,326 @@
             obj_ = self.mixedclass_(MixedContainer.CategoryComplex,
                 MixedContainer.TypeNone, 'para', obj_)
             self.content_.append(obj_)
             if hasattr(self, 'add_para'):
                 self.add_para(obj_.value)
             elif hasattr(self, 'set_para'):
                 self.set_para(obj_.value)
+        elif nodeName_ == 'sect5':
+            obj_ = docSect5Type.factory(parent_object_=self)
+            obj_.build(child_, gds_collector_=gds_collector_)
+            obj_ = self.mixedclass_(MixedContainer.CategoryComplex,
+                MixedContainer.TypeNone, 'sect5', obj_)
+            self.content_.append(obj_)
+            if hasattr(self, 'add_sect5'):
+                self.add_sect5(obj_.value)
+            elif hasattr(self, 'set_sect5'):
+                self.set_sect5(obj_.value)
         if not fromsubclass_ and child_.tail is not None:
             obj_ = self.mixedclass_(MixedContainer.CategoryText,
                 MixedContainer.TypeNone, '', child_.tail)
             self.content_.append(obj_)
 # end class docInternalS4Type
 
 
+class docInternalS5Type(GeneratedsSuper):
+    __hash__ = GeneratedsSuper.__hash__
+    subclass = None
+    superclass = None
+    def __init__(self, para=None, sect5=None, valueOf_=None, mixedclass_=None, content_=None, gds_collector_=None, **kwargs_):
+        self.gds_collector_ = gds_collector_
+        self.gds_elementtree_node_ = None
+        self.original_tagname_ = None
+        self.parent_object_ = kwargs_.get('parent_object_')
+        self.ns_prefix_ = None
+        if para is None:
+            self.para = []
+        else:
+            self.para = para
+        self.para_nsprefix_ = None
+        if sect5 is None:
+            self.sect5 = []
+        else:
+            self.sect5 = sect5
+        self.sect5_nsprefix_ = None
+        self.valueOf_ = valueOf_
+        if mixedclass_ is None:
+            self.mixedclass_ = MixedContainer
+        else:
+            self.mixedclass_ = mixedclass_
+        if content_ is None:
+            self.content_ = []
+        else:
+            self.content_ = content_
+        self.valueOf_ = valueOf_
+    def factory(*args_, **kwargs_):
+        if CurrentSubclassModule_ is not None:
+            subclass = getSubclassFromModule_(
+                CurrentSubclassModule_, docInternalS5Type)
+            if subclass is not None:
+                return subclass(*args_, **kwargs_)
+        if docInternalS5Type.subclass:
+            return docInternalS5Type.subclass(*args_, **kwargs_)
+        else:
+            return docInternalS5Type(*args_, **kwargs_)
+    factory = staticmethod(factory)
+    def get_ns_prefix_(self):
+        return self.ns_prefix_
+    def set_ns_prefix_(self, ns_prefix):
+        self.ns_prefix_ = ns_prefix
+    def get_para(self):
+        return self.para
+    def set_para(self, para):
+        self.para = para
+    def add_para(self, value):
+        self.para.append(value)
+    def insert_para_at(self, index, value):
+        self.para.insert(index, value)
+    def replace_para_at(self, index, value):
+        self.para[index] = value
+    def get_sect5(self):
+        return self.sect5
+    def set_sect5(self, sect5):
+        self.sect5 = sect5
+    def add_sect5(self, value):
+        self.sect5.append(value)
+    def insert_sect5_at(self, index, value):
+        self.sect5.insert(index, value)
+    def replace_sect5_at(self, index, value):
+        self.sect5[index] = value
+    def get_valueOf_(self): return self.valueOf_
+    def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
+    def hasContent_(self):
+        if (
+            self.para or
+            self.sect5 or
+            (1 if type(self.valueOf_) in [int,float] else self.valueOf_) or
+            self.content_
+        ):
+            return True
+        else:
+            return False
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='docInternalS5Type', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('docInternalS5Type')
+        if imported_ns_def_ is not None:
+            namespacedef_ = imported_ns_def_
+        if pretty_print:
+            eol_ = '\n'
+        else:
+            eol_ = ''
+        if self.original_tagname_ is not None and name_ == 'docInternalS5Type':
+            name_ = self.original_tagname_
+        if UseCapturedNS_ and self.ns_prefix_:
+            namespaceprefix_ = self.ns_prefix_ + ':'
+        showIndent(outfile, level, pretty_print)
+        outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
+        already_processed = set()
+        self.exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='docInternalS5Type')
+        if self.hasContent_():
+            outfile.write('>%s' % (eol_, ))
+            self.exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='docInternalS5Type', pretty_print=pretty_print)
+            showIndent(outfile, level, pretty_print)
+            outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
+        else:
+            outfile.write('/>%s' % (eol_, ))
+    def exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='docInternalS5Type'):
+        pass
+    def exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='docInternalS5Type', fromsubclass_=False, pretty_print=True):
+        if not fromsubclass_:
+            for item_ in self.content_:
+                item_.export(outfile, level, item_.name, namespaceprefix_, pretty_print=pretty_print)
+        if pretty_print:
+            eol_ = '\n'
+        else:
+            eol_ = ''
+        for para_ in self.para:
+            namespaceprefix_ = self.para_nsprefix_ + ':' if (UseCapturedNS_ and self.para_nsprefix_) else ''
+            para_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='para', pretty_print=pretty_print)
+        for sect5_ in self.sect5:
+            namespaceprefix_ = self.sect5_nsprefix_ + ':' if (UseCapturedNS_ and self.sect5_nsprefix_) else ''
+            sect5_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='sect5', pretty_print=pretty_print)
+    def build(self, node, gds_collector_=None):
+        self.gds_collector_ = gds_collector_
+        if SaveElementTreeNode:
+            self.gds_elementtree_node_ = node
+        already_processed = set()
+        self.ns_prefix_ = node.prefix
+        self.buildAttributes(node, node.attrib, already_processed)
+        self.valueOf_ = get_all_text_(node)
+        if node.text is not None:
+            obj_ = self.mixedclass_(MixedContainer.CategoryText,
+                MixedContainer.TypeNone, '', node.text)
+            self.content_.append(obj_)
+        for child in node:
+            nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
+            self.buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
+        return self
+    def buildAttributes(self, node, attrs, already_processed):
+        pass
+    def buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
+        if nodeName_ == 'para':
+            obj_ = docParaType.factory(parent_object_=self)
+            obj_.build(child_, gds_collector_=gds_collector_)
+            obj_ = self.mixedclass_(MixedContainer.CategoryComplex,
+                MixedContainer.TypeNone, 'para', obj_)
+            self.content_.append(obj_)
+            if hasattr(self, 'add_para'):
+                self.add_para(obj_.value)
+            elif hasattr(self, 'set_para'):
+                self.set_para(obj_.value)
+        elif nodeName_ == 'sect5':
+            obj_ = docSect6Type.factory(parent_object_=self)
+            obj_.build(child_, gds_collector_=gds_collector_)
+            obj_ = self.mixedclass_(MixedContainer.CategoryComplex,
+                MixedContainer.TypeNone, 'sect5', obj_)
+            self.content_.append(obj_)
+            if hasattr(self, 'add_sect5'):
+                self.add_sect5(obj_.value)
+            elif hasattr(self, 'set_sect5'):
+                self.set_sect5(obj_.value)
+        if not fromsubclass_ and child_.tail is not None:
+            obj_ = self.mixedclass_(MixedContainer.CategoryText,
+                MixedContainer.TypeNone, '', child_.tail)
+            self.content_.append(obj_)
+# end class docInternalS5Type
+
+
+class docInternalS6Type(GeneratedsSuper):
+    __hash__ = GeneratedsSuper.__hash__
+    subclass = None
+    superclass = None
+    def __init__(self, para=None, valueOf_=None, mixedclass_=None, content_=None, gds_collector_=None, **kwargs_):
+        self.gds_collector_ = gds_collector_
+        self.gds_elementtree_node_ = None
+        self.original_tagname_ = None
+        self.parent_object_ = kwargs_.get('parent_object_')
+        self.ns_prefix_ = None
+        if para is None:
+            self.para = []
+        else:
+            self.para = para
+        self.para_nsprefix_ = None
+        self.valueOf_ = valueOf_
+        if mixedclass_ is None:
+            self.mixedclass_ = MixedContainer
+        else:
+            self.mixedclass_ = mixedclass_
+        if content_ is None:
+            self.content_ = []
+        else:
+            self.content_ = content_
+        self.valueOf_ = valueOf_
+    def factory(*args_, **kwargs_):
+        if CurrentSubclassModule_ is not None:
+            subclass = getSubclassFromModule_(
+                CurrentSubclassModule_, docInternalS6Type)
+            if subclass is not None:
+                return subclass(*args_, **kwargs_)
+        if docInternalS6Type.subclass:
+            return docInternalS6Type.subclass(*args_, **kwargs_)
+        else:
+            return docInternalS6Type(*args_, **kwargs_)
+    factory = staticmethod(factory)
+    def get_ns_prefix_(self):
+        return self.ns_prefix_
+    def set_ns_prefix_(self, ns_prefix):
+        self.ns_prefix_ = ns_prefix
+    def get_para(self):
+        return self.para
+    def set_para(self, para):
+        self.para = para
+    def add_para(self, value):
+        self.para.append(value)
+    def insert_para_at(self, index, value):
+        self.para.insert(index, value)
+    def replace_para_at(self, index, value):
+        self.para[index] = value
+    def get_valueOf_(self): return self.valueOf_
+    def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
+    def hasContent_(self):
+        if (
+            self.para or
+            (1 if type(self.valueOf_) in [int,float] else self.valueOf_) or
+            self.content_
+        ):
+            return True
+        else:
+            return False
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='docInternalS6Type', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('docInternalS6Type')
+        if imported_ns_def_ is not None:
+            namespacedef_ = imported_ns_def_
+        if pretty_print:
+            eol_ = '\n'
+        else:
+            eol_ = ''
+        if self.original_tagname_ is not None and name_ == 'docInternalS6Type':
+            name_ = self.original_tagname_
+        if UseCapturedNS_ and self.ns_prefix_:
+            namespaceprefix_ = self.ns_prefix_ + ':'
+        showIndent(outfile, level, pretty_print)
+        outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
+        already_processed = set()
+        self.exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='docInternalS6Type')
+        if self.hasContent_():
+            outfile.write('>%s' % (eol_, ))
+            self.exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='docInternalS6Type', pretty_print=pretty_print)
+            showIndent(outfile, level, pretty_print)
+            outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
+        else:
+            outfile.write('/>%s' % (eol_, ))
+    def exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='docInternalS6Type'):
+        pass
+    def exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='docInternalS6Type', fromsubclass_=False, pretty_print=True):
+        if not fromsubclass_:
+            for item_ in self.content_:
+                item_.export(outfile, level, item_.name, namespaceprefix_, pretty_print=pretty_print)
+        if pretty_print:
+            eol_ = '\n'
+        else:
+            eol_ = ''
+        for para_ in self.para:
+            namespaceprefix_ = self.para_nsprefix_ + ':' if (UseCapturedNS_ and self.para_nsprefix_) else ''
+            para_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='para', pretty_print=pretty_print)
+    def build(self, node, gds_collector_=None):
+        self.gds_collector_ = gds_collector_
+        if SaveElementTreeNode:
+            self.gds_elementtree_node_ = node
+        already_processed = set()
+        self.ns_prefix_ = node.prefix
+        self.buildAttributes(node, node.attrib, already_processed)
+        self.valueOf_ = get_all_text_(node)
+        if node.text is not None:
+            obj_ = self.mixedclass_(MixedContainer.CategoryText,
+                MixedContainer.TypeNone, '', node.text)
+            self.content_.append(obj_)
+        for child in node:
+            nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
+            self.buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
+        return self
+    def buildAttributes(self, node, attrs, already_processed):
+        pass
+    def buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
+        if nodeName_ == 'para':
+            obj_ = docParaType.factory(parent_object_=self)
+            obj_.build(child_, gds_collector_=gds_collector_)
+            obj_ = self.mixedclass_(MixedContainer.CategoryComplex,
+                MixedContainer.TypeNone, 'para', obj_)
+            self.content_.append(obj_)
+            if hasattr(self, 'add_para'):
+                self.add_para(obj_.value)
+            elif hasattr(self, 'set_para'):
+                self.set_para(obj_.value)
+        if not fromsubclass_ and child_.tail is not None:
+            obj_ = self.mixedclass_(MixedContainer.CategoryText,
+                MixedContainer.TypeNone, '', child_.tail)
+            self.content_.append(obj_)
+# end class docInternalS6Type
+
+
 class docTitleType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ulink=None, bold=None, s=None, strike=None, underline=None, emphasis=None, computeroutput=None, subscript=None, superscript=None, center=None, small=None, cite=None, del_=None, ins=None, htmlonly=None, manonly=None, xmlonly=None, rtfonly=None, latexonly=None, docbookonly=None, image=None, dot=None, msc=None, plantuml=None, anchor=None, formula=None, ref=None, emoji=None, linebreak=None, valueOf_=None, mixedclass_=None, content_=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
@@ -16552,20 +17382,22 @@
 # end class docListType
 
 
 class docListItemType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
-    def __init__(self, value=None, para=None, gds_collector_=None, **kwargs_):
+    def __init__(self, override=None, value=None, para=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
         self.parent_object_ = kwargs_.get('parent_object_')
         self.ns_prefix_ = None
+        self.override = _cast(None, override)
+        self.override_nsprefix_ = None
         self.value = _cast(int, value)
         self.value_nsprefix_ = None
         if para is None:
             self.para = []
         else:
             self.para = para
         self.para_nsprefix_ = None
@@ -16590,18 +17422,35 @@
         self.para = para
     def add_para(self, value):
         self.para.append(value)
     def insert_para_at(self, index, value):
         self.para.insert(index, value)
     def replace_para_at(self, index, value):
         self.para[index] = value
+    def get_override(self):
+        return self.override
+    def set_override(self, override):
+        self.override = override
     def get_value(self):
         return self.value
     def set_value(self, value):
         self.value = value
+    def validate_DoxCheck(self, value):
+        # Validate type DoxCheck, a restriction on xsd:string.
+        if value is not None and Validate_simpletypes_ and self.gds_collector_ is not None:
+            if not isinstance(value, str):
+                lineno = self.gds_get_node_lineno_()
+                self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (str)' % {"value": value, "lineno": lineno, })
+                return False
+            value = value
+            enumerations = ['checked', 'unchecked']
+            if value not in enumerations:
+                lineno = self.gds_get_node_lineno_()
+                self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on DoxCheck' % {"value" : encode_str_2_3(value), "lineno": lineno} )
+                result = False
     def hasContent_(self):
         if (
             self.para
         ):
             return True
         else:
             return False
@@ -16625,14 +17474,17 @@
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='docListItemType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='docListItemType'):
+        if self.override is not None and 'override' not in already_processed:
+            already_processed.add('override')
+            outfile.write(' override=%s' % (self.gds_encode(self.gds_format_string(quote_attrib(self.override), input_name='override')), ))
         if self.value is not None and 'value' not in already_processed:
             already_processed.add('value')
             outfile.write(' value="%s"' % self.gds_format_integer(self.value, input_name='value'))
     def exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='docListItemType', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
@@ -16648,14 +17500,19 @@
         self.ns_prefix_ = node.prefix
         self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
         return self
     def buildAttributes(self, node, attrs, already_processed):
+        value = find_attr_value_('override', node)
+        if value is not None and 'override' not in already_processed:
+            already_processed.add('override')
+            self.override = value
+            self.validate_DoxCheck(self.override)    # validate type DoxCheck
         value = find_attr_value_('value', node)
         if value is not None and 'value' not in already_processed:
             already_processed.add('value')
             self.value = self.gds_parse_integer(value, node, 'value')
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'para':
             obj_ = docParaType.factory(parent_object_=self)
@@ -16721,15 +17578,15 @@
         # Validate type DoxSimpleSectKind, a restriction on xsd:string.
         if value is not None and Validate_simpletypes_ and self.gds_collector_ is not None:
             if not isinstance(value, str):
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (str)' % {"value": value, "lineno": lineno, })
                 return False
             value = value
-            enumerations = ['see', 'return', 'author', 'authors', 'version', 'since', 'date', 'note', 'warning', 'pre', 'post', 'copyright', 'invariant', 'remark', 'attention', 'par', 'rcs']
+            enumerations = ['see', 'return', 'author', 'authors', 'version', 'since', 'date', 'note', 'warning', 'pre', 'post', 'copyright', 'invariant', 'remark', 'attention', 'important', 'par', 'rcs']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on DoxSimpleSectKind' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
     def hasContent_(self):
         if (
             self.title is not None or
@@ -23994,15 +24851,15 @@
         # Validate type DoxPlantumlEngine, a restriction on xsd:string.
         if value is not None and Validate_simpletypes_ and self.gds_collector_ is not None:
             if not isinstance(value, str):
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (str)' % {"value": value, "lineno": lineno, })
                 return False
             value = value
-            enumerations = ['uml', 'bpm', 'wire', 'dot', 'ditaa', 'salt', 'math', 'latex', 'gantt', 'mindmap', 'wbs', 'yaml', 'creole', 'json', 'flow', 'board', 'git', 'hcl', 'regex', 'ebnf']
+            enumerations = ['uml', 'bpm', 'wire', 'dot', 'ditaa', 'salt', 'math', 'latex', 'gantt', 'mindmap', 'wbs', 'yaml', 'creole', 'json', 'flow', 'board', 'git', 'hcl', 'regex', 'ebnf', 'files']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on DoxPlantumlEngine' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
     def hasContent_(self):
         if (
             self.ulink or
@@ -27557,14 +28414,16 @@
     "docImageFileType",
     "docImageType",
     "docIndexEntryType",
     "docInternalS1Type",
     "docInternalS2Type",
     "docInternalS3Type",
     "docInternalS4Type",
+    "docInternalS5Type",
+    "docInternalS6Type",
     "docInternalType",
     "docLanguageType",
     "docListItemType",
     "docListType",
     "docMarkupType",
     "docParBlockType",
     "docParaType",
@@ -27576,14 +28435,16 @@
     "docPlantumlType",
     "docRefTextType",
     "docRowType",
     "docSect1Type",
     "docSect2Type",
     "docSect3Type",
     "docSect4Type",
+    "docSect5Type",
+    "docSect6Type",
     "docSimpleSectType",
     "docSummaryType",
     "docTableType",
     "docTitleType",
     "docTocItemType",
     "docTocListType",
     "docURLLink",
```

## Comparing `doxmlparser-1.10.0.dist-info/LICENSE` & `doxmlparser-1.11.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `doxmlparser-1.10.0.dist-info/METADATA` & `doxmlparser-1.11.0.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doxmlparser
-Version: 1.10.0
+Version: 1.11.0
 Summary: Python API to access doxygen generated XML output
 Home-page: https://github.com/doxygen/doxygen/addon/doxmlparser
 Author: Dimitri van Heesch
 Author-email: doxygen@gmail.com
 License: Copyright 2021 Dimitri van Heesch
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
```

## Comparing `doxmlparser-1.10.0.dist-info/RECORD` & `doxmlparser-1.11.0.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 doxmlparser/__init__.py,sha256=Tmxid3UuSOLteXyF31IgsmGJo4PkK3z97NO_EHW5bRo,45
-doxmlparser/compound.py,sha256=9yxIWgN9by9F_eDVgR0pbvAGPFUqIR5uIBDbqXyAMNo,1284355
+doxmlparser/compound.py,sha256=kFAYY9KCPH3KtUWArNjJRAKN8hGcrh0hM1s26C0i-24,1324076
 doxmlparser/index.py,sha256=yCPbnnoaWXJO75rCFJgVtv25-JC_a6usinPLizoKhPE,64628
-doxmlparser-1.10.0.dist-info/LICENSE,sha256=8jql5JStfG01ijNLfGXYDn3UpuggBXIvwPgg0VQKlZk,1058
-doxmlparser-1.10.0.dist-info/METADATA,sha256=a3OnozRI6qHLtpG3rzIEFCgI2zVQNh26sQqCztssCsw,1937
-doxmlparser-1.10.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-doxmlparser-1.10.0.dist-info/top_level.txt,sha256=HIIf8e3It_45WLP3Kvwa3XHIDHf0WYbwuNXcpmvMBDc,12
-doxmlparser-1.10.0.dist-info/RECORD,,
+doxmlparser-1.11.0.dist-info/LICENSE,sha256=8jql5JStfG01ijNLfGXYDn3UpuggBXIvwPgg0VQKlZk,1058
+doxmlparser-1.11.0.dist-info/METADATA,sha256=jvDE1eIYXyYTNbQ9sakqkyozIZsZxEuz5xam5h_dGtE,1937
+doxmlparser-1.11.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+doxmlparser-1.11.0.dist-info/top_level.txt,sha256=HIIf8e3It_45WLP3Kvwa3XHIDHf0WYbwuNXcpmvMBDc,12
+doxmlparser-1.11.0.dist-info/RECORD,,
```

