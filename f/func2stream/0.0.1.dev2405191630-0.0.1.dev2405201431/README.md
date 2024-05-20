# Comparing `tmp/func2stream-0.0.1.dev2405191630.tar.gz` & `tmp/func2stream-0.0.1.dev2405201431.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "func2stream-0.0.1.dev2405191630.tar", last modified: Sun May 19 16:30:31 2024, max compression
+gzip compressed data, was "func2stream-0.0.1.dev2405201431.tar", last modified: Mon May 20 14:31:04 2024, max compression
```

## Comparing `func2stream-0.0.1.dev2405191630.tar` & `func2stream-0.0.1.dev2405201431.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 16:30:31.800305 func2stream-0.0.1.dev2405191630/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-19 16:30:27.000000 func2stream-0.0.1.dev2405191630/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-05-19 16:30:31.800305 func2stream-0.0.1.dev2405191630/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-19 16:30:27.000000 func2stream-0.0.1.dev2405191630/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 16:30:31.800305 func2stream-0.0.1.dev2405191630/func2stream/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-19 16:30:27.000000 func2stream-0.0.1.dev2405191630/func2stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16943 2024-05-19 16:30:27.000000 func2stream-0.0.1.dev2405191630/func2stream/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-19 16:30:27.000000 func2stream-0.0.1.dev2405191630/func2stream/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-05-19 16:30:27.000000 func2stream-0.0.1.dev2405191630/func2stream/video.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 16:30:31.800305 func2stream-0.0.1.dev2405191630/func2stream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-05-19 16:30:31.000000 func2stream-0.0.1.dev2405191630/func2stream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-19 16:30:31.000000 func2stream-0.0.1.dev2405191630/func2stream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 16:30:31.000000 func2stream-0.0.1.dev2405191630/func2stream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-19 16:30:31.000000 func2stream-0.0.1.dev2405191630/func2stream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-19 16:30:31.000000 func2stream-0.0.1.dev2405191630/func2stream.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-19 16:30:27.000000 func2stream-0.0.1.dev2405191630/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 16:30:31.800305 func2stream-0.0.1.dev2405191630/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-19 16:30:27.000000 func2stream-0.0.1.dev2405191630/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:31:04.788317 func2stream-0.0.1.dev2405201431/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-20 14:31:00.000000 func2stream-0.0.1.dev2405201431/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-05-20 14:31:04.788317 func2stream-0.0.1.dev2405201431/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-20 14:31:00.000000 func2stream-0.0.1.dev2405201431/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:31:04.784317 func2stream-0.0.1.dev2405201431/func2stream/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-20 14:31:00.000000 func2stream-0.0.1.dev2405201431/func2stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16946 2024-05-20 14:31:00.000000 func2stream-0.0.1.dev2405201431/func2stream/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-20 14:31:00.000000 func2stream-0.0.1.dev2405201431/func2stream/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-05-20 14:31:00.000000 func2stream-0.0.1.dev2405201431/func2stream/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:31:04.788317 func2stream-0.0.1.dev2405201431/func2stream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-05-20 14:31:04.000000 func2stream-0.0.1.dev2405201431/func2stream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-20 14:31:04.000000 func2stream-0.0.1.dev2405201431/func2stream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 14:31:04.000000 func2stream-0.0.1.dev2405201431/func2stream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-20 14:31:04.000000 func2stream-0.0.1.dev2405201431/func2stream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-20 14:31:04.000000 func2stream-0.0.1.dev2405201431/func2stream.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-20 14:31:00.000000 func2stream-0.0.1.dev2405201431/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 14:31:04.788317 func2stream-0.0.1.dev2405201431/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-20 14:31:00.000000 func2stream-0.0.1.dev2405201431/setup.py
```

### Comparing `func2stream-0.0.1.dev2405191630/LICENSE` & `func2stream-0.0.1.dev2405201431/LICENSE`

 * *Files identical despite different names*

### Comparing `func2stream-0.0.1.dev2405191630/PKG-INFO` & `func2stream-0.0.1.dev2405201431/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: func2stream
-Version: 0.0.1.dev2405191630
+Version: 0.0.1.dev2405201431
 Summary: Effortlessly transform functions into asynchronous elements for building high-performance pipelines
 Home-page: https://github.com/BICHENG/func2stream
 Author: BI CHENG
 License: MPL-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `func2stream-0.0.1.dev2405191630/README.md` & `func2stream-0.0.1.dev2405201431/README.md`

 * *Files identical despite different names*

### Comparing `func2stream-0.0.1.dev2405191630/func2stream/core.py` & `func2stream-0.0.1.dev2405201431/func2stream/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,17 +221,17 @@
             self.elements[-1].sink = sink;return self
         
         self.set_source=_set_source
         self.set_sink=_set_sink
         
     def start(self):
         assert any([
-            self.elements[-1].sink is not None,
-            isinstance(self.elements[-1], DataSource)
-            ]), f"{self.elements[-1].friendly_name}@{self.friendly_name} has no output queue, cannot start"
+            self.elements[0].source is not None,
+            isinstance(self.elements[0], DataSource)
+            ]), f"{self.elements[0].friendly_name}@{self.friendly_name} has no input queue, cannot start"     
         
         if self.elements[-1].sink is None:
             self.elements[-1].sink = _queue(1, leaky=True)
             print(f"SINK {self.elements[-1].friendly_name} will be a pipe that automatically discards old items when full")
         for i in [0, -1]: self.elements[i].start()
         self.source = self.elements[0].source
         self.sink = self.elements[-1].sink
```

### Comparing `func2stream-0.0.1.dev2405191630/func2stream/utils.py` & `func2stream-0.0.1.dev2405201431/func2stream/utils.py`

 * *Files identical despite different names*

### Comparing `func2stream-0.0.1.dev2405191630/func2stream/video.py` & `func2stream-0.0.1.dev2405201431/func2stream/video.py`

 * *Files identical despite different names*

### Comparing `func2stream-0.0.1.dev2405191630/func2stream.egg-info/PKG-INFO` & `func2stream-0.0.1.dev2405201431/func2stream.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: func2stream
-Version: 0.0.1.dev2405191630
+Version: 0.0.1.dev2405201431
 Summary: Effortlessly transform functions into asynchronous elements for building high-performance pipelines
 Home-page: https://github.com/BICHENG/func2stream
 Author: BI CHENG
 License: MPL-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `func2stream-0.0.1.dev2405191630/setup.py` & `func2stream-0.0.1.dev2405201431/setup.py`

 * *Files identical despite different names*

