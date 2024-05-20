# Comparing `tmp/url_remote-0.0.94.tar.gz` & `tmp/url_remote-0.0.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "url_remote-0.0.94.tar", last modified: Thu May 16 23:54:54 2024, max compression
+gzip compressed data, was "url_remote-0.0.95.tar", last modified: Mon May 20 17:08:01 2024, max compression
```

## Comparing `url_remote-0.0.94.tar` & `url_remote-0.0.95.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 23:54:54.736615 url_remote-0.0.94/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-16 23:54:54.736615 url_remote-0.0.94/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-16 23:54:46.000000 url_remote-0.0.94/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-16 23:54:46.000000 url_remote-0.0.94/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 23:54:54.736615 url_remote-0.0.94/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-16 23:54:46.000000 url_remote-0.0.94/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 23:54:54.732615 url_remote-0.0.94/url_remote/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 23:54:54.736615 url_remote-0.0.94/url_remote/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 23:54:46.000000 url_remote-0.0.94/url_remote/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-16 23:54:46.000000 url_remote-0.0.94/url_remote/src/action_name_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-16 23:54:46.000000 url_remote-0.0.94/url_remote/src/api_version_dicts.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-16 23:54:46.000000 url_remote-0.0.94/url_remote/src/authentiction_api_version_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-16 23:54:46.000000 url_remote-0.0.94/url_remote/src/brand_name_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-16 23:54:46.000000 url_remote-0.0.94/url_remote/src/component_name_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-16 23:54:46.000000 url_remote-0.0.94/url_remote/src/entity_name_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-16 23:54:46.000000 url_remote-0.0.94/url_remote/src/environment_name_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     9051 2024-05-16 23:54:46.000000 url_remote-0.0.94/url_remote/src/our_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-16 23:54:46.000000 url_remote-0.0.94/url_remote/src/url_circlez.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 23:54:54.736615 url_remote-0.0.94/url_remote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-16 23:54:54.000000 url_remote-0.0.94/url_remote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-16 23:54:54.000000 url_remote-0.0.94/url_remote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 23:54:54.000000 url_remote-0.0.94/url_remote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-16 23:54:54.000000 url_remote-0.0.94/url_remote.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:08:01.403626 url_remote-0.0.95/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-20 17:08:01.403626 url_remote-0.0.95/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-20 17:07:47.000000 url_remote-0.0.95/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-20 17:07:47.000000 url_remote-0.0.95/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 17:08:01.403626 url_remote-0.0.95/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-20 17:07:47.000000 url_remote-0.0.95/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:08:01.399626 url_remote-0.0.95/url_remote/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:08:01.403626 url_remote-0.0.95/url_remote/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:07:47.000000 url_remote-0.0.95/url_remote/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-20 17:07:47.000000 url_remote-0.0.95/url_remote/src/action_name_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-20 17:07:47.000000 url_remote-0.0.95/url_remote/src/api_version_dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-20 17:07:47.000000 url_remote-0.0.95/url_remote/src/authentiction_api_version_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-20 17:07:47.000000 url_remote-0.0.95/url_remote/src/brand_name_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-20 17:07:47.000000 url_remote-0.0.95/url_remote/src/component_name_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-20 17:07:47.000000 url_remote-0.0.95/url_remote/src/entity_name_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-20 17:07:47.000000 url_remote-0.0.95/url_remote/src/environment_name_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9051 2024-05-20 17:07:47.000000 url_remote-0.0.95/url_remote/src/our_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-20 17:07:47.000000 url_remote-0.0.95/url_remote/src/url_circlez.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:08:01.403626 url_remote-0.0.95/url_remote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-20 17:08:01.000000 url_remote-0.0.95/url_remote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-20 17:08:01.000000 url_remote-0.0.95/url_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 17:08:01.000000 url_remote-0.0.95/url_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-20 17:08:01.000000 url_remote-0.0.95/url_remote.egg-info/top_level.txt
```

### Comparing `url_remote-0.0.94/README.md` & `url_remote-0.0.95/README.md`

 * *Files identical despite different names*

### Comparing `url_remote-0.0.94/setup.py` & `url_remote-0.0.95/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "url-remote"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.94',  # https://pypi.org/project/url-remote
+    version='0.0.95',  # https://pypi.org/project/url-remote
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="URL Local",
```

### Comparing `url_remote-0.0.94/url_remote/src/action_name_enum.py` & `url_remote-0.0.95/url_remote/src/action_name_enum.py`

 * *Files identical despite different names*

### Comparing `url_remote-0.0.94/url_remote/src/component_name_enum.py` & `url_remote-0.0.95/url_remote/src/component_name_enum.py`

 * *Files identical despite different names*

### Comparing `url_remote-0.0.94/url_remote/src/our_url.py` & `url_remote-0.0.95/url_remote/src/our_url.py`

 * *Files identical despite different names*

### Comparing `url_remote-0.0.94/url_remote.egg-info/SOURCES.txt` & `url_remote-0.0.95/url_remote.egg-info/SOURCES.txt`

 * *Files identical despite different names*

