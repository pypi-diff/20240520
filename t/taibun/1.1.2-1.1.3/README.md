# Comparing `tmp/taibun-1.1.2.tar.gz` & `tmp/taibun-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taibun-1.1.2.tar", last modified: Tue May 14 09:10:09 2024, max compression
+gzip compressed data, was "taibun-1.1.3.tar", last modified: Mon May 20 10:37:46 2024, max compression
```

## Comparing `taibun-1.1.2.tar` & `taibun-1.1.3.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 09:10:09.638762 taibun-1.1.2/
--rw-rw-rw-   0        0        0     1099 2024-04-30 01:55:12.000000 taibun-1.1.2/LICENSE
--rw-rw-rw-   0        0        0    16288 2024-05-14 09:10:09.635482 taibun-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0    15495 2024-05-14 09:07:00.000000 taibun-1.1.2/README.md
--rw-rw-rw-   0        0        0      103 2024-05-11 09:38:22.000000 taibun-1.1.2/pyproject.toml
--rw-rw-rw-   0        0        0      875 2024-05-14 09:10:09.643584 taibun-1.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-14 09:10:09.463725 taibun-1.1.2/taibun/
--rw-rw-rw-   0        0        0       85 2024-05-07 21:05:54.000000 taibun-1.1.2/taibun/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 09:10:09.532323 taibun-1.1.2/taibun/data/
--rw-rw-rw-   0        0        0    32697 2024-05-11 10:03:23.000000 taibun-1.1.2/taibun/data/traditional.json
--rw-rw-rw-   0        0        0      744 2024-05-11 23:38:34.000000 taibun-1.1.2/taibun/data/vars.json
--rw-rw-rw-   0        0        0  1894437 2024-05-14 05:48:24.000000 taibun-1.1.2/taibun/data/words.json
--rw-rw-rw-   0        0        0    25197 2024-05-12 01:58:19.000000 taibun-1.1.2/taibun/taibun.py
-drwxrwxrwx   0        0        0        0 2024-05-14 09:10:09.630659 taibun-1.1.2/taibun.egg-info/
--rw-rw-rw-   0        0        0    16288 2024-05-14 09:10:09.000000 taibun-1.1.2/taibun.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      664 2024-05-14 09:10:09.000000 taibun-1.1.2/taibun.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 09:10:09.000000 taibun-1.1.2/taibun.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-14 09:10:09.000000 taibun-1.1.2/taibun.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-14 09:10:09.623006 taibun-1.1.2/tests/
--rw-rw-rw-   0        0        0     2350 2024-05-10 21:33:06.000000 taibun-1.1.2/tests/test_additional.py
--rw-rw-rw-   0        0        0    17804 2024-05-10 21:33:06.000000 taibun-1.1.2/tests/test_convert_non_cjk.py
--rw-rw-rw-   0        0        0     9343 2024-05-10 21:33:06.000000 taibun-1.1.2/tests/test_delimiter.py
--rw-rw-rw-   0        0        0     6995 2024-05-10 21:33:06.000000 taibun-1.1.2/tests/test_format.py
--rw-rw-rw-   0        0        0    18978 2024-05-10 21:33:06.000000 taibun-1.1.2/tests/test_ipa_conversion.py
--rw-rw-rw-   0        0        0     6841 2024-05-10 21:33:06.000000 taibun-1.1.2/tests/test_pingyim_conversion.py
--rw-rw-rw-   0        0        0     7306 2024-05-10 21:33:06.000000 taibun-1.1.2/tests/test_poj_conversion.py
--rw-rw-rw-   0        0        0    12530 2024-05-10 21:33:06.000000 taibun-1.1.2/tests/test_punctuation.py
--rw-rw-rw-   0        0        0    34058 2024-05-11 20:31:46.000000 taibun-1.1.2/tests/test_sandhi.py
--rw-rw-rw-   0        0        0     7214 2024-05-10 21:33:06.000000 taibun-1.1.2/tests/test_tailo_conversion.py
--rw-rw-rw-   0        0        0     7304 2024-05-10 21:33:06.000000 taibun-1.1.2/tests/test_tlpa_conversion.py
--rw-rw-rw-   0        0        0     1573 2024-05-10 21:33:06.000000 taibun-1.1.2/tests/test_tokenisation.py
--rw-rw-rw-   0        0        0     7197 2024-05-10 21:33:06.000000 taibun-1.1.2/tests/test_tongiong_conversion.py
--rw-rw-rw-   0        0        0    11681 2024-05-10 21:33:06.000000 taibun-1.1.2/tests/test_zhuyin_conversion.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:37:46.756819 taibun-1.1.3/
+-rw-rw-rw-   0        0        0     1099 2024-04-30 01:55:12.000000 taibun-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0    16307 2024-05-20 10:37:46.756819 taibun-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0    15514 2024-05-20 10:33:29.000000 taibun-1.1.3/README.md
+-rw-rw-rw-   0        0        0      103 2024-05-11 09:38:22.000000 taibun-1.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0      875 2024-05-20 10:37:46.765403 taibun-1.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 10:37:46.550818 taibun-1.1.3/taibun/
+-rw-rw-rw-   0        0        0       85 2024-05-07 21:05:54.000000 taibun-1.1.3/taibun/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:37:46.630342 taibun-1.1.3/taibun/data/
+-rw-rw-rw-   0        0        0     2188 2024-05-20 10:19:40.000000 taibun-1.1.3/taibun/data/simplified.json
+-rw-rw-rw-   0        0        0    70011 2024-05-20 10:02:42.000000 taibun-1.1.3/taibun/data/traditional.json
+-rw-rw-rw-   0        0        0      835 2024-05-20 08:22:03.000000 taibun-1.1.3/taibun/data/vars.json
+-rw-rw-rw-   0        0        0  1893399 2024-05-20 08:22:41.000000 taibun-1.1.3/taibun/data/words.json
+-rw-rw-rw-   0        0        0    25068 2024-05-20 10:16:45.000000 taibun-1.1.3/taibun/taibun.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:37:46.748705 taibun-1.1.3/taibun.egg-info/
+-rw-rw-rw-   0        0        0    16307 2024-05-20 10:37:46.000000 taibun-1.1.3/taibun.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      692 2024-05-20 10:37:46.000000 taibun-1.1.3/taibun.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 10:37:46.000000 taibun-1.1.3/taibun.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-20 10:37:46.000000 taibun-1.1.3/taibun.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-20 10:37:46.744631 taibun-1.1.3/tests/
+-rw-rw-rw-   0        0        0     2350 2024-05-10 21:33:06.000000 taibun-1.1.3/tests/test_additional.py
+-rw-rw-rw-   0        0        0    17804 2024-05-10 21:33:06.000000 taibun-1.1.3/tests/test_convert_non_cjk.py
+-rw-rw-rw-   0        0        0     9343 2024-05-10 21:33:06.000000 taibun-1.1.3/tests/test_delimiter.py
+-rw-rw-rw-   0        0        0     6995 2024-05-10 21:33:06.000000 taibun-1.1.3/tests/test_format.py
+-rw-rw-rw-   0        0        0    18978 2024-05-10 21:33:06.000000 taibun-1.1.3/tests/test_ipa_conversion.py
+-rw-rw-rw-   0        0        0     6841 2024-05-10 21:33:06.000000 taibun-1.1.3/tests/test_pingyim_conversion.py
+-rw-rw-rw-   0        0        0     7306 2024-05-10 21:33:06.000000 taibun-1.1.3/tests/test_poj_conversion.py
+-rw-rw-rw-   0        0        0    12530 2024-05-10 21:33:06.000000 taibun-1.1.3/tests/test_punctuation.py
+-rw-rw-rw-   0        0        0    34066 2024-05-20 09:38:45.000000 taibun-1.1.3/tests/test_sandhi.py
+-rw-rw-rw-   0        0        0     7214 2024-05-10 21:33:06.000000 taibun-1.1.3/tests/test_tailo_conversion.py
+-rw-rw-rw-   0        0        0     7304 2024-05-10 21:33:06.000000 taibun-1.1.3/tests/test_tlpa_conversion.py
+-rw-rw-rw-   0        0        0     1573 2024-05-10 21:33:06.000000 taibun-1.1.3/tests/test_tokenisation.py
+-rw-rw-rw-   0        0        0     7197 2024-05-10 21:33:06.000000 taibun-1.1.3/tests/test_tongiong_conversion.py
+-rw-rw-rw-   0        0        0    11681 2024-05-10 21:33:06.000000 taibun-1.1.3/tests/test_zhuyin_conversion.py
```

### Comparing `taibun-1.1.2/LICENSE` & `taibun-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `taibun-1.1.2/PKG-INFO` & `taibun-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taibun
-Version: 1.1.2
+Version: 1.1.3
 Summary: Taiwanese Hokkien Transliterator and Tokeniser
 Home-page: https://github.com/andreihar/taibun
 Author: Andrei Harbachov
 Author-email: andrei.harbachov@gmail.com
 License: MIT
 Keywords: python,taiwan,taiwanese,taigi,hokkien,romanization,transliteration,transliterator,tokenization,tokenizer
 Classifier: Topic :: Text Processing :: Linguistic
@@ -18,15 +18,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
   <a href="https://github.com/andreihar/taibun">
-    <img src="https://github.com/andreihar/taibun/raw/main/readme/logo.png" alt="Logo" width="90" height="80">
+    <img src="[readme/logo.png](https://github.com/andreihar/taibun/raw/main/readme/logo.png)" alt="Logo" width="90" height="80">
   </a>
   
 # Taibun
 
 
 
 <!-- PROJECT SHIELDS -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: taibun Version: 1.1.2 Summary: Taiwanese Hokkien
+Metadata-Version: 2.1 Name: taibun Version: 1.1.3 Summary: Taiwanese Hokkien
 Transliterator and Tokeniser Home-page: https://github.com/andreihar/taibun
 Author: Andrei Harbachov Author-email: andrei.harbachov@gmail.com License: MIT
 Keywords:
 python,taiwan,taiwanese,taigi,hokkien,romanization,transliteration,transliterator,tokenization,tokenizer
 Classifier: Topic :: Text Processing :: Linguistic Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
```

### Comparing `taibun-1.1.2/README.md` & `taibun-1.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
   <a href="https://github.com/andreihar/taibun">
-    <img src="https://github.com/andreihar/taibun/raw/main/readme/logo.png" alt="Logo" width="90" height="80">
+    <img src="[readme/logo.png](https://github.com/andreihar/taibun/raw/main/readme/logo.png)" alt="Logo" width="90" height="80">
   </a>
   
 # Taibun
 
 
 
 <!-- PROJECT SHIELDS -->
```

### Comparing `taibun-1.1.2/setup.cfg` & `taibun-1.1.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2074 6169 6275 6e0d 0a76 6572 7369   = taibun..versi
-00000020: 6f6e 203d 2031 2e31 2e32 0d0a 6175 7468  on = 1.1.2..auth
+00000020: 6f6e 203d 2031 2e31 2e33 0d0a 6175 7468  on = 1.1.3..auth
 00000030: 6f72 203d 2041 6e64 7265 6920 4861 7262  or = Andrei Harb
 00000040: 6163 686f 760d 0a61 7574 686f 725f 656d  achov..author_em
 00000050: 6169 6c20 3d20 616e 6472 6569 2e68 6172  ail = andrei.har
 00000060: 6261 6368 6f76 4067 6d61 696c 2e63 6f6d  bachov@gmail.com
 00000070: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000080: 5461 6977 616e 6573 6520 486f 6b6b 6965  Taiwanese Hokkie
 00000090: 6e20 5472 616e 736c 6974 6572 6174 6f72  n Transliterator
```

### Comparing `taibun-1.1.2/taibun/data/vars.json` & `taibun-1.1.3/taibun/data/vars.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8863636363636364%*

 * *Differences: {"'廕'": "'蔭'", "'歎'": "'嘆'", "'聼'": "'聽'", "'譁'": "'嘩'", "'鍾'": "'鐘'"}*

```diff
@@ -1,41 +1,46 @@
 {
     "\u50de": "\u507d",
     "\u5553": "\u555f",
     "\u5cef": "\u5cf0",
     "\u5e7a": "\u4e48",
+    "\u5ed5": "\u852d",
     "\u654d": "\u6558",
     "\u67b1": "\u6aaf",
     "\u67fa": "\u67b4",
     "\u6a90": "\u7c37",
+    "\u6b4e": "\u5606",
     "\u6c61": "\u6c59",
     "\u6fd5": "\u6ebc",
     "\u7232": "\u70ba",
     "\u7240": "\u5e8a",
     "\u75f9": "\u75fa",
     "\u7661": "\u75f4",
     "\u7681": "\u7682",
     "\u7ac8": "\u7076",
     "\u7ca7": "\u599d",
     "\u7cc9": "\u7cbd",
     "\u7e94": "\u624d",
     "\u7fa3": "\u7fa4",
+    "\u807c": "\u807d",
     "\u8123": "\u5507",
     "\u81fa": "\u53f0",
     "\u83f8": "\u7159",
     "\u8518": "\u53c3",
     "\u8768": "\u8671",
     "\u8846": "\u773e",
     "\u885e": "\u885b",
     "\u88cf": "\u88e1",
     "\u8988": "\u6838",
     "\u8aac": "\u8aaa",
+    "\u8b41": "\u5629",
     "\u920e": "\u9264",
     "\u9262": "\u7f3d",
     "\u92ed": "\u92b3",
     "\u937c": "\u91dd",
+    "\u937e": "\u9418",
     "\u95b2": "\u95b1",
     "\u9b8e": "\u9bf0",
     "\u9c1b": "\u9c2e",
     "\u9eaa": "\u9eb5",
     "\u9f76": "\u984e"
 }
```

### Comparing `taibun-1.1.2/taibun/data/words.json` & `taibun-1.1.3/taibun/data/words.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992227173800394%*

 * *Differences: {"'蔭化'": "'ìm-hua'",*

 * * "'蔭肥'": "'ìm-puî'",*

 * * "'鐘情'": "'tsiong-tsîng'",*

 * * "'鐘愛'": "'tsiong-ài'",*

 * * "'長嘆'": "'tiông-thàn'",*

 * * 'delete': "['凶險', '反譁', '迴響', '迴轉', '譁', '係項', '廕', '廕化', '廕火', '廕肥', '干證', '慨歎', '鏡檯', '講台', "*

 * *           "'唸經', '內里', '嚨喉鍾仔', '軟痠', '黃痠桶', '朴實', '摒盪', '憑準', '痠軟', '洗盪', '四周圍', '鐵干證', '托夢', "*

 * *           "'歎', '頭齣', '弔禮', '長歎', '直升機', '衝犯', '衝磅', '齣頭', '鍾', '鍾情', '鍾愛', '周詳', '致廕']"}*

```diff
@@ -2981,15 +2981,14 @@
     "\u4fbf\u886b": "pi\u0101n-sann",
     "\u4fbf\u8ca8": "pi\u0101n-hu\u00e8/pi\u0101n-h\u00e8",
     "\u4fbf\u8eca": "pi\u0101n-tshia",
     "\u4fbf\u9053": "pi\u0101n-t\u014d",
     "\u4fbf\u98ef": "pi\u0101n-pn\u0304g",
     "\u4fc2": "h\u0113",
     "\u4fc2\u6578": "h\u0113-s\u00f2o",
-    "\u4fc2\u9805": "h\u0113-h\u0101ng",
     "\u4fc3": "tshiok",
     "\u4fc3\u4f7f": "tshiok-s\u00fa",
     "\u4fc3\u501a": "tshik-u\u00e1",
     "\u4fc3\u5c31": "tshik-tsi\u016b",
     "\u4fc3\u6210": "tshiok-s\u00eeng",
     "\u4fc3\u6642\u9593": "tshik-s\u00ee-kan",
     "\u4fc3\u6b72\u58fd": "tshik-hu\u00e8-si\u016b/tshik-h\u00e8-si\u016b",
@@ -4639,15 +4638,14 @@
     "\u5167\u8932": "l\u0101i-kh\u00f2o",
     "\u5167\u8996\u93e1": "l\u0101i-s\u012b-ki\u00e0nn",
     "\u5167\u89aa": "l\u0101i-tshin",
     "\u5167\u89d2": "l\u0101i-kak",
     "\u5167\u8eab": "l\u0101i-sin",
     "\u5167\u9053": "l\u0101i-t\u014d",
     "\u5167\u90e8": "l\u0101i-p\u014do",
-    "\u5167\u91cc": "l\u0101i-l\u00ed",
     "\u5167\u91cd\u5de1": "l\u0101i-t\u00eeng-s\u00fbn",
     "\u5167\u91ce": "l\u0101i-i\u00e1",
     "\u5167\u91ce\u624b": "l\u0101i-i\u00e1-tshi\u00fa",
     "\u5167\u92b7": "l\u0101i-siau",
     "\u5167\u9580": "l\u0101i-mn\u0302g",
     "\u5167\u9580\u5340": "L\u0101i-b\u00fbn-khu",
     "\u5167\u95a3": "lu\u0113-koh",
@@ -5485,15 +5483,14 @@
     "\u51f6\u5df4\u54e9\u8c93": "hiong-pa-l\u00ed-niau",
     "\u51f6\u5e74": "hiong-li\u00e2n",
     "\u51f6\u624b": "hiong-tshi\u00fa",
     "\u51f6\u62f3": "hiong-k\u00fbn",
     "\u51f6\u6b72": "hiong-su\u00e8",
     "\u51f6\u731b": "hiong-b\u00edng",
     "\u51f6\u8eab": "hiong-sin",
-    "\u51f6\u96aa": "hiong-hi\u00e1m",
     "\u51f9": "nah",
     "\u51f9\u4ed4\u5e95": "lap-\u00e1-t\u00e9/lap-\u00e1-tu\u00e9",
     "\u51f9\u6d6a": "\u0100u-l\u014dng",
     "\u51f9\u8170": "nah-io",
     "\u51fa": "tshut",
     "\u51fa\u4e01": "tshut-ting",
     "\u51fa\u4e0d\u7522": "tshut-put-s\u00e1n",
@@ -7993,15 +7990,14 @@
     "\u53cd\u8239": "p\u00edng-ts\u00fbn",
     "\u53cd\u8272": "hu\u00e1n-sik",
     "\u53cd\u85e4": "p\u00edng-t\u00een",
     "\u53cd\u8986": "p\u00edng-phak",
     "\u53cd\u89c0": "hu\u00e1n-kuan",
     "\u53cd\u89d2": "hu\u00e1n-kak",
     "\u53cd\u8abf": "hu\u00e1n-ti\u0101u",
-    "\u53cd\u8b41": "hu\u00e1n-hu\u0101",
     "\u53cd\u8b49": "hu\u00e1n-ts\u00ecng",
     "\u53cd\u8b8a": "p\u00edng-p\u00ecnn",
     "\u53cd\u8ce3": "p\u00edng-b\u0113/p\u00edng-bu\u0113",
     "\u53cd\u8d77\u53cd\u5012": "hu\u00e1n-kh\u00ed-hu\u00e1n-t\u00f3",
     "\u53cd\u8eab": "p\u00edng-sin",
     "\u53cd\u8eca": "p\u00edng-tshia",
     "\u53cd\u8eca\u9b5a": "p\u00edng-tshia-h\u00ee/p\u00edng-tshia-h\u00fb",
@@ -9037,15 +9033,14 @@
     "\u5468\u5bc6": "tsiu-bi\u030dt",
     "\u5468\u5be7": "Tsiu-l\u00eeng",
     "\u5468\u6021\u6021": "Tsiu-\u00ee-\u00ee",
     "\u5468\u65cb": "tsiu-su\u00e2n",
     "\u5468\u745c": "Tsiu-j\u00fb/Tsiu-l\u00fb",
     "\u5468\u77e5": "tsiu-ti",
     "\u5468\u7ae0": "tsiu-tsiong",
-    "\u5468\u8a73": "tsiu-si\u00f4ng",
     "\u5468\u908a": "tsiu-pinn",
     "\u5471": "ku\u0101",
     "\u5472": "tsh\u016b",
     "\u5473": "b\u012b",
     "\u5473\u7d20": "b\u012b-s\u00f2o",
     "\u5473\u7d20\u7c89": "b\u012b-s\u00f2o-h\u00fan",
     "\u5473\u89ba": "b\u012b-kak",
@@ -9418,15 +9413,14 @@
     "\u5531\u8d77": "tshi\u00f9nn-kh\u00ed",
     "\u5537": "--ioh",
     "\u5538": "li\u0101m",
     "\u5538\u5922\u8a71": "li\u0101m-b\u0101ng-u\u0113",
     "\u5538\u5957\u982d": "li\u0101m-th\u00f2-th\u00e2u",
     "\u5538\u66f8": "li\u0101m-tsu",
     "\u5538\u6b4c\u8a23": "li\u0101m-ko-kuat",
-    "\u5538\u7d93": "li\u0101m-king",
     "\u5538\u8a23": "li\u0101m-kuat",
     "\u553e": "th\u00f2",
     "\u5544": "tok",
     "\u5544\u50f9": "tok-k\u00e8",
     "\u5544\u5544": "tok-tok",
     "\u5544\u6a39\u4ed4\u9ce5": "tok-tshi\u016b-\u00e1-tsi\u00e1u",
     "\u5544\u6a39\u9ce5": "tok-tshi\u016b-tsi\u00e1u",
@@ -9972,15 +9966,14 @@
     "\u56a8\u5589\u6846\u4ed4": "n\u00e2-\u00e2u-khing-\u00e1",
     "\u56a8\u5589\u6e34": "n\u00e2-\u00e2u-khuah",
     "\u56a8\u5589\u6ef4\u4ed4": "n\u00e2-\u00e2u-tih-\u00e1",
     "\u56a8\u5589\u75c7": "n\u00e2-\u00e2u-ts\u00ecng",
     "\u56a8\u5589\u7a7a": "n\u00e2-\u00e2u-khang",
     "\u56a8\u5589\u7ba1": "n\u00e2-\u00e2u-k\u0144g",
     "\u56a8\u5589\u8482\u4ed4": "n\u00e2-\u00e2u-t\u00ec-\u00e1",
-    "\u56a8\u5589\u937e\u4ed4": "n\u00e2-\u00e2u-tsing-\u00e1",
     "\u56a8\u5589\u9418": "n\u00e2-\u00e2u-tsing",
     "\u56a8\u5589\u9418\u4ed4": "n\u00e2-\u00e2u-tsing-\u00e1",
     "\u56a8\u5589\u9aa8": "n\u00e2-\u00e2u-kut",
     "\u56ae": "hi\u00f2ng",
     "\u56b4": "gi\u00e2m",
     "\u56b4\u51ac": "gi\u00e2m-tong",
     "\u56b4\u5211": "gi\u00e2m-h\u00eeng",
@@ -10037,15 +10030,14 @@
     "\u56db\u5169": "s\u00ec-ni\u00fa",
     "\u56db\u51fa": "s\u00ec-tshut",
     "\u56db\u5341\u6345": "s\u00ec-tsa\u030dp-th\u00f3ng",
     "\u56db\u53c9\u8c93": "s\u00ec-tshe-niau",
     "\u56db\u53e5\u4ed4": "s\u00ec-k\u00f9-\u00e1",
     "\u56db\u5408\u9662": "s\u00ec-ha\u030dp-\u012bnn",
     "\u56db\u5468": "s\u00ec-tsiu",
-    "\u56db\u5468\u570d": "s\u00ec-tsiu-u\u00ee",
     "\u56db\u5468\u5898": "s\u00ec-tsiu-k\u00eenn",
     "\u56db\u56db\u6563\u6563": "s\u00ec-s\u00ec-su\u00e0nn-su\u00e0nn",
     "\u56db\u570d": "s\u00ec-u\u00ee",
     "\u56db\u57ce": "S\u00ec-si\u00e2nn",
     "\u56db\u584a\u539d": "s\u00ec-t\u00e8-tsh\u00f9",
     "\u56db\u5b63": "s\u00f9-ku\u00ec",
     "\u56db\u5b63\u6625": "s\u00f9-ku\u00ec-tshun",
@@ -16541,15 +16533,14 @@
     "\u5e72\u70cf": "kan-oo",
     "\u5e72\u7126": "kan-ta",
     "\u5e72\u7901": "kan-ta",
     "\u5e72\u7901\u6025": "kan-ta-kip",
     "\u5e72\u7919": "kan-g\u0101i",
     "\u5e72\u7d93": "kan-kenn/kan-kinn",
     "\u5e72\u82b1": "kan-hue",
-    "\u5e72\u8b49": "kan-ts\u00ecng",
     "\u5e72\u8c46": "Kan-t\u0101u",
     "\u5e72\u8c9d": "kan-pu\u00e8",
     "\u5e72\u8f46": "kan-lo\u030dk",
     "\u5e72\u9023": "kan-li\u00e2n",
     "\u5e72\u904e": "kan-ku\u00e8/kan-k\u00e8",
     "\u5e72\u9091": "Kan-ip",
     "\u5e72\u91dd": "kan-tsiam",
@@ -16972,18 +16963,14 @@
     "\u5ec9": "li\u00e2m",
     "\u5ec9\u50f9": "li\u00e2m-k\u00e8",
     "\u5ec9\u660e": "li\u00e2m-b\u00eeng",
     "\u5ec9\u6f54": "li\u00e2m-kiat",
     "\u5ec9\u76f4": "li\u00e2m-ti\u030dt",
     "\u5eca": "l\u00f4ng",
     "\u5ecd": "ph\u014do",
-    "\u5ed5": "\u00ecm",
-    "\u5ed5\u5316": "\u00ecm-hua",
-    "\u5ed5\u706b": "\u00ecm-hu\u00e9/\u00ecm-h\u00e9",
-    "\u5ed5\u80a5": "\u00ecm-pu\u00ee",
     "\u5ed6": "li\u0101u",
     "\u5ed6\u5cfb": "Li\u0101u-ts\u00f9n",
     "\u5eda": "t\u00f4o",
     "\u5eda\u5177": "t\u00fb-kh\u016b",
     "\u5eda\u5b50": "t\u00f4o-ts\u00ed",
     "\u5eda\u5b50\u5e2b": "t\u00f4o-ts\u00ed-sai",
     "\u5eda\u5e2b": "t\u00fb-su",
@@ -17167,15 +17154,14 @@
     "\u5f13\u958b": "king-khui",
     "\u5f13\u978b": "kiong-\u00ea/kiong-u\u00ea",
     "\u5f14": "ti\u00e0u",
     "\u5f14\u554f": "ti\u00e0u-b\u016bn",
     "\u5f14\u55aa": "ti\u00e0u-song",
     "\u5f14\u6587": "ti\u00e0u-b\u00fbn",
     "\u5f14\u796d": "ti\u00e0u-ts\u00e8",
-    "\u5f14\u79ae": "ti\u00e0u-l\u00e9",
     "\u5f14\u8a5e": "ti\u00e0u-s\u00fb",
     "\u5f14\u8fad": "ti\u00e0u-s\u00fb",
     "\u5f15": "\u00edn",
     "\u5f15\u4eba": "\u00edn-l\u00e2ng",
     "\u5f15\u4eba\u5165\u52dd": "\u00edn-j\u00een-ji\u030dp-s\u00ecng/\u00edn-l\u00een-li\u030dp-s\u00ecng",
     "\u5f15\u4eba\u6ce8\u76ee": "\u00edn-l\u00e2ng-ts\u00f9-bo\u030dk",
     "\u5f15\u4ee5\u70ba\u50b2": "\u00edn-\u00ed-u\u00ee-ng\u014do",
@@ -18849,15 +18835,14 @@
     "\u6163\u7528\u8a9e": "ku\u00e0n-i\u014dng-g\u00ed/ku\u00e0n-i\u014dng-g\u00fa",
     "\u6163\u7aca": "ku\u00e0n-tshiap",
     "\u6163\u7df4": "ku\u00e0n-li\u0101n",
     "\u6167": "hu\u012b",
     "\u6167\u6839": "hu\u012b-kin/hu\u012b-kun",
     "\u6168": "kh\u00e0i",
     "\u6168\u5606": "kh\u00e0i-th\u00e0n",
-    "\u6168\u6b4e": "kh\u00e0i-th\u00e0n",
     "\u6168\u7136": "kh\u00e0i-ji\u00e2n/kh\u00e0i-li\u00e2n",
     "\u616e": "l\u012b/l\u016b",
     "\u6170": "u\u00ec",
     "\u6170\u52c9": "u\u00ec-bi\u00e1n",
     "\u6170\u52de": "u\u00ec-l\u00f4",
     "\u6170\u554f": "u\u00ec-b\u016bn",
     "\u6170\u554f\u91d1": "u\u00ec-b\u016bn-kim",
@@ -18898,15 +18883,14 @@
     "\u6191\u4f9d": "p\u00een-i",
     "\u6191\u4fe1": "p\u00een-s\u00ecn",
     "\u6191\u51c6": "p\u00een-ts\u00fan",
     "\u6191\u63a0\u6e96": "p\u00een-lia\u030dh-ts\u00fan",
     "\u6191\u64da": "p\u00een-k\u00ec/p\u00een-k\u00f9",
     "\u6191\u672c\u4e8b": "p\u00een-p\u00fan-s\u016b",
     "\u6191\u689d": "p\u00een-ti\u00e2u",
-    "\u6191\u6e96": "p\u00een-ts\u00fan",
     "\u6191\u798f\u6c23": "p\u00een-hok-kh\u00ec",
     "\u6191\u8b49": "p\u00een-ts\u00ecng",
     "\u6191\u982d": "p\u00een-th\u00e2u",
     "\u6191\u982d\u4f86": "p\u00een-th\u00e2u-l\u00e2i",
     "\u6194": "tsi\u00e2u",
     "\u6194\u60b4": "tsi\u00e2u-tsu\u012b",
     "\u619a": "t\u0101n",
@@ -19647,15 +19631,14 @@
     "\u6253\u9f13\u5c71": "T\u00e1-k\u00f3o-suann",
     "\u6253\u9f13\u5dba": "T\u00e1nn-k\u00f3o-ni\u00e1",
     "\u6253\u9f13\u793e": "T\u00e1nn-k\u00f3o-si\u0101",
     "\u6258": "thok",
     "\u6258\u4e0b\u6597": "thuh-\u0113-t\u00e1u",
     "\u6258\u4e0b\u9826": "thuh-\u0113-hu\u00e2i",
     "\u6258\u5152\u6240": "thok-j\u00ee-s\u00f3o/thok-l\u00ee-s\u00f3o",
-    "\u6258\u5922": "thok-b\u0101ng",
     "\u6258\u67b4\u4ed4": "thuh-ku\u00e1i-\u00e1",
     "\u6258\u7834": "thuh-phu\u00e0",
     "\u6258\u798f\u6e2c\u9a57": "thok-hok-tshik-gi\u0101m",
     "\u6258\u7cbe\u795e": "thuh-tsing-s\u00een",
     "\u6258\u7f3d": "thok-puat",
     "\u6258\u81ed": "thuh-tsh\u00e0u",
     "\u6258\u8a71\u9aa8": "thuh-u\u0113-kut",
@@ -21803,15 +21786,14 @@
     "\u6452\u5009": "pi\u00e0nn-tshng",
     "\u6452\u5009\u5eab": "pi\u00e0nn-tshng-kh\u00f2o",
     "\u6452\u5712": "pi\u00e0nn-hn\u0302g",
     "\u6452\u623f\u9593": "pi\u00e0nn-p\u00e2ng-king",
     "\u6452\u6383": "pi\u00e0nn-s\u00e0u",
     "\u6452\u6c34": "pi\u00e0nn-tsu\u00ed",
     "\u6452\u7262": "pi\u00e0nn-ti\u00e2u",
-    "\u6452\u76ea": "pi\u00e0nn-tn\u0304g",
     "\u6452\u8569": "pi\u00e0nn-tn\u0304g",
     "\u6452\u8ca8\u5e95": "pi\u00e0nn-hu\u00e8-t\u00e9/pi\u00e0nn-h\u00e8-tu\u00e9",
     "\u6452\u8ce3": "pi\u00e0nn-b\u0113/pi\u00e0nn-bu\u0113",
     "\u6454": "siak",
     "\u6454\u5012": "siak-t\u00f3",
     "\u6454\u5927\u7720": "si\u00e0ng-tu\u0101-b\u00een",
     "\u6454\u5927\u96e8": "si\u00e0ng-tu\u0101-h\u014do",
@@ -25002,15 +24984,14 @@
     "\u6731\u9dfa": "tsu-l\u014do",
     "\u6734": "phoh",
     "\u6734\u4ed4": "phoh-\u00e1",
     "\u6734\u4ed4\u6a39": "phoh-\u00e1-tshi\u016b",
     "\u6734\u4ed4\u8de4": "Phoh-\u00e1-kha",
     "\u6734\u5b50\u5e02": "Phoh-ts\u00fa-tsh\u012b",
     "\u6734\u5b50\u6eaa": "Phoh-ts\u00fa-khe/Phoh-ts\u00fa-khue",
-    "\u6734\u5be6": "phoh-si\u030dt",
     "\u673d": "hi\u00fa",
     "\u673d\u721b": "hi\u00fa-nu\u0101",
     "\u6746": "kuainn",
     "\u6749": "sam",
     "\u6749\u4ed4": "sam-\u00e1",
     "\u6749\u4ed4\u67f4": "sam-\u00e1-tsh\u00e2",
     "\u6749\u4ed4\u884c": "sam-\u00e1-h\u00e2ng",
@@ -26751,15 +26732,14 @@
     "\u6b4c\u8072": "kua-siann",
     "\u6b4c\u821e": "kua-b\u00fa",
     "\u6b4c\u8a5e": "kua-s\u00fb",
     "\u6b4c\u8a69": "kua-si",
     "\u6b4c\u8b20": "kua-i\u00e2u",
     "\u6b4c\u8b5c": "kua-ph\u00f3o",
     "\u6b4c\u980c": "ko-si\u014dng",
-    "\u6b4e": "th\u00e0n",
     "\u6b50": "au",
     "\u6b50\u4e9e": "Au-a",
     "\u6b50\u5f0f": "Au-sik",
     "\u6b50\u6253": "au-t\u00e1nn",
     "\u6b50\u6d32": "Au-tsiu",
     "\u6b50\u6d32\u4eba": "Au-tsiu-l\u00e2ng",
     "\u6b50\u6d32\u9322": "Au-tsiu-ts\u00eenn",
@@ -28818,15 +28798,14 @@
     "\u6d17\u6de8": "s\u00e9-ts\u012bng/su\u00e9-ts\u012bng",
     "\u6d17\u6e05": "s\u00e9-tshing/su\u00e9-tshing",
     "\u6d17\u6e05\u6c23": "s\u00e9-tshing-kh\u00ec/su\u00e9-tshing-kh\u00ec",
     "\u6d17\u6fef": "s\u00e9-tso\u030dk/su\u00e9-tso\u030dk",
     "\u6d17\u718a": "S\u00e9-h\u00eem/Su\u00e9-h\u00eem",
     "\u6d17\u7248": "s\u00e9-p\u00e1n/su\u00e9-p\u00e1n",
     "\u6d17\u724c": "s\u00e9-p\u00e2i/su\u00e9-p\u00e2i",
-    "\u6d17\u76ea": "s\u00e9-tn\u0304g/su\u00e9-tn\u0304g",
     "\u6d17\u77f3\u4ed4": "s\u00e9-tsio\u030dh-\u00e1/su\u00e9-tsio\u030dh-\u00e1",
     "\u6d17\u7897": "s\u00e9-u\u00e1nn/su\u00e9-u\u00e1nn",
     "\u6d17\u79ae": "s\u00e9-l\u00e9/su\u00e9-l\u00e9",
     "\u6d17\u814e": "s\u00e9-s\u012bn/su\u00e9-s\u012bn",
     "\u6d17\u8166": "s\u00e9-n\u00e1u/su\u00e9-n\u00e1u",
     "\u6d17\u8170\u5b50": "s\u00e9-io-ts\u00ed/su\u00e9-io-ts\u00ed",
     "\u6d17\u8569": "s\u00e9-tn\u0304g/su\u00e9-tn\u0304g",
@@ -34615,15 +34594,14 @@
     "\u75df\u8a71": "si\u00e1u-u\u0113",
     "\u75df\u8c93": "si\u00e1u-niau",
     "\u75df\u8caa": "si\u00e1u-tham",
     "\u75df\u8df3": "si\u00e1u-thi\u00e0u",
     "\u75df\u9f63": "si\u00e1u-tshut",
     "\u75df\u9f63\u4ed4": "si\u00e1u-tshut-\u00e1",
     "\u75e0": "sng",
-    "\u75e0\u8edf": "sng-n\u0144g",
     "\u75e1": "p\u00f4o",
     "\u75e2": "l\u012b",
     "\u75e2\u75c5": "l\u012b-p\u0113nn/l\u012b-p\u012bnn",
     "\u75e2\u75c7": "l\u012b-ts\u00ecng",
     "\u75e3": "k\u00ec",
     "\u75e3\u6bdb": "k\u00ec-mn\u0302g",
     "\u75e3\u9b1a": "k\u00ec-tshiu",
@@ -35531,15 +35509,14 @@
     "\u76f4": "ti\u030dt",
     "\u76f4\u4e0b": "ti\u030dt-h\u0101",
     "\u76f4\u4eba": "ti\u030dt-l\u00e2ng",
     "\u76f4\u5165": "ti\u030dt-ji\u030dp/ti\u030dt-li\u030dp",
     "\u76f4\u5207\u9762": "ti\u030dt-tshiat-b\u012bn",
     "\u76f4\u52a0\u5f04": "Ti\u030dt-ka-l\u014dng",
     "\u76f4\u5347": "ti\u030dt-sing",
-    "\u76f4\u5347\u6a5f": "ti\u030dt-sing-ki",
     "\u76f4\u5589": "ti\u030dt-\u00e2u",
     "\u76f4\u5c6c": "ti\u030dt-sio\u030dk",
     "\u76f4\u5f91": "ti\u030dt-k\u00ecng",
     "\u76f4\u5fc3\u6027": "ti\u030dt-sim-s\u00ecng",
     "\u76f4\u6027\u5730": "ti\u030dt-s\u00ecng-t\u0113/ti\u030dt-s\u00ecng-tu\u0113",
     "\u76f4\u6392\u8f2a": "ti\u030dt-p\u00e2i-li\u00e1n",
     "\u76f4\u63a5": "ti\u030dt-tsiap",
@@ -42215,15 +42192,14 @@
     "\u81f4\u5230": "t\u00ec-k\u00e0u",
     "\u81f4\u529b": "t\u00ec-li\u030dk",
     "\u81f4\u52dd": "t\u00ec-s\u00ecng",
     "\u81f4\u547d": "t\u00ec-b\u012bng",
     "\u81f4\u547d\u50b7": "t\u00ec-b\u012bng-siong",
     "\u81f4\u547d\u8655": "t\u00ec-b\u012bng-tsh\u00f9",
     "\u81f4\u5bcc": "t\u00ec-h\u00f9",
-    "\u81f4\u5ed5": "t\u00ec-\u00ecm",
     "\u81f4\u5fc3": "t\u00ec-sim",
     "\u81f4\u6068": "t\u00ec-h\u012bn/t\u00ec-h\u016bn",
     "\u81f4\u610f": "t\u00ec-\u00ec",
     "\u81f4\u6210": "t\u00ec-tsi\u00e2nn",
     "\u81f4\u656c": "t\u00ec-k\u00ecng",
     "\u81f4\u6b49": "t\u00ec-khi\u00e0m",
     "\u81f4\u6b7b": "t\u00ec-s\u00ed",
@@ -44009,22 +43985,24 @@
     "\u852b\u812f": "lian-p\u00f3o",
     "\u852c": "se",
     "\u852c\u679c": "soo-k\u00f3",
     "\u852c\u83dc": "soo-tsh\u00e0i",
     "\u852d": "\u00ecm",
     "\u852d\u4efd": "\u00ecm-h\u016bn",
     "\u852d\u5206": "\u00ecm-h\u016bn",
+    "\u852d\u5316": "\u00ecm-hua",
     "\u852d\u5806": "\u00ecm-tui",
     "\u852d\u5c4d": "\u00ecm-si",
     "\u852d\u5f71": "\u00ecm-\u00edng",
     "\u852d\u706b": "\u00ecm-hu\u00e9/\u00ecm-h\u00e9",
     "\u852d\u74dc\u4ed4": "\u00ecm-kue-\u00e1",
     "\u852d\u767d": "\u00ecm-pe\u030dh",
     "\u852d\u7da0": "\u00ecm-li\u030dk",
     "\u852d\u80a1": "\u00ecm-k\u00f3o",
+    "\u852d\u80a5": "\u00ecm-pu\u00ee",
     "\u852d\u8449": "\u00ecm-hio\u030dh",
     "\u852d\u852d": "\u00ecm-\u0144g",
     "\u852d\u8c49": "\u00ecm-s\u012bnn",
     "\u852d\u8c49\u4ed4": "\u00ecm-s\u012bnn-\u00e1",
     "\u852d\u8eab": "\u00ecm-sin",
     "\u852d\u9152": "\u00ecm-tsi\u00fa",
     "\u8534\u6f41": "mu\u00e2-\u00ednn",
@@ -45100,19 +45078,17 @@
     "\u885d\u61f8": "tsh\u00ecng-ku\u00e2n",
     "\u885d\u62da": "tshiong-pi\u00e0nn",
     "\u885d\u64ca": "tshiong-kik",
     "\u885d\u6c34": "tsh\u00ecng-tsu\u00ed",
     "\u885d\u6e67": "tshiong-\u00edng",
     "\u885d\u6fc0": "tsh\u00ecng-kik",
     "\u885d\u7159": "tsh\u00ecng-ian",
-    "\u885d\u72af": "tshiong-hu\u0101n",
     "\u885d\u7687": "tsh\u00ecng-h\u00f4ng",
     "\u885d\u7834": "tshiong-phu\u00e0",
     "\u885d\u78b0": "tsh\u00f3ng-p\u014dng",
-    "\u885d\u78c5": "tshiong-p\u014dng",
     "\u885d\u7a81": "tshiong-tu\u030dt",
     "\u885d\u7d05\u71c8": "tshiong-\u00e2ng-ting",
     "\u885d\u7dda": "tshiong-su\u00e0nn",
     "\u885d\u8457\u9b3c": "tshiong-tio\u030dh-ku\u00ed",
     "\u885d\u92d2\u9677\u9663": "tshiong-hong-h\u0101m-t\u012bn",
     "\u885d\u9762": "tsh\u00ecng-b\u012bn",
     "\u885d\u98a8": "tsh\u00ecng-hong",
@@ -46695,15 +46671,14 @@
     "\u8b1b\u50f9": "k\u00f3ng-k\u00e8",
     "\u8b1b\u50f9\u6578": "k\u00f3ng-k\u00e8-si\u00e0u",
     "\u8b1b\u5187\u8a71": "k\u00f3ng-ph\u00e0nn-u\u0113",
     "\u8b1b\u51fa": "k\u00f3ng-tshut",
     "\u8b1b\u52a0\u8a71": "k\u00f3ng-ke-u\u0113",
     "\u8b1b\u5343\u8b1b\u842c": "k\u00e1ng-tshing-k\u00e1ng-b\u0101n",
     "\u8b1b\u53e4": "k\u00f3ng-k\u00f3o",
-    "\u8b1b\u53f0": "k\u00e1ng-t\u00e2i",
     "\u8b1b\u548c": "k\u00f3ng-h\u00f4",
     "\u8b1b\u5629": "k\u00f3ng-hu\u0101",
     "\u8b1b\u5802": "k\u00e1ng-tn\u0302g",
     "\u8b1b\u5927\u8a71": "k\u00f3ng-tu\u0101-u\u0113",
     "\u8b1b\u597d": "k\u00f3ng-h\u00f3",
     "\u8b1b\u597d\u8a71": "k\u00f3ng-h\u00f3-u\u0113",
     "\u8b1b\u5b78": "k\u00e1ng-ha\u030dk",
@@ -46791,15 +46766,14 @@
     "\u8b40\u6d61": "h\u00e0m-phu\u030dh",
     "\u8b40\u72d7": "h\u00e0m-k\u00e1u",
     "\u8b40\u72d7\u6f72": "h\u00e0m-k\u00e1u-si\u00e2u",
     "\u8b40\u8a71": "h\u00e0m-u\u0113",
     "\u8b40\u8b40": "h\u00e0m-h\u00e0m",
     "\u8b40\u8b40\u4ed4": "h\u00e0m-h\u00e0m-\u00e1",
     "\u8b40\u93e1": "h\u00e0m-ki\u00e0nn",
-    "\u8b41": "hu\u0101",
     "\u8b49": "ts\u00ecng",
     "\u8b49\u4ea4\u6240": "Ts\u00ecng-kau-s\u00f3o",
     "\u8b49\u4ea4\u7a05": "ts\u00ecng-kau-su\u00e8/ts\u00ecng-kau-s\u00e8",
     "\u8b49\u4eba": "ts\u00ecng-j\u00een/ts\u00ecng-l\u00een",
     "\u8b49\u4ef6": "ts\u00ecng-ki\u0101nn",
     "\u8b49\u5238": "ts\u00ecng-k\u01f9g",
     "\u8b49\u5238\u5546": "ts\u00ecng-k\u01f9g-siong",
@@ -48994,15 +48968,14 @@
     "\u8edf\u6c6b": "n\u0144g-tsi\u00e1nn",
     "\u8edf\u723d": "n\u0144g-s\u0144g",
     "\u8edf\u7247": "n\u0144g-ph\u00ecnn",
     "\u8edf\u7259": "n\u0144g-g\u00ea",
     "\u8edf\u7334": "n\u0144g-k\u00e2u",
     "\u8edf\u7403\u4ed4": "n\u0144g-ki\u00fb-\u00e1",
     "\u8edf\u7565": "n\u0144g-lio\u030dh",
-    "\u8edf\u75e0": "n\u0144g-sng",
     "\u8edf\u7981": "n\u0144g-k\u00ecm",
     "\u8edf\u7b46": "n\u0144g-pit",
     "\u8edf\u7cd6": "n\u0144g-thn\u0302g",
     "\u8edf\u7d21\u7d21": "n\u0144g-ph\u00e1ng-ph\u00e1ng",
     "\u8edf\u7dda": "n\u0144g-su\u00e0nn",
     "\u8edf\u809a": "n\u0144g-t\u00f3o",
     "\u8edf\u80a5": "n\u0144g-pu\u00ee",
@@ -49494,17 +49467,15 @@
     "\u8feb\u8fd1": "pik-k\u012bn/pik-k\u016bn",
     "\u8fed": "tia\u030dt",
     "\u8ff0": "su\u030dt",
     "\u8ff0\u8aaa": "su\u030dt-suat",
     "\u8ff4": "hu\u00ea",
     "\u8ff4\u5eca": "hu\u00ea-l\u00f4ng",
     "\u8ff4\u8178": "hu\u00ea-tn\u0302g",
-    "\u8ff4\u8f49": "hu\u00ea-t\u0144g",
     "\u8ff4\u907f": "hu\u00ea-p\u012b",
-    "\u8ff4\u97ff": "hu\u00ea-hi\u00e1ng",
     "\u8ff5": "th\u00e0ng",
     "\u8ff5\u5149": "th\u00e0ng-kng",
     "\u8ff5\u5929\u82b3": "Th\u00e0ng-thinn-phang",
     "\u8ff5\u5fc3": "th\u00e0ng-sim",
     "\u8ff5\u6d77": "th\u00e0ng-h\u00e1i",
     "\u8ff5\u904e": "th\u00e0ng-ku\u00e8/th\u00e0ng-k\u00e8",
     "\u8ff7": "b\u00ea",
@@ -51940,17 +51911,14 @@
     "\u935b\u9318": "tu\u00e0n-thu\u00ee",
     "\u9364": "tshiah",
     "\u9364\u7b95": "tshiah-ki",
     "\u9365": "keh/kueh",
     "\u9365\u4ed4": "keh-\u00e1/kueh-\u00e1",
     "\u9375": "ki\u0101n",
     "\u9375\u8a9e": "ki\u0101n-g\u00ed/ki\u0101n-g\u00fa",
-    "\u937e": "tsing",
-    "\u937e\u60c5": "tsiong-ts\u00eeng",
-    "\u937e\u611b": "tsiong-\u00e0i",
     "\u9394": "i\u00fbnn",
     "\u9394\u53bb": "i\u00fbnn-kh\u00ec",
     "\u9396": "s\u00f3",
     "\u9396\u5319": "s\u00f3-s\u00ee",
     "\u9396\u5319\u4f34": "s\u00f3-s\u00ee-phu\u0101nn",
     "\u9396\u5319\u5708\u4ed4": "s\u00f3-s\u00ee-khian-\u00e1",
     "\u9396\u5589": "s\u00f3-\u00e2u",
@@ -51989,15 +51957,14 @@
     "\u93ae\u975c\u5291": "t\u00ecn-ts\u012bng-tse",
     "\u93c3": "tso\u030dk",
     "\u93d8": "tshiong",
     "\u93e1": "ki\u00e0nn",
     "\u93e1\u4ec1": "ki\u00e0nn-j\u00een/ki\u00e0nn-l\u00een",
     "\u93e1\u53f0\u684c": "ki\u00e0nn-t\u00e2i-toh",
     "\u93e1\u6846": "ki\u00e0nn-khing",
-    "\u93e1\u6aaf": "ki\u00e0nn-t\u00e2i",
     "\u93e1\u76d2": "ki\u00e0nn-a\u030dp",
     "\u93e1\u78e8\u93e1": "ki\u00e0nn-bu\u00e2-ki\u00e0nn",
     "\u93e1\u8089": "ki\u00e0nn-bah",
     "\u93e1\u81fa": "ki\u00e0nn-t\u00e2i",
     "\u93e1\u93e1": "ki\u00e0nn-ki\u00e0nn",
     "\u93e1\u9762": "ki\u00e0nn-b\u012bn",
     "\u93e1\u982d": "ki\u00e0nn-th\u00e2u",
@@ -52016,14 +51983,16 @@
     "\u9403\u9238": "n\u00e2-pua\u030dh",
     "\u9410": "li\u00e2u",
     "\u9418": "tsing",
     "\u9418\u4e73\u77f3": "tsing-j\u00fa-tsio\u030dh/tsing-l\u00fa-tsio\u030dh",
     "\u9418\u4ed4": "tsing-\u00e1",
     "\u9418\u5976": "tsing-ling/tsing-ni",
     "\u9418\u5976\u77f3": "tsing-ling-tsio\u030dh/tsing-ni-tsio\u030dh",
+    "\u9418\u60c5": "tsiong-ts\u00eeng",
+    "\u9418\u611b": "tsiong-\u00e0i",
     "\u9418\u69cc": "tsing-thu\u00ee",
     "\u9418\u8072": "tsing-siann",
     "\u9418\u9336": "tsing-pi\u00f3",
     "\u9418\u97ff": "tsing-hi\u00e1ng",
     "\u9418\u9ede": "tsing-ti\u00e1m",
     "\u9418\u9ede\u8cbb": "tsing-ti\u00e1m-hu\u00ec",
     "\u942e\u5200": "li\u00e2m-to",
@@ -52046,15 +52015,14 @@
     "\u9435\u5b9a": "thih-t\u012bng",
     "\u9435\u5c3a": "thih-tshioh",
     "\u9435\u5c4e": "thih-s\u00e1i",
     "\u9435\u5de5\u5ee0": "thih-kang-tshi\u00fann",
     "\u9435\u5e3d": "thih-b\u014d",
     "\u9435\u5e3d\u87f2": "Thih-b\u014d-th\u00e2ng",
     "\u9435\u5e55": "thih-b\u014do",
-    "\u9435\u5e72\u8b49": "thih-kan-ts\u00ecng",
     "\u9435\u5f48": "thih-tu\u00e2nn",
     "\u9435\u624b": "thih-tshi\u00fa",
     "\u9435\u6253": "thih-t\u00e1",
     "\u9435\u62c4\u4ed4": "thih-t\u00fa-\u00e1",
     "\u9435\u62f3\u982d": "thih-k\u00fbn-th\u00e2u",
     "\u9435\u6383\u5e1a": "thih-s\u00e0u-tshi\u00fa",
     "\u9435\u642d": "thih-tah",
@@ -52232,14 +52200,15 @@
     "\u9577": "ti\u00f3ng",
     "\u9577\u4e0a": "ti\u00f3ng-si\u0101ng",
     "\u9577\u4e45": "tn\u0302g-k\u00fa",
     "\u9577\u5225": "ti\u00f4ng-pia\u030dt",
     "\u9577\u547d": "tn\u0302g-mi\u0101",
     "\u9577\u547d\u5bcc\u8cb4": "ti\u00f4ng-b\u012bng-h\u00f9-ku\u00ec",
     "\u9577\u548c\u5bae": "Ti\u00f4ng-h\u00f4-kiong",
+    "\u9577\u5606": "ti\u00f4ng-th\u00e0n",
     "\u9577\u56db\u89d2\u5f62": "tn\u0302g-s\u00ec-kak-h\u00eeng",
     "\u9577\u57ce": "Tn\u0302g-si\u00e2nn",
     "\u9577\u5824": "ti\u00f4ng-th\u00ea",
     "\u9577\u58fd": "ti\u00f4ng-si\u016b",
     "\u9577\u58fd\u71c8": "ti\u00f4ng-si\u016b-ting",
     "\u9577\u5947": "ti\u00f4ng-k\u00ee",
     "\u9577\u5973": "ti\u00f3ng-l\u00ed/ti\u00f3ng-l\u00fa",
@@ -52285,15 +52254,14 @@
     "\u9577\u682a\u5713": "tn\u0302g-tu-\u00eenn",
     "\u9577\u6848\u684c": "ti\u00f4ng-\u00e0n-toh",
     "\u9577\u6876\u9774": "tn\u0302g-th\u00e1ng-hia",
     "\u9577\u6905\u982d\u4ed4": "tn\u0302g-\u00ed-th\u00e2u-\u00e1",
     "\u9577\u69ae": "Ti\u00f3ng-\u00eeng",
     "\u9577\u69ae\u822a\u7a7a": "ti\u00f4ng-\u00eeng-h\u00e2ng-khong",
     "\u9577\u6a02": "Ti\u00f4ng-lo\u030dk",
-    "\u9577\u6b4e": "ti\u00f4ng-th\u00e0n",
     "\u9577\u6b72\u58fd": "tn\u0302g-hu\u00e8-si\u016b/tn\u0302g-h\u00e8-si\u016b",
     "\u9577\u6c5f": "Tn\u0302g-kang",
     "\u9577\u6c5f\u4e09\u5cfd": "Tn\u0302g-kang-sann-kiap",
     "\u9577\u6c5f\u6d41\u57df": "Tn\u0302g-kang-l\u00e2u-hi\u030dk",
     "\u9577\u6c99": "Tn\u0302g-sua",
     "\u9577\u6c99\u7063": "Tn\u0302g-sua-uan",
     "\u9577\u6cbb\u4e45\u5b89": "ti\u00f4ng-t\u012b-ki\u00fa-an",
@@ -54993,15 +54961,14 @@
     "\u982d\u9999": "th\u00e2u-hiunn",
     "\u982d\u9ad3": "th\u00e2u-tshu\u00e9/th\u00e2u-tsh\u00e9",
     "\u982d\u9b03": "th\u00e2u-tsang",
     "\u982d\u9b03\u578b": "th\u00e2u-tsang-h\u00eeng",
     "\u982d\u9b03\u5c3e": "th\u00e2u-tsang-bu\u00e9/th\u00e2u-tsang-b\u00e9",
     "\u982d\u9b03\u6cb9": "th\u00e2u-tsang-i\u00fb",
     "\u982d\u9ea9": "th\u00e2u-phoo",
-    "\u982d\u9f63": "th\u00e2u-tshut",
     "\u9837": "\u0101m",
     "\u9837\u570d\u4ed4": "\u0101m-u\u00ee-\u00e1",
     "\u9837\u5782": "\u0101m-su\u00ea",
     "\u9837\u5782\u4ed4": "\u0101m-su\u00ea-\u00e1",
     "\u9837\u5782\u8c46": "\u0101m-su\u00ea-t\u0101u",
     "\u9837\u5dfe": "\u0101m-kin/\u0101m-kun",
     "\u9837\u5e36": "\u0101m-tu\u00e0",
@@ -57314,15 +57281,14 @@
     "\u9ec3\u725b": "n\u0302g-g\u00fb",
     "\u9ec3\u725b\u7968": "n\u0302g-g\u00fb-phi\u00f2",
     "\u9ec3\u74dc": "n\u0302g-kue",
     "\u9ec3\u74dc\u4ed4": "n\u0302g-kue-\u00e1",
     "\u9ec3\u74dc\u9b5a": "n\u0302g-kue-h\u00ee/n\u0302g-kue-h\u00fb",
     "\u9ec3\u75b8": "n\u0302g-th\u00e1n",
     "\u9ec3\u75e0": "n\u0302g-sng",
-    "\u9ec3\u75e0\u6876": "n\u0302g-sng-th\u00e1ng",
     "\u9ec3\u75e0\u75b8": "n\u0302g-sng-th\u00e1n",
     "\u9ec3\u75e0\u96e8": "n\u0302g-sng-h\u014do",
     "\u9ec3\u761f\u75ab": "n\u0302g-un-i\u030dk",
     "\u9ec3\u76ee\u5b50": "n\u0302g-ba\u030dk-ts\u00ed",
     "\u9ec3\u76ee\u6a39": "n\u0302g-ba\u030dk-tshi\u016b",
     "\u9ec3\u77f3": "n\u0302g-tsio\u030dh",
     "\u9ec3\u78da\u9f20": "N\u0302g-tsng-tsh\u00ed/N\u0302g-tsng-tsh\u00fa",
@@ -57694,15 +57660,14 @@
     "\u9f52\u86c7": "kh\u00ed-tsu\u00e2",
     "\u9f52\u8708\u86a3": "kh\u00ed-gi\u00e2-kang",
     "\u9f52\u87e7\u8708": "kh\u00ed-l\u00e2-gi\u00e2",
     "\u9f52\u8c46": "kh\u00ed-t\u0101u",
     "\u9f52\u8f2a": "kh\u00ed-l\u00fbn",
     "\u9f61": "l\u00eeng",
     "\u9f63": "tshut",
-    "\u9f63\u982d": "tshut-th\u00e2u",
     "\u9f67": "kh\u00e8/khu\u00e8",
     "\u9f67\u9f52\u985e": "giat-kh\u00ed-lu\u012b",
     "\u9f6a": "tsak",
     "\u9f74": "gi\u00e0ng",
     "\u9f74\u7259": "gi\u00e0ng-g\u00ea",
     "\u9f74\u7259\u9f52\u8073": "gi\u00e0ng-g\u00ea-tsh\u00ed-tsh\u00e0ng",
     "\u9f74\u9f52": "gi\u00e0ng-kh\u00ed",
```

### Comparing `taibun-1.1.2/taibun/taibun.py` & `taibun-1.1.3/taibun/taibun.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 import unicodedata
 
 data_dir = os.path.join(os.path.dirname(__file__), "data")
 with open(os.path.join(data_dir, "words.json"), 'r', encoding="utf-8") as f:
     word_dict = json.load(f)
 with open(os.path.join(data_dir, "traditional.json"), 'r', encoding="utf-8") as f:
     trad_dict = json.load(f)
+with open(os.path.join(data_dir, "simplified.json"), 'r', encoding="utf-8") as f:
+    simp_dict = {**{v: k for k, v in trad_dict.items() if len(k) == 1}, **json.load(f)}
 with open(os.path.join(data_dir, "vars.json"), 'r', encoding="utf-8") as f:
     vars_dict = json.load(f)
-simp_dict = {item: k for k, v in trad_dict.items() for item in v}
 
 # Helper to check if the character is a Chinese character
 def is_cjk(input):
     return all(
         0x4E00 <= ord(char) <= 0x9FFF or  # BASIC
         0x3400 <= ord(char) <= 0x4DBF or  # Ext A
         0x20000 <= ord(char) <= 0x2A6DF or  # Ext B
@@ -26,44 +27,26 @@
 
 # Convert Traditional to Simplified characters
 def to_simplified(input):
     return ''.join(simp_dict.get(c, c) for c in input)
 
 # Convert Simplified to Traditional characters
 def to_traditional(input):
-    return ''.join(get_best_solution(input))
-
-def get_best_solution(input):
     input = ''.join(vars_dict.get(c, c) for c in input)
-    traditional_variants = ['']
-    for c in input:
-        if c in trad_dict:
-            traditional_variants = [variant + trad for variant in traditional_variants for trad in trad_dict[c]]
-        else:
-            traditional_variants = [variant + c for variant in traditional_variants]
-    tokenised = []
-    for traditional in traditional_variants:
-        temp_tokenised = []
-        while traditional:
-            for j in range(4, 0, -1):
-                if len(traditional) < j:
-                    continue
-                word = traditional[:j]
-                if word_dict.get(word) or j == 1:
-                    if j == 1 and temp_tokenised and not (is_cjk(temp_tokenised[-1]) or is_cjk(word)):
-                        temp_tokenised[-1] += word
-                    else:
-                        temp_tokenised.append(word)
-                    traditional = traditional[j:]
-                    break
-            else:
-                traditional = ""
-        if len(temp_tokenised) < len(tokenised) or not tokenised:
-            tokenised = temp_tokenised
-    return tokenised
+    traditional = []
+    while input:
+        for j in range(4, 0, -1):
+            if len(input) < j:
+                continue
+            word = input[:j]
+            if word in trad_dict or j == 1:
+                traditional.append(trad_dict.get(word, word))
+                input = input[j:]
+                break
+    return "".join(traditional)
 
 
 """
 Description: Converts Chinese characters to Taiwanese Hokkien phonetic transcriptions.
              Supports both Traditional and Simplified characters.
 Invariant: system = `Tailo` (default), `POJ`, `Zhuyin`, `TLPA`, `Pingyim`, `Tongiong`, `IPA`
            dialect = `south` (Zhangzhou-leaning, default), `north` (Quanzhou-leaning)
@@ -444,15 +427,30 @@
 class Tokeniser(object):
 
     def __init__(self, keep_original=True):
         self.keep_original = keep_original
 
     # Tokenise the text into separate words
     def tokenise(self, input):
-        tokenised = get_best_solution(input)
+        tokenised = []
+        traditional = to_traditional(input)
+        while traditional:
+            for j in range (4, 0, -1):
+                if len(traditional) < j:
+                    continue
+                word = traditional[:j]
+                if word_dict.get(word) or j == 1:
+                    if j == 1 and tokenised and not (is_cjk(tokenised[-1]) or is_cjk(word)):
+                        tokenised[-1] += word
+                    else:
+                        tokenised.append(word)
+                    traditional = traditional[j:]
+                    break
+            else:
+                traditional = ""
         punctuations = re.compile(r"([.,!?\"#$%&()*+/:;<=>@[\]^`{|}~\t。．，、！？；：（）［］【】「」“”]\s*)")
         if self.keep_original:
             indices = [0] + [len(item) for item in tokenised]
             tokenised = [input[sum(indices[:i+1]):sum(indices[:i+2])] for i in range(len(indices)-1)]
         tokenised = [
             item 
             for word in tokenised
```

### Comparing `taibun-1.1.2/taibun.egg-info/PKG-INFO` & `taibun-1.1.3/taibun.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taibun
-Version: 1.1.2
+Version: 1.1.3
 Summary: Taiwanese Hokkien Transliterator and Tokeniser
 Home-page: https://github.com/andreihar/taibun
 Author: Andrei Harbachov
 Author-email: andrei.harbachov@gmail.com
 License: MIT
 Keywords: python,taiwan,taiwanese,taigi,hokkien,romanization,transliteration,transliterator,tokenization,tokenizer
 Classifier: Topic :: Text Processing :: Linguistic
@@ -18,15 +18,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
   <a href="https://github.com/andreihar/taibun">
-    <img src="https://github.com/andreihar/taibun/raw/main/readme/logo.png" alt="Logo" width="90" height="80">
+    <img src="[readme/logo.png](https://github.com/andreihar/taibun/raw/main/readme/logo.png)" alt="Logo" width="90" height="80">
   </a>
   
 # Taibun
 
 
 
 <!-- PROJECT SHIELDS -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: taibun Version: 1.1.2 Summary: Taiwanese Hokkien
+Metadata-Version: 2.1 Name: taibun Version: 1.1.3 Summary: Taiwanese Hokkien
 Transliterator and Tokeniser Home-page: https://github.com/andreihar/taibun
 Author: Andrei Harbachov Author-email: andrei.harbachov@gmail.com License: MIT
 Keywords:
 python,taiwan,taiwanese,taigi,hokkien,romanization,transliteration,transliterator,tokenization,tokenizer
 Classifier: Topic :: Text Processing :: Linguistic Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
```

### Comparing `taibun-1.1.2/taibun.egg-info/SOURCES.txt` & `taibun-1.1.3/taibun.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup.cfg
 taibun/__init__.py
 taibun/taibun.py
 taibun.egg-info/PKG-INFO
 taibun.egg-info/SOURCES.txt
 taibun.egg-info/dependency_links.txt
 taibun.egg-info/top_level.txt
+taibun/data/simplified.json
 taibun/data/traditional.json
 taibun/data/vars.json
 taibun/data/words.json
 tests/test_additional.py
 tests/test_convert_non_cjk.py
 tests/test_delimiter.py
 tests/test_format.py
```

### Comparing `taibun-1.1.2/tests/test_additional.py` & `taibun-1.1.3/tests/test_additional.py`

 * *Files identical despite different names*

### Comparing `taibun-1.1.2/tests/test_convert_non_cjk.py` & `taibun-1.1.3/tests/test_convert_non_cjk.py`

 * *Files identical despite different names*

### Comparing `taibun-1.1.2/tests/test_delimiter.py` & `taibun-1.1.3/tests/test_delimiter.py`

 * *Files identical despite different names*

### Comparing `taibun-1.1.2/tests/test_format.py` & `taibun-1.1.3/tests/test_format.py`

 * *Files identical despite different names*

### Comparing `taibun-1.1.2/tests/test_ipa_conversion.py` & `taibun-1.1.3/tests/test_ipa_conversion.py`

 * *Files identical despite different names*

### Comparing `taibun-1.1.2/tests/test_pingyim_conversion.py` & `taibun-1.1.3/tests/test_pingyim_conversion.py`

 * *Files identical despite different names*

### Comparing `taibun-1.1.2/tests/test_poj_conversion.py` & `taibun-1.1.3/tests/test_poj_conversion.py`

 * *Files identical despite different names*

### Comparing `taibun-1.1.2/tests/test_punctuation.py` & `taibun-1.1.3/tests/test_punctuation.py`

 * *Files identical despite different names*

### Comparing `taibun-1.1.2/tests/test_sandhi.py` & `taibun-1.1.3/tests/test_sandhi.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,63 +73,63 @@
     ]
     for transl, system in test_data:
         data = list(zip(hanji_data, transl))
         checker(data, Converter(system=system, punctuation='none', sandhi='incl_last'), Converter(system=system, dialect="north", punctuation='none', sandhi='incl_last'))
 
 def test_add_auto():
     test_data = [
-        (["biò-āng-á","āng-boo-á","bá-iu-á","huē-ta-á","bī-bī-á/bì-bī-á","bàn-bān-á","bue-iā-á/be-iā-á","tì tshú á tíng gua lé kiânn","thôo kha tshīng-khì--ah","guan tì tshù guā lang kang-tāi gí/guan tì tshù guā lang kang-tài gú","tì kōng-hn̂g lāi khùn","tsia iu tshiā-hò bô","tse tsiá kau-á pu̍t-sī è puī/tse tsiá kau-á pu̍t-sì è puī"], "Tailo"),
-        (["biò-āng-á","āng-bo͘-á","bá-iu-á","hōe-ta-á","bī-bī-á/bì-bī-á","bàn-bān-á","boe-iā-á/be-iā-á","tì chhú á téng goa lé kiâⁿ","thô͘ kha chhēng-khì--ah","goan tì chhù gōa lang kang-tāi gí/goan tì chhù gōa lang kang-tài gú","tì kōng-hn̂g lāi khùn","chia iu chhiā-hò bô","che chiá kau-á pu̍t-sī è pūi/che chiá kau-á pu̍t-sì è pūi"], "POJ"),
-        (["ㆠㄧㄜ˪ ㄤ˫ ㄚˋ","ㄤ˫ ㆠㆦ ㄚˋ","ㆠㄚˋ ㄧㄨ ㄚˋ","ㄏㄨㆤ˫ ㄉㄚ ㄚˋ","ㆠㄧ˫ ㆠㄧ˫ ㄚˋ/ㆠㄧ˪ ㆠㄧ˫ ㄚˋ","ㆠㄢ˪ ㆠㄢ˫ ㄚˋ","ㆠㄨㆤ ㄧㄚ˫ ㄚˋ/ㆠㆤ ㄧㄚ˫ ㄚˋ","ㄉㄧ˪ ㄘㄨˋ ㄚˋ ㄉㄧㄥˋ ㆣㄨㄚ ㄌㆤˋ ㄍㄧㆩˊ","ㄊㆦˊ ㄎㄚ ㄑㄧㄥ˫ ㄎㄧ˪ ㄚ","ㆣㄨㄢ ㄉㄧ˪ ㄘㄨ˪ ㆣㄨㄚ˫ ㄌㄤ ㄍㄤ ㄉㄞ˫ ㆣㄧˋ/ㆣㄨㄢ ㄉㄧ˪ ㄘㄨ˪ ㆣㄨㄚ˫ ㄌㄤ ㄍㄤ ㄉㄞ˪ ㆣㄨˋ","ㄉㄧ˪ ㄍㆲ˫ ㄏㆭˊ ㄌㄞ˫ ㄎㄨㄣ˪","ㄐㄧㄚ ㄧㄨ ㄑㄧㄚ˫ ㄏㄜ˪ ㆠㄜˊ","ㄗㆤ ㄐㄧㄚˋ ㄍㄠ ㄚˋ ㄅㄨㆵ˙ ㄒㄧ˫ ㆤ˪ ㄅㄨㄧ˫/ㄗㆤ ㄐㄧㄚˋ ㄍㄠ ㄚˋ ㄅㄨㆵ˙ ㄒㄧ˪ ㆤ˪ ㄅㄨㄧ˫"], "Zhuyin"),
-        (["bio3 ang7 a2","ang7 boo1 a2","ba2 iu1 a2","hue7 ta1 a2","bi7 bi7 a2/bi3 bi7 a2","ban3 ban7 a2","bue1 ia7 a2/be1 ia7 a2","ti3 chu2 a2 ting2 gua1 le2 kiann5","thoo5 kha1 ching7 khi3 ah0","guan1 ti3 chu3 gua7 lang1 kang1 tai7 gi2/guan1 ti3 chu3 gua7 lang1 kang1 tai3 gu2","ti3 kong7 hng5 lai7 khun3","cia1 iu1 chia7 ho3 bo5","ce1 cia2 kau1 a2 put8 si7 e3 pui7/ce1 cia2 kau1 a2 put8 si3 e3 pui7"], "TLPA"),
-        (["bbiòângǎ","ângbboōǎ","bbǎyūǎ","huêdāǎ","bbîbbîǎ/bbìbbîǎ","bbànbbânǎ","bbuēyâǎ/bbēyâǎ","dì cǔ ǎ dǐng gguā lě giná","toó kā cîngkì ah","gguān dì cù gguâ lāng gāngdâi ggǐ/gguān dì cù gguâ lāng gāngdài ggǔ","dì gônghńg lâi kùn","ziā yū ciâhò bbó","zē ziǎ gāoǎ bútsî è buî/zē ziǎ gāoǎ bútsì è buî"], "Pingyim"),
-        (["bhiôr-āng-à","āng-bhor-à","bhà-iu-à","huē-da-à","bhī-bhī-à/bhî-bhī-à","bhân-bhān-à","bhue-iā-à/bhe-iā-à","dî cù à dìng ghua lè giănn","tŏr ka cīng-kî--åh","ghuan dî cû ghuā lang gang-dāi ghì/ghuan dî cû ghuā lang gang-dâi ghù","dî gōng-hn̆g lāi kûn","zia iu ciā-hôr bhŏr","ze zià gau-à but-sī ê buī/ze zià gau-à but-sî ê buī"], "Tongiong"),
-        (["biə¹¹ aŋ²² a⁵³/bio²¹ aŋ³³ a⁵¹","aŋ²² bɔ⁴⁴ a⁵³/aŋ³³ bɔ⁵⁵ a⁵¹","ba⁵³ iu⁴⁴ a⁵³/ba⁵¹ iu⁵⁵ a⁵¹","hue²² ta⁴⁴ a⁵³/hue³³ ta⁵⁵ a⁵¹","bi²² bi²² a⁵³/bi²¹ bi³³ a⁵¹","ban¹¹ ban²² a⁵³/ban²¹ ban³³ a⁵¹","bue⁴⁴ ia²² a⁵³/be⁵⁵ ia³³ a⁵¹","ti¹¹ tsʰu⁵³ a⁵³ tiɪŋ⁵³ gua⁴⁴ le⁵³ kiã²⁵/ti²¹ tsʰu⁵¹ a⁵¹ tiɪŋ⁵¹ gua⁵⁵ le⁵¹ kiã²⁴","tʰɔ²⁵ kʰa⁴⁴ tɕʰiɪŋ²² kʰi¹¹ a/tʰɔ²⁴ kʰa⁵⁵ tɕʰiɪŋ³³ kʰi²¹ a","guan⁴⁴ ti¹¹ tsʰu¹¹ gua²² laŋ⁴⁴ kaŋ⁴⁴ tai²² gi⁵³/guan⁵⁵ ti²¹ tsʰu²¹ gua³³ laŋ⁵⁵ kaŋ⁵⁵ tai²¹ gu⁵¹","ti¹¹ kɔŋ²² hŋ̍²⁵ lai²² kʰun¹¹/ti²¹ kɔŋ³³ hŋ̍²⁴ lai³³ kʰun²¹","tɕia⁴⁴ iu⁴⁴ tɕʰia²² hə¹¹ bə²⁵/tɕia⁵⁵ iu⁵⁵ tɕʰia³³ ho²¹ bo²⁴","tse⁴⁴ tɕia⁵³ kau⁴⁴ a⁵³ put̚⁵ ɕi²² e¹¹ pui²²/tse⁵⁵ tɕia⁵¹ kau⁵⁵ a⁵¹ put̚⁴ ɕi²¹ e²¹ pui³³"], "IPA")
+        (["biò-āng-á","āng-boo-á","bá-iu-á","huē-ta-á","bī-bī-á/bì-bī-á","bàn-bān-á","bue-iā-á/be-iā-á","tì tshú á tíng gua lé kiânn","thôo kha tshīng-khì--ah","guan tì tshù guā lang kong Tāi-gí/guan tì tshù guā lang kong Tài-gú","tì kōng-hn̂g lāi khùn","tsia iu tshiā-hò bô","tse tsiá kau-á pu̍t-sī è puī/tse tsiá kau-á pu̍t-sì è puī"], "Tailo"),
+        (["biò-āng-á","āng-bo͘-á","bá-iu-á","hōe-ta-á","bī-bī-á/bì-bī-á","bàn-bān-á","boe-iā-á/be-iā-á","tì chhú á téng goa lé kiâⁿ","thô͘ kha chhēng-khì--ah","goan tì chhù gōa lang kong Tāi-gí/goan tì chhù gōa lang kong Tài-gú","tì kōng-hn̂g lāi khùn","chia iu chhiā-hò bô","che chiá kau-á pu̍t-sī è pūi/che chiá kau-á pu̍t-sì è pūi"], "POJ"),
+        (["ㆠㄧㄜ˪ ㄤ˫ ㄚˋ","ㄤ˫ ㆠㆦ ㄚˋ","ㆠㄚˋ ㄧㄨ ㄚˋ","ㄏㄨㆤ˫ ㄉㄚ ㄚˋ","ㆠㄧ˫ ㆠㄧ˫ ㄚˋ/ㆠㄧ˪ ㆠㄧ˫ ㄚˋ","ㆠㄢ˪ ㆠㄢ˫ ㄚˋ","ㆠㄨㆤ ㄧㄚ˫ ㄚˋ/ㆠㆤ ㄧㄚ˫ ㄚˋ","ㄉㄧ˪ ㄘㄨˋ ㄚˋ ㄉㄧㄥˋ ㆣㄨㄚ ㄌㆤˋ ㄍㄧㆩˊ","ㄊㆦˊ ㄎㄚ ㄑㄧㄥ˫ ㄎㄧ˪ ㄚ","ㆣㄨㄢ ㄉㄧ˪ ㄘㄨ˪ ㆣㄨㄚ˫ ㄌㄤ ㄍㆲ ㄉㄞ˫ ㆣㄧˋ/ㆣㄨㄢ ㄉㄧ˪ ㄘㄨ˪ ㆣㄨㄚ˫ ㄌㄤ ㄍㆲ ㄉㄞ˪ ㆣㄨˋ","ㄉㄧ˪ ㄍㆲ˫ ㄏㆭˊ ㄌㄞ˫ ㄎㄨㄣ˪","ㄐㄧㄚ ㄧㄨ ㄑㄧㄚ˫ ㄏㄜ˪ ㆠㄜˊ","ㄗㆤ ㄐㄧㄚˋ ㄍㄠ ㄚˋ ㄅㄨㆵ˙ ㄒㄧ˫ ㆤ˪ ㄅㄨㄧ˫/ㄗㆤ ㄐㄧㄚˋ ㄍㄠ ㄚˋ ㄅㄨㆵ˙ ㄒㄧ˪ ㆤ˪ ㄅㄨㄧ˫"], "Zhuyin"),
+        (["bio3 ang7 a2","ang7 boo1 a2","ba2 iu1 a2","hue7 ta1 a2","bi7 bi7 a2/bi3 bi7 a2","ban3 ban7 a2","bue1 ia7 a2/be1 ia7 a2","ti3 chu2 a2 ting2 gua1 le2 kiann5","thoo5 kha1 ching7 khi3 ah0","guan1 ti3 chu3 gua7 lang1 kong1 Tai7 gi2/guan1 ti3 chu3 gua7 lang1 kong1 Tai3 gu2","ti3 kong7 hng5 lai7 khun3","cia1 iu1 chia7 ho3 bo5","ce1 cia2 kau1 a2 put8 si7 e3 pui7/ce1 cia2 kau1 a2 put8 si3 e3 pui7"], "TLPA"),
+        (["bbiòângǎ","ângbboōǎ","bbǎyūǎ","huêdāǎ","bbîbbîǎ/bbìbbîǎ","bbànbbânǎ","bbuēyâǎ/bbēyâǎ","dì cǔ ǎ dǐng gguā lě giná","toó kā cîngkì ah","gguān dì cù gguâ lāng gōng Dâiggǐ/gguān dì cù gguâ lāng gōng Dàiggǔ","dì gônghńg lâi kùn","ziā yū ciâhò bbó","zē ziǎ gāoǎ bútsî è buî/zē ziǎ gāoǎ bútsì è buî"], "Pingyim"),
+        (["bhiôr-āng-à","āng-bhor-à","bhà-iu-à","huē-da-à","bhī-bhī-à/bhî-bhī-à","bhân-bhān-à","bhue-iā-à/bhe-iā-à","dî cù à dìng ghua lè giănn","tŏr ka cīng-kî--åh","ghuan dî cû ghuā lang gong Dāi-ghì/ghuan dî cû ghuā lang gong Dâi-ghù","dî gōng-hn̆g lāi kûn","zia iu ciā-hôr bhŏr","ze zià gau-à but-sī ê buī/ze zià gau-à but-sî ê buī"], "Tongiong"),
+        (["biə¹¹ aŋ²² a⁵³/bio²¹ aŋ³³ a⁵¹","aŋ²² bɔ⁴⁴ a⁵³/aŋ³³ bɔ⁵⁵ a⁵¹","ba⁵³ iu⁴⁴ a⁵³/ba⁵¹ iu⁵⁵ a⁵¹","hue²² ta⁴⁴ a⁵³/hue³³ ta⁵⁵ a⁵¹","bi²² bi²² a⁵³/bi²¹ bi³³ a⁵¹","ban¹¹ ban²² a⁵³/ban²¹ ban³³ a⁵¹","bue⁴⁴ ia²² a⁵³/be⁵⁵ ia³³ a⁵¹","ti¹¹ tsʰu⁵³ a⁵³ tiɪŋ⁵³ gua⁴⁴ le⁵³ kiã²⁵/ti²¹ tsʰu⁵¹ a⁵¹ tiɪŋ⁵¹ gua⁵⁵ le⁵¹ kiã²⁴","tʰɔ²⁵ kʰa⁴⁴ tɕʰiɪŋ²² kʰi¹¹ a/tʰɔ²⁴ kʰa⁵⁵ tɕʰiɪŋ³³ kʰi²¹ a","guan⁴⁴ ti¹¹ tsʰu¹¹ gua²² laŋ⁴⁴ kɔŋ⁴⁴ Tai²² gi⁵³/guan⁵⁵ ti²¹ tsʰu²¹ gua³³ laŋ⁵⁵ kɔŋ⁵⁵ Tai²¹ gu⁵¹","ti¹¹ kɔŋ²² hŋ̍²⁵ lai²² kʰun¹¹/ti²¹ kɔŋ³³ hŋ̍²⁴ lai³³ kʰun²¹","tɕia⁴⁴ iu⁴⁴ tɕʰia²² hə¹¹ bə²⁵/tɕia⁵⁵ iu⁵⁵ tɕʰia³³ ho²¹ bo²⁴","tse⁴⁴ tɕia⁵³ kau⁴⁴ a⁵³ put̚⁵ ɕi²² e¹¹ pui²²/tse⁵⁵ tɕia⁵¹ kau⁵⁵ a⁵¹ put̚⁴ ɕi²¹ e²¹ pui³³"], "IPA")
     ]
     for transl, system in test_data:
         data = list(zip(hanji_a, transl))
         checker(data, Converter(system=system, punctuation='none', sandhi='auto'), Converter(system=system, dialect="north", punctuation='none', sandhi='auto'))
 
 def test_add_none():
     test_data = [
-        (["biō-ang-á","ang-bóo-á","bah-iù-á","hue-tah-á","bî-bî-á","bān-bān-á","bué-ia̍h-á/bé-ia̍h-á","tī tshù á tíng guá leh kiânn","thôo kha tshing-khì--ah","guán tī tshù guā láng káng-tâi gí/guán tī tshù guā láng káng-tâi gú","tī kong-hn̂g lāi khùn","tsia iú tshia-hō bô","tse tsiah káu-á put-sî ē puī"], "Tailo"),
-        (["biō-ang-á","ang-bó͘-á","bah-iù-á","hoe-tah-á","bî-bî-á","bān-bān-á","bóe-ia̍h-á/bé-ia̍h-á","tī chhù á téng góa leh kiâⁿ","thô͘ kha chheng-khì--ah","goán tī chhù gōa láng káng-tâi gí/goán tī chhù gōa láng káng-tâi gú","tī kong-hn̂g lāi khùn","chia iú chhia-hō bô","che chiah káu-á put-sî ē pūi"], "POJ"),
-        (["ㆠㄧㄜ˫ ㄤ ㄚˋ","ㄤ ㆠㆦˋ ㄚˋ","ㆠㄚㆷ ㄧㄨ˪ ㄚˋ","ㄏㄨㆤ ㄉㄚㆷ ㄚˋ","ㆠㄧˊ ㆠㄧˊ ㄚˋ","ㆠㄢ˫ ㆠㄢ˫ ㄚˋ","ㆠㄨㆤˋ ㄧㄚㆷ˙ ㄚˋ/ㆠㆤˋ ㄧㄚㆷ˙ ㄚˋ","ㄉㄧ˫ ㄘㄨ˪ ㄚˋ ㄉㄧㄥˋ ㆣㄨㄚˋ ㄌㆤㆷ ㄍㄧㆩˊ","ㄊㆦˊ ㄎㄚ ㄑㄧㄥ ㄎㄧ˪ ㄚ","ㆣㄨㄢˋ ㄉㄧ˫ ㄘㄨ˪ ㆣㄨㄚ˫ ㄌㄤˋ ㄍㄤˋ ㄉㄞˊ ㆣㄧˋ/ㆣㄨㄢˋ ㄉㄧ˫ ㄘㄨ˪ ㆣㄨㄚ˫ ㄌㄤˋ ㄍㄤˋ ㄉㄞˊ ㆣㄨˋ","ㄉㄧ˫ ㄍㆲ ㄏㆭˊ ㄌㄞ˫ ㄎㄨㄣ˪","ㄐㄧㄚ ㄧㄨˋ ㄑㄧㄚ ㄏㄜ˫ ㆠㄜˊ","ㄗㆤ ㄐㄧㄚㆷ ㄍㄠˋ ㄚˋ ㄅㄨㆵ ㄒㄧˊ ㆤ˫ ㄅㄨㄧ˫"], "Zhuyin"),
-        (["bio7 ang1 a2","ang1 boo2 a2","bah4 iu3 a2","hue1 tah4 a2","bi5 bi5 a2","ban7 ban7 a2","bue2 iah8 a2/be2 iah8 a2","ti7 chu3 a2 ting2 gua2 leh4 kiann5","thoo5 kha1 ching1 khi3 ah0","guan2 ti7 chu3 gua7 lang2 kang2 tai5 gi2/guan2 ti7 chu3 gua7 lang2 kang2 tai5 gu2","ti7 kong1 hng5 lai7 khun3","cia1 iu2 chia1 ho7 bo5","ce1 ciah4 kau2 a2 put4 si5 e7 pui7"], "TLPA"),
-        (["bbiôāngǎ","āngbboǒǎ","bbāhyùǎ","huēdāhǎ","bbíbbíǎ","bbânbbânǎ","bbuěyáhǎ/bběyáhǎ","dî cù ǎ dǐng gguǎ lēh giná","toó kā cīngkì ah","gguǎn dî cù gguâ lǎng gǎngdái ggǐ/gguǎn dî cù gguâ lǎng gǎngdái ggǔ","dî gōnghńg lâi kùn","ziā yǔ ciāhô bbó","zē ziāh gǎoǎ būtsí ê buî"], "Pingyim"),
-        (["bhiōr-ang-à","ang-bhòr-à","bhāh-iû-à","hue-dāh-à","bhĭ-bhĭ-à","bhān-bhān-à","bhuè-iah-à/bhè-iah-à","dī cû à dìng ghuà lēh giănn","tŏr ka cing-kî--åh","ghuàn dī cû ghuā làng gàng-dăi ghì/ghuàn dī cû ghuā làng gàng-dăi ghù","dī gong-hn̆g lāi kûn","zia iù cia-hōr bhŏr","ze ziāh gàu-à būt-sĭ ē buī"], "Tongiong"),
-        (["biə²² aŋ⁴⁴ a⁵³/bio³³ aŋ⁵⁵ a⁵¹","aŋ⁴⁴ bɔ⁵³ a⁵³/aŋ⁵⁵ bɔ⁵¹ a⁵¹","baʔ²¹ iu¹¹ a⁵³/baʔ³² iu²¹ a⁵¹","hue⁴⁴ taʔ²¹ a⁵³/hue⁵⁵ taʔ³² a⁵¹","bi²⁵ bi²⁵ a⁵³/bi²⁴ bi²⁴ a⁵¹","ban²² ban²² a⁵³/ban³³ ban³³ a⁵¹","bue⁵³ iaʔ⁵ a⁵³/be⁵¹ iaʔ⁴ a⁵¹","ti²² tsʰu¹¹ a⁵³ tiɪŋ⁵³ gua⁵³ leʔ²¹ kiã²⁵/ti³³ tsʰu²¹ a⁵¹ tiɪŋ⁵¹ gua⁵¹ leʔ³² kiã²⁴","tʰɔ²⁵ kʰa⁴⁴ tɕʰiɪŋ⁴⁴ kʰi¹¹ a/tʰɔ²⁴ kʰa⁵⁵ tɕʰiɪŋ⁵⁵ kʰi²¹ a","guan⁵³ ti²² tsʰu¹¹ gua²² laŋ⁵³ kaŋ⁵³ tai²⁵ gi⁵³/guan⁵¹ ti³³ tsʰu²¹ gua³³ laŋ⁵¹ kaŋ⁵¹ tai²⁴ gu⁵¹","ti²² kɔŋ⁴⁴ hŋ̍²⁵ lai²² kʰun¹¹/ti³³ kɔŋ⁵⁵ hŋ̍²⁴ lai³³ kʰun²¹","tɕia⁴⁴ iu⁵³ tɕʰia⁴⁴ hə²² bə²⁵/tɕia⁵⁵ iu⁵¹ tɕʰia⁵⁵ ho³³ bo²⁴","tse⁴⁴ tɕiaʔ²¹ kau⁵³ a⁵³ put̚²¹ ɕi²⁵ e²² pui²²/tse⁵⁵ tɕiaʔ³² kau⁵¹ a⁵¹ put̚³² ɕi²⁴ e³³ pui³³"], "IPA")
+        (["biō-ang-á","ang-bóo-á","bah-iù-á","hue-tah-á","bî-bî-á","bān-bān-á","bué-ia̍h-á/bé-ia̍h-á","tī tshù á tíng guá leh kiânn","thôo kha tshing-khì--ah","guán tī tshù guā láng kóng Tâi-gí/guán tī tshù guā láng kóng Tâi-gú","tī kong-hn̂g lāi khùn","tsia iú tshia-hō bô","tse tsiah káu-á put-sî ē puī"], "Tailo"),
+        (["biō-ang-á","ang-bó͘-á","bah-iù-á","hoe-tah-á","bî-bî-á","bān-bān-á","bóe-ia̍h-á/bé-ia̍h-á","tī chhù á téng góa leh kiâⁿ","thô͘ kha chheng-khì--ah","goán tī chhù gōa láng kóng Tâi-gí/goán tī chhù gōa láng kóng Tâi-gú","tī kong-hn̂g lāi khùn","chia iú chhia-hō bô","che chiah káu-á put-sî ē pūi"], "POJ"),
+        (["ㆠㄧㄜ˫ ㄤ ㄚˋ","ㄤ ㆠㆦˋ ㄚˋ","ㆠㄚㆷ ㄧㄨ˪ ㄚˋ","ㄏㄨㆤ ㄉㄚㆷ ㄚˋ","ㆠㄧˊ ㆠㄧˊ ㄚˋ","ㆠㄢ˫ ㆠㄢ˫ ㄚˋ","ㆠㄨㆤˋ ㄧㄚㆷ˙ ㄚˋ/ㆠㆤˋ ㄧㄚㆷ˙ ㄚˋ","ㄉㄧ˫ ㄘㄨ˪ ㄚˋ ㄉㄧㄥˋ ㆣㄨㄚˋ ㄌㆤㆷ ㄍㄧㆩˊ","ㄊㆦˊ ㄎㄚ ㄑㄧㄥ ㄎㄧ˪ ㄚ","ㆣㄨㄢˋ ㄉㄧ˫ ㄘㄨ˪ ㆣㄨㄚ˫ ㄌㄤˋ ㄍㆲˋ ㄉㄞˊ ㆣㄧˋ/ㆣㄨㄢˋ ㄉㄧ˫ ㄘㄨ˪ ㆣㄨㄚ˫ ㄌㄤˋ ㄍㆲˋ ㄉㄞˊ ㆣㄨˋ","ㄉㄧ˫ ㄍㆲ ㄏㆭˊ ㄌㄞ˫ ㄎㄨㄣ˪","ㄐㄧㄚ ㄧㄨˋ ㄑㄧㄚ ㄏㄜ˫ ㆠㄜˊ","ㄗㆤ ㄐㄧㄚㆷ ㄍㄠˋ ㄚˋ ㄅㄨㆵ ㄒㄧˊ ㆤ˫ ㄅㄨㄧ˫"], "Zhuyin"),
+        (["bio7 ang1 a2","ang1 boo2 a2","bah4 iu3 a2","hue1 tah4 a2","bi5 bi5 a2","ban7 ban7 a2","bue2 iah8 a2/be2 iah8 a2","ti7 chu3 a2 ting2 gua2 leh4 kiann5","thoo5 kha1 ching1 khi3 ah0","guan2 ti7 chu3 gua7 lang2 kong2 Tai5 gi2/guan2 ti7 chu3 gua7 lang2 kong2 Tai5 gu2","ti7 kong1 hng5 lai7 khun3","cia1 iu2 chia1 ho7 bo5","ce1 ciah4 kau2 a2 put4 si5 e7 pui7"], "TLPA"),
+        (["bbiôāngǎ","āngbboǒǎ","bbāhyùǎ","huēdāhǎ","bbíbbíǎ","bbânbbânǎ","bbuěyáhǎ/bběyáhǎ","dî cù ǎ dǐng gguǎ lēh giná","toó kā cīngkì ah","gguǎn dî cù gguâ lǎng gǒng Dáiggǐ/gguǎn dî cù gguâ lǎng gǒng Dáiggǔ","dî gōnghńg lâi kùn","ziā yǔ ciāhô bbó","zē ziāh gǎoǎ būtsí ê buî"], "Pingyim"),
+        (["bhiōr-ang-à","ang-bhòr-à","bhāh-iû-à","hue-dāh-à","bhĭ-bhĭ-à","bhān-bhān-à","bhuè-iah-à/bhè-iah-à","dī cû à dìng ghuà lēh giănn","tŏr ka cing-kî--åh","ghuàn dī cû ghuā làng gòng Dăi-ghì/ghuàn dī cû ghuā làng gòng Dăi-ghù","dī gong-hn̆g lāi kûn","zia iù cia-hōr bhŏr","ze ziāh gàu-à būt-sĭ ē buī"], "Tongiong"),
+        (["biə²² aŋ⁴⁴ a⁵³/bio³³ aŋ⁵⁵ a⁵¹","aŋ⁴⁴ bɔ⁵³ a⁵³/aŋ⁵⁵ bɔ⁵¹ a⁵¹","baʔ²¹ iu¹¹ a⁵³/baʔ³² iu²¹ a⁵¹","hue⁴⁴ taʔ²¹ a⁵³/hue⁵⁵ taʔ³² a⁵¹","bi²⁵ bi²⁵ a⁵³/bi²⁴ bi²⁴ a⁵¹","ban²² ban²² a⁵³/ban³³ ban³³ a⁵¹","bue⁵³ iaʔ⁵ a⁵³/be⁵¹ iaʔ⁴ a⁵¹","ti²² tsʰu¹¹ a⁵³ tiɪŋ⁵³ gua⁵³ leʔ²¹ kiã²⁵/ti³³ tsʰu²¹ a⁵¹ tiɪŋ⁵¹ gua⁵¹ leʔ³² kiã²⁴","tʰɔ²⁵ kʰa⁴⁴ tɕʰiɪŋ⁴⁴ kʰi¹¹ a/tʰɔ²⁴ kʰa⁵⁵ tɕʰiɪŋ⁵⁵ kʰi²¹ a","guan⁵³ ti²² tsʰu¹¹ gua²² laŋ⁵³ kɔŋ⁵³ Tai²⁵ gi⁵³/guan⁵¹ ti³³ tsʰu²¹ gua³³ laŋ⁵¹ kɔŋ⁵¹ Tai²⁴ gu⁵¹","ti²² kɔŋ⁴⁴ hŋ̍²⁵ lai²² kʰun¹¹/ti³³ kɔŋ⁵⁵ hŋ̍²⁴ lai³³ kʰun²¹","tɕia⁴⁴ iu⁵³ tɕʰia⁴⁴ hə²² bə²⁵/tɕia⁵⁵ iu⁵¹ tɕʰia⁵⁵ ho³³ bo²⁴","tse⁴⁴ tɕiaʔ²¹ kau⁵³ a⁵³ put̚²¹ ɕi²⁵ e²² pui²²/tse⁵⁵ tɕiaʔ³² kau⁵¹ a⁵¹ put̚³² ɕi²⁴ e³³ pui³³"], "IPA")
     ]
     for transl, system in test_data:
         data = list(zip(hanji_a, transl))
         checker(data, Converter(system=system, punctuation='none', sandhi='none'), Converter(system=system, dialect="north", punctuation='none', sandhi='none'))
 
 def test_add_exc_last():
     test_data = [
-        (["biò-āng-á","āng-boo-á","bá-iú-á","huē-tá-á","bī-bī-á/bì-bì-á","bàn-bàn-á","bue-ià-á/be-ià-á","tì tshú a ting gua lé kiânn","thōo khā tshīng-khì--ah/thòo khā tshīng-khì--ah","guan tì tshú guà lang kang-tāi gí/guan tì tshú guà lang kang-tài gú","tì kōng-hn̄g lài khùn/tì kōng-hǹg lài khùn","tsiā iu tshiā-hò bô","tsē tsiá kau-a pu̍t-sī è puī/tsē tsiá kau-a pu̍t-sì è puī"], "Tailo"),
-        (["biò-āng-á","āng-bo͘-á","bá-iú-á","hōe-tá-á","bī-bī-á/bì-bì-á","bàn-bàn-á","boe-ià-á/be-ià-á","tì chhú a teng goa lé kiâⁿ","thō͘ khā chhēng-khì--ah/thò͘ khā chhēng-khì--ah","goan tì chhú gòa lang kang-tāi gí/goan tì chhú gòa lang kang-tài gú","tì kōng-hn̄g lài khùn/tì kōng-hǹg lài khùn","chiā iu chhiā-hò bô","chē chiá kau-a pu̍t-sī è pūi/chē chiá kau-a pu̍t-sì è pūi"], "POJ"),
-        (["ㆠㄧㄜ˪ ㄤ˫ ㄚˋ","ㄤ˫ ㆠㆦ ㄚˋ","ㆠㄚˋ ㄧㄨˋ ㄚˋ","ㄏㄨㆤ˫ ㄉㄚˋ ㄚˋ","ㆠㄧ˫ ㆠㄧ˫ ㄚˋ/ㆠㄧ˪ ㆠㄧ˪ ㄚˋ","ㆠㄢ˪ ㆠㄢ˪ ㄚˋ","ㆠㄨㆤ ㄧㄚ˪ ㄚˋ/ㆠㆤ ㄧㄚ˪ ㄚˋ","ㄉㄧ˪ ㄘㄨˋ ㄚ ㄉㄧㄥ ㆣㄨㄚ ㄌㆤˋ ㄍㄧㆩˊ","ㄊㆦ˫ ㄎㄚ˫ ㄑㄧㄥ˫ ㄎㄧ˪ ㄚ/ㄊㆦ˪ ㄎㄚ˫ ㄑㄧㄥ˫ ㄎㄧ˪ ㄚ","ㆣㄨㄢ ㄉㄧ˪ ㄘㄨˋ ㆣㄨㄚ˪ ㄌㄤ ㄍㄤ ㄉㄞ˫ ㆣㄧˋ/ㆣㄨㄢ ㄉㄧ˪ ㄘㄨˋ ㆣㄨㄚ˪ ㄌㄤ ㄍㄤ ㄉㄞ˪ ㆣㄨˋ","ㄉㄧ˪ ㄍㆲ˫ ㄏㆭ˫ ㄌㄞ˪ ㄎㄨㄣ˪/ㄉㄧ˪ ㄍㆲ˫ ㄏㆭ˪ ㄌㄞ˪ ㄎㄨㄣ˪","ㄐㄧㄚ˫ ㄧㄨ ㄑㄧㄚ˫ ㄏㄜ˪ ㆠㄜˊ","ㄗㆤ˫ ㄐㄧㄚˋ ㄍㄠ ㄚ ㄅㄨㆵ˙ ㄒㄧ˫ ㆤ˪ ㄅㄨㄧ˫/ㄗㆤ˫ ㄐㄧㄚˋ ㄍㄠ ㄚ ㄅㄨㆵ˙ ㄒㄧ˪ ㆤ˪ ㄅㄨㄧ˫"], "Zhuyin"),
-        (["bio3 ang7 a2","ang7 boo1 a2","ba2 iu2 a2","hue7 ta2 a2","bi7 bi7 a2/bi3 bi3 a2","ban3 ban3 a2","bue1 ia3 a2/be1 ia3 a2","ti3 chu2 a1 ting1 gua1 le2 kiann5","thoo7 kha7 ching7 khi3 ah0/thoo3 kha7 ching7 khi3 ah0","guan1 ti3 chu2 gua3 lang1 kang1 tai7 gi2/guan1 ti3 chu2 gua3 lang1 kang1 tai3 gu2","ti3 kong7 hng7 lai3 khun3/ti3 kong7 hng3 lai3 khun3","cia7 iu1 chia7 ho3 bo5","ce7 cia2 kau1 a1 put8 si7 e3 pui7/ce7 cia2 kau1 a1 put8 si3 e3 pui7"], "TLPA"),
-        (["bbiòângǎ","ângbboōǎ","bbǎyǔǎ","huêdǎǎ","bbîbbîǎ/bbìbbìǎ","bbànbbànǎ","bbuēyàǎ/bbēyàǎ","dì cǔ ā dīng gguā lě giná","toô kâ cîngkì ah/toò kâ cîngkì ah","gguān dì cǔ gguà lāng gāngdâi ggǐ/gguān dì cǔ gguà lāng gāngdài ggǔ","dì gônghn̂g lài kùn/dì gônghǹg lài kùn","ziâ yū ciâhò bbó","zê ziǎ gāoā bútsî è buî/zê ziǎ gāoā bútsì è buî"], "Pingyim"),
-        (["bhiôr-āng-à","āng-bhor-à","bhà-iù-à","huē-dà-à","bhī-bhī-à/bhî-bhî-à","bhân-bhân-à","bhue-iâ-à/bhe-iâ-à","dî cù a ding ghua lè giănn","tōr kā cīng-kî--åh/tôr kā cīng-kî--åh","ghuan dî cù ghuâ lang gang-dāi ghì/ghuan dî cù ghuâ lang gang-dâi ghù","dî gōng-hn̄g lâi kûn/dî gōng-hn̂g lâi kûn","ziā iu ciā-hôr bhŏr","zē zià gau-a but-sī ê buī/zē zià gau-a but-sî ê buī"], "Tongiong"),
-        (["biə¹¹ aŋ²² a⁵³/bio²¹ aŋ³³ a⁵¹","aŋ²² bɔ⁴⁴ a⁵³/aŋ³³ bɔ⁵⁵ a⁵¹","ba⁵³ iu⁵³ a⁵³/ba⁵¹ iu⁵¹ a⁵¹","hue²² ta⁵³ a⁵³/hue³³ ta⁵¹ a⁵¹","bi²² bi²² a⁵³/bi²¹ bi²¹ a⁵¹","ban¹¹ ban¹¹ a⁵³/ban²¹ ban²¹ a⁵¹","bue⁴⁴ ia¹¹ a⁵³/be⁵⁵ ia²¹ a⁵¹","ti¹¹ tsʰu⁵³ a⁴⁴ tiɪŋ⁴⁴ gua⁴⁴ le⁵³ kiã²⁵/ti²¹ tsʰu⁵¹ a⁵⁵ tiɪŋ⁵⁵ gua⁵⁵ le⁵¹ kiã²⁴","tʰɔ²² kʰa²² tɕʰiɪŋ²² kʰi¹¹ a/tʰɔ²¹ kʰa³³ tɕʰiɪŋ³³ kʰi²¹ a","guan⁴⁴ ti¹¹ tsʰu⁵³ gua¹¹ laŋ⁴⁴ kaŋ⁴⁴ tai²² gi⁵³/guan⁵⁵ ti²¹ tsʰu⁵¹ gua²¹ laŋ⁵⁵ kaŋ⁵⁵ tai²¹ gu⁵¹","ti¹¹ kɔŋ²² hŋ̍²² lai¹¹ kʰun¹¹/ti²¹ kɔŋ³³ hŋ̍²¹ lai²¹ kʰun²¹","tɕia²² iu⁴⁴ tɕʰia²² hə¹¹ bə²⁵/tɕia³³ iu⁵⁵ tɕʰia³³ ho²¹ bo²⁴","tse²² tɕia⁵³ kau⁴⁴ a⁴⁴ put̚⁵ ɕi²² e¹¹ pui²²/tse³³ tɕia⁵¹ kau⁵⁵ a⁵⁵ put̚⁴ ɕi²¹ e²¹ pui³³"], "IPA")
+        (["biò-āng-á","āng-boo-á","bá-iú-á","huē-tá-á","bī-bī-á/bì-bì-á","bàn-bàn-á","bue-ià-á/be-ià-á","tì tshú a ting gua lé kiânn","thōo khā tshīng-khì--ah/thòo khā tshīng-khì--ah","guan tì tshú guà lang kong Tāi-gí/guan tì tshú guà lang kong Tài-gú","tì kōng-hn̄g lài khùn/tì kōng-hǹg lài khùn","tsiā iu tshiā-hò bô","tsē tsiá kau-a pu̍t-sī è puī/tsē tsiá kau-a pu̍t-sì è puī"], "Tailo"),
+        (["biò-āng-á","āng-bo͘-á","bá-iú-á","hōe-tá-á","bī-bī-á/bì-bì-á","bàn-bàn-á","boe-ià-á/be-ià-á","tì chhú a teng goa lé kiâⁿ","thō͘ khā chhēng-khì--ah/thò͘ khā chhēng-khì--ah","goan tì chhú gòa lang kong Tāi-gí/goan tì chhú gòa lang kong Tài-gú","tì kōng-hn̄g lài khùn/tì kōng-hǹg lài khùn","chiā iu chhiā-hò bô","chē chiá kau-a pu̍t-sī è pūi/chē chiá kau-a pu̍t-sì è pūi"], "POJ"),
+        (["ㆠㄧㄜ˪ ㄤ˫ ㄚˋ","ㄤ˫ ㆠㆦ ㄚˋ","ㆠㄚˋ ㄧㄨˋ ㄚˋ","ㄏㄨㆤ˫ ㄉㄚˋ ㄚˋ","ㆠㄧ˫ ㆠㄧ˫ ㄚˋ/ㆠㄧ˪ ㆠㄧ˪ ㄚˋ","ㆠㄢ˪ ㆠㄢ˪ ㄚˋ","ㆠㄨㆤ ㄧㄚ˪ ㄚˋ/ㆠㆤ ㄧㄚ˪ ㄚˋ","ㄉㄧ˪ ㄘㄨˋ ㄚ ㄉㄧㄥ ㆣㄨㄚ ㄌㆤˋ ㄍㄧㆩˊ","ㄊㆦ˫ ㄎㄚ˫ ㄑㄧㄥ˫ ㄎㄧ˪ ㄚ/ㄊㆦ˪ ㄎㄚ˫ ㄑㄧㄥ˫ ㄎㄧ˪ ㄚ","ㆣㄨㄢ ㄉㄧ˪ ㄘㄨˋ ㆣㄨㄚ˪ ㄌㄤ ㄍㆲ ㄉㄞ˫ ㆣㄧˋ/ㆣㄨㄢ ㄉㄧ˪ ㄘㄨˋ ㆣㄨㄚ˪ ㄌㄤ ㄍㆲ ㄉㄞ˪ ㆣㄨˋ","ㄉㄧ˪ ㄍㆲ˫ ㄏㆭ˫ ㄌㄞ˪ ㄎㄨㄣ˪/ㄉㄧ˪ ㄍㆲ˫ ㄏㆭ˪ ㄌㄞ˪ ㄎㄨㄣ˪","ㄐㄧㄚ˫ ㄧㄨ ㄑㄧㄚ˫ ㄏㄜ˪ ㆠㄜˊ","ㄗㆤ˫ ㄐㄧㄚˋ ㄍㄠ ㄚ ㄅㄨㆵ˙ ㄒㄧ˫ ㆤ˪ ㄅㄨㄧ˫/ㄗㆤ˫ ㄐㄧㄚˋ ㄍㄠ ㄚ ㄅㄨㆵ˙ ㄒㄧ˪ ㆤ˪ ㄅㄨㄧ˫"], "Zhuyin"),
+        (["bio3 ang7 a2","ang7 boo1 a2","ba2 iu2 a2","hue7 ta2 a2","bi7 bi7 a2/bi3 bi3 a2","ban3 ban3 a2","bue1 ia3 a2/be1 ia3 a2","ti3 chu2 a1 ting1 gua1 le2 kiann5","thoo7 kha7 ching7 khi3 ah0/thoo3 kha7 ching7 khi3 ah0","guan1 ti3 chu2 gua3 lang1 kong1 Tai7 gi2/guan1 ti3 chu2 gua3 lang1 kong1 Tai3 gu2","ti3 kong7 hng7 lai3 khun3/ti3 kong7 hng3 lai3 khun3","cia7 iu1 chia7 ho3 bo5","ce7 cia2 kau1 a1 put8 si7 e3 pui7/ce7 cia2 kau1 a1 put8 si3 e3 pui7"], "TLPA"),
+        (["bbiòângǎ","ângbboōǎ","bbǎyǔǎ","huêdǎǎ","bbîbbîǎ/bbìbbìǎ","bbànbbànǎ","bbuēyàǎ/bbēyàǎ","dì cǔ ā dīng gguā lě giná","toô kâ cîngkì ah/toò kâ cîngkì ah","gguān dì cǔ gguà lāng gōng Dâiggǐ/gguān dì cǔ gguà lāng gōng Dàiggǔ","dì gônghn̂g lài kùn/dì gônghǹg lài kùn","ziâ yū ciâhò bbó","zê ziǎ gāoā bútsî è buî/zê ziǎ gāoā bútsì è buî"], "Pingyim"),
+        (["bhiôr-āng-à","āng-bhor-à","bhà-iù-à","huē-dà-à","bhī-bhī-à/bhî-bhî-à","bhân-bhân-à","bhue-iâ-à/bhe-iâ-à","dî cù a ding ghua lè giănn","tōr kā cīng-kî--åh/tôr kā cīng-kî--åh","ghuan dî cù ghuâ lang gong Dāi-ghì/ghuan dî cù ghuâ lang gong Dâi-ghù","dî gōng-hn̄g lâi kûn/dî gōng-hn̂g lâi kûn","ziā iu ciā-hôr bhŏr","zē zià gau-a but-sī ê buī/zē zià gau-a but-sî ê buī"], "Tongiong"),
+        (["biə¹¹ aŋ²² a⁵³/bio²¹ aŋ³³ a⁵¹","aŋ²² bɔ⁴⁴ a⁵³/aŋ³³ bɔ⁵⁵ a⁵¹","ba⁵³ iu⁵³ a⁵³/ba⁵¹ iu⁵¹ a⁵¹","hue²² ta⁵³ a⁵³/hue³³ ta⁵¹ a⁵¹","bi²² bi²² a⁵³/bi²¹ bi²¹ a⁵¹","ban¹¹ ban¹¹ a⁵³/ban²¹ ban²¹ a⁵¹","bue⁴⁴ ia¹¹ a⁵³/be⁵⁵ ia²¹ a⁵¹","ti¹¹ tsʰu⁵³ a⁴⁴ tiɪŋ⁴⁴ gua⁴⁴ le⁵³ kiã²⁵/ti²¹ tsʰu⁵¹ a⁵⁵ tiɪŋ⁵⁵ gua⁵⁵ le⁵¹ kiã²⁴","tʰɔ²² kʰa²² tɕʰiɪŋ²² kʰi¹¹ a/tʰɔ²¹ kʰa³³ tɕʰiɪŋ³³ kʰi²¹ a","guan⁴⁴ ti¹¹ tsʰu⁵³ gua¹¹ laŋ⁴⁴ kɔŋ⁴⁴ Tai²² gi⁵³/guan⁵⁵ ti²¹ tsʰu⁵¹ gua²¹ laŋ⁵⁵ kɔŋ⁵⁵ Tai²¹ gu⁵¹","ti¹¹ kɔŋ²² hŋ̍²² lai¹¹ kʰun¹¹/ti²¹ kɔŋ³³ hŋ̍²¹ lai²¹ kʰun²¹","tɕia²² iu⁴⁴ tɕʰia²² hə¹¹ bə²⁵/tɕia³³ iu⁵⁵ tɕʰia³³ ho²¹ bo²⁴","tse²² tɕia⁵³ kau⁴⁴ a⁴⁴ put̚⁵ ɕi²² e¹¹ pui²²/tse³³ tɕia⁵¹ kau⁵⁵ a⁵⁵ put̚⁴ ɕi²¹ e²¹ pui³³"], "IPA")
     ]
     for transl, system in test_data:
         data = list(zip(hanji_a, transl))
         checker(data, Converter(system=system, punctuation='none', sandhi='exc_last'), Converter(system=system, dialect="north", punctuation='none', sandhi='exc_last'))
 
 def test_add_incl_last():
     test_data = [
-        (["biò-āng-a","āng-boo-a","bá-iú-a","huē-tá-a","bī-bī-a/bì-bì-a","bàn-bàn-a","bue-ià-a/be-ià-a","tì tshú a ting gua lé kiānn/tì tshú a ting gua lé kiànn","thōo khā tshīng-khì--ah/thòo khā tshīng-khì--ah","guan tì tshú guà lang kang-tāi gi/guan tì tshú guà lang kang-tài gu","tì kōng-hn̄g lài khún/tì kōng-hǹg lài khún","tsiā iu tshiā-hò bō/tsiā iu tshiā-hò bò","tsē tsiá kau-a pu̍t-sī è puì/tsē tsiá kau-a pu̍t-sì è puì"], "Tailo"),
-        (["biò-āng-a","āng-bo͘-a","bá-iú-a","hōe-tá-a","bī-bī-a/bì-bì-a","bàn-bàn-a","boe-ià-a/be-ià-a","tì chhú a teng goa lé kiāⁿ/tì chhú a teng goa lé kiàⁿ","thō͘ khā chhēng-khì--ah/thò͘ khā chhēng-khì--ah","goan tì chhú gòa lang kang-tāi gi/goan tì chhú gòa lang kang-tài gu","tì kōng-hn̄g lài khún/tì kōng-hǹg lài khún","chiā iu chhiā-hò bō/chiā iu chhiā-hò bò","chē chiá kau-a pu̍t-sī è pùi/chē chiá kau-a pu̍t-sì è pùi"], "POJ"),
-        (["ㆠㄧㄜ˪ ㄤ˫ ㄚ","ㄤ˫ ㆠㆦ ㄚ","ㆠㄚˋ ㄧㄨˋ ㄚ","ㄏㄨㆤ˫ ㄉㄚˋ ㄚ","ㆠㄧ˫ ㆠㄧ˫ ㄚ/ㆠㄧ˪ ㆠㄧ˪ ㄚ","ㆠㄢ˪ ㆠㄢ˪ ㄚ","ㆠㄨㆤ ㄧㄚ˪ ㄚ/ㆠㆤ ㄧㄚ˪ ㄚ","ㄉㄧ˪ ㄘㄨˋ ㄚ ㄉㄧㄥ ㆣㄨㄚ ㄌㆤˋ ㄍㄧㆩ˫/ㄉㄧ˪ ㄘㄨˋ ㄚ ㄉㄧㄥ ㆣㄨㄚ ㄌㆤˋ ㄍㄧㆩ˪","ㄊㆦ˫ ㄎㄚ˫ ㄑㄧㄥ˫ ㄎㄧ˪ ㄚ/ㄊㆦ˪ ㄎㄚ˫ ㄑㄧㄥ˫ ㄎㄧ˪ ㄚ","ㆣㄨㄢ ㄉㄧ˪ ㄘㄨˋ ㆣㄨㄚ˪ ㄌㄤ ㄍㄤ ㄉㄞ˫ ㆣㄧ/ㆣㄨㄢ ㄉㄧ˪ ㄘㄨˋ ㆣㄨㄚ˪ ㄌㄤ ㄍㄤ ㄉㄞ˪ ㆣㄨ","ㄉㄧ˪ ㄍㆲ˫ ㄏㆭ˫ ㄌㄞ˪ ㄎㄨㄣˋ/ㄉㄧ˪ ㄍㆲ˫ ㄏㆭ˪ ㄌㄞ˪ ㄎㄨㄣˋ","ㄐㄧㄚ˫ ㄧㄨ ㄑㄧㄚ˫ ㄏㄜ˪ ㆠㄜ˫/ㄐㄧㄚ˫ ㄧㄨ ㄑㄧㄚ˫ ㄏㄜ˪ ㆠㄜ˪","ㄗㆤ˫ ㄐㄧㄚˋ ㄍㄠ ㄚ ㄅㄨㆵ˙ ㄒㄧ˫ ㆤ˪ ㄅㄨㄧ˪/ㄗㆤ˫ ㄐㄧㄚˋ ㄍㄠ ㄚ ㄅㄨㆵ˙ ㄒㄧ˪ ㆤ˪ ㄅㄨㄧ˪"], "Zhuyin"),
-        (["bio3 ang7 a1","ang7 boo1 a1","ba2 iu2 a1","hue7 ta2 a1","bi7 bi7 a1/bi3 bi3 a1","ban3 ban3 a1","bue1 ia3 a1/be1 ia3 a1","ti3 chu2 a1 ting1 gua1 le2 kiann7/ti3 chu2 a1 ting1 gua1 le2 kiann3","thoo7 kha7 ching7 khi3 ah0/thoo3 kha7 ching7 khi3 ah0","guan1 ti3 chu2 gua3 lang1 kang1 tai7 gi1/guan1 ti3 chu2 gua3 lang1 kang1 tai3 gu1","ti3 kong7 hng7 lai3 khun2/ti3 kong7 hng3 lai3 khun2","cia7 iu1 chia7 ho3 bo7/cia7 iu1 chia7 ho3 bo3","ce7 cia2 kau1 a1 put8 si7 e3 pui3/ce7 cia2 kau1 a1 put8 si3 e3 pui3"], "TLPA"),
-        (["bbiòângā","ângbboōā","bbǎyǔā","huêdǎā","bbîbbîā/bbìbbìā","bbànbbànā","bbuēyàā/bbēyàā","dì cǔ ā dīng gguā lě ginâ/dì cǔ ā dīng gguā lě ginà","toô kâ cîngkì ah/toò kâ cîngkì ah","gguān dì cǔ gguà lāng gāngdâi ggī/gguān dì cǔ gguà lāng gāngdài ggū","dì gônghn̂g lài kǔn/dì gônghǹg lài kǔn","ziâ yū ciâhò bbô/ziâ yū ciâhò bbò","zê ziǎ gāoā bútsî è buì/zê ziǎ gāoā bútsì è buì"], "Pingyim"),
-        (["bhiôr-āng-a","āng-bhor-a","bhà-iù-a","huē-dà-a","bhī-bhī-a/bhî-bhî-a","bhân-bhân-a","bhue-iâ-a/bhe-iâ-a","dî cù a ding ghua lè giānn/dî cù a ding ghua lè giânn","tōr kā cīng-kî--åh/tôr kā cīng-kî--åh","ghuan dî cù ghuâ lang gang-dāi ghi/ghuan dî cù ghuâ lang gang-dâi ghu","dî gōng-hn̄g lâi kùn/dî gōng-hn̂g lâi kùn","ziā iu ciā-hôr bhōr/ziā iu ciā-hôr bhôr","zē zià gau-a but-sī ê buî/zē zià gau-a but-sî ê buî"], "Tongiong"),
-        (["biə¹¹ aŋ²² a⁴⁴/bio²¹ aŋ³³ a⁵⁵","aŋ²² bɔ⁴⁴ a⁴⁴/aŋ³³ bɔ⁵⁵ a⁵⁵","ba⁵³ iu⁵³ a⁴⁴/ba⁵¹ iu⁵¹ a⁵⁵","hue²² ta⁵³ a⁴⁴/hue³³ ta⁵¹ a⁵⁵","bi²² bi²² a⁴⁴/bi²¹ bi²¹ a⁵⁵","ban¹¹ ban¹¹ a⁴⁴/ban²¹ ban²¹ a⁵⁵","bue⁴⁴ ia¹¹ a⁴⁴/be⁵⁵ ia²¹ a⁵⁵","ti¹¹ tsʰu⁵³ a⁴⁴ tiɪŋ⁴⁴ gua⁴⁴ le⁵³ kiã²²/ti²¹ tsʰu⁵¹ a⁵⁵ tiɪŋ⁵⁵ gua⁵⁵ le⁵¹ kiã²¹","tʰɔ²² kʰa²² tɕʰiɪŋ²² kʰi¹¹ a/tʰɔ²¹ kʰa³³ tɕʰiɪŋ³³ kʰi²¹ a","guan⁴⁴ ti¹¹ tsʰu⁵³ gua¹¹ laŋ⁴⁴ kaŋ⁴⁴ tai²² gi⁴⁴/guan⁵⁵ ti²¹ tsʰu⁵¹ gua²¹ laŋ⁵⁵ kaŋ⁵⁵ tai²¹ gu⁵⁵","ti¹¹ kɔŋ²² hŋ̍²² lai¹¹ kʰun⁵³/ti²¹ kɔŋ³³ hŋ̍²¹ lai²¹ kʰun⁵¹","tɕia²² iu⁴⁴ tɕʰia²² hə¹¹ bə²²/tɕia³³ iu⁵⁵ tɕʰia³³ ho²¹ bo²¹","tse²² tɕia⁵³ kau⁴⁴ a⁴⁴ put̚⁵ ɕi²² e¹¹ pui¹¹/tse³³ tɕia⁵¹ kau⁵⁵ a⁵⁵ put̚⁴ ɕi²¹ e²¹ pui²¹"], "IPA")
+        (["biò-āng-a","āng-boo-a","bá-iú-a","huē-tá-a","bī-bī-a/bì-bì-a","bàn-bàn-a","bue-ià-a/be-ià-a","tì tshú a ting gua lé kiānn/tì tshú a ting gua lé kiànn","thōo khā tshīng-khì--ah/thòo khā tshīng-khì--ah","guan tì tshú guà lang kong Tāi-gi/guan tì tshú guà lang kong Tài-gu","tì kōng-hn̄g lài khún/tì kōng-hǹg lài khún","tsiā iu tshiā-hò bō/tsiā iu tshiā-hò bò","tsē tsiá kau-a pu̍t-sī è puì/tsē tsiá kau-a pu̍t-sì è puì"], "Tailo"),
+        (["biò-āng-a","āng-bo͘-a","bá-iú-a","hōe-tá-a","bī-bī-a/bì-bì-a","bàn-bàn-a","boe-ià-a/be-ià-a","tì chhú a teng goa lé kiāⁿ/tì chhú a teng goa lé kiàⁿ","thō͘ khā chhēng-khì--ah/thò͘ khā chhēng-khì--ah","goan tì chhú gòa lang kong Tāi-gi/goan tì chhú gòa lang kong Tài-gu","tì kōng-hn̄g lài khún/tì kōng-hǹg lài khún","chiā iu chhiā-hò bō/chiā iu chhiā-hò bò","chē chiá kau-a pu̍t-sī è pùi/chē chiá kau-a pu̍t-sì è pùi"], "POJ"),
+        (["ㆠㄧㄜ˪ ㄤ˫ ㄚ","ㄤ˫ ㆠㆦ ㄚ","ㆠㄚˋ ㄧㄨˋ ㄚ","ㄏㄨㆤ˫ ㄉㄚˋ ㄚ","ㆠㄧ˫ ㆠㄧ˫ ㄚ/ㆠㄧ˪ ㆠㄧ˪ ㄚ","ㆠㄢ˪ ㆠㄢ˪ ㄚ","ㆠㄨㆤ ㄧㄚ˪ ㄚ/ㆠㆤ ㄧㄚ˪ ㄚ","ㄉㄧ˪ ㄘㄨˋ ㄚ ㄉㄧㄥ ㆣㄨㄚ ㄌㆤˋ ㄍㄧㆩ˫/ㄉㄧ˪ ㄘㄨˋ ㄚ ㄉㄧㄥ ㆣㄨㄚ ㄌㆤˋ ㄍㄧㆩ˪","ㄊㆦ˫ ㄎㄚ˫ ㄑㄧㄥ˫ ㄎㄧ˪ ㄚ/ㄊㆦ˪ ㄎㄚ˫ ㄑㄧㄥ˫ ㄎㄧ˪ ㄚ","ㆣㄨㄢ ㄉㄧ˪ ㄘㄨˋ ㆣㄨㄚ˪ ㄌㄤ ㄍㆲ ㄉㄞ˫ ㆣㄧ/ㆣㄨㄢ ㄉㄧ˪ ㄘㄨˋ ㆣㄨㄚ˪ ㄌㄤ ㄍㆲ ㄉㄞ˪ ㆣㄨ","ㄉㄧ˪ ㄍㆲ˫ ㄏㆭ˫ ㄌㄞ˪ ㄎㄨㄣˋ/ㄉㄧ˪ ㄍㆲ˫ ㄏㆭ˪ ㄌㄞ˪ ㄎㄨㄣˋ","ㄐㄧㄚ˫ ㄧㄨ ㄑㄧㄚ˫ ㄏㄜ˪ ㆠㄜ˫/ㄐㄧㄚ˫ ㄧㄨ ㄑㄧㄚ˫ ㄏㄜ˪ ㆠㄜ˪","ㄗㆤ˫ ㄐㄧㄚˋ ㄍㄠ ㄚ ㄅㄨㆵ˙ ㄒㄧ˫ ㆤ˪ ㄅㄨㄧ˪/ㄗㆤ˫ ㄐㄧㄚˋ ㄍㄠ ㄚ ㄅㄨㆵ˙ ㄒㄧ˪ ㆤ˪ ㄅㄨㄧ˪"], "Zhuyin"),
+        (["bio3 ang7 a1","ang7 boo1 a1","ba2 iu2 a1","hue7 ta2 a1","bi7 bi7 a1/bi3 bi3 a1","ban3 ban3 a1","bue1 ia3 a1/be1 ia3 a1","ti3 chu2 a1 ting1 gua1 le2 kiann7/ti3 chu2 a1 ting1 gua1 le2 kiann3","thoo7 kha7 ching7 khi3 ah0/thoo3 kha7 ching7 khi3 ah0","guan1 ti3 chu2 gua3 lang1 kong1 Tai7 gi1/guan1 ti3 chu2 gua3 lang1 kong1 Tai3 gu1","ti3 kong7 hng7 lai3 khun2/ti3 kong7 hng3 lai3 khun2","cia7 iu1 chia7 ho3 bo7/cia7 iu1 chia7 ho3 bo3","ce7 cia2 kau1 a1 put8 si7 e3 pui3/ce7 cia2 kau1 a1 put8 si3 e3 pui3"], "TLPA"),
+        (["bbiòângā","ângbboōā","bbǎyǔā","huêdǎā","bbîbbîā/bbìbbìā","bbànbbànā","bbuēyàā/bbēyàā","dì cǔ ā dīng gguā lě ginâ/dì cǔ ā dīng gguā lě ginà","toô kâ cîngkì ah/toò kâ cîngkì ah","gguān dì cǔ gguà lāng gōng Dâiggī/gguān dì cǔ gguà lāng gōng Dàiggū","dì gônghn̂g lài kǔn/dì gônghǹg lài kǔn","ziâ yū ciâhò bbô/ziâ yū ciâhò bbò","zê ziǎ gāoā bútsî è buì/zê ziǎ gāoā bútsì è buì"], "Pingyim"),
+        (["bhiôr-āng-a","āng-bhor-a","bhà-iù-a","huē-dà-a","bhī-bhī-a/bhî-bhî-a","bhân-bhân-a","bhue-iâ-a/bhe-iâ-a","dî cù a ding ghua lè giānn/dî cù a ding ghua lè giânn","tōr kā cīng-kî--åh/tôr kā cīng-kî--åh","ghuan dî cù ghuâ lang gong Dāi-ghi/ghuan dî cù ghuâ lang gong Dâi-ghu","dî gōng-hn̄g lâi kùn/dî gōng-hn̂g lâi kùn","ziā iu ciā-hôr bhōr/ziā iu ciā-hôr bhôr","zē zià gau-a but-sī ê buî/zē zià gau-a but-sî ê buî"], "Tongiong"),
+        (["biə¹¹ aŋ²² a⁴⁴/bio²¹ aŋ³³ a⁵⁵","aŋ²² bɔ⁴⁴ a⁴⁴/aŋ³³ bɔ⁵⁵ a⁵⁵","ba⁵³ iu⁵³ a⁴⁴/ba⁵¹ iu⁵¹ a⁵⁵","hue²² ta⁵³ a⁴⁴/hue³³ ta⁵¹ a⁵⁵","bi²² bi²² a⁴⁴/bi²¹ bi²¹ a⁵⁵","ban¹¹ ban¹¹ a⁴⁴/ban²¹ ban²¹ a⁵⁵","bue⁴⁴ ia¹¹ a⁴⁴/be⁵⁵ ia²¹ a⁵⁵","ti¹¹ tsʰu⁵³ a⁴⁴ tiɪŋ⁴⁴ gua⁴⁴ le⁵³ kiã²²/ti²¹ tsʰu⁵¹ a⁵⁵ tiɪŋ⁵⁵ gua⁵⁵ le⁵¹ kiã²¹","tʰɔ²² kʰa²² tɕʰiɪŋ²² kʰi¹¹ a/tʰɔ²¹ kʰa³³ tɕʰiɪŋ³³ kʰi²¹ a","guan⁴⁴ ti¹¹ tsʰu⁵³ gua¹¹ laŋ⁴⁴ kɔŋ⁴⁴ Tai²² gi⁴⁴/guan⁵⁵ ti²¹ tsʰu⁵¹ gua²¹ laŋ⁵⁵ kɔŋ⁵⁵ Tai²¹ gu⁵⁵","ti¹¹ kɔŋ²² hŋ̍²² lai¹¹ kʰun⁵³/ti²¹ kɔŋ³³ hŋ̍²¹ lai²¹ kʰun⁵¹","tɕia²² iu⁴⁴ tɕʰia²² hə¹¹ bə²²/tɕia³³ iu⁵⁵ tɕʰia³³ ho²¹ bo²¹","tse²² tɕia⁵³ kau⁴⁴ a⁴⁴ put̚⁵ ɕi²² e¹¹ pui¹¹/tse³³ tɕia⁵¹ kau⁵⁵ a⁵⁵ put̚⁴ ɕi²¹ e²¹ pui²¹"], "IPA")
     ]
     for transl, system in test_data:
         data = list(zip(hanji_a, transl))
         checker(data, Converter(system=system, punctuation='none', sandhi='incl_last'), Converter(system=system, dialect="north", punctuation='none', sandhi='incl_last'))
 
 def test_sentence_auto():
     test_data = [
```

### Comparing `taibun-1.1.2/tests/test_tailo_conversion.py` & `taibun-1.1.3/tests/test_tailo_conversion.py`

 * *Files identical despite different names*

### Comparing `taibun-1.1.2/tests/test_tlpa_conversion.py` & `taibun-1.1.3/tests/test_tlpa_conversion.py`

 * *Files identical despite different names*

### Comparing `taibun-1.1.2/tests/test_tokenisation.py` & `taibun-1.1.3/tests/test_tokenisation.py`

 * *Files identical despite different names*

### Comparing `taibun-1.1.2/tests/test_tongiong_conversion.py` & `taibun-1.1.3/tests/test_tongiong_conversion.py`

 * *Files identical despite different names*

### Comparing `taibun-1.1.2/tests/test_zhuyin_conversion.py` & `taibun-1.1.3/tests/test_zhuyin_conversion.py`

 * *Files identical despite different names*

