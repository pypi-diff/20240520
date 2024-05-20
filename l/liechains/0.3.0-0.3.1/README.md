# Comparing `tmp/liechains-0.3.0.tar.gz` & `tmp/liechains-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liechains-0.3.0.tar", last modified: Wed May 15 03:49:47 2024, max compression
+gzip compressed data, was "liechains-0.3.1.tar", last modified: Mon May 20 08:33:52 2024, max compression
```

## Comparing `liechains-0.3.0.tar` & `liechains-0.3.1.tar`

### file list

```diff
@@ -1,39 +1,42 @@
-drwxr-xr-x   0 liewhite   (501) staff       (20)        0 2024-05-15 03:49:47.273298 liechains-0.3.0/
--rw-r--r--   0 liewhite   (501) staff       (20)      391 2024-05-15 03:49:47.273088 liechains-0.3.0/PKG-INFO
--rw-r--r--   0 liewhite   (501) staff       (20)       79 2023-12-23 16:23:29.000000 liechains-0.3.0/README
-drwxr-xr-x   0 liewhite   (501) staff       (20)        0 2024-05-15 03:49:47.268433 liechains-0.3.0/ether/
--rw-r--r--   0 liewhite   (501) staff       (20)       79 2024-01-05 02:46:35.000000 liechains-0.3.0/ether/__init__.py
--rw-r--r--   0 liewhite   (501) staff       (20)    87154 2024-01-19 06:15:15.000000 liechains-0.3.0/ether/abis.py
--rw-r--r--   0 liewhite   (501) staff       (20)     2196 2024-01-17 07:25:06.000000 liechains-0.3.0/ether/chains.py
--rw-r--r--   0 liewhite   (501) staff       (20)     2386 2024-02-18 06:11:21.000000 liechains-0.3.0/ether/client.py
-drwxr-xr-x   0 liewhite   (501) staff       (20)        0 2024-05-15 03:49:47.269504 liechains-0.3.0/ether/dex/
--rw-r--r--   0 liewhite   (501) staff       (20)        0 2024-05-15 02:32:41.000000 liechains-0.3.0/ether/dex/__init__.py
--rw-r--r--   0 liewhite   (501) staff       (20)      296 2024-05-15 03:04:21.000000 liechains-0.3.0/ether/dex/swap.py
--rw-r--r--   0 liewhite   (501) staff       (20)    23963 2024-05-15 03:02:54.000000 liechains-0.3.0/ether/dex/univ2.py
--rw-r--r--   0 liewhite   (501) staff       (20)    25419 2024-05-15 03:48:41.000000 liechains-0.3.0/ether/dex/univ3.py
-drwxr-xr-x   0 liewhite   (501) staff       (20)        0 2024-05-15 03:49:47.271061 liechains-0.3.0/ether/flashbots/
--rw-r--r--   0 liewhite   (501) staff       (20)     1069 2023-12-23 13:20:13.000000 liechains-0.3.0/ether/flashbots/__init__.py
--rw-r--r--   0 liewhite   (501) staff       (20)     1970 2023-12-23 13:20:13.000000 liechains-0.3.0/ether/flashbots/blox.py
--rw-r--r--   0 liewhite   (501) staff       (20)     8467 2023-12-23 13:20:13.000000 liechains-0.3.0/ether/flashbots/flashbots.py
--rw-r--r--   0 liewhite   (501) staff       (20)     1510 2023-12-23 13:20:13.000000 liechains-0.3.0/ether/flashbots/middleware.py
--rw-r--r--   0 liewhite   (501) staff       (20)     2400 2023-12-23 13:20:13.000000 liechains-0.3.0/ether/flashbots/provider.py
--rw-r--r--   0 liewhite   (501) staff       (20)     1923 2023-12-23 13:20:13.000000 liechains-0.3.0/ether/flashbots/types.py
--rw-r--r--   0 liewhite   (501) staff       (20)      592 2024-01-02 03:50:13.000000 liechains-0.3.0/ether/mev.py
-drwxr-xr-x   0 liewhite   (501) staff       (20)        0 2024-05-15 03:49:47.271340 liechains-0.3.0/ether/middlewares/
--rw-r--r--   0 liewhite   (501) staff       (20)        0 2024-01-17 06:27:34.000000 liechains-0.3.0/ether/middlewares/__init__.py
--rw-r--r--   0 liewhite   (501) staff       (20)    10060 2024-01-17 06:44:14.000000 liechains-0.3.0/ether/middlewares/remote_signer.py
-drwxr-xr-x   0 liewhite   (501) staff       (20)        0 2024-05-15 03:49:47.271955 liechains-0.3.0/ether/tools/
--rw-r--r--   0 liewhite   (501) staff       (20)        0 2023-12-25 07:24:34.000000 liechains-0.3.0/ether/tools/__init__.py
--rw-r--r--   0 liewhite   (501) staff       (20)      468 2023-12-25 07:49:26.000000 liechains-0.3.0/ether/tools/erc20_balance.py
--rw-r--r--   0 liewhite   (501) staff       (20)      731 2023-12-29 09:41:21.000000 liechains-0.3.0/ether/tools/mnemonic.py
--rw-r--r--   0 liewhite   (501) staff       (20)     2062 2024-02-18 09:48:22.000000 liechains-0.3.0/ether/utils.py
--rw-r--r--   0 liewhite   (501) staff       (20)      908 2024-01-09 09:12:59.000000 liechains-0.3.0/ether/wallet.py
--rw-r--r--   0 liewhite   (501) staff       (20)      958 2023-12-23 13:22:12.000000 liechains-0.3.0/ether/ws.py
-drwxr-xr-x   0 liewhite   (501) staff       (20)        0 2024-05-15 03:49:47.272839 liechains-0.3.0/liechains.egg-info/
--rw-r--r--   0 liewhite   (501) staff       (20)      391 2024-05-15 03:49:47.000000 liechains-0.3.0/liechains.egg-info/PKG-INFO
--rw-r--r--   0 liewhite   (501) staff       (20)      683 2024-05-15 03:49:47.000000 liechains-0.3.0/liechains.egg-info/SOURCES.txt
--rw-r--r--   0 liewhite   (501) staff       (20)        1 2024-05-15 03:49:47.000000 liechains-0.3.0/liechains.egg-info/dependency_links.txt
--rw-r--r--   0 liewhite   (501) staff       (20)       35 2024-05-15 03:49:47.000000 liechains-0.3.0/liechains.egg-info/requires.txt
--rw-r--r--   0 liewhite   (501) staff       (20)        6 2024-05-15 03:49:47.000000 liechains-0.3.0/liechains.egg-info/top_level.txt
--rw-r--r--   0 liewhite   (501) staff       (20)       38 2024-05-15 03:49:47.273336 liechains-0.3.0/setup.cfg
--rw-r--r--   0 liewhite   (501) staff       (20)      532 2024-05-15 03:49:20.000000 liechains-0.3.0/setup.py
+drwxr-xr-x   0 liewhite   (501) staff       (20)        0 2024-05-20 08:33:52.573495 liechains-0.3.1/
+-rw-r--r--   0 liewhite   (501) staff       (20)      391 2024-05-20 08:33:52.573230 liechains-0.3.1/PKG-INFO
+-rw-r--r--   0 liewhite   (501) staff       (20)       79 2023-12-23 16:23:29.000000 liechains-0.3.1/README
+drwxr-xr-x   0 liewhite   (501) staff       (20)        0 2024-05-20 08:33:52.559795 liechains-0.3.1/ether/
+-rw-r--r--   0 liewhite   (501) staff       (20)       79 2024-01-05 02:46:35.000000 liechains-0.3.1/ether/__init__.py
+-rw-r--r--   0 liewhite   (501) staff       (20)    87154 2024-01-19 06:15:15.000000 liechains-0.3.1/ether/abis.py
+-rw-r--r--   0 liewhite   (501) staff       (20)     2196 2024-01-17 07:25:06.000000 liechains-0.3.1/ether/chains.py
+-rw-r--r--   0 liewhite   (501) staff       (20)     2386 2024-02-18 06:11:21.000000 liechains-0.3.1/ether/client.py
+drwxr-xr-x   0 liewhite   (501) staff       (20)        0 2024-05-20 08:33:52.562155 liechains-0.3.1/ether/dex/
+-rw-r--r--   0 liewhite   (501) staff       (20)        0 2024-05-15 02:32:41.000000 liechains-0.3.1/ether/dex/__init__.py
+-rw-r--r--   0 liewhite   (501) staff       (20)    18165 2024-05-20 08:33:27.000000 liechains-0.3.1/ether/dex/balancer.py
+-rw-r--r--   0 liewhite   (501) staff       (20)     9747 2024-05-20 07:03:20.000000 liechains-0.3.1/ether/dex/curve.py
+-rw-r--r--   0 liewhite   (501) staff       (20)     1812 2024-05-16 02:48:29.000000 liechains-0.3.1/ether/dex/limit_order.py
+-rw-r--r--   0 liewhite   (501) staff       (20)      296 2024-05-15 03:04:21.000000 liechains-0.3.1/ether/dex/swap.py
+-rw-r--r--   0 liewhite   (501) staff       (20)    23963 2024-05-15 03:02:54.000000 liechains-0.3.1/ether/dex/univ2.py
+-rw-r--r--   0 liewhite   (501) staff       (20)    25419 2024-05-15 03:48:41.000000 liechains-0.3.1/ether/dex/univ3.py
+drwxr-xr-x   0 liewhite   (501) staff       (20)        0 2024-05-20 08:33:52.566273 liechains-0.3.1/ether/flashbots/
+-rw-r--r--   0 liewhite   (501) staff       (20)     1069 2023-12-23 13:20:13.000000 liechains-0.3.1/ether/flashbots/__init__.py
+-rw-r--r--   0 liewhite   (501) staff       (20)     1970 2023-12-23 13:20:13.000000 liechains-0.3.1/ether/flashbots/blox.py
+-rw-r--r--   0 liewhite   (501) staff       (20)     8467 2023-12-23 13:20:13.000000 liechains-0.3.1/ether/flashbots/flashbots.py
+-rw-r--r--   0 liewhite   (501) staff       (20)     1510 2023-12-23 13:20:13.000000 liechains-0.3.1/ether/flashbots/middleware.py
+-rw-r--r--   0 liewhite   (501) staff       (20)     2400 2023-12-23 13:20:13.000000 liechains-0.3.1/ether/flashbots/provider.py
+-rw-r--r--   0 liewhite   (501) staff       (20)     1923 2023-12-23 13:20:13.000000 liechains-0.3.1/ether/flashbots/types.py
+-rw-r--r--   0 liewhite   (501) staff       (20)      592 2024-01-02 03:50:13.000000 liechains-0.3.1/ether/mev.py
+drwxr-xr-x   0 liewhite   (501) staff       (20)        0 2024-05-20 08:33:52.566560 liechains-0.3.1/ether/middlewares/
+-rw-r--r--   0 liewhite   (501) staff       (20)        0 2024-01-17 06:27:34.000000 liechains-0.3.1/ether/middlewares/__init__.py
+-rw-r--r--   0 liewhite   (501) staff       (20)    10060 2024-01-17 06:44:14.000000 liechains-0.3.1/ether/middlewares/remote_signer.py
+drwxr-xr-x   0 liewhite   (501) staff       (20)        0 2024-05-20 08:33:52.571709 liechains-0.3.1/ether/tools/
+-rw-r--r--   0 liewhite   (501) staff       (20)        0 2023-12-25 07:24:34.000000 liechains-0.3.1/ether/tools/__init__.py
+-rw-r--r--   0 liewhite   (501) staff       (20)      468 2023-12-25 07:49:26.000000 liechains-0.3.1/ether/tools/erc20_balance.py
+-rw-r--r--   0 liewhite   (501) staff       (20)      731 2023-12-29 09:41:21.000000 liechains-0.3.1/ether/tools/mnemonic.py
+-rw-r--r--   0 liewhite   (501) staff       (20)     2062 2024-02-18 09:48:22.000000 liechains-0.3.1/ether/utils.py
+-rw-r--r--   0 liewhite   (501) staff       (20)      908 2024-01-09 09:12:59.000000 liechains-0.3.1/ether/wallet.py
+-rw-r--r--   0 liewhite   (501) staff       (20)      958 2023-12-23 13:22:12.000000 liechains-0.3.1/ether/ws.py
+drwxr-xr-x   0 liewhite   (501) staff       (20)        0 2024-05-20 08:33:52.572887 liechains-0.3.1/liechains.egg-info/
+-rw-r--r--   0 liewhite   (501) staff       (20)      391 2024-05-20 08:33:52.000000 liechains-0.3.1/liechains.egg-info/PKG-INFO
+-rw-r--r--   0 liewhite   (501) staff       (20)      749 2024-05-20 08:33:52.000000 liechains-0.3.1/liechains.egg-info/SOURCES.txt
+-rw-r--r--   0 liewhite   (501) staff       (20)        1 2024-05-20 08:33:52.000000 liechains-0.3.1/liechains.egg-info/dependency_links.txt
+-rw-r--r--   0 liewhite   (501) staff       (20)       35 2024-05-20 08:33:52.000000 liechains-0.3.1/liechains.egg-info/requires.txt
+-rw-r--r--   0 liewhite   (501) staff       (20)        6 2024-05-20 08:33:52.000000 liechains-0.3.1/liechains.egg-info/top_level.txt
+-rw-r--r--   0 liewhite   (501) staff       (20)       38 2024-05-20 08:33:52.573539 liechains-0.3.1/setup.cfg
+-rw-r--r--   0 liewhite   (501) staff       (20)      532 2024-05-20 08:33:45.000000 liechains-0.3.1/setup.py
```

### Comparing `liechains-0.3.0/ether/abis.py` & `liechains-0.3.1/ether/abis.py`

 * *Files identical despite different names*

### Comparing `liechains-0.3.0/ether/chains.py` & `liechains-0.3.1/ether/chains.py`

 * *Files identical despite different names*

### Comparing `liechains-0.3.0/ether/client.py` & `liechains-0.3.1/ether/client.py`

 * *Files identical despite different names*

### Comparing `liechains-0.3.0/ether/dex/univ2.py` & `liechains-0.3.1/ether/dex/univ2.py`

 * *Files identical despite different names*

### Comparing `liechains-0.3.0/ether/dex/univ3.py` & `liechains-0.3.1/ether/dex/univ3.py`

 * *Files identical despite different names*

### Comparing `liechains-0.3.0/ether/flashbots/__init__.py` & `liechains-0.3.1/ether/flashbots/__init__.py`

 * *Files identical despite different names*

### Comparing `liechains-0.3.0/ether/flashbots/blox.py` & `liechains-0.3.1/ether/flashbots/blox.py`

 * *Files identical despite different names*

### Comparing `liechains-0.3.0/ether/flashbots/flashbots.py` & `liechains-0.3.1/ether/flashbots/flashbots.py`

 * *Files identical despite different names*

### Comparing `liechains-0.3.0/ether/flashbots/middleware.py` & `liechains-0.3.1/ether/flashbots/middleware.py`

 * *Files identical despite different names*

### Comparing `liechains-0.3.0/ether/flashbots/provider.py` & `liechains-0.3.1/ether/flashbots/provider.py`

 * *Files identical despite different names*

### Comparing `liechains-0.3.0/ether/flashbots/types.py` & `liechains-0.3.1/ether/flashbots/types.py`

 * *Files identical despite different names*

### Comparing `liechains-0.3.0/ether/mev.py` & `liechains-0.3.1/ether/mev.py`

 * *Files identical despite different names*

### Comparing `liechains-0.3.0/ether/middlewares/remote_signer.py` & `liechains-0.3.1/ether/middlewares/remote_signer.py`

 * *Files identical despite different names*

### Comparing `liechains-0.3.0/ether/tools/mnemonic.py` & `liechains-0.3.1/ether/tools/mnemonic.py`

 * *Files identical despite different names*

### Comparing `liechains-0.3.0/ether/utils.py` & `liechains-0.3.1/ether/utils.py`

 * *Files identical despite different names*

### Comparing `liechains-0.3.0/ether/wallet.py` & `liechains-0.3.1/ether/wallet.py`

 * *Files identical despite different names*

### Comparing `liechains-0.3.0/ether/ws.py` & `liechains-0.3.1/ether/ws.py`

 * *Files identical despite different names*

### Comparing `liechains-0.3.0/liechains.egg-info/SOURCES.txt` & `liechains-0.3.1/liechains.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 ether/chains.py
 ether/client.py
 ether/mev.py
 ether/utils.py
 ether/wallet.py
 ether/ws.py
 ether/dex/__init__.py
+ether/dex/balancer.py
+ether/dex/curve.py
+ether/dex/limit_order.py
 ether/dex/swap.py
 ether/dex/univ2.py
 ether/dex/univ3.py
 ether/flashbots/__init__.py
 ether/flashbots/blox.py
 ether/flashbots/flashbots.py
 ether/flashbots/middleware.py
```

### Comparing `liechains-0.3.0/setup.py` & `liechains-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="liechains",
-    version="0.3.0",
+    version="0.3.1",
     author="leeliewhite",
     author_email="leeliewhite@gmail.com",
     description="toolkit for blockchains",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

