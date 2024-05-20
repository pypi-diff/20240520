# Comparing `tmp/TsingPig_Lab-0.1.6.tar.gz` & `tmp/TsingPig_Lab-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\TsingPig_Lab-0.1.6.tar", last modified: Fri May 17 15:09:42 2024, max compression
+gzip compressed data, was "dist\TsingPig_Lab-0.1.7.tar", last modified: Mon May 20 12:53:10 2024, max compression
```

## Comparing `TsingPig_Lab-0.1.6.tar` & `TsingPig_Lab-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 15:09:42.760136 TsingPig_Lab-0.1.6/
--rw-rw-rw-   0        0        0     6924 2024-05-17 15:09:42.758658 TsingPig_Lab-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     5183 2024-05-17 15:09:32.000000 TsingPig_Lab-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 15:09:42.752412 TsingPig_Lab-0.1.6/TsingPig_Lab.egg-info/
--rw-rw-rw-   0        0        0     6924 2024-05-17 15:09:42.000000 TsingPig_Lab-0.1.6/TsingPig_Lab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2024-05-17 15:09:42.000000 TsingPig_Lab-0.1.6/TsingPig_Lab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 15:09:42.000000 TsingPig_Lab-0.1.6/TsingPig_Lab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-17 15:09:42.000000 TsingPig_Lab-0.1.6/TsingPig_Lab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-17 15:09:42.760136 TsingPig_Lab-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      941 2024-05-16 06:31:47.000000 TsingPig_Lab-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-17 15:09:42.758155 TsingPig_Lab-0.1.6/tsingpig_lab/
--rw-rw-rw-   0        0        0     3264 2024-05-17 15:07:22.000000 TsingPig_Lab-0.1.6/tsingpig_lab/Algorithms.py
--rw-rw-rw-   0        0        0     1322 2024-05-16 07:56:09.000000 TsingPig_Lab-0.1.6/tsingpig_lab/DataStructures.py
--rw-rw-rw-   0        0        0      260 2024-05-17 15:09:18.000000 TsingPig_Lab-0.1.6/tsingpig_lab/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 12:53:10.697860 TsingPig_Lab-0.1.7/
+-rw-rw-rw-   0        0        0    10628 2024-05-20 12:53:10.697860 TsingPig_Lab-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     8269 2024-05-20 12:52:56.000000 TsingPig_Lab-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 12:53:10.691928 TsingPig_Lab-0.1.7/TsingPig_Lab.egg-info/
+-rw-rw-rw-   0        0        0    10628 2024-05-20 12:53:10.000000 TsingPig_Lab-0.1.7/TsingPig_Lab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2024-05-20 12:53:10.000000 TsingPig_Lab-0.1.7/TsingPig_Lab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 12:53:10.000000 TsingPig_Lab-0.1.7/TsingPig_Lab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-20 12:53:10.000000 TsingPig_Lab-0.1.7/TsingPig_Lab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 12:53:10.698862 TsingPig_Lab-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      941 2024-05-16 06:31:47.000000 TsingPig_Lab-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 12:53:10.695942 TsingPig_Lab-0.1.7/tsingpig_lab/
+-rw-rw-rw-   0        0        0     3264 2024-05-17 15:07:22.000000 TsingPig_Lab-0.1.7/tsingpig_lab/Algorithms.py
+-rw-rw-rw-   0        0        0     8209 2024-05-20 12:48:59.000000 TsingPig_Lab-0.1.7/tsingpig_lab/DataStructures.py
+-rw-rw-rw-   0        0        0      260 2024-05-20 12:51:34.000000 TsingPig_Lab-0.1.7/tsingpig_lab/__init__.py
```

### Comparing `TsingPig_Lab-0.1.6/PKG-INFO` & `TsingPig_Lab-0.1.7/TsingPig_Lab.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 Metadata-Version: 2.1
-Name: TsingPig_Lab
-Version: 0.1.6
+Name: TsingPig-Lab
+Version: 0.1.7
 Summary: TsingPig_Lab is a package for algorithm.
 Home-page: https://gitlab.com/tsingpig-code/tsingpig_lab
 Author: TsingPig
 Author-email: 1114196607@qq.com
 License: UNKNOWN
 Description: # TsingPig - Lab
         
         ![image.png](https://pic.leetcode.cn/1715846857-WsuYYB-image.png)
         
+        [TOC]
+        
         ## 1. Introduction
         This is a python package for simple algorithms and data structures which is developed by **tsingpig**.
         
-        **Version: v0.1.6**
-        
         Author: TsingPig
         
         Repo: https://gitlab.com/tsingpig-code/tsingpig_lab
         
         You can connect me by email: 1114196607@qq.com
         
         Thanks for your support!
         
         
         
-        ## 2. Functions
+        ## 2. Features
         ### 2.1. DataStructures
         
         #### 2.1.1 Sparse Table (ST)
         
         A data structure ST table (Sparse Table) that supports interval contribution problem queries.
         
         **Usage**
         
         | Method                                               | Time Complexity | Description                                                  |
         | ---------------------------------------------------- | --------------- | ------------------------------------------------------------ |
         | `__init__(nums: List, opt = lambda a, b: max(a, b))` | $O(n \log n)$   | Initialize the Sparse Table (ST) data structure with the given list of numbers and an optional comparison function. |
         | `qry(L: int, R: int)`                                | $O(1)$          | Query the opt value within the range [L, R].                 |
         
-        **Simple**
+        **Example **
         
         ``` python
         from tsingpig_lab.DataStructures import ST as ST
         st = ST([1, 9, 0, 2, 4, 5])
         print(st.qry(1, 3))	# 9
         ```
         
@@ -51,32 +51,109 @@
         
         ```python
         from tsingpig_lab.DataStructures import ST as ST
         st = ST([1, 9, -99, 2, 4, 5], lambda a, b: min(a, b))
         print(st.qry(1, 4)) # -99
         ```
         
+        > Please note that the issue of contribution needs to be met. It means $Opt (x, x)=x$
         
         
-        > Please note that the issue of contribution needs to be met. It means $Opt (x, x)=x$
+        
+        #### 2.1.2 Fenwick Tree
+        
+        A data structure Fenwick Tree that supports range queries efficiently.
+        
+        **Usage**
+        
+        | Method                                                       | Time Complexity | Description                                                  |
+        | ------------------------------------------------------------ | --------------- | ------------------------------------------------------------ |
+        | `__init__(n: int, discretize: bool = False, nums: List[int] = None)` | $O(n \log n)$   | Initialize the Fenwick Tree data structure with the given array length `n` and optionally with discretized values. |
+        | `update(x: int, val: int = 1)`                               | $O(\log n)$     | Update the value at index `x` by adding `val`.               |
+        | `query(lx: int, rx: int = None)`                             | $O(\log n)$     | If only `lx` is provided, query the number of elements less than or equal to `lx`. If both `lx` and `rx` are provided, query the number of elements between `lx` and `rx` inclusive. |
+        
+        **Example **
+        
+        Example without discretization
+        
+        ```python
+        from tsingpig_lab.DataStructures import FenwickTree as FenwickTree
+        tr = FenwickTree(10)
+        tr.update(1, 1)
+        tr.update(2, 2)
+        tr.update(3, 5)
+        tr.update(1, 3)
+        # [0, 4, 2, 5, 0, 0, 0, 0, 0, 0]
+        print(tr.query(1, 10))	# 11
+        ```
+        
+        Example with discretization锛宨t allows the input array `nums` has repeated elements.
+        
+        ```python
+        from tsingpig_lab.DataStructures import FenwickTree as FenwickTree
+        nums = [1, 9, -99, 2, 4, 5, -99]
+        ft = FenwickTree(len(nums), discretize=True, nums=nums)
+        ft.update(2, 4)
+        ft.update(-99, 3)
+        # [0, 0, 3, 4, 0, 0]
+        print(ft.query(-99, 9)) # 7
+        ```
+        
+        
+        
+        #### 2.1.3 Segment Tree
+        
+        **Usage**
+        
+        | Method                                    | Time Complexity | Description                                                  |
+        | ----------------------------------------- | --------------- | ------------------------------------------------------------ |
+        | `__init__(nums, ops='sum')`               | $O(n)$          | Initialize the Segment Tree data structure with the given array `nums` and operation type `ops`, defaulting to sum operation. |
+        | `build(idx=1, l=1, r=None)`               | $O(n)$          | Build the Segment Tree.                                      |
+        | `update(ul, ur, val, idx=1, l=1, r=None)` | $O(\log n)$     | Update the range [ul, ur] with the given value `val`.        |
+        | `query(ql, qr, idx=1, l=1, r=None)`       | $O(\log n)$     | Query the result value within the range [ql, qr].            |
+        
+        **Sample**
+        
+        ```python
+        from tsingpig_lab.DataStructures import SegmentTree as SegmentTree
+        
+        tr = SegmentTree([1, 2, 3, 4, 5], 'sum')
+        tr.build()
+        print(tr.query(1, 5))  # 15
+        print(tr.query(2, 5))  # 14
+        tr.update(2, 4, 2)  # 1 4 5 6 5
+        print(tr.query(2, 5))  # 20
+        
+        tr = SegmentTree([8, 4, 5, 7, 9], 'min')
+        tr.build()
+        print(tr.query(1, 4)) # 4
+        tr.update(1, 4, 5) # [5, 4, 5, 5, 9]
+        print(tr.query(4, 5)) # 5
+        tr.update(3, 5, -10) # [5, 4, -10, -10, -10]
+        print(tr.query(1, 3)) # -10
+        ```
+        
+        
+        
+        > Note: The index is start with 1.
         
         ### 2.2. Algorithms
         
         #### 2.2.1 BaseConverter 
         
         Using for convert input number with base-a to result number with base-b.
         
         **Usage**
         
         | Method                     | Time Complexity | Description                                                  |
         | -------------------------- | --------------- | ------------------------------------------------------------ |
         | `__init__(a: int, b: int)` | N/A             | Initialize the BaseConverter with base `a` to convert numbers to base `b`. The bases must be within the range [2, 16]. |
         | `convert(num: str) -> str` | $O(\log n)$     | Convert a number in base `a` (given as a string) to its representation in base `b`. |
         
-        **Simple**
+        **Example **
         
         As shown below, you create a base converter from base-10 to base-2.
         
         ```python
         from tsingpig_lab.Algorithms import BaseConverter
         baseCon = BaseConverter(10, 2)
         print(baseCon.convert("123"))  # 1111011
@@ -88,25 +165,25 @@
         
         ```python
         from tsingpig_lab.Algorithms import BaseConverter
         baseCon = BaseConverter(16, 10)
         print(baseCon.convert("1BF52"))  # 114514
         ```
         
-        ### 2.2.2 Bin
+        #### 2.2.2 Bin
         
         **Usage**
         
         | Method                            | Time Complexity | Description                                                  |
         | --------------------------------- | --------------- | ------------------------------------------------------------ |
         | `__init__(num: str, b: int = 2) ` | N/A             | Initialize the Bin object with a number string `num` in base `b` (default is binary). If `b` is not 2, it converts the number from base `b` to base 2. |
         | `grey_to_bin() -> str `           | $O(n)$          | Converts the stored binary string, treated as a Gray code, to its corresponding binary code. $n$ is the length of the binary representation of $num$ . |
         | `bin_to_grey() -> str`            | $O(n)$          | Converts the stored binary string, treated as a binary code, to its corresponding Gray code. |
         
-        **Simple**
+        **Example **
         
         As shown below, you initialize a binary object base on 2.
         
         ```python
         from tsingpig_lab.Algorithms import Bin
         b = Bin('1111')
         ```
@@ -141,33 +218,33 @@
         # 3. Note for Pypi
         
         **How to upload your own package**
         
         Firstly, open your package folder and type this command in its' corresponding cmd:
         
         ```
-         python setup.py sdist
+        python setup.py sdist
         ```
         
         Then:
         
         ```
         twine upload dist/*
         ```
         
         And then it works, users can download your package by this line in conda:
         
         ```
-        pip install TsingPig-Lab==0.1.5 -i https://www.pypi.org/simple/
+        pip install TsingPig-Lab==0.1.6 -i https://www.pypi.org/simple/
         ```
         
         API
         
         ```
-        pypi-AgEIcHlwaS5vcmcCJDMxZTVjYjEwLTI1ZjgtNDkyYy1hYjk5LTIwODhkMmRhOGU4MQACKlszLCI3NDRkODY1Ni02ODE3LTRiNjEtYTliMi1kZThmOTI0YjQ5ZWEiXQAABiA7fW5wFoRjJYg7bF0l9tnQWja3Lo-ag6U96-XcTmKChw
+        pypi-AgEIcHlwaS5vcmcCJDg0MjZkZGM0LWQ0MjQtNGUyNC04NWI3LTExMTMwYTE4NjU2NQACKlszLCI3NDRkODY1Ni02ODE3LTRiNjEtYTliMi1kZThmOTI0YjQ5ZWEiXQAABiBN54j1SgGHWIqkPfyu1Iq3i5qwGrUB5UGPpeEYpyIf4A
         ```
         
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `TsingPig_Lab-0.1.6/README.md` & `TsingPig_Lab-0.1.7/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 # TsingPig - Lab
 
 ![image.png](https://pic.leetcode.cn/1715846857-WsuYYB-image.png)
 
+[TOC]
+
 ## 1. Introduction
 This is a python package for simple algorithms and data structures which is developed by **tsingpig**.
 
-**Version: v0.1.6**
-
 Author: TsingPig
 
 Repo: https://gitlab.com/tsingpig-code/tsingpig_lab
 
 You can connect me by email: 1114196607@qq.com
 
 Thanks for your support!
 
 
 
-## 2. Functions
+## 2. Features
 ### 2.1. DataStructures
 
 #### 2.1.1 Sparse Table (ST)
 
 A data structure ST table (Sparse Table) that supports interval contribution problem queries.
 
 **Usage**
 
 | Method                                               | Time Complexity | Description                                                  |
 | ---------------------------------------------------- | --------------- | ------------------------------------------------------------ |
 | `__init__(nums: List, opt = lambda a, b: max(a, b))` | $O(n \log n)$   | Initialize the Sparse Table (ST) data structure with the given list of numbers and an optional comparison function. |
 | `qry(L: int, R: int)`                                | $O(1)$          | Query the opt value within the range [L, R].                 |
 
-**Simple**
+**Example **
 
 ``` python
 from tsingpig_lab.DataStructures import ST as ST
 st = ST([1, 9, 0, 2, 4, 5])
 print(st.qry(1, 3))	# 9
 ```
 
@@ -43,32 +43,109 @@
 
 ```python
 from tsingpig_lab.DataStructures import ST as ST
 st = ST([1, 9, -99, 2, 4, 5], lambda a, b: min(a, b))
 print(st.qry(1, 4)) # -99
 ```
 
+> Please note that the issue of contribution needs to be met. It means $Opt (x, x)=x$
 
 
-> Please note that the issue of contribution needs to be met. It means $Opt (x, x)=x$
+
+#### 2.1.2 Fenwick Tree
+
+A data structure Fenwick Tree that supports range queries efficiently.
+
+**Usage**
+
+| Method                                                       | Time Complexity | Description                                                  |
+| ------------------------------------------------------------ | --------------- | ------------------------------------------------------------ |
+| `__init__(n: int, discretize: bool = False, nums: List[int] = None)` | $O(n \log n)$   | Initialize the Fenwick Tree data structure with the given array length `n` and optionally with discretized values. |
+| `update(x: int, val: int = 1)`                               | $O(\log n)$     | Update the value at index `x` by adding `val`.               |
+| `query(lx: int, rx: int = None)`                             | $O(\log n)$     | If only `lx` is provided, query the number of elements less than or equal to `lx`. If both `lx` and `rx` are provided, query the number of elements between `lx` and `rx` inclusive. |
+
+**Example **
+
+Example without discretization
+
+```python
+from tsingpig_lab.DataStructures import FenwickTree as FenwickTree
+tr = FenwickTree(10)
+tr.update(1, 1)
+tr.update(2, 2)
+tr.update(3, 5)
+tr.update(1, 3)
+# [0, 4, 2, 5, 0, 0, 0, 0, 0, 0]
+print(tr.query(1, 10))	# 11
+```
+
+Example with discretization，it allows the input array `nums` has repeated elements.
+
+```python
+from tsingpig_lab.DataStructures import FenwickTree as FenwickTree
+nums = [1, 9, -99, 2, 4, 5, -99]
+ft = FenwickTree(len(nums), discretize=True, nums=nums)
+ft.update(2, 4)
+ft.update(-99, 3)
+# [0, 0, 3, 4, 0, 0]
+print(ft.query(-99, 9)) # 7
+```
+
+
+
+#### 2.1.3 Segment Tree
+
+**Usage**
+
+| Method                                    | Time Complexity | Description                                                  |
+| ----------------------------------------- | --------------- | ------------------------------------------------------------ |
+| `__init__(nums, ops='sum')`               | $O(n)$          | Initialize the Segment Tree data structure with the given array `nums` and operation type `ops`, defaulting to sum operation. |
+| `build(idx=1, l=1, r=None)`               | $O(n)$          | Build the Segment Tree.                                      |
+| `update(ul, ur, val, idx=1, l=1, r=None)` | $O(\log n)$     | Update the range [ul, ur] with the given value `val`.        |
+| `query(ql, qr, idx=1, l=1, r=None)`       | $O(\log n)$     | Query the result value within the range [ql, qr].            |
+
+**Sample**
+
+```python
+from tsingpig_lab.DataStructures import SegmentTree as SegmentTree
+
+tr = SegmentTree([1, 2, 3, 4, 5], 'sum')
+tr.build()
+print(tr.query(1, 5))  # 15
+print(tr.query(2, 5))  # 14
+tr.update(2, 4, 2)  # 1 4 5 6 5
+print(tr.query(2, 5))  # 20
+
+tr = SegmentTree([8, 4, 5, 7, 9], 'min')
+tr.build()
+print(tr.query(1, 4)) # 4
+tr.update(1, 4, 5) # [5, 4, 5, 5, 9]
+print(tr.query(4, 5)) # 5
+tr.update(3, 5, -10) # [5, 4, -10, -10, -10]
+print(tr.query(1, 3)) # -10
+```
+
+
+
+> Note: The index is start with 1.
 
 ### 2.2. Algorithms
 
 #### 2.2.1 BaseConverter 
 
 Using for convert input number with base-a to result number with base-b.
 
 **Usage**
 
 | Method                     | Time Complexity | Description                                                  |
 | -------------------------- | --------------- | ------------------------------------------------------------ |
 | `__init__(a: int, b: int)` | N/A             | Initialize the BaseConverter with base `a` to convert numbers to base `b`. The bases must be within the range [2, 16]. |
 | `convert(num: str) -> str` | $O(\log n)$     | Convert a number in base `a` (given as a string) to its representation in base `b`. |
 
-**Simple**
+**Example **
 
 As shown below, you create a base converter from base-10 to base-2.
 
 ```python
 from tsingpig_lab.Algorithms import BaseConverter
 baseCon = BaseConverter(10, 2)
 print(baseCon.convert("123"))  # 1111011
@@ -80,25 +157,25 @@
 
 ```python
 from tsingpig_lab.Algorithms import BaseConverter
 baseCon = BaseConverter(16, 10)
 print(baseCon.convert("1BF52"))  # 114514
 ```
 
-### 2.2.2 Bin
+#### 2.2.2 Bin
 
 **Usage**
 
 | Method                            | Time Complexity | Description                                                  |
 | --------------------------------- | --------------- | ------------------------------------------------------------ |
 | `__init__(num: str, b: int = 2) ` | N/A             | Initialize the Bin object with a number string `num` in base `b` (default is binary). If `b` is not 2, it converts the number from base `b` to base 2. |
 | `grey_to_bin() -> str `           | $O(n)$          | Converts the stored binary string, treated as a Gray code, to its corresponding binary code. $n$ is the length of the binary representation of $num$ . |
 | `bin_to_grey() -> str`            | $O(n)$          | Converts the stored binary string, treated as a binary code, to its corresponding Gray code. |
 
-**Simple**
+**Example **
 
 As shown below, you initialize a binary object base on 2.
 
 ```python
 from tsingpig_lab.Algorithms import Bin
 b = Bin('1111')
 ```
@@ -133,28 +210,28 @@
 # 3. Note for Pypi
 
 **How to upload your own package**
 
 Firstly, open your package folder and type this command in its' corresponding cmd:
 
 ```
- python setup.py sdist
+python setup.py sdist
 ```
 
 Then:
 
 ```
 twine upload dist/*
 ```
 
 And then it works, users can download your package by this line in conda:
 
 ```
-pip install TsingPig-Lab==0.1.5 -i https://www.pypi.org/simple/
+pip install TsingPig-Lab==0.1.6 -i https://www.pypi.org/simple/
 ```
 
 API
 
 ```
-pypi-AgEIcHlwaS5vcmcCJDMxZTVjYjEwLTI1ZjgtNDkyYy1hYjk5LTIwODhkMmRhOGU4MQACKlszLCI3NDRkODY1Ni02ODE3LTRiNjEtYTliMi1kZThmOTI0YjQ5ZWEiXQAABiA7fW5wFoRjJYg7bF0l9tnQWja3Lo-ag6U96-XcTmKChw
+pypi-AgEIcHlwaS5vcmcCJDg0MjZkZGM0LWQ0MjQtNGUyNC04NWI3LTExMTMwYTE4NjU2NQACKlszLCI3NDRkODY1Ni02ODE3LTRiNjEtYTliMi1kZThmOTI0YjQ5ZWEiXQAABiBN54j1SgGHWIqkPfyu1Iq3i5qwGrUB5UGPpeEYpyIf4A
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `TsingPig_Lab-0.1.6/TsingPig_Lab.egg-info/PKG-INFO` & `TsingPig_Lab-0.1.7/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 Metadata-Version: 2.1
-Name: TsingPig-Lab
-Version: 0.1.6
+Name: TsingPig_Lab
+Version: 0.1.7
 Summary: TsingPig_Lab is a package for algorithm.
 Home-page: https://gitlab.com/tsingpig-code/tsingpig_lab
 Author: TsingPig
 Author-email: 1114196607@qq.com
 License: UNKNOWN
 Description: # TsingPig - Lab
         
         ![image.png](https://pic.leetcode.cn/1715846857-WsuYYB-image.png)
         
+        [TOC]
+        
         ## 1. Introduction
         This is a python package for simple algorithms and data structures which is developed by **tsingpig**.
         
-        **Version: v0.1.6**
-        
         Author: TsingPig
         
         Repo: https://gitlab.com/tsingpig-code/tsingpig_lab
         
         You can connect me by email: 1114196607@qq.com
         
         Thanks for your support!
         
         
         
-        ## 2. Functions
+        ## 2. Features
         ### 2.1. DataStructures
         
         #### 2.1.1 Sparse Table (ST)
         
         A data structure ST table (Sparse Table) that supports interval contribution problem queries.
         
         **Usage**
         
         | Method                                               | Time Complexity | Description                                                  |
         | ---------------------------------------------------- | --------------- | ------------------------------------------------------------ |
         | `__init__(nums: List, opt = lambda a, b: max(a, b))` | $O(n \log n)$   | Initialize the Sparse Table (ST) data structure with the given list of numbers and an optional comparison function. |
         | `qry(L: int, R: int)`                                | $O(1)$          | Query the opt value within the range [L, R].                 |
         
-        **Simple**
+        **Example **
         
         ``` python
         from tsingpig_lab.DataStructures import ST as ST
         st = ST([1, 9, 0, 2, 4, 5])
         print(st.qry(1, 3))	# 9
         ```
         
@@ -51,32 +51,109 @@
         
         ```python
         from tsingpig_lab.DataStructures import ST as ST
         st = ST([1, 9, -99, 2, 4, 5], lambda a, b: min(a, b))
         print(st.qry(1, 4)) # -99
         ```
         
+        > Please note that the issue of contribution needs to be met. It means $Opt (x, x)=x$
         
         
-        > Please note that the issue of contribution needs to be met. It means $Opt (x, x)=x$
+        
+        #### 2.1.2 Fenwick Tree
+        
+        A data structure Fenwick Tree that supports range queries efficiently.
+        
+        **Usage**
+        
+        | Method                                                       | Time Complexity | Description                                                  |
+        | ------------------------------------------------------------ | --------------- | ------------------------------------------------------------ |
+        | `__init__(n: int, discretize: bool = False, nums: List[int] = None)` | $O(n \log n)$   | Initialize the Fenwick Tree data structure with the given array length `n` and optionally with discretized values. |
+        | `update(x: int, val: int = 1)`                               | $O(\log n)$     | Update the value at index `x` by adding `val`.               |
+        | `query(lx: int, rx: int = None)`                             | $O(\log n)$     | If only `lx` is provided, query the number of elements less than or equal to `lx`. If both `lx` and `rx` are provided, query the number of elements between `lx` and `rx` inclusive. |
+        
+        **Example **
+        
+        Example without discretization
+        
+        ```python
+        from tsingpig_lab.DataStructures import FenwickTree as FenwickTree
+        tr = FenwickTree(10)
+        tr.update(1, 1)
+        tr.update(2, 2)
+        tr.update(3, 5)
+        tr.update(1, 3)
+        # [0, 4, 2, 5, 0, 0, 0, 0, 0, 0]
+        print(tr.query(1, 10))	# 11
+        ```
+        
+        Example with discretization锛宨t allows the input array `nums` has repeated elements.
+        
+        ```python
+        from tsingpig_lab.DataStructures import FenwickTree as FenwickTree
+        nums = [1, 9, -99, 2, 4, 5, -99]
+        ft = FenwickTree(len(nums), discretize=True, nums=nums)
+        ft.update(2, 4)
+        ft.update(-99, 3)
+        # [0, 0, 3, 4, 0, 0]
+        print(ft.query(-99, 9)) # 7
+        ```
+        
+        
+        
+        #### 2.1.3 Segment Tree
+        
+        **Usage**
+        
+        | Method                                    | Time Complexity | Description                                                  |
+        | ----------------------------------------- | --------------- | ------------------------------------------------------------ |
+        | `__init__(nums, ops='sum')`               | $O(n)$          | Initialize the Segment Tree data structure with the given array `nums` and operation type `ops`, defaulting to sum operation. |
+        | `build(idx=1, l=1, r=None)`               | $O(n)$          | Build the Segment Tree.                                      |
+        | `update(ul, ur, val, idx=1, l=1, r=None)` | $O(\log n)$     | Update the range [ul, ur] with the given value `val`.        |
+        | `query(ql, qr, idx=1, l=1, r=None)`       | $O(\log n)$     | Query the result value within the range [ql, qr].            |
+        
+        **Sample**
+        
+        ```python
+        from tsingpig_lab.DataStructures import SegmentTree as SegmentTree
+        
+        tr = SegmentTree([1, 2, 3, 4, 5], 'sum')
+        tr.build()
+        print(tr.query(1, 5))  # 15
+        print(tr.query(2, 5))  # 14
+        tr.update(2, 4, 2)  # 1 4 5 6 5
+        print(tr.query(2, 5))  # 20
+        
+        tr = SegmentTree([8, 4, 5, 7, 9], 'min')
+        tr.build()
+        print(tr.query(1, 4)) # 4
+        tr.update(1, 4, 5) # [5, 4, 5, 5, 9]
+        print(tr.query(4, 5)) # 5
+        tr.update(3, 5, -10) # [5, 4, -10, -10, -10]
+        print(tr.query(1, 3)) # -10
+        ```
+        
+        
+        
+        > Note: The index is start with 1.
         
         ### 2.2. Algorithms
         
         #### 2.2.1 BaseConverter 
         
         Using for convert input number with base-a to result number with base-b.
         
         **Usage**
         
         | Method                     | Time Complexity | Description                                                  |
         | -------------------------- | --------------- | ------------------------------------------------------------ |
         | `__init__(a: int, b: int)` | N/A             | Initialize the BaseConverter with base `a` to convert numbers to base `b`. The bases must be within the range [2, 16]. |
         | `convert(num: str) -> str` | $O(\log n)$     | Convert a number in base `a` (given as a string) to its representation in base `b`. |
         
-        **Simple**
+        **Example **
         
         As shown below, you create a base converter from base-10 to base-2.
         
         ```python
         from tsingpig_lab.Algorithms import BaseConverter
         baseCon = BaseConverter(10, 2)
         print(baseCon.convert("123"))  # 1111011
@@ -88,25 +165,25 @@
         
         ```python
         from tsingpig_lab.Algorithms import BaseConverter
         baseCon = BaseConverter(16, 10)
         print(baseCon.convert("1BF52"))  # 114514
         ```
         
-        ### 2.2.2 Bin
+        #### 2.2.2 Bin
         
         **Usage**
         
         | Method                            | Time Complexity | Description                                                  |
         | --------------------------------- | --------------- | ------------------------------------------------------------ |
         | `__init__(num: str, b: int = 2) ` | N/A             | Initialize the Bin object with a number string `num` in base `b` (default is binary). If `b` is not 2, it converts the number from base `b` to base 2. |
         | `grey_to_bin() -> str `           | $O(n)$          | Converts the stored binary string, treated as a Gray code, to its corresponding binary code. $n$ is the length of the binary representation of $num$ . |
         | `bin_to_grey() -> str`            | $O(n)$          | Converts the stored binary string, treated as a binary code, to its corresponding Gray code. |
         
-        **Simple**
+        **Example **
         
         As shown below, you initialize a binary object base on 2.
         
         ```python
         from tsingpig_lab.Algorithms import Bin
         b = Bin('1111')
         ```
@@ -141,33 +218,33 @@
         # 3. Note for Pypi
         
         **How to upload your own package**
         
         Firstly, open your package folder and type this command in its' corresponding cmd:
         
         ```
-         python setup.py sdist
+        python setup.py sdist
         ```
         
         Then:
         
         ```
         twine upload dist/*
         ```
         
         And then it works, users can download your package by this line in conda:
         
         ```
-        pip install TsingPig-Lab==0.1.5 -i https://www.pypi.org/simple/
+        pip install TsingPig-Lab==0.1.6 -i https://www.pypi.org/simple/
         ```
         
         API
         
         ```
-        pypi-AgEIcHlwaS5vcmcCJDMxZTVjYjEwLTI1ZjgtNDkyYy1hYjk5LTIwODhkMmRhOGU4MQACKlszLCI3NDRkODY1Ni02ODE3LTRiNjEtYTliMi1kZThmOTI0YjQ5ZWEiXQAABiA7fW5wFoRjJYg7bF0l9tnQWja3Lo-ag6U96-XcTmKChw
+        pypi-AgEIcHlwaS5vcmcCJDg0MjZkZGM0LWQ0MjQtNGUyNC04NWI3LTExMTMwYTE4NjU2NQACKlszLCI3NDRkODY1Ni02ODE3LTRiNjEtYTliMi1kZThmOTI0YjQ5ZWEiXQAABiBN54j1SgGHWIqkPfyu1Iq3i5qwGrUB5UGPpeEYpyIf4A
         ```
         
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `TsingPig_Lab-0.1.6/setup.py` & `TsingPig_Lab-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `TsingPig_Lab-0.1.6/tsingpig_lab/Algorithms.py` & `TsingPig_Lab-0.1.7/tsingpig_lab/Algorithms.py`

 * *Files identical despite different names*

