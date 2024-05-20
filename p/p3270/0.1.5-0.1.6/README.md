# Comparing `tmp/p3270-0.1.5.tar.gz` & `tmp/p3270-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p3270-0.1.5.tar", last modified: Thu Apr  6 05:23:57 2023, max compression
+gzip compressed data, was "p3270-0.1.6.tar", last modified: Mon May 20 17:42:22 2024, max compression
```

## Comparing `p3270-0.1.5.tar` & `p3270-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mstiri     (501) staff       (20)        0 2023-04-06 05:23:57.974757 p3270-0.1.5/
--rw-r--r--   0 mstiri     (501) staff       (20)    35147 2021-01-12 20:07:40.000000 p3270-0.1.5/LICENSE.txt
--rw-r--r--   0 mstiri     (501) staff       (20)       54 2021-01-12 20:07:40.000000 p3270-0.1.5/MANIFEST.in
--rw-r--r--   0 mstiri     (501) staff       (20)     1465 2023-04-06 05:23:57.974129 p3270-0.1.5/PKG-INFO
--rw-r--r--   0 mstiri     (501) staff       (20)    11324 2022-08-08 14:52:47.000000 p3270-0.1.5/README.md
-drwxr-xr-x   0 mstiri     (501) staff       (20)        0 2023-04-06 05:23:57.969685 p3270-0.1.5/p3270/
--rw-r--r--   0 mstiri     (501) staff       (20)       66 2021-01-12 20:07:40.000000 p3270-0.1.5/p3270/__init__.py
--rw-r--r--   0 mstiri     (501) staff       (20)      556 2021-01-12 20:07:40.000000 p3270-0.1.5/p3270/p3270.cfg
--rw-r--r--   0 mstiri     (501) staff       (20)    32185 2023-04-06 05:04:10.000000 p3270-0.1.5/p3270/p3270.py
-drwxr-xr-x   0 mstiri     (501) staff       (20)        0 2023-04-06 05:23:57.973301 p3270-0.1.5/p3270.egg-info/
--rw-r--r--   0 mstiri     (501) staff       (20)     1465 2023-04-06 05:23:57.000000 p3270-0.1.5/p3270.egg-info/PKG-INFO
--rw-r--r--   0 mstiri     (501) staff       (20)      207 2023-04-06 05:23:57.000000 p3270-0.1.5/p3270.egg-info/SOURCES.txt
--rw-r--r--   0 mstiri     (501) staff       (20)        1 2023-04-06 05:23:57.000000 p3270-0.1.5/p3270.egg-info/dependency_links.txt
--rw-r--r--   0 mstiri     (501) staff       (20)        6 2023-04-06 05:23:57.000000 p3270-0.1.5/p3270.egg-info/top_level.txt
--rw-r--r--   0 mstiri     (501) staff       (20)       38 2023-04-06 05:23:57.974886 p3270-0.1.5/setup.cfg
--rw-r--r--   0 mstiri     (501) staff       (20)     1594 2023-04-06 05:11:36.000000 p3270-0.1.5/setup.py
+drwxr-xr-x   0 mstiri     (501) staff       (20)        0 2024-05-20 17:42:22.786599 p3270-0.1.6/
+-rw-r--r--   0 mstiri     (501) staff       (20)    35147 2021-01-12 20:07:40.000000 p3270-0.1.6/LICENSE.txt
+-rw-r--r--   0 mstiri     (501) staff       (20)       54 2021-01-12 20:07:40.000000 p3270-0.1.6/MANIFEST.in
+-rw-r--r--   0 mstiri     (501) staff       (20)     1465 2024-05-20 17:42:22.785632 p3270-0.1.6/PKG-INFO
+-rw-r--r--   0 mstiri     (501) staff       (20)    11324 2022-08-08 14:52:47.000000 p3270-0.1.6/README.md
+drwxr-xr-x   0 mstiri     (501) staff       (20)        0 2024-05-20 17:42:22.782130 p3270-0.1.6/p3270/
+-rw-r--r--   0 mstiri     (501) staff       (20)       66 2021-01-12 20:07:40.000000 p3270-0.1.6/p3270/__init__.py
+-rw-r--r--   0 mstiri     (501) staff       (20)      556 2021-01-12 20:07:40.000000 p3270-0.1.6/p3270/p3270.cfg
+-rw-r--r--   0 mstiri     (501) staff       (20)    32334 2024-05-20 17:28:41.000000 p3270-0.1.6/p3270/p3270.py
+drwxr-xr-x   0 mstiri     (501) staff       (20)        0 2024-05-20 17:42:22.784905 p3270-0.1.6/p3270.egg-info/
+-rw-r--r--   0 mstiri     (501) staff       (20)     1465 2024-05-20 17:42:22.000000 p3270-0.1.6/p3270.egg-info/PKG-INFO
+-rw-r--r--   0 mstiri     (501) staff       (20)      207 2024-05-20 17:42:22.000000 p3270-0.1.6/p3270.egg-info/SOURCES.txt
+-rw-r--r--   0 mstiri     (501) staff       (20)        1 2024-05-20 17:42:22.000000 p3270-0.1.6/p3270.egg-info/dependency_links.txt
+-rw-r--r--   0 mstiri     (501) staff       (20)        6 2024-05-20 17:42:22.000000 p3270-0.1.6/p3270.egg-info/top_level.txt
+-rw-r--r--   0 mstiri     (501) staff       (20)       38 2024-05-20 17:42:22.786793 p3270-0.1.6/setup.cfg
+-rw-r--r--   0 mstiri     (501) staff       (20)     1594 2024-05-20 17:31:28.000000 p3270-0.1.6/setup.py
```

### Comparing `p3270-0.1.5/LICENSE.txt` & `p3270-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `p3270-0.1.5/PKG-INFO` & `p3270-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p3270
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python library to communicate with IBM hosts
 Home-page: https://github.com/mstiri/p3270
 Author: Mossaab Stiri
 Author-email: mossaab.stiri@gmail.com
 Keywords: IBM CICS 3270 TN3270 test automation Mainframe z/OS
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
```

### Comparing `p3270-0.1.5/README.md` & `p3270-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `p3270-0.1.5/p3270/p3270.cfg` & `p3270-0.1.6/p3270/p3270.cfg`

 * *Files identical despite different names*

### Comparing `p3270-0.1.5/p3270/p3270.py` & `p3270-0.1.6/p3270/p3270.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         self.modelName = modelName
         self.configFile = configFile
         self.verifyCert = verifyCert
         self.enableTLS = enableTLS
         self.timeout = timeoutInSec
         self.path = path
         self.conf = Config(cfgFile=self.configFile, hostName=self.hostName,
-                           hostPort=self.hostPort, luName=self.luName, modelName=self.modelName, codePage=codePage)
+                           hostPort=self.hostPort, luName=self.luName, modelName=self.modelName, codePage=codePage, enableTLS = self.enableTLS)
         if self.conf.isValid():
             self.subpro = None
             self.makeArgs()
             self.s3270 = S3270(self.args, self.conf.encoding)
         else:
             raise InvalidConfiguration
         self._isValid = self.conf.isValid()
@@ -296,18 +296,18 @@
 
     def moveToFirstInputField(self):
         """ Move cursor to the first input field.
         """
         logger.info("Move cursor to the first input field")
         return self.s3270.do('Home')
 
-    def sendText(self, text):
-        """ Send text to host.
+    def sendText(self, text, asterisks=False):
+        """ Send text to host. Possible to hide value (asterisk it) in log by set asterisks to True.
         """
-        logger.info("Send the following text: [{}]".format(text))
+        logger.info("Send the following text: [{}]".format('*' * len(text) if asterisks else text))
         return self.s3270.do('String("{}")'.format(text))
 
     def saveScreen(self, fileName='screen', dataType='html'):
         """ Save the current screen in the form of an HTML file.
             Other types supported: rtf,txt
         """
         if fileName and self.conf.screensDir:
```

### Comparing `p3270-0.1.5/p3270.egg-info/PKG-INFO` & `p3270-0.1.6/p3270.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p3270
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python library to communicate with IBM hosts
 Home-page: https://github.com/mstiri/p3270
 Author: Mossaab Stiri
 Author-email: mossaab.stiri@gmail.com
 Keywords: IBM CICS 3270 TN3270 test automation Mainframe z/OS
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
```

### Comparing `p3270-0.1.5/setup.py` & `p3270-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #from distutils.core import setup
 import setuptools
 
 setuptools.setup(
     name='p3270',
     packages=['p3270'],
-    version='0.1.5',
+    version='0.1.6',
     description='Python library to communicate with IBM hosts',
     author='Mossaab Stiri',
     author_email='mossaab.stiri@gmail.com',
     url='https://github.com/mstiri/p3270',
     long_description='''
     A Python library that provides an interface to communicate with IBM hosts: send commands and text, receive output (screens). The library provides the means to do what a human can do using a 3270 emulator.
```

