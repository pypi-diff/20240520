# Comparing `tmp/damo-2.3.4.tar.gz` & `tmp/damo-2.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "damo-2.3.4.tar", last modified: Sun May 12 16:23:41 2024, max compression
+gzip compressed data, was "damo-2.3.5.tar", last modified: Mon May 20 18:59:59 2024, max compression
```

## Comparing `damo-2.3.4.tar` & `damo-2.3.5.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-05-12 16:23:41.666266 damo-2.3.4/
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     7492 2024-05-12 16:23:41.666266 damo-2.3.4/PKG-INFO
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     6971 2024-05-12 16:23:38.000000 damo-2.3.4/README.md
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      104 2023-09-30 00:42:34.000000 damo-2.3.4/pyproject.toml
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)       38 2024-05-12 16:23:41.666266 damo-2.3.4/setup.cfg
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1104 2024-05-11 18:53:35.000000 damo-2.3.4/setup.py
-drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-05-12 16:23:41.654266 damo-2.3.4/src/
-drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-05-12 16:23:41.666266 damo-2.3.4/src/damo/
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)        0 2024-05-12 16:23:38.000000 damo-2.3.4/src/damo/__init__.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1442 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/_damo_ascii_color.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     7357 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/_damo_deprecated.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      963 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/_damo_deprecation_notice.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      620 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/_damo_dist.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    10121 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/_damo_fmt_str.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     2356 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/_damo_fs.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     5535 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/_damo_paddr_layout.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      522 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/_damo_print.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    44940 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/_damo_records.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      780 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/_damo_subcmds.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    47260 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/_damon.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    22388 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/_damon_args.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    17432 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/_damon_dbgfs.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    28814 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/_damon_sysfs.py
--rwxr-xr-x   0 sjpark    (1000) sjpark    (1000)     4258 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1858 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_adjust.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1094 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_convert_record_format.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1309 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_features.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1144 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_fmt_json.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    12165 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_heats.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4498 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_lru_sort.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     2860 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_monitor.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     2578 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_nr_regions.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4472 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_reclaim.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     5645 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_record.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     3866 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_record_info.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4278 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_replay.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1587 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_report.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4566 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_report_footprint.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1672 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_report_profile.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     3886 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_report_raw.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1493 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_report_times.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1502 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_schemes.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    26317 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_show.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      520 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_start.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4201 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_status.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      567 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_stop.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      685 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_tune.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     3763 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_validate.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)       22 2024-05-12 16:23:29.000000 damo-2.3.4/src/damo/damo_version.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     6186 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_wss.py
-drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-05-12 16:23:41.666266 damo-2.3.4/src/damo.egg-info/
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     7492 2024-05-12 16:23:41.000000 damo-2.3.4/src/damo.egg-info/PKG-INFO
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1277 2024-05-12 16:23:41.000000 damo-2.3.4/src/damo.egg-info/SOURCES.txt
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)        1 2024-05-12 16:23:41.000000 damo-2.3.4/src/damo.egg-info/dependency_links.txt
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)       40 2024-05-12 16:23:41.000000 damo-2.3.4/src/damo.egg-info/entry_points.txt
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)        5 2024-05-12 16:23:41.000000 damo-2.3.4/src/damo.egg-info/top_level.txt
+drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-05-20 18:59:59.218819 damo-2.3.5/
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     7502 2024-05-20 18:59:59.218819 damo-2.3.5/PKG-INFO
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     6981 2024-05-20 18:59:55.000000 damo-2.3.5/README.md
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      104 2023-09-30 00:42:34.000000 damo-2.3.5/pyproject.toml
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)       38 2024-05-20 18:59:59.218819 damo-2.3.5/setup.cfg
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1104 2024-05-11 18:53:35.000000 damo-2.3.5/setup.py
+drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-05-20 18:59:59.194819 damo-2.3.5/src/
+drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-05-20 18:59:59.214819 damo-2.3.5/src/damo/
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)        0 2024-05-20 18:59:55.000000 damo-2.3.5/src/damo/__init__.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1442 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/_damo_ascii_color.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     7357 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/_damo_deprecated.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      963 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/_damo_deprecation_notice.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      620 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/_damo_dist.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    10121 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/_damo_fmt_str.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     2356 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/_damo_fs.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     5535 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/_damo_paddr_layout.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      522 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/_damo_print.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    44681 2024-05-19 19:03:17.000000 damo-2.3.5/src/damo/_damo_records.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      780 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/_damo_subcmds.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    47260 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/_damon.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    23912 2024-05-19 19:03:17.000000 damo-2.3.5/src/damo/_damon_args.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    17432 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/_damon_dbgfs.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    28814 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/_damon_sysfs.py
+-rwxr-xr-x   0 sjpark    (1000) sjpark    (1000)     4278 2024-05-18 15:38:34.000000 damo-2.3.5/src/damo/damo.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1858 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_adjust.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1094 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_convert_record_format.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1309 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_features.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1144 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_fmt_json.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    12165 2024-05-19 17:56:08.000000 damo-2.3.5/src/damo/damo_heats.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4498 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_lru_sort.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     2860 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_monitor.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     2578 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_nr_regions.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4472 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_reclaim.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     5645 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_record.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     3866 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_record_info.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4278 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_replay.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1587 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_report.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4566 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_report_footprint.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1672 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_report_profile.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     3886 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_report_raw.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1493 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_report_times.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1502 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_schemes.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    26899 2024-05-19 19:34:35.000000 damo-2.3.5/src/damo/damo_show.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      520 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_start.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4201 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_status.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      567 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_stop.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      685 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_tune.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     3763 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_validate.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)       22 2024-05-20 18:59:47.000000 damo-2.3.5/src/damo/damo_version.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     6186 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_wss.py
+drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-05-20 18:59:59.218819 damo-2.3.5/src/damo.egg-info/
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     7502 2024-05-20 18:59:59.000000 damo-2.3.5/src/damo.egg-info/PKG-INFO
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1277 2024-05-20 18:59:59.000000 damo-2.3.5/src/damo.egg-info/SOURCES.txt
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)        1 2024-05-20 18:59:59.000000 damo-2.3.5/src/damo.egg-info/dependency_links.txt
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)       40 2024-05-20 18:59:59.000000 damo-2.3.5/src/damo.egg-info/entry_points.txt
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)        5 2024-05-20 18:59:59.000000 damo-2.3.5/src/damo.egg-info/top_level.txt
```

### Comparing `damo-2.3.4/PKG-INFO` & `damo-2.3.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damo
-Version: 2.3.4
+Version: 2.3.5
 Summary: DAMON user-space tool
 Home-page: https://github.com/awslabs/damo
 Author: SeongJae Park
 Author-email: sj@kernel.org
 Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
 Project-URL: DAMON, https://damonitor.github.io
 Classifier: Programming Language :: Python :: 3
@@ -38,25 +38,25 @@
 
 [![Packaging status](https://repology.org/badge/vertical-allrepos/damo.svg)](https://repology.org/project/damo/versions)
 
 Follow below instructions and commands to monitor and visualize the access
 pattern of your workload.
 
     $ # ensure DAMON is enabled on your kernel
-    $ # install damo from PyPI, or use your distribution's package manager
-    $ sudo pip3 install damo
+    $ # install damo using packaging systems listed above,
+    $ # or cloning the source repo and updating $PATH.
     $ sudo damo show $(pidof <your workload>)
     $ sudo damo record $(pidof <your workload>)
     $ sudo damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The second and last commands will show the access pattern of your workload,
 like below:
 
 ![masim_stairs_snapshot](images/masim_stairs_snapshot.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.3.4/images/masim_stairs_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.3.5/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I ensure DAMON is enabled on my kernel?
 -----------------------------------------------
@@ -64,15 +64,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.4/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.5/USAGE.md) file.
 
 
 What does the version numbers mean?
 -----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -92,15 +92,15 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some features are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.4/USAGE.md) file?
+Why some features are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.5/USAGE.md) file?
 ------------------------------------------------------------------
 
 Because those are not yet stabilized.  In other words, such features are in
 their experimental stages, and therefore could be deprecated and removed
 without notice and grace periods.  The documented features could also be
 deprecated, but those will provide some notifications and grace periods.  If
 there are some features you're relying on but not documented, please
@@ -115,15 +115,15 @@
 [FEATURES_DEPRECATION_SCHEDULE.md](FEATURES_DEPRECATION_SCHEDULE.md) file.
 
 
 Quick Intro for Major Features
 ==============================
 
 Below are quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.4/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.5/USAGE.md) file.
 
 
 Snapshot Data Access Pattern
 ----------------------------
 
 Below commands repeatedly get a snapshot of the access pattern of a program for
 every second.
```

### Comparing `damo-2.3.4/README.md` & `damo-2.3.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -23,25 +23,25 @@
 
 [![Packaging status](https://repology.org/badge/vertical-allrepos/damo.svg)](https://repology.org/project/damo/versions)
 
 Follow below instructions and commands to monitor and visualize the access
 pattern of your workload.
 
     $ # ensure DAMON is enabled on your kernel
-    $ # install damo from PyPI, or use your distribution's package manager
-    $ sudo pip3 install damo
+    $ # install damo using packaging systems listed above,
+    $ # or cloning the source repo and updating $PATH.
     $ sudo damo show $(pidof <your workload>)
     $ sudo damo record $(pidof <your workload>)
     $ sudo damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The second and last commands will show the access pattern of your workload,
 like below:
 
 ![masim_stairs_snapshot](images/masim_stairs_snapshot.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.3.4/images/masim_stairs_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.3.5/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I ensure DAMON is enabled on my kernel?
 -----------------------------------------------
@@ -49,15 +49,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.4/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.5/USAGE.md) file.
 
 
 What does the version numbers mean?
 -----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -77,15 +77,15 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some features are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.4/USAGE.md) file?
+Why some features are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.5/USAGE.md) file?
 ------------------------------------------------------------------
 
 Because those are not yet stabilized.  In other words, such features are in
 their experimental stages, and therefore could be deprecated and removed
 without notice and grace periods.  The documented features could also be
 deprecated, but those will provide some notifications and grace periods.  If
 there are some features you're relying on but not documented, please
@@ -100,15 +100,15 @@
 [FEATURES_DEPRECATION_SCHEDULE.md](FEATURES_DEPRECATION_SCHEDULE.md) file.
 
 
 Quick Intro for Major Features
 ==============================
 
 Below are quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.4/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.5/USAGE.md) file.
 
 
 Snapshot Data Access Pattern
 ----------------------------
 
 Below commands repeatedly get a snapshot of the access pattern of a program for
 every second.
```

### Comparing `damo-2.3.4/setup.py` & `damo-2.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.4/src/damo/_damo_ascii_color.py` & `damo-2.3.5/src/damo/_damo_ascii_color.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.4/src/damo/_damo_deprecated.py` & `damo-2.3.5/src/damo/_damo_deprecated.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.4/src/damo/_damo_deprecation_notice.py` & `damo-2.3.5/src/damo/_damo_deprecation_notice.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.4/src/damo/_damo_dist.py` & `damo-2.3.5/src/damo/_damo_dist.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.4/src/damo/_damo_fmt_str.py` & `damo-2.3.5/src/damo/_damo_fmt_str.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.4/src/damo/_damo_fs.py` & `damo-2.3.5/src/damo/_damo_fs.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.4/src/damo/_damo_paddr_layout.py` & `damo-2.3.5/src/damo/_damo_paddr_layout.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.4/src/damo/_damo_print.py` & `damo-2.3.5/src/damo/_damo_print.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.4/src/damo/_damo_records.py` & `damo-2.3.5/src/damo/_damo_records.py`

 * *Files 1% similar despite different names*

```diff
@@ -494,15 +494,15 @@
             file_permission)
 
 def update_records_file(file_path, file_format, file_permission=None,
         monitoring_intervals=None):
     return rewrite_record_file(file_path, file_path, file_format,
             file_permission, monitoring_intervals)
 
-# memory footprint recording
+# for recording
 
 # Meaning of the fileds of ProcMemFootprint are as below.
 #
 # ======== ===============================       ==============================
 # Field    Content
 # ======== ===============================       ==============================
 # size     total program size (pages)            (same as VmSize in status)
@@ -651,38 +651,16 @@
     os.chmod(filepath, file_permission)
 
 def load_mem_footprint(filepath):
     with open(filepath, 'r') as f:
         kvpairs = json.load(f)
     return [MemFootprintsSnapshot.from_kvpairs(x) for x in kvpairs]
 
-# record-polling
-
-def pid_running(pid):
-    '''pid should be string'''
-    try:
-        subprocess.check_output(['ps', '--pid', pid])
-        return True
-    except:
-        return False
-
-def all_targets_terminated(targets):
-    for target in targets:
-        if pid_running('%s' % target.pid):
-            return False
-    return True
-
-def __poll_target_pids(kdamonds, add_childs):
-    '''Return if polling should continued'''
-
+def add_childs_target(kdamonds):
     current_targets = kdamonds[0].contexts[0].targets
-    if all_targets_terminated(current_targets):
-        return False
-    if not add_childs:
-        return True
 
     for target in current_targets:
         if target.pid == None:
             continue
         try:
             childs_pids = subprocess.check_output(
                     ['ps', '--ppid', '%s' % target.pid, '-o', 'pid=']
@@ -705,35 +683,44 @@
             new_targets.append(_damon.DamonTarget(pid=child_pid, regions=[]))
         if new_targets == []:
             continue
 
         # commit the new set of targets
         kdamonds[0].contexts[0].targets = new_targets
         err = _damon.commit(kdamonds)
-        if err != None:
-            # this might be not a problem; some of processes might
-            # finished meanwhile
+        if err is not None:
+            return 'commit failed (%s)' % err
+    return None
+
+def pid_running(pid):
+    '''pid should be string'''
+    try:
+        subprocess.check_output(['ps', '--pid', pid])
+        return True
+    except:
+        return False
+
+def all_targets_terminated(targets):
+    for target in targets:
+        if pid_running('%s' % target.pid):
             return False
     return True
 
-def poll_target_pids(kdamonds, add_childs):
-    has_pid_target = False
-    if kdamonds:
-        for kdamond in kdamonds:
-            for ctx in kdamond.contexts:
-                if _damon.target_has_pid(ctx.ops):
-                    has_pid_target = True
-                    break
-            if has_pid_target:
-                break
-    if has_pid_target is False:
+def poll_target_pids(kdamonds):
+    '''Return True if >=1 target processes are running'''
+    has_running_process = False
+    if not kdamonds:
         return False
-    return __poll_target_pids(kdamonds, add_childs)
-
-# for recording
+    for kdamond in kdamonds:
+        for ctx in kdamond.contexts:
+            if not _damon.target_has_pid(ctx.ops):
+                continue
+            if not all_targets_terminated(ctx.targets):
+                return True
+    return False
 
 class RecordingHandle:
     # for tracepoint recording
     tracepoint = None
     file_path = None
     file_format = None
     file_permission = None
@@ -770,16 +757,19 @@
     if handle.tracepoint is not None:
         handle.perf_pipe = subprocess.Popen(
                 [PERF, 'record', '-a', '-e', handle.tracepoint,
                  '-o', handle.file_path])
     if handle.do_profile:
         cmd = [PERF, 'record', '-o', '%s.profile' % handle.file_path]
         handle.perf_profile_pipe = subprocess.Popen(cmd)
-    while (poll_target_pids(handle.kdamonds, handle.add_child_tasks) or
+    while (poll_target_pids(handle.kdamonds) or
            _damon.any_kdamond_running()):
+        if handle.add_child_tasks is True:
+            add_childs_target(handle.kdamonds)
+
         if handle.mem_footprint_snapshots is not None:
             record_mem_footprint(handle.kdamonds,
                                  handle.mem_footprint_snapshots)
         time.sleep(1)
 
 def finish_recording(handle):
     try:
```

### Comparing `damo-2.3.4/src/damo/_damo_subcmds.py` & `damo-2.3.5/src/damo/_damo_subcmds.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.4/src/damo/_damon.py` & `damo-2.3.5/src/damo/_damon.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.4/src/damo/_damon_args.py` & `damo-2.3.5/src/damo/_damon_args.py`

 * *Files 5% similar despite different names*

```diff
@@ -148,40 +148,46 @@
     if nr_cmd_args >= 5:
         weights[1] = cmd_args[4]
     if nr_cmd_args >= 6:
         weights[2] = cmd_args[5]
 
     return [time_ms, sz_bytes, reset_interval_ms, weights]
 
+def damos_options_to_quotas(quotas, goals):
+    gargs = goals
+    # garg should be <metric> <target value> [current value]
+    # [current value] is given for only 'user_input' <metric>
+    for garg in gargs:
+        if not len(garg) in [2, 3]:
+            return None, 'Wrong --damos_quota_goal (%s)' % garg
+        if garg[0] == 'user_input' and len(garg) != 3:
+            return None, 'Wrong --damos_quota_goal (%s)' % garg
+        if garg[0] != 'user_input' and len(garg) != 2:
+            return None, 'Wrong --damos_quota_goal (%s)' % garg
+    try:
+        goals = [_damon.DamosQuotaGoal(*garg) for garg in gargs]
+    except Exception as e:
+        return None, 'Wrong --damos_quota_goal (%s, %s)' % (gargs, e)
+
+    qargs = quotas
+    if len(qargs) > 6:
+        return None, 'Wrong --damos_quotas (%s, >6 parameters)' % qargs
+    try:
+        quotas = _damon.DamosQuotas(*damos_quotas_cons_arg(qargs),
+                                    goals=goals)
+    except Exception as e:
+        return None, 'Wrong --damos_quotas (%s, %s)' % (qargs, e)
+    return quotas, None
+
 def damos_options_to_scheme(sz_region, access_rate, age, action,
         apply_interval, quotas, goals, wmarks, filters):
     if quotas != None:
-        gargs = goals
-        # garg should be <metric> <target value> [current value]
-        # [current value] is given for only 'user_input' <metric>
-        for garg in gargs:
-            if not len(garg) in [2, 3]:
-                return None, 'Wrong --damos_quota_goal (%s)' % garg
-            if garg[0] == 'user_input' and len(garg) != 3:
-                return None, 'Wrong --damos_quota_goal (%s)' % garg
-            if garg[0] != 'user_input' and len(garg) != 2:
-                return None, 'Wrong --damos_quota_goal (%s)' % garg
-        try:
-            goals = [_damon.DamosQuotaGoal(*garg) for garg in gargs]
-        except Exception as e:
-            return None, 'Wrong --damos_quota_goal (%s, %s)' % (gargs, e)
-
-        qargs = quotas
-        if len(qargs) > 6:
-            return None, 'Wrong --damos_quotas (%s, >6 parameters)' % qargs
-        try:
-            quotas = _damon.DamosQuotas(*damos_quotas_cons_arg(qargs),
-                                        goals=goals)
-        except Exception as e:
-            return None, 'Wrong --damos_quotas (%s, %s)' % (qargs, e)
+        quotas, err = damos_options_to_quotas(quotas, goals)
+        if err is not None:
+            return None, err
 
     if wmarks != None:
         wargs = wmarks
         try:
             wmarks = _damon.DamosWatermarks(wargs[0], wargs[1], wargs[2],
                     wargs[3], wargs[4])
         except Exception as e:
@@ -197,14 +203,26 @@
                     access_rate, _damon.unit_percent, age, _damon.unit_usec),
                 action=action, apply_interval_us=apply_interval, quotas=quotas,
                 watermarks=wmarks, filters=filters), None
     except Exception as e:
         return None, 'Wrong \'--damos_*\' argument (%s)' % e
 
 def damos_options_to_schemes(args):
+    if args.damos_quota_interval:
+        for i, interval in enumerate(args.damos_quota_interval):
+            t, s = 0, 0
+            if i < len(args.damos_quota_time):
+                t = args.damos_quota_time[i]
+            if i < len(args.damos_quota_space):
+                s = args.damos_quota_space[i]
+            if i < len(args.damos_quota_weights):
+                w1, w2, w3 = args.damos_quota_weights[i]
+            else:
+                w1, w2, w3 = 1, 1, 1
+            args.damos_quotas.append([t, s, interval, w1, w2, w3])
     nr_schemes = len(args.damos_action)
     if len(args.damos_sz_region) > nr_schemes:
         return [], 'too much --damos_sz_region'
     if len(args.damos_access_rate) > nr_schemes:
         return [], 'too much --damos_access_rate'
     if len(args.damos_age) > nr_schemes:
         return [], 'too much --damos_age'
@@ -381,21 +399,24 @@
     '''
     if not args.damos_action:
         for key, value in args.__dict__.items():
             if key.startswith('damos_') and len(value):
                 if key == 'damos_action': continue
                 return False, '\'damos_action\' not specified while using --damos_* option(s)'
 
+    if len(args.damos_quotas) > 0 and len(args.damos_quota_interval) > 0:
+        return False, '--damos_quotas and --damos_quota_interval cannot passed together'
+
     '''
     Verify if 'reset_interval_ms' is specified in args when setting quota goals
     '''
     if args.damos_quota_goal:
         damos_quotas = args.damos_quotas
 
-        if not len(damos_quotas):
+        if not len(damos_quotas) and not len(args.damos_quota_interval):
             return False, '\'reset_interval_ms\' not specified when setting quota goals'
 
         #reset_interval_ms is specified in --damos_quotas as 3rd arg
         for quota in damos_quotas:
             if len(quota) < 3:
                 return False, '\'reset_interval_ms\' not specified when setting quota goals'
 
@@ -523,14 +544,25 @@
     parser.add_argument('--damos_quotas', default=[],
             metavar='<quota parameter>', nargs='+', action='append',
             help=' '.join([
             'damos quotas (<time (ms)> [<size (bytes)> [<reset interval (ms)>',
                 '[<size priority weight (permil)>',
                 '[<access rate priority weight> (permil)',
                 '[<age priority weight> (permil)]]]]])']))
+    parser.add_argument('--damos_quota_interval', default=[],
+                        metavar='<milliseconds>', action='append',
+                        help='quota reset interval')
+    parser.add_argument('--damos_quota_time', default=[],
+                        metavar='<milliseconds>', action='append',
+                        help='time quota')
+    parser.add_argument('--damos_quota_space', default=[], metavar='<bytes>',
+                        action='append', help='space quota')
+    parser.add_argument('--damos_quota_weights', default=[],
+                        metavar='<permil>', nargs=3, action='append',
+                        help='quota\'s prioritization weights')
     parser.add_argument('--damos_quota_goal', nargs='+', action='append',
             default=[],
             metavar='<metric or value>',
             help=' '.join([
                 'damos quota goal (<metric> <target value> [current value]).',
                 '<metric> shoule be {%s}.' %
                 ','.join(_damon.qgoal_metrics)]))
```

### Comparing `damo-2.3.4/src/damo/_damon_dbgfs.py` & `damo-2.3.5/src/damo/_damon_dbgfs.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.4/src/damo/_damon_sysfs.py` & `damo-2.3.5/src/damo/_damon_sysfs.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.4/src/damo/damo.py` & `damo-2.3.5/src/damo/damo.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 # SPDX-License-Identifier: GPL-2.0
 
 import argparse
 import os
 
-os.sys.path.insert(0, os.path.dirname(os.path.abspath(__file__)))
+damo_dir = os.path.dirname(os.path.abspath(__file__))
+os.sys.path.insert(0, damo_dir)
 import sys
 
 import _damo_subcmds
 import damo_adjust
 import damo_convert_record_format
 import damo_features
 import damo_fmt_json
```

### Comparing `damo-2.3.4/src/damo/damo_adjust.py` & `damo-2.3.5/src/damo/damo_adjust.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.4/src/damo/damo_convert_record_format.py` & `damo-2.3.5/src/damo/damo_convert_record_format.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.4/src/damo/damo_features.py` & `damo-2.3.5/src/damo/damo_features.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.4/src/damo/damo_fmt_json.py` & `damo-2.3.5/src/damo/damo_fmt_json.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.4/src/damo/damo_heats.py` & `damo-2.3.5/src/damo/damo_heats.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.4/src/damo/damo_lru_sort.py` & `damo-2.3.5/src/damo/damo_lru_sort.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.4/src/damo/damo_monitor.py` & `damo-2.3.5/src/damo/damo_monitor.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.4/src/damo/damo_nr_regions.py` & `damo-2.3.5/src/damo/damo_nr_regions.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.4/src/damo/damo_reclaim.py` & `damo-2.3.5/src/damo/damo_reclaim.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.4/src/damo/damo_record.py` & `damo-2.3.5/src/damo/damo_record.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.4/src/damo/damo_record_info.py` & `damo-2.3.5/src/damo/damo_record_info.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.4/src/damo/damo_replay.py` & `damo-2.3.5/src/damo/damo_replay.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.4/src/damo/damo_report.py` & `damo-2.3.5/src/damo/damo_report.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.4/src/damo/damo_report_footprint.py` & `damo-2.3.5/src/damo/damo_report_footprint.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.4/src/damo/damo_report_profile.py` & `damo-2.3.5/src/damo/damo_report_profile.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.4/src/damo/damo_report_raw.py` & `damo-2.3.5/src/damo/damo_report_raw.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.4/src/damo/damo_report_times.py` & `damo-2.3.5/src/damo/damo_report_times.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.4/src/damo/damo_schemes.py` & `damo-2.3.5/src/damo/damo_schemes.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.4/src/damo/damo_show.py` & `damo-2.3.5/src/damo/damo_show.py`

 * *Files 8% similar despite different names*

```diff
@@ -417,34 +417,36 @@
             args.format_region = '<box>%s' % default_region_format
         else:
             args.format_region = '<box>\n%s' % default_region_format
         if args.format_snapshot_tail.find('<region box description>') == -1:
             args.format_snapshot_tail = ('%s\n<region box description>' %
                     args.format_record_tail)
 
+def temperature_of(region):
+    if region.nr_accesses.percent > 0:
+        return region.nr_accesses.percent * region.age.usec
+    else:
+        return -1 * region.age.usec
+
 def sorted_regions(regions, sort_fields, sort_dsc_keys):
     for field in sort_fields:
+        dsc = sort_dsc_keys != None and ('all' in sort_dsc_keys or
+                                         field in sort_dsc_keys)
         if field == 'address':
-            dsc = sort_dsc_keys != None and ('all' in sort_dsc_keys or
-                    'address' in sort_dsc_keys)
             regions = sorted(regions, key=lambda r: r.start, reverse=dsc)
         elif field == 'access_rate':
-            dsc = sort_dsc_keys != None and ('all' in sort_dsc_keys or
-                    'access_rate' in sort_dsc_keys)
             regions = sorted(regions, key=lambda r: r.nr_accesses.percent,
                     reverse=dsc)
         elif field == 'age':
-            dsc = sort_dsc_keys != None and ('all' in sort_dsc_keys or
-                    'age' in sort_dsc_keys)
-            regions = sorted(regions, key=lambda r: r.age.usec,
-                    reverse=dsc)
+            regions = sorted(regions, key=lambda r: r.age.usec, reverse=dsc)
         elif field == 'size':
-            dsc = sort_dsc_keys != None and ('all' in sort_dsc_keys or
-                    'size' in sort_dsc_keys)
             regions = sorted(regions, key=lambda r: r.size(), reverse=dsc)
+        elif field == 'temperature':
+            regions = sorted(regions, key=lambda r: temperature_of(r),
+                             reverse=dsc)
     return regions
 
 def pr_records(args, records):
     if args.json:
         _damo_print.pr_with_pager_if_needed(
                 json.dumps([r.to_kvpairs(args.raw_number) for r in records],
                            indent=4))
@@ -518,14 +520,21 @@
     return False
 
 def main(args):
     handled = handle_ls_keywords(args)
     if handled:
         return
 
+    if args.style == 'simple-boxes':
+        args.format_region = '<box> size <size> access rate <access rate> age <age>'
+        args.region_box_min_max_height = [1, 1]
+        args.region_box_min_max_length = [1, 40]
+        args.region_box_align = 'right'
+        args.region_box_colorset = 'emotion'
+
     args.region_box_values = [v if v != 'none' else None
             for v in args.region_box_values]
 
     record_filter, err = _damo_records.args_to_filter(args)
     if err != None:
         print(err)
         exit(1)
@@ -562,21 +571,28 @@
     parser.add_argument('--input_file', metavar='<file>',
             help='source of the access pattern to show')
     parser.add_argument('--tried_regions_of', nargs=3, type=int,
             action='append',
             metavar=('<kdamond idx>', '<context idx>', '<scheme idx>'),
             help='show tried regions of given schemes')
 
-    # how to show
-    parser.add_argument('--sort_regions_by',
-            choices=['address', 'access_rate', 'age', 'size'], nargs='+',
+    # how to show, in simple selection
+    parser.add_argument(
+            '--style', choices=['detailed', 'simple-boxes'],
+            default='detailed',
+            help='output format selection among pre-configures ones')
+    # how to show, in highly tunable way
+    parser.add_argument(
+            '--sort_regions_by', nargs='+',
+            choices=['address', 'access_rate', 'age', 'size', 'temperature'],
             default=['address'],
             help='fields to sort regions by')
     parser.add_argument('--sort_regions_dsc',
-            choices=['address', 'access_rate', 'age', 'size', 'all'],
+            choices=['address', 'access_rate', 'age', 'size', 'temperature',
+                     'all'],
             nargs='+',
             help='sort regions in descending order for the given keys')
     parser.add_argument('--dont_merge_regions', action='store_true',
             help='don\'t merge contiguous regions of same access pattern')
 
     # don't set default for record head and snapshot head because it depends on
     # given number of record and snapshots.  Decide those in set_formats().
```

### Comparing `damo-2.3.4/src/damo/damo_start.py` & `damo-2.3.5/src/damo/damo_start.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.4/src/damo/damo_status.py` & `damo-2.3.5/src/damo/damo_status.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.4/src/damo/damo_stop.py` & `damo-2.3.5/src/damo/damo_stop.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.4/src/damo/damo_tune.py` & `damo-2.3.5/src/damo/damo_tune.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.4/src/damo/damo_validate.py` & `damo-2.3.5/src/damo/damo_validate.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.4/src/damo/damo_wss.py` & `damo-2.3.5/src/damo/damo_wss.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.4/src/damo.egg-info/PKG-INFO` & `damo-2.3.5/src/damo.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damo
-Version: 2.3.4
+Version: 2.3.5
 Summary: DAMON user-space tool
 Home-page: https://github.com/awslabs/damo
 Author: SeongJae Park
 Author-email: sj@kernel.org
 Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
 Project-URL: DAMON, https://damonitor.github.io
 Classifier: Programming Language :: Python :: 3
@@ -38,25 +38,25 @@
 
 [![Packaging status](https://repology.org/badge/vertical-allrepos/damo.svg)](https://repology.org/project/damo/versions)
 
 Follow below instructions and commands to monitor and visualize the access
 pattern of your workload.
 
     $ # ensure DAMON is enabled on your kernel
-    $ # install damo from PyPI, or use your distribution's package manager
-    $ sudo pip3 install damo
+    $ # install damo using packaging systems listed above,
+    $ # or cloning the source repo and updating $PATH.
     $ sudo damo show $(pidof <your workload>)
     $ sudo damo record $(pidof <your workload>)
     $ sudo damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The second and last commands will show the access pattern of your workload,
 like below:
 
 ![masim_stairs_snapshot](images/masim_stairs_snapshot.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.3.4/images/masim_stairs_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.3.5/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I ensure DAMON is enabled on my kernel?
 -----------------------------------------------
@@ -64,15 +64,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.4/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.5/USAGE.md) file.
 
 
 What does the version numbers mean?
 -----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -92,15 +92,15 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some features are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.4/USAGE.md) file?
+Why some features are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.5/USAGE.md) file?
 ------------------------------------------------------------------
 
 Because those are not yet stabilized.  In other words, such features are in
 their experimental stages, and therefore could be deprecated and removed
 without notice and grace periods.  The documented features could also be
 deprecated, but those will provide some notifications and grace periods.  If
 there are some features you're relying on but not documented, please
@@ -115,15 +115,15 @@
 [FEATURES_DEPRECATION_SCHEDULE.md](FEATURES_DEPRECATION_SCHEDULE.md) file.
 
 
 Quick Intro for Major Features
 ==============================
 
 Below are quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.4/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.5/USAGE.md) file.
 
 
 Snapshot Data Access Pattern
 ----------------------------
 
 Below commands repeatedly get a snapshot of the access pattern of a program for
 every second.
```

### Comparing `damo-2.3.4/src/damo.egg-info/SOURCES.txt` & `damo-2.3.5/src/damo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

