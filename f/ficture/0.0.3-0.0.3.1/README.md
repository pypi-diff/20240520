# Comparing `tmp/ficture-0.0.3.tar.gz` & `tmp/ficture-0.0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ficture-0.0.3.tar", last modified: Wed Apr 17 18:52:04 2024, max compression
+gzip compressed data, was "ficture-0.0.3.1.tar", last modified: Mon May 20 17:26:19 2024, max compression
```

## Comparing `ficture-0.0.3.tar` & `ficture-0.0.3.1.tar`

### file list

```diff
@@ -1,73 +1,74 @@
-drwxr-xr-x   0 bluebear   (501) staff       (20)        0 2024-04-17 18:52:04.236161 ficture-0.0.3/
--rw-r--r--   0 bluebear   (501) staff       (20)    19347 2024-04-04 10:02:06.000000 ficture-0.0.3/LICENSE
--rw-r--r--   0 bluebear   (501) staff       (20)       57 2024-04-04 13:57:26.000000 ficture-0.0.3/MANIFEST.in
--rw-r--r--   0 bluebear   (501) staff       (20)     1846 2024-04-17 18:52:04.236099 ficture-0.0.3/PKG-INFO
--rw-r--r--   0 bluebear   (501) staff       (20)     1058 2024-04-04 07:30:11.000000 ficture-0.0.3/README.md
-drwxr-xr-x   0 bluebear   (501) staff       (20)        0 2024-04-17 18:52:04.216858 ficture-0.0.3/ficture/
--rw-r--r--   0 bluebear   (501) staff       (20)      263 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/__init__.py
--rw-r--r--   0 bluebear   (501) staff       (20)     1604 2024-04-17 03:52:06.000000 ficture-0.0.3/ficture/cli.py
-drwxr-xr-x   0 bluebear   (501) staff       (20)        0 2024-04-17 18:52:04.219176 ficture-0.0.3/ficture/loaders/
--rw-r--r--   0 bluebear   (501) staff       (20)        0 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/loaders/__init__.py
--rw-r--r--   0 bluebear   (501) staff       (20)    10715 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/loaders/data_loader.py
--rw-r--r--   0 bluebear   (501) staff       (20)     4077 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/loaders/pixel_factor_loader.py
--rw-r--r--   0 bluebear   (501) staff       (20)    12685 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/loaders/pixel_loader.py
--rw-r--r--   0 bluebear   (501) staff       (20)    10013 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/loaders/pixel_to_unit_loader.py
--rw-r--r--   0 bluebear   (501) staff       (20)     7907 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/loaders/unit_loader.py
-drwxr-xr-x   0 bluebear   (501) staff       (20)        0 2024-04-17 18:52:04.220037 ficture-0.0.3/ficture/models/
--rw-r--r--   0 bluebear   (501) staff       (20)        0 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/models/__init__.py
--rw-r--r--   0 bluebear   (501) staff       (20)     2442 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/models/lda_minibatch.py
--rw-r--r--   0 bluebear   (501) staff       (20)    28506 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/models/online_lda.py
--rw-r--r--   0 bluebear   (501) staff       (20)    10460 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/models/online_slda.py
--rw-r--r--   0 bluebear   (501) staff       (20)     2350 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/models/slda_minibatch.py
-drwxr-xr-x   0 bluebear   (501) staff       (20)        0 2024-04-17 18:52:04.226083 ficture-0.0.3/ficture/scripts/
--rw-r--r--   0 bluebear   (501) staff       (20)      212 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/scripts/__init__.py
--rw-r--r--   0 bluebear   (501) staff       (20)     6411 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/scripts/choose_color.py
--rw-r--r--   0 bluebear   (501) staff       (20)     5394 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/scripts/de_bulk.py
--rw-r--r--   0 bluebear   (501) staff       (20)    10343 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/scripts/factor_report.py
--rw-r--r--   0 bluebear   (501) staff       (20)     2442 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/scripts/factor_report.template.html
--rw-r--r--   0 bluebear   (501) staff       (20)     4738 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/scripts/filter_boundary.py
--rw-r--r--   0 bluebear   (501) staff       (20)     7726 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/scripts/filter_density.py
--rw-r--r--   0 bluebear   (501) staff       (20)    10560 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/scripts/filter_poly.py
--rw-r--r--   0 bluebear   (501) staff       (20)    11914 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/scripts/init_model_selection.py
--rw-r--r--   0 bluebear   (501) staff       (20)    12193 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/scripts/lda_univ.py
--rw-r--r--   0 bluebear   (501) staff       (20)     9058 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/scripts/make_dge_univ.py
--rw-r--r--   0 bluebear   (501) staff       (20)     7444 2024-04-17 03:52:06.000000 ficture-0.0.3/ficture/scripts/make_spatial_minibatch.py
--rw-r--r--   0 bluebear   (501) staff       (20)    11623 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/scripts/plot_base.py
--rw-r--r--   0 bluebear   (501) staff       (20)    11866 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/scripts/plot_hexagon.py
--rw-r--r--   0 bluebear   (501) staff       (20)     7246 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/scripts/plot_pixel_full.py
--rw-r--r--   0 bluebear   (501) staff       (20)     6782 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/scripts/plot_pixel_multi.py
--rw-r--r--   0 bluebear   (501) staff       (20)     4698 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/scripts/plot_pixel_single.py
--rw-r--r--   0 bluebear   (501) staff       (20)    20563 2024-04-17 03:52:06.000000 ficture-0.0.3/ficture/scripts/run_together.py
--rw-r--r--   0 bluebear   (501) staff       (20)     9333 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/scripts/slda_decode.py
--rw-r--r--   0 bluebear   (501) staff       (20)     8932 2024-04-17 03:52:06.000000 ficture-0.0.3/ficture/scripts/transform_univ.py
-drwxr-xr-x   0 bluebear   (501) staff       (20)        0 2024-04-17 18:52:04.227310 ficture-0.0.3/ficture/utils/
--rw-r--r--   0 bluebear   (501) staff       (20)        0 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/utils/__init__.py
--rw-r--r--   0 bluebear   (501) staff       (20)     4501 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/utils/filter_fn.py
--rw-r--r--   0 bluebear   (501) staff       (20)     2123 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/utils/hexagon_fn.py
--rw-r--r--   0 bluebear   (501) staff       (20)    11956 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/utils/image_fn.py
--rw-r--r--   0 bluebear   (501) staff       (20)     1447 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/utils/layout_fn.py
--rw-r--r--   0 bluebear   (501) staff       (20)     3767 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/utils/mds_color_circle.py
--rw-r--r--   0 bluebear   (501) staff       (20)     2457 2024-04-17 03:52:06.000000 ficture-0.0.3/ficture/utils/minimake.py
--rw-r--r--   0 bluebear   (501) staff       (20)    14775 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/utils/utilt.py
--rw-r--r--   0 bluebear   (501) staff       (20)     5885 2024-04-04 13:57:26.000000 ficture-0.0.3/ficture/utils/visualize_factors.py
-drwxr-xr-x   0 bluebear   (501) staff       (20)        0 2024-04-17 18:52:04.235852 ficture-0.0.3/ficture.egg-info/
--rw-r--r--   0 bluebear   (501) staff       (20)     1846 2024-04-17 18:52:04.000000 ficture-0.0.3/ficture.egg-info/PKG-INFO
--rw-r--r--   0 bluebear   (501) staff       (20)     1981 2024-04-17 18:52:04.000000 ficture-0.0.3/ficture.egg-info/SOURCES.txt
--rw-r--r--   0 bluebear   (501) staff       (20)        1 2024-04-17 18:52:04.000000 ficture-0.0.3/ficture.egg-info/dependency_links.txt
--rw-r--r--   0 bluebear   (501) staff       (20)       45 2024-04-17 18:52:04.000000 ficture-0.0.3/ficture.egg-info/entry_points.txt
--rw-r--r--   0 bluebear   (501) staff       (20)      127 2024-04-17 18:52:04.000000 ficture-0.0.3/ficture.egg-info/requires.txt
--rw-r--r--   0 bluebear   (501) staff       (20)        8 2024-04-17 18:52:04.000000 ficture-0.0.3/ficture.egg-info/top_level.txt
-drwxr-xr-x   0 bluebear   (501) staff       (20)        0 2024-04-17 18:52:04.235632 ficture-0.0.3/info/
--rw-r--r--   0 bluebear   (501) staff       (20)   743896 2024-03-20 18:43:57.000000 ficture-0.0.3/info/Homo_sapiens.GRCh38.107.names.tsv.gz
--rw-r--r--   0 bluebear   (501) staff       (20)   953535 2024-03-20 18:43:57.000000 ficture-0.0.3/info/Mus_musculus.GRCm38.102.names.tsv.gz
--rw-r--r--   0 bluebear   (501) staff       (20)   957882 2024-03-20 18:43:57.000000 ficture-0.0.3/info/Mus_musculus.GRCm39.107.names.tsv.gz
--rw-r--r--   0 bluebear   (501) staff       (20)   323108 2024-03-20 18:43:57.000000 ficture-0.0.3/info/gencode.human.mouse.combined.gene.types.tsv.gz
--rw-r--r--   0 bluebear   (501) staff       (20)   356994 2024-03-20 18:43:57.000000 ficture-0.0.3/info/gencode.human.mouse.combined.gene_names.clean.tsv
--rw-r--r--   0 bluebear   (501) staff       (20)       40 2024-03-20 18:43:57.000000 ficture-0.0.3/info/hiseq.half_right.coordinate_minmax.tsv
--rw-r--r--   0 bluebear   (501) staff       (20)       43 2024-03-20 18:43:57.000000 ficture-0.0.3/info/hiseq.l1.half_right.coordinate_minmax.tsv
--rw-r--r--   0 bluebear   (501) staff       (20)       40 2024-03-20 18:43:57.000000 ficture-0.0.3/info/hiseq.l2.half_right.coordinate_minmax.tsv
--rw-r--r--   0 bluebear   (501) staff       (20)     1518 2024-03-20 18:43:57.000000 ficture-0.0.3/info/hiseq.layout.tsv
--rw-r--r--   0 bluebear   (501) staff       (20)      320 2024-03-20 18:43:57.000000 ficture-0.0.3/info/hiseq.tile_list.txt
--rw-r--r--   0 bluebear   (501) staff       (20)      840 2024-04-17 18:51:54.000000 ficture-0.0.3/pyproject.toml
--rw-r--r--   0 bluebear   (501) staff       (20)      268 2024-04-17 18:52:04.236400 ficture-0.0.3/setup.cfg
--rw-r--r--   0 bluebear   (501) staff       (20)       38 2024-04-04 13:57:26.000000 ficture-0.0.3/setup.py
+drwxrws---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)        0 2024-05-20 17:26:19.895878 ficture-0.0.3.1/
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)    19347 2023-09-11 21:49:40.000000 ficture-0.0.3.1/LICENSE
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)       57 2023-11-04 03:07:00.000000 ficture-0.0.3.1/MANIFEST.in
+-rwxrwxr--   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     1239 2024-05-20 17:26:19.892723 ficture-0.0.3.1/PKG-INFO
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)      491 2024-04-25 06:10:24.000000 ficture-0.0.3.1/README.md
+drwxrws---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)        0 2024-05-20 17:26:19.369020 ficture-0.0.3.1/ficture/
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)      263 2023-11-04 03:02:24.000000 ficture-0.0.3.1/ficture/__init__.py
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     1659 2024-05-16 13:43:04.000000 ficture-0.0.3.1/ficture/cli.py
+drwxrws---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)        0 2024-05-20 17:26:19.459779 ficture-0.0.3.1/ficture/loaders/
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)        0 2023-11-04 03:02:24.000000 ficture-0.0.3.1/ficture/loaders/__init__.py
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)    10715 2024-04-25 06:10:25.000000 ficture-0.0.3.1/ficture/loaders/data_loader.py
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     4103 2024-05-16 13:17:58.000000 ficture-0.0.3.1/ficture/loaders/pixel_factor_loader.py
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)    12796 2024-05-16 13:20:29.000000 ficture-0.0.3.1/ficture/loaders/pixel_loader.py
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)    10013 2024-04-25 06:10:25.000000 ficture-0.0.3.1/ficture/loaders/pixel_to_unit_loader.py
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     7915 2024-04-25 10:14:31.000000 ficture-0.0.3.1/ficture/loaders/unit_loader.py
+drwxrws---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)        0 2024-05-20 17:26:19.489809 ficture-0.0.3.1/ficture/models/
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)        0 2023-11-04 03:02:24.000000 ficture-0.0.3.1/ficture/models/__init__.py
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     2442 2023-11-04 03:02:24.000000 ficture-0.0.3.1/ficture/models/lda_minibatch.py
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)    28506 2024-04-25 06:10:25.000000 ficture-0.0.3.1/ficture/models/online_lda.py
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)    10460 2024-04-25 06:10:25.000000 ficture-0.0.3.1/ficture/models/online_slda.py
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     2350 2023-11-04 03:02:24.000000 ficture-0.0.3.1/ficture/models/slda_minibatch.py
+drwxrws---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)        0 2024-05-20 17:26:19.663885 ficture-0.0.3.1/ficture/scripts/
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)      212 2023-11-04 03:02:24.000000 ficture-0.0.3.1/ficture/scripts/__init__.py
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     8588 2024-05-20 16:07:09.000000 ficture-0.0.3.1/ficture/scripts/choose_color.py
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     5394 2024-04-25 06:10:25.000000 ficture-0.0.3.1/ficture/scripts/de_bulk.py
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)    10343 2024-04-25 06:10:25.000000 ficture-0.0.3.1/ficture/scripts/factor_report.py
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     2442 2023-11-04 03:02:24.000000 ficture-0.0.3.1/ficture/scripts/factor_report.template.html
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     4738 2024-04-25 06:10:25.000000 ficture-0.0.3.1/ficture/scripts/filter_boundary.py
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     7726 2024-04-25 06:10:25.000000 ficture-0.0.3.1/ficture/scripts/filter_density.py
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)    10560 2024-04-25 06:10:25.000000 ficture-0.0.3.1/ficture/scripts/filter_poly.py
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)    11961 2024-05-16 13:36:04.000000 ficture-0.0.3.1/ficture/scripts/init_model_selection.py
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)    12193 2024-04-25 06:10:25.000000 ficture-0.0.3.1/ficture/scripts/lda_univ.py
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     9033 2024-05-20 16:24:04.000000 ficture-0.0.3.1/ficture/scripts/make_dge_univ.py
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)    10502 2024-05-16 13:43:04.000000 ficture-0.0.3.1/ficture/scripts/make_sge_by_hexagon.py
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     7444 2024-04-25 06:10:25.000000 ficture-0.0.3.1/ficture/scripts/make_spatial_minibatch.py
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)    11623 2024-04-25 06:10:25.000000 ficture-0.0.3.1/ficture/scripts/plot_base.py
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)    11866 2024-04-25 06:10:25.000000 ficture-0.0.3.1/ficture/scripts/plot_hexagon.py
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     7245 2024-05-16 13:26:40.000000 ficture-0.0.3.1/ficture/scripts/plot_pixel_full.py
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     6782 2024-04-25 06:10:25.000000 ficture-0.0.3.1/ficture/scripts/plot_pixel_multi.py
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     4698 2024-04-25 06:10:25.000000 ficture-0.0.3.1/ficture/scripts/plot_pixel_single.py
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)    21645 2024-05-20 16:55:37.000000 ficture-0.0.3.1/ficture/scripts/run_together.py
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     9332 2024-04-25 07:04:33.000000 ficture-0.0.3.1/ficture/scripts/slda_decode.py
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     8931 2024-05-16 13:43:04.000000 ficture-0.0.3.1/ficture/scripts/transform_univ.py
+drwxrws---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)        0 2024-05-20 17:26:19.756477 ficture-0.0.3.1/ficture/utils/
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)        0 2023-11-04 03:02:24.000000 ficture-0.0.3.1/ficture/utils/__init__.py
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     4501 2024-04-25 06:10:25.000000 ficture-0.0.3.1/ficture/utils/filter_fn.py
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     2123 2024-04-25 06:10:25.000000 ficture-0.0.3.1/ficture/utils/hexagon_fn.py
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)    11956 2023-11-04 03:02:24.000000 ficture-0.0.3.1/ficture/utils/image_fn.py
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     1447 2023-11-04 03:02:24.000000 ficture-0.0.3.1/ficture/utils/layout_fn.py
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     3767 2024-04-25 06:10:25.000000 ficture-0.0.3.1/ficture/utils/mds_color_circle.py
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     2457 2024-04-25 06:10:25.000000 ficture-0.0.3.1/ficture/utils/minimake.py
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)    14775 2024-04-25 06:10:25.000000 ficture-0.0.3.1/ficture/utils/utilt.py
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     5885 2024-04-25 06:10:25.000000 ficture-0.0.3.1/ficture/utils/visualize_factors.py
+drwxrws---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)        0 2024-05-20 17:26:19.883842 ficture-0.0.3.1/ficture.egg-info/
+-rwxrwxr--   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     1239 2024-05-20 17:26:19.000000 ficture-0.0.3.1/ficture.egg-info/PKG-INFO
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     2020 2024-05-20 17:26:19.000000 ficture-0.0.3.1/ficture.egg-info/SOURCES.txt
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)        1 2024-05-20 17:26:19.000000 ficture-0.0.3.1/ficture.egg-info/dependency_links.txt
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)       45 2024-05-20 17:26:19.000000 ficture-0.0.3.1/ficture.egg-info/entry_points.txt
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)      115 2024-05-20 17:26:19.000000 ficture-0.0.3.1/ficture.egg-info/requires.txt
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)        8 2024-05-20 17:26:19.000000 ficture-0.0.3.1/ficture.egg-info/top_level.txt
+drwxrws---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)        0 2024-05-20 17:26:19.875161 ficture-0.0.3.1/info/
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)   743896 2024-04-25 06:10:25.000000 ficture-0.0.3.1/info/Homo_sapiens.GRCh38.107.names.tsv.gz
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)   953535 2024-04-25 06:10:25.000000 ficture-0.0.3.1/info/Mus_musculus.GRCm38.102.names.tsv.gz
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)   957882 2024-04-25 06:10:25.000000 ficture-0.0.3.1/info/Mus_musculus.GRCm39.107.names.tsv.gz
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)   323108 2024-04-25 06:10:25.000000 ficture-0.0.3.1/info/gencode.human.mouse.combined.gene.types.tsv.gz
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)   356994 2024-04-25 06:10:25.000000 ficture-0.0.3.1/info/gencode.human.mouse.combined.gene_names.clean.tsv
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)       40 2024-04-25 06:10:25.000000 ficture-0.0.3.1/info/hiseq.half_right.coordinate_minmax.tsv
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)       43 2024-04-25 06:10:25.000000 ficture-0.0.3.1/info/hiseq.l1.half_right.coordinate_minmax.tsv
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)       40 2024-04-25 06:10:25.000000 ficture-0.0.3.1/info/hiseq.l2.half_right.coordinate_minmax.tsv
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     1518 2024-04-25 06:10:25.000000 ficture-0.0.3.1/info/hiseq.layout.tsv
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)      320 2024-04-25 06:10:25.000000 ficture-0.0.3.1/info/hiseq.tile_list.txt
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)      824 2024-05-20 17:26:02.000000 ficture-0.0.3.1/pyproject.toml
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)      268 2024-05-20 17:26:19.900434 ficture-0.0.3.1/setup.cfg
+-rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)       38 2023-11-04 04:37:40.000000 ficture-0.0.3.1/setup.py
```

### Comparing `ficture-0.0.3/LICENSE` & `ficture-0.0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ficture-0.0.3/ficture/cli.py` & `ficture-0.0.3.1/ficture/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,23 +5,23 @@
     # MAYBE.. should change legacy file names to match callable module names
     module_map = {\
         "filter_by_density": "filter_poly", \
         # "filter_by_density_v1": "filter_density", \
         "filter_by_boundary": "filter_boundary", \
         "make_spatial_minibatch": "make_spatial_minibatch",\
         "make_dge": "make_dge_univ", \
+        "make_sge_by_hexagon": "make_sge_by_hexagon", \
         "fit_model": "init_model_selection", \
         # "lda": "lda_univ", \
         "transform": "transform_univ", \
         "choose_color": "choose_color", \
         "plot_base": "plot_base", \
         "de_bulk": "de_bulk", \
         "factor_report": "factor_report", \
         "slda_decode": "slda_decode", \
-
         "plot_base": "plot_base", \
         "plot_hexagon": "plot_hexagon", \
         "plot_pixel_multi": "plot_pixel_multi", \
         "plot_pixel_full": "plot_pixel_full", \
         "plot_pixel_single": "plot_pixel_single", \
         "run_together": "run_together", \
     }
```

### Comparing `ficture-0.0.3/ficture/loaders/data_loader.py` & `ficture-0.0.3.1/ficture/loaders/data_loader.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.3/ficture/loaders/pixel_factor_loader.py` & `ficture-0.0.3.1/ficture/loaders/pixel_factor_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,19 +47,20 @@
         self.xmax = min(xmax, self.meta["SIZE_X"])
         self.ymin = max(ymin, 0)
         self.ymax = min(ymax, self.meta["SIZE_Y"])
         if full:
             self.reader = pd.read_csv(input,sep='\t',skiprows=nheader,chunksize=chunksize,names=self.header, dtype=dty)
         else:
             # Translate target region to index
-            block = [int(x / self.meta['BLOCK_SIZE']) for x in [self.xmin, self.xmax - 1] ]
-            pos_range = [int(x*self.meta['SCALE']) for x in [self.ymin, self.ymax]]
             if self.meta['BLOCK_AXIS'] == "Y":
                 block = [int(x / self.meta['BLOCK_SIZE']) for x in [self.ymin, self.ymax - 1] ]
                 pos_range = [int(x*self.meta['SCALE']) for x in [self.xmin, self.xmax]]
+            else:
+                block = [int(x / self.meta['BLOCK_SIZE']) for x in [self.xmin, self.xmax - 1] ]
+                pos_range = [int(x*self.meta['SCALE']) for x in [self.ymin, self.ymax]]
             block = np.arange(block[0], block[1]+1) * self.meta['BLOCK_SIZE']
             query = []
             pos_range = '-'.join([str(x) for x in pos_range])
             for i,b in enumerate(block):
                 query.append( str(b)+':'+pos_range )
 
             cmd = " ".join( ["tabix", input] + query )
```

### Comparing `ficture-0.0.3/ficture/loaders/pixel_loader.py` & `ficture-0.0.3.1/ficture/loaders/pixel_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         self.pixel_reader = reader
         self.batch_id = batch_id
         self.mu_scale = mu_scale
         self.file_is_open = True
         self.ft_dict = ft_dict
         self.M = len(self.ft_dict)
         self.key = key
-        self.precision = np.clip(precision, 0.1, np.inf)
+        self.precision = precision
         self.radius = radius
         self.adj_penal = adj_penal
         self.nu = np.log(.5) / np.log(halflife)
         self.out_buff = self.radius * halflife
         self.thread = thread
         self.verbose = verbose
 
@@ -64,21 +64,24 @@
             try:
                 chunk = next(self.pixel_reader)
             except StopIteration:
                 self.file_is_open = False
                 break
             chunk = chunk.loc[chunk.gene.isin(self.ft_dict) & \
                               (chunk[self.key] > 0), :]
-            chunk.X = (chunk.X * self.mu_scale / self.precision).astype(int)
-            chunk.Y = (chunk.Y * self.mu_scale / self.precision).astype(int)
-            chunk = chunk.groupby(by=[self.batch_id,"gene","X","Y"]).agg({self.key: "sum"}).reset_index()
+            chunk.X *= self.mu_scale
+            chunk.Y *= self.mu_scale
+            if self.precision > 0:
+                chunk.X = (chunk.X / self.precision).astype(int)
+                chunk.Y = (chunk.Y / self.precision).astype(int)
+                chunk = chunk.groupby(by=[self.batch_id,"gene","X","Y"]).agg({self.key: "sum"}).reset_index()
+                chunk.X *= self.precision
+                chunk.Y *= self.precision
             random_pref = chunk[self.batch_id].map(lambda x : x[-5:]).values
-            chunk['j'] = random_pref + '_' + chunk.X.astype(str) + '_' + chunk.Y.astype(str)
-            chunk.X *= self.precision
-            chunk.Y *= self.precision
+            chunk['j'] = random_pref + '_' + (chunk.X*100).astype(int).astype(str) + '_' + (chunk.Y*100).astype(int).astype(str)
             # Keep pixels close enough to at least one anchor
             pts = chunk[["j", "X", "Y"]].drop_duplicates(subset="j")
             dist, indx = self.ref.query(X = np.array(pts[['X','Y']]), k = 1, return_distance = True)
             dist = dist.squeeze()
 
             kept_pixel = dist < self.radius
             if np.sum(kept_pixel) == 0:
```

### Comparing `ficture-0.0.3/ficture/loaders/pixel_to_unit_loader.py` & `ficture-0.0.3.1/ficture/loaders/pixel_to_unit_loader.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.3/ficture/loaders/unit_loader.py` & `ficture-0.0.3.1/ficture/loaders/unit_loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             n_unit = len(self.df.unit.unique())
         left = pd.DataFrame()
         if self.file_is_open:
             last_indx = self.df.unit.iloc[-1]
             left = self.df[self.df.unit == last_indx]
             self.df = self.df[self.df.unit != last_indx]
         self.brc = self.df[['unit']+self.unit_attr].drop_duplicates(subset=['unit'])
-        self.brc = self.brc.merge(right = self.df.groupby(by='unit').agg({self.key:sum, self.bkey:sum}).reset_index(), on = 'unit', how = 'inner' )
+        self.brc = self.brc.merge(right = self.df.groupby(by='unit').agg({self.key:"sum", self.bkey:"sum"}).reset_index(), on = 'unit', how = 'inner' )
         self.brc = self.brc[self.brc[self.key] >= self.min_ct_per_unit]
         buffer_weight = self.brc[self.bkey].values / (self.brc[self.bkey].values + self.brc[self.key].values)
         barcode_kept=list(self.brc.unit)
         bt_dict={x:i for i,x in enumerate(barcode_kept)}
         N = len(bt_dict)
         self.df = self.df[self.df.unit.isin(bt_dict) & self.df.gene.isin(self.ft_dict)]
         if self.prefix > 0:
@@ -90,17 +90,17 @@
         self.test_mtx = None
 
     def _make_matrix(self):
         self.brc = self.df[['unit']+self.unit_attr].drop_duplicates(subset=['unit'])
         if self.prefix > 0:
             lab = self.brc.unit.str[:self.prefix].unique()
             self.batch_id_list += [x for x in lab if x not in self.batch_id_list]
-        self.brc = self.brc.merge(right = self.df.groupby(by='unit').agg({self.train_key:sum}).reset_index(), on = 'unit', how = 'inner' )
+        self.brc = self.brc.merge(right = self.df.groupby(by='unit').agg({self.train_key:"sum"}).reset_index(), on = 'unit', how = 'inner' )
         if self.key != self.train_key:
-            self.brc = self.brc.merge(right = self.df.groupby(by='unit').agg({self.key:sum}).reset_index(), on = 'unit', how = 'inner' )
+            self.brc = self.brc.merge(right = self.df.groupby(by='unit').agg({self.key:"sum"}).reset_index(), on = 'unit', how = 'inner' )
         self.brc = self.brc[self.brc[self.key] >= self.min_ct_per_unit]
         barcode_kept=list(self.brc.unit)
         bt_dict={x:i for i,x in enumerate(barcode_kept)}
         N = len(bt_dict)
         self.df = self.df[self.df.unit.isin(bt_dict)]
         self.mtx = coo_array((self.df[self.train_key].values, \
                             (self.df.unit.map(bt_dict).values, \
```

### Comparing `ficture-0.0.3/ficture/models/lda_minibatch.py` & `ficture-0.0.3.1/ficture/models/lda_minibatch.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.3/ficture/models/online_lda.py` & `ficture-0.0.3.1/ficture/models/online_lda.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.3/ficture/models/online_slda.py` & `ficture-0.0.3.1/ficture/models/online_slda.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.3/ficture/models/slda_minibatch.py` & `ficture-0.0.3.1/ficture/models/slda_minibatch.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.3/ficture/scripts/choose_color.py` & `ficture-0.0.3.1/ficture/scripts/choose_color.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,27 +2,69 @@
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 
 import sklearn.neighbors
 from scipy.sparse import coo_array
 from datetime import datetime
+from sklearn.manifold import MDS
 
 from ficture.utils.utilt import plot_colortable
-from ficture.utils.mds_color_circle import assign_color_mds_circle
+# from ficture.utils.mds_color_circle import assign_color_mds_circle
+
+def assign_color_mds_line(mtx, cmap_name, weight=None, top_color=None, seed=None):
+    # mtx is a K by K similarity/proximity matrix
+    assert mtx.shape[0] == mtx.shape[1], "mtx must be square"
+    K = mtx.shape[0]
+    # weight is a K vector of factor abundance
+    if weight is None:
+        weight = np.ones(K)
+    weight /= weight.sum()
+    # The color of the top factor (the one with the largest weight)
+    if top_color is None:
+        top_color = "#fcd217"
+    else:
+        match = re.search(r'^#(?:[0-9a-fA-F]{3}){1,2}$', top_color)
+        if match is None:
+            top_color = "#fcd217"
+    # Find the offset to map the top factor to the desired color
+    cgrid = 200
+    cmtx=plt.get_cmap(cmap_name)(np.arange(cgrid)/cgrid)
+    h = top_color.lstrip('#')
+    top_color_rgb = [int(h[i:i+2], 16)/255 for i in (0, 2, 4)]
+    d = np.abs(cmtx[:, :3] - np.array(top_color_rgb).reshape((1, -1)) ).sum(axis = 1)
+    anchor_pos = d.argmin() / cgrid
+    anchor_angle = anchor_pos * 2 * np.pi
+
+    mds = MDS(n_components=1, dissimilarity="precomputed", random_state=seed)
+    mds_coordinates = mds.fit_transform(mtx).flatten()
+    c_order = np.argsort(np.argsort(mds_coordinates))
+    w_vec = weight[np.argsort(mds_coordinates)]
+    w_vec = np.cumsum(w_vec) - w_vec/2
+    normalized_coordinates = np.zeros(K)
+    normalized_coordinates[c_order] = w_vec
+    angle = normalized_coordinates * 2 * np.pi
+    anchor_k = np.argmax(weight)
+    angle_shift = angle + (anchor_angle - angle[anchor_k])
+    if angle_shift.max() > 2*np.pi:
+        angle_shift -= np.pi * 2
+    angle_shift[angle_shift < 0] = 2 * np.pi + angle_shift[angle_shift < 0]
+    c_pos = angle_shift / np.pi / 2
+    return c_pos
 
 def choose_color(_args):
 
     parser = argparse.ArgumentParser()
     parser.add_argument('--input', type=str, help='')
     parser.add_argument('--output', type=str, help='')
     parser.add_argument('--cmap_name', type=str, default="turbo", help="Name of Matplotlib colormap to use (better close to a circular colormap)")
     parser.add_argument('--top_color', type=str, default="#fcd217", help="HEX color code for the top factor")
     parser.add_argument('--even_space', action='store_true', help="Evenly space the factors on the circle")
     parser.add_argument('--annotation', type=str, default = '', help='')
+    parser.add_argument('--circle', action='store_true', help="")
     parser.add_argument('--seed', type=int, default=-1, help='')
     args = parser.parse_args(_args)
 
     if len(_args) == 0:
         parser.print_help()
         return
 
@@ -74,22 +116,30 @@
     mask = (dist < nn + .5) & (dist > 0)
     r_indx = r_indx[mask]
     c_indx = c_indx[mask]
     # Compute spatial similarity
     Sig = coo_array((np.ones(len(r_indx)), (r_indx, c_indx)), shape=(N, N)).tocsr()
     W = np.array(df.loc[:, factor_header])
     mtx = W.T @ Sig @ W
-    # Translate into a symmetric dissimilarity measure
+    # Translate into a symmetric similarity measure
     # Large values in mtx indicate close proximity, to be mapped to distinct colors
     np.fill_diagonal(mtx, 0)
     mtx /= mtx.sum(axis = 1)
     mtx = mtx + mtx.T
 
-    # Assign color using MDS with circular constraint
-    c_pos = assign_color_mds_circle(mtx, cmap_name, weight=weight, top_color=args.top_color, seed=seed)
+    if args.circle:
+        # Assign color using MDS with circular constraint
+        from ficture.utils.mds_color_circle import assign_color_mds_circle
+        c_pos = assign_color_mds_circle(mtx, cmap_name, weight=weight, top_color=args.top_color, seed=seed)
+    else:
+        c_pos = assign_color_mds_line(mtx, cmap_name, weight=weight, top_color=args.top_color, seed=seed)
+
+    # # Assign color using MDS with circular constraint
+    # c_pos = assign_color_mds_circle(mtx, cmap_name, weight=weight, top_color=args.top_color, seed=seed)
+
     spectral_offset = .05 # avoid extremely dark colors
     c_pos = (c_pos - c_pos.min()) / (c_pos.max() - c_pos.min()) * (1 - spectral_offset) + spectral_offset
 
     c_rank = np.argsort(np.argsort(c_pos))
     cmtx = plt.get_cmap(cmap_name)(c_pos) # K x 4
     df = pd.DataFrame({"Name":np.arange(K).astype(str), "Color_index":c_rank})
     df = pd.concat([df, pd.DataFrame(cmtx[:, :3], columns=["R", "G", "B"])], axis=1)
```

### Comparing `ficture-0.0.3/ficture/scripts/de_bulk.py` & `ficture-0.0.3.1/ficture/scripts/de_bulk.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.3/ficture/scripts/factor_report.py` & `ficture-0.0.3.1/ficture/scripts/factor_report.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.3/ficture/scripts/factor_report.template.html` & `ficture-0.0.3.1/ficture/scripts/factor_report.template.html`

 * *Files identical despite different names*

### Comparing `ficture-0.0.3/ficture/scripts/filter_boundary.py` & `ficture-0.0.3.1/ficture/scripts/filter_boundary.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.3/ficture/scripts/filter_density.py` & `ficture-0.0.3.1/ficture/scripts/filter_density.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.3/ficture/scripts/filter_poly.py` & `ficture-0.0.3.1/ficture/scripts/filter_poly.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.3/ficture/scripts/init_model_selection.py` & `ficture-0.0.3.1/ficture/scripts/init_model_selection.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,15 @@
     unit_attr = [x.lower() for x in args.unit_attr]
     gene_key = args.feature_label.lower()
     logging.basicConfig(level= getattr(logging, "INFO", None))
 
     feature_list = None
     if os.path.isfile(args.feature):
         feature_list = pd.read_csv(args.feature, sep='\t', dtype={gene_key:str})[gene_key].tolist()
+        feature_list = list(set(feature_list))
 
     feature, brc, mtx_org, ft_dict, bc_dict = make_mtx_from_dge(args.input,\
         min_ct_per_unit = args.min_ct_per_unit, \
         min_ct_per_feature = args.min_ct_per_feature, \
         feature_list = feature_list, \
         unit = args.unit_label, key = key)
     unit_sum = mtx_org.sum(axis = 1)
```

### Comparing `ficture-0.0.3/ficture/scripts/lda_univ.py` & `ficture-0.0.3.1/ficture/scripts/lda_univ.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.3/ficture/scripts/make_dge_univ.py` & `ficture-0.0.3.1/ficture/scripts/make_dge_univ.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,16 +46,16 @@
     logging.info(f"Random seed {r_seed}")
     mj = args.major_axis
 
     # Input file and numerical columns to use as counts
     ct_header = args.count_header
     key = args.key
     if key not in ct_header:
-        key = ct_header[0]
-        logging.warning(f"The designated major key is not one of the specified count columns, --key is ignored the first existing key is chosen")
+        ct_header = [key]
+        logging.warning(f"The designated major key is not one of the specified count columns, --count_header is ignored")
     if not os.path.isfile(args.input):
         sys.exit(f"ERROR: cannot find input file \n {args.input}")
     with gzip.open(args.input, 'rt') as rf:
         input_header=rf.readline().strip().split('\t')
         ct_header = [v for v in input_header if v in ct_header]
         if len(ct_header) == 0:
             sys.exit("Input header does not contain the specified --count_header")
```

### Comparing `ficture-0.0.3/ficture/scripts/make_spatial_minibatch.py` & `ficture-0.0.3.1/ficture/scripts/make_spatial_minibatch.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.3/ficture/scripts/plot_base.py` & `ficture-0.0.3.1/ficture/scripts/plot_base.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.3/ficture/scripts/plot_hexagon.py` & `ficture-0.0.3.1/ficture/scripts/plot_hexagon.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.3/ficture/scripts/plot_pixel_full.py` & `ficture-0.0.3.1/ficture/scripts/plot_pixel_full.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
                 for c in rgb:
                     df[c] = color_info.loc[df['K1'].values, c].values
             else:
                 for c in rgb:
                     df[c] = 0
                     for k in range(1,loader.meta['TOPK']+1):
                         df[c] += color_info.loc[df['K'+str(k)].values, c].values * df['P'+str(k)].values
-        df = df.groupby(by=['X','Y']).agg({c:np.mean for c in rgb}).reset_index()
+        df = df.groupby(by=['X','Y']).agg({c:"mean" for c in rgb}).reset_index()
         logging.info(f"Reading pixels... {df.X.iloc[-1]}, {df.Y.iloc[-1]}, {df.shape[0]}")
         for i,c in enumerate(rgb):
             df[c] = np.clip(np.around(df[c] * 255),0,255).astype(np.uint8)
             img[df.Y.values, df.X.values, [i]*df.shape[0]] = df[c].values
         if args.debug:
             break
```

### Comparing `ficture-0.0.3/ficture/scripts/plot_pixel_multi.py` & `ficture-0.0.3.1/ficture/scripts/plot_pixel_multi.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.3/ficture/scripts/plot_pixel_single.py` & `ficture-0.0.3.1/ficture/scripts/plot_pixel_single.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.3/ficture/scripts/run_together.py` & `ficture-0.0.3.1/ficture/scripts/run_together.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
     parser = argparse.ArgumentParser()
 
     cmd_params = parser.add_argument_group("Commands", "FICTURE commands to run together")
     cmd_params.add_argument('--all', action='store_true', default=False, help='Run all FICTURE commands (preprocess, segment, lda, decode)')
     cmd_params.add_argument('--preprocess', action='store_true', default=False, help='Perform preprocess step')
     cmd_params.add_argument('--segment', action='store_true', default=False, help='Perform hexagonal segmentation')
+    cmd_params.add_argument('--sge', action='store_true', default=False, help='Create hexagonal SGEs')
     cmd_params.add_argument('--lda', action='store_true', default=False, help='Perform LDA model training')
     cmd_params.add_argument('--decode', action='store_true', default=False, help='Perform pixel-level decoding')
 
     run_params = parser.add_argument_group("Run Options", "Run options for FICTURE commands")
     run_params.add_argument('--dry-run', action='store_true', default=False, help='Dry run. Generate only the Makefile without running it')
     run_params.add_argument('--restart', action='store_true', default=False, help='Restart the run. Ignore all intermediate files and start from the beginning')
     run_params.add_argument('--threads', type=int, default=1, help='Maximum number of threads to use in each process')
@@ -30,29 +31,30 @@
     key_params = parser.add_argument_group("Key Parameters", "Key parameters that requires user's attention")
     key_params.add_argument('--in-tsv', required=True, type=str, help='Input TSV file (e.g. transcript.tsv.gz)')
     key_params.add_argument('--out-dir', required= True, type=str, help='Output directory')
     key_params.add_argument('--in-minmax', type=str, help='Input coordinate minmax TSV file (e.g. coordinate_minmax.tsv). If absent, it will be generated')
     key_params.add_argument('--in-feature', type=str, help='Input TSV file (e.g. feature.clean.tsv.gz) that specify which genes to use as input. If absent, it will be use all genes')
     key_params.add_argument('--major-axis', type=str, default='Y', help='Axis where transcripts.tsv.gz are sorted')
     key_params.add_argument('--mu-scale', type=float, default=1.0, help='Scale factor for mu (pixels per um)')
-    key_params.add_argument('--train-width', type=str, default="18", help='Hexagon flat-to-flat width (in um) during training. Use comma to specify multiple values')
+    key_params.add_argument('--train-width', type=str, default="12", help='Hexagon flat-to-flat width (in um) during training. Use comma to specify multiple values')
     key_params.add_argument('--n-factor', type=str, default="12", help='Number of factors to train. Use comma to specify multiple values')
     key_params.add_argument('--anchor-res', type=float, default=4, help='Anchor resolution for decoding')
     key_params.add_argument('--plot-each-factor', action='store_true', default=False, help='Plot individual factors in pixel-level decoding')
 
-
     aux_params = parser.add_argument_group("Auxiliary Parameters", "Auxiliary parameters (using default is recommended)")
     aux_params.add_argument('--train-epoch', type=int, default=3, help='Training epoch for LDA model')
     aux_params.add_argument('--train-epoch-id-len', type=int, default=2, help='Training epoch ID length')
     aux_params.add_argument('--train-n-move', type=int, default=2, help='Level of hexagonal sliding during training')
+    aux_params.add_argument('--sge-n-move', type=int, default=1, help='Level of hexagonal sliding during SGE generation')
     aux_params.add_argument('--fit-width', type=float, help='Hexagon flat-to-flat width (in um) during model fitting (default: same to train-width)')
     aux_params.add_argument('--key-col', type=str, default="Count", help='Columns from the input file to be used as key')
     aux_params.add_argument('--minibatch-size', type=int, default=500, help='Batch size used in minibatch processing')
     aux_params.add_argument('--minibatch-buffer', type=int, default=30, help='Batch buffer used in minibatch processing')
     aux_params.add_argument('--min-ct-unit-dge', type=int, default=50, help='Minimum count per hexagon in DGE generation')
+    aux_params.add_argument('--min-ct-unit-sge', type=int, default=1, help='Minimum count per hexagon in SGE generation')
     aux_params.add_argument('--min-ct-feature', type=int, default=20, help='Minimum count per feature during LDA training')
     aux_params.add_argument('--min-ct-unit-fit', type=int, default=20, help='Minimum count per hexagon unit during model fitting')
     aux_params.add_argument('--lda-rand-init', type=int, default=10, help='Number of random initialization during model training')
     aux_params.add_argument('--decode-top-k', type=int, default=3, help='Top K columns to output in pixel-level decoding results')
     aux_params.add_argument('--de-max-pval', type=float, default=1e-3, help='p-value cutoff for differential expression')
     aux_params.add_argument('--de-min-fold', type=float, default=1.5, help='Fold-change cutoff for differential expression')
     aux_params.add_argument('--decode-block-size', type=int, default=100, help='Block size for pixel decoding output')
@@ -70,18 +72,19 @@
     aux_params.add_argument('--sort', type=str, default="sort", help='Path to sort binary. For faster processing, you may add arguments like "sort -T /path/to/new/tmpdir --parallel=20 -S 10G"')
 
     args = parser.parse_args(_args)
 
     if len(_args) == 0:
         parser.print_help()
         return
-    
+
     if args.all:
         args.preprocess = True
         args.segment = True
+        args.sge = False
         args.lda = True
         args.decode = True
 
     ## parse input parameters
     train_widths = [int(x) for x in args.train_width.split(",")]
     n_factors = [int(x) for x in args.n_factor.split(",")]
 
@@ -102,85 +105,95 @@
     if not shutil.which(args.sort.split(" ")[0]):
         logging.error(f"Cannot find {args.sort}. Please make sure that the path to --sort is correct")
         sys.exit(1)
 
     if args.preprocess:
         ## create output directory if needed
         cmds = []
-        cmds.append(rf"$(info --------------------------------------------------------------)") 
-        cmds.append(rf"$(info Creating minibatch from {args.in_tsv}...)") 
-        cmds.append(rf"$(info --------------------------------------------------------------)") 
+        cmds.append(rf"$(info --------------------------------------------------------------)")
+        cmds.append(rf"$(info Creating minibatch from {args.in_tsv}...)")
+        cmds.append(rf"$(info --------------------------------------------------------------)")
         ## create minibatch
         cmds.append(f"ficture make_spatial_minibatch --input {args.in_tsv} --output {batch_tsv} --mu_scale {args.mu_scale} --batch_size {args.minibatch_size} --batch_buff {args.minibatch_buffer} --major_axis {args.major_axis}")
         cmds.append(f"{args.sort} -k 2,2n -k 1,1g {batch_tsv} | {args.gzip} -c > {batch_out}")
-        cmds.append(f"rm {batch_tsv}") 
+        cmds.append(f"rm {batch_tsv}")
         mm.add_target(batch_out, [args.in_tsv], cmds)
 
         if args.in_minmax is None:
             script_path = f"{args.out_dir}/write_minmax.sh"
             with open(script_path, "w") as f:
                 f.write(r"""#!/bin/bash
 input=$1
 output=$2
-mu_scale=$3                        
+mu_scale=$3
 gzip -cd ${input} | awk 'BEGIN{FS=OFS="\t"} NR==1{for(i=1;i<=NF;i++){if($i=="X")x=i;if($i=="Y")y=i}print $x,$y;next}{print $x,$y}' | perl -slane 'print join("\t",$F[0]/${mu_scale},$F[1]/${mu_scale})' -- -mu_scale="${mu_scale}" | awk -F'\t' ' BEGIN { min1 = "undef"; max1 = "undef"; min2 = "undef"; max2 = "undef"; } { if (NR == 2 || $1 < min1) min1 = $1; if (NR == 2 || $1 > max1) max1 = $1; if (NR == 2 || $2 < min2) min2 = $2; if (NR == 2 || $2 > max2) max2 = $2; } END { print "xmin\t", min1; print "xmax\t", max1; print "ymin\t", min2; print "ymax\t", max2; }' > ${output}
 """)
             cmds = []
-            cmds.append(rf"$(info --------------------------------------------------------------)") 
-            cmds.append(rf"$(info Obtaining boundary coordinates to {minmax_out}...)") 
-            cmds.append(rf"$(info --------------------------------------------------------------)") 
+            cmds.append(rf"$(info --------------------------------------------------------------)")
+            cmds.append(rf"$(info Obtaining boundary coordinates to {minmax_out}...)")
+            cmds.append(rf"$(info --------------------------------------------------------------)")
             cmds.append(f"bash {script_path} {args.in_tsv} {minmax_out} {args.mu_scale}")
             mm.add_target(minmax_out, [args.in_tsv], cmds)
 
     if args.segment:
         for train_width in train_widths:
             dge_out = f"{args.out_dir}/hexagon.d_{train_width}.tsv"
             cmds = []
-            cmds.append(rf"$(info --------------------------------------------------------------)") 
-            cmds.append(rf"$(info Creating DGE for {train_width}um...)") 
-            cmds.append(rf"$(info --------------------------------------------------------------)") 
-            cmds.append(f"ficture make_dge --key {args.key_col} --count_header {args.key_col} --input {args.in_tsv} --output {dge_out} --hex_width {train_width} --n_move {args.train_n_move} --min_ct_per_unit {args.min_ct_unit_dge} --mu_scale {args.mu_scale} --precision {args.dge_precision} --major_axis {args.major_axis}")
+            cmds.append(rf"$(info --------------------------------------------------------------)")
+            cmds.append(rf"$(info Creating DGE for {train_width}um...)")
+            cmds.append(rf"$(info --------------------------------------------------------------)")
+            cmds.append(f"ficture make_dge --key {args.key_col} --input {args.in_tsv} --output {dge_out} --hex_width {train_width} --n_move {args.train_n_move} --min_ct_per_unit {args.min_ct_unit_dge} --mu_scale {args.mu_scale} --precision {args.dge_precision} --major_axis {args.major_axis}")
             cmds.append(f"{args.sort} -k 1,1n {dge_out} | {args.gzip} -c > {dge_out}.gz")
             cmds.append(f"rm {dge_out}")
             mm.add_target(f"{dge_out}.gz", [args.in_tsv], cmds)
-    
+
+    if args.sge:
+        for train_width in train_widths:
+            sge_out_dir = f"{args.out_dir}/segment/sge.d_{train_width}"
+            cmds = []
+            cmds.append(rf"$(info --------------------------------------------------------------)")
+            cmds.append(rf"$(info Creating SGE for {train_width}um...)")
+            cmds.append(rf"$(info --------------------------------------------------------------)")
+            cmds.append(f"ficture make_sge_by_hexagon --key {args.key_col} --input {args.in_tsv} --feature {args.in_feature} --output_path {sge_out_dir} --hex_width {train_width} --n_move {args.sge_n_move} --min_ct_per_unit {args.min_ct_unit_sge} --mu_scale {args.mu_scale} --precision {args.dge_precision} --major_axis {args.major_axis} --transfer_gene_prefix")
+            mm.add_target(f"{sge_out_dir}/barcodes.tsv.gz", [args.in_tsv], cmds)
+
     if args.lda:
         for train_width in train_widths:
             for n_factor in n_factors:
                 model_id=f"nF{n_factor}.d_{train_width}"
                 model_path=f"{args.out_dir}/analysis/{model_id}"
                 figure_path=f"{model_path}/figure"
                 hexagon = f"{args.out_dir}/hexagon.d_{train_width}.tsv.gz"
                 model_prefix=f"{model_path}/{model_id}"
                 model=f"{model_prefix}.model.p"
                 feature_arg = f"--feature {args.in_feature}" if args.in_feature is not None else ""
 
                 cmds = []
-                cmds.append(rf"$(info --------------------------------------------------------------)") 
-                cmds.append(rf"$(info Creating LDA for {train_width}um and {n_factor} factors...)") 
-                cmds.append(rf"$(info --------------------------------------------------------------)") 
+                cmds.append(rf"$(info --------------------------------------------------------------)")
+                cmds.append(rf"$(info Creating LDA for {train_width}um and {n_factor} factors...)")
+                cmds.append(rf"$(info --------------------------------------------------------------)")
                 cmds.append(f"mkdir -p {model_path}/figure")
-                cmds.append(f"ficture fit_model --input {hexagon} --output {model_prefix} {feature_arg} --nFactor {n_factor} --epoch {args.train_epoch} --epoch_id_length {args.train_epoch_id_len} --unit_attr X Y --key {args.key_col} --min_ct_per_feature {args.min_ct_feature} --test_split 0.5 --R {args.lda_rand_init} --thread {args.threads}")              
+                cmds.append(f"ficture fit_model --input {hexagon} --output {model_prefix} {feature_arg} --nFactor {n_factor} --epoch {args.train_epoch} --epoch_id_length {args.train_epoch_id_len} --unit_attr X Y --key {args.key_col} --min_ct_per_feature {args.min_ct_feature} --test_split 0.5 --R {args.lda_rand_init} --thread {args.threads}")
 
                 fit_tsv=f"{model_path}/{model_id}.fit_result.tsv.gz"
                 fig_prefix=f"{figure_path}/{model_id}"
                 cmap=f"{figure_path}/{model_id}.rgb.tsv"
                 cmds.append(f"ficture choose_color --input {fit_tsv} --output {fig_prefix} --cmap_name {args.cmap_name}")
 
                 fillr = (train_width / 2 + 1)
                 cmds.append(f"ficture plot_base --input {fit_tsv} --output {fig_prefix}.coarse --fill_range {fillr} --color_table {cmap} --plot_um_per_pixel {args.lda_plot_um_per_pixel} --plot_discretized")
                 cmds.append(f"touch {model_prefix}.done")
 
                 mm.add_target(f"{model_prefix}.done", [args.in_tsv, hexagon], cmds)
-    
+
     if args.decode:
         if not shutil.which(args.bgzip.split(" ")[0]):
             logging.error(f"Cannot find {args.bgzip}. Please make sure that the path to --bgzip is correct")
             sys.exit(1)
-        
+
         if not shutil.which(args.tabix.split(" ")[0]):
             logging.error(f"Cannot find {args.tabix}. Please make sure that the path to --tabix is correct")
             sys.exit(1)
 
 
         script_path = f"{args.out_dir}/sort_decode.sh"
         with open(script_path, "w") as f:
@@ -190,15 +203,15 @@
 coor=$3
 model_id=$4
 bsize=$5
 scale=$6
 topk=$7
 bgzip=$8
 tabix=$9
-                    
+
 K=$( echo $model_id | sed 's/nF\([0-9]\{1,\}\)\..*/\1/' )
 while IFS=$'\t' read -r r_key r_val; do
     export "${r_key}"="${r_val}"
 done < ${coor}
 echo -e "${xmin}, ${xmax}; ${ymin}, ${ymax}"
 
 offsetx=${xmin}
@@ -232,61 +245,61 @@
                     cmds = []
 
                     fit_nmove = int(fit_width / args.anchor_res)
                     anchor_info=f"prj_{fit_width}.r_{args.anchor_res}"
                     radius = args.anchor_res + 1
 
                     prj_prefix = f"{model_path}/{model_id}.{anchor_info}"
-                    cmds.append(rf"$(info --------------------------------------------------------------)") 
-                    cmds.append(rf"$(info Creating projection for {train_width}um and {n_factor} factors, at {fit_width}um)") 
-                    cmds.append(rf"$(info --------------------------------------------------------------)") 
+                    cmds.append(rf"$(info --------------------------------------------------------------)")
+                    cmds.append(rf"$(info Creating projection for {train_width}um and {n_factor} factors, at {fit_width}um)")
+                    cmds.append(rf"$(info --------------------------------------------------------------)")
                     cmds.append(f"ficture transform --input {args.in_tsv} --output_pref {prj_prefix} --model {model} --key {args.key_col} --major_axis {args.major_axis} --hex_width {fit_width} --n_move {fit_nmove} --min_ct_per_unit {args.min_ct_unit_fit} --mu_scale {args.mu_scale} --thread {args.threads} --precision {args.fit_precision}")
 
                     batch_input=f"{args.out_dir}/batched.matrix.tsv.gz"
                     anchor=f"{prj_prefix}.fit_result.tsv.gz"
                     decode_basename=f"{model_id}.decode.{anchor_info}_{radius}"
                     decode_prefix=f"{model_path}/{decode_basename}"
-                    
-                    cmds.append(rf"$(info --------------------------------------------------------------)") 
-                    cmds.append(rf"$(info Performing pixel-level decoding..)") 
-                    cmds.append(rf"$(info --------------------------------------------------------------)") 
+
+                    cmds.append(rf"$(info --------------------------------------------------------------)")
+                    cmds.append(rf"$(info Performing pixel-level decoding..)")
+                    cmds.append(rf"$(info --------------------------------------------------------------)")
                     cmds.append(f"ficture slda_decode --input {batch_in} --output {decode_prefix} --model {model} --anchor {anchor} --anchor_in_um --neighbor_radius {radius} --mu_scale {args.mu_scale} --key {args.key_col} --precision {args.decode_precision} --lite_topk_output_pixel {args.decode_top_k} --lite_topk_output_anchor {args.decode_top_k} --thread {args.threads}")
 
-                    cmds.append(rf"$(info --------------------------------------------------------------)") 
-                    cmds.append(rf"$(info Sorting and reformatting the pixel-level output..)") 
-                    cmds.append(rf"$(info --------------------------------------------------------------)") 
+                    cmds.append(rf"$(info --------------------------------------------------------------)")
+                    cmds.append(rf"$(info Sorting and reformatting the pixel-level output..)")
+                    cmds.append(rf"$(info --------------------------------------------------------------)")
                     cmds.append(f"bash {script_path} {decode_prefix}.pixel.tsv.gz {decode_prefix}.pixel.sorted.tsv.gz {minmax_out} {model_id} {args.decode_block_size} {args.decode_scale} {args.decode_top_k} {args.bgzip} {args.tabix}")
 
                     de_input=f"{decode_prefix}.posterior.count.tsv.gz"
                     de_output=f"{decode_prefix}.bulk_chisq.tsv"
 
-                    cmds.append(rf"$(info --------------------------------------------------------------)") 
-                    cmds.append(rf"$(info Performing pseudo-bulk differential expression analysis..)") 
-                    cmds.append(rf"$(info --------------------------------------------------------------)") 
+                    cmds.append(rf"$(info --------------------------------------------------------------)")
+                    cmds.append(rf"$(info Performing pseudo-bulk differential expression analysis..)")
+                    cmds.append(rf"$(info --------------------------------------------------------------)")
                     cmds.append(f"ficture de_bulk --input {de_input} --output {de_output} --min_ct_per_feature {args.min_ct_feature} --max_pval_output {args.de_max_pval} --min_fold_output {args.de_min_fold} --thread {args.threads}")
 
                     cmap=f"{figure_path}/{model_id}.rgb.tsv"
                     cmds.append(f"ficture factor_report --path {model_path} --pref {decode_basename} --color_table {cmap}")
 
                     decode_tsv=f"{decode_prefix}.pixel.sorted.tsv.gz"
                     decode_png=f"{model_path}/figure/{decode_basename}.pixel.png"
 
-                    cmds.append(rf"$(info --------------------------------------------------------------)") 
-                    cmds.append(rf"$(info Drawing pixel-level output image...)") 
-                    cmds.append(rf"$(info --------------------------------------------------------------)") 
+                    cmds.append(rf"$(info --------------------------------------------------------------)")
+                    cmds.append(rf"$(info Drawing pixel-level output image...)")
+                    cmds.append(rf"$(info --------------------------------------------------------------)")
                     cmds.append(f"ficture plot_pixel_full --input {decode_tsv} --color_table {cmap} --output {decode_png} --plot_um_per_pixel {args.decode_plot_um_per_pixel} --full")
 
                     if args.plot_each_factor:
                         sub_prefix=f"{model_path}/figure/sub/{decode_basename}.pixel"
                         cmds.append(f"mkdir -p {model_path}/figure/sub")
                         cmds.append(f"ficture plot_pixel_single --input {decode_tsv} --output {sub_prefix} --plot_um_per_pixel {args.decode_sub_um_per_pixel} --full --all")
 
                     cmds.append(f"touch {decode_prefix}.done")
                     mm.add_target(f"{decode_prefix}.done", [batch_in, hexagon,f"{model_prefix}.done"], cmds)
-    
+
 
     if len(mm.targets) == 0:
         logging.error("There is no target to run. Please make sure that at least on run option was turned on")
         sys.exit(1)
 
     ## write makefile
     mm.write_makefile(f"{args.out_dir}/Makefile")
@@ -295,8 +308,8 @@
         ## run makefile
         os.system(f"make -f {args.out_dir}/Makefile -n")
         print(f"To execute the pipeline, run the following command:\nmake -f {args.out_dir}/Makefile -j {args.n_jobs}")
     else:
         os.system(f"make -f {args.out_dir}/Makefile -j {args.n_jobs}")
 
 if __name__ == "__main__":
-    run_together(sys.argv[1:])
+    run_together(sys.argv[1:])
```

### Comparing `ficture-0.0.3/ficture/scripts/slda_decode.py` & `ficture-0.0.3.1/ficture/scripts/slda_decode.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     parser.add_argument('--anchor_in_um', action='store_true')
     parser.add_argument('--feature', type=str, default='', help='')
 
     # Data realted parameters
     parser.add_argument('--mu_scale', type=float, default=26.67, help='Coordinate to um translate')
     parser.add_argument('--key', type=str, default = 'gn', help='gt: genetotal, gn: gene, spl: velo-spliced, unspl: velo-unspliced')
     parser.add_argument('--batch_id', type=str, default = 'random_index', help='Input has to have a column with this name indicating the minibatch id')
-    parser.add_argument('--precision', type=float, default=.25, help='If positive, collapse pixels within X um.')
+    parser.add_argument('--precision', type=float, default=.1, help='If positive, collapse pixels within X um.')
 
     # Learning related parameters
     parser.add_argument('--thread', type=int, default=1, help='')
     parser.add_argument('--neighbor_radius', type=float, default=25, help='The radius (um) of each anchor point\'s territory')
     parser.add_argument('--halflife', type=float, default=0.7, help='Control the decay of distance-based weight')
     parser.add_argument('--theta_init_bound_multiplier', type=float, default=.2, help='')
     parser.add_argument('--inner_max_iter', type=int, default=30, help='')
```

### Comparing `ficture-0.0.3/ficture/scripts/transform_univ.py` & `ficture-0.0.3.1/ficture/scripts/transform_univ.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 def transform(_args):
 
     parser = argparse.ArgumentParser(prog = "transform")
     parser.add_argument('--input', type=str, help='')
     parser.add_argument('--output', '--output_pref', type=str, help='')
     parser.add_argument('--model', type=str, help='')
     parser.add_argument('--feature', type=str, default='', help='')
-
     parser.add_argument('--key', type=str, default = 'gn', help='gt: genetotal, gn: gene, spl: velo-spliced, unspl: velo-unspliced')
     parser.add_argument('--major_axis', type=str, default=None, help='X or Y')
     parser.add_argument('--region_id', type=str, default=None, help='')
     parser.add_argument('--min_ct_per_unit', type=int, default=20, help='')
     parser.add_argument('--mu_scale', type=float, default=26.67, help='Coordinate to um translate')
     parser.add_argument('--thread', type=int, default=-1, help='')
     parser.add_argument('--n_move', type=int, default=3, help='')
```

### Comparing `ficture-0.0.3/ficture/utils/filter_fn.py` & `ficture-0.0.3.1/ficture/utils/filter_fn.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.3/ficture/utils/hexagon_fn.py` & `ficture-0.0.3.1/ficture/utils/hexagon_fn.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.3/ficture/utils/image_fn.py` & `ficture-0.0.3.1/ficture/utils/image_fn.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.3/ficture/utils/layout_fn.py` & `ficture-0.0.3.1/ficture/utils/layout_fn.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.3/ficture/utils/mds_color_circle.py` & `ficture-0.0.3.1/ficture/utils/mds_color_circle.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.3/ficture/utils/minimake.py` & `ficture-0.0.3.1/ficture/utils/minimake.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.3/ficture/utils/utilt.py` & `ficture-0.0.3.1/ficture/utils/utilt.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.3/ficture/utils/visualize_factors.py` & `ficture-0.0.3.1/ficture/utils/visualize_factors.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.3/ficture.egg-info/SOURCES.txt` & `ficture-0.0.3.1/ficture.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 ficture/scripts/factor_report.template.html
 ficture/scripts/filter_boundary.py
 ficture/scripts/filter_density.py
 ficture/scripts/filter_poly.py
 ficture/scripts/init_model_selection.py
 ficture/scripts/lda_univ.py
 ficture/scripts/make_dge_univ.py
+ficture/scripts/make_sge_by_hexagon.py
 ficture/scripts/make_spatial_minibatch.py
 ficture/scripts/plot_base.py
 ficture/scripts/plot_hexagon.py
 ficture/scripts/plot_pixel_full.py
 ficture/scripts/plot_pixel_multi.py
 ficture/scripts/plot_pixel_single.py
 ficture/scripts/run_together.py
```

### Comparing `ficture-0.0.3/info/Homo_sapiens.GRCh38.107.names.tsv.gz` & `ficture-0.0.3.1/info/Homo_sapiens.GRCh38.107.names.tsv.gz`

 * *Files identical despite different names*

### Comparing `ficture-0.0.3/info/Mus_musculus.GRCm38.102.names.tsv.gz` & `ficture-0.0.3.1/info/Mus_musculus.GRCm38.102.names.tsv.gz`

 * *Files identical despite different names*

### Comparing `ficture-0.0.3/info/Mus_musculus.GRCm39.107.names.tsv.gz` & `ficture-0.0.3.1/info/Mus_musculus.GRCm39.107.names.tsv.gz`

 * *Files identical despite different names*

### Comparing `ficture-0.0.3/info/gencode.human.mouse.combined.gene.types.tsv.gz` & `ficture-0.0.3.1/info/gencode.human.mouse.combined.gene.types.tsv.gz`

 * *Files identical despite different names*

### Comparing `ficture-0.0.3/info/gencode.human.mouse.combined.gene_names.clean.tsv` & `ficture-0.0.3.1/info/gencode.human.mouse.combined.gene_names.clean.tsv`

 * *Files identical despite different names*

### Comparing `ficture-0.0.3/info/hiseq.layout.tsv` & `ficture-0.0.3.1/info/hiseq.layout.tsv`

 * *Files identical despite different names*

### Comparing `ficture-0.0.3/pyproject.toml` & `ficture-0.0.3.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [project]
 name = "ficture"
 description = "Segmentation free factor analysis for sub-micron resolution spatial transcriptomics"
-version = "0.0.3"
+version = "0.0.3.1"
 authors = [{name = "Yichen Si", email = "ycsi@umich.edu"}]
 license = {text = "CC BY-NC 4.0"}
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = [
     "numpy", "pandas",
     "scipy", "scikit-learn",
     "joblib",
     "matplotlib", "Pillow", "Jinja2", "opencv-python",
     "shapely", "geojson", "geopandas",
-    "torch", "pymde", "ete3", "PyQt5"
+    "ete3", "PyQt5"
 ]
 
 [project.scripts]
 ficture = "ficture.cli:main"
 
 [build-system]
 requires = ["setuptools", "wheel"]
```

