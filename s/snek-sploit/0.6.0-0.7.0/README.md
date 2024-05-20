# Comparing `tmp/snek_sploit-0.6.0.tar.gz` & `tmp/snek_sploit-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snek_sploit-0.6.0.tar", max compression
+gzip compressed data, was "snek_sploit-0.7.0.tar", max compression
```

## Comparing `snek_sploit-0.6.0.tar` & `snek_sploit-0.7.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1069 2024-05-14 08:38:36.810348 snek_sploit-0.6.0/LICENSE
--rw-r--r--   0        0        0     1539 2024-05-14 08:38:36.810348 snek_sploit-0.6.0/README.md
--rw-r--r--   0        0        0      686 2024-05-14 08:38:36.810348 snek_sploit-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     1393 2024-05-14 08:38:36.810348 snek_sploit-0.6.0/snek_sploit/__init__.py
--rw-r--r--   0        0        0        0 2024-05-14 08:38:36.810348 snek_sploit-0.6.0/snek_sploit/lib/__init__.py
--rw-r--r--   0        0        0     4696 2024-05-14 08:38:36.814348 snek_sploit-0.6.0/snek_sploit/lib/context.py
--rw-r--r--   0        0        0     3004 2024-05-14 08:38:36.814348 snek_sploit-0.6.0/snek_sploit/lib/metasploit.py
--rw-r--r--   0        0        0        0 2024-05-14 08:38:36.814348 snek_sploit-0.6.0/snek_sploit/lib/rpc/__init__.py
--rw-r--r--   0        0        0     3086 2024-05-14 08:38:36.814348 snek_sploit-0.6.0/snek_sploit/lib/rpc/auth.py
--rw-r--r--   0        0        0    10952 2024-05-14 08:38:36.814348 snek_sploit-0.6.0/snek_sploit/lib/rpc/consoles.py
--rw-r--r--   0        0        0     7892 2024-05-14 08:38:36.814348 snek_sploit-0.6.0/snek_sploit/lib/rpc/core.py
--rw-r--r--   0        0        0    12331 2024-05-14 08:38:36.814348 snek_sploit-0.6.0/snek_sploit/lib/rpc/db.py
--rw-r--r--   0        0        0      728 2024-05-14 08:38:36.814348 snek_sploit-0.6.0/snek_sploit/lib/rpc/health.py
--rw-r--r--   0        0        0     2676 2024-05-14 08:38:36.814348 snek_sploit-0.6.0/snek_sploit/lib/rpc/jobs.py
--rw-r--r--   0        0        0    19865 2024-05-14 08:38:36.814348 snek_sploit-0.6.0/snek_sploit/lib/rpc/modules.py
--rw-r--r--   0        0        0     1629 2024-05-14 08:38:36.814348 snek_sploit-0.6.0/snek_sploit/lib/rpc/plugins.py
--rw-r--r--   0        0        0    24221 2024-05-14 08:38:36.814348 snek_sploit-0.6.0/snek_sploit/lib/rpc/sessions.py
--rw-r--r--   0        0        0        0 2024-05-14 08:38:36.814348 snek_sploit-0.6.0/snek_sploit/util/__init__.py
--rw-r--r--   0        0        0     1887 2024-05-14 08:38:36.814348 snek_sploit-0.6.0/snek_sploit/util/constants.py
--rw-r--r--   0        0        0      448 2024-05-14 08:38:36.814348 snek_sploit-0.6.0/snek_sploit/util/enums.py
--rw-r--r--   0        0        0      276 2024-05-14 08:38:36.814348 snek_sploit-0.6.0/snek_sploit/util/exceptions.py
--rw-r--r--   0        0        0      713 2024-05-14 08:38:36.814348 snek_sploit-0.6.0/snek_sploit/util/retry.py
--rw-r--r--   0        0        0     2439 1970-01-01 00:00:00.000000 snek_sploit-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-20 10:59:51.205724 snek_sploit-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1539 2024-05-20 10:59:51.205724 snek_sploit-0.7.0/README.md
+-rw-r--r--   0        0        0      686 2024-05-20 10:59:51.205724 snek_sploit-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1393 2024-05-20 10:59:51.205724 snek_sploit-0.7.0/snek_sploit/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-20 10:59:51.205724 snek_sploit-0.7.0/snek_sploit/lib/__init__.py
+-rw-r--r--   0        0        0     4696 2024-05-20 10:59:51.205724 snek_sploit-0.7.0/snek_sploit/lib/context.py
+-rw-r--r--   0        0        0     3004 2024-05-20 10:59:51.205724 snek_sploit-0.7.0/snek_sploit/lib/metasploit.py
+-rw-r--r--   0        0        0        0 2024-05-20 10:59:51.205724 snek_sploit-0.7.0/snek_sploit/lib/rpc/__init__.py
+-rw-r--r--   0        0        0     3086 2024-05-20 10:59:51.205724 snek_sploit-0.7.0/snek_sploit/lib/rpc/auth.py
+-rw-r--r--   0        0        0    10952 2024-05-20 10:59:51.205724 snek_sploit-0.7.0/snek_sploit/lib/rpc/consoles.py
+-rw-r--r--   0        0        0     7892 2024-05-20 10:59:51.205724 snek_sploit-0.7.0/snek_sploit/lib/rpc/core.py
+-rw-r--r--   0        0        0    12331 2024-05-20 10:59:51.205724 snek_sploit-0.7.0/snek_sploit/lib/rpc/db.py
+-rw-r--r--   0        0        0      728 2024-05-20 10:59:51.205724 snek_sploit-0.7.0/snek_sploit/lib/rpc/health.py
+-rw-r--r--   0        0        0     2676 2024-05-20 10:59:51.205724 snek_sploit-0.7.0/snek_sploit/lib/rpc/jobs.py
+-rw-r--r--   0        0        0    19865 2024-05-20 10:59:51.205724 snek_sploit-0.7.0/snek_sploit/lib/rpc/modules.py
+-rw-r--r--   0        0        0     1629 2024-05-20 10:59:51.205724 snek_sploit-0.7.0/snek_sploit/lib/rpc/plugins.py
+-rw-r--r--   0        0        0    24454 2024-05-20 10:59:51.205724 snek_sploit-0.7.0/snek_sploit/lib/rpc/sessions.py
+-rw-r--r--   0        0        0        0 2024-05-20 10:59:51.205724 snek_sploit-0.7.0/snek_sploit/util/__init__.py
+-rw-r--r--   0        0        0     1887 2024-05-20 10:59:51.205724 snek_sploit-0.7.0/snek_sploit/util/constants.py
+-rw-r--r--   0        0        0      448 2024-05-20 10:59:51.205724 snek_sploit-0.7.0/snek_sploit/util/enums.py
+-rw-r--r--   0        0        0      276 2024-05-20 10:59:51.205724 snek_sploit-0.7.0/snek_sploit/util/exceptions.py
+-rw-r--r--   0        0        0      713 2024-05-20 10:59:51.205724 snek_sploit-0.7.0/snek_sploit/util/retry.py
+-rw-r--r--   0        0        0     2439 1970-01-01 00:00:00.000000 snek_sploit-0.7.0/PKG-INFO
```

### Comparing `snek_sploit-0.6.0/LICENSE` & `snek_sploit-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.6.0/README.md` & `snek_sploit-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.6.0/pyproject.toml` & `snek_sploit-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snek-sploit"
-version = "0.6.0"
+version = "0.7.0"
 description = "Python RPC client for Metasploit Framework"
 authors = [
     "Jiří Rája <jiri.raja@gmail.com>"
 ]
 maintainers = [
     "Jiří Rája <jiri.raja@gmail.com>"
 ]
```

### Comparing `snek_sploit-0.6.0/snek_sploit/__init__.py` & `snek_sploit-0.7.0/snek_sploit/__init__.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.6.0/snek_sploit/lib/context.py` & `snek_sploit-0.7.0/snek_sploit/lib/context.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.6.0/snek_sploit/lib/metasploit.py` & `snek_sploit-0.7.0/snek_sploit/lib/metasploit.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.6.0/snek_sploit/lib/rpc/auth.py` & `snek_sploit-0.7.0/snek_sploit/lib/rpc/auth.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.6.0/snek_sploit/lib/rpc/consoles.py` & `snek_sploit-0.7.0/snek_sploit/lib/rpc/consoles.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.6.0/snek_sploit/lib/rpc/core.py` & `snek_sploit-0.7.0/snek_sploit/lib/rpc/core.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.6.0/snek_sploit/lib/rpc/db.py` & `snek_sploit-0.7.0/snek_sploit/lib/rpc/db.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.6.0/snek_sploit/lib/rpc/health.py` & `snek_sploit-0.7.0/snek_sploit/lib/rpc/health.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.6.0/snek_sploit/lib/rpc/jobs.py` & `snek_sploit-0.7.0/snek_sploit/lib/rpc/jobs.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.6.0/snek_sploit/lib/rpc/modules.py` & `snek_sploit-0.7.0/snek_sploit/lib/rpc/modules.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.6.0/snek_sploit/lib/rpc/plugins.py` & `snek_sploit-0.7.0/snek_sploit/lib/rpc/plugins.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.6.0/snek_sploit/lib/rpc/sessions.py` & `snek_sploit-0.7.0/snek_sploit/lib/rpc/sessions.py`

 * *Files 2% similar despite different names*

```diff
@@ -445,14 +445,26 @@
         minimal_execution_time: float,
         timeout: float,
         success_flags: List[str],
         reading_delay: float,
     ) -> str:
         pass
 
+    @abstractmethod
+    def execute_in_shell(
+        self,
+        executable: str,
+        arguments: List[str],
+        minimal_execution_time: float,
+        timeout: float,
+        success_flags: List[str],
+        reading_delay: float,
+    ) -> str:
+        pass
+
     def gather_output(
         self,
         minimal_execution_time: float = 3,
         timeout: float = None,
         success_flags: List[str] = None,
         reading_delay: float = 1,
     ) -> str:
@@ -499,44 +511,45 @@
     def write(self, data: str) -> bool:
         self._rpc.shell_write(self.id, data)
         return True
 
     def read(self) -> str:
         return self._rpc.shell_read(self.id)
 
-    def upgrade_to_meterpreter(self, local_host: str, local_port: int, payload: str = None) -> bool:
-        # TODO: Custom update_to_meterpreter implementation? https://github.com/rapid7/metasploit-framework/issues/8800
-        #  The current one fails since its unable to use x64 instead of x86 architecture, we could add an optional
-        #  payload argument, which would mitigate this issue partially
-        if payload is None:
-            return self._rpc.shell_upgrade(self.id, local_host, local_port)
-
-        # TODO: set PAYLOAD_OVERRIDE: linux/x64/meterpreter/reverse_tcp,
-        #  module: post/multi/manage/shell_to_meterpreter
-        return False
+    def upgrade_to_meterpreter(self, local_host: str, local_port: int) -> bool:
+        return self._rpc.shell_upgrade(self.id, local_host, local_port)
 
     def execute(
         self,
         command: str,
         minimal_execution_time: float = 3,
         timeout: float = None,
         success_flags: List[str] = None,
         reading_delay: float = 1,
     ) -> str:
         self.clear_buffer()
         self.write(command)
 
         return self.gather_output(minimal_execution_time, timeout, success_flags, reading_delay)
 
+    def execute_in_shell(
+        self,
+        executable: str,
+        arguments: List[str],
+        minimal_execution_time: float = 3,
+        timeout: float = None,
+        success_flags: List[str] = None,
+        reading_delay: float = 1,
+    ) -> str:
+        command = " ".join([executable, *arguments])
+
+        return self.execute(command, minimal_execution_time, timeout, success_flags, reading_delay)
+
 
 class SessionMeterpreter(Session):
-    # TODO: execute and execute_in_shell are partially finished, since they have to be tested with the x64 payload.
-    #   If it works seamlessly, then good. However, even if it works, try to play with the run_single and channel
-    #   combination a bit more. Also, make sure to remove the process ID, or save it into memory or return it. Right
-    #   now it poisons the command output.
     @property
     def directory_separator(self):
         return self._rpc.meterpreter_directory_separator(self.id)
 
     def write(self, data: str) -> bool:
         return self._rpc.meterpreter_write(self.id, data)
 
@@ -569,25 +582,24 @@
         self.clear_buffer()
         self.write(command)
 
         return self.gather_output(minimal_execution_time, timeout, success_flags, reading_delay)
 
     def execute_in_shell(
         self,
-        command: str,
+        executable: str,
         arguments: List[str],
         minimal_execution_time: float = 3,
         timeout: float = None,
         success_flags: List[str] = None,
         reading_delay: float = 1,
     ) -> str:
+        # TODO: Remove the process ID from the output? eg. add postprocessing?
         self.clear_buffer()
-
-        # TODO: test with custom x64 payload
-        self.run_single(f"execute -f {command} -c -i -a {' '.join(arguments)}")
+        self.run_single(f"execute -f {executable} -c -i -a {' '.join(arguments)}")
 
         return self.gather_output(minimal_execution_time, timeout, success_flags, reading_delay)
 
 
 class SessionRing(Session):
     def write(self, data: str) -> bool:
         self._rpc.ring_put(self.id, data)
@@ -605,14 +617,27 @@
         reading_delay: float = 1,
     ) -> str:
         self.clear_buffer()
         self.write(command)
 
         return self.gather_output(minimal_execution_time, timeout, success_flags, reading_delay)
 
+    def execute_in_shell(
+        self,
+        executable: str,
+        arguments: List[str],
+        minimal_execution_time: float = 3,
+        timeout: float = None,
+        success_flags: List[str] = None,
+        reading_delay: float = 1,
+    ) -> str:
+        command = " ".join([executable, *arguments])
+
+        return self.execute(command, minimal_execution_time, timeout, success_flags, reading_delay)
+
 
 class Sessions(ContextBase):
     def __init__(self, context: Context):
         super().__init__(context)
         self.rpc = RPCSessions(context)
 
     def get(self, session_id: int) -> Union[SessionShell, SessionMeterpreter, SessionRing]:
```

### Comparing `snek_sploit-0.6.0/snek_sploit/util/constants.py` & `snek_sploit-0.7.0/snek_sploit/util/constants.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.6.0/snek_sploit/util/retry.py` & `snek_sploit-0.7.0/snek_sploit/util/retry.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.6.0/PKG-INFO` & `snek_sploit-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snek-sploit
-Version: 0.6.0
+Version: 0.7.0
 Summary: Python RPC client for Metasploit Framework
 Home-page: https://github.com/SadParad1se/snek-sploit
 License: MIT
 Keywords: metasploit,msf,rpc,client
 Author: Jiří Rája
 Author-email: jiri.raja@gmail.com
 Maintainer: Jiří Rája
```

