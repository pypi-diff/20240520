# Comparing `tmp/gspread_models-1.0.3.tar.gz` & `tmp/gspread_models-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gspread_models-1.0.3.tar", last modified: Fri Apr 19 20:04:28 2024, max compression
+gzip compressed data, was "gspread_models-1.0.5.tar", last modified: Mon May 20 21:46:46 2024, max compression
```

## Comparing `gspread_models-1.0.3.tar` & `gspread_models-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:04:28.285833 gspread_models-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-19 20:04:14.000000 gspread_models-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-04-19 20:04:28.285833 gspread_models-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-19 20:04:14.000000 gspread_models-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:04:28.285833 gspread_models-1.0.3/gspread_models/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-19 20:04:14.000000 gspread_models-1.0.3/gspread_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-04-19 20:04:14.000000 gspread_models-1.0.3/gspread_models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-19 20:04:14.000000 gspread_models-1.0.3/gspread_models/date_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-19 20:04:14.000000 gspread_models-1.0.3/gspread_models/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:04:28.285833 gspread_models-1.0.3/gspread_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-04-19 20:04:28.000000 gspread_models-1.0.3/gspread_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-19 20:04:28.000000 gspread_models-1.0.3/gspread_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 20:04:28.000000 gspread_models-1.0.3/gspread_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-19 20:04:28.000000 gspread_models-1.0.3/gspread_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-19 20:04:28.000000 gspread_models-1.0.3/gspread_models.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 20:04:28.285833 gspread_models-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-19 20:04:14.000000 gspread_models-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:46:46.752837 gspread_models-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-20 21:46:42.000000 gspread_models-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-05-20 21:46:46.752837 gspread_models-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6986 2024-05-20 21:46:42.000000 gspread_models-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:46:46.752837 gspread_models-1.0.5/gspread_models/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-20 21:46:42.000000 gspread_models-1.0.5/gspread_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5874 2024-05-20 21:46:42.000000 gspread_models-1.0.5/gspread_models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-20 21:46:42.000000 gspread_models-1.0.5/gspread_models/date_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-20 21:46:42.000000 gspread_models-1.0.5/gspread_models/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:46:46.752837 gspread_models-1.0.5/gspread_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-05-20 21:46:46.000000 gspread_models-1.0.5/gspread_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-20 21:46:46.000000 gspread_models-1.0.5/gspread_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 21:46:46.000000 gspread_models-1.0.5/gspread_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-20 21:46:46.000000 gspread_models-1.0.5/gspread_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-20 21:46:46.000000 gspread_models-1.0.5/gspread_models.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 21:46:46.752837 gspread_models-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-20 21:46:42.000000 gspread_models-1.0.5/setup.py
```

### Comparing `gspread_models-1.0.3/LICENSE` & `gspread_models-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gspread_models-1.0.3/gspread_models/base.py` & `gspread_models-1.0.5/gspread_models/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 
 #from abc import abstractmethod
 from typing import List, Dict
-#from functools import cached_property
+from functools import lru_cache #,cached_property
 from datetime import datetime
 
-from gspread_models.service import SpreadsheetService
+from gspread import Worksheet #, Spreadsheet
+#from gspread_models.service import SpreadsheetService
 
 
 class BaseModel:
 
     SHEET_NAME = None # abstract constant (str) to be set in child class
 
     COLUMNS = [] # abstract constant to be set in child class
@@ -34,15 +35,17 @@
             val = self.attrs.get(col)
             #if val.startswith("20"):
             # convert datetime parsable string to datetime object, dynamically
             if self.service.validate_timestamp(val):
                 val = self.service.parse_timestamp(val)
             setattr(self, col, val)
 
+    #
     # INSTANCE METHODS
+    #
 
     @property
     def created_at(self):
         """Wraps timestamp string from the sheet in a native datetime object."""
         return self.service.parse_timestamp(self.attrs.get("created_at"))
 
     #@property
@@ -77,107 +80,100 @@
         print(dict(self))
         #if self.id:
         #    self.attrs["updated_at"] = self.service.generate_timestamp()
         #    self.update(dict(self))
         #return self.create(dict(self))
         return self.create_all([dict(self)])
 
-
+    #
     # CLASS METHODS
+    #
 
     @classmethod
     def set_document_id(cls, document_id):
         cls.service.document_id = document_id
 
     @classmethod
-    def get_sheet(cls):
-       print(f"SHEET ('{cls.SHEET_NAME}')...")
+    def get_sheet(cls) -> Worksheet:
+       print(f"GET SHEET ('{cls.SHEET_NAME}')...")
        return cls.service.get_sheet(sheet_name=cls.SHEET_NAME)
 
+    # using @property + @lru_cache because @cached_property throws:
+    # ... TypeError: Cannot use cached_property instance without calling __set_name__ on it.
+    @classmethod
+    @property
+    @lru_cache(maxsize=None)
+    def sheet(cls) -> Worksheet:
+        """Caches the sheet to avoid unnecessary API requests."""
+        return cls.get_sheet()
 
-
-    # API
+    # ... API
 
     @classmethod
-    def find(cls, by_id, sheet=None):
+    def find(cls, by_id):
         """Fetches a record by its unique identifier."""
-        sheet = sheet or cls.get_sheet() # assumes sheet exists, with the proper headers!
-        records = sheet.get_all_records()
+        records = cls.sheet.get_all_records()
         for record in records:
             if record.get("id") == by_id:
                 return cls(record)
         return None
 
     @classmethod
-    def all(cls, sheet=None):
+    def all(cls):
         """Fetches all records from a given sheet."""
-        sheet = sheet or cls.get_sheet() # assumes sheet exists, with the proper headers!
-        records = sheet.get_all_records()
+        records = cls.sheet.get_all_records()
         return [cls(record) for record in records]
 
     @classmethod
-    def destroy_all(cls, sheet=None):
+    def destroy_all(cls):
         """Removes all records from a given sheet, except the header row."""
-        sheet = sheet or cls.get_sheet()
-        records = sheet.get_all_records()
+        records = cls.sheet.get_all_records()
         # start on the second row, and delete one more than the number of records (to account for header row)
-        return sheet.delete_rows(start_index=2, end_index=len(records)+1)
+        return cls.sheet.delete_rows(start_index=2, end_index=len(records)+1)
 
     @classmethod
     def where(cls, **kwargs):
         """Filter records which match all provided values."""
-        #sheet = sheet or cls.get_sheet() # assumes sheet exists, with the proper headers!
-        sheet = cls.get_sheet()
-        records = sheet.get_all_records()
+        records = cls.sheet.get_all_records()
         objs = []
         for attrs in records:
             obj = cls(attrs)
 
-            #for k,v in kwargs.items():
-            #    if getattr(obj, k) == v:
-            #        objs.append(obj)
-
-            #match_all_conditions = all(dict(obj).get(k) == v for k, v in kwargs.items())
             match_all = all(getattr(obj, k) == v for k, v in kwargs.items())
 
             if match_all:
                 objs.append(obj)
 
         return objs
 
     @classmethod
     def create_all(cls, new_records:List[Dict], records=[]):
         """Appends new records (list of dictionaries) to the sheet.
             Adds auto-incrementing unique identifiers, and timestamp columns.
         """
-        sheet = cls.get_sheet() # assumes sheet exists, with the proper headers!
-
-        records = records or cls.all(sheet=sheet)
-        #next_row_number = len(records) + 2 # plus headers plus one
+        records = records or cls.all()
 
         # auto-increment integer identifier:
         if any(records):
             existing_ids = [r.id for r in records]
             next_id = max(existing_ids) + 1
         else:
             next_id = 1
 
         rows = []
         for attrs in new_records:
             attrs["id"] = next_id
             now = cls.service.generate_timestamp()
             attrs["created_at"] = now
-            #attrs["updated_at"] = now
 
             inst = cls(attrs)
             rows.append(inst.row)
             next_id += 1
 
-        #return sheet.insert_rows(rows, row=next_row_number)
-        return sheet.append_rows(rows)
+        return cls.sheet.append_rows(rows)
 
     @classmethod
     def create(cls, new_record:dict):
         """Appends new records (list of dictionaries) to the sheet.
             Adds auto-incrementing unique identifiers, and timestamp columns.
         """
         return cls.create_all([new_record])
```

### Comparing `gspread_models-1.0.3/gspread_models/date_parser.py` & `gspread_models-1.0.5/gspread_models/date_parser.py`

 * *Files identical despite different names*

### Comparing `gspread_models-1.0.3/gspread_models/service.py` & `gspread_models-1.0.5/gspread_models/service.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 
 import os
 from typing import List
 from functools import cached_property
 
 from dotenv import load_dotenv
-from gspread import service_account, authorize, Worksheet
+from gspread import service_account, authorize, Worksheet, Spreadsheet
 from gspread.exceptions import WorksheetNotFound #, SpreadsheetNotFound
 
 from gspread_models.date_parser import DateParser
 
 load_dotenv()
 
 DEFAULT_FILEPATH = os.path.join(os.path.dirname(__file__), "..", "google-credentials.json")
@@ -37,17 +37,17 @@
 
         self.document_id = document_id
 
         print("SPREADSHEET SERVICE...")
         print("DOCUMENT ID:", self.document_id)
 
     @cached_property
-    def doc(self):
-        """Get the given document. NOTE: this will make an API call."""
-        return self.client.open_by_key(self.document_id) #> <class 'gspread.models.Spreadsheet'>
+    def doc(self) -> Spreadsheet:
+        """Get the given document."""
+        return self.client.open_by_key(self.document_id)
 
     @property
     def sheets(self) -> List[Worksheet]:
         """List all sheets in the given document."""
         return self.doc.worksheets()
 
     def get_sheet(self, sheet_name) -> Worksheet:
```

### Comparing `gspread_models-1.0.3/setup.py` & `gspread_models-1.0.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,25 @@
 # setup.py
 
-from setuptools import setup #, find_packages
+from setuptools import setup
 
 from gspread_models import VERSION
 
-# PyPI doesn't display the links in this markdown:
-#with open("README.md", "r") as fh:
-#    long_description = fh.read()
-
+# FYI: PyPI doesn't display the links in this markdown
 # https://stackoverflow.com/a/26737672/670433
-# relative links in README as shown on PiPY are broken, so let's try converting to RST instead perhaps
-try:
-    import pypandoc
-    long_description = pypandoc.convert_file("README.md", "rst")
-except(IOError, ImportError, OSError) as err:
-    print("PANDOC RST CONVERSION ERROR. FALLBACK TO MARKDOWN...")
-    print(err)
-    long_description = open("README.md").read()
-
-# https://stackoverflow.com/a/53069528/670433
-#with open("requirements.txt", "r") as f:
-#    install_requires = f.read().splitlines() #> ["gunicorn", "docutils>=0.3", "lxml==0.5a7"]
-
+with open("README.md", "r") as fh:
+    long_description = fh.read()
 
 setup(
     name="gspread_models",
     version=VERSION,
     author="Michael Rossetti",
     author_email="datacreativellc@gmail.com",
-    description="Model based ORM interface into Google Sheets, using the gspread package.",
+    description="An Object Relational Mapper (ORM) for the Google Sheets API. Provides a straightforward and intuitive model-based query interface, making it easy to interact with Google Sheets as if it were more like a database. Offers a fast and flexible way to get up and running with a Google Sheets database, for rapid prototyping and development in Python.",
     long_description=long_description,
     long_description_content_type="text/markdown", # required if using a md file for long desc
     license="MIT",
     url="https://github.com/s2t2/gspread-models-py",
-    keywords="google sheets gspread models orm spreadsheet",
+    keywords="google sheets gspread models orm spreadsheet google-sheets google-sheets-api gspread-models gspread_models",
     install_requires=["python-dotenv", "gspread>=6.0.2"],  # install_requires
     packages=["gspread_models"], # find_packages()
 )
```

