# Comparing `tmp/metar-taf-parser-mivek-1.8.2.tar.gz` & `tmp/metar_taf_parser_mivek-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metar-taf-parser-mivek-1.8.2.tar", last modified: Sun Jan 14 21:30:23 2024, max compression
+gzip compressed data, was "metar_taf_parser_mivek-1.9.0.tar", last modified: Mon May 20 07:42:18 2024, max compression
```

## Comparing `metar-taf-parser-mivek-1.8.2.tar` & `metar_taf_parser_mivek-1.9.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 21:30:23.535304 metar-taf-parser-mivek-1.8.2/
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-01-14 21:30:15.000000 metar-taf-parser-mivek-1.8.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-01-14 21:30:15.000000 metar-taf-parser-mivek-1.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-01-14 21:30:16.000000 metar-taf-parser-mivek-1.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9471 2024-01-14 21:30:23.535304 metar-taf-parser-mivek-1.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8869 2024-01-14 21:30:16.000000 metar-taf-parser-mivek-1.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 21:30:23.523305 metar-taf-parser-mivek-1.8.2/metar_taf_parser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-14 21:30:16.000000 metar-taf-parser-mivek-1.8.2/metar_taf_parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 21:30:23.523305 metar-taf-parser-mivek-1.8.2/metar_taf_parser/command/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-14 21:30:16.000000 metar-taf-parser-mivek-1.8.2/metar_taf_parser/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-01-14 21:30:16.000000 metar-taf-parser-mivek-1.8.2/metar_taf_parser/command/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-01-14 21:30:16.000000 metar-taf-parser-mivek-1.8.2/metar_taf_parser/command/metar.py
--rw-r--r--   0 runner    (1001) docker     (127)    26943 2024-01-14 21:30:16.000000 metar-taf-parser-mivek-1.8.2/metar_taf_parser/command/remark.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-01-14 21:30:16.000000 metar-taf-parser-mivek-1.8.2/metar_taf_parser/command/taf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 21:30:23.523305 metar-taf-parser-mivek-1.8.2/metar_taf_parser/commons/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-14 21:30:16.000000 metar-taf-parser-mivek-1.8.2/metar_taf_parser/commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-01-14 21:30:16.000000 metar-taf-parser-mivek-1.8.2/metar_taf_parser/commons/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-01-14 21:30:16.000000 metar-taf-parser-mivek-1.8.2/metar_taf_parser/commons/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-01-14 21:30:16.000000 metar-taf-parser-mivek-1.8.2/metar_taf_parser/commons/i18n.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 21:30:23.527305 metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 21:30:23.519305 metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 21:30:23.531304 metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11604 2024-01-14 21:30:16.000000 metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    11479 2024-01-14 21:30:16.000000 metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 21:30:23.519305 metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 21:30:23.531304 metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    16704 2024-01-14 21:30:16.000000 metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    16524 2024-01-14 21:30:16.000000 metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/en/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 21:30:23.519305 metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 21:30:23.531304 metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-01-14 21:30:16.000000 metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-01-14 21:30:16.000000 metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 21:30:23.519305 metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 21:30:23.531304 metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    17485 2024-01-14 21:30:16.000000 metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    17307 2024-01-14 21:30:16.000000 metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 21:30:23.519305 metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 21:30:23.531304 metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    12684 2024-01-14 21:30:16.000000 metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    12543 2024-01-14 21:30:16.000000 metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/it/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)    16524 2024-01-14 21:30:16.000000 metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 21:30:23.523305 metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 21:30:23.531304 metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-01-14 21:30:16.000000 metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-01-14 21:30:16.000000 metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 21:30:23.523305 metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/ru-RU/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 21:30:23.531304 metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/ru-RU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    21361 2024-01-14 21:30:16.000000 metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/ru-RU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    21181 2024-01-14 21:30:16.000000 metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/ru-RU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 21:30:23.523305 metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 21:30:23.531304 metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    15112 2024-01-14 21:30:16.000000 metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    14975 2024-01-14 21:30:16.000000 metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 21:30:23.523305 metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/zh-CN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 21:30:23.531304 metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/zh-CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11595 2024-01-14 21:30:16.000000 metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/zh-CN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-01-14 21:30:16.000000 metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/zh-CN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 21:30:23.527305 metar-taf-parser-mivek-1.8.2/metar_taf_parser/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-14 21:30:16.000000 metar-taf-parser-mivek-1.8.2/metar_taf_parser/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-01-14 21:30:16.000000 metar-taf-parser-mivek-1.8.2/metar_taf_parser/model/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    22139 2024-01-14 21:30:16.000000 metar-taf-parser-mivek-1.8.2/metar_taf_parser/model/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 21:30:23.527305 metar-taf-parser-mivek-1.8.2/metar_taf_parser/parser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-14 21:30:16.000000 metar-taf-parser-mivek-1.8.2/metar_taf_parser/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13594 2024-01-14 21:30:16.000000 metar-taf-parser-mivek-1.8.2/metar_taf_parser/parser/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 21:30:23.535304 metar-taf-parser-mivek-1.8.2/metar_taf_parser_mivek.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9471 2024-01-14 21:30:23.000000 metar-taf-parser-mivek-1.8.2/metar_taf_parser_mivek.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-01-14 21:30:23.000000 metar-taf-parser-mivek-1.8.2/metar_taf_parser_mivek.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-14 21:30:23.000000 metar-taf-parser-mivek-1.8.2/metar_taf_parser_mivek.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-14 21:30:23.000000 metar-taf-parser-mivek-1.8.2/metar_taf_parser_mivek.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-01-14 21:30:16.000000 metar-taf-parser-mivek-1.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-01-14 21:30:23.535304 metar-taf-parser-mivek-1.8.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:42:18.966693 metar_taf_parser_mivek-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-05-20 07:42:15.000000 metar_taf_parser_mivek-1.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-20 07:42:15.000000 metar_taf_parser_mivek-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-20 07:42:15.000000 metar_taf_parser_mivek-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9471 2024-05-20 07:42:18.966693 metar_taf_parser_mivek-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8869 2024-05-20 07:42:15.000000 metar_taf_parser_mivek-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:42:18.954692 metar_taf_parser_mivek-1.9.0/metar_taf_parser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 07:42:15.000000 metar_taf_parser_mivek-1.9.0/metar_taf_parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:42:18.954692 metar_taf_parser_mivek-1.9.0/metar_taf_parser/command/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 07:42:15.000000 metar_taf_parser_mivek-1.9.0/metar_taf_parser/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-05-20 07:42:15.000000 metar_taf_parser_mivek-1.9.0/metar_taf_parser/command/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-05-20 07:42:15.000000 metar_taf_parser_mivek-1.9.0/metar_taf_parser/command/metar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26943 2024-05-20 07:42:15.000000 metar_taf_parser_mivek-1.9.0/metar_taf_parser/command/remark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-20 07:42:15.000000 metar_taf_parser_mivek-1.9.0/metar_taf_parser/command/taf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:42:18.954692 metar_taf_parser_mivek-1.9.0/metar_taf_parser/commons/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 07:42:15.000000 metar_taf_parser_mivek-1.9.0/metar_taf_parser/commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-20 07:42:15.000000 metar_taf_parser_mivek-1.9.0/metar_taf_parser/commons/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-20 07:42:15.000000 metar_taf_parser_mivek-1.9.0/metar_taf_parser/commons/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-20 07:42:15.000000 metar_taf_parser_mivek-1.9.0/metar_taf_parser/commons/i18n.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:42:18.958693 metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:42:18.950693 metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:42:18.958693 metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11604 2024-05-20 07:42:15.000000 metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    11479 2024-05-20 07:42:15.000000 metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:42:18.950693 metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:42:18.962693 metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16817 2024-05-20 07:42:15.000000 metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    16642 2024-05-20 07:42:15.000000 metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/en/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:42:18.950693 metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:42:18.962693 metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     6829 2024-05-20 07:42:15.000000 metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-05-20 07:42:15.000000 metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:42:18.950693 metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:42:18.962693 metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16489 2024-05-20 07:42:15.000000 metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    16338 2024-05-20 07:42:15.000000 metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:42:18.950693 metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:42:18.962693 metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    17245 2024-05-20 07:42:15.000000 metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    17092 2024-05-20 07:42:15.000000 metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/it/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)    16642 2024-05-20 07:42:15.000000 metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:42:18.950693 metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:42:18.962693 metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-05-20 07:42:15.000000 metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-05-20 07:42:15.000000 metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:42:18.950693 metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/ru-RU/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:42:18.962693 metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/ru-RU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    21572 2024-05-20 07:42:15.000000 metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/ru-RU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    21397 2024-05-20 07:42:15.000000 metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/ru-RU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:42:18.950693 metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:42:18.962693 metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    14776 2024-05-20 07:42:15.000000 metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    14630 2024-05-20 07:42:15.000000 metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:42:18.950693 metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/zh-CN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:42:18.962693 metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/zh-CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    12570 2024-05-20 07:42:15.000000 metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/zh-CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    12420 2024-05-20 07:42:15.000000 metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/zh-CN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:42:18.958693 metar_taf_parser_mivek-1.9.0/metar_taf_parser/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 07:42:15.000000 metar_taf_parser_mivek-1.9.0/metar_taf_parser/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-20 07:42:15.000000 metar_taf_parser_mivek-1.9.0/metar_taf_parser/model/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22139 2024-05-20 07:42:15.000000 metar_taf_parser_mivek-1.9.0/metar_taf_parser/model/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:42:18.958693 metar_taf_parser_mivek-1.9.0/metar_taf_parser/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 07:42:15.000000 metar_taf_parser_mivek-1.9.0/metar_taf_parser/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13594 2024-05-20 07:42:15.000000 metar_taf_parser_mivek-1.9.0/metar_taf_parser/parser/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:42:18.966693 metar_taf_parser_mivek-1.9.0/metar_taf_parser_mivek.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9471 2024-05-20 07:42:18.000000 metar_taf_parser_mivek-1.9.0/metar_taf_parser_mivek.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-05-20 07:42:18.000000 metar_taf_parser_mivek-1.9.0/metar_taf_parser_mivek.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 07:42:18.000000 metar_taf_parser_mivek-1.9.0/metar_taf_parser_mivek.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-20 07:42:18.000000 metar_taf_parser_mivek-1.9.0/metar_taf_parser_mivek.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-20 07:42:15.000000 metar_taf_parser_mivek-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-20 07:42:18.966693 metar_taf_parser_mivek-1.9.0/setup.cfg
```

### Comparing `metar-taf-parser-mivek-1.8.2/CHANGELOG.md` & `metar_taf_parser_mivek-1.9.0/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Change Log 
 
+## [1.9.0] - 2024-05-19
+
+### Added
+
+- When information about a runway is incomplete in a METAR, a `ParseError` is raised instead of `ValueError`.
+
 ## [1.8.2] - 2024-01-14
 
 ### Fixed
 
 - Fix the calm wind regex to prevent parsing error with visibility.
 - Fix single quotes in French translations.
```

### Comparing `metar-taf-parser-mivek-1.8.2/LICENSE` & `metar_taf_parser_mivek-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metar-taf-parser-mivek-1.8.2/PKG-INFO` & `metar_taf_parser_mivek-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metar-taf-parser-mivek
-Version: 1.8.2
+Version: 1.9.0
 Summary: Python project parsing metar and taf message
 Home-page: https://github.com/mivek/python-metar-taf-parser
 Author: Jean-Kevin KPADEY
 Author-email: jeankevin.kpadey@gmail.com
 Project-URL: Bug Tracker, https://github.com/mivek/python-metar-taf-parser/issues
 Keywords: metar,taf,parser,icao,airport
 Classifier: Programming Language :: Python :: 3
```

### Comparing `metar-taf-parser-mivek-1.8.2/README.md` & `metar_taf_parser_mivek-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `metar-taf-parser-mivek-1.8.2/metar_taf_parser/command/common.py` & `metar_taf_parser_mivek-1.9.0/metar_taf_parser/command/common.py`

 * *Files identical despite different names*

### Comparing `metar-taf-parser-mivek-1.8.2/metar_taf_parser/command/metar.py` & `metar_taf_parser_mivek-1.9.0/metar_taf_parser/command/metar.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import re
 
 from metar_taf_parser.commons import converter
+from metar_taf_parser.commons.exception import ParseError
 from metar_taf_parser.model.enum import DepositType, DepositCoverage
 from metar_taf_parser.model.model import RunwayInfo, Metar
 from metar_taf_parser.commons.i18n import _
 
 
 class AltimeterCommand:
     regex = r'^Q(\d{4})$'
@@ -37,14 +38,30 @@
 
     def execute(self, metar: Metar, input: str):
         matches = self._pattern.search(input).groups()
         mercury = float(matches[0]) / 100
         metar.altimeter = int(converter.convert_inches_mercury_to_pascal(mercury))
 
 
+def _parse_runway(matches, metar, runway):
+    runway.name = matches[0][0]
+    runway.indicator = matches[0][1]
+    runway.min_range = int(matches[0][2])
+    runway.trend = matches[0][3]
+    metar.add_runway_info(runway)
+
+
+def _parse_runway_max_range(matches, metar, runway):
+    runway.name = matches[0][0]
+    runway.min_range = int(matches[0][1])
+    runway.max_range = int(matches[0][2])
+    runway.trend = matches[0][3]
+    metar.add_runway_info(runway)
+
+
 class RunwayCommand:
     generic_regex = r'^(R\d{2}\w?/)'
     runway_max_range_regex = r'^R(\d{2}\w?)/(\d{4})V(\d{3,4})([UDN])?(FT)?'
     runway_regex = r'^R(\d{2}\w?)/([MP])?(\d{4})([UDN])?(FT)?$'
     runway_deposit_regex = r'^R(\d{2}\w?)/([/\d])([/\d])(//|\d{2})(//|\d{2})$'
 
     def __init__(self):
@@ -75,39 +92,37 @@
 
     def can_parse(self, input: str):
         return self._generic_pattern.match(input)
 
     def execute(self, metar: Metar, input: str):
         matches = self._runway_deposit_pattern.findall(input)
         runway = RunwayInfo()
-        if matches:
-            runway.name = matches[0][0]
-            runway.deposit_type = DepositType(matches[0][1])
-            runway.coverage = DepositCoverage(matches[0][2])
-            runway.thickness = self.__parse_deposit_thickness(matches[0][3])
-            runway.braking_capacity = self.__parse_deposit_braking_capacity(matches[0][4])
-            metar.add_runway_info(runway)
-            return
-
-        matches = self._runway_pattern.findall(input)
-        if matches:
-            runway.name = matches[0][0]
-            runway.indicator = matches[0][1]
-            runway.min_range = int(matches[0][2])
-            runway.trend = matches[0][3]
-            metar.add_runway_info(runway)
-            return
-
-        matches = self._max_range_pattern.findall(input)
-        if matches:
-            runway.name = matches[0][0]
-            runway.min_range = int(matches[0][1])
-            runway.max_range = int(matches[0][2])
-            runway.trend = matches[0][3]
-            metar.add_runway_info(runway)
+        try:
+            if matches:
+                self.__parse_runway_deposit(matches, metar, runway)
+                return
+
+            matches = self._runway_pattern.findall(input)
+            if matches:
+                _parse_runway(matches, metar, runway)
+                return
+
+            matches = self._max_range_pattern.findall(input)
+            if matches:
+                _parse_runway_max_range(matches, metar, runway)
+        except ValueError:
+            raise ParseError(_("ErrorCode.IncompleteRunwayInformation"))
+
+    def __parse_runway_deposit(self, matches, metar, runway):
+        runway.name = matches[0][0]
+        runway.deposit_type = DepositType(matches[0][1])
+        runway.coverage = DepositCoverage(matches[0][2])
+        runway.thickness = self.__parse_deposit_thickness(matches[0][3])
+        runway.braking_capacity = self.__parse_deposit_braking_capacity(matches[0][4])
+        metar.add_runway_info(runway)
 
     def __parse_deposit_thickness(self, input):
         thickness = self._deposit_thickness.get(input, 'DepositThickness.default')
         return _(thickness).format(input)
 
     def __parse_deposit_braking_capacity(self, input):
         braking_capacity = self._deposit_braking_capacity.get(input, 'DepositBrakingCapacity.default')
```

### Comparing `metar-taf-parser-mivek-1.8.2/metar_taf_parser/command/remark.py` & `metar_taf_parser_mivek-1.9.0/metar_taf_parser/command/remark.py`

 * *Files identical despite different names*

### Comparing `metar-taf-parser-mivek-1.8.2/metar_taf_parser/command/taf.py` & `metar_taf_parser_mivek-1.9.0/metar_taf_parser/command/taf.py`

 * *Files identical despite different names*

### Comparing `metar-taf-parser-mivek-1.8.2/metar_taf_parser/commons/converter.py` & `metar_taf_parser_mivek-1.9.0/metar_taf_parser/commons/converter.py`

 * *Files identical despite different names*

### Comparing `metar-taf-parser-mivek-1.8.2/metar_taf_parser/commons/i18n.py` & `metar_taf_parser_mivek-1.9.0/metar_taf_parser/commons/i18n.py`

 * *Files identical despite different names*

### Comparing `metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/de/LC_MESSAGES/messages.mo` & `metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/de/LC_MESSAGES/messages.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -4,15 +4,15 @@
 "PO-Revision-Date: \n"
 "Last-Translator: \n"
 "Language-Team: \n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"X-Generator: Poedit 3.2.2\n"
+"X-Generator: Poedit 3.4.2\n"
 
 msgid "CloudQuantity.BKN"
 msgstr "stark bewölkt"
 
 msgid "CloudQuantity.FEW"
 msgstr "leicht bewölkt"
```

### Comparing `metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/de/LC_MESSAGES/messages.po` & `metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/en/LC_MESSAGES/messages.mo` & `metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/en/LC_MESSAGES/messages.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -4,15 +4,15 @@
 "PO-Revision-Date: \n"
 "Last-Translator: \n"
 "Language-Team: \n"
 "Language: en\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"X-Generator: Poedit 3.4.1\n"
+"X-Generator: Poedit 3.4.2\n"
 
 msgid "CloudQuantity.BKN"
 msgstr "broken"
 
 msgid "CloudQuantity.FEW"
 msgstr "few"
 
@@ -252,14 +252,17 @@
 
 msgid "Error.prefix"
 msgstr "An error occured. Error code n°"
 
 msgid "ErrorCode.AirportNotFound"
 msgstr "The airport was not found for this message."
 
+msgid "ErrorCode.IncompleteRunwayInformation"
+msgstr "The runway information is incomplete and cannot be parsed."
+
 msgid "ErrorCode.InvalidMessage"
 msgstr "The entered message is invalid."
 
 msgid "Flag.AMD"
 msgstr "amended TAF"
 
 msgid "Flag.AUTO"
```

### Comparing `metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/en/LC_MESSAGES/messages.po` & `metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/en/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -255,14 +255,18 @@
 msgstr "The airport was not found for this message."
 
 #:
 msgid "ErrorCode.InvalidMessage"
 msgstr "The entered message is invalid."
 
 #:
+msgid "ErrorCode.IncompleteRunwayInformation"
+msgstr "The runway information is incomplete and cannot be parsed."
+
+#:
 msgid "Flag.AMD"
 msgstr "amended TAF"
 
 #:
 msgid "Flag.AUTO"
 msgstr "automated METAR"
```

### Comparing `metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/es/LC_MESSAGES/messages.po` & `metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/pl/LC_MESSAGES/messages.po`

 * *Files 26% similar despite different names*

```diff
@@ -1,256 +1,300 @@
 msgid ""
 msgstr ""
 "MIME-Version: 1.0"
 "Content-Type: text/plain; charset=UTF-8"
 "Content-Transfer-Encoding: 8bit"
 "X-Generator: prop2po"
 "Project-Id-Version: metar_taf_parser"
-"Language: es"
+"Language: pl"
+#:
+msgid "CloudQuantity.BKN"
+msgstr "Od 5/8 do 7/8"
+
+#:
+msgid "CloudQuantity.FEW"
+msgstr "Od 1/8 do 2/8"
+
 #:
 msgid "CloudQuantity.NSC"
-msgstr "sin nubes significativas."
+msgstr "Nieznaczne zachmurzenie."
 
 #:
 msgid "CloudQuantity.OVC"
-msgstr "cubierto"
+msgstr "8/8"
+
+#:
+msgid "CloudQuantity.SCT"
+msgstr "Od 3/8 do 4/8"
 
 #:
 msgid "CloudQuantity.SKC"
-msgstr "cielo claro"
+msgstr "Czyste niebo"
 
 #:
 msgid "CloudType.AC"
-msgstr "Altocumulus"
+msgstr "Średnie kłębiaste"
 
 #:
 msgid "CloudType.AS"
-msgstr "Altostratus"
+msgstr "Średnia warstwowa"
 
 #:
 msgid "CloudType.CB"
-msgstr "Cumulonimbus"
+msgstr "Kłębiasta deszczowa"
 
 #:
 msgid "CloudType.CC"
-msgstr "Cirrocumulus"
+msgstr "Piętra wysokiego rodzaj kłębiasto-pierzaste"
 
 #:
 msgid "CloudType.CI"
-msgstr "Cirrus"
+msgstr "Pierzasta"
 
 #:
 msgid "CloudType.CS"
-msgstr "Cirrostratus"
+msgstr "Warstwowo - pierzasta"
 
 #:
 msgid "CloudType.CU"
-msgstr "Cumulus"
+msgstr "Kłębiasta"
 
 #:
 msgid "CloudType.NS"
-msgstr "Nimbostratus"
+msgstr "Warstwowa deszczowa"
 
 #:
 msgid "CloudType.SC"
-msgstr "Stratocumulus"
+msgstr "Kłębiasto warstwowa"
 
 #:
 msgid "CloudType.ST"
-msgstr "Stratus"
+msgstr "Warstwowa"
 
 #:
 msgid "CloudType.TCU"
-msgstr "Torrecumulus"
+msgstr "Wypiętrzona chmura kłębiasta"
+
+#:
+msgid "Descriptive.BC"
+msgstr "płaty"
+
+#:
+msgid "Descriptive.BL"
+msgstr "zawieja"
+
+#:
+msgid "Descriptive.DR"
+msgstr "zamieć przyziemna"
+
+#:
+msgid "Descriptive.FZ"
+msgstr "opad marznący"
 
 #:
-msgid "DepositBrakingCapacity.//"
-msgstr "no reportado"
+msgid "Descriptive.MI"
+msgstr "niskie"
 
 #:
-msgid "DepositCoverage.LESS_10"
-msgstr "menos de 10%"
+msgid "Descriptive.PR"
+msgstr "częściowe"
 
 #:
-msgid "DepositCoverage.FROM_11_TO_25"
-msgstr "de 11% a 25%"
+msgid "Descriptive.SH"
+msgstr "opad przelotny"
 
 #:
-msgid "DepositCoverage.FROM_26_TO_50"
-msgstr "de 26% a 50%"
+msgid "Descriptive.TS"
+msgstr "burza"
 
 #:
-msgid "DepositCoverage.FROM_51_TO_100"
-msgstr "de 51% a 100%"
+msgid "Error.prefix"
+msgstr "Wystąpił błąd. Kod błędu numer"
 
 #:
-msgid "DepositThickness.//"
-msgstr "no reportado"
+msgid "ErrorCode.AirportNotFound"
+msgstr "Nie znaleziono lotniska w tej depeszy."
 
 #:
-msgid "DepositThickness.00"
-msgstr "menos de 1 mm"
+msgid "ErrorCode.InvalidMessage"
+msgstr "Wprowadzona depesza jest nieprawidłowa."
 
 #:
-msgid "DepositThickness.THICKNESS_10"
-msgstr "10 cm"
+msgid "Intensity.-"
+msgstr "Słaby"
 
 #:
-msgid "DepositThickness.THICKNESS_15"
-msgstr "15 cm"
+msgid "Intensity.+"
+msgstr "Silny"
 
 #:
-msgid "DepositThickness.THICKNESS_20"
-msgstr "20 cm"
+msgid "Intensity.VC"
+msgstr "W pobliżu"
 
 #:
-msgid "DepositThickness.THICKNESS_25"
-msgstr "25 cm"
+msgid "Phenomenon.BR"
+msgstr "zamglenie"
 
 #:
-msgid "DepositThickness.THICKNESS_30"
-msgstr "30 cm"
+msgid "Phenomenon.DS"
+msgstr "burza piaskowa"
 
 #:
-msgid "DepositThickness.THICKNESS_35"
-msgstr "35 cm"
+msgid "Phenomenon.DU"
+msgstr "pył"
 
 #:
-msgid "DepositThickness.98"
-msgstr "40 cm o más"
+msgid "Phenomenon.DZ"
+msgstr "mżawka"
 
 #:
-msgid "DepositThickness.99"
-msgstr "cerrado"
+msgid "Phenomenon.FC"
+msgstr "trąba powietrzna"
 
 #:
-msgid "DepositType.NOT_REPORTED"
-msgstr "no reportado"
+msgid "Phenomenon.FG"
+msgstr "mgła"
 
 #:
-msgid "DepositType.CLEAR_DRY"
-msgstr "claro y seco"
+msgid "Phenomenon.FU"
+msgstr "dym"
 
 #:
-msgid "DepositType.DAMP"
-msgstr "húmedo"
+msgid "Phenomenon.GR"
+msgstr "grad"
 
 #:
-msgid "DepositType.WET_WATER_PATCHES"
-msgstr "húmedo o con charcos"
+msgid "Phenomenon.GS"
+msgstr "krupa śnieżna"
 
 #:
-msgid "DepositType.RIME_FROST_COVERED"
-msgstr "escarcha o cubierto de hielo"
+msgid "Phenomenon.HZ"
+msgstr "zmętnienie"
 
 #:
-msgid "DepositType.DRY_SNOW"
-msgstr "nieve seca"
+msgid "Phenomenon.IC"
+msgstr "słupki lodowe"
 
 #:
-msgid "DepositType.WET_SNOW"
-msgstr "nieve húmeda"
+msgid "Phenomenon.PL"
+msgstr "deszcz lodowy"
 
 #:
-msgid "DepositType.ICE"
-msgstr "hielo"
+msgid "Phenomenon.PO"
+msgstr "wiry pyłowe"
 
 #:
-msgid "DepositType.COMPACTED_SNOW"
-msgstr "nieve compactada o enrollada"
+msgid "Phenomenon.PY"
+msgstr "aerozol"
 
 #:
-msgid "DepositType.FROZEN_RIDGES"
-msgstr "huellas o cumbres congeladas"
+msgid "Phenomenon.RA"
+msgstr "deszcz"
 
 #:
-msgid "DepositType.SLUSH"
-msgstr "nieve derretida"
+msgid "Phenomenon.SA"
+msgstr "piasek"
+
+#:
+msgid "Phenomenon.SG"
+msgstr "śnieg ziarnisty"
+
+#:
+msgid "Phenomenon.SN"
+msgstr "śnieg"
+
+#:
+msgid "Phenomenon.SQ"
+msgstr "nawałnica"
 
 #:
 msgid "Phenomenon.SS"
-msgstr "tormenta de arena"
+msgstr "burza piaskowa"
 
 #:
 msgid "Phenomenon.UP"
-msgstr "precipitación desconocida"
+msgstr "marznący deszcz"
 
 #:
 msgid "Phenomenon.VA"
-msgstr "ceniza volcánica"
+msgstr "popiół wulkaniczny"
+
+#:
+msgid "MetarFacade.InvalidIcao"
+msgstr "Kod Icao jest nieprawidłowy"
 
 #:
-msgid "Phenomenon.TS"
-msgstr "tormenta"
+msgid "Converter.D"
+msgstr "malejący"
 
 #:
-msgid "Remark.AO1"
-msgstr "estaciones automáticas sin discriminador de precipitación"
+msgid "Converter.E"
+msgstr "wschód"
 
 #:
-msgid "Remark.AO2"
-msgstr "estaciones automáticas con discriminador de precipitación"
+msgid "Converter.N"
+msgstr "północ"
 
 #:
-msgid "Remark.ALQDS"
-msgstr "todos los cuadrantes"
+msgid "Converter.NE"
+msgstr "północny wschód"
 
 #:
-msgid "Remark.Barometer.0"
-msgstr "Subiendo, después bajando"
+msgid "Converter.NSC"
+msgstr "nieznaczna zmiana"
 
 #:
-msgid "Remark.Barometer.1"
-msgstr "Subiendo, después estacionaria; o subiendo,\ndespués aumentando con más lentitud"
+msgid "Converter.NW"
+msgstr "północny zachód"
 
 #:
-msgid "Remark.Barometer.2"
-msgstr "subiendo, regular o irregularmente"
+msgid "Converter.S"
+msgstr "południe"
 
 #:
-msgid "Remark.Barometer.3"
-msgstr "Bajando o estacionaria; después subiendo; o subiendo y después subiendo más rápidamente"
+msgid "Converter.SE"
+msgstr "południowy zachód"
 
 #:
-msgid "Remark.Barometer.4"
-msgstr "Estacionaria"
+msgid "Converter.SW"
+msgstr "połódniowy wschód"
 
 #:
-msgid "Remark.Barometer.5"
-msgstr "Bajando, después subiendo"
+msgid "Converter.U"
+msgstr "rosnący"
 
 #:
-msgid "Remark.Barometer.6"
-msgstr "Bajando, después estacionaria; o bajando y\ndespués bajando más lentamente"
+msgid "Converter.VRB"
+msgstr "Zmienny"
 
 #:
-msgid "Remark.Barometer.7"
-msgstr "Bajando, regular o irregularmente"
+msgid "Converter.W"
+msgstr "zachód"
 
 #:
-msgid "Remark.Barometer.8"
-msgstr "Estacionaria o subiendo y después bajando; o bajando y después bajando más rápidamente"
+msgid "WeatherChangeType.FM"
+msgstr "od"
 
 #:
-msgid "Remark.BASED"
-msgstr "basado"
+msgid "WeatherChangeType.BECMG"
+msgstr "Nadchodząca"
 
 #:
-msgid "Remark.Ceiling.Height"
-msgstr "techo de nubes entre {0} y {1} pies"
+msgid "WeatherChangeType.TEMPO"
+msgstr "Tymczasowa"
 
 #:
-msgid "Remark.Ceiling.Second.Location"
-msgstr "techo de nubes de {0} pies medido por un segundo sensor ubicado en {1}"
+msgid "WeatherChangeType.PROB"
+msgstr "Prawdopodobieństwo"
 
 #:
-msgid "Remark.DSNT"
-msgstr "distante"
+msgid "TimeIndicator.AT"
+msgstr "o"
 
 #:
-msgid "Remark.FCST"
-msgstr "pronóstico"
+msgid "TimeIndicator.FM"
+msgstr "od"
 
 #:
-msgid "Remark.FUNNELCLOUD"
-msgstr "nube embudo"
+msgid "TimeIndicator.TL"
+msgstr "do"
```

### Comparing `metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/fr/LC_MESSAGES/messages.mo` & `metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/fr/LC_MESSAGES/messages.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -4,15 +4,15 @@
 "PO-Revision-Date: \n"
 "Last-Translator: \n"
 "Language-Team: \n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"X-Generator: Poedit 3.4\n"
+"X-Generator: Poedit 3.4.2\n"
 
 msgid "CloudQuantity.BKN"
 msgstr "nuages fragmentés"
 
 msgid "CloudQuantity.FEW"
 msgstr "peu"
 
@@ -24,44 +24,20 @@
 
 msgid "CloudQuantity.SCT"
 msgstr "nuages épars"
 
 msgid "CloudQuantity.SKC"
 msgstr "pas de nuage"
 
-msgid "CloudType.AC"
-msgstr "Altocumulus"
-
-msgid "CloudType.AS"
-msgstr "Altostratus"
-
 msgid "CloudType.CB"
 msgstr "Cumunolinbus"
 
 msgid "CloudType.CC"
 msgstr "Cirrocumulus"
 
-msgid "CloudType.CI"
-msgstr "Cirrus"
-
-msgid "CloudType.CS"
-msgstr "Cirrostratus"
-
-msgid "CloudType.CU"
-msgstr "Cumulus"
-
-msgid "CloudType.NS"
-msgstr "Nimbostratus"
-
-msgid "CloudType.SC"
-msgstr "Stratocumulus"
-
-msgid "CloudType.ST"
-msgstr "Stratus"
-
 msgid "CloudType.TCU"
 msgstr "Cumulus bourgeonnant"
 
 msgid "Converter.D"
 msgstr "decroissant"
 
 msgid "Converter.E"
@@ -105,17 +81,14 @@
 
 msgid "Converter.SW"
 msgstr "Sud Ouest"
 
 msgid "Converter.U"
 msgstr "accroissement"
 
-msgid "Converter.VRB"
-msgstr "Variable"
-
 msgid "Converter.W"
 msgstr "Ouest"
 
 msgid "Converter.WNW"
 msgstr "Ouest Nord Ouest"
 
 msgid "Converter.WSW"
@@ -138,17 +111,14 @@
 
 msgid "DepositBrakingCapacity.95"
 msgstr "bonne"
 
 msgid "DepositBrakingCapacity.99"
 msgstr "valeurs non fiables"
 
-msgid "DepositBrakingCapacity.default"
-msgstr "friction coefficient of {0}"
-
 msgid "DepositCoverage.FROM_11_TO_25"
 msgstr "de 11% à 25%"
 
 msgid "DepositCoverage.FROM_26_TO_50"
 msgstr "de 26% à 50%"
 
 msgid "DepositCoverage.FROM_51_TO_100"
@@ -162,41 +132,20 @@
 
 msgid "DepositThickness.//"
 msgstr "non reportée"
 
 msgid "DepositThickness.00"
 msgstr "moins de 1 mm"
 
-msgid "DepositThickness.92"
-msgstr "10 cm"
-
-msgid "DepositThickness.93"
-msgstr "15 cm"
-
-msgid "DepositThickness.94"
-msgstr "20 cm"
-
-msgid "DepositThickness.95"
-msgstr "25 cm"
-
-msgid "DepositThickness.96"
-msgstr "30 cm"
-
-msgid "DepositThickness.97"
-msgstr "35 cm"
-
 msgid "DepositThickness.98"
 msgstr "40 cm ou plus"
 
 msgid "DepositThickness.99"
 msgstr "fermée"
 
-msgid "DepositThickness.default"
-msgstr "{0} mm"
-
 msgid "DepositType.CLEAR_DRY"
 msgstr "clair et sec"
 
 msgid "DepositType.COMPACTED_SNOW"
 msgstr "neige compactée ou roulée"
 
 msgid "DepositType.DAMP"
@@ -252,14 +201,19 @@
 
 msgid "Error.prefix"
 msgstr "Une erreur est survenue. Code erreur n°"
 
 msgid "ErrorCode.AirportNotFound"
 msgstr "L'aéroport n'a pas été trouvé pour ce message."
 
+msgid "ErrorCode.IncompleteRunwayInformation"
+msgstr ""
+"Les informations sur la piste sont incomplètes et ne peuvent pas être "
+"analysées."
+
 msgid "ErrorCode.InvalidMessage"
 msgstr "Le message entré est invalide."
 
 msgid "Flag.AMD"
 msgstr "TAF modifié"
 
 msgid "Flag.AUTO"
@@ -360,17 +314,14 @@
 
 msgid "Phenomenon.PL"
 msgstr "granules de glace"
 
 msgid "Phenomenon.PO"
 msgstr "tourbillon de poussières sable"
 
-msgid "Phenomenon.PY"
-msgstr "spray"
-
 msgid "Phenomenon.RA"
 msgstr "pluie"
 
 msgid "Phenomenon.SA"
 msgstr "sable"
 
 msgid "Phenomenon.SG"
@@ -478,15 +429,15 @@
 msgstr "température horaire de {0}°C"
 
 msgid "Remark.Hourly.Temperature.Dew.Point"
 msgstr "température horaire de {0}°C et point de rosée de {1}°C"
 
 msgid "Remark.Ice.Accretion.Amount"
 msgstr ""
-"{0}/100 d'un pouce d'accrétion de glace au cours des {1} dernières heures"
+"{0}/100 d''un pouce d''accrétion de glace au cours des {1} dernières heures"
 
 msgid "Remark.LGT"
 msgstr "léger"
 
 msgid "Remark.LTG"
 msgstr "éclair"
 
@@ -515,15 +466,15 @@
 msgstr "{0} pouces de précipitations tombées au cours des 24 dernières heures"
 
 msgid "Remark.Precipitation.Amount.3.6"
 msgstr "{1} pouces de précipitations tombées au cours des {0} dernières heures"
 
 msgid "Remark.Precipitation.Amount.Hourly"
 msgstr ""
-"{0}/100 d'un pouce de précipitation est tombé au cours de la dernière heure"
+"{0}/100 d''un pouce de précipitation est tombé au cours de la dernière heure"
 
 msgid "Remark.Precipitation.Beg"
 msgstr "{0} {1} commençant à {2}:{3}"
 
 msgid "Remark.Precipitation.Beg.End"
 msgstr "{0} {1} commencant à {2}:{3} finissant à {4}:{5}"
 
@@ -553,15 +504,15 @@
 "épaisseur de neige de {0} pouces sur la dernière heure avec une épaisseur "
 "totale au sol de {1} pouces"
 
 msgid "Remark.Snow.Pellets"
 msgstr "{0} grésil"
 
 msgid "Remark.Sunshine.Duration"
-msgstr "{0} minutes d'ensoleillement"
+msgstr "{0} minutes d''ensoleillement"
 
 msgid "Remark.Surface.Visibility"
 msgstr "visibility de surface de {0} miles"
 
 msgid "Remark.TORNADO"
 msgstr "tornade"
 
@@ -579,17 +530,14 @@
 
 msgid "Remark.Tornadic.Activity.Ending"
 msgstr "{0} finissant à {1}:{2} {3} SM {4} de la station"
 
 msgid "Remark.Tower.Visibility"
 msgstr "visibility de la tour de contrôle de {0} miles"
 
-msgid "Remark.VIRGA"
-msgstr "virga"
-
 msgid "Remark.Variable.Prevailing.Visibility"
 msgstr "variation de la visibilité dominante entre {0} et {1} SM"
 
 msgid "Remark.Variable.Sky.Condition"
 msgstr "couche de nuages variant entre {0} et {1}"
 
 msgid "Remark.Variable.Sky.Condition.Height"
@@ -598,21 +546,21 @@
 msgid "Remark.Virga.Direction"
 msgstr "virga au {0} de la station"
 
 msgid "Remark.WATERSPOUT"
 msgstr "trombe"
 
 msgid "Remark.Water.Equivalent.Snow.Ground"
-msgstr "équivalent d'eau de {0} pouces de neige"
+msgstr "équivalent d''eau de {0} pouces de neige"
 
 msgid "Remark.WindShift"
 msgstr "changement de vent à {0}:{1}"
 
 msgid "Remark.WindShift.FROPA"
-msgstr "changement de vent accompagné d'un passage de front à {0}:{1}"
+msgstr "changement de vent accompagné d''un passage de front à {0}:{1}"
 
 msgid "TimeIndicator.AT"
 msgstr "à"
 
 msgid "TimeIndicator.FM"
 msgstr "De"
 
@@ -624,23 +572,17 @@
 
 msgid "ToString.altimeter"
 msgstr "altimètre (hPa)"
 
 msgid "ToString.amendment"
 msgstr "amendement"
 
-msgid "ToString.auto"
-msgstr "auto"
-
 msgid "ToString.baseHeight"
 msgstr "Base de la couche en pied"
 
-msgid "ToString.cavok"
-msgstr "cavok"
-
 msgid "ToString.clouds"
 msgstr "nuages"
 
 msgid "ToString.day.hour"
 msgstr "heure du jour"
 
 msgid "ToString.day.month"
@@ -690,17 +632,14 @@
 
 msgid "ToString.message"
 msgstr "message original"
 
 msgid "ToString.name"
 msgstr "nom"
 
-msgid "ToString.nosig"
-msgstr "nosig"
-
 msgid "ToString.phenomenons"
 msgstr "phénomènes"
 
 msgid "ToString.probability"
 msgstr "probabilité"
 
 msgid "ToString.quantity"
@@ -735,17 +674,14 @@
 
 msgid "ToString.trend"
 msgstr "tendance"
 
 msgid "ToString.trends"
 msgstr "tendances"
 
-msgid "ToString.type"
-msgstr "type"
-
 msgid "ToString.vertical.visibility"
 msgstr "visibilité verticale (pieds)"
 
 msgid "ToString.visibility.main"
 msgstr "visibilité principale"
 
 msgid "ToString.visibility.max"
@@ -756,17 +692,14 @@
 
 msgid "ToString.visibility.min.direction"
 msgstr "direction de la visibilité minimale"
 
 msgid "ToString.weather.conditions"
 msgstr "conditions météorologique"
 
-msgid "ToString.wind.direction"
-msgstr "direction"
-
 msgid "ToString.wind.direction.degrees"
 msgstr "direction (degrés)"
 
 msgid "ToString.wind.gusts"
 msgstr "rafales"
 
 msgid "ToString.wind.max.variation"
```

### Comparing `metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/fr/LC_MESSAGES/messages.po` & `metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/fr/LC_MESSAGES/messages.po`

 * *Files 8% similar despite different names*

```diff
@@ -27,54 +27,22 @@
 msgstr "nuages épars"
 
 #:
 msgid "CloudQuantity.SKC"
 msgstr "pas de nuage"
 
 #:
-msgid "CloudType.AC"
-msgstr "Altocumulus"
-
-#:
-msgid "CloudType.AS"
-msgstr "Altostratus"
-
-#:
 msgid "CloudType.CB"
 msgstr "Cumunolinbus"
 
 #:
 msgid "CloudType.CC"
 msgstr "Cirrocumulus"
 
 #:
-msgid "CloudType.CI"
-msgstr "Cirrus"
-
-#:
-msgid "CloudType.CS"
-msgstr "Cirrostratus"
-
-#:
-msgid "CloudType.CU"
-msgstr "Cumulus"
-
-#:
-msgid "CloudType.NS"
-msgstr "Nimbostratus"
-
-#:
-msgid "CloudType.SC"
-msgstr "Stratocumulus"
-
-#:
-msgid "CloudType.ST"
-msgstr "Stratus"
-
-#:
 msgid "CloudType.TCU"
 msgstr "Cumulus bourgeonnant"
 
 #:
 msgid "DepositBrakingCapacity.//"
 msgstr "non reportée"
 
@@ -99,18 +67,14 @@
 msgstr "bonne"
 
 #:
 msgid "DepositBrakingCapacity.99"
 msgstr "valeurs non fiables"
 
 #:
-msgid "DepositBrakingCapacity.default"
-msgstr "friction coefficient of {0}"
-
-#:
 msgid "DepositCoverage.NOT_REPORTED"
 msgstr "non reportée"
 
 #:
 msgid "DepositCoverage.LESS_10"
 msgstr "moins de 10%"
 
@@ -131,50 +95,22 @@
 msgstr "non reportée"
 
 #:
 msgid "DepositThickness.00"
 msgstr "moins de 1 mm"
 
 #:
-msgid "DepositThickness.92"
-msgstr "10 cm"
-
-#:
-msgid "DepositThickness.93"
-msgstr "15 cm"
-
-#:
-msgid "DepositThickness.94"
-msgstr "20 cm"
-
-#:
-msgid "DepositThickness.95"
-msgstr "25 cm"
-
-#:
-msgid "DepositThickness.96"
-msgstr "30 cm"
-
-#:
-msgid "DepositThickness.97"
-msgstr "35 cm"
-
-#:
 msgid "DepositThickness.98"
 msgstr "40 cm ou plus"
 
 #:
 msgid "DepositThickness.99"
 msgstr "fermée"
 
 #:
-msgid "DepositThickness.default"
-msgstr "{0} mm"
-
-#:
 msgid "DepositType.NOT_REPORTED"
 msgstr "non reportée"
 
 #:
 msgid "DepositType.CLEAR_DRY"
 msgstr "clair et sec"
 
@@ -255,14 +191,18 @@
 msgstr "L'aéroport n'a pas été trouvé pour ce message."
 
 #:
 msgid "ErrorCode.InvalidMessage"
 msgstr "Le message entré est invalide."
 
 #:
+msgid "ErrorCode.IncompleteRunwayInformation"
+msgstr "Les informations sur la piste sont incomplètes et ne peuvent pas être analysées."
+
+#:
 msgid "Flag.AMD"
 msgstr "TAF modifié"
 
 #:
 msgid "Flag.AUTO"
 msgstr "METAR automatisé"
 
@@ -391,18 +331,14 @@
 msgstr "granules de glace"
 
 #:
 msgid "Phenomenon.PO"
 msgstr "tourbillon de poussières sable"
 
 #:
-msgid "Phenomenon.PY"
-msgstr "spray"
-
-#:
 msgid "Phenomenon.RA"
 msgstr "pluie"
 
 #:
 msgid "Phenomenon.SA"
 msgstr "sable"
 
@@ -532,15 +468,15 @@
 
 #:
 msgid "Remark.Hourly.Temperature.Dew.Point"
 msgstr "température horaire de {0}°C et point de rosée de {1}°C"
 
 #:
 msgid "Remark.Ice.Accretion.Amount"
-msgstr "{0}/100 d'un pouce d'accrétion de glace au cours des {1} dernières heures"
+msgstr "{0}/100 d''un pouce d''accrétion de glace au cours des {1} dernières heures"
 
 #:
 msgid "Remark.HVY"
 msgstr "fort"
 
 #:
 msgid "Remark.LGT"
@@ -568,15 +504,15 @@
 
 #:
 msgid "Remark.PeakWind"
 msgstr "vent de pointe de {1} noeuds en provenance de {0} degrés à {2}:{3}"
 
 #:
 msgid "Remark.Precipitation.Amount.Hourly"
-msgstr "{0}/100 d'un pouce de précipitation est tombé au cours de la dernière heure"
+msgstr "{0}/100 d''un pouce de précipitation est tombé au cours de la dernière heure"
 
 #:
 msgid "Remark.Precipitation.Amount.3.6"
 msgstr "{1} pouces de précipitations tombées au cours des {0} dernières heures"
 
 #:
 msgid "Remark.Precipitation.Amount.24"
@@ -632,15 +568,15 @@
 
 #:
 msgid "Remark.Snow.Pellets"
 msgstr "{0} grésil"
 
 #:
 msgid "Remark.Sunshine.Duration"
-msgstr "{0} minutes d'ensoleillement"
+msgstr "{0} minutes d''ensoleillement"
 
 #:
 msgid "Remark.Surface.Visibility"
 msgstr "visibility de surface de {0} miles"
 
 #:
 msgid "Remark.Thunderstorm.Location"
@@ -679,36 +615,32 @@
 msgstr "couche de nuages variant entre {0} et {1}"
 
 #:
 msgid "Remark.Variable.Sky.Condition.Height"
 msgstr "couche de nuages à {0} pieds variant entre {1} et {2}"
 
 #:
-msgid "Remark.VIRGA"
-msgstr "virga"
-
-#:
 msgid "Remark.Virga.Direction"
 msgstr "virga au {0} de la station"
 
 #:
 msgid "Remark.WATERSPOUT"
 msgstr "trombe"
 
 #:
 msgid "Remark.Water.Equivalent.Snow.Ground"
-msgstr "équivalent d'eau de {0} pouces de neige"
+msgstr "équivalent d''eau de {0} pouces de neige"
 
 #:
 msgid "Remark.WindShift"
 msgstr "changement de vent à {0}:{1}"
 
 #:
 msgid "Remark.WindShift.FROPA"
-msgstr "changement de vent accompagné d'un passage de front à {0}:{1}"
+msgstr "changement de vent accompagné d''un passage de front à {0}:{1}"
 
 #:
 msgid "MetarFacade.InvalidIcao"
 msgstr "Code ICAO invalide."
 
 #:
 msgid "Converter.D"
@@ -771,18 +703,14 @@
 msgstr "Sud Ouest"
 
 #:
 msgid "Converter.U"
 msgstr "accroissement"
 
 #:
-msgid "Converter.VRB"
-msgstr "Variable"
-
-#:
 msgid "Converter.W"
 msgstr "Ouest"
 
 #:
 msgid "Converter.WNW"
 msgstr "Ouest Nord Ouest"
 
@@ -831,26 +759,18 @@
 msgstr "altimètre (hPa)"
 
 #:
 msgid "ToString.amendment"
 msgstr "amendement"
 
 #:
-msgid "ToString.auto"
-msgstr "auto"
-
-#:
 msgid "ToString.baseHeight"
 msgstr "Base de la couche en pied"
 
 #:
-msgid "ToString.cavok"
-msgstr "cavok"
-
-#:
 msgid "ToString.clouds"
 msgstr "nuages"
 
 #:
 msgid "ToString.day.month"
 msgstr "jour du mois"
 
@@ -919,18 +839,14 @@
 msgstr "message original"
 
 #:
 msgid "ToString.name"
 msgstr "nom"
 
 #:
-msgid "ToString.nosig"
-msgstr "nosig"
-
-#:
 msgid "ToString.phenomenons"
 msgstr "phénomènes"
 
 #:
 msgid "ToString.probability"
 msgstr "probabilité"
 
@@ -979,18 +895,14 @@
 msgstr "tendance"
 
 #:
 msgid "ToString.trends"
 msgstr "tendances"
 
 #:
-msgid "ToString.type"
-msgstr "type"
-
-#:
 msgid "ToString.visibility.main"
 msgstr "visibilité principale"
 
 #:
 msgid "ToString.visibility.min"
 msgstr "visibilité minimale"
 
@@ -1007,18 +919,14 @@
 msgstr "visibilité verticale (pieds)"
 
 #:
 msgid "ToString.weather.conditions"
 msgstr "conditions météorologique"
 
 #:
-msgid "ToString.wind.direction"
-msgstr "direction"
-
-#:
 msgid "ToString.wind.direction.degrees"
 msgstr "direction (degrés)"
 
 #:
 msgid "ToString.wind.gusts"
 msgstr "rafales"
```

### Comparing `metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/it/LC_MESSAGES/messages.mo` & `metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/zh-CN/LC_MESSAGES/messages.mo`

 * *Files 20% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,639 +1,692 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "PO-Revision-Date: \n"
 "Last-Translator: \n"
 "Language-Team: \n"
-"Language: it\n"
+"Language: zh_CN\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"X-Generator: Poedit 3.2.2\n"
+"X-Generator: Poedit 3.4.2\n"
 
 msgid "CloudQuantity.BKN"
-msgstr "molto nuvoloso"
+msgstr "5-7分云"
 
 msgid "CloudQuantity.FEW"
-msgstr "leggermente nuvoloso"
+msgstr "少云"
 
 msgid "CloudQuantity.NSC"
-msgstr "Nessuna nuvola significativa"
+msgstr "没有明显的云。"
 
 msgid "CloudQuantity.OVC"
-msgstr "coperto"
+msgstr "满天云"
 
 msgid "CloudQuantity.SCT"
-msgstr "sparse"
+msgstr "3-4分云"
 
 msgid "CloudQuantity.SKC"
-msgstr "cielo sereno"
+msgstr "天空晴朗"
 
 msgid "CloudType.AC"
-msgstr "Altocumulo"
+msgstr "高积云"
 
 msgid "CloudType.AS"
-msgstr "Altostrato"
+msgstr "高层云"
 
 msgid "CloudType.CB"
-msgstr "Cumulonembo"
+msgstr "积雨云"
 
 msgid "CloudType.CC"
-msgstr "Cirrocumulo"
+msgstr "卷积云"
 
 msgid "CloudType.CI"
-msgstr "Cirro"
+msgstr "Cirrus"
 
 msgid "CloudType.CS"
-msgstr "Cirrostrato"
+msgstr "卷层云"
 
 msgid "CloudType.CU"
-msgstr "Cumulo"
+msgstr "积云"
 
 msgid "CloudType.NS"
-msgstr "Nembostrato"
+msgstr "雨层云"
 
 msgid "CloudType.SC"
-msgstr "Stratocumulo"
+msgstr "层积云"
 
 msgid "CloudType.ST"
-msgstr "Strato"
+msgstr "层云"
 
 msgid "CloudType.TCU"
-msgstr "Cumuli torreggiantidecreasing"
+msgstr "高耸积云"
 
 msgid "Converter.D"
-msgstr "Diminuzione"
+msgstr "减少"
 
 msgid "Converter.E"
-msgstr "Est"
+msgstr "东"
 
 msgid "Converter.ENE"
-msgstr "Est Nord Est"
+msgstr "东东北"
 
 msgid "Converter.ESE"
-msgstr "Est Sud Est"
+msgstr "东东南"
 
 msgid "Converter.N"
-msgstr "Nord"
+msgstr "北"
 
 msgid "Converter.NE"
-msgstr "Nord Est"
+msgstr "东北"
 
 msgid "Converter.NNE"
-msgstr "Nord Nord Est"
+msgstr "北东北"
 
 msgid "Converter.NNW"
-msgstr "Nord Nord Ovest"
+msgstr "北西北"
 
 msgid "Converter.NSC"
-msgstr "nessun cambiamento significativo"
+msgstr "无明显变化"
 
 msgid "Converter.NW"
-msgstr "Nord Ovest"
+msgstr "西北"
 
 msgid "Converter.S"
-msgstr "Sud"
+msgstr "南"
 
 msgid "Converter.SE"
-msgstr "Sud Est"
+msgstr "东南"
 
 msgid "Converter.SSE"
-msgstr "Sud Sud Est"
+msgstr "南东南"
 
 msgid "Converter.SSW"
-msgstr "Sud Sud Ovest"
+msgstr "南西南"
 
 msgid "Converter.SW"
-msgstr "Sud Ovest"
+msgstr "西南"
 
 msgid "Converter.U"
-msgstr "sempre più"
+msgstr "上升"
 
 msgid "Converter.VRB"
-msgstr "Variabile"
+msgstr "多变的"
 
 msgid "Converter.W"
-msgstr "Ovest"
+msgstr "西"
 
 msgid "Converter.WNW"
-msgstr "Ovest Nord Ovest"
+msgstr "西西北"
 
 msgid "Converter.WSW"
-msgstr "Ovest Sud Ovest"
+msgstr "西西南"
 
 msgid "DepositBrakingCapacity.//"
-msgstr "non riportato "
+msgstr "未报告"
 
 msgid "DepositBrakingCapacity.91"
-msgstr "scarso"
+msgstr "差"
 
 msgid "DepositBrakingCapacity.92"
-msgstr "medio/scarso"
+msgstr "中差"
 
 msgid "DepositBrakingCapacity.93"
-msgstr "medio"
+msgstr "中"
 
 msgid "DepositBrakingCapacity.94"
-msgstr "medio/buono"
+msgstr "良好"
 
 msgid "DepositBrakingCapacity.95"
-msgstr "buono"
+msgstr "好"
 
 msgid "DepositBrakingCapacity.99"
-msgstr "cifre inaffidabili"
+msgstr "数字不可靠"
+
+msgid "DepositBrakingCapacity.default"
+msgstr "摩擦系数为 {0}"
 
 msgid "DepositCoverage.FROM_11_TO_25"
-msgstr "dal 11% al 25%"
+msgstr "从11%到25%"
 
 msgid "DepositCoverage.FROM_26_TO_50"
-msgstr "dal 26% al 50%"
+msgstr "从26%到50%"
 
 msgid "DepositCoverage.FROM_51_TO_100"
-msgstr "dal 51% al 100%"
+msgstr "从51%到100%"
 
 msgid "DepositCoverage.LESS_10"
-msgstr "meno del 10%"
+msgstr "低于10%"
 
 msgid "DepositCoverage.NOT_REPORTED"
-msgstr "non riportato"
+msgstr "未报告"
 
 msgid "DepositThickness.//"
-msgstr "non riportato"
+msgstr "未报告"
 
 msgid "DepositThickness.00"
-msgstr "meno di 1 mm"
+msgstr "小于 1 毫米"
 
-msgid "DepositThickness.98"
-msgstr "40 cm"
+msgid "DepositThickness.92"
+msgstr "10 厘米"
 
-msgid "DepositThickness.99"
-msgstr "chiusa"
+msgid "DepositThickness.93"
+msgstr "15 厘米"
+
+msgid "DepositThickness.94"
+msgstr "20 厘米"
 
-msgid "DepositThickness.THICKNESS_10"
-msgstr "10 cm"
+msgid "DepositThickness.95"
+msgstr "25 厘米"
 
-msgid "DepositThickness.THICKNESS_15"
-msgstr "15 cm"
+msgid "DepositThickness.96"
+msgstr "30 厘米"
 
-msgid "DepositThickness.THICKNESS_20"
-msgstr "20 cm"
+msgid "DepositThickness.97"
+msgstr "35 厘米"
 
-msgid "DepositThickness.THICKNESS_25"
-msgstr "25 cm"
+msgid "DepositThickness.98"
+msgstr "40厘米或以上"
 
-msgid "DepositThickness.THICKNESS_30"
-msgstr "30 cm"
+msgid "DepositThickness.99"
+msgstr "已关闭"
 
-msgid "DepositThickness.THICKNESS_35"
-msgstr "35 cm"
+msgid "DepositThickness.default"
+msgstr "{0} 毫米"
 
 msgid "DepositType.CLEAR_DRY"
-msgstr "pulita e asciutta"
+msgstr "干净"
 
 msgid "DepositType.COMPACTED_SNOW"
-msgstr "neve compatta"
+msgstr "压实或滚压的雪"
 
 msgid "DepositType.DAMP"
-msgstr "umido"
+msgstr "潮湿"
 
 msgid "DepositType.DRY_SNOW"
-msgstr "neve asciutta"
+msgstr "干雪"
 
 msgid "DepositType.FROZEN_RIDGES"
-msgstr "solchi o creste congelate"
+msgstr "冷冻的轮辙或冰脊"
 
 msgid "DepositType.ICE"
-msgstr "ghiaccio"
+msgstr "冰"
 
 msgid "DepositType.NOT_REPORTED"
-msgstr "non riportato"
+msgstr "未报告"
 
 msgid "DepositType.RIME_FROST_COVERED"
-msgstr "ricoperta di brina"
+msgstr "雾凇和霜覆盖"
+
+msgid "DepositType.SLUSH"
+msgstr "雪浆"
 
 msgid "DepositType.WET_SNOW"
-msgstr "neve bagnata"
+msgstr "湿雪"
 
 msgid "DepositType.WET_WATER_PATCHES"
-msgstr "pozzanghere bagnate"
+msgstr "湿和水纹"
 
 msgid "Descriptive.BC"
-msgstr "banchi di nebbia"
+msgstr "补丁"
 
 msgid "Descriptive.BL"
-msgstr "sollevamento alto"
+msgstr "吹"
 
 msgid "Descriptive.DR"
-msgstr "sollevamento basso"
+msgstr "低漂"
 
 msgid "Descriptive.FZ"
-msgstr "congelantesi"
+msgstr "冰冻"
 
 msgid "Descriptive.MI"
-msgstr "strati di nebbia"
+msgstr "浅"
 
 msgid "Descriptive.PR"
-msgstr "parziale"
+msgstr "部分的"
 
 msgid "Descriptive.SH"
-msgstr "rovescio"
+msgstr "阵雨"
 
 msgid "Descriptive.TS"
-msgstr "temporale"
+msgstr "雷雨"
 
 msgid "Error.prefix"
-msgstr "Si è verificato un errore. Errore nr. "
+msgstr "发生错误。 错误代码 n°"
 
 msgid "ErrorCode.AirportNotFound"
-msgstr "L’aeroporto non è stato trovato in questa notifica"
+msgstr "找不到此消息的机场。"
 
 msgid "ErrorCode.InvalidMessage"
-msgstr "Il messaggio non è valido"
+msgstr "输入的消息无效。"
+
+msgid "Flag.AMD"
+msgstr "修正后的TAF"
+
+msgid "Flag.AUTO"
+msgstr "自动生成的METAR"
+
+msgid "Flag.CNL"
+msgstr "已取消的TAF"
+
+msgid "Flag.COR"
+msgstr "已更正的METAR/TAF"
+
+msgid "Flag.NIL"
+msgstr "暂无数据"
+
+msgid "IcingIntensity.0"
+msgstr "微量结冰"
+
+msgid "IcingIntensity.1"
+msgstr "轻度混合结冰"
+
+msgid "IcingIntensity.2"
+msgstr "云中轻度霜冻结冰"
+
+msgid "IcingIntensity.7"
+msgstr "重度混合结冰"
 
 msgid "Indicator.M"
-msgstr "minore di"
+msgstr "小于"
 
 msgid "Indicator.P"
-msgstr "maggiore di"
+msgstr "大于"
 
 msgid "Intensity.+"
-msgstr "Forte"
+msgstr "强的"
 
 msgid "Intensity.-"
-msgstr "Debole"
+msgstr "弱的"
 
 msgid "Intensity.VC"
-msgstr "Nelle vicinanze"
+msgstr "在附近"
 
 msgid "MetarFacade.InvalidIcao"
-msgstr "Codice ICAO non valido"
+msgstr "ICAO 代码无效。"
 
 msgid "Phenomenon.BR"
-msgstr "foschia"
+msgstr "薄雾"
 
 msgid "Phenomenon.DS"
-msgstr "tempesta di polvere "
+msgstr "沙尘暴"
 
 msgid "Phenomenon.DU"
-msgstr "polvere su un’area estesa"
+msgstr "弥漫的灰尘"
 
 msgid "Phenomenon.DZ"
-msgstr "pioviggine"
+msgstr "细雨"
 
 msgid "Phenomenon.FC"
-msgstr "tornado o tromba marina"
+msgstr "漏斗云"
 
 msgid "Phenomenon.FG"
-msgstr "nebbia"
+msgstr "雾"
 
 msgid "Phenomenon.FU"
-msgstr "fumo"
+msgstr "烟"
 
 msgid "Phenomenon.GR"
-msgstr "grandine"
+msgstr "冰雹"
 
 msgid "Phenomenon.GS"
-msgstr "grandine piccola e/o granuli di neve"
+msgstr "小冰雹和/或雪粒"
 
 msgid "Phenomenon.HZ"
-msgstr "caligine"
+msgstr "雾霾"
 
 msgid "Phenomenon.IC"
-msgstr "cristalli di ghiaccio"
+msgstr "冰晶"
 
 msgid "Phenomenon.PL"
-msgstr "granuli di ghiaccio"
+msgstr "冰粒"
 
 msgid "Phenomenon.PO"
-msgstr "mulinelli di polvere/sabbia"
+msgstr "尘土或沙尘旋风"
 
 msgid "Phenomenon.PY"
-msgstr "schizzi"
+msgstr "喷"
 
 msgid "Phenomenon.RA"
-msgstr "pioggia"
+msgstr "雨"
 
 msgid "Phenomenon.SA"
-msgstr "sabbia"
+msgstr "沙"
 
 msgid "Phenomenon.SG"
-msgstr "neve granulosa"
+msgstr "雪粒"
 
 msgid "Phenomenon.SN"
-msgstr "neve"
+msgstr "雪"
 
 msgid "Phenomenon.SQ"
-msgstr "groppo"
+msgstr "狂风"
 
 msgid "Phenomenon.SS"
-msgstr "tempesta di sabbia"
+msgstr "沙暴"
 
 msgid "Phenomenon.TS"
-msgstr "temporale"
+msgstr "雷雨"
 
 msgid "Phenomenon.UP"
-msgstr "precipitazione sconosciuta"
+msgstr "未知降水"
 
 msgid "Phenomenon.VA"
-msgstr "cenere vulcanica"
+msgstr "火山灰"
+
+msgid "Remark.ALQDS"
+msgstr "全象限"
 
 msgid "Remark.AO1"
-msgstr "stazioni automatizzate senza discriminatore di precipitazione"
+msgstr "没有降水鉴别器的自动化站"
 
 msgid "Remark.AO2"
-msgstr "stazione automatizzata con discriminatore di precipitazione"
+msgstr "带有降水鉴别器的自动化站"
 
 msgid "Remark.BASED"
-msgstr "basato"
+msgstr "基于"
+
+msgid "Remark.Barometer.0"
+msgstr "先增加后减少"
+
+msgid "Remark.Barometer.1"
+msgstr "先增加后稳定, 或是先增加后缓慢增加"
+
+msgid "Remark.Barometer.2"
+msgstr "稳定或不稳定的增加"
+
+msgid "Remark.Barometer.3"
+msgstr "先减少或保持稳定，然后增加；或先增加然后快速增加"
+
+msgid "Remark.Barometer.4"
+msgstr "稳定"
+
+msgid "Remark.Barometer.5"
+msgstr "减小，然后增加"
+
+msgid "Remark.Barometer.6"
+msgstr "先减少后稳定；或先减少后更缓慢减少"
+
+msgid "Remark.Barometer.7"
+msgstr "稳定或不稳定地减少"
+
+msgid "Remark.Barometer.8"
+msgstr "先稳定或增加，然后减少；或先减少快速减少"
 
 msgid "Remark.Ceiling.Height"
-msgstr "base delle nubi tra {0} e {1} piedi"
+msgstr "上限在 {0} 到 {1} 英尺之间变化"
 
 msgid "Remark.Ceiling.Second.Location"
-msgstr ""
-"base delle nubi di {0} piedi misurato da un secondo sensore situato a {1}"
+msgstr "由位于 {1} 处的第二个传感器测量的 {0} 英尺的上限"
+
+msgid "Remark.DSNT"
+msgstr "距离"
 
 msgid "Remark.FCST"
-msgstr "previsione"
+msgstr "预报"
 
 msgid "Remark.FUNNELCLOUD"
-msgstr "nuvole a imbuto"
+msgstr "漏斗云"
 
 msgid "Remark.HVY"
-msgstr "pesante"
+msgstr "重度的"
 
 msgid "Remark.Hail"
-msgstr "chicchi di grandine più grandi con un diametro di {0} pollici"
+msgstr "直径为 {0} 英寸的最大的冰雹"
 
 msgid "Remark.Hail.LesserThan"
-msgstr ""
-"chicchi di grandine più grandi con un diametro inferiore di {0} pollici"
+msgstr "直径小于 {0} 英寸的最大的冰雹"
+
+msgid "Remark.Hourly.Maximum.Minimum.Temperature"
+msgstr "24小时最高温度为{0}°C，24小时最低温度为{1}°C"
+
+msgid "Remark.Hourly.Maximum.Temperature"
+msgstr "6小时最高温度为{0}°C"
+
+msgid "Remark.Hourly.Minimum.Temperature"
+msgstr "6 小时最低温度为 {0}° C"
+
+msgid "Remark.Hourly.Temperature"
+msgstr "小时气温 {0}°C"
+
+msgid "Remark.Hourly.Temperature.Dew.Point"
+msgstr "小时气温为{0}°C，露点为{1}°C"
+
+msgid "Remark.Ice.Accretion.Amount"
+msgstr "过去{1} 小时内积冰{0}/100英寸"
 
 msgid "Remark.LGT"
-msgstr "leggero"
+msgstr "轻微的"
+
+msgid "Remark.LTG"
+msgstr "闪电"
 
 msgid "Remark.MOD"
-msgstr "moderato"
+msgstr "中等"
 
 msgid "Remark.NXT"
-msgstr "prossimo"
+msgstr "下一个"
 
 msgid "Remark.ON"
-msgstr "on"
+msgstr "在"
 
 msgid "Remark.Obscuration"
-msgstr "{0} strato a {1} piedi composto da {2}"
+msgstr "{0} 层位于 {1} 英尺，由 {2} 组成"
 
 msgid "Remark.PRESFR"
-msgstr "pressione in caduta rapidamente "
+msgstr "气压骤降"
 
 msgid "Remark.PRESRR"
-msgstr "pressione in salita rapidamente"
+msgstr "气压骤升"
 
 msgid "Remark.PeakWind"
-msgstr "picco di vento di {1} nodi da {0} gradi a {2}:{3}"
-
-msgid "Remark.Precipitation.Beg.End"
-msgstr "{0} {1} inizia a {2}:{3} e termina a {4}:{5}"
-
-msgid "Remark.SLPNO"
-msgstr "pressione a livello del mare non disponibile"
+msgstr "在 {2}:{3} 有位于 {0} 度，风速 {1} 节的峰值风"
 
 msgid "Remark.Sea.Level.Pressure"
-msgstr "pressione a livello del mare di {0} HPa"
-
-msgid "Remark.Second.Location.Visibility"
-msgstr "visibilità di {0} SM misurata da un secondo sensore situato a {1}"
-
-msgid "Remark.Sector.Visibility"
-msgstr "visibilità di {1} SM in direzione {0}"
-
-msgid "Remark.Snow.Increasing.Rapidly"
-msgstr ""
-"aumento dell’altezza della neve di {0} pollici nell’ultima ora con "
-"un’altezza totale al suolo di {1} pollici"
-
-msgid "Remark.Snow.Pellets"
-msgstr "{0} neve tonda "
-
-msgid "Remark.Surface.Visibility"
-msgstr "visibilità in superficie di {0} Statute Miles"
+msgstr "海平面气压{0} 百帕"
 
 msgid "Remark.TORNADO"
-msgstr "tornado"
-
-msgid "Remark.Thunderstorm.Location"
-msgstr "temporale {0} dalla stazione"
-
-msgid "Remark.Thunderstorm.Location.Moving"
-msgstr "temporale {0} dalla stazione si muove in direzione di {1}"
-
-msgid "Remark.Tornadic.Activity.BegEnd"
-msgstr "{0} inizia a {1}:{2} e termina a {3}:{4} {5} SM {6} dalla stazione"
-
-msgid "Remark.Tornadic.Activity.Beginning"
-msgstr "{0} inizia a {1}:{2} {3} SM {4} dalla stazione"
-
-msgid "Remark.Tornadic.Activity.Ending"
-msgstr "{0} termina a {1}:{2} {3} SM {4} dalla stazione"
-
-msgid "Remark.Tower.Visibility"
-msgstr "visibilità dalla torre di controllo di {0} Statute Miles"
+msgstr "龙卷风"
 
 msgid "Remark.VIRGA"
-msgstr "virga"
-
-msgid "Remark.Variable.Prevailing.Visibility"
-msgstr "visibilità prevalentemente variabile tra {0} e {1} SM"
-
-msgid "Remark.Variable.Sky.Condition"
-msgstr "strato di nuvole che varia tra {0} e {1}"
-
-msgid "Remark.Variable.Sky.Condition.Height"
-msgstr "strato di nubi a {0} piedi che varia tra {1} e {2}"
-
-msgid "Remark.Virga.Direction"
-msgstr "virga {0} dalla stazione"
+msgstr "幡状云"
 
 msgid "Remark.WATERSPOUT"
-msgstr "tromba marina"
+msgstr "水龙卷"
 
-msgid "Remark.WindShift"
-msgstr "spostamento del vento a {0}:{1}"
+msgid "Remark.Water.Equivalent.Snow.Ground"
+msgstr "相当于{0} 英寸雪的降水"
 
-msgid "Remark.WindShift.FROPA"
-msgstr "spostamento del vento accompagnato da passaggio frontale a {0}:{1}"
+msgid "Remark.WindShift"
+msgstr "风力转变于 {0}:{1}"
 
 msgid "TimeIndicator.AT"
-msgstr "alle"
+msgstr "在"
 
 msgid "TimeIndicator.FM"
-msgstr "dalle"
+msgstr "从"
 
 msgid "TimeIndicator.TL"
-msgstr "fino alle"
+msgstr "直到"
 
 msgid "ToString.airport"
-msgstr "aeroporto"
+msgstr "机场"
 
 msgid "ToString.altimeter"
-msgstr "altimetro (hPa)"
+msgstr "修正海压（百帕）"
 
 msgid "ToString.amendment"
-msgstr "emendamento"
+msgstr "修订"
 
 msgid "ToString.auto"
-msgstr "auto"
+msgstr "自动观测"
 
 msgid "ToString.cavok"
-msgstr "cavok"
+msgstr "能见度≥10km"
 
 msgid "ToString.clouds"
-msgstr "nuvole"
+msgstr "云"
 
 msgid "ToString.day.hour"
-msgstr "ora del giorno"
+msgstr "当日某小时"
 
 msgid "ToString.day.month"
-msgstr "giorno del mese"
+msgstr "当月某天"
 
 msgid "ToString.deposit.braking"
-msgstr "capacità frenante"
+msgstr "制动能力"
 
 msgid "ToString.deposit.coverage"
-msgstr "copertura"
+msgstr "覆盖范围"
 
 msgid "ToString.deposit.thickness"
-msgstr "spessore"
+msgstr "厚度"
 
 msgid "ToString.deposit.type"
-msgstr "tipo di deposito"
+msgstr "沉积物类型"
 
 msgid "ToString.descriptive"
-msgstr "descrittivo"
+msgstr "描述"
 
 msgid "ToString.dew.point"
-msgstr "punto di rugiada"
+msgstr "露点"
 
 msgid "ToString.end.day.month"
-msgstr "ultimo giorno del mese"
+msgstr "当月的结束日"
 
 msgid "ToString.end.hour.day"
-msgstr "ultima ora del giorno"
+msgstr "当日的结束小时"
+
+msgid "ToString.flags"
+msgstr "旗子"
 
 msgid "ToString.height.feet"
-msgstr "altezza (ft)"
+msgstr "高度（英尺）"
 
 msgid "ToString.height.meter"
-msgstr "altezza (m)"
+msgstr "高度（米）"
 
 msgid "ToString.indicator"
-msgstr "indicatore"
+msgstr "指示器"
 
 msgid "ToString.intensity"
-msgstr "intensità"
+msgstr "强度"
 
 msgid "ToString.message"
-msgstr "messaggio originale"
+msgstr "原始消息"
 
 msgid "ToString.name"
-msgstr "nome"
+msgstr "名称"
 
 msgid "ToString.nosig"
-msgstr "nosig"
+msgstr "无重大变化"
 
 msgid "ToString.phenomenons"
-msgstr "fenomeni"
+msgstr "现象"
 
 msgid "ToString.probability"
-msgstr "probabilità"
+msgstr "可能性"
 
 msgid "ToString.quantity"
-msgstr "quantità"
+msgstr "数量"
 
 msgid "ToString.remark"
-msgstr "remark"
+msgstr "备注"
 
 msgid "ToString.report.time"
-msgstr "ora del rapporto"
+msgstr "报告时间"
 
 msgid "ToString.runway.info"
-msgstr "informazioni sulle piste"
+msgstr "跑道信息"
 
 msgid "ToString.start.day.month"
-msgstr "primo giorno del mese"
+msgstr "当月起始日"
 
 msgid "ToString.start.hour.day"
-msgstr "prima ora del giorno"
+msgstr "当日起始小时"
 
 msgid "ToString.start.minute"
-msgstr "minuto di inizio"
+msgstr "起始分钟"
 
 msgid "ToString.temperature"
-msgstr "temperatura (°C)"
+msgstr "温度（°C）"
 
 msgid "ToString.temperature.max"
-msgstr "temperatura massima (°C)"
+msgstr "最高温度（°C）"
 
 msgid "ToString.temperature.min"
-msgstr "temperatura minima (°C)"
+msgstr "最低温度（°C）"
 
 msgid "ToString.trend"
-msgstr "tendenza"
+msgstr "趋势预报"
 
 msgid "ToString.trends"
-msgstr "tendenze"
+msgstr "趋势"
 
 msgid "ToString.type"
-msgstr "tipo"
+msgstr "类型"
 
 msgid "ToString.vertical.visibility"
-msgstr "visibilità verticale (ft)"
+msgstr "垂直能见度（英尺）"
 
 msgid "ToString.visibility.main"
-msgstr "visibilità principale"
+msgstr "主要能见度"
 
 msgid "ToString.visibility.max"
-msgstr "visibilità massima"
+msgstr "最大能见度"
 
 msgid "ToString.visibility.min"
-msgstr "visibilità minima"
+msgstr "最小能见度"
 
 msgid "ToString.visibility.min.direction"
-msgstr "direzione visibilità minima"
+msgstr "最小能见方向"
 
 msgid "ToString.weather.conditions"
-msgstr "condizioni meteo"
+msgstr "天气状况"
 
 msgid "ToString.wind.direction"
-msgstr "direzione"
+msgstr "方向"
 
 msgid "ToString.wind.direction.degrees"
-msgstr "direzione (gradi)"
+msgstr "方向(度)"
 
 msgid "ToString.wind.gusts"
-msgstr "raffiche"
+msgstr "阵风"
 
 msgid "ToString.wind.max.variation"
-msgstr "variazione massima del vento"
+msgstr "最大风力变化量"
 
 msgid "ToString.wind.min.variation"
-msgstr "variazione minima del vento"
+msgstr "最小风力变化量"
 
 msgid "ToString.wind.speed"
-msgstr "velocità"
+msgstr "速度"
 
 msgid "ToString.wind.unit"
-msgstr "unità"
+msgstr "单位"
+
+msgid "TurbulenceIntensity.0"
+msgstr "无"
+
+msgid "TurbulenceIntensity.1"
+msgstr "轻度乱流"
+
+msgid "TurbulenceIntensity.8"
+msgstr "云中偶发重度颠簸"
+
+msgid "TurbulenceIntensity.X"
+msgstr "极端乱流"
 
 msgid "WeatherChangeType.BECMG"
-msgstr "Diventa"
+msgstr "变得"
 
 msgid "WeatherChangeType.FM"
-msgstr "Da"
+msgstr "从"
+
+msgid "WeatherChangeType.INTER"
+msgstr "间歇的"
 
 msgid "WeatherChangeType.PROB"
-msgstr "Probabilità"
+msgstr "可能性"
 
 msgid "WeatherChangeType.TEMPO"
-msgstr "Temporanea"
+msgstr "暂时的"
```

### Comparing `metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/it/LC_MESSAGES/messages.po` & `metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/messages.pot`

 * *Files 17% similar despite different names*

```diff
@@ -1,840 +1,1088 @@
 msgid ""
 msgstr ""
 "MIME-Version: 1.0"
 "Content-Type: text/plain; charset=UTF-8"
 "Content-Transfer-Encoding: 8bit"
 "X-Generator: prop2po"
 "Project-Id-Version: metar_taf_parser"
-"Language: it"
+"Language: en"
 #:
 msgid "CloudQuantity.BKN"
-msgstr "molto nuvoloso"
+msgstr "broken"
 
 #:
 msgid "CloudQuantity.FEW"
-msgstr "leggermente nuvoloso"
+msgstr "few"
 
 #:
 msgid "CloudQuantity.NSC"
-msgstr "Nessuna nuvola significativa"
+msgstr "no significant clouds."
 
 #:
 msgid "CloudQuantity.OVC"
-msgstr "coperto"
+msgstr "overcast"
 
 #:
 msgid "CloudQuantity.SCT"
-msgstr "sparse"
+msgstr "scattered"
 
 #:
 msgid "CloudQuantity.SKC"
-msgstr "cielo sereno"
+msgstr "sky clear"
 
 #:
 msgid "CloudType.AC"
-msgstr "Altocumulo"
+msgstr "Altocumulus"
 
 #:
 msgid "CloudType.AS"
-msgstr "Altostrato"
+msgstr "Altostratus"
 
 #:
 msgid "CloudType.CB"
-msgstr "Cumulonembo"
+msgstr "Cumulonimbus"
 
 #:
 msgid "CloudType.CC"
-msgstr "Cirrocumulo"
+msgstr "CirroCumulus"
 
 #:
 msgid "CloudType.CI"
-msgstr "Cirro"
+msgstr "Cirrus"
 
 #:
 msgid "CloudType.CS"
-msgstr "Cirrostrato"
+msgstr "Cirrostratus"
 
 #:
 msgid "CloudType.CU"
-msgstr "Cumulo"
+msgstr "Cumulus"
 
 #:
 msgid "CloudType.NS"
-msgstr "Nembostrato"
+msgstr "Nimbostratus"
 
 #:
 msgid "CloudType.SC"
-msgstr "Stratocumulo"
+msgstr "Stratocumulus"
 
 #:
 msgid "CloudType.ST"
-msgstr "Strato"
+msgstr "Stratus"
 
 #:
 msgid "CloudType.TCU"
-msgstr "Cumuli torreggiantidecreasing"
+msgstr "Towering cumulus"
 
 #:
 msgid "DepositBrakingCapacity.//"
-msgstr "non riportato "
+msgstr "not reported"
 
 #:
 msgid "DepositBrakingCapacity.91"
-msgstr "scarso"
+msgstr "poor"
 
 #:
 msgid "DepositBrakingCapacity.92"
-msgstr "medio/scarso"
+msgstr "poor/medium"
 
 #:
 msgid "DepositBrakingCapacity.93"
-msgstr "medio"
+msgstr "medium"
 
 #:
 msgid "DepositBrakingCapacity.94"
-msgstr "medio/buono"
+msgstr "medium/good"
 
 #:
 msgid "DepositBrakingCapacity.95"
-msgstr "buono"
+msgstr "good"
 
 #:
 msgid "DepositBrakingCapacity.99"
-msgstr "cifre inaffidabili"
+msgstr "figures unreliable"
+
+#:
+msgid "DepositBrakingCapacity.default"
+msgstr "friction coefficient of {0}"
 
 #:
 msgid "DepositCoverage.NOT_REPORTED"
-msgstr "non riportato"
+msgstr "not reported"
 
 #:
 msgid "DepositCoverage.LESS_10"
-msgstr "meno del 10%"
+msgstr "less than 10%"
 
 #:
 msgid "DepositCoverage.FROM_11_TO_25"
-msgstr "dal 11% al 25%"
+msgstr "from 11% to 25%"
 
 #:
 msgid "DepositCoverage.FROM_26_TO_50"
-msgstr "dal 26% al 50%"
+msgstr "from 26% to 50%"
 
 #:
 msgid "DepositCoverage.FROM_51_TO_100"
-msgstr "dal 51% al 100%"
+msgstr "from 51% to 100%"
 
 #:
 msgid "DepositThickness.//"
-msgstr "non riportato"
+msgstr "not reported"
 
 #:
 msgid "DepositThickness.00"
-msgstr "meno di 1 mm"
+msgstr "less than 1 mm"
 
 #:
-msgid "DepositThickness.THICKNESS_10"
+msgid "DepositThickness.92"
 msgstr "10 cm"
 
 #:
-msgid "DepositThickness.THICKNESS_15"
+msgid "DepositThickness.93"
 msgstr "15 cm"
 
 #:
-msgid "DepositThickness.THICKNESS_20"
+msgid "DepositThickness.94"
 msgstr "20 cm"
 
 #:
-msgid "DepositThickness.THICKNESS_25"
+msgid "DepositThickness.95"
 msgstr "25 cm"
 
 #:
-msgid "DepositThickness.THICKNESS_30"
+msgid "DepositThickness.96"
 msgstr "30 cm"
 
 #:
-msgid "DepositThickness.THICKNESS_35"
+msgid "DepositThickness.97"
 msgstr "35 cm"
 
 #:
 msgid "DepositThickness.98"
-msgstr "40 cm"
+msgstr "40 cm or more"
 
 #:
 msgid "DepositThickness.99"
-msgstr "chiusa"
+msgstr "closed"
+
+#:
+msgid "DepositThickness.default"
+msgstr "{0} mm"
 
 #:
 msgid "DepositType.NOT_REPORTED"
-msgstr "non riportato"
+msgstr "not reported"
 
 #:
 msgid "DepositType.CLEAR_DRY"
-msgstr "pulita e asciutta"
+msgstr "clear and dry"
 
 #:
 msgid "DepositType.DAMP"
-msgstr "umido"
+msgstr "damp"
 
 #:
 msgid "DepositType.WET_WATER_PATCHES"
-msgstr "pozzanghere bagnate"
+msgstr "wet or water patches"
 
 #:
 msgid "DepositType.RIME_FROST_COVERED"
-msgstr "ricoperta di brina"
+msgstr "rime or frost covered"
 
 #:
 msgid "DepositType.DRY_SNOW"
-msgstr "neve asciutta"
+msgstr "dry snow"
 
 #:
 msgid "DepositType.WET_SNOW"
-msgstr "neve bagnata"
+msgstr "wet snow"
 
 #:
 msgid "DepositType.ICE"
-msgstr "ghiaccio"
+msgstr "ice"
 
 #:
 msgid "DepositType.COMPACTED_SNOW"
-msgstr "neve compatta"
+msgstr "compacted or rolled snow"
 
 #:
 msgid "DepositType.FROZEN_RIDGES"
-msgstr "solchi o creste congelate"
+msgstr "frozen ruts or ridges"
+
+#:
+msgid "DepositType.SLUSH"
+msgstr "slush"
 
 #:
 msgid "Descriptive.BC"
-msgstr "banchi di nebbia"
+msgstr "patches"
 
 #:
 msgid "Descriptive.BL"
-msgstr "sollevamento alto"
+msgstr "blowing"
 
 #:
 msgid "Descriptive.DR"
-msgstr "sollevamento basso"
+msgstr "low drifting"
 
 #:
 msgid "Descriptive.FZ"
-msgstr "congelantesi"
+msgstr "freezing"
 
 #:
 msgid "Descriptive.MI"
-msgstr "strati di nebbia"
+msgstr "shallow"
 
 #:
 msgid "Descriptive.PR"
-msgstr "parziale"
+msgstr "partial"
 
 #:
 msgid "Descriptive.SH"
-msgstr "rovescio"
+msgstr "showers of"
 
 #:
 msgid "Descriptive.TS"
-msgstr "temporale"
+msgstr "thunderstorm"
 
 #:
 msgid "Error.prefix"
-msgstr "Si è verificato un errore. Errore nr. "
+msgstr "An error occured. Error code n°"
 
 #:
 msgid "ErrorCode.AirportNotFound"
-msgstr "L’aeroporto non è stato trovato in questa notifica"
+msgstr "The airport was not found for this message."
 
 #:
 msgid "ErrorCode.InvalidMessage"
-msgstr "Il messaggio non è valido"
+msgstr "The entered message is invalid."
+
+#:
+msgid "ErrorCode.IncompleteRunwayInformation"
+msgstr "The runway information is incomplete and cannot be parsed."
+
+#:
+msgid "Flag.AMD"
+msgstr "amended TAF"
+
+#:
+msgid "Flag.AUTO"
+msgstr "automated METAR"
+
+#:
+msgid "Flag.CNL"
+msgstr "canceled TAF"
+
+#:
+msgid "Flag.COR"
+msgstr "corrected METAR/TAF"
+
+#:
+msgid "Flag.NIL"
+msgstr "no data"
+
+#:
+msgid "IcingIntensity.0"
+msgstr "Trace Icing or None"
+
+#:
+msgid "IcingIntensity.1"
+msgstr "Light Mixed Icing"
+
+#:
+msgid "IcingIntensity.2"
+msgstr "Light Rime Icing In Cloud"
+
+#:
+msgid "IcingIntensity.3"
+msgstr "Light Clear Icing In Precipitation"
+
+#:
+msgid "IcingIntensity.4"
+msgstr "Moderate Mixed Icing"
+
+#:
+msgid "IcingIntensity.5"
+msgstr "Moderate Rime Icing In Cloud"
+
+#:
+msgid "IcingIntensity.6"
+msgstr "Moderate Clear Icing In Precipitation"
+
+#:
+msgid "IcingIntensity.7"
+msgstr "Severe Mixed Icing"
+
+#:
+msgid "IcingIntensity.8"
+msgstr "Severe Rime Icing In Cloud"
+
+#:
+msgid "IcingIntensity.9"
+msgstr "Severe Clear Icing In Precipitation"
 
 #:
 msgid "Indicator.M"
-msgstr "minore di"
+msgstr "less than"
 
 #:
 msgid "Indicator.P"
-msgstr "maggiore di"
+msgstr "greater than"
 
 #:
 msgid "Intensity.-"
-msgstr "Debole"
+msgstr "Light"
 
 #:
 msgid "Intensity.+"
-msgstr "Forte"
+msgstr "Heavy"
+
+#:
+msgid "Intensity.RE"
+msgstr "Recent"
 
 #:
 msgid "Intensity.VC"
-msgstr "Nelle vicinanze"
+msgstr "In the vicinity"
 
 #:
 msgid "Phenomenon.BR"
-msgstr "foschia"
+msgstr "mist"
 
 #:
 msgid "Phenomenon.DS"
-msgstr "tempesta di polvere "
+msgstr "duststorm"
 
 #:
 msgid "Phenomenon.DU"
-msgstr "polvere su un’area estesa"
+msgstr "widespread dust"
 
 #:
 msgid "Phenomenon.DZ"
-msgstr "pioviggine"
+msgstr "drizzle"
 
 #:
 msgid "Phenomenon.FC"
-msgstr "tornado o tromba marina"
+msgstr "funnel cloud"
 
 #:
 msgid "Phenomenon.FG"
-msgstr "nebbia"
+msgstr "fog"
 
 #:
 msgid "Phenomenon.FU"
-msgstr "fumo"
+msgstr "smoke"
 
 #:
 msgid "Phenomenon.GR"
-msgstr "grandine"
+msgstr "hail"
 
 #:
 msgid "Phenomenon.GS"
-msgstr "grandine piccola e/o granuli di neve"
+msgstr "small hail and/or snow pellets"
 
 #:
 msgid "Phenomenon.HZ"
-msgstr "caligine"
+msgstr "haze"
 
 #:
 msgid "Phenomenon.IC"
-msgstr "cristalli di ghiaccio"
+msgstr "ice crystals"
 
 #:
 msgid "Phenomenon.PL"
-msgstr "granuli di ghiaccio"
+msgstr "ice pellets"
 
 #:
 msgid "Phenomenon.PO"
-msgstr "mulinelli di polvere/sabbia"
+msgstr "dust or sand whirls"
 
 #:
 msgid "Phenomenon.PY"
-msgstr "schizzi"
+msgstr "spray"
 
 #:
 msgid "Phenomenon.RA"
-msgstr "pioggia"
+msgstr "rain"
 
 #:
 msgid "Phenomenon.SA"
-msgstr "sabbia"
+msgstr "sand"
 
 #:
 msgid "Phenomenon.SG"
-msgstr "neve granulosa"
+msgstr "snow grains"
 
 #:
 msgid "Phenomenon.SN"
-msgstr "neve"
+msgstr "snow"
 
 #:
 msgid "Phenomenon.SQ"
-msgstr "groppo"
+msgstr "squall"
 
 #:
 msgid "Phenomenon.SS"
-msgstr "tempesta di sabbia"
+msgstr "sandstorm"
 
 #:
 msgid "Phenomenon.UP"
-msgstr "precipitazione sconosciuta"
+msgstr "unknown precipitation"
 
 #:
 msgid "Phenomenon.VA"
-msgstr "cenere vulcanica"
+msgstr "volcanic ash"
 
 #:
 msgid "Phenomenon.TS"
-msgstr "temporale"
+msgstr "thunderstorm"
 
 #:
 msgid "Remark.AO1"
-msgstr "stazioni automatizzate senza discriminatore di precipitazione"
+msgstr "automated stations without a precipitation discriminator"
 
 #:
 msgid "Remark.AO2"
-msgstr "stazione automatizzata con discriminatore di precipitazione"
+msgstr "automated station with a precipitation discriminator"
+
+#:
+msgid "Remark.ALQDS"
+msgstr "all quadrants"
+
+#:
+msgid "Remark.Barometer.0"
+msgstr "Increase, then decrease"
+
+#:
+msgid "Remark.Barometer.1"
+msgstr "Increase, then steady, or increase then Increase more slowly"
+
+#:
+msgid "Remark.Barometer.2"
+msgstr "steady or unsteady increase"
+
+#:
+msgid "Remark.Barometer.3"
+msgstr "Decrease or steady, then increase; or increase then increase more rapidly"
+
+#:
+msgid "Remark.Barometer.4"
+msgstr "Steady"
+
+#:
+msgid "Remark.Barometer.5"
+msgstr "Decrease, then increase"
+
+#:
+msgid "Remark.Barometer.6"
+msgstr "Decrease then steady; or decrease then decrease more slowly"
+
+#:
+msgid "Remark.Barometer.7"
+msgstr "Steady or unsteady decrease"
+
+#:
+msgid "Remark.Barometer.8"
+msgstr "Steady or increase, then decrease; or decrease then decrease more rapidly"
 
 #:
 msgid "Remark.BASED"
-msgstr "basato"
+msgstr "based"
 
 #:
 msgid "Remark.Ceiling.Height"
-msgstr "base delle nubi tra {0} e {1} piedi"
+msgstr "ceiling varying between {0} and {1} feet"
 
 #:
 msgid "Remark.Ceiling.Second.Location"
-msgstr "base delle nubi di {0} piedi misurato da un secondo sensore situato a {1}"
+msgstr "ceiling of {0} feet mesured by a second sensor located at {1}"
+
+#:
+msgid "Remark.DSNT"
+msgstr "distant"
 
 #:
 msgid "Remark.FCST"
-msgstr "previsione"
+msgstr "forecast"
 
 #:
 msgid "Remark.FUNNELCLOUD"
-msgstr "nuvole a imbuto"
+msgstr "funnel cloud"
 
 #:
 msgid "Remark.Hail"
-msgstr "chicchi di grandine più grandi con un diametro di {0} pollici"
+msgstr "largest hailstones with a diameter of {0} inches"
 
 #:
 msgid "Remark.Hail.LesserThan"
-msgstr "chicchi di grandine più grandi con un diametro inferiore di {0} pollici"
+msgstr "largest hailstones with a diameter less than {0} inches"
+
+#:
+msgid "Remark.Hourly.Maximum.Temperature"
+msgstr "6-hourly maximum temperature of {0}°C"
+
+#:
+msgid "Remark.Hourly.Maximum.Minimum.Temperature"
+msgstr "24-hour maximum temperature of {0}°C and 24-hour minimum temperature of {1}°C"
+
+#:
+msgid "Remark.Hourly.Minimum.Temperature"
+msgstr "6-hourly minimum temperature of {0}°C"
+
+#:
+msgid "Remark.Hourly.Temperature"
+msgstr "hourly temperature of {0}°C"
+
+#:
+msgid "Remark.Hourly.Temperature.Dew.Point"
+msgstr "hourly temperature of {0}°C and dew point of {1}°C"
+
+#:
+msgid "Remark.Ice.Accretion.Amount"
+msgstr "{0}/100 of an inch of ice accretion in the past {1} hour(s)"
 
 #:
 msgid "Remark.HVY"
-msgstr "pesante"
+msgstr "heavy"
 
 #:
 msgid "Remark.LGT"
-msgstr "leggero"
+msgstr "light"
+
+#:
+msgid "Remark.LTG"
+msgstr "lightning"
 
 #:
 msgid "Remark.MOD"
-msgstr "moderato"
+msgstr "moderate"
 
 #:
 msgid "Remark.Obscuration"
-msgstr "{0} strato a {1} piedi composto da {2}"
+msgstr "{0} layer at {1} feet composed of {2}"
 
 #:
 msgid "Remark.ON"
 msgstr "on"
 
 #:
 msgid "Remark.NXT"
-msgstr "prossimo"
+msgstr "next"
 
 #:
 msgid "Remark.PeakWind"
-msgstr "picco di vento di {1} nodi da {0} gradi a {2}:{3}"
+msgstr "peak wind of {1} knots from {0} degrees at {2}:{3}"
+
+#:
+msgid "Remark.Precipitation.Amount.Hourly"
+msgstr "{0}/100 of an inch of precipitation fell in the last hour"
+
+#:
+msgid "Remark.Precipitation.Amount.3.6"
+msgstr "{1} inches of precipitation fell in the last {0} hours"
+
+#:
+msgid "Remark.Precipitation.Amount.24"
+msgstr "{0} inches of precipitation fell in the last 24 hours"
+
+#:
+msgid "Remark.Precipitation.Beg"
+msgstr "{0} {1} beginning at {2}:{3}"
 
 #:
 msgid "Remark.Precipitation.Beg.End"
-msgstr "{0} {1} inizia a {2}:{3} e termina a {4}:{5}"
+msgstr "{0} {1} beginning at {2}:{3} ending at {4}:{5}"
+
+#:
+msgid "Remark.Precipitation.End"
+msgstr "{0} {1} ending at {2}:{3}"
+
+#:
+msgid "Remark.Pressure.Tendency"
+msgstr "of {0} hectopascals in the past 3 hours"
 
 #:
 msgid "Remark.PRESFR"
-msgstr "pressione in caduta rapidamente "
+msgstr "pressure falling rapidly"
 
 #:
 msgid "Remark.PRESRR"
-msgstr "pressione in salita rapidamente"
+msgstr "pressure rising rapidly"
 
 #:
 msgid "Remark.Second.Location.Visibility"
-msgstr "visibilità di {0} SM misurata da un secondo sensore situato a {1}"
+msgstr "visibility of {0} SM mesured by a second sensor located at {1}"
 
 #:
 msgid "Remark.Sea.Level.Pressure"
-msgstr "pressione a livello del mare di {0} HPa"
+msgstr "sea level pressure of {0} HPa"
 
 #:
 msgid "Remark.Sector.Visibility"
-msgstr "visibilità di {1} SM in direzione {0}"
+msgstr "visibility of {1} SM in the {0} direction"
 
 #:
 msgid "Remark.SLPNO"
-msgstr "pressione a livello del mare non disponibile"
+msgstr "sea level pressure not available"
+
+#:
+msgid "Remark.Snow.Depth"
+msgstr "snow depth of {0} inches"
 
 #:
 msgid "Remark.Snow.Increasing.Rapidly"
-msgstr "aumento dell’altezza della neve di {0} pollici nell’ultima ora con un’altezza totale al suolo di {1} pollici"
+msgstr "snow depth increase of {0} inches in the past hour with a total depth on the ground of {1} inches"
 
 #:
 msgid "Remark.Snow.Pellets"
-msgstr "{0} neve tonda "
+msgstr "{0} snow pellets"
+
+#:
+msgid "Remark.Sunshine.Duration"
+msgstr "{0} minutes of sunshine"
 
 #:
 msgid "Remark.Surface.Visibility"
-msgstr "visibilità in superficie di {0} Statute Miles"
+msgstr "surface visibility of {0} statute miles"
 
 #:
 msgid "Remark.Thunderstorm.Location"
-msgstr "temporale {0} dalla stazione"
+msgstr "thunderstorm {0} of the station"
 
 #:
 msgid "Remark.Thunderstorm.Location.Moving"
-msgstr "temporale {0} dalla stazione si muove in direzione di {1}"
+msgstr "thunderstorm {0} of the station moving towards {1}"
 
 #:
 msgid "Remark.Tornadic.Activity.Beginning"
-msgstr "{0} inizia a {1}:{2} {3} SM {4} dalla stazione"
+msgstr "{0} beginning at {1}:{2} {3} SM {4} of the station"
 
 #:
 msgid "Remark.Tornadic.Activity.BegEnd"
-msgstr "{0} inizia a {1}:{2} e termina a {3}:{4} {5} SM {6} dalla stazione"
+msgstr "{0} beginning at {1}:{2} ending at {3}:{4} {5} SM {6} of the station"
 
 #:
 msgid "Remark.Tornadic.Activity.Ending"
-msgstr "{0} termina a {1}:{2} {3} SM {4} dalla stazione"
+msgstr "{0} ending at {1}:{2} {3} SM {4} of the station"
 
 #:
 msgid "Remark.TORNADO"
 msgstr "tornado"
 
 #:
 msgid "Remark.Tower.Visibility"
-msgstr "visibilità dalla torre di controllo di {0} Statute Miles"
+msgstr "control tower visibility of {0} statute miles"
 
 #:
 msgid "Remark.Variable.Prevailing.Visibility"
-msgstr "visibilità prevalentemente variabile tra {0} e {1} SM"
+msgstr "variable prevailing visibility between {0} and {1} SM"
 
 #:
 msgid "Remark.Variable.Sky.Condition"
-msgstr "strato di nuvole che varia tra {0} e {1}"
+msgstr "cloud layer varying between {0} and {1}"
 
 #:
 msgid "Remark.Variable.Sky.Condition.Height"
-msgstr "strato di nubi a {0} piedi che varia tra {1} e {2}"
+msgstr "cloud layer at {0} feet varying between {1} and {2}"
 
 #:
 msgid "Remark.VIRGA"
 msgstr "virga"
 
 #:
 msgid "Remark.Virga.Direction"
-msgstr "virga {0} dalla stazione"
+msgstr "virga {0} from the station"
 
 #:
 msgid "Remark.WATERSPOUT"
-msgstr "tromba marina"
+msgstr "waterspout"
+
+#:
+msgid "Remark.Water.Equivalent.Snow.Ground"
+msgstr "water equivalent of {0} inches of snow"
 
 #:
 msgid "Remark.WindShift"
-msgstr "spostamento del vento a {0}:{1}"
+msgstr "wind shift at {0}:{1}"
 
 #:
 msgid "Remark.WindShift.FROPA"
-msgstr "spostamento del vento accompagnato da passaggio frontale a {0}:{1}"
+msgstr "wind shift accompanied by frontal passage at {0}:{1}"
 
 #:
 msgid "MetarFacade.InvalidIcao"
-msgstr "Codice ICAO non valido"
+msgstr "Icao code is invalid."
 
 #:
 msgid "Converter.D"
-msgstr "Diminuzione"
+msgstr "decreasing"
 
 #:
 msgid "Converter.E"
-msgstr "Est"
+msgstr "East"
 
 #:
 msgid "Converter.ENE"
-msgstr "Est Nord Est"
+msgstr "East North East"
 
 #:
 msgid "Converter.ESE"
-msgstr "Est Sud Est"
+msgstr "East South East"
 
 #:
 msgid "Converter.N"
-msgstr "Nord"
+msgstr "North"
 
 #:
 msgid "Converter.NE"
-msgstr "Nord Est"
+msgstr "North East"
 
 #:
 msgid "Converter.NNE"
-msgstr "Nord Nord Est"
+msgstr "North North East"
 
 #:
 msgid "Converter.NNW"
-msgstr "Nord Nord Ovest"
+msgstr "North North West"
 
 #:
 msgid "Converter.NSC"
-msgstr "nessun cambiamento significativo"
+msgstr "no significant change"
 
 #:
 msgid "Converter.NW"
-msgstr "Nord Ovest"
+msgstr "North West"
 
 #:
 msgid "Converter.S"
-msgstr "Sud"
+msgstr "South"
 
 #:
 msgid "Converter.SE"
-msgstr "Sud Est"
+msgstr "South East"
 
 #:
 msgid "Converter.SSE"
-msgstr "Sud Sud Est"
+msgstr "South South East"
 
 #:
 msgid "Converter.SSW"
-msgstr "Sud Sud Ovest"
+msgstr "South South West"
 
 #:
 msgid "Converter.SW"
-msgstr "Sud Ovest"
+msgstr "South West"
 
 #:
 msgid "Converter.U"
-msgstr "sempre più"
+msgstr "up rising"
 
 #:
 msgid "Converter.VRB"
-msgstr "Variabile"
+msgstr "Variable"
 
 #:
 msgid "Converter.W"
-msgstr "Ovest"
+msgstr "West"
 
 #:
 msgid "Converter.WNW"
-msgstr "Ovest Nord Ovest"
+msgstr "West North West"
 
 #:
 msgid "Converter.WSW"
-msgstr "Ovest Sud Ovest"
+msgstr "West South West"
 
 #:
 msgid "WeatherChangeType.FM"
-msgstr "Da"
+msgstr "From"
 
 #:
 msgid "WeatherChangeType.BECMG"
-msgstr "Diventa"
+msgstr "Becoming"
+
+#:
+msgid "WeatherChangeType.INTER"
+msgstr "Intermittent"
 
 #:
 msgid "WeatherChangeType.TEMPO"
-msgstr "Temporanea"
+msgstr "Temporary"
 
 #:
 msgid "WeatherChangeType.PROB"
-msgstr "Probabilità"
+msgstr "Probability"
 
 #:
 msgid "TimeIndicator.AT"
-msgstr "alle"
+msgstr "at"
 
 #:
 msgid "TimeIndicator.FM"
-msgstr "dalle"
+msgstr "From"
 
 #:
 msgid "TimeIndicator.TL"
-msgstr "fino alle"
+msgstr "until"
 
 #:
 msgid "ToString.airport"
-msgstr "aeroporto"
+msgstr "airport"
 
 #:
 msgid "ToString.altimeter"
-msgstr "altimetro (hPa)"
+msgstr "altimeter (hPa)"
 
 #:
 msgid "ToString.amendment"
-msgstr "emendamento"
+msgstr "amendment"
 
 #:
 msgid "ToString.auto"
 msgstr "auto"
 
 #:
+msgid "ToString.baseHeight"
+msgstr "base layer in feet"
+
+#:
 msgid "ToString.cavok"
 msgstr "cavok"
 
 #:
 msgid "ToString.clouds"
-msgstr "nuvole"
+msgstr "clouds"
 
 #:
 msgid "ToString.day.month"
-msgstr "giorno del mese"
+msgstr "day of the month"
 
 #:
 msgid "ToString.day.hour"
-msgstr "ora del giorno"
+msgstr "hour of the day"
 
 #:
 msgid "ToString.deposit.braking"
-msgstr "capacità frenante"
+msgstr "braking capacity"
 
 #:
 msgid "ToString.deposit.coverage"
-msgstr "copertura"
+msgstr "coverage"
 
 #:
 msgid "ToString.deposit.thickness"
-msgstr "spessore"
+msgstr "thickness"
 
 #:
 msgid "ToString.deposit.type"
-msgstr "tipo di deposito"
+msgstr "type of deposit"
+
+#:
+msgid "ToString.depth"
+msgstr "layer depth in feet"
 
 #:
 msgid "ToString.descriptive"
-msgstr "descrittivo"
+msgstr "descriptive"
 
 #:
 msgid "ToString.dew.point"
-msgstr "punto di rugiada"
+msgstr "dew point"
 
 #:
 msgid "ToString.end.day.month"
-msgstr "ultimo giorno del mese"
+msgstr "end day of the month"
 
 #:
 msgid "ToString.end.hour.day"
-msgstr "ultima ora del giorno"
+msgstr "end hour of the day"
+
+#:
+msgid "ToString.flags"
+msgstr "flags"
 
 #:
 msgid "ToString.height.feet"
-msgstr "altezza (ft)"
+msgstr "height (ft)"
 
 #:
 msgid "ToString.height.meter"
-msgstr "altezza (m)"
+msgstr "height (m)"
 
 #:
 msgid "ToString.intensity"
-msgstr "intensità"
+msgstr "intensity"
 
 #:
 msgid "ToString.indicator"
-msgstr "indicatore"
+msgstr "indicator"
 
 #:
 msgid "ToString.message"
-msgstr "messaggio originale"
+msgstr "original message"
 
 #:
 msgid "ToString.name"
-msgstr "nome"
+msgstr "name"
 
 #:
 msgid "ToString.nosig"
 msgstr "nosig"
 
 #:
 msgid "ToString.phenomenons"
-msgstr "fenomeni"
+msgstr "phenomenons"
 
 #:
 msgid "ToString.probability"
-msgstr "probabilità"
+msgstr "probability"
 
 #:
 msgid "ToString.quantity"
-msgstr "quantità"
+msgstr "quantity"
 
 #:
 msgid "ToString.remark"
-msgstr "remark"
+msgstr "remarks"
 
 #:
 msgid "ToString.report.time"
-msgstr "ora del rapporto"
+msgstr "time of report"
 
 #:
 msgid "ToString.runway.info"
-msgstr "informazioni sulle piste"
+msgstr "runways information"
 
 #:
 msgid "ToString.start.day.month"
-msgstr "primo giorno del mese"
+msgstr "starting day of the month"
 
 #:
 msgid "ToString.start.hour.day"
-msgstr "prima ora del giorno"
+msgstr "starting hour of the day"
 
 #:
 msgid "ToString.start.minute"
-msgstr "minuto di inizio"
+msgstr "starting minute"
 
 #:
 msgid "ToString.temperature"
-msgstr "temperatura (°C)"
+msgstr "temperature (°C)"
 
 #:
 msgid "ToString.temperature.max"
-msgstr "temperatura massima (°C)"
+msgstr "maximum temperature (°C)"
 
 #:
 msgid "ToString.temperature.min"
-msgstr "temperatura minima (°C)"
+msgstr "minimum temperature (°C)"
 
 #:
 msgid "ToString.trend"
-msgstr "tendenza"
+msgstr "trend"
 
 #:
 msgid "ToString.trends"
-msgstr "tendenze"
+msgstr "trends"
 
 #:
 msgid "ToString.type"
-msgstr "tipo"
+msgstr "type"
 
 #:
 msgid "ToString.visibility.main"
-msgstr "visibilità principale"
+msgstr "main visibility"
 
 #:
 msgid "ToString.visibility.min"
-msgstr "visibilità minima"
+msgstr "minimum visibility"
 
 #:
 msgid "ToString.visibility.min.direction"
-msgstr "direzione visibilità minima"
+msgstr "minimum visibility direction"
 
 #:
 msgid "ToString.visibility.max"
-msgstr "visibilità massima"
+msgstr "maximum visibility"
 
 #:
 msgid "ToString.vertical.visibility"
-msgstr "visibilità verticale (ft)"
+msgstr "vertical visibility (ft)"
 
 #:
 msgid "ToString.weather.conditions"
-msgstr "condizioni meteo"
+msgstr "weather conditions"
 
 #:
 msgid "ToString.wind.direction"
-msgstr "direzione"
+msgstr "direction"
 
 #:
 msgid "ToString.wind.direction.degrees"
-msgstr "direzione (gradi)"
+msgstr "direction (degrees)"
 
 #:
 msgid "ToString.wind.gusts"
-msgstr "raffiche"
+msgstr "gusts"
 
 #:
 msgid "ToString.wind.min.variation"
-msgstr "variazione minima del vento"
+msgstr "minimal wind variation"
 
 #:
 msgid "ToString.wind.max.variation"
-msgstr "variazione massima del vento"
+msgstr "maximal wind variation"
 
 #:
 msgid "ToString.wind.speed"
-msgstr "velocità"
+msgstr "speed"
 
 #:
 msgid "ToString.wind.unit"
-msgstr "unità"
+msgstr "unit"
+
+#:
+msgid "TurbulenceIntensity.0"
+msgstr "None"
+
+#:
+msgid "TurbulenceIntensity.1"
+msgstr "Light turbulence"
+
+#:
+msgid "TurbulenceIntensity.2"
+msgstr "Moderate turbulence in clear air, occasional"
+
+#:
+msgid "TurbulenceIntensity.3"
+msgstr "Moderate turbulence in clear air, frequent"
+
+#:
+msgid "TurbulenceIntensity.4"
+msgstr "Moderate turbulence in cloud, occasional"
+
+#:
+msgid "TurbulenceIntensity.5"
+msgstr "Moderate turbulence in cloud, frequent"
+
+#:
+msgid "TurbulenceIntensity.6"
+msgstr "Severe turbulence in clear air, occasional"
+
+#:
+msgid "TurbulenceIntensity.7"
+msgstr "Severe turbulence in clear air, frequent"
+
+#:
+msgid "TurbulenceIntensity.8"
+msgstr "Severe turbulence in cloud, occasional"
+
+#:
+msgid "TurbulenceIntensity.9"
+msgstr "Severe turbulence in cloud, frequent"
+
+#:
+msgid "TurbulenceIntensity.X"
+msgstr "Extreme turbulence"
```

### Comparing `metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/messages.pot` & `metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/it/LC_MESSAGES/messages.po`

 * *Files 18% similar despite different names*

```diff
@@ -1,142 +1,142 @@
 msgid ""
 msgstr ""
 "MIME-Version: 1.0"
 "Content-Type: text/plain; charset=UTF-8"
 "Content-Transfer-Encoding: 8bit"
 "X-Generator: prop2po"
 "Project-Id-Version: metar_taf_parser"
-"Language: en"
+"Language: it"
 #:
 msgid "CloudQuantity.BKN"
-msgstr "broken"
+msgstr "molto nuvoloso"
 
 #:
 msgid "CloudQuantity.FEW"
-msgstr "few"
+msgstr "leggermente nuvoloso"
 
 #:
 msgid "CloudQuantity.NSC"
-msgstr "no significant clouds."
+msgstr "Nessuna nuvola significativa"
 
 #:
 msgid "CloudQuantity.OVC"
-msgstr "overcast"
+msgstr "coperto"
 
 #:
 msgid "CloudQuantity.SCT"
-msgstr "scattered"
+msgstr "sparse"
 
 #:
 msgid "CloudQuantity.SKC"
-msgstr "sky clear"
+msgstr "cielo sereno"
 
 #:
 msgid "CloudType.AC"
-msgstr "Altocumulus"
+msgstr "Altocumulo"
 
 #:
 msgid "CloudType.AS"
-msgstr "Altostratus"
+msgstr "Altostrato"
 
 #:
 msgid "CloudType.CB"
-msgstr "Cumulonimbus"
+msgstr "Cumulonembo"
 
 #:
 msgid "CloudType.CC"
-msgstr "CirroCumulus"
+msgstr "Cirrocumulo"
 
 #:
 msgid "CloudType.CI"
-msgstr "Cirrus"
+msgstr "Cirro"
 
 #:
 msgid "CloudType.CS"
-msgstr "Cirrostratus"
+msgstr "Cirrostrato"
 
 #:
 msgid "CloudType.CU"
-msgstr "Cumulus"
+msgstr "Cumulo"
 
 #:
 msgid "CloudType.NS"
-msgstr "Nimbostratus"
+msgstr "Nembostrato"
 
 #:
 msgid "CloudType.SC"
-msgstr "Stratocumulus"
+msgstr "Stratocumulo"
 
 #:
 msgid "CloudType.ST"
-msgstr "Stratus"
+msgstr "Strato"
 
 #:
 msgid "CloudType.TCU"
-msgstr "Towering cumulus"
+msgstr "Cumuli torreggiantidecreasing"
 
 #:
 msgid "DepositBrakingCapacity.//"
-msgstr "not reported"
+msgstr "non riportato "
 
 #:
 msgid "DepositBrakingCapacity.91"
-msgstr "poor"
+msgstr "scarso"
 
 #:
 msgid "DepositBrakingCapacity.92"
-msgstr "poor/medium"
+msgstr "medio/scarso"
 
 #:
 msgid "DepositBrakingCapacity.93"
-msgstr "medium"
+msgstr "medio"
 
 #:
 msgid "DepositBrakingCapacity.94"
-msgstr "medium/good"
+msgstr "medio/buono"
 
 #:
 msgid "DepositBrakingCapacity.95"
-msgstr "good"
+msgstr "buono"
 
 #:
 msgid "DepositBrakingCapacity.99"
-msgstr "figures unreliable"
+msgstr "cifre inaffidabili"
 
 #:
 msgid "DepositBrakingCapacity.default"
-msgstr "friction coefficient of {0}"
+msgstr "coefficiente di attrito di {0}"
 
 #:
 msgid "DepositCoverage.NOT_REPORTED"
-msgstr "not reported"
+msgstr "non riportato"
 
 #:
 msgid "DepositCoverage.LESS_10"
-msgstr "less than 10%"
+msgstr "meno del 10%"
 
 #:
 msgid "DepositCoverage.FROM_11_TO_25"
-msgstr "from 11% to 25%"
+msgstr "dal 11% al 25%"
 
 #:
 msgid "DepositCoverage.FROM_26_TO_50"
-msgstr "from 26% to 50%"
+msgstr "dal 26% al 50%"
 
 #:
 msgid "DepositCoverage.FROM_51_TO_100"
-msgstr "from 51% to 100%"
+msgstr "dal 51% al 100%"
 
 #:
 msgid "DepositThickness.//"
-msgstr "not reported"
+msgstr "non riportato"
 
 #:
 msgid "DepositThickness.00"
-msgstr "less than 1 mm"
+msgstr "meno di 1 mm"
 
 #:
 msgid "DepositThickness.92"
 msgstr "10 cm"
 
 #:
 msgid "DepositThickness.93"
@@ -156,929 +156,925 @@
 
 #:
 msgid "DepositThickness.97"
 msgstr "35 cm"
 
 #:
 msgid "DepositThickness.98"
-msgstr "40 cm or more"
+msgstr "40 cm"
 
 #:
 msgid "DepositThickness.99"
-msgstr "closed"
+msgstr "chiusa"
 
 #:
 msgid "DepositThickness.default"
 msgstr "{0} mm"
 
 #:
 msgid "DepositType.NOT_REPORTED"
-msgstr "not reported"
+msgstr "non riportato"
 
 #:
 msgid "DepositType.CLEAR_DRY"
-msgstr "clear and dry"
+msgstr "pulita e asciutta"
 
 #:
 msgid "DepositType.DAMP"
-msgstr "damp"
+msgstr "umido"
 
 #:
 msgid "DepositType.WET_WATER_PATCHES"
-msgstr "wet or water patches"
+msgstr "pozzanghere bagnate"
 
 #:
 msgid "DepositType.RIME_FROST_COVERED"
-msgstr "rime or frost covered"
+msgstr "ricoperta di brina"
 
 #:
 msgid "DepositType.DRY_SNOW"
-msgstr "dry snow"
+msgstr "neve asciutta"
 
 #:
 msgid "DepositType.WET_SNOW"
-msgstr "wet snow"
+msgstr "neve bagnata"
 
 #:
 msgid "DepositType.ICE"
-msgstr "ice"
+msgstr "ghiaccio"
 
 #:
 msgid "DepositType.COMPACTED_SNOW"
-msgstr "compacted or rolled snow"
+msgstr "neve compatta"
 
 #:
 msgid "DepositType.FROZEN_RIDGES"
-msgstr "frozen ruts or ridges"
+msgstr "solchi o creste congelate"
 
 #:
 msgid "DepositType.SLUSH"
-msgstr "slush"
+msgstr "fanghiglia"
 
 #:
 msgid "Descriptive.BC"
-msgstr "patches"
+msgstr "banchi di nebbia"
 
 #:
 msgid "Descriptive.BL"
-msgstr "blowing"
+msgstr "sollevamento alto"
 
 #:
 msgid "Descriptive.DR"
-msgstr "low drifting"
+msgstr "sollevamento basso"
 
 #:
 msgid "Descriptive.FZ"
-msgstr "freezing"
+msgstr "congelantesi"
 
 #:
 msgid "Descriptive.MI"
-msgstr "shallow"
+msgstr "strati di nebbia"
 
 #:
 msgid "Descriptive.PR"
-msgstr "partial"
+msgstr "parziale"
 
 #:
 msgid "Descriptive.SH"
-msgstr "showers of"
+msgstr "rovescio"
 
 #:
 msgid "Descriptive.TS"
-msgstr "thunderstorm"
+msgstr "temporale"
 
 #:
 msgid "Error.prefix"
-msgstr "An error occured. Error code n°"
+msgstr "Si è verificato un errore. Errore nr. "
 
 #:
 msgid "ErrorCode.AirportNotFound"
-msgstr "The airport was not found for this message."
+msgstr "L’aeroporto non è stato trovato in questa notifica"
 
 #:
 msgid "ErrorCode.InvalidMessage"
-msgstr "The entered message is invalid."
+msgstr "Il messaggio non è valido"
 
 #:
 msgid "Flag.AMD"
-msgstr "amended TAF"
+msgstr "TAF modificato"
 
 #:
 msgid "Flag.AUTO"
-msgstr "automated METAR"
+msgstr "METAR automatizzato"
 
 #:
 msgid "Flag.CNL"
-msgstr "canceled TAF"
+msgstr "TAF cancellato"
 
 #:
 msgid "Flag.COR"
-msgstr "corrected METAR/TAF"
+msgstr "METAR/TAF corretto"
 
 #:
 msgid "Flag.NIL"
-msgstr "no data"
+msgstr "nessun dato"
 
 #:
 msgid "IcingIntensity.0"
-msgstr "Trace Icing or None"
+msgstr "Trace di ghiaccio o nessuno"
 
 #:
 msgid "IcingIntensity.1"
-msgstr "Light Mixed Icing"
+msgstr "Ghiaccio misto leggero"
 
 #:
 msgid "IcingIntensity.2"
-msgstr "Light Rime Icing In Cloud"
+msgstr "Ghiacciamento leggero in nuvola"
 
 #:
 msgid "IcingIntensity.3"
-msgstr "Light Clear Icing In Precipitation"
+msgstr "Ghiacciamento chiaro leggero in precipitazione"
 
 #:
 msgid "IcingIntensity.4"
-msgstr "Moderate Mixed Icing"
+msgstr "Ghiaccio misto moderato"
 
 #:
 msgid "IcingIntensity.5"
-msgstr "Moderate Rime Icing In Cloud"
+msgstr "Ghiacciamento moderato in nuvola"
 
 #:
 msgid "IcingIntensity.6"
-msgstr "Moderate Clear Icing In Precipitation"
+msgstr "Ghiacciamento chiaro moderato in precipitazione"
 
 #:
 msgid "IcingIntensity.7"
-msgstr "Severe Mixed Icing"
+msgstr "Ghiaccio misto grave"
 
 #:
 msgid "IcingIntensity.8"
-msgstr "Severe Rime Icing In Cloud"
+msgstr "Ghiacciamento grave in nuvola"
 
 #:
 msgid "IcingIntensity.9"
-msgstr "Severe Clear Icing In Precipitation"
+msgstr "Grave Ghiacciamento chiaro in precipitazione"
 
 #:
 msgid "Indicator.M"
-msgstr "less than"
+msgstr "minore di"
 
 #:
 msgid "Indicator.P"
-msgstr "greater than"
+msgstr "maggiore di"
 
 #:
 msgid "Intensity.-"
-msgstr "Light"
+msgstr "Debole"
 
 #:
 msgid "Intensity.+"
-msgstr "Heavy"
-
-#:
-msgid "Intensity.RE"
-msgstr "Recent"
+msgstr "Forte"
 
 #:
 msgid "Intensity.VC"
-msgstr "In the vicinity"
+msgstr "Nelle vicinanze"
 
 #:
 msgid "Phenomenon.BR"
-msgstr "mist"
+msgstr "foschia"
 
 #:
 msgid "Phenomenon.DS"
-msgstr "duststorm"
+msgstr "tempesta di polvere "
 
 #:
 msgid "Phenomenon.DU"
-msgstr "widespread dust"
+msgstr "polvere su un’area estesa"
 
 #:
 msgid "Phenomenon.DZ"
-msgstr "drizzle"
+msgstr "pioviggine"
 
 #:
 msgid "Phenomenon.FC"
-msgstr "funnel cloud"
+msgstr "tornado o tromba marina"
 
 #:
 msgid "Phenomenon.FG"
-msgstr "fog"
+msgstr "nebbia"
 
 #:
 msgid "Phenomenon.FU"
-msgstr "smoke"
+msgstr "fumo"
 
 #:
 msgid "Phenomenon.GR"
-msgstr "hail"
+msgstr "grandine"
 
 #:
 msgid "Phenomenon.GS"
-msgstr "small hail and/or snow pellets"
+msgstr "grandine piccola e/o granuli di neve"
 
 #:
 msgid "Phenomenon.HZ"
-msgstr "haze"
+msgstr "caligine"
 
 #:
 msgid "Phenomenon.IC"
-msgstr "ice crystals"
+msgstr "cristalli di ghiaccio"
 
 #:
 msgid "Phenomenon.PL"
-msgstr "ice pellets"
+msgstr "granuli di ghiaccio"
 
 #:
 msgid "Phenomenon.PO"
-msgstr "dust or sand whirls"
+msgstr "mulinelli di polvere/sabbia"
 
 #:
 msgid "Phenomenon.PY"
-msgstr "spray"
+msgstr "schizzi"
 
 #:
 msgid "Phenomenon.RA"
-msgstr "rain"
+msgstr "pioggia"
 
 #:
 msgid "Phenomenon.SA"
-msgstr "sand"
+msgstr "sabbia"
 
 #:
 msgid "Phenomenon.SG"
-msgstr "snow grains"
+msgstr "neve granulosa"
 
 #:
 msgid "Phenomenon.SN"
-msgstr "snow"
+msgstr "neve"
 
 #:
 msgid "Phenomenon.SQ"
-msgstr "squall"
+msgstr "groppo"
 
 #:
 msgid "Phenomenon.SS"
-msgstr "sandstorm"
+msgstr "tempesta di sabbia"
 
 #:
 msgid "Phenomenon.UP"
-msgstr "unknown precipitation"
+msgstr "precipitazione sconosciuta"
 
 #:
 msgid "Phenomenon.VA"
-msgstr "volcanic ash"
+msgstr "cenere vulcanica"
 
 #:
 msgid "Phenomenon.TS"
-msgstr "thunderstorm"
+msgstr "temporale"
 
 #:
 msgid "Remark.AO1"
-msgstr "automated stations without a precipitation discriminator"
+msgstr "stazioni automatizzate senza discriminatore di precipitazione"
 
 #:
 msgid "Remark.AO2"
-msgstr "automated station with a precipitation discriminator"
+msgstr "stazione automatizzata con discriminatore di precipitazione"
 
 #:
 msgid "Remark.ALQDS"
-msgstr "all quadrants"
+msgstr "tutti i quadranti"
 
 #:
 msgid "Remark.Barometer.0"
-msgstr "Increase, then decrease"
+msgstr "Incrementa, poi diminuisci"
 
 #:
 msgid "Remark.Barometer.1"
-msgstr "Increase, then steady, or increase then Increase more slowly"
+msgstr "Incrementa, poi stabile, o aumenta poi aumenta più lentamente"
 
 #:
 msgid "Remark.Barometer.2"
-msgstr "steady or unsteady increase"
+msgstr "aumento costante o instabile"
 
 #:
 msgid "Remark.Barometer.3"
-msgstr "Decrease or steady, then increase; or increase then increase more rapidly"
+msgstr "Diminuire o stabile, quindi aumentare; o aumentare poi aumentare più rapidamente"
 
 #:
 msgid "Remark.Barometer.4"
-msgstr "Steady"
+msgstr "Costante"
 
 #:
 msgid "Remark.Barometer.5"
-msgstr "Decrease, then increase"
+msgstr "Diminuire, poi aumentare"
 
 #:
 msgid "Remark.Barometer.6"
-msgstr "Decrease then steady; or decrease then decrease more slowly"
+msgstr "Diminuire quindi costante; o diminuire, quindi diminuire più lentamente"
 
 #:
 msgid "Remark.Barometer.7"
-msgstr "Steady or unsteady decrease"
+msgstr "Riduzione costante o instabile"
 
 #:
 msgid "Remark.Barometer.8"
-msgstr "Steady or increase, then decrease; or decrease then decrease more rapidly"
+msgstr "Stazionario o aumenta, quindi diminuisce; o diminuire poi diminuisce più rapidamente"
 
 #:
 msgid "Remark.BASED"
-msgstr "based"
+msgstr "basato"
 
 #:
 msgid "Remark.Ceiling.Height"
-msgstr "ceiling varying between {0} and {1} feet"
+msgstr "base delle nubi tra {0} e {1} piedi"
 
 #:
 msgid "Remark.Ceiling.Second.Location"
-msgstr "ceiling of {0} feet mesured by a second sensor located at {1}"
+msgstr "base delle nubi di {0} piedi misurato da un secondo sensore situato a {1}"
 
 #:
 msgid "Remark.DSNT"
-msgstr "distant"
+msgstr "distante"
 
 #:
 msgid "Remark.FCST"
-msgstr "forecast"
+msgstr "previsione"
 
 #:
 msgid "Remark.FUNNELCLOUD"
-msgstr "funnel cloud"
+msgstr "nuvole a imbuto"
 
 #:
 msgid "Remark.Hail"
-msgstr "largest hailstones with a diameter of {0} inches"
+msgstr "chicchi di grandine più grandi con un diametro di {0} pollici"
 
 #:
 msgid "Remark.Hail.LesserThan"
-msgstr "largest hailstones with a diameter less than {0} inches"
+msgstr "chicchi di grandine più grandi con un diametro inferiore di {0} pollici"
 
 #:
 msgid "Remark.Hourly.Maximum.Temperature"
-msgstr "6-hourly maximum temperature of {0}°C"
+msgstr "Temperatura massima ogni 6 ore di {0}°C"
 
 #:
 msgid "Remark.Hourly.Maximum.Minimum.Temperature"
-msgstr "24-hour maximum temperature of {0}°C and 24-hour minimum temperature of {1}°C"
+msgstr "Temperatura massima ogni 24 ore di {0}°C e temperatura minima ogni 24 ore di {1}°C"
 
 #:
 msgid "Remark.Hourly.Minimum.Temperature"
-msgstr "6-hourly minimum temperature of {0}°C"
+msgstr "Temperatura minima su 6 ore di {0}°C"
 
 #:
 msgid "Remark.Hourly.Temperature"
-msgstr "hourly temperature of {0}°C"
+msgstr "temperatura oraria di {0}°C"
 
 #:
 msgid "Remark.Hourly.Temperature.Dew.Point"
-msgstr "hourly temperature of {0}°C and dew point of {1}°C"
+msgstr "temperatura oraria di {0}°C e punto di rugiada di {1}°C"
 
 #:
 msgid "Remark.Ice.Accretion.Amount"
-msgstr "{0}/100 of an inch of ice accretion in the past {1} hour(s)"
+msgstr "{0}/100 di pollice di accrescimento di ghiaccio nelle ultime {1} ore"
 
 #:
 msgid "Remark.HVY"
-msgstr "heavy"
+msgstr "pesante"
 
 #:
 msgid "Remark.LGT"
-msgstr "light"
+msgstr "leggero"
 
 #:
 msgid "Remark.LTG"
-msgstr "lightning"
+msgstr "fulmine"
 
 #:
 msgid "Remark.MOD"
-msgstr "moderate"
+msgstr "moderato"
 
 #:
 msgid "Remark.Obscuration"
-msgstr "{0} layer at {1} feet composed of {2}"
+msgstr "{0} strato a {1} piedi composto da {2}"
 
 #:
 msgid "Remark.ON"
 msgstr "on"
 
 #:
 msgid "Remark.NXT"
-msgstr "next"
+msgstr "prossimo"
 
 #:
 msgid "Remark.PeakWind"
-msgstr "peak wind of {1} knots from {0} degrees at {2}:{3}"
+msgstr "picco di vento di {1} nodi da {0} gradi a {2}:{3}"
 
 #:
 msgid "Remark.Precipitation.Amount.Hourly"
-msgstr "{0}/100 of an inch of precipitation fell in the last hour"
+msgstr "Nell''ultima ora è caduto {0}/100 di pollice di precipitazioni"
 
 #:
 msgid "Remark.Precipitation.Amount.3.6"
-msgstr "{1} inches of precipitation fell in the last {0} hours"
+msgstr "{1} pollici di precipitazioni sono caduti nelle ultime {0} ore"
 
 #:
 msgid "Remark.Precipitation.Amount.24"
-msgstr "{0} inches of precipitation fell in the last 24 hours"
+msgstr "{0} pollici di precipitazioni sono caduti nelle ultime 24 ore"
 
 #:
 msgid "Remark.Precipitation.Beg"
-msgstr "{0} {1} beginning at {2}:{3}"
+msgstr "{0} {1} inizia alle {2}:{3}"
 
 #:
 msgid "Remark.Precipitation.Beg.End"
-msgstr "{0} {1} beginning at {2}:{3} ending at {4}:{5}"
+msgstr "{0} {1} inizia a {2}:{3} e termina a {4}:{5}"
 
 #:
 msgid "Remark.Precipitation.End"
-msgstr "{0} {1} ending at {2}:{3}"
+msgstr "{0} {1} termina alle {2}:{3}"
 
 #:
 msgid "Remark.Pressure.Tendency"
-msgstr "of {0} hectopascals in the past 3 hours"
+msgstr "di {0} HPa nelle ultime 3 ore"
 
 #:
 msgid "Remark.PRESFR"
-msgstr "pressure falling rapidly"
+msgstr "pressione in caduta rapidamente "
 
 #:
 msgid "Remark.PRESRR"
-msgstr "pressure rising rapidly"
+msgstr "pressione in salita rapidamente"
 
 #:
 msgid "Remark.Second.Location.Visibility"
-msgstr "visibility of {0} SM mesured by a second sensor located at {1}"
+msgstr "visibilità di {0} SM misurata da un secondo sensore situato a {1}"
 
 #:
 msgid "Remark.Sea.Level.Pressure"
-msgstr "sea level pressure of {0} HPa"
+msgstr "pressione a livello del mare di {0} HPa"
 
 #:
 msgid "Remark.Sector.Visibility"
-msgstr "visibility of {1} SM in the {0} direction"
+msgstr "visibilità di {1} SM in direzione {0}"
 
 #:
 msgid "Remark.SLPNO"
-msgstr "sea level pressure not available"
+msgstr "pressione a livello del mare non disponibile"
 
 #:
 msgid "Remark.Snow.Depth"
-msgstr "snow depth of {0} inches"
+msgstr "altezza della neve di {0} pollici"
 
 #:
 msgid "Remark.Snow.Increasing.Rapidly"
-msgstr "snow depth increase of {0} inches in the past hour with a total depth on the ground of {1} inches"
+msgstr "aumento dell’altezza della neve di {0} pollici nell’ultima ora con un’altezza totale al suolo di {1} pollici"
 
 #:
 msgid "Remark.Snow.Pellets"
-msgstr "{0} snow pellets"
+msgstr "{0} neve tonda "
 
 #:
 msgid "Remark.Sunshine.Duration"
-msgstr "{0} minutes of sunshine"
+msgstr "{0} minuti di sole"
 
 #:
 msgid "Remark.Surface.Visibility"
-msgstr "surface visibility of {0} statute miles"
+msgstr "visibilità in superficie di {0} Statute Miles"
 
 #:
 msgid "Remark.Thunderstorm.Location"
-msgstr "thunderstorm {0} of the station"
+msgstr "temporale {0} dalla stazione"
 
 #:
 msgid "Remark.Thunderstorm.Location.Moving"
-msgstr "thunderstorm {0} of the station moving towards {1}"
+msgstr "temporale {0} dalla stazione si muove in direzione di {1}"
 
 #:
 msgid "Remark.Tornadic.Activity.Beginning"
-msgstr "{0} beginning at {1}:{2} {3} SM {4} of the station"
+msgstr "{0} inizia a {1}:{2} {3} SM {4} dalla stazione"
 
 #:
 msgid "Remark.Tornadic.Activity.BegEnd"
-msgstr "{0} beginning at {1}:{2} ending at {3}:{4} {5} SM {6} of the station"
+msgstr "{0} inizia a {1}:{2} e termina a {3}:{4} {5} SM {6} dalla stazione"
 
 #:
 msgid "Remark.Tornadic.Activity.Ending"
-msgstr "{0} ending at {1}:{2} {3} SM {4} of the station"
+msgstr "{0} termina a {1}:{2} {3} SM {4} dalla stazione"
 
 #:
 msgid "Remark.TORNADO"
 msgstr "tornado"
 
 #:
 msgid "Remark.Tower.Visibility"
-msgstr "control tower visibility of {0} statute miles"
+msgstr "visibilità dalla torre di controllo di {0} Statute Miles"
 
 #:
 msgid "Remark.Variable.Prevailing.Visibility"
-msgstr "variable prevailing visibility between {0} and {1} SM"
+msgstr "visibilità prevalentemente variabile tra {0} e {1} SM"
 
 #:
 msgid "Remark.Variable.Sky.Condition"
-msgstr "cloud layer varying between {0} and {1}"
+msgstr "strato di nuvole che varia tra {0} e {1}"
 
 #:
 msgid "Remark.Variable.Sky.Condition.Height"
-msgstr "cloud layer at {0} feet varying between {1} and {2}"
+msgstr "strato di nubi a {0} piedi che varia tra {1} e {2}"
 
 #:
 msgid "Remark.VIRGA"
 msgstr "virga"
 
 #:
 msgid "Remark.Virga.Direction"
-msgstr "virga {0} from the station"
+msgstr "virga {0} dalla stazione"
 
 #:
 msgid "Remark.WATERSPOUT"
-msgstr "waterspout"
+msgstr "tromba marina"
 
 #:
 msgid "Remark.Water.Equivalent.Snow.Ground"
-msgstr "water equivalent of {0} inches of snow"
+msgstr "equivalente in acqua di {0} pollici di neve"
 
 #:
 msgid "Remark.WindShift"
-msgstr "wind shift at {0}:{1}"
+msgstr "spostamento del vento a {0}:{1}"
 
 #:
 msgid "Remark.WindShift.FROPA"
-msgstr "wind shift accompanied by frontal passage at {0}:{1}"
+msgstr "spostamento del vento accompagnato da passaggio frontale a {0}:{1}"
 
 #:
 msgid "MetarFacade.InvalidIcao"
-msgstr "Icao code is invalid."
+msgstr "Codice ICAO non valido"
 
 #:
 msgid "Converter.D"
-msgstr "decreasing"
+msgstr "Diminuzione"
 
 #:
 msgid "Converter.E"
-msgstr "East"
+msgstr "Est"
 
 #:
 msgid "Converter.ENE"
-msgstr "East North East"
+msgstr "Est Nord Est"
 
 #:
 msgid "Converter.ESE"
-msgstr "East South East"
+msgstr "Est Sud Est"
 
 #:
 msgid "Converter.N"
-msgstr "North"
+msgstr "Nord"
 
 #:
 msgid "Converter.NE"
-msgstr "North East"
+msgstr "Nord Est"
 
 #:
 msgid "Converter.NNE"
-msgstr "North North East"
+msgstr "Nord Nord Est"
 
 #:
 msgid "Converter.NNW"
-msgstr "North North West"
+msgstr "Nord Nord Ovest"
 
 #:
 msgid "Converter.NSC"
-msgstr "no significant change"
+msgstr "nessun cambiamento significativo"
 
 #:
 msgid "Converter.NW"
-msgstr "North West"
+msgstr "Nord Ovest"
 
 #:
 msgid "Converter.S"
-msgstr "South"
+msgstr "Sud"
 
 #:
 msgid "Converter.SE"
-msgstr "South East"
+msgstr "Sud Est"
 
 #:
 msgid "Converter.SSE"
-msgstr "South South East"
+msgstr "Sud Sud Est"
 
 #:
 msgid "Converter.SSW"
-msgstr "South South West"
+msgstr "Sud Sud Ovest"
 
 #:
 msgid "Converter.SW"
-msgstr "South West"
+msgstr "Sud Ovest"
 
 #:
 msgid "Converter.U"
-msgstr "up rising"
+msgstr "sempre più"
 
 #:
 msgid "Converter.VRB"
-msgstr "Variable"
+msgstr "Variabile"
 
 #:
 msgid "Converter.W"
-msgstr "West"
+msgstr "Ovest"
 
 #:
 msgid "Converter.WNW"
-msgstr "West North West"
+msgstr "Ovest Nord Ovest"
 
 #:
 msgid "Converter.WSW"
-msgstr "West South West"
+msgstr "Ovest Sud Ovest"
 
 #:
 msgid "WeatherChangeType.FM"
-msgstr "From"
+msgstr "Da"
 
 #:
 msgid "WeatherChangeType.BECMG"
-msgstr "Becoming"
+msgstr "Diventa"
 
 #:
 msgid "WeatherChangeType.INTER"
-msgstr "Intermittent"
+msgstr "Intermittente"
 
 #:
 msgid "WeatherChangeType.TEMPO"
-msgstr "Temporary"
+msgstr "Temporanea"
 
 #:
 msgid "WeatherChangeType.PROB"
-msgstr "Probability"
+msgstr "Probabilità"
 
 #:
 msgid "TimeIndicator.AT"
-msgstr "at"
+msgstr "alle"
 
 #:
 msgid "TimeIndicator.FM"
-msgstr "From"
+msgstr "dalle"
 
 #:
 msgid "TimeIndicator.TL"
-msgstr "until"
+msgstr "fino alle"
 
 #:
 msgid "ToString.airport"
-msgstr "airport"
+msgstr "aeroporto"
 
 #:
 msgid "ToString.altimeter"
-msgstr "altimeter (hPa)"
+msgstr "altimetro (hPa)"
 
 #:
 msgid "ToString.amendment"
-msgstr "amendment"
+msgstr "emendamento"
 
 #:
 msgid "ToString.auto"
 msgstr "auto"
 
 #:
 msgid "ToString.baseHeight"
-msgstr "base layer in feet"
+msgstr "strato di base in piedi"
 
 #:
 msgid "ToString.cavok"
 msgstr "cavok"
 
 #:
 msgid "ToString.clouds"
-msgstr "clouds"
+msgstr "nuvole"
 
 #:
 msgid "ToString.day.month"
-msgstr "day of the month"
+msgstr "giorno del mese"
 
 #:
 msgid "ToString.day.hour"
-msgstr "hour of the day"
+msgstr "ora del giorno"
 
 #:
 msgid "ToString.deposit.braking"
-msgstr "braking capacity"
+msgstr "capacità frenante"
 
 #:
 msgid "ToString.deposit.coverage"
-msgstr "coverage"
+msgstr "copertura"
 
 #:
 msgid "ToString.deposit.thickness"
-msgstr "thickness"
+msgstr "spessore"
 
 #:
 msgid "ToString.deposit.type"
-msgstr "type of deposit"
+msgstr "tipo di deposito"
 
 #:
 msgid "ToString.depth"
-msgstr "layer depth in feet"
+msgstr "profondità dello strato nei piedi"
 
 #:
 msgid "ToString.descriptive"
-msgstr "descriptive"
+msgstr "descrittivo"
 
 #:
 msgid "ToString.dew.point"
-msgstr "dew point"
+msgstr "punto di rugiada"
 
 #:
 msgid "ToString.end.day.month"
-msgstr "end day of the month"
+msgstr "ultimo giorno del mese"
 
 #:
 msgid "ToString.end.hour.day"
-msgstr "end hour of the day"
+msgstr "ultima ora del giorno"
 
 #:
 msgid "ToString.flags"
-msgstr "flags"
+msgstr "bandiere"
 
 #:
 msgid "ToString.height.feet"
-msgstr "height (ft)"
+msgstr "altezza (ft)"
 
 #:
 msgid "ToString.height.meter"
-msgstr "height (m)"
+msgstr "altezza (m)"
 
 #:
 msgid "ToString.intensity"
-msgstr "intensity"
+msgstr "intensità"
 
 #:
 msgid "ToString.indicator"
-msgstr "indicator"
+msgstr "indicatore"
 
 #:
 msgid "ToString.message"
-msgstr "original message"
+msgstr "messaggio originale"
 
 #:
 msgid "ToString.name"
-msgstr "name"
+msgstr "nome"
 
 #:
 msgid "ToString.nosig"
 msgstr "nosig"
 
 #:
 msgid "ToString.phenomenons"
-msgstr "phenomenons"
+msgstr "fenomeni"
 
 #:
 msgid "ToString.probability"
-msgstr "probability"
+msgstr "probabilità"
 
 #:
 msgid "ToString.quantity"
-msgstr "quantity"
+msgstr "quantità"
 
 #:
 msgid "ToString.remark"
-msgstr "remarks"
+msgstr "remark"
 
 #:
 msgid "ToString.report.time"
-msgstr "time of report"
+msgstr "ora del rapporto"
 
 #:
 msgid "ToString.runway.info"
-msgstr "runways information"
+msgstr "informazioni sulle piste"
 
 #:
 msgid "ToString.start.day.month"
-msgstr "starting day of the month"
+msgstr "primo giorno del mese"
 
 #:
 msgid "ToString.start.hour.day"
-msgstr "starting hour of the day"
+msgstr "prima ora del giorno"
 
 #:
 msgid "ToString.start.minute"
-msgstr "starting minute"
+msgstr "minuto di inizio"
 
 #:
 msgid "ToString.temperature"
-msgstr "temperature (°C)"
+msgstr "temperatura (°C)"
 
 #:
 msgid "ToString.temperature.max"
-msgstr "maximum temperature (°C)"
+msgstr "temperatura massima (°C)"
 
 #:
 msgid "ToString.temperature.min"
-msgstr "minimum temperature (°C)"
+msgstr "temperatura minima (°C)"
 
 #:
 msgid "ToString.trend"
-msgstr "trend"
+msgstr "tendenza"
 
 #:
 msgid "ToString.trends"
-msgstr "trends"
+msgstr "tendenze"
 
 #:
 msgid "ToString.type"
-msgstr "type"
+msgstr "tipo"
 
 #:
 msgid "ToString.visibility.main"
-msgstr "main visibility"
+msgstr "visibilità principale"
 
 #:
 msgid "ToString.visibility.min"
-msgstr "minimum visibility"
+msgstr "visibilità minima"
 
 #:
 msgid "ToString.visibility.min.direction"
-msgstr "minimum visibility direction"
+msgstr "direzione visibilità minima"
 
 #:
 msgid "ToString.visibility.max"
-msgstr "maximum visibility"
+msgstr "visibilità massima"
 
 #:
 msgid "ToString.vertical.visibility"
-msgstr "vertical visibility (ft)"
+msgstr "visibilità verticale (ft)"
 
 #:
 msgid "ToString.weather.conditions"
-msgstr "weather conditions"
+msgstr "condizioni meteo"
 
 #:
 msgid "ToString.wind.direction"
-msgstr "direction"
+msgstr "direzione"
 
 #:
 msgid "ToString.wind.direction.degrees"
-msgstr "direction (degrees)"
+msgstr "direzione (gradi)"
 
 #:
 msgid "ToString.wind.gusts"
-msgstr "gusts"
+msgstr "raffiche"
 
 #:
 msgid "ToString.wind.min.variation"
-msgstr "minimal wind variation"
+msgstr "variazione minima del vento"
 
 #:
 msgid "ToString.wind.max.variation"
-msgstr "maximal wind variation"
+msgstr "variazione massima del vento"
 
 #:
 msgid "ToString.wind.speed"
-msgstr "speed"
+msgstr "velocità"
 
 #:
 msgid "ToString.wind.unit"
-msgstr "unit"
+msgstr "unità"
 
 #:
 msgid "TurbulenceIntensity.0"
-msgstr "None"
+msgstr "Nessuno"
 
 #:
 msgid "TurbulenceIntensity.1"
-msgstr "Light turbulence"
+msgstr "Turbolenza leggera"
 
 #:
 msgid "TurbulenceIntensity.2"
-msgstr "Moderate turbulence in clear air, occasional"
+msgstr "Moderata turbolenza con aria limpida, occasionale"
 
 #:
 msgid "TurbulenceIntensity.3"
-msgstr "Moderate turbulence in clear air, frequent"
+msgstr "Moderata turbolenza con aria limpida, frequente"
 
 #:
 msgid "TurbulenceIntensity.4"
-msgstr "Moderate turbulence in cloud, occasional"
+msgstr "Moderata turbolenza in nubi, occasionale"
 
 #:
 msgid "TurbulenceIntensity.5"
-msgstr "Moderate turbulence in cloud, frequent"
+msgstr "Moderata turbolenza in nubi, frequente"
 
 #:
 msgid "TurbulenceIntensity.6"
-msgstr "Severe turbulence in clear air, occasional"
+msgstr "Forte turbolenza in aria limpida, occasionale"
 
 #:
 msgid "TurbulenceIntensity.7"
-msgstr "Severe turbulence in clear air, frequent"
+msgstr "Forte turbolenza in aria limpida, frequente"
 
 #:
 msgid "TurbulenceIntensity.8"
-msgstr "Severe turbulence in cloud, occasional"
+msgstr "Forte turbolenza in nubi, occasionale"
 
 #:
 msgid "TurbulenceIntensity.9"
-msgstr "Severe turbulence in cloud, frequent"
+msgstr "Forte turbolenza in nubi, frequente"
 
 #:
 msgid "TurbulenceIntensity.X"
-msgstr "Extreme turbulence"
+msgstr "Estrema turbolenza"
```

### Comparing `metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/pl/LC_MESSAGES/messages.mo` & `metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/pl/LC_MESSAGES/messages.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -4,15 +4,15 @@
 "PO-Revision-Date: \n"
 "Last-Translator: \n"
 "Language-Team: \n"
 "Language: pl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"X-Generator: Poedit 3.2\n"
+"X-Generator: Poedit 3.4.2\n"
 
 msgid "CloudQuantity.BKN"
 msgstr "Od 5/8 do 7/8"
 
 msgid "CloudQuantity.FEW"
 msgstr "Od 1/8 do 2/8"
```

### Comparing `metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/ru-RU/LC_MESSAGES/messages.mo` & `metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/ru-RU/LC_MESSAGES/messages.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -252,14 +252,19 @@
 
 msgid "Error.prefix"
 msgstr "Произошла ошибка. Код ошибки n°"
 
 msgid "ErrorCode.AirportNotFound"
 msgstr "Аэропорт не найден для этого сообщения."
 
+msgid "ErrorCode.IncompleteRunwayInformation"
+msgstr ""
+"Информация о взлетно-посадочной полосе является неполной и не может быть "
+"обработана."
+
 msgid "ErrorCode.InvalidMessage"
 msgstr "Введенное сообщение неверное."
 
 msgid "Flag.AMD"
 msgstr "Измененный TAF"
 
 msgid "Flag.AUTO"
```

### Comparing `metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/ru-RU/LC_MESSAGES/messages.po` & `metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/ru-RU/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 msgid ""
 msgstr ""
 "MIME-Version: 1.0"
 "Content-Type: text/plain; charset=UTF-8"
 "Content-Transfer-Encoding: 8bit"
 "X-Generator: prop2po"
 "Project-Id-Version: metar_taf_parser"
-"Language: ru_RU"
+"Language: ru-RU"
 #:
 msgid "CloudQuantity.BKN"
 msgstr "разорванная"
 
 #:
 msgid "CloudQuantity.FEW"
 msgstr "незначительная"
@@ -255,14 +255,18 @@
 msgstr "Аэропорт не найден для этого сообщения."
 
 #:
 msgid "ErrorCode.InvalidMessage"
 msgstr "Введенное сообщение неверное."
 
 #:
+msgid "ErrorCode.IncompleteRunwayInformation"
+msgstr "Информация о взлетно-посадочной полосе является неполной и не может быть обработана."
+
+#:
 msgid "Flag.AMD"
 msgstr "Измененный TAF"
 
 #:
 msgid "Flag.AUTO"
 msgstr "автоматический МЕТАР"
```

### Comparing `metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/tr/LC_MESSAGES/messages.mo` & `metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/tr/LC_MESSAGES/messages.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -4,15 +4,15 @@
 "PO-Revision-Date: \n"
 "Last-Translator: \n"
 "Language-Team: \n"
 "Language: tr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"X-Generator: Poedit 3.2.2\n"
+"X-Generator: Poedit 3.4.2\n"
 
 msgid "CloudQuantity.BKN"
 msgstr "parçalı çok bulutlu"
 
 msgid "CloudQuantity.FEW"
 msgstr "az bulutlu"
 
@@ -165,32 +165,14 @@
 
 msgid "DepositThickness.98"
 msgstr "40 cm veya daha fazla"
 
 msgid "DepositThickness.99"
 msgstr "kullanılmaz"
 
-msgid "DepositThickness.THICKNESS_10"
-msgstr "10 cm"
-
-msgid "DepositThickness.THICKNESS_15"
-msgstr "15 cm"
-
-msgid "DepositThickness.THICKNESS_20"
-msgstr "20 cm"
-
-msgid "DepositThickness.THICKNESS_25"
-msgstr "25 cm"
-
-msgid "DepositThickness.THICKNESS_30"
-msgstr "30 cm"
-
-msgid "DepositThickness.THICKNESS_35"
-msgstr "35 cm"
-
 msgid "DepositType.CLEAR_DRY"
 msgstr "açık ve kuru"
 
 msgid "DepositType.COMPACTED_SNOW"
 msgstr "yoğun veya sıkışmış kar"
 
 msgid "DepositType.DAMP"
```

### Comparing `metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/tr/LC_MESSAGES/messages.po` & `metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/tr/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 msgid ""
 msgstr ""
 "MIME-Version: 1.0"
 "Content-Type: text/plain; charset=UTF-8"
 "Content-Transfer-Encoding: 8bit"
 "X-Generator: prop2po"
 "Project-Id-Version: metar_taf_parser"
-"Language: tr_TR"
+"Language: tr"
 #:
 msgid "CloudQuantity.BKN"
 msgstr "parçalı çok bulutlu"
 
 #:
 msgid "CloudQuantity.FEW"
 msgstr "az bulutlu"
@@ -127,38 +127,14 @@
 msgstr "rapor edilmedi"
 
 #:
 msgid "DepositThickness.00"
 msgstr "1 mm'den daha az"
 
 #:
-msgid "DepositThickness.THICKNESS_10"
-msgstr "10 cm"
-
-#:
-msgid "DepositThickness.THICKNESS_15"
-msgstr "15 cm"
-
-#:
-msgid "DepositThickness.THICKNESS_20"
-msgstr "20 cm"
-
-#:
-msgid "DepositThickness.THICKNESS_25"
-msgstr "25 cm"
-
-#:
-msgid "DepositThickness.THICKNESS_30"
-msgstr "30 cm"
-
-#:
-msgid "DepositThickness.THICKNESS_35"
-msgstr "35 cm"
-
-#:
 msgid "DepositThickness.98"
 msgstr "40 cm veya daha fazla"
 
 #:
 msgid "DepositThickness.99"
 msgstr "kullanılmaz"
```

### Comparing `metar-taf-parser-mivek-1.8.2/metar_taf_parser/locale/zh-CN/LC_MESSAGES/messages.po` & `metar_taf_parser_mivek-1.9.0/metar_taf_parser/locale/zh-CN/LC_MESSAGES/messages.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 msgid ""
 msgstr ""
 "MIME-Version: 1.0"
 "Content-Type: text/plain; charset=UTF-8"
 "Content-Transfer-Encoding: 8bit"
 "X-Generator: prop2po"
 "Project-Id-Version: metar_taf_parser"
-"Language: zh_CN"
+"Language: zn-CN"
 #:
 msgid "CloudQuantity.BKN"
 msgstr "5-7分云"
 
 #:
 msgid "CloudQuantity.FEW"
 msgstr "少云"
@@ -87,26 +87,30 @@
 msgstr "中差"
 
 #:
 msgid "DepositBrakingCapacity.93"
 msgstr "中"
 
 #:
-msgid "DepositBrakingCapacity.MEDIUM_GOOD"
+msgid "DepositBrakingCapacity.94"
 msgstr "良好"
 
 #:
 msgid "DepositBrakingCapacity.95"
 msgstr "好"
 
 #:
 msgid "DepositBrakingCapacity.99"
 msgstr "数字不可靠"
 
 #:
+msgid "DepositBrakingCapacity.default"
+msgstr "摩擦系数为 {0}"
+
+#:
 msgid "DepositCoverage.NOT_REPORTED"
 msgstr "未报告"
 
 #:
 msgid "DepositCoverage.LESS_10"
 msgstr "低于10%"
 
@@ -127,46 +131,50 @@
 msgstr "未报告"
 
 #:
 msgid "DepositThickness.00"
 msgstr "小于 1 毫米"
 
 #:
-msgid "DepositThickness.THICKNESS_10"
+msgid "DepositThickness.92"
 msgstr "10 厘米"
 
 #:
-msgid "DepositThickness.THICKNESS_15"
+msgid "DepositThickness.93"
 msgstr "15 厘米"
 
 #:
-msgid "DepositThickness.THICKNESS_20"
+msgid "DepositThickness.94"
 msgstr "20 厘米"
 
 #:
-msgid "DepositThickness.THICKNESS_25"
+msgid "DepositThickness.95"
 msgstr "25 厘米"
 
 #:
-msgid "DepositThickness.THICKNESS_30"
+msgid "DepositThickness.96"
 msgstr "30 厘米"
 
 #:
-msgid "DepositThickness.THICKNESS_35"
+msgid "DepositThickness.97"
 msgstr "35 厘米"
 
 #:
 msgid "DepositThickness.98"
 msgstr "40厘米或以上"
 
 #:
 msgid "DepositThickness.99"
 msgstr "已关闭"
 
 #:
+msgid "DepositThickness.default"
+msgstr "{0} 毫米"
+
+#:
 msgid "DepositType.NOT_REPORTED"
 msgstr "未报告"
 
 #:
 msgid "DepositType.CLEAR_DRY"
 msgstr "干净"
 
@@ -247,14 +255,50 @@
 msgstr "找不到此消息的机场。"
 
 #:
 msgid "ErrorCode.InvalidMessage"
 msgstr "输入的消息无效。"
 
 #:
+msgid "Flag.AMD"
+msgstr "修正后的TAF"
+
+#:
+msgid "Flag.AUTO"
+msgstr "自动生成的METAR"
+
+#:
+msgid "Flag.CNL"
+msgstr "已取消的TAF"
+
+#:
+msgid "Flag.COR"
+msgstr "已更正的METAR/TAF"
+
+#:
+msgid "Flag.NIL"
+msgstr "暂无数据"
+
+#:
+msgid "IcingIntensity.0"
+msgstr "微量结冰"
+
+#:
+msgid "IcingIntensity.1"
+msgstr "轻度混合结冰"
+
+#:
+msgid "IcingIntensity.2"
+msgstr "云中轻度霜冻结冰"
+
+#:
+msgid "IcingIntensity.7"
+msgstr "重度混合结冰"
+
+#:
 msgid "Indicator.M"
 msgstr "小于"
 
 #:
 msgid "Indicator.P"
 msgstr "大于"
 
@@ -495,14 +539,26 @@
 msgstr "下一个"
 
 #:
 msgid "Remark.PeakWind"
 msgstr "在 {2}:{3} 有位于 {0} 度，风速 {1} 节的峰值风"
 
 #:
+msgid "Remark.PRESFR"
+msgstr "气压骤降"
+
+#:
+msgid "Remark.PRESRR"
+msgstr "气压骤升"
+
+#:
+msgid "Remark.Sea.Level.Pressure"
+msgstr "海平面气压{0} 百帕"
+
+#:
 msgid "Remark.TORNADO"
 msgstr "龙卷风"
 
 #:
 msgid "Remark.VIRGA"
 msgstr "幡状云"
 
@@ -695,14 +751,18 @@
 msgstr "当月的结束日"
 
 #:
 msgid "ToString.end.hour.day"
 msgstr "当日的结束小时"
 
 #:
+msgid "ToString.flags"
+msgstr "旗子"
+
+#:
 msgid "ToString.height.feet"
 msgstr "高度（英尺）"
 
 #:
 msgid "ToString.height.meter"
 msgstr "高度（米）"
 
@@ -834,7 +894,23 @@
 msgid "ToString.wind.speed"
 msgstr "速度"
 
 #:
 msgid "ToString.wind.unit"
 msgstr "单位"
 
+#:
+msgid "TurbulenceIntensity.0"
+msgstr "无"
+
+#:
+msgid "TurbulenceIntensity.1"
+msgstr "轻度乱流"
+
+#:
+msgid "TurbulenceIntensity.8"
+msgstr "云中偶发重度颠簸"
+
+#:
+msgid "TurbulenceIntensity.X"
+msgstr "极端乱流"
+
```

### Comparing `metar-taf-parser-mivek-1.8.2/metar_taf_parser/model/enum.py` & `metar_taf_parser_mivek-1.9.0/metar_taf_parser/model/enum.py`

 * *Files identical despite different names*

### Comparing `metar-taf-parser-mivek-1.8.2/metar_taf_parser/model/model.py` & `metar_taf_parser_mivek-1.9.0/metar_taf_parser/model/model.py`

 * *Files identical despite different names*

### Comparing `metar-taf-parser-mivek-1.8.2/metar_taf_parser/parser/parser.py` & `metar_taf_parser_mivek-1.9.0/metar_taf_parser/parser/parser.py`

 * *Files identical despite different names*

### Comparing `metar-taf-parser-mivek-1.8.2/metar_taf_parser_mivek.egg-info/PKG-INFO` & `metar_taf_parser_mivek-1.9.0/metar_taf_parser_mivek.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metar-taf-parser-mivek
-Version: 1.8.2
+Version: 1.9.0
 Summary: Python project parsing metar and taf message
 Home-page: https://github.com/mivek/python-metar-taf-parser
 Author: Jean-Kevin KPADEY
 Author-email: jeankevin.kpadey@gmail.com
 Project-URL: Bug Tracker, https://github.com/mivek/python-metar-taf-parser/issues
 Keywords: metar,taf,parser,icao,airport
 Classifier: Programming Language :: Python :: 3
```

### Comparing `metar-taf-parser-mivek-1.8.2/metar_taf_parser_mivek.egg-info/SOURCES.txt` & `metar_taf_parser_mivek-1.9.0/metar_taf_parser_mivek.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metar-taf-parser-mivek-1.8.2/setup.cfg` & `metar_taf_parser_mivek-1.9.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = metar-taf-parser-mivek
-version = 1.8.2
+version = 1.9.0
 author = Jean-Kevin KPADEY
 author_email = jeankevin.kpadey@gmail.com
 description = Python project parsing metar and taf message
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mivek/python-metar-taf-parser
 project_urls =
```

