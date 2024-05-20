# Comparing `tmp/sanghyunjo-1.0.1.tar.gz` & `tmp/sanghyunjo-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sanghyunjo-1.0.1.tar", last modified: Thu May 16 08:18:46 2024, max compression
+gzip compressed data, was "dist\sanghyunjo-1.1.0.tar", last modified: Mon May 20 07:11:26 2024, max compression
```

## Comparing `sanghyunjo-1.0.1.tar` & `sanghyunjo-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 08:18:46.460187 sanghyunjo-1.0.1/
--rw-rw-rw-   0        0        0     1087 2024-05-16 07:32:54.000000 sanghyunjo-1.0.1/LICENSE
--rw-rw-rw-   0        0        0       53 2024-05-16 07:24:52.000000 sanghyunjo-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      365 2024-05-16 08:18:46.459190 sanghyunjo-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1029 2024-05-16 07:32:26.000000 sanghyunjo-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 08:18:46.436208 sanghyunjo-1.0.1/sanghyunjo/
--rw-rw-rw-   0        0        0       90 2024-05-16 08:18:19.000000 sanghyunjo-1.0.1/sanghyunjo/__init__.py
--rw-rw-rw-   0        0        0     8746 2024-05-16 07:27:12.000000 sanghyunjo-1.0.1/sanghyunjo/cv.py
-drwxrwxrwx   0        0        0        0 2024-05-16 08:18:46.449175 sanghyunjo-1.0.1/sanghyunjo/fonts/
--rw-rw-rw-   0        0        0    34888 2023-07-19 08:59:35.000000 sanghyunjo-1.0.1/sanghyunjo/fonts/Times New Roman MT Std.otf
--rw-rw-rw-   0        0        0      348 2024-05-16 06:52:07.000000 sanghyunjo-1.0.1/sanghyunjo/json_utils.py
--rw-rw-rw-   0        0        0     2795 2024-05-16 07:13:32.000000 sanghyunjo-1.0.1/sanghyunjo/misc.py
-drwxrwxrwx   0        0        0        0 2024-05-16 08:18:46.451169 sanghyunjo-1.0.1/sanghyunjo.egg-info/
--rw-rw-rw-   0        0        0      365 2024-05-16 08:18:46.000000 sanghyunjo-1.0.1/sanghyunjo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2024-05-16 08:18:46.000000 sanghyunjo-1.0.1/sanghyunjo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 08:18:46.000000 sanghyunjo-1.0.1/sanghyunjo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-16 07:28:15.000000 sanghyunjo-1.0.1/sanghyunjo.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-16 08:18:46.000000 sanghyunjo-1.0.1/sanghyunjo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 08:18:46.461185 sanghyunjo-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      792 2024-05-16 08:17:50.000000 sanghyunjo-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:11:26.869385 sanghyunjo-1.1.0/
+-rw-rw-rw-   0        0        0     1087 2024-05-16 07:32:54.000000 sanghyunjo-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0       53 2024-05-16 07:24:52.000000 sanghyunjo-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      365 2024-05-20 07:11:26.868386 sanghyunjo-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1029 2024-05-16 07:32:26.000000 sanghyunjo-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 07:11:26.846438 sanghyunjo-1.1.0/sanghyunjo/
+-rw-rw-rw-   0        0        0      188 2024-05-20 07:11:20.000000 sanghyunjo-1.1.0/sanghyunjo/__init__.py
+-rw-rw-rw-   0        0        0     8772 2024-05-20 07:10:55.000000 sanghyunjo-1.1.0/sanghyunjo/cv.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:11:26.866391 sanghyunjo-1.1.0/sanghyunjo/fonts/
+-rw-rw-rw-   0        0        0    34888 2023-07-19 08:59:35.000000 sanghyunjo-1.1.0/sanghyunjo/fonts/Times New Roman MT Std.otf
+-rw-rw-rw-   0        0        0      358 2024-05-20 07:08:56.000000 sanghyunjo-1.1.0/sanghyunjo/json_utils.py
+-rw-rw-rw-   0        0        0     2795 2024-05-16 07:13:32.000000 sanghyunjo-1.1.0/sanghyunjo/misc.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:11:26.867389 sanghyunjo-1.1.0/sanghyunjo.egg-info/
+-rw-rw-rw-   0        0        0      365 2024-05-20 07:11:26.000000 sanghyunjo-1.1.0/sanghyunjo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2024-05-20 07:11:26.000000 sanghyunjo-1.1.0/sanghyunjo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 07:11:26.000000 sanghyunjo-1.1.0/sanghyunjo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-16 07:28:15.000000 sanghyunjo-1.1.0/sanghyunjo.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-20 07:11:26.000000 sanghyunjo-1.1.0/sanghyunjo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 07:11:26.869385 sanghyunjo-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      828 2024-05-20 07:09:32.000000 sanghyunjo-1.1.0/setup.py
```

### Comparing `sanghyunjo-1.0.1/LICENSE` & `sanghyunjo-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sanghyunjo-1.0.1/README.md` & `sanghyunjo-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `sanghyunjo-1.0.1/sanghyunjo/cv.py` & `sanghyunjo-1.1.0/sanghyunjo/cv.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         elif event == cv2.EVENT_RBUTTONDOWN: self.rightdown(x, y)
         elif event == cv2.EVENT_RBUTTONUP: self.rightup(x, y)
         elif event == cv2.EVENT_MOUSEMOVE: self.move(x, y)
         elif event == cv2.EVENT_MOUSEWHEEL: 
             if flags > 0: self.wheelup()
             else: self.wheeldown()
 
-def imread(path, mode='opencv', unicode=False, mask=False):
+def read_image(path, mode='opencv', unicode=False, mask=False):
     if mode == 'opencv': 
         if unicode: 
             return cv2.imdecode(
                 np.fromfile(path, dtype=np.uint8), 
                 cv2.IMREAD_UNCHANGED
             )
         else: 
@@ -51,37 +51,25 @@
     else: 
         try: 
             image = Image.open(path)
             return image if mask else image.convert('RGB')
         except FileNotFoundError: 
             return None
 
-def imwrite(path, image, palette=None):
+def write_image(path, image, palette=None):
     if palette is None: cv2.imwrite(path, image)
     else:
         image = Image.fromarray(image.astype(np.uint8)).convert('P')
         image.putpalette(palette)
         image.save(path)
 
-def imshow(winname, image, wait=-1, title=''):
-    cv2.imshow(winname, image)
-
-    if len(title) > 0:
-        cv2.setWindowTitle(winname, title)
-
-    key = None
-    if wait >= 0:
-        key = cv2.waitKey(wait)
-
-    return key
-
-def viread(path):
+def read_video(path):
     return VideoReader(path)
 
-def viwrite(path, frames, fps):
+def write_video(path, frames, fps):
     h, w = frames[0].shape[:2]
     
     writer = VideoWriter(path, w, h, fps)
     for frame in frames:
         writer(frame)
     writer.close()
 
@@ -183,32 +171,44 @@
     drw = ImageDraw.Draw(pillow_image)
     drw.ellipse(
         [(x-size, y-size), (x+size, y+size)], 
         (b, g, r, 0), (eb, eg, er, 0), edge_size
     )
     image[:, :, :] = np.asarray(pillow_image)
 
-def showHeatmaps(heatmaps, tags=None, image=None, option='SEISMIC', norm=False):
+def show_image(winname, image, wait=-1, title=''):
+    cv2.imshow(winname, image)
+
+    if len(title) > 0:
+        cv2.setWindowTitle(winname, title)
+
+    key = None
+    if wait >= 0:
+        key = cv2.waitKey(wait)
+
+    return key
+
+def visualize_heatmaps(heatmaps, tags=None, image=None, option='SEISMIC', norm=False):
     vis_heatmaps = []
 
     if image is not None:
-        drawText(image, 'Input', (0, 0))
+        draw_text(image, 'Input', (0, 0))
         vis_heatmaps.append(image)
 
     if tags is None:
         tags = [None for _ in heatmaps]
 
     for tag, heatmap in zip(tags, heatmaps):
         if norm: 
             min_v = heatmap.min()
             max_v = heatmap.max()
             heatmap = (heatmap - min_v) / (max_v - min_v + 1e-5)
         
-        heatmap = applyColor(heatmap, option)
-        if tag is not None: drawText(heatmap, tag, (0, 0), font_size=40)
+        heatmap = colorize(heatmap, option)
+        if tag is not None: draw_text(heatmap, tag, (0, 0), font_size=40)
         vis_heatmaps.append(heatmap)
 
     return np.concatenate(vis_heatmaps, axis=1)
 
 def resize(image, size=None, scale=None, mode='bicubic'):
     inp_dict = {
         'bicubic': cv2.INTER_CUBIC,
```

### Comparing `sanghyunjo-1.0.1/sanghyunjo/fonts/Times New Roman MT Std.otf` & `sanghyunjo-1.1.0/sanghyunjo/fonts/Times New Roman MT Std.otf`

 * *Files identical despite different names*

### Comparing `sanghyunjo-1.0.1/sanghyunjo/misc.py` & `sanghyunjo-1.1.0/sanghyunjo/misc.py`

 * *Files identical despite different names*

### Comparing `sanghyunjo-1.0.1/setup.py` & `sanghyunjo-1.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from setuptools import setup, find_packages
 
+import sanghyunjo as shj
+
 setup(
     name='sanghyunjo',
-    version='1.0.1',
+    version=shj.__version__,
     description='Wrapped utility functions for existing AI packages to simplify their usage',
     author='Sanghyun Jo (shjo-april)',
     author_email='shjo.april@gmail.com',
     url='https://github.com/shjo-april/sanghyunjo',
     install_requires=[],
     packages=find_packages(exclude=[]),
     keywords=['sanghyun', 'sanghyunjo', 'shjo', 'ai', 'utils', 'wrapper'],
```

