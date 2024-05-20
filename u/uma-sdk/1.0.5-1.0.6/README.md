# Comparing `tmp/uma_sdk-1.0.5.zip` & `tmp/uma_sdk-1.0.6.zip`

## zipinfo {}

```diff
@@ -1,49 +1,49 @@
-Zip file size: 40084 bytes, number of entries: 47
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 21:08 uma_sdk-1.0.5/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 21:08 uma_sdk-1.0.5/uma_sdk.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 21:08 uma_sdk-1.0.5/uma/
--rw-r--r--  2.0 unx    11352 b- defN 24-May-02 21:08 uma_sdk-1.0.5/LICENSE
--rwxr-xr-x  2.0 unx       87 b- defN 24-May-02 21:08 uma_sdk-1.0.5/setup.py
--rw-r--r--  2.0 unx      133 b- defN 24-May-02 21:08 uma_sdk-1.0.5/README.md
--rw-r--r--  2.0 unx       81 b- defN 24-May-02 21:08 uma_sdk-1.0.5/pyproject.toml
--rw-r--r--  2.0 unx      648 b- defN 24-May-02 21:08 uma_sdk-1.0.5/setup.cfg
--rw-r--r--  2.0 unx      631 b- defN 24-May-02 21:08 uma_sdk-1.0.5/PKG-INFO
--rw-r--r--  2.0 unx        1 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma_sdk.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx      924 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma_sdk.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx        4 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma_sdk.egg-info/top_level.txt
--rw-r--r--  2.0 unx      631 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma_sdk.egg-info/PKG-INFO
--rw-r--r--  2.0 unx       30 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma_sdk.egg-info/requires.txt
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 21:08 uma_sdk-1.0.5/uma/protocol/
--rw-r--r--  2.0 unx     3407 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/JSONable.py
--rw-r--r--  2.0 unx     1624 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/public_key_cache.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/py.typed
--rw-r--r--  2.0 unx      284 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/uma_invoice_creator.py
--rw-r--r--  2.0 unx     2878 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/version.py
--rw-r--r--  2.0 unx      239 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/type_utils.py
--rw-r--r--  2.0 unx     2061 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/nonce_cache.py
--rw-r--r--  2.0 unx     2160 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/__init__.py
--rw-r--r--  2.0 unx     1117 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/cert_utils.py
--rw-r--r--  2.0 unx      266 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/urls.py
--rw-r--r--  2.0 unx    30711 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/uma.py
--rw-r--r--  2.0 unx      868 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/exceptions.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 21:08 uma_sdk-1.0.5/uma/protocol/v1/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 21:08 uma_sdk-1.0.5/uma/protocol/v0/
--rw-r--r--  2.0 unx     2591 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/protocol/lnurlp_request.py
--rw-r--r--  2.0 unx     8829 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/protocol/payreq_response.py
--rw-r--r--  2.0 unx     1724 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/protocol/post_tx_callback.py
--rw-r--r--  2.0 unx      132 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/protocol/payee_data.py
--rw-r--r--  2.0 unx     2307 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/protocol/payer_data.py
--rw-r--r--  2.0 unx      557 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/protocol/counterparty_data.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/protocol/__init__.py
--rw-r--r--  2.0 unx     3324 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/protocol/lnurlp_response.py
--rw-r--r--  2.0 unx     7993 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/protocol/payreq.py
--rw-r--r--  2.0 unx     4498 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/protocol/pubkey_response.py
--rw-r--r--  2.0 unx     4609 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/protocol/currency.py
--rw-r--r--  2.0 unx      231 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/protocol/kyc_status.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/protocol/v1/__init__.py
--rw-r--r--  2.0 unx     4294 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/protocol/v1/payreq.py
--rw-r--r--  2.0 unx     2702 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/protocol/v1/currency.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/protocol/v0/__init__.py
--rw-r--r--  2.0 unx     1788 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/protocol/v0/payreq.py
--rw-r--r--  2.0 unx     1950 b- defN 24-May-02 21:08 uma_sdk-1.0.5/uma/protocol/v0/currency.py
-47 files, 107666 bytes uncompressed, 33256 bytes compressed:  69.1%
+Zip file size: 40119 bytes, number of entries: 47
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 21:33 uma_sdk-1.0.6/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 21:33 uma_sdk-1.0.6/uma/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 21:33 uma_sdk-1.0.6/uma_sdk.egg-info/
+-rw-r--r--  2.0 unx      133 b- defN 24-May-20 21:33 uma_sdk-1.0.6/README.md
+-rw-r--r--  2.0 unx    11352 b- defN 24-May-20 21:33 uma_sdk-1.0.6/LICENSE
+-rw-r--r--  2.0 unx       81 b- defN 24-May-20 21:33 uma_sdk-1.0.6/pyproject.toml
+-rw-r--r--  2.0 unx      631 b- defN 24-May-20 21:33 uma_sdk-1.0.6/PKG-INFO
+-rw-r--r--  2.0 unx      648 b- defN 24-May-20 21:33 uma_sdk-1.0.6/setup.cfg
+-rwxr-xr-x  2.0 unx       87 b- defN 24-May-20 21:33 uma_sdk-1.0.6/setup.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 21:33 uma_sdk-1.0.6/uma/protocol/
+-rw-r--r--  2.0 unx     3407 b- defN 24-May-20 21:33 uma_sdk-1.0.6/uma/JSONable.py
+-rw-r--r--  2.0 unx     2160 b- defN 24-May-20 21:33 uma_sdk-1.0.6/uma/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 21:33 uma_sdk-1.0.6/uma/py.typed
+-rw-r--r--  2.0 unx    30807 b- defN 24-May-20 21:33 uma_sdk-1.0.6/uma/uma.py
+-rw-r--r--  2.0 unx     2061 b- defN 24-May-20 21:33 uma_sdk-1.0.6/uma/nonce_cache.py
+-rw-r--r--  2.0 unx     1624 b- defN 24-May-20 21:33 uma_sdk-1.0.6/uma/public_key_cache.py
+-rw-r--r--  2.0 unx      239 b- defN 24-May-20 21:33 uma_sdk-1.0.6/uma/type_utils.py
+-rw-r--r--  2.0 unx     2878 b- defN 24-May-20 21:33 uma_sdk-1.0.6/uma/version.py
+-rw-r--r--  2.0 unx      266 b- defN 24-May-20 21:33 uma_sdk-1.0.6/uma/urls.py
+-rw-r--r--  2.0 unx      284 b- defN 24-May-20 21:33 uma_sdk-1.0.6/uma/uma_invoice_creator.py
+-rw-r--r--  2.0 unx      868 b- defN 24-May-20 21:33 uma_sdk-1.0.6/uma/exceptions.py
+-rw-r--r--  2.0 unx     1117 b- defN 24-May-20 21:33 uma_sdk-1.0.6/uma/cert_utils.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 21:33 uma_sdk-1.0.6/uma/protocol/v1/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 21:33 uma_sdk-1.0.6/uma/protocol/v0/
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 21:33 uma_sdk-1.0.6/uma/protocol/__init__.py
+-rw-r--r--  2.0 unx      132 b- defN 24-May-20 21:33 uma_sdk-1.0.6/uma/protocol/payee_data.py
+-rw-r--r--  2.0 unx     2307 b- defN 24-May-20 21:33 uma_sdk-1.0.6/uma/protocol/payer_data.py
+-rw-r--r--  2.0 unx     8829 b- defN 24-May-20 21:33 uma_sdk-1.0.6/uma/protocol/payreq_response.py
+-rw-r--r--  2.0 unx      231 b- defN 24-May-20 21:33 uma_sdk-1.0.6/uma/protocol/kyc_status.py
+-rw-r--r--  2.0 unx     1724 b- defN 24-May-20 21:33 uma_sdk-1.0.6/uma/protocol/post_tx_callback.py
+-rw-r--r--  2.0 unx     7993 b- defN 24-May-20 21:33 uma_sdk-1.0.6/uma/protocol/payreq.py
+-rw-r--r--  2.0 unx     4498 b- defN 24-May-20 21:33 uma_sdk-1.0.6/uma/protocol/pubkey_response.py
+-rw-r--r--  2.0 unx     2591 b- defN 24-May-20 21:33 uma_sdk-1.0.6/uma/protocol/lnurlp_request.py
+-rw-r--r--  2.0 unx     4609 b- defN 24-May-20 21:33 uma_sdk-1.0.6/uma/protocol/currency.py
+-rw-r--r--  2.0 unx     3324 b- defN 24-May-20 21:33 uma_sdk-1.0.6/uma/protocol/lnurlp_response.py
+-rw-r--r--  2.0 unx      557 b- defN 24-May-20 21:33 uma_sdk-1.0.6/uma/protocol/counterparty_data.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 21:33 uma_sdk-1.0.6/uma/protocol/v1/__init__.py
+-rw-r--r--  2.0 unx     4294 b- defN 24-May-20 21:33 uma_sdk-1.0.6/uma/protocol/v1/payreq.py
+-rw-r--r--  2.0 unx     2702 b- defN 24-May-20 21:33 uma_sdk-1.0.6/uma/protocol/v1/currency.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 21:33 uma_sdk-1.0.6/uma/protocol/v0/__init__.py
+-rw-r--r--  2.0 unx     1788 b- defN 24-May-20 21:33 uma_sdk-1.0.6/uma/protocol/v0/payreq.py
+-rw-r--r--  2.0 unx     1950 b- defN 24-May-20 21:33 uma_sdk-1.0.6/uma/protocol/v0/currency.py
+-rw-r--r--  2.0 unx      924 b- defN 24-May-20 21:33 uma_sdk-1.0.6/uma_sdk.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx       30 b- defN 24-May-20 21:33 uma_sdk-1.0.6/uma_sdk.egg-info/requires.txt
+-rw-r--r--  2.0 unx      631 b- defN 24-May-20 21:33 uma_sdk-1.0.6/uma_sdk.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx        4 b- defN 24-May-20 21:33 uma_sdk-1.0.6/uma_sdk.egg-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-May-20 21:33 uma_sdk-1.0.6/uma_sdk.egg-info/dependency_links.txt
+47 files, 107762 bytes uncompressed, 33291 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -1,142 +1,142 @@
-Filename: uma_sdk-1.0.5/
+Filename: uma_sdk-1.0.6/
 Comment: 
 
-Filename: uma_sdk-1.0.5/uma_sdk.egg-info/
+Filename: uma_sdk-1.0.6/uma/
 Comment: 
 
-Filename: uma_sdk-1.0.5/uma/
+Filename: uma_sdk-1.0.6/uma_sdk.egg-info/
 Comment: 
 
-Filename: uma_sdk-1.0.5/LICENSE
+Filename: uma_sdk-1.0.6/README.md
 Comment: 
 
-Filename: uma_sdk-1.0.5/setup.py
+Filename: uma_sdk-1.0.6/LICENSE
 Comment: 
 
-Filename: uma_sdk-1.0.5/README.md
+Filename: uma_sdk-1.0.6/pyproject.toml
 Comment: 
 
-Filename: uma_sdk-1.0.5/pyproject.toml
+Filename: uma_sdk-1.0.6/PKG-INFO
 Comment: 
 
-Filename: uma_sdk-1.0.5/setup.cfg
+Filename: uma_sdk-1.0.6/setup.cfg
 Comment: 
 
-Filename: uma_sdk-1.0.5/PKG-INFO
+Filename: uma_sdk-1.0.6/setup.py
 Comment: 
 
-Filename: uma_sdk-1.0.5/uma_sdk.egg-info/dependency_links.txt
+Filename: uma_sdk-1.0.6/uma/protocol/
 Comment: 
 
-Filename: uma_sdk-1.0.5/uma_sdk.egg-info/SOURCES.txt
+Filename: uma_sdk-1.0.6/uma/JSONable.py
 Comment: 
 
-Filename: uma_sdk-1.0.5/uma_sdk.egg-info/top_level.txt
+Filename: uma_sdk-1.0.6/uma/__init__.py
 Comment: 
 
-Filename: uma_sdk-1.0.5/uma_sdk.egg-info/PKG-INFO
+Filename: uma_sdk-1.0.6/uma/py.typed
 Comment: 
 
-Filename: uma_sdk-1.0.5/uma_sdk.egg-info/requires.txt
+Filename: uma_sdk-1.0.6/uma/uma.py
 Comment: 
 
-Filename: uma_sdk-1.0.5/uma/protocol/
+Filename: uma_sdk-1.0.6/uma/nonce_cache.py
 Comment: 
 
-Filename: uma_sdk-1.0.5/uma/JSONable.py
+Filename: uma_sdk-1.0.6/uma/public_key_cache.py
 Comment: 
 
-Filename: uma_sdk-1.0.5/uma/public_key_cache.py
+Filename: uma_sdk-1.0.6/uma/type_utils.py
 Comment: 
 
-Filename: uma_sdk-1.0.5/uma/py.typed
+Filename: uma_sdk-1.0.6/uma/version.py
 Comment: 
 
-Filename: uma_sdk-1.0.5/uma/uma_invoice_creator.py
+Filename: uma_sdk-1.0.6/uma/urls.py
 Comment: 
 
-Filename: uma_sdk-1.0.5/uma/version.py
+Filename: uma_sdk-1.0.6/uma/uma_invoice_creator.py
 Comment: 
 
-Filename: uma_sdk-1.0.5/uma/type_utils.py
+Filename: uma_sdk-1.0.6/uma/exceptions.py
 Comment: 
 
-Filename: uma_sdk-1.0.5/uma/nonce_cache.py
+Filename: uma_sdk-1.0.6/uma/cert_utils.py
 Comment: 
 
-Filename: uma_sdk-1.0.5/uma/__init__.py
+Filename: uma_sdk-1.0.6/uma/protocol/v1/
 Comment: 
 
-Filename: uma_sdk-1.0.5/uma/cert_utils.py
+Filename: uma_sdk-1.0.6/uma/protocol/v0/
 Comment: 
 
-Filename: uma_sdk-1.0.5/uma/urls.py
+Filename: uma_sdk-1.0.6/uma/protocol/__init__.py
 Comment: 
 
-Filename: uma_sdk-1.0.5/uma/uma.py
+Filename: uma_sdk-1.0.6/uma/protocol/payee_data.py
 Comment: 
 
-Filename: uma_sdk-1.0.5/uma/exceptions.py
+Filename: uma_sdk-1.0.6/uma/protocol/payer_data.py
 Comment: 
 
-Filename: uma_sdk-1.0.5/uma/protocol/v1/
+Filename: uma_sdk-1.0.6/uma/protocol/payreq_response.py
 Comment: 
 
-Filename: uma_sdk-1.0.5/uma/protocol/v0/
+Filename: uma_sdk-1.0.6/uma/protocol/kyc_status.py
 Comment: 
 
-Filename: uma_sdk-1.0.5/uma/protocol/lnurlp_request.py
+Filename: uma_sdk-1.0.6/uma/protocol/post_tx_callback.py
 Comment: 
 
-Filename: uma_sdk-1.0.5/uma/protocol/payreq_response.py
+Filename: uma_sdk-1.0.6/uma/protocol/payreq.py
 Comment: 
 
-Filename: uma_sdk-1.0.5/uma/protocol/post_tx_callback.py
+Filename: uma_sdk-1.0.6/uma/protocol/pubkey_response.py
 Comment: 
 
-Filename: uma_sdk-1.0.5/uma/protocol/payee_data.py
+Filename: uma_sdk-1.0.6/uma/protocol/lnurlp_request.py
 Comment: 
 
-Filename: uma_sdk-1.0.5/uma/protocol/payer_data.py
+Filename: uma_sdk-1.0.6/uma/protocol/currency.py
 Comment: 
 
-Filename: uma_sdk-1.0.5/uma/protocol/counterparty_data.py
+Filename: uma_sdk-1.0.6/uma/protocol/lnurlp_response.py
 Comment: 
 
-Filename: uma_sdk-1.0.5/uma/protocol/__init__.py
+Filename: uma_sdk-1.0.6/uma/protocol/counterparty_data.py
 Comment: 
 
-Filename: uma_sdk-1.0.5/uma/protocol/lnurlp_response.py
+Filename: uma_sdk-1.0.6/uma/protocol/v1/__init__.py
 Comment: 
 
-Filename: uma_sdk-1.0.5/uma/protocol/payreq.py
+Filename: uma_sdk-1.0.6/uma/protocol/v1/payreq.py
 Comment: 
 
-Filename: uma_sdk-1.0.5/uma/protocol/pubkey_response.py
+Filename: uma_sdk-1.0.6/uma/protocol/v1/currency.py
 Comment: 
 
-Filename: uma_sdk-1.0.5/uma/protocol/currency.py
+Filename: uma_sdk-1.0.6/uma/protocol/v0/__init__.py
 Comment: 
 
-Filename: uma_sdk-1.0.5/uma/protocol/kyc_status.py
+Filename: uma_sdk-1.0.6/uma/protocol/v0/payreq.py
 Comment: 
 
-Filename: uma_sdk-1.0.5/uma/protocol/v1/__init__.py
+Filename: uma_sdk-1.0.6/uma/protocol/v0/currency.py
 Comment: 
 
-Filename: uma_sdk-1.0.5/uma/protocol/v1/payreq.py
+Filename: uma_sdk-1.0.6/uma_sdk.egg-info/SOURCES.txt
 Comment: 
 
-Filename: uma_sdk-1.0.5/uma/protocol/v1/currency.py
+Filename: uma_sdk-1.0.6/uma_sdk.egg-info/requires.txt
 Comment: 
 
-Filename: uma_sdk-1.0.5/uma/protocol/v0/__init__.py
+Filename: uma_sdk-1.0.6/uma_sdk.egg-info/PKG-INFO
 Comment: 
 
-Filename: uma_sdk-1.0.5/uma/protocol/v0/payreq.py
+Filename: uma_sdk-1.0.6/uma_sdk.egg-info/top_level.txt
 Comment: 
 
-Filename: uma_sdk-1.0.5/uma/protocol/v0/currency.py
+Filename: uma_sdk-1.0.6/uma_sdk.egg-info/dependency_links.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `uma_sdk-1.0.5/LICENSE` & `uma_sdk-1.0.6/LICENSE`

 * *Files identical despite different names*

## Comparing `uma_sdk-1.0.5/setup.cfg` & `uma_sdk-1.0.6/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = uma-sdk
-version = 1.0.5
+version = 1.0.6
 description = Python SDK for UMA (universal money address)
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Lightspark Group, Inc.
 author_email = info@lightspark.com
 license = Apache-2.0
 license_files = LICENSE
```

## Comparing `uma_sdk-1.0.5/PKG-INFO` & `uma_sdk-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uma-sdk
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python SDK for UMA (universal money address)
 Author: Lightspark Group, Inc.
 Author-email: info@lightspark.com
 License: Apache-2.0
 Project-URL: Documentation, https://app.lightspark.com/docs/uma-sdk/introduction
 Project-URL: Source Code, https://github.com/uma-universal-money-address/uma-python-sdk/
 Description-Content-Type: text/markdown
```

## Comparing `uma_sdk-1.0.5/uma_sdk.egg-info/SOURCES.txt` & `uma_sdk-1.0.6/uma_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `uma_sdk-1.0.5/uma_sdk.egg-info/PKG-INFO` & `uma_sdk-1.0.6/uma_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uma-sdk
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python SDK for UMA (universal money address)
 Author: Lightspark Group, Inc.
 Author-email: info@lightspark.com
 License: Apache-2.0
 Project-URL: Documentation, https://app.lightspark.com/docs/uma-sdk/introduction
 Project-URL: Source Code, https://github.com/uma-universal-money-address/uma-python-sdk/
 Description-Content-Type: text/markdown
```

## Comparing `uma_sdk-1.0.5/uma/JSONable.py` & `uma_sdk-1.0.6/uma/JSONable.py`

 * *Files identical despite different names*

## Comparing `uma_sdk-1.0.5/uma/public_key_cache.py` & `uma_sdk-1.0.6/uma/public_key_cache.py`

 * *Files identical despite different names*

## Comparing `uma_sdk-1.0.5/uma/version.py` & `uma_sdk-1.0.6/uma/version.py`

 * *Files identical despite different names*

## Comparing `uma_sdk-1.0.5/uma/nonce_cache.py` & `uma_sdk-1.0.6/uma/nonce_cache.py`

 * *Files identical despite different names*

## Comparing `uma_sdk-1.0.5/uma/__init__.py` & `uma_sdk-1.0.6/uma/__init__.py`

 * *Files identical despite different names*

## Comparing `uma_sdk-1.0.5/uma/cert_utils.py` & `uma_sdk-1.0.6/uma/cert_utils.py`

 * *Files identical despite different names*

## Comparing `uma_sdk-1.0.5/uma/uma.py` & `uma_sdk-1.0.6/uma/uma.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
         )
     compliance_data = compliance_from_payer_data(request.payer_data)
     if not compliance_data:
         raise InvalidRequestException("Missing compliance data in request")
 
     nonce_cache.check_and_save_nonce(
         compliance_data.signature_nonce,
-        datetime.fromtimestamp(compliance_data.signature_timestamp, timezone.utc),
+        _parse_timestamp(compliance_data.signature_timestamp),
     )
     _verify_signature(
         request.signable_payload(),
         compliance_data.signature,
         other_vasp_pubkeys.get_signing_pubkey(),
     )
 
@@ -370,17 +370,15 @@
 
     return LnurlpRequest(
         receiver_address=receiver_address,
         nonce=nonce,
         signature=signature,
         is_subject_to_travel_rule=is_subject_to_travel_rule,
         vasp_domain=vasp_domain,
-        timestamp=(
-            datetime.fromtimestamp(int(timestamp), timezone.utc) if timestamp else None
-        ),
+        timestamp=(_parse_timestamp(int(timestamp)) if timestamp else None),
         uma_version=uma_version,
     )
 
 
 def is_uma_lnurlp_query(url: str) -> bool:
     try:
         request = parse_lnurlp_request(url)
@@ -583,17 +581,15 @@
     if response.uma_major_version != 1:
         raise InvalidRequestException(
             "Signatures were added to payreq responses in UMA v1. This response is from an UMA v0 receiving VASP."
         )
 
     nonce_cache.check_and_save_nonce(
         none_throws(compliance_data.signature_nonce),
-        datetime.fromtimestamp(
-            none_throws(compliance_data.signature_timestamp), timezone.utc
-        ),
+        _parse_timestamp(none_throws(compliance_data.signature_timestamp)),
     )
     _verify_signature(
         compliance_data.signable_payload(sender_address, receiver_address),
         none_throws(compliance_data.signature),
         other_vasp_pubkeys.get_signing_pubkey(),
     )
 
@@ -611,15 +607,15 @@
     receiver_kyc_status: KycStatus,
     comment_chars_allowed: Optional[int] = None,
     nostr_pubkey: Optional[str] = None,
 ) -> LnurlpResponse:
     if not request.is_uma_request():
         raise InvalidRequestException(
             "The request is not a UMA request. Cannot create an UMA response. "
-            + "Just create an LnurlpReasponse directly instead."
+            + "Just create an LnurlpResponse directly instead."
         )
     uma_version = select_lower_version(
         none_throws(request.uma_version), UMA_PROTOCOL_VERSION
     )
     compliance = _create_signed_lnurlp_compliance_response(
         request=request,
         signing_private_key=signing_private_key,
@@ -684,15 +680,15 @@
     nonce_cache: INonceCache,
 ) -> None:
     if not response.compliance:
         raise InvalidRequestException("Missing compliance data in response")
 
     nonce_cache.check_and_save_nonce(
         response.compliance.signature_nonce,
-        datetime.fromtimestamp(response.compliance.signature_timestamp, timezone.utc),
+        _parse_timestamp(response.compliance.signature_timestamp),
     )
     _verify_signature(
         response.signable_payload(),
         none_throws(response.compliance).signature,
         other_vasp_pubkeys.get_signing_pubkey(),
     )
 
@@ -775,14 +771,23 @@
         or not callback.signature_timestamp
     ):
         raise InvalidRequestException(
             "Missing post transaction callback signature, nonce, or timestamp. Is this an UMA v0 callback? If so, don't verify the signature."
         )
     nonce_cache.check_and_save_nonce(
         callback.signature_nonce,
-        datetime.fromtimestamp(callback.signature_timestamp, timezone.utc),
+        _parse_timestamp(callback.signature_timestamp),
     )
     _verify_signature(
         callback.signable_payload(),
         none_throws(callback.signature),
         other_vasp_pubkeys.get_signing_pubkey(),
     )
+
+
+def _parse_timestamp(
+    timestamp: float,
+) -> datetime:
+    try:
+        return datetime.fromtimestamp(timestamp, timezone.utc)
+    except ValueError as ex:
+        raise InvalidRequestException("Invalid timestamp in request.") from ex
```

## Comparing `uma_sdk-1.0.5/uma/exceptions.py` & `uma_sdk-1.0.6/uma/exceptions.py`

 * *Files identical despite different names*

## Comparing `uma_sdk-1.0.5/uma/protocol/lnurlp_request.py` & `uma_sdk-1.0.6/uma/protocol/lnurlp_request.py`

 * *Files identical despite different names*

## Comparing `uma_sdk-1.0.5/uma/protocol/payreq_response.py` & `uma_sdk-1.0.6/uma/protocol/payreq_response.py`

 * *Files identical despite different names*

## Comparing `uma_sdk-1.0.5/uma/protocol/post_tx_callback.py` & `uma_sdk-1.0.6/uma/protocol/post_tx_callback.py`

 * *Files identical despite different names*

## Comparing `uma_sdk-1.0.5/uma/protocol/payer_data.py` & `uma_sdk-1.0.6/uma/protocol/payer_data.py`

 * *Files identical despite different names*

## Comparing `uma_sdk-1.0.5/uma/protocol/counterparty_data.py` & `uma_sdk-1.0.6/uma/protocol/counterparty_data.py`

 * *Files identical despite different names*

## Comparing `uma_sdk-1.0.5/uma/protocol/lnurlp_response.py` & `uma_sdk-1.0.6/uma/protocol/lnurlp_response.py`

 * *Files identical despite different names*

## Comparing `uma_sdk-1.0.5/uma/protocol/payreq.py` & `uma_sdk-1.0.6/uma/protocol/payreq.py`

 * *Files identical despite different names*

## Comparing `uma_sdk-1.0.5/uma/protocol/pubkey_response.py` & `uma_sdk-1.0.6/uma/protocol/pubkey_response.py`

 * *Files identical despite different names*

## Comparing `uma_sdk-1.0.5/uma/protocol/currency.py` & `uma_sdk-1.0.6/uma/protocol/currency.py`

 * *Files identical despite different names*

## Comparing `uma_sdk-1.0.5/uma/protocol/v1/payreq.py` & `uma_sdk-1.0.6/uma/protocol/v1/payreq.py`

 * *Files identical despite different names*

## Comparing `uma_sdk-1.0.5/uma/protocol/v1/currency.py` & `uma_sdk-1.0.6/uma/protocol/v1/currency.py`

 * *Files identical despite different names*

## Comparing `uma_sdk-1.0.5/uma/protocol/v0/payreq.py` & `uma_sdk-1.0.6/uma/protocol/v0/payreq.py`

 * *Files identical despite different names*

## Comparing `uma_sdk-1.0.5/uma/protocol/v0/currency.py` & `uma_sdk-1.0.6/uma/protocol/v0/currency.py`

 * *Files identical despite different names*

