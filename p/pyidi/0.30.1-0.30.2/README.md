# Comparing `tmp/pyidi-0.30.1.tar.gz` & `tmp/pyidi-0.30.2.tar.gz`

## Comparing `pyidi-0.30.1.tar` & `pyidi-0.30.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 pyidi-0.30.1/pyidi/__init__.py
--rw-r--r--   0        0        0    13604 2020-02-02 00:00:00.000000 pyidi-0.30.1/pyidi/gui.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 pyidi-0.30.1/pyidi/load_analysis.py
--rw-r--r--   0        0        0    20874 2020-02-02 00:00:00.000000 pyidi-0.30.1/pyidi/pyidi.py
--rw-r--r--   0        0        0    15253 2020-02-02 00:00:00.000000 pyidi-0.30.1/pyidi/selection.py
--rw-r--r--   0        0        0    12405 2020-02-02 00:00:00.000000 pyidi-0.30.1/pyidi/tools.py
--rw-r--r--   0        0        0     9257 2020-02-02 00:00:00.000000 pyidi-0.30.1/pyidi/video_reader.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 pyidi-0.30.1/pyidi/methods/__init__.py
--rw-r--r--   0        0        0     7249 2020-02-02 00:00:00.000000 pyidi-0.30.1/pyidi/methods/_gradient_based_optical_flow.py
--rw-r--r--   0        0        0    29292 2020-02-02 00:00:00.000000 pyidi-0.30.1/pyidi/methods/_lucas_kanade.py
--rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 pyidi-0.30.1/pyidi/methods/_lucas_kanade_scipy.py
--rw-r--r--   0        0        0    25982 2020-02-02 00:00:00.000000 pyidi-0.30.1/pyidi/methods/_lucas_kanade_scipy2.py
--rw-r--r--   0        0        0    16877 2020-02-02 00:00:00.000000 pyidi-0.30.1/pyidi/methods/_simplified_optical_flow.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 pyidi-0.30.1/pyidi/methods/idi_method.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 pyidi-0.30.1/pyidi/postprocessing/__init__.py
--rw-r--r--   0        0        0    18261 2020-02-02 00:00:00.000000 pyidi-0.30.1/pyidi/postprocessing/_motion_magnification.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 pyidi-0.30.1/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pyidi-0.30.1/LICENSE
--rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 pyidi-0.30.1/README.md
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 pyidi-0.30.1/pyproject.toml
--rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 pyidi-0.30.1/PKG-INFO
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 pyidi-0.30.2/pyidi/__init__.py
+-rw-r--r--   0        0        0    13604 2020-02-02 00:00:00.000000 pyidi-0.30.2/pyidi/gui.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 pyidi-0.30.2/pyidi/load_analysis.py
+-rw-r--r--   0        0        0    21063 2020-02-02 00:00:00.000000 pyidi-0.30.2/pyidi/pyidi.py
+-rw-r--r--   0        0        0    15253 2020-02-02 00:00:00.000000 pyidi-0.30.2/pyidi/selection.py
+-rw-r--r--   0        0        0    12405 2020-02-02 00:00:00.000000 pyidi-0.30.2/pyidi/tools.py
+-rw-r--r--   0        0        0     9615 2020-02-02 00:00:00.000000 pyidi-0.30.2/pyidi/video_reader.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 pyidi-0.30.2/pyidi/methods/__init__.py
+-rw-r--r--   0        0        0     7249 2020-02-02 00:00:00.000000 pyidi-0.30.2/pyidi/methods/_gradient_based_optical_flow.py
+-rw-r--r--   0        0        0    29292 2020-02-02 00:00:00.000000 pyidi-0.30.2/pyidi/methods/_lucas_kanade.py
+-rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 pyidi-0.30.2/pyidi/methods/_lucas_kanade_scipy.py
+-rw-r--r--   0        0        0    25982 2020-02-02 00:00:00.000000 pyidi-0.30.2/pyidi/methods/_lucas_kanade_scipy2.py
+-rw-r--r--   0        0        0    16877 2020-02-02 00:00:00.000000 pyidi-0.30.2/pyidi/methods/_simplified_optical_flow.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 pyidi-0.30.2/pyidi/methods/idi_method.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 pyidi-0.30.2/pyidi/postprocessing/__init__.py
+-rw-r--r--   0        0        0    18261 2020-02-02 00:00:00.000000 pyidi-0.30.2/pyidi/postprocessing/_motion_magnification.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 pyidi-0.30.2/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pyidi-0.30.2/LICENSE
+-rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 pyidi-0.30.2/README.md
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 pyidi-0.30.2/pyproject.toml
+-rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 pyidi-0.30.2/PKG-INFO
```

### Comparing `pyidi-0.30.1/pyidi/gui.py` & `pyidi-0.30.2/pyidi/gui.py`

 * *Files identical despite different names*

### Comparing `pyidi-0.30.1/pyidi/load_analysis.py` & `pyidi-0.30.2/pyidi/load_analysis.py`

 * *Files identical despite different names*

### Comparing `pyidi-0.30.1/pyidi/pyidi.py` & `pyidi-0.30.2/pyidi/pyidi.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,21 +183,19 @@
                     self.method.clear_temp_files()
                     
             return self.displacements
         else:
             raise ValueError('IDI method has not yet been set. Please call `set_method()` first.')
 
 
-    # def close_video(self):
-    #     """
-    #     Close the .mraw video memmap.
-    #     """
-    #     if hasattr(self, 'mraw'):
-    #         self.mraw._mmap.close()
-    #         del self.mraw
+    def close_video(self):
+        """
+        Close the .mraw video memmap.
+        """
+        self.reader.close()
     
 
     def create_analysis_directory(self):
         if type(self.cih_file) == str:
             cih_file_ = os.path.split(self.cih_file)[-1].split('.')[0]
         else:
             cih_file_ = 'ndarary_video'
@@ -226,15 +224,15 @@
         out = {
             'info': {
                 'width': self.reader.image_width,
                 'height': self.reader.image_height,
                 'N': self.reader.N
             },
             'createdate': datetime.datetime.now().strftime("%Y %m %d    %H:%M:%S"),
-            'cih_file': self.cih_file,
+            'cih_file': self.cih_file if type(self.cih_file) == str else 'ndarray',
             'settings': self.method.create_settings_dict(),
             'method': self.method_name
         }
 
         with open(os.path.join(root, 'settings.txt'), 'w') as f:
             json.dump(out, f, sort_keys=True, indent=2)
 
@@ -265,14 +263,19 @@
     def gui(self):
         self.gui_obj = gui.gui(self)
 
     @property
     def mraw(self):
         warnings.warn('`self.mraw` is deprecated and will be removed in the next version. Please use `self.reader.mraw` instead.', DeprecationWarning)
         return self.reader.mraw
+    
+    @property
+    def info(self):
+        #warnings.warn('`self.info` is deprecated and will be removed in the next version. Please use `self.reader.info` instead.', DeprecationWarning)
+        return self.reader.info
 
 #     def gui(self):
 #         """Napari interface.
 #         """
 #         available_gui_methods = [
 #             ('---', '---'),
 #             ('Simplified Optical Flow', 'sof'),
```

### Comparing `pyidi-0.30.1/pyidi/selection.py` & `pyidi-0.30.2/pyidi/selection.py`

 * *Files identical despite different names*

### Comparing `pyidi-0.30.1/pyidi/tools.py` & `pyidi-0.30.2/pyidi/tools.py`

 * *Files identical despite different names*

### Comparing `pyidi-0.30.1/pyidi/video_reader.py` & `pyidi-0.30.2/pyidi/video_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 
 
         if self.file_format in PHORTRON_HEADER_FILE:
             self.mraw, info = pyMRAW.load_video(input_file)
             self.N = info['Total Frame']
             self.image_width = info['Image Width']
             self.image_height = info['Image Height']
+            self.info = info
         
         elif self.file_format in SUPPORTED_IMAGE_FORMATS:
             image_prop = iio.improps(input_file)
             self.image_meta = iio.immeta(input_file, plugin='pyav')
             if image_prop.n_images is None:
                 self.is_n_images = False
                 sc_dir = os.scandir(self.root)
@@ -185,14 +186,23 @@
             image = iio.imread(input_file, index=frame_number, plugin='pyav')
             image = image[:, :, CHANNELS.get(use_channel.upper())]
         
         else:
             raise ValueError('Unsupported channel! Only R, G, B and Y are supported.')
 
         return image
+    
+    def close(self):
+        """
+        Close the video and clear the resources.
+        In case of a MRAW video, closes the memory map for "mraw" file format.
+        """
+        if hasattr(self, 'mraw') and self.file_format in PHORTRON_HEADER_FILE:
+            self.mraw._mmap.close()
+            del self.mraw
 
 def _rgb2luma(rgb_image):
     """Converts "RGB" image to "YUV" and returns only "Y" (luma) component.
 
     :param rgb_image: "RGB" image "(w, h, channels)"
     :type rgb_image: numpy.array
     :return: luma image
```

### Comparing `pyidi-0.30.1/pyidi/methods/_gradient_based_optical_flow.py` & `pyidi-0.30.2/pyidi/methods/_gradient_based_optical_flow.py`

 * *Files identical despite different names*

### Comparing `pyidi-0.30.1/pyidi/methods/_lucas_kanade.py` & `pyidi-0.30.2/pyidi/methods/_lucas_kanade.py`

 * *Files identical despite different names*

### Comparing `pyidi-0.30.1/pyidi/methods/_lucas_kanade_scipy.py` & `pyidi-0.30.2/pyidi/methods/_lucas_kanade_scipy.py`

 * *Files identical despite different names*

### Comparing `pyidi-0.30.1/pyidi/methods/_lucas_kanade_scipy2.py` & `pyidi-0.30.2/pyidi/methods/_lucas_kanade_scipy2.py`

 * *Files identical despite different names*

### Comparing `pyidi-0.30.1/pyidi/methods/_simplified_optical_flow.py` & `pyidi-0.30.2/pyidi/methods/_simplified_optical_flow.py`

 * *Files identical despite different names*

### Comparing `pyidi-0.30.1/pyidi/methods/idi_method.py` & `pyidi-0.30.2/pyidi/methods/idi_method.py`

 * *Files identical despite different names*

### Comparing `pyidi-0.30.1/pyidi/postprocessing/_motion_magnification.py` & `pyidi-0.30.2/pyidi/postprocessing/_motion_magnification.py`

 * *Files identical despite different names*

### Comparing `pyidi-0.30.1/.gitignore` & `pyidi-0.30.2/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -117,8 +117,10 @@
 
 # Pyre type checker
 .pyre/
 
 /data/*.pkl
 
 #other
-server_user_id.txt
+server_user_id.txt
+
+/temp
```

### Comparing `pyidi-0.30.1/LICENSE` & `pyidi-0.30.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyidi-0.30.1/README.md` & `pyidi-0.30.2/README.md`

 * *Files identical despite different names*

### Comparing `pyidi-0.30.1/pyproject.toml` & `pyidi-0.30.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyidi"
-version = "0.30.1"
+version = "0.30.2"
 authors = [{name = "Klemen Zaletelj, Domen Gorjup, Janko Slavič et al.", email = "janko.slavic@fs.uni-lj.si"}]
 maintainers = [{name = "Klemen Zaletelj, Domen Gorjup, Janko Slavič et al.", email = "janko.slavic@fs.uni-lj.si"}]
 license = "MIT"
 description = "Python Image Displacement Identification."
 readme = "README.md"
 keywords = ['computer vision', 'dic', 'gradient-based', 'displacement identification']
 requires-python = ">=3.10"
```

### Comparing `pyidi-0.30.1/PKG-INFO` & `pyidi-0.30.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyidi
-Version: 0.30.1
+Version: 0.30.2
 Summary: Python Image Displacement Identification.
 Project-URL: homepage, https://github.com/ladisk/pyidi
 Project-URL: documentation, https://pyidi.readthedocs.io/en/latest/
 Project-URL: source, https://github.com/ladisk/pyidi
 Author-email: "Klemen Zaletelj, Domen Gorjup, Janko Slavič et al." <janko.slavic@fs.uni-lj.si>
 Maintainer-email: "Klemen Zaletelj, Domen Gorjup, Janko Slavič et al." <janko.slavic@fs.uni-lj.si>
 License-Expression: MIT
```

