# Comparing `tmp/qtlink-1.2.8.tar.gz` & `tmp/qtlink-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtlink-1.2.8.tar", last modified: Mon Apr 22 07:59:21 2024, max compression
+gzip compressed data, was "qtlink-1.2.9.tar", last modified: Mon Apr 22 11:31:10 2024, max compression
```

## Comparing `qtlink-1.2.8.tar` & `qtlink-1.2.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:21.195845 qtlink-1.2.8/
--rw-rw-rw-   0        0        0     7816 2024-04-03 12:33:35.000000 qtlink-1.2.8/LICENSE
--rw-rw-rw-   0        0        0      466 2024-04-22 07:59:21.195845 qtlink-1.2.8/PKG-INFO
--rw-rw-rw-   0        0        0      405 2024-04-15 02:16:32.000000 qtlink-1.2.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:21.133616 qtlink-1.2.8/qtlink/
--rw-rw-rw-   0        0        0      117 2024-04-10 12:00:18.000000 qtlink-1.2.8/qtlink/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:21.185835 qtlink-1.2.8/qtlink/dialog/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:50:18.000000 qtlink-1.2.8/qtlink/dialog/__init__.py
--rw-rw-rw-   0        0        0     1499 2024-04-22 07:57:00.000000 qtlink-1.2.8/qtlink/dialog/dialog_info.py
--rw-rw-rw-   0        0        0     2060 2024-04-17 13:09:04.000000 qtlink-1.2.8/qtlink/dialog/dialog_table_check.py
--rw-rw-rw-   0        0        0     2096 2024-04-17 13:09:04.000000 qtlink-1.2.8/qtlink/dialog/dialog_table_display.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:21.195845 qtlink-1.2.8/qtlink/mpl_canvas/
--rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.2.8/qtlink/mpl_canvas/__init__.py
--rw-rw-rw-   0        0        0     2601 2024-04-14 15:07:00.000000 qtlink-1.2.8/qtlink/mpl_canvas/mpl_canvas.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:21.195845 qtlink-1.2.8/qtlink/table/
--rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.2.8/qtlink/table/__init__.py
--rw-rw-rw-   0        0        0     7729 2024-04-14 15:07:00.000000 qtlink-1.2.8/qtlink/table/table_controller.py
--rw-rw-rw-   0        0        0     6847 2024-04-14 15:07:00.000000 qtlink-1.2.8/qtlink/table/table_controller_multiple_check.py
--rw-rw-rw-   0        0        0     2822 2024-04-14 15:07:00.000000 qtlink-1.2.8/qtlink/table/table_controller_single_check.py
--rw-rw-rw-   0        0        0     5182 2024-04-18 14:03:24.000000 qtlink-1.2.8/qtlink/util.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:21.195845 qtlink-1.2.8/qtlink/widgets/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:49:33.000000 qtlink-1.2.8/qtlink/widgets/__init__.py
--rw-rw-rw-   0        0        0     2094 2024-04-17 09:07:46.000000 qtlink-1.2.8/qtlink/widgets/drop_widget.py
--rw-rw-rw-   0        0        0     2073 2024-04-14 14:01:58.000000 qtlink-1.2.8/qtlink/widgets/list_widget.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:21.195845 qtlink-1.2.8/qtlink.egg-info/
--rw-rw-rw-   0        0        0      466 2024-04-22 07:59:21.000000 qtlink-1.2.8/qtlink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      639 2024-04-22 07:59:21.000000 qtlink-1.2.8/qtlink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 07:59:21.000000 qtlink-1.2.8/qtlink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-22 07:59:21.000000 qtlink-1.2.8/qtlink.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-22 07:59:21.000000 qtlink-1.2.8/qtlink.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-22 07:59:21.195845 qtlink-1.2.8/setup.cfg
--rw-rw-rw-   0        0        0      637 2024-04-22 07:57:08.000000 qtlink-1.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 11:31:10.722250 qtlink-1.2.9/
+-rw-rw-rw-   0        0        0     7816 2024-04-03 12:33:35.000000 qtlink-1.2.9/LICENSE
+-rw-rw-rw-   0        0        0      466 2024-04-22 11:31:10.722250 qtlink-1.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2024-04-15 02:16:32.000000 qtlink-1.2.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-22 11:31:10.549476 qtlink-1.2.9/qtlink/
+-rw-rw-rw-   0        0        0      117 2024-04-10 12:00:18.000000 qtlink-1.2.9/qtlink/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 11:31:10.628052 qtlink-1.2.9/qtlink/dialog/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:50:18.000000 qtlink-1.2.9/qtlink/dialog/__init__.py
+-rw-rw-rw-   0        0        0     1499 2024-04-22 07:57:00.000000 qtlink-1.2.9/qtlink/dialog/dialog_info.py
+-rw-rw-rw-   0        0        0     2060 2024-04-17 13:09:04.000000 qtlink-1.2.9/qtlink/dialog/dialog_table_check.py
+-rw-rw-rw-   0        0        0     2096 2024-04-17 13:09:04.000000 qtlink-1.2.9/qtlink/dialog/dialog_table_display.py
+drwxrwxrwx   0        0        0        0 2024-04-22 11:31:10.643678 qtlink-1.2.9/qtlink/mpl_canvas/
+-rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.2.9/qtlink/mpl_canvas/__init__.py
+-rw-rw-rw-   0        0        0     2601 2024-04-14 15:07:00.000000 qtlink-1.2.9/qtlink/mpl_canvas/mpl_canvas.py
+drwxrwxrwx   0        0        0        0 2024-04-22 11:31:10.674911 qtlink-1.2.9/qtlink/table/
+-rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.2.9/qtlink/table/__init__.py
+-rw-rw-rw-   0        0        0     8347 2024-04-22 11:27:28.000000 qtlink-1.2.9/qtlink/table/table_controller.py
+-rw-rw-rw-   0        0        0     6847 2024-04-14 15:07:00.000000 qtlink-1.2.9/qtlink/table/table_controller_multiple_check.py
+-rw-rw-rw-   0        0        0     2822 2024-04-14 15:07:00.000000 qtlink-1.2.9/qtlink/table/table_controller_single_check.py
+-rw-rw-rw-   0        0        0     5182 2024-04-18 14:03:24.000000 qtlink-1.2.9/qtlink/util.py
+drwxrwxrwx   0        0        0        0 2024-04-22 11:31:10.722250 qtlink-1.2.9/qtlink/widgets/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:49:33.000000 qtlink-1.2.9/qtlink/widgets/__init__.py
+-rw-rw-rw-   0        0        0     2094 2024-04-17 09:07:46.000000 qtlink-1.2.9/qtlink/widgets/drop_widget.py
+-rw-rw-rw-   0        0        0     2073 2024-04-14 14:01:58.000000 qtlink-1.2.9/qtlink/widgets/list_widget.py
+drwxrwxrwx   0        0        0        0 2024-04-22 11:31:10.722250 qtlink-1.2.9/qtlink.egg-info/
+-rw-rw-rw-   0        0        0      466 2024-04-22 11:31:10.000000 qtlink-1.2.9/qtlink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      639 2024-04-22 11:31:10.000000 qtlink-1.2.9/qtlink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 11:31:10.000000 qtlink-1.2.9/qtlink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-22 11:31:10.000000 qtlink-1.2.9/qtlink.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-22 11:31:10.000000 qtlink-1.2.9/qtlink.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-22 11:31:10.722250 qtlink-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      637 2024-04-22 11:29:01.000000 qtlink-1.2.9/setup.py
```

### Comparing `qtlink-1.2.8/LICENSE` & `qtlink-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.8/qtlink/dialog/dialog_info.py` & `qtlink-1.2.9/qtlink/dialog/dialog_info.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.8/qtlink/dialog/dialog_table_check.py` & `qtlink-1.2.9/qtlink/dialog/dialog_table_check.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.8/qtlink/dialog/dialog_table_display.py` & `qtlink-1.2.9/qtlink/dialog/dialog_table_display.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.8/qtlink/mpl_canvas/mpl_canvas.py` & `qtlink-1.2.9/qtlink/mpl_canvas/mpl_canvas.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.8/qtlink/table/table_controller.py` & `qtlink-1.2.9/qtlink/table/table_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,36 +34,51 @@
         if highlight_hover_row:
             self.tableview.setMouseTracking(True)
             self.hover_delegate = HoverDelegate(tableview=tableview)
             self.tableview.entered.connect(self.hover_delegate.on_entered)
         else:
             self.hover_delegate = None
 
-    def update_table_data(self, table_data: list[dict], hide_columns: list[str] = None):
+    def update_table_data(self,
+                          table_data: list[dict] = None,
+                          hide_columns: list[str] = None,
+                          init_columns: list[str] = None):
         """更新表格数据
         :param table_data: 原始表格数据，表格中的每一行数据都应使用字典格式，其中的键将按顺序自动识别为表格的列名。
         :param hide_columns: 需要隐藏/不显示的列名。
+        :param init_columns: 用于无数据时初始化显示表头。
         """
-        self.before_update_table_data(table_data, hide_columns=hide_columns)
+        if table_data is None:
+            table_data = []
+        self.before_update_table_data(table_data, hide_columns=hide_columns, init_columns=init_columns)
 
         for data in table_data:
             items = [QStandardItem(str(data.get(column, None)) if data.get(column, None) is not None else '')
                      for column in self.table_columns]
             self.model.appendRow(items)
 
         self.set_table()
 
-    def before_update_table_data(self, table_data, hide_columns: list[str] = None):
+    def before_update_table_data(self,
+                                 table_data: list[dict],
+                                 hide_columns: list[str] = None,
+                                 init_columns: list[str] = None):
         if not self.first_load:
             # 保存当前列宽
             self.save_current_column_widths()
         self.first_load = False
         self.raw_data = table_data
         # 传入空列表将同步清空表头，传入只有键无值的结构才保持显示表头，而无表格数据。
-        self.table_columns = self.get_table_columns_from_data(table_data, hide_columns=hide_columns)
+
+        if table_data:
+            self.table_columns = self.get_table_columns_from_data(table_data, hide_columns=hide_columns)
+        elif not table_data and init_columns:
+            self.table_columns = init_columns
+        else:
+            raise ValueError('表头设置错误')
         self.model.clear()
 
     def set_table(self):
         self.model.setHorizontalHeaderLabels(self.table_columns)
         self.tableview.setModel(self.model)
 
         if self.column_widths is not None:
```

### Comparing `qtlink-1.2.8/qtlink/table/table_controller_multiple_check.py` & `qtlink-1.2.9/qtlink/table/table_controller_multiple_check.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.8/qtlink/table/table_controller_single_check.py` & `qtlink-1.2.9/qtlink/table/table_controller_single_check.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.8/qtlink/util.py` & `qtlink-1.2.9/qtlink/util.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.8/qtlink/widgets/drop_widget.py` & `qtlink-1.2.9/qtlink/widgets/drop_widget.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.8/qtlink/widgets/list_widget.py` & `qtlink-1.2.9/qtlink/widgets/list_widget.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.8/qtlink.egg-info/SOURCES.txt` & `qtlink-1.2.9/qtlink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.8/setup.py` & `qtlink-1.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="qtlink",
-    version="1.2.8",
+    version="1.2.9",
     author="NanHaiLoong",
     author_email="nanhai@163.com",
     description="a ui framework based on pyside6",
     long_description='a ui framework based on pyside6',
     long_description_content_type="text/markdown",
     url="https://gitee.com/darlingxyz/qtlink",
     install_requires=['PySide6'],
```

