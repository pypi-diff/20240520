# Comparing `tmp/deepdog-1.2.1.tar.gz` & `tmp/deepdog-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepdog-1.2.1.tar", max compression
+gzip compressed data, was "deepdog-1.3.0.tar", max compression
```

## Comparing `deepdog-1.2.1.tar` & `deepdog-1.3.0.tar`

### file list

```diff
@@ -1,24 +1,28 @@
--rw-r--r--   0        0        0      366 2024-05-12 01:51:49.254232 deepdog-1.2.1/deepdog/__init__.py
--rw-r--r--   0        0        0        0 2024-05-12 01:51:49.254232 deepdog-1.2.1/deepdog/cli/__init__.py
--rw-r--r--   0        0        0       80 2024-05-12 01:51:49.254232 deepdog-1.2.1/deepdog/cli/probs/__init__.py
--rw-r--r--   0        0        0     1389 2024-05-12 01:51:49.254232 deepdog-1.2.1/deepdog/cli/probs/args.py
--rw-r--r--   0        0        0     6243 2024-05-12 01:51:49.254232 deepdog-1.2.1/deepdog/cli/probs/dicts.py
--rw-r--r--   0        0        0     2945 2024-05-12 01:51:49.254232 deepdog-1.2.1/deepdog/cli/probs/main.py
--rw-r--r--   0        0        0      161 2024-05-12 01:51:49.258232 deepdog-1.2.1/deepdog/direct_monte_carlo/__init__.py
--rw-r--r--   0        0        0      329 2024-05-12 01:52:16.423528 deepdog-1.2.1/deepdog/direct_monte_carlo/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     7897 2024-05-12 01:52:16.427528 deepdog-1.2.1/deepdog/direct_monte_carlo/__pycache__/direct_mc.cpython-39.pyc
--rw-r--r--   0        0        0     3902 2024-05-12 01:52:16.435528 deepdog-1.2.1/deepdog/direct_monte_carlo/__pycache__/dmc_filters.cpython-39.pyc
--rw-r--r--   0        0        0      461 2024-05-12 01:51:49.258232 deepdog-1.2.1/deepdog/direct_monte_carlo/compose_filter.py
--rw-r--r--   0        0        0     9338 2024-05-12 01:51:49.258232 deepdog-1.2.1/deepdog/direct_monte_carlo/direct_mc.py
--rw-r--r--   0        0        0     3393 2024-05-12 01:51:49.258232 deepdog-1.2.1/deepdog/direct_monte_carlo/dmc_filters.py
--rw-r--r--   0        0        0     1710 2024-05-12 01:51:49.258232 deepdog-1.2.1/deepdog/indexify/__init__.py
--rw-r--r--   0        0        0     2436 2024-05-12 01:52:16.511532 deepdog-1.2.1/deepdog/indexify/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0       73 2024-05-12 01:51:49.258232 deepdog-1.2.1/deepdog/meta.py
--rw-r--r--   0        0        0    12392 2024-05-12 01:51:49.258232 deepdog-1.2.1/deepdog/real_spectrum_run.py
--rw-r--r--   0        0        0     5869 2024-05-12 01:51:49.258232 deepdog-1.2.1/deepdog/results/__init__.py
--rw-r--r--   0        0        0     7172 2024-05-12 01:52:16.539533 deepdog-1.2.1/deepdog/results/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      110 2024-05-12 01:51:49.258232 deepdog-1.2.1/deepdog/subset_simulation/__init__.py
--rw-r--r--   0        0        0    11428 2024-05-12 01:51:49.258232 deepdog-1.2.1/deepdog/subset_simulation/subset_simulation_impl.py
--rw-r--r--   0        0        0     6794 2024-05-12 01:51:49.258232 deepdog-1.2.1/deepdog/temp_aware_real_spectrum_run.py
--rw-r--r--   0        0        0     1084 2024-05-12 01:51:49.258232 deepdog-1.2.1/pyproject.toml
--rw-r--r--   0        0        0      398 1970-01-01 00:00:00.000000 deepdog-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0      366 2024-05-20 03:14:22.918857 deepdog-1.3.0/deepdog/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-20 03:14:22.918857 deepdog-1.3.0/deepdog/cli/__init__.py
+-rw-r--r--   0        0        0       80 2024-05-20 03:14:22.918857 deepdog-1.3.0/deepdog/cli/probs/__init__.py
+-rw-r--r--   0        0        0     1389 2024-05-20 03:14:22.918857 deepdog-1.3.0/deepdog/cli/probs/args.py
+-rw-r--r--   0        0        0     6243 2024-05-20 03:14:22.918857 deepdog-1.3.0/deepdog/cli/probs/dicts.py
+-rw-r--r--   0        0        0     3010 2024-05-20 03:14:22.918857 deepdog-1.3.0/deepdog/cli/probs/main.py
+-rw-r--r--   0        0        0      161 2024-05-20 03:14:22.918857 deepdog-1.3.0/deepdog/direct_monte_carlo/__init__.py
+-rw-r--r--   0        0        0      329 2024-05-20 03:14:53.104389 deepdog-1.3.0/deepdog/direct_monte_carlo/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1072 2024-05-20 03:14:53.108389 deepdog-1.3.0/deepdog/direct_monte_carlo/__pycache__/cost_function_filter.cpython-39.pyc
+-rw-r--r--   0        0        0     7897 2024-05-20 03:14:53.108389 deepdog-1.3.0/deepdog/direct_monte_carlo/__pycache__/direct_mc.cpython-39.pyc
+-rw-r--r--   0        0        0     3902 2024-05-20 03:14:53.124390 deepdog-1.3.0/deepdog/direct_monte_carlo/__pycache__/dmc_filters.cpython-39.pyc
+-rw-r--r--   0        0        0      461 2024-05-20 03:14:22.918857 deepdog-1.3.0/deepdog/direct_monte_carlo/compose_filter.py
+-rw-r--r--   0        0        0      664 2024-05-20 03:14:22.918857 deepdog-1.3.0/deepdog/direct_monte_carlo/cost_function_filter.py
+-rw-r--r--   0        0        0     9338 2024-05-20 03:14:22.918857 deepdog-1.3.0/deepdog/direct_monte_carlo/direct_mc.py
+-rw-r--r--   0        0        0     3393 2024-05-20 03:14:22.918857 deepdog-1.3.0/deepdog/direct_monte_carlo/dmc_filters.py
+-rw-r--r--   0        0        0     1710 2024-05-20 03:14:22.918857 deepdog-1.3.0/deepdog/indexify/__init__.py
+-rw-r--r--   0        0        0     2436 2024-05-20 03:14:53.184394 deepdog-1.3.0/deepdog/indexify/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0       73 2024-05-20 03:14:22.918857 deepdog-1.3.0/deepdog/meta.py
+-rw-r--r--   0        0        0    12392 2024-05-20 03:14:22.918857 deepdog-1.3.0/deepdog/real_spectrum_run.py
+-rw-r--r--   0        0        0     5869 2024-05-20 03:14:22.918857 deepdog-1.3.0/deepdog/results/__init__.py
+-rw-r--r--   0        0        0     7172 2024-05-20 03:14:53.208395 deepdog-1.3.0/deepdog/results/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      110 2024-05-20 03:14:22.918857 deepdog-1.3.0/deepdog/subset_simulation/__init__.py
+-rw-r--r--   0        0        0      297 2024-05-20 03:14:53.256397 deepdog-1.3.0/deepdog/subset_simulation/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    14006 2024-05-20 03:14:53.264397 deepdog-1.3.0/deepdog/subset_simulation/__pycache__/subset_simulation_impl.cpython-39.pyc
+-rw-r--r--   0        0        0    19872 2024-05-20 03:14:22.918857 deepdog-1.3.0/deepdog/subset_simulation/subset_simulation_impl.py
+-rw-r--r--   0        0        0     6794 2024-05-20 03:14:22.918857 deepdog-1.3.0/deepdog/temp_aware_real_spectrum_run.py
+-rw-r--r--   0        0        0     1084 2024-05-20 03:14:22.918857 deepdog-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      398 1970-01-01 00:00:00.000000 deepdog-1.3.0/PKG-INFO
```

### Comparing `deepdog-1.2.1/deepdog/cli/probs/args.py` & `deepdog-1.3.0/deepdog/cli/probs/args.py`

 * *Files identical despite different names*

### Comparing `deepdog-1.2.1/deepdog/cli/probs/dicts.py` & `deepdog-1.3.0/deepdog/cli/probs/dicts.py`

 * *Files identical despite different names*

### Comparing `deepdog-1.2.1/deepdog/cli/probs/main.py` & `deepdog-1.3.0/deepdog/cli/probs/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 		)
 		# _logger.info(out_files)
 		parsed_output_files = [
 			deepdog.results.read_output_file(f, indexifier)
 			for f in tqdm.tqdm(out_files, desc="reading files", leave=False)
 		]
 
+		# Refactor here to allow for arbitrary likelihood file sources
 		_logger.info("building uncoalesced dict")
 		uncoalesced_dict = deepdog.cli.probs.dicts.build_model_dict(parsed_output_files)
 
 		if "uncoalesced_outfile" in args and args.uncoalesced_outfile:
 			deepdog.cli.probs.dicts.write_uncoalesced_dict(
 				args.uncoalesced_outfile, uncoalesced_dict
 			)
```

### Comparing `deepdog-1.2.1/deepdog/direct_monte_carlo/__pycache__/direct_mc.cpython-39.pyc` & `deepdog-1.3.0/deepdog/direct_monte_carlo/__pycache__/direct_mc.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun May 12 01:51:49 2024 UTC, .py size: 9338 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 b520 4066 7a24 0000  a........ @fz$..
+00000000: 610d 0d0a 0000 0000 0ec0 4a66 7a24 0000  a.........Jfz$..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 e400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c03 5a02 6400 6401 6c04 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c05 5a02 6400 6401 6c06 5a06 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6402 6c07 6d08 5a08 6d09 5a09 6d0a 5a0a  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0b 5a0b 6d0c 5a0c 0100 6400 6403 6c0d  m.Z.m.Z...d.d.l.
@@ -34,15 +34,15 @@
 00000210: 7175 616c 6e61 6d65 5f5f da03 696e 74da  qualname__..int.
 00000220: 0f5f 5f61 6e6e 6f74 6174 696f 6e73 5f5f  .__annotations__
 00000230: da05 666c 6f61 74da 0373 7472 a900 7214  ..float..str..r.
 00000240: 0000 0072 1400 0000 fa61 2f68 6f6d 652f  ...r.....a/home/
 00000250: 6a65 6e6b 696e 732f 6167 656e 742f 776f  jenkins/agent/wo
 00000260: 726b 7370 6163 652f 6769 7465 612d 7068  rkspace/gitea-ph
 00000270: 7973 6963 735f 6465 6570 646f 675f 312e  ysics_deepdog_1.
-00000280: 322e 312f 6465 6570 646f 672f 6469 7265  2.1/deepdog/dire
+00000280: 332e 302f 6465 6570 646f 672f 6469 7265  3.0/deepdog/dire
 00000290: 6374 5f6d 6f6e 7465 5f63 6172 6c6f 2f64  ct_monte_carlo/d
 000002a0: 6972 6563 745f 6d63 2e70 7972 0800 0000  irect_mc.pyr....
 000002b0: 1400 0000 7308 0000 000a 0208 0108 0108  ....s...........
 000002c0: 0172 0800 0000 6300 0000 0000 0000 0000  .r....c.........
 000002d0: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
 000002e0: 8200 0000 6500 5a01 6400 5a02 5500 6401  ....e.Z.d.Z.U.d.
 000002f0: 5a03 6504 6505 6402 3c00 6403 5a06 6504  Z.e.e.d.<.d.Z.e.
```

### Comparing `deepdog-1.2.1/deepdog/direct_monte_carlo/__pycache__/dmc_filters.cpython-39.pyc` & `deepdog-1.3.0/deepdog/direct_monte_carlo/__pycache__/dmc_filters.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun May 12 01:51:49 2024 UTC, .py size: 3393 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 b520 4066 410d 0000  a........ @fA...
+00000000: 610d 0d0a 0000 0000 0ec0 4a66 410d 0000  a.........JfA...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 5a07 6400 6404 6c08  ..d.d.l.Z.d.d.l.
 00000060: 5a07 6400 6404 6c09 5a07 6400 6404 6c0a  Z.d.d.l.Z.d.d.l.
 00000070: 5a07 6400 6404 6c00 5a00 4700 6405 6406  Z.d.d.l.Z.G.d.d.
@@ -31,15 +31,15 @@
 000001e0: 0000 0073 1800 0000 6700 7c00 5d10 7d01  ...s....g.|.].}.
 000001f0: 7c01 6a00 7c01 6a01 6602 9102 7104 5300  |.j.|.j.f...q.S.
 00000200: a900 a902 da01 72da 0166 a902 da02 2e30  ......r..f.....0
 00000210: da07 6d65 6173 7572 6572 0800 0000 7208  ..measurer....r.
 00000220: 0000 00fa 632f 686f 6d65 2f6a 656e 6b69  ....c/home/jenki
 00000230: 6e73 2f61 6765 6e74 2f77 6f72 6b73 7061  ns/agent/workspa
 00000240: 6365 2f67 6974 6561 2d70 6879 7369 6373  ce/gitea-physics
-00000250: 5f64 6565 7064 6f67 5f31 2e32 2e31 2f64  _deepdog_1.2.1/d
+00000250: 5f64 6565 7064 6f67 5f31 2e33 2e30 2f64  _deepdog_1.3.0/d
 00000260: 6565 7064 6f67 2f64 6972 6563 745f 6d6f  eepdog/direct_mo
 00000270: 6e74 655f 6361 726c 6f2f 646d 635f 6669  nte_carlo/dmc_fi
 00000280: 6c74 6572 732e 7079 da0a 3c6c 6973 7463  lters.py..<listc
 00000290: 6f6d 703e 0e00 0000 f300 0000 007a 3553  omp>.........z5S
 000002a0: 696e 676c 6544 6f74 506f 7465 6e74 6961  ingleDotPotentia
 000002b0: 6c46 696c 7465 722e 5f5f 696e 6974 5f5f  lFilter.__init__
 000002c0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
```

### Comparing `deepdog-1.2.1/deepdog/direct_monte_carlo/direct_mc.py` & `deepdog-1.3.0/deepdog/direct_monte_carlo/direct_mc.py`

 * *Files identical despite different names*

### Comparing `deepdog-1.2.1/deepdog/direct_monte_carlo/dmc_filters.py` & `deepdog-1.3.0/deepdog/direct_monte_carlo/dmc_filters.py`

 * *Files identical despite different names*

### Comparing `deepdog-1.2.1/deepdog/indexify/__init__.py` & `deepdog-1.3.0/deepdog/indexify/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdog-1.2.1/deepdog/indexify/__pycache__/__init__.cpython-39.pyc` & `deepdog-1.3.0/deepdog/indexify/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun May 12 01:51:49 2024 UTC, .py size: 1710 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 b520 4066 ae06 0000  a........ @f....
+00000000: 610d 0d0a 0000 0000 0ec0 4a66 ae06 0000  a.........Jf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6503 a005 6506 a101 5a07 6403 6404  Z.e...e...Z.d.d.
 00000060: 8400 5a08 4700 6405 6406 8400 6406 8302  ..Z.G.d.d...d...
 00000070: 5a09 6402 5300 2907 7ac7 0a50 726f 6261  Z.d.S.).z..Proba
@@ -41,15 +41,15 @@
 00000280: 8302 8301 5600 0100 7102 6400 5300 a901  ....V...q.d.S...
 00000290: 4e29 03da 0464 6963 74da 037a 6970 da04  N)...dict..zip..
 000002a0: 6b65 7973 2902 da02 2e30 da01 78a9 01da  keys)....0..x...
 000002b0: 0564 6963 7473 a900 fa56 2f68 6f6d 652f  .dicts...V/home/
 000002c0: 6a65 6e6b 696e 732f 6167 656e 742f 776f  jenkins/agent/wo
 000002d0: 726b 7370 6163 652f 6769 7465 612d 7068  rkspace/gitea-ph
 000002e0: 7973 6963 735f 6465 6570 646f 675f 312e  ysics_deepdog_1.
-000002f0: 322e 312f 6465 6570 646f 672f 696e 6465  2.1/deepdog/inde
+000002f0: 332e 302f 6465 6570 646f 672f 696e 6465  3.0/deepdog/inde
 00000300: 7869 6679 2f5f 5f69 6e69 745f 5f2e 7079  xify/__init__.py
 00000310: da09 3c67 656e 6578 7072 3e17 0000 00f3  ..<genexpr>.....
 00000320: 0000 0000 7a20 5f64 6963 745f 7072 6f64  ....z _dict_prod
 00000330: 7563 742e 3c6c 6f63 616c 733e 2e3c 6765  uct.<locals>.<ge
 00000340: 6e65 7870 723e 2904 da04 6c69 7374 da09  nexpr>)...list..
 00000350: 6974 6572 746f 6f6c 73da 0770 726f 6475  itertools..produ
 00000360: 6374 da06 7661 6c75 6573 7208 0000 0072  ct..valuesr....r
```

### Comparing `deepdog-1.2.1/deepdog/real_spectrum_run.py` & `deepdog-1.3.0/deepdog/real_spectrum_run.py`

 * *Files identical despite different names*

### Comparing `deepdog-1.2.1/deepdog/results/__init__.py` & `deepdog-1.3.0/deepdog/results/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdog-1.2.1/deepdog/results/__pycache__/__init__.cpython-39.pyc` & `deepdog-1.3.0/deepdog/results/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun May 12 01:51:49 2024 UTC, .py size: 5869 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 b520 4066 ed16 0000  a........ @f....
+00000000: 610d 0d0a 0000 0000 0ec0 4a66 ed16 0000  a.........Jf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 5001 0000 6400  .....@...sP...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a05 6400 6401 6c06 5a06 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6401 6c07 5a07 6503 a008 6509 a101 5a0a  d.l.Z.e...e...Z.
 00000070: 6501 a00b 6402 a101 5a0c 6403 6404 8400  e...d...Z.d.d...
@@ -33,15 +33,15 @@
 00000200: 5d0e 7d01 7400 a001 7c01 a101 9102 7104  ].}.t...|.....q.
 00000210: 5300 a900 a902 da02 7265 da07 636f 6d70  S.......re..comp
 00000220: 696c 65a9 02da 022e 30da 0770 6174 7465  ile.....0..patte
 00000230: 726e 7202 0000 0072 0200 0000 fa55 2f68  rnr....r.....U/h
 00000240: 6f6d 652f 6a65 6e6b 696e 732f 6167 656e  ome/jenkins/agen
 00000250: 742f 776f 726b 7370 6163 652f 6769 7465  t/workspace/gite
 00000260: 612d 7068 7973 6963 735f 6465 6570 646f  a-physics_deepdo
-00000270: 675f 312e 322e 312f 6465 6570 646f 672f  g_1.2.1/deepdog/
+00000270: 675f 312e 332e 302f 6465 6570 646f 672f  g_1.3.0/deepdog/
 00000280: 7265 7375 6c74 732f 5f5f 696e 6974 5f5f  results/__init__
 00000290: 2e70 79da 0a3c 6c69 7374 636f 6d70 3e0f  .py..<listcomp>.
 000002a0: 0000 0073 0400 0000 0602 02ff 720a 0000  ...s........r...
 000002b0: 0029 037a ca67 656f 6d5f 283f 503c 786d  .).z.geom_(?P<xm
 000002c0: 696e 3e2d 3f5c 642b 295f 283f 503c 786d  in>-?\d+)_(?P<xm
 000002d0: 6178 3e2d 3f5c 642b 295f 283f 503c 796d  ax>-?\d+)_(?P<ym
 000002e0: 696e 3e2d 3f5c 642b 295f 283f 503c 796d  in>-?\d+)_(?P<ym
```

### Comparing `deepdog-1.2.1/deepdog/temp_aware_real_spectrum_run.py` & `deepdog-1.3.0/deepdog/temp_aware_real_spectrum_run.py`

 * *Files identical despite different names*

### Comparing `deepdog-1.2.1/pyproject.toml` & `deepdog-1.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "deepdog"
-version = "1.2.1"
+version = "1.3.0"
 description = ""
 authors = ["Deepak Mallubhotla <dmallubhotla+github@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.10"
-pdme = "^1.2.0"
+pdme = "^1.5.0"
 numpy = "1.22.3"
 scipy = "1.10"
 tqdm = "^4.66.2"
 
 [tool.poetry.dev-dependencies]
 pytest = ">=6"
 flake8 = "^4.0.1"
```

