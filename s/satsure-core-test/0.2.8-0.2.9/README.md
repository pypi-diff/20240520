# Comparing `tmp/satsure-core-test-0.2.8.tar.gz` & `tmp/satsure-core-test-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satsure-core-test-0.2.8.tar", last modified: Fri May 17 11:56:43 2024, max compression
+gzip compressed data, was "satsure-core-test-0.2.9.tar", last modified: Mon May 20 14:04:19 2024, max compression
```

## Comparing `satsure-core-test-0.2.8.tar` & `satsure-core-test-0.2.9.tar`

### file list

```diff
@@ -1,61 +1,75 @@
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-17 11:56:43.189221 satsure-core-test-0.2.8/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 07:48:02.000000 satsure-core-test-0.2.8/LICENCE.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      515 2024-05-17 11:56:43.189005 satsure-core-test-0.2.8/PKG-INFO
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 07:48:18.000000 satsure-core-test-0.2.8/README.md
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-17 11:56:43.177597 satsure-core-test-0.2.8/satelite/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-17 10:21:25.000000 satsure-core-test-0.2.8/satelite/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      976 2024-05-17 10:21:25.000000 satsure-core-test-0.2.8/satelite/config.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-17 11:56:43.178429 satsure-core-test-0.2.8/satelite/core/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       65 2024-05-17 10:57:24.000000 satsure-core-test-0.2.8/satelite/core/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     6366 2024-05-17 11:56:39.000000 satsure-core-test-0.2.8/satelite/core/downloader.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      826 2024-05-17 10:21:25.000000 satsure-core-test-0.2.8/satelite/core/uploader.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-17 11:56:43.179463 satsure-core-test-0.2.8/satelite/gdal/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-17 10:21:25.000000 satsure-core-test-0.2.8/satelite/gdal/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     5973 2024-05-17 10:57:24.000000 satsure-core-test-0.2.8/satelite/gdal/gdal_commands.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-17 11:56:43.180143 satsure-core-test-0.2.8/satelite/models/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-17 10:21:25.000000 satsure-core-test-0.2.8/satelite/models/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      372 2024-05-17 10:21:25.000000 satsure-core-test-0.2.8/satelite/models/s2_enum.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-17 11:56:43.180546 satsure-core-test-0.2.8/satelite/raster/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-17 10:21:25.000000 satsure-core-test-0.2.8/satelite/raster/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     8913 2024-05-17 10:21:25.000000 satsure-core-test-0.2.8/satelite/raster/raster.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-17 11:56:43.183287 satsure-core-test-0.2.8/satelite/sentinel2/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      499 2024-05-17 10:21:25.000000 satsure-core-test-0.2.8/satelite/sentinel2/__init__.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-17 11:56:43.183951 satsure-core-test-0.2.8/satelite/sentinel2/band_stack/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       50 2024-05-17 11:04:57.000000 satsure-core-test-0.2.8/satelite/sentinel2/band_stack/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2834 2024-05-17 10:21:25.000000 satsure-core-test-0.2.8/satelite/sentinel2/band_stack/generate_band_stack.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2429 2024-05-17 10:21:25.000000 satsure-core-test-0.2.8/satelite/sentinel2/fetch_unique_tile_date.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1634 2024-05-17 10:21:25.000000 satsure-core-test-0.2.8/satelite/sentinel2/fetch_unique_tile_date_pystac.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3204 2024-05-17 10:21:25.000000 satsure-core-test-0.2.8/satelite/sentinel2/get_tiles.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-17 11:56:43.184432 satsure-core-test-0.2.8/satelite/sentinel2/indices/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       43 2024-05-17 11:04:57.000000 satsure-core-test-0.2.8/satelite/sentinel2/indices/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3975 2024-05-17 10:21:25.000000 satsure-core-test-0.2.8/satelite/sentinel2/indices/general_indices.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      835 2024-05-17 10:21:25.000000 satsure-core-test-0.2.8/satelite/sentinel2/mosaic_custom_bands.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2553 2024-05-17 10:21:25.000000 satsure-core-test-0.2.8/satelite/sentinel2/mosaic_same_bands.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1502 2024-05-17 10:21:25.000000 satsure-core-test-0.2.8/satelite/sentinel2/path_row_from_shp.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3251 2024-05-17 10:21:25.000000 satsure-core-test-0.2.8/satelite/sentinel2/s2_l1c_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2912 2024-05-17 10:21:25.000000 satsure-core-test-0.2.8/satelite/sentinel2/s2_l2a_urls.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-17 11:56:43.184701 satsure-core-test-0.2.8/satelite/tests/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-17 10:21:25.000000 satsure-core-test-0.2.8/satelite/tests/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1004 2024-05-17 10:21:25.000000 satsure-core-test-0.2.8/satelite/tests/conftest.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-17 11:56:43.187329 satsure-core-test-0.2.8/satelite/tests/sentinel2/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-17 10:21:25.000000 satsure-core-test-0.2.8/satelite/tests/sentinel2/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      384 2024-05-17 10:21:25.000000 satsure-core-test-0.2.8/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      430 2024-05-17 10:21:25.000000 satsure-core-test-0.2.8/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1176 2024-05-17 10:21:25.000000 satsure-core-test-0.2.8/satelite/tests/sentinel2/test_genarate_band_stack.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1318 2024-05-17 10:21:25.000000 satsure-core-test-0.2.8/satelite/tests/sentinel2/test_general_indices.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1326 2024-05-17 10:21:25.000000 satsure-core-test-0.2.8/satelite/tests/sentinel2/test_get_tile.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      322 2024-05-17 10:21:25.000000 satsure-core-test-0.2.8/satelite/tests/sentinel2/test_mosaic_same_bands.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      871 2024-05-17 10:21:25.000000 satsure-core-test-0.2.8/satelite/tests/sentinel2/test_s2_l1c_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      898 2024-05-17 10:21:25.000000 satsure-core-test-0.2.8/satelite/tests/sentinel2/test_s2_l2a_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1543 2024-05-17 10:21:25.000000 satsure-core-test-0.2.8/satelite/tests/sentinel2/test_validate.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-17 11:56:43.187951 satsure-core-test-0.2.8/satelite/validators/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       47 2024-05-17 11:04:57.000000 satsure-core-test-0.2.8/satelite/validators/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2360 2024-05-17 11:02:14.000000 satsure-core-test-0.2.8/satelite/validators/check_shape_of_rid.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-17 11:56:43.188779 satsure-core-test-0.2.8/satsure_core_test.egg-info/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      515 2024-05-17 11:56:43.000000 satsure-core-test-0.2.8/satsure_core_test.egg-info/PKG-INFO
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1661 2024-05-17 11:56:43.000000 satsure-core-test-0.2.8/satsure_core_test.egg-info/SOURCES.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        1 2024-05-17 11:56:43.000000 satsure-core-test-0.2.8/satsure_core_test.egg-info/dependency_links.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      141 2024-05-17 11:56:43.000000 satsure-core-test-0.2.8/satsure_core_test.egg-info/requires.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        9 2024-05-17 11:56:43.000000 satsure-core-test-0.2.8/satsure_core_test.egg-info/top_level.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       38 2024-05-17 11:56:43.189264 satsure-core-test-0.2.8/setup.cfg
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      601 2024-05-17 11:56:39.000000 satsure-core-test-0.2.8/setup.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-20 14:04:19.045443 satsure-core-test-0.2.9/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-19 09:09:36.000000 satsure-core-test-0.2.9/LICENCE.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      536 2024-05-20 14:04:19.045261 satsure-core-test-0.2.9/PKG-INFO
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-19 09:09:36.000000 satsure-core-test-0.2.9/README.md
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-20 14:04:19.033589 satsure-core-test-0.2.9/satsure_core/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-19 09:33:06.000000 satsure-core-test-0.2.9/satsure_core/__init__.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-20 14:04:19.033806 satsure-core-test-0.2.9/satsure_core/satelite/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-19 09:27:06.000000 satsure-core-test-0.2.9/satsure_core/satelite/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      976 2024-05-19 09:27:06.000000 satsure-core-test-0.2.9/satsure_core/satelite/config.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-20 14:04:19.034735 satsure-core-test-0.2.9/satsure_core/satelite/core/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       65 2024-05-19 09:35:17.000000 satsure-core-test-0.2.9/satsure_core/satelite/core/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     6366 2024-05-19 09:39:40.000000 satsure-core-test-0.2.9/satsure_core/satelite/core/downloader.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      826 2024-05-19 09:27:06.000000 satsure-core-test-0.2.9/satsure_core/satelite/core/uploader.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-20 14:04:19.035273 satsure-core-test-0.2.9/satsure_core/satelite/gdal/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       69 2024-05-19 09:35:17.000000 satsure-core-test-0.2.9/satsure_core/satelite/gdal/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     5986 2024-05-19 10:00:10.000000 satsure-core-test-0.2.9/satsure_core/satelite/gdal/gdal_commands.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-20 14:04:19.035805 satsure-core-test-0.2.9/satsure_core/satelite/models/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       46 2024-05-19 10:10:14.000000 satsure-core-test-0.2.9/satsure_core/satelite/models/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      372 2024-05-19 09:27:06.000000 satsure-core-test-0.2.9/satsure_core/satelite/models/s2_enum.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-20 14:04:19.036185 satsure-core-test-0.2.9/satsure_core/satelite/raster/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      113 2024-05-19 10:10:14.000000 satsure-core-test-0.2.9/satsure_core/satelite/raster/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     8913 2024-05-19 09:27:06.000000 satsure-core-test-0.2.9/satsure_core/satelite/raster/raster.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-20 14:04:19.038491 satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      499 2024-05-19 09:57:43.000000 satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/__init__.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-20 14:04:19.039056 satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/band_stack/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       50 2024-05-19 10:10:14.000000 satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/band_stack/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2839 2024-05-19 10:10:14.000000 satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/band_stack/generate_band_stack.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2429 2024-05-19 09:27:06.000000 satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/fetch_unique_tile_date.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1634 2024-05-19 09:57:43.000000 satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/fetch_unique_tile_date_pystac.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3768 2024-05-20 07:41:47.000000 satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/get_tiles.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-20 14:04:19.039500 satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/indices/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       43 2024-05-19 10:10:14.000000 satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/indices/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3981 2024-05-19 10:10:14.000000 satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/indices/general_indices.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      835 2024-05-19 09:27:06.000000 satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/mosaic_custom_bands.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2559 2024-05-19 10:10:14.000000 satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/mosaic_same_bands.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1502 2024-05-19 09:27:06.000000 satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/path_row_from_shp.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3279 2024-05-19 10:12:42.000000 satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/s2_l1c_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2940 2024-05-19 10:12:42.000000 satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/s2_l2a_urls.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-20 14:04:19.039810 satsure-core-test-0.2.9/satsure_core/satelite/tests/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-19 09:27:06.000000 satsure-core-test-0.2.9/satsure_core/satelite/tests/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1004 2024-05-19 09:27:06.000000 satsure-core-test-0.2.9/satsure_core/satelite/tests/conftest.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-20 14:04:19.040647 satsure-core-test-0.2.9/satsure_core/satelite/tests/gdal/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-19 09:33:14.000000 satsure-core-test-0.2.9/satsure_core/satelite/tests/gdal/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      671 2024-05-19 10:10:14.000000 satsure-core-test-0.2.9/satsure_core/satelite/tests/gdal/test_create_jpeg_image.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      431 2024-05-19 10:10:14.000000 satsure-core-test-0.2.9/satsure_core/satelite/tests/gdal/test_get_projection.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      711 2024-05-19 10:10:14.000000 satsure-core-test-0.2.9/satsure_core/satelite/tests/gdal/test_reproject.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-20 14:04:19.041711 satsure-core-test-0.2.9/satsure_core/satelite/tests/raster/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-19 09:33:14.000000 satsure-core-test-0.2.9/satsure_core/satelite/tests/raster/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      993 2024-05-19 10:10:14.000000 satsure-core-test-0.2.9/satsure_core/satelite/tests/raster/test_mask_cloud.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      690 2024-05-19 10:10:14.000000 satsure-core-test-0.2.9/satsure_core/satelite/tests/raster/test_merge.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1097 2024-05-19 10:10:14.000000 satsure-core-test-0.2.9/satsure_core/satelite/tests/raster/test_normalised_difference_index.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      530 2024-05-19 10:10:14.000000 satsure-core-test-0.2.9/satsure_core/satelite/tests/raster/test_offset_file.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      645 2024-05-19 10:10:14.000000 satsure-core-test-0.2.9/satsure_core/satelite/tests/raster/test_resample_file.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-20 14:04:19.044016 satsure-core-test-0.2.9/satsure_core/satelite/tests/sentinel2/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-19 09:27:06.000000 satsure-core-test-0.2.9/satsure_core/satelite/tests/sentinel2/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      397 2024-05-19 09:33:15.000000 satsure-core-test-0.2.9/satsure_core/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      443 2024-05-19 09:33:15.000000 satsure-core-test-0.2.9/satsure_core/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1169 2024-05-19 10:12:42.000000 satsure-core-test-0.2.9/satsure_core/satelite/tests/sentinel2/test_genarate_band_stack.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1331 2024-05-19 09:33:15.000000 satsure-core-test-0.2.9/satsure_core/satelite/tests/sentinel2/test_general_indices.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1352 2024-05-19 09:33:15.000000 satsure-core-test-0.2.9/satsure_core/satelite/tests/sentinel2/test_get_tile.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      335 2024-05-19 09:33:15.000000 satsure-core-test-0.2.9/satsure_core/satelite/tests/sentinel2/test_mosaic_same_bands.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      884 2024-05-19 09:33:15.000000 satsure-core-test-0.2.9/satsure_core/satelite/tests/sentinel2/test_s2_l1c_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      911 2024-05-19 09:57:43.000000 satsure-core-test-0.2.9/satsure_core/satelite/tests/sentinel2/test_s2_l2a_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1545 2024-05-19 10:12:42.000000 satsure-core-test-0.2.9/satsure_core/satelite/tests/sentinel2/test_validate.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-20 14:04:19.044351 satsure-core-test-0.2.9/satsure_core/satelite/validators/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       47 2024-05-19 10:10:14.000000 satsure-core-test-0.2.9/satsure_core/satelite/validators/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2360 2024-05-19 09:39:40.000000 satsure-core-test-0.2.9/satsure_core/satelite/validators/check_shape_of_rid.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-20 14:04:19.045051 satsure-core-test-0.2.9/satsure_core_test.egg-info/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      536 2024-05-20 14:04:18.000000 satsure-core-test-0.2.9/satsure_core_test.egg-info/PKG-INFO
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2724 2024-05-20 14:04:18.000000 satsure-core-test-0.2.9/satsure_core_test.egg-info/SOURCES.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        1 2024-05-20 14:04:18.000000 satsure-core-test-0.2.9/satsure_core_test.egg-info/dependency_links.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      147 2024-05-20 14:04:18.000000 satsure-core-test-0.2.9/satsure_core_test.egg-info/requires.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       13 2024-05-20 14:04:18.000000 satsure-core-test-0.2.9/satsure_core_test.egg-info/top_level.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       38 2024-05-20 14:04:19.045563 satsure-core-test-0.2.9/setup.cfg
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      533 2024-05-20 14:03:47.000000 satsure-core-test-0.2.9/setup.py
```

### Comparing `satsure-core-test-0.2.8/PKG-INFO` & `satsure-core-test-0.2.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: satsure-core-test
-Version: 0.2.8
+Version: 0.2.9
 Summary: satsure core package
 Author: Satsure
 Author-email: kmstpm@email.com
 License-File: LICENCE.txt
 Requires-Dist: awscli
+Requires-Dist: boto3
 Requires-Dist: fiona
 Requires-Dist: gdal==3.6.2
 Requires-Dist: google-cloud-storage
 Requires-Dist: pandas
 Requires-Dist: pyproj
 Requires-Dist: pystac
 Requires-Dist: pystac-client
```

### Comparing `satsure-core-test-0.2.8/satelite/config.py` & `satsure-core-test-0.2.9/satsure_core/satelite/config.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.8/satelite/core/downloader.py` & `satsure-core-test-0.2.9/satsure_core/satelite/core/downloader.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.8/satelite/core/uploader.py` & `satsure-core-test-0.2.9/satsure_core/satelite/core/uploader.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.8/satelite/gdal/gdal_commands.py` & `satsure-core-test-0.2.9/satsure_core/satelite/gdal/gdal_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 import subprocess
 from pathlib import Path, PosixPath
 from tempfile import NamedTemporaryFile
 from typing import Optional, Union, Tuple,Dict
 
-from satelite.core import Downloader
+from satsure_core.satelite.core import Downloader
 
 
 def create_jpeg_image(
         input_file: PosixPath,
         output_file: Optional[str] = None,
         bands_position: Tuple[int, int, int] = (3, 2, 1),
         quality: int = 10,
```

### Comparing `satsure-core-test-0.2.8/satelite/raster/raster.py` & `satsure-core-test-0.2.9/satsure_core/satelite/raster/raster.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.8/satelite/sentinel2/band_stack/generate_band_stack.py` & `satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/band_stack/generate_band_stack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path, PosixPath
 from typing import Tuple
 
-from satelite.gdal.gdal_commands import create_jpeg_image
-from satelite.raster.raster import merge
+from satsure_core.satelite.gdal import create_jpeg_image
+from satsure_core.satelite.raster import merge
 
 
 class GenerateBandStack:
     """
     Stack bands based band input
     """
     BANDS = ("B02", "B03", "B04", "B08", "B12")
```

### Comparing `satsure-core-test-0.2.8/satelite/sentinel2/fetch_unique_tile_date.py` & `satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/fetch_unique_tile_date.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.8/satelite/sentinel2/fetch_unique_tile_date_pystac.py` & `satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/fetch_unique_tile_date_pystac.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.8/satelite/sentinel2/get_tiles.py` & `satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/get_tiles.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,48 +1,64 @@
 from os import environ
 
 import fiona
 from fiona.session import AWSSession
 from sqlalchemy import text
 
-from satelite.config import DBSession
+from satsure_core.satelite.config import DBSession
 
 
 class GetTiles:
     """To get tiles from different resources"""
 
     def __init__(self):
         self.db = DBSession.create()
 
-    def fetch_tile_from_db(self, sql_query, geom_):
+    def fetch_tile_from_db(self, sql_query, geom_list):
         """
             Fetch tile from database
         :param sql_query:
         :param geom_:
         :return:
         """
 
-        result = self.db.execute(sql_query,
-                                 {"geojson_geometry": str(geom_)})
+        result = self.db.execute(
+            sql_query,
+            {
+                "minx": geom_list['minx'][0],
+                "miny": geom_list['miny'][0],
+                "maxx": geom_list['maxx'][0],
+                "maxy": geom_list['maxy'][0],
+            },
+        )
         return result.fetchall()
 
     def get_tile_from_geom(self, geom_list: list) -> list:
         """generate tile from in geom
         :rtype: list
         """
         tile_list = set()
+        # print(geometry,geojson_geometry)
         sql_query = text(
             f"""SELECT tile FROM tileids WHERE ST_Intersects( geometry,
-                                            ST_GeomFromGeoJSON(:geojson_geometry)) """
+                                            ST_GeomFromText(:geojson_geometry)) """
+        )
+        sql_query = text(
+            """
+                            SELECT tile FROM tileids
+                            WHERE ST_Intersects(
+                                geometry,
+                                ST_MakeEnvelope(:minx, :miny, :maxx, :maxy, 4326) -- 4326 is the SRID, adjust if needed
+                            )
+                            """
         )
 
-        for geom_ in geom_list:
-            rows = self.fetch_tile_from_db(sql_query, geom_)
-            for row in rows:
-                tile_list.add(row[0])
+        rows = self.fetch_tile_from_db(sql_query, geom_list)
+        for row in rows:
+            tile_list.add(row[0])
 
         tile_list = list(tile_list)
         self.db.close()
 
         return tile_list
 
     def get_tile_from_rids(self, rids: list, shape_path: str):
```

### Comparing `satsure-core-test-0.2.8/satelite/sentinel2/indices/general_indices.py` & `satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/indices/general_indices.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path, PosixPath
 from typing import Tuple
 
-from satelite.raster.raster import create_normalised_difference_index, \
+from satsure_core.satelite.raster import create_normalised_difference_index, \
     mask_cloud
 
 
 class GeneralIndices:
     """
      Create indices based on bands
     """
```

### Comparing `satsure-core-test-0.2.8/satelite/sentinel2/mosaic_custom_bands.py` & `satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/mosaic_custom_bands.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.8/satelite/sentinel2/mosaic_same_bands.py` & `satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/mosaic_same_bands.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path, PosixPath
 from typing import List
 
-from satelite.raster.raster import merge
+from satsure_core.satelite.raster import merge
 
 
 class MosaicSameBands:
     """
     Stack similar bands on same date
     """
     BANDS = ("B02", "B03", "B04", "B05", "B08", "B12",)
```

### Comparing `satsure-core-test-0.2.8/satelite/sentinel2/path_row_from_shp.py` & `satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/path_row_from_shp.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.8/satelite/sentinel2/s2_l1c_urls.py` & `satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/s2_l1c_urls.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import re
 from pathlib import PosixPath
 from typing import List, Tuple
 
 from google.cloud import storage
 from google.oauth2 import service_account
 
-from satelite.config import GCP_BASE_URL, key_json, S3_L1C_BUCKET
-from satelite.core.downloader import Downloader
-from satelite.models.s2_enum import ProcessingLevel, BaseBands
+from satsure_core.satelite.config import GCP_BASE_URL, key_json, S3_L1C_BUCKET
+from satsure_core.satelite.core import Downloader
+from satsure_core.satelite.models.s2_enum import ProcessingLevel, BaseBands
 
 
 class S2L1CUrls:
     """
         This class used to fetch L1C urls from given tile code and from date
     """
```

### Comparing `satsure-core-test-0.2.8/satelite/sentinel2/s2_l2a_urls.py` & `satsure-core-test-0.2.9/satsure_core/satelite/sentinel2/s2_l2a_urls.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import datetime
 from pathlib import PosixPath
 from subprocess import PIPE, Popen
 from typing import List, Tuple
 
-from satelite.config import S3_L2A_BUCKET, S3_L2A_PREFIX
-from satelite.models.s2_enum import ProcessingLevel, BaseBands
-from satelite.core.downloader import Downloader
+from satsure_core.satelite.config import S3_L2A_BUCKET, S3_L2A_PREFIX
+from satsure_core.satelite.models.s2_enum import ProcessingLevel, BaseBands
+from satsure_core.satelite.core import Downloader
 
 
 class S2L2AUrls:
     """
         This class used to fetch L2A urls from given tile code and from date
     """
```

### Comparing `satsure-core-test-0.2.8/satelite/tests/conftest.py` & `satsure-core-test-0.2.9/satsure_core/satelite/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.8/satelite/tests/sentinel2/test_genarate_band_stack.py` & `satsure-core-test-0.2.9/satsure_core/satelite/tests/sentinel2/test_genarate_band_stack.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import glob
 import os
 from pathlib import Path
 
 import pytest
 
-from satelite.sentinel2.band_stack.generate_band_stack import GenerateBandStack
+from satsure_core.satelite.sentinel2.band_stack import GenerateBandStack
 
 
 @pytest.mark.skip("need to do upload tif files")
 class TestGenerateBandStack:
 
     def test_create_fcc(self):
         """
```

### Comparing `satsure-core-test-0.2.8/satelite/tests/sentinel2/test_general_indices.py` & `satsure-core-test-0.2.9/satsure_core/satelite/tests/sentinel2/test_general_indices.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import glob
 import os
 from pathlib import Path
 
 import pytest
 
-from satelite.sentinel2.indices.general_indices import GeneralIndices
+from satsure_core.satelite.sentinel2.indices.general_indices import GeneralIndices
 
 
 @pytest.mark.skip("need to add tiff files")
 class TestGeneralIndices:
     """Testcase for General Indices """
 
     def test_general_indices(self):
```

### Comparing `satsure-core-test-0.2.8/satelite/tests/sentinel2/test_get_tile.py` & `satsure-core-test-0.2.9/satsure_core/satelite/tests/sentinel2/test_get_tile.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from satelite.sentinel2 import GetTiles
-from satelite.config import DBSession
+from satsure_core.satelite.sentinel2 import GetTiles
+from satsure_core.satelite.config import DBSession
 
 
 class TestGetTiles:
 
     def test_get_tile_from_geom(self, monkeypatch):
         """testcase to get tile from geom"""
         geom = [{
```

### Comparing `satsure-core-test-0.2.8/satelite/tests/sentinel2/test_s2_l1c_urls.py` & `satsure-core-test-0.2.9/satsure_core/satelite/tests/sentinel2/test_s2_l1c_urls.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pathlib import Path
 
-from satelite.sentinel2 import S2L1CUrls
+from satsure_core.satelite.sentinel2 import S2L1CUrls
 
 
 class TestS2L1CUrls:
 
     def test_get_urls(self, monkeypatch):
         """
             Testcase to check get_urls data
```

### Comparing `satsure-core-test-0.2.8/satelite/tests/sentinel2/test_s2_l2a_urls.py` & `satsure-core-test-0.2.9/satsure_core/satelite/tests/sentinel2/test_s2_l2a_urls.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import datetime
 from pathlib import Path
 
-from satelite.sentinel2 import S2L2AUrls
+from satsure_core.satelite.sentinel2 import S2L2AUrls
 
 
 class TestS2L2AUrls:
 
     def test_get_urls(self, monkeypatch):
         """
             Testcase to check get_urls data
```

### Comparing `satsure-core-test-0.2.8/satelite/tests/sentinel2/test_validate.py` & `satsure-core-test-0.2.9/satsure_core/satelite/tests/sentinel2/test_validate.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 
 import pytest
 
-from satelite.core.downloader import Downloader
+from satsure_core.satelite.core import Downloader
 
 
 class TestDownloader:
 
     def test_validate_fields(self):
         """Testcase to validate input params
         """
```

### Comparing `satsure-core-test-0.2.8/satelite/validators/check_shape_of_rid.py` & `satsure-core-test-0.2.9/satsure_core/satelite/validators/check_shape_of_rid.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.8/satsure_core_test.egg-info/PKG-INFO` & `satsure-core-test-0.2.9/satsure_core_test.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: satsure-core-test
-Version: 0.2.8
+Version: 0.2.9
 Summary: satsure core package
 Author: Satsure
 Author-email: kmstpm@email.com
 License-File: LICENCE.txt
 Requires-Dist: awscli
+Requires-Dist: boto3
 Requires-Dist: fiona
 Requires-Dist: gdal==3.6.2
 Requires-Dist: google-cloud-storage
 Requires-Dist: pandas
 Requires-Dist: pyproj
 Requires-Dist: pystac
 Requires-Dist: pystac-client
```

### Comparing `satsure-core-test-0.2.8/setup.py` & `satsure-core-test-0.2.9/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='satsure-core-test',
-    version='0.2.8',
+    version='0.2.9',
     description='satsure core package',
     author='Satsure',
     author_email='kmstpm@email.com',
     packages=find_packages(),
-    install_requires=['awscli', 'fiona','gdal==3.6.2', 'google-cloud-storage', 'pandas',
+    install_requires=['awscli','boto3', 'fiona','gdal==3.6.2', 'google-cloud-storage', 'pandas',
                       'pyproj', 'pystac','pystac-client', 'python-dotenv', 'rasterstats',
                       'rasterio', 'requests', 'requests', 'sqlalchemy', 'wget'],
-    include_package_data=True,
-    package_data={
-        'satsure-core-test': ['satelite/*.json'],
-    }
+    include_package_data=True
 )
```

