# Comparing `tmp/dishka-1.1.1.tar.gz` & `tmp/dishka-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dishka-1.1.1.tar", last modified: Fri Apr 26 21:44:04 2024, max compression
+gzip compressed data, was "dishka-1.2.0.tar", last modified: Mon May 20 21:22:59 2024, max compression
```

## Comparing `dishka-1.1.1.tar` & `dishka-1.2.0.tar`

### file list

```diff
@@ -1,69 +1,70 @@
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-26 21:44:04.023128 dishka-1.1.1/
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)    11357 2024-01-25 16:39:00.000000 dishka-1.1.1/LICENSE
--rw-r--r--   0 tishka17  (1000) tishka17  (1000)    12011 2024-04-26 21:44:04.023128 dishka-1.1.1/PKG-INFO
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)    11074 2024-04-21 10:24:38.000000 dishka-1.1.1/README.md
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1097 2024-04-26 21:43:35.000000 dishka-1.1.1/pyproject.toml
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)       38 2024-04-26 21:44:04.023128 dishka-1.1.1/setup.cfg
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-26 21:44:04.019128 dishka-1.1.1/src/
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-26 21:44:04.019128 dishka-1.1.1/src/dishka/
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      843 2024-04-21 10:24:38.000000 dishka-1.1.1/src/dishka/__init__.py
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-26 21:44:04.019128 dishka-1.1.1/src/dishka/_adaptix/
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      639 2024-04-21 10:24:38.000000 dishka-1.1.1/src/dishka/_adaptix/common.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     5460 2024-04-21 10:24:38.000000 dishka-1.1.1/src/dishka/_adaptix/feature_requirement.py
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-26 21:44:04.019128 dishka-1.1.1/src/dishka/_adaptix/type_tools/
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      609 2024-04-21 10:24:38.000000 dishka-1.1.1/src/dishka/_adaptix/type_tools/__init__.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     4141 2024-04-21 10:24:38.000000 dishka-1.1.1/src/dishka/_adaptix/type_tools/basic_utils.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      994 2024-04-21 10:24:38.000000 dishka-1.1.1/src/dishka/_adaptix/type_tools/constants.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1530 2024-04-21 10:24:38.000000 dishka-1.1.1/src/dishka/_adaptix/type_tools/fundamentals.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     3907 2024-04-21 10:24:38.000000 dishka-1.1.1/src/dishka/_adaptix/type_tools/generic_resolver.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1828 2024-04-21 10:24:38.000000 dishka-1.1.1/src/dishka/_adaptix/type_tools/implicit_params.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1059 2024-04-21 10:24:38.000000 dishka-1.1.1/src/dishka/_adaptix/type_tools/norm_utils.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)    25528 2024-04-21 10:24:38.000000 dishka-1.1.1/src/dishka/_adaptix/type_tools/normalize_type.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     7025 2024-04-21 10:24:38.000000 dishka-1.1.1/src/dishka/async_container.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     6664 2024-04-21 10:24:38.000000 dishka-1.1.1/src/dishka/container.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      476 2024-03-24 23:55:01.000000 dishka-1.1.1/src/dishka/container_objects.py
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-26 21:44:04.019128 dishka-1.1.1/src/dishka/dependency_source/
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      542 2024-04-21 10:24:38.000000 dishka-1.1.1/src/dishka/dependency_source/__init__.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1038 2024-03-19 22:45:31.000000 dishka-1.1.1/src/dishka/dependency_source/alias.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1416 2024-04-24 19:42:27.000000 dishka-1.1.1/src/dishka/dependency_source/composite.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1515 2024-03-19 22:45:31.000000 dishka-1.1.1/src/dishka/dependency_source/context_var.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1324 2024-03-19 22:45:31.000000 dishka-1.1.1/src/dishka/dependency_source/decorator.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2164 2024-04-26 21:28:12.000000 dishka-1.1.1/src/dishka/dependency_source/factory.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      905 2024-03-19 22:45:31.000000 dishka-1.1.1/src/dishka/dependency_source/make_alias.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      678 2024-03-19 22:45:31.000000 dishka-1.1.1/src/dishka/dependency_source/make_context_var.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1462 2024-04-01 21:05:02.000000 dishka-1.1.1/src/dishka/dependency_source/make_decorator.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)    16505 2024-04-26 21:43:29.000000 dishka-1.1.1/src/dishka/dependency_source/make_factory.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1949 2024-03-19 22:45:31.000000 dishka-1.1.1/src/dishka/dependency_source/unpack_provides.py
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-26 21:44:04.019128 dishka-1.1.1/src/dishka/entities/
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        0 2024-02-29 00:39:11.000000 dishka-1.1.1/src/dishka/entities/__init__.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)       40 2024-02-29 00:39:11.000000 dishka-1.1.1/src/dishka/entities/component.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1178 2024-04-20 19:15:28.000000 dishka-1.1.1/src/dishka/entities/depends_marker.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1123 2024-03-04 22:02:38.000000 dishka-1.1.1/src/dishka/entities/key.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      347 2024-03-19 22:45:31.000000 dishka-1.1.1/src/dishka/entities/provides_marker.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      783 2024-03-24 23:55:01.000000 dishka-1.1.1/src/dishka/entities/scope.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2730 2024-03-26 23:39:41.000000 dishka-1.1.1/src/dishka/error_rendering.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1715 2024-03-04 22:02:38.000000 dishka-1.1.1/src/dishka/exceptions.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     3398 2024-04-21 10:24:38.000000 dishka-1.1.1/src/dishka/factory_compiler.py
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-26 21:44:04.023128 dishka-1.1.1/src/dishka/integrations/
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        0 2024-02-08 23:15:26.000000 dishka-1.1.1/src/dishka/integrations/__init__.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2279 2024-03-24 23:55:01.000000 dishka-1.1.1/src/dishka/integrations/aiogram.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1232 2024-03-24 23:55:01.000000 dishka-1.1.1/src/dishka/integrations/aiohttp.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2445 2024-03-04 22:02:38.000000 dishka-1.1.1/src/dishka/integrations/arq.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     5268 2024-03-24 23:55:01.000000 dishka-1.1.1/src/dishka/integrations/base.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1417 2024-03-24 23:55:01.000000 dishka-1.1.1/src/dishka/integrations/fastapi.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     3676 2024-04-21 10:24:38.000000 dishka-1.1.1/src/dishka/integrations/faststream.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1421 2024-03-24 23:55:01.000000 dishka-1.1.1/src/dishka/integrations/flask.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1749 2024-03-24 23:55:01.000000 dishka-1.1.1/src/dishka/integrations/litestar.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1617 2024-04-21 10:24:38.000000 dishka-1.1.1/src/dishka/integrations/sanic.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1248 2024-03-24 23:55:01.000000 dishka-1.1.1/src/dishka/integrations/starlette.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2226 2024-04-02 21:16:55.000000 dishka-1.1.1/src/dishka/integrations/taskiq.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1379 2024-03-28 15:28:45.000000 dishka-1.1.1/src/dishka/integrations/telebot.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     6855 2024-04-21 10:24:38.000000 dishka-1.1.1/src/dishka/provider.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        0 2024-02-18 18:04:06.000000 dishka-1.1.1/src/dishka/py.typed
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)    13177 2024-04-26 21:43:29.000000 dishka-1.1.1/src/dishka/registry.py
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-26 21:44:04.023128 dishka-1.1.1/src/dishka.egg-info/
--rw-r--r--   0 tishka17  (1000) tishka17  (1000)    12011 2024-04-26 21:44:04.000000 dishka-1.1.1/src/dishka.egg-info/PKG-INFO
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2037 2024-04-26 21:44:04.000000 dishka-1.1.1/src/dishka.egg-info/SOURCES.txt
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        1 2024-04-26 21:44:04.000000 dishka-1.1.1/src/dishka.egg-info/dependency_links.txt
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)       50 2024-04-26 21:44:04.000000 dishka-1.1.1/src/dishka.egg-info/requires.txt
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        7 2024-04-26 21:44:04.000000 dishka-1.1.1/src/dishka.egg-info/top_level.txt
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-05-20 21:22:59.500606 dishka-1.2.0/
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)    11357 2024-01-25 16:39:00.000000 dishka-1.2.0/LICENSE
+-rw-r--r--   0 tishka17  (1000) tishka17  (1000)    12011 2024-05-20 21:22:59.500606 dishka-1.2.0/PKG-INFO
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)    11074 2024-05-20 21:22:19.000000 dishka-1.2.0/README.md
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1097 2024-05-20 21:22:27.000000 dishka-1.2.0/pyproject.toml
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)       38 2024-05-20 21:22:59.500606 dishka-1.2.0/setup.cfg
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-05-20 21:22:59.496602 dishka-1.2.0/src/
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-05-20 21:22:59.496602 dishka-1.2.0/src/dishka/
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      843 2024-05-16 13:52:24.000000 dishka-1.2.0/src/dishka/__init__.py
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-05-20 21:22:59.496602 dishka-1.2.0/src/dishka/_adaptix/
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      639 2024-05-16 13:52:24.000000 dishka-1.2.0/src/dishka/_adaptix/common.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     5460 2024-05-16 13:52:24.000000 dishka-1.2.0/src/dishka/_adaptix/feature_requirement.py
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-05-20 21:22:59.496602 dishka-1.2.0/src/dishka/_adaptix/type_tools/
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      609 2024-05-16 13:52:24.000000 dishka-1.2.0/src/dishka/_adaptix/type_tools/__init__.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     4141 2024-05-16 13:52:24.000000 dishka-1.2.0/src/dishka/_adaptix/type_tools/basic_utils.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      994 2024-05-16 13:52:24.000000 dishka-1.2.0/src/dishka/_adaptix/type_tools/constants.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1530 2024-05-16 13:52:24.000000 dishka-1.2.0/src/dishka/_adaptix/type_tools/fundamentals.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     3907 2024-05-16 13:52:24.000000 dishka-1.2.0/src/dishka/_adaptix/type_tools/generic_resolver.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1828 2024-05-16 13:52:24.000000 dishka-1.2.0/src/dishka/_adaptix/type_tools/implicit_params.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1059 2024-05-16 13:52:24.000000 dishka-1.2.0/src/dishka/_adaptix/type_tools/norm_utils.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)    25528 2024-05-16 13:52:24.000000 dishka-1.2.0/src/dishka/_adaptix/type_tools/normalize_type.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     7400 2024-05-20 21:22:19.000000 dishka-1.2.0/src/dishka/async_container.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     7074 2024-05-20 21:22:19.000000 dishka-1.2.0/src/dishka/container.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      476 2024-05-16 13:52:24.000000 dishka-1.2.0/src/dishka/container_objects.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      857 2024-05-20 21:22:19.000000 dishka-1.2.0/src/dishka/context_proxy.py
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-05-20 21:22:59.496602 dishka-1.2.0/src/dishka/dependency_source/
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      542 2024-05-16 13:52:24.000000 dishka-1.2.0/src/dishka/dependency_source/__init__.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1070 2024-05-20 21:22:19.000000 dishka-1.2.0/src/dishka/dependency_source/alias.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1416 2024-05-16 13:52:24.000000 dishka-1.2.0/src/dishka/dependency_source/composite.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1551 2024-05-20 21:22:19.000000 dishka-1.2.0/src/dishka/dependency_source/context_var.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1635 2024-05-20 21:22:19.000000 dishka-1.2.0/src/dishka/dependency_source/decorator.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2505 2024-05-20 21:22:19.000000 dishka-1.2.0/src/dishka/dependency_source/factory.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      905 2024-05-16 13:52:24.000000 dishka-1.2.0/src/dishka/dependency_source/make_alias.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      678 2024-05-16 13:52:24.000000 dishka-1.2.0/src/dishka/dependency_source/make_context_var.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1462 2024-05-16 13:52:24.000000 dishka-1.2.0/src/dishka/dependency_source/make_decorator.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)    17319 2024-05-20 21:22:19.000000 dishka-1.2.0/src/dishka/dependency_source/make_factory.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1998 2024-05-20 21:22:19.000000 dishka-1.2.0/src/dishka/dependency_source/unpack_provides.py
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-05-20 21:22:59.500606 dishka-1.2.0/src/dishka/entities/
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        0 2024-05-16 13:52:24.000000 dishka-1.2.0/src/dishka/entities/__init__.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)       40 2024-05-16 13:52:24.000000 dishka-1.2.0/src/dishka/entities/component.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1178 2024-05-16 13:52:24.000000 dishka-1.2.0/src/dishka/entities/depends_marker.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1123 2024-05-16 13:52:24.000000 dishka-1.2.0/src/dishka/entities/key.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      347 2024-05-16 13:52:24.000000 dishka-1.2.0/src/dishka/entities/provides_marker.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      783 2024-05-16 13:52:24.000000 dishka-1.2.0/src/dishka/entities/scope.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2730 2024-05-16 13:52:24.000000 dishka-1.2.0/src/dishka/error_rendering.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1715 2024-05-16 13:52:24.000000 dishka-1.2.0/src/dishka/exceptions.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     3789 2024-05-20 21:22:19.000000 dishka-1.2.0/src/dishka/factory_compiler.py
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-05-20 21:22:59.500606 dishka-1.2.0/src/dishka/integrations/
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        0 2024-05-16 13:52:24.000000 dishka-1.2.0/src/dishka/integrations/__init__.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2279 2024-05-16 13:52:24.000000 dishka-1.2.0/src/dishka/integrations/aiogram.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2160 2024-05-20 21:22:19.000000 dishka-1.2.0/src/dishka/integrations/aiohttp.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2445 2024-05-16 13:52:24.000000 dishka-1.2.0/src/dishka/integrations/arq.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     5268 2024-05-16 13:52:24.000000 dishka-1.2.0/src/dishka/integrations/base.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1686 2024-05-20 21:22:19.000000 dishka-1.2.0/src/dishka/integrations/fastapi.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     4200 2024-05-20 21:22:19.000000 dishka-1.2.0/src/dishka/integrations/faststream.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1421 2024-05-16 13:52:24.000000 dishka-1.2.0/src/dishka/integrations/flask.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1749 2024-05-16 13:52:24.000000 dishka-1.2.0/src/dishka/integrations/litestar.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1617 2024-05-16 13:52:24.000000 dishka-1.2.0/src/dishka/integrations/sanic.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1619 2024-05-20 21:22:19.000000 dishka-1.2.0/src/dishka/integrations/starlette.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2226 2024-05-16 13:52:24.000000 dishka-1.2.0/src/dishka/integrations/taskiq.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1379 2024-05-16 13:52:24.000000 dishka-1.2.0/src/dishka/integrations/telebot.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     6855 2024-05-16 13:52:24.000000 dishka-1.2.0/src/dishka/provider.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        0 2024-05-16 13:52:24.000000 dishka-1.2.0/src/dishka/py.typed
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)    14023 2024-05-20 21:22:19.000000 dishka-1.2.0/src/dishka/registry.py
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-05-20 21:22:59.500606 dishka-1.2.0/src/dishka.egg-info/
+-rw-r--r--   0 tishka17  (1000) tishka17  (1000)    12011 2024-05-20 21:22:59.000000 dishka-1.2.0/src/dishka.egg-info/PKG-INFO
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2065 2024-05-20 21:22:59.000000 dishka-1.2.0/src/dishka.egg-info/SOURCES.txt
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        1 2024-05-20 21:22:59.000000 dishka-1.2.0/src/dishka.egg-info/dependency_links.txt
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)       50 2024-05-20 21:22:59.000000 dishka-1.2.0/src/dishka.egg-info/requires.txt
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        7 2024-05-20 21:22:59.000000 dishka-1.2.0/src/dishka.egg-info/top_level.txt
```

### Comparing `dishka-1.1.1/LICENSE` & `dishka-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dishka-1.1.1/PKG-INFO` & `dishka-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dishka
-Version: 1.1.1
+Version: 1.2.0
 Summary: Minimal DI framework
 Author-email: Andrey Tikhonov <17@itishka.org>
 License: Apache-2.0
 Project-URL: Source, https://github.com/reagento/dishka
 Project-URL: Homepage, https://github.com/reagento/dishka
 Project-URL: Documentation, https://dishka.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/reagento/dishka/issues
@@ -63,15 +63,15 @@
 
 ```python
 from dishka import Provider
 
 provider = Provider()
 ```
 
-3. Register functions which provide dependencies. Do not forget to place correct typehints for parameters and result. We use `scope=Scope.APP` for dependencies which ar created only once in applicaiton lifetime, and `scope=Scope.REQUEST` for those which should be recreated for each processing request/event/etc.
+3. Register functions which provide dependencies. Do not forget to place correct typehints for parameters and result. We use `scope=Scope.APP` for dependencies which ar created only once in application lifetime, and `scope=Scope.REQUEST` for those which should be recreated for each processing request/event/etc.
 
 ```python
 from dishka import Provider, Scope
 
 def get_a() -> A:
    return A()
 
@@ -163,15 +163,15 @@
 **Container** is what you use to get your dependency. You just call `.get(SomeType)` and it finds a way to get you an instance of that type. It does not create things itself, but manages their lifecycle and caches. It delegates objects creation to providers which are passed during creation.
 
 **Provider** is a collection of functions which really provide some objects. 
 Provider itself is a class with some attributes and methods. Each of them is either result of `provide`, `alias` or `decorate`. They can be used as provider methods, functions to assign attributes or method decorators.
 
 `@provide` can be used as a decorator for some method. This method will be called when corresponding dependency has to be created. Name of the method is not important: just check that it is different form other `Provider` attributes. Type hints do matter: they show what this method creates and what does it require. All method parameters are treated as other dependencies and created using container.
 
-If `provide` is used with some class then that class itself is treated as a factory (`__init__` is analyzed for parameters). But do not forget to assing that call to some attribute otherwise it will be ignored.
+If `provide` is used with some class then that class itself is treated as a factory (`__init__` is analyzed for parameters). But do not forget to assign that call to some attribute otherwise it will be ignored.
 
 **Component** - is an isolated group of providers within the same container identified by a string. When dependency is requested it is searched only within the same component as its dependant, unless it is declared explicitly.
 
 This allows you to have multiple parts of application build separately without need to think if the use same types.
 
 ### Tips
 
@@ -271,21 +271,21 @@
         ...
 
 container = make_container(MyProvider(), context={App: app})
 with container(context={RequestClass: request_instance}) as request_container:
     pass
 ```
 
-* Having to many dependencies? Or maybe want to replace only part of them in tests keeping others? Create multiple `Provider` classes
+* Having too many dependencies? Or maybe want to replace only part of them in tests keeping others? Create multiple `Provider` classes
 
 ```python
 container = make_container(MyProvider(), OtherProvider())
 ```
 
-* Tired of providing `scope==` for each depedency? Set it inside your `Provider` class and all dependencies with no scope will use it.
+* Tired of providing `scope` for each dependency? Set it inside your `Provider` class and all dependencies with no scope will use it.
 
 ```python
 class MyProvider(Provider):
    scope = Scope.APP
 
    @provide
    async def get_a(self) -> A:
```

### Comparing `dishka-1.1.1/README.md` & `dishka-1.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 ```python
 from dishka import Provider
 
 provider = Provider()
 ```
 
-3. Register functions which provide dependencies. Do not forget to place correct typehints for parameters and result. We use `scope=Scope.APP` for dependencies which ar created only once in applicaiton lifetime, and `scope=Scope.REQUEST` for those which should be recreated for each processing request/event/etc.
+3. Register functions which provide dependencies. Do not forget to place correct typehints for parameters and result. We use `scope=Scope.APP` for dependencies which ar created only once in application lifetime, and `scope=Scope.REQUEST` for those which should be recreated for each processing request/event/etc.
 
 ```python
 from dishka import Provider, Scope
 
 def get_a() -> A:
    return A()
 
@@ -140,15 +140,15 @@
 **Container** is what you use to get your dependency. You just call `.get(SomeType)` and it finds a way to get you an instance of that type. It does not create things itself, but manages their lifecycle and caches. It delegates objects creation to providers which are passed during creation.
 
 **Provider** is a collection of functions which really provide some objects. 
 Provider itself is a class with some attributes and methods. Each of them is either result of `provide`, `alias` or `decorate`. They can be used as provider methods, functions to assign attributes or method decorators.
 
 `@provide` can be used as a decorator for some method. This method will be called when corresponding dependency has to be created. Name of the method is not important: just check that it is different form other `Provider` attributes. Type hints do matter: they show what this method creates and what does it require. All method parameters are treated as other dependencies and created using container.
 
-If `provide` is used with some class then that class itself is treated as a factory (`__init__` is analyzed for parameters). But do not forget to assing that call to some attribute otherwise it will be ignored.
+If `provide` is used with some class then that class itself is treated as a factory (`__init__` is analyzed for parameters). But do not forget to assign that call to some attribute otherwise it will be ignored.
 
 **Component** - is an isolated group of providers within the same container identified by a string. When dependency is requested it is searched only within the same component as its dependant, unless it is declared explicitly.
 
 This allows you to have multiple parts of application build separately without need to think if the use same types.
 
 ### Tips
 
@@ -248,21 +248,21 @@
         ...
 
 container = make_container(MyProvider(), context={App: app})
 with container(context={RequestClass: request_instance}) as request_container:
     pass
 ```
 
-* Having to many dependencies? Or maybe want to replace only part of them in tests keeping others? Create multiple `Provider` classes
+* Having too many dependencies? Or maybe want to replace only part of them in tests keeping others? Create multiple `Provider` classes
 
 ```python
 container = make_container(MyProvider(), OtherProvider())
 ```
 
-* Tired of providing `scope==` for each depedency? Set it inside your `Provider` class and all dependencies with no scope will use it.
+* Tired of providing `scope` for each dependency? Set it inside your `Provider` class and all dependencies with no scope will use it.
 
 ```python
 class MyProvider(Provider):
    scope = Scope.APP
 
    @provide
    async def get_a(self) -> A:
```

### Comparing `dishka-1.1.1/pyproject.toml` & `dishka-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "dishka"
-version = "1.1.1"
+version = "1.2.0"
 readme = "README.md"
 authors = [
     { name = "Andrey Tikhonov", email = "17@itishka.org" },
 ]
 license = { text = "Apache-2.0" }
 description = "Minimal DI framework"
 requires-python = ">=3.10"
```

### Comparing `dishka-1.1.1/src/dishka/__init__.py` & `dishka-1.2.0/src/dishka/__init__.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.1/src/dishka/_adaptix/common.py` & `dishka-1.2.0/src/dishka/_adaptix/common.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.1/src/dishka/_adaptix/feature_requirement.py` & `dishka-1.2.0/src/dishka/_adaptix/feature_requirement.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.1/src/dishka/_adaptix/type_tools/__init__.py` & `dishka-1.2.0/src/dishka/_adaptix/type_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.1/src/dishka/_adaptix/type_tools/basic_utils.py` & `dishka-1.2.0/src/dishka/_adaptix/type_tools/basic_utils.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.1/src/dishka/_adaptix/type_tools/constants.py` & `dishka-1.2.0/src/dishka/_adaptix/type_tools/constants.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.1/src/dishka/_adaptix/type_tools/fundamentals.py` & `dishka-1.2.0/src/dishka/_adaptix/type_tools/fundamentals.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.1/src/dishka/_adaptix/type_tools/generic_resolver.py` & `dishka-1.2.0/src/dishka/_adaptix/type_tools/generic_resolver.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.1/src/dishka/_adaptix/type_tools/implicit_params.py` & `dishka-1.2.0/src/dishka/_adaptix/type_tools/implicit_params.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.1/src/dishka/_adaptix/type_tools/norm_utils.py` & `dishka-1.2.0/src/dishka/_adaptix/type_tools/norm_utils.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.1/src/dishka/_adaptix/type_tools/normalize_type.py` & `dishka-1.2.0/src/dishka/_adaptix/type_tools/normalize_type.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.1/src/dishka/async_container.py` & `dishka-1.2.0/src/dishka/async_container.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,59 +1,69 @@
+import warnings
 from asyncio import Lock
-from collections.abc import Callable
+from collections.abc import Callable, MutableMapping
 from typing import Any, Optional, TypeVar
 
 from dishka.entities.component import DEFAULT_COMPONENT, Component
 from dishka.entities.key import DependencyKey
 from dishka.entities.scope import BaseScope, Scope
 from .container_objects import Exit
+from .context_proxy import ContextProxy
 from .dependency_source import FactoryType
 from .exceptions import (
     ExitError,
     NoFactoryError,
 )
 from .provider import BaseProvider
 from .registry import Registry, RegistryBuilder
 
 T = TypeVar("T")
 
 
 class AsyncContainer:
     __slots__ = (
-        "registry", "child_registries", "context", "parent_container",
-        "lock", "_exits", "close_parent",
+        "registry", "child_registries", "parent_container",
+        "lock", "_exits", "close_parent", "_cache", "_context",
     )
 
     def __init__(
             self,
             registry: Registry,
             *child_registries: Registry,
             parent_container: Optional["AsyncContainer"] = None,
             context: dict | None = None,
             lock_factory: Callable[[], Lock] | None = None,
             close_parent: bool = False,
     ):
         self.registry = registry
         self.child_registries = child_registries
-        self.context = {DependencyKey(type(self), DEFAULT_COMPONENT): self}
+        self._context = {DependencyKey(type(self), DEFAULT_COMPONENT): self}
         if context:
             for key, value in context.items():
-                if isinstance(key, DependencyKey):
-                    self.context[key] = value
-                else:
-                    self.context[DependencyKey(key, DEFAULT_COMPONENT)] = value
-
+                if not isinstance(key, DependencyKey):
+                    key = DependencyKey(key, DEFAULT_COMPONENT)
+                self._context[key] = value
+        self._cache = {**self._context}
         self.parent_container = parent_container
         if lock_factory:
             self.lock = lock_factory()
         else:
             self.lock = None
         self._exits: list[Exit] = []
         self.close_parent = close_parent
 
+    @property
+    def context(self) -> MutableMapping[DependencyKey, Any]:
+        warnings.warn(
+            "`container.context` is deprecated",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        return ContextProxy(cache=self._cache, context=self._context)
+
     def __call__(
             self,
             context: dict | None = None,
             lock_factory: Callable[[], Lock] | None = None,
             scope: BaseScope | None = None,
     ) -> "AsyncContextWrapper":
         """
@@ -106,26 +116,25 @@
         key = DependencyKey(dependency_type, component)
         if not lock:
             return await self._get_unlocked(key)
         async with lock:
             return await self._get_unlocked(key)
 
     async def _get_unlocked(self, key: DependencyKey) -> Any:
-        if key in self.context:
-            return self.context[key]
+        if key in self._cache:
+            return self._cache[key]
         compiled = self.registry.get_compiled_async(key)
         if not compiled:
             if not self.parent_container:
                 raise NoFactoryError(key)
             return await self.parent_container.get(
                 key.type_hint, key.component,
             )
         try:
-            return await compiled(self._get_unlocked, self._exits,
-                                  self.context)
+            return await compiled(self._get_unlocked, self._exits, self._cache)
         except NoFactoryError as e:
             e.add_path(self.registry.get_factory(key))
             raise
 
     async def close(self, exception: Exception | None = None):
         errors = []
         for exit_generator in self._exits[::-1]:
@@ -136,14 +145,15 @@
                     exit_generator.callable.send(exception)
             except StopIteration:  # noqa: PERF203
                 pass
             except StopAsyncIteration:
                 pass
             except Exception as err:  # noqa: BLE001
                 errors.append(err)
+        self._cache = {**self._context}
         if self.close_parent:
             try:
                 await self.parent_container.close(exception)
             except Exception as err:  # noqa: BLE001
                 errors.append(err)
         if errors:
             raise ExitError("Cleanup context errors", errors)
```

### Comparing `dishka-1.1.1/src/dishka/container.py` & `dishka-1.2.0/src/dishka/container.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,58 +1,69 @@
-from collections.abc import Callable
+import warnings
+from collections.abc import Callable, MutableMapping
 from threading import Lock
 from typing import Any, Optional, TypeVar
 
 from dishka.entities.component import DEFAULT_COMPONENT, Component
 from dishka.entities.key import DependencyKey
 from dishka.entities.scope import BaseScope, Scope
 from .container_objects import Exit
+from .context_proxy import ContextProxy
 from .dependency_source import FactoryType
 from .exceptions import (
     ExitError,
     NoFactoryError,
 )
 from .provider import BaseProvider
 from .registry import Registry, RegistryBuilder
 
 T = TypeVar("T")
 
 
 class Container:
     __slots__ = (
-        "registry", "child_registries", "context", "parent_container",
-        "lock", "_exits", "close_parent",
+        "registry", "child_registries", "parent_container",
+        "lock", "_exits", "close_parent", "_cache", "_context",
     )
 
     def __init__(
             self,
             registry: Registry,
             *child_registries: Registry,
             parent_container: Optional["Container"] = None,
             context: dict | None = None,
             lock_factory: Callable[[], Lock] | None = None,
             close_parent: bool = False,
     ):
         self.registry = registry
         self.child_registries = child_registries
-        self.context = {DependencyKey(type(self), DEFAULT_COMPONENT): self}
+        self._context = {DependencyKey(type(self), DEFAULT_COMPONENT): self}
         if context:
             for key, value in context.items():
-                if isinstance(key, DependencyKey):
-                    self.context[key] = value
-                else:
-                    self.context[DependencyKey(key, DEFAULT_COMPONENT)] = value
+                if not isinstance(key, DependencyKey):
+                    key = DependencyKey(key, DEFAULT_COMPONENT)
+                self._context[key] = value
+        self._cache = {**self._context}
         self.parent_container = parent_container
         if lock_factory:
             self.lock = lock_factory()
         else:
             self.lock = None
         self._exits: list[Exit] = []
         self.close_parent = close_parent
 
+    @property
+    def context(self) -> MutableMapping[DependencyKey, Any]:
+        warnings.warn(
+            "`container.context` is deprecated",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        return ContextProxy(cache=self._cache, context=self._context)
+
     def __call__(
             self,
             context: dict | None = None,
             lock_factory: Callable[[], Lock] | None = None,
             scope: BaseScope | None = None,
     ) -> "ContextWrapper":
         """
@@ -104,39 +115,40 @@
         key = DependencyKey(dependency_type, component)
         if not lock:
             return self._get_unlocked(key)
         with lock:
             return self._get_unlocked(key)
 
     def _get_unlocked(self, key: DependencyKey) -> Any:
-        if key in self.context:
-            return self.context[key]
+        if key in self._cache:
+            return self._cache[key]
         compiled = self.registry.get_compiled(key)
         if not compiled:
             if not self.parent_container:
                 raise NoFactoryError(key)
             return self.parent_container.get(
                 key.type_hint, key.component,
             )
         try:
-            return compiled(self._get_unlocked, self._exits, self.context)
+            return compiled(self._get_unlocked, self._exits, self._cache)
         except NoFactoryError as e:
             e.add_path(self.registry.get_factory(key))
             raise
 
     def close(self, exception: Exception | None = None) -> None:
         errors = []
         for exit_generator in self._exits[::-1]:
             try:
                 if exit_generator.type is FactoryType.GENERATOR:
                     exit_generator.callable.send(exception)
             except StopIteration:  # noqa: PERF203
                 pass
             except Exception as err:  # noqa: BLE001
                 errors.append(err)
+        self._cache = {**self._context}
         if self.close_parent:
             try:
                 self.parent_container.close(exception)
             except Exception as err:  # noqa: BLE001
                 errors.append(err)
 
         if errors:
```

### Comparing `dishka-1.1.1/src/dishka/dependency_source/__init__.py` & `dishka-1.2.0/src/dishka/dependency_source/__init__.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.1/src/dishka/dependency_source/alias.py` & `dishka-1.2.0/src/dishka/dependency_source/alias.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,13 +28,14 @@
     ) -> Factory:
         return Factory(
             scope=scope,
             source=_identity,
             provides=self.provides.with_component(component),
             is_to_bind=False,
             dependencies=[self.source.with_component(component)],
+            kw_dependencies={},
             type_=FactoryType.ALIAS,
             cache=self.cache,
         )
 
     def __get__(self, instance, owner):
         return self
```

### Comparing `dishka-1.1.1/src/dishka/dependency_source/composite.py` & `dishka-1.2.0/src/dishka/dependency_source/composite.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.1/src/dishka/dependency_source/context_var.py` & `dishka-1.2.0/src/dishka/dependency_source/context_var.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         if component == DEFAULT_COMPONENT:
             return Factory(
                 scope=self.scope,
                 source=context_stub,
                 provides=self.provides,
                 is_to_bind=False,
                 dependencies=[],
+                kw_dependencies={},
                 type_=FactoryType.CONTEXT,
                 cache=False,
             )
         else:
             aliased = Alias(
                 source=self.provides.with_component(DEFAULT_COMPONENT),
                 provides=DependencyKey(self.provides.type_hint,
```

### Comparing `dishka-1.1.1/src/dishka/dependency_source/decorator.py` & `dishka-1.2.0/src/dishka/dependency_source/decorator.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,13 +32,21 @@
                 (
                     new_dependency
                     if dep.type_hint == self.provides.type_hint
                     else dep
                 ).with_component(component)
                 for dep in self.factory.dependencies
             ],
+            kw_dependencies={
+                name: (
+                    new_dependency
+                    if dep.type_hint == self.provides.type_hint
+                    else dep
+                ).with_component(component)
+                for name, dep in self.factory.kw_dependencies.items()
+            },
             type_=self.factory.type,
             cache=cache,
         )
 
     def __get__(self, instance, owner):
         return Decorator(self.factory.__get__(instance, owner))
```

### Comparing `dishka-1.1.1/src/dishka/dependency_source/factory.py` & `dishka-1.2.0/src/dishka/dependency_source/factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from collections.abc import (
+    Mapping,
     Sequence,
 )
 from enum import Enum
-from typing import (
-    Any,
-)
+from typing import Any
 
 from dishka.entities.component import Component
 from dishka.entities.key import DependencyKey
 from dishka.entities.scope import BaseScope
 
 
 class FactoryType(Enum):
@@ -19,30 +18,33 @@
     VALUE = "value"
     ALIAS = "alias"
     CONTEXT = "context"
 
 
 class Factory:
     __slots__ = (
-        "dependencies", "source", "provides", "scope", "type",
+        "dependencies", "kw_dependencies",
+        "source", "provides", "scope", "type",
         "is_to_bind", "cache",
     )
 
     def __init__(
             self,
             *,
             dependencies: Sequence[DependencyKey],
+            kw_dependencies: Mapping[str, DependencyKey],
             source: Any,
             provides: DependencyKey,
             scope: BaseScope | None,
             type_: FactoryType,
             is_to_bind: bool,
             cache: bool,
     ):
         self.dependencies = dependencies
+        self.kw_dependencies = kw_dependencies
         self.source = source
         self.provides = provides
         self.scope = scope
         self.type = type_
         self.is_to_bind = is_to_bind
         self.cache = cache
 
@@ -54,27 +56,32 @@
             source = self.source.__get__(instance, owner)
             dependencies = self.dependencies[1:]
         else:
             source = self.source
             dependencies = self.dependencies[:]
         return Factory(
             dependencies=dependencies,
+            kw_dependencies=self.kw_dependencies,
             source=source,
             provides=self.provides,
             scope=scope,
             type_=self.type,
             is_to_bind=False,
             cache=self.cache,
         )
 
     def with_component(self, component: Component) -> "Factory":
         return Factory(
             dependencies=[
                 d.with_component(component) for d in self.dependencies
             ],
+            kw_dependencies={
+                name: d.with_component(component)
+                for name, d in self.kw_dependencies.items()
+            },
             source=self.source,
             provides=self.provides.with_component(component),
             scope=self.scope,
             is_to_bind=self.is_to_bind,
             cache=self.cache,
             type_=self.type,
         )
```

### Comparing `dishka-1.1.1/src/dishka/dependency_source/make_alias.py` & `dishka-1.2.0/src/dishka/dependency_source/make_alias.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.1/src/dishka/dependency_source/make_context_var.py` & `dishka-1.2.0/src/dishka/dependency_source/make_context_var.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.1/src/dishka/dependency_source/make_decorator.py` & `dishka-1.2.0/src/dishka/dependency_source/make_decorator.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.1/src/dishka/dependency_source/make_factory.py` & `dishka-1.2.0/src/dishka/dependency_source/make_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     Callable,
     Generator,
     Iterable,
     Iterator,
     Sequence,
 )
 from inspect import (
+    Parameter,
     isasyncgenfunction,
     isbuiltin,
     isclass,
     iscoroutinefunction,
     isfunction,
     isgeneratorfunction,
     ismethod,
@@ -210,18 +211,25 @@
             f"If your are using `if TYPE_CHECKING` to import '{e.name}' "
             f"then try removing it. \n"
             f"Or, create a separate factory with all types imported.",
             name=e.name,
         ) from e
 
     hints.pop("return", _empty)
+    params = signature(init).parameters
+    kw_dependency_keys = {
+        name: hint_to_dependency_key(hints.pop(name))
+        for name, param in params.items()
+        if param.kind is Parameter.KEYWORD_ONLY
+    }
     dependencies = list(hints.values())
 
     return Factory(
         dependencies=hints_to_dependency_keys(dependencies),
+        kw_dependencies=kw_dependency_keys,
         type_=FactoryType.FACTORY,
         source=source,
         scope=scope,
         provides=hint_to_dependency_key(provides),
         is_to_bind=False,
         cache=cache,
     )
@@ -263,27 +271,35 @@
     if is_in_class:
         self = next(iter(params.values()), None)
         if self and self.name not in hints:
             # add self to dependencies, so it can be easily removed
             # if we will bind factory to provider instance
             hints = {self.name: Any, **hints}
     possible_dependency = hints.pop("return", _empty)
+
+    kw_dependency_keys = {
+        name: hint_to_dependency_key(hints.pop(name))
+        for name, param in params.items()
+        if param.kind is Parameter.KEYWORD_ONLY
+    }
     dependencies = list(hints.values())
+
     if not provides:
         if possible_dependency is _empty:
             name = getattr(source, "__qualname__", "") or str(source)
             raise ValueError(f"Failed to analyze `{name}`. \n"
                              f"Missing return type hint.")
         try:
             provides = _clean_result_hint(factory_type, possible_dependency)
         except TypeError as e:
             name = getattr(source, "__qualname__", "") or str(source)
             raise TypeError(f"Failed to analyze `{name}`. \n" + str(e)) from e
     return Factory(
         dependencies=hints_to_dependency_keys(dependencies),
+        kw_dependencies=kw_dependency_keys,
         type_=factory_type,
         source=source,
         scope=scope,
         provides=hint_to_dependency_key(provides),
         is_to_bind=is_in_class,
         cache=cache,
     )
@@ -312,28 +328,38 @@
             f"Failed to analyze `{name}`. \n"
             f"Type '{e.name}' is not defined. \n\n"
             f"If your are using `if TYPE_CHECKING` to import '{e.name}' "
             f"then try removing it. \n"
             f"Or, create a separate factory with all types imported.",
             name=e.name,
         ) from e
+
     possible_dependency = hints.pop("return", _empty)
+
+    params = signature(source).parameters
+    kw_dependency_keys = {
+        name: hint_to_dependency_key(hints.pop(name))
+        for name, param in params.items()
+        if param.kind is Parameter.KEYWORD_ONLY
+    }
     dependencies = list(hints.values())
+
     if not provides:
         if possible_dependency is _empty:
             name = getattr(source, "__qualname__", "") or str(source)
             raise ValueError(f"Failed to analyze `{name}`. \n"
                              f"Missing return type hint.")
         try:
             provides = _clean_result_hint(factory_type, possible_dependency)
         except TypeError as e:
             name = getattr(source, "__qualname__", "") or str(source)
             raise TypeError(f"Failed to analyze `{name}`. \n" + str(e)) from e
     return Factory(
         dependencies=hints_to_dependency_keys(dependencies),
+        kw_dependencies=kw_dependency_keys,
         type_=factory_type,
         source=source,
         scope=scope,
         provides=hint_to_dependency_key(provides),
         is_to_bind=False,
         cache=cache,
     )
@@ -359,14 +385,15 @@
     )
     if factory.is_to_bind:
         dependencies = factory.dependencies[1:]  # remove `self`
     else:
         dependencies = factory.dependencies
     return Factory(
         dependencies=dependencies,
+        kw_dependencies=factory.kw_dependencies,
         type_=factory.type,
         source=source,
         scope=scope,
         provides=factory.provides,
         is_to_bind=False,
         cache=cache,
     )
```

### Comparing `dishka-1.1.1/src/dishka/dependency_source/unpack_provides.py` & `dishka-1.2.0/src/dishka/dependency_source/unpack_provides.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,14 +20,15 @@
             source=DependencyKey(provides_first, factory.provides.component),
             cache=factory.cache,
         )
         for provides_other in provides_others
     ]
     res.append(Factory(
         dependencies=factory.dependencies,
+        kw_dependencies=factory.kw_dependencies,
         type_=factory.type,
         source=factory.source,
         scope=factory.scope,
         provides=DependencyKey(provides_first,
                                factory.provides.component),
         is_to_bind=factory.is_to_bind,
         cache=factory.cache,
```

### Comparing `dishka-1.1.1/src/dishka/entities/depends_marker.py` & `dishka-1.2.0/src/dishka/entities/depends_marker.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.1/src/dishka/entities/key.py` & `dishka-1.2.0/src/dishka/entities/key.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.1/src/dishka/entities/scope.py` & `dishka-1.2.0/src/dishka/entities/scope.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.1/src/dishka/error_rendering.py` & `dishka-1.2.0/src/dishka/error_rendering.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.1/src/dishka/exceptions.py` & `dishka-1.2.0/src/dishka/exceptions.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.1/src/dishka/factory_compiler.py` & `dishka-1.2.0/src/dishka/factory_compiler.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,30 +6,40 @@
 * factory_type - factory.type
 * provides - factory.provides
 * Exit
 * NoContextValueError
 * UnsupportedFactoryError
 
 When formatting substituted:
-* await - "async " for async container or empty string
+* await - "await " for async container or empty string
 * async - "async " for async container or empty string
 * args - "getter(arg1), getter(arg2)..." or async version
+* kwargs - "arg1=getter(arg1), arg2=getter(arg2)..." or async version
 * cache - expression to save cache
 """
 
 from .container_objects import CompiledFactory, Exit
 from .dependency_source import Factory, FactoryType
 from .exceptions import NoContextValueError, UnsupportedFactoryError
 
 
-def make_args(names: list[str]):
-    return ", ".join(
-        "{await} getter(%s)" % arg
-        for arg in names
+def make_args(args: list[str], kwargs: list[str]) -> str:
+    res = ", ".join(
+        f"{{await}}getter({arg})"
+        for arg in args
     )
+    if not kwargs:
+        return res
+    if res:
+        res += ", "
+    res += ", ".join(
+        f"{arg}={{await}}getter({arg})"
+        for arg in kwargs
+    )
+    return res
 
 
 GENERATOR = """
 {async}def get(getter, exits, context):
     generator = source({args})
     solved = next(generator)
     exits.append(Exit(factory_type, generator))
@@ -94,39 +104,47 @@
     FactoryType.ALIAS: ALIAS,
 }
 
 CACHE = "context[provides] = solved"
 
 
 def compile_factory(*, factory: Factory, is_async: bool) -> CompiledFactory:
-    names = {f"arg{i}": dep for i, dep in enumerate(factory.dependencies)}
+    args = {
+        f"_dishka_arg{i}": dep
+        for i, dep in enumerate(factory.dependencies)
+    }
+    kwargs = factory.kw_dependencies
+
     if is_async:
         async_ = "async "
         await_ = "await "
         body_template = ASYNC_BODIES.get(factory.type, INVALID)
     else:
         async_ = ""
         await_ = ""
         body_template = SYNC_BODIES.get(factory.type, INVALID)
     if factory.cache:
         cache = CACHE
     else:
         cache = ""
 
-    args = make_args(list(names)).format_map({"await": await_})
+    args_str = make_args(list(args), list(kwargs)).format_map({
+        "await": await_,
+    })
     body = body_template.format_map({
         "async": async_,
         "await": await_,
-        "args": args,
+        "args": args_str,
         "cache": cache,
     })
     func_globals = {
         "source": factory.source,
         "provides": factory.provides,
         "factory_type": factory.type,
         "Exit": Exit,
         "NoContextValueError": NoContextValueError,
         "UnsupportedFactoryError": UnsupportedFactoryError,
-        **names,
+        **args,
+        **kwargs,
     }
     exec(body, func_globals)  # noqa: S102
     return func_globals["get"]
```

### Comparing `dishka-1.1.1/src/dishka/integrations/aiogram.py` & `dishka-1.2.0/src/dishka/integrations/aiogram.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.1/src/dishka/integrations/arq.py` & `dishka-1.2.0/src/dishka/integrations/arq.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.1/src/dishka/integrations/base.py` & `dishka-1.2.0/src/dishka/integrations/base.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.1/src/dishka/integrations/fastapi.py` & `dishka-1.2.0/src/dishka/integrations/fastapi.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,50 +5,58 @@
     "setup_dishka",
 ]
 
 from collections.abc import Callable
 from inspect import Parameter
 from typing import Any, get_type_hints
 
-from fastapi import FastAPI, Request
+from fastapi import FastAPI, Request, WebSocket
 from fastapi.routing import APIRoute
 
 from dishka import AsyncContainer, FromDishka
 from .base import wrap_injection
 from .starlette import ContainerMiddleware
 
 
-def inject(func):
+def inject(func: Callable) -> Callable:
     hints = get_type_hints(func)
-    request_param = next(
+    request_hint = next(
         (name for name, hint in hints.items() if hint is Request),
         None,
     )
-    if request_param:
-        additional_params = []
+    websocket_hint = next(
+        (name for name, hint in hints.items() if hint is WebSocket),
+        None,
+    )
+    if request_hint is None and websocket_hint is None:
+        additional_params = [
+            Parameter(
+                name="___dishka_request",
+                annotation=Request,
+                kind=Parameter.KEYWORD_ONLY,
+            ),
+        ]
     else:
-        request_param = "____dishka_request"
-        additional_params = [Parameter(
-            name=request_param,
-            annotation=Request,
-            kind=Parameter.KEYWORD_ONLY,
-        )]
-
+        additional_params = []
+    param_name = request_hint or websocket_hint or "___dishka_request"
     return wrap_injection(
         func=func,
         remove_depends=True,
-        container_getter=lambda _, p: p[request_param].state.dishka_container,
+        container_getter=lambda _, p: p[param_name].state.dishka_container,
         additional_params=additional_params,
         is_async=True,
     )
 
 
 class DishkaRoute(APIRoute):
     def __init__(
-            self, path: str, endpoint: Callable[..., Any], **kwargs,
+        self,
+        path: str,
+        endpoint: Callable[..., Any],
+        **kwargs,
     ):
         endpoint = inject(endpoint)
         super().__init__(path, endpoint, **kwargs)
 
 
 def setup_dishka(container: AsyncContainer, app: FastAPI) -> None:
     app.add_middleware(ContainerMiddleware)
```

### Comparing `dishka-1.1.1/src/dishka/integrations/faststream.py` & `dishka-1.2.0/src/dishka/integrations/faststream.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 else:
 
     class DishkaMiddleware(_DishkaBaseMiddleware):
         async def consume_scope(
                 self,
                 call_next: Callable[[Any], Awaitable[Any]],
-                msg: StreamMessage[any],
+                msg: StreamMessage[Any],
         ) -> AsyncIterator[DecodedMessage]:
             async with self.container(
                 {
                     StreamMessage: msg,
                     type(msg): msg,
                     ContextRepo: context,
                 },
@@ -104,14 +104,26 @@
 
     else:
         app.broker._middlewares = (  # noqa: SLF001
             DishkaMiddleware(container),
             *app.broker._middlewares,  # noqa: SLF001
         )
 
+        for subscriber in app.broker._subscribers.values():  # noqa: SLF001
+            subscriber._broker_middlewares = (  # noqa: SLF001
+                DishkaMiddleware(container),
+                *subscriber._broker_middlewares,  # noqa: SLF001
+            )
+
+        for publisher in app.broker._publishers.values():  # noqa: SLF001
+            publisher._broker_middlewares = (  # noqa: SLF001
+                DishkaMiddleware(container),
+                *publisher._broker_middlewares,  # noqa: SLF001
+            )
+
         if auto_inject:
             app.broker._call_decorators = (  # noqa: SLF001
                 inject,
                 *app.broker._call_decorators,  # noqa: SLF001
             )
```

### Comparing `dishka-1.1.1/src/dishka/integrations/flask.py` & `dishka-1.2.0/src/dishka/integrations/flask.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.1/src/dishka/integrations/litestar.py` & `dishka-1.2.0/src/dishka/integrations/litestar.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.1/src/dishka/integrations/sanic.py` & `dishka-1.2.0/src/dishka/integrations/sanic.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.1/src/dishka/integrations/starlette.py` & `dishka-1.2.0/src/dishka/integrations/starlette.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,16 +3,18 @@
     "inject",
     "setup_dishka",
 ]
 
 from starlette.applications import Starlette
 from starlette.requests import Request
 from starlette.types import ASGIApp, Receive, Scope, Send
+from starlette.websockets import WebSocket
 
 from dishka import AsyncContainer, FromDishka
+from dishka import Scope as DIScope
 from .base import wrap_injection
 
 
 def inject(func):
     return wrap_injection(
         func=func,
         remove_depends=True,
@@ -25,20 +27,29 @@
 class ContainerMiddleware:
     def __init__(self, app: ASGIApp) -> None:
         self.app = app
 
     async def __call__(
             self, scope: Scope, receive: Receive, send: Send,
     ) -> None:
-        if scope["type"] != "http":
+        if scope["type"] not in ("http", "websocket"):
             return await self.app(scope, receive, send)
 
-        request = Request(scope)
+        if scope["type"] == "http":
+            request = Request(scope)
+            context = {Request: request}
+            di_scope = DIScope.REQUEST
+
+        else:
+            request = WebSocket(scope, receive, send)
+            context = {WebSocket: request}
+            di_scope = DIScope.SESSION
+
         async with request.app.state.dishka_container(
-                {Request: request},
+            context, scope=di_scope,
         ) as request_container:
             request.state.dishka_container = request_container
             return await self.app(scope, receive, send)
 
 
 def setup_dishka(container: AsyncContainer, app: Starlette) -> None:
     app.add_middleware(ContainerMiddleware)
```

### Comparing `dishka-1.1.1/src/dishka/integrations/taskiq.py` & `dishka-1.2.0/src/dishka/integrations/taskiq.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.1/src/dishka/integrations/telebot.py` & `dishka-1.2.0/src/dishka/integrations/telebot.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.1/src/dishka/provider.py` & `dishka-1.2.0/src/dishka/provider.py`

 * *Files identical despite different names*

### Comparing `dishka-1.1.1/src/dishka/registry.py` & `dishka-1.2.0/src/dishka/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,18 +107,32 @@
                 hint = hint[tuple(
                     params_replacement[param]
                     for param in get_type_vars(hint)
                 )]
             new_dependencies.append(DependencyKey(
                 hint, source_dependency.component,
             ))
+        new_kw_dependencies: dict[str, DependencyKey] = {}
+        for name, source_dependency in factory.kw_dependencies.items():
+            hint = source_dependency.type_hint
+            if isinstance(hint, TypeVar):
+                hint = params_replacement[hint]
+            elif get_origin(hint):
+                hint = hint[tuple(
+                    params_replacement[param]
+                    for param in get_type_vars(hint)
+                )]
+            new_kw_dependencies[name] = DependencyKey(
+                hint, source_dependency.component,
+            )
         return Factory(
             source=factory.source,
             provides=dependency_key,
             dependencies=new_dependencies,
+            kw_dependencies=new_kw_dependencies,
             is_to_bind=factory.is_to_bind,
             type_=factory.type,
             scope=factory.scope,
             cache=factory.cache,
         )
 
 
@@ -150,14 +164,19 @@
     ):
         self.path[factory.provides] = factory
         try:
             for dep in factory.dependencies:
                 # ignore TypeVar parameters
                 if not isinstance(dep.type_hint, TypeVar):
                     self._validate_key(dep, registry_index)
+            for dep in factory.kw_dependencies.values():
+                # ignore TypeVar parameters
+                if not isinstance(dep.type_hint, TypeVar):
+                    self._validate_key(dep, registry_index)
+
         except NoFactoryError as e:
             e.add_path(factory)
             raise
         finally:
             self.path.pop(factory.provides)
         self.valid_keys[factory.provides] = True
```

### Comparing `dishka-1.1.1/src/dishka.egg-info/PKG-INFO` & `dishka-1.2.0/src/dishka.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dishka
-Version: 1.1.1
+Version: 1.2.0
 Summary: Minimal DI framework
 Author-email: Andrey Tikhonov <17@itishka.org>
 License: Apache-2.0
 Project-URL: Source, https://github.com/reagento/dishka
 Project-URL: Homepage, https://github.com/reagento/dishka
 Project-URL: Documentation, https://dishka.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/reagento/dishka/issues
@@ -63,15 +63,15 @@
 
 ```python
 from dishka import Provider
 
 provider = Provider()
 ```
 
-3. Register functions which provide dependencies. Do not forget to place correct typehints for parameters and result. We use `scope=Scope.APP` for dependencies which ar created only once in applicaiton lifetime, and `scope=Scope.REQUEST` for those which should be recreated for each processing request/event/etc.
+3. Register functions which provide dependencies. Do not forget to place correct typehints for parameters and result. We use `scope=Scope.APP` for dependencies which ar created only once in application lifetime, and `scope=Scope.REQUEST` for those which should be recreated for each processing request/event/etc.
 
 ```python
 from dishka import Provider, Scope
 
 def get_a() -> A:
    return A()
 
@@ -163,15 +163,15 @@
 **Container** is what you use to get your dependency. You just call `.get(SomeType)` and it finds a way to get you an instance of that type. It does not create things itself, but manages their lifecycle and caches. It delegates objects creation to providers which are passed during creation.
 
 **Provider** is a collection of functions which really provide some objects. 
 Provider itself is a class with some attributes and methods. Each of them is either result of `provide`, `alias` or `decorate`. They can be used as provider methods, functions to assign attributes or method decorators.
 
 `@provide` can be used as a decorator for some method. This method will be called when corresponding dependency has to be created. Name of the method is not important: just check that it is different form other `Provider` attributes. Type hints do matter: they show what this method creates and what does it require. All method parameters are treated as other dependencies and created using container.
 
-If `provide` is used with some class then that class itself is treated as a factory (`__init__` is analyzed for parameters). But do not forget to assing that call to some attribute otherwise it will be ignored.
+If `provide` is used with some class then that class itself is treated as a factory (`__init__` is analyzed for parameters). But do not forget to assign that call to some attribute otherwise it will be ignored.
 
 **Component** - is an isolated group of providers within the same container identified by a string. When dependency is requested it is searched only within the same component as its dependant, unless it is declared explicitly.
 
 This allows you to have multiple parts of application build separately without need to think if the use same types.
 
 ### Tips
 
@@ -271,21 +271,21 @@
         ...
 
 container = make_container(MyProvider(), context={App: app})
 with container(context={RequestClass: request_instance}) as request_container:
     pass
 ```
 
-* Having to many dependencies? Or maybe want to replace only part of them in tests keeping others? Create multiple `Provider` classes
+* Having too many dependencies? Or maybe want to replace only part of them in tests keeping others? Create multiple `Provider` classes
 
 ```python
 container = make_container(MyProvider(), OtherProvider())
 ```
 
-* Tired of providing `scope==` for each depedency? Set it inside your `Provider` class and all dependencies with no scope will use it.
+* Tired of providing `scope` for each dependency? Set it inside your `Provider` class and all dependencies with no scope will use it.
 
 ```python
 class MyProvider(Provider):
    scope = Scope.APP
 
    @provide
    async def get_a(self) -> A:
```

### Comparing `dishka-1.1.1/src/dishka.egg-info/SOURCES.txt` & `dishka-1.2.0/src/dishka.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 src/dishka/__init__.py
 src/dishka/async_container.py
 src/dishka/container.py
 src/dishka/container_objects.py
+src/dishka/context_proxy.py
 src/dishka/error_rendering.py
 src/dishka/exceptions.py
 src/dishka/factory_compiler.py
 src/dishka/provider.py
 src/dishka/py.typed
 src/dishka/registry.py
 src/dishka.egg-info/PKG-INFO
```

