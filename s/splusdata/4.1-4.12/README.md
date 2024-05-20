# Comparing `tmp/splusdata-4.1-py3-none-any.whl.zip` & `tmp/splusdata-4.12-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,28 +1,29 @@
-Zip file size: 38598 bytes, number of entries: 26
--rw-r--r--  2.0 unx      134 b- defN 23-Sep-26 02:34 splusdata/__init__.py
+Zip file size: 39481 bytes, number of entries: 27
+-rw-r--r--  2.0 unx      186 b- defN 24-May-20 18:29 splusdata/__init__.py
 -rw-r--r--  2.0 unx    16393 b- defN 23-Dec-02 21:19 splusdata/connect.py
--rw-r--r--  2.0 unx    23617 b- defN 24-Apr-14 23:09 splusdata/core.py
+-rw-r--r--  2.0 unx    23630 b- defN 24-Apr-26 14:08 splusdata/core.py
 -rw-rw-r--  2.0 unx    10239 b- defN 20-Nov-02 11:00 splusdata/get.py
 -rw-rw-r--  2.0 unx     1496 b- defN 20-Oct-28 17:36 splusdata/get_fits.py
 -rw-rw-r--  2.0 unx     9439 b- defN 20-Oct-11 08:08 splusdata/graph.py
 -rw-rw-r--  2.0 unx      965 b- defN 20-Nov-22 20:42 splusdata/imgs.py
 -rw-rw-r--  2.0 unx     9573 b- defN 20-Oct-11 08:08 splusdata/plot.py
 -rw-r--r--  2.0 unx     6158 b- defN 23-Dec-05 15:28 splusdata/readconf.py
 -rw-rw-r--  2.0 unx     2802 b- defN 20-Oct-11 08:08 splusdata/search_coords.py
 -rw-rw-r--  2.0 unx     3822 b- defN 20-Nov-02 11:00 splusdata/searchcoords.py
 -rw-rw-r--  2.0 unx        0 b- defN 21-May-11 08:16 splusdata/features/__init__.py
 -rw-rw-r--  2.0 unx     7397 b- defN 21-May-11 08:21 splusdata/features/filterbw.py
 -rw-rw-r--  2.0 unx    12215 b- defN 21-May-11 10:56 splusdata/features/g_star.py
+-rw-r--r--  2.0 unx     2039 b- defN 24-May-20 18:37 splusdata/features/hipscat.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Oct-13 23:48 splusdata/models/__init__.py
 -rw-r--r--  2.0 unx    12215 b- defN 23-Dec-02 21:19 splusdata/models/star_gal_quasar.py
 -rw-r--r--  2.0 unx       66 b- defN 22-Oct-13 23:48 splusdata/vacs/__init__.py
 -rw-r--r--  2.0 unx      760 b- defN 22-Oct-13 23:48 splusdata/vacs/pdfs.py
 -rw-r--r--  2.0 unx    13534 b- defN 23-Dec-02 21:19 splusdata/vacs/sqg.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Oct-13 23:48 splusdata/variability/__init__.py
--rw-rw-r--  2.0 unx    10255 b- defN 24-Apr-14 23:10 splusdata-4.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      574 b- defN 24-Apr-14 23:10 splusdata-4.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-14 23:10 splusdata-4.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       54 b- defN 24-Apr-14 23:10 splusdata-4.1.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       10 b- defN 24-Apr-14 23:10 splusdata-4.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2085 b- defN 24-Apr-14 23:10 splusdata-4.1.dist-info/RECORD
-26 files, 143895 bytes uncompressed, 35258 bytes compressed:  75.5%
+-rw-rw-r--  2.0 unx    10255 b- defN 24-May-20 18:39 splusdata-4.12.dist-info/LICENSE
+-rw-r--r--  2.0 unx      575 b- defN 24-May-20 18:39 splusdata-4.12.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-20 18:39 splusdata-4.12.dist-info/WHEEL
+-rw-r--r--  2.0 unx       54 b- defN 24-May-20 18:39 splusdata-4.12.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       10 b- defN 24-May-20 18:39 splusdata-4.12.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2177 b- defN 24-May-20 18:39 splusdata-4.12.dist-info/RECORD
+27 files, 146092 bytes uncompressed, 35995 bytes compressed:  75.4%
```

## zipnote {}

```diff
@@ -36,14 +36,17 @@
 
 Filename: splusdata/features/filterbw.py
 Comment: 
 
 Filename: splusdata/features/g_star.py
 Comment: 
 
+Filename: splusdata/features/hipscat.py
+Comment: 
+
 Filename: splusdata/models/__init__.py
 Comment: 
 
 Filename: splusdata/models/star_gal_quasar.py
 Comment: 
 
 Filename: splusdata/vacs/__init__.py
@@ -54,26 +57,26 @@
 
 Filename: splusdata/vacs/sqg.py
 Comment: 
 
 Filename: splusdata/variability/__init__.py
 Comment: 
 
-Filename: splusdata-4.1.dist-info/LICENSE
+Filename: splusdata-4.12.dist-info/LICENSE
 Comment: 
 
-Filename: splusdata-4.1.dist-info/METADATA
+Filename: splusdata-4.12.dist-info/METADATA
 Comment: 
 
-Filename: splusdata-4.1.dist-info/WHEEL
+Filename: splusdata-4.12.dist-info/WHEEL
 Comment: 
 
-Filename: splusdata-4.1.dist-info/entry_points.txt
+Filename: splusdata-4.12.dist-info/entry_points.txt
 Comment: 
 
-Filename: splusdata-4.1.dist-info/top_level.txt
+Filename: splusdata-4.12.dist-info/top_level.txt
 Comment: 
 
-Filename: splusdata-4.1.dist-info/RECORD
+Filename: splusdata-4.12.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## splusdata/__init__.py

```diff
@@ -1,6 +1,7 @@
 from splusdata.connect import connect
 
 from splusdata.features import filterbw
+from splusdata.features.hipscat import get_hipscats
 import splusdata.vacs
 
 from splusdata.core import Core
```

## splusdata/core.py

```diff
@@ -183,15 +183,15 @@
             If the response contains an error.
         """
         response = self.session.request(method, url, data=data, json=json_, params=params, headers=self.headers)
         
         if self.auto_renew and response.status_code == 401:
             print("Renewing splus session token.")
             self.authenticate(self.username, self.password)
-            response = self.session.request(method, url, data=data, json=json_, params=params, headers=self.headers)
+            response = self.session.request(method, url, data=data, json=json_, params=params, stream=True, headers=self.headers)
 
         resjson = None
         try:
             resjson = response.json()
         except:
             pass
```

## Comparing `splusdata-4.1.dist-info/LICENSE` & `splusdata-4.12.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `splusdata-4.1.dist-info/METADATA` & `splusdata-4.12.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splusdata
-Version: 4.1
+Version: 4.12
 Summary: Download SPLUS catalogs, FITS and more
 Home-page: https://github.com/schwarzam/splusdata
 Author: Gustavo Schwarz
 Author-email: gustavo.b.schwarz@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `splusdata-4.1.dist-info/RECORD` & `splusdata-4.12.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-splusdata/__init__.py,sha256=f3k0KS0i53Jy4PLHGLrbsGXzkmMGzU_FliQod9dG55c,134
+splusdata/__init__.py,sha256=qY9pANBVn8K2vH8V9KoabEsYlLcGF8VYzni3bA-YyP8,186
 splusdata/connect.py,sha256=scdf_oECqa8X7rSec3Oin4gl6WsYBRXUvDdZdUiqlos,16393
-splusdata/core.py,sha256=ZGw5sDifOOvu5uwvMvbYcv85ePjobW89W6OLxeF2nY0,23617
+splusdata/core.py,sha256=Ei4pZEGxiCxagCmobnaD0j8DG9aZH-uC9tEV5SkpX8I,23630
 splusdata/get.py,sha256=jgrP2XPR41gfN2rXymV3YHmaI2FHO9rCfT1iteXaZnI,10239
 splusdata/get_fits.py,sha256=2eV0kCnqkm1B9l5brRwkRiOIb0s400-pEC_9KG2UZeQ,1496
 splusdata/graph.py,sha256=X4RVvAZz6b-hbBo8xNpIEpGcY9tWEwKNrN-JVQGgBr8,9439
 splusdata/imgs.py,sha256=2DkjStXZ6LJuYyNzJ-3tC4NCHmUkT8wx3S-4n-TbTzU,965
 splusdata/plot.py,sha256=mlApJGefhRl1kg_ydNSNUqenD_VbU5ORIjWuhoERtTY,9573
 splusdata/readconf.py,sha256=jdWjy3JnmHZaZRGiyTy8wMU5Qrtt-8BvQqj_a0lvyBk,6158
 splusdata/search_coords.py,sha256=M74Rp2T1G52aX8x45PlihNOsclTVAiWVhF2Lg4At4HA,2802
 splusdata/searchcoords.py,sha256=-Fwk2T_poVS-dnwgvROw1g-os4BlB7Ui0Wr-iHp28No,3822
 splusdata/features/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 splusdata/features/filterbw.py,sha256=5gTxfQx33LhO6R3yMoi-Qf_iea8jUf13gMNN2A4VK8c,7397
 splusdata/features/g_star.py,sha256=keoD5JUYHN6Futeu9S9czVDay80wpnxKhA-rKOcUsew,12215
+splusdata/features/hipscat.py,sha256=y5NqlhiX9MvrI18QmO18UpEiC5kg5oJdZdNyqmoEvQw,2039
 splusdata/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 splusdata/models/star_gal_quasar.py,sha256=keoD5JUYHN6Futeu9S9czVDay80wpnxKhA-rKOcUsew,12215
 splusdata/vacs/__init__.py,sha256=3nIdhXDRGIZ7vCo83-sUpQREM9ewEZBt6YjyOn1hCxY,66
 splusdata/vacs/pdfs.py,sha256=0POHSQXINmnUy8bbpCJ9rvVjdbMMJxPLvnxyZ1mJzxQ,760
 splusdata/vacs/sqg.py,sha256=MimHAAkBLEKtFPFMi_6bjcF622DJ_fRJ43fMvwEcB4M,13534
 splusdata/variability/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-splusdata-4.1.dist-info/LICENSE,sha256=TRD-XzqhdrBbIpokiGa61wuDTBc_ElKoFP9HSNihODc,10255
-splusdata-4.1.dist-info/METADATA,sha256=osR8AecFqcBrL4CtS_ZbXjxmittiuxUACHaVYYrKnB8,574
-splusdata-4.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-splusdata-4.1.dist-info/entry_points.txt,sha256=aODiYSDboShwPhOCoVIQYDKyslYnPB66bg1IbUtq2_0,54
-splusdata-4.1.dist-info/top_level.txt,sha256=AhhSeP7Zw8JdgbX6waqMUKVjfXLucnDgFJ2RBh2D5AI,10
-splusdata-4.1.dist-info/RECORD,,
+splusdata-4.12.dist-info/LICENSE,sha256=TRD-XzqhdrBbIpokiGa61wuDTBc_ElKoFP9HSNihODc,10255
+splusdata-4.12.dist-info/METADATA,sha256=y4ivDbLEA5Q88W2nrfNaOuR7LszApTpdA-Z2MffOOao,575
+splusdata-4.12.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+splusdata-4.12.dist-info/entry_points.txt,sha256=aODiYSDboShwPhOCoVIQYDKyslYnPB66bg1IbUtq2_0,54
+splusdata-4.12.dist-info/top_level.txt,sha256=AhhSeP7Zw8JdgbX6waqMUKVjfXLucnDgFJ2RBh2D5AI,10
+splusdata-4.12.dist-info/RECORD,,
```

