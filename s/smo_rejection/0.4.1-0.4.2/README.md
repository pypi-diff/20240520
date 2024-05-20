# Comparing `tmp/smo_rejection-0.4.1.tar.gz` & `tmp/smo_rejection-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smo_rejection-0.4.1.tar", max compression
+gzip compressed data, was "smo_rejection-0.4.2.tar", max compression
```

## Comparing `smo_rejection-0.4.1.tar` & `smo_rejection-0.4.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      283 2024-05-19 12:21:12.881693 smo_rejection-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     2061 2024-05-18 10:29:03.252234 smo_rejection-0.4.1/README.md
--rw-r--r--   0        0        0      229 2024-05-19 12:21:12.886692 smo_rejection-0.4.1/smo_rejection/__init__.py
--rw-r--r--   0        0        0     1709 2024-05-18 10:29:03.257241 smo_rejection-0.4.1/smo_rejection/exception.py
--rw-r--r--   0        0        0     1628 2024-05-18 10:29:03.257241 smo_rejection-0.4.1/smo_rejection/models.py
--rw-r--r--   0        0        0     2797 2024-05-19 12:21:12.896691 smo_rejection-0.4.1/smo_rejection/pdf_export.py
--rw-r--r--   0        0        0     4419 2024-05-18 10:29:03.257241 smo_rejection-0.4.1/smo_rejection/processing.py
--rw-r--r--   0        0        0     4307 2024-05-18 10:29:03.258245 smo_rejection-0.4.1/smo_rejection/simulation.py
--rw-r--r--   0        0        0     2471 2024-05-18 10:29:03.258245 smo_rejection-0.4.1/smo_rejection/utils.py
--rw-r--r--   0        0        0     2675 2024-05-19 12:21:12.898690 smo_rejection-0.4.1/smo_rejection/xml_export.py
--rw-r--r--   0        0        0     2357 1970-01-01 00:00:00.000000 smo_rejection-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      283 2024-05-20 07:59:33.308864 smo_rejection-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0    16387 2024-05-20 07:59:33.306860 smo_rejection-0.4.2/README.md
+-rw-r--r--   0        0        0      301 2024-05-20 07:59:33.316861 smo_rejection-0.4.2/smo_rejection/__init__.py
+-rw-r--r--   0        0        0     1709 2024-05-18 10:29:03.257241 smo_rejection-0.4.2/smo_rejection/exception.py
+-rw-r--r--   0        0        0     1628 2024-05-18 10:29:03.257241 smo_rejection-0.4.2/smo_rejection/models.py
+-rw-r--r--   0        0        0     4236 2024-05-20 07:59:33.326861 smo_rejection-0.4.2/smo_rejection/pdf_export.py
+-rw-r--r--   0        0        0     4419 2024-05-18 10:29:03.257241 smo_rejection-0.4.2/smo_rejection/processing.py
+-rw-r--r--   0        0        0     4307 2024-05-18 10:29:03.258245 smo_rejection-0.4.2/smo_rejection/simulation.py
+-rw-r--r--   0        0        0     2471 2024-05-18 10:29:03.258245 smo_rejection-0.4.2/smo_rejection/utils.py
+-rw-r--r--   0        0        0     4797 2024-05-20 07:59:33.329863 smo_rejection-0.4.2/smo_rejection/xml_export.py
+-rw-r--r--   0        0        0    16485 1970-01-01 00:00:00.000000 smo_rejection-0.4.2/PKG-INFO
```

### Comparing `smo_rejection-0.4.1/README.md` & `smo_rejection-0.4.2/smo_rejection/exception.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,39 @@
-## Исключения
-
-- NumIterationsNegative
-    Исключение выбрасывается, если количество итераций отрицательное.
-
-- NumIterationsIsZero
-Исключение выбрасывается, если количество итераций равно нулю.
-
-- NumThreadsNegative
-    Исключение выбрасывается, если количество потоков отрицательное.
-
-- NumThreadsIsZero
-    Исключение выбрасывается, если количество потоков равно нулю.
-
-- AlphaIsZero
-    Исключение выбрасывается, если параметр alpha равен нулю.
-
-- AlphaNegative
-    Исключение выбрасывается, если параметр alpha отрицательный.
-
-- ServiceTimeNegative
-    Исключение выбрасывается, если время обслуживания отрицательное.
-
-- MaxTimeNegative
-    Исключение выбрасывается, если максимальное время симуляции отрицательное.
-
-## Вспомогательные функции
-
-- round_value
-    Округляет заданное число до 4 знаков после запятой.
-
-
-- generate_random_number
-    Генерирует случайное число в диапазоне [0, 1] с округлением до 4 знаков после запятой.
-    Если сгенерировано 0, повторяет генерацию.
-
-
-- calculate_ln
-    Возвращает результат натурального логарифма от случайного числа r_i с округлением до 4 знаков после запятой.
-
-
-- calculate_time
-    Возвращает время между двумя последовательными заявками с округлением до 4 знаков после запятой.
+class InvalidInputError(Exception):
+    """Исключение для недопустимых входных значений."""
+    pass
+
+class SimulationError(Exception):
+    """Исключение для ошибок во время симуляции."""
+    pass
+
+class NumIterationsNegative(Exception):
+    """Исключение выбрасывается, если количество итераций отрицательное."""
+    pass
+
+class NumIterationsIsZero(Exception):
+    """Исключение выбрасывается, если количество итераций равно нулю."""
+    pass
+
+class NumChannelsNegative(Exception):
+    """Исключение выбрасывается, если количество каналов отрицательное."""
+    pass
+
+class NumChannelsIsZero(Exception):
+    """Исключение выбрасывается, если количество каналов равно нулю."""
+    pass
+
+class AlphaIsZero(Exception):
+    """Исключение выбрасывается, если параметр alpha равен нулю."""
+    pass
+
+class AlphaNegative(Exception):
+    """Исключение выбрасывается, если параметр alpha отрицательный."""
+    pass
+
+class ServiceTimeNegative(Exception):
+    """Исключение выбрасывается, если время обслуживания отрицательное."""
+    pass
+
+class MaxTimeNegative(Exception):
+    """Исключение выбрасывается, если максимальное время симуляции отрицательное."""
+    pass
```

### Comparing `smo_rejection-0.4.1/smo_rejection/models.py` & `smo_rejection-0.4.2/smo_rejection/models.py`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.4.1/smo_rejection/pdf_export.py` & `smo_rejection-0.4.2/smo_rejection/pdf_export.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,48 +4,67 @@
 from reportlab.lib.units import inch
 from reportlab.lib import colors
 from reportlab.pdfbase.ttfonts import TTFont
 from reportlab.pdfbase import pdfmetrics
 from .utils import calculate_mean_served_requests
 
 def export_to_pdf(results, filename):
+    """
+    Экспортирует результаты симуляции в PDF-файл.
+
+    ### Параметры:
+    * `results (list)` - Список результатов симуляции.
+    * `filename (str)` - Имя файла для сохранения результатов.
+
+    ### Примечание:
+    Функция создает новый PDF-документ и записывает в него результаты симуляции.
+    """
+    # Регистрация шрифта Arial для поддержки кириллицы
     pdfmetrics.registerFont(TTFont('Arial', 'arial.ttf'))
 
+    # Получение стандартных стилей и добавление стилей для кириллицы
     styles = getSampleStyleSheet()
     styles.add(ParagraphStyle(name='Cyrillic', fontName='Arial', fontSize=10))
     styles.add(ParagraphStyle(name='CyrillicHeading3', fontName='Arial', fontSize=12, spaceAfter=6))
 
+    # Создание документа PDF с указанным размером страницы и кодировкой
     doc = SimpleDocTemplate(filename, pagesize=letter, encoding='UTF-8')
     elements = []
 
     for i, result in enumerate(results, start=1):
+        # Добавление заголовка для каждой симуляции
         header = Paragraph(f"----------------------------------------- Симуляция номер: {i} -----------------------------------------", styles["CyrillicHeading3"])
         elements.append(header)
 
+        # Подготовка данных для таблицы
         table_data = [["Индекс", "Случайное число", "МЕЖ", "Время в очереди", "Сервер 1", "Сервер 2", "Сервер 3", "Обслужено", "Отказов"]]
         for entry in result.request_times:
             row = [entry["index"], entry["rand_value"], entry["iba"], entry["app_time"]]
             for j in range(1, 4):
                 row.append(entry[f"server_{j}"])
             row.extend([entry["Обслужено"], entry["Отказов"]])
             table_data.append(row)
 
+        # Создание таблицы и установка стилей
         table = Table(table_data)
         table.setStyle(TableStyle([
             ('FONTNAME', (0, 0), (-1, -1), 'Arial'),
             ('FONTSIZE', (0, 0), (-1, -1), 8),
             ('ALIGN', (0, 0), (-1, -1), 'CENTER'),
             ('INNERGRID', (0, 0), (-1, -1), 0.25, colors.black),
             ('BOX', (0, 0), (-1, -1), 0.25, colors.black),
         ]))
         elements.append(table)
 
+        # Добавление итогов для каждой симуляции
         served_count = Paragraph(f"Количество исполненных заявок: {result.served_requests}", styles["Cyrillic"])
         rejected_count = Paragraph(f"Количество отказов: {result.rejected_requests}", styles["Cyrillic"])
         elements.append(served_count)
         elements.append(rejected_count)
-        elements.append(Spacer(1, 0.5 * inch))
+        elements.append(Spacer(1, 0.5 * inch))  # Добавление отступа между симуляциями
 
+    # Добавление среднего количества обслуженных заявок в конце документа
     mean_served = Paragraph(f"В качестве оценки искомого математического ожидания a – числа обслуженных заявок примем выборочную среднюю: a = {calculate_mean_served_requests(results)}", styles["Cyrillic"])
     elements.append(mean_served)
 
+    # Построение и сохранение PDF документа
     doc.build(elements)
```

### Comparing `smo_rejection-0.4.1/smo_rejection/processing.py` & `smo_rejection-0.4.2/smo_rejection/processing.py`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.4.1/smo_rejection/simulation.py` & `smo_rejection-0.4.2/smo_rejection/simulation.py`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.4.1/smo_rejection/utils.py` & `smo_rejection-0.4.2/smo_rejection/utils.py`

 * *Files identical despite different names*

