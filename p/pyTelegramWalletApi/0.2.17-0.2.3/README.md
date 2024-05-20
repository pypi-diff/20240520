# Comparing `tmp/pyTelegramWalletApi-0.2.17.tar.gz` & `tmp/pyTelegramWalletApi-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyTelegramWalletApi-0.2.17.tar", last modified: Thu Apr  4 09:01:26 2024, max compression
+gzip compressed data, was "pyTelegramWalletApi-0.2.3.tar", last modified: Mon May 20 02:14:37 2024, max compression
```

## Comparing `pyTelegramWalletApi-0.2.17.tar` & `pyTelegramWalletApi-0.2.3.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 09:01:26.066820 pyTelegramWalletApi-0.2.17/
--rw-rw-rw-   0        0        0     2462 2024-04-04 09:01:26.066820 pyTelegramWalletApi-0.2.17/PKG-INFO
--rw-rw-rw-   0        0        0     2259 2024-04-04 09:00:44.000000 pyTelegramWalletApi-0.2.17/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 09:01:26.023818 pyTelegramWalletApi-0.2.17/pyTelegramWalletApi.egg-info/
--rw-rw-rw-   0        0        0     2462 2024-04-04 09:01:25.000000 pyTelegramWalletApi-0.2.17/pyTelegramWalletApi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      388 2024-04-04 09:01:25.000000 pyTelegramWalletApi-0.2.17/pyTelegramWalletApi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 09:01:25.000000 pyTelegramWalletApi-0.2.17/pyTelegramWalletApi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-04 09:01:25.000000 pyTelegramWalletApi-0.2.17/pyTelegramWalletApi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-04 09:01:25.000000 pyTelegramWalletApi-0.2.17/pyTelegramWalletApi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-04 09:01:26.074819 pyTelegramWalletApi-0.2.17/setup.cfg
--rw-rw-rw-   0        0        0      572 2024-04-04 09:00:44.000000 pyTelegramWalletApi-0.2.17/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 09:01:26.030819 pyTelegramWalletApi-0.2.17/tests/
--rw-rw-rw-   0        0        0        0 2023-10-02 22:55:55.000000 pyTelegramWalletApi-0.2.17/tests/__init__.py
--rw-rw-rw-   0        0        0     1513 2024-04-04 08:56:55.000000 pyTelegramWalletApi-0.2.17/tests/rest_tests.py
-drwxrwxrwx   0        0        0        0 2024-04-04 09:01:26.049821 pyTelegramWalletApi-0.2.17/wallet/
--rw-rw-rw-   0        0        0       70 2023-10-02 23:59:27.000000 pyTelegramWalletApi-0.2.17/wallet/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 09:01:26.052820 pyTelegramWalletApi-0.2.17/wallet/rest/
--rw-rw-rw-   0        0        0    14517 2023-10-22 06:53:53.000000 pyTelegramWalletApi-0.2.17/wallet/rest/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 09:01:26.064819 pyTelegramWalletApi-0.2.17/wallet/selenium/
--rw-rw-rw-   0        0        0      719 2023-10-19 08:46:48.000000 pyTelegramWalletApi-0.2.17/wallet/selenium/__init__.py
--rw-rw-rw-   0        0        0     8322 2023-10-22 10:10:20.000000 pyTelegramWalletApi-0.2.17/wallet/types.py
--rw-rw-rw-   0        0        0     2288 2024-04-04 08:50:32.000000 pyTelegramWalletApi-0.2.17/wallet/web_client.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:14:37.089371 pyTelegramWalletApi-0.2.3/
+-rw-rw-rw-   0        0        0     4828 2024-05-20 02:14:37.089371 pyTelegramWalletApi-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4620 2024-05-20 02:11:16.000000 pyTelegramWalletApi-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 02:14:36.996367 pyTelegramWalletApi-0.2.3/pyTelegramWalletApi.egg-info/
+-rw-rw-rw-   0        0        0     4828 2024-05-20 02:14:36.000000 pyTelegramWalletApi-0.2.3/pyTelegramWalletApi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      481 2024-05-20 02:14:36.000000 pyTelegramWalletApi-0.2.3/pyTelegramWalletApi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 02:14:36.000000 pyTelegramWalletApi-0.2.3/pyTelegramWalletApi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-20 02:14:36.000000 pyTelegramWalletApi-0.2.3/pyTelegramWalletApi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-20 02:14:36.000000 pyTelegramWalletApi-0.2.3/pyTelegramWalletApi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 02:14:37.099372 pyTelegramWalletApi-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      571 2024-05-20 00:11:57.000000 pyTelegramWalletApi-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:14:37.041369 pyTelegramWalletApi-0.2.3/tests/
+-rw-rw-rw-   0        0        0        0 2023-10-02 22:55:55.000000 pyTelegramWalletApi-0.2.3/tests/__init__.py
+-rw-rw-rw-   0        0        0      902 2024-05-20 00:04:34.000000 pyTelegramWalletApi-0.2.3/tests/test_account.py
+-rw-rw-rw-   0        0        0     2680 2024-05-20 00:04:34.000000 pyTelegramWalletApi-0.2.3/tests/test_p2p.py
+-rw-rw-rw-   0        0        0      733 2024-05-20 00:05:20.000000 pyTelegramWalletApi-0.2.3/tests/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:14:37.048369 pyTelegramWalletApi-0.2.3/wallet/
+-rw-rw-rw-   0        0        0       70 2023-10-02 23:59:27.000000 pyTelegramWalletApi-0.2.3/wallet/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:14:37.052369 pyTelegramWalletApi-0.2.3/wallet/rest/
+-rw-rw-rw-   0        0        0    18205 2024-05-20 02:07:30.000000 pyTelegramWalletApi-0.2.3/wallet/rest/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:14:37.086371 pyTelegramWalletApi-0.2.3/wallet/types/
+-rw-rw-rw-   0        0        0      184 2024-05-19 04:12:35.000000 pyTelegramWalletApi-0.2.3/wallet/types/__init__.py
+-rw-rw-rw-   0        0        0      975 2024-05-18 18:26:30.000000 pyTelegramWalletApi-0.2.3/wallet/types/balances.py
+-rw-rw-rw-   0        0        0     4987 2024-05-19 20:06:10.000000 pyTelegramWalletApi-0.2.3/wallet/types/offers.py
+-rw-rw-rw-   0        0        0     3128 2024-05-18 23:18:10.000000 pyTelegramWalletApi-0.2.3/wallet/types/transactions.py
+-rw-rw-rw-   0        0        0     4201 2024-05-19 19:38:34.000000 pyTelegramWalletApi-0.2.3/wallet/web_client.py
```

### Comparing `pyTelegramWalletApi-0.2.17/setup.py` & `pyTelegramWalletApi-0.2.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 requirements = ["requests", "selenium-wire", "pytest"]
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='pyTelegramWalletApi',
-    version='0.2.17',
+    version='0.2.3',
     author='no-name-user-name',
     description='Telegram Wallet API',
     packages=find_packages(),
     install_requires=requirements,
     author_email='dimazver61@gmail.com',
     long_description=long_description,
     long_description_content_type='text/markdown'
```

