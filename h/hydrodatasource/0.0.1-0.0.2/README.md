# Comparing `tmp/hydrodatasource-0.0.1.tar.gz` & `tmp/hydrodatasource-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydrodatasource-0.0.1.tar", last modified: Thu Mar 28 01:07:11 2024, max compression
+gzip compressed data, was "hydrodatasource-0.0.2.tar", last modified: Mon May 20 12:41:59 2024, max compression
```

## Comparing `hydrodatasource-0.0.1.tar` & `hydrodatasource-0.0.2.tar`

### file list

```diff
@@ -1,76 +1,95 @@
-drwxrwxrwx   0        0        0        0 2024-03-28 01:07:11.345707 hydrodatasource-0.0.1/
--rw-rw-rw-   0        0        0      173 2024-02-20 08:43:26.000000 hydrodatasource-0.0.1/AUTHORS.rst
--rw-rw-rw-   0        0        0     1533 2023-10-24 13:30:40.000000 hydrodatasource-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      314 2024-02-20 08:43:26.000000 hydrodatasource-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1125 2024-03-28 01:07:11.344679 hydrodatasource-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     8190 2024-03-28 01:01:26.000000 hydrodatasource-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-28 01:07:10.880130 hydrodatasource-0.0.1/hydrodatasource/
--rw-rw-rw-   0        0        0       88 2024-02-20 08:43:26.000000 hydrodatasource-0.0.1/hydrodatasource/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-28 01:07:10.986307 hydrodatasource-0.0.1/hydrodatasource/cleaner/
--rw-rw-rw-   0        0        0        0 2024-02-20 08:43:26.000000 hydrodatasource-0.0.1/hydrodatasource/cleaner/__init__.py
--rw-rw-rw-   0        0        0    29087 2024-03-23 09:17:12.000000 hydrodatasource-0.0.1/hydrodatasource/cleaner/dmca_esr.py
--rw-rw-rw-   0        0        0     7850 2024-02-20 08:43:26.000000 hydrodatasource-0.0.1/hydrodatasource/cleaner/fixdata.py
--rw-rw-rw-   0        0        0     6309 2024-02-26 00:20:12.000000 hydrodatasource-0.0.1/hydrodatasource/cleaner/get_moving_inq.py
--rw-rw-rw-   0        0        0    18151 2024-03-16 07:55:22.000000 hydrodatasource-0.0.1/hydrodatasource/cleaner/smooth_inq.py
-drwxrwxrwx   0        0        0        0 2024-03-28 01:07:11.003307 hydrodatasource-0.0.1/hydrodatasource/configs/
--rw-rw-rw-   0        0        0        0 2024-02-20 08:43:26.000000 hydrodatasource-0.0.1/hydrodatasource/configs/__init__.py
--rw-rw-rw-   0        0        0     3593 2024-02-26 00:20:12.000000 hydrodatasource-0.0.1/hydrodatasource/configs/config.py
-drwxrwxrwx   0        0        0        0 2024-03-28 01:07:11.108908 hydrodatasource-0.0.1/hydrodatasource/downloader/
--rw-rw-rw-   0        0        0      365 2024-02-20 08:43:26.000000 hydrodatasource-0.0.1/hydrodatasource/downloader/__init__.py
--rw-rw-rw-   0        0        0     3630 2024-02-20 08:43:26.000000 hydrodatasource-0.0.1/hydrodatasource/downloader/dem.py
--rw-rw-rw-   0        0        0     6488 2024-02-20 08:43:26.000000 hydrodatasource-0.0.1/hydrodatasource/downloader/downloader.py
--rw-rw-rw-   0        0        0     5385 2024-02-20 08:43:26.000000 hydrodatasource-0.0.1/hydrodatasource/downloader/gfs_config_dict.py
--rw-rw-rw-   0        0        0    14454 2024-02-20 08:43:26.000000 hydrodatasource-0.0.1/hydrodatasource/downloader/gfs_downloader_auto.py
--rw-rw-rw-   0        0        0     9792 2024-02-20 08:43:26.000000 hydrodatasource-0.0.1/hydrodatasource/downloader/gpm_downloader_auto.py
--rw-rw-rw-   0        0        0    16018 2024-03-28 00:38:31.000000 hydrodatasource-0.0.1/hydrodatasource/downloader/hydrostation.py
--rw-rw-rw-   0        0        0    12663 2024-03-16 07:55:22.000000 hydrodatasource-0.0.1/hydrodatasource/downloader/minio.py
--rw-rw-rw-   0        0        0     6313 2024-02-20 08:43:26.000000 hydrodatasource-0.0.1/hydrodatasource/downloader/ncep_gfs.py
--rw-rw-rw-   0        0        0     7849 2024-02-20 08:43:26.000000 hydrodatasource-0.0.1/hydrodatasource/downloader/s3.py
-drwxrwxrwx   0        0        0        0 2024-03-28 01:07:11.160490 hydrodatasource-0.0.1/hydrodatasource/processor/
--rw-rw-rw-   0        0        0        0 2024-02-20 08:43:26.000000 hydrodatasource-0.0.1/hydrodatasource/processor/__init__.py
--rw-rw-rw-   0        0        0    11191 2024-03-28 00:38:14.000000 hydrodatasource-0.0.1/hydrodatasource/processor/data_checker.py
--rw-rw-rw-   0        0        0     2257 2024-03-28 00:38:04.000000 hydrodatasource-0.0.1/hydrodatasource/processor/era5.py
--rw-rw-rw-   0        0        0    12073 2024-03-28 00:37:32.000000 hydrodatasource-0.0.1/hydrodatasource/processor/gpm_gfs.py
--rw-rw-rw-   0        0        0    21938 2024-02-20 11:53:09.000000 hydrodatasource-0.0.1/hydrodatasource/processor/grdc.py
--rw-rw-rw-   0        0        0     9424 2024-03-28 00:37:22.000000 hydrodatasource-0.0.1/hydrodatasource/processor/mask.py
--rw-rw-rw-   0        0        0     5505 2024-03-28 00:37:05.000000 hydrodatasource-0.0.1/hydrodatasource/processor/minio_process.py
-drwxrwxrwx   0        0        0        0 2024-03-28 01:07:11.233021 hydrodatasource-0.0.1/hydrodatasource/reader/
--rw-rw-rw-   0        0        0        2 2024-02-20 08:43:26.000000 hydrodatasource-0.0.1/hydrodatasource/reader/__init__.py
--rw-rw-rw-   0        0        0     6973 2024-03-28 00:36:39.000000 hydrodatasource-0.0.1/hydrodatasource/reader/access_fs.py
--rw-rw-rw-   0        0        0    23690 2024-03-28 00:35:06.000000 hydrodatasource-0.0.1/hydrodatasource/reader/data_source.py
--rw-rw-rw-   0        0        0    13825 2024-02-20 08:43:26.000000 hydrodatasource-0.0.1/hydrodatasource/reader/era5.py
--rw-rw-rw-   0        0        0     6611 2024-02-20 08:43:26.000000 hydrodatasource-0.0.1/hydrodatasource/reader/gfs.py
--rw-rw-rw-   0        0        0    29135 2024-02-20 08:43:26.000000 hydrodatasource-0.0.1/hydrodatasource/reader/gpm.py
--rw-rw-rw-   0        0        0     4942 2024-03-28 00:34:58.000000 hydrodatasource-0.0.1/hydrodatasource/reader/grdc.py
--rw-rw-rw-   0        0        0    37878 2024-03-28 00:34:49.000000 hydrodatasource-0.0.1/hydrodatasource/reader/minio.py
--rw-rw-rw-   0        0        0     5983 2024-02-20 08:43:26.000000 hydrodatasource-0.0.1/hydrodatasource/reader/minio_api.py
--rw-rw-rw-   0        0        0     6642 2024-03-28 00:33:44.000000 hydrodatasource-0.0.1/hydrodatasource/reader/reader.py
--rw-rw-rw-   0        0        0     1838 2024-03-28 00:33:13.000000 hydrodatasource-0.0.1/hydrodatasource/reader/stations.py
-drwxrwxrwx   0        0        0        0 2024-03-28 01:07:11.243010 hydrodatasource-0.0.1/hydrodatasource/utils/
--rw-rw-rw-   0        0        0        0 2024-03-16 07:55:22.000000 hydrodatasource-0.0.1/hydrodatasource/utils/__init__.py
--rw-rw-rw-   0        0        0     7713 2024-03-23 08:34:34.000000 hydrodatasource-0.0.1/hydrodatasource/utils/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-28 01:07:10.928311 hydrodatasource-0.0.1/hydrodatasource.egg-info/
--rw-rw-rw-   0        0        0     1125 2024-03-28 01:07:10.000000 hydrodatasource-0.0.1/hydrodatasource.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2043 2024-03-28 01:07:10.000000 hydrodatasource-0.0.1/hydrodatasource.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      305 2024-03-28 01:07:10.000000 hydrodatasource-0.0.1/hydrodatasource.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-03-28 01:07:10.000000 hydrodatasource-0.0.1/hydrodatasource.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      134 2024-03-28 01:07:10.000000 hydrodatasource-0.0.1/hydrodatasource.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-03-28 01:07:10.000000 hydrodatasource-0.0.1/hydrodatasource.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      328 2024-03-23 03:40:06.000000 hydrodatasource-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0      480 2024-03-28 01:07:11.352621 hydrodatasource-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1874 2024-03-28 00:25:15.000000 hydrodatasource-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-28 01:07:11.336675 hydrodatasource-0.0.1/tests/
--rw-rw-rw-   0        0        0     1556 2024-03-28 00:23:10.000000 hydrodatasource-0.0.1/tests/test_aoi_reading.py
--rw-rw-rw-   0        0        0     3709 2024-03-28 00:42:38.000000 hydrodatasource-0.0.1/tests/test_data_checker.py
--rw-rw-rw-   0        0        0     2650 2024-03-28 00:42:31.000000 hydrodatasource-0.0.1/tests/test_downloader.py
--rw-rw-rw-   0        0        0     3962 2024-03-28 00:42:14.000000 hydrodatasource-0.0.1/tests/test_gpm_gfs.py
--rw-rw-rw-   0        0        0      983 2024-03-28 00:41:49.000000 hydrodatasource-0.0.1/tests/test_process_inq.py
--rw-rw-rw-   0        0        0     1632 2024-03-28 00:41:57.000000 hydrodatasource-0.0.1/tests/test_processor.py
--rw-rw-rw-   0        0        0     2488 2024-03-28 00:41:10.000000 hydrodatasource-0.0.1/tests/test_read_blob.py
--rw-rw-rw-   0        0        0     3734 2024-03-28 00:40:41.000000 hydrodatasource-0.0.1/tests/test_reader.py
--rw-rw-rw-   0        0        0     1408 2024-03-28 00:40:26.000000 hydrodatasource-0.0.1/tests/test_reader_basins.py
--rw-rw-rw-   0        0        0     1161 2024-03-28 00:39:17.000000 hydrodatasource-0.0.1/tests/test_reader_stations.py
--rw-rw-rw-   0        0        0     1732 2024-03-28 00:40:18.000000 hydrodatasource-0.0.1/tests/test_rr_event_iden.py
--rw-rw-rw-   0        0        0     4571 2024-03-28 00:39:56.000000 hydrodatasource-0.0.1/tests/test_spec_path.py
--rw-rw-rw-   0        0        0      866 2024-03-28 00:39:40.000000 hydrodatasource-0.0.1/tests/test_sync.py
--rw-rw-rw-   0        0        0     2998 2024-03-28 00:39:32.000000 hydrodatasource-0.0.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:41:58.993286 hydrodatasource-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-20 12:41:58.993286 hydrodatasource-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8092 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:41:58.981286 hydrodatasource-0.0.2/hydrodatasource/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:41:58.985286 hydrodatasource-0.0.2/hydrodatasource/cleaner/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/cleaner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/cleaner/cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28332 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/cleaner/dmca_esr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8116 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/cleaner/fixdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/cleaner/get_moving_inq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/cleaner/rain_anomaly.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11557 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/cleaner/rainfall_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18263 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/cleaner/smooth_inq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10653 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/cleaner/streamflow_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/cleaner/waterlevel_cleaner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:41:58.985286 hydrodatasource-0.0.2/hydrodatasource/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/configs/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:41:58.985286 hydrodatasource-0.0.2/hydrodatasource/downloader/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/downloader/dem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/downloader/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/downloader/gfs_config_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14129 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/downloader/gfs_downloader_auto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9546 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/downloader/gpm_downloader_auto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15536 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/downloader/hydrostation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12277 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/downloader/minio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6154 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/downloader/ncep_gfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7605 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/downloader/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:41:58.989286 hydrodatasource-0.0.2/hydrodatasource/processor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/processor/basin_mean_rainfall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10861 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/processor/data_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/processor/era5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11746 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/processor/gpm_gfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21325 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/processor/grdc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11252 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/processor/mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/processor/minio_process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:41:58.989286 hydrodatasource-0.0.2/hydrodatasource/reader/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6560 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/reader/access_fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23515 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/reader/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13370 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/reader/era5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/reader/gfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28329 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/reader/gpm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/reader/grdc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36778 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/reader/minio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5843 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/reader/minio_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/reader/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/reader/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18828 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/reader/spliter_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/reader/stations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:41:58.989286 hydrodatasource-0.0.2/hydrodatasource/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9819 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/hydrodatasource/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:41:58.993286 hydrodatasource-0.0.2/hydrodatasource.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-20 12:41:58.000000 hydrodatasource-0.0.2/hydrodatasource.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-20 12:41:58.000000 hydrodatasource-0.0.2/hydrodatasource.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-20 12:41:58.000000 hydrodatasource-0.0.2/hydrodatasource.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 12:41:58.000000 hydrodatasource-0.0.2/hydrodatasource.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-20 12:41:58.000000 hydrodatasource-0.0.2/hydrodatasource.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-20 12:41:58.000000 hydrodatasource-0.0.2/hydrodatasource.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-20 12:41:58.993286 hydrodatasource-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:41:58.993286 hydrodatasource-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/tests/test_aoi_reading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/tests/test_data_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/tests/test_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/tests/test_gpm_gfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/tests/test_grid_mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/tests/test_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/tests/test_process_inq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/tests/test_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/tests/test_rainfall_average.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/tests/test_rainfall_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/tests/test_read_blob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/tests/test_read_gfs_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/tests/test_read_gpm_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/tests/test_read_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/tests/test_reader_basins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/tests/test_reader_stations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/tests/test_rr_event_iden.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7988 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/tests/test_spec_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/tests/test_split_grid_data_from_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/tests/test_streamflow_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/tests/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/tests/test_unify_usa_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6792 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-20 12:41:44.000000 hydrodatasource-0.0.2/tests/test_waterlevel_cleaner.py
```

### Comparing `hydrodatasource-0.0.1/LICENSE` & `hydrodatasource-0.0.2/LICENSE`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-BSD 3-Clause License
-
-Copyright (c) 2023, Open Water Science
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-3. Neither the name of the copyright holder nor the names of its
-   contributors may be used to endorse or promote products derived from
-   this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+BSD 3-Clause License
+
+Copyright (c) 2023, Open Water Science
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `hydrodatasource-0.0.1/PKG-INFO` & `hydrodatasource-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,36 @@
-Metadata-Version: 2.1
-Name: hydrodatasource
-Version: 0.0.1
-Summary: A python project to deal with hydrological datasources
-Home-page: https://github.com/iHeadWater/hydrodatasource
-Author: Wenyu Ouyang
-Author-email: hust2014owen@gmail.com
-License: BSD license
-Keywords: hydrodatasource
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS.rst
-Requires-Dist: geopandas
-Requires-Dist: openpyxl~=3.1
-Requires-Dist: xlrd
-Requires-Dist: requests
-Requires-Dist: kerchunk
-Requires-Dist: cfgrib
-Requires-Dist: eccodes
-Requires-Dist: h5py
-Requires-Dist: wget
-Requires-Dist: chardet
-Requires-Dist: intake
-Requires-Dist: dataretrieval
-Requires-Dist: pygeohydro
-Requires-Dist: pykalman
-Requires-Dist: hydrodataset
+Metadata-Version: 2.1
+Name: hydrodatasource
+Version: 0.0.2
+Summary: A python project to deal with hydrological datasources
+Home-page: https://github.com/iHeadWater/hydrodatasource
+Author: Wenyu Ouyang
+Author-email: hust2014owen@gmail.com
+License: BSD license
+Keywords: hydrodatasource
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS.rst
+Requires-Dist: geopandas
+Requires-Dist: openpyxl~=3.1
+Requires-Dist: xlrd
+Requires-Dist: requests
+Requires-Dist: kerchunk
+Requires-Dist: cfgrib
+Requires-Dist: eccodes
+Requires-Dist: h5py
+Requires-Dist: wget
+Requires-Dist: chardet
+Requires-Dist: intake
+Requires-Dist: dataretrieval
+Requires-Dist: pygeohydro
+Requires-Dist: pykalman
+Requires-Dist: psycopg2-binary
+Requires-Dist: hydrodataset
```

### Comparing `hydrodatasource-0.0.1/README.md` & `hydrodatasource-0.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,117 +1,117 @@
-<!--
- * @Author: Wenyu Ouyang
- * @Date: 2023-10-24 21:30:40
- * @LastEditTime: 2024-03-28 09:01:10
- * @LastEditors: Wenyu Ouyang
- * @Description: Readme for hydrodata
- * @FilePath: \hydrodata\README.md
- * Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
--->
-# hydrodatasource
-
-
-[![image](https://img.shields.io/pypi/v/hydrodatasource.svg)](https://pypi.python.org/pypi/hydrodatasource)
-[![image](https://img.shields.io/conda/vn/conda-forge/hydrodatasource.svg)](https://anaconda.org/conda-forge/hydrodatasource)
-
-[![image](https://pyup.io/repos/github/iHeadWater/hydrodatasource/shield.svg)](https://pyup.io/repos/github/iHeadWater/hydrodatasource)
-
--   Free software: BSD license
--   Documentation: https://WenyuOuyang.github.io/hydrodata
-
-📜 [中文文档](README.zh.md)
-
-
-Although there are many hydrological datasets for various watersheds, a noticeable issue is that many data sources remain unorganized and are not part of public datasets. This includes data that hasn't been organized due to its recency, data not considered by existing datasets, and data that will not be made public. These data sources represent a significant portion of available data. For example, the commonly used CAMELS dataset only includes data up to December 2014, almost ten years ago; GRDC runoff data, while useful, is rarely included in specific datasets. Real-time and near-real-time gridded data such as GFS, GPM, SMAP, etc., are infrequently compiled into datasets, with more emphasis on higher quality data like ERA5Land being used for research. A large portion of hydrological data in China is not public, and thus cannot be used to construct datasets.
-
-To address this, we conceived the hydrodatasource repository, aiming to provide a unified way of organizing these data sources for better utilization in scientific research and production, especially within the context of watersheds. For information on currently available public datasets, please visit: [hydrodataset](https://github.com/OuyangWenyu/hydrodataset).
-
-Specifically, this repository aims to provide a unified pathway for acquiring, managing, and using watershed hydrological data, making the computation of hydrological models, particularly AI-based models, more convenient.
-
-## How many data sources are there
-
-Considering watersheds as the primary focus of data description, our data sources mainly include:
-
-| **Primary Category** | **Secondary Category** | **Update Frequency** | **Data Structure** | **Specific Data Source** |
-| --- | --- | --- | --- | --- |
-| Baseline | Geographic Maps | Historical Archive | Vector | Watershed boundaries, site locations, and other shapefiles |
-|  | Elevation Data | Historical Archive | Raster | [DEM](https://github.com/DahnJ/Awesome-DEM) |
-|  | Attribute Data | Historical Archive | Tabular | HydroATLAS dataset |
-| Meteorological | Reanalysis Data Sets | Historical Archive, Delayed Dynamic | Raster | ERA5Land |
-|  | Remote Sensing Precipitation | Historical Archive, Near Real-Time Dynamic | Raster | GPM |
-|  | Weather Model Forecasts | Historical Archive, Real-Time Rolling | Raster | GFS |
-|  | AI Weather Forecasts | Real-Time Rolling | Raster | AIFS |
-|  | Ground Weather Stations | Historical Archive | Tabular | NOAA weather stations |
-|  | Ground Rainfall Stations | Historical Archive, Real-Time/Delayed Dynamic | Tabular | Non-public rainfall stations |
-| Hydrology | Remote Sensing Soil Moisture | Historical Archive, Near Real-Time Dynamic | Raster | SMAP |
-|  | Soil Moisture Stations | Historical Archive, Real-Time Dynamic | Tabular | Non-public soil moisture stations |
-|  | Ground Hydrological Stations | Historical Archive | Tabular | USGS |
-|  | Ground Hydrological Stations | Historical Archive, Real-Time Dynamic | Tabular | Non-public water level and flow stations |
-|  | Runoff Data Sets | Historical Archive | Tabular | GRDC |
-
-Note: The update frequency primarily refers to the frequency of updates in this repository, not necessarily the actual data source's update frequency.
-
-## What are the main features
-
-Before using it, it is essential to understand the main features of this repository, as this will guide its use.
-
-Our goal is to make this tool accessible to users with varying hardware resources. To elaborate on hardware resources: due to the extensive variety and volume of data involved, we have set up a MinIO service. MinIO is an open-source object storage service, which can be conveniently deployed locally or in the cloud; in our case, it's deployed locally. Thus, data is stored on MinIO and accessed via its API. This approach allows effective data management and the development of a unified access interface, simplifying data retrieval. However, it does require specific hardware resources, like disk space and memory. Therefore, we also offer a fully local file interaction mode for a portion of the data, although this mode won't be covered by complete functional testing.
-
-Based on this approach, we handle different types of data differently:
-
-For non-public data, we mainly provide utility functions in the public code to assist users in processing their data, facilitating the use of our open-source models. Of course, developers internally provide data retrieval services for their own data.
-For public data, we offer code for data download, format conversion, and reading, supporting users in handling data on their local systems.
-Now, let's expand on these two parts.
-
-### For non-public data
-
-The non-public data primarily involves ground station data. We provide tools for data format conversion for these data types. We define a data format that users need to prepare, and the subsequent process involves using these tools directly. In general, we expect users to prepare their data in a specific tabular format, which we will then convert into netCDF format for model reading. As for the exact format to prepare, we provide a data_checker function to verify the data format. Users can use this function to understand the specifics. We will also add a document detailing the specific format, which is yet to be completed.
-
-### For public data
-
-The public data mainly consists of those already organized into datasets. We provide code for data download, format conversion, and reading to support users in operating data on their local systems. These datasets include, but are not limited to, CAMELS, GRDC, ERA5Land, etc.
-
-However, as previously mentioned, we do not provide complete test coverage for local files. Our primary testing is conducted on MinIO.
-
-## How to use
-
-### Installation
-
-We recommend installing the package via pip:
-
-```bash
-pip install hydrodatasource
-```
-
-### Usage
-
-Our agreed data file organization structure at the primary level looks like this:
-
-```dir
-├── datasets-origin
-├── datasets-interim
-├── basins-origin
-├── basins-interim
-├── reservoirs-origin
-├── reservoirs-interim
-├── grids-origin
-├── grids-interim
-├── stations-origin
-├── stations-interim
-```
-
-Here, datasets-origin contains the datasets, basins-origin contains watershed data, reservoirs-origin stores reservoir data, rivers-origin holds river data, grids-origin includes gridded data, and stations-origin has station data.
-
-Data in the origin folders is raw data, while the interim folders contain data that has undergone preliminary processing. Essentially, the data in origin is the result of initial processing in GitLab's One Thing One Vote project, and interim is where origin data is processed into a specific format based on a particular requirement.
-
-This categorization fully covers the types of data listed in the table.
-
-For non-public station data:
-
-First, users need to prepare their data in a tabular format. To understand the specific format required, execute the following command:
-
-```python
-from hydrodatasource import station
-station.get_station_format()
-```
-
+<!--
+ * @Author: Wenyu Ouyang
+ * @Date: 2023-10-24 21:30:40
+ * @LastEditTime: 2024-05-20 20:35:58
+ * @LastEditors: Wenyu Ouyang
+ * @Description: Readme for hydrodatasource
+ * @FilePath: \hydrodatasource\README.md
+ * Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
+-->
+# hydrodatasource
+
+
+[![image](https://img.shields.io/pypi/v/hydrodatasource.svg)](https://pypi.python.org/pypi/hydrodatasource)
+[![image](https://img.shields.io/conda/vn/conda-forge/hydrodatasource.svg)](https://anaconda.org/conda-forge/hydrodatasource)
+
+[![image](https://pyup.io/repos/github/iHeadWater/hydrodatasource/shield.svg)](https://pyup.io/repos/github/iHeadWater/hydrodatasource)
+
+-   Free software: BSD license
+-   Documentation: https://WenyuOuyang.github.io/hydrodatasource
+
+📜 [中文文档](README.zh.md)
+
+
+Although there are many hydrological datasets for various watersheds, a noticeable issue is that many data sources remain unorganized and are not part of public datasets. This includes data that hasn't been organized due to its recency, data not considered by existing datasets, and data that will not be made public. These data sources represent a significant portion of available data. For example, the commonly used CAMELS dataset only includes data up to December 2014, almost ten years ago; GRDC runoff data, while useful, is rarely included in specific datasets. Real-time and near-real-time gridded data such as GFS, GPM, SMAP, etc., are infrequently compiled into datasets, with more emphasis on higher quality data like ERA5Land being used for research. A large portion of hydrological data in China is not public, and thus cannot be used to construct datasets.
+
+To address this, we conceived the hydrodatasource repository, aiming to provide a unified way of organizing these data sources for better utilization in scientific research and production, especially within the context of watersheds. For information on currently available public datasets, please visit: [hydrodataset](https://github.com/OuyangWenyu/hydrodataset).
+
+Specifically, this repository aims to provide a unified pathway for acquiring, managing, and using watershed hydrological data, making the computation of hydrological models, particularly AI-based models, more convenient.
+
+## How many data sources are there
+
+Considering watersheds as the primary focus of data description, our data sources mainly include:
+
+| **Primary Category** | **Secondary Category** | **Update Frequency** | **Data Structure** | **Specific Data Source** |
+| --- | --- | --- | --- | --- |
+| Baseline | Geographic Maps | Historical Archive | Vector | Watershed boundaries, site locations, and other shapefiles |
+|  | Elevation Data | Historical Archive | Raster | [DEM](https://github.com/DahnJ/Awesome-DEM) |
+|  | Attribute Data | Historical Archive | Tabular | HydroATLAS dataset |
+| Meteorological | Reanalysis Data Sets | Historical Archive, Delayed Dynamic | Raster | ERA5Land |
+|  | Remote Sensing Precipitation | Historical Archive, Near Real-Time Dynamic | Raster | GPM |
+|  | Weather Model Forecasts | Historical Archive, Real-Time Rolling | Raster | GFS |
+|  | AI Weather Forecasts | Real-Time Rolling | Raster | AIFS |
+|  | Ground Weather Stations | Historical Archive | Tabular | NOAA weather stations |
+|  | Ground Rainfall Stations | Historical Archive, Real-Time/Delayed Dynamic | Tabular | Non-public rainfall stations |
+| Hydrology | Remote Sensing Soil Moisture | Historical Archive, Near Real-Time Dynamic | Raster | SMAP |
+|  | Soil Moisture Stations | Historical Archive, Real-Time Dynamic | Tabular | Non-public soil moisture stations |
+|  | Ground Hydrological Stations | Historical Archive | Tabular | USGS |
+|  | Ground Hydrological Stations | Historical Archive, Real-Time Dynamic | Tabular | Non-public water level and flow stations |
+|  | Runoff Data Sets | Historical Archive | Tabular | GRDC |
+
+Note: The update frequency primarily refers to the frequency of updates in this repository, not necessarily the actual data source's update frequency.
+
+## What are the main features
+
+Before using it, it is essential to understand the main features of this repository, as this will guide its use.
+
+Our goal is to make this tool accessible to users with varying hardware resources. To elaborate on hardware resources: due to the extensive variety and volume of data involved, we have set up a MinIO service. MinIO is an open-source object storage service, which can be conveniently deployed locally or in the cloud; in our case, it's deployed locally. Thus, data is stored on MinIO and accessed via its API. This approach allows effective data management and the development of a unified access interface, simplifying data retrieval. However, it does require specific hardware resources, like disk space and memory. Therefore, we also offer a fully local file interaction mode for a portion of the data, although this mode won't be covered by complete functional testing.
+
+Based on this approach, we handle different types of data differently:
+
+For non-public data, we mainly provide utility functions in the public code to assist users in processing their data, facilitating the use of our open-source models. Of course, developers internally provide data retrieval services for their own data.
+For public data, we offer code for data download, format conversion, and reading, supporting users in handling data on their local systems.
+Now, let's expand on these two parts.
+
+### For non-public data
+
+The non-public data primarily involves ground station data. We provide tools for data format conversion for these data types. We define a data format that users need to prepare, and the subsequent process involves using these tools directly. In general, we expect users to prepare their data in a specific tabular format, which we will then convert into netCDF format for model reading. As for the exact format to prepare, we provide a data_checker function to verify the data format. Users can use this function to understand the specifics. We will also add a document detailing the specific format, which is yet to be completed.
+
+### For public data
+
+The public data mainly consists of those already organized into datasets. We provide code for data download, format conversion, and reading to support users in operating data on their local systems. These datasets include, but are not limited to, CAMELS, GRDC, ERA5Land, etc.
+
+However, as previously mentioned, we do not provide complete test coverage for local files. Our primary testing is conducted on MinIO.
+
+## How to use
+
+### Installation
+
+We recommend installing the package via pip:
+
+```bash
+pip install hydrodatasource
+```
+
+### Usage
+
+Our agreed data file organization structure at the primary level looks like this:
+
+```dir
+├── datasets-origin
+├── datasets-interim
+├── basins-origin
+├── basins-interim
+├── reservoirs-origin
+├── reservoirs-interim
+├── grids-origin
+├── grids-interim
+├── stations-origin
+├── stations-interim
+```
+
+Here, datasets-origin contains the datasets, basins-origin contains watershed data, reservoirs-origin stores reservoir data, rivers-origin holds river data, grids-origin includes gridded data, and stations-origin has station data.
+
+Data in the origin folders is raw data, while the interim folders contain data that has undergone preliminary processing. Essentially, the data in origin is the result of initial processing in GitLab's One Thing One Vote project, and interim is where origin data is processed into a specific format based on a particular requirement.
+
+This categorization fully covers the types of data listed in the table.
+
+For non-public station data:
+
+First, users need to prepare their data in a tabular format. To understand the specific format required, execute the following command:
+
+```python
+from hydrodatasource import station
+station.get_station_format()
+```
+
 Place the files in the stations-origin folder. For the specific parent absolute path, please configure it in the hydro_settings.yml file in your computer's user folder.
```

### Comparing `hydrodatasource-0.0.1/hydrodatasource/cleaner/dmca_esr.py` & `hydrodatasource-0.0.2/hydrodatasource/cleaner/dmca_esr.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,755 +1,755 @@
-"""
-Author: Jingyi Wang, Yang Wang, and Wenyu Ouyang
-Date: 2023-10-28 09:23:22
-LastEditTime: 2024-03-23 17:16:39
-LastEditors: Wenyu Ouyang
-Description: DMCA-ESR method (https://doi.org/10.1029/2021WR031283)
-FilePath: \hydrodata\hydrodata\cleaner\dmca_esr.py
-Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
-"""
-
-import numpy as np
-import pandas as pd
-
-
-def movmean(X, n):
-    ones = np.ones(X.shape)
-    kernel = np.ones(n)
-    return np.convolve(X, kernel, mode="same") / np.convolve(ones, kernel, mode="same")
-
-
-def step1_step2_tr_and_fluctuations_timeseries(rain, flow, rain_min, max_window):
-    """
-    The first two steps are used for calculation of the catchment response time,
-    the rainfall and streamflow fluctuations, and rainfall fluctuation.
-
-    Parameters
-    ----------
-    rain : np.ndarray
-        unit is mm/h
-    flow : np.ndarray
-        unit is m³/h
-    rain_min : _type_
-        最小降雨量阈值
-    max_window : _type_
-        场次划分最大窗口, 决定场次长度
-
-    Returns
-    -------
-    _type_
-        _description_
-    """
-    rain = rain.T
-    flow = flow.T
-    rain_int = np.nancumsum(rain)
-    flow_int = np.nancumsum(flow)
-    T = rain.size
-    rain_mean = np.empty(((max_window - 1) // 2, T))
-    flow_mean = np.empty(((max_window - 1) // 2, T))
-    fluct_rain = np.empty(((max_window - 1) // 2, T))
-    fluct_flow = np.empty(((max_window - 1) // 2, T))
-    F_rain = np.empty((max_window - 1) // 2)
-    F_flow = np.empty((max_window - 1) // 2)
-    F_rain_flow = np.empty((max_window - 1) // 2)
-    rho = np.empty((max_window - 1) // 2)
-    for window in np.arange(3, max_window + 1, 2):
-        int_index = int((window - 1) / 2 - 1)
-        start_slice = int(window - 0.5 * (window - 1))
-        dst_slice = int(T - 0.5 * (window - 1))
-        # 新建一个循环体长度*数据长度的大数组
-        rain_mean[int_index] = movmean(rain_int, window)
-        flow_mean[int_index] = movmean(flow_int, window)
-        fluct_rain[int_index] = rain_int - rain_mean[int_index, :]
-        F_rain[int_index] = (1 / (T - window + 1)) * np.nansum(
-            (fluct_rain[int_index, start_slice:dst_slice]) ** 2
-        )
-        fluct_flow[int_index, np.newaxis] = flow_int - flow_mean[int_index, :]
-        F_flow[int_index] = (1 / (T - window + 1)) * np.nansum(
-            (fluct_flow[int_index, start_slice:dst_slice]) ** 2
-        )
-        F_rain_flow[int_index] = (1 / (T - window + 1)) * np.nansum(
-            (fluct_rain[int_index, start_slice:dst_slice])
-            * (fluct_flow[int_index, start_slice:dst_slice])
-        )
-        rho[int_index] = F_rain_flow[int_index] / (
-            np.sqrt(F_rain[int_index]) * np.sqrt(F_flow[int_index])
-        )
-    pos_min = np.argmin(rho)
-    Tr = pos_min + 1
-    tol_fluct_rain = (rain_min / (2 * Tr + 1)) * Tr
-    tol_fluct_flow = flow_int[-1] / 1e15
-    fluct_rain[pos_min, np.fabs(fluct_rain[pos_min, :]) < tol_fluct_rain] = 0
-    fluct_flow[pos_min, np.fabs(fluct_flow[pos_min, :]) < tol_fluct_flow] = 0
-    fluct_rain_Tr = fluct_rain[pos_min, :]
-    fluct_flow_Tr = fluct_flow[pos_min, :]
-    fluct_bivariate_Tr = fluct_rain_Tr * fluct_flow_Tr
-    fluct_bivariate_Tr[np.fabs(fluct_bivariate_Tr) < np.finfo(np.float64).eps] = (
-        0  # 便于比较
-    )
-    return Tr, fluct_rain_Tr, fluct_flow_Tr, fluct_bivariate_Tr
-
-
-def step3_core_identification(fluct_bivariate_Tr):
-    d = np.diff(
-        fluct_bivariate_Tr, prepend=[0], append=[0]
-    )  # 计算相邻数值差分，为0代表两端点处于0区间
-    d[np.fabs(d) < np.finfo(np.float64).eps] = 0  # 确保计算正确
-    d = np.logical_not(d)  # 求0-1数组，为真代表为0区间
-    d0 = np.logical_not(
-        np.convolve(d, [1, 1], "valid")
-    )  # 对相邻元素做OR，代表原数组数值是否处于某一0区间，再取反表示取有效值
-    valid = np.logical_or(fluct_bivariate_Tr, d0)  # 有效core
-    d_ = np.diff(valid, prepend=[0], append=[0])  # 求差分方便取上下边沿
-    beginning_core = np.argwhere(d_ == 1)  # 上边沿为begin
-    end_core = np.argwhere(d_ == -1) - 1  # 下边沿为end
-    return beginning_core, end_core
-
-
-def step4_end_rain_events(beginning_core, end_core, rain, fluct_rain_Tr, rain_min):
-    end_rain = end_core.copy()
-    rain = rain.T
-    for g in range(end_core.size):
-        if end_core[g] + 2 < fluct_rain_Tr.size and (
-            np.fabs(fluct_rain_Tr[end_core[g] + 1]) < np.finfo(np.float64).eps
-            and np.fabs(fluct_rain_Tr[end_core[g] + 2]) < np.finfo(np.float64).eps
-        ):
-            # case 1&2
-            if np.fabs(rain[end_core[g]]) < np.finfo(np.float64).eps:
-                # case 1
-                while (
-                    end_rain[g] > beginning_core[g]
-                    and np.fabs(rain[end_rain[g]]) < np.finfo(np.float64).eps
-                ):
-                    end_rain[g] = end_rain[g] - 1
-            else:
-                # case 2
-                bound = (
-                    beginning_core[g + 1] if g + 1 < beginning_core.size else rain.size
-                )
-                while end_rain[g] < bound and rain[end_rain[g]] > rain_min:
-                    end_rain[g] = end_rain[g] + 1
-                end_rain[g] = end_rain[g] - 1  # 回到最后一个
-        else:
-            # case 3
-            # 若在降水，先跳过
-            while end_rain[g] >= beginning_core[g] and rain[end_rain[g]] > rain_min:
-                end_rain[g] = end_rain[g] - 1
-            while end_rain[g] >= beginning_core[g] and rain[end_rain[g]] < rain_min:
-                end_rain[g] = end_rain[g] - 1
-    return end_rain
-
-
-def step5_beginning_rain_events(
-    beginning_core, end_rain, rain, fluct_rain_Tr, rain_min
-):
-    beginning_rain = beginning_core.copy()
-    rain = rain.T
-    for g in range(beginning_core.size):
-        if (
-            beginning_core[g] >= 2
-            and np.fabs(fluct_rain_Tr[beginning_core[g] - 1]) < np.finfo(np.float64).eps
-            and np.fabs(fluct_rain_Tr[beginning_core[g] - 2]) < np.finfo(np.float64).eps
-            and np.fabs(rain[beginning_core[g]]) < np.finfo(np.float64).eps
-        ):
-            # case 1
-            while (
-                beginning_rain[g] < end_rain[g]
-                and np.fabs(rain[beginning_rain[g]]) < np.finfo(np.float64).eps
-            ):
-                beginning_rain[g] = beginning_rain[g] + 1
-        else:
-            # case 2&3
-            bound = end_rain[g - 1] if g >= 1 else -1
-            while beginning_rain[g] > bound and rain[beginning_rain[g]] > rain_min:
-                beginning_rain[g] = beginning_rain[g] - 1
-            beginning_rain[g] = beginning_rain[g] + 1  # 回到第一个
-    return beginning_rain
-
-
-def step6_checks_on_rain_events(
-    beginning_rain, end_rain, rain, rain_min, beginning_core, end_core
-):
-    rain = rain.T
-    beginning_rain = beginning_rain.copy()
-    end_rain = end_rain.copy()
-    if beginning_rain[0] == 0:  # 掐头
-        beginning_rain = beginning_rain[1:]
-        end_rain = end_rain[1:]
-        beginning_core = beginning_core[1:]
-        end_core = end_core[1:]
-    if end_rain[-1] == rain.size - 1:  # 去尾
-        beginning_rain = beginning_rain[:-2]
-        end_rain = end_rain[:-2]
-        beginning_core = beginning_core[:-2]
-        end_core = end_core[:-2]
-    error_time_reversed = beginning_rain > end_rain
-    error_wrong_delimiter = np.logical_or(
-        rain[beginning_rain - 1] > rain_min, rain[end_rain + 1] > rain_min
-    )
-    beginning_rain[error_time_reversed] = -2
-    beginning_rain[error_wrong_delimiter] = -2
-    end_rain[error_time_reversed] = -2
-    end_rain[error_wrong_delimiter] = -2
-    beginning_core[error_time_reversed] = -2
-    beginning_core[error_wrong_delimiter] = -2
-    end_core[error_time_reversed] = -2
-    end_core[error_wrong_delimiter] = -2
-    beginning_rain = beginning_rain[beginning_rain != -2]
-    end_rain = end_rain[end_rain != -2]
-    beginning_core = beginning_core[beginning_core != -2]
-    end_core = end_core[end_core != -2]
-    return beginning_rain, end_rain, beginning_core, end_core
-
-
-def step7_end_flow_events(
-    end_rain_checked, beginning_core, end_core, rain, fluct_rain_Tr, fluct_flow_Tr, Tr
-):
-    end_flow = np.empty(end_core.size, dtype=int)
-    for g in range(end_rain_checked.size):
-        if end_core[g] + 2 < fluct_rain_Tr.size and (
-            np.fabs(fluct_rain_Tr[end_core[g] + 1]) < np.finfo(np.float64).eps
-            and np.fabs(fluct_rain_Tr[end_core[g] + 2]) < np.finfo(np.float64).eps
-        ):
-            # case 1
-            end_flow[g] = end_rain_checked[g]
-            bound = (
-                beginning_core[g + 1] + Tr if g + 1 < beginning_core.size else rain.size
-            )
-            bound = min(bound, rain.size)  # 防溢出
-            # 若flow为负，先跳过
-            while end_flow[g] < bound and fluct_flow_Tr[end_flow[g]] <= 0:
-                end_flow[g] = end_flow[g] + 1
-            while end_flow[g] < bound and fluct_flow_Tr[end_flow[g]] > 0:
-                end_flow[g] = end_flow[g] + 1
-            end_flow[g] = end_flow[g] - 1  # 回到最后一个
-        else:
-            # case 2
-            end_flow[g] = end_core[g]
-            while end_flow[g] >= beginning_core[g] and fluct_flow_Tr[end_flow[g]] <= 0:
-                end_flow[g] = end_flow[g] - 1
-    return end_flow
-
-
-def step8_beginning_flow_events(
-    beginning_rain_checked,
-    end_rain_checked,
-    rain,
-    beginning_core,
-    fluct_rain_Tr,
-    fluct_flow_Tr,
-):
-    beginning_flow = np.empty(beginning_rain_checked.size, dtype=int)
-    for g in range(beginning_rain_checked.size):
-        if beginning_core[g] >= 2 and (
-            np.fabs(fluct_rain_Tr[beginning_core[g] - 1]) < np.finfo(np.float64).eps
-            and np.fabs(fluct_rain_Tr[beginning_core[g] - 2]) < np.finfo(np.float64).eps
-        ):
-            beginning_flow[g] = beginning_rain_checked[g]  # case 1
-        else:
-            beginning_flow[g] = beginning_core[g]  # case 2
-        while (
-            beginning_flow[g] < end_rain_checked[g]
-            and fluct_flow_Tr[beginning_flow[g]] >= 0
-        ):
-            beginning_flow[g] = beginning_flow[g] + 1
-    return beginning_flow
-
-
-def step9_checks_on_flow_events(
-    beginning_rain_checked, end_rain_checked, beginning_flow, end_flow, fluct_flow_Tr
-):
-    beginning_flow_checked = np.empty_like(beginning_flow, dtype=object)
-    end_flow_checked = np.empty_like(end_flow, dtype=object)
-    for g in range(len(beginning_flow)):
-        if (
-            not np.isnan(beginning_flow[g])
-            and not np.isnan(end_flow[g])
-            and (
-                end_flow[g] <= beginning_flow[g]
-                or fluct_flow_Tr[beginning_flow[g]] > 0
-                or fluct_flow_Tr[end_flow[g]] < 0
-                or beginning_flow[g] < beginning_rain_checked[g]
-                or end_flow[g] < end_rain_checked[g]
-            )
-        ):
-            beginning_flow_checked[g] = np.nan
-            end_flow_checked[g] = np.nan
-        else:
-            beginning_flow_checked[g] = beginning_flow[g]
-            end_flow_checked[g] = end_flow[g]
-
-    index_events = [
-        i
-        for i in range(len(beginning_rain_checked))
-        if not np.isnan(beginning_rain_checked[i])
-        and not np.isnan(beginning_flow_checked[i])
-        and not np.isnan(end_rain_checked[i])
-        and not np.isnan(end_flow_checked[i])
-    ]
-
-    beginning_flow_ungrouped = beginning_flow_checked[index_events]
-    end_flow_ungrouped = end_flow_checked[index_events]
-    beginning_rain_ungrouped = beginning_rain_checked[index_events]
-    end_rain_ungrouped = end_rain_checked[index_events]
-    return (
-        beginning_rain_ungrouped,
-        end_rain_ungrouped,
-        beginning_flow_ungrouped,
-        end_flow_ungrouped,
-    )
-    # The following code is written by Wang, Yang
-    # error_time_reversed = beginning_flow > end_flow
-    # error_wrong_fluct = np.logical_or(
-    #     np.logical_or(fluct_flow_Tr[beginning_flow] > 0, fluct_flow_Tr[end_flow] < 0),
-    #     np.logical_or(
-    #         beginning_flow < beginning_rain_checked, end_flow < end_rain_checked
-    #     ),
-    # )
-    # beginning_flow[error_time_reversed] = -3
-    # beginning_flow[error_wrong_fluct] = -3
-    # end_flow[error_time_reversed] = -3
-    # end_flow[error_wrong_fluct] = -3
-    # beginning_flow = beginning_flow[beginning_flow != -3]
-    # end_flow = end_flow[end_flow != -3]
-
-    # beginning_rain_checked[error_time_reversed] = -3
-    # beginning_rain_checked[error_wrong_fluct] = -3
-    # end_rain_checked[error_time_reversed] = -3
-    # end_rain_checked[error_wrong_fluct] = -3
-    # beginning_rain = beginning_rain_checked[beginning_rain_checked != -3]
-    # end_rain = end_rain_checked[end_rain_checked != -3]
-    # return beginning_rain, end_rain, beginning_flow, end_flow
-
-
-def step10_checks_on_overlapping_events(
-    beginning_rain_ungrouped,
-    end_rain_ungrouped,
-    beginning_flow_ungrouped,
-    end_flow_ungrouped,
-    time,
-):
-    # rain
-    # order1 = np.reshape(
-    #     np.hstack(
-    #         (
-    #             np.reshape(beginning_rain_ungrouped, (-1, 1)),
-    #             np.reshape(end_rain_ungrouped, (-1, 1)),
-    #         )
-    #     ),
-    #     (1, -1),
-    # )
-    # reversed1 = np.diff(order1) <= 0
-    # order1[np.hstack((reversed1, [[False]]))] = -2
-    # order1[np.hstack(([[False]], reversed1))] = -2
-    # order1 = order1[order1 != -2]
-    # # flow
-    # order2 = np.reshape(
-    #     np.hstack(
-    #         (
-    #             np.reshape(beginning_flow_ungrouped, (-1, 1)),
-    #             np.reshape(end_flow_ungrouped, (-1, 1)),
-    #         )
-    #     ),
-    #     (1, -1),
-    # )
-    # reversed2 = np.diff(order2) <= 0
-    # order2[np.hstack((reversed2, [[False]]))] = -3
-    # order2[np.hstack(([[False]], reversed2))] = -3
-    # order2 = order2[order2 != -3]
-    # # group
-    # rain_grouped = np.reshape(order1, (-1, 2)).T
-    # beginning_rain_grouped = rain_grouped[0]
-    # end_rain_grouped = rain_grouped[1]
-    # flow_grouped = np.reshape(order2, (-1, 2)).T
-    # beginning_flow_grouped = flow_grouped[0]
-    # end_flow_grouped = flow_grouped[1]
-    # return (
-    #     time[beginning_rain_grouped],
-    #     time[end_rain_grouped],
-    #     time[beginning_flow_grouped],
-    #     time[end_flow_grouped],
-    # )
-
-    beginning_rain_ungrouped = beginning_rain_ungrouped.astype(float)
-    beginning_flow_ungrouped = beginning_flow_ungrouped.astype(float)
-    end_rain_ungrouped = end_rain_ungrouped.astype(float)
-    end_flow_ungrouped = end_flow_ungrouped.astype(float)
-    q = 1
-    marker_overlapping = []
-    for g in range(len(end_rain_ungrouped) - 1):
-        if (
-            end_rain_ungrouped[g] > beginning_rain_ungrouped[g + 1]
-            or end_flow_ungrouped[g] > beginning_flow_ungrouped[g + 1]
-        ):
-            marker_overlapping.append(g)
-            q += 1
-    if marker_overlapping:
-        q = 0
-        while q < len(marker_overlapping) - 1:
-            to_group = [marker_overlapping[q]]
-            while (
-                q < len(marker_overlapping)
-                and marker_overlapping[q] == marker_overlapping[q + 1] - 1
-            ):
-                to_group.append(marker_overlapping[q + 1])
-                q += 1
-
-            beginning_rain_ungrouped[to_group[0]] = beginning_rain_ungrouped[
-                to_group[0]
-            ]
-            beginning_flow_ungrouped[to_group[0]] = beginning_flow_ungrouped[
-                to_group[0]
-            ]
-            end_flow_ungrouped[to_group[0]] = end_flow_ungrouped[to_group[-1] + 1]
-            end_rain_ungrouped[to_group[0]] = end_rain_ungrouped[to_group[-1] + 1]
-
-            if len(to_group) > 1:
-                beginning_rain_ungrouped[to_group[1:]] = np.nan
-                beginning_flow_ungrouped[to_group[1:]] = np.nan
-                end_flow_ungrouped[to_group[1:]] = np.nan
-                end_rain_ungrouped[to_group[1:]] = np.nan
-
-            beginning_rain_ungrouped[to_group[-1] + 1] = np.nan
-            beginning_flow_ungrouped[to_group[-1] + 1] = np.nan
-            end_flow_ungrouped[to_group[-1] + 1] = np.nan
-            end_rain_ungrouped[to_group[-1] + 1] = np.nan
-
-            to_group = []
-            q += 1
-
-    index_events2 = np.where(
-        ~np.isnan(beginning_rain_ungrouped)
-        & ~np.isnan(beginning_flow_ungrouped)
-        & ~np.isnan(end_rain_ungrouped)
-        & ~np.isnan(end_flow_ungrouped)
-    )[0]
-    beginning_flow_grouped = beginning_flow_ungrouped[index_events2]
-    end_flow_grouped = end_flow_ungrouped[index_events2]
-    beginning_rain_grouped = beginning_rain_ungrouped[index_events2]
-    end_rain_grouped = end_rain_ungrouped[index_events2]
-    beginning_rain_grouped = beginning_rain_grouped.astype(int)
-    end_rain_grouped = end_rain_grouped.astype(int)
-    beginning_flow_grouped = beginning_flow_grouped.astype(int)
-    end_flow_grouped = end_flow_grouped.astype(int)
-    beginning_rain = time[beginning_rain_grouped]
-    end_rain = time[end_rain_grouped]
-    end_flow = time[end_flow_grouped]
-    beginning_flow = time[beginning_flow_grouped]
-    return beginning_rain, end_rain, beginning_flow, end_flow
-    # biliu_rain_division = pd.DataFrame({'BEGINNING_RAIN': BEGINNING_RAIN, 'END_RAIN': END_RAIN})
-    # biliu_rain_division.to_csv(os.path.join(definitions.ROOT_DIR, 'example/yingnariver_data/yingna_rain_flow_division/yingna_rain_division.txt'), sep='\t')
-    # biliu_flow_division = pd.DataFrame({'BEGINNING_FLOW': BEGINNING_FLOW, 'END_FLOW': END_FLOW})
-    # biliu_flow_division.to_csv(os.path.join(definitions.ROOT_DIR, 'example/yingnariver_data/yingna_rain_flow_division/yingna_flow_division.txt'), sep='\t')
-
-
-def baseflow_curve(beginning_flow, end_flow, flow, time):
-    baseflow = np.copy(flow)
-    beg_end_series = np.array([], dtype=beginning_flow[0].dtype)
-    for j in range(len(beginning_flow)):
-        beg_end_series = np.concatenate(
-            (beg_end_series, [beginning_flow[j], end_flow[j]])
-        )
-
-    for k in range(len(beg_end_series) - 1):
-        index_beg = np.where(time == beg_end_series[k])[0]
-        index_end = np.where(time == beg_end_series[k + 1])[0]
-        index_beg = int(index_beg)
-        index_end = int(index_end)
-        if (
-            len(np.where(np.isnan(flow[index_beg : index_end + 1]) == 1)[0])
-            >= len(flow[index_beg : index_end + 1]) * 0.9
-        ):
-            baseflow[index_beg : index_end + 1] = np.nan
-        elif index_end - index_beg == 1:
-            baseflow[index_beg] = flow[index_beg]
-            baseflow[index_end] = flow[index_end]
-        elif flow[index_beg] < flow[index_end]:
-            increment = (flow[index_end] - flow[index_beg]) / (index_end - index_beg)
-            for m in range(index_beg + 1, index_end):
-                baseflow[m] = baseflow[index_beg] + increment * (m - index_beg)
-        elif flow[index_beg] > flow[index_end]:
-            increment = (flow[index_beg] - flow[index_end]) / (index_end - index_beg)
-            for m in range(index_beg + 1, index_end):
-                baseflow[m] = baseflow[index_beg] - increment * (m - index_beg)
-
-    for m in range(len(baseflow)):
-        baseflow[m] = min(baseflow[m], flow[m])
-    return baseflow
-
-
-def step11_event_analysis(
-    beginning_rain,
-    end_rain,
-    beginning_flow,
-    end_flow,
-    rain,
-    flow,
-    time,
-    flow_threshold,
-    multiple=1,
-    flag=0,
-    duration_max=2400,
-):
-    """The step 11 is a new step for the DMCA-ESR method
-    we proposed to check again for the rainfall-runoff events.
-
-    Parameters
-    ----------
-    beginning_rain : _type_
-        _description_
-    end_rain : _type_
-        _description_
-    beginning_flow : _type_
-        _description_
-    end_flow : _type_
-        _description_
-    rain : _type_
-        _description_
-    flow : _type_
-        _description_
-    time : _type_
-        _description_
-    flag : int, by default 0
-        if flag != 1, calculation target is flow - baseflow,
-        if flag == 1, cal target is flow
-        the default value 0 is recommended as flag == 1 is just for comparison
-    multiple : int
-        1h means the multiple is 1, 1d means the multiple is 24
-    flow_threshold : float
-        flow threshold -- remove events with max flow lower than it
-        its unit is mm_h
-    duration_max : int
-        maximum duration of the rainfall-runoff events we set; unit is hour
-
-    Returns
-    -------
-    _type_
-        _description_
-    """
-    duration_rain = np.zeros(len(beginning_rain))
-    duration_runoff = np.zeros(len(beginning_flow))
-    volume_rain = np.zeros(len(beginning_rain))
-    volume_runoff = np.zeros(len(beginning_flow))
-    runoff_ratio = np.zeros(len(beginning_rain))
-    for h in range(len(beginning_rain)):
-        duration_rain[h] = (
-            (np.datetime64(end_rain[h]) - np.datetime64(beginning_rain[h]))
-            / np.timedelta64(1, "s")
-            / (60 * 60 * multiple)
-        )
-        duration_runoff[h] = (
-            (np.datetime64(end_flow[h]) - np.datetime64(beginning_flow[h]))
-            / np.timedelta64(1, "s")
-            / (60 * 60 * multiple)
-        )
-        index_beginning_event = np.where(time == beginning_rain[h])[0]
-        index_end_event = np.where(time == end_rain[h])[0]
-        index_beginning_event = int(index_beginning_event)
-        index_end_event = int(index_end_event)
-        volume_rain[h] = (
-            np.nansum(rain[index_beginning_event:index_end_event]) * multiple
-        )
-
-    if flag == 1:
-        for h in range(len(beginning_flow)):
-            index_beginning_event = np.where(time == beginning_flow[h])[0]
-            index_end_event = np.where(time == end_flow[h])[0]
-            volume_runoff[h] = (
-                np.nansum(flow[index_beginning_event:index_end_event]) * multiple
-            )
-    else:
-        baseflow = baseflow_curve(beginning_flow, end_flow, flow, time)
-        for h in range(len(beginning_flow)):
-            index_beginning_event = np.where(time == beginning_flow[h])[0]
-            index_end_event = np.where(time == end_flow[h])[0]
-            index_beginning_event = int(index_beginning_event)
-            index_end_event = int(index_end_event)
-
-            q = flow[index_beginning_event:index_end_event]
-            qb = baseflow[index_beginning_event:index_end_event]
-            volume_runoff[h] = np.nansum(q - qb) * multiple
-    runoff_ratio = volume_runoff / volume_rain
-    result_df = pd.DataFrame(
-        {
-            "BEGINNING_RAIN": beginning_rain,
-            "END_RAIN": end_rain,
-            "BEGINNING_FLOW": beginning_flow,
-            "END_FLOW": end_flow,
-            "DURATION_RAIN": duration_rain,
-            "DURATION_RUNOFF": duration_runoff,
-            "VOLUME_RAIN": volume_rain,
-            "VOLUME_RUNOFF": volume_runoff,
-            "RUNOFF_RATIO": runoff_ratio,
-        }
-    )
-    drop_list = []
-    for i in range(len(beginning_rain)):
-        index_beginning_event = np.where(time == beginning_flow[i])[0]
-        index_end_event = np.where(time == end_flow[i])[0]
-        index_beginning_event = int(index_beginning_event)
-        index_end_event = int(index_end_event)
-        if flow[index_beginning_event:index_end_event].max() < flow_threshold:
-            drop_list.append(i)
-        if result_df["DURATION_RAIN"].iloc[i] > duration_max:
-            drop_list.append(i)
-        if result_df["DURATION_RUNOFF"].iloc[i] > duration_max:
-            drop_list.append(i)
-        if result_df["VOLUME_RAIN"].iloc[i] == 0:
-            drop_list.append(i)
-        if result_df["VOLUME_RUNOFF"].iloc[i] == 0:
-            drop_list.append(i)
-        if runoff_ratio[i] > 1:
-            drop_list.append(i)
-    drop_array = np.unique(np.array(drop_list, dtype=int))
-    result_df = result_df.drop(index=drop_array)
-    duration_rain = result_df["DURATION_RAIN"]
-    volume_rain = result_df["VOLUME_RAIN"]
-    duration_runoff = result_df["DURATION_RUNOFF"]
-    volume_runoff = result_df["VOLUME_RUNOFF"]
-    runoff_ratio = result_df["RUNOFF_RATIO"]
-    beginning_rain = result_df["BEGINNING_RAIN"]
-    end_rain = result_df["END_RAIN"]
-    beginning_flow = result_df["BEGINNING_FLOW"]
-    end_flow = result_df["END_FLOW"]
-    return (
-        duration_rain,
-        volume_rain,
-        duration_runoff,
-        volume_runoff,
-        runoff_ratio,
-        beginning_rain,
-        end_rain,
-        beginning_flow,
-        end_flow,
-    )
-
-
-def rainfall_runoff_event_identify(
-    rain, flow, rain_min=0.02, max_window=100, multiple=24, flow_threshold=0.02
-):
-    """Full process for identification of rainfall-runoff events
-    We make function for each step, name the function as the step number and
-    add some anther necessary steps for the DMCA-ESR method.
-
-    Parameters
-    ----------
-    rain : pd.Series
-        rainfall time series, for the original data,
-        unit must be same as the time interval.
-        For example, when unit is mm/day, time interval is day
-    flow : pd.Series
-        streamflow time series,
-        the requirement for unit is same as the rainfall
-    rain_min : float
-        minimum rainfall threshold; its unit is mm/h
-    max_window : int
-        maximum window size in the first two steps
-        it has no unit, just meaning the number of time intervals,
-        no matter the time unit is hour, day, or others
-    multiple : int
-        24 for daily data, meaning convert unit from mm/day to mm/h
-        1 for hourly data
-    flow_threshold : float
-        events with max flow lower than it will be removed; its unit is mm/h
-    """
-    time = rain.index.to_numpy()
-    rain = rain.to_numpy() / multiple
-    flow = flow.to_numpy() / multiple
-    (
-        Tr,
-        fluct_rain_Tr,
-        fluct_flow_Tr,
-        fluct_bivariate_Tr,
-    ) = step1_step2_tr_and_fluctuations_timeseries(rain, flow, rain_min, max_window)
-    beginning_core, end_core = step3_core_identification(fluct_bivariate_Tr)
-    end_rain = step4_end_rain_events(
-        beginning_core, end_core, rain, fluct_rain_Tr, rain_min
-    )
-    beginning_rain = step5_beginning_rain_events(
-        beginning_core, end_rain, rain, fluct_rain_Tr, rain_min
-    )
-    (
-        beginning_rain_checked,
-        end_rain_checked,
-        beginning_core,
-        end_core,
-    ) = step6_checks_on_rain_events(
-        beginning_rain, end_rain, rain, rain_min, beginning_core, end_core
-    )
-    end_flow = step7_end_flow_events(
-        end_rain_checked,
-        beginning_core,
-        end_core,
-        rain,
-        fluct_rain_Tr,
-        fluct_flow_Tr,
-        Tr,
-    )
-    beginning_flow = step8_beginning_flow_events(
-        beginning_rain_checked,
-        end_rain_checked,
-        rain,
-        beginning_core,
-        fluct_rain_Tr,
-        fluct_flow_Tr,
-    )
-    (
-        beginning_rain_ungrouped,
-        end_rain_ungrouped,
-        beginning_flow_ungrouped,
-        end_flow_ungrouped,
-    ) = step9_checks_on_flow_events(
-        beginning_rain_checked,
-        end_rain_checked,
-        beginning_flow,
-        end_flow,
-        fluct_flow_Tr,
-    )
-    (
-        beginning_rain,
-        end_rain,
-        beginning_flow,
-        end_flow,
-    ) = step10_checks_on_overlapping_events(
-        beginning_rain_ungrouped,
-        end_rain_ungrouped,
-        beginning_flow_ungrouped,
-        end_flow_ungrouped,
-        time,
-    )
-    (
-        duration_rain,
-        volume_rain,
-        duration_runoff,
-        volume_runoff,
-        runoff_ratio,
-        beginning_rain,
-        end_rain,
-        beginning_flow,
-        end_flow,
-    ) = step11_event_analysis(
-        beginning_rain,
-        end_rain,
-        beginning_flow,
-        end_flow,
-        rain,
-        flow,
-        time,
-        flow_threshold,
-        multiple=multiple,
-    )
-    print(beginning_rain, end_rain, beginning_flow, end_flow)
-    print(len(beginning_rain), len(end_rain), len(beginning_flow), len(end_flow))
-    return pd.DataFrame(
-        {
-            "BEGINNING_RAIN": beginning_rain,
-            "END_RAIN": end_rain,
-            "DURATION_RAIN": duration_rain,
-            "BEGINNING_FLOW": beginning_flow,
-            "END_FLOW": end_flow,
-            "DURATION_RUNOFF": duration_runoff,
-            "VOLUME_RAIN": volume_rain,
-            "VULUME_RUNOFF": volume_runoff,
-            "RUNOFF_RATIO": runoff_ratio,
-        }
-    )
+"""
+Author: Jingyi Wang, Yang Wang, and Wenyu Ouyang
+Date: 2023-10-28 09:23:22
+LastEditTime: 2024-03-23 17:16:39
+LastEditors: Wenyu Ouyang
+Description: DMCA-ESR method (https://doi.org/10.1029/2021WR031283)
+FilePath: \hydrodata\hydrodata\cleaner\dmca_esr.py
+Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
+"""
+
+import numpy as np
+import pandas as pd
+
+
+def movmean(X, n):
+    ones = np.ones(X.shape)
+    kernel = np.ones(n)
+    return np.convolve(X, kernel, mode="same") / np.convolve(ones, kernel, mode="same")
+
+
+def step1_step2_tr_and_fluctuations_timeseries(rain, flow, rain_min, max_window):
+    """
+    The first two steps are used for calculation of the catchment response time,
+    the rainfall and streamflow fluctuations, and rainfall fluctuation.
+
+    Parameters
+    ----------
+    rain : np.ndarray
+        unit is mm/h
+    flow : np.ndarray
+        unit is m³/h
+    rain_min : _type_
+        最小降雨量阈值
+    max_window : _type_
+        场次划分最大窗口, 决定场次长度
+
+    Returns
+    -------
+    _type_
+        _description_
+    """
+    rain = rain.T
+    flow = flow.T
+    rain_int = np.nancumsum(rain)
+    flow_int = np.nancumsum(flow)
+    T = rain.size
+    rain_mean = np.empty(((max_window - 1) // 2, T))
+    flow_mean = np.empty(((max_window - 1) // 2, T))
+    fluct_rain = np.empty(((max_window - 1) // 2, T))
+    fluct_flow = np.empty(((max_window - 1) // 2, T))
+    F_rain = np.empty((max_window - 1) // 2)
+    F_flow = np.empty((max_window - 1) // 2)
+    F_rain_flow = np.empty((max_window - 1) // 2)
+    rho = np.empty((max_window - 1) // 2)
+    for window in np.arange(3, max_window + 1, 2):
+        int_index = int((window - 1) / 2 - 1)
+        start_slice = int(window - 0.5 * (window - 1))
+        dst_slice = int(T - 0.5 * (window - 1))
+        # 新建一个循环体长度*数据长度的大数组
+        rain_mean[int_index] = movmean(rain_int, window)
+        flow_mean[int_index] = movmean(flow_int, window)
+        fluct_rain[int_index] = rain_int - rain_mean[int_index, :]
+        F_rain[int_index] = (1 / (T - window + 1)) * np.nansum(
+            (fluct_rain[int_index, start_slice:dst_slice]) ** 2
+        )
+        fluct_flow[int_index, np.newaxis] = flow_int - flow_mean[int_index, :]
+        F_flow[int_index] = (1 / (T - window + 1)) * np.nansum(
+            (fluct_flow[int_index, start_slice:dst_slice]) ** 2
+        )
+        F_rain_flow[int_index] = (1 / (T - window + 1)) * np.nansum(
+            (fluct_rain[int_index, start_slice:dst_slice])
+            * (fluct_flow[int_index, start_slice:dst_slice])
+        )
+        rho[int_index] = F_rain_flow[int_index] / (
+            np.sqrt(F_rain[int_index]) * np.sqrt(F_flow[int_index])
+        )
+    pos_min = np.argmin(rho)
+    Tr = pos_min + 1
+    tol_fluct_rain = (rain_min / (2 * Tr + 1)) * Tr
+    tol_fluct_flow = flow_int[-1] / 1e15
+    fluct_rain[pos_min, np.fabs(fluct_rain[pos_min, :]) < tol_fluct_rain] = 0
+    fluct_flow[pos_min, np.fabs(fluct_flow[pos_min, :]) < tol_fluct_flow] = 0
+    fluct_rain_Tr = fluct_rain[pos_min, :]
+    fluct_flow_Tr = fluct_flow[pos_min, :]
+    fluct_bivariate_Tr = fluct_rain_Tr * fluct_flow_Tr
+    fluct_bivariate_Tr[np.fabs(fluct_bivariate_Tr) < np.finfo(np.float64).eps] = (
+        0  # 便于比较
+    )
+    return Tr, fluct_rain_Tr, fluct_flow_Tr, fluct_bivariate_Tr
+
+
+def step3_core_identification(fluct_bivariate_Tr):
+    d = np.diff(
+        fluct_bivariate_Tr, prepend=[0], append=[0]
+    )  # 计算相邻数值差分，为0代表两端点处于0区间
+    d[np.fabs(d) < np.finfo(np.float64).eps] = 0  # 确保计算正确
+    d = np.logical_not(d)  # 求0-1数组，为真代表为0区间
+    d0 = np.logical_not(
+        np.convolve(d, [1, 1], "valid")
+    )  # 对相邻元素做OR，代表原数组数值是否处于某一0区间，再取反表示取有效值
+    valid = np.logical_or(fluct_bivariate_Tr, d0)  # 有效core
+    d_ = np.diff(valid, prepend=[0], append=[0])  # 求差分方便取上下边沿
+    beginning_core = np.argwhere(d_ == 1)  # 上边沿为begin
+    end_core = np.argwhere(d_ == -1) - 1  # 下边沿为end
+    return beginning_core, end_core
+
+
+def step4_end_rain_events(beginning_core, end_core, rain, fluct_rain_Tr, rain_min):
+    end_rain = end_core.copy()
+    rain = rain.T
+    for g in range(end_core.size):
+        if end_core[g] + 2 < fluct_rain_Tr.size and (
+            np.fabs(fluct_rain_Tr[end_core[g] + 1]) < np.finfo(np.float64).eps
+            and np.fabs(fluct_rain_Tr[end_core[g] + 2]) < np.finfo(np.float64).eps
+        ):
+            # case 1&2
+            if np.fabs(rain[end_core[g]]) < np.finfo(np.float64).eps:
+                # case 1
+                while (
+                    end_rain[g] > beginning_core[g]
+                    and np.fabs(rain[end_rain[g]]) < np.finfo(np.float64).eps
+                ):
+                    end_rain[g] = end_rain[g] - 1
+            else:
+                # case 2
+                bound = (
+                    beginning_core[g + 1] if g + 1 < beginning_core.size else rain.size
+                )
+                while end_rain[g] < bound and rain[end_rain[g]] > rain_min:
+                    end_rain[g] = end_rain[g] + 1
+                end_rain[g] = end_rain[g] - 1  # 回到最后一个
+        else:
+            # case 3
+            # 若在降水，先跳过
+            while end_rain[g] >= beginning_core[g] and rain[end_rain[g]] > rain_min:
+                end_rain[g] = end_rain[g] - 1
+            while end_rain[g] >= beginning_core[g] and rain[end_rain[g]] < rain_min:
+                end_rain[g] = end_rain[g] - 1
+    return end_rain
+
+
+def step5_beginning_rain_events(
+    beginning_core, end_rain, rain, fluct_rain_Tr, rain_min
+):
+    beginning_rain = beginning_core.copy()
+    rain = rain.T
+    for g in range(beginning_core.size):
+        if (
+            beginning_core[g] >= 2
+            and np.fabs(fluct_rain_Tr[beginning_core[g] - 1]) < np.finfo(np.float64).eps
+            and np.fabs(fluct_rain_Tr[beginning_core[g] - 2]) < np.finfo(np.float64).eps
+            and np.fabs(rain[beginning_core[g]]) < np.finfo(np.float64).eps
+        ):
+            # case 1
+            while (
+                beginning_rain[g] < end_rain[g]
+                and np.fabs(rain[beginning_rain[g]]) < np.finfo(np.float64).eps
+            ):
+                beginning_rain[g] = beginning_rain[g] + 1
+        else:
+            # case 2&3
+            bound = end_rain[g - 1] if g >= 1 else -1
+            while beginning_rain[g] > bound and rain[beginning_rain[g]] > rain_min:
+                beginning_rain[g] = beginning_rain[g] - 1
+            beginning_rain[g] = beginning_rain[g] + 1  # 回到第一个
+    return beginning_rain
+
+
+def step6_checks_on_rain_events(
+    beginning_rain, end_rain, rain, rain_min, beginning_core, end_core
+):
+    rain = rain.T
+    beginning_rain = beginning_rain.copy()
+    end_rain = end_rain.copy()
+    if beginning_rain[0] == 0:  # 掐头
+        beginning_rain = beginning_rain[1:]
+        end_rain = end_rain[1:]
+        beginning_core = beginning_core[1:]
+        end_core = end_core[1:]
+    if end_rain[-1] == rain.size - 1:  # 去尾
+        beginning_rain = beginning_rain[:-2]
+        end_rain = end_rain[:-2]
+        beginning_core = beginning_core[:-2]
+        end_core = end_core[:-2]
+    error_time_reversed = beginning_rain > end_rain
+    error_wrong_delimiter = np.logical_or(
+        rain[beginning_rain - 1] > rain_min, rain[end_rain + 1] > rain_min
+    )
+    beginning_rain[error_time_reversed] = -2
+    beginning_rain[error_wrong_delimiter] = -2
+    end_rain[error_time_reversed] = -2
+    end_rain[error_wrong_delimiter] = -2
+    beginning_core[error_time_reversed] = -2
+    beginning_core[error_wrong_delimiter] = -2
+    end_core[error_time_reversed] = -2
+    end_core[error_wrong_delimiter] = -2
+    beginning_rain = beginning_rain[beginning_rain != -2]
+    end_rain = end_rain[end_rain != -2]
+    beginning_core = beginning_core[beginning_core != -2]
+    end_core = end_core[end_core != -2]
+    return beginning_rain, end_rain, beginning_core, end_core
+
+
+def step7_end_flow_events(
+    end_rain_checked, beginning_core, end_core, rain, fluct_rain_Tr, fluct_flow_Tr, Tr
+):
+    end_flow = np.empty(end_core.size, dtype=int)
+    for g in range(end_rain_checked.size):
+        if end_core[g] + 2 < fluct_rain_Tr.size and (
+            np.fabs(fluct_rain_Tr[end_core[g] + 1]) < np.finfo(np.float64).eps
+            and np.fabs(fluct_rain_Tr[end_core[g] + 2]) < np.finfo(np.float64).eps
+        ):
+            # case 1
+            end_flow[g] = end_rain_checked[g]
+            bound = (
+                beginning_core[g + 1] + Tr if g + 1 < beginning_core.size else rain.size
+            )
+            bound = min(bound, rain.size)  # 防溢出
+            # 若flow为负，先跳过
+            while end_flow[g] < bound and fluct_flow_Tr[end_flow[g]] <= 0:
+                end_flow[g] = end_flow[g] + 1
+            while end_flow[g] < bound and fluct_flow_Tr[end_flow[g]] > 0:
+                end_flow[g] = end_flow[g] + 1
+            end_flow[g] = end_flow[g] - 1  # 回到最后一个
+        else:
+            # case 2
+            end_flow[g] = end_core[g]
+            while end_flow[g] >= beginning_core[g] and fluct_flow_Tr[end_flow[g]] <= 0:
+                end_flow[g] = end_flow[g] - 1
+    return end_flow
+
+
+def step8_beginning_flow_events(
+    beginning_rain_checked,
+    end_rain_checked,
+    rain,
+    beginning_core,
+    fluct_rain_Tr,
+    fluct_flow_Tr,
+):
+    beginning_flow = np.empty(beginning_rain_checked.size, dtype=int)
+    for g in range(beginning_rain_checked.size):
+        if beginning_core[g] >= 2 and (
+            np.fabs(fluct_rain_Tr[beginning_core[g] - 1]) < np.finfo(np.float64).eps
+            and np.fabs(fluct_rain_Tr[beginning_core[g] - 2]) < np.finfo(np.float64).eps
+        ):
+            beginning_flow[g] = beginning_rain_checked[g]  # case 1
+        else:
+            beginning_flow[g] = beginning_core[g]  # case 2
+        while (
+            beginning_flow[g] < end_rain_checked[g]
+            and fluct_flow_Tr[beginning_flow[g]] >= 0
+        ):
+            beginning_flow[g] = beginning_flow[g] + 1
+    return beginning_flow
+
+
+def step9_checks_on_flow_events(
+    beginning_rain_checked, end_rain_checked, beginning_flow, end_flow, fluct_flow_Tr
+):
+    beginning_flow_checked = np.empty_like(beginning_flow, dtype=object)
+    end_flow_checked = np.empty_like(end_flow, dtype=object)
+    for g in range(len(beginning_flow)):
+        if (
+            not np.isnan(beginning_flow[g])
+            and not np.isnan(end_flow[g])
+            and (
+                end_flow[g] <= beginning_flow[g]
+                or fluct_flow_Tr[beginning_flow[g]] > 0
+                or fluct_flow_Tr[end_flow[g]] < 0
+                or beginning_flow[g] < beginning_rain_checked[g]
+                or end_flow[g] < end_rain_checked[g]
+            )
+        ):
+            beginning_flow_checked[g] = np.nan
+            end_flow_checked[g] = np.nan
+        else:
+            beginning_flow_checked[g] = beginning_flow[g]
+            end_flow_checked[g] = end_flow[g]
+
+    index_events = [
+        i
+        for i in range(len(beginning_rain_checked))
+        if not np.isnan(beginning_rain_checked[i])
+        and not np.isnan(beginning_flow_checked[i])
+        and not np.isnan(end_rain_checked[i])
+        and not np.isnan(end_flow_checked[i])
+    ]
+
+    beginning_flow_ungrouped = beginning_flow_checked[index_events]
+    end_flow_ungrouped = end_flow_checked[index_events]
+    beginning_rain_ungrouped = beginning_rain_checked[index_events]
+    end_rain_ungrouped = end_rain_checked[index_events]
+    return (
+        beginning_rain_ungrouped,
+        end_rain_ungrouped,
+        beginning_flow_ungrouped,
+        end_flow_ungrouped,
+    )
+    # The following code is written by Wang, Yang
+    # error_time_reversed = beginning_flow > end_flow
+    # error_wrong_fluct = np.logical_or(
+    #     np.logical_or(fluct_flow_Tr[beginning_flow] > 0, fluct_flow_Tr[end_flow] < 0),
+    #     np.logical_or(
+    #         beginning_flow < beginning_rain_checked, end_flow < end_rain_checked
+    #     ),
+    # )
+    # beginning_flow[error_time_reversed] = -3
+    # beginning_flow[error_wrong_fluct] = -3
+    # end_flow[error_time_reversed] = -3
+    # end_flow[error_wrong_fluct] = -3
+    # beginning_flow = beginning_flow[beginning_flow != -3]
+    # end_flow = end_flow[end_flow != -3]
+
+    # beginning_rain_checked[error_time_reversed] = -3
+    # beginning_rain_checked[error_wrong_fluct] = -3
+    # end_rain_checked[error_time_reversed] = -3
+    # end_rain_checked[error_wrong_fluct] = -3
+    # beginning_rain = beginning_rain_checked[beginning_rain_checked != -3]
+    # end_rain = end_rain_checked[end_rain_checked != -3]
+    # return beginning_rain, end_rain, beginning_flow, end_flow
+
+
+def step10_checks_on_overlapping_events(
+    beginning_rain_ungrouped,
+    end_rain_ungrouped,
+    beginning_flow_ungrouped,
+    end_flow_ungrouped,
+    time,
+):
+    # rain
+    # order1 = np.reshape(
+    #     np.hstack(
+    #         (
+    #             np.reshape(beginning_rain_ungrouped, (-1, 1)),
+    #             np.reshape(end_rain_ungrouped, (-1, 1)),
+    #         )
+    #     ),
+    #     (1, -1),
+    # )
+    # reversed1 = np.diff(order1) <= 0
+    # order1[np.hstack((reversed1, [[False]]))] = -2
+    # order1[np.hstack(([[False]], reversed1))] = -2
+    # order1 = order1[order1 != -2]
+    # # flow
+    # order2 = np.reshape(
+    #     np.hstack(
+    #         (
+    #             np.reshape(beginning_flow_ungrouped, (-1, 1)),
+    #             np.reshape(end_flow_ungrouped, (-1, 1)),
+    #         )
+    #     ),
+    #     (1, -1),
+    # )
+    # reversed2 = np.diff(order2) <= 0
+    # order2[np.hstack((reversed2, [[False]]))] = -3
+    # order2[np.hstack(([[False]], reversed2))] = -3
+    # order2 = order2[order2 != -3]
+    # # group
+    # rain_grouped = np.reshape(order1, (-1, 2)).T
+    # beginning_rain_grouped = rain_grouped[0]
+    # end_rain_grouped = rain_grouped[1]
+    # flow_grouped = np.reshape(order2, (-1, 2)).T
+    # beginning_flow_grouped = flow_grouped[0]
+    # end_flow_grouped = flow_grouped[1]
+    # return (
+    #     time[beginning_rain_grouped],
+    #     time[end_rain_grouped],
+    #     time[beginning_flow_grouped],
+    #     time[end_flow_grouped],
+    # )
+
+    beginning_rain_ungrouped = beginning_rain_ungrouped.astype(float)
+    beginning_flow_ungrouped = beginning_flow_ungrouped.astype(float)
+    end_rain_ungrouped = end_rain_ungrouped.astype(float)
+    end_flow_ungrouped = end_flow_ungrouped.astype(float)
+    q = 1
+    marker_overlapping = []
+    for g in range(len(end_rain_ungrouped) - 1):
+        if (
+            end_rain_ungrouped[g] > beginning_rain_ungrouped[g + 1]
+            or end_flow_ungrouped[g] > beginning_flow_ungrouped[g + 1]
+        ):
+            marker_overlapping.append(g)
+            q += 1
+    if marker_overlapping:
+        q = 0
+        while q < len(marker_overlapping) - 1:
+            to_group = [marker_overlapping[q]]
+            while (
+                q < len(marker_overlapping)
+                and marker_overlapping[q] == marker_overlapping[q + 1] - 1
+            ):
+                to_group.append(marker_overlapping[q + 1])
+                q += 1
+
+            beginning_rain_ungrouped[to_group[0]] = beginning_rain_ungrouped[
+                to_group[0]
+            ]
+            beginning_flow_ungrouped[to_group[0]] = beginning_flow_ungrouped[
+                to_group[0]
+            ]
+            end_flow_ungrouped[to_group[0]] = end_flow_ungrouped[to_group[-1] + 1]
+            end_rain_ungrouped[to_group[0]] = end_rain_ungrouped[to_group[-1] + 1]
+
+            if len(to_group) > 1:
+                beginning_rain_ungrouped[to_group[1:]] = np.nan
+                beginning_flow_ungrouped[to_group[1:]] = np.nan
+                end_flow_ungrouped[to_group[1:]] = np.nan
+                end_rain_ungrouped[to_group[1:]] = np.nan
+
+            beginning_rain_ungrouped[to_group[-1] + 1] = np.nan
+            beginning_flow_ungrouped[to_group[-1] + 1] = np.nan
+            end_flow_ungrouped[to_group[-1] + 1] = np.nan
+            end_rain_ungrouped[to_group[-1] + 1] = np.nan
+
+            to_group = []
+            q += 1
+
+    index_events2 = np.where(
+        ~np.isnan(beginning_rain_ungrouped)
+        & ~np.isnan(beginning_flow_ungrouped)
+        & ~np.isnan(end_rain_ungrouped)
+        & ~np.isnan(end_flow_ungrouped)
+    )[0]
+    beginning_flow_grouped = beginning_flow_ungrouped[index_events2]
+    end_flow_grouped = end_flow_ungrouped[index_events2]
+    beginning_rain_grouped = beginning_rain_ungrouped[index_events2]
+    end_rain_grouped = end_rain_ungrouped[index_events2]
+    beginning_rain_grouped = beginning_rain_grouped.astype(int)
+    end_rain_grouped = end_rain_grouped.astype(int)
+    beginning_flow_grouped = beginning_flow_grouped.astype(int)
+    end_flow_grouped = end_flow_grouped.astype(int)
+    beginning_rain = time[beginning_rain_grouped]
+    end_rain = time[end_rain_grouped]
+    end_flow = time[end_flow_grouped]
+    beginning_flow = time[beginning_flow_grouped]
+    return beginning_rain, end_rain, beginning_flow, end_flow
+    # biliu_rain_division = pd.DataFrame({'BEGINNING_RAIN': BEGINNING_RAIN, 'END_RAIN': END_RAIN})
+    # biliu_rain_division.to_csv(os.path.join(definitions.ROOT_DIR, 'example/yingnariver_data/yingna_rain_flow_division/yingna_rain_division.txt'), sep='\t')
+    # biliu_flow_division = pd.DataFrame({'BEGINNING_FLOW': BEGINNING_FLOW, 'END_FLOW': END_FLOW})
+    # biliu_flow_division.to_csv(os.path.join(definitions.ROOT_DIR, 'example/yingnariver_data/yingna_rain_flow_division/yingna_flow_division.txt'), sep='\t')
+
+
+def baseflow_curve(beginning_flow, end_flow, flow, time):
+    baseflow = np.copy(flow)
+    beg_end_series = np.array([], dtype=beginning_flow[0].dtype)
+    for j in range(len(beginning_flow)):
+        beg_end_series = np.concatenate(
+            (beg_end_series, [beginning_flow[j], end_flow[j]])
+        )
+
+    for k in range(len(beg_end_series) - 1):
+        index_beg = np.where(time == beg_end_series[k])[0]
+        index_end = np.where(time == beg_end_series[k + 1])[0]
+        index_beg = int(index_beg)
+        index_end = int(index_end)
+        if (
+            len(np.where(np.isnan(flow[index_beg : index_end + 1]) == 1)[0])
+            >= len(flow[index_beg : index_end + 1]) * 0.9
+        ):
+            baseflow[index_beg : index_end + 1] = np.nan
+        elif index_end - index_beg == 1:
+            baseflow[index_beg] = flow[index_beg]
+            baseflow[index_end] = flow[index_end]
+        elif flow[index_beg] < flow[index_end]:
+            increment = (flow[index_end] - flow[index_beg]) / (index_end - index_beg)
+            for m in range(index_beg + 1, index_end):
+                baseflow[m] = baseflow[index_beg] + increment * (m - index_beg)
+        elif flow[index_beg] > flow[index_end]:
+            increment = (flow[index_beg] - flow[index_end]) / (index_end - index_beg)
+            for m in range(index_beg + 1, index_end):
+                baseflow[m] = baseflow[index_beg] - increment * (m - index_beg)
+
+    for m in range(len(baseflow)):
+        baseflow[m] = min(baseflow[m], flow[m])
+    return baseflow
+
+
+def step11_event_analysis(
+    beginning_rain,
+    end_rain,
+    beginning_flow,
+    end_flow,
+    rain,
+    flow,
+    time,
+    flow_threshold,
+    multiple=1,
+    flag=0,
+    duration_max=2400,
+):
+    """The step 11 is a new step for the DMCA-ESR method
+    we proposed to check again for the rainfall-runoff events.
+
+    Parameters
+    ----------
+    beginning_rain : _type_
+        _description_
+    end_rain : _type_
+        _description_
+    beginning_flow : _type_
+        _description_
+    end_flow : _type_
+        _description_
+    rain : _type_
+        _description_
+    flow : _type_
+        _description_
+    time : _type_
+        _description_
+    flag : int, by default 0
+        if flag != 1, calculation target is flow - baseflow,
+        if flag == 1, cal target is flow
+        the default value 0 is recommended as flag == 1 is just for comparison
+    multiple : int
+        1h means the multiple is 1, 1d means the multiple is 24
+    flow_threshold : float
+        flow threshold -- remove events with max flow lower than it
+        its unit is mm_h
+    duration_max : int
+        maximum duration of the rainfall-runoff events we set; unit is hour
+
+    Returns
+    -------
+    _type_
+        _description_
+    """
+    duration_rain = np.zeros(len(beginning_rain))
+    duration_runoff = np.zeros(len(beginning_flow))
+    volume_rain = np.zeros(len(beginning_rain))
+    volume_runoff = np.zeros(len(beginning_flow))
+    runoff_ratio = np.zeros(len(beginning_rain))
+    for h in range(len(beginning_rain)):
+        duration_rain[h] = (
+            (np.datetime64(end_rain[h]) - np.datetime64(beginning_rain[h]))
+            / np.timedelta64(1, "s")
+            / (60 * 60 * multiple)
+        )
+        duration_runoff[h] = (
+            (np.datetime64(end_flow[h]) - np.datetime64(beginning_flow[h]))
+            / np.timedelta64(1, "s")
+            / (60 * 60 * multiple)
+        )
+        index_beginning_event = np.where(time == beginning_rain[h])[0]
+        index_end_event = np.where(time == end_rain[h])[0]
+        index_beginning_event = int(index_beginning_event)
+        index_end_event = int(index_end_event)
+        volume_rain[h] = (
+            np.nansum(rain[index_beginning_event:index_end_event]) * multiple
+        )
+
+    if flag == 1:
+        for h in range(len(beginning_flow)):
+            index_beginning_event = np.where(time == beginning_flow[h])[0]
+            index_end_event = np.where(time == end_flow[h])[0]
+            volume_runoff[h] = (
+                np.nansum(flow[index_beginning_event:index_end_event]) * multiple
+            )
+    else:
+        baseflow = baseflow_curve(beginning_flow, end_flow, flow, time)
+        for h in range(len(beginning_flow)):
+            index_beginning_event = np.where(time == beginning_flow[h])[0]
+            index_end_event = np.where(time == end_flow[h])[0]
+            index_beginning_event = int(index_beginning_event)
+            index_end_event = int(index_end_event)
+
+            q = flow[index_beginning_event:index_end_event]
+            qb = baseflow[index_beginning_event:index_end_event]
+            volume_runoff[h] = np.nansum(q - qb) * multiple
+    runoff_ratio = volume_runoff / volume_rain
+    result_df = pd.DataFrame(
+        {
+            "BEGINNING_RAIN": beginning_rain,
+            "END_RAIN": end_rain,
+            "BEGINNING_FLOW": beginning_flow,
+            "END_FLOW": end_flow,
+            "DURATION_RAIN": duration_rain,
+            "DURATION_RUNOFF": duration_runoff,
+            "VOLUME_RAIN": volume_rain,
+            "VOLUME_RUNOFF": volume_runoff,
+            "RUNOFF_RATIO": runoff_ratio,
+        }
+    )
+    drop_list = []
+    for i in range(len(beginning_rain)):
+        index_beginning_event = np.where(time == beginning_flow[i])[0]
+        index_end_event = np.where(time == end_flow[i])[0]
+        index_beginning_event = int(index_beginning_event)
+        index_end_event = int(index_end_event)
+        if flow[index_beginning_event:index_end_event].max() < flow_threshold:
+            drop_list.append(i)
+        if result_df["DURATION_RAIN"].iloc[i] > duration_max:
+            drop_list.append(i)
+        if result_df["DURATION_RUNOFF"].iloc[i] > duration_max:
+            drop_list.append(i)
+        if result_df["VOLUME_RAIN"].iloc[i] == 0:
+            drop_list.append(i)
+        if result_df["VOLUME_RUNOFF"].iloc[i] == 0:
+            drop_list.append(i)
+        if runoff_ratio[i] > 1:
+            drop_list.append(i)
+    drop_array = np.unique(np.array(drop_list, dtype=int))
+    result_df = result_df.drop(index=drop_array)
+    duration_rain = result_df["DURATION_RAIN"]
+    volume_rain = result_df["VOLUME_RAIN"]
+    duration_runoff = result_df["DURATION_RUNOFF"]
+    volume_runoff = result_df["VOLUME_RUNOFF"]
+    runoff_ratio = result_df["RUNOFF_RATIO"]
+    beginning_rain = result_df["BEGINNING_RAIN"]
+    end_rain = result_df["END_RAIN"]
+    beginning_flow = result_df["BEGINNING_FLOW"]
+    end_flow = result_df["END_FLOW"]
+    return (
+        duration_rain,
+        volume_rain,
+        duration_runoff,
+        volume_runoff,
+        runoff_ratio,
+        beginning_rain,
+        end_rain,
+        beginning_flow,
+        end_flow,
+    )
+
+
+def rainfall_runoff_event_identify(
+    rain, flow, rain_min=0.02, max_window=100, multiple=24, flow_threshold=0.02
+):
+    """Full process for identification of rainfall-runoff events
+    We make function for each step, name the function as the step number and
+    add some anther necessary steps for the DMCA-ESR method.
+
+    Parameters
+    ----------
+    rain : pd.Series
+        rainfall time series, for the original data,
+        unit must be same as the time interval.
+        For example, when unit is mm/day, time interval is day
+    flow : pd.Series
+        streamflow time series,
+        the requirement for unit is same as the rainfall
+    rain_min : float
+        minimum rainfall threshold; its unit is mm/h
+    max_window : int
+        maximum window size in the first two steps
+        it has no unit, just meaning the number of time intervals,
+        no matter the time unit is hour, day, or others
+    multiple : int
+        24 for daily data, meaning convert unit from mm/day to mm/h
+        1 for hourly data
+    flow_threshold : float
+        events with max flow lower than it will be removed; its unit is mm/h
+    """
+    time = rain.index.to_numpy()
+    rain = rain.to_numpy() / multiple
+    flow = flow.to_numpy() / multiple
+    (
+        Tr,
+        fluct_rain_Tr,
+        fluct_flow_Tr,
+        fluct_bivariate_Tr,
+    ) = step1_step2_tr_and_fluctuations_timeseries(rain, flow, rain_min, max_window)
+    beginning_core, end_core = step3_core_identification(fluct_bivariate_Tr)
+    end_rain = step4_end_rain_events(
+        beginning_core, end_core, rain, fluct_rain_Tr, rain_min
+    )
+    beginning_rain = step5_beginning_rain_events(
+        beginning_core, end_rain, rain, fluct_rain_Tr, rain_min
+    )
+    (
+        beginning_rain_checked,
+        end_rain_checked,
+        beginning_core,
+        end_core,
+    ) = step6_checks_on_rain_events(
+        beginning_rain, end_rain, rain, rain_min, beginning_core, end_core
+    )
+    end_flow = step7_end_flow_events(
+        end_rain_checked,
+        beginning_core,
+        end_core,
+        rain,
+        fluct_rain_Tr,
+        fluct_flow_Tr,
+        Tr,
+    )
+    beginning_flow = step8_beginning_flow_events(
+        beginning_rain_checked,
+        end_rain_checked,
+        rain,
+        beginning_core,
+        fluct_rain_Tr,
+        fluct_flow_Tr,
+    )
+    (
+        beginning_rain_ungrouped,
+        end_rain_ungrouped,
+        beginning_flow_ungrouped,
+        end_flow_ungrouped,
+    ) = step9_checks_on_flow_events(
+        beginning_rain_checked,
+        end_rain_checked,
+        beginning_flow,
+        end_flow,
+        fluct_flow_Tr,
+    )
+    (
+        beginning_rain,
+        end_rain,
+        beginning_flow,
+        end_flow,
+    ) = step10_checks_on_overlapping_events(
+        beginning_rain_ungrouped,
+        end_rain_ungrouped,
+        beginning_flow_ungrouped,
+        end_flow_ungrouped,
+        time,
+    )
+    (
+        duration_rain,
+        volume_rain,
+        duration_runoff,
+        volume_runoff,
+        runoff_ratio,
+        beginning_rain,
+        end_rain,
+        beginning_flow,
+        end_flow,
+    ) = step11_event_analysis(
+        beginning_rain,
+        end_rain,
+        beginning_flow,
+        end_flow,
+        rain,
+        flow,
+        time,
+        flow_threshold,
+        multiple=multiple,
+    )
+    print(beginning_rain, end_rain, beginning_flow, end_flow)
+    print(len(beginning_rain), len(end_rain), len(beginning_flow), len(end_flow))
+    return pd.DataFrame(
+        {
+            "BEGINNING_RAIN": beginning_rain,
+            "END_RAIN": end_rain,
+            "DURATION_RAIN": duration_rain,
+            "BEGINNING_FLOW": beginning_flow,
+            "END_FLOW": end_flow,
+            "DURATION_RUNOFF": duration_runoff,
+            "VOLUME_RAIN": volume_rain,
+            "VULUME_RUNOFF": volume_runoff,
+            "RUNOFF_RATIO": runoff_ratio,
+        }
+    )
```

### Comparing `hydrodatasource-0.0.1/hydrodatasource/cleaner/fixdata.py` & `hydrodatasource-0.0.2/hydrodatasource/cleaner/fixdata.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,136 +1,175 @@
-import os
-
-import numpy as np
-import pandas as pd
-from shapely import distance
-
-
-# 雨量数据异常处理, 参见https://dlut-water.yuque.com/aq3llt/iag1ec/32727520
-def get_filter_data_by_time(data_path, rain_attr='DRP', time_attr='TM', id_attr='STCD', rain_max_hour=200, filter_list=None):
-    '''
-    :param data_path: 保存待处理数据文件的文件夹，姑且认为数据文件为“86_单位名称+站号.csv”形式，参考https://dlut-water.yuque.com/kgo8gd/tnld77/pum8d50qrbs1474h
-    :param rain_attr: 表格中标示降雨的属性（列名），默认为DRP
-    :param time_attr: 表格中标示时间的属性（列名），默认为TM
-    :param id_attr: 表格中标示站号的属性（列名），默认为STCD
-    :param rain_max_hour: 每小时最大降雨量，默认为200，超过这个阈值的排除
-    :param filter_list: 其他预处理过程得到的黑名单，以过滤不可用的站点
-    :return: 站点号与根据时间峰值排除后的表格构成的dict
-    '''
-    if filter_list is None:
-        filter_list = []
-    time_df_dict = {}
-    for dir_name, sub_dir, files in os.walk(data_path):
-        for file in files:
-            # 目前stcd采用文件名分离出的‘单位名称+站号’，和站点数据表里的站点号未必一致，需要另行考虑
-            stcd = (file.split('.')[0]).split('_')[1]
-            cached_csv_path = os.path.join(data_path, stcd + '.csv')
-            if (stcd not in filter_list) & (~os.path.exists(cached_csv_path)):
-                drop_list = []
-                csv_path = os.path.join(data_path, file)
-                table = pd.read_csv(csv_path, engine='c')
-                # 按降雨最大阈值为200和小时雨量一致性过滤索引
-                # 有些数据不严格按照小时尺度排列，出于简单可以一概按照小时重采样
-                if rain_attr in table.columns:
-                    table[time_attr] = pd.to_datetime(table[time_attr], format='%Y-%m-%d %H:%M:%S')
-                    table = table.drop(index=table.index[table[rain_attr].isna()])
-                    # 整小时数据，再按小时重采样求和，结果不变
-                    table = table.set_index(time_attr).resample('H').sum()
-                    cached_time_array = table.index[table[id_attr] != 0].to_numpy()
-                    cached_drp_array = table[rain_attr][table[id_attr] != 0].to_numpy()
-                    table[time_attr] = np.nan
-                    table[rain_attr][cached_time_array] = cached_drp_array
-                    table = table.fillna(-1).reset_index()
-                    for i in range(0, len(table[rain_attr])):
-                        if table[rain_attr][i] > rain_max_hour:
-                            drop_list.append(i)
-                        if i >= 5:
-                            hour_slice = table[rain_attr][i - 5:i + 1].to_numpy()
-                            if hour_slice.all() == np.mean(hour_slice):
-                                drop_list.extend(list(range(i - 5, i + 1)))
-                    drop_array = np.unique(np.array(drop_list, dtype=int))
-                    table = table.drop(index=drop_array)
-                    drop_array_minus = table.index[table[time_attr] == -1]
-                    table = table.drop(index=drop_array_minus)
-                time_df_dict[stcd] = table
-                # 在这里会生成csv数据表，存在副作用
-                table.to_csv(cached_csv_path)
-            elif (int(stcd) not in filter_list) & (os.path.exists(cached_csv_path)):
-                table = pd.read_csv(cached_csv_path, engine='c')
-                time_df_dict[stcd] = table
-    return time_df_dict
-
-
-def get_filter_data_by_space(time_df_dict, filter_list, station_gdf, csv_path, rain_attr='DRP', time_attr='TM', id_attr='STCD'):
-    '''
-    :param time_df_dict: 根据get_filter_data_by_time()得到的中间数据dict
-    :param filter_list: 其他预处理过程得到的黑名单，以过滤不可用的站点
-    :param station_gdf: 存储站点位置的GeoDataFrame
-    :param csv_path: 按站点保存清洗后数据的文件夹
-    :param rain_attr: 表格中标示降雨的属性（列名），默认为DRP
-    :param time_attr: 表格中标示时间的属性（列名），默认为TM
-    :param id_attr: station_gdf表格中标示站号的属性（列名），默认为STCD
-    :return: 站点号与根据空间均值排除后的表格构成的dict
-    '''
-    neighbor_stas_dict = find_neighbor_dict(station_gdf, filter_list)[0]
-    space_df_dict = {}
-    for key in time_df_dict:
-        time_drop_list = []
-        neighbor_stas = neighbor_stas_dict[key]
-        table = time_df_dict[key]
-        table = table.set_index(time_attr)
-        for time in table.index:
-            rain_time_dict = {}
-            for neighbor in neighbor_stas:
-                neighbor_df = time_df_dict[str(neighbor)]
-                neighbor_df = neighbor_df.set_index(time_attr)
-                if time in neighbor_df.index:
-                    rain_time_dict[str(neighbor)] = neighbor_df[rain_attr][time]
-            if len(rain_time_dict) == 0:
-                continue
-            elif 0 < len(rain_time_dict) < 12:
-                weight_rain = 0
-                weight_dis = 0
-                for sta in rain_time_dict.keys():
-                    point = station_gdf.geometry[station_gdf[id_attr] == str(sta)].values[0]
-                    point_self = station_gdf.geometry[station_gdf[id_attr] == str(key)].values[0]
-                    dis = distance(point, point_self)
-                    weight_rain += table[rain_attr][time] / (dis ** 2)
-                    weight_dis += 1 / (dis ** 2)
-                interp_rain = weight_rain / weight_dis
-                if abs(interp_rain - table[rain_attr][time]) > 4:
-                    time_drop_list.append(time)
-            elif len(rain_time_dict) >= 12:
-                rain_time_series = pd.Series(rain_time_dict.values())
-                quantile_25 = rain_time_series.quantile(q=0.25)
-                quantile_75 = rain_time_series.quantile(q=0.75)
-                average = rain_time_series.mean()
-                if rain_attr in table.columns:
-                    MA_Tct = (table[rain_attr][time] - average) / (quantile_75 - quantile_25)
-                    if MA_Tct > 4:
-                        time_drop_list.append(time)
-        table = table.drop(index=time_drop_list).drop(columns=['Unnamed: 0'])
-        space_df_dict[key] = table
-        # 会生成csv文件，有副作用
-        table.to_csv(os.path.join(csv_path, key+'.csv'))
-    return space_df_dict
-
-
-def find_neighbor_dict(station_gdf, filter_list, id_attr='STCD'):
-    '''
-    :param station_gdf: 存储有站点位置的GeoDataFrame
-    :param filter_list: 其他预处理过程得到的黑名单，以过滤不可用的站点
-    :param id_attr: station_gdf表格中标示站号的属性（列名），默认为STCD
-    :return: 与各站相邻的站点号（取0-0.2度）
-    '''
-    station_gdf = station_gdf.set_index(id_attr).drop(index=filter_list).reset_index()
-    station_gdf[id_attr] = station_gdf[id_attr].astype('str')
-    neighbor_dict = {}
-    for i in range(0, len(station_gdf.geometry)):
-        stcd = station_gdf[id_attr][i]
-        station_gdf['distance'] = station_gdf.apply(lambda x:
-                                                          distance(station_gdf.geometry[i], x.geometry), axis=1)
-        nearest_stas = station_gdf[(station_gdf['distance'] > 0) & (station_gdf['distance'] <= 0.2)]
-        nearest_stas_list = nearest_stas[id_attr].to_list()
-        neighbor_dict[stcd] = nearest_stas_list
-    station_gdf = station_gdf.drop(columns=['distance'])
-    return neighbor_dict
+import os
+
+import numpy as np
+import pandas as pd
+from shapely import distance
+
+
+# 雨量数据异常处理, 参见https://dlut-water.yuque.com/aq3llt/iag1ec/32727520
+def get_filter_data_by_time(
+    data_path,
+    rain_attr="DRP",
+    time_attr="TM",
+    id_attr="STCD",
+    rain_max_hour=200,
+    filter_list=None,
+):
+    """
+
+    Parameters
+    ----------
+    data_path : _type_
+        保存待处理数据文件的文件夹，姑且认为数据文件为“86_单位名称+站号.csv”形式，参考https://dlut-water.yuque.com/kgo8gd/tnld77/pum8d50qrbs1474h
+    rain_attr : str, optional
+        表格中标示降雨的属性（列名），默认为DRP, by default "DRP"
+    time_attr : str, optional
+        表格中标示时间的属性（列名），默认为TM, by default "TM"
+    id_attr : str, optional
+        表格中标示站号的属性（列名），默认为STCD, by default "STCD"
+    rain_max_hour : int, optional
+        每小时最大降雨量，默认为200，超过这个阈值的排除, by default 200
+    filter_list : _type_, optional
+        其他预处理过程得到的黑名单，以过滤不可用的站点, by default None
+
+    Returns
+    -------
+    _type_
+        _description_
+    """
+    if filter_list is None:
+        filter_list = []
+    time_df_dict = {}
+    for dir_name, sub_dir, files in os.walk(data_path):
+        for file in files:
+            # 目前stcd采用文件名分离出的‘单位名称+站号’，和站点数据表里的站点号未必一致，需要另行考虑
+            stcd = (file.split(".")[0]).split("_")[1]
+            cached_csv_path = os.path.join(data_path, stcd + ".csv")
+            if (stcd not in filter_list) & (~os.path.exists(cached_csv_path)):
+                drop_list = []
+                csv_path = os.path.join(data_path, file)
+                table = pd.read_csv(csv_path, engine="c")
+                # 按降雨最大阈值为200和小时雨量一致性过滤索引
+                # 有些数据不严格按照小时尺度排列，出于简单可以一概按照小时重采样
+                if rain_attr in table.columns:
+                    table[time_attr] = pd.to_datetime(
+                        table[time_attr], format="%Y-%m-%d %H:%M:%S"
+                    )
+                    table = table.drop(index=table.index[table[rain_attr].isna()])
+                    # 整小时数据，再按小时重采样求和，结果不变
+                    table = table.set_index(time_attr).resample("H").sum()
+                    cached_time_array = table.index[table[id_attr] != 0].to_numpy()
+                    cached_drp_array = table[rain_attr][table[id_attr] != 0].to_numpy()
+                    table[time_attr] = np.nan
+                    table[rain_attr][cached_time_array] = cached_drp_array
+                    table = table.fillna(-1).reset_index()
+                    for i in range(len(table[rain_attr])):
+                        if table[rain_attr][i] > rain_max_hour:
+                            drop_list.append(i)
+                        if i >= 5:
+                            hour_slice = table[rain_attr][i - 5 : i + 1].to_numpy()
+                            if hour_slice.all() == np.mean(hour_slice):
+                                drop_list.extend(list(range(i - 5, i + 1)))
+                    drop_array = np.unique(np.array(drop_list, dtype=int))
+                    table = table.drop(index=drop_array)
+                    drop_array_minus = table.index[table[time_attr] == -1]
+                    table = table.drop(index=drop_array_minus)
+                time_df_dict[stcd] = table
+                # 在这里会生成csv数据表，存在副作用
+                table.to_csv(cached_csv_path)
+            elif (int(stcd) not in filter_list) & (os.path.exists(cached_csv_path)):
+                table = pd.read_csv(cached_csv_path, engine="c")
+                time_df_dict[stcd] = table
+    return time_df_dict
+
+
+def get_filter_data_by_space(
+    time_df_dict,
+    filter_list,
+    station_gdf,
+    csv_path,
+    rain_attr="DRP",
+    time_attr="TM",
+    id_attr="STCD",
+):
+    """
+    :param time_df_dict: 根据get_filter_data_by_time()得到的中间数据dict
+    :param filter_list: 其他预处理过程得到的黑名单，以过滤不可用的站点
+    :param station_gdf: 存储站点位置的GeoDataFrame
+    :param csv_path: 按站点保存清洗后数据的文件夹
+    :param rain_attr: 表格中标示降雨的属性（列名），默认为DRP
+    :param time_attr: 表格中标示时间的属性（列名），默认为TM
+    :param id_attr: station_gdf表格中标示站号的属性（列名），默认为STCD
+    :return: 站点号与根据空间均值排除后的表格构成的dict
+    """
+    neighbor_stas_dict = find_neighbor_dict(station_gdf, filter_list)[0]
+    space_df_dict = {}
+    for key in time_df_dict:
+        time_drop_list = []
+        neighbor_stas = neighbor_stas_dict[key]
+        table = time_df_dict[key]
+        table = table.set_index(time_attr)
+        for time in table.index:
+            rain_time_dict = {}
+            for neighbor in neighbor_stas:
+                neighbor_df = time_df_dict[str(neighbor)]
+                neighbor_df = neighbor_df.set_index(time_attr)
+                if time in neighbor_df.index:
+                    rain_time_dict[str(neighbor)] = neighbor_df[rain_attr][time]
+            if not rain_time_dict:
+                continue
+            elif 0 < len(rain_time_dict) < 12:
+                weight_rain = 0
+                weight_dis = 0
+                for sta in rain_time_dict:
+                    point = station_gdf.geometry[
+                        station_gdf[id_attr] == str(sta)
+                    ].values[0]
+                    point_self = station_gdf.geometry[
+                        station_gdf[id_attr] == str(key)
+                    ].values[0]
+                    dis = distance(point, point_self)
+                    weight_rain += table[rain_attr][time] / (dis**2)
+                    weight_dis += 1 / (dis**2)
+                interp_rain = weight_rain / weight_dis
+                if abs(interp_rain - table[rain_attr][time]) > 4:
+                    time_drop_list.append(time)
+            elif len(rain_time_dict) >= 12:
+                rain_time_series = pd.Series(rain_time_dict.values())
+                quantile_25 = rain_time_series.quantile(q=0.25)
+                quantile_75 = rain_time_series.quantile(q=0.75)
+                average = rain_time_series.mean()
+                if rain_attr in table.columns:
+                    MA_Tct = (table[rain_attr][time] - average) / (
+                        quantile_75 - quantile_25
+                    )
+                    if MA_Tct > 4:
+                        time_drop_list.append(time)
+        table = table.drop(index=time_drop_list).drop(columns=["Unnamed: 0"])
+        space_df_dict[key] = table
+        # 会生成csv文件，有副作用
+        table.to_csv(os.path.join(csv_path, key + ".csv"))
+    return space_df_dict
+
+
+def find_neighbor_dict(station_gdf, filter_list, id_attr="STCD"):
+    """
+    :param station_gdf: 存储有站点位置的GeoDataFrame
+    :param filter_list: 其他预处理过程得到的黑名单，以过滤不可用的站点
+    :param id_attr: station_gdf表格中标示站号的属性（列名），默认为STCD
+    :return: 与各站相邻的站点号（取0-0.2度）
+    """
+    station_gdf = station_gdf.set_index(id_attr).drop(index=filter_list).reset_index()
+    station_gdf[id_attr] = station_gdf[id_attr].astype("str")
+    neighbor_dict = {}
+    for i in range(len(station_gdf.geometry)):
+        stcd = station_gdf[id_attr][i]
+        station_gdf["distance"] = station_gdf.apply(
+            lambda x: distance(station_gdf.geometry[i], x.geometry), axis=1
+        )
+        nearest_stas = station_gdf[
+            (station_gdf["distance"] > 0) & (station_gdf["distance"] <= 0.2)
+        ]
+        nearest_stas_list = nearest_stas[id_attr].to_list()
+        neighbor_dict[stcd] = nearest_stas_list
+    station_gdf = station_gdf.drop(columns=["distance"])
+    return neighbor_dict
```

### Comparing `hydrodatasource-0.0.1/hydrodatasource/cleaner/get_moving_inq.py` & `hydrodatasource-0.0.2/hydrodatasource/cleaner/get_moving_inq.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,134 +1,209 @@
-import numpy as np
-import pandas as pd
-from pykalman import KalmanFilter
-
-
-def calculate_esm(QFi, Qi):  # 计算平滑度
-    numerator_list = []
-    denominator_list = []
-    for i in range(len(QFi) - 1):
-        numerator = (QFi.values[i + 1] - QFi.values[i]) ** 2
-        denominator = (Qi.values[i + 1] - Qi.values[i]) ** 2
-        numerator_list.append(numerator)
-        denominator_list.append(denominator)
-    numerator_total = np.sum(numerator_list)
-    denominator_total = np.sum(denominator_list)
-    esm = 1 - numerator_total / denominator_total
-    return esm
-
-
-def get_moving_average_inq(inq_data_df):
-    """
-    :param inq_data_df: 入库流量表格，需要有TM（时间）和INQ（入库流量）两列
-    :return:
-    """
-    inq_data = inq_data_df['INQ']
-    inq_data_df['TM'] = pd.to_datetime(inq_data_df['TM'], format="%d/%m/%Y %H:%M")
-    # 滑动平均
-    window_size = 5
-    inq_moving_average = np.convolve(inq_data_df['INQ'], np.ones(window_size) / window_size, mode='same')
-    # 五点三次
-    QF = np.zeros(len(inq_data))
-    QF[0] = 1 / 70 * (69 * inq_data[0] + 4 * inq_data[1] - 6 * inq_data[2] + 4 * inq_data[3] - inq_data[4])
-    QF[1] = 1 / 30 * (2 * inq_data[0] + 27 * inq_data[1] + 12 * inq_data[2] - 8 * inq_data[3] + 2 * inq_data[4])
-    for i in range(2, len(inq_data) - 2):
-        QF[i] = 1 / 35 * (
-                (-3) * inq_data[i - 2] + 12 * inq_data[i - 1] + 17 * inq_data[i] + 12 * inq_data[i + 1] - 3 * inq_data[
-                i + 2])
-    QF[len(inq_data) - 2] = 1 / 35 * (
-            2 * inq_data[len(inq_data) - 5] - 8 * inq_data[len(inq_data) - 4] + 12 * inq_data[len(inq_data) - 3] + 27 *
-            inq_data[len(inq_data) - 2] + 2 * inq_data[len(inq_data) - 1])
-    QF[len(inq_data) - 1] = 1 / 70 * (
-            (-1) * inq_data[len(inq_data) - 5] + 4 * inq_data[len(inq_data) - 4] - 6 * inq_data[len(inq_data) - 3] + 4 *
-            inq_data[len(inq_data) - 2] + 69 * inq_data[len(inq_data) - 1])
-    # 卡尔曼滤波
-    initial_state_mean = 0
-    initial_state_covariance = 0.5
-    observation_covariance = 0.5
-    transition_covariance = 0.5
-    kf = KalmanFilter(
-        initial_state_mean=initial_state_mean,
-        initial_state_covariance=initial_state_covariance,
-        observation_covariance=observation_covariance,
-        transition_covariance=transition_covariance,
-        n_dim_obs=1
-    )
-    kf = kf.em(inq_data, n_iter=10)
-    inq_Kalman, _ = kf.filter(inq_data)
-    inq_Kalman = np.ravel(inq_Kalman)
-    result_df = pd.DataFrame({
-        'TM': inq_data_df['TM'],
-        'INQ_moving': inq_moving_average,
-        'INQ_QF': QF,
-        'INQ_Kalman': inq_Kalman.flatten(),
-        'INQ_orig': inq_data_df['INQ'],
-    })
-    # 计算误差
-    W_bias_rela_moving_list = []
-    Q_bias_rela_moving_list = []
-    time_bias_moving_list = []
-    esm_bias_moving_list = []
-    W_bias_rela_Kalman_list = []
-    Q_bias_rela_Kalman_list = []
-    time_bias_Kalman_list = []
-    esm_bias_Kalman_list = []
-    W_bias_rela_QF_list = []
-    Q_bias_rela_QF_list = []
-    time_bias_QF_list = []
-    esm_bias_QF_list = []
-    inq_moving_filtered = result_df['INQ_moving']
-    inq_QF_filtered = result_df['INQ_QF']
-    inq_Kalman_filtered = result_df['INQ_Kalman']
-    inq_orig_filtered = result_df['INQ_orig']
-    # 滑动平均的误差
-    W_bias_rela_moving = abs(inq_moving_filtered.sum() - inq_orig_filtered.sum()) / inq_orig_filtered.sum()
-    Q_bias_rela_moving = abs(inq_moving_filtered.max() - inq_orig_filtered.max()) / inq_orig_filtered.max()
-    time_bias_moving = abs(inq_moving_filtered.argmax() - inq_orig_filtered.argmax()) / inq_orig_filtered.argmax()
-    esm_bias_moving = calculate_esm(inq_moving_filtered, inq_orig_filtered)
-    W_bias_rela_moving_list.append(W_bias_rela_moving)
-    Q_bias_rela_moving_list.append(Q_bias_rela_moving)
-    time_bias_moving_list.append(time_bias_moving)
-    esm_bias_moving_list.append(esm_bias_moving)
-    # 五点三次的误差
-    W_bias_rela_QF = abs(inq_QF_filtered.sum() - inq_orig_filtered.sum()) / inq_orig_filtered.sum()
-    Q_bias_rela_QF = abs(inq_QF_filtered.max() - inq_orig_filtered.max()) / inq_orig_filtered.max()
-    time_bias_QF = abs(inq_QF_filtered.argmax() - inq_orig_filtered.argmax()) / inq_orig_filtered.argmax()
-    esm_bias_QF = calculate_esm(inq_QF_filtered, inq_orig_filtered)
-    W_bias_rela_QF_list.append(W_bias_rela_QF)
-    Q_bias_rela_QF_list.append(Q_bias_rela_QF)
-    time_bias_QF_list.append(time_bias_QF)
-    esm_bias_QF_list.append(esm_bias_QF)
-    # 卡尔曼滤波的误差
-    W_bias_rela_Kalman = abs(inq_Kalman_filtered.sum() - inq_orig_filtered.sum()) / inq_orig_filtered.sum()
-    Q_bias_rela_Kalman = abs(inq_Kalman_filtered.max() - inq_orig_filtered.max()) / inq_orig_filtered.max()
-    time_bias_Kalman = abs(inq_Kalman_filtered.argmax() - inq_orig_filtered.argmax()) / inq_orig_filtered.argmax()
-    esm_bias_Kalman = calculate_esm(inq_Kalman_filtered, inq_orig_filtered)
-    W_bias_rela_Kalman_list.append(W_bias_rela_Kalman)
-    Q_bias_rela_Kalman_list.append(Q_bias_rela_Kalman)
-    time_bias_Kalman_list.append(time_bias_Kalman)
-    esm_bias_Kalman_list.append(esm_bias_Kalman)
-    inq_bias_df = pd.DataFrame({
-        'TM': inq_data_df['TM'],
-        'INQ_moving': inq_moving_average,
-        'INQ_QF': QF,
-        'INQ_Kalman': inq_Kalman.flatten(),
-        'INQ_orig': inq_data_df['INQ'],
-
-    })
-    bias = pd.DataFrame({
-        # 'TM': inq_data_df['TM'],
-        'W_bias_rela_moving_list': W_bias_rela_moving_list,
-        'Q_bias_rela_moving_list': Q_bias_rela_moving_list,
-        'time_bias_moving_list': time_bias_moving_list,
-        'esm_bias_moving_list': esm_bias_moving_list,
-        'W_bias_rela_Kalman_list': W_bias_rela_Kalman_list,
-        'Q_bias_rela_Kalman_list': Q_bias_rela_Kalman_list,
-        'time_bias_Kalman_list': time_bias_Kalman_list,
-        'esm_bias_Kalman_list': esm_bias_Kalman_list,
-        'W_bias_rela_QF_list': W_bias_rela_QF_list,
-        'W_bias_rela_QF_list': W_bias_rela_QF_list,
-        'Q_bias_rela_QF_list': Q_bias_rela_QF_list,
-        'time_bias_QF_list': time_bias_QF_list,
-        'esm_bias_QF_list': esm_bias_QF_list
-    })
-    return inq_bias_df
+import numpy as np
+import pandas as pd
+from pykalman import KalmanFilter
+
+
+def calculate_esm(QFi, Qi):  # 计算平滑度
+    numerator_list = []
+    denominator_list = []
+    for i in range(len(QFi) - 1):
+        numerator = (QFi.values[i + 1] - QFi.values[i]) ** 2
+        denominator = (Qi.values[i + 1] - Qi.values[i]) ** 2
+        numerator_list.append(numerator)
+        denominator_list.append(denominator)
+    numerator_total = np.sum(numerator_list)
+    denominator_total = np.sum(denominator_list)
+    return 1 - numerator_total / denominator_total
+
+
+def get_moving_average_inq(inq_data_df):
+    """
+    :param inq_data_df: 入库流量表格，需要有TM（时间）和INQ（入库流量）两列
+    :return:
+    """
+    inq_data = inq_data_df["INQ"]
+    inq_data_df["TM"] = pd.to_datetime(inq_data_df["TM"], format="%d/%m/%Y %H:%M")
+    # 滑动平均
+    window_size = 5
+    inq_moving_average = np.convolve(
+        inq_data_df["INQ"], np.ones(window_size) / window_size, mode="same"
+    )
+    # 五点三次
+    QF = np.zeros(len(inq_data))
+    QF[0] = (
+        1
+        / 70
+        * (
+            69 * inq_data[0]
+            + 4 * inq_data[1]
+            - 6 * inq_data[2]
+            + 4 * inq_data[3]
+            - inq_data[4]
+        )
+    )
+    QF[1] = (
+        1
+        / 30
+        * (
+            2 * inq_data[0]
+            + 27 * inq_data[1]
+            + 12 * inq_data[2]
+            - 8 * inq_data[3]
+            + 2 * inq_data[4]
+        )
+    )
+    for i in range(2, len(inq_data) - 2):
+        QF[i] = (
+            1
+            / 35
+            * (
+                (-3) * inq_data[i - 2]
+                + 12 * inq_data[i - 1]
+                + 17 * inq_data[i]
+                + 12 * inq_data[i + 1]
+                - 3 * inq_data[i + 2]
+            )
+        )
+    QF[len(inq_data) - 2] = (
+        1
+        / 35
+        * (
+            2 * inq_data[len(inq_data) - 5]
+            - 8 * inq_data[len(inq_data) - 4]
+            + 12 * inq_data[len(inq_data) - 3]
+            + 27 * inq_data[len(inq_data) - 2]
+            + 2 * inq_data[len(inq_data) - 1]
+        )
+    )
+    QF[len(inq_data) - 1] = (
+        1
+        / 70
+        * (
+            (-1) * inq_data[len(inq_data) - 5]
+            + 4 * inq_data[len(inq_data) - 4]
+            - 6 * inq_data[len(inq_data) - 3]
+            + 4 * inq_data[len(inq_data) - 2]
+            + 69 * inq_data[len(inq_data) - 1]
+        )
+    )
+    # 卡尔曼滤波
+    initial_state_mean = 0
+    initial_state_covariance = 0.5
+    observation_covariance = 0.5
+    transition_covariance = 0.5
+    kf = KalmanFilter(
+        initial_state_mean=initial_state_mean,
+        initial_state_covariance=initial_state_covariance,
+        observation_covariance=observation_covariance,
+        transition_covariance=transition_covariance,
+        n_dim_obs=1,
+    )
+    kf = kf.em(inq_data, n_iter=10)
+    inq_Kalman, _ = kf.filter(inq_data)
+    inq_Kalman = np.ravel(inq_Kalman)
+    result_df = pd.DataFrame(
+        {
+            "TM": inq_data_df["TM"],
+            "INQ_moving": inq_moving_average,
+            "INQ_QF": QF,
+            "INQ_Kalman": inq_Kalman.flatten(),
+            "INQ_orig": inq_data_df["INQ"],
+        }
+    )
+    # 计算误差
+    W_bias_rela_moving_list = []
+    Q_bias_rela_moving_list = []
+    time_bias_moving_list = []
+    esm_bias_moving_list = []
+    W_bias_rela_Kalman_list = []
+    Q_bias_rela_Kalman_list = []
+    time_bias_Kalman_list = []
+    esm_bias_Kalman_list = []
+    W_bias_rela_QF_list = []
+    Q_bias_rela_QF_list = []
+    time_bias_QF_list = []
+    esm_bias_QF_list = []
+    inq_moving_filtered = result_df["INQ_moving"]
+    inq_QF_filtered = result_df["INQ_QF"]
+    inq_Kalman_filtered = result_df["INQ_Kalman"]
+    inq_orig_filtered = result_df["INQ_orig"]
+    # 滑动平均的误差
+    W_bias_rela_moving = (
+        abs(inq_moving_filtered.sum() - inq_orig_filtered.sum())
+        / inq_orig_filtered.sum()
+    )
+    Q_bias_rela_moving = (
+        abs(inq_moving_filtered.max() - inq_orig_filtered.max())
+        / inq_orig_filtered.max()
+    )
+    time_bias_moving = (
+        abs(inq_moving_filtered.argmax() - inq_orig_filtered.argmax())
+        / inq_orig_filtered.argmax()
+    )
+    esm_bias_moving = calculate_esm(inq_moving_filtered, inq_orig_filtered)
+    W_bias_rela_moving_list.append(W_bias_rela_moving)
+    Q_bias_rela_moving_list.append(Q_bias_rela_moving)
+    time_bias_moving_list.append(time_bias_moving)
+    esm_bias_moving_list.append(esm_bias_moving)
+    # 五点三次的误差
+    W_bias_rela_QF = (
+        abs(inq_QF_filtered.sum() - inq_orig_filtered.sum()) / inq_orig_filtered.sum()
+    )
+    Q_bias_rela_QF = (
+        abs(inq_QF_filtered.max() - inq_orig_filtered.max()) / inq_orig_filtered.max()
+    )
+    time_bias_QF = (
+        abs(inq_QF_filtered.argmax() - inq_orig_filtered.argmax())
+        / inq_orig_filtered.argmax()
+    )
+    esm_bias_QF = calculate_esm(inq_QF_filtered, inq_orig_filtered)
+    W_bias_rela_QF_list.append(W_bias_rela_QF)
+    Q_bias_rela_QF_list.append(Q_bias_rela_QF)
+    time_bias_QF_list.append(time_bias_QF)
+    esm_bias_QF_list.append(esm_bias_QF)
+    # 卡尔曼滤波的误差
+    W_bias_rela_Kalman = (
+        abs(inq_Kalman_filtered.sum() - inq_orig_filtered.sum())
+        / inq_orig_filtered.sum()
+    )
+    Q_bias_rela_Kalman = (
+        abs(inq_Kalman_filtered.max() - inq_orig_filtered.max())
+        / inq_orig_filtered.max()
+    )
+    time_bias_Kalman = (
+        abs(inq_Kalman_filtered.argmax() - inq_orig_filtered.argmax())
+        / inq_orig_filtered.argmax()
+    )
+    esm_bias_Kalman = calculate_esm(inq_Kalman_filtered, inq_orig_filtered)
+    W_bias_rela_Kalman_list.append(W_bias_rela_Kalman)
+    Q_bias_rela_Kalman_list.append(Q_bias_rela_Kalman)
+    time_bias_Kalman_list.append(time_bias_Kalman)
+    esm_bias_Kalman_list.append(esm_bias_Kalman)
+    inq_bias_df = pd.DataFrame(
+        {
+            "TM": inq_data_df["TM"],
+            "INQ_moving": inq_moving_average,
+            "INQ_QF": QF,
+            "INQ_Kalman": inq_Kalman.flatten(),
+            "INQ_orig": inq_data_df["INQ"],
+        }
+    )
+    bias = pd.DataFrame(
+        {
+            # 'TM': inq_data_df['TM'],
+            "W_bias_rela_moving_list": W_bias_rela_moving_list,
+            "Q_bias_rela_moving_list": Q_bias_rela_moving_list,
+            "time_bias_moving_list": time_bias_moving_list,
+            "esm_bias_moving_list": esm_bias_moving_list,
+            "W_bias_rela_Kalman_list": W_bias_rela_Kalman_list,
+            "Q_bias_rela_Kalman_list": Q_bias_rela_Kalman_list,
+            "time_bias_Kalman_list": time_bias_Kalman_list,
+            "esm_bias_Kalman_list": esm_bias_Kalman_list,
+            "W_bias_rela_QF_list": W_bias_rela_QF_list,
+            "W_bias_rela_QF_list": W_bias_rela_QF_list,
+            "Q_bias_rela_QF_list": Q_bias_rela_QF_list,
+            "time_bias_QF_list": time_bias_QF_list,
+            "esm_bias_QF_list": esm_bias_QF_list,
+        }
+    )
+    return inq_bias_df
```

### Comparing `hydrodatasource-0.0.1/hydrodatasource/cleaner/smooth_inq.py` & `hydrodatasource-0.0.2/hydrodatasource/cleaner/smooth_inq.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,380 +1,438 @@
-import xarray as xr
-import pandas as pd
-import numpy as np
-import matplotlib.pyplot as plt
-from scipy.signal import cwt, morlet, butter, filtfilt
-from scipy.fft import fft, ifft, fftfreq
-from scipy.optimize import curve_fit
-import os
-
-class Cleaner:
-    """
-    参数中文说明如下：
-    - file_path (必选项): 文件路径，指定要处理的数据文件路径。支持.txt格式。
-    - column_id: ID 列名，用于标识数据中的不同组或实例。若不表明则默认全体数据为一个分组。
-    - ID_list: ID 列的值列表，指定要处理的特定 ID 列表。
-    - column_flow (必选项): 流量数据列名，在 DataFrame 中表示流量的列名。
-    - column_time (必选项): 时间数据列名，在 DataFrame 中表示时间的列名。
-    - start_time: 起始时间，指定要处理的数据时间范围的起始时间。
-    - end_time: 结束时间，指定要处理的数据时间范围的结束时间。
-    - preprocess: 数据预处理标志，指示是否进行数据预处理优化（如平滑缺失值）。默认为 True。
-    - method: 处理函数类型，要使用的特定处理函数类型。选项包括 'FFT'、'wavelet'、'kalman'、'moving_average'、'moving_average_difference'、'robust'、'lowpass'，默认为 'moving_average'。
-    - save_path: 保存路径，指定处理后数据应保存的路径。如果未指定，则用户必须定义如何存储结果（例如创建一个新文件并命名为 ***.csv）。
-    - plot: 绘图标志，指示是否绘制处理后数据的图形。默认为 False，表示不生成图形，除非明确请求。
-    - window_size: 滑动窗口的大小，用于所选方法的滑动窗口大小。默认为 5。
-    - cutoff_frequency: 低通滤波器的截止频率，适用于选择了滤波方法的情况。默认为 0.1。
-    - sampling_rate: 数据的采样率，适用于某些处理方法。默认为 1.0。
-    - order: 滤波器的阶数或其他相关参数，适用于所选方法的滤波器的阶数或其他相关参数。默认为 5。
-    - cwt_row: 连续小波变换的行参数（如果适用）。默认为 1。
-    - time_step: 时间步长，表示数据的时间步长。默认为 1.0。
-    - iterations: 迭代次数，表示迭代的次数。默认为 3。
-    """
-    def __init__(self, file_path, column_id='ID', ID_list=None, column_flow='INQ', column_time='Time', start_time=None, end_time=None, preprocess=True, method='moving_average', save_path=None, plot=True, window_size=5, cutoff_frequency=0.1, time_step=1.0, iterations=3, sampling_rate=1.0, order=5, cwt_row=1):
-        self.file_path = file_path
-        self.column_id = column_id
-        self.ID_list = ID_list
-        self.column_flow = column_flow
-        self.column_time = column_time
-        self.start_time = start_time
-        self.end_time = end_time
-        self.preprocess = preprocess
-        self.method = method
-        self.save_path = save_path
-        self.plot = plot
-        self.window_size = window_size
-        self.cutoff_frequency = cutoff_frequency
-        self.sampling_rate = sampling_rate
-        self.order = order
-        self.cwt_row = cwt_row
-        self.time_step = time_step
-        self.iterations = iterations
-
-    def data_balanced(self, origin_data,transform_data):
-        """
-        对一维流量数据进行总量平衡变换。
-        :origin_data: 原始一维流量数据。
-        :transform_data: 平滑转换后的一维流量数据。
-        """
-        # Calculate the flow balance factor and keep the total volume consistent
-        streamflow_data_before = np.sum(origin_data)
-        streamflow_data_after = np.sum(transform_data)
-        scaling_factor = streamflow_data_before / streamflow_data_after
-        balanced_data = transform_data * scaling_factor
-
-        print(f"Total flow (before smoothing): {streamflow_data_before}")
-        print(f"Total flow (after smoothing): {np.sum(balanced_data)}")
-        return balanced_data
-
-    def moving_average(self, streamflow_data, window_size=20):
-        """
-        对流量数据应用滑动平均进行平滑处理，并保持流量总量平衡。
-        :window_size: 滑动窗口大小
-        :return: 平滑处理后的流量数据
-        """
-        smoothed_data = np.convolve(streamflow_data, np.ones(window_size)/window_size, mode='same')
-        
-        # Apply non-negative constraints
-        smoothed_data[smoothed_data < 0] = 0
-        return self.data_balanced(streamflow_data,smoothed_data)
-
-    def kalman_filter(self, streamflow_data):
-        """
-        对流量数据应用卡尔曼滤波进行平滑处理，并保持流量总量平衡。
-        :param streamflow_data: 原始流量数据
-        """
-        A = np.array([[1]])  
-        H = np.array([[1]])  
-        Q = np.array([[0.01]])  
-        R = np.array([[0.01]])  
-        X_estimated = np.array([streamflow_data[0]])  
-        P_estimated = np.eye(1) * 0.01  
-        estimated_states = []
-
-        for measurement in streamflow_data:
-            # predict
-            X_predicted = A.dot(X_estimated)
-            P_predicted = A.dot(P_estimated).dot(A.T) + Q
-
-            # update
-            measurement_residual = measurement - H.dot(X_predicted)
-            S = H.dot(P_predicted).dot(H.T) + R
-            K = P_predicted.dot(H.T).dot(np.linalg.inv(S))  # kalman gain
-            X_estimated = X_predicted + K.dot(measurement_residual)
-            P_estimated = P_predicted - K.dot(H).dot(P_predicted)
-            estimated_states.append(X_estimated.item())
-
-        estimated_states = np.array(estimated_states)
-        
-        # Apply non-negative constraints
-        estimated_states[estimated_states < 0] = 0
-        return self.data_balanced(streamflow_data,estimated_states)
-
-    def moving_average_difference(self, streamflow_data, window_size=20):
-        """
-        对流量数据应用滑动平均差算法进行平滑处理，并保持流量总量平衡。
-        :window_size: 滑动窗口的大小
-        """
-        streamflow_data_series = pd.Series(streamflow_data)
-        # Calculate the forward moving average（MU）
-        forward_ma = streamflow_data_series.rolling(window=window_size, min_periods=1).mean()
-
-        # Calculate the backward moving average（MD）
-        backward_ma = streamflow_data_series.iloc[::-1].rolling(window=window_size, min_periods=1).mean().iloc[::-1]
-
-        # Calculate the difference between the forward and backward sliding averages
-        ma_difference = abs(forward_ma - backward_ma)
-
-        # Apply non-negative constraints
-        ma_difference[ma_difference < 0] = 0
-        return self.data_balanced(streamflow_data,ma_difference.to_numpy())
-    
-
-    def quadratic_function(self, x, a, b, c):
-        return a * x**2 + b * x + c
-    def robust_fitting(self, streamflow_data, k=1.5):
-        """
-        对流量数据应用抗差修正算法进行平滑处理，并保持流量总量平衡。
-        默认采用二次曲线进行拟合优化，该算法处理性能较差
-        """
-        time_steps = np.arange(len(streamflow_data))
-        params, _ = curve_fit(self.quadratic_function, time_steps, streamflow_data)
-        smoothed_streamflow = self.quadratic_function(time_steps, *params)
-        residuals = streamflow_data - smoothed_streamflow
-        m = len(streamflow_data)
-        sigma = np.sqrt(np.sum(residuals**2) / (m - 1))
-
-        for _ in range(10):
-            weights = np.where(np.abs(residuals) <= k * sigma, 1, k * sigma / np.abs(residuals))
-            sigma = np.sqrt(np.sum(weights * residuals**2) / (m - 1))
-
-        corrected_streamflow = weights * streamflow_data + (1 - weights) * smoothed_streamflow
-        corrected_streamflow[corrected_streamflow < 0] = 0
-        return self.data_balanced(streamflow_data, corrected_streamflow)
-
-    def lowpass_filter(self, streamflow_data):
-        """
-        对一维流量数据应用调整后的低通滤波器。
-        :cutoff_frequency: 低通滤波器的截止频率。
-        :sampling_rate: 数据的采样率。
-        :order: 滤波器的阶数，默认为5。
-        """
-        def apply_low_pass_filter(signal, cutoff_frequency, sampling_rate, order=5):
-            nyquist_frequency = 0.5 * sampling_rate
-            normalized_cutoff = cutoff_frequency / nyquist_frequency
-            b, a = butter(order, normalized_cutoff, btype='low', analog=False)
-            filtered_signal = filtfilt(b, a, signal)
-            return filtered_signal
-        
-        # Apply a low-pass filter
-        low_pass_filtered_signal = apply_low_pass_filter(streamflow_data, self.cutoff_frequency, self.sampling_rate, self.order)
-        
-        # Apply non-negative constraints
-        low_pass_filtered_signal[low_pass_filtered_signal < 0] = 0
-
-        return self.data_balanced(streamflow_data, low_pass_filtered_signal)
-
-    def FFT(self, streamflow_data):
-        """
-        对流量数据进行迭代的傅里叶滤波处理，包括非负值调整和流量总量调整。
-        :cutoff_frequency: 傅里叶滤波的截止频率。
-        :time_step: 数据采样间隔。
-        :iterations: 迭代次数。
-        """
-        current_signal = streamflow_data.copy()
-
-        for _ in range(self.iterations):
-            n = len(current_signal)
-            yf = fft(current_signal)
-            xf = fftfreq(n, d=self.time_step)
-            
-            # Applied frequency filtering
-            yf[np.abs(xf) > self.cutoff_frequency] = 0
-            
-            # FFT and take the real part
-            filtered_signal = ifft(yf).real
-            
-            # Apply non-negative constraints
-            filtered_signal[filtered_signal < 0] = 0
-            
-            # Adjust the total flow to match the original flow
-            current_signal = self.data_balanced(streamflow_data, filtered_signal)
-
-        return current_signal
-
-    def wavelet(self, streamflow_data):
-        """
-        对一维流量数据进行小波变换分析前后拓展数据以减少边缘失真，然后调整总流量。
-        :cwt_row: 小波变换中使用的特定宽度。
-        """
-        # Expand the data edge by 24 lines on each side
-        extended_data = np.concatenate([
-            np.full(24, streamflow_data[0]),  # Expand the first 24 lines with the first element
-            streamflow_data,  
-            np.full(24, streamflow_data[-1])  # Expand the last 24 lines with the last element
-        ])
-        widths=np.arange(1, 31)
-        # Wavelet transform by Morlet wavelet directly
-        extended_cwt = cwt(extended_data, morlet, widths)
-        scaled_cwtmatr = np.abs(extended_cwt)
-        
-        # Select a specific width for analysis (can be briefly understood as selecting a cutoff frequency)
-        cwt_row_extended = scaled_cwtmatr[self.cwt_row, :]  
-        
-        # Remove the extended part
-        adjusted_cwt_row = cwt_row_extended[24:-24]  
-        adjusted_cwt_row[adjusted_cwt_row < 0] = 0
-        return self.data_balanced(streamflow_data, adjusted_cwt_row)
-
-
-    def streamflow_smooth(self, df):
-        #  Fill missing values as the average of the previous 10 hours
-        if self.preprocess:
-            df[self.column_flow] = df[self.column_flow].fillna(df[self.column_flow].rolling(window=11, min_periods=1).mean())
-            # Populate the part that is still NaN with a fill value of 0
-            df[self.column_flow] = df[self.column_flow].fillna(0)
-        #Record the generated data
-        df[self.column_time] = pd.to_datetime(df[self.column_time])
-
-        # Calibrate index range
-        start_idx = df.index[df[self.column_time] >= pd.to_datetime(self.start_time)].min()
-        end_idx = df.index[df[self.column_time] <= pd.to_datetime(self.end_time)].max()
-        
-        # Apply the selected method
-        # extract One-dimensional flow data
-        streamflow_data = df.loc[start_idx:end_idx, self.column_flow]
-        streamflow_data = streamflow_data.values.squeeze()
-        print(streamflow_data)
-
-        if self.method == 'moving_average':
-            filtered_data = self.moving_average(streamflow_data)
-        elif self.method == 'FFT':
-            filtered_data = self.FFT(streamflow_data)
-        elif self.method == 'wavelet':
-            filtered_data = self.wavelet(streamflow_data)
-        elif self.method == 'kalman':
-            filtered_data = self.kalman_filter(streamflow_data)
-        elif self.method == 'lowpass':
-            filtered_data = self.lowpass_filter(streamflow_data)
-        elif self.method == 'moving_average_difference':
-            filtered_data = self.moving_average_difference(streamflow_data)
-        elif self.method == 'robust':
-            filtered_data = self.robust_fitting(streamflow_data)   
-        else:
-            raise ValueError("Unsupported method")
-        
-        # Assume that filtered_data is the result of processing within the same start-stop time
-        # Insert processed data into the corresponding position in the original data set
-        df.loc[start_idx:end_idx, self.method +'_INQ_Filtered'] = filtered_data
-        
-        return df
-
-    def time_filter(self, df):
-        # filter by watershed number + start and end time
-        df[self.column_time] = pd.to_datetime(df[self.column_time])
-        # Filters data for a specified time range
-        min_time = df[self.column_time].min()
-        max_time = df[self.column_time].max()
-
-        # adjust start_time
-        if self.start_time is None or pd.to_datetime(self.start_time) < min_time:
-            self.start_time = min_time
-        else:
-            self.start_time = pd.to_datetime(self.start_time)
-
-        # adjust end_time
-        if self.end_time is None or pd.to_datetime(self.end_time) > max_time:
-            self.end_time = max_time
-        else:
-            self.end_time = pd.to_datetime(self.end_time)
-
-        # An empty DataFrame is returned If the adjusted start time is greater than the end time 
-        if self.start_time > self.end_time:
-            raise ValueError("Capture data time error")
-        return self.start_time, self.end_time
-
-    def drawplot(self, df, id):
-        df = df[(df[self.column_time] > self.start_time) & (df[self.column_time] < self.end_time)]
-        plt.figure(figsize=(10, 6))
-        plt.plot(df[self.column_time], df[self.column_flow], label='Original')
-        plt.plot(df[self.column_time], df[self.method +'_INQ_Filtered'], label='Filtered', linestyle='--')
-        plt.legend()
-        plt.xlabel('Time')
-        plt.ylabel('Flow')
-        if id:
-            plt.title(f"BASIN ID: {id} Streamflow Data Processing")
-        else:
-            plt.title(f"All Dataset Streamflow Data Processing")
-        plt.gcf().autofmt_xdate()  # Automatically rotate date markers to prevent overlapping
-        plt.grid(True)
-        plt.show()
-
-    def process_inq(self):
-        if self.file_path.endswith('.csv'):
-            df = pd.read_csv(self.file_path, dtype={self.column_id: str})    
-
-        elif self.file_path.endswith(('.nc', '.h5', '.netcdf')):
-            ds = xr.open_dataset(self.file_path)
-            # turn xarray into DataFrame
-            df = ds.to_dataframe()            
-
-        elif self.file_path.endswith('.txt'):
-            # Assuming .txt files are comma-delimited, if they are tab-delimited, use sep='\t'
-            df = pd.read_csv(self.file_path, sep=',', dtype={self.column_id: str})  
-
-        else:
-            raise ValueError("Unsupported file format")
-        
-        # data processing
-        print(df)
-        df = df.reset_index(drop=True)
-        original_df = df
-        df[self.column_flow] = pd.to_numeric(df[self.column_flow], errors='coerce')
-
-        # time_filter
-        df[self.column_time] = pd.to_datetime(df[self.column_time])
-        self.start_time, self.end_time = self.time_filter(df)
-
-        # add a new column and initialize as NaN if no exist
-        if (self.method + '_INQ_Filtered') not in df.columns:
-            df[self.method + '_INQ_Filtered'] = np.nan
-
-        # group by-basin  
-        if self.column_id is not None:  
-            grouped = df.groupby(self.column_id)
-            filtered_groups = []
-            for id, group in grouped:
-                try:
-                    if self.ID_list is None or str(id) in self.ID_list:
-                        print("当前处理数据为：")
-                        print(group)
-                        filtered_group = self.streamflow_smooth(group)
-                        filtered_groups.append(filtered_group)
-
-                        # Draw a comparison image of data processing
-                        if self.plot:
-                            self.drawplot(df=filtered_group, id=id)
-
-                except Exception as e:
-                    print(f"处理流域编号: {id} 的数据时发生错误: {e}")
-
-            # Merge the filtered grouped data into a new DataFrame
-            filtered_df = pd.concat(filtered_groups) 
-        else:
-            print("当前处理数据为整个数据集：")
-            print(df)  # print all DataFrame
-            filtered_df = self.streamflow_smooth(df)
-
-            # Draw a comparison image of data processing
-            if self.plot:
-                self.drawplot(df=filtered_df, id=None)
-
-        #save data
-        if self.save_path:
-            if self.file_path.endswith(('.nc', '.h5', '.netcdf')):
-                # the 'basin' column should be an eight-digit string
-                original_df[self.column_id] = original_df[self.column_id].astype(str).str.zfill(8)
-
-            original_df[self.method + '_INQ_Filtered'] = filtered_df[self.method + '_INQ_Filtered']
-            original_df.to_csv(self.save_path, index=False)
-        
-        return filtered_df
+import xarray as xr
+import pandas as pd
+import numpy as np
+import matplotlib.pyplot as plt
+from scipy.signal import cwt, morlet, butter, filtfilt
+from scipy.fft import fft, ifft, fftfreq
+from scipy.optimize import curve_fit
+
+
+class Cleaner:
+    """
+    参数中文说明如下：
+    - file_path (必选项): 文件路径，指定要处理的数据文件路径。支持.txt格式。
+    - column_id: ID 列名，用于标识数据中的不同组或实例。若不表明则默认全体数据为一个分组。
+    - ID_list: ID 列的值列表，指定要处理的特定 ID 列表。
+    - column_flow (必选项): 流量数据列名，在 DataFrame 中表示流量的列名。
+    - column_time (必选项): 时间数据列名，在 DataFrame 中表示时间的列名。
+    - start_time: 起始时间，指定要处理的数据时间范围的起始时间。
+    - end_time: 结束时间，指定要处理的数据时间范围的结束时间。
+    - preprocess: 数据预处理标志，指示是否进行数据预处理优化（如平滑缺失值）。默认为 True。
+    - method: 处理函数类型，要使用的特定处理函数类型。选项包括 'FFT'、'wavelet'、'kalman'、'moving_average'、'moving_average_difference'、'robust'、'lowpass'，默认为 'moving_average'。
+    - save_path: 保存路径，指定处理后数据应保存的路径。如果未指定，则用户必须定义如何存储结果（例如创建一个新文件并命名为 ***.csv）。
+    - plot: 绘图标志，指示是否绘制处理后数据的图形。默认为 False，表示不生成图形，除非明确请求。
+    - window_size: 滑动窗口的大小，用于所选方法的滑动窗口大小。默认为 5。
+    - cutoff_frequency: 低通滤波器的截止频率，适用于选择了滤波方法的情况。默认为 0.1。
+    - sampling_rate: 数据的采样率，适用于某些处理方法。默认为 1.0。
+    - order: 滤波器的阶数或其他相关参数，适用于所选方法的滤波器的阶数或其他相关参数。默认为 5。
+    - cwt_row: 连续小波变换的行参数（如果适用）。默认为 1。
+    - time_step: 时间步长，表示数据的时间步长。默认为 1.0。
+    - iterations: 迭代次数，表示迭代的次数。默认为 3。
+    """
+
+    def __init__(
+        self,
+        file_path,
+        column_id="ID",
+        ID_list=None,
+        column_flow="INQ",
+        column_time="Time",
+        start_time=None,
+        end_time=None,
+        preprocess=True,
+        method="moving_average",
+        save_path=None,
+        plot=True,
+        window_size=5,
+        cutoff_frequency=0.1,
+        time_step=1.0,
+        iterations=3,
+        sampling_rate=1.0,
+        order=5,
+        cwt_row=1,
+    ):
+        self.file_path = file_path
+        self.column_id = column_id
+        self.ID_list = ID_list
+        self.column_flow = column_flow
+        self.column_time = column_time
+        self.start_time = start_time
+        self.end_time = end_time
+        self.preprocess = preprocess
+        self.method = method
+        self.save_path = save_path
+        self.plot = plot
+        self.window_size = window_size
+        self.cutoff_frequency = cutoff_frequency
+        self.sampling_rate = sampling_rate
+        self.order = order
+        self.cwt_row = cwt_row
+        self.time_step = time_step
+        self.iterations = iterations
+
+    def data_balanced(self, origin_data, transform_data):
+        """
+        对一维流量数据进行总量平衡变换。
+        :origin_data: 原始一维流量数据。
+        :transform_data: 平滑转换后的一维流量数据。
+        """
+        # Calculate the flow balance factor and keep the total volume consistent
+        streamflow_data_before = np.sum(origin_data)
+        streamflow_data_after = np.sum(transform_data)
+        scaling_factor = streamflow_data_before / streamflow_data_after
+        balanced_data = transform_data * scaling_factor
+
+        print(f"Total flow (before smoothing): {streamflow_data_before}")
+        print(f"Total flow (after smoothing): {np.sum(balanced_data)}")
+        return balanced_data
+
+    def moving_average(self, streamflow_data, window_size=20):
+        """
+        对流量数据应用滑动平均进行平滑处理，并保持流量总量平衡。
+        :window_size: 滑动窗口大小
+        :return: 平滑处理后的流量数据
+        """
+        smoothed_data = np.convolve(
+            streamflow_data, np.ones(window_size) / window_size, mode="same"
+        )
+
+        # Apply non-negative constraints
+        smoothed_data[smoothed_data < 0] = 0
+        return self.data_balanced(streamflow_data, smoothed_data)
+
+    def kalman_filter(self, streamflow_data):
+        """
+        对流量数据应用卡尔曼滤波进行平滑处理，并保持流量总量平衡。
+        :param streamflow_data: 原始流量数据
+        """
+        A = np.array([[1]])
+        H = np.array([[1]])
+        Q = np.array([[0.01]])
+        R = np.array([[0.01]])
+        X_estimated = np.array([streamflow_data[0]])
+        P_estimated = np.eye(1) * 0.01
+        estimated_states = []
+
+        for measurement in streamflow_data:
+            # predict
+            X_predicted = A.dot(X_estimated)
+            P_predicted = A.dot(P_estimated).dot(A.T) + Q
+
+            # update
+            measurement_residual = measurement - H.dot(X_predicted)
+            S = H.dot(P_predicted).dot(H.T) + R
+            K = P_predicted.dot(H.T).dot(np.linalg.inv(S))  # kalman gain
+            X_estimated = X_predicted + K.dot(measurement_residual)
+            P_estimated = P_predicted - K.dot(H).dot(P_predicted)
+            estimated_states.append(X_estimated.item())
+
+        estimated_states = np.array(estimated_states)
+
+        # Apply non-negative constraints
+        estimated_states[estimated_states < 0] = 0
+        return self.data_balanced(streamflow_data, estimated_states)
+
+    def moving_average_difference(self, streamflow_data, window_size=20):
+        """
+        对流量数据应用滑动平均差算法进行平滑处理，并保持流量总量平衡。
+        :window_size: 滑动窗口的大小
+        """
+        streamflow_data_series = pd.Series(streamflow_data)
+        # Calculate the forward moving average（MU）
+        forward_ma = streamflow_data_series.rolling(
+            window=window_size, min_periods=1
+        ).mean()
+
+        # Calculate the backward moving average（MD）
+        backward_ma = (
+            streamflow_data_series.iloc[::-1]
+            .rolling(window=window_size, min_periods=1)
+            .mean()
+            .iloc[::-1]
+        )
+
+        # Calculate the difference between the forward and backward sliding averages
+        ma_difference = abs(forward_ma - backward_ma)
+
+        # Apply non-negative constraints
+        ma_difference[ma_difference < 0] = 0
+        return self.data_balanced(streamflow_data, ma_difference.to_numpy())
+
+    def quadratic_function(self, x, a, b, c):
+        return a * x**2 + b * x + c
+
+    def robust_fitting(self, streamflow_data, k=1.5):
+        """
+        对流量数据应用抗差修正算法进行平滑处理，并保持流量总量平衡。
+        默认采用二次曲线进行拟合优化，该算法处理性能较差
+        """
+        time_steps = np.arange(len(streamflow_data))
+        params, _ = curve_fit(self.quadratic_function, time_steps, streamflow_data)
+        smoothed_streamflow = self.quadratic_function(time_steps, *params)
+        residuals = streamflow_data - smoothed_streamflow
+        m = len(streamflow_data)
+        sigma = np.sqrt(np.sum(residuals**2) / (m - 1))
+
+        for _ in range(10):
+            weights = np.where(
+                np.abs(residuals) <= k * sigma, 1, k * sigma / np.abs(residuals)
+            )
+            sigma = np.sqrt(np.sum(weights * residuals**2) / (m - 1))
+
+        corrected_streamflow = (
+            weights * streamflow_data + (1 - weights) * smoothed_streamflow
+        )
+        corrected_streamflow[corrected_streamflow < 0] = 0
+        return self.data_balanced(streamflow_data, corrected_streamflow)
+
+    def lowpass_filter(self, streamflow_data):
+        """
+        对一维流量数据应用调整后的低通滤波器。
+        :cutoff_frequency: 低通滤波器的截止频率。
+        :sampling_rate: 数据的采样率。
+        :order: 滤波器的阶数，默认为5。
+        """
+
+        def apply_low_pass_filter(signal, cutoff_frequency, sampling_rate, order=5):
+            nyquist_frequency = 0.5 * sampling_rate
+            normalized_cutoff = cutoff_frequency / nyquist_frequency
+            b, a = butter(order, normalized_cutoff, btype="low", analog=False)
+            filtered_signal = filtfilt(b, a, signal)
+            return filtered_signal
+
+        # Apply a low-pass filter
+        low_pass_filtered_signal = apply_low_pass_filter(
+            streamflow_data, self.cutoff_frequency, self.sampling_rate, self.order
+        )
+
+        # Apply non-negative constraints
+        low_pass_filtered_signal[low_pass_filtered_signal < 0] = 0
+
+        return self.data_balanced(streamflow_data, low_pass_filtered_signal)
+
+    def FFT(self, streamflow_data):
+        """
+        对流量数据进行迭代的傅里叶滤波处理，包括非负值调整和流量总量调整。
+        :cutoff_frequency: 傅里叶滤波的截止频率。
+        :time_step: 数据采样间隔。
+        :iterations: 迭代次数。
+        """
+        current_signal = streamflow_data.copy()
+
+        for _ in range(self.iterations):
+            n = len(current_signal)
+            yf = fft(current_signal)
+            xf = fftfreq(n, d=self.time_step)
+
+            # Applied frequency filtering
+            yf[np.abs(xf) > self.cutoff_frequency] = 0
+
+            # FFT and take the real part
+            filtered_signal = ifft(yf).real
+
+            # Apply non-negative constraints
+            filtered_signal[filtered_signal < 0] = 0
+
+            # Adjust the total flow to match the original flow
+            current_signal = self.data_balanced(streamflow_data, filtered_signal)
+
+        return current_signal
+
+    def wavelet(self, streamflow_data):
+        """
+        对一维流量数据进行小波变换分析前后拓展数据以减少边缘失真，然后调整总流量。
+        :cwt_row: 小波变换中使用的特定宽度。
+        """
+        # Expand the data edge by 24 lines on each side
+        extended_data = np.concatenate(
+            [
+                np.full(
+                    24, streamflow_data[0]
+                ),  # Expand the first 24 lines with the first element
+                streamflow_data,
+                np.full(
+                    24, streamflow_data[-1]
+                ),  # Expand the last 24 lines with the last element
+            ]
+        )
+        widths = np.arange(1, 31)
+        # Wavelet transform by Morlet wavelet directly
+        extended_cwt = cwt(extended_data, morlet, widths)
+        scaled_cwtmatr = np.abs(extended_cwt)
+
+        # Select a specific width for analysis (can be briefly understood as selecting a cutoff frequency)
+        cwt_row_extended = scaled_cwtmatr[self.cwt_row, :]
+
+        # Remove the extended part
+        adjusted_cwt_row = cwt_row_extended[24:-24]
+        adjusted_cwt_row[adjusted_cwt_row < 0] = 0
+        return self.data_balanced(streamflow_data, adjusted_cwt_row)
+
+    def streamflow_smooth(self, df):
+        #  Fill missing values as the average of the previous 10 hours
+        if self.preprocess:
+            df[self.column_flow] = df[self.column_flow].fillna(
+                df[self.column_flow].rolling(window=11, min_periods=1).mean()
+            )
+            # Populate the part that is still NaN with a fill value of 0
+            df[self.column_flow] = df[self.column_flow].fillna(0)
+        # Record the generated data
+        df[self.column_time] = pd.to_datetime(df[self.column_time])
+
+        # Calibrate index range
+        start_idx = df.index[
+            df[self.column_time] >= pd.to_datetime(self.start_time)
+        ].min()
+        end_idx = df.index[df[self.column_time] <= pd.to_datetime(self.end_time)].max()
+
+        # Apply the selected method
+        # extract One-dimensional flow data
+        streamflow_data = df.loc[start_idx:end_idx, self.column_flow]
+        streamflow_data = streamflow_data.values.squeeze()
+        print(streamflow_data)
+
+        if self.method == "moving_average":
+            filtered_data = self.moving_average(streamflow_data)
+        elif self.method == "FFT":
+            filtered_data = self.FFT(streamflow_data)
+        elif self.method == "wavelet":
+            filtered_data = self.wavelet(streamflow_data)
+        elif self.method == "kalman":
+            filtered_data = self.kalman_filter(streamflow_data)
+        elif self.method == "lowpass":
+            filtered_data = self.lowpass_filter(streamflow_data)
+        elif self.method == "moving_average_difference":
+            filtered_data = self.moving_average_difference(streamflow_data)
+        elif self.method == "robust":
+            filtered_data = self.robust_fitting(streamflow_data)
+        else:
+            raise ValueError("Unsupported method")
+
+        # Assume that filtered_data is the result of processing within the same start-stop time
+        # Insert processed data into the corresponding position in the original data set
+        df.loc[start_idx:end_idx, self.method + "_INQ_Filtered"] = filtered_data
+
+        return df
+
+    def time_filter(self, df):
+        # filter by watershed number + start and end time
+        df[self.column_time] = pd.to_datetime(df[self.column_time])
+        # Filters data for a specified time range
+        min_time = df[self.column_time].min()
+        max_time = df[self.column_time].max()
+
+        # adjust start_time
+        if self.start_time is None or pd.to_datetime(self.start_time) < min_time:
+            self.start_time = min_time
+        else:
+            self.start_time = pd.to_datetime(self.start_time)
+
+        # adjust end_time
+        if self.end_time is None or pd.to_datetime(self.end_time) > max_time:
+            self.end_time = max_time
+        else:
+            self.end_time = pd.to_datetime(self.end_time)
+
+        # An empty DataFrame is returned If the adjusted start time is greater than the end time
+        if self.start_time > self.end_time:
+            raise ValueError("Capture data time error")
+        return self.start_time, self.end_time
+
+    def drawplot(self, df, id):
+        df = df[
+            (df[self.column_time] > self.start_time)
+            & (df[self.column_time] < self.end_time)
+        ]
+        plt.figure(figsize=(10, 6))
+        plt.plot(df[self.column_time], df[self.column_flow], label="Original")
+        plt.plot(
+            df[self.column_time],
+            df[self.method + "_INQ_Filtered"],
+            label="Filtered",
+            linestyle="--",
+        )
+        plt.legend()
+        plt.xlabel("Time")
+        plt.ylabel("Flow")
+        if id:
+            plt.title(f"BASIN ID: {id} Streamflow Data Processing")
+        else:
+            plt.title("All Dataset Streamflow Data Processing")
+        plt.gcf().autofmt_xdate()  # Automatically rotate date markers to prevent overlapping
+        plt.grid(True)
+        plt.show()
+
+    def process_inq(self):
+        if self.file_path.endswith(".csv"):
+            df = pd.read_csv(self.file_path, dtype={self.column_id: str})
+
+        elif self.file_path.endswith((".nc", ".h5", ".netcdf")):
+            ds = xr.open_dataset(self.file_path)
+            # turn xarray into DataFrame
+            df = ds.to_dataframe()
+
+        elif self.file_path.endswith(".txt"):
+            # Assuming .txt files are comma-delimited, if they are tab-delimited, use sep='\t'
+            df = pd.read_csv(self.file_path, sep=",", dtype={self.column_id: str})
+
+        else:
+            raise ValueError("Unsupported file format")
+
+        # data processing
+        print(df)
+        df = df.reset_index(drop=True)
+        original_df = df
+        df[self.column_flow] = pd.to_numeric(df[self.column_flow], errors="coerce")
+
+        # time_filter
+        df[self.column_time] = pd.to_datetime(df[self.column_time])
+        self.start_time, self.end_time = self.time_filter(df)
+
+        # add a new column and initialize as NaN if no exist
+        if (self.method + "_INQ_Filtered") not in df.columns:
+            df[self.method + "_INQ_Filtered"] = np.nan
+
+        # group by-basin
+        if self.column_id is not None:
+            grouped = df.groupby(self.column_id)
+            filtered_groups = []
+            for id, group in grouped:
+                try:
+                    if self.ID_list is None or str(id) in self.ID_list:
+                        print("当前处理数据为：")
+                        print(group)
+                        filtered_group = self.streamflow_smooth(group)
+                        filtered_groups.append(filtered_group)
+
+                        # Draw a comparison image of data processing
+                        if self.plot:
+                            self.drawplot(df=filtered_group, id=id)
+
+                except Exception as e:
+                    print(f"处理流域编号: {id} 的数据时发生错误: {e}")
+
+            # Merge the filtered grouped data into a new DataFrame
+            filtered_df = pd.concat(filtered_groups)
+        else:
+            print("当前处理数据为整个数据集：")
+            print(df)  # print all DataFrame
+            filtered_df = self.streamflow_smooth(df)
+
+            # Draw a comparison image of data processing
+            if self.plot:
+                self.drawplot(df=filtered_df, id=None)
+
+        # save data
+        if self.save_path:
+            if self.file_path.endswith((".nc", ".h5", ".netcdf")):
+                # the 'basin' column should be an eight-digit string
+                original_df[self.column_id] = (
+                    original_df[self.column_id].astype(str).str.zfill(8)
+                )
+
+            original_df[self.method + "_INQ_Filtered"] = filtered_df[
+                self.method + "_INQ_Filtered"
+            ]
+            original_df.to_csv(self.save_path, index=False)
+
+        return filtered_df
```

### Comparing `hydrodatasource-0.0.1/hydrodatasource/configs/config.py` & `hydrodatasource-0.0.2/hydrodatasource/configs/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,116 +1,131 @@
-"""
-Author: Jianfeng Zhu
-Date: 2023-10-25 18:49:02
-LastEditTime: 2024-02-15 21:08:19
-LastEditors: Wenyu Ouyang
-Description: Some configs for minio server
-FilePath: \hydrodata\hydrodata\configs\config.py
-Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
-"""
-
-import os
-from pathlib import Path
-import boto3
-import s3fs
-import yaml
-from minio import Minio
-
-
-def read_setting(setting_path):
-    if not os.path.exists(setting_path):
-        raise FileNotFoundError(f"Configuration file not found: {setting_path}")
-
-    with open(setting_path, "r") as file:
-        setting = yaml.safe_load(file)
-
-    example_setting = (
-        "minio:\n"
-        "  server_url: 'http://minio.waterism.com:9090' # Update with your URL\n"
-        "  client_endpoint: 'http://minio.waterism.com:9000' # Update with your URL\n"
-        "  access_key: 'your minio access key'\n"
-        "  secret: 'your minio secret'\n\n"
-        "local_data_path:\n"
-        "  root: 'D:\\data\\waterism' # Update with your root data directory\n"
-        "  datasets-origin: 'D:\\data\\waterism\\datasets-origin'\n"
-        "  datasets-interim: 'D:\\data\\waterism\\datasets-interim'"
-    )
-
-    if setting is None:
-        raise ValueError(
-            f"Configuration file is empty or has invalid format.\n\nExample configuration:\n{example_setting}"
-        )
-
-    # Define the expected structure
-    expected_structure = {
-        "minio": ["server_url", "client_endpoint", "access_key", "secret"],
-        "local_data_path": ["root", "datasets-origin", "datasets-interim"],
-    }
-
-    # Validate the structure
-    try:
-        for key, subkeys in expected_structure.items():
-            if key not in setting:
-                raise KeyError(f"Missing required key in config: {key}")
-
-            if isinstance(subkeys, list):
-                for subkey in subkeys:
-                    if subkey not in setting[key]:
-                        raise KeyError(f"Missing required subkey '{subkey}' in '{key}'")
-    except KeyError as e:
-        raise ValueError(
-            f"Incorrect configuration format: {e}\n\nExample configuration:\n{example_setting}"
-        ) from e
-
-    return setting
-
-
-SETTING_FILE = os.path.join(Path.home(), "hydro_setting.yml")
-SETTING = {}
-try:
-    SETTING = read_setting(SETTING_FILE)
-except ValueError as e:
-    print(e)
-except Exception as e:
-    print(f"Unexpected error: {e}")
-
-LOCAL_DATA_PATH = SETTING["local_data_path"]["root"]
-
-MINIO_PARAM = {
-    "endpoint_url": SETTING["minio"]["client_endpoint"],
-    "key": SETTING["minio"]["access_key"],
-    "secret": SETTING["minio"]["secret"],
-}
-
-FS = s3fs.S3FileSystem(
-    client_kwargs={"endpoint_url": MINIO_PARAM["endpoint_url"]},
-    key=MINIO_PARAM["key"],
-    secret=MINIO_PARAM["secret"],
-    use_ssl=False,
-)
-
-# remote_options parameters for xr open_dataset from minio
-RO = {
-    "client_kwargs": {"endpoint_url": MINIO_PARAM["endpoint_url"]},
-    "key": MINIO_PARAM["key"],
-    "secret": MINIO_PARAM["secret"],
-    "use_ssl": False,
-}
-
-
-# Set up MinIO client
-S3 = boto3.client(
-    "s3",
-    endpoint_url=SETTING["minio"]["server_url"],
-    aws_access_key_id=MINIO_PARAM["key"],
-    aws_secret_access_key=MINIO_PARAM["secret"],
-)
-MC = Minio(
-    SETTING["minio"]["server_url"].replace("http://", ""),
-    access_key=MINIO_PARAM["key"],
-    secret_key=MINIO_PARAM["secret"],
-    secure=False,  # True if using HTTPS
-)
-STATION_BUCKET = "stations"
-STATION_OBJECT = "sites.csv"
-
-GRID_INTERIM_BUCKET = "grids-interim"
+"""
+Author: Jianfeng Zhu
+Date: 2023-10-25 18:49:02
+LastEditTime: 2024-02-15 21:08:19
+LastEditors: Wenyu Ouyang
+Description: Some configs for minio server
+FilePath: \hydrodata\hydrodata\configs\config.py
+Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
+"""
+
+import os
+from pathlib import Path
+import boto3
+import s3fs
+import yaml
+from minio import Minio
+import psycopg2
+
+
+def read_setting(setting_path):
+    if not os.path.exists(setting_path):
+        raise FileNotFoundError(f"Configuration file not found: {setting_path}")
+
+    with open(setting_path, 'r', encoding='utf-8') as file:  # 指定编码为 UTF-8
+        setting = yaml.safe_load(file)
+
+    example_setting = (
+        "minio:\n"
+        "  server_url: 'http://minio.waterism.com:9090' # Update with your URL\n"
+        "  client_endpoint: 'http://minio.waterism.com:9000' # Update with your URL\n"
+        "  access_key: 'your minio access key'\n"
+        "  secret: 'your minio secret'\n\n"
+        "local_data_path:\n"
+        "  root: 'D:\\data\\waterism' # Update with your root data directory\n"
+        "  datasets-origin: 'D:\\data\\waterism\\datasets-origin'\n"
+        "  datasets-interim: 'D:\\data\\waterism\\datasets-interim'\n"
+        "postgres:\n"
+        "  server_url: your_postgres_server_url\n"
+        "  port: 5432\n"
+        "  username: your_postgres_username\n"
+        "  password: your_postgres_secret_code\n"
+        "  database: your_postgres_database\n"
+        )
+
+    if setting is None:
+        raise ValueError(
+            f"Configuration file is empty or has invalid format.\n\nExample configuration:\n{example_setting}"
+        )
+
+    # Define the expected structure
+    expected_structure = {
+        "minio": ["server_url", "client_endpoint", "access_key", "secret"],
+        "local_data_path": ["root", "datasets-origin", "datasets-interim"],
+        "postgres":["server_url", "port", "username", "password", "database"]
+    }
+
+    # Validate the structure
+    try:
+        for key, subkeys in expected_structure.items():
+            if key not in setting:
+                raise KeyError(f"Missing required key in config: {key}")
+
+            if isinstance(subkeys, list):
+                for subkey in subkeys:
+                    if subkey not in setting[key]:
+                        raise KeyError(f"Missing required subkey '{subkey}' in '{key}'")
+    except KeyError as e:
+        raise ValueError(
+            f"Incorrect configuration format: {e}\n\nExample configuration:\n{example_setting}"
+        ) from e
+
+    return setting
+
+
+SETTING_FILE = os.path.join(Path.home(), "hydro_setting.yml")
+try:
+    SETTING = read_setting(SETTING_FILE)
+except ValueError as e:
+    print(e)
+except Exception as e:
+    print(f"Unexpected error: {e}")
+
+LOCAL_DATA_PATH = SETTING["local_data_path"]["root"]
+
+MINIO_PARAM = {
+    "endpoint_url": SETTING["minio"]["client_endpoint"],
+    "key": SETTING["minio"]["access_key"],
+    "secret": SETTING["minio"]["secret"],
+}
+
+FS = s3fs.S3FileSystem(
+    client_kwargs={"endpoint_url": MINIO_PARAM["endpoint_url"]},
+    key=MINIO_PARAM["key"],
+    secret=MINIO_PARAM["secret"],
+    use_ssl=False,
+)
+
+# remote_options parameters for xr open_dataset from minio
+RO = {
+    "client_kwargs": {"endpoint_url": MINIO_PARAM["endpoint_url"]},
+    "key": MINIO_PARAM["key"],
+    "secret": MINIO_PARAM["secret"],
+    "use_ssl": False,
+}
+
+
+# Set up MinIO client
+S3 = boto3.client(
+    "s3",
+    endpoint_url=SETTING["minio"]["client_endpoint"],
+    aws_access_key_id=MINIO_PARAM["key"],
+    aws_secret_access_key=MINIO_PARAM["secret"],
+)
+MC = Minio(
+    SETTING["minio"]["client_endpoint"].replace("http://", ""),
+    access_key=MINIO_PARAM["key"],
+    secret_key=MINIO_PARAM["secret"],
+    secure=False,  # True if using HTTPS
+)
+STATION_BUCKET = "stations"
+STATION_OBJECT = "sites.csv"
+
+GRID_INTERIM_BUCKET = "grids-interim"
+
+PS = psycopg2.connect(
+    database=SETTING["postgres"]["database"],
+    user=SETTING["postgres"]["username"],
+    password=SETTING["postgres"]["password"],
+    host=SETTING["postgres"]["server_url"],
+    port=SETTING["postgres"]["port"],
+)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hydrodatasource-0.0.1/hydrodatasource/downloader/downloader.py` & `hydrodatasource-0.0.2/hydrodatasource/downloader/downloader.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,198 +1,198 @@
-"""
-Author: Jianfeng Zhu
-Date: 2023-10-06 20:50:41
-LastEditTime: 2023-10-14 11:50:48
-LastEditors: Wenyu Ouyang
-Description: 该模块用于下载，通常是url链接或执行命令：`download_from_url` - 通过url链接下载文件；`download_by_stream` - 通过stream方式下载url链接；`download_singletasking` - 单函数线程下载文件，显示进度条
-FilePath: /hydrodata/hydrodata/downloader/downloader.py
-Copyright (c) 2023-2024 Jianfeng Zhu. All rights reserved.
-"""
-import requests
-from tqdm import tqdm
-from zipfile import ZipFile
-
-import wget
-
-from ftplib import FTP
-import os
-
-
-def download_ftp_file(ftp_url, path=None, retries=3):
-    # Parse the FTP URL
-    url_parts = ftp_url.replace("ftp://", "").split("/")
-    host = url_parts[0]
-    file_path = "/".join(url_parts[1:])
-    remote_filename = url_parts[-1]
-
-    # If path is a directory, specify the filename to save the downloaded file
-    if path and os.path.isdir(path):
-        path = os.path.join(path, remote_filename)
-
-    # Connect to the FTP server
-    ftp = FTP(host)
-    ftp.login()
-
-    # Get remote file size
-    remote_file_size = ftp.size(file_path)
-
-    # Check if the file already exists at the specified path and has the same size as the remote file
-    if path and os.path.exists(path) and os.path.getsize(path) == remote_file_size:
-        return path
-
-    # Download the file
-    for _ in range(retries):
-        with open(path, "wb") as local_file:
-            ftp.retrbinary(f"RETR {file_path}", local_file.write)
-
-        # Verify the downloaded file size
-        if os.path.getsize(path) == remote_file_size:
-            return path
-
-    raise ValueError(
-        "Failed to download the file after multiple attempts. The file might be corrupted or incomplete."
-    )
-
-
-def wget_download(url, save_path=None):
-    """
-    Downloads a file using wget.
-
-    Parameters:
-    - url (str): The URL of the file to be downloaded.
-    - save_path (str, optional): dir or file to save (default: current working directory).
-
-    Returns:
-    - str: The path to the downloaded file.
-    """
-    if save_path and os.path.isdir(save_path):
-        output_filename = os.path.join(save_path, os.path.basename(url))
-    elif save_path:
-        output_filename = save_path
-    else:
-        output_filename = os.path.basename(url)
-
-    # Check if the file already exists
-    if os.path.exists(output_filename):
-        print(f"File {output_filename} already exists. Skipping download.")
-        return output_filename
-
-    return wget.download(url, out=output_filename)
-
-
-def unzip_file(zip_path, output_folder=None):
-    """
-    Unzips a ZIP file.
-
-    Parameters:
-    - zip_path (str): The path to the ZIP file.
-    - output_folder (str, optional): The folder where the ZIP file should be extracted to.
-                                     Defaults to a folder named after the ZIP file in the ZIP file's directory.
-
-    Returns:
-    - str: The path to the extracted folder.
-    """
-    if not output_folder:
-        output_folder = os.path.join(
-            os.path.dirname(zip_path), os.path.splitext(os.path.basename(zip_path))[0]
-        )
-
-    # Check if the output folder already exists
-    if not os.path.exists(output_folder):
-        with ZipFile(zip_path, "r") as zip_ref:
-            zip_ref.extractall(output_folder)
-    else:
-        print(f"Files already extracted to {output_folder}. Skipping extraction.")
-
-    return output_folder
-
-
-def download_from_url(url, file_name):
-    """
-    通过url链接下载文件的一般方法
-
-    Args:
-        url (str): url链接
-        file_name (str): 文件的本地存储地址
-
-    """
-    f = requests.get(url)
-    with open(file_name, "wb") as tiff:
-        tiff.write(f.content)
-    f.close()
-
-
-def download_by_stream(url, file_name):
-    """
-    通过stream下载url链接文件
-
-    Args:
-        url (str): url链接
-        file_name (str): 文件的本地存储地址
-
-    """
-
-    headers = {
-        "User-Agent": "Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Safari/537.36 QIHU 360SE"
-    }
-
-    # 发起 head 请求，即只会获取响应头部信息
-    head = requests.head(url, headers=headers)
-
-    if head.status_code == 404:
-        print("404 not found.")
-    elif head.status_code == 200:
-        response = requests.get(url, headers=headers, stream=True)
-        with open(file_name, mode="wb") as f:
-            # 写入分块文件
-            for i, chunk in enumerate(response.iter_content(chunk_size=1024), start=1):
-                f.write(chunk)
-                print("\r", "已下载：%.2f MB" % (i / 1024), end="", flush=True)
-
-            print(f"{file_name}下载完成。")
-
-
-def download_sigletasking(url: str, file_name: str):
-    """
-    单函数线程下载文件，显示进度条
-
-    Args:
-        url (str): 文件链接
-        file_name (str): 文件名或文件路径
-
-    """
-    # 文件下载直链
-    # 请求头
-    headers = {
-        "User-Agent": "Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Safari/537.36 QIHU 360SE"
-    }
-
-    # 发起 head 请求，即只会获取响应头部信息
-    head = requests.head(url, headers=headers)
-
-    if head.status_code == 404:
-        print("404 not found.")
-    elif head.status_code == 200:
-        # 文件大小，以 B 为单位
-        file_size = head.headers.get("Content-Length")
-        if file_size is not None:
-            download_single_task_with_chunks(file_size, url, headers, file_name)
-        else:
-            # 未获取到文件大小，采用stream方法下载
-            # download_from_url(url,file_name)
-            download_by_stream(url, file_name)
-
-
-def download_single_task_with_chunks(file_size, url, headers, file_name):
-    file_size = int(file_size)
-    response = requests.get(url, headers=headers, stream=True)
-    # 一块文件的大小
-    # chunk_size = 1024
-    chunk_size = file_size // 100 + 1
-    bar = tqdm(total=file_size, desc=f"下载文件 {file_name}")
-    with open(file_name, mode="wb") as f:
-        # 写入分块文件
-        for chunk in response.iter_content(chunk_size=chunk_size):
-            f.write(chunk)
-            bar.update(chunk_size)
-    # 关闭进度条
-    bar.close()
+"""
+Author: Jianfeng Zhu
+Date: 2023-10-06 20:50:41
+LastEditTime: 2023-10-14 11:50:48
+LastEditors: Wenyu Ouyang
+Description: 该模块用于下载，通常是url链接或执行命令：`download_from_url` - 通过url链接下载文件；`download_by_stream` - 通过stream方式下载url链接；`download_singletasking` - 单函数线程下载文件，显示进度条
+FilePath: /hydrodata/hydrodata/downloader/downloader.py
+Copyright (c) 2023-2024 Jianfeng Zhu. All rights reserved.
+"""
+import requests
+from tqdm import tqdm
+from zipfile import ZipFile
+
+import wget
+
+from ftplib import FTP
+import os
+
+
+def download_ftp_file(ftp_url, path=None, retries=3):
+    # Parse the FTP URL
+    url_parts = ftp_url.replace("ftp://", "").split("/")
+    host = url_parts[0]
+    file_path = "/".join(url_parts[1:])
+    remote_filename = url_parts[-1]
+
+    # If path is a directory, specify the filename to save the downloaded file
+    if path and os.path.isdir(path):
+        path = os.path.join(path, remote_filename)
+
+    # Connect to the FTP server
+    ftp = FTP(host)
+    ftp.login()
+
+    # Get remote file size
+    remote_file_size = ftp.size(file_path)
+
+    # Check if the file already exists at the specified path and has the same size as the remote file
+    if path and os.path.exists(path) and os.path.getsize(path) == remote_file_size:
+        return path
+
+    # Download the file
+    for _ in range(retries):
+        with open(path, "wb") as local_file:
+            ftp.retrbinary(f"RETR {file_path}", local_file.write)
+
+        # Verify the downloaded file size
+        if os.path.getsize(path) == remote_file_size:
+            return path
+
+    raise ValueError(
+        "Failed to download the file after multiple attempts. The file might be corrupted or incomplete."
+    )
+
+
+def wget_download(url, save_path=None):
+    """
+    Downloads a file using wget.
+
+    Parameters:
+    - url (str): The URL of the file to be downloaded.
+    - save_path (str, optional): dir or file to save (default: current working directory).
+
+    Returns:
+    - str: The path to the downloaded file.
+    """
+    if save_path and os.path.isdir(save_path):
+        output_filename = os.path.join(save_path, os.path.basename(url))
+    elif save_path:
+        output_filename = save_path
+    else:
+        output_filename = os.path.basename(url)
+
+    # Check if the file already exists
+    if os.path.exists(output_filename):
+        print(f"File {output_filename} already exists. Skipping download.")
+        return output_filename
+
+    return wget.download(url, out=output_filename)
+
+
+def unzip_file(zip_path, output_folder=None):
+    """
+    Unzips a ZIP file.
+
+    Parameters:
+    - zip_path (str): The path to the ZIP file.
+    - output_folder (str, optional): The folder where the ZIP file should be extracted to.
+                                     Defaults to a folder named after the ZIP file in the ZIP file's directory.
+
+    Returns:
+    - str: The path to the extracted folder.
+    """
+    if not output_folder:
+        output_folder = os.path.join(
+            os.path.dirname(zip_path), os.path.splitext(os.path.basename(zip_path))[0]
+        )
+
+    # Check if the output folder already exists
+    if not os.path.exists(output_folder):
+        with ZipFile(zip_path, "r") as zip_ref:
+            zip_ref.extractall(output_folder)
+    else:
+        print(f"Files already extracted to {output_folder}. Skipping extraction.")
+
+    return output_folder
+
+
+def download_from_url(url, file_name):
+    """
+    通过url链接下载文件的一般方法
+
+    Args:
+        url (str): url链接
+        file_name (str): 文件的本地存储地址
+
+    """
+    f = requests.get(url)
+    with open(file_name, "wb") as tiff:
+        tiff.write(f.content)
+    f.close()
+
+
+def download_by_stream(url, file_name):
+    """
+    通过stream下载url链接文件
+
+    Args:
+        url (str): url链接
+        file_name (str): 文件的本地存储地址
+
+    """
+
+    headers = {
+        "User-Agent": "Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Safari/537.36 QIHU 360SE"
+    }
+
+    # 发起 head 请求，即只会获取响应头部信息
+    head = requests.head(url, headers=headers)
+
+    if head.status_code == 404:
+        print("404 not found.")
+    elif head.status_code == 200:
+        response = requests.get(url, headers=headers, stream=True)
+        with open(file_name, mode="wb") as f:
+            # 写入分块文件
+            for i, chunk in enumerate(response.iter_content(chunk_size=1024), start=1):
+                f.write(chunk)
+                print("\r", "已下载：%.2f MB" % (i / 1024), end="", flush=True)
+
+            print(f"{file_name}下载完成。")
+
+
+def download_sigletasking(url: str, file_name: str):
+    """
+    单函数线程下载文件，显示进度条
+
+    Args:
+        url (str): 文件链接
+        file_name (str): 文件名或文件路径
+
+    """
+    # 文件下载直链
+    # 请求头
+    headers = {
+        "User-Agent": "Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Safari/537.36 QIHU 360SE"
+    }
+
+    # 发起 head 请求，即只会获取响应头部信息
+    head = requests.head(url, headers=headers)
+
+    if head.status_code == 404:
+        print("404 not found.")
+    elif head.status_code == 200:
+        # 文件大小，以 B 为单位
+        file_size = head.headers.get("Content-Length")
+        if file_size is not None:
+            download_single_task_with_chunks(file_size, url, headers, file_name)
+        else:
+            # 未获取到文件大小，采用stream方法下载
+            # download_from_url(url,file_name)
+            download_by_stream(url, file_name)
+
+
+def download_single_task_with_chunks(file_size, url, headers, file_name):
+    file_size = int(file_size)
+    response = requests.get(url, headers=headers, stream=True)
+    # 一块文件的大小
+    # chunk_size = 1024
+    chunk_size = file_size // 100 + 1
+    bar = tqdm(total=file_size, desc=f"下载文件 {file_name}")
+    with open(file_name, mode="wb") as f:
+        # 写入分块文件
+        for chunk in response.iter_content(chunk_size=chunk_size):
+            f.write(chunk)
+            bar.update(chunk_size)
+    # 关闭进度条
+    bar.close()
```

### Comparing `hydrodatasource-0.0.1/hydrodatasource/downloader/gfs_config_dict.py` & `hydrodatasource-0.0.2/hydrodatasource/downloader/gfs_config_dict.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,186 +1,186 @@
-# https://nomads.ncep.noaa.gov/gribfilter.php?ds=gfs_0p25_1hr
-gfs_parameters_dict = {
-    'var_4LFTX': 'off',
-    'var_ABSV': 'off',
-    'var_ACPCP': 'off',
-    'var_ALBDO': 'off',
-    'var_APCP': 'off',
-    'var_CAPE': 'off',
-    'var_CFRZR': 'off',
-    'var_CICEP': 'off',
-    'var_CIN': 'off',
-    'var_CLWMR': 'off',
-    'var_CNWAT': 'off',
-    'var_CPOFP': 'off',
-    'var_CPRAT': 'off',
-    'var_CRAIN': 'off',
-    'var_CSNOW': 'off',
-    'var_CWAT': 'off',
-    'var_CWORK': 'off',
-    'var_DLWRF': 'off',
-    'var_DPT': 'off',
-    'var_DSWRF': 'off',
-    'var_DZDT': 'off',
-    'var_FLDCP': 'off',
-    'var_FRICV': 'off',
-    'var_GFLUX': 'off',
-    'var_GRLEV': 'off',
-    'var_GUST': 'off',
-    'var_HCDC': 'off',
-    'var_HGT': 'off',
-    'var_HINDEX': 'off',
-    'var_HLCY': 'off',
-    'var_HPBL': 'off',
-    'var_ICAHT': 'off',
-    'var_ICEC': 'off',
-    'var_ICEG': 'off',
-    'var_ICETK': 'off',
-    'var_ICETMP': 'off',
-    'var_ICMR': 'off',
-    'var_LAND': 'off',
-    'var_LCDC': 'off',
-    'var_LFTX': 'off',
-    'var_LHTFL': 'off',
-    'var_MCDC': 'off',
-    'var_MSLET': 'off',
-    'var_O3MR': 'off',
-    'var_PEVFR': 'off',
-    'var_PLPL': 'off',
-    'var_POT': 'off',
-    'var_PRATE': 'off',
-    'var_PRES': 'off',
-    'var_PRMSL': 'off',
-    'var_PWAT': 'off',
-    'var_REFC': 'off',
-    'var_REFD': 'off',
-    'var_RH': 'off',
-    'var_RWMR': 'off',
-    'var_SFCR': 'off',
-    'var_SHTFL': 'off',
-    'var_SNMR': 'off',
-    'var_SNOD': 'off',
-    'var_SOILL': 'off',
-    'var_SOILW': 'off',
-    'var_SOTYP': 'off',
-    'var_SPFH': 'off',
-    'var_SUNSD': 'off',
-    'var_TCDC': 'off',
-    'var_TMAX': 'off',
-    'var_TMIN': 'off',
-    'var_TMP': 'off',
-    'var_TOZNE': 'off',
-    'var_TSOIL': 'off',
-    'var_UFLX': 'off',
-    'var_UGRD': 'off',
-    'var_U-GWD': 'off',
-    'var_ULWRF': 'off',
-    'var_USTM': 'off',
-    'var_USWRF': 'off',
-    'var_VEG': 'off',
-    'var_VFLX': 'off',
-    'var_VGRD': 'off',
-    'var_V-GWD': 'off',
-    'var_VIS': 'off',
-    'var_VRATE': 'off',
-    'var_VSTM': 'off',
-    'var_VVEL': 'off',
-    'var_VWSH': 'off',
-    'var_WATR': 'off',
-    'var_WEASD': 'off',
-    'var_WILT': 'off',
-}
-
-gfs_levels_dict = {
-    'lev_0-0.1_m_below_ground': 'off',
-    'lev_0.1-0.4_m_below_ground': 'off',
-    'lev_0.4-1_m_below_ground': 'off',
-    'lev_1-2_m_below_ground': 'off',
-    'lev_2_m_above_ground': 'off',
-    'lev_10_m_above_ground': 'off',
-    'lev_20_m_above_ground': 'off',
-    'lev_30_m_above_ground': 'off',
-    'lev_40_m_above_ground': 'off',
-    'lev_50_m_above_ground': 'off',
-    'lev_80_m_above_ground': 'off',
-    'lev_100_m_above_ground': 'off',
-    'lev_1000_m_above_ground': 'off',
-    'lev_4000_m_above_ground': 'off',
-    'lev_10_m_above_mean_sea_level': 'off',
-    'lev_1829_m_above_mean_sea_level': 'off',
-    'lev_2743_m_above_mean_sea_level': 'off',
-    'lev_3658_m_above_mean_sea_level': 'off',
-    'lev_3000-0_m_above_ground': 'off',
-    'lev_6000-0_m_above_ground': 'off',
-    'lev_180-0_mb_above_ground': 'off',
-    'lev_255-0_mb_above_ground': 'off',
-    'lev_90-0_mb_above_ground': 'off',
-    'lev_30-0_mb_above_ground': 'off',
-    'lev_0C_isotherm': 'off',
-    'lev_1_hybrid_level': 'off',
-    'lev_2_hybrid_level': 'off',
-    'lev_1000_mb': 'off',
-    'lev_975_mb': 'off',
-    'lev_950_mb': 'off',
-    'lev_925_mb': 'off',
-    'lev_900_mb': 'off',
-    'lev_850_mb': 'off',
-    'lev_800_mb': 'off',
-    'lev_750_mb': 'off',
-    'lev_700_mb': 'off',
-    'lev_650_mb': 'off',
-    'lev_600_mb': 'off',
-    'lev_550_mb': 'off',
-    'lev_500_mb': 'off',
-    'lev_450_mb': 'off',
-    'lev_400_mb': 'off',
-    'lev_350_mb': 'off',
-    'lev_300_mb': 'off',
-    'lev_250_mb': 'off',
-    'lev_200_mb': 'off',
-    'lev_150_mb': 'off',
-    'lev_100_mb': 'off',
-    'lev_70_mb': 'off',
-    'lev_50_mb': 'off',
-    'lev_40_mb': 'off',
-    'lev_30_mb': 'off',
-    'lev_20_mb': 'off',
-    'lev_15_mb': 'off',
-    'lev_10_mb': 'off',
-    'lev_7_mb': 'off',
-    'lev_5_mb': 'off',
-    'lev_3_mb': 'off',
-    'lev_2_mb': 'off',
-    'lev_1_mb': 'off',
-    'lev_0.7_mb': 'off',
-    'lev_0.4_mb': 'off',
-    'lev_0.2_mb': 'off',
-    'lev_0.1_mb': 'off',
-    'lev_0.07_mb': 'off',
-    'lev_0.04_mb': 'off',
-    'lev_0.02_mb': 'off',
-    'lev_0.01_mb': 'off',
-    'lev_surface': 'off',
-    'lev_mean_sea_level': 'off',
-    'lev_boundary_layer_cloud_layer': 'off',
-    'lev_planetary_boundary_layer': 'off',
-    'lev_tropopause': 'off',
-    'lev_entire_atmosphere': 'off',
-    'lev_entire_atmosphere_(considered_as_a_single_layer)': 'off',
-    'lev_top_atmosphere': 'off',
-    'lev_convective_cloud_layer': 'off',
-    'lev_convective_bottom_level': 'off',
-    'lev_convective_top_level': 'off',
-    'lev_high_cloud_layer': 'off',
-    'lev_high_cloud_bottom_level': 'off',
-    'lev_high_cloud_top_level': 'off',
-    'lev_low_cloud_layer': 'off',
-    'lev_low_cloud_bottom_level': 'off',
-    'lev_low_cloud_top_level': 'off',
-    'lev_middle_cloud_layer': 'off',
-    'lev_middle_cloud_bottom_level': 'off',
-    'lev_middle_cloud_top_level': 'off',
-    'lev_cloud_ceiling': 'off',
-    'lev_highest_tropospheric_freezing_level': 'off',
-    'lev_PV%3D-2e-06_(Km%5E2%2Fkg%2Fs)_surface': 'off',
-    'lev_PV%3D2e-06_(Km%5E2%2Fkg%2Fs)_surface': 'off',
-}
+# https://nomads.ncep.noaa.gov/gribfilter.php?ds=gfs_0p25_1hr
+gfs_parameters_dict = {
+    'var_4LFTX': 'off',
+    'var_ABSV': 'off',
+    'var_ACPCP': 'off',
+    'var_ALBDO': 'off',
+    'var_APCP': 'off',
+    'var_CAPE': 'off',
+    'var_CFRZR': 'off',
+    'var_CICEP': 'off',
+    'var_CIN': 'off',
+    'var_CLWMR': 'off',
+    'var_CNWAT': 'off',
+    'var_CPOFP': 'off',
+    'var_CPRAT': 'off',
+    'var_CRAIN': 'off',
+    'var_CSNOW': 'off',
+    'var_CWAT': 'off',
+    'var_CWORK': 'off',
+    'var_DLWRF': 'off',
+    'var_DPT': 'off',
+    'var_DSWRF': 'off',
+    'var_DZDT': 'off',
+    'var_FLDCP': 'off',
+    'var_FRICV': 'off',
+    'var_GFLUX': 'off',
+    'var_GRLEV': 'off',
+    'var_GUST': 'off',
+    'var_HCDC': 'off',
+    'var_HGT': 'off',
+    'var_HINDEX': 'off',
+    'var_HLCY': 'off',
+    'var_HPBL': 'off',
+    'var_ICAHT': 'off',
+    'var_ICEC': 'off',
+    'var_ICEG': 'off',
+    'var_ICETK': 'off',
+    'var_ICETMP': 'off',
+    'var_ICMR': 'off',
+    'var_LAND': 'off',
+    'var_LCDC': 'off',
+    'var_LFTX': 'off',
+    'var_LHTFL': 'off',
+    'var_MCDC': 'off',
+    'var_MSLET': 'off',
+    'var_O3MR': 'off',
+    'var_PEVFR': 'off',
+    'var_PLPL': 'off',
+    'var_POT': 'off',
+    'var_PRATE': 'off',
+    'var_PRES': 'off',
+    'var_PRMSL': 'off',
+    'var_PWAT': 'off',
+    'var_REFC': 'off',
+    'var_REFD': 'off',
+    'var_RH': 'off',
+    'var_RWMR': 'off',
+    'var_SFCR': 'off',
+    'var_SHTFL': 'off',
+    'var_SNMR': 'off',
+    'var_SNOD': 'off',
+    'var_SOILL': 'off',
+    'var_SOILW': 'off',
+    'var_SOTYP': 'off',
+    'var_SPFH': 'off',
+    'var_SUNSD': 'off',
+    'var_TCDC': 'off',
+    'var_TMAX': 'off',
+    'var_TMIN': 'off',
+    'var_TMP': 'off',
+    'var_TOZNE': 'off',
+    'var_TSOIL': 'off',
+    'var_UFLX': 'off',
+    'var_UGRD': 'off',
+    'var_U-GWD': 'off',
+    'var_ULWRF': 'off',
+    'var_USTM': 'off',
+    'var_USWRF': 'off',
+    'var_VEG': 'off',
+    'var_VFLX': 'off',
+    'var_VGRD': 'off',
+    'var_V-GWD': 'off',
+    'var_VIS': 'off',
+    'var_VRATE': 'off',
+    'var_VSTM': 'off',
+    'var_VVEL': 'off',
+    'var_VWSH': 'off',
+    'var_WATR': 'off',
+    'var_WEASD': 'off',
+    'var_WILT': 'off',
+}
+
+gfs_levels_dict = {
+    'lev_0-0.1_m_below_ground': 'off',
+    'lev_0.1-0.4_m_below_ground': 'off',
+    'lev_0.4-1_m_below_ground': 'off',
+    'lev_1-2_m_below_ground': 'off',
+    'lev_2_m_above_ground': 'off',
+    'lev_10_m_above_ground': 'off',
+    'lev_20_m_above_ground': 'off',
+    'lev_30_m_above_ground': 'off',
+    'lev_40_m_above_ground': 'off',
+    'lev_50_m_above_ground': 'off',
+    'lev_80_m_above_ground': 'off',
+    'lev_100_m_above_ground': 'off',
+    'lev_1000_m_above_ground': 'off',
+    'lev_4000_m_above_ground': 'off',
+    'lev_10_m_above_mean_sea_level': 'off',
+    'lev_1829_m_above_mean_sea_level': 'off',
+    'lev_2743_m_above_mean_sea_level': 'off',
+    'lev_3658_m_above_mean_sea_level': 'off',
+    'lev_3000-0_m_above_ground': 'off',
+    'lev_6000-0_m_above_ground': 'off',
+    'lev_180-0_mb_above_ground': 'off',
+    'lev_255-0_mb_above_ground': 'off',
+    'lev_90-0_mb_above_ground': 'off',
+    'lev_30-0_mb_above_ground': 'off',
+    'lev_0C_isotherm': 'off',
+    'lev_1_hybrid_level': 'off',
+    'lev_2_hybrid_level': 'off',
+    'lev_1000_mb': 'off',
+    'lev_975_mb': 'off',
+    'lev_950_mb': 'off',
+    'lev_925_mb': 'off',
+    'lev_900_mb': 'off',
+    'lev_850_mb': 'off',
+    'lev_800_mb': 'off',
+    'lev_750_mb': 'off',
+    'lev_700_mb': 'off',
+    'lev_650_mb': 'off',
+    'lev_600_mb': 'off',
+    'lev_550_mb': 'off',
+    'lev_500_mb': 'off',
+    'lev_450_mb': 'off',
+    'lev_400_mb': 'off',
+    'lev_350_mb': 'off',
+    'lev_300_mb': 'off',
+    'lev_250_mb': 'off',
+    'lev_200_mb': 'off',
+    'lev_150_mb': 'off',
+    'lev_100_mb': 'off',
+    'lev_70_mb': 'off',
+    'lev_50_mb': 'off',
+    'lev_40_mb': 'off',
+    'lev_30_mb': 'off',
+    'lev_20_mb': 'off',
+    'lev_15_mb': 'off',
+    'lev_10_mb': 'off',
+    'lev_7_mb': 'off',
+    'lev_5_mb': 'off',
+    'lev_3_mb': 'off',
+    'lev_2_mb': 'off',
+    'lev_1_mb': 'off',
+    'lev_0.7_mb': 'off',
+    'lev_0.4_mb': 'off',
+    'lev_0.2_mb': 'off',
+    'lev_0.1_mb': 'off',
+    'lev_0.07_mb': 'off',
+    'lev_0.04_mb': 'off',
+    'lev_0.02_mb': 'off',
+    'lev_0.01_mb': 'off',
+    'lev_surface': 'off',
+    'lev_mean_sea_level': 'off',
+    'lev_boundary_layer_cloud_layer': 'off',
+    'lev_planetary_boundary_layer': 'off',
+    'lev_tropopause': 'off',
+    'lev_entire_atmosphere': 'off',
+    'lev_entire_atmosphere_(considered_as_a_single_layer)': 'off',
+    'lev_top_atmosphere': 'off',
+    'lev_convective_cloud_layer': 'off',
+    'lev_convective_bottom_level': 'off',
+    'lev_convective_top_level': 'off',
+    'lev_high_cloud_layer': 'off',
+    'lev_high_cloud_bottom_level': 'off',
+    'lev_high_cloud_top_level': 'off',
+    'lev_low_cloud_layer': 'off',
+    'lev_low_cloud_bottom_level': 'off',
+    'lev_low_cloud_top_level': 'off',
+    'lev_middle_cloud_layer': 'off',
+    'lev_middle_cloud_bottom_level': 'off',
+    'lev_middle_cloud_top_level': 'off',
+    'lev_cloud_ceiling': 'off',
+    'lev_highest_tropospheric_freezing_level': 'off',
+    'lev_PV%3D-2e-06_(Km%5E2%2Fkg%2Fs)_surface': 'off',
+    'lev_PV%3D2e-06_(Km%5E2%2Fkg%2Fs)_surface': 'off',
+}
```

### Comparing `hydrodatasource-0.0.1/hydrodatasource/downloader/gfs_downloader_auto.py` & `hydrodatasource-0.0.2/hydrodatasource/downloader/gfs_downloader_auto.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,325 +1,325 @@
-#!/home/zhujianfeng/.conda/envs/stac-test/bin/python
-
-import datetime
-import json
-import os
-import subprocess
-from pathlib import Path
-
-import kerchunk.grib2
-import numpy as np
-import s3fs
-import ujson
-from apscheduler.schedulers.blocking import BlockingScheduler  # 后台运行
-from kerchunk.combine import MultiZarrToZarr, drop
-from minio import Minio
-import yaml
-
-work_dir = Path(__file__).resolve().parent
-with open(work_dir / 'privacy_config.yaml', 'r') as f:
-    privacy_config = yaml.safe_load(f)
-storage_options = {
-    'client_kwargs': {'endpoint_url': privacy_config['minio']['client_endpoint']},
-    'key': privacy_config['minio']['access_key'],
-    'secret': privacy_config['minio']['secret']
-}
-minioClient = Minio(storage_options['client_kwargs'],
-                    storage_options['key'],
-                    secret_key=privacy_config['minio']['secret'],
-                    secure=False)
-fs = s3fs.S3FileSystem(
-    client_kwargs={"endpoint_url": privacy_config['minio']['client_endpoint']},
-    key=privacy_config['minio']['access_key'],
-    secret=privacy_config['minio']['secret']
-)
-
-sc = BlockingScheduler(timezone="Asia/Shanghai")
-
-bbox = [73, 3, 136, 54]
-
-
-@sc.scheduled_job('cron', day_of_week='*', hour='12', minute='10', second='00')
-def gfs_downloader_00():
-    f = open('log.txt', 'a', encoding='utf8')
-    date = datetime.datetime.now()
-    # date=date + datetime.timedelta(days = -1)
-    date = date.strftime('%Y%m%d')
-    creation_time = '00'
-    urls = []
-    # https://nomads.ncep.noaa.gov/gribfilter.php?ds=gfs_0p25_1hr
-    # https://github.com/albertotb/get-gfs
-    # https://dtcenter.org/nwp-containers-online-tutorial/publicly-available-data-sets
-    # https://www.nco.ncep.noaa.gov/pmb/docs/grib2/grib2_doc/, PWAT指降雨
-    url_ = ('https://nomads.ncep.noaa.gov/cgi-bin/filter_gfs_0p25.pl?file=gfs.tCCz.pgrb2.0p25.fFFF'
-            '&lev_10_m_above_ground=on&lev_2_m_above_ground=on&lev_entire_atmosphere=on&lev_entire_atmosphere_%5C'
-            '%28considered_as_a_single_layer%5C%29=on&lev_surface=on&var_APCP=on&var_DSWRF=on&var_PWAT=on&var_RH=on'
-            '&var_SPFH=on&var_TCDC=on&var_TMP=on&var_UGRD=on&var_VGRD=on&subregion=&leftlon=') + str(
-        bbox[0]) + '&rightlon=' + str(bbox[2]) + '&toplat=' + str(bbox[3]) + '&bottomlat=' + str(
-        bbox[1]) + '&dir=%2Fgfs.YYYYMMDD%2FCC%2Fatmos'
-    # save_dir='gfs/'
-    for forecast_time in range(1, 121):
-        # ncep_gfs.get_gfs_from_ncep(date,creation_time,forecast_time,bbox=[73,3,136,54],save_dir=save_dir)
-        url = url_.replace('YYYYMMDD', date).replace('CC', creation_time.zfill(2)).replace('FFF',
-                                                                                           str(forecast_time).zfill(3))
-        urls.append(url)
-
-    with open('./urls.txt', mode='w') as gpm:
-        [gpm.write(str(url) + '\n') for url in urls]
-
-    subprocess.run("cat urls.txt | tr -d '\r' | xargs -n 1 curl -LJO -n -c ~/.urs_cookies -b ~/.urs_cookies",
-                   shell=True)
-
-    check_file()
-    upload2server(date, creation_time)
-    single_json(date, creation_time)
-    multi_json(date, creation_time)
-    print(datetime.datetime.now().strftime('%Y%m%d-%H:%M:%S'), '定时任务成功执行')
-    print(datetime.datetime.now().strftime('%Y%m%d-%H:%M:%S'), '定时任务成功执行', file=f)
-
-
-@sc.scheduled_job('cron', day_of_week='*', hour='18', minute='10', second='00')
-def gfs_downloader_06():
-    f = open('log.txt', 'a', encoding='utf8')
-    date = datetime.datetime.now()
-    date = date.strftime('%Y%m%d')
-    creation_time = '06'
-    urls = []
-    url_ = (
-               'https://nomads.ncep.noaa.gov/cgi-bin/filter_gfs_0p25.pl?file=gfs.tCCz.pgrb2.0p25.fFFF&lev_10_m_above_ground'
-               '=on&lev_2_m_above_ground=on&lev_entire_atmosphere=on'
-               '&lev_entire_atmosphere_%5C%28considered_as_a_single_layer%5C%29=on&lev_surface=on&var_APCP=on&'
-               'var_DSWRF=on&var_PWAT=on&var_RH=on&var_SPFH=on&var_TCDC=on&var_TMP=on&var_UGRD=on&var_VGRD=on&subregion'
-               '=&leftlon=') + str(
-        bbox[0]) + '&rightlon=' + str(bbox[2]) + '&toplat=' + str(bbox[3]) + '&bottomlat=' + str(
-        bbox[1]) + '&dir=%2Fgfs.YYYYMMDD%2FCC%2Fatmos'
-
-    # save_dir='gfs/'
-    for forecast_time in range(1, 121):
-        # ncep_gfs.get_gfs_from_ncep(date,creation_time,forecast_time,bbox=[73,3,136,54],save_dir=save_dir)
-        url = url_.replace('YYYYMMDD', date).replace('CC', creation_time.zfill(2)).replace('FFF',
-                                                                                           str(forecast_time).zfill(3))
-        urls.append(url)
-    with open('./urls.txt', mode='w') as gpm:
-        [gpm.write(str(url) + '\n') for url in urls]
-    subprocess.run("cat urls.txt | tr -d '\r' | xargs -n 1 curl -LJO -n -c ~/.urs_cookies -b ~/.urs_cookies",
-                   shell=True)
-    check_file()
-    upload2server(date, creation_time)
-    single_json(date, creation_time)
-    multi_json(date, creation_time)
-    print(datetime.datetime.now().strftime('%Y%m%d-%H:%M:%S'), '定时任务成功执行')
-    print(datetime.datetime.now().strftime('%Y%m%d-%H:%M:%S'), '定时任务成功执行', file=f)
-    f.close()
-
-
-@sc.scheduled_job('cron', day_of_week='*', hour='00', minute='10', second='00')
-def gfs_downloader_12():
-    date = datetime.datetime.now()
-    date = date + datetime.timedelta(days=-1)
-    date = date.strftime('%Y%m%d')
-    creation_time = '12'
-    urls = []
-    url_ = ('https://nomads.ncep.noaa.gov/cgi-bin/filter_gfs_0p25.pl?file=gfs.tCCz.pgrb2.0p25.fFFF'
-            '&lev_10_m_above_ground=on&lev_2_m_above_ground=on&lev_entire_atmosphere=on&lev_entire_atmosphere_%5C'
-            '%28considered_as_a_single_layer%5C%29=on&lev_surface=on&var_APCP=on&var_DSWRF=on&var_PWAT=on&var_RH=on'
-            '&var_SPFH=on&var_TCDC=on&var_TMP=on&var_UGRD=on&var_VGRD=on&subregion=&leftlon=') + str(
-        bbox[0]) + '&rightlon=' + str(bbox[2]) + '&toplat=' + str(bbox[3]) + '&bottomlat=' + str(
-        bbox[1]) + '&dir=%2Fgfs.YYYYMMDD%2FCC%2Fatmos'
-    # save_dir='gfs/'
-    for forecast_time in range(1, 121):
-        # ncep_gfs.get_gfs_from_ncep(date,creation_time,forecast_time,bbox=[73,3,136,54],save_dir=save_dir)
-        url = url_.replace('YYYYMMDD', date).replace('CC', creation_time.zfill(2)).replace('FFF',
-                                                                                           str(forecast_time).zfill(3))
-        urls.append(url)
-
-    with open('./urls.txt', mode='w') as gpm:
-        [gpm.write(str(url) + '\n') for url in urls]
-    subprocess.run("cat urls.txt | tr -d '\r' | xargs -n 1 curl -LJO -n -c ~/.urs_cookies -b ~/.urs_cookies",
-                   shell=True)
-    check_file()
-    upload2server(date, creation_time)
-    single_json(date, creation_time)
-    multi_json(date, creation_time)
-    print(datetime.datetime.now().strftime('%Y%m%d-%H:%M:%S'), '定时任务成功执行')
-    print(datetime.datetime.now().strftime('%Y%m%d-%H:%M:%S'), '定时任务成功执行', file=f)
-
-
-@sc.scheduled_job('cron', day_of_week='*', hour='06', minute='10', second='00')
-def gfs_downloader_18():
-    date = datetime.datetime.now()
-    date = date + datetime.timedelta(days=-1)
-    date = date.strftime('%Y%m%d')
-    creation_time = '18'
-    urls = []
-    url_ = ('https://nomads.ncep.noaa.gov/cgi-bin/filter_gfs_0p25.pl?file=gfs.tCCz.pgrb2.0p25.fFFF'
-            '&lev_10_m_above_ground=on&lev_2_m_above_ground=on&lev_entire_atmosphere=on&lev_entire_atmosphere_%5C'
-            '%28considered_as_a_single_layer%5C%29=on&lev_surface=on&var_APCP=on&var_DSWRF=on&var_PWAT=on&var_RH=on'
-            '&var_SPFH=on&var_TCDC=on&var_TMP=on&var_UGRD=on&var_VGRD=on&subregion=&leftlon=') + str(
-        bbox[0]) + '&rightlon=' + str(bbox[2]) + '&toplat=' + str(bbox[3]) + '&bottomlat=' + str(
-        bbox[1]) + '&dir=%2Fgfs.YYYYMMDD%2FCC%2Fatmos'
-    # save_dir='gfs/'
-    for forecast_time in range(1, 121):
-        # ncep_gfs.get_gfs_from_ncep(date,creation_time,forecast_time,bbox=[73,3,136,54],save_dir=save_dir)
-        url = url_.replace('YYYYMMDD', date).replace('CC', creation_time.zfill(2)).replace('FFF',
-                                                                                           str(forecast_time).zfill(3))
-        urls.append(url)
-    with open('./urls.txt', mode='w') as gpm:
-        [gpm.write(str(url) + '\n') for url in urls]
-    subprocess.run("cat urls.txt | tr -d '\r' | xargs -n 1 curl -LJO -n -c ~/.urs_cookies -b ~/.urs_cookies",
-                   shell=True)
-    check_file()
-    upload2server(date, creation_time)
-    single_json(date, creation_time)
-    multi_json(date, creation_time)
-    print(datetime.datetime.now().strftime('%Y%m%d-%H:%M:%S'), '定时任务成功执行')
-    print(datetime.datetime.now().strftime('%Y%m%d-%H:%M:%S'), '定时任务成功执行', file=f)
-
-
-def check_file():
-    while True:
-        count = 0
-        for root, dirs, filenames in os.walk('.'):
-            for filename in filenames:
-                if 'pgrb2' in filename:
-                    filepath = os.path.join(root, filename)
-                    size = os.path.getsize(filepath)
-                    count = count + 1
-                    if size < 600000:
-                        os.remove(filepath)
-                        count = count - 1
-        if count >= 120:
-            break
-
-        else:
-            subprocess.run("cat urls.txt | tr -d '\r' | xargs -n 1 curl -LJO -n -c ~/.urs_cookies -b ~/.urs_cookies",
-                           shell=True)
-    print("检查下载完成！")
-
-
-def str_insert(str_origin, pos, str_add):
-    str_list = list(str_origin)
-    str_list.insert(pos, str_add)
-    str_out = ''.join(str_list)
-    return str_out
-
-
-def upload2server(gfs_date, create_time):
-    for root, dirs, filenames in os.walk('.'):
-        for filename in filenames:
-            if 'pgrb2' in filename:
-                # gfs_date = filename[3:11]
-                year = gfs_date[0:4]
-                month = gfs_date[4:6]
-                day = gfs_date[6:8]
-                # create_time = filename[13:15]
-                gfs_name = str_insert(filename, 3, gfs_date)
-                minio_path = f'geodata/gfs/{year}/{month}/{day}/{create_time}/{gfs_name}'
-                try:
-                    print(minioClient.fput_object('watermodel-pub', minio_path, os.path.join(root, filename)))
-                    path = Path(f"/ftproot/geodata/gfs/{year}/{month}/{day}/{create_time}")
-                    if not path.is_dir():
-                        path.mkdir(parents=True, exist_ok=True)
-                    file_path = os.path.join(root, filename)
-                    os.system(f"mv {file_path} /ftproot/geodata/gfs/{year}/{month}/{day}/{create_time}/{gfs_name}")
-                except Exception as err:
-                    print(err)
-    print("上传完成！")
-
-
-def gen_json(flist):
-    for furl in flist:
-
-        try:
-
-            out = [kerchunk.grib2.scan_grib(u, storage_options=storage_options, inline_threshold=3000,
-                                            filter={"shortName": "tp"}) for u in [furl]]
-            outs = out[0][0]
-            outf = furl + '.json'  # file name to save json to
-            outf = outf.replace('watermodel-pub', 'test').replace('gfs/', 'gfs/tp/')
-
-            with fs.open(outf, 'wb') as ff:
-                ff.write(ujson.dumps(outs).encode())
-
-            # print(outf)
-        except:
-            print(furl, "出错！")
-
-
-def single_json(gfs_date, create_time):
-    year = gfs_date[0:4]
-    month = gfs_date[4:6]
-    day = gfs_date[6:8]
-
-    flist = fs.glob(f'watermodel-pub/geodata/gfs/{year}/{month}/{day}/{create_time}/*')
-    flist = ['s3://' + str for str in flist]
-    # print(flist)
-    gen_json(flist)
-
-
-def fn_to_time(index, fs, var, fn):
-    import re
-    import datetime
-    import time
-    today = datetime.datetime.strptime(time.strftime("%Y-%m-%d %H-%M-%S", time.gmtime(int(fs['time'][0]))),
-                                       '%Y-%m-%d %H-%M-%S')
-    ex = re.compile(r'.*f(\d+)')
-    i = int(ex.match(fn).groups()[0])
-    offset = datetime.timedelta(hours=i)
-    return today + offset
-
-
-def fn_to_index(index, fs, var, fn):
-    import re
-    ex = re.compile(r'.*f(\d+)')
-    i = int(ex.match(fn).groups()[0])
-    return i
-
-
-def gen_mzz(year, month, day, time):
-    json_list = fs.glob(
-        f"test/geodata/gfs/tp/{str(year).zfill(4)}/{str(month).zfill(2)}/{str(day).zfill(2)}/{time}/*.json")
-    if len(json_list) == 0:
-        return
-    json_list = ['s3://' + str for str in json_list]
-
-    mzz = MultiZarrToZarr(
-        json_list,
-        target_options=storage_options,
-        remote_protocol='s3',
-        remote_options=storage_options,
-        preprocess=drop(("surface", "step", "valid_time")),
-        coo_map={'valid_time': fn_to_time, 'step': fn_to_index},
-        coo_dtypes={'valid_time': np.dtype('M8[ns]'), 'step': np.dtype('int64')},
-        concat_dims=['valid_time', 'step'],
-        identical_dims=['latitude', 'longitude', 'time']
-    )
-
-    d = mzz.translate()
-    with fs.open(
-        f's3://test/geodata/gfs/tp/{str(year).zfill(4)}/{str(month).zfill(2)}/{str(day).zfill(2)}/gfs{str(year).zfill(4)}{str(month).zfill(2)}{str(day).zfill(2)}.t{time}z.0p25.json',
-        'wb') as ff:
-        ff.write(ujson.dumps(d).encode())
-    print(
-        f's3://test/geodata/gfs/tp/{str(year).zfill(4)}/{str(month).zfill(2)}/{str(day).zfill(2)}/gfs{str(year).zfill(4)}{str(month).zfill(2)}{str(day).zfill(2)}.t{time}z.0p25.json')
-
-    with fs.open('test/geodata/gfs/gfs.json') as ff:
-        cont = json.load(ff)
-    cont['tp'][-1]['end'] = f'{year}-{month}-{day}T{time}'
-    with fs.open('test/geodata/gfs/gfs.json', 'w') as ff:
-        json.dump(cont, ff)
-    print('更新至', f'{year}-{month}-{day}T{time}')
-
-
-def multi_json(gfs_date, create_time):
-    year = gfs_date[0:4]
-    month = gfs_date[4:6]
-    day = gfs_date[6:8]
-    gen_mzz(year, month, day, create_time)
-
-
-if __name__ == '__main__':
-    try:
-        sc.start()
-    except Exception as e:
-        sc.shutdown()
-        print(datetime.datetime.now().strftime('%Y%m%d-%H:%M:%S'), '下载任务停止')
+#!/home/zhujianfeng/.conda/envs/stac-test/bin/python
+
+import datetime
+import json
+import os
+import subprocess
+from pathlib import Path
+
+import kerchunk.grib2
+import numpy as np
+import s3fs
+import ujson
+from apscheduler.schedulers.blocking import BlockingScheduler  # 后台运行
+from kerchunk.combine import MultiZarrToZarr, drop
+from minio import Minio
+import yaml
+
+work_dir = Path(__file__).resolve().parent
+with open(work_dir / 'privacy_config.yaml', 'r') as f:
+    privacy_config = yaml.safe_load(f)
+storage_options = {
+    'client_kwargs': {'endpoint_url': privacy_config['minio']['client_endpoint']},
+    'key': privacy_config['minio']['access_key'],
+    'secret': privacy_config['minio']['secret']
+}
+minioClient = Minio(storage_options['client_kwargs'],
+                    storage_options['key'],
+                    secret_key=privacy_config['minio']['secret'],
+                    secure=False)
+fs = s3fs.S3FileSystem(
+    client_kwargs={"endpoint_url": privacy_config['minio']['client_endpoint']},
+    key=privacy_config['minio']['access_key'],
+    secret=privacy_config['minio']['secret']
+)
+
+sc = BlockingScheduler(timezone="Asia/Shanghai")
+
+bbox = [73, 3, 136, 54]
+
+
+@sc.scheduled_job('cron', day_of_week='*', hour='12', minute='10', second='00')
+def gfs_downloader_00():
+    f = open('log.txt', 'a', encoding='utf8')
+    date = datetime.datetime.now()
+    # date=date + datetime.timedelta(days = -1)
+    date = date.strftime('%Y%m%d')
+    creation_time = '00'
+    urls = []
+    # https://nomads.ncep.noaa.gov/gribfilter.php?ds=gfs_0p25_1hr
+    # https://github.com/albertotb/get-gfs
+    # https://dtcenter.org/nwp-containers-online-tutorial/publicly-available-data-sets
+    # https://www.nco.ncep.noaa.gov/pmb/docs/grib2/grib2_doc/, PWAT指降雨
+    url_ = ('https://nomads.ncep.noaa.gov/cgi-bin/filter_gfs_0p25.pl?file=gfs.tCCz.pgrb2.0p25.fFFF'
+            '&lev_10_m_above_ground=on&lev_2_m_above_ground=on&lev_entire_atmosphere=on&lev_entire_atmosphere_%5C'
+            '%28considered_as_a_single_layer%5C%29=on&lev_surface=on&var_APCP=on&var_DSWRF=on&var_PWAT=on&var_RH=on'
+            '&var_SPFH=on&var_TCDC=on&var_TMP=on&var_UGRD=on&var_VGRD=on&subregion=&leftlon=') + str(
+        bbox[0]) + '&rightlon=' + str(bbox[2]) + '&toplat=' + str(bbox[3]) + '&bottomlat=' + str(
+        bbox[1]) + '&dir=%2Fgfs.YYYYMMDD%2FCC%2Fatmos'
+    # save_dir='gfs/'
+    for forecast_time in range(1, 121):
+        # ncep_gfs.get_gfs_from_ncep(date,creation_time,forecast_time,bbox=[73,3,136,54],save_dir=save_dir)
+        url = url_.replace('YYYYMMDD', date).replace('CC', creation_time.zfill(2)).replace('FFF',
+                                                                                           str(forecast_time).zfill(3))
+        urls.append(url)
+
+    with open('./urls.txt', mode='w') as gpm:
+        [gpm.write(str(url) + '\n') for url in urls]
+
+    subprocess.run("cat urls.txt | tr -d '\r' | xargs -n 1 curl -LJO -n -c ~/.urs_cookies -b ~/.urs_cookies",
+                   shell=True)
+
+    check_file()
+    upload2server(date, creation_time)
+    single_json(date, creation_time)
+    multi_json(date, creation_time)
+    print(datetime.datetime.now().strftime('%Y%m%d-%H:%M:%S'), '定时任务成功执行')
+    print(datetime.datetime.now().strftime('%Y%m%d-%H:%M:%S'), '定时任务成功执行', file=f)
+
+
+@sc.scheduled_job('cron', day_of_week='*', hour='18', minute='10', second='00')
+def gfs_downloader_06():
+    f = open('log.txt', 'a', encoding='utf8')
+    date = datetime.datetime.now()
+    date = date.strftime('%Y%m%d')
+    creation_time = '06'
+    urls = []
+    url_ = (
+               'https://nomads.ncep.noaa.gov/cgi-bin/filter_gfs_0p25.pl?file=gfs.tCCz.pgrb2.0p25.fFFF&lev_10_m_above_ground'
+               '=on&lev_2_m_above_ground=on&lev_entire_atmosphere=on'
+               '&lev_entire_atmosphere_%5C%28considered_as_a_single_layer%5C%29=on&lev_surface=on&var_APCP=on&'
+               'var_DSWRF=on&var_PWAT=on&var_RH=on&var_SPFH=on&var_TCDC=on&var_TMP=on&var_UGRD=on&var_VGRD=on&subregion'
+               '=&leftlon=') + str(
+        bbox[0]) + '&rightlon=' + str(bbox[2]) + '&toplat=' + str(bbox[3]) + '&bottomlat=' + str(
+        bbox[1]) + '&dir=%2Fgfs.YYYYMMDD%2FCC%2Fatmos'
+
+    # save_dir='gfs/'
+    for forecast_time in range(1, 121):
+        # ncep_gfs.get_gfs_from_ncep(date,creation_time,forecast_time,bbox=[73,3,136,54],save_dir=save_dir)
+        url = url_.replace('YYYYMMDD', date).replace('CC', creation_time.zfill(2)).replace('FFF',
+                                                                                           str(forecast_time).zfill(3))
+        urls.append(url)
+    with open('./urls.txt', mode='w') as gpm:
+        [gpm.write(str(url) + '\n') for url in urls]
+    subprocess.run("cat urls.txt | tr -d '\r' | xargs -n 1 curl -LJO -n -c ~/.urs_cookies -b ~/.urs_cookies",
+                   shell=True)
+    check_file()
+    upload2server(date, creation_time)
+    single_json(date, creation_time)
+    multi_json(date, creation_time)
+    print(datetime.datetime.now().strftime('%Y%m%d-%H:%M:%S'), '定时任务成功执行')
+    print(datetime.datetime.now().strftime('%Y%m%d-%H:%M:%S'), '定时任务成功执行', file=f)
+    f.close()
+
+
+@sc.scheduled_job('cron', day_of_week='*', hour='00', minute='10', second='00')
+def gfs_downloader_12():
+    date = datetime.datetime.now()
+    date = date + datetime.timedelta(days=-1)
+    date = date.strftime('%Y%m%d')
+    creation_time = '12'
+    urls = []
+    url_ = ('https://nomads.ncep.noaa.gov/cgi-bin/filter_gfs_0p25.pl?file=gfs.tCCz.pgrb2.0p25.fFFF'
+            '&lev_10_m_above_ground=on&lev_2_m_above_ground=on&lev_entire_atmosphere=on&lev_entire_atmosphere_%5C'
+            '%28considered_as_a_single_layer%5C%29=on&lev_surface=on&var_APCP=on&var_DSWRF=on&var_PWAT=on&var_RH=on'
+            '&var_SPFH=on&var_TCDC=on&var_TMP=on&var_UGRD=on&var_VGRD=on&subregion=&leftlon=') + str(
+        bbox[0]) + '&rightlon=' + str(bbox[2]) + '&toplat=' + str(bbox[3]) + '&bottomlat=' + str(
+        bbox[1]) + '&dir=%2Fgfs.YYYYMMDD%2FCC%2Fatmos'
+    # save_dir='gfs/'
+    for forecast_time in range(1, 121):
+        # ncep_gfs.get_gfs_from_ncep(date,creation_time,forecast_time,bbox=[73,3,136,54],save_dir=save_dir)
+        url = url_.replace('YYYYMMDD', date).replace('CC', creation_time.zfill(2)).replace('FFF',
+                                                                                           str(forecast_time).zfill(3))
+        urls.append(url)
+
+    with open('./urls.txt', mode='w') as gpm:
+        [gpm.write(str(url) + '\n') for url in urls]
+    subprocess.run("cat urls.txt | tr -d '\r' | xargs -n 1 curl -LJO -n -c ~/.urs_cookies -b ~/.urs_cookies",
+                   shell=True)
+    check_file()
+    upload2server(date, creation_time)
+    single_json(date, creation_time)
+    multi_json(date, creation_time)
+    print(datetime.datetime.now().strftime('%Y%m%d-%H:%M:%S'), '定时任务成功执行')
+    print(datetime.datetime.now().strftime('%Y%m%d-%H:%M:%S'), '定时任务成功执行', file=f)
+
+
+@sc.scheduled_job('cron', day_of_week='*', hour='06', minute='10', second='00')
+def gfs_downloader_18():
+    date = datetime.datetime.now()
+    date = date + datetime.timedelta(days=-1)
+    date = date.strftime('%Y%m%d')
+    creation_time = '18'
+    urls = []
+    url_ = ('https://nomads.ncep.noaa.gov/cgi-bin/filter_gfs_0p25.pl?file=gfs.tCCz.pgrb2.0p25.fFFF'
+            '&lev_10_m_above_ground=on&lev_2_m_above_ground=on&lev_entire_atmosphere=on&lev_entire_atmosphere_%5C'
+            '%28considered_as_a_single_layer%5C%29=on&lev_surface=on&var_APCP=on&var_DSWRF=on&var_PWAT=on&var_RH=on'
+            '&var_SPFH=on&var_TCDC=on&var_TMP=on&var_UGRD=on&var_VGRD=on&subregion=&leftlon=') + str(
+        bbox[0]) + '&rightlon=' + str(bbox[2]) + '&toplat=' + str(bbox[3]) + '&bottomlat=' + str(
+        bbox[1]) + '&dir=%2Fgfs.YYYYMMDD%2FCC%2Fatmos'
+    # save_dir='gfs/'
+    for forecast_time in range(1, 121):
+        # ncep_gfs.get_gfs_from_ncep(date,creation_time,forecast_time,bbox=[73,3,136,54],save_dir=save_dir)
+        url = url_.replace('YYYYMMDD', date).replace('CC', creation_time.zfill(2)).replace('FFF',
+                                                                                           str(forecast_time).zfill(3))
+        urls.append(url)
+    with open('./urls.txt', mode='w') as gpm:
+        [gpm.write(str(url) + '\n') for url in urls]
+    subprocess.run("cat urls.txt | tr -d '\r' | xargs -n 1 curl -LJO -n -c ~/.urs_cookies -b ~/.urs_cookies",
+                   shell=True)
+    check_file()
+    upload2server(date, creation_time)
+    single_json(date, creation_time)
+    multi_json(date, creation_time)
+    print(datetime.datetime.now().strftime('%Y%m%d-%H:%M:%S'), '定时任务成功执行')
+    print(datetime.datetime.now().strftime('%Y%m%d-%H:%M:%S'), '定时任务成功执行', file=f)
+
+
+def check_file():
+    while True:
+        count = 0
+        for root, dirs, filenames in os.walk('.'):
+            for filename in filenames:
+                if 'pgrb2' in filename:
+                    filepath = os.path.join(root, filename)
+                    size = os.path.getsize(filepath)
+                    count = count + 1
+                    if size < 600000:
+                        os.remove(filepath)
+                        count = count - 1
+        if count >= 120:
+            break
+
+        else:
+            subprocess.run("cat urls.txt | tr -d '\r' | xargs -n 1 curl -LJO -n -c ~/.urs_cookies -b ~/.urs_cookies",
+                           shell=True)
+    print("检查下载完成！")
+
+
+def str_insert(str_origin, pos, str_add):
+    str_list = list(str_origin)
+    str_list.insert(pos, str_add)
+    str_out = ''.join(str_list)
+    return str_out
+
+
+def upload2server(gfs_date, create_time):
+    for root, dirs, filenames in os.walk('.'):
+        for filename in filenames:
+            if 'pgrb2' in filename:
+                # gfs_date = filename[3:11]
+                year = gfs_date[0:4]
+                month = gfs_date[4:6]
+                day = gfs_date[6:8]
+                # create_time = filename[13:15]
+                gfs_name = str_insert(filename, 3, gfs_date)
+                minio_path = f'geodata/gfs/{year}/{month}/{day}/{create_time}/{gfs_name}'
+                try:
+                    print(minioClient.fput_object('watermodel-pub', minio_path, os.path.join(root, filename)))
+                    path = Path(f"/ftproot/geodata/gfs/{year}/{month}/{day}/{create_time}")
+                    if not path.is_dir():
+                        path.mkdir(parents=True, exist_ok=True)
+                    file_path = os.path.join(root, filename)
+                    os.system(f"mv {file_path} /ftproot/geodata/gfs/{year}/{month}/{day}/{create_time}/{gfs_name}")
+                except Exception as err:
+                    print(err)
+    print("上传完成！")
+
+
+def gen_json(flist):
+    for furl in flist:
+
+        try:
+
+            out = [kerchunk.grib2.scan_grib(u, storage_options=storage_options, inline_threshold=3000,
+                                            filter={"shortName": "tp"}) for u in [furl]]
+            outs = out[0][0]
+            outf = furl + '.json'  # file name to save json to
+            outf = outf.replace('watermodel-pub', 'test').replace('gfs/', 'gfs/tp/')
+
+            with fs.open(outf, 'wb') as ff:
+                ff.write(ujson.dumps(outs).encode())
+
+            # print(outf)
+        except:
+            print(furl, "出错！")
+
+
+def single_json(gfs_date, create_time):
+    year = gfs_date[0:4]
+    month = gfs_date[4:6]
+    day = gfs_date[6:8]
+
+    flist = fs.glob(f'watermodel-pub/geodata/gfs/{year}/{month}/{day}/{create_time}/*')
+    flist = ['s3://' + str for str in flist]
+    # print(flist)
+    gen_json(flist)
+
+
+def fn_to_time(index, fs, var, fn):
+    import re
+    import datetime
+    import time
+    today = datetime.datetime.strptime(time.strftime("%Y-%m-%d %H-%M-%S", time.gmtime(int(fs['time'][0]))),
+                                       '%Y-%m-%d %H-%M-%S')
+    ex = re.compile(r'.*f(\d+)')
+    i = int(ex.match(fn).groups()[0])
+    offset = datetime.timedelta(hours=i)
+    return today + offset
+
+
+def fn_to_index(index, fs, var, fn):
+    import re
+    ex = re.compile(r'.*f(\d+)')
+    i = int(ex.match(fn).groups()[0])
+    return i
+
+
+def gen_mzz(year, month, day, time):
+    json_list = fs.glob(
+        f"test/geodata/gfs/tp/{str(year).zfill(4)}/{str(month).zfill(2)}/{str(day).zfill(2)}/{time}/*.json")
+    if len(json_list) == 0:
+        return
+    json_list = ['s3://' + str for str in json_list]
+
+    mzz = MultiZarrToZarr(
+        json_list,
+        target_options=storage_options,
+        remote_protocol='s3',
+        remote_options=storage_options,
+        preprocess=drop(("surface", "step", "valid_time")),
+        coo_map={'valid_time': fn_to_time, 'step': fn_to_index},
+        coo_dtypes={'valid_time': np.dtype('M8[ns]'), 'step': np.dtype('int64')},
+        concat_dims=['valid_time', 'step'],
+        identical_dims=['latitude', 'longitude', 'time']
+    )
+
+    d = mzz.translate()
+    with fs.open(
+        f's3://test/geodata/gfs/tp/{str(year).zfill(4)}/{str(month).zfill(2)}/{str(day).zfill(2)}/gfs{str(year).zfill(4)}{str(month).zfill(2)}{str(day).zfill(2)}.t{time}z.0p25.json',
+        'wb') as ff:
+        ff.write(ujson.dumps(d).encode())
+    print(
+        f's3://test/geodata/gfs/tp/{str(year).zfill(4)}/{str(month).zfill(2)}/{str(day).zfill(2)}/gfs{str(year).zfill(4)}{str(month).zfill(2)}{str(day).zfill(2)}.t{time}z.0p25.json')
+
+    with fs.open('test/geodata/gfs/gfs.json') as ff:
+        cont = json.load(ff)
+    cont['tp'][-1]['end'] = f'{year}-{month}-{day}T{time}'
+    with fs.open('test/geodata/gfs/gfs.json', 'w') as ff:
+        json.dump(cont, ff)
+    print('更新至', f'{year}-{month}-{day}T{time}')
+
+
+def multi_json(gfs_date, create_time):
+    year = gfs_date[0:4]
+    month = gfs_date[4:6]
+    day = gfs_date[6:8]
+    gen_mzz(year, month, day, create_time)
+
+
+if __name__ == '__main__':
+    try:
+        sc.start()
+    except Exception as e:
+        sc.shutdown()
+        print(datetime.datetime.now().strftime('%Y%m%d-%H:%M:%S'), '下载任务停止')
```

### Comparing `hydrodatasource-0.0.1/hydrodatasource/downloader/gpm_downloader_auto.py` & `hydrodatasource-0.0.2/hydrodatasource/downloader/gpm_downloader_auto.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,246 +1,246 @@
-#!/home/zhujianfeng/.conda/envs/stac-test/bin/python
-
-import calendar
-import datetime
-import subprocess
-from pathlib import Path
-
-import s3fs
-import yaml
-
-from apscheduler.schedulers.blocking import BlockingScheduler  # 后台运行
-from minio import Minio
-
-
-work_dir = Path(__file__).resolve().parent
-with open(work_dir / 'privacy_config.yaml', 'r') as f:
-    privacy_config = yaml.safe_load(f)
-storage_options = {
-    'client_kwargs': {'endpoint_url': privacy_config['minio']['client_endpoint']},
-    'key': privacy_config['minio']['access_key'],
-    'secret': privacy_config['minio']['secret']
-}
-minioClient = Minio(storage_options['client_kwargs'],
-                    storage_options['key'],
-                    secret_key=privacy_config['minio']['secret'],
-                    secure=False)
-fs = s3fs.S3FileSystem(
-    client_kwargs={"endpoint_url": privacy_config['minio']['client_endpoint']},
-    key=privacy_config['minio']['access_key'],
-    secret=privacy_config['minio']['secret']
-)
-
-flist = []
-
-sc = BlockingScheduler(timezone="Asia/Shanghai")
-
-
-@sc.scheduled_job('cron', day_of_week='*', hour='*', minute='55', second='00')
-def gpm_downloader():
-    # f = open('log.txt', 'a', encoding='utf8')
-
-    date = datetime.datetime.now()
-    date = date + datetime.timedelta(hours=-14)
-    # date=date.strftime('%Y%m%d')
-
-    year = int(date.strftime('%Y'))
-    month = int(date.strftime('%m'))
-    day = int(date.strftime('%d'))
-    hour = int(date.strftime('%H'))
-
-    new = []
-    date = str(year) + str(month).zfill(2) + str(day).zfill(2)
-
-    for time in range(0, 2):
-        # time=time*30
-        # should.append(date+str(time).zfill(4))
-
-        # url='https://gpm1.gesdisc.eosdis.nasa.gov/daac-bin/OTF/HTTP_services.cgi?FILENAME=%2Fdata%2FGPM_L3%2FGPM_3IMERGHHE.06%2FYYYY%2FAAA%2F3B-HHR-E.MS.MRG.3IMERG.YYYYMMDD-SBBBBBB-ECCCCCC.EEEE.V06C.HDF5&FORMAT=bmM0Lw&BBOX=3%2C73%2C54%2C136&LABEL=3B-HHR-E.MS.MRG.3IMERG.YYYYMMDD-SBBBBBB-ECCCCCC.EEEE.V06C.HDF5.SUB.nc4&SHORTNAME=GPM_3IMERGHHE&SERVICE=L34RS_GPM&VERSION=1.02&DATASET_VERSION=06&VARIABLES=precipitationCal%2CrandomError%2CprecipitationUncal%2CIRkalmanFilterWeight%2CHQprecipSource%2CHQprecipitation%2CprobabilityLiquidPrecipitation%2CHQobservationTime%2CIRprecipitation'
-        # url='https://gpm1.gesdisc.eosdis.nasa.gov/opendap/GPM_L3/GPM_3IMERGHHE.06/YYYY/AAA/3B-HHR-E.MS.MRG.3IMERG.YYYYMMDD-SBBBBBB-ECCCCCC.EEEE.V06D.HDF5.nc4?IRkalmanFilterWeight%5B0:0%5D%5B2530:3159%5D%5B930:1439%5D,HQprecipSource%5B0:0%5D%5B2530:3159%5D%5B930:1439%5D,precipitationCal%5B0:0%5D%5B2530:3159%5D%5B930:1439%5D,precipitationUncal%5B0:0%5D%5B2530:3159%5D%5B930:1439%5D,HQprecipitation%5B0:0%5D%5B2530:3159%5D%5B930:1439%5D,probabilityLiquidPrecipitation%5B0:0%5D%5B2530:3159%5D%5B930:1439%5D,HQobservationTime%5B0:0%5D%5B2530:3159%5D%5B930:1439%5D,randomError%5B0:0%5D%5B2530:3159%5D%5B930:1439%5D,IRprecipitation%5B0:0%5D%5B2530:3159%5D%5B930:1439%5D,time,lon%5B2530:3159%5D,lat%5B930:1439%5D'
-        # url='https://gpm1.gesdisc.eosdis.nasa.gov/daac-bin/OTF/HTTP_services.cgi?FILENAME=%2Fdata%2FGPM_L3%2FGPM_3IMERGHHE.06%2F2023%2FAAA%2F3B-HHR-E.MS.MRG.3IMERG.YYYYMMDD-SBBBBBB-ECCCCCC.EEEE.V06D.HDF5&DATASET_VERSION=06&SERVICE=L34RS_GPM&FORMAT=bmM0Lw&SHORTNAME=GPM_3IMERGHHE&VERSION=1.02&VARIABLES=precipitationCal%2CrandomError%2CprecipitationUncal%2CIRkalmanFilterWeight%2CHQprecipSource%2CHQprecipitation%2CprobabilityLiquidPrecipitation%2CHQobservationTime%2CIRprecipitation&LABEL=3B-HHR-E.MS.MRG.3IMERG.YYYYMMDD-SBBBBBB-ECCCCCC.EEEE.V06D.HDF5.SUB.nc4&BBOX=3%2C73%2C54%2C136'
-        url = ('https://gpm1.gesdisc.eosdis.nasa.gov/daac-bin/OTF/HTTP_services.cgi?'
-               'FILENAME=%2Fdata%2FGPM_L3%2FGPM_3IMERGHHE.06%2FYYYY%2FAAA%2F3B-HHR-E.MS.MRG.3IMERG.YYYYMMDD-SBBBBBB'
-               '-ECCCCCC.EEEE.V06E.HDF5&VARIABLES=precipitationCal%2CrandomError%2CprecipitationUncal'
-               '%2CIRkalmanFilterWeight%2CHQprecipSource%2CHQprecipitation%2CprobabilityLiquidPrecipitation'
-               '%2CHQobservationTime%2CIRprecipitation&DATASET_VERSION=06&BBOX=3%2C73%2C54%2C136&SERVICE=L34RS_GPM'
-               '&VERSION=1.02&SHORTNAME=GPM_3IMERGHHE&FORMAT=bmM0Lw&LABEL=3B-HHR-E.MS.MRG.3IMERG.YYYYMMDD-SBBBBBB'
-               '-ECCCCCC.EEEE.V06E.HDF5.SUB.nc4')
-
-        YYYY = str(year)
-        MM = str(month).zfill(2)
-        DD = str(day).zfill(2)
-
-        AAA = str(daynum(year, month, day)).zfill(3)
-
-        EEEE = str(hour * 60 + time * 30).zfill(4)
-
-        start = int(hour * 10000 + time * 30 * 100)
-        BBBBBB = str(start).zfill(6)
-
-        end = int(start + 2959)
-        CCCCCC = str(end).zfill(6)
-
-        url = url.replace('YYYY', YYYY).replace('MM', MM).replace('DD', DD).replace('AAA', AAA).replace('EEEE',
-                                                                                                        EEEE).replace(
-            'BBBBBB', BBBBBB).replace('CCCCCC', CCCCCC)
-        # print(url)
-        # break
-        new.append(url)
-
-    with open('./gpm.txt', mode='w') as gpm:
-        [gpm.write(str(url) + '\n') for url in new]
-
-    subprocess.run("cat gpm.txt | tr -d '\r' | xargs -n 1 curl -LJO -n -c ~/.urs_cookies -b ~/.urs_cookies", shell=True)
-
-    flist = []
-    upload()
-
-    update()
-
-    print(datetime.datetime.now().strftime('%Y%m%d-%H:%M:%S'), '定时任务成功执行')
-    # print(datetime.datetime.now().strftime('%Y%m%d-%H:%M:%S'),'定时任务成功执行',file=f)
-
-    # f.close()
-
-
-def daynum(year, month, day):
-    totalday = 0
-    if calendar.isleap(year):
-        days = [31, 29, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31]
-    else:
-        days = [31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31]
-    for i in range(1, 13):
-        if i == month:
-            for j in range(1, i):
-                totalday = totalday + days[j - 1]
-    totalday = totalday + day
-    return totalday
-
-
-def upload():
-    for root, dirs, filenames in os.walk('.'):
-        for filename in filenames:
-
-            if ".nc4" in filename and "2024" in filename:
-
-                gpm_date = filename[23:31]
-                year = gpm_date[0:4]
-                month = gpm_date[4:6]
-                day = gpm_date[6:8]
-
-                minio_path = f'geodata/gpm/{year}/{month}/{day}/{filename}'
-
-                # print(minio_path)
-
-                # # minio_path = minio_path.replace('_land','')
-
-                try:
-                    print(minioClient.fput_object('watermodel-pub', minio_path, os.path.join(root, filename)))
-                    flist.append(minio_path)
-                    if not os.path.exists(f"/ftproot/geodata/gpm_30m/{year}"):
-                        os.mkdir(f"/ftproot/geodata/gpm_30m/{year}")
-                    os.system(f"mv {filename} /ftproot/geodata/gpm_30m/{year}")
-                except Exception as err:
-                    print(err)
-
-
-import kerchunk.hdf
-
-import os
-import ujson
-import json
-
-so = dict(mode='rb', storage_options=storage_options, default_fill_cache=False,
-          default_cache_type='first')  # args to fs.open()
-
-
-# default_fill_cache=False avoids caching data in between file chunks to lowers memory usage.
-
-def gen_json(file_url):
-    with fs.open(file_url, **so) as infile:
-        # print(file_url)
-        try:
-            h5chunks = kerchunk.hdf.SingleHdf5ToZarr(infile, file_url)
-        except:
-            f = open('zarrmissed.txt', mode='a')
-            print(file_url, file=f)
-            f.close()
-            return
-
-        outf = file_url[:-4] + '.json'  # file name to save json to
-        outf = outf.replace('watermodel-pub', 'test')
-        with fs.open(outf, 'wb') as f:
-            f.write(ujson.dumps(h5chunks.translate()).encode());
-
-
-def single_json(nc_list):
-    for file in nc_list:
-        gen_json(file)
-
-
-from kerchunk.combine import MultiZarrToZarr
-
-
-def multi_json(flist):
-    # print('multi_json')
-
-    flist.sort()
-    lasted = flist[-1]
-
-    filename = lasted.split('/')[-1]
-
-    gpm_date = filename[23:39]
-    yyyy = gpm_date[0:4]
-    mm = gpm_date[4:6]
-    dd = gpm_date[6:8]
-    hh = gpm_date[10:12]
-    mi = gpm_date[12:14]
-    ss = gpm_date[14:16]
-
-    json_list = fs.glob(f"test/geodata/gpm/{yyyy}/{mm}/*/*.json")
-    json_list = ['s3://' + str for str in json_list]
-
-    mzz = MultiZarrToZarr(
-        json_list,
-        target_options=storage_options,
-        remote_protocol='s3',
-        remote_options=storage_options,
-        concat_dims=['time'],
-        identical_dims=['lat', 'lon']
-    )
-
-    d = mzz.translate()
-
-    # output = f's3://test/geodata/gpm/{yyyy}/{mm}/gpm{yyyy}{mm}_{dd}.json'
-    output = f's3://test/geodata/gpm/{yyyy}/{mm}/gpm{yyyy}{mm}_inc.json'
-    # days = calendar.monthrange(int(yyyy),int(mm))[1]
-    # if int(dd)==days and hh=='23' and mi=='30':
-    #     output = f's3://test/geodata/gpm/{yyyy}/{mm}/gpm{yyyy}{mm}_inc.json'
-    with fs.open(output, 'wb') as f:
-        f.write(ujson.dumps(d).encode())
-    print(output, "写入成功！")
-
-    with fs.open('test/geodata/gpm/gpm.json') as f:
-        cont = json.load(f)
-    cont['end'] = f'{yyyy}-{mm}-{dd}T{hh}:{mi}:00.000000000'
-    with fs.open('test/geodata/gpm/gpm.json', 'w') as f:
-        json.dump(cont, f)
-    print('更新至', filename)
-
-
-def update():
-    nc_list = ['watermodel-pub/' + str for str in flist]
-    single_json(nc_list)
-
-    multi_json(flist)
-
-
-if __name__ == '__main__':
-
-    try:
-        sc.start()
-
-    except Exception as e:
-        sc.shutdown()
-        print(datetime.datetime.now().strftime('%Y%m%d-%H:%M:%S'), '下载任务停止')
-        # print(datetime.datetime.now().strftime('%Y%m%d-%H:%M:%S'),'下载任务停止',file=f)
+#!/home/zhujianfeng/.conda/envs/stac-test/bin/python
+
+import calendar
+import datetime
+import subprocess
+from pathlib import Path
+
+import s3fs
+import yaml
+
+from apscheduler.schedulers.blocking import BlockingScheduler  # 后台运行
+from minio import Minio
+
+
+work_dir = Path(__file__).resolve().parent
+with open(work_dir / 'privacy_config.yaml', 'r') as f:
+    privacy_config = yaml.safe_load(f)
+storage_options = {
+    'client_kwargs': {'endpoint_url': privacy_config['minio']['client_endpoint']},
+    'key': privacy_config['minio']['access_key'],
+    'secret': privacy_config['minio']['secret']
+}
+minioClient = Minio(storage_options['client_kwargs'],
+                    storage_options['key'],
+                    secret_key=privacy_config['minio']['secret'],
+                    secure=False)
+fs = s3fs.S3FileSystem(
+    client_kwargs={"endpoint_url": privacy_config['minio']['client_endpoint']},
+    key=privacy_config['minio']['access_key'],
+    secret=privacy_config['minio']['secret']
+)
+
+flist = []
+
+sc = BlockingScheduler(timezone="Asia/Shanghai")
+
+
+@sc.scheduled_job('cron', day_of_week='*', hour='*', minute='55', second='00')
+def gpm_downloader():
+    # f = open('log.txt', 'a', encoding='utf8')
+
+    date = datetime.datetime.now()
+    date = date + datetime.timedelta(hours=-14)
+    # date=date.strftime('%Y%m%d')
+
+    year = int(date.strftime('%Y'))
+    month = int(date.strftime('%m'))
+    day = int(date.strftime('%d'))
+    hour = int(date.strftime('%H'))
+
+    new = []
+    date = str(year) + str(month).zfill(2) + str(day).zfill(2)
+
+    for time in range(0, 2):
+        # time=time*30
+        # should.append(date+str(time).zfill(4))
+
+        # url='https://gpm1.gesdisc.eosdis.nasa.gov/daac-bin/OTF/HTTP_services.cgi?FILENAME=%2Fdata%2FGPM_L3%2FGPM_3IMERGHHE.06%2FYYYY%2FAAA%2F3B-HHR-E.MS.MRG.3IMERG.YYYYMMDD-SBBBBBB-ECCCCCC.EEEE.V06C.HDF5&FORMAT=bmM0Lw&BBOX=3%2C73%2C54%2C136&LABEL=3B-HHR-E.MS.MRG.3IMERG.YYYYMMDD-SBBBBBB-ECCCCCC.EEEE.V06C.HDF5.SUB.nc4&SHORTNAME=GPM_3IMERGHHE&SERVICE=L34RS_GPM&VERSION=1.02&DATASET_VERSION=06&VARIABLES=precipitationCal%2CrandomError%2CprecipitationUncal%2CIRkalmanFilterWeight%2CHQprecipSource%2CHQprecipitation%2CprobabilityLiquidPrecipitation%2CHQobservationTime%2CIRprecipitation'
+        # url='https://gpm1.gesdisc.eosdis.nasa.gov/opendap/GPM_L3/GPM_3IMERGHHE.06/YYYY/AAA/3B-HHR-E.MS.MRG.3IMERG.YYYYMMDD-SBBBBBB-ECCCCCC.EEEE.V06D.HDF5.nc4?IRkalmanFilterWeight%5B0:0%5D%5B2530:3159%5D%5B930:1439%5D,HQprecipSource%5B0:0%5D%5B2530:3159%5D%5B930:1439%5D,precipitationCal%5B0:0%5D%5B2530:3159%5D%5B930:1439%5D,precipitationUncal%5B0:0%5D%5B2530:3159%5D%5B930:1439%5D,HQprecipitation%5B0:0%5D%5B2530:3159%5D%5B930:1439%5D,probabilityLiquidPrecipitation%5B0:0%5D%5B2530:3159%5D%5B930:1439%5D,HQobservationTime%5B0:0%5D%5B2530:3159%5D%5B930:1439%5D,randomError%5B0:0%5D%5B2530:3159%5D%5B930:1439%5D,IRprecipitation%5B0:0%5D%5B2530:3159%5D%5B930:1439%5D,time,lon%5B2530:3159%5D,lat%5B930:1439%5D'
+        # url='https://gpm1.gesdisc.eosdis.nasa.gov/daac-bin/OTF/HTTP_services.cgi?FILENAME=%2Fdata%2FGPM_L3%2FGPM_3IMERGHHE.06%2F2023%2FAAA%2F3B-HHR-E.MS.MRG.3IMERG.YYYYMMDD-SBBBBBB-ECCCCCC.EEEE.V06D.HDF5&DATASET_VERSION=06&SERVICE=L34RS_GPM&FORMAT=bmM0Lw&SHORTNAME=GPM_3IMERGHHE&VERSION=1.02&VARIABLES=precipitationCal%2CrandomError%2CprecipitationUncal%2CIRkalmanFilterWeight%2CHQprecipSource%2CHQprecipitation%2CprobabilityLiquidPrecipitation%2CHQobservationTime%2CIRprecipitation&LABEL=3B-HHR-E.MS.MRG.3IMERG.YYYYMMDD-SBBBBBB-ECCCCCC.EEEE.V06D.HDF5.SUB.nc4&BBOX=3%2C73%2C54%2C136'
+        url = ('https://gpm1.gesdisc.eosdis.nasa.gov/daac-bin/OTF/HTTP_services.cgi?'
+               'FILENAME=%2Fdata%2FGPM_L3%2FGPM_3IMERGHHE.06%2FYYYY%2FAAA%2F3B-HHR-E.MS.MRG.3IMERG.YYYYMMDD-SBBBBBB'
+               '-ECCCCCC.EEEE.V06E.HDF5&VARIABLES=precipitationCal%2CrandomError%2CprecipitationUncal'
+               '%2CIRkalmanFilterWeight%2CHQprecipSource%2CHQprecipitation%2CprobabilityLiquidPrecipitation'
+               '%2CHQobservationTime%2CIRprecipitation&DATASET_VERSION=06&BBOX=3%2C73%2C54%2C136&SERVICE=L34RS_GPM'
+               '&VERSION=1.02&SHORTNAME=GPM_3IMERGHHE&FORMAT=bmM0Lw&LABEL=3B-HHR-E.MS.MRG.3IMERG.YYYYMMDD-SBBBBBB'
+               '-ECCCCCC.EEEE.V06E.HDF5.SUB.nc4')
+
+        YYYY = str(year)
+        MM = str(month).zfill(2)
+        DD = str(day).zfill(2)
+
+        AAA = str(daynum(year, month, day)).zfill(3)
+
+        EEEE = str(hour * 60 + time * 30).zfill(4)
+
+        start = int(hour * 10000 + time * 30 * 100)
+        BBBBBB = str(start).zfill(6)
+
+        end = int(start + 2959)
+        CCCCCC = str(end).zfill(6)
+
+        url = url.replace('YYYY', YYYY).replace('MM', MM).replace('DD', DD).replace('AAA', AAA).replace('EEEE',
+                                                                                                        EEEE).replace(
+            'BBBBBB', BBBBBB).replace('CCCCCC', CCCCCC)
+        # print(url)
+        # break
+        new.append(url)
+
+    with open('./gpm.txt', mode='w') as gpm:
+        [gpm.write(str(url) + '\n') for url in new]
+
+    subprocess.run("cat gpm.txt | tr -d '\r' | xargs -n 1 curl -LJO -n -c ~/.urs_cookies -b ~/.urs_cookies", shell=True)
+
+    flist = []
+    upload()
+
+    update()
+
+    print(datetime.datetime.now().strftime('%Y%m%d-%H:%M:%S'), '定时任务成功执行')
+    # print(datetime.datetime.now().strftime('%Y%m%d-%H:%M:%S'),'定时任务成功执行',file=f)
+
+    # f.close()
+
+
+def daynum(year, month, day):
+    totalday = 0
+    if calendar.isleap(year):
+        days = [31, 29, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31]
+    else:
+        days = [31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31]
+    for i in range(1, 13):
+        if i == month:
+            for j in range(1, i):
+                totalday = totalday + days[j - 1]
+    totalday = totalday + day
+    return totalday
+
+
+def upload():
+    for root, dirs, filenames in os.walk('.'):
+        for filename in filenames:
+
+            if ".nc4" in filename and "2024" in filename:
+
+                gpm_date = filename[23:31]
+                year = gpm_date[0:4]
+                month = gpm_date[4:6]
+                day = gpm_date[6:8]
+
+                minio_path = f'geodata/gpm/{year}/{month}/{day}/{filename}'
+
+                # print(minio_path)
+
+                # # minio_path = minio_path.replace('_land','')
+
+                try:
+                    print(minioClient.fput_object('watermodel-pub', minio_path, os.path.join(root, filename)))
+                    flist.append(minio_path)
+                    if not os.path.exists(f"/ftproot/geodata/gpm_30m/{year}"):
+                        os.mkdir(f"/ftproot/geodata/gpm_30m/{year}")
+                    os.system(f"mv {filename} /ftproot/geodata/gpm_30m/{year}")
+                except Exception as err:
+                    print(err)
+
+
+import kerchunk.hdf
+
+import os
+import ujson
+import json
+
+so = dict(mode='rb', storage_options=storage_options, default_fill_cache=False,
+          default_cache_type='first')  # args to fs.open()
+
+
+# default_fill_cache=False avoids caching data in between file chunks to lowers memory usage.
+
+def gen_json(file_url):
+    with fs.open(file_url, **so) as infile:
+        # print(file_url)
+        try:
+            h5chunks = kerchunk.hdf.SingleHdf5ToZarr(infile, file_url)
+        except:
+            f = open('zarrmissed.txt', mode='a')
+            print(file_url, file=f)
+            f.close()
+            return
+
+        outf = file_url[:-4] + '.json'  # file name to save json to
+        outf = outf.replace('watermodel-pub', 'test')
+        with fs.open(outf, 'wb') as f:
+            f.write(ujson.dumps(h5chunks.translate()).encode());
+
+
+def single_json(nc_list):
+    for file in nc_list:
+        gen_json(file)
+
+
+from kerchunk.combine import MultiZarrToZarr
+
+
+def multi_json(flist):
+    # print('multi_json')
+
+    flist.sort()
+    lasted = flist[-1]
+
+    filename = lasted.split('/')[-1]
+
+    gpm_date = filename[23:39]
+    yyyy = gpm_date[0:4]
+    mm = gpm_date[4:6]
+    dd = gpm_date[6:8]
+    hh = gpm_date[10:12]
+    mi = gpm_date[12:14]
+    ss = gpm_date[14:16]
+
+    json_list = fs.glob(f"test/geodata/gpm/{yyyy}/{mm}/*/*.json")
+    json_list = ['s3://' + str for str in json_list]
+
+    mzz = MultiZarrToZarr(
+        json_list,
+        target_options=storage_options,
+        remote_protocol='s3',
+        remote_options=storage_options,
+        concat_dims=['time'],
+        identical_dims=['lat', 'lon']
+    )
+
+    d = mzz.translate()
+
+    # output = f's3://test/geodata/gpm/{yyyy}/{mm}/gpm{yyyy}{mm}_{dd}.json'
+    output = f's3://test/geodata/gpm/{yyyy}/{mm}/gpm{yyyy}{mm}_inc.json'
+    # days = calendar.monthrange(int(yyyy),int(mm))[1]
+    # if int(dd)==days and hh=='23' and mi=='30':
+    #     output = f's3://test/geodata/gpm/{yyyy}/{mm}/gpm{yyyy}{mm}_inc.json'
+    with fs.open(output, 'wb') as f:
+        f.write(ujson.dumps(d).encode())
+    print(output, "写入成功！")
+
+    with fs.open('test/geodata/gpm/gpm.json') as f:
+        cont = json.load(f)
+    cont['end'] = f'{yyyy}-{mm}-{dd}T{hh}:{mi}:00.000000000'
+    with fs.open('test/geodata/gpm/gpm.json', 'w') as f:
+        json.dump(cont, f)
+    print('更新至', filename)
+
+
+def update():
+    nc_list = ['watermodel-pub/' + str for str in flist]
+    single_json(nc_list)
+
+    multi_json(flist)
+
+
+if __name__ == '__main__':
+
+    try:
+        sc.start()
+
+    except Exception as e:
+        sc.shutdown()
+        print(datetime.datetime.now().strftime('%Y%m%d-%H:%M:%S'), '下载任务停止')
+        # print(datetime.datetime.now().strftime('%Y%m%d-%H:%M:%S'),'下载任务停止',file=f)
```

### Comparing `hydrodatasource-0.0.1/hydrodatasource/downloader/minio.py` & `hydrodatasource-0.0.2/hydrodatasource/downloader/minio.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,386 +1,386 @@
-"""
-该模块用于获取minio服务器中的数据列表，包括：
-
-- `Era5_land`
-- `GPM_IMERG_Early`
-- `GFS_atmos`
-"""
-
-from ..configs.config import MINIO_PARAM
-from ..configs.config import FS
-import os
-import numpy as np
-import pandas as pd
-import geopandas as gpd
-import json
-
-
-class ERA5LCatalog:
-    """
-    用于获取era5-land的数据源信息，并搜索minio服务器中的数据范围
-
-    Attributes:
-        collection_id (str): 数据集名称
-        data_sources (str): 数据源
-        description (str): 数据源链接
-        spatial_resolution (str): 空间分辨率
-        temporal_resolution (str): 时间分辨率
-        datasets (dict): minio服务器中的已有数据集
-
-    Method:
-        search(aoi, start_time, end_time): 搜索minio服务器中的数据范围
-    """
-
-    def __init__(self):
-        self._collection_id = "era5-land"
-        self._datasources = "ECMWF"
-        self._description = "https://cds.climate.copernicus.eu/cdsapp#!/dataset/reanalysis-era5-land?tab=overview"
-        self._spatialresolution = "0.1 x 0.1; Native resolution is 9 km."
-        self._temporalresolution = "hourly"
-        self._datasets = self._get_datasets()
-        self._bucket_name = "test"
-
-    def _get_datasets(self):
-        dss = {}
-        ds = {}
-        with FS.open(os.path.join(self._bucket_name, "geodata/era5_land/era5l.json")) as f:
-            era5 = json.load(f)
-            ds["start_time"] = np.datetime64(era5["start"])
-            ds["end_time"] = np.datetime64(era5["end"])
-            ds["bbox"] = era5["bbox"]
-        dss["wis"] = ds
-        return dss
-
-    @property
-    def collection_id(self):
-        return self._collection_id
-
-    @property
-    def data_sources(self):
-        return self._datasources
-
-    @property
-    def description(self):
-        return self._description
-
-    @property
-    def spatial_resolution(self):
-        return self._spatialresolution
-
-    @property
-    def temporal_resolution(self):
-        return self._temporalresolution
-
-    @property
-    def datasets(self):
-        return self._datasets
-
-    def search(self, aoi, start_time=None, end_time=None):
-        """
-        查询并获取数据清单
-
-        Args:
-            aoi (GeoDataFrame): 矢量数据范围
-            strt_time (datatime64): 查询的起始时间
-            end_time (datatime64): 查询的终止时间
-
-        Returns:
-            datalist (GeoDataFrame): 符合条件的数据清单
-        """
-
-        clips = []
-
-        for key, value in self._datasets.items():
-            start = start_time
-            end = end_time
-            if start_time is None:
-                start = value["start_time"]
-            if end_time is None:
-                end = value["end_time"]
-
-            if start < value["start_time"]:
-                start = value["start_time"]
-            if end > value["end_time"]:
-                end = value["end_time"]
-
-            if start <= end:
-                df = pd.DataFrame(
-                    {
-                        "id": [self._collection_id],
-                        "dataset": [key],
-                        "start_time": [str(start)],
-                        "end_time": [str(end)],
-                        "geometry": [
-                            f"POLYGON(({value['bbox'][0]} {value['bbox'][3]},{value['bbox'][0]} {value['bbox'][1]},\
-                                     {value['bbox'][2]} {value['bbox'][1]},{value['bbox'][2]} {value['bbox'][3]},{value['bbox'][0]} {value['bbox'][3]}))"
-                        ],
-                    }
-                )
-                df["geometry"] = gpd.GeoSeries.from_wkt(df["geometry"])
-                gdf = gpd.GeoDataFrame(df, geometry="geometry", crs="EPSG:4326")
-
-                clips.append(gdf.clip(aoi))
-
-        return pd.concat(clips)
-
-
-class GPMCatalog:
-    """
-    用于获取gpm的数据源信息，并搜索minio服务器中的数据范围
-
-    Attributes:
-        collection_id (str): 数据集名称
-        data_sources (str): 数据源
-        description (str): 数据源链接
-        spatial_resolution (str): 空间分辨率
-        temporal_resolution (str): 时间分辨率
-        datasets (dict): minio服务器中的已有数据集
-
-    Method:
-        search(aoi, start_time, end_time): 搜索minio服务器中的数据范围
-    """
-
-    def __init__(self):
-        self._collection_id = "gpm-imerg-early"
-        self._datasources = "NASA & JAXA"
-        self._description = (
-            "https://disc.gsfc.nasa.gov/datasets/GPM_3IMERGHHE_06/summary"
-        )
-        self._spatialresolution = "0.1 x 0.1; Native resolution is 9 km. (60°S-60°N)"
-        self._temporalresolution = "half-hourly; 1 day"
-        self._bucket_name = "test"
-        self._datasets = self._get_datasets()
-
-    def _get_datasets(self):
-        dss = {}
-        lds = []
-        ds = {}
-        with FS.open(os.path.join(self._bucket_name, "geodata/gpm/gpm.json")) as f:
-            gpm = json.load(f)
-            ds["time_resolution"] = "30 minutes"
-            ds["start_time"] = np.datetime64(gpm["start"])
-            ds["end_time"] = np.datetime64(gpm["end"])
-            ds["bbox"] = gpm["bbox"]
-        lds.append(ds)
-
-        ds = {}
-        with FS.open(os.path.join(self._bucket_name, "geodata/gpm1d/gpm1d.json")) as f:
-            gpm = json.load(f)
-            ds["time_resolution"] = "1 day"
-            ds["start_time"] = np.datetime64(gpm["start"])
-            ds["end_time"] = np.datetime64(gpm["end"])
-            ds["bbox"] = gpm["bbox"]
-        lds.append(ds)
-        dss["wis"] = lds
-
-        lds = []
-        ds = {}
-        with FS.open(os.path.join(self._bucket_name, "camdata/gpm/gpm.json")) as f:
-            gpm = json.load(f)
-            ds["time_resolution"] = "30 minutes"
-            ds["start_time"] = np.datetime64(gpm["start"])
-            ds["end_time"] = np.datetime64(gpm["end"])
-            ds["bbox"] = gpm["bbox"]
-        lds.append(ds)
-
-        ds = {}
-        with FS.open(os.path.join(self._bucket_name, "camdata/gpm1d/gpm1d.json")) as f:
-            gpm = json.load(f)
-            ds["time_resolution"] = "1 day"
-            ds["start_time"] = np.datetime64(gpm["start"])
-            ds["end_time"] = np.datetime64(gpm["end"])
-            ds["bbox"] = gpm["bbox"]
-        lds.append(ds)
-        dss["camels"] = lds
-
-        return dss
-
-    @property
-    def collection_id(self):
-        return self._collection_id
-
-    @property
-    def data_sources(self):
-        return self._datasources
-
-    @property
-    def description(self):
-        return self._description
-
-    @property
-    def spatial_resolution(self):
-        return self._spatialresolution
-
-    @property
-    def temporal_resolution(self):
-        return self._temporalresolution
-
-    @property
-    def datasets(self):
-        return self._datasets
-
-    def search(self, aoi, start_time=None, end_time=None):
-        """
-        查询并获取数据清单
-
-        Args:
-            aoi (GeoDataFrame): 矢量数据范围
-            strt_time (datatime64): 查询的起始时间
-            end_time (datatime64): 查询的终止时间
-
-        Returns:
-            datalist (GeoDataFrame): 符合条件的数据清单
-        """
-
-        clips = []
-
-        for key, value in self._datasets.items():
-            for v in value:
-                start = start_time
-                end = end_time
-                if start_time is None:
-                    start = v["start_time"]
-                if end_time is None:
-                    end = v["end_time"]
-
-                if start < v["start_time"]:
-                    start = v["start_time"]
-                if end > v["end_time"]:
-                    end = v["end_time"]
-
-                if start <= end:
-                    df = pd.DataFrame(
-                        {
-                            "id": [self._collection_id],
-                            "dataset": [key],
-                            "time_resolution": v["time_resolution"],
-                            "start_time": [str(start)],
-                            "end_time": [str(end)],
-                            "geometry": [
-                                f"POLYGON(({v['bbox'][0]} {v['bbox'][3]},{v['bbox'][0]} {v['bbox'][1]},\
-                                         {v['bbox'][2]} {v['bbox'][1]},{v['bbox'][2]} {v['bbox'][3]},{v['bbox'][0]} {v['bbox'][3]}))"
-                            ],
-                        }
-                    )
-                    df["geometry"] = gpd.GeoSeries.from_wkt(df["geometry"])
-                    gdf = gpd.GeoDataFrame(df, geometry="geometry", crs="EPSG:4326")
-
-                    clips.append(gdf.clip(aoi))
-
-        return pd.concat(clips)
-
-
-class GFSCatalog:
-    """
-    用于获取gfs的数据源信息，并搜索minio服务器中的数据范围
-
-    Attributes:
-        collection_id (str): 数据集名称
-        data_sources (str): 数据源
-        description (str): 数据源链接
-        spatial_resolution (str): 空间分辨率
-        temporal_resolution (str): 时间分辨率
-        datasets (dict): minio服务器中的已有数据集
-
-    Method:
-        search(aoi, start_time, end_time): 搜索minio服务器中的数据范围
-    """
-
-    def __init__(self, variable="tp"):
-        self._variable = variable
-        self._collection_id = f"gfs_atmos.{variable}"
-        self._datasources = "NOAA"
-        self._description = (
-            "https://www.emc.ncep.noaa.gov/emc/pages/numerical_forecast_systems/gfs.php"
-        )
-        self._spatialresolution = "0.25 x 0.25"
-        self._temporalresolution = "hourly; 1-120h"
-        self._bucket_name = "test"
-        self._datasets = self._get_datasets()
-
-    def _get_datasets(self):
-        dss = {}
-
-        ds = {}
-        with FS.open(os.path.join(self._bucket_name, "geodata/gfs/gfs.json")) as f:
-            gfs = json.load(f)
-        dss["wis"] = gfs[self._variable]
-
-        return dss
-
-    @property
-    def variable(self):
-        return self._variable
-
-    @property
-    def collection_id(self):
-        return self._collection_id
-
-    @property
-    def data_sources(self):
-        return self._datasources
-
-    @property
-    def description(self):
-        return self._description
-
-    @property
-    def spatial_resolution(self):
-        return self._spatialresolution
-
-    @property
-    def temporal_resolution(self):
-        return self._temporalresolution
-
-    @property
-    def datasets(self):
-        return self._datasets
-
-    def search(self, aoi, start_time=None, end_time=None):
-        """
-        查询并获取数据清单
-
-        Args:
-            aoi (GeoDataFrame): 矢量数据范围
-            start_time (datatime64): 查询的起始时间
-            end_time (datatime64): 查询的终止时间
-
-        Returns:
-            datalist (GeoDataFrame): 符合条件的数据清单
-        """
-
-        clips = []
-
-        for key, value in self._datasets.items():
-            for v in value:
-                start = start_time
-                end = end_time
-                if start_time is None:
-                    start = np.datetime64(v["start"])
-                if end_time is None:
-                    end = np.datetime64(v["end"])
-
-                if start < np.datetime64(v["start"]):
-                    start = np.datetime64(v["start"])
-
-                if end > np.datetime64(v["end"]):
-                    end = np.datetime64(v["end"])
-
-                if start <= end:
-                    df = pd.DataFrame(
-                        {
-                            "id": [self._collection_id],
-                            "dataset": [key],
-                            "start_time": [str(start)],
-                            "end_time": [str(end)],
-                            "geometry": [
-                                f"POLYGON(({v['bbox'][0]} {v['bbox'][3]},{v['bbox'][0]} {v['bbox'][1]},{v['bbox'][2]} {v['bbox'][1]},{v['bbox'][2]} {v['bbox'][3]},{v['bbox'][0]} {v['bbox'][3]}))"
-                            ],
-                        }
-                    )
-                    df["geometry"] = gpd.GeoSeries.from_wkt(df["geometry"])
-                    gdf = gpd.GeoDataFrame(df, geometry="geometry", crs="EPSG:4326")
-
-                    clips.append(gdf.clip(aoi))
-
-        return pd.concat(clips)
+"""
+该模块用于获取minio服务器中的数据列表，包括：
+
+- `Era5_land`
+- `GPM_IMERG_Early`
+- `GFS_atmos`
+"""
+
+from ..configs.config import MINIO_PARAM
+from ..configs.config import FS
+import os
+import numpy as np
+import pandas as pd
+import geopandas as gpd
+import json
+
+
+class ERA5LCatalog:
+    """
+    用于获取era5-land的数据源信息，并搜索minio服务器中的数据范围
+
+    Attributes:
+        collection_id (str): 数据集名称
+        data_sources (str): 数据源
+        description (str): 数据源链接
+        spatial_resolution (str): 空间分辨率
+        temporal_resolution (str): 时间分辨率
+        datasets (dict): minio服务器中的已有数据集
+
+    Method:
+        search(aoi, start_time, end_time): 搜索minio服务器中的数据范围
+    """
+
+    def __init__(self):
+        self._collection_id = "era5-land"
+        self._datasources = "ECMWF"
+        self._description = "https://cds.climate.copernicus.eu/cdsapp#!/dataset/reanalysis-era5-land?tab=overview"
+        self._spatialresolution = "0.1 x 0.1; Native resolution is 9 km."
+        self._temporalresolution = "hourly"
+        self._datasets = self._get_datasets()
+        self._bucket_name = "test"
+
+    def _get_datasets(self):
+        dss = {}
+        ds = {}
+        with FS.open(os.path.join(self._bucket_name, "geodata/era5_land/era5l.json")) as f:
+            era5 = json.load(f)
+            ds["start_time"] = np.datetime64(era5["start"])
+            ds["end_time"] = np.datetime64(era5["end"])
+            ds["bbox"] = era5["bbox"]
+        dss["wis"] = ds
+        return dss
+
+    @property
+    def collection_id(self):
+        return self._collection_id
+
+    @property
+    def data_sources(self):
+        return self._datasources
+
+    @property
+    def description(self):
+        return self._description
+
+    @property
+    def spatial_resolution(self):
+        return self._spatialresolution
+
+    @property
+    def temporal_resolution(self):
+        return self._temporalresolution
+
+    @property
+    def datasets(self):
+        return self._datasets
+
+    def search(self, aoi, start_time=None, end_time=None):
+        """
+        查询并获取数据清单
+
+        Args:
+            aoi (GeoDataFrame): 矢量数据范围
+            strt_time (datatime64): 查询的起始时间
+            end_time (datatime64): 查询的终止时间
+
+        Returns:
+            datalist (GeoDataFrame): 符合条件的数据清单
+        """
+
+        clips = []
+
+        for key, value in self._datasets.items():
+            start = start_time
+            end = end_time
+            if start_time is None:
+                start = value["start_time"]
+            if end_time is None:
+                end = value["end_time"]
+
+            if start < value["start_time"]:
+                start = value["start_time"]
+            if end > value["end_time"]:
+                end = value["end_time"]
+
+            if start <= end:
+                df = pd.DataFrame(
+                    {
+                        "id": [self._collection_id],
+                        "dataset": [key],
+                        "start_time": [str(start)],
+                        "end_time": [str(end)],
+                        "geometry": [
+                            f"POLYGON(({value['bbox'][0]} {value['bbox'][3]},{value['bbox'][0]} {value['bbox'][1]},\
+                                     {value['bbox'][2]} {value['bbox'][1]},{value['bbox'][2]} {value['bbox'][3]},{value['bbox'][0]} {value['bbox'][3]}))"
+                        ],
+                    }
+                )
+                df["geometry"] = gpd.GeoSeries.from_wkt(df["geometry"])
+                gdf = gpd.GeoDataFrame(df, geometry="geometry", crs="EPSG:4326")
+
+                clips.append(gdf.clip(aoi))
+
+        return pd.concat(clips)
+
+
+class GPMCatalog:
+    """
+    用于获取gpm的数据源信息，并搜索minio服务器中的数据范围
+
+    Attributes:
+        collection_id (str): 数据集名称
+        data_sources (str): 数据源
+        description (str): 数据源链接
+        spatial_resolution (str): 空间分辨率
+        temporal_resolution (str): 时间分辨率
+        datasets (dict): minio服务器中的已有数据集
+
+    Method:
+        search(aoi, start_time, end_time): 搜索minio服务器中的数据范围
+    """
+
+    def __init__(self):
+        self._collection_id = "gpm-imerg-early"
+        self._datasources = "NASA & JAXA"
+        self._description = (
+            "https://disc.gsfc.nasa.gov/datasets/GPM_3IMERGHHE_06/summary"
+        )
+        self._spatialresolution = "0.1 x 0.1; Native resolution is 9 km. (60°S-60°N)"
+        self._temporalresolution = "half-hourly; 1 day"
+        self._bucket_name = "test"
+        self._datasets = self._get_datasets()
+
+    def _get_datasets(self):
+        dss = {}
+        lds = []
+        ds = {}
+        with FS.open(os.path.join(self._bucket_name, "geodata/gpm/gpm.json")) as f:
+            gpm = json.load(f)
+            ds["time_resolution"] = "30 minutes"
+            ds["start_time"] = np.datetime64(gpm["start"])
+            ds["end_time"] = np.datetime64(gpm["end"])
+            ds["bbox"] = gpm["bbox"]
+        lds.append(ds)
+
+        ds = {}
+        with FS.open(os.path.join(self._bucket_name, "geodata/gpm1d/gpm1d.json")) as f:
+            gpm = json.load(f)
+            ds["time_resolution"] = "1 day"
+            ds["start_time"] = np.datetime64(gpm["start"])
+            ds["end_time"] = np.datetime64(gpm["end"])
+            ds["bbox"] = gpm["bbox"]
+        lds.append(ds)
+        dss["wis"] = lds
+
+        lds = []
+        ds = {}
+        with FS.open(os.path.join(self._bucket_name, "camdata/gpm/gpm.json")) as f:
+            gpm = json.load(f)
+            ds["time_resolution"] = "30 minutes"
+            ds["start_time"] = np.datetime64(gpm["start"])
+            ds["end_time"] = np.datetime64(gpm["end"])
+            ds["bbox"] = gpm["bbox"]
+        lds.append(ds)
+
+        ds = {}
+        with FS.open(os.path.join(self._bucket_name, "camdata/gpm1d/gpm1d.json")) as f:
+            gpm = json.load(f)
+            ds["time_resolution"] = "1 day"
+            ds["start_time"] = np.datetime64(gpm["start"])
+            ds["end_time"] = np.datetime64(gpm["end"])
+            ds["bbox"] = gpm["bbox"]
+        lds.append(ds)
+        dss["camels"] = lds
+
+        return dss
+
+    @property
+    def collection_id(self):
+        return self._collection_id
+
+    @property
+    def data_sources(self):
+        return self._datasources
+
+    @property
+    def description(self):
+        return self._description
+
+    @property
+    def spatial_resolution(self):
+        return self._spatialresolution
+
+    @property
+    def temporal_resolution(self):
+        return self._temporalresolution
+
+    @property
+    def datasets(self):
+        return self._datasets
+
+    def search(self, aoi, start_time=None, end_time=None):
+        """
+        查询并获取数据清单
+
+        Args:
+            aoi (GeoDataFrame): 矢量数据范围
+            strt_time (datatime64): 查询的起始时间
+            end_time (datatime64): 查询的终止时间
+
+        Returns:
+            datalist (GeoDataFrame): 符合条件的数据清单
+        """
+
+        clips = []
+
+        for key, value in self._datasets.items():
+            for v in value:
+                start = start_time
+                end = end_time
+                if start_time is None:
+                    start = v["start_time"]
+                if end_time is None:
+                    end = v["end_time"]
+
+                if start < v["start_time"]:
+                    start = v["start_time"]
+                if end > v["end_time"]:
+                    end = v["end_time"]
+
+                if start <= end:
+                    df = pd.DataFrame(
+                        {
+                            "id": [self._collection_id],
+                            "dataset": [key],
+                            "time_resolution": v["time_resolution"],
+                            "start_time": [str(start)],
+                            "end_time": [str(end)],
+                            "geometry": [
+                                f"POLYGON(({v['bbox'][0]} {v['bbox'][3]},{v['bbox'][0]} {v['bbox'][1]},\
+                                         {v['bbox'][2]} {v['bbox'][1]},{v['bbox'][2]} {v['bbox'][3]},{v['bbox'][0]} {v['bbox'][3]}))"
+                            ],
+                        }
+                    )
+                    df["geometry"] = gpd.GeoSeries.from_wkt(df["geometry"])
+                    gdf = gpd.GeoDataFrame(df, geometry="geometry", crs="EPSG:4326")
+
+                    clips.append(gdf.clip(aoi))
+
+        return pd.concat(clips)
+
+
+class GFSCatalog:
+    """
+    用于获取gfs的数据源信息，并搜索minio服务器中的数据范围
+
+    Attributes:
+        collection_id (str): 数据集名称
+        data_sources (str): 数据源
+        description (str): 数据源链接
+        spatial_resolution (str): 空间分辨率
+        temporal_resolution (str): 时间分辨率
+        datasets (dict): minio服务器中的已有数据集
+
+    Method:
+        search(aoi, start_time, end_time): 搜索minio服务器中的数据范围
+    """
+
+    def __init__(self, variable="tp"):
+        self._variable = variable
+        self._collection_id = f"gfs_atmos.{variable}"
+        self._datasources = "NOAA"
+        self._description = (
+            "https://www.emc.ncep.noaa.gov/emc/pages/numerical_forecast_systems/gfs.php"
+        )
+        self._spatialresolution = "0.25 x 0.25"
+        self._temporalresolution = "hourly; 1-120h"
+        self._bucket_name = "test"
+        self._datasets = self._get_datasets()
+
+    def _get_datasets(self):
+        dss = {}
+
+        ds = {}
+        with FS.open(os.path.join(self._bucket_name, "geodata/gfs/gfs.json")) as f:
+            gfs = json.load(f)
+        dss["wis"] = gfs[self._variable]
+
+        return dss
+
+    @property
+    def variable(self):
+        return self._variable
+
+    @property
+    def collection_id(self):
+        return self._collection_id
+
+    @property
+    def data_sources(self):
+        return self._datasources
+
+    @property
+    def description(self):
+        return self._description
+
+    @property
+    def spatial_resolution(self):
+        return self._spatialresolution
+
+    @property
+    def temporal_resolution(self):
+        return self._temporalresolution
+
+    @property
+    def datasets(self):
+        return self._datasets
+
+    def search(self, aoi, start_time=None, end_time=None):
+        """
+        查询并获取数据清单
+
+        Args:
+            aoi (GeoDataFrame): 矢量数据范围
+            start_time (datatime64): 查询的起始时间
+            end_time (datatime64): 查询的终止时间
+
+        Returns:
+            datalist (GeoDataFrame): 符合条件的数据清单
+        """
+
+        clips = []
+
+        for key, value in self._datasets.items():
+            for v in value:
+                start = start_time
+                end = end_time
+                if start_time is None:
+                    start = np.datetime64(v["start"])
+                if end_time is None:
+                    end = np.datetime64(v["end"])
+
+                if start < np.datetime64(v["start"]):
+                    start = np.datetime64(v["start"])
+
+                if end > np.datetime64(v["end"]):
+                    end = np.datetime64(v["end"])
+
+                if start <= end:
+                    df = pd.DataFrame(
+                        {
+                            "id": [self._collection_id],
+                            "dataset": [key],
+                            "start_time": [str(start)],
+                            "end_time": [str(end)],
+                            "geometry": [
+                                f"POLYGON(({v['bbox'][0]} {v['bbox'][3]},{v['bbox'][0]} {v['bbox'][1]},{v['bbox'][2]} {v['bbox'][1]},{v['bbox'][2]} {v['bbox'][3]},{v['bbox'][0]} {v['bbox'][3]}))"
+                            ],
+                        }
+                    )
+                    df["geometry"] = gpd.GeoSeries.from_wkt(df["geometry"])
+                    gdf = gpd.GeoDataFrame(df, geometry="geometry", crs="EPSG:4326")
+
+                    clips.append(gdf.clip(aoi))
+
+        return pd.concat(clips)
```

### Comparing `hydrodatasource-0.0.1/hydrodatasource/downloader/ncep_gfs.py` & `hydrodatasource-0.0.2/hydrodatasource/downloader/ncep_gfs.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,159 +1,159 @@
-"""
-该模块用于global forecast system数据下载
-
-如非特指，默认下载精度为0.25度。
-
-数据说明: [https://www.ncei.noaa.gov/products/weather-climate-models/global-forecast](https://www.ncei.noaa.gov/products/weather-climate-models/global-forecast)
-
-- `search` - 返回符合搜索条件的dem数据下载地址列表
-- `download` - 将列表中的数据下载到本地
-"""
-
-
-from .downloader import download_sigletasking
-import os
-import subprocess
-
-
-def get_gfs_from_ncep(
-    date: str,
-    creation_time: str,
-    forecast_time: int,
-    bbox=[115, 38, 136, 54],
-    save_dir=".",
-    cover=False,
-):
-    """
-    从ncep官网下载近期gfs数据
-
-    官方链接: [https://nomads.ncep.noaa.gov/cgi-bin/filter_gfs_0p25_1hr.pl](https://nomads.ncep.noaa.gov/cgi-bin/filter_gfs_0p25_1hr.pl)
-
-    下载url示例: [https://nomads.ncep.noaa.gov/cgi-bin/filter_gfs_0p25_1hr.pl?file=gfs.t00z.pgrb2.0p25.f001&all_lev=on&all_var=on&subregion=&leftlon=115&rightlon=136&toplat=54&bottomlat=38&dir=%2Fgfs.20220815%2F00%2Fatmos](https://nomads.ncep.noaa.gov/cgi-bin/filter_gfs_0p25_1hr.pl?file=gfs.t00z.pgrb2.0p25.f001&all_lev=on&all_var=on&subregion=&leftlon=115&rightlon=136&toplat=54&bottomlat=38&dir=%2Fgfs.20220815%2F00%2Fatmos)
-
-    Args:
-        date (str): 下载日期，格式为：YYYYMMDD
-        creation_time (str): 数据创建时间，可以是00、06、12、18中的一个
-        forecast_time (int): 预测序列，范围1-384
-        bbox (list): 下载数据的矩形范围
-        save_dir (str): 存储文件夹
-        cover (bool): 若文件已存在，是否覆盖
-
-    """
-
-    file_name_ = "gfsYYYYMMDD.tCCz.pgrb2.0p25.fFFF"
-
-    url_ = (f"https://nomads.ncep.noaa.gov/cgi-bin/filter_gfs_0p25.pl?file=gfs.tCCz.pgrb2.0p25.fFFF"
-            f"&lev_10_m_above_ground=on&lev_2_m_above_ground=on&lev_entire_atmosphere=on&lev_entire_atmosphere_%5C"
-            f"%28considered_as_a_single_layer%5C%29=on&lev_surface=on&var_APCP=on&var_DSWRF=on&var_PWAT=on&var_RH=on"
-            f"&var_SPFH=on&var_TCDC=on&var_TMP=on&var_UGRD=on&var_VGRD=on&subregion=&leftlon="
-            f"{str(bbox[0])}&rightlon={str(bbox[2])}&toplat={str(bbox[3])}&bottomlat="
-            f"{str(bbox[1])}&dir=%2Fgfs.YYYYMMDD%2FCC%2Fatmos")
-    url = (
-        url_.replace("YYYYMMDD", date)
-        .replace("CC", creation_time.zfill(2))
-        .replace("FFF", str(forecast_time).zfill(3))
-    )
-    file_name = (
-        file_name_.replace("YYYYMMDD", date)
-        .replace("CC", creation_time.zfill(2))
-        .replace("FFF", str(forecast_time).zfill(3))
-    )
-
-    file_path = os.path.join(save_dir, file_name)
-    if os.path.exists(file_path) and not cover:
-        print(f"{file_name}已存在.")
-        return
-
-    if not os.path.exists(os.path.dirname(file_path)):
-        os.makedirs(os.path.dirname(file_path))
-
-    download_sigletasking(url, os.path.join(save_dir, file_name))
-
-
-def get_gfs_from_aws(
-    date: str, creation_time: str, forecast_time: int, save_dir=".", cover=False
-):
-    """
-    从aws下载gfs数据，数据时间范围从2021年2月26日开始。
-
-    需要安装[aws cli](https://docs.aws.amazon.com/zh_cn/cli/latest/userguide/getting-started-install.html)
-
-    建议使用aws cli命令行下载
-
-    aws链接: [https://registry.opendata.aws/noaa-gfs-bdp-pds/](https://registry.opendata.aws/noaa-gfs-bdp-pds/)
-
-    下载url示例: [https://nomads.ncep.noaa.gov/cgi-bin/filter_gfs_0p25_1hr.pl?file=gfs.t00z.pgrb2.0p25.f001&all_lev=on
-    &all_var=on&subregion=&leftlon=115&rightlon=136&toplat=54&bottomlat=38&dir=%2Fgfs.20220815%2F00%2Fatmos](
-    https://nomads.ncep.noaa.gov/cgi-bin/filter_gfs_0p25_1hr.pl?file=gfs.t00z.pgrb2.0p25.f001&all_lev=on&all_var=on
-    &subregion=&leftlon=115&rightlon=136&toplat=54&bottomlat=38&dir=%2Fgfs.20220815%2F00%2Fatmos)
-
-    Args:
-        date (str): 下载日期，格式为：YYYYMMDD
-        creation_time (str): 数据创建时间，可以是00、06、12、18中的一个
-        forecast_time (int): 预测序列，范围1-384
-        save_dir (str): 存储文件夹
-        cover (bool): 若文件已存在，是否覆盖
-
-    """
-
-    url_ = "s3://noaa-gfs-bdp-pds/gfs.YYYYMMDD/CC/atmos/gfs.tCCz.pgrb2.0p25.fFFF"
-    if (date + creation_time.zfill(2)) < "2021032212":
-        url_ = "s3://noaa-gfs-bdp-pds/gfs.YYYYMMDD/CC/gfs.tCCz.pgrb2.0p25.fFFF"
-    file_name_ = "gfsYYYYMMDD.tCCz.pgrb2.0p25.fFFF"
-
-    url = (
-        url_.replace("YYYYMMDD", date)
-        .replace("CC", creation_time.zfill(2))
-        .replace("FFF", str(forecast_time).zfill(3))
-    )
-    file_name = (
-        file_name_.replace("YYYYMMDD", date)
-        .replace("CC", creation_time.zfill(2))
-        .replace("FFF", str(forecast_time).zfill(3))
-    )
-
-    file_path = os.path.join(save_dir, file_name)
-    if os.path.exists(file_path) and not cover:
-        print(f"{file_name}已存在.")
-        return
-
-    if not os.path.exists(os.path.dirname(file_path)):
-        os.makedirs(os.path.dirname(file_path))
-
-    # download_sigletasking(url,os.path.join(save_dir,file_name)
-    subprocess.call(["aws", "s3", "cp", url, file_path])
-
-
-def get_gfs_from_gee(
-    date: str,
-    creation_time: str,
-    forecast_time: int,
-    bbox=None,
-    save_dir=".",
-    cover=False,
-):
-    """
-    从google earth engine下载获取gfs数据，时间范围从2015年7月1日开始。
-
-    需要科学上网！
-
-    需要gee for python本地配置
-    - pip install google-api-python-client
-    - pip install pyCrytod
-    - pip install earthengine-api
-    - earthengine authenticate (需要gcloud)
-
-    gfs from gee链接: [https://developers.google.cn/earth-engine/datasets/catalog/NOAA_GFS0P25](https://developers.google.cn/earth-engine/datasets/catalog/NOAA_GFS0P25)
-
-    Args:
-        date (str): 下载日期，格式为：YYYYMMDD
-        creation_time (str): 数据创建时间，可以是00、06、12、18中的一个
-        forecast_time (int): 预测序列，范围1-384
-        bbox (list): 下载数据的矩形范围
-        save_dir (str): 存储文件夹
-        cover (bool): 若文件已存在，是否覆盖
-
-    """
-    if bbox is None:
-        bbox = [115, 38, 136, 54]
-    pass
+"""
+该模块用于global forecast system数据下载
+
+如非特指，默认下载精度为0.25度。
+
+数据说明: [https://www.ncei.noaa.gov/products/weather-climate-models/global-forecast](https://www.ncei.noaa.gov/products/weather-climate-models/global-forecast)
+
+- `search` - 返回符合搜索条件的dem数据下载地址列表
+- `download` - 将列表中的数据下载到本地
+"""
+
+
+from .downloader import download_sigletasking
+import os
+import subprocess
+
+
+def get_gfs_from_ncep(
+    date: str,
+    creation_time: str,
+    forecast_time: int,
+    bbox=[115, 38, 136, 54],
+    save_dir=".",
+    cover=False,
+):
+    """
+    从ncep官网下载近期gfs数据
+
+    官方链接: [https://nomads.ncep.noaa.gov/cgi-bin/filter_gfs_0p25_1hr.pl](https://nomads.ncep.noaa.gov/cgi-bin/filter_gfs_0p25_1hr.pl)
+
+    下载url示例: [https://nomads.ncep.noaa.gov/cgi-bin/filter_gfs_0p25_1hr.pl?file=gfs.t00z.pgrb2.0p25.f001&all_lev=on&all_var=on&subregion=&leftlon=115&rightlon=136&toplat=54&bottomlat=38&dir=%2Fgfs.20220815%2F00%2Fatmos](https://nomads.ncep.noaa.gov/cgi-bin/filter_gfs_0p25_1hr.pl?file=gfs.t00z.pgrb2.0p25.f001&all_lev=on&all_var=on&subregion=&leftlon=115&rightlon=136&toplat=54&bottomlat=38&dir=%2Fgfs.20220815%2F00%2Fatmos)
+
+    Args:
+        date (str): 下载日期，格式为：YYYYMMDD
+        creation_time (str): 数据创建时间，可以是00、06、12、18中的一个
+        forecast_time (int): 预测序列，范围1-384
+        bbox (list): 下载数据的矩形范围
+        save_dir (str): 存储文件夹
+        cover (bool): 若文件已存在，是否覆盖
+
+    """
+
+    file_name_ = "gfsYYYYMMDD.tCCz.pgrb2.0p25.fFFF"
+
+    url_ = (f"https://nomads.ncep.noaa.gov/cgi-bin/filter_gfs_0p25.pl?file=gfs.tCCz.pgrb2.0p25.fFFF"
+            f"&lev_10_m_above_ground=on&lev_2_m_above_ground=on&lev_entire_atmosphere=on&lev_entire_atmosphere_%5C"
+            f"%28considered_as_a_single_layer%5C%29=on&lev_surface=on&var_APCP=on&var_DSWRF=on&var_PWAT=on&var_RH=on"
+            f"&var_SPFH=on&var_TCDC=on&var_TMP=on&var_UGRD=on&var_VGRD=on&subregion=&leftlon="
+            f"{str(bbox[0])}&rightlon={str(bbox[2])}&toplat={str(bbox[3])}&bottomlat="
+            f"{str(bbox[1])}&dir=%2Fgfs.YYYYMMDD%2FCC%2Fatmos")
+    url = (
+        url_.replace("YYYYMMDD", date)
+        .replace("CC", creation_time.zfill(2))
+        .replace("FFF", str(forecast_time).zfill(3))
+    )
+    file_name = (
+        file_name_.replace("YYYYMMDD", date)
+        .replace("CC", creation_time.zfill(2))
+        .replace("FFF", str(forecast_time).zfill(3))
+    )
+
+    file_path = os.path.join(save_dir, file_name)
+    if os.path.exists(file_path) and not cover:
+        print(f"{file_name}已存在.")
+        return
+
+    if not os.path.exists(os.path.dirname(file_path)):
+        os.makedirs(os.path.dirname(file_path))
+
+    download_sigletasking(url, os.path.join(save_dir, file_name))
+
+
+def get_gfs_from_aws(
+    date: str, creation_time: str, forecast_time: int, save_dir=".", cover=False
+):
+    """
+    从aws下载gfs数据，数据时间范围从2021年2月26日开始。
+
+    需要安装[aws cli](https://docs.aws.amazon.com/zh_cn/cli/latest/userguide/getting-started-install.html)
+
+    建议使用aws cli命令行下载
+
+    aws链接: [https://registry.opendata.aws/noaa-gfs-bdp-pds/](https://registry.opendata.aws/noaa-gfs-bdp-pds/)
+
+    下载url示例: [https://nomads.ncep.noaa.gov/cgi-bin/filter_gfs_0p25_1hr.pl?file=gfs.t00z.pgrb2.0p25.f001&all_lev=on
+    &all_var=on&subregion=&leftlon=115&rightlon=136&toplat=54&bottomlat=38&dir=%2Fgfs.20220815%2F00%2Fatmos](
+    https://nomads.ncep.noaa.gov/cgi-bin/filter_gfs_0p25_1hr.pl?file=gfs.t00z.pgrb2.0p25.f001&all_lev=on&all_var=on
+    &subregion=&leftlon=115&rightlon=136&toplat=54&bottomlat=38&dir=%2Fgfs.20220815%2F00%2Fatmos)
+
+    Args:
+        date (str): 下载日期，格式为：YYYYMMDD
+        creation_time (str): 数据创建时间，可以是00、06、12、18中的一个
+        forecast_time (int): 预测序列，范围1-384
+        save_dir (str): 存储文件夹
+        cover (bool): 若文件已存在，是否覆盖
+
+    """
+
+    url_ = "s3://noaa-gfs-bdp-pds/gfs.YYYYMMDD/CC/atmos/gfs.tCCz.pgrb2.0p25.fFFF"
+    if (date + creation_time.zfill(2)) < "2021032212":
+        url_ = "s3://noaa-gfs-bdp-pds/gfs.YYYYMMDD/CC/gfs.tCCz.pgrb2.0p25.fFFF"
+    file_name_ = "gfsYYYYMMDD.tCCz.pgrb2.0p25.fFFF"
+
+    url = (
+        url_.replace("YYYYMMDD", date)
+        .replace("CC", creation_time.zfill(2))
+        .replace("FFF", str(forecast_time).zfill(3))
+    )
+    file_name = (
+        file_name_.replace("YYYYMMDD", date)
+        .replace("CC", creation_time.zfill(2))
+        .replace("FFF", str(forecast_time).zfill(3))
+    )
+
+    file_path = os.path.join(save_dir, file_name)
+    if os.path.exists(file_path) and not cover:
+        print(f"{file_name}已存在.")
+        return
+
+    if not os.path.exists(os.path.dirname(file_path)):
+        os.makedirs(os.path.dirname(file_path))
+
+    # download_sigletasking(url,os.path.join(save_dir,file_name)
+    subprocess.call(["aws", "s3", "cp", url, file_path])
+
+
+def get_gfs_from_gee(
+    date: str,
+    creation_time: str,
+    forecast_time: int,
+    bbox=None,
+    save_dir=".",
+    cover=False,
+):
+    """
+    从google earth engine下载获取gfs数据，时间范围从2015年7月1日开始。
+
+    需要科学上网！
+
+    需要gee for python本地配置
+    - pip install google-api-python-client
+    - pip install pyCrytod
+    - pip install earthengine-api
+    - earthengine authenticate (需要gcloud)
+
+    gfs from gee链接: [https://developers.google.cn/earth-engine/datasets/catalog/NOAA_GFS0P25](https://developers.google.cn/earth-engine/datasets/catalog/NOAA_GFS0P25)
+
+    Args:
+        date (str): 下载日期，格式为：YYYYMMDD
+        creation_time (str): 数据创建时间，可以是00、06、12、18中的一个
+        forecast_time (int): 预测序列，范围1-384
+        bbox (list): 下载数据的矩形范围
+        save_dir (str): 存储文件夹
+        cover (bool): 若文件已存在，是否覆盖
+
+    """
+    if bbox is None:
+        bbox = [115, 38, 136, 54]
+    pass
```

### Comparing `hydrodatasource-0.0.1/hydrodatasource/processor/data_checker.py` & `hydrodatasource-0.0.2/hydrodatasource/processor/data_checker.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,330 +1,330 @@
-"""
-Author: Wenyu Ouyang
-Date: 2024-03-24 08:48:57
-LastEditTime: 2024-03-28 08:38:13
-LastEditors: Wenyu Ouyang
-Description: Check user's data format is correct (local and minio)
-FilePath: \hydrodata\hydrodatasource\processor\data_checker.py
-Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
-"""
-
-import os
-import pandas as pd
-from hydrodatasource.configs.config import (
-    LOCAL_DATA_PATH,
-)
-
-
-class DataChecker:
-    """
-    A class to check the format of station, reservoir, and basin data based on specified rules.
-    """
-
-    def __init__(self):
-        """
-        Initialize the DataChecker with the path to the data.
-        """
-        self.base_path = LOCAL_DATA_PATH
-        # TODO: all specifications should be checked again
-        # NOTE: we prioritize the basin data format check as it is directly related to the model
-        self.expected_structure = {
-            "stations-origin": [
-                "pp_stations",
-                "zq_stations",
-                "zz_stations",
-                "stations_list",
-            ],
-            "reservoirs-origin": ["day_data", "hour_data", "reservoirs_list"],
-            "basins-origin": [
-                "basins_list",
-                "basin_shapefiles",
-                "hour_data",
-                "attributes.nc",
-                "basins_shp.zip",
-                "HydroRIVERS_v10_shp.zip",
-            ],
-        }
-        self.expected_columns = {
-            # 站点基础信息表
-            "stations_list": [
-                "ID",
-                "STCD",
-                "STTYPE",
-                "VARTYPE",
-                "DIVISION",
-                "LON",
-                "LAT",
-            ],
-            # 雨量站时序数据表
-            "pp_stations": ["ID", "STCD", "TM", "DRP", "INTV", "PDR", "DYP", "WTH"],
-            # 河道水文站/水位站时序信息表
-            "zq_stations": [
-                "ID",
-                "STCD",
-                "TM",
-                "Z",
-                "Q",
-                "XSA",
-                "XSAVV",
-                "XSMXV",
-                "FLWCHRCD",
-                "WPTN",
-                "MSQMT",
-                "MSAMT",
-                "MSVMT",
-            ],
-            "zz_stations": [
-                "ID",
-                "STCD",
-                "TM",
-                "Z",
-                "Q",
-                "XSA",
-                "XSAVV",
-                "XSMXV",
-                "FLWCHRCD",
-                "WPTN",
-                "MSQMT",
-                "MSAMT",
-                "MSVMT",
-            ],
-            # 水库基础信息表
-            "reservoirs_list": [
-                "ID",
-                "STCD",
-                "TTCP",
-                "DDZ",
-                "NORMZ",
-                "FSLTDZ",
-                "LON",
-                "LAT",
-                "BASIN",
-            ],
-            # 水库时序数据表
-            "reservoirs": [
-                "ID",
-                "STCD",
-                "TM",
-                "RZ",
-                "INQ",
-                "W",
-                "BLRZ",
-                "OTQ",
-                "RWCHRCD",
-                "RWPTN",
-                "INQDR",
-                "MSQMT",
-            ],
-            # 流域属性数据
-            "basins_attributes": [
-                "basin",
-                "area",
-                "ele_mt_smn",
-                "slp_dg_sav",
-                "sgr_dk_sav",
-                "for_pc_sse",
-                "glc_cl_smj",
-                "run_mm_syr",
-                "inu_pc_slt",
-                "cmi_ix_syr",
-                "aet_mm_syr",
-                "snw_pc_syr",
-                "swc_pc_syr",
-                "gwt_cm_sav",
-                "cly_pc_sav",
-                "dor_pc_pva",
-            ],
-            # 流域时序平均数据表
-            "basins_mean_data": [
-                # 根据文档提供的信息定义列名，例如:
-                "BAS_CODE",
-                "TS",
-                "GPM_TP",
-                "GFS_TP",
-                "GFS_10U",
-                "GFS_10V",
-                "GFS_2SH",
-                "GFS_2R",
-                "GFS_DSWRF",
-                "GFS_PWAT",
-                "GFS_2T",
-                "GFS_TCC",
-                "SMP",
-                "Q",
-                # 注意：这里的列名需要根据文档中的实际定义进行调整
-            ],
-            # 流域时序网格数据
-            "basins_grid_data": [
-                # 根据文档中的具体格式定义列名
-                # 例如:
-                "BAS_CODE",
-                "TS",
-                "GRID_DATA_TYPE",
-                "GRID_VALUE",
-                # 注意：这里的列名需要根据文档中的实际定义进行调整
-            ],
-            # others should be check again and more need to be added
-        }
-
-    def check_folder_structure(self):
-        """
-        Checks if the folder structure in the base directory matches the expected structure.
-
-        Returns
-        -------
-        bool
-            True if the structure matches, False otherwise.
-        """
-        for main_folder, subfolders in self.expected_structure.items():
-            main_folder_path = os.path.join(self.base_path, main_folder)
-            if not os.path.exists(main_folder_path):
-                print(f"Missing main folder: {main_folder}")
-                return False
-            for subfolder in subfolders:
-                subfolder_path = os.path.join(main_folder_path, subfolder)
-                if not os.path.exists(subfolder_path):
-                    print(f"Missing subfolder: {subfolder} in {main_folder}")
-                    return False
-        return True
-
-    def check_station_data_files(self, station_types=None):
-        """
-        Checks the format of station data files including both basic info and time-series data.
-        """
-        if station_types is None:
-            # one can specify the station types to check,
-            # such as ["pp"], ["zz"], or ["zq"]
-            station_types = ["pp", "zz", "zq"]
-        is_correct = True
-        for station_type in station_types:
-            # Check basic info file
-            basic_info_file = os.path.join(
-                # here we use / rather than os.path.join to avoid path issues for minio
-                self.base_path,
-                f"stations-origin/{station_type}_stations.csv",
-            )
-            if not self.check_file_format(
-                basic_info_file, self.expected_columns[f"{station_type}_stations"]
-            ):
-                print(f"Basic info file format error: {basic_info_file}")
-                is_correct = False
-
-            # Check time-series data files
-            time_series_folder = os.path.join(
-                self.base_path, f"stations-origin/{station_type}_stations"
-            )
-            if not self.check_files_in_folder(
-                time_series_folder, self.expected_columns[f"{station_type}_stations"]
-            ):
-                print(f"Time series file format error in folder: {time_series_folder}")
-                is_correct = False
-
-        return is_correct
-
-    def check_file_format(self, file_path, expected_columns):
-        """
-        Checks the format of a given file.
-
-        Parameters
-        ----------
-        file_path : str
-            Path to the file.
-        expected_columns : list
-            List of expected column names.
-
-        Returns
-        -------
-        bool
-            True if the file format is correct, False otherwise.
-        """
-        try:
-            data = pd.read_csv(file_path)
-            return all(column in data.columns for column in expected_columns)
-        except Exception as e:
-            print(f"Error reading file {file_path}: {e}")
-            return False
-
-    def check_files_in_folder(self, folder_path, expected_columns):
-        """
-        Checks the format of all CSV files in a folder.
-
-        Parameters
-        ----------
-        folder_path : str
-            Path to the folder containing the files.
-        expected_columns : list
-            List of expected column names for the files.
-
-        Returns
-        -------
-        bool
-            True if all file formats are correct, False otherwise.
-        """
-        is_correct = True
-        for file in os.listdir(folder_path):
-            if file.endswith(".csv"):
-                file_path = os.path.join(folder_path, file)
-                if not self.check_file_format(file_path, expected_columns):
-                    print(f"File format error: {file_path}")
-                    is_correct = False
-        return is_correct
-
-    def check_basin_data_files(self):
-        """
-        Checks the format of basin data files including attributes and time-series data.
-        """
-        is_correct = True
-
-        # Check basin attributes data file
-        basin_attributes_file = os.path.join(
-            self.base_path, "basins-origin/attributes.nc"
-        )
-        if not os.path.isfile(basin_attributes_file):
-            print(f"Missing basin attributes data file: {basin_attributes_file}")
-            is_correct = False
-
-        # Check basin time-series data file
-        basin_time_series_file = os.path.join(
-            self.base_path, "basins-origin/basins_mean_data.csv"
-        )
-        if not self.check_file_format(
-            basin_time_series_file, self.expected_columns["basins_mean_data"]
-        ):
-            print(f"Basin time series data file format error: {basin_time_series_file}")
-            is_correct = False
-
-        # Check for spatial data files, if required
-        # Example: checking for a specific shapefile
-        basin_shapefile = os.path.join(self.base_path, "basins-origin/basins_shp.zip")
-        if not os.path.isfile(basin_shapefile):
-            print(f"Missing basin shapefile: {basin_shapefile}")
-            is_correct = False
-
-        return is_correct
-
-    def check_basin_average_time_series_data(self):
-        """
-        Checks the format of basin average time-series data file.
-        """
-        # Define the file path for basin average time-series data
-        basin_avg_time_series_file = os.path.join(
-            self.base_path, "basins-origin/basin_average_time_series.csv"
-        )
-
-        # Check if the file exists
-        if not os.path.isfile(basin_avg_time_series_file):
-            print(
-                f"Missing basin average time series data file: {basin_avg_time_series_file}"
-            )
-            return False
-
-        # Check the file format
-        if not self.check_file_format(
-            basin_avg_time_series_file, self.expected_columns["basins_mean_data"]
-        ):
-            print(
-                f"Basin average time series data file format error: {basin_avg_time_series_file}"
-            )
-            return False
-
-        return True
+"""
+Author: Wenyu Ouyang
+Date: 2024-03-24 08:48:57
+LastEditTime: 2024-03-28 08:38:13
+LastEditors: Wenyu Ouyang
+Description: Check user's data format is correct (local and minio)
+FilePath: \hydrodata\hydrodatasource\processor\data_checker.py
+Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
+"""
+
+import os
+import pandas as pd
+from hydrodatasource.configs.config import (
+    LOCAL_DATA_PATH,
+)
+
+
+class DataChecker:
+    """
+    A class to check the format of station, reservoir, and basin data based on specified rules.
+    """
+
+    def __init__(self):
+        """
+        Initialize the DataChecker with the path to the data.
+        """
+        self.base_path = LOCAL_DATA_PATH
+        # TODO: all specifications should be checked again
+        # NOTE: we prioritize the basin data format check as it is directly related to the model
+        self.expected_structure = {
+            "stations-origin": [
+                "pp_stations",
+                "zq_stations",
+                "zz_stations",
+                "stations_list",
+            ],
+            "reservoirs-origin": ["day_data", "hour_data", "reservoirs_list"],
+            "basins-origin": [
+                "basins_list",
+                "basin_shapefiles",
+                "hour_data",
+                "attributes.nc",
+                "basins_shp.zip",
+                "HydroRIVERS_v10_shp.zip",
+            ],
+        }
+        self.expected_columns = {
+            # 站点基础信息表
+            "stations_list": [
+                "ID",
+                "STCD",
+                "STTYPE",
+                "VARTYPE",
+                "DIVISION",
+                "LON",
+                "LAT",
+            ],
+            # 雨量站时序数据表
+            "pp_stations": ["ID", "STCD", "TM", "DRP", "INTV", "PDR", "DYP", "WTH"],
+            # 河道水文站/水位站时序信息表
+            "zq_stations": [
+                "ID",
+                "STCD",
+                "TM",
+                "Z",
+                "Q",
+                "XSA",
+                "XSAVV",
+                "XSMXV",
+                "FLWCHRCD",
+                "WPTN",
+                "MSQMT",
+                "MSAMT",
+                "MSVMT",
+            ],
+            "zz_stations": [
+                "ID",
+                "STCD",
+                "TM",
+                "Z",
+                "Q",
+                "XSA",
+                "XSAVV",
+                "XSMXV",
+                "FLWCHRCD",
+                "WPTN",
+                "MSQMT",
+                "MSAMT",
+                "MSVMT",
+            ],
+            # 水库基础信息表
+            "reservoirs_list": [
+                "ID",
+                "STCD",
+                "TTCP",
+                "DDZ",
+                "NORMZ",
+                "FSLTDZ",
+                "LON",
+                "LAT",
+                "BASIN",
+            ],
+            # 水库时序数据表
+            "reservoirs": [
+                "ID",
+                "STCD",
+                "TM",
+                "RZ",
+                "INQ",
+                "W",
+                "BLRZ",
+                "OTQ",
+                "RWCHRCD",
+                "RWPTN",
+                "INQDR",
+                "MSQMT",
+            ],
+            # 流域属性数据
+            "basins_attributes": [
+                "basin",
+                "area",
+                "ele_mt_smn",
+                "slp_dg_sav",
+                "sgr_dk_sav",
+                "for_pc_sse",
+                "glc_cl_smj",
+                "run_mm_syr",
+                "inu_pc_slt",
+                "cmi_ix_syr",
+                "aet_mm_syr",
+                "snw_pc_syr",
+                "swc_pc_syr",
+                "gwt_cm_sav",
+                "cly_pc_sav",
+                "dor_pc_pva",
+            ],
+            # 流域时序平均数据表
+            "basins_mean_data": [
+                # 根据文档提供的信息定义列名，例如:
+                "BAS_CODE",
+                "TS",
+                "GPM_TP",
+                "GFS_TP",
+                "GFS_10U",
+                "GFS_10V",
+                "GFS_2SH",
+                "GFS_2R",
+                "GFS_DSWRF",
+                "GFS_PWAT",
+                "GFS_2T",
+                "GFS_TCC",
+                "SMP",
+                "Q",
+                # 注意：这里的列名需要根据文档中的实际定义进行调整
+            ],
+            # 流域时序网格数据
+            "basins_grid_data": [
+                # 根据文档中的具体格式定义列名
+                # 例如:
+                "BAS_CODE",
+                "TS",
+                "GRID_DATA_TYPE",
+                "GRID_VALUE",
+                # 注意：这里的列名需要根据文档中的实际定义进行调整
+            ],
+            # others should be check again and more need to be added
+        }
+
+    def check_folder_structure(self):
+        """
+        Checks if the folder structure in the base directory matches the expected structure.
+
+        Returns
+        -------
+        bool
+            True if the structure matches, False otherwise.
+        """
+        for main_folder, subfolders in self.expected_structure.items():
+            main_folder_path = os.path.join(self.base_path, main_folder)
+            if not os.path.exists(main_folder_path):
+                print(f"Missing main folder: {main_folder}")
+                return False
+            for subfolder in subfolders:
+                subfolder_path = os.path.join(main_folder_path, subfolder)
+                if not os.path.exists(subfolder_path):
+                    print(f"Missing subfolder: {subfolder} in {main_folder}")
+                    return False
+        return True
+
+    def check_station_data_files(self, station_types=None):
+        """
+        Checks the format of station data files including both basic info and time-series data.
+        """
+        if station_types is None:
+            # one can specify the station types to check,
+            # such as ["pp"], ["zz"], or ["zq"]
+            station_types = ["pp", "zz", "zq"]
+        is_correct = True
+        for station_type in station_types:
+            # Check basic info file
+            basic_info_file = os.path.join(
+                # here we use / rather than os.path.join to avoid path issues for minio
+                self.base_path,
+                f"stations-origin/{station_type}_stations.csv",
+            )
+            if not self.check_file_format(
+                basic_info_file, self.expected_columns[f"{station_type}_stations"]
+            ):
+                print(f"Basic info file format error: {basic_info_file}")
+                is_correct = False
+
+            # Check time-series data files
+            time_series_folder = os.path.join(
+                self.base_path, f"stations-origin/{station_type}_stations"
+            )
+            if not self.check_files_in_folder(
+                time_series_folder, self.expected_columns[f"{station_type}_stations"]
+            ):
+                print(f"Time series file format error in folder: {time_series_folder}")
+                is_correct = False
+
+        return is_correct
+
+    def check_file_format(self, file_path, expected_columns):
+        """
+        Checks the format of a given file.
+
+        Parameters
+        ----------
+        file_path : str
+            Path to the file.
+        expected_columns : list
+            List of expected column names.
+
+        Returns
+        -------
+        bool
+            True if the file format is correct, False otherwise.
+        """
+        try:
+            data = pd.read_csv(file_path)
+            return all(column in data.columns for column in expected_columns)
+        except Exception as e:
+            print(f"Error reading file {file_path}: {e}")
+            return False
+
+    def check_files_in_folder(self, folder_path, expected_columns):
+        """
+        Checks the format of all CSV files in a folder.
+
+        Parameters
+        ----------
+        folder_path : str
+            Path to the folder containing the files.
+        expected_columns : list
+            List of expected column names for the files.
+
+        Returns
+        -------
+        bool
+            True if all file formats are correct, False otherwise.
+        """
+        is_correct = True
+        for file in os.listdir(folder_path):
+            if file.endswith(".csv"):
+                file_path = os.path.join(folder_path, file)
+                if not self.check_file_format(file_path, expected_columns):
+                    print(f"File format error: {file_path}")
+                    is_correct = False
+        return is_correct
+
+    def check_basin_data_files(self):
+        """
+        Checks the format of basin data files including attributes and time-series data.
+        """
+        is_correct = True
+
+        # Check basin attributes data file
+        basin_attributes_file = os.path.join(
+            self.base_path, "basins-origin/attributes.nc"
+        )
+        if not os.path.isfile(basin_attributes_file):
+            print(f"Missing basin attributes data file: {basin_attributes_file}")
+            is_correct = False
+
+        # Check basin time-series data file
+        basin_time_series_file = os.path.join(
+            self.base_path, "basins-origin/basins_mean_data.csv"
+        )
+        if not self.check_file_format(
+            basin_time_series_file, self.expected_columns["basins_mean_data"]
+        ):
+            print(f"Basin time series data file format error: {basin_time_series_file}")
+            is_correct = False
+
+        # Check for spatial data files, if required
+        # Example: checking for a specific shapefile
+        basin_shapefile = os.path.join(self.base_path, "basins-origin/basins_shp.zip")
+        if not os.path.isfile(basin_shapefile):
+            print(f"Missing basin shapefile: {basin_shapefile}")
+            is_correct = False
+
+        return is_correct
+
+    def check_basin_average_time_series_data(self):
+        """
+        Checks the format of basin average time-series data file.
+        """
+        # Define the file path for basin average time-series data
+        basin_avg_time_series_file = os.path.join(
+            self.base_path, "basins-origin/basin_average_time_series.csv"
+        )
+
+        # Check if the file exists
+        if not os.path.isfile(basin_avg_time_series_file):
+            print(
+                f"Missing basin average time series data file: {basin_avg_time_series_file}"
+            )
+            return False
+
+        # Check the file format
+        if not self.check_file_format(
+            basin_avg_time_series_file, self.expected_columns["basins_mean_data"]
+        ):
+            print(
+                f"Basin average time series data file format error: {basin_avg_time_series_file}"
+            )
+            return False
+
+        return True
```

### Comparing `hydrodatasource-0.0.1/hydrodatasource/processor/gpm_gfs.py` & `hydrodatasource-0.0.2/hydrodatasource/processor/gpm_gfs.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,327 +1,327 @@
-from datetime import timedelta
-import datetime
-import xarray as xr
-import pandas as pd
-import tempfile
-import os
-import numpy as np
-import json
-
-from hydrodatasource.configs.config import (
-    FS,
-    GRID_INTERIM_BUCKET,
-    LOCAL_DATA_PATH,
-    MC,
-    RO,
-)
-from hydrodatasource.utils.utils import generate_time_intervals
-from hydrodatasource.processor.mask import gen_single_mask
-from hydrodatasource.reader import minio
-
-
-def process_data(initial_date, initial_time, mask, dataset):
-    # Convert the initial date and time to a datetime object
-    current_datetime = datetime.datetime.strptime(
-        f"{initial_date} {initial_time}", "%Y-%m-%d %H"
-    )
-    initial_datetime = datetime.datetime.strptime(
-        f"{initial_date} {initial_time}", "%Y-%m-%d %H"
-    )
-    gfs_reader = minio.GFSReader()
-    box = (
-        mask.coords["lon"][0] - 0.2,
-        mask.coords["lat"][0] - 0.2,
-        mask.coords["lon"][-1] + 0.2,
-        mask.coords["lat"][-1] + 0.2,
-    )
-
-    while True:
-        # Your existing code to process the data
-        data = gfs_reader.open_dataset(
-            creation_date=np.datetime64(current_datetime.strftime("%Y-%m-%d")),
-            creation_time=current_datetime.strftime("%H"),
-            bbox=box,
-            dataset=dataset,
-            time_chunks=24,
-        )
-        data = data.load()
-        data = data.to_dataset()
-        data = data.transpose("time", "valid_time", "lon", "lat")
-
-        # Adjust the slicing based on the current datetime
-        total_hours_passed = int(
-            (initial_datetime - current_datetime).total_seconds() / 3600
-        )
-
-        # Adjust the slicing based on the total hours passed
-        start_slice = total_hours_passed + 1
-        end_slice = start_slice + 6
-        # Minio上存储的gfs数据都是该时刻未来120小时后的数据，因此这里设置了一个报错
-        if start_slice > 120:
-            raise Exception("This datetime does not have enough data to merge")
-        data = data.isel(time=0, valid_time=slice(start_slice, end_slice))
-
-        # Check for negative values
-        data_det = data["total_precipitation_surface"].values
-        has_negative = data_det < 0
-        if has_negative.any():
-            # If negative, roll back time by 6 hours and repeat
-            current_datetime -= timedelta(hours=6)
-        else:
-            # No negative values found, return the data
-            return data
-
-
-def make_gpm_dataset(
-    time_periods,
-    dataset,
-    mask,
-):
-    gpm_reader = minio.GPMReader()
-    latest_data = xr.Dataset()
-    box = (
-        mask.coords["lon"][0],
-        mask.coords["lat"][0],
-        mask.coords["lon"][-1],
-        mask.coords["lat"][-1],
-    )
-    for time_num in time_periods:
-        start_time = np.datetime64(time_num[0])
-        end_time = np.datetime64(time_num[1])
-        data = gpm_reader.open_dataset(
-            start_time=start_time,
-            end_time=end_time,
-            dataset=dataset,
-            bbox=box,
-            time_resolution="30m",
-            time_chunks=24,
-        )
-        data = data.load()
-        # data = data.to_dataset()
-        # 转换时间维度至Pandas的DateTime格式并创建分组标签
-        times = pd.to_datetime(data["time"].values)
-        group_labels = times.floor("h")
-
-        # 创建一个新的DataArray，其时间维度与原始数据集匹配
-        group_labels_da = xr.DataArray(
-            group_labels, coords={"time": data["time"]}, dims=["time"]
-        )
-
-        # 对数据进行分组并求和
-        merge_gpm_data = data.groupby(group_labels_da).mean("time")
-
-        # 将维度名称从group_labels_da重新命名为'time'
-        merge_gpm_data = merge_gpm_data.rename({"group": "time"})
-        merge_gpm_data.name = "tp"
-        merge_gpm_data = merge_gpm_data.to_dataset()
-        w_data = mask["w"]
-        w_data_interpolated = w_data.interp(
-            lat=merge_gpm_data.lat, lon=merge_gpm_data.lon, method="nearest"
-        ).fillna(0)
-        w_data_broadcasted = w_data_interpolated.broadcast_like(merge_gpm_data["tp"])
-        merge_gpm_data = merge_gpm_data["tp"] * w_data_broadcasted
-        if isinstance(latest_data, xr.DataArray):
-            latest_data.name = "tp"
-            latest_data = latest_data.to_dataset()
-        if isinstance(merge_gpm_data, xr.DataArray):
-            merge_gpm_data.name = "tp"
-            merge_gpm_data = merge_gpm_data.to_dataset()
-        is_empty = not latest_data.data_vars
-        if is_empty:
-            latest_data = merge_gpm_data
-        else:
-            latest_data = xr.concat([latest_data, merge_gpm_data], dim="time")
-    return latest_data
-
-
-def make_gfs_dataset(
-    time_periods,
-    dataset,
-    mask,
-):
-    final_latest_data = xr.Dataset()
-    for time_num in time_periods:
-        start_time = datetime.datetime.strptime(time_num[0], "%Y-%m-%dT%H:%M:%S")
-        end_time = datetime.datetime.strptime(time_num[1], "%Y-%m-%dT%H:%M:%S")
-        gfs_time_list = generate_time_intervals(start_time, end_time)
-        w_data = mask["w"]
-        latest_data = xr.Dataset()
-
-        for date, time in gfs_time_list:
-            data = process_data(date, time, mask, dataset)
-            if isinstance(data, xr.DataArray):
-                data = data.to_dataset()
-            if "total_precipitation_surface" in data.data_vars:
-                data = data.rename({"total_precipitation_surface": "tp"})
-            data = data.drop_vars("time")
-            # print(data)
-            data = data.rename({"valid_time": "time"})
-            w_data_interpolated = w_data.interp(
-                lat=data.lat, lon=data.lon, method="nearest"
-            ).fillna(0)
-
-            # 将 w 数据广播到与当前数据集相同的时间维度上
-            w_data_broadcasted = w_data_interpolated.broadcast_like(data["tp"])
-            data["tp"] = data["tp"] * w_data_broadcasted
-            if isinstance(latest_data, xr.DataArray):
-                latest_data.name = "tp"
-                latest_data = latest_data.to_dataset()
-            if isinstance(data, xr.DataArray):
-                data.name = "tp"
-                data = data.to_dataset()
-            is_empty = not latest_data.data_vars
-            latest_data = (
-                data if is_empty else xr.concat([latest_data, data], dim="time")
-            )
-        if isinstance(latest_data, xr.DataArray):
-            latest_data.name = "tp"
-            latest_data = latest_data.to_dataset()
-        if isinstance(final_latest_data, xr.DataArray):
-            final_latest_data.name = "tp"
-            final_latest_data = final_latest_data.to_dataset()
-        is_final_empty = not final_latest_data.data_vars
-        if is_final_empty:
-            final_latest_data = latest_data
-        else:
-            final_latest_data = xr.concat([final_latest_data, latest_data], dim="time")
-    return final_latest_data
-
-
-def make_merge_dataset(
-    gpm_data, gfs_data, time_periods, gpm_length, gfs_length, time_now_length
-):
-    # 指定时间段
-    for time_num in time_periods:
-        start_time = pd.to_datetime(time_num[0])
-        end_time = pd.to_datetime(time_num[1])
-    time_range = pd.date_range(start=start_time, end=end_time, freq="H")
-
-    # 创建一个空的 xarray 数据集来存储结果
-    combined_data = xr.Dataset()
-
-    # 循环处理每个小时的数据
-    for specified_time in time_range:
-        m_hours = gpm_length
-        n_hours = gfs_length
-
-        # 选取specified_time前指定时间段的时间的gpm数据
-        gpm_data_filtered = gpm_data.sel(
-            time=slice(specified_time - pd.Timedelta(hours=m_hours), specified_time)
-        )
-        # 选取specified_time后指定时间段的时间的gfs数据
-        gfs_data_filtered = gfs_data.sel(
-            time=slice(
-                specified_time + pd.Timedelta(1),  # gfs数据要在
-                specified_time + pd.Timedelta(hours=n_hours),
-            )
-        )
-
-        gfs_data_interpolated = gfs_data_filtered.interp(
-            lat=gpm_data.lat, lon=gpm_data.lon, method="linear"
-        )
-        combined_hourly_data = xr.concat(
-            [gpm_data_filtered, gfs_data_interpolated], dim="time"
-        )
-        combined_hourly_data = combined_hourly_data.rename({"time": "step"})
-        combined_hourly_data["step"] = np.arange(len(combined_hourly_data.step))
-        time_now_hour = (
-            specified_time
-            - pd.Timedelta(hours=m_hours)
-            + pd.Timedelta(hours=time_now_length)
-        )
-        combined_hourly_data.coords["time_now"] = time_now_hour
-        combined_hourly_data = combined_hourly_data.expand_dims("time_now")
-
-        # 合并到结果数据集中
-        combined_data = xr.merge(
-            [combined_data, combined_hourly_data], combine_attrs="override"
-        )
-    return combined_data
-
-
-def make1nc41basin(
-    basin_id="1_02051500",
-    dataname="gpm",
-    local_path=LOCAL_DATA_PATH,
-    mask_path=os.path.join(LOCAL_DATA_PATH, "dataset-origin", "mask"),
-    shp_path=os.path.join(LOCAL_DATA_PATH, "dataset-origin", "shp"),
-    dataset="camels",
-    time_periods=[["2017-01-01T00:00:00", "2017-01-31T00:00:00"]],
-    local_save=True,
-    minio_upload=False,
-    gpm_length=None,
-    gfs_length=None,
-    time_now_length=None,
-    gpm_path=None,
-    gfs_path=None,
-):
-    if dataset not in ["camels", "wis"]:
-        # 流域是国内还是国外，国外是camels，国内是wis
-        raise ValueError("Invalid dataset")
-
-    mask = gen_single_mask(basin_id, shp_path, dataname, mask_path)
-
-    # 如果是合并数据，需要额外处理
-    if dataname == "merge":
-        mask = gen_single_mask(basin_id, shp_path, "gpm", mask_path)
-        gpm_data = (
-            make_gpm_dataset(time_periods, dataset, mask)
-            if gpm_path is None
-            else xr.open_dataset(gpm_path)
-        )
-        mask = gen_single_mask(basin_id, shp_path, "gfs", mask_path)
-        gfs_data = (
-            make_gfs_dataset(time_periods, dataset, mask)
-            if gfs_path is None
-            else xr.open_dataset(gfs_path)
-        )
-
-    data_functions = {
-        "gpm": lambda: make_gpm_dataset(time_periods, dataset, mask),
-        "gfs": lambda: make_gfs_dataset(time_periods, dataset, mask),
-        "merge": lambda: make_merge_dataset(
-            gpm_data, gfs_data, time_periods, gpm_length, gfs_length, time_now_length
-        ),
-    }
-
-    # 检查数据名称是否有效
-    if dataname not in data_functions:
-        raise NotImplementedError(
-            f"This type of data ({dataname}) is not available for now, please try gpm, gfs, or merge"
-        )
-
-    # 根据数据名称调用相应的函数
-    latest_data = data_functions[dataname]()
-
-    if local_save:
-        local_save_path = os.path.join(local_path, "datasets-interim", basin_id)
-        if not os.path.exists(local_save_path):
-            os.makedirs(local_save_path)
-        local_file_path = os.path.join(
-            local_path, "datasets-interim", basin_id, dataname
-        )
-        local_file_name = local_file_path + ".nc"
-        latest_data.to_netcdf(local_file_name)
-
-    if minio_upload:
-        object_name = basin_id + "/" + dataname + ".nc"
-
-        # 元数据
-        time_periods_str = json.dumps(time_periods)
-        metadata = {
-            "X-Amz-Meta-Time_Periods": time_periods_str,
-        }
-
-        with tempfile.NamedTemporaryFile() as tmp:
-            # 将数据集保存到临时文件
-            latest_data.to_netcdf(tmp.name)
-
-            # 重置文件读取指针
-            tmp.seek(0)
-
-            # 上传到 MinIO
-            MC.fput_object(
-                GRID_INTERIM_BUCKET, object_name, tmp.name, metadata=metadata
-            )
-
-    return latest_data
+from datetime import timedelta
+import datetime
+import xarray as xr
+import pandas as pd
+import tempfile
+import os
+import numpy as np
+import json
+
+from hydrodatasource.configs.config import (
+    FS,
+    GRID_INTERIM_BUCKET,
+    LOCAL_DATA_PATH,
+    MC,
+    RO,
+)
+from hydrodatasource.utils.utils import generate_time_intervals
+from hydrodatasource.processor.mask import gen_single_mask
+from hydrodatasource.reader import minio
+
+
+def process_data(initial_date, initial_time, mask, dataset):
+    # Convert the initial date and time to a datetime object
+    current_datetime = datetime.datetime.strptime(
+        f"{initial_date} {initial_time}", "%Y-%m-%d %H"
+    )
+    initial_datetime = datetime.datetime.strptime(
+        f"{initial_date} {initial_time}", "%Y-%m-%d %H"
+    )
+    gfs_reader = minio.GFSReader()
+    box = (
+        mask.coords["lon"][0] - 0.2,
+        mask.coords["lat"][0] - 0.2,
+        mask.coords["lon"][-1] + 0.2,
+        mask.coords["lat"][-1] + 0.2,
+    )
+
+    while True:
+        # Your existing code to process the data
+        data = gfs_reader.open_dataset(
+            creation_date=np.datetime64(current_datetime.strftime("%Y-%m-%d")),
+            creation_time=current_datetime.strftime("%H"),
+            bbox=box,
+            dataset=dataset,
+            time_chunks=24,
+        )
+        data = data.load()
+        data = data.to_dataset()
+        data = data.transpose("time", "valid_time", "lon", "lat")
+
+        # Adjust the slicing based on the current datetime
+        total_hours_passed = int(
+            (initial_datetime - current_datetime).total_seconds() / 3600
+        )
+
+        # Adjust the slicing based on the total hours passed
+        start_slice = total_hours_passed + 1
+        end_slice = start_slice + 6
+        # Minio上存储的gfs数据都是该时刻未来120小时后的数据，因此这里设置了一个报错
+        if start_slice > 120:
+            raise Exception("This datetime does not have enough data to merge")
+        data = data.isel(time=0, valid_time=slice(start_slice, end_slice))
+
+        # Check for negative values
+        data_det = data["total_precipitation_surface"].values
+        has_negative = data_det < 0
+        if has_negative.any():
+            # If negative, roll back time by 6 hours and repeat
+            current_datetime -= timedelta(hours=6)
+        else:
+            # No negative values found, return the data
+            return data
+
+
+def make_gpm_dataset(
+    time_periods,
+    dataset,
+    mask,
+):
+    gpm_reader = minio.GPMReader()
+    latest_data = xr.Dataset()
+    box = (
+        mask.coords["lon"][0],
+        mask.coords["lat"][0],
+        mask.coords["lon"][-1],
+        mask.coords["lat"][-1],
+    )
+    for time_num in time_periods:
+        start_time = np.datetime64(time_num[0])
+        end_time = np.datetime64(time_num[1])
+        data = gpm_reader.open_dataset(
+            start_time=start_time,
+            end_time=end_time,
+            dataset=dataset,
+            bbox=box,
+            time_resolution="30m",
+            time_chunks=24,
+        )
+        data = data.load()
+        # data = data.to_dataset()
+        # 转换时间维度至Pandas的DateTime格式并创建分组标签
+        times = pd.to_datetime(data["time"].values)
+        group_labels = times.floor("h")
+
+        # 创建一个新的DataArray，其时间维度与原始数据集匹配
+        group_labels_da = xr.DataArray(
+            group_labels, coords={"time": data["time"]}, dims=["time"]
+        )
+
+        # 对数据进行分组并求和
+        merge_gpm_data = data.groupby(group_labels_da).mean("time")
+
+        # 将维度名称从group_labels_da重新命名为'time'
+        merge_gpm_data = merge_gpm_data.rename({"group": "time"})
+        merge_gpm_data.name = "tp"
+        merge_gpm_data = merge_gpm_data.to_dataset()
+        w_data = mask["w"]
+        w_data_interpolated = w_data.interp(
+            lat=merge_gpm_data.lat, lon=merge_gpm_data.lon, method="nearest"
+        ).fillna(0)
+        w_data_broadcasted = w_data_interpolated.broadcast_like(merge_gpm_data["tp"])
+        merge_gpm_data = merge_gpm_data["tp"] * w_data_broadcasted
+        if isinstance(latest_data, xr.DataArray):
+            latest_data.name = "tp"
+            latest_data = latest_data.to_dataset()
+        if isinstance(merge_gpm_data, xr.DataArray):
+            merge_gpm_data.name = "tp"
+            merge_gpm_data = merge_gpm_data.to_dataset()
+        is_empty = not latest_data.data_vars
+        if is_empty:
+            latest_data = merge_gpm_data
+        else:
+            latest_data = xr.concat([latest_data, merge_gpm_data], dim="time")
+    return latest_data
+
+
+def make_gfs_dataset(
+    time_periods,
+    dataset,
+    mask,
+):
+    final_latest_data = xr.Dataset()
+    for time_num in time_periods:
+        start_time = datetime.datetime.strptime(time_num[0], "%Y-%m-%dT%H:%M:%S")
+        end_time = datetime.datetime.strptime(time_num[1], "%Y-%m-%dT%H:%M:%S")
+        gfs_time_list = generate_time_intervals(start_time, end_time)
+        w_data = mask["w"]
+        latest_data = xr.Dataset()
+
+        for date, time in gfs_time_list:
+            data = process_data(date, time, mask, dataset)
+            if isinstance(data, xr.DataArray):
+                data = data.to_dataset()
+            if "total_precipitation_surface" in data.data_vars:
+                data = data.rename({"total_precipitation_surface": "tp"})
+            data = data.drop_vars("time")
+            # print(data)
+            data = data.rename({"valid_time": "time"})
+            w_data_interpolated = w_data.interp(
+                lat=data.lat, lon=data.lon, method="nearest"
+            ).fillna(0)
+
+            # 将 w 数据广播到与当前数据集相同的时间维度上
+            w_data_broadcasted = w_data_interpolated.broadcast_like(data["tp"])
+            data["tp"] = data["tp"] * w_data_broadcasted
+            if isinstance(latest_data, xr.DataArray):
+                latest_data.name = "tp"
+                latest_data = latest_data.to_dataset()
+            if isinstance(data, xr.DataArray):
+                data.name = "tp"
+                data = data.to_dataset()
+            is_empty = not latest_data.data_vars
+            latest_data = (
+                data if is_empty else xr.concat([latest_data, data], dim="time")
+            )
+        if isinstance(latest_data, xr.DataArray):
+            latest_data.name = "tp"
+            latest_data = latest_data.to_dataset()
+        if isinstance(final_latest_data, xr.DataArray):
+            final_latest_data.name = "tp"
+            final_latest_data = final_latest_data.to_dataset()
+        is_final_empty = not final_latest_data.data_vars
+        if is_final_empty:
+            final_latest_data = latest_data
+        else:
+            final_latest_data = xr.concat([final_latest_data, latest_data], dim="time")
+    return final_latest_data
+
+
+def make_merge_dataset(
+    gpm_data, gfs_data, time_periods, gpm_length, gfs_length, time_now_length
+):
+    # 指定时间段
+    for time_num in time_periods:
+        start_time = pd.to_datetime(time_num[0])
+        end_time = pd.to_datetime(time_num[1])
+    time_range = pd.date_range(start=start_time, end=end_time, freq="H")
+
+    # 创建一个空的 xarray 数据集来存储结果
+    combined_data = xr.Dataset()
+
+    # 循环处理每个小时的数据
+    for specified_time in time_range:
+        m_hours = gpm_length
+        n_hours = gfs_length
+
+        # 选取specified_time前指定时间段的时间的gpm数据
+        gpm_data_filtered = gpm_data.sel(
+            time=slice(specified_time - pd.Timedelta(hours=m_hours), specified_time)
+        )
+        # 选取specified_time后指定时间段的时间的gfs数据
+        gfs_data_filtered = gfs_data.sel(
+            time=slice(
+                specified_time + pd.Timedelta(1),  # gfs数据要在
+                specified_time + pd.Timedelta(hours=n_hours),
+            )
+        )
+
+        gfs_data_interpolated = gfs_data_filtered.interp(
+            lat=gpm_data.lat, lon=gpm_data.lon, method="linear"
+        )
+        combined_hourly_data = xr.concat(
+            [gpm_data_filtered, gfs_data_interpolated], dim="time"
+        )
+        combined_hourly_data = combined_hourly_data.rename({"time": "step"})
+        combined_hourly_data["step"] = np.arange(len(combined_hourly_data.step))
+        time_now_hour = (
+            specified_time
+            - pd.Timedelta(hours=m_hours)
+            + pd.Timedelta(hours=time_now_length)
+        )
+        combined_hourly_data.coords["time_now"] = time_now_hour
+        combined_hourly_data = combined_hourly_data.expand_dims("time_now")
+
+        # 合并到结果数据集中
+        combined_data = xr.merge(
+            [combined_data, combined_hourly_data], combine_attrs="override"
+        )
+    return combined_data
+
+
+def make1nc41basin(
+    basin_id="1_02051500",
+    dataname="gpm",
+    local_path=LOCAL_DATA_PATH,
+    mask_path=os.path.join(LOCAL_DATA_PATH, "dataset-origin", "mask"),
+    shp_path=os.path.join(LOCAL_DATA_PATH, "dataset-origin", "shp"),
+    dataset="camels",
+    time_periods=[["2017-01-01T00:00:00", "2017-01-31T00:00:00"]],
+    local_save=True,
+    minio_upload=False,
+    gpm_length=None,
+    gfs_length=None,
+    time_now_length=None,
+    gpm_path=None,
+    gfs_path=None,
+):
+    if dataset not in ["camels", "wis"]:
+        # 流域是国内还是国外，国外是camels，国内是wis
+        raise ValueError("Invalid dataset")
+
+    mask = gen_single_mask(basin_id, shp_path, dataname, mask_path)
+
+    # 如果是合并数据，需要额外处理
+    if dataname == "merge":
+        mask = gen_single_mask(basin_id, shp_path, "gpm", mask_path)
+        gpm_data = (
+            make_gpm_dataset(time_periods, dataset, mask)
+            if gpm_path is None
+            else xr.open_dataset(gpm_path)
+        )
+        mask = gen_single_mask(basin_id, shp_path, "gfs", mask_path)
+        gfs_data = (
+            make_gfs_dataset(time_periods, dataset, mask)
+            if gfs_path is None
+            else xr.open_dataset(gfs_path)
+        )
+
+    data_functions = {
+        "gpm": lambda: make_gpm_dataset(time_periods, dataset, mask),
+        "gfs": lambda: make_gfs_dataset(time_periods, dataset, mask),
+        "merge": lambda: make_merge_dataset(
+            gpm_data, gfs_data, time_periods, gpm_length, gfs_length, time_now_length
+        ),
+    }
+
+    # 检查数据名称是否有效
+    if dataname not in data_functions:
+        raise NotImplementedError(
+            f"This type of data ({dataname}) is not available for now, please try gpm, gfs, or merge"
+        )
+
+    # 根据数据名称调用相应的函数
+    latest_data = data_functions[dataname]()
+
+    if local_save:
+        local_save_path = os.path.join(local_path, "datasets-interim", basin_id)
+        if not os.path.exists(local_save_path):
+            os.makedirs(local_save_path)
+        local_file_path = os.path.join(
+            local_path, "datasets-interim", basin_id, dataname
+        )
+        local_file_name = local_file_path + ".nc"
+        latest_data.to_netcdf(local_file_name)
+
+    if minio_upload:
+        object_name = basin_id + "/" + dataname + ".nc"
+
+        # 元数据
+        time_periods_str = json.dumps(time_periods)
+        metadata = {
+            "X-Amz-Meta-Time_Periods": time_periods_str,
+        }
+
+        with tempfile.NamedTemporaryFile() as tmp:
+            # 将数据集保存到临时文件
+            latest_data.to_netcdf(tmp.name)
+
+            # 重置文件读取指针
+            tmp.seek(0)
+
+            # 上传到 MinIO
+            MC.fput_object(
+                GRID_INTERIM_BUCKET, object_name, tmp.name, metadata=metadata
+            )
+
+    return latest_data
```

### Comparing `hydrodatasource-0.0.1/hydrodatasource/processor/grdc.py` & `hydrodatasource-0.0.2/hydrodatasource/processor/grdc.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,613 +1,613 @@
-"""
-Author: Wenyu Ouyang
-Date: 2023-11-03 09:16:41
-LastEditTime: 2024-02-20 19:53:03
-LastEditors: Wenyu Ouyang
-Description: Preprocess scripts for hydrostations data
-FilePath: \hydrodata\hydrodata\processor\preprocess_grdc.py
-Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
-"""
-
-import json
-import os
-import re
-import argparse
-import datetime
-import logging
-from pathlib import Path
-from typing import Dict, Optional, Tuple, Union
-from uu import Error
-import zipfile
-from dateutil.parser import parse
-import geopandas as gpd
-import numpy as np
-import pandas as pd
-from shapely.geometry import Point
-import requests
-from hydrodataset import CACHE_DIR
-
-
-# Path to the cache file
-cache_file_path = os.path.join(CACHE_DIR, "country_phone_codes.json")
-STATION_LST_COLUMNS = [
-    "ID",
-    "STCD",
-    "STNAME",
-    "STTYPE",
-    "VARTYPE",
-    "AGENCY",
-    "DIVISION",
-    "LON",
-    "LAT",
-    "SOURCE",
-]
-BASIN_LST_COLUMNS = [
-    "ID",
-    "NAME",
-    "LON",
-    "LAT",
-    "AREA",
-    "SOURCE",
-]
-
-
-def fetch_country_phone_codes():
-    # If the cache file exists, load the data from it
-    if os.path.exists(cache_file_path):
-        with open(cache_file_path, "r") as file:
-            country_phone_codes = json.load(file)
-        return country_phone_codes
-
-    # If the cache file doesn't exist, fetch the data from the API
-    url = "https://restcountries.com/v3.1/all"
-    response = requests.get(url)
-
-    if response.status_code != 200:
-        raise Error(f"Error fetching data: {response.status_code}")
-    countries = response.json()
-    country_phone_codes = {
-        country["name"]["common"]: (
-            re.sub(r"\D", "", country["idd"]["root"] + country["idd"]["suffixes"][0])
-            if "idd" in country
-            and "root" in country["idd"]
-            and "suffixes" in country["idd"]
-            and country["idd"]["suffixes"]
-            else "Unknown"
-        )
-        for country in countries
-    }
-
-    # Save the data to the cache file
-    with open(cache_file_path, "w") as file:
-        json.dump(country_phone_codes, file)
-
-    return country_phone_codes
-
-
-# Use the function
-country_phone_codes = fetch_country_phone_codes()
-world = gpd.read_file(gpd.datasets.get_path("naturalearth_lowres"))
-
-
-def save_and_zip_grdc_shp(gdf, basin_id, output_dir):
-    # Load the countries dataset from geopandas
-
-    # Sample point (longitude, latitude)
-    longitude, latitude = gdf["long_org"].iloc[0], gdf["lat_org"].iloc[0]
-
-    # Create a Point object from the coordinates
-    point = Point(longitude, latitude)
-
-    # Find the country that contains the point
-    country = world[world.geometry.contains(point)]
-
-    phone_code = country_phone_codes.get(country.iloc[0]["name"], "Unknown")
-    station_name = gdf["station"].iloc[0]
-    file_name = f"{phone_code}_grdc{basin_id}_{station_name}"
-    gdf["grdc_no"] = [
-        pc + "_grdc" + sc for pc, sc in zip([phone_code], gdf["grdc_no"].values)
-    ]
-    # change columns to uniform names
-    # pp may means post-processed, while org means original, hence we use pp
-    column_mapping = dict(
-        zip(
-            ["grdc_no", "station", "long_pp", "lat_pp", "area", "source"],
-            BASIN_LST_COLUMNS,
-        )
-    )
-    gdf = gdf.rename(columns=column_mapping)
-    other_columns = [col for col in gdf.columns if col not in BASIN_LST_COLUMNS]
-    new_order = BASIN_LST_COLUMNS + other_columns
-    gdf = gdf[new_order]
-    return save_shp(gdf, output_dir, file_name)
-
-
-def save_shp(gdf, output_dir, file_name):
-    shapefile_path = os.path.join(output_dir, file_name)
-    # Save the GeoDataFrame as a Shapefile
-    gdf.to_file(shapefile_path)
-
-    # Zip the Shapefile components directly
-    zip_path = os.path.join(output_dir, f"{file_name}.zip")
-    with zipfile.ZipFile(zip_path, "w") as zipf:
-        for extension in [".shp", ".shx", ".dbf", ".prj", ".cpg"]:
-            file_path = os.path.join(
-                f"{shapefile_path}",
-                f"{file_name}{extension}",
-            )
-            if os.path.exists(file_path):
-                zipf.write(file_path, os.path.basename(file_path))
-        # Remove the temporary Shapefile components
-    for extension in [".shp", ".shx", ".dbf", ".prj", ".cpg"]:
-        file_path = os.path.join(f"{shapefile_path}", f"{file_name}{extension}")
-        if os.path.exists(file_path):
-            os.remove(file_path)
-    os.removedirs(shapefile_path)
-    return zip_path
-
-
-# Create a directory for the basin shapefiles and their ZIPs
-def onegeojson2basinsshp4grdc(gjson_path, final_zip_dir):
-    # Create a directory for the final ZIP files
-    os.makedirs(final_zip_dir, exist_ok=True)
-    # Load the GeoJSON file
-    basins_gdf = gpd.read_file(gjson_path)
-    basins_gdf["grdc_no"] = basins_gdf["grdc_no"].astype(int).astype(str).str.zfill(8)
-
-    # Iterate through each basin and create individual Shapefiles and ZIPs
-    for index, row in basins_gdf.iterrows():
-        basin_id = row["grdc_no"]
-        basin_gdf = basins_gdf[basins_gdf.index == index]
-        save_and_zip_grdc_shp(basin_gdf, basin_id, final_zip_dir)
-
-
-def _get_time(time_iso: str) -> datetime.datetime:
-    """Return a datetime in UTC.
-    Convert a date string in ISO format to a datetime
-    and check if it is in UTC.
-    """
-    time = parse(time_iso)
-    if time.tzname() != "UTC":
-        raise ValueError(
-            "The time is not in UTC. The ISO format for a UTC time "
-            "is 'YYYY-MM-DDTHH:MM:SSZ'"
-        )
-    return time
-
-
-def _to_absolute_path(
-    input_path: str,
-    parent: Optional[Path] = None,
-    must_exist: bool = False,
-    must_be_in_parent=True,
-) -> Path:
-    """Parse input string as :py:class:`pathlib.Path` object.
-    Args:
-        input_path: Input string path that can be a relative or absolute path.
-        parent: Optional parent path of the input path
-        must_exist: Optional argument to check if the input path exists.
-        must_be_in_parent: Optional argument to check if the input path is
-            subpath of parent path
-    Returns:
-        The input path that is an absolute path and a :py:class:`pathlib.Path` object.
-    """
-    pathlike = Path(input_path)
-    if parent:
-        pathlike = parent.joinpath(pathlike)
-        if must_be_in_parent:
-            try:
-                pathlike.relative_to(parent)
-            except ValueError as e:
-                raise ValueError(
-                    f"Input path {input_path} is not a subpath of parent {parent}"
-                ) from e
-
-    return pathlike.expanduser().resolve(strict=must_exist)
-
-
-def _grdc_metadata_reader(grdc_station_path, all_lines):
-    """
-    Initiating a dictionary that will contain all GRDC attributes.
-    This function is based on earlier work by Rolf Hut.
-    https://github.com/RolfHut/GRDC2NetCDF/blob/master/GRDC2NetCDF.py
-    DOI: 10.5281/zenodo.19695
-    that function was based on earlier work by Edwin Sutanudjaja from Utrecht University.
-    https://github.com/edwinkost/discharge_analysis_IWMI
-    Modified by Susan Branchett
-    """
-
-    # split the content of the file into several lines
-    all_lines = all_lines.replace("\r", "")
-    all_lines = all_lines.split("\n")
-
-    # get grdc ids (from files) and check their consistency with their
-    # file names
-    id_from_file_name = int(
-        os.path.basename(grdc_station_path).split(".")[0].split("_")[0]
-    )
-    id_from_grdc = None
-    if id_from_file_name == int(all_lines[8].split(":")[1].strip()):
-        id_from_grdc = int(all_lines[8].split(":")[1].strip())
-    else:
-        print(
-            f"GRDC station {id_from_file_name} ({str(grdc_station_path)}) is NOT used."
-        )
-
-    attribute_grdc = {}
-    if id_from_grdc is not None:
-        attribute_grdc["grdc_file_name"] = str(grdc_station_path)
-        attribute_grdc["id_from_grdc"] = id_from_grdc
-
-        try:
-            attribute_grdc["file_generation_date"] = str(
-                all_lines[6].split(":")[1].strip()
-            )
-        except (IndexError, ValueError):
-            attribute_grdc["file_generation_date"] = "NA"
-
-        try:
-            attribute_grdc["river_name"] = str(all_lines[9].split(":")[1].strip())
-        except (IndexError, ValueError):
-            attribute_grdc["river_name"] = "NA"
-
-        try:
-            attribute_grdc["station_name"] = str(all_lines[10].split(":")[1].strip())
-        except (IndexError, ValueError):
-            attribute_grdc["station_name"] = "NA"
-
-        try:
-            attribute_grdc["country_code"] = str(all_lines[11].split(":")[1].strip())
-        except (IndexError, ValueError):
-            attribute_grdc["country_code"] = "NA"
-
-        try:
-            attribute_grdc["grdc_latitude_in_arc_degree"] = float(
-                all_lines[12].split(":")[1].strip()
-            )
-        except (IndexError, ValueError):
-            attribute_grdc["grdc_latitude_in_arc_degree"] = "NA"
-
-        try:
-            attribute_grdc["grdc_longitude_in_arc_degree"] = float(
-                all_lines[13].split(":")[1].strip()
-            )
-        except (IndexError, ValueError):
-            attribute_grdc["grdc_longitude_in_arc_degree"] = "NA"
-
-        try:
-            attribute_grdc["grdc_catchment_area_in_km2"] = float(
-                all_lines[14].split(":")[1].strip()
-            )
-            if attribute_grdc["grdc_catchment_area_in_km2"] <= 0.0:
-                attribute_grdc["grdc_catchment_area_in_km2"] = "NA"
-        except (IndexError, ValueError):
-            attribute_grdc["grdc_catchment_area_in_km2"] = "NA"
-
-        try:
-            attribute_grdc["altitude_masl"] = float(all_lines[15].split(":")[1].strip())
-        except (IndexError, ValueError):
-            attribute_grdc["altitude_masl"] = "NA"
-
-        try:
-            attribute_grdc["dataSetContent"] = str(all_lines[21].split(":")[1].strip())
-        except (IndexError, ValueError):
-            attribute_grdc["dataSetContent"] = "NA"
-
-        try:
-            attribute_grdc["units"] = str(all_lines[23].split(":")[1].strip())
-        except (IndexError, ValueError):
-            attribute_grdc["units"] = "NA"
-
-        try:
-            attribute_grdc["time_series"] = str(all_lines[24].split(":")[1].strip())
-        except (IndexError, ValueError):
-            attribute_grdc["time_series"] = "NA"
-
-        try:
-            attribute_grdc["no_of_years"] = int(all_lines[25].split(":")[1].strip())
-        except (IndexError, ValueError):
-            attribute_grdc["no_of_years"] = "NA"
-
-        try:
-            attribute_grdc["last_update"] = str(all_lines[26].split(":")[1].strip())
-        except (IndexError, ValueError):
-            attribute_grdc["last_update"] = "NA"
-
-        try:
-            attribute_grdc["nrMeasurements"] = int(
-                str(all_lines[34].split(":")[1].strip())
-            )
-        except (IndexError, ValueError):
-            attribute_grdc["nrMeasurements"] = "NA"
-
-    return attribute_grdc
-
-
-def _grdc_read(grdc_station_path, start, end, column):
-    with grdc_station_path.open("r", encoding="cp1252", errors="ignore") as file:
-        data = file.read()
-
-    metadata = _grdc_metadata_reader(grdc_station_path, data)
-
-    all_lines = data.split("\n")
-    header = next(
-        (i + 1 for i, line in enumerate(all_lines) if line.startswith("# DATA")),
-        0,
-    )
-    # Import GRDC data into dataframe and modify dataframe format
-    grdc_data = pd.read_csv(
-        grdc_station_path,
-        encoding="cp1252",
-        skiprows=header,
-        delimiter=";",
-        parse_dates=["YYYY-MM-DD"],
-        na_values="-999",
-    )
-    grdc_station_df = pd.DataFrame(
-        {column: grdc_data[" Value"].array},
-        index=grdc_data["YYYY-MM-DD"].array,
-    )
-    grdc_station_df.index.rename("time", inplace=True)
-
-    # Create a continuous date range based on the given start and end dates
-    full_date_range = pd.date_range(start=start, end=end)
-    full_df = pd.DataFrame(index=full_date_range)
-    full_df.index.rename("time", inplace=True)
-
-    # Merge the two dataframes, so the dates without data will have NaN values
-    merged_df = full_df.merge(
-        grdc_station_df, left_index=True, right_index=True, how="left"
-    )
-
-    return metadata, merged_df
-
-
-def _count_missing_data(df, column):
-    """Return number of missing data."""
-    return df[column].isna().sum()
-
-
-logger = logging.getLogger(__name__)
-
-
-def _log_metadata(metadata):
-    """Print some information about data."""
-    coords = (
-        metadata["grdc_latitude_in_arc_degree"],
-        metadata["grdc_longitude_in_arc_degree"],
-    )
-    message = (
-        f"GRDC station {metadata['id_from_grdc']} is selected. "
-        f"The river name is: {metadata['river_name']}."
-        f"The coordinates are: {coords}."
-        f"The catchment area in km2 is: {metadata['grdc_catchment_area_in_km2']}. "
-        f"There are {metadata['nrMissingData']} missing values during "
-        f"{metadata['UserStartTime']}_{metadata['UserEndTime']} at this station. "
-        f"See the metadata for more information."
-    )
-    logger.info("%s", message)
-
-
-MetaDataType = Dict[str, Union[str, int, float]]
-
-
-def read_grdc_daily_data(
-    station_id: str,
-    start_time: str,
-    end_time: str,
-    data_home: Optional[str],
-    parameter: str = "Q",
-    column: str = "streamflow",
-) -> Tuple[pd.core.frame.DataFrame, MetaDataType]:
-    """read daily river discharge data from Global Runoff Data Centre (GRDC).
-
-    Requires the GRDC daily data files in a local directory. The GRDC daily data
-    files can be ordered at
-    https://www.bafg.de/GRDC/EN/02_srvcs/21_tmsrs/riverdischarge_node.html
-
-    Parameters
-    ----------
-        station_id: The station id to get. The station id can be found in the
-            catalogues at
-            https://www.bafg.de/GRDC/EN/02_srvcs/21_tmsrs/212_prjctlgs/project_catalogue_node.html
-        start_time: Start time of model in UTC and ISO format string e.g.
-            'YYYY-MM-DDTHH:MM:SSZ'.
-        end_time: End time of model in  UTC and ISO format string e.g.
-            'YYYY-MM-DDTHH:MM:SSZ'.
-        parameter: optional. The parameter code to get, e.g. ('Q') discharge,
-            cubic meters per second.
-        data_home : optional. The directory where the daily grdc data is
-            located. If left out will use the grdc_location in the eWaterCycle
-            configuration file.
-        column: optional. Name of column in dataframe. Default: "streamflow".
-
-    Returns:
-        grdc data in a dataframe and metadata.
-
-    Examples:
-        .. code-block:: python
-
-            from ewatercycle.observation.grdc import get_grdc_data
-
-            df, meta = get_grdc_data('6335020',
-                                    '2000-01-01T00:00Z',
-                                    '2001-01-01T00:00Z')
-            df.describe()
-                     streamflow
-            count   4382.000000
-            mean    2328.992469
-            std	    1190.181058
-            min	     881.000000
-            25%	    1550.000000
-            50%	    2000.000000
-            75%	    2730.000000
-            max	   11300.000000
-
-            meta
-            {'grdc_file_name': '/home/myusername/git/eWaterCycle/ewatercycle/6335020_Q_Day.Cmd.txt',
-            'id_from_grdc': 6335020,
-            'file_generation_date': '2019-03-27',
-            'river_name': 'RHINE RIVER',
-            'station_name': 'REES',
-            'country_code': 'DE',
-            'grdc_latitude_in_arc_degree': 51.756918,
-            'grdc_longitude_in_arc_degree': 6.395395,
-            'grdc_catchment_area_in_km2': 159300.0,
-            'altitude_masl': 8.0,
-            'dataSetContent': 'MEAN DAILY DISCHARGE (Q)',
-            'units': 'm³/s',
-            'time_series': '1814-11 - 2016-12',
-            'no_of_years': 203,
-            'last_update': '2018-05-24',
-            'nrMeasurements': 'NA',
-            'UserStartTime': '2000-01-01T00:00Z',
-            'UserEndTime': '2001-01-01T00:00Z',
-            'nrMissingData': 0}
-    """  # noqa: E501
-    if data_home:
-        data_path = _to_absolute_path(data_home)
-    else:
-        raise ValueError(
-            "Provide the grdc path using `data_home` argument"
-            "or using `grdc_location` in ewatercycle configuration file."
-        )
-
-    if not data_path.exists():
-        raise ValueError(f"The grdc directory {data_path} does not exist!")
-
-    # Read the raw data
-    raw_file = data_path / f"{station_id}_{parameter}_Day.Cmd.txt"
-    if not raw_file.exists():
-        raise ValueError(f"The grdc file {raw_file} does not exist!")
-
-    # Convert the raw data to an xarray
-    metadata, df = _grdc_read(
-        raw_file,
-        start=_get_time(start_time).date(),
-        end=_get_time(end_time).date(),
-        column=column,
-    )
-
-    # Add start/end_time to metadata
-    metadata["UserStartTime"] = start_time
-    metadata["UserEndTime"] = end_time
-
-    # Add number of missing data to metadata
-    metadata["nrMissingData"] = _count_missing_data(df, column)
-
-    # Show info about data
-    _log_metadata(metadata)
-
-    return df, metadata
-
-
-def grdcstationdata2csvandshp(grdc_path, des_dir):
-    all_gdfs = []  # List to store all GeoDataFrames
-    phone_codes = []
-    for grdc_file in os.listdir(grdc_path):
-        if grdc_file.endswith(".txt"):
-            try:
-                df, meta = read_grdc_daily_data(
-                    grdc_file.split("_")[0],
-                    "1980-01-01T00:00Z",
-                    "2001-01-01T00:00Z",
-                    grdc_path,
-                )
-
-                geometry = [
-                    Point(
-                        meta["grdc_longitude_in_arc_degree"],
-                        meta["grdc_latitude_in_arc_degree"],
-                    )
-                ]
-
-                country = world[world.geometry.contains(geometry[0])]
-                phone_code = country_phone_codes.get(country.iloc[0]["name"], "Unknown")
-                phone_codes.append(phone_code)
-
-                # Save the data as a CSV file
-                sta_id = str(meta["id_from_grdc"]).zfill(8)
-                save_csv_file = f"zq_{phone_code}_grdc{sta_id}.csv"
-                save_dir = os.path.join(des_dir, "zq_stations")
-                if not os.path.exists(save_dir):
-                    os.makedirs(save_dir)
-                grdc_file_path = os.path.join(save_dir, save_csv_file)
-                df.to_csv(grdc_file_path)
-
-                gdf = gpd.GeoDataFrame([meta], geometry=geometry)
-                all_gdfs.append(gdf)  # Append the GeoDataFrame to the list
-
-            except FileNotFoundError as e:
-                print(f"Error reading data for station {grdc_file}: {e}")
-
-    # Concatenate all GeoDataFrames into a single GeoDataFrame
-    combined_gdf = pd.concat(all_gdfs)
-
-    # Set the coordinate reference system (CRS) to WGS84
-    combined_gdf.crs = "EPSG:4326"
-    # Define a dictionary where keys are old names and values are new names
-    new_column_names = {
-        "id_from_grdc": "STCD",
-        "station_name": "STNAME",
-        "grdc_latitude_in_arc_degree": "LAT",
-        "grdc_longitude_in_arc_degree": "LON",
-    }
-    # Rename the columns
-    combined_gdf = combined_gdf.rename(columns=new_column_names)
-    # Drop the columns you don't need
-    columns_to_drop = [
-        col
-        for col in combined_gdf.columns
-        if col not in new_column_names.values() and col != "geometry"
-    ]
-    combined_gdf = combined_gdf.drop(columns=columns_to_drop)
-
-    # Add new columns and set their values
-    combined_gdf["STCD"] = combined_gdf["STCD"].astype(str).str.zfill(8)
-    combined_gdf["ID"] = [
-        pc + "_grdc" + sc for pc, sc in zip(phone_codes, combined_gdf["STCD"].values)
-    ]
-    combined_gdf["STTYPE"] = "streamflow_station"
-    combined_gdf["VARTYPE"] = "streamflow"
-    combined_gdf["AGENCY"] = np.nan
-    combined_gdf["DIVISION"] = np.nan
-    combined_gdf["SOURCE"] = "GRDC"
-
-    combined_gdf = combined_gdf[STATION_LST_COLUMNS + ["geometry"]]
-    save_zq_dir = os.path.join(des_dir, "stations_list")
-    if not os.path.exists(save_zq_dir):
-        os.makedirs(save_zq_dir)
-    save_shp(combined_gdf, save_zq_dir, "zq_stations")
-    # Drop the geometry column and save as CSV
-    combined_csv_path = os.path.join(save_zq_dir, "zq_stations.csv")
-    combined_gdf.drop(columns=["geometry"]).to_csv(combined_csv_path, index=False)
-
-
-if __name__ == "__main__":
-    # Create the parser
-    parser = argparse.ArgumentParser(description="Give me paths..")
-
-    # Add the arguments
-    parser.add_argument(
-        "--grdc_path",
-        type=str,
-        help="The directory where the final ZIP file will be saved",
-        default=r"C:\Users\wenyu\.hydrodataset\cache\grdc",
-    )
-    parser.add_argument(
-        "--basin_dir",
-        type=str,
-        help="The name of the directory to move basin-files to",
-        default="D:\\data\\waterism\\basins-origin\\basins_list",
-    )
-    parser.add_argument(
-        "--station_dir",
-        type=str,
-        help="The name of the directory to upload station-files to",
-        default="D:\\data\\waterism\\stations-origin",
-    )
-    # Parse the arguments
-    args = parser.parse_args()
-    geojson_path = os.path.join(args.grdc_path, "stationbasins.geojson")
-    grdcstationdata2csvandshp(args.grdc_path, args.station_dir)
-    onegeojson2basinsshp4grdc(geojson_path, args.basin_dir)
+"""
+Author: Wenyu Ouyang
+Date: 2023-11-03 09:16:41
+LastEditTime: 2024-02-20 19:53:03
+LastEditors: Wenyu Ouyang
+Description: Preprocess scripts for hydrostations data
+FilePath: \hydrodata\hydrodata\processor\preprocess_grdc.py
+Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
+"""
+
+import json
+import os
+import re
+import argparse
+import datetime
+import logging
+from pathlib import Path
+from typing import Dict, Optional, Tuple, Union
+from uu import Error
+import zipfile
+from dateutil.parser import parse
+import geopandas as gpd
+import numpy as np
+import pandas as pd
+from shapely.geometry import Point
+import requests
+from hydrodataset import CACHE_DIR
+
+
+# Path to the cache file
+cache_file_path = os.path.join(CACHE_DIR, "country_phone_codes.json")
+STATION_LST_COLUMNS = [
+    "ID",
+    "STCD",
+    "STNAME",
+    "STTYPE",
+    "VARTYPE",
+    "AGENCY",
+    "DIVISION",
+    "LON",
+    "LAT",
+    "SOURCE",
+]
+BASIN_LST_COLUMNS = [
+    "ID",
+    "NAME",
+    "LON",
+    "LAT",
+    "AREA",
+    "SOURCE",
+]
+
+
+def fetch_country_phone_codes():
+    # If the cache file exists, load the data from it
+    if os.path.exists(cache_file_path):
+        with open(cache_file_path, "r") as file:
+            country_phone_codes = json.load(file)
+        return country_phone_codes
+
+    # If the cache file doesn't exist, fetch the data from the API
+    url = "https://restcountries.com/v3.1/all"
+    response = requests.get(url)
+
+    if response.status_code != 200:
+        raise Error(f"Error fetching data: {response.status_code}")
+    countries = response.json()
+    country_phone_codes = {
+        country["name"]["common"]: (
+            re.sub(r"\D", "", country["idd"]["root"] + country["idd"]["suffixes"][0])
+            if "idd" in country
+            and "root" in country["idd"]
+            and "suffixes" in country["idd"]
+            and country["idd"]["suffixes"]
+            else "Unknown"
+        )
+        for country in countries
+    }
+
+    # Save the data to the cache file
+    with open(cache_file_path, "w") as file:
+        json.dump(country_phone_codes, file)
+
+    return country_phone_codes
+
+
+# Use the function
+country_phone_codes = fetch_country_phone_codes()
+world = gpd.read_file(gpd.datasets.get_path("naturalearth_lowres"))
+
+
+def save_and_zip_grdc_shp(gdf, basin_id, output_dir):
+    # Load the countries dataset from geopandas
+
+    # Sample point (longitude, latitude)
+    longitude, latitude = gdf["long_org"].iloc[0], gdf["lat_org"].iloc[0]
+
+    # Create a Point object from the coordinates
+    point = Point(longitude, latitude)
+
+    # Find the country that contains the point
+    country = world[world.geometry.contains(point)]
+
+    phone_code = country_phone_codes.get(country.iloc[0]["name"], "Unknown")
+    station_name = gdf["station"].iloc[0]
+    file_name = f"{phone_code}_grdc{basin_id}_{station_name}"
+    gdf["grdc_no"] = [
+        pc + "_grdc" + sc for pc, sc in zip([phone_code], gdf["grdc_no"].values)
+    ]
+    # change columns to uniform names
+    # pp may means post-processed, while org means original, hence we use pp
+    column_mapping = dict(
+        zip(
+            ["grdc_no", "station", "long_pp", "lat_pp", "area", "source"],
+            BASIN_LST_COLUMNS,
+        )
+    )
+    gdf = gdf.rename(columns=column_mapping)
+    other_columns = [col for col in gdf.columns if col not in BASIN_LST_COLUMNS]
+    new_order = BASIN_LST_COLUMNS + other_columns
+    gdf = gdf[new_order]
+    return save_shp(gdf, output_dir, file_name)
+
+
+def save_shp(gdf, output_dir, file_name):
+    shapefile_path = os.path.join(output_dir, file_name)
+    # Save the GeoDataFrame as a Shapefile
+    gdf.to_file(shapefile_path)
+
+    # Zip the Shapefile components directly
+    zip_path = os.path.join(output_dir, f"{file_name}.zip")
+    with zipfile.ZipFile(zip_path, "w") as zipf:
+        for extension in [".shp", ".shx", ".dbf", ".prj", ".cpg"]:
+            file_path = os.path.join(
+                f"{shapefile_path}",
+                f"{file_name}{extension}",
+            )
+            if os.path.exists(file_path):
+                zipf.write(file_path, os.path.basename(file_path))
+        # Remove the temporary Shapefile components
+    for extension in [".shp", ".shx", ".dbf", ".prj", ".cpg"]:
+        file_path = os.path.join(f"{shapefile_path}", f"{file_name}{extension}")
+        if os.path.exists(file_path):
+            os.remove(file_path)
+    os.removedirs(shapefile_path)
+    return zip_path
+
+
+# Create a directory for the basin shapefiles and their ZIPs
+def onegeojson2basinsshp4grdc(gjson_path, final_zip_dir):
+    # Create a directory for the final ZIP files
+    os.makedirs(final_zip_dir, exist_ok=True)
+    # Load the GeoJSON file
+    basins_gdf = gpd.read_file(gjson_path)
+    basins_gdf["grdc_no"] = basins_gdf["grdc_no"].astype(int).astype(str).str.zfill(8)
+
+    # Iterate through each basin and create individual Shapefiles and ZIPs
+    for index, row in basins_gdf.iterrows():
+        basin_id = row["grdc_no"]
+        basin_gdf = basins_gdf[basins_gdf.index == index]
+        save_and_zip_grdc_shp(basin_gdf, basin_id, final_zip_dir)
+
+
+def _get_time(time_iso: str) -> datetime.datetime:
+    """Return a datetime in UTC.
+    Convert a date string in ISO format to a datetime
+    and check if it is in UTC.
+    """
+    time = parse(time_iso)
+    if time.tzname() != "UTC":
+        raise ValueError(
+            "The time is not in UTC. The ISO format for a UTC time "
+            "is 'YYYY-MM-DDTHH:MM:SSZ'"
+        )
+    return time
+
+
+def _to_absolute_path(
+    input_path: str,
+    parent: Optional[Path] = None,
+    must_exist: bool = False,
+    must_be_in_parent=True,
+) -> Path:
+    """Parse input string as :py:class:`pathlib.Path` object.
+    Args:
+        input_path: Input string path that can be a relative or absolute path.
+        parent: Optional parent path of the input path
+        must_exist: Optional argument to check if the input path exists.
+        must_be_in_parent: Optional argument to check if the input path is
+            subpath of parent path
+    Returns:
+        The input path that is an absolute path and a :py:class:`pathlib.Path` object.
+    """
+    pathlike = Path(input_path)
+    if parent:
+        pathlike = parent.joinpath(pathlike)
+        if must_be_in_parent:
+            try:
+                pathlike.relative_to(parent)
+            except ValueError as e:
+                raise ValueError(
+                    f"Input path {input_path} is not a subpath of parent {parent}"
+                ) from e
+
+    return pathlike.expanduser().resolve(strict=must_exist)
+
+
+def _grdc_metadata_reader(grdc_station_path, all_lines):
+    """
+    Initiating a dictionary that will contain all GRDC attributes.
+    This function is based on earlier work by Rolf Hut.
+    https://github.com/RolfHut/GRDC2NetCDF/blob/master/GRDC2NetCDF.py
+    DOI: 10.5281/zenodo.19695
+    that function was based on earlier work by Edwin Sutanudjaja from Utrecht University.
+    https://github.com/edwinkost/discharge_analysis_IWMI
+    Modified by Susan Branchett
+    """
+
+    # split the content of the file into several lines
+    all_lines = all_lines.replace("\r", "")
+    all_lines = all_lines.split("\n")
+
+    # get grdc ids (from files) and check their consistency with their
+    # file names
+    id_from_file_name = int(
+        os.path.basename(grdc_station_path).split(".")[0].split("_")[0]
+    )
+    id_from_grdc = None
+    if id_from_file_name == int(all_lines[8].split(":")[1].strip()):
+        id_from_grdc = int(all_lines[8].split(":")[1].strip())
+    else:
+        print(
+            f"GRDC station {id_from_file_name} ({str(grdc_station_path)}) is NOT used."
+        )
+
+    attribute_grdc = {}
+    if id_from_grdc is not None:
+        attribute_grdc["grdc_file_name"] = str(grdc_station_path)
+        attribute_grdc["id_from_grdc"] = id_from_grdc
+
+        try:
+            attribute_grdc["file_generation_date"] = str(
+                all_lines[6].split(":")[1].strip()
+            )
+        except (IndexError, ValueError):
+            attribute_grdc["file_generation_date"] = "NA"
+
+        try:
+            attribute_grdc["river_name"] = str(all_lines[9].split(":")[1].strip())
+        except (IndexError, ValueError):
+            attribute_grdc["river_name"] = "NA"
+
+        try:
+            attribute_grdc["station_name"] = str(all_lines[10].split(":")[1].strip())
+        except (IndexError, ValueError):
+            attribute_grdc["station_name"] = "NA"
+
+        try:
+            attribute_grdc["country_code"] = str(all_lines[11].split(":")[1].strip())
+        except (IndexError, ValueError):
+            attribute_grdc["country_code"] = "NA"
+
+        try:
+            attribute_grdc["grdc_latitude_in_arc_degree"] = float(
+                all_lines[12].split(":")[1].strip()
+            )
+        except (IndexError, ValueError):
+            attribute_grdc["grdc_latitude_in_arc_degree"] = "NA"
+
+        try:
+            attribute_grdc["grdc_longitude_in_arc_degree"] = float(
+                all_lines[13].split(":")[1].strip()
+            )
+        except (IndexError, ValueError):
+            attribute_grdc["grdc_longitude_in_arc_degree"] = "NA"
+
+        try:
+            attribute_grdc["grdc_catchment_area_in_km2"] = float(
+                all_lines[14].split(":")[1].strip()
+            )
+            if attribute_grdc["grdc_catchment_area_in_km2"] <= 0.0:
+                attribute_grdc["grdc_catchment_area_in_km2"] = "NA"
+        except (IndexError, ValueError):
+            attribute_grdc["grdc_catchment_area_in_km2"] = "NA"
+
+        try:
+            attribute_grdc["altitude_masl"] = float(all_lines[15].split(":")[1].strip())
+        except (IndexError, ValueError):
+            attribute_grdc["altitude_masl"] = "NA"
+
+        try:
+            attribute_grdc["dataSetContent"] = str(all_lines[21].split(":")[1].strip())
+        except (IndexError, ValueError):
+            attribute_grdc["dataSetContent"] = "NA"
+
+        try:
+            attribute_grdc["units"] = str(all_lines[23].split(":")[1].strip())
+        except (IndexError, ValueError):
+            attribute_grdc["units"] = "NA"
+
+        try:
+            attribute_grdc["time_series"] = str(all_lines[24].split(":")[1].strip())
+        except (IndexError, ValueError):
+            attribute_grdc["time_series"] = "NA"
+
+        try:
+            attribute_grdc["no_of_years"] = int(all_lines[25].split(":")[1].strip())
+        except (IndexError, ValueError):
+            attribute_grdc["no_of_years"] = "NA"
+
+        try:
+            attribute_grdc["last_update"] = str(all_lines[26].split(":")[1].strip())
+        except (IndexError, ValueError):
+            attribute_grdc["last_update"] = "NA"
+
+        try:
+            attribute_grdc["nrMeasurements"] = int(
+                str(all_lines[34].split(":")[1].strip())
+            )
+        except (IndexError, ValueError):
+            attribute_grdc["nrMeasurements"] = "NA"
+
+    return attribute_grdc
+
+
+def _grdc_read(grdc_station_path, start, end, column):
+    with grdc_station_path.open("r", encoding="cp1252", errors="ignore") as file:
+        data = file.read()
+
+    metadata = _grdc_metadata_reader(grdc_station_path, data)
+
+    all_lines = data.split("\n")
+    header = next(
+        (i + 1 for i, line in enumerate(all_lines) if line.startswith("# DATA")),
+        0,
+    )
+    # Import GRDC data into dataframe and modify dataframe format
+    grdc_data = pd.read_csv(
+        grdc_station_path,
+        encoding="cp1252",
+        skiprows=header,
+        delimiter=";",
+        parse_dates=["YYYY-MM-DD"],
+        na_values="-999",
+    )
+    grdc_station_df = pd.DataFrame(
+        {column: grdc_data[" Value"].array},
+        index=grdc_data["YYYY-MM-DD"].array,
+    )
+    grdc_station_df.index.rename("time", inplace=True)
+
+    # Create a continuous date range based on the given start and end dates
+    full_date_range = pd.date_range(start=start, end=end)
+    full_df = pd.DataFrame(index=full_date_range)
+    full_df.index.rename("time", inplace=True)
+
+    # Merge the two dataframes, so the dates without data will have NaN values
+    merged_df = full_df.merge(
+        grdc_station_df, left_index=True, right_index=True, how="left"
+    )
+
+    return metadata, merged_df
+
+
+def _count_missing_data(df, column):
+    """Return number of missing data."""
+    return df[column].isna().sum()
+
+
+logger = logging.getLogger(__name__)
+
+
+def _log_metadata(metadata):
+    """Print some information about data."""
+    coords = (
+        metadata["grdc_latitude_in_arc_degree"],
+        metadata["grdc_longitude_in_arc_degree"],
+    )
+    message = (
+        f"GRDC station {metadata['id_from_grdc']} is selected. "
+        f"The river name is: {metadata['river_name']}."
+        f"The coordinates are: {coords}."
+        f"The catchment area in km2 is: {metadata['grdc_catchment_area_in_km2']}. "
+        f"There are {metadata['nrMissingData']} missing values during "
+        f"{metadata['UserStartTime']}_{metadata['UserEndTime']} at this station. "
+        f"See the metadata for more information."
+    )
+    logger.info("%s", message)
+
+
+MetaDataType = Dict[str, Union[str, int, float]]
+
+
+def read_grdc_daily_data(
+    station_id: str,
+    start_time: str,
+    end_time: str,
+    data_home: Optional[str],
+    parameter: str = "Q",
+    column: str = "streamflow",
+) -> Tuple[pd.core.frame.DataFrame, MetaDataType]:
+    """read daily river discharge data from Global Runoff Data Centre (GRDC).
+
+    Requires the GRDC daily data files in a local directory. The GRDC daily data
+    files can be ordered at
+    https://www.bafg.de/GRDC/EN/02_srvcs/21_tmsrs/riverdischarge_node.html
+
+    Parameters
+    ----------
+        station_id: The station id to get. The station id can be found in the
+            catalogues at
+            https://www.bafg.de/GRDC/EN/02_srvcs/21_tmsrs/212_prjctlgs/project_catalogue_node.html
+        start_time: Start time of model in UTC and ISO format string e.g.
+            'YYYY-MM-DDTHH:MM:SSZ'.
+        end_time: End time of model in  UTC and ISO format string e.g.
+            'YYYY-MM-DDTHH:MM:SSZ'.
+        parameter: optional. The parameter code to get, e.g. ('Q') discharge,
+            cubic meters per second.
+        data_home : optional. The directory where the daily grdc data is
+            located. If left out will use the grdc_location in the eWaterCycle
+            configuration file.
+        column: optional. Name of column in dataframe. Default: "streamflow".
+
+    Returns:
+        grdc data in a dataframe and metadata.
+
+    Examples:
+        .. code-block:: python
+
+            from ewatercycle.observation.grdc import get_grdc_data
+
+            df, meta = get_grdc_data('6335020',
+                                    '2000-01-01T00:00Z',
+                                    '2001-01-01T00:00Z')
+            df.describe()
+                     streamflow
+            count   4382.000000
+            mean    2328.992469
+            std	    1190.181058
+            min	     881.000000
+            25%	    1550.000000
+            50%	    2000.000000
+            75%	    2730.000000
+            max	   11300.000000
+
+            meta
+            {'grdc_file_name': '/home/myusername/git/eWaterCycle/ewatercycle/6335020_Q_Day.Cmd.txt',
+            'id_from_grdc': 6335020,
+            'file_generation_date': '2019-03-27',
+            'river_name': 'RHINE RIVER',
+            'station_name': 'REES',
+            'country_code': 'DE',
+            'grdc_latitude_in_arc_degree': 51.756918,
+            'grdc_longitude_in_arc_degree': 6.395395,
+            'grdc_catchment_area_in_km2': 159300.0,
+            'altitude_masl': 8.0,
+            'dataSetContent': 'MEAN DAILY DISCHARGE (Q)',
+            'units': 'm³/s',
+            'time_series': '1814-11 - 2016-12',
+            'no_of_years': 203,
+            'last_update': '2018-05-24',
+            'nrMeasurements': 'NA',
+            'UserStartTime': '2000-01-01T00:00Z',
+            'UserEndTime': '2001-01-01T00:00Z',
+            'nrMissingData': 0}
+    """  # noqa: E501
+    if data_home:
+        data_path = _to_absolute_path(data_home)
+    else:
+        raise ValueError(
+            "Provide the grdc path using `data_home` argument"
+            "or using `grdc_location` in ewatercycle configuration file."
+        )
+
+    if not data_path.exists():
+        raise ValueError(f"The grdc directory {data_path} does not exist!")
+
+    # Read the raw data
+    raw_file = data_path / f"{station_id}_{parameter}_Day.Cmd.txt"
+    if not raw_file.exists():
+        raise ValueError(f"The grdc file {raw_file} does not exist!")
+
+    # Convert the raw data to an xarray
+    metadata, df = _grdc_read(
+        raw_file,
+        start=_get_time(start_time).date(),
+        end=_get_time(end_time).date(),
+        column=column,
+    )
+
+    # Add start/end_time to metadata
+    metadata["UserStartTime"] = start_time
+    metadata["UserEndTime"] = end_time
+
+    # Add number of missing data to metadata
+    metadata["nrMissingData"] = _count_missing_data(df, column)
+
+    # Show info about data
+    _log_metadata(metadata)
+
+    return df, metadata
+
+
+def grdcstationdata2csvandshp(grdc_path, des_dir):
+    all_gdfs = []  # List to store all GeoDataFrames
+    phone_codes = []
+    for grdc_file in os.listdir(grdc_path):
+        if grdc_file.endswith(".txt"):
+            try:
+                df, meta = read_grdc_daily_data(
+                    grdc_file.split("_")[0],
+                    "1980-01-01T00:00Z",
+                    "2001-01-01T00:00Z",
+                    grdc_path,
+                )
+
+                geometry = [
+                    Point(
+                        meta["grdc_longitude_in_arc_degree"],
+                        meta["grdc_latitude_in_arc_degree"],
+                    )
+                ]
+
+                country = world[world.geometry.contains(geometry[0])]
+                phone_code = country_phone_codes.get(country.iloc[0]["name"], "Unknown")
+                phone_codes.append(phone_code)
+
+                # Save the data as a CSV file
+                sta_id = str(meta["id_from_grdc"]).zfill(8)
+                save_csv_file = f"zq_{phone_code}_grdc{sta_id}.csv"
+                save_dir = os.path.join(des_dir, "zq_stations")
+                if not os.path.exists(save_dir):
+                    os.makedirs(save_dir)
+                grdc_file_path = os.path.join(save_dir, save_csv_file)
+                df.to_csv(grdc_file_path)
+
+                gdf = gpd.GeoDataFrame([meta], geometry=geometry)
+                all_gdfs.append(gdf)  # Append the GeoDataFrame to the list
+
+            except FileNotFoundError as e:
+                print(f"Error reading data for station {grdc_file}: {e}")
+
+    # Concatenate all GeoDataFrames into a single GeoDataFrame
+    combined_gdf = pd.concat(all_gdfs)
+
+    # Set the coordinate reference system (CRS) to WGS84
+    combined_gdf.crs = "EPSG:4326"
+    # Define a dictionary where keys are old names and values are new names
+    new_column_names = {
+        "id_from_grdc": "STCD",
+        "station_name": "STNAME",
+        "grdc_latitude_in_arc_degree": "LAT",
+        "grdc_longitude_in_arc_degree": "LON",
+    }
+    # Rename the columns
+    combined_gdf = combined_gdf.rename(columns=new_column_names)
+    # Drop the columns you don't need
+    columns_to_drop = [
+        col
+        for col in combined_gdf.columns
+        if col not in new_column_names.values() and col != "geometry"
+    ]
+    combined_gdf = combined_gdf.drop(columns=columns_to_drop)
+
+    # Add new columns and set their values
+    combined_gdf["STCD"] = combined_gdf["STCD"].astype(str).str.zfill(8)
+    combined_gdf["ID"] = [
+        pc + "_grdc" + sc for pc, sc in zip(phone_codes, combined_gdf["STCD"].values)
+    ]
+    combined_gdf["STTYPE"] = "streamflow_station"
+    combined_gdf["VARTYPE"] = "streamflow"
+    combined_gdf["AGENCY"] = np.nan
+    combined_gdf["DIVISION"] = np.nan
+    combined_gdf["SOURCE"] = "GRDC"
+
+    combined_gdf = combined_gdf[STATION_LST_COLUMNS + ["geometry"]]
+    save_zq_dir = os.path.join(des_dir, "stations_list")
+    if not os.path.exists(save_zq_dir):
+        os.makedirs(save_zq_dir)
+    save_shp(combined_gdf, save_zq_dir, "zq_stations")
+    # Drop the geometry column and save as CSV
+    combined_csv_path = os.path.join(save_zq_dir, "zq_stations.csv")
+    combined_gdf.drop(columns=["geometry"]).to_csv(combined_csv_path, index=False)
+
+
+if __name__ == "__main__":
+    # Create the parser
+    parser = argparse.ArgumentParser(description="Give me paths..")
+
+    # Add the arguments
+    parser.add_argument(
+        "--grdc_path",
+        type=str,
+        help="The directory where the final ZIP file will be saved",
+        default=r"C:\Users\wenyu\.hydrodataset\cache\grdc",
+    )
+    parser.add_argument(
+        "--basin_dir",
+        type=str,
+        help="The name of the directory to move basin-files to",
+        default="D:\\data\\waterism\\basins-origin\\basins_list",
+    )
+    parser.add_argument(
+        "--station_dir",
+        type=str,
+        help="The name of the directory to upload station-files to",
+        default="D:\\data\\waterism\\stations-origin",
+    )
+    # Parse the arguments
+    args = parser.parse_args()
+    geojson_path = os.path.join(args.grdc_path, "stationbasins.geojson")
+    grdcstationdata2csvandshp(args.grdc_path, args.station_dir)
+    onegeojson2basinsshp4grdc(geojson_path, args.basin_dir)
```

### Comparing `hydrodatasource-0.0.1/hydrodatasource/processor/minio_process.py` & `hydrodatasource-0.0.2/hydrodatasource/processor/minio_process.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,177 +1,177 @@
-import ujson
-import kerchunk.hdf
-from kerchunk.combine import MultiZarrToZarr
-import kerchunk.netCDF3
-import geopandas as gpd
-import os
-import shutil
-import boto3
-
-from hydroutils.hydro_s3 import boto3_upload_file, boto3_download_file
-
-from hydrodatasource.configs.config import FS
-from hydrodatasource.configs.config import RO
-
-so = dict(
-    mode="rb", storage_options=RO, default_fill_cache=False, default_cache_type="first"
-)  # args to fs.open()
-# default_fill_cache=False avoids caching data in between file chunks to lowers memory usage.
-
-
-class HDFProcessor:
-    """
-    适用于gpm等Hdf5格式数据。
-
-    Attributes:
-
-    Method:
-    """
-
-    def __init__(self):
-        pass
-
-    def nc_to_zarr(self, nc_path, json_path):
-        with FS.open(nc_path, **so) as infile:
-            try:
-                h5chunks = kerchunk.hdf.SingleHdf5ToZarr(infile, nc_path)
-            except Exception:
-                print(nc_path, "未生成！")
-                return
-
-            with FS.open(json_path, "wb") as f:
-                f.write(ujson.dumps(h5chunks.translate()).encode())
-
-    def multi_to_zarr(
-        self, json_paths, file_path, concat_dims=None, identical_dims=None
-    ):
-        if concat_dims is None:
-            concat_dims = ["time"]
-        if identical_dims is None:
-            identical_dims = ["lat", "lon"]
-        json_list = FS.glob(json_paths)
-        json_list = [f"s3://{str}" for str in json_list]
-
-        mzz = MultiZarrToZarr(
-            json_list,
-            target_options=RO,
-            remote_protocol="s3",
-            remote_options=RO,
-            concat_dims=concat_dims,
-            identical_dims=identical_dims,
-        )
-
-        d = mzz.translate()
-
-        with FS.open(file_path) as f:
-            f.write(ujson.dumps(d).encode())
-
-
-class NC3Processor:
-    """
-    适用于era5等netCDF3格式数据。
-
-    Attributes:
-
-    Method:
-    """
-
-    def __init__(self):
-        pass
-
-    def nc_to_zarr(self, nc_path, json_path):
-        try:
-            h5chunks = kerchunk.netCDF3.netcdf_recording_file(
-                f"s3://{nc_path}", storage_options=RO
-            )
-        except Exception:
-            print(nc_path, "未生成！")
-            return
-
-        with FS.open(json_path, "wb") as f:
-            f.write(ujson.dumps(h5chunks.translate()).encode())
-
-    def multi_to_zarr(
-        self, json_paths, file_path, concat_dims=None, identical_dims=None
-    ):
-        if concat_dims is None:
-            concat_dims = ["time"]
-        if identical_dims is None:
-            identical_dims = ["latitude", "longitude"]
-        json_list = FS.glob(json_paths)
-        json_list = [f"s3://{str}" for str in json_list]
-
-        mzz = MultiZarrToZarr(
-            json_list,
-            target_options=RO,
-            remote_protocol="s3",
-            remote_options=RO,
-            concat_dims=concat_dims,
-            identical_dims=identical_dims,
-        )
-
-        d = mzz.translate()
-
-        with FS.open(file_path) as f:
-            f.write(ujson.dumps(d).encode())
-
-
-def geojson_to_shp(input_geojson, output_folder=None, keep_folder=True):
-    """Trans geojson to shp and zip it, return the path of zip file"""
-    gdf = gpd.read_file(input_geojson)
-
-    # 根据输入的GeoJSON文件确定输出路径
-    if not output_folder:
-        output_folder = os.path.join(os.path.dirname(input_geojson), "shp_output")
-
-    # 确保输出文件夹存在
-    if not os.path.exists(output_folder):
-        os.makedirs(output_folder)
-
-    # 写入Shapefile
-    base_name = os.path.splitext(os.path.basename(input_geojson))[0]
-    output_shp = os.path.join(output_folder, f"{base_name}.shp")
-    gdf.to_file(output_shp)
-
-    # 将Shapefile及其相关文件打包成ZIP文件
-    archive_path = shutil.make_archive(
-        os.path.join(os.path.dirname(output_folder), base_name), "zip", output_folder
-    )
-
-    # 根据参数决定是否删除子文件夹
-    if not keep_folder:
-        shutil.rmtree(output_folder)
-
-    return archive_path
-
-
-class GeoProcessor:
-    def __init__(self, minio_paras):
-        self.boto = boto3.client(
-            "s3",
-            endpoint_url=minio_paras["endpoint_url"],
-            aws_access_key_id=minio_paras["access_key"],
-            aws_secret_access_key=minio_paras["secret_key"],
-        )
-        self.bucket_name = minio_paras["bucket_name"]
-        self.endpoint = minio_paras["endpoint_url"].replace("http://", "")
-
-    def upload_geojson(self, gj_local_path, gj_mo_name=None, upload_shp=True):
-        """Upload geojson file and optionally its shpfile version."""
-        # 如果gj_mo_name没有提供，则使用gj_local_path的文件名
-        if gj_mo_name is None:
-            gj_mo_name = os.path.basename(gj_local_path)
-
-        if upload_shp:
-            shp_zip_path = geojson_to_shp(gj_local_path)
-            zip_name = os.path.basename(shp_zip_path)
-            boto3_upload_file(self.boto, self.bucket_name, zip_name, shp_zip_path)
-
-    def read_shp(self, shp_name):
-        """Read shpfile from minio."""
-        return gpd.read_file(
-            f"zip+http://{self.endpoint}/{self.bucket_name}/{shp_name}"
-        )
-
-    def download_shp(self, shp_name, local_path):
-        """Download shpfile from minio."""
-        boto3_download_file(self.boto, self.bucket_name, shp_name, local_path)
+import ujson
+import kerchunk.hdf
+from kerchunk.combine import MultiZarrToZarr
+import kerchunk.netCDF3
+import geopandas as gpd
+import os
+import shutil
+import boto3
+
+from hydroutils.hydro_s3 import boto3_upload_file, boto3_download_file
+
+from hydrodatasource.configs.config import FS
+from hydrodatasource.configs.config import RO
+
+so = dict(
+    mode="rb", storage_options=RO, default_fill_cache=False, default_cache_type="first"
+)  # args to fs.open()
+# default_fill_cache=False avoids caching data in between file chunks to lowers memory usage.
+
+
+class HDFProcessor:
+    """
+    适用于gpm等Hdf5格式数据。
+
+    Attributes:
+
+    Method:
+    """
+
+    def __init__(self):
+        pass
+
+    def nc_to_zarr(self, nc_path, json_path):
+        with FS.open(nc_path, **so) as infile:
+            try:
+                h5chunks = kerchunk.hdf.SingleHdf5ToZarr(infile, nc_path)
+            except Exception:
+                print(nc_path, "未生成！")
+                return
+
+            with FS.open(json_path, "wb") as f:
+                f.write(ujson.dumps(h5chunks.translate()).encode())
+
+    def multi_to_zarr(
+        self, json_paths, file_path, concat_dims=None, identical_dims=None
+    ):
+        if concat_dims is None:
+            concat_dims = ["time"]
+        if identical_dims is None:
+            identical_dims = ["lat", "lon"]
+        json_list = FS.glob(json_paths)
+        json_list = [f"s3://{str}" for str in json_list]
+
+        mzz = MultiZarrToZarr(
+            json_list,
+            target_options=RO,
+            remote_protocol="s3",
+            remote_options=RO,
+            concat_dims=concat_dims,
+            identical_dims=identical_dims,
+        )
+
+        d = mzz.translate()
+
+        with FS.open(file_path) as f:
+            f.write(ujson.dumps(d).encode())
+
+
+class NC3Processor:
+    """
+    适用于era5等netCDF3格式数据。
+
+    Attributes:
+
+    Method:
+    """
+
+    def __init__(self):
+        pass
+
+    def nc_to_zarr(self, nc_path, json_path):
+        try:
+            h5chunks = kerchunk.netCDF3.netcdf_recording_file(
+                f"s3://{nc_path}", storage_options=RO
+            )
+        except Exception:
+            print(nc_path, "未生成！")
+            return
+
+        with FS.open(json_path, "wb") as f:
+            f.write(ujson.dumps(h5chunks.translate()).encode())
+
+    def multi_to_zarr(
+        self, json_paths, file_path, concat_dims=None, identical_dims=None
+    ):
+        if concat_dims is None:
+            concat_dims = ["time"]
+        if identical_dims is None:
+            identical_dims = ["latitude", "longitude"]
+        json_list = FS.glob(json_paths)
+        json_list = [f"s3://{str}" for str in json_list]
+
+        mzz = MultiZarrToZarr(
+            json_list,
+            target_options=RO,
+            remote_protocol="s3",
+            remote_options=RO,
+            concat_dims=concat_dims,
+            identical_dims=identical_dims,
+        )
+
+        d = mzz.translate()
+
+        with FS.open(file_path) as f:
+            f.write(ujson.dumps(d).encode())
+
+
+def geojson_to_shp(input_geojson, output_folder=None, keep_folder=True):
+    """Trans geojson to shp and zip it, return the path of zip file"""
+    gdf = gpd.read_file(input_geojson)
+
+    # 根据输入的GeoJSON文件确定输出路径
+    if not output_folder:
+        output_folder = os.path.join(os.path.dirname(input_geojson), "shp_output")
+
+    # 确保输出文件夹存在
+    if not os.path.exists(output_folder):
+        os.makedirs(output_folder)
+
+    # 写入Shapefile
+    base_name = os.path.splitext(os.path.basename(input_geojson))[0]
+    output_shp = os.path.join(output_folder, f"{base_name}.shp")
+    gdf.to_file(output_shp)
+
+    # 将Shapefile及其相关文件打包成ZIP文件
+    archive_path = shutil.make_archive(
+        os.path.join(os.path.dirname(output_folder), base_name), "zip", output_folder
+    )
+
+    # 根据参数决定是否删除子文件夹
+    if not keep_folder:
+        shutil.rmtree(output_folder)
+
+    return archive_path
+
+
+class GeoProcessor:
+    def __init__(self, minio_paras):
+        self.boto = boto3.client(
+            "s3",
+            endpoint_url=minio_paras["endpoint_url"],
+            aws_access_key_id=minio_paras["access_key"],
+            aws_secret_access_key=minio_paras["secret_key"],
+        )
+        self.bucket_name = minio_paras["bucket_name"]
+        self.endpoint = minio_paras["endpoint_url"].replace("http://", "")
+
+    def upload_geojson(self, gj_local_path, gj_mo_name=None, upload_shp=True):
+        """Upload geojson file and optionally its shpfile version."""
+        # 如果gj_mo_name没有提供，则使用gj_local_path的文件名
+        if gj_mo_name is None:
+            gj_mo_name = os.path.basename(gj_local_path)
+
+        if upload_shp:
+            shp_zip_path = geojson_to_shp(gj_local_path)
+            zip_name = os.path.basename(shp_zip_path)
+            boto3_upload_file(self.boto, self.bucket_name, zip_name, shp_zip_path)
+
+    def read_shp(self, shp_name):
+        """Read shpfile from minio."""
+        return gpd.read_file(
+            f"zip+http://{self.endpoint}/{self.bucket_name}/{shp_name}"
+        )
+
+    def download_shp(self, shp_name, local_path):
+        """Download shpfile from minio."""
+        boto3_download_file(self.boto, self.bucket_name, shp_name, local_path)
```

### Comparing `hydrodatasource-0.0.1/hydrodatasource/reader/access_fs.py` & `hydrodatasource-0.0.2/hydrodatasource/reader/access_fs.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,152 +1,135 @@
-import glob
-import logging
-import os
-
-import geopandas as gpd
-import intake as intk
-import pandas as pd
-import ujson
-import xarray as xr
-import zarr
-from kerchunk.hdf import SingleHdf5ToZarr
-
-import hydrodatasource.configs.config as conf
-
-
-def spec_path(url_path: str, head="local", need_cache=False, is_dir=False):
-    if is_dir is False:
-        if head == "local":
-            url_path = os.path.join(conf.LOCAL_DATA_PATH, url_path)
-            ret_data = read_valid_data(url_path, need_cache=need_cache)
-        elif head == "minio":
-            url_path = "s3://" + url_path
-            ret_data = read_valid_data(
-                url_path, storage_option=conf.MINIO_PARAM, need_cache=need_cache
-            )
-        else:
-            raise ValueError("head should be 'local' or 'minio'")
-    else:
-        ret_data = []
-        if head == "local":
-            url_path = os.path.join(conf.LOCAL_DATA_PATH, url_path)
-            for file in glob.glob(url_path + "/**", recursive=True):
-                if not os.path.isdir(file):
-                    ret_data.append(read_valid_data(file, need_cache=need_cache))
-        elif head == "minio":
-            url_path = "s3://" + url_path
-            for file in conf.FS.glob(url_path + "/**"):
-                if not conf.FS.isdir(file):
-                    ret_data.append(
-                        read_valid_data(
-                            file, storage_option=conf.MINIO_PARAM, need_cache=need_cache
-                        )
-                    )
-        else:
-            raise ValueError("head should be 'local' or 'minio'")
-    return ret_data
-
-
-# Extract from HydroForecast
-def read_valid_data(obj: str, storage_option=None, need_cache=False, need_refer=False):
-    """
-    Read valid data from different file types.
-    See https://intake.readthedocs.io/en/latest/plugin-directory.html
-    pip install intake-xarray intake-geopandas
-
-    Parameters:
-    obj (str): The file path or URL of the data, format is 's3://bucket_name/file_name'.
-    storage_option (dict, optional): The storage options for accessing the data. Defaults to None.
-    need_cache (bool, optional): Whether to cache the data. Defaults to False.
-
-    Returns:
-    object: The data object.
-    """
-    data_obj = None
-    dot_in_obj = "." in obj
-    cache_name = obj.lstrip("s3://").split("/")[-1]
-    if not dot_in_obj:
-        data_obj = pd.read_fwf(obj, storage_options=storage_option)
-        if (need_cache is True) & (storage_option is not None):
-            data_obj.to_file(path=os.path.join(conf.LOCAL_DATA_PATH, cache_name))
-    elif dot_in_obj:
-        ext_name = obj.split(".")[-1]
-        if ext_name == "csv":
-            data_obj = pd.read_csv(obj, storage_options=storage_option)
-            if (need_cache is True) & (storage_option is not None):
-                data_obj.to_csv(path=os.path.join(conf.LOCAL_DATA_PATH, cache_name))
-        elif (
-            (ext_name == "nc")
-            or (ext_name == "nc4")
-            or (ext_name == "hdf5")
-            or (ext_name == "h5")
-        ):
-            if need_refer is True:
-                data_obj = gen_refer_and_read_zarr(obj, storage_option=storage_option)
-            else:
-                """
-                nc_source = intk.datatypes.HDF5(obj, storage_options=storage_option)
-                nc_src_reader = intk.readers.DaskHDF(nc_source).to_reader()
-                data_obj: xr.Dataset = nc_src_reader.read()
-                """
-                if (ext_name == "nc") or (ext_name == "nc4"):
-                    data_obj = xr.open_dataset(conf.FS.open(obj), chunks="auto")
-                elif (ext_name == "hdf5") or (ext_name == "h5"):
-                    data_obj = xr.open_dataset(
-                        conf.FS.open(obj),
-                        engine="h5netcdf",
-                        chunks="auto",
-                        phony_dims="access",
-                    )
-            if (need_cache is True) & (storage_option is not None):
-                data_obj.to_netcdf(path=os.path.join(conf.LOCAL_DATA_PATH, cache_name))
-        elif ext_name == "json":
-            data_obj = pd.read_json(obj, storage_options=storage_option)
-            if (need_cache is True) & (storage_option is not None):
-                data_obj.to_json(
-                    path_or_buf=os.path.join(conf.LOCAL_DATA_PATH, cache_name)
-                )
-        elif ext_name == "zip":
-            # Now zipfile is used to read shapefile
-            # Can't read shapefile directly, see this: https://github.com/geopandas/geopandas/issues/3129
-            # pip install pyogrio
-            data_obj = gpd.read_file(conf.FS.open(obj), engine="pyogrio")
-            if (need_cache is True) & (storage_option is not None):
-                data_obj.to_file(path=os.path.join(conf.LOCAL_DATA_PATH, cache_name))
-        elif "grb2" in obj:
-            # ValueError: unrecognized engine cfgrib must be one of: ['netcdf4', 'h5netcdf', 'scipy', 'store', 'zarr']
-            # https://blog.csdn.net/weixin_44052055/article/details/108658464?spm=1001.2014.3001.5501
-            # 似乎只能用conda来装eccodes
-            grib_ds = xr.open_dataset(conf.FS.open(obj))
-            if (need_cache is True) & (storage_option is not None):
-                grib_ds.to_netcdf(path=os.path.join(conf.LOCAL_DATA_PATH, cache_name))
-        elif ext_name == "txt":
-            data_obj = pd.read_fwf(obj, storage_options=storage_option)
-            if (need_cache is True) & (storage_option is not None):
-                data_obj.to_csv(os.path.join(conf.LOCAL_DATA_PATH, cache_name))
-        elif ext_name == ".zarr":
-            zarr_mapper = conf.FS.get_mapper(obj)
-            # KVStore is introduced in zarr specification V3
-            # https://zarr-specs.readthedocs.io/en/latest/v3/stores.html
-            zarr_store = zarr.storage.KVStore(zarr_mapper)
-            data_obj = xr.open_zarr(zarr_store)
-        else:
-            logging.error(f"Unsupported file type: {ext_name}")
-    else:
-        data_obj = object()
-        logging.error("这是数据存储，不是百度云盘！")
-    return data_obj
-
-
-def gen_refer_and_read_zarr(obj_path, storage_option=None):
-    # https://github.com/fsspec/kerchunk/discussions/431
-    obj_json_path = "s3://references/" + str(obj_path) + ".json"
-    if not conf.FS.exists(obj_json_path):
-        obj_path = "s3://" + obj_path
-        with conf.FS.open(obj_path, "rb") as fpj:
-            nc_chunks = SingleHdf5ToZarr(fpj, obj_path)
-            with conf.FS.open(obj_json_path, "wb") as fp:
-                fp.write(ujson.dumps(nc_chunks.translate()).encode())
-    data_type_obj = intk.datatypes.HDF5(obj_json_path, storage_options=storage_option)
-    data_reader_obj = intk.readers.XArrayDatasetReader(data_type_obj).to_reader()
-    data_obj = data_reader_obj.read()
-    return data_obj
+import glob
+import logging
+import os
+
+import geopandas as gpd
+import intake as intk
+import pandas as pd
+import ujson
+import xarray as xr
+import zarr
+from kerchunk.hdf import SingleHdf5ToZarr
+import hydrodatasource.configs.config as conf
+
+
+def spec_path(url_path: str, head='local', need_cache=False, is_dir=False):
+    if is_dir is False:
+        if head == 'local':
+            url_path = os.path.join(conf.LOCAL_DATA_PATH, url_path)
+            ret_data = read_valid_data(url_path, need_cache=need_cache)
+        elif head == 'minio':
+            url_path = 's3://' + url_path
+            ret_data = read_valid_data(url_path, storage_option=conf.MINIO_PARAM, need_cache=need_cache)
+        else:
+            raise ValueError("head should be 'local' or 'minio'")
+    else:
+        ret_data = []
+        if head == 'local':
+            url_path = os.path.join(conf.LOCAL_DATA_PATH, url_path)
+            for file in glob.glob(url_path + '/**', recursive=True):
+                if not os.path.isdir(file):
+                    ret_data.append(read_valid_data(file, need_cache=need_cache))
+        elif head == 'minio':
+            url_path = 's3://' + url_path
+            for file in conf.FS.glob(url_path + '/**'):
+                if not conf.FS.isdir(file):
+                    ret_data.append(read_valid_data(file, storage_option=conf.MINIO_PARAM, need_cache=need_cache))
+        else:
+            raise ValueError("head should be 'local' or 'minio'")
+    return ret_data
+
+
+# Extract from HydroForecast
+def read_valid_data(obj: str, storage_option=None, need_cache=False, need_refer=False):
+    """
+    Read valid data from different file types.
+    See https://intake.readthedocs.io/en/latest/plugin-directory.html
+    pip install intake-xarray intake-geopandas
+
+    Parameters:
+    obj (str): The file path or URL of the data, format is 's3://bucket_name/file_name'.
+    storage_option (dict, optional): The storage options for accessing the data. Defaults to None.
+    need_cache (bool, optional): Whether to cache the data. Defaults to False.
+
+    Returns:
+    object: The data object.
+    """
+    data_obj = None
+    dot_in_obj = '.' in obj
+    cache_name = obj.lstrip('s3://').split('/')[-1]
+    if not dot_in_obj:
+        data_obj = pd.read_fwf(obj, storage_options=storage_option)
+        if (need_cache is True) & (storage_option is not None):
+            data_obj.to_file(path=os.path.join(conf.LOCAL_DATA_PATH, cache_name))
+    elif dot_in_obj:
+        ext_name = obj.split('.')[-1]
+        if ext_name == 'csv':
+            data_obj = pd.read_csv(obj, storage_options=storage_option)
+            data_obj = xr.Dataset(data_obj)
+            if (need_cache is True) & (storage_option is not None):
+                data_obj.to_csv(path_or_buf=os.path.join(conf.LOCAL_DATA_PATH, cache_name))
+        elif (ext_name == 'nc') or (ext_name == 'nc4') or (ext_name == 'hdf5') or (ext_name == 'h5') or ('nc4' in obj):
+            if need_refer is True:
+                data_obj = gen_refer_and_read_zarr(obj, storage_option=storage_option)
+            else:
+                '''
+                nc_source = intk.datatypes.HDF5(obj, storage_options=storage_option)
+                nc_src_reader = intk.readers.DaskHDF(nc_source).to_reader()
+                data_obj: xr.Dataset = nc_src_reader.read()
+                '''
+                if (ext_name == 'nc') or (ext_name == 'nc4') or ('nc4' in obj):
+                    data_obj = xr.open_dataset(conf.FS.open(obj), chunks='auto')
+                elif (ext_name == 'hdf5') or (ext_name == 'h5'):
+                    data_obj = xr.open_dataset(conf.FS.open(obj), engine='h5netcdf', chunks='auto', phony_dims='access')
+            if (need_cache is True) & (storage_option is not None):
+                data_obj.to_netcdf(path=os.path.join(conf.LOCAL_DATA_PATH, cache_name))
+        elif ext_name == 'json':
+            data_obj = pd.read_json(obj, storage_options=storage_option)
+            if (need_cache is True) & (storage_option is not None):
+                data_obj.to_json(path_or_buf=os.path.join(conf.LOCAL_DATA_PATH, cache_name))
+        elif ext_name == 'zip':
+            # Now zipfile is used to read shapefile
+            # Can't read shapefile directly, see this: https://github.com/geopandas/geopandas/issues/3129
+            # pip install pyogrio
+            data_obj = gpd.read_file(conf.FS.open(obj), engine='pyogrio')
+            if (need_cache is True) & (storage_option is not None):
+                data_obj.to_file(path=os.path.join(conf.LOCAL_DATA_PATH, cache_name))
+        elif 'grb2' in obj:
+            # ValueError: unrecognized engine cfgrib must be one of: ['netcdf4', 'h5netcdf', 'scipy', 'store', 'zarr']
+            # https://blog.csdn.net/weixin_44052055/article/details/108658464?spm=1001.2014.3001.5501
+            # 似乎只能用conda来装eccodes
+            grib_ds = xr.open_dataset(conf.FS.open(obj))
+            if (need_cache is True) & (storage_option is not None):
+                grib_ds.to_netcdf(path=os.path.join(conf.LOCAL_DATA_PATH, cache_name))
+        elif ext_name == 'txt':
+            data_obj = pd.read_fwf(obj, storage_options=storage_option)
+            if (need_cache is True) & (storage_option is not None):
+                data_obj.to_csv(os.path.join(conf.LOCAL_DATA_PATH, cache_name))
+        elif ext_name == 'zarr':
+            zarr_mapper = conf.FS.get_mapper(obj)
+            # KVStore is introduced in zarr specification V3
+            # https://zarr-specs.readthedocs.io/en/latest/v3/stores.html
+            zarr_store = zarr.storage.KVStore(zarr_mapper)
+            data_obj = xr.open_zarr(zarr_store)
+        else:
+            logging.error(f'Unsupported file type: {ext_name}')
+    else:
+        data_obj = object()
+        logging.error("这是数据存储，不是百度云盘！")
+    return data_obj
+
+
+def gen_refer_and_read_zarr(obj_path, storage_option=None):
+    # https://github.com/fsspec/kerchunk/discussions/431
+    obj_json_path = 's3://references/' + str(obj_path) + '.json'
+    if not conf.FS.exists(obj_json_path):
+        obj_path = 's3://' + obj_path
+        with conf.FS.open(obj_path, 'rb') as fpj:
+            nc_chunks = SingleHdf5ToZarr(fpj, obj_path)
+            with conf.FS.open(obj_json_path, 'wb') as fp:
+                fp.write(ujson.dumps(nc_chunks.translate()).encode())
+    data_type_obj = intk.datatypes.HDF5(obj_json_path, storage_options=storage_option)
+    data_reader_obj = intk.readers.XArrayDatasetReader(data_type_obj).to_reader()
+    data_obj = data_reader_obj.read()
+    return data_obj
+
```

### Comparing `hydrodatasource-0.0.1/hydrodatasource/reader/era5.py` & `hydrodatasource-0.0.2/hydrodatasource/reader/era5.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,455 +1,455 @@
-"""
-该模块用于从minio中读取era5-land数据，主要方法包括：
-
-- `open_dataset` - 普通读取数据方法
-- `from_shp` - 通过已有矢量范围读取数据方法
-- `from_aoi` - 通过已有GeoDataFrame范围读取数据方法
-- `to_netcdf` - 保存到本地文件
-"""
-
-from ..configs.config import FS, MINIO_PARAM
-from ..configs.config import RO
-from ..utils.utils import regen_box
-import os
-import s3fs
-import numpy as np
-import xarray as xr
-
-bucket_name = MINIO_PARAM["bucket_name"]
-
-start = np.datetime64("2015-01-01T00:00:00.000000000")
-end = np.datetime64("2021-12-31T23:00:00.000000000")
-box = (115, 38, 136, 54)
-variables = [
-    "10 metre U wind component",
-    "10 metre V wind component",
-    "2 metre dewpoint temperature",
-    "2 metre temperature",
-    "Evaporation",
-    "Evaporation from bare soil",
-    "Evaporation from open water surfaces excluding oceans",
-    "Evaporation from the top of canopy",
-    "Evaporation from vegetation transpiration",
-    "Forecast albedo",
-    "Lake bottom temperature",
-    "Lake ice total depth",
-    "Lake ice surface temperature",
-    "Lake mix-layer depth",
-    "Lake mix-layer temperature",
-    "Lake shape factor",
-    "Lake total layer temperature",
-    "Leaf area index, high vegetation",
-    "Leaf area index, low vegetation",
-    "Potential evaporation",
-    "Runoff",
-    "Skin reservoir content",
-    "Skin temperature",
-    "Snow albedo",
-    "Snow cover",
-    "Snow density",
-    "Snow depth",
-    "Snow depth water equivalent",
-    "Snow evaporation",
-    "Snowfall",
-    "Snowmelt",
-    "Soil temperature level 1",
-    "Soil temperature level 2",
-    "Soil temperature level 3",
-    "Soil temperature level 4",
-    "Sub-surface runoff",
-    "Surface latent heat flux",
-    "Surface net solar radiation",
-    "Surface net thermal radiation",
-    "Surface pressure",
-    "Surface runoff",
-    "Surface sensible heat flux",
-    "Surface solar radiation downwards",
-    "Surface thermal radiation downwards",
-    "Temperature of snow layer",
-    "Total precipitation",
-    "Volumetric soil water layer 1",
-    "Volumetric soil water layer 2",
-    "Volumetric soil water layer 3",
-    "Volumetric soil water layer 4",
-]
-accumulated = [
-    # '10 metre U wind component',
-    # '10 metre V wind component',
-    # '2 metre dewpoint temperature',
-    # '2 metre temperature',
-    "Evaporation",
-    "Evaporation from bare soil",
-    "Evaporation from open water surfaces excluding oceans",
-    "Evaporation from the top of canopy",
-    "Evaporation from vegetation transpiration",
-    # 'Forecast albedo',
-    # 'Lake bottom temperature',
-    # 'Lake ice total depth',
-    # 'Lake ice surface temperature',
-    # 'Lake mix-layer depth',
-    # 'Lake mix-layer temperature',
-    # 'Lake shape factor',
-    # 'Lake total layer temperature',
-    # 'Leaf area index, high vegetation',
-    # 'Leaf area index, low vegetation',
-    "Potential evaporation",
-    "Runoff",
-    # 'Skin reservoir content',
-    # 'Skin temperature',
-    # 'Snow albedo',
-    # 'Snow cover',
-    # 'Snow density',
-    # 'Snow depth',
-    # 'Snow depth water equivalent',
-    "Snow evaporation",
-    "Snowfall",
-    "Snowmelt",
-    # 'Soil temperature level 1',
-    # 'Soil temperature level 2',
-    # 'Soil temperature level 3',
-    # 'Soil temperature level 4',
-    "Sub-surface runoff",
-    "Surface latent heat flux",
-    "Surface net solar radiation",
-    "Surface net thermal radiation",
-    # 'Surface pressure',
-    "Surface runoff",
-    "Surface sensible heat flux",
-    "Surface solar radiation downwards",
-    "Surface thermal radiation downwards",
-    # 'Temperature of snow layer',
-    "Total precipitation",
-    # 'Volumetric soil water layer 1',
-    # 'Volumetric soil water layer 2',
-    # 'Volumetric soil water layer 3',
-    # 'Volumetric soil water layer 4'
-]
-
-
-def open_dataset(
-    data_variables=variables, start_time=start, end_time=end, bbox=box, time_chunks=24
-):
-    """
-    从minio服务器读取era5-land数据
-
-    Args:
-        data_variables (list): 数据变量列表
-        start_time (datetime64): 开始时间
-        end_time (datetime64): 结束时间
-        bbox (list|tuple): 四至范围
-        time_chunks (int): 分块数量
-
-    Returns:
-        dataset (Dataset): 读取结果
-    """
-
-    chunks = {"time": time_chunks}
-    ds = xr.open_dataset(
-        "reference://",
-        engine="zarr",
-        chunks=chunks,
-        backend_kwargs={
-            "consolidated": False,
-            "storage_options": {
-                "fo": FS.open(f"s3://{bucket_name}/geodata/era5_land/era5_land_.json"),
-                "remote_protocol": "s3",
-                "remote_options": RO,
-            },
-        },
-    )
-
-    ds = ds.filter_by_attrs(long_name=lambda v: v in data_variables)
-    ds = ds.rename({"longitude": "lon", "latitude": "lat"})
-    ds = ds.transpose("time", "lon", "lat")
-
-    start_time = max(start_time, start)
-    end_time = min(end_time, end)
-    times = slice(start_time, end_time)
-    ds = ds.sel(time=times)
-
-    bbox = regen_box(bbox, 0.1, 0)
-
-    if bbox[0] < box[0]:
-        left = box[0]
-    else:
-        left = bbox[0]
-
-    if bbox[1] < box[1]:
-        bottom = box[1]
-    else:
-        bottom = bbox[1]
-
-    if bbox[2] > box[2]:
-        right = box[2]
-    else:
-        right = bbox[2]
-
-    if bbox[3] > box[3]:
-        top = box[3]
-    else:
-        top = bbox[3]
-
-    longitudes = slice(left - 0.00001, right + 0.00001)
-    latitudes = slice(bottom - 0.00001, top + 0.00001)
-
-    ds = ds.sortby("lat", ascending=True)
-    ds = ds.sel(lon=longitudes, lat=latitudes)
-
-    return ds
-
-
-import geopandas as gpd
-
-
-def from_shp(
-    data_variables=variables, start_time=start, end_time=end, shp=None, time_chunks=24
-):
-    """
-    通过已有的矢量数据范围从minio服务器读取era5-land数据
-
-    Args:
-        data_variables (list): 数据变量列表
-        start_time (datetime64): 开始时间
-        end_time (datetime64): 结束时间
-        shp (str): 矢量数据路径
-        time_chunks (int): 分块数量
-
-    Returns:
-        dataset (Dataset): 读取结果
-    """
-
-    gdf = gpd.GeoDataFrame.from_file(shp)
-    b = gdf.bounds
-    bbox = regen_box(
-        (b.loc[0]["minx"], b.loc[0]["miny"], b.loc[0]["maxx"], b.loc[0]["maxy"]), 0.1, 0
-    )
-
-    return open_dataset(data_variables, start_time, end_time, bbox, time_chunks)
-
-
-def from_aoi(
-    data_variables=variables,
-    start_time=start,
-    end_time=end,
-    aoi: gpd.GeoDataFrame = None,
-    time_chunks=24,
-):
-    """
-    用过已有的GeoPandas.GeoDataFrame对象从minio服务器读取era5-land数据
-
-    Args:
-        data_variables (list): 数据变量列表
-        start_time (datetime64): 开始时间
-        end_time (datetime64): 结束时间
-        aoi (GeoDataFrame): 已有的GeoPandas.GeoDataFrame对象
-        time_chunks (int): 分块数量
-
-    Returns:
-        dataset (Dataset): 读取结果
-    """
-
-    b = aoi.bounds
-    bbox = regen_box(
-        (b.loc[0]["minx"], b.loc[0]["miny"], b.loc[0]["maxx"], b.loc[0]["maxy"]), 0.1, 0
-    )
-
-    return open_dataset(data_variables, start_time, end_time, bbox, time_chunks)
-
-
-from netCDF4 import Dataset, date2num, num2date
-import time
-from datetime import datetime, timedelta
-
-
-def _creatspinc(value, data_vars, lats, lons, starttime, filename, resolution):
-    gridspi = Dataset(filename, "w", format="NETCDF4")
-
-    # dimensions
-    gridspi.createDimension("time", value[0].shape[0])
-    gridspi.createDimension("lat", value[0].shape[2])  # len(lat)
-    gridspi.createDimension("lon", value[0].shape[1])
-
-    # Create coordinate variables for dimensions
-    times = gridspi.createVariable("time", np.float64, ("time",))
-    latitudes = gridspi.createVariable("lat", np.float32, ("lat",))
-    longitudes = gridspi.createVariable("lon", np.float32, ("lon",))
-
-    # Create the actual variable
-    for var, attr in data_vars.items():
-        gridspi.createVariable(
-            var,
-            np.float32,
-            (
-                "time",
-                "lon",
-                "lat",
-            ),
-        )
-
-    # Global Attributes
-    gridspi.description = "var"
-    gridspi.history = f"Created {time.ctime(time.time())}"
-    gridspi.source = "netCDF4 python module tutorial"
-
-    # Variable Attributes
-    latitudes.units = "degree_north"
-    longitudes.units = "degree_east"
-    times.units = "days since 1970-01-01 00:00:00"
-    times.calendar = "gregorian"
-
-    # data
-    latitudes[:] = lats
-    longitudes[:] = lons
-
-    # Fill in times
-    dates = []
-    if resolution == "daily":
-        dates.extend(starttime + n for n in range(value[0].shape[0]))
-        times[:] = dates[:]
-
-    elif resolution == "6-hourly":
-        # for n in range(value[0].shape[0]):
-        #     dates.append(starttime + (n+1) * np.timedelta64(6, 'h'))
-
-        dates.extend(
-            starttime + (n + 1) * timedelta(hours=6) for n in range(value[0].shape[0])
-        )
-        times[:] = date2num(dates, units=times.units, calendar=times.calendar)
-        # print 'time values (in units %s): ' % times.units +'\n', times[:]
-        dates = num2date(times[:], units=times.units, calendar=times.calendar)
-
-    # Fill in values
-    i = 0
-    for var, attr in data_vars.items():
-        gridspi.variables[var].long_name = attr["long_name"]
-        gridspi.variables[var].units = attr["units"]
-        gridspi.variables[var][:] = value[i][:]
-        i = i + 1
-
-    gridspi.close()
-
-
-def to_netcdf(
-    data_variables=variables,
-    start_time=start,
-    end_time=end,
-    shp=None,
-    resolution="hourly",
-    save_file="era5.nc",
-    time_chunks=24,
-):
-    """
-    读取数据并保存为本地nc文件
-
-    Args:
-        data_variables (list): 数据变量列表
-        start_time (datetime64): 开始时间
-        end_time (datetime64): 结束时间
-        shp (str): 已有的矢量数据路径
-        resolution (str): 输出的时间分辨率
-        save_file (str): 输出的文件路径
-        time_chunks (int): 分块数量
-
-    Returns:
-        dataset (Dataset): 读取结果
-    """
-
-    gdf = gpd.GeoDataFrame.from_file(shp)
-    b = gdf.bounds
-    bbox = regen_box(
-        (b.loc[0]["minx"], b.loc[0]["miny"], b.loc[0]["maxx"], b.loc[0]["maxy"]), 0.1, 0
-    )
-
-    if resolution == "hourly":
-        ds = open_dataset(data_variables, start_time, end_time, bbox, time_chunks)
-
-        if ds.to_netcdf(save_file) is None:
-            print(save_file, "已生成")
-            ds = xr.open_dataset(save_file)
-            return ds
-
-    if resolution == "daily":
-        start_time = np.datetime64(f"{str(start_time)[:10]}T01:00:00.000000000")
-        end_time = np.datetime64(str(end_time)[:10]) + 1
-        end_time = np.datetime64(f"{str(end_time)}T00:00:00.000000000")
-
-        ds = open_dataset(data_variables, start_time, end_time, bbox, time_chunks)
-
-        days = ds["time"].size // 24
-
-        data_vars = {k: v.attrs for k, v in ds.data_vars.items()}
-        daily_arr = []
-
-        for var, attr in data_vars.items():
-            a = ds[var].to_numpy()
-
-            if attr["long_name"] in accumulated:
-                xlist = [x for x in range(a.shape[0]) if x % 24 != 23]
-                _a = np.delete(a, xlist, axis=0)
-
-                daily_arr.append(_a)
-
-            else:
-                r = np.split(a, days, axis=0)
-                _r = [
-                    np.expand_dims(np.mean(r[i], axis=0), axis=0) for i in range(len(r))
-                ]
-                __r = np.concatenate(_r)
-
-                daily_arr.append(__r)
-
-        lats = ds["lat"].to_numpy()
-        lons = ds["lon"].to_numpy()
-
-        start_time = np.datetime64(str(start_time)[:10])
-
-        _creatspinc(daily_arr, data_vars, lats, lons, start_time, save_file, "daily")
-
-        new = xr.open_dataset(save_file)
-        print(save_file, "已生成")
-        return new
-
-    if resolution == "6-hourly":
-        start_time = np.datetime64(f"{str(start_time)[:10]}T01:00:00.000000000")
-        end_time = np.datetime64(str(end_time)[:10]) + 1
-        end_time = np.datetime64(f"{str(end_time)}T00:00:00.000000000")
-
-        ds = open_dataset(data_variables, start_time, end_time, bbox, time_chunks)
-
-        days = ds["time"].size // 6
-
-        data_vars = {k: v.attrs for k, v in ds.data_vars.items()}
-        daily_arr = []
-
-        for var, attr in data_vars.items():
-            a = ds[var].to_numpy()
-
-            if attr["long_name"] in accumulated:
-                xlist = [x for x in range(a.shape[0]) if x % 6 != 5]
-                _a = np.delete(a, xlist, axis=0)
-
-                daily_arr.append(_a)
-
-            else:
-                r = np.split(a, days, axis=0)
-                _r = [
-                    np.expand_dims(np.mean(r[i], axis=0), axis=0) for i in range(len(r))
-                ]
-                __r = np.concatenate(_r)
-
-                daily_arr.append(__r)
-
-        lats = ds["lat"].to_numpy()
-        lons = ds["lon"].to_numpy()
-
-        # start_time = np.datetime64(f'{str(start_time)[:10]}')
-        year = int(f"{str(start_time)[:4]}")
-        month = int(f"{str(start_time)[5:7]}")
-        day = int(f"{str(start_time)[8:10]}")
-        dt = datetime(year, month, day, 0, 0, 0)
-
-        _creatspinc(daily_arr, data_vars, lats, lons, dt, save_file, "6-hourly")
-
-        new = xr.open_dataset(save_file)
-        print(save_file, "已生成")
-        return new
+"""
+该模块用于从minio中读取era5-land数据，主要方法包括：
+
+- `open_dataset` - 普通读取数据方法
+- `from_shp` - 通过已有矢量范围读取数据方法
+- `from_aoi` - 通过已有GeoDataFrame范围读取数据方法
+- `to_netcdf` - 保存到本地文件
+"""
+
+from ..configs.config import FS, MINIO_PARAM
+from ..configs.config import RO
+from ..utils.utils import regen_box
+import os
+import s3fs
+import numpy as np
+import xarray as xr
+
+bucket_name = MINIO_PARAM["bucket_name"]
+
+start = np.datetime64("2015-01-01T00:00:00.000000000")
+end = np.datetime64("2021-12-31T23:00:00.000000000")
+box = (115, 38, 136, 54)
+variables = [
+    "10 metre U wind component",
+    "10 metre V wind component",
+    "2 metre dewpoint temperature",
+    "2 metre temperature",
+    "Evaporation",
+    "Evaporation from bare soil",
+    "Evaporation from open water surfaces excluding oceans",
+    "Evaporation from the top of canopy",
+    "Evaporation from vegetation transpiration",
+    "Forecast albedo",
+    "Lake bottom temperature",
+    "Lake ice total depth",
+    "Lake ice surface temperature",
+    "Lake mix-layer depth",
+    "Lake mix-layer temperature",
+    "Lake shape factor",
+    "Lake total layer temperature",
+    "Leaf area index, high vegetation",
+    "Leaf area index, low vegetation",
+    "Potential evaporation",
+    "Runoff",
+    "Skin reservoir content",
+    "Skin temperature",
+    "Snow albedo",
+    "Snow cover",
+    "Snow density",
+    "Snow depth",
+    "Snow depth water equivalent",
+    "Snow evaporation",
+    "Snowfall",
+    "Snowmelt",
+    "Soil temperature level 1",
+    "Soil temperature level 2",
+    "Soil temperature level 3",
+    "Soil temperature level 4",
+    "Sub-surface runoff",
+    "Surface latent heat flux",
+    "Surface net solar radiation",
+    "Surface net thermal radiation",
+    "Surface pressure",
+    "Surface runoff",
+    "Surface sensible heat flux",
+    "Surface solar radiation downwards",
+    "Surface thermal radiation downwards",
+    "Temperature of snow layer",
+    "Total precipitation",
+    "Volumetric soil water layer 1",
+    "Volumetric soil water layer 2",
+    "Volumetric soil water layer 3",
+    "Volumetric soil water layer 4",
+]
+accumulated = [
+    # '10 metre U wind component',
+    # '10 metre V wind component',
+    # '2 metre dewpoint temperature',
+    # '2 metre temperature',
+    "Evaporation",
+    "Evaporation from bare soil",
+    "Evaporation from open water surfaces excluding oceans",
+    "Evaporation from the top of canopy",
+    "Evaporation from vegetation transpiration",
+    # 'Forecast albedo',
+    # 'Lake bottom temperature',
+    # 'Lake ice total depth',
+    # 'Lake ice surface temperature',
+    # 'Lake mix-layer depth',
+    # 'Lake mix-layer temperature',
+    # 'Lake shape factor',
+    # 'Lake total layer temperature',
+    # 'Leaf area index, high vegetation',
+    # 'Leaf area index, low vegetation',
+    "Potential evaporation",
+    "Runoff",
+    # 'Skin reservoir content',
+    # 'Skin temperature',
+    # 'Snow albedo',
+    # 'Snow cover',
+    # 'Snow density',
+    # 'Snow depth',
+    # 'Snow depth water equivalent',
+    "Snow evaporation",
+    "Snowfall",
+    "Snowmelt",
+    # 'Soil temperature level 1',
+    # 'Soil temperature level 2',
+    # 'Soil temperature level 3',
+    # 'Soil temperature level 4',
+    "Sub-surface runoff",
+    "Surface latent heat flux",
+    "Surface net solar radiation",
+    "Surface net thermal radiation",
+    # 'Surface pressure',
+    "Surface runoff",
+    "Surface sensible heat flux",
+    "Surface solar radiation downwards",
+    "Surface thermal radiation downwards",
+    # 'Temperature of snow layer',
+    "Total precipitation",
+    # 'Volumetric soil water layer 1',
+    # 'Volumetric soil water layer 2',
+    # 'Volumetric soil water layer 3',
+    # 'Volumetric soil water layer 4'
+]
+
+
+def open_dataset(
+    data_variables=variables, start_time=start, end_time=end, bbox=box, time_chunks=24
+):
+    """
+    从minio服务器读取era5-land数据
+
+    Args:
+        data_variables (list): 数据变量列表
+        start_time (datetime64): 开始时间
+        end_time (datetime64): 结束时间
+        bbox (list|tuple): 四至范围
+        time_chunks (int): 分块数量
+
+    Returns:
+        dataset (Dataset): 读取结果
+    """
+
+    chunks = {"time": time_chunks}
+    ds = xr.open_dataset(
+        "reference://",
+        engine="zarr",
+        chunks=chunks,
+        backend_kwargs={
+            "consolidated": False,
+            "storage_options": {
+                "fo": FS.open(f"s3://{bucket_name}/geodata/era5_land/era5_land_.json"),
+                "remote_protocol": "s3",
+                "remote_options": RO,
+            },
+        },
+    )
+
+    ds = ds.filter_by_attrs(long_name=lambda v: v in data_variables)
+    ds = ds.rename({"longitude": "lon", "latitude": "lat"})
+    ds = ds.transpose("time", "lon", "lat")
+
+    start_time = max(start_time, start)
+    end_time = min(end_time, end)
+    times = slice(start_time, end_time)
+    ds = ds.sel(time=times)
+
+    bbox = regen_box(bbox, 0.1, 0)
+
+    if bbox[0] < box[0]:
+        left = box[0]
+    else:
+        left = bbox[0]
+
+    if bbox[1] < box[1]:
+        bottom = box[1]
+    else:
+        bottom = bbox[1]
+
+    if bbox[2] > box[2]:
+        right = box[2]
+    else:
+        right = bbox[2]
+
+    if bbox[3] > box[3]:
+        top = box[3]
+    else:
+        top = bbox[3]
+
+    longitudes = slice(left - 0.00001, right + 0.00001)
+    latitudes = slice(bottom - 0.00001, top + 0.00001)
+
+    ds = ds.sortby("lat", ascending=True)
+    ds = ds.sel(lon=longitudes, lat=latitudes)
+
+    return ds
+
+
+import geopandas as gpd
+
+
+def from_shp(
+    data_variables=variables, start_time=start, end_time=end, shp=None, time_chunks=24
+):
+    """
+    通过已有的矢量数据范围从minio服务器读取era5-land数据
+
+    Args:
+        data_variables (list): 数据变量列表
+        start_time (datetime64): 开始时间
+        end_time (datetime64): 结束时间
+        shp (str): 矢量数据路径
+        time_chunks (int): 分块数量
+
+    Returns:
+        dataset (Dataset): 读取结果
+    """
+
+    gdf = gpd.GeoDataFrame.from_file(shp)
+    b = gdf.bounds
+    bbox = regen_box(
+        (b.loc[0]["minx"], b.loc[0]["miny"], b.loc[0]["maxx"], b.loc[0]["maxy"]), 0.1, 0
+    )
+
+    return open_dataset(data_variables, start_time, end_time, bbox, time_chunks)
+
+
+def from_aoi(
+    data_variables=variables,
+    start_time=start,
+    end_time=end,
+    aoi: gpd.GeoDataFrame = None,
+    time_chunks=24,
+):
+    """
+    用过已有的GeoPandas.GeoDataFrame对象从minio服务器读取era5-land数据
+
+    Args:
+        data_variables (list): 数据变量列表
+        start_time (datetime64): 开始时间
+        end_time (datetime64): 结束时间
+        aoi (GeoDataFrame): 已有的GeoPandas.GeoDataFrame对象
+        time_chunks (int): 分块数量
+
+    Returns:
+        dataset (Dataset): 读取结果
+    """
+
+    b = aoi.bounds
+    bbox = regen_box(
+        (b.loc[0]["minx"], b.loc[0]["miny"], b.loc[0]["maxx"], b.loc[0]["maxy"]), 0.1, 0
+    )
+
+    return open_dataset(data_variables, start_time, end_time, bbox, time_chunks)
+
+
+from netCDF4 import Dataset, date2num, num2date
+import time
+from datetime import datetime, timedelta
+
+
+def _creatspinc(value, data_vars, lats, lons, starttime, filename, resolution):
+    gridspi = Dataset(filename, "w", format="NETCDF4")
+
+    # dimensions
+    gridspi.createDimension("time", value[0].shape[0])
+    gridspi.createDimension("lat", value[0].shape[2])  # len(lat)
+    gridspi.createDimension("lon", value[0].shape[1])
+
+    # Create coordinate variables for dimensions
+    times = gridspi.createVariable("time", np.float64, ("time",))
+    latitudes = gridspi.createVariable("lat", np.float32, ("lat",))
+    longitudes = gridspi.createVariable("lon", np.float32, ("lon",))
+
+    # Create the actual variable
+    for var, attr in data_vars.items():
+        gridspi.createVariable(
+            var,
+            np.float32,
+            (
+                "time",
+                "lon",
+                "lat",
+            ),
+        )
+
+    # Global Attributes
+    gridspi.description = "var"
+    gridspi.history = f"Created {time.ctime(time.time())}"
+    gridspi.source = "netCDF4 python module tutorial"
+
+    # Variable Attributes
+    latitudes.units = "degree_north"
+    longitudes.units = "degree_east"
+    times.units = "days since 1970-01-01 00:00:00"
+    times.calendar = "gregorian"
+
+    # data
+    latitudes[:] = lats
+    longitudes[:] = lons
+
+    # Fill in times
+    dates = []
+    if resolution == "daily":
+        dates.extend(starttime + n for n in range(value[0].shape[0]))
+        times[:] = dates[:]
+
+    elif resolution == "6-hourly":
+        # for n in range(value[0].shape[0]):
+        #     dates.append(starttime + (n+1) * np.timedelta64(6, 'h'))
+
+        dates.extend(
+            starttime + (n + 1) * timedelta(hours=6) for n in range(value[0].shape[0])
+        )
+        times[:] = date2num(dates, units=times.units, calendar=times.calendar)
+        # print 'time values (in units %s): ' % times.units +'\n', times[:]
+        dates = num2date(times[:], units=times.units, calendar=times.calendar)
+
+    # Fill in values
+    i = 0
+    for var, attr in data_vars.items():
+        gridspi.variables[var].long_name = attr["long_name"]
+        gridspi.variables[var].units = attr["units"]
+        gridspi.variables[var][:] = value[i][:]
+        i = i + 1
+
+    gridspi.close()
+
+
+def to_netcdf(
+    data_variables=variables,
+    start_time=start,
+    end_time=end,
+    shp=None,
+    resolution="hourly",
+    save_file="era5.nc",
+    time_chunks=24,
+):
+    """
+    读取数据并保存为本地nc文件
+
+    Args:
+        data_variables (list): 数据变量列表
+        start_time (datetime64): 开始时间
+        end_time (datetime64): 结束时间
+        shp (str): 已有的矢量数据路径
+        resolution (str): 输出的时间分辨率
+        save_file (str): 输出的文件路径
+        time_chunks (int): 分块数量
+
+    Returns:
+        dataset (Dataset): 读取结果
+    """
+
+    gdf = gpd.GeoDataFrame.from_file(shp)
+    b = gdf.bounds
+    bbox = regen_box(
+        (b.loc[0]["minx"], b.loc[0]["miny"], b.loc[0]["maxx"], b.loc[0]["maxy"]), 0.1, 0
+    )
+
+    if resolution == "hourly":
+        ds = open_dataset(data_variables, start_time, end_time, bbox, time_chunks)
+
+        if ds.to_netcdf(save_file) is None:
+            print(save_file, "已生成")
+            ds = xr.open_dataset(save_file)
+            return ds
+
+    if resolution == "daily":
+        start_time = np.datetime64(f"{str(start_time)[:10]}T01:00:00.000000000")
+        end_time = np.datetime64(str(end_time)[:10]) + 1
+        end_time = np.datetime64(f"{str(end_time)}T00:00:00.000000000")
+
+        ds = open_dataset(data_variables, start_time, end_time, bbox, time_chunks)
+
+        days = ds["time"].size // 24
+
+        data_vars = {k: v.attrs for k, v in ds.data_vars.items()}
+        daily_arr = []
+
+        for var, attr in data_vars.items():
+            a = ds[var].to_numpy()
+
+            if attr["long_name"] in accumulated:
+                xlist = [x for x in range(a.shape[0]) if x % 24 != 23]
+                _a = np.delete(a, xlist, axis=0)
+
+                daily_arr.append(_a)
+
+            else:
+                r = np.split(a, days, axis=0)
+                _r = [
+                    np.expand_dims(np.mean(r[i], axis=0), axis=0) for i in range(len(r))
+                ]
+                __r = np.concatenate(_r)
+
+                daily_arr.append(__r)
+
+        lats = ds["lat"].to_numpy()
+        lons = ds["lon"].to_numpy()
+
+        start_time = np.datetime64(str(start_time)[:10])
+
+        _creatspinc(daily_arr, data_vars, lats, lons, start_time, save_file, "daily")
+
+        new = xr.open_dataset(save_file)
+        print(save_file, "已生成")
+        return new
+
+    if resolution == "6-hourly":
+        start_time = np.datetime64(f"{str(start_time)[:10]}T01:00:00.000000000")
+        end_time = np.datetime64(str(end_time)[:10]) + 1
+        end_time = np.datetime64(f"{str(end_time)}T00:00:00.000000000")
+
+        ds = open_dataset(data_variables, start_time, end_time, bbox, time_chunks)
+
+        days = ds["time"].size // 6
+
+        data_vars = {k: v.attrs for k, v in ds.data_vars.items()}
+        daily_arr = []
+
+        for var, attr in data_vars.items():
+            a = ds[var].to_numpy()
+
+            if attr["long_name"] in accumulated:
+                xlist = [x for x in range(a.shape[0]) if x % 6 != 5]
+                _a = np.delete(a, xlist, axis=0)
+
+                daily_arr.append(_a)
+
+            else:
+                r = np.split(a, days, axis=0)
+                _r = [
+                    np.expand_dims(np.mean(r[i], axis=0), axis=0) for i in range(len(r))
+                ]
+                __r = np.concatenate(_r)
+
+                daily_arr.append(__r)
+
+        lats = ds["lat"].to_numpy()
+        lons = ds["lon"].to_numpy()
+
+        # start_time = np.datetime64(f'{str(start_time)[:10]}')
+        year = int(f"{str(start_time)[:4]}")
+        month = int(f"{str(start_time)[5:7]}")
+        day = int(f"{str(start_time)[8:10]}")
+        dt = datetime(year, month, day, 0, 0, 0)
+
+        _creatspinc(daily_arr, data_vars, lats, lons, dt, save_file, "6-hourly")
+
+        new = xr.open_dataset(save_file)
+        print(save_file, "已生成")
+        return new
```

### Comparing `hydrodatasource-0.0.1/hydrodatasource/reader/gfs.py` & `hydrodatasource-0.0.2/hydrodatasource/reader/gfs.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,216 +1,216 @@
-"""
-该模块用于从minio中读取gfs数据，主要方法包括：
-
-- `open_dataset` - 普通读取数据方法
-- `from_shp` - 通过已有矢量范围读取数据方法
-- `from_aoi` - 通过已有GeoDataFrame范围读取数据方法
-"""
-
-import os
-import numpy as np
-import s3fs
-import xarray as xr
-import calendar
-from datetime import date
-import json
-
-from ..configs.config import FS, MINIO_PARAM
-
-from ..configs.config import RO
-from ..utils.utils import regen_box
-
-bucket_name = MINIO_PARAM["bucket_name"]
-
-# 后期从minio读取
-start = np.datetime64("2016-07-10")
-end = np.datetime64("2023-08-17")
-change = np.datetime64("2022-09-01")
-# change_date = date(2022,9,1)
-box = (115, 38, 136, 54)
-
-
-# 2t  ----- temperature_2m_above_ground
-# 2sh ----- specific_humidity_2m_above_ground
-# 2r  ----- relative_humidity_2m_above_ground
-# 10u ----- u_component_of_wind_10m_above_ground
-# 10v ----- v_component_of_wind_10m_above_ground
-# tp  ----- total_precipitation_surface
-# pwat----- precipitable_water_entire_atmosphere
-# tcc ----- total_cloud_cover_entire_atmosphere
-# dswrf ----- downward_shortwave_radiation_flux
-
-variables = {
-    "dswrf": "downward_shortwave_radiation_flux",
-    "pwat": "precipitable_water_entire_atmosphere",
-    "2r": "relative_humidity_2m_above_ground",
-    "2sh": "specific_humidity_2m_above_ground",
-    "2t": "temperature_2m_above_ground",
-    "tcc": "total_cloud_cover_entire_atmosphere",
-    "tp": "total_precipitation_surface",
-    "10u": "u_component_of_wind_10m_above_ground",
-    "10v": "v_component_of_wind_10m_above_ground",
-}
-
-
-def open_dataset(
-    data_variable="tp",
-    creation_date=np.datetime64("2022-09-01"),
-    creation_time="00",
-    bbox=box,
-    time_chunks=24,
-):
-    """
-    从minio服务器读取gfs数据
-
-    Args:
-        data_variables (str): 数据变量，目前只支持tp，即降雨
-        creation_date (datetime64): 创建日期
-        creation_time (datetime64): 创建时间，即00\06\12\18之一
-        bbox (list|tuple): 四至范围
-        time_chunks (int): 分块数量
-
-    Returns:
-        dataset (Dataset): 读取结果
-    """
-
-    if data_variable in variables.keys():
-        short_name = data_variable
-        full_name = variables[data_variable]
-
-        with FS.open(f"{bucket_name}/geodata/gfs/gfs.json") as f:
-            cont = json.load(f)
-            start = np.datetime64(cont[short_name][0]["start"])
-            end = np.datetime64(cont[short_name][-1]["end"])
-
-        if creation_date < start or creation_date > end:
-            print("超出时间范围！")
-            return
-
-        if creation_time not in ["00", "06", "12", "18"]:
-            print("creation_time必须是00、06、12、18之一！")
-            return
-
-        year = str(creation_date.astype("object").year)
-        month = str(creation_date.astype("object").month).zfill(2)
-        day = str(creation_date.astype("object").day).zfill(2)
-
-        if creation_date < change:
-            json_url = f"s3://{bucket_name}/geodata/gfs/gfs_history/{year}/{month}/{day}/gfs{year}{month}{day}.t{creation_time}z.0p25.json"
-        else:
-            json_url = f"s3://{bucket_name}/geodata/gfs/{short_name}/{year}/{month}/{day}/gfs{year}{month}{day}.t{creation_time}z.0p25.json"
-
-        chunks = {"valid_time": time_chunks}
-        ds = xr.open_dataset(
-            "reference://",
-            engine="zarr",
-            chunks=chunks,
-            backend_kwargs={
-                "consolidated": False,
-                "storage_options": {
-                    "fo": FS.open(json_url),
-                    "remote_protocol": "s3",
-                    "remote_options": RO,
-                },
-            },
-        )
-
-        if creation_date < change:
-            ds = ds[full_name]
-
-        # ds = ds.filter_by_attrs(long_name=lambda v: v in data_variables)
-        ds = ds.rename({"longitude": "lon", "latitude": "lat"})
-        # ds = ds.transpose('time','valid_time','lon','lat')
-
-        bbox = regen_box(bbox, 0.25, 0)
-
-        if bbox[0] < box[0]:
-            left = box[0]
-        else:
-            left = bbox[0]
-
-        if bbox[1] < box[1]:
-            bottom = box[1]
-        else:
-            bottom = bbox[1]
-
-        if bbox[2] > box[2]:
-            right = box[2]
-        else:
-            right = bbox[2]
-
-        if bbox[3] > box[3]:
-            top = box[3]
-        else:
-            top = bbox[3]
-
-        longitudes = slice(left - 0.00001, right + 0.00001)
-        latitudes = slice(bottom - 0.00001, top + 0.00001)
-
-        ds = ds.sortby("lat", ascending=True)
-        ds = ds.sel(lon=longitudes, lat=latitudes)
-
-        return ds
-
-    else:
-        print("变量名不存在！")
-
-
-import geopandas as gpd
-
-
-def from_shp(
-    data_variable="tp",
-    creation_date=np.datetime64("2022-09-01"),
-    creation_time="00",
-    shp=None,
-    time_chunks=24,
-):
-    """
-    通过已有的矢量数据范围从minio服务器读取gfs数据
-
-    Args:
-        data_variables (str): 数据变量，目前只支持tp，即降雨
-        creation_date (datetime64): 创建日期
-        creation_time (datetime64): 创建时间，即00\06\12\18之一
-        shp (str): 矢量数据路径
-        time_chunks (int): 分块数量
-
-    Returns:
-        dataset (Dataset): 读取结果
-    """
-
-    gdf = gpd.GeoDataFrame.from_file(shp)
-    b = gdf.bounds
-    bbox = regen_box(
-        (b.loc[0]["minx"], b.loc[0]["miny"], b.loc[0]["maxx"], b.loc[0]["maxy"]), 0.1, 0
-    )
-
-    return open_dataset(data_variable, creation_date, creation_time, bbox, time_chunks)
-
-
-def from_aoi(
-    data_variable="tp",
-    creation_date=np.datetime64("2022-09-01"),
-    creation_time="00",
-    aoi: gpd.GeoDataFrame = None,
-    time_chunks=24,
-):
-    """
-    通过已有的GeoPandas.GeoDataFrame对象从minio服务器读取gfs数据
-
-    Args:
-        data_variables (str): 数据变量，目前只支持tp，即降雨
-        creation_date (datetime64): 创建日期
-        creation_time (datetime64): 创建时间，即00\06\12\18之一
-        aoi (GeoDataFrame): 已有的GeoPandas.GeoDataFrame对象
-        time_chunks (int): 分块数量
-
-    Returns:
-        dataset (Dataset): 读取结果
-    """
-    b = aoi.bounds
-    bbox = regen_box(
-        (b.loc[0]["minx"], b.loc[0]["miny"], b.loc[0]["maxx"], b.loc[0]["maxy"]), 0.1, 0
-    )
-
-    return open_dataset(data_variable, creation_date, creation_time, bbox, time_chunks)
+"""
+该模块用于从minio中读取gfs数据，主要方法包括：
+
+- `open_dataset` - 普通读取数据方法
+- `from_shp` - 通过已有矢量范围读取数据方法
+- `from_aoi` - 通过已有GeoDataFrame范围读取数据方法
+"""
+
+import os
+import numpy as np
+import s3fs
+import xarray as xr
+import calendar
+from datetime import date
+import json
+
+from ..configs.config import FS, MINIO_PARAM
+
+from ..configs.config import RO
+from ..utils.utils import regen_box
+
+bucket_name = MINIO_PARAM["bucket_name"]
+
+# 后期从minio读取
+start = np.datetime64("2016-07-10")
+end = np.datetime64("2023-08-17")
+change = np.datetime64("2022-09-01")
+# change_date = date(2022,9,1)
+box = (115, 38, 136, 54)
+
+
+# 2t  ----- temperature_2m_above_ground
+# 2sh ----- specific_humidity_2m_above_ground
+# 2r  ----- relative_humidity_2m_above_ground
+# 10u ----- u_component_of_wind_10m_above_ground
+# 10v ----- v_component_of_wind_10m_above_ground
+# tp  ----- total_precipitation_surface
+# pwat----- precipitable_water_entire_atmosphere
+# tcc ----- total_cloud_cover_entire_atmosphere
+# dswrf ----- downward_shortwave_radiation_flux
+
+variables = {
+    "dswrf": "downward_shortwave_radiation_flux",
+    "pwat": "precipitable_water_entire_atmosphere",
+    "2r": "relative_humidity_2m_above_ground",
+    "2sh": "specific_humidity_2m_above_ground",
+    "2t": "temperature_2m_above_ground",
+    "tcc": "total_cloud_cover_entire_atmosphere",
+    "tp": "total_precipitation_surface",
+    "10u": "u_component_of_wind_10m_above_ground",
+    "10v": "v_component_of_wind_10m_above_ground",
+}
+
+
+def open_dataset(
+    data_variable="tp",
+    creation_date=np.datetime64("2022-09-01"),
+    creation_time="00",
+    bbox=box,
+    time_chunks=24,
+):
+    """
+    从minio服务器读取gfs数据
+
+    Args:
+        data_variables (str): 数据变量，目前只支持tp，即降雨
+        creation_date (datetime64): 创建日期
+        creation_time (datetime64): 创建时间，即00\06\12\18之一
+        bbox (list|tuple): 四至范围
+        time_chunks (int): 分块数量
+
+    Returns:
+        dataset (Dataset): 读取结果
+    """
+
+    if data_variable in variables.keys():
+        short_name = data_variable
+        full_name = variables[data_variable]
+
+        with FS.open(f"{bucket_name}/geodata/gfs/gfs.json") as f:
+            cont = json.load(f)
+            start = np.datetime64(cont[short_name][0]["start"])
+            end = np.datetime64(cont[short_name][-1]["end"])
+
+        if creation_date < start or creation_date > end:
+            print("超出时间范围！")
+            return
+
+        if creation_time not in ["00", "06", "12", "18"]:
+            print("creation_time必须是00、06、12、18之一！")
+            return
+
+        year = str(creation_date.astype("object").year)
+        month = str(creation_date.astype("object").month).zfill(2)
+        day = str(creation_date.astype("object").day).zfill(2)
+
+        if creation_date < change:
+            json_url = f"s3://{bucket_name}/geodata/gfs/gfs_history/{year}/{month}/{day}/gfs{year}{month}{day}.t{creation_time}z.0p25.json"
+        else:
+            json_url = f"s3://{bucket_name}/geodata/gfs/{short_name}/{year}/{month}/{day}/gfs{year}{month}{day}.t{creation_time}z.0p25.json"
+
+        chunks = {"valid_time": time_chunks}
+        ds = xr.open_dataset(
+            "reference://",
+            engine="zarr",
+            chunks=chunks,
+            backend_kwargs={
+                "consolidated": False,
+                "storage_options": {
+                    "fo": FS.open(json_url),
+                    "remote_protocol": "s3",
+                    "remote_options": RO,
+                },
+            },
+        )
+
+        if creation_date < change:
+            ds = ds[full_name]
+
+        # ds = ds.filter_by_attrs(long_name=lambda v: v in data_variables)
+        ds = ds.rename({"longitude": "lon", "latitude": "lat"})
+        # ds = ds.transpose('time','valid_time','lon','lat')
+
+        bbox = regen_box(bbox, 0.25, 0)
+
+        if bbox[0] < box[0]:
+            left = box[0]
+        else:
+            left = bbox[0]
+
+        if bbox[1] < box[1]:
+            bottom = box[1]
+        else:
+            bottom = bbox[1]
+
+        if bbox[2] > box[2]:
+            right = box[2]
+        else:
+            right = bbox[2]
+
+        if bbox[3] > box[3]:
+            top = box[3]
+        else:
+            top = bbox[3]
+
+        longitudes = slice(left - 0.00001, right + 0.00001)
+        latitudes = slice(bottom - 0.00001, top + 0.00001)
+
+        ds = ds.sortby("lat", ascending=True)
+        ds = ds.sel(lon=longitudes, lat=latitudes)
+
+        return ds
+
+    else:
+        print("变量名不存在！")
+
+
+import geopandas as gpd
+
+
+def from_shp(
+    data_variable="tp",
+    creation_date=np.datetime64("2022-09-01"),
+    creation_time="00",
+    shp=None,
+    time_chunks=24,
+):
+    """
+    通过已有的矢量数据范围从minio服务器读取gfs数据
+
+    Args:
+        data_variables (str): 数据变量，目前只支持tp，即降雨
+        creation_date (datetime64): 创建日期
+        creation_time (datetime64): 创建时间，即00\06\12\18之一
+        shp (str): 矢量数据路径
+        time_chunks (int): 分块数量
+
+    Returns:
+        dataset (Dataset): 读取结果
+    """
+
+    gdf = gpd.GeoDataFrame.from_file(shp)
+    b = gdf.bounds
+    bbox = regen_box(
+        (b.loc[0]["minx"], b.loc[0]["miny"], b.loc[0]["maxx"], b.loc[0]["maxy"]), 0.1, 0
+    )
+
+    return open_dataset(data_variable, creation_date, creation_time, bbox, time_chunks)
+
+
+def from_aoi(
+    data_variable="tp",
+    creation_date=np.datetime64("2022-09-01"),
+    creation_time="00",
+    aoi: gpd.GeoDataFrame = None,
+    time_chunks=24,
+):
+    """
+    通过已有的GeoPandas.GeoDataFrame对象从minio服务器读取gfs数据
+
+    Args:
+        data_variables (str): 数据变量，目前只支持tp，即降雨
+        creation_date (datetime64): 创建日期
+        creation_time (datetime64): 创建时间，即00\06\12\18之一
+        aoi (GeoDataFrame): 已有的GeoPandas.GeoDataFrame对象
+        time_chunks (int): 分块数量
+
+    Returns:
+        dataset (Dataset): 读取结果
+    """
+    b = aoi.bounds
+    bbox = regen_box(
+        (b.loc[0]["minx"], b.loc[0]["miny"], b.loc[0]["maxx"], b.loc[0]["maxy"]), 0.1, 0
+    )
+
+    return open_dataset(data_variable, creation_date, creation_time, bbox, time_chunks)
```

### Comparing `hydrodatasource-0.0.1/hydrodatasource/reader/grdc.py` & `hydrodatasource-0.0.2/hydrodatasource/reader/grdc.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-"""
-Author: Wenyu Ouyang
-Date: 2023-01-02 22:23:24
-LastEditTime: 2024-03-28 08:34:57
-LastEditors: Wenyu Ouyang
-Description: read the Global Runoff Data Centre (GRDC) daily data
-FilePath: \hydrodata\hydrodatasource\reader\grdc.py
-Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
-"""
-# Global Runoff Data Centre module from ewatercycle: https://github.com/eWaterCycle/ewatercycle/blob/main/src/ewatercycle/observation/grdc.py
-import datetime
-import os
-import pandas as pd
-import xarray as xr
-
-from hydrodatasource.downloader.hydrostation import catalogue_grdc
-from hydrodatasource.processor.grdc import read_grdc_daily_data
-
-
-def dailygrdc2netcdf(start_date, end_date, data_dir=None, station_ids=None):
-    """
-    Parameters
-    ----------
-    start_date : _type_
-        a startDate provided in YYYY-MM-DD
-    end_date : _type_
-        a endDate provided in YYYY-MM-DD
-    """
-    nc_file = os.path.join(data_dir, "grdc_daily_data.nc")
-    if os.path.exists(nc_file):
-        return
-
-    catalogue = catalogue_grdc(data_dir)
-    # Create empty lists to store data and metadata
-    data_list = []
-    meta_list = []
-
-    if station_ids is None:
-        # Filter the catalogue based on the provided station IDs
-        filenames = os.listdir(data_dir)
-        # Extract station IDs from filenames that match the pattern
-        station_ids = [
-            int(fname.split("_")[0])
-            for fname in filenames
-            if fname.endswith("_Q_Day.Cmd.txt")
-        ]
-    catalogue = catalogue[catalogue["grdc_no"].isin(station_ids)]
-
-    # Loop over each station in the catalogue
-    for station_id in catalogue["grdc_no"]:
-        try:
-            st = datetime.datetime.strptime(start_date, "%Y-%m-%d").strftime(
-                "%Y-%m-%dT%H:%M:%SZ"
-            )
-            et = datetime.datetime.strptime(end_date, "%Y-%m-%d").strftime(
-                "%Y-%m-%dT%H:%M:%SZ"
-            )
-            df, meta = read_grdc_daily_data(str(station_id), st, et, data_dir)
-        except Exception as e:
-            print(f"Error reading data for station {station_id}: {e}")
-            # Create an empty DataFrame with the same structure
-            df = pd.DataFrame(
-                columns=["streamflow"],
-                index=pd.date_range(start=start_date, end=end_date),
-            )
-            df["streamflow"] = float("nan")
-            meta = {
-                "grdc_file_name": "",
-                "id_from_grdc": station_id,
-                "river_name": "",
-                "station_name": "",
-                "country_code": "",
-                "grdc_latitude_in_arc_degree": float("nan"),
-                "grdc_longitude_in_arc_degree": float("nan"),
-                "grdc_catchment_area_in_km2": float("nan"),
-                "altitude_masl": float("nan"),
-                "dataSetContent": "",
-                "units": "m³/s",
-                "time_series": "",
-                "no_of_years": 0,
-                "last_update": "",
-                "nrMeasurements": "NA",
-                "UserStartTime": start_date,
-                "UserEndTime": end_date,
-                "nrMissingData": 0,
-            }
-
-        # Convert the DataFrame to an xarray DataArray and append to the list
-        # da = xr.DataArray(
-        #     df["streamflow"].values,
-        #     coords=[df.index, [station_id]],
-        #     dims=["time", "station"],
-        # )
-        coords_dict = {"time": df.index, "station": [station_id]}
-        da = xr.DataArray(
-            data=df["streamflow"].values.reshape(-1, 1),
-            coords=coords_dict,
-            dims=["time", "station"],
-            name="streamflow",
-            attrs={"units": meta.get("units", "unknown")},
-        )
-        data_list.append(da)
-
-        # Append metadata
-        meta_list.append(meta)
-
-    # Concatenate all DataArrays along the 'station' dimension
-    ds = xr.concat(data_list, dim="station")
-
-    # Assign attributes
-    ds.attrs["description"] = "Daily river discharge"
-    ds.station.attrs["description"] = "GRDC station number"
-
-    # Write the xarray Dataset to a NetCDF file
-    ds.to_netcdf(nc_file)
-
-    print("NetCDF file created successfully!")
-
-
-class GRDCDataHandler:
-    def handle(self, configuration):
-        aoi_param = configuration["aoi"].aoi_param
-        start_time = aoi_param["start_time"]
-        end_time = aoi_param["end_time"]
-        station_id = aoi_param["station_id"]
-        # Based on configuration, read and handle GRDC data specifically
-        nc_file = configuration["path"]
-        if not os.path.isfile(nc_file):
-            dailygrdc2netcdf(start_time, end_time, data_dir=os.path.dirname(nc_file))
-        ds = xr.open_dataset(nc_file)
-        # choose data for given basin
-        return ds.sel(station=int(station_id)).sel(time=slice(start_time, end_time))
+"""
+Author: Wenyu Ouyang
+Date: 2023-01-02 22:23:24
+LastEditTime: 2024-03-28 08:34:57
+LastEditors: Wenyu Ouyang
+Description: read the Global Runoff Data Centre (GRDC) daily data
+FilePath: \hydrodata\hydrodatasource\reader\grdc.py
+Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
+"""
+# Global Runoff Data Centre module from ewatercycle: https://github.com/eWaterCycle/ewatercycle/blob/main/src/ewatercycle/observation/grdc.py
+import datetime
+import os
+import pandas as pd
+import xarray as xr
+
+from hydrodatasource.downloader.hydrostation import catalogue_grdc
+from hydrodatasource.processor.grdc import read_grdc_daily_data
+
+
+def dailygrdc2netcdf(start_date, end_date, data_dir=None, station_ids=None):
+    """
+    Parameters
+    ----------
+    start_date : _type_
+        a startDate provided in YYYY-MM-DD
+    end_date : _type_
+        a endDate provided in YYYY-MM-DD
+    """
+    nc_file = os.path.join(data_dir, "grdc_daily_data.nc")
+    if os.path.exists(nc_file):
+        return
+
+    catalogue = catalogue_grdc(data_dir)
+    # Create empty lists to store data and metadata
+    data_list = []
+    meta_list = []
+
+    if station_ids is None:
+        # Filter the catalogue based on the provided station IDs
+        filenames = os.listdir(data_dir)
+        # Extract station IDs from filenames that match the pattern
+        station_ids = [
+            int(fname.split("_")[0])
+            for fname in filenames
+            if fname.endswith("_Q_Day.Cmd.txt")
+        ]
+    catalogue = catalogue[catalogue["grdc_no"].isin(station_ids)]
+
+    # Loop over each station in the catalogue
+    for station_id in catalogue["grdc_no"]:
+        try:
+            st = datetime.datetime.strptime(start_date, "%Y-%m-%d").strftime(
+                "%Y-%m-%dT%H:%M:%SZ"
+            )
+            et = datetime.datetime.strptime(end_date, "%Y-%m-%d").strftime(
+                "%Y-%m-%dT%H:%M:%SZ"
+            )
+            df, meta = read_grdc_daily_data(str(station_id), st, et, data_dir)
+        except Exception as e:
+            print(f"Error reading data for station {station_id}: {e}")
+            # Create an empty DataFrame with the same structure
+            df = pd.DataFrame(
+                columns=["streamflow"],
+                index=pd.date_range(start=start_date, end=end_date),
+            )
+            df["streamflow"] = float("nan")
+            meta = {
+                "grdc_file_name": "",
+                "id_from_grdc": station_id,
+                "river_name": "",
+                "station_name": "",
+                "country_code": "",
+                "grdc_latitude_in_arc_degree": float("nan"),
+                "grdc_longitude_in_arc_degree": float("nan"),
+                "grdc_catchment_area_in_km2": float("nan"),
+                "altitude_masl": float("nan"),
+                "dataSetContent": "",
+                "units": "m³/s",
+                "time_series": "",
+                "no_of_years": 0,
+                "last_update": "",
+                "nrMeasurements": "NA",
+                "UserStartTime": start_date,
+                "UserEndTime": end_date,
+                "nrMissingData": 0,
+            }
+
+        # Convert the DataFrame to an xarray DataArray and append to the list
+        # da = xr.DataArray(
+        #     df["streamflow"].values,
+        #     coords=[df.index, [station_id]],
+        #     dims=["time", "station"],
+        # )
+        coords_dict = {"time": df.index, "station": [station_id]}
+        da = xr.DataArray(
+            data=df["streamflow"].values.reshape(-1, 1),
+            coords=coords_dict,
+            dims=["time", "station"],
+            name="streamflow",
+            attrs={"units": meta.get("units", "unknown")},
+        )
+        data_list.append(da)
+
+        # Append metadata
+        meta_list.append(meta)
+
+    # Concatenate all DataArrays along the 'station' dimension
+    ds = xr.concat(data_list, dim="station")
+
+    # Assign attributes
+    ds.attrs["description"] = "Daily river discharge"
+    ds.station.attrs["description"] = "GRDC station number"
+
+    # Write the xarray Dataset to a NetCDF file
+    ds.to_netcdf(nc_file)
+
+    print("NetCDF file created successfully!")
+
+
+class GRDCDataHandler:
+    def handle(self, configuration):
+        aoi_param = configuration["aoi"].aoi_param
+        start_time = aoi_param["start_time"]
+        end_time = aoi_param["end_time"]
+        station_id = aoi_param["station_id"]
+        # Based on configuration, read and handle GRDC data specifically
+        nc_file = configuration["path"]
+        if not os.path.isfile(nc_file):
+            dailygrdc2netcdf(start_time, end_time, data_dir=os.path.dirname(nc_file))
+        ds = xr.open_dataset(nc_file)
+        # choose data for given basin
+        return ds.sel(station=int(station_id)).sel(time=slice(start_time, end_time))
```

### Comparing `hydrodatasource-0.0.1/hydrodatasource/reader/minio.py` & `hydrodatasource-0.0.2/hydrodatasource/reader/minio.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,1100 +1,1100 @@
-"""
-Author: Jianfeng Zhu
-Date: 2023-10-22 16:47:36
-LastEditTime: 2024-03-28 08:34:13
-LastEditors: Wenyu Ouyang
-Description: Reader class for grid data in minio
-FilePath: \hydrodata\hydrodatasource\reader\minio.py
-Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
-"""
-
-import os
-import numpy as np
-import xarray as xr
-from datetime import datetime
-import calendar
-import dask
-import json
-import geopandas as gpd
-
-from ..configs.config import FS, MINIO_PARAM, RO
-from ..utils.utils import regen_box, creatspinc
-from hydrodatasource.downloader.minio import ERA5LCatalog, GFSCatalog, GPMCatalog
-
-dask.config.set({"array.slicing.split_large_chunks": False})
-
-
-class ERA5LReader:
-    """
-    用于从minio中读取era5-land数据
-
-    Methods:
-        open_dataset(data_variables, start_time, end_time, dataset, bbox): 从minio中读取era5-land数据
-        from_shp(data_variables, start_time, end_time, dataset, shp): 通过已有的矢量数据范围从minio服务器读取era5-land数据
-        from_aoi(data_variables, start_time, end_time, dataset, aoi): 用过已有的GeoPandas.GeoDataFrame对象从minio服务器读取era5-land数据
-        to_netcdf(data_variables, start_time, end_time, dataset, shp, resolution, save_file): 读取数据并保存为本地nc文件
-    """
-
-    def __init__(self):
-        self._variables = [
-            "10 metre U wind component",
-            "10 metre V wind component",
-            "2 metre dewpoint temperature",
-            "2 metre temperature",
-            "Evaporation",
-            "Evaporation from bare soil",
-            "Evaporation from open water surfaces excluding oceans",
-            "Evaporation from the top of canopy",
-            "Evaporation from vegetation transpiration",
-            "Forecast albedo",
-            "Lake bottom temperature",
-            "Lake ice total depth",
-            "Lake ice surface temperature",
-            "Lake mix-layer depth",
-            "Lake mix-layer temperature",
-            "Lake shape factor",
-            "Lake total layer temperature",
-            "Leaf area index, high vegetation",
-            "Leaf area index, low vegetation",
-            "Potential evaporation",
-            "Runoff",
-            "Skin reservoir content",
-            "Skin temperature",
-            "Snow albedo",
-            "Snow cover",
-            "Snow density",
-            "Snow depth",
-            "Snow depth water equivalent",
-            "Snow evaporation",
-            "Snowfall",
-            "Snowmelt",
-            "Soil temperature level 1",
-            "Soil temperature level 2",
-            "Soil temperature level 3",
-            "Soil temperature level 4",
-            "Sub-surface runoff",
-            "Surface latent heat flux",
-            "Surface net solar radiation",
-            "Surface net thermal radiation",
-            "Surface pressure",
-            "Surface runoff",
-            "Surface sensible heat flux",
-            "Surface solar radiation downwards",
-            "Surface thermal radiation downwards",
-            "Temperature of snow layer",
-            "Total precipitation",
-            "Volumetric soil water layer 1",
-            "Volumetric soil water layer 2",
-            "Volumetric soil water layer 3",
-            "Volumetric soil water layer 4",
-        ]
-
-        self._accumulated = [
-            "Evaporation",
-            "Evaporation from bare soil",
-            "Evaporation from open water surfaces excluding oceans",
-            "Evaporation from the top of canopy",
-            "Evaporation from vegetation transpiration",
-            "Potential evaporation",
-            "Runoff",
-            "Snow evaporation",
-            "Snowfall",
-            "Snowmelt",
-            "Sub-surface runoff",
-            "Surface latent heat flux",
-            "Surface net solar radiation",
-            "Surface net thermal radiation",
-            "Surface runoff",
-            "Surface sensible heat flux",
-            "Surface solar radiation downwards",
-            "Surface thermal radiation downwards",
-            "Total precipitation",
-        ]
-        self._bucket_name = "test"
-
-    def open_dataset(
-        self,
-        data_variables=["Total precipitation"],
-        start_time=None,
-        end_time=None,
-        dataset="wis",
-        bbox=None,
-        time_chunks=24,
-    ):
-        """
-        从minio服务器读取era5-land数据
-
-        Args:
-            data_variables (list): 数据变量列表
-            start_time (datetime64): 开始时间
-            end_time (datetime64): 结束时间
-            dataset (str): wis或camels
-            bbox (list|tuple): 四至范围
-            time_chunks (int): 分块数量
-
-        Returns:
-            dataset (Dataset): 读取结果
-        """
-
-        if end_time <= start_time:
-            raise Exception("结束时间不能早于开始时间")
-
-        if bbox[0] > bbox[2] or bbox[1] > bbox[3]:
-            raise Exception("四至范围格式错误")
-
-        if dataset != "wis" and dataset != "camels":
-            raise Exception("dataset参数错误")
-
-        if dataset == "wis":
-            self._dataset = "geodata"
-        elif dataset == "camels":
-            self._dataset = "camdata"
-
-        with FS.open(
-            os.path.join(self._bucket_name, f"{self._dataset}/era5_land/era5l.json")
-        ) as f:
-            cont = json.load(f)
-            self._starttime = np.datetime64(cont["start"])
-            self._endtime = np.datetime64(cont["end"])
-            self._bbox = cont["bbox"]
-
-        chunks = {"time": time_chunks}
-        ds = xr.open_dataset(
-            "reference://",
-            engine="zarr",
-            chunks=chunks,
-            backend_kwargs={
-                "consolidated": False,
-                "storage_options": {
-                    # no matter you run code in windows or linux, the bucket's format should be Linux style
-                    # so we don't use os.join.path
-                    "fo": f"s3://{self._bucket_name}/{self._dataset}/era5_land/era5_land_.json",
-                    "target_protocol": "s3",
-                    "target_options": RO,
-                    "remote_protocol": "s3",
-                    "remote_options": RO,
-                },
-            },
-        )
-
-        ds = ds.filter_by_attrs(long_name=lambda v: v in data_variables)
-        ds = ds.rename({"longitude": "lon", "latitude": "lat"})
-        ds = ds.transpose("time", "lon", "lat")
-
-        start_time = max(start_time, self._starttime)
-        end_time = min(end_time, self._endtime)
-        times = slice(start_time, end_time)
-        ds = ds.sel(time=times)
-
-        bbox = regen_box(bbox, 0.1, 0)
-
-        if bbox[0] < self._bbox[0]:
-            left = self._bbox[0]
-        else:
-            left = bbox[0]
-
-        if bbox[1] < self._bbox[1]:
-            bottom = self._bbox[1]
-        else:
-            bottom = bbox[1]
-
-        if bbox[2] > self._bbox[2]:
-            right = self._bbox[2]
-        else:
-            right = bbox[2]
-
-        if bbox[3] > self._bbox[3]:
-            top = self._bbox[3]
-        else:
-            top = bbox[3]
-
-        longitudes = slice(left - 0.00001, right + 0.00001)
-        latitudes = slice(bottom - 0.00001, top + 0.00001)
-
-        ds = ds.sortby("lat", ascending=True)
-        ds = ds.sel(lon=longitudes, lat=latitudes)
-
-        return ds
-
-    def from_shp(
-        self,
-        data_variables=["Total precipitation"],
-        start_time=None,
-        end_time=None,
-        dataset="wis",
-        shp=None,
-        time_chunks=24,
-    ):
-        """
-        通过已有的矢量数据范围从minio服务器读取era5-land数据
-
-        Args:
-            data_variables (list): 数据变量列表
-            start_time (datetime64): 开始时间
-            end_time (datetime64): 结束时间
-            dataset (str): wis或camels
-            shp (str): 矢量数据路径
-            time_chunks (int): 分块数量
-
-        Returns:
-            dataset (Dataset): 读取结果
-        """
-
-        gdf = gpd.GeoDataFrame.from_file(shp)
-        b = gdf.bounds
-        bbox = regen_box(
-            (b.loc[0]["minx"], b.loc[0]["miny"], b.loc[0]["maxx"], b.loc[0]["maxy"]),
-            0.1,
-            0,
-        )
-
-        ds = self.open_dataset(
-            data_variables, start_time, end_time, dataset, bbox, time_chunks
-        )
-
-        return self.open_dataset(
-            data_variables, start_time, end_time, dataset, bbox, time_chunks
-        )
-
-    def from_aoi(
-        self,
-        data_variables=["Total precipitation"],
-        start_time=None,
-        end_time=None,
-        dataset="wis",
-        aoi: gpd.GeoDataFrame = None,
-        time_chunks=24,
-    ):
-        """
-        用过已有的GeoPandas.GeoDataFrame对象从minio服务器读取era5-land数据
-
-        Args:
-            data_variables (list): 数据变量列表
-            start_time (datetime64): 开始时间
-            end_time (datetime64): 结束时间
-            dataset (str): wis或camels
-            aoi (GeoDataFrame): 已有的GeoPandas.GeoDataFrame对象
-            time_chunks (int): 分块数量
-
-        Returns:
-            dataset (Dataset): 读取结果
-        """
-
-        b = aoi.bounds
-        bbox = regen_box(
-            (b.loc[0]["minx"], b.loc[0]["miny"], b.loc[0]["maxx"], b.loc[0]["maxy"]),
-            0.1,
-            0,
-        )
-
-        ds = self.open_dataset(
-            data_variables, start_time, end_time, dataset, bbox, time_chunks
-        )
-
-        return ds
-
-    def to_netcdf(
-        self,
-        data_variables=["Total precipitation"],
-        start_time=None,
-        end_time=None,
-        dataset="wis",
-        shp=None,
-        resolution="hourly",
-        save_file="era5.nc",
-        time_chunks=24,
-    ):
-        """
-        读取数据并保存为本地nc文件
-
-        Args:
-            data_variables (list): 数据变量列表
-            start_time (datetime64): 开始时间
-            end_time (datetime64): 结束时间
-            dataset (str): wis或camels
-            shp (str): 已有的矢量数据路径
-            resolution (str): 输出的时间分辨率
-            save_file (str): 输出的文件路径
-            time_chunks (int): 分块数量
-
-        Returns:
-            dataset (Dataset): 读取结果
-        """
-
-        gdf = gpd.GeoDataFrame.from_file(shp)
-        b = gdf.bounds
-        bbox = regen_box(
-            (b.loc[0]["minx"], b.loc[0]["miny"], b.loc[0]["maxx"], b.loc[0]["maxy"]),
-            0.1,
-            0,
-        )
-
-        if resolution == "hourly":
-            ds = self.open_dataset(
-                data_variables, start_time, end_time, dataset, bbox, time_chunks
-            )
-
-            if ds.to_netcdf(save_file) == None:
-                print(save_file, "已生成")
-                ds = xr.open_dataset(save_file)
-                return ds
-
-        if resolution == "daily":
-            start_time = np.datetime64(f"{str(start_time)[:10]}T01:00:00.000000000")
-            end_time = np.datetime64(str(end_time)[:10]) + 1
-            end_time = np.datetime64(f"{str(end_time)}T00:00:00.000000000")
-
-            ds = self.open_dataset(
-                data_variables, start_time, end_time, dataset, bbox, time_chunks
-            )
-
-            days = ds["time"].size // 24
-
-            data_vars = {}
-            for k, v in ds.data_vars.items():
-                data_vars[k] = v.attrs
-
-            daily_arr = []
-
-            for var, attr in data_vars.items():
-                a = ds[var].to_numpy()
-
-                if attr["long_name"] in self._accumulated:
-                    xlist = [x for x in range(a.shape[0]) if x % 24 != 23]
-                    _a = np.delete(a, xlist, axis=0)
-
-                    daily_arr.append(_a)
-
-                else:
-                    r = np.split(a, days, axis=0)
-                    _r = [
-                        np.expand_dims(np.mean(r[i], axis=0), axis=0)
-                        for i in range(len(r))
-                    ]
-                    __r = np.concatenate(_r)
-
-                    daily_arr.append(__r)
-
-            lats = ds["lat"].to_numpy()
-            lons = ds["lon"].to_numpy()
-
-            start_time = np.datetime64(str(start_time)[:10])
-
-            creatspinc(daily_arr, data_vars, lats, lons, start_time, save_file, "daily")
-
-            new = xr.open_dataset(save_file)
-            print(save_file, "已生成")
-            return new
-
-        if resolution == "6-hourly":
-            start_time = np.datetime64(f"{str(start_time)[:10]}T01:00:00.000000000")
-            end_time = np.datetime64(str(end_time)[:10]) + 1
-            end_time = np.datetime64(f"{str(end_time)}T00:00:00.000000000")
-
-            ds = self.open_dataset(
-                data_variables, start_time, end_time, dataset, bbox, time_chunks
-            )
-
-            days = ds["time"].size // 6
-
-            data_vars = {}
-            for k, v in ds.data_vars.items():
-                data_vars[k] = v.attrs
-
-            daily_arr = []
-
-            for var, attr in data_vars.items():
-                a = ds[var].to_numpy()
-
-                if attr["long_name"] in self._accumulated:
-                    xlist = [x for x in range(a.shape[0]) if x % 6 != 5]
-                    _a = np.delete(a, xlist, axis=0)
-
-                    daily_arr.append(_a)
-
-                else:
-                    r = np.split(a, days, axis=0)
-                    _r = [
-                        np.expand_dims(np.mean(r[i], axis=0), axis=0)
-                        for i in range(len(r))
-                    ]
-                    __r = np.concatenate(_r)
-
-                    daily_arr.append(__r)
-
-            lats = ds["lat"].to_numpy()
-            lons = ds["lon"].to_numpy()
-
-            # start_time = np.datetime64(f'{str(start_time)[:10]}')
-            year = int(f"{str(start_time)[0:4]}")
-            month = int(f"{str(start_time)[5:7]}")
-            day = int(f"{str(start_time)[8:10]}")
-            dt = datetime(year, month, day, 0, 0, 0)
-
-            creatspinc(daily_arr, data_vars, lats, lons, dt, save_file, "6-hourly")
-
-            new = xr.open_dataset(save_file)
-            print(save_file, "已生成")
-            return new
-
-
-class GPMReader:
-    """
-    用于从minio中读取gpm数据
-
-    Methods:
-        open_dataset(start_time, end_time, dataset, bbox, time_resolution): 从minio中读取gpm数据
-        from_shp(start_time, end_time, dataset, shp, time_resolution): 通过已有的矢量数据范围从minio服务器读取gpm数据
-        from_aoi(start_time, end_time, dataset, aoi, time_resolution): 用过已有的GeoPandas.GeoDataFrame对象从minio服务器读取gpm数据
-    """
-
-    def __init__(self):
-        self._bucket_name = "test"
-
-    def _get_dataset(self, scale, start_time, end_time, bbox, time_chunks):
-        year = str(start_time)[:4]
-        month = str(start_time)[5:7].zfill(2)
-        day = str(self._endtime)[8:10].zfill(2)
-
-        if scale == "Y":
-            minio_path = f"s3://{self._bucket_name}/{self._dataset}/gpm{self._time_resolution}/{year}/gpm{year}_inc.json"
-
-        elif scale == "M":
-            minio_path = f"s3://{self._bucket_name}/{self._dataset}/gpm{self._time_resolution}/{year}/{month}/gpm{year}{month}_inc.json"
-
-        chunks = {"time": time_chunks}
-        ds = xr.open_dataset(
-            "reference://",
-            engine="zarr",
-            chunks=chunks,
-            backend_kwargs={
-                "consolidated": False,
-                "storage_options": {
-                    "fo": minio_path,
-                    "target_protocol": "s3",
-                    "target_options": RO,
-                    "remote_protocol": "s3",
-                    "remote_options": RO,
-                },
-            },
-        )
-
-        # if self._time_resolution == '1d':
-        #     ds = cf2datetime(ds)
-
-        ds = ds["precipitationCal"]
-        # ds.to_dataframe().filter(['precipitationCal','precipitationUncal']).to_xarray()
-
-        # ds = ds.rename({"longitude": "lon", "latitude": "lat"})
-        ds = ds.transpose("time", "lon", "lat")
-
-        times = slice(start_time, end_time)
-        ds = ds.sel(time=times)
-
-        left = bbox[0]
-        right = bbox[2]
-        bottom = bbox[1]
-        top = bbox[3]
-
-        longitudes = slice(left - 0.00001, right + 0.00001)
-        latitudes = slice(bottom - 0.00001, top + 0.00001)
-
-        ds = ds.sortby("lat", ascending=True)
-        ds = ds.sel(lon=longitudes, lat=latitudes)
-
-        return ds
-
-    def open_dataset(
-        self,
-        start_time=np.datetime64("2023-01-01T00:00:00.000000000"),
-        end_time=np.datetime64("2023-01-02T00:00:00.000000000"),
-        dataset="wis",
-        bbox=(121, 39, 122, 40),
-        time_resolution="1d",
-        time_chunks=48,
-    ):
-        """
-        从minio服务器读取gpm数据
-
-        Args:
-            start_time (datetime64): 开始时间
-            end_time (datetime64): 结束时间
-            dataset (str): wis或camels
-            bbox (list|tuple): 四至范围
-            time_resolution (str): 1d或30m
-            time_chunks (int): 分块数量
-
-        Returns:
-            dataset (Dataset): 读取结果
-        """
-
-        if end_time <= start_time:
-            raise Exception("结束时间不能早于开始时间")
-
-        if bbox[0] > bbox[2] or bbox[1] > bbox[3]:
-            raise Exception("四至范围错误")
-
-        if dataset != "wis" and dataset != "camels":
-            raise Exception("dataset参数错误")
-
-        if time_resolution != "1d" and time_resolution != "30m":
-            raise Exception("time_resolution参数错误")
-
-        # dataset_name = get_dataset_name()
-        if dataset == "wis":
-            self._dataset = "geodata"
-        elif dataset == "camels":
-            self._dataset = "camdata"
-
-        if time_resolution == "1d":
-            self._time_resolution = "1d"
-        elif time_resolution == "30m":
-            self._time_resolution = ""
-
-        with FS.open(
-            os.path.join(
-                self._bucket_name,
-                f"{self._dataset}/gpm{self._time_resolution}/gpm{self._time_resolution}.json",
-            )
-        ) as f:
-            cont = json.load(f)
-            self._starttime = np.datetime64(cont["start"])
-            self._endtime = np.datetime64(cont["end"])
-            self._bbox = cont["bbox"]
-
-        if start_time < self._starttime:
-            start_time = self._starttime
-
-        if end_time > self._endtime:
-            end_time = self._endtime
-
-        bbox = regen_box(bbox, 0.1, 0.05)
-
-        if bbox[0] < self._bbox[0]:
-            bbox[0] = self._bbox[0]
-        if bbox[1] < self._bbox[1]:
-            bbox[1] = self._bbox[1]
-        if bbox[2] > self._bbox[2]:
-            bbox[2] = self._bbox[2]
-        if bbox[3] > self._bbox[3]:
-            bbox[3] = self._bbox[3]
-
-        year_start = int(str(start_time)[:4])
-        year_end = int(str(end_time)[:4])
-        end_year = int(str(self._endtime)[:4])
-
-        if year_end < end_year:
-            if year_start == year_end:
-                ds = self._get_dataset(
-                    scale="Y",
-                    start_time=start_time,
-                    end_time=end_time,
-                    bbox=bbox,
-                    time_chunks=time_chunks,
-                )
-                return ds
-
-            elif year_start < year_end:
-                dss = []
-                years = range(year_start, year_end + 1)
-                for year in years:
-                    if year == year_start:
-                        dss.append(
-                            self._get_dataset(
-                                scale="Y",
-                                start_time=start_time,
-                                end_time=np.datetime64(
-                                    f"{year}-12-31T23:30:00.000000000"
-                                ),
-                                bbox=bbox,
-                                time_chunks=time_chunks,
-                            )
-                        )
-
-                    elif year == year_end:
-                        dss.append(
-                            self._get_dataset(
-                                scale="Y",
-                                start_time=np.datetime64(
-                                    f"{year}-01-01T00:00:00.000000000"
-                                ),
-                                end_time=end_time,
-                                bbox=bbox,
-                                time_chunks=time_chunks,
-                            )
-                        )
-
-                    else:
-                        dss.append(
-                            self._get_dataset(
-                                scale="Y",
-                                start_time=np.datetime64(
-                                    f"{year}-01-01T00:00:00.000000000"
-                                ),
-                                end_time=np.datetime64(
-                                    f"{year}-12-31T23:30:00.000000000"
-                                ),
-                                bbox=bbox,
-                                time_chunks=time_chunks,
-                            )
-                        )
-                return xr.merge(dss)
-
-        else:
-            month_end = int(str(end_time)[5:7])
-            end_month = int(str(self._endtime)[5:7])
-
-            if year_start == year_end:
-                month_start = int(str(start_time)[5:7])
-                if month_start == month_end:
-                    return self._get_dataset(
-                        scale="M",
-                        start_time=start_time,
-                        end_time=end_time,
-                        bbox=bbox,
-                        time_chunks=time_chunks,
-                    )
-                dss = []
-                for m in range(month_start, month_end + 1):
-                    if m == month_start:
-                        d = calendar.monthrange(year_start, m)[1]
-                        dss.append(
-                            self._get_dataset(
-                                scale="M",
-                                start_time=start_time,
-                                end_time=np.datetime64(
-                                    f"{year_start}-{str(m).zfill(2)}-{str(d).zfill(2)}T23:30:00.000000000"
-                                ),
-                                bbox=bbox,
-                                time_chunks=time_chunks,
-                            )
-                        )
-                    elif m == month_end:
-                        dss.append(
-                            self._get_dataset(
-                                scale="M",
-                                start_time=np.datetime64(
-                                    f"{year_start}-{str(m).zfill(2)}-01T00:00:00.000000000"
-                                ),
-                                end_time=end_time,
-                                bbox=bbox,
-                                time_chunks=time_chunks,
-                            )
-                        )
-                    else:
-                        d = calendar.monthrange(year_start, m)[1]
-                        dss.append(
-                            self._get_dataset(
-                                scale="M",
-                                start_time=np.datetime64(
-                                    f"{year_start}-{str(m).zfill(2)}-01T00:00:00.000000000"
-                                ),
-                                end_time=np.datetime64(
-                                    f"{year_start}-{str(m).zfill(2)}-{str(d).zfill(2)}T23:30:00.000000000"
-                                ),
-                                bbox=bbox,
-                                time_chunks=time_chunks,
-                            )
-                        )
-
-            else:
-                dss = []
-
-                for y in range(year_start, year_end + 1):
-                    if y == year_start:
-                        dss.append(
-                            self._get_dataset(
-                                scale="Y",
-                                start_time=start_time,
-                                end_time=np.datetime64(f"{y}-12-31T23:30:00.000000000"),
-                                bbox=bbox,
-                                time_chunks=time_chunks,
-                            )
-                        )
-
-                    elif y == year_end:
-                        for m in range(1, month_end + 1):
-                            if m == month_end:
-                                dss.append(
-                                    self._get_dataset(
-                                        scale="M",
-                                        start_time=np.datetime64(
-                                            f"{str(y).zfill(4)}-{str(m).zfill(2)}-01T00:00:00.000000000"
-                                        ),
-                                        end_time=end_time,
-                                        bbox=bbox,
-                                        time_chunks=time_chunks,
-                                    )
-                                )
-                            else:
-                                d = calendar.monthrange(y, m)[1]
-                                dss.append(
-                                    self._get_dataset(
-                                        scale="M",
-                                        start_time=np.datetime64(
-                                            f"{str(y).zfill(4)}-{str(m).zfill(2)}-01T00:00:00.000000000"
-                                        ),
-                                        end_time=np.datetime64(
-                                            f"{str(y).zfill(4)}-{str(m).zfill(2)}-{str(d).zfill(2)}T23:30:00.000000000"
-                                        ),
-                                        bbox=bbox,
-                                        time_chunks=time_chunks,
-                                    )
-                                )
-
-                    else:
-                        dss.append(
-                            self._get_dataset(
-                                scale="Y",
-                                start_time=np.datetime64(
-                                    f"{y}-01-01T00:00:00.000000000"
-                                ),
-                                end_time=np.datetime64(f"{y}-12-31T23:30:00.000000000"),
-                                bbox=bbox,
-                                time_chunks=time_chunks,
-                            )
-                        )
-
-            return xr.merge(dss)
-
-    def from_shp(
-        self,
-        start_time=np.datetime64("2023-01-01T00:00:00.000000000"),
-        end_time=np.datetime64("2023-01-02T00:00:00.000000000"),
-        dataset="wis",
-        shp=None,
-        time_resolution="1d",
-        time_chunks=48,
-    ):
-        """
-        通过已有的矢量数据范围从minio服务器读取gpm数据
-
-        Args:
-            start_time (datetime64): 开始时间
-            end_time (datetime64): 结束时间
-            dataset (str): wis或camels
-            shp (str): 矢量数据路径
-            time_resolution (str): 1d或30m
-            time_chunks (int): 分块数量
-
-        Returns:
-            dataset (Dataset): 读取结果
-        """
-
-        gdf = gpd.GeoDataFrame.from_file(shp)
-        b = gdf.bounds
-        bbox = regen_box(
-            (b.loc[0]["minx"], b.loc[0]["miny"], b.loc[0]["maxx"], b.loc[0]["maxy"]),
-            0.1,
-            0.05,
-        )
-
-        ds = self.open_dataset(
-            start_time, end_time, dataset, bbox, time_resolution, time_chunks
-        )
-        return ds
-
-    def from_aoi(
-        self,
-        start_time=np.datetime64("2023-01-01T00:00:00.000000000"),
-        end_time=np.datetime64("2023-01-02T00:00:00.000000000"),
-        dataset="wis",
-        aoi: gpd.GeoDataFrame = None,
-        time_resolution="1d",
-        time_chunks=48,
-    ):
-        """
-        用过已有的GeoPandas.GeoDataFrame对象从minio服务器读取gpm数据
-
-        Args:
-            start_time (datetime64): 开始时间
-            end_time (datetime64): 结束时间
-            dataset (str): wis或camels
-            aoi (GeoDataFrame): 已有的GeoPandas.GeoDataFrame对象
-            time_resolution (str): 1d或30m
-            time_chunks (int): 分块数量
-
-        Returns:
-            dataset (Dataset): 读取结果
-        """
-
-        b = aoi.bounds
-        bbox = regen_box(
-            (b.loc[0]["minx"], b.loc[0]["miny"], b.loc[0]["maxx"], b.loc[0]["maxy"]),
-            0.1,
-            0.05,
-        )
-        ds = self.open_dataset(
-            start_time, end_time, dataset, bbox, time_resolution, time_chunks
-        )
-        return ds
-
-
-class GFSReader:
-    """
-    用于从minio中读取gpm数据
-
-    Attributes:
-        variables (dict): 变量名称及缩写
-
-    Methods:
-        open_dataset(data_variables, creation_date, creation_time, bbox): 从minio中读取gfs数据
-        from_shp(data_variables, creation_date, creation_time, shp): 通过已有的矢量数据范围从minio服务器读取gfs数据
-        from_aoi(data_variables, creation_date, creation_time, aoi): 用过已有的GeoPandas.GeoDataFrame对象从minio服务器读取gfs数据
-    """
-
-    def __init__(self):
-        self._variables = {
-            "dswrf": "downward_shortwave_radiation_flux",
-            "pwat": "precipitable_water_entire_atmosphere",
-            "2r": "relative_humidity_2m_above_ground",
-            "2sh": "specific_humidity_2m_above_ground",
-            "2t": "temperature_2m_above_ground",
-            "tcc": "total_cloud_cover_entire_atmosphere",
-            "tp": "total_precipitation_surface",
-            "10u": "u_component_of_wind_10m_above_ground",
-            "10v": "v_component_of_wind_10m_above_ground",
-        }
-        self._bucket_name = "test"
-        self._default = "tp"
-
-    @property
-    def variables(self):
-        return self._variables
-
-    @property
-    def default_variable(self):
-        return self._default
-
-    def set_default_variable(self, short_name):
-        if short_name in self._variables.keys():
-            self._default = short_name
-        else:
-            raise Exception("变量设置错误")
-
-    def open_dataset(
-        self,
-        creation_date=np.datetime64("2022-09-01"),
-        creation_time="00",
-        dataset="wis",
-        bbox=(115, 38, 136, 54),
-        time_chunks=24,
-    ):
-        """
-        从minio服务器读取gfs数据
-
-        Args:
-            creation_date (datetime64): 创建日期
-            creation_time (datetime64): 创建时间，即00\06\12\18之一
-            dataset (str): wis或camels
-            bbox (list|tuple): 四至范围
-            time_chunks (int): 分块数量
-
-        Returns:
-            dataset (Dataset): 读取结果
-        """
-
-        if bbox[0] > bbox[2] or bbox[1] > bbox[3]:
-            raise Exception("四至范围格式错误")
-
-        if dataset != "wis" and dataset != "camels":
-            raise Exception("dataset参数错误")
-
-        if dataset == "wis":
-            self._dataset = "geodata"
-        elif dataset == "camels":
-            self._dataset = "camdata"
-
-        with FS.open(os.path.join(self._bucket_name, f"{self._dataset}/gfs/gfs.json")) as f:
-            cont = json.load(f)
-            self._paras = cont
-
-        short_name = self._default
-        full_name = self._variables[short_name]
-
-        start = np.datetime64(self._paras[short_name][0]["start"])
-        end = np.datetime64(self._paras[short_name][-1]["end"])
-
-        if creation_date < start or creation_date > end:
-            print("超出时间范围！")
-            return
-
-        if creation_time not in ["00", "06", "12", "18"]:
-            print("creation_time必须是00、06、12、18之一！")
-            return
-
-        year = str(creation_date.astype("object").year)
-        month = str(creation_date.astype("object").month).zfill(2)
-        day = str(creation_date.astype("object").day).zfill(2)
-
-        change = np.datetime64("2022-09-01")
-        if creation_date < change:
-            json_url = f"s3://{self._bucket_name}/{self._dataset}/gfs/gfs_history/{year}/{month}/{day}/gfs{year}{month}{day}.t{creation_time}z.0p25.json"
-        else:
-            json_url = f"s3://{self._bucket_name}/{self._dataset}/gfs/{short_name}/{year}/{month}/{day}/gfs{year}{month}{day}.t{creation_time}z.0p25.json"
-
-        chunks = {"valid_time": time_chunks}
-        ds = xr.open_dataset(
-            "reference://",
-            engine="zarr",
-            chunks=chunks,
-            backend_kwargs={
-                "consolidated": False,
-                "storage_options": {
-                    "fo": json_url,
-                    "target_protocol": "s3",
-                    "target_options": RO,
-                    "remote_protocol": "s3",
-                    "remote_options": RO,
-                },
-            },
-        )
-
-        if creation_date < change:
-            ds = ds[full_name]
-            box = self._paras[short_name][0]["bbox"]
-        else:
-            box = self.paras[short_name][-1]["bbox"]
-
-        # ds = ds.filter_by_attrs(long_name=lambda v: v in data_variables)
-        ds = ds.rename({"longitude": "lon", "latitude": "lat"})
-        # ds = ds.transpose('time','valid_time','lon','lat')
-
-        bbox = regen_box(bbox, 0.25, 0)
-
-        if bbox[0] < box[0]:
-            left = box[0]
-        else:
-            left = bbox[0]
-
-        if bbox[1] < box[1]:
-            bottom = box[1]
-        else:
-            bottom = bbox[1]
-
-        if bbox[2] > box[2]:
-            right = box[2]
-        else:
-            right = bbox[2]
-
-        if bbox[3] > box[3]:
-            top = box[3]
-        else:
-            top = bbox[3]
-
-        longitudes = slice(left - 0.00001, right + 0.00001)
-        latitudes = slice(bottom - 0.00001, top + 0.00001)
-
-        ds = ds.sortby("lat", ascending=True)
-        ds = ds.sel(lon=longitudes, lat=latitudes)
-
-        return ds
-
-    def from_shp(
-        self,
-        creation_date=np.datetime64("2022-09-01"),
-        creation_time="00",
-        dataset="wis",
-        shp=None,
-        time_chunks=24,
-    ):
-        """
-        通过已有的矢量数据范围从minio服务器读取gfs数据
-
-        Args:
-            creation_date (datetime64): 创建日期
-            creation_time (datetime64): 创建时间，即00\06\12\18之一
-            dataset (str): wis或camels
-            shp (str): 矢量数据路径
-            time_chunks (int): 分块数量
-
-        Returns:
-            dataset (Dataset): 读取结果
-        """
-
-        gdf = gpd.GeoDataFrame.from_file(shp)
-        b = gdf.bounds
-        bbox = regen_box(
-            (b.loc[0]["minx"], b.loc[0]["miny"], b.loc[0]["maxx"], b.loc[0]["maxy"]),
-            0.1,
-            0,
-        )
-
-        ds = self.open_dataset(creation_date, creation_time, dataset, bbox, time_chunks)
-
-        return ds
-
-    def from_aoi(
-        self,
-        creation_date=np.datetime64("2022-09-01"),
-        creation_time="00",
-        dataset="wis",
-        aoi: gpd.GeoDataFrame = None,
-        time_chunks=24,
-    ):
-        """
-        通过已有的GeoPandas.GeoDataFrame对象从minio服务器读取gfs数据
-
-        Args:
-            creation_date (datetime64): 创建日期
-            creation_time (datetime64): 创建时间，即00\06\12\18之一
-            dataset (str): wis或camels
-            aoi (GeoDataFrame): 已有的GeoPandas.GeoDataFrame对象
-            time_chunks (int): 分块数量
-
-        Returns:
-            dataset (Dataset): 读取结果
-        """
-        b = aoi.bounds
-        bbox = regen_box(
-            (b.loc[0]["minx"], b.loc[0]["miny"], b.loc[0]["maxx"], b.loc[0]["maxy"]),
-            0.1,
-            0,
-        )
-
-        ds = self.open_dataset(creation_date, creation_time, dataset, bbox, time_chunks)
-
-        return ds
-
-
-class Era5L:
-    def __init__(self):
-        self._catalog = ERA5LCatalog()
-        self._reader = ERA5LReader()
-
-    @property
-    def catalog(self):
-        return self._catalog
-
-    @property
-    def reader(self):
-        return self._reader
-
-
-class GPM:
-    def __init__(self):
-        self._catalog = GPMCatalog()
-        self._reader = GPMReader()
-
-    @property
-    def catalog(self):
-        return self._catalog
-
-    @property
-    def reader(self):
-        return self._reader
-
-
-class GFS:
-    def __init__(self, variable="tp"):
-        self._catalog = GFSCatalog(variable)
-        self._reader = GFSReader()
-        self._reader.set_default_variable(self._catalog.variable)
-
-    @property
-    def catalog(self):
-        return self._catalog
-
-    @property
-    def reader(self):
-        return self._reader
+"""
+Author: Jianfeng Zhu
+Date: 2023-10-22 16:47:36
+LastEditTime: 2024-03-28 08:34:13
+LastEditors: Wenyu Ouyang
+Description: Reader class for grid data in minio
+FilePath: \hydrodata\hydrodatasource\reader\minio.py
+Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
+"""
+
+import os
+import numpy as np
+import xarray as xr
+from datetime import datetime
+import calendar
+import dask
+import json
+import geopandas as gpd
+
+from ..configs.config import FS, MINIO_PARAM, RO
+from ..utils.utils import regen_box, creatspinc
+from hydrodatasource.downloader.minio import ERA5LCatalog, GFSCatalog, GPMCatalog
+
+dask.config.set({"array.slicing.split_large_chunks": False})
+
+
+class ERA5LReader:
+    """
+    用于从minio中读取era5-land数据
+
+    Methods:
+        open_dataset(data_variables, start_time, end_time, dataset, bbox): 从minio中读取era5-land数据
+        from_shp(data_variables, start_time, end_time, dataset, shp): 通过已有的矢量数据范围从minio服务器读取era5-land数据
+        from_aoi(data_variables, start_time, end_time, dataset, aoi): 用过已有的GeoPandas.GeoDataFrame对象从minio服务器读取era5-land数据
+        to_netcdf(data_variables, start_time, end_time, dataset, shp, resolution, save_file): 读取数据并保存为本地nc文件
+    """
+
+    def __init__(self):
+        self._variables = [
+            "10 metre U wind component",
+            "10 metre V wind component",
+            "2 metre dewpoint temperature",
+            "2 metre temperature",
+            "Evaporation",
+            "Evaporation from bare soil",
+            "Evaporation from open water surfaces excluding oceans",
+            "Evaporation from the top of canopy",
+            "Evaporation from vegetation transpiration",
+            "Forecast albedo",
+            "Lake bottom temperature",
+            "Lake ice total depth",
+            "Lake ice surface temperature",
+            "Lake mix-layer depth",
+            "Lake mix-layer temperature",
+            "Lake shape factor",
+            "Lake total layer temperature",
+            "Leaf area index, high vegetation",
+            "Leaf area index, low vegetation",
+            "Potential evaporation",
+            "Runoff",
+            "Skin reservoir content",
+            "Skin temperature",
+            "Snow albedo",
+            "Snow cover",
+            "Snow density",
+            "Snow depth",
+            "Snow depth water equivalent",
+            "Snow evaporation",
+            "Snowfall",
+            "Snowmelt",
+            "Soil temperature level 1",
+            "Soil temperature level 2",
+            "Soil temperature level 3",
+            "Soil temperature level 4",
+            "Sub-surface runoff",
+            "Surface latent heat flux",
+            "Surface net solar radiation",
+            "Surface net thermal radiation",
+            "Surface pressure",
+            "Surface runoff",
+            "Surface sensible heat flux",
+            "Surface solar radiation downwards",
+            "Surface thermal radiation downwards",
+            "Temperature of snow layer",
+            "Total precipitation",
+            "Volumetric soil water layer 1",
+            "Volumetric soil water layer 2",
+            "Volumetric soil water layer 3",
+            "Volumetric soil water layer 4",
+        ]
+
+        self._accumulated = [
+            "Evaporation",
+            "Evaporation from bare soil",
+            "Evaporation from open water surfaces excluding oceans",
+            "Evaporation from the top of canopy",
+            "Evaporation from vegetation transpiration",
+            "Potential evaporation",
+            "Runoff",
+            "Snow evaporation",
+            "Snowfall",
+            "Snowmelt",
+            "Sub-surface runoff",
+            "Surface latent heat flux",
+            "Surface net solar radiation",
+            "Surface net thermal radiation",
+            "Surface runoff",
+            "Surface sensible heat flux",
+            "Surface solar radiation downwards",
+            "Surface thermal radiation downwards",
+            "Total precipitation",
+        ]
+        self._bucket_name = "test"
+
+    def open_dataset(
+        self,
+        data_variables=["Total precipitation"],
+        start_time=None,
+        end_time=None,
+        dataset="wis",
+        bbox=None,
+        time_chunks=24,
+    ):
+        """
+        从minio服务器读取era5-land数据
+
+        Args:
+            data_variables (list): 数据变量列表
+            start_time (datetime64): 开始时间
+            end_time (datetime64): 结束时间
+            dataset (str): wis或camels
+            bbox (list|tuple): 四至范围
+            time_chunks (int): 分块数量
+
+        Returns:
+            dataset (Dataset): 读取结果
+        """
+
+        if end_time <= start_time:
+            raise Exception("结束时间不能早于开始时间")
+
+        if bbox[0] > bbox[2] or bbox[1] > bbox[3]:
+            raise Exception("四至范围格式错误")
+
+        if dataset != "wis" and dataset != "camels":
+            raise Exception("dataset参数错误")
+
+        if dataset == "wis":
+            self._dataset = "geodata"
+        elif dataset == "camels":
+            self._dataset = "camdata"
+
+        with FS.open(
+            os.path.join(self._bucket_name, f"{self._dataset}/era5_land/era5l.json")
+        ) as f:
+            cont = json.load(f)
+            self._starttime = np.datetime64(cont["start"])
+            self._endtime = np.datetime64(cont["end"])
+            self._bbox = cont["bbox"]
+
+        chunks = {"time": time_chunks}
+        ds = xr.open_dataset(
+            "reference://",
+            engine="zarr",
+            chunks=chunks,
+            backend_kwargs={
+                "consolidated": False,
+                "storage_options": {
+                    # no matter you run code in windows or linux, the bucket's format should be Linux style
+                    # so we don't use os.join.path
+                    "fo": f"s3://{self._bucket_name}/{self._dataset}/era5_land/era5_land_.json",
+                    "target_protocol": "s3",
+                    "target_options": RO,
+                    "remote_protocol": "s3",
+                    "remote_options": RO,
+                },
+            },
+        )
+
+        ds = ds.filter_by_attrs(long_name=lambda v: v in data_variables)
+        ds = ds.rename({"longitude": "lon", "latitude": "lat"})
+        ds = ds.transpose("time", "lon", "lat")
+
+        start_time = max(start_time, self._starttime)
+        end_time = min(end_time, self._endtime)
+        times = slice(start_time, end_time)
+        ds = ds.sel(time=times)
+
+        bbox = regen_box(bbox, 0.1, 0)
+
+        if bbox[0] < self._bbox[0]:
+            left = self._bbox[0]
+        else:
+            left = bbox[0]
+
+        if bbox[1] < self._bbox[1]:
+            bottom = self._bbox[1]
+        else:
+            bottom = bbox[1]
+
+        if bbox[2] > self._bbox[2]:
+            right = self._bbox[2]
+        else:
+            right = bbox[2]
+
+        if bbox[3] > self._bbox[3]:
+            top = self._bbox[3]
+        else:
+            top = bbox[3]
+
+        longitudes = slice(left - 0.00001, right + 0.00001)
+        latitudes = slice(bottom - 0.00001, top + 0.00001)
+
+        ds = ds.sortby("lat", ascending=True)
+        ds = ds.sel(lon=longitudes, lat=latitudes)
+
+        return ds
+
+    def from_shp(
+        self,
+        data_variables=["Total precipitation"],
+        start_time=None,
+        end_time=None,
+        dataset="wis",
+        shp=None,
+        time_chunks=24,
+    ):
+        """
+        通过已有的矢量数据范围从minio服务器读取era5-land数据
+
+        Args:
+            data_variables (list): 数据变量列表
+            start_time (datetime64): 开始时间
+            end_time (datetime64): 结束时间
+            dataset (str): wis或camels
+            shp (str): 矢量数据路径
+            time_chunks (int): 分块数量
+
+        Returns:
+            dataset (Dataset): 读取结果
+        """
+
+        gdf = gpd.GeoDataFrame.from_file(shp)
+        b = gdf.bounds
+        bbox = regen_box(
+            (b.loc[0]["minx"], b.loc[0]["miny"], b.loc[0]["maxx"], b.loc[0]["maxy"]),
+            0.1,
+            0,
+        )
+
+        ds = self.open_dataset(
+            data_variables, start_time, end_time, dataset, bbox, time_chunks
+        )
+
+        return self.open_dataset(
+            data_variables, start_time, end_time, dataset, bbox, time_chunks
+        )
+
+    def from_aoi(
+        self,
+        data_variables=["Total precipitation"],
+        start_time=None,
+        end_time=None,
+        dataset="wis",
+        aoi: gpd.GeoDataFrame = None,
+        time_chunks=24,
+    ):
+        """
+        用过已有的GeoPandas.GeoDataFrame对象从minio服务器读取era5-land数据
+
+        Args:
+            data_variables (list): 数据变量列表
+            start_time (datetime64): 开始时间
+            end_time (datetime64): 结束时间
+            dataset (str): wis或camels
+            aoi (GeoDataFrame): 已有的GeoPandas.GeoDataFrame对象
+            time_chunks (int): 分块数量
+
+        Returns:
+            dataset (Dataset): 读取结果
+        """
+
+        b = aoi.bounds
+        bbox = regen_box(
+            (b.loc[0]["minx"], b.loc[0]["miny"], b.loc[0]["maxx"], b.loc[0]["maxy"]),
+            0.1,
+            0,
+        )
+
+        ds = self.open_dataset(
+            data_variables, start_time, end_time, dataset, bbox, time_chunks
+        )
+
+        return ds
+
+    def to_netcdf(
+        self,
+        data_variables=["Total precipitation"],
+        start_time=None,
+        end_time=None,
+        dataset="wis",
+        shp=None,
+        resolution="hourly",
+        save_file="era5.nc",
+        time_chunks=24,
+    ):
+        """
+        读取数据并保存为本地nc文件
+
+        Args:
+            data_variables (list): 数据变量列表
+            start_time (datetime64): 开始时间
+            end_time (datetime64): 结束时间
+            dataset (str): wis或camels
+            shp (str): 已有的矢量数据路径
+            resolution (str): 输出的时间分辨率
+            save_file (str): 输出的文件路径
+            time_chunks (int): 分块数量
+
+        Returns:
+            dataset (Dataset): 读取结果
+        """
+
+        gdf = gpd.GeoDataFrame.from_file(shp)
+        b = gdf.bounds
+        bbox = regen_box(
+            (b.loc[0]["minx"], b.loc[0]["miny"], b.loc[0]["maxx"], b.loc[0]["maxy"]),
+            0.1,
+            0,
+        )
+
+        if resolution == "hourly":
+            ds = self.open_dataset(
+                data_variables, start_time, end_time, dataset, bbox, time_chunks
+            )
+
+            if ds.to_netcdf(save_file) == None:
+                print(save_file, "已生成")
+                ds = xr.open_dataset(save_file)
+                return ds
+
+        if resolution == "daily":
+            start_time = np.datetime64(f"{str(start_time)[:10]}T01:00:00.000000000")
+            end_time = np.datetime64(str(end_time)[:10]) + 1
+            end_time = np.datetime64(f"{str(end_time)}T00:00:00.000000000")
+
+            ds = self.open_dataset(
+                data_variables, start_time, end_time, dataset, bbox, time_chunks
+            )
+
+            days = ds["time"].size // 24
+
+            data_vars = {}
+            for k, v in ds.data_vars.items():
+                data_vars[k] = v.attrs
+
+            daily_arr = []
+
+            for var, attr in data_vars.items():
+                a = ds[var].to_numpy()
+
+                if attr["long_name"] in self._accumulated:
+                    xlist = [x for x in range(a.shape[0]) if x % 24 != 23]
+                    _a = np.delete(a, xlist, axis=0)
+
+                    daily_arr.append(_a)
+
+                else:
+                    r = np.split(a, days, axis=0)
+                    _r = [
+                        np.expand_dims(np.mean(r[i], axis=0), axis=0)
+                        for i in range(len(r))
+                    ]
+                    __r = np.concatenate(_r)
+
+                    daily_arr.append(__r)
+
+            lats = ds["lat"].to_numpy()
+            lons = ds["lon"].to_numpy()
+
+            start_time = np.datetime64(str(start_time)[:10])
+
+            creatspinc(daily_arr, data_vars, lats, lons, start_time, save_file, "daily")
+
+            new = xr.open_dataset(save_file)
+            print(save_file, "已生成")
+            return new
+
+        if resolution == "6-hourly":
+            start_time = np.datetime64(f"{str(start_time)[:10]}T01:00:00.000000000")
+            end_time = np.datetime64(str(end_time)[:10]) + 1
+            end_time = np.datetime64(f"{str(end_time)}T00:00:00.000000000")
+
+            ds = self.open_dataset(
+                data_variables, start_time, end_time, dataset, bbox, time_chunks
+            )
+
+            days = ds["time"].size // 6
+
+            data_vars = {}
+            for k, v in ds.data_vars.items():
+                data_vars[k] = v.attrs
+
+            daily_arr = []
+
+            for var, attr in data_vars.items():
+                a = ds[var].to_numpy()
+
+                if attr["long_name"] in self._accumulated:
+                    xlist = [x for x in range(a.shape[0]) if x % 6 != 5]
+                    _a = np.delete(a, xlist, axis=0)
+
+                    daily_arr.append(_a)
+
+                else:
+                    r = np.split(a, days, axis=0)
+                    _r = [
+                        np.expand_dims(np.mean(r[i], axis=0), axis=0)
+                        for i in range(len(r))
+                    ]
+                    __r = np.concatenate(_r)
+
+                    daily_arr.append(__r)
+
+            lats = ds["lat"].to_numpy()
+            lons = ds["lon"].to_numpy()
+
+            # start_time = np.datetime64(f'{str(start_time)[:10]}')
+            year = int(f"{str(start_time)[0:4]}")
+            month = int(f"{str(start_time)[5:7]}")
+            day = int(f"{str(start_time)[8:10]}")
+            dt = datetime(year, month, day, 0, 0, 0)
+
+            creatspinc(daily_arr, data_vars, lats, lons, dt, save_file, "6-hourly")
+
+            new = xr.open_dataset(save_file)
+            print(save_file, "已生成")
+            return new
+
+
+class GPMReader:
+    """
+    用于从minio中读取gpm数据
+
+    Methods:
+        open_dataset(start_time, end_time, dataset, bbox, time_resolution): 从minio中读取gpm数据
+        from_shp(start_time, end_time, dataset, shp, time_resolution): 通过已有的矢量数据范围从minio服务器读取gpm数据
+        from_aoi(start_time, end_time, dataset, aoi, time_resolution): 用过已有的GeoPandas.GeoDataFrame对象从minio服务器读取gpm数据
+    """
+
+    def __init__(self):
+        self._bucket_name = "test"
+
+    def _get_dataset(self, scale, start_time, end_time, bbox, time_chunks):
+        year = str(start_time)[:4]
+        month = str(start_time)[5:7].zfill(2)
+        day = str(self._endtime)[8:10].zfill(2)
+
+        if scale == "Y":
+            minio_path = f"s3://{self._bucket_name}/{self._dataset}/gpm{self._time_resolution}/{year}/gpm{year}_inc.json"
+
+        elif scale == "M":
+            minio_path = f"s3://{self._bucket_name}/{self._dataset}/gpm{self._time_resolution}/{year}/{month}/gpm{year}{month}_inc.json"
+
+        chunks = {"time": time_chunks}
+        ds = xr.open_dataset(
+            "reference://",
+            engine="zarr",
+            chunks=chunks,
+            backend_kwargs={
+                "consolidated": False,
+                "storage_options": {
+                    "fo": minio_path,
+                    "target_protocol": "s3",
+                    "target_options": RO,
+                    "remote_protocol": "s3",
+                    "remote_options": RO,
+                },
+            },
+        )
+
+        # if self._time_resolution == '1d':
+        #     ds = cf2datetime(ds)
+
+        ds = ds["precipitationCal"]
+        # ds.to_dataframe().filter(['precipitationCal','precipitationUncal']).to_xarray()
+
+        # ds = ds.rename({"longitude": "lon", "latitude": "lat"})
+        ds = ds.transpose("time", "lon", "lat")
+
+        times = slice(start_time, end_time)
+        ds = ds.sel(time=times)
+
+        left = bbox[0]
+        right = bbox[2]
+        bottom = bbox[1]
+        top = bbox[3]
+
+        longitudes = slice(left - 0.00001, right + 0.00001)
+        latitudes = slice(bottom - 0.00001, top + 0.00001)
+
+        ds = ds.sortby("lat", ascending=True)
+        ds = ds.sel(lon=longitudes, lat=latitudes)
+
+        return ds
+
+    def open_dataset(
+        self,
+        start_time=np.datetime64("2023-01-01T00:00:00.000000000"),
+        end_time=np.datetime64("2023-01-02T00:00:00.000000000"),
+        dataset="wis",
+        bbox=(121, 39, 122, 40),
+        time_resolution="1d",
+        time_chunks=48,
+    ):
+        """
+        从minio服务器读取gpm数据
+
+        Args:
+            start_time (datetime64): 开始时间
+            end_time (datetime64): 结束时间
+            dataset (str): wis或camels
+            bbox (list|tuple): 四至范围
+            time_resolution (str): 1d或30m
+            time_chunks (int): 分块数量
+
+        Returns:
+            dataset (Dataset): 读取结果
+        """
+
+        if end_time <= start_time:
+            raise Exception("结束时间不能早于开始时间")
+
+        if bbox[0] > bbox[2] or bbox[1] > bbox[3]:
+            raise Exception("四至范围错误")
+
+        if dataset != "wis" and dataset != "camels":
+            raise Exception("dataset参数错误")
+
+        if time_resolution != "1d" and time_resolution != "30m":
+            raise Exception("time_resolution参数错误")
+
+        # dataset_name = get_dataset_name()
+        if dataset == "wis":
+            self._dataset = "geodata"
+        elif dataset == "camels":
+            self._dataset = "camdata"
+
+        if time_resolution == "1d":
+            self._time_resolution = "1d"
+        elif time_resolution == "30m":
+            self._time_resolution = ""
+
+        with FS.open(
+            os.path.join(
+                self._bucket_name,
+                f"{self._dataset}/gpm{self._time_resolution}/gpm{self._time_resolution}.json",
+            )
+        ) as f:
+            cont = json.load(f)
+            self._starttime = np.datetime64(cont["start"])
+            self._endtime = np.datetime64(cont["end"])
+            self._bbox = cont["bbox"]
+
+        if start_time < self._starttime:
+            start_time = self._starttime
+
+        if end_time > self._endtime:
+            end_time = self._endtime
+
+        bbox = regen_box(bbox, 0.1, 0.05)
+
+        if bbox[0] < self._bbox[0]:
+            bbox[0] = self._bbox[0]
+        if bbox[1] < self._bbox[1]:
+            bbox[1] = self._bbox[1]
+        if bbox[2] > self._bbox[2]:
+            bbox[2] = self._bbox[2]
+        if bbox[3] > self._bbox[3]:
+            bbox[3] = self._bbox[3]
+
+        year_start = int(str(start_time)[:4])
+        year_end = int(str(end_time)[:4])
+        end_year = int(str(self._endtime)[:4])
+
+        if year_end < end_year:
+            if year_start == year_end:
+                ds = self._get_dataset(
+                    scale="Y",
+                    start_time=start_time,
+                    end_time=end_time,
+                    bbox=bbox,
+                    time_chunks=time_chunks,
+                )
+                return ds
+
+            elif year_start < year_end:
+                dss = []
+                years = range(year_start, year_end + 1)
+                for year in years:
+                    if year == year_start:
+                        dss.append(
+                            self._get_dataset(
+                                scale="Y",
+                                start_time=start_time,
+                                end_time=np.datetime64(
+                                    f"{year}-12-31T23:30:00.000000000"
+                                ),
+                                bbox=bbox,
+                                time_chunks=time_chunks,
+                            )
+                        )
+
+                    elif year == year_end:
+                        dss.append(
+                            self._get_dataset(
+                                scale="Y",
+                                start_time=np.datetime64(
+                                    f"{year}-01-01T00:00:00.000000000"
+                                ),
+                                end_time=end_time,
+                                bbox=bbox,
+                                time_chunks=time_chunks,
+                            )
+                        )
+
+                    else:
+                        dss.append(
+                            self._get_dataset(
+                                scale="Y",
+                                start_time=np.datetime64(
+                                    f"{year}-01-01T00:00:00.000000000"
+                                ),
+                                end_time=np.datetime64(
+                                    f"{year}-12-31T23:30:00.000000000"
+                                ),
+                                bbox=bbox,
+                                time_chunks=time_chunks,
+                            )
+                        )
+                return xr.merge(dss)
+
+        else:
+            month_end = int(str(end_time)[5:7])
+            end_month = int(str(self._endtime)[5:7])
+
+            if year_start == year_end:
+                month_start = int(str(start_time)[5:7])
+                if month_start == month_end:
+                    return self._get_dataset(
+                        scale="M",
+                        start_time=start_time,
+                        end_time=end_time,
+                        bbox=bbox,
+                        time_chunks=time_chunks,
+                    )
+                dss = []
+                for m in range(month_start, month_end + 1):
+                    if m == month_start:
+                        d = calendar.monthrange(year_start, m)[1]
+                        dss.append(
+                            self._get_dataset(
+                                scale="M",
+                                start_time=start_time,
+                                end_time=np.datetime64(
+                                    f"{year_start}-{str(m).zfill(2)}-{str(d).zfill(2)}T23:30:00.000000000"
+                                ),
+                                bbox=bbox,
+                                time_chunks=time_chunks,
+                            )
+                        )
+                    elif m == month_end:
+                        dss.append(
+                            self._get_dataset(
+                                scale="M",
+                                start_time=np.datetime64(
+                                    f"{year_start}-{str(m).zfill(2)}-01T00:00:00.000000000"
+                                ),
+                                end_time=end_time,
+                                bbox=bbox,
+                                time_chunks=time_chunks,
+                            )
+                        )
+                    else:
+                        d = calendar.monthrange(year_start, m)[1]
+                        dss.append(
+                            self._get_dataset(
+                                scale="M",
+                                start_time=np.datetime64(
+                                    f"{year_start}-{str(m).zfill(2)}-01T00:00:00.000000000"
+                                ),
+                                end_time=np.datetime64(
+                                    f"{year_start}-{str(m).zfill(2)}-{str(d).zfill(2)}T23:30:00.000000000"
+                                ),
+                                bbox=bbox,
+                                time_chunks=time_chunks,
+                            )
+                        )
+
+            else:
+                dss = []
+
+                for y in range(year_start, year_end + 1):
+                    if y == year_start:
+                        dss.append(
+                            self._get_dataset(
+                                scale="Y",
+                                start_time=start_time,
+                                end_time=np.datetime64(f"{y}-12-31T23:30:00.000000000"),
+                                bbox=bbox,
+                                time_chunks=time_chunks,
+                            )
+                        )
+
+                    elif y == year_end:
+                        for m in range(1, month_end + 1):
+                            if m == month_end:
+                                dss.append(
+                                    self._get_dataset(
+                                        scale="M",
+                                        start_time=np.datetime64(
+                                            f"{str(y).zfill(4)}-{str(m).zfill(2)}-01T00:00:00.000000000"
+                                        ),
+                                        end_time=end_time,
+                                        bbox=bbox,
+                                        time_chunks=time_chunks,
+                                    )
+                                )
+                            else:
+                                d = calendar.monthrange(y, m)[1]
+                                dss.append(
+                                    self._get_dataset(
+                                        scale="M",
+                                        start_time=np.datetime64(
+                                            f"{str(y).zfill(4)}-{str(m).zfill(2)}-01T00:00:00.000000000"
+                                        ),
+                                        end_time=np.datetime64(
+                                            f"{str(y).zfill(4)}-{str(m).zfill(2)}-{str(d).zfill(2)}T23:30:00.000000000"
+                                        ),
+                                        bbox=bbox,
+                                        time_chunks=time_chunks,
+                                    )
+                                )
+
+                    else:
+                        dss.append(
+                            self._get_dataset(
+                                scale="Y",
+                                start_time=np.datetime64(
+                                    f"{y}-01-01T00:00:00.000000000"
+                                ),
+                                end_time=np.datetime64(f"{y}-12-31T23:30:00.000000000"),
+                                bbox=bbox,
+                                time_chunks=time_chunks,
+                            )
+                        )
+
+            return xr.merge(dss)
+
+    def from_shp(
+        self,
+        start_time=np.datetime64("2023-01-01T00:00:00.000000000"),
+        end_time=np.datetime64("2023-01-02T00:00:00.000000000"),
+        dataset="wis",
+        shp=None,
+        time_resolution="1d",
+        time_chunks=48,
+    ):
+        """
+        通过已有的矢量数据范围从minio服务器读取gpm数据
+
+        Args:
+            start_time (datetime64): 开始时间
+            end_time (datetime64): 结束时间
+            dataset (str): wis或camels
+            shp (str): 矢量数据路径
+            time_resolution (str): 1d或30m
+            time_chunks (int): 分块数量
+
+        Returns:
+            dataset (Dataset): 读取结果
+        """
+
+        gdf = gpd.GeoDataFrame.from_file(shp)
+        b = gdf.bounds
+        bbox = regen_box(
+            (b.loc[0]["minx"], b.loc[0]["miny"], b.loc[0]["maxx"], b.loc[0]["maxy"]),
+            0.1,
+            0.05,
+        )
+
+        ds = self.open_dataset(
+            start_time, end_time, dataset, bbox, time_resolution, time_chunks
+        )
+        return ds
+
+    def from_aoi(
+        self,
+        start_time=np.datetime64("2023-01-01T00:00:00.000000000"),
+        end_time=np.datetime64("2023-01-02T00:00:00.000000000"),
+        dataset="wis",
+        aoi: gpd.GeoDataFrame = None,
+        time_resolution="1d",
+        time_chunks=48,
+    ):
+        """
+        用过已有的GeoPandas.GeoDataFrame对象从minio服务器读取gpm数据
+
+        Args:
+            start_time (datetime64): 开始时间
+            end_time (datetime64): 结束时间
+            dataset (str): wis或camels
+            aoi (GeoDataFrame): 已有的GeoPandas.GeoDataFrame对象
+            time_resolution (str): 1d或30m
+            time_chunks (int): 分块数量
+
+        Returns:
+            dataset (Dataset): 读取结果
+        """
+
+        b = aoi.bounds
+        bbox = regen_box(
+            (b.loc[0]["minx"], b.loc[0]["miny"], b.loc[0]["maxx"], b.loc[0]["maxy"]),
+            0.1,
+            0.05,
+        )
+        ds = self.open_dataset(
+            start_time, end_time, dataset, bbox, time_resolution, time_chunks
+        )
+        return ds
+
+
+class GFSReader:
+    """
+    用于从minio中读取gpm数据
+
+    Attributes:
+        variables (dict): 变量名称及缩写
+
+    Methods:
+        open_dataset(data_variables, creation_date, creation_time, bbox): 从minio中读取gfs数据
+        from_shp(data_variables, creation_date, creation_time, shp): 通过已有的矢量数据范围从minio服务器读取gfs数据
+        from_aoi(data_variables, creation_date, creation_time, aoi): 用过已有的GeoPandas.GeoDataFrame对象从minio服务器读取gfs数据
+    """
+
+    def __init__(self):
+        self._variables = {
+            "dswrf": "downward_shortwave_radiation_flux",
+            "pwat": "precipitable_water_entire_atmosphere",
+            "2r": "relative_humidity_2m_above_ground",
+            "2sh": "specific_humidity_2m_above_ground",
+            "2t": "temperature_2m_above_ground",
+            "tcc": "total_cloud_cover_entire_atmosphere",
+            "tp": "total_precipitation_surface",
+            "10u": "u_component_of_wind_10m_above_ground",
+            "10v": "v_component_of_wind_10m_above_ground",
+        }
+        self._bucket_name = "test"
+        self._default = "tp"
+
+    @property
+    def variables(self):
+        return self._variables
+
+    @property
+    def default_variable(self):
+        return self._default
+
+    def set_default_variable(self, short_name):
+        if short_name in self._variables.keys():
+            self._default = short_name
+        else:
+            raise Exception("变量设置错误")
+
+    def open_dataset(
+        self,
+        creation_date=np.datetime64("2022-09-01"),
+        creation_time="00",
+        dataset="wis",
+        bbox=(115, 38, 136, 54),
+        time_chunks=24,
+    ):
+        """
+        从minio服务器读取gfs数据
+
+        Args:
+            creation_date (datetime64): 创建日期
+            creation_time (datetime64): 创建时间，即00\06\12\18之一
+            dataset (str): wis或camels
+            bbox (list|tuple): 四至范围
+            time_chunks (int): 分块数量
+
+        Returns:
+            dataset (Dataset): 读取结果
+        """
+
+        if bbox[0] > bbox[2] or bbox[1] > bbox[3]:
+            raise Exception("四至范围格式错误")
+
+        if dataset != "wis" and dataset != "camels":
+            raise Exception("dataset参数错误")
+
+        if dataset == "wis":
+            self._dataset = "geodata"
+        elif dataset == "camels":
+            self._dataset = "camdata"
+
+        with FS.open(os.path.join(self._bucket_name, f"{self._dataset}/gfs/gfs.json")) as f:
+            cont = json.load(f)
+            self._paras = cont
+
+        short_name = self._default
+        full_name = self._variables[short_name]
+
+        start = np.datetime64(self._paras[short_name][0]["start"])
+        end = np.datetime64(self._paras[short_name][-1]["end"])
+
+        if creation_date < start or creation_date > end:
+            print("超出时间范围！")
+            return
+
+        if creation_time not in ["00", "06", "12", "18"]:
+            print("creation_time必须是00、06、12、18之一！")
+            return
+
+        year = str(creation_date.astype("object").year)
+        month = str(creation_date.astype("object").month).zfill(2)
+        day = str(creation_date.astype("object").day).zfill(2)
+
+        change = np.datetime64("2022-09-01")
+        if creation_date < change:
+            json_url = f"s3://{self._bucket_name}/{self._dataset}/gfs/gfs_history/{year}/{month}/{day}/gfs{year}{month}{day}.t{creation_time}z.0p25.json"
+        else:
+            json_url = f"s3://{self._bucket_name}/{self._dataset}/gfs/{short_name}/{year}/{month}/{day}/gfs{year}{month}{day}.t{creation_time}z.0p25.json"
+
+        chunks = {"valid_time": time_chunks}
+        ds = xr.open_dataset(
+            "reference://",
+            engine="zarr",
+            chunks=chunks,
+            backend_kwargs={
+                "consolidated": False,
+                "storage_options": {
+                    "fo": json_url,
+                    "target_protocol": "s3",
+                    "target_options": RO,
+                    "remote_protocol": "s3",
+                    "remote_options": RO,
+                },
+            },
+        )
+
+        if creation_date < change:
+            ds = ds[full_name]
+            box = self._paras[short_name][0]["bbox"]
+        else:
+            box = self.paras[short_name][-1]["bbox"]
+
+        # ds = ds.filter_by_attrs(long_name=lambda v: v in data_variables)
+        ds = ds.rename({"longitude": "lon", "latitude": "lat"})
+        # ds = ds.transpose('time','valid_time','lon','lat')
+
+        bbox = regen_box(bbox, 0.25, 0)
+
+        if bbox[0] < box[0]:
+            left = box[0]
+        else:
+            left = bbox[0]
+
+        if bbox[1] < box[1]:
+            bottom = box[1]
+        else:
+            bottom = bbox[1]
+
+        if bbox[2] > box[2]:
+            right = box[2]
+        else:
+            right = bbox[2]
+
+        if bbox[3] > box[3]:
+            top = box[3]
+        else:
+            top = bbox[3]
+
+        longitudes = slice(left - 0.00001, right + 0.00001)
+        latitudes = slice(bottom - 0.00001, top + 0.00001)
+
+        ds = ds.sortby("lat", ascending=True)
+        ds = ds.sel(lon=longitudes, lat=latitudes)
+
+        return ds
+
+    def from_shp(
+        self,
+        creation_date=np.datetime64("2022-09-01"),
+        creation_time="00",
+        dataset="wis",
+        shp=None,
+        time_chunks=24,
+    ):
+        """
+        通过已有的矢量数据范围从minio服务器读取gfs数据
+
+        Args:
+            creation_date (datetime64): 创建日期
+            creation_time (datetime64): 创建时间，即00\06\12\18之一
+            dataset (str): wis或camels
+            shp (str): 矢量数据路径
+            time_chunks (int): 分块数量
+
+        Returns:
+            dataset (Dataset): 读取结果
+        """
+
+        gdf = gpd.GeoDataFrame.from_file(shp)
+        b = gdf.bounds
+        bbox = regen_box(
+            (b.loc[0]["minx"], b.loc[0]["miny"], b.loc[0]["maxx"], b.loc[0]["maxy"]),
+            0.1,
+            0,
+        )
+
+        ds = self.open_dataset(creation_date, creation_time, dataset, bbox, time_chunks)
+
+        return ds
+
+    def from_aoi(
+        self,
+        creation_date=np.datetime64("2022-09-01"),
+        creation_time="00",
+        dataset="wis",
+        aoi: gpd.GeoDataFrame = None,
+        time_chunks=24,
+    ):
+        """
+        通过已有的GeoPandas.GeoDataFrame对象从minio服务器读取gfs数据
+
+        Args:
+            creation_date (datetime64): 创建日期
+            creation_time (datetime64): 创建时间，即00\06\12\18之一
+            dataset (str): wis或camels
+            aoi (GeoDataFrame): 已有的GeoPandas.GeoDataFrame对象
+            time_chunks (int): 分块数量
+
+        Returns:
+            dataset (Dataset): 读取结果
+        """
+        b = aoi.bounds
+        bbox = regen_box(
+            (b.loc[0]["minx"], b.loc[0]["miny"], b.loc[0]["maxx"], b.loc[0]["maxy"]),
+            0.1,
+            0,
+        )
+
+        ds = self.open_dataset(creation_date, creation_time, dataset, bbox, time_chunks)
+
+        return ds
+
+
+class Era5L:
+    def __init__(self):
+        self._catalog = ERA5LCatalog()
+        self._reader = ERA5LReader()
+
+    @property
+    def catalog(self):
+        return self._catalog
+
+    @property
+    def reader(self):
+        return self._reader
+
+
+class GPM:
+    def __init__(self):
+        self._catalog = GPMCatalog()
+        self._reader = GPMReader()
+
+    @property
+    def catalog(self):
+        return self._catalog
+
+    @property
+    def reader(self):
+        return self._reader
+
+
+class GFS:
+    def __init__(self, variable="tp"):
+        self._catalog = GFSCatalog(variable)
+        self._reader = GFSReader()
+        self._reader.set_default_variable(self._catalog.variable)
+
+    @property
+    def catalog(self):
+        return self._catalog
+
+    @property
+    def reader(self):
+        return self._reader
```

### Comparing `hydrodatasource-0.0.1/hydrodatasource/reader/minio_api.py` & `hydrodatasource-0.0.2/hydrodatasource/reader/minio_api.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,140 +1,140 @@
-"""Main module."""
-import asyncio
-import os
-import pathlib
-
-from minio import Minio
-import chardet
-
-
-async def minio_upload_csv(client, bucket_name, object_name, file_path):
-    """upload csv to minio
-
-    Parameters
-    ----------
-    client : _type_
-        the minio client
-    bucket_name : _type_
-        the bucket name
-    object_name : _type_
-        the object name
-    file_path : _type_
-        the local file path
-    """
-    # Make a bucket
-    bucket_names = [bucket.name for bucket in client.list_buckets()]
-    if bucket_name not in bucket_names:
-        client.make_bucket(bucket_name)
-    # Upload an object
-    client.fput_object(bucket_name, object_name, file_path)
-    # List objects
-    objects = client.list_objects(bucket_name, recursive=True)
-    return [obj.object_name for obj in objects]
-
-
-async def minio_download_csv(client: Minio, bucket_name, object_name: str, file_path: str, version_id=None):
-    try:
-        response = client.get_object(bucket_name, object_name, version_id)
-        # 图片不能直接解码, 但可以直接对文件写入response.data
-        encoding = chardet.detect(response.data)['encoding']
-        object_path = os.path.join(file_path, object_name)
-        object_parent = pathlib.Path(object_path).parent
-        if not object_parent.exists():
-            object_parent.mkdir(parents=True)
-        if encoding is not None:
-            res_csv: str = response.data.decode(encoding)
-            with open(object_path, 'w+', encoding=encoding) as fp:
-                fp.write(res_csv)
-        else:
-            with open(object_path, 'wb') as fp:
-                fp.write(response.data)
-    finally:
-        response.close()
-        response.release_conn()
-
-
-async def boto3_upload_csv(client, bucket_name, object_name, file_path):
-    """upload csv to minio
-
-    Parameters
-    ----------
-    client : _type_
-        the minio client
-    bucket_name : _type_
-        the bucket name
-    object_name : _type_
-        the object name
-    file_path : _type_
-        the local file path
-    """
-    # Make a bucket
-    bucket_names = [dic['Name'] for dic in client.list_buckets()['Buckets']]
-    if bucket_name not in bucket_names:
-        client.create_bucket(Bucket=bucket_name)
-    # Upload an object
-    client.upload_file(file_path, bucket_name, object_name)
-    # List objects
-    objects = [dic['Key'] for dic in client.list_objects(Bucket=bucket_name)['Contents']]
-    return objects
-
-
-async def boto3_download_csv(client, bucket_name, object_name, file_path: str):
-    client.download_file(bucket_name, object_name, file_path)
-
-
-async def boto3_sync_files(client, bucket_name, local_path, bucket_path=None):
-    """
-    :param client: the boto3 client
-    :param bucket_name: the bucket name which you want to sync your data
-    :param local_path: the path on your local machine
-    :param bucket_path: the path under your bucket which you want to sync
-    :return:
-    """
-    remote_objects = [dic['Key'] for dic in client.list_objects(Bucket=bucket_name)['Contents']]
-    local_objects = [str(path.relative_to(local_path)).replace('\\', '/')
-                     for path in pathlib.Path(local_path).rglob(pattern='*') if path.is_file()]
-    objects_in_remote = [obj for obj in remote_objects if obj not in local_objects]
-    objects_in_local = [obj for obj in local_objects if obj not in remote_objects]
-    task_batch_dload = asyncio.create_task(boto3_batch_download(objects_in_remote, client, bucket_name, local_path))
-    task_batch_upload = asyncio.create_task(boto3_batch_upload(objects_in_local, client, bucket_name, local_path))
-    await asyncio.gather(task_batch_upload, task_batch_dload)
-
-
-async def minio_batch_download(objects_in_remote, client: Minio, bucket_name, local_path):
-    # 将下载任务打包成大量task容易造成许多上下文切换进而挤兑，目前看来不如顺序下载
-    for obj in objects_in_remote:
-        await minio_download_csv(client, bucket_name, obj, local_path)
-
-
-async def minio_batch_upload(objects_in_local, client: Minio, bucket_name, local_path):
-    for obj in objects_in_local:
-        await minio_upload_csv(client, bucket_name, obj, local_path)
-
-
-async def boto3_batch_download(objects_in_remote, client, bucket_name, local_path):
-    # 将下载任务打包成大量task容易造成许多上下文切换进而挤兑，目前看来不如顺序下载
-    for obj in objects_in_remote:
-        await boto3_download_csv(client, bucket_name, obj, local_path)
-
-
-async def boto3_batch_upload(objects_in_remote, client, bucket_name, local_path):
-    for obj in objects_in_remote:
-        await boto3_upload_csv(client, bucket_name, obj, local_path)
-
-
-async def minio_sync_files(client: Minio, bucket_name, local_path, bucket_path=None):
-    """
-    :param client: the minio client
-    :param bucket_name: the bucket name which you want to sync your data
-    :param local_path: the path on your local machine, contents of bucket_name will be saved to the directory directly
-    :param bucket_path: the path under your bucket which you want to sync
-    :return:
-    """
-    remote_objects = [obj.object_name for obj in client.list_objects(bucket_name, prefix=bucket_path, recursive=True)]
-    local_objects = [str(path.relative_to(local_path)).replace('\\', '/')
-                     for path in pathlib.Path(local_path).rglob(pattern='*') if path.is_file()]
-    objects_in_remote = [obj for obj in remote_objects if obj not in local_objects]
-    objects_in_local = [obj for obj in local_objects if obj not in remote_objects]
-    task_batch_dload = asyncio.create_task(minio_batch_download(objects_in_remote, client, bucket_name, local_path))
-    task_batch_upload = asyncio.create_task(minio_batch_upload(objects_in_local, client, bucket_name, local_path))
-    await asyncio.gather(task_batch_upload, task_batch_dload)
+"""Main module."""
+import asyncio
+import os
+import pathlib
+
+from minio import Minio
+import chardet
+
+
+async def minio_upload_csv(client, bucket_name, object_name, file_path):
+    """upload csv to minio
+
+    Parameters
+    ----------
+    client : _type_
+        the minio client
+    bucket_name : _type_
+        the bucket name
+    object_name : _type_
+        the object name
+    file_path : _type_
+        the local file path
+    """
+    # Make a bucket
+    bucket_names = [bucket.name for bucket in client.list_buckets()]
+    if bucket_name not in bucket_names:
+        client.make_bucket(bucket_name)
+    # Upload an object
+    client.fput_object(bucket_name, object_name, file_path)
+    # List objects
+    objects = client.list_objects(bucket_name, recursive=True)
+    return [obj.object_name for obj in objects]
+
+
+async def minio_download_csv(client: Minio, bucket_name, object_name: str, file_path: str, version_id=None):
+    try:
+        response = client.get_object(bucket_name, object_name, version_id)
+        # 图片不能直接解码, 但可以直接对文件写入response.data
+        encoding = chardet.detect(response.data)['encoding']
+        object_path = os.path.join(file_path, object_name)
+        object_parent = pathlib.Path(object_path).parent
+        if not object_parent.exists():
+            object_parent.mkdir(parents=True)
+        if encoding is not None:
+            res_csv: str = response.data.decode(encoding)
+            with open(object_path, 'w+', encoding=encoding) as fp:
+                fp.write(res_csv)
+        else:
+            with open(object_path, 'wb') as fp:
+                fp.write(response.data)
+    finally:
+        response.close()
+        response.release_conn()
+
+
+async def boto3_upload_csv(client, bucket_name, object_name, file_path):
+    """upload csv to minio
+
+    Parameters
+    ----------
+    client : _type_
+        the minio client
+    bucket_name : _type_
+        the bucket name
+    object_name : _type_
+        the object name
+    file_path : _type_
+        the local file path
+    """
+    # Make a bucket
+    bucket_names = [dic['Name'] for dic in client.list_buckets()['Buckets']]
+    if bucket_name not in bucket_names:
+        client.create_bucket(Bucket=bucket_name)
+    # Upload an object
+    client.upload_file(file_path, bucket_name, object_name)
+    # List objects
+    objects = [dic['Key'] for dic in client.list_objects(Bucket=bucket_name)['Contents']]
+    return objects
+
+
+async def boto3_download_csv(client, bucket_name, object_name, file_path: str):
+    client.download_file(bucket_name, object_name, file_path)
+
+
+async def boto3_sync_files(client, bucket_name, local_path, bucket_path=None):
+    """
+    :param client: the boto3 client
+    :param bucket_name: the bucket name which you want to sync your data
+    :param local_path: the path on your local machine
+    :param bucket_path: the path under your bucket which you want to sync
+    :return:
+    """
+    remote_objects = [dic['Key'] for dic in client.list_objects(Bucket=bucket_name)['Contents']]
+    local_objects = [str(path.relative_to(local_path)).replace('\\', '/')
+                     for path in pathlib.Path(local_path).rglob(pattern='*') if path.is_file()]
+    objects_in_remote = [obj for obj in remote_objects if obj not in local_objects]
+    objects_in_local = [obj for obj in local_objects if obj not in remote_objects]
+    task_batch_dload = asyncio.create_task(boto3_batch_download(objects_in_remote, client, bucket_name, local_path))
+    task_batch_upload = asyncio.create_task(boto3_batch_upload(objects_in_local, client, bucket_name, local_path))
+    await asyncio.gather(task_batch_upload, task_batch_dload)
+
+
+async def minio_batch_download(objects_in_remote, client: Minio, bucket_name, local_path):
+    # 将下载任务打包成大量task容易造成许多上下文切换进而挤兑，目前看来不如顺序下载
+    for obj in objects_in_remote:
+        await minio_download_csv(client, bucket_name, obj, local_path)
+
+
+async def minio_batch_upload(objects_in_local, client: Minio, bucket_name, local_path):
+    for obj in objects_in_local:
+        await minio_upload_csv(client, bucket_name, obj, local_path)
+
+
+async def boto3_batch_download(objects_in_remote, client, bucket_name, local_path):
+    # 将下载任务打包成大量task容易造成许多上下文切换进而挤兑，目前看来不如顺序下载
+    for obj in objects_in_remote:
+        await boto3_download_csv(client, bucket_name, obj, local_path)
+
+
+async def boto3_batch_upload(objects_in_remote, client, bucket_name, local_path):
+    for obj in objects_in_remote:
+        await boto3_upload_csv(client, bucket_name, obj, local_path)
+
+
+async def minio_sync_files(client: Minio, bucket_name, local_path, bucket_path=None):
+    """
+    :param client: the minio client
+    :param bucket_name: the bucket name which you want to sync your data
+    :param local_path: the path on your local machine, contents of bucket_name will be saved to the directory directly
+    :param bucket_path: the path under your bucket which you want to sync
+    :return:
+    """
+    remote_objects = [obj.object_name for obj in client.list_objects(bucket_name, prefix=bucket_path, recursive=True)]
+    local_objects = [str(path.relative_to(local_path)).replace('\\', '/')
+                     for path in pathlib.Path(local_path).rglob(pattern='*') if path.is_file()]
+    objects_in_remote = [obj for obj in remote_objects if obj not in local_objects]
+    objects_in_local = [obj for obj in local_objects if obj not in remote_objects]
+    task_batch_dload = asyncio.create_task(minio_batch_download(objects_in_remote, client, bucket_name, local_path))
+    task_batch_upload = asyncio.create_task(minio_batch_upload(objects_in_local, client, bucket_name, local_path))
+    await asyncio.gather(task_batch_upload, task_batch_dload)
```

### Comparing `hydrodatasource-0.0.1/hydrodatasource/reader/reader.py` & `hydrodatasource-0.0.2/hydrodatasource/reader/reader.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-"""
-Author: Wenyu Ouyang
-Date: 2023-10-31 09:26:31
-LastEditTime: 2024-03-28 08:33:33
-LastEditors: Wenyu Ouyang
-Description: Interface for reader
-FilePath: \hydrodata\hydrodatasource\reader\reader.py
-Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
-"""
-
-from abc import ABC, abstractmethod
-import os
-import json
-import datetime
-import xarray as xr
-
-from hydrodatasource.processor.gpm_gfs import make1nc41basin
-from hydrodatasource.configs.config import LOCAL_DATA_PATH, GRID_INTERIM_BUCKET, RO, FS
-from hydrodatasource.processor.mask import gen_single_mask
-
-
-class AOI:
-    def __init__(self, aoi_type, aoi_param):
-        self._aoi_type = aoi_type  # can be "grid", "station", "basin" etc.
-        self._aoi_param = aoi_param  # this can be a bounding box, coordinates, etc.
-
-    @property
-    def aoi_type(self):
-        return self._aoi_type
-
-    @property
-    def aoi_param(self):
-        return self._aoi_param
-
-    def get_mask(self):
-        # If it's a polygon, return its mask for data extraction
-        if self._aoi_type == "basin":
-            return gen_single_mask(
-                basin_id=self._aoi_param,
-                shp_path=os.path.join(LOCAL_DATA_PATH, "datasets-origin", "shp"),
-                dataname="gpm",
-                mask_path=os.path.join(LOCAL_DATA_PATH, "datasets-origin", "mask"),
-            )
-        else:
-            # basin only for now
-            raise NotImplementedError("Only basin available for now")
-
-    # ... any other useful methods to describe or manipulate the AOI
-
-
-class CommonHandler(AOI):
-    def __init__(self, aoi_type, aoi_param, region=None, time_periods=None):
-        super().__init__(aoi_type, aoi_param)
-        self._region = region  # camels or wis, "camels" is on behalf of us, "wis" is on behalf of cn
-        self._time_periods = time_periods
-
-    @property
-    def region(self):
-        return self._region
-
-    @property
-    def time_periods(self):
-        return self._time_periods
-
-    def is_valid_time_periods(self):
-        # 检查 time_periods 是否是列表
-        if not isinstance(self._time_periods, list):
-            return False
-
-        for period in self._time_periods:
-            # 检查每个元素是否是包含两个元素的列表
-            if not isinstance(period, list) or len(period) != 2:
-                return False
-
-            # 检查每个元素是否是字符串且符合日期时间格式
-            for date_str in period:
-                if not isinstance(date_str, str):
-                    return False
-                try:
-                    datetime.datetime.strptime(date_str, "%Y-%m-%dT%H:%M:%S")
-                except ValueError:
-                    return False
-
-        return True
-
-    def read_file_from_minio(self):
-        try:
-            json_file_path = os.path.join(self._aoi_param, f"{self._dataname}.json")
-            # 从 MinIO 读取 JSON 文件
-            with FS.open(f"{GRID_INTERIM_BUCKET}/{json_file_path}") as f:
-                json_data = json.load(f)
-            # 使用 xarray 和 kerchunk 读取数据
-            return xr.open_dataset(
-                "reference://",
-                engine="zarr",
-                backend_kwargs={
-                    "consolidated": False,
-                    "storage_options": {
-                        "fo": json_data,
-                        "remote_protocol": "s3",
-                        "remote_options": RO,
-                    },
-                },
-            )
-        except:
-            raise FileNotFoundError(
-                "Please check the file in the minio server. \
-                This error is generally caused by the following two situations:\n\
-                    1. There is no file for this basin in the minio server. Please make a new one and upload it.\n\
-                    2. Check your settings. Make sure you have enough permission to access the minio server and the bucket."
-            )
-
-
-class DataHandler(CommonHandler):
-    def __init__(
-        self,
-        aoi_type,
-        aoi_param,
-        region=None,
-        time_periods=None,
-        dataname=None,
-        minio_read=True,
-        local_save=True,
-        minio_upload=False,
-    ):
-        super().__init__(aoi_type, aoi_param, region, time_periods)
-        self._dataname = dataname
-        self._minio_read = minio_read
-        self._local_save = local_save
-        self._minio_upload = minio_upload
-
-    @property
-    def dataname(self):
-        return self._local_file_path
-
-    @property
-    def dataname(self):
-        return self._dataname
-
-    @property
-    def minio_read(self):
-        return self._minio_read
-
-    @property
-    def local_save(self):
-        return self._local_save
-
-    @property
-    def minio_upload(self):
-        return self._minio_upload
-
-    def handle(self):
-        if self._minio_read == True:
-            return self.read_file_from_minio()
-        else:
-            return make1nc41basin(
-                basin_id=self._aoi_param,
-                dataname=self._dataname,
-                local_path=LOCAL_DATA_PATH,
-                mask_path=os.path.join(LOCAL_DATA_PATH, "datasets-origin", "mask"),
-                shp_path=os.path.join(LOCAL_DATA_PATH, "datasets-origin", "shp"),
-                dataset=self._region,
-                time_periods=self._time_periods,
-                local_save=self._local_save,
-                minio_upload=self._minio_upload,
-            )
-
-    # TODO: time_periods is only used in make1nc41basin funtion, it needs to be used in other cases
-
-
-class DataReaderStrategy(ABC):
-    @abstractmethod
-    def read(self, path: str, aoi: AOI):
-        pass
-
-
-class AbstractFileReader(DataReaderStrategy):
-    def __init__(self, data_handler):
-        self.data_handler = data_handler
-
-    @abstractmethod
-    def configure(self, path: str, aoi: AOI):
-        pass
-
-    def read(self, path: str, aoi: AOI):
-        configuration = self.configure(path, aoi)
-        return self.data_handler.handle(configuration)
-
-
-class LocalFileReader(AbstractFileReader):
-    def configure(self, path: str, aoi: AOI):
-        return {"type": "local", "path": path, "aoi": aoi}
-
-
-class MinioFileReader(AbstractFileReader):
-    def __init__(self, minio_client, data_handler):
-        super().__init__(data_handler)
-        self.client = minio_client
-
-    def configure(self, path: str, aoi: AOI):
-        return {"type": "minio", "bucket": "your_bucket_name", "path": path, "aoi": aoi}
+"""
+Author: Wenyu Ouyang
+Date: 2023-10-31 09:26:31
+LastEditTime: 2024-03-28 08:33:33
+LastEditors: Wenyu Ouyang
+Description: Interface for reader
+FilePath: \hydrodata\hydrodatasource\reader\reader.py
+Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
+"""
+
+from abc import ABC, abstractmethod
+import os
+import json
+import datetime
+import xarray as xr
+
+from hydrodatasource.processor.gpm_gfs import make1nc41basin
+from hydrodatasource.configs.config import LOCAL_DATA_PATH, GRID_INTERIM_BUCKET, RO, FS
+from hydrodatasource.processor.mask import gen_single_mask
+
+
+class AOI:
+    def __init__(self, aoi_type, aoi_param):
+        self._aoi_type = aoi_type  # can be "grid", "station", "basin" etc.
+        self._aoi_param = aoi_param  # this can be a bounding box, coordinates, etc.
+
+    @property
+    def aoi_type(self):
+        return self._aoi_type
+
+    @property
+    def aoi_param(self):
+        return self._aoi_param
+
+    def get_mask(self):
+        # If it's a polygon, return its mask for data extraction
+        if self._aoi_type == "basin":
+            return gen_single_mask(
+                basin_id=self._aoi_param,
+                shp_path=os.path.join(LOCAL_DATA_PATH, "datasets-origin", "shp"),
+                dataname="gpm",
+                mask_path=os.path.join(LOCAL_DATA_PATH, "datasets-origin", "mask"),
+            )
+        else:
+            # basin only for now
+            raise NotImplementedError("Only basin available for now")
+
+    # ... any other useful methods to describe or manipulate the AOI
+
+
+class CommonHandler(AOI):
+    def __init__(self, aoi_type, aoi_param, region=None, time_periods=None):
+        super().__init__(aoi_type, aoi_param)
+        self._region = region  # camels or wis, "camels" is on behalf of us, "wis" is on behalf of cn
+        self._time_periods = time_periods
+
+    @property
+    def region(self):
+        return self._region
+
+    @property
+    def time_periods(self):
+        return self._time_periods
+
+    def is_valid_time_periods(self):
+        # 检查 time_periods 是否是列表
+        if not isinstance(self._time_periods, list):
+            return False
+
+        for period in self._time_periods:
+            # 检查每个元素是否是包含两个元素的列表
+            if not isinstance(period, list) or len(period) != 2:
+                return False
+
+            # 检查每个元素是否是字符串且符合日期时间格式
+            for date_str in period:
+                if not isinstance(date_str, str):
+                    return False
+                try:
+                    datetime.datetime.strptime(date_str, "%Y-%m-%dT%H:%M:%S")
+                except ValueError:
+                    return False
+
+        return True
+
+    def read_file_from_minio(self):
+        try:
+            json_file_path = os.path.join(self._aoi_param, f"{self._dataname}.json")
+            # 从 MinIO 读取 JSON 文件
+            with FS.open(f"{GRID_INTERIM_BUCKET}/{json_file_path}") as f:
+                json_data = json.load(f)
+            # 使用 xarray 和 kerchunk 读取数据
+            return xr.open_dataset(
+                "reference://",
+                engine="zarr",
+                backend_kwargs={
+                    "consolidated": False,
+                    "storage_options": {
+                        "fo": json_data,
+                        "remote_protocol": "s3",
+                        "remote_options": RO,
+                    },
+                },
+            )
+        except:
+            raise FileNotFoundError(
+                "Please check the file in the minio server. \
+                This error is generally caused by the following two situations:\n\
+                    1. There is no file for this basin in the minio server. Please make a new one and upload it.\n\
+                    2. Check your settings. Make sure you have enough permission to access the minio server and the bucket."
+            )
+
+
+class DataHandler(CommonHandler):
+    def __init__(
+        self,
+        aoi_type,
+        aoi_param,
+        region=None,
+        time_periods=None,
+        dataname=None,
+        minio_read=True,
+        local_save=True,
+        minio_upload=False,
+    ):
+        super().__init__(aoi_type, aoi_param, region, time_periods)
+        self._dataname = dataname
+        self._minio_read = minio_read
+        self._local_save = local_save
+        self._minio_upload = minio_upload
+
+    @property
+    def dataname(self):
+        return self._local_file_path
+
+    @property
+    def dataname(self):
+        return self._dataname
+
+    @property
+    def minio_read(self):
+        return self._minio_read
+
+    @property
+    def local_save(self):
+        return self._local_save
+
+    @property
+    def minio_upload(self):
+        return self._minio_upload
+
+    def handle(self):
+        if self._minio_read == True:
+            return self.read_file_from_minio()
+        else:
+            return make1nc41basin(
+                basin_id=self._aoi_param,
+                dataname=self._dataname,
+                local_path=LOCAL_DATA_PATH,
+                mask_path=os.path.join(LOCAL_DATA_PATH, "datasets-origin", "mask"),
+                shp_path=os.path.join(LOCAL_DATA_PATH, "datasets-origin", "shp"),
+                dataset=self._region,
+                time_periods=self._time_periods,
+                local_save=self._local_save,
+                minio_upload=self._minio_upload,
+            )
+
+    # TODO: time_periods is only used in make1nc41basin funtion, it needs to be used in other cases
+
+
+class DataReaderStrategy(ABC):
+    @abstractmethod
+    def read(self, path: str, aoi: AOI):
+        pass
+
+
+class AbstractFileReader(DataReaderStrategy):
+    def __init__(self, data_handler):
+        self.data_handler = data_handler
+
+    @abstractmethod
+    def configure(self, path: str, aoi: AOI):
+        pass
+
+    def read(self, path: str, aoi: AOI):
+        configuration = self.configure(path, aoi)
+        return self.data_handler.handle(configuration)
+
+
+class LocalFileReader(AbstractFileReader):
+    def configure(self, path: str, aoi: AOI):
+        return {"type": "local", "path": path, "aoi": aoi}
+
+
+class MinioFileReader(AbstractFileReader):
+    def __init__(self, minio_client, data_handler):
+        super().__init__(data_handler)
+        self.client = minio_client
+
+    def configure(self, path: str, aoi: AOI):
+        return {"type": "minio", "bucket": "your_bucket_name", "path": path, "aoi": aoi}
```

### Comparing `hydrodatasource-0.0.1/hydrodatasource/utils/utils.py` & `hydrodatasource-0.0.2/hydrodatasource/utils/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,228 +1,287 @@
-import numpy as np
-from netCDF4 import Dataset, date2num, num2date
-import time
-from datetime import datetime, timedelta
-import pandas as pd
-import pint
-import xarray as xr
-
-# please don't remove the following line although it seems not used
-import pint_xarray  # noqa
-
-
-def creatspinc(value, data_vars, lats, lons, starttime, filename, resolution):
-    gridspi = Dataset(filename, "w", format="NETCDF4")
-
-    # dimensions
-    gridspi.createDimension("time", value[0].shape[0])
-    gridspi.createDimension("lat", value[0].shape[2])  # len(lat)
-    gridspi.createDimension("lon", value[0].shape[1])
-
-    # Create coordinate variables for dimensions
-    times = gridspi.createVariable("time", np.float64, ("time",))
-    latitudes = gridspi.createVariable("lat", np.float32, ("lat",))
-    longitudes = gridspi.createVariable("lon", np.float32, ("lon",))
-
-    # Create the actual variable
-    for var, attr in data_vars.items():
-        gridspi.createVariable(
-            var,
-            np.float32,
-            (
-                "time",
-                "lon",
-                "lat",
-            ),
-        )
-
-    # Global Attributes
-    gridspi.description = "var"
-    gridspi.history = f"Created {time.ctime(time.time())}"
-    gridspi.source = "netCDF4 python module tutorial"
-
-    # Variable Attributes
-    latitudes.units = "degree_north"
-    longitudes.units = "degree_east"
-    times.units = "days since 1970-01-01 00:00:00"
-    times.calendar = "gregorian"
-
-    # data
-    latitudes[:] = lats
-    longitudes[:] = lons
-
-    # Fill in times
-    dates = []
-    if resolution == "daily":
-        for n in range(value[0].shape[0]):
-            dates.append(starttime + n)
-        times[:] = dates[:]
-
-    elif resolution == "6-hourly":
-        # for n in range(value[0].shape[0]):
-        #     dates.append(starttime + (n+1) * np.timedelta64(6, 'h'))
-
-        for n in range(value[0].shape[0]):
-            dates.append(starttime + (n + 1) * timedelta(hours=6))
-
-        times[:] = date2num(dates, units=times.units, calendar=times.calendar)
-        # print 'time values (in units %s): ' % times.units +'\n', times[:]
-        dates = num2date(times[:], units=times.units, calendar=times.calendar)
-
-    # Fill in values
-    i = 0
-    for var, attr in data_vars.items():
-        gridspi.variables[var].long_name = attr["long_name"]
-        gridspi.variables[var].units = attr["units"]
-        gridspi.variables[var][:] = value[i][:]
-        i = i + 1
-
-    gridspi.close()
-
-
-def regen_box(bbox, resolution, offset):
-    lx = bbox[0]
-    rx = bbox[2]
-    LLON = np.round(
-        int(lx)
-        + resolution * int((lx - int(lx)) / resolution + 0.5)
-        + offset
-        * (int(lx * 10) / 10 + offset - lx)
-        / abs(int(lx * 10) // 10 + offset - lx + 0.0000001),
-        3,
-    )
-    RLON = np.round(
-        int(rx)
-        + resolution * int((rx - int(rx)) / resolution + 0.5)
-        - offset
-        * (int(rx * 10) / 10 + offset - rx)
-        / abs(int(rx * 10) // 10 + offset - rx + 0.0000001),
-        3,
-    )
-
-    by = bbox[1]
-    ty = bbox[3]
-    BLAT = np.round(
-        int(by)
-        + resolution * int((by - int(by)) / resolution + 0.5)
-        + offset
-        * (int(by * 10) / 10 + offset - by)
-        / abs(int(by * 10) // 10 + offset - by + 0.0000001),
-        3,
-    )
-    TLAT = np.round(
-        int(ty)
-        + resolution * int((ty - int(ty)) / resolution + 0.5)
-        - offset
-        * (int(ty * 10) / 10 + offset - ty)
-        / abs(int(ty * 10) // 10 + offset - ty + 0.0000001),
-        3,
-    )
-
-    # print(LLON,BLAT,RLON,TLAT)
-    return [LLON, BLAT, RLON, TLAT]
-
-
-def validate(date_text, formatter, error):
-    try:
-        return datetime.strptime(date_text, formatter)
-    except ValueError as e:
-        raise ValueError(error) from e
-
-
-def cf2datetime(ds):
-    ds = ds.copy()
-    time_tmp1 = ds.indexes["time"]
-    attrs = ds.coords["time"].attrs
-    time_tmp2 = []
-    for i in range(time_tmp1.shape[0]):
-        tmp = time_tmp1[i]
-        a = str(tmp.year).zfill(4)
-        b = str(tmp.month).zfill(2)
-        c = str(tmp.day).zfill(2)
-        d = str(tmp.hour).zfill(2)
-        e = str(tmp.minute).zfill(2)
-        f = str(tmp.second).zfill(2)
-        time_tmp2.append(np.datetime64(f"{a}-{b}-{c} {d}:{e}:{f}.00000000"))
-    ds = ds.assign_coords(time=time_tmp2)
-    ds.coords["time"].attrs = attrs
-
-    return ds
-
-
-def generate_time_intervals(start_date, end_date):
-    # Initialize an empty list to store the intervals
-    intervals = []
-
-    # Loop over days
-    while start_date <= end_date:
-        # Loop over the four time intervals in a day
-        intervals.extend(
-            [start_date.strftime("%Y-%m-%d"), hour] for hour in ["00", "06", "12", "18"]
-        )
-        # Move to the next day
-        start_date += timedelta(days=1)
-
-    return intervals
-
-
-def streamflow_unit_conv(streamflow, area, target_unit="mm/d", inverse=False):
-    """Convert the unit of streamflow data to mm/xx(time) for a basin or inverse.
-
-    Parameters
-    ----------
-    streamflow: xarray.Dataset, numpy.ndarray, pandas.DataFrame/Series
-        Streamflow data of each basin.
-    area: xarray.Dataset or pint.Quantity wrapping numpy.ndarray, pandas.DataFrame/Series
-        Area of each basin.
-    target_unit: str
-        The unit to convert to.
-    inverse: bool
-        If True, convert the unit to m^3/s.
-        If False, convert the unit to mm/day or mm/h.
-
-    Returns
-    -------
-    Converted data in the same type as the input streamflow.
-    """
-
-    # Function to handle the conversion for numpy and pandas
-    def np_pd_conversion(streamflow, area, target_unit, inverse):
-        if not inverse:
-            result = (streamflow / area).to(target_unit)
-        else:
-            result = (streamflow * area).to(target_unit)
-        return result.magnitude
-
-    # Handle xarray
-    if isinstance(streamflow, xr.Dataset) and isinstance(area, xr.Dataset):
-        if not inverse:
-            if target_unit not in ["mm/d", "mm/day", "mm/h", "mm/hour"]:
-                raise ValueError("target_unit should be 'mm/d' or 'mm/h'")
-            q = streamflow.pint.quantify()
-            a = area.pint.quantify()
-            r = q[list(q.keys())[0]] / a[list(a.keys())[0]]
-            result = r.pint.to(target_unit).to_dataset(name=list(q.keys())[0])
-        else:
-            if target_unit not in ["m^3/s", "m3/s"]:
-                raise ValueError("target_unit should be 'm^3/s'")
-            r = streamflow.pint.quantify()
-            a = area.pint.quantify()
-            q = r[list(r.keys())[0]] * a[list(a.keys())[0]]
-            result = q.pint.to(target_unit).to_dataset(name=list(r.keys())[0])
-        # dequantify to get normal xr_dataset
-        return result.pint.dequantify()
-
-    # Handle numpy and pandas
-    elif isinstance(streamflow, pint.Quantity) and isinstance(area, pint.Quantity):
-        if type(streamflow.magnitude) not in [np.ndarray, pd.DataFrame, pd.Series]:
-            raise TypeError(
-                "Input streamflow must be xarray.Dataset, or pint.Quantity wrapping numpy.ndarray, or pandas.DataFrame/Series"
-            )
-        if type(area.magnitude) != type(streamflow.magnitude):
-            raise TypeError("streamflow and area must be the same type")
-        return np_pd_conversion(streamflow, area, target_unit, inverse)
-
-    else:
-        raise TypeError(
-            "Input streamflow must be xarray.Dataset, or pint.Quantity wrapping numpy.ndarray, or pandas.DataFrame/Series"
-        )
+import re
+import numpy as np
+from netCDF4 import Dataset, date2num, num2date
+import time
+from datetime import datetime, timedelta
+import pandas as pd
+import pint
+import xarray as xr
+
+# please don't remove the following line although it seems not used
+import pint_xarray  # noqa
+
+
+def creatspinc(value, data_vars, lats, lons, starttime, filename, resolution):
+    gridspi = Dataset(filename, "w", format="NETCDF4")
+
+    # dimensions
+    gridspi.createDimension("time", value[0].shape[0])
+    gridspi.createDimension("lat", value[0].shape[2])  # len(lat)
+    gridspi.createDimension("lon", value[0].shape[1])
+
+    # Create coordinate variables for dimensions
+    times = gridspi.createVariable("time", np.float64, ("time",))
+    latitudes = gridspi.createVariable("lat", np.float32, ("lat",))
+    longitudes = gridspi.createVariable("lon", np.float32, ("lon",))
+
+    # Create the actual variable
+    for var, attr in data_vars.items():
+        gridspi.createVariable(
+            var,
+            np.float32,
+            (
+                "time",
+                "lon",
+                "lat",
+            ),
+        )
+
+    # Global Attributes
+    gridspi.description = "var"
+    gridspi.history = f"Created {time.ctime(time.time())}"
+    gridspi.source = "netCDF4 python module tutorial"
+
+    # Variable Attributes
+    latitudes.units = "degree_north"
+    longitudes.units = "degree_east"
+    times.units = "days since 1970-01-01 00:00:00"
+    times.calendar = "gregorian"
+
+    # data
+    latitudes[:] = lats
+    longitudes[:] = lons
+
+    # Fill in times
+    dates = []
+    if resolution == "daily":
+        for n in range(value[0].shape[0]):
+            dates.append(starttime + n)
+        times[:] = dates[:]
+
+    elif resolution == "6-hourly":
+        # for n in range(value[0].shape[0]):
+        #     dates.append(starttime + (n+1) * np.timedelta64(6, 'h'))
+
+        for n in range(value[0].shape[0]):
+            dates.append(starttime + (n + 1) * timedelta(hours=6))
+
+        times[:] = date2num(dates, units=times.units, calendar=times.calendar)
+        # print 'time values (in units %s): ' % times.units +'\n', times[:]
+        dates = num2date(times[:], units=times.units, calendar=times.calendar)
+
+    # Fill in values
+    i = 0
+    for var, attr in data_vars.items():
+        gridspi.variables[var].long_name = attr["long_name"]
+        gridspi.variables[var].units = attr["units"]
+        gridspi.variables[var][:] = value[i][:]
+        i = i + 1
+
+    gridspi.close()
+
+
+def regen_box(bbox, resolution, offset):
+    lx = bbox[0]
+    rx = bbox[2]
+    LLON = np.round(
+        int(lx)
+        + resolution * int((lx - int(lx)) / resolution + 0.5)
+        + offset
+        * (int(lx * 10) / 10 + offset - lx)
+        / abs(int(lx * 10) // 10 + offset - lx + 0.0000001),
+        3,
+    )
+    RLON = np.round(
+        int(rx)
+        + resolution * int((rx - int(rx)) / resolution + 0.5)
+        - offset
+        * (int(rx * 10) / 10 + offset - rx)
+        / abs(int(rx * 10) // 10 + offset - rx + 0.0000001),
+        3,
+    )
+
+    by = bbox[1]
+    ty = bbox[3]
+    BLAT = np.round(
+        int(by)
+        + resolution * int((by - int(by)) / resolution + 0.5)
+        + offset
+        * (int(by * 10) / 10 + offset - by)
+        / abs(int(by * 10) // 10 + offset - by + 0.0000001),
+        3,
+    )
+    TLAT = np.round(
+        int(ty)
+        + resolution * int((ty - int(ty)) / resolution + 0.5)
+        - offset
+        * (int(ty * 10) / 10 + offset - ty)
+        / abs(int(ty * 10) // 10 + offset - ty + 0.0000001),
+        3,
+    )
+
+    # print(LLON,BLAT,RLON,TLAT)
+    return [LLON, BLAT, RLON, TLAT]
+
+
+def validate(date_text, formatter, error):
+    try:
+        return datetime.strptime(date_text, formatter)
+    except ValueError as e:
+        raise ValueError(error) from e
+
+
+def cf2datetime(ds):
+    ds = ds.copy()
+    time_tmp1 = ds.indexes["time"]
+    attrs = ds.coords["time"].attrs
+    time_tmp2 = []
+    for i in range(time_tmp1.shape[0]):
+        tmp = time_tmp1[i]
+        a = str(tmp.year).zfill(4)
+        b = str(tmp.month).zfill(2)
+        c = str(tmp.day).zfill(2)
+        d = str(tmp.hour).zfill(2)
+        e = str(tmp.minute).zfill(2)
+        f = str(tmp.second).zfill(2)
+        time_tmp2.append(np.datetime64(f"{a}-{b}-{c} {d}:{e}:{f}.00000000"))
+    ds = ds.assign_coords(time=time_tmp2)
+    ds.coords["time"].attrs = attrs
+
+    return ds
+
+
+def generate_time_intervals(start_date, end_date):
+    # Initialize an empty list to store the intervals
+    intervals = []
+
+    # Loop over days
+    while start_date <= end_date:
+        # Loop over the four time intervals in a day
+        intervals.extend(
+            [start_date.strftime("%Y-%m-%d"), hour] for hour in ["00", "06", "12", "18"]
+        )
+        # Move to the next day
+        start_date += timedelta(days=1)
+
+    return intervals
+
+
+def _convert_target_unit(target_unit):
+    """Convert user-friendly unit to standard unit for internal calculations."""
+    if match := re.match(r"mm/(\d+)(h|d)", target_unit):
+        num, unit = match.groups()
+        return int(num), unit
+    return None, None
+
+
+def streamflow_unit_conv(streamflow, area, target_unit="mm/d", inverse=False):
+    """Convert the unit of streamflow data to mm/xx(time) for a basin or inverse.
+
+    Parameters
+    ----------
+    streamflow: xarray.Dataset, numpy.ndarray, pandas.DataFrame/Series
+        Streamflow data of each basin.
+    area: xarray.Dataset or pint.Quantity wrapping numpy.ndarray, pandas.DataFrame/Series
+        Area of each basin.
+    target_unit: str
+        The unit to convert to.
+    inverse: bool
+        If True, convert the unit to m^3/s.
+        If False, convert the unit to mm/day or mm/h.
+
+    Returns
+    -------
+    Converted data in the same type as the input streamflow.
+    """
+    # Convert the user input unit format
+    num, unit = _convert_target_unit(target_unit)
+    if unit:
+        if unit == "h":
+            standard_unit = "mm/h"
+            conversion_factor = num
+        elif unit == "d":
+            standard_unit = "mm/d"
+            conversion_factor = num
+        else:
+            raise ValueError(f"Unsupported unit: {unit}")
+    else:
+        standard_unit = target_unit
+        conversion_factor = 1
+    # Regular expression to match units with numbers
+    custom_unit_pattern = re.compile(r"mm/(\d+)(h|d)")
+
+    # Function to handle the conversion for numpy and pandas
+    def np_pd_conversion(streamflow, area, target_unit, inverse, conversion_factor):
+        if not inverse:
+            result = (streamflow / area).to(target_unit) * conversion_factor
+        else:
+            result = (streamflow * area).to(target_unit) / conversion_factor
+        return result.magnitude
+
+    # Handle xarray
+    if isinstance(streamflow, xr.Dataset) and isinstance(area, xr.Dataset):
+        streamflow_units = streamflow[list(streamflow.keys())[0]].attrs.get(
+            "units", None
+        )
+        if not inverse:
+            if not (
+                custom_unit_pattern.match(target_unit)
+                or re.match(r"mm/(?!\d)", target_unit)
+            ):
+                raise ValueError(
+                    "target_unit should be a valid unit like 'mm/d', 'mm/day', 'mm/h', 'mm/hour', 'mm/3h', 'mm/5d'"
+                )
+
+            q = streamflow.pint.quantify()
+            a = area.pint.quantify()
+            r = q[list(q.keys())[0]] / a[list(a.keys())[0]]
+            # result = r.pint.to(target_unit).to_dataset(name=list(q.keys())[0])
+            result = (r.pint.to(standard_unit) * conversion_factor).to_dataset(
+                name=list(q.keys())[0]
+            )
+            # Manually set the unit attribute to the custom unit
+            result_ = result.pint.dequantify()
+            result_[list(result_.keys())[0]].attrs["units"] = target_unit
+            return result_
+        else:
+            if streamflow_units:
+                if custom_match := custom_unit_pattern.match(streamflow_units):
+                    num, unit = custom_match.groups()
+                    if unit == "h":
+                        standard_unit = "mm/h"
+                        conversion_factor = int(num)
+                    elif unit == "d":
+                        standard_unit = "mm/d"
+                        conversion_factor = int(num)
+                    # Convert custom unit to standard unit
+                    r_ = streamflow / conversion_factor
+                    r_[list(r_.keys())[0]].attrs["units"] = standard_unit
+                    r = r_.pint.quantify()
+                else:
+                    r = streamflow.pint.quantify()
+            else:
+                r = streamflow.pint.quantify()
+            if target_unit not in ["m^3/s", "m3/s"]:
+                raise ValueError("target_unit should be 'm^3/s'")
+            a = area.pint.quantify()
+            q = r[list(r.keys())[0]] * a[list(a.keys())[0]]
+            result = q.pint.to(target_unit).to_dataset(name=list(r.keys())[0])
+            # dequantify to get normal xr_dataset
+            return result.pint.dequantify()
+
+    # Handle numpy and pandas
+    elif isinstance(streamflow, pint.Quantity) and isinstance(area, pint.Quantity):
+        if type(streamflow.magnitude) not in [np.ndarray, pd.DataFrame, pd.Series]:
+            raise TypeError(
+                "Input streamflow must be xarray.Dataset, or pint.Quantity wrapping numpy.ndarray, or pandas.DataFrame/Series"
+            )
+        if type(area.magnitude) != type(streamflow.magnitude):
+            raise TypeError("streamflow and area must be the same type")
+        return np_pd_conversion(
+            streamflow, area, standard_unit, inverse, conversion_factor
+        )
+
+    else:
+        raise TypeError(
+            "Input streamflow must be xarray.Dataset, or pint.Quantity wrapping numpy.ndarray, or pandas.DataFrame/Series"
+        )
```

### Comparing `hydrodatasource-0.0.1/hydrodatasource.egg-info/PKG-INFO` & `hydrodatasource-0.0.2/hydrodatasource.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,36 @@
-Metadata-Version: 2.1
-Name: hydrodatasource
-Version: 0.0.1
-Summary: A python project to deal with hydrological datasources
-Home-page: https://github.com/iHeadWater/hydrodatasource
-Author: Wenyu Ouyang
-Author-email: hust2014owen@gmail.com
-License: BSD license
-Keywords: hydrodatasource
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS.rst
-Requires-Dist: geopandas
-Requires-Dist: openpyxl~=3.1
-Requires-Dist: xlrd
-Requires-Dist: requests
-Requires-Dist: kerchunk
-Requires-Dist: cfgrib
-Requires-Dist: eccodes
-Requires-Dist: h5py
-Requires-Dist: wget
-Requires-Dist: chardet
-Requires-Dist: intake
-Requires-Dist: dataretrieval
-Requires-Dist: pygeohydro
-Requires-Dist: pykalman
-Requires-Dist: hydrodataset
+Metadata-Version: 2.1
+Name: hydrodatasource
+Version: 0.0.2
+Summary: A python project to deal with hydrological datasources
+Home-page: https://github.com/iHeadWater/hydrodatasource
+Author: Wenyu Ouyang
+Author-email: hust2014owen@gmail.com
+License: BSD license
+Keywords: hydrodatasource
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS.rst
+Requires-Dist: geopandas
+Requires-Dist: openpyxl~=3.1
+Requires-Dist: xlrd
+Requires-Dist: requests
+Requires-Dist: kerchunk
+Requires-Dist: cfgrib
+Requires-Dist: eccodes
+Requires-Dist: h5py
+Requires-Dist: wget
+Requires-Dist: chardet
+Requires-Dist: intake
+Requires-Dist: dataretrieval
+Requires-Dist: pygeohydro
+Requires-Dist: pykalman
+Requires-Dist: psycopg2-binary
+Requires-Dist: hydrodataset
```

### Comparing `hydrodatasource-0.0.1/tests/test_data_checker.py` & `hydrodatasource-0.0.2/tests/test_data_checker.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,110 +1,110 @@
-import os
-import pandas as pd
-
-from hydrodatasource.processor.data_checker import DataChecker
-
-
-def test_check_folder_structure():
-    """
-    Test to check if the folder structure in the local data path matches the expected format.
-    """
-    # Initialize the DataChecker with the local data path from the settings
-    data_checker = DataChecker()
-
-    # Check the folder structure
-    result = data_checker.check_folder_structure()
-
-    # Assert that the result is correct
-    assert result
-
-
-def test_check_file_format(tmpdir):
-    """
-    Test to check if the file format is correct.
-    """
-    # Initialize the DataChecker with the local data path from the settings
-    data_checker = DataChecker()
-
-    # Define a sample file path and expected columns
-    file_path = os.path.join(str(tmpdir), "file.csv")
-    expected_columns = ["column1", "column2", "column3"]
-
-    # Create a sample file with the expected columns
-    sample_data = pd.DataFrame(columns=expected_columns)
-    sample_data.to_csv(file_path, index=False)
-
-    # Check the file format
-    result = data_checker.check_file_format(file_path, expected_columns)
-
-    # Assert that the result is True
-    assert result
-
-    # Clean up the sample file
-    os.remove(file_path)
-
-
-def test_check_files_in_folder(tmpdir):
-    """
-    Test to check the format of all CSV files in a folder.
-    """
-    # Initialize the DataChecker with the local data path from the settings
-    data_checker = DataChecker()
-
-    # Define a sample folder path and expected columns
-    folder_path = str(tmpdir)
-    expected_columns = ["column1", "column2", "column3"]
-
-    # Create sample CSV files with the expected columns
-    file1_path = os.path.join(folder_path, "file1.csv")
-    file2_path = os.path.join(folder_path, "file2.csv")
-    file3_path = os.path.join(folder_path, "file3.csv")
-
-    sample_data = pd.DataFrame(columns=expected_columns)
-    sample_data.to_csv(file1_path, index=False)
-    sample_data.to_csv(file2_path, index=False)
-    sample_data.to_csv(file3_path, index=False)
-
-    # Check the file formats in the folder
-    result = data_checker.check_files_in_folder(folder_path, expected_columns)
-
-    # Assert that the result is True
-    assert result
-
-    # Clean up the sample files
-    os.remove(file1_path)
-    os.remove(file2_path)
-    os.remove(file3_path)
-
-
-def test_check_station_data_files(tmpdir):
-    """
-    Test to check the format of station data files.
-    """
-    # Initialize the DataChecker
-    data_checker = DataChecker()
-
-    # Define a sample folder path and expected columns
-    folder_path = tmpdir.mkdir("stations-origin")
-    expected_columns = {
-        "pp_stations": ["column1", "column2", "column3"],
-        "zz_stations": ["column4", "column5", "column6"],
-        "zq_stations": ["column7", "column8", "column9"],
-    }
-
-    # Create directories and sample files for each station type
-    for station_type in ["pp", "zz", "zq"]:
-        # Create station directories
-        station_dir = folder_path.mkdir(f"{station_type}_stations")
-        basic_info_file = station_dir.join(f"{station_type}_stations.csv")
-        time_series_file = station_dir.join("time_series.csv")
-
-        # Create a sample file with the expected columns
-        sample_data = pd.DataFrame(columns=expected_columns[f"{station_type}_stations"])
-        sample_data.to_csv(str(basic_info_file), index=False)
-        sample_data.to_csv(str(time_series_file), index=False)
-
-    # Check the format of station data files
-    result = data_checker.check_station_data_files()
-
-    # Assert that the result is True
-    assert result
+import os
+import pandas as pd
+
+from hydrodatasource.processor.data_checker import DataChecker
+
+
+def test_check_folder_structure():
+    """
+    Test to check if the folder structure in the local data path matches the expected format.
+    """
+    # Initialize the DataChecker with the local data path from the settings
+    data_checker = DataChecker()
+
+    # Check the folder structure
+    result = data_checker.check_folder_structure()
+
+    # Assert that the result is correct
+    assert result
+
+
+def test_check_file_format(tmpdir):
+    """
+    Test to check if the file format is correct.
+    """
+    # Initialize the DataChecker with the local data path from the settings
+    data_checker = DataChecker()
+
+    # Define a sample file path and expected columns
+    file_path = os.path.join(str(tmpdir), "file.csv")
+    expected_columns = ["column1", "column2", "column3"]
+
+    # Create a sample file with the expected columns
+    sample_data = pd.DataFrame(columns=expected_columns)
+    sample_data.to_csv(file_path, index=False)
+
+    # Check the file format
+    result = data_checker.check_file_format(file_path, expected_columns)
+
+    # Assert that the result is True
+    assert result
+
+    # Clean up the sample file
+    os.remove(file_path)
+
+
+def test_check_files_in_folder(tmpdir):
+    """
+    Test to check the format of all CSV files in a folder.
+    """
+    # Initialize the DataChecker with the local data path from the settings
+    data_checker = DataChecker()
+
+    # Define a sample folder path and expected columns
+    folder_path = str(tmpdir)
+    expected_columns = ["column1", "column2", "column3"]
+
+    # Create sample CSV files with the expected columns
+    file1_path = os.path.join(folder_path, "file1.csv")
+    file2_path = os.path.join(folder_path, "file2.csv")
+    file3_path = os.path.join(folder_path, "file3.csv")
+
+    sample_data = pd.DataFrame(columns=expected_columns)
+    sample_data.to_csv(file1_path, index=False)
+    sample_data.to_csv(file2_path, index=False)
+    sample_data.to_csv(file3_path, index=False)
+
+    # Check the file formats in the folder
+    result = data_checker.check_files_in_folder(folder_path, expected_columns)
+
+    # Assert that the result is True
+    assert result
+
+    # Clean up the sample files
+    os.remove(file1_path)
+    os.remove(file2_path)
+    os.remove(file3_path)
+
+
+def test_check_station_data_files(tmpdir):
+    """
+    Test to check the format of station data files.
+    """
+    # Initialize the DataChecker
+    data_checker = DataChecker()
+
+    # Define a sample folder path and expected columns
+    folder_path = tmpdir.mkdir("stations-origin")
+    expected_columns = {
+        "pp_stations": ["column1", "column2", "column3"],
+        "zz_stations": ["column4", "column5", "column6"],
+        "zq_stations": ["column7", "column8", "column9"],
+    }
+
+    # Create directories and sample files for each station type
+    for station_type in ["pp", "zz", "zq"]:
+        # Create station directories
+        station_dir = folder_path.mkdir(f"{station_type}_stations")
+        basic_info_file = station_dir.join(f"{station_type}_stations.csv")
+        time_series_file = station_dir.join("time_series.csv")
+
+        # Create a sample file with the expected columns
+        sample_data = pd.DataFrame(columns=expected_columns[f"{station_type}_stations"])
+        sample_data.to_csv(str(basic_info_file), index=False)
+        sample_data.to_csv(str(time_series_file), index=False)
+
+    # Check the format of station data files
+    result = data_checker.check_station_data_files()
+
+    # Assert that the result is True
+    assert result
```

### Comparing `hydrodatasource-0.0.1/tests/test_downloader.py` & `hydrodatasource-0.0.2/tests/test_downloader.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-"""
-Author: Wenyu Ouyang
-Date: 2023-10-13 20:50:01
-LastEditTime: 2024-03-28 08:42:28
-LastEditors: Wenyu Ouyang
-Description: Test downloading function
-FilePath: \hydrodata\tests\test_downloader.py
-Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
-"""
-import os
-import pandas as pd
-
-import hydrodataset as hds
-
-from hydrodatasource.downloader.hydrostation import (
-    catalogue_grdc,
-    download_grdc_month_data,
-    download_grdc_daily_data,
-    download_nwis_daily_flow,
-)
-
-
-def test_catalogue_grdc():
-    grdc_catalogue = catalogue_grdc(hds.CACHE_DIR)
-    assert isinstance(grdc_catalogue, pd.DataFrame)
-    assert grdc_catalogue.shape == (10707, 24)
-    assert "grdc_no" in grdc_catalogue.columns
-    assert "station" in grdc_catalogue.columns
-    assert "lat" in grdc_catalogue.columns
-    assert "long" in grdc_catalogue.columns
-    assert "d_start" in grdc_catalogue.columns
-    assert "d_end" in grdc_catalogue.columns
-    assert "d_yrs" in grdc_catalogue.columns
-    assert "m_start" in grdc_catalogue.columns
-    assert "m_end" in grdc_catalogue.columns
-    assert "m_yrs" in grdc_catalogue.columns
-    assert "t_start" in grdc_catalogue.columns
-    assert "t_end" in grdc_catalogue.columns
-    assert "t_yrs" in grdc_catalogue.columns
-    assert "area" in grdc_catalogue.columns
-    assert "altitude" in grdc_catalogue.columns
-    assert "r_volume_yr" in grdc_catalogue.columns
-    assert "r_height_yr" in grdc_catalogue.columns
-    assert "lta_discharge" in grdc_catalogue.columns
-    assert "d_miss" in grdc_catalogue.columns
-    assert "m_miss" in grdc_catalogue.columns
-    assert "wmo_reg" in grdc_catalogue.columns
-    assert "sub_reg" in grdc_catalogue.columns
-
-
-def test_download_grdc_ts(id="2181200"):
-    data = download_grdc_month_data(id, hds.CACHE_DIR)
-
-    # Check that the returned data is a dictionary
-    assert isinstance(data, dict)
-
-    # Check that the dictionary contains tables with river discharge data
-    assert all(isinstance(table, str) for table in data.values())
-
-
-def test_download_grdc_daily_data(tmp_path):
-    station_id = "12345"
-    file_path = download_grdc_daily_data(tmp_path, station_id)
-    assert os.path.exists(file_path) == False
-
-
-def test_download_usgs_streamflow():
-    camels = hds.Camels()
-    sites_id = camels.read_object_ids().tolist()
-    date_range = ("2020-10-01", "2021-10-01")
-    gage_dict = camels.camels_sites
-    save_dir = os.path.join("test_data", "camels_streamflow_2021")
-    unit = "cfs"
-    qobs = download_nwis_daily_flow(sites_id, date_range, gage_dict, save_dir, unit)
-    print(qobs)
+"""
+Author: Wenyu Ouyang
+Date: 2023-10-13 20:50:01
+LastEditTime: 2024-03-28 08:42:28
+LastEditors: Wenyu Ouyang
+Description: Test downloading function
+FilePath: \hydrodata\tests\test_downloader.py
+Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
+"""
+import os
+import pandas as pd
+
+import hydrodataset as hds
+
+from hydrodatasource.downloader.hydrostation import (
+    catalogue_grdc,
+    download_grdc_month_data,
+    download_grdc_daily_data,
+    download_nwis_daily_flow,
+)
+
+
+def test_catalogue_grdc():
+    grdc_catalogue = catalogue_grdc(hds.CACHE_DIR)
+    assert isinstance(grdc_catalogue, pd.DataFrame)
+    assert grdc_catalogue.shape == (10707, 24)
+    assert "grdc_no" in grdc_catalogue.columns
+    assert "station" in grdc_catalogue.columns
+    assert "lat" in grdc_catalogue.columns
+    assert "long" in grdc_catalogue.columns
+    assert "d_start" in grdc_catalogue.columns
+    assert "d_end" in grdc_catalogue.columns
+    assert "d_yrs" in grdc_catalogue.columns
+    assert "m_start" in grdc_catalogue.columns
+    assert "m_end" in grdc_catalogue.columns
+    assert "m_yrs" in grdc_catalogue.columns
+    assert "t_start" in grdc_catalogue.columns
+    assert "t_end" in grdc_catalogue.columns
+    assert "t_yrs" in grdc_catalogue.columns
+    assert "area" in grdc_catalogue.columns
+    assert "altitude" in grdc_catalogue.columns
+    assert "r_volume_yr" in grdc_catalogue.columns
+    assert "r_height_yr" in grdc_catalogue.columns
+    assert "lta_discharge" in grdc_catalogue.columns
+    assert "d_miss" in grdc_catalogue.columns
+    assert "m_miss" in grdc_catalogue.columns
+    assert "wmo_reg" in grdc_catalogue.columns
+    assert "sub_reg" in grdc_catalogue.columns
+
+
+def test_download_grdc_ts(id="2181200"):
+    data = download_grdc_month_data(id, hds.CACHE_DIR)
+
+    # Check that the returned data is a dictionary
+    assert isinstance(data, dict)
+
+    # Check that the dictionary contains tables with river discharge data
+    assert all(isinstance(table, str) for table in data.values())
+
+
+def test_download_grdc_daily_data(tmp_path):
+    station_id = "12345"
+    file_path = download_grdc_daily_data(tmp_path, station_id)
+    assert os.path.exists(file_path) == False
+
+
+def test_download_usgs_streamflow():
+    camels = hds.Camels()
+    sites_id = camels.read_object_ids().tolist()
+    date_range = ("2020-10-01", "2021-10-01")
+    gage_dict = camels.camels_sites
+    save_dir = os.path.join("test_data", "camels_streamflow_2021")
+    unit = "cfs"
+    qobs = download_nwis_daily_flow(sites_id, date_range, gage_dict, save_dir, unit)
+    print(qobs)
```

### Comparing `hydrodatasource-0.0.1/tests/test_process_inq.py` & `hydrodatasource-0.0.2/tests/test_process_inq.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-"""
-Author: Tianxu Liu
-Date: 2024-03-16 15:55:22
-LastEditTime: 2024-03-28 08:41:34
-LastEditors: Wenyu Ouyang
-Description: test process inq
-FilePath: \hydrodata\tests\test_process_inq.py
-Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
-"""
-import pytest
-from hydrodatasource.cleaner.smooth_inq import Cleaner
-
-
-@pytest.fixture
-def cleaner():
-    cleaner = Cleaner(
-        file_path="/home/liutianxv/sample_data.csv",
-        column_id="ID",
-        ID_list=None,
-        column_flow="INQ",
-        column_time="TM",
-        start_time=None,
-        end_time=None,
-        preprocess=True,
-        method="kalman",
-        save_path="/home/liutianxv/sample_data.csv",
-        plot=True,
-        window_size=20,
-        cutoff_frequency=0.035,
-        iterations=3,
-        sampling_rate=1.0,
-        time_step=1,
-        order=5,
-        cwt_row=10,
-    )
-    return cleaner
-
-
-def test_process_inq(cleaner):
-    cleaner.process_inq()
+"""
+Author: Tianxu Liu
+Date: 2024-03-16 15:55:22
+LastEditTime: 2024-03-28 08:41:34
+LastEditors: Wenyu Ouyang
+Description: test process inq
+FilePath: \hydrodata\tests\test_process_inq.py
+Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
+"""
+import pytest
+from hydrodatasource.cleaner.smooth_inq import Cleaner
+
+
+@pytest.fixture
+def cleaner():
+    cleaner = Cleaner(
+        file_path="/home/liutianxv/sample_data.csv",
+        column_id="ID",
+        ID_list=None,
+        column_flow="INQ",
+        column_time="TM",
+        start_time=None,
+        end_time=None,
+        preprocess=True,
+        method="kalman",
+        save_path="/home/liutianxv/sample_data.csv",
+        plot=True,
+        window_size=20,
+        cutoff_frequency=0.035,
+        iterations=3,
+        sampling_rate=1.0,
+        time_step=1,
+        order=5,
+        cwt_row=10,
+    )
+    return cleaner
+
+
+def test_process_inq(cleaner):
+    cleaner.process_inq()
```

### Comparing `hydrodatasource-0.0.1/tests/test_processor.py` & `hydrodatasource-0.0.2/tests/test_processor.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-"""
-Author: Wenyu Ouyang
-Date: 2023-10-28 08:28:37
-LastEditTime: 2024-03-28 08:41:56
-LastEditors: Wenyu Ouyang
-Description: Test funcs for processor
-FilePath: \hydrodata\tests\test_processor.py
-Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
-"""
-
-import os
-import geopandas as gpd
-from hydrodatasource.processor.minio_process import GeoProcessor, geojson_to_shp
-
-
-def test_geojson_to_shp(tmp_path):
-    # create a temporary GeoJSON file
-    input_geojson = os.path.join(tmp_path, "test.geojson")
-    points = gpd.points_from_xy([0, 1], [0, 1])
-    gdf = gpd.GeoDataFrame({"col1": [1, 2], "geometry": points})
-    gdf.to_file(input_geojson, driver="GeoJSON")
-
-    # call the function with the temporary GeoJSON file
-    output_folder = os.path.join(tmp_path, "shp_output")
-    geojson_to_shp(input_geojson, output_folder=output_folder)
-
-    # check that the Shapefile was created
-    assert os.path.exists(os.path.join(output_folder, "test.shp"))
-
-    # check that the ZIP file was created
-    assert os.path.exists(os.path.join(tmp_path, "test.zip"))
-
-
-def test_upload_and_read_shp(tmp_path, minio_paras):
-    # create a temporary GeoJSON file
-    input_geojson = os.path.join(tmp_path, "test.geojson")
-    points = gpd.points_from_xy([0, 1], [0, 1])
-    gdf = gpd.GeoDataFrame({"col1": [1, 2], "geometry": points})
-    gdf.to_file(input_geojson, driver="GeoJSON")
-    geo_processor = GeoProcessor(minio_paras)
-    geo_processor.upload_geojson(gj_local_path=input_geojson, gj_mo_name="test.geojson")
-    gdf_rd = geo_processor.read_shp("test.zip")
-    assert gdf_rd.equals(gdf)
+"""
+Author: Wenyu Ouyang
+Date: 2023-10-28 08:28:37
+LastEditTime: 2024-03-28 08:41:56
+LastEditors: Wenyu Ouyang
+Description: Test funcs for processor
+FilePath: \hydrodata\tests\test_processor.py
+Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
+"""
+
+import os
+import geopandas as gpd
+from hydrodatasource.processor.minio_process import GeoProcessor, geojson_to_shp
+
+
+def test_geojson_to_shp(tmp_path):
+    # create a temporary GeoJSON file
+    input_geojson = os.path.join(tmp_path, "test.geojson")
+    points = gpd.points_from_xy([0, 1], [0, 1])
+    gdf = gpd.GeoDataFrame({"col1": [1, 2], "geometry": points})
+    gdf.to_file(input_geojson, driver="GeoJSON")
+
+    # call the function with the temporary GeoJSON file
+    output_folder = os.path.join(tmp_path, "shp_output")
+    geojson_to_shp(input_geojson, output_folder=output_folder)
+
+    # check that the Shapefile was created
+    assert os.path.exists(os.path.join(output_folder, "test.shp"))
+
+    # check that the ZIP file was created
+    assert os.path.exists(os.path.join(tmp_path, "test.zip"))
+
+
+def test_upload_and_read_shp(tmp_path, minio_paras):
+    # create a temporary GeoJSON file
+    input_geojson = os.path.join(tmp_path, "test.geojson")
+    points = gpd.points_from_xy([0, 1], [0, 1])
+    gdf = gpd.GeoDataFrame({"col1": [1, 2], "geometry": points})
+    gdf.to_file(input_geojson, driver="GeoJSON")
+    geo_processor = GeoProcessor(minio_paras)
+    geo_processor.upload_geojson(gj_local_path=input_geojson, gj_mo_name="test.geojson")
+    gdf_rd = geo_processor.read_shp("test.zip")
+    assert gdf_rd.equals(gdf)
```

### Comparing `hydrodatasource-0.0.1/tests/test_reader.py` & `hydrodatasource-0.0.2/tests/test_reader.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,123 +1,123 @@
-"""
-Author: Wenyu Ouyang
-Date: 2023-11-01 08:58:50
-LastEditTime: 2024-03-28 08:40:38
-LastEditors: Wenyu Ouyang
-Description: Test funcs for reader.py
-FilePath: \hydrodata\tests\test_reader.py
-Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
-"""
-
-import os
-from minio import Minio
-import hydrodataset as hds
-
-from hydrodatasource.configs.config import LOCAL_DATA_PATH
-from hydrodatasource.reader.grdc import GRDCDataHandler
-from hydrodatasource.reader.reader import (
-    AOI,
-    DataHandler,
-    LocalFileReader,
-    MinioFileReader,
-)
-
-
-def test_gpm_read_minio():
-    data_handler = DataHandler(
-        aoi_type="basin",  # only basin for now, the streamflow data needs to be reorganized in the minio server,  then to be read.
-        aoi_param="86_21401550",
-        dataname="gpm",
-        minio_read=True,
-    )
-    data = data_handler.handle()
-    assert data is not None
-    return data
-
-
-def test_gfs_read_minio():
-    data_handler = DataHandler(
-        aoi_type="basin", aoi_param="86_21401550", dataname="gfs", minio_read=True
-    )
-    data = data_handler.handle()
-    assert data is not None
-    return data
-
-
-def test_gpm_gfs_read_minio():
-    data_handler = DataHandler(
-        aoi_type="basin", aoi_param="86_21401550", dataname="gpm_gfs", minio_read=True
-    )
-    data = data_handler.handle()
-    assert data is not None
-    return data
-
-
-def test_gpm_read_with_process():
-    # if there is no data in minio, we want to merge a new one and save in local_data_path
-    data_handler = DataHandler(
-        aoi_type="basin",
-        aoi_param="86_21401550",
-        region="wis",
-        time_periods=[["2017-01-01T00:00:00", "2017-01-31T00:00:00"]],
-        dataname="gpm",
-        minio_read=False,
-        local_save=True,
-    )
-    data = data_handler.handle()
-    assert data is not None
-    return data
-
-
-# The new method no longer needs ways below, but I keep them in case we need it.
-
-# def test_reader_interface(minio_paras):
-#     # 初始化Minio客户端
-#     minio_server = minio_paras["endpoint_url"]
-#     minio_client = Minio(
-#         minio_server.replace("http://", ""),
-#         access_key=minio_paras["access_key"],
-#         secret_key=minio_paras["secret_key"],
-#         secure=False,
-#     )
-
-#     gpm_handler = GPMDataHandler()
-#     gfs_handler = GFSDataHandler()
-#     aoi = AOI("grid", {"lat": 0, "lon": 0, "size": 1})
-
-#     local_gpm_reader = LocalFileReader(gpm_handler)
-#     local_gfs_reader = LocalFileReader(gfs_handler)
-#     local_gpm_reader.read("path/to/file", aoi)
-
-#     # Assume you have initialized the minio_client somewhere
-#     minio_gpm_reader = MinioFileReader(minio_client, gpm_handler)
-#     minio_gfs_reader = MinioFileReader(minio_client, gfs_handler)
-#     minio_gpm_reader.read("path/to/file", aoi)
-
-
-# def test_reader_grdc():
-#     grdc_handler = GRDCDataHandler()
-#     aoi = AOI(
-#         "station",
-#         {"station_id": "2181200", "start_time": "1980-01-01", "end_time": "2001-01-01"},
-#     )
-
-#     local_grdc_reader = LocalFileReader(grdc_handler)
-#     grdc_data = local_grdc_reader.read(
-#         os.path.join(hds.CACHE_DIR.joinpath("grdc_daily_data"), "grdc_daily_data.nc"),
-#         aoi,
-#     )
-
-
-# def test_reader_station():
-#     station_handler = StationDataHandler()
-#     aoi = AOI(
-#         "station",
-#         {"station_id": "2181200", "start_time": "1980-01-01", "end_time": "2001-01-01"},
-#     )
-
-#     local_station_reader = LocalFileReader(station_handler)
-#     data = local_station_reader.read(
-#         os.path.join(LOCAL_DATA_PATH, "station.nc"),
-#         aoi,
-#     )
-#     print(data)
+"""
+Author: Wenyu Ouyang
+Date: 2023-11-01 08:58:50
+LastEditTime: 2024-03-28 08:40:38
+LastEditors: Wenyu Ouyang
+Description: Test funcs for reader.py
+FilePath: \hydrodata\tests\test_reader.py
+Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
+"""
+
+import os
+from minio import Minio
+import hydrodataset as hds
+
+from hydrodatasource.configs.config import LOCAL_DATA_PATH
+from hydrodatasource.reader.grdc import GRDCDataHandler
+from hydrodatasource.reader.reader import (
+    AOI,
+    DataHandler,
+    LocalFileReader,
+    MinioFileReader,
+)
+
+
+def test_gpm_read_minio():
+    data_handler = DataHandler(
+        aoi_type="basin",  # only basin for now, the streamflow data needs to be reorganized in the minio server,  then to be read.
+        aoi_param="86_21401550",
+        dataname="gpm",
+        minio_read=True,
+    )
+    data = data_handler.handle()
+    assert data is not None
+    return data
+
+
+def test_gfs_read_minio():
+    data_handler = DataHandler(
+        aoi_type="basin", aoi_param="86_21401550", dataname="gfs", minio_read=True
+    )
+    data = data_handler.handle()
+    assert data is not None
+    return data
+
+
+def test_gpm_gfs_read_minio():
+    data_handler = DataHandler(
+        aoi_type="basin", aoi_param="86_21401550", dataname="gpm_gfs", minio_read=True
+    )
+    data = data_handler.handle()
+    assert data is not None
+    return data
+
+
+def test_gpm_read_with_process():
+    # if there is no data in minio, we want to merge a new one and save in local_data_path
+    data_handler = DataHandler(
+        aoi_type="basin",
+        aoi_param="86_21401550",
+        region="wis",
+        time_periods=[["2017-01-01T00:00:00", "2017-01-31T00:00:00"]],
+        dataname="gpm",
+        minio_read=False,
+        local_save=True,
+    )
+    data = data_handler.handle()
+    assert data is not None
+    return data
+
+
+# The new method no longer needs ways below, but I keep them in case we need it.
+
+# def test_reader_interface(minio_paras):
+#     # 初始化Minio客户端
+#     minio_server = minio_paras["endpoint_url"]
+#     minio_client = Minio(
+#         minio_server.replace("http://", ""),
+#         access_key=minio_paras["access_key"],
+#         secret_key=minio_paras["secret_key"],
+#         secure=False,
+#     )
+
+#     gpm_handler = GPMDataHandler()
+#     gfs_handler = GFSDataHandler()
+#     aoi = AOI("grid", {"lat": 0, "lon": 0, "size": 1})
+
+#     local_gpm_reader = LocalFileReader(gpm_handler)
+#     local_gfs_reader = LocalFileReader(gfs_handler)
+#     local_gpm_reader.read("path/to/file", aoi)
+
+#     # Assume you have initialized the minio_client somewhere
+#     minio_gpm_reader = MinioFileReader(minio_client, gpm_handler)
+#     minio_gfs_reader = MinioFileReader(minio_client, gfs_handler)
+#     minio_gpm_reader.read("path/to/file", aoi)
+
+
+# def test_reader_grdc():
+#     grdc_handler = GRDCDataHandler()
+#     aoi = AOI(
+#         "station",
+#         {"station_id": "2181200", "start_time": "1980-01-01", "end_time": "2001-01-01"},
+#     )
+
+#     local_grdc_reader = LocalFileReader(grdc_handler)
+#     grdc_data = local_grdc_reader.read(
+#         os.path.join(hds.CACHE_DIR.joinpath("grdc_daily_data"), "grdc_daily_data.nc"),
+#         aoi,
+#     )
+
+
+# def test_reader_station():
+#     station_handler = StationDataHandler()
+#     aoi = AOI(
+#         "station",
+#         {"station_id": "2181200", "start_time": "1980-01-01", "end_time": "2001-01-01"},
+#     )
+
+#     local_station_reader = LocalFileReader(station_handler)
+#     data = local_station_reader.read(
+#         os.path.join(LOCAL_DATA_PATH, "station.nc"),
+#         aoi,
+#     )
+#     print(data)
```

### Comparing `hydrodatasource-0.0.1/tests/test_reader_basins.py` & `hydrodatasource-0.0.2/tests/test_reader_basins.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-#!/usr/bin/env python
-"""
-Author: Wenyu Ouyang
-Date: 2023-10-25 15:16:21
-LastEditTime: 2024-03-28 08:40:25
-LastEditors: Wenyu Ouyang
-Description: Tests for reading basins' data
-FilePath: \hydrodata\tests\test_reader_basins.py
-Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
-"""
-import os.path
-import pathlib
-
-from hydrodatasource.reader import stations
-from hydrodatasource.configs import config
-from hydrodatasource.reader import minio_api
-
-
-def test_content():
-    # preprocess.huanren_preprocess()
-    stations.biliu_stbprp_decode()
-
-
-def test_upload_csv():
-    test_path = pathlib.Path(os.path.abspath(os.path.curdir)).parent
-    client = config.MC
-    bucket_name = config.MINIO_PARAM["bucket_path"]
-    minio_api.boto3_upload_csv(
-        client,
-        bucket_name,
-        "nyc_taxi",
-        os.path.join(test_path, "test_data/nyc_taxi.csv"),
-    )
-    minio_api.minio_upload_csv(
-        client,
-        bucket_name,
-        "driver_data_site24",
-        os.path.join(test_path, "test_data/driver_data_site24.csv"),
-    )
-
-
-def test_download_csv_minio():
-    client = config.S3
-    bucket_name = config.MINIO_PARAM["bucket_path"]
-    # minio_api.minio_download_csv(client, bucket_name, 'nyc_taxi', file_path='test_dload')
-    minio_api.boto3_download_csv(
-        client, bucket_name, "driver_data_site24", "driver_data_site24.csv"
-    )
+#!/usr/bin/env python
+"""
+Author: Wenyu Ouyang
+Date: 2023-10-25 15:16:21
+LastEditTime: 2024-03-28 08:40:25
+LastEditors: Wenyu Ouyang
+Description: Tests for reading basins' data
+FilePath: \hydrodata\tests\test_reader_basins.py
+Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
+"""
+import os.path
+import pathlib
+
+from hydrodatasource.reader import stations
+from hydrodatasource.configs import config
+from hydrodatasource.reader import minio_api
+
+
+def test_content():
+    # preprocess.huanren_preprocess()
+    stations.biliu_stbprp_decode()
+
+
+def test_upload_csv():
+    test_path = pathlib.Path(os.path.abspath(os.path.curdir)).parent
+    client = config.MC
+    bucket_name = config.MINIO_PARAM["bucket_path"]
+    minio_api.boto3_upload_csv(
+        client,
+        bucket_name,
+        "nyc_taxi",
+        os.path.join(test_path, "test_data/nyc_taxi.csv"),
+    )
+    minio_api.minio_upload_csv(
+        client,
+        bucket_name,
+        "driver_data_site24",
+        os.path.join(test_path, "test_data/driver_data_site24.csv"),
+    )
+
+
+def test_download_csv_minio():
+    client = config.S3
+    bucket_name = config.MINIO_PARAM["bucket_path"]
+    # minio_api.minio_download_csv(client, bucket_name, 'nyc_taxi', file_path='test_dload')
+    minio_api.boto3_download_csv(
+        client, bucket_name, "driver_data_site24", "driver_data_site24.csv"
+    )
```

### Comparing `hydrodatasource-0.0.1/tests/test_reader_stations.py` & `hydrodatasource-0.0.2/tests/test_reader_stations.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-"""
-Author: Wenyu Ouyang
-Date: 2023-10-31 20:56:23
-LastEditTime: 2024-03-28 08:39:15
-LastEditors: Wenyu Ouyang
-Description: Test funcs for reading stations' data
-FilePath: \hydrodata\tests\test_reader_stations.py
-Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
-"""
-
-import os
-import pandas as pd
-
-from hydrodatasource.reader.stations import huanren_preprocess
-
-
-def test_huanren_preprocess(tmp_path):
-    # create a temporary directory for testing
-    test_dir = tmp_path / "test_data"
-    test_dir.mkdir()
-
-    # create a test excel file
-    test_file = test_dir / "test_file.xlsx"
-    test_data = pd.DataFrame(
-        {"date": ["2022-01-01", "2022-01-02", "2022-01-03"], "flow": [1.0, 2.0, 3.0]}
-    )
-    test_data.to_excel(test_file, index=False)
-
-    # set up local data path and run function
-    os.environ["LOCAL_DATA_PATH"] = str(test_dir)
-    huanren_preprocess()
-
-    # check that the output file was created and has the correct data
-    output_file = test_dir / "huanren" / "tidy.csv"
-    assert output_file.exists()
-    output_data = pd.read_csv(output_file)
-    assert output_data.equals(test_data)
+"""
+Author: Wenyu Ouyang
+Date: 2023-10-31 20:56:23
+LastEditTime: 2024-03-28 08:39:15
+LastEditors: Wenyu Ouyang
+Description: Test funcs for reading stations' data
+FilePath: \hydrodata\tests\test_reader_stations.py
+Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
+"""
+
+import os
+import pandas as pd
+
+from hydrodatasource.reader.stations import huanren_preprocess
+
+
+def test_huanren_preprocess(tmp_path):
+    # create a temporary directory for testing
+    test_dir = tmp_path / "test_data"
+    test_dir.mkdir()
+
+    # create a test excel file
+    test_file = test_dir / "test_file.xlsx"
+    test_data = pd.DataFrame(
+        {"date": ["2022-01-01", "2022-01-02", "2022-01-03"], "flow": [1.0, 2.0, 3.0]}
+    )
+    test_data.to_excel(test_file, index=False)
+
+    # set up local data path and run function
+    os.environ["LOCAL_DATA_PATH"] = str(test_dir)
+    huanren_preprocess()
+
+    # check that the output file was created and has the correct data
+    output_file = test_dir / "huanren" / "tidy.csv"
+    assert output_file.exists()
+    output_data = pd.read_csv(output_file)
+    assert output_data.equals(test_data)
```

### Comparing `hydrodatasource-0.0.1/tests/test_rr_event_iden.py` & `hydrodatasource-0.0.2/tests/test_rr_event_iden.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-"""
-Author: Yang Wang, Jingyi Wang, and Wenyu Ouyang
-Date: 2023-10-28 09:23:22
-LastEditTime: 2024-03-28 08:40:17
-LastEditors: Wenyu Ouyang
-Description: Test for rainfall-runoff event identification
-FilePath: \hydrodata\tests\test_rr_event_iden.py
-Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
-"""
-
-import os
-import numpy as np
-from pint import UnitRegistry
-
-from hydrodataset import Camels
-
-from hydrodatasource.configs.config import SETTING
-from hydrodatasource.cleaner.dmca_esr import rainfall_runoff_event_identify
-from hydrodatasource.utils.utils import streamflow_unit_conv
-
-
-def test_rainfall_runoff_event_identify():
-    camels = Camels(
-        os.path.join(
-            SETTING["local_data_path"]["datasets-origin"], "camels", "camels_us"
-        )
-    )
-    gage_ids = camels.read_object_ids()
-    ureg = UnitRegistry()
-
-    rain = camels.read_ts_xrdataset(
-        gage_ids[:1], ["1980-01-01", "2015-01-01"], var_lst=["prcp"]
-    )
-    flow = camels.read_ts_xrdataset(
-        gage_ids[:1], ["1980-01-01", "2015-01-01"], var_lst=["streamflow"]
-    )
-    # trans unit to mm/day
-    basin_area = camels.read_area(gage_ids[:1])
-    r_mmd = streamflow_unit_conv(flow, basin_area)
-    flow_threshold = streamflow_unit_conv(
-        np.array([100]) * ureg.m**3 / ureg.s,
-        basin_area.isel(basin=0).to_array().to_numpy() * ureg.km**2,
-        target_unit="mm/h",
-    )
-    flood_events = rainfall_runoff_event_identify(
-        rain["prcp"].isel(basin=0).to_series(),
-        r_mmd["streamflow"].isel(basin=0).to_series(),
-        flow_threshold=flow_threshold[0],
-    )
-    assert flood_events["BEGINNING_RAIN"].shape[0] == flood_events["END_RAIN"].shape[0]
+"""
+Author: Yang Wang, Jingyi Wang, and Wenyu Ouyang
+Date: 2023-10-28 09:23:22
+LastEditTime: 2024-03-28 08:40:17
+LastEditors: Wenyu Ouyang
+Description: Test for rainfall-runoff event identification
+FilePath: \hydrodata\tests\test_rr_event_iden.py
+Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
+"""
+
+import os
+import numpy as np
+from pint import UnitRegistry
+
+from hydrodataset import Camels
+
+from hydrodatasource.configs.config import SETTING
+from hydrodatasource.cleaner.dmca_esr import rainfall_runoff_event_identify
+from hydrodatasource.utils.utils import streamflow_unit_conv
+
+
+def test_rainfall_runoff_event_identify():
+    camels = Camels(
+        os.path.join(
+            SETTING["local_data_path"]["datasets-origin"], "camels", "camels_us"
+        )
+    )
+    gage_ids = camels.read_object_ids()
+    ureg = UnitRegistry()
+
+    rain = camels.read_ts_xrdataset(
+        gage_ids[:1], ["1980-01-01", "2015-01-01"], var_lst=["prcp"]
+    )
+    flow = camels.read_ts_xrdataset(
+        gage_ids[:1], ["1980-01-01", "2015-01-01"], var_lst=["streamflow"]
+    )
+    # trans unit to mm/day
+    basin_area = camels.read_area(gage_ids[:1])
+    r_mmd = streamflow_unit_conv(flow, basin_area)
+    flow_threshold = streamflow_unit_conv(
+        np.array([100]) * ureg.m**3 / ureg.s,
+        basin_area.isel(basin=0).to_array().to_numpy() * ureg.km**2,
+        target_unit="mm/h",
+    )
+    flood_events = rainfall_runoff_event_identify(
+        rain["prcp"].isel(basin=0).to_series(),
+        r_mmd["streamflow"].isel(basin=0).to_series(),
+        flow_threshold=flow_threshold[0],
+    )
+    assert flood_events["BEGINNING_RAIN"].shape[0] == flood_events["END_RAIN"].shape[0]
```

