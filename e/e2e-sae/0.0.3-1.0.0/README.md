# Comparing `tmp/e2e_sae-0.0.3.tar.gz` & `tmp/e2e_sae-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e2e_sae-0.0.3.tar", last modified: Fri May 17 20:17:18 2024, max compression
+gzip compressed data, was "e2e_sae-1.0.0.tar", last modified: Mon May 20 12:41:10 2024, max compression
```

## Comparing `e2e_sae-0.0.3.tar` & `e2e_sae-1.0.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-17 20:17:18.002145 e2e_sae-0.0.3/
--rw-r--r--   0 dan        (501) staff       (20)     1071 2024-04-21 12:55:51.000000 e2e_sae-0.0.3/LICENSE
--rw-r--r--   0 dan        (501) staff       (20)     4769 2024-05-17 20:17:18.001778 e2e_sae-0.0.3/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)     3724 2024-05-17 12:29:31.000000 e2e_sae-0.0.3/README.md
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-17 20:17:17.998436 e2e_sae-0.0.3/e2e_sae/
--rw-r--r--   0 dan        (501) staff       (20)       56 2024-04-22 15:36:40.000000 e2e_sae-0.0.3/e2e_sae/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)     3027 2024-04-22 15:36:40.000000 e2e_sae-0.0.3/e2e_sae/data.py
--rw-r--r--   0 dan        (501) staff       (20)     1605 2024-04-22 15:36:40.000000 e2e_sae-0.0.3/e2e_sae/hooks.py
--rw-r--r--   0 dan        (501) staff       (20)     2577 2024-04-22 15:36:40.000000 e2e_sae-0.0.3/e2e_sae/loader.py
--rw-r--r--   0 dan        (501) staff       (20)     1948 2024-04-22 15:36:40.000000 e2e_sae-0.0.3/e2e_sae/log.py
--rw-r--r--   0 dan        (501) staff       (20)    11196 2024-04-22 15:36:40.000000 e2e_sae-0.0.3/e2e_sae/losses.py
--rw-r--r--   0 dan        (501) staff       (20)    11914 2024-04-22 15:36:40.000000 e2e_sae-0.0.3/e2e_sae/metrics.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-17 20:17:17.999876 e2e_sae-0.0.3/e2e_sae/models/
--rw-r--r--   0 dan        (501) staff       (20)        0 2024-04-22 15:36:40.000000 e2e_sae-0.0.3/e2e_sae/models/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)     5364 2024-04-22 15:36:40.000000 e2e_sae-0.0.3/e2e_sae/models/mlp.py
--rw-r--r--   0 dan        (501) staff       (20)     3132 2024-04-22 15:36:40.000000 e2e_sae-0.0.3/e2e_sae/models/sparsifiers.py
--rw-r--r--   0 dan        (501) staff       (20)    20943 2024-05-17 10:10:13.000000 e2e_sae-0.0.3/e2e_sae/models/transformers.py
--rw-r--r--   0 dan        (501) staff       (20)    11142 2024-05-17 16:32:10.000000 e2e_sae-0.0.3/e2e_sae/plotting.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-17 20:17:18.000205 e2e_sae-0.0.3/e2e_sae/scripts/
--rw-r--r--   0 dan        (501) staff       (20)        0 2024-05-10 16:49:48.000000 e2e_sae-0.0.3/e2e_sae/scripts/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)    13657 2024-04-22 15:36:40.000000 e2e_sae-0.0.3/e2e_sae/scripts/upload_hf_dataset.py
--rw-r--r--   0 dan        (501) staff       (20)      151 2024-04-22 15:36:40.000000 e2e_sae-0.0.3/e2e_sae/settings.py
--rw-r--r--   0 dan        (501) staff       (20)     1692 2024-04-22 15:36:40.000000 e2e_sae-0.0.3/e2e_sae/types.py
--rw-r--r--   0 dan        (501) staff       (20)    12944 2024-05-17 10:10:13.000000 e2e_sae-0.0.3/e2e_sae/utils.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-17 20:17:18.001227 e2e_sae-0.0.3/e2e_sae.egg-info/
--rw-r--r--   0 dan        (501) staff       (20)     4769 2024-05-17 20:17:17.000000 e2e_sae-0.0.3/e2e_sae.egg-info/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)      671 2024-05-17 20:17:17.000000 e2e_sae-0.0.3/e2e_sae.egg-info/SOURCES.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2024-05-17 20:17:17.000000 e2e_sae-0.0.3/e2e_sae.egg-info/dependency_links.txt
--rw-r--r--   0 dan        (501) staff       (20)      391 2024-05-17 20:17:17.000000 e2e_sae-0.0.3/e2e_sae.egg-info/requires.txt
--rw-r--r--   0 dan        (501) staff       (20)        8 2024-05-17 20:17:17.000000 e2e_sae-0.0.3/e2e_sae.egg-info/top_level.txt
--rw-r--r--   0 dan        (501) staff       (20)     2289 2024-05-17 20:16:02.000000 e2e_sae-0.0.3/pyproject.toml
--rw-r--r--   0 dan        (501) staff       (20)       38 2024-05-17 20:17:18.002203 e2e_sae-0.0.3/setup.cfg
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-17 20:17:18.001012 e2e_sae-0.0.3/tests/
--rw-r--r--   0 dan        (501) staff       (20)     1900 2024-04-22 15:36:40.000000 e2e_sae-0.0.3/tests/test_mlp.py
--rw-r--r--   0 dan        (501) staff       (20)     8053 2024-04-22 15:36:40.000000 e2e_sae-0.0.3/tests/test_sae.py
--rw-r--r--   0 dan        (501) staff       (20)     2534 2024-05-14 08:17:02.000000 e2e_sae-0.0.3/tests/test_train_tlens_saes.py
--rw-r--r--   0 dan        (501) staff       (20)     1064 2024-04-22 15:36:40.000000 e2e_sae-0.0.3/tests/test_transformer.py
--rw-r--r--   0 dan        (501) staff       (20)     2103 2024-04-22 15:36:40.000000 e2e_sae-0.0.3/tests/test_utils.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-20 12:41:10.953428 e2e_sae-1.0.0/
+-rw-r--r--   0 dan        (501) staff       (20)     1071 2024-04-21 12:55:51.000000 e2e_sae-1.0.0/LICENSE
+-rw-r--r--   0 dan        (501) staff       (20)     4769 2024-05-20 12:41:10.953135 e2e_sae-1.0.0/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)     3724 2024-05-17 12:29:31.000000 e2e_sae-1.0.0/README.md
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-20 12:41:10.948813 e2e_sae-1.0.0/e2e_sae/
+-rw-r--r--   0 dan        (501) staff       (20)       56 2024-04-22 15:36:40.000000 e2e_sae-1.0.0/e2e_sae/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)     3027 2024-04-22 15:36:40.000000 e2e_sae-1.0.0/e2e_sae/data.py
+-rw-r--r--   0 dan        (501) staff       (20)     1605 2024-04-22 15:36:40.000000 e2e_sae-1.0.0/e2e_sae/hooks.py
+-rw-r--r--   0 dan        (501) staff       (20)     2577 2024-04-22 15:36:40.000000 e2e_sae-1.0.0/e2e_sae/loader.py
+-rw-r--r--   0 dan        (501) staff       (20)     1948 2024-04-22 15:36:40.000000 e2e_sae-1.0.0/e2e_sae/log.py
+-rw-r--r--   0 dan        (501) staff       (20)    11196 2024-04-22 15:36:40.000000 e2e_sae-1.0.0/e2e_sae/losses.py
+-rw-r--r--   0 dan        (501) staff       (20)    11914 2024-04-22 15:36:40.000000 e2e_sae-1.0.0/e2e_sae/metrics.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-20 12:41:10.950542 e2e_sae-1.0.0/e2e_sae/models/
+-rw-r--r--   0 dan        (501) staff       (20)        0 2024-04-22 15:36:40.000000 e2e_sae-1.0.0/e2e_sae/models/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)     5364 2024-04-22 15:36:40.000000 e2e_sae-1.0.0/e2e_sae/models/mlp.py
+-rw-r--r--   0 dan        (501) staff       (20)     3132 2024-04-22 15:36:40.000000 e2e_sae-1.0.0/e2e_sae/models/sparsifiers.py
+-rw-r--r--   0 dan        (501) staff       (20)    20943 2024-05-17 10:10:13.000000 e2e_sae-1.0.0/e2e_sae/models/transformers.py
+-rw-r--r--   0 dan        (501) staff       (20)    11142 2024-05-17 16:32:10.000000 e2e_sae-1.0.0/e2e_sae/plotting.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-20 12:41:10.951123 e2e_sae-1.0.0/e2e_sae/scripts/
+-rw-r--r--   0 dan        (501) staff       (20)        0 2024-05-10 16:49:48.000000 e2e_sae-1.0.0/e2e_sae/scripts/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)    13657 2024-04-22 15:36:40.000000 e2e_sae-1.0.0/e2e_sae/scripts/upload_hf_dataset.py
+-rw-r--r--   0 dan        (501) staff       (20)      151 2024-04-22 15:36:40.000000 e2e_sae-1.0.0/e2e_sae/settings.py
+-rw-r--r--   0 dan        (501) staff       (20)     1692 2024-04-22 15:36:40.000000 e2e_sae-1.0.0/e2e_sae/types.py
+-rw-r--r--   0 dan        (501) staff       (20)    12944 2024-05-17 10:10:13.000000 e2e_sae-1.0.0/e2e_sae/utils.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-20 12:41:10.952625 e2e_sae-1.0.0/e2e_sae.egg-info/
+-rw-r--r--   0 dan        (501) staff       (20)     4769 2024-05-20 12:41:10.000000 e2e_sae-1.0.0/e2e_sae.egg-info/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)      671 2024-05-20 12:41:10.000000 e2e_sae-1.0.0/e2e_sae.egg-info/SOURCES.txt
+-rw-r--r--   0 dan        (501) staff       (20)        1 2024-05-20 12:41:10.000000 e2e_sae-1.0.0/e2e_sae.egg-info/dependency_links.txt
+-rw-r--r--   0 dan        (501) staff       (20)      391 2024-05-20 12:41:10.000000 e2e_sae-1.0.0/e2e_sae.egg-info/requires.txt
+-rw-r--r--   0 dan        (501) staff       (20)        8 2024-05-20 12:41:10.000000 e2e_sae-1.0.0/e2e_sae.egg-info/top_level.txt
+-rw-r--r--   0 dan        (501) staff       (20)     2289 2024-05-20 12:40:11.000000 e2e_sae-1.0.0/pyproject.toml
+-rw-r--r--   0 dan        (501) staff       (20)       38 2024-05-20 12:41:10.953489 e2e_sae-1.0.0/setup.cfg
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-20 12:41:10.952362 e2e_sae-1.0.0/tests/
+-rw-r--r--   0 dan        (501) staff       (20)     1900 2024-04-22 15:36:40.000000 e2e_sae-1.0.0/tests/test_mlp.py
+-rw-r--r--   0 dan        (501) staff       (20)     8053 2024-04-22 15:36:40.000000 e2e_sae-1.0.0/tests/test_sae.py
+-rw-r--r--   0 dan        (501) staff       (20)     2534 2024-05-14 08:17:02.000000 e2e_sae-1.0.0/tests/test_train_tlens_saes.py
+-rw-r--r--   0 dan        (501) staff       (20)     1064 2024-04-22 15:36:40.000000 e2e_sae-1.0.0/tests/test_transformer.py
+-rw-r--r--   0 dan        (501) staff       (20)     2103 2024-04-22 15:36:40.000000 e2e_sae-1.0.0/tests/test_utils.py
```

### Comparing `e2e_sae-0.0.3/LICENSE` & `e2e_sae-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `e2e_sae-0.0.3/PKG-INFO` & `e2e_sae-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2e_sae
-Version: 0.0.3
+Version: 1.0.0
 Summary: Repo for training sparse autoencoders end-to-end
 Project-URL: repository, https://github.com/ApolloResearch/e2e_sae
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch~=2.2.0
 Requires-Dist: torchvision~=0.17.0
```

### Comparing `e2e_sae-0.0.3/README.md` & `e2e_sae-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `e2e_sae-0.0.3/e2e_sae/data.py` & `e2e_sae-1.0.0/e2e_sae/data.py`

 * *Files identical despite different names*

### Comparing `e2e_sae-0.0.3/e2e_sae/hooks.py` & `e2e_sae-1.0.0/e2e_sae/hooks.py`

 * *Files identical despite different names*

### Comparing `e2e_sae-0.0.3/e2e_sae/loader.py` & `e2e_sae-1.0.0/e2e_sae/loader.py`

 * *Files identical despite different names*

### Comparing `e2e_sae-0.0.3/e2e_sae/log.py` & `e2e_sae-1.0.0/e2e_sae/log.py`

 * *Files identical despite different names*

### Comparing `e2e_sae-0.0.3/e2e_sae/losses.py` & `e2e_sae-1.0.0/e2e_sae/losses.py`

 * *Files identical despite different names*

### Comparing `e2e_sae-0.0.3/e2e_sae/metrics.py` & `e2e_sae-1.0.0/e2e_sae/metrics.py`

 * *Files identical despite different names*

### Comparing `e2e_sae-0.0.3/e2e_sae/models/mlp.py` & `e2e_sae-1.0.0/e2e_sae/models/mlp.py`

 * *Files identical despite different names*

### Comparing `e2e_sae-0.0.3/e2e_sae/models/sparsifiers.py` & `e2e_sae-1.0.0/e2e_sae/models/sparsifiers.py`

 * *Files identical despite different names*

### Comparing `e2e_sae-0.0.3/e2e_sae/models/transformers.py` & `e2e_sae-1.0.0/e2e_sae/models/transformers.py`

 * *Files identical despite different names*

### Comparing `e2e_sae-0.0.3/e2e_sae/plotting.py` & `e2e_sae-1.0.0/e2e_sae/plotting.py`

 * *Files identical despite different names*

### Comparing `e2e_sae-0.0.3/e2e_sae/scripts/upload_hf_dataset.py` & `e2e_sae-1.0.0/e2e_sae/scripts/upload_hf_dataset.py`

 * *Files identical despite different names*

### Comparing `e2e_sae-0.0.3/e2e_sae/types.py` & `e2e_sae-1.0.0/e2e_sae/types.py`

 * *Files identical despite different names*

### Comparing `e2e_sae-0.0.3/e2e_sae/utils.py` & `e2e_sae-1.0.0/e2e_sae/utils.py`

 * *Files identical despite different names*

### Comparing `e2e_sae-0.0.3/e2e_sae.egg-info/PKG-INFO` & `e2e_sae-1.0.0/e2e_sae.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2e_sae
-Version: 0.0.3
+Version: 1.0.0
 Summary: Repo for training sparse autoencoders end-to-end
 Project-URL: repository, https://github.com/ApolloResearch/e2e_sae
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch~=2.2.0
 Requires-Dist: torchvision~=0.17.0
```

### Comparing `e2e_sae-0.0.3/e2e_sae.egg-info/SOURCES.txt` & `e2e_sae-1.0.0/e2e_sae.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `e2e_sae-0.0.3/pyproject.toml` & `e2e_sae-1.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "e2e_sae"
-version = "0.0.3"
+version = "1.0.0"
 description = "Repo for training sparse autoencoders end-to-end"
 requires-python = ">=3.11"
 readme = "README.md"
 dependencies = [
     "torch~=2.2.0",
     "torchvision~=0.17.0",
     "einops~=0.7.0",
```

### Comparing `e2e_sae-0.0.3/tests/test_mlp.py` & `e2e_sae-1.0.0/tests/test_mlp.py`

 * *Files identical despite different names*

### Comparing `e2e_sae-0.0.3/tests/test_sae.py` & `e2e_sae-1.0.0/tests/test_sae.py`

 * *Files identical despite different names*

### Comparing `e2e_sae-0.0.3/tests/test_train_tlens_saes.py` & `e2e_sae-1.0.0/tests/test_train_tlens_saes.py`

 * *Files identical despite different names*

### Comparing `e2e_sae-0.0.3/tests/test_transformer.py` & `e2e_sae-1.0.0/tests/test_transformer.py`

 * *Files identical despite different names*

### Comparing `e2e_sae-0.0.3/tests/test_utils.py` & `e2e_sae-1.0.0/tests/test_utils.py`

 * *Files identical despite different names*

