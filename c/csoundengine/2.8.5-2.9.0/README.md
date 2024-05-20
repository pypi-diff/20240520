# Comparing `tmp/csoundengine-2.8.5.tar.gz` & `tmp/csoundengine-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csoundengine-2.8.5.tar", last modified: Wed May  1 16:04:10 2024, max compression
+gzip compressed data, was "csoundengine-2.9.0.tar", last modified: Mon May 20 18:47:27 2024, max compression
```

## Comparing `csoundengine-2.8.5.tar` & `csoundengine-2.9.0.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-05-01 16:04:10.975024 csoundengine-2.8.5/
--rw-rw-r--   0 em        (1000) em        (1000)    35128 2021-11-13 21:37:59.000000 csoundengine-2.8.5/LICENSE.txt
--rw-rw-r--   0 em        (1000) em        (1000)       24 2021-11-13 21:37:59.000000 csoundengine-2.8.5/MANIFEST.in
--rw-r--r--   0 em        (1000) em        (1000)     6749 2024-05-01 16:04:10.975024 csoundengine-2.8.5/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)     5728 2024-01-10 12:24:51.000000 csoundengine-2.8.5/README.rst
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-05-01 16:04:10.960024 csoundengine-2.8.5/csoundengine/
--rw-r--r--   0 em        (1000) em        (1000)     4112 2024-04-19 12:36:50.000000 csoundengine-2.8.5/csoundengine/__init__.py
--rw-rw-r--   0 em        (1000) em        (1000)     1055 2023-03-14 09:38:54.000000 csoundengine-2.8.5/csoundengine/__sessionbase.py
--rw-r--r--   0 em        (1000) em        (1000)      177 2023-11-24 08:20:24.000000 csoundengine-2.8.5/csoundengine/_common.py
--rw-r--r--   0 em        (1000) em        (1000)     6244 2024-04-25 07:47:16.000000 csoundengine-2.8.5/csoundengine/abstractrenderer.py
--rw-r--r--   0 em        (1000) em        (1000)    12846 2024-04-25 19:14:45.000000 csoundengine-2.8.5/csoundengine/baseschedevent.py
--rw-rw-r--   0 em        (1000) em        (1000)     5848 2024-04-17 08:24:25.000000 csoundengine-2.8.5/csoundengine/busproxy.py
--rw-r--r--   0 em        (1000) em        (1000)     8470 2024-04-25 08:46:55.000000 csoundengine-2.8.5/csoundengine/config.py
--rw-rw-r--   0 em        (1000) em        (1000)        0 2023-10-17 11:02:49.000000 csoundengine-2.8.5/csoundengine/contants.py
--rwxr-xr-x   0 em        (1000) em        (1000)   126875 2024-04-19 12:01:57.000000 csoundengine-2.8.5/csoundengine/csoundlib.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-05-01 16:04:10.955024 csoundengine-2.8.5/csoundengine/data/
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-05-01 16:04:10.955024 csoundengine-2.8.5/csoundengine/data/plugins6/
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-05-01 16:04:10.963024 csoundengine-2.8.5/csoundengine/data/plugins6/linux-x86_64/
--rw-rw-r--   0 em        (1000) em        (1000)    31400 2024-04-03 07:40:27.000000 csoundengine-2.8.5/csoundengine/data/plugins6/linux-x86_64/libbeosc.so
--rw-rw-r--   0 em        (1000) em        (1000)   130864 2024-04-03 07:40:27.000000 csoundengine-2.8.5/csoundengine/data/plugins6/linux-x86_64/libelse.so
--rw-rw-r--   0 em        (1000) em        (1000)   346592 2024-04-03 07:40:27.000000 csoundengine-2.8.5/csoundengine/data/plugins6/linux-x86_64/libjsfx.so
--rw-rw-r--   0 em        (1000) em        (1000)   108568 2024-04-03 07:40:27.000000 csoundengine-2.8.5/csoundengine/data/plugins6/linux-x86_64/libklib.so
--rw-rw-r--   0 em        (1000) em        (1000)    28312 2024-04-03 07:40:27.000000 csoundengine-2.8.5/csoundengine/data/plugins6/linux-x86_64/libpathtools.so
--rw-rw-r--   0 em        (1000) em        (1000)    31624 2024-04-03 07:40:27.000000 csoundengine-2.8.5/csoundengine/data/plugins6/linux-x86_64/libpoly.so
--rw-rw-r--   0 em        (1000) em        (1000)    18392 2024-04-03 07:40:27.000000 csoundengine-2.8.5/csoundengine/data/plugins6/linux-x86_64/librisset.so
--rw-rw-r--   0 em        (1000) em        (1000)    18616 2024-04-03 07:40:27.000000 csoundengine-2.8.5/csoundengine/data/plugins6/linux-x86_64/libsndmeta.so
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-05-01 16:04:10.964024 csoundengine-2.8.5/csoundengine/data/plugins6/macos-arm64/
--rw-rw-r--   0 em        (1000) em        (1000)    67147 2024-04-03 07:40:28.000000 csoundengine-2.8.5/csoundengine/data/plugins6/macos-arm64/libbeosc.dylib
--rw-rw-r--   0 em        (1000) em        (1000)   122938 2024-04-03 07:40:28.000000 csoundengine-2.8.5/csoundengine/data/plugins6/macos-arm64/libelse.dylib
--rw-rw-r--   0 em        (1000) em        (1000)   104074 2024-04-03 07:40:28.000000 csoundengine-2.8.5/csoundengine/data/plugins6/macos-arm64/libklib.dylib
--rw-rw-r--   0 em        (1000) em        (1000)    51231 2024-04-03 07:40:28.000000 csoundengine-2.8.5/csoundengine/data/plugins6/macos-arm64/libpathtools.dylib
--rw-rw-r--   0 em        (1000) em        (1000)    67578 2024-04-03 07:40:28.000000 csoundengine-2.8.5/csoundengine/data/plugins6/macos-arm64/libpoly.dylib
--rw-rw-r--   0 em        (1000) em        (1000)    50588 2024-04-03 07:40:28.000000 csoundengine-2.8.5/csoundengine/data/plugins6/macos-arm64/librisset.dylib
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-05-01 16:04:10.966024 csoundengine-2.8.5/csoundengine/data/plugins6/macos-x86_64/
--rw-rw-r--   0 em        (1000) em        (1000)    66544 2024-04-03 07:40:29.000000 csoundengine-2.8.5/csoundengine/data/plugins6/macos-x86_64/libbeosc.dylib
--rw-rw-r--   0 em        (1000) em        (1000)   138896 2024-04-03 07:40:29.000000 csoundengine-2.8.5/csoundengine/data/plugins6/macos-x86_64/libelse.dylib
--rw-rw-r--   0 em        (1000) em        (1000)   483304 2024-04-03 07:40:29.000000 csoundengine-2.8.5/csoundengine/data/plugins6/macos-x86_64/libjsfx.dylib
--rw-rw-r--   0 em        (1000) em        (1000)   103560 2024-04-03 07:40:29.000000 csoundengine-2.8.5/csoundengine/data/plugins6/macos-x86_64/libklib.dylib
--rw-rw-r--   0 em        (1000) em        (1000)    50784 2024-04-03 07:40:29.000000 csoundengine-2.8.5/csoundengine/data/plugins6/macos-x86_64/libpathtools.dylib
--rw-rw-r--   0 em        (1000) em        (1000)    67016 2024-04-03 07:40:29.000000 csoundengine-2.8.5/csoundengine/data/plugins6/macos-x86_64/libpoly.dylib
--rw-rw-r--   0 em        (1000) em        (1000)    50056 2024-04-03 07:40:29.000000 csoundengine-2.8.5/csoundengine/data/plugins6/macos-x86_64/librisset.dylib
--rw-rw-r--   0 em        (1000) em        (1000)    50080 2024-04-03 07:40:29.000000 csoundengine-2.8.5/csoundengine/data/plugins6/macos-x86_64/libsndmeta.dylib
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-05-01 16:04:10.968024 csoundengine-2.8.5/csoundengine/data/plugins6/windows-x86_64/
--rw-rw-r--   0 em        (1000) em        (1000)    45568 2024-04-03 07:40:29.000000 csoundengine-2.8.5/csoundengine/data/plugins6/windows-x86_64/beosc.dll
--rw-rw-r--   0 em        (1000) em        (1000)    98304 2024-04-03 07:40:29.000000 csoundengine-2.8.5/csoundengine/data/plugins6/windows-x86_64/else.dll
--rw-rw-r--   0 em        (1000) em        (1000)    60928 2024-04-03 07:40:29.000000 csoundengine-2.8.5/csoundengine/data/plugins6/windows-x86_64/klib.dll
--rw-rw-r--   0 em        (1000) em        (1000)    18432 2024-04-03 07:40:29.000000 csoundengine-2.8.5/csoundengine/data/plugins6/windows-x86_64/pathtools.dll
--rw-rw-r--   0 em        (1000) em        (1000)    24576 2024-04-03 07:40:29.000000 csoundengine-2.8.5/csoundengine/data/plugins6/windows-x86_64/poly.dll
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-05-01 16:04:10.955024 csoundengine-2.8.5/csoundengine/data/plugins7/
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-05-01 16:04:10.970024 csoundengine-2.8.5/csoundengine/data/plugins7/linux-x86_64/
--rw-rw-r--   0 em        (1000) em        (1000)    31400 2024-04-03 07:40:30.000000 csoundengine-2.8.5/csoundengine/data/plugins7/linux-x86_64/libbeosc.so
--rw-rw-r--   0 em        (1000) em        (1000)   130864 2024-04-03 07:40:30.000000 csoundengine-2.8.5/csoundengine/data/plugins7/linux-x86_64/libelse.so
--rw-rw-r--   0 em        (1000) em        (1000)   346592 2024-04-03 07:40:30.000000 csoundengine-2.8.5/csoundengine/data/plugins7/linux-x86_64/libjsfx.so
--rw-rw-r--   0 em        (1000) em        (1000)   108568 2024-04-03 07:40:30.000000 csoundengine-2.8.5/csoundengine/data/plugins7/linux-x86_64/libklib.so
--rw-rw-r--   0 em        (1000) em        (1000)    28312 2024-04-03 07:40:30.000000 csoundengine-2.8.5/csoundengine/data/plugins7/linux-x86_64/libpathtools.so
--rw-rw-r--   0 em        (1000) em        (1000)    31624 2024-04-03 07:40:30.000000 csoundengine-2.8.5/csoundengine/data/plugins7/linux-x86_64/libpoly.so
--rw-rw-r--   0 em        (1000) em        (1000)    18392 2024-04-03 07:40:30.000000 csoundengine-2.8.5/csoundengine/data/plugins7/linux-x86_64/librisset.so
--rw-rw-r--   0 em        (1000) em        (1000)    18616 2024-04-03 07:40:30.000000 csoundengine-2.8.5/csoundengine/data/plugins7/linux-x86_64/libsndmeta.so
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-05-01 16:04:10.973024 csoundengine-2.8.5/csoundengine/data/plugins7/macos-x86_64/
--rw-rw-r--   0 em        (1000) em        (1000)    66544 2024-04-03 07:40:31.000000 csoundengine-2.8.5/csoundengine/data/plugins7/macos-x86_64/libbeosc.dylib
--rw-rw-r--   0 em        (1000) em        (1000)   138896 2024-04-03 07:40:31.000000 csoundengine-2.8.5/csoundengine/data/plugins7/macos-x86_64/libelse.dylib
--rw-rw-r--   0 em        (1000) em        (1000)   483304 2024-04-03 07:40:31.000000 csoundengine-2.8.5/csoundengine/data/plugins7/macos-x86_64/libjsfx.dylib
--rw-rw-r--   0 em        (1000) em        (1000)   103560 2024-04-03 07:40:31.000000 csoundengine-2.8.5/csoundengine/data/plugins7/macos-x86_64/libklib.dylib
--rw-rw-r--   0 em        (1000) em        (1000)    50784 2024-04-03 07:40:31.000000 csoundengine-2.8.5/csoundengine/data/plugins7/macos-x86_64/libpathtools.dylib
--rw-rw-r--   0 em        (1000) em        (1000)    67016 2024-04-03 07:40:31.000000 csoundengine-2.8.5/csoundengine/data/plugins7/macos-x86_64/libpoly.dylib
--rw-rw-r--   0 em        (1000) em        (1000)    50056 2024-04-03 07:40:31.000000 csoundengine-2.8.5/csoundengine/data/plugins7/macos-x86_64/librisset.dylib
--rw-rw-r--   0 em        (1000) em        (1000)    50080 2024-04-03 07:40:31.000000 csoundengine-2.8.5/csoundengine/data/plugins7/macos-x86_64/libsndmeta.dylib
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-05-01 16:04:10.974024 csoundengine-2.8.5/csoundengine/data/plugins7/windows-x86_64/
--rw-rw-r--   0 em        (1000) em        (1000)    45568 2024-04-03 07:40:32.000000 csoundengine-2.8.5/csoundengine/data/plugins7/windows-x86_64/beosc.dll
--rw-rw-r--   0 em        (1000) em        (1000)    98304 2024-04-03 07:40:32.000000 csoundengine-2.8.5/csoundengine/data/plugins7/windows-x86_64/else.dll
--rw-rw-r--   0 em        (1000) em        (1000)    60928 2024-04-03 07:40:32.000000 csoundengine-2.8.5/csoundengine/data/plugins7/windows-x86_64/klib.dll
--rw-rw-r--   0 em        (1000) em        (1000)    18432 2024-04-03 07:40:32.000000 csoundengine-2.8.5/csoundengine/data/plugins7/windows-x86_64/pathtools.dll
--rw-rw-r--   0 em        (1000) em        (1000)    24576 2024-04-03 07:40:32.000000 csoundengine-2.8.5/csoundengine/data/plugins7/windows-x86_64/poly.dll
--rw-rw-r--   0 em        (1000) em        (1000)    13367 2024-04-19 12:39:25.000000 csoundengine-2.8.5/csoundengine/dependencies.py
--rwxr-xr-x   0 em        (1000) em        (1000)   154902 2024-04-25 21:36:08.000000 csoundengine-2.8.5/csoundengine/engine.py
--rw-r--r--   0 em        (1000) em        (1000)    24396 2024-04-17 08:14:41.000000 csoundengine-2.8.5/csoundengine/engineorc.py
--rw-rw-r--   0 em        (1000) em        (1000)      145 2023-10-11 21:51:48.000000 csoundengine-2.8.5/csoundengine/errors.py
--rw-r--r--   0 em        (1000) em        (1000)     2686 2024-04-18 10:55:30.000000 csoundengine-2.8.5/csoundengine/event.py
--rw-r--r--   0 em        (1000) em        (1000)    41738 2024-04-18 11:00:12.000000 csoundengine-2.8.5/csoundengine/instr.py
--rw-r--r--   0 em        (1000) em        (1000)    12225 2024-04-23 10:37:57.000000 csoundengine-2.8.5/csoundengine/instrtools.py
--rw-r--r--   0 em        (1000) em        (1000)    10720 2023-11-14 20:14:02.000000 csoundengine-2.8.5/csoundengine/interact.py
--rw-r--r--   0 em        (1000) em        (1000)    21429 2024-04-10 06:06:37.000000 csoundengine-2.8.5/csoundengine/internal.py
--rw-r--r--   0 em        (1000) em        (1000)     4997 2023-11-14 20:14:02.000000 csoundengine-2.8.5/csoundengine/jacktools.py
--rw-rw-r--   0 em        (1000) em        (1000)     3121 2023-10-26 22:00:07.000000 csoundengine-2.8.5/csoundengine/jupytertools.py
--rw-r--r--   0 em        (1000) em        (1000)     4517 2024-04-17 08:24:52.000000 csoundengine-2.8.5/csoundengine/linuxaudio.py
--rw-r--r--   0 em        (1000) em        (1000)     5815 2023-11-14 20:14:02.000000 csoundengine-2.8.5/csoundengine/magic.py
--rw-r--r--   0 em        (1000) em        (1000)    68303 2024-05-01 15:58:47.000000 csoundengine-2.8.5/csoundengine/offline.py
--rw-rw-r--   0 em        (1000) em        (1000)     5690 2023-11-01 14:45:02.000000 csoundengine-2.8.5/csoundengine/offlineorc.py
--rw-rw-r--   0 em        (1000) em        (1000)     6007 2023-10-11 21:51:48.000000 csoundengine-2.8.5/csoundengine/paramtable.py
--rwxrwxr-x   0 em        (1000) em        (1000)     7787 2024-04-17 07:56:12.000000 csoundengine-2.8.5/csoundengine/plotting.py
--rw-rw-r--   0 em        (1000) em        (1000)        0 2021-11-13 21:37:59.000000 csoundengine-2.8.5/csoundengine/py.typed
--rw-r--r--   0 em        (1000) em        (1000)    15152 2024-04-25 19:27:37.000000 csoundengine-2.8.5/csoundengine/schedevent.py
--rw-r--r--   0 em        (1000) em        (1000)    82528 2024-04-25 20:08:07.000000 csoundengine-2.8.5/csoundengine/session.py
--rw-rw-r--   0 em        (1000) em        (1000)      779 2024-03-28 17:26:41.000000 csoundengine-2.8.5/csoundengine/sessionhandler.py
--rw-r--r--   0 em        (1000) em        (1000)     8113 2024-04-23 21:31:04.000000 csoundengine-2.8.5/csoundengine/sessioninstrs.py
--rw-rw-r--   0 em        (1000) em        (1000)     1996 2024-04-19 11:09:00.000000 csoundengine-2.8.5/csoundengine/state.py
--rw-r--r--   0 em        (1000) em        (1000)    34694 2024-04-25 10:56:50.000000 csoundengine-2.8.5/csoundengine/synth.py
--rw-r--r--   0 em        (1000) em        (1000)     5965 2023-11-14 20:14:02.000000 csoundengine-2.8.5/csoundengine/tableproxy.py
--rw-rw-r--   0 em        (1000) em        (1000)      600 2022-09-25 13:10:18.000000 csoundengine-2.8.5/csoundengine/termui.py
--rw-rw-r--   0 em        (1000) em        (1000)     3101 2024-04-16 11:20:08.000000 csoundengine-2.8.5/csoundengine/tools.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-05-01 16:04:10.975024 csoundengine-2.8.5/csoundengine.egg-info/
--rw-r--r--   0 em        (1000) em        (1000)     6749 2024-05-01 16:04:10.000000 csoundengine-2.8.5/csoundengine.egg-info/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)     3778 2024-05-01 16:04:10.000000 csoundengine-2.8.5/csoundengine.egg-info/SOURCES.txt
--rw-rw-r--   0 em        (1000) em        (1000)        1 2024-05-01 16:04:10.000000 csoundengine-2.8.5/csoundengine.egg-info/dependency_links.txt
--rw-rw-r--   0 em        (1000) em        (1000)        1 2022-02-17 19:50:17.000000 csoundengine-2.8.5/csoundengine.egg-info/not-zip-safe
--rw-rw-r--   0 em        (1000) em        (1000)      277 2024-05-01 16:04:10.000000 csoundengine-2.8.5/csoundengine.egg-info/requires.txt
--rw-rw-r--   0 em        (1000) em        (1000)       13 2024-05-01 16:04:10.000000 csoundengine-2.8.5/csoundengine.egg-info/top_level.txt
--rw-rw-r--   0 em        (1000) em        (1000)       38 2024-05-01 16:04:10.976024 csoundengine-2.8.5/setup.cfg
--rwxrwxr-x   0 em        (1000) em        (1000)     1754 2024-05-01 16:02:30.000000 csoundengine-2.8.5/setup.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-05-01 16:04:10.975024 csoundengine-2.8.5/test/
--rw-rw-r--   0 em        (1000) em        (1000)      719 2024-04-26 06:47:12.000000 csoundengine-2.8.5/test/test1.py
--rw-rw-r--   0 em        (1000) em        (1000)     1088 2024-04-26 07:12:43.000000 csoundengine-2.8.5/test/test2.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-05-20 18:47:27.096485 csoundengine-2.9.0/
+-rw-rw-r--   0 em        (1000) em        (1000)    35128 2021-11-13 21:37:59.000000 csoundengine-2.9.0/LICENSE.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       24 2021-11-13 21:37:59.000000 csoundengine-2.9.0/MANIFEST.in
+-rw-r--r--   0 em        (1000) em        (1000)     6749 2024-05-20 18:47:27.096485 csoundengine-2.9.0/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)     5728 2024-01-10 12:24:51.000000 csoundengine-2.9.0/README.rst
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-05-20 18:47:27.065484 csoundengine-2.9.0/csoundengine/
+-rw-r--r--   0 em        (1000) em        (1000)     4112 2024-05-20 10:09:52.000000 csoundengine-2.9.0/csoundengine/__init__.py
+-rw-rw-r--   0 em        (1000) em        (1000)     1055 2023-03-14 09:38:54.000000 csoundengine-2.9.0/csoundengine/__sessionbase.py
+-rw-r--r--   0 em        (1000) em        (1000)      177 2023-11-24 08:20:24.000000 csoundengine-2.9.0/csoundengine/_common.py
+-rw-r--r--   0 em        (1000) em        (1000)     6244 2024-04-25 07:47:16.000000 csoundengine-2.9.0/csoundengine/abstractrenderer.py
+-rw-r--r--   0 em        (1000) em        (1000)    12846 2024-04-25 19:14:45.000000 csoundengine-2.9.0/csoundengine/baseschedevent.py
+-rw-rw-r--   0 em        (1000) em        (1000)     5848 2024-04-17 08:24:25.000000 csoundengine-2.9.0/csoundengine/busproxy.py
+-rw-r--r--   0 em        (1000) em        (1000)     8470 2024-04-25 08:46:55.000000 csoundengine-2.9.0/csoundengine/config.py
+-rw-rw-r--   0 em        (1000) em        (1000)        0 2023-10-17 11:02:49.000000 csoundengine-2.9.0/csoundengine/contants.py
+-rwxr-xr-x   0 em        (1000) em        (1000)   128690 2024-05-20 18:23:30.000000 csoundengine-2.9.0/csoundengine/csoundlib.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-05-20 18:47:27.054484 csoundengine-2.9.0/csoundengine/data/
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-05-20 18:47:27.053484 csoundengine-2.9.0/csoundengine/data/plugins6/
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-05-20 18:47:27.071484 csoundengine-2.9.0/csoundengine/data/plugins6/linux-x86_64/
+-rw-rw-r--   0 em        (1000) em        (1000)    31400 2024-04-03 07:40:27.000000 csoundengine-2.9.0/csoundengine/data/plugins6/linux-x86_64/libbeosc.so
+-rw-rw-r--   0 em        (1000) em        (1000)   130864 2024-04-03 07:40:27.000000 csoundengine-2.9.0/csoundengine/data/plugins6/linux-x86_64/libelse.so
+-rw-rw-r--   0 em        (1000) em        (1000)   346592 2024-04-03 07:40:27.000000 csoundengine-2.9.0/csoundengine/data/plugins6/linux-x86_64/libjsfx.so
+-rw-rw-r--   0 em        (1000) em        (1000)   108568 2024-04-03 07:40:27.000000 csoundengine-2.9.0/csoundengine/data/plugins6/linux-x86_64/libklib.so
+-rw-rw-r--   0 em        (1000) em        (1000)    28312 2024-04-03 07:40:27.000000 csoundengine-2.9.0/csoundengine/data/plugins6/linux-x86_64/libpathtools.so
+-rw-rw-r--   0 em        (1000) em        (1000)    31624 2024-04-03 07:40:27.000000 csoundengine-2.9.0/csoundengine/data/plugins6/linux-x86_64/libpoly.so
+-rw-rw-r--   0 em        (1000) em        (1000)    18392 2024-04-03 07:40:27.000000 csoundengine-2.9.0/csoundengine/data/plugins6/linux-x86_64/librisset.so
+-rw-rw-r--   0 em        (1000) em        (1000)    18616 2024-04-03 07:40:27.000000 csoundengine-2.9.0/csoundengine/data/plugins6/linux-x86_64/libsndmeta.so
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-05-20 18:47:27.074484 csoundengine-2.9.0/csoundengine/data/plugins6/macos-arm64/
+-rw-rw-r--   0 em        (1000) em        (1000)    67147 2024-04-03 07:40:28.000000 csoundengine-2.9.0/csoundengine/data/plugins6/macos-arm64/libbeosc.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)   122938 2024-04-03 07:40:28.000000 csoundengine-2.9.0/csoundengine/data/plugins6/macos-arm64/libelse.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)   104074 2024-04-03 07:40:28.000000 csoundengine-2.9.0/csoundengine/data/plugins6/macos-arm64/libklib.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)    51231 2024-04-03 07:40:28.000000 csoundengine-2.9.0/csoundengine/data/plugins6/macos-arm64/libpathtools.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)    67578 2024-04-03 07:40:28.000000 csoundengine-2.9.0/csoundengine/data/plugins6/macos-arm64/libpoly.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)    50588 2024-04-03 07:40:28.000000 csoundengine-2.9.0/csoundengine/data/plugins6/macos-arm64/librisset.dylib
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-05-20 18:47:27.079485 csoundengine-2.9.0/csoundengine/data/plugins6/macos-x86_64/
+-rw-rw-r--   0 em        (1000) em        (1000)    66544 2024-04-03 07:40:29.000000 csoundengine-2.9.0/csoundengine/data/plugins6/macos-x86_64/libbeosc.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)   138896 2024-04-03 07:40:29.000000 csoundengine-2.9.0/csoundengine/data/plugins6/macos-x86_64/libelse.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)   483304 2024-04-03 07:40:29.000000 csoundengine-2.9.0/csoundengine/data/plugins6/macos-x86_64/libjsfx.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)   103560 2024-04-03 07:40:29.000000 csoundengine-2.9.0/csoundengine/data/plugins6/macos-x86_64/libklib.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)    50784 2024-04-03 07:40:29.000000 csoundengine-2.9.0/csoundengine/data/plugins6/macos-x86_64/libpathtools.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)    67016 2024-04-03 07:40:29.000000 csoundengine-2.9.0/csoundengine/data/plugins6/macos-x86_64/libpoly.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)    50056 2024-04-03 07:40:29.000000 csoundengine-2.9.0/csoundengine/data/plugins6/macos-x86_64/librisset.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)    50080 2024-04-03 07:40:29.000000 csoundengine-2.9.0/csoundengine/data/plugins6/macos-x86_64/libsndmeta.dylib
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-05-20 18:47:27.082485 csoundengine-2.9.0/csoundengine/data/plugins6/windows-x86_64/
+-rw-rw-r--   0 em        (1000) em        (1000)    45568 2024-04-03 07:40:29.000000 csoundengine-2.9.0/csoundengine/data/plugins6/windows-x86_64/beosc.dll
+-rw-rw-r--   0 em        (1000) em        (1000)    98304 2024-04-03 07:40:29.000000 csoundengine-2.9.0/csoundengine/data/plugins6/windows-x86_64/else.dll
+-rw-rw-r--   0 em        (1000) em        (1000)    60928 2024-04-03 07:40:29.000000 csoundengine-2.9.0/csoundengine/data/plugins6/windows-x86_64/klib.dll
+-rw-rw-r--   0 em        (1000) em        (1000)    18432 2024-04-03 07:40:29.000000 csoundengine-2.9.0/csoundengine/data/plugins6/windows-x86_64/pathtools.dll
+-rw-rw-r--   0 em        (1000) em        (1000)    24576 2024-04-03 07:40:29.000000 csoundengine-2.9.0/csoundengine/data/plugins6/windows-x86_64/poly.dll
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-05-20 18:47:27.054484 csoundengine-2.9.0/csoundengine/data/plugins7/
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-05-20 18:47:27.087484 csoundengine-2.9.0/csoundengine/data/plugins7/linux-x86_64/
+-rw-rw-r--   0 em        (1000) em        (1000)    31400 2024-04-03 07:40:30.000000 csoundengine-2.9.0/csoundengine/data/plugins7/linux-x86_64/libbeosc.so
+-rw-rw-r--   0 em        (1000) em        (1000)   130864 2024-04-03 07:40:30.000000 csoundengine-2.9.0/csoundengine/data/plugins7/linux-x86_64/libelse.so
+-rw-rw-r--   0 em        (1000) em        (1000)   346592 2024-04-03 07:40:30.000000 csoundengine-2.9.0/csoundengine/data/plugins7/linux-x86_64/libjsfx.so
+-rw-rw-r--   0 em        (1000) em        (1000)   108568 2024-04-03 07:40:30.000000 csoundengine-2.9.0/csoundengine/data/plugins7/linux-x86_64/libklib.so
+-rw-rw-r--   0 em        (1000) em        (1000)    28312 2024-04-03 07:40:30.000000 csoundengine-2.9.0/csoundengine/data/plugins7/linux-x86_64/libpathtools.so
+-rw-rw-r--   0 em        (1000) em        (1000)    31624 2024-04-03 07:40:30.000000 csoundengine-2.9.0/csoundengine/data/plugins7/linux-x86_64/libpoly.so
+-rw-rw-r--   0 em        (1000) em        (1000)    18392 2024-04-03 07:40:30.000000 csoundengine-2.9.0/csoundengine/data/plugins7/linux-x86_64/librisset.so
+-rw-rw-r--   0 em        (1000) em        (1000)    18616 2024-04-03 07:40:30.000000 csoundengine-2.9.0/csoundengine/data/plugins7/linux-x86_64/libsndmeta.so
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-05-20 18:47:27.092485 csoundengine-2.9.0/csoundengine/data/plugins7/macos-x86_64/
+-rw-rw-r--   0 em        (1000) em        (1000)    66544 2024-04-03 07:40:31.000000 csoundengine-2.9.0/csoundengine/data/plugins7/macos-x86_64/libbeosc.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)   138896 2024-04-03 07:40:31.000000 csoundengine-2.9.0/csoundengine/data/plugins7/macos-x86_64/libelse.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)   483304 2024-04-03 07:40:31.000000 csoundengine-2.9.0/csoundengine/data/plugins7/macos-x86_64/libjsfx.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)   103560 2024-04-03 07:40:31.000000 csoundengine-2.9.0/csoundengine/data/plugins7/macos-x86_64/libklib.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)    50784 2024-04-03 07:40:31.000000 csoundengine-2.9.0/csoundengine/data/plugins7/macos-x86_64/libpathtools.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)    67016 2024-04-03 07:40:31.000000 csoundengine-2.9.0/csoundengine/data/plugins7/macos-x86_64/libpoly.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)    50056 2024-04-03 07:40:31.000000 csoundengine-2.9.0/csoundengine/data/plugins7/macos-x86_64/librisset.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)    50080 2024-04-03 07:40:31.000000 csoundengine-2.9.0/csoundengine/data/plugins7/macos-x86_64/libsndmeta.dylib
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-05-20 18:47:27.095485 csoundengine-2.9.0/csoundengine/data/plugins7/windows-x86_64/
+-rw-rw-r--   0 em        (1000) em        (1000)    45568 2024-04-03 07:40:32.000000 csoundengine-2.9.0/csoundengine/data/plugins7/windows-x86_64/beosc.dll
+-rw-rw-r--   0 em        (1000) em        (1000)    98304 2024-04-03 07:40:32.000000 csoundengine-2.9.0/csoundengine/data/plugins7/windows-x86_64/else.dll
+-rw-rw-r--   0 em        (1000) em        (1000)    60928 2024-04-03 07:40:32.000000 csoundengine-2.9.0/csoundengine/data/plugins7/windows-x86_64/klib.dll
+-rw-rw-r--   0 em        (1000) em        (1000)    18432 2024-04-03 07:40:32.000000 csoundengine-2.9.0/csoundengine/data/plugins7/windows-x86_64/pathtools.dll
+-rw-rw-r--   0 em        (1000) em        (1000)    24576 2024-04-03 07:40:32.000000 csoundengine-2.9.0/csoundengine/data/plugins7/windows-x86_64/poly.dll
+-rw-rw-r--   0 em        (1000) em        (1000)    13367 2024-04-19 12:39:25.000000 csoundengine-2.9.0/csoundengine/dependencies.py
+-rwxr-xr-x   0 em        (1000) em        (1000)   155036 2024-05-20 09:56:09.000000 csoundengine-2.9.0/csoundengine/engine.py
+-rw-r--r--   0 em        (1000) em        (1000)    24396 2024-04-17 08:14:41.000000 csoundengine-2.9.0/csoundengine/engineorc.py
+-rw-rw-r--   0 em        (1000) em        (1000)      145 2023-10-11 21:51:48.000000 csoundengine-2.9.0/csoundengine/errors.py
+-rw-r--r--   0 em        (1000) em        (1000)     2686 2024-04-18 10:55:30.000000 csoundengine-2.9.0/csoundengine/event.py
+-rw-r--r--   0 em        (1000) em        (1000)    41738 2024-04-18 11:00:12.000000 csoundengine-2.9.0/csoundengine/instr.py
+-rw-r--r--   0 em        (1000) em        (1000)    12225 2024-04-23 10:37:57.000000 csoundengine-2.9.0/csoundengine/instrtools.py
+-rw-r--r--   0 em        (1000) em        (1000)    10720 2023-11-14 20:14:02.000000 csoundengine-2.9.0/csoundengine/interact.py
+-rw-r--r--   0 em        (1000) em        (1000)    21429 2024-04-10 06:06:37.000000 csoundengine-2.9.0/csoundengine/internal.py
+-rw-r--r--   0 em        (1000) em        (1000)     4997 2023-11-14 20:14:02.000000 csoundengine-2.9.0/csoundengine/jacktools.py
+-rw-rw-r--   0 em        (1000) em        (1000)     3121 2023-10-26 22:00:07.000000 csoundengine-2.9.0/csoundengine/jupytertools.py
+-rw-r--r--   0 em        (1000) em        (1000)     4517 2024-04-17 08:24:52.000000 csoundengine-2.9.0/csoundengine/linuxaudio.py
+-rw-r--r--   0 em        (1000) em        (1000)     5815 2023-11-14 20:14:02.000000 csoundengine-2.9.0/csoundengine/magic.py
+-rw-r--r--   0 em        (1000) em        (1000)    75218 2024-05-20 10:13:07.000000 csoundengine-2.9.0/csoundengine/offline.py
+-rw-rw-r--   0 em        (1000) em        (1000)     5690 2023-11-01 14:45:02.000000 csoundengine-2.9.0/csoundengine/offlineorc.py
+-rw-rw-r--   0 em        (1000) em        (1000)     6007 2023-10-11 21:51:48.000000 csoundengine-2.9.0/csoundengine/paramtable.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     7787 2024-04-17 07:56:12.000000 csoundengine-2.9.0/csoundengine/plotting.py
+-rw-rw-r--   0 em        (1000) em        (1000)        0 2021-11-13 21:37:59.000000 csoundengine-2.9.0/csoundengine/py.typed
+-rw-r--r--   0 em        (1000) em        (1000)    15152 2024-04-25 19:27:37.000000 csoundengine-2.9.0/csoundengine/schedevent.py
+-rw-r--r--   0 em        (1000) em        (1000)    82528 2024-04-25 20:08:07.000000 csoundengine-2.9.0/csoundengine/session.py
+-rw-rw-r--   0 em        (1000) em        (1000)      779 2024-03-28 17:26:41.000000 csoundengine-2.9.0/csoundengine/sessionhandler.py
+-rw-r--r--   0 em        (1000) em        (1000)     8113 2024-04-23 21:31:04.000000 csoundengine-2.9.0/csoundengine/sessioninstrs.py
+-rw-rw-r--   0 em        (1000) em        (1000)     1996 2024-04-19 11:09:00.000000 csoundengine-2.9.0/csoundengine/state.py
+-rw-r--r--   0 em        (1000) em        (1000)    34694 2024-04-25 10:56:50.000000 csoundengine-2.9.0/csoundengine/synth.py
+-rw-r--r--   0 em        (1000) em        (1000)     5965 2023-11-14 20:14:02.000000 csoundengine-2.9.0/csoundengine/tableproxy.py
+-rw-rw-r--   0 em        (1000) em        (1000)      657 2024-05-07 11:58:10.000000 csoundengine-2.9.0/csoundengine/termui.py
+-rw-rw-r--   0 em        (1000) em        (1000)     3101 2024-04-16 11:20:08.000000 csoundengine-2.9.0/csoundengine/tools.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-05-20 18:47:27.095485 csoundengine-2.9.0/csoundengine.egg-info/
+-rw-r--r--   0 em        (1000) em        (1000)     6749 2024-05-20 18:47:27.000000 csoundengine-2.9.0/csoundengine.egg-info/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)     3778 2024-05-20 18:47:27.000000 csoundengine-2.9.0/csoundengine.egg-info/SOURCES.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        1 2024-05-20 18:47:27.000000 csoundengine-2.9.0/csoundengine.egg-info/dependency_links.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        1 2022-02-17 19:50:17.000000 csoundengine-2.9.0/csoundengine.egg-info/not-zip-safe
+-rw-rw-r--   0 em        (1000) em        (1000)      277 2024-05-20 18:47:27.000000 csoundengine-2.9.0/csoundengine.egg-info/requires.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       13 2024-05-20 18:47:27.000000 csoundengine-2.9.0/csoundengine.egg-info/top_level.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       38 2024-05-20 18:47:27.096485 csoundengine-2.9.0/setup.cfg
+-rwxrwxr-x   0 em        (1000) em        (1000)     1754 2024-05-20 18:46:59.000000 csoundengine-2.9.0/setup.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-05-20 18:47:27.095485 csoundengine-2.9.0/test/
+-rw-rw-r--   0 em        (1000) em        (1000)      719 2024-04-26 06:47:12.000000 csoundengine-2.9.0/test/test1.py
+-rw-rw-r--   0 em        (1000) em        (1000)     1088 2024-04-26 07:12:43.000000 csoundengine-2.9.0/test/test2.py
```

### Comparing `csoundengine-2.8.5/LICENSE.txt` & `csoundengine-2.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/PKG-INFO` & `csoundengine-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csoundengine
-Version: 2.8.5
+Version: 2.9.0
 Summary: A synthesis framework using csound
 Home-page: https://github.com/gesellkammer/csoundengine
 Author: Eduardo Moguillansky
 Author-email: eduardo.moguillansky@gmail.com
 License: BSD
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -21,15 +21,15 @@
 Requires-Dist: ipywidgets
 Requires-Dist: progressbar2
 Requires-Dist: xxhash
 Requires-Dist: docstring_parser
 Requires-Dist: typing_extensions
 Requires-Dist: ctcsound7>=0.4.6
 Requires-Dist: sndfileio>=1.9.4
-Requires-Dist: emlib>=1.14.1
+Requires-Dist: emlib>=1.15.0
 Requires-Dist: configdict>=2.10.0
 Requires-Dist: bpf4>=1.10.1
 Requires-Dist: numpyx>=1.3.3
 Requires-Dist: pitchtools>=1.14.0
 Requires-Dist: risset>=2.9.1
 Requires-Dist: sounddevice
```

### Comparing `csoundengine-2.8.5/README.rst` & `csoundengine-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/__init__.py` & `csoundengine-2.9.0/csoundengine/__init__.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/__sessionbase.py` & `csoundengine-2.9.0/csoundengine/__sessionbase.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/abstractrenderer.py` & `csoundengine-2.9.0/csoundengine/abstractrenderer.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/baseschedevent.py` & `csoundengine-2.9.0/csoundengine/baseschedevent.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/busproxy.py` & `csoundengine-2.9.0/csoundengine/busproxy.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/config.py` & `csoundengine-2.9.0/csoundengine/config.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/csoundlib.py` & `csoundengine-2.9.0/csoundengine/csoundlib.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,38 +16,39 @@
 import os as _os
 import sys
 import subprocess as _subprocess
 import re as _re
 import shutil as _shutil
 import logging as _logging
 import textwrap as _textwrap
+import functools as _functools
 import io as _io
 from pathlib import Path as _Path
 import tempfile as _tempfile
-import cachetools as _cachetools
 import dataclasses
+import cachetools as _cachetools
+import numpy as np
 
 from ._common import *
 from csoundengine import jacktools
 from csoundengine import linuxaudio
 from csoundengine import state as _state
 from csoundengine.config import config
 from csoundengine.internal import normalizePlatform
-import functools as _functools
 import emlib.misc
 import emlib.textlib
 import emlib.dialogs
 import emlib.mathlib
 from emlib.common import runonce
-import numpy as np
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from typing import Callable, Sequence, Iterator, Any, Set
     Curve = Callable[[float], float]
+    from sf2utils.sf2parse import Sf2File
 
 
 try:
     import ctcsound7 as ctcsound
 except Exception as e:
     if 'sphinx' in sys.modules:
         print("Called while building sphinx documentation?")
@@ -248,15 +249,14 @@
 
     def bufferSizeAndNum(self) -> tuple[int, int]:
         """
         The buffer size and number of buffers needed for this backend
         """
         return (self.defaultBufferSize, self.defaultNumBuffers)
 
-    # @_functools.cache
     def audioDevices(self) -> tuple[list[AudioDevice], list[AudioDevice]]:
         """
         Query csound for audio devices for this backend
 
         Returns:
             a tuple (inputDevices: list[AudioDevice], outputDevices: list[AudioDevice])
         """
@@ -3529,14 +3529,21 @@
         >>> idx.nameToIndex
         {'piano': 0}
     """
     return SoundFontIndex(sfpath)
 
 
 @_functools.cache
+def _sf2file(path: str) -> Sf2File:
+    from sf2utils.sf2parse import Sf2File
+    f = open(path, 'rb')
+    return Sf2File(f)
+
+
+@_functools.cache
 def _soundfontInstrumentsAndPresets(sfpath: str
                                     ) -> tuple[list[tuple[int, str]],
                                                list[tuple[int, int, str]]]:
     """
     Returns a tuple (instruments, presets)
 
     Where instruments is a list of tuples(instridx, instrname) and presets
@@ -3546,17 +3553,15 @@
         sfpath: the path to the soundfont
 
     Returns:
         a tuple (instruments, presets), where instruments is a list
         of tuples (instrindex, instrname) and prests is a list of
         tuples (bank, presetindex, name)
     """
-    from sf2utils.sf2parse import Sf2File
-    f = open(sfpath, 'rb')
-    sf = Sf2File(f)
+    sf = _sf2file(sfpath)
     instruments: list[tuple[int, str]] = [(num, instr.name.strip())
                                           for num, instr in enumerate(sf.instruments)
                                           if instr.name and instr.name != 'EOI']
     presets: list[tuple[int, int, str]] = [(p.bank, p.preset, p.name.strip())
                                            for p in sf.presets
                                            if p.name and p.name != 'EOP']
     presets.sort()
@@ -3638,14 +3643,66 @@
     """
     if sfpath == "?":
         sfpath = _state.openSoundfont(ensureSelection=True)
     sfindex = soundfontIndex(sfpath)
     return sfindex.nameToIndex.get(name)
 
 
+@_functools.cache
+def soundfontKeyrange(sfpath: str, preset: tuple[int, int]) -> tuple[int, int] | None:
+    sf = _sf2file(sfpath)
+    for p in sf.presets:
+        if p.bank == preset[0] and p.preset == preset[1]:
+            return p.key_range.start, p.key_range.stop
+    return None
+
+
+def soundfontPeak(sfpath: str, preset: tuple[int, int], pitches: tuple[int, int] = None, dur=0.05
+                  ) -> float:
+    from csoundengine.offline import OfflineEngine
+    e = OfflineEngine(nchnls=0, ksmps=128, numAudioBuses=0, numControlBuses=0)
+    bank, prog = preset
+    presetnum = 1
+    if pitches is None:
+        keyrange = soundfontKeyrange(sfpath, preset)
+        if not keyrange:
+            raise ValueError(f"No defined key range for preset {preset} in soundfont {sfpath}")
+        minpitch, maxpitch = keyrange
+        pitch1 = int((maxpitch - minpitch) * 0.2 + minpitch)
+        pitch2 = int((maxpitch - minpitch) * 0.8 + minpitch)
+        pitches = (pitch1, pitch2)
+    e.compile(fr'''
+    gi_sfhandle sfload "{sfpath}"
+    gi_presetindex sfpreset {prog}, {bank}, gi_sfhandle, {presetnum}
+    chnset 0, "sfpeak"
+    
+    instr sfpeak
+        ipreset = p4
+        ipitch1 = p5
+        ipitch2 = p6
+        kmax0 init 0
+        a1 sfplaym 127, ipitch1, 1, 1, ipreset, 0
+        a2 sfplaym 127, ipitch2, 1, 1, ipreset, 0
+        kmax1 peak a1
+        kmax2 peak a2
+        kmax = max(kmax1, kmax2)
+        if kmax > kmax0 then
+            chnset kmax, "sfpeak"
+        endif
+        kmax0 = kmax
+    endin
+    ''')
+
+    e.sched('sfpeak', 0, dur, (presetnum, pitches[0], pitches[1]))
+    e.perform(extratime=0.1)
+    value, error = e.csound.controlChannel("sfpeak")
+    e.stop()
+    return float(value)
+
+
 def splitInclude(line: str) -> str:
     """
     Given an include line it splits the include path
 
     Example
     ~~~~~~~
```

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins6/linux-x86_64/libbeosc.so` & `csoundengine-2.9.0/csoundengine/data/plugins6/linux-x86_64/libbeosc.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins6/linux-x86_64/libelse.so` & `csoundengine-2.9.0/csoundengine/data/plugins6/linux-x86_64/libelse.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins6/linux-x86_64/libjsfx.so` & `csoundengine-2.9.0/csoundengine/data/plugins6/linux-x86_64/libjsfx.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins6/linux-x86_64/libklib.so` & `csoundengine-2.9.0/csoundengine/data/plugins6/linux-x86_64/libklib.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins6/linux-x86_64/libpathtools.so` & `csoundengine-2.9.0/csoundengine/data/plugins6/linux-x86_64/libpathtools.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins6/linux-x86_64/libpoly.so` & `csoundengine-2.9.0/csoundengine/data/plugins6/linux-x86_64/libpoly.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins6/linux-x86_64/librisset.so` & `csoundengine-2.9.0/csoundengine/data/plugins6/linux-x86_64/librisset.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins6/linux-x86_64/libsndmeta.so` & `csoundengine-2.9.0/csoundengine/data/plugins6/linux-x86_64/libsndmeta.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins6/macos-arm64/libbeosc.dylib` & `csoundengine-2.9.0/csoundengine/data/plugins6/macos-arm64/libbeosc.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins6/macos-arm64/libelse.dylib` & `csoundengine-2.9.0/csoundengine/data/plugins6/macos-arm64/libelse.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins6/macos-arm64/libklib.dylib` & `csoundengine-2.9.0/csoundengine/data/plugins6/macos-arm64/libklib.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins6/macos-arm64/libpathtools.dylib` & `csoundengine-2.9.0/csoundengine/data/plugins6/macos-arm64/libpathtools.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins6/macos-arm64/libpoly.dylib` & `csoundengine-2.9.0/csoundengine/data/plugins6/macos-arm64/libpoly.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins6/macos-arm64/librisset.dylib` & `csoundengine-2.9.0/csoundengine/data/plugins6/macos-arm64/librisset.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins6/macos-x86_64/libbeosc.dylib` & `csoundengine-2.9.0/csoundengine/data/plugins6/macos-x86_64/libbeosc.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins6/macos-x86_64/libelse.dylib` & `csoundengine-2.9.0/csoundengine/data/plugins6/macos-x86_64/libelse.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins6/macos-x86_64/libjsfx.dylib` & `csoundengine-2.9.0/csoundengine/data/plugins6/macos-x86_64/libjsfx.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins6/macos-x86_64/libklib.dylib` & `csoundengine-2.9.0/csoundengine/data/plugins6/macos-x86_64/libklib.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins6/macos-x86_64/libpathtools.dylib` & `csoundengine-2.9.0/csoundengine/data/plugins6/macos-x86_64/libpathtools.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins6/macos-x86_64/libpoly.dylib` & `csoundengine-2.9.0/csoundengine/data/plugins6/macos-x86_64/libpoly.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins6/macos-x86_64/librisset.dylib` & `csoundengine-2.9.0/csoundengine/data/plugins6/macos-x86_64/librisset.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins6/macos-x86_64/libsndmeta.dylib` & `csoundengine-2.9.0/csoundengine/data/plugins6/macos-x86_64/libsndmeta.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins6/windows-x86_64/beosc.dll` & `csoundengine-2.9.0/csoundengine/data/plugins6/windows-x86_64/beosc.dll`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins6/windows-x86_64/else.dll` & `csoundengine-2.9.0/csoundengine/data/plugins6/windows-x86_64/else.dll`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins6/windows-x86_64/klib.dll` & `csoundengine-2.9.0/csoundengine/data/plugins6/windows-x86_64/klib.dll`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins6/windows-x86_64/pathtools.dll` & `csoundengine-2.9.0/csoundengine/data/plugins6/windows-x86_64/pathtools.dll`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins6/windows-x86_64/poly.dll` & `csoundengine-2.9.0/csoundengine/data/plugins6/windows-x86_64/poly.dll`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins7/linux-x86_64/libbeosc.so` & `csoundengine-2.9.0/csoundengine/data/plugins7/linux-x86_64/libbeosc.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins7/linux-x86_64/libelse.so` & `csoundengine-2.9.0/csoundengine/data/plugins7/linux-x86_64/libelse.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins7/linux-x86_64/libjsfx.so` & `csoundengine-2.9.0/csoundengine/data/plugins7/linux-x86_64/libjsfx.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins7/linux-x86_64/libklib.so` & `csoundengine-2.9.0/csoundengine/data/plugins7/linux-x86_64/libklib.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins7/linux-x86_64/libpathtools.so` & `csoundengine-2.9.0/csoundengine/data/plugins7/linux-x86_64/libpathtools.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins7/linux-x86_64/libpoly.so` & `csoundengine-2.9.0/csoundengine/data/plugins7/linux-x86_64/libpoly.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins7/linux-x86_64/librisset.so` & `csoundengine-2.9.0/csoundengine/data/plugins7/linux-x86_64/librisset.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins7/linux-x86_64/libsndmeta.so` & `csoundengine-2.9.0/csoundengine/data/plugins7/linux-x86_64/libsndmeta.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins7/macos-x86_64/libbeosc.dylib` & `csoundengine-2.9.0/csoundengine/data/plugins7/macos-x86_64/libbeosc.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins7/macos-x86_64/libelse.dylib` & `csoundengine-2.9.0/csoundengine/data/plugins7/macos-x86_64/libelse.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins7/macos-x86_64/libjsfx.dylib` & `csoundengine-2.9.0/csoundengine/data/plugins7/macos-x86_64/libjsfx.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins7/macos-x86_64/libklib.dylib` & `csoundengine-2.9.0/csoundengine/data/plugins7/macos-x86_64/libklib.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins7/macos-x86_64/libpathtools.dylib` & `csoundengine-2.9.0/csoundengine/data/plugins7/macos-x86_64/libpathtools.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins7/macos-x86_64/libpoly.dylib` & `csoundengine-2.9.0/csoundengine/data/plugins7/macos-x86_64/libpoly.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins7/macos-x86_64/librisset.dylib` & `csoundengine-2.9.0/csoundengine/data/plugins7/macos-x86_64/librisset.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins7/macos-x86_64/libsndmeta.dylib` & `csoundengine-2.9.0/csoundengine/data/plugins7/macos-x86_64/libsndmeta.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins7/windows-x86_64/beosc.dll` & `csoundengine-2.9.0/csoundengine/data/plugins7/windows-x86_64/beosc.dll`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins7/windows-x86_64/else.dll` & `csoundengine-2.9.0/csoundengine/data/plugins7/windows-x86_64/else.dll`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins7/windows-x86_64/klib.dll` & `csoundengine-2.9.0/csoundengine/data/plugins7/windows-x86_64/klib.dll`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins7/windows-x86_64/pathtools.dll` & `csoundengine-2.9.0/csoundengine/data/plugins7/windows-x86_64/pathtools.dll`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/data/plugins7/windows-x86_64/poly.dll` & `csoundengine-2.9.0/csoundengine/data/plugins7/windows-x86_64/poly.dll`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/dependencies.py` & `csoundengine-2.9.0/csoundengine/dependencies.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/engine.py` & `csoundengine-2.9.0/csoundengine/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -340,14 +340,15 @@
                  udpport: int = 0,
                  commandlineOptions: list[str] | None = None,
                  includes: list[str] | None = None,
                  midibackend: str = 'default',
                  midiin: str | None = None,
                  autosync=False,
                  latency: float | None = None,
+                 sampleAccurate: bool = None,
                  numthreads: int = 0):
         if not name:
             name = _generateUniqueEngineName()
         elif name in Engine.activeEngines:
             raise KeyError(f"Engine '{name}' already exists")
 
         if backend == 'portaudio':
@@ -493,14 +494,18 @@
 
         if quiet is None:
             quiet = cfg['suppress_output']
 
         if quiet:
             commandlineOptions.append('-m0')
             commandlineOptions.append('-d')
+
+        if sampleAccurate:
+            commandlineOptions.append('--sample-accurate')
+
         self.name = name
         "Name of this Engine"
 
         assert sr is not None and sr > 0
         self.sr: int = sr
         "Sample rate"
```

### Comparing `csoundengine-2.8.5/csoundengine/engineorc.py` & `csoundengine-2.9.0/csoundengine/engineorc.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/event.py` & `csoundengine-2.9.0/csoundengine/event.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/instr.py` & `csoundengine-2.9.0/csoundengine/instr.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/instrtools.py` & `csoundengine-2.9.0/csoundengine/instrtools.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/interact.py` & `csoundengine-2.9.0/csoundengine/interact.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/internal.py` & `csoundengine-2.9.0/csoundengine/internal.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/jacktools.py` & `csoundengine-2.9.0/csoundengine/jacktools.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/jupytertools.py` & `csoundengine-2.9.0/csoundengine/jupytertools.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/linuxaudio.py` & `csoundengine-2.9.0/csoundengine/linuxaudio.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/magic.py` & `csoundengine-2.9.0/csoundengine/magic.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/offline.py` & `csoundengine-2.9.0/csoundengine/offline.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 import sys
 import sndfileio
 import bpf4
 import numpy as np
 from functools import cache
 from dataclasses import dataclass
 import textwrap
+import tempfile
+import ctcsound7 as ctcsound
 
-from .errors import RenderError
+from .errors import RenderError, CsoundError
 from .config import config, logger
 from .instr import Instr
 from .schedevent import SchedEvent, SchedEventGroup
 from .event import Event
 from .abstractrenderer import AbstractRenderer
 from . import csoundlib
 from . import internal
@@ -36,15 +38,16 @@
 if TYPE_CHECKING or "sphinx" in sys.modules:
     from typing import Callable, Sequence, Iterator, Any
     import subprocess
 
 
 __all__ = (
     "Renderer",
-    "RenderJob"
+    "RenderJob",
+    "OfflineEngine"
 )
 
 
 _EMPTYDICT: dict[str, Any] = {}
 
 
 @dataclass
@@ -1743,7 +1746,176 @@
     for key, value in controls.items():
         assert key.startswith('k')
         lines.append(f"    {key} tab i__slicestart__ + {idx}, i__tabnum__")
         idx += 1
     lines.append("    ; --- end generated code\n")
     out = emlib.textlib.stripLines(emlib.textlib.joinPreservingIndentation(lines))
     return out
+
+
+class OfflineEngine:
+    def __init__(self,
+                 sr=44100,
+                 ksmps: int = 64,
+                 outfile: str = '',
+                 nchnls=2,
+                 a4: int = 0,
+                 globalcode='',
+                 numAudioBuses: int | None = None,
+                 numControlBuses: int | None = None,
+                 quiet=True,
+                 includes: list[str] | None = None,
+                 sampleAccurate=False,
+                 commandlineOptions: list[str] = None):
+        self.outfile = outfile or tempfile.mktemp(prefix='csoundengine', suffix='.wav')
+        self.sr = sr
+        self.ksmps = ksmps
+        self.a4 = a4 or config['A4']
+        self.nchnls = nchnls
+        self.globalcode = globalcode
+        self.numAudioBuses = numAudioBuses if numAudioBuses is not None else config['num_audio_buses']
+        self.numControlBuses = numControlBuses if numControlBuses is not None else config['num_control_buses']
+        self.includes = includes
+        self._builtinInstrs: dict[str, int] = {}
+        """Dict of built-in instrs, mapping instr name to number"""
+
+        self._reservedInstrnums: set[int] = set()
+        self._reservedInstrnumRanges: list[tuple[str, int, int]] = [
+            ('builtinorc', engineorc.CONSTS['reservedInstrsStart'], engineorc.CONSTS['userInstrsStart'] - 1)]
+
+        self._shouldPerform = False
+        self._endtime = 0.
+        self.nosound = False
+        self.options = ["-d"]
+        if quiet:
+            self.options.extend(["--messagelevel=0", "--m-amps=0", "--m-range=0"])
+
+        if nchnls == 0:
+            self.options.append('--nosound')
+            self.nosound = True
+        if sampleAccurate:
+            self.options.append('--sample-accurate')
+        if commandlineOptions:
+            self.options.extend(commandlineOptions)
+        self.csound = self._start()
+
+    def _start(self) -> ctcsound.Csound:
+        cs = ctcsound.Csound()
+        for option in self.options:
+            cs.setOption(option)
+        if not self.nosound:
+            cs.setOption(f'-o{self.outfile}')
+
+        if self.includes:
+            includelines = [f'#include "{include}"' for include in self.includes]
+            includestr = "\n".join(includelines)
+        else:
+            includestr = ""
+
+        orc, instrmap = engineorc.makeOrc(sr=self.sr,
+                                          ksmps=self.ksmps,
+                                          nchnls=self.nchnls,
+                                          nchnls_i=0,
+                                          a4=self.a4,
+                                          globalcode=self.globalcode,
+                                          includestr=includestr,
+                                          numAudioBuses=self.numAudioBuses,
+                                          numControlBuses=self.numControlBuses)
+
+        self._builtinInstrs = instrmap
+        self._reservedInstrnums.update(set(instrmap.values()))
+
+        err = cs.compileOrc(orc)
+        if err:
+            tmporc = tempfile.mktemp(prefix="csoundengine-", suffix=".orc")
+            open(tmporc, "w").write(orc)
+            logger.error(f"Error compiling base orchestra. A copy of the orchestra"
+                         f" has been saved to {tmporc}")
+
+            logger.error(internal.addLineNumbers(orc))
+            raise CsoundError(f"Error compiling base ochestra, error: {err}")
+        cs.start()
+        return cs
+
+    def compile(self, code: str) -> None:
+        codeblocks = csoundlib.parseOrc(code)
+        for codeblock in codeblocks:
+            if codeblock.kind == 'instr' and codeblock.name[0].isdigit():
+                instrnum = int(codeblock.name)
+                for rangename, mininstr, maxinstr in self._reservedInstrnumRanges:
+                    if mininstr <= instrnum < maxinstr:
+                        logger.error(f"Instrument number {instrnum} is reserved. Code:")
+                        logger.error("\n" + textwrap.indent(codeblock.text, "    "))
+                        raise ValueError(f"Cannot use instrument number {instrnum}, "
+                                         f"the range {mininstr} - {maxinstr} is reserved for '{rangename}'")
+
+                if instrnum in self._reservedInstrnums:
+                    raise ValueError("Cannot compile instrument with number "
+                                     f"{instrnum}: this is a reserved instr and "
+                                     f"cannot be redefined. Reserved instrs: "
+                                     f"{sorted(self._reservedInstrnums)}")
+
+        self.csound.compileOrc(code)
+        self._shouldPerform = True
+
+    def sched(self,
+              instr: int | float | str,
+              delay=0.,
+              dur=-1,
+              args: np.ndarray | list[float | str] | None = None,
+              ):
+        if dur >= 0 and delay + dur > self._endtime:
+            self._endtime = delay + dur
+        elif delay > self._endtime:
+            self._endtime = delay
+
+        if isinstance(instr, str):
+            msg = f'i "{instr}" {delay} {dur} '
+            if args:
+                argstrs = [str(arg) if not isinstance(arg, str) else f'"{arg}"'
+                           for arg in args]
+                msg += ' '.join(argstrs)
+            self.csound.inputMessage(msg)
+
+        else:
+            if isinstance(args, np.ndarray):
+                pfields = np.empty((len(args) + 3,), dtype=float)
+                pfields[0] = instr
+                pfields[1] = delay
+                pfields[2] = dur
+                pfields[3:] = args
+            elif not args:
+                pfields = [instr, delay, dur]
+            elif isinstance(args, (list, tuple)):
+                pfields = [instr, delay, dur]
+                pfields.extend(float(a) if not isinstance(a, str) else self.strSet(a) for a in args)
+            else:
+                raise TypeError(f"Expected a sequence or array, got {args}")
+            self.csound.scoreEventAbsolute(type_='i', pFields=pfields, timeOffset=0)
+        self._shouldPerform = True
+
+    def setEndMarker(self, time: float):
+        self._endtime = time
+
+    def perform(self, extratime=0.):
+        assert self.csound is not None
+        if self._endtime == 0.:
+            raise CsoundError("The render time is 0.")
+
+        if self._shouldPerform:
+            maxsamples = int((self._endtime + extratime) * self.sr)
+            cs = self.csound
+            logger.debug("Starting performance")
+            while not cs.performKsmps() and cs.currentTimeSamples() < maxsamples:
+                pass
+
+    def stop(self):
+        self.csound.stop()
+
+    def cancel(self):
+        self._shouldPerform = False
+        if self.csound:
+            self.csound.stop()
+
+    def __del__(self):
+        if self.csound and self._shouldPerform:
+            self.perform()
```

### Comparing `csoundengine-2.8.5/csoundengine/offlineorc.py` & `csoundengine-2.9.0/csoundengine/offlineorc.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/paramtable.py` & `csoundengine-2.9.0/csoundengine/paramtable.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/plotting.py` & `csoundengine-2.9.0/csoundengine/plotting.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/schedevent.py` & `csoundengine-2.9.0/csoundengine/schedevent.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/session.py` & `csoundengine-2.9.0/csoundengine/session.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/sessionhandler.py` & `csoundengine-2.9.0/csoundengine/sessionhandler.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/sessioninstrs.py` & `csoundengine-2.9.0/csoundengine/sessioninstrs.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/state.py` & `csoundengine-2.9.0/csoundengine/state.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/synth.py` & `csoundengine-2.9.0/csoundengine/synth.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/tableproxy.py` & `csoundengine-2.9.0/csoundengine/tableproxy.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine/tools.py` & `csoundengine-2.9.0/csoundengine/tools.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/csoundengine.egg-info/PKG-INFO` & `csoundengine-2.9.0/csoundengine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csoundengine
-Version: 2.8.5
+Version: 2.9.0
 Summary: A synthesis framework using csound
 Home-page: https://github.com/gesellkammer/csoundengine
 Author: Eduardo Moguillansky
 Author-email: eduardo.moguillansky@gmail.com
 License: BSD
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -21,15 +21,15 @@
 Requires-Dist: ipywidgets
 Requires-Dist: progressbar2
 Requires-Dist: xxhash
 Requires-Dist: docstring_parser
 Requires-Dist: typing_extensions
 Requires-Dist: ctcsound7>=0.4.6
 Requires-Dist: sndfileio>=1.9.4
-Requires-Dist: emlib>=1.14.1
+Requires-Dist: emlib>=1.15.0
 Requires-Dist: configdict>=2.10.0
 Requires-Dist: bpf4>=1.10.1
 Requires-Dist: numpyx>=1.3.3
 Requires-Dist: pitchtools>=1.14.0
 Requires-Dist: risset>=2.9.1
 Requires-Dist: sounddevice
```

### Comparing `csoundengine-2.8.5/csoundengine.egg-info/SOURCES.txt` & `csoundengine-2.9.0/csoundengine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/setup.py` & `csoundengine-2.9.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from setuptools import setup
 import os
 
-version = (2, 8, 5)
+version = (2, 9, 0)
 
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 
@@ -48,15 +48,15 @@
         "progressbar2",
         "xxhash",
         "docstring_parser",
         "typing_extensions",
 
         "ctcsound7>=0.4.6",
         "sndfileio>=1.9.4",
-        "emlib>=1.14.1",
+        "emlib>=1.15.0",
         "configdict>=2.10.0",
         "bpf4>=1.10.1",
         "numpyx>=1.3.3",
         "pitchtools>=1.14.0",
         "risset>=2.9.1",
         "sounddevice"
     ],
```

### Comparing `csoundengine-2.8.5/test/test1.py` & `csoundengine-2.9.0/test/test1.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.5/test/test2.py` & `csoundengine-2.9.0/test/test2.py`

 * *Files identical despite different names*

