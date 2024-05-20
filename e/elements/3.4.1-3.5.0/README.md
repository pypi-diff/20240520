# Comparing `tmp/elements-3.4.1.tar.gz` & `tmp/elements-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elements-3.4.1.tar", last modified: Mon May 13 22:50:35 2024, max compression
+gzip compressed data, was "elements-3.5.0.tar", last modified: Mon May 20 19:05:33 2024, max compression
```

## Comparing `elements-3.4.1.tar` & `elements-3.5.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-13 22:50:35.586840 elements-3.4.1/
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1058 2023-12-10 19:43:58.000000 elements-3.4.1/LICENSE
--rw-r-----   0 danijar  (322066) primarygroup (89939)       59 2023-12-10 19:43:58.000000 elements-3.4.1/MANIFEST.in
--rw-r-----   0 danijar  (322066) primarygroup (89939)    10803 2024-05-13 22:50:35.586840 elements-3.4.1/PKG-INFO
--rw-r-----   0 danijar  (322066) primarygroup (89939)    10443 2024-05-10 21:35:11.000000 elements-3.4.1/README.md
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-13 22:50:35.582840 elements-3.4.1/elements/
--rw-r-----   0 danijar  (322066) primarygroup (89939)      541 2024-05-13 22:50:26.000000 elements-3.4.1/elements/__init__.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3540 2024-02-05 03:02:13.000000 elements-3.4.1/elements/agg.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3370 2023-12-10 19:55:19.000000 elements-3.4.1/elements/checkpoint.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     5998 2024-02-05 02:06:54.000000 elements-3.4.1/elements/config.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)      916 2023-12-10 19:47:36.000000 elements-3.4.1/elements/counter.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     4211 2023-12-13 01:50:18.000000 elements-3.4.1/elements/flags.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)      320 2023-12-10 19:43:58.000000 elements-3.4.1/elements/fps.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)    12996 2024-02-06 00:22:22.000000 elements-3.4.1/elements/logger.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     6870 2024-05-13 22:50:21.000000 elements-3.4.1/elements/path.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     6052 2023-12-10 19:43:58.000000 elements-3.4.1/elements/plotting.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3169 2023-12-10 19:52:49.000000 elements-3.4.1/elements/printing.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1630 2023-12-10 19:47:10.000000 elements-3.4.1/elements/rwlock.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2847 2023-12-10 19:47:13.000000 elements-3.4.1/elements/timer.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1443 2024-05-10 21:58:03.000000 elements-3.4.1/elements/tree.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     7666 2023-12-10 19:47:25.000000 elements-3.4.1/elements/usage.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)      228 2024-02-26 02:12:34.000000 elements-3.4.1/elements/utils.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2199 2023-12-10 19:54:08.000000 elements-3.4.1/elements/uuid.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1671 2023-12-10 19:47:30.000000 elements-3.4.1/elements/when.py
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-13 22:50:35.586840 elements-3.4.1/elements.egg-info/
--rw-r-----   0 danijar  (322066) primarygroup (89939)    10803 2024-05-13 22:50:35.000000 elements-3.4.1/elements.egg-info/PKG-INFO
--rw-r-----   0 danijar  (322066) primarygroup (89939)      654 2024-05-13 22:50:35.000000 elements-3.4.1/elements.egg-info/SOURCES.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)        1 2024-05-13 22:50:35.000000 elements-3.4.1/elements.egg-info/dependency_links.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       39 2024-05-13 22:50:35.000000 elements-3.4.1/elements.egg-info/requires.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)        9 2024-05-13 22:50:35.000000 elements-3.4.1/elements.egg-info/top_level.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       53 2024-05-13 22:39:18.000000 elements-3.4.1/requirements-optional.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       39 2024-05-13 22:39:20.000000 elements-3.4.1/requirements.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       38 2024-05-13 22:50:35.586840 elements-3.4.1/setup.cfg
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1095 2023-12-10 20:02:30.000000 elements-3.4.1/setup.py
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-13 22:50:35.586840 elements-3.4.1/tests/
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2112 2023-12-10 20:38:32.000000 elements-3.4.1/tests/test_basics.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     4454 2023-12-13 01:48:36.000000 elements-3.4.1/tests/test_flags.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1506 2024-05-10 21:58:08.000000 elements-3.4.1/tests/test_path.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2331 2024-05-10 22:02:36.000000 elements-3.4.1/tests/test_tree.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-20 19:05:33.913949 elements-3.5.0/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1058 2023-12-10 19:43:58.000000 elements-3.5.0/LICENSE
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       59 2023-12-10 19:43:58.000000 elements-3.5.0/MANIFEST.in
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    10803 2024-05-20 19:05:33.913949 elements-3.5.0/PKG-INFO
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    10443 2024-05-10 21:35:11.000000 elements-3.5.0/README.md
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-20 19:05:33.909949 elements-3.5.0/elements/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      551 2024-05-20 19:03:34.000000 elements-3.5.0/elements/__init__.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3540 2024-02-05 03:02:13.000000 elements-3.5.0/elements/agg.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3993 2024-05-20 19:03:19.000000 elements-3.5.0/elements/checkpoint.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     5998 2024-02-05 02:06:54.000000 elements-3.5.0/elements/config.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      916 2023-12-10 19:47:36.000000 elements-3.5.0/elements/counter.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     4211 2023-12-13 01:50:18.000000 elements-3.5.0/elements/flags.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      320 2023-12-10 19:43:58.000000 elements-3.5.0/elements/fps.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    12996 2024-02-06 00:22:22.000000 elements-3.5.0/elements/logger.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     7702 2024-05-16 00:32:50.000000 elements-3.5.0/elements/path.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     6052 2023-12-10 19:43:58.000000 elements-3.5.0/elements/plotting.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3169 2023-12-10 19:52:49.000000 elements-3.5.0/elements/printing.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1630 2023-12-10 19:47:10.000000 elements-3.5.0/elements/rwlock.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2847 2023-12-10 19:47:13.000000 elements-3.5.0/elements/timer.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1443 2024-05-10 21:58:03.000000 elements-3.5.0/elements/tree.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     7666 2023-12-10 19:47:25.000000 elements-3.5.0/elements/usage.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      228 2024-02-26 02:12:34.000000 elements-3.5.0/elements/utils.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2199 2023-12-10 19:54:08.000000 elements-3.5.0/elements/uuid.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1671 2023-12-10 19:47:30.000000 elements-3.5.0/elements/when.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-20 19:05:33.909949 elements-3.5.0/elements.egg-info/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    10803 2024-05-20 19:05:33.000000 elements-3.5.0/elements.egg-info/PKG-INFO
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      679 2024-05-20 19:05:33.000000 elements-3.5.0/elements.egg-info/SOURCES.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        1 2024-05-20 19:05:33.000000 elements-3.5.0/elements.egg-info/dependency_links.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       66 2024-05-20 19:05:33.000000 elements-3.5.0/elements.egg-info/requires.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        9 2024-05-20 19:05:33.000000 elements-3.5.0/elements.egg-info/top_level.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       53 2024-05-13 22:39:18.000000 elements-3.5.0/requirements-optional.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       66 2024-05-14 17:34:25.000000 elements-3.5.0/requirements.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       38 2024-05-20 19:05:33.913949 elements-3.5.0/setup.cfg
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1095 2023-12-10 20:02:30.000000 elements-3.5.0/setup.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-20 19:05:33.913949 elements-3.5.0/tests/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2112 2024-05-20 18:51:09.000000 elements-3.5.0/tests/test_basics.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1889 2024-05-20 19:03:28.000000 elements-3.5.0/tests/test_checkpoint.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     4454 2023-12-13 01:48:36.000000 elements-3.5.0/tests/test_flags.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1505 2024-05-14 17:33:06.000000 elements-3.5.0/tests/test_path.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2331 2024-05-10 22:02:36.000000 elements-3.5.0/tests/test_tree.py
```

### Comparing `elements-3.4.1/LICENSE` & `elements-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `elements-3.4.1/PKG-INFO` & `elements-3.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elements
-Version: 3.4.1
+Version: 3.5.0
 Summary: Building blocks for productive research.
 Home-page: http://github.com/danijar/elements
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `elements-3.4.1/README.md` & `elements-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `elements-3.4.1/elements/__init__.py` & `elements-3.5.0/elements/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-__version__ = '3.4.1'
+__version__ = '3.5.0'
 
 from .agg import Agg
-from .checkpoint import Checkpoint
+from .checkpoint import Checkpoint, Saveable
 from .config import Config
 from .counter import Counter
 from .flags import Flags
 from .fps import FPS
 from .logger import Logger
 from .path import Path
 from .printing import format_ as format
```

### Comparing `elements-3.4.1/elements/agg.py` & `elements-3.5.0/elements/agg.py`

 * *Files identical despite different names*

### Comparing `elements-3.4.1/elements/checkpoint.py` & `elements-3.5.0/elements/checkpoint.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,23 +3,49 @@
 import time
 
 from . import printing
 from . import path
 from . import timer
 
 
+class Saveable:
+
+  """Helper for creating the `save() -> data` and `load(data)` methods that
+  make an object saveable."""
+
+  def __init__(self, attrs=None, save=None, load=None):
+    assert bool(save) == bool(load)
+    assert bool(save) != bool(attrs)
+    self._save = save
+    self._load = load
+    self._attrs = attrs
+
+  def save(self):
+    if self._save:
+      return self._save()
+    if self._attrs:
+      return {k: getattr(self, k) for k in self._attrs}
+
+  def load(self, data):
+    if self._load:
+      return self._load(data)
+    if self._attrs:
+      for key in self._attrs:
+        setattr(self, key, data[key])
+
+
 class Checkpoint:
 
   def __init__(self, filename=None, parallel=True):
     self._filename = filename and path.Path(filename)
     self._values = {}
     self._parallel = parallel
+    self._promise = None
     if self._parallel:
       self._worker = concurrent.futures.ThreadPoolExecutor(1, 'checkpoint')
-      self._promise = None
 
   def __setattr__(self, name, value):
     if name in ('exists', 'save', 'load'):
       return super().__setattr__(name, value)
     if name.startswith('_'):
       return super().__setattr__(name, value)
     has_load = hasattr(value, 'load') and callable(value.load)
@@ -47,25 +73,25 @@
       print('Did not find any checkpoint.')
     return exists
 
   def save(self, filename=None, keys=None):
     assert self._filename or filename
     filename = path.Path(filename or self._filename)
     printing.print_(f'Writing checkpoint: {filename}')
+    keys = tuple(self._values.keys() if keys is None else keys)
+    assert all([not k.startswith('_') for k in keys]), keys
+    data = {k: self._values[k].save() for k in keys}
     if self._parallel:
       self._promise and self._promise.result()
-      self._promise = self._worker.submit(self._save, filename, keys)
+      self._promise = self._worker.submit(self._save, filename, data)
     else:
-      self._save(filename, keys)
+      self._save(filename, data)
 
   @timer.section('checkpoint_save')
-  def _save(self, filename, keys):
-    keys = tuple(self._values.keys() if keys is None else keys)
-    assert all([not k.startswith('_') for k in keys]), keys
-    data = {k: self._values[k].save() for k in keys}
+  def _save(self, filename, data):
     data['_timestamp'] = time.time()
     filename.parent.mkdirs()
     content = pickle.dumps(data)
     if str(filename).startswith('gs://'):
       filename.write(content, mode='wb')
     else:
       # Write to a temporary file and then atomically rename, so that the file
```

### Comparing `elements-3.4.1/elements/config.py` & `elements-3.5.0/elements/config.py`

 * *Files identical despite different names*

### Comparing `elements-3.4.1/elements/counter.py` & `elements-3.5.0/elements/counter.py`

 * *Files identical despite different names*

### Comparing `elements-3.4.1/elements/flags.py` & `elements-3.5.0/elements/flags.py`

 * *Files identical despite different names*

### Comparing `elements-3.4.1/elements/logger.py` & `elements-3.5.0/elements/logger.py`

 * *Files identical despite different names*

### Comparing `elements-3.4.1/elements/path.py` & `elements-3.5.0/elements/path.py`

 * *Files 5% similar despite different names*

```diff
@@ -179,16 +179,27 @@
     super().__init__(path)
     if not type(self).fs:
       import gcsfs
       type(self).fs = gcsfs.GCSFileSystem()
 
   @contextlib.contextmanager
   def open(self, mode='r'):
+    print('### open gcp path:', str(self))
     yield self.fs.open(str(self), mode)
 
+  # def read(self, mode='r'):
+  #   assert mode in 'r rb'.split(), mode
+  #   with self.open(mode) as f:
+  #     return f.read()
+
+  # def write(self, content, mode='w'):
+  #   assert mode in 'w a wb ab'.split(), mode
+  #   with self.open(mode) as f:
+  #     f.write(content)
+
   def absolute(self):
     return self
 
   def glob(self, pattern):
     path = str(self)
     protocol = path.split('://', 1)[0] + '://' if '://' in path else ''
     for path in self.fs.glob(f'{str(self)}/{pattern}'):
@@ -217,14 +228,55 @@
     self.fs.copy(str(self), str(dest), recursive=True)
 
   def move(self, dest):
     dest = Path(dest)
     self.fs.mv(self, str(dest), recursive=True)
 
 
+class GCSFile:
+
+  def __init__(self):
+    self._closed = False
+
+  @property
+  def closed(self):
+    return self._closed
+
+  def __len__(self):
+    pass
+
+  def __enter__(self):
+    pass
+
+  def __exit__(self, *args):
+    self.close()
+
+  def read(self, size=-1):
+    pass
+
+  def readline(self, size=-1):
+    pass
+
+  def seek(self, offset, whence=0):
+    pass
+
+  def tell(self):
+    pass
+
+  def write(self, data):
+    size = 0
+    return size
+
+  def flush(self):
+    pass
+
+  def close(self):
+    self._closed = True
+
+
 class TFPath(Path):
 
   __slots__ = ('_path',)
 
   gfile = None
 
   def __init__(self, path):
```

### Comparing `elements-3.4.1/elements/plotting.py` & `elements-3.5.0/elements/plotting.py`

 * *Files identical despite different names*

### Comparing `elements-3.4.1/elements/printing.py` & `elements-3.5.0/elements/printing.py`

 * *Files identical despite different names*

### Comparing `elements-3.4.1/elements/rwlock.py` & `elements-3.5.0/elements/rwlock.py`

 * *Files identical despite different names*

### Comparing `elements-3.4.1/elements/timer.py` & `elements-3.5.0/elements/timer.py`

 * *Files identical despite different names*

### Comparing `elements-3.4.1/elements/tree.py` & `elements-3.5.0/elements/tree.py`

 * *Files identical despite different names*

### Comparing `elements-3.4.1/elements/usage.py` & `elements-3.5.0/elements/usage.py`

 * *Files identical despite different names*

### Comparing `elements-3.4.1/elements/uuid.py` & `elements-3.5.0/elements/uuid.py`

 * *Files identical despite different names*

### Comparing `elements-3.4.1/elements/when.py` & `elements-3.5.0/elements/when.py`

 * *Files identical despite different names*

### Comparing `elements-3.4.1/elements.egg-info/PKG-INFO` & `elements-3.5.0/elements.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elements
-Version: 3.4.1
+Version: 3.5.0
 Summary: Building blocks for productive research.
 Home-page: http://github.com/danijar/elements
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `elements-3.4.1/elements.egg-info/SOURCES.txt` & `elements-3.5.0/elements.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,10 +24,11 @@
 elements/when.py
 elements.egg-info/PKG-INFO
 elements.egg-info/SOURCES.txt
 elements.egg-info/dependency_links.txt
 elements.egg-info/requires.txt
 elements.egg-info/top_level.txt
 tests/test_basics.py
+tests/test_checkpoint.py
 tests/test_flags.py
 tests/test_path.py
 tests/test_tree.py
```

### Comparing `elements-3.4.1/setup.py` & `elements-3.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `elements-3.4.1/tests/test_basics.py` & `elements-3.5.0/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `elements-3.4.1/tests/test_flags.py` & `elements-3.5.0/tests/test_flags.py`

 * *Files identical despite different names*

### Comparing `elements-3.4.1/tests/test_path.py` & `elements-3.5.0/tests/test_path.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import elements
+import pytest
 
 
 class TestPath:
 
   def test_str_canonical(self):
     examples = ['/', 'foo/bar', 'file.txt', '/bar.tar.gz']
     for example in examples:
@@ -27,18 +28,18 @@
     assert str(elements.Path('./foo')) == 'foo'
 
   def test_trailing_slash(self):
     assert str(elements.Path('./')) == '.'
     assert str(elements.Path('a/')) == 'a'
     assert str(elements.Path('foo/bar/')) == 'foo/bar'
 
-  # @pytest.mark.filterwarnings('ignore::DeprecationWarning')
-  # def test_protocols(self):
-  #   assert str(elements.Path('gs://')) == ('gs://')
-  #   assert str(elements.Path('gs://foo/bar')) == 'gs://foo/bar'
+  @pytest.mark.filterwarnings('ignore::UserWarning')
+  def test_protocols(self):
+    assert str(elements.Path('gs://')) == ('gs://')
+    assert str(elements.Path('gs://foo/bar')) == 'gs://foo/bar'
 
   def test_parent(self):
     empty = elements.Path('.')
     root = elements.Path('/')
     assert (root / 'foo' / 'bar.txt').parent.parent == root
     assert (empty / 'foo' / 'bar.txt').parent.parent == empty
     assert root.parent == root
```

### Comparing `elements-3.4.1/tests/test_tree.py` & `elements-3.5.0/tests/test_tree.py`

 * *Files identical despite different names*

