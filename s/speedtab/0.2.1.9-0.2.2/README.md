# Comparing `tmp/speedtab-0.2.1.9.tar.gz` & `tmp/speedtab-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speedtab-0.2.1.9.tar", max compression
+gzip compressed data, was "speedtab-0.2.2.tar", max compression
```

## Comparing `speedtab-0.2.1.9.tar` & `speedtab-0.2.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      567 2024-04-22 14:48:24.759600 speedtab-0.2.1.9/pyproject.toml
--rw-r--r--   0        0        0      382 2023-12-14 09:13:27.273500 speedtab-0.2.1.9/speedtab/__init__.py
--rw-r--r--   0        0        0    88073 2024-04-22 14:48:24.699600 speedtab-0.2.1.9/speedtab/client.py
--rw-r--r--   0        0        0     7739 2023-12-14 09:47:11.439768 speedtab-0.2.1.9/speedtab/enums.py
--rw-r--r--   0        0        0     1824 2023-12-14 09:47:11.343768 speedtab-0.2.1.9/speedtab/formats.py
--rw-r--r--   0        0        0      783 2024-04-22 14:48:54.819719 speedtab-0.2.1.9/setup.py
--rw-r--r--   0        0        0      808 2024-04-22 14:48:54.819719 speedtab-0.2.1.9/PKG-INFO
+-rw-r--r--   0        0        0      565 2024-05-20 11:04:23.399363 speedtab-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      396 2024-05-20 11:03:39.194954 speedtab-0.2.2/speedtab/__init__.py
+-rw-r--r--   0        0        0    88502 2024-05-08 11:32:46.430705 speedtab-0.2.2/speedtab/client.py
+-rw-r--r--   0        0        0     7739 2023-12-14 09:47:11.439768 speedtab-0.2.2/speedtab/enums.py
+-rw-r--r--   0        0        0     1824 2023-12-14 09:47:11.343768 speedtab-0.2.2/speedtab/formats.py
+-rw-r--r--   0        0        0      781 2024-05-20 11:04:36.499879 speedtab-0.2.2/setup.py
+-rw-r--r--   0        0        0      806 2024-05-20 11:04:36.499879 speedtab-0.2.2/PKG-INFO
```

### Comparing `speedtab-0.2.1.9/pyproject.toml` & `speedtab-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "speedtab"
-version = "0.2.1.9"
+version = "0.2.2"
 description = "Convenient wrapper for working with Google Spreadsheets"
 authors = ["Bogdan Gergel <bogger147@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/BoggerSancho/SpeedTab-beta"
 repository = "https://github.com/BoggerSancho/SpeedTab-beta"
 
 [tool.poetry.dependencies]
```

### Comparing `speedtab-0.2.1.9/speedtab/client.py` & `speedtab-0.2.2/speedtab/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -491,16 +491,17 @@
                   y_right_axis_max: float = None,
                   x_scale: int = 1,
                   y_scale: int = 1,
                   offset_x_pixels: int = 0,
                   offset_y_pixels: int = 0,
                   header_count: int = 1,
                   nrows: int = None,
-                  data_sheet_name=None,
-                  data_start=(0, 0)
+                  reverse_axis_order: bool = False,
+                  data_sheet_name: str = None,
+                  data_start: Union[tuple, str] = (0, 0),
                   ):
         """Adds chart to a sheet.
 
         :param columns: A column from which the data for the chart will be taken. Requires an index from data_start param.
         E.g. columns=[1] would mean to select the second column from a given dataset.
         :param target_axis: Defines axis (left only, right only or mixed if you input list), defaults to AxisPosition.LEFT_AXIS.
         :param index_column: Defines from where in the selected dataset the index will be taken for the chart, defaults to 0.
@@ -520,14 +521,15 @@
         :param y_right_axis_max: Sets a maximum value on the y-axis situated on the right, defaults to None.
         :param x_scale: Defines chart size on the x scale, defaults to 1.
         :param y_scale: Defines chart size on the y scale, defaults to 1.
         :param offset_x_pixels: Shifts chart position on the cell from default upper left position upwards or downwards in pixels, defaults to 0.
         :param offset_y_pixels: Shifts chart position on the cell from default upper left position to the left or right in pixels, defaults to 0.
         :param header_count: _description_, defaults to 1. #TODO: describe this
         :param nrows: Sets top n rows to take data from, defaults to None.
+        :param reverse_axis_order: Defines x axis order.
         :param data_sheet_name: The name of the sheet from where to take data for the chart, defaults to None.
         :param data_start: A starting position for data that is taken for a chart, defaults to (0, 0).
         :raises ValueError: In case if you want to set mixed axis make sure that amount of columns same as amount of axis.
         :return: A SpreadSheet object.
         """
 
         data_start_cell = parse_range(data_start)
@@ -601,15 +603,16 @@
                                                     'endRowIndex': data_start_cell[
                                                                        0] + nrows + 1 if nrows is not None else None,
                                                     'startColumnIndex': data_start_cell[1] + index_column,
                                                     'endColumnIndex': data_start_cell[1] + index_column + 1,
                                                 }
                                             ]
                                         }
-                                    }
+                                    },
+                                    'reversed': reverse_axis_order,
                                 }
                             ],
                             'series': [*series],
                             'headerCount': header_count,
                         }
                     },
                     'position': {
@@ -648,16 +651,17 @@
                         y_axis_max_right: float = None,
                         x_scale: int = 1,
                         y_scale: int = 1,
                         offset_x_pixels: int = 0,
                         offset_y_pixels: int = 0,
                         header_count: int = 1,
                         nrows: int = None,
-                        data_sheet_name=None,
-                        data_start=(0, 0)
+                        reverse_axis_order: bool = False,
+                        data_sheet_name: str = None,
+                        data_start: Union[tuple, str] = (0, 0),
                         ):
         """Adds combo chart.
 
         :param left_columns: A column from which the data for the left y-axis will be taken. Requires an index from data_start param.
         E.g. columns=[1] would mean to select the second column from a given dataset for the left y-axis.
         :param right_columns: A column from which the data for the right y-axis will be taken. Requires an index from data_start param.
         E.g. columns=[1] would mean selecting the second column from a given dataset for the right x-axis.
@@ -680,14 +684,15 @@
         :param y_axis_max_right: Sets a maximum value on the y-axis situated on the right, defaults to None.
         :param x_scale: Defines chart size on the x scale, defaults to 1.
         :param y_scale: Defines chart size on the y scale, defaults to 1.
         :param offset_x_pixels: Shifts chart position on the cell from default upper left position upwards or downwards in pixels, defaults to 0
         :param offset_y_pixels: Shifts chart position on the cell from default upper left position to the left or right in pixels, defaults to 0
         :param header_count: _description_, defaults to 1. #TODO: explain this param
         :param nrows: Sets top n rows to take data from, defaults to None.
+        :param reverse_axis_order: Defines x axis order.
         :param data_sheet_name: The name of the sheet from where to take data for the chart, defaults to None.
         :param data_start: A starting position for data that is taken for a chart, defaults to (0, 0).
         :return: A SpreadSheet object.
         """
 
         data_start_cell = parse_range(data_start)
         series = [{
@@ -771,19 +776,20 @@
                                                     'endRowIndex': data_start_cell[
                                                                        0] + nrows + 1 if nrows is not None else None,
                                                     'startColumnIndex': data_start_cell[1] + index_column,
                                                     'endColumnIndex': data_start_cell[1] + index_column + 1,
                                                 }
                                             ]
                                         }
-                                    }
+                                    },
+                                    'reversed': reverse_axis_order,
                                 }
                             ],
                             'series': [*series],
-                            'headerCount': header_count
+                            'headerCount': header_count,
                         }
                     },
                     'position': {
                         'overlayPosition': {
                             'anchorCell': {
                                 'sheetId': self.sheet_id,
                                 'rowIndex': self.work_zone.get('startRowIndex'),
@@ -1755,15 +1761,15 @@
                    file.get('file_type') == 'folder' and file.get('name') == folder_name]
 
         if folders and selected_fields:
             return [[folder.get(x) for x in selected_fields] for folder in folders]
         elif folders:
             return [folder.get('id') for folder in folders]
         elif mkdir:
-            return self.create_folder(folder_name, current_folder)
+            return [self.create_folder(folder_name, current_folder)]
         else:
             return print(f"A folder called '{folder_name}' does not exist. To create one, set mkdir=True")
 
     def select_files(self, folder_id: str = None, trashed: bool = False):
         """Selects files in a given folder.
 
         :param folder_id: Folder's id, defaults to None (selects files from the whole Drive).
```

### Comparing `speedtab-0.2.1.9/speedtab/enums.py` & `speedtab-0.2.2/speedtab/enums.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.2.1.9/speedtab/formats.py` & `speedtab-0.2.2/speedtab/formats.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.2.1.9/setup.py` & `speedtab-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['google-api-python-client>=2.58.0,<3.0.0',
  'google-auth-httplib2>=0.1.0,<0.2.0',
  'google-auth-oauthlib>=0.5.2,<0.6.0']
 
 setup_kwargs = {
     'name': 'speedtab',
-    'version': '0.2.1.9',
+    'version': '0.2.2',
     'description': 'Convenient wrapper for working with Google Spreadsheets',
     'long_description': None,
     'author': 'Bogdan Gergel',
     'author_email': 'bogger147@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/BoggerSancho/SpeedTab-beta',
```

### Comparing `speedtab-0.2.1.9/PKG-INFO` & `speedtab-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedtab
-Version: 0.2.1.9
+Version: 0.2.2
 Summary: Convenient wrapper for working with Google Spreadsheets
 Home-page: https://github.com/BoggerSancho/SpeedTab-beta
 License: MIT
 Author: Bogdan Gergel
 Author-email: bogger147@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

