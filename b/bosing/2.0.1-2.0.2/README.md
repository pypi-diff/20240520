# Comparing `tmp/bosing-2.0.1.tar.gz` & `tmp/bosing-2.0.2.tar.gz`

## Comparing `bosing-2.0.1.tar` & `bosing-2.0.2.tar`

### file list

```diff
@@ -1,46 +1,48 @@
--rw-r--r--   0        0        0      598 1970-01-01 00:00:00.000000 bosing-2.0.1/Cargo.toml
--rw-r--r--   0     1001      127      505 2024-05-03 09:42:22.000000 bosing-2.0.1/.github/dependabot.yml
--rw-r--r--   0     1001      127      690 2024-05-03 09:42:22.000000 bosing-2.0.1/.github/workflows/auto-dep.yml
--rw-r--r--   0     1001      127     6323 2024-05-03 09:42:22.000000 bosing-2.0.1/.github/workflows/ci.yml
--rw-r--r--   0     1001      127      696 2024-05-03 09:42:22.000000 bosing-2.0.1/.gitignore
--rw-r--r--   0     1001      127      972 2024-05-03 09:42:22.000000 bosing-2.0.1/.readthedocs.yaml
--rw-r--r--   0     1001      127     1068 2024-05-03 09:42:22.000000 bosing-2.0.1/LICENSE.txt
--rw-r--r--   0     1001      127     1360 2024-05-03 09:42:22.000000 bosing-2.0.1/README.md
--rw-r--r--   0     1001      127    10767 2024-05-03 09:42:22.000000 bosing-2.0.1/bosing.pyi
--rw-r--r--   0     1001      127       78 2024-05-03 09:42:22.000000 bosing-2.0.1/clippy.toml
--rw-r--r--   0     1001      127      634 2024-05-03 09:42:22.000000 bosing-2.0.1/docs/Makefile
--rw-r--r--   0     1001      127      175 2024-05-03 09:42:22.000000 bosing-2.0.1/docs/_templates/autosummary/class.rst
--rw-r--r--   0     1001      127     1147 2024-05-03 09:42:22.000000 bosing-2.0.1/docs/_templates/autosummary/module.rst
--rw-r--r--   0     1001      127       82 2024-05-03 09:42:22.000000 bosing-2.0.1/docs/api.rst
--rw-r--r--   0     1001      127     1464 2024-05-03 09:42:22.000000 bosing-2.0.1/docs/conf.py
--rw-r--r--   0     1001      127     1258 2024-05-03 09:42:22.000000 bosing-2.0.1/docs/index.rst
--rw-r--r--   0     1001      127     1716 2024-05-03 09:42:22.000000 bosing-2.0.1/docs/instruction.rst
--rw-r--r--   0     1001      127      765 2024-05-03 09:42:22.000000 bosing-2.0.1/docs/make.bat
--rw-r--r--   0     1001      127      347 2024-05-03 09:42:22.000000 bosing-2.0.1/docs/quickstart.rst
--rw-r--r--   0     1001      127       22 2024-05-03 09:42:22.000000 bosing-2.0.1/docs/requirements.txt
--rw-r--r--   0     1001      127     5534 2024-05-03 09:42:22.000000 bosing-2.0.1/docs/schedule.rst
--rw-r--r--   0     1001      127     1171 2024-05-03 09:42:22.000000 bosing-2.0.1/example/flexible.py
--rw-r--r--   0     1001      127      533 2024-05-03 09:42:22.000000 bosing-2.0.1/example/hann.py
--rw-r--r--   0     1001      127      788 2024-05-03 09:42:22.000000 bosing-2.0.1/example/interp.py
--rw-r--r--   0     1001      127      696 2024-05-03 09:42:22.000000 bosing-2.0.1/example/overlap.py
--rw-r--r--   0     1001      127     2074 2024-05-03 09:42:22.000000 bosing-2.0.1/example/schedule.py
--rw-r--r--   0     1001      127     2343 2024-05-03 09:42:22.000000 bosing-2.0.1/example/schedule_stress.py
--rw-r--r--   0     1001      127     6064 2024-05-03 09:42:22.000000 bosing-2.0.1/ruff_defaults.toml
--rw-r--r--   0     1001      127     7345 2024-05-03 09:42:22.000000 bosing-2.0.1/src/executor.rs
--rw-r--r--   0     1001      127    63044 2024-05-03 09:42:22.000000 bosing-2.0.1/src/lib.rs
--rw-r--r--   0     1001      127    12435 2024-05-03 09:42:22.000000 bosing-2.0.1/src/pulse.rs
--rw-r--r--   0     1001      127     6647 2024-05-03 09:42:22.000000 bosing-2.0.1/src/quant.rs
--rw-r--r--   0     1001      127     2662 2024-05-03 09:42:22.000000 bosing-2.0.1/src/schedule/absolute.rs
--rw-r--r--   0     1001      127     7589 2024-05-03 09:42:22.000000 bosing-2.0.1/src/schedule/grid.rs
--rw-r--r--   0     1001      127     3561 2024-05-03 09:42:22.000000 bosing-2.0.1/src/schedule/play.rs
--rw-r--r--   0     1001      127     2490 2024-05-03 09:42:22.000000 bosing-2.0.1/src/schedule/repeat.rs
--rw-r--r--   0     1001      127     4225 2024-05-03 09:42:22.000000 bosing-2.0.1/src/schedule/simple.rs
--rw-r--r--   0     1001      127     5752 2024-05-03 09:42:22.000000 bosing-2.0.1/src/schedule/stack.rs
--rw-r--r--   0     1001      127    10472 2024-05-03 09:42:22.000000 bosing-2.0.1/src/schedule.rs
--rw-r--r--   0     1001      127     7649 2024-05-03 09:42:22.000000 bosing-2.0.1/src/shape.rs
--rw-r--r--   0     1001      127       14 2024-05-03 09:42:22.000000 bosing-2.0.1/stubtest-allowlist.txt
--rw-r--r--   0     1001      127        0 2024-05-03 09:42:22.000000 bosing-2.0.1/tests/__init__.py
--rw-r--r--   0     1001      127     1291 2024-05-03 09:42:22.000000 bosing-2.0.1/tests/test_basic.py
--rw-r--r--   0     1001      127    18328 2024-05-03 09:42:30.000000 bosing-2.0.1/Cargo.lock
--rw-r--r--   0     1001      127     1863 2024-05-03 09:42:22.000000 bosing-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     2249 1970-01-01 00:00:00.000000 bosing-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0      678 1970-01-01 00:00:00.000000 bosing-2.0.2/Cargo.toml
+-rw-r--r--   0     1001      127      505 2024-05-20 10:50:44.000000 bosing-2.0.2/.github/dependabot.yml
+-rw-r--r--   0     1001      127      690 2024-05-20 10:50:44.000000 bosing-2.0.2/.github/workflows/auto-dep.yml
+-rw-r--r--   0     1001      127     6323 2024-05-20 10:50:44.000000 bosing-2.0.2/.github/workflows/ci.yml
+-rw-r--r--   0     1001      127      696 2024-05-20 10:50:44.000000 bosing-2.0.2/.gitignore
+-rw-r--r--   0     1001      127      972 2024-05-20 10:50:44.000000 bosing-2.0.2/.readthedocs.yaml
+-rw-r--r--   0     1001      127     1068 2024-05-20 10:50:44.000000 bosing-2.0.2/LICENSE.txt
+-rw-r--r--   0     1001      127     1360 2024-05-20 10:50:44.000000 bosing-2.0.2/README.md
+-rw-r--r--   0     1001      127    10767 2024-05-20 10:50:44.000000 bosing-2.0.2/bosing.pyi
+-rw-r--r--   0     1001      127       78 2024-05-20 10:50:44.000000 bosing-2.0.2/clippy.toml
+-rw-r--r--   0     1001      127      634 2024-05-20 10:50:44.000000 bosing-2.0.2/docs/Makefile
+-rw-r--r--   0     1001      127      175 2024-05-20 10:50:44.000000 bosing-2.0.2/docs/_templates/autosummary/class.rst
+-rw-r--r--   0     1001      127     1147 2024-05-20 10:50:44.000000 bosing-2.0.2/docs/_templates/autosummary/module.rst
+-rw-r--r--   0     1001      127       82 2024-05-20 10:50:44.000000 bosing-2.0.2/docs/api.rst
+-rw-r--r--   0     1001      127     1464 2024-05-20 10:50:44.000000 bosing-2.0.2/docs/conf.py
+-rw-r--r--   0     1001      127     1258 2024-05-20 10:50:44.000000 bosing-2.0.2/docs/index.rst
+-rw-r--r--   0     1001      127     1716 2024-05-20 10:50:44.000000 bosing-2.0.2/docs/instruction.rst
+-rw-r--r--   0     1001      127      765 2024-05-20 10:50:44.000000 bosing-2.0.2/docs/make.bat
+-rw-r--r--   0     1001      127      347 2024-05-20 10:50:44.000000 bosing-2.0.2/docs/quickstart.rst
+-rw-r--r--   0     1001      127       22 2024-05-20 10:50:44.000000 bosing-2.0.2/docs/requirements.txt
+-rw-r--r--   0     1001      127     5534 2024-05-20 10:50:44.000000 bosing-2.0.2/docs/schedule.rst
+-rw-r--r--   0     1001      127     1171 2024-05-20 10:50:44.000000 bosing-2.0.2/example/flexible.py
+-rw-r--r--   0     1001      127      533 2024-05-20 10:50:44.000000 bosing-2.0.2/example/hann.py
+-rw-r--r--   0     1001      127      788 2024-05-20 10:50:44.000000 bosing-2.0.2/example/interp.py
+-rw-r--r--   0     1001      127      696 2024-05-20 10:50:44.000000 bosing-2.0.2/example/overlap.py
+-rw-r--r--   0     1001      127     2074 2024-05-20 10:50:44.000000 bosing-2.0.2/example/schedule.py
+-rw-r--r--   0     1001      127     2343 2024-05-20 10:50:44.000000 bosing-2.0.2/example/schedule_stress.py
+-rw-r--r--   0     1001      127     6064 2024-05-20 10:50:44.000000 bosing-2.0.2/ruff_defaults.toml
+-rw-r--r--   0     1001      127    11370 2024-05-20 10:50:44.000000 bosing-2.0.2/src/executor.rs
+-rw-r--r--   0     1001      127    63438 2024-05-20 10:50:44.000000 bosing-2.0.2/src/lib.rs
+-rw-r--r--   0     1001      127    14085 2024-05-20 10:50:44.000000 bosing-2.0.2/src/pulse.rs
+-rw-r--r--   0     1001      127     7540 2024-05-20 10:50:44.000000 bosing-2.0.2/src/quant.rs
+-rw-r--r--   0     1001      127     2367 2024-05-20 10:50:44.000000 bosing-2.0.2/src/schedule/absolute.rs
+-rw-r--r--   0     1001      127     9689 2024-05-20 10:50:44.000000 bosing-2.0.2/src/schedule/grid/helper.rs
+-rw-r--r--   0     1001      127     6941 2024-05-20 10:50:44.000000 bosing-2.0.2/src/schedule/grid.rs
+-rw-r--r--   0     1001      127     3145 2024-05-20 10:50:44.000000 bosing-2.0.2/src/schedule/play.rs
+-rw-r--r--   0     1001      127     2010 2024-05-20 10:50:44.000000 bosing-2.0.2/src/schedule/repeat.rs
+-rw-r--r--   0     1001      127     3577 2024-05-20 10:50:44.000000 bosing-2.0.2/src/schedule/simple.rs
+-rw-r--r--   0     1001      127     3132 2024-05-20 10:50:44.000000 bosing-2.0.2/src/schedule/stack/helper.rs
+-rw-r--r--   0     1001      127     7464 2024-05-20 10:50:44.000000 bosing-2.0.2/src/schedule/stack.rs
+-rw-r--r--   0     1001      127     7859 2024-05-20 10:50:44.000000 bosing-2.0.2/src/schedule.rs
+-rw-r--r--   0     1001      127     7677 2024-05-20 10:50:44.000000 bosing-2.0.2/src/shape.rs
+-rw-r--r--   0     1001      127       14 2024-05-20 10:50:44.000000 bosing-2.0.2/stubtest-allowlist.txt
+-rw-r--r--   0     1001      127        0 2024-05-20 10:50:44.000000 bosing-2.0.2/tests/__init__.py
+-rw-r--r--   0     1001      127     1291 2024-05-20 10:50:44.000000 bosing-2.0.2/tests/test_basic.py
+-rw-r--r--   0     1001      127    21393 2024-05-20 10:50:50.000000 bosing-2.0.2/Cargo.lock
+-rw-r--r--   0     1001      127     1863 2024-05-20 10:50:44.000000 bosing-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2249 1970-01-01 00:00:00.000000 bosing-2.0.2/PKG-INFO
```

### Comparing `bosing-2.0.1/Cargo.toml` & `bosing-2.0.2/Cargo.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "bosing"
-version = "2.0.1"
+version = "2.0.2"
 edition = "2021"
 license = "MIT"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "bosing"
 crate-type = ["cdylib"]
@@ -19,7 +19,12 @@
 itertools = "0.12.1"
 ndarray = { version = "0.15.6", features = ["rayon"] }
 num = "0.4.2"
 numpy = "0.21.0"
 ordered-float = "4.2.0"
 pyo3 = { version = "0.21.2", features = ["hashbrown", "anyhow"] }
 rayon = "1.10.0"
+thiserror = "1.0.60"
+
+[dev-dependencies]
+mockall = "0.12.1"
+test-case = "3.3.1"
```

### Comparing `bosing-2.0.1/.github/workflows/auto-dep.yml` & `bosing-2.0.2/.github/workflows/auto-dep.yml`

 * *Files identical despite different names*

### Comparing `bosing-2.0.1/.github/workflows/ci.yml` & `bosing-2.0.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `bosing-2.0.1/.gitignore` & `bosing-2.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `bosing-2.0.1/.readthedocs.yaml` & `bosing-2.0.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `bosing-2.0.1/LICENSE.txt` & `bosing-2.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bosing-2.0.1/README.md` & `bosing-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `bosing-2.0.1/bosing.pyi` & `bosing-2.0.2/bosing.pyi`

 * *Files identical despite different names*

### Comparing `bosing-2.0.1/docs/Makefile` & `bosing-2.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bosing-2.0.1/docs/_templates/autosummary/module.rst` & `bosing-2.0.2/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `bosing-2.0.1/docs/conf.py` & `bosing-2.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.1/docs/index.rst` & `bosing-2.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bosing-2.0.1/docs/instruction.rst` & `bosing-2.0.2/docs/instruction.rst`

 * *Files identical despite different names*

### Comparing `bosing-2.0.1/docs/make.bat` & `bosing-2.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bosing-2.0.1/docs/schedule.rst` & `bosing-2.0.2/docs/schedule.rst`

 * *Files identical despite different names*

### Comparing `bosing-2.0.1/example/flexible.py` & `bosing-2.0.2/example/flexible.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.1/example/hann.py` & `bosing-2.0.2/example/hann.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.1/example/interp.py` & `bosing-2.0.2/example/interp.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.1/example/overlap.py` & `bosing-2.0.2/example/overlap.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.1/example/schedule.py` & `bosing-2.0.2/example/schedule.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.1/example/schedule_stress.py` & `bosing-2.0.2/example/schedule_stress.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.1/ruff_defaults.toml` & `bosing-2.0.2/ruff_defaults.toml`

 * *Files identical despite different names*

### Comparing `bosing-2.0.1/src/executor.rs` & `bosing-2.0.2/src/schedule/grid.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,228 +1,249 @@
-use hashbrown::HashMap;
+mod helper;
+
+use std::sync::OnceLock;
+
+use anyhow::{bail, Result};
 
 use crate::{
-    pulse::{Envelope, PulseList, PulseListBuilder},
-    quant::{Amplitude, ChannelId, Frequency, Phase, ShapeId, Time},
-    schedule::{self, ArrangedElement, ElementVariant},
-    shape::Shape,
+    quant::{ChannelId, Time},
+    schedule::{grid::helper::Helper, merge_channel_ids, Alignment, Arranged, ElementRef, Measure},
+    GridLength,
 };
 
+use super::{Arrange, TimeRange};
+
+#[derive(Debug, Clone)]
+pub(crate) struct GridEntry {
+    element: ElementRef,
+    column: usize,
+    span: usize,
+}
+
+#[derive(Debug, Clone)]
+pub(crate) struct Grid {
+    children: Vec<GridEntry>,
+    columns: Vec<GridLength>,
+    channel_ids: Vec<ChannelId>,
+    measure_result: OnceLock<MeasureResult>,
+}
+
 #[derive(Debug, Clone)]
-pub struct Executor {
-    channels: HashMap<ChannelId, Channel>,
-    shapes: HashMap<ShapeId, Shape>,
-    amp_tolerance: Amplitude,
-    time_tolerance: Time,
+struct MeasureResult {
+    total_duration: Time,
+    column_sizes: Vec<Time>,
+    child_durations: Vec<Time>,
 }
 
-impl Executor {
-    pub fn new(amp_tolerance: Amplitude, time_tolerance: Time) -> Self {
+struct MeasureItem {
+    column: usize,
+    span: usize,
+    duration: Time,
+}
+
+impl GridEntry {
+    pub(crate) fn new(element: ElementRef) -> Self {
         Self {
-            channels: HashMap::new(),
-            shapes: HashMap::new(),
-            amp_tolerance,
-            time_tolerance,
+            element,
+            column: 0,
+            span: 1,
         }
     }
 
-    pub fn add_channel(&mut self, name: ChannelId, base_freq: Frequency) {
-        self.channels.insert(
-            name,
-            Channel::new(base_freq, self.amp_tolerance, self.time_tolerance),
-        );
+    pub(crate) fn with_column(mut self, column: usize) -> Self {
+        self.column = column;
+        self
     }
 
-    pub fn add_shape(&mut self, name: ShapeId, shape: Shape) {
-        self.shapes.insert(name, shape);
+    pub(crate) fn with_span(mut self, span: usize) -> Result<Self> {
+        if span == 0 {
+            bail!("Span should be greater than 0");
+        }
+        self.span = span;
+        Ok(self)
     }
+}
 
-    pub fn execute(&mut self, element: &ArrangedElement) {
-        self.execute_dispatch(element, Time::ZERO);
+impl Grid {
+    pub(crate) fn new() -> Self {
+        Self::default()
     }
 
-    pub fn into_result(self) -> HashMap<ChannelId, PulseList> {
-        self.channels
-            .into_iter()
-            .map(|(n, b)| (n, b.pulses.build()))
-            .collect()
+    pub(crate) fn with_columns(mut self, columns: Vec<GridLength>) -> Self {
+        if columns.is_empty() {
+            self.columns = vec![GridLength::star(1.0).unwrap()];
+        } else {
+            self.columns = columns;
+        }
+        self.measure_result.take();
+        self
     }
 
-    fn execute_dispatch(&mut self, element: &ArrangedElement, time: Time) {
-        if element.element().common.phantom() {
-            return;
-        }
-        let time = time + element.inner_time();
-        let duration = element.inner_duration();
-        match &element.element().variant {
-            ElementVariant::Play(e) => self.execute_play(e, time, duration),
-            ElementVariant::ShiftPhase(e) => self.execute_shift_phase(e),
-            ElementVariant::SetPhase(e) => self.execute_set_phase(e, time),
-            ElementVariant::ShiftFreq(e) => self.execute_shift_freq(e, time),
-            ElementVariant::SetFreq(e) => self.execute_set_freq(e, time),
-            ElementVariant::SwapPhase(e) => self.execute_swap_phase(e, time),
-            ElementVariant::Barrier(_) => (),
-            ElementVariant::Repeat(e) => {
-                let child = &element.try_get_children().expect("Invalid arrange data")[0];
-                self.execute_repeat(e, child, time, duration);
-            }
-            ElementVariant::Stack(_) | ElementVariant::Absolute(_) | ElementVariant::Grid(_) => {
-                let children = element.try_get_children().expect("Invalid arrange data");
-                self.execute_container(children, time);
-            }
-        }
+    pub(crate) fn with_children(mut self, children: Vec<GridEntry>) -> Self {
+        let channel_ids = merge_channel_ids(children.iter().map(|e| e.element.variant.channels()));
+        self.children = children;
+        self.channel_ids = channel_ids;
+        self.measure_result.take();
+        self
+    }
+
+    pub(crate) fn columns(&self) -> &[GridLength] {
+        &self.columns
+    }
+
+    fn measure_result(&self) -> &MeasureResult {
+        self.measure_result.get_or_init(|| {
+            measure_grid(
+                self.children.iter().map(|e| MeasureItem {
+                    duration: e.element.measure(),
+                    column: e.column,
+                    span: e.span,
+                }),
+                &self.columns,
+            )
+        })
     }
+}
 
-    fn execute_play(&mut self, element: &schedule::Play, time: Time, duration: Time) {
-        let shape = element.shape_id().map(|id| self.shapes[id].clone());
-        let width = element.width();
-        let plateau = if element.flexible() {
-            duration - width
-        } else {
-            element.plateau()
-        };
-        let amplitude = element.amplitude();
-        let drag_coef = element.drag_coef();
-        let freq = element.frequency();
-        let phase = element.phase();
-        let channel = self.channels.get_mut(element.channel_id()).unwrap();
-        channel.add_pulse(
-            shape, time, width, plateau, amplitude, drag_coef, freq, phase,
-        );
-    }
-
-    fn execute_shift_phase(&mut self, element: &schedule::ShiftPhase) {
-        let delta_phase = element.phase();
-        let channel = self.channels.get_mut(element.channel_id()).unwrap();
-        channel.shift_phase(delta_phase);
-    }
-
-    fn execute_set_phase(&mut self, element: &schedule::SetPhase, time: Time) {
-        let phase = element.phase();
-        let channel = self.channels.get_mut(element.channel_id()).unwrap();
-        channel.set_phase(phase, time);
-    }
-
-    fn execute_shift_freq(&mut self, element: &schedule::ShiftFreq, time: Time) {
-        let delta_freq = element.frequency();
-        let channel = self.channels.get_mut(element.channel_id()).unwrap();
-        channel.shift_freq(delta_freq, time);
-    }
-
-    fn execute_set_freq(&mut self, element: &schedule::SetFreq, time: Time) {
-        let freq = element.frequency();
-        let channel = self.channels.get_mut(element.channel_id()).unwrap();
-        channel.set_freq(freq, time);
-    }
-
-    fn execute_swap_phase(&mut self, element: &schedule::SwapPhase, time: Time) {
-        let ch1 = element.channel_id1();
-        let ch2 = element.channel_id2();
-        if ch1 == ch2 {
-            return;
-        }
-        let [channel, other] = self.channels.get_many_mut([ch1, ch2]).unwrap();
-        channel.swap_phase(other, time);
-    }
-
-    fn execute_repeat(
-        &mut self,
-        element: &schedule::Repeat,
-        child: &ArrangedElement,
-        time: Time,
-        duration: Time,
-    ) {
-        let count = element.count();
-        if count == 0 {
-            return;
-        }
-        let spacing = element.spacing();
-        let time_step = (duration + spacing) / count as f64;
-        for i in 0..count {
-            let child_time = time + i as f64 * time_step;
-            self.execute_dispatch(child, child_time);
-        }
-    }
-
-    fn execute_container(&mut self, children: &[ArrangedElement], time: Time) {
-        for child in children {
-            self.execute_dispatch(child, time);
+impl Default for Grid {
+    fn default() -> Self {
+        Self {
+            children: vec![],
+            columns: vec![GridLength::star(1.0).unwrap()],
+            channel_ids: vec![],
+            measure_result: OnceLock::new(),
         }
     }
 }
 
-#[derive(Debug, Clone)]
-struct Channel {
-    base_freq: Frequency,
-    delta_freq: Frequency,
-    phase: Phase,
-    pulses: PulseListBuilder,
-}
+impl Measure for Grid {
+    fn measure(&self) -> Time {
+        let MeasureResult { total_duration, .. } = self.measure_result();
+        *total_duration
+    }
 
-impl Channel {
-    fn new(base_freq: Frequency, amp_tolerance: Amplitude, time_tolerance: Time) -> Self {
-        Self {
-            base_freq,
-            delta_freq: Frequency::ZERO,
-            phase: Phase::ZERO,
-            pulses: PulseListBuilder::new(amp_tolerance, time_tolerance),
-        }
+    fn channels(&self) -> &[ChannelId] {
+        &self.channel_ids
     }
+}
 
-    fn shift_freq(&mut self, delta_freq: Frequency, time: Time) {
-        let delta_phase = -delta_freq * time;
-        self.delta_freq += delta_freq;
-        self.phase += delta_phase;
-    }
-
-    fn set_freq(&mut self, freq: Frequency, time: Time) {
-        let delta_freq = freq - self.delta_freq;
-        let delta_phase = -delta_freq * time;
-        self.delta_freq = freq;
-        self.phase += delta_phase;
-    }
-
-    fn shift_phase(&mut self, delta_phase: Phase) {
-        self.phase += delta_phase;
-    }
-
-    fn set_phase(&mut self, phase: Phase, time: Time) {
-        self.phase = phase - self.delta_freq * time;
-    }
-
-    fn total_freq(&self) -> Frequency {
-        self.base_freq + self.delta_freq
-    }
-
-    fn swap_phase(&mut self, other: &mut Self, time: Time) {
-        let delta_freq = self.total_freq() - other.total_freq();
-        let phase1 = self.phase;
-        let phase2 = other.phase;
-        self.phase = phase2 - delta_freq * time;
-        other.phase = phase1 + delta_freq * time;
-    }
-
-    fn add_pulse(
-        &mut self,
-        shape: Option<Shape>,
-        time: Time,
-        width: Time,
-        plateau: Time,
-        amplitude: Amplitude,
-        drag_coef: f64,
-        freq: Frequency,
-        phase: Phase,
-    ) {
-        let envelope = Envelope::new(shape, width, plateau);
-        let global_freq = self.total_freq();
-        let local_freq = freq;
-        self.pulses.push(
-            envelope,
-            global_freq,
-            local_freq,
-            time,
-            amplitude,
-            drag_coef,
-            phase,
+impl Arrange for Grid {
+    fn arrange(&self, time_range: TimeRange) -> impl Iterator<Item = Arranged<&ElementRef>> {
+        let MeasureResult {
+            column_sizes,
+            child_durations,
+            ..
+        } = self.measure_result();
+        let mut helper = Helper::new_with_column_sizes(&self.columns, column_sizes.clone());
+        helper.expand_to_fit(time_range.span);
+        let column_starts = helper.column_starts();
+        self.children.iter().zip(child_durations).map(
+            move |(
+                GridEntry {
+                    element,
+                    column,
+                    span,
+                },
+                &child_duration,
+            )| {
+                let span = helper.normalize_span(*column, *span);
+                let start = span.start();
+                let span = span.span();
+                let span_duration = column_starts[start + span] - column_starts[start];
+                let child_duration = match element.common.alignment {
+                    Alignment::Stretch => span_duration,
+                    _ => child_duration,
+                };
+                let child_offset = match element.common.alignment {
+                    Alignment::End => span_duration - child_duration,
+                    Alignment::Center => (span_duration - child_duration) / 2.0,
+                    _ => Time::ZERO,
+                } + column_starts[start];
+                let child_time_range = TimeRange {
+                    start: time_range.start + child_offset,
+                    span: child_duration,
+                };
+                Arranged {
+                    item: element,
+                    time_range: child_time_range,
+                }
+            },
         )
     }
 }
+
+fn measure_grid<I>(children: I, columns: &[GridLength]) -> MeasureResult
+where
+    I: IntoIterator<Item = MeasureItem>,
+{
+    let mut helper = Helper::new(columns);
+    let children: Vec<MeasureItem> = children.into_iter().collect();
+    for &MeasureItem {
+        duration,
+        column,
+        span,
+    } in &children
+    {
+        let span = helper.normalize_span(column, span);
+        if span.span() == 1 {
+            helper.expand_span_to_fit(span, duration);
+        }
+    }
+    for &MeasureItem {
+        duration,
+        column,
+        span,
+    } in &children
+    {
+        let span = helper.normalize_span(column, span);
+        if span.span() != 1 {
+            helper.expand_span_to_fit(span, duration);
+        }
+    }
+    let column_sizes = helper.into_column_sizes();
+    let total_duration = column_sizes.iter().sum();
+    MeasureResult {
+        total_duration,
+        column_sizes,
+        child_durations: children.into_iter().map(|item| item.duration).collect(),
+    }
+}
+
+#[cfg(test)]
+mod tests {
+    use test_case::test_case;
+
+    use super::*;
+
+    fn time_vec(v: &[f64]) -> Vec<Time> {
+        v.iter().map(|&d| Time::new(d).unwrap()).collect()
+    }
+
+    #[test_case(&[(40.0, 0, 1)], &["30"], (30.0, vec![30.0]); "not enough size")]
+    #[test_case(
+        &[(40.0, 0, 1), (40.0, 2, 1), (100.0, 0, 3)],
+        &["auto", "*", "auto"],
+        (100.0, vec![40.0, 20.0, 40.0]);
+        "sandwiched"
+    )]
+    #[test_case(&[], &["*"], (0.0, vec![0.0]); "empty star")]
+    #[test_case(&[], &["10"], (10.0, vec![10.0]); "empty fixed")]
+    fn measure_grid(children: &[(f64, usize, usize)], columns: &[&str], expected: (f64, Vec<f64>)) {
+        let children = children
+            .iter()
+            .map(|&(duration, column, span)| MeasureItem {
+                duration: Time::new(duration).unwrap(),
+                column,
+                span,
+            });
+        let columns: Vec<GridLength> = columns.iter().map(|s| s.parse().unwrap()).collect();
+
+        let MeasureResult {
+            total_duration,
+            column_sizes,
+            ..
+        } = super::measure_grid(children, &columns);
+
+        assert_eq!(total_duration, Time::new(expected.0).unwrap());
+        assert_eq!(column_sizes, time_vec(&expected.1));
+    }
+}
```

### Comparing `bosing-2.0.1/src/lib.rs` & `bosing-2.0.2/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 //! Although Element struct may contains [`Py<Element>`] as children, it is not
 //! possible to create cyclic references because we don't allow mutate the
 //! children after creation.
-use std::{borrow::Borrow, fmt::Debug, sync::Arc};
+mod executor;
+mod pulse;
+mod quant;
+mod schedule;
+mod shape;
+
+use std::{borrow::Borrow, fmt::Debug, str::FromStr, sync::Arc};
 
 use hashbrown::HashMap;
 use indoc::indoc;
 use numpy::{
     dot_bound, prelude::*, AllowTypeChange, PyArray1, PyArray2, PyArrayLike1, PyArrayLike2,
 };
 use pyo3::{
-    exceptions::{PyTypeError, PyValueError},
+    exceptions::{PyRuntimeError, PyTypeError, PyValueError},
     prelude::*,
     types::{DerefToPyAny, PyDict},
 };
 use rayon::prelude::*;
 
-use executor::Executor;
-use pulse::{PulseList, Sampler};
-use quant::{Amplitude, ChannelId, Frequency, Phase, ShapeId, Time};
-use schedule::{ElementCommonBuilder, ElementRef};
-
-mod executor;
-mod pulse;
-mod quant;
-mod schedule;
-mod shape;
+use crate::{
+    executor::Executor,
+    pulse::{PulseList, Sampler},
+    quant::{Amplitude, ChannelId, Frequency, Phase, ShapeId, Time},
+    schedule::{ElementCommonBuilder, ElementRef},
+};
 
 /// Channel configuration.
 ///
 /// `align_level` is the time axis alignment granularity. With sampling interval
 /// :math:`\Delta t` and `align_level` :math:`n`, start of pulse is aligned to
 /// the nearest multiple of :math:`2^n \Delta t`.
 ///
@@ -175,15 +177,15 @@
 ///
 /// - :attr:`Alignment.End`
 /// - :attr:`Alignment.Start`
 /// - :attr:`Alignment.Center`
 /// - :attr:`Alignment.Stretch`: Stretch the element to fill the parent.
 #[pyclass(frozen)]
 #[derive(Debug, Clone, Copy, PartialEq, Eq)]
-pub enum Alignment {
+enum Alignment {
     End,
     Start,
     Center,
     Stretch,
 }
 
 #[pymethods]
@@ -1151,15 +1153,15 @@
 ///     This is the default order.
 ///
 /// - :attr:`Direction.Forward`:
 ///     Process children in original order and schedule them as early as
 ///     possible.
 #[pyclass(frozen)]
 #[derive(Debug, Clone, Copy, PartialEq, Eq)]
-pub enum Direction {
+enum Direction {
     Backward,
     Forward,
 }
 
 #[pymethods]
 impl Direction {
     /// Convert the value to Direction.
@@ -1510,15 +1512,15 @@
 /// Length of a grid column.
 ///
 /// :class:`GridLength` is used to specify the length of a grid column. The
 /// length can be specified in seconds, as a fraction of the remaining duration,
 /// or automatically.
 #[pyclass(get_all, frozen)]
 #[derive(Debug, Clone)]
-pub struct GridLength {
+struct GridLength {
     value: f64,
     unit: GridLengthUnit,
 }
 
 #[pymethods]
 impl GridLength {
     /// Create an automatic grid length.
@@ -1537,15 +1539,15 @@
     ///
     /// Args:
     ///     value (float): Ratio of the remaining duration.
     /// Returns:
     ///     GridLength: Ratio based grid length.
     #[staticmethod]
     fn star(value: f64) -> PyResult<Self> {
-        if !value.is_finite() || value <= 0.0 {
+        if !(value.is_finite() && value > 0.0) {
             return Err(PyValueError::new_err("The value must be greater than 0."));
         }
         Ok(GridLength {
             value,
             unit: GridLengthUnit::Star,
         })
     }
@@ -1554,15 +1556,15 @@
     ///
     /// Args:
     ///     value (float): Fixed length in seconds.
     /// Returns:
     ///     GridLength: Fixed grid length.
     #[staticmethod]
     fn fixed(value: f64) -> PyResult<Self> {
-        if !value.is_finite() || value < 0.0 {
+        if !(value.is_finite() && value >= 0.0) {
             return Err(PyValueError::new_err(
                 "The value must be greater than or equal to 0.",
             ));
         }
         Ok(GridLength {
             value,
             unit: GridLengthUnit::Seconds,
@@ -1591,34 +1593,57 @@
         let py = obj.py();
         if let Ok(slf) = obj.extract() {
             return Ok(slf);
         }
         if let Ok(v) = obj.extract() {
             return Py::new(py, GridLength::fixed(v)?);
         }
-        if let Ok(s) = obj.extract::<&str>() {
-            if s == "auto" {
-                return Py::new(py, GridLength::auto());
-            }
-            if s == "*" {
-                return Py::new(py, GridLength::star(1.0)?);
-            }
-            if let Some(v) = s.strip_suffix('*').and_then(|x| x.parse().ok()) {
-                return Py::new(py, GridLength::star(v)?);
-            }
-            if let Ok(v) = s.parse() {
-                return Py::new(py, GridLength::fixed(v)?);
-            }
+        if let Ok(s) = obj.extract() {
+            return Py::new(py, GridLength::from_str(s)?);
         }
         Err(PyValueError::new_err(
             "Failed to convert the value to GridLength.",
         ))
     }
 }
 
+impl GridLength {
+    fn is_auto(&self) -> bool {
+        self.unit == GridLengthUnit::Auto
+    }
+
+    fn is_star(&self) -> bool {
+        self.unit == GridLengthUnit::Star
+    }
+
+    fn is_fixed(&self) -> bool {
+        self.unit == GridLengthUnit::Seconds
+    }
+}
+
+impl FromStr for GridLength {
+    type Err = anyhow::Error;
+
+    fn from_str(s: &str) -> Result<Self, Self::Err> {
+        if s == "auto" {
+            return Ok(GridLength::auto());
+        }
+        if s == "*" {
+            return Ok(GridLength::star(1.0)?);
+        }
+        if let Some(v) = s.strip_suffix('*').and_then(|x| x.parse().ok()) {
+            return Ok(GridLength::star(v)?);
+        }
+        if let Ok(v) = s.parse() {
+            return Ok(GridLength::fixed(v)?);
+        }
+        Err(anyhow::anyhow!("Invalid GridLength string: {}", s))
+    }
+}
+
 fn extract_grid_length(obj: &Bound<PyAny>) -> PyResult<GridLength> {
     GridLength::convert(obj).and_then(|x| x.extract(obj.py()))
 }
 
 /// A child element in a grid layout.
 ///
 /// Args:
@@ -1778,14 +1803,15 @@
         let rust_children = children
             .iter()
             .map(|x| {
                 let element = x.element.get().0.clone();
                 schedule::GridEntry::new(element)
                     .with_column(x.column)
                     .with_span(x.span)
+                    .expect("Should be checked in GridEntry::new")
             })
             .collect();
         let variant = schedule::Grid::new()
             .with_children(rust_children)
             .with_columns(columns);
         Ok((
             Self { children },
@@ -1828,14 +1854,15 @@
         let rust_children = children
             .iter()
             .map(|x| {
                 let element = x.element.get().0.clone();
                 schedule::GridEntry::new(element)
                     .with_column(x.column)
                     .with_span(x.span)
+                    .expect("Should be checked in GridEntry::new")
             })
             .collect();
         let rust_base = &slf.downcast::<Element>()?.get().0;
         let common = rust_base.common.clone();
         let variant = Self::variant(slf).clone().with_children(rust_children);
         Py::new(
             py,
@@ -1929,15 +1956,15 @@
         schedule,
         &channels,
         &shapes,
         time_tolerance,
         amp_tolerance,
         allow_oversize,
     )?;
-    let waveforms = sample_waveform(py, &channels, pulse_lists, crosstalk, time_tolerance);
+    let waveforms = sample_waveform(py, &channels, pulse_lists, crosstalk, time_tolerance)?;
     py.allow_threads(|| {
         waveforms
             .into_par_iter()
             .map(|(n, w)| {
                 Python::with_gil(|py| {
                     let mut w = w.into_bound(py);
                     let c = &channels[&n];
@@ -1954,40 +1981,35 @@
     schedule: Bound<Element>,
     channels: &HashMap<ChannelId, Channel>,
     shapes: &HashMap<ShapeId, Py<Shape>>,
     time_tolerance: Time,
     amp_tolerance: Amplitude,
     allow_oversize: bool,
 ) -> PyResult<HashMap<ChannelId, PulseList>> {
-    let root = schedule.get().0.clone();
-    let measured = schedule::measure(root, Time::INFINITY);
-    let arrange_options = schedule::ScheduleOptions {
-        time_tolerance,
-        allow_oversize,
-    };
-    let arranged = schedule::arrange(&measured, Time::ZERO, measured.duration(), &arrange_options)?;
-    let mut executor = Executor::new(amp_tolerance, time_tolerance);
+    let mut executor = Executor::new(amp_tolerance, time_tolerance, allow_oversize);
     for (n, c) in channels {
         executor.add_channel(n.clone(), c.base_freq);
     }
     for (n, s) in shapes {
         let s = s.bind(py);
         executor.add_shape(n.clone(), Shape::get_rust_shape(s)?);
     }
-    executor.execute(&arranged);
+    executor
+        .execute(&schedule.get().0)
+        .map_err(|e| PyRuntimeError::new_err(e.to_string()))?;
     Ok(executor.into_result())
 }
 
 fn sample_waveform(
     py: Python,
     channels: &HashMap<ChannelId, Channel>,
     pulse_lists: HashMap<ChannelId, PulseList>,
     crosstalk: Option<(PyArrayLike2<f64, AllowTypeChange>, Vec<ChannelId>)>,
     time_tolerance: Time,
-) -> HashMap<ChannelId, Py<PyArray2<f64>>> {
+) -> PyResult<HashMap<ChannelId, Py<PyArray2<f64>>>> {
     let waveforms: HashMap<_, _> = channels
         .iter()
         .map(|(n, c)| {
             let n_w = if c.is_real { 1 } else { 2 };
             (
                 n.clone(),
                 PyArray2::zeros_bound(py, (n_w, c.length), false).unbind(),
@@ -1999,16 +2021,16 @@
         // SAFETY: These arrays are just created.
         let array = unsafe { waveforms[n].bind(py).as_array_mut() };
         sampler.add_channel(n.clone(), array, c.sample_rate, c.delay, c.align_level);
     }
     if let Some((crosstalk, names)) = &crosstalk {
         sampler.set_crosstalk(crosstalk.as_array(), names.clone());
     }
-    sampler.sample(time_tolerance);
-    waveforms
+    sampler.sample(time_tolerance)?;
+    Ok(waveforms)
 }
 
 fn post_process<'py>(
     py: Python<'py>,
     w: &mut Bound<'py, PyArray2<f64>>,
     c: &Channel,
 ) -> PyResult<()> {
```

### Comparing `bosing-2.0.1/src/pulse.rs` & `bosing-2.0.2/src/pulse.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 use std::{
     ops::{Add, Mul},
     sync::Arc,
 };
 
+use anyhow::{bail, Context, Result};
 use cached::proc_macro::cached;
 use float_cmp::approx_eq;
 use hashbrown::HashMap;
 use itertools::{izip, Itertools};
 use ndarray::{s, ArrayView2, ArrayViewMut2};
 use numpy::Complex64;
 use rayon::prelude::*;
@@ -17,22 +18,22 @@
 };
 
 /// A pulse envelope
 ///
 /// If `shape` is `None`, constructor will set `plateau` to `width + plateau`
 /// and `width` to `0`.
 #[derive(Debug, Clone, PartialEq, Eq, Hash)]
-pub struct Envelope {
+pub(crate) struct Envelope {
     shape: Option<Shape>,
     width: Time,
     plateau: Time,
 }
 
 impl Envelope {
-    pub fn new(mut shape: Option<Shape>, mut width: Time, mut plateau: Time) -> Self {
+    pub(crate) fn new(mut shape: Option<Shape>, mut width: Time, mut plateau: Time) -> Self {
         if shape.is_none() {
             plateau += width;
             width = Time::ZERO;
         }
         if width == Time::ZERO {
             shape = None
         }
@@ -78,47 +79,47 @@
             amp: self.amp * rhs,
             drag: self.drag * rhs,
         }
     }
 }
 
 #[derive(Debug, Clone)]
-pub struct PulseList {
+pub(crate) struct PulseList {
     items: HashMap<ListBin, Vec<(Time, PulseAmplitude)>>,
 }
 
 #[derive(Debug, Clone)]
-pub struct Crosstalk<'a> {
+pub(crate) struct Crosstalk<'a> {
     matrix: ArrayView2<'a, f64>,
     names: Vec<ChannelId>,
 }
 
 impl<'a> Crosstalk<'a> {
-    pub fn new(matrix: ArrayView2<'a, f64>, names: Vec<ChannelId>) -> Self {
+    pub(crate) fn new(matrix: ArrayView2<'a, f64>, names: Vec<ChannelId>) -> Self {
         Self { matrix, names }
     }
 }
 
 #[derive(Debug)]
-pub struct Sampler<'a> {
+pub(crate) struct Sampler<'a> {
     channels: HashMap<ChannelId, Channel<'a>>,
     pulse_lists: HashMap<ChannelId, PulseList>,
     crosstalk: Option<Crosstalk<'a>>,
 }
 
 impl<'a> Sampler<'a> {
-    pub fn new(pulse_lists: HashMap<ChannelId, PulseList>) -> Self {
+    pub(crate) fn new(pulse_lists: HashMap<ChannelId, PulseList>) -> Self {
         Self {
             channels: HashMap::new(),
             pulse_lists,
             crosstalk: None,
         }
     }
 
-    pub fn add_channel(
+    pub(crate) fn add_channel(
         &mut self,
         name: ChannelId,
         waveform: ArrayViewMut2<'a, f64>,
         sample_rate: Frequency,
         delay: Time,
         align_level: i32,
     ) {
@@ -129,27 +130,27 @@
                 sample_rate,
                 align_level,
                 delay,
             },
         );
     }
 
-    pub fn set_crosstalk(&mut self, crosstalk: ArrayView2<'a, f64>, names: Vec<ChannelId>) {
+    pub(crate) fn set_crosstalk(&mut self, crosstalk: ArrayView2<'a, f64>, names: Vec<ChannelId>) {
         self.crosstalk = Some(Crosstalk::new(crosstalk, names));
     }
 
-    pub fn sample(self, time_tolerance: Time) {
+    pub(crate) fn sample(self, time_tolerance: Time) -> Result<()> {
         if let Some(crosstalk) = self.crosstalk {
             let ct_lookup = crosstalk
                 .names
                 .iter()
                 .enumerate()
                 .map(|(i, name)| (name, i))
                 .collect::<HashMap<_, _>>();
-            self.channels.into_par_iter().for_each(|(n, c)| {
+            self.channels.into_par_iter().try_for_each(|(n, c)| {
                 let row_index = ct_lookup.get(&n).copied();
                 if let Some(row_index) = row_index {
                     let row = crosstalk.matrix.slice(s![row_index, ..]);
                     let lists = row
                         .iter()
                         .copied()
                         .zip(&crosstalk.names)
@@ -158,67 +159,82 @@
                         lists,
                         c.waveform,
                         c.sample_rate,
                         c.delay,
                         c.align_level,
                         time_tolerance,
                     )
+                    .with_context(|| format!("Failed to sample channel '{}'", n))
                 } else {
                     let list = self.pulse_lists[&n]
                         .items
                         .iter()
                         .map(|(bin, items)| (bin.clone(), items.iter().copied()));
                     sample_pulse_list(list, c.waveform, c.sample_rate, c.delay, c.align_level)
+                        .with_context(|| format!("Failed to sample channel '{}'", n))
                 }
-            });
+            })
         } else {
-            self.channels.into_par_iter().for_each(|(n, c)| {
+            self.channels.into_par_iter().try_for_each(|(n, c)| {
                 let list = self.pulse_lists[&n]
                     .items
                     .iter()
                     .map(|(bin, items)| (bin.clone(), items.iter().copied()));
                 sample_pulse_list(list, c.waveform, c.sample_rate, c.delay, c.align_level)
+                    .with_context(|| format!("Failed to sample channel '{}'", n))
             })
         }
     }
 }
 
 #[derive(Debug)]
 struct Channel<'a> {
     waveform: ArrayViewMut2<'a, f64>,
     sample_rate: Frequency,
     align_level: i32,
     delay: Time,
 }
 
 #[derive(Debug, Clone)]
-pub struct PulseListBuilder {
+pub(crate) struct PulseListBuilder {
     items: HashMap<ListBin, Vec<(Time, PulseAmplitude)>>,
     amp_tolerance: Amplitude,
     time_tolerance: Time,
 }
 
+pub(crate) struct PushArgs {
+    pub(crate) envelope: Envelope,
+    pub(crate) global_freq: Frequency,
+    pub(crate) local_freq: Frequency,
+    pub(crate) time: Time,
+    pub(crate) amplitude: Amplitude,
+    pub(crate) drag_coef: f64,
+    pub(crate) phase: Phase,
+}
+
 impl PulseListBuilder {
-    pub fn new(amp_tolerance: Amplitude, time_tolerance: Time) -> Self {
+    pub(crate) fn new(amp_tolerance: Amplitude, time_tolerance: Time) -> Self {
         Self {
             items: HashMap::new(),
             amp_tolerance,
             time_tolerance,
         }
     }
 
-    pub fn push(
+    pub(crate) fn push(
         &mut self,
-        envelope: Envelope,
-        global_freq: Frequency,
-        local_freq: Frequency,
-        time: Time,
-        amplitude: Amplitude,
-        drag_coef: f64,
-        phase: Phase,
+        PushArgs {
+            envelope,
+            global_freq,
+            local_freq,
+            time,
+            amplitude,
+            drag_coef,
+            phase,
+        }: PushArgs,
     ) {
         if approx_eq!(
             f64,
             amplitude.value(),
             0.0,
             epsilon = self.amp_tolerance.value()
         ) {
@@ -231,15 +247,15 @@
         };
         let amp = amplitude.value() * phase.phaser();
         let drag = amp * Complex64::i() * drag_coef;
         let amplitude = PulseAmplitude { amp, drag };
         self.items.entry(bin).or_default().push((time, amplitude));
     }
 
-    pub fn build(mut self) -> PulseList {
+    pub(crate) fn build(mut self) -> PulseList {
         for pulses in self.items.values_mut() {
             pulses.sort_unstable_by_key(|(time, _)| *time);
             let mut i = 0;
             for j in 1..pulses.len() {
                 if approx_eq!(
                     f64,
                     pulses[i].0.value(),
@@ -341,15 +357,15 @@
 fn merge_and_sample<'a>(
     lists: impl IntoIterator<Item = (f64, &'a PulseList)>,
     waveform: ArrayViewMut2<f64>,
     sample_rate: Frequency,
     delay: Time,
     align_level: i32,
     time_tolerance: Time,
-) {
+) -> Result<()> {
     let mut merged: HashMap<ListBin, Vec<_>> = HashMap::new();
     for (multiplier, list) in lists {
         if multiplier == 0.0 {
             continue;
         }
         for (bin, items) in &list.items {
             merged.entry(bin.clone()).or_default().push(
@@ -384,47 +400,61 @@
 
 fn sample_pulse_list<PL, L>(
     list: PL,
     mut waveform: ArrayViewMut2<f64>,
     sample_rate: Frequency,
     delay: Time,
     align_level: i32,
-) where
+) -> Result<()>
+where
     PL: IntoIterator<Item = (ListBin, L)>,
     L: IntoIterator<Item = (Time, PulseAmplitude)>,
 {
     for (bin, items) in list {
         let ListBin {
             envelope,
             global_freq,
             local_freq,
         } = bin;
         for (time, PulseAmplitude { amp, drag }) in items {
             let t_start = time + delay;
             let i_frac_start = AlignedIndex::new(t_start, sample_rate, align_level).unwrap();
-            let i_start = i_frac_start.ceil_as_usize().unwrap();
+            if i_frac_start.value() < 0.0 {
+                bail!("The start time of a pulse is negative, try adjusting channel delay or schedule. start time: {}", t_start.value());
+            }
+            let i_start = i_frac_start.ceil_to_usize().unwrap();
             let index_offset = i_frac_start.index_offset().unwrap();
             let total_freq = global_freq + local_freq;
             let dt = sample_rate.dt();
             let phase0 = global_freq * (i_start as f64 * dt - delay)
                 + local_freq * index_offset.value() * dt;
             let dphase = total_freq * dt;
+            if i_start >= waveform.shape()[1] {
+                bail!("The start index of a pulse is out of bounds, try adjusting channel delay, length or schedule. start index: {}, start time: {}", i_start, t_start.value());
+            }
             let mut waveform = waveform.slice_mut(s![.., i_start..]);
             if let Some(shape) = &envelope.shape {
                 let envelope = get_envelope(
                     shape.clone(),
                     envelope.width,
                     envelope.plateau,
                     index_offset,
                     sample_rate,
                 );
                 let drag = drag * sample_rate.value();
+                if waveform.shape()[1] < envelope.len() {
+                    bail!("The pulse end time is out of bounds, try adjusting channel delay, length or schedule. end time: {}", t_start.value() + envelope.len() as f64 * dt.value());
+                }
                 mix_add_envelope(waveform, &envelope, amp, drag, phase0, dphase);
             } else {
                 let plateau = envelope.plateau;
                 let i_plateau = (plateau.value() * sample_rate.value()).ceil() as usize;
+                if waveform.shape()[1] < i_plateau {
+                    bail!("The pulse end time is out of bounds, try adjusting channel delay, length or schedule. end time: {}", t_start.value() + plateau.value());
+                }
                 let waveform = waveform.slice_mut(s![.., ..i_plateau]);
                 mix_add_plateau(waveform, amp, phase0, dphase);
             }
         }
     }
+    Ok(())
 }
```

### Comparing `bosing-2.0.1/src/quant.rs` & `bosing-2.0.2/src/quant.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,126 @@
 use std::{
     iter::Sum,
     ops::{Add, AddAssign, Div, Mul, Neg, Sub, SubAssign},
     sync::Arc,
 };
 
-use anyhow::{bail, Result};
 use num::NumCast;
 use numpy::Complex64;
 use ordered_float::NotNan;
-use pyo3::{prelude::*, types::PyFloat, IntoPy};
+use pyo3::{exceptions::PyValueError, prelude::*, types::PyFloat, IntoPy};
+use thiserror::Error;
+
+#[derive(Debug, Error)]
+pub(crate) enum Error {
+    #[error("NaN value is not allowed")]
+    NanValue(#[from] ordered_float::FloatIsNan),
+    #[error("Infinite value is not allowed")]
+    InfiniteValue,
+}
+
+macro_rules! def_quant {
+    ($t:ident) => {
+        #[derive(Debug, Clone, Copy, PartialEq, Eq, Hash, PartialOrd, Ord, Default)]
+        pub(crate) struct $t(NotNan<f64>);
+    };
+}
+
+def_quant!(Time);
+def_quant!(Frequency);
+def_quant!(Phase);
+def_quant!(Amplitude);
+
+#[derive(Debug, Clone, Copy, PartialEq, Eq, Hash, PartialOrd, Ord)]
+pub(crate) struct AlignedIndex(NotNan<f64>);
+
+macro_rules! def_id {
+    ($t:ident) => {
+        #[derive(Debug, Clone, PartialEq, Eq, Hash)]
+        pub(crate) struct $t(Arc<str>);
+    };
+}
+
+def_id!(ChannelId);
+def_id!(ShapeId);
+
+type Result<T> = std::result::Result<T, Error>;
+
+impl Time {
+    pub(crate) const INFINITY: Self = Self(unsafe { NotNan::new_unchecked(f64::INFINITY) });
+}
+
+impl Phase {
+    fn radians(&self) -> f64 {
+        self.value() * std::f64::consts::TAU
+    }
+
+    pub(crate) fn phaser(&self) -> Complex64 {
+        Complex64::from_polar(1.0, self.radians())
+    }
+}
+
+impl Frequency {
+    pub(crate) fn dt(&self) -> Time {
+        Time::new(1.0 / self.value()).expect("Frequency should be non-zero")
+    }
+}
+
+impl AlignedIndex {
+    pub(crate) fn new(time: Time, sample_rate: Frequency, align_level: i32) -> Result<Self> {
+        fn scaleb(x: f64, s: i32) -> f64 {
+            x * (s as f64).exp2()
+        }
+        let scaled_sr = scaleb(sample_rate.value(), -align_level);
+        let i = (time.value() * scaled_sr).ceil();
+        let aligned_index = scaleb(i, align_level);
+        Self::from_value(aligned_index)
+    }
+
+    fn from_value(value: f64) -> Result<Self> {
+        if value.is_infinite() {
+            return Err(Error::InfiniteValue);
+        }
+        Ok(Self(NotNan::new(value)?))
+    }
+
+    pub(crate) fn value(&self) -> f64 {
+        self.0.into_inner()
+    }
+
+    pub(crate) fn ceil_to_usize(&self) -> Option<usize> {
+        <usize as NumCast>::from(self.0.ceil())
+    }
+
+    pub(crate) fn index_offset(&self) -> Result<Self> {
+        Self::from_value(self.0.ceil() - self.0.into_inner())
+    }
+}
+
+impl Mul<Time> for Frequency {
+    type Output = Phase;
+
+    fn mul(self, rhs: Time) -> Self::Output {
+        Phase::new(self.value() * rhs.value()).expect("Should be a valid phase value")
+    }
+}
+
+impl Mul<Frequency> for Time {
+    type Output = Phase;
+
+    fn mul(self, rhs: Frequency) -> Self::Output {
+        Phase::new(self.value() * rhs.value()).expect("Should be a valid phase value")
+    }
+}
+
+impl From<Error> for PyErr {
+    fn from(err: Error) -> Self {
+        PyValueError::new_err(err.to_string())
+    }
+}
 
 macro_rules! forward_ref_binop {
     ($trait:ident, $method:ident, $t:ty) => {
         impl<'a> $trait<$t> for &'a $t {
             type Output = $t;
 
             fn $method(self, rhs: $t) -> Self::Output {
@@ -35,29 +143,25 @@
                 $trait::$method(*self, *rhs)
             }
         }
     };
 }
 
 macro_rules! impl_quant {
-    ($t:ident) => {
-        #[derive(Debug, Clone, Copy, PartialEq, Eq, Hash, PartialOrd, Ord, Default)]
-        pub struct $t(NotNan<f64>);
-
+    ($t:ty) => {
         impl $t {
-            pub fn new(value: f64) -> Result<Self> {
+            pub(crate) fn new(value: f64) -> Result<Self> {
                 Ok(Self(NotNan::new(value)?))
             }
 
-            pub fn value(&self) -> f64 {
+            pub(crate) fn value(&self) -> f64 {
                 self.0.into_inner()
             }
 
-            pub const INFINITY: Self = Self(unsafe { NotNan::new_unchecked(f64::INFINITY) });
-            pub const ZERO: Self = Self(unsafe { NotNan::new_unchecked(0.0) });
+            pub(crate) const ZERO: Self = Self(unsafe { NotNan::new_unchecked(0.0) });
         }
 
         impl<'py> FromPyObject<'py> for $t {
             fn extract_bound(ob: &Bound<'py, PyAny>) -> PyResult<Self> {
                 let value = ob.extract()?;
                 Ok(Self::new(value)?)
             }
@@ -148,105 +252,42 @@
         impl From<$t> for f64 {
             fn from(q: $t) -> Self {
                 q.value()
             }
         }
 
         impl TryFrom<f64> for $t {
-            type Error = anyhow::Error;
+            type Error = Error;
 
             fn try_from(value: f64) -> Result<Self> {
                 Self::new(value)
             }
         }
     };
 }
 
 impl_quant!(Time);
 impl_quant!(Frequency);
 impl_quant!(Phase);
 impl_quant!(Amplitude);
 
-impl Phase {
-    fn radians(&self) -> f64 {
-        self.value() * std::f64::consts::TAU
-    }
-
-    pub fn phaser(&self) -> Complex64 {
-        Complex64::from_polar(1.0, self.radians())
-    }
-}
-
-impl Frequency {
-    pub fn dt(&self) -> Time {
-        Time::new(1.0 / self.value()).expect("Frequency should be non-zero")
-    }
-}
-
-impl Mul<Time> for Frequency {
-    type Output = Phase;
-
-    fn mul(self, rhs: Time) -> Self::Output {
-        Phase::new(self.value() * rhs.value()).expect("Should be a valid phase value")
-    }
-}
-
-impl Mul<Frequency> for Time {
-    type Output = Phase;
-
-    fn mul(self, rhs: Frequency) -> Self::Output {
-        Phase::new(self.value() * rhs.value()).expect("Should be a valid phase value")
-    }
-}
-
-#[derive(Debug, Clone, Copy, PartialEq, Eq, Hash, PartialOrd, Ord)]
-pub struct AlignedIndex(NotNan<f64>);
-
-impl AlignedIndex {
-    pub fn new(time: Time, sample_rate: Frequency, align_level: i32) -> Result<Self> {
-        fn scaleb(x: f64, s: i32) -> f64 {
-            x * (s as f64).exp2()
-        }
-        let scaled_sr = scaleb(sample_rate.value(), -align_level);
-        let i = (time.value() * scaled_sr).ceil();
-        let aligned_index = scaleb(i, align_level);
-        Self::from_value(aligned_index)
-    }
-
-    fn from_value(value: f64) -> Result<Self> {
-        if value.is_infinite() {
-            bail!("Infinite value is not allowed");
-        }
-        Ok(Self(NotNan::new(value)?))
-    }
-
-    pub fn value(&self) -> f64 {
-        self.0.into_inner()
-    }
-
-    pub fn ceil_as_usize(&self) -> Option<usize> {
-        <usize as NumCast>::from(self.0.ceil())
-    }
-
-    pub fn index_offset(&self) -> Result<Self> {
-        Self::from_value(self.0.ceil() - self.0.into_inner())
-    }
-}
-
 macro_rules! impl_id {
-    ($t:ident) => {
-        #[derive(Debug, Clone, PartialEq, Eq, Hash)]
-        pub struct $t(Arc<str>);
-
+    ($t:ty) => {
         impl $t {
-            pub fn new(name: impl Into<Arc<str>>) -> Self {
+            pub(crate) fn new(name: impl Into<Arc<str>>) -> Self {
                 Self(name.into())
             }
         }
 
+        impl std::fmt::Display for $t {
+            fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
+                write!(f, "{}", self.0)
+            }
+        }
+
         impl<'py> FromPyObject<'py> for $t {
             fn extract_bound(ob: &Bound<'py, PyAny>) -> PyResult<Self> {
                 let name = ob.extract::<&str>()?;
                 Ok(Self::new(name))
             }
         }
```

### Comparing `bosing-2.0.1/src/schedule/absolute.rs` & `bosing-2.0.2/src/schedule/absolute.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,99 +1,99 @@
+use std::sync::OnceLock;
+
 use anyhow::{bail, Result};
-use itertools::Itertools as _;
 
-use super::{
-    arrange, measure, ArrangeContext, ArrangeResult, ArrangeResultVariant, ElementRef,
-    MeasureContext, MeasureResult, MeasureResultVariant, Schedule,
+use crate::{
+    quant::{ChannelId, Time},
+    schedule::{merge_channel_ids, ElementRef, Measure},
 };
-use crate::quant::{ChannelId, Time};
+
+use super::{Arrange, Arranged, TimeRange};
 
 #[derive(Debug, Clone)]
-pub struct AbsoluteEntry {
+pub(crate) struct AbsoluteEntry {
     time: Time,
     element: ElementRef,
 }
 
+#[derive(Debug, Clone, Default)]
+pub(crate) struct Absolute {
+    children: Vec<AbsoluteEntry>,
+    channel_ids: Vec<ChannelId>,
+    measure_result: OnceLock<Time>,
+}
+
 impl AbsoluteEntry {
-    pub fn new(element: ElementRef) -> Self {
+    pub(crate) fn new(element: ElementRef) -> Self {
         Self {
             time: Time::ZERO,
             element,
         }
     }
 
-    pub fn with_time(mut self, time: Time) -> Result<Self> {
+    pub(crate) fn with_time(mut self, time: Time) -> Result<Self> {
         if !time.value().is_finite() {
             bail!("Invalid time {:?}", time);
         }
         self.time = time;
         Ok(self)
     }
 }
 
-#[derive(Debug, Clone)]
-pub struct Absolute {
-    children: Vec<AbsoluteEntry>,
-    channel_ids: Vec<ChannelId>,
-}
-
-impl Default for Absolute {
-    fn default() -> Self {
-        Self::new()
-    }
-}
-
 impl Absolute {
-    pub fn new() -> Self {
-        Self {
-            children: vec![],
-            channel_ids: vec![],
-        }
+    pub(crate) fn new() -> Self {
+        Self::default()
     }
 
-    pub fn with_children(mut self, children: Vec<AbsoluteEntry>) -> Self {
-        let channel_ids = children
-            .iter()
-            .flat_map(|e| e.element.variant.channels())
-            .cloned()
-            .unique()
-            .collect();
+    pub(crate) fn with_children(mut self, children: Vec<AbsoluteEntry>) -> Self {
+        let channel_ids = merge_channel_ids(children.iter().map(|e| e.element.variant.channels()));
         self.children = children;
         self.channel_ids = channel_ids;
         self
     }
-}
 
-impl Schedule for Absolute {
-    fn measure(&self, context: &MeasureContext) -> MeasureResult {
-        let mut max_time = Time::ZERO;
-        let mut measured_children = vec![];
-        for e in &self.children {
-            let measured_child = measure(e.element.clone(), context.max_duration);
-            max_time = max_time.max(e.time + measured_child.duration);
-            measured_children.push(measured_child);
-        }
-        MeasureResult(max_time, MeasureResultVariant::Multiple(measured_children))
+    fn measure_result(&self) -> &Time {
+        self.measure_result
+            .get_or_init(|| measure_absolute(self.children.iter().map(|e| (&e.element, e.time))))
     }
+}
 
-    fn arrange(&self, context: &ArrangeContext) -> Result<ArrangeResult> {
-        let measured_children = match &context.measured_self.data {
-            MeasureResultVariant::Multiple(v) => v,
-            _ => bail!("Invalid measure data"),
-        };
-        let arranged_children = self
-            .children
-            .iter()
-            .map(|e| e.time)
-            .zip(measured_children.iter())
-            .map(|(t, mc)| arrange(mc, t, mc.duration, context.options))
-            .collect::<Result<_>>()?;
-        Ok(ArrangeResult(
-            context.final_duration,
-            ArrangeResultVariant::Multiple(arranged_children),
-        ))
+impl Measure for Absolute {
+    fn measure(&self) -> Time {
+        *self.measure_result()
     }
 
     fn channels(&self) -> &[ChannelId] {
         &self.channel_ids
     }
 }
+
+impl Arrange for Absolute {
+    fn arrange(&self, time_range: TimeRange) -> impl Iterator<Item = Arranged<&ElementRef>> {
+        self.children.iter().map(
+            move |AbsoluteEntry {
+                      time: offset,
+                      element,
+                  }| {
+                Arranged {
+                    item: element,
+                    time_range: TimeRange {
+                        start: time_range.start + offset,
+                        span: element.measure(),
+                    },
+                }
+            },
+        )
+    }
+}
+
+fn measure_absolute<I, M>(children: I) -> Time
+where
+    I: IntoIterator<Item = (M, Time)>,
+    M: Measure,
+{
+    children
+        .into_iter()
+        .map(|(child, offset)| offset + child.measure())
+        .max()
+        .unwrap_or(Time::ZERO)
+}
```

### Comparing `bosing-2.0.1/src/shape.rs` & `bosing-2.0.2/src/shape.rs`

 * *Files 1% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 /// A shape that can be used to modulate the amplitude of a signal.
 ///
 /// The shape is defined in the range \[-0.5, 0.5\].
 ///
 /// Internally, shape instances are cached such that we can compare and hash
 /// by instance address.
 #[derive(Debug, Clone)]
-pub struct Shape(Arc<ShapeVariant>);
+pub(crate) struct Shape(Arc<ShapeVariant>);
 
 impl Shape {
-    pub fn new_hann() -> Self {
+    pub(crate) fn new_hann() -> Self {
         Self(get_shape_instance(ShapeKey::Hann))
     }
 
-    pub fn new_interp(knots: Vec<f64>, controls: Vec<f64>, degree: usize) -> Result<Self> {
+    pub(crate) fn new_interp(knots: Vec<f64>, controls: Vec<f64>, degree: usize) -> Result<Self> {
         let knots = knots
             .into_iter()
             .map(NotNan::new)
             .collect::<Result<_, _>>()?;
         let controls = controls
             .into_iter()
             .map(NotNan::new)
             .collect::<Result<_, _>>()?;
         let key = ShapeKey::Interp(knots, controls, degree);
         Ok(Self(get_shape_instance(key)))
     }
 
-    pub fn sample_array(&self, x0: f64, dx: f64, array: &mut [f64]) {
+    pub(crate) fn sample_array(&self, x0: f64, dx: f64, array: &mut [f64]) {
         self.0.sample_array(x0, dx, array);
     }
 }
 
 impl Hash for Shape {
     fn hash<H: std::hash::Hasher>(&self, state: &mut H) {
         Arc::as_ptr(&self.0).hash(state);
```

### Comparing `bosing-2.0.1/tests/test_basic.py` & `bosing-2.0.2/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.1/Cargo.lock` & `bosing-2.0.2/Cargo.lock`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,20 @@
 [[package]]
 name = "allocator-api2"
 version = "0.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c6cb57a04249c6480766f7f7cef5467412af1490f8d1e243141daddada3264f"
 
 [[package]]
+name = "anstyle"
+version = "1.0.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "038dfcf04a5feb68e9c60b21c9625a54c2c0616e79b72b0fd87075a056ae1d1b"
+
+[[package]]
 name = "anyhow"
 version = "1.0.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f538837af36e6f6a9be0faa67f9a314f8119e4e4b5867c6ab40ed60360142519"
 
 [[package]]
 name = "autocfg"
@@ -36,29 +42,32 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bosing"
-version = "2.0.1"
+version = "2.0.2"
 dependencies = [
  "anyhow",
  "bspline",
  "cached",
  "float-cmp",
  "hashbrown",
  "indoc",
  "itertools",
+ "mockall",
  "ndarray",
  "num",
  "numpy",
  "ordered-float",
  "pyo3",
  "rayon",
+ "test-case",
+ "thiserror",
 ]
 
 [[package]]
 name = "bspline"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "af7483eaaefe53f63b5b140f639c5ed6749f8e545768803dc5b89f43acb8ee84"
@@ -163,14 +172,20 @@
 dependencies = [
  "darling_core",
  "quote",
  "syn 2.0.58",
 ]
 
 [[package]]
+name = "downcast"
+version = "0.11.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1435fa1053d8b2fbbe9be7e97eca7f33d37b28409959813daefc1446a14247f1"
+
+[[package]]
 name = "either"
 version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a47c1c47d2f5964e29c61246e81db715514cd532db6b5116a25ea3c03d6780a2"
 
 [[package]]
 name = "float-cmp"
@@ -184,14 +199,20 @@
 [[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
 [[package]]
+name = "fragile"
+version = "2.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6c2141d6d6c8512188a7891b4b01590a45f6dac67afb4f255c4124dbb86d4eaa"
+
+[[package]]
 name = "hashbrown"
 version = "0.14.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5274423e17b7c9fc20b6e7e208532f9b19825d82dfd615708b70edd83df41f1"
 dependencies = [
  "ahash",
  "allocator-api2",
@@ -231,14 +252,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ba291022dbbd398a455acf126c1e341954079855bc60dfdda641363bd6922569"
 dependencies = [
  "either",
 ]
 
 [[package]]
+name = "lazy_static"
+version = "1.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
+
+[[package]]
 name = "libc"
 version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
 name = "lock_api"
@@ -266,14 +293,41 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
+name = "mockall"
+version = "0.12.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "43766c2b5203b10de348ffe19f7e54564b64f3d6018ff7648d1e2d6d3a0f0a48"
+dependencies = [
+ "cfg-if",
+ "downcast",
+ "fragile",
+ "lazy_static",
+ "mockall_derive",
+ "predicates",
+ "predicates-tree",
+]
+
+[[package]]
+name = "mockall_derive"
+version = "0.12.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "af7cbce79ec385a1d4f54baa90a76401eb15d9cab93685f62e7e9f942aa00ae2"
+dependencies = [
+ "cfg-if",
+ "proc-macro2",
+ "quote",
+ "syn 2.0.58",
+]
+
+[[package]]
 name = "ndarray"
 version = "0.15.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "adb12d4e967ec485a5f71c6311fe28158e9d6f4bc4a447b474184d0f91a8fa32"
 dependencies = [
  "matrixmultiply",
  "num-complex",
@@ -414,14 +468,40 @@
 [[package]]
 name = "portable-atomic"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
 
 [[package]]
+name = "predicates"
+version = "3.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "68b87bfd4605926cdfefc1c3b5f8fe560e3feca9d5552cf68c466d3d8236c7e8"
+dependencies = [
+ "anstyle",
+ "predicates-core",
+]
+
+[[package]]
+name = "predicates-core"
+version = "1.0.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b794032607612e7abeb4db69adb4e33590fa6cf1149e95fd7cb00e634b92f174"
+
+[[package]]
+name = "predicates-tree"
+version = "1.0.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "368ba315fb8c5052ab692e68a0eefec6ec57b23a36959c14496f0b0df2c0cecf"
+dependencies = [
+ "predicates-core",
+ "termtree",
+]
+
+[[package]]
 name = "proc-macro2"
 version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
 dependencies = [
  "unicode-ident",
 ]
@@ -584,27 +664,66 @@
 [[package]]
 name = "target-lexicon"
 version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
+name = "termtree"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3369f5ac52d5eb6ab48c6b4ffdc8efbcad6b89c765749064ba298f2c68a16a76"
+
+[[package]]
+name = "test-case"
+version = "3.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "eb2550dd13afcd286853192af8601920d959b14c401fcece38071d53bf0768a8"
+dependencies = [
+ "test-case-macros",
+]
+
+[[package]]
+name = "test-case-core"
+version = "3.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "adcb7fd841cd518e279be3d5a3eb0636409487998a4aff22f3de87b81e88384f"
+dependencies = [
+ "cfg-if",
+ "proc-macro2",
+ "quote",
+ "syn 2.0.58",
+]
+
+[[package]]
+name = "test-case-macros"
+version = "3.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5c89e72a01ed4c579669add59014b9a524d609c0c88c6a585ce37485879f6ffb"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.58",
+ "test-case-core",
+]
+
+[[package]]
 name = "thiserror"
-version = "1.0.59"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f0126ad08bff79f29fc3ae6a55cc72352056dfff61e3ff8bb7129476d44b23aa"
+checksum = "579e9083ca58dd9dcf91a9923bb9054071b9ebbd800b342194c9feb0ee89fc18"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.59"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d1cd413b5d558b4c5bf3680e324a6fa5014e7b7c067a51e69dbdf47eb7148b66"
+checksum = "e2470041c06ec3ac1ab38d0356a6119054dedaea53e12fbefc0de730a1c08524"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.58",
 ]
 
 [[package]]
```

### Comparing `bosing-2.0.1/pyproject.toml` & `bosing-2.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bosing-2.0.1/PKG-INFO` & `bosing-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bosing
-Version: 2.0.1
+Version: 2.0.2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
```

