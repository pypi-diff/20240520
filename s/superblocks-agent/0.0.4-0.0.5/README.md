# Comparing `tmp/superblocks-agent-0.0.4.tar.gz` & `tmp/superblocks-agent-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superblocks-agent-0.0.4.tar", last modified: Sat May 18 01:58:56 2024, max compression
+gzip compressed data, was "superblocks-agent-0.0.5.tar", last modified: Mon May 20 13:29:36 2024, max compression
```

## Comparing `superblocks-agent-0.0.4.tar` & `superblocks-agent-0.0.5.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-18 01:58:56.205670 superblocks-agent-0.0.4/
--rw-r--r--   0 joeygreco   (501) staff       (20)     1068 2024-05-06 19:43:05.000000 superblocks-agent-0.0.4/LICENSE
--rw-r--r--   0 joeygreco   (501) staff       (20)       25 2024-05-15 16:03:40.000000 superblocks-agent-0.0.4/MANIFEST.in
--rw-r--r--   0 joeygreco   (501) staff       (20)     2273 2024-05-18 01:58:56.205462 superblocks-agent-0.0.4/PKG-INFO
--rw-r--r--   0 joeygreco   (501) staff       (20)     1895 2024-05-18 01:58:39.000000 superblocks-agent-0.0.4/README.md
--rw-r--r--   0 joeygreco   (501) staff       (20)      298 2024-05-15 14:39:28.000000 superblocks-agent-0.0.4/pyproject.toml
--rw-r--r--   0 joeygreco   (501) staff       (20)       65 2024-05-16 21:07:17.000000 superblocks-agent-0.0.4/requirements.txt
--rw-r--r--   0 joeygreco   (501) staff       (20)       38 2024-05-18 01:58:56.205781 superblocks-agent-0.0.4/setup.cfg
--rw-r--r--   0 joeygreco   (501) staff       (20)     1025 2024-05-10 20:19:54.000000 superblocks-agent-0.0.4/setup.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-18 01:58:56.195245 superblocks-agent-0.0.4/superblocks_agent/
--rw-r--r--   0 joeygreco   (501) staff       (20)       42 2024-05-06 20:42:01.000000 superblocks-agent-0.0.4/superblocks_agent/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)       94 2024-05-18 01:58:50.000000 superblocks-agent-0.0.4/superblocks_agent/_version.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-18 01:58:56.197287 superblocks-agent-0.0.4/superblocks_agent/enumeration/
--rw-r--r--   0 joeygreco   (501) staff       (20)      363 2024-05-17 13:31:35.000000 superblocks-agent-0.0.4/superblocks_agent/enumeration/BaseEnum.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1057 2024-05-17 13:33:54.000000 superblocks-agent-0.0.4/superblocks_agent/enumeration/ViewMode.py
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:31:35.000000 superblocks-agent-0.0.4/superblocks_agent/enumeration/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-18 01:58:56.199720 superblocks-agent-0.0.4/superblocks_agent/model/
--rw-r--r--   0 joeygreco   (501) staff       (20)      181 2024-05-17 13:31:35.000000 superblocks-agent-0.0.4/superblocks_agent/model/Agent.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      734 2024-05-17 13:36:17.000000 superblocks-agent-0.0.4/superblocks_agent/model/ApiConfig.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      250 2024-05-17 13:37:34.000000 superblocks-agent-0.0.4/superblocks_agent/model/ApiResult.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      124 2024-05-17 13:31:35.000000 superblocks-agent-0.0.4/superblocks_agent/model/Auth.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      284 2024-05-17 13:35:23.000000 superblocks-agent-0.0.4/superblocks_agent/model/ClientConfig.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      404 2024-05-17 13:31:35.000000 superblocks-agent-0.0.4/superblocks_agent/model/ExecutionError.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1890 2024-05-17 13:38:39.000000 superblocks-agent-0.0.4/superblocks_agent/model/ExecutionResult.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1000 2024-05-17 13:38:39.000000 superblocks-agent-0.0.4/superblocks_agent/model/MockApiFilters.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      270 2024-05-17 13:37:49.000000 superblocks-agent-0.0.4/superblocks_agent/model/StepResult.py
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:31:35.000000 superblocks-agent-0.0.4/superblocks_agent/model/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-18 01:58:56.200384 superblocks-agent-0.0.4/superblocks_agent/model/abstract/
--rw-r--r--   0 joeygreco   (501) staff       (20)      475 2024-05-17 13:36:41.000000 superblocks-agent-0.0.4/superblocks_agent/model/abstract/BaseMock.py
--rw-r--r--   0 joeygreco   (501) staff       (20)       54 2024-05-17 13:31:35.000000 superblocks-agent-0.0.4/superblocks_agent/model/abstract/MockFilters.py
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:31:35.000000 superblocks-agent-0.0.4/superblocks_agent/model/abstract/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-18 01:58:56.201326 superblocks-agent-0.0.4/superblocks_agent/things/
--rw-r--r--   0 joeygreco   (501) staff       (20)     6605 2024-05-17 13:38:39.000000 superblocks-agent-0.0.4/superblocks_agent/things/Api.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2449 2024-05-17 13:38:39.000000 superblocks-agent-0.0.4/superblocks_agent/things/ApiMock.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2068 2024-05-17 13:38:39.000000 superblocks-agent-0.0.4/superblocks_agent/things/Client.py
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:31:35.000000 superblocks-agent-0.0.4/superblocks_agent/things/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-18 01:58:56.201948 superblocks-agent-0.0.4/superblocks_agent/type_/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:31:35.000000 superblocks-agent-0.0.4/superblocks_agent/type_/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      290 2024-05-17 13:31:35.000000 superblocks-agent-0.0.4/superblocks_agent/type_/client.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      264 2024-05-17 13:40:43.000000 superblocks-agent-0.0.4/superblocks_agent/type_/mock.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-18 01:58:56.202621 superblocks-agent-0.0.4/superblocks_agent/util/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:31:35.000000 superblocks-agent-0.0.4/superblocks_agent/util/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2905 2024-05-17 13:31:35.000000 superblocks-agent-0.0.4/superblocks_agent/util/convert.py
--rw-r--r--   0 joeygreco   (501) staff       (20)       71 2024-05-17 13:31:35.000000 superblocks-agent-0.0.4/superblocks_agent/util/generate.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-18 01:58:56.196497 superblocks-agent-0.0.4/superblocks_agent.egg-info/
--rw-r--r--   0 joeygreco   (501) staff       (20)     2273 2024-05-18 01:58:56.000000 superblocks-agent-0.0.4/superblocks_agent.egg-info/PKG-INFO
--rw-r--r--   0 joeygreco   (501) staff       (20)     1740 2024-05-18 01:58:56.000000 superblocks-agent-0.0.4/superblocks_agent.egg-info/SOURCES.txt
--rw-r--r--   0 joeygreco   (501) staff       (20)        1 2024-05-18 01:58:56.000000 superblocks-agent-0.0.4/superblocks_agent.egg-info/dependency_links.txt
--rw-r--r--   0 joeygreco   (501) staff       (20)       65 2024-05-18 01:58:56.000000 superblocks-agent-0.0.4/superblocks_agent.egg-info/requires.txt
--rw-r--r--   0 joeygreco   (501) staff       (20)       28 2024-05-18 01:58:56.000000 superblocks-agent-0.0.4/superblocks_agent.egg-info/top_level.txt
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-18 01:58:56.192816 superblocks-agent-0.0.4/test_unit/
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-18 01:58:56.203084 superblocks-agent-0.0.4/test_unit/test_enumeration/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:32:57.000000 superblocks-agent-0.0.4/test_unit/test_enumeration/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1400 2024-05-17 13:33:54.000000 superblocks-agent-0.0.4/test_unit/test_enumeration/test_ViewMode.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-18 01:58:56.203754 superblocks-agent-0.0.4/test_unit/test_model/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:32:57.000000 superblocks-agent-0.0.4/test_unit/test_model/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2596 2024-05-17 13:33:54.000000 superblocks-agent-0.0.4/test_unit/test_model/test_ExecutionResult.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      743 2024-05-17 13:33:54.000000 superblocks-agent-0.0.4/test_unit/test_model/test_MockApiFilters.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-18 01:58:56.204403 superblocks-agent-0.0.4/test_unit/test_things/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:32:57.000000 superblocks-agent-0.0.4/test_unit/test_things/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     8120 2024-05-17 13:33:54.000000 superblocks-agent-0.0.4/test_unit/test_things/test_Api.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     4135 2024-05-17 13:33:54.000000 superblocks-agent-0.0.4/test_unit/test_things/test_ApiMock.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-18 01:58:56.205074 superblocks-agent-0.0.4/test_unit/test_util/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:32:57.000000 superblocks-agent-0.0.4/test_unit/test_util/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3911 2024-05-17 13:33:54.000000 superblocks-agent-0.0.4/test_unit/test_util/test_convert.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      479 2024-05-17 13:33:54.000000 superblocks-agent-0.0.4/test_unit/test_util/test_generate.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-20 13:29:36.671802 superblocks-agent-0.0.5/
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1068 2024-05-06 19:43:05.000000 superblocks-agent-0.0.5/LICENSE
+-rw-r--r--   0 joeygreco   (501) staff       (20)       25 2024-05-15 16:03:40.000000 superblocks-agent-0.0.5/MANIFEST.in
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2318 2024-05-20 13:29:36.671573 superblocks-agent-0.0.5/PKG-INFO
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1940 2024-05-20 13:15:54.000000 superblocks-agent-0.0.5/README.md
+-rw-r--r--   0 joeygreco   (501) staff       (20)      298 2024-05-15 14:39:28.000000 superblocks-agent-0.0.5/pyproject.toml
+-rw-r--r--   0 joeygreco   (501) staff       (20)       65 2024-05-16 21:07:17.000000 superblocks-agent-0.0.5/requirements.txt
+-rw-r--r--   0 joeygreco   (501) staff       (20)       38 2024-05-20 13:29:36.671938 superblocks-agent-0.0.5/setup.cfg
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1025 2024-05-10 20:19:54.000000 superblocks-agent-0.0.5/setup.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-20 13:29:36.652902 superblocks-agent-0.0.5/superblocks_agent/
+-rw-r--r--   0 joeygreco   (501) staff       (20)       42 2024-05-06 20:42:01.000000 superblocks-agent-0.0.5/superblocks_agent/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)       94 2024-05-20 13:29:08.000000 superblocks-agent-0.0.5/superblocks_agent/_version.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-20 13:29:36.656412 superblocks-agent-0.0.5/superblocks_agent/core/
+-rw-r--r--   0 joeygreco   (501) staff       (20)     6601 2024-05-20 13:28:29.000000 superblocks-agent-0.0.5/superblocks_agent/core/Api.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2449 2024-05-17 13:38:39.000000 superblocks-agent-0.0.5/superblocks_agent/core/ApiMock.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2114 2024-05-20 13:24:56.000000 superblocks-agent-0.0.5/superblocks_agent/core/Client.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:31:35.000000 superblocks-agent-0.0.5/superblocks_agent/core/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-20 13:29:36.657635 superblocks-agent-0.0.5/superblocks_agent/enumeration/
+-rw-r--r--   0 joeygreco   (501) staff       (20)      363 2024-05-17 13:31:35.000000 superblocks-agent-0.0.5/superblocks_agent/enumeration/BaseEnum.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1057 2024-05-17 13:33:54.000000 superblocks-agent-0.0.5/superblocks_agent/enumeration/ViewMode.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:31:35.000000 superblocks-agent-0.0.5/superblocks_agent/enumeration/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-20 13:29:36.662252 superblocks-agent-0.0.5/superblocks_agent/model/
+-rw-r--r--   0 joeygreco   (501) staff       (20)      181 2024-05-17 13:31:35.000000 superblocks-agent-0.0.5/superblocks_agent/model/Agent.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      734 2024-05-17 13:36:17.000000 superblocks-agent-0.0.5/superblocks_agent/model/ApiConfig.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      250 2024-05-17 13:37:34.000000 superblocks-agent-0.0.5/superblocks_agent/model/ApiResult.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      124 2024-05-17 13:31:35.000000 superblocks-agent-0.0.5/superblocks_agent/model/Auth.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      284 2024-05-17 13:35:23.000000 superblocks-agent-0.0.5/superblocks_agent/model/ClientConfig.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      404 2024-05-17 13:31:35.000000 superblocks-agent-0.0.5/superblocks_agent/model/ExecutionError.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1890 2024-05-17 13:38:39.000000 superblocks-agent-0.0.5/superblocks_agent/model/ExecutionResult.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1000 2024-05-17 13:38:39.000000 superblocks-agent-0.0.5/superblocks_agent/model/MockApiFilters.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      270 2024-05-17 13:37:49.000000 superblocks-agent-0.0.5/superblocks_agent/model/StepResult.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:31:35.000000 superblocks-agent-0.0.5/superblocks_agent/model/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-20 13:29:36.663509 superblocks-agent-0.0.5/superblocks_agent/model/abstract/
+-rw-r--r--   0 joeygreco   (501) staff       (20)      475 2024-05-17 13:36:41.000000 superblocks-agent-0.0.5/superblocks_agent/model/abstract/BaseMock.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)       54 2024-05-17 13:31:35.000000 superblocks-agent-0.0.5/superblocks_agent/model/abstract/MockFilters.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:31:35.000000 superblocks-agent-0.0.5/superblocks_agent/model/abstract/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-20 13:29:36.664596 superblocks-agent-0.0.5/superblocks_agent/type_/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:31:35.000000 superblocks-agent-0.0.5/superblocks_agent/type_/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      290 2024-05-17 13:31:35.000000 superblocks-agent-0.0.5/superblocks_agent/type_/client.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      264 2024-05-17 13:40:43.000000 superblocks-agent-0.0.5/superblocks_agent/type_/mock.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-20 13:29:36.665753 superblocks-agent-0.0.5/superblocks_agent/util/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:31:35.000000 superblocks-agent-0.0.5/superblocks_agent/util/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2905 2024-05-17 13:31:35.000000 superblocks-agent-0.0.5/superblocks_agent/util/convert.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)       71 2024-05-17 13:31:35.000000 superblocks-agent-0.0.5/superblocks_agent/util/generate.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-20 13:29:36.654478 superblocks-agent-0.0.5/superblocks_agent.egg-info/
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2318 2024-05-20 13:29:36.000000 superblocks-agent-0.0.5/superblocks_agent.egg-info/PKG-INFO
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1726 2024-05-20 13:29:36.000000 superblocks-agent-0.0.5/superblocks_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 joeygreco   (501) staff       (20)        1 2024-05-20 13:29:36.000000 superblocks-agent-0.0.5/superblocks_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 joeygreco   (501) staff       (20)       65 2024-05-20 13:29:36.000000 superblocks-agent-0.0.5/superblocks_agent.egg-info/requires.txt
+-rw-r--r--   0 joeygreco   (501) staff       (20)       28 2024-05-20 13:29:36.000000 superblocks-agent-0.0.5/superblocks_agent.egg-info/top_level.txt
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-20 13:29:36.649743 superblocks-agent-0.0.5/test_unit/
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-20 13:29:36.667313 superblocks-agent-0.0.5/test_unit/test_core/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:32:57.000000 superblocks-agent-0.0.5/test_unit/test_core/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     8116 2024-05-20 13:28:29.000000 superblocks-agent-0.0.5/test_unit/test_core/test_Api.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     4133 2024-05-20 13:28:29.000000 superblocks-agent-0.0.5/test_unit/test_core/test_ApiMock.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-20 13:29:36.668438 superblocks-agent-0.0.5/test_unit/test_enumeration/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:32:57.000000 superblocks-agent-0.0.5/test_unit/test_enumeration/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1400 2024-05-17 13:33:54.000000 superblocks-agent-0.0.5/test_unit/test_enumeration/test_ViewMode.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-20 13:29:36.669870 superblocks-agent-0.0.5/test_unit/test_model/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:32:57.000000 superblocks-agent-0.0.5/test_unit/test_model/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2596 2024-05-17 13:33:54.000000 superblocks-agent-0.0.5/test_unit/test_model/test_ExecutionResult.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      743 2024-05-17 13:33:54.000000 superblocks-agent-0.0.5/test_unit/test_model/test_MockApiFilters.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-20 13:29:36.670998 superblocks-agent-0.0.5/test_unit/test_util/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:32:57.000000 superblocks-agent-0.0.5/test_unit/test_util/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3911 2024-05-17 13:33:54.000000 superblocks-agent-0.0.5/test_unit/test_util/test_convert.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      479 2024-05-17 13:33:54.000000 superblocks-agent-0.0.5/test_unit/test_util/test_generate.py
```

### Comparing `superblocks-agent-0.0.4/LICENSE` & `superblocks-agent-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.4/PKG-INFO` & `superblocks-agent-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superblocks-agent
-Version: 0.0.4
+Version: 0.0.5
 Summary: The Official Python SDK for Superblocks
 Home-page: https://github.com/superblocksteam/orchestrator/tree/main/clients/python
 Author: Joey Greco
 Author-email: joeyagreco@gmail.com
 License: MIT
 Keywords: superblocks api sdk
 Requires-Python: >=3.10
@@ -30,14 +30,15 @@
 ```python3
 import asyncio
 
 from superblocks_agent.things.Client import Client
 from superblocks_agent.model.ClientConfig import ClientConfig
 from superblocks_agent.model.Agent import Agent
 from superblocks_agent.model.Auth import Auth
+from superblocks_agent.things.Api import Api
 
 
 client = Client(ClientConfig(agent=Agent(endpoint="agent_url"), auth=Auth(token="auth_token")))
 api = Api("some_api_id")
 execution_result = asyncio.run(api.run(client=client))
 ```
```

### Comparing `superblocks-agent-0.0.4/README.md` & `superblocks-agent-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 ```python3
 import asyncio
 
 from superblocks_agent.things.Client import Client
 from superblocks_agent.model.ClientConfig import ClientConfig
 from superblocks_agent.model.Agent import Agent
 from superblocks_agent.model.Auth import Auth
+from superblocks_agent.things.Api import Api
 
 
 client = Client(ClientConfig(agent=Agent(endpoint="agent_url"), auth=Auth(token="auth_token")))
 api = Api("some_api_id")
 execution_result = asyncio.run(api.run(client=client))
 ```
```

### Comparing `superblocks-agent-0.0.4/setup.py` & `superblocks-agent-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.4/superblocks_agent/enumeration/ViewMode.py` & `superblocks-agent-0.0.5/superblocks_agent/enumeration/ViewMode.py`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.4/superblocks_agent/model/ApiConfig.py` & `superblocks-agent-0.0.5/superblocks_agent/model/ApiConfig.py`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.4/superblocks_agent/model/ExecutionResult.py` & `superblocks-agent-0.0.5/superblocks_agent/model/ExecutionResult.py`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.4/superblocks_agent/model/MockApiFilters.py` & `superblocks-agent-0.0.5/superblocks_agent/model/MockApiFilters.py`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.4/superblocks_agent/things/Api.py` & `superblocks-agent-0.0.5/superblocks_agent/core/Api.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,18 +7,18 @@
     TwoWayRequest,
     TwoWayResponse,
 )
 from superblocks_types.api.v1.service_pb2_grpc import ExecutorServiceStub
 from superblocks_types.common.v1.common_pb2 import Profile
 from superblocks_types.common.v1.errors_pb2 import Error
 
+from superblocks_agent.core.ApiMock import ApiMock
+from superblocks_agent.core.Client import Client
 from superblocks_agent.model.ApiConfig import ApiConfig
 from superblocks_agent.model.ExecutionResult import ExecutionResult
-from superblocks_agent.things.ApiMock import ApiMock
-from superblocks_agent.things.Client import Client
 from superblocks_agent.util.convert import from_protobuf_value, to_protobuf_value
 from superblocks_agent.util.generate import get_unique_id_for_object
 
 
 class Api:
     def __init__(self, api_id: str, *, config: Optional[ApiConfig] = None):
         self.__api_id = api_id
```

### Comparing `superblocks-agent-0.0.4/superblocks_agent/things/ApiMock.py` & `superblocks-agent-0.0.5/superblocks_agent/core/ApiMock.py`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.4/superblocks_agent/things/Client.py` & `superblocks-agent-0.0.5/superblocks_agent/core/Client.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 from superblocks_types.api.v1.service_pb2 import StreamResponse
 
 from superblocks_agent.model.ClientConfig import ClientConfig
 from superblocks_agent.type_.client import GenericMetadata, TwoWayStreamResponseHandler
 
 
 class Client:
-    def __init__(self, client_config: ClientConfig):
-        self.__client_config = client_config
+    def __init__(self, config: ClientConfig):
+        self.__config = config
 
     async def run(
         self,
         *,
         with_stub: object,
         stub_func_name: str,
         initial_requests: list[object],
         response_handler: TwoWayStreamResponseHandler,
     ) -> list[StreamResponse]:
-        stub = with_stub(channel=grpc.insecure_channel(target=self.__client_config.agent.endpoint))
+        # TODO: (joey) throw clear errors here for auth/connection issues
+        stub = with_stub(channel=grpc.insecure_channel(target=self.__config.agent.endpoint))
         stub_function = getattr(stub, stub_func_name)
 
         return self.__handle_two_way_stream(
             stub_function=stub_function,
             requests=initial_requests,
             response_handler=response_handler,
         )
```

### Comparing `superblocks-agent-0.0.4/superblocks_agent/util/convert.py` & `superblocks-agent-0.0.5/superblocks_agent/util/convert.py`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.4/superblocks_agent.egg-info/PKG-INFO` & `superblocks-agent-0.0.5/superblocks_agent.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superblocks-agent
-Version: 0.0.4
+Version: 0.0.5
 Summary: The Official Python SDK for Superblocks
 Home-page: https://github.com/superblocksteam/orchestrator/tree/main/clients/python
 Author: Joey Greco
 Author-email: joeyagreco@gmail.com
 License: MIT
 Keywords: superblocks api sdk
 Requires-Python: >=3.10
@@ -30,14 +30,15 @@
 ```python3
 import asyncio
 
 from superblocks_agent.things.Client import Client
 from superblocks_agent.model.ClientConfig import ClientConfig
 from superblocks_agent.model.Agent import Agent
 from superblocks_agent.model.Auth import Auth
+from superblocks_agent.things.Api import Api
 
 
 client = Client(ClientConfig(agent=Agent(endpoint="agent_url"), auth=Auth(token="auth_token")))
 api = Api("some_api_id")
 execution_result = asyncio.run(api.run(client=client))
 ```
```

### Comparing `superblocks-agent-0.0.4/superblocks_agent.egg-info/SOURCES.txt` & `superblocks-agent-0.0.5/superblocks_agent.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 superblocks_agent/__init__.py
 superblocks_agent/_version.py
 superblocks_agent.egg-info/PKG-INFO
 superblocks_agent.egg-info/SOURCES.txt
 superblocks_agent.egg-info/dependency_links.txt
 superblocks_agent.egg-info/requires.txt
 superblocks_agent.egg-info/top_level.txt
+superblocks_agent/core/Api.py
+superblocks_agent/core/ApiMock.py
+superblocks_agent/core/Client.py
+superblocks_agent/core/__init__.py
 superblocks_agent/enumeration/BaseEnum.py
 superblocks_agent/enumeration/ViewMode.py
 superblocks_agent/enumeration/__init__.py
 superblocks_agent/model/Agent.py
 superblocks_agent/model/ApiConfig.py
 superblocks_agent/model/ApiResult.py
 superblocks_agent/model/Auth.py
@@ -23,28 +27,24 @@
 superblocks_agent/model/ExecutionResult.py
 superblocks_agent/model/MockApiFilters.py
 superblocks_agent/model/StepResult.py
 superblocks_agent/model/__init__.py
 superblocks_agent/model/abstract/BaseMock.py
 superblocks_agent/model/abstract/MockFilters.py
 superblocks_agent/model/abstract/__init__.py
-superblocks_agent/things/Api.py
-superblocks_agent/things/ApiMock.py
-superblocks_agent/things/Client.py
-superblocks_agent/things/__init__.py
 superblocks_agent/type_/__init__.py
 superblocks_agent/type_/client.py
 superblocks_agent/type_/mock.py
 superblocks_agent/util/__init__.py
 superblocks_agent/util/convert.py
 superblocks_agent/util/generate.py
+test_unit/test_core/__init__.py
+test_unit/test_core/test_Api.py
+test_unit/test_core/test_ApiMock.py
 test_unit/test_enumeration/__init__.py
 test_unit/test_enumeration/test_ViewMode.py
 test_unit/test_model/__init__.py
 test_unit/test_model/test_ExecutionResult.py
 test_unit/test_model/test_MockApiFilters.py
-test_unit/test_things/__init__.py
-test_unit/test_things/test_Api.py
-test_unit/test_things/test_ApiMock.py
 test_unit/test_util/__init__.py
 test_unit/test_util/test_convert.py
 test_unit/test_util/test_generate.py
```

### Comparing `superblocks-agent-0.0.4/test_unit/test_enumeration/test_ViewMode.py` & `superblocks-agent-0.0.5/test_unit/test_enumeration/test_ViewMode.py`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.4/test_unit/test_model/test_ExecutionResult.py` & `superblocks-agent-0.0.5/test_unit/test_model/test_ExecutionResult.py`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.4/test_unit/test_model/test_MockApiFilters.py` & `superblocks-agent-0.0.5/test_unit/test_model/test_MockApiFilters.py`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.4/test_unit/test_things/test_Api.py` & `superblocks-agent-0.0.5/test_unit/test_core/test_Api.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,19 @@
     StreamResponse,
     TwoWayRequest,
     TwoWayResponse,
 )
 from superblocks_types.common.v1.common_pb2 import Profile
 from superblocks_types.common.v1.errors_pb2 import Error
 
+from superblocks_agent.core.Api import Api
+from superblocks_agent.core.ApiMock import ApiMock
 from superblocks_agent.enumeration.ViewMode import ViewMode
 from superblocks_agent.model.ApiConfig import ApiConfig
 from superblocks_agent.model.MockApiFilters import MockApiFilters
-from superblocks_agent.things.Api import Api
-from superblocks_agent.things.ApiMock import ApiMock
 from superblocks_agent.util.convert import Mock_, to_protobuf_value
 from superblocks_agent.util.generate import get_unique_id_for_object
 
 
 class TestApi(unittest.TestCase):
     def test_build_execute_request(self):
         api = Api(
```

### Comparing `superblocks-agent-0.0.4/test_unit/test_things/test_ApiMock.py` & `superblocks-agent-0.0.5/test_unit/test_core/test_ApiMock.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 
 from superblocks_types.api.v1.service_pb2 import Mock
 
+from superblocks_agent.core.ApiMock import ApiMock, on
 from superblocks_agent.model.MockApiFilters import MockApiFilters
-from superblocks_agent.things.ApiMock import ApiMock, on
 from superblocks_agent.util.convert import Mock_, to_protobuf_value
 from superblocks_agent.util.generate import get_unique_id_for_object
 
 
 class TestApiMock(unittest.TestCase):
     def test_return_(self):
         # overwrites existing return val
```

### Comparing `superblocks-agent-0.0.4/test_unit/test_util/test_convert.py` & `superblocks-agent-0.0.5/test_unit/test_util/test_convert.py`

 * *Files identical despite different names*

