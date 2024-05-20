# Comparing `tmp/sphinx-plot-directive-1.0.2.tar.gz` & `tmp/sphinx-plot-directive-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-plot-directive-1.0.2.tar", last modified: Mon Feb  5 02:39:57 2024, max compression
+gzip compressed data, was "sphinx-plot-directive-1.0.3.tar", last modified: Mon May 20 03:35:39 2024, max compression
```

## Comparing `sphinx-plot-directive-1.0.2.tar` & `sphinx-plot-directive-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 test1     (1000) test1     (1000)        0 2024-02-05 02:39:57.604643 sphinx-plot-directive-1.0.2/
--rw-r--r--   0 test1     (1000) test1     (1000)     1418 2024-01-31 03:06:42.000000 sphinx-plot-directive-1.0.2/LICENSE
--rw-r--r--   0 test1     (1000) test1     (1000)       51 2024-01-31 03:06:42.000000 sphinx-plot-directive-1.0.2/MANIFEST.in
--rw-rw-r--   0 test1     (1000) test1     (1000)    15816 2024-02-05 02:39:57.604643 sphinx-plot-directive-1.0.2/PKG-INFO
--rw-r--r--   0 test1     (1000) test1     (1000)    15331 2024-02-05 02:33:58.000000 sphinx-plot-directive-1.0.2/README.rst
--rw-r--r--   0 test1     (1000) test1     (1000)       76 2024-02-05 02:39:57.608643 sphinx-plot-directive-1.0.2/setup.cfg
--rw-r--r--   0 test1     (1000) test1     (1000)      682 2024-02-05 02:37:33.000000 sphinx-plot-directive-1.0.2/setup.py
-drwxrwxr-x   0 test1     (1000) test1     (1000)        0 2024-02-05 02:39:57.604643 sphinx-plot-directive-1.0.2/sphinx_plot_directive/
--rw-r--r--   0 test1     (1000) test1     (1000)    26372 2024-02-04 07:11:47.000000 sphinx-plot-directive-1.0.2/sphinx_plot_directive/__init__.py
-drwxrwxr-x   0 test1     (1000) test1     (1000)        0 2024-02-05 02:39:57.604643 sphinx-plot-directive-1.0.2/sphinx_plot_directive.egg-info/
--rw-rw-r--   0 test1     (1000) test1     (1000)    15816 2024-02-05 02:39:57.000000 sphinx-plot-directive-1.0.2/sphinx_plot_directive.egg-info/PKG-INFO
--rw-rw-r--   0 test1     (1000) test1     (1000)      307 2024-02-05 02:39:57.000000 sphinx-plot-directive-1.0.2/sphinx_plot_directive.egg-info/SOURCES.txt
--rw-rw-r--   0 test1     (1000) test1     (1000)        1 2024-02-05 02:39:57.000000 sphinx-plot-directive-1.0.2/sphinx_plot_directive.egg-info/dependency_links.txt
--rw-rw-r--   0 test1     (1000) test1     (1000)       16 2024-02-05 02:39:57.000000 sphinx-plot-directive-1.0.2/sphinx_plot_directive.egg-info/requires.txt
--rw-rw-r--   0 test1     (1000) test1     (1000)       22 2024-02-05 02:39:57.000000 sphinx-plot-directive-1.0.2/sphinx_plot_directive.egg-info/top_level.txt
+drwxrwxr-x   0 wind1     (1000) wind1     (1000)        0 2024-05-20 03:35:39.670230 sphinx-plot-directive-1.0.3/
+-rw-rw-r--   0 wind1     (1000) wind1     (1000)     1418 2024-01-31 03:06:42.000000 sphinx-plot-directive-1.0.3/LICENSE
+-rw-rw-r--   0 wind1     (1000) wind1     (1000)       51 2024-01-31 03:06:42.000000 sphinx-plot-directive-1.0.3/MANIFEST.in
+-rw-rw-r--   0 wind1     (1000) wind1     (1000)    15966 2024-05-20 03:35:39.670230 sphinx-plot-directive-1.0.3/PKG-INFO
+-rw-rw-r--   0 wind1     (1000) wind1     (1000)    15481 2024-05-20 03:35:20.000000 sphinx-plot-directive-1.0.3/README.rst
+-rw-rw-r--   0 wind1     (1000) wind1     (1000)       76 2024-05-20 03:35:39.670230 sphinx-plot-directive-1.0.3/setup.cfg
+-rw-rw-r--   0 wind1     (1000) wind1     (1000)      682 2024-05-16 06:24:57.000000 sphinx-plot-directive-1.0.3/setup.py
+drwxrwxr-x   0 wind1     (1000) wind1     (1000)        0 2024-05-20 03:35:39.670230 sphinx-plot-directive-1.0.3/sphinx_plot_directive/
+-rw-rw-r--   0 wind1     (1000) wind1     (1000)    26404 2024-05-16 06:24:57.000000 sphinx-plot-directive-1.0.3/sphinx_plot_directive/__init__.py
+drwxrwxr-x   0 wind1     (1000) wind1     (1000)        0 2024-05-20 03:35:39.670230 sphinx-plot-directive-1.0.3/sphinx_plot_directive.egg-info/
+-rw-rw-r--   0 wind1     (1000) wind1     (1000)    15966 2024-05-20 03:35:39.000000 sphinx-plot-directive-1.0.3/sphinx_plot_directive.egg-info/PKG-INFO
+-rw-rw-r--   0 wind1     (1000) wind1     (1000)      307 2024-05-20 03:35:39.000000 sphinx-plot-directive-1.0.3/sphinx_plot_directive.egg-info/SOURCES.txt
+-rw-rw-r--   0 wind1     (1000) wind1     (1000)        1 2024-05-20 03:35:39.000000 sphinx-plot-directive-1.0.3/sphinx_plot_directive.egg-info/dependency_links.txt
+-rw-rw-r--   0 wind1     (1000) wind1     (1000)       16 2024-05-20 03:35:39.000000 sphinx-plot-directive-1.0.3/sphinx_plot_directive.egg-info/requires.txt
+-rw-rw-r--   0 wind1     (1000) wind1     (1000)       22 2024-05-20 03:35:39.000000 sphinx-plot-directive-1.0.3/sphinx_plot_directive.egg-info/top_level.txt
```

### Comparing `sphinx-plot-directive-1.0.2/LICENSE` & `sphinx-plot-directive-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-plot-directive-1.0.2/PKG-INFO` & `sphinx-plot-directive-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-plot-directive
-Version: 1.0.2
+Version: 1.0.3
 Summary: "A .. plot::" directive for plotting figures in a Sphinx document.
 Home-page: https://github.com/guoyoooping/sphinx-plot-directive
 Author: Yongping Guo
 Author-email: guoyoooping@163.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -451,14 +451,19 @@
 .. |actdiag_example| image:: http://blockdiag.com/en/_images/actdiag-27aec367951ef70f7b5badceebbcc0c2bc687752.png
 .. |nwdiag_example| image:: http://blockdiag.com/en/_images/nwdiag-be3d31eeeacd641176a6f63703748e33d278419a.png
 
 6. Changelog
 ============
 
 1.0 Initial upload.
+1.0.3 Support inline image. For example, then you can use ::
+
+    |test1| inline.
+
+    |test1| plot:: convert palms.jpg -grayscale rec601luma out.jpg
 
 Refenreces
 ==========
 
 #. gnuplot, http://www.gnuplot.info/
 #. ditaa, https://github.com/tmthrgd/ditaa-ditaa
 #. Matplotlib, https://matplotlib.org/
```

### Comparing `sphinx-plot-directive-1.0.2/README.rst` & `sphinx-plot-directive-1.0.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -436,14 +436,19 @@
 .. |actdiag_example| image:: http://blockdiag.com/en/_images/actdiag-27aec367951ef70f7b5badceebbcc0c2bc687752.png
 .. |nwdiag_example| image:: http://blockdiag.com/en/_images/nwdiag-be3d31eeeacd641176a6f63703748e33d278419a.png
 
 6. Changelog
 ============
 
 1.0 Initial upload.
+1.0.3 Support inline image. For example, then you can use ::
+
+    |test1| inline.
+
+    |test1| plot:: convert palms.jpg -grayscale rec601luma out.jpg
 
 Refenreces
 ==========
 
 #. gnuplot, http://www.gnuplot.info/
 #. ditaa, https://github.com/tmthrgd/ditaa-ditaa
 #. Matplotlib, https://matplotlib.org/
```

### Comparing `sphinx-plot-directive-1.0.2/setup.py` & `sphinx-plot-directive-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='sphinx-plot-directive',
-    version='1.0.2',
+    version='1.0.3',
     description='"A .. plot::" directive for plotting figures in a Sphinx document.',
     long_description=open('README.rst').read(),
     url='https://github.com/guoyoooping/sphinx-plot-directive',
     author='Yongping Guo',
     author_email='guoyoooping@163.com',
     license='MIT',
     packages=['sphinx_plot_directive'],
```

### Comparing `sphinx-plot-directive-1.0.2/sphinx_plot_directive/__init__.py` & `sphinx-plot-directive-1.0.3/sphinx_plot_directive/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,20 +174,19 @@
 
     if app.builder.config.plot_log_level > 1:
         print("%s(), args: %s" %(sys._getframe().f_code.co_name, args))
     # 2) generate the output file
     try:
         print(' '.join(args))
         p = Popen(args, stdout=PIPE, stdin=PIPE, stderr=PIPE)
-        stdout, stderr = (p.stdout.read().decode("utf-8"),
-                p.stderr.read().decode("utf-8"))
+        stdout, stderr = (p.stdout.read(), p.stderr.read())
         if stdout:
-            print("[1;30m%s[0m" %(stdout))
+            print("[1;30m%s[0m" %(stdout.decode(errors='ignore')))
         if stderr:
-            print("[31m%s[0m" %(stderr))
+            print("[31m%s[0m" %(stderr.decode(errors='ignore')))
             if not path.isfile(out["outfullfn"]):
                 out["outrelfn"] = None
                 out["outfullfn"] = None
                 return out
     except OSError as err:
         os.chdir(currpath)
         print("[31mError in call: %s.[0m" %(args))
@@ -484,16 +483,17 @@
             out = cmd_2_image(app, img.plot)
             if options.get("hidden", False) or (not out["outfullfn"]):
                 #Don't render the image if there is hidden
                 nodes.image.pop(img)
                 continue
             img['uri'] = out["outrelfn"]
             if img.get('alt', None):
-                #For inline 用于类似这样的调用:.. |test1| plot:: convert
-                #palms.jpg -grayscale rec601luma out.jpg
+                #For inline image:
+                #    用于类似这样的调用:.. |test1| plot:: convert
+                #    palms.jpg -grayscale rec601luma out.jpg
                 uris[img['alt']] = img['uri']
                 if app.builder.config.plot_log_level > 0:
                     print("uris: %s" %(uris))
             if os.path.splitext(out["outfullfn"])[-1] in [".png",".jpg",".gif"] \
                     and path.isfile(out["outfullfn"]):
                 #对于png, jpg, gif 文件，手动获取它的大小
                 print("get size of: %s" %(out["outfullfn"]))
```

### Comparing `sphinx-plot-directive-1.0.2/sphinx_plot_directive.egg-info/PKG-INFO` & `sphinx-plot-directive-1.0.3/sphinx_plot_directive.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-plot-directive
-Version: 1.0.2
+Version: 1.0.3
 Summary: "A .. plot::" directive for plotting figures in a Sphinx document.
 Home-page: https://github.com/guoyoooping/sphinx-plot-directive
 Author: Yongping Guo
 Author-email: guoyoooping@163.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -451,14 +451,19 @@
 .. |actdiag_example| image:: http://blockdiag.com/en/_images/actdiag-27aec367951ef70f7b5badceebbcc0c2bc687752.png
 .. |nwdiag_example| image:: http://blockdiag.com/en/_images/nwdiag-be3d31eeeacd641176a6f63703748e33d278419a.png
 
 6. Changelog
 ============
 
 1.0 Initial upload.
+1.0.3 Support inline image. For example, then you can use ::
+
+    |test1| inline.
+
+    |test1| plot:: convert palms.jpg -grayscale rec601luma out.jpg
 
 Refenreces
 ==========
 
 #. gnuplot, http://www.gnuplot.info/
 #. ditaa, https://github.com/tmthrgd/ditaa-ditaa
 #. Matplotlib, https://matplotlib.org/
```

