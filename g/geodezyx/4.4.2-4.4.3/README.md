# Comparing `tmp/geodezyx-4.4.2.tar.gz` & `tmp/geodezyx-4.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geodezyx-4.4.2.tar", last modified: Wed Apr 17 15:45:23 2024, max compression
+gzip compressed data, was "geodezyx-4.4.3.tar", last modified: Mon May 20 15:26:02 2024, max compression
```

## Comparing `geodezyx-4.4.2.tar` & `geodezyx-4.4.3.tar`

### file list

```diff
@@ -1,117 +1,118 @@
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-04-17 15:45:23.930724 geodezyx-4.4.2/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7652 2024-02-08 10:49:07.000000 geodezyx-4.4.2/LICENSE
--rw-r--r--   0 psakicki  (1000) psakicki  (1000)     2197 2024-04-17 15:45:23.930724 geodezyx-4.4.2/PKG-INFO
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     6655 2024-04-17 15:03:14.000000 geodezyx-4.4.2/README.md
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-04-17 15:45:23.906724 geodezyx-4.4.2/geodezyx/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     2350 2024-04-17 14:12:11.000000 geodezyx-4.4.2/geodezyx/__init__.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-04-17 15:45:23.906724 geodezyx-4.4.2/geodezyx/athmo/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       21 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/athmo/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    30501 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/athmo/athmo.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-04-17 15:45:23.910724 geodezyx-4.4.2/geodezyx/conv/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      344 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/conv/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     9545 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/conv/conv_angle.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    23341 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/conv/conv_coords.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     9504 2024-04-17 14:04:02.000000 geodezyx-4.4.2/geodezyx/conv/conv_geometric.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     5908 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/conv/conv_interpolators.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     3876 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/conv/conv_proj_lambert.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     6572 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/conv/conv_proj_utm.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    10474 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/conv/conv_rinex.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    12023 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/conv/conv_rotation_matrices.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    80367 2024-04-17 14:04:02.000000 geodezyx-4.4.2/geodezyx/conv/conv_time.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-04-17 15:45:23.910724 geodezyx-4.4.2/geodezyx/externlib/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     1339 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/externlib/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      797 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/externlib/externlib.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-04-17 15:45:23.914724 geodezyx-4.4.2/geodezyx/files_rw/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      595 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/files_rw/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    81708 2024-04-17 14:04:02.000000 geodezyx-4.4.2/geodezyx/files_rw/geo_files_converter_lib.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     9417 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/files_rw/read_athmo.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     4812 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/files_rw/read_coords_misc.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    79500 2024-04-17 14:04:02.000000 geodezyx-4.4.2/geodezyx/files_rw/read_coords_time_series.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    19068 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/files_rw/read_eop.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    28653 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/files_rw/read_geo_files_misc.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    17067 2024-04-17 14:04:02.000000 geodezyx-4.4.2/geodezyx/files_rw/read_gnss_prods.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7241 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/files_rw/read_gnss_qc.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     8729 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/files_rw/read_igs_combi.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    18109 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/files_rw/read_logsheets.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    14652 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/files_rw/read_rinex.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     2825 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/files_rw/read_slr.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    37758 2024-04-17 14:12:11.000000 geodezyx-4.4.2/geodezyx/files_rw/write_geo_files.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     6422 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/files_rw/write_rinex.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-04-17 15:45:23.914724 geodezyx-4.4.2/geodezyx/geodyn/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      136 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/geodyn/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    10131 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/geodyn/emsgfz_load_interp.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    13584 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/geodyn/euler_pole_calc.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    27563 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/geodyn/velo_field_map_plt.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     6087 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/geodyn/volcano_mogi.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-04-17 15:45:23.914724 geodezyx-4.4.2/geodezyx/logconfig/
--rwxrwxr-x   0 psakicki  (1000) psakicki  (1000)       80 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/logconfig/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     2329 2024-04-17 14:12:11.000000 geodezyx-4.4.2/geodezyx/logconfig/loggzyx.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-04-17 15:45:23.914724 geodezyx-4.4.2/geodezyx/marine/
--rwxrwxr-x   0 psakicki  (1000) psakicki  (1000)      119 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/marine/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     2575 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/marine/marine.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     9675 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/marine/obp.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    30838 2024-04-17 14:04:02.000000 geodezyx-4.4.2/geodezyx/marine/obscom.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-04-17 15:45:23.918724 geodezyx-4.4.2/geodezyx/megalib/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      153 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/megalib/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      139 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/megalib/genefun.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      295 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/megalib/geo_files_converter_lib.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      571 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/megalib/geoclass.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      334 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/megalib/geodetik.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      408 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/megalib/megalib.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      720 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/megalib/softs_runner.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-04-17 15:45:23.922724 geodezyx-4.4.2/geodezyx/operational/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      672 2024-04-17 14:04:02.000000 geodezyx-4.4.2/geodezyx/operational/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    10790 2024-04-17 14:04:02.000000 geodezyx-4.4.2/geodezyx/operational/anubis_frontend.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7433 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/operational/cluster_gfz.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7006 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/operational/download_cddis.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7150 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/operational/download_dropbox.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    14599 2024-04-17 14:04:02.000000 geodezyx-4.4.2/geodezyx/operational/download_find_files.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    34383 2024-04-17 14:12:11.000000 geodezyx-4.4.2/geodezyx/operational/download_prods.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    20363 2024-04-17 14:04:02.000000 geodezyx-4.4.2/geodezyx/operational/download_rinex.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    13921 2024-04-17 14:04:02.000000 geodezyx-4.4.2/geodezyx/operational/download_utils.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    79416 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/operational/gins_runner.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    26851 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/operational/groops_frontend.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    15751 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/operational/hector_frontend.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7915 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/operational/midas_frontend.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    14061 2024-04-17 14:04:02.000000 geodezyx-4.4.2/geodezyx/operational/pride_pppar_frontend.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    26025 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/operational/rinex_lister_plotter.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    32108 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/operational/rinex_utils.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7041 2024-04-17 14:04:02.000000 geodezyx-4.4.2/geodezyx/operational/rtklib_frontend.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     9145 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/operational/track_frontend.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-04-17 15:45:23.922724 geodezyx-4.4.2/geodezyx/reffram/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      107 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/reffram/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    43896 2024-04-17 14:04:02.000000 geodezyx-4.4.2/geodezyx/reffram/geometry.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    63732 2024-04-17 14:04:02.000000 geodezyx-4.4.2/geodezyx/reffram/gnss_products.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    11346 2024-04-17 14:04:02.000000 geodezyx-4.4.2/geodezyx/reffram/kepler_gzyx.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     3864 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/reffram/quaternions.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-04-17 15:45:23.922724 geodezyx-4.4.2/geodezyx/stats/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       50 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/stats/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    30945 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/stats/least_squares.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    44079 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/stats/stats.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-04-17 15:45:23.926724 geodezyx-4.4.2/geodezyx/time_series/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       97 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/time_series/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    48885 2024-04-17 14:04:02.000000 geodezyx-4.4.2/geodezyx/time_series/ts_class.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    17296 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/time_series/ts_export.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    39108 2024-04-17 14:04:02.000000 geodezyx-4.4.2/geodezyx/time_series/ts_fcts.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-04-17 15:45:23.926724 geodezyx-4.4.2/geodezyx/toolbox_meta/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       96 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/toolbox_meta/__init__.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-04-17 15:45:23.926724 geodezyx-4.4.2/geodezyx/utils/
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      242 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/utils/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     2011 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/utils/dict_utils.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    13503 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/utils/list_utils.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     3622 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/utils/pandas_utils.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7245 2024-02-08 10:49:07.000000 geodezyx-4.4.2/geodezyx/utils/plot_utils.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    18458 2024-04-17 14:04:02.000000 geodezyx-4.4.2/geodezyx/utils/shell_like.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    25869 2024-04-17 14:12:11.000000 geodezyx-4.4.2/geodezyx/utils/utils_core.py
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-04-17 15:45:23.926724 geodezyx-4.4.2/geodezyx.egg-info/
--rw-r--r--   0 psakicki  (1000) psakicki  (1000)     2197 2024-04-17 15:45:23.000000 geodezyx-4.4.2/geodezyx.egg-info/PKG-INFO
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     3101 2024-04-17 15:45:23.000000 geodezyx-4.4.2/geodezyx.egg-info/SOURCES.txt
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)        1 2024-04-17 15:45:23.000000 geodezyx-4.4.2/geodezyx.egg-info/dependency_links.txt
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      215 2024-04-17 15:45:23.000000 geodezyx-4.4.2/geodezyx.egg-info/requires.txt
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       14 2024-04-17 15:45:23.000000 geodezyx-4.4.2/geodezyx.egg-info/top_level.txt
-drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-04-17 15:45:23.926724 geodezyx-4.4.2/misc/
--rwxrwxr-x   0 psakicki  (1000) psakicki  (1000)       98 2024-02-08 10:49:07.000000 geodezyx-4.4.2/misc/__init__.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     1225 2024-02-08 10:49:07.000000 geodezyx-4.4.2/misc/import_generic.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     3778 2024-02-08 10:49:07.000000 geodezyx-4.4.2/misc/refactoring.py
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       38 2024-04-17 15:45:23.930724 geodezyx-4.4.2/setup.cfg
--rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    10322 2024-04-17 14:44:56.000000 geodezyx-4.4.2/setup.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-05-20 15:26:02.447947 geodezyx-4.4.3/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7652 2024-04-30 11:38:13.000000 geodezyx-4.4.3/LICENSE
+-rw-r--r--   0 psakicki  (1000) psakicki  (1000)     2197 2024-05-20 15:26:02.447947 geodezyx-4.4.3/PKG-INFO
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     6916 2024-05-20 15:05:43.000000 geodezyx-4.4.3/README.md
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-05-20 15:26:02.423947 geodezyx-4.4.3/geodezyx/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     2335 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/__init__.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-05-20 15:26:02.427947 geodezyx-4.4.3/geodezyx/athmo/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       21 2024-04-30 11:38:14.000000 geodezyx-4.4.3/geodezyx/athmo/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    30474 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/athmo/athmo.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-05-20 15:26:02.427947 geodezyx-4.4.3/geodezyx/conv/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      268 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/conv/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     9548 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/conv/conv_angle.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    23343 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/conv/conv_coords.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     9468 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/conv/conv_geometric.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     5910 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/conv/conv_interpolators.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     3871 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/conv/conv_proj_lambert.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     6573 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/conv/conv_proj_utm.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    10473 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/conv/conv_rinex.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    12024 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/conv/conv_rotation_matrices.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    81054 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/conv/conv_time.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-05-20 15:26:02.427947 geodezyx-4.4.3/geodezyx/externlib/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     1339 2024-04-30 11:38:14.000000 geodezyx-4.4.3/geodezyx/externlib/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       82 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/externlib/externlib.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-05-20 15:26:02.431947 geodezyx-4.4.3/geodezyx/files_rw/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      470 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/files_rw/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    81673 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/files_rw/geo_files_converter_lib.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     9419 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/files_rw/read_athmo.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     4813 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/files_rw/read_coords_misc.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    79477 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/files_rw/read_coords_time_series.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    19068 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/files_rw/read_eop.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    28562 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/files_rw/read_geo_files_misc.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    17355 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/files_rw/read_gnss_prods.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7239 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/files_rw/read_gnss_qc.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     8729 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/files_rw/read_igs_combi.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    18108 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/files_rw/read_logsheets.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    14631 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/files_rw/read_rinex.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     2826 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/files_rw/read_slr.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    37759 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/files_rw/write_geo_files.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     6421 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/files_rw/write_rinex.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-05-20 15:26:02.435947 geodezyx-4.4.3/geodezyx/geodyn/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      136 2024-04-30 11:38:14.000000 geodezyx-4.4.3/geodezyx/geodyn/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    10131 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/geodyn/emsgfz_load_interp.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    13584 2024-04-30 11:38:14.000000 geodezyx-4.4.3/geodezyx/geodyn/euler_pole_calc.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    27564 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/geodyn/velo_field_map_plt.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     6088 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/geodyn/volcano_mogi.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-05-20 15:26:02.435947 geodezyx-4.4.3/geodezyx/logconfig/
+-rwxrwxr-x   0 psakicki  (1000) psakicki  (1000)       80 2024-04-30 11:38:14.000000 geodezyx-4.4.3/geodezyx/logconfig/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     2329 2024-04-30 11:38:14.000000 geodezyx-4.4.3/geodezyx/logconfig/loggzyx.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-05-20 15:26:02.435947 geodezyx-4.4.3/geodezyx/marine/
+-rwxrwxr-x   0 psakicki  (1000) psakicki  (1000)      111 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/marine/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     2575 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/marine/marine.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     9593 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/marine/obp.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    30816 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/marine/obscom.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-05-20 15:26:02.435947 geodezyx-4.4.3/geodezyx/megalib/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      153 2024-04-30 11:38:14.000000 geodezyx-4.4.3/geodezyx/megalib/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      111 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/megalib/genefun.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      181 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/megalib/geo_files_converter_lib.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      226 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/megalib/geoclass.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      111 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/megalib/geodetik.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      132 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/megalib/megalib.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      171 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/megalib/softs_runner.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-05-20 15:26:02.439947 geodezyx-4.4.3/geodezyx/operational/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      703 2024-04-30 11:38:14.000000 geodezyx-4.4.3/geodezyx/operational/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    10747 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/operational/anubis_frontend.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7432 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/operational/cluster_gfz.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     6953 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/operational/download_cddis.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7135 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/operational/download_dropbox.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    14598 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/operational/download_find_files.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    34340 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/operational/download_prods.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    23695 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/operational/download_rinex.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    20970 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/operational/download_rinex_legacy.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    14112 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/operational/download_utils.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    79419 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/operational/gins_runner.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    26740 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/operational/groops_frontend.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    15737 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/operational/hector_frontend.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7915 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/operational/midas_frontend.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    14024 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/operational/pride_pppar_frontend.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    26025 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/operational/rinex_lister_plotter.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    32108 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/operational/rinex_utils.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7040 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/operational/rtklib_frontend.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     9144 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/operational/track_frontend.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-05-20 15:26:02.443947 geodezyx-4.4.3/geodezyx/reffram/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      107 2024-04-30 11:38:14.000000 geodezyx-4.4.3/geodezyx/reffram/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    43896 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/reffram/geometry.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    67284 2024-05-20 15:25:03.000000 geodezyx-4.4.3/geodezyx/reffram/gnss_products.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    11346 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/reffram/kepler_gzyx.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     3865 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/reffram/quaternions.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-05-20 15:26:02.443947 geodezyx-4.4.3/geodezyx/stats/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       50 2024-04-30 11:38:14.000000 geodezyx-4.4.3/geodezyx/stats/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    30946 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/stats/least_squares.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    44868 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/stats/stats.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-05-20 15:26:02.443947 geodezyx-4.4.3/geodezyx/time_series/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       97 2024-04-30 11:38:14.000000 geodezyx-4.4.3/geodezyx/time_series/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    48885 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/time_series/ts_class.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    17295 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/time_series/ts_export.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    39098 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/time_series/ts_fcts.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-05-20 15:26:02.443947 geodezyx-4.4.3/geodezyx/toolbox_meta/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       96 2024-04-30 11:38:14.000000 geodezyx-4.4.3/geodezyx/toolbox_meta/__init__.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-05-20 15:26:02.447947 geodezyx-4.4.3/geodezyx/utils/
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      427 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/utils/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     2011 2024-04-30 11:38:14.000000 geodezyx-4.4.3/geodezyx/utils/dict_utils.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    13504 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/utils/list_utils.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     4701 2024-05-20 14:03:47.000000 geodezyx-4.4.3/geodezyx/utils/pandas_utils.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     7247 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/utils/plot_utils.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    18458 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/utils/shell_like.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    25870 2024-05-20 10:43:18.000000 geodezyx-4.4.3/geodezyx/utils/utils_core.py
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-05-20 15:26:02.447947 geodezyx-4.4.3/geodezyx.egg-info/
+-rw-r--r--   0 psakicki  (1000) psakicki  (1000)     2197 2024-05-20 15:26:02.000000 geodezyx-4.4.3/geodezyx.egg-info/PKG-INFO
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     3147 2024-05-20 15:26:02.000000 geodezyx-4.4.3/geodezyx.egg-info/SOURCES.txt
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)        1 2024-05-20 15:26:02.000000 geodezyx-4.4.3/geodezyx.egg-info/dependency_links.txt
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      215 2024-05-20 15:26:02.000000 geodezyx-4.4.3/geodezyx.egg-info/requires.txt
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       14 2024-05-20 15:26:02.000000 geodezyx-4.4.3/geodezyx.egg-info/top_level.txt
+drwxrwxr-x   0 psakicki  (1000) psakicki  (1000)        0 2024-05-20 15:26:02.447947 geodezyx-4.4.3/misc/
+-rwxrwxr-x   0 psakicki  (1000) psakicki  (1000)       98 2024-04-30 11:38:14.000000 geodezyx-4.4.3/misc/__init__.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)      140 2024-05-20 10:43:18.000000 geodezyx-4.4.3/misc/import_generic.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)     3763 2024-05-20 10:43:18.000000 geodezyx-4.4.3/misc/refactoring.py
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)       38 2024-05-20 15:26:02.447947 geodezyx-4.4.3/setup.cfg
+-rw-rw-r--   0 psakicki  (1000) psakicki  (1000)    10323 2024-05-20 15:04:01.000000 geodezyx-4.4.3/setup.py
```

### Comparing `geodezyx-4.4.2/LICENSE` & `geodezyx-4.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.2/PKG-INFO` & `geodezyx-4.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geodezyx
-Version: 4.4.2
+Version: 4.4.3
 Summary: geodezyx (a.k.a. The GeodeZYX toolbox) aims to provide simple but useful functions for Geodesy and Geophysics.
 Home-page: https://github.com/IPGP/geodezyx
 Author: Pierre Sakic & Gustavo Mansur
 Author-email: sakic@ipgp.fr
 Keywords: geodesy,geophysics,reference frames,gnss
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `geodezyx-4.4.2/README.md` & `geodezyx-4.4.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <img src="./geodezyx_toolbox_logo.png" width="300">
 
 # geodezyx (aka ___The GeodeZYX Toolbox___) 
 
-**Version 4.4.2 / 2024-04-17**, README Revision: 2024-04-17
+**Version 4.4.3 / 2024-05-20**, README Revision: 2024-05-20
 
 
 **Authors:** Pierre Sakic (IPGP, Paris, France) & Gustavo Mansur (GFZ, Potsdam, Germany)
 
 **Documentation:** [https://ipgp.github.io/geodezyx](https://ipgp.github.io/geodezyx/)
 
 **GitHub repository:** [https://github.com/IPGP/geodezyx](https://github.com/IPGP/geodezyx) 
@@ -61,32 +61,38 @@
 
 You can also install the version hosted on PyPI (but you will not get the latest changes)
 
 ``pip install geodezyx``
 
 ### clone and manually install from GitHub
 
-You can manually fork and clone the GitHub repository
-[https://github.com/IPGP/geodezyx/](https://github.com/IPGP/geodezyx/)
+You can manually fork and/or clone the GitHub repository
+([https://github.com/IPGP/geodezyx/](https://github.com/IPGP/geodezyx/))
+using your favorite flavor:
+* SSH: ``git clone git@github.com:IPGP/geodezyx.git``
+* https: ``git clone https://github.com/IPGP/geodezyx.git``
 
 and install the Toolbox you downloaded with ``python setup.py install``
 
 Alternatively, you can also add the ``geodezyx`` folder in your ``PYTHONPATH`` (for experimented users)
 
 ## Changelog
 
+### v4.4.3, 2024-05-20
+  * Speed execution optimization for orbit/clock-related functions
+  * Misc routine improvements
 
 ### v4.4.2, 2024-04-17
   * The GitHub repository, and the project in general, has been renamed as ``geodezyx`` (in lower case)
     to uniformize its multiple spellings and then avoid confusion.
     * It must be transparent for your clones but updating them is recommended \
       https://docs.github.com/en/repositories/creating-and-managing-repositories/renaming-a-repository
   * misc routine improvements
   * Refactoring of the GNSS data/products dowmload functions
-      
+
 ### v4.4.1, 2024-02-08
   * The GitHub repository has now been moved under the IPGP organization.
     * It must be transparent for your clones but updating them is recommended \
       https://docs.github.com/en/repositories/creating-and-managing-repositories/renaming-a-repository  
   * The version numbering goes without a starting zero from now on.  
     Initially, this first zero was kept as a "perpetual beta" marker,  
     but The GeodeZYX toolbox is a grown-up project now!
```

### Comparing `geodezyx-4.4.2/geodezyx/__init__.py` & `geodezyx-4.4.3/geodezyx/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # import matplotlib.pyplot as plt
 # import multiprocessing as mp
 ## from natsort import natsorted, ns
 # import numpy as np
 # import numpy as npaa
 # import operator
 import os 
-from os import remove, close, path
+from os import path
 # import pandas as df
 # import pandas as pd
 # import pickle
 # import scipy
 # from scipy.signal import butter, lfilter, freqz
 # import shutil
 # import string
```

### Comparing `geodezyx-4.4.2/geodezyx/athmo/athmo.py` & `geodezyx-4.4.3/geodezyx/athmo/athmo.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 """
 
 #from geodezyx import *                   # Import the GeodeZYX modules
 #from geodezyx.externlib import *         # Import the external modules
 #from geodezyx.megalib.megalib import *   # Import the legacy modules names
 
 import numpy as np
-import re
-import pandas as df
-from geodezyx import conv,utils
+
+from geodezyx import conv, utils
+
 
 def PWV_conversion(zwd,Tm):
     """
     This function convert from Zenith Wet delay to Precipitate Water Vapor (PWV)
 
     Parameters
     ----------
```

### Comparing `geodezyx-4.4.2/geodezyx/conv/conv_angle.py` & `geodezyx-4.4.3/geodezyx/conv/conv_angle.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,27 +14,28 @@
 functions for Geodesy and Geophysics under the GNU LGPL v3 License
 
 Copyright (C) 2019 Pierre Sakic et al. (IPGP, sakic@ipgp.fr)
 GitHub repository :
 https://github.com/GeodeZYX/geodezyx-toolbox
 """
 
+#### Import the logger
+import logging
+# import scipy
+# from pyorbital import astronomy
+import re
+import warnings
+
 ########## BEGIN IMPORT ##########
 #### External modules
 import numpy as np
-#import scipy
-#from pyorbital import astronomy
-import re
-import warnings
 
 #### geodeZYX modules
 from geodezyx import utils
 
-#### Import the logger
-import logging
 log = logging.getLogger(__name__)
 
 #### Import star style
 # from geodezyx import *                   # Import the GeodeZYX modules
 # from geodezyx.externlib import *         # Import the external modules
 # from geodezyx.megalib.megalib import *   # Import the legacy modules names
```

### Comparing `geodezyx-4.4.2/geodezyx/conv/conv_coords.py` & `geodezyx-4.4.3/geodezyx/conv/conv_coords.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,27 +15,28 @@
 
 Copyright (C) 2019 Pierre Sakic et al. (IPGP, sakic@ipgp.fr)
 GitHub repository :
 https://github.com/GeodeZYX/geodezyx-toolbox
 """
 
 
+#### Import the logger
+import logging
+
 ########## BEGIN IMPORT ##########
 #### External modules
 import numpy as np
 import scipy
 from pyorbital import astronomy
-#import re
 
 #### geodeZYX modules
 from geodezyx import utils
 from geodezyx.conv import conv_rotation_matrices as rotmat
 
-#### Import the logger
-import logging
+# import re
 log = logging.getLogger(__name__)
 
 #### Import star style
 # from geodezyx import *                   # Import the GeodeZYX modules
 # from geodezyx.externlib import *         # Import the external modules
 # from geodezyx.megalib.megalib import *   # Import the legacy modules names
```

### Comparing `geodezyx-4.4.2/geodezyx/conv/conv_geometric.py` & `geodezyx-4.4.3/geodezyx/conv/conv_geometric.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,18 +19,17 @@
 """
 
 
 ########## BEGIN IMPORT ##########
 #### External modules
 import numpy as np
 import scipy
-import re
+
 
 #### geodeZYX modules
-from geodezyx import utils
 
 #### Import star style
 # from geodezyx import *                   # Import the GeodeZYX modules
 # from geodezyx.externlib import *         # Import the external modules
 # from geodezyx.megalib.megalib import *   # Import the legacy modules names
 
 ##########  END IMPORT  ##########
```

### Comparing `geodezyx-4.4.2/geodezyx/conv/conv_interpolators.py` & `geodezyx-4.4.3/geodezyx/conv/conv_interpolators.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,23 @@
 """
 Created on Tue Aug 24 13:58:51 2021
 
 @author: psakicki
 """
 
 import datetime as dt
+#### Import the logger
+import logging
+
+import numpy as np
 import scipy
 from scipy.spatial.transform import Rotation
-import numpy as np
 
-from geodezyx import utils,conv
+from geodezyx import utils, conv
 
-#### Import the logger
-import logging
 log = logging.getLogger(__name__)
 
 
 
 #  _______ _                   _____           _             _____       _                        _       _   _             
 # |__   __(_)                 / ____|         (_)           |_   _|     | |                      | |     | | (_)            
 #    | |   _ _ __ ___   ___  | (___   ___ _ __ _  ___  ___    | |  _ __ | |_ ___ _ __ _ __   ___ | | __ _| |_ _  ___  _ __
```

### Comparing `geodezyx-4.4.2/geodezyx/conv/conv_proj_lambert.py` & `geodezyx-4.4.3/geodezyx/conv/conv_proj_lambert.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,23 +15,24 @@
 
 Copyright (C) 2019 Pierre Sakic et al. (IPGP, sakic@ipgp.fr)
 GitHub repository :
 https://github.com/GeodeZYX/geodezyx-toolbox
 """
 
 
+#### Import the logger
+import logging
+
 ########## BEGIN IMPORT ##########
 #### External modules
 import numpy as np
 
 #### geodeZYX modules
-from geodezyx import utils,conv
+from geodezyx import conv
 
-#### Import the logger
-import logging
 log = logging.getLogger(__name__)
 
 ##########  END IMPORT  ##########
 
 
 #  _____           _           _   _                _____           _        
 # |  __ \         (_)         | | (_)              / ____|         | |
```

### Comparing `geodezyx-4.4.2/geodezyx/conv/conv_proj_utm.py` & `geodezyx-4.4.3/geodezyx/conv/conv_proj_utm.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 functions for Geodesy and Geophysics under the GNU LGPL v3 License
 
 Copyright (C) 2019 Pierre Sakic et al. (IPGP, sakic@ipgp.fr)
 GitHub repository :
 https://github.com/GeodeZYX/geodezyx-toolbox
 """
 
+#### Import the logger
+import logging
+
 ########## BEGIN IMPORT ##########
 #### External modules
 import numpy as np
 
 #### geodeZYX modules
-#from geodezyx import utils,conv
-
-#### Import the logger
-import logging
+# from geodezyx import utils,conv
 log = logging.getLogger(__name__)
 
 ##########  END IMPORT  ##########
 
     
 def utm_geo2xy(lat,lon,ellips="wgs84",zone=None): 
     """
```

### Comparing `geodezyx-4.4.2/geodezyx/conv/conv_rinex.py` & `geodezyx-4.4.3/geodezyx/conv/conv_rinex.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,28 +15,26 @@
 
 Copyright (C) 2019 Pierre Sakic et al. (IPGP, sakic@ipgp.fr)
 GitHub repository :
 https://github.com/GeodeZYX/geodezyx-toolbox
 """
 
 
+#### Import the logger
+import logging
 ########## BEGIN IMPORT ##########
 #### External modules
-import os 
-#import scipy
-#from scipy.spatial.transform import Rotation
+import os
+# import scipy
+# from scipy.spatial.transform import Rotation
 import re
 
-
 ### Imported in the corresponding function to avoid cyclic import
 ### from geodezyx.conv import conv_interpolators
 ### https://stackoverflow.com/questions/1250103/attributeerror-module-object-has-no-attribute
-
-#### Import the logger
-import logging
 log = logging.getLogger(__name__)
 
 
 def rinex_regex_search_tester(str_in,
                               short_name=True,
                               long_name=True,
                               brdc_long_name=False,
```

### Comparing `geodezyx-4.4.2/geodezyx/conv/conv_rotation_matrices.py` & `geodezyx-4.4.3/geodezyx/conv/conv_rotation_matrices.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,26 +17,27 @@
 GitHub repository :
 https://github.com/GeodeZYX/geodezyx-toolbox
 """
 
 
 
 
+#### Import the logger
+import logging
+
 ########## BEGIN IMPORT ##########
 #### External modules
 import numpy as np
-# import scipy
-# from pyorbital import astronomy
-# import re
 
 #### geodeZYX modules
 from geodezyx import utils
 
-#### Import the logger
-import logging
+# import scipy
+# from pyorbital import astronomy
+# import re
 log = logging.getLogger(__name__)
 
 ##########  END IMPORT  ##########
 
 #  _____       _        _   _               __  __       _        _               
 # |  __ \     | |      | | (_)             |  \/  |     | |      (_)              
 # | |__) |___ | |_ __ _| |_ _  ___  _ __   | \  / | __ _| |_ _ __ _  ___ ___  ___
```

### Comparing `geodezyx-4.4.2/geodezyx/conv/conv_time.py` & `geodezyx-4.4.3/geodezyx/conv/conv_time.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,39 +18,39 @@
 https://github.com/GeodeZYX/geodezyx-toolbox
 """
 
 
 ########## BEGIN IMPORT ##########
 #### External modules
 import datetime as dt
+#### Import the logger
+import logging
 import math
-import numpy as np
-import os 
-import pandas as pd
-#import scipy
-#from scipy.spatial.transform import Rotation
+import os
+import re
+# import scipy
+# from scipy.spatial.transform import Rotation
 import string
 import struct
 import subprocess
-import re
 import time
 import warnings
 ## Finding day of year
-from datetime import datetime, date 
+from datetime import datetime, date
 
-#### geodeZYX modules
-from geodezyx import utils,stats
+import numpy as np
+import pandas as pd
 
+#### geodeZYX modules
+from geodezyx import utils, stats
 ### Imported in the corresponding function to avoid cyclic import
 ### from geodezyx.conv import conv_interpolators
 from geodezyx.conv import conv_rinex
-### https://stackoverflow.com/questions/1250103/attributeerror-module-object-has-no-attribute
 
-#### Import the logger
-import logging
+### https://stackoverflow.com/questions/1250103/attributeerror-module-object-has-no-attribute
 log = logging.getLogger(__name__)
 
 
 
 ##########  END IMPORT  ##########
 
 
@@ -242,21 +242,21 @@
     Parameters
     ----------
     start_dt,end_dt : datetime
         Datetimes
         
     Returns
     -------
-    Out_range : list of datetime
+    out_range : list of datetime
         range of dates  
     """
-    Out_range = [start_dt]
-    while Out_range[-1] < end_dt:
-        Out_range.append(Out_range[-1] + dt.timedelta(days=day_step) + dt.timedelta(seconds=sec_step))
-    return Out_range
+    out_range = [start_dt]
+    while out_range[-1] < end_dt:
+        out_range.append(out_range[-1] + dt.timedelta(days=day_step) + dt.timedelta(seconds=sec_step))
+    return out_range
 
 def dt2posix(dtin,out_array=False):       
     """
     Time representation conversion
     
     Python's Datetime => POSIX Time
 
@@ -1545,14 +1545,16 @@
     
     Create a RINEX name from a station name and date
 
     Parameters
     ----------
     statname : string
         name of the station
+        if is more than 4 characters long (typically for 9-chars. names), 
+        only the 4 first characters will be used
     
     datein : datetime
         date of the wished RINEX name
         
     rnxtype : string
         extension of the RINEX ("d.Z",".o") ...
         
@@ -1568,19 +1570,23 @@
 
     alphabet = list(string.ascii_lowercase)
 
     if session_a_instead_of_daily_session:
         sess = alphabet[datein.hour]
     else:
         sess = '0'
+        
+    out_rnx_name = statname[:4] + dt2doy(datein) + sess + '.' + datein.strftime('%y') + rnxtype
+    out_rnx_name = out_rnx_name.lower()
 
-    return statname + dt2doy(datein) + sess + '.' + datein.strftime('%y') + rnxtype
+    return out_rnx_name
 
 
-def statname_dt2rinexname_long(statname,datein,
+def statname_dt2rinexname_long(statname,
+                               datein,
                                country="XXX",
                                data_source="R",
                                file_period="00U",
                                data_freq="00U",
                                data_type="MO",                               
                                format_compression='crx.gz',
                                preset_type=None):
@@ -1679,31 +1685,30 @@
     
     if len(statname) == 4:
         statname_ok = statname + "00" + country
     elif len(statname) == 9 and country != "XXX":
         statname_ok = statname[:4] + "00" + country
     else:
         statname_ok = statname
-        
-        
+
     if preset_type == "daily":
         file_period="01D"
         data_freq="30S"     
                 
     elif preset_type == "hourly":
         file_period="01H"
         data_freq="01S"     
-        
-        
+
     date_ok = datein.strftime('%Y') +  dt2doy(datein) + datein.strftime('%H%M')
     period_freq_ok = "_" + file_period + "_" + data_freq + "_" + data_type
     data_source_ok = "_" + data_source + "_"
     
     out_rnx_name = statname_ok + data_source_ok + date_ok + period_freq_ok + '.' + format_compression
-    
+    out_rnx_name = out_rnx_name.upper()
+
     return out_rnx_name
     
 
 
 
 def datestr_sinex_2_dt(datestrin):
     """
@@ -2012,88 +2017,89 @@
     gpsweek = np.floor(gpsweek_decimal)
     gpsweek_decimal_part = np.modf(gpsweek_decimal)[0]
     gpssecs = np.round(86400 * 7 * gpsweek_decimal_part) + date_diff.seconds
     
     return int(gpsweek),int(gpssecs)
 
 #### LEAP SECONDS MANAGEMENT
-    
-def leap_seconds(f):
-    """
-    Return a list of tuples of this format: (timestamp, number_of_seconds)
-        timestamp: a 32-bit timestamp, seconds since the UNIX epoch
-        number_of_seconds: how many leap-seconds occur at timestamp
-
-    INTERNAL_FUNCTION
-
-    Source
-    ------
-    http://stackoverflow.com/questions/19332902/extract-historic-leap-seconds-from-tzdata
-
-    """
-    TZFILE_MAGIC = 'TZif'.encode('US-ASCII')
-
-    fmt = ">4s c 15x 6l"
-    size = struct.calcsize(fmt)
-    (tzfile_magic, tzfile_format, ttisgmtcnt, ttisstdcnt, leapcnt, timecnt,
-        typecnt, charcnt) =  struct.unpack(fmt, f.read(size))
-    #print("DEBUG: tzfile_magic: {} tzfile_format: {} ttisgmtcnt: {} ttisstdcnt: {} leapcnt: {} timecnt: {} typecnt: {} charcnt: {}".format(tzfile_magic, tzfile_format, ttisgmtcnt, ttisstdcnt, leapcnt, timecnt, typecnt, charcnt))
-
-    # Make sure it is a tzfile(5) file
-    assert tzfile_magic == TZFILE_MAGIC, (
-            "Not a tzfile; file magic was: '{}'".format(tzfile_magic))
-
-    # comments below show struct codes such as "l" for 32-bit long integer
-    offset = (timecnt*4  # transition times, each "l"
-        + timecnt*1  # indices tying transition time to ttinfo values, each "B"
-        + typecnt*6  # ttinfo structs, each stored as "lBB"
-        + charcnt*1)  # timezone abbreviation chars, each "c"
-
-    f.seek(offset, 1) # seek offset bytes from current position
-
-    fmt = '>{}l'.format(leapcnt*2)
-    #print("DEBUG: leapcnt: {}  fmt: '{}'".format(leapcnt, fmt))
-    size = struct.calcsize(fmt)
-    data = struct.unpack(fmt, f.read(size))
-
-    lst = [(data[i], data[i+1]) for i in range(0, len(data), 2)]
-    assert all(lst[i][0] < lst[i+1][0] for i in range(len(lst)-1))
-    assert all(lst[i][1] == lst[i+1][1]-1 for i in range(len(lst)-1))
-    return lst
-
-def print_leaps(leap_lst):
-    """
-    INTERNAL_FUNCTION
-    """
-    # leap_lst is tuples: (timestamp, num_leap_seconds)
-    outlist = []
-    for ts, num_secs in leap_lst:
-        dtime = (dt.datetime.utcfromtimestamp(ts - num_secs+1))
-        outlist.append((dtime,num_secs))
-    return outlist
 
 def get_leapsecond_frontend():
     """
     INTERNAL_FUNCTION
 
     Nota :
     Universal Time (UT1) and International Atomic Time (TAI) were defined as equal 
     in 1958. When UTC was introduced in 1972, UT1 had shifted by around 10 seconds
     in relation to TAI. 
     We therefore chose an initial offset of 10 seconds between UTC and TAI.
 
         the initial 10sec are added in find_leapsecond
     """
+
+    def _parse_leap_seconds_file(f):
+        """
+        Return a list of tuples of this format: (timestamp, number_of_seconds)
+            timestamp: a 32-bit timestamp, seconds since the UNIX epoch
+            number_of_seconds: how many leap-seconds occur at timestamp
+
+        INTERNAL_FUNCTION
+
+        Source
+        ------
+        http://stackoverflow.com/questions/19332902/extract-historic-leap-seconds-from-tzdata
+
+        """
+        TZFILE_MAGIC = 'TZif'.encode('US-ASCII')
+
+        fmt = ">4s c 15x 6l"
+        size = struct.calcsize(fmt)
+        (tzfile_magic, tzfile_format, ttisgmtcnt, ttisstdcnt, leapcnt, timecnt,
+         typecnt, charcnt) = struct.unpack(fmt, f.read(size))
+        # print("DEBUG: tzfile_magic: {} tzfile_format: {} ttisgmtcnt: {} ttisstdcnt: {} leapcnt: {} timecnt: {} typecnt: {} charcnt: {}".format(tzfile_magic, tzfile_format, ttisgmtcnt, ttisstdcnt, leapcnt, timecnt, typecnt, charcnt))
+
+        # Make sure it is a tzfile(5) file
+        assert tzfile_magic == TZFILE_MAGIC, (
+            "Not a tzfile; file magic was: '{}'".format(tzfile_magic))
+
+        # comments below show struct codes such as "l" for 32-bit long integer
+        offset = (timecnt * 4  # transition times, each "l"
+                  + timecnt * 1  # indices tying transition time to ttinfo values, each "B"
+                  + typecnt * 6  # ttinfo structs, each stored as "lBB"
+                  + charcnt * 1)  # timezone abbreviation chars, each "c"
+
+        f.seek(offset, 1)  # seek offset bytes from current position
+
+        fmt = '>{}l'.format(leapcnt * 2)
+        # print("DEBUG: leapcnt: {}  fmt: '{}'".format(leapcnt, fmt))
+        size = struct.calcsize(fmt)
+        data = struct.unpack(fmt, f.read(size))
+
+        lst = [(data[i], data[i + 1]) for i in range(0, len(data), 2)]
+        assert all(lst[i][0] < lst[i + 1][0] for i in range(len(lst) - 1))
+        assert all(lst[i][1] == lst[i + 1][1] - 1 for i in range(len(lst) - 1))
+        return lst
+
+    def _print_leaps(leap_lst):
+        """
+        INTERNAL_FUNCTION
+        """
+        # leap_lst is tuples: (timestamp, num_leap_seconds)
+        outlist = []
+        for ts, num_secs in leap_lst:
+            dtime = (dt.datetime.utcfromtimestamp(ts - num_secs + 1))
+            outlist.append((dtime, num_secs))
+        return outlist
+
     zoneinfo_fname = '/usr/share/zoneinfo/right/UTC'
 
     try:
         ### Linux case : AUTO Mode
         with open(zoneinfo_fname, 'rb') as f:
-            leap_lst = leap_seconds(f)
-            final_leap_lis = print_leaps(leap_lst)
+            leap_lst = _parse_leap_seconds_file(f)
+            final_leap_lis = _print_leaps(leap_lst)
     except:
         ### Windows case : MANUAL Mode
         final_leap_lis = [(dt.datetime(1972, 7, 1, 0, 0), 1),
          (dt.datetime(1973, 1, 1, 0, 0), 2),
          (dt.datetime(1974, 1, 1, 0, 0), 3),
          (dt.datetime(1975, 1, 1, 0, 0), 4),
          (dt.datetime(1976, 1, 1, 0, 0), 5),
@@ -2115,17 +2121,22 @@
          (dt.datetime(1997, 7, 1, 0, 0), 21),
          (dt.datetime(1999, 1, 1, 0, 0), 22),
          (dt.datetime(2006, 1, 1, 0, 0), 23),
          (dt.datetime(2009, 1, 1, 0, 0), 24),
          (dt.datetime(2012, 7, 1, 0, 0), 25),
          (dt.datetime(2015, 7, 1, 0, 0), 26),
          (dt.datetime(2017, 1, 1, 0, 0), 27)]
+        log.warning("Harcoded leap second list loaded\nIt might be wrong if IERS's bulletin C has been updated!\nlast known update: %s",final_leap_lis[-1])
+
     return final_leap_lis
 
-def find_leapsecond(dtin,get_leapsec_lis=[],
+
+LEAP_SEC_LIS = get_leapsecond_frontend()
+
+def find_leapsecond(dtin,get_leapsec_lis=LEAP_SEC_LIS,
                     apply_initial_delta=True):
     """
     Find the TAI-UTC leap second for a given datetime
 
     Parameters
     ----------
     dtin : datetime
```

### Comparing `geodezyx-4.4.2/geodezyx/externlib/__init__.py` & `geodezyx-4.4.3/geodezyx/externlib/__init__.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.2/geodezyx/files_rw/geo_files_converter_lib.py` & `geodezyx-4.4.3/geodezyx/files_rw/geo_files_converter_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,34 +22,35 @@
 #import dateutil
 
 #import geodezyx.megalib.geodetik as geok
 
 ########## BEGIN IMPORT ##########
 #### External modules
 import datetime as dt
-import dateutil
-from io import BytesIO,StringIO
 import itertools
+#### Import the logger
+import logging
+import os
+import re
+import shutil
+import textwrap
+from io import BytesIO, StringIO
+
+import dateutil
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
-import os 
 import pandas as pd
-import shutil
-import textwrap
-import re
 
 #### geodeZYX modules
 from geodezyx import conv
 from geodezyx import operational
 from geodezyx import utils
 from geodezyx.files_rw import read_logsheets
 
-#### Import the logger
-import logging
 log = logging.getLogger(__name__)
 
 ##########  END IMPORT  ##########
 
 
    #_____          __  __ _____ _______                                   _
   #/ ____|   /\   |  \/  |_   _|__   __|                                 | |
@@ -469,16 +470,15 @@
 
     return outdico
 
 def write_eqfile_from_dico(dicoin,outdir,outfilename):
     outfilepath = os.path.join(outdir,outfilename)
     fil = open(outfilepath,'w+')
 
-    from collections import OrderedDict
-#    dicoin = OrderedDict(sorted(dicoin.items(), key=lambda dicoin: dicoin[1]))
+    #    dicoin = OrderedDict(sorted(dicoin.items(), key=lambda dicoin: dicoin[1]))
 #    dicoin = sorted(dicoin, key=dicoin.get)
     for k,v in dicoin.items():
         for i in range(len(v)):
             stat = k
             if i+2 > 9:
                 statbis = stat + '_' + str(i+2) + 'S'
             else:
```

### Comparing `geodezyx-4.4.2/geodezyx/files_rw/read_athmo.py` & `geodezyx-4.4.3/geodezyx/files_rw/read_athmo.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 # -*- coding: utf-8 -*-
 """
 Created on Wed Jun 30 10:52:09 2021
 
 @author: psakic
 """
 
+import re
+
 ########## BEGIN IMPORT ##########
 #### External modules
 import numpy as np
 import pandas as pd
-import re
 
 #### geodeZYX modules
 from geodezyx import conv
 from geodezyx import utils
 
+
 #### Import star style
 # from geodezyx import *                   # Import the GeodeZYX modules
 # from geodezyx.externlib import *         # Import the external modules
 # from geodezyx.megalib.megalib import *   # Import the legacy modules names
 
 ##########  END IMPORT  ##########
```

### Comparing `geodezyx-4.4.2/geodezyx/files_rw/read_coords_misc.py` & `geodezyx-4.4.3/geodezyx/files_rw/read_coords_misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,22 +5,23 @@
 
 @author: psakicki
 """
 
 ########## BEGIN IMPORT ##########
 #### External modules
 import datetime as dt
+#### Import the logger
+import logging
+
 import numpy as np
 
 #### geodeZYX modules
 from geodezyx import conv
 from geodezyx import utils
 
-#### Import the logger
-import logging
 log = logging.getLogger(__name__)
 
 
 def stations_in_EPOS_sta_coords_file_mono(coords_file_path):
     """
     Gives stations in a EPOS coords. file (YYYY_DDD_sta_coordinates)
```

### Comparing `geodezyx-4.4.2/geodezyx/files_rw/read_coords_time_series.py` & `geodezyx-4.4.3/geodezyx/files_rw/read_coords_time_series.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,32 +16,33 @@
 GitHub repository :
 https://github.com/GeodeZYX/geodezyx-toolbox
 """
 
 ########## BEGIN IMPORT ##########
 #### External modules
 import datetime as dt
-import dateutil
 import glob
+import gzip
+#### Import the logger
+import logging
+import os
+import re
+
+import dateutil
 import numpy as np
-import os 
-from io import StringIO
 import pandas as pd
 import scipy
-import re
-import gzip
+
 #### geodeZYX modules
 from geodezyx import conv
 from geodezyx import files_rw
 from geodezyx import reffram
 from geodezyx import time_series
 from geodezyx import utils
 
-#### Import the logger
-import logging
 log = logging.getLogger(__name__)
 
 ##########  END IMPORT  ##########
 
 def read_all_points(filein):
     """selectionne automatiquement le type de fichier brut en entrée
        INPUT  : chemin du fichier brut de POINTS
```

### Comparing `geodezyx-4.4.2/geodezyx/files_rw/read_eop.py` & `geodezyx-4.4.3/geodezyx/files_rw/read_eop.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 
 @author: psakicki
 """
 
 ########## BEGIN IMPORT ##########
 #### External modules
 import linecache
+#### Import the logger
+import logging
+import os
+
 import numpy as np
-import os 
 import pandas as pd
 
 #### geodeZYX modules
 from geodezyx import conv
 from geodezyx import utils
 
-#### Import the logger
-import logging
 log = logging.getLogger(__name__)
 
 
 def read_erp(file_path_in,ac=None):
     """
     
     Read IGS Analysis Center ERP files
```

### Comparing `geodezyx-4.4.2/geodezyx/files_rw/read_geo_files_misc.py` & `geodezyx-4.4.3/geodezyx/files_rw/read_geo_files_misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,29 +16,25 @@
 GitHub repository :
 https://github.com/GeodeZYX/geodezyx-toolbox
 """
 
 ########## BEGIN IMPORT ##########
 #### External modules
 import datetime as dt
-import gzip
 import linecache
-import io
+#### Import the logger
+import logging
+import os
+
 import numpy as np
-import os 
 import pandas as pd
-import re
 
 #### geodeZYX modules
-from geodezyx import conv
-from geodezyx import time_series
 from geodezyx import utils
 
-#### Import the logger
-import logging
 log = logging.getLogger(__name__)
 
 
 ##########  END IMPORT  ##########
 
 
  #  ______                _   _                _____                                         _
```

### Comparing `geodezyx-4.4.2/geodezyx/files_rw/read_gnss_prods.py` & `geodezyx-4.4.3/geodezyx/files_rw/read_gnss_prods.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,27 +5,26 @@
 
 @author: psakicki
 """
 
 ########## BEGIN IMPORT ##########
 #### External modules
 import gzip
+#### Import the logger
+import logging
+import os
+
 import numpy as np
-import os 
 import pandas as pd
-import warnings
 
 #### geodeZYX modules
 from geodezyx import conv
-#from geodezyx import time_series
+# from geodezyx import time_series
 from geodezyx import utils
 
-
-#### Import the logger
-import logging
 log = logging.getLogger(__name__)
 
  #   _____ _            _       __ _ _           
  #  / ____| |          | |     / _(_) |          
  # | |    | | ___   ___| | __ | |_ _| | ___  ___ 
  # | |    | |/ _ \ / __| |/ / |  _| | |/ _ \/ __|
  # | |____| | (_) | (__|   <  | | | | |  __/\__ \
@@ -59,14 +58,20 @@
                           only_first_occur=True,line_number=True)
     
     DFclk = pd.read_csv(file_path_in,skiprows=HeadLine[0]+1,header=None,
                         delim_whitespace = True,
                         names=['type', 'name', 'year', 'month', 'day', 'hour',
                                'minute', 'second',"n_values",'bias', 'sigma'])
     
+    
+    # Special case when D-0n instead of E-0n (e.g. IAC), 
+    # then values are not converted to float and kept as generic objects...
+    if DFclk['bias'].dtype == "O" and DFclk['bias'].str.match(".*D(\+|-)\d\d$").any():
+        DFclk['bias'] = DFclk['bias'].str.replace("D","E").astype(float)
+    
     DFclk["ac"] = os.path.basename(file_path_in)[:3] 
     DFclk["name"] = DFclk["name"].str.upper()
     if names_4char:
         DFclk['name'] = DFclk['name'].str[:4]
     
     DFclk['epoch'] = pd.to_datetime(DFclk[['year', 'month', 'day',
                                            'hour','minute', 'second']])
```

### Comparing `geodezyx-4.4.2/geodezyx/files_rw/read_gnss_qc.py` & `geodezyx-4.4.3/geodezyx/files_rw/read_gnss_qc.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 # -*- coding: utf-8 -*-
 """
 Created on Fri Dec  1 17:46:14 2023
 
 @author: psakic
 """
 
+#### Import the logger
+import logging
+import os
 import re
 from io import StringIO
-import pandas as pd 
-import numpy as np
-import os 
 
+import numpy as np
+import pandas as pd
 
-#### Import the logger
-import logging
 log = logging.getLogger(__name__)
 
 #                       _     _     
 #     /\               | |   (_)    
 #    /  \   _ __  _   _| |__  _ ___ 
 #   / /\ \ | '_ \| | | | '_ \| / __|
 #  / ____ \| | | | |_| | |_) | \__ \
```

### Comparing `geodezyx-4.4.2/geodezyx/files_rw/read_igs_combi.py` & `geodezyx-4.4.3/geodezyx/files_rw/read_igs_combi.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,27 +2,28 @@
 # -*- coding: utf-8 -*-
 """
 Created on Wed Jun 23 11:42:14 2021
 
 @author: psakicki
 """
 
+#### Import the logger
+import logging
+import os
+import re
+
 ########## BEGIN IMPORT ##########
 #### External modules
 import numpy as np
-import os 
 import pandas as pd
-import re
 
 #### geodeZYX modules
 from geodezyx import conv
 from geodezyx import utils
 
-#### Import the logger
-import logging
 log = logging.getLogger(__name__)
 
  #  _____ _____  _____    _____                _     _             _   _                _____        __ _       ______ _ _           
  # |_   _/ ____|/ ____|  / ____|              | |   (_)           | | (_)              / ____|      / _| |     |  ____(_) |          
  #   | || |  __| (___   | |     ___  _ __ ___ | |__  _ _ __   __ _| |_ _  ___  _ __   | (___   ___ | |_| |_    | |__   _| | ___  ___ 
  #   | || | |_ |\___ \  | |    / _ \| '_ ` _ \| '_ \| | '_ \ / _` | __| |/ _ \| '_ \   \___ \ / _ \|  _| __|   |  __| | | |/ _ \/ __|
  #  _| || |__| |____) | | |___| (_) | | | | | | |_) | | | | | (_| | |_| | (_) | | | |  ____) | (_) | | | |_ _  | |    | | |  __/\__ \
```

### Comparing `geodezyx-4.4.2/geodezyx/files_rw/read_logsheets.py` & `geodezyx-4.4.3/geodezyx/files_rw/read_logsheets.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,26 +18,27 @@
 """
 
 
 ########## BEGIN IMPORT ##########
 #### External modules
 import copy
 import datetime as dt
-import dateutil
 import glob
-import os 
+#### Import the logger
+import logging
+import os
+import re
+
+import dateutil
 import pandas as pd
-import re 
 
 #### geodeZYX modules
 from geodezyx import conv
 from geodezyx import utils
 
-#### Import the logger
-import logging
 log = logging.getLogger(__name__)
 
 
 ##########  END IMPORT  ##########
 
 #  _                     _               _                            _
 # | |                   | |             | |                          | |
```

### Comparing `geodezyx-4.4.2/geodezyx/files_rw/read_rinex.py` & `geodezyx-4.4.3/geodezyx/files_rw/read_rinex.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,32 +13,31 @@
 functions for Geodesy and Geophysics under the GNU LGPL v3 License
 
 Copyright (C) 2019 Pierre Sakic et al. (IPGP, sakic@ipgp.fr)
 GitHub repository :
 https://github.com/GeodeZYX/geodezyx-toolbox
 """
 
+#### Import the logger
+import logging
+import os
+import pathlib
+import re
+from io import StringIO
+
+import hatanaka
 ########## BEGIN IMPORT ##########
 #### External modules
-import datetime as dt
 import numpy as np
 import pandas as pd
-from io import StringIO
-import re
-import os
-import pathlib
 from tqdm import tqdm
-import hatanaka
 
 #### geodeZYX modules
-from geodezyx import operational,utils
-
+from geodezyx import operational, utils
 
-#### Import the logger
-import logging
 log = logging.getLogger(__name__)
 
 
 def read_rinex2_obs(rnx_in,
                     set_index=None):
     """
     Read a RINEX Observation, version 2
```

### Comparing `geodezyx-4.4.2/geodezyx/files_rw/read_slr.py` & `geodezyx-4.4.3/geodezyx/files_rw/read_slr.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
 @author: psakicki
 """
 
 import datetime as dt
 import io
 import os
-import pandas as pd
 
+import pandas as pd
 
-from geodezyx import conv,utils
+from geodezyx import conv, utils
 
 
 def read_pdm_res_slr_mono(res_file_in,
                           sol="sol"):
     """
     Read a PDM7 res(idual) file for SLR Validation
```

### Comparing `geodezyx-4.4.2/geodezyx/files_rw/write_geo_files.py` & `geodezyx-4.4.3/geodezyx/files_rw/write_geo_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,28 +16,29 @@
 GitHub repository :
 https://github.com/GeodeZYX/geodezyx-toolbox
 """
 
 ########## BEGIN IMPORT ##########
 #### External modules
 import datetime as dt
+#### Import the logger
+import logging
+import os
+import re
+
 import numpy as np
-import os 
 import pandas as pd
-import re
 
 #### geodeZYX modules
 from geodezyx import conv
-from geodezyx import utils
 from geodezyx import files_rw
 from geodezyx import reffram
-#from geodezyx.megalib.megalib import *   # Import the legacy modules names
+from geodezyx import utils
 
-#### Import the logger
-import logging
+# from geodezyx.megalib.megalib import *   # Import the legacy modules names
 log = logging.getLogger(__name__)
 
 
 #### Import star style
 # from geodezyx import *                   # Import the GeodeZYX modules
 # from geodezyx.externlib import *         # Import the external modules
 # from geodezyx.megalib.megalib import *   # Import the legacy modules names
```

### Comparing `geodezyx-4.4.2/geodezyx/files_rw/write_rinex.py` & `geodezyx-4.4.3/geodezyx/files_rw/write_rinex.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,27 +13,26 @@
 functions for Geodesy and Geophysics under the GNU LGPL v3 License
 
 Copyright (C) 2019 Pierre Sakic et al. (IPGP, sakic@ipgp.fr)
 GitHub repository :
 https://github.com/GeodeZYX/geodezyx-toolbox
 """
 
+#### Import the logger
+import logging
+from io import StringIO
+
 ########## BEGIN IMPORT ##########
 #### External modules
 import numpy as np
 import pandas as pd
-from io import StringIO
-
 
 #### geodeZYX modules
 from geodezyx import files_rw, utils
 
-
-#### Import the logger
-import logging
 log = logging.getLogger(__name__)
 
 
 def write_rinex3(DFrnx_in,rnx_header=""):
     
     import rinexfile
```

### Comparing `geodezyx-4.4.2/geodezyx/geodyn/emsgfz_load_interp.py` & `geodezyx-4.4.3/geodezyx/geodyn/emsgfz_load_interp.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -14,29 +14,29 @@
 GitHub repository :
 https://github.com/GeodeZYX/geodezyx-toolbox
 """
 
 ########## BEGIN IMPORT ##########
 #### External modules
 import datetime as dt
-import pandas as pd
-import numpy as np
-import os
 import itertools
-import scipy
+#### Import the logger
+import logging
+import os
 import urllib.request
 from urllib.parse import quote
 
+import numpy as np
+import pandas as pd
+import scipy
 
 #### geodeZYX modules
 from geodezyx import conv
 from geodezyx import utils
 
-#### Import the logger
-import logging
 log = logging.getLogger(__name__)
 
 ##########  END IMPORT  ##########
 
 def ESMGFZ_downloader(latitude,longitude,output_dir,
                       components=["NTAL","NTOL","HYDL","SLEL"],
                       CM_CF="CF",
```

### Comparing `geodezyx-4.4.2/geodezyx/geodyn/euler_pole_calc.py` & `geodezyx-4.4.3/geodezyx/geodyn/euler_pole_calc.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.2/geodezyx/geodyn/velo_field_map_plt.py` & `geodezyx-4.4.3/geodezyx/geodyn/velo_field_map_plt.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 """
 
 
 
 ########## BEGIN IMPORT ##########
 #### External modules
 import math
+
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
 
 try:
     import netCDF4
     from mpl_toolkits.basemap import Basemap
```

### Comparing `geodezyx-4.4.2/geodezyx/geodyn/volcano_mogi.py` & `geodezyx-4.4.3/geodezyx/geodyn/volcano_mogi.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,17 @@
 """
 
 
 
 """
 
 """
-import numpy as np
 import matplotlib.pyplot as plt
+import numpy as np
+
 
 # =====================
 # Inverse Models
 # =====================
 def invert(xargs,xcen,ycen,depth,dV):
     """
     Wrapper of mogi.forward to project to LOS and adjust arguments to work
```

### Comparing `geodezyx-4.4.2/geodezyx/logconfig/loggzyx.py` & `geodezyx-4.4.3/geodezyx/logconfig/loggzyx.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.2/geodezyx/marine/marine.py` & `geodezyx-4.4.3/geodezyx/marine/marine.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,28 +14,28 @@
 
 Copyright (C) 2019 Pierre Sakic et al. (IPGP, sakic@ipgp.fr)
 GitHub repository :
 https://github.com/GeodeZYX/geodezyx-toolbox
 """
 
 
+#### Import the logger
+import logging
+
 ########## BEGIN IMPORT ##########
 #### External modules
 import numpy as np
 
 #### geodeZYX modules
 from geodezyx import utils
 
 #### Import star style
 # from geodezyx import *                   # Import the GeodeZYX modules
 # from geodezyx.externlib import *         # Import the external modules
 # from geodezyx.megalib.megalib import *   # Import the legacy modules names
-
-#### Import the logger
-import logging
 log = logging.getLogger(__name__)
 
 ##########  END IMPORT  ##########
 
 def gebco_bathy_grid_extractor(dataset,latmin,latmax,lonmin,lonmax):
     """
     for safety reasons, lat and lon input MUST BE in the dataset,
```

### Comparing `geodezyx-4.4.2/geodezyx/marine/obp.py` & `geodezyx-4.4.3/geodezyx/marine/obp.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,25 +9,24 @@
 sensors in the context of the REVOSIMA network
 
 It is based on the work of Yann Terden Tranchant
 
 """
 
 
-import xarray as xr
 import numpy as np
-import seawater
 import pandas as pd
-#from datetime import datetime, timedelta
-import scipy.optimize as optimize
+import seawater
+import xarray as xr
+from scipy.signal import butter, filtfilt
+
 
-from scipy.signal import butter, lfilter, sosfilt, filtfilt
+# from datetime import datetime, timedelta
 
 #import numpy as np
-import matplotlib.pyplot as plt
 #from scipy.signal import butter
 
 def butter_highpass(cutoff, fs, order=5):
     nyq = 0.5 * fs
     normal_cutoff = cutoff / nyq
     b, a = butter(order, normal_cutoff, btype='high', analog=False)
     return b, a
```

### Comparing `geodezyx-4.4.2/geodezyx/marine/obscom.py` & `geodezyx-4.4.3/geodezyx/marine/obscom.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,25 +5,26 @@
 
 @author: psakic
 
 This module regroups the functions for the resolution estimation of the 
 REVOSIMA's OBSCOM-embeded pressure sensor
 """
 
-from geodezyx import utils
+import itertools
+#### Import the logger
+import logging
+
 import matplotlib.pyplot as plt
 import numpy as np
-import itertools
+import pandas as pd
 import scipy
-import geodezyx as gzyx
+
 import geodezyx.conv as conv
-import pandas as pd
+from geodezyx import utils
 
-#### Import the logger
-import logging
 log = logging.getLogger(__name__)
 
 
  #  ______               _                 _    __                  _   _                 
  # |  ____|             | |               | |  / _|                | | (_)                
  # | |__ _ __ ___  _ __ | |_ ___ _ __   __| | | |_ _   _ _ __   ___| |_ _  ___  _ __  ___ 
  # |  __| '__/ _ \| '_ \| __/ _ \ '_ \ / _` | |  _| | | | '_ \ / __| __| |/ _ \| '_ \/ __|
```

### Comparing `geodezyx-4.4.2/geodezyx/operational/__init__.py` & `geodezyx-4.4.3/geodezyx/operational/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from .anubis_frontend       import *
 from .cluster_gfz           import *
 # from .gins_runner         import *
 # from .gnss_downloader     import *
-from .download_cddis         import *
-from .download_dropbox       import *
-from .download_find_files    import *
-from .download_prods         import *
-from .download_rinex         import *
-from .download_utils         import *
+from .download_cddis        import *
+from .download_dropbox      import *
+from .download_find_files   import *
+from .download_prods        import *
+from .download_rinex        import *
+from .download_rinex_legacy import *
+from .download_utils        import *
 from .groops_frontend       import *
 from .hector_frontend       import *
 from .midas_frontend        import *
 from .pride_pppar_frontend  import *
 from .rinex_lister_plotter  import *
 from .rinex_utils           import *
 from .rtklib_frontend       import *
```

### Comparing `geodezyx-4.4.2/geodezyx/operational/anubis_frontend.py` & `geodezyx-4.4.3/geodezyx/operational/anubis_frontend.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,30 +5,28 @@
 
 @author: psakic
 """
 
 ########## BEGIN IMPORT ##########
 #### External modules
 import datetime as dt
-import os 
+#### Import the logger
+import logging
+import os
 import re
 import subprocess
 import time
-
-#manage XML
+# manage XML
 from xml.etree import ElementTree as et
-from xml.etree.ElementTree import Element
 
 #### geodeZYX modules
 from geodezyx import conv
 from geodezyx import operational
 from geodezyx import utils
 
-#### Import the logger
-import logging
 log = logging.getLogger(__name__)
 
 ##########  END IMPORT  ##########
 
 def anubis_runner(rnx_inp,
                   out_dir_main,
                   xml_config_generic,
```

### Comparing `geodezyx-4.4.2/geodezyx/operational/cluster_gfz.py` & `geodezyx-4.4.3/geodezyx/operational/cluster_gfz.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,31 +17,31 @@
 https://github.com/GeodeZYX/geodezyx-toolbox
 """
 
 
 ########## BEGIN IMPORT ##########
 #### External modules
 import datetime as dt
-import numpy as np
+import getpass
+#### Import the logger
+import logging
 import os
-import subprocess 
 import re
+import subprocess
 import time
-import getpass
+
+import numpy as np
 
 #### geodeZYX modules
 from geodezyx import utils
 
 #### Import star style
 # from geodezyx import *                   # Import the GeodeZYX modules
 # from geodezyx.externlib import *         # Import the external modules
 # from geodezyx.megalib.megalib import *   # Import the legacy modules names
-
-#### Import the logger
-import logging
 log = logging.getLogger(__name__)
 
 
 utils.symbols_list()
 
 ##########  END IMPORT  ##########
 def cluster_GFZ_run(commands_list,
```

### Comparing `geodezyx-4.4.2/geodezyx/operational/download_cddis.py` & `geodezyx-4.4.3/geodezyx/operational/download_cddis.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,40 +9,36 @@
 The GeodeZYX Toolbox is a software for simple but useful
 functions for Geodesy and Geophysics under the GNU LGPL v3 License
 Copyright (C) 2019 Pierre Sakic et al. (IPGP, sakic@ipgp.fr)
 GitHub repository :
 https://github.com/GeodeZYX/geodezyx-toolbox
 """
 
+#### Import the logger
+import logging
 ########## BEGIN IMPORT ##########
 #### External modules
 # import datetime as dt
-from ftplib import FTP
 # import glob
 # import itertools
 # import multiprocessing as mp
 import os
-import pandas as pd 
-# import re
-# import shutil
-import urllib
-import ftplib
+
+import pandas as pd
 
 #### geodeZYX modules
 from geodezyx import conv
 from geodezyx import utils
 
+# import re
+# import shutil
 #### Import star style
 # from geodezyx import *                   # Import the GeodeZYX modules
 # from geodezyx.externlib import *         # Import the external modules
 # from geodezyx.megalib.megalib import *   # Import the legacy modules names
-
-
-#### Import the logger
-import logging
 log = logging.getLogger(__name__)
 
 ##########  END IMPORT  ##########
 
 ## GUS CDDIS FCT FOR REPRO3 ONLY!!!! 2022-10-10
 def list_file_in_ftp(email = 'mansur@gfz-potsdam.de',
                      host = 'gdc.cddis.eosdis.nasa.gov',
```

### Comparing `geodezyx-4.4.2/geodezyx/operational/download_dropbox.py` & `geodezyx-4.4.3/geodezyx/operational/download_dropbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,22 +17,23 @@
     the other can be read only
     
 reset the token after changing the permissions!
 
 """
 
 import datetime as dt
+#### Import the logger
+import logging
+import os
+
 import pandas as pd
-#import wget
-import subprocess
+
+# import wget
 from geodezyx import conv, utils
-import os
 
-#### Import the logger
-import logging
 log = logging.getLogger(__name__)
 
 def dropbox_connect(dropbox_access_token):
     """Create a connection to Dropbox."""
 
     import dropbox
     from   dropbox.exceptions import AuthError
```

### Comparing `geodezyx-4.4.2/geodezyx/operational/download_find_files.py` & `geodezyx-4.4.3/geodezyx/operational/download_find_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,35 +14,34 @@
 """
 
 ########## BEGIN IMPORT ##########
 # External modules
 import datetime as dt
 # from ftplib import FTP
 import glob
+# Import the logger
+import logging
 # import itertools
 # import multiprocessing as mp
 import os
-import pandas as pd
 import re
-# import shutil
-# import urllib
-# import ftplib
+
+import pandas as pd
 
 # geodeZYX modules
 from geodezyx import conv
 from geodezyx import utils
 
+# import shutil
+# import urllib
+# import ftplib
 # Import star style
 # from geodezyx import *                   # Import the GeodeZYX modules
 # from geodezyx.externlib import *         # Import the external modules
 # from geodezyx.megalib.megalib import *   # Import the legacy modules names
-
-
-# Import the logger
-import logging
 log = logging.getLogger(__name__)
 
 ##########  END IMPORT  ##########
 
 
 def rinex_finder(main_dir,
                  short_name=True,
```

### Comparing `geodezyx-4.4.2/geodezyx/operational/download_prods.py` & `geodezyx-4.4.3/geodezyx/operational/download_prods.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,41 +11,37 @@
 Copyright (C) 2019 Pierre Sakic et al. (IPGP, sakic@ipgp.fr)
 GitHub repository :
 https://github.com/GeodeZYX/geodezyx-toolbox
 """
 
 ########## BEGIN IMPORT ##########
 #### External modules
-import datetime as dt
-from ftplib import FTP
 # import glob
 import itertools
+#### Import the logger
+import logging
 import multiprocessing as mp
-import numpy as np
 import os
-# import pandas as pd 
+# import pandas as pd
 import re
 import shutil
-# import urllib
-# import ftplib
 
+import numpy as np
+
+import geodezyx.operational.download_utils as dlutils
 #### geodeZYX modules
 from geodezyx import conv
 from geodezyx import utils
 
-import geodezyx.operational.download_utils as dlutils
-
+# import urllib
+# import ftplib
 #### Import star style
 # from geodezyx import *                   # Import the GeodeZYX modules
 # from geodezyx.externlib import *         # Import the external modules
 # from geodezyx.megalib.megalib import *   # Import the legacy modules names
-
-
-#### Import the logger
-import logging
 log = logging.getLogger(__name__)
 
 ##########  END IMPORT  ##########
 
 
 
 #  _____               _            _         _____                      _                 _           
@@ -336,17 +332,17 @@
             [Potential_localfiles_list.append(os.path.join(archive_dir_specif,f)) for f in Files_remote_date_list]
         
         Potential_localfiles_list_all = Potential_localfiles_list_all +  Potential_localfiles_list 
 
         ### Actual Download
         if ftp_download and parallel_download == 1:
             for tup in Downld_tuples_list:
-                dlutils.FTP_downloader(*tup)
+                dlutils.ftp_downloader_core(*tup)
         elif ftp_download and parallel_download > 1:
-            _ = pool.map_async(dlutils.FTP_downloader_wo_objects,
+            _ = pool.map_async(dlutils.ftp_downloader_wo_objects,
                                Downld_tuples_list)
         elif not ftp_download and parallel_download == 1:
             for tup in Downld_tuples_list:
                 dlutils.downloader_wrap(tup)
         elif not ftp_download and parallel_download > 1:
             _ = pool.map(dlutils.downloader_wrap,Downld_tuples_list)
```

### Comparing `geodezyx-4.4.2/geodezyx/operational/download_rinex.py` & `geodezyx-4.4.3/geodezyx/operational/download_rinex_legacy.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,39 +12,37 @@
 GitHub repository :
 https://github.com/GeodeZYX/geodezyx-toolbox
 """
 
 ########## BEGIN IMPORT ##########
 #### External modules
 import datetime as dt
+#### Import the logger
+import logging
 # from ftplib import FTP
 # import glob
 # import itertools
 import multiprocessing as mp
 import os
-# import pandas as pd 
-# import re
-# import shutil
-# import urllib
-# import ftplib
 
+import geodezyx.operational.download_utils as dlutils
 #### geodeZYX modules
 from geodezyx import conv
 from geodezyx import utils
-import geodezyx.operational.download_utils as dlutils
 
+# import pandas as pd
+# import re
+# import shutil
+# import urllib
+# import ftplib
 #### Import star style
 # from geodezyx import *                   # Import the GeodeZYX modules
 # from geodezyx.externlib import *         # Import the external modules
 # from geodezyx.megalib.megalib import *   # Import the legacy modules names
 
-
-#### Import the logger
-import logging
-
 log = logging.getLogger(__name__)
 
 
 ##########  END IMPORT  ##########
 
 
 #_____________ _   _ ________   __  _____                      _                 _
@@ -56,33 +54,33 @@
 
 
 ############################################################################
 ######## RINEX DOWNLOADER
 ############################################################################
 
 
-def igs_sopac_server(stat, date):
+def igs_sopac_server_legacy(stat, date):
     # plante si trop de requete
     urlserver = "ftp://garner.ucsd.edu/pub/rinex/"
     rnxname = conv.statname_dt2rinexname(stat.lower(), date)
     url = os.path.join(urlserver, str(date.year), conv.dt2doy(date), rnxname)
     return url
 
 
-def igs_cddis_server(stat, date, user = '', passwd = ''):
+def igs_cddis_server_legacy(stat, date, user ='', passwd =''):
     # a privilegier
     urlserver = "ftp://gdc.cddis.eosdis.nasa.gov/gps/data/daily/"
     rnxname = conv.statname_dt2rinexname(stat.lower(), date)
     url = os.path.join(urlserver, str(date.year), conv.dt2doy(date), date.strftime('%y') + 'd', rnxname)
     if not passwd:
         passwd = 'sakic@ipgp.fr'
     return url, user, passwd
 
 
-def igs_cddis_nav_server(stat, date):
+def igs_cddis_nav_server_legacy(stat, date):
     # a privilegier
     urlserver = "ftp://cddis.gsfc.nasa.gov/gps/data/daily/"
     rnxname = conv.statname_dt2rinexname(stat.lower(), date, 'n.Z')
     url = os.path.join(urlserver, str(date.year), conv.dt2doy(date), date.strftime('%y') + 'n', rnxname)
     return url
 
 
@@ -90,37 +88,37 @@
     urlserver = "ftp://igs-ftp.bkg.bund.de/IGS/BRDC/"
     #ftp://igs-ftp.bkg.bund.de/IGS/BRDC/2024/082/BRDC00WRD_S_20240820000_01D_MN.rnx.gz
     rnxname = "BRDC00WRD_S_" + conv.dt2str(date, '%Y%j') + "0000_01D_MN.rnx.gz"
     url = os.path.join(urlserver, str(date.year), conv.dt2doy(date), rnxname)
     return url
 
 
-def nav_rob_server(stat, date):
+def nav_rob_server_legacy(stat, date):
     urlserver = "ftp://epncb.oma.be/pub/obs/BRDC/"
     #ftp://epncb.oma.be/pub/obs/BRDC/2018/BRDC00GOP_R_20180010000_01D_MN.rnx.gz
     rnxname = "BRDC00GOP_R_" + conv.dt2str(date, '%Y%j') + "0000_01D_MN.rnx.gz"
     url = os.path.join(urlserver, str(date.year), rnxname)
     return url
 
 
-def rgp_ign_smn_server(stat, date):
+def rgp_ign_smn_server_legacy(stat, date):
     urlserver = "ftp://rgpdata.ign.fr/pub/data/"
     rnxname = conv.statname_dt2rinexname(stat.lower(), date)
     url = os.path.join(urlserver, str(date.year), conv.dt2doy(date), 'data_30', rnxname)
     return url
 
 
 def rgp_ign_mlv_server(stat, date):
     urlserver = "ftp://rgpdata.ensg.eu/pub/data/"
     rnxname = conv.statname_dt2rinexname(stat.lower(), date)
     url = os.path.join(urlserver, str(date.year), conv.dt2doy(date), 'data_30', rnxname)
     return url
 
 
-def rgp_ign_smn_1Hz_server(stat, date):
+def rgp_ign_smn_1_hz_server_legacy(stat, date):
     urlserver = "ftp://rgpdata.ign.fr/pub/data/"
 
     urls = []
 
     for h in range(24):
         date_session = date
         date_session = date_session.replace(hour=h)
@@ -132,15 +130,15 @@
                            'data_1', rnxname)
 
         urls.append(url)
 
     return urls
 
 
-def unavco_server(stat, date):
+def unavco_server_legacy(stat, date):
     urlserver = 'ftp://data-out.unavco.org/pub/rinex'
     rnxname = conv.statname_dt2rinexname(stat.lower(), date)
     url = os.path.join(urlserver, 'obs', str(date.year), conv.dt2doy(date), rnxname)
     return url
 
 
 def renag_server(stat, date):
@@ -152,48 +150,48 @@
 def uwiseismic_server(stat, date, user='', passwd=''):
     urlserver = "ftp://www2.uwiseismic.com/"
     rnxname = conv.statname_dt2rinexname(stat.lower(), date)
     url = os.path.join(urlserver, 'rinex', str(date.year), conv.dt2doy(date), rnxname)
     return url, user, passwd
 
 
-def orpheon_server(stat, date, user='', passwd=''):
+def orpheon_server_legacy(stat, date, user='', passwd=''):
     urlserver = "ftp://renag.unice.fr/"
     rnxname = conv.statname_dt2rinexname(stat.lower(), date)
     url = os.path.join(urlserver, str(date.year), conv.dt2doy(date), rnxname)
     return url, user, passwd
 
 
-def ovsg_server(stat, date, user='', passwd=''):
+def ovsg_server_legacy(stat, date, user='', passwd=''):
     if dt.datetime(2009, 1, 1) <= date <= dt.datetime(2014, 2, 10):
         urlserver = "http://webobs.ovsg.univ-ag.fr/rawdata/GPS-GPSDATA.backtemp_20140210/"
     else:
         urlserver = "http://webobs.ovsg.univ-ag.fr/rawdata/GPS/GPSDATA/"
     rnxname = conv.statname_dt2rinexname(stat.lower(), date)
     url = os.path.join(urlserver, str(date.year), conv.dt2doy(date), 'rinex', rnxname)
     return url, user, passwd
 
 
-def geoaus_server(stat, date):
+def geoaus_server_legacy(stat, date):
     """ Geosciences Australia
         ex : ftp://ftp.ga.gov.au/geodesy-outgoing/gnss/data/daily/2010/10063/ """
     urlserver = "ftp://ftp.ga.gov.au/geodesy-outgoing/gnss/data/daily/"
     rnxname = conv.statname_dt2rinexname(stat.lower(), date)
     url = os.path.join(urlserver, str(date.year), date.strftime('%y') + conv.dt2doy(date), rnxname)
     return url
 
 
-def sonel_server(stat, date):
+def sonel_server_legacy(stat, date):
     """ex : ftp://ftp.sonel.org/gps/data/2015/001/ """
     urlserver = 'ftp://ftp.sonel.org/gps/data/'
     rnxname = conv.statname_dt2rinexname(stat.lower(), date)
     url = os.path.join(urlserver, str(date.year), conv.dt2doy(date), rnxname)
     return url
 
-def ens_fr(stat, date):
+def ens_fr_legacy(stat, date):
     urlserver = 'ftp://gnss.ens.fr/pub/public/crl/GPS/rinex/'
     rnxname = conv.statname_dt2rinexname(stat.lower(), date)
     url = os.path.join(urlserver, str(date.year), conv.dt2doy(date), rnxname)
     return url
 
 
 def effective_save_dir(parent_archive_dir, stat, date, archtype='stat'):
@@ -223,26 +221,26 @@
     week, dow = conv.dt2gpstime(date)
     for f in fff:
         out_save_dir = os.path.join(out_save_dir, eval(f))
     return out_save_dir
 
 def multi_downloader_rinex(**kwargs):
     log.warn('multi_downloader_rinex is a legacy alias for the newly renamed function download_gnss_rinex')
-    return download_gnss_rinex(**kwargs)
+    return download_gnss_rinex_legacy(**kwargs)
 
 
-def download_gnss_rinex(statdico, archive_dir, startdate, enddate,
-                        archtype='stat', parallel_download=4,
-                        sorted_mode=False, user='', passwd='',
-                        filter_ftp_crawler=True,
-                        path_ftp_crawled_files_save=None,
-                        path_ftp_crawled_files_load=None,
-                        quiet_mode=False,
-                        final_archive_for_sup_check=None,
-                        force=False):
+def download_gnss_rinex_legacy(statdico, archive_dir, startdate, enddate,
+                               archtype='stat', parallel_download=4,
+                               sorted_mode=False, user='', passwd='',
+                               filter_ftp_crawler=True,
+                               path_ftp_crawled_files_save=None,
+                               path_ftp_crawled_files_load=None,
+                               quiet_mode=False,
+                               final_archive_for_sup_check=None,
+                               force=False):
     """
     Parameters
     ----------
     statdico : dict
         a statdico is a dictionary associating Archives Centers to list of stations
 
         Exemple:
@@ -341,75 +339,86 @@
     Returns
     -------
     url_list : list of str
         list of URLs
 
     savedir_list : list of str
         list of downloaded products paths
+        
+    Minimal exemple
+    ---------------
+        >>> statdic = dict()  
+        >>> statdic['igs_cddis'] = ['ZIMM']  
+        >>> archive_dir = '/home/USER/test_dl_rnx'  
+        >>> startdate = dt.datetime(2000,1,1)
+        >>> enddate = dt.datetime(2000,1,31)
+        >>> geodezyx.operational.download_gnss_rinex_legacy(statdic, archive_dir, startdate, enddate)
+    
     """
 
     curdate = startdate
 
     pool = mp.Pool(processes=parallel_download)
 
     urllist = []
     savedirlist = []
 
     log.info("generating the list of potential RINEXs ...")
+
     while curdate <= enddate:
         for netwk, statlis in list(statdico.items()):
             
             if not utils.is_iterable(statlis):
                 log.warning("%s given in the 'statdico' should be a list and it is not.",
                             statlis)
             
             for stat in statlis:
                 stat = stat.lower()
-                mode1Hz = False
+                mode1hz = False
                 secure_ftp = False
 
                 if netwk in ('igs_cddis','igs'):
                     secure_ftp = True
-                    url = igs_cddis_server(stat, curdate, user, passwd)
+                    url = igs_cddis_server_legacy(stat, curdate, user, passwd)
                 elif netwk == 'igs_sopac':
-                    url = igs_sopac_server(stat, curdate)
+                    url = igs_sopac_server_legacy(stat, curdate)
                 elif netwk == 'rgp':
-                    url = rgp_ign_smn_server(stat, curdate)
+                    url = rgp_ign_smn_server_legacy(stat, curdate)
                 elif netwk == 'rgp_mlv':
                     url = rgp_ign_mlv_server(stat, curdate)
                 elif netwk == 'rgp_1Hz':
-                    urls = rgp_ign_smn_1Hz_server(stat, curdate)
-                    mode1Hz = True
+                    urls = rgp_ign_smn_1_hz_server_legacy(stat, curdate)
+                    mode1hz = True
                 elif netwk == 'renag':
                     url = renag_server(stat, curdate)
                 elif netwk == 'orpheon':
-                    url = orpheon_server(stat, curdate, user, passwd)
+                    url = orpheon_server_legacy(stat, curdate, user, passwd)
                 elif netwk == 'uwiseismic':
                     url = uwiseismic_server(stat, curdate, user, passwd)
                 elif netwk == 'ovsg':
-                    url = ovsg_server(stat, curdate, user, passwd)
+                    url = ovsg_server_legacy(stat, curdate, user, passwd)
                 elif netwk == 'unavco':
-                    url = unavco_server(stat, curdate)
+                    url = unavco_server_legacy(stat, curdate)
                 elif netwk == 'sonel':
-                    url = sonel_server(stat, curdate)
+                    url = sonel_server_legacy(stat, curdate)
                 elif netwk == 'geoaus':
-                    url = geoaus_server(stat, curdate)
+                    url = geoaus_server_legacy(stat, curdate)
                 elif netwk in ('nav', 'brdc'):
-                    url = nav_rob_server(stat, curdate)
+                    url = nav_rob_server_legacy(stat, curdate)
                 elif netwk in ('nav_rt', 'brdc_rt'):
                     url = nav_bkg_server(stat, curdate)
                 elif netwk == 'ens_fr':
-                    url = ens_fr(stat, curdate)
+                    url = ens_fr_legacy(stat, curdate)
                 else:
                     log.warning('unkwn server dic in the dico, skip ...')
                     continue
 
                 savedir = effective_save_dir(archive_dir, stat, curdate, archtype)
 
-                if not mode1Hz:
+                if not mode1hz:
                     urllist.append(url)
                     savedirlist.append(savedir)
                 else:
                     urllist = urllist + urls
                     savedirlist = savedirlist + [savedir] * len(urls)
 
         curdate = curdate + dt.timedelta(days=1)
@@ -428,17 +437,17 @@
     log.info(str(len(urllist)) + " potential RINEXs")
 
     ### Use of the advanced FTP Crawler
     if filter_ftp_crawler:
         if path_ftp_crawled_files_load: ## if the previous files are loaded
             urllist, savedirlist = utils.pickle_loader(path_ftp_crawled_files_load)
         else: ## regular case
-            urllist, savedirlist = dlutils.ftp_files_crawler(urllist,
-                                                             savedirlist, 
-                                                             secure_ftp=secure_ftp)
+            urllist, savedirlist = dlutils.ftp_files_crawler_legacy(urllist,
+                                                                    savedirlist,
+                                                                    secure_ftp=secure_ftp)
             if path_ftp_crawled_files_save:
                 savetup = (urllist, savedirlist)
                 utils.pickle_saver(savetup,
                                    full_path=path_ftp_crawled_files_save)
 
     ##### Check if the rinex file already exists in the final archive
     if final_archive_for_sup_check and not force:
@@ -452,32 +461,32 @@
             if not os.path.basename(u) in Files_final_arch_basename:
                 urllist_new.append(u)
                 savedirlist_new.append(sd)
 
         urllist, savedirlist = urllist_new, savedirlist_new
 
     if not quiet_mode:
-        if not secure_ftp:
+        if not secure_ftp: ### all the servers except CDDIS
             if sorted_mode:
                 _ = [pool.apply_async(dlutils.downloader, args=(u, sd, force)) for u, sd in zip(urllist, savedirlist)]
             else:
                 forcelis = [force] * len(urllist)
                 _ = pool.map(dlutils.downloader_wrap, list(zip(urllist,
                                                                savedirlist,
                                                                forcelis)))
         else: ## secure FTP i.e. CDDIS
             ftp_obj , _ = dlutils.ftp_objt_create(secure_ftp_inp=secure_ftp,
                                                   host=url[0].split("/")[2],
                                                   user=url[1],
                                                   passwd=url[2])
             
             for iurl,isavedir in zip(urllist,savedirlist):
-                localpath , bool_dl = dlutils.FTP_downloader_full_remote_path(ftp_obj,
-                                                                              iurl[0],
-                                                                              isavedir)
+                localpath , bool_dl = dlutils.ftp_downloader(ftp_obj,
+                                                             iurl[0],
+                                                             isavedir)
                 
 
     localfiles_lis = []
     skiped_url = 0
     for url, savedir in zip(urllist, savedirlist):
         try:
             if type(url) is tuple:
@@ -569,8 +578,8 @@
         else:
             mv_fct(rnx, savedir)
             mv_cnt += 1
 
     log.info('RINEXs skiped :' + str(skip_cnt) + ' (because already exist)')
     log.info('RINEXs moved  :' + str(mv_cnt))
 
-    return None
+    return None
```

### Comparing `geodezyx-4.4.2/geodezyx/operational/download_utils.py` & `geodezyx-4.4.3/geodezyx/operational/download_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,40 +9,39 @@
 The GeodeZYX Toolbox is a software for simple but useful
 functions for Geodesy and Geophysics under the GNU LGPL v3 License
 Copyright (C) 2019 Pierre Sakic et al. (IPGP, sakic@ipgp.fr)
 GitHub repository :
 https://github.com/GeodeZYX/geodezyx-toolbox
 """
 
-########## BEGIN IMPORT ##########
-#### External modules
-# import datetime as dt
-from ftplib import FTP, FTP_TLS
+import ftplib
+#### Import the logger
+import logging
 # import glob
 # import itertools
 # import multiprocessing as mp
 import os
-import pandas as pd 
 # import re
 import shutil
 import urllib
-import ftplib
+########## BEGIN IMPORT ##########
+#### External modules
+# import datetime as dt
+from ftplib import FTP, FTP_TLS
+
+import pandas as pd
 
 #### geodeZYX modules
 from geodezyx import conv
 from geodezyx import utils
 
 #### Import star style
 # from geodezyx import *                   # Import the GeodeZYX modules
 # from geodezyx.externlib import *         # Import the external modules
 # from geodezyx.megalib.megalib import *   # Import the legacy modules names
-
-
-#### Import the logger
-import logging
 log = logging.getLogger(__name__)
 
 ##########  END IMPORT  ##########
 
 
 def start_end_date_easy(start_year,start_doy,end_year,end_doy):
     """
@@ -110,25 +109,23 @@
 #  _    _ _______ _______ _____    _____                      _                 _ 
 # | |  | |__   __|__   __|  __ \  |  __ \                    | |               | |
 # | |__| |  | |     | |  | |__) | | |  | | _____      ___ __ | | ___   __ _  __| |
 # |  __  |  | |     | |  |  ___/  | |  | |/ _ \ \ /\ / / '_ \| |/ _ \ / _` |/ _` |
 # | |  | |  | |     | |  | |      | |__| | (_) \ V  V /| | | | | (_) | (_| | (_| |
 # |_|  |_|  |_|     |_|  |_|      |_____/ \___/ \_/\_/ |_| |_|_|\___/ \__,_|\__,_|
                                                                                 
-                                                                                
-
 
 #### HTTP classic Download
 
 def downloader(url,savedir,force = False,
                check_if_file_already_exists_uncompressed=True):
     """
     general function to download a file
-
-    INTERNAL_FUNCTION
+    
+    can also handle non secure FTP
     """
 
     if type(url) is tuple:
         need_auth = True
         username = url[1]
         password = url[2]
         url = url[0]
@@ -137,24 +134,24 @@
         username = ''
         password = ''
         
     url_print = str(url)
 
     rnxname = os.path.basename(url)
 
-    Pot_compress_files_list = [os.path.join(savedir , rnxname)]
+    pot_compress_files_list = [os.path.join(savedir , rnxname)]
 
     if check_if_file_already_exists_uncompressed:
-        Pot_compress_files_list.append(os.path.join(savedir ,
+        pot_compress_files_list.append(os.path.join(savedir ,
                                                     rnxname.replace(".gz","")))
-        Pot_compress_files_list.append(os.path.join(savedir ,
+        pot_compress_files_list.append(os.path.join(savedir ,
                                                     rnxname.replace(".Z","")))
-        Pot_compress_files_list = list(set(Pot_compress_files_list))
+        pot_compress_files_list = list(set(pot_compress_files_list))
 
-    for f in Pot_compress_files_list:
+    for f in pot_compress_files_list:
         if os.path.isfile(f) and (not force):
             log.info(os.path.basename(f) + " already exists locally ;)")
             return None
         
     ##### LOCAL FILE (particular case for GFZ)
     if os.path.isfile(url):
         log.info("INFO : downloader : the is a local file, a simple copy will be used")
@@ -191,23 +188,18 @@
         with open(outpath, "wb") as code:
             code.write(data)
         return_str = outpath
         
     elif (("ftp" in url) and need_auth):
         log.critical("MUST BE IMPEMENTED")
         return_str = ""
-
-
-        
-        
     else:
         log.error("something goes wrong with the URL")
         log.error(url)
         return_str = ""
-        
 
     return return_str
 
 
 def downloader_wrap(intup):
     downloader(*intup)
     return None
@@ -263,34 +255,34 @@
         #ftp.prot_p()
     else:     
         ftp_constuctor = FTP
         #ftp = ftp_constuctor(arch_center_main)
         #ftp.login()
         
     ## create a list of FTP object for multiple downloads
-    Ftp_obj_list_out = [ftp_constuctor(host) for i in range(parallel_download)]
+    ftp_obj_list_out = [ftp_constuctor(host) for i in range(parallel_download)]
     if secure_ftp_inp:
-        [f.login(user,passwd) for f in Ftp_obj_list_out]
-        [f.prot_p() for f in Ftp_obj_list_out]    
+        [f.login(user,passwd) for f in ftp_obj_list_out]
+        [f.prot_p() for f in ftp_obj_list_out]
     else:
-        [f.login() for f in Ftp_obj_list_out]    
+        [f.login() for f in ftp_obj_list_out]
         
     # define the main obj for crawling
-    ftp_main = Ftp_obj_list_out[0]
+    ftp_main = ftp_obj_list_out[0]
     
     # change the directory of the main ftp obj if we ask for it
     if chdir:
         log.info("Move to: %s",chdir)
         ftp_main.cwd(chdir)
     
-    return ftp_main, Ftp_obj_list_out
+    return ftp_main, ftp_obj_list_out
 
 
 
-def ftp_files_crawler(urllist,savedirlist,secure_ftp):
+def ftp_files_crawler_legacy(urllist, savedirlist, secure_ftp):
     """
     filter urllist,savedirlist generated with download_gnss_rinex with an
     optimized FTP crawl
 
     """
     ### create a DataFrame based on the urllist and savedirlist lists
     DF = pd.concat((pd.DataFrame(urllist),pd.DataFrame(savedirlist)),axis=1)
@@ -374,15 +366,21 @@
     else:
         urllist_out = list(DFgood.url)    
     
     savedirlist_out = list(DFgood.savedir)
     
     return urllist_out, savedirlist_out
 
-def FTP_downloader(ftp_obj,filename,localdir):   
+def ftp_downloader_core(ftp_obj, filename, localdir):
+    """
+    do the FTP download, if we are aleady in the right FTP folder
+
+    internal function of ftp_downloader
+
+    """
     localpath = os.path.join(localdir,filename)
     
     if not os.path.isdir(localdir):
         utils.create_dir(localdir)
     
     if not utils.empty_file_check(localpath):
         log.info(filename + " already exists ;)")
@@ -398,30 +396,41 @@
         except Exception as e:
             log.warning(localpath + " download failed :(")
             log.warning(e)
             bool_dl = False
     
     return localpath , bool_dl
 
-def FTP_downloader_full_remote_path(ftp_obj,full_remote_path,localdir):   
-    
-    #host = full_remote_path[0].split("/")[2]          
-    
+def ftp_downloader(ftp_obj, full_remote_path, localdir):
+    """
+    download a file through FTP protocol
+    """
+
     filename = os.path.basename(full_remote_path)
     intermed_path = full_remote_path.split("/")[3:]
     intermed_path.remove(filename)
     intermed_path = "/" + "/".join(intermed_path)
 
     ftp_obj.cwd(intermed_path)
     
-    return FTP_downloader(ftp_obj, filename, localdir)
+    return ftp_downloader_core(ftp_obj, filename, localdir)
 
-def FTP_downloader_wo_objects(tupin):
+def ftp_downloader_wrap(intup):
+    outtup = ftp_downloader(*intup)
+    return outtup
+
+
+def ftp_downloader_wo_objects(tupin):
+    """
+    create the necessary FTP object
+
+    should not be used anymore
+    """
     arch_center_main,wwww_dir,filename,localdir = tupin
     ftp_obj_wk = FTP(arch_center_main)
     ftp_obj_wk.login()
     ftp_obj_wk.cwd(wwww_dir)
-    localpath , bool_dl = FTP_downloader(ftp_obj_wk,filename,localdir)
+    localpath , bool_dl = ftp_downloader_core(ftp_obj_wk, filename, localdir)
     ftp_obj_wk.close()
     return localpath , bool_dl
```

### Comparing `geodezyx-4.4.2/geodezyx/operational/gins_runner.py` & `geodezyx-4.4.3/geodezyx/operational/gins_runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,35 +20,36 @@
 
 ########## BEGIN IMPORT ##########
 #### External modules
 import collections
 import copy
 import datetime as dt
 import glob
+#### Import the logger
+import logging
 import multiprocessing as mp
-import numpy as np
 import os
-import pandas as pd
 import re
 import shutil
 import subprocess
 import sys
 import time
+
+import numpy as np
+import pandas as pd
 import yaml
-from bs4 import UnicodeDammit #finding the right encoding for debug
+from bs4 import UnicodeDammit  # finding the right encoding for debug
 
 #### geodeZYX modules
 from geodezyx import conv
-from geodezyx import utils
 from geodezyx import files_rw
 from geodezyx import operational
 from geodezyx import time_series
+from geodezyx import utils
 
-#### Import the logger
-import logging
 log = logging.getLogger(__name__)
 
 ##########  END IMPORT  ##########
 
 def get_gins_path(extended=False):
     try:
         gs_user =  os.environ['GS_USER']
```

### Comparing `geodezyx-4.4.2/geodezyx/operational/groops_frontend.py` & `geodezyx-4.4.3/geodezyx/operational/groops_frontend.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,26 +3,25 @@
 """
 Created on Tue Jan 17 10:54:49 2023
 
 @author: psakicki
 """
 
 import datetime as dt
-import numpy as np
-import subprocess
-import urllib
-from geodezyx import utils, conv, operational
-from xml.etree import ElementTree as et
+#### Import the logger
+import logging
 import os
-from threading import Thread
 import time
+import urllib
+from threading import Thread
 
+import numpy as np
+
+from geodezyx import utils, conv, operational
 
-#### Import the logger
-import logging
 log = logging.getLogger(__name__)
 
 def log_subprocess(pipe,logger=None,file=None,file2=None):
     """
     Intern fuction for subprocess_frontend2
     to write the stdout/err in the console logger + a logfile
     """
@@ -83,15 +82,15 @@
     -----
     Inspired by:
     https://stackoverflow.com/questions/21953835/run-subprocess-and-print-output-to-logging
     And for the threading:
     https://stackoverflow.com/questions/6809590/merging-a-python-scripts-subprocess-stdout-and-stderr-while-keeping-them-disti
     """
     
-    from subprocess import Popen, PIPE, STDOUT
+    from subprocess import Popen, PIPE
     now = utils.get_timestamp()
     
     #### manage the paths of the output logs
     if save_log:
         if not log_dir:
             log_dir = os.getcwd()
     
@@ -280,15 +279,14 @@
     return Files_hour_list
     
 #%%
 
 
 def _search_xml_groops_global(xmlpath,global_label):
     from xml.etree import ElementTree as et
-    from xml.etree.ElementTree import Element
 
     xmltree = et.parse(xmlpath)
 
     for element in xmltree.getroot().find("global"):
         if element.attrib["label"] == global_label:  
             elementok = element
             return elementok.text
```

### Comparing `geodezyx-4.4.2/geodezyx/operational/hector_frontend.py` & `geodezyx-4.4.3/geodezyx/operational/hector_frontend.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,28 +17,28 @@
 https://github.com/GeodeZYX/geodezyx-toolbox
 """
 
 ########## BEGIN IMPORT ##########
 #### External modules
 import datetime as dt
 import glob
-import matplotlib.pyplot as plt
-import numpy as np
-import os 
-import pandas
+#### Import the logger
+import logging
+import os
 import shutil
 import subprocess
 import time
 
+import matplotlib.pyplot as plt
+import numpy as np
+
+from geodezyx import reffram
 #### geodeZYX modules
 from geodezyx import utils
-from geodezyx import reffram
 
-#### Import the logger
-import logging
 log = logging.getLogger(__name__)
 
 ##########  END IMPORT  ##########
 #  _    _ ______ _____ _______ ____  _____
 # | |  | |  ____/ ____|__   __/ __ \|  __ \
 # | |__| | |__ | |       | | | |  | | |__) |
 # |  __  |  __|| |       | | | |  | |  _  /
```

### Comparing `geodezyx-4.4.2/geodezyx/operational/midas_frontend.py` & `geodezyx-4.4.3/geodezyx/operational/midas_frontend.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,28 +16,29 @@
 GitHub repository :
 https://github.com/GeodeZYX/geodezyx-toolbox
 """
 
 ########## BEGIN IMPORT ##########
 #### External modules
 import glob
+#### Import the logger
+import logging
+import os
+import shutil
+import subprocess
+
 import matplotlib.pyplot as plt
 import numpy as np
-import os 
 import pandas as pd
-import shutil
-import subprocess
 
 #### geodeZYX modules
 from geodezyx import conv
 from geodezyx import stats
 from geodezyx import utils
 
-#### Import the logger
-import logging
 log = logging.getLogger(__name__)
 
 ##########  END IMPORT  ##########
 
 
 #
 #  __  __ _____ _____           _____
```

### Comparing `geodezyx-4.4.2/geodezyx/operational/pride_pppar_frontend.py` & `geodezyx-4.4.3/geodezyx/operational/pride_pppar_frontend.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,32 +2,30 @@
 # -*- coding: utf-8 -*-
 """
 Created on Wed Feb 14 18:01:49 2024
 
 @author: psakic
 """
 
-#### Import star style
-from geodezyx import operational
-from geodezyx import conv
-from geodezyx import files_rw
-from geodezyx import utils
-
 import datetime as dt
-import os 
-import shutil
-import hatanaka
-from subprocess import Popen, PIPE
+#### Import the logger
+import logging
 import multiprocessing as mp
+import os
+import shutil
+import subprocess
 
+import hatanaka
 
-import subprocess
+from geodezyx import conv
+from geodezyx import files_rw
+#### Import star style
+from geodezyx import operational
+from geodezyx import utils
 
-#### Import the logger
-import logging
 log = logging.getLogger(__name__)
 
 def run_command(command):
     # Run the command and capture both stdout and stderr
     process = subprocess.Popen([command],
                                stdout=subprocess.PIPE,
                                stderr=subprocess.STDOUT,
```

### Comparing `geodezyx-4.4.2/geodezyx/operational/rinex_lister_plotter.py` & `geodezyx-4.4.3/geodezyx/operational/rinex_lister_plotter.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,27 +15,28 @@
 GitHub repository :
 https://github.com/GeodeZYX/geodezyx-toolbox
 """
 
 ########## BEGIN IMPORT ##########
 #### External modules
 import datetime as dt
+#### Import the logger
+import logging
+import os
+import re
+
 import matplotlib.pyplot as plt
 import numpy as np
-import os 
-import re
 import tabulate
 
 #### geodeZYX modules
 from geodezyx import conv
 from geodezyx import operational
 from geodezyx import utils
 
-#### Import the logger
-import logging
 log = logging.getLogger(__name__)
 
 ##########  END IMPORT  ##########
 
 def rinex_lister(path,add_long_names=True):
     """
     find all rinex in a folder and his subfolders
```

### Comparing `geodezyx-4.4.2/geodezyx/operational/rinex_utils.py` & `geodezyx-4.4.3/geodezyx/operational/rinex_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,31 +16,32 @@
 GitHub repository :
 https://github.com/GeodeZYX/geodezyx-toolbox
 """
 
 ########## BEGIN IMPORT ##########
 #### External modules
 import datetime as dt
-import dateutil
 import glob
-import numpy as np
-import os 
-import pandas as pd
+#### Import the logger
+import logging
+import os
+import re
 import shutil
 import string
 import subprocess
-import re
+
+import dateutil
 import hatanaka
+import numpy as np
+import pandas as pd
 
 #### geodeZYX modules
 from geodezyx import conv
 from geodezyx import utils
 
-#### Import the logger
-import logging
 log = logging.getLogger(__name__)
 
 ##########  END IMPORT  ##########
 
 
 
 def rinexs_table_from_list(rnxs_inp,
```

### Comparing `geodezyx-4.4.2/geodezyx/operational/rtklib_frontend.py` & `geodezyx-4.4.3/geodezyx/operational/rtklib_frontend.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,28 +14,28 @@
 
 Copyright (C) 2019 Pierre Sakic et al. (IPGP, sakic@ipgp.fr)
 GitHub repository :
 https://github.com/GeodeZYX/geodezyx-toolbox
 """
 
 
+import collections
 ########## BEGIN IMPORT ##########
 #### External modules
 import datetime as dt
-import os 
+#### Import the logger
+import logging
+import os
 import subprocess
-import collections
 
 #### geodeZYX modules
 from geodezyx import files_rw
 from geodezyx import operational
 from geodezyx import utils
 
-#### Import the logger
-import logging
 log = logging.getLogger(__name__)
 
 ##########  END IMPORT  ##########
 
 
 def read_conf_file(filein):
     outdic = collections.OrderedDict()
```

### Comparing `geodezyx-4.4.2/geodezyx/operational/track_frontend.py` & `geodezyx-4.4.3/geodezyx/operational/track_frontend.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,26 +19,26 @@
 
 
 
 ########## BEGIN IMPORT ##########
 #### External modules
 import datetime as dt
 import glob
-import os 
+#### Import the logger
+import logging
+import os
 import shutil
 import subprocess
 
 #### geodeZYX modules
 from geodezyx import conv
 from geodezyx import files_rw
 from geodezyx import operational
 from geodezyx import utils
 
-#### Import the logger
-import logging
 log = logging.getLogger(__name__)
 
 ##########  END IMPORT  ##########
 
 def track_runner(rnx_rover,rnx_base,working_dir,experience_prefix,
                  XYZbase  = [], XYZrover = [] , outtype = 'XYZ',mode = 'short',
                  interval=None,antmodfile = "~/gg/tables/antmod.dat",
```

### Comparing `geodezyx-4.4.2/geodezyx/reffram/geometry.py` & `geodezyx-4.4.3/geodezyx/reffram/geometry.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -16,26 +16,26 @@
 GitHub repository :
 https://github.com/GeodeZYX/geodezyx-toolbox
 """
 
 ########## BEGIN IMPORT ##########
 #### External modules
 import io
-import pandas as pd
+#### Import the logger
+import logging
+
 import numpy as np
+import pandas as pd
 import scipy
 
-
 #### geodeZYX modules
 from geodezyx import conv
 from geodezyx import stats
 from geodezyx import utils
 
-#### Import the logger
-import logging
 log = logging.getLogger(__name__)
 
 ##########  END IMPORT  ##########
 
 
 #  _    _ _       _       _                    _    _____                _      _   _        ______   _       
 # | |  | (_)     | |     | |                  | |  / ____|              | |    | | (_)      |  ____| | |
```

### Comparing `geodezyx-4.4.2/geodezyx/reffram/gnss_products.py` & `geodezyx-4.4.3/geodezyx/reffram/gnss_products.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,36 +18,35 @@
 https://github.com/GeodeZYX/geodezyx-toolbox
 """
 
 ########## BEGIN IMPORT ##########
 #### External modules
 import datetime as dt
 import itertools
+#### Import the logger
+import logging
+import os
+import re
+
 import matplotlib
 import matplotlib.pyplot as plt
 import natsort
 import numpy as np
-import os 
 import pandas as pd
-import re
-
 import pyorbital.astronomy
 
-### disabled and imported directly in the needed fct
-## import geodezyx.reffram.sofa18 as sofa
-
 #### geodeZYX modules
 from geodezyx import conv
 from geodezyx import files_rw
 from geodezyx import stats
 from geodezyx import utils
 from geodezyx.reffram import kepler_gzyx
 
-#### Import the logger
-import logging
+### disabled and imported directly in the needed fct
+## import geodezyx.reffram.sofa18 as sofa
 log = logging.getLogger(__name__)
 
 ##########  END IMPORT  ##########
 
 def compar_orbit(Data_inp_1,Data_inp_2,step_data = 900,
                  sats_used_list = ['G'],
                  name1='',name2='',use_name_1_2_for_table_name = False,
@@ -67,15 +66,14 @@
         per default data sampling
 
     sats_used_list : list of str
         used constellation or satellite : G E R C ... E01 , G02 ...
         Individuals satellites are prioritary on whole constellations
         e.g. ['G',"E04"]
 
-
     RTNoutput : bool
         select output, Radial Transverse Normal or XYZ
 
     convert_ECEF_ECI : bool
         convert sp3 ECEF => ECI (Terrestrial => Celestrial)
         must be True in operational to avoid artifacts.
 
@@ -117,23 +115,23 @@
     References
     ----------
     "Coordinate Systems", ASEN 3200 1/24/06 George H. Born
 
     """
 
     # selection of both used Constellations AND satellites
-    const_used_list = []
-    sv_used_list    = []
-    for sat in sats_used_list:
-        if len(sat) == 1:
-            const_used_list.append(sat)
-        elif len(sat) == 3:
-            sv_used_list.append(sat)
-            if not sat[0] in const_used_list:
-                const_used_list.append(sat[0])
+    sys_used_list = []
+    prn_used_list  = []
+    for e in sats_used_list:
+        if len(e) == 1: ## it is a constellation
+            sys_used_list.append(e)
+        elif len(e) == 3: ## it is a satellite
+            prn_used_list.append(e)
+            if not e[0] in sys_used_list:
+                sys_used_list.append(e[0])
 
     # Read the files or DataFrames
     # metadata attributes are not copied
     # Thus, manual copy ...
     # (Dirty way, should be impoved without so many lines ...)
     if type(Data_inp_1) is str:
         D1orig = files_rw.read_sp3(Data_inp_1,epoch_as_pd_index=True)
@@ -197,133 +195,142 @@
 
         D1 = D1orig[np.logical_not(D1_null_bool)]
         D2 = D2orig[np.logical_not(D2_null_bool)]
 
         if np.any(D1_null_bool) or np.any(D2_null_bool):
             sat_nul = utils.join_improved(" " ,*list(set(D1orig[D1_null_bool]["prn"])))
             log.warning("Null values contained in SP3 files : ")
-            log.warning("f1: %s %s" , np.sum(D1_null_bool) , utils.join_improved(" " , *list(set(D1orig[D1_null_bool]["prn"]))))
-            log.warning("f2: %s %s" , np.sum(D2_null_bool) , utils.join_improved(" " , *list(set(D2orig[D2_null_bool]["prn"]))))
+            log.warning("f1: %s %s", np.sum(D1_null_bool),
+                        utils.join_improved(" ", *list(set(D1orig[D1_null_bool]["prn"]))))
+            log.warning("f2: %s %s", np.sum(D2_null_bool),
+                        utils.join_improved(" ", *list(set(D2orig[D2_null_bool]["prn"]))))
         else:
             sat_nul = []
 
     else:
         D1 = D1orig.copy()
         D2 = D2orig.copy()
 
-    for constuse in const_used_list:
-        D1const = D1[D1['sys'] == constuse]
-        D2const = D2[D2['sys'] == constuse]
+    D1sys_grp = D1.groupby("sys")
+    D2sys_grp = D2.groupby("sys")
+
+    for sysuse in sys_used_list:
+        D1sys = D1sys_grp.get_group(sysuse) # D1sys = D1[D1['sys'] == sysuse]
+        D2sys = D2sys_grp.get_group(sysuse) # D2sys = D2[D2['sys'] == sysuse]
 
         # checking if the data correspond to the step
-        bool_step1 = np.mod((D1const.index - np.min(D1.index)).seconds,step_data) == 0
-        bool_step2 = np.mod((D2const.index - np.min(D2.index)).seconds,step_data) == 0
+        bool_step1 = np.mod((D1sys.index - np.min(D1.index)).seconds,step_data) == 0
+        bool_step2 = np.mod((D2sys.index - np.min(D2.index)).seconds,step_data) == 0
 
-        D1window = D1const[bool_step1]
-        D2window = D2const[bool_step2]
+        D1win = D1sys[bool_step1]
+        D2win = D2sys[bool_step2]
         
         # find common sats and common epochs
-        sv_set   = sorted(list(set(D1window['prni']).intersection(set(D2window['prni']))))
-        epoc_set = sorted(list(set(D1window.index).intersection(set(D2window.index))))
+        prni_set = sorted(list(set(D1win['prni']).intersection(set(D2win['prni']))))
+        epoc_set = sorted(list(set(D1win.index).intersection(set(D2win.index))))
 
         # if special selection of sats, then apply it
         # (it is late and this selection is incredibely complicated ...)
-        if np.any([True  if constuse in e else False for e in sv_used_list]):
+        if np.any([True if sysuse in e else False for e in prn_used_list]):
             # first find the selected sats for the good constellation
-            sv_used_select_list = [int(e[1:]) for e in sv_used_list if constuse in e]
-            #and apply it
-            sv_set = sorted(list(set(sv_set).intersection(set(sv_used_select_list))))
+            prni_used_select_list = [int(e[1:]) for e in prn_used_list if sysuse in e]
+            # and apply it
+            prni_set = sorted(list(set(prni_set).intersection(set(prni_used_select_list))))
+
+        D1win_prni_grp = D1win.groupby("prni")
+        D2win_prni_grp = D2win.groupby("prni")
 
-        for svv in sv_set:
+        for prni in prni_set:
             # First research : find corresponding epoch for the SV
             # this one is sufficent if there is no gaps (e.g. with 0.00000) i.e.
             # same nb of obs in the 2 files
             # NB : .reindex() is smart, it fills the DataFrame
             # with NaN
             try:
-                D1sv_orig = D1window[D1window['prni'] == svv].reindex(epoc_set)
-                D2sv_orig = D2window[D2window['prni'] == svv].reindex(epoc_set)
+                D1prni_orig = D1win_prni_grp.get_group(prni).reindex(epoc_set)
+                # D1win[D1win['prni'] == prni].reindex(epoc_set)
+                D2prni_orig = D2win_prni_grp.get_group(prni).reindex(epoc_set)
+                # D2win[D2win['prni'] == prni].reindex(epoc_set)
             except Exception as exce:
                 log.info("ERR : Unable to re-index with an unique epoch")
                 log.info("      are you sure there is no multiple-defined epochs for the same sat ?")
                 log.info("      it happens e.g. when multiple ACs are in the same DataFrame ")
                 log.info("TIP : Filter the input Dataframe before calling this fct with")
                 log.info("      DF = DF[DF['AC'] == 'gbm']")
                 
-                Dtmp1 = D1orig[D1orig['prni'] == svv]
-                Dtmp2 = D2orig[D2orig['prni'] == svv]
+                Dtmp1 = D1orig[D1orig['prni'] == prni]
+                Dtmp2 = D2orig[D2orig['prni'] == prni]
                 
                 dupli1 = np.sum(Dtmp1.duplicated(["epoch","prn"]))
                 dupli2 = np.sum(Dtmp2.duplicated(["epoch","prn"]))
                 
                 log.info("FWIW: duplicated epoch/sat in DF1 & DF2: %s %s",dupli1,dupli2)
 
                 raise exce
 
             # Second research, it is a security in case of gap
             # This step is useless, because .reindex() will fill the DataFrame
             # with NaN
-            if len(D1sv_orig) != len(D2sv_orig):
-                log.info("different epochs nbr for SV %s %s %s",svv,len(D1sv_orig),len(D2sv_orig))
-                epoc_sv_set = sorted(list(set(D1sv_orig.index).intersection(set(D2sv_orig.index))))
-                D1sv = D1sv_orig.loc[epoc_sv_set]
-                D2sv = D2sv_orig.loc[epoc_sv_set]
+            if len(D1prni_orig) != len(D2prni_orig):
+                log.info("different epochs nbr for SV %s %s %s",prni, len(D1prni_orig), len(D2prni_orig))
+                epoc_prni_set = sorted(list(set(D1prni_orig.index).intersection(set(D2prni_orig.index))))
+                D1prni = D1prni_orig.loc[epoc_prni_set]
+                D2prni = D2prni_orig.loc[epoc_prni_set]
             else:
-                D1sv = D1sv_orig
-                D2sv = D2sv_orig
+                D1prni = D1prni_orig
+                D2prni = D2prni_orig
 
-            P1     = D1sv[['x','y','z']]
-            P2     = D2sv[['x','y','z']]
+            P1 = D1prni[['x','y','z']]
+            P2 = D2prni[['x','y','z']]
 
             # Start ECEF => ECI
             if convert_ECEF_ECI:
                 # Backup because the columns xyz will be reaffected
-                #D1sv_bkp = D1sv.copy()
-                #D2sv_bkp = D2sv.copy()
+                #D1sv_bkp = D1prni.copy()
+                #D2sv_bkp = D2prni.copy()
     
                 P1b = conv.ECEF2ECI(np.array(P1),conv.dt_gpstime2dt_utc(P1.index.to_pydatetime(),out_array=True))
                 P2b = conv.ECEF2ECI(np.array(P2),conv.dt_gpstime2dt_utc(P2.index.to_pydatetime(),out_array=True))
 
-                D1sv[['x','y','z']] = P1b
-                D2sv[['x','y','z']] = P2b
+                D1prni[['x','y','z']] = P1b
+                D2prni[['x','y','z']] = P2b
 
-                P1  = D1sv[['x','y','z']]
-                P2  = D2sv[['x','y','z']]
+                P1 = D1prni[['x','y','z']]
+                P2 = D2prni[['x','y','z']]
             # End ECEF => ECI
 
             if not RTNoutput:
                 # Compatible with the documentation +
                 # empirically tested with OV software
                 # it is  P1 - P2 (and not P2 - P1)
                 Delta_P = P1 - P2
 
-
                 Diff_sat = Delta_P.copy()
                 Diff_sat.columns = ['dx','dy','dz']
 
             else:
                 rnorm = np.linalg.norm(P1,axis=1)
 
-                Vx = utils.diff_pandas(D1sv,'x')
-                Vy = utils.diff_pandas(D1sv,'y')
-                Vz = utils.diff_pandas(D1sv,'z')
-
-                V =  pd.concat((Vx , Vy , Vz),axis=1)
+                Vx = utils.diff_pandas(D1prni,'x',use_np_diff=False)
+                Vy = utils.diff_pandas(D1prni,'y',use_np_diff=False)
+                Vz = utils.diff_pandas(D1prni,'z',use_np_diff=False)
+                
+                V = pd.concat((Vx , Vy , Vz),axis=1)
                 V.columns = ['vx','vy','vz']
 
                 R = P1.divide(rnorm,axis=0)
                 R.columns = ['xnorm','ynorm','znorm']
 
-                H      = pd.DataFrame(np.cross(R,V),columns=['hx','hy','hz'])
-                hnorm  = np.linalg.norm(H,axis=1)
+                H = pd.DataFrame(np.cross(R,V),columns=['hx','hy','hz'])
+                hnorm = np.linalg.norm(H,axis=1)
 
-                C         = H.divide(hnorm,axis=0)
+                C = H.divide(hnorm,axis=0)
                 C.columns = ['hxnorm','hynorm','hznorm']
 
-                I         = pd.DataFrame(np.cross(C,R),columns=['ix','iy','iz'])
+                I = pd.DataFrame(np.cross(C,R),columns=['ix','iy','iz'])
 
                 R_ar = np.array(R)
                 I_ar = np.array(I)
                 C_ar = np.array(C)
 
                 #R_ar[1]
                 Beta = np.stack((R_ar,I_ar,C_ar),axis=1)
@@ -337,21 +344,22 @@
                 Astk = []
 
                 for i in range(len(Delta_P)):
                     A = np.dot(Beta[i,:,:],np.array(Delta_P)[i])
                     Astk.append(A)
 
                 Diff_sat = pd.DataFrame(np.vstack(Astk),
-                                   index = P1.index,columns=['dr','dt','dn'])
+                                        index = P1.index,
+                                        columns=['dr','dt','dn'])
 
             Diff_sat = Diff_sat * conv_coef # metrer conversion
 
-            Diff_sat['sys'] = [constuse] * len(Diff_sat.index)
-            Diff_sat['prni']    = [svv]      * len(Diff_sat.index)
-            Diff_sat['prn']   = [constuse + str(svv).zfill(2)] * len(Diff_sat.index)
+            Diff_sat['sys'] = [sysuse] * len(Diff_sat.index)
+            Diff_sat['prni'] = [prni] * len(Diff_sat.index)
+            Diff_sat['prn'] = [sysuse + str(prni).zfill(2)] * len(Diff_sat.index)
 
             Diff_sat_stk.append(Diff_sat)
 
     Diff_sat_all = pd.concat(Diff_sat_stk)
     Date = Diff_sat.index[0]
 
     # Attribute definition
@@ -372,15 +380,14 @@
         Diff_sat_all.frame_col_name3 = 'dz'
 
         if convert_ECEF_ECI:
             Diff_sat_all.frame_type = 'ECI'
         else:
             Diff_sat_all.frame_type = 'ECEF'
 
-
     # Name definitions
     if name1:
         Diff_sat_all.name1 = name1
     else:
         Diff_sat_all.name1 = D1orig.name
 
     if name2:
@@ -394,15 +401,14 @@
     Diff_sat_all.path1 = D1orig.path
     Diff_sat_all.path2 = D2orig.path
 
     Diff_sat_all.name = ' '.join(('Orbits comparison ('+Diff_sat_all.frame_type +') b/w',
                                   Diff_sat_all.name1 ,'(ref.) and',
                                   Diff_sat_all.name2 ,',',Date.strftime("%Y-%m-%d"),
                                   ', doy', str(conv.dt2doy(Date))))
-
     
     if return_satNull:
         return Diff_sat_all, sat_nul
     else:
         return Diff_sat_all
 
 
@@ -433,15 +439,14 @@
     Returns
     -------
     the Figure and the 3 Axes if no save is asked
     export path (str) if save is asked
     but plot a plot anyway
     """
 
-    import matplotlib.dates as mdates
     fig,[axr,axt,axn] = plt.subplots(3,1,sharex='all')
 
     satdispo = natsort.natsorted(list(set(Diff_sat_all_df_in['prn'])))
 
     SymbStk = []
 
     cm = plt.get_cmap('viridis')
@@ -816,17 +821,15 @@
 
     Returns
     -------
     the Figure and the 3 Axes if no save is asked
     export path (str) if save is asked
     but plot a plot anyway
     """
-    
-    
-    import matplotlib.dates as mdates
+
     fig,axr = plt.subplots(1,1,sharex='all')
     Diff_sat_all_df_in = Diff_sat_all_df_in.reset_index()
     satdispo = natsort.natsorted(list(set(Diff_sat_all_df_in[col_name])))
     # satdispo = natsort.natsorted(list(set(Diff_sat_all_df_in['sat'])))
        
     SymbStk = []
        
@@ -1466,49 +1469,82 @@
     OrbDFwrk = OrbDFin.reset_index()
     OrbDFwrk = OrbDFwrk.sort_values(index_order)
     OrbDFwrk["sys"] = OrbDFwrk["prn"].apply(lambda x: x[0])
     OrbDFwrk["prni"] = OrbDFwrk["prn"].apply(lambda x: int(x[1:]))
     return OrbDFwrk
 
 def OrbDF_common_epoch_finder(OrbDFa_in,OrbDFb_in,return_index=False,
-                              supplementary_sort=False,order=["prn","epoch"]):
+                          supplementary_sort=False,order=["prn","epoch"],
+                          skip_reg2multidx_OrbDFa=False,
+                          skip_reg2multidx_OrbDFb=False):
     """
-    Find common sats and epochs in to Orbit DF,
-    and output the corresponding Orbit DFs
-    order >> normally for sp3 is sat and epoch, 
-    but can be used for snx files as STAT and epoch
-    """
-    
-    OrbDFa = OrbDF_reg_2_multidx(OrbDFa_in,index_order = order)
-    OrbDFb = OrbDF_reg_2_multidx(OrbDFb_in,index_order = order)
-    
+    This function finds common satellites and epochs in two Orbit DataFrames and outputs the corresponding Orbit DataFrames.
+
+    Parameters
+    ----------
+    OrbDFa_in : DataFrame
+        The first input Orbit DataFrame.
+    OrbDFb_in : DataFrame
+        The second input Orbit DataFrame.
+    return_index : bool, optional
+        If True, the function also returns the common index. Default is False.
+    supplementary_sort : bool, optional
+        If True, an additional sort is performed. This is useful for multi GNSS where the output DataFrame may not be well sorted. Default is False.
+    order : list of str, optional
+        The order of the index for the multi-index DataFrame. Default is ["prn","epoch"].
+    skip_reg2multidx_OrbDFa : bool, optional
+        If True, skips the conversion of the first input DataFrame to a multi-index DataFrame. Default is False.
+        The inputs are assumed to be already in multi-index format to optimize execution speed.
+        (For advanced use only)
+    skip_reg2multidx_OrbDFb : bool, optional
+        If True, skips the conversion of the second input DataFrame to a multi-index DataFrame. Default is False.
+        The inputs are assumed to be already in multi-index format to optimize execution speed.
+        (For advanced use only)
+
+    Returns
+    -------
+    OrbDFa_out : DataFrame
+        The first output Orbit DataFrame with common satellites and epochs.
+    OrbDFb_out : DataFrame
+        The second output Orbit DataFrame with common satellites and epochs.
+    Iinter : Index, optional
+        The common index. Only returned if return_index is True.
+
+    Note
+    ----
+    designed for orbits/sp3 first with sat and epoch as order parmeter,
+    but can be used also for instance for snx files with
+    STAT and epoch as order parmeter
+    """
+    if not skip_reg2multidx_OrbDFa:
+        OrbDFa = OrbDF_reg_2_multidx(OrbDFa_in,index_order = order)
+    else:
+        OrbDFa = OrbDFa_in
+    if not skip_reg2multidx_OrbDFb:
+        OrbDFb = OrbDF_reg_2_multidx(OrbDFb_in,index_order = order)
+    else:
+        OrbDFb = OrbDFb_in
+
     I1 = OrbDFa.index
     I2 = OrbDFb.index
-    
+
     Iinter = I1.intersection(I2)
-    ### A sort of the Index to avoid issues ...
     Iinter = Iinter.sort_values()
-    
+
     OrbDFa_out = OrbDFa.loc[Iinter]
     OrbDFb_out = OrbDFb.loc[Iinter]
-    
+
     if supplementary_sort:
-        # for multi GNSS, OrbDF_out are not well sorted (why ??? ...)
-        # we do a supplementary sort
-        # NB 202003: maybe because Iiter was not sorted ...
-        # should be fixed with the Iinter.sort_values() above 
-        # but we maintain this sort
         OrbDFa_out = OrbDFa_out.sort_values(order)
         OrbDFb_out = OrbDFb_out.sort_values(order)
 
-    
     if len(OrbDFa_out) != len(OrbDFb_out):
         log.warning("len(Orb/ClkDFa_out) != len(Orb/ClkDFb_out)")
         log.warning("TIPS : ClkDFa_in and/or ClkDFb_in might contain duplicates")
-    
+
     if return_index:
         return OrbDFa_out , OrbDFb_out , Iinter
     else:
         return OrbDFa_out , OrbDFb_out
 
 
 def OrbDF_const_sv_columns_maker(OrbDFin,inplace=True):
@@ -1528,15 +1564,15 @@
  #   _____ _            _      _____        _        ______                              
  #  / ____| |          | |    |  __ \      | |      |  ____|                             
  # | |    | | ___   ___| | __ | |  | | __ _| |_ __ _| |__ _ __ __ _ _ __ ___   ___  ___  
  # | |    | |/ _ \ / __| |/ / | |  | |/ _` | __/ _` |  __| '__/ _` | '_ ` _ \ / _ \/ __| 
  # | |____| | (_) | (__|   <  | |__| | (_| | || (_| | |  | | | (_| | | | | | |  __/\__ \ 
  #  \_____|_|\___/ \___|_|\_\ |_____/ \__,_|\__\__,_|_|  |_|  \__,_|_| |_| |_|\___||___/ 
                                                                                                                                                                         
-### Clock DataFrames   
+### Clock DataFrames
 
 def ClkDF_filter(ClkDF_in,
              typ=("AS","AR"),
              name=None,
              ac=None,
              epoch_strt=dt.datetime(1980,1,1),
              epoch_end=dt.datetime(2099,1,1),
@@ -1608,14 +1644,70 @@
         
     ##epoch
     BOOLtmp = (epoch_strt <= ClkDF_wrk.epoch) & (ClkDF_wrk.epoch < epoch_end)
     BOOL    = BOOL & np.array(BOOLtmp)    
     
     return ClkDF_wrk[BOOL]
 
+def ClkDF_filter2(ClkDF_in,
+             typ=("AS","AR"),
+             name=None,
+             ac=None,
+             epoch_strt=dt.datetime(1980,1,1),
+             epoch_end=dt.datetime(2099,1,1),
+             name_regex=False):
+    """
+    attempt for a faster version of ClkDF_filter, but the original is faster
+    """
+    
+    if type(ClkDF_in) is str:
+        ClkDF_wrk = utils.pickle_loader(ClkDF_in)
+    else:
+        ClkDF_wrk = ClkDF_in
+        
+    clkdf_stk = []
+    
+    for (ityp, iname, iac), clkdf_grp in ClkDF_wrk.groupby(["type","name","ac"]):
+        if typ:
+            bool_typ = True if ityp in typ else False
+        else:
+            bool_typ = True
+        
+        if name:
+            if not name_regex:
+                bool_name = True if iname in name else False
+            else:
+                bool_name = any([re.search(n, iname) for n in name])
+        else:
+            bool_name = True
+            
+        if ac:
+            bool_ac = True if iac in ac else False
+        else:
+            bool_ac = True
+            
+        
+        if not (bool_typ and bool_name and bool_ac):
+            continue
+        else:
+            if epoch_strt > dt.datetime(1980,1,1) or epoch_end < dt.datetime(2099,1,1):
+                bool_epoc = (epoch_strt <= clkdf_grp["epoch"]) & (clkdf_grp["epoch"] < epoch_end)
+                clkdf_stk.append(clkdf_grp[bool_epoc])
+            else:
+                clkdf_stk.append(clkdf_grp)
+
+                
+            
+    clkdf_out = pd.concat(clkdf_stk)
+    
+    return clkdf_out
+                
+            
+
+
 def ClkDF_reg_2_multidx(ClkDFin,index_order=["name","epoch"]):
     """
     From an regular Clock DF generated by read_clk(), set some columns 
     (typically ["name","epoch"]) as indexes
     The outputed DF is then a Multi-index DF
     
     It an adapted version of OrbDF_reg_2_multidx
```

### Comparing `geodezyx-4.4.2/geodezyx/reffram/kepler_gzyx.py` & `geodezyx-4.4.3/geodezyx/reffram/kepler_gzyx.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,27 +13,28 @@
 functions for Geodesy and Geophysics under the GNU LGPL v3 License
 
 Copyright (C) 2019 Pierre Sakic et al. (IPGP, sakic@ipgp.fr)
 GitHub repository :
 https://github.com/GeodeZYX/geodezyx-toolbox
 """
 
+import datetime as dt
+#### Import the logger
+import logging
+
 ########## BEGIN IMPORT ##########
 #### External modules
 import numpy as np
 import pandas as pd
-import datetime as dt
-#from pytwobodyorbit import TwoBodyOrbit
-from pytwobodyorbit import TwoBodyOrbit  
+# from pytwobodyorbit import TwoBodyOrbit
+from pytwobodyorbit import TwoBodyOrbit
 
 #### geodeZYX modules
 from geodezyx import conv
 
-#### Import the logger
-import logging
 log = logging.getLogger(__name__)
 
 ##########  END IMPORT  ##########
 
 
 def ECI_2_kepler_elts(pos,vel,rad2deg=True,
                       mu=3.9860044188e14):
```

### Comparing `geodezyx-4.4.2/geodezyx/reffram/quaternions.py` & `geodezyx-4.4.3/geodezyx/reffram/quaternions.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 #### External modules
 import numpy as np
 from scipy.spatial.transform import Rotation
 
 #### geodeZYX modules
 from geodezyx import utils
 
+
 ##########  END IMPORT  ##########
 
 
 #   ____              _                  _
 #  / __ \            | |                (_)
 # | |  | |_   _  __ _| |_ ___ _ __ _ __  _  ___  _ __  ___
 # | |  | | | | |/ _` | __/ _ \ '__| '_ \| |/ _ \| '_ \/ __|
```

### Comparing `geodezyx-4.4.2/geodezyx/stats/least_squares.py` & `geodezyx-4.4.3/geodezyx/stats/least_squares.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,27 +12,28 @@
 functions for Geodesy and Geophysics under the GNU LGPL v3 License
 
 Copyright (C) 2019 Pierre Sakic et al. (IPGP, sakic@ipgp.fr)
 GitHub repository :
 https://github.com/GeodeZYX/geodezyx-toolbox
 """
 
+import itertools
+#### Import the logger
+import logging
+import multiprocessing as mp
+
+import matplotlib.pyplot as plt
 ########## BEGIN IMPORT ##########
 #### External modules
 import numpy as np
 import scipy
-import itertools
-import multiprocessing as mp
-import matplotlib.pyplot as plt
 
 #### geodeZYX modules
 from geodezyx import utils
 
-#### Import the logger
-import logging
 log = logging.getLogger(__name__)
 
 ##########  END IMPORT  ##########
 
 
 
 #  _                    _      _____                  _    _ _   _ _
```

### Comparing `geodezyx-4.4.2/geodezyx/stats/stats.py` & `geodezyx-4.4.3/geodezyx/stats/stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,92 +16,94 @@
 https://github.com/GeodeZYX/geodezyx-toolbox
 """
 
 
 ########## BEGIN IMPORT ##########
 #### External modules
 import datetime as dt
+#### Import the logger
+import logging
+
+import matplotlib.pyplot as plt
 import numpy as np
 import scipy
-import matplotlib.pyplot as plt
+
 #### geodeZYX modules
 from geodezyx import conv
 from geodezyx import utils
 
-
-#### Import the logger
-import logging
 log = logging.getLogger(__name__)
 
 ##########  END IMPORT  ##########
 
 
 
-def linear_regression(x,y,fulloutput=False,alpha=.95):
-    """    
-    From 2 vectors X and Y, returns linear regression coefficients a and b
+def linear_regression(x, y, fulloutput=False, simple_lsq=False, alpha=.95):
+    """
+    Performs linear regression on two vectors, X and Y, and returns the coefficients a (slope) and b (intercept).
 
     Parameters
     ----------
-    X & Y : list or numpy.array
-        Values
+    x : list or numpy.array
+        The X values.
+    y : list or numpy.array
+        The Y values.
+    simple_lsq : bool, optional
+        If True, performs a basic, low-level least square inversion (faster, but less outputs).
+        If False, calls scipy's linregress. Default is False.
+    fulloutput : bool, optional
+        If True, returns additional outputs (confidence interval for the slope and standard deviation).
+        Default is False.
+    alpha : float, optional
+        The alpha value for the confidence interval. Default is .95.
 
-    fulloutput : bool
-        full output
-        
-    alpha : float
-        alpha value for the confidence interval
-                
     Returns
     -------
-    a & b : float
-        Linear regression coefficients
-    
-    If fulloutput == True:
-        
-    confid_interval_slope : float 2-tuple
-        confidence interval for the slope
-        
-    std_err : float
-        standard deviation
-        
-    Note
-    ----
-    http://glowingpython.blogspot.fr/2012/03/linear-regression-with-numpy.html 
-    
-    This function is doing more or less the same job as scipy.stats.linregress
-    """
+    slope : float
+        The slope (a) of the linear regression.
+    intercept : float
+        The intercept (b) of the linear regression.
+    confid_interval_slope : tuple of float, optional
+        The confidence interval for the slope. Only returned if fulloutput is True.
+    std_err : float, optional
+        The standard deviation. Only returned if fulloutput is True.
+
+    Notes
+    -----
+    This function performs a similar job to scipy.stats.linregress.
 
-    # On bosse avec des arrays
-    x = np.array(x)
-    y = np.array(y)
+    Regarding computation speed: low-level least square inversion is faster for small datasets.
+    For larger datasets, scipy's linregress is faster (n points > ~13000).
 
-    if len(x) != len(y):
-        log.error("ERR : linear_regression : len(x) != len(y)")
-        log.info("      len(x) : " , len(x))
-        log.info("      len(y) : " , len(y))
-
-        return 0,0
-
-    A = np.array([x, np.ones(len(x))])
-    # linearly generated sequence
-    #### Too slow approach
-    ## https://www.freecodecamp.org/news/data-science-with-python-8-ways-to-do-linear-regression-and-measure-their-speed-b5577d75f8b/
-    ## w = np.linalg.lstsq(A.T,y,rcond=None)[0] # obtaining the parameters
-    
-    slope, intercept, r_value, p_value, std_err = scipy.stats.linregress(x,y)
+    """
+    # Ensure x and y are numpy arrays
+    if not isinstance(x, np.ndarray):
+        x = np.array(x)
+    if not isinstance(y, np.ndarray):
+        y = np.array(y)
 
-    if not fulloutput:
-        #return w[0],w[1]
-        return slope, intercept
+    # Check if lengths of x and y are equal
+    if len(x) != len(y):
+        log.error("len(x) (%i) != len(y) (%i)", len(x), len(y))
+        return 0, 0
 
+    # Perform least squares regression if simple_lsq is True
+    if simple_lsq:
+        A = np.array([x, np.ones(len(x))]) # x2 faster than np.column_stack([x, np.ones(len(x))])
+        slope, intercept = np.linalg.lstsq(A.T, y, rcond=None)[0]  # obtaining the parameters
     else:
-        #slope, intercept, r_value, p_value, std_err = scipy.stats.linregress(x,y)
-        return slope,intercept,confid_interval_slope(x,y,alpha),std_err
+        # Perform scipy's linregress if simple_lsq is False
+        slope, intercept, r_value, p_value, std_err = scipy.stats.linregress(x, y)
 
+    # Return only the slope and intercept if fulloutput is False
+    if simple_lsq or not fulloutput:
+        return slope, intercept
+    else:
+        # Return the slope, intercept, confidence interval, and standard deviation if fulloutput is True
+        return slope, intercept, confid_interval_slope(x, y, alpha), std_err
 
 def linear_reg_getvalue(X,a,b,full=True):
     """    
     From a vector X and coefficients a & b, get Y = a*X + b
 
     Parameters
     ----------
```

### Comparing `geodezyx-4.4.2/geodezyx/time_series/ts_class.py` & `geodezyx-4.4.3/geodezyx/time_series/ts_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 # -*- coding: utf-8 -*-
 """
 Created on Fri Aug  2 13:55:33 2019
 
 @author: psakicki
 """
 
+import copy
+import datetime as dt
+#### Import the logger
+import logging
+import os
 ########## BEGIN IMPORT ##########
 #### External modules
 from collections import Counter
-import copy
-import datetime as dt
+
 import matplotlib
 import matplotlib.pyplot as plt
-from matplotlib.widgets import MultiCursor
 import numpy as np
 import pandas as pd
-import os 
 import scipy
+from matplotlib.widgets import MultiCursor
 
 #### geodeZYX modules
 from geodezyx import conv
 from geodezyx import files_rw
+from geodezyx import reffram
 from geodezyx import stats
-from geodezyx import utils
 from geodezyx import time_series
-from geodezyx import reffram
+from geodezyx import utils
 
-#### Import the logger
-import logging
 log = logging.getLogger(__name__)
 log.setLevel(logging.INFO)
 
 ##########  END IMPORT  ##########
 
 class Point():
```

### Comparing `geodezyx-4.4.2/geodezyx/time_series/ts_export.py` & `geodezyx-4.4.3/geodezyx/time_series/ts_export.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,23 +5,24 @@
 
 @author: psakicki
 """
 
 ########## BEGIN IMPORT ##########
 #### External modules
 import copy
+#### Import the logger
+import logging
+import os
+
 import matplotlib.pyplot as plt
-import os 
 
 #### geodeZYX modules
 from geodezyx import conv
-from geodezyx import time_series 
+from geodezyx import time_series
 
-#### Import the logger
-import logging
 log = logging.getLogger(__name__)
 
 ##########  END IMPORT  ##########
 
 def export_ts_figure_pdf(fig,export_path,filename,close=False):
     """ fig can accept a int (id of a Figure)
          OR the figure Object itself """
```

### Comparing `geodezyx-4.4.2/geodezyx/time_series/ts_fcts.py` & `geodezyx-4.4.3/geodezyx/time_series/ts_fcts.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 @author: psakicki
 """
 
 ########## BEGIN IMPORT ##########
 #### External modules
 import copy
 import datetime as dt
+import itertools
+#### Import the logger
+import logging
+
 import matplotlib.pyplot as plt
 import numpy as np
-import os 
 import scipy
-import itertools
 
 #### geodeZYX modules
 from geodezyx import conv
+from geodezyx import reffram
 from geodezyx import stats
-from geodezyx import utils
 from geodezyx import time_series
-from geodezyx import reffram
+from geodezyx import utils
 
-#### Import the logger
-import logging
 log = logging.getLogger(__name__)
 
 ##########  END IMPORT  ##########
 
 
 
 def print4compar(dA,dB,dC,dD,coortype):
```

### Comparing `geodezyx-4.4.2/geodezyx/utils/dict_utils.py` & `geodezyx-4.4.3/geodezyx/utils/dict_utils.py`

 * *Files identical despite different names*

### Comparing `geodezyx-4.4.2/geodezyx/utils/list_utils.py` & `geodezyx-4.4.3/geodezyx/utils/list_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,21 +19,22 @@
 
 
 ########## BEGIN IMPORT ##########
 #### External modules
 import bisect
 import collections
 import itertools
+#### Import the logger
+import logging
+import re
+
 import natsort
 import numpy as np
-import re
-#### geodeZYX modules
 
-#### Import the logger
-import logging
+#### geodeZYX modules
 log = logging.getLogger(__name__)
 
 
 ##########  END IMPORT  ##########
 
 
 def is_listoflist(inp):
```

### Comparing `geodezyx-4.4.2/geodezyx/utils/plot_utils.py` & `geodezyx-4.4.3/geodezyx/utils/plot_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,26 +15,28 @@
 Copyright (C) 2019 Pierre Sakic et al. (IPGP, sakic@ipgp.fr)
 GitHub repository :
 https://github.com/GeodeZYX/geodezyx-toolbox
 """
 
 
 
+#### Import the logger
+import logging
+import os
+
 ########## BEGIN IMPORT ##########
 #### External modules
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
-import os
 import scipy
+
 #### geodeZYX modules
 from geodezyx import utils
 
-#### Import the logger
-import logging
 log = logging.getLogger(__name__)
 
 ##########  END IMPORT  ##########
 
 
 def color_list(L , colormap='jet'):
     cm     = plt.get_cmap(colormap)
```

### Comparing `geodezyx-4.4.2/geodezyx/utils/shell_like.py` & `geodezyx-4.4.3/geodezyx/utils/shell_like.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -20,24 +20,24 @@
 
 
 ########## BEGIN IMPORT ##########
 #### External modules
 import fnmatch
 import glob
 import gzip
+#### Import the logger
+import logging
 import os
 import re
 import shutil
 import subprocess
 
 #### geodeZYX modules
 from geodezyx import utils
 
-#### Import the logger
-import logging
 log = logging.getLogger(__name__)
 
 ##########  END IMPORT  ##########
 
 
 
 #################
```

### Comparing `geodezyx-4.4.2/geodezyx/utils/utils_core.py` & `geodezyx-4.4.3/geodezyx/utils/utils_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,31 +19,32 @@
 
 
 ########## BEGIN IMPORT ##########
 #### External modules
 import datetime as dt
 import gzip
 import inspect
-import numpy as np
+import io
+#### Import the logger
+import logging
 import os
-import pandas as pd
-import pickle
 import pathlib
+import pickle
 import re
-import scipy
 import sys
 import tempfile
 import time
 import uuid
-import io
+
+import numpy as np
+import pandas as pd
 import pathvalidate
-#### geodeZYX modules
+import scipy
 
-#### Import the logger
-import logging
+#### geodeZYX modules
 log = logging.getLogger(__name__)
 
 ##########  END IMPORT  ##########
 
 
 
 def clear_all():
```

### Comparing `geodezyx-4.4.2/geodezyx.egg-info/PKG-INFO` & `geodezyx-4.4.3/geodezyx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geodezyx
-Version: 4.4.2
+Version: 4.4.3
 Summary: geodezyx (a.k.a. The GeodeZYX toolbox) aims to provide simple but useful functions for Geodesy and Geophysics.
 Home-page: https://github.com/IPGP/geodezyx
 Author: Pierre Sakic & Gustavo Mansur
 Author-email: sakic@ipgp.fr
 Keywords: geodesy,geophysics,reference frames,gnss
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `geodezyx-4.4.2/geodezyx.egg-info/SOURCES.txt` & `geodezyx-4.4.3/geodezyx.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 geodezyx/operational/anubis_frontend.py
 geodezyx/operational/cluster_gfz.py
 geodezyx/operational/download_cddis.py
 geodezyx/operational/download_dropbox.py
 geodezyx/operational/download_find_files.py
 geodezyx/operational/download_prods.py
 geodezyx/operational/download_rinex.py
+geodezyx/operational/download_rinex_legacy.py
 geodezyx/operational/download_utils.py
 geodezyx/operational/gins_runner.py
 geodezyx/operational/groops_frontend.py
 geodezyx/operational/hector_frontend.py
 geodezyx/operational/midas_frontend.py
 geodezyx/operational/pride_pppar_frontend.py
 geodezyx/operational/rinex_lister_plotter.py
```

### Comparing `geodezyx-4.4.2/misc/refactoring.py` & `geodezyx-4.4.3/misc/refactoring.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 # -*- coding: utf-8 -*-
 """
 Created on Tue Aug  6 09:32:31 2019
 
 @author: psakicki
 """
 
-from geodezyx import *
-from geodezyx import utils
-import os,re
-
 #### Import the logger
 import logging
+import os
+import re
+
+from geodezyx import utils
+
 log = logging.getLogger(__name__)
 
 ################ GENERATION OF THE DICT
 p="/home/psakicki/CODES/GeodeZYX-Toolbox_v4/geodezyx"
 
 Lmodul = utils.find_recursive(p,"*py")
```

### Comparing `geodezyx-4.4.2/setup.py` & `geodezyx-4.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """A setuptools based setup module.
 
 See:
 https://packaging.python.org/guides/distributing-packages-using-setuptools/
 https://github.com/pypa/sampleproject
 """
 
+import pathlib
+
 # Always prefer setuptools over distutils
 from setuptools import setup, find_packages
-import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
@@ -33,15 +34,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='4.4.2',  # Required
+    version='4.4.3',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='geodezyx (a.k.a. The GeodeZYX toolbox) aims to provide simple but useful functions for Geodesy and Geophysics.',  # Optional
 
     # This is an optional longer description of your project that represents
```

