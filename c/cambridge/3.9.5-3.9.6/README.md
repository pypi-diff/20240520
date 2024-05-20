# Comparing `tmp/cambridge-3.9.5.tar.gz` & `tmp/cambridge-3.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cambridge-3.9.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cambridge-3.9.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cambridge-3.9.5.tar` & `cambridge-3.9.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       72 2024-03-03 06:01:31.364439 cambridge-3.9.5/.gitignore
--rw-r--r--   0        0        0    32422 2022-09-14 04:27:11.000000 cambridge-3.9.5/LICENSE
--rw-r--r--   0        0        0     4122 2024-03-06 13:40:28.754758 cambridge-3.9.5/README.md
--rw-r--r--   0        0        0      266 2024-05-20 04:57:50.982394 cambridge-3.9.5/cambridge/__init__.py
--rw-r--r--   0        0        0     9591 2024-03-14 06:49:30.831288 cambridge-3.9.5/cambridge/args.py
--rw-r--r--   0        0        0     2306 2024-04-02 14:57:17.675678 cambridge-3.9.5/cambridge/cache.py
--rw-r--r--   0        0        0     1769 2024-03-05 14:25:39.637097 cambridge-3.9.5/cambridge/color.py
--rw-r--r--   0        0        0     3076 2024-04-28 03:52:00.789105 cambridge-3.9.5/cambridge/console.py
--rw-r--r--   0        0        0    18565 2024-03-14 06:49:30.832165 cambridge-3.9.5/cambridge/dicts/cambridge.py
--rw-r--r--   0        0        0     5591 2024-04-11 02:16:45.056855 cambridge-3.9.5/cambridge/dicts/dict.py
--rw-r--r--   0        0        0    47547 2024-05-20 04:46:21.156373 cambridge-3.9.5/cambridge/dicts/webster.py
--rw-r--r--   0        0        0      770 2024-03-11 05:51:25.317401 cambridge-3.9.5/cambridge/errors.py
--rw-r--r--   0        0        0      599 2024-03-05 14:25:39.642688 cambridge-3.9.5/cambridge/log.py
--rw-r--r--   0        0        0      682 2024-03-05 14:25:39.643531 cambridge-3.9.5/cambridge/main.py
--rw-r--r--   0        0        0     2561 2024-03-13 08:59:30.744980 cambridge-3.9.5/cambridge/utils.py
--rw-r--r--   0        0        0      731 2024-03-03 06:01:31.379053 cambridge-3.9.5/pyproject.toml
--rw-r--r--   0        0        0       45 2024-03-03 06:01:31.380018 cambridge-3.9.5/requirements.txt
--rw-r--r--   0        0        0   430578 2024-03-06 13:51:33.866712 cambridge-3.9.5/screenshots/cambridge.png
--rw-r--r--   0        0        0   338780 2023-08-21 11:28:38.010650 cambridge-3.9.5/screenshots/fzf.png
--rw-r--r--   0        0        0   228507 2023-11-10 15:57:56.401249 cambridge-3.9.5/screenshots/webster.png
--rw-r--r--   0        0        0     4827 1970-01-01 00:00:00.000000 cambridge-3.9.5/PKG-INFO
+-rw-r--r--   0        0        0       72 2024-03-03 06:01:31.364439 cambridge-3.9.6/.gitignore
+-rw-r--r--   0        0        0    32422 2022-09-14 04:27:11.000000 cambridge-3.9.6/LICENSE
+-rw-r--r--   0        0        0     4122 2024-03-06 13:40:28.754758 cambridge-3.9.6/README.md
+-rw-r--r--   0        0        0      266 2024-05-20 15:27:35.310334 cambridge-3.9.6/cambridge/__init__.py
+-rw-r--r--   0        0        0     9591 2024-03-14 06:49:30.831288 cambridge-3.9.6/cambridge/args.py
+-rw-r--r--   0        0        0     2306 2024-04-02 14:57:17.675678 cambridge-3.9.6/cambridge/cache.py
+-rw-r--r--   0        0        0     1769 2024-03-05 14:25:39.637097 cambridge-3.9.6/cambridge/color.py
+-rw-r--r--   0        0        0     3076 2024-04-28 03:52:00.789105 cambridge-3.9.6/cambridge/console.py
+-rw-r--r--   0        0        0    18565 2024-03-14 06:49:30.832165 cambridge-3.9.6/cambridge/dicts/cambridge.py
+-rw-r--r--   0        0        0     5591 2024-04-11 02:16:45.056855 cambridge-3.9.6/cambridge/dicts/dict.py
+-rw-r--r--   0        0        0    47633 2024-05-20 15:26:43.897515 cambridge-3.9.6/cambridge/dicts/webster.py
+-rw-r--r--   0        0        0      770 2024-03-11 05:51:25.317401 cambridge-3.9.6/cambridge/errors.py
+-rw-r--r--   0        0        0      599 2024-03-05 14:25:39.642688 cambridge-3.9.6/cambridge/log.py
+-rw-r--r--   0        0        0      682 2024-03-05 14:25:39.643531 cambridge-3.9.6/cambridge/main.py
+-rw-r--r--   0        0        0     2561 2024-03-13 08:59:30.744980 cambridge-3.9.6/cambridge/utils.py
+-rw-r--r--   0        0        0      731 2024-03-03 06:01:31.379053 cambridge-3.9.6/pyproject.toml
+-rw-r--r--   0        0        0       45 2024-03-03 06:01:31.380018 cambridge-3.9.6/requirements.txt
+-rw-r--r--   0        0        0   430578 2024-03-06 13:51:33.866712 cambridge-3.9.6/screenshots/cambridge.png
+-rw-r--r--   0        0        0   338780 2023-08-21 11:28:38.010650 cambridge-3.9.6/screenshots/fzf.png
+-rw-r--r--   0        0        0   228507 2023-11-10 15:57:56.401249 cambridge-3.9.6/screenshots/webster.png
+-rw-r--r--   0        0        0     4827 1970-01-01 00:00:00.000000 cambridge-3.9.6/PKG-INFO
```

### Comparing `cambridge-3.9.5/LICENSE` & `cambridge-3.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.5/README.md` & `cambridge-3.9.6/README.md`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.5/cambridge/args.py` & `cambridge-3.9.6/cambridge/args.py`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.5/cambridge/cache.py` & `cambridge-3.9.6/cambridge/cache.py`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.5/cambridge/color.py` & `cambridge-3.9.6/cambridge/color.py`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.5/cambridge/console.py` & `cambridge-3.9.6/cambridge/console.py`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.5/cambridge/dicts/cambridge.py` & `cambridge-3.9.6/cambridge/dicts/cambridge.py`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.5/cambridge/dicts/dict.py` & `cambridge-3.9.6/cambridge/dicts/dict.py`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.5/cambridge/dicts/webster.py` & `cambridge-3.9.6/cambridge/dicts/webster.py`

 * *Files 2% similar despite different names*

```diff
@@ -386,18 +386,19 @@
     phrases = [] # li tags, each tag has one phrase
     for i in pr_sec.iterdescendants():
         if i.tag == "li":
             phrases.append(i)
 
     for phrase in phrases:
         ts = list(phrase.itertext())
+        ts = "". join(ts).strip("\n").strip()
         if phrase != phrases[-1]:
-            c_print(f"[{w_col.rph_item}]{ts[1]},", end=" ")
+            c_print(f"[{w_col.rph_item}]{ts},", end=" ")
         else:
-            c_print(f"[{w_col.rph_item}]{ts[1]}", end="")
+            c_print(f"[{w_col.rph_item}]{ts}", end="")
 
 
 ###########################################
 # parse and print dictionary-entry-[number]
 ###########################################
 
 # --- parse class "vg" --- #
@@ -643,45 +644,54 @@
     if attr == "sense  no-subnum":
         sense_content = children[0] # class "sense-content w-100"
 
     # meaning with "1" + "a"
     elif attr == "sense has-sn has-num":
         sn = children[0].getchildren()[0].text
 
-        if "has-subnum" in ancestor_attr and "sb-0" not in parent_attr:
+        node_prev = node.getprevious()
+        if "has-subnum" in ancestor_attr and node_prev is None and "sb-0" in parent_attr:
+            c_print(f"[bold {w_col.meaning_letter}]{sn}", end = " ")
+        elif "has-subnum" in ancestor_attr and (node_prev is not None or parent_attr != "pseq no-subnum"):
             if num_label_count == 2:
                 print(" ", end="")
             c_print(f"  [bold {w_col.meaning_letter}]{sn}", end = " ")
         else:
             c_print(f"[bold {w_col.meaning_letter}]{sn}", end = " ")
 
         sense_content = children[1] # class "sense-content w-100"
 
     # meaing with only "b" or "1" + "a" + "(1)", or "1" + "a"
     elif attr == "sense has-sn" or attr == "sen has-sn":
-        if num_label_count == 2:
-            print(" ", end="")
-
         sn = children[0].getchildren()[0].text
 
         if "has-subnum" in ancestor_attr and "sb-0" in parent_attr:
             c_print(f"[bold {w_col.meaning_letter}]{sn}", end = " ")
-        elif "letter-only" in ancestor_attr:
-            c_print(f"[bold {w_col.meaning_letter}]{sn}", end = " ")
         else:
-            c_print(f"  [bold {w_col.meaning_letter}]{sn}", end = " ")
+            if num_label_count == 2:
+                    print(" ", end="")
+
+            if "letter-only" in ancestor_attr:
+                if "sb-0" not in parent_attr:
+                    print("  ", end="")
+                c_print(f"[bold {w_col.meaning_letter}]{sn}", end = " ")
+            else:
+                c_print(f"  [bold {w_col.meaning_letter}]{sn}", end = " ")
 
         sense_content = children[1] # class "sense-content w-100"
 
     # meaning with only (2)
     elif attr == "sense has-num-only has-subnum-only":
         if num_label_count == 2:
             print(" ", end="")
         if "letter-only" in ancestor_attr:
-            print("  ", end="")
+            if children[0].attrib["class"] == "sn":
+                print("    ", end = "")
+            else:
+                print("  ", end="")
         else:
             print("    ", end = "")
         sense_content = children[1] # class "sense-content w-100"
 
     # meaning with only number
     elif attr == "sense has-sn has-num-only":
         sense_content = children[1] # class "sense-content w-100"
@@ -743,15 +753,15 @@
     attr = node.attrib["class"]         # "sb-0 sb-entry"
     child_attr = child.attrib["class"]  # "sense has-sn" or "pseq no-subnum"
     if "pseq" in child_attr:
         elms = child.getchildren()[0].getchildren()
         for e in elms:
             e_attr = e.attrib["class"]  # "sense has-sn"
             sense(e, e_attr, attr, parent_attr, num_label_count)     # e.g. sense(child, "sense has-sn", "sb-0 sb-entry", "....", 1)
-    else:
+    elif "sense" in child_attr and child.tag != "span":
         sense(child, child_attr, attr, parent_attr, num_label_count) # e.g. sense(child, "sense has-sn", "sb-0 sb-entry, "sb has-num has-let ms-lg-4 ms-3 w-100", 1)
 
 
 def vg_sseq_entry_item(node):
     """Print one meaning of one entry(noun entry, adjective entry, or verb entry and so forth). e.g. 1: the monetary worth of something."""
 
     num_label_count = 0
@@ -764,35 +774,28 @@
             num_label_count = len(child.text)
 
         # print meaning content
         if "ms-lg-4 ms-3 w-100" in attr:
             for c in child.iterchildren():
                 cc = c.getchildren()
                 if cc[0].get("class") == "sen has-num-only":
-                    cc_0 = cc[0][0]
-                    cc_1 = cc[0][1]
-                    if cc_0.tag != "span":
-                        for i in cc_0.iterchildren():
-                            i_attr = i.get("class")
-                            if i_attr is not None:
-                                if ("badge mw-badge" in i_attr) or ("il" in i_attr):
-                                    print_meaning_badge(i.text.strip())
-                                if "if" in i_attr:
-                                    print_class_if(i.text)
-                                if i_attr == "et":
-                                    et(i)
-                        print()
-                    elif cc_0.tag == "span" and cc_1.tag == "span" and cc_1.attrib["class"] == "sgram":
-                        print_class_sgram(cc_1)
-                        print()
-                    elif cc_0.tag == "span" and cc_1.tag == "span" and "sl badge mw-badge" in cc_1.attrib["class"]:
-                        print_meaning_badge(cc_1.text, end="\n")
-                    elif cc_0.tag == "span" and cc_1.tag == "span" and cc_1.attrib["class"] == "et":
-                        et(cc_1)
-                    continue
+                    for i in cc[0].iterchildren():
+                        i_attr = i.get("class")
+                        if i_attr is not None:
+                            if ("badge mw-badge" in i_attr) or ("il" in i_attr):
+                                print_meaning_badge(i.text.strip())
+                                if "sl " in i_attr:
+                                    print()
+                            if "if" in i_attr:
+                                print_class_if(i.text)
+                            if i_attr == "et":
+                                et(i)
+                            if i_attr == "sgram":
+                                print_class_sgram(i)
+                            continue
 
                 # print class "sb-0 sb-entry", "sb-1 sb-entry" ...
                 sb_entry(c, attr, num_label_count)
 
 def et(node):
     for t in node.itertext():
         print(t.strip("\n"), end= "")
@@ -1059,15 +1062,15 @@
     else:
         c_print(f"[{w_col.meaning_content}]{text}", end=end)
 
 
 def format_basedon_ancestor(ancestor_attr, prefix="", suffix="", root_attr=""):
     print(prefix, end="")
     if ancestor_attr == "sense has-sn has-num-only":
-        print("  ", end=suffix)
+        print("   ", end=suffix)
     if ancestor_attr == "sense has-sn has-num":
         print("    ", end=suffix)
     if ancestor_attr == "sense has-sn":
         if "no-sn letter-only" in root_attr:
             print("  ", end=suffix)
         else:
             print("    ", end=suffix)
```

### Comparing `cambridge-3.9.5/cambridge/errors.py` & `cambridge-3.9.6/cambridge/errors.py`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.5/cambridge/log.py` & `cambridge-3.9.6/cambridge/log.py`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.5/cambridge/main.py` & `cambridge-3.9.6/cambridge/main.py`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.5/cambridge/utils.py` & `cambridge-3.9.6/cambridge/utils.py`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.5/pyproject.toml` & `cambridge-3.9.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.5/screenshots/cambridge.png` & `cambridge-3.9.6/screenshots/cambridge.png`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.5/screenshots/fzf.png` & `cambridge-3.9.6/screenshots/fzf.png`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.5/screenshots/webster.png` & `cambridge-3.9.6/screenshots/webster.png`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.5/PKG-INFO` & `cambridge-3.9.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cambridge
-Version: 3.9.5
+Version: 3.9.6
 Summary: cambridge is a terminal version of Cambridge Dictionary.
 Home-page: https://github.com/KateWang2016/cambridge
 Keywords: dictionary, cambridge, webster, English, web scraping, python
 Author: Kate Wang
 Author-email: kate.wang2018@gmail.com
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

