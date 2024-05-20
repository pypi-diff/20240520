# Comparing `tmp/braingraphstudio-0.1.0.tar.gz` & `tmp/braingraphstudio-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/braingraphstudio-0.1.0.tar", last modified: Mon May 13 21:46:02 2024, max compression
+gzip compressed data, was "dist/braingraphstudio-0.1.1.tar", last modified: Mon May 20 18:21:39 2024, max compression
```

## Comparing `braingraphstudio-0.1.0.tar` & `braingraphstudio-0.1.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2024-05-13 21:46:02.992246 braingraphstudio-0.1.0/
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2024-05-13 21:46:02.951309 braingraphstudio-0.1.0/BrainGraphStudio/
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2024-05-13 21:46:02.955240 braingraphstudio-0.1.0/BrainGraphStudio/BrainGB/
--rw-r--r--   0 berk       (502) staff       (20)        0 2024-05-13 08:15:27.000000 braingraphstudio-0.1.0/BrainGraphStudio/BrainGB/__init__.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2024-05-13 21:46:02.955690 braingraphstudio-0.1.0/BrainGraphStudio/BrainGB/src/
--rw-r--r--   0 berk       (502) staff       (20)        0 2024-05-13 08:15:27.000000 braingraphstudio-0.1.0/BrainGraphStudio/BrainGB/src/__init__.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2024-05-13 21:46:02.961837 braingraphstudio-0.1.0/BrainGraphStudio/BrainGB/src/dataset/
--rw-r--r--   0 berk       (502) staff       (20)       74 2024-05-13 08:15:27.000000 braingraphstudio-0.1.0/BrainGraphStudio/BrainGB/src/dataset/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)      127 2024-05-13 08:15:27.000000 braingraphstudio-0.1.0/BrainGraphStudio/BrainGB/src/dataset/base_transform.py
--rw-r--r--   0 berk       (502) staff       (20)      613 2024-05-13 08:15:27.000000 braingraphstudio-0.1.0/BrainGraphStudio/BrainGB/src/dataset/brain_data.py
--rw-r--r--   0 berk       (502) staff       (20)     4406 2024-05-13 08:15:27.000000 braingraphstudio-0.1.0/BrainGraphStudio/BrainGB/src/dataset/brain_dataset.py
--rw-r--r--   0 berk       (502) staff       (20)      250 2024-05-13 08:15:27.000000 braingraphstudio-0.1.0/BrainGraphStudio/BrainGB/src/dataset/maskable_list.py
--rw-r--r--   0 berk       (502) staff       (20)     6455 2024-05-13 08:15:27.000000 braingraphstudio-0.1.0/BrainGraphStudio/BrainGB/src/dataset/transforms.py
--rw-r--r--   0 berk       (502) staff       (20)     2502 2024-05-13 08:15:27.000000 braingraphstudio-0.1.0/BrainGraphStudio/BrainGB/src/dataset/utils.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2024-05-13 21:46:02.969499 braingraphstudio-0.1.0/BrainGraphStudio/BrainGB/src/models/
--rw-r--r--   0 berk       (502) staff       (20)       92 2024-05-13 08:15:27.000000 braingraphstudio-0.1.0/BrainGraphStudio/BrainGB/src/models/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)      696 2024-05-13 08:15:27.000000 braingraphstudio-0.1.0/BrainGraphStudio/BrainGB/src/models/brainnn.py
--rw-r--r--   0 berk       (502) staff       (20)     6347 2024-05-13 08:15:27.000000 braingraphstudio-0.1.0/BrainGraphStudio/BrainGB/src/models/gat.py
--rw-r--r--   0 berk       (502) staff       (20)     5862 2024-05-13 08:15:27.000000 braingraphstudio-0.1.0/BrainGraphStudio/BrainGB/src/models/gcn.py
--rw-r--r--   0 berk       (502) staff       (20)     2915 2024-05-13 08:15:27.000000 braingraphstudio-0.1.0/BrainGraphStudio/BrainGB/src/models/losses.py
--rw-r--r--   0 berk       (502) staff       (20)      823 2024-05-13 08:15:27.000000 braingraphstudio-0.1.0/BrainGraphStudio/BrainGB/src/models/mlp.py
--rw-r--r--   0 berk       (502) staff       (20)     2226 2024-05-13 08:15:27.000000 braingraphstudio-0.1.0/BrainGraphStudio/BrainGB/src/models/pna.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2024-05-13 21:46:02.974322 braingraphstudio-0.1.0/BrainGraphStudio/BrainGB/src/utils/
--rw-r--r--   0 berk       (502) staff       (20)      109 2024-05-13 08:15:27.000000 braingraphstudio-0.1.0/BrainGraphStudio/BrainGB/src/utils/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)      570 2024-05-13 08:15:27.000000 braingraphstudio-0.1.0/BrainGraphStudio/BrainGB/src/utils/bin_edges.py
--rw-r--r--   0 berk       (502) staff       (20)      209 2024-05-13 08:15:27.000000 braingraphstudio-0.1.0/BrainGraphStudio/BrainGB/src/utils/get_y.py
--rw-r--r--   0 berk       (502) staff       (20)     1684 2024-05-13 08:15:27.000000 braingraphstudio-0.1.0/BrainGraphStudio/BrainGB/src/utils/mixup.py
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-12-20 08:58:35.000000 braingraphstudio-0.1.0/BrainGraphStudio/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)     5534 2024-05-13 07:52:56.000000 braingraphstudio-0.1.0/BrainGraphStudio/__main__.py
--rw-r--r--   0 berk       (502) staff       (20)     3807 2024-05-13 08:05:13.000000 braingraphstudio-0.1.0/BrainGraphStudio/data.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2024-05-13 21:46:02.977070 braingraphstudio-0.1.0/BrainGraphStudio/gui/
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-12-20 08:49:33.000000 braingraphstudio-0.1.0/BrainGraphStudio/gui/__init__.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2024-05-13 21:46:02.978555 braingraphstudio-0.1.0/BrainGraphStudio/gui/ims/
--rw-r--r--   0 berk       (502) staff       (20)        0 2024-04-22 21:09:31.000000 braingraphstudio-0.1.0/BrainGraphStudio/gui/ims/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)    27281 2024-05-13 21:00:52.000000 braingraphstudio-0.1.0/BrainGraphStudio/gui/pages.py
--rw-r--r--   0 berk       (502) staff       (20)     3272 2024-05-13 02:52:12.000000 braingraphstudio-0.1.0/BrainGraphStudio/gui/utils.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2024-05-13 21:46:02.982026 braingraphstudio-0.1.0/BrainGraphStudio/models/
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-09-11 00:39:15.000000 braingraphstudio-0.1.0/BrainGraphStudio/models/__init__.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2024-05-13 21:46:02.986917 braingraphstudio-0.1.0/BrainGraphStudio/models/brainGNN/
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-12-20 08:37:40.000000 braingraphstudio-0.1.0/BrainGraphStudio/models/brainGNN/__init__.py
--rw-r--r--   0 berk       (502) staff       (20)     3798 2024-04-22 21:55:16.000000 braingraphstudio-0.1.0/BrainGraphStudio/models/brainGNN/braingnn.py
--rw-r--r--   0 berk       (502) staff       (20)     2865 2024-04-22 21:56:55.000000 braingraphstudio-0.1.0/BrainGraphStudio/models/brainGNN/braingraphconv.py
--rw-r--r--   0 berk       (502) staff       (20)     6458 2024-04-23 07:06:45.000000 braingraphstudio-0.1.0/BrainGraphStudio/models/brainGNN/brainmsgpassing.py
--rw-r--r--   0 berk       (502) staff       (20)      617 2023-12-20 08:42:32.000000 braingraphstudio-0.1.0/BrainGraphStudio/models/brainGNN/inits.py
--rw-r--r--   0 berk       (502) staff       (20)      573 2024-05-06 22:01:44.000000 braingraphstudio-0.1.0/BrainGraphStudio/models/brainGNN/loss.py
--rw-r--r--   0 berk       (502) staff       (20)     4135 2024-05-13 18:59:50.000000 braingraphstudio-0.1.0/BrainGraphStudio/models/model.py
--rw-r--r--   0 berk       (502) staff       (20)     2677 2024-01-01 12:59:54.000000 braingraphstudio-0.1.0/BrainGraphStudio/models/params.py
--rw-r--r--   0 berk       (502) staff       (20)        0 2024-04-15 20:28:59.000000 braingraphstudio-0.1.0/BrainGraphStudio/models/train.py
--rw-r--r--   0 berk       (502) staff       (20)        0 2023-12-20 09:08:56.000000 braingraphstudio-0.1.0/BrainGraphStudio/models/utils.py
--rw-r--r--   0 berk       (502) staff       (20)     1712 2024-05-13 02:57:07.000000 braingraphstudio-0.1.0/BrainGraphStudio/nni.py
--rw-r--r--   0 berk       (502) staff       (20)     3005 2024-05-13 18:28:24.000000 braingraphstudio-0.1.0/BrainGraphStudio/utils.py
-drwxr-xr-x   0 berk       (502) staff       (20)        0 2024-05-13 21:46:02.988313 braingraphstudio-0.1.0/BrainGraphStudio.egg-info/
--rw-r--r--   0 berk       (502) staff       (20)     4742 2024-05-13 21:46:02.000000 braingraphstudio-0.1.0/BrainGraphStudio.egg-info/PKG-INFO
--rw-r--r--   0 berk       (502) staff       (20)     1902 2024-05-13 21:46:02.000000 braingraphstudio-0.1.0/BrainGraphStudio.egg-info/SOURCES.txt
--rw-r--r--   0 berk       (502) staff       (20)        1 2024-05-13 21:46:02.000000 braingraphstudio-0.1.0/BrainGraphStudio.egg-info/dependency_links.txt
--rw-r--r--   0 berk       (502) staff       (20)       55 2024-05-13 21:46:02.000000 braingraphstudio-0.1.0/BrainGraphStudio.egg-info/entry_points.txt
--rw-r--r--   0 berk       (502) staff       (20)      228 2024-05-13 21:46:02.000000 braingraphstudio-0.1.0/BrainGraphStudio.egg-info/requires.txt
--rw-r--r--   0 berk       (502) staff       (20)       17 2024-05-13 21:46:02.000000 braingraphstudio-0.1.0/BrainGraphStudio.egg-info/top_level.txt
--rw-r--r--   0 berk       (502) staff       (20)     4742 2024-05-13 21:46:02.991201 braingraphstudio-0.1.0/PKG-INFO
--rw-r--r--   0 berk       (502) staff       (20)     3693 2024-05-13 21:36:18.000000 braingraphstudio-0.1.0/README.md
--rw-r--r--   0 berk       (502) staff       (20)       38 2024-05-13 21:46:02.992391 braingraphstudio-0.1.0/setup.cfg
--rw-r--r--   0 berk       (502) staff       (20)     1753 2024-05-13 21:46:01.000000 braingraphstudio-0.1.0/setup.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2024-05-20 18:21:39.041868 braingraphstudio-0.1.1/
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2024-05-20 18:21:38.992370 braingraphstudio-0.1.1/BrainGraphStudio/
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2024-05-20 18:21:38.996983 braingraphstudio-0.1.1/BrainGraphStudio/BrainGB/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2024-05-13 08:15:27.000000 braingraphstudio-0.1.1/BrainGraphStudio/BrainGB/__init__.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2024-05-20 18:21:38.997540 braingraphstudio-0.1.1/BrainGraphStudio/BrainGB/src/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2024-05-13 08:15:27.000000 braingraphstudio-0.1.1/BrainGraphStudio/BrainGB/src/__init__.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2024-05-20 18:21:39.004069 braingraphstudio-0.1.1/BrainGraphStudio/BrainGB/src/dataset/
+-rw-r--r--   0 berk       (502) staff       (20)       74 2024-05-13 08:15:27.000000 braingraphstudio-0.1.1/BrainGraphStudio/BrainGB/src/dataset/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)      127 2024-05-13 08:15:27.000000 braingraphstudio-0.1.1/BrainGraphStudio/BrainGB/src/dataset/base_transform.py
+-rw-r--r--   0 berk       (502) staff       (20)      613 2024-05-13 08:15:27.000000 braingraphstudio-0.1.1/BrainGraphStudio/BrainGB/src/dataset/brain_data.py
+-rw-r--r--   0 berk       (502) staff       (20)     4406 2024-05-13 08:15:27.000000 braingraphstudio-0.1.1/BrainGraphStudio/BrainGB/src/dataset/brain_dataset.py
+-rw-r--r--   0 berk       (502) staff       (20)      250 2024-05-13 08:15:27.000000 braingraphstudio-0.1.1/BrainGraphStudio/BrainGB/src/dataset/maskable_list.py
+-rw-r--r--   0 berk       (502) staff       (20)     6455 2024-05-13 08:15:27.000000 braingraphstudio-0.1.1/BrainGraphStudio/BrainGB/src/dataset/transforms.py
+-rw-r--r--   0 berk       (502) staff       (20)     2502 2024-05-13 08:15:27.000000 braingraphstudio-0.1.1/BrainGraphStudio/BrainGB/src/dataset/utils.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2024-05-20 18:21:39.012118 braingraphstudio-0.1.1/BrainGraphStudio/BrainGB/src/models/
+-rw-r--r--   0 berk       (502) staff       (20)       92 2024-05-13 08:15:27.000000 braingraphstudio-0.1.1/BrainGraphStudio/BrainGB/src/models/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)      696 2024-05-13 08:15:27.000000 braingraphstudio-0.1.1/BrainGraphStudio/BrainGB/src/models/brainnn.py
+-rw-r--r--   0 berk       (502) staff       (20)     6347 2024-05-13 08:15:27.000000 braingraphstudio-0.1.1/BrainGraphStudio/BrainGB/src/models/gat.py
+-rw-r--r--   0 berk       (502) staff       (20)     5862 2024-05-13 08:15:27.000000 braingraphstudio-0.1.1/BrainGraphStudio/BrainGB/src/models/gcn.py
+-rw-r--r--   0 berk       (502) staff       (20)     2915 2024-05-13 08:15:27.000000 braingraphstudio-0.1.1/BrainGraphStudio/BrainGB/src/models/losses.py
+-rw-r--r--   0 berk       (502) staff       (20)      823 2024-05-13 08:15:27.000000 braingraphstudio-0.1.1/BrainGraphStudio/BrainGB/src/models/mlp.py
+-rw-r--r--   0 berk       (502) staff       (20)     2226 2024-05-13 08:15:27.000000 braingraphstudio-0.1.1/BrainGraphStudio/BrainGB/src/models/pna.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2024-05-20 18:21:39.017592 braingraphstudio-0.1.1/BrainGraphStudio/BrainGB/src/utils/
+-rw-r--r--   0 berk       (502) staff       (20)      109 2024-05-13 08:15:27.000000 braingraphstudio-0.1.1/BrainGraphStudio/BrainGB/src/utils/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)      570 2024-05-13 08:15:27.000000 braingraphstudio-0.1.1/BrainGraphStudio/BrainGB/src/utils/bin_edges.py
+-rw-r--r--   0 berk       (502) staff       (20)      209 2024-05-13 08:15:27.000000 braingraphstudio-0.1.1/BrainGraphStudio/BrainGB/src/utils/get_y.py
+-rw-r--r--   0 berk       (502) staff       (20)     1684 2024-05-13 08:15:27.000000 braingraphstudio-0.1.1/BrainGraphStudio/BrainGB/src/utils/mixup.py
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-12-20 08:58:35.000000 braingraphstudio-0.1.1/BrainGraphStudio/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)     5534 2024-05-13 07:52:56.000000 braingraphstudio-0.1.1/BrainGraphStudio/__main__.py
+-rw-r--r--   0 berk       (502) staff       (20)     3807 2024-05-13 08:05:13.000000 braingraphstudio-0.1.1/BrainGraphStudio/data.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2024-05-20 18:21:39.021914 braingraphstudio-0.1.1/BrainGraphStudio/gui/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-12-20 08:49:33.000000 braingraphstudio-0.1.1/BrainGraphStudio/gui/__init__.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2024-05-20 18:21:39.023127 braingraphstudio-0.1.1/BrainGraphStudio/gui/ims/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2024-04-22 21:09:31.000000 braingraphstudio-0.1.1/BrainGraphStudio/gui/ims/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)    27281 2024-05-13 21:00:52.000000 braingraphstudio-0.1.1/BrainGraphStudio/gui/pages.py
+-rw-r--r--   0 berk       (502) staff       (20)     3272 2024-05-13 02:52:12.000000 braingraphstudio-0.1.1/BrainGraphStudio/gui/utils.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2024-05-20 18:21:39.028430 braingraphstudio-0.1.1/BrainGraphStudio/models/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-09-11 00:39:15.000000 braingraphstudio-0.1.1/BrainGraphStudio/models/__init__.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2024-05-20 18:21:39.036302 braingraphstudio-0.1.1/BrainGraphStudio/models/brainGNN/
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-12-20 08:37:40.000000 braingraphstudio-0.1.1/BrainGraphStudio/models/brainGNN/__init__.py
+-rw-r--r--   0 berk       (502) staff       (20)     3798 2024-04-22 21:55:16.000000 braingraphstudio-0.1.1/BrainGraphStudio/models/brainGNN/braingnn.py
+-rw-r--r--   0 berk       (502) staff       (20)     2865 2024-04-22 21:56:55.000000 braingraphstudio-0.1.1/BrainGraphStudio/models/brainGNN/braingraphconv.py
+-rw-r--r--   0 berk       (502) staff       (20)     6458 2024-04-23 07:06:45.000000 braingraphstudio-0.1.1/BrainGraphStudio/models/brainGNN/brainmsgpassing.py
+-rw-r--r--   0 berk       (502) staff       (20)      617 2023-12-20 08:42:32.000000 braingraphstudio-0.1.1/BrainGraphStudio/models/brainGNN/inits.py
+-rw-r--r--   0 berk       (502) staff       (20)      573 2024-05-06 22:01:44.000000 braingraphstudio-0.1.1/BrainGraphStudio/models/brainGNN/loss.py
+-rw-r--r--   0 berk       (502) staff       (20)     4135 2024-05-13 18:59:50.000000 braingraphstudio-0.1.1/BrainGraphStudio/models/model.py
+-rw-r--r--   0 berk       (502) staff       (20)     2677 2024-01-01 12:59:54.000000 braingraphstudio-0.1.1/BrainGraphStudio/models/params.py
+-rw-r--r--   0 berk       (502) staff       (20)        0 2024-04-15 20:28:59.000000 braingraphstudio-0.1.1/BrainGraphStudio/models/train.py
+-rw-r--r--   0 berk       (502) staff       (20)        0 2023-12-20 09:08:56.000000 braingraphstudio-0.1.1/BrainGraphStudio/models/utils.py
+-rw-r--r--   0 berk       (502) staff       (20)     1712 2024-05-13 02:57:07.000000 braingraphstudio-0.1.1/BrainGraphStudio/nni.py
+-rw-r--r--   0 berk       (502) staff       (20)     3005 2024-05-13 18:28:24.000000 braingraphstudio-0.1.1/BrainGraphStudio/utils.py
+drwxr-xr-x   0 berk       (502) staff       (20)        0 2024-05-20 18:21:39.037630 braingraphstudio-0.1.1/BrainGraphStudio.egg-info/
+-rw-r--r--   0 berk       (502) staff       (20)     4742 2024-05-20 18:21:38.000000 braingraphstudio-0.1.1/BrainGraphStudio.egg-info/PKG-INFO
+-rw-r--r--   0 berk       (502) staff       (20)     1902 2024-05-20 18:21:38.000000 braingraphstudio-0.1.1/BrainGraphStudio.egg-info/SOURCES.txt
+-rw-r--r--   0 berk       (502) staff       (20)        1 2024-05-20 18:21:38.000000 braingraphstudio-0.1.1/BrainGraphStudio.egg-info/dependency_links.txt
+-rw-r--r--   0 berk       (502) staff       (20)       55 2024-05-20 18:21:38.000000 braingraphstudio-0.1.1/BrainGraphStudio.egg-info/entry_points.txt
+-rw-r--r--   0 berk       (502) staff       (20)      228 2024-05-20 18:21:38.000000 braingraphstudio-0.1.1/BrainGraphStudio.egg-info/requires.txt
+-rw-r--r--   0 berk       (502) staff       (20)       17 2024-05-20 18:21:38.000000 braingraphstudio-0.1.1/BrainGraphStudio.egg-info/top_level.txt
+-rw-r--r--   0 berk       (502) staff       (20)     4742 2024-05-20 18:21:39.040892 braingraphstudio-0.1.1/PKG-INFO
+-rw-r--r--   0 berk       (502) staff       (20)     3693 2024-05-13 21:36:18.000000 braingraphstudio-0.1.1/README.md
+-rw-r--r--   0 berk       (502) staff       (20)       38 2024-05-20 18:21:39.042061 braingraphstudio-0.1.1/setup.cfg
+-rw-r--r--   0 berk       (502) staff       (20)     1753 2024-05-20 18:21:29.000000 braingraphstudio-0.1.1/setup.py
```

### Comparing `braingraphstudio-0.1.0/BrainGraphStudio/BrainGB/src/dataset/brain_data.py` & `braingraphstudio-0.1.1/BrainGraphStudio/BrainGB/src/dataset/brain_data.py`

 * *Files identical despite different names*

### Comparing `braingraphstudio-0.1.0/BrainGraphStudio/BrainGB/src/dataset/brain_dataset.py` & `braingraphstudio-0.1.1/BrainGraphStudio/BrainGB/src/dataset/brain_dataset.py`

 * *Files identical despite different names*

### Comparing `braingraphstudio-0.1.0/BrainGraphStudio/BrainGB/src/dataset/transforms.py` & `braingraphstudio-0.1.1/BrainGraphStudio/BrainGB/src/dataset/transforms.py`

 * *Files identical despite different names*

### Comparing `braingraphstudio-0.1.0/BrainGraphStudio/BrainGB/src/dataset/utils.py` & `braingraphstudio-0.1.1/BrainGraphStudio/BrainGB/src/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `braingraphstudio-0.1.0/BrainGraphStudio/BrainGB/src/models/brainnn.py` & `braingraphstudio-0.1.1/BrainGraphStudio/BrainGB/src/models/brainnn.py`

 * *Files identical despite different names*

### Comparing `braingraphstudio-0.1.0/BrainGraphStudio/BrainGB/src/models/gat.py` & `braingraphstudio-0.1.1/BrainGraphStudio/BrainGB/src/models/gat.py`

 * *Files identical despite different names*

### Comparing `braingraphstudio-0.1.0/BrainGraphStudio/BrainGB/src/models/gcn.py` & `braingraphstudio-0.1.1/BrainGraphStudio/BrainGB/src/models/gcn.py`

 * *Files identical despite different names*

### Comparing `braingraphstudio-0.1.0/BrainGraphStudio/BrainGB/src/models/losses.py` & `braingraphstudio-0.1.1/BrainGraphStudio/BrainGB/src/models/losses.py`

 * *Files identical despite different names*

### Comparing `braingraphstudio-0.1.0/BrainGraphStudio/BrainGB/src/models/mlp.py` & `braingraphstudio-0.1.1/BrainGraphStudio/BrainGB/src/models/mlp.py`

 * *Files identical despite different names*

### Comparing `braingraphstudio-0.1.0/BrainGraphStudio/BrainGB/src/models/pna.py` & `braingraphstudio-0.1.1/BrainGraphStudio/BrainGB/src/models/pna.py`

 * *Files identical despite different names*

### Comparing `braingraphstudio-0.1.0/BrainGraphStudio/BrainGB/src/utils/bin_edges.py` & `braingraphstudio-0.1.1/BrainGraphStudio/BrainGB/src/utils/bin_edges.py`

 * *Files identical despite different names*

### Comparing `braingraphstudio-0.1.0/BrainGraphStudio/BrainGB/src/utils/mixup.py` & `braingraphstudio-0.1.1/BrainGraphStudio/BrainGB/src/utils/mixup.py`

 * *Files identical despite different names*

### Comparing `braingraphstudio-0.1.0/BrainGraphStudio/__main__.py` & `braingraphstudio-0.1.1/BrainGraphStudio/__main__.py`

 * *Files identical despite different names*

### Comparing `braingraphstudio-0.1.0/BrainGraphStudio/data.py` & `braingraphstudio-0.1.1/BrainGraphStudio/data.py`

 * *Files identical despite different names*

### Comparing `braingraphstudio-0.1.0/BrainGraphStudio/gui/pages.py` & `braingraphstudio-0.1.1/BrainGraphStudio/gui/pages.py`

 * *Files identical despite different names*

### Comparing `braingraphstudio-0.1.0/BrainGraphStudio/gui/utils.py` & `braingraphstudio-0.1.1/BrainGraphStudio/gui/utils.py`

 * *Files identical despite different names*

### Comparing `braingraphstudio-0.1.0/BrainGraphStudio/models/brainGNN/braingnn.py` & `braingraphstudio-0.1.1/BrainGraphStudio/models/brainGNN/braingnn.py`

 * *Files identical despite different names*

### Comparing `braingraphstudio-0.1.0/BrainGraphStudio/models/brainGNN/braingraphconv.py` & `braingraphstudio-0.1.1/BrainGraphStudio/models/brainGNN/braingraphconv.py`

 * *Files identical despite different names*

### Comparing `braingraphstudio-0.1.0/BrainGraphStudio/models/brainGNN/brainmsgpassing.py` & `braingraphstudio-0.1.1/BrainGraphStudio/models/brainGNN/brainmsgpassing.py`

 * *Files identical despite different names*

### Comparing `braingraphstudio-0.1.0/BrainGraphStudio/models/brainGNN/inits.py` & `braingraphstudio-0.1.1/BrainGraphStudio/models/brainGNN/inits.py`

 * *Files identical despite different names*

### Comparing `braingraphstudio-0.1.0/BrainGraphStudio/models/brainGNN/loss.py` & `braingraphstudio-0.1.1/BrainGraphStudio/models/brainGNN/loss.py`

 * *Files identical despite different names*

### Comparing `braingraphstudio-0.1.0/BrainGraphStudio/models/model.py` & `braingraphstudio-0.1.1/BrainGraphStudio/models/model.py`

 * *Files identical despite different names*

### Comparing `braingraphstudio-0.1.0/BrainGraphStudio/models/params.py` & `braingraphstudio-0.1.1/BrainGraphStudio/models/params.py`

 * *Files identical despite different names*

### Comparing `braingraphstudio-0.1.0/BrainGraphStudio/nni.py` & `braingraphstudio-0.1.1/BrainGraphStudio/nni.py`

 * *Files identical despite different names*

### Comparing `braingraphstudio-0.1.0/BrainGraphStudio/utils.py` & `braingraphstudio-0.1.1/BrainGraphStudio/utils.py`

 * *Files identical despite different names*

### Comparing `braingraphstudio-0.1.0/BrainGraphStudio.egg-info/PKG-INFO` & `braingraphstudio-0.1.1/BrainGraphStudio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BrainGraphStudio
-Version: 0.1.0
+Version: 0.1.1
 Summary: A GUI-based toolkit for building, training, and optimizing graph neural networks for brain graph analysis
 Home-page: https://github.com/berkyalcinkaya/BrainGraphStudio
 Author: Berk Yalcinkaya
 Author-email: berkyalcinkaya55@gmail.com
 License: BSD
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: BSD License
@@ -14,15 +14,15 @@
 Requires-Dist: pandas~=1.2.3
 Requires-Dist: scikit-learn~=1.0.2
 Requires-Dist: networkx~=2.6.2
 Requires-Dist: node2vec~=0.4.4
 Requires-Dist: scipy~=1.7.3
 Requires-Dist: nni~=2.4
 Provides-Extra: cpu
-Requires-Dist: torch==1.8.0; extra == "cpu"
+Requires-Dist: torch==1.8.1; extra == "cpu"
 Requires-Dist: torchvision==0.9.1; extra == "cpu"
 Requires-Dist: torchaudio==0.8.1; extra == "cpu"
 Provides-Extra: gpu
 Requires-Dist: torch==1.8.1+cu101; extra == "gpu"
 Requires-Dist: torchvision==0.9.1+cu101; extra == "gpu"
 Requires-Dist: torchaudio==0.8.1; extra == "gpu"
```

### Comparing `braingraphstudio-0.1.0/BrainGraphStudio.egg-info/SOURCES.txt` & `braingraphstudio-0.1.1/BrainGraphStudio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `braingraphstudio-0.1.0/PKG-INFO` & `braingraphstudio-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BrainGraphStudio
-Version: 0.1.0
+Version: 0.1.1
 Summary: A GUI-based toolkit for building, training, and optimizing graph neural networks for brain graph analysis
 Home-page: https://github.com/berkyalcinkaya/BrainGraphStudio
 Author: Berk Yalcinkaya
 Author-email: berkyalcinkaya55@gmail.com
 License: BSD
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: BSD License
@@ -14,15 +14,15 @@
 Requires-Dist: pandas~=1.2.3
 Requires-Dist: scikit-learn~=1.0.2
 Requires-Dist: networkx~=2.6.2
 Requires-Dist: node2vec~=0.4.4
 Requires-Dist: scipy~=1.7.3
 Requires-Dist: nni~=2.4
 Provides-Extra: cpu
-Requires-Dist: torch==1.8.0; extra == "cpu"
+Requires-Dist: torch==1.8.1; extra == "cpu"
 Requires-Dist: torchvision==0.9.1; extra == "cpu"
 Requires-Dist: torchaudio==0.8.1; extra == "cpu"
 Provides-Extra: gpu
 Requires-Dist: torch==1.8.1+cu101; extra == "gpu"
 Requires-Dist: torchvision==0.9.1+cu101; extra == "gpu"
 Requires-Dist: torchaudio==0.8.1; extra == "gpu"
```

### Comparing `braingraphstudio-0.1.0/README.md` & `braingraphstudio-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `braingraphstudio-0.1.0/setup.py` & `braingraphstudio-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         'node2vec~=0.4.4',
         'scipy~=1.7.3',
         'nni~=2.4'
     ]
 
 extras_require={
         'cpu': [
-            'torch==1.8.0',
+            'torch==1.8.1',
             'torchvision==0.9.1',
             'torchaudio==0.8.1'
         ],
         'gpu': [
             'torch==1.8.1+cu101',
             'torchvision==0.9.1+cu101',
             'torchaudio==0.8.1'
@@ -29,15 +29,15 @@
 packages = ["BrainGraphStudio", "BrainGraphStudio.gui", "BrainGraphStudio.gui.ims",
             "BrainGraphStudio.models", "BrainGraphStudio.models.brainGNN", "BrainGraphStudio.BrainGB",
             "BrainGraphStudio.BrainGB.src", "BrainGraphStudio.BrainGB.src.dataset", "BrainGraphStudio.BrainGB.src.models", 
             "BrainGraphStudio.BrainGB.src.utils"]
 
 setup(
     name = "BrainGraphStudio",
-    version = "0.1.0",
+    version = "0.1.1",
     description = "A GUI-based toolkit for building, training, and optimizing graph neural networks for brain graph analysis",
     author = "Berk Yalcinkaya",
     url = "https://github.com/berkyalcinkaya/BrainGraphStudio",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author_email="berkyalcinkaya55@gmail.com",
     license = "BSD",
```

