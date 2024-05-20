# Comparing `tmp/elemento-cli-0.1.6.tar.gz` & `tmp/elemento-cli-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elemento-cli-0.1.6.tar", last modified: Fri Oct 20 16:44:25 2023, max compression
+gzip compressed data, was "elemento-cli-0.1.7.tar", last modified: Mon May 20 09:31:57 2024, max compression
```

## Comparing `elemento-cli-0.1.6.tar` & `elemento-cli-0.1.7.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-10-20 16:44:25.231322 elemento-cli-0.1.6/
--rw-r--r--   0 filippovalle   (501) staff       (20)     4893 2023-10-20 16:44:25.231194 elemento-cli-0.1.6/PKG-INFO
--rw-r--r--   0 filippovalle   (501) staff       (20)     4648 2023-07-21 15:54:48.000000 elemento-cli-0.1.6/README.md
--rw-r--r--   0 filippovalle   (501) staff       (20)     2772 2023-04-18 10:37:58.000000 elemento-cli-0.1.6/betterprinttable.py
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-10-20 16:44:25.221102 elemento-cli-0.1.6/common/
--rw-r--r--   0 filippovalle   (501) staff       (20)      558 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/README.md
--rw-r--r--   0 filippovalle   (501) staff       (20)        0 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/__init__.py
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-10-20 16:44:25.221357 elemento-cli-0.1.6/common/lib/
--rw-r--r--   0 filippovalle   (501) staff       (20)        0 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/lib/__init__.py
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-10-20 16:44:25.221461 elemento-cli-0.1.6/common/lib/components/
--rw-r--r--   0 filippovalle   (501) staff       (20)       94 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/lib/components/__init__.py
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-10-20 16:44:25.223066 elemento-cli-0.1.6/common/lib/components/cpu/
--rw-r--r--   0 filippovalle   (501) staff       (20)      174 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/lib/components/cpu/__init__.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      127 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/lib/components/cpu/common.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     1824 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/lib/components/cpu/cpudescriptor.py
--rw-r--r--   0 filippovalle   (501) staff       (20)    88145 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/lib/components/cpu/cpuinfo.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      647 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/lib/components/cpu/cpumatcher.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     1443 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/lib/components/cpu/cpurequirements.py
--rw-r--r--   0 filippovalle   (501) staff       (20)    12275 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/lib/components/cpu/cpustatus.py
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-10-20 16:44:25.224320 elemento-cli-0.1.6/common/lib/components/cpu/tests/
--rwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/lib/components/cpu/tests/__init__.py
--rwxr-xr-x   0 filippovalle   (501) staff       (20)     5890 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/lib/components/cpu/tests/test_coresstatus.py
--rwxr-xr-x   0 filippovalle   (501) staff       (20)     7412 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/lib/components/cpu/tests/test_corestatus.py
--rwxr-xr-x   0 filippovalle   (501) staff       (20)      959 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/lib/components/cpu/tests/test_cpudescriptor.py
--rwxr-xr-x   0 filippovalle   (501) staff       (20)     2694 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/lib/components/cpu/tests/test_cpumatcher.py
--rwxr-xr-x   0 filippovalle   (501) staff       (20)     2105 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/lib/components/cpu/tests/test_cpustatus.py
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-10-20 16:44:25.224956 elemento-cli-0.1.6/common/lib/components/memory/
--rw-r--r--   0 filippovalle   (501) staff       (20)      134 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/lib/components/memory/__init__.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      788 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/lib/components/memory/memdescriptor.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      456 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/lib/components/memory/memmatcher.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      615 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/lib/components/memory/memrequirements.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     2405 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/lib/components/memory/memstatus.py
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-10-20 16:44:25.225524 elemento-cli-0.1.6/common/lib/components/misc/
--rw-r--r--   0 filippovalle   (501) staff       (20)       65 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/lib/components/misc/__init__.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      461 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/lib/components/misc/miscmatcher.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      609 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/lib/components/misc/miscrequirements.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     1525 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/lib/components/misc/miscstatus.py
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-10-20 16:44:25.226365 elemento-cli-0.1.6/common/lib/components/net/
--rw-r--r--   0 filippovalle   (501) staff       (20)       88 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/lib/components/net/__init__.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      449 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/lib/components/net/netmatcher.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     2016 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/lib/components/net/netrequirements.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     1909 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/lib/components/net/netspeed.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     7668 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/lib/components/net/netstatus.py
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-10-20 16:44:25.226970 elemento-cli-0.1.6/common/lib/components/pcidev/
--rw-r--r--   0 filippovalle   (501) staff       (20)       68 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/lib/components/pcidev/__init__.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      456 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/lib/components/pcidev/pcimatcher.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      940 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/lib/components/pcidev/pcirequirements.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     7024 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/lib/components/pcidev/pcistatus.py
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-10-20 16:44:25.227895 elemento-cli-0.1.6/common/lib/components/pcidev/tests/
--rwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/lib/components/pcidev/tests/__init__.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     1037 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/lib/components/pcidev/tests/test_pciaddress.py
--rwxr-xr-x   0 filippovalle   (501) staff       (20)      747 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/lib/components/pcidev/tests/test_pcidevice.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      785 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/lib/components/pcidev/tests/test_pcimatcher.py
--rwxr-xr-x   0 filippovalle   (501) staff       (20)      682 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/lib/components/pcidev/tests/test_pcirequirements.py
--rwxr-xr-x   0 filippovalle   (501) staff       (20)      793 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/lib/components/pcidev/tests/test_pciscanner.py
--rwxr-xr-x   0 filippovalle   (501) staff       (20)     2481 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/lib/components/pcidev/tests/test_pcistatus.py
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-10-20 16:44:25.228421 elemento-cli-0.1.6/common/lib/system/
--rw-r--r--   0 filippovalle   (501) staff       (20)      108 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/lib/system/__init__.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      565 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/lib/system/systemmatcher.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     1416 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/lib/system/systemrequirements.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     6528 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/lib/system/systemstatus.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      106 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/requirements.txt
--rwxr-xr-x   0 filippovalle   (501) staff       (20)      167 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/common/run_tests.sh
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-10-20 16:44:25.229174 elemento-cli-0.1.6/ecd/
--rw-r--r--   0 filippovalle   (501) staff       (20)        0 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/ecd/__init__.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      677 2022-11-25 10:13:55.000000 elemento-cli-0.1.6/ecd/networking.json
--rw-r--r--   0 filippovalle   (501) staff       (20)      222 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/ecd/networking.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     1104 2022-11-25 10:13:32.000000 elemento-cli-0.1.6/ecd/restkeys.json
--rw-r--r--   0 filippovalle   (501) staff       (20)      222 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/ecd/restkeys.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      148 2022-11-10 10:08:31.000000 elemento-cli-0.1.6/ecd/test.py
--rwxr-xr-x   0 filippovalle   (501) staff       (20)     5790 2023-04-18 10:37:58.000000 elemento-cli-0.1.6/elemento
--rwxr-xr-x   0 filippovalle   (501) staff       (20)     5790 2023-04-18 10:37:58.000000 elemento-cli-0.1.6/elemento.py
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-10-20 16:44:25.229704 elemento-cli-0.1.6/elemento_cli.egg-info/
--rw-r--r--   0 filippovalle   (501) staff       (20)     4893 2023-10-20 16:44:25.000000 elemento-cli-0.1.6/elemento_cli.egg-info/PKG-INFO
--rw-r--r--   0 filippovalle   (501) staff       (20)     2472 2023-10-20 16:44:25.000000 elemento-cli-0.1.6/elemento_cli.egg-info/SOURCES.txt
--rw-r--r--   0 filippovalle   (501) staff       (20)        1 2023-10-20 16:44:25.000000 elemento-cli-0.1.6/elemento_cli.egg-info/dependency_links.txt
--rw-r--r--   0 filippovalle   (501) staff       (20)       84 2023-10-20 16:44:25.000000 elemento-cli-0.1.6/elemento_cli.egg-info/requires.txt
--rw-r--r--   0 filippovalle   (501) staff       (20)       20 2023-10-20 16:44:25.000000 elemento-cli-0.1.6/elemento_cli.egg-info/top_level.txt
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-10-20 16:44:25.230836 elemento-cli-0.1.6/handlers/
--rw-r--r--   0 filippovalle   (501) staff       (20)     2168 2023-03-17 11:00:12.000000 elemento-cli-0.1.6/handlers/__init__.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     6781 2023-03-17 11:00:12.000000 elemento-cli-0.1.6/handlers/account.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     3261 2023-03-17 11:00:12.000000 elemento-cli-0.1.6/handlers/iso.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     6871 2023-03-17 11:00:12.000000 elemento-cli-0.1.6/handlers/login.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     6950 2023-03-17 11:00:12.000000 elemento-cli-0.1.6/handlers/network.py
--rw-r--r--   0 filippovalle   (501) staff       (20)    13353 2023-10-20 16:44:17.000000 elemento-cli-0.1.6/handlers/vm.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     9397 2023-09-28 15:15:54.000000 elemento-cli-0.1.6/handlers/volumes.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     3888 2023-09-28 15:15:54.000000 elemento-cli-0.1.6/headers.py
--rw-r--r--   0 filippovalle   (501) staff       (20)       38 2023-10-20 16:44:25.231365 elemento-cli-0.1.6/setup.cfg
--rw-r--r--   0 filippovalle   (501) staff       (20)     2972 2023-10-20 16:44:24.000000 elemento-cli-0.1.6/setup.py
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2024-05-20 09:31:57.536775 elemento-cli-0.1.7/
+-rw-r--r--   0 filippovalle   (501) staff       (20)     4913 2024-05-20 09:31:57.536660 elemento-cli-0.1.7/PKG-INFO
+-rw-r--r--   0 filippovalle   (501) staff       (20)     4648 2023-07-21 15:54:48.000000 elemento-cli-0.1.7/README.md
+-rw-r--r--   0 filippovalle   (501) staff       (20)     2772 2023-04-18 10:37:58.000000 elemento-cli-0.1.7/betterprinttable.py
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2024-05-20 09:31:57.525546 elemento-cli-0.1.7/common/
+-rw-r--r--   0 filippovalle   (501) staff       (20)      558 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/README.md
+-rw-r--r--   0 filippovalle   (501) staff       (20)        0 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/__init__.py
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2024-05-20 09:31:57.525880 elemento-cli-0.1.7/common/lib/
+-rw-r--r--   0 filippovalle   (501) staff       (20)        0 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/lib/__init__.py
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2024-05-20 09:31:57.526003 elemento-cli-0.1.7/common/lib/components/
+-rw-r--r--   0 filippovalle   (501) staff       (20)       94 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/lib/components/__init__.py
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2024-05-20 09:31:57.527665 elemento-cli-0.1.7/common/lib/components/cpu/
+-rw-r--r--   0 filippovalle   (501) staff       (20)      174 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/lib/components/cpu/__init__.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      127 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/lib/components/cpu/common.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     1824 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/lib/components/cpu/cpudescriptor.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)    88145 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/lib/components/cpu/cpuinfo.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      647 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/lib/components/cpu/cpumatcher.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     1443 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/lib/components/cpu/cpurequirements.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)    12275 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/lib/components/cpu/cpustatus.py
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2024-05-20 09:31:57.528925 elemento-cli-0.1.7/common/lib/components/cpu/tests/
+-rwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/lib/components/cpu/tests/__init__.py
+-rwxr-xr-x   0 filippovalle   (501) staff       (20)     5890 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/lib/components/cpu/tests/test_coresstatus.py
+-rwxr-xr-x   0 filippovalle   (501) staff       (20)     7412 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/lib/components/cpu/tests/test_corestatus.py
+-rwxr-xr-x   0 filippovalle   (501) staff       (20)      959 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/lib/components/cpu/tests/test_cpudescriptor.py
+-rwxr-xr-x   0 filippovalle   (501) staff       (20)     2694 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/lib/components/cpu/tests/test_cpumatcher.py
+-rwxr-xr-x   0 filippovalle   (501) staff       (20)     2105 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/lib/components/cpu/tests/test_cpustatus.py
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2024-05-20 09:31:57.529702 elemento-cli-0.1.7/common/lib/components/memory/
+-rw-r--r--   0 filippovalle   (501) staff       (20)      134 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/lib/components/memory/__init__.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      788 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/lib/components/memory/memdescriptor.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      456 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/lib/components/memory/memmatcher.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      615 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/lib/components/memory/memrequirements.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     2405 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/lib/components/memory/memstatus.py
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2024-05-20 09:31:57.530322 elemento-cli-0.1.7/common/lib/components/misc/
+-rw-r--r--   0 filippovalle   (501) staff       (20)       65 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/lib/components/misc/__init__.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      461 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/lib/components/misc/miscmatcher.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      609 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/lib/components/misc/miscrequirements.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     1525 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/lib/components/misc/miscstatus.py
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2024-05-20 09:31:57.531025 elemento-cli-0.1.7/common/lib/components/net/
+-rw-r--r--   0 filippovalle   (501) staff       (20)       88 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/lib/components/net/__init__.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      449 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/lib/components/net/netmatcher.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     2016 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/lib/components/net/netrequirements.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     1909 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/lib/components/net/netspeed.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     7668 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/lib/components/net/netstatus.py
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2024-05-20 09:31:57.531687 elemento-cli-0.1.7/common/lib/components/pcidev/
+-rw-r--r--   0 filippovalle   (501) staff       (20)       68 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/lib/components/pcidev/__init__.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      456 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/lib/components/pcidev/pcimatcher.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      940 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/lib/components/pcidev/pcirequirements.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     7024 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/lib/components/pcidev/pcistatus.py
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2024-05-20 09:31:57.532804 elemento-cli-0.1.7/common/lib/components/pcidev/tests/
+-rwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/lib/components/pcidev/tests/__init__.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     1037 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/lib/components/pcidev/tests/test_pciaddress.py
+-rwxr-xr-x   0 filippovalle   (501) staff       (20)      747 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/lib/components/pcidev/tests/test_pcidevice.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      785 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/lib/components/pcidev/tests/test_pcimatcher.py
+-rwxr-xr-x   0 filippovalle   (501) staff       (20)      682 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/lib/components/pcidev/tests/test_pcirequirements.py
+-rwxr-xr-x   0 filippovalle   (501) staff       (20)      793 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/lib/components/pcidev/tests/test_pciscanner.py
+-rwxr-xr-x   0 filippovalle   (501) staff       (20)     2481 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/lib/components/pcidev/tests/test_pcistatus.py
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2024-05-20 09:31:57.533434 elemento-cli-0.1.7/common/lib/system/
+-rw-r--r--   0 filippovalle   (501) staff       (20)      108 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/lib/system/__init__.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      565 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/lib/system/systemmatcher.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     1416 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/lib/system/systemrequirements.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     6528 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/lib/system/systemstatus.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      106 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/requirements.txt
+-rwxr-xr-x   0 filippovalle   (501) staff       (20)      167 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/common/run_tests.sh
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2024-05-20 09:31:57.534321 elemento-cli-0.1.7/ecd/
+-rw-r--r--   0 filippovalle   (501) staff       (20)        0 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/ecd/__init__.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      677 2022-11-25 10:13:55.000000 elemento-cli-0.1.7/ecd/networking.json
+-rw-r--r--   0 filippovalle   (501) staff       (20)      222 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/ecd/networking.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     1104 2022-11-25 10:13:32.000000 elemento-cli-0.1.7/ecd/restkeys.json
+-rw-r--r--   0 filippovalle   (501) staff       (20)      222 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/ecd/restkeys.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      148 2022-11-10 10:08:31.000000 elemento-cli-0.1.7/ecd/test.py
+-rwxr-xr-x   0 filippovalle   (501) staff       (20)     5790 2023-04-18 10:37:58.000000 elemento-cli-0.1.7/elemento
+-rwxr-xr-x   0 filippovalle   (501) staff       (20)     5790 2023-04-18 10:37:58.000000 elemento-cli-0.1.7/elemento.py
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2024-05-20 09:31:57.534927 elemento-cli-0.1.7/elemento_cli.egg-info/
+-rw-r--r--   0 filippovalle   (501) staff       (20)     4913 2024-05-20 09:31:57.000000 elemento-cli-0.1.7/elemento_cli.egg-info/PKG-INFO
+-rw-r--r--   0 filippovalle   (501) staff       (20)     2472 2024-05-20 09:31:57.000000 elemento-cli-0.1.7/elemento_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 filippovalle   (501) staff       (20)        1 2024-05-20 09:31:57.000000 elemento-cli-0.1.7/elemento_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 filippovalle   (501) staff       (20)      101 2024-05-20 09:31:57.000000 elemento-cli-0.1.7/elemento_cli.egg-info/requires.txt
+-rw-r--r--   0 filippovalle   (501) staff       (20)       20 2024-05-20 09:31:57.000000 elemento-cli-0.1.7/elemento_cli.egg-info/top_level.txt
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2024-05-20 09:31:57.536304 elemento-cli-0.1.7/handlers/
+-rw-r--r--   0 filippovalle   (501) staff       (20)     2168 2023-03-17 11:00:12.000000 elemento-cli-0.1.7/handlers/__init__.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     6781 2023-03-17 11:00:12.000000 elemento-cli-0.1.7/handlers/account.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     3261 2023-03-17 11:00:12.000000 elemento-cli-0.1.7/handlers/iso.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     6871 2023-03-17 11:00:12.000000 elemento-cli-0.1.7/handlers/login.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     6950 2023-03-17 11:00:12.000000 elemento-cli-0.1.7/handlers/network.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)    13353 2023-10-20 16:49:35.000000 elemento-cli-0.1.7/handlers/vm.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     9397 2023-09-28 15:15:54.000000 elemento-cli-0.1.7/handlers/volumes.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     3888 2023-09-28 15:15:54.000000 elemento-cli-0.1.7/headers.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)       38 2024-05-20 09:31:57.536814 elemento-cli-0.1.7/setup.cfg
+-rw-r--r--   0 filippovalle   (501) staff       (20)     3009 2024-05-20 09:30:23.000000 elemento-cli-0.1.7/setup.py
```

### Comparing `elemento-cli-0.1.6/PKG-INFO` & `elemento-cli-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: elemento-cli
-Version: 0.1.6
+Version: 0.1.7
 Summary: CLI for Elemento
 Home-page: https://elemento.cloud
 Author: Elemento
 Author-email: hello@elemento.cloud
 License: GPL
+Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 <br/>
 <br/>
 <br/>
 <img src="https://raw.githubusercontent.com/Elemento-Modular-Cloud/graphic-assets/main/logos/horizontal/Logo%20horizontal%20lightbg%20transp.svg" width=50%/>
@@ -174,7 +175,9 @@
 
 Check the status of your service `sudo systemctl status elementolicensing`
 
 
 # Doubts? Need help?
 
 Open an *issue* in our [helpcenter](https://github.com/Elemento-Modular-Cloud/helpcenter)
+
+
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: elemento-cli Version: 0.1.6 Summary: CLI for
+Metadata-Version: 2.1 Name: elemento-cli Version: 0.1.7 Summary: CLI for
 Elemento Home-page: https://elemento.cloud Author: Elemento Author-email:
-hello@elemento.cloud License: GPL Requires-Python: >=3.9 Description-Content-
-Type: text/markdown
+hello@elemento.cloud License: GPL Platform: UNKNOWN Requires-Python: >=3.9
+Description-Content-Type: text/markdown
 
 
 [https://raw.githubusercontent.com/Elemento-Modular-Cloud/graphic-assets/main/
 logos/horizontal/Logo%20horizontal%20lightbg%20transp.svg]
 # Elemento command line overview ###### tags: `elemento` `CLI` `tech` `CTO`
 `tutorials`
 # Elemento command line overview ## Authentication Before using the Elemento
```

### Comparing `elemento-cli-0.1.6/README.md` & `elemento-cli-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/betterprinttable.py` & `elemento-cli-0.1.7/betterprinttable.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/common/README.md` & `elemento-cli-0.1.7/common/README.md`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/common/lib/components/cpu/cpudescriptor.py` & `elemento-cli-0.1.7/common/lib/components/cpu/cpudescriptor.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/common/lib/components/cpu/cpuinfo.py` & `elemento-cli-0.1.7/common/lib/components/cpu/cpuinfo.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/common/lib/components/cpu/cpumatcher.py` & `elemento-cli-0.1.7/common/lib/components/cpu/cpumatcher.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/common/lib/components/cpu/cpurequirements.py` & `elemento-cli-0.1.7/common/lib/components/cpu/cpurequirements.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/common/lib/components/cpu/cpustatus.py` & `elemento-cli-0.1.7/common/lib/components/cpu/cpustatus.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/common/lib/components/cpu/tests/test_coresstatus.py` & `elemento-cli-0.1.7/common/lib/components/cpu/tests/test_coresstatus.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/common/lib/components/cpu/tests/test_corestatus.py` & `elemento-cli-0.1.7/common/lib/components/cpu/tests/test_corestatus.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/common/lib/components/cpu/tests/test_cpudescriptor.py` & `elemento-cli-0.1.7/common/lib/components/cpu/tests/test_cpudescriptor.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/common/lib/components/cpu/tests/test_cpumatcher.py` & `elemento-cli-0.1.7/common/lib/components/cpu/tests/test_cpumatcher.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/common/lib/components/cpu/tests/test_cpustatus.py` & `elemento-cli-0.1.7/common/lib/components/cpu/tests/test_cpustatus.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/common/lib/components/memory/memdescriptor.py` & `elemento-cli-0.1.7/common/lib/components/memory/memdescriptor.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/common/lib/components/memory/memrequirements.py` & `elemento-cli-0.1.7/common/lib/components/memory/memrequirements.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/common/lib/components/memory/memstatus.py` & `elemento-cli-0.1.7/common/lib/components/memory/memstatus.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/common/lib/components/misc/miscrequirements.py` & `elemento-cli-0.1.7/common/lib/components/misc/miscrequirements.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/common/lib/components/misc/miscstatus.py` & `elemento-cli-0.1.7/common/lib/components/misc/miscstatus.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/common/lib/components/net/netrequirements.py` & `elemento-cli-0.1.7/common/lib/components/net/netrequirements.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/common/lib/components/net/netspeed.py` & `elemento-cli-0.1.7/common/lib/components/net/netspeed.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/common/lib/components/net/netstatus.py` & `elemento-cli-0.1.7/common/lib/components/net/netstatus.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/common/lib/components/pcidev/pcirequirements.py` & `elemento-cli-0.1.7/common/lib/components/pcidev/pcirequirements.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/common/lib/components/pcidev/pcistatus.py` & `elemento-cli-0.1.7/common/lib/components/pcidev/pcistatus.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/common/lib/components/pcidev/tests/test_pciaddress.py` & `elemento-cli-0.1.7/common/lib/components/pcidev/tests/test_pciaddress.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/common/lib/components/pcidev/tests/test_pcidevice.py` & `elemento-cli-0.1.7/common/lib/components/pcidev/tests/test_pcidevice.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/common/lib/components/pcidev/tests/test_pcimatcher.py` & `elemento-cli-0.1.7/common/lib/components/pcidev/tests/test_pcimatcher.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/common/lib/components/pcidev/tests/test_pcirequirements.py` & `elemento-cli-0.1.7/common/lib/components/pcidev/tests/test_pcirequirements.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/common/lib/components/pcidev/tests/test_pciscanner.py` & `elemento-cli-0.1.7/common/lib/components/pcidev/tests/test_pciscanner.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/common/lib/components/pcidev/tests/test_pcistatus.py` & `elemento-cli-0.1.7/common/lib/components/pcidev/tests/test_pcistatus.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/common/lib/system/systemmatcher.py` & `elemento-cli-0.1.7/common/lib/system/systemmatcher.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/common/lib/system/systemrequirements.py` & `elemento-cli-0.1.7/common/lib/system/systemrequirements.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/common/lib/system/systemstatus.py` & `elemento-cli-0.1.7/common/lib/system/systemstatus.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/ecd/networking.json` & `elemento-cli-0.1.7/ecd/networking.json`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/ecd/restkeys.json` & `elemento-cli-0.1.7/ecd/restkeys.json`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/elemento` & `elemento-cli-0.1.7/elemento`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/elemento.py` & `elemento-cli-0.1.7/elemento.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/elemento_cli.egg-info/PKG-INFO` & `elemento-cli-0.1.7/elemento_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: elemento-cli
-Version: 0.1.6
+Version: 0.1.7
 Summary: CLI for Elemento
 Home-page: https://elemento.cloud
 Author: Elemento
 Author-email: hello@elemento.cloud
 License: GPL
+Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 <br/>
 <br/>
 <br/>
 <img src="https://raw.githubusercontent.com/Elemento-Modular-Cloud/graphic-assets/main/logos/horizontal/Logo%20horizontal%20lightbg%20transp.svg" width=50%/>
@@ -174,7 +175,9 @@
 
 Check the status of your service `sudo systemctl status elementolicensing`
 
 
 # Doubts? Need help?
 
 Open an *issue* in our [helpcenter](https://github.com/Elemento-Modular-Cloud/helpcenter)
+
+
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: elemento-cli Version: 0.1.6 Summary: CLI for
+Metadata-Version: 2.1 Name: elemento-cli Version: 0.1.7 Summary: CLI for
 Elemento Home-page: https://elemento.cloud Author: Elemento Author-email:
-hello@elemento.cloud License: GPL Requires-Python: >=3.9 Description-Content-
-Type: text/markdown
+hello@elemento.cloud License: GPL Platform: UNKNOWN Requires-Python: >=3.9
+Description-Content-Type: text/markdown
 
 
 [https://raw.githubusercontent.com/Elemento-Modular-Cloud/graphic-assets/main/
 logos/horizontal/Logo%20horizontal%20lightbg%20transp.svg]
 # Elemento command line overview ###### tags: `elemento` `CLI` `tech` `CTO`
 `tutorials`
 # Elemento command line overview ## Authentication Before using the Elemento
```

### Comparing `elemento-cli-0.1.6/elemento_cli.egg-info/SOURCES.txt` & `elemento-cli-0.1.7/elemento_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/handlers/__init__.py` & `elemento-cli-0.1.7/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/handlers/account.py` & `elemento-cli-0.1.7/handlers/account.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/handlers/iso.py` & `elemento-cli-0.1.7/handlers/iso.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/handlers/login.py` & `elemento-cli-0.1.7/handlers/login.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/handlers/network.py` & `elemento-cli-0.1.7/handlers/network.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/handlers/vm.py` & `elemento-cli-0.1.7/handlers/vm.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/handlers/volumes.py` & `elemento-cli-0.1.7/handlers/volumes.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/headers.py` & `elemento-cli-0.1.7/headers.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.6/setup.py` & `elemento-cli-0.1.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="elemento-cli",
-    version="0.1.6",
+    version="0.1.7",
     author="Elemento",
     author_email="hello@elemento.cloud",
     description="CLI for Elemento",
     license="GPL",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://elemento.cloud",
@@ -45,17 +45,19 @@
     include_package_data=True,
     scripts=['elemento.py', 'elemento', "headers.py", "betterprinttable.py"],
     package_data={
         ".":["headers.py"],
         "ecd":["*"],
         "common": ["*"],
         "handlers": ["*.py"]},
-    install_requires = ["argparse", 
+    install_requires = [
+        "argparse", 
         "argcomplete", 
         "tabulate", 
-        "si_prefix",
         "jsonpickle",
-        "requests",
+        "pyasyncore",
         "pwinput",
+        "requests",
+        "si_prefix===1.0",
         "urllib3==1.26.6"],
     python_requires='>=3.9',
 )
```

