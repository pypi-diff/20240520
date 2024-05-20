# Comparing `tmp/testplans-0.2.8.tar.gz` & `tmp/testplans-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testplans-0.2.8.tar", last modified: Wed May  8 10:13:28 2024, max compression
+gzip compressed data, was "testplans-0.2.9.tar", last modified: Wed May  8 10:45:20 2024, max compression
```

## Comparing `testplans-0.2.8.tar` & `testplans-0.2.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 10:13:28.027063 testplans-0.2.8/
--rw-rw-rw-   0        0        0     1082 2023-11-27 14:37:20.000000 testplans-0.2.8/LICENSE
--rw-rw-rw-   0        0        0     5494 2024-05-08 10:13:28.027063 testplans-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     4584 2024-05-08 10:12:56.000000 testplans-0.2.8/README.md
--rw-rw-rw-   0        0        0       42 2024-05-08 10:13:28.028061 testplans-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 testplans-0.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:13:28.019610 testplans-0.2.8/testplans/
--rw-rw-rw-   0        0        0      105 2024-02-01 12:13:36.000000 testplans-0.2.8/testplans/__init__.py
--rw-rw-rw-   0        0        0      776 2024-03-15 14:57:12.000000 testplans-0.2.8/testplans/_results.py
--rw-rw-rw-   0        0        0     3974 2024-05-08 07:37:04.000000 testplans-0.2.8/testplans/api.py
--rw-rw-rw-   0        0        0     7686 2024-04-22 13:45:33.000000 testplans-0.2.8/testplans/devices.py
--rw-rw-rw-   0        0        0     6347 2024-04-22 14:33:47.000000 testplans-0.2.8/testplans/gui.py
--rw-rw-rw-   0        0        0    11908 2024-05-08 07:37:04.000000 testplans-0.2.8/testplans/main.py
--rw-rw-rw-   0        0        0     1561 2024-04-22 14:50:31.000000 testplans-0.2.8/testplans/models.py
--rw-rw-rw-   0        0        0    12244 2024-05-08 10:11:05.000000 testplans-0.2.8/testplans/tc.py
--rw-rw-rw-   0        0        0     8975 2024-04-26 12:19:02.000000 testplans-0.2.8/testplans/tm.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:13:28.026038 testplans-0.2.8/testplans.egg-info/
--rw-rw-rw-   0        0        0     5494 2024-05-08 10:13:27.000000 testplans-0.2.8/testplans.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2024-05-08 10:13:28.000000 testplans-0.2.8/testplans.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 10:13:27.000000 testplans-0.2.8/testplans.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-08 10:13:27.000000 testplans-0.2.8/testplans.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 10:45:20.597301 testplans-0.2.9/
+-rw-rw-rw-   0        0        0     1082 2023-11-27 14:37:20.000000 testplans-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0     5494 2024-05-08 10:45:20.596800 testplans-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4584 2024-05-08 10:43:50.000000 testplans-0.2.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-08 10:45:20.597301 testplans-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 testplans-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:45:20.591714 testplans-0.2.9/testplans/
+-rw-rw-rw-   0        0        0      105 2024-02-01 12:13:36.000000 testplans-0.2.9/testplans/__init__.py
+-rw-rw-rw-   0        0        0      776 2024-03-15 14:57:12.000000 testplans-0.2.9/testplans/_results.py
+-rw-rw-rw-   0        0        0     3974 2024-05-08 07:37:04.000000 testplans-0.2.9/testplans/api.py
+-rw-rw-rw-   0        0        0     7686 2024-04-22 13:45:33.000000 testplans-0.2.9/testplans/devices.py
+-rw-rw-rw-   0        0        0     6347 2024-04-22 14:33:47.000000 testplans-0.2.9/testplans/gui.py
+-rw-rw-rw-   0        0        0    11898 2024-05-08 10:43:49.000000 testplans-0.2.9/testplans/main.py
+-rw-rw-rw-   0        0        0     1561 2024-04-22 14:50:31.000000 testplans-0.2.9/testplans/models.py
+-rw-rw-rw-   0        0        0    12340 2024-05-08 10:43:49.000000 testplans-0.2.9/testplans/tc.py
+-rw-rw-rw-   0        0        0     8975 2024-04-26 12:19:02.000000 testplans-0.2.9/testplans/tm.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:45:20.595738 testplans-0.2.9/testplans.egg-info/
+-rw-rw-rw-   0        0        0     5494 2024-05-08 10:45:20.000000 testplans-0.2.9/testplans.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2024-05-08 10:45:20.000000 testplans-0.2.9/testplans.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 10:45:20.000000 testplans-0.2.9/testplans.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-08 10:45:20.000000 testplans-0.2.9/testplans.egg-info/top_level.txt
```

### Comparing `testplans-0.2.8/LICENSE` & `testplans-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `testplans-0.2.8/PKG-INFO` & `testplans-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testplans
-Version: 0.2.8
+Version: 0.2.9
 Summary: simple testplan framework for several DUTs
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/testplans
 Keywords: testplan,testplan structure framework,testplan gui,testplan multy dut,testplan several dut
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# testplans (v0.2.8)
+# testplans (v0.2.9)
 
 ## DESCRIPTION_SHORT
 simple testplan framework for several DUTs
 
 ## DESCRIPTION_LONG
 designed to apply testplan for several DUTs
```

### Comparing `testplans-0.2.8/README.md` & `testplans-0.2.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# testplans (v0.2.8)
+# testplans (v0.2.9)
 
 ## DESCRIPTION_SHORT
 simple testplan framework for several DUTs
 
 ## DESCRIPTION_LONG
 designed to apply testplan for several DUTs
```

### Comparing `testplans-0.2.8/setup.py` & `testplans-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.8/testplans/_results.py` & `testplans-0.2.9/testplans/_results.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.8/testplans/api.py` & `testplans-0.2.9/testplans/api.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.8/testplans/devices.py` & `testplans-0.2.9/testplans/devices.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.8/testplans/gui.py` & `testplans-0.2.9/testplans/gui.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.8/testplans/main.py` & `testplans-0.2.9/testplans/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -235,21 +235,19 @@
         self.tp__teardown(0)
 
     def run(self) -> None:
         self.LOGGER.debug("TP START")
         if self.tp__check_active():
             return
 
-        if not self.tp__startup():
-            return
-
-        for step, tc in enumerate(self.TCS__CLS, start=1):
-            self.progress = int(step / len(self.TCS__CLS) * 100) - 1
-            self.tc_active = tc
-            tc.run__cls()
+        if self.tp__startup():
+            for step, tc in enumerate(self.TCS__CLS, start=1):
+                self.progress = int(step / len(self.TCS__CLS) * 100) - 1
+                self.tc_active = tc
+                tc.run__cls()
 
         # FINISH TP ---------------------------------------------------
         self.tp__teardown()
         self.LOGGER.debug("TP FINISH")
 
     # =================================================================================================================
     def get__info__stand(self) -> ModelStand:
```

### Comparing `testplans-0.2.8/testplans/models.py` & `testplans-0.2.9/testplans/models.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.8/testplans/tc.py` & `testplans-0.2.9/testplans/tc.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,34 +298,33 @@
         # ---------------------------------
         print(f"run__cls=clear__cls")
         cls.clear__cls()
 
         print(f"run__cls=startup__cls")
         cls.result__cls_startup = cls.startup__cls()
         print(f"run__cls={cls.result__cls_startup=}")
-        if not cls.result__cls_startup:
-            return
-
-        # BATCH --------------------------
-        for tc_inst in cls.TCS__INST:
-            if tc_inst.skip_tc_dut:
-                continue
-
-            print(f"run__cls=tc_inst.start({tc_inst.INDEX=})")
-            tc_inst.start()
-            if not cls.ASYNC:
-                print(f"run__cls=tc_inst.wait({tc_inst.INDEX=})inONEBYONE")
-                tc_inst.wait()
-
-        # FINISH --------------------------
-        if cls.ASYNC:
+        if cls.result__cls_startup:
+            # BATCH --------------------------
             for tc_inst in cls.TCS__INST:
-                print(f"run__cls=tc_inst.wait({tc_inst.INDEX=})inPARALLEL")
-                tc_inst.wait()
+                if tc_inst.skip_tc_dut:
+                    continue
+
+                print(f"run__cls=tc_inst.start({tc_inst.INDEX=})")
+                tc_inst.start()
+                if not cls.ASYNC:
+                    print(f"run__cls=tc_inst.wait({tc_inst.INDEX=})inONEBYONE")
+                    tc_inst.wait()
+
+            # WAIT --------------------------
+            if cls.ASYNC:
+                for tc_inst in cls.TCS__INST:
+                    print(f"run__cls=tc_inst.wait({tc_inst.INDEX=})inPARALLEL")
+                    tc_inst.wait()
 
+        # FINISH -------------------------------------------------
         print(f"run__cls=teardown__cls")
         cls.teardown__cls()
         print(f"run__cls=FINISH={cls.NAME=}={'='*50}")
 
     # REDEFINE ========================================================================================================
     pass
     pass
```

### Comparing `testplans-0.2.8/testplans/tm.py` & `testplans-0.2.9/testplans/tm.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.8/testplans.egg-info/PKG-INFO` & `testplans-0.2.9/testplans.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testplans
-Version: 0.2.8
+Version: 0.2.9
 Summary: simple testplan framework for several DUTs
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/testplans
 Keywords: testplan,testplan structure framework,testplan gui,testplan multy dut,testplan several dut
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# testplans (v0.2.8)
+# testplans (v0.2.9)
 
 ## DESCRIPTION_SHORT
 simple testplan framework for several DUTs
 
 ## DESCRIPTION_LONG
 designed to apply testplan for several DUTs
```

