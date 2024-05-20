# Comparing `tmp/deltabot_cli-6.1.1.tar.gz` & `tmp/deltabot_cli-6.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltabot_cli-6.1.1.tar", last modified: Sun Apr 28 01:43:45 2024, max compression
+gzip compressed data, was "deltabot_cli-6.2.0.tar", last modified: Mon May 20 16:33:46 2024, max compression
```

## Comparing `deltabot_cli-6.1.1.tar` & `deltabot_cli-6.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:43:45.867744 deltabot_cli-6.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:43:45.863744 deltabot_cli-6.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:43:45.863744 deltabot_cli-6.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-28 01:43:36.000000 deltabot_cli-6.1.1/.github/workflows/python-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-28 01:43:36.000000 deltabot_cli-6.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-28 01:43:36.000000 deltabot_cli-6.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-28 01:43:45.867744 deltabot_cli-6.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-28 01:43:36.000000 deltabot_cli-6.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:43:45.867744 deltabot_cli-6.1.1/deltabot_cli/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-28 01:43:36.000000 deltabot_cli-6.1.1/deltabot_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-28 01:43:36.000000 deltabot_cli-6.1.1/deltabot_cli/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13473 2024-04-28 01:43:36.000000 deltabot_cli-6.1.1/deltabot_cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:43:45.867744 deltabot_cli-6.1.1/deltabot_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-28 01:43:45.000000 deltabot_cli-6.1.1/deltabot_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-28 01:43:45.000000 deltabot_cli-6.1.1/deltabot_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 01:43:45.000000 deltabot_cli-6.1.1/deltabot_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-28 01:43:45.000000 deltabot_cli-6.1.1/deltabot_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-28 01:43:45.000000 deltabot_cli-6.1.1/deltabot_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:43:45.867744 deltabot_cli-6.1.1/examples/
--rwxr-xr-x   0 runner    (1001) docker     (127)      504 2024-04-28 01:43:36.000000 deltabot_cli-6.1.1/examples/echobot.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2492 2024-04-28 01:43:36.000000 deltabot_cli-6.1.1/examples/echobot_advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-28 01:43:36.000000 deltabot_cli-6.1.1/pylama.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-28 01:43:36.000000 deltabot_cli-6.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 01:43:45.867744 deltabot_cli-6.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:33:46.165863 deltabot_cli-6.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:33:46.161862 deltabot_cli-6.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:33:46.161862 deltabot_cli-6.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-20 16:33:36.000000 deltabot_cli-6.2.0/.github/workflows/python-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-20 16:33:36.000000 deltabot_cli-6.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-05-20 16:33:36.000000 deltabot_cli-6.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-20 16:33:46.165863 deltabot_cli-6.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-20 16:33:36.000000 deltabot_cli-6.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:33:46.161862 deltabot_cli-6.2.0/deltabot_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-20 16:33:36.000000 deltabot_cli-6.2.0/deltabot_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-20 16:33:36.000000 deltabot_cli-6.2.0/deltabot_cli/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14246 2024-05-20 16:33:36.000000 deltabot_cli-6.2.0/deltabot_cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:33:46.165863 deltabot_cli-6.2.0/deltabot_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-20 16:33:46.000000 deltabot_cli-6.2.0/deltabot_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-20 16:33:46.000000 deltabot_cli-6.2.0/deltabot_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 16:33:46.000000 deltabot_cli-6.2.0/deltabot_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-20 16:33:46.000000 deltabot_cli-6.2.0/deltabot_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-20 16:33:46.000000 deltabot_cli-6.2.0/deltabot_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:33:46.165863 deltabot_cli-6.2.0/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      504 2024-05-20 16:33:36.000000 deltabot_cli-6.2.0/examples/echobot.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2492 2024-05-20 16:33:36.000000 deltabot_cli-6.2.0/examples/echobot_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-20 16:33:36.000000 deltabot_cli-6.2.0/pylama.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-20 16:33:36.000000 deltabot_cli-6.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 16:33:46.165863 deltabot_cli-6.2.0/setup.cfg
```

### Comparing `deltabot_cli-6.1.1/.github/workflows/python-ci.yml` & `deltabot_cli-6.2.0/.github/workflows/python-ci.yml`

 * *Files identical despite different names*

### Comparing `deltabot_cli-6.1.1/LICENSE` & `deltabot_cli-6.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deltabot_cli-6.1.1/PKG-INFO` & `deltabot_cli-6.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltabot-cli
-Version: 6.1.1
+Version: 6.2.0
 Summary: Library to speedup Delta Chat bot development
 Author-email: adbenitez <adb@merlinux.eu>
 Project-URL: Homepage, https://github.com/deltachat-bot/deltabot-cli-py
 Keywords: deltachat,bot,deltabot-cli
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `deltabot_cli-6.1.1/README.md` & `deltabot_cli-6.2.0/README.md`

 * *Files identical despite different names*

### Comparing `deltabot_cli-6.1.1/deltabot_cli/_utils.py` & `deltabot_cli-6.2.0/deltabot_cli/_utils.py`

 * *Files identical despite different names*

### Comparing `deltabot_cli-6.1.1/deltabot_cli/cli.py` & `deltabot_cli-6.2.0/deltabot_cli/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import logging
 import os
 import subprocess
 import sys
 import time
 from argparse import ArgumentParser, Namespace
+from pathlib import Path
 from threading import Thread
 from typing import Callable, Set, Union
 
 import qrcode
 from appdirs import user_config_dir
 from deltachat2 import Bot, CoreEvent, Event, EventType, IOTransport, JsonRpcError, Rpc
 from deltachat2.events import EventFilter, HookCollection, HookDecorator, RawEvent
@@ -127,14 +128,17 @@
         init_parser.add_argument("addr", help="the e-mail address to use")
         init_parser.add_argument("password", help="account password")
 
         config_parser = self.add_subcommand(_config_cmd, name="config")
         config_parser.add_argument("option", help="option name", nargs="?")
         config_parser.add_argument("value", help="option value to set", nargs="?")
 
+        import_parser = self.add_subcommand(_import_cmd, name="import")
+        import_parser.add_argument("path", help="path to the account backup", type=Path)
+
         self.add_subcommand(_serve_cmd, name="serve")
         self.add_subcommand(_qr_cmd, name="qr")
         self.add_subcommand(_list_cmd, name="list")
         self.add_subcommand(_remove_cmd, name="remove")
 
     def get_accounts_dir(self, args: Namespace) -> str:
         """Get bot's account folder."""
@@ -336,15 +340,15 @@
 def _list_cmd(cli: BotCli, bot: Bot, _args: Namespace) -> None:
     """show a list of existing bot accounts"""
     rpc = bot.rpc
     accounts = rpc.get_all_account_ids()
     for accid in accounts:
         addr = cli.get_address(rpc, accid)
         if not rpc.is_configured(accid):
-            addr = addr + " (not configured)"
+            addr = f"{addr or ''} (not configured)"
         print(f"#{accid} - {addr}")
 
 
 def _remove_cmd(cli: BotCli, bot: Bot, args: Namespace) -> None:
     """remove Delta Chat accounts from the bot"""
     if args.account:
         accid = cli.get_account(bot.rpc, args.account)
@@ -361,7 +365,24 @@
                 " address with -a/--account option"
             )
             sys.exit(1)
 
     addr = cli.get_address(bot.rpc, accid)
     bot.rpc.remove_account(accid)
     print(f"Account #{accid} ({addr}) removed successfully.")
+
+
+def _import_cmd(_cli: BotCli, bot: Bot, args: Namespace) -> None:
+    """import account backup"""
+    if not args.path.exists():
+        bot.logger.error(f"path doesn't exist: {str(args.path)!r}")
+        sys.exit(1)
+    accid = bot.rpc.add_account()
+    try:
+        bot.rpc.import_backup(accid, str(args.path), None)
+    except JsonRpcError as ex:
+        bot.rpc.remove_account(accid)
+        bot.logger.exception(ex)
+        sys.exit(1)
+    else:
+        addr = bot.rpc.get_config(accid, "configured_addr")
+        print(f"Account #{accid} ({addr}) imported successfully.")
```

### Comparing `deltabot_cli-6.1.1/deltabot_cli.egg-info/PKG-INFO` & `deltabot_cli-6.2.0/deltabot_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltabot-cli
-Version: 6.1.1
+Version: 6.2.0
 Summary: Library to speedup Delta Chat bot development
 Author-email: adbenitez <adb@merlinux.eu>
 Project-URL: Homepage, https://github.com/deltachat-bot/deltabot-cli-py
 Keywords: deltachat,bot,deltabot-cli
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `deltabot_cli-6.1.1/examples/echobot_advanced.py` & `deltabot_cli-6.2.0/examples/echobot_advanced.py`

 * *Files identical despite different names*

### Comparing `deltabot_cli-6.1.1/pyproject.toml` & `deltabot_cli-6.2.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -37,14 +37,17 @@
   "pylama",
   "pytest",
 ]
 
 [tool.setuptools_scm]
 # can be empty if no extra settings are needed, presence enables setuptools_scm
 
+[tool.setuptools]
+packages = ["deltabot_cli"]
+
 [tool.black]
 line-length = 100
 
 [tool.isort]
 profile = "black"
 
 [tool.mypy]
```

