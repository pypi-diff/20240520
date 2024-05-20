# Comparing `tmp/aempsconn-0.1.3.1.tar.gz` & `tmp/aempsconn-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aempsconn-0.1.3.1.tar", max compression
+gzip compressed data, was "aempsconn-1.0.0.tar", max compression
```

## Comparing `aempsconn-0.1.3.1.tar` & `aempsconn-1.0.0.tar`

### file list

```diff
@@ -1,40 +1,43 @@
--rw-r--r--   0        0        0     1063 2023-10-09 08:28:26.633576 aempsconn-0.1.3.1/LICENSE
--rw-r--r--   0        0        0     4026 2023-10-09 08:28:26.633576 aempsconn-0.1.3.1/README.md
--rw-r--r--   0        0        0      131 2023-10-09 08:28:26.633576 aempsconn-0.1.3.1/aempsconn/__init__.py
--rw-r--r--   0        0        0      555 2023-10-09 08:28:26.633576 aempsconn-0.1.3.1/aempsconn/datatypes/__init__.py
--rw-r--r--   0        0        0      327 2023-10-09 08:28:26.633576 aempsconn-0.1.3.1/aempsconn/datatypes/atc.py
--rw-r--r--   0        0        0      755 2023-10-09 08:28:26.633576 aempsconn-0.1.3.1/aempsconn/datatypes/documento.py
--rw-r--r--   0        0        0      380 2023-10-09 08:28:26.633576 aempsconn-0.1.3.1/aempsconn/datatypes/elemento.py
--rw-r--r--   0        0        0      374 2023-10-09 08:28:26.633576 aempsconn-0.1.3.1/aempsconn/datatypes/estado.py
--rw-r--r--   0        0        0      504 2023-10-09 08:28:26.633576 aempsconn-0.1.3.1/aempsconn/datatypes/excipiente.py
--rw-r--r--   0        0        0      430 2023-10-09 08:28:26.633576 aempsconn-0.1.3.1/aempsconn/datatypes/foto.py
--rw-r--r--   0        0        0     7792 2023-10-09 08:28:26.633576 aempsconn-0.1.3.1/aempsconn/datatypes/medicamento.py
--rw-r--r--   0        0        0      607 2023-10-09 08:28:26.633576 aempsconn-0.1.3.1/aempsconn/datatypes/pactivo.py
--rw-r--r--   0        0        0      847 2023-10-09 08:28:26.633576 aempsconn-0.1.3.1/aempsconn/datatypes/presentacion.py
--rw-r--r--   0        0        0      483 2023-10-09 08:28:26.633576 aempsconn-0.1.3.1/aempsconn/datatypes/seccion.py
--rw-r--r--   0        0        0      602 2023-10-09 08:28:26.633576 aempsconn-0.1.3.1/aempsconn/datatypes/suministro.py
--rw-r--r--   0        0        0       94 2023-10-09 08:28:26.633576 aempsconn-0.1.3.1/aempsconn/decorators/__init__.py
--rw-r--r--   0        0        0     1480 2023-10-09 08:28:26.633576 aempsconn-0.1.3.1/aempsconn/decorators/http_res_handler.py
--rw-r--r--   0        0        0      888 2023-10-09 08:28:26.633576 aempsconn-0.1.3.1/aempsconn/decorators/json_res_handler.py
--rw-r--r--   0        0        0      162 2023-10-09 08:28:26.637576 aempsconn-0.1.3.1/aempsconn/errors/__init__.py
--rw-r--r--   0        0        0     2353 2023-10-09 08:28:26.637576 aempsconn-0.1.3.1/aempsconn/errors/errors.py
--rw-r--r--   0        0        0      651 2023-10-09 08:28:26.637576 aempsconn-0.1.3.1/aempsconn/filter/__init__.py
--rw-r--r--   0        0        0      872 2023-10-09 08:28:26.637576 aempsconn-0.1.3.1/aempsconn/filter/filter.py
--rw-r--r--   0        0        0     1659 2023-10-09 08:28:26.637576 aempsconn-0.1.3.1/aempsconn/filter/filter_medicamento.py
--rw-r--r--   0        0        0     9645 2023-10-09 08:28:26.637576 aempsconn-0.1.3.1/aempsconn/filter/filter_medicamentos.py
--rw-r--r--   0        0        0       40 2023-10-09 08:28:26.637576 aempsconn-0.1.3.1/aempsconn/logger/__init__.py
--rw-r--r--   0        0        0      401 2023-10-09 08:28:26.637576 aempsconn-0.1.3.1/aempsconn/logger/custom_logger.py
--rw-r--r--   0        0        0      927 2023-10-09 08:28:26.637576 aempsconn-0.1.3.1/aempsconn/logger/formatter.py
--rw-r--r--   0        0        0       23 2023-10-09 08:28:26.637576 aempsconn-0.1.3.1/aempsconn/modules/__init__.py
--rw-r--r--   0        0        0     1496 2023-10-09 08:28:26.637576 aempsconn-0.1.3.1/aempsconn/modules/base.py
--rw-r--r--   0        0        0       76 2023-10-09 08:28:26.637576 aempsconn-0.1.3.1/aempsconn/modules/cima/__init__.py
--rw-r--r--   0        0        0     1318 2023-10-09 08:28:26.637576 aempsconn-0.1.3.1/aempsconn/modules/cima/medicamento.py
--rw-r--r--   0        0        0     1627 2023-10-09 08:28:26.637576 aempsconn-0.1.3.1/aempsconn/modules/cima/medicamentos.py
--rw-r--r--   0        0        0       37 2023-10-09 08:28:26.637576 aempsconn-0.1.3.1/aempsconn/orchestrate/__init__.py
--rw-r--r--   0        0        0     1639 2023-10-09 08:28:26.637576 aempsconn-0.1.3.1/aempsconn/orchestrate/orchestrate.py
--rw-r--r--   0        0        0       72 2023-10-09 08:28:26.637576 aempsconn-0.1.3.1/aempsconn/utils/__init__.py
--rw-r--r--   0        0        0      736 2023-10-09 08:28:26.637576 aempsconn-0.1.3.1/aempsconn/utils/config.py
--rw-r--r--   0        0        0      391 2023-10-09 08:28:26.637576 aempsconn-0.1.3.1/aempsconn/utils/endpoint.py
--rw-r--r--   0        0        0      194 2023-10-09 08:28:26.637576 aempsconn-0.1.3.1/aempsconn/utils/signal_handler.py
--rw-r--r--   0        0        0      646 2023-10-09 08:28:26.637576 aempsconn-0.1.3.1/pyproject.toml
--rw-r--r--   0        0        0     4942 1970-01-01 00:00:00.000000 aempsconn-0.1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-20 18:41:47.580822 aempsconn-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2109 2024-05-20 18:41:47.580822 aempsconn-1.0.0/README.md
+-rw-r--r--   0        0        0      599 2024-05-20 18:41:47.580822 aempsconn-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1387 2024-05-20 18:41:47.580822 aempsconn-1.0.0/src/aempsconn/aemps.py
+-rw-r--r--   0        0        0      250 2024-05-20 18:41:47.580822 aempsconn-1.0.0/src/aempsconn/filter/__init__.py
+-rw-r--r--   0        0        0     2652 2024-05-20 18:41:47.580822 aempsconn-1.0.0/src/aempsconn/filter/maestras.py
+-rw-r--r--   0        0        0     1049 2024-05-20 18:41:47.580822 aempsconn-1.0.0/src/aempsconn/filter/medicamento.py
+-rw-r--r--   0        0        0     6457 2024-05-20 18:41:47.580822 aempsconn-1.0.0/src/aempsconn/filter/medicamentos.py
+-rw-r--r--   0        0        0     3111 2024-05-20 18:41:47.580822 aempsconn-1.0.0/src/aempsconn/filter/presentaciones.py
+-rw-r--r--   0        0        0     2253 2024-05-20 18:41:47.580822 aempsconn-1.0.0/src/aempsconn/filter/vmpp.py
+-rw-r--r--   0        0        0      180 2024-05-20 18:41:47.580822 aempsconn-1.0.0/src/aempsconn/modules/__init__.py
+-rw-r--r--   0        0        0      633 2024-05-20 18:41:47.580822 aempsconn-1.0.0/src/aempsconn/modules/medicamento.py
+-rw-r--r--   0        0        0      643 2024-05-20 18:41:47.580822 aempsconn-1.0.0/src/aempsconn/modules/medicamentos.py
+-rw-r--r--   0        0        0      664 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/modules/presentaciones.py
+-rw-r--r--   0        0        0      627 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/modules/vmpp.py
+-rw-r--r--   0        0        0       60 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/objects/__init__.py
+-rw-r--r--   0        0        0      155 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/objects/atc.py
+-rw-r--r--   0        0        0      223 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/objects/descripcion_clinica.py
+-rw-r--r--   0        0        0      560 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/objects/documento.py
+-rw-r--r--   0        0        0      250 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/objects/documento_material.py
+-rw-r--r--   0        0        0     1238 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/objects/estado.py
+-rw-r--r--   0        0        0      199 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/objects/excipiente.py
+-rw-r--r--   0        0        0      281 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/objects/foto.py
+-rw-r--r--   0        0        0      168 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/objects/item.py
+-rw-r--r--   0        0        0      345 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/objects/material.py
+-rw-r--r--   0        0        0     1248 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/objects/medicamento.py
+-rw-r--r--   0        0        0      464 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/objects/nota.py
+-rw-r--r--   0        0        0      601 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/objects/presentacion.py
+-rw-r--r--   0        0        0      218 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/objects/principio_activo.py
+-rw-r--r--   0        0        0      269 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/objects/problema_suministro.py
+-rw-r--r--   0        0        0      789 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/objects/registro_cambios.py
+-rw-r--r--   0        0        0      183 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/objects/seccion.py
+-rw-r--r--   0        0        0       48 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/utils/__init__.py
+-rw-r--r--   0        0        0      829 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/utils/constants.py
+-rw-r--r--   0        0        0      135 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/utils/filter/__init__.py
+-rw-r--r--   0        0        0      984 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/utils/filter/base_operator.py
+-rw-r--r--   0        0        0      576 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/utils/filter/filter.py
+-rw-r--r--   0        0        0      389 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/utils/filter/operator.py
+-rw-r--r--   0        0        0      753 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/utils/hof.py
+-rw-r--r--   0        0        0       95 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/utils/module/__init__.py
+-rw-r--r--   0        0        0     1454 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/utils/module/base_module.py
+-rw-r--r--   0        0        0     5157 2024-05-20 18:41:47.584822 aempsconn-1.0.0/src/aempsconn/utils/request_handler.py
+-rw-r--r--   0        0        0     2892 1970-01-01 00:00:00.000000 aempsconn-1.0.0/PKG-INFO
```

### Comparing `aempsconn-0.1.3.1/LICENSE` & `aempsconn-1.0.0/LICENSE`

 * *Files identical despite different names*

