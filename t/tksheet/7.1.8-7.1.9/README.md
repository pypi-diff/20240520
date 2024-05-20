# Comparing `tmp/tksheet-7.1.8.tar.gz` & `tmp/tksheet-7.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tksheet-7.1.8.tar", last modified: Thu Apr 18 17:47:17 2024, max compression
+gzip compressed data, was "tksheet-7.1.9.tar", last modified: Sun Apr 21 17:20:29 2024, max compression
```

## Comparing `tksheet-7.1.8.tar` & `tksheet-7.1.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2024-04-18 17:47:17.832809 tksheet-7.1.8/
--rw-rw-r--   0 rg        (1000) rg        (1000)     1101 2024-01-20 17:50:45.000000 tksheet-7.1.8/LICENSE.txt
--rw-r--r--   0 rg        (1000) rg        (1000)     6013 2024-04-18 17:47:17.832809 tksheet-7.1.8/PKG-INFO
--rw-rw-r--   0 rg        (1000) rg        (1000)     3914 2024-01-30 18:05:54.000000 tksheet-7.1.8/README.md
--rw-rw-r--   0 rg        (1000) rg        (1000)     1099 2024-04-09 11:49:17.000000 tksheet-7.1.8/pyproject.toml
--rw-rw-r--   0 rg        (1000) rg        (1000)       38 2024-04-18 17:47:17.832809 tksheet-7.1.8/setup.cfg
-drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2024-04-18 17:47:17.828809 tksheet-7.1.8/tksheet/
--rw-rw-r--   0 rg        (1000) rg        (1000)     1994 2024-04-17 16:38:46.000000 tksheet-7.1.8/tksheet/__init__.py
--rw-rw-r--   0 rg        (1000) rg        (1000)    51594 2024-01-25 08:44:04.000000 tksheet-7.1.8/tksheet/colors.py
--rw-rw-r--   0 rg        (1000) rg        (1000)   100204 2024-04-18 17:26:28.000000 tksheet-7.1.8/tksheet/column_headers.py
--rw-rw-r--   0 rg        (1000) rg        (1000)    10037 2024-01-25 08:44:04.000000 tksheet-7.1.8/tksheet/formatters.py
--rw-rw-r--   0 rg        (1000) rg        (1000)    39709 2024-04-16 16:58:22.000000 tksheet-7.1.8/tksheet/functions.py
--rw-rw-r--   0 rg        (1000) rg        (1000)   318290 2024-04-18 17:24:33.000000 tksheet-7.1.8/tksheet/main_table.py
--rw-rw-r--   0 rg        (1000) rg        (1000)    13628 2024-04-18 07:38:29.000000 tksheet-7.1.8/tksheet/other_classes.py
--rw-rw-r--   0 rg        (1000) rg        (1000)   105673 2024-04-18 17:25:32.000000 tksheet-7.1.8/tksheet/row_index.py
--rw-rw-r--   0 rg        (1000) rg        (1000)   257298 2024-04-18 17:34:24.000000 tksheet-7.1.8/tksheet/sheet.py
--rw-rw-r--   0 rg        (1000) rg        (1000)    11978 2024-04-04 14:40:28.000000 tksheet-7.1.8/tksheet/sheet_options.py
--rw-rw-r--   0 rg        (1000) rg        (1000)     6681 2024-03-30 19:35:35.000000 tksheet-7.1.8/tksheet/text_editor.py
--rw-rw-r--   0 rg        (1000) rg        (1000)    13398 2024-03-19 10:12:20.000000 tksheet-7.1.8/tksheet/themes.py
--rw-rw-r--   0 rg        (1000) rg        (1000)     8275 2024-02-08 18:45:37.000000 tksheet-7.1.8/tksheet/top_left_rectangle.py
--rw-rw-r--   0 rg        (1000) rg        (1000)      340 2024-01-25 08:44:04.000000 tksheet-7.1.8/tksheet/types.py
--rw-rw-r--   0 rg        (1000) rg        (1000)     2288 2024-04-18 17:22:58.000000 tksheet-7.1.8/tksheet/vars.py
-drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2024-04-18 17:47:17.832809 tksheet-7.1.8/tksheet.egg-info/
--rw-r--r--   0 rg        (1000) rg        (1000)     6013 2024-04-18 17:47:17.000000 tksheet-7.1.8/tksheet.egg-info/PKG-INFO
--rw-rw-r--   0 rg        (1000) rg        (1000)      481 2024-04-18 17:47:17.000000 tksheet-7.1.8/tksheet.egg-info/SOURCES.txt
--rw-rw-r--   0 rg        (1000) rg        (1000)        1 2024-04-18 17:47:17.000000 tksheet-7.1.8/tksheet.egg-info/dependency_links.txt
--rw-rw-r--   0 rg        (1000) rg        (1000)        8 2024-04-18 17:47:17.000000 tksheet-7.1.8/tksheet.egg-info/top_level.txt
+drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2024-04-21 17:20:29.001799 tksheet-7.1.9/
+-rw-rw-r--   0 rg        (1000) rg        (1000)     1101 2024-01-20 17:50:45.000000 tksheet-7.1.9/LICENSE.txt
+-rw-r--r--   0 rg        (1000) rg        (1000)     6013 2024-04-21 17:20:28.997799 tksheet-7.1.9/PKG-INFO
+-rw-rw-r--   0 rg        (1000) rg        (1000)     3914 2024-01-30 18:05:54.000000 tksheet-7.1.9/README.md
+-rw-rw-r--   0 rg        (1000) rg        (1000)     1099 2024-04-18 17:49:38.000000 tksheet-7.1.9/pyproject.toml
+-rw-rw-r--   0 rg        (1000) rg        (1000)       38 2024-04-21 17:20:29.001799 tksheet-7.1.9/setup.cfg
+drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2024-04-21 17:20:28.997799 tksheet-7.1.9/tksheet/
+-rw-rw-r--   0 rg        (1000) rg        (1000)     1994 2024-04-18 17:49:41.000000 tksheet-7.1.9/tksheet/__init__.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)    51594 2024-01-25 08:44:04.000000 tksheet-7.1.9/tksheet/colors.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)   100204 2024-04-18 17:26:28.000000 tksheet-7.1.9/tksheet/column_headers.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)    10037 2024-01-25 08:44:04.000000 tksheet-7.1.9/tksheet/formatters.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)    39697 2024-04-19 13:45:43.000000 tksheet-7.1.9/tksheet/functions.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)   318310 2024-04-21 14:51:11.000000 tksheet-7.1.9/tksheet/main_table.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)    13628 2024-04-18 07:38:29.000000 tksheet-7.1.9/tksheet/other_classes.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)   105673 2024-04-18 17:25:32.000000 tksheet-7.1.9/tksheet/row_index.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)   258919 2024-04-21 14:40:22.000000 tksheet-7.1.9/tksheet/sheet.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)    11978 2024-04-20 18:10:51.000000 tksheet-7.1.9/tksheet/sheet_options.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)     6681 2024-03-30 19:35:35.000000 tksheet-7.1.9/tksheet/text_editor.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)    13398 2024-03-19 10:12:20.000000 tksheet-7.1.9/tksheet/themes.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)     8275 2024-02-08 18:45:37.000000 tksheet-7.1.9/tksheet/top_left_rectangle.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)      340 2024-01-25 08:44:04.000000 tksheet-7.1.9/tksheet/types.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)     2288 2024-04-18 17:22:58.000000 tksheet-7.1.9/tksheet/vars.py
+drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2024-04-21 17:20:28.997799 tksheet-7.1.9/tksheet.egg-info/
+-rw-r--r--   0 rg        (1000) rg        (1000)     6013 2024-04-21 17:20:28.000000 tksheet-7.1.9/tksheet.egg-info/PKG-INFO
+-rw-rw-r--   0 rg        (1000) rg        (1000)      481 2024-04-21 17:20:28.000000 tksheet-7.1.9/tksheet.egg-info/SOURCES.txt
+-rw-rw-r--   0 rg        (1000) rg        (1000)        1 2024-04-21 17:20:28.000000 tksheet-7.1.9/tksheet.egg-info/dependency_links.txt
+-rw-rw-r--   0 rg        (1000) rg        (1000)        8 2024-04-21 17:20:28.000000 tksheet-7.1.9/tksheet.egg-info/top_level.txt
```

### Comparing `tksheet-7.1.8/LICENSE.txt` & `tksheet-7.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tksheet-7.1.8/PKG-INFO` & `tksheet-7.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tksheet
-Version: 7.1.8
+Version: 7.1.9
 Summary: Tkinter table / sheet widget
 Author-email: ragardner <github@ragardner.simplelogin.com>
 License: Copyright (c) 2019 ragardner and open source contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `tksheet-7.1.8/README.md` & `tksheet-7.1.9/README.md`

 * *Files identical despite different names*

### Comparing `tksheet-7.1.8/pyproject.toml` & `tksheet-7.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tksheet"
 description = "Tkinter table / sheet widget"
 readme = "README.md"
-version = "7.1.8"
+version = "7.1.9"
 authors = [{ name = "ragardner", email = "github@ragardner.simplelogin.com" }]
 requires-python = ">=3.8"
 license = {file = "LICENSE.txt"}
 keywords = ["tkinter", "table", "widget", "sheet", "grid", "tk"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
```

### Comparing `tksheet-7.1.8/tksheet/__init__.py` & `tksheet-7.1.9/tksheet/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ruff: noqa: F401
 
 """
 tksheet - A Python tkinter table widget
 """
 
-__version__ = "7.1.8"
+__version__ = "7.1.9"
 
 from .colors import (
     color_map,
 )
 from .column_headers import ColumnHeaders
 from .formatters import (
     Formatter,
```

### Comparing `tksheet-7.1.8/tksheet/colors.py` & `tksheet-7.1.9/tksheet/colors.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.1.8/tksheet/column_headers.py` & `tksheet-7.1.9/tksheet/column_headers.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.1.8/tksheet/formatters.py` & `tksheet-7.1.9/tksheet/formatters.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.1.8/tksheet/functions.py` & `tksheet-7.1.9/tksheet/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -610,15 +610,15 @@
 
 
 def try_binding(
     binding: None | Callable,
     event: dict,
     new_name: None | str = None,
 ) -> bool:
-    if binding is not None:
+    if binding:
         try:
             if new_name is None:
                 binding(event)
             else:
                 binding(change_eventname(event, new_name))
         except Exception:
             return False
```

### Comparing `tksheet-7.1.8/tksheet/main_table.py` & `tksheet-7.1.9/tksheet/main_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -1126,15 +1126,19 @@
             disp_new_idxs = get_new_indexes(
                 seqlen=len(self.row_positions) - 1,
                 move_to=move_to,
                 to_move=to_move,
             )
         else:
             disp_new_idxs = {}
-        totalrows = self.fix_data_len(move_to)
+        self.fix_data_len(move_to)
+        totalrows = max(
+            self.total_data_rows(),
+            len(self.row_positions) - 1,
+        )
         if self.all_rows_displayed or data_indexes:
             data_new_idxs = get_new_indexes(seqlen=totalrows, move_to=move_to, to_move=to_move)
         elif not self.all_rows_displayed and not data_indexes:
             data_new_idxs = get_new_indexes(seqlen=len(self.displayed_rows), move_to=move_to, to_move=to_move)
             data_old_idxs = dict(zip(data_new_idxs.values(), data_new_idxs))
             data_new_idxs = dict(
                 zip(
@@ -1153,15 +1157,20 @@
         move_data: bool = True,
         create_selections: bool = True,
         data_indexes: bool = False,
         event_data: EventDataDict | None = None,
     ) -> tuple[dict[int, int], dict[int, int], EventDataDict]:
         self.saved_row_heights = {}
         if not isinstance(totalrows, int):
-            totalrows = self.fix_data_len(max(data_new_idxs.values(), default=0))
+            totalrows = max(
+                self.total_data_rows(),
+                len(self.row_positions) - 1,
+                max(data_new_idxs.values(), default=0),
+            )
+            totalrows = self.fix_data_len(totalrows)
         if event_data is None:
             event_data = event_dict(
                 name="move_rows",
                 sheet=self.PAR.name,
                 boxes=self.get_boxes(),
                 selected=self.selected,
             )
@@ -1440,17 +1449,15 @@
         saved_cells = False
 
         if modification["added"]["rows"] or modification["added"]["columns"]:
             event_data = self.save_cells_using_modification(modification, event_data)
             saved_cells = True
 
         if modification["moved"]["columns"]:
-            totalcols = self.equalize_data_row_lengths()
-            if totalcols < (mx_k := max(modification["moved"]["columns"]["data"].values())):
-                totalcols = mx_k
+            totalcols = max(self.equalize_data_row_lengths(), max(modification["moved"]["columns"]["data"].values()))
             data_new_idxs, disp_new_idxs, event_data = self.move_columns_adjust_options_dict(
                 data_new_idxs=dict(
                     zip(
                         modification["moved"]["columns"]["data"].values(),
                         modification["moved"]["columns"]["data"],
                     )
                 ),
@@ -1467,17 +1474,15 @@
             event_data["moved"]["columns"] = {
                 "data": data_new_idxs,
                 "displayed": disp_new_idxs,
             }
             self.restore_options_named_spans(modification)
 
         if modification["moved"]["rows"]:
-            totalrows = self.total_data_rows()
-            if totalrows < (mx_k := max(modification["moved"]["rows"]["data"].values())):
-                totalrows = mx_k
+            totalrows = max(self.total_data_rows(), max(modification["moved"]["rows"]["data"].values()))
             data_new_idxs, disp_new_idxs, event_data = self.move_rows_adjust_options_dict(
                 data_new_idxs=dict(
                     zip(
                         modification["moved"]["rows"]["data"].values(),
                         modification["moved"]["rows"]["data"],
                     )
                 ),
@@ -2741,46 +2746,48 @@
         self.RI.rsz_w = None
         self.RI.rsz_h = None
         self.CH.rsz_w = None
         self.CH.rsz_h = None
 
     def mouse_motion(self, event: object):
         self.reset_mouse_motion_creations()
-        if self.extra_motion_func:
-            self.extra_motion_func(event)
+        try_binding(self.extra_motion_func, event)
 
     def not_currently_resizing(self) -> bool:
         return all(v is None for v in (self.RI.rsz_h, self.RI.rsz_w, self.CH.rsz_h, self.CH.rsz_w))
 
     def rc(self, event=None):
         self.mouseclick_outside_editor_or_dropdown_all_canvases()
         self.focus_set()
         popup_menu = None
         if (self.single_selection_enabled or self.toggle_selection_enabled) and self.not_currently_resizing():
             r = self.identify_row(y=event.y)
             c = self.identify_col(x=event.x)
             if r < len(self.row_positions) - 1 and c < len(self.col_positions) - 1:
-                if self.col_selected(c) and self.rc_popup_menus_enabled:
-                    popup_menu = self.CH.ch_rc_popup_menu
-                elif self.row_selected(r) and self.rc_popup_menus_enabled:
-                    popup_menu = self.RI.ri_rc_popup_menu
-                elif self.cell_selected(r, c) and self.rc_popup_menus_enabled:
-                    popup_menu = self.rc_popup_menu
+                if self.col_selected(c):
+                    if self.rc_popup_menus_enabled:
+                        popup_menu = self.CH.ch_rc_popup_menu
+                elif self.row_selected(r):
+                    if self.rc_popup_menus_enabled:
+                        popup_menu = self.RI.ri_rc_popup_menu
+                elif self.cell_selected(r, c):
+                    if self.rc_popup_menus_enabled:
+                        popup_menu = self.rc_popup_menu
                 else:
                     if self.rc_select_enabled:
                         if self.single_selection_enabled:
                             self.select_cell(r, c, redraw=True)
                         elif self.toggle_selection_enabled:
                             self.toggle_select_cell(r, c, redraw=True)
                     if self.rc_popup_menus_enabled:
                         popup_menu = self.rc_popup_menu
             else:
+                self.deselect("all")
                 popup_menu = self.empty_rc_popup_menu
-        if self.extra_rc_func:
-            self.extra_rc_func(event)
+        try_binding(self.extra_rc_func, event)
         if popup_menu is not None:
             popup_menu.tk_popup(event.x_root, event.y_root)
 
     def b1_press(self, event=None):
         self.closed_dropdown = self.mouseclick_outside_editor_or_dropdown_all_canvases()
         self.focus_set()
         if (
@@ -2796,16 +2803,15 @@
                 self.being_drawn_item = self.select_cell(r, c, redraw=True)
         elif self.toggle_selection_enabled and self.not_currently_resizing():
             r = self.identify_row(y=event.y)
             c = self.identify_col(x=event.x)
             if r < len(self.row_positions) - 1 and c < len(self.col_positions) - 1:
                 self.toggle_select_cell(r, c, redraw=True)
         self.b1_pressed_loc = (r, c)
-        if self.extra_b1_press_func:
-            self.extra_b1_press_func(event)
+        try_binding(self.extra_b1_press_func, event)
 
     def create_resize_line(self, x1, y1, x2, y2, width, fill, tag):
         if self.hidd_resize_lines:
             t, sh = self.hidd_resize_lines.popitem()
             self.coords(t, x1, y1, x2, y2)
             if sh:
                 self.itemconfig(t, width=width, fill=fill, tag=tag)
@@ -2965,16 +2971,15 @@
                     if self.drag_selection_binding_func:
                         self.drag_selection_binding_func(sel_event)
                     self.PAR.emit_event("<<SheetSelect>>", data=sel_event)
             if self.scroll_if_event_offscreen(event):
                 need_redraw = True
             if need_redraw:
                 self.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True, redraw_table=True)
-        if self.extra_b1_motion_func:
-            self.extra_b1_motion_func(event)
+        try_binding(self.extra_b1_motion_func, event)
 
     def ctrl_b1_motion(self, event: object):
         if self.ctrl_select_enabled and self.drag_selection_enabled and self.not_currently_resizing():
             need_redraw = False
             end_row = self.identify_row(y=event.y)
             end_col = self.identify_col(x=event.x)
             if (
@@ -3078,16 +3083,15 @@
                         and self.canvasy(event.y) < self.row_positions[r] + self.table_txt_height + 4
                     ):
                         self.open_cell(event)
             else:
                 self.mouseclick_outside_editor_or_dropdown_all_canvases()
         self.b1_pressed_loc = None
         self.closed_dropdown = None
-        if self.extra_b1_release_func:
-            self.extra_b1_release_func(event)
+        try_binding(self.extra_b1_release_func, event)
 
     def double_b1(self, event=None):
         self.mouseclick_outside_editor_or_dropdown_all_canvases()
         self.focus_set()
         if (
             self.identify_col(x=event.x, allow_end=False) is None
             or self.identify_row(y=event.y, allow_end=False) is None
@@ -3103,16 +3107,15 @@
         elif self.toggle_selection_enabled and self.not_currently_resizing():
             r = self.identify_row(y=event.y)
             c = self.identify_col(x=event.x)
             if r < len(self.row_positions) - 1 and c < len(self.col_positions) - 1:
                 self.toggle_select_cell(r, c, redraw=True)
                 if self.edit_cell_enabled:
                     self.open_cell(event)
-        if self.extra_double_b1_func:
-            self.extra_double_b1_func(event)
+        try_binding(self.extra_double_b1_func, event)
 
     def identify_row(self, event=None, y=None, allow_end=True):
         if event is None:
             y2 = self.canvasy(y)
         elif y is None:
             y2 = self.canvasy(event.y)
         r = bisect_left(self.row_positions, y2)
@@ -3325,15 +3328,17 @@
                         (
                             (
                                 self.min_row_height
                                 if h == old_min_row_height
                                 else (
                                     default_row_height
                                     if h == old_default_row_height
-                                    else self.min_row_height if h < self.min_row_height else h
+                                    else self.min_row_height
+                                    if h < self.min_row_height
+                                    else h
                                 )
                             )
                             for h in self.gen_row_heights()
                         ),
                     )
                 )
             )
@@ -4270,15 +4275,15 @@
             "header": header,
             "column_widths": column_widths,
             "displayed_columns": saved_displayed_columns,
         }
         return event_data
 
     def rc_add_columns(self, event: object = None):
-        rowlen = self.equalize_data_row_lengths(include_header=False)
+        rowlen = self.equalize_data_row_lengths()
         selcols = sorted(self.get_selected_cols())
         if (
             selcols
             and isinstance(self.CH.popup_menu_loc, int)
             and selcols[0] <= self.CH.popup_menu_loc
             and selcols[-1] >= self.CH.popup_menu_loc
         ):
@@ -4856,32 +4861,23 @@
         else:
             if not isinstance(self._row_index, int) and index is not None and isinstance(index, int):
                 return self._row_index[index]
             else:
                 return self._row_index
 
     def total_data_cols(self, include_header: bool = True) -> int:
-        h_total = 0
-        d_total = 0
-        if include_header:
-            if isinstance(self._headers, (list, tuple)):
-                h_total = len(self._headers)
-        # map() for some reason is 15% faster than max(key=len)
-        # using python 3.11 windows 11
+        h_total = len(self._headers) if include_header and isinstance(self._headers, (list, tuple)) else 0
+        # map() for some reason is 15% faster than max(key=len) using python 3.11 windows 11
         d_total = max(map(len, self.data), default=0)
-        return h_total if h_total > d_total else d_total
+        return max(h_total, d_total)
 
     def total_data_rows(self, include_index: bool = True) -> int:
-        i_total = 0
-        d_total = 0
-        if include_index:
-            if isinstance(self._row_index, (list, tuple)):
-                i_total = len(self._row_index)
+        i_total = len(self._row_index) if include_index and isinstance(self._row_index, (list, tuple)) else 0
         d_total = len(self.data)
-        return i_total if i_total > d_total else d_total
+        return max(i_total, d_total)
 
     def data_dimensions(self, total_rows: int | None = None, total_columns: int | None = None):
         if total_rows is None and total_columns is None:
             return self.total_data_rows(), self.total_data_cols()
         if total_rows is not None:
             if len(self.data) < total_rows:
                 ncols = self.total_data_cols() if total_columns is None else total_columns
@@ -4893,22 +4889,23 @@
                 if (lnr := len(r)) > total_columns:
                     r = r[:total_columns]
                 elif lnr < total_columns:
                     r += self.get_empty_row_seq(rn, end=total_columns, start=lnr)
 
     def equalize_data_row_lengths(
         self,
-        include_header: bool = False,
+        include_header: bool = True,
         total_data_cols: int | None = None,
         at_least_cols: int | None = None,
     ) -> int:
         if not isinstance(total_data_cols, int):
             total_data_cols = self.total_data_cols(include_header=include_header)
         if isinstance(at_least_cols, int) and at_least_cols > total_data_cols:
             total_data_cols = at_least_cols
+        total_data_cols = max(total_data_cols, len(self.col_positions) - 1)
         if include_header and total_data_cols > len(self._headers):
             self.CH.fix_header(total_data_cols)
         for rn, r in enumerate(self.data):
             if total_data_cols > (lnr := len(r)):
                 r += self.get_empty_row_seq(rn, end=total_data_cols, start=lnr)
         return total_data_cols
```

### Comparing `tksheet-7.1.8/tksheet/other_classes.py` & `tksheet-7.1.9/tksheet/other_classes.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.1.8/tksheet/row_index.py` & `tksheet-7.1.9/tksheet/row_index.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.1.8/tksheet/sheet.py` & `tksheet-7.1.9/tksheet/sheet.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 from .other_classes import (
     DotDict,
     EventDataDict,
     FontTuple,
     GeneratedMouseEvent,
     Node,
     Selected,
+    SelectionBox,
     Span,
 )
 from .row_index import RowIndex
 from .sheet_options import (
     new_sheet_options,
 )
 from .themes import (
@@ -1066,14 +1067,25 @@
         self.MT.undo(event)
         return self
 
     def redo(self, event: object = None) -> Sheet:
         self.MT.redo(event)
         return self
 
+    def has_focus(
+        self,
+    ) -> bool:
+        """
+        Check if any Sheet widgets have focus
+        Includes child widgets such as scroll bars
+        Returns bool
+        """
+        widget = self.focus_get()
+        return widget == self or any(widget == c for c in self.children.values())
+
     def focus_set(
         self,
         canvas: Literal[
             "table",
             "header",
             "row_index",
             "index",
@@ -1387,19 +1399,15 @@
                 res = res[0][0]
             # it's a single list
             elif len(res) == 1:
                 res = res[0]
             # retrieving a list of index cells or
             elif (index and not span.transposed and not table and not header) or (
                 # it's a column that's spread across sublists
-                table
-                and res
-                and not span.transposed
-                and len(res[0]) == 1
-                and len(res[-1]) == 1
+                table and res and not span.transposed and len(res[0]) == 1 and len(res[-1]) == 1
             ):
                 res = list(chain.from_iterable(res))
         elif span.ndim == 1:
             # flatten sublists
             if len(res) == 1 and len(res[0]) == 1:
                 res = res[0]
             else:
@@ -2385,16 +2393,39 @@
         if undo:
             self.MT.undo_stack.append(ev_stack_dict(event_data))
         if emit_event:
             self.emit_event("<<SheetModified>>", event_data)
         self.set_refresh_timer(redraw)
         return data_idxs, disp_idxs, event_data
 
-    def equalize_data_row_lengths(self, include_header: bool = False) -> int:
-        return self.MT.equalize_data_row_lengths(include_header=include_header)
+    def equalize_data_row_lengths(
+        self,
+        include_header: bool = True,
+    ) -> int:
+        return self.MT.equalize_data_row_lengths(
+            include_header=include_header,
+        )
+
+    def full_move_rows_idxs(self, data_idxs: dict[int, int]) -> dict[int, int]:
+        """
+        Converts the dict provided by moving rows event data
+        Under the keys ['moved']['rows']['data']
+        Into a dict of {old index: new index} for every row
+        Includes row numbers in cell options, spans, etc.
+        """
+        return self.MT.get_full_new_idxs(self.MT.get_max_row_idx(), data_idxs)
+
+    def full_move_columns_idxs(self, data_idxs: dict[int, int]) -> dict[int, int]:
+        """
+        Converts the dict provided by moving columns event data
+        Under the keys ['moved']['columns']['data']
+        Into a dict of {old index: new index} for every column
+        Includes column numbers in cell options, spans, etc.
+        """
+        return self.MT.get_full_new_idxs(self.MT.get_max_column_idx(), data_idxs)
 
     # Highlighting Cells
 
     def highlight(
         self,
         *key: CreateSpanTypes,
         bg: bool | None | str = False,
@@ -2972,14 +3003,18 @@
     def boxes(self, boxes: Sequence[tuple[tuple[int, int, int, int], str]]) -> Sheet:
         self.MT.deselect()
         self.MT.reselect_from_get_boxes(
             boxes={box[0] if isinstance(box[0], tuple) else tuple(box[0]): box[1] for box in boxes}
         )
         return self
 
+    @property
+    def canvas_boxes(self) -> dict[int, SelectionBox]:
+        return self.MT.selection_boxes
+
     def cell_selected(
         self,
         r: int,
         c: int,
         rows: bool = False,
         columns: bool = False,
     ) -> bool:
@@ -3004,16 +3039,25 @@
         ):
             return True
         return False
 
     def all_selected(self) -> bool:
         return self.MT.all_selected()
 
-    def get_ctrl_x_c_boxes(self) -> tuple[dict[tuple[int, int, int, int], str], int]:
-        return self.MT.get_ctrl_x_c_boxes()
+    def get_ctrl_x_c_boxes(
+        self,
+        nrows: bool = True,
+    ) -> tuple[dict[tuple[int, int, int, int], str], int] | dict[tuple[int, int, int, int], str]:
+        if nrows:
+            return self.MT.get_ctrl_x_c_boxes()
+        return self.MT.get_ctrl_x_c_boxes()[0]
+
+    @property
+    def ctrl_boxes(self) -> dict[tuple[int, int, int, int], str]:
+        return self.MT.get_ctrl_x_c_boxes()[0]
 
     def get_selected_min_max(
         self,
     ) -> tuple[int, int, int, int] | tuple[None, None, None, None]:
         """
         Returns (min_y, min_x, max_y, max_x) of all selection boxes
         """
@@ -4462,15 +4506,15 @@
             row_index=True,
             create_selections=False,
             fill=False,
         )
         self.RI.tree_rns = {n.iid: i for i, n in enumerate(self.MT._row_index)}
         self.hide_rows(
             set(self.RI.tree_rns[iid] for iid in self.get_children() if self.RI.tree[iid].parent),
-            deselect_all=True,
+            deselect_all=False,
             data_indexes=True,
         )
         return self
 
     def tree_reset(self) -> Sheet:
         self.deselect()
         self.RI.tree_reset()
@@ -4789,15 +4833,15 @@
         self.show_rows(to_show)
         self.set_refresh_timer(True)
         return self
 
     reattach = move
 
     def exists(self, item: str) -> bool:
-        return item in self.RI.tree
+        return item.lower() in self.RI.tree
 
     def parent(self, item: str) -> str:
         if (item := item.lower()) not in self.RI.tree:
             raise ValueError(f"Item '{item}' does not exist.")
         return self.RI.tree[item].parent.iid if self.RI.tree[item].parent else self.RI.tree[item].parent
 
     def index(self, item: str) -> int:
@@ -5415,15 +5459,15 @@
         self.set_refresh_timer(redraw)
 
     def highlight_cells(
         self,
         row: int = 0,
         column: int = 0,
         cells: list = [],
-        canvas: str = "table",
+        canvas: Literal["table", "index", "header"] = "table",
         bg: bool | None | str = False,
         fg: bool | None | str = False,
         redraw: bool = True,
         overwrite: bool = True,
     ) -> None:
         if bg is False and fg is False:
             return
```

### Comparing `tksheet-7.1.8/tksheet/sheet_options.py` & `tksheet-7.1.9/tksheet/sheet_options.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.1.8/tksheet/text_editor.py` & `tksheet-7.1.9/tksheet/text_editor.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.1.8/tksheet/themes.py` & `tksheet-7.1.9/tksheet/themes.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.1.8/tksheet/top_left_rectangle.py` & `tksheet-7.1.9/tksheet/top_left_rectangle.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.1.8/tksheet/vars.py` & `tksheet-7.1.9/tksheet/vars.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.1.8/tksheet.egg-info/PKG-INFO` & `tksheet-7.1.9/tksheet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tksheet
-Version: 7.1.8
+Version: 7.1.9
 Summary: Tkinter table / sheet widget
 Author-email: ragardner <github@ragardner.simplelogin.com>
 License: Copyright (c) 2019 ragardner and open source contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

