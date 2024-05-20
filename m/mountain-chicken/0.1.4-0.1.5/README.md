# Comparing `tmp/mountain_chicken-0.1.4.tar.gz` & `tmp/mountain_chicken-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mountain_chicken-0.1.4.tar", last modified: Mon May 20 08:46:37 2024, max compression
+gzip compressed data, was "mountain_chicken-0.1.5.tar", last modified: Mon May 20 08:54:53 2024, max compression
```

## Comparing `mountain_chicken-0.1.4.tar` & `mountain_chicken-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 08:46:37.270873 mountain_chicken-0.1.4/
--rw-rw-rw-   0        0        0       63 2024-05-20 08:46:37.270373 mountain_chicken-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       29 2024-05-13 15:05:37.000000 mountain_chicken-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 08:46:37.259372 mountain_chicken-0.1.4/mountain_chicken/
--rw-rw-rw-   0        0        0      104 2024-05-19 20:07:34.000000 mountain_chicken-0.1.4/mountain_chicken/__init__.py
--rw-rw-rw-   0        0        0     2580 2024-05-18 17:21:49.000000 mountain_chicken-0.1.4/mountain_chicken/base.py
--rw-rw-rw-   0        0        0      954 2024-05-13 19:08:16.000000 mountain_chicken-0.1.4/mountain_chicken/double_dict.py
--rw-rw-rw-   0        0        0      658 2024-05-16 12:49:31.000000 mountain_chicken-0.1.4/mountain_chicken/mutable_string.py
-drwxrwxrwx   0        0        0        0 2024-05-20 08:46:37.269874 mountain_chicken-0.1.4/mountain_chicken.egg-info/
--rw-rw-rw-   0        0        0       63 2024-05-20 08:46:37.000000 mountain_chicken-0.1.4/mountain_chicken.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2024-05-20 08:46:37.000000 mountain_chicken-0.1.4/mountain_chicken.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 08:46:37.000000 mountain_chicken-0.1.4/mountain_chicken.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-20 08:46:37.000000 mountain_chicken-0.1.4/mountain_chicken.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 08:46:37.270873 mountain_chicken-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      202 2024-05-20 08:46:16.000000 mountain_chicken-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 08:54:53.387762 mountain_chicken-0.1.5/
+-rw-rw-rw-   0        0        0       63 2024-05-20 08:54:53.387262 mountain_chicken-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       29 2024-05-13 15:05:37.000000 mountain_chicken-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 08:54:53.380133 mountain_chicken-0.1.5/mountain_chicken/
+-rw-rw-rw-   0        0        0      102 2024-05-20 08:54:12.000000 mountain_chicken-0.1.5/mountain_chicken/__init__.py
+-rw-rw-rw-   0        0        0     2542 2024-05-20 08:53:23.000000 mountain_chicken-0.1.5/mountain_chicken/base.py
+-rw-rw-rw-   0        0        0      953 2024-05-20 08:52:38.000000 mountain_chicken-0.1.5/mountain_chicken/double_dict.py
+-rw-rw-rw-   0        0        0      656 2024-05-20 08:53:35.000000 mountain_chicken-0.1.5/mountain_chicken/mutable_string.py
+drwxrwxrwx   0        0        0        0 2024-05-20 08:54:53.386763 mountain_chicken-0.1.5/mountain_chicken.egg-info/
+-rw-rw-rw-   0        0        0       63 2024-05-20 08:54:53.000000 mountain_chicken-0.1.5/mountain_chicken.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2024-05-20 08:54:53.000000 mountain_chicken-0.1.5/mountain_chicken.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 08:54:53.000000 mountain_chicken-0.1.5/mountain_chicken.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-20 08:54:53.000000 mountain_chicken-0.1.5/mountain_chicken.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 08:54:53.388261 mountain_chicken-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      202 2024-05-20 08:54:20.000000 mountain_chicken-0.1.5/setup.py
```

### Comparing `mountain_chicken-0.1.4/mountain_chicken/base.py` & `mountain_chicken-0.1.5/mountain_chicken/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from double_dict import double_dict
 from typing import Any, Self, List
 
-class base:
+class Base:
     def __init__(self, base: int, number: str = "") -> None:
         self.number: str = number.lstrip("0")
         self.base: int = base
         self.letters: str = "0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZ"[:self.base]
         
         #check characters are valid
         if not all(l in self.letters for l in self.number): 
@@ -40,15 +40,15 @@
             
             else:
                 remainder = 0
                 res.append(self.d[cur])
         
         if remainder: res.append(str(remainder))
         
-        return base(self.base, "".join(res[::-1]))
+        return Base(self.base, "".join(res[::-1]))
 
     def __radd__(self, other):
         
         if other == 0:
             return self
         
         return self.__add__(other)
@@ -75,18 +75,18 @@
                 
                 while cur:
                     temp.append(str(cur%self.base))
                     cur = cur//self.base
                 
                 temp = temp[::-1]
                 
-                res.append(base(self.base, "".join(temp) + (i+j)*"0"))
+                res.append(Base(self.base, "".join(temp) + (i+j)*"0"))
         
         return sum(res)
 
 
 
 
-print(base(10,"123") * base(10,"456"))
+
```

### Comparing `mountain_chicken-0.1.4/mountain_chicken/double_dict.py` & `mountain_chicken-0.1.5/mountain_chicken/double_dict.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any
 
 
-class double_dict:
+class DoubleDict:
     def __init__(self, d: dict, **kwargs) -> None:
         self._d = d
         self._rev_d = {key : value for value,key in self._d.items()}
         if "default" in kwargs:
             self.default = kwargs["default"]
         else:
             self.default = False
```

### Comparing `mountain_chicken-0.1.4/mountain_chicken/mutable_string.py` & `mountain_chicken-0.1.5/mountain_chicken/mutable_string.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import List
 
-class mutable_string:
+class MutableString:
     def __init__(self, word: str = "") -> None:
         self.word = word
         self.length = len(word)
 
     def __len__(self) -> int:
         return self.length
     
     def __add__(word1, word2) -> str:
-        return mutable_string(word1.word + word2.word)
+        return MutableString(word1.word + word2.word)
     
     def __getitem__(self, index: int) -> str:
         return self.word[index]
     
     def __setitem__(self, index: int, characters: str) -> None:
         self.array = [*self.word]
         self.array[index] = characters
```

