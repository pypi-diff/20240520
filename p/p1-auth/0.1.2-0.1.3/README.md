# Comparing `tmp/p1_auth-0.1.2.tar.gz` & `tmp/p1_auth-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p1_auth-0.1.2.tar", last modified: Thu May 16 17:08:50 2024, max compression
+gzip compressed data, was "p1_auth-0.1.3.tar", last modified: Mon May 20 20:12:16 2024, max compression
```

## Comparing `p1_auth-0.1.2.tar` & `p1_auth-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2024-05-16 17:08:50.886457 p1_auth-0.1.2/
--rw-r--r--   0 jametobin   (502) staff       (20)     4458 2024-05-16 17:08:50.886330 p1_auth-0.1.2/PKG-INFO
--rw-r--r--   0 jametobin   (502) staff       (20)     3482 2024-05-15 15:17:01.000000 p1_auth-0.1.2/README.md
-drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2024-05-16 17:08:50.881663 p1_auth-0.1.2/p1_auth/
--rw-r--r--   0 jametobin   (502) staff       (20)        0 2024-05-15 15:17:01.000000 p1_auth-0.1.2/p1_auth/__init__.py
--rw-r--r--   0 jametobin   (502) staff       (20)      849 2024-05-15 15:17:01.000000 p1_auth-0.1.2/p1_auth/admin.py
--rw-r--r--   0 jametobin   (502) staff       (20)      145 2024-05-15 15:17:01.000000 p1_auth-0.1.2/p1_auth/apps.py
--rw-r--r--   0 jametobin   (502) staff       (20)     5708 2024-05-16 17:08:01.000000 p1_auth-0.1.2/p1_auth/backends.py
--rw-r--r--   0 jametobin   (502) staff       (20)      460 2024-05-15 15:17:01.000000 p1_auth-0.1.2/p1_auth/middleware.py
-drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2024-05-16 17:08:50.885279 p1_auth-0.1.2/p1_auth/migrations/
--rw-r--r--   0 jametobin   (502) staff       (20)     1250 2024-05-15 15:17:01.000000 p1_auth-0.1.2/p1_auth/migrations/0001_initial.py
--rw-r--r--   0 jametobin   (502) staff       (20)        0 2024-05-15 15:17:01.000000 p1_auth-0.1.2/p1_auth/migrations/__init__.py
--rw-r--r--   0 jametobin   (502) staff       (20)     3599 2024-05-15 15:17:01.000000 p1_auth-0.1.2/p1_auth/models.py
--rw-r--r--   0 jametobin   (502) staff       (20)       60 2024-05-15 15:17:01.000000 p1_auth-0.1.2/p1_auth/tests.py
--rw-r--r--   0 jametobin   (502) staff       (20)      613 2024-05-15 15:17:01.000000 p1_auth-0.1.2/p1_auth/views.py
-drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2024-05-16 17:08:50.885709 p1_auth-0.1.2/p1_auth.egg-info/
--rw-r--r--   0 jametobin   (502) staff       (20)     4458 2024-05-16 17:08:50.000000 p1_auth-0.1.2/p1_auth.egg-info/PKG-INFO
--rw-r--r--   0 jametobin   (502) staff       (20)      395 2024-05-16 17:08:50.000000 p1_auth-0.1.2/p1_auth.egg-info/SOURCES.txt
--rw-r--r--   0 jametobin   (502) staff       (20)        1 2024-05-16 17:08:50.000000 p1_auth-0.1.2/p1_auth.egg-info/dependency_links.txt
--rw-r--r--   0 jametobin   (502) staff       (20)       41 2024-05-16 17:08:50.000000 p1_auth-0.1.2/p1_auth.egg-info/requires.txt
--rw-r--r--   0 jametobin   (502) staff       (20)        8 2024-05-16 17:08:50.000000 p1_auth-0.1.2/p1_auth.egg-info/top_level.txt
--rw-r--r--   0 jametobin   (502) staff       (20)     1053 2024-05-16 17:08:50.886838 p1_auth-0.1.2/setup.cfg
--rw-r--r--   0 jametobin   (502) staff       (20)       95 2024-05-15 15:17:01.000000 p1_auth-0.1.2/setup.py
+drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2024-05-20 20:12:16.008617 p1_auth-0.1.3/
+-rw-r--r--   0 jametobin   (502) staff       (20)     5620 2024-05-20 20:12:16.008454 p1_auth-0.1.3/PKG-INFO
+-rw-r--r--   0 jametobin   (502) staff       (20)     4644 2024-05-20 20:11:59.000000 p1_auth-0.1.3/README.md
+drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2024-05-20 20:12:16.003877 p1_auth-0.1.3/p1_auth/
+-rw-r--r--   0 jametobin   (502) staff       (20)        0 2024-05-15 15:17:01.000000 p1_auth-0.1.3/p1_auth/__init__.py
+-rw-r--r--   0 jametobin   (502) staff       (20)      849 2024-05-15 15:17:01.000000 p1_auth-0.1.3/p1_auth/admin.py
+-rw-r--r--   0 jametobin   (502) staff       (20)      145 2024-05-15 15:17:01.000000 p1_auth-0.1.3/p1_auth/apps.py
+-rw-r--r--   0 jametobin   (502) staff       (20)     5708 2024-05-20 20:11:07.000000 p1_auth-0.1.3/p1_auth/backends.py
+-rw-r--r--   0 jametobin   (502) staff       (20)      460 2024-05-15 15:17:01.000000 p1_auth-0.1.3/p1_auth/middleware.py
+drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2024-05-20 20:12:16.007542 p1_auth-0.1.3/p1_auth/migrations/
+-rw-r--r--   0 jametobin   (502) staff       (20)     1250 2024-05-15 15:17:01.000000 p1_auth-0.1.3/p1_auth/migrations/0001_initial.py
+-rw-r--r--   0 jametobin   (502) staff       (20)        0 2024-05-15 15:17:01.000000 p1_auth-0.1.3/p1_auth/migrations/__init__.py
+-rw-r--r--   0 jametobin   (502) staff       (20)     3599 2024-05-15 15:17:01.000000 p1_auth-0.1.3/p1_auth/models.py
+-rw-r--r--   0 jametobin   (502) staff       (20)       60 2024-05-15 15:17:01.000000 p1_auth-0.1.3/p1_auth/tests.py
+-rw-r--r--   0 jametobin   (502) staff       (20)      613 2024-05-15 15:17:01.000000 p1_auth-0.1.3/p1_auth/views.py
+drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2024-05-20 20:12:16.007898 p1_auth-0.1.3/p1_auth.egg-info/
+-rw-r--r--   0 jametobin   (502) staff       (20)     5620 2024-05-20 20:12:15.000000 p1_auth-0.1.3/p1_auth.egg-info/PKG-INFO
+-rw-r--r--   0 jametobin   (502) staff       (20)      395 2024-05-20 20:12:15.000000 p1_auth-0.1.3/p1_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 jametobin   (502) staff       (20)        1 2024-05-20 20:12:15.000000 p1_auth-0.1.3/p1_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 jametobin   (502) staff       (20)       41 2024-05-20 20:12:15.000000 p1_auth-0.1.3/p1_auth.egg-info/requires.txt
+-rw-r--r--   0 jametobin   (502) staff       (20)        8 2024-05-20 20:12:15.000000 p1_auth-0.1.3/p1_auth.egg-info/top_level.txt
+-rw-r--r--   0 jametobin   (502) staff       (20)     1053 2024-05-20 20:12:16.009141 p1_auth-0.1.3/setup.cfg
+-rw-r--r--   0 jametobin   (502) staff       (20)       95 2024-05-15 15:17:01.000000 p1_auth-0.1.3/setup.py
```

### Comparing `p1_auth-0.1.2/PKG-INFO` & `p1_auth-0.1.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,68 @@
-Metadata-Version: 2.1
-Name: p1-auth
-Version: 0.1.2
-Summary: Installable Django Authentication that adds support for Platform One
-Home-page: https://github.com/OpenLXP/p1-auth/
-Author: OpenLXP
-Author-email: openlxphost@gmail.com
-License: MIT
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django :: 3.2
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Requires-Dist: PyJWT>=2.0.0
-Requires-Dist: djangorestframework>=3.13.0
-
 # p1-auth
 
 Provides an authentication system for Platform One by decoding non-encrypted JWTs.
 
+> [!CAUTION]
+> Signatures are not verified.
+
 Additionally provides configurations to automatically populate user attributes and assign user membership from JWT fields.
 
+## Installation
+
+After running `pip install p1-auth` add the following to the settings.py file as needed.
+
+```python
+INSTALLED_APPS = [
+    ...
+    'p1_auth',
+    ...
+]
+```
+
+Adding `p1_auth` to the `INSTALLED_APPS` is required for use.
+
+```python
+MIDDLEWARE = [
+    ...
+    'django.contrib.sessions.middleware.SessionMiddleware',
+    ...
+    'p1_auth.middleware.AuthenticateSessionMiddleware',
+    ...
+    'django.contrib.auth.middleware.AuthenticationMiddleware',
+    ...
+]
+```
+
+The `p1-auth` middleware can be used to force creation of sessions for use with django admin.  If it is used, it should be between django `SessionMiddleware` and `AuthenticationMiddleware` as shown above.
+
+```python
+AUTHENTICATION_BACKENDS = (
+    ...
+    'p1_auth.backends.PlatformOneAuthentication',
+    ...
+)
+```
+
+`PlatformOneAuthentication` authenticates django requests.
+
+```python
+REST_FRAMEWORK = {
+    ...
+    'DEFAULT_AUTHENTICATION_CLASSES': [
+        ...
+        'p1_auth.backends.PlatformOneRestAuthentication',
+        ...
+    ],
+    ...
+}
+```
+
+`PlatformOneRestAuthentication` authenticates django-rest-framework requests.
+
 ## settings.py
 
 This section covers configurations that can be set in the settings.py file.
 
 ### USER_ATTRIBUTES_MAP
 
 A python dictionary to map between fields on the User model and the JWT fields.
@@ -118,8 +149,8 @@
 
 ### AttributeCheck
 
 AttributeCheck allows specifying the JWT key (jwt_attribute) and an expected value.
 
 Jwt_attribute should be a valid JSON key, or a JSON object for traversing the JWT to where the key will be.
 
-Expected_value is the expected JSON value.
+Expected_value is the expected JSON value.
```

### Comparing `p1_auth-0.1.2/p1_auth/admin.py` & `p1_auth-0.1.3/p1_auth/admin.py`

 * *Files identical despite different names*

### Comparing `p1_auth-0.1.2/p1_auth/backends.py` & `p1_auth-0.1.3/p1_auth/backends.py`

 * *Files identical despite different names*

### Comparing `p1_auth-0.1.2/p1_auth/migrations/0001_initial.py` & `p1_auth-0.1.3/p1_auth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `p1_auth-0.1.2/p1_auth/models.py` & `p1_auth-0.1.3/p1_auth/models.py`

 * *Files identical despite different names*

### Comparing `p1_auth-0.1.2/p1_auth/views.py` & `p1_auth-0.1.3/p1_auth/views.py`

 * *Files identical despite different names*

### Comparing `p1_auth-0.1.2/p1_auth.egg-info/PKG-INFO` & `p1_auth-0.1.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p1-auth
-Version: 0.1.2
+Version: 0.1.3
 Summary: Installable Django Authentication that adds support for Platform One
 Home-page: https://github.com/OpenLXP/p1-auth/
 Author: OpenLXP
 Author-email: openlxphost@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -22,16 +22,71 @@
 Requires-Dist: PyJWT>=2.0.0
 Requires-Dist: djangorestframework>=3.13.0
 
 # p1-auth
 
 Provides an authentication system for Platform One by decoding non-encrypted JWTs.
 
+> [!CAUTION]
+> Signatures are not verified.
+
 Additionally provides configurations to automatically populate user attributes and assign user membership from JWT fields.
 
+## Installation
+
+After running `pip install p1-auth` add the following to the settings.py file as needed.
+
+```python
+INSTALLED_APPS = [
+    ...
+    'p1_auth',
+    ...
+]
+```
+
+Adding `p1_auth` to the `INSTALLED_APPS` is required for use.
+
+```python
+MIDDLEWARE = [
+    ...
+    'django.contrib.sessions.middleware.SessionMiddleware',
+    ...
+    'p1_auth.middleware.AuthenticateSessionMiddleware',
+    ...
+    'django.contrib.auth.middleware.AuthenticationMiddleware',
+    ...
+]
+```
+
+The `p1-auth` middleware can be used to force creation of sessions for use with django admin.  If it is used, it should be between django `SessionMiddleware` and `AuthenticationMiddleware` as shown above.
+
+```python
+AUTHENTICATION_BACKENDS = (
+    ...
+    'p1_auth.backends.PlatformOneAuthentication',
+    ...
+)
+```
+
+`PlatformOneAuthentication` authenticates django requests.
+
+```python
+REST_FRAMEWORK = {
+    ...
+    'DEFAULT_AUTHENTICATION_CLASSES': [
+        ...
+        'p1_auth.backends.PlatformOneRestAuthentication',
+        ...
+    ],
+    ...
+}
+```
+
+`PlatformOneRestAuthentication` authenticates django-rest-framework requests.
+
 ## settings.py
 
 This section covers configurations that can be set in the settings.py file.
 
 ### USER_ATTRIBUTES_MAP
 
 A python dictionary to map between fields on the User model and the JWT fields.
```

### Comparing `p1_auth-0.1.2/setup.cfg` & `p1_auth-0.1.3/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = p1-auth
-version = 0.1.2
+version = 0.1.3
 description = Installable Django Authentication that adds support for Platform One
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/OpenLXP/p1-auth/
 author = OpenLXP
 author_email = openlxphost@gmail.com
 license = MIT
```

