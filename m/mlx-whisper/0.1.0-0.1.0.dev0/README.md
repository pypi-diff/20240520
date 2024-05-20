# Comparing `tmp/mlx_whisper-0.1.0.tar.gz` & `tmp/mlx_whisper-0.1.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlx_whisper-0.1.0.tar", last modified: Wed May  1 16:03:30 2024, max compression
+gzip compressed data, was "mlx_whisper-0.1.0.dev0.tar", last modified: Mon May 20 04:39:14 2024, max compression
```

## Comparing `mlx_whisper-0.1.0.tar` & `mlx_whisper-0.1.0.dev0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-05-01 16:03:30.329575 mlx_whisper-0.1.0/
--rw-r--r--   0 awnihannun   (501) staff       (20)      170 2024-05-01 16:03:16.000000 mlx_whisper-0.1.0/MANIFEST.in
--rw-r--r--   0 awnihannun   (501) staff       (20)     3471 2024-05-01 16:03:30.329375 mlx_whisper-0.1.0/PKG-INFO
--rw-r--r--   0 awnihannun   (501) staff       (20)     2937 2024-05-01 16:03:16.000000 mlx_whisper-0.1.0/README.md
-drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-05-01 16:03:30.326973 mlx_whisper-0.1.0/mlx_whisper/
--rw-r--r--   0 awnihannun   (501) staff       (20)      148 2024-05-01 16:03:16.000000 mlx_whisper-0.1.0/mlx_whisper/__init__.py
-drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-05-01 16:03:30.328556 mlx_whisper-0.1.0/mlx_whisper/assets/
--rw-r--r--   0 awnihannun   (501) staff       (20)   835554 2024-05-01 16:03:16.000000 mlx_whisper-0.1.0/mlx_whisper/assets/gpt2.tiktoken
--rw-r--r--   0 awnihannun   (501) staff       (20)     4271 2024-05-01 16:03:16.000000 mlx_whisper-0.1.0/mlx_whisper/assets/mel_filters.npz
--rw-r--r--   0 awnihannun   (501) staff       (20)   816730 2024-05-01 16:03:16.000000 mlx_whisper-0.1.0/mlx_whisper/assets/multilingual.tiktoken
--rw-r--r--   0 awnihannun   (501) staff       (20)     5080 2024-05-01 16:03:16.000000 mlx_whisper-0.1.0/mlx_whisper/audio.py
--rw-r--r--   0 awnihannun   (501) staff       (20)    28161 2024-05-01 16:03:16.000000 mlx_whisper-0.1.0/mlx_whisper/decoding.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     1190 2024-05-01 16:03:16.000000 mlx_whisper-0.1.0/mlx_whisper/load_models.py
--rw-r--r--   0 awnihannun   (501) staff       (20)       79 2024-05-01 16:03:16.000000 mlx_whisper-0.1.0/mlx_whisper/requirements.txt
--rw-r--r--   0 awnihannun   (501) staff       (20)    10880 2024-05-01 16:03:16.000000 mlx_whisper-0.1.0/mlx_whisper/timing.py
--rw-r--r--   0 awnihannun   (501) staff       (20)    12407 2024-05-01 16:03:16.000000 mlx_whisper-0.1.0/mlx_whisper/tokenizer.py
--rw-r--r--   0 awnihannun   (501) staff       (20)    10592 2024-05-01 16:03:16.000000 mlx_whisper-0.1.0/mlx_whisper/torch_whisper.py
--rw-r--r--   0 awnihannun   (501) staff       (20)    22942 2024-05-01 16:03:16.000000 mlx_whisper-0.1.0/mlx_whisper/transcribe.py
--rw-r--r--   0 awnihannun   (501) staff       (20)       59 2024-05-01 16:03:16.000000 mlx_whisper-0.1.0/mlx_whisper/version.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     8669 2024-05-01 16:03:16.000000 mlx_whisper-0.1.0/mlx_whisper/whisper.py
-drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-05-01 16:03:30.329163 mlx_whisper-0.1.0/mlx_whisper.egg-info/
--rw-r--r--   0 awnihannun   (501) staff       (20)     3471 2024-05-01 16:03:30.000000 mlx_whisper-0.1.0/mlx_whisper.egg-info/PKG-INFO
--rw-r--r--   0 awnihannun   (501) staff       (20)      586 2024-05-01 16:03:30.000000 mlx_whisper-0.1.0/mlx_whisper.egg-info/SOURCES.txt
--rw-r--r--   0 awnihannun   (501) staff       (20)        1 2024-05-01 16:03:30.000000 mlx_whisper-0.1.0/mlx_whisper.egg-info/dependency_links.txt
--rw-r--r--   0 awnihannun   (501) staff       (20)       79 2024-05-01 16:03:30.000000 mlx_whisper-0.1.0/mlx_whisper.egg-info/requires.txt
--rw-r--r--   0 awnihannun   (501) staff       (20)       12 2024-05-01 16:03:30.000000 mlx_whisper-0.1.0/mlx_whisper.egg-info/top_level.txt
--rw-r--r--   0 awnihannun   (501) staff       (20)       38 2024-05-01 16:03:30.329620 mlx_whisper-0.1.0/setup.cfg
--rw-r--r--   0 awnihannun   (501) staff       (20)      896 2024-05-01 16:03:16.000000 mlx_whisper-0.1.0/setup.py
+drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-05-20 04:39:14.331228 mlx_whisper-0.1.0.dev0/
+-rw-r--r--   0 awnihannun   (501) staff       (20)      170 2024-05-03 19:36:29.000000 mlx_whisper-0.1.0.dev0/MANIFEST.in
+-rw-r--r--   0 awnihannun   (501) staff       (20)     3476 2024-05-20 04:39:14.331022 mlx_whisper-0.1.0.dev0/PKG-INFO
+-rw-r--r--   0 awnihannun   (501) staff       (20)     2937 2024-05-03 19:36:29.000000 mlx_whisper-0.1.0.dev0/README.md
+drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-05-20 04:39:14.327886 mlx_whisper-0.1.0.dev0/mlx_whisper/
+-rw-r--r--   0 awnihannun   (501) staff       (20)      148 2024-05-03 19:36:29.000000 mlx_whisper-0.1.0.dev0/mlx_whisper/__init__.py
+drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-05-20 04:39:14.330165 mlx_whisper-0.1.0.dev0/mlx_whisper/assets/
+-rw-r--r--   0 awnihannun   (501) staff       (20)   835554 2024-05-03 19:36:29.000000 mlx_whisper-0.1.0.dev0/mlx_whisper/assets/gpt2.tiktoken
+-rw-r--r--   0 awnihannun   (501) staff       (20)     4271 2024-05-03 19:36:29.000000 mlx_whisper-0.1.0.dev0/mlx_whisper/assets/mel_filters.npz
+-rw-r--r--   0 awnihannun   (501) staff       (20)   816730 2024-05-03 19:36:29.000000 mlx_whisper-0.1.0.dev0/mlx_whisper/assets/multilingual.tiktoken
+-rw-r--r--   0 awnihannun   (501) staff       (20)     5080 2024-05-03 19:36:29.000000 mlx_whisper-0.1.0.dev0/mlx_whisper/audio.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)    28161 2024-05-03 19:36:29.000000 mlx_whisper-0.1.0.dev0/mlx_whisper/decoding.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     1190 2024-05-03 19:36:29.000000 mlx_whisper-0.1.0.dev0/mlx_whisper/load_models.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)       79 2024-05-03 19:36:29.000000 mlx_whisper-0.1.0.dev0/mlx_whisper/requirements.txt
+-rw-r--r--   0 awnihannun   (501) staff       (20)    10880 2024-05-03 19:36:29.000000 mlx_whisper-0.1.0.dev0/mlx_whisper/timing.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)    12407 2024-05-03 19:36:29.000000 mlx_whisper-0.1.0.dev0/mlx_whisper/tokenizer.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)    10592 2024-05-03 19:36:29.000000 mlx_whisper-0.1.0.dev0/mlx_whisper/torch_whisper.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)    22942 2024-05-03 19:36:29.000000 mlx_whisper-0.1.0.dev0/mlx_whisper/transcribe.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)       64 2024-05-20 04:39:09.000000 mlx_whisper-0.1.0.dev0/mlx_whisper/version.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     8669 2024-05-03 19:36:29.000000 mlx_whisper-0.1.0.dev0/mlx_whisper/whisper.py
+drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-05-20 04:39:14.330802 mlx_whisper-0.1.0.dev0/mlx_whisper.egg-info/
+-rw-r--r--   0 awnihannun   (501) staff       (20)     3476 2024-05-20 04:39:14.000000 mlx_whisper-0.1.0.dev0/mlx_whisper.egg-info/PKG-INFO
+-rw-r--r--   0 awnihannun   (501) staff       (20)      586 2024-05-20 04:39:14.000000 mlx_whisper-0.1.0.dev0/mlx_whisper.egg-info/SOURCES.txt
+-rw-r--r--   0 awnihannun   (501) staff       (20)        1 2024-05-20 04:39:14.000000 mlx_whisper-0.1.0.dev0/mlx_whisper.egg-info/dependency_links.txt
+-rw-r--r--   0 awnihannun   (501) staff       (20)       79 2024-05-20 04:39:14.000000 mlx_whisper-0.1.0.dev0/mlx_whisper.egg-info/requires.txt
+-rw-r--r--   0 awnihannun   (501) staff       (20)       34 2024-05-20 04:39:14.000000 mlx_whisper-0.1.0.dev0/mlx_whisper.egg-info/top_level.txt
+-rw-r--r--   0 awnihannun   (501) staff       (20)       38 2024-05-20 04:39:14.331272 mlx_whisper-0.1.0.dev0/setup.cfg
+-rw-r--r--   0 awnihannun   (501) staff       (20)      916 2024-05-20 04:36:38.000000 mlx_whisper-0.1.0.dev0/setup.py
```

### Comparing `mlx_whisper-0.1.0/PKG-INFO` & `mlx_whisper-0.1.0.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlx-whisper
-Version: 0.1.0
+Version: 0.1.0.dev0
 Summary: OpenAI Whisper on Apple silicon with MLX and the Hugging Face Hub
 Home-page: https://github.com/ml-explore/mlx-examples
 Author: MLX Contributors
 Author-email: mlx@group.apple.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `mlx_whisper-0.1.0/README.md` & `mlx_whisper-0.1.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `mlx_whisper-0.1.0/mlx_whisper/assets/gpt2.tiktoken` & `mlx_whisper-0.1.0.dev0/mlx_whisper/assets/gpt2.tiktoken`

 * *Files identical despite different names*

### Comparing `mlx_whisper-0.1.0/mlx_whisper/assets/mel_filters.npz` & `mlx_whisper-0.1.0.dev0/mlx_whisper/assets/mel_filters.npz`

 * *Files identical despite different names*

### Comparing `mlx_whisper-0.1.0/mlx_whisper/assets/multilingual.tiktoken` & `mlx_whisper-0.1.0.dev0/mlx_whisper/assets/multilingual.tiktoken`

 * *Files identical despite different names*

### Comparing `mlx_whisper-0.1.0/mlx_whisper/audio.py` & `mlx_whisper-0.1.0.dev0/mlx_whisper/audio.py`

 * *Files identical despite different names*

### Comparing `mlx_whisper-0.1.0/mlx_whisper/decoding.py` & `mlx_whisper-0.1.0.dev0/mlx_whisper/decoding.py`

 * *Files identical despite different names*

### Comparing `mlx_whisper-0.1.0/mlx_whisper/load_models.py` & `mlx_whisper-0.1.0.dev0/mlx_whisper/load_models.py`

 * *Files identical despite different names*

### Comparing `mlx_whisper-0.1.0/mlx_whisper/timing.py` & `mlx_whisper-0.1.0.dev0/mlx_whisper/timing.py`

 * *Files identical despite different names*

### Comparing `mlx_whisper-0.1.0/mlx_whisper/tokenizer.py` & `mlx_whisper-0.1.0.dev0/mlx_whisper/tokenizer.py`

 * *Files identical despite different names*

### Comparing `mlx_whisper-0.1.0/mlx_whisper/torch_whisper.py` & `mlx_whisper-0.1.0.dev0/mlx_whisper/torch_whisper.py`

 * *Files identical despite different names*

### Comparing `mlx_whisper-0.1.0/mlx_whisper/transcribe.py` & `mlx_whisper-0.1.0.dev0/mlx_whisper/transcribe.py`

 * *Files identical despite different names*

### Comparing `mlx_whisper-0.1.0/mlx_whisper/whisper.py` & `mlx_whisper-0.1.0.dev0/mlx_whisper/whisper.py`

 * *Files identical despite different names*

### Comparing `mlx_whisper-0.1.0/mlx_whisper.egg-info/PKG-INFO` & `mlx_whisper-0.1.0.dev0/mlx_whisper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlx-whisper
-Version: 0.1.0
+Version: 0.1.0.dev0
 Summary: OpenAI Whisper on Apple silicon with MLX and the Hugging Face Hub
 Home-page: https://github.com/ml-explore/mlx-examples
 Author: MLX Contributors
 Author-email: mlx@group.apple.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `mlx_whisper-0.1.0/mlx_whisper.egg-info/SOURCES.txt` & `mlx_whisper-0.1.0.dev0/mlx_whisper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlx_whisper-0.1.0/setup.py` & `mlx_whisper-0.1.0.dev0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright © 2024 Apple Inc.
 
 import sys
 from pathlib import Path
 
-from setuptools import find_packages, setup
+from setuptools import find_namespace_packages, setup
 
 package_dir = Path(__file__).parent / "mlx_whisper"
 
 with open(package_dir / "requirements.txt") as fid:
     requirements = [l.strip() for l in fid.readlines()]
 
 sys.path.append(str(package_dir))
@@ -22,11 +22,11 @@
     long_description_content_type="text/markdown",
     readme="README.md",
     author_email="mlx@group.apple.com",
     author="MLX Contributors",
     url="https://github.com/ml-explore/mlx-examples",
     license="MIT",
     install_requires=requirements,
-    packages=find_packages(),
+    packages=find_namespace_packages(),
     include_package_data=True,
     python_requires=">=3.8",
 )
```

