# Comparing `tmp/ckanext-ark-1.0.2.tar.gz` & `tmp/ckanext_ark-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-ark-1.0.2.tar", last modified: Sun Jul 10 04:00:35 2022, max compression
+gzip compressed data, was "ckanext_ark-1.0.3.tar", last modified: Mon May 20 05:01:59 2024, max compression
```

## Comparing `ckanext-ark-1.0.2.tar` & `ckanext_ark-1.0.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2022-07-10 04:00:35.405415 ckanext-ark-1.0.2/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1070 2022-06-10 01:09:27.000000 ckanext-ark-1.0.2/LICENSE
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)       53 2022-06-25 16:03:22.000000 ckanext-ark-1.0.2/MANIFEST.in
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     5951 2022-07-10 04:00:35.405415 ckanext-ark-1.0.2/PKG-INFO
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     5443 2022-07-05 06:51:55.000000 ckanext-ark-1.0.2/README.md
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2022-07-10 04:00:35.405415 ckanext-ark-1.0.2/ckanext/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      219 2022-04-28 04:33:40.000000 ckanext-ark-1.0.2/ckanext/__init__.py
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2022-07-10 04:00:35.405415 ckanext-ark-1.0.2/ckanext/ark/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2022-06-13 12:08:07.000000 ckanext-ark-1.0.2/ckanext/ark/__init__.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     3074 2022-07-08 04:25:47.000000 ckanext-ark-1.0.2/ckanext/ark/cli.py
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2022-07-10 04:00:35.405415 ckanext-ark-1.0.2/ckanext/ark/i18n/
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2022-07-10 04:00:35.405415 ckanext-ark-1.0.2/ckanext/ark/i18n/zh_Hant_TW/
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2022-07-10 04:00:35.405415 ckanext-ark-1.0.2/ckanext/ark/i18n/zh_Hant_TW/LC_MESSAGES/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1046 2022-07-05 06:31:21.000000 ckanext-ark-1.0.2/ckanext/ark/i18n/zh_Hant_TW/LC_MESSAGES/ckanext-ark.mo
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2022-07-10 04:00:35.405415 ckanext-ark-1.0.2/ckanext/ark/lib/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2022-04-28 08:53:03.000000 ckanext-ark-1.0.2/ckanext/ark/lib/__init__.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     3397 2022-06-28 05:30:23.000000 ckanext-ark-1.0.2/ckanext/ark/lib/helpers.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      995 2022-07-07 10:29:25.000000 ckanext-ark-1.0.2/ckanext/ark/lib/minter.py
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2022-07-10 04:00:35.405415 ckanext-ark-1.0.2/ckanext/ark/model/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2022-04-28 08:03:41.000000 ckanext-ark-1.0.2/ckanext/ark/model/__init__.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      723 2022-06-13 14:54:59.000000 ckanext-ark-1.0.2/ckanext/ark/model/ark.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     3172 2022-06-16 07:46:27.000000 ckanext-ark-1.0.2/ckanext/ark/model/crud.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2774 2022-06-28 05:39:36.000000 ckanext-ark-1.0.2/ckanext/ark/plugin.py
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2022-07-10 04:00:35.405415 ckanext-ark-1.0.2/ckanext/ark/templates/
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2022-07-10 04:00:35.405415 ckanext-ark-1.0.2/ckanext/ark/templates/ark/
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2022-07-10 04:00:35.405415 ckanext-ark-1.0.2/ckanext/ark/templates/ark/snippets/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      809 2022-06-28 07:53:24.000000 ckanext-ark-1.0.2/ckanext/ark/templates/ark/snippets/ark.html
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      603 2022-06-15 01:59:26.000000 ckanext-ark-1.0.2/ckanext/ark/templates/ark/snippets/defunct.html
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1727 2022-06-16 03:52:13.000000 ckanext-ark-1.0.2/ckanext/ark/views.py
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2022-07-10 04:00:35.405415 ckanext-ark-1.0.2/ckanext_ark.egg-info/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     5951 2022-07-10 04:00:35.000000 ckanext-ark-1.0.2/ckanext_ark.egg-info/PKG-INFO
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      719 2022-07-10 04:00:35.000000 ckanext-ark-1.0.2/ckanext_ark.egg-info/SOURCES.txt
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)        1 2022-07-10 04:00:35.000000 ckanext-ark-1.0.2/ckanext_ark.egg-info/dependency_links.txt
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      107 2022-07-10 04:00:35.000000 ckanext-ark-1.0.2/ckanext_ark.egg-info/entry_points.txt
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)        8 2022-07-10 04:00:35.000000 ckanext-ark-1.0.2/ckanext_ark.egg-info/namespace_packages.txt
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)       10 2022-07-10 04:00:35.000000 ckanext-ark-1.0.2/ckanext_ark.egg-info/requires.txt
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)       13 2022-07-10 04:00:35.000000 ckanext-ark-1.0.2/ckanext_ark.egg-info/top_level.txt
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      645 2022-07-10 04:00:35.405415 ckanext-ark-1.0.2/setup.cfg
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1548 2022-07-10 03:57:46.000000 ckanext-ark-1.0.2/setup.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2024-05-20 05:01:58.994571 ckanext_ark-1.0.3/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1070 2024-05-03 16:35:45.000000 ckanext_ark-1.0.3/LICENSE
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       53 2024-05-03 16:35:45.000000 ckanext_ark-1.0.3/MANIFEST.in
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     6061 2024-05-20 05:01:58.994571 ckanext_ark-1.0.3/PKG-INFO
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     5450 2024-05-20 04:50:05.000000 ckanext_ark-1.0.3/README.md
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2024-05-20 05:01:58.994571 ckanext_ark-1.0.3/ckanext/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      219 2024-05-03 16:35:45.000000 ckanext_ark-1.0.3/ckanext/__init__.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2024-05-20 05:01:58.994571 ckanext_ark-1.0.3/ckanext/ark/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2024-05-03 16:35:45.000000 ckanext_ark-1.0.3/ckanext/ark/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     3074 2024-05-03 16:35:45.000000 ckanext_ark-1.0.3/ckanext/ark/cli.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2024-05-20 05:01:58.994571 ckanext_ark-1.0.3/ckanext/ark/i18n/
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2024-05-20 05:01:58.994571 ckanext_ark-1.0.3/ckanext/ark/i18n/zh_Hant_TW/
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2024-05-20 05:01:58.994571 ckanext_ark-1.0.3/ckanext/ark/i18n/zh_Hant_TW/LC_MESSAGES/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1046 2024-05-03 16:35:45.000000 ckanext_ark-1.0.3/ckanext/ark/i18n/zh_Hant_TW/LC_MESSAGES/ckanext-ark.mo
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2024-05-20 05:01:58.994571 ckanext_ark-1.0.3/ckanext/ark/lib/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2024-05-03 16:35:45.000000 ckanext_ark-1.0.3/ckanext/ark/lib/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     3397 2024-05-04 05:10:35.000000 ckanext_ark-1.0.3/ckanext/ark/lib/helpers.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      995 2024-05-03 16:35:45.000000 ckanext_ark-1.0.3/ckanext/ark/lib/minter.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2024-05-20 05:01:58.994571 ckanext_ark-1.0.3/ckanext/ark/model/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2024-05-03 16:35:45.000000 ckanext_ark-1.0.3/ckanext/ark/model/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      723 2024-05-03 16:35:45.000000 ckanext_ark-1.0.3/ckanext/ark/model/ark.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     3172 2024-05-03 16:35:45.000000 ckanext_ark-1.0.3/ckanext/ark/model/crud.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     3076 2024-05-03 16:35:45.000000 ckanext_ark-1.0.3/ckanext/ark/plugin.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2024-05-20 05:01:58.994571 ckanext_ark-1.0.3/ckanext/ark/templates/
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2024-05-20 05:01:58.994571 ckanext_ark-1.0.3/ckanext/ark/templates/ark/
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2024-05-20 05:01:58.994571 ckanext_ark-1.0.3/ckanext/ark/templates/ark/snippets/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      809 2024-05-03 16:35:45.000000 ckanext_ark-1.0.3/ckanext/ark/templates/ark/snippets/ark.html
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      603 2024-05-03 16:35:45.000000 ckanext_ark-1.0.3/ckanext/ark/templates/ark/snippets/defunct.html
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1803 2024-05-04 02:00:14.000000 ckanext_ark-1.0.3/ckanext/ark/views.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2024-05-20 05:01:58.994571 ckanext_ark-1.0.3/ckanext_ark.egg-info/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     6061 2024-05-20 05:01:58.000000 ckanext_ark-1.0.3/ckanext_ark.egg-info/PKG-INFO
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      719 2024-05-20 05:01:58.000000 ckanext_ark-1.0.3/ckanext_ark.egg-info/SOURCES.txt
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        1 2024-05-20 05:01:58.000000 ckanext_ark-1.0.3/ckanext_ark.egg-info/dependency_links.txt
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      107 2024-05-20 05:01:58.000000 ckanext_ark-1.0.3/ckanext_ark.egg-info/entry_points.txt
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        8 2024-05-20 05:01:58.000000 ckanext_ark-1.0.3/ckanext_ark.egg-info/namespace_packages.txt
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       22 2024-05-20 05:01:58.000000 ckanext_ark-1.0.3/ckanext_ark.egg-info/requires.txt
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       13 2024-05-20 05:01:58.000000 ckanext_ark-1.0.3/ckanext_ark.egg-info/top_level.txt
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      645 2024-05-20 05:01:58.994571 ckanext_ark-1.0.3/setup.cfg
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1621 2024-05-20 05:01:29.000000 ckanext_ark-1.0.3/setup.py
```

### Comparing `ckanext-ark-1.0.2/LICENSE` & `ckanext_ark-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-ark-1.0.2/PKG-INFO` & `ckanext_ark-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: ckanext-ark
-Version: 1.0.2
+Version: 1.0.3
 Summary: A CKAN extension for assigning Archival Resource Key (ARK) identifiers to datasets.
 Home-page: https://github.com/depositar/ckanext-ark
 Author: Cheng-Jen Lee
 Author-email: u103133.u103135@gmail.com
 License: MIT
 Keywords: CKAN ARK
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: ckantoolkit
+Requires-Dist: noid-mint
 
 [![License](https://img.shields.io/github/license/depositar/ckanext-ark)](https://opensource.org/licenses/MIT)
 [![Tests](https://github.com/depositar/ckanext-ark/workflows/Tests/badge.svg)](https://github.com/depositar/ckanext-ark/actions)
 [![Codecov](https://codecov.io/gh/depositar/ckanext-ark/branch/main/graph/badge.svg)](https://codecov.io/gh/depositar/ckanext-ark)
 [![Python](https://img.shields.io/pypi/pyversions/ckanext-ark)](https://pypi.org/project/ckanext-ark)
 [![CKAN](https://img.shields.io/badge/ckan-2.9-orange.svg)](https://github.com/ckan/ckan)
 
@@ -25,19 +28,19 @@
 
 ## Requirements
 
 Compatibility with core CKAN versions:
 
 | CKAN version    | Compatible?   |
 | --------------- | ------------- |
-| 2.7 and earlier | no            |
-| 2.8             | not tested    |
+| 2.8 and earlier | no            |
 | 2.9             | yes           |
+| 2.10            | yes           |
 
-This extension is compatible with Python 3.7 and 3.8.
+This extension is compatible with Python 3.8, 3.9, and 3.10.
 
 ## Installation
 
 To install ckanext-ark:
 
 1. Activate your CKAN virtual environment, for example:
```

### Comparing `ckanext-ark-1.0.2/README.md` & `ckanext_ark-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 
 ## Requirements
 
 Compatibility with core CKAN versions:
 
 | CKAN version    | Compatible?   |
 | --------------- | ------------- |
-| 2.7 and earlier | no            |
-| 2.8             | not tested    |
+| 2.8 and earlier | no            |
 | 2.9             | yes           |
+| 2.10            | yes           |
 
-This extension is compatible with Python 3.7 and 3.8.
+This extension is compatible with Python 3.8, 3.9, and 3.10.
 
 ## Installation
 
 To install ckanext-ark:
 
 1. Activate your CKAN virtual environment, for example:
```

### Comparing `ckanext-ark-1.0.2/ckanext/ark/cli.py` & `ckanext_ark-1.0.3/ckanext/ark/cli.py`

 * *Files identical despite different names*

### Comparing `ckanext-ark-1.0.2/ckanext/ark/i18n/zh_Hant_TW/LC_MESSAGES/ckanext-ark.mo` & `ckanext_ark-1.0.3/ckanext/ark/i18n/zh_Hant_TW/LC_MESSAGES/ckanext-ark.mo`

 * *Files identical despite different names*

### Comparing `ckanext-ark-1.0.2/ckanext/ark/lib/helpers.py` & `ckanext_ark-1.0.3/ckanext/ark/lib/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 
 from ckan.plugins import toolkit
 
 
 def _get_nma_url():
-    '''Return the NMA URL. Try and use ckanext.ark.nma_url but if that's not set
-    use ckan.site_url.
+    '''Return the NMA URL. Try and use ckanext.ark.nma_url
+    but if that's not set use ckan.site_url.
 
     :returns: the NMA URL
     :rtype: string
     '''
     nma_url = toolkit.config.get('ckanext.ark.nma_url',
                                  toolkit.config.get('ckan.site_url'))
     return nma_url.rstrip('/')
```

### Comparing `ckanext-ark-1.0.2/ckanext/ark/lib/minter.py` & `ckanext_ark-1.0.3/ckanext/ark/lib/minter.py`

 * *Files identical despite different names*

### Comparing `ckanext-ark-1.0.2/ckanext/ark/model/ark.py` & `ckanext_ark-1.0.3/ckanext/ark/model/ark.py`

 * *Files identical despite different names*

### Comparing `ckanext-ark-1.0.2/ckanext/ark/model/crud.py` & `ckanext_ark-1.0.3/ckanext/ark/model/crud.py`

 * *Files identical despite different names*

### Comparing `ckanext-ark-1.0.2/ckanext/ark/plugin.py` & `ckanext_ark-1.0.3/ckanext/ark/plugin.py`

 * *Files 25% similar despite different names*

```diff
@@ -30,15 +30,20 @@
     # IClick
 
     def get_commands(self):
         return cli.get_commands()
 
     # IPackageController
 
+    # CKAN < 2.10
     def after_update(self, context, pkg_dict):
+        return self.after_dataset_update(context, pkg_dict)
+
+    # CKAN >= 2.10
+    def after_dataset_update(self, context, pkg_dict):
         '''Dataset has been created/updated. Check status of the dataset to
         determine if we should mint ARK.
         '''
         # Is this active and public? If so we need to make sure we have
         # an active ARK
         if (pkg_dict.get('state', 'active') == 'active' and
                 not pkg_dict.get('private', False)):
@@ -67,15 +72,20 @@
             ARKQuery.update_ark(identifier=ark.identifier,
                                 last_modified=datetime.datetime.utcnow(),
                                 **erc_record
                                 )
 
         return pkg_dict
 
+    # CKAN < 2.10
     def after_show(self, context, pkg_dict):
+        return self.after_dataset_show(context, pkg_dict)
+
+    # CKAN >= 2.10
+    def after_dataset_show(self, context, pkg_dict):
         '''Add the ARK details to the pkg_dict so it can be displayed.
         '''
         ark = ARKQuery.read_package(pkg_dict['id'])
         if ark:
             pkg_dict.update({
                 'ark': f'ark:{ark.identifier}',
                 'erc_who': ark.who,
```

### Comparing `ckanext-ark-1.0.2/ckanext/ark/templates/ark/snippets/ark.html` & `ckanext_ark-1.0.3/ckanext/ark/templates/ark/snippets/ark.html`

 * *Files identical despite different names*

### Comparing `ckanext-ark-1.0.2/ckanext/ark/templates/ark/snippets/defunct.html` & `ckanext_ark-1.0.3/ckanext/ark/templates/ark/snippets/defunct.html`

 * *Files identical despite different names*

### Comparing `ckanext-ark-1.0.2/ckanext/ark/views.py` & `ckanext_ark-1.0.3/ckanext/ark/views.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,27 +6,28 @@
 from ckanext.ark.lib.helpers import get_ark_url, get_erc_support, \
     get_erc_support_commitment
 from ckanext.ark.model.crud import ARKQuery
 
 blueprints = Blueprint('ark', __name__)
 
 
-@blueprints.route('/ark:/<path:path>/')
-@blueprints.route('/ark:<path:path>/')
+@blueprints.route('/ark:/<path:path>', strict_slashes=False)
+@blueprints.route('/ark:<path:path>', strict_slashes=False)
 def read(path):
     # Show NAA metadata
     if path == toolkit.config.get('ckanext.ark.naan'):
         response = make_response(get_erc_support_commitment())
         response.headers['Content-type'] = 'text/plain; charset=UTF-8'
         return response
     ark = ARKQuery.read_ark(path)
     if not ark:
         return base.abort(404, _('ARK not found'))
     # Show ERC metadata
-    if 'info' in request.args or request.environ['REQUEST_URI'][-2:] == '/?':
+    if 'info' in request.args or \
+            request.environ['REQUEST_URI'].split('?', maxsplit=1)[-1] == '':
         response = {
             'erc': {
                 'who': ark.who,
                 'what': ark.what,
                 'when': ark.when,
                 'where': get_ark_url(ark.identifier)
             },
```

### Comparing `ckanext-ark-1.0.2/ckanext_ark.egg-info/PKG-INFO` & `ckanext_ark-1.0.3/ckanext_ark.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: ckanext-ark
-Version: 1.0.2
+Version: 1.0.3
 Summary: A CKAN extension for assigning Archival Resource Key (ARK) identifiers to datasets.
 Home-page: https://github.com/depositar/ckanext-ark
 Author: Cheng-Jen Lee
 Author-email: u103133.u103135@gmail.com
 License: MIT
 Keywords: CKAN ARK
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: ckantoolkit
+Requires-Dist: noid-mint
 
 [![License](https://img.shields.io/github/license/depositar/ckanext-ark)](https://opensource.org/licenses/MIT)
 [![Tests](https://github.com/depositar/ckanext-ark/workflows/Tests/badge.svg)](https://github.com/depositar/ckanext-ark/actions)
 [![Codecov](https://codecov.io/gh/depositar/ckanext-ark/branch/main/graph/badge.svg)](https://codecov.io/gh/depositar/ckanext-ark)
 [![Python](https://img.shields.io/pypi/pyversions/ckanext-ark)](https://pypi.org/project/ckanext-ark)
 [![CKAN](https://img.shields.io/badge/ckan-2.9-orange.svg)](https://github.com/ckan/ckan)
 
@@ -25,19 +28,19 @@
 
 ## Requirements
 
 Compatibility with core CKAN versions:
 
 | CKAN version    | Compatible?   |
 | --------------- | ------------- |
-| 2.7 and earlier | no            |
-| 2.8             | not tested    |
+| 2.8 and earlier | no            |
 | 2.9             | yes           |
+| 2.10            | yes           |
 
-This extension is compatible with Python 3.7 and 3.8.
+This extension is compatible with Python 3.8, 3.9, and 3.10.
 
 ## Installation
 
 To install ckanext-ark:
 
 1. Activate your CKAN virtual environment, for example:
```

### Comparing `ckanext-ark-1.0.2/ckanext_ark.egg-info/SOURCES.txt` & `ckanext_ark-1.0.3/ckanext_ark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-ark-1.0.2/setup.cfg` & `ckanext_ark-1.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `ckanext-ark-1.0.2/setup.py` & `ckanext_ark-1.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,32 +8,34 @@
 
 # Get the long description from the relevant file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='ckanext-ark',
-    version='1.0.2',
+    version='1.0.3',
     description='A CKAN extension for assigning Archival Resource Key '
                 '(ARK) identifiers to datasets.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/depositar/ckanext-ark',
     author='Cheng-Jen Lee',
     author_email='u103133.u103135@gmail.com',
     license='MIT',
     classifiers=[
         'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
     ],
     keywords='CKAN ARK',
     packages=find_namespace_packages(exclude=['ckanext.ark.tests']),
     namespace_packages=['ckanext'],
     install_requires=[
+        'ckantoolkit',
         'noid-mint'
     ],
     include_package_data=True,
     entry_points='''
         [ckan.plugins]
         ark=ckanext.ark.plugin:ArkPlugin
```

