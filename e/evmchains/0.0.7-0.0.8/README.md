# Comparing `tmp/evmchains-0.0.7.tar.gz` & `tmp/evmchains-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evmchains-0.0.7.tar", last modified: Thu Apr 18 20:26:20 2024, max compression
+gzip compressed data, was "evmchains-0.0.8.tar", last modified: Mon May 20 15:07:10 2024, max compression
```

## Comparing `evmchains-0.0.7.tar` & `evmchains-0.0.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:26:20.070538 evmchains-0.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:26:20.062538 evmchains-0.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:26:20.066537 evmchains-0.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-18 20:26:03.000000 evmchains-0.0.7/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-18 20:26:03.000000 evmchains-0.0.7/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-18 20:26:03.000000 evmchains-0.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-18 20:26:03.000000 evmchains-0.0.7/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-18 20:26:03.000000 evmchains-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15775 2024-04-18 20:26:20.070538 evmchains-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-18 20:26:03.000000 evmchains-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:26:20.066537 evmchains-0.0.7/evmchains/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-18 20:26:03.000000 evmchains-0.0.7/evmchains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-18 20:26:19.000000 evmchains-0.0.7/evmchains/_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)    33001 2024-04-18 20:26:03.000000 evmchains-0.0.7/evmchains/chains.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:26:03.000000 evmchains-0.0.7/evmchains/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-18 20:26:03.000000 evmchains-0.0.7/evmchains/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:26:20.066537 evmchains-0.0.7/evmchains.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15775 2024-04-18 20:26:20.000000 evmchains-0.0.7/evmchains.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-18 20:26:20.000000 evmchains-0.0.7/evmchains.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 20:26:20.000000 evmchains-0.0.7/evmchains.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-18 20:26:20.000000 evmchains-0.0.7/evmchains.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-18 20:26:20.000000 evmchains-0.0.7/evmchains.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-18 20:26:03.000000 evmchains-0.0.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:26:20.066537 evmchains-0.0.7/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-04-18 20:26:03.000000 evmchains-0.0.7/scripts/update.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-18 20:26:20.070538 evmchains-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-18 20:26:03.000000 evmchains-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:26:20.066537 evmchains-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-18 20:26:03.000000 evmchains-0.0.7/tests/test_func.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:07:10.545918 evmchains-0.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:07:10.541918 evmchains-0.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:07:10.541918 evmchains-0.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-20 15:06:53.000000 evmchains-0.0.8/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-20 15:06:53.000000 evmchains-0.0.8/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-20 15:06:53.000000 evmchains-0.0.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-20 15:06:53.000000 evmchains-0.0.8/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-20 15:06:53.000000 evmchains-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15775 2024-05-20 15:07:10.545918 evmchains-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-20 15:06:53.000000 evmchains-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:07:10.541918 evmchains-0.0.8/evmchains/
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-20 15:06:53.000000 evmchains-0.0.8/evmchains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-20 15:07:10.000000 evmchains-0.0.8/evmchains/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35091 2024-05-20 15:06:53.000000 evmchains-0.0.8/evmchains/chains.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:06:53.000000 evmchains-0.0.8/evmchains/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-20 15:06:53.000000 evmchains-0.0.8/evmchains/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:07:10.545918 evmchains-0.0.8/evmchains.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15775 2024-05-20 15:07:10.000000 evmchains-0.0.8/evmchains.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-20 15:07:10.000000 evmchains-0.0.8/evmchains.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 15:07:10.000000 evmchains-0.0.8/evmchains.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-20 15:07:10.000000 evmchains-0.0.8/evmchains.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 15:07:10.000000 evmchains-0.0.8/evmchains.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-20 15:06:53.000000 evmchains-0.0.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:07:10.545918 evmchains-0.0.8/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-05-20 15:06:53.000000 evmchains-0.0.8/scripts/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-20 15:07:10.545918 evmchains-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-20 15:06:53.000000 evmchains-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:07:10.545918 evmchains-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-20 15:06:53.000000 evmchains-0.0.8/tests/test_func.py
```

### Comparing `evmchains-0.0.7/.github/workflows/release.yaml` & `evmchains-0.0.8/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `evmchains-0.0.7/.github/workflows/test.yaml` & `evmchains-0.0.8/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `evmchains-0.0.7/.gitignore` & `evmchains-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `evmchains-0.0.7/CONTRIBUTING.md` & `evmchains-0.0.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `evmchains-0.0.7/LICENSE` & `evmchains-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `evmchains-0.0.7/PKG-INFO` & `evmchains-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evmchains
-Version: 0.0.7
+Version: 0.0.8
 Summary: Packaged metadata on Ethereum Virtual Machine (EVM) chains
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `evmchains-0.0.7/README.md` & `evmchains-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `evmchains-0.0.7/evmchains/__init__.py` & `evmchains-0.0.8/evmchains/__init__.py`

 * *Files identical despite different names*

### Comparing `evmchains-0.0.7/evmchains/chains.py` & `evmchains-0.0.8/evmchains/chains.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This file is auto-generated by scripts/update.py
-# 2024-04-09 14:08:35.326760
+# 2024-05-17 16:06:29.822636
 # Do not edit this file directly.
 from typing import Any, Dict
 
 PUBLIC_CHAIN_META: Dict[str, Dict[str, Dict[str, Any]]] = {
     "arbitrum": {
         "mainnet": {
             "chain": "ETH",
@@ -486,14 +486,15 @@
                 "https://rpc2.sepolia.org",
                 "https://rpc-sepolia.rockx.com",
                 "https://rpc.sepolia.ethpandaops.io",
                 "https://sepolia.infura.io/v3/${INFURA_API_KEY}",
                 "https://sepolia.gateway.tenderly.co",
                 "https://ethereum-sepolia-rpc.publicnode.com",
                 "https://sepolia.drpc.org",
+                "https://rpc-sepolia.rockx.com",
             ],
             "shortName": "sep",
             "slip44": 1,
         },
     },
     "fantom": {
         "mainnet": {
@@ -936,8 +937,71 @@
                 "https://rpc.sepolia.linea.build",
                 "https://linea-sepolia.infura.io/v3/${INFURA_API_KEY}",
             ],
             "shortName": "linea-sepolia",
             "slip44": 1,
         },
     },
+    "rootstock": {
+        "mainnet": {
+            "chain": "Rootstock",
+            "chainId": 30,
+            "ens": None,
+            "explorers": [
+                {
+                    "name": "Rootstock Explorer",
+                    "standard": "EIP3091",
+                    "url": "https://explorer.rsk.co",
+                },
+                {
+                    "icon": "blockscout",
+                    "name": "blockscout",
+                    "standard": "EIP3091",
+                    "url": "https://rootstock.blockscout.com",
+                },
+            ],
+            "faucets": [],
+            "features": None,
+            "icon": "rootstock",
+            "infoURL": "https://rootstock.io",
+            "name": "Rootstock Mainnet",
+            "nativeCurrency": {
+                "decimals": 18,
+                "name": "Smart Bitcoin",
+                "symbol": "RBTC",
+            },
+            "networkId": 30,
+            "rpc": ["https://public-node.rsk.co", "https://mycrypto.rsk.co"],
+            "shortName": "rsk",
+            "slip44": 137,
+        },
+        "testnet": {
+            "chain": "Rootstock",
+            "chainId": 31,
+            "ens": None,
+            "explorers": [
+                {
+                    "name": "RSK Testnet Explorer",
+                    "standard": "EIP3091",
+                    "url": "https://explorer.testnet.rsk.co",
+                }
+            ],
+            "faucets": ["https://faucet.rsk.co/"],
+            "features": None,
+            "icon": "rootstock",
+            "infoURL": "https://rootstock.io",
+            "name": "Rootstock Testnet",
+            "nativeCurrency": {
+                "decimals": 18,
+                "name": "Testnet Smart Bitcoin",
+                "symbol": "tRBTC",
+            },
+            "networkId": 31,
+            "rpc": [
+                "https://public-node.testnet.rsk.co",
+                "https://mycrypto.testnet.rsk.co",
+            ],
+            "shortName": "trsk",
+            "slip44": 1,
+        },
+    },
 }
```

### Comparing `evmchains-0.0.7/evmchains.egg-info/PKG-INFO` & `evmchains-0.0.8/evmchains.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evmchains
-Version: 0.0.7
+Version: 0.0.8
 Summary: Packaged metadata on Ethereum Virtual Machine (EVM) chains
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `evmchains-0.0.7/pyproject.toml` & `evmchains-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `evmchains-0.0.7/scripts/update.py` & `evmchains-0.0.8/scripts/update.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,18 @@
         "mainnet": 1101,
         "testnet": 1442,
     },
     "linea": {
         "mainnet": 59144,
         "sepolia": 59141,
     },
+    "rootstock": {
+        "mainnet": 30,
+        "testnet": 31,
+    },
 }
 
 pp = PrettyPrinter(indent=4)
 logger = logging.getLogger("update")
 logger.setLevel(logging.DEBUG)
```

### Comparing `evmchains-0.0.7/tests/test_func.py` & `evmchains-0.0.8/tests/test_func.py`

 * *Files identical despite different names*

