# Comparing `tmp/buildbot-worker-3.9.1.tar.gz` & `tmp/buildbot-worker-3.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildbot-worker-3.9.1.tar", last modified: Sat Sep  2 16:02:32 2023, max compression
+gzip compressed data, was "buildbot-worker-3.9.2.tar", last modified: Sat Sep  2 20:50:41 2023, max compression
```

## Comparing `buildbot-worker-3.9.1.tar` & `buildbot-worker-3.9.2.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:02:32.636358 buildbot-worker-3.9.1/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    15122 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/COPYING
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      206 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/MANIFEST.in
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    32708 2023-09-02 16:02:32.636358 buildbot-worker-3.9.1/NEWS
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1222 2023-09-02 16:02:32.636358 buildbot-worker-3.9.1/PKG-INFO
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2079 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/README
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      192 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/UPGRADING
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:02:32.636358 buildbot-worker-3.9.1/buildbot_worker/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        5 2023-09-02 16:02:32.636358 buildbot-worker-3.9.1/buildbot_worker/VERSION
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4722 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    11562 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/base.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      904 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/bot.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:02:32.628358 buildbot-worker-3.9.1/buildbot_worker/commands/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/commands/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9032 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/commands/base.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    10085 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/commands/fs.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2055 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/commands/registry.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2188 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/commands/shell.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    12685 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/commands/transfer.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4122 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/commands/utils.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2975 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/compat.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1242 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/exceptions.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3673 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/interfaces.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:02:32.628358 buildbot-worker-3.9.1/buildbot_worker/monkeypatches/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      814 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/monkeypatches/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1048 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/monkeypatches/testcase_assert.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    14126 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/msgpack.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2181 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/null.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    30789 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/pb.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6067 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/pbutil.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    33292 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/runprocess.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:02:32.628358 buildbot-worker-3.9.1/buildbot_worker/scripts/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/scripts/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1439 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/scripts/base.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7366 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/scripts/create_worker.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3926 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/scripts/logwatcher.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1383 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/scripts/restart.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9842 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/scripts/runner.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5098 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/scripts/start.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2538 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/scripts/stop.py
--rwxr-xr-x   0 buildbot  (1000) buildbot  (1000)    25140 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/scripts/windows_service.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:02:32.632358 buildbot-worker-3.9.1/buildbot_worker/test/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2154 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/test/__init__.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:02:32.632358 buildbot-worker-3.9.1/buildbot_worker/test/fake/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/test/fake/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2303 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/test/fake/protocolcommand.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6121 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/test/fake/reactor.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1378 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/test/fake/remote.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7615 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/test/fake/runprocess.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1486 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/test/reactor.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1088 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/test/test_extra_coverage.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7461 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/test/test_util_hangcheck.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:02:32.632358 buildbot-worker-3.9.1/buildbot_worker/test/unit/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/test/unit/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3543 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/test/unit/runprocess-scripts.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    13020 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/test/unit/test_bot.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    10251 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/test/unit/test_bot_Worker.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4979 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/test/unit/test_commands_base.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    15776 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/test/unit/test_commands_fs.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1506 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/test/unit/test_commands_registry.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2042 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/test/unit/test_commands_shell.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    16534 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/test/unit/test_commands_transfer.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5327 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/test/unit/test_commands_utils.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    21230 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/test/unit/test_msgpack.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    35747 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/test/unit/test_runprocess.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4196 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/test/unit/test_scripts_base.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    30379 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/test/unit/test_scripts_create_worker.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3647 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/test/unit/test_scripts_restart.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    17044 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/test/unit/test_scripts_runner.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2523 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/test/unit/test_scripts_start.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6297 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/test/unit/test_scripts_stop.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5341 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/test/unit/test_util.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2835 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/test/unit/test_util_deferwaiter.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:02:32.636358 buildbot-worker-3.9.1/buildbot_worker/test/util/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/test/util/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5077 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/test/util/command.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1066 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/test/util/compat.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8124 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/test/util/misc.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2367 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/test/util/sourcecommand.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    18013 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/test/util/test_buffer_manager.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5853 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/test/util/test_lineboundaries.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4805 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/tunnel.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:02:32.636358 buildbot-worker-3.9.1/buildbot_worker/util/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3581 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/util/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4189 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/util/_hangcheck.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1558 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/util/_notifier.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7025 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/util/buffer_manager.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1923 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/util/deferwaiter.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4276 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/buildbot_worker/util/lineboundaries.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:02:32.628358 buildbot-worker-3.9.1/buildbot_worker.egg-info/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1222 2023-09-02 16:02:32.000000 buildbot-worker-3.9.1/buildbot_worker.egg-info/PKG-INFO
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3078 2023-09-02 16:02:32.000000 buildbot-worker-3.9.1/buildbot_worker.egg-info/SOURCES.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        1 2023-09-02 16:02:32.000000 buildbot-worker-3.9.1/buildbot_worker.egg-info/dependency_links.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      163 2023-09-02 16:02:32.000000 buildbot-worker-3.9.1/buildbot_worker.egg-info/entry_points.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      113 2023-09-02 16:02:32.000000 buildbot-worker-3.9.1/buildbot_worker.egg-info/requires.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       16 2023-09-02 16:02:32.000000 buildbot-worker-3.9.1/buildbot_worker.egg-info/top_level.txt
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:02:32.636358 buildbot-worker-3.9.1/docs/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3815 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/docs/buildbot-worker.1
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      110 2023-09-02 16:02:32.636358 buildbot-worker-3.9.1/setup.cfg
--rwxr-xr-x   0 buildbot  (1000) buildbot  (1000)     6847 2023-09-02 16:00:07.000000 buildbot-worker-3.9.1/setup.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:50:41.303143 buildbot-worker-3.9.2/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    15122 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/COPYING
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      206 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/MANIFEST.in
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    32987 2023-09-02 20:50:41.303143 buildbot-worker-3.9.2/NEWS
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1222 2023-09-02 20:50:41.299143 buildbot-worker-3.9.2/PKG-INFO
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2079 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/README
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      192 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/UPGRADING
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:50:41.303143 buildbot-worker-3.9.2/buildbot_worker/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        5 2023-09-02 20:50:41.303143 buildbot-worker-3.9.2/buildbot_worker/VERSION
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4722 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    11562 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/base.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      904 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/bot.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:50:41.291143 buildbot-worker-3.9.2/buildbot_worker/commands/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/commands/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9032 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/commands/base.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    10085 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/commands/fs.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2055 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/commands/registry.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2188 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/commands/shell.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    12685 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/commands/transfer.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4122 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/commands/utils.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2975 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/compat.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1242 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/exceptions.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3673 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/interfaces.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:50:41.295143 buildbot-worker-3.9.2/buildbot_worker/monkeypatches/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      814 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/monkeypatches/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1048 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/monkeypatches/testcase_assert.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    14126 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/msgpack.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2181 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/null.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    30789 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/pb.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6067 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/pbutil.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    33292 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/runprocess.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:50:41.295143 buildbot-worker-3.9.2/buildbot_worker/scripts/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/scripts/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1439 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/scripts/base.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7366 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/scripts/create_worker.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3926 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/scripts/logwatcher.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1383 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/scripts/restart.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9842 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/scripts/runner.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5098 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/scripts/start.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2538 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/scripts/stop.py
+-rwxr-xr-x   0 buildbot  (1000) buildbot  (1000)    25140 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/scripts/windows_service.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:50:41.295143 buildbot-worker-3.9.2/buildbot_worker/test/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2154 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/test/__init__.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:50:41.295143 buildbot-worker-3.9.2/buildbot_worker/test/fake/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/test/fake/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2303 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/test/fake/protocolcommand.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6121 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/test/fake/reactor.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1378 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/test/fake/remote.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7615 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/test/fake/runprocess.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1486 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/test/reactor.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1088 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/test/test_extra_coverage.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7461 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/test/test_util_hangcheck.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:50:41.299143 buildbot-worker-3.9.2/buildbot_worker/test/unit/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/test/unit/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3543 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/test/unit/runprocess-scripts.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    13020 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/test/unit/test_bot.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    10251 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/test/unit/test_bot_Worker.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4979 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/test/unit/test_commands_base.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    15776 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/test/unit/test_commands_fs.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1506 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/test/unit/test_commands_registry.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2042 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/test/unit/test_commands_shell.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    16534 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/test/unit/test_commands_transfer.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5327 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/test/unit/test_commands_utils.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    21230 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/test/unit/test_msgpack.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    35747 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/test/unit/test_runprocess.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4196 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/test/unit/test_scripts_base.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    30379 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/test/unit/test_scripts_create_worker.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3647 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/test/unit/test_scripts_restart.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    17044 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/test/unit/test_scripts_runner.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2523 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/test/unit/test_scripts_start.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6297 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/test/unit/test_scripts_stop.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5341 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/test/unit/test_util.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2835 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/test/unit/test_util_deferwaiter.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:50:41.299143 buildbot-worker-3.9.2/buildbot_worker/test/util/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/test/util/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5077 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/test/util/command.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1066 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/test/util/compat.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8124 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/test/util/misc.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2367 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/test/util/sourcecommand.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    18013 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/test/util/test_buffer_manager.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5853 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/test/util/test_lineboundaries.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4805 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/tunnel.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:50:41.299143 buildbot-worker-3.9.2/buildbot_worker/util/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3581 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/util/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4189 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/util/_hangcheck.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1558 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/util/_notifier.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7025 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/util/buffer_manager.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1923 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/util/deferwaiter.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4276 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/buildbot_worker/util/lineboundaries.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:50:41.291143 buildbot-worker-3.9.2/buildbot_worker.egg-info/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1222 2023-09-02 20:50:41.000000 buildbot-worker-3.9.2/buildbot_worker.egg-info/PKG-INFO
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3078 2023-09-02 20:50:41.000000 buildbot-worker-3.9.2/buildbot_worker.egg-info/SOURCES.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        1 2023-09-02 20:50:41.000000 buildbot-worker-3.9.2/buildbot_worker.egg-info/dependency_links.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      163 2023-09-02 20:50:41.000000 buildbot-worker-3.9.2/buildbot_worker.egg-info/entry_points.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      113 2023-09-02 20:50:41.000000 buildbot-worker-3.9.2/buildbot_worker.egg-info/requires.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       16 2023-09-02 20:50:41.000000 buildbot-worker-3.9.2/buildbot_worker.egg-info/top_level.txt
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:50:41.299143 buildbot-worker-3.9.2/docs/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3815 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/docs/buildbot-worker.1
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      110 2023-09-02 20:50:41.303143 buildbot-worker-3.9.2/setup.cfg
+-rwxr-xr-x   0 buildbot  (1000) buildbot  (1000)     6847 2023-09-02 20:48:25.000000 buildbot-worker-3.9.2/setup.py
```

### Comparing `buildbot-worker-3.9.1/COPYING` & `buildbot-worker-3.9.2/COPYING`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/NEWS` & `buildbot-worker-3.9.2/NEWS`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,24 @@
     towncrier helps to avoid the need for rebase when several people work at the same time on the release notes files.
 
     Each PR should come with a file in the newsfragment directory
 
 .. towncrier release notes start
 
 
+Buildbot ``3.9.2`` ( ``2023-09-02`` )
+=====================================
+
+Bug fixes
+---------
+
+- Work around requirements parsing error for the Twisted dependency by pinning Twisted to 22.10 or older.
+  This fixes buildbot crash on startup when newest Twisted is installed.
+
+
 Buildbot ``3.9.1`` ( ``2023-09-02`` )
 =====================================
 
 Bug fixes
 ---------
 
 - Fixed handling of primary key columns on Postgres in the ``copy-db`` script.
```

### Comparing `buildbot-worker-3.9.1/PKG-INFO` & `buildbot-worker-3.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildbot-worker
-Version: 3.9.1
+Version: 3.9.2
 Summary: Buildbot Worker Daemon
 Home-page: http://buildbot.net/
 Author: Brian Warner
 Author-email: warner-buildbot@lothar.com
 Maintainer: Dustin J. Mitchell
 Maintainer-email: dustin@v.igoro.us
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `buildbot-worker-3.9.1/README` & `buildbot-worker-3.9.2/README`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/__init__.py` & `buildbot-worker-3.9.2/buildbot_worker/__init__.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/base.py` & `buildbot-worker-3.9.2/buildbot_worker/base.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/bot.py` & `buildbot-worker-3.9.2/buildbot_worker/bot.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/commands/base.py` & `buildbot-worker-3.9.2/buildbot_worker/commands/base.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/commands/fs.py` & `buildbot-worker-3.9.2/buildbot_worker/commands/fs.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/commands/registry.py` & `buildbot-worker-3.9.2/buildbot_worker/commands/registry.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/commands/shell.py` & `buildbot-worker-3.9.2/buildbot_worker/commands/shell.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/commands/transfer.py` & `buildbot-worker-3.9.2/buildbot_worker/commands/transfer.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/commands/utils.py` & `buildbot-worker-3.9.2/buildbot_worker/commands/utils.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/compat.py` & `buildbot-worker-3.9.2/buildbot_worker/compat.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/exceptions.py` & `buildbot-worker-3.9.2/buildbot_worker/exceptions.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/interfaces.py` & `buildbot-worker-3.9.2/buildbot_worker/interfaces.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/monkeypatches/__init__.py` & `buildbot-worker-3.9.2/buildbot_worker/monkeypatches/__init__.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/monkeypatches/testcase_assert.py` & `buildbot-worker-3.9.2/buildbot_worker/monkeypatches/testcase_assert.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/msgpack.py` & `buildbot-worker-3.9.2/buildbot_worker/msgpack.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/null.py` & `buildbot-worker-3.9.2/buildbot_worker/null.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/pb.py` & `buildbot-worker-3.9.2/buildbot_worker/pb.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/pbutil.py` & `buildbot-worker-3.9.2/buildbot_worker/pbutil.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/runprocess.py` & `buildbot-worker-3.9.2/buildbot_worker/runprocess.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/scripts/base.py` & `buildbot-worker-3.9.2/buildbot_worker/scripts/base.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/scripts/create_worker.py` & `buildbot-worker-3.9.2/buildbot_worker/scripts/create_worker.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/scripts/logwatcher.py` & `buildbot-worker-3.9.2/buildbot_worker/scripts/logwatcher.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/scripts/restart.py` & `buildbot-worker-3.9.2/buildbot_worker/scripts/restart.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/scripts/runner.py` & `buildbot-worker-3.9.2/buildbot_worker/scripts/runner.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/scripts/start.py` & `buildbot-worker-3.9.2/buildbot_worker/scripts/start.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/scripts/stop.py` & `buildbot-worker-3.9.2/buildbot_worker/scripts/stop.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/scripts/windows_service.py` & `buildbot-worker-3.9.2/buildbot_worker/scripts/windows_service.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/test/__init__.py` & `buildbot-worker-3.9.2/buildbot_worker/test/__init__.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/test/fake/protocolcommand.py` & `buildbot-worker-3.9.2/buildbot_worker/test/fake/protocolcommand.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/test/fake/reactor.py` & `buildbot-worker-3.9.2/buildbot_worker/test/fake/reactor.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/test/fake/remote.py` & `buildbot-worker-3.9.2/buildbot_worker/test/fake/remote.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/test/fake/runprocess.py` & `buildbot-worker-3.9.2/buildbot_worker/test/fake/runprocess.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/test/reactor.py` & `buildbot-worker-3.9.2/buildbot_worker/test/reactor.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/test/test_extra_coverage.py` & `buildbot-worker-3.9.2/buildbot_worker/test/test_extra_coverage.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/test/test_util_hangcheck.py` & `buildbot-worker-3.9.2/buildbot_worker/test/test_util_hangcheck.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/test/unit/runprocess-scripts.py` & `buildbot-worker-3.9.2/buildbot_worker/test/unit/runprocess-scripts.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/test/unit/test_bot.py` & `buildbot-worker-3.9.2/buildbot_worker/test/unit/test_bot.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/test/unit/test_bot_Worker.py` & `buildbot-worker-3.9.2/buildbot_worker/test/unit/test_bot_Worker.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/test/unit/test_commands_base.py` & `buildbot-worker-3.9.2/buildbot_worker/test/unit/test_commands_base.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/test/unit/test_commands_fs.py` & `buildbot-worker-3.9.2/buildbot_worker/test/unit/test_commands_fs.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/test/unit/test_commands_registry.py` & `buildbot-worker-3.9.2/buildbot_worker/test/unit/test_commands_registry.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/test/unit/test_commands_shell.py` & `buildbot-worker-3.9.2/buildbot_worker/test/unit/test_commands_shell.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/test/unit/test_commands_transfer.py` & `buildbot-worker-3.9.2/buildbot_worker/test/unit/test_commands_transfer.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/test/unit/test_commands_utils.py` & `buildbot-worker-3.9.2/buildbot_worker/test/unit/test_commands_utils.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/test/unit/test_msgpack.py` & `buildbot-worker-3.9.2/buildbot_worker/test/unit/test_msgpack.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/test/unit/test_runprocess.py` & `buildbot-worker-3.9.2/buildbot_worker/test/unit/test_runprocess.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/test/unit/test_scripts_base.py` & `buildbot-worker-3.9.2/buildbot_worker/test/unit/test_scripts_base.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/test/unit/test_scripts_create_worker.py` & `buildbot-worker-3.9.2/buildbot_worker/test/unit/test_scripts_create_worker.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/test/unit/test_scripts_restart.py` & `buildbot-worker-3.9.2/buildbot_worker/test/unit/test_scripts_restart.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/test/unit/test_scripts_runner.py` & `buildbot-worker-3.9.2/buildbot_worker/test/unit/test_scripts_runner.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/test/unit/test_scripts_start.py` & `buildbot-worker-3.9.2/buildbot_worker/test/unit/test_scripts_start.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/test/unit/test_scripts_stop.py` & `buildbot-worker-3.9.2/buildbot_worker/test/unit/test_scripts_stop.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/test/unit/test_util.py` & `buildbot-worker-3.9.2/buildbot_worker/test/unit/test_util.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/test/unit/test_util_deferwaiter.py` & `buildbot-worker-3.9.2/buildbot_worker/test/unit/test_util_deferwaiter.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/test/util/command.py` & `buildbot-worker-3.9.2/buildbot_worker/test/util/command.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/test/util/compat.py` & `buildbot-worker-3.9.2/buildbot_worker/test/util/compat.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/test/util/misc.py` & `buildbot-worker-3.9.2/buildbot_worker/test/util/misc.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/test/util/sourcecommand.py` & `buildbot-worker-3.9.2/buildbot_worker/test/util/sourcecommand.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/test/util/test_buffer_manager.py` & `buildbot-worker-3.9.2/buildbot_worker/test/util/test_buffer_manager.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/test/util/test_lineboundaries.py` & `buildbot-worker-3.9.2/buildbot_worker/test/util/test_lineboundaries.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/tunnel.py` & `buildbot-worker-3.9.2/buildbot_worker/tunnel.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/util/__init__.py` & `buildbot-worker-3.9.2/buildbot_worker/util/__init__.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/util/_hangcheck.py` & `buildbot-worker-3.9.2/buildbot_worker/util/_hangcheck.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/util/_notifier.py` & `buildbot-worker-3.9.2/buildbot_worker/util/_notifier.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/util/buffer_manager.py` & `buildbot-worker-3.9.2/buildbot_worker/util/buffer_manager.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/util/deferwaiter.py` & `buildbot-worker-3.9.2/buildbot_worker/util/deferwaiter.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker/util/lineboundaries.py` & `buildbot-worker-3.9.2/buildbot_worker/util/lineboundaries.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/buildbot_worker.egg-info/PKG-INFO` & `buildbot-worker-3.9.2/buildbot_worker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildbot-worker
-Version: 3.9.1
+Version: 3.9.2
 Summary: Buildbot Worker Daemon
 Home-page: http://buildbot.net/
 Author: Brian Warner
 Author-email: warner-buildbot@lothar.com
 Maintainer: Dustin J. Mitchell
 Maintainer-email: dustin@v.igoro.us
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `buildbot-worker-3.9.1/buildbot_worker.egg-info/SOURCES.txt` & `buildbot-worker-3.9.2/buildbot_worker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/docs/buildbot-worker.1` & `buildbot-worker-3.9.2/docs/buildbot-worker.1`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.9.1/setup.py` & `buildbot-worker-3.9.2/setup.py`

 * *Files identical despite different names*

