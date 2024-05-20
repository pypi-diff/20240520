# Comparing `tmp/crypto_licensing-3.3.2.tar.gz` & `tmp/crypto_licensing-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto_licensing-3.3.2.tar", last modified: Sat Aug 12 21:09:57 2023, max compression
+gzip compressed data, was "crypto_licensing-4.0.0.tar", last modified: Sun May 19 23:54:58 2024, max compression
```

## Comparing `crypto_licensing-3.3.2.tar` & `crypto_licensing-4.0.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 perry      (501) staff       (20)        0 2023-08-12 21:09:57.117569 crypto_licensing-3.3.2/
--rw-rw-r--   0 perry      (501) staff       (20)    35147 2022-01-25 19:29:48.000000 crypto_licensing-3.3.2/COPYING
--rw-rw-r--   0 perry      (501) staff       (20)     1184 2023-02-05 15:25:14.000000 crypto_licensing-3.3.2/LICENSE
--rw-rw-r--   0 perry      (501) staff       (20)      138 2022-02-23 17:37:17.000000 crypto_licensing-3.3.2/MANIFEST.in
--rw-rw-r--   0 perry      (501) staff       (20)     1392 2023-08-12 21:09:57.116950 crypto_licensing-3.3.2/PKG-INFO
--rw-rw-r--   0 perry      (501) staff       (20)     4468 2023-02-05 15:25:14.000000 crypto_licensing-3.3.2/README.org
--rw-rw-r--   0 perry      (501) staff       (20)     7177 2023-02-05 15:25:14.000000 crypto_licensing-3.3.2/README.txt
-drwxrwxr-x   0 perry      (501) staff       (20)        0 2023-08-12 21:09:57.081644 crypto_licensing-3.3.2/crypto_licensing/
--rw-rw-r--   0 perry      (501) staff       (20)     1364 2023-07-23 20:36:37.000000 crypto_licensing-3.3.2/crypto_licensing/__init__.py
--rw-rw-r--   0 perry      (501) staff       (20)     1365 2023-02-14 14:41:09.000000 crypto_licensing-3.3.2/crypto_licensing/__main__.py
--rw-rw-r--   0 perry      (501) staff       (20)    10632 2023-02-16 18:04:11.000000 crypto_licensing-3.3.2/crypto_licensing/cli.py
--rw-rw-r--   0 perry      (501) staff       (20)     3993 2023-02-15 19:50:25.000000 crypto_licensing-3.3.2/crypto_licensing/cli_test.py
--rw-rw-r--   0 perry      (501) staff       (20)     5264 2023-02-05 15:25:14.000000 crypto_licensing-3.3.2/crypto_licensing/crypto_test.py
-drwxrwxr-x   0 perry      (501) staff       (20)        0 2023-08-12 21:09:57.082451 crypto_licensing-3.3.2/crypto_licensing/ed25519/
--rw-rw-r--   0 perry      (501) staff       (20)     1655 2023-02-14 14:07:01.000000 crypto_licensing-3.3.2/crypto_licensing/ed25519/__init__.py
--rw-rw-r--   0 perry      (501) staff       (20)     5033 2022-01-24 17:18:08.000000 crypto_licensing-3.3.2/crypto_licensing/ed25519_djb.py
-drwxrwxr-x   0 perry      (501) staff       (20)        0 2023-08-12 21:09:57.084385 crypto_licensing-3.3.2/crypto_licensing/ed25519ll_pyonly/
--rw-rw-r--   0 perry      (501) staff       (20)     2319 2023-02-05 15:25:14.000000 crypto_licensing-3.3.2/crypto_licensing/ed25519ll_pyonly/__init__.py
--rw-rw-r--   0 perry      (501) staff       (20)     6905 2022-01-19 19:14:43.000000 crypto_licensing-3.3.2/crypto_licensing/ed25519ll_pyonly/djbec.py
-drwxrwxr-x   0 perry      (501) staff       (20)        0 2023-08-12 21:09:57.104139 crypto_licensing-3.3.2/crypto_licensing/licensing/
--rw-rw-r--   0 perry      (501) staff       (20)     1606 2023-02-21 15:58:27.000000 crypto_licensing-3.3.2/crypto_licensing/licensing/__init__.py
--rw-rw-r--   0 perry      (501) staff       (20)     1196 2023-02-14 14:07:40.000000 crypto_licensing-3.3.2/crypto_licensing/licensing/__main__.py
--rw-rw-r--   0 perry      (501) staff       (20)     1942 2023-02-05 15:25:14.000000 crypto_licensing-3.3.2/crypto_licensing/licensing/bitquery_test.py
--rw-rw-r--   0 perry      (501) staff       (20)     2194 2023-02-14 14:08:13.000000 crypto_licensing-3.3.2/crypto_licensing/licensing/defaults.py
-drwxrwxr-x   0 perry      (501) staff       (20)        0 2023-08-12 21:09:57.108134 crypto_licensing-3.3.2/crypto_licensing/licensing/doh/
--rw-rw-r--   0 perry      (501) staff       (20)     4511 2023-08-12 20:38:18.000000 crypto_licensing-3.3.2/crypto_licensing/licensing/doh/__init__.py
--rw-rw-r--   0 perry      (501) staff       (20)     1362 2023-02-14 14:15:34.000000 crypto_licensing-3.3.2/crypto_licensing/licensing/doh/__main__.py
--rw-rw-r--   0 perry      (501) staff       (20)     2731 2023-02-14 14:16:10.000000 crypto_licensing-3.3.2/crypto_licensing/licensing/doh/cli.py
--rw-rw-r--   0 perry      (501) staff       (20)     3656 2023-08-12 20:37:42.000000 crypto_licensing-3.3.2/crypto_licensing/licensing/doh_test.py
--rw-rw-r--   0 perry      (501) staff       (20)    17971 2023-02-05 15:25:14.000000 crypto_licensing-3.3.2/crypto_licensing/licensing/grant_test.py
--rw-rw-r--   0 perry      (501) staff       (20)     7469 2023-02-05 15:25:14.000000 crypto_licensing-3.3.2/crypto_licensing/licensing/licensing_test.py
--rw-rw-r--   0 perry      (501) staff       (20)    96445 2023-02-14 14:08:47.000000 crypto_licensing-3.3.2/crypto_licensing/licensing/main.py
--rw-rw-r--   0 perry      (501) staff       (20)   155417 2023-07-22 14:39:37.000000 crypto_licensing-3.3.2/crypto_licensing/licensing/verification.py
--rw-rw-r--   0 perry      (501) staff       (20)    41145 2023-02-23 18:12:32.000000 crypto_licensing-3.3.2/crypto_licensing/licensing/verification_test.py
--rw-rw-r--   0 perry      (501) staff       (20)    43647 2023-08-12 21:01:50.000000 crypto_licensing-3.3.2/crypto_licensing/misc.py
--rw-rw-r--   0 perry      (501) staff       (20)     9528 2023-02-05 15:25:17.000000 crypto_licensing-3.3.2/crypto_licensing/misc_test.py
--rw-rw-r--   0 perry      (501) staff       (20)       88 2023-08-12 20:54:49.000000 crypto_licensing-3.3.2/crypto_licensing/version.py
-drwxrwxr-x   0 perry      (501) staff       (20)        0 2023-08-12 21:09:57.115821 crypto_licensing-3.3.2/crypto_licensing.egg-info/
--rw-rw-r--   0 perry      (501) staff       (20)     1392 2023-08-12 21:09:57.000000 crypto_licensing-3.3.2/crypto_licensing.egg-info/PKG-INFO
--rw-rw-r--   0 perry      (501) staff       (20)     1331 2023-08-12 21:09:57.000000 crypto_licensing-3.3.2/crypto_licensing.egg-info/SOURCES.txt
--rw-rw-r--   0 perry      (501) staff       (20)        1 2023-08-12 21:09:57.000000 crypto_licensing-3.3.2/crypto_licensing.egg-info/dependency_links.txt
--rw-rw-r--   0 perry      (501) staff       (20)       74 2023-08-12 21:09:57.000000 crypto_licensing-3.3.2/crypto_licensing.egg-info/entry_points.txt
--rw-rw-r--   0 perry      (501) staff       (20)      263 2023-08-12 21:09:57.000000 crypto_licensing-3.3.2/crypto_licensing.egg-info/requires.txt
--rw-rw-r--   0 perry      (501) staff       (20)      134 2023-08-12 21:09:57.000000 crypto_licensing-3.3.2/crypto_licensing.egg-info/top_level.txt
--rw-rw-r--   0 perry      (501) staff       (20)       48 2023-02-05 15:25:14.000000 crypto_licensing-3.3.2/requirements-dev.txt
--rw-rw-r--   0 perry      (501) staff       (20)       21 2023-02-05 15:25:14.000000 crypto_licensing-3.3.2/requirements-tests.txt
--rw-rw-r--   0 perry      (501) staff       (20)      312 2023-02-05 15:25:14.000000 crypto_licensing-3.3.2/requirements.txt
--rw-rw-r--   0 perry      (501) staff       (20)       38 2023-08-12 21:09:57.117723 crypto_licensing-3.3.2/setup.cfg
--rw-rw-r--   0 perry      (501) staff       (20)     3157 2023-02-21 16:32:39.000000 crypto_licensing-3.3.2/setup.py
+drwxr-xr-x   0 perry      (501) staff       (20)        0 2024-05-19 23:54:58.939116 crypto_licensing-4.0.0/
+-rw-rw-r--   0 perry      (501) staff       (20)    35147 2022-01-25 19:29:48.000000 crypto_licensing-4.0.0/COPYING
+-rw-rw-r--   0 perry      (501) staff       (20)     1184 2023-02-05 15:25:14.000000 crypto_licensing-4.0.0/LICENSE
+-rw-rw-r--   0 perry      (501) staff       (20)      138 2022-02-23 17:37:17.000000 crypto_licensing-4.0.0/MANIFEST.in
+-rw-r--r--   0 perry      (501) staff       (20)     2085 2024-05-19 23:54:58.938398 crypto_licensing-4.0.0/PKG-INFO
+-rw-rw-r--   0 perry      (501) staff       (20)     4468 2023-02-05 15:25:14.000000 crypto_licensing-4.0.0/README.org
+-rw-rw-r--   0 perry      (501) staff       (20)     7177 2023-02-05 15:25:14.000000 crypto_licensing-4.0.0/README.txt
+drwxr-xr-x   0 perry      (501) staff       (20)        0 2024-05-19 23:54:58.922057 crypto_licensing-4.0.0/crypto_licensing/
+-rw-rw-r--   0 perry      (501) staff       (20)     1364 2023-07-23 20:36:37.000000 crypto_licensing-4.0.0/crypto_licensing/__init__.py
+-rw-rw-r--   0 perry      (501) staff       (20)     1365 2023-02-14 14:41:09.000000 crypto_licensing-4.0.0/crypto_licensing/__main__.py
+-rw-rw-r--   0 perry      (501) staff       (20)    10632 2023-02-16 18:04:11.000000 crypto_licensing-4.0.0/crypto_licensing/cli.py
+-rw-rw-r--   0 perry      (501) staff       (20)     3993 2023-02-15 19:50:25.000000 crypto_licensing-4.0.0/crypto_licensing/cli_test.py
+-rw-rw-r--   0 perry      (501) staff       (20)     5264 2023-02-05 15:25:14.000000 crypto_licensing-4.0.0/crypto_licensing/crypto_test.py
+drwxr-xr-x   0 perry      (501) staff       (20)        0 2024-05-19 23:54:58.922597 crypto_licensing-4.0.0/crypto_licensing/ed25519/
+-rw-rw-r--   0 perry      (501) staff       (20)     1655 2023-02-14 14:07:01.000000 crypto_licensing-4.0.0/crypto_licensing/ed25519/__init__.py
+-rw-rw-r--   0 perry      (501) staff       (20)     5033 2022-01-24 17:18:08.000000 crypto_licensing-4.0.0/crypto_licensing/ed25519_djb.py
+drwxr-xr-x   0 perry      (501) staff       (20)        0 2024-05-19 23:54:58.923694 crypto_licensing-4.0.0/crypto_licensing/ed25519ll_pyonly/
+-rw-rw-r--   0 perry      (501) staff       (20)     2319 2023-02-05 15:25:14.000000 crypto_licensing-4.0.0/crypto_licensing/ed25519ll_pyonly/__init__.py
+-rw-rw-r--   0 perry      (501) staff       (20)     6905 2022-01-19 19:14:43.000000 crypto_licensing-4.0.0/crypto_licensing/ed25519ll_pyonly/djbec.py
+drwxr-xr-x   0 perry      (501) staff       (20)        0 2024-05-19 23:54:58.930267 crypto_licensing-4.0.0/crypto_licensing/licensing/
+-rw-rw-r--   0 perry      (501) staff       (20)     1606 2023-02-21 15:58:27.000000 crypto_licensing-4.0.0/crypto_licensing/licensing/__init__.py
+-rw-rw-r--   0 perry      (501) staff       (20)     1196 2023-02-14 14:07:40.000000 crypto_licensing-4.0.0/crypto_licensing/licensing/__main__.py
+-rw-rw-r--   0 perry      (501) staff       (20)     1942 2023-02-05 15:25:14.000000 crypto_licensing-4.0.0/crypto_licensing/licensing/bitquery_test.py
+-rw-rw-r--   0 perry      (501) staff       (20)     2194 2023-02-14 14:08:13.000000 crypto_licensing-4.0.0/crypto_licensing/licensing/defaults.py
+drwxr-xr-x   0 perry      (501) staff       (20)        0 2024-05-19 23:54:58.931991 crypto_licensing-4.0.0/crypto_licensing/licensing/doh/
+-rw-rw-r--   0 perry      (501) staff       (20)     4511 2023-08-12 20:38:18.000000 crypto_licensing-4.0.0/crypto_licensing/licensing/doh/__init__.py
+-rw-rw-r--   0 perry      (501) staff       (20)     1362 2023-02-14 14:15:34.000000 crypto_licensing-4.0.0/crypto_licensing/licensing/doh/__main__.py
+-rw-rw-r--   0 perry      (501) staff       (20)     2731 2023-02-14 14:16:10.000000 crypto_licensing-4.0.0/crypto_licensing/licensing/doh/cli.py
+-rw-rw-r--   0 perry      (501) staff       (20)     4075 2024-05-18 21:53:39.000000 crypto_licensing-4.0.0/crypto_licensing/licensing/doh_test.py
+-rw-rw-r--   0 perry      (501) staff       (20)    17971 2023-02-05 15:25:14.000000 crypto_licensing-4.0.0/crypto_licensing/licensing/grant_test.py
+-rw-rw-r--   0 perry      (501) staff       (20)     7469 2023-02-05 15:25:14.000000 crypto_licensing-4.0.0/crypto_licensing/licensing/licensing_test.py
+-rw-rw-r--   0 perry      (501) staff       (20)    96445 2023-02-14 14:08:47.000000 crypto_licensing-4.0.0/crypto_licensing/licensing/main.py
+-rw-rw-r--   0 perry      (501) staff       (20)   155417 2023-07-22 14:39:37.000000 crypto_licensing-4.0.0/crypto_licensing/licensing/verification.py
+-rw-rw-r--   0 perry      (501) staff       (20)    41145 2023-02-23 18:12:32.000000 crypto_licensing-4.0.0/crypto_licensing/licensing/verification_test.py
+-rw-rw-r--   0 perry      (501) staff       (20)    43627 2024-05-18 21:53:39.000000 crypto_licensing-4.0.0/crypto_licensing/misc.py
+-rw-rw-r--   0 perry      (501) staff       (20)     9528 2023-02-05 15:25:17.000000 crypto_licensing-4.0.0/crypto_licensing/misc_test.py
+-rw-rw-r--   0 perry      (501) staff       (20)       88 2024-05-18 21:53:39.000000 crypto_licensing-4.0.0/crypto_licensing/version.py
+drwxr-xr-x   0 perry      (501) staff       (20)        0 2024-05-19 23:54:58.936257 crypto_licensing-4.0.0/crypto_licensing.egg-info/
+-rw-r--r--   0 perry      (501) staff       (20)     2085 2024-05-19 23:54:58.000000 crypto_licensing-4.0.0/crypto_licensing.egg-info/PKG-INFO
+-rw-rw-r--   0 perry      (501) staff       (20)     1331 2024-05-19 23:54:58.000000 crypto_licensing-4.0.0/crypto_licensing.egg-info/SOURCES.txt
+-rw-rw-r--   0 perry      (501) staff       (20)        1 2024-05-19 23:54:58.000000 crypto_licensing-4.0.0/crypto_licensing.egg-info/dependency_links.txt
+-rw-rw-r--   0 perry      (501) staff       (20)       74 2024-05-19 23:54:58.000000 crypto_licensing-4.0.0/crypto_licensing.egg-info/entry_points.txt
+-rw-rw-r--   0 perry      (501) staff       (20)      304 2024-05-19 23:54:58.000000 crypto_licensing-4.0.0/crypto_licensing.egg-info/requires.txt
+-rw-rw-r--   0 perry      (501) staff       (20)      134 2024-05-19 23:54:58.000000 crypto_licensing-4.0.0/crypto_licensing.egg-info/top_level.txt
+-rw-rw-r--   0 perry      (501) staff       (20)       48 2023-02-05 15:25:14.000000 crypto_licensing-4.0.0/requirements-dev.txt
+-rw-rw-r--   0 perry      (501) staff       (20)       21 2023-02-05 15:25:14.000000 crypto_licensing-4.0.0/requirements-tests.txt
+-rw-rw-r--   0 perry      (501) staff       (20)      352 2024-05-18 21:53:39.000000 crypto_licensing-4.0.0/requirements.txt
+-rw-r--r--   0 perry      (501) staff       (20)       38 2024-05-19 23:54:58.939280 crypto_licensing-4.0.0/setup.cfg
+-rw-rw-r--   0 perry      (501) staff       (20)     3157 2023-02-21 16:32:39.000000 crypto_licensing-4.0.0/setup.py
```

### Comparing `crypto_licensing-3.3.2/COPYING` & `crypto_licensing-4.0.0/COPYING`

 * *Files identical despite different names*

### Comparing `crypto_licensing-3.3.2/LICENSE` & `crypto_licensing-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crypto_licensing-3.3.2/README.org` & `crypto_licensing-4.0.0/README.org`

 * *Files identical despite different names*

### Comparing `crypto_licensing-3.3.2/README.txt` & `crypto_licensing-4.0.0/README.txt`

 * *Files identical despite different names*

### Comparing `crypto_licensing-3.3.2/crypto_licensing/__init__.py` & `crypto_licensing-4.0.0/crypto_licensing/__init__.py`

 * *Files identical despite different names*

### Comparing `crypto_licensing-3.3.2/crypto_licensing/__main__.py` & `crypto_licensing-4.0.0/crypto_licensing/__main__.py`

 * *Files identical despite different names*

### Comparing `crypto_licensing-3.3.2/crypto_licensing/cli.py` & `crypto_licensing-4.0.0/crypto_licensing/cli.py`

 * *Files identical despite different names*

### Comparing `crypto_licensing-3.3.2/crypto_licensing/cli_test.py` & `crypto_licensing-4.0.0/crypto_licensing/cli_test.py`

 * *Files identical despite different names*

### Comparing `crypto_licensing-3.3.2/crypto_licensing/crypto_test.py` & `crypto_licensing-4.0.0/crypto_licensing/crypto_test.py`

 * *Files identical despite different names*

### Comparing `crypto_licensing-3.3.2/crypto_licensing/ed25519/__init__.py` & `crypto_licensing-4.0.0/crypto_licensing/ed25519/__init__.py`

 * *Files identical despite different names*

### Comparing `crypto_licensing-3.3.2/crypto_licensing/ed25519_djb.py` & `crypto_licensing-4.0.0/crypto_licensing/ed25519_djb.py`

 * *Files identical despite different names*

### Comparing `crypto_licensing-3.3.2/crypto_licensing/ed25519ll_pyonly/__init__.py` & `crypto_licensing-4.0.0/crypto_licensing/ed25519ll_pyonly/__init__.py`

 * *Files identical despite different names*

### Comparing `crypto_licensing-3.3.2/crypto_licensing/ed25519ll_pyonly/djbec.py` & `crypto_licensing-4.0.0/crypto_licensing/ed25519ll_pyonly/djbec.py`

 * *Files identical despite different names*

### Comparing `crypto_licensing-3.3.2/crypto_licensing/licensing/__init__.py` & `crypto_licensing-4.0.0/crypto_licensing/licensing/__init__.py`

 * *Files identical despite different names*

### Comparing `crypto_licensing-3.3.2/crypto_licensing/licensing/__main__.py` & `crypto_licensing-4.0.0/crypto_licensing/licensing/__main__.py`

 * *Files identical despite different names*

### Comparing `crypto_licensing-3.3.2/crypto_licensing/licensing/bitquery_test.py` & `crypto_licensing-4.0.0/crypto_licensing/licensing/bitquery_test.py`

 * *Files identical despite different names*

### Comparing `crypto_licensing-3.3.2/crypto_licensing/licensing/defaults.py` & `crypto_licensing-4.0.0/crypto_licensing/licensing/defaults.py`

 * *Files identical despite different names*

### Comparing `crypto_licensing-3.3.2/crypto_licensing/licensing/doh/__init__.py` & `crypto_licensing-4.0.0/crypto_licensing/licensing/doh/__init__.py`

 * *Files identical despite different names*

### Comparing `crypto_licensing-3.3.2/crypto_licensing/licensing/doh/__main__.py` & `crypto_licensing-4.0.0/crypto_licensing/licensing/doh/__main__.py`

 * *Files identical despite different names*

### Comparing `crypto_licensing-3.3.2/crypto_licensing/licensing/doh/cli.py` & `crypto_licensing-4.0.0/crypto_licensing/licensing/doh/cli.py`

 * *Files identical despite different names*

### Comparing `crypto_licensing-3.3.2/crypto_licensing/licensing/doh_test.py` & `crypto_licensing-4.0.0/crypto_licensing/licensing/doh_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # -*- coding: utf-8 -*-
 
+import ast
 import json
 
 from ..misc import urlopen, urlencode, Request
 from . import doh
 
 import requests
 
+import dns.resolver
+
 
 def test_doh_smoke():
     """For example:
 
         curl -H "accept: application/dns-json" "https://cloudflare-dns.com/dns-query?name=example.com&type=AAAA"
     """
     #url				= 'https://cloudflare-dns.com/dns-query'
@@ -68,18 +71,29 @@
 
     assert len( recs ) == 1
     assert recs[0].get( 'data' ) \
         == 'v=DKIM1; k=ed25519; p=5cijeUNWyR1mvbIJpqNmUJ6V4Od7vPEgVWOEjxiim8w='
 
     # Now ensure multi-record (long) TXT entries are properly handled.
     recs			= doh.query(
-        "default._domainkey.xn----7hcbr.email", 'TXT' )
-    print( json.dumps( recs ) )
-    assert recs[0].get( 'data' ) \
-        == "v=DKIM1; k=rsa; p=MIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEA7qXVANitIc6CXteBZ/iJaTkoxZvosIu9WxGLrO2C3x5WkdzYPzTGwwosdKczTGuSZct6RPrUcwR3Rkh2p+b2hq1cn8qqHWN2XPNqZKv3VIiy2Vfahu5cUqaI3WmOIFyR57s21xi8bnKkuKfCCgKPefr9qw4bsZggaythKCosyUGFq3CG4fovTsUKGXsG5JzNm" "K61IAWLA7fnNK8SGKwoj9uVVFN1ps+mINFpqLtFvM7TweT1dlx5AShD8lJ0Bt+7EUTLp/nRRbZXbW1iKViSqiyJP4+2D0fxj8DkLOos5KKzAq9BrHYD9DsF9c8qgApO1U0iF4KsnqXMIHPbjtycTQIDAQAB;"
+        "default._domainkey.xn--8dbaco.email", 'TXT' )
+    recs_expected		= "v=DKIM1; k=rsa; p=MIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEA7qXVANitIc6CXteBZ/iJaTkoxZvosIu9WxGLrO2C3x5WkdzYPzTGwwosdKczTGuSZct6RPrUcwR3Rkh2p+b2hq1cn8qqHWN2XPNqZKv3VIiy2Vfahu5cUqaI3WmOIFyR57s21xi8bnKkuKfCCgKPefr9qw4bsZggaythKCosyUGFq3CG4fovTsUKGXsG5JzNmK61IAWLA7fnNK8SGKwoj9uVVFN1ps+mINFpqLtFvM7TweT1dlx5AShD8lJ0Bt+7EUTLp/nRRbZXbW1iKViSqiyJP4+2D0fxj8DkLOos5KKzAq9BrHYD9DsF9c8qgApO1U0iF4KsnqXMIHPbjtycTQIDAQAB;"
+    print( json.dumps( recs, indent=4 ))
+    assert recs[0].get( 'data' ) == recs_expected
 
     # Via Cloudflare, too?
     recs			= doh.query(
-        "default._domainkey.xn----7hcbr.email", 'TXT', provider=doh.DoH_Provider.CLOUDFLARE )
-    print( json.dumps( recs ) )
-    assert recs[0].get( 'data' ) \
-        == "v=DKIM1; k=rsa; p=MIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEA7qXVANitIc6CXteBZ/iJaTkoxZvosIu9WxGLrO2C3x5WkdzYPzTGwwosdKczTGuSZct6RPrUcwR3Rkh2p+b2hq1cn8qqHWN2XPNqZKv3VIiy2Vfahu5cUqaI3WmOIFyR57s21xi8bnKkuKfCCgKPefr9qw4bsZggaythKCosyUGFq3CG4fovTsUKGXsG5JzNm" "K61IAWLA7fnNK8SGKwoj9uVVFN1ps+mINFpqLtFvM7TweT1dlx5AShD8lJ0Bt+7EUTLp/nRRbZXbW1iKViSqiyJP4+2D0fxj8DkLOos5KKzAq9BrHYD9DsF9c8qgApO1U0iF4KsnqXMIHPbjtycTQIDAQAB;"
+        "default._domainkey.xn--8dbaco.email", 'TXT', provider=doh.DoH_Provider.CLOUDFLARE )
+    print( json.dumps( recs, indent=4 ))
+    assert recs[0].get( 'data' ) == recs_expected
+
+    # Standard DNS resolver splits long records
+    recs			= dns.resolver.query(
+        "default._domainkey.xn--8dbaco.email", 'TXT' )
+    recs_str			= list( map( str, recs ))
+    print( json.dumps( recs_str, indent=4 ))
+    assert recs_str \
+        == [
+            '"v=DKIM1; k=rsa; p=MIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEA7qXVANitIc6CXteBZ/iJaTkoxZvosIu9WxGLrO2C3x5WkdzYPzTGwwosdKczTGuSZct6RPrUcwR3Rkh2p+b2hq1cn8qqHWN2XPNqZKv3VIiy2Vfahu5cUqaI3WmOIFyR57s21xi8bnKkuKfCCgKPefr9qw4bsZggaythKCosyUGFq3CG4fovTsUKGXsG5JzNm" "K61IAWLA7fnNK8SGKwoj9uVVFN1ps+mINFpqLtFvM7TweT1dlx5AShD8lJ0Bt+7EUTLp/nRRbZXbW1iKViSqiyJP4+2D0fxj8DkLOos5KKzAq9BrHYD9DsF9c8qgApO1U0iF4KsnqXMIHPbjtycTQIDAQAB;"'
+        ]
+    assert ast.literal_eval( *recs_str ) == recs_expected
+
```

### Comparing `crypto_licensing-3.3.2/crypto_licensing/licensing/grant_test.py` & `crypto_licensing-4.0.0/crypto_licensing/licensing/grant_test.py`

 * *Files identical despite different names*

### Comparing `crypto_licensing-3.3.2/crypto_licensing/licensing/licensing_test.py` & `crypto_licensing-4.0.0/crypto_licensing/licensing/licensing_test.py`

 * *Files identical despite different names*

### Comparing `crypto_licensing-3.3.2/crypto_licensing/licensing/main.py` & `crypto_licensing-4.0.0/crypto_licensing/licensing/main.py`

 * *Files identical despite different names*

### Comparing `crypto_licensing-3.3.2/crypto_licensing/licensing/verification.py` & `crypto_licensing-4.0.0/crypto_licensing/licensing/verification.py`

 * *Files identical despite different names*

### Comparing `crypto_licensing-3.3.2/crypto_licensing/licensing/verification_test.py` & `crypto_licensing-4.0.0/crypto_licensing/licensing/verification_test.py`

 * *Files identical despite different names*

### Comparing `crypto_licensing-3.3.2/crypto_licensing/misc.py` & `crypto_licensing-4.0.0/crypto_licensing/misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -761,15 +761,15 @@
         dt			= super( Timestamp, self ).astimezone( tz )
         result			= dt.strftime( self._fmt )
         if subsecond:
             result	       += ( '%.*f' % ( subsecond, value ))[-subsecond-1:]
         if tz is not self.UTC or tzdetail is not None:
             if isinstance( tzdetail, (bool, type_str_base, type(None)) ):
                 if tzdetail is None or bool( tzdetail ):
-                    # full zone name if tzdetail is bool/str and Truthy (default)                    
+                    # full zone name if tzdetail is bool/str and Truthy (default)
                     try:
                         result += " " + dt.tzinfo.key
                     except AttributeError:
                         result += " " + dt.tzinfo.zone
                 else:
                     # Warning: result not parse-able, b/c TZ abbreviations are wildly non-deterministic
                     result       += dt.strftime(' %Z' )   # default abbreviation for non-UTC (only if tzdetail=='')
```

### Comparing `crypto_licensing-3.3.2/crypto_licensing/misc_test.py` & `crypto_licensing-4.0.0/crypto_licensing/misc_test.py`

 * *Files identical despite different names*

### Comparing `crypto_licensing-3.3.2/crypto_licensing.egg-info/SOURCES.txt` & `crypto_licensing-4.0.0/crypto_licensing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto_licensing-3.3.2/setup.py` & `crypto_licensing-4.0.0/setup.py`

 * *Files identical despite different names*

