# Comparing `tmp/manifestoo_core-1.5.tar.gz` & `tmp/manifestoo_core-1.6.tar.gz`

## Comparing `manifestoo_core-1.5.tar` & `manifestoo_core-1.6.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 manifestoo_core-1.5/.coveragerc
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 manifestoo_core-1.5/.flake8
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 manifestoo_core-1.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 manifestoo_core-1.5/.readthedocs.yaml
--rw-r--r--   0        0        0     4794 2020-02-02 00:00:00.000000 manifestoo_core-1.5/HISTORY.rst
--rwxr-xr-x   0        0        0     3324 2020-02-02 00:00:00.000000 manifestoo_core-1.5/mk_core_addons
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 manifestoo_core-1.5/tox.ini
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 manifestoo_core-1.5/docs/Makefile
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 manifestoo_core-1.5/docs/api.md
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 manifestoo_core-1.5/docs/changelog.rst
--rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 manifestoo_core-1.5/docs/conf.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 manifestoo_core-1.5/docs/develop.md
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 manifestoo_core-1.5/docs/index.md
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 manifestoo_core-1.5/docs/installation.md
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 manifestoo_core-1.5/docs/make.bat
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 manifestoo_core-1.5/news/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 manifestoo_core-1.5/src/manifestoo_core/__init__.py
--rw-r--r--   0        0        0     2795 2020-02-02 00:00:00.000000 manifestoo_core-1.5/src/manifestoo_core/addon.py
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 manifestoo_core-1.5/src/manifestoo_core/addons_set.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 manifestoo_core-1.5/src/manifestoo_core/exceptions.py
--rw-r--r--   0        0        0     5959 2020-02-02 00:00:00.000000 manifestoo_core-1.5/src/manifestoo_core/git_postversion.py
--rw-r--r--   0        0        0     6285 2020-02-02 00:00:00.000000 manifestoo_core-1.5/src/manifestoo_core/manifest.py
--rw-r--r--   0        0        0    18625 2020-02-02 00:00:00.000000 manifestoo_core-1.5/src/manifestoo_core/metadata.py
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 manifestoo_core-1.5/src/manifestoo_core/odoo_series.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 manifestoo_core-1.5/src/manifestoo_core/py.typed
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 manifestoo_core-1.5/src/manifestoo_core/core_addons/__init__.py
--rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 manifestoo_core-1.5/src/manifestoo_core/core_addons/addons-10.0-c.txt
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 manifestoo_core-1.5/src/manifestoo_core/core_addons/addons-10.0-e.txt
--rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 manifestoo_core-1.5/src/manifestoo_core/core_addons/addons-11.0-c.txt
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 manifestoo_core-1.5/src/manifestoo_core/core_addons/addons-11.0-e.txt
--rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 manifestoo_core-1.5/src/manifestoo_core/core_addons/addons-12.0-c.txt
--rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 manifestoo_core-1.5/src/manifestoo_core/core_addons/addons-12.0-e.txt
--rw-r--r--   0        0        0     4909 2020-02-02 00:00:00.000000 manifestoo_core-1.5/src/manifestoo_core/core_addons/addons-13.0-c.txt
--rw-r--r--   0        0        0     4608 2020-02-02 00:00:00.000000 manifestoo_core-1.5/src/manifestoo_core/core_addons/addons-13.0-e.txt
--rw-r--r--   0        0        0     5538 2020-02-02 00:00:00.000000 manifestoo_core-1.5/src/manifestoo_core/core_addons/addons-14.0-c.txt
--rw-r--r--   0        0        0     6622 2020-02-02 00:00:00.000000 manifestoo_core-1.5/src/manifestoo_core/core_addons/addons-14.0-e.txt
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 manifestoo_core-1.5/src/manifestoo_core/core_addons/addons-15.0-c.txt
--rw-r--r--   0        0        0     7522 2020-02-02 00:00:00.000000 manifestoo_core-1.5/src/manifestoo_core/core_addons/addons-15.0-e.txt
--rw-r--r--   0        0        0     7491 2020-02-02 00:00:00.000000 manifestoo_core-1.5/src/manifestoo_core/core_addons/addons-16.0-c.txt
--rw-r--r--   0        0        0     9267 2020-02-02 00:00:00.000000 manifestoo_core-1.5/src/manifestoo_core/core_addons/addons-16.0-e.txt
--rw-r--r--   0        0        0     7816 2020-02-02 00:00:00.000000 manifestoo_core-1.5/src/manifestoo_core/core_addons/addons-17.0-c.txt
--rw-r--r--   0        0        0    11069 2020-02-02 00:00:00.000000 manifestoo_core-1.5/src/manifestoo_core/core_addons/addons-17.0-e.txt
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 manifestoo_core-1.5/src/manifestoo_core/core_addons/addons-8.0-c.txt
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 manifestoo_core-1.5/src/manifestoo_core/core_addons/addons-8.0-e.txt
--rw-r--r--   0        0        0     3766 2020-02-02 00:00:00.000000 manifestoo_core-1.5/src/manifestoo_core/core_addons/addons-9.0-c.txt
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 manifestoo_core-1.5/src/manifestoo_core/core_addons/addons-9.0-e.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 manifestoo_core-1.5/tests/__init__.py
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 manifestoo_core-1.5/tests/common.py
--rw-r--r--   0        0        0     3891 2020-02-02 00:00:00.000000 manifestoo_core-1.5/tests/test_addon.py
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 manifestoo_core-1.5/tests/test_addons_set.py
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 manifestoo_core-1.5/tests/test_core_addons.py
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 manifestoo_core-1.5/tests/test_manifest.py
--rw-r--r--   0        0        0    25068 2020-02-02 00:00:00.000000 manifestoo_core-1.5/tests/test_metadata.py
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 manifestoo_core-1.5/tests/test_odoo_series.py
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 manifestoo_core-1.5/.gitignore
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 manifestoo_core-1.5/LICENSE
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 manifestoo_core-1.5/README.md
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 manifestoo_core-1.5/pyproject.toml
--rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 manifestoo_core-1.5/PKG-INFO
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 manifestoo_core-1.6/.coveragerc
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 manifestoo_core-1.6/.flake8
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 manifestoo_core-1.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 manifestoo_core-1.6/.readthedocs.yaml
+-rw-r--r--   0        0        0     4942 2020-02-02 00:00:00.000000 manifestoo_core-1.6/HISTORY.rst
+-rwxr-xr-x   0        0        0     3324 2020-02-02 00:00:00.000000 manifestoo_core-1.6/mk_core_addons
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 manifestoo_core-1.6/tox.ini
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 manifestoo_core-1.6/docs/Makefile
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 manifestoo_core-1.6/docs/api.md
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 manifestoo_core-1.6/docs/changelog.rst
+-rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 manifestoo_core-1.6/docs/conf.py
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 manifestoo_core-1.6/docs/develop.md
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 manifestoo_core-1.6/docs/index.md
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 manifestoo_core-1.6/docs/installation.md
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 manifestoo_core-1.6/docs/make.bat
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 manifestoo_core-1.6/news/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 manifestoo_core-1.6/src/manifestoo_core/__init__.py
+-rw-r--r--   0        0        0     2795 2020-02-02 00:00:00.000000 manifestoo_core-1.6/src/manifestoo_core/addon.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 manifestoo_core-1.6/src/manifestoo_core/addons_set.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 manifestoo_core-1.6/src/manifestoo_core/exceptions.py
+-rw-r--r--   0        0        0     5953 2020-02-02 00:00:00.000000 manifestoo_core-1.6/src/manifestoo_core/git_postversion.py
+-rw-r--r--   0        0        0     6285 2020-02-02 00:00:00.000000 manifestoo_core-1.6/src/manifestoo_core/manifest.py
+-rw-r--r--   0        0        0    18625 2020-02-02 00:00:00.000000 manifestoo_core-1.6/src/manifestoo_core/metadata.py
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 manifestoo_core-1.6/src/manifestoo_core/odoo_series.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 manifestoo_core-1.6/src/manifestoo_core/py.typed
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 manifestoo_core-1.6/src/manifestoo_core/core_addons/__init__.py
+-rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 manifestoo_core-1.6/src/manifestoo_core/core_addons/addons-10.0-c.txt
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 manifestoo_core-1.6/src/manifestoo_core/core_addons/addons-10.0-e.txt
+-rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 manifestoo_core-1.6/src/manifestoo_core/core_addons/addons-11.0-c.txt
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 manifestoo_core-1.6/src/manifestoo_core/core_addons/addons-11.0-e.txt
+-rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 manifestoo_core-1.6/src/manifestoo_core/core_addons/addons-12.0-c.txt
+-rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 manifestoo_core-1.6/src/manifestoo_core/core_addons/addons-12.0-e.txt
+-rw-r--r--   0        0        0     4909 2020-02-02 00:00:00.000000 manifestoo_core-1.6/src/manifestoo_core/core_addons/addons-13.0-c.txt
+-rw-r--r--   0        0        0     4608 2020-02-02 00:00:00.000000 manifestoo_core-1.6/src/manifestoo_core/core_addons/addons-13.0-e.txt
+-rw-r--r--   0        0        0     5538 2020-02-02 00:00:00.000000 manifestoo_core-1.6/src/manifestoo_core/core_addons/addons-14.0-c.txt
+-rw-r--r--   0        0        0     6622 2020-02-02 00:00:00.000000 manifestoo_core-1.6/src/manifestoo_core/core_addons/addons-14.0-e.txt
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 manifestoo_core-1.6/src/manifestoo_core/core_addons/addons-15.0-c.txt
+-rw-r--r--   0        0        0     7522 2020-02-02 00:00:00.000000 manifestoo_core-1.6/src/manifestoo_core/core_addons/addons-15.0-e.txt
+-rw-r--r--   0        0        0     7491 2020-02-02 00:00:00.000000 manifestoo_core-1.6/src/manifestoo_core/core_addons/addons-16.0-c.txt
+-rw-r--r--   0        0        0     9354 2020-02-02 00:00:00.000000 manifestoo_core-1.6/src/manifestoo_core/core_addons/addons-16.0-e.txt
+-rw-r--r--   0        0        0     8056 2020-02-02 00:00:00.000000 manifestoo_core-1.6/src/manifestoo_core/core_addons/addons-17.0-c.txt
+-rw-r--r--   0        0        0    11292 2020-02-02 00:00:00.000000 manifestoo_core-1.6/src/manifestoo_core/core_addons/addons-17.0-e.txt
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 manifestoo_core-1.6/src/manifestoo_core/core_addons/addons-8.0-c.txt
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 manifestoo_core-1.6/src/manifestoo_core/core_addons/addons-8.0-e.txt
+-rw-r--r--   0        0        0     3766 2020-02-02 00:00:00.000000 manifestoo_core-1.6/src/manifestoo_core/core_addons/addons-9.0-c.txt
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 manifestoo_core-1.6/src/manifestoo_core/core_addons/addons-9.0-e.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 manifestoo_core-1.6/tests/__init__.py
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 manifestoo_core-1.6/tests/common.py
+-rw-r--r--   0        0        0     3891 2020-02-02 00:00:00.000000 manifestoo_core-1.6/tests/test_addon.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 manifestoo_core-1.6/tests/test_addons_set.py
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 manifestoo_core-1.6/tests/test_core_addons.py
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 manifestoo_core-1.6/tests/test_manifest.py
+-rw-r--r--   0        0        0    25068 2020-02-02 00:00:00.000000 manifestoo_core-1.6/tests/test_metadata.py
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 manifestoo_core-1.6/tests/test_odoo_series.py
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 manifestoo_core-1.6/.gitignore
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 manifestoo_core-1.6/LICENSE
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 manifestoo_core-1.6/README.md
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 manifestoo_core-1.6/pyproject.toml
+-rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 manifestoo_core-1.6/PKG-INFO
```

### Comparing `manifestoo_core-1.5/HISTORY.rst` & `manifestoo_core-1.6/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v1.6 (2024-05-20)
+=================
+
+Features
+--------
+
+- Update core addon lists. (`#71 <https://github.com/acsone/manifestoo-core/issues/71>`_)
+
+
 v1.5 (2024-03-16)
 =================
 
 Features
 --------
 
 - Update core addon lists. (`#67 <https://github.com/acsone/manifestoo-core/issues/67>`_)
```

### Comparing `manifestoo_core-1.5/mk_core_addons` & `manifestoo_core-1.6/mk_core_addons`

 * *Files identical despite different names*

### Comparing `manifestoo_core-1.5/tox.ini` & `manifestoo_core-1.6/tox.ini`

 * *Files identical despite different names*

### Comparing `manifestoo_core-1.5/docs/Makefile` & `manifestoo_core-1.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `manifestoo_core-1.5/docs/api.md` & `manifestoo_core-1.6/docs/api.md`

 * *Files identical despite different names*

### Comparing `manifestoo_core-1.5/docs/conf.py` & `manifestoo_core-1.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `manifestoo_core-1.5/docs/develop.md` & `manifestoo_core-1.6/docs/develop.md`

 * *Files identical despite different names*

### Comparing `manifestoo_core-1.5/docs/make.bat` & `manifestoo_core-1.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `manifestoo_core-1.5/src/manifestoo_core/addon.py` & `manifestoo_core-1.6/src/manifestoo_core/addon.py`

 * *Files identical despite different names*

### Comparing `manifestoo_core-1.5/src/manifestoo_core/addons_set.py` & `manifestoo_core-1.6/src/manifestoo_core/addons_set.py`

 * *Files identical despite different names*

### Comparing `manifestoo_core-1.5/src/manifestoo_core/exceptions.py` & `manifestoo_core-1.6/src/manifestoo_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `manifestoo_core-1.5/src/manifestoo_core/git_postversion.py` & `manifestoo_core-1.6/src/manifestoo_core/git_postversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,19 +171,19 @@
             last_sha = sha
         else:
             count += 1
     if not count:
         return last_version
     if last_sha:
         if strategy == POST_VERSION_STRATEGY_NINETYNINE_DEVN:
-            return last_version + ".99.dev%s" % count
+            return last_version + f".99.dev{count}"
         if strategy == POST_VERSION_STRATEGY_P1_DEVN:
-            return _bump_last(last_version) + ".dev%s" % count
+            return _bump_last(last_version) + f".dev{count}"
         if strategy == POST_VERSION_STRATEGY_DOT_N:
-            return last_version + ".%s" % count
+            return last_version + f".{count}"
         msg = f"Unknown postversion strategy: {strategy}"
         raise UnknownPostVersionStrategy(msg)
     if uncommitted:
         return last_version + ".dev1"
     # if everything is committed, the last commit
     # must have the same version as current,
     # so last_sha must be set and we'll never reach this branch
```

### Comparing `manifestoo_core-1.5/src/manifestoo_core/manifest.py` & `manifestoo_core-1.6/src/manifestoo_core/manifest.py`

 * *Files identical despite different names*

### Comparing `manifestoo_core-1.5/src/manifestoo_core/metadata.py` & `manifestoo_core-1.6/src/manifestoo_core/metadata.py`

 * *Files identical despite different names*

### Comparing `manifestoo_core-1.5/src/manifestoo_core/odoo_series.py` & `manifestoo_core-1.6/src/manifestoo_core/odoo_series.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Odoo Series and Editions."""
+
 from enum import Enum
 from typing import Optional, Set
 
 from .addons_set import AddonsSet
 from .exceptions import UnsupportedOdooSeries
 
 __all__ = [
```

### Comparing `manifestoo_core-1.5/src/manifestoo_core/core_addons/__init__.py` & `manifestoo_core-1.6/src/manifestoo_core/core_addons/__init__.py`

 * *Files identical despite different names*

### Comparing `manifestoo_core-1.5/src/manifestoo_core/core_addons/addons-10.0-c.txt` & `manifestoo_core-1.6/src/manifestoo_core/core_addons/addons-10.0-c.txt`

 * *Files identical despite different names*

### Comparing `manifestoo_core-1.5/src/manifestoo_core/core_addons/addons-10.0-e.txt` & `manifestoo_core-1.6/src/manifestoo_core/core_addons/addons-10.0-e.txt`

 * *Files identical despite different names*

### Comparing `manifestoo_core-1.5/src/manifestoo_core/core_addons/addons-11.0-c.txt` & `manifestoo_core-1.6/src/manifestoo_core/core_addons/addons-11.0-c.txt`

 * *Files identical despite different names*

### Comparing `manifestoo_core-1.5/src/manifestoo_core/core_addons/addons-11.0-e.txt` & `manifestoo_core-1.6/src/manifestoo_core/core_addons/addons-11.0-e.txt`

 * *Files identical despite different names*

### Comparing `manifestoo_core-1.5/src/manifestoo_core/core_addons/addons-12.0-c.txt` & `manifestoo_core-1.6/src/manifestoo_core/core_addons/addons-12.0-c.txt`

 * *Files identical despite different names*

### Comparing `manifestoo_core-1.5/src/manifestoo_core/core_addons/addons-12.0-e.txt` & `manifestoo_core-1.6/src/manifestoo_core/core_addons/addons-12.0-e.txt`

 * *Files identical despite different names*

### Comparing `manifestoo_core-1.5/src/manifestoo_core/core_addons/addons-13.0-c.txt` & `manifestoo_core-1.6/src/manifestoo_core/core_addons/addons-13.0-c.txt`

 * *Files identical despite different names*

### Comparing `manifestoo_core-1.5/src/manifestoo_core/core_addons/addons-13.0-e.txt` & `manifestoo_core-1.6/src/manifestoo_core/core_addons/addons-13.0-e.txt`

 * *Files identical despite different names*

### Comparing `manifestoo_core-1.5/src/manifestoo_core/core_addons/addons-14.0-c.txt` & `manifestoo_core-1.6/src/manifestoo_core/core_addons/addons-14.0-c.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# generated on Fri Mar 15 20:05:06 2024
+# generated on Tue May 14 15:22:27 2024
 account
 account_check_printing
 account_debit_note
 account_edi
 account_edi_extended
 account_edi_facturx
 account_edi_proxy_client
```

### Comparing `manifestoo_core-1.5/src/manifestoo_core/core_addons/addons-14.0-e.txt` & `manifestoo_core-1.6/src/manifestoo_core/core_addons/addons-14.0-e.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# generated on Fri Mar 15 20:05:24 2024
+# generated on Tue May 14 15:22:41 2024
 account_3way_match
 account_accountant
 account_accountant_check_printing
 account_asset
 account_auto_transfer
 account_avatax
 account_avatax_sale
```

### Comparing `manifestoo_core-1.5/src/manifestoo_core/core_addons/addons-15.0-c.txt` & `manifestoo_core-1.6/src/manifestoo_core/core_addons/addons-15.0-c.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# generated on Fri Mar 15 20:04:23 2024
+# generated on Tue May 14 15:21:47 2024
 account
 account_check_printing
 account_debit_note
 account_edi
 account_edi_facturx
 account_edi_proxy_client
 account_edi_ubl
```

### Comparing `manifestoo_core-1.5/src/manifestoo_core/core_addons/addons-15.0-e.txt` & `manifestoo_core-1.6/src/manifestoo_core/core_addons/addons-15.0-e.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# generated on Fri Mar 15 20:04:38 2024
+# generated on Tue May 14 15:22:00 2024
 account_3way_match
 account_accountant
 account_accountant_batch_payment
 account_accountant_check_printing
 account_asset
 account_asset_fleet
 account_asset_ndt
```

### Comparing `manifestoo_core-1.5/src/manifestoo_core/core_addons/addons-16.0-c.txt` & `manifestoo_core-1.6/src/manifestoo_core/core_addons/addons-16.0-c.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# generated on Fri Mar 15 20:03:36 2024
+# generated on Tue May 14 15:20:58 2024
 account
 account_check_printing
 account_debit_note
 account_edi
 account_edi_proxy_client
 account_edi_ubl_cii
 account_fleet
```

### Comparing `manifestoo_core-1.5/src/manifestoo_core/core_addons/addons-16.0-e.txt` & `manifestoo_core-1.6/src/manifestoo_core/core_addons/addons-16.0-e.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# generated on Fri Mar 15 20:03:53 2024
+# generated on Tue May 14 15:21:14 2024
 account_3way_match
 account_accountant
 account_accountant_batch_payment
 account_asset
 account_asset_fleet
 account_auto_transfer
 account_avatax
@@ -23,14 +23,15 @@
 account_followup
 account_inter_company_rules
 account_intrastat
 account_invoice_extract
 account_invoice_extract_purchase
 account_online_synchronization
 account_predictive_bills
+account_reconcile_wizard
 account_reports
 account_reports_cash_basis
 account_reports_tax_reminder
 account_saft
 account_sepa
 account_sepa_direct_debit
 account_sepa_pain_001_001_09
@@ -244,14 +245,16 @@
 l10n_mx_reports_closing
 l10n_mx_xml_polizas
 l10n_mz_reports
 l10n_nl_intrastat
 l10n_nl_reports
 l10n_nl_reports_sbr
 l10n_nl_reports_sbr_icp
+l10n_nl_reports_sbr_ob_nummer
+l10n_nl_reports_sbr_status_info
 l10n_no_reports
 l10n_no_saft
 l10n_pe_edi
 l10n_pe_edi_stock
 l10n_pe_edi_stock_20
 l10n_pe_reports
 l10n_pk_reports
```

### Comparing `manifestoo_core-1.5/src/manifestoo_core/core_addons/addons-17.0-c.txt` & `manifestoo_core-1.6/src/manifestoo_core/core_addons/addons-17.0-c.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# generated on Fri Mar 15 20:02:50 2024
+# generated on Tue May 14 15:20:20 2024
 account
 account_audit_trail
 account_check_printing
 account_debit_note
 account_edi
 account_edi_proxy_client
 account_edi_ubl_cii
@@ -110,23 +110,30 @@
 l10n_ar_pos
 l10n_ar_website_sale
 l10n_ar_withholding
 l10n_at
 l10n_au
 l10n_be
 l10n_be_pos_sale
+l10n_bf
 l10n_bg
+l10n_bj
 l10n_bo
 l10n_br
 l10n_br_pix
 l10n_br_sales
 l10n_br_website_sale
 l10n_ca
+l10n_cd
+l10n_cf
+l10n_cg
 l10n_ch
+l10n_ci
 l10n_cl
+l10n_cm
 l10n_cn
 l10n_cn_city
 l10n_co
 l10n_co_pos
 l10n_cr
 l10n_cz
 l10n_de
@@ -159,24 +166,29 @@
 l10n_fi_sale
 l10n_fr
 l10n_fr_facturx_chorus_pro
 l10n_fr_fec
 l10n_fr_hr_holidays
 l10n_fr_hr_work_entry_holidays
 l10n_fr_pos_cert
+l10n_ga
 l10n_gcc_invoice
 l10n_gcc_invoice_stock_account
 l10n_gcc_pos
+l10n_gn
+l10n_gq
 l10n_gr
 l10n_gt
+l10n_gw
 l10n_hk
 l10n_hn
 l10n_hr
 l10n_hr_kuna
 l10n_hu
+l10n_hu_edi
 l10n_id
 l10n_id_efaktur
 l10n_ie
 l10n_il
 l10n_in
 l10n_in_edi
 l10n_in_edi_ewaybill
@@ -191,49 +203,60 @@
 l10n_it_edi_website_sale
 l10n_it_edi_withholding
 l10n_it_stock_ddt
 l10n_jp
 l10n_jp_ubl_pint
 l10n_ke
 l10n_ke_edi_tremol
+l10n_km
 l10n_kz
 l10n_latam_base
 l10n_latam_check
 l10n_latam_invoice_document
 l10n_lt
 l10n_lu
 l10n_lv
 l10n_ma
+l10n_ml
 l10n_mn
+l10n_mt
+l10n_mu_account
 l10n_mx
 l10n_mx_hr
 l10n_my
+l10n_my_ubl_pint
 l10n_mz
+l10n_ne
+l10n_ng
 l10n_nl
 l10n_no
 l10n_nz
 l10n_pa
 l10n_pe
 l10n_pe_pos
 l10n_pe_website_sale
 l10n_ph
 l10n_pk
 l10n_pl
 l10n_pt
 l10n_ro
 l10n_ro_edi
 l10n_rs
+l10n_rw
 l10n_sa
 l10n_sa_edi
 l10n_sa_pos
 l10n_se
 l10n_sg
 l10n_si
 l10n_sk
+l10n_sn
 l10n_syscohada
+l10n_td
+l10n_tg
 l10n_th
 l10n_tn
 l10n_tr
 l10n_tw
 l10n_ua
 l10n_ug
 l10n_uk
@@ -307,14 +330,15 @@
 portal_rating
 pos_adyen
 pos_discount
 pos_epson_printer
 pos_hr
 pos_hr_restaurant
 pos_loyalty
+pos_mercado_pago
 pos_mercury
 pos_mrp
 pos_online_payment
 pos_online_payment_self_order
 pos_paytm
 pos_razorpay
 pos_restaurant
@@ -356,14 +380,15 @@
 purchase_requisition_sale
 purchase_requisition_stock
 purchase_stock
 rating
 repair
 resource
 sale
+sale_async_emails
 sale_crm
 sale_expense
 sale_expense_margin
 sale_loyalty
 sale_loyalty_delivery
 sale_management
 sale_margin
```

### Comparing `manifestoo_core-1.5/src/manifestoo_core/core_addons/addons-17.0-e.txt` & `manifestoo_core-1.6/src/manifestoo_core/core_addons/addons-17.0-e.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# generated on Fri Mar 15 20:03:07 2024
+# generated on Tue May 14 15:20:36 2024
 account_3way_match
 account_accountant
 account_accountant_batch_payment
 account_accountant_fleet
 account_asset
 account_asset_fleet
 account_auto_transfer
@@ -188,17 +188,21 @@
 l10n_be_reports_post_wizard
 l10n_be_reports_sms
 l10n_be_soda
 l10n_be_us_consolidation_demo
 l10n_bg_reports
 l10n_bo_reports
 l10n_br_avatax
+l10n_br_avatax_services
 l10n_br_edi
 l10n_br_edi_sale
+l10n_br_edi_sale_services
+l10n_br_edi_services
 l10n_br_reports
+l10n_br_sale_subscription
 l10n_br_test_avatax_sale
 l10n_ca_check_printing
 l10n_ca_reports
 l10n_ch_hr_payroll
 l10n_ch_hr_payroll_account
 l10n_ch_reports
 l10n_cl_edi
@@ -263,14 +267,15 @@
 l10n_lu_hr_payroll
 l10n_lu_hr_payroll_account
 l10n_lu_reports
 l10n_ma_hr_payroll
 l10n_ma_hr_payroll_account
 l10n_ma_reports
 l10n_mn_reports
+l10n_mt_reports
 l10n_mx_edi
 l10n_mx_edi_extended
 l10n_mx_edi_landing
 l10n_mx_edi_pos
 l10n_mx_edi_sale
 l10n_mx_edi_stock
 l10n_mx_edi_stock_30
@@ -278,21 +283,25 @@
 l10n_mx_edi_stock_extended_30
 l10n_mx_edi_website_sale
 l10n_mx_hr_payroll
 l10n_mx_hr_payroll_account
 l10n_mx_reports
 l10n_mx_reports_closing
 l10n_mx_xml_polizas
+l10n_my_reports
 l10n_mz_reports
+l10n_ng_reports
 l10n_nl_hr_payroll
 l10n_nl_hr_payroll_account
 l10n_nl_intrastat
 l10n_nl_reports
 l10n_nl_reports_sbr
 l10n_nl_reports_sbr_icp
+l10n_nl_reports_sbr_ob_nummer
+l10n_nl_reports_sbr_status_info
 l10n_no_reports
 l10n_no_saft
 l10n_pe_edi
 l10n_pe_edi_stock
 l10n_pe_reports
 l10n_ph_reports
 l10n_pk_reports
@@ -303,14 +312,15 @@
 l10n_pt_reports
 l10n_ro_hr_payroll
 l10n_ro_hr_payroll_account
 l10n_ro_reports
 l10n_ro_saft
 l10n_ro_saft_import
 l10n_rs_reports
+l10n_rw_reports
 l10n_sa_hr_payroll
 l10n_sa_hr_payroll_account
 l10n_se_reports
 l10n_se_sie_import
 l10n_sg_reports
 l10n_si_reports
 l10n_sk_hr_payroll
```

### Comparing `manifestoo_core-1.5/src/manifestoo_core/core_addons/addons-8.0-c.txt` & `manifestoo_core-1.6/src/manifestoo_core/core_addons/addons-8.0-c.txt`

 * *Files identical despite different names*

### Comparing `manifestoo_core-1.5/src/manifestoo_core/core_addons/addons-9.0-c.txt` & `manifestoo_core-1.6/src/manifestoo_core/core_addons/addons-9.0-c.txt`

 * *Files identical despite different names*

### Comparing `manifestoo_core-1.5/src/manifestoo_core/core_addons/addons-9.0-e.txt` & `manifestoo_core-1.6/src/manifestoo_core/core_addons/addons-9.0-e.txt`

 * *Files identical despite different names*

### Comparing `manifestoo_core-1.5/tests/common.py` & `manifestoo_core-1.6/tests/common.py`

 * *Files identical despite different names*

### Comparing `manifestoo_core-1.5/tests/test_addon.py` & `manifestoo_core-1.6/tests/test_addon.py`

 * *Files identical despite different names*

### Comparing `manifestoo_core-1.5/tests/test_addons_set.py` & `manifestoo_core-1.6/tests/test_addons_set.py`

 * *Files identical despite different names*

### Comparing `manifestoo_core-1.5/tests/test_core_addons.py` & `manifestoo_core-1.6/tests/test_core_addons.py`

 * *Files identical despite different names*

### Comparing `manifestoo_core-1.5/tests/test_manifest.py` & `manifestoo_core-1.6/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `manifestoo_core-1.5/tests/test_metadata.py` & `manifestoo_core-1.6/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `manifestoo_core-1.5/tests/test_odoo_series.py` & `manifestoo_core-1.6/tests/test_odoo_series.py`

 * *Files identical despite different names*

### Comparing `manifestoo_core-1.5/.gitignore` & `manifestoo_core-1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `manifestoo_core-1.5/LICENSE` & `manifestoo_core-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `manifestoo_core-1.5/README.md` & `manifestoo_core-1.6/README.md`

 * *Files identical despite different names*

### Comparing `manifestoo_core-1.5/pyproject.toml` & `manifestoo_core-1.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -56,15 +56,18 @@
 
 [tool.hatch.build]
 exclude = [
     "/.github",
 ]
 
 [tool.ruff]
+target-version = "py37"
 fix = true
+
+[tool.ruff.lint]
 extend-select = [
     "B",  # flake8-bugbear
     "C4",  # flake8-comprehensions
     "C90",  # mccabe
     "E",
     "F",
     "I",  # isort
@@ -74,32 +77,31 @@
     "PERF",
     "RUF",
     "S",  # flake8-bandit
     "T100",  # flake8-debugger
     "TRY",
     "W",
 ]
-target-version = "py37"
 ignore = [
     # "C408",   # Unnecessary `dict` call (rewrite as a literal)
 ]
 exclude = [
     "docs/conf.py",
     "mk_core_addons",
 ]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "tests/*.py" = [
     "S101", # use of assert detected
     "S603", # `subprocess` call: check for execution of untrusted input
     "S607", # Starting a process with a partial executable path
 ]
 
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 known-first-party = ["manifestoo_core"]
 
 
 [tool.coverage.run]
 branch = true
 source_pkgs = ["manifestoo_core"]
```

### Comparing `manifestoo_core-1.5/PKG-INFO` & `manifestoo_core-1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: manifestoo_core
-Version: 1.5
+Version: 1.6
 Summary: A library to reason about Odoo addons manifests
 Project-URL: Homepage, https://github.com/acsone/manifestoo-core
 Project-URL: Documentation, https://manifestoo-core.readthedocs.io/en/stable/
 Project-URL: Changelog, https://manifestoo-core.readthedocs.io/en/stable/changelog.html
 Project-URL: Source, https://github.com/acsone/manifestoo-core
 Author-email: Stéphane Bidoul <stephane.bidoul@acsone.eu>
 License-File: LICENSE
```

