# Comparing `tmp/smo_rejection-0.4.0.tar.gz` & `tmp/smo_rejection-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smo_rejection-0.4.0.tar", max compression
+gzip compressed data, was "smo_rejection-0.4.1.tar", max compression
```

## Comparing `smo_rejection-0.4.0.tar` & `smo_rejection-0.4.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0      283 2024-05-19 12:01:10.683744 smo_rejection-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2061 2024-05-18 10:29:03.252234 smo_rejection-0.4.0/README.md
--rw-r--r--   0        0        0      188 2024-05-19 12:00:20.787948 smo_rejection-0.4.0/smo_rejection/__init__.py
--rw-r--r--   0        0        0     1709 2024-05-18 10:29:03.257241 smo_rejection-0.4.0/smo_rejection/exception.py
--rw-r--r--   0        0        0     1628 2024-05-18 10:29:03.257241 smo_rejection-0.4.0/smo_rejection/models.py
--rw-r--r--   0        0        0     2193 2024-05-19 11:59:54.473573 smo_rejection-0.4.0/smo_rejection/pdf_export.py
--rw-r--r--   0        0        0     4419 2024-05-18 10:29:03.257241 smo_rejection-0.4.0/smo_rejection/processing.py
--rw-r--r--   0        0        0     4307 2024-05-18 10:29:03.258245 smo_rejection-0.4.0/smo_rejection/simulation.py
--rw-r--r--   0        0        0     2471 2024-05-18 10:29:03.258245 smo_rejection-0.4.0/smo_rejection/utils.py
--rw-r--r--   0        0        0     2357 1970-01-01 00:00:00.000000 smo_rejection-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      283 2024-05-19 12:21:12.881693 smo_rejection-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2061 2024-05-18 10:29:03.252234 smo_rejection-0.4.1/README.md
+-rw-r--r--   0        0        0      229 2024-05-19 12:21:12.886692 smo_rejection-0.4.1/smo_rejection/__init__.py
+-rw-r--r--   0        0        0     1709 2024-05-18 10:29:03.257241 smo_rejection-0.4.1/smo_rejection/exception.py
+-rw-r--r--   0        0        0     1628 2024-05-18 10:29:03.257241 smo_rejection-0.4.1/smo_rejection/models.py
+-rw-r--r--   0        0        0     2797 2024-05-19 12:21:12.896691 smo_rejection-0.4.1/smo_rejection/pdf_export.py
+-rw-r--r--   0        0        0     4419 2024-05-18 10:29:03.257241 smo_rejection-0.4.1/smo_rejection/processing.py
+-rw-r--r--   0        0        0     4307 2024-05-18 10:29:03.258245 smo_rejection-0.4.1/smo_rejection/simulation.py
+-rw-r--r--   0        0        0     2471 2024-05-18 10:29:03.258245 smo_rejection-0.4.1/smo_rejection/utils.py
+-rw-r--r--   0        0        0     2675 2024-05-19 12:21:12.898690 smo_rejection-0.4.1/smo_rejection/xml_export.py
+-rw-r--r--   0        0        0     2357 1970-01-01 00:00:00.000000 smo_rejection-0.4.1/PKG-INFO
```

### Comparing `smo_rejection-0.4.0/README.md` & `smo_rejection-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.4.0/smo_rejection/exception.py` & `smo_rejection-0.4.1/smo_rejection/exception.py`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.4.0/smo_rejection/models.py` & `smo_rejection-0.4.1/smo_rejection/models.py`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.4.0/smo_rejection/pdf_export.py` & `smo_rejection-0.4.1/smo_rejection/pdf_export.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,51 @@
 from reportlab.lib.pagesizes import letter
-from reportlab.platypus import SimpleDocTemplate, Table, TableStyle, Spacer
-from reportlab.lib.styles import getSampleStyleSheet
+from reportlab.platypus import SimpleDocTemplate, Table, TableStyle, Paragraph, Spacer
+from reportlab.lib.styles import getSampleStyleSheet, ParagraphStyle
 from reportlab.lib.units import inch
 from reportlab.lib import colors
+from reportlab.pdfbase.ttfonts import TTFont
+from reportlab.pdfbase import pdfmetrics
 from .utils import calculate_mean_served_requests
 
 def export_to_pdf(results, filename):
+    pdfmetrics.registerFont(TTFont('Arial', 'arial.ttf'))
+
     styles = getSampleStyleSheet()
-    doc = SimpleDocTemplate(filename, pagesize=letter)
+    styles.add(ParagraphStyle(name='Cyrillic', fontName='Arial', fontSize=10))
+    styles.add(ParagraphStyle(name='CyrillicHeading3', fontName='Arial', fontSize=12, spaceAfter=6))
+
+    doc = SimpleDocTemplate(filename, pagesize=letter, encoding='UTF-8')
     elements = []
 
     for i, result in enumerate(results, start=1):
-        header = f"---------------------------- Cимуляция номер: {i} ----------------------------"
+        header = Paragraph(f"----------------------------------------- Симуляция номер: {i} -----------------------------------------", styles["CyrillicHeading3"])
         elements.append(header)
 
-        table_data = [["index", "rand_value", "iba", "app_time", "server_1", "server_2", "server_3", "Обслужено", "Отказов"]]
+        table_data = [["Индекс", "Случайное число", "МЕЖ", "Время в очереди", "Сервер 1", "Сервер 2", "Сервер 3", "Обслужено", "Отказов"]]
         for entry in result.request_times:
             row = [entry["index"], entry["rand_value"], entry["iba"], entry["app_time"]]
             for j in range(1, 4):
                 row.append(entry[f"server_{j}"])
             row.extend([entry["Обслужено"], entry["Отказов"]])
             table_data.append(row)
 
         table = Table(table_data)
         table.setStyle(TableStyle([
-            ('FONTNAME', (0, 0), (-1, -1), 'Courier'),
+            ('FONTNAME', (0, 0), (-1, -1), 'Arial'),
             ('FONTSIZE', (0, 0), (-1, -1), 8),
             ('ALIGN', (0, 0), (-1, -1), 'CENTER'),
             ('INNERGRID', (0, 0), (-1, -1), 0.25, colors.black),
             ('BOX', (0, 0), (-1, -1), 0.25, colors.black),
         ]))
         elements.append(table)
 
-        served_count = f"Количество исполненных заявок: {result.served_requests}"
-        rejected_count = f"Количество отказов: {result.rejected_requests}"
+        served_count = Paragraph(f"Количество исполненных заявок: {result.served_requests}", styles["Cyrillic"])
+        rejected_count = Paragraph(f"Количество отказов: {result.rejected_requests}", styles["Cyrillic"])
         elements.append(served_count)
         elements.append(rejected_count)
         elements.append(Spacer(1, 0.5 * inch))
 
-    mean_served = f"В качестве оценки искомого математического ожидания a – числа обслуженных заявок примем выборочную среднюю: a = {calculate_mean_served_requests(results)}"
+    mean_served = Paragraph(f"В качестве оценки искомого математического ожидания a – числа обслуженных заявок примем выборочную среднюю: a = {calculate_mean_served_requests(results)}", styles["Cyrillic"])
     elements.append(mean_served)
 
-    doc.build(elements)
+    doc.build(elements)
```

### Comparing `smo_rejection-0.4.0/smo_rejection/processing.py` & `smo_rejection-0.4.1/smo_rejection/processing.py`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.4.0/smo_rejection/simulation.py` & `smo_rejection-0.4.1/smo_rejection/simulation.py`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.4.0/smo_rejection/utils.py` & `smo_rejection-0.4.1/smo_rejection/utils.py`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.4.0/PKG-INFO` & `smo_rejection-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smo_rejection
-Version: 0.4.0
+Version: 0.4.1
 Summary: 
 Author: mbtmrw
 Author-email: keks2324098@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

