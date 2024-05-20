# Comparing `tmp/django_superapp-1.0.0.tar.gz` & `tmp/django_superapp-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_superapp-1.0.0.tar", last modified: Mon May 20 08:21:16 2024, max compression
+gzip compressed data, was "django_superapp-1.0.4.tar", last modified: Mon May 20 09:03:26 2024, max compression
```

## Comparing `django_superapp-1.0.0.tar` & `django_superapp-1.0.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 iosif      (501) staff       (20)        0 2024-05-20 08:21:16.973188 django_superapp-1.0.0/
--rw-r--r--   0 iosif      (501) staff       (20)      372 2024-05-20 08:21:16.973117 django_superapp-1.0.0/PKG-INFO
--rw-r--r--   0 iosif      (501) staff       (20)       91 2024-05-20 07:48:56.000000 django_superapp-1.0.0/README.md
--rw-rw-r--   0 iosif      (501) staff       (20)       50 2023-10-23 03:11:54.000000 django_superapp-1.0.0/pyproject.toml
--rw-rw-r--   0 iosif      (501) staff       (20)      259 2024-05-20 08:21:16.973478 django_superapp-1.0.0/setup.cfg
--rw-rw-r--   0 iosif      (501) staff       (20)      392 2024-05-20 07:55:51.000000 django_superapp-1.0.0/setup.py
-drwxr-xr-x   0 iosif      (501) staff       (20)        0 2024-05-20 08:21:16.966100 django_superapp-1.0.0/src/
-drwxr-xr-x   0 iosif      (501) staff       (20)        0 2024-05-20 08:21:16.970263 django_superapp-1.0.0/src/django_superapp/
--rw-rw-r--   0 iosif      (501) staff       (20)        0 2024-05-17 09:42:40.000000 django_superapp-1.0.0/src/django_superapp/__init__.py
--rwxr-xr-x   0 iosif      (501) staff       (20)      118 2024-05-16 14:27:33.000000 django_superapp-1.0.0/src/django_superapp/apps.py
--rw-r--r--   0 iosif      (501) staff       (20)      685 2024-05-17 13:32:06.000000 django_superapp-1.0.0/src/django_superapp/autocomplete.py
--rw-r--r--   0 iosif      (501) staff       (20)      384 2024-05-17 13:32:06.000000 django_superapp-1.0.0/src/django_superapp/db_fields.py
--rw-r--r--   0 iosif      (501) staff       (20)     2093 2024-04-17 08:02:01.000000 django_superapp-1.0.0/src/django_superapp/decorators.py
--rwxr-xr-x   0 iosif      (501) staff       (20)      826 2024-05-17 12:43:02.000000 django_superapp-1.0.0/src/django_superapp/forms.py
--rw-r--r--   0 iosif      (501) staff       (20)     6254 2024-05-20 07:34:45.000000 django_superapp-1.0.0/src/django_superapp/helpers.py
-drwxr-xr-x   0 iosif      (501) staff       (20)        0 2024-05-20 08:21:16.971207 django_superapp-1.0.0/src/django_superapp/management/
--rw-r--r--   0 iosif      (501) staff       (20)        0 2024-04-17 08:02:01.000000 django_superapp-1.0.0/src/django_superapp/management/__init__.py
-drwxr-xr-x   0 iosif      (501) staff       (20)        0 2024-05-20 08:21:16.972086 django_superapp-1.0.0/src/django_superapp/management/commands/
--rw-r--r--   0 iosif      (501) staff       (20)        0 2024-04-17 08:02:01.000000 django_superapp-1.0.0/src/django_superapp/management/commands/__init__.py
--rw-r--r--   0 iosif      (501) staff       (20)      486 2024-04-17 08:02:01.000000 django_superapp-1.0.0/src/django_superapp/management/commands/list_all_permissions.py
--rw-r--r--   0 iosif      (501) staff       (20)      764 2024-04-17 08:02:01.000000 django_superapp-1.0.0/src/django_superapp/management/commands/list_all_urls_patterns.py
--rw-r--r--   0 iosif      (501) staff       (20)      584 2024-04-19 10:45:19.000000 django_superapp-1.0.0/src/django_superapp/management/commands/truncate_all_models.py
-drwxr-xr-x   0 iosif      (501) staff       (20)        0 2024-05-20 08:21:16.972606 django_superapp-1.0.0/src/django_superapp/migrations/
--rw-r--r--   0 iosif      (501) staff       (20)        0 2024-04-17 08:02:01.000000 django_superapp-1.0.0/src/django_superapp/migrations/__init__.py
--rw-r--r--   0 iosif      (501) staff       (20)     1663 2024-05-17 14:38:37.000000 django_superapp-1.0.0/src/django_superapp/settings.py
--rwxr-xr-x   0 iosif      (501) staff       (20)     1267 2024-05-17 12:25:23.000000 django_superapp-1.0.0/src/django_superapp/sites.py
--rwxr-xr-x   0 iosif      (501) staff       (20)     1443 2024-05-20 07:34:45.000000 django_superapp-1.0.0/src/django_superapp/urls.py
--rw-r--r--   0 iosif      (501) staff       (20)     2517 2024-05-17 13:36:11.000000 django_superapp-1.0.0/src/django_superapp/widgets.py
-drwxr-xr-x   0 iosif      (501) staff       (20)        0 2024-05-20 08:21:16.972796 django_superapp-1.0.0/src/django_superapp.egg-info/
--rw-r--r--   0 iosif      (501) staff       (20)      372 2024-05-20 08:21:16.000000 django_superapp-1.0.0/src/django_superapp.egg-info/PKG-INFO
--rw-r--r--   0 iosif      (501) staff       (20)      931 2024-05-20 08:21:16.000000 django_superapp-1.0.0/src/django_superapp.egg-info/SOURCES.txt
--rw-r--r--   0 iosif      (501) staff       (20)        1 2024-05-20 08:21:16.000000 django_superapp-1.0.0/src/django_superapp.egg-info/dependency_links.txt
--rw-r--r--   0 iosif      (501) staff       (20)      124 2024-05-20 08:21:16.000000 django_superapp-1.0.0/src/django_superapp.egg-info/requires.txt
--rw-r--r--   0 iosif      (501) staff       (20)       16 2024-05-20 08:21:16.000000 django_superapp-1.0.0/src/django_superapp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:03:26.420712 django_superapp-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-20 09:03:26.420712 django_superapp-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-20 09:03:08.000000 django_superapp-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-20 09:03:08.000000 django_superapp-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-20 09:03:26.420712 django_superapp-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-20 09:03:08.000000 django_superapp-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:03:26.412712 django_superapp-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:03:26.416712 django_superapp-1.0.4/src/django_superapp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 09:03:08.000000 django_superapp-1.0.4/src/django_superapp/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      118 2024-05-20 09:03:08.000000 django_superapp-1.0.4/src/django_superapp/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-20 09:03:08.000000 django_superapp-1.0.4/src/django_superapp/autocomplete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-20 09:03:08.000000 django_superapp-1.0.4/src/django_superapp/db_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-20 09:03:08.000000 django_superapp-1.0.4/src/django_superapp/decorators.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      826 2024-05-20 09:03:08.000000 django_superapp-1.0.4/src/django_superapp/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-05-20 09:03:08.000000 django_superapp-1.0.4/src/django_superapp/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:03:26.416712 django_superapp-1.0.4/src/django_superapp/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 09:03:08.000000 django_superapp-1.0.4/src/django_superapp/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:03:26.420712 django_superapp-1.0.4/src/django_superapp/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 09:03:08.000000 django_superapp-1.0.4/src/django_superapp/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-20 09:03:08.000000 django_superapp-1.0.4/src/django_superapp/management/commands/list_all_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-20 09:03:08.000000 django_superapp-1.0.4/src/django_superapp/management/commands/list_all_urls_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-20 09:03:08.000000 django_superapp-1.0.4/src/django_superapp/management/commands/truncate_all_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:03:26.420712 django_superapp-1.0.4/src/django_superapp/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 09:03:08.000000 django_superapp-1.0.4/src/django_superapp/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-20 09:03:08.000000 django_superapp-1.0.4/src/django_superapp/settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1267 2024-05-20 09:03:08.000000 django_superapp-1.0.4/src/django_superapp/sites.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1443 2024-05-20 09:03:08.000000 django_superapp-1.0.4/src/django_superapp/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-20 09:03:08.000000 django_superapp-1.0.4/src/django_superapp/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:03:26.420712 django_superapp-1.0.4/src/django_superapp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-20 09:03:26.000000 django_superapp-1.0.4/src/django_superapp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-20 09:03:26.000000 django_superapp-1.0.4/src/django_superapp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 09:03:26.000000 django_superapp-1.0.4/src/django_superapp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-20 09:03:26.000000 django_superapp-1.0.4/src/django_superapp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-20 09:03:26.000000 django_superapp-1.0.4/src/django_superapp.egg-info/top_level.txt
```

### Comparing `django_superapp-1.0.0/src/django_superapp/autocomplete.py` & `django_superapp-1.0.4/src/django_superapp/autocomplete.py`

 * *Files identical despite different names*

### Comparing `django_superapp-1.0.0/src/django_superapp/decorators.py` & `django_superapp-1.0.4/src/django_superapp/decorators.py`

 * *Files identical despite different names*

### Comparing `django_superapp-1.0.0/src/django_superapp/forms.py` & `django_superapp-1.0.4/src/django_superapp/forms.py`

 * *Files identical despite different names*

### Comparing `django_superapp-1.0.0/src/django_superapp/helpers.py` & `django_superapp-1.0.4/src/django_superapp/helpers.py`

 * *Files identical despite different names*

### Comparing `django_superapp-1.0.0/src/django_superapp/management/commands/list_all_urls_patterns.py` & `django_superapp-1.0.4/src/django_superapp/management/commands/list_all_urls_patterns.py`

 * *Files identical despite different names*

### Comparing `django_superapp-1.0.0/src/django_superapp/management/commands/truncate_all_models.py` & `django_superapp-1.0.4/src/django_superapp/management/commands/truncate_all_models.py`

 * *Files identical despite different names*

### Comparing `django_superapp-1.0.0/src/django_superapp/settings.py` & `django_superapp-1.0.4/src/django_superapp/settings.py`

 * *Files identical despite different names*

### Comparing `django_superapp-1.0.0/src/django_superapp/sites.py` & `django_superapp-1.0.4/src/django_superapp/sites.py`

 * *Files identical despite different names*

### Comparing `django_superapp-1.0.0/src/django_superapp/urls.py` & `django_superapp-1.0.4/src/django_superapp/urls.py`

 * *Files identical despite different names*

### Comparing `django_superapp-1.0.0/src/django_superapp/widgets.py` & `django_superapp-1.0.4/src/django_superapp/widgets.py`

 * *Files identical despite different names*

### Comparing `django_superapp-1.0.0/src/django_superapp.egg-info/SOURCES.txt` & `django_superapp-1.0.4/src/django_superapp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

