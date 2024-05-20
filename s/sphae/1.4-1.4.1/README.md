# Comparing `tmp/sphae-1.4.tar.gz` & `tmp/sphae-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphae-1.4.tar", last modified: Tue May  7 04:43:26 2024, max compression
+gzip compressed data, was "sphae-1.4.1.tar", last modified: Mon May 20 01:16:30 2024, max compression
```

## Comparing `sphae-1.4.tar` & `sphae-1.4.1.tar`

### file list

```diff
@@ -1,83 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:43:26.771425 sphae-1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-07 04:43:22.000000 sphae-1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-07 04:43:22.000000 sphae-1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11043 2024-05-07 04:43:26.771425 sphae-1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9939 2024-05-07 04:43:22.000000 sphae-1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 04:43:26.771425 sphae-1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-07 04:43:22.000000 sphae-1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:43:26.763425 sphae-1.4/sphae/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 04:43:22.000000 sphae-1.4/sphae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-05-07 04:43:22.000000 sphae-1.4/sphae/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:43:26.763425 sphae-1.4/sphae/config/
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-07 04:43:22.000000 sphae-1.4/sphae/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-07 04:43:22.000000 sphae-1.4/sphae/sphae.CITATION
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-07 04:43:22.000000 sphae-1.4/sphae/sphae.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-07 04:43:22.000000 sphae-1.4/sphae/sphae.VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:43:26.763425 sphae-1.4/sphae/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/Snakefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:43:26.763425 sphae-1.4/sphae/workflow/envs/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/envs/checkv.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/envs/flye.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/envs/graph.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/envs/medaka.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/envs/megahit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/envs/pharokka.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/envs/phold.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/envs/phynteny.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/envs/samtools.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/envs/trimnami.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/envs/viralverify.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/install.smk
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:43:26.767425 sphae-1.4/sphae/workflow/rules/
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/rules/1.preflight-database.smk
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/rules/1.preflight.smk
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/rules/10.final-reporting.smk
--rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/rules/2.targets.smk
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/rules/3.qc_qa.smk
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/rules/4.assembly.smk
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/rules/5.checkv.smk
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/rules/5.components.smk
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/rules/5.viralverify.smk
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/rules/6.phage_genome.smk
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/rules/6.stat_join.smk
--rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/rules/7.pharokka.smk
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/rules/8.phold.smk
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/rules/9.phynteny.smk
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:43:26.767425 sphae-1.4/sphae/workflow/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     5812 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/components.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    32928 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/fastg2gfa
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:43:26.767425 sphae-1.4/sphae/workflow/scripts/graph_utils/
--rw-r--r--   0 runner    (1001) docker     (127)    20327 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/graph_utils/build_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1651 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/joining_stats.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1898 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/pick_phage_contigs.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1758 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/rename_genomes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:43:26.771425 sphae-1.4/sphae/workflow/scripts/roblib/
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/roblib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/roblib/alignments.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/roblib/bcolors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/roblib/blast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/roblib/colours.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/roblib/date_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/roblib/dna.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/roblib/dnadist.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/roblib/file_chooser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/roblib/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10765 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/roblib/genbank.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/roblib/geography.py
--rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/roblib/newick.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/roblib/rob_error.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2355 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/roblib/seqio_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10890 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/roblib/sequences.py
--rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/roblib/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/roblib/strings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/roblib/translate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9164 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:43:26.771425 sphae-1.4/sphae.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11043 2024-05-07 04:43:26.000000 sphae-1.4/sphae.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-05-07 04:43:26.000000 sphae-1.4/sphae.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 04:43:26.000000 sphae-1.4/sphae.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-07 04:43:26.000000 sphae-1.4/sphae.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 04:43:26.000000 sphae-1.4/sphae.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-07 04:43:26.000000 sphae-1.4/sphae.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:43:26.771425 sphae-1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-07 04:43:22.000000 sphae-1.4/tests/test_sphae.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:16:30.023738 sphae-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-20 01:16:26.000000 sphae-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-20 01:16:26.000000 sphae-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11955 2024-05-20 01:16:30.023738 sphae-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10849 2024-05-20 01:16:26.000000 sphae-1.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 01:16:30.023738 sphae-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-20 01:16:26.000000 sphae-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:16:30.015738 sphae-1.4.1/sphae/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8629 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:16:30.015738 sphae-1.4.1/sphae/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/sphae.CITATION
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/sphae.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/sphae.VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:16:30.015738 sphae-1.4.1/sphae/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/Snakefile
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/Snakefile-annot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:16:30.015738 sphae-1.4.1/sphae/workflow/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/envs/checkv.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/envs/flye.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/envs/graph.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/envs/medaka.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/envs/megahit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/envs/pharokka.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/envs/phold.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/envs/phynteny.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/envs/qc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/envs/samtools.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/envs/viralverify.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/install.smk
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:16:30.019738 sphae-1.4.1/sphae/workflow/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/rules/1.preflight-annot.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/rules/1.preflight.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     7452 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/rules/10.final-reporting.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/rules/2.targets-annot.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/rules/2.targets.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/rules/3.qc_qa.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/rules/4.assembly.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/rules/5.checkv.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/rules/5.components.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/rules/5.viralverify.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/rules/6.phage_genome.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/rules/6.stat_join.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/rules/7.pharokka.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     8567 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/rules/789.annot.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/rules/8.phold.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/rules/9.phynteny.smk
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:16:30.019738 sphae-1.4.1/sphae/workflow/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5812 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/scripts/components.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    32928 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/scripts/fastg2gfa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:16:30.019738 sphae-1.4.1/sphae/workflow/scripts/graph_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    20327 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/scripts/graph_utils/build_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1651 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/scripts/joining_stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1898 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/scripts/pick_phage_contigs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1758 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/scripts/rename_genomes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:16:30.023738 sphae-1.4.1/sphae/workflow/scripts/roblib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/scripts/roblib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/scripts/roblib/alignments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/scripts/roblib/bcolors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/scripts/roblib/blast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/scripts/roblib/colours.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/scripts/roblib/date_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/scripts/roblib/dna.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/scripts/roblib/dnadist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/scripts/roblib/file_chooser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/scripts/roblib/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10765 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/scripts/roblib/genbank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/scripts/roblib/geography.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/scripts/roblib/newick.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/scripts/roblib/rob_error.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2355 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/scripts/roblib/seqio_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10890 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/scripts/roblib/sequences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/scripts/roblib/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/scripts/roblib/strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/scripts/roblib/translate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7667 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/scripts/summary-annot.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9890 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/scripts/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-20 01:16:26.000000 sphae-1.4.1/sphae/workflow/scripts/summary_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:16:30.023738 sphae-1.4.1/sphae.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11955 2024-05-20 01:16:30.000000 sphae-1.4.1/sphae.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-20 01:16:30.000000 sphae-1.4.1/sphae.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 01:16:30.000000 sphae-1.4.1/sphae.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-20 01:16:30.000000 sphae-1.4.1/sphae.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 01:16:30.000000 sphae-1.4.1/sphae.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-20 01:16:30.000000 sphae-1.4.1/sphae.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:16:30.023738 sphae-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-20 01:16:26.000000 sphae-1.4.1/tests/test_sphae.py
```

### Comparing `sphae-1.4/LICENSE` & `sphae-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sphae-1.4/PKG-INFO` & `sphae-1.4.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphae
-Version: 1.4
+Version: 1.4.1
 Summary: Assembling pure culture phages from both Illumina and Nanopore sequencing technology
 Home-page: https://github.com/linsalrob/sphae
 Author: Bhavya Papudeshi
 Author-email: npbhavya13@gmail.com
 License: The MIT License (MIT)
 Keywords: phage 'phage therapy' bioinformatics microbiology bacteria genome genomics
 Platform: any
@@ -40,36 +40,34 @@
 ## Phage toolkit to detect phage candidates for phage therapy
 <p align="center">
   <img src="sphae.png#gh-light-mode-only" width="300">
   <img src="sphaedark.png#gh-dark-mode-only" width="300">
 </p>
 
 
-
 **Overview**
 
 This snakemake workflow was built using Snaketool [https://doi.org/10.1371/journal.pcbi.1010705], to assemble and annotate phage sequences. Currently, this tool is being developed for phage genomes. The steps include,
 
 - Quality control that removes adaptor sequences, low-quality reads and host contamination (optional). 
 - Assembly
 - Contig quality checks; read coverage, viral or not, completeness, and assembly graph components. 
-- Phage genome annotation'
-- Annotation of the phage genome 
+- Phage genome annotation
   
-A complete list of programs used for each step is mentioned in the sphae.CITATION file. 
+A complete list of programs used for each step is mentioned in the `sphae.CITATION` file. 
 
 ### Install 
 
 **Pip install**
 
 ```bash
 pip install sphae
 ```
 
-** conda install** 
+**Conda install** 
 ```bash
 conda install sphae
 ```
 **Source Install**
 
 Setting up a new conda environment 
 
@@ -92,29 +90,34 @@
 pip install -e .
 
 #confirm the workflow is installed by running the below command 
 sphae --help
 ```
 
 ## Installing databases
-Run command,
+Run the below command,
 
-```
+```bash
+#Installs the database to default directory, `sphae/workflow/databases`
 sphae install
+
+#Install database to specific directory
+sphae install --db-dir <directory> 
 ```
 
   Install the databases to a directory, `sphae/workflow/databases`
 
   This workflow requires the 
   - Pfam35.0 database to run viral_verify for contig classification. 
   - CheckV database to test for phage completeness
   - Pharokka databases 
   - Phynteny models
+  - Phold databases
 
-This step takes approximately 1hr 30min to install and requires 9G of storage
+This step requires ~17G of storage
 
 ## Running the workflow
 
 The command `sphae run` will run QC, assembly and annotation
 
 **Commands to run**
 
@@ -125,15 +128,22 @@
 sphae run --input tests/data/illumina-subset --output example -k 
 
 #For nanopore reads, place the reads, one file per sample in a directory
 sphae run --input tests/data/nanopore-subset --sequencing longread --output example -k
 
 #To run either of the commands on the cluster, add --profile slurm to the command. For instance here is the command for longreads/nanopore reads 
 #Before running this below command, make sure have slurm config files setup, here is a tutorial, https://fame.flinders.edu.au/blog/2021/08/02/snakemake-profiles-updated 
-sphae run --input tests/data/nanopore-subset --preprocess longread --output example --profile slurm -k
+sphae run --input tests/data/nanopore-subset --preprocess longread --output example --profile slurm -k --threads 16
+```
+
+**Command to run only annotation steps**
+
+```bash
+#the genomes directory has the already assembled complete genomes
+sphae annotate --genome <genomes directory> --output example -k 
 ```
 
 **Output**
 
 Output is saved to `example/RESULTS` directory. In this directory, there will be four files 
   - Genome annotations in GenBank format (Phynteny output)
   - Genome in fasta format (either the reoriented to terminase output from Pharokka, or assembled viral contigs)
@@ -147,22 +157,19 @@
   - If the assembled contig is circular or not (From the assembly graph)
   - Completeness (calculated from CheckV)
   - Contamination (calculated from CheckV)
   - Taxonomy accession ID (Pharokka output, searches the genome against INPHARED database using mash)
   - Taxa mash includes the number of matching hashes of the assembled genome to the accession ID/Taxa name. Higher the matching hash- more likely the genome is related to the taxa predicted
   - Gene searches:
     - Whether integrase is found (search for integrase gene in annotations)
-    - Whether anti-microbial genes were found (Pharokka search against AMR database)
+    - Whether anti-microbial genes were found (Phold and Pharokka search against AMR database)
     - Whether any virulence factors were found (Pharokka search against virulence gene database)
     - Whether any CRISPR spacers were found (Pharokka search against MinCED database) 
- 
 
 ### FAQ
-- Sure, here are the clarifications for each scenario:
-
 1. **"Failed during assembly":**
    - This message indicates that the assembly process was unsuccessful. It suggests that the assembler could not generate contigs, which are contiguous sequences of DNA, typically representing segments of a genome. 
    - To confirm this, you can check the logs located at `sphae.out/PROCESSING/assembly/flye/<sample name>/assembly_info.txt` or `sphae.out/PROCESSING/assembly/megahit/<sample name>/log`. These logs should provide details about the error or the step at which the assembly failed.
    - One possible reason for this failure could be insufficient genome coverage, meaning that there were not enough sequencing reads to accurately assemble the genome.
 
 2. **"Genome includes multiple contigs, fragmented":**
    - This message indicates that the assembly generated numerous short fragments (contigs) instead of a single, contiguous sequence representing a nearly complete phage genome. 
@@ -177,26 +184,34 @@
      subsample:
          --bases 1000M
      ```
    - Increase or decrease the number of bases (e.g., `1000M` for 1000 megabases) based on your requirements.
    - After making the changes, rerun sphae and ensure that the updated subsampling parameters are reflected in the `sphae.out/sphae.config.yaml` file.
 
 4. **"What does 'No integrases found ...but Phynteny predicted a few unknown function genes to have some similarity with integrase genes but with low confidence. Maybe a false positive or a novel integrase gene' mean?"**
-  This message indicates that while no integrase genes were explicitly identified, the analysis detected certain genes that exhibited similarities to integrase genes. However, these genes were associated with low confidence scores, suggesting a possibility of being false positives or potentially representing novel integrase genes.
-
-  [Phynteny](https://github.com/susiegriggo/Phynteny), the tool used for this prediction, assigns a confidence score to each gene prediction. If this score falls below a certain threshold (typically 90%), the gene remains classified as having an unknown function. To further investigate these genes, advanced techniques such as folding using tools like [ColabFold](https://github.com/sokrypton/ColabFold) can be employed. Analyzing the structure of these genes may provide additional insights into their functionality and potential role in biological processes.
-
-5. **How do I visualize the phages and gene annotations?**
+   This message indicates that while no integrase genes were explicitly identified, the analysis detected certain genes that exhibited similarities to integrase genes. However, these genes were associated with low confidence scores, suggesting a possibility of being false positives or potentially representing novel integrase genes.
+   
+   [Phynteny](https://github.com/susiegriggo/Phynteny), the tool used for this prediction, assigns a confidence score to each gene prediction. If this score falls below a certain threshold (typically 90%), the gene remains classified as having an unknown function. To further investigate these genes, advanced techniques such as folding using tools like [ColabFold](https://github.com/sokrypton/ColabFold) and [Foldseek](https://github.com/steineggerlab/foldseek) can be employed. Analyzing the structure of these genes may provide additional insights into their functionality and potential role in biological processes.
+
+1. **How do I visualize the phages and gene annotations?**
+   To visualize the phages and gene annotations, I recommend using [Clinker](https://github.com/gamcil/clinker). First, gather all the sample genbank files from `sphae.out/RESULTS` and place them in a new directory. Then, execute the clinker command to generate clinker plots, which compare the genes in each genome to each other.
+   
+   Additionally, for enhanced visualization, consider running [dnaapler](https://github.com/gbouras13/dnaapler) on the genomes in fasta format obtained from 
+   `sphae.out/RESULTS`. This step generates reoriented phages that start with terminase genes. Pharokka -> Phold -> Phynteny has to be rerun, and the resulting genbank files can be used for visualization. To perform the annotation steps, run the command 
+   `sphae annotate --input <reoriented genomes from dnaapler in fasta format directory>`
+   
+   Please note that dnaapler may fail if terminase genes are not found, particularly when working with novel phages. The reason these steps haven't been added to sphae. If you encounter any challenges during this process, please feel free to leave an issue, and I'll provide improved documentation to assist you further with the command on how to install and run the command different commands. 
 
-  To visualize the phages and gene annotations, I recommend using [Clinker](https://github.com/gamcil/clinker). First, gather all the sample genbank files from `sphae.out/RESULTS` and place them in a new directory. Then, execute the clinker command to generate clinker plots, which compare the genes in each genome to each other.
-
-  Additionally, for enhanced visualization, consider running [dnaapler](https://github.com/gbouras13/dnaapler) on the genomes in fasta format obtained from `sphae.out/RESULTS`. This step generates reoriented phages that start with terminase genes. Pharokka has been rerun, and the resulting genbank files can be used for visualization. 
+2. **Where are the intermediate files being saved?**
+   These files are being saved in `sphae.out/PROCESSING`. If you need more information on the file structure here, or have ideas of better organization then leave an issue and I will make a note to have more documentation. 
 
-  Please note that dnaapler may fail if terminase genes are not found, particularly when working with novel phages. The reason these steps haven't been added to sphae. If you encounter any challenges during this process, please feel free to leave an issue, and I'll provide improved documentation to assist you further with the command on how to install and run the command different commands. 
+3. **Just run annotation on already assembled genomes?**
+   
+    `sphae annotate --input <input genomes>`
+    This command runs only Pharokka, Phold and Phynteny to annotate the assembled genomes. The results are saved to a new directory labeled `sphae.out/annotation`. 
 
-6. **Where are the intermediate files being saved?**
-   These files are being saved in `sphae.out/PROCESSING`. If you need more information on the file structure here, or have ideas of better organization then leave an issue and I will make a note to have more documentation. 
+    Note: Currently, Sphae runs Phold in CPU mode, but efforts are underway to support Phold GPU mode for faster processing of this step.
 
 ## Issues and Questions
 
-This is still a work in progress, so if you come across any issues or errors, report them under Issues. 
+If you come across any issues or errors, report them under [Issues](https://github.com/linsalrob/sphae/issues).
```

### Comparing `sphae-1.4/README.md` & `sphae-1.4.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -10,36 +10,34 @@
 ## Phage toolkit to detect phage candidates for phage therapy
 <p align="center">
   <img src="sphae.png#gh-light-mode-only" width="300">
   <img src="sphaedark.png#gh-dark-mode-only" width="300">
 </p>
 
 
-
 **Overview**
 
 This snakemake workflow was built using Snaketool [https://doi.org/10.1371/journal.pcbi.1010705], to assemble and annotate phage sequences. Currently, this tool is being developed for phage genomes. The steps include,
 
 - Quality control that removes adaptor sequences, low-quality reads and host contamination (optional). 
 - Assembly
 - Contig quality checks; read coverage, viral or not, completeness, and assembly graph components. 
-- Phage genome annotation'
-- Annotation of the phage genome 
+- Phage genome annotation
   
-A complete list of programs used for each step is mentioned in the sphae.CITATION file. 
+A complete list of programs used for each step is mentioned in the `sphae.CITATION` file. 
 
 ### Install 
 
 **Pip install**
 
 ```bash
 pip install sphae
 ```
 
-** conda install** 
+**Conda install** 
 ```bash
 conda install sphae
 ```
 **Source Install**
 
 Setting up a new conda environment 
 
@@ -62,29 +60,34 @@
 pip install -e .
 
 #confirm the workflow is installed by running the below command 
 sphae --help
 ```
 
 ## Installing databases
-Run command,
+Run the below command,
 
-```
+```bash
+#Installs the database to default directory, `sphae/workflow/databases`
 sphae install
+
+#Install database to specific directory
+sphae install --db-dir <directory> 
 ```
 
   Install the databases to a directory, `sphae/workflow/databases`
 
   This workflow requires the 
   - Pfam35.0 database to run viral_verify for contig classification. 
   - CheckV database to test for phage completeness
   - Pharokka databases 
   - Phynteny models
+  - Phold databases
 
-This step takes approximately 1hr 30min to install and requires 9G of storage
+This step requires ~17G of storage
 
 ## Running the workflow
 
 The command `sphae run` will run QC, assembly and annotation
 
 **Commands to run**
 
@@ -95,15 +98,22 @@
 sphae run --input tests/data/illumina-subset --output example -k 
 
 #For nanopore reads, place the reads, one file per sample in a directory
 sphae run --input tests/data/nanopore-subset --sequencing longread --output example -k
 
 #To run either of the commands on the cluster, add --profile slurm to the command. For instance here is the command for longreads/nanopore reads 
 #Before running this below command, make sure have slurm config files setup, here is a tutorial, https://fame.flinders.edu.au/blog/2021/08/02/snakemake-profiles-updated 
-sphae run --input tests/data/nanopore-subset --preprocess longread --output example --profile slurm -k
+sphae run --input tests/data/nanopore-subset --preprocess longread --output example --profile slurm -k --threads 16
+```
+
+**Command to run only annotation steps**
+
+```bash
+#the genomes directory has the already assembled complete genomes
+sphae annotate --genome <genomes directory> --output example -k 
 ```
 
 **Output**
 
 Output is saved to `example/RESULTS` directory. In this directory, there will be four files 
   - Genome annotations in GenBank format (Phynteny output)
   - Genome in fasta format (either the reoriented to terminase output from Pharokka, or assembled viral contigs)
@@ -117,22 +127,19 @@
   - If the assembled contig is circular or not (From the assembly graph)
   - Completeness (calculated from CheckV)
   - Contamination (calculated from CheckV)
   - Taxonomy accession ID (Pharokka output, searches the genome against INPHARED database using mash)
   - Taxa mash includes the number of matching hashes of the assembled genome to the accession ID/Taxa name. Higher the matching hash- more likely the genome is related to the taxa predicted
   - Gene searches:
     - Whether integrase is found (search for integrase gene in annotations)
-    - Whether anti-microbial genes were found (Pharokka search against AMR database)
+    - Whether anti-microbial genes were found (Phold and Pharokka search against AMR database)
     - Whether any virulence factors were found (Pharokka search against virulence gene database)
     - Whether any CRISPR spacers were found (Pharokka search against MinCED database) 
- 
 
 ### FAQ
-- Sure, here are the clarifications for each scenario:
-
 1. **"Failed during assembly":**
    - This message indicates that the assembly process was unsuccessful. It suggests that the assembler could not generate contigs, which are contiguous sequences of DNA, typically representing segments of a genome. 
    - To confirm this, you can check the logs located at `sphae.out/PROCESSING/assembly/flye/<sample name>/assembly_info.txt` or `sphae.out/PROCESSING/assembly/megahit/<sample name>/log`. These logs should provide details about the error or the step at which the assembly failed.
    - One possible reason for this failure could be insufficient genome coverage, meaning that there were not enough sequencing reads to accurately assemble the genome.
 
 2. **"Genome includes multiple contigs, fragmented":**
    - This message indicates that the assembly generated numerous short fragments (contigs) instead of a single, contiguous sequence representing a nearly complete phage genome. 
@@ -147,26 +154,34 @@
      subsample:
          --bases 1000M
      ```
    - Increase or decrease the number of bases (e.g., `1000M` for 1000 megabases) based on your requirements.
    - After making the changes, rerun sphae and ensure that the updated subsampling parameters are reflected in the `sphae.out/sphae.config.yaml` file.
 
 4. **"What does 'No integrases found ...but Phynteny predicted a few unknown function genes to have some similarity with integrase genes but with low confidence. Maybe a false positive or a novel integrase gene' mean?"**
-  This message indicates that while no integrase genes were explicitly identified, the analysis detected certain genes that exhibited similarities to integrase genes. However, these genes were associated with low confidence scores, suggesting a possibility of being false positives or potentially representing novel integrase genes.
-
-  [Phynteny](https://github.com/susiegriggo/Phynteny), the tool used for this prediction, assigns a confidence score to each gene prediction. If this score falls below a certain threshold (typically 90%), the gene remains classified as having an unknown function. To further investigate these genes, advanced techniques such as folding using tools like [ColabFold](https://github.com/sokrypton/ColabFold) can be employed. Analyzing the structure of these genes may provide additional insights into their functionality and potential role in biological processes.
-
-5. **How do I visualize the phages and gene annotations?**
+   This message indicates that while no integrase genes were explicitly identified, the analysis detected certain genes that exhibited similarities to integrase genes. However, these genes were associated with low confidence scores, suggesting a possibility of being false positives or potentially representing novel integrase genes.
+   
+   [Phynteny](https://github.com/susiegriggo/Phynteny), the tool used for this prediction, assigns a confidence score to each gene prediction. If this score falls below a certain threshold (typically 90%), the gene remains classified as having an unknown function. To further investigate these genes, advanced techniques such as folding using tools like [ColabFold](https://github.com/sokrypton/ColabFold) and [Foldseek](https://github.com/steineggerlab/foldseek) can be employed. Analyzing the structure of these genes may provide additional insights into their functionality and potential role in biological processes.
+
+1. **How do I visualize the phages and gene annotations?**
+   To visualize the phages and gene annotations, I recommend using [Clinker](https://github.com/gamcil/clinker). First, gather all the sample genbank files from `sphae.out/RESULTS` and place them in a new directory. Then, execute the clinker command to generate clinker plots, which compare the genes in each genome to each other.
+   
+   Additionally, for enhanced visualization, consider running [dnaapler](https://github.com/gbouras13/dnaapler) on the genomes in fasta format obtained from 
+   `sphae.out/RESULTS`. This step generates reoriented phages that start with terminase genes. Pharokka -> Phold -> Phynteny has to be rerun, and the resulting genbank files can be used for visualization. To perform the annotation steps, run the command 
+   `sphae annotate --input <reoriented genomes from dnaapler in fasta format directory>`
+   
+   Please note that dnaapler may fail if terminase genes are not found, particularly when working with novel phages. The reason these steps haven't been added to sphae. If you encounter any challenges during this process, please feel free to leave an issue, and I'll provide improved documentation to assist you further with the command on how to install and run the command different commands. 
 
-  To visualize the phages and gene annotations, I recommend using [Clinker](https://github.com/gamcil/clinker). First, gather all the sample genbank files from `sphae.out/RESULTS` and place them in a new directory. Then, execute the clinker command to generate clinker plots, which compare the genes in each genome to each other.
-
-  Additionally, for enhanced visualization, consider running [dnaapler](https://github.com/gbouras13/dnaapler) on the genomes in fasta format obtained from `sphae.out/RESULTS`. This step generates reoriented phages that start with terminase genes. Pharokka has been rerun, and the resulting genbank files can be used for visualization. 
+2. **Where are the intermediate files being saved?**
+   These files are being saved in `sphae.out/PROCESSING`. If you need more information on the file structure here, or have ideas of better organization then leave an issue and I will make a note to have more documentation. 
 
-  Please note that dnaapler may fail if terminase genes are not found, particularly when working with novel phages. The reason these steps haven't been added to sphae. If you encounter any challenges during this process, please feel free to leave an issue, and I'll provide improved documentation to assist you further with the command on how to install and run the command different commands. 
+3. **Just run annotation on already assembled genomes?**
+   
+    `sphae annotate --input <input genomes>`
+    This command runs only Pharokka, Phold and Phynteny to annotate the assembled genomes. The results are saved to a new directory labeled `sphae.out/annotation`. 
 
-6. **Where are the intermediate files being saved?**
-   These files are being saved in `sphae.out/PROCESSING`. If you need more information on the file structure here, or have ideas of better organization then leave an issue and I will make a note to have more documentation. 
+    Note: Currently, Sphae runs Phold in CPU mode, but efforts are underway to support Phold GPU mode for faster processing of this step.
 
 ## Issues and Questions
 
-This is still a work in progress, so if you come across any issues or errors, report them under Issues. 
+If you come across any issues or errors, report them under [Issues](https://github.com/linsalrob/sphae/issues).
```

### Comparing `sphae-1.4/setup.py` & `sphae-1.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `sphae-1.4/sphae/__main__.py` & `sphae-1.4.1/sphae/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 Check out the wiki for a detailed look at customising this file:
 https://github.com/beardymcjohnface/Snaketool/wiki/Customising-your-Snaketool
 """
 
 import os
 import click
-
+from shutil import copyfile
 from snaketool_utils.cli_utils import OrderedCommands, run_snakemake, copy_config, echo_click
 
 
 def snake_base(rel_path):
     """Get the filepath to a Snaketool system file (relative to __main__.py)"""
     return os.path.join(os.path.dirname(os.path.realpath(__file__)), rel_path)
 
@@ -36,22 +36,23 @@
 
 
 def common_options(func):
     """Common command line args
     Define common command line args here, and include them with the @common_options decorator below.
     """
     options = [
-        click.option('--output', help='Output directory', type=click.Path(),
+        click.option('--input', '_input', help='Directory of reads', type=click.Path(), required=False, default='test/illumina-subset', show_default=True),
+        click.option('--output', 'output', help='Output directory', type=click.Path(),
                      default='sphae.out', show_default=True),
-        click.option("--configfile", default="sphae.config.yaml", show_default=False, callback=default_to_output,
-                     help="Custom config file [default: (outputDir)/sphae.config.yaml]",),
+        click.option("--configfile", default="config.yaml", show_default=False, callback=default_to_output,
+                     help="Custom config file [default: config.yaml]"),
         click.option('--threads', help='Number of threads to use', default=1, show_default=True),
         click.option('--profile', help='Snakemake profile', default=None, show_default=False),
-        click.option('--db-dir', help='Custom database directory', type=str, required=False),
-        click.option('--temp-dir', help='Temp directory', type=str, required=False),
+        click.option('--db_dir', 'db_dir', help='Custom database directory', type=click.Path(), required=False),
+        click.option('--temp-dir', help='Temp directory', required=False),
         click.option('--use-conda/--no-use-conda', default=True, help='Use conda for Snakemake rules',
                      show_default=True),
         click.option('--conda-prefix', default=snake_base(os.path.join('workflow', 'conda')),
                      help='Custom conda env directory', type=click.Path(), show_default=False),
         click.option('--snake-default', multiple=True,
                      default=['--rerun-incomplete', '--printshellcmds', '--nolock', '--show-failed-logs'],
                      help="Customise Snakemake runtime args", show_default=True),
@@ -70,76 +71,123 @@
     """Assembling pure culture phages from both Illumina and Nanopore sequencing technology
     \b
     For more options, run:
     sphae command --help"""
     pass
 
 
-help_msg_extra = """
+help_msg_run = """
+\b
+RUN EXAMPLES 
 \b
-INSTALLING DATABASES REQUIRED
-This command downloads the databases to the directory 'database' 
+#Paired end reads 
+sphae --input <input directory with paired end reads> --output <output directory> -k 
 \b
-sphae install 
+#Longread sequencing data
+sphae run --input <input directory with nanopore reads in fastq format> --sequencing longread --output <output directory> -k
 \b
+#Submit sphae run to slurm 
+sphae --input <input directory with paired end reads> --output <output directory> -k --profile slurm
+"""
+
+help_msg_install = """
 \b
-CLUSTER EXECUTION:
-sphae run ... --profile [profile]
-For information on Snakemake profiles see:
-https://snakemake.readthedocs.io/en/stable/executing/cli.html#profiles
-\b
-RUN EXAMPLES:
-Required:           sphae run --input [file]
-Specify threads:    sphae run ... --threads [threads]
-Disable conda:      sphae run ... --no-use-conda 
-Change defaults:    sphae run ... --snake-default="-k --nolock"
-Add Snakemake args: sphae run ... --dry-run --keep-going --touch
-Specify targets:    sphae run ... all print_targets
+INSTALL EXAMPLES 
 \b
+sphae install\t\t\t\tBy default, the databases are downloaded to `sphae/workflow/databases`
+sphae install --db-dir [directory]\t\tDefine the database path
 """
 
+help_msg_annotate ="""
+\b
+ANNOTATE EXAMPLES
+\b
+sphae anntoate --genome <genomes>  
+sphae annotate --genome <genomes> --output <output> #define output directory
+sphae annotate --genome <genomes> --output <output> --db <database> #define database path
+"""
 
-@click.command(epilog=help_msg_extra, context_settings=dict(help_option_names=["-h", "--help"], ignore_unknown_options=True))
-@common_options
-def install(**kwargs):
+@click.command(epilog=help_msg_install, context_settings=dict(help_option_names=["-h", "--help"], ignore_unknown_options=True))
+@click.option('--db_dir', 'db_dir', help='Custom database directory', type=click.Path(), required=False)
+@click.option('--output', 'output', help='Output directory', type=click.Path(), default='sphae.out', show_default=True)
+@click.option("--configfile", default="config.yaml", show_default=False, callback=default_to_output,help="Custom config file [default: (outputDir)/config.yaml]",)
+@click.option('--threads', help='Number of threads to use', default=1, show_default=True)
+@click.option('--profile', help='Snakemake profile', default=None, show_default=False)
+@click.option('--temp-dir', 'temp_dir', help='Temp directory', required=False)
+@click.option('--use-conda/--no-use-conda', default=True, help='Use conda for Snakemake rules',show_default=True)
+@click.option('--conda-prefix', default=snake_base(os.path.join('workflow', 'conda')),help='Custom conda env directory', type=click.Path(), show_default=False)
+@click.option('--snake-default', multiple=True,default=['--rerun-incomplete', '--printshellcmds', '--nolock', '--show-failed-logs'], help="Customise Snakemake runtime args", show_default=True)
+@click.option("--log", default="sphae.log", callback=default_to_output, hidden=True,)
+@click.option("--system-config", default=snake_base(os.path.join("config", "config.yaml")),hidden=True,)
+@click.argument("snake_args", nargs=-1)
+def install(db_dir, output, temp_dir, configfile, **kwargs):
     """The install function for databases"""
+    copy_config(configfile, system_config=snake_base(os.path.join('config', 'config.yaml')))
+
     merge_config = {
-        'sphae': {
-            'args': kwargs   
+        'args': {
+            "db_dir": db_dir, 
+            "output": output, 
+            "temp_dir": temp_dir,
+            "configfile": configfile
         }
     }
 
     # run!
     run_snakemake(
         snakefile_path=snake_base(os.path.join('workflow', 'install.smk')),
+        configfile=configfile,
         merge_config=merge_config,
         **kwargs
     )
 
+@click.command(epilog=help_msg_annotate, context_settings=dict(help_option_names=["-h", "--help"], ignore_unknown_options=True))
+@common_options
+@click.option('--genome', 'genome', help='Input genome assembled or downloaded', type=click.Path(), required=False)
+def annotate(genome, output, db_dir, temp_dir, configfile, **kwargs):
+    """Annotate option"""
+    copy_config(configfile, system_config=snake_base(os.path.join('config', 'config.yaml')))
+    merge_config = {
+        'args': {
+            "db_dir": db_dir, 
+            "output": output, 
+            "genome": genome, 
+            "temp_dir": temp_dir,
+            "configfile": configfile 
+        }
+    }
 
-@click.command(epilog=help_msg_extra, context_settings=dict(help_option_names=["-h", "--help"], ignore_unknown_options=True))
-@click.option('--input', '_input', help='Input samples TSV or directory of reads', type=str, required=False,
-                default='test/illumina-subset', show_default=True)
-@click.option('--host', help='Host genome for filtering', type=str, required=False)
-@click.option('--sequencing', help="sequencing method", default='paired', show_default=True,
-                type=click.Choice(['paired', 'longread']))
+    # run!
+    run_snakemake(
+        snakefile_path=snake_base(os.path.join('workflow', 'Snakefile-annot')),
+        configfile=configfile,
+        merge_config=merge_config,
+        **kwargs
+    )
+@click.command(epilog=help_msg_run, context_settings=dict(help_option_names=["-h", "--help"], ignore_unknown_options=True))
 @common_options
-def run(**kwargs):
+@click.option('--sequencing', 'sequencing', help="sequencing method", default='paired', show_default=True, type=click.Choice(['paired', 'longread']))
+def run(_input, output, db_dir, sequencing, temp_dir, configfile, **kwargs):
     """Run sphae"""
-
-    # Config to add or update in configfile
+    copy_config(configfile, system_config=snake_base(os.path.join('config', 'config.yaml')))
+    
     merge_config = {
-        'sphae': {
-            'args': kwargs   
+        "args": {
+            "input": _input, 
+            "output": output, 
+            "db_dir": db_dir,  
+            "sequencing": sequencing, 
+            "temp_dir": temp_dir,
         }
     }
 
     # run!
     run_snakemake(
         snakefile_path=snake_base(os.path.join('workflow', 'Snakefile')),
+        configfile=configfile,
         merge_config=merge_config,
         **kwargs
     )
 
 
 @click.command()
 @click.option('--configfile', default='config.yaml', help='Copy template config to file', show_default=True)
@@ -152,17 +200,16 @@
 def citation(**kwargs):
     """Print the citation(s) for this tool"""
     print_citation()
 
 
 cli.add_command(run)
 cli.add_command(install)
+cli.add_command(annotate)
 cli.add_command(config)
 cli.add_command(citation)
 
-
 def main():
     cli()
 
-
 if __name__ == '__main__':
-    main()
+    main()
```

### Comparing `sphae-1.4/sphae/sphae.CITATION` & `sphae-1.4.1/sphae/sphae.CITATION`

 * *Files 9% similar despite different names*

```diff
@@ -27,9 +27,11 @@
 
 Pharokka:
 https://github.com/gbouras13/pharokka
 
 Phynteny:
 https://github.com/susiegriggo/Phynteny
 
+Phold
+https://github.com/gbouras13/phold
```

### Comparing `sphae-1.4/sphae/sphae.LICENSE` & `sphae-1.4.1/sphae/sphae.LICENSE`

 * *Files identical despite different names*

### Comparing `sphae-1.4/sphae/workflow/Snakefile` & `sphae-1.4.1/sphae/workflow/Snakefile`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-import attrmap as ap
-#import attrmap.utils as au
-
+import yaml
+import os
+import glob
 
 """Parse config"""
 configfile: os.path.join(workflow.basedir, "..", "config", "config.yaml")
-config.update(config["sphae"])
-config = ap.AttrMap(config)
 
 """Rules"""
 include: os.path.join("rules", "1.preflight.smk")
 include: os.path.join("rules", "2.targets.smk")
 include: os.path.join("rules", "3.qc_qa.smk")
 include: os.path.join("rules", "4.assembly.smk")
 include: os.path.join("rules", "5.components.smk")
@@ -26,46 +24,30 @@
 """Mark target rules"""
 target_rules = []
 def targetRule(fn):
     assert fn.__name__.startswith('__')
     target_rules.append(fn.__name__[2:])
     return fn
 
-
 @targetRule
 rule all:
     input:
-        targets.qc,
-        targets.assemble,
-        targets.annotate,
-        targets.coverage,
-
+        targets['qc'],
+        targets['assemble'],
+        targets['annotate']
 
 @targetRule
 rule qc:
     input:
-        targets.qc,
+        targets['qc']
 
 
 @targetRule
 rule assemble:
     input:
-        targets.assemble,
-
-
-@targetRule
-rule coverage:
-    input:
-        targets.coverage,
-
+        targets['assemble']
 
 @targetRule
 rule annotate:
     input:
-        targets.annotate,
+        targets['annotate']
 
-
-@targetRule
-rule print_targets:
-    run:
-        print("\nTop level rules are: \n", file=sys.stderr)
-        print("* " + "\n* ".join(target_rules) + "\n\n", file=sys.stderr)
```

### Comparing `sphae-1.4/sphae/workflow/install.smk` & `sphae-1.4.1/sphae/workflow/install.smk`

 * *Files 26% similar despite different names*

```diff
@@ -1,102 +1,103 @@
-"""
-Spae
-assembly and annotation of phage genomes 
-
-2022, Bhavya Papudeshi
+import yaml
+import os
+import glob
 
-This is an auxiliary Snakefile to install databases or dependencies.
 """
-
-
-import attrmap as ap
-#import attrmap.utils as au
-
-
-"""Parse config"""
+Parse config
+"""
 configfile: os.path.join(workflow.basedir, "..", "config", "config.yaml")
-config = ap.AttrMap(config)
-
 
+"""
+DIRECTORIES
+"""
+dir = {}
+dir_env = os.path.join(workflow.basedir, "envs")
 
-"""Preflight"""
-include: "rules/1.preflight-database.smk"
+# database dir
+try:
+    if config['args']['db_dir'] is None:
+        dir_db = os.path.join(workflow.basedir, 'databases')
+    else:
+        dir_db = config['args']['db_dir']
+except KeyError:
+    dir_db = os.path.join(workflow.basedir, 'databases')
+print(f"Databases are being saved in, {dir_db} \n")
 
 """Targets"""
-targets = ap.AttrMap()
-
+targets = type('', (), {})()
 targets.db = []
 
-targets.db.append(os.path.join(databaseDir, 'Pfam35.0', 'Pfam-A.hmm.gz'))
-targets.db.append(os.path.join(databaseDir, 'pharokka_db', 'phrogs_db.index'))
-targets.db.append(os.path.join(databaseDir, 'checkv-db-v1.5', 'README.txt'))
-targets.db.append(os.path.join(databaseDir, 'phynteny_models_zenodo', 'grid_search_model.m_400.b_256.lr_0.0001.dr_0.1.l_2.a_tanh.o_rmsprop.rep_0.best_val_loss.h5'))
-targets.db.append(os.path.join(databaseDir, "phold", "phold_annots.tsv"))
+targets.db.append(os.path.join(dir_db, 'Pfam35.0', 'Pfam-A.hmm.gz'))
+targets.db.append(os.path.join(dir_db, 'pharokka_db', 'phrogs_db.index'))
+targets.db.append(os.path.join(dir_db, 'checkv-db-v1.5', 'README.txt'))
+targets.db.append(os.path.join(dir_db, 'phynteny_models_zenodo', 'grid_search_model.m_400.b_256.lr_0.0001.dr_0.1.l_2.a_tanh.o_rmsprop.rep_0.best_val_loss.h5'))
+targets.db.append(os.path.join(dir_db, "phold", "phold_annots.tsv"))
 
 """RUN SNAKEMAKE"""
 rule all:
     input:
         targets.db
 
 
 """RULES"""
 rule pfam_download:
     params:
-        os.path.join(config.db.pfam, config.db.pfam_file)
+        os.path.join(config['db']['pfam'], config['db']['pfam_file'])
     output:
-        os.path.join(databaseDir, config.db.pfam_file)
+        os.path.join(dir_db, config['db']['pfam_file'])
     shell:
         """
             curl -Lo {output} {params}
         """
 
 rule  pharokka_download:
     params: 
-        pharokka=os.path.join(databaseDir, 'pharokka_db')
+        pharokka=os.path.join(dir_db, 'pharokka_db')
     output:
-        out=os.path.join(databaseDir, 'pharokka_db', 'phrogs_db.index')
+        out=os.path.join(dir_db, 'pharokka_db', 'phrogs_db.index')
     conda:
-        os.path.join(dir.env, "pharokka.yaml")
+        os.path.join(dir_env, "pharokka.yaml")
     shell:
         """
             install_databases.py -o {params.pharokka}
         """
 
 rule checkv_database:
     params:
-        checkv_db=os.path.join(databaseDir)
+        checkv_db=os.path.join(dir_db)
     output:
-        os.path.join(databaseDir, "checkv-db-v1.5", "README.txt")
+        os.path.join(dir_db, "checkv-db-v1.5", "README.txt")
     conda:
-        os.path.join(dir.env, "checkv.yaml")
+        os.path.join(dir_env, "checkv.yaml")
     shell:
         """
             checkv download_database {params.checkv_db}
         """
 
 rule phynteny_models:
     params:
-        url = os.path.join(config.db.models),
-        download = os.path.join(databaseDir, "phynteny_models_v0.1.11.tar.gz"),
-        models = os.path.join(databaseDir)
+        url = os.path.join(config['db']['models']),
+        download = os.path.join(dir_db, "phynteny_models_v0.1.11.tar.gz"),
+        models = os.path.join(dir_db)
     output:
-        out = os.path.join(databaseDir, 'phynteny_models_zenodo', 'grid_search_model.m_400.b_256.lr_0.0001.dr_0.1.l_2.a_tanh.o_rmsprop.rep_0.best_val_loss.h5')
+        out = os.path.join(dir_db, 'phynteny_models_zenodo', 'grid_search_model.m_400.b_256.lr_0.0001.dr_0.1.l_2.a_tanh.o_rmsprop.rep_0.best_val_loss.h5')
     conda:
-        os.path.join(dir.env, "phynteny.yaml")
+        os.path.join(dir_env, "phynteny.yaml")
     shell:
         """
             wget -O {params.download} {params.url}
             tar -xvzf {params.download} -C {params.models}
         """
 
 rule phold_install:
     params:
-        phold_db=os.path.join(databaseDir, "phold")
+        phold_db=os.path.join(dir_db, "phold")
     output:
-        os.path.join(databaseDir, "phold", "phold_annots.tsv")
+        os.path.join(dir_db, "phold", "phold_annots.tsv")
     conda:
-        os.path.join(dir.env, "phold.yaml")
+        os.path.join(dir_env, "phold.yaml")
     shell:
         """
         phold install -d {params.phold_db}
         """
```

### Comparing `sphae-1.4/sphae/workflow/rules/1.preflight.smk` & `sphae-1.4.1/sphae/workflow/rules/1.preflight.smk`

 * *Files 26% similar despite different names*

```diff
@@ -1,93 +1,93 @@
 import os
-import attrmap as ap
-import attrmap.utils as au
 import glob
+import yaml
 from metasnek import fastq_finder
 
 """
-ONSTART/END/ERROR
+CONFIG FILE
 """
-def copy_log_file():
-    files = glob.glob(os.path.join(".snakemake", "log", "*.snakemake.log"))
-    if not files:
-        return None
-    current_log = max(files, key=os.path.getmtime)
-    #shell("cat " + current_log + " >> " + str(config.args.log))
-
-
-onstart:
-    """Cleanup old log files before starting"""
-    if os.path.isdir(dir.log):
-        oldLogs = filter(re.compile(r'.*.log').match, os.listdir(dir.log))
-        for logfile in oldLogs:
-            os.unlink(os.path.join(dir.log, logfile))
-
-# onsuccess:
-#     """Print a success message"""
-#     sys.stderr.write('\n\nphage_genomes finished successfully!\n\n')
-#     copy_log_file()
-
-# onerror:
-#     """Print an error message"""
-#     sys.stderr.write('\n\nERROR: phage_genomes failed to finish.\n\n')
-#     copy_log_file()
-
+configfile: os.path.join(workflow.basedir, "..", "config", "config.yaml")
 
 """
 DIRECTORIES
 """
-dir = ap.AttrMap()
-dir.out = config.args.output
-dir.fastp = os.path.join(dir.out, 'PROCESSING' ,'results','fastp')
-dir.nanopore = os.path.join(dir.out, 'PROCESSING','results','filtlong')
-dir.assembly = os.path.join(dir.out, 'PROCESSING','assembly')
-dir.megahit = os.path.join(dir.assembly, 'megahit')
-dir.flye = os.path.join(dir.assembly, 'flye')
-dir.genome = os.path.join(dir.out, 'PROCESSING','genome')
-dir.cov = os.path.join(dir.out, 'PROCESSING','coverage')
-dir.pharokka = os.path.join(dir.out, 'PROCESSING','pharokka')
-dir.log = os.path.join(dir.out, 'logs')
-dir.bench = os.path.join(dir.out, 'PROCESSING','benchmarks')
-dir.final = os.path.join(dir.out, 'RESULTS')
+dir = {}
+
+#declaring output file
+try:
+    if config['args']['output'] is None:
+        dir_out = os.path.join('sphae.out')
+    else:
+        dir_out = config['args']['output']
+except KeyError:
+    dir_out = os.path.join('sphae.out')
+
+dir_fastp = os.path.join(dir_out, 'PROCESSING' ,'fastp')
+dir_nanopore = os.path.join(dir_out, 'PROCESSING','filtlong')
+dir_assembly = os.path.join(dir_out, 'PROCESSING','assembly')
+dir_megahit = os.path.join(dir_assembly, 'megahit')
+dir_flye = os.path.join(dir_assembly, 'flye')
+dir_genome = os.path.join(dir_out, 'PROCESSING','genome')
+dir_pharokka = os.path.join(dir_out, 'PROCESSING','annotate')
+dir_log = os.path.join(dir_out, 'logs')
+dir_final = os.path.join(dir_out, 'RESULTS')
 
-dir.env = os.path.join(workflow.basedir, "envs")
-dir.script = os.path.join(workflow.basedir, "scripts")
+dir_env = os.path.join(workflow.basedir, "envs")
+dir_script = os.path.join(workflow.basedir, "scripts")
 
 # database dir
-if config.args.db_dir is None:
-    dir.db = os.path.join(workflow.basedir, 'databases')
+if config['args']['db_dir'] is None:
+    dir_db = os.path.join(workflow.basedir, 'databases')
 else:
-    dir.db = config.args.db_dir
+    dir_db = config['args']['db_dir']
 
 # temp dir
-if config.args.temp_dir is None:
-    dir.temp = os.path.join(dir.out, "temp")
+if config['args']['temp_dir'] is None:
+    dir_temp = os.path.join(dir_out, "temp")
 else:
-    dir.temp = config.args.temp_dir
+    dir_temp = config['args']['temp_dir']
 
+#reading the input files
+input_dir = config['args']['input']
 
-"""
-PARSE SAMPLES
+# List of file paths matching the pattern
+if config['args']['sequencing'] == 'paired':
+    file_paths = glob.glob(os.path.join(input_dir, '*_R1*.fastq*'))
+    samples_names = [os.path.splitext(os.path.basename(file_path))[0].rsplit('_R1', 1)[0] for file_path in file_paths]
+    extn = [os.path.splitext(os.path.basename(file_path))[0].rsplit('_R1', 1)[1] + os.path.splitext(os.path.basename(file_path))[1] for file_path in file_paths]
+elif config['args']['sequencing'] == 'longread':
+    file_paths = glob.glob(os.path.join(input_dir, '*.fastq*'))
+    samples_names, extn = zip(*(os.path.splitext(os.path.basename(file_path)) if '.' in os.path.basename(file_path) else (os.path.basename(file_path), '') for file_path in file_paths))
+    
+print(f"Samples are {samples_names}")
+print(f"Extensions are {extn}")
+
+FQEXTN = extn[0]
+PATTERN_R1 = '{sample}_R1' + FQEXTN
+PATTERN_R2 = '{sample}_R2' + FQEXTN
+PATTERN_LONG='{sample}'+FQEXTN
 
-samples (dict):
-    reads (dict):
-        r1 (str): filepath
-        r2 (str): filepath
-    names (list): keys(samples["reads"])
+"""ONSTART/END/ERROR
+Tasks to perform at various stages the start and end of a run.
 """
+def copy_log_file():
+    files = glob.glob(os.path.join(".snakemake", "log", "*.snakemake.log"))
+    if not files:
+        return None
+    current_log = max(files, key=os.path.getmtime)
+    target_log = os.path.join(dir['log'], os.path.basename(current_log))
+    shutil.copy(current_log, target_log)
 
-samples = ap.AttrMap()
-
-samples.reads = fastq_finder.parse_samples_to_dictionary(config.args._input)
-samples.names = list(au.get_keys(samples.reads))
-samples = au.convert_state(samples, read_only=True)
-fastq_finder.write_samples_tsv(samples.reads, os.path.join(dir.out, "samples.tsv"))
-
-
-"""
-Wildcard constraints
-"""
-wildcard_constraints:
-    sample="[a-zA-Z0-9_-]+",
-    host = ".{0}|\.hostRm|\.hostRm_s",
-    subsample = ".{0}|\.subsampled"
+dir = {'log': os.path.join(dir_out, 'logs')}
+onstart:
+    """Cleanup old log files before starting"""
+    if os.path.isdir(dir["log"]):
+        oldLogs = filter(re.compile(r'.*.log').match, os.listdir(dir["log"]))
+        for logfile in oldLogs:
+            os.unlink(os.path.join(dir["log"], logfile))
+onsuccess:
+    """Print a success message"""
+    sys.stderr.write('\n\nSphaehost ran successfully!\n\n')
+onerror:
+    """Print an error message"""
+    sys.stderr.write('\n\nSphaehost run failed\n\n')
```

### Comparing `sphae-1.4/sphae/workflow/rules/4.assembly.smk` & `sphae-1.4.1/sphae/workflow/rules/4.assembly.smk`

 * *Files 22% similar despite different names*

```diff
@@ -3,35 +3,33 @@
 Illumina paired end reads - Megahit
 Nanopore reads - Flye
 """
 
 rule flye:
     """Assemble longreads with Flye"""
     input:
-        os.path.join(dir.nanopore, "{sample}_S.subsampled.fastq.gz"),
+        os.path.join(dir_nanopore, "{sample}_filt.fastq.gz"),
     output:
-        fasta = os.path.join(dir.flye, "{sample}-sr", "assembly.fasta"),
-        gfa = os.path.join(dir.flye, "{sample}-sr", "assembly_graph.gfa"),
-        path= os.path.join(dir.flye, "{sample}-sr", "assembly_info.txt"),
-        log=os.path.join(dir.flye, "{sample}-sr", "flye.log")
+        fasta = os.path.join(dir_flye, "{sample}-sr", "assembly.fasta"),
+        gfa = os.path.join(dir_flye, "{sample}-sr", "assembly_graph.gfa"),
+        path= os.path.join(dir_flye, "{sample}-sr", "assembly_info.txt"),
+        log=os.path.join(dir_flye, "{sample}-sr", "flye.log")
     params:
-        out= os.path.join(dir.flye, "{sample}-sr"),
-        model = config.params.flye,
-        g = config.params.genomeSize
+        out= os.path.join(dir_flye, "{sample}-sr"),
+        model = config['params']['flye'],
+        g = config['params']['genomeSize']
     log:
-        os.path.join(dir.log, "flye.{sample}.log")
-    benchmark:
-        os.path.join(dir.bench,"flye.{sample}.txt")
+        os.path.join(dir_log, "flye.{sample}.log")
     conda:
-        os.path.join(dir.env, "flye.yaml")
+        os.path.join(dir_env, "flye.yaml")
     threads:
-        config.resources.bigjob.cpu
+        config['resources']['bigjob']['cpu']
     resources:
-        mem_mb=config.resources.bigjob.mem,
-        time=config.resources.bigjob.time
+        mem_mb=config['resources']['bigjob']['mem'],
+        time=config['resources']['bigjob']['time']
     shell:
         """
         if flye \
             {params.model} \
             {input} \
             --threads {threads}  \
             --asm-coverage 50 \
@@ -49,32 +47,30 @@
                 touch {output.log}
         fi
         """
 
 rule medaka:
     """Polish longread assembly with medaka"""
     input:
-        fasta = os.path.join(dir.flye, "{sample}-sr", "assembly.fasta"),
-        fastq = os.path.join(dir.nanopore, "{sample}_S.subsampled.fastq.gz"),
+        fasta = os.path.join(dir_flye, "{sample}-sr", "assembly.fasta"),
+        fastq = os.path.join(dir_nanopore, "{sample}_filt.fastq.gz"),
     output:
-        fasta = os.path.join(dir.flye,"{sample}-sr", "consensus.fasta")
+        fasta = os.path.join(dir_flye,"{sample}-sr", "consensus.fasta")
     conda:
-        os.path.join(dir.env, "medaka.yaml")
+        os.path.join(dir_env, "medaka.yaml")
     params:
-        model = config.params.medaka,
-        dir= directory(os.path.join(dir.flye,"{sample}-sr"))
+        model = config['params']['medaka'],
+        dir= directory(os.path.join(dir_flye,"{sample}-sr"))
     threads:
-        config.resources.bigjob.cpu
+        config['resources']['bigjob']['cpu']
     resources:
-        mem_mb=config.resources.bigjob.mem,
-        time=config.resources.bigjob.time
+        mem_mb=config['resources']['bigjob']['mem'],
+        time=config['resources']['bigjob']['time']
     log:
-        os.path.join(dir.log, "medaka.{sample}.log")
-    benchmark:
-        os.path.join(dir.bench, "medaka.{sample}.txt")
+        os.path.join(dir_log, "medaka.{sample}.log")
     shell:
         """
         if [[ -s {input.fasta} ]] ; then
             medaka_consensus \
                 -i {input.fastq} \
                 -d {input.fasta} \
                 -o {params.dir} \
@@ -87,61 +83,57 @@
         fi
         """
 
 
 rule megahit:
     """Assemble short reads with MEGAHIT"""
     input:
-        r1 = os.path.join(dir.fastp, "{sample}_R1.subsampled.fastq.gz"),
-        r2 = os.path.join(dir.fastp, "{sample}_R2.subsampled.fastq.gz")
+        r1 = os.path.join(dir_fastp, "{sample}_subsampled_R1.fastq.gz"),
+        r2 = os.path.join(dir_fastp, "{sample}_subsampled_R2.fastq.gz")
     output:
-        contigs=os.path.join(dir.megahit, "{sample}-pr", "final.contigs.fa"),
-        log=os.path.join(dir.megahit, "{sample}-pr", "log")
+        contigs=os.path.join(dir_megahit, "{sample}-pr", "final.contigs.fa"),
+        log=os.path.join(dir_megahit, "{sample}-pr", "log")
     params:
-        os.path.join(dir.megahit, "{sample}-pr")
+        os.path.join(dir_megahit, "{sample}-pr")
     log:
-        os.path.join(dir.log, "megahit.{sample}.log")
-    benchmark:
-        os.path.join(dir.bench, "megahit.{sample}.txt")
+        os.path.join(dir_log, "megahit.{sample}.log")
     threads:
-        config.resources.bigjob.cpu
+        config['resources']['bigjob']['cpu']
     resources:
-        mem_mb=config.resources.bigjob.mem,
-        time=config.resources.bigjob.time
+        mem_mb=config['resources']['bigjob']['mem'],
+        time=config['resources']['bigjob']['time']
     conda:
-        os.path.join(dir.env, "megahit.yaml")
+        os.path.join(dir_env, "megahit.yaml")
     shell:
         """
         if megahit \
             -1 {input.r1} \
             -2 {input.r2} \
             -o {params} \
             -t {threads} -f \
             2> {log}; then
-                touch {output.contigs}
-                touch {output.log}
-            else
-                touch {output.contigs}
-                touch {output.log}
+            touch {output.contigs}
+            touch {output.log}
+        else
+            touch {output.contigs}
+            touch {output.log}
         fi
         """
 
 rule fastg:
     """Save the MEGAHIT graph"""
     input:
-        os.path.join(dir.megahit, "{sample}-pr", "final.contigs.fa")
+        os.path.join(dir_megahit, "{sample}-pr", "final.contigs.fa")
     output:
-        fastg=os.path.join(dir.megahit, "{sample}-pr", "final.fastg"),
-        graph=os.path.join(dir.megahit, "{sample}-pr", "final.gfa")
+        fastg=os.path.join(dir_megahit, "{sample}-pr", "final.fastg"),
+        graph=os.path.join(dir_megahit, "{sample}-pr", "final.gfa")
     conda:
-        os.path.join(dir.env, "megahit.yaml")
+        os.path.join(dir_env, "megahit.yaml")
     log:
-        os.path.join(dir.log, "fastg.{sample}.log")
-    benchmark:
-        os.path.join(dir.bench, "fastg.{sample}.txt")
+        os.path.join(dir_log, "fastg.{sample}.log")
     shell:
         """
         if [[ -s {input} ]] ; then
             kmer=$(head -1 {input} | sed 's/>//' | sed 's/_.*//')
             megahit_toolkit contig2fastg $kmer {input} > {output.fastg} 2> {log}
             Bandage reduce {output.fastg} {output.graph} 2>> {log}
             touch {output.fastg}
```

### Comparing `sphae-1.4/sphae/workflow/rules/5.checkv.smk` & `sphae-1.4.1/sphae/workflow/rules/6.phage_genome.smk`

 * *Files 22% similar despite different names*

```diff
@@ -1,72 +1,88 @@
 """
-Running CheckV to get the completeness of phage genomes 
+The resulting assemblies can have multiple contigs, so selecting the phage contigs
 """
 
-rule checkv_megahit:
+rule genomes_megahit:
     input:
-        contigs = os.path.join(dir.megahit, "{sample}-pr", "final.contigs.fa")
+        csv = os.path.join(dir_assembly, "{sample}-assembly-stats_megahit.csv")
     output:
-        out = os.path.join(dir.megahit, "{sample}-pr", "checkv", "quality_summary.tsv")
+        out = os.path.join(dir_genome, "{sample}-pr", "{sample}-genome-candidates.csv")
     conda:
-        os.path.join(dir.env, "checkv.yaml")
+        os.path.join(dir_env, "graph.yaml")
+    localrule: True
+    log:
+        os.path.join(dir_log, "picking_contigs.{sample}.log")
+    script:
+        os.path.join(dir_script, 'pick_phage_contigs.py')
+
+rule genomes_extract_megahit:
+    input:
+        contigs = os.path.join(dir_megahit, "{sample}-pr", "final.contigs.fa"),
+        csv = os.path.join(dir_genome, "{sample}-pr", "{sample}-genome-candidates.csv"),
+    output:
+        fasta=os.path.join(dir_genome, "{sample}-pr", "{sample}.fasta")  
     params:
-        out = os.path.join(dir.megahit, "{sample}-pr", "checkv"),
-        db = os.path.join(dir.db, "checkv-db-v1.5")
+        outdir = os.path.join(dir_genome, "{sample}-pr"),
+    conda:
+        os.path.join(dir_env, "samtools.yaml")
     threads:
-        config.resources.smalljob.cpu
+        config['resources']['smalljob']['cpu']
     resources:
-        mem_mb=config.resources.smalljob.mem,
-        time=config.resources.smalljob.time
+        mem_mb = config['resources']['smalljob']['mem'],
+        time = config['resources']['smalljob']['time']
     log:
-        os.path.join(dir.log, "checkv_megahit.{sample}.log")
-    benchmark:
-        os.path.join(dir.bench, "checkv_megahit.{sample}.txt")
+        os.path.join(dir_log, "samtools.{sample}.log")
     shell:
         """
-        export CHECKVDB={params.db}
-        if [[ -s {input.contigs} ]] ; then
-            checkv end_to_end\
-                {input.contigs} \
-                {params.out} \
-                -t {threads} \
-                &> {log}
-            touch {output.out}
-        else
-            touch {output.out}
-        fi
-        """
+        #get the contig or contigs name from the csv file, and run samtools 
+        awk -F, 'NR>1 {{print $2}}' {input.csv} > {params.outdir}/phage-genome-contig
 
+        touch {output.fasta}
 
-rule checkv_flye_nano:
+        #extracting the contigs from the assembly
+        for f in `cat {params.outdir}/phage-genome-contig`; do samtools faidx {input.contigs} "$f" >> {output.fasta} ; done 
+        """    
+
+rule genomes_flye:
     input:
-        contigs = os.path.join(dir.flye, "{sample}-sr", "assembly.fasta"),
+        csv = os.path.join(dir_assembly, "{sample}-assembly-stats_flye.csv")
     output:
-        out = os.path.join(dir.flye, "{sample}-sr", "checkv", "quality_summary.tsv")
+        out =os.path.join(dir_genome, "{sample}-sr", "{sample}-genome-candidates.csv")
     conda:
-        os.path.join(dir.env, "checkv.yaml")
+        os.path.join(dir_env, "graph.yaml")
+    localrule: True
+    log:
+        os.path.join(dir_log, "picking_contigs.{sample}.log")
+    script:
+        os.path.join(dir_script, 'pick_phage_contigs.py')
+
+
+rule genomes_extract_flye:
+    input:
+        contigs = os.path.join(dir_flye, "{sample}-sr", "assembly.fasta"),
+        csv = os.path.join(dir_genome, "{sample}-sr", "{sample}-genome-candidates.csv"),
+    output:
+        os.path.join(dir_genome, "{sample}-sr", "{sample}.fasta")
     params:
-        out = os.path.join(dir.flye, "{sample}-sr", "checkv"),
-        db = os.path.join(dir.db, "checkv-db-v1.5")
+        outdir = os.path.join(dir_genome, "{sample}-sr"),
+        sample = "{sample}"
+    conda:
+        os.path.join(dir_env, "samtools.yaml")
     threads:
-        config.resources.smalljob.cpu
+        config['resources']['smalljob']['cpu']
     resources:
-        mem_mb=config.resources.smalljob.mem,
-        time=config.resources.smalljob.time
+        mem_mb = config['resources']['smalljob']['mem'],
+        time = config['resources']['smalljob']['time']
     log:
-        os.path.join(dir.log, "checkv_flye_nano.{sample}.log")
-    benchmark:
-        os.path.join(dir.bench, "checkv_flye_nano.{sample}.txt")
+        os.path.join(dir_log, "samtools.{sample}.log")
     shell:
         """
-        export CHECKVDB={params.db}
-        if [[ -s {input.contigs} ]] ; then
-            checkv end_to_end\
-                {input.contigs} \
-                {params.out} \
-                -t {threads} \
-                &> {log}
-            touch {output.out}
-        else
-            touch {output.out}
-        fi
-        """
+        #get the contig or contigs name from the csv file, and run samtools 
+        awk -F, 'NR>1 {{print $2}}' {input.csv} > {params.outdir}/phage-genome-contig
+
+        touch {output}
+        
+        #extracting the contigs from the assembly
+        for f in `cat {params.outdir}/phage-genome-contig`; do samtools faidx {input.contigs} "$f" >> {output} ; done 
+        """ 
+
```

### Comparing `sphae-1.4/sphae/workflow/rules/5.components.smk` & `sphae-1.4.1/sphae/workflow/rules/5.components.smk`

 * *Files 23% similar despite different names*

```diff
@@ -1,52 +1,48 @@
 """
 Getting the components from the assembly graph
 """
     
 rule components_megahit:
     input:
-        contigs = os.path.join(dir.megahit, "{sample}-pr", "final.contigs.fa"),
-        path = os.path.join(dir.megahit, "{sample}-pr", "final.fastg"),
-        graph = os.path.join(dir.megahit, "{sample}-pr", "final.fastg"),
+        contigs = os.path.join(dir_megahit, "{sample}-pr", "final.contigs.fa"),
+        path = os.path.join(dir_megahit, "{sample}-pr", "final.fastg"),
+        graph = os.path.join(dir_megahit, "{sample}-pr", "final.fastg"),
     output:
-        os.path.join(dir.megahit, "{sample}-pr", "graph_seq_details_megahit.tsv")
+        os.path.join(dir_megahit, "{sample}-pr", "graph_seq_details_megahit.tsv")
     params:
-        o = os.path.join(dir.megahit, "{sample}-pr"),
+        o = os.path.join(dir_megahit, "{sample}-pr"),
         assembler = 'megahit'
     conda:
-        os.path.join(dir.env, "graph.yaml")
+        os.path.join(dir_env, "graph.yaml")
     log:
-        os.path.join(dir.log, "components_megahit.{sample}.log")
-    benchmark:
-        os.path.join(dir.bench, "components_megahit.{sample}.txt")
+        os.path.join(dir_log, "components_megahit.{sample}.log")
     threads:
-        config.resources.smalljob.cpu
+        config['resources']['smalljob']['cpu']
     resources:
-        mem_mb=config.resources.smalljob.mem,
-        time=config.resources.smalljob.time
+        mem_mb=config['resources']['smalljob']['mem'],
+        time=config['resources']['smalljob']['time']
     script:
-        os.path.join(dir.script, 'components.py')
+        os.path.join(dir_script, 'components.py')
 
 
 rule components_flye_nano:
     input:
-        contigs = os.path.join(dir.flye, "{sample}-sr", "assembly.fasta"),
-        graph = os.path.join(dir.flye, "{sample}-sr", "assembly_graph.gfa"),
-        path = os.path.join(dir.flye, "{sample}-sr", "assembly_info.txt")
+        contigs = os.path.join(dir_flye, "{sample}-sr", "assembly.fasta"),
+        graph = os.path.join(dir_flye, "{sample}-sr", "assembly_graph.gfa"),
+        path = os.path.join(dir_flye, "{sample}-sr", "assembly_info.txt")
     output:
-        os.path.join(dir.flye, "{sample}-sr", "graph_seq_details_flye.tsv"),
+        os.path.join(dir_flye, "{sample}-sr", "graph_seq_details_flye.tsv"),
     params:
-        o = os.path.join(dir.flye, "{sample}-sr"),
+        o = os.path.join(dir_flye, "{sample}-sr"),
         assembler = 'flye'
     log:
-        os.path.join(dir.log, "components_flye_nano.{sample}.log")
-    benchmark:
-        os.path.join(dir.bench, "components_flye_nano.{sample}.txt")
+        os.path.join(dir_log, "components_flye_nano.{sample}.log")
     conda:
-        os.path.join(dir.env, "graph.yaml")
+        os.path.join(dir_env, "graph.yaml")
     threads:
-        config.resources.smalljob.cpu
+        config['resources']['smalljob']['cpu']
     resources:
-        mem_mb=config.resources.smalljob.mem,
-        time=config.resources.smalljob.time
+        mem_mb=config['resources']['smalljob']['mem'],
+        time=config['resources']['smalljob']['time']
     script:
-        os.path.join(dir.script, 'components.py')
+        os.path.join(dir_script, 'components.py')
```

### Comparing `sphae-1.4/sphae/workflow/rules/6.stat_join.smk` & `sphae-1.4.1/sphae/workflow/rules/6.stat_join.smk`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 rule join_assembly_stats_megahit:
     input:
-        viralverify = os.path.join(dir.megahit, "{sample}-pr", "final.contigs_result_table.csv"),
-        comp = os.path.join(dir.megahit, "{sample}-pr", "graph_seq_details_megahit.tsv"),
-        checkv = os.path.join(dir.megahit, "{sample}-pr", "checkv", "quality_summary.tsv")
+        viralverify = os.path.join(dir_megahit, "{sample}-pr", "final.contigs_result_table.csv"),
+        comp = os.path.join(dir_megahit, "{sample}-pr", "graph_seq_details_megahit.tsv"),
+        checkv = os.path.join(dir_megahit, "{sample}-pr", "checkv", "quality_summary.tsv")
     output:
-        csv = os.path.join(dir.assembly, "{sample}-assembly-stats_megahit.csv")
+        csv = os.path.join(dir_assembly, "{sample}-assembly-stats_megahit.csv")
     conda:
-        os.path.join(dir.env, "graph.yaml")
+        os.path.join(dir_env, "graph.yaml")
     script:
-        os.path.join(dir.script, 'joining_stats.py')
+        os.path.join(dir_script, 'joining_stats.py')
 
 
 rule join_assembly_stats_flye:
     input:
-        viralverify = os.path.join(dir.flye, "{sample}-sr", "assembly_result_table.csv"),
-        comp = os.path.join(dir.flye, "{sample}-sr", "graph_seq_details_flye.tsv"),
-        checkv = os.path.join(dir.flye, "{sample}-sr", "checkv", "quality_summary.tsv")
+        viralverify = os.path.join(dir_flye, "{sample}-sr", "assembly_result_table.csv"),
+        comp = os.path.join(dir_flye, "{sample}-sr", "graph_seq_details_flye.tsv"),
+        checkv = os.path.join(dir_flye, "{sample}-sr", "checkv", "quality_summary.tsv")
     output:
-        csv = os.path.join(dir.assembly, "{sample}-assembly-stats_flye.csv")
+        csv = os.path.join(dir_assembly, "{sample}-assembly-stats_flye.csv")
     conda:
-        os.path.join(dir.env, "graph.yaml")
+        os.path.join(dir_env, "graph.yaml")
     script:
-        os.path.join(dir.script, 'joining_stats.py')
+        os.path.join(dir_script, 'joining_stats.py')
```

### Comparing `sphae-1.4/sphae/workflow/rules/7.pharokka.smk` & `sphae-1.4.1/sphae/workflow/rules/7.pharokka.smk`

 * *Files 12% similar despite different names*

```diff
@@ -1,149 +1,139 @@
 """
 Running pharokka for anntoation 
 """
+"""
+Running pharokka for anntoation 
+"""
 rule rename_contigs_megahit:
     input:
-        fin=os.path.join(dir.genome, "{sample}-pr", "{sample}.fasta"),
+        fin=os.path.join(dir_genome, "{sample}-pr", "{sample}.fasta"),
     params:
         s ="{sample}"
     output:
-        out=os.path.join(dir.genome, "{sample}-pr", "{sample}_genome.fasta"),
-        csv=os.path.join(dir.genome, "{sample}-pr", "{sample}_temp.csv")
+        out=os.path.join(dir_genome, "{sample}-pr", "{sample}_genome.fasta"),
+        csv=os.path.join(dir_genome, "{sample}-pr", "{sample}_temp.csv")
     localrule: True
     log:
-        os.path.join(dir.log, "rename-contigs.{sample}.log")
+        os.path.join(dir_log, "rename-contigs.{sample}.log")
     script:
-        os.path.join(dir.script, 'rename_genomes.py')
-
+        os.path.join(dir_script, 'rename_genomes.py')
 
 rule pharokka_megahit:
     """Annotate genomes with Pharokka"""
     input:
-        os.path.join(dir.genome, "{sample}-pr", "{sample}_genome.fasta"),
+        os.path.join(dir_genome, "{sample}-pr", "{sample}_genome.fasta"),
     params:
-        o=os.path.join(dir.pharokka, "{sample}-pr"),
-        db=os.path.join(dir.db, "pharokka_db"),
+        o=os.path.join(dir_pharokka, "{sample}-pharokka"),
+        db=os.path.join(dir_db, "pharokka_db"),
         sp="{sample}"
     output:
-        gbk=os.path.join(dir.pharokka, "{sample}-pr", "{sample}.gbk"),
-        plot=os.path.join(dir.pharokka, "{sample}-pr", "{sample}_pharokka_plot.png"),
-        card=os.path.join(dir.pharokka, "{sample}-pr", "top_hits_card.tsv"),
-        vfdb=os.path.join(dir.pharokka, "{sample}-pr", "top_hits_vfdb.tsv"),
-        spacers=os.path.join(dir.pharokka, "{sample}-pr", "{sample}_minced_spacers.txt"),
-        taxa=os.path.join(dir.pharokka, "{sample}-pr", "{sample}_top_hits_mash_inphared.tsv"),
-        cdden=os.path.join(dir.pharokka, "{sample}-pr", "{sample}_length_gc_cds_density.tsv"),
-        cds=os.path.join(dir.pharokka, "{sample}-pr", "{sample}_cds_functions.tsv")
+        gbk=os.path.join(dir_pharokka, "{sample}-pharokka", "{sample}.gbk"),
+        card=os.path.join(dir_pharokka, "{sample}-pharokka", "top_hits_card.tsv"),
+        vfdb=os.path.join(dir_pharokka, "{sample}-pharokka", "top_hits_vfdb.tsv"),
+        spacers=os.path.join(dir_pharokka, "{sample}-pharokka", "{sample}_minced_spacers.txt"),
+        taxa=os.path.join(dir_pharokka, "{sample}-pharokka", "{sample}_top_hits_mash_inphared.tsv"),
+        cdden=os.path.join(dir_pharokka, "{sample}-pharokka", "{sample}_length_gc_cds_density.tsv"),
+        cds=os.path.join(dir_pharokka, "{sample}-pharokka", "{sample}_cds_functions.tsv")
     conda:
-        os.path.join(dir.env, "pharokka.yaml")
+        os.path.join(dir_env, "pharokka.yaml")
     threads:
-        config.resources.smalljob.cpu
+        config['resources']['smalljob']['cpu']
     resources:
-        mem_mb = config.resources.smalljob.mem,
-        time = config.resources.smalljob.time
+        mem_mb = config['resources']['smalljob']['mem'],
+        time = config['resources']['smalljob']['time']
     log:
-        os.path.join(dir.log, "pharokka.{sample}.log")
-    benchmark:
-        os.path.join(dir.bench,"pharokka_megahit_{sample}.txt")
+        os.path.join(dir_log, "pharokka.{sample}.log")
     shell:
         """
         if [[ -s {input} ]] ; then
             pharokka.py \
                 -i {input} \
                 -o {params.o} \
                 -d {params.db} \
                 -t {threads} \
                 -f -p {params.sp}\
                 2> {log}
-            pharokka_plotter.py -i {input} -n {params.sp}_pharokka_plot -o {params.o} -p {params.sp} -f
             touch {output.gbk}
-            touch {output.plot}
             touch {output.card}
             touch {output.vfdb}
             touch {output.spacers}
             touch {output.taxa}
             touch {output.cdden}
             touch {output.cds}
         else
             touch {output.gbk}
-            touch {output.plot}
             touch {output.card}
             touch {output.vfdb}
             touch {output.spacers}
             touch {output.taxa}
             touch {output.cdden}
             touch {output.cds}
         fi
         """
 
 rule rename_contigs_flye:
     input:
-        fin=os.path.join(dir.genome, "{sample}-sr", "{sample}.fasta"),
+        fin=os.path.join(dir_genome, "{sample}-sr", "{sample}.fasta"),
     params:
         s ="{sample}"
     output:
-        out=os.path.join(dir.genome, "{sample}-sr", "{sample}_genome.fasta"),
-        csv=os.path.join(dir.genome, "{sample}-sr", "{sample}_temp.csv")
+        out=os.path.join(dir_genome, "{sample}-sr", "{sample}_genome.fasta"),
+        csv=os.path.join(dir_genome, "{sample}-sr", "{sample}_temp.csv")
     localrule: True
     log:
-        os.path.join(dir.log, "rename-contigs.{sample}.log")
+        os.path.join(dir_log, "rename-contigs.{sample}.log")
     script:
-        os.path.join(dir.script, 'rename_genomes.py')
+        os.path.join(dir_script, 'rename_genomes.py')
 
 rule pharokka_flye:
     """Annotate genomes with Pharokka"""
     input:
-        os.path.join(dir.genome, "{sample}-sr", "{sample}_genome.fasta")
+        os.path.join(dir_genome, "{sample}-sr", "{sample}_genome.fasta")
     params:
-        o=os.path.join(dir.pharokka, "{sample}-sr"),
-        db=os.path.join(dir.db, "pharokka_db"),
+        o=os.path.join(dir_pharokka, "{sample}-pharokka"),
+        db=os.path.join(dir_db, "pharokka_db"),
         sp="{sample}"
     output:
-        gbk=os.path.join(dir.pharokka, "{sample}-sr", "{sample}.gbk"),
-        plot=os.path.join(dir.pharokka, "{sample}-sr", "{sample}_pharokka_plot.png"),
-        card=os.path.join(dir.pharokka, "{sample}-sr", "top_hits_card.tsv"),
-        vfdb=os.path.join(dir.pharokka, "{sample}-sr", "top_hits_vfdb.tsv"),
-        spacers=os.path.join(dir.pharokka, "{sample}-sr", "{sample}_minced_spacers.txt"),
-        taxa=os.path.join(dir.pharokka, "{sample}-sr", "{sample}_top_hits_mash_inphared.tsv"),
-        cdden=os.path.join(dir.pharokka, "{sample}-sr", "{sample}_length_gc_cds_density.tsv"),
-        cds=os.path.join(dir.pharokka, "{sample}-sr", "{sample}_cds_functions.tsv")
+        gbk=os.path.join(dir_pharokka, "{sample}-pharokka", "{sample}.gbk"),
+        card=os.path.join(dir_pharokka, "{sample}-pharokka", "top_hits_card.tsv"),
+        vfdb=os.path.join(dir_pharokka, "{sample}-pharokka", "top_hits_vfdb.tsv"),
+        spacers=os.path.join(dir_pharokka, "{sample}-pharokka", "{sample}_minced_spacers.txt"),
+        taxa=os.path.join(dir_pharokka, "{sample}-pharokka", "{sample}_top_hits_mash_inphared.tsv"),
+        cdden=os.path.join(dir_pharokka, "{sample}-pharokka", "{sample}_length_gc_cds_density.tsv"),
+        cds=os.path.join(dir_pharokka, "{sample}-pharokka", "{sample}_cds_functions.tsv")
     conda:
-        os.path.join(dir.env, "pharokka.yaml")
+        os.path.join(dir_env, "pharokka.yaml")
     threads:
-        config.resources.smalljob.cpu
+        config['resources']['smalljob']['cpu']
     resources:
-        mem_mb = config.resources.smalljob.mem,
-        time = config.resources.smalljob.time
+        mem_mb = config['resources']['smalljob']['mem'],
+        time = config['resources']['smalljob']['time']
     log:
-        os.path.join(dir.log, "pharokka.{sample}.log")
-    benchmark:
-        os.path.join(dir.bench,"pharokka_flye_{sample}.txt")
+        os.path.join(dir_log, "pharokka.{sample}.log")
     shell:
         """
         if [[ -s {input} ]] ; then
             pharokka.py \
                 -i {input} \
                 -o {params.o} \
                 -d {params.db} \
                 -t {threads} \
                 -f -p {params.sp}\
                 2> {log}
 
-            pharokka_plotter.py -i {input} -n {params.sp}_pharokka_plot -o {params.o} -p {params.sp} -f
             touch {output.gbk}
-            touch {output.plot}
             touch {output.card}
             touch {output.vfdb}
             touch {output.spacers}
             touch {output.taxa}
             touch {output.cdden}
             touch {output.cds}
         else
             touch {output.gbk}
-            touch {output.plot}
             touch {output.card}
             touch {output.vfdb}
             touch {output.spacers}
             touch {output.taxa}
             touch {output.cdden}
             touch {output.cds}
         fi
```

### Comparing `sphae-1.4/sphae/workflow/rules/8.phold.smk` & `sphae-1.4.1/sphae/workflow/rules/8.phold.smk`

 * *Files 22% similar despite different names*

```diff
@@ -1,65 +1,69 @@
 """
 Running Phold to improve the anntoation 
 https://github.com/gbouras13/phold
 """
 rule phold_run_paired:
     input:
-        gbk=os.path.join(dir.pharokka, "{sample}-pr", "{sample}.gbk")
+        gbk=os.path.join(dir_pharokka, "{sample}-pharokka", "{sample}.gbk")
     params:
-        predict=os.path.join(dir.pharokka,"{sample}-pr-predict"),
-        o=os.path.join(dir.pharokka,"{sample}-pr-phold"),
+        predict=os.path.join(dir_pharokka,"{sample}-pr-predict"),
+        o=os.path.join(dir_pharokka,"{sample}-pr-phold"),
         prefix="{sample}",
-        db=os.path.join(dir.db, "phold")
+        db=os.path.join(dir_db, "phold")
     output:
-        gbk=os.path.join(dir.pharokka,"{sample}-pr-phold","{sample}.gbk")
+        gbk=os.path.join(dir_pharokka,"{sample}-pr-phold","{sample}.gbk"),
+        acr=os.path.join(dir_pharokka,"{sample}-pr-phold","sub_db_tophits", "acr_cds_predictions.tsv"),
+        card=os.path.join(dir_pharokka,"{sample}-pr-phold","sub_db_tophits", "card_cds_predictions.tsv"),
+        defense=os.path.join(dir_pharokka,"{sample}-pr-phold","sub_db_tophits", "defensefinder_cds_predictions.tsv"),
+        vfdb=os.path.join(dir_pharokka,"{sample}-pr-phold","sub_db_tophits", "vfdb_cds_predictions.tsv")
     threads: 
-        config.resources.smalljob.cpu
+        config['resources']['smalljob']['cpu']
     conda:
-        os.path.join(dir.env, "phold.yaml")
+        os.path.join(dir_env, "phold.yaml")
     resources:
-        mem_mb = config.resources.smalljob.mem,
-        time = config.resources.smalljob.time
+        mem_mb = config['resources']['smalljob']['mem'],
+        time = config['resources']['smalljob']['time']
     log:
-        os.path.join(dir.log, "phold.{sample}.log")
-    benchmark:
-        os.path.join(dir.bench,"phold_megahit_{sample}.txt")
+        os.path.join(dir_log, "phold.{sample}.log")
     shell:
         """
         if [[ -s {input.gbk} ]] ; then
-            phold predict -i {input.gbk} -o {params.predict} -p {params.prefix} -t {threads} --cpu -d {params.db} -f
-            phold compare -i {input.gbk} --predictions_dir {params.predict} -p {params.prefix} -o {params.o} -t {threads} -d {params.db} -f
+            phold predict -i {input.gbk} -o {params.predict} -p {params.prefix} -t {threads} --cpu -d {params.db} -f 2> {log}
+            phold compare -i {input.gbk} --predictions_dir {params.predict} -p {params.prefix} -o {params.o} -t {threads} -d {params.db} -f 2> {log}
         else
             touch {output.gbk}
         fi
         """
 
 rule phold_run_longreads:
     input:
-        gbk=os.path.join(dir.pharokka, "{sample}-sr", "{sample}.gbk")
+        gbk=os.path.join(dir_pharokka, "{sample}-pharokka", "{sample}.gbk")
     params:
-        predict=os.path.join(dir.pharokka,"{sample}-sr-predict"),
-        o=os.path.join(dir.pharokka,"{sample}-sr-phold"),
+        predict=os.path.join(dir_pharokka,"{sample}-sr-predict"),
+        o=os.path.join(dir_pharokka,"{sample}-sr-phold"),
         prefix="{sample}",
-        db=os.path.join(dir.db, "phold")
+        db=os.path.join(dir_db, "phold")
     output:
-        gbk=os.path.join(dir.pharokka,"{sample}-sr-phold","{sample}.gbk"),
+        gbk=os.path.join(dir_pharokka,"{sample}-sr-phold","{sample}.gbk"),
+        acr=os.path.join(dir_pharokka,"{sample}-sr-phold","sub_db_tophits", "acr_cds_predictions.tsv"),
+        card=os.path.join(dir_pharokka,"{sample}-sr-phold","sub_db_tophits", "card_cds_predictions.tsv"),
+        defense=os.path.join(dir_pharokka,"{sample}-sr-phold","sub_db_tophits", "defensefinder_cds_predictions.tsv"),
+        vfdb=os.path.join(dir_pharokka,"{sample}-sr-phold","sub_db_tophits", "vfdb_cds_predictions.tsv")
     threads: 
-        config.resources.smalljob.cpu
+        config['resources']['smalljob']['cpu']
     conda:
-        os.path.join(dir.env, "phold.yaml")
+        os.path.join(dir_env, "phold.yaml")
     resources:
-        mem_mb = config.resources.smalljob.mem,
-        time = config.resources.smalljob.time
+        mem_mb = config['resources']['smalljob']['mem'],
+        time = config['resources']['smalljob']['time']
     log:
-        os.path.join(dir.log, "phold.{sample}.log")
-    benchmark:
-        os.path.join(dir.bench,"phold_flye_{sample}.txt")
+        os.path.join(dir_log, "phold.{sample}.log")
     shell:
         """
         if [[ -s {input.gbk} ]] ; then
-            phold predict -i {input.gbk} -o {params.predict} -p {params.prefix} -t {threads} --cpu -d {params.db} -f
-            phold compare -i {input.gbk} --predictions_dir {params.predict} -p {params.prefix} -o {params.o} -t {threads} -d {params.db} -f
+            phold predict -i {input.gbk} -o {params.predict} -p {params.prefix} -t {threads} --cpu -d {params.db} -f 2> {log}
+            phold compare -i {input.gbk} --predictions_dir {params.predict} -p {params.prefix} -o {params.o} -t {threads} -d {params.db} -f 2> {log}
         else
             touch {output.gbk}
         fi
-        """
+        """
```

### Comparing `sphae-1.4/sphae/workflow/scripts/components.py` & `sphae-1.4.1/sphae/workflow/scripts/components.py`

 * *Files identical despite different names*

### Comparing `sphae-1.4/sphae/workflow/scripts/fastg2gfa` & `sphae-1.4.1/sphae/workflow/scripts/fastg2gfa`

 * *Files identical despite different names*

### Comparing `sphae-1.4/sphae/workflow/scripts/graph_utils/build_utils.py` & `sphae-1.4.1/sphae/workflow/scripts/graph_utils/build_utils.py`

 * *Files identical despite different names*

### Comparing `sphae-1.4/sphae/workflow/scripts/joining_stats.py` & `sphae-1.4.1/sphae/workflow/scripts/joining_stats.py`

 * *Files identical despite different names*

### Comparing `sphae-1.4/sphae/workflow/scripts/pick_phage_contigs.py` & `sphae-1.4.1/sphae/workflow/scripts/pick_phage_contigs.py`

 * *Files identical despite different names*

### Comparing `sphae-1.4/sphae/workflow/scripts/rename_genomes.py` & `sphae-1.4.1/sphae/workflow/scripts/rename_genomes.py`

 * *Files identical despite different names*

### Comparing `sphae-1.4/sphae/workflow/scripts/roblib/__init__.py` & `sphae-1.4.1/sphae/workflow/scripts/roblib/__init__.py`

 * *Files identical despite different names*

### Comparing `sphae-1.4/sphae/workflow/scripts/roblib/alignments.py` & `sphae-1.4.1/sphae/workflow/scripts/roblib/alignments.py`

 * *Files identical despite different names*

### Comparing `sphae-1.4/sphae/workflow/scripts/roblib/bcolors.py` & `sphae-1.4.1/sphae/workflow/scripts/roblib/bcolors.py`

 * *Files identical despite different names*

### Comparing `sphae-1.4/sphae/workflow/scripts/roblib/blast.py` & `sphae-1.4.1/sphae/workflow/scripts/roblib/blast.py`

 * *Files identical despite different names*

### Comparing `sphae-1.4/sphae/workflow/scripts/roblib/colours.py` & `sphae-1.4.1/sphae/workflow/scripts/roblib/colours.py`

 * *Files identical despite different names*

### Comparing `sphae-1.4/sphae/workflow/scripts/roblib/date_parsing.py` & `sphae-1.4.1/sphae/workflow/scripts/roblib/date_parsing.py`

 * *Files identical despite different names*

### Comparing `sphae-1.4/sphae/workflow/scripts/roblib/dna.py` & `sphae-1.4.1/sphae/workflow/scripts/roblib/dna.py`

 * *Files identical despite different names*

### Comparing `sphae-1.4/sphae/workflow/scripts/roblib/dnadist.py` & `sphae-1.4.1/sphae/workflow/scripts/roblib/dnadist.py`

 * *Files identical despite different names*

### Comparing `sphae-1.4/sphae/workflow/scripts/roblib/file_chooser.py` & `sphae-1.4.1/sphae/workflow/scripts/roblib/file_chooser.py`

 * *Files identical despite different names*

### Comparing `sphae-1.4/sphae/workflow/scripts/roblib/functions.py` & `sphae-1.4.1/sphae/workflow/scripts/roblib/functions.py`

 * *Files identical despite different names*

### Comparing `sphae-1.4/sphae/workflow/scripts/roblib/genbank.py` & `sphae-1.4.1/sphae/workflow/scripts/roblib/genbank.py`

 * *Files identical despite different names*

### Comparing `sphae-1.4/sphae/workflow/scripts/roblib/geography.py` & `sphae-1.4.1/sphae/workflow/scripts/roblib/geography.py`

 * *Files identical despite different names*

### Comparing `sphae-1.4/sphae/workflow/scripts/roblib/newick.py` & `sphae-1.4.1/sphae/workflow/scripts/roblib/newick.py`

 * *Files identical despite different names*

### Comparing `sphae-1.4/sphae/workflow/scripts/roblib/rob_error.py` & `sphae-1.4.1/sphae/workflow/scripts/roblib/rob_error.py`

 * *Files identical despite different names*

### Comparing `sphae-1.4/sphae/workflow/scripts/roblib/seqio_filter.py` & `sphae-1.4.1/sphae/workflow/scripts/roblib/seqio_filter.py`

 * *Files identical despite different names*

### Comparing `sphae-1.4/sphae/workflow/scripts/roblib/sequences.py` & `sphae-1.4.1/sphae/workflow/scripts/roblib/sequences.py`

 * *Files identical despite different names*

### Comparing `sphae-1.4/sphae/workflow/scripts/roblib/stats.py` & `sphae-1.4.1/sphae/workflow/scripts/roblib/stats.py`

 * *Files identical despite different names*

### Comparing `sphae-1.4/sphae/workflow/scripts/roblib/translate.py` & `sphae-1.4.1/sphae/workflow/scripts/roblib/translate.py`

 * *Files identical despite different names*

### Comparing `sphae-1.4/sphae/workflow/scripts/summary.py` & `sphae-1.4.1/sphae/workflow/scripts/summary.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,29 +64,38 @@
                         summary.write("No recombinase\n")
                     else: 
                         summary.write("Recombinases found in genome\n")
                     if 'transposase' not in open(input_files['gbk']).read().lower():
                         summary.write("No transposase\n")
                     else: 
                         summary.write("Transposases found in genome\n")
-                
-                if len(open(input_files['amr']).readlines()) == 1:
-                    summary.write("No AMR genes\n")
+                #AMR genes 
+                if (len(open(input_files['amr']).readlines()) == 1) and (len(open(input_files['card']).readlines()) == 0):
+                    summary.write("No AMR genes found\n")
                 else:
-                    summary.write("AMR genes found\n")
+                    summary.write("AMR genes found\n")                
 
-                if len(open(input_files['vfdb']).readlines()) == 1:
+                #Virulence genes 
+                if (len(open(input_files['vfdb']).readlines()) == 1) and (len(open(input_files['vfdb_phold']).readlines()) == 0):
                     summary.write("No virulence factor genes\n")
                 else:
-                    summary.write("Virulence factor genes found\n")
+                    summary.write("Virulence genes found\n")
 
-                if len(open(input_files['spacers']).readlines()) > 2:
+                #CRISPR spacers 
+                if (len(open(input_files['spacers']).readlines()) == 0) and (len(open(input_files['acr']).readlines()) == 0):
+                    summary.write("No CRISPR spacers found\n")
+                else:
                     summary.write("CRISPR spacers found\n")
+                
+                #Defense finder genes  
+                if (len(open(input_files['defense']).readlines()) == 0):
+                    summary.write("No Defense genes found\n")
                 else:
-                    summary.write("No CRISPR spacers found\n")
+                    summary.write("Defense genes found\n")
+                
             else:
                 summary.write("Genome includes multiple contigs, fragmented\n")
         else:
             summary.write("No contigs from the assembly were assigned viral, likely contigs too short in size\n")
 
 
 def analyze_assembly(input_files, output_summary, params):
@@ -114,20 +123,24 @@
 # Replace input_files and output_params with the actual paths to your input/output files and parameters
 input_files = {
         'assembly': snakemake.input.assembly,
         'table': snakemake.input.table,
         'genome': snakemake.input.genome,
         'gbk': snakemake.input.gbk,
         'plot': snakemake.input.plot,
+        'taxa': snakemake.input.ph_taxa,
+        'cdden': snakemake.input.cdden,
+        'cds': snakemake.input.cds,
         'amr': snakemake.input.amr,
         'vfdb': snakemake.input.vfdb,
         'spacers': snakemake.input.spacers,
-        'taxa': snakemake.input.ph_taxa,
-        'cdden': snakemake.input.cdden,
-        'cds': snakemake.input.cds
+        'acr': snakemake.input.acr,
+        'card': snakemake.input.card,
+        'defense': snakemake.input.defense,
+        'vfdb_phold': snakemake.input.vfdb_phold,
 }
 
 output_summary = snakemake.output.summary
 
 params = {
     'sample' : snakemake.params.sample,
     'genomes': snakemake.params.genomes,
```

### Comparing `sphae-1.4/sphae.egg-info/PKG-INFO` & `sphae-1.4.1/sphae.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphae
-Version: 1.4
+Version: 1.4.1
 Summary: Assembling pure culture phages from both Illumina and Nanopore sequencing technology
 Home-page: https://github.com/linsalrob/sphae
 Author: Bhavya Papudeshi
 Author-email: npbhavya13@gmail.com
 License: The MIT License (MIT)
 Keywords: phage 'phage therapy' bioinformatics microbiology bacteria genome genomics
 Platform: any
@@ -40,36 +40,34 @@
 ## Phage toolkit to detect phage candidates for phage therapy
 <p align="center">
   <img src="sphae.png#gh-light-mode-only" width="300">
   <img src="sphaedark.png#gh-dark-mode-only" width="300">
 </p>
 
 
-
 **Overview**
 
 This snakemake workflow was built using Snaketool [https://doi.org/10.1371/journal.pcbi.1010705], to assemble and annotate phage sequences. Currently, this tool is being developed for phage genomes. The steps include,
 
 - Quality control that removes adaptor sequences, low-quality reads and host contamination (optional). 
 - Assembly
 - Contig quality checks; read coverage, viral or not, completeness, and assembly graph components. 
-- Phage genome annotation'
-- Annotation of the phage genome 
+- Phage genome annotation
   
-A complete list of programs used for each step is mentioned in the sphae.CITATION file. 
+A complete list of programs used for each step is mentioned in the `sphae.CITATION` file. 
 
 ### Install 
 
 **Pip install**
 
 ```bash
 pip install sphae
 ```
 
-** conda install** 
+**Conda install** 
 ```bash
 conda install sphae
 ```
 **Source Install**
 
 Setting up a new conda environment 
 
@@ -92,29 +90,34 @@
 pip install -e .
 
 #confirm the workflow is installed by running the below command 
 sphae --help
 ```
 
 ## Installing databases
-Run command,
+Run the below command,
 
-```
+```bash
+#Installs the database to default directory, `sphae/workflow/databases`
 sphae install
+
+#Install database to specific directory
+sphae install --db-dir <directory> 
 ```
 
   Install the databases to a directory, `sphae/workflow/databases`
 
   This workflow requires the 
   - Pfam35.0 database to run viral_verify for contig classification. 
   - CheckV database to test for phage completeness
   - Pharokka databases 
   - Phynteny models
+  - Phold databases
 
-This step takes approximately 1hr 30min to install and requires 9G of storage
+This step requires ~17G of storage
 
 ## Running the workflow
 
 The command `sphae run` will run QC, assembly and annotation
 
 **Commands to run**
 
@@ -125,15 +128,22 @@
 sphae run --input tests/data/illumina-subset --output example -k 
 
 #For nanopore reads, place the reads, one file per sample in a directory
 sphae run --input tests/data/nanopore-subset --sequencing longread --output example -k
 
 #To run either of the commands on the cluster, add --profile slurm to the command. For instance here is the command for longreads/nanopore reads 
 #Before running this below command, make sure have slurm config files setup, here is a tutorial, https://fame.flinders.edu.au/blog/2021/08/02/snakemake-profiles-updated 
-sphae run --input tests/data/nanopore-subset --preprocess longread --output example --profile slurm -k
+sphae run --input tests/data/nanopore-subset --preprocess longread --output example --profile slurm -k --threads 16
+```
+
+**Command to run only annotation steps**
+
+```bash
+#the genomes directory has the already assembled complete genomes
+sphae annotate --genome <genomes directory> --output example -k 
 ```
 
 **Output**
 
 Output is saved to `example/RESULTS` directory. In this directory, there will be four files 
   - Genome annotations in GenBank format (Phynteny output)
   - Genome in fasta format (either the reoriented to terminase output from Pharokka, or assembled viral contigs)
@@ -147,22 +157,19 @@
   - If the assembled contig is circular or not (From the assembly graph)
   - Completeness (calculated from CheckV)
   - Contamination (calculated from CheckV)
   - Taxonomy accession ID (Pharokka output, searches the genome against INPHARED database using mash)
   - Taxa mash includes the number of matching hashes of the assembled genome to the accession ID/Taxa name. Higher the matching hash- more likely the genome is related to the taxa predicted
   - Gene searches:
     - Whether integrase is found (search for integrase gene in annotations)
-    - Whether anti-microbial genes were found (Pharokka search against AMR database)
+    - Whether anti-microbial genes were found (Phold and Pharokka search against AMR database)
     - Whether any virulence factors were found (Pharokka search against virulence gene database)
     - Whether any CRISPR spacers were found (Pharokka search against MinCED database) 
- 
 
 ### FAQ
-- Sure, here are the clarifications for each scenario:
-
 1. **"Failed during assembly":**
    - This message indicates that the assembly process was unsuccessful. It suggests that the assembler could not generate contigs, which are contiguous sequences of DNA, typically representing segments of a genome. 
    - To confirm this, you can check the logs located at `sphae.out/PROCESSING/assembly/flye/<sample name>/assembly_info.txt` or `sphae.out/PROCESSING/assembly/megahit/<sample name>/log`. These logs should provide details about the error or the step at which the assembly failed.
    - One possible reason for this failure could be insufficient genome coverage, meaning that there were not enough sequencing reads to accurately assemble the genome.
 
 2. **"Genome includes multiple contigs, fragmented":**
    - This message indicates that the assembly generated numerous short fragments (contigs) instead of a single, contiguous sequence representing a nearly complete phage genome. 
@@ -177,26 +184,34 @@
      subsample:
          --bases 1000M
      ```
    - Increase or decrease the number of bases (e.g., `1000M` for 1000 megabases) based on your requirements.
    - After making the changes, rerun sphae and ensure that the updated subsampling parameters are reflected in the `sphae.out/sphae.config.yaml` file.
 
 4. **"What does 'No integrases found ...but Phynteny predicted a few unknown function genes to have some similarity with integrase genes but with low confidence. Maybe a false positive or a novel integrase gene' mean?"**
-  This message indicates that while no integrase genes were explicitly identified, the analysis detected certain genes that exhibited similarities to integrase genes. However, these genes were associated with low confidence scores, suggesting a possibility of being false positives or potentially representing novel integrase genes.
-
-  [Phynteny](https://github.com/susiegriggo/Phynteny), the tool used for this prediction, assigns a confidence score to each gene prediction. If this score falls below a certain threshold (typically 90%), the gene remains classified as having an unknown function. To further investigate these genes, advanced techniques such as folding using tools like [ColabFold](https://github.com/sokrypton/ColabFold) can be employed. Analyzing the structure of these genes may provide additional insights into their functionality and potential role in biological processes.
-
-5. **How do I visualize the phages and gene annotations?**
+   This message indicates that while no integrase genes were explicitly identified, the analysis detected certain genes that exhibited similarities to integrase genes. However, these genes were associated with low confidence scores, suggesting a possibility of being false positives or potentially representing novel integrase genes.
+   
+   [Phynteny](https://github.com/susiegriggo/Phynteny), the tool used for this prediction, assigns a confidence score to each gene prediction. If this score falls below a certain threshold (typically 90%), the gene remains classified as having an unknown function. To further investigate these genes, advanced techniques such as folding using tools like [ColabFold](https://github.com/sokrypton/ColabFold) and [Foldseek](https://github.com/steineggerlab/foldseek) can be employed. Analyzing the structure of these genes may provide additional insights into their functionality and potential role in biological processes.
+
+1. **How do I visualize the phages and gene annotations?**
+   To visualize the phages and gene annotations, I recommend using [Clinker](https://github.com/gamcil/clinker). First, gather all the sample genbank files from `sphae.out/RESULTS` and place them in a new directory. Then, execute the clinker command to generate clinker plots, which compare the genes in each genome to each other.
+   
+   Additionally, for enhanced visualization, consider running [dnaapler](https://github.com/gbouras13/dnaapler) on the genomes in fasta format obtained from 
+   `sphae.out/RESULTS`. This step generates reoriented phages that start with terminase genes. Pharokka -> Phold -> Phynteny has to be rerun, and the resulting genbank files can be used for visualization. To perform the annotation steps, run the command 
+   `sphae annotate --input <reoriented genomes from dnaapler in fasta format directory>`
+   
+   Please note that dnaapler may fail if terminase genes are not found, particularly when working with novel phages. The reason these steps haven't been added to sphae. If you encounter any challenges during this process, please feel free to leave an issue, and I'll provide improved documentation to assist you further with the command on how to install and run the command different commands. 
 
-  To visualize the phages and gene annotations, I recommend using [Clinker](https://github.com/gamcil/clinker). First, gather all the sample genbank files from `sphae.out/RESULTS` and place them in a new directory. Then, execute the clinker command to generate clinker plots, which compare the genes in each genome to each other.
-
-  Additionally, for enhanced visualization, consider running [dnaapler](https://github.com/gbouras13/dnaapler) on the genomes in fasta format obtained from `sphae.out/RESULTS`. This step generates reoriented phages that start with terminase genes. Pharokka has been rerun, and the resulting genbank files can be used for visualization. 
+2. **Where are the intermediate files being saved?**
+   These files are being saved in `sphae.out/PROCESSING`. If you need more information on the file structure here, or have ideas of better organization then leave an issue and I will make a note to have more documentation. 
 
-  Please note that dnaapler may fail if terminase genes are not found, particularly when working with novel phages. The reason these steps haven't been added to sphae. If you encounter any challenges during this process, please feel free to leave an issue, and I'll provide improved documentation to assist you further with the command on how to install and run the command different commands. 
+3. **Just run annotation on already assembled genomes?**
+   
+    `sphae annotate --input <input genomes>`
+    This command runs only Pharokka, Phold and Phynteny to annotate the assembled genomes. The results are saved to a new directory labeled `sphae.out/annotation`. 
 
-6. **Where are the intermediate files being saved?**
-   These files are being saved in `sphae.out/PROCESSING`. If you need more information on the file structure here, or have ideas of better organization then leave an issue and I will make a note to have more documentation. 
+    Note: Currently, Sphae runs Phold in CPU mode, but efforts are underway to support Phold GPU mode for faster processing of this step.
 
 ## Issues and Questions
 
-This is still a work in progress, so if you come across any issues or errors, report them under Issues. 
+If you come across any issues or errors, report them under [Issues](https://github.com/linsalrob/sphae/issues).
```

### Comparing `sphae-1.4/sphae.egg-info/SOURCES.txt` & `sphae-1.4.1/sphae.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -11,46 +11,51 @@
 sphae.egg-info/SOURCES.txt
 sphae.egg-info/dependency_links.txt
 sphae.egg-info/entry_points.txt
 sphae.egg-info/requires.txt
 sphae.egg-info/top_level.txt
 sphae/config/config.yaml
 sphae/workflow/Snakefile
+sphae/workflow/Snakefile-annot
 sphae/workflow/install.smk
 sphae/workflow/envs/checkv.yaml
 sphae/workflow/envs/flye.yaml
 sphae/workflow/envs/graph.yaml
 sphae/workflow/envs/medaka.yaml
 sphae/workflow/envs/megahit.yaml
 sphae/workflow/envs/pharokka.yaml
 sphae/workflow/envs/phold.yaml
 sphae/workflow/envs/phynteny.yaml
+sphae/workflow/envs/qc.yaml
 sphae/workflow/envs/samtools.yaml
-sphae/workflow/envs/trimnami.yaml
 sphae/workflow/envs/viralverify.yaml
-sphae/workflow/rules/1.preflight-database.smk
+sphae/workflow/rules/1.preflight-annot.smk
 sphae/workflow/rules/1.preflight.smk
 sphae/workflow/rules/10.final-reporting.smk
+sphae/workflow/rules/2.targets-annot.smk
 sphae/workflow/rules/2.targets.smk
 sphae/workflow/rules/3.qc_qa.smk
 sphae/workflow/rules/4.assembly.smk
 sphae/workflow/rules/5.checkv.smk
 sphae/workflow/rules/5.components.smk
 sphae/workflow/rules/5.viralverify.smk
 sphae/workflow/rules/6.phage_genome.smk
 sphae/workflow/rules/6.stat_join.smk
 sphae/workflow/rules/7.pharokka.smk
+sphae/workflow/rules/789.annot.smk
 sphae/workflow/rules/8.phold.smk
 sphae/workflow/rules/9.phynteny.smk
 sphae/workflow/scripts/components.py
 sphae/workflow/scripts/fastg2gfa
 sphae/workflow/scripts/joining_stats.py
 sphae/workflow/scripts/pick_phage_contigs.py
 sphae/workflow/scripts/rename_genomes.py
+sphae/workflow/scripts/summary-annot.py
 sphae/workflow/scripts/summary.py
+sphae/workflow/scripts/summary_functions.py
 sphae/workflow/scripts/graph_utils/build_utils.py
 sphae/workflow/scripts/roblib/__init__.py
 sphae/workflow/scripts/roblib/alignments.py
 sphae/workflow/scripts/roblib/bcolors.py
 sphae/workflow/scripts/roblib/blast.py
 sphae/workflow/scripts/roblib/colours.py
 sphae/workflow/scripts/roblib/date_parsing.py
```

### Comparing `sphae-1.4/tests/test_sphae.py` & `sphae-1.4.1/tests/test_sphae.py`

 * *Files identical despite different names*

