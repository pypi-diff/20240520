# Comparing `tmp/paraview_trame_components-0.6.0.tar.gz` & `tmp/paraview_trame_components-0.7.0.tar.gz`

## Comparing `paraview_trame_components-0.6.0.tar` & `paraview_trame_components-0.7.0.tar`

### file list

```diff
@@ -1,28 +1,31 @@
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/examples/all.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/examples/cone-with-slider.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/examples/cone.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/examples/multi-views.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/examples/pipeline.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/examples/state-loader-slider.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/examples/state-loader.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/examples/test-cols.py
--rw-r--r--   0        0        0     8663 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/examples/wavelet-contour-state.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/ptc/__init__.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/ptc/cli.py
--rw-r--r--   0        0        0     4722 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/ptc/colors.py
--rw-r--r--   0        0        0     4939 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/ptc/core.py
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/ptc/palette.py
--rw-r--r--   0        0        0     4471 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/ptc/pipeline.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/ptc/utils.py
--rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/ptc/vcr.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/ptc/vuetify.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/ptc/assets/__init__.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/ptc/layouts/__init__.py
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/ptc/layouts/col.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/ptc/layouts/factory.py
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/ptc/layouts/side.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/.gitignore
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/LICENSE
--rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/README.md
--rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     4489 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 paraview_trame_components-0.7.0/examples/all.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 paraview_trame_components-0.7.0/examples/cone-with-slider.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 paraview_trame_components-0.7.0/examples/cone.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 paraview_trame_components-0.7.0/examples/multi-views.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 paraview_trame_components-0.7.0/examples/open-file-button.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 paraview_trame_components-0.7.0/examples/open-file.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 paraview_trame_components-0.7.0/examples/pipeline.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 paraview_trame_components-0.7.0/examples/state-loader-slider.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 paraview_trame_components-0.7.0/examples/state-loader.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 paraview_trame_components-0.7.0/examples/test-cols.py
+-rw-r--r--   0        0        0     8663 2020-02-02 00:00:00.000000 paraview_trame_components-0.7.0/examples/wavelet-contour-state.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 paraview_trame_components-0.7.0/ptc/__init__.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 paraview_trame_components-0.7.0/ptc/cli.py
+-rw-r--r--   0        0        0     4722 2020-02-02 00:00:00.000000 paraview_trame_components-0.7.0/ptc/colors.py
+-rw-r--r--   0        0        0     6189 2020-02-02 00:00:00.000000 paraview_trame_components-0.7.0/ptc/core.py
+-rw-r--r--   0        0        0    14829 2020-02-02 00:00:00.000000 paraview_trame_components-0.7.0/ptc/file.py
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 paraview_trame_components-0.7.0/ptc/palette.py
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 paraview_trame_components-0.7.0/ptc/pipeline.py
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 paraview_trame_components-0.7.0/ptc/utils.py
+-rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 paraview_trame_components-0.7.0/ptc/vcr.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 paraview_trame_components-0.7.0/ptc/vuetify.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 paraview_trame_components-0.7.0/ptc/assets/__init__.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 paraview_trame_components-0.7.0/ptc/layouts/__init__.py
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 paraview_trame_components-0.7.0/ptc/layouts/col.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 paraview_trame_components-0.7.0/ptc/layouts/factory.py
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 paraview_trame_components-0.7.0/ptc/layouts/side.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 paraview_trame_components-0.7.0/.gitignore
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 paraview_trame_components-0.7.0/LICENSE
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 paraview_trame_components-0.7.0/README.md
+-rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 paraview_trame_components-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     4489 2020-02-02 00:00:00.000000 paraview_trame_components-0.7.0/PKG-INFO
```

### Comparing `paraview_trame_components-0.6.0/examples/cone-with-slider.py` & `paraview_trame_components-0.7.0/examples/cone-with-slider.py`

 * *Files identical despite different names*

### Comparing `paraview_trame_components-0.6.0/examples/multi-views.py` & `paraview_trame_components-0.7.0/examples/multi-views.py`

 * *Files identical despite different names*

### Comparing `paraview_trame_components-0.6.0/examples/pipeline.py` & `paraview_trame_components-0.7.0/examples/pipeline.py`

 * *Files identical despite different names*

### Comparing `paraview_trame_components-0.6.0/examples/state-loader-slider.py` & `paraview_trame_components-0.7.0/examples/state-loader-slider.py`

 * *Files identical despite different names*

### Comparing `paraview_trame_components-0.6.0/examples/test-cols.py` & `paraview_trame_components-0.7.0/examples/test-cols.py`

 * *Files identical despite different names*

### Comparing `paraview_trame_components-0.6.0/examples/wavelet-contour-state.py` & `paraview_trame_components-0.7.0/examples/wavelet-contour-state.py`

 * *Files identical despite different names*

### Comparing `paraview_trame_components-0.6.0/ptc/colors.py` & `paraview_trame_components-0.7.0/ptc/colors.py`

 * *Files identical despite different names*

### Comparing `paraview_trame_components-0.6.0/ptc/core.py` & `paraview_trame_components-0.7.0/ptc/core.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from paraview import simple
 from trame.app import get_server
 from trame.decorators import TrameApp, change, controller
 from trame.ui.vuetify3 import VAppLayout
 from trame.widgets import html
 from trame.widgets import paraview as pv_widgets
+from trame.widgets import vuetify3 as v3
 
 from .layouts import create_layout_manager
 
 
 class InvalidContainerNameError(Exception):
     def __init__(self, name):
         super().__init__(f"Container {name} not available")
@@ -20,15 +21,18 @@
         self.template_name = template_name
         self.server = get_server(server)
         self.views = views
         self.html_views = []
         self.proxy_views = []
         self.ui = None
         if self.views is None or len(self.views) == 0:
-            self.views = [simple.GetActiveView()]
+            view = simple.GetActiveView()
+            if view is None:
+                view = simple.CreateRenderView()
+            self.views = [view]
 
         if from_state:
             for view in self.views:
                 view.MakeRenderWindowInteractor(True)
 
         self._build_ui()
 
@@ -62,47 +66,66 @@
                     if isinstance(view, list | tuple):
                         with html.Div(
                             classes="d-flex align-stretch fill-height flex-column flex-grow-1 flex-shrink-1"
                         ):
                             for v in view:
                                 view_id = len(self.html_views)
                                 with html.Div(
-                                    classes="flex-grow-1 flex-shrink-1 border-thin",
+                                    classes="flex-grow-1 flex-shrink-1 border-thin position-relative",
                                     style=(
                                         f"{{ overflow: 'hidden', zIndex: 0, padding: '1px', margin: '1px', outline: active_view_id === {view_id} ? 'solid 1.5px blue' : 'none' }}",
                                     ),
                                     click=f"active_view_id = {view_id}",
                                 ):
                                     view_html = pv_widgets.VtkRemoteView(
                                         v,
                                         interactive_ratio=1,
                                         style="z-index: -1;",
                                     )
+                                    v3.VBtn(
+                                        icon="mdi-crop-free",
+                                        click=view_html.reset_camera,
+                                        classes="position-absolute",
+                                        style="top: 1rem;right: 1rem; z-index: 1;",
+                                        variant="outlined",
+                                        size="small",
+                                    )
+                                    self.ctrl.on_data_loaded.add(view_html.reset_camera)
                                     self.ctrl.view_update.add(view_html.update)
                                     self.ctrl.view_reset_camera.add(
                                         view_html.reset_camera
                                     )
                                     self.html_views.append(view_html)
                                     self.proxy_views.append(v)
                     else:
                         view_id = len(self.html_views)
                         with html.Div(
-                            classes="flex-grow-1 flex-shrink-1 border-thin",
+                            classes="flex-grow-1 flex-shrink-1 border-thin position-relative",
                             style=(
                                 f"{{ overflow: 'hidden', zIndex: 0, padding: '1px', margin: '1px', outline: active_view_id === {view_id} ? 'solid 1.5px blue' : 'none' }}",
                             ),
                             click=f"active_view_id = {view_id}",
                         ):
                             view_html = pv_widgets.VtkRemoteView(
                                 view,
                                 interactive_ratio=1,
                                 style="z-index: -1;",
                             )
+                            v3.VBtn(
+                                icon="mdi-crop-free",
+                                click=view_html.reset_camera,
+                                classes="position-absolute",
+                                style="top: 1rem;right: 1rem; z-index: 1;",
+                                variant="outlined",
+                                size="small",
+                            )
+
                             self.ctrl.view_update.add(view_html.update)
                             self.ctrl.view_reset_camera.add(view_html.reset_camera)
+                            self.ctrl.on_data_loaded.add(view_html.reset_camera)
                             self.html_views.append(view_html)
                             self.proxy_views.append(view)
 
     @controller.add("on_data_change")
     def update(self):
         self.ctrl.view_update()
```

### Comparing `paraview_trame_components-0.6.0/ptc/palette.py` & `paraview_trame_components-0.7.0/ptc/palette.py`

 * *Files identical despite different names*

### Comparing `paraview_trame_components-0.6.0/ptc/pipeline.py` & `paraview_trame_components-0.7.0/ptc/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
                     "pointer-events: auto; user-select: none; background: rgba(255, 255, 255, 0.5);",
                 ),
             },
         )
         self._deleted_ids = set()
         self.update()
         self.server.controller.on_active_view_change.add(self.update)
+        self.server.controller.on_data_loaded.add(self.update)
 
     def on_active_change(self, active_ids, **_):
         current_active = simple.GetActiveSource()
         proxy = None
         if len(active_ids):
             _id = active_ids[0]
             if _id in self._deleted_ids:
```

### Comparing `paraview_trame_components-0.6.0/ptc/utils.py` & `paraview_trame_components-0.7.0/ptc/utils.py`

 * *Files identical despite different names*

### Comparing `paraview_trame_components-0.6.0/ptc/vcr.py` & `paraview_trame_components-0.7.0/ptc/vcr.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 
 from paraview import simple
 from trame.app import asynchronous
-from trame.decorators import TrameApp, change
+from trame.decorators import TrameApp, change, controller
 from trame.widgets import html, vuetify3
 
 
 @TrameApp()
 class TimeControl(vuetify3.VCard):
     def __init__(
         self,
@@ -98,26 +98,30 @@
         return self.server.state
 
     @property
     def time_values(self):
         return list(simple.GetTimeKeeper().TimestepValues)
 
     @change("time_index")
+    @controller.add("on_data_loaded")
     def update(self, **_):
         time_values = self.time_values
         self.state.time_nb = len(time_values)
         if self.time_index >= self.state.time_nb:
             self.state.time_index = 0
         if self.time_index < 0:
             self.state.time_index = self.state.time_nb + self.time_index
 
         tk = simple.GetTimeKeeper()
-        self.state.time_value = time_values[self.state.time_index]
-        tk.Time = self.state.time_value
-        self.server.controller.on_data_change()
+        if len(time_values) < 1:
+            self.state.time_value = 0
+        else:
+            self.state.time_value = time_values[self.state.time_index]
+            tk.Time = self.state.time_value
+            self.server.controller.on_data_change()
 
     @property
     def time_index(self):
         return self.state.time_index
 
     def first(self):
         self.state.time_index = 0
```

### Comparing `paraview_trame_components-0.6.0/ptc/layouts/col.py` & `paraview_trame_components-0.7.0/ptc/layouts/col.py`

 * *Files identical despite different names*

### Comparing `paraview_trame_components-0.6.0/ptc/layouts/side.py` & `paraview_trame_components-0.7.0/ptc/layouts/side.py`

 * *Files identical despite different names*

### Comparing `paraview_trame_components-0.6.0/LICENSE` & `paraview_trame_components-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paraview_trame_components-0.6.0/README.md` & `paraview_trame_components-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 ```bash
 # Adjust path to point to your ParaView executable
 export PVPYTHON=/Applications/ParaView-5.12.0.app/Contents/bin/pvpython
 
 # Run the scripts
 $PVPYTHON --force-offscreen-rendering ./examples/cone.py
-$PVPYTHON --force-offscreen-rendering ./examples/cone_width_slider.py
+$PVPYTHON --force-offscreen-rendering ./examples/cone-width-slider.py
 $PVPYTHON --force-offscreen-rendering ./examples/wavelet-contour-state.py
 $PVPYTHON --force-offscreen-rendering ./examples/pipeline.py
 ```
 
 ## Scripts structure
 
 Each script add `import paraview.web.venv` at the top to enable your virtual environment via the `PV_VENV` environment variable.
```

### Comparing `paraview_trame_components-0.6.0/pyproject.toml` & `paraview_trame_components-0.7.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "paraview-trame-components"
-version = "0.6.0"
+version = "0.7.0"
 requires-python = ">= 3.10"
 dependencies = [
   "trame",
   "trame-vtk",
   "trame-vuetify",
   "trame-components",
 ]
@@ -76,14 +76,15 @@
 
 [tool.ruff.lint]
 select = ["ALL"]
 ignore = [
   # ok
   "C408",
   "PLR2004",
+  "SIM117",
   
   # need cleanup
   "ARG001",
   "ANN001",
   "ANN002",
   "ANN003",
   "ANN101",
@@ -111,14 +112,17 @@
 "examples/wavelet*.py" = ["F403", "F405"]
 "examples/*.py" = [
   "INP001",
   "I001", 
   "F401", 
   "E402", 
   "ANN001", "ANN003",
+  "T201",
+  "ERA001",
+  "SIM117",
 ]
 
 
 # -----------------------------------------------------------------------------
 
 [tool.codespell]
 skip = "**/package-lock.json,PKG-INFO,**/dist/**,CHANGELOG.md"
```

### Comparing `paraview_trame_components-0.6.0/PKG-INFO` & `paraview_trame_components-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: paraview-trame-components
-Version: 0.6.0
+Version: 0.7.0
 Summary: Macro components for ParaView
 Author-email: Sebastien Jourdain <sebastien.jourdain@kitware.com>
 Maintainer-email: Sebastien Jourdain <sebastien.jourdain@kitware.com>
 License: Copyright 2024 Kitware Inc.
         
         Licensed under the Apache License, Version 2.0 (the "License");
         you may not use this file except in compliance with the License.
@@ -66,15 +66,15 @@
 
 ```bash
 # Adjust path to point to your ParaView executable
 export PVPYTHON=/Applications/ParaView-5.12.0.app/Contents/bin/pvpython
 
 # Run the scripts
 $PVPYTHON --force-offscreen-rendering ./examples/cone.py
-$PVPYTHON --force-offscreen-rendering ./examples/cone_width_slider.py
+$PVPYTHON --force-offscreen-rendering ./examples/cone-width-slider.py
 $PVPYTHON --force-offscreen-rendering ./examples/wavelet-contour-state.py
 $PVPYTHON --force-offscreen-rendering ./examples/pipeline.py
 ```
 
 ## Scripts structure
 
 Each script add `import paraview.web.venv` at the top to enable your virtual environment via the `PV_VENV` environment variable.
```

