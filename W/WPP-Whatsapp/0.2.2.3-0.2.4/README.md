# Comparing `tmp/wpp_whatsapp-0.2.2.3.tar.gz` & `tmp/wpp_whatsapp-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wpp_whatsapp-0.2.2.3.tar", last modified: Sun May  5 18:41:01 2024, max compression
+gzip compressed data, was "wpp_whatsapp-0.2.4.tar", last modified: Mon May 20 16:59:41 2024, max compression
```

## Comparing `wpp_whatsapp-0.2.2.3.tar` & `wpp_whatsapp-0.2.4.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:41:01.179731 wpp_whatsapp-0.2.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-05-05 18:41:01.179731 wpp_whatsapp-0.2.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:41:01.175731 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:41:01.175731 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/
--rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/Whatsapp.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:41:01.175731 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/helpers/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/helpers/download_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/helpers/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/helpers/jsFunction.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/helpers/scrap-img.py
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/helpers/wa_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:41:01.179731 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/BusinessLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/CatalogLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7487 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/ControlsLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/GroupLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)    31817 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/HostLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/LabelsLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12529 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/ListenerLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/ProfileLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13361 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/RetrieverLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)    19632 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/SenderLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/StatusLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/UILayer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:41:01.179731 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/model/status_find.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:41:01.179731 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/controllers/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/controllers/browser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/controllers/init_multi.py
--rw-r--r--   0 runner    (1001) docker     (127)    10304 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/controllers/initializer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:41:01.179731 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/js_lib/
--rw-r--r--   0 runner    (1001) docker     (127)    89768 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/js_lib/wapi.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:41:01.179731 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/utils/ffmpeg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:41:01.179731 wpp_whatsapp-0.2.2.3/WPP_Whatsapp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-05-05 18:41:01.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-05 18:41:01.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 18:41:01.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-05 18:41:01.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-05 18:41:01.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 18:41:01.179731 wpp_whatsapp-0.2.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:41:01.179731 wpp_whatsapp-0.2.2.3/test/
--rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/test/test_hiden.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/test/test_setinterval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:59:41.580255 wpp_whatsapp-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-20 16:59:37.000000 wpp_whatsapp-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-05-20 16:59:41.576255 wpp_whatsapp-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-20 16:59:37.000000 wpp_whatsapp-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:59:41.572255 wpp_whatsapp-0.2.4/WPP_Whatsapp/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-20 16:59:37.000000 wpp_whatsapp-0.2.4/WPP_Whatsapp/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-20 16:59:37.000000 wpp_whatsapp-0.2.4/WPP_Whatsapp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:59:41.572255 wpp_whatsapp-0.2.4/WPP_Whatsapp/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-05-20 16:59:37.000000 wpp_whatsapp-0.2.4/WPP_Whatsapp/api/Whatsapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 16:59:37.000000 wpp_whatsapp-0.2.4/WPP_Whatsapp/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-20 16:59:37.000000 wpp_whatsapp-0.2.4/WPP_Whatsapp/api/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:59:41.572255 wpp_whatsapp-0.2.4/WPP_Whatsapp/api/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 16:59:37.000000 wpp_whatsapp-0.2.4/WPP_Whatsapp/api/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-20 16:59:37.000000 wpp_whatsapp-0.2.4/WPP_Whatsapp/api/helpers/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-20 16:59:37.000000 wpp_whatsapp-0.2.4/WPP_Whatsapp/api/helpers/download_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-20 16:59:37.000000 wpp_whatsapp-0.2.4/WPP_Whatsapp/api/helpers/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-20 16:59:37.000000 wpp_whatsapp-0.2.4/WPP_Whatsapp/api/helpers/jsFunction.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 16:59:37.000000 wpp_whatsapp-0.2.4/WPP_Whatsapp/api/helpers/scrap-img.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-20 16:59:37.000000 wpp_whatsapp-0.2.4/WPP_Whatsapp/api/helpers/wa_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:59:41.576255 wpp_whatsapp-0.2.4/WPP_Whatsapp/api/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-20 16:59:37.000000 wpp_whatsapp-0.2.4/WPP_Whatsapp/api/layers/BusinessLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-20 16:59:37.000000 wpp_whatsapp-0.2.4/WPP_Whatsapp/api/layers/CatalogLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7487 2024-05-20 16:59:37.000000 wpp_whatsapp-0.2.4/WPP_Whatsapp/api/layers/ControlsLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-05-20 16:59:37.000000 wpp_whatsapp-0.2.4/WPP_Whatsapp/api/layers/GroupLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31817 2024-05-20 16:59:37.000000 wpp_whatsapp-0.2.4/WPP_Whatsapp/api/layers/HostLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-20 16:59:37.000000 wpp_whatsapp-0.2.4/WPP_Whatsapp/api/layers/LabelsLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12529 2024-05-20 16:59:37.000000 wpp_whatsapp-0.2.4/WPP_Whatsapp/api/layers/ListenerLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-05-20 16:59:37.000000 wpp_whatsapp-0.2.4/WPP_Whatsapp/api/layers/ProfileLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13361 2024-05-20 16:59:37.000000 wpp_whatsapp-0.2.4/WPP_Whatsapp/api/layers/RetrieverLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19632 2024-05-20 16:59:37.000000 wpp_whatsapp-0.2.4/WPP_Whatsapp/api/layers/SenderLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-05-20 16:59:37.000000 wpp_whatsapp-0.2.4/WPP_Whatsapp/api/layers/StatusLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-20 16:59:37.000000 wpp_whatsapp-0.2.4/WPP_Whatsapp/api/layers/UILayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 16:59:37.000000 wpp_whatsapp-0.2.4/WPP_Whatsapp/api/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:59:41.576255 wpp_whatsapp-0.2.4/WPP_Whatsapp/api/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 16:59:37.000000 wpp_whatsapp-0.2.4/WPP_Whatsapp/api/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-20 16:59:37.000000 wpp_whatsapp-0.2.4/WPP_Whatsapp/api/model/status_find.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:59:41.576255 wpp_whatsapp-0.2.4/WPP_Whatsapp/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 16:59:37.000000 wpp_whatsapp-0.2.4/WPP_Whatsapp/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 16:59:37.000000 wpp_whatsapp-0.2.4/WPP_Whatsapp/controllers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-20 16:59:37.000000 wpp_whatsapp-0.2.4/WPP_Whatsapp/controllers/browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-05-20 16:59:37.000000 wpp_whatsapp-0.2.4/WPP_Whatsapp/controllers/init_multi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10304 2024-05-20 16:59:37.000000 wpp_whatsapp-0.2.4/WPP_Whatsapp/controllers/initializer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:59:41.576255 wpp_whatsapp-0.2.4/WPP_Whatsapp/js_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)    89768 2024-05-20 16:59:37.000000 wpp_whatsapp-0.2.4/WPP_Whatsapp/js_lib/wapi.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:59:41.576255 wpp_whatsapp-0.2.4/WPP_Whatsapp/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 16:59:37.000000 wpp_whatsapp-0.2.4/WPP_Whatsapp/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-20 16:59:37.000000 wpp_whatsapp-0.2.4/WPP_Whatsapp/utils/ffmpeg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:59:41.576255 wpp_whatsapp-0.2.4/WPP_Whatsapp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-05-20 16:59:41.000000 wpp_whatsapp-0.2.4/WPP_Whatsapp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-20 16:59:41.000000 wpp_whatsapp-0.2.4/WPP_Whatsapp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 16:59:41.000000 wpp_whatsapp-0.2.4/WPP_Whatsapp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-20 16:59:41.000000 wpp_whatsapp-0.2.4/WPP_Whatsapp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-20 16:59:41.000000 wpp_whatsapp-0.2.4/WPP_Whatsapp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 16:59:41.580255 wpp_whatsapp-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-20 16:59:37.000000 wpp_whatsapp-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:59:41.576255 wpp_whatsapp-0.2.4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-05-20 16:59:37.000000 wpp_whatsapp-0.2.4/test/test_hiden.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-20 16:59:37.000000 wpp_whatsapp-0.2.4/test/test_setinterval.py
```

### Comparing `wpp_whatsapp-0.2.2.3/LICENSE` & `wpp_whatsapp-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.3/PKG-INFO` & `wpp_whatsapp-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WPP_Whatsapp
-Version: 0.2.2.3
+Version: 0.2.4
 Summary: WPP_Whatsapp aim of exporting functions from WhatsApp Web to the python, which can be used to support the creation of any interaction, such as customer service, media sending, intelligence recognition based on phrases artificial and many other things, use your imagination
 Home-page: https://github.com/3mora2/WPP_Whatsapp
 Author: Ammar Alkotb
 Author-email: ammar.alkotb@gmail.com
 License: MIT License
 Project-URL: Bug Report, https://github.com/3mora2/WPP_Whatsapp/issues/new
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `wpp_whatsapp-0.2.2.3/README.md` & `wpp_whatsapp-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/Whatsapp.py` & `wpp_whatsapp-0.2.4/WPP_Whatsapp/api/Whatsapp.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,18 +110,18 @@
 
     def getMessages(self, chatId, params=None, timeout=120):
         """
         :param chatId:
         :param params: (count, id, direction)
         :return:
         """
-        return self.ThreadsafeBrowser.run_threadsafe(self.getMessages_, chatId, params, timeout_=timeout)
+        return self.ThreadsafeBrowser.run_threadsafe(self.getMessages_( chatId, params), timeout_=timeout)
 
-    def rejectCall(self, callId, timeout=120):
-        return self.ThreadsafeBrowser.run_threadsafe(self.rejectCall_, callId, timeout_=timeout)
+    def rejectCall(self, callId="", timeout=120):
+        return self.ThreadsafeBrowser.run_threadsafe(self.rejectCall_( callId), timeout_=timeout)
 
     #############################
     async def useHere_(self):
         return await self.ThreadsafeBrowser.page_evaluate("() => WAPI.takeOver()", page=self.page)
 
     async def logout_(self):
         return await self.ThreadsafeBrowser.page_evaluate("() => WPP.conn.logout()", page=self.page)
@@ -137,10 +137,10 @@
         """
         if not params:
             params = {}
         chatId = self.valid_chatId(chatId)
         return await self.ThreadsafeBrowser.page_evaluate("({ chatId, params }) => WAPI.getMessages(chatId, params)",
                                                           {"chatId": chatId, "params": params}, page=self.page)
 
-    async def rejectCall_(self, callId):
+    async def rejectCall_(self, callId=""):
         return await self.ThreadsafeBrowser.page_evaluate(
-            "({callId}) => WPP.call.rejectCall(callId)", callId, page=self.page)
+            "(callId) => WPP.call.rejectCall(callId)", callId, page=self.page)
```

### Comparing `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/const.py` & `wpp_whatsapp-0.2.4/WPP_Whatsapp/api/const.py`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/helpers/decorators.py` & `wpp_whatsapp-0.2.4/WPP_Whatsapp/api/helpers/decorators.py`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/helpers/download_file.py` & `wpp_whatsapp-0.2.4/WPP_Whatsapp/api/helpers/download_file.py`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/helpers/jsFunction.py` & `wpp_whatsapp-0.2.4/WPP_Whatsapp/api/helpers/jsFunction.py`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/helpers/wa_version.py` & `wpp_whatsapp-0.2.4/WPP_Whatsapp/api/helpers/wa_version.py`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/CatalogLayer.py` & `wpp_whatsapp-0.2.4/WPP_Whatsapp/api/layers/CatalogLayer.py`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/ControlsLayer.py` & `wpp_whatsapp-0.2.4/WPP_Whatsapp/api/layers/ControlsLayer.py`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/GroupLayer.py` & `wpp_whatsapp-0.2.4/WPP_Whatsapp/api/layers/GroupLayer.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,16 +43,16 @@
     async def getGroupMembersIds_(self, groupId):
         groupId = self.valid_chatId(groupId)
         return await self.ThreadsafeBrowser.page_evaluate("""(groupId) => Promise.resolve(WPP.group.getParticipants(groupId)).then(
           (participants) => participants.map((p) => p.id))""", groupId, page=self.page)
 
     async def getGroupMembers_(self, groupId):
         groupId = self.valid_chatId(groupId)
-        membersIds = self.getGroupMembersIds(groupId)
-        return [self.getContact(memberId.get("_serialized")) for memberId in membersIds]
+        membersIds = await self.getGroupMembersIds_(groupId)
+        return [await self.getContact_(memberId.get("_serialized")) for memberId in membersIds]
 
     async def getGroupInviteLink_(self, chatId):
         chatId = self.valid_chatId(chatId)
         code = await self.ThreadsafeBrowser.page_evaluate("(chatId) => WPP.group.getInviteCode(chatId)", chatId, page=self.page)
 
         return f"https://chat.whatsapp.com/{code}" if code else None
```

### Comparing `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/HostLayer.py` & `wpp_whatsapp-0.2.4/WPP_Whatsapp/api/layers/HostLayer.py`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/LabelsLayer.py` & `wpp_whatsapp-0.2.4/WPP_Whatsapp/api/layers/LabelsLayer.py`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/ListenerLayer.py` & `wpp_whatsapp-0.2.4/WPP_Whatsapp/api/layers/ListenerLayer.py`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/ProfileLayer.py` & `wpp_whatsapp-0.2.4/WPP_Whatsapp/api/layers/ProfileLayer.py`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/RetrieverLayer.py` & `wpp_whatsapp-0.2.4/WPP_Whatsapp/api/layers/RetrieverLayer.py`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/SenderLayer.py` & `wpp_whatsapp-0.2.4/WPP_Whatsapp/api/layers/SenderLayer.py`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/StatusLayer.py` & `wpp_whatsapp-0.2.4/WPP_Whatsapp/api/layers/StatusLayer.py`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/UILayer.py` & `wpp_whatsapp-0.2.4/WPP_Whatsapp/api/layers/UILayer.py`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/model/status_find.py` & `wpp_whatsapp-0.2.4/WPP_Whatsapp/api/model/status_find.py`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/controllers/browser.py` & `wpp_whatsapp-0.2.4/WPP_Whatsapp/controllers/browser.py`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/controllers/init_multi.py` & `wpp_whatsapp-0.2.4/WPP_Whatsapp/controllers/init_multi.py`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/controllers/initializer.py` & `wpp_whatsapp-0.2.4/WPP_Whatsapp/controllers/initializer.py`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/js_lib/wapi.js` & `wpp_whatsapp-0.2.4/WPP_Whatsapp/js_lib/wapi.js`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/utils/ffmpeg.py` & `wpp_whatsapp-0.2.4/WPP_Whatsapp/utils/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.3/WPP_Whatsapp.egg-info/PKG-INFO` & `wpp_whatsapp-0.2.4/WPP_Whatsapp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WPP_Whatsapp
-Version: 0.2.2.3
+Version: 0.2.4
 Summary: WPP_Whatsapp aim of exporting functions from WhatsApp Web to the python, which can be used to support the creation of any interaction, such as customer service, media sending, intelligence recognition based on phrases artificial and many other things, use your imagination
 Home-page: https://github.com/3mora2/WPP_Whatsapp
 Author: Ammar Alkotb
 Author-email: ammar.alkotb@gmail.com
 License: MIT License
 Project-URL: Bug Report, https://github.com/3mora2/WPP_Whatsapp/issues/new
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `wpp_whatsapp-0.2.2.3/WPP_Whatsapp.egg-info/SOURCES.txt` & `wpp_whatsapp-0.2.4/WPP_Whatsapp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.3/setup.py` & `wpp_whatsapp-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 long_description = open("README.md", encoding="utf-8").read()
 description = ("WPP_Whatsapp aim of exporting functions from WhatsApp Web to the python, which can be used to support "
                "the creation of any interaction, such as customer service, media sending, intelligence recognition "
                "based on phrases artificial and many other things, use your imagination")
 
-version = "0.2.2.3"
+version = "0.2.4"
 
 setup(
     name="WPP_Whatsapp",
     version=version,
     license="MIT License",
     author="Ammar Alkotb",
     author_email="ammar.alkotb@gmail.com",
```

### Comparing `wpp_whatsapp-0.2.2.3/test/test_hiden.py` & `wpp_whatsapp-0.2.4/test/test_hiden.py`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.3/test/test_setinterval.py` & `wpp_whatsapp-0.2.4/test/test_setinterval.py`

 * *Files identical despite different names*

