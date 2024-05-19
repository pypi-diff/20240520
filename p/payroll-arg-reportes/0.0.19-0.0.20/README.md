# Comparing `tmp/payroll_arg_reportes-0.0.19.tar.gz` & `tmp/payroll_arg_reportes-0.0.20.tar.gz`

## Comparing `payroll_arg_reportes-0.0.19.tar` & `payroll_arg_reportes-0.0.20.tar`

### file list

```diff
@@ -1,37 +1,45 @@
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.19/requirements.txt
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.19/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.19/.github/workflows/tests.yml
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.19/docs/libro-de-sueldos.md
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.19/docs/pypi-publish.md
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.19/docs/recibo-de-sueldos.md
--rw-r--r--   0        0        0   285657 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.19/docs/images/libro-sueldo.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.19/py_arg_reports/__init__.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.19/py_arg_reports/config.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.19/py_arg_reports/logs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.19/py_arg_reports/base_reports/__init__.py
--rw-r--r--   0        0        0     8971 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.19/py_arg_reports/base_reports/recibo_base_1.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.19/py_arg_reports/reporters/__init__.py
--rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.19/py_arg_reports/reporters/descarga_excel.py
--rw-r--r--   0        0        0    28320 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.19/py_arg_reports/reporters/recibo_sueldo.py
--rw-r--r--   0        0        0     9673 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.19/py_arg_reports/reporters/libro_sueldo/__init__.py
--rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.19/py_arg_reports/reporters/libro_sueldo/data.py
--rw-r--r--   0        0        0    10488 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.19/py_arg_reports/reporters/libro_sueldo/samples/samples-recibo-info.json
--rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.19/py_arg_reports/reporters/samples/samples-recibo-info.json
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.19/py_arg_reports/tables/base_tables.py
--rw-r--r--   0        0        0   154914 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.19/py_arg_reports/test_cases/liquidacion_completa.json
--rw-r--r--   0        0        0    10093 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.19/py_arg_reports/test_cases/liquidacion_corta.json
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.19/py_arg_reports/test_cases/test_libro_sueldo.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.19/py_arg_reports/test_cases/test_recibo.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.19/py_arg_reports/tools/__init__.py
--rw-r--r--   0        0        0    14126 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.19/py_arg_reports/tools/base.py
--rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.19/py_arg_reports/tools/recibos_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.19/tests/__init__.py
--rw-r--r--   0        0        0     3914 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.19/tests/test_download_recibo.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.19/tests/libro_sueldo/__init__.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.19/tests/libro_sueldo/test_base_pdf.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.19/tests/temp/.gitignore
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.19/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.19/LICENSE
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.19/README.md
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.19/pyproject.toml
--rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.19/PKG-INFO
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/requirements.txt
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/docs/f931.md
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/docs/libro-de-sueldos.md
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/docs/pypi-publish.md
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/docs/recibo-de-sueldos.md
+-rw-r--r--   0        0        0   285657 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/docs/images/libro-sueldo.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/py_arg_reports/__init__.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/py_arg_reports/config.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/py_arg_reports/logs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/py_arg_reports/base_reports/__init__.py
+-rw-r--r--   0        0        0     8971 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/py_arg_reports/base_reports/recibo_base_1.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/py_arg_reports/reporters/__init__.py
+-rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/py_arg_reports/reporters/descarga_excel.py
+-rw-r--r--   0        0        0    28320 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/py_arg_reports/reporters/recibo_sueldo.py
+-rw-r--r--   0        0        0     7740 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/py_arg_reports/reporters/f931/reporter.py
+-rw-r--r--   0        0        0     6442 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/py_arg_reports/reporters/f931/tools.py
+-rwxr-xr-x   0        0        0    17144 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/py_arg_reports/reporters/f931/samples/Formato_SICOSS_v42.pdf
+-rw-r--r--   0        0        0     3887 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/py_arg_reports/reporters/f931/samples/f931-info.json
+-rw-r--r--   0        0        0     9675 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/py_arg_reports/reporters/libro_sueldo/__init__.py
+-rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/py_arg_reports/reporters/libro_sueldo/data.py
+-rw-r--r--   0        0        0    10488 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/py_arg_reports/reporters/libro_sueldo/samples/samples-recibo-info.json
+-rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/py_arg_reports/reporters/samples/samples-recibo-info.json
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/py_arg_reports/tables/base_tables.py
+-rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/py_arg_reports/test_cases/f931-info.json
+-rw-r--r--   0        0        0   154914 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/py_arg_reports/test_cases/liquidacion_completa.json
+-rw-r--r--   0        0        0    10093 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/py_arg_reports/test_cases/liquidacion_corta.json
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/py_arg_reports/test_cases/test_f931.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/py_arg_reports/test_cases/test_libro_sueldo.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/py_arg_reports/test_cases/test_recibo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/py_arg_reports/tools/__init__.py
+-rw-r--r--   0        0        0    14126 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/py_arg_reports/tools/base.py
+-rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/py_arg_reports/tools/recibos_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/tests/__init__.py
+-rw-r--r--   0        0        0     3914 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/tests/test_download_recibo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/tests/f931/__init__.py
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/tests/f931/test_generacion_f931.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/tests/libro_sueldo/__init__.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/tests/libro_sueldo/test_base_pdf.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/LICENSE
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/README.md
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/pyproject.toml
+-rw-r--r--   0        0        0     3856 2020-02-02 00:00:00.000000 payroll_arg_reportes-0.0.20/PKG-INFO
```

### Comparing `payroll_arg_reportes-0.0.19/.github/workflows/python-publish.yml` & `payroll_arg_reportes-0.0.20/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.19/.github/workflows/tests.yml` & `payroll_arg_reportes-0.0.20/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.19/docs/libro-de-sueldos.md` & `payroll_arg_reportes-0.0.20/docs/libro-de-sueldos.md`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.19/docs/pypi-publish.md` & `payroll_arg_reportes-0.0.20/docs/pypi-publish.md`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.19/docs/recibo-de-sueldos.md` & `payroll_arg_reportes-0.0.20/docs/recibo-de-sueldos.md`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.19/docs/images/libro-sueldo.png` & `payroll_arg_reportes-0.0.20/docs/images/libro-sueldo.png`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.19/py_arg_reports/base_reports/recibo_base_1.py` & `payroll_arg_reportes-0.0.20/py_arg_reports/base_reports/recibo_base_1.py`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.19/py_arg_reports/reporters/descarga_excel.py` & `payroll_arg_reportes-0.0.20/py_arg_reports/reporters/descarga_excel.py`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.19/py_arg_reports/reporters/recibo_sueldo.py` & `payroll_arg_reportes-0.0.20/py_arg_reports/reporters/recibo_sueldo.py`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.19/py_arg_reports/reporters/libro_sueldo/__init__.py` & `payroll_arg_reportes-0.0.20/py_arg_reports/reporters/libro_sueldo/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 F14 = Format(font_size=14)
 F10 = Format(font_size=10)
 F9 = Format(font_size=9)
 t10_line_sep = 0.5
 t9_line_sep = 0.3
 
 
-def descargar_libro(json_data: dict, output_path: str, filename: str) -> str:
+def descargar_libro(json_data: dict, output_path: str, filename: str) -> tuple:
     """ Descarga el libro sueldo en formato PDF,
         Retorna una tupla:
          - False, error: si falla
          - True, None: si todo salió bien
     """
 
     try:
@@ -195,15 +195,15 @@
     empleado_block.rectangle(Rect(1, y_titles+1.6, 6, 0.6), fill_color='#D0D0D0AA')
     neto_a_cobrar = float_to_format_currency(empleado["totales_liquidacion"]["neto_liquidacion"])
     empleado_block.text(f'Neto a cobrar   {neto_a_cobrar}', bold=True, x=1.2, y=y_titles+2, format_=F10)
 
 
 if __name__ == '__main__':
     """
-    Esto es para hacer pruebas rapido con los arhcivos de ejemplo.
+    Esto es para hacer pruebas rapido con los archivos de ejemplo.
     Dejar para hacer correcciones rápidas.
     En estas pruebas escupir los logs en la consola
     """
     import json
     # Descargar el libro
     json_data_test_file = 'py_arg_reports/reporters/libro_sueldo/samples/samples-recibo-info.json'
     json_data = json.load(open(json_data_test_file))
```

### Comparing `payroll_arg_reportes-0.0.19/py_arg_reports/reporters/libro_sueldo/data.py` & `payroll_arg_reportes-0.0.20/py_arg_reports/reporters/libro_sueldo/data.py`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.19/py_arg_reports/reporters/libro_sueldo/samples/samples-recibo-info.json` & `payroll_arg_reportes-0.0.20/py_arg_reports/reporters/libro_sueldo/samples/samples-recibo-info.json`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.19/py_arg_reports/reporters/samples/samples-recibo-info.json` & `payroll_arg_reportes-0.0.20/py_arg_reports/reporters/samples/samples-recibo-info.json`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.19/py_arg_reports/test_cases/liquidacion_completa.json` & `payroll_arg_reportes-0.0.20/py_arg_reports/test_cases/liquidacion_completa.json`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.19/py_arg_reports/test_cases/liquidacion_corta.json` & `payroll_arg_reportes-0.0.20/py_arg_reports/test_cases/liquidacion_corta.json`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.19/py_arg_reports/tools/base.py` & `payroll_arg_reportes-0.0.20/py_arg_reports/tools/base.py`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.19/py_arg_reports/tools/recibos_utils.py` & `payroll_arg_reportes-0.0.20/py_arg_reports/tools/recibos_utils.py`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.19/tests/test_download_recibo.py` & `payroll_arg_reportes-0.0.20/tests/test_download_recibo.py`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.19/tests/libro_sueldo/test_base_pdf.py` & `payroll_arg_reportes-0.0.20/tests/libro_sueldo/test_base_pdf.py`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.19/LICENSE` & `payroll_arg_reportes-0.0.20/LICENSE`

 * *Files identical despite different names*

### Comparing `payroll_arg_reportes-0.0.19/README.md` & `payroll_arg_reportes-0.0.20/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
    - 3: Descuento
  - Los campos `pk` se refieren a _primary key_ y no son necesarios para la generación de los reportes.
  - Puede haber más campos en tus datos, esta librería solo necesita los campos que se mencionan en cada reporte.
 
 ### Reportes Legales
 
 - [Recibo de Sueldos](https://github.com/Artimezoft/payroll_arg_reportes/blob/develop/docs/recibo-de-sueldos.md)
-- F.931
+- [F.931](https://github.com/Artimezoft/payroll_arg_reportes/blob/develop/docs/f931.md)
 - Libro de Sueldos Digital
 - [Libro de Sueldos](https://github.com/Artimezoft/payroll_arg_reportes/blob/develop/docs/libro-de-sueldos.md)
 - Sicore
 - F.1357
 
 
 ### Reportes Sindicales
```

### Comparing `payroll_arg_reportes-0.0.19/pyproject.toml` & `payroll_arg_reportes-0.0.20/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "payroll_arg_reportes"
-version = "0.0.19"
+version = "0.0.20"
 dependencies = [
   "numero-a-letras>=0.0.4",
   "reportlab==4.0.8",
   "XlsxWriter==3.2.0",
 ]
 requires-python = ">=3.10"
 authors = [
```

### Comparing `payroll_arg_reportes-0.0.19/PKG-INFO` & `payroll_arg_reportes-0.0.20/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: payroll_arg_reportes
-Version: 0.0.19
+Version: 0.0.20
 Summary: Reportes para Payroll en Argentina
 Project-URL: Homepage, https://github.com/Artimezoft/payroll_arg_reportes
 Project-URL: Issues, https://github.com/Artimezoft/payroll_arg_reportes/issues
 Author-email: Eugenio <coding_with@eugeniovazquez.com.ar>, Andres <andres@data99.com.ar>
 Maintainer-email: Eugenio <coding_with@eugeniovazquez.com.ar>, Andres <andres@data99.com.ar>
 License: MIT License
         
@@ -52,15 +52,15 @@
    - 3: Descuento
  - Los campos `pk` se refieren a _primary key_ y no son necesarios para la generación de los reportes.
  - Puede haber más campos en tus datos, esta librería solo necesita los campos que se mencionan en cada reporte.
 
 ### Reportes Legales
 
 - [Recibo de Sueldos](https://github.com/Artimezoft/payroll_arg_reportes/blob/develop/docs/recibo-de-sueldos.md)
-- F.931
+- [F.931](https://github.com/Artimezoft/payroll_arg_reportes/blob/develop/docs/f931.md)
 - Libro de Sueldos Digital
 - [Libro de Sueldos](https://github.com/Artimezoft/payroll_arg_reportes/blob/develop/docs/libro-de-sueldos.md)
 - Sicore
 - F.1357
 
 
 ### Reportes Sindicales
```

