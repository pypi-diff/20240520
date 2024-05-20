# Comparing `tmp/psl-2024.5.20.tar.gz` & `tmp/psl-2024.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psl-2024.5.20.tar", last modified: Mon May 20 13:05:22 2024, max compression
+gzip compressed data, was "psl-2024.5.6.tar", last modified: Mon May  6 13:04:35 2024, max compression
```

## Comparing `psl-2024.5.20.tar` & `psl-2024.5.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:05:22.377212 psl-2024.5.20/
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-05-20 13:04:55.000000 psl-2024.5.20/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-20 13:04:55.000000 psl-2024.5.20/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-20 13:05:22.377212 psl-2024.5.20/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-20 13:04:55.000000 psl-2024.5.20/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:05:22.377212 psl-2024.5.20/psl/
--rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-05-20 13:05:01.000000 psl-2024.5.20/psl/__init__.py
--rw-------   0 runner    (1001) docker     (127)   133761 2024-05-20 13:05:01.000000 psl-2024.5.20/psl/psl.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 13:04:55.000000 psl-2024.5.20/psl/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:05:22.377212 psl-2024.5.20/psl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-20 13:05:22.000000 psl-2024.5.20/psl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-20 13:05:22.000000 psl-2024.5.20/psl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 13:05:22.000000 psl-2024.5.20/psl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 13:05:12.000000 psl-2024.5.20/psl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-20 13:05:22.000000 psl-2024.5.20/psl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 13:05:22.377212 psl-2024.5.20/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-20 13:04:55.000000 psl-2024.5.20/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:04:35.715896 psl-2024.5.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-05-06 13:04:09.000000 psl-2024.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-06 13:04:09.000000 psl-2024.5.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-05-06 13:04:35.715896 psl-2024.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-06 13:04:09.000000 psl-2024.5.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:04:35.715896 psl-2024.5.6/psl/
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-05-06 13:04:15.000000 psl-2024.5.6/psl/__init__.py
+-rw-------   0 runner    (1001) docker     (127)   133574 2024-05-06 13:04:15.000000 psl-2024.5.6/psl/psl.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:04:09.000000 psl-2024.5.6/psl/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:04:35.715896 psl-2024.5.6/psl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-05-06 13:04:35.000000 psl-2024.5.6/psl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-06 13:04:35.000000 psl-2024.5.6/psl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 13:04:35.000000 psl-2024.5.6/psl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 13:04:25.000000 psl-2024.5.6/psl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-06 13:04:35.000000 psl-2024.5.6/psl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 13:04:35.715896 psl-2024.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-06 13:04:09.000000 psl-2024.5.6/setup.py
```

### Comparing `psl-2024.5.20/LICENSE` & `psl-2024.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `psl-2024.5.20/PKG-INFO` & `psl-2024.5.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psl
-Version: 2024.5.20
+Version: 2024.5.6
 Summary: Mozilla Public Suffix list as a Python package and updated daily
 Home-page: https://github.com/sethmlarson/psl
 Author: Seth Michael Larson
 Author-email: sethmichaellarson@gmail.com
 License: MPL-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `psl-2024.5.20/README.md` & `psl-2024.5.6/README.md`

 * *Files identical despite different names*

### Comparing `psl-2024.5.20/psl/__init__.py` & `psl-2024.5.6/psl/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import functools
 import pathlib
 import typing
 
-__version__ = "2024.5.20"
-__checksum__ = "c982c3c6a888911c0cf3e910c39abd59e3c249ac"
+__version__ = "2024.5.6"
+__checksum__ = "7c0c6cfa0fe6e11d438448a2b8c76092ae19abfa"
 __all__ = ["PUBLIC_SUFFIX_URL", "domain_suffixes", "Suffixes", "domain_can_set_cookie"]
 
 
 PUBLIC_SUFFIX_URL = "https://publicsuffix.org/list/public_suffix_list.dat"
 _PUBLIC_SUFFIX_PATH = pathlib.Path(__file__).parent / "psl.txt"
```

### Comparing `psl-2024.5.20/psl/psl.txt` & `psl-2024.5.6/psl/psl.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7714,18 +7714,15 @@
 radio.am
 radio.fm
 c.la
 certmgr.org
 cx.ua
 discourse.group
 discourse.team
-cleverapps.cc
-*.services.clever-cloud.com
 cleverapps.io
-cleverapps.tech
 clerk.app
 clerkstage.app
 *.lcl.dev
 *.lclstage.dev
 *.stg.dev
 *.stgstage.dev
 clickrising.net
@@ -8259,16 +8256,14 @@
 eu-2.evennode.com
 eu-3.evennode.com
 eu-4.evennode.com
 us-1.evennode.com
 us-2.evennode.com
 us-3.evennode.com
 us-4.evennode.com
-expo.app
-staging.expo.app
 twmail.cc
 twmail.net
 twmail.org
 mymailer.com.tw
 url.tw
 onfabrica.com
 ru.net
@@ -8574,15 +8569,14 @@
 heteml.net
 graphic.design
 cloudapps.digital
 london.cloudapps.digital
 pymnt.uk
 ro.im
 goip.de
-*.hosted.app
 *.run.app
 web.app
 *.0emm.com
 appspot.com
 *.r.appspot.com
 codespot.com
 googleapis.com
@@ -9049,15 +9043,14 @@
 noop.app
 *.northflank.app
 *.build.run
 *.code.run
 *.database.run
 *.migration.run
 noticeable.news
-notion.site
 dnsking.ch
 mypi.co
 n4t.co
 001www.com
 ddnslive.com
 myiphost.com
 forumz.info
@@ -9166,15 +9159,14 @@
 sytes.net
 webhop.me
 zapto.org
 stage.nodeart.io
 pcloud.host
 nyc.mn
 prvcy.page
-observablehq.cloud
 static.observableusercontent.com
 cya.gg
 omg.lol
 cloudycluster.net
 omniwe.site
 123hjemmeside.dk
 123hjemmeside.no
@@ -9455,15 +9447,14 @@
 sellfy.store
 senseering.net
 minisite.ms
 magnet.page
 biz.ua
 co.ua
 pp.ua
-sheezy.games
 shiftcrypto.dev
 shiftcrypto.io
 shiftedit.io
 myshopblocks.com
 myshopify.com
 shopitsite.com
 shopware.store
@@ -9672,16 +9663,14 @@
 org.yt
 virtualuser.de
 virtual-user.de
 upli.io
 urown.cloud
 dnsupdate.info
 lib.de.us
-express.val.run
-web.val.run
 2038.io
 vercel.app
 vercel.dev
 now.sh
 router.management
 v-info.info
 voorloper.cloud
@@ -9696,15 +9685,14 @@
 bookonline.app
 hotelwithflight.com
 *.wadl.top
 wedeploy.io
 wedeploy.me
 wedeploy.sh
 remotewd.com
-box.ca
 pages.wiardweb.com
 wmflabs.org
 toolforge.org
 wmcloud.org
 panel.gg
 daemon.panel.gg
 messwithdns.com
@@ -9744,13 +9732,12 @@
 ybo.trade
 ynh.fr
 nohost.me
 noho.st
 za.net
 za.org
 zap.cloud
-zeabur.app
 bss.design
 basicserver.io
 virtualserver.io
 enterprisecloud.nu
 // ===END PRIVATE DOMAINS===
```

### Comparing `psl-2024.5.20/psl.egg-info/PKG-INFO` & `psl-2024.5.6/psl.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psl
-Version: 2024.5.20
+Version: 2024.5.6
 Summary: Mozilla Public Suffix list as a Python package and updated daily
 Home-page: https://github.com/sethmlarson/psl
 Author: Seth Michael Larson
 Author-email: sethmichaellarson@gmail.com
 License: MPL-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `psl-2024.5.20/setup.py` & `psl-2024.5.6/setup.py`

 * *Files identical despite different names*

