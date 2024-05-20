# Comparing `tmp/g2p-mix-0.4.8.tar.gz` & `tmp/g2p-mix-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g2p-mix-0.4.8.tar", last modified: Fri May 17 06:14:32 2024, max compression
+gzip compressed data, was "g2p-mix-0.4.9.tar", last modified: Mon May 20 12:49:42 2024, max compression
```

## Comparing `g2p-mix-0.4.8.tar` & `g2p-mix-0.4.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:14:32.566651 g2p-mix-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-17 06:14:31.000000 g2p-mix-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-17 06:14:31.000000 g2p-mix-0.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-17 06:14:32.566651 g2p-mix-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-17 06:14:31.000000 g2p-mix-0.4.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-17 06:14:31.000000 g2p-mix-0.4.8/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:14:32.562651 g2p-mix-0.4.8/g2p_mix/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-17 06:14:31.000000 g2p-mix-0.4.8/g2p_mix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-17 06:14:31.000000 g2p-mix-0.4.8/g2p_mix/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-05-17 06:14:31.000000 g2p-mix-0.4.8/g2p_mix/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:14:32.562651 g2p-mix-0.4.8/g2p_mix/dict/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-17 06:14:31.000000 g2p-mix-0.4.8/g2p_mix/dict/phrases.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-17 06:14:31.000000 g2p-mix-0.4.8/g2p_mix/dict/single.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-17 06:14:31.000000 g2p-mix-0.4.8/g2p_mix/g2p_eng.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-17 06:14:31.000000 g2p-mix-0.4.8/g2p_mix/g2p_jyut.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-17 06:14:31.000000 g2p-mix-0.4.8/g2p_mix/g2p_mix.py
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-05-17 06:14:31.000000 g2p-mix-0.4.8/g2p_mix/g2p_pth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:14:32.558651 g2p-mix-0.4.8/g2p_mix/nltk_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:14:32.562651 g2p-mix-0.4.8/g2p_mix/nltk_data/corpora/
--rw-r--r--   0 runner    (1001) docker     (127)   896069 2024-05-17 06:14:31.000000 g2p-mix-0.4.8/g2p_mix/nltk_data/corpora/cmudict.zip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:14:32.562651 g2p-mix-0.4.8/g2p_mix/nltk_data/taggers/
--rw-r--r--   0 runner    (1001) docker     (127)  2526731 2024-05-17 06:14:31.000000 g2p-mix-0.4.8/g2p_mix/nltk_data/taggers/averaged_perceptron_tagger.zip
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-17 06:14:31.000000 g2p-mix-0.4.8/g2p_mix/token.py
--rw-r--r--   0 runner    (1001) docker     (127)    11040 2024-05-17 06:14:31.000000 g2p-mix-0.4.8/g2p_mix/tone_sandhi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:14:32.562651 g2p-mix-0.4.8/g2p_mix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-17 06:14:32.000000 g2p-mix-0.4.8/g2p_mix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-17 06:14:32.000000 g2p-mix-0.4.8/g2p_mix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 06:14:32.000000 g2p-mix-0.4.8/g2p_mix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-17 06:14:32.000000 g2p-mix-0.4.8/g2p_mix.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-17 06:14:32.000000 g2p-mix-0.4.8/g2p_mix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-17 06:14:32.000000 g2p-mix-0.4.8/g2p_mix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-17 06:14:31.000000 g2p-mix-0.4.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 06:14:32.566651 g2p-mix-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-17 06:14:31.000000 g2p-mix-0.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:49:42.529775 g2p-mix-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-20 12:49:41.000000 g2p-mix-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-20 12:49:41.000000 g2p-mix-0.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-20 12:49:42.529775 g2p-mix-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-20 12:49:41.000000 g2p-mix-0.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-20 12:49:41.000000 g2p-mix-0.4.9/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:49:42.521775 g2p-mix-0.4.9/g2p_mix/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-20 12:49:41.000000 g2p-mix-0.4.9/g2p_mix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-20 12:49:41.000000 g2p-mix-0.4.9/g2p_mix/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-05-20 12:49:41.000000 g2p-mix-0.4.9/g2p_mix/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:49:42.525775 g2p-mix-0.4.9/g2p_mix/dict/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-20 12:49:41.000000 g2p-mix-0.4.9/g2p_mix/dict/phrases.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-20 12:49:41.000000 g2p-mix-0.4.9/g2p_mix/dict/single.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-20 12:49:41.000000 g2p-mix-0.4.9/g2p_mix/g2p_eng.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-20 12:49:41.000000 g2p-mix-0.4.9/g2p_mix/g2p_jyut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-20 12:49:41.000000 g2p-mix-0.4.9/g2p_mix/g2p_mix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-05-20 12:49:41.000000 g2p-mix-0.4.9/g2p_mix/g2p_pth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:49:42.521775 g2p-mix-0.4.9/g2p_mix/nltk_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:49:42.525775 g2p-mix-0.4.9/g2p_mix/nltk_data/corpora/
+-rw-r--r--   0 runner    (1001) docker     (127)   896069 2024-05-20 12:49:41.000000 g2p-mix-0.4.9/g2p_mix/nltk_data/corpora/cmudict.zip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:49:42.525775 g2p-mix-0.4.9/g2p_mix/nltk_data/taggers/
+-rw-r--r--   0 runner    (1001) docker     (127)  2526731 2024-05-20 12:49:41.000000 g2p-mix-0.4.9/g2p_mix/nltk_data/taggers/averaged_perceptron_tagger.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-20 12:49:41.000000 g2p-mix-0.4.9/g2p_mix/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11040 2024-05-20 12:49:41.000000 g2p-mix-0.4.9/g2p_mix/tone_sandhi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:49:42.525775 g2p-mix-0.4.9/g2p_mix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-20 12:49:42.000000 g2p-mix-0.4.9/g2p_mix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-20 12:49:42.000000 g2p-mix-0.4.9/g2p_mix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 12:49:42.000000 g2p-mix-0.4.9/g2p_mix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-20 12:49:42.000000 g2p-mix-0.4.9/g2p_mix.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-20 12:49:42.000000 g2p-mix-0.4.9/g2p_mix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-20 12:49:42.000000 g2p-mix-0.4.9/g2p_mix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-20 12:49:41.000000 g2p-mix-0.4.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 12:49:42.529775 g2p-mix-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-20 12:49:41.000000 g2p-mix-0.4.9/setup.py
```

### Comparing `g2p-mix-0.4.8/LICENSE` & `g2p-mix-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.4.8/PKG-INFO` & `g2p-mix-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g2p-mix
-Version: 0.4.8
+Version: 0.4.9
 Summary: G2P mix
 Home-page: https://github.com/pengzhendong/g2p-mix
 Author: Zhendong Peng
 Author-email: pzd17@tsinghua.org.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `g2p-mix-0.4.8/README.md` & `g2p-mix-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.4.8/g2p_mix/__init__.py` & `g2p-mix-0.4.9/g2p_mix/__init__.py`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.4.8/g2p_mix/cli.py` & `g2p-mix-0.4.9/g2p_mix/cli.py`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.4.8/g2p_mix/constants.py` & `g2p-mix-0.4.9/g2p_mix/constants.py`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.4.8/g2p_mix/g2p_eng.py` & `g2p-mix-0.4.9/g2p_mix/g2p_eng.py`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.4.8/g2p_mix/g2p_jyut.py` & `g2p-mix-0.4.9/g2p_mix/g2p_jyut.py`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.4.8/g2p_mix/g2p_mix.py` & `g2p-mix-0.4.9/g2p_mix/g2p_mix.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,28 +13,30 @@
 # limitations under the License.
 
 import os
 import re
 
 from pypinyin.constants import RE_HANS
 
-from .g2p_jyut import G2pJyut
-from .g2p_pth import G2pPth
 from .token import Token
 
 
 os.environ["TRANSFORMERS_OFFLINE"] = "1"
 os.environ["HF_DATASETS_OFFLINE"] = "1"
 
 
 class G2pMix:
     def __init__(self, jyut=False, strict=False, use_g2pw=False):
         if jyut:
+            from .g2p_jyut import G2pJyut
+
             self.g2per = G2pJyut()
         else:
+            from .g2p_pth import G2pPth
+
             self.g2per = G2pPth(strict, use_g2pw)
 
         self.jyut = jyut
         # add space between ascii and chinese characters
         self.pattern = re.compile(
             r"(?<=[\u4e00-\u9fa5])(?=[\x00-\x19\x21-\x7F])|(?<=[\x00-\x19\x21-\x7F])(?=[\u4e00-\u9fa5])"
         )
```

### Comparing `g2p-mix-0.4.8/g2p_mix/g2p_pth.py` & `g2p-mix-0.4.9/g2p_mix/g2p_pth.py`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.4.8/g2p_mix/nltk_data/corpora/cmudict.zip` & `g2p-mix-0.4.9/g2p_mix/nltk_data/corpora/cmudict.zip`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.4.8/g2p_mix/nltk_data/taggers/averaged_perceptron_tagger.zip` & `g2p-mix-0.4.9/g2p_mix/nltk_data/taggers/averaged_perceptron_tagger.zip`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.4.8/g2p_mix/token.py` & `g2p-mix-0.4.9/g2p_mix/token.py`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.4.8/g2p_mix/tone_sandhi.py` & `g2p-mix-0.4.9/g2p_mix/tone_sandhi.py`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.4.8/g2p_mix.egg-info/PKG-INFO` & `g2p-mix-0.4.9/g2p_mix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g2p-mix
-Version: 0.4.8
+Version: 0.4.9
 Summary: G2P mix
 Home-page: https://github.com/pengzhendong/g2p-mix
 Author: Zhendong Peng
 Author-email: pzd17@tsinghua.org.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `g2p-mix-0.4.8/g2p_mix.egg-info/SOURCES.txt` & `g2p-mix-0.4.9/g2p_mix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.4.8/setup.py` & `g2p-mix-0.4.9/setup.py`

 * *Files identical despite different names*

