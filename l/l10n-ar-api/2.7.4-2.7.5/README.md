# Comparing `tmp/l10n_ar_api-2.7.4.tar.gz` & `tmp/l10n_ar_api-2.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "l10n_ar_api-2.7.4.tar", last modified: Mon Apr 29 14:42:57 2024, max compression
+gzip compressed data, was "l10n_ar_api-2.7.5.tar", last modified: Mon May 20 20:17:52 2024, max compression
```

## Comparing `l10n_ar_api-2.7.4.tar` & `l10n_ar_api-2.7.5.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-04-29 14:42:57.386157 l10n_ar_api-2.7.4/
--rw-r--r--   0 lbaldi     (501) staff       (20)      729 2024-04-29 14:42:57.385867 l10n_ar_api-2.7.4/PKG-INFO
--rwxr-xr-x   0 lbaldi     (501) staff       (20)     1391 2023-12-07 15:36:31.000000 l10n_ar_api-2.7.4/README.md
-drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-04-29 14:42:57.350695 l10n_ar_api-2.7.4/l10n_ar_api/
--rwxr-xr-x   0 lbaldi     (501) staff       (20)      206 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.4/l10n_ar_api/__init__.py
-drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-04-29 14:42:57.353537 l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/
--rwxr-xr-x   0 lbaldi     (501) staff       (20)      188 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/__init__.py
--rwxr-xr-x   0 lbaldi     (501) staff       (20)     1324 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/config.py
-drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-04-29 14:42:57.354527 l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/ws_sr_padron/
--rwxrwxrwx   0 lbaldi     (501) staff       (20)       27 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/ws_sr_padron/__init__.py
--rwxr-xr-x   0 lbaldi     (501) staff       (20)     1764 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/ws_sr_padron/ws_sr_padron.py
-drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-04-29 14:42:57.356791 l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/wsaa/
--rwxrwxrwx   0 lbaldi     (501) staff       (20)       66 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/wsaa/__init__.py
--rwxrwxrwx   0 lbaldi     (501) staff       (20)     1830 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/wsaa/certificate.py
--rwxr-xr-x   0 lbaldi     (501) staff       (20)     4964 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/wsaa/tokens.py
--rwxr-xr-x   0 lbaldi     (501) staff       (20)      944 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/wsaa/wsaa.py
-drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-04-29 14:42:57.358665 l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/wsbfe/
--rw-r--r--   0 lbaldi     (501) staff       (20)       62 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/wsbfe/__init__.py
--rw-r--r--   0 lbaldi     (501) staff       (20)      218 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/wsbfe/error.py
--rw-r--r--   0 lbaldi     (501) staff       (20)     3749 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/wsbfe/invoice.py
--rw-r--r--   0 lbaldi     (501) staff       (20)    12022 2023-10-18 16:07:13.000000 l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/wsbfe/wsbfe.py
-drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-04-29 14:42:57.360968 l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/wsct/
--rwxr-xr-x   0 lbaldi     (501) staff       (20)       60 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/wsct/__init__.py
--rwxr-xr-x   0 lbaldi     (501) staff       (20)      296 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/wsct/error.py
--rwxr-xr-x   0 lbaldi     (501) staff       (20)     5025 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/wsct/invoice.py
--rw-r--r--   0 lbaldi     (501) staff       (20)    17475 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/wsct/wsct.py
-drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-04-29 14:42:57.363315 l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/wsfe/
--rwxr-xr-x   0 lbaldi     (501) staff       (20)       88 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/wsfe/__init__.py
--rwxrwxrwx   0 lbaldi     (501) staff       (20)      248 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/wsfe/error.py
--rwxr-xr-x   0 lbaldi     (501) staff       (20)     4499 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/wsfe/invoice.py
--rw-r--r--   0 lbaldi     (501) staff       (20)      879 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/wsfe/qr_generator.py
--rw-r--r--   0 lbaldi     (501) staff       (20)    14310 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/wsfe/wsfe.py
-drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-04-29 14:42:57.365429 l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/wsfex/
--rwxrwxrwx   0 lbaldi     (501) staff       (20)       62 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/wsfex/__init__.py
--rwxrwxrwx   0 lbaldi     (501) staff       (20)      222 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/wsfex/error.py
--rwxr-xr-x   0 lbaldi     (501) staff       (20)     4326 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/wsfex/invoice.py
--rwxr-xr-x   0 lbaldi     (501) staff       (20)    12271 2023-10-18 16:07:13.000000 l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/wsfex/wsfex.py
-drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-04-29 14:42:57.367000 l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/wstesimbrefiscal/
--rwxr-xr-x   0 lbaldi     (501) staff       (20)       50 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/wstesimbrefiscal/__init__.py
--rwxr-xr-x   0 lbaldi     (501) staff       (20)      282 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/wstesimbrefiscal/error.py
--rw-r--r--   0 lbaldi     (501) staff       (20)     5574 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/wstesimbrefiscal/wstesimbrefiscal.py
-drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-04-29 14:42:57.368652 l10n_ar_api-2.7.4/l10n_ar_api/anmat_webservices/
--rw-r--r--   0 lbaldi     (501) staff       (20)       41 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.4/l10n_ar_api/anmat_webservices/__init__.py
--rw-r--r--   0 lbaldi     (501) staff       (20)     4923 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.4/l10n_ar_api/anmat_webservices/anmat.py
--rwxr-xr-x   0 lbaldi     (501) staff       (20)      199 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.4/l10n_ar_api/anmat_webservices/config.py
-drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-04-29 14:42:57.370177 l10n_ar_api-2.7.4/l10n_ar_api/arba_webservices/
--rwxrwxrwx   0 lbaldi     (501) staff       (20)      939 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.4/l10n_ar_api/arba_webservices/__init__.py
--rwxrwxrwx   0 lbaldi     (501) staff       (20)      252 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.4/l10n_ar_api/arba_webservices/config.py
-drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-04-29 14:42:57.371892 l10n_ar_api-2.7.4/l10n_ar_api/arba_webservices/cot/
--rw-r--r--   0 lbaldi     (501) staff       (20)       26 2023-12-07 15:36:31.000000 l10n_ar_api-2.7.4/l10n_ar_api/arba_webservices/cot/__init__.py
--rwxr-xr-x   0 lbaldi     (501) staff       (20)     1251 2023-12-07 15:36:31.000000 l10n_ar_api-2.7.4/l10n_ar_api/arba_webservices/cot/config.py
--rwxr-xr-x   0 lbaldi     (501) staff       (20)    20330 2024-01-22 14:51:58.000000 l10n_ar_api-2.7.4/l10n_ar_api/arba_webservices/cot/cot.py
--rwxr-xr-x   0 lbaldi     (501) staff       (20)     1979 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.4/l10n_ar_api/arba_webservices/iibb.py
-drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-04-29 14:42:57.374010 l10n_ar_api-2.7.4/l10n_ar_api/documents/
--rwxrwxrwx   0 lbaldi     (501) staff       (20)      101 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.4/l10n_ar_api/documents/__init__.py
--rwxrwxrwx   0 lbaldi     (501) staff       (20)      597 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.4/l10n_ar_api/documents/invoice.py
--rwxrwxrwx   0 lbaldi     (501) staff       (20)      611 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.4/l10n_ar_api/documents/tax.py
-drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-04-29 14:42:57.375858 l10n_ar_api-2.7.4/l10n_ar_api/documents/tests/
--rwxrwxrwx   0 lbaldi     (501) staff       (20)       85 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.4/l10n_ar_api/documents/tests/__init__.py
--rwxrwxrwx   0 lbaldi     (501) staff       (20)     1568 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.4/l10n_ar_api/documents/tests/test_gross_income.py
--rwxrwxrwx   0 lbaldi     (501) staff       (20)     2377 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.4/l10n_ar_api/documents/tests/test_profit.py
--rwxrwxrwx   0 lbaldi     (501) staff       (20)      246 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.4/l10n_ar_api/documents/tests/test_tribute.py
--rwxr-xr-x   0 lbaldi     (501) staff       (20)     3553 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.4/l10n_ar_api/documents/tribute.py
-drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-04-29 14:42:57.377603 l10n_ar_api-2.7.4/l10n_ar_api/padron/
--rwxrwxrwx   0 lbaldi     (501) staff       (20)       46 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.4/l10n_ar_api/padron/__init__.py
--rwxr-xr-x   0 lbaldi     (501) staff       (20)    10346 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.4/l10n_ar_api/padron/banks.py
--rw-r--r--   0 lbaldi     (501) staff       (20)       60 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.4/l10n_ar_api/padron/config.py
--rwxr-xr-x   0 lbaldi     (501) staff       (20)      712 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.4/l10n_ar_api/padron/contributor.py
-drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-04-29 14:42:57.378783 l10n_ar_api-2.7.4/l10n_ar_api/padron/test/
--rwxrwxrwx   0 lbaldi     (501) staff       (20)       57 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.4/l10n_ar_api/padron/test/__init__.py
--rwxrwxrwx   0 lbaldi     (501) staff       (20)      836 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.4/l10n_ar_api/padron/test/test_banks.py
--rwxrwxrwx   0 lbaldi     (501) staff       (20)      899 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.4/l10n_ar_api/padron/test/test_contributors.py
-drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-04-29 14:42:57.379945 l10n_ar_api-2.7.4/l10n_ar_api/presentations/
--rwxrwxrwx   0 lbaldi     (501) staff       (20)       59 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.4/l10n_ar_api/presentations/__init__.py
--rwxrwxrwx   0 lbaldi     (501) staff       (20)     2253 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.4/l10n_ar_api/presentations/presentation.py
--rwxr-xr-x   0 lbaldi     (501) staff       (20)   141463 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.4/l10n_ar_api/presentations/presentation_line.py
-drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-04-29 14:42:57.385184 l10n_ar_api-2.7.4/l10n_ar_api/presentations/test/
--rwxr-xr-x   0 lbaldi     (501) staff       (20)      209 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.4/l10n_ar_api/presentations/test/__init__.py
--rwxrwxrwx   0 lbaldi     (501) staff       (20)     8316 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.4/l10n_ar_api/presentations/test/test_purchases_sales_presentation.py
--rwxrwxrwx   0 lbaldi     (501) staff       (20)     9156 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.4/l10n_ar_api/presentations/test/test_purchases_sales_presentation_line.py
--rw-r--r--   0 lbaldi     (501) staff       (20)     7411 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.4/l10n_ar_api/presentations/test/test_purchases_sales_vat_digital_book.py
--rw-r--r--   0 lbaldi     (501) staff       (20)     8082 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.4/l10n_ar_api/presentations/test/test_purchases_sales_vat_digital_book_line.py
-drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-04-29 14:42:57.352626 l10n_ar_api-2.7.4/l10n_ar_api.egg-info/
--rwxrwxrwx   0 lbaldi     (501) staff       (20)      729 2024-04-29 14:42:57.000000 l10n_ar_api-2.7.4/l10n_ar_api.egg-info/PKG-INFO
--rwxrwxrwx   0 lbaldi     (501) staff       (20)     2904 2024-04-29 14:42:57.000000 l10n_ar_api-2.7.4/l10n_ar_api.egg-info/SOURCES.txt
--rwxrwxrwx   0 lbaldi     (501) staff       (20)        1 2024-04-29 14:42:57.000000 l10n_ar_api-2.7.4/l10n_ar_api.egg-info/dependency_links.txt
--rwxrwxrwx   0 lbaldi     (501) staff       (20)       84 2024-04-29 14:42:57.000000 l10n_ar_api-2.7.4/l10n_ar_api.egg-info/requires.txt
--rwxrwxrwx   0 lbaldi     (501) staff       (20)       12 2024-04-29 14:42:57.000000 l10n_ar_api-2.7.4/l10n_ar_api.egg-info/top_level.txt
--rw-r--r--   0 lbaldi     (501) staff       (20)       38 2024-04-29 14:42:57.386314 l10n_ar_api-2.7.4/setup.cfg
--rwxr-xr-x   0 lbaldi     (501) staff       (20)     1285 2024-04-29 14:42:36.000000 l10n_ar_api-2.7.4/setup.py
+drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-05-20 20:17:52.464404 l10n_ar_api-2.7.5/
+-rw-r--r--   0 lbaldi     (501) staff       (20)      729 2024-05-20 20:17:52.464145 l10n_ar_api-2.7.5/PKG-INFO
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)     1391 2023-12-07 15:36:31.000000 l10n_ar_api-2.7.5/README.md
+drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-05-20 20:17:52.432841 l10n_ar_api-2.7.5/l10n_ar_api/
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)      206 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.5/l10n_ar_api/__init__.py
+drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-05-20 20:17:52.435690 l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)      188 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/__init__.py
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)     1324 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/config.py
+drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-05-20 20:17:52.436756 l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/ws_sr_padron/
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)       27 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/ws_sr_padron/__init__.py
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)     1764 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/ws_sr_padron/ws_sr_padron.py
+drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-05-20 20:17:52.438594 l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/wsaa/
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)       66 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/wsaa/__init__.py
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)     1830 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/wsaa/certificate.py
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)     4964 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/wsaa/tokens.py
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)      944 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/wsaa/wsaa.py
+drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-05-20 20:17:52.440593 l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/wsbfe/
+-rw-r--r--   0 lbaldi     (501) staff       (20)       62 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/wsbfe/__init__.py
+-rw-r--r--   0 lbaldi     (501) staff       (20)      218 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/wsbfe/error.py
+-rw-r--r--   0 lbaldi     (501) staff       (20)     3749 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/wsbfe/invoice.py
+-rw-r--r--   0 lbaldi     (501) staff       (20)    12022 2023-10-18 16:07:13.000000 l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/wsbfe/wsbfe.py
+drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-05-20 20:17:52.442599 l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/wsct/
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)       60 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/wsct/__init__.py
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)      296 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/wsct/error.py
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)     5025 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/wsct/invoice.py
+-rw-r--r--   0 lbaldi     (501) staff       (20)    17475 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/wsct/wsct.py
+drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-05-20 20:17:52.445150 l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/wsfe/
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)       88 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/wsfe/__init__.py
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)      248 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/wsfe/error.py
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)     4499 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/wsfe/invoice.py
+-rw-r--r--   0 lbaldi     (501) staff       (20)      879 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/wsfe/qr_generator.py
+-rw-r--r--   0 lbaldi     (501) staff       (20)    14310 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/wsfe/wsfe.py
+drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-05-20 20:17:52.446798 l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/wsfex/
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)       62 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/wsfex/__init__.py
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)      222 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/wsfex/error.py
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)     4326 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/wsfex/invoice.py
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)    12271 2023-10-18 16:07:13.000000 l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/wsfex/wsfex.py
+drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-05-20 20:17:52.448238 l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/wstesimbrefiscal/
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)       50 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/wstesimbrefiscal/__init__.py
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)      282 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/wstesimbrefiscal/error.py
+-rw-r--r--   0 lbaldi     (501) staff       (20)     5574 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/wstesimbrefiscal/wstesimbrefiscal.py
+drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-05-20 20:17:52.449924 l10n_ar_api-2.7.5/l10n_ar_api/anmat_webservices/
+-rw-r--r--   0 lbaldi     (501) staff       (20)       41 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.5/l10n_ar_api/anmat_webservices/__init__.py
+-rw-r--r--   0 lbaldi     (501) staff       (20)     4923 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.5/l10n_ar_api/anmat_webservices/anmat.py
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)      199 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.5/l10n_ar_api/anmat_webservices/config.py
+drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-05-20 20:17:52.451372 l10n_ar_api-2.7.5/l10n_ar_api/arba_webservices/
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)      939 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.5/l10n_ar_api/arba_webservices/__init__.py
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)      252 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.5/l10n_ar_api/arba_webservices/config.py
+drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-05-20 20:17:52.452946 l10n_ar_api-2.7.5/l10n_ar_api/arba_webservices/cot/
+-rw-r--r--   0 lbaldi     (501) staff       (20)       26 2023-12-07 15:36:31.000000 l10n_ar_api-2.7.5/l10n_ar_api/arba_webservices/cot/__init__.py
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)     1251 2023-12-07 15:36:31.000000 l10n_ar_api-2.7.5/l10n_ar_api/arba_webservices/cot/config.py
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)    20330 2024-01-22 14:51:58.000000 l10n_ar_api-2.7.5/l10n_ar_api/arba_webservices/cot/cot.py
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)     1979 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.5/l10n_ar_api/arba_webservices/iibb.py
+drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-05-20 20:17:52.454996 l10n_ar_api-2.7.5/l10n_ar_api/documents/
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)      101 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.5/l10n_ar_api/documents/__init__.py
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)      597 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.5/l10n_ar_api/documents/invoice.py
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)      611 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.5/l10n_ar_api/documents/tax.py
+drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-05-20 20:17:52.456301 l10n_ar_api-2.7.5/l10n_ar_api/documents/tests/
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)       85 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.5/l10n_ar_api/documents/tests/__init__.py
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)     1568 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.5/l10n_ar_api/documents/tests/test_gross_income.py
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)     2377 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.5/l10n_ar_api/documents/tests/test_profit.py
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)      246 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.5/l10n_ar_api/documents/tests/test_tribute.py
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)     3759 2024-05-20 20:17:23.000000 l10n_ar_api-2.7.5/l10n_ar_api/documents/tribute.py
+drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-05-20 20:17:52.457760 l10n_ar_api-2.7.5/l10n_ar_api/padron/
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)       46 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.5/l10n_ar_api/padron/__init__.py
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)    10346 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.5/l10n_ar_api/padron/banks.py
+-rw-r--r--   0 lbaldi     (501) staff       (20)       60 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.5/l10n_ar_api/padron/config.py
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)      712 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.5/l10n_ar_api/padron/contributor.py
+drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-05-20 20:17:52.458836 l10n_ar_api-2.7.5/l10n_ar_api/padron/test/
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)       57 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.5/l10n_ar_api/padron/test/__init__.py
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)      836 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.5/l10n_ar_api/padron/test/test_banks.py
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)      899 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.5/l10n_ar_api/padron/test/test_contributors.py
+drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-05-20 20:17:52.459970 l10n_ar_api-2.7.5/l10n_ar_api/presentations/
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)       59 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.5/l10n_ar_api/presentations/__init__.py
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)     2253 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.5/l10n_ar_api/presentations/presentation.py
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)   141463 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.5/l10n_ar_api/presentations/presentation_line.py
+drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-05-20 20:17:52.463437 l10n_ar_api-2.7.5/l10n_ar_api/presentations/test/
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)      209 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.5/l10n_ar_api/presentations/test/__init__.py
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)     8316 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.5/l10n_ar_api/presentations/test/test_purchases_sales_presentation.py
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)     9156 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.5/l10n_ar_api/presentations/test/test_purchases_sales_presentation_line.py
+-rw-r--r--   0 lbaldi     (501) staff       (20)     7411 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.5/l10n_ar_api/presentations/test/test_purchases_sales_vat_digital_book.py
+-rw-r--r--   0 lbaldi     (501) staff       (20)     8082 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.5/l10n_ar_api/presentations/test/test_purchases_sales_vat_digital_book_line.py
+drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-05-20 20:17:52.434660 l10n_ar_api-2.7.5/l10n_ar_api.egg-info/
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)      729 2024-05-20 20:17:52.000000 l10n_ar_api-2.7.5/l10n_ar_api.egg-info/PKG-INFO
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)     2904 2024-05-20 20:17:52.000000 l10n_ar_api-2.7.5/l10n_ar_api.egg-info/SOURCES.txt
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)        1 2024-05-20 20:17:52.000000 l10n_ar_api-2.7.5/l10n_ar_api.egg-info/dependency_links.txt
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)       84 2024-05-20 20:17:52.000000 l10n_ar_api-2.7.5/l10n_ar_api.egg-info/requires.txt
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)       12 2024-05-20 20:17:52.000000 l10n_ar_api-2.7.5/l10n_ar_api.egg-info/top_level.txt
+-rw-r--r--   0 lbaldi     (501) staff       (20)       38 2024-05-20 20:17:52.464504 l10n_ar_api-2.7.5/setup.cfg
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)     1285 2024-05-20 20:17:23.000000 l10n_ar_api-2.7.5/setup.py
```

### Comparing `l10n_ar_api-2.7.4/PKG-INFO` & `l10n_ar_api-2.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: l10n_ar_api
-Version: 2.7.4
+Version: 2.7.5
 Summary: Libreria para localizacion Argentina
 Home-page: https://github.com/odoo-arg/l10n_ar_api
 Author: BLUEORANGE GROUP SRL
 Author-email: daniel@blueorange.com.ar
 License: UNKNOWN
 Description: Libreria para localizacion Argentina
 Keywords: Libreria para localizacion Argentina
```

### Comparing `l10n_ar_api-2.7.4/README.md` & `l10n_ar_api-2.7.5/README.md`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/config.py` & `l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/config.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/ws_sr_padron/ws_sr_padron.py` & `l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/ws_sr_padron/ws_sr_padron.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/wsaa/certificate.py` & `l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/wsaa/certificate.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/wsaa/tokens.py` & `l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/wsaa/tokens.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/wsaa/wsaa.py` & `l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/wsaa/wsaa.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/wsbfe/invoice.py` & `l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/wsbfe/invoice.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/wsbfe/wsbfe.py` & `l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/wsbfe/wsbfe.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/wsct/invoice.py` & `l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/wsct/invoice.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/wsct/wsct.py` & `l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/wsct/wsct.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/wsfe/invoice.py` & `l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/wsfe/invoice.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/wsfe/qr_generator.py` & `l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/wsfe/qr_generator.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/wsfe/wsfe.py` & `l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/wsfe/wsfe.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/wsfex/invoice.py` & `l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/wsfex/invoice.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/wsfex/wsfex.py` & `l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/wsfex/wsfex.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.4/l10n_ar_api/afip_webservices/wstesimbrefiscal/wstesimbrefiscal.py` & `l10n_ar_api-2.7.5/l10n_ar_api/afip_webservices/wstesimbrefiscal/wstesimbrefiscal.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.4/l10n_ar_api/anmat_webservices/anmat.py` & `l10n_ar_api-2.7.5/l10n_ar_api/anmat_webservices/anmat.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.4/l10n_ar_api/arba_webservices/__init__.py` & `l10n_ar_api-2.7.5/l10n_ar_api/arba_webservices/__init__.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.4/l10n_ar_api/arba_webservices/cot/config.py` & `l10n_ar_api-2.7.5/l10n_ar_api/arba_webservices/cot/config.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.4/l10n_ar_api/arba_webservices/cot/cot.py` & `l10n_ar_api-2.7.5/l10n_ar_api/arba_webservices/cot/cot.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.4/l10n_ar_api/arba_webservices/iibb.py` & `l10n_ar_api-2.7.5/l10n_ar_api/arba_webservices/iibb.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.4/l10n_ar_api/documents/invoice.py` & `l10n_ar_api-2.7.5/l10n_ar_api/documents/invoice.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.4/l10n_ar_api/documents/tax.py` & `l10n_ar_api-2.7.5/l10n_ar_api/documents/tax.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.4/l10n_ar_api/documents/tests/test_gross_income.py` & `l10n_ar_api-2.7.5/l10n_ar_api/documents/tests/test_gross_income.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.4/l10n_ar_api/documents/tests/test_profit.py` & `l10n_ar_api-2.7.5/l10n_ar_api/documents/tests/test_profit.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.4/l10n_ar_api/documents/tribute.py` & `l10n_ar_api-2.7.5/l10n_ar_api/documents/tribute.py`

 * *Files 9% similar despite different names*

```diff
@@ -79,31 +79,33 @@
 
 
 class Profit:
 
     def __init__(self):
         self.activity = None
 
-    def calculate_value(self, accumulated, amount_to_pay):
+    def calculate_value(self, accumulated, amount_to_pay, first_retention=True):
         """
         Devuelve el valor a retener/percibir para la actividad
         :param accumulated: Acumulado de pagos necesario para deducir el valor
         :param amount_to_pay: Importe a pagar sin impuestos
+        :param first_retention: Si es la primera retencion, se restará el minimo no imponible
         :return: Base imponible y Valor que se debe retener
         """
         if not self.activity:
             raise AttributeError("Agregar actividad en el tributo antes de calcular el valor")
 
         minimum_no_aplicable = self.activity.minimum_no_aplicable
         # El acumulado se debe restar siempre, excepto en el caso que el acumulado sea mayor al minimo no imponible
         # y no se haya retenido por primera vez (porque no sobrepaso el minimo), entonces en ese caso el valor de la
         # retencion es por la anterior + la actual
-        if ((accumulated - minimum_no_aplicable) * self.activity.percentage / 100) >= self.activity.minimum_tax:
+        if ((accumulated - minimum_no_aplicable) * self.activity.percentage / 100) >= self.activity.minimum_tax\
+                and first_retention:
             accumulated = minimum_no_aplicable
 
-        base = amount_to_pay + accumulated - minimum_no_aplicable
+        base = amount_to_pay + accumulated - minimum_no_aplicable if first_retention else amount_to_pay + accumulated
         value = apply_rounding(base * (self.activity.percentage / 100))
 
         if value < self.activity.minimum_tax:
             value = 0
 
         return base, value
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `l10n_ar_api-2.7.4/l10n_ar_api/padron/banks.py` & `l10n_ar_api-2.7.5/l10n_ar_api/padron/banks.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.4/l10n_ar_api/padron/contributor.py` & `l10n_ar_api-2.7.5/l10n_ar_api/padron/contributor.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.4/l10n_ar_api/padron/test/test_banks.py` & `l10n_ar_api-2.7.5/l10n_ar_api/padron/test/test_banks.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.4/l10n_ar_api/padron/test/test_contributors.py` & `l10n_ar_api-2.7.5/l10n_ar_api/padron/test/test_contributors.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.4/l10n_ar_api/presentations/presentation.py` & `l10n_ar_api-2.7.5/l10n_ar_api/presentations/presentation.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.4/l10n_ar_api/presentations/presentation_line.py` & `l10n_ar_api-2.7.5/l10n_ar_api/presentations/presentation_line.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.4/l10n_ar_api/presentations/test/test_purchases_sales_presentation.py` & `l10n_ar_api-2.7.5/l10n_ar_api/presentations/test/test_purchases_sales_presentation.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.4/l10n_ar_api/presentations/test/test_purchases_sales_presentation_line.py` & `l10n_ar_api-2.7.5/l10n_ar_api/presentations/test/test_purchases_sales_presentation_line.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.4/l10n_ar_api/presentations/test/test_purchases_sales_vat_digital_book.py` & `l10n_ar_api-2.7.5/l10n_ar_api/presentations/test/test_purchases_sales_vat_digital_book.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.4/l10n_ar_api/presentations/test/test_purchases_sales_vat_digital_book_line.py` & `l10n_ar_api-2.7.5/l10n_ar_api/presentations/test/test_purchases_sales_vat_digital_book_line.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.4/l10n_ar_api.egg-info/PKG-INFO` & `l10n_ar_api-2.7.5/l10n_ar_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: l10n-ar-api
-Version: 2.7.4
+Version: 2.7.5
 Summary: Libreria para localizacion Argentina
 Home-page: https://github.com/odoo-arg/l10n_ar_api
 Author: BLUEORANGE GROUP SRL
 Author-email: daniel@blueorange.com.ar
 License: UNKNOWN
 Description: Libreria para localizacion Argentina
 Keywords: Libreria para localizacion Argentina
```

### Comparing `l10n_ar_api-2.7.4/l10n_ar_api.egg-info/SOURCES.txt` & `l10n_ar_api-2.7.5/l10n_ar_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.4/setup.py` & `l10n_ar_api-2.7.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 if sys.version_info[0] >= 3:
     install_requires.append('bs4')
 else:
     install_requires.append('BeautifulSoup')
 
 setup(
     name='l10n_ar_api',
-    version='2.7.4',
+    version='2.7.5',
     description='Libreria para localizacion Argentina',
     long_description='Libreria para localizacion Argentina',
     url='https://github.com/odoo-arg/l10n_ar_api',
     author='BLUEORANGE GROUP SRL',
     author_email='daniel@blueorange.com.ar',
     license='',
     classifiers=[
```

