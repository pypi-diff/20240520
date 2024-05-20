# Comparing `tmp/imas_tools-0.4.0.tar.gz` & `tmp/imas_tools-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imas_tools-0.4.0.tar", max compression
+gzip compressed data, was "imas_tools-0.4.1.tar", max compression
```

## Comparing `imas_tools-0.4.0.tar` & `imas_tools-0.4.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2024-04-13 09:02:36.035606 imas_tools-0.4.0/imas_tools/__init__.py
--rw-r--r--   0        0        0        0 2024-04-15 13:36:34.820658 imas_tools-0.4.0/imas_tools/portal/__init__.py
--rw-r--r--   0        0        0     4772 2024-04-19 15:23:32.617350 imas_tools-0.4.0/imas_tools/portal/article.py
--rw-r--r--   0        0        0     2363 2024-04-18 15:56:10.247192 imas_tools-0.4.0/imas_tools/portal/interfaces.py
--rw-r--r--   0        0        0     4126 2024-04-13 12:27:59.670781 imas_tools-0.4.0/imas_tools/recochoku.py
--rw-r--r--   0        0        0        0 2024-05-20 16:09:08.603881 imas_tools-0.4.0/imas_tools/story/__init__.py
--rw-r--r--   0        0        0      579 2024-05-20 16:09:28.637319 imas_tools-0.4.0/imas_tools/story/adapter.py
--rw-r--r--   0        0        0     3061 2024-05-20 16:08:35.466738 imas_tools-0.4.0/imas_tools/story/gakuen_parser.py
--rw-r--r--   0        0        0      465 2024-05-20 16:17:21.451486 imas_tools-0.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-13 09:02:36.044152 imas_tools-0.4.0/README.md
--rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 imas_tools-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-13 09:02:36.035606 imas_tools-0.4.1/imas_tools/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 13:36:34.820658 imas_tools-0.4.1/imas_tools/portal/__init__.py
+-rw-r--r--   0        0        0     4772 2024-04-19 15:23:32.617350 imas_tools-0.4.1/imas_tools/portal/article.py
+-rw-r--r--   0        0        0     2363 2024-04-18 15:56:10.247192 imas_tools-0.4.1/imas_tools/portal/interfaces.py
+-rw-r--r--   0        0        0     4126 2024-04-13 12:27:59.670781 imas_tools-0.4.1/imas_tools/recochoku.py
+-rw-r--r--   0        0        0        0 2024-05-20 16:09:08.603881 imas_tools-0.4.1/imas_tools/story/__init__.py
+-rw-r--r--   0        0        0      591 2024-05-20 16:52:00.011700 imas_tools-0.4.1/imas_tools/story/adapter.py
+-rw-r--r--   0        0        0     3071 2024-05-20 16:54:11.355982 imas_tools-0.4.1/imas_tools/story/gakuen_parser.py
+-rw-r--r--   0        0        0      465 2024-05-20 16:54:46.498490 imas_tools-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-13 09:02:36.044152 imas_tools-0.4.1/README.md
+-rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 imas_tools-0.4.1/PKG-INFO
```

### Comparing `imas_tools-0.4.0/imas_tools/portal/article.py` & `imas_tools-0.4.1/imas_tools/portal/article.py`

 * *Files identical despite different names*

### Comparing `imas_tools-0.4.0/imas_tools/portal/interfaces.py` & `imas_tools-0.4.1/imas_tools/portal/interfaces.py`

 * *Files identical despite different names*

### Comparing `imas_tools-0.4.0/imas_tools/recochoku.py` & `imas_tools-0.4.1/imas_tools/recochoku.py`

 * *Files identical despite different names*

### Comparing `imas_tools-0.4.0/imas_tools/story/adapter.py` & `imas_tools-0.4.1/imas_tools/story/adapter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from .gakuen_parser import parse_messages
 
 
-def gakuen_txt_to_sc_csv(gakuen_txt: str, txt_name: str) -> str:
-    parsed = parse_messages(gakuen_txt.split("\n"))
+def gakuen_txt_to_sc_csv(gakuen_txt: str, txt_name_without_ext: str) -> str:
+    parsed = parse_messages(gakuen_txt)
     sc_csv = "id,name,text,trans\n"
     for line in parsed:
         if line["__tag__"] == "message":
             sc_csv += f"0000000000000,{line['name']},{line['text']},\n"
         if line["__tag__"] == "choicegroup":
             for choice in line["choices"]:
                 sc_csv += f"select,,{choice['text']},\n"
-    sc_csv += f"info,${txt_name}.txt,,"
+    sc_csv += f"info,${txt_name_without_ext}.txt,,"
     sc_csv += f"译者,,,"
     return sc_csv
```

### Comparing `imas_tools-0.4.0/imas_tools/story/gakuen_parser.py` & `imas_tools-0.4.1/imas_tools/story/gakuen_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,22 +68,22 @@
             obj[key] = [obj[key], value]
     if message[i] != "]":
         raise ValueError()
     i = i + 1
     return i, obj
 
 
-def parse_message(message):
+def parse_message(message: str):
     i, o = parse_object(message, 0)
     if i != len(message):
         raise ValueError()
     return o
 
 
-def parse_messages(messages) -> list:
+def parse_messages(messages: str) -> list:
     return [
         parse_message(message) for message in messages.split("\n") if message.strip()
     ]
 
 
 def encode_json(obj):
     return (
```

### Comparing `imas_tools-0.4.0/PKG-INFO` & `imas_tools-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imas-tools
-Version: 0.4.0
+Version: 0.4.1
 Summary: 
 Author: darwintree
 Author-email: 17946284+darwintree@users.noreply.github.com
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

