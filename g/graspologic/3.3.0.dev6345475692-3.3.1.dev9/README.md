# Comparing `tmp/graspologic-3.3.0.dev6345475692.tar.gz` & `tmp/graspologic-3.3.1.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graspologic-3.3.0.dev6345475692.tar", last modified: Fri Sep 29 00:23:20 2023, max compression
+gzip compressed data, was "graspologic-3.3.1.dev9.tar", max compression
```

## Comparing `graspologic-3.3.0.dev6345475692.tar` & `graspologic-3.3.1.dev9.tar`

### file list

```diff
@@ -1,217 +1,163 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 00:23:20.943869 graspologic-3.3.0.dev6345475692/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      211 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6176 2023-09-29 00:23:20.943869 graspologic-3.3.0.dev6345475692/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 00:23:20.899868 graspologic-3.3.0.dev6345475692/graspologic/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 00:23:20.899868 graspologic-3.3.0.dev6345475692/graspologic/align/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/align/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4615 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/align/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4197 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/align/orthogonal_procrustes.py
--rw-r--r--   0 runner    (1001) docker     (127)    17718 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/align/seedless_procrustes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3733 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/align/sign_flips.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 00:23:20.903868 graspologic-3.3.0.dev6345475692/graspologic/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29918 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/cluster/autogmm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/cluster/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    16896 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/cluster/divisive_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    11062 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/cluster/gclust.py
--rw-r--r--   0 runner    (1001) docker     (127)     4208 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/cluster/kclust.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 00:23:20.903868 graspologic-3.3.0.dev6345475692/graspologic/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6898 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 00:23:20.903868 graspologic-3.3.0.dev6345475692/graspologic/datasets/drosophila/
--rw-r--r--   0 runner    (1001) docker     (127)    87769 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/drosophila/left_adjacency.csv
--rw-r--r--   0 runner    (1001) docker     (127)      418 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/drosophila/left_cell_labels.csv
--rw-r--r--   0 runner    (1001) docker     (127)    91164 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/drosophila/right_adjacency.csv
--rw-r--r--   0 runner    (1001) docker     (127)      426 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/drosophila/right_cell_labels.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 00:23:20.903868 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/
--rw-r--r--   0 runner    (1001) docker     (127)    19847 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/atlas.csv
--rw-r--r--   0 runner    (1001) docker     (127)      297 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/blocks.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 00:23:20.923868 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/
--rw-r--r--   0 runner    (1001) docker     (127)   465335 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54776_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (127)   417268 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54777_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (127)   481030 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54779_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (127)   513067 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54781_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (127)   486685 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54790_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (127)   502512 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54793_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (127)   501644 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54794_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (127)   490182 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54797_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (127)   423952 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54811_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (127)   410522 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54813_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (127)   418663 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54815_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (127)   426113 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54817_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (127)   459110 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54821_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (127)   456778 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54823_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (127)   500977 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54829_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (127)   429240 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54831_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (127)   412281 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54833_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (127)   486497 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54835_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (127)   466098 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54842_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (127)   469626 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54847_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (127)   431457 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54849_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (127)   408031 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54851_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (127)   450727 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54853_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (127)   343162 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54855_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (127)   451278 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54864_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (127)   496115 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54866_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (127)   493788 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54868_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (127)   481678 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54870_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (127)   479782 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54883_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (127)   416610 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54885_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (127)   363031 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54887_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (127)   474339 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54890_ses-1_dti.edgelist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 00:23:20.927868 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/
--rwxr-xr-x   0 runner    (1001) docker     (127)    33536 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54776.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)    33530 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54777.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)    33537 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54779.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)    33535 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54781.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)    33544 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54790.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)    33551 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54793.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)    33549 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54794.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)    33555 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54797.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)    33519 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54811.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)    33525 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54813.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)    33530 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54815.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)    33528 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54817.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)    33501 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54821.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)    33510 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54823.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)    33536 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54829.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)    33538 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54831.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)    33530 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54833.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)    33535 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54835.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)    33505 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54842.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)    33508 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54847.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)    33520 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54849.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)    33520 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54851.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)    33525 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54853.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)    33527 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54855.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)    33551 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54864.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)    33551 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54866.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)    33551 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54868.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)    33552 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54870.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)    33508 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54883.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)    33514 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54885.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)    33509 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54887.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)    33496 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54890.csv
--rw-r--r--   0 runner    (1001) docker     (127)      684 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/participants.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 00:23:20.927868 graspologic-3.3.0.dev6345475692/graspologic/embed/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/embed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6964 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/embed/ase.py
--rw-r--r--   0 runner    (1001) docker     (127)    17726 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/embed/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8276 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/embed/case.py
--rw-r--r--   0 runner    (1001) docker     (127)     7501 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/embed/lse.py
--rw-r--r--   0 runner    (1001) docker     (127)    10531 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/embed/mase.py
--rw-r--r--   0 runner    (1001) docker     (127)     8280 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/embed/mds.py
--rw-r--r--   0 runner    (1001) docker     (127)     6972 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/embed/mug2vec.py
--rw-r--r--   0 runner    (1001) docker     (127)    19443 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/embed/n2v.py
--rw-r--r--   0 runner    (1001) docker     (127)    11477 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/embed/omni.py
--rw-r--r--   0 runner    (1001) docker     (127)    11836 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/embed/svd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 00:23:20.931868 graspologic-3.3.0.dev6345475692/graspologic/inference/
--rw-r--r--   0 runner    (1001) docker     (127)      429 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/inference/binomial.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/inference/density_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    20574 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/inference/group_connection_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    20135 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/inference/latent_distribution_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9843 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/inference/latent_position_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/inference/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 00:23:20.931868 graspologic-3.3.0.dev6345475692/graspologic/layouts/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/layouts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10697 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/layouts/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16074 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/layouts/auto.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/layouts/classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6076 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/layouts/colors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 00:23:20.931868 graspologic-3.3.0.dev6345475692/graspologic/layouts/include/
--rw-r--r--   0 runner    (1001) docker     (127)    28486 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/layouts/include/colors-100.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 00:23:20.931868 graspologic-3.3.0.dev6345475692/graspologic/layouts/nooverlap/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/layouts/nooverlap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7027 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/layouts/nooverlap/_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/layouts/nooverlap/_node.py
--rw-r--r--   0 runner    (1001) docker     (127)    42453 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/layouts/nooverlap/_quad_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/layouts/nooverlap/_quad_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/layouts/nooverlap/nooverlap.py
--rw-r--r--   0 runner    (1001) docker     (127)    10077 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/layouts/render.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 00:23:20.931868 graspologic-3.3.0.dev6345475692/graspologic/match/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/match/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26978 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/match/solver.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/match/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    14081 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/match/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 00:23:20.935869 graspologic-3.3.0.dev6345475692/graspologic/models/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7322 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7136 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/models/edge_swaps.py
--rw-r--r--   0 runner    (1001) docker     (127)     5488 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/models/er.py
--rw-r--r--   0 runner    (1001) docker     (127)     5906 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/models/rdpg.py
--rw-r--r--   0 runner    (1001) docker     (127)    19671 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/models/sbm_estimators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 00:23:20.935869 graspologic-3.3.0.dev6345475692/graspologic/nominate/
--rw-r--r--   0 runner    (1001) docker     (127)    16972 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/nominate/VNviaSGM.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/nominate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10972 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/nominate/spectralVN.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 00:23:20.935869 graspologic-3.3.0.dev6345475692/graspologic/partition/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/partition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25155 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/partition/leiden.py
--rw-r--r--   0 runner    (1001) docker     (127)     5311 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/partition/modularity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 00:23:20.935869 graspologic-3.3.0.dev6345475692/graspologic/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/pipeline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 00:23:20.935869 graspologic-3.3.0.dev6345475692/graspologic/pipeline/embed/
--rw-r--r--   0 runner    (1001) docker     (127)      691 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/pipeline/embed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/pipeline/embed/_elbow.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/pipeline/embed/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     9212 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/pipeline/embed/adjacency_spectral_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/pipeline/embed/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (127)     9918 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/pipeline/embed/laplacian_spectral_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)    12828 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/pipeline/embed/omnibus_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     4044 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/pipeline/graph_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 00:23:20.935869 graspologic-3.3.0.dev6345475692/graspologic/plot/
--rw-r--r--   0 runner    (1001) docker     (127)      528 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    64262 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/plot/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    34806 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/plot/plot_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/preconditions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 00:23:20.935869 graspologic-3.3.0.dev6345475692/graspologic/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      604 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16315 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/preprocessing/graph_cuts.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 00:23:20.935869 graspologic-3.3.0.dev6345475692/graspologic/simulations/
--rw-r--r--   0 runner    (1001) docker     (127)      482 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/simulations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4904 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/simulations/rdpg_corr.py
--rw-r--r--   0 runner    (1001) docker     (127)    38533 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/simulations/simulations.py
--rw-r--r--   0 runner    (1001) docker     (127)    10269 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/simulations/simulations_corr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 00:23:20.935869 graspologic-3.3.0.dev6345475692/graspologic/subgraph/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/subgraph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8504 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/subgraph/sg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 00:23:20.939869 graspologic-3.3.0.dev6345475692/graspologic/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4201 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/utils/ptr.py
--rw-r--r--   0 runner    (1001) docker     (127)    40460 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/graspologic/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 00:23:20.899868 graspologic-3.3.0.dev6345475692/graspologic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6176 2023-09-29 00:23:20.000000 graspologic-3.3.0.dev6345475692/graspologic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7495 2023-09-29 00:23:20.000000 graspologic-3.3.0.dev6345475692/graspologic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-29 00:23:20.000000 graspologic-3.3.0.dev6345475692/graspologic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      538 2023-09-29 00:23:20.000000 graspologic-3.3.0.dev6345475692/graspologic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-09-29 00:23:20.000000 graspologic-3.3.0.dev6345475692/graspologic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      145 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2023-09-29 00:23:20.943869 graspologic-3.3.0.dev6345475692/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      129 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 00:23:20.899868 graspologic-3.3.0.dev6345475692/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 00:23:20.939869 graspologic-3.3.0.dev6345475692/tests/embed/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/tests/embed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6925 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/tests/embed/test_n2v.py
--rw-r--r--   0 runner    (1001) docker     (127)     8998 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/tests/embed/test_omni.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 00:23:20.939869 graspologic-3.3.0.dev6345475692/tests/layouts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/tests/layouts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 00:23:20.939869 graspologic-3.3.0.dev6345475692/tests/layouts/nooverlap/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/tests/layouts/nooverlap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/tests/layouts/nooverlap/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/tests/layouts/nooverlap/test_grid_cell_creation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7998 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/tests/layouts/nooverlap/test_nooverlap.py
--rw-r--r--   0 runner    (1001) docker     (127)     5783 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/tests/layouts/nooverlap/test_overlap_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/tests/layouts/test_auto.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 00:23:20.939869 graspologic-3.3.0.dev6345475692/tests/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/tests/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5774 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/tests/pipeline/test_graph_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 00:23:20.939869 graspologic-3.3.0.dev6345475692/tests/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/tests/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11354 2023-09-29 00:22:09.000000 graspologic-3.3.0.dev6345475692/tests/preprocessing/graph_cuts.py
+-rw-r--r--   0        0        0     1074 2024-05-20 21:38:52.989539 graspologic-3.3.1.dev9/LICENSE.txt
+-rw-r--r--   0        0        0     4124 2024-05-20 21:38:52.989539 graspologic-3.3.1.dev9/README.md
+-rw-r--r--   0        0        0      605 2024-05-20 21:38:53.005539 graspologic-3.3.1.dev9/graspologic/__init__.py
+-rw-r--r--   0        0        0      304 2024-05-20 21:38:53.005539 graspologic-3.3.1.dev9/graspologic/align/__init__.py
+-rw-r--r--   0        0        0     4615 2024-05-20 21:38:53.005539 graspologic-3.3.1.dev9/graspologic/align/base.py
+-rw-r--r--   0        0        0     4197 2024-05-20 21:38:53.005539 graspologic-3.3.1.dev9/graspologic/align/orthogonal_procrustes.py
+-rw-r--r--   0        0        0    17718 2024-05-20 21:38:53.005539 graspologic-3.3.1.dev9/graspologic/align/seedless_procrustes.py
+-rw-r--r--   0        0        0     3733 2024-05-20 21:38:53.005539 graspologic-3.3.1.dev9/graspologic/align/sign_flips.py
+-rw-r--r--   0        0        0      328 2024-05-20 21:38:53.005539 graspologic-3.3.1.dev9/graspologic/cluster/__init__.py
+-rw-r--r--   0        0        0    30149 2024-05-20 21:38:53.009539 graspologic-3.3.1.dev9/graspologic/cluster/autogmm.py
+-rw-r--r--   0        0        0     2576 2024-05-20 21:38:53.009539 graspologic-3.3.1.dev9/graspologic/cluster/base.py
+-rw-r--r--   0        0        0    16926 2024-05-20 21:38:53.009539 graspologic-3.3.1.dev9/graspologic/cluster/divisive_cluster.py
+-rw-r--r--   0        0        0    11062 2024-05-20 21:38:53.009539 graspologic-3.3.1.dev9/graspologic/cluster/gclust.py
+-rw-r--r--   0        0        0     4178 2024-05-20 21:38:53.009539 graspologic-3.3.1.dev9/graspologic/cluster/kclust.py
+-rw-r--r--   0        0        0      238 2024-05-20 21:38:53.009539 graspologic-3.3.1.dev9/graspologic/datasets/__init__.py
+-rw-r--r--   0        0        0     6898 2024-05-20 21:38:53.009539 graspologic-3.3.1.dev9/graspologic/datasets/base.py
+-rw-r--r--   0        0        0    87769 2024-05-20 21:38:53.009539 graspologic-3.3.1.dev9/graspologic/datasets/drosophila/left_adjacency.csv
+-rw-r--r--   0        0        0      418 2024-05-20 21:38:53.009539 graspologic-3.3.1.dev9/graspologic/datasets/drosophila/left_cell_labels.csv
+-rw-r--r--   0        0        0    91164 2024-05-20 21:38:53.009539 graspologic-3.3.1.dev9/graspologic/datasets/drosophila/right_adjacency.csv
+-rw-r--r--   0        0        0      426 2024-05-20 21:38:53.009539 graspologic-3.3.1.dev9/graspologic/datasets/drosophila/right_cell_labels.csv
+-rw-r--r--   0        0        0    19847 2024-05-20 21:38:53.009539 graspologic-3.3.1.dev9/graspologic/datasets/mice/atlas.csv
+-rw-r--r--   0        0        0      297 2024-05-20 21:38:53.009539 graspologic-3.3.1.dev9/graspologic/datasets/mice/blocks.csv
+-rw-r--r--   0        0        0   465335 2024-05-20 21:38:53.009539 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54776_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   417268 2024-05-20 21:38:53.013539 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54777_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   481030 2024-05-20 21:38:53.013539 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54779_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   513067 2024-05-20 21:38:53.017539 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54781_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   486685 2024-05-20 21:38:53.017539 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54790_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   502512 2024-05-20 21:38:53.021539 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54793_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   501644 2024-05-20 21:38:53.021539 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54794_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   490182 2024-05-20 21:38:53.025539 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54797_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   423952 2024-05-20 21:38:53.025539 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54811_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   410522 2024-05-20 21:38:53.029539 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54813_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   418663 2024-05-20 21:38:53.029539 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54815_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   426113 2024-05-20 21:38:53.033539 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54817_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   459110 2024-05-20 21:38:53.033539 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54821_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   456778 2024-05-20 21:38:53.037539 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54823_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   500977 2024-05-20 21:38:53.037539 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54829_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   429240 2024-05-20 21:38:53.037539 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54831_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   412281 2024-05-20 21:38:53.041539 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54833_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   486497 2024-05-20 21:38:53.041539 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54835_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   466098 2024-05-20 21:38:53.045539 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54842_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   469626 2024-05-20 21:38:53.045539 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54847_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   431457 2024-05-20 21:38:53.049539 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54849_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   408031 2024-05-20 21:38:53.049539 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54851_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   450727 2024-05-20 21:38:53.053540 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54853_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   343162 2024-05-20 21:38:53.053540 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54855_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   451278 2024-05-20 21:38:53.053540 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54864_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   496115 2024-05-20 21:38:53.057540 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54866_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   493788 2024-05-20 21:38:53.057540 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54868_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   481678 2024-05-20 21:38:53.061540 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54870_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   479782 2024-05-20 21:38:53.061540 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54883_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   416610 2024-05-20 21:38:53.065540 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54885_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   363031 2024-05-20 21:38:53.065540 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54887_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   474339 2024-05-20 21:38:53.069540 graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54890_ses-1_dti.edgelist
+-rwxr-xr-x   0        0        0    33536 2024-05-20 21:38:53.069540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54776.csv
+-rwxr-xr-x   0        0        0    33530 2024-05-20 21:38:53.069540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54777.csv
+-rwxr-xr-x   0        0        0    33537 2024-05-20 21:38:53.069540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54779.csv
+-rwxr-xr-x   0        0        0    33535 2024-05-20 21:38:53.069540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54781.csv
+-rwxr-xr-x   0        0        0    33544 2024-05-20 21:38:53.069540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54790.csv
+-rwxr-xr-x   0        0        0    33551 2024-05-20 21:38:53.069540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54793.csv
+-rwxr-xr-x   0        0        0    33549 2024-05-20 21:38:53.069540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54794.csv
+-rwxr-xr-x   0        0        0    33555 2024-05-20 21:38:53.069540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54797.csv
+-rwxr-xr-x   0        0        0    33519 2024-05-20 21:38:53.069540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54811.csv
+-rwxr-xr-x   0        0        0    33525 2024-05-20 21:38:53.069540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54813.csv
+-rwxr-xr-x   0        0        0    33530 2024-05-20 21:38:53.069540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54815.csv
+-rwxr-xr-x   0        0        0    33528 2024-05-20 21:38:53.069540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54817.csv
+-rwxr-xr-x   0        0        0    33501 2024-05-20 21:38:53.069540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54821.csv
+-rwxr-xr-x   0        0        0    33510 2024-05-20 21:38:53.069540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54823.csv
+-rwxr-xr-x   0        0        0    33536 2024-05-20 21:38:53.069540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54829.csv
+-rwxr-xr-x   0        0        0    33538 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54831.csv
+-rwxr-xr-x   0        0        0    33530 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54833.csv
+-rwxr-xr-x   0        0        0    33535 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54835.csv
+-rwxr-xr-x   0        0        0    33505 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54842.csv
+-rwxr-xr-x   0        0        0    33508 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54847.csv
+-rwxr-xr-x   0        0        0    33520 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54849.csv
+-rwxr-xr-x   0        0        0    33520 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54851.csv
+-rwxr-xr-x   0        0        0    33525 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54853.csv
+-rwxr-xr-x   0        0        0    33527 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54855.csv
+-rwxr-xr-x   0        0        0    33551 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54864.csv
+-rwxr-xr-x   0        0        0    33551 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54866.csv
+-rwxr-xr-x   0        0        0    33551 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54868.csv
+-rwxr-xr-x   0        0        0    33552 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54870.csv
+-rwxr-xr-x   0        0        0    33508 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54883.csv
+-rwxr-xr-x   0        0        0    33514 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54885.csv
+-rwxr-xr-x   0        0        0    33509 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54887.csv
+-rwxr-xr-x   0        0        0    33496 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54890.csv
+-rw-r--r--   0        0        0      684 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/datasets/mice/participants.csv
+-rw-r--r--   0        0        0      699 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/embed/__init__.py
+-rw-r--r--   0        0        0     6965 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/embed/ase.py
+-rw-r--r--   0        0        0    17726 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/embed/base.py
+-rw-r--r--   0        0        0     8276 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/embed/case.py
+-rw-r--r--   0        0        0     7502 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/embed/lse.py
+-rw-r--r--   0        0        0    10447 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/embed/mase.py
+-rw-r--r--   0        0        0     8317 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/embed/mds.py
+-rw-r--r--   0        0        0     6972 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/embed/mug2vec.py
+-rw-r--r--   0        0        0    19443 2024-05-20 21:38:53.073540 graspologic-3.3.1.dev9/graspologic/embed/n2v.py
+-rw-r--r--   0        0        0    11479 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/embed/omni.py
+-rw-r--r--   0        0        0    11834 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/embed/svd.py
+-rw-r--r--   0        0        0      429 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/inference/__init__.py
+-rw-r--r--   0        0        0     2880 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/inference/binomial.py
+-rw-r--r--   0        0        0     4564 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/inference/density_test.py
+-rw-r--r--   0        0        0    20564 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/inference/group_connection_test.py
+-rw-r--r--   0        0        0    20135 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/inference/latent_distribution_test.py
+-rw-r--r--   0        0        0     9837 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/inference/latent_position_test.py
+-rw-r--r--   0        0        0     2392 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/inference/utils.py
+-rw-r--r--   0        0        0      428 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/layouts/__init__.py
+-rw-r--r--   0        0        0    10697 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/layouts/__main__.py
+-rw-r--r--   0        0        0    16074 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/layouts/auto.py
+-rw-r--r--   0        0        0      345 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/layouts/classes.py
+-rw-r--r--   0        0        0     6154 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/layouts/colors.py
+-rw-r--r--   0        0        0    28486 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/layouts/include/colors-100.json
+-rw-r--r--   0        0        0      174 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/layouts/nooverlap/__init__.py
+-rw-r--r--   0        0        0     7029 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/layouts/nooverlap/_grid.py
+-rw-r--r--   0        0        0      860 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/layouts/nooverlap/_node.py
+-rw-r--r--   0        0        0    42453 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/layouts/nooverlap/_quad_node.py
+-rw-r--r--   0        0        0     2171 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/layouts/nooverlap/_quad_tree.py
+-rw-r--r--   0        0        0      964 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/layouts/nooverlap/nooverlap.py
+-rw-r--r--   0        0        0    10077 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/layouts/render.py
+-rw-r--r--   0        0        0      152 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/match/__init__.py
+-rw-r--r--   0        0        0    26991 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/match/solver.py
+-rw-r--r--   0        0        0      840 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/match/types.py
+-rw-r--r--   0        0        0    14080 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/match/wrappers.py
+-rw-r--r--   0        0        0      459 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/models/__init__.py
+-rw-r--r--   0        0        0     7322 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/models/base.py
+-rw-r--r--   0        0        0     7136 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/models/edge_swaps.py
+-rw-r--r--   0        0        0     5488 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/models/er.py
+-rw-r--r--   0        0        0     5906 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/models/rdpg.py
+-rw-r--r--   0        0        0    19673 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/models/sbm_estimators.py
+-rw-r--r--   0        0        0    16934 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/nominate/VNviaSGM.py
+-rw-r--r--   0        0        0      234 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/nominate/__init__.py
+-rw-r--r--   0        0        0    10972 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/nominate/spectralVN.py
+-rw-r--r--   0        0        0      419 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/partition/__init__.py
+-rw-r--r--   0        0        0    25153 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/partition/leiden.py
+-rw-r--r--   0        0        0     5311 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/partition/modularity.py
+-rw-r--r--   0        0        0     1091 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/pipeline/__init__.py
+-rw-r--r--   0        0        0      744 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/pipeline/embed/__init__.py
+-rw-r--r--   0        0        0     2318 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/pipeline/embed/_elbow.py
+-rw-r--r--   0        0        0       91 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/pipeline/embed/_types.py
+-rw-r--r--   0        0        0     9212 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/pipeline/embed/adjacency_spectral_embedding.py
+-rw-r--r--   0        0        0     4269 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/pipeline/embed/embeddings.py
+-rw-r--r--   0        0        0     9918 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/pipeline/embed/laplacian_spectral_embedding.py
+-rw-r--r--   0        0        0    12796 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/pipeline/embed/omnibus_embedding.py
+-rw-r--r--   0        0        0     4045 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/pipeline/graph_builder.py
+-rw-r--r--   0        0        0      528 2024-05-20 21:38:53.077540 graspologic-3.3.1.dev9/graspologic/plot/__init__.py
+-rw-r--r--   0        0        0    64195 2024-05-20 21:38:53.081540 graspologic-3.3.1.dev9/graspologic/plot/plot.py
+-rw-r--r--   0        0        0    34806 2024-05-20 21:38:53.081540 graspologic-3.3.1.dev9/graspologic/plot/plot_matrix.py
+-rw-r--r--   0        0        0     3456 2024-05-20 21:38:53.081540 graspologic-3.3.1.dev9/graspologic/preconditions.py
+-rw-r--r--   0        0        0      604 2024-05-20 21:38:53.081540 graspologic-3.3.1.dev9/graspologic/preprocessing/__init__.py
+-rw-r--r--   0        0        0    16315 2024-05-20 21:38:53.081540 graspologic-3.3.1.dev9/graspologic/preprocessing/graph_cuts.py
+-rw-r--r--   0        0        0        0 2024-05-20 21:38:53.081540 graspologic-3.3.1.dev9/graspologic/py.typed
+-rw-r--r--   0        0        0      482 2024-05-20 21:38:53.081540 graspologic-3.3.1.dev9/graspologic/simulations/__init__.py
+-rw-r--r--   0        0        0     4904 2024-05-20 21:38:53.081540 graspologic-3.3.1.dev9/graspologic/simulations/rdpg_corr.py
+-rw-r--r--   0        0        0    38533 2024-05-20 21:38:53.081540 graspologic-3.3.1.dev9/graspologic/simulations/simulations.py
+-rw-r--r--   0        0        0    10269 2024-05-20 21:38:53.081540 graspologic-3.3.1.dev9/graspologic/simulations/simulations_corr.py
+-rw-r--r--   0        0        0      153 2024-05-20 21:38:53.081540 graspologic-3.3.1.dev9/graspologic/subgraph/__init__.py
+-rw-r--r--   0        0        0     8470 2024-05-20 21:38:53.081540 graspologic-3.3.1.dev9/graspologic/subgraph/sg.py
+-rw-r--r--   0        0        0     1781 2024-05-20 21:38:53.081540 graspologic-3.3.1.dev9/graspologic/types.py
+-rw-r--r--   0        0        0     1195 2024-05-20 21:38:53.081540 graspologic-3.3.1.dev9/graspologic/utils/__init__.py
+-rw-r--r--   0        0        0     4201 2024-05-20 21:38:53.081540 graspologic-3.3.1.dev9/graspologic/utils/ptr.py
+-rw-r--r--   0        0        0    40441 2024-05-20 21:38:53.081540 graspologic-3.3.1.dev9/graspologic/utils/utils.py
+-rw-r--r--   0        0        0     1765 2024-05-20 21:38:53.081540 graspologic-3.3.1.dev9/graspologic/version.py
+-rw-r--r--   0        0        0     4306 2024-05-20 21:39:33.610047 graspologic-3.3.1.dev9/pyproject.toml
+-rw-r--r--   0        0        0     5662 1970-01-01 00:00:00.000000 graspologic-3.3.1.dev9/PKG-INFO
```

### Comparing `graspologic-3.3.0.dev6345475692/LICENSE.txt` & `graspologic-3.3.1.dev9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/PKG-INFO` & `graspologic-3.3.1.dev9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,67 +1,51 @@
 Metadata-Version: 2.1
 Name: graspologic
-Version: 3.3.0.dev6345475692
-Summary: A set of python modules for graph statistics
+Version: 3.3.1.dev9
+Summary: A set of Python modules for graph statistics
 Home-page: https://github.com/microsoft/graspologic
-Author: Eric Bridgeford, Jaewon Chung, Benjamin Pedigo, Bijan Varjavand
-Author-email: j1c@jhu.edu
+License: MIT
+Author: Eric Bridgeford
 Maintainer: Dax Pryce
 Maintainer-email: daxpryce@microsoft.com
-License: MIT
+Requires-Python: >=3.9,<3.13
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: <3.12,>=3.8
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Requires-Dist: POT (>=0.7.0,<0.8.0)
+Requires-Dist: anytree (>=2.12.1,<3.0.0)
+Requires-Dist: beartype (>=0.10.4,<0.11.0)
+Requires-Dist: gensim (>=4.3.2,<5.0.0)
+Requires-Dist: graspologic-native (>=1.2.1,<2.0.0)
+Requires-Dist: hyppo (>=0.3.2,<0.4.0)
+Requires-Dist: joblib (>=1.4.2,<2.0.0)
+Requires-Dist: matplotlib (>=3.8.4,<4.0.0)
+Requires-Dist: networkx (>=2.8.8,<3.0.0)
+Requires-Dist: numpy (>=1.26.4,<2.0.0)
+Requires-Dist: scikit-learn (>=1.4.2,<2.0.0)
+Requires-Dist: scipy (==1.12.0)
+Requires-Dist: seaborn (>=0.13.2,<0.14.0)
+Requires-Dist: statsmodels (>=0.14.2,<0.15.0)
+Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
+Requires-Dist: umap-learn (>=0.5.6,<0.6.0)
+Project-URL: Repository, https://github.com/microsoft/graspologic
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: anytree>=2.8.0
-Requires-Dist: beartype>=0.10.0
-Requires-Dist: gensim!=4.2.0,>=4.0.0
-Requires-Dist: graspologic-native>=1.1.1
-Requires-Dist: hyppo>=0.3.2
-Requires-Dist: joblib>=0.17.0
-Requires-Dist: matplotlib!=3.3.*,!=3.6.1,>=3.0.0
-Requires-Dist: networkx>=2.1
-Requires-Dist: numpy>=1.8.1
-Requires-Dist: POT>=0.7.0
-Requires-Dist: seaborn>=0.11.0
-Requires-Dist: scikit-learn>=0.22.0
-Requires-Dist: scipy>=1.9.0
-Requires-Dist: statsmodels>=0.13.2
-Requires-Dist: typing-extensions>=4.4.0
-Requires-Dist: umap-learn>=0.4.6
-Provides-Extra: dev
-Requires-Dist: black; extra == "dev"
-Requires-Dist: ipykernel>=5.1.0; extra == "dev"
-Requires-Dist: ipython!=8.7.0,>=7.4.0; extra == "dev"
-Requires-Dist: isort>=5.9.3; extra == "dev"
-Requires-Dist: mypy>=0.910; extra == "dev"
-Requires-Dist: nbsphinx>=0.8.7; extra == "dev"
-Requires-Dist: numpydoc>=1.1.0; extra == "dev"
-Requires-Dist: pandoc>=1.1.0; extra == "dev"
-Requires-Dist: pytest>=6.2.5; extra == "dev"
-Requires-Dist: pytest-cov>=3.0.0; extra == "dev"
-Requires-Dist: sphinx>=4.2.0; extra == "dev"
-Requires-Dist: sphinxcontrib-rawfiles>=0.1.1; extra == "dev"
-Requires-Dist: sphinx-rtd-theme>=1.0.0; extra == "dev"
-Requires-Dist: testfixtures>=6.18.3; extra == "dev"
 
 <!-- omit in toc -->
 # graspologic
 [![Paper shield](https://img.shields.io/badge/JMLR-Paper-red)](http://www.jmlr.org/papers/volume20/19-490/19-490.pdf)
 [![PyPI version](https://img.shields.io/pypi/v/graspologic.svg)](https://pypi.org/project/graspologic/)
 [![Downloads shield](https://pepy.tech/badge/graspologic)](https://pepy.tech/project/graspologic)
-![graspologic CI](https://github.com/microsoft/graspologic/workflows/graspologic%20CI/badge.svg)
+[![graspologic Build](https://github.com/microsoft/graspologic/actions/workflows/build.yml/badge.svg)](https://github.com/microsoft/graspologic/actions/workflows/build.yml)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 ## `graspologic` is a package for graph statistical algorithms.
 <!-- no toc -->
 - [Overview](#overview)
 - [Documentation](#documentation)
 - [System Requirements](#system-requirements)
@@ -90,17 +74,18 @@
 ### OS Requirements
 `graspologic` is tested on the following OSes:
 - Linux x64
 - macOS x64
 - Windows 10 x64
 
 And across the following **x86_64** versions of Python:
-- 3.8
 - 3.9
 - 3.10
+- 3.11
+- 3.12
 
 If you try to use `graspologic` for a different platform than the ones listed and notice any unexpected behavior,
 please feel free to [raise an issue](https://github.com/microsoft/graspologic/issues/new).  It's better for ourselves and our users
 if we have concrete examples of things not working!
 
 # Installation Guide
 <!-- omit in toc -->
@@ -131,7 +116,8 @@
 # Issues
 We appreciate detailed bug reports and feature requests (though we appreciate pull requests even more!). Please visit our [issues](https://github.com/microsoft/graspologic/issues) page if you have questions or ideas.
 
 # Citing `graspologic`
 If you find `graspologic` useful in your work, please cite the package via the [GraSPy paper](http://www.jmlr.org/papers/volume20/19-490/19-490.pdf)
 
 > Chung, J., Pedigo, B. D., Bridgeford, E. W., Varjavand, B. K., Helm, H. S., & Vogelstein, J. T. (2019). GraSPy: Graph Statistics in Python. Journal of Machine Learning Research, 20(158), 1-7.
+
```

### Comparing `graspologic-3.3.0.dev6345475692/README.md` & `graspologic-3.3.1.dev9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!-- omit in toc -->
 # graspologic
 [![Paper shield](https://img.shields.io/badge/JMLR-Paper-red)](http://www.jmlr.org/papers/volume20/19-490/19-490.pdf)
 [![PyPI version](https://img.shields.io/pypi/v/graspologic.svg)](https://pypi.org/project/graspologic/)
 [![Downloads shield](https://pepy.tech/badge/graspologic)](https://pepy.tech/project/graspologic)
-![graspologic CI](https://github.com/microsoft/graspologic/workflows/graspologic%20CI/badge.svg)
+[![graspologic Build](https://github.com/microsoft/graspologic/actions/workflows/build.yml/badge.svg)](https://github.com/microsoft/graspologic/actions/workflows/build.yml)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 ## `graspologic` is a package for graph statistical algorithms.
 <!-- no toc -->
 - [Overview](#overview)
 - [Documentation](#documentation)
 - [System Requirements](#system-requirements)
@@ -36,17 +36,18 @@
 ### OS Requirements
 `graspologic` is tested on the following OSes:
 - Linux x64
 - macOS x64
 - Windows 10 x64
 
 And across the following **x86_64** versions of Python:
-- 3.8
 - 3.9
 - 3.10
+- 3.11
+- 3.12
 
 If you try to use `graspologic` for a different platform than the ones listed and notice any unexpected behavior,
 please feel free to [raise an issue](https://github.com/microsoft/graspologic/issues/new).  It's better for ourselves and our users
 if we have concrete examples of things not working!
 
 # Installation Guide
 <!-- omit in toc -->
```

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/__init__.py` & `graspologic-3.3.1.dev9/graspologic/__init__.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/align/base.py` & `graspologic-3.3.1.dev9/graspologic/align/base.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/align/orthogonal_procrustes.py` & `graspologic-3.3.1.dev9/graspologic/align/orthogonal_procrustes.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/align/seedless_procrustes.py` & `graspologic-3.3.1.dev9/graspologic/align/seedless_procrustes.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/align/sign_flips.py` & `graspologic-3.3.1.dev9/graspologic/align/sign_flips.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/cluster/autogmm.py` & `graspologic-3.3.1.dev9/graspologic/cluster/autogmm.py`

 * *Files 1% similar despite different names*

```diff
@@ -565,16 +565,20 @@
             subset_idxs = np.random.choice(np.arange(0, n), self.max_agglom_size)
             X_subset = X[subset_idxs, :]
 
         ag_labels: List[np.ndarray] = []
         if self.label_init is None:
             for p_ag in param_grid_ag:
                 if p_ag["affinity"] != "none":
+                    p_ag_without_affinity = p_ag.copy()
+                    affinity = p_ag_without_affinity.pop("affinity", None)
                     agg = AgglomerativeClustering(
-                        n_clusters=self.min_components, **p_ag
+                        n_clusters=self.min_components,
+                        metric=affinity,
+                        **p_ag_without_affinity,
                     )
                     agg.fit(X_subset)
                     hierarchical_labels = _hierarchical_labels(
                         agg.children_, lower_ncomponents, upper_ncomponents
                     )
                     ag_labels.append(hierarchical_labels)
 
@@ -754,17 +758,18 @@
     merge_start = n_samples - max_components - 1
     merge_end = n_samples - min_components - 1
 
     for n in range(merge_end + 1):
         inds = np.where(np.isin(hierarchical_labels[:, n], children[n, :]))[0]
         hierarchical_labels[inds, -1] = n_samples + n
         if n < merge_end:
-            hierarchical_labels = np.hstack(
-                (hierarchical_labels, hierarchical_labels[:, -1].reshape((-1, 1)))
-            )
+            hierarchical_labels = np.hstack((
+                hierarchical_labels,
+                hierarchical_labels[:, -1].reshape((-1, 1)),
+            ))
 
     hierarchical_labels = hierarchical_labels[:, merge_start:]
     for i in range(hierarchical_labels.shape[1]):
         _, hierarchical_labels[:, i] = np.unique(
             hierarchical_labels[:, i], return_inverse=True
         )
```

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/cluster/base.py` & `graspologic-3.3.1.dev9/graspologic/cluster/base.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/cluster/divisive_cluster.py` & `graspologic-3.3.1.dev9/graspologic/cluster/divisive_cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,15 +210,15 @@
         else:
             min_components = 1
 
         if self.cluster_method == "gmm":
             cluster = AutoGMMCluster(
                 min_components=min_components,
                 max_components=self.max_components,
-                **self.cluster_kws
+                **self.cluster_kws,
             )
             cluster.fit(X)
             model = cluster.model_
             criter = cluster.criter_
             k = cluster.n_components_
             pred = cluster.predict(X)
 
@@ -271,17 +271,18 @@
                 if (
                     len(new_X) > self.max_components
                     and len(new_X) >= self.min_split
                     and self.depth + 1 < self.max_level
                 ):
                     child_labels = dc._fit(new_X)
                     while labels.shape[1] <= child_labels.shape[1]:
-                        labels = np.column_stack(
-                            (labels, np.zeros((len(X), 1), dtype=int))
-                        )
+                        labels = np.column_stack((
+                            labels,
+                            np.zeros((len(X), 1), dtype=int),
+                        ))
                     labels[inds, 1 : child_labels.shape[1] + 1] = child_labels
                 else:
                     # make a "GaussianMixture" model for clusters
                     # that were not fitted
                     if self.cluster_method == "gmm":
                         cluster_idx = len(dc.parent.children) - 1
                         parent_model = dc.parent.model_
```

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/cluster/gclust.py` & `graspologic-3.3.1.dev9/graspologic/cluster/gclust.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/cluster/kclust.py` & `graspologic-3.3.1.dev9/graspologic/cluster/kclust.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,17 +84,15 @@
         Returns
         -------
         self
         """
         # Deal with number of clusters
         if self.max_clusters > X.shape[0]:
             msg = "n_components must be >= n_samples, but got \
-                n_components = {}, n_samples = {}".format(
-                self.max_clusters, X.shape[0]
-            )
+                n_components = {}, n_samples = {}".format(self.max_clusters, X.shape[0])
             raise ValueError(msg)
         else:
             max_clusters = self.max_clusters
 
         # Get parameters
         random_state = self.random_state
```

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/base.py` & `graspologic-3.3.1.dev9/graspologic/datasets/base.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/drosophila/left_adjacency.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/drosophila/left_adjacency.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/drosophila/right_adjacency.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/drosophila/right_adjacency.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/atlas.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/atlas.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54776_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54776_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54777_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54777_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54779_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54779_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54781_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54781_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54790_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54790_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54793_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54793_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54794_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54794_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54797_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54797_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54811_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54811_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54813_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54813_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54815_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54815_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54817_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54817_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54821_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54821_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54823_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54823_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54829_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54829_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54831_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54831_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54833_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54833_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54835_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54835_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54842_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54842_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54847_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54847_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54849_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54849_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54851_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54851_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54853_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54853_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54855_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54855_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54864_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54864_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54866_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54866_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54868_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54868_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54870_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54870_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54883_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54883_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54885_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54885_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54887_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54887_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/edgelists/sub-54890_ses-1_dti.edgelist` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/edgelists/sub-54890_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54776.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54776.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54777.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54777.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54779.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54779.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54781.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54781.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54790.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54790.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54793.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54793.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54794.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54794.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54797.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54797.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54811.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54811.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54813.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54813.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54815.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54815.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54817.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54817.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54821.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54821.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54823.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54823.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54829.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54829.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54831.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54831.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54833.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54833.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54835.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54835.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54842.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54842.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54847.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54847.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54849.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54849.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54851.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54851.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54853.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54853.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54855.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54855.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54864.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54864.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54866.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54866.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54868.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54868.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54870.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54870.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54883.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54883.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54885.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54885.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54887.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54887.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/features/54890.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/features/54890.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/datasets/mice/participants.csv` & `graspologic-3.3.1.dev9/graspologic/datasets/mice/participants.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/embed/__init__.py` & `graspologic-3.3.1.dev9/graspologic/embed/__init__.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/embed/ase.py` & `graspologic-3.3.1.dev9/graspologic/embed/ase.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
         self.is_fitted_ = False
 
     def fit(
         self,
         graph: GraphRepresentation,
         y: Optional[Any] = None,
         *args: Any,
-        **kwargs: Any
+        **kwargs: Any,
     ) -> "AdjacencySpectralEmbed":
         """
         Fit ASE model to input graph
 
         Parameters
         ----------
         graph : array-like, scipy.sparse.csr_array, or networkx.Graph
```

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/embed/base.py` & `graspologic-3.3.1.dev9/graspologic/embed/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
 
     @abstractmethod
     def fit(
         self,
         graph: GraphRepresentation,
         y: Optional[Any] = None,
         *args: Any,
-        **kwargs: Any
+        **kwargs: Any,
     ) -> "BaseSpectralEmbed":
         """
         A method for embedding.
         Parameters
         ----------
         graph: np.ndarray or networkx.Graph
         y : Ignored
@@ -217,15 +217,15 @@
                 return self.latent_left_, self.latent_right_
 
     def fit_transform(
         self,
         graph: GraphRepresentation,
         y: Optional[Any] = None,
         *args: Any,
-        **kwargs: Any
+        **kwargs: Any,
     ) -> Union[np.ndarray, Tuple[np.ndarray, np.ndarray]]:
         """
         Fit the model with graphs and apply the transformation.
 
         n_dimension is either automatically determined or based on user input.
 
         Parameters
@@ -308,16 +308,16 @@
         if isinstance(X, nx.classes.graph.Graph):
             X = import_graph(X)
         directed = self.latent_right_ is not None
 
         # correct types?
         if directed and not isinstance(X, tuple):
             if X.shape[0] == X.shape[1]:  # in case original matrix was passed
-                msg = """A square matrix A was passed to ``transform`` in the directed case. 
-                If this was the original in-sample matrix, either use ``fit_transform`` 
+                msg = """A square matrix A was passed to ``transform`` in the directed case.
+                If this was the original in-sample matrix, either use ``fit_transform``
                 or pass a tuple (A.T, A). If this was an out-of-sample matrix, directed
                 graphs require a tuple (X_out, X_in)."""
                 raise TypeError(msg)
             else:
                 msg = "Directed graphs require a tuple (X_out, X_in) for out-of-sample transforms."
                 raise TypeError(msg)
         if not directed and not isinstance(X, np.ndarray):
```

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/embed/case.py` & `graspologic-3.3.1.dev9/graspologic/embed/case.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/embed/lse.py` & `graspologic-3.3.1.dev9/graspologic/embed/lse.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
         self.regularizer = regularizer
 
     def fit(
         self,
         graph: GraphRepresentation,
         y: Optional[Any] = None,
         *args: Any,
-        **kwargs: Any
+        **kwargs: Any,
     ) -> "LaplacianSpectralEmbed":
         """
         Fit LSE model to input graph
 
         By default, uses the Laplacian normalization of the form:
 
         .. math:: L = D^{-1/2} A D^{-1/2}
```

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/embed/mase.py` & `graspologic-3.3.1.dev9/graspologic/embed/mase.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,26 +168,22 @@
             best_dimension = self.n_components
 
         if not self.scaled:
             Us = np.hstack([U[:, :best_dimension] for U in Us])
             Vs = np.hstack([V.T[:, :best_dimension] for V in Vs])
         else:
             # Equivalent to ASE
-            Us = np.hstack(
-                [
-                    U[:, :best_dimension] @ np.diag(np.sqrt(D[:best_dimension]))
-                    for U, D in zip(Us, Ds)
-                ]
-            )
-            Vs = np.hstack(
-                [
-                    V.T[:, :best_dimension] @ np.diag(np.sqrt(D[:best_dimension]))
-                    for V, D in zip(Vs, Ds)
-                ]
-            )
+            Us = np.hstack([
+                U[:, :best_dimension] @ np.diag(np.sqrt(D[:best_dimension]))
+                for U, D in zip(Us, Ds)
+            ])
+            Vs = np.hstack([
+                V.T[:, :best_dimension] @ np.diag(np.sqrt(D[:best_dimension]))
+                for V, D in zip(Vs, Ds)
+            ])
 
         # Second SVD for vertices
         # The notation is slightly different than the paper
         Uhat, sing_vals_left, _ = select_svd(
             Us,
             n_components=self.n_components,
             n_elbows=self.n_elbows,
```

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/embed/mds.py` & `graspologic-3.3.1.dev9/graspologic/embed/mds.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # Copyright (c) Microsoft Corporation and contributors.
 # Licensed under the MIT License.
 
-from typing import Any, Optional, Union
+from typing import TYPE_CHECKING, Any, Optional, Union
 
 import numpy as np
 from sklearn.base import BaseEstimator
 from sklearn.utils import check_array
 from typing_extensions import Literal
 
-from graspologic.types import Tuple
-
 from ..utils import is_symmetric
 from .svd import SvdAlgorithmType, select_svd
 
+if TYPE_CHECKING:
+    from graspologic.types import Tuple
+
 
 def _get_centering_matrix(n: int) -> np.ndarray:
     """
     Compute the centering array
 
     Parameters
     ----------
```

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/embed/mug2vec.py` & `graspologic-3.3.1.dev9/graspologic/embed/mug2vec.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/embed/n2v.py` & `graspologic-3.3.1.dev9/graspologic/embed/n2v.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/embed/omni.py` & `graspologic-3.3.1.dev9/graspologic/embed/omni.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         # row
         rows.append(hstack(current_row))
 
     return csr_array(vstack(rows, format="csr"))
 
 
 def _get_laplacian_matrices(
-    graphs: Union[np.ndarray, List[GraphRepresentation]]
+    graphs: Union[np.ndarray, List[GraphRepresentation]],
 ) -> Union[np.ndarray, List[np.ndarray]]:
     """
     Helper function to convert graph adjacency matrices to graph Laplacian
 
     Parameters
     ----------
     graphs : list
@@ -78,15 +78,15 @@
         # Copying is necessary to not overwrite input array
         out = np.array([to_laplacian(graphs[i]) for i in range(len(graphs))])
 
     return out
 
 
 def _get_omni_matrix(
-    graphs: Union[AdjacencyMatrix, List[AdjacencyMatrix]]
+    graphs: Union[AdjacencyMatrix, List[AdjacencyMatrix]],
 ) -> np.ndarray:
     """
     Helper function for creating the omnibus matrix.
 
     Parameters
     ----------
     graphs : list
```

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/embed/svd.py` & `graspologic-3.3.1.dev9/graspologic/embed/svd.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         if s2.size != 0:
             mu2 = np.mean(s2)
         else:
             # Prevent numpy warning for taking mean of empty array
             mu2 = -np.inf
 
         # compute pooled variance
-        variance = ((np.sum((s1 - mu1) ** 2) + np.sum((s2 - mu2) ** 2))) / (
+        variance = (np.sum((s1 - mu1) ** 2) + np.sum((s2 - mu2) ** 2)) / (
             n_elements - 1 - (idx < n_elements)
         )
         std = np.sqrt(variance)
 
         # compute log likelihoods
         likelihoods[idx - 1] = np.sum(norm.logpdf(s1, loc=mu1, scale=std)) + np.sum(
             norm.logpdf(s2, loc=mu2, scale=std)
```

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/inference/binomial.py` & `graspologic-3.3.1.dev9/graspologic/inference/binomial.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,10 +75,10 @@
             n2,
             method="score",
             compare="ratio",
             alternative="two-sided",
             value=null_ratio,
         )
     else:
-        raise ValueError()
+        raise ValueError
 
     return BinomialResult(stat, pvalue)
```

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/inference/density_test.py` & `graspologic-3.3.1.dev9/graspologic/inference/density_test.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/inference/group_connection_test.py` & `graspologic-3.3.1.dev9/graspologic/inference/group_connection_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -374,26 +374,26 @@
             "Test will be run on the loopless version of these adjacency matrices."
         )
         warnings.warn(msg)
 
     B1, n_observed1, n_possible1, group_counts1 = fit_sbm(A1, labels1)
     B2, n_observed2, n_possible2, group_counts2 = fit_sbm(A2, labels2)
     if not n_observed1.index.equals(n_observed2.index):
-        raise ValueError()
+        raise ValueError
     elif not n_observed1.columns.equals(n_observed2.columns):
-        raise ValueError()
+        raise ValueError
     elif not n_possible1.index.equals(n_possible2.index):
-        raise ValueError()
+        raise ValueError
     elif not n_observed1.columns.equals(n_observed2.columns):
-        raise ValueError()
+        raise ValueError
 
     index = n_observed1.index.copy()
 
     if n_observed1.shape[0] != n_observed2.shape[0]:
-        raise ValueError()
+        raise ValueError
 
     K = n_observed1.shape[0]
 
     uncorrected_pvalues_temp = np.empty(
         (K, K), dtype=float
     )  # had to make a new variable to keep mypy happy
     uncorrected_pvalues = _make_adjacency_dataframe(uncorrected_pvalues_temp, index)
```

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/inference/latent_distribution_test.py` & `graspologic-3.3.1.dev9/graspologic/inference/latent_distribution_test.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/inference/latent_position_test.py` & `graspologic-3.3.1.dev9/graspologic/inference/latent_position_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,17 +120,17 @@
        "A Semiparametric Two-Sample Hypothesis Testing Problem for Random Graphs"
        Journal of Computational and Graphical Statistics, Vol. 26(2), 2017
     """
 
     if type(embedding) is not str:
         raise TypeError("embedding must be str")
     if type(n_bootstraps) is not int:
-        raise TypeError()
+        raise TypeError
     if type(test_case) is not str:
-        raise TypeError()
+        raise TypeError
     if n_bootstraps < 1:
         raise ValueError(
             "{} is invalid number of bootstraps, must be greater than 1".format(
                 n_bootstraps
             )
         )
     if embedding not in ["ase", "omnibus"]:
@@ -144,15 +144,15 @@
     if not isinstance(workers, int):
         msg = "workers must be an int, not {}".format(type(workers))
         raise TypeError(msg)
 
     A1 = import_graph(A1)
     A2 = import_graph(A2)
     if not is_symmetric(A1) or not is_symmetric(A2):
-        raise NotImplementedError()  # TODO asymmetric case
+        raise NotImplementedError  # TODO asymmetric case
     if A1.shape != A2.shape:
         raise ValueError("Input matrices do not have matching dimensions")
     num_components: int
     if n_components is None:
         # get the last elbow from ZG for each and take the maximum
         num_dims1 = select_dimension(A1)[0][-1]
         num_dims2 = select_dimension(A2)[0][-1]
```

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/inference/utils.py` & `graspologic-3.3.1.dev9/graspologic/inference/utils.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/layouts/__main__.py` & `graspologic-3.3.1.dev9/graspologic/layouts/__main__.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/layouts/auto.py` & `graspologic-3.3.1.dev9/graspologic/layouts/auto.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/layouts/colors.py` & `graspologic-3.3.1.dev9/graspologic/layouts/colors.py`

 * *Files 7% similar despite different names*

```diff
@@ -152,18 +152,22 @@
         provided for the node as it relates to the total range of all values.
 
     """
     color_scheme = _get_colors(light_background, theme_path)
     color_list = color_scheme["sequential"]
     num_colors = len(color_list)
 
-    keys, values = zip(*node_and_value.items())
+    keys = []
+    values = []
+    for k, v in node_and_value.items():
+        keys.append(k)
+        values.append(v)
 
     if use_log_scale:
-        values = map(math.log, values)
+        values = [math.log(v) for v in values]
 
     np_values = np.array(values).reshape(1, -1)
     new_values = minmax_scale(np_values, feature_range=(0, num_colors - 1), axis=1)
     node_colors = {}
     for key_index, node_id in enumerate(keys):
         index = int(new_values[0, key_index])
```

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/layouts/include/colors-100.json` & `graspologic-3.3.1.dev9/graspologic/layouts/include/colors-100.json`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/layouts/nooverlap/_grid.py` & `graspologic-3.3.1.dev9/graspologic/layouts/nooverlap/_grid.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,15 @@
             y += cell_size
         # for c in sorted(self.grid):
         # 	print (c)
         return rows
 
     def print_stats(self) -> None:
         print(
-            f"cell size: {self.cell_size}, area: {self.cell_size*self.cell_size}, "
+            f"cell size: {self.cell_size}, area: {self.cell_size * self.cell_size}, "
             f"rows: {self._get_y_cells()}, cols: {self._get_x_cells()}"
         )
 
     def _get_area(self, node_list: List[_Node]) -> float:
         area = 0.0
         for n in node_list:
             area += n.size * n.size * 4
```

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/layouts/nooverlap/_node.py` & `graspologic-3.3.1.dev9/graspologic/layouts/nooverlap/_node.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/layouts/nooverlap/_quad_node.py` & `graspologic-3.3.1.dev9/graspologic/layouts/nooverlap/_quad_node.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/layouts/nooverlap/_quad_tree.py` & `graspologic-3.3.1.dev9/graspologic/layouts/nooverlap/_quad_tree.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/layouts/nooverlap/nooverlap.py` & `graspologic-3.3.1.dev9/graspologic/layouts/nooverlap/nooverlap.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     local_nodes = [
         _Node(node.node_id, node.x, node.y, node.size, node.community)
         for node in node_positions
     ]
     qt = _QuadTree(local_nodes, 50)
     qt.layout_dense_first(first_color=None)
     stop = time.time()
-    logger.info(f"removed overlap in {stop-start} seconds")
+    logger.info(f"removed overlap in {stop - start} seconds")
 
     new_positions = [
         NodePosition(
             node_id=node.node_id,
             x=node.x,
             y=node.y,
             size=node.size,
```

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/layouts/render.py` & `graspologic-3.3.1.dev9/graspologic/layouts/render.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/match/solver.py` & `graspologic-3.3.1.dev9/graspologic/match/solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -426,17 +426,18 @@
         # project back onto the feasible region (permutations)
         if P.shape != (0, 0):
             permutation = self.linear_sum_assignment(P, rng, maximize=True)
         else:  # the case where input was all seeded
             permutation = np.array([], dtype=int)
 
         # deal with seed-nonseed sorting from the initialization
-        permutation = np.concatenate(
-            (np.arange(self.n_seeds), permutation + self.n_seeds)
-        )
+        permutation = np.concatenate((
+            np.arange(self.n_seeds),
+            permutation + self.n_seeds,
+        ))
         final_permutation = np.empty(self.n, dtype=int)
         final_permutation[self.perm_A] = self.perm_B[permutation]
 
         # deal with un-padding
         matching = np.column_stack((np.arange(self.n), final_permutation))
         if self.padded:
             if self._padded_B:
```

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/match/types.py` & `graspologic-3.3.1.dev9/graspologic/match/types.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/match/wrappers.py` & `graspologic-3.3.1.dev9/graspologic/match/wrappers.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     """
     Sorted indices in ``A`` which were matched.
     """
 
     indices_B: np.ndarray
     """
     Indices in ``B`` which were matched. Element ``indices_B[i]`` was matched
-    to element ``indices_A[i]``. ``indices_B`` can also be thought of as a 
+    to element ``indices_A[i]``. ``indices_B`` can also be thought of as a
     permutation of the nodes of ``B`` with respect to ``A``.
     """
 
     score: float
     """
     Objective function value at the end of optimization.
     """
```

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/models/base.py` & `graspologic-3.3.1.dev9/graspologic/models/base.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/models/edge_swaps.py` & `graspologic-3.3.1.dev9/graspologic/models/edge_swaps.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/models/er.py` & `graspologic-3.3.1.dev9/graspologic/models/er.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/models/rdpg.py` & `graspologic-3.3.1.dev9/graspologic/models/rdpg.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/models/sbm_estimators.py` & `graspologic-3.3.1.dev9/graspologic/models/sbm_estimators.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
             n_components=self.n_components, **self.embed_kws
         ).fit_transform(embed_graph)
         if isinstance(latent, tuple):
             latent = np.concatenate(latent, axis=1)
         gc = GaussianCluster(
             min_components=self.min_comm,
             max_components=self.max_comm,
-            **self.cluster_kws
+            **self.cluster_kws,
         )
         vertex_assignments = gc.fit_predict(latent)  # type: ignore
         self.vertex_assignments_ = vertex_assignments
 
     def fit(
         self, graph: GraphRepresentation, y: Optional[Any] = None
     ) -> "SBMEstimator":
@@ -370,15 +370,15 @@
         lse = LaplacianSpectralEmbed(
             form="R-DAD", n_components=self.n_components, **self.embed_kws
         )
         latent = lse.fit_transform(graph)
         gc = GaussianCluster(
             min_components=self.min_comm,
             max_components=self.max_comm,
-            **self.cluster_kws
+            **self.cluster_kws,
         )
         self.vertex_assignments_ = gc.fit_predict(latent)  # type: ignore
 
     def fit(
         self, graph: GraphRepresentation, y: Optional[Any] = None
     ) -> "DCSBMEstimator":
         """
```

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/nominate/VNviaSGM.py` & `graspologic-3.3.1.dev9/graspologic/nominate/VNviaSGM.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,17 +255,15 @@
         )
 
         close_seeds = np.intersect1d(subgraph_A_perm, seeds_reord)
 
         if len(close_seeds) <= 0:
             warnings.warn(
                 'Voi {} was not a member of the induced subgraph A[{}], \
-                Try increasing "order_voi_subgraph"'.format(
-                    voi, seedsA
-                )
+                Try increasing "order_voi_subgraph"'.format(voi, seedsA)
             )
             self.n_seeds_ = None
             self.nomination_list_ = None
             return self
 
         # Generate the two induced subgraphs that will be used by the matching
         # algorithm using the seeds that we identified in the previous step.
```

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/nominate/spectralVN.py` & `graspologic-3.3.1.dev9/graspologic/nominate/spectralVN.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/partition/leiden.py` & `graspologic-3.3.1.dev9/graspologic/partition/leiden.py`

 * *Files identical despite different names*

```diff
@@ -348,16 +348,16 @@
     """Node id"""
     cluster: int
     """Leiden cluster id"""
     parent_cluster: Optional[int]
     """Only used when level != 0, but will indicate the previous cluster id that this node was in"""
     level: int
     """
-    Each time a community has a higher population than we would like, we create a subnetwork 
-    of that community and process it again to break it into smaller chunks. Each time we 
+    Each time a community has a higher population than we would like, we create a subnetwork
+    of that community and process it again to break it into smaller chunks. Each time we
     detect this, the level increases by 1
     """
     is_final_cluster: bool
     """
     Whether this is the terminal cluster in the hierarchical leiden process or not
     """
```

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/partition/modularity.py` & `graspologic-3.3.1.dev9/graspologic/partition/modularity.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/pipeline/__init__.py` & `graspologic-3.3.1.dev9/graspologic/pipeline/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,12 +11,13 @@
 
 ``pipeline`` is intended to smooth the transition between a common developer and
 a graph machine learning subject matter expert. We make a presumption that most
 programmers are software developers first, and dabbling in ML second, and our intention
 is to bridge this gap.
 
 """
+
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT license.
 
 from . import embed
 from .graph_builder import GraphBuilder
```

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/pipeline/embed/__init__.py` & `graspologic-3.3.1.dev9/graspologic/pipeline/embed/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT license.
-
+# ruff: noqa: E402 SVD_SOLVER_TYPES needs to be first
 """
 The embed module of ``graspologic.pipeline.embed`` is intended to provide faster
 application development support. The functions provided in it reflect common call
 patterns used when developing data processing pipelines and future consumption
 by nearest neighbor services and visualization routines.
 """
 
 __SVD_SOLVER_TYPES = ["randomized", "full", "truncated"]
-
 from .adjacency_spectral_embedding import adjacency_spectral_embedding
 from .embeddings import Embeddings, EmbeddingsView
 from .laplacian_spectral_embedding import laplacian_spectral_embedding
 from .omnibus_embedding import omnibus_embedding_pairwise
+
```

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/pipeline/embed/_elbow.py` & `graspologic-3.3.1.dev9/graspologic/pipeline/embed/_elbow.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         if s2.size != 0:
             mu2 = np.mean(s2)
         else:
             # Prevent numpy warning for taking mean of empty array
             mu2 = -np.inf
 
         # compute pooled variance
-        variance = ((np.sum((s1 - mu1) ** 2) + np.sum((s2 - mu2) ** 2))) / (
+        variance = (np.sum((s1 - mu1) ** 2) + np.sum((s2 - mu2) ** 2)) / (
             n_elements - 1 - (idx < n_elements)
         )
         std = np.sqrt(variance)
 
         # compute log likelihoods
         likelihoods[idx - 1] = np.sum(norm.logpdf(s1, loc=mu1, scale=std)) + np.sum(
             norm.logpdf(s2, loc=mu2, scale=std)
```

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/pipeline/embed/adjacency_spectral_embedding.py` & `graspologic-3.3.1.dev9/graspologic/pipeline/embed/adjacency_spectral_embedding.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/pipeline/embed/embeddings.py` & `graspologic-3.3.1.dev9/graspologic/pipeline/embed/embeddings.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/pipeline/embed/laplacian_spectral_embedding.py` & `graspologic-3.3.1.dev9/graspologic/pipeline/embed/laplacian_spectral_embedding.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/pipeline/embed/omnibus_embedding.py` & `graspologic-3.3.1.dev9/graspologic/pipeline/embed/omnibus_embedding.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,17 +161,17 @@
     graph_embeddings = []
 
     # create a graph that contains all nodes and edges across the entire corpus
     union_graph = graphs[0].copy()
     for graph in graphs[1:]:
         union_graph.add_edges_from(graph.edges())
 
-    union_graph_lcc: Union[
-        nx.Graph, nx.Digraph, nx.OrderedGraph, nx.OrderedDiGraph
-    ] = largest_connected_component(union_graph)
+    union_graph_lcc: Union[nx.Graph, nx.Digraph, nx.OrderedGraph, nx.OrderedDiGraph] = (
+        largest_connected_component(union_graph)
+    )
     union_graph_lcc_nodes: Set[Any] = set(list(union_graph_lcc.nodes()))
 
     union_node_ids = np.array(list(union_graph_lcc_nodes))
 
     previous_graph = graphs[0].copy()
 
     for graph in graphs[1:]:
@@ -216,20 +216,18 @@
             elbow_cut, graph.is_directed(), model.singular_values_, previous_embedding
         )
 
         current_embedding_cut = _elbow_cut_if_needed(
             elbow_cut, graph.is_directed(), model.singular_values_, current_embedding
         )
 
-        graph_embeddings.append(
-            (
-                Embeddings(union_node_ids, previous_embedding_cut),
-                Embeddings(union_node_ids, current_embedding_cut),
-            )
-        )
+        graph_embeddings.append((
+            Embeddings(union_node_ids, previous_embedding_cut),
+            Embeddings(union_node_ids, current_embedding_cut),
+        ))
 
     return graph_embeddings
 
 
 def _graphs_precondition_checks(
     graphs: List[NxGraphType],
     weight_attribute: str,
```

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/pipeline/graph_builder.py` & `graspologic-3.3.1.dev9/graspologic/pipeline/graph_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     @beartype
     def add_edge(
         self,
         source: Any,
         target: Any,
         weight: Union[int, float] = 1.0,
         sum_weight: bool = True,
-        **attributes: Any
+        **attributes: Any,
     ) -> None:
         """
         Adds a weighted edge between the provided source and target. The source
         and target id are converted to a unique ``int``.
 
         If no weight is provided, a default weight of ``1.0`` is used.
```

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/plot/__init__.py` & `graspologic-3.3.1.dev9/graspologic/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/plot/plot.py` & `graspologic-3.3.1.dev9/graspologic/plot/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿# Copyright (c) Microsoft Corporation and contributors.
+# Copyright (c) Microsoft Corporation and contributors.
 # Licensed under the MIT License.
 
 import warnings
 from typing import Any, Collection, Literal, Optional, Union
 
 import matplotlib as mpl
 import matplotlib.axes
@@ -68,17 +68,15 @@
     # Handle context
     if context is not None:
         if not isinstance(context, str):
             msg = "context must be a string, not {}.".format(type(context))
             raise TypeError(msg)
         elif context not in ["paper", "notebook", "talk", "poster"]:
             msg = "context must be one of (paper, notebook, talk, poster), \
-                not {}.".format(
-                context
-            )
+                not {}.".format(context)
             raise ValueError(msg)
 
     # Handle font_scale
     if font_scale is not None:
         if not isinstance(font_scale, (int, float)):
             msg = "font_scale must be an integer or float, not {}.".format(
                 type(font_scale)
@@ -872,24 +870,22 @@
 
     # reformat covariances in preparation for ellipse plotting
     if gmm.covariance_type == "tied":
         covariances = np.repeat(
             gmm.covariances_[np.newaxis, :, :], n_components, axis=0
         )
     elif gmm.covariance_type == "diag":
-        covariances = np.array(
-            [np.diag(gmm.covariances_[i]) for i in range(n_components)]
-        )
+        covariances = np.array([
+            np.diag(gmm.covariances_[i]) for i in range(n_components)
+        ])
     elif gmm.covariance_type == "spherical":
-        covariances = np.array(
-            [
-                np.diag(np.repeat(gmm.covariances_[i], X.shape[1]))
-                for i in range(n_components)
-            ]
-        )
+        covariances = np.array([
+            np.diag(np.repeat(gmm.covariances_[i], X.shape[1]))
+            for i in range(n_components)
+        ])
 
     # setting up the data DataFrame
     if labels is None:
         lab_names = [i for i in range(n_components)]
         data["labels"] = np.asarray([lab_names[Y_[i]] for i in range(Y_.shape[0])])
     else:
         data["labels"] = labels
```

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/plot/plot_matrix.py` & `graspologic-3.3.1.dev9/graspologic/plot/plot_matrix.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/preconditions.py` & `graspologic-3.3.1.dev9/graspologic/preconditions.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/preprocessing/__init__.py` & `graspologic-3.3.1.dev9/graspologic/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/preprocessing/graph_cuts.py` & `graspologic-3.3.1.dev9/graspologic/preprocessing/graph_cuts.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/simulations/rdpg_corr.py` & `graspologic-3.3.1.dev9/graspologic/simulations/rdpg_corr.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/simulations/simulations.py` & `graspologic-3.3.1.dev9/graspologic/simulations/simulations.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/simulations/simulations_corr.py` & `graspologic-3.3.1.dev9/graspologic/simulations/simulations_corr.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/subgraph/sg.py` & `graspologic-3.3.1.dev9/graspologic/subgraph/sg.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,20 +109,18 @@
             raise ValueError(msg)
         else:
             self.graphs = graphs
             self.labels = labels
 
         self.__construct_contingency()
         verts = np.shape(self.graphs)[0]
-        sigmat = np.array(
-            [
-                [fisher_exact(self.contmat_[i, j, :, :])[1] for j in range(verts)]
-                for i in range(verts)
-            ]
-        )
+        sigmat = np.array([
+            [fisher_exact(self.contmat_[i, j, :, :])[1] for j in range(verts)]
+            for i in range(verts)
+        ])
 
         if isinstance(constraints, (int)):  # incoherent
             nedges = constraints
             _sigsub_dstack = np.dstack(
                 np.unravel_index(np.argsort(sigmat.ravel()), np.shape(sigmat))
             )
             _sigsub = _sigsub_dstack[0, :nedges, :]
```

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/types.py` & `graspologic-3.3.1.dev9/graspologic/types.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/utils/__init__.py` & `graspologic-3.3.1.dev9/graspologic/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/utils/ptr.py` & `graspologic-3.3.1.dev9/graspologic/utils/ptr.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/utils/utils.py` & `graspologic-3.3.1.dev9/graspologic/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from graspologic.types import Dict, List, Tuple
 
 from ..types import GraphRepresentation
 
 
 @beartype
 def average_matrices(
-    matrices: Union[np.ndarray, Union[List[np.ndarray], List[csr_array]]]
+    matrices: Union[np.ndarray, Union[List[np.ndarray], List[csr_array]]],
 ) -> Union[np.ndarray, csr_array]:
     """
     Helper method to encapsulate calculating the average of matrices represented either as a
     list of numpy.ndarray or a list of scipy.sparse.csr_array.
 
     Parameters
     ----------
@@ -100,17 +100,15 @@
             allow_nd=True,  # For omni tensor input
             ensure_min_features=min_features,
             ensure_min_samples=min_samples,
             copy=copy,
         )
     else:
         msg = "Input must be networkx.Graph, np.array, or scipy.sparse.csr_array,\
-        not {}.".format(
-            type(graph)
-        )
+        not {}.".format(type(graph))
         raise TypeError(msg)
     return out
 
 
 def import_edgelist(
     path: Union[str, Path, Iterable[Union[str, Path]]],
     extension: str = "edgelist",
@@ -1156,17 +1154,17 @@
             node_id_dict[source] = str(len(node_id_dict.keys()))
 
         if target not in node_id_dict:
             node_id_dict[target] = str(len(node_id_dict.keys()))
 
         graph_remapped.add_edge(node_id_dict[source], node_id_dict[target])
 
-        graph_remapped[node_id_dict[source]][node_id_dict[target]][
-            weight_attribute
-        ] = weight
+        graph_remapped[node_id_dict[source]][node_id_dict[target]][weight_attribute] = (
+            weight
+        )
 
     return graph_remapped, node_id_dict
 
 
 def suppress_common_warnings() -> None:
     """
     Suppresses common warnings that occur when using graspologic.
```

### Comparing `graspologic-3.3.0.dev6345475692/graspologic/version.py` & `graspologic-3.3.1.dev9/graspologic/version.py`

 * *Files identical despite different names*

