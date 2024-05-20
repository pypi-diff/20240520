# Comparing `tmp/netter-0.1.tar.gz` & `tmp/netter-0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netter-0.1.tar", last modified: Mon May 20 11:00:25 2024, max compression
+gzip compressed data, was "netter-0.1a1.tar", last modified: Mon Apr 29 08:49:44 2024, max compression
```

## Comparing `netter-0.1.tar` & `netter-0.1a1.tar`

### file list

```diff
@@ -1,26 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:00:25.608359 netter-0.1/
--rw-r--r--   0 root         (0) root         (0)     1018 2024-05-20 11:00:25.608359 netter-0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-29 08:46:37.000000 netter-0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:00:25.608359 netter-0.1/netter/
--rw-r--r--   0 root         (0) root         (0)       44 2024-05-16 05:55:14.000000 netter-0.1/netter/__init__.py
--rw-r--r--   0 root         (0) root         (0)      368 2024-05-20 10:58:46.000000 netter-0.1/netter/attribute.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:00:25.608359 netter-0.1/netter/cmds/
--rw-r--r--   0 root         (0) root         (0)      796 2024-05-20 01:59:54.000000 netter-0.1/netter/cmds/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1438 2024-05-20 01:59:54.000000 netter-0.1/netter/cmds/address.py
--rw-r--r--   0 root         (0) root         (0)     6746 2024-05-20 10:36:26.000000 netter-0.1/netter/cmds/domain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:00:25.608359 netter-0.1/netter/utils/
--rw-r--r--   0 root         (0) root         (0)      665 2024-05-20 01:59:54.000000 netter-0.1/netter/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4831 2024-05-16 05:55:14.000000 netter-0.1/netter/utils/adapters.py
--rw-r--r--   0 root         (0) root         (0)      982 2024-05-08 08:22:56.000000 netter-0.1/netter/utils/format.py
--rw-r--r--   0 root         (0) root         (0)     1012 2024-05-08 09:49:26.000000 netter-0.1/netter/utils/platform.py
--rw-r--r--   0 root         (0) root         (0)     5107 2024-05-20 01:59:54.000000 netter-0.1/netter/utils/prober.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:00:25.608359 netter-0.1/netter.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1018 2024-05-20 11:00:25.000000 netter-0.1/netter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      464 2024-05-20 11:00:25.000000 netter-0.1/netter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 11:00:25.000000 netter-0.1/netter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2024-05-20 11:00:25.000000 netter-0.1/netter.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       79 2024-05-20 11:00:25.000000 netter-0.1/netter.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-05-20 11:00:25.000000 netter-0.1/netter.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 11:00:25.000000 netter-0.1/netter.egg-info/zip-safe
--rw-r--r--   0 root         (0) root         (0)      652 2024-05-20 11:00:25.608359 netter-0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1329 2024-05-10 02:38:47.000000 netter-0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 08:49:44.610128 netter-0.1a1/
+-rw-r--r--   0 root         (0) root         (0)      901 2024-04-29 08:49:44.610128 netter-0.1a1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-29 08:46:37.000000 netter-0.1a1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 08:49:44.610128 netter-0.1a1/netter/
+-rw-r--r--   0 root         (0) root         (0)       15 2024-04-29 08:45:50.000000 netter-0.1a1/netter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      376 2024-04-29 08:47:27.000000 netter-0.1a1/netter/attribute.py
+-rw-r--r--   0 root         (0) root         (0)      709 2024-04-29 08:47:32.000000 netter-0.1a1/netter/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 08:49:44.610128 netter-0.1a1/netter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      901 2024-04-29 08:49:44.000000 netter-0.1a1/netter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      292 2024-04-29 08:49:44.000000 netter-0.1a1/netter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-29 08:49:44.000000 netter-0.1a1/netter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2024-04-29 08:49:44.000000 netter-0.1a1/netter.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-29 08:49:44.000000 netter-0.1a1/netter.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-29 08:49:44.000000 netter-0.1a1/netter.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-29 08:49:44.000000 netter-0.1a1/netter.egg-info/zip-safe
+-rw-r--r--   0 root         (0) root         (0)      655 2024-04-29 08:49:44.610128 netter-0.1a1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1033 2024-04-29 08:47:08.000000 netter-0.1a1/setup.py
```

### Comparing `netter-0.1/PKG-INFO` & `netter-0.1a1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netter
-Version: 0.1
+Version: 0.1a1
 Summary: A network toolkit.
 Home-page: https://github.com/bondbox/netter/
 Author: Mingzhe Zou
 Author-email: zoumingzhe@outlook.com
 License: MIT
 Project-URL: Source Code, https://github.com/bondbox/netter/
 Project-URL: Bug Tracker, https://github.com/bondbox/netter/issues
@@ -16,16 +16,12 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: xarg-python>=1.5.1
-Requires-Dist: dnspython
-Requires-Dist: psutil
-Requires-Dist: ping3
-Requires-Dist: wmi; platform_system == "Windows"
+Requires-Dist: xarg-python>=1.5
 
 # netter
 
 A network toolkit.
```

### Comparing `netter-0.1/netter/cmds/__init__.py` & `netter-0.1a1/netter/command.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,28 +4,27 @@
 from typing import Sequence
 
 from xarg import add_command
 from xarg import argp
 from xarg import commands
 from xarg import run_command
 
-from ..attribute import __description__
-from ..attribute import __url_home__
-from ..attribute import __version__
-from .address import add_cmd_public_ip
-from .domain import add_cmd_nameserver
+from .attribute import __description__
+from .attribute import __url_home__
+from .attribute import __version__
 
 
 @add_command("netter")
 def add_cmd(_arg: argp):
     pass
 
 
-@run_command(add_cmd, add_cmd_public_ip, add_cmd_nameserver)
+@run_command(add_cmd)
 def run_cmd(cmds: commands) -> int:
+    cmds.stdout("Hello, world!")
     return 0
 
 
 def main(argv: Optional[Sequence[str]] = None) -> int:
     cmds = commands()
     cmds.version = __version__
     return cmds.run(root=add_cmd, argv=argv, description=__description__,
```

### Comparing `netter-0.1/netter.egg-info/PKG-INFO` & `netter-0.1a1/netter.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netter
-Version: 0.1
+Version: 0.1a1
 Summary: A network toolkit.
 Home-page: https://github.com/bondbox/netter/
 Author: Mingzhe Zou
 Author-email: zoumingzhe@outlook.com
 License: MIT
 Project-URL: Source Code, https://github.com/bondbox/netter/
 Project-URL: Bug Tracker, https://github.com/bondbox/netter/issues
@@ -16,16 +16,12 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: xarg-python>=1.5.1
-Requires-Dist: dnspython
-Requires-Dist: psutil
-Requires-Dist: ping3
-Requires-Dist: wmi; platform_system == "Windows"
+Requires-Dist: xarg-python>=1.5
 
 # netter
 
 A network toolkit.
```

### Comparing `netter-0.1/setup.cfg` & `netter-0.1a1/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -17,13 +17,13 @@
 [options]
 zip_safe = True
 include_package_data = True
 python_requires = >=3.8
 
 [options.entry_points]
 console_scripts = 
-	netter = netter.cmds:main
+	netter = netter.command:main
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

