# Comparing `tmp/checkgen-0.2.0.tar.gz` & `tmp/checkgen-0.3.1.tar.gz`

## Comparing `checkgen-0.2.0.tar` & `checkgen-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 checkgen-0.2.0/requirements.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 checkgen-0.2.0/.idea/.gitignore
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 checkgen-0.2.0/.idea/checkprint.iml
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 checkgen-0.2.0/.idea/misc.xml
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 checkgen-0.2.0/.idea/modules.xml
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 checkgen-0.2.0/.idea/vcs.xml
--rw-r--r--   0        0        0    24840 2020-02-02 00:00:00.000000 checkgen-0.2.0/.idea/workspace.xml
--rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 checkgen-0.2.0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 checkgen-0.2.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 checkgen-0.2.0/src/checkgen/__init__.py
--rw-r--r--   0        0        0     6331 2020-02-02 00:00:00.000000 checkgen-0.2.0/src/checkgen/document.py
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 checkgen-0.2.0/src/checkgen/models.py
--rw-r--r--   0        0        0     3834 2020-02-02 00:00:00.000000 checkgen-0.2.0/src/checkgen/printer.py
--rw-r--r--   0        0        0    42132 2020-02-02 00:00:00.000000 checkgen-0.2.0/src/checkgen/assets/fonts/Cookie-Regular.ttf
--rw-r--r--   0        0        0   130832 2020-02-02 00:00:00.000000 checkgen-0.2.0/src/checkgen/assets/fonts/OpenSans-Regular.ttf
--rw-r--r--   0        0        0    57392 2020-02-02 00:00:00.000000 checkgen-0.2.0/src/checkgen/assets/fonts/TitilliumWeb-Regular.ttf
--rw-r--r--   0        0        0    15580 2020-02-02 00:00:00.000000 checkgen-0.2.0/src/checkgen/assets/fonts/micrenc.ttf
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 checkgen-0.2.0/LICENSE
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 checkgen-0.2.0/README.md
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 checkgen-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 checkgen-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 checkgen-0.3.1/requirements.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 checkgen-0.3.1/.idea/.gitignore
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 checkgen-0.3.1/.idea/checkprint.iml
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 checkgen-0.3.1/.idea/misc.xml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 checkgen-0.3.1/.idea/modules.xml
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 checkgen-0.3.1/.idea/vcs.xml
+-rw-r--r--   0        0        0    24840 2020-02-02 00:00:00.000000 checkgen-0.3.1/.idea/workspace.xml
+-rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 checkgen-0.3.1/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 checkgen-0.3.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 checkgen-0.3.1/src/checkgen/__init__.py
+-rw-r--r--   0        0        0     6850 2020-02-02 00:00:00.000000 checkgen-0.3.1/src/checkgen/document.py
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 checkgen-0.3.1/src/checkgen/models.py
+-rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 checkgen-0.3.1/src/checkgen/printer.py
+-rw-r--r--   0        0        0    42132 2020-02-02 00:00:00.000000 checkgen-0.3.1/src/checkgen/assets/fonts/Cookie-Regular.ttf
+-rw-r--r--   0        0        0   130832 2020-02-02 00:00:00.000000 checkgen-0.3.1/src/checkgen/assets/fonts/OpenSans-Regular.ttf
+-rw-r--r--   0        0        0    57392 2020-02-02 00:00:00.000000 checkgen-0.3.1/src/checkgen/assets/fonts/TitilliumWeb-Regular.ttf
+-rw-r--r--   0        0        0    15580 2020-02-02 00:00:00.000000 checkgen-0.3.1/src/checkgen/assets/fonts/micrenc.ttf
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 checkgen-0.3.1/LICENSE
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 checkgen-0.3.1/README.md
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 checkgen-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 checkgen-0.3.1/PKG-INFO
```

### Comparing `checkgen-0.2.0/.idea/checkprint.iml` & `checkgen-0.3.1/.idea/checkprint.iml`

 * *Files identical despite different names*

### Comparing `checkgen-0.2.0/.idea/vcs.xml` & `checkgen-0.3.1/.idea/vcs.xml`

 * *Files identical despite different names*

### Comparing `checkgen-0.2.0/.idea/workspace.xml` & `checkgen-0.3.1/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `checkgen-0.2.0/.idea/inspectionProfiles/Project_Default.xml` & `checkgen-0.3.1/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `checkgen-0.2.0/src/checkgen/document.py` & `checkgen-0.3.1/src/checkgen/document.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from contextlib import contextmanager
+
 import fpdf
 from pathlib import Path
 
 FONTS = Path(__file__).absolute().parent / 'assets' / 'fonts'
 
 
 class Document(fpdf.FPDF):
@@ -67,14 +69,19 @@
 
     def box(self, *, left, top, width, height):
         self.horizontal_line(left=left, top=top, width=width)
         self.horizontal_line(left=left, top=top + height, width=width)
         self.vertical_line(left=left, top=top, height=height)
         self.vertical_line(left=left + width, top=top, height=height)
 
+    @contextmanager
+    def use_rotation(self, angle, *, left, top):
+        with self.rotation(angle, x=left, y=top + self._offset):
+            yield
+
 
 class Check:
     def __init__(self, issuer, check_number):
         self.issuer = issuer
         self.check_number = check_number
 
     def print_micr(self, document):
@@ -170,7 +177,15 @@
         document.print_cell(payment.written_amount(), width=6.6, height=0.25, pad=True)
 
         # memo
         if payment.memo:
             document.set_position(left=0.875, top=2.3)
             document.use_regular_font(10)
             document.print_cell(payment.memo, width=2, height=0.25)
+
+    def mark_as_void(self, document):
+        top = 2
+        for left in [2, 4]:
+            with document.use_rotation(45, left=left, top=top):
+                document.set_position(left=left, top=top)
+                document.use_metadata_font(20)
+                document.print_cell('VOID VOID VOID', width=3, height=0.5)
```

### Comparing `checkgen-0.2.0/src/checkgen/models.py` & `checkgen-0.3.1/src/checkgen/models.py`

 * *Files identical despite different names*

### Comparing `checkgen-0.2.0/src/checkgen/printer.py` & `checkgen-0.3.1/src/checkgen/printer.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,35 +66,35 @@
         if remainder:
             if fold_last_payment and payments:
                 self._payments[-1].amount += remainder
             else:
                 self._payments.append(Payment(payee, remainder, date, memo))
 
     def print(self, *, empty_checks=EmptyChecks.PRINT, type=PrintType.MICR | PrintType.LABELS | PrintType.INFORMATION,
-              target_num_checks=0):
+              target_num_checks=0, void=False):
         num_checks = math.ceil(max(len(self._payments), target_num_checks) / 3) * 3 \
             if empty_checks is EmptyChecks.PRINT \
             else len(self._payments)
 
         book = Book(self.issuer, max(num_checks, target_num_checks), self.starting_check_number)
 
-        report = book.print(self._payments, type=type)
+        report = book.print(self._payments, type=type, void=void)
 
         return book, report
 
 
 class Book:
     def __init__(self, issuer, num_checks=3, starting_check_number=1001):
         self.document = Document()
 
         self.checks = []
         for i in range(num_checks):
             self.checks.append(Check(issuer, starting_check_number + i))
 
-    def print(self, payments=None, *, type=PrintType.MICR | PrintType.LABELS | PrintType.INFORMATION):
+    def print(self, payments=None, *, type=PrintType.MICR | PrintType.LABELS | PrintType.INFORMATION, void=False):
         report = []
 
         for i, check in enumerate(self.checks):
             record = {'num': check.check_number, 'date': None, 'payee': None, 'amount': None}
 
             if i % 3 == 0:
                 self.document.add_page()
@@ -106,14 +106,17 @@
 
             if PrintType.LABELS in type:
                 check.print_check_labels(self.document)
 
             if PrintType.INFORMATION in type:
                 check.print_check_information(self.document)
 
+            if void:
+                check.mark_as_void(self.document)
+
             if payments and i < len(payments):
                 payment = payments[i]
 
                 record |= {'date': payment.date, 'payee': payment.payee, 'amount': payment.amount}
 
                 check.fill_check(self.document, payment)
```

### Comparing `checkgen-0.2.0/src/checkgen/assets/fonts/Cookie-Regular.ttf` & `checkgen-0.3.1/src/checkgen/assets/fonts/Cookie-Regular.ttf`

 * *Files identical despite different names*

### Comparing `checkgen-0.2.0/src/checkgen/assets/fonts/OpenSans-Regular.ttf` & `checkgen-0.3.1/src/checkgen/assets/fonts/OpenSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `checkgen-0.2.0/src/checkgen/assets/fonts/TitilliumWeb-Regular.ttf` & `checkgen-0.3.1/src/checkgen/assets/fonts/TitilliumWeb-Regular.ttf`

 * *Files identical despite different names*

### Comparing `checkgen-0.2.0/src/checkgen/assets/fonts/micrenc.ttf` & `checkgen-0.3.1/src/checkgen/assets/fonts/micrenc.ttf`

 * *Files identical despite different names*

### Comparing `checkgen-0.2.0/LICENSE` & `checkgen-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `checkgen-0.2.0/README.md` & `checkgen-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `checkgen-0.2.0/pyproject.toml` & `checkgen-0.3.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "checkgen"
-version = "0.2.0"
+version = "0.3.1"
 description = "Print bank checks"
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
     { name = "Yanky Hoffman" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "fpdf2 == 2.7.8",
+    "fpdf2 == 2.7.9",
     "num2words == 0.5.13",
 ]
 
 [project.urls]
 Homepage = "https://github.com/yankyhoffman/check-generator"
```

### Comparing `checkgen-0.2.0/PKG-INFO` & `checkgen-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.3
 Name: checkgen
-Version: 0.2.0
+Version: 0.3.1
 Summary: Print bank checks
 Project-URL: Homepage, https://github.com/yankyhoffman/check-generator
 Author: Yanky Hoffman
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
-Requires-Dist: fpdf2==2.7.8
+Requires-Dist: fpdf2==2.7.9
 Requires-Dist: num2words==0.5.13
 Description-Content-Type: text/markdown
 
 # checkgen
 
 Print checks on 3 checks per page in bulk.
```

