# Comparing `tmp/linkedit-1.0.1.tar.gz` & `tmp/linkedit-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkedit-1.0.1.tar", last modified: Sun May 19 17:41:05 2024, max compression
+gzip compressed data, was "linkedit-1.0.2.tar", last modified: Sun May 19 22:13:04 2024, max compression
```

## Comparing `linkedit-1.0.1.tar` & `linkedit-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-19 17:41:05.679989 linkedit-1.0.1/
--rw-r--r--   0 khiat     (1000) khiat     (1000)    74013 2024-05-19 17:41:05.679989 linkedit-1.0.1/PKG-INFO
--rw-rw-r--   0 khiat     (1000) khiat     (1000)    73559 2024-05-19 15:00:32.000000 linkedit-1.0.1/README.md
-drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-19 17:41:05.679989 linkedit-1.0.1/linkedit/
--rw-rw-r--   0 khiat     (1000) khiat     (1000)      280 2024-05-19 17:39:14.000000 linkedit-1.0.1/linkedit/__init__.py
--rw-r--r--   0 khiat     (1000) khiat     (1000)   100701 2024-05-19 17:39:05.000000 linkedit-1.0.1/linkedit/linkedit.py
-drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-19 17:41:05.679989 linkedit-1.0.1/linkedit.egg-info/
--rw-r--r--   0 khiat     (1000) khiat     (1000)    74013 2024-05-19 17:41:05.000000 linkedit-1.0.1/linkedit.egg-info/PKG-INFO
--rw-r--r--   0 khiat     (1000) khiat     (1000)      219 2024-05-19 17:41:05.000000 linkedit-1.0.1/linkedit.egg-info/SOURCES.txt
--rw-r--r--   0 khiat     (1000) khiat     (1000)        1 2024-05-19 17:41:05.000000 linkedit-1.0.1/linkedit.egg-info/dependency_links.txt
--rw-r--r--   0 khiat     (1000) khiat     (1000)       16 2024-05-19 17:41:05.000000 linkedit-1.0.1/linkedit.egg-info/requires.txt
--rw-r--r--   0 khiat     (1000) khiat     (1000)        9 2024-05-19 17:41:05.000000 linkedit-1.0.1/linkedit.egg-info/top_level.txt
--rw-r--r--   0 khiat     (1000) khiat     (1000)       38 2024-05-19 17:41:05.679989 linkedit-1.0.1/setup.cfg
--rw-rw-r--   0 khiat     (1000) khiat     (1000)      721 2024-05-19 17:40:01.000000 linkedit-1.0.1/setup.py
+drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-19 22:13:04.287960 linkedit-1.0.2/
+-rw-r--r--   0 khiat     (1000) khiat     (1000)    74013 2024-05-19 22:13:04.287960 linkedit-1.0.2/PKG-INFO
+-rw-rw-r--   0 khiat     (1000) khiat     (1000)    73559 2024-05-19 15:00:32.000000 linkedit-1.0.2/README.md
+drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-19 22:13:04.287960 linkedit-1.0.2/linkedit/
+-rw-rw-r--   0 khiat     (1000) khiat     (1000)      280 2024-05-19 17:39:14.000000 linkedit-1.0.2/linkedit/__init__.py
+-rw-r--r--   0 khiat     (1000) khiat     (1000)   100702 2024-05-19 22:10:01.000000 linkedit-1.0.2/linkedit/linkedit.py
+drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-19 22:13:04.287960 linkedit-1.0.2/linkedit.egg-info/
+-rw-r--r--   0 khiat     (1000) khiat     (1000)    74013 2024-05-19 22:13:04.000000 linkedit-1.0.2/linkedit.egg-info/PKG-INFO
+-rw-r--r--   0 khiat     (1000) khiat     (1000)      219 2024-05-19 22:13:04.000000 linkedit-1.0.2/linkedit.egg-info/SOURCES.txt
+-rw-r--r--   0 khiat     (1000) khiat     (1000)        1 2024-05-19 22:13:04.000000 linkedit-1.0.2/linkedit.egg-info/dependency_links.txt
+-rw-r--r--   0 khiat     (1000) khiat     (1000)       16 2024-05-19 22:13:04.000000 linkedit-1.0.2/linkedit.egg-info/requires.txt
+-rw-r--r--   0 khiat     (1000) khiat     (1000)        9 2024-05-19 22:13:04.000000 linkedit-1.0.2/linkedit.egg-info/top_level.txt
+-rw-r--r--   0 khiat     (1000) khiat     (1000)       38 2024-05-19 22:13:04.287960 linkedit-1.0.2/setup.cfg
+-rw-rw-r--   0 khiat     (1000) khiat     (1000)      721 2024-05-19 22:12:46.000000 linkedit-1.0.2/setup.py
```

### Comparing `linkedit-1.0.1/PKG-INFO` & `linkedit-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkedit
-Version: 1.0.1
+Version: 1.0.2
 Summary: Sophisticate Linked List
 Home-page: https://pypi.org/project/linkedit/
 Author: khiat Mohammed Abderrezzak
 Author-email: khiat.abderrezzak@gmail.com
 License: MIT
 Keywords: linked list
 Classifier: Programming Language :: Python :: 3
```

### Comparing `linkedit-1.0.1/README.md` & `linkedit-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `linkedit-1.0.1/linkedit/linkedit.py` & `linkedit-1.0.2/linkedit/linkedit.py`

 * *Files 0% similar despite different names*

```diff
@@ -307,15 +307,15 @@
         """Remove first occurrence of value.
 
         Raises ValueError if the value is not present."""
         node_index: int = self.index(value)
         try:
             self.pop(node_index)
             return
-        except IndexError as e3:
+        except IndexError as e2:
             pass
         if not self.circular:
             error_msg: str = f"{value} not in the non circular singly linked list"
             raise ValueError(error_msg)
         else:
             error_msg: str = f"{value} not in the circular singly linked list"
             raise ValueError(error_msg)
@@ -376,15 +376,15 @@
         if not isinstance(rotate, int):
             raise TypeError("rotate must be an integer")
         helper1: list = []
         helper2: list = []
         head: object | None = self._head
         try:
             rotate: int = rotate % self.len
-        except ZeroDivisionError as e4:
+        except ZeroDivisionError as e3:
             return
         for _ in range(self.len - rotate):
             helper1.append(head.data)
             head: object | None = head.next
         for _ in range(self.len - rotate, self.len):
             helper2.append(head.data)
             head: object | None = head.next
@@ -398,15 +398,15 @@
         if not isinstance(rotate, int):
             raise TypeError("rotate must be an integer")
         helper1: list = []
         helper2: list = []
         head: object | None = self._head
         try:
             rotate: int = rotate % self.len
-        except ZeroDivisionError as e5:
+        except ZeroDivisionError as e4:
             return
         for _ in range(rotate):
             helper1.append(head.data)
             head: object | None = head.next
         for _ in range(rotate, self.len):
             helper2.append(head.data)
             head: object | None = head.next
@@ -443,15 +443,15 @@
 class singlyLinkedList(linkedList):
     @property
     def head(
         self: "singlyLinkedList",
     ) -> int | float | complex | str | list | tuple | set | dict | None:
         try:
             return self._head
-        except AttributeError as e6:
+        except AttributeError as e5:
             pass
         if not self.circular:
             raise TypeError("Empty non circular singly linked list")
         else:
             raise TypeError("Empty circular singly linked list")
 
     @head.setter
@@ -479,15 +479,15 @@
                 new_node.next = self._head
             self._tail: object = new_node
         else:
             try:
                 if len(data) > 0:
                     for i in data:
                         self.append(i)
-            except TypeError as e7:
+            except TypeError as e6:
                 if data is not None:
                     new_node: object = singlyLinkedListNode(data)
                     self.len += 1
                     self._head: object = new_node
                     if self.circular:
                         new_node.next = new_node
                     self._tail: object = new_node
@@ -707,15 +707,15 @@
                                     else (
                                         blue(f'"{head.next.data}"')
                                         if len(head.next.data) > 1
                                         else f"{head.next.data}"
                                     )
                                 )
                             )
-                        except AttributeError as e8:
+                        except AttributeError as e7:
                             after: str = (
                                 f"{blue('None')} {green('(')}{red('NULL')}{green(')')}"
                             )
                         linked_list.append(
                             [
                                 (
                                     blue(f"{head.data}")
@@ -1026,15 +1026,15 @@
                 new_list: list = new_list[index.start : index.stop : index.step]
                 return singlyLinkedList(
                     new_list,
                     detail=self.detail,
                     circular=self.circular,
                     base=self._base,
                 )
-            except TypeError as e9:
+            except TypeError as e8:
                 pass
             raise TypeError(
                 "slice indices must be integers or None or have an __index__ method"
             )
 
     def to_doubly(self: "singlyLinkedList") -> object:
         return doublyLinkedList() + self
@@ -1098,15 +1098,15 @@
         head: object | None = self._head
         new_dict: dict = {}
         for _ in range(self.len):
             try:
                 next_value: (
                     int | float | complex | str | list | tuple | set | dict | None
                 ) = head.next.data
-            except AttributeError as e2:
+            except AttributeError as e9:
                 next_value: None = None
             new_dict[head.data] = {
                 "current value @ddress" if not node else "current node": (
                     (
                         (
                             bin(id(head))
                             if self._base == 2
@@ -1917,15 +1917,15 @@
         head: object | None = self._head
         new_dict: dict = {}
         for _ in range(self.len):
             try:
                 next_value: (
                     int | float | complex | str | list | tuple | set | dict | None
                 ) = head.next.data
-            except AttributeError as e2:
+            except AttributeError as e16:
                 next_value: None = None
             new_dict[head.data] = {
                 "prev value" if not node else "prev node value": (
                     (head.prev.data if head.prev is not None else None)
                     if not node
                     else head.prev.data if head.prev is not None else None
                 ),
@@ -2068,65 +2068,65 @@
     @head.setter
     def head(self: "orthogonalLinkedList", data: list) -> None:
         if isinstance(data, list):
             som = 0
             for i in range(len(data)):
                 try:
                     som += len(data[i])
-                except TypeError as e16:
+                except TypeError as e17:
                     raise TypeError("just 2D array(list) allowed") from None
             if som % len(data):
                 raise TypeError("2D array(list) columns is not with the same length")
             else:
                 data[0][0] = orthogonalLinkedListNode(data[0][0])
                 for i in range(len(data)):
                     for j in range(len(data[i])):
                         if i == 0:
                             try:
                                 data[i][j + 1] = orthogonalLinkedListNode(
                                     data[i][j + 1]
                                 )
-                            except IndexError as e17:
+                            except IndexError as e18:
                                 pass
                         try:
                             data[i + 1][j] = orthogonalLinkedListNode(data[i + 1][j])
-                        except IndexError as e18:
+                        except IndexError as e19:
                             pass
                         if i == 0:
                             if j == 0:
                                 try:
                                     data[i][j].next = data[i][j + 1]
-                                except IndexError as e19:
+                                except IndexError as e20:
                                     pass
                             elif j == len(data[i]) - 1:
                                 data[i][j].prev = data[i][j - 1]
                             else:
                                 data[i][j].prev = data[i][j - 1]
                                 data[i][j].next = data[i][j + 1]
                             try:
                                 data[i][j].down = data[i + 1][j]
-                            except IndexError as e20:
+                            except IndexError as e21:
                                 pass
                         elif i == len(data) - 1:
                             if j == 0:
                                 try:
                                     data[i][j].next = data[i][j + 1]
-                                except IndexError as e21:
+                                except IndexError as e22:
                                     pass
                             elif j == len(data[i]) - 1:
                                 data[i][j].prev = data[i][j - 1]
                             else:
                                 data[i][j].prev = data[i][j - 1]
                                 data[i][j].next = data[i][j + 1]
                             data[i][j].up = data[i - 1][j]
                         else:
                             if j == 0:
                                 try:
                                     data[i][j].next = data[i][j + 1]
-                                except IndexError as e22:
+                                except IndexError as e23:
                                     pass
                             elif j == len(data[i]) - 1:
                                 data[i][j].prev = data[i][j - 1]
                             else:
                                 data[i][j].prev = data[i][j - 1]
                                 data[i][j].next = data[i][j + 1]
                             data[i][j].up = data[i - 1][j]
@@ -2197,51 +2197,51 @@
                         else:
                             if len(self._head[i][j].prev.data) == 0:
                                 prev_data = self._head[i][j].prev.data
                             elif len(self._head[i][j].prev.data) == 1:
                                 prev_data = blue(f"'{self._head[i][j].prev.data}'")
                             else:
                                 prev_data = blue(f'"{self._head[i][j].prev.data}"')
-                    except AttributeError as e23:
+                    except AttributeError as e24:
                         prev_data = blue("None")
                     try:
                         if not isinstance(self._head[i][j].next.data, str):
                             next_data = blue(f"{self._head[i][j].next.data}")
                         else:
                             if len(self._head[i][j].next.data) == 0:
                                 next_data = self._head[i][j].next.data
                             elif len(self._head[i][j].next.data) == 1:
                                 next_data = blue(f"'{self._head[i][j].next.data}'")
                             else:
                                 next_data = blue(f'"{self._head[i][j].next.data}"')
-                    except AttributeError as e24:
+                    except AttributeError as e25:
                         next_data = blue("None")
                     try:
                         if not isinstance(self._head[i][j].up.data, str):
                             up_data = blue(f"{self._head[i][j].up.data}")
                         else:
                             if len(self._head[i][j].up.data) == 0:
                                 up_data = self._head[i][j].up.data
                             elif len(self._head[i][j].up.data) == 1:
                                 up_data = blue(f"'{self._head[i][j].up.data}'")
                             else:
                                 up_data = blue(f'"{self._head[i][j].up.data}"')
-                    except AttributeError as e25:
+                    except AttributeError as e26:
                         up_data = blue("None")
                     try:
                         if not isinstance(self._head[i][j].down.data, str):
                             down_data = blue(f"{self._head[i][j].down.data}")
                         else:
                             if len(self._head[i][j].down.data) == 0:
                                 down_data = self._head[i][j].down.data
                             elif len(self._head[i][j].down.data) == 1:
                                 down_data = blue(f"'{self._head[i][j].down.data}'")
                             else:
                                 down_data = blue(f'"{self._head[i][j].down.data}"')
-                    except AttributeError as e26:
+                    except AttributeError as e27:
                         down_data = blue("None")
                     current_data = (
                         blue(f"{self._head[i][j].data}")
                         if not isinstance(self._head[i][j].data, str)
                         else (
                             self._head[i][j].data
                             if len(self._head[i][j].data) == 0
```

### Comparing `linkedit-1.0.1/linkedit.egg-info/PKG-INFO` & `linkedit-1.0.2/linkedit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkedit
-Version: 1.0.1
+Version: 1.0.2
 Summary: Sophisticate Linked List
 Home-page: https://pypi.org/project/linkedit/
 Author: khiat Mohammed Abderrezzak
 Author-email: khiat.abderrezzak@gmail.com
 License: MIT
 Keywords: linked list
 Classifier: Programming Language :: Python :: 3
```

### Comparing `linkedit-1.0.1/setup.py` & `linkedit-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="linkedit",
-    version="1.0.1",
+    version="1.0.2",
     author="khiat Mohammed Abderrezzak",
     author_email="khiat.abderrezzak@gmail.com",
     license="MIT",
     description="Sophisticate Linked List",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://pypi.org/project/linkedit/",
```

