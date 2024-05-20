# Comparing `tmp/azizkitten-11.1.1.tar.gz` & `tmp/azizkitten-11.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azizkitten-11.1.1.tar", last modified: Thu May 16 18:33:04 2024, max compression
+gzip compressed data, was "azizkitten-11.1.2.tar", last modified: Mon May 20 17:14:28 2024, max compression
```

## Comparing `azizkitten-11.1.1.tar` & `azizkitten-11.1.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 18:33:04.486074 azizkitten-11.1.1/
-drwxrwxrwx   0        0        0        0 2024-05-16 18:33:04.474647 azizkitten-11.1.1/AzizKitten/
--rw-rw-rw-   0        0        0      956 2024-05-16 18:30:48.000000 azizkitten-11.1.1/AzizKitten/__init__.py
--rw-rw-rw-   0        0        0      199 2024-02-06 13:32:20.000000 azizkitten-11.1.1/AzizKitten/acos.py
--rw-rw-rw-   0        0        0       64 2024-02-06 13:34:15.000000 azizkitten-11.1.1/AzizKitten/acot.py
--rw-rw-rw-   0        0        0       64 2024-02-06 13:33:55.000000 azizkitten-11.1.1/AzizKitten/acsc.py
--rw-rw-rw-   0        0        0    19953 2024-02-06 12:37:23.000000 azizkitten-11.1.1/AzizKitten/among_us.py
--rw-rw-rw-   0        0        0       64 2024-02-06 13:33:33.000000 azizkitten-11.1.1/AzizKitten/asec.py
--rw-rw-rw-   0        0        0      406 2024-02-06 13:31:30.000000 azizkitten-11.1.1/AzizKitten/asin.py
--rw-rw-rw-   0        0        0      141 2024-05-16 17:14:01.000000 azizkitten-11.1.1/AzizKitten/atan.py
--rw-rw-rw-   0        0        0      409 2024-02-06 12:37:23.000000 azizkitten-11.1.1/AzizKitten/bin_rep.py
--rw-rw-rw-   0        0        0     2128 2024-05-16 17:14:20.000000 azizkitten-11.1.1/AzizKitten/cbrt.py
--rw-rw-rw-   0        0        0      199 2024-05-16 17:28:31.000000 azizkitten-11.1.1/AzizKitten/constants.py
--rw-rw-rw-   0        0        0      306 2024-05-16 17:14:09.000000 azizkitten-11.1.1/AzizKitten/cos.py
--rw-rw-rw-   0        0        0       71 2024-02-09 14:35:45.000000 azizkitten-11.1.1/AzizKitten/cosh.py
--rw-rw-rw-   0        0        0      168 2024-02-24 15:38:52.000000 azizkitten-11.1.1/AzizKitten/cot.py
--rw-rw-rw-   0        0        0       96 2024-02-24 15:39:19.000000 azizkitten-11.1.1/AzizKitten/coth.py
--rw-rw-rw-   0        0        0      139 2024-02-06 13:26:25.000000 azizkitten-11.1.1/AzizKitten/csc.py
--rw-rw-rw-   0        0        0       62 2024-02-09 14:42:18.000000 azizkitten-11.1.1/AzizKitten/csch.py
--rw-rw-rw-   0        0        0     2230 2024-05-16 18:29:38.000000 azizkitten-11.1.1/AzizKitten/cubic.py
--rw-rw-rw-   0        0        0       67 2024-05-16 18:30:33.000000 azizkitten-11.1.1/AzizKitten/degrees.py
--rw-rw-rw-   0        0        0       60 2024-02-06 13:34:42.000000 azizkitten-11.1.1/AzizKitten/exp.py
--rw-rw-rw-   0        0        0      506 2024-05-14 18:00:41.000000 azizkitten-11.1.1/AzizKitten/factorial.py
--rw-rw-rw-   0        0        0      135 2024-02-10 09:32:39.000000 azizkitten-11.1.1/AzizKitten/floor.py
--rw-rw-rw-   0        0        0       81 2024-02-07 12:42:22.000000 azizkitten-11.1.1/AzizKitten/gcd.py
--rw-rw-rw-   0        0        0      605 2024-05-14 17:51:40.000000 azizkitten-11.1.1/AzizKitten/integrate.py
--rw-rw-rw-   0        0        0       82 2024-02-07 12:42:13.000000 azizkitten-11.1.1/AzizKitten/lcm.py
--rw-rw-rw-   0        0        0     1485 2024-02-10 11:22:50.000000 azizkitten-11.1.1/AzizKitten/limit.py
--rw-rw-rw-   0        0        0      516 2024-05-14 17:38:20.000000 azizkitten-11.1.1/AzizKitten/ln.py
--rw-rw-rw-   0        0        0       74 2024-02-06 13:22:15.000000 azizkitten-11.1.1/AzizKitten/log.py
--rw-rw-rw-   0        0        0     2249 2024-02-06 12:37:23.000000 azizkitten-11.1.1/AzizKitten/ment_calc.py
--rw-rw-rw-   0        0        0     6268 2024-02-06 12:37:23.000000 azizkitten-11.1.1/AzizKitten/mystery.py
--rw-rw-rw-   0        0        0      560 2024-05-16 17:14:04.000000 azizkitten-11.1.1/AzizKitten/quad.py
--rw-rw-rw-   0        0        0       69 2024-05-16 18:30:59.000000 azizkitten-11.1.1/AzizKitten/radians.py
--rw-rw-rw-   0        0        0      139 2024-02-06 13:30:00.000000 azizkitten-11.1.1/AzizKitten/sec.py
--rw-rw-rw-   0        0        0       62 2024-02-09 14:41:44.000000 azizkitten-11.1.1/AzizKitten/sech.py
--rw-rw-rw-   0        0        0      310 2024-05-16 17:14:11.000000 azizkitten-11.1.1/AzizKitten/sin.py
--rw-rw-rw-   0        0        0       71 2024-02-10 11:23:11.000000 azizkitten-11.1.1/AzizKitten/sinh.py
--rw-rw-rw-   0        0        0      114 2024-05-14 17:41:04.000000 azizkitten-11.1.1/AzizKitten/sqrt.py
--rw-rw-rw-   0        0        0      169 2024-02-06 13:30:05.000000 azizkitten-11.1.1/AzizKitten/tan.py
--rw-rw-rw-   0        0        0       96 2024-02-09 14:36:37.000000 azizkitten-11.1.1/AzizKitten/tanh.py
-drwxrwxrwx   0        0        0        0 2024-05-16 18:33:04.484348 azizkitten-11.1.1/AzizKitten.egg-info/
--rw-rw-rw-   0        0        0      785 2024-05-16 18:33:04.000000 azizkitten-11.1.1/AzizKitten.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      961 2024-05-16 18:33:04.000000 azizkitten-11.1.1/AzizKitten.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 18:33:04.000000 azizkitten-11.1.1/AzizKitten.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-16 18:33:04.000000 azizkitten-11.1.1/AzizKitten.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1055 2024-02-06 12:37:22.000000 azizkitten-11.1.1/LICENSE
--rw-rw-rw-   0        0        0       84 2024-02-06 12:37:22.000000 azizkitten-11.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0      785 2024-05-16 18:33:04.485347 azizkitten-11.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      173 2024-02-06 12:37:22.000000 azizkitten-11.1.1/README.md
--rw-rw-rw-   0        0        0      673 2024-05-16 18:31:35.000000 azizkitten-11.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-16 18:33:04.487073 azizkitten-11.1.1/setup.cfg
--rw-rw-rw-   0        0        0      708 2024-05-16 18:31:15.000000 azizkitten-11.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:14:28.139589 azizkitten-11.1.2/
+drwxrwxrwx   0        0        0        0 2024-05-20 17:14:28.124585 azizkitten-11.1.2/AzizKitten/
+-rw-rw-rw-   0        0        0      956 2024-05-16 18:30:48.000000 azizkitten-11.1.2/AzizKitten/__init__.py
+-rw-rw-rw-   0        0        0      199 2024-02-06 13:32:20.000000 azizkitten-11.1.2/AzizKitten/acos.py
+-rw-rw-rw-   0        0        0       64 2024-02-06 13:34:15.000000 azizkitten-11.1.2/AzizKitten/acot.py
+-rw-rw-rw-   0        0        0       64 2024-02-06 13:33:55.000000 azizkitten-11.1.2/AzizKitten/acsc.py
+-rw-rw-rw-   0        0        0    19953 2024-02-06 12:37:23.000000 azizkitten-11.1.2/AzizKitten/among_us.py
+-rw-rw-rw-   0        0        0       64 2024-02-06 13:33:33.000000 azizkitten-11.1.2/AzizKitten/asec.py
+-rw-rw-rw-   0        0        0      406 2024-02-06 13:31:30.000000 azizkitten-11.1.2/AzizKitten/asin.py
+-rw-rw-rw-   0        0        0      141 2024-05-16 17:14:01.000000 azizkitten-11.1.2/AzizKitten/atan.py
+-rw-rw-rw-   0        0        0      409 2024-02-06 12:37:23.000000 azizkitten-11.1.2/AzizKitten/bin_rep.py
+-rw-rw-rw-   0        0        0     2128 2024-05-16 17:14:20.000000 azizkitten-11.1.2/AzizKitten/cbrt.py
+-rw-rw-rw-   0        0        0      199 2024-05-16 17:28:31.000000 azizkitten-11.1.2/AzizKitten/constants.py
+-rw-rw-rw-   0        0        0      306 2024-05-16 17:14:09.000000 azizkitten-11.1.2/AzizKitten/cos.py
+-rw-rw-rw-   0        0        0       71 2024-02-09 14:35:45.000000 azizkitten-11.1.2/AzizKitten/cosh.py
+-rw-rw-rw-   0        0        0      168 2024-02-24 15:38:52.000000 azizkitten-11.1.2/AzizKitten/cot.py
+-rw-rw-rw-   0        0        0       96 2024-02-24 15:39:19.000000 azizkitten-11.1.2/AzizKitten/coth.py
+-rw-rw-rw-   0        0        0      139 2024-02-06 13:26:25.000000 azizkitten-11.1.2/AzizKitten/csc.py
+-rw-rw-rw-   0        0        0       62 2024-02-09 14:42:18.000000 azizkitten-11.1.2/AzizKitten/csch.py
+-rw-rw-rw-   0        0        0     2312 2024-05-20 17:12:54.000000 azizkitten-11.1.2/AzizKitten/cubic.py
+-rw-rw-rw-   0        0        0       67 2024-05-16 18:30:33.000000 azizkitten-11.1.2/AzizKitten/degrees.py
+-rw-rw-rw-   0        0        0       60 2024-02-06 13:34:42.000000 azizkitten-11.1.2/AzizKitten/exp.py
+-rw-rw-rw-   0        0        0      506 2024-05-14 18:00:41.000000 azizkitten-11.1.2/AzizKitten/factorial.py
+-rw-rw-rw-   0        0        0      135 2024-02-10 09:32:39.000000 azizkitten-11.1.2/AzizKitten/floor.py
+-rw-rw-rw-   0        0        0       81 2024-02-07 12:42:22.000000 azizkitten-11.1.2/AzizKitten/gcd.py
+-rw-rw-rw-   0        0        0      605 2024-05-14 17:51:40.000000 azizkitten-11.1.2/AzizKitten/integrate.py
+-rw-rw-rw-   0        0        0       82 2024-02-07 12:42:13.000000 azizkitten-11.1.2/AzizKitten/lcm.py
+-rw-rw-rw-   0        0        0     1485 2024-02-10 11:22:50.000000 azizkitten-11.1.2/AzizKitten/limit.py
+-rw-rw-rw-   0        0        0      516 2024-05-14 17:38:20.000000 azizkitten-11.1.2/AzizKitten/ln.py
+-rw-rw-rw-   0        0        0       74 2024-02-06 13:22:15.000000 azizkitten-11.1.2/AzizKitten/log.py
+-rw-rw-rw-   0        0        0     2249 2024-02-06 12:37:23.000000 azizkitten-11.1.2/AzizKitten/ment_calc.py
+-rw-rw-rw-   0        0        0     6268 2024-02-06 12:37:23.000000 azizkitten-11.1.2/AzizKitten/mystery.py
+-rw-rw-rw-   0        0        0      560 2024-05-16 17:14:04.000000 azizkitten-11.1.2/AzizKitten/quad.py
+-rw-rw-rw-   0        0        0       69 2024-05-16 18:30:59.000000 azizkitten-11.1.2/AzizKitten/radians.py
+-rw-rw-rw-   0        0        0      139 2024-02-06 13:30:00.000000 azizkitten-11.1.2/AzizKitten/sec.py
+-rw-rw-rw-   0        0        0       62 2024-02-09 14:41:44.000000 azizkitten-11.1.2/AzizKitten/sech.py
+-rw-rw-rw-   0        0        0      310 2024-05-16 17:14:11.000000 azizkitten-11.1.2/AzizKitten/sin.py
+-rw-rw-rw-   0        0        0       71 2024-02-10 11:23:11.000000 azizkitten-11.1.2/AzizKitten/sinh.py
+-rw-rw-rw-   0        0        0      114 2024-05-14 17:41:04.000000 azizkitten-11.1.2/AzizKitten/sqrt.py
+-rw-rw-rw-   0        0        0      169 2024-02-06 13:30:05.000000 azizkitten-11.1.2/AzizKitten/tan.py
+-rw-rw-rw-   0        0        0       96 2024-02-09 14:36:37.000000 azizkitten-11.1.2/AzizKitten/tanh.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:14:28.136585 azizkitten-11.1.2/AzizKitten.egg-info/
+-rw-rw-rw-   0        0        0      785 2024-05-20 17:14:27.000000 azizkitten-11.1.2/AzizKitten.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      961 2024-05-20 17:14:28.000000 azizkitten-11.1.2/AzizKitten.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 17:14:27.000000 azizkitten-11.1.2/AzizKitten.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-20 17:14:27.000000 azizkitten-11.1.2/AzizKitten.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1055 2024-02-06 12:37:22.000000 azizkitten-11.1.2/LICENSE
+-rw-rw-rw-   0        0        0       84 2024-02-06 12:37:22.000000 azizkitten-11.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      785 2024-05-20 17:14:28.138602 azizkitten-11.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2024-02-06 12:37:22.000000 azizkitten-11.1.2/README.md
+-rw-rw-rw-   0        0        0      673 2024-05-20 17:13:36.000000 azizkitten-11.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-20 17:14:28.140588 azizkitten-11.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      708 2024-05-20 17:13:44.000000 azizkitten-11.1.2/setup.py
```

### Comparing `azizkitten-11.1.1/AzizKitten/__init__.py` & `azizkitten-11.1.2/AzizKitten/__init__.py`

 * *Files identical despite different names*

### Comparing `azizkitten-11.1.1/AzizKitten/among_us.py` & `azizkitten-11.1.2/AzizKitten/among_us.py`

 * *Files identical despite different names*

### Comparing `azizkitten-11.1.1/AzizKitten/cbrt.py` & `azizkitten-11.1.2/AzizKitten/cbrt.py`

 * *Files identical despite different names*

### Comparing `azizkitten-11.1.1/AzizKitten/cubic.py` & `azizkitten-11.1.2/AzizKitten/cubic.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 def cubic(a,b,c,d):
     from .cbrt import cbrt
     from .sqrt import sqrt
     from .quad import quad
     if a == 0:
         raise ValueError("value of 'a' must be different to 0.")
-    if a+b+c+d == 0:
+    if d == 0:
+        quad(a,b,c)
+        cubic.x1, cubic.x2, cubic.x3 = 0, quad.x1, quad.x2
+    elif a+b+c+d == 0:
         A = a
         B = b+a
         C = -d
         quad(A,B,C)
-        cubic.x1 = 1
-        cubic.x2, cubic.x3 = quad.x1, quad.x2
+        cubic.x1, cubic.x2, cubic.x3 = 1, quad.x1, quad.x2
     elif -a+b-c+d == 0:
         A = a
         B = b-a
         C = d
         quad(A,B,C)
-        cubic.x1 = 1
-        cubic.x2, cubic.x3 = quad.x1, quad.x2
+        cubic.x1, cubic.x2, cubic.x3 = -1, quad.x1, quad.x2
     else:
         p = (3*a*c-b**2)/(3*a**2)
         q = (2*b**3-9*a*b*c+27*a**2*d)/(27*a**3)
         cubic.x1 = cbrt(-q/2+sqrt(q**2/4+p**3/27))+cbrt(-q/2-sqrt(q**2/4+p**3/27))-b/(3*a)
         cubic.x2 = (-1+sqrt(-3))/2*cbrt(-q/2+sqrt(q**2/4+p**3/27))+(-1-sqrt(-3))/2*cbrt(-q/2-sqrt(q**2/4+p**3/27))-b/(3*a)
         cubic.x3 = (-1-sqrt(-3))/2*cbrt(-q/2+sqrt(q**2/4+p**3/27))+(-1+sqrt(-3))/2*cbrt(-q/2-sqrt(q**2/4+p**3/27))-b/(3*a)
     if type(cubic.x1) is complex:
```

### Comparing `azizkitten-11.1.1/AzizKitten/integrate.py` & `azizkitten-11.1.2/AzizKitten/integrate.py`

 * *Files identical despite different names*

### Comparing `azizkitten-11.1.1/AzizKitten/limit.py` & `azizkitten-11.1.2/AzizKitten/limit.py`

 * *Files identical despite different names*

### Comparing `azizkitten-11.1.1/AzizKitten/ln.py` & `azizkitten-11.1.2/AzizKitten/ln.py`

 * *Files identical despite different names*

### Comparing `azizkitten-11.1.1/AzizKitten/ment_calc.py` & `azizkitten-11.1.2/AzizKitten/ment_calc.py`

 * *Files identical despite different names*

### Comparing `azizkitten-11.1.1/AzizKitten/mystery.py` & `azizkitten-11.1.2/AzizKitten/mystery.py`

 * *Files identical despite different names*

### Comparing `azizkitten-11.1.1/AzizKitten/quad.py` & `azizkitten-11.1.2/AzizKitten/quad.py`

 * *Files identical despite different names*

### Comparing `azizkitten-11.1.1/AzizKitten.egg-info/PKG-INFO` & `azizkitten-11.1.2/AzizKitten.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AzizKitten
-Version: 11.1.1
+Version: 11.1.2
 Summary: AzizOmrane's own Python package
 Author: AzizKitten
 Author-email: AzizKitten <azizprv43@gmail.com>
 Project-URL: AboutMe, https://azizkitten.github.io
 Project-URL: Documentation, https://azizkitten.github.io/python
 Project-URL: Bug Tracker, https://github.com/AzizKitten/azizkitten.github.io/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `azizkitten-11.1.1/AzizKitten.egg-info/SOURCES.txt` & `azizkitten-11.1.2/AzizKitten.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azizkitten-11.1.1/LICENSE` & `azizkitten-11.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `azizkitten-11.1.1/PKG-INFO` & `azizkitten-11.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AzizKitten
-Version: 11.1.1
+Version: 11.1.2
 Summary: AzizOmrane's own Python package
 Author: AzizKitten
 Author-email: AzizKitten <azizprv43@gmail.com>
 Project-URL: AboutMe, https://azizkitten.github.io
 Project-URL: Documentation, https://azizkitten.github.io/python
 Project-URL: Bug Tracker, https://github.com/AzizKitten/azizkitten.github.io/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `azizkitten-11.1.1/pyproject.toml` & `azizkitten-11.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "AzizKitten"
-version = "11.1.1"
+version = "11.1.2"
 authors = [
   { name="AzizKitten", email="azizprv43@gmail.com" },
 ]
 description = "AzizOmrane's own Python package"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `azizkitten-11.1.1/setup.py` & `azizkitten-11.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="AzizKitten",
-    version="11.1.1",
+    version="11.1.2",
     packages=find_packages(),
     include_package_data=True,
     author="AzizKitten",
     author_email="azizprv43@gmail.com",
     description="AzizOmrane's own python library",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

