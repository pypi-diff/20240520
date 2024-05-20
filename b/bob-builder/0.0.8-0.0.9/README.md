# Comparing `tmp/bob-builder-0.0.8.tar.gz` & `tmp/bob-builder-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bob-builder-0.0.8.tar", last modified: Tue Feb 16 21:29:22 2016, max compression
+gzip compressed data, was "dist/bob-builder-0.0.9.tar", last modified: Wed Feb 17 05:18:25 2016, max compression
```

## Comparing `bob-builder-0.0.8.tar` & `bob-builder-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 kreitz     (501) staff       (20)        0 2016-02-16 21:29:22.000000 bob-builder-0.0.8/
-drwxr-xr-x   0 kreitz     (501) staff       (20)        0 2016-02-16 21:29:22.000000 bob-builder-0.0.8/bob/
--rw-r--r--   0 kreitz     (501) staff       (20)       18 2016-02-05 19:35:57.000000 bob-builder-0.0.8/bob/__init__.py
--rw-r--r--   0 kreitz     (501) staff       (20)     1260 2016-02-05 19:35:57.000000 bob-builder-0.0.8/bob/cli.py
--rw-r--r--   0 kreitz     (501) staff       (20)     4486 2016-02-16 21:28:41.000000 bob-builder-0.0.8/bob/models.py
--rw-r--r--   0 kreitz     (501) staff       (20)     1445 2016-02-16 21:28:41.000000 bob-builder-0.0.8/bob/utils.py
-drwxr-xr-x   0 kreitz     (501) staff       (20)        0 2016-02-16 21:29:22.000000 bob-builder-0.0.8/bob_builder.egg-info/
--rw-r--r--   0 kreitz     (501) staff       (20)        1 2016-02-16 21:29:22.000000 bob-builder-0.0.8/bob_builder.egg-info/dependency_links.txt
--rw-r--r--   0 kreitz     (501) staff       (20)       42 2016-02-16 21:29:22.000000 bob-builder-0.0.8/bob_builder.egg-info/entry_points.txt
--rw-r--r--   0 kreitz     (501) staff       (20)       47 2016-02-16 21:29:22.000000 bob-builder-0.0.8/bob_builder.egg-info/pbr.json
--rw-r--r--   0 kreitz     (501) staff       (20)      244 2016-02-16 21:29:22.000000 bob-builder-0.0.8/bob_builder.egg-info/PKG-INFO
--rw-r--r--   0 kreitz     (501) staff       (20)       18 2016-02-16 21:29:22.000000 bob-builder-0.0.8/bob_builder.egg-info/requires.txt
--rw-r--r--   0 kreitz     (501) staff       (20)      304 2016-02-16 21:29:22.000000 bob-builder-0.0.8/bob_builder.egg-info/SOURCES.txt
--rw-r--r--   0 kreitz     (501) staff       (20)        4 2016-02-16 21:29:22.000000 bob-builder-0.0.8/bob_builder.egg-info/top_level.txt
--rw-r--r--   0 kreitz     (501) staff       (20)      244 2016-02-16 21:29:22.000000 bob-builder-0.0.8/PKG-INFO
--rw-r--r--   0 kreitz     (501) staff       (20)       59 2016-02-16 21:29:22.000000 bob-builder-0.0.8/setup.cfg
--rwxr-xr-x   0 kreitz     (501) staff       (20)      566 2016-02-16 21:28:41.000000 bob-builder-0.0.8/setup.py
+drwxr-xr-x   0 kreitz     (501) staff       (20)        0 2016-02-17 05:18:25.000000 bob-builder-0.0.9/
+drwxr-xr-x   0 kreitz     (501) staff       (20)        0 2016-02-17 05:18:25.000000 bob-builder-0.0.9/bob/
+-rw-r--r--   0 kreitz     (501) staff       (20)       18 2016-02-05 19:35:57.000000 bob-builder-0.0.9/bob/__init__.py
+-rw-r--r--   0 kreitz     (501) staff       (20)     1297 2016-02-17 05:16:53.000000 bob-builder-0.0.9/bob/cli.py
+-rw-r--r--   0 kreitz     (501) staff       (20)     4498 2016-02-17 05:16:53.000000 bob-builder-0.0.9/bob/models.py
+-rw-r--r--   0 kreitz     (501) staff       (20)     1445 2016-02-16 21:28:41.000000 bob-builder-0.0.9/bob/utils.py
+drwxr-xr-x   0 kreitz     (501) staff       (20)        0 2016-02-17 05:18:25.000000 bob-builder-0.0.9/bob_builder.egg-info/
+-rw-r--r--   0 kreitz     (501) staff       (20)        1 2016-02-17 05:18:25.000000 bob-builder-0.0.9/bob_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 kreitz     (501) staff       (20)       42 2016-02-17 05:18:25.000000 bob-builder-0.0.9/bob_builder.egg-info/entry_points.txt
+-rw-r--r--   0 kreitz     (501) staff       (20)       47 2016-02-17 05:18:25.000000 bob-builder-0.0.9/bob_builder.egg-info/pbr.json
+-rw-r--r--   0 kreitz     (501) staff       (20)      244 2016-02-17 05:18:25.000000 bob-builder-0.0.9/bob_builder.egg-info/PKG-INFO
+-rw-r--r--   0 kreitz     (501) staff       (20)       18 2016-02-17 05:18:25.000000 bob-builder-0.0.9/bob_builder.egg-info/requires.txt
+-rw-r--r--   0 kreitz     (501) staff       (20)      304 2016-02-17 05:18:25.000000 bob-builder-0.0.9/bob_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 kreitz     (501) staff       (20)        4 2016-02-17 05:18:25.000000 bob-builder-0.0.9/bob_builder.egg-info/top_level.txt
+-rw-r--r--   0 kreitz     (501) staff       (20)      244 2016-02-17 05:18:25.000000 bob-builder-0.0.9/PKG-INFO
+-rw-r--r--   0 kreitz     (501) staff       (20)       59 2016-02-17 05:18:25.000000 bob-builder-0.0.9/setup.cfg
+-rwxr-xr-x   0 kreitz     (501) staff       (20)      566 2016-02-17 05:17:05.000000 bob-builder-0.0.9/setup.py
```

### Comparing `bob-builder-0.0.8/bob/cli.py` & `bob-builder-0.0.9/bob/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,29 +9,30 @@
     -h --help
     --overwrite  allow overwriting of deployed archives.
 
 Configuration:
     Environment Variables: AWS_ACCESS_KEY_ID, AWS_SECRET_ACCESS_KEY, S3_BUCKET, S3_PREFIX (optional)
 """
 import os
+import sys
 
 from docopt import docopt
 from .models import Formula
 
 
 
 def build(formula):
 
     f = Formula(path=formula)
 
     try:
         assert f.exists
     except AssertionError:
         print 'Formula {} doesn\'t appear to exist.'.format(formula)
-        exit(1)
+        sys.exit(1)
 
     # CLI lies ahead.
     f.build()
 
     return f
 
     # Tarball
@@ -68,7 +69,8 @@
 
 
 def dispatch():
     try:
         main()
     except KeyboardInterrupt:
         print 'ool.'
+        sys.exit(130)
```

### Comparing `bob-builder-0.0.8/bob/models.py` & `bob-builder-0.0.9/bob/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -95,15 +95,15 @@
                 key_name = '{}{}.tar.gz'.format(S3_PREFIX, dep)
                 key = bucket.get_key(key_name)
 
                 if not key:
                     print
                     print 'ERROR: Archive {} does not exist.'.format(key_name)
                     print '    Please deploy it to continue.'
-                    exit(1)
+                    sys.exit(1)
 
                 # Grab the Dep from S3, download it to a temp file.
                 archive = mkstemp()[1]
                 key.get_contents_to_filename(archive)
 
                 # Extract the Dep to the appropriate location.
                 extract_tree(archive, self.build_path)
@@ -125,15 +125,15 @@
 
         pipe(p.stdout, sys.stdout, indent=True)
         p.wait()
 
         if p.returncode != 0:
             print
             print 'ERROR: An error occurred.'
-            exit(1)
+            sys.exit(1)
 
 
     def archive(self):
         """Archives the build directory as a tar.gz."""
         archive = mkstemp()[1]
         archive_tree(self.build_path, archive)
 
@@ -148,14 +148,14 @@
         key_name = '{}{}.tar.gz'.format(S3_PREFIX, self.path)
         key = bucket.get_key(key_name)
 
         if key:
             if not allow_overwrite:
                 print 'ERROR: Archive {} already exists.'.format(key_name)
                 print '    Use the --overwrite flag to continue.'
-                exit(1)
+                sys.exit(1)
         else:
             key = bucket.new_key(key_name)
 
         # Upload the archive, set permissions.
         key.set_contents_from_filename(self.archived_path)
         key.set_acl('public-read')
```

### Comparing `bob-builder-0.0.8/bob/utils.py` & `bob-builder-0.0.9/bob/utils.py`

 * *Files identical despite different names*

### Comparing `bob-builder-0.0.8/setup.py` & `bob-builder-0.0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     'boto',
     'docopt',
     'envoy'
 ]
 
 setup(
     name='bob-builder',
-    version='0.0.8',
+    version='0.0.9',
     install_requires=deps,
     description='Binary Build Toolkit.',
     # long_description='Meh.',/
     author='Kenneth Reitz',
     author_email='kenneth@heroku.com',
     url='https://github.com/heroku/build-toolkit',
     packages=['bob'],
```

