# Comparing `tmp/cambridge-3.9.4.tar.gz` & `tmp/cambridge-3.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cambridge-3.9.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cambridge-3.9.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cambridge-3.9.4.tar` & `cambridge-3.9.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       72 2024-03-03 06:01:31.364439 cambridge-3.9.4/.gitignore
--rw-r--r--   0        0        0    32422 2022-09-14 04:27:11.000000 cambridge-3.9.4/LICENSE
--rw-r--r--   0        0        0     4122 2024-03-06 13:40:28.754758 cambridge-3.9.4/README.md
--rw-r--r--   0        0        0      266 2024-03-30 03:39:49.973183 cambridge-3.9.4/cambridge/__init__.py
--rw-r--r--   0        0        0     9591 2024-03-14 06:49:30.831288 cambridge-3.9.4/cambridge/args.py
--rw-r--r--   0        0        0     2306 2024-03-10 16:30:26.328948 cambridge-3.9.4/cambridge/cache.py
--rw-r--r--   0        0        0     1769 2024-03-05 14:25:39.637097 cambridge-3.9.4/cambridge/color.py
--rw-r--r--   0        0        0     3075 2024-03-14 13:37:53.187305 cambridge-3.9.4/cambridge/console.py
--rw-r--r--   0        0        0    18565 2024-03-14 06:49:30.832165 cambridge-3.9.4/cambridge/dicts/cambridge.py
--rw-r--r--   0        0        0     5598 2024-03-11 05:51:17.784462 cambridge-3.9.4/cambridge/dicts/dict.py
--rw-r--r--   0        0        0    47679 2024-03-30 03:39:49.975334 cambridge-3.9.4/cambridge/dicts/webster.py
--rw-r--r--   0        0        0      770 2024-03-11 05:51:25.317401 cambridge-3.9.4/cambridge/errors.py
--rw-r--r--   0        0        0      599 2024-03-05 14:25:39.642688 cambridge-3.9.4/cambridge/log.py
--rw-r--r--   0        0        0      682 2024-03-05 14:25:39.643531 cambridge-3.9.4/cambridge/main.py
--rw-r--r--   0        0        0     2561 2024-03-13 08:59:30.744980 cambridge-3.9.4/cambridge/utils.py
--rw-r--r--   0        0        0      731 2024-03-03 06:01:31.379053 cambridge-3.9.4/pyproject.toml
--rw-r--r--   0        0        0       45 2024-03-03 06:01:31.380018 cambridge-3.9.4/requirements.txt
--rw-r--r--   0        0        0   430578 2024-03-06 13:51:33.866712 cambridge-3.9.4/screenshots/cambridge.png
--rw-r--r--   0        0        0   338780 2023-08-21 11:28:38.010650 cambridge-3.9.4/screenshots/fzf.png
--rw-r--r--   0        0        0   228507 2023-11-10 15:57:56.401249 cambridge-3.9.4/screenshots/webster.png
--rw-r--r--   0        0        0     4827 1970-01-01 00:00:00.000000 cambridge-3.9.4/PKG-INFO
+-rw-r--r--   0        0        0       72 2024-03-03 06:01:31.364439 cambridge-3.9.5/.gitignore
+-rw-r--r--   0        0        0    32422 2022-09-14 04:27:11.000000 cambridge-3.9.5/LICENSE
+-rw-r--r--   0        0        0     4122 2024-03-06 13:40:28.754758 cambridge-3.9.5/README.md
+-rw-r--r--   0        0        0      266 2024-05-20 04:57:50.982394 cambridge-3.9.5/cambridge/__init__.py
+-rw-r--r--   0        0        0     9591 2024-03-14 06:49:30.831288 cambridge-3.9.5/cambridge/args.py
+-rw-r--r--   0        0        0     2306 2024-04-02 14:57:17.675678 cambridge-3.9.5/cambridge/cache.py
+-rw-r--r--   0        0        0     1769 2024-03-05 14:25:39.637097 cambridge-3.9.5/cambridge/color.py
+-rw-r--r--   0        0        0     3076 2024-04-28 03:52:00.789105 cambridge-3.9.5/cambridge/console.py
+-rw-r--r--   0        0        0    18565 2024-03-14 06:49:30.832165 cambridge-3.9.5/cambridge/dicts/cambridge.py
+-rw-r--r--   0        0        0     5591 2024-04-11 02:16:45.056855 cambridge-3.9.5/cambridge/dicts/dict.py
+-rw-r--r--   0        0        0    47547 2024-05-20 04:46:21.156373 cambridge-3.9.5/cambridge/dicts/webster.py
+-rw-r--r--   0        0        0      770 2024-03-11 05:51:25.317401 cambridge-3.9.5/cambridge/errors.py
+-rw-r--r--   0        0        0      599 2024-03-05 14:25:39.642688 cambridge-3.9.5/cambridge/log.py
+-rw-r--r--   0        0        0      682 2024-03-05 14:25:39.643531 cambridge-3.9.5/cambridge/main.py
+-rw-r--r--   0        0        0     2561 2024-03-13 08:59:30.744980 cambridge-3.9.5/cambridge/utils.py
+-rw-r--r--   0        0        0      731 2024-03-03 06:01:31.379053 cambridge-3.9.5/pyproject.toml
+-rw-r--r--   0        0        0       45 2024-03-03 06:01:31.380018 cambridge-3.9.5/requirements.txt
+-rw-r--r--   0        0        0   430578 2024-03-06 13:51:33.866712 cambridge-3.9.5/screenshots/cambridge.png
+-rw-r--r--   0        0        0   338780 2023-08-21 11:28:38.010650 cambridge-3.9.5/screenshots/fzf.png
+-rw-r--r--   0        0        0   228507 2023-11-10 15:57:56.401249 cambridge-3.9.5/screenshots/webster.png
+-rw-r--r--   0        0        0     4827 1970-01-01 00:00:00.000000 cambridge-3.9.5/PKG-INFO
```

### Comparing `cambridge-3.9.4/LICENSE` & `cambridge-3.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.4/README.md` & `cambridge-3.9.5/README.md`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.4/cambridge/args.py` & `cambridge-3.9.5/cambridge/args.py`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.4/cambridge/cache.py` & `cambridge-3.9.5/cambridge/cache.py`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.4/cambridge/color.py` & `cambridge-3.9.5/cambridge/color.py`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.4/cambridge/console.py` & `cambridge-3.9.5/cambridge/console.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,20 +8,21 @@
     Optional,
     Literal
 )
 
 JustifyMethod = Literal["left", "center", "right"]
 
 Symbol = {
-    "L_BRACKET" : "[",
-    "R_BRACKET" : "]",
-    "SLASH"     : "/",
-    "HASH"      : "#"
+    "L_BRACKET" : '[',
+    "R_BRACKET" : ']',
+    "SLASH"     : '/',
+    "HASH"      : '#'
 }
 
+
 def hex_to_rgb(hex):
     h = hex[1:]
     return tuple(int(h[i : i + 2], 16) for i in (0, 2, 4))
 
 
 def get_color_escape(r, g, b, background=False):
     return '\033[{};2;{};{};{}m'.format(48 if background else 38, r, g, b)
```

### Comparing `cambridge-3.9.4/cambridge/dicts/cambridge.py` & `cambridge-3.9.5/cambridge/dicts/cambridge.py`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.4/cambridge/dicts/dict.py` & `cambridge-3.9.5/cambridge/dicts/dict.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         c_print("[bold]%2d" % (count+1), end="")
         if dict == DICT.MERRIAM_WEBSTER.name:
             c_print("[#4A7D95] %s" % sug)
         else:
             print("\033[34m" + " " + sug + "\033[0m")
 
     c_print(f"Press [NUMBER] to look up the suggestion inferred from the unfound [red]{input_word}[/red], [ENTER] to toggle dictionary, or [ANY OTHER KEY] to exit: ", end="")
-    key = input("\033[1m")
+    key = input("")
     if key.isnumeric() and (1 <= int(key) <= len(suggestions)):
         if dict == DICT.MERRIAM_WEBSTER.name:
             webster.search_webster(con, cur, suggestions[int(key) - 1])
         if dict == DICT.CAMBRIDGE.name:
            cambridge.search_cambridge(con, cur, suggestions[int(key) - 1], False, is_ch)
     elif key == "":
         if dict == DICT.CAMBRIDGE.name:
```

### Comparing `cambridge-3.9.4/cambridge/dicts/webster.py` & `cambridge-3.9.5/cambridge/dicts/webster.py`

 * *Files 1% similar despite different names*

```diff
@@ -357,17 +357,17 @@
             for i in child.getchildren():
                 if i.attrib["class"] == "vl":
                     print_or_badge(i.text)
                 else:
                     c_print(f"[{w_col.ph_item} bold]{i.text}", end = "\n")
 
 
-###########################################
-# parse and print related phrases
-###########################################
+##########################################################
+# parse and print related phrases (Phrases Containing ...)
+##########################################################
 
 def related_phrases(node):
     print()
 
     children = node.getchildren()
 
     title = children[1]
@@ -386,23 +386,18 @@
     phrases = [] # li tags, each tag has one phrase
     for i in pr_sec.iterdescendants():
         if i.tag == "li":
             phrases.append(i)
 
     for phrase in phrases:
         ts = list(phrase.itertext())
-        for t in ts:
-            t = t.strip("\n").strip()
-            if t != ts[-1]:
-                c_print(f"[{w_col.rph_item}]{t}", end="")
-            else:
-                if phrase != phrases[-1]:
-                    c_print(f"[{w_col.rph_item}]{t},", end=" ")
-                else:
-                    c_print(f"[{w_col.rph_item}]{t}", end="")
+        if phrase != phrases[-1]:
+            c_print(f"[{w_col.rph_item}]{ts[1]},", end=" ")
+        else:
+            c_print(f"[{w_col.rph_item}]{ts[1]}", end="")
 
 
 ###########################################
 # parse and print dictionary-entry-[number]
 ###########################################
 
 # --- parse class "vg" --- #
```

### Comparing `cambridge-3.9.4/cambridge/errors.py` & `cambridge-3.9.5/cambridge/errors.py`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.4/cambridge/log.py` & `cambridge-3.9.5/cambridge/log.py`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.4/cambridge/main.py` & `cambridge-3.9.5/cambridge/main.py`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.4/cambridge/utils.py` & `cambridge-3.9.5/cambridge/utils.py`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.4/pyproject.toml` & `cambridge-3.9.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.4/screenshots/cambridge.png` & `cambridge-3.9.5/screenshots/cambridge.png`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.4/screenshots/fzf.png` & `cambridge-3.9.5/screenshots/fzf.png`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.4/screenshots/webster.png` & `cambridge-3.9.5/screenshots/webster.png`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.4/PKG-INFO` & `cambridge-3.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cambridge
-Version: 3.9.4
+Version: 3.9.5
 Summary: cambridge is a terminal version of Cambridge Dictionary.
 Home-page: https://github.com/KateWang2016/cambridge
 Keywords: dictionary, cambridge, webster, English, web scraping, python
 Author: Kate Wang
 Author-email: kate.wang2018@gmail.com
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

