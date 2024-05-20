# Comparing `tmp/seqlogic-0.0.9.tar.gz` & `tmp/seqlogic-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqlogic-0.0.9.tar", last modified: Sun May  5 19:09:58 2024, max compression
+gzip compressed data, was "seqlogic-0.1.0.tar", last modified: Sun May 19 07:15:49 2024, max compression
```

## Comparing `seqlogic-0.0.9.tar` & `seqlogic-0.1.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 19:09:58.483721 seqlogic-0.0.9/
--rw-rw-rw-   0        0        0      956 2024-05-05 19:09:58.482539 seqlogic-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      740 2024-03-11 04:13:25.000000 seqlogic-0.0.9/README.md
--rw-rw-rw-   0        0        0      263 2024-05-05 19:09:14.000000 seqlogic-0.0.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-05 19:09:58.484723 seqlogic-0.0.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-05 19:09:58.418208 seqlogic-0.0.9/src/
-drwxrwxrwx   0        0        0        0 2024-05-05 19:09:58.434033 seqlogic-0.0.9/src/seqlogic/
--rw-rw-rw-   0        0        0      357 2024-05-05 19:08:40.000000 seqlogic-0.0.9/src/seqlogic/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 19:09:58.461745 seqlogic-0.0.9/src/seqlogic/algorithms/
--rw-rw-rw-   0        0        0       27 2023-11-27 07:28:50.000000 seqlogic-0.0.9/src/seqlogic/algorithms/__init__.py
--rw-rw-rw-   0        0        0    12685 2024-03-10 17:38:01.000000 seqlogic-0.0.9/src/seqlogic/algorithms/aes.py
--rw-rw-rw-   0        0        0      285 2024-04-30 03:11:09.000000 seqlogic-0.0.9/src/seqlogic/algorithms/gray.py
--rw-rw-rw-   0        0        0    21662 2024-05-05 19:08:40.000000 seqlogic-0.0.9/src/seqlogic/bits.py
--rw-rw-rw-   0        0        0     7609 2024-05-05 19:08:40.000000 seqlogic-0.0.9/src/seqlogic/design.py
--rw-rw-rw-   0        0        0     2981 2024-04-01 05:33:29.000000 seqlogic-0.0.9/src/seqlogic/hier.py
--rw-rw-rw-   0        0        0    80210 2024-05-05 19:08:40.000000 seqlogic-0.0.9/src/seqlogic/lbool.py
--rw-rw-rw-   0        0        0    13702 2024-05-05 19:08:40.000000 seqlogic-0.0.9/src/seqlogic/sim.py
--rw-rw-rw-   0        0        0     1368 2024-05-05 19:08:40.000000 seqlogic-0.0.9/src/seqlogic/util.py
-drwxrwxrwx   0        0        0        0 2024-05-05 19:09:58.479748 seqlogic-0.0.9/src/seqlogic.egg-info/
--rw-rw-rw-   0        0        0      956 2024-05-05 19:09:58.000000 seqlogic-0.0.9/src/seqlogic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      630 2024-05-05 19:09:58.000000 seqlogic-0.0.9/src/seqlogic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 19:09:58.000000 seqlogic-0.0.9/src/seqlogic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-05 19:09:58.000000 seqlogic-0.0.9/src/seqlogic.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-05 19:09:58.478746 seqlogic-0.0.9/tests/
--rw-rw-rw-   0        0        0     4281 2024-05-05 07:44:15.000000 seqlogic-0.0.9/tests/test_aes.py
--rw-rw-rw-   0        0        0    24103 2024-05-05 19:08:40.000000 seqlogic-0.0.9/tests/test_bits.py
--rw-rw-rw-   0        0        0     2583 2024-05-05 19:08:40.000000 seqlogic-0.0.9/tests/test_enum.py
--rw-rw-rw-   0        0        0     4731 2024-05-05 19:08:40.000000 seqlogic-0.0.9/tests/test_fsm.py
--rw-rw-rw-   0        0        0      684 2024-04-21 07:30:53.000000 seqlogic-0.0.9/tests/test_gray.py
--rw-rw-rw-   0        0        0      705 2024-03-11 02:48:00.000000 seqlogic-0.0.9/tests/test_hier.py
--rw-rw-rw-   0        0        0    27044 2024-05-05 19:08:40.000000 seqlogic-0.0.9/tests/test_lbool.py
--rw-rw-rw-   0        0        0     3533 2024-05-05 19:08:40.000000 seqlogic-0.0.9/tests/test_lfsr.py
--rw-rw-rw-   0        0        0    29052 2024-04-30 03:11:09.000000 seqlogic-0.0.9/tests/test_riscv.py
--rw-rw-rw-   0        0        0     4327 2024-05-05 19:08:40.000000 seqlogic-0.0.9/tests/test_sim.py
--rw-rw-rw-   0        0        0     2456 2024-05-05 19:08:40.000000 seqlogic-0.0.9/tests/test_struct.py
+drwxrwxrwx   0        0        0        0 2024-05-19 07:15:49.692863 seqlogic-0.1.0/
+-rw-rw-rw-   0        0        0      956 2024-05-19 07:15:49.690865 seqlogic-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      740 2024-03-11 04:13:25.000000 seqlogic-0.1.0/README.md
+-rw-rw-rw-   0        0        0      263 2024-05-19 07:10:09.000000 seqlogic-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-19 07:15:49.692863 seqlogic-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-19 07:15:49.623866 seqlogic-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-19 07:15:49.641862 seqlogic-0.1.0/src/seqlogic/
+-rw-rw-rw-   0        0        0      357 2024-05-05 19:08:40.000000 seqlogic-0.1.0/src/seqlogic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 07:15:49.663863 seqlogic-0.1.0/src/seqlogic/algorithms/
+-rw-rw-rw-   0        0        0       27 2023-11-27 07:28:50.000000 seqlogic-0.1.0/src/seqlogic/algorithms/__init__.py
+-rw-rw-rw-   0        0        0    12685 2024-03-10 17:38:01.000000 seqlogic-0.1.0/src/seqlogic/algorithms/aes.py
+-rw-rw-rw-   0        0        0      285 2024-04-30 03:11:09.000000 seqlogic-0.1.0/src/seqlogic/algorithms/gray.py
+-rw-rw-rw-   0        0        0    21662 2024-05-08 03:13:26.000000 seqlogic-0.1.0/src/seqlogic/bits.py
+-rw-rw-rw-   0        0        0     8227 2024-05-19 06:58:21.000000 seqlogic-0.1.0/src/seqlogic/design.py
+-rw-rw-rw-   0        0        0     2981 2024-04-01 05:33:29.000000 seqlogic-0.1.0/src/seqlogic/hier.py
+-rw-rw-rw-   0        0        0    83685 2024-05-19 01:01:33.000000 seqlogic-0.1.0/src/seqlogic/lbool.py
+-rw-rw-rw-   0        0        0    13408 2024-05-08 02:03:42.000000 seqlogic-0.1.0/src/seqlogic/sim.py
+-rw-rw-rw-   0        0        0     1368 2024-05-05 19:08:40.000000 seqlogic-0.1.0/src/seqlogic/util.py
+drwxrwxrwx   0        0        0        0 2024-05-19 07:15:49.688862 seqlogic-0.1.0/src/seqlogic.egg-info/
+-rw-rw-rw-   0        0        0      956 2024-05-19 07:15:49.000000 seqlogic-0.1.0/src/seqlogic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      630 2024-05-19 07:15:49.000000 seqlogic-0.1.0/src/seqlogic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 07:15:49.000000 seqlogic-0.1.0/src/seqlogic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-19 07:15:49.000000 seqlogic-0.1.0/src/seqlogic.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-19 07:15:49.686866 seqlogic-0.1.0/tests/
+-rw-rw-rw-   0        0        0     4281 2024-05-08 03:13:26.000000 seqlogic-0.1.0/tests/test_aes.py
+-rw-rw-rw-   0        0        0    24103 2024-05-08 03:13:26.000000 seqlogic-0.1.0/tests/test_bits.py
+-rw-rw-rw-   0        0        0     3205 2024-05-19 01:15:33.000000 seqlogic-0.1.0/tests/test_enum.py
+-rw-rw-rw-   0        0        0     4731 2024-05-05 19:08:40.000000 seqlogic-0.1.0/tests/test_fsm.py
+-rw-rw-rw-   0        0        0      684 2024-04-21 07:30:53.000000 seqlogic-0.1.0/tests/test_gray.py
+-rw-rw-rw-   0        0        0      705 2024-03-11 02:48:00.000000 seqlogic-0.1.0/tests/test_hier.py
+-rw-rw-rw-   0        0        0    30024 2024-05-19 00:05:08.000000 seqlogic-0.1.0/tests/test_lbool.py
+-rw-rw-rw-   0        0        0     3533 2024-05-05 19:08:40.000000 seqlogic-0.1.0/tests/test_lfsr.py
+-rw-rw-rw-   0        0        0    38708 2024-05-19 04:01:24.000000 seqlogic-0.1.0/tests/test_riscv.py
+-rw-rw-rw-   0        0        0     4327 2024-05-05 19:08:40.000000 seqlogic-0.1.0/tests/test_sim.py
+-rw-rw-rw-   0        0        0     3024 2024-05-12 18:46:32.000000 seqlogic-0.1.0/tests/test_struct.py
```

### Comparing `seqlogic-0.0.9/PKG-INFO` & `seqlogic-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqlogic
-Version: 0.0.9
+Version: 0.1.0
 Summary: Sequential Logic
 Project-URL: Repository, https://github.com/cjdrake/seqlogic.git
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # Sequential Logic
```

### Comparing `seqlogic-0.0.9/README.md` & `seqlogic-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `seqlogic-0.0.9/src/seqlogic/algorithms/aes.py` & `seqlogic-0.1.0/src/seqlogic/algorithms/aes.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.0.9/src/seqlogic/bits.py` & `seqlogic-0.1.0/src/seqlogic/bits.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.0.9/src/seqlogic/design.py` & `seqlogic-0.1.0/src/seqlogic/design.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from collections import defaultdict
 from collections.abc import Callable
 
 from vcd.writer import VarValue
 from vcd.writer import VCDWriter as VcdWriter
 
 from .hier import Branch, Leaf
-from .lbool import Vec, ones, zeros
+from .lbool import Vec, VecEnum, ones, zeros
 from .sim import Aggregate, Region, SimAwaitable, Singular, State, changed, get_loop
 
 _item2char = {
     0b00: "x",
     0b01: "0",
     0b10: "1",
     0b11: "x",
@@ -102,18 +102,19 @@
             assert isinstance(child, _TraceIf)
             child.dump_vcd(vcdw, pattern)
 
 
 class _TraceSingular(Leaf, _TraceIf, Singular, _ProcIf):
     """Combine hierarchy and sim semantics for singular data types."""
 
-    def __init__(self, name: str, parent: Module, value):
+    def __init__(self, name: str, parent: Module, dtype: type):
         Leaf.__init__(self, name, parent)
-        Singular.__init__(self, value)
+        Singular.__init__(self, dtype.xes())
         _ProcIf.__init__(self)
+        self._dtype = dtype
         self._waves_change = None
         self._vcd_change = None
 
     def update(self):
         if self._waves_change and self.dirty():
             self._waves_change()
         if self._vcd_change and self.dirty():
@@ -129,28 +130,35 @@
                 t = self._sim.time
                 waves[t][self] = self._next_value
 
             self._waves_change = change
 
     def dump_vcd(self, vcdw, pattern: str):
         assert isinstance(self._parent, Module)
-        if re.match(pattern, self.qualname):
-            var = vcdw.register_var(
-                scope=self._parent.scope,
-                name=self.name,
-                var_type="reg",
-                size=len(self._value),
-                init=_vec2vcd(self._value),
-            )
-
-            def change():
-                t = self._sim.time
-                vcdw.change(var, t, _vec2vcd(self._next_value))
-
-            self._vcd_change = change
+        if issubclass(self._dtype, VecEnum):
+            if re.match(pattern, self.qualname):
+                var = vcdw.register_var(
+                    scope=self._parent.scope,
+                    name=self.name,
+                    var_type="string",
+                    init=self._value.name,
+                )
+                self._vcd_change = lambda: vcdw.change(var, self._sim.time, self._next_value.name)
+        else:
+            if re.match(pattern, self.qualname):
+                var = vcdw.register_var(
+                    scope=self._parent.scope,
+                    name=self.name,
+                    var_type="reg",
+                    size=len(self._value),
+                    init=_vec2vcd(self._value),
+                )
+                self._vcd_change = lambda: vcdw.change(
+                    var, self._sim.time, _vec2vcd(self._next_value)
+                )
 
     def connect(self, src):
         """Convenience function to reduce process boilerplate."""
 
         async def proc():
             while True:
                 await changed(src)
@@ -158,52 +166,58 @@
 
         self._procs.append((Region.REACTIVE, proc, (), {}))
 
 
 class Bits(_TraceSingular):
     """Leaf-level bitvector design component."""
 
-    def __init__(self, name: str, parent: Module, dtype: type):
-        super().__init__(name, parent, value=dtype.xes())
-
 
 class Bit(Bits):
     """One-bit specialization of Bits that supports edge detection."""
 
     def __init__(self, name: str, parent: Module):
         super().__init__(name, parent, dtype=Vec[1])
 
+    def is_neg(self) -> bool:
+        """Return True when bit is stable 0 => 0."""
+        return self._value == zeros(1) and self._next_value == zeros(1)
+
     def is_posedge(self) -> bool:
-        """Return True when signal transitions from 0 to 1."""
+        """Return True when bit transitions 0 => 1."""
         return self._value == zeros(1) and self._next_value == ones(1)
 
+    def is_negedge(self) -> bool:
+        """Return True when bit transition 1 => 0."""
+        return self._value == ones(1) and self._next_value == zeros(1)
+
+    def is_pos(self) -> bool:
+        """Return True when bit is stable 1 => 1."""
+        return self._value == ones(1) and self._next_value == ones(1)
+
     async def posedge(self) -> State:
         """Suspend; resume execution at signal posedge."""
         self._sim.add_event(self, self.is_posedge)
         state = await SimAwaitable()
         return state
 
-    def is_negedge(self) -> bool:
-        """Return True when signal transitions from 1 to 0."""
-        return self._value == ones(1) and self._next_value == zeros(1)
-
     async def negedge(self) -> State:
         """Suspend; resume execution at signal negedge."""
         self._sim.add_event(self, self.is_negedge)
         state = await SimAwaitable()
         return state
 
 
 class _TraceAggregate(Leaf, _TraceIf, Aggregate, _ProcIf):
     """Combine hierarchy and sim semantics for aggregate data types."""
 
-    def __init__(self, name: str, parent: Module, value):
+    def __init__(self, name: str, parent: Module, dtype: type):
         Leaf.__init__(self, name, parent)
-        Aggregate.__init__(self, value)
+        Aggregate.__init__(self, dtype.xes())
         _ProcIf.__init__(self)
+        self._dtype = dtype
 
 
 class _ArrayXPropItem:
     """Array X-Prop item helper."""
 
     def __init__(self, dtype: type):
         self._dtype = dtype
@@ -218,24 +232,17 @@
 
     next = property(fset=_set_next)
 
 
 class Array(_TraceAggregate):
     """Leaf-level array of bitvector/enum/struct/union design components."""
 
-    def __init__(
-        self,
-        name: str,
-        parent: Module,
-        shape: tuple[int, ...],
-        dtype: type,
-    ):
+    def __init__(self, name: str, parent: Module, shape: tuple[int, ...], dtype: type):
         assert len(shape) == 1
-        super().__init__(name, parent, value=dtype.xes())
-        self._dtype = dtype
+        super().__init__(name, parent, dtype)
 
     def __getitem__(self, key: int | Vec):
         match key:
             case int():
                 return super().__getitem__(key)
             case Vec():
                 try:
```

### Comparing `seqlogic-0.0.9/src/seqlogic/hier.py` & `seqlogic-0.1.0/src/seqlogic/hier.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.0.9/src/seqlogic/lbool.py` & `seqlogic-0.1.0/src/seqlogic/lbool.py`

 * *Files 5% similar despite different names*

```diff
@@ -312,45 +312,58 @@
     * ones
     * dcs
     """
 
     def __class_getitem__(cls, n: int):
         if n < 0:
             raise ValueError(f"Expected n ≥ 0, got {n}")
-
         if (vec_n := _VecN.get(n)) is None:
             _VecN[n] = vec_n = type(f"Vec[{n}]", (Vec,), {"_n": n})
         return vec_n
 
     @classproperty
     def nbits(cls):  # pylint: disable=no-self-argument
         """Number of bits of data."""
         return _ITEM_BITS * cls._n
 
     @classmethod
+    def check_len(cls, n: int):
+        """Check for valid input length."""
+        if n != cls._n:
+            raise TypeError(f"Expected n = {cls._n}, got {n}")
+
+    @classmethod
+    def check_data(cls, data: int):
+        """Check for valid input data."""
+        a, b = 0, 1 << cls.nbits
+        if not a <= data < b:
+            raise ValueError(f"Expected data in [{a}, {b}), got {data}")
+
+    @classmethod
     def xes(cls):
-        return cls(0)
+        obj = object.__new__(cls)
+        obj._data = 0
+        return obj
 
     @classmethod
     def dcs(cls):
-        return cls((1 << cls.nbits) - 1)
+        obj = object.__new__(cls)
+        obj._data = (1 << cls.nbits) - 1
+        return obj
 
     def __init__(self, data: int):
         """Initialize.
 
         Args:
             data: lbool items packed into an int.
 
         Raises:
             ValueError if data is invalid/inconsistent
         """
-        assert hasattr(self, "_n")
-        a, b = 0, 1 << self.nbits
-        if not a <= data < b:
-            raise ValueError(f"Expected data in [{a}, {b}), got {data}")
+        self.check_data(data)
         self._data = data
 
     def __len__(self) -> int:
         return self._n
 
     def __getitem__(self, key: int | slice) -> Vec:
         match key:
@@ -460,15 +473,15 @@
 
         Returns:
             vec of equal length, data contains NOR result.
 
         Raises:
             ValueError: vec lengths do not match.
         """
-        self._check_len(other)
+        self.check_len(len(other))
 
         x0_0 = self._bit_mask[0]
         x0_01 = x0_0 << 1
         x0_1 = self._bit_mask[1]
         x0_10 = x0_1 >> 1
 
         x1_0 = other._bit_mask[0]
@@ -490,15 +503,15 @@
 
         Returns:
             vec of equal length, data contains OR result.
 
         Raises:
             ValueError: vec lengths do not match.
         """
-        self._check_len(other)
+        self.check_len(len(other))
 
         x0_0 = self._bit_mask[0]
         x0_01 = x0_0 << 1
         x0_1 = self._bit_mask[1]
 
         x1_0 = other._bit_mask[0]
         x1_01 = x1_0 << 1
@@ -529,15 +542,15 @@
 
         Returns:
             vec of equal length, data contains NAND result.
 
         Raises:
             ValueError: vec lengths do not match.
         """
-        self._check_len(other)
+        self.check_len(len(other))
 
         x0_0 = self._bit_mask[0]
         x0_01 = x0_0 << 1
         x0_1 = self._bit_mask[1]
         x0_10 = x0_1 >> 1
 
         x1_0 = other._bit_mask[0]
@@ -559,15 +572,15 @@
 
         Returns:
             vec of equal length, data contains AND result.
 
         Raises:
             ValueError: vec lengths do not match.
         """
-        self._check_len(other)
+        self.check_len(len(other))
 
         x0_0 = self._bit_mask[0]
         x0_1 = self._bit_mask[1]
         x0_10 = x0_1 >> 1
 
         x1_0 = other._bit_mask[0]
         x1_1 = other._bit_mask[1]
@@ -598,15 +611,15 @@
 
         Returns:
             vec of equal length, data contains XNOR result.
 
         Raises:
             ValueError: vec lengths do not match.
         """
-        self._check_len(other)
+        self.check_len(len(other))
 
         x0_0 = self._bit_mask[0]
         x0_01 = x0_0 << 1
         x0_1 = self._bit_mask[1]
         x0_10 = x0_1 >> 1
 
         x1_0 = other._bit_mask[0]
@@ -628,15 +641,15 @@
 
         Returns:
             vec of equal length, data contains XOR result.
 
         Raises:
             ValueError: vec lengths do not match.
         """
-        self._check_len(other)
+        self.check_len(len(other))
 
         x0_0 = self._bit_mask[0]
         x0_01 = x0_0 << 1
         x0_1 = self._bit_mask[1]
         x0_10 = x0_1 >> 1
 
         x1_0 = other._bit_mask[0]
@@ -726,150 +739,150 @@
 
         Args:
             other: vec of equal length.
 
         Returns:
             Vec[1] result of self == other
         """
-        self._check_len(other)
+        self.check_len(len(other))
         try:
             return (_Vec0, _Vec1)[self.to_uint() == other.to_uint()]
         except ValueError:
             return _VecX
 
     def neq(self, other: Vec) -> Vec[1]:
         """Not Equal operator.
 
         Args:
             other: vec of equal length.
 
         Returns:
             Vec[1] result of self != other
         """
-        self._check_len(other)
+        self.check_len(len(other))
         try:
             return (_Vec0, _Vec1)[self.to_uint() != other.to_uint()]
         except ValueError:
             return _VecX
 
     def ltu(self, other: Vec) -> Vec[1]:
         """Less than operator (unsigned).
 
         Args:
             other: vec of equal length.
 
         Returns:
             Vec[1] result of unsigned(self) < unsigned(other)
         """
-        self._check_len(other)
+        self.check_len(len(other))
         try:
             return (_Vec0, _Vec1)[self.to_uint() < other.to_uint()]
         except ValueError:
             return _VecX
 
     def lteu(self, other: Vec) -> Vec[1]:
         """Less than or equal operator (unsigned).
 
         Args:
             other: vec of equal length.
 
         Returns:
             Vec[1] result of unsigned(self) ≤ unsigned(other)
         """
-        self._check_len(other)
+        self.check_len(len(other))
         try:
             return (_Vec0, _Vec1)[self.to_uint() <= other.to_uint()]
         except ValueError:
             return _VecX
 
     def lt(self, other: Vec) -> Vec[1]:
         """Less than operator (signed).
 
         Args:
             other: vec of equal length.
 
         Returns:
             Vec[1] result of signed(self) < signed(other)
         """
-        self._check_len(other)
+        self.check_len(len(other))
         try:
             return (_Vec0, _Vec1)[self.to_int() < other.to_int()]
         except ValueError:
             return _VecX
 
     def lte(self, other: Vec) -> Vec[1]:
         """Less than or equal operator (signed).
 
         Args:
             other: vec of equal length.
 
         Returns:
             Vec[1] result of signed(self) ≤ signed(other)
         """
-        self._check_len(other)
+        self.check_len(len(other))
         try:
             return (_Vec0, _Vec1)[self.to_int() <= other.to_int()]
         except ValueError:
             return _VecX
 
     def gtu(self, other: Vec) -> Vec[1]:
         """Greater than operator (unsigned).
 
         Args:
             other: vec of equal length.
 
         Returns:
             Vec[1] result of unsigned(self) > unsigned(other)
         """
-        self._check_len(other)
+        self.check_len(len(other))
         try:
             return (_Vec0, _Vec1)[self.to_uint() > other.to_uint()]
         except ValueError:
             return _VecX
 
     def gteu(self, other: Vec) -> Vec[1]:
         """Greater than or equal operator (unsigned).
 
         Args:
             other: vec of equal length.
 
         Returns:
             Vec[1] result of unsigned(self) ≥ unsigned(other)
         """
-        self._check_len(other)
+        self.check_len(len(other))
         try:
             return (_Vec0, _Vec1)[self.to_uint() >= other.to_uint()]
         except ValueError:
             return _VecX
 
     def gt(self, other: Vec) -> Vec[1]:
         """Greater than operator (signed).
 
         Args:
             other: vec of equal length.
 
         Returns:
             Vec[1] result of signed(self) > signed(other)
         """
-        self._check_len(other)
+        self.check_len(len(other))
         try:
             return (_Vec0, _Vec1)[self.to_int() > other.to_int()]
         except ValueError:
             return _VecX
 
     def gte(self, other: Vec) -> Vec[1]:
         """Greater than or equal operator (signed).
 
         Args:
             other: vec of equal length.
 
         Returns:
             Vec[1] result of signed(self) ≥ signed(other)
         """
-        self._check_len(other)
+        self.check_len(len(other))
         try:
             return (_Vec0, _Vec1)[self.to_int() >= other.to_int()]
         except ValueError:
             return _VecX
 
     def match(self, pattern: str | Vec) -> Vec[1]:
         """Pattern match operator."""
@@ -877,15 +890,15 @@
             case str() as lit:
                 pattern = lit2vec(lit)
             case Vec():
                 pass
             case _:
                 raise TypeError("Expected pattern to be str or Vec")
 
-        self._check_len(pattern)
+        self.check_len(len(pattern))
 
         # Propagate X
         if self.has_x() or pattern.has_x():
             return _VecX
 
         for i in range(self._n):
             a = self._get_item(i)
@@ -1049,15 +1062,15 @@
 
         Returns:
             3-tuple of (sum, carry-out, overflow).
 
         Raises:
             ValueError: vec lengths are invalid/inconsistent.
         """
-        self._check_len(other)
+        self.check_len(len(other))
 
         # Rename for readability
         n, a, b = self._n, self, other
 
         if a.has_x() or b.has_x() or ci.has_x():
             return Vec[n](_fill(_X, n)), _VecX
         if a.has_dc() or b.has_dc() or ci.has_dc():
@@ -1107,18 +1120,14 @@
         if v0 is None:
             v0 = dcs(v1._n)
         else:
             if v1._n != v0._n:
                 raise ValueError("Expected matching operand lengths")
         return v1 if self else v0
 
-    def _check_len(self, other: Vec):
-        if self._n != other._n:
-            raise ValueError(f"Expected n = {self._n}, got {other._n}")
-
     def _count(self, byte_cnt: dict[int, int], item: int) -> int:
         y = 0
         n, data = self._n, self._data
 
         stride = 4
         while n >= stride:
             y += byte_cnt[data & _BYTE_MASK]
@@ -1312,47 +1321,48 @@
     n, data = 0, 0
     for x in xs:
         data |= _from_bit[x] << (_ITEM_BITS * n)
         n += 1
     return Vec[n](data)
 
 
-_NUM_RE = re.compile(
-    r"((?P<BinSize>[0-9]+)b(?P<BinDigits>[X01\-_]+))|"
-    r"((?P<HexSize>[0-9]+)h(?P<HexDigits>[0-9a-fA-F_]+))"
+_LIT_RE = re.compile(
+    r"((?P<BinSize>[1-9][0-9]*)b(?P<BinDigits>[X01\-_]+))|"
+    r"((?P<HexSize>[1-9][0-9]*)h(?P<HexDigits>[0-9a-fA-F_]+))"
 )
 
 
 def _lit2vec(lit: str) -> tuple[int, int]:
-    if m := _NUM_RE.match(lit):
+    if m := _LIT_RE.fullmatch(lit):
         # Binary
         if m.group("BinSize"):
-            size = int(m.group("BinSize"))
+            n = int(m.group("BinSize"))
             digits = m.group("BinDigits").replace("_", "")
-            ndigits = len(digits)
-            if ndigits != size:
-                s = f"Expected {size} digits, got {ndigits}"
+            if len(digits) != n:
+                s = f"Expected {n} digits, got {len(digits)}"
                 raise ValueError(s)
-            n, data = 0, 0
-            for c in reversed(digits):
-                data |= _from_char[c] << (n * _ITEM_BITS)
-                n += 1
+            data = 0
+            for i, c in enumerate(reversed(digits)):
+                data |= _from_char[c] << (i * _ITEM_BITS)
             return n, data
         # Hexadecimal
         elif m.group("HexSize"):
-            size = int(m.group("HexSize"))
+            n = int(m.group("HexSize"))
             digits = m.group("HexDigits").replace("_", "")
-            ndigits = len(digits)
-            if 4 * ndigits != size:
-                s = f"Expected size to match # digits, got {size} ≠ {4 * ndigits}"
+            exp = (n + 3) // 4
+            if len(digits) != exp:
+                s = f"Expected {exp} digits, got {len(digits)}"
                 raise ValueError(s)
-            n, data = 0, 0
-            for c in reversed(digits):
-                data |= _from_hexchar[c] << (n * _ITEM_BITS)
-                n += 4
+            data = 0
+            for i, c in enumerate(reversed(digits)):
+                try:
+                    x = _from_hexchar[min(n - 4 * i, 4)][c]
+                except KeyError as e:
+                    raise ValueError(f"Character overflows size: {c}") from e
+                data |= x << (4 * i * _ITEM_BITS)
             return n, data
         else:  # pragma: no cover
             assert False
     else:
         raise ValueError(f"Expected str literal, got {lit}")
 
 
@@ -1450,36 +1460,32 @@
 
 def rep(obj: int | str | Vec, n: int) -> Vec:
     """Repeat a vector n times."""
     objs = [obj] * n
     return cat(*objs)
 
 
-def _consts(x: int, n: int) -> Vec:
-    return Vec[n](_fill(x, n))
-
-
 def xes(n: int) -> Vec:
     """Return a vec packed with n X items."""
     return Vec[n](0)
 
 
 def zeros(n: int) -> Vec:
     """Return a vec packed with n 0 items."""
-    return _consts(_0, n)
+    return Vec[n](_fill(_0, n))
 
 
 def ones(n: int) -> Vec:
     """Return a vec packed with n 1 items."""
-    return _consts(_1, n)
+    return Vec[n](_fill(_1, n))
 
 
 def dcs(n: int) -> Vec:
     """Return a vec packed with n DC items."""
-    return _consts(_W, n)
+    return Vec[n](_fill(_W, n))
 
 
 # Empty
 _VecE = Vec[0](0)
 
 # One bit values
 _VecX = Vec[1](_X)
@@ -1492,212 +1498,275 @@
     """Enum Metaclass: Create enum base classes."""
 
     def __new__(mcs, name, bases, attrs):
         # Base case for API
         if name == "VecEnum":
             return super().__new__(mcs, name, bases, attrs)
 
-        base_attrs = {}
-        # ident = literal
-        lit2name: dict[str, str] = {}
+        enum_attrs = {}
         data2name: dict[int, str] = {}
         n = None
         dc_data = None
         for key, val in attrs.items():
             if key.startswith("__"):
-                base_attrs[key] = val
+                enum_attrs[key] = val
+            # NAME = lit
             else:
                 if n is None:
                     n, data = _lit2vec(val)
                     dc_data = (1 << _ITEM_BITS * n) - 1
                 else:
                     n_i, data = _lit2vec(val)
                     if n_i != n:
                         raise ValueError(f"Expected lit len {n}, got {n_i}")
                 if key in ("X", "DC"):
                     raise ValueError(f"Cannot use reserved name = '{key}'")
                 if data in (0, dc_data):
                     raise ValueError(f"Cannot use reserved data = {data}")
-                lit2name[val] = key
+                if data in data2name:
+                    raise ValueError(f"Duplicate data: {val}")
                 data2name[data] = key
 
         # Empty Enum
         if n is None:
-            # Create class
-            super_cls = Vec[0]
-            cls = super().__new__(mcs, name, bases + (super_cls,), base_attrs)
-            # Instantiate member
-            obj = object.__new__(cls)  # pyright: ignore[reportArgumentType]
-            super_cls.__init__(obj, 0)
-            # Define methods
-            cls.__new__ = lambda c: obj
-            cls.__init__ = lambda s: None
-            cls.name = property(fget=lambda self: "")
-
-            return cls
-
-        # Add X member
-        x_lit = f"{n}b" + "X" * n
-        lit2name[x_lit] = "X"
-        data2name[0] = "X"
+            raise ValueError("Empty Enum is not supported")
 
-        # Add DC member
-        dc_lit = f"{n}b" + "-" * n
-        lit2name[dc_lit] = "DC"
+        # Help the type checker
         assert dc_data is not None
-        data2name[dc_data] = "DC"
 
-        def _new(cls, arg: str | int):
-            match arg:
-                case str() as lit:
-                    try:
-                        name = lit2name[lit]
-                    except KeyError as e:
-                        raise ValueError(f"Invalid lit: {lit}") from e
-                case int() as data:
-                    try:
-                        name = data2name[data]
-                    except KeyError as e:
-                        raise ValueError(f"Invalid data: {data}") from e
-                case _:
-                    raise TypeError("Expected arg to be str or int")
-            return getattr(cls, name)
+        # Add X/DC members
+        data2name[0] = "X"
+        data2name[dc_data] = "DC"
 
-        # Create class
-        super_cls = Vec[n]
-        cls = super().__new__(mcs, name, bases + (super_cls,), base_attrs)
+        # Create Enum class
+        enum = super().__new__(mcs, name, bases + (Vec[n],), enum_attrs)
 
         # Instantiate members
         for data, name in data2name.items():
-            obj = object.__new__(cls)  # pyright: ignore[reportArgumentType]
-            super_cls.__init__(obj, data)
+            obj = object.__new__(enum)  # pyright: ignore[reportArgumentType]
+            obj._data = data
             obj._name = name
-            setattr(cls, name, obj)
+            setattr(enum, name, obj)
+
+        # Override Vec __new__ method
+        def _new(cls, arg: str | int | Vec):
+            match arg:
+                case str() as lit:
+                    n, data = _lit2vec(lit)
+                    cls.check_len(n)
+                case int() as data:
+                    cls.check_data(data)
+                case Vec() as v:
+                    n, data = len(v), v.data
+                    cls.check_len(n)
+                case _:
+                    raise TypeError("Expected arg to be str, int, or Vec")
+            try:
+                obj = getattr(cls, data2name[data])
+            except KeyError:
+                obj = object.__new__(enum)  # pyright: ignore[reportArgumentType]
+                obj._data = data
+                obj._name = f"{cls.__name__}({Vec[cls._n].__str__(obj)})"
+            return obj
+
+        enum.__new__ = _new
+
+        # Override Vec __init__ method (to do nothing)
+        enum.__init__ = lambda self, arg: None
+
+        # Override Vec xes/dcs methods
+        enum.xes = classmethod(lambda cls: getattr(cls, "X"))
+        enum.dcs = classmethod(lambda cls: getattr(cls, "DC"))
 
-        # Define methods
-        cls.__new__ = _new
-        cls.__init__ = lambda s, lit: None
-        cls.name = property(fget=lambda self: self._name)
+        # Create name property
+        enum.name = property(fget=lambda self: self._name)
 
-        return cls
+        return enum
 
 
 class VecEnum(metaclass=_VecEnumMeta):
     """Enum Base Class: Create enums."""
 
 
-def _vec_struct_init(fields: list[tuple[str, type]]) -> str:
-    """Return code for a Struct __init__ method w/ fields."""
+def _struct_init_source(fields: list[tuple[str, type]]) -> str:
+    """Return source code for Struct __init__ method w/ fields."""
     lines = []
-    line = "def init(self"
-    for field_name, field_type in fields:
-        line += f", {field_name}: {field_type.__name__} | None = None"
-    line += "):\n"
-    lines.append(line)
-    lines.append("    _n = 0\n")
-    lines.append("    _data = 0\n")
-    for field_name, field_type in fields:
-        offset = f"({_ITEM_BITS} * self._{field_name}_base)"
-        lines.append(f"    self._{field_name}_base = _n\n")
-        lines.append(f"    self._{field_name}_size = {field_type._n}\n")
-        lines.append(f"    _n += self._{field_name}_size\n")
-        lines.append(f"    if {field_name} is not None:\n")
-        lines.append(f"        _data |= {field_name}.data << {offset}\n")
-    lines.append("    self._data = _data\n")
+    s = ", ".join(f"{fn}: {ft.__name__} | None = None" for fn, ft in fields)
+    lines.append(f"def struct_init(self, {s}):\n")
+    lines.append("    data = 0\n")
+    for fn, _ in fields:
+        s = f"Expected field {fn} to have {{exp}} bits, got {{got}}"
+        lines.append(f"    if {fn} is not None:\n")
+        lines.append(f"        got, exp = len({fn}), self._{fn}_size\n")
+        lines.append("        if got != exp:\n")
+        lines.append(f'            raise TypeError(f"{s}")\n')
+        lines.append(f"        data |= {fn}.data << ({_ITEM_BITS} * self._{fn}_base)\n")
+    lines.append("    self._data = data\n")
     return "".join(lines)
 
 
 class _VecStructMeta(type):
     """Struct Metaclass: Create struct base classes."""
 
     def __new__(mcs, name, bases, attrs):
         # Base case for API
         if name == "VecStruct":
             return super().__new__(mcs, name, bases, attrs)
 
         # Scan attributes for field_name: field_type items
-        base_attrs = {}
-        # ident: vec_type
+        struct_attrs = {}
         fields: list[tuple[str, type]] = []
         for key, val in attrs.items():
             if key == "__annotations__":
                 for field_name, field_type in val.items():
                     fields.append((field_name, field_type))
+            # name: Type
             else:
-                base_attrs[key] = val
+                struct_attrs[key] = val
+
+        # Add struct member base/size attributes
+        base = 0
+        for field_name, field_type in fields:
+            struct_attrs[f"_{field_name}_base"] = base
+            struct_attrs[f"_{field_name}_size"] = field_type._n
+            base += field_type._n
 
         # Create Struct class
         n = sum(field_type._n for _, field_type in fields)
-        super_cls = Vec[n]
-        cls = super().__new__(mcs, name, bases + (super_cls,), base_attrs)
-
-        # Create Struct.__init__
-        code = _vec_struct_init(fields)
-        d = {}
-        exec(code, None, d)  # pylint: disable=exec-used
-        cls.__init__ = d["init"]
-
-        # Override Struct.xes and Struct.dcs methods
-        def _xes():
-            return cls()
-
-        def _dcs():
-            kwargs = {fn: ft.dcs() for fn, ft in fields}
-            return cls(**kwargs)  # pyright: ignore[reportCallIssue]
+        struct = super().__new__(mcs, name, bases + (Vec[n],), struct_attrs)
 
-        cls.xes = _xes
-        cls.dcs = _dcs
+        # Override Vec __init__ method
+        source = _struct_init_source(fields)
+        globals_ = {"Vec": Vec}
+        globals_.update({ft.__name__: ft for _, ft in fields})
+        locals_ = {}
+        exec(source, globals_, locals_)  # pylint: disable=exec-used
+        struct.__init__ = locals_["struct_init"]
 
-        # Create Struct.__str__
+        # Override Vec __str__ method
         def _str(self):
             args = []
             for fn, ft in fields:
                 v = getattr(self, fn)
                 if issubclass(ft, VecEnum):
                     arg = f"{fn}={ft.__name__}.{v.name}"
                 else:
                     arg = f"{fn}={v!s}"
                 args.append(arg)
             return f'{name}({", ".join(args)})'
 
-        cls.__str__ = _str
+        struct.__str__ = _str
 
-        # Create Struct.__repr__
+        # Override Vec __repr__ method
         def _repr(self):
             args = []
             for fn, ft in fields:
                 v = getattr(self, fn)
                 if issubclass(ft, VecEnum):
                     arg = f"{fn}={ft.__name__}.{v.name}"
                 else:
                     arg = f"{fn}={v!r}"
                 args.append(arg)
             return f'{name}({", ".join(args)})'
 
-        cls.__repr__ = _repr
+        struct.__repr__ = _repr
 
         # Create Struct fields
         def _fget(name, cls, self):
-            n = getattr(self, f"_{name}_size")
-            nbits = _ITEM_BITS * n
+            nbits = _ITEM_BITS * getattr(self, f"_{name}_size")
+            offset = _ITEM_BITS * getattr(self, f"_{name}_base")
             mask = (1 << nbits) - 1
-            i = getattr(self, f"_{name}_base")
-            data = (self._data >> (_ITEM_BITS * i)) & mask
+            data = (self._data >> offset) & mask
+            if issubclass(cls, (VecStruct, VecUnion)):
+                obj = object.__new__(cls)
+                obj._data = data
+                return obj
+            # Vec, VecEnum
             return cls(data)
 
         for fn, ft in fields:
-            setattr(cls, fn, property(fget=partial(_fget, fn, ft)))
+            setattr(struct, fn, property(fget=partial(_fget, fn, ft)))
 
-        return cls
+        return struct
 
 
 class VecStruct(metaclass=_VecStructMeta):
     """Struct Base Class: Create struct."""
 
 
+def _union_init_source(n: int, fields: list[tuple[str, type]]) -> str:
+    """Return source code for Union __init__ method w/ fields."""
+    lines = []
+    s1 = " | ".join(ft.__name__ for _, ft in fields)
+    s2 = "Expected input to have at most {{exp}} bits, got {{got}}"
+    lines.append(f"def union_init(self, v: {s1}):\n")
+    lines.append(f"    got, exp = len(v), {n}\n")
+    lines.append("    if got > exp:\n")
+    lines.append(f'        raise TypeError("{s2}")\n')
+    lines.append("    self._data = v.data\n")
+    return "".join(lines)
+
+
+class _VecUnionMeta(type):
+    """Union Metaclass: Create union base classes."""
+
+    def __new__(mcs, name, bases, attrs):
+        # Base case for API
+        if name == "VecUnion":
+            return super().__new__(mcs, name, bases, attrs)
+
+        # Scan attributes for field_name: field_type items
+        union_attrs = {}
+        fields: list[tuple[str, type]] = []
+        for key, val in attrs.items():
+            if key == "__annotations__":
+                for field_name, field_type in val.items():
+                    fields.append((field_name, field_type))
+            # name: Type
+            else:
+                union_attrs[key] = val
+
+        # Add union member base/size attributes
+        for field_name, field_type in fields:
+            union_attrs[f"_{field_name}_size"] = field_type._n
+
+        # Create Union class
+        n = max(field_type._n for _, field_type in fields)
+        union = super().__new__(mcs, name, bases + (Vec[n],), union_attrs)
+
+        # Override Vec __init__ method
+        source = _union_init_source(n, fields)
+        globals_ = {"Vec": Vec}
+        globals_.update({ft.__name__: ft for _, ft in fields})
+        locals_ = {}
+        exec(source, globals_, locals_)  # pylint: disable=exec-used
+        union.__init__ = locals_["union_init"]
+
+        # Create Union fields
+        def _fget(name, cls, self):
+            nbits = _ITEM_BITS * getattr(self, f"_{name}_size")
+            mask = (1 << nbits) - 1
+            data = self._data & mask
+            if issubclass(cls, (VecStruct, VecUnion)):
+                obj = object.__new__(cls)
+                obj._data = data
+                return obj
+            # Vec, VecEnum
+            return cls(data)
+
+        for fn, ft in fields:
+            setattr(union, fn, property(fget=partial(_fget, fn, ft)))
+
+        return union
+
+
+class VecUnion(metaclass=_VecUnionMeta):
+    """Union Base Class: Create union."""
+
+
 _from_bit = (_0, _1)
 
 _from_char = {
     "X": _X,
     "0": _0,
     "1": _1,
     "-": _W,
@@ -1707,36 +1776,58 @@
     _X: "X",
     _0: "0",
     _1: "1",
     _W: "-",
 }
 
 _from_hexchar = {
-    "0": 0b01_01_01_01,
-    "1": 0b01_01_01_10,
-    "2": 0b01_01_10_01,
-    "3": 0b01_01_10_10,
-    "4": 0b01_10_01_01,
-    "5": 0b01_10_01_10,
-    "6": 0b01_10_10_01,
-    "7": 0b01_10_10_10,
-    "8": 0b10_01_01_01,
-    "9": 0b10_01_01_10,
-    "a": 0b10_01_10_01,
-    "A": 0b10_01_10_01,
-    "b": 0b10_01_10_10,
-    "B": 0b10_01_10_10,
-    "c": 0b10_10_01_01,
-    "C": 0b10_10_01_01,
-    "d": 0b10_10_01_10,
-    "D": 0b10_10_01_10,
-    "e": 0b10_10_10_01,
-    "E": 0b10_10_10_01,
-    "f": 0b10_10_10_10,
-    "F": 0b10_10_10_10,
+    1: {
+        "0": 0b01,
+        "1": 0b10,
+    },
+    2: {
+        "0": 0b01_01,
+        "1": 0b01_10,
+        "2": 0b10_01,
+        "3": 0b10_10,
+    },
+    3: {
+        "0": 0b01_01_01,
+        "1": 0b01_01_10,
+        "2": 0b01_10_01,
+        "3": 0b01_10_10,
+        "4": 0b10_01_01,
+        "5": 0b10_01_10,
+        "6": 0b10_10_01,
+        "7": 0b10_10_10,
+    },
+    4: {
+        "0": 0b01_01_01_01,
+        "1": 0b01_01_01_10,
+        "2": 0b01_01_10_01,
+        "3": 0b01_01_10_10,
+        "4": 0b01_10_01_01,
+        "5": 0b01_10_01_10,
+        "6": 0b01_10_10_01,
+        "7": 0b01_10_10_10,
+        "8": 0b10_01_01_01,
+        "9": 0b10_01_01_10,
+        "a": 0b10_01_10_01,
+        "A": 0b10_01_10_01,
+        "b": 0b10_01_10_10,
+        "B": 0b10_01_10_10,
+        "c": 0b10_10_01_01,
+        "C": 0b10_10_01_01,
+        "d": 0b10_10_01_10,
+        "D": 0b10_10_01_10,
+        "e": 0b10_10_10_01,
+        "E": 0b10_10_10_01,
+        "f": 0b10_10_10_10,
+        "F": 0b10_10_10_10,
+    },
 }
 
 _byte_cnt_xes = {
     0b00_00_00_00: 4,
     0b00_00_00_01: 3,
     0b00_00_00_10: 3,
     0b00_00_00_11: 3,
```

### Comparing `seqlogic-0.0.9/src/seqlogic/sim.py` & `seqlogic-0.1.0/src/seqlogic/sim.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,21 +45,17 @@
     def __init__(self, value):
         super().__init__()
         self._value = value
         self._next_value = value
         self._changed = False
 
     def get_value(self):
-        if self._sim.region is None:
-            return self._value
         if self._sim.region == Region.REACTIVE:
             return self._next_value
-        if self._sim.region == Region.ACTIVE:
-            return self._value
-        assert False
+        return self._value
 
     value = property(fget=get_value)
 
     def set_next(self, value):
         self._changed = value != self._next_value
         self._next_value = value
 
@@ -88,21 +84,17 @@
         self._next_values = defaultdict(lambda: value)
         self._changed = set()
 
     def __getitem__(self, key: int):
         return _AggrItem(self, key)
 
     def get_value(self, index: int):
-        if self._sim.region is None:
-            return self._values[index]
         if self._sim.region == Region.REACTIVE:
             return self._next_values[index]
-        if self._sim.region == Region.ACTIVE:
-            return self._values[index]
-        assert False
+        return self._values[index]
 
     def set_next(self, index: int, value):
         if value != self._next_values[index]:
             self._changed.add(index)
         self._next_values[index] = value
 
         # Notify the event loop
```

### Comparing `seqlogic-0.0.9/src/seqlogic/util.py` & `seqlogic-0.1.0/src/seqlogic/util.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.0.9/src/seqlogic.egg-info/PKG-INFO` & `seqlogic-0.1.0/src/seqlogic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqlogic
-Version: 0.0.9
+Version: 0.1.0
 Summary: Sequential Logic
 Project-URL: Repository, https://github.com/cjdrake/seqlogic.git
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # Sequential Logic
```

### Comparing `seqlogic-0.0.9/src/seqlogic.egg-info/SOURCES.txt` & `seqlogic-0.1.0/src/seqlogic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seqlogic-0.0.9/tests/test_aes.py` & `seqlogic-0.1.0/tests/test_aes.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.0.9/tests/test_bits.py` & `seqlogic-0.1.0/tests/test_bits.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.0.9/tests/test_enum.py` & `seqlogic-0.1.0/tests/test_enum.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,79 +1,85 @@
 """Test seqlogic.lbool.VecEnum."""
 
-# pyright: reportArgumentType=false
-# pyright: reportAttributeAccessIssue=false
-# pyright: reportCallIssue=false
+# pylint: disable = unused-variable
+
+# pyright: reportArgumentType = false
+# pyright: reportAttributeAccessIssue = false
+# pyright: reportCallIssue = false
 
 import pytest
 
-from seqlogic.lbool import VecEnum, ones, zeros
+from seqlogic.lbool import Vec, VecEnum, ones, zeros
 
 
 class Color(VecEnum):
     """Boilerplate bit array enum."""
 
     RED = "2b00"
     GREEN = "2b01"
     BLUE = "2b10"
 
 
 def test_empty():
-    class Empty(VecEnum):
-        pass
+    with pytest.raises(ValueError):
 
-    e = Empty()
-    assert len(e) == 0
-    assert e.name == ""
-    assert e.data == 0
-    assert str(e) == ""
-    assert Empty() is e
+        class Empty(VecEnum):
+            pass
 
 
 def test_basic():
     assert len(Color.RED) == 2
     assert Color.RED.name == "RED"
     assert Color.RED.data == 0b0101
     assert str(Color.RED) == "2b00"
     assert Color("2b00") is Color.RED
+    assert Color("2b0_0") is Color.RED
+    assert Color(0b0101) is Color.RED
+    assert Color(Vec[2](0b0101)) is Color.RED
 
     assert len(Color.GREEN) == 2
     assert Color.GREEN.name == "GREEN"
     assert Color.GREEN.data == 0b0110
     assert str(Color.GREEN) == "2b01"
     assert Color("2b01") is Color.GREEN
+    assert Color("2b0_1") is Color.GREEN
+    assert Color(0b0110) is Color.GREEN
+    assert Color(Vec[2](0b0110)) is Color.GREEN
 
     assert len(Color.BLUE) == 2
     assert Color.BLUE.name == "BLUE"
     assert Color.BLUE.data == 0b1001
     assert str(Color.BLUE) == "2b10"
     assert Color("2b10") is Color.BLUE
+    assert Color("2b1_0") is Color.BLUE
     assert Color(0b1001) is Color.BLUE
+    assert Color(Vec[2](0b1001)) is Color.BLUE
 
     assert len(Color.X) == 2
     assert Color.X.name == "X"
     assert Color.X.data == 0
     assert str(Color.X) == "2bXX"
     assert Color("2bXX") is Color.X
-
+    assert Color(0b0000) is Color.X
     assert Color.xes() is Color.X
+    assert Color(Vec[2](0b0000)) is Color.X
 
     assert len(Color.DC) == 2
     assert Color.DC.name == "DC"
     assert Color.DC.data == 0b1111
     assert str(Color.DC) == "2b--"
     assert Color("2b--") is Color.DC
     assert Color(0b1111) is Color.DC
-
     assert Color.dcs() is Color.DC
+    assert Color(Vec[2](0b1111)) is Color.DC
+
+    assert str(Color("2b11").name) == "Color(2b11)"
+    assert str(Color(0b1010).name) == "Color(2b11)"
+    assert str(Color(Vec[2](0b1010)).name) == "Color(2b11)"
 
-    with pytest.raises(ValueError):
-        _ = Color("2b11")
-    with pytest.raises(ValueError):
-        _ = Color(0b1010)
     with pytest.raises(TypeError):
         _ = Color(1.23e4)
 
 
 def test_slicing():
     assert Color.GREEN[0] == ones(1)
     assert Color.GREEN[1] == zeros(1)
@@ -106,7 +112,14 @@
     with pytest.raises(ValueError):
 
         class InvalidMembers(VecEnum):
             A = "2b00"
             B = "3b000"
 
         _ = InvalidMembers()
+
+    with pytest.raises(ValueError):
+
+        class DuplicateMembers(VecEnum):
+            A = "2b00"
+            B = "2b01"
+            C = "2b00"
```

### Comparing `seqlogic-0.0.9/tests/test_fsm.py` & `seqlogic-0.1.0/tests/test_fsm.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.0.9/tests/test_gray.py` & `seqlogic-0.1.0/tests/test_gray.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.0.9/tests/test_hier.py` & `seqlogic-0.1.0/tests/test_hier.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.0.9/tests/test_lbool.py` & `seqlogic-0.1.0/tests/test_lbool.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,41 +22,44 @@
     vec,
     xes,
     xnor,
     xor,
 )
 
 E = Vec[0](0)
-F = vec(False)
-T = vec(True)
-X = vec("1bX")
-
-
-LNOT = {
-    "X": "X",
-    "0": "1",
-    "1": "0",
-    "-": "-",
-}
+X = Vec[1](0b00)
+F = Vec[1](0b01)
+T = Vec[1](0b10)
+W = Vec[1](0b11)
 
 
 def test_vec():
-    assert vec() == Vec[0](0)
-    assert vec(None) == Vec[0](0)
-    assert vec(False) == Vec[1](0b01)
-    assert vec(True) == Vec[1](0b10)
-    assert vec(0) == Vec[1](0b01)
-    assert vec(1) == Vec[1](0b10)
+    # None/Empty
+    assert vec() == vec(None) == vec([]) == E
+    # Single bool input
+    assert vec(False) == vec(0) == F
+    assert vec(True) == vec(1) == T
+    # Sequence of bools
     assert vec([False, True, 0, 1]) == Vec[4](0b10_01_10_01)
+    # String
+    assert vec("4b-10X") == Vec[4](0b11_10_01_00)
 
     # Invalid input type
     with pytest.raises(TypeError):
         vec({"key": "val"})
 
 
+LNOT = {
+    "X": "X",
+    "0": "1",
+    "1": "0",
+    "-": "-",
+}
+
+
 def test_lnot():
     for x, y in LNOT.items():
         x = lbool._from_char[x]
         y = lbool._from_char[y]
         assert not_(x) == y
 
 
@@ -352,15 +355,15 @@
 def test_vec_lxor():
     x0 = Vec[16](0b11111111_10101010_01010101_00000000)
     x1 = Vec[16](0b11100100_11100100_11100100_11100100)
     assert x0.xor(x1) == Vec[16](0b11111100_11011000_11100100_00000000)
     assert (x0 ^ x1) == Vec[16](0b11111100_11011000_11100100_00000000)
 
     # Vector length mismatch
-    with pytest.raises(ValueError):
+    with pytest.raises(TypeError):
         x0.xor(Vec[8](0b11111111_00000000))
 
 
 UOR = {
     0b00_00: 0b00,
     0b01_00: 0b00,
     0b10_00: 0b00,
@@ -1024,36 +1027,139 @@
         int2vec(2, 2)
     with pytest.raises(ValueError):
         int2vec(3, 2)
     with pytest.raises(ValueError):
         int2vec(4, 3)
 
 
-def test_lit2vec():
-    # literal doesn't match size
+LIT2VEC_BIN = {
+    "1b0": (1, 0b01),
+    "1b1": (1, 0b10),
+    "2b00": (2, 0b01_01),
+    "2b01": (2, 0b01_10),
+    "2b10": (2, 0b10_01),
+    "2b11": (2, 0b10_10),
+    "3b100": (3, 0b10_01_01),
+    "3b101": (3, 0b10_01_10),
+    "3b110": (3, 0b10_10_01),
+    "3b111": (3, 0b10_10_10),
+    "4b1000": (4, 0b10_01_01_01),
+    "4b1001": (4, 0b10_01_01_10),
+    "4b1010": (4, 0b10_01_10_01),
+    "4b1011": (4, 0b10_01_10_10),
+    "4b1100": (4, 0b10_10_01_01),
+    "4b1101": (4, 0b10_10_01_10),
+    "4b1110": (4, 0b10_10_10_01),
+    "4b1111": (4, 0b10_10_10_10),
+    "5b1_0000": (5, 0b10_01_01_01_01),
+    "5b1_1111": (5, 0b10_10_10_10_10),
+    "6b10_0000": (6, 0b10_01_01_01_01_01),
+    "6b11_1111": (6, 0b10_10_10_10_10_10),
+    "7b100_0000": (7, 0b10_01_01_01_01_01_01),
+    "7b111_1111": (7, 0b10_10_10_10_10_10_10),
+    "8b1000_0000": (8, 0b10_01_01_01_01_01_01_01),
+    "8b1111_1111": (8, 0b10_10_10_10_10_10_10_10),
+    "9b1_0000_0000": (9, 0b10_01_01_01_01_01_01_01_01),
+    "9b1_1111_1111": (9, 0b10_10_10_10_10_10_10_10_10),
+}
+
+
+def test_lit2vec_bin():
+    # Valid inputs
+    for lit, (n, data) in LIT2VEC_BIN.items():
+        v = vec(lit)
+        assert len(v) == n and v.data == data
+
+    v = vec("4b-1_0X")
+    assert len(v) == 4 and v.data == 0b11_10_01_00
+    v = vec("4bX01-")
+    assert len(v) == 4 and v.data == 0b00_01_10_11
+
+    # Not a literal
     with pytest.raises(ValueError):
-        vec("4b1010_1010")
+        vec("invalid")
+
+    # Size cannot be zero
+    with pytest.raises(ValueError):
+        vec("0b0")
+    # Contains illegal characters
+    with pytest.raises(ValueError):
+        vec("4b1XW0")
+
+    # Size is too big
     with pytest.raises(ValueError):
         vec("8b1010")
+
+    # Size is too small
+    with pytest.raises(ValueError):
+        vec("4b1010_1010")
+
+
+LIT2VEC_HEX = {
+    "1h0": (1, 0b01),
+    "1h1": (1, 0b10),
+    "2h0": (2, 0b01_01),
+    "2h1": (2, 0b01_10),
+    "2h2": (2, 0b10_01),
+    "2h3": (2, 0b10_10),
+    "3h4": (3, 0b10_01_01),
+    "3h5": (3, 0b10_01_10),
+    "3h6": (3, 0b10_10_01),
+    "3h7": (3, 0b10_10_10),
+    "4h8": (4, 0b10_01_01_01),
+    "4h9": (4, 0b10_01_01_10),
+    "4hA": (4, 0b10_01_10_01),
+    "4hB": (4, 0b10_01_10_10),
+    "4hC": (4, 0b10_10_01_01),
+    "4hD": (4, 0b10_10_01_10),
+    "4hE": (4, 0b10_10_10_01),
+    "4hF": (4, 0b10_10_10_10),
+    "5h10": (5, 0b10_01_01_01_01),
+    "5h1F": (5, 0b10_10_10_10_10),
+    "6h20": (6, 0b10_01_01_01_01_01),
+    "6h3F": (6, 0b10_10_10_10_10_10),
+    "7h40": (7, 0b10_01_01_01_01_01_01),
+    "7h7F": (7, 0b10_10_10_10_10_10_10),
+    "8h80": (8, 0b10_01_01_01_01_01_01_01),
+    "8hFF": (8, 0b10_10_10_10_10_10_10_10),
+    "9h100": (9, 0b10_01_01_01_01_01_01_01_01),
+    "9h1FF": (9, 0b10_10_10_10_10_10_10_10_10),
+}
+
+
+def test_lit2vec_hex():
+    # Valid inputs
+    for lit, (n, data) in LIT2VEC_HEX.items():
+        v = vec(lit)
+        assert len(v) == n and v.data == data
+
+    # Not a literal
+    with pytest.raises(ValueError):
+        vec("invalid")
+
+    # Size cannot be zero
+    with pytest.raises(ValueError):
+        vec("0h0")
+    # Contains illegal characters
+    with pytest.raises(ValueError):
+        vec("8hd3@d_b33f")
+
+    # Size is too big
     with pytest.raises(ValueError):
         vec("16hdead_beef")
+
+    # Size is too small
     with pytest.raises(ValueError):
         vec("8hdead")
 
-    # Invalid input
+    # Invalid characters
     with pytest.raises(ValueError):
-        vec("invalid")
-
-    # Valid input
-    v = vec("4b-1_0X")
-    assert v.data == 0b11_10_01_00
-    v = vec("64hFeDc_Ba98_7654_3210")
-    assert v.data == 0xAAA9_A6A5_9A99_9695_6A69_6665_5A59_5655
-    v = vec("64hfEdC_bA98_7654_3210")
-    assert v.data == 0xAAA9_A6A5_9A99_9695_6A69_6665_5A59_5655
+        vec("3h8")  # Only 0..7 is legal
+    with pytest.raises(ValueError):
+        vec("5h20")  # Only 0..1F is legal
 
 
 def test_vec_basic():
     # n is non-negative
     with pytest.raises(ValueError):
         Vec[-1](42)
```

### Comparing `seqlogic-0.0.9/tests/test_lfsr.py` & `seqlogic-0.1.0/tests/test_lfsr.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.0.9/tests/test_sim.py` & `seqlogic-0.1.0/tests/test_sim.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.0.9/tests/test_struct.py` & `seqlogic-0.1.0/tests/test_struct.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Test seqlogic.lbool.VecStruct."""
 
 # PyRight is confused by MetaClass behavior
 # pyright: reportArgumentType=false
 # pyright: reportAttributeAccessIssue=false
 # pyright: reportCallIssue=false
 
+import pytest
+
 from seqlogic.lbool import Vec, VecEnum, VecStruct, vec
 
 
 class Pixel(VecStruct):
     r: Vec[8]
     g: Vec[8]
     b: Vec[8]
@@ -20,14 +22,20 @@
 
 
 class Mixed(VecStruct):
     a: Vec[4]
     b: MyEnum
 
 
+class Nested(VecStruct):
+    q: Vec[4]
+    r: MyEnum
+    s: Mixed
+
+
 def test_empty():
     class EmptyStruct(VecStruct):
         pass
 
     s = EmptyStruct()
     assert len(s) == 0
     assert s.data == 0
@@ -75,7 +83,23 @@
     mx = Mixed()
     assert str(mx) == "Mixed(a=4bXXXX, b=MyEnum.X)"
     assert repr(mx) == "Mixed(a=Vec[4](0b00000000), b=MyEnum.X)"
 
     m1 = Mixed(a=vec("4b1010"), b=MyEnum.A)
     assert str(m1) == "Mixed(a=4b1010, b=MyEnum.A)"
     assert m1.b.B.name == "B"
+
+
+def test_nested():
+    n1 = Nested()
+    assert str(n1) == "Nested(q=4bXXXX, r=MyEnum.X, s=Mixed(a=4bXXXX, b=MyEnum.X))"
+
+    n2 = Nested(q=vec("4b1010"), r=MyEnum.A, s=Mixed(a=vec("4b0101"), b=MyEnum.B))
+    assert str(n2) == "Nested(q=4b1010, r=MyEnum.A, s=Mixed(a=4b0101, b=MyEnum.B))"
+
+
+def test_init_errors():
+    with pytest.raises(TypeError):
+        Pixel(r=vec("7b010_1010"))
+
+    with pytest.raises(TypeError):
+        Pixel(r=vec("9b0_0000_0000"))
```

