# Comparing `tmp/git_trunk-0.6.0.tar.gz` & `tmp/git_trunk-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_trunk-0.6.0.tar", last modified: Wed May 15 10:45:44 2024, max compression
+gzip compressed data, was "git_trunk-0.7.1.tar", last modified: Mon May 20 12:02:27 2024, max compression
```

## Comparing `git_trunk-0.6.0.tar` & `git_trunk-0.7.1.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:45:44.345400 git_trunk-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:45:44.337400 git_trunk-0.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:45:44.341400 git_trunk-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-15 10:45:38.000000 git_trunk-0.6.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-15 10:45:38.000000 git_trunk-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    43540 2024-05-15 10:45:38.000000 git_trunk-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-15 10:45:38.000000 git_trunk-0.6.0/MANIFEST
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-15 10:45:38.000000 git_trunk-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9949 2024-05-15 10:45:44.345400 git_trunk-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9097 2024-05-15 10:45:38.000000 git_trunk-0.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:45:44.341400 git_trunk-0.6.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)    13851 2024-05-15 10:45:38.000000 git_trunk-0.6.0/bin/git-trunk
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:45:44.341400 git_trunk-0.6.0/git_trunk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 10:45:38.000000 git_trunk-0.6.0/git_trunk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14257 2024-05-15 10:45:38.000000 git_trunk-0.6.0/git_trunk/git_trunk_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    24084 2024-05-15 10:45:38.000000 git_trunk-0.6.0/git_trunk/git_trunk_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     9228 2024-05-15 10:45:38.000000 git_trunk-0.6.0/git_trunk/git_trunk_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:45:44.341400 git_trunk-0.6.0/git_trunk/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-15 10:45:38.000000 git_trunk-0.6.0/git_trunk/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5700 2024-05-15 10:45:38.000000 git_trunk-0.6.0/git_trunk/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-05-15 10:45:38.000000 git_trunk-0.6.0/git_trunk/tests/test_git_trunk_finish.py
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-05-15 10:45:38.000000 git_trunk-0.6.0/git_trunk/tests/test_git_trunk_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-05-15 10:45:38.000000 git_trunk-0.6.0/git_trunk/tests/test_git_trunk_refresh.py
--rw-r--r--   0 runner    (1001) docker     (127)    10723 2024-05-15 10:45:38.000000 git_trunk-0.6.0/git_trunk/tests/test_git_trunk_release.py
--rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-05-15 10:45:38.000000 git_trunk-0.6.0/git_trunk/tests/test_git_trunk_squash.py
--rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-05-15 10:45:38.000000 git_trunk-0.6.0/git_trunk/tests/test_git_trunk_start.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:45:44.341400 git_trunk-0.6.0/git_trunk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9949 2024-05-15 10:45:44.000000 git_trunk-0.6.0/git_trunk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-15 10:45:44.000000 git_trunk-0.6.0/git_trunk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 10:45:44.000000 git_trunk-0.6.0/git_trunk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-15 10:45:44.000000 git_trunk-0.6.0/git_trunk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 10:45:44.000000 git_trunk-0.6.0/git_trunk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 10:45:44.345400 git_trunk-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-15 10:45:38.000000 git_trunk-0.6.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-15 10:45:38.000000 git_trunk-0.6.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:02:27.814908 git_trunk-0.7.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:02:27.810908 git_trunk-0.7.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:02:27.810908 git_trunk-0.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-05-20 12:02:22.000000 git_trunk-0.7.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-20 12:02:22.000000 git_trunk-0.7.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    43540 2024-05-20 12:02:22.000000 git_trunk-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-20 12:02:22.000000 git_trunk-0.7.1/MANIFEST
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-20 12:02:22.000000 git_trunk-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10879 2024-05-20 12:02:27.814908 git_trunk-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10077 2024-05-20 12:02:22.000000 git_trunk-0.7.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:02:27.810908 git_trunk-0.7.1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15086 2024-05-20 12:02:22.000000 git_trunk-0.7.1/bin/git-trunk
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:02:27.810908 git_trunk-0.7.1/git_trunk/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-20 12:02:22.000000 git_trunk-0.7.1/git_trunk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14257 2024-05-20 12:02:22.000000 git_trunk-0.7.1/git_trunk/git_trunk_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26513 2024-05-20 12:02:22.000000 git_trunk-0.7.1/git_trunk/git_trunk_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10125 2024-05-20 12:02:22.000000 git_trunk-0.7.1/git_trunk/git_trunk_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:02:27.814908 git_trunk-0.7.1/git_trunk/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-20 12:02:22.000000 git_trunk-0.7.1/git_trunk/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5700 2024-05-20 12:02:22.000000 git_trunk-0.7.1/git_trunk/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-05-20 12:02:22.000000 git_trunk-0.7.1/git_trunk/tests/test_git_trunk_finish.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-05-20 12:02:22.000000 git_trunk-0.7.1/git_trunk/tests/test_git_trunk_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-05-20 12:02:22.000000 git_trunk-0.7.1/git_trunk/tests/test_git_trunk_refresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10723 2024-05-20 12:02:22.000000 git_trunk-0.7.1/git_trunk/tests/test_git_trunk_release.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-05-20 12:02:22.000000 git_trunk-0.7.1/git_trunk/tests/test_git_trunk_squash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-05-20 12:02:22.000000 git_trunk-0.7.1/git_trunk/tests/test_git_trunk_start.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12390 2024-05-20 12:02:22.000000 git_trunk-0.7.1/git_trunk/tests/test_git_trunk_submodule_update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:02:27.814908 git_trunk-0.7.1/git_trunk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10879 2024-05-20 12:02:27.000000 git_trunk-0.7.1/git_trunk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-20 12:02:27.000000 git_trunk-0.7.1/git_trunk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 12:02:27.000000 git_trunk-0.7.1/git_trunk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-20 12:02:27.000000 git_trunk-0.7.1/git_trunk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 12:02:27.000000 git_trunk-0.7.1/git_trunk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-20 12:02:27.814908 git_trunk-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-20 12:02:22.000000 git_trunk-0.7.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-20 12:02:22.000000 git_trunk-0.7.1/tox.ini
```

### Comparing `git_trunk-0.6.0/.github/workflows/main.yml` & `git_trunk-0.7.1/.github/workflows/main.yml`

 * *Files 14% similar despite different names*

```diff
@@ -24,16 +24,17 @@
         run: pip install tox
       - name: Run lint
         run: tox -e lint
 
   test:
     runs-on: ubuntu-latest
     strategy:
+      fail-fast: false
       matrix:
-        python: [3.7, 3.8, 3.9, "3.10", "3.11", "3.12"]
+        python: [3.8, 3.9, "3.10", "3.11", "3.12"]
     steps:
       - uses: actions/checkout@v4
       - name: Setup Python
         uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python }}
       - name: Install dependencies
```

### Comparing `git_trunk-0.6.0/LICENSE` & `git_trunk-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `git_trunk-0.6.0/PKG-INFO` & `git_trunk-0.7.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: git_trunk
-Version: 0.6.0
+Version: 0.7.1
 Summary: Git Trunk based workflow
 Home-page: https://github.com/focusate/git-trunk
 Maintainer: Andrius Laukavičius
 Maintainer-email: andrius@timefordev.com
 License: LGPLv3
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
-Requires-Python: >=3.5
+Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: footil>=0.24.0
 Requires-Dist: gitpython
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
-.. image:: https://travis-ci.com/focusate/git-trunk.svg?branch=master
-    :target: https://travis-ci.com/focusate/git-trunk
+.. image:: https://github.com/focusate/git-trunk/actions/workflows/main.yml/badge.svg
+    :target: https://github.com/focusate/git-trunk/actions/workflows/main.yml
+    :alt: Test & Deploy
 
 Git Trunk based workflow
 ########################
 
 Adds git-trunk commands that automates some common git procedures.
 
 Usage: :code:`git trunk <command>`
@@ -37,16 +37,17 @@
 
 * :code:`init`: initialize trunk configuration to be used for other commands.
 * :code:`start`: create new branch specifying custom name or use patterns to fetch/filter remote branches. First match is used to create local branch.
 * :code:`finish`: finish active branch by merging it to trunk (then remove it).
 * :code:`release`: create tag with new release version.
 * :code:`refresh`: update trunk branch and rebase it on active branch.
 * :code:`squash`: squash commits on active branch.
+* :code:`submodule-update`: update submodules.
 
-Code was tested using :code:`git version 2.25.1`.
+Code was tested using :code:`git version 2.43.2`.
 
 Source code in:
 
 * `github <https://github.com/focusate/git-trunk/>`_.
 * `pypi <https://pypi.org/project/git_trunk/>`_.
 
 Quick Start
@@ -139,14 +140,34 @@
 
 By default it tries to squash all ahead trunk commits into first one. It is possible to specify how many commits to squash with :code:`--count` argument. Value cant be greater than maximum possible commits to squash on that branch (or actually default count that is used).
 
 By default squash message generated is to concatenate all commit messages (including commit other commits are being squashed into). It is also possible to specify custom commit message, which replaces default message. It is also possible to not specify any message (but then edit mode must be enabled to enter one manually).
 
 By default squash message edit is enabled, which allows to edit tag message before it is saved. Can be disabled if needed.
 
+submodule-update
+----------------
+
+``submodule-update`` command is used to run submodule updates.
+
+It is possible to manage these options via configuration:
+
+* ``pathspec``: paths for which submodules to do updates. If left empty, will update all.
+* ``depth``: how many commits to fetch. If its 0, then it will fetch all history normally.
+* ``single-branch``: whether to fetch single default branch.
+
+There is also ``--cleanup`` argument when initiating command (not able to set via
+ configuration). With this option you can do full cleanup of existing local submodules.
+
+Do note that all local changes (that are not saved on remote) will be deleted.
+
+Also if submodules have have been moved around, automatic cleanup might fail. So you
+might need to do manual cleanup, deleting all submodules where it is currently located
+and then ``.git/modules/`` content as well.
+
 Testing
 =======
 
 To test with newer ``git``, adding submodules from files must be enabled:
 
 .. code-block::
```

### Comparing `git_trunk-0.6.0/README.rst` & `git_trunk-0.7.1/git_trunk.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,34 @@
-.. image:: https://travis-ci.com/focusate/git-trunk.svg?branch=master
-    :target: https://travis-ci.com/focusate/git-trunk
+Metadata-Version: 2.1
+Name: git_trunk
+Version: 0.7.1
+Summary: Git Trunk based workflow
+Home-page: https://github.com/focusate/git-trunk
+Maintainer: Andrius Laukavičius
+Maintainer-email: andrius@timefordev.com
+License: LGPLv3
+Classifier: Environment :: Other Environment
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development
+Classifier: Topic :: Utilities
+Requires-Python: >=3.8
+License-File: LICENSE
+Requires-Dist: footil>=0.24.0
+Requires-Dist: gitpython
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+
+.. image:: https://github.com/focusate/git-trunk/actions/workflows/main.yml/badge.svg
+    :target: https://github.com/focusate/git-trunk/actions/workflows/main.yml
+    :alt: Test & Deploy
 
 Git Trunk based workflow
 ########################
 
 Adds git-trunk commands that automates some common git procedures.
 
 Usage: :code:`git trunk <command>`
@@ -12,16 +37,17 @@
 
 * :code:`init`: initialize trunk configuration to be used for other commands.
 * :code:`start`: create new branch specifying custom name or use patterns to fetch/filter remote branches. First match is used to create local branch.
 * :code:`finish`: finish active branch by merging it to trunk (then remove it).
 * :code:`release`: create tag with new release version.
 * :code:`refresh`: update trunk branch and rebase it on active branch.
 * :code:`squash`: squash commits on active branch.
+* :code:`submodule-update`: update submodules.
 
-Code was tested using :code:`git version 2.25.1`.
+Code was tested using :code:`git version 2.43.2`.
 
 Source code in:
 
 * `github <https://github.com/focusate/git-trunk/>`_.
 * `pypi <https://pypi.org/project/git_trunk/>`_.
 
 Quick Start
@@ -114,14 +140,34 @@
 
 By default it tries to squash all ahead trunk commits into first one. It is possible to specify how many commits to squash with :code:`--count` argument. Value cant be greater than maximum possible commits to squash on that branch (or actually default count that is used).
 
 By default squash message generated is to concatenate all commit messages (including commit other commits are being squashed into). It is also possible to specify custom commit message, which replaces default message. It is also possible to not specify any message (but then edit mode must be enabled to enter one manually).
 
 By default squash message edit is enabled, which allows to edit tag message before it is saved. Can be disabled if needed.
 
+submodule-update
+----------------
+
+``submodule-update`` command is used to run submodule updates.
+
+It is possible to manage these options via configuration:
+
+* ``pathspec``: paths for which submodules to do updates. If left empty, will update all.
+* ``depth``: how many commits to fetch. If its 0, then it will fetch all history normally.
+* ``single-branch``: whether to fetch single default branch.
+
+There is also ``--cleanup`` argument when initiating command (not able to set via
+ configuration). With this option you can do full cleanup of existing local submodules.
+
+Do note that all local changes (that are not saved on remote) will be deleted.
+
+Also if submodules have have been moved around, automatic cleanup might fail. So you
+might need to do manual cleanup, deleting all submodules where it is currently located
+and then ``.git/modules/`` content as well.
+
 Testing
 =======
 
 To test with newer ``git``, adding submodules from files must be enabled:
 
 .. code-block::
```

### Comparing `git_trunk-0.6.0/bin/git-trunk` & `git_trunk-0.7.1/bin/git-trunk`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 #!/usr/bin/env python3
+import sys
 import abc
 import argparse
 from distutils.util import strtobool
 
 from git_trunk.git_trunk_config import GitTrunkConfig
 from git_trunk.git_trunk_base import DEFAULT_LOG_LEVEL
 from git_trunk.git_trunk_commands import (
     GitTrunkInit,
     GitTrunkStart,
     GitTrunkFinish,
     GitTrunkRelease,
     GitTrunkRefresh,
     GitTrunkSquash,
+    GitTrunkSubmoduleUpdate,
 )
 from git_trunk import __version__
 
 
 _subparsers_map = {}
 
 
@@ -103,14 +105,18 @@
             name = '--%s' % name
         self.parser.add_argument(
             name,
             help=self.description
         )
 
 
+class ArgAdderInt(ArgAdderStr):
+    pass
+
+
 class ArgAdderBool(BaseArgAdder):
     """Class to add bool type argument on parser."""
 
     def add(self) -> None:
         """Override to implement bool type argument add."""
         add_bool_arg(
             self.parser,
@@ -188,18 +194,20 @@
 
 class SubparserTrunkInit(BaseSubparserTrunk):
     """Init command subparser."""
 
     git_trunk_class = GitTrunkInit
     arg_adders_map = {
         str: ArgAdderStr,
+        int: ArgAdderInt,
         bool: ArgAdderBool,
     }
     convert_func_map = {
         str: None,
+        int: int,
         bool: strtorealbool,
     }
     config_struct = GitTrunkConfig.get_config_struct()
 
     def _get_option_type(self, option_vals):
         return type(option_vals['default'])
 
@@ -250,22 +258,24 @@
             if inp:
                 if convert_func:
                     inp = convert_func(inp)
                 init_cfg[section][key] = inp
 
         init_cfg = trunk_init._init_cfg
         for section, section_struct in self.config_struct.items():
+            print("Sub-command:", section)
             for option, option_vals in section_struct.items():
                 option_type = self._get_option_type(option_vals)
                 convert_func = self.convert_func_map[option_type]
                 handle_input(
                     option,
                     option_vals['label'],
                     section,
                     convert_func=convert_func)
+            print()
 
     def init_trunk_class(self, init_kwargs, args):
         """Override to implement input confirmation."""
         trunk_init = super().init_trunk_class(init_kwargs, args)
         if not args.no_confirm:
             print(
                 "Enter new value to set it, leave empty to keep current "
@@ -396,14 +406,41 @@
             'count': args.count,
             'include_squash_msg': not args.no_squash_msg,
             'custom_msg': args.custom_msg,
         })
         return init_kwargs, run_kwargs
 
 
+class SubparserTrunkSubmoduleUpdate(BaseSubparserTrunk):
+    """Submodule update command subparser."""
+
+    git_trunk_class = GitTrunkSubmoduleUpdate
+
+    def __init__(self, subparsers: argparse._SubParsersAction):
+        """Initialize submodule-update subparser."""
+        super().__init__(subparsers)
+        self.parser.add_argument(
+            '--cleanup',
+            action='store_true',
+            help="whether to do full submodules cleanup before update")
+
+    def prepare_args(self, args):
+        """Override to prepare GitTrunkSubmoduleUpdate specific args."""
+        init_kwargs, run_kwargs = super().prepare_args(args)
+        if args.cleanup:
+            answer = input(
+                "--cleanup option will remove all submodules locally. Are you sure you"
+                + " want to do it? y/n\n"
+            )
+            if not strtorealbool(answer):
+                sys.exit(0)
+        run_kwargs.update({'cleanup': args.cleanup})
+        return init_kwargs, run_kwargs
+
+
 def main():
     """Run specified git-trunk command."""
 
     parser = argparse.ArgumentParser(description="Git Trunk")
     subparsers = parser.add_subparsers(
         dest='command', help="Git Trunk Commands")
     parser.add_argument(
@@ -412,14 +449,15 @@
         version='git-trunk version {version}'.format(version=__version__))
     SubparserTrunkInit(subparsers)
     SubparserTrunkStart(subparsers)
     SubparserTrunkFinish(subparsers)
     SubparserTrunkRelease(subparsers)
     SubparserTrunkRefresh(subparsers)
     SubparserTrunkSquash(subparsers)
+    SubparserTrunkSubmoduleUpdate(subparsers)
     args = parser.parse_args()
     dest_subparser = _subparsers_map[args.command]
     dest_subparser.execute(args)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `git_trunk-0.6.0/git_trunk/git_trunk_base.py` & `git_trunk-0.7.1/git_trunk/git_trunk_base.py`

 * *Files identical despite different names*

### Comparing `git_trunk-0.6.0/git_trunk/git_trunk_commands.py` & `git_trunk-0.7.1/git_trunk/git_trunk_commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 """Git Trunk based workflow helper commands."""
+from __future__ import annotations
 import re
+import os
+import pathlib
 from collections import namedtuple
 from typing import Optional, Union
 import natsort
 from footil.path import chdir_tmp
 from footil.patterns import MethodCommand
 from footil import version as version_manager
 import git  # GitPython
@@ -14,14 +17,18 @@
 EMPTY_VERSION = '0.0.0'  # default version when are no versions yet
 
 MethodData = namedtuple('MethodData', 'method args kwargs')
 # Set defaults for args and kwargs.
 MethodData.__new__.__defaults__ = ((), {})
 
 
+def is_empty_dir(path: pathlib.Path) -> bool:
+    return not any(path.iterdir())
+
+
 class GitTrunkInit(gt_base.GitTrunkCommand):
     """Class to handle trunk configuration initialization."""
 
     def _prepare_init_config(self, kwargs) -> dict:
         """Init cfg struct with existing cfg (if any) for run method.
 
         Value is determined using this priority:
@@ -219,16 +226,18 @@
                 "branch: %s" % trunk_branch_name)
         # If active branch is not ahead trunk branch. There is no point
         # to finish it (no new changes).
         if not self.count_commits_ahead_trunk():
             raise ValueError(
                 "%s branch has no changes to be finished"
                 " on %s." % (self.active_branch_name, trunk_branch_name))
-        if (self.config.section['require_squash'] and
-                self.max_squash_commits_count):
+        if (
+            self.config.section['require_squash']
+            and self.max_squash_commits_count
+        ):
             raise ValueError(
                 "%s branch must be squashed first before finishing" %
                 self.active_branch_name)
         return res
 
     def run(self, **kwargs) -> None:
         """Merge active on trunk, push and then delete active branch.
@@ -628,7 +637,71 @@
                 gt_base._git_cmd(['commit', '--amend'])
         if self.config.section['force_push_squash']:
             tracking_data = self.active_tracking_branch_data
             if tracking_data:
                 self.git_push(
                     tracking_data.remote, tracking_data.head, '--force'
                 )
+
+
+class GitTrunkSubmoduleUpdate(gt_base.GitTrunkCommand):
+    """Command to update/init submodules."""
+
+    section = gt_config.SUBMODULE_UPDATE_SECTION
+
+    def run(self, cleanup=False, **kwargs):
+        """Update submodules.
+
+        Args:
+            cleanup: whether to do full submodules cleanup before update
+
+        These commands will be run:
+
+        """
+        super().run(**kwargs)
+        if cleanup:
+            self._cleanup_submodules()
+        self.git.submodule(
+            *self._prepare_cmd_args(**kwargs), _log_input=True, _log_output=True
+        )
+
+    def _prepare_cmd_args(self, **kwargs):
+        args = self._prepare_base_args(**kwargs)
+        section = self.config.section
+        depth = section['depth']
+        if depth:
+            args.append(f'--depth={depth}')
+        if section['single_branch']:
+            args.append('--single-branch')
+        path_spec = section['path_spec']
+        if path_spec:
+            args.extend(path_spec.split(' '))
+        return args
+
+    def _prepare_base_args(self, **kwargs):
+        return ['update', '--init']
+
+    def _cleanup_submodules(self):
+        paths = self._get_gitmodule_paths()
+        non_empty_paths = [str(p) for p in paths if p.is_dir() and not is_empty_dir(p)]
+        # NOTE. If submodules were moved around, some data might not be picked up
+        # by deinit, so manual clean up could be needed.
+        if non_empty_paths:
+            self.git.submodule(
+                'deinit', '-f', *non_empty_paths, _log_input=True, _log_output=True
+            )
+        git_modules_content = '.git/modules/*'
+        os.system(f'rm -rf {git_modules_content}')
+        print(git_modules_content, "content removed")
+
+    def _get_gitmodule_paths(self) -> list[pathlib.Path]:
+        cfg_path = pathlib.Path(self.git.working_dir) / '.gitmodules'
+        if not cfg_path.is_file():
+            raise ValueError(f"No .gitmodule found in {self.git.working_dir}")
+        cfg = git.GitConfigParser(file_or_files=cfg_path)
+        paths = []
+        for section in cfg.sections():
+            items = cfg.items(section)
+            # Assuming path exists
+            path = [x[1] for x in items if x[0] == 'path'][0]
+            paths.append(pathlib.Path(path))
+        return paths
```

### Comparing `git_trunk-0.6.0/git_trunk/git_trunk_config.py` & `git_trunk-0.7.1/git_trunk/git_trunk_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 SEP = '"'
 BASE_SECTION = 'trunk'
 START_SECTION = 'start'
 FINISH_SECTION = 'finish'
 RELEASE_SECTION = 'release'
 SQUASH_SECTION = 'squash'
+SUBMODULE_UPDATE_SECTION = 'submodule-update'
 SECTION_PATTERN = '{section} {sep}%s{sep}'.format(
     section=BASE_SECTION, sep=SEP)
 
 # True means, BASE section, False other sections.
 PATH_SECTION_PATTERN_MAP = {
     True: '{section} %(sep)s{path}%(sep)s' % {'sep': SEP},
     False: '{path}.{section}'
@@ -139,14 +140,35 @@
                     'force_push_squash',
                     default=True,
                     description=(
                         "Whether to force push to remote tracking branch"
                         " after squashing."
                     )
                 ),
+            },
+            SUBMODULE_UPDATE_SECTION: {
+                'pathspec': cls.get_option_vals(
+                    'path_spec',
+                    default='',
+                    forced_type=str,
+                    description="Path spec to update specific submodules. If"
+                    + " left empty, updates all."
+                ),
+                'depth': cls.get_option_vals(
+                    'depth',
+                    default=0,
+                    forced_type=int,
+                    description="How many latest commits to fetch. "
+                    + "0 means, all commits"
+                ),
+                'singlebranch': cls.get_option_vals(
+                    'single_branch',
+                    default=False,
+                    description="Whether to fetch only HEAD (default) branch"
+                ),
             }
         }
 
     def handle_exception(
             self, exception: Exception, msg: str, section: str, option: str):
         """Handle exception when reading git configuration.
```

### Comparing `git_trunk-0.6.0/git_trunk/tests/common.py` & `git_trunk-0.7.1/git_trunk/tests/common.py`

 * *Files identical despite different names*

### Comparing `git_trunk-0.6.0/git_trunk/tests/test_git_trunk_finish.py` & `git_trunk-0.7.1/git_trunk/tests/test_git_trunk_finish.py`

 * *Files identical despite different names*

### Comparing `git_trunk-0.6.0/git_trunk/tests/test_git_trunk_init.py` & `git_trunk-0.7.1/git_trunk/tests/test_git_trunk_init.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from git_trunk.git_trunk_commands import GitTrunkInit
 from git_trunk.git_trunk_config import (
     BASE_SECTION,
     START_SECTION,
     FINISH_SECTION,
     RELEASE_SECTION,
     SQUASH_SECTION,
+    SUBMODULE_UPDATE_SECTION,
 )
 from . import common
 
 
 class TestGitTrunkInit(common.GitTrunkCommon):
     """Class to test git-trunk init command."""
 
@@ -79,14 +80,15 @@
     def test_02_get_config(self):
         """Get config options.
 
         Check if every option has expected type.
         """
         self.git_trunk_init._init_cfg[BASE_SECTION]['trunkbranch'] = '12.0'
         self.git_trunk_init._init_cfg[RELEASE_SECTION]['versionprefix'] = '1'
+        self.git_trunk_init._init_cfg[SUBMODULE_UPDATE_SECTION]['pathspec'] = 'abc'
         self.git_trunk_init.run()
         trunk_init = GitTrunkInit(
             repo_path=self.dir_local.name, log_level=common.LOG_LEVEL)
         config = trunk_init.config
         self.assertEqual(
             config.sections,
             # Note. Other defaults are modified on common.py.
@@ -106,15 +108,20 @@
                     'release_branch_prefix': 'release/',
                     'use_semver': True,
                     'edit_tag_message': False,
                 },
                 SQUASH_SECTION: {
                     'edit_squash_message': False,
                     'force_push_squash': True
-                }
+                },
+                SUBMODULE_UPDATE_SECTION: {
+                    'path_spec': 'abc',
+                    'depth': 0,
+                    'single_branch': False,
+                },
             }
         )
 
     def test_03_remote_name(self):
         """Get remote name with set/not set active branch.
 
         Case 1: default remote on active branch.
```

### Comparing `git_trunk-0.6.0/git_trunk/tests/test_git_trunk_refresh.py` & `git_trunk-0.7.1/git_trunk/tests/test_git_trunk_refresh.py`

 * *Files identical despite different names*

### Comparing `git_trunk-0.6.0/git_trunk/tests/test_git_trunk_release.py` & `git_trunk-0.7.1/git_trunk/tests/test_git_trunk_release.py`

 * *Files identical despite different names*

### Comparing `git_trunk-0.6.0/git_trunk/tests/test_git_trunk_squash.py` & `git_trunk-0.7.1/git_trunk/tests/test_git_trunk_squash.py`

 * *Files identical despite different names*

### Comparing `git_trunk-0.6.0/git_trunk/tests/test_git_trunk_start.py` & `git_trunk-0.7.1/git_trunk/tests/test_git_trunk_start.py`

 * *Files identical despite different names*

### Comparing `git_trunk-0.6.0/git_trunk.egg-info/PKG-INFO` & `git_trunk-0.7.1/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,10 @@
-Metadata-Version: 2.1
-Name: git_trunk
-Version: 0.6.0
-Summary: Git Trunk based workflow
-Home-page: https://github.com/focusate/git-trunk
-Maintainer: Andrius Laukavičius
-Maintainer-email: andrius@timefordev.com
-License: LGPLv3
-Classifier: Environment :: Other Environment
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Software Development
-Classifier: Topic :: Utilities
-Requires-Python: >=3.5
-License-File: LICENSE
-Requires-Dist: footil>=0.24.0
-Requires-Dist: gitpython
-Provides-Extra: test
-Requires-Dist: pytest; extra == "test"
-
-.. image:: https://travis-ci.com/focusate/git-trunk.svg?branch=master
-    :target: https://travis-ci.com/focusate/git-trunk
+.. image:: https://github.com/focusate/git-trunk/actions/workflows/main.yml/badge.svg
+    :target: https://github.com/focusate/git-trunk/actions/workflows/main.yml
+    :alt: Test & Deploy
 
 Git Trunk based workflow
 ########################
 
 Adds git-trunk commands that automates some common git procedures.
 
 Usage: :code:`git trunk <command>`
@@ -37,16 +13,17 @@
 
 * :code:`init`: initialize trunk configuration to be used for other commands.
 * :code:`start`: create new branch specifying custom name or use patterns to fetch/filter remote branches. First match is used to create local branch.
 * :code:`finish`: finish active branch by merging it to trunk (then remove it).
 * :code:`release`: create tag with new release version.
 * :code:`refresh`: update trunk branch and rebase it on active branch.
 * :code:`squash`: squash commits on active branch.
+* :code:`submodule-update`: update submodules.
 
-Code was tested using :code:`git version 2.25.1`.
+Code was tested using :code:`git version 2.43.2`.
 
 Source code in:
 
 * `github <https://github.com/focusate/git-trunk/>`_.
 * `pypi <https://pypi.org/project/git_trunk/>`_.
 
 Quick Start
@@ -139,14 +116,34 @@
 
 By default it tries to squash all ahead trunk commits into first one. It is possible to specify how many commits to squash with :code:`--count` argument. Value cant be greater than maximum possible commits to squash on that branch (or actually default count that is used).
 
 By default squash message generated is to concatenate all commit messages (including commit other commits are being squashed into). It is also possible to specify custom commit message, which replaces default message. It is also possible to not specify any message (but then edit mode must be enabled to enter one manually).
 
 By default squash message edit is enabled, which allows to edit tag message before it is saved. Can be disabled if needed.
 
+submodule-update
+----------------
+
+``submodule-update`` command is used to run submodule updates.
+
+It is possible to manage these options via configuration:
+
+* ``pathspec``: paths for which submodules to do updates. If left empty, will update all.
+* ``depth``: how many commits to fetch. If its 0, then it will fetch all history normally.
+* ``single-branch``: whether to fetch single default branch.
+
+There is also ``--cleanup`` argument when initiating command (not able to set via
+ configuration). With this option you can do full cleanup of existing local submodules.
+
+Do note that all local changes (that are not saved on remote) will be deleted.
+
+Also if submodules have have been moved around, automatic cleanup might fail. So you
+might need to do manual cleanup, deleting all submodules where it is currently located
+and then ``.git/modules/`` content as well.
+
 Testing
 =======
 
 To test with newer ``git``, adding submodules from files must be enabled:
 
 .. code-block::
```

### Comparing `git_trunk-0.6.0/git_trunk.egg-info/SOURCES.txt` & `git_trunk-0.7.1/git_trunk.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 .gitignore
 LICENSE
 MANIFEST
 MANIFEST.in
 README.rst
+setup.cfg
 setup.py
 tox.ini
 .github/workflows/main.yml
 bin/git-trunk
 git_trunk/__init__.py
 git_trunk/git_trunk_base.py
 git_trunk/git_trunk_commands.py
@@ -19,8 +20,9 @@
 git_trunk/tests/__init__.py
 git_trunk/tests/common.py
 git_trunk/tests/test_git_trunk_finish.py
 git_trunk/tests/test_git_trunk_init.py
 git_trunk/tests/test_git_trunk_refresh.py
 git_trunk/tests/test_git_trunk_release.py
 git_trunk/tests/test_git_trunk_squash.py
-git_trunk/tests/test_git_trunk_start.py
+git_trunk/tests/test_git_trunk_start.py
+git_trunk/tests/test_git_trunk_submodule_update.py
```

### Comparing `git_trunk-0.6.0/setup.py` & `git_trunk-0.7.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,19 +16,18 @@
     extras_require=extras,
     setup_requires=[
         'setuptools_scm',
     ],
     scripts=['bin/git-trunk'],
     maintainer='Andrius Laukavičius',
     maintainer_email='andrius@timefordev.com',
-    python_requires='>=3.5',
+    python_requires='>=3.8',
     classifiers=[
         'Environment :: Other Environment',
         'Intended Audience :: Developers',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
         'Topic :: Software Development',
         'Topic :: Utilities',
```

