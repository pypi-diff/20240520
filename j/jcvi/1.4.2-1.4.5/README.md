# Comparing `tmp/jcvi-1.4.2.tar.gz` & `tmp/jcvi-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcvi-1.4.2.tar", last modified: Fri Mar  1 06:50:26 2024, max compression
+gzip compressed data, was "jcvi-1.4.5.tar", last modified: Mon Apr 29 06:37:24 2024, max compression
```

## Comparing `jcvi-1.4.2.tar` & `jcvi-1.4.5.tar`

### file list

```diff
@@ -1,215 +1,208 @@
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-03-01 06:50:26.997631 jcvi-1.4.2/
--rw-r--r--   0 bao        (501) staff       (20)     1292 2020-03-03 07:11:04.000000 jcvi-1.4.2/LICENSE
--rw-r--r--   0 bao        (501) staff       (20)       91 2022-11-27 15:24:30.000000 jcvi-1.4.2/MANIFEST.in
--rw-r--r--   0 bao        (501) staff       (20)     9485 2024-03-01 06:50:26.997455 jcvi-1.4.2/PKG-INFO
--rw-r--r--   0 bao        (501) staff       (20)     8250 2023-07-25 21:30:23.000000 jcvi-1.4.2/README.md
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-03-01 06:50:26.962449 jcvi-1.4.2/jcvi/
--rw-r--r--   0 bao        (501) staff       (20)      770 2022-11-26 21:23:29.000000 jcvi-1.4.2/jcvi/__init__.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-03-01 06:50:26.965337 jcvi-1.4.2/jcvi/algorithms/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/algorithms/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      263 2021-06-19 08:23:09.000000 jcvi-1.4.2/jcvi/algorithms/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)     6422 2021-06-19 08:23:09.000000 jcvi-1.4.2/jcvi/algorithms/ec.py
--rw-r--r--   0 bao        (501) staff       (20)     5678 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/algorithms/formula.py
--rw-r--r--   0 bao        (501) staff       (20)    14132 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/algorithms/graph.py
--rwxr-xr-x   0 bao        (501) staff       (20)     6275 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/algorithms/lis.py
--rwxr-xr-x   0 bao        (501) staff       (20)    24228 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/algorithms/lpsolve.py
--rw-r--r--   0 bao        (501) staff       (20)     6104 2021-06-19 08:23:09.000000 jcvi-1.4.2/jcvi/algorithms/matrix.py
--rw-r--r--   0 bao        (501) staff       (20)     1296 2021-06-19 19:45:56.000000 jcvi-1.4.2/jcvi/algorithms/maxsum.py
--rw-r--r--   0 bao        (501) staff       (20)     1203 2023-11-24 05:16:26.000000 jcvi-1.4.2/jcvi/algorithms/ml.py
--rwxr-xr-x   0 bao        (501) staff       (20)     4999 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/algorithms/supermap.py
--rw-r--r--   0 bao        (501) staff       (20)    12559 2022-11-26 15:55:17.000000 jcvi-1.4.2/jcvi/algorithms/tsp.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-03-01 06:50:26.967825 jcvi-1.4.2/jcvi/annotation/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/annotation/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      261 2021-06-19 08:23:09.000000 jcvi-1.4.2/jcvi/annotation/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    21414 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/annotation/ahrd.py
--rw-r--r--   0 bao        (501) staff       (20)     7899 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/annotation/automaton.py
--rwxr-xr-x   0 bao        (501) staff       (20)     6417 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/annotation/depth.py
--rw-r--r--   0 bao        (501) staff       (20)     7042 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/annotation/evm.py
--rw-r--r--   0 bao        (501) staff       (20)    14687 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/annotation/maker.py
--rw-r--r--   0 bao        (501) staff       (20)    19485 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/annotation/pasa.py
--rw-r--r--   0 bao        (501) staff       (20)    12822 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/annotation/qc.py
--rw-r--r--   0 bao        (501) staff       (20)    42839 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/annotation/reformat.py
--rw-r--r--   0 bao        (501) staff       (20)    12645 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/annotation/stats.py
--rw-r--r--   0 bao        (501) staff       (20)     6793 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/annotation/train.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-03-01 06:50:26.972388 jcvi-1.4.2/jcvi/apps/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/apps/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      258 2021-06-19 08:23:09.000000 jcvi-1.4.2/jcvi/apps/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    16889 2023-02-19 15:03:46.000000 jcvi-1.4.2/jcvi/apps/align.py
--rw-r--r--   0 bao        (501) staff       (20)    68211 2024-03-01 06:44:50.000000 jcvi-1.4.2/jcvi/apps/base.py
--rw-r--r--   0 bao        (501) staff       (20)    12271 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/apps/biomart.py
--rwxr-xr-x   0 bao        (501) staff       (20)     3554 2021-06-19 19:45:56.000000 jcvi-1.4.2/jcvi/apps/blastplus.py
--rw-r--r--   0 bao        (501) staff       (20)     5219 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/apps/bowtie.py
--rw-r--r--   0 bao        (501) staff       (20)     7695 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/apps/bwa.py
--rw-r--r--   0 bao        (501) staff       (20)     7279 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/apps/cdhit.py
--rw-r--r--   0 bao        (501) staff       (20)     2623 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/apps/emboss.py
--rw-r--r--   0 bao        (501) staff       (20)    21332 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/apps/fetch.py
--rw-r--r--   0 bao        (501) staff       (20)    19459 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/apps/gbsubmit.py
--rw-r--r--   0 bao        (501) staff       (20)     6892 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/apps/gmap.py
--rw-r--r--   0 bao        (501) staff       (20)    18476 2023-04-29 14:56:25.000000 jcvi-1.4.2/jcvi/apps/grid.py
--rw-r--r--   0 bao        (501) staff       (20)    33945 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/apps/ks.py
--rwxr-xr-x   0 bao        (501) staff       (20)     7238 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/apps/lastz.py
--rwxr-xr-x   0 bao        (501) staff       (20)     3004 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/apps/mask.py
--rw-r--r--   0 bao        (501) staff       (20)    35471 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/apps/phylo.py
--rw-r--r--   0 bao        (501) staff       (20)     1896 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/apps/r.py
--rw-r--r--   0 bao        (501) staff       (20)     4901 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/apps/restriction.py
--rw-r--r--   0 bao        (501) staff       (20)     2116 2021-06-19 08:23:09.000000 jcvi-1.4.2/jcvi/apps/script.py
--rw-r--r--   0 bao        (501) staff       (20)     3784 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/apps/softlink.py
--rw-r--r--   0 bao        (501) staff       (20)    33065 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/apps/uclust.py
--rw-r--r--   0 bao        (501) staff       (20)     5208 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/apps/uniprot.py
--rw-r--r--   0 bao        (501) staff       (20)     3661 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/apps/vecscreen.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-03-01 06:50:26.975956 jcvi-1.4.2/jcvi/assembly/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/assembly/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      257 2021-06-19 08:23:09.000000 jcvi-1.4.2/jcvi/assembly/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    66136 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/assembly/allmaps.py
--rw-r--r--   0 bao        (501) staff       (20)    15451 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/assembly/allpaths.py
--rw-r--r--   0 bao        (501) staff       (20)    13265 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/assembly/automaton.py
--rw-r--r--   0 bao        (501) staff       (20)     5544 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/assembly/base.py
--rw-r--r--   0 bao        (501) staff       (20)    34986 2023-11-24 05:16:26.000000 jcvi-1.4.2/jcvi/assembly/ca.py
--rw-r--r--   0 bao        (501) staff       (20)     3457 2022-09-27 05:18:33.000000 jcvi-1.4.2/jcvi/assembly/chic.pyx
--rw-r--r--   0 bao        (501) staff       (20)     4581 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/assembly/coverage.py
--rw-r--r--   0 bao        (501) staff       (20)     8676 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/assembly/gaps.py
--rw-r--r--   0 bao        (501) staff       (20)    20212 2023-02-19 15:03:46.000000 jcvi-1.4.2/jcvi/assembly/geneticmap.py
--rw-r--r--   0 bao        (501) staff       (20)    34693 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/assembly/goldenpath.py
--rw-r--r--   0 bao        (501) staff       (20)    57613 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/assembly/hic.py
--rw-r--r--   0 bao        (501) staff       (20)    43632 2023-05-05 09:23:28.000000 jcvi-1.4.2/jcvi/assembly/kmer.py
--rw-r--r--   0 bao        (501) staff       (20)    12519 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/assembly/opticalmap.py
--rw-r--r--   0 bao        (501) staff       (20)    27279 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/assembly/patch.py
--rw-r--r--   0 bao        (501) staff       (20)    15741 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/assembly/postprocess.py
--rw-r--r--   0 bao        (501) staff       (20)    23470 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/assembly/preprocess.py
--rw-r--r--   0 bao        (501) staff       (20)     6287 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/assembly/sim.py
--rw-r--r--   0 bao        (501) staff       (20)     8830 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/assembly/soap.py
--rw-r--r--   0 bao        (501) staff       (20)    16183 2023-04-26 05:51:28.000000 jcvi-1.4.2/jcvi/assembly/syntenypath.py
--rw-r--r--   0 bao        (501) staff       (20)     5042 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/assembly/trinity.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-03-01 06:50:26.977736 jcvi-1.4.2/jcvi/compara/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/compara/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      251 2021-06-19 08:23:09.000000 jcvi-1.4.2/jcvi/compara/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)     4218 2023-09-28 09:59:53.000000 jcvi-1.4.2/jcvi/compara/base.py
--rwxr-xr-x   0 bao        (501) staff       (20)     9796 2023-04-26 05:51:28.000000 jcvi-1.4.2/jcvi/compara/blastfilter.py
--rw-r--r--   0 bao        (501) staff       (20)    28049 2023-09-27 02:58:13.000000 jcvi-1.4.2/jcvi/compara/catalog.py
--rw-r--r--   0 bao        (501) staff       (20)    26355 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/compara/fractionation.py
--rw-r--r--   0 bao        (501) staff       (20)     9216 2023-04-26 05:51:28.000000 jcvi-1.4.2/jcvi/compara/pad.py
--rw-r--r--   0 bao        (501) staff       (20)     3051 2021-06-19 08:23:09.000000 jcvi-1.4.2/jcvi/compara/phylogeny.py
--rwxr-xr-x   0 bao        (501) staff       (20)     7948 2023-04-26 05:51:28.000000 jcvi-1.4.2/jcvi/compara/quota.py
--rw-r--r--   0 bao        (501) staff       (20)    10341 2023-04-26 05:51:28.000000 jcvi-1.4.2/jcvi/compara/reconstruct.py
--rwxr-xr-x   0 bao        (501) staff       (20)     9233 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/compara/synfind.py
--rwxr-xr-x   0 bao        (501) staff       (20)    57574 2023-04-26 05:51:28.000000 jcvi-1.4.2/jcvi/compara/synteny.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-03-01 06:50:26.983225 jcvi-1.4.2/jcvi/formats/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/formats/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      262 2021-06-19 08:23:09.000000 jcvi-1.4.2/jcvi/formats/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    63559 2023-12-20 05:50:50.000000 jcvi-1.4.2/jcvi/formats/agp.py
--rw-r--r--   0 bao        (501) staff       (20)    33830 2023-09-28 09:59:53.000000 jcvi-1.4.2/jcvi/formats/base.py
--rwxr-xr-x   0 bao        (501) staff       (20)    75058 2023-11-24 03:51:46.000000 jcvi-1.4.2/jcvi/formats/bed.py
--rw-r--r--   0 bao        (501) staff       (20)    43184 2023-06-19 14:46:14.000000 jcvi-1.4.2/jcvi/formats/blast.py
--rw-r--r--   0 bao        (501) staff       (20)     7010 2022-09-27 05:18:33.000000 jcvi-1.4.2/jcvi/formats/cblast.pyx
--rw-r--r--   0 bao        (501) staff       (20)     3193 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/formats/cdt.py
--rw-r--r--   0 bao        (501) staff       (20)     8612 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/formats/chain.py
--rw-r--r--   0 bao        (501) staff       (20)     4644 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/formats/contig.py
--rw-r--r--   0 bao        (501) staff       (20)    15170 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/formats/coords.py
--rw-r--r--   0 bao        (501) staff       (20)     6529 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/formats/excel.py
--rw-r--r--   0 bao        (501) staff       (20)    75590 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/formats/fasta.py
--rw-r--r--   0 bao        (501) staff       (20)    29575 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/formats/fastq.py
--rw-r--r--   0 bao        (501) staff       (20)    15549 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/formats/genbank.py
--rw-r--r--   0 bao        (501) staff       (20)   120171 2023-11-24 03:51:46.000000 jcvi-1.4.2/jcvi/formats/gff.py
--rw-r--r--   0 bao        (501) staff       (20)     3979 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/formats/html.py
--rw-r--r--   0 bao        (501) staff       (20)     4612 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/formats/maf.py
--rwxr-xr-x   0 bao        (501) staff       (20)     2842 2021-07-05 22:45:00.000000 jcvi-1.4.2/jcvi/formats/obo.py
--rw-r--r--   0 bao        (501) staff       (20)     2900 2021-01-11 06:59:36.000000 jcvi-1.4.2/jcvi/formats/paf.py
--rw-r--r--   0 bao        (501) staff       (20)     2785 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/formats/pdf.py
--rwxr-xr-x   0 bao        (501) staff       (20)    10355 2023-11-24 05:16:26.000000 jcvi-1.4.2/jcvi/formats/psl.py
--rw-r--r--   0 bao        (501) staff       (20)     2746 2021-06-19 08:23:09.000000 jcvi-1.4.2/jcvi/formats/pyblast.py
--rw-r--r--   0 bao        (501) staff       (20)    28231 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/formats/sam.py
--rw-r--r--   0 bao        (501) staff       (20)     8041 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/formats/sizes.py
--rw-r--r--   0 bao        (501) staff       (20)    25480 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/formats/vcf.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-03-01 06:50:26.987777 jcvi-1.4.2/jcvi/graphics/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/graphics/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      271 2021-06-19 08:23:09.000000 jcvi-1.4.2/jcvi/graphics/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    16271 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/graphics/align.py
--rw-r--r--   0 bao        (501) staff       (20)    15265 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/graphics/assembly.py
--rw-r--r--   0 bao        (501) staff       (20)    21857 2023-11-24 05:06:52.000000 jcvi-1.4.2/jcvi/graphics/base.py
--rwxr-xr-x   0 bao        (501) staff       (20)    10006 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/graphics/blastplot.py
--rw-r--r--   0 bao        (501) staff       (20)    22275 2023-11-24 05:06:52.000000 jcvi-1.4.2/jcvi/graphics/chromosome.py
--rw-r--r--   0 bao        (501) staff       (20)     7145 2021-06-19 08:23:09.000000 jcvi-1.4.2/jcvi/graphics/coverage.py
--rwxr-xr-x   0 bao        (501) staff       (20)    14873 2023-04-26 05:51:28.000000 jcvi-1.4.2/jcvi/graphics/dotplot.py
--rw-r--r--   0 bao        (501) staff       (20)    21810 2023-02-06 05:16:46.000000 jcvi-1.4.2/jcvi/graphics/glyph.py
--rw-r--r--   0 bao        (501) staff       (20)    23626 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/graphics/grabseeds.py
--rwxr-xr-x   0 bao        (501) staff       (20)     2379 2021-06-19 08:23:09.000000 jcvi-1.4.2/jcvi/graphics/graph.py
--rw-r--r--   0 bao        (501) staff       (20)     5025 2021-03-26 15:38:36.000000 jcvi-1.4.2/jcvi/graphics/heatmap.py
--rw-r--r--   0 bao        (501) staff       (20)     9612 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/graphics/histogram.py
--rw-r--r--   0 bao        (501) staff       (20)    13375 2023-02-08 03:44:09.000000 jcvi-1.4.2/jcvi/graphics/karyotype.py
--rw-r--r--   0 bao        (501) staff       (20)    31416 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/graphics/landscape.py
--rw-r--r--   0 bao        (501) staff       (20)     1276 2021-06-19 08:23:09.000000 jcvi-1.4.2/jcvi/graphics/logo.py
--rw-r--r--   0 bao        (501) staff       (20)     3893 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/graphics/mummerplot.py
--rw-r--r--   0 bao        (501) staff       (20)    22507 2024-02-08 05:51:57.000000 jcvi-1.4.2/jcvi/graphics/synteny.py
--rw-r--r--   0 bao        (501) staff       (20)     5488 2021-06-19 19:45:56.000000 jcvi-1.4.2/jcvi/graphics/table.py
--rw-r--r--   0 bao        (501) staff       (20)    20377 2022-11-26 16:06:34.000000 jcvi-1.4.2/jcvi/graphics/tree.py
--rw-r--r--   0 bao        (501) staff       (20)     6194 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/graphics/wheel.py
--rw-r--r--   0 bao        (501) staff       (20)     1675 2021-03-26 15:38:36.000000 jcvi-1.4.2/jcvi/graphics/whisker.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-03-01 06:50:26.990978 jcvi-1.4.2/jcvi/projects/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/projects/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      260 2021-06-19 08:23:09.000000 jcvi-1.4.2/jcvi/projects/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    22445 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/projects/age.py
--rw-r--r--   0 bao        (501) staff       (20)     1571 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/projects/alfalfa.py
--rw-r--r--   0 bao        (501) staff       (20)    15907 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/projects/allmaps.py
--rw-r--r--   0 bao        (501) staff       (20)     6750 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/projects/bites.py
--rw-r--r--   0 bao        (501) staff       (20)     5679 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/projects/heterosis.py
--rw-r--r--   0 bao        (501) staff       (20)    14136 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/projects/ies.py
--rw-r--r--   0 bao        (501) staff       (20)    22201 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/projects/misc.py
--rw-r--r--   0 bao        (501) staff       (20)    25024 2023-02-06 05:16:46.000000 jcvi-1.4.2/jcvi/projects/napus.py
--rw-r--r--   0 bao        (501) staff       (20)    12754 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/projects/pineapple.py
--rw-r--r--   0 bao        (501) staff       (20)     2367 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/projects/pistachio.py
--rw-r--r--   0 bao        (501) staff       (20)    67857 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/projects/str.py
--rw-r--r--   0 bao        (501) staff       (20)    25768 2023-04-29 14:56:25.000000 jcvi-1.4.2/jcvi/projects/sugarcane.py
--rw-r--r--   0 bao        (501) staff       (20)    23950 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/projects/synfind.py
--rw-r--r--   0 bao        (501) staff       (20)    21554 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/projects/tgbs.py
--rw-r--r--   0 bao        (501) staff       (20)    11941 2023-04-26 05:51:28.000000 jcvi-1.4.2/jcvi/projects/vanilla.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-03-01 06:50:26.993042 jcvi-1.4.2/jcvi/utils/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/utils/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      260 2021-06-19 08:23:09.000000 jcvi-1.4.2/jcvi/utils/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    24200 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/utils/aws.py
--rw-r--r--   0 bao        (501) staff       (20)    12512 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/utils/cbook.py
--rw-r--r--   0 bao        (501) staff       (20)      355 2021-01-11 02:34:49.000000 jcvi-1.4.2/jcvi/utils/console.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-03-01 06:50:26.995455 jcvi-1.4.2/jcvi/utils/data/
--rwxr-xr-x   0 bao        (501) staff       (20)    16912 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/utils/data/Airswing.ttf
--rwxr-xr-x   0 bao        (501) staff       (20)   103940 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/utils/data/Collegia.ttf
--rwxr-xr-x   0 bao        (501) staff       (20)    20468 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/utils/data/HookedUp.ttf
--rw-r--r--   0 bao        (501) staff       (20)    25832 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/utils/data/Humor-Sans.ttf
--rw-r--r--   0 bao        (501) staff       (20)    28065 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/utils/data/TREDs.meta.csv
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/utils/data/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      911 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/utils/data/adapters.fasta
--rw-r--r--   0 bao        (501) staff       (20)     3321 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/utils/data/blosum80.mat
--rw-r--r--   0 bao        (501) staff       (20)     7686 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/utils/data/chrY.hg38.unique_ccn.gc
--rw-r--r--   0 bao        (501) staff       (20)      282 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/utils/data/colorchecker.txt
--rw-r--r--   0 bao        (501) staff       (20)    45544 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/utils/data/hg38.band.txt
--rw-r--r--   0 bao        (501) staff       (20)    11672 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/utils/data/hg38.chrom.sizes
--rw-r--r--   0 bao        (501) staff       (20)     1000 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/utils/data/instance.json
--rw-r--r--   0 bao        (501) staff       (20)     9795 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/utils/db.py
--rw-r--r--   0 bao        (501) staff       (20)     4145 2021-01-09 20:22:53.000000 jcvi-1.4.2/jcvi/utils/ez_setup.py
--rwxr-xr-x   0 bao        (501) staff       (20)     2884 2021-06-19 08:23:09.000000 jcvi-1.4.2/jcvi/utils/grouper.py
--rw-r--r--   0 bao        (501) staff       (20)    10437 2021-06-19 08:23:09.000000 jcvi-1.4.2/jcvi/utils/orderedcollections.py
--rw-r--r--   0 bao        (501) staff       (20)    14595 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/utils/range.py
--rw-r--r--   0 bao        (501) staff       (20)     3946 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/utils/table.py
--rw-r--r--   0 bao        (501) staff       (20)     4687 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/utils/taxonomy.py
--rw-r--r--   0 bao        (501) staff       (20)     1522 2021-07-13 05:06:52.000000 jcvi-1.4.2/jcvi/utils/validator.py
--rwxr-xr-x   0 bao        (501) staff       (20)     1377 2021-01-15 14:44:37.000000 jcvi-1.4.2/jcvi/utils/webcolors.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-03-01 06:50:26.997122 jcvi-1.4.2/jcvi/variation/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.2/jcvi/variation/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      259 2021-06-19 08:23:09.000000 jcvi-1.4.2/jcvi/variation/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    45321 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/variation/cnv.py
--rw-r--r--   0 bao        (501) staff       (20)     7036 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/variation/deconvolute.py
--rw-r--r--   0 bao        (501) staff       (20)     9385 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/variation/delly.py
--rw-r--r--   0 bao        (501) staff       (20)    11777 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/variation/impute.py
--rw-r--r--   0 bao        (501) staff       (20)     3478 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/variation/phase.py
--rw-r--r--   0 bao        (501) staff       (20)    10831 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/variation/snp.py
--rw-r--r--   0 bao        (501) staff       (20)    48818 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/variation/str.py
--rw-r--r--   0 bao        (501) staff       (20)     3672 2023-02-06 03:44:04.000000 jcvi-1.4.2/jcvi/variation/tassel.py
--rw-r--r--   0 bao        (501) staff       (20)      176 2024-03-01 06:50:26.000000 jcvi-1.4.2/jcvi/version.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-03-01 06:50:26.963389 jcvi-1.4.2/jcvi.egg-info/
--rw-r--r--   0 bao        (501) staff       (20)     9485 2024-03-01 06:50:26.000000 jcvi-1.4.2/jcvi.egg-info/PKG-INFO
--rw-r--r--   0 bao        (501) staff       (20)     4727 2024-03-01 06:50:26.000000 jcvi-1.4.2/jcvi.egg-info/SOURCES.txt
--rw-r--r--   0 bao        (501) staff       (20)        1 2024-03-01 06:50:26.000000 jcvi-1.4.2/jcvi.egg-info/dependency_links.txt
--rw-r--r--   0 bao        (501) staff       (20)        1 2022-11-26 21:54:22.000000 jcvi-1.4.2/jcvi.egg-info/not-zip-safe
--rw-r--r--   0 bao        (501) staff       (20)      215 2024-03-01 06:50:26.000000 jcvi-1.4.2/jcvi.egg-info/requires.txt
--rw-r--r--   0 bao        (501) staff       (20)        5 2024-03-01 06:50:26.000000 jcvi-1.4.2/jcvi.egg-info/top_level.txt
--rw-r--r--   0 bao        (501) staff       (20)      359 2022-11-26 21:23:29.000000 jcvi-1.4.2/pyproject.toml
--rw-r--r--   0 bao        (501) staff       (20)     1235 2024-03-01 06:50:26.998004 jcvi-1.4.2/setup.cfg
--rw-r--r--   0 bao        (501) staff       (20)      553 2022-11-26 21:23:29.000000 jcvi-1.4.2/setup.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-29 06:37:24.136548 jcvi-1.4.5/
+-rw-r--r--   0 bao        (501) staff       (20)     1292 2020-03-03 07:11:04.000000 jcvi-1.4.5/LICENSE
+-rw-r--r--   0 bao        (501) staff       (20)       91 2022-11-27 15:24:30.000000 jcvi-1.4.5/MANIFEST.in
+-rw-r--r--   0 bao        (501) staff       (20)     8915 2024-04-29 06:37:24.136638 jcvi-1.4.5/PKG-INFO
+-rw-r--r--   0 bao        (501) staff       (20)     8250 2023-07-25 21:30:23.000000 jcvi-1.4.5/README.md
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-29 06:37:24.111129 jcvi-1.4.5/jcvi/
+-rw-r--r--   0 bao        (501) staff       (20)      770 2022-11-26 21:23:29.000000 jcvi-1.4.5/jcvi/__init__.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-29 06:37:24.113130 jcvi-1.4.5/jcvi/algorithms/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/algorithms/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      263 2021-06-19 08:23:09.000000 jcvi-1.4.5/jcvi/algorithms/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)     6422 2021-06-19 08:23:09.000000 jcvi-1.4.5/jcvi/algorithms/ec.py
+-rw-r--r--   0 bao        (501) staff       (20)     6412 2024-04-28 07:29:54.000000 jcvi-1.4.5/jcvi/algorithms/formula.py
+-rw-r--r--   0 bao        (501) staff       (20)    14132 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/algorithms/graph.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     6275 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/algorithms/lis.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    24228 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/algorithms/lpsolve.py
+-rw-r--r--   0 bao        (501) staff       (20)     6104 2021-06-19 08:23:09.000000 jcvi-1.4.5/jcvi/algorithms/matrix.py
+-rw-r--r--   0 bao        (501) staff       (20)     1296 2021-06-19 19:45:56.000000 jcvi-1.4.5/jcvi/algorithms/maxsum.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     4999 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/algorithms/supermap.py
+-rw-r--r--   0 bao        (501) staff       (20)    12559 2022-11-26 15:55:17.000000 jcvi-1.4.5/jcvi/algorithms/tsp.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-29 06:37:24.114664 jcvi-1.4.5/jcvi/annotation/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/annotation/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      261 2021-06-19 08:23:09.000000 jcvi-1.4.5/jcvi/annotation/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    21414 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/annotation/ahrd.py
+-rw-r--r--   0 bao        (501) staff       (20)     7899 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/annotation/automaton.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     6417 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/annotation/depth.py
+-rw-r--r--   0 bao        (501) staff       (20)     7042 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/annotation/evm.py
+-rw-r--r--   0 bao        (501) staff       (20)    14687 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/annotation/maker.py
+-rw-r--r--   0 bao        (501) staff       (20)    19485 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/annotation/pasa.py
+-rw-r--r--   0 bao        (501) staff       (20)    12822 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/annotation/qc.py
+-rw-r--r--   0 bao        (501) staff       (20)    42839 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/annotation/reformat.py
+-rw-r--r--   0 bao        (501) staff       (20)    12645 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/annotation/stats.py
+-rw-r--r--   0 bao        (501) staff       (20)     6793 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/annotation/train.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-29 06:37:24.117447 jcvi-1.4.5/jcvi/apps/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/apps/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      258 2021-06-19 08:23:09.000000 jcvi-1.4.5/jcvi/apps/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    20591 2024-04-29 06:36:47.000000 jcvi-1.4.5/jcvi/apps/align.py
+-rw-r--r--   0 bao        (501) staff       (20)    68344 2024-04-28 07:29:54.000000 jcvi-1.4.5/jcvi/apps/base.py
+-rw-r--r--   0 bao        (501) staff       (20)    12271 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/apps/biomart.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     3554 2021-06-19 19:45:56.000000 jcvi-1.4.5/jcvi/apps/blastplus.py
+-rw-r--r--   0 bao        (501) staff       (20)     5219 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/apps/bowtie.py
+-rw-r--r--   0 bao        (501) staff       (20)     7695 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/apps/bwa.py
+-rw-r--r--   0 bao        (501) staff       (20)     7279 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/apps/cdhit.py
+-rw-r--r--   0 bao        (501) staff       (20)     2623 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/apps/emboss.py
+-rw-r--r--   0 bao        (501) staff       (20)    21333 2024-04-29 06:36:47.000000 jcvi-1.4.5/jcvi/apps/fetch.py
+-rw-r--r--   0 bao        (501) staff       (20)    19459 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/apps/gbsubmit.py
+-rw-r--r--   0 bao        (501) staff       (20)     6892 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/apps/gmap.py
+-rw-r--r--   0 bao        (501) staff       (20)    18477 2024-04-29 06:36:47.000000 jcvi-1.4.5/jcvi/apps/grid.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     7238 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/apps/lastz.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     3004 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/apps/mask.py
+-rw-r--r--   0 bao        (501) staff       (20)    35471 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/apps/phylo.py
+-rw-r--r--   0 bao        (501) staff       (20)     1896 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/apps/r.py
+-rw-r--r--   0 bao        (501) staff       (20)     4901 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/apps/restriction.py
+-rw-r--r--   0 bao        (501) staff       (20)     3784 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/apps/softlink.py
+-rw-r--r--   0 bao        (501) staff       (20)    33065 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/apps/uclust.py
+-rw-r--r--   0 bao        (501) staff       (20)     5208 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/apps/uniprot.py
+-rw-r--r--   0 bao        (501) staff       (20)     3661 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/apps/vecscreen.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-29 06:37:24.120301 jcvi-1.4.5/jcvi/assembly/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/assembly/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      257 2021-06-19 08:23:09.000000 jcvi-1.4.5/jcvi/assembly/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    66136 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/assembly/allmaps.py
+-rw-r--r--   0 bao        (501) staff       (20)    15451 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/assembly/allpaths.py
+-rw-r--r--   0 bao        (501) staff       (20)    13265 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/assembly/automaton.py
+-rw-r--r--   0 bao        (501) staff       (20)     5544 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/assembly/base.py
+-rw-r--r--   0 bao        (501) staff       (20)    34986 2023-11-24 05:16:26.000000 jcvi-1.4.5/jcvi/assembly/ca.py
+-rw-r--r--   0 bao        (501) staff       (20)     3457 2022-09-27 05:18:33.000000 jcvi-1.4.5/jcvi/assembly/chic.pyx
+-rw-r--r--   0 bao        (501) staff       (20)     4581 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/assembly/coverage.py
+-rw-r--r--   0 bao        (501) staff       (20)     8676 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/assembly/gaps.py
+-rw-r--r--   0 bao        (501) staff       (20)    20002 2024-04-29 06:10:52.000000 jcvi-1.4.5/jcvi/assembly/geneticmap.py
+-rw-r--r--   0 bao        (501) staff       (20)    34692 2024-04-29 06:36:47.000000 jcvi-1.4.5/jcvi/assembly/goldenpath.py
+-rw-r--r--   0 bao        (501) staff       (20)    56167 2024-04-29 06:10:52.000000 jcvi-1.4.5/jcvi/assembly/hic.py
+-rw-r--r--   0 bao        (501) staff       (20)    43034 2024-04-29 06:10:52.000000 jcvi-1.4.5/jcvi/assembly/kmer.py
+-rw-r--r--   0 bao        (501) staff       (20)    12519 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/assembly/opticalmap.py
+-rw-r--r--   0 bao        (501) staff       (20)    27279 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/assembly/patch.py
+-rw-r--r--   0 bao        (501) staff       (20)    15741 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/assembly/postprocess.py
+-rw-r--r--   0 bao        (501) staff       (20)    23472 2024-04-29 06:36:47.000000 jcvi-1.4.5/jcvi/assembly/preprocess.py
+-rw-r--r--   0 bao        (501) staff       (20)     6287 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/assembly/sim.py
+-rw-r--r--   0 bao        (501) staff       (20)     8830 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/assembly/soap.py
+-rw-r--r--   0 bao        (501) staff       (20)    16183 2023-04-26 05:51:28.000000 jcvi-1.4.5/jcvi/assembly/syntenypath.py
+-rw-r--r--   0 bao        (501) staff       (20)     5042 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/assembly/trinity.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-29 06:37:24.121981 jcvi-1.4.5/jcvi/compara/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/compara/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      251 2021-06-19 08:23:09.000000 jcvi-1.4.5/jcvi/compara/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)     4218 2023-09-28 09:59:53.000000 jcvi-1.4.5/jcvi/compara/base.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     9796 2023-04-26 05:51:28.000000 jcvi-1.4.5/jcvi/compara/blastfilter.py
+-rw-r--r--   0 bao        (501) staff       (20)    28698 2024-04-29 06:36:47.000000 jcvi-1.4.5/jcvi/compara/catalog.py
+-rw-r--r--   0 bao        (501) staff       (20)    26355 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/compara/fractionation.py
+-rw-r--r--   0 bao        (501) staff       (20)    33945 2024-04-29 06:10:52.000000 jcvi-1.4.5/jcvi/compara/ks.py
+-rw-r--r--   0 bao        (501) staff       (20)     9216 2023-04-26 05:51:28.000000 jcvi-1.4.5/jcvi/compara/pad.py
+-rw-r--r--   0 bao        (501) staff       (20)     8322 2024-04-29 06:10:52.000000 jcvi-1.4.5/jcvi/compara/pedigree.py
+-rw-r--r--   0 bao        (501) staff       (20)     3051 2021-06-19 08:23:09.000000 jcvi-1.4.5/jcvi/compara/phylogeny.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     7948 2023-04-26 05:51:28.000000 jcvi-1.4.5/jcvi/compara/quota.py
+-rw-r--r--   0 bao        (501) staff       (20)    10341 2023-04-26 05:51:28.000000 jcvi-1.4.5/jcvi/compara/reconstruct.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     9233 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/compara/synfind.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    57574 2023-04-26 05:51:28.000000 jcvi-1.4.5/jcvi/compara/synteny.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-29 06:37:24.125211 jcvi-1.4.5/jcvi/formats/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/formats/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      262 2021-06-19 08:23:09.000000 jcvi-1.4.5/jcvi/formats/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    63559 2024-04-29 06:36:47.000000 jcvi-1.4.5/jcvi/formats/agp.py
+-rw-r--r--   0 bao        (501) staff       (20)    33830 2023-09-28 09:59:53.000000 jcvi-1.4.5/jcvi/formats/base.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    75125 2024-04-29 06:36:47.000000 jcvi-1.4.5/jcvi/formats/bed.py
+-rw-r--r--   0 bao        (501) staff       (20)    43184 2023-06-19 14:46:14.000000 jcvi-1.4.5/jcvi/formats/blast.py
+-rw-r--r--   0 bao        (501) staff       (20)     7010 2022-09-27 05:18:33.000000 jcvi-1.4.5/jcvi/formats/cblast.pyx
+-rw-r--r--   0 bao        (501) staff       (20)     3193 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/formats/cdt.py
+-rw-r--r--   0 bao        (501) staff       (20)     8612 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/formats/chain.py
+-rw-r--r--   0 bao        (501) staff       (20)     4644 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/formats/contig.py
+-rw-r--r--   0 bao        (501) staff       (20)    15169 2024-04-29 06:36:47.000000 jcvi-1.4.5/jcvi/formats/coords.py
+-rw-r--r--   0 bao        (501) staff       (20)     6529 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/formats/excel.py
+-rw-r--r--   0 bao        (501) staff       (20)    75591 2024-04-29 06:36:47.000000 jcvi-1.4.5/jcvi/formats/fasta.py
+-rw-r--r--   0 bao        (501) staff       (20)    29575 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/formats/fastq.py
+-rw-r--r--   0 bao        (501) staff       (20)    15545 2024-04-29 06:36:47.000000 jcvi-1.4.5/jcvi/formats/genbank.py
+-rw-r--r--   0 bao        (501) staff       (20)   120223 2024-04-05 14:11:25.000000 jcvi-1.4.5/jcvi/formats/gff.py
+-rw-r--r--   0 bao        (501) staff       (20)     3979 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/formats/html.py
+-rw-r--r--   0 bao        (501) staff       (20)     4612 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/formats/maf.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     2842 2021-07-05 22:45:00.000000 jcvi-1.4.5/jcvi/formats/obo.py
+-rw-r--r--   0 bao        (501) staff       (20)     2900 2021-01-11 06:59:36.000000 jcvi-1.4.5/jcvi/formats/paf.py
+-rw-r--r--   0 bao        (501) staff       (20)     2783 2024-04-29 06:36:47.000000 jcvi-1.4.5/jcvi/formats/pdf.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    10355 2023-11-24 05:16:26.000000 jcvi-1.4.5/jcvi/formats/psl.py
+-rw-r--r--   0 bao        (501) staff       (20)     2746 2021-06-19 08:23:09.000000 jcvi-1.4.5/jcvi/formats/pyblast.py
+-rw-r--r--   0 bao        (501) staff       (20)    28231 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/formats/sam.py
+-rw-r--r--   0 bao        (501) staff       (20)     8041 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/formats/sizes.py
+-rw-r--r--   0 bao        (501) staff       (20)    25480 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/formats/vcf.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-29 06:37:24.127800 jcvi-1.4.5/jcvi/graphics/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/graphics/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      271 2021-06-19 08:23:09.000000 jcvi-1.4.5/jcvi/graphics/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    16271 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/graphics/align.py
+-rw-r--r--   0 bao        (501) staff       (20)    15265 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/graphics/assembly.py
+-rw-r--r--   0 bao        (501) staff       (20)    24647 2024-04-29 06:10:52.000000 jcvi-1.4.5/jcvi/graphics/base.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    10002 2024-04-29 06:36:47.000000 jcvi-1.4.5/jcvi/graphics/blastplot.py
+-rw-r--r--   0 bao        (501) staff       (20)    22341 2024-04-29 06:10:52.000000 jcvi-1.4.5/jcvi/graphics/chromosome.py
+-rw-r--r--   0 bao        (501) staff       (20)     7145 2021-06-19 08:23:09.000000 jcvi-1.4.5/jcvi/graphics/coverage.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    14873 2023-04-26 05:51:28.000000 jcvi-1.4.5/jcvi/graphics/dotplot.py
+-rw-r--r--   0 bao        (501) staff       (20)    21810 2023-02-06 05:16:46.000000 jcvi-1.4.5/jcvi/graphics/glyph.py
+-rw-r--r--   0 bao        (501) staff       (20)    24862 2024-04-24 05:29:17.000000 jcvi-1.4.5/jcvi/graphics/grabseeds.py
+-rw-r--r--   0 bao        (501) staff       (20)     5025 2021-03-26 15:38:36.000000 jcvi-1.4.5/jcvi/graphics/heatmap.py
+-rw-r--r--   0 bao        (501) staff       (20)     9610 2024-04-29 06:36:47.000000 jcvi-1.4.5/jcvi/graphics/histogram.py
+-rw-r--r--   0 bao        (501) staff       (20)    13375 2023-02-08 03:44:09.000000 jcvi-1.4.5/jcvi/graphics/karyotype.py
+-rw-r--r--   0 bao        (501) staff       (20)    32418 2024-04-29 06:10:52.000000 jcvi-1.4.5/jcvi/graphics/landscape.py
+-rw-r--r--   0 bao        (501) staff       (20)     3893 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/graphics/mummerplot.py
+-rw-r--r--   0 bao        (501) staff       (20)    22507 2024-02-08 05:51:57.000000 jcvi-1.4.5/jcvi/graphics/synteny.py
+-rw-r--r--   0 bao        (501) staff       (20)     5488 2021-06-19 19:45:56.000000 jcvi-1.4.5/jcvi/graphics/table.py
+-rw-r--r--   0 bao        (501) staff       (20)    20377 2022-11-26 16:06:34.000000 jcvi-1.4.5/jcvi/graphics/tree.py
+-rw-r--r--   0 bao        (501) staff       (20)     6194 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/graphics/wheel.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-29 06:37:24.129711 jcvi-1.4.5/jcvi/projects/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/projects/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      260 2021-06-19 08:23:09.000000 jcvi-1.4.5/jcvi/projects/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    22445 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/projects/age.py
+-rw-r--r--   0 bao        (501) staff       (20)    15907 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/projects/allmaps.py
+-rw-r--r--   0 bao        (501) staff       (20)     6750 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/projects/bites.py
+-rw-r--r--   0 bao        (501) staff       (20)    14136 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/projects/ies.py
+-rw-r--r--   0 bao        (501) staff       (20)     7050 2024-04-29 06:10:52.000000 jcvi-1.4.5/jcvi/projects/jcvi.py
+-rw-r--r--   0 bao        (501) staff       (20)    22179 2024-04-29 06:10:52.000000 jcvi-1.4.5/jcvi/projects/misc.py
+-rw-r--r--   0 bao        (501) staff       (20)    25024 2023-02-06 05:16:46.000000 jcvi-1.4.5/jcvi/projects/napus.py
+-rw-r--r--   0 bao        (501) staff       (20)    12754 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/projects/pineapple.py
+-rw-r--r--   0 bao        (501) staff       (20)    67853 2024-04-29 06:36:47.000000 jcvi-1.4.5/jcvi/projects/str.py
+-rw-r--r--   0 bao        (501) staff       (20)    25766 2024-04-29 06:36:47.000000 jcvi-1.4.5/jcvi/projects/sugarcane.py
+-rw-r--r--   0 bao        (501) staff       (20)    23950 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/projects/synfind.py
+-rw-r--r--   0 bao        (501) staff       (20)    21554 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/projects/tgbs.py
+-rw-r--r--   0 bao        (501) staff       (20)    11941 2023-04-26 05:51:28.000000 jcvi-1.4.5/jcvi/projects/vanilla.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-29 06:37:24.131265 jcvi-1.4.5/jcvi/utils/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/utils/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      260 2021-06-19 08:23:09.000000 jcvi-1.4.5/jcvi/utils/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    24200 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/utils/aws.py
+-rw-r--r--   0 bao        (501) staff       (20)    12513 2024-04-29 06:36:47.000000 jcvi-1.4.5/jcvi/utils/cbook.py
+-rw-r--r--   0 bao        (501) staff       (20)      355 2021-01-11 02:34:49.000000 jcvi-1.4.5/jcvi/utils/console.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-29 06:37:24.135332 jcvi-1.4.5/jcvi/utils/data/
+-rwxr-xr-x   0 bao        (501) staff       (20)    16912 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/utils/data/Airswing.ttf
+-rwxr-xr-x   0 bao        (501) staff       (20)   103940 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/utils/data/Collegia.ttf
+-rwxr-xr-x   0 bao        (501) staff       (20)    20468 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/utils/data/HookedUp.ttf
+-rw-r--r--   0 bao        (501) staff       (20)    25832 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/utils/data/Humor-Sans.ttf
+-rw-r--r--   0 bao        (501) staff       (20)    28065 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/utils/data/TREDs.meta.csv
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/utils/data/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      911 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/utils/data/adapters.fasta
+-rw-r--r--   0 bao        (501) staff       (20)     3321 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/utils/data/blosum80.mat
+-rw-r--r--   0 bao        (501) staff       (20)     7686 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/utils/data/chrY.hg38.unique_ccn.gc
+-rw-r--r--   0 bao        (501) staff       (20)      282 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/utils/data/colorchecker.txt
+-rw-r--r--   0 bao        (501) staff       (20)    45544 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/utils/data/hg38.band.txt
+-rw-r--r--   0 bao        (501) staff       (20)    11672 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/utils/data/hg38.chrom.sizes
+-rw-r--r--   0 bao        (501) staff       (20)     1000 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/utils/data/instance.json
+-rw-r--r--   0 bao        (501) staff       (20)     9793 2024-04-29 06:36:47.000000 jcvi-1.4.5/jcvi/utils/db.py
+-rw-r--r--   0 bao        (501) staff       (20)     4145 2021-01-09 20:22:53.000000 jcvi-1.4.5/jcvi/utils/ez_setup.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     2884 2021-06-19 08:23:09.000000 jcvi-1.4.5/jcvi/utils/grouper.py
+-rw-r--r--   0 bao        (501) staff       (20)    10437 2021-06-19 08:23:09.000000 jcvi-1.4.5/jcvi/utils/orderedcollections.py
+-rw-r--r--   0 bao        (501) staff       (20)    14595 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/utils/range.py
+-rw-r--r--   0 bao        (501) staff       (20)     3946 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/utils/table.py
+-rw-r--r--   0 bao        (501) staff       (20)     4687 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/utils/taxonomy.py
+-rw-r--r--   0 bao        (501) staff       (20)     1522 2021-07-13 05:06:52.000000 jcvi-1.4.5/jcvi/utils/validator.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     1377 2021-01-15 14:44:37.000000 jcvi-1.4.5/jcvi/utils/webcolors.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-29 06:37:24.136406 jcvi-1.4.5/jcvi/variation/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/variation/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      259 2021-06-19 08:23:09.000000 jcvi-1.4.5/jcvi/variation/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    45321 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/variation/cnv.py
+-rw-r--r--   0 bao        (501) staff       (20)     7036 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/variation/deconvolute.py
+-rw-r--r--   0 bao        (501) staff       (20)     9385 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/variation/delly.py
+-rw-r--r--   0 bao        (501) staff       (20)    11777 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/variation/impute.py
+-rw-r--r--   0 bao        (501) staff       (20)     3478 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/variation/phase.py
+-rw-r--r--   0 bao        (501) staff       (20)    10831 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/variation/snp.py
+-rw-r--r--   0 bao        (501) staff       (20)    48818 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/variation/str.py
+-rw-r--r--   0 bao        (501) staff       (20)      176 2024-04-29 06:37:23.000000 jcvi-1.4.5/jcvi/version.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-29 06:37:24.111885 jcvi-1.4.5/jcvi.egg-info/
+-rw-r--r--   0 bao        (501) staff       (20)     8915 2024-04-29 06:37:24.000000 jcvi-1.4.5/jcvi.egg-info/PKG-INFO
+-rw-r--r--   0 bao        (501) staff       (20)     4561 2024-04-29 06:37:24.000000 jcvi-1.4.5/jcvi.egg-info/SOURCES.txt
+-rw-r--r--   0 bao        (501) staff       (20)        1 2024-04-29 06:37:24.000000 jcvi-1.4.5/jcvi.egg-info/dependency_links.txt
+-rw-r--r--   0 bao        (501) staff       (20)        1 2022-11-26 21:54:22.000000 jcvi-1.4.5/jcvi.egg-info/not-zip-safe
+-rw-r--r--   0 bao        (501) staff       (20)      221 2024-04-29 06:37:24.000000 jcvi-1.4.5/jcvi.egg-info/requires.txt
+-rw-r--r--   0 bao        (501) staff       (20)        5 2024-04-29 06:37:24.000000 jcvi-1.4.5/jcvi.egg-info/top_level.txt
+-rw-r--r--   0 bao        (501) staff       (20)      359 2022-11-26 21:23:29.000000 jcvi-1.4.5/pyproject.toml
+-rw-r--r--   0 bao        (501) staff       (20)     1242 2024-04-29 06:37:24.137099 jcvi-1.4.5/setup.cfg
+-rw-r--r--   0 bao        (501) staff       (20)      553 2022-11-26 21:23:29.000000 jcvi-1.4.5/setup.py
```

### Comparing `jcvi-1.4.2/LICENSE` & `jcvi-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/PKG-INFO` & `jcvi-1.4.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,24 @@
 Metadata-Version: 2.1
 Name: jcvi
-Version: 1.4.2
+Version: 1.4.5
 Summary: Python utility libraries on genome assembly, annotation and comparative genomics
 Home-page: http://github.com/tanghaibao/jcvi
 Author: Haibao Tang, Vivek Krishnakumar, Jingping Li
 Author-email: tanghaibao@gmail.com
 License: BSD
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: CrossMap
-Requires-Dist: PyPDF2
-Requires-Dist: biopython
-Requires-Dist: boto3
-Requires-Dist: brewer2mpl
-Requires-Dist: deap
-Requires-Dist: ete3
-Requires-Dist: ftpretty
-Requires-Dist: gffutils
-Requires-Dist: goatools
-Requires-Dist: genomepy
-Requires-Dist: graphviz
-Requires-Dist: jinja2
-Requires-Dist: matplotlib
-Requires-Dist: more-itertools
-Requires-Dist: natsort
-Requires-Dist: networkx
-Requires-Dist: numpy
-Requires-Dist: ortools
-Requires-Dist: pybedtools
-Requires-Dist: rich
-Requires-Dist: scikit-image
-Requires-Dist: scipy
-Requires-Dist: seaborn
-Requires-Dist: webcolors
 
 # JCVI utility libraries
 
 [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.31631.svg)](https://doi.org/10.5281/zenodo.594205)
 [![Latest PyPI version](https://img.shields.io/pypi/v/jcvi.svg)](https://pypi.python.org/pypi/jcvi)
 [![bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/jcvi/README.html?highlight=jcvi)
 [![Github Actions](https://github.com/tanghaibao/jcvi/workflows/build/badge.svg)](https://github.com/tanghaibao/jcvi/actions)
@@ -246,7 +222,9 @@
 **Feel free to check out other scripts in the package, it is not just
 for FASTA.**
 
 ## Star History
 
 [![Star History
 Chart](https://api.star-history.com/svg?repos=tanghaibao/jcvi&type=Date)](https://star-history.com/#tanghaibao/jcvi&Date)
+
+
```

### Comparing `jcvi-1.4.2/README.md` & `jcvi-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/__init__.py` & `jcvi-1.4.5/jcvi/__init__.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/algorithms/ec.py` & `jcvi-1.4.5/jcvi/algorithms/ec.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/algorithms/formula.py` & `jcvi-1.4.5/jcvi/algorithms/formula.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 
 """
 Some math formula for various calculations
 """
 import sys
-import numpy as np
 
+from collections import Counter
+from functools import lru_cache
 from math import log, exp, sqrt
 
-from jcvi.utils.cbook import human_size
+import numpy as np
+import scipy
+
+from ..utils.cbook import human_size
 
 
 def mean_confidence_interval(data, confidence=0.95):
     # Compute the confidence interval around the mean
-    import scipy
 
     a = 1.0 * np.array(data)
     n = len(a)
     m, se = np.mean(a), scipy.stats.sem(a)
     h = se * scipy.stats.t._ppf((1 + confidence) / 2.0, n - 1)
     return m, m - h, m + h
 
@@ -172,15 +175,15 @@
     >>> jukesCantorD(.7)
     (2.0310376508266565, 0.47249999999999864)
     """
     assert 0 <= p < 0.75
 
     rD = 1 - 4.0 / 3 * p
     D = -0.75 * log(rD)
-    varD = p * (1 - p) / (rD ** 2 * L)
+    varD = p * (1 - p) / (rD**2 * L)
 
     return D, varD
 
 
 def jukesCantorP(D):
     """
     >>> jukesCantorP(.1)
@@ -214,12 +217,39 @@
     print("NumReads: {0}M".format(numreads), file=sys.stderr)
     print("K: {0}".format(K), file=sys.stderr)
 
     ram = human_size(ram * 1000, a_kilobyte_is_1024_bytes=True)
     print("RAM usage: {0} (MAXKMERLENGTH=31)".format(ram), file=sys.stderr)
 
 
-if __name__ == "__main__":
+@lru_cache(maxsize=None)
+def calc_ldscore(a: str, b: str) -> float:
+    """
+    Calculate Linkage disequilibrium (r2) between two genotypes.
+    """
+    assert len(a) == len(b), f"{a}\n{b}"
+    # Assumes markers as A/B
+    c = Counter(zip(a, b))
+    c_aa = c[("A", "A")]
+    c_ab = c[("A", "B")]
+    c_ba = c[("B", "A")]
+    c_bb = c[("B", "B")]
+    n = c_aa + c_ab + c_ba + c_bb
+    if n == 0:
+        return 0
 
-    import doctest
+    f = 1.0 / n
+    x_aa = c_aa * f
+    x_ab = c_ab * f
+    x_ba = c_ba * f
+    x_bb = c_bb * f
+    p_a = x_aa + x_ab
+    p_b = x_ba + x_bb
+    q_a = x_aa + x_ba
+    q_b = x_ab + x_bb
+    D = x_aa - p_a * q_a
+    denominator = p_a * p_b * q_a * q_b
+    if denominator == 0:
+        return 0
 
-    doctest.testmod()
+    r2 = D * D / denominator
+    return r2
```

### Comparing `jcvi-1.4.2/jcvi/algorithms/graph.py` & `jcvi-1.4.5/jcvi/algorithms/graph.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/algorithms/lis.py` & `jcvi-1.4.5/jcvi/algorithms/lis.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/algorithms/lpsolve.py` & `jcvi-1.4.5/jcvi/algorithms/lpsolve.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/algorithms/matrix.py` & `jcvi-1.4.5/jcvi/algorithms/matrix.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/algorithms/maxsum.py` & `jcvi-1.4.5/jcvi/algorithms/maxsum.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/algorithms/supermap.py` & `jcvi-1.4.5/jcvi/algorithms/supermap.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/algorithms/tsp.py` & `jcvi-1.4.5/jcvi/algorithms/tsp.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/annotation/ahrd.py` & `jcvi-1.4.5/jcvi/annotation/ahrd.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/annotation/automaton.py` & `jcvi-1.4.5/jcvi/annotation/automaton.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/annotation/depth.py` & `jcvi-1.4.5/jcvi/annotation/depth.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/annotation/evm.py` & `jcvi-1.4.5/jcvi/annotation/evm.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/annotation/maker.py` & `jcvi-1.4.5/jcvi/annotation/maker.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/annotation/pasa.py` & `jcvi-1.4.5/jcvi/annotation/pasa.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/annotation/qc.py` & `jcvi-1.4.5/jcvi/annotation/qc.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/annotation/reformat.py` & `jcvi-1.4.5/jcvi/annotation/reformat.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/annotation/stats.py` & `jcvi-1.4.5/jcvi/annotation/stats.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/annotation/train.py` & `jcvi-1.4.5/jcvi/annotation/train.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/apps/align.py` & `jcvi-1.4.5/jcvi/apps/align.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,14 +28,21 @@
 def run_formatdb(infile=None, outfile=None, dbtype="nucl"):
     cmd = "makeblastdb"
     cmd += " -dbtype {0} -in {1}".format(dbtype, infile)
     sh(cmd)
 
 
 @depends
+def run_diamond_makedb(infile=None, outfile=None):
+    cmd = "diamond makedb"
+    cmd += " --in {0} --db {1} -p 5".format(infile, infile)
+    sh(cmd)
+
+
+@depends
 def run_blat(
     infile=None,
     outfile=None,
     db="UniVec_Core",
     pctid=95,
     hitlen=50,
     cpus=16,
@@ -582,9 +589,130 @@
             logging.error(message)
             logging.fatal("Failed to run `lastal`. Aborted.")
             cleanup(lastfile)
             sys.exit(1)
     return lastfile
 
 
+def blast_main(args, dbtype=None):
+    """
+    %prog database.fasta query.fasta
+
+    Run blastp/blastn by calling BLAST+ blastp/blastn depends on dbtype.
+    """
+    p = OptionParser(blast_main.__doc__)
+    p.add_option(
+        "--dbtype",
+        default="nucl",
+        choices=("nucl", "prot"),
+        help="Molecule type of subject database",
+    )
+    p.add_option("--path", help="Specify BLAST path for blastn or blastp")
+
+    p.set_cpus()
+    p.set_outdir()
+    p.set_params()
+
+    opts, args = p.parse_args(args)
+
+    if len(args) != 2:
+        sys.exit(not p.print_help())
+
+    subject, query = args
+    path = opts.path
+    cpus = opts.cpus
+    if not dbtype:
+        dbtype = opts.dbtype
+
+    getpath = lambda x: op.join(path, x) if path else x
+    cmd = "blastn" if dbtype == "nucl" else "blastp"
+    lastdb_bin = getpath("makeblastdb")
+    lastal_bin = getpath(cmd)
+    for bin in (lastdb_bin, lastal_bin):
+        if not which(bin):
+            logging.fatal("`%s` not found on PATH. Have you installed BLAST?", bin)
+            sys.exit(1)
+
+    db_suffix = ".nin" if dbtype == "nucl" else ".pin"
+
+    run_formatdb(infile=subject, outfile=subject + db_suffix, dbtype=dbtype)
+
+    blastfile = get_outfile(subject, query, suffix="last", outdir=opts.outdir)
+    # Make several attempts to run LASTAL
+    try:
+        sh(
+            cmd
+            + f" -num_threads {cpus} -query {query} -db {subject} -out {blastfile}"
+            + " -outfmt 6 -max_target_seqs 1000 -evalue 1e-5",
+            check=False,
+            redirect_error=STDOUT,
+        )
+    except CalledProcessError as e:  # multi-threading disabled
+        message = f"{cmd} failed with message:"
+        message += "\n{0}".format(e.output.decode())
+        logging.error(message)
+        logging.fatal("Failed to run `blast`. Aborted.")
+        cleanup(blastfile)
+        sys.exit(1)
+    return blastfile
+
+
+def diamond_blastp_main(args, dbtype="prot"):
+    """
+    %prog database.fasta query.fasta
+
+    Run diamond blastp for protein alignment.
+    """
+    p = OptionParser(diamond_blastp_main.__doc__)
+
+    p.add_option("--path", help="Specify diamond path for diamond blastp")
+
+    p.set_cpus()
+    p.set_outdir()
+    p.set_params()
+
+    opts, args = p.parse_args(args)
+
+    if len(args) != 2:
+        sys.exit(not p.print_help())
+
+    subject, query = args
+    path = opts.path
+    cpus = opts.cpus
+    if not dbtype:
+        dbtype = opts.dbtype
+
+    getpath = lambda x: op.join(path, x) if path else x
+    cmd = "diamond blastp"
+    diamond_bin = getpath("diamond")
+    for bin in (diamond_bin,):
+        if not which(bin):
+            logging.fatal("`%s` not found on PATH. Have you installed Diamond?", bin)
+            sys.exit(1)
+
+    run_diamond_makedb(
+        infile=subject,
+        outfile=subject + ".dmnd",
+    )
+
+    blastfile = get_outfile(subject, query, suffix="last", outdir=opts.outdir)
+    # Make several attempts to run LASTAL
+    try:
+        sh(
+            cmd
+            + f" --threads {cpus} --query {query} --db {subject} --out {blastfile}"
+            + " --ultra-sensitive --max-target-seqs 1000 --evalue 1e-5 --outfmt 6",
+            check=False,
+            redirect_error=STDOUT,
+        )
+    except CalledProcessError as e:  # multi-threading disabled
+        message = f"{cmd} failed with message:"
+        message += "\n{0}".format(e.output.decode())
+        logging.error(message)
+        logging.fatal("Failed to run `diamond blastp`. Aborted.")
+        cleanup(blastfile)
+        sys.exit(1)
+    return blastfile
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `jcvi-1.4.2/jcvi/apps/base.py` & `jcvi-1.4.5/jcvi/apps/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,28 +21,30 @@
     NoOptionError,
     NoSectionError,
     ParsingError,
 )
 from socket import gethostname
 from subprocess import PIPE, call, check_output
 from optparse import OptionParser as OptionP, OptionGroup, SUPPRESS_HELP
-from typing import Any, Collection, List, Optional, Union
+from typing import Any, Collection, List, Optional, Tuple, Union
 
 from natsort import natsorted
 from rich.console import Console
 from rich.logging import RichHandler
 
 from jcvi import __copyright__, __version__
 
 # http://newbebweb.blogspot.com/2012/02/python-head-ioerror-errno-32-broken.html
 nobreakbuffer = lambda: signal.signal(signal.SIGPIPE, signal.SIG_DFL)
 nobreakbuffer()
 os.environ["LC_ALL"] = "C"
 JCVIHELP = "JCVI utility libraries {} [{}]\n".format(__version__, __copyright__)
 
+TextCollection = Union[str, List[str], Tuple[str, ...]]
+
 
 def debug(level=logging.DEBUG):
     """
     Turn on the debugging
     """
     logging.basicConfig(
         level=level,
@@ -1348,29 +1350,29 @@
         if op.isfile(param):
             values = list(set(x.strip() for x in open(param)))
         else:
             values = list(set(param.split(",")))
     return values
 
 
-def listify(a):
+def listify(a: TextCollection) -> TextCollection:
     """
     Convert something to a list if it is not already a list.
     """
-    return a if (isinstance(a, list) or isinstance(a, tuple)) else [a]
+    return a if isinstance(a, (list, tuple)) else [a]  # type: ignore
 
 
-def last_updated(a):
+def last_updated(a: str) -> float:
     """
     Check the time since file was last updated.
     """
     return time.time() - op.getmtime(a)
 
 
-def need_update(a: str, b: str, warn: bool = False) -> bool:
+def need_update(a: TextCollection, b: TextCollection, warn: bool = False) -> bool:
     """
     Check if file a is newer than file b and decide whether or not to update
     file b. Can generalize to two lists.
 
     Args:
         a: file or list of files
         b: file or list of files
```

### Comparing `jcvi-1.4.2/jcvi/apps/biomart.py` & `jcvi-1.4.5/jcvi/apps/biomart.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/apps/blastplus.py` & `jcvi-1.4.5/jcvi/apps/blastplus.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/apps/bowtie.py` & `jcvi-1.4.5/jcvi/apps/bowtie.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/apps/bwa.py` & `jcvi-1.4.5/jcvi/apps/bwa.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/apps/cdhit.py` & `jcvi-1.4.5/jcvi/apps/cdhit.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/apps/emboss.py` & `jcvi-1.4.5/jcvi/apps/emboss.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/apps/fetch.py` & `jcvi-1.4.5/jcvi/apps/fetch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Wrapper for fetching data from various online repositories \
 (Entrez, Ensembl, Phytozome, and SRA)
 """
+
 import logging
 import os.path as op
 import re
 import sys
 import time
 
 from os.path import join as urljoin
```

### Comparing `jcvi-1.4.2/jcvi/apps/gbsubmit.py` & `jcvi-1.4.5/jcvi/apps/gbsubmit.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/apps/gmap.py` & `jcvi-1.4.5/jcvi/apps/gmap.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/apps/grid.py` & `jcvi-1.4.5/jcvi/apps/grid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Codes to submit multiple jobs to JCVI grid engine
 """
+
 import os.path as op
 import sys
 import re
 import logging
 import platform
 
 from multiprocessing import (
```

### Comparing `jcvi-1.4.2/jcvi/apps/ks.py` & `jcvi-1.4.5/jcvi/compara/ks.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/apps/lastz.py` & `jcvi-1.4.5/jcvi/apps/lastz.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/apps/mask.py` & `jcvi-1.4.5/jcvi/apps/mask.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/apps/phylo.py` & `jcvi-1.4.5/jcvi/apps/phylo.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/apps/r.py` & `jcvi-1.4.5/jcvi/apps/r.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/apps/restriction.py` & `jcvi-1.4.5/jcvi/apps/restriction.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/apps/softlink.py` & `jcvi-1.4.5/jcvi/apps/softlink.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/apps/uclust.py` & `jcvi-1.4.5/jcvi/apps/uclust.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/apps/uniprot.py` & `jcvi-1.4.5/jcvi/apps/uniprot.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/apps/vecscreen.py` & `jcvi-1.4.5/jcvi/apps/vecscreen.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/assembly/allmaps.py` & `jcvi-1.4.5/jcvi/assembly/allmaps.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/assembly/allpaths.py` & `jcvi-1.4.5/jcvi/assembly/allpaths.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/assembly/automaton.py` & `jcvi-1.4.5/jcvi/assembly/automaton.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/assembly/base.py` & `jcvi-1.4.5/jcvi/assembly/base.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/assembly/ca.py` & `jcvi-1.4.5/jcvi/assembly/ca.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/assembly/chic.pyx` & `jcvi-1.4.5/jcvi/assembly/chic.pyx`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/assembly/coverage.py` & `jcvi-1.4.5/jcvi/assembly/coverage.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/assembly/gaps.py` & `jcvi-1.4.5/jcvi/assembly/gaps.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/assembly/geneticmap.py` & `jcvi-1.4.5/jcvi/assembly/geneticmap.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,24 +3,35 @@
 
 """
 Use genetic map to break chimeric scaffolds, order and orient scaffolds onto
 chromosomes.
 """
 import os.path as op
 import sys
-import logging
-import numpy as np
 
-from collections import Counter
-from functools import lru_cache
 from itertools import combinations, groupby
+from random import sample
+from typing import Tuple
+
+import numpy as np
+import seaborn as sns
 
-from jcvi.formats.base import BaseFile, LineFile, must_open, read_block
-from jcvi.formats.bed import Bed, fastaFromBed
-from jcvi.apps.base import OptionParser, ActionDispatcher, need_update
+from ..apps.base import OptionParser, ActionDispatcher, logger, need_update
+from ..algorithms.formula import calc_ldscore
+from ..algorithms.matrix import symmetrize
+from ..formats.base import BaseFile, LineFile, must_open, read_block
+from ..formats.bed import Bed, fastaFromBed
+from ..graphics.base import (
+    Rectangle,
+    draw_cmap,
+    normalize_axes,
+    plt,
+    plot_heatmap,
+    savefig,
+)
 
 
 MSTheader = """population_type {0}
 population_name LG
 distance_function kosambi
 cut_off_p_value 0.000001
 no_map_dist 10.0
@@ -61,18 +72,18 @@
         for lg, markers in sorted(self.items()):
             for marker, pos in markers:
                 if not switch:
                     line = (lg, pos, pos + 1, marker)
                 else:
                     seqid_spos = marker.rsplit(sep, 1)
                     if len(seqid_spos) != 2:
-                        logging.error(
-                            "Error: `{}` must be in the form e.g. `name{}position`".format(
-                                marker, sep
-                            )
+                        logger.error(
+                            "Error: `%s` must be in the form e.g. `name%sposition`",
+                            marker,
+                            sep,
                         )
                         continue
                     seqid, spos = seqid_spos
                     spos = int(spos)
                     marker = "{0}:{1}".format(lg, pos / 1000.0)
                     line = (seqid, spos - 1, spos, marker)
                 print("\t".join(str(x) for x in line), file=fw)
@@ -111,34 +122,30 @@
                 break
 
         for row in fp:
             self.append(MSTMapLine(row, startidx=startidx))
 
         self.nmarkers = len(self)
         self.nind = len(self[0].genotype)
-        logging.debug(
-            "Map contains {0} markers in {1} individuals".format(
-                self.nmarkers, self.nind
-            )
+        logger.debug(
+            "Map contains %d markers in %d individuals", self.nmarkers, self.nind
         )
 
 
 class MSTMatrix(object):
     def __init__(self, matrix, markerheader, population_type, missing_threshold):
         self.matrix = matrix
         self.markerheader = markerheader
         self.population_type = population_type
         self.missing_threshold = missing_threshold
         self.ngenotypes = len(matrix)
         self.nind = len(markerheader) - 1
         assert self.nind == len(matrix[0]) - 1
-        logging.debug(
-            "Imported {0} markers and {1} individuals.".format(
-                self.ngenotypes, self.nind
-            )
+        logger.debug(
+            "Imported %d markers and %d individuals.", self.ngenotypes, self.nind
         )
 
     def write(self, filename="stdout", header=True):
         fw = must_open(filename, "w")
         if header:
             print(
                 MSTheader.format(
@@ -153,15 +160,15 @@
         for m in self.matrix:
             print("\t".join(m), file=fw)
 
 
 def main():
     actions = (
         ("breakpoint", "find scaffold breakpoints using genetic map"),
-        ("ld", "calculate pairwise linkage disequilibrium"),
+        ("heatmap", "calculate pairwise linkage disequilibrium"),
         ("bed", "convert MSTmap output to bed format"),
         ("fasta", "extract markers based on map"),
         ("anchor", "anchor scaffolds based on map"),
         ("rename", "rename markers according to the new mapping locations"),
         ("header", "rename lines in the map header"),
         # Plot genetic map
         ("blat", "make ALLMAPS input csv based on sequences"),
@@ -319,164 +326,140 @@
     )
     ax.set_xlim(xlim)
     ax.set_ylim(ylim)
 
     title = "Alignment: {} vs {}".format(gx, gy)
     title += " ({} markers)".format(thousands(npairs))
     root.set_title(markup(title), x=0.5, y=0.96, color="k")
-    logging.debug(title)
+    logger.debug(title)
     normalize_axes(root)
 
     image_name = opts.outfile or (csvfile.rsplit(".", 1)[0] + "." + iopts.format)
     savefig(image_name, dpi=iopts.dpi, iopts=iopts)
     fig.clear()
 
 
-@lru_cache(maxsize=None)
-def calc_ldscore(a, b):
-    assert len(a) == len(b), "{0}\n{1}".format(a, b)
-    # Assumes markers as A/B
-    c = Counter(zip(a, b))
-    c_aa = c[("A", "A")]
-    c_ab = c[("A", "B")]
-    c_ba = c[("B", "A")]
-    c_bb = c[("B", "B")]
-    n = c_aa + c_ab + c_ba + c_bb
-    if n == 0:
-        return 0
-
-    f = 1.0 / n
-    x_aa = c_aa * f
-    x_ab = c_ab * f
-    x_ba = c_ba * f
-    x_bb = c_bb * f
-    p_a = x_aa + x_ab
-    p_b = x_ba + x_bb
-    q_a = x_aa + x_ba
-    q_b = x_ab + x_bb
-    D = x_aa - p_a * q_a
-    denominator = p_a * p_b * q_a * q_b
-    if denominator == 0:
-        return 0
-
-    r2 = D * D / denominator
-    return r2
-
-
-def ld(args):
+def read_subsampled_matrix(mstmap: str, subsample: int) -> Tuple[np.ndarray, str, int]:
     """
-    %prog ld map
-
-    Calculate pairwise linkage disequilibrium given MSTmap.
+    Read the subsampled matrix from file if it exists, otherwise calculate it.
     """
-    from random import sample
-    from jcvi.algorithms.matrix import symmetrize
-
-    p = OptionParser(ld.__doc__)
-    p.add_option(
-        "--subsample",
-        default=1000,
-        type="int",
-        help="Subsample markers to speed up",
-    )
-    opts, args, iopts = p.set_image_options(args, figsize="8x8")
-
-    if len(args) != 1:
-        sys.exit(not p.print_help())
-
-    (mstmap,) = args
-    subsample = opts.subsample
     data = MSTMap(mstmap)
 
-    markerbedfile = mstmap + ".subsample.bed"
-    ldmatrix = mstmap + ".subsample.matrix"
     # Take random subsample while keeping marker order
     if subsample < data.nmarkers:
         data = [data[x] for x in sorted(sample(range(len(data)), subsample))]
     else:
-        logging.debug("Use all markers, --subsample ignored")
+        logger.debug("Use all markers, --subsample ignored")
 
     nmarkers = len(data)
+    markerbedfile = mstmap + ".subsample.bed"
+    ldmatrix = mstmap + ".subsample.matrix"
     if need_update(mstmap, (ldmatrix, markerbedfile)):
-        fw = open(markerbedfile, "w")
-        print("\n".join(x.bedline for x in data), file=fw)
-        logging.debug(
-            "Write marker set of size {0} to file `{1}`.".format(
-                nmarkers, markerbedfile
+        with open(markerbedfile, "w", encoding="utf-8") as fw:
+            print("\n".join(x.bedline for x in data), file=fw)
+            logger.debug(
+                "Write marker set of size %d to file `%s`.", nmarkers, markerbedfile
             )
-        )
-        fw.close()
 
         M = np.zeros((nmarkers, nmarkers), dtype=float)
         for i, j in combinations(range(nmarkers), 2):
             a = data[i]
             b = data[j]
             M[i, j] = calc_ldscore(a.genotype, b.genotype)
 
         M = symmetrize(M)
 
-        logging.debug("Write LD matrix to file `{0}`.".format(ldmatrix))
+        logger.debug("Write LD matrix to file `%s`.", ldmatrix)
         M.tofile(ldmatrix)
     else:
         nmarkers = len(Bed(markerbedfile))
         M = np.fromfile(ldmatrix, dtype="float").reshape(nmarkers, nmarkers)
-        logging.debug("LD matrix `{0}` exists ({1}x{1}).".format(ldmatrix, nmarkers))
+        logger.debug("LD matrix `%s` exists (%dx%d).", ldmatrix, nmarkers, nmarkers)
 
-    from jcvi.graphics.base import plt, savefig, Rectangle, draw_cmap
+    return M, markerbedfile, nmarkers
 
-    plt.rcParams["axes.linewidth"] = 0
-
-    fig = plt.figure(1, (iopts.w, iopts.h))
-    root = fig.add_axes([0, 0, 1, 1])
-    ax = fig.add_axes([0.1, 0.1, 0.8, 0.8])  # the heatmap
 
-    ax.matshow(M, cmap=iopts.cmap)
+def draw_geneticmap_heatmap(root, ax, mstmap: str, subsample: int):
+    """
+    Draw the heatmap of the genetic map.
+    """
+    M, markerbedfile, nmarkers = read_subsampled_matrix(mstmap, subsample)
 
     # Plot chromosomes breaks
-    bed = Bed(markerbedfile)
-    xsize = len(bed)
+    b = Bed(markerbedfile)
+    xsize = len(b)
     extent = (0, nmarkers)
     chr_labels = []
     ignore_size = 20
 
-    for seqid, beg, end in bed.get_breaks():
+    breaks = []
+    for seqid, beg, end in b.get_breaks():
         ignore = abs(end - beg) < ignore_size
         pos = (beg + end) / 2
         chr_labels.append((seqid, pos, ignore))
         if ignore:
             continue
-        ax.plot((end, end), extent, "w-", lw=1)
-        ax.plot(extent, (end, end), "w-", lw=1)
+        breaks.append(end)
+
+    cmap = sns.color_palette("rocket", as_cmap=True)
+    plot_heatmap(ax, M, breaks, cmap=cmap, plot_breaks=True)
 
     # Plot chromosome labels
     for label, pos, ignore in chr_labels:
-        pos = 0.1 + pos * 0.8 / xsize
         if not ignore:
+            xpos = 0.1 + pos * 0.8 / xsize
             root.text(
-                pos, 0.91, label, ha="center", va="bottom", rotation=45, color="grey"
+                xpos, 0.91, label, ha="center", va="bottom", rotation=45, color="grey"
             )
-            root.text(0.09, pos, label, ha="right", va="center", color="grey")
+            ypos = 0.9 - pos * 0.8 / xsize
+            root.text(0.09, ypos, label, ha="right", va="center", color="grey")
 
     ax.set_xlim(extent)
-    ax.set_ylim(extent)
+    ax.set_ylim((nmarkers, 0))  # Invert y-axis
     ax.set_axis_off()
 
-    draw_cmap(root, "Pairwise LD (r2)", 0, 1, cmap=iopts.cmap)
+    draw_cmap(root, r"Pairwise LD ($r^2$)", 0, 1, cmap=cmap)
 
     root.add_patch(Rectangle((0.1, 0.1), 0.8, 0.8, fill=False, ec="k", lw=2))
     m = mstmap.split(".")[0]
-    root.text(
-        0.5, 0.06, "Linkage Disequilibrium between {0} markers".format(m), ha="center"
+    root.text(0.5, 0.06, f"Linkage Disequilibrium between {m} markers", ha="center")
+
+    normalize_axes(root)
+
+
+def heatmap(args):
+    """
+    %prog heatmap map
+
+    Calculate pairwise linkage disequilibrium given MSTmap.
+    """
+    p = OptionParser(heatmap.__doc__)
+    p.add_option(
+        "--subsample",
+        default=1000,
+        type="int",
+        help="Subsample markers to speed up",
     )
+    opts, args, iopts = p.set_image_options(args, figsize="8x8")
+
+    if len(args) != 1:
+        sys.exit(not p.print_help())
+
+    (mstmap,) = args
+
+    plt.rcParams["axes.linewidth"] = 0
+
+    fig = plt.figure(1, (iopts.w, iopts.h))
+    root = fig.add_axes((0, 0, 1, 1))
+    ax = fig.add_axes((0.1, 0.1, 0.8, 0.8))  # the heatmap
 
-    root.set_xlim(0, 1)
-    root.set_ylim(0, 1)
-    root.set_axis_off()
+    draw_geneticmap_heatmap(root, ax, mstmap, opts.subsample)
 
-    image_name = m + ".subsample" + "." + iopts.format
+    pf = mstmap.split(".")[0]
+    image_name = pf + ".subsample" + "." + iopts.format
     savefig(image_name, dpi=iopts.dpi, iopts=iopts)
 
 
 def header(args):
     """
     %prog header map conversion_table
 
@@ -715,15 +698,15 @@
 
         if left_label == BREAK and right_label == BREAK:
             nsingletons += 1
             continue
 
         good.append(a)
 
-    logging.debug("A total of {0} singleton markers removed.".format(nsingletons))
+    logger.debug("A total of %d singleton markers removed.", nsingletons)
 
     for a, b in pairwise(good):
         label, rr = check_markers(a, b, diff)
         if label == BREAK:
             print("\t".join(str(x) for x in rr))
```

### Comparing `jcvi-1.4.2/jcvi/assembly/goldenpath.py` & `jcvi-1.4.5/jcvi/assembly/goldenpath.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,15 +288,14 @@
         else:
             assert 0
 
         return type
 
 
 class CertificateLine(object):
-
     """
     North  chr1  2  0  AC229737.8  telomere     58443
     South  chr1  2  1  AC229737.8  AC202463.29  58443  37835  58443  + Non-terminal
     """
 
     def __init__(self, line):
         args = line.split()
```

### Comparing `jcvi-1.4.2/jcvi/assembly/hic.py` & `jcvi-1.4.5/jcvi/assembly/hic.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,49 +2,57 @@
 # -*- coding: UTF-8 -*-
 
 """
 Process Hi-C output into AGP for chromosomal-scale scaffolding.
 """
 import array
 import json
-import logging
 import math
 import os
 import os.path as op
 import sys
+
 from collections import defaultdict
 from functools import partial
 from multiprocessing import Pool
+from typing import List, Optional, Tuple
 
 import numpy as np
 
 from natsort import natsorted
 
-from jcvi.algorithms.ec import GA_run, GA_setup
-from jcvi.algorithms.formula import outlier_cutoff
-from jcvi.algorithms.matrix import get_signs
-from jcvi.apps.base import ActionDispatcher, OptionParser, backup, iglob, mkdir, symlink
-from jcvi.apps.grid import Jobs
-from jcvi.assembly.allmaps import make_movie
-from jcvi.compara.synteny import check_beds, get_bed_filenames
-from jcvi.formats.agp import order_to_agp
-from jcvi.formats.base import LineFile, must_open
-from jcvi.formats.bed import Bed
-from jcvi.formats.blast import Blast
-from jcvi.formats.sizes import Sizes
-from jcvi.graphics.base import (
+from ..algorithms.ec import GA_run, GA_setup
+from ..algorithms.formula import outlier_cutoff
+from ..algorithms.matrix import get_signs
+from ..apps.base import (
+    ActionDispatcher,
+    OptionParser,
+    backup,
+    iglob,
+    logger,
+    mkdir,
+    symlink,
+)
+from ..apps.grid import Jobs
+from ..assembly.allmaps import make_movie
+from ..compara.synteny import check_beds, get_bed_filenames
+from ..formats.agp import order_to_agp
+from ..formats.base import LineFile, must_open
+from ..formats.bed import Bed
+from ..formats.blast import Blast
+from ..formats.sizes import Sizes
+from ..graphics.base import (
     markup,
     normalize_axes,
     plt,
+    plot_heatmap,
     savefig,
-    ticker,
-    human_readable,
 )
-from jcvi.graphics.dotplot import dotplot
-from jcvi.utils.cbook import gene_name, human_size
+from ..graphics.dotplot import dotplot
+from ..utils.cbook import gene_name
 
 # Map orientations to ints
 FF = {"+": 1, "-": -1, "?": 1}
 RR = {"+": -1, "-": 1, "?": -1}
 LB = 18  # Lower bound for golden_array()
 UB = 29  # Upper bound for golden_array()
 BB = UB - LB + 1  # Span for golden_array()
@@ -124,15 +132,15 @@
         keyword, if available in the third column, is less confident.
 
         tig00015093     46912
         tig00035238     46779   recover
         tig00030900     119291
         """
         idsfile = self.idsfile
-        logging.debug("Parse idsfile `{}`".format(idsfile))
+        logger.debug("Parse idsfile `%s`", idsfile)
         fp = open(idsfile)
         tigs = []
         for row in fp:
             if row[0] == "#":  # Header
                 continue
             atoms = row.split()
             tig, _, size = atoms
@@ -148,15 +156,15 @@
         self.tig_to_size = dict(tigs)
 
         # Initially all contigs are considered active
         self.active = set(_tigs)
 
     def parse_clm(self):
         clmfile = self.clmfile
-        logging.debug("Parse clmfile `{}`".format(clmfile))
+        logger.debug("Parse clmfile `%s`", clmfile)
         fp = open(clmfile)
         contacts = {}
         contacts_oriented = defaultdict(dict)
         orientations = defaultdict(list)
         for row in fp:
             atoms = row.strip().split("\t")
             assert len(atoms) == 3, "Malformed line `{}`".format(atoms)
@@ -204,17 +212,15 @@
             s = self.tig_to_size[x]
             logd = np.log10(d * 1.0 / min(s, 500000))
             logdensities[x] = logd
 
         return logdensities
 
     def report_active(self):
-        logging.debug(
-            "Active contigs: {} (length={})".format(self.N, self.active_sizes.sum())
-        )
+        logger.debug("Active contigs: %d (length=%d)", self.N, self.active_sizes.sum())
 
     def activate(self, tourfile=None, minsize=10000, backuptour=True):
         """
         Select contigs in the current partition. This is the setup phase of the
         algorithm, and supports two modes:
 
         - "de novo": This is useful at the start of a new run where no tours
@@ -225,19 +231,19 @@
           of the pairwise strandedness matrix O.
 
         - "hotstart": This is useful when there was a past run, with a given
           tourfile. In this case, the active contig list and orientations are
           derived from the last tour in the file.
         """
         if tourfile and (not op.exists(tourfile)):
-            logging.debug("Tourfile `{}` not found".format(tourfile))
+            logger.debug("Tourfile `%s` not found", tourfile)
             tourfile = None
 
         if tourfile:
-            logging.debug("Importing tourfile `{}`".format(tourfile))
+            logger.debug("Importing tourfile `%s`", tourfile)
             tour, tour_o = iter_last_tour(tourfile, self)
             self.active = set(tour)
             tig_to_idx = self.tig_to_idx
             tour = [tig_to_idx[x] for x in tour]
             signs = sorted([(x, FF[o]) for (x, o) in zip(tour, tour_o)])
             _, signs = zip(*signs)
             self.signs = np.array(signs, dtype=int)
@@ -245,27 +251,27 @@
                 backup(tourfile)
             tour = array.array("i", tour)
         else:
             self.report_active()
             while True:
                 logdensities = self.calculate_densities()
                 lb, ub = outlier_cutoff(list(logdensities.values()))
-                logging.debug("Log10(link_densities) ~ [{}, {}]".format(lb, ub))
+                logger.debug("Log10(link_densities) ~ [%d, %d]", lb, ub)
                 remove = set(
                     x
                     for x, d in logdensities.items()
                     if (d < lb and self.tig_to_size[x] < minsize * 10)
                 )
                 if remove:
                     self.active -= remove
                     self.report_active()
                 else:
                     break
 
-            logging.debug("Remove contigs with size < {}".format(minsize))
+            logger.debug("Remove contigs with size < %d", minsize)
             self.active = set(x for x in self.active if self.tig_to_size[x] >= minsize)
             tour = range(self.N)  # Use starting (random) order otherwise
             tour = array.array("i", tour)
 
             # Determine orientations
             self.flip_all(tour)
 
@@ -294,15 +300,15 @@
         evaluation under the right condition.
         """
         from .chic import score_evaluate_Q
 
         return score_evaluate_Q(tour, self.active_sizes, self.Q)
 
     def flip_log(self, method, score, score_flipped, tag):
-        logging.debug("{}: {} => {} {}".format(method, score, score_flipped, tag))
+        logger.debug("%s: %d => %d %s", method, score, score_flipped, tag)
 
     def flip_all(self, tour):
         """Initialize the orientations based on pairwise O matrix."""
         if self.signs is None:  # First run
             score = 0
         else:
             old_signs = self.signs[: self.N]
@@ -355,24 +361,24 @@
                 score,
                 score_flipped,
                 tag,
             )
             if tag == ACCEPT:
                 any_tag_ACCEPT = True
                 score = score_flipped
-        logging.debug("FLIPONE: N_accepts={} N_rejects={}".format(n_accepts, n_rejects))
+        logger.debug("FLIPONE: N_accepts=%d N_rejects=%d", n_accepts, n_rejects)
         return ACCEPT if any_tag_ACCEPT else REJECT
 
     def prune_tour(self, tour, cpus):
         """Test deleting each contig and check the delta_score; tour here must
         be an array of ints.
         """
         while True:
             (tour_score,) = self.evaluate_tour_M(tour)
-            logging.debug("Starting score: {}".format(tour_score))
+            logger.debug("Starting score: %d", tour_score)
             active_sizes = self.active_sizes
             M = self.M
             args = []
             for i, t in enumerate(tour):
                 stour = tour[:i] + tour[i + 1 :]
                 args.append((t, stour, tour_score, active_sizes, M))
 
@@ -385,15 +391,15 @@
                 len(tour), len(results)
             )
 
             # Identify outliers
             active_contigs = self.active_contigs
             idx, log10deltas = zip(*results)
             lb, ub = outlier_cutoff(log10deltas)
-            logging.debug("Log10(delta_score) ~ [{}, {}]".format(lb, ub))
+            logger.debug("Log10(delta_score) ~ [%d, %d]", lb, ub)
 
             remove = set(active_contigs[x] for (x, d) in results if d < lb)
             self.active -= remove
             self.report_active()
 
             tig_to_idx = self.tig_to_idx
             tour = [active_contigs[x] for x in tour]
@@ -597,15 +603,15 @@
         sum_logX += logXs
         sum_logY += logYs
 
     B = (N * sum_logXlogY - sum_logX * sum_logY) / (
         N * sum_logXlogX - sum_logX * sum_logX
     )
     A = math.exp((sum_logY - B * sum_logX) / N)
-    logging.debug("Power law Y = {:.1f} * X ^ {:.4f}".format(A, B))
+    logger.debug("Power law Y = %.1f * X ^ %.4f", A, B)
     label = "$Y={:.1f} \\times X^{{ {:.4f} }}$".format(A, B)
     return A, B, label
 
 
 def dist(args):
     """
     %prog dist input.dist.npy genome.json
@@ -642,15 +648,15 @@
     df["BinStart"] = distbin_starts[xstart:xend]
     df["LinkDensity"] = a[xstart:xend] / distbin_sizes[xstart:xend]
     ax = sns.lineplot(
         x="BinStart", y="LinkDensity", data=df, lw=3, color="lightslategray"
     )
     tx = df["BinStart"]
     A, B, label = fit_power_law(tx, df["LinkDensity"])
-    ty = A * tx ** B
+    ty = A * tx**B
     ax.plot(tx, ty, "r:", lw=3, label=label)
     ax.legend()
     if opts.title:
         ax.set_title(markup(opts.title))
     ax.set_xlabel("Link size (bp)")
     ax.set_ylabel(r"Density (\# of links per bp)")
     ax.set_xscale("log", nonposx="clip")
@@ -675,71 +681,38 @@
     data = []
     with open(groupsfile) as fp:
         for row in fp:
             seqids, color = row.split()
             yield seqids, color
 
 
-def heatmap(args):
+def read_matrix(
+    npyfile: str,
+    header: dict,
+    contig: Optional[str],
+    groups: List[Tuple[str, str]],
+    vmin: int,
+    vmax: int,
+    plot_breaks: bool,
+):
     """
-    %prog heatmap input.npy genome.json
-
-    Plot heatmap based on .npy data file. The .npy stores a square matrix with
-    bins of genome, and cells inside the matrix represent number of links
-    between bin i and bin j. The `genome.json` contains the offsets of each
-    contig/chr so that we know where to draw boundary lines, or extract per
-    contig/chromosome heatmap.
-
-    If a 'groups' file is given (with --groups), we will draw squares on the
-    heatmap. The 'groups' file has the following format, for example:
-
-    seq1,seq2 b
-    seq1 g
-    seq2 g
-
-    This will first draw a square around seq1+seq2 with blue color, then seq1
-    and seq2 individually with green color.
+    Read the matrix from the npy file and apply log transformation and thresholding.
     """
-    p = OptionParser(heatmap.__doc__)
-    p.add_option("--title", help="Title of the heatmap")
-    p.add_option("--groups", help="Groups file, see doc")
-    p.add_option("--vmin", default=1, type="int", help="Minimum value in the heatmap")
-    p.add_option("--vmax", default=6, type="int", help="Maximum value in the heatmap")
-    p.add_option("--chr", help="Plot this contig/chr only")
-    p.add_option(
-        "--nobreaks",
-        default=False,
-        action="store_true",
-        help="Do not plot breaks (esp. if contigs are small)",
-    )
-    opts, args, iopts = p.set_image_options(
-        args, figsize="11x11", style="white", cmap="coolwarm", format="png", dpi=120
-    )
-
-    if len(args) != 2:
-        sys.exit(not p.print_help())
-
-    npyfile, jsonfile = args
-    contig = opts.chr
-    groups = list(generate_groups(opts.groups)) if opts.groups else []
-
-    # Load contig/chromosome starts and sizes
-    header = json.loads(open(jsonfile).read())
-    resolution = header.get("resolution")
-    assert resolution is not None, "`resolution` not found in `{}`".format(jsonfile)
-    logging.debug("Resolution set to {}".format(resolution))
     # Load the matrix
     A = np.load(npyfile)
+    total_bins = header["total_bins"]
 
     # Select specific submatrix
     if contig:
         contig_start = header["starts"][contig]
         contig_size = header["sizes"][contig]
         contig_end = contig_start + contig_size
         A = A[contig_start:contig_end, contig_start:contig_end]
+    else:
+        A = A[:total_bins, :total_bins]
 
     # Convert seqids to positions for each group
     new_groups = []
     for seqids, color in groups:
         seqids = seqids.split(",")
         assert all(
             x in header["starts"] for x in seqids
@@ -758,53 +731,136 @@
 
     # Several concerns in practice:
     # The diagonal counts may be too strong, this can either be resolved by
     # masking them. Or perform a log transform on the entire heatmap.
     B = A.astype("float64")
     B += 1.0
     B = np.log(B)
-    vmin, vmax = opts.vmin, opts.vmax
     B[B < vmin] = vmin
     B[B > vmax] = vmax
     print(B)
-    logging.debug(
-        "Matrix log-transformation and thresholding ({}-{}) done".format(vmin, vmax)
-    )
-
-    # Canvas
-    fig = plt.figure(1, (iopts.w, iopts.h))
-    root = fig.add_axes([0, 0, 1, 1])  # whole canvas
-    ax = fig.add_axes([0.05, 0.05, 0.9, 0.9])  # just the heatmap
+    logger.debug("Matrix log-transformation and thresholding (%d-%d) done", vmin, vmax)
 
     breaks = list(header["starts"].values())
-    breaks += [header["total_bins"]]  # This is actually discarded
+    breaks += [total_bins]  # This is actually discarded
     breaks = sorted(breaks)[1:]
-    if contig or opts.nobreaks:
+    if contig or not plot_breaks:
         breaks = []
-    plot_heatmap(ax, B, breaks, iopts, groups=new_groups, binsize=resolution)
+
+    return B, new_groups, breaks
+
+
+def draw_hic_heatmap(
+    root,
+    ax,
+    npyfile: str,
+    jsonfile: str,
+    contig: Optional[str],
+    groups_file: str,
+    title: str,
+    vmin: int,
+    vmax: int,
+    plot_breaks: bool,
+):
+    """
+    Draw heatmap based on .npy file. The .npy file stores a square matrix with
+    bins of genome, and cells inside the matrix represent number of links
+    between bin i and bin j. The `genome.json` contains the offsets of each
+    contig/chr so that we know where to draw boundary lines, or extract per
+    contig/chromosome heatmap.
+    """
+    groups = list(generate_groups(groups_file)) if groups_file else []
+
+    # Load contig/chromosome starts and sizes
+    header = json.loads(open(jsonfile, encoding="utf-8").read())
+    resolution = header.get("resolution")
+    assert resolution is not None, "`resolution` not found in `{}`".format(jsonfile)
+    logger.debug("Resolution set to %d", resolution)
+
+    B, new_groups, breaks = read_matrix(
+        npyfile, header, contig, groups, vmin, vmax, plot_breaks
+    )
+    plot_heatmap(ax, B, breaks, groups=new_groups, binsize=resolution)
 
     # Title
-    pf = npyfile.rsplit(".", 1)[0]
-    title = opts.title
     if contig:
-        title += "-{}".format(contig)
+        title += f"-{contig}"
     root.text(
         0.5,
-        0.98,
+        0.96,
         markup(title),
         color="darkslategray",
-        size=18,
         ha="center",
         va="center",
     )
 
     normalize_axes(root)
+
+
+def heatmap(args):
+    """
+    %prog heatmap input.npy genome.json
+
+    Plot heatmap based on .npy data file. The .npy stores a square matrix with
+    bins of genome, and cells inside the matrix represent number of links
+    between bin i and bin j. The `genome.json` contains the offsets of each
+    contig/chr so that we know where to draw boundary lines, or extract per
+    contig/chromosome heatmap.
+
+    If a 'groups' file is given (with --groups), we will draw squares on the
+    heatmap. The 'groups' file has the following format, for example:
+
+    seq1,seq2 b
+    seq1 g
+    seq2 g
+
+    This will first draw a square around seq1+seq2 with blue color, then seq1
+    and seq2 individually with green color.
+    """
+    p = OptionParser(heatmap.__doc__)
+    p.add_option("--title", help="Title of the heatmap")
+    p.add_option("--groups", help="Groups file, see doc")
+    p.add_option("--vmin", default=1, type="int", help="Minimum value in the heatmap")
+    p.add_option("--vmax", default=6, type="int", help="Maximum value in the heatmap")
+    p.add_option("--chr", help="Plot this contig/chr only")
+    p.add_option(
+        "--nobreaks",
+        default=False,
+        action="store_true",
+        help="Do not plot breaks (esp. if contigs are small)",
+    )
+    opts, args, iopts = p.set_image_options(
+        args, figsize="11x11", style="white", cmap="coolwarm", dpi=120
+    )
+
+    if len(args) != 2:
+        sys.exit(not p.print_help())
+
+    npyfile, jsonfile = args
+    # Canvas
+    fig = plt.figure(1, (iopts.w, iopts.h))
+    root = fig.add_axes((0, 0, 1, 1))  # whole canvas
+    ax = fig.add_axes((0.05, 0.05, 0.9, 0.9))  # just the heatmap
+
+    draw_hic_heatmap(
+        root,
+        ax,
+        npyfile,
+        jsonfile,
+        contig=opts.chr,
+        groups_file=opts.groups,
+        title=opts.title,
+        vmin=opts.vmin,
+        vmax=opts.vmax,
+        plot_breaks=not opts.nobreaks,
+    )
+
+    pf = npyfile.rsplit(".", 1)[0]
     image_name = pf + "." + iopts.format
     # macOS sometimes has way too verbose output
-    logging.getLogger().setLevel(logging.CRITICAL)
     savefig(image_name, dpi=iopts.dpi, iopts=iopts)
 
 
 def mergemat(args):
     """
     %prog mergemat *.npy
 
@@ -815,25 +871,23 @@
     opts, args = p.parse_args(args)
 
     if len(args) < 1:
         sys.exit(not p.print_help())
 
     npyfiles = args
     A = np.load(npyfiles[0])
-    logging.debug(
-        "Load `{}`: matrix of shape {}:; sum={}".format(npyfiles[0], A.shape, A.sum())
-    )
+    logger.debug("Load `%s`: matrix of shape %s; sum=%d", npyfiles[0], A.shape, A.sum())
     for npyfile in npyfiles[1:]:
         B = np.load(npyfile)
         A += B
-        logging.debug("Load `{}`: sum={}".format(npyfiles[0], A.sum()))
+        logger.debug("Load `%s`: sum=%d", npyfiles[0], A.sum())
 
     pf = opts.outfile
     np.save(pf, A)
-    logging.debug("Combined {} files into `{}.npy`".format(len(npyfiles), pf))
+    logger.debug("Combined %d files into `%s.npy`", len(npyfiles), pf)
 
 
 def get_seqstarts(bamfile, N, seqids=None):
     """Go through the SQ headers and pull out all sequences with size
     greater than the resolution settings, i.e. contains at least a few cells
     """
     import pysam
@@ -930,18 +984,18 @@
     def default(o):
         if isinstance(o, np.int64):
             return int(o)
         raise TypeError
 
     json.dump(header, fwjson, sort_keys=True, indent=4, default=default)
     fwjson.close()
-    logging.debug("Contig bin starts written to `{}`".format(jsonfile))
+    logger.debug("Contig bin starts written to `%s`", jsonfile)
 
     print(sorted(seqstarts.items(), key=lambda x: x[-1]))
-    logging.debug("Initialize matrix of size {}x{}".format(total_bins, total_bins))
+    logger.debug("Initialize matrix of size %dx%d", total_bins, total_bins)
     A = np.zeros((total_bins, total_bins), dtype="int")
     B = np.zeros(bins, dtype="int")
 
     # Find the bin ID of each read
     def bin_number(chr, pos):
         return seqstarts[chr] + pos // N
 
@@ -985,20 +1039,20 @@
         abin, bbin = bin_number(achr, apos), bin_number(bchr, bpos)
         A[abin, bbin] += 1
         if abin != bbin:
             A[bbin, abin] += 1
 
         k += 1
 
-    logging.debug("Total reads counted: {}".format(percentage(2 * k, j)))
+    logger.debug("Total reads counted: %s", percentage(2 * k, j))
     bamfile.close()
     np.save(pf, A)
-    logging.debug("Link counts written to `{}.npy`".format(pf))
+    logger.debug("Link counts written to `%s.npy`", pf)
     np.save(pf + ".dist", B)
-    logging.debug("Link dists written to `{}.dist.npy`".format(pf))
+    logger.debug("Link dists written to `%s.dist.npy`", pf)
 
 
 def simulate(args):
     """
     %prog simulate test
 
     Simulate CLM and IDS files with given names.
@@ -1035,15 +1089,15 @@
     ContigStarts[1:] = np.cumsum(ContigSizes)[:-1]
 
     # Write IDS file
     idsfile = pf + ".ids"
     fw = open(idsfile, "w")
     print("#Contig\tRECounts\tLength", file=fw)
     for i, s in enumerate(ContigSizes):
-        print("tig{:04d}\t{}\t{}".format(i, s // (4 ** 4), s), file=fw)
+        print("tig{:04d}\t{}\t{}".format(i, s // (4**4), s), file=fw)
     fw.close()
 
     # Simulate the gene positions
     GenePositions = np.sort(np.random.randint(0, GenomeSize, size=Genes))
     write_last_and_beds(pf, GenePositions, ContigStarts)
 
     # Simulate links, uniform start, with link distances following 1/x, where x
@@ -1186,15 +1240,15 @@
         logdensities = clm.calculate_densities()
         densityfile = pf + ".density"
         fw = open(densityfile, "w")
         for name, logd in logdensities.items():
             s = clm.tig_to_size[name]
             print("\t".join(str(x) for x in (name, s, logd)), file=fw)
         fw.close()
-        logging.debug("Density written to `{}`".format(densityfile))
+        logger.debug("Density written to `%s`", densityfile)
 
     tourfile = clmfile.rsplit(".", 1)[0] + ".tour"
     tour = clm.activate(tourfile=tourfile, backuptour=False)
     clm.flip_all(tour)
     clm.flip_whole(tour)
     clm.flip_one(tour)
 
@@ -1249,15 +1303,15 @@
             tour = clm.prune_tour(tour, cpus)
 
     # Flip orientations
     phase = 1
     while True:
         tag1, tag2 = optimize_orientations(fwtour, clm, phase, cpus)
         if tag1 == REJECT and tag2 == REJECT:
-            logging.debug("Terminating ... no more {}".format(ACCEPT))
+            logger.debug("Terminating ... no more %s", ACCEPT)
             break
         phase += 1
 
     fwtour.close()
 
 
 def optimize_ordering(fwtour, clm, phase, cpus):
@@ -1329,15 +1383,15 @@
 
     qbed = Bed(qbedfile, sorted=False)
     contig_to_beds = dict(qbed.sub_beds())
 
     # Create a separate directory for the subplots and movie
     mkdir(odir, overwrite=True)
     os.chdir(odir)
-    logging.debug("Change into subdir `{}`".format(odir))
+    logger.debug("Change into subdir `%s`", odir)
 
     # Make anchorsfile
     anchorsfile = ".".join(op.basename(lastfile).split(".", 2)[:2]) + ".anchors"
     fw = open(anchorsfile, "w")
     for b in Blast(lastfile):
         print(
             "\t".join((gene_name(b.query), gene_name(b.subject), str(int(b.score)))),
@@ -1377,18 +1431,16 @@
     """
     row = open(tourfile).readlines()[-1]
     _tour, _tour_o = separate_tour_and_o(row)
     tour = []
     tour_o = []
     for tc, to in zip(_tour, _tour_o):
         if tc not in clm.contigs:
-            logging.debug(
-                "Contig `{}` in file `{}` not found in `{}`".format(
-                    tc, tourfile, clm.idsfile
-                )
+            logger.debug(
+                "Contig `%s` in file `%s` not found in `%s`", tc, tourfile, clm.idsfile
             )
             continue
         tour.append(tc)
         tour_o.append(to)
     return tour, tour_o
 
 
@@ -1630,21 +1682,21 @@
     label = opts.label or op.basename(image_name).rsplit(".", 1)[0]
 
     clm = CLMFile(clmfile)
     totalbins, bins, breaks = make_bins(tour, clm.tig_to_size)
     M = read_clm(clm, totalbins, bins)
 
     fig = plt.figure(1, (iopts.w, iopts.h))
-    root = fig.add_axes([0, 0, 1, 1])  # whole canvas
-    ax1 = fig.add_axes([0.05, 0.1, 0.4, 0.8])  # heatmap
-    ax2 = fig.add_axes([0.55, 0.1, 0.4, 0.8])  # dot plot
-    ax2_root = fig.add_axes([0.5, 0, 0.5, 1])  # dot plot canvas
+    root = fig.add_axes((0, 0, 1, 1))  # whole canvas
+    ax1 = fig.add_axes((0.05, 0.1, 0.4, 0.8))  # heatmap
+    ax2 = fig.add_axes((0.55, 0.1, 0.4, 0.8))  # dot plot
+    ax2_root = fig.add_axes((0.5, 0, 0.5, 1))  # dot plot canvas
 
     # Left axis: heatmap
-    plot_heatmap(ax1, M, breaks, iopts)
+    plot_heatmap(ax1, M, breaks, binsize=BINSIZE)
 
     # Right axis: synteny
     qbed, sbed, qorder, sorder, is_self = check_beds(anchorsfile, p, opts, sorted=False)
     dotplot(anchorsfile, qbed, sbed, fig, ax2_root, ax2, sep=False, title="")
 
     root.text(0.5, 0.98, clm.name, color="g", ha="center", va="center")
     root.text(0.5, 0.95, label, color="darkslategray", ha="center", va="center")
@@ -1677,67 +1729,14 @@
         M[xstart:xend, ystart:yend] = z
         M[ystart:yend, xstart:xend] = z
 
     M = np.log10(M + 1)
     return M
 
 
-def plot_heatmap(ax, M, breaks, iopts, groups=[], plot_breaks=False, binsize=BINSIZE):
-    """Plot heatmap illustrating the contact probabilities in Hi-C data.
-
-    Args:
-        ax (pyplot.axes): Matplotlib axis
-        M (np.array): 2D numpy-array
-        breaks (List[int]): Positions of chromosome starts. Can be None.
-        iopts (OptionParser options): Graphical options passed in from commandline
-        groups (List, optional): [(start, end, [(position, seqid)], color)]. Defaults to [].
-        plot_breaks (bool): Whether to plot white breaks. Defaults to False.
-        binsize (int, optional): Resolution of the heatmap. Defaults to BINSIZE.
-    """
-    import seaborn as sns
-
-    cmap = sns.cubehelix_palette(rot=0.5, as_cmap=True)
-    ax.imshow(M, cmap=cmap, interpolation="none")
-    _, xmax = ax.get_xlim()
-    xlim = (0, xmax)
-    if plot_breaks:
-        for b in breaks[:-1]:
-            ax.plot([b, b], xlim, "w-")
-            ax.plot(xlim, [b, b], "w-")
-
-    def simplify_seqid(seqid):
-        seqid = seqid.replace("_", "")
-        if seqid[:3].lower() == "chr":
-            seqid = seqid[3:]
-        return seqid.lstrip("0")
-
-    for start, end, position_seqids, color in groups:
-        # Plot a square
-        ax.plot([start, start], [start, end], "-", color=color)
-        ax.plot([start, end], [start, start], "-", color=color)
-        ax.plot([start, end], [end, end], "-", color=color)
-        ax.plot([end, end], [start, end], "-", color=color)
-        for position, seqid in position_seqids:
-            seqid = simplify_seqid(seqid)
-            ax.text(position, end, seqid, ha="center", va="top")
-
-    ax.set_xlim(xlim)
-    ax.set_ylim((xlim[1], xlim[0]))  # Flip the y-axis so the origin is at the top
-    ax.set_xticklabels(ax.get_xticks(), family="Helvetica", color="gray")
-    ax.set_yticklabels(ax.get_yticks(), family="Helvetica", color="gray", rotation=90)
-    ax.tick_params(left=True, bottom=True, labelleft=True, labelbottom=True)
-    formatter = ticker.FuncFormatter(
-        lambda x, pos: human_readable(int(x) * binsize, pos, base=True)
-    )
-    ax.xaxis.set_major_formatter(formatter)
-    ax.yaxis.set_major_formatter(formatter)
-    binlabel = "Resolution = {} per bin".format(human_size(binsize, precision=0))
-    ax.set_xlabel(binlabel)
-
-
 def agp(args):
     """
     %prog agp main_results/ contigs.fasta
 
     Generate AGP file based on LACHESIS output.
     """
     p = OptionParser(agp.__doc__)
@@ -1757,15 +1756,15 @@
     for ofile in orderingfiles:
         co = ContigOrdering(ofile)
         anchored |= set([x.contig_name for x in co])
         obj = op.basename(ofile).split(".")[0]
         co.write_agp(obj, sizes, fwagp)
 
     singletons = contigs - anchored
-    logging.debug("Anchored: {}, Singletons: {}".format(len(anchored), len(singletons)))
+    logger.debug("Anchored: %d, Singletons: %d", len(anchored), len(singletons))
 
     for s in natsorted(singletons):
         order_to_agp(s, [(s, "?")], sizes, fwagp)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `jcvi-1.4.2/jcvi/assembly/kmer.py` & `jcvi-1.4.5/jcvi/assembly/kmer.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,40 +2,48 @@
 # -*- coding: UTF-8 -*-
 
 """
 Deals with K-mers and K-mer distribution from reads or genome
 """
 import os.path as op
 import sys
-import logging
 import math
-import numpy as np
 
 from collections import defaultdict
-from more_itertools import chunked
 from typing import List
 
-from jcvi.graphics.base import (
-    plt,
+import numpy as np
+from more_itertools import chunked
+
+from ..apps.grid import MakeManager
+from ..apps.base import (
+    ActionDispatcher,
+    OptionParser,
+    PIPE,
+    Popen,
+    logger,
+    need_update,
+    sh,
+)
+from ..formats.fasta import Fasta
+from ..formats.base import BaseFile, must_open, get_number
+from ..graphics.base import (
     adjust_spines,
     asciiplot,
-    set_human_axis,
-    savefig,
     markup,
-    panel_labels,
     normalize_axes,
+    panel_labels,
+    plt,
+    savefig,
+    set_human_axis,
     set_ticklabels_helvetica,
     write_messages,
 )
-from jcvi.formats.fasta import Fasta
-from jcvi.formats.base import BaseFile, must_open, get_number
-from jcvi.utils.cbook import thousands, percentage
-from jcvi.assembly.automaton import iter_project
-from jcvi.apps.grid import MakeManager
-from jcvi.apps.base import OptionParser, ActionDispatcher, sh, need_update, Popen, PIPE
+from ..utils.cbook import thousands, percentage
+from .automaton import iter_project
 
 
 KMERYL, KSOAP, KALLPATHS = range(3)
 
 
 class KmerSpectrum(BaseFile):
     def __init__(self, histfile):
@@ -44,15 +52,15 @@
 
     def load_data(self, histfile):
         self.data = []
         self.totalKmers = 0
         self.hist = {}
         kformat = self.guess_format(histfile)
         kformats = ("Meryl", "Soap", "AllPaths")
-        logging.debug("Guessed format: {0}".format(kformats[kformat]))
+        logger.debug("Guessed format: %s", kformats[kformat])
 
         fp = open(histfile)
         for rowno, row in enumerate(fp):
             if row[0] == "#":
                 continue
             if kformat == KSOAP:
                 K = rowno + 1
@@ -266,33 +274,29 @@
         copy_messages = []
         for i, g in enumerate(GG):
             start, end = bins[i]
             mid = (start + end) / 2
             copy_num = start if start == end else "{}-{}".format(start, end)
             g_copies = int(round(g * mid * (end - start + 1)))
             copy_series.append((mid, copy_num, g_copies, g))
-            copy_message = "CN {}: {:.1f} Mb ({:.1f} percent)".format(
-                copy_num, g_copies / 1e6, g_copies * 100 / genome_size
-            )
+            copy_message = f"CN {copy_num}: {g_copies / 1e6:.1f} Mb ({ g_copies * 100 / genome_size:.1f} percent)"
             copy_messages.append(copy_message)
             m += copy_message + "\n"
 
         if genome_size > inferred_genome_size:
             g_copies = genome_size - inferred_genome_size
             copy_num = "{}+".format(end + 1)
             copy_series.append((end + 1, copy_num, g_copies, g_copies / (end + 1)))
-            m += "CN {}: {:.1f} Mb ({:.1f} percent)\n".format(
-                copy_num, g_copies / 1e6, g_copies * 100 / genome_size
-            )
+            m += f"CN {copy_num}: {g_copies / 1e6:.1f} Mb ({ g_copies * 100 / genome_size:.1f} percent)\n"
 
         # Determine ploidy
         def determine_ploidy(copy_series, threshold=0.15):
             counts_so_far = 1
             ploidy_so_far = 0
-            for mid, copy_num, g_copies, g in copy_series:
+            for mid, _, g_copies, _ in copy_series:
                 if g_copies / counts_so_far < threshold:
                     break
                 counts_so_far += g_copies
                 ploidy_so_far = mid
             return int(ploidy_so_far)
 
         ploidy = determine_ploidy(copy_series)
@@ -300,15 +304,15 @@
         self.ploidy_message = "Ploidy: {}".format(ploidy)
         m += self.ploidy_message + "\n"
         self.copy_messages = copy_messages[:ploidy]
 
         # Repeat content
         def calc_repeats(copy_series, ploidy, genome_size):
             unique = 0
-            for mid, copy_num, g_copies, g in copy_series:
+            for mid, _, g_copies, _ in copy_series:
                 if mid <= ploidy:
                     unique += g_copies
                 else:
                     break
             return 1 - unique / genome_size
 
         repeats = calc_repeats(copy_series, ploidy, genome_size)
@@ -351,17 +355,18 @@
         """
         from math import sqrt
 
         data = self.data
         kf_ceil = max(K for (K, c) in data)
         if kf_ceil > covmax:
             exceeds = sum(1 for (K, c) in data if K > covmax)
-            logging.debug(
-                "A total of {0} distinct K-mers appear > "
-                "{1} times. Ignored ...".format(exceeds, covmax)
+            logger.debug(
+                "A total of %d distinct K-mers appear > %d times. Ignored ...",
+                exceeds,
+                covmax,
             )
             kf_ceil = covmax
 
         nkf = kf_ceil + 1
         a = [0] * nkf
         for kf, c in data:
             if kf > kf_ceil:
@@ -509,15 +514,15 @@
         op = " + sum " if action == "union" else " * "
         mm = MakeManager()
         if batch > 1:
             filename = outfile + ".{}.def"
             # Divide indices into batches
             batches = []
             batchsize = (len(self.indices) + batch - 1) // batch
-            logging.debug("Use batchsize of %d", batchsize)
+            logger.debug("Use batchsize of %d", batchsize)
             for i, indices in enumerate(chunked(self.indices, batchsize)):
                 filename_i = filename.format(i + 1)
                 outfile_i = outfile + ".{}".format(i + 1)
                 self.write_definitions(
                     filename_i, indices, outfile_i, op, ci_in=ci_in, ci_out=0
                 )
                 cmd = "kmc_tools complex {}".format(filename_i)
@@ -656,15 +661,15 @@
     for row in fp:
         kmer = row.split()[0]
         kmer_rc = rc(kmer)
         KMERS.add(kmer)
         KMERS.add(kmer_rc)
 
     K = len(kmer)
-    logging.debug("Imported {} {}-mers".format(len(KMERS), K))
+    logger.debug("Imported %d %d-mers", len(KMERS), K)
 
     for name, seq in parse_fasta(fastafile):
         name = name.split()[0]
         for i in range(len(seq) - K):
             if i % 5000000 == 0:
                 print("{}:{}".format(name, i), file=sys.stderr)
             kmer = seq[i : i + K]
@@ -719,15 +724,15 @@
     indices = args
     if opts.exclude:
         before = set(indices)
         exclude_ids = set(x.strip() for x in open(opts.exclude))
         indices = [x for x in indices if x.rsplit(".", 2)[0] not in exclude_ids]
         after = set(indices)
         if before > after:
-            logging.debug(
+            logger.debug(
                 "Excluded accessions %d → %d (%s)",
                 len(before),
                 len(after),
                 ",".join(before - after),
             )
     if opts.action == "reduce":
         mm = MakeManager()
@@ -964,37 +969,39 @@
     t.flush()
 
     f = Fasta(fastafile, lazy=True)
     for name, rec in f.iteritems_ordered():
         kmers = list(make_kmers(rec.seq, K))
         print("\n".join(kmers), file=proc.stdin)
     proc.stdin.close()
-    logging.debug(cmd)
+    logger.debug(cmd)
     proc.wait()
 
     a = bitarray()
     binfile = ".".join((fastafile, jfdb, "bin"))
     fw = open(binfile, "w")
     t.seek(0)
     for row in t:
         c = row.strip()
         a.append(int(c))
     a.tofile(fw)
-    logging.debug("Serialize {0} bits to `{1}`.".format(len(a), binfile))
+    logger.debug("Serialize %d bits to `%s`.", len(a), binfile)
     fw.close()
     sh("rm {0}".format(t.name))
 
-    logging.debug(
-        "Shared K-mers (K={0}) between `{1}` and `{2}` written to `{3}`.".format(
-            K, fastafile, jfdb, binfile
-        )
+    logger.debug(
+        "Shared K-mers (K=%d) between `%s` and `%s` written to `%s`.",
+        K,
+        fastafile,
+        jfdb,
+        binfile,
     )
     cntfile = ".".join((fastafile, jfdb, "cnt"))
     bincount([fastafile, binfile, "-o", cntfile, "-K {0}".format(K)])
-    logging.debug("Shared K-mer counts written to `{0}`.".format(cntfile))
+    logger.debug("Shared K-mer counts written to `%s`.", cntfile)
 
 
 def bincount(args):
     """
     %prog bincount fastafile binfile
 
     Count K-mers in the bin.
@@ -1120,18 +1127,18 @@
 
     totalfilesize = sum(getfilesize(x) for x in fastqfiles)
     fq = fastqfiles[0]
     pf = opts.prefix
     gzip = fq.endswith(".gz")
 
     hashsize = totalfilesize / coverage
-    logging.debug(
-        "Total file size: {0}, hashsize (-s): {1}".format(
-            human_size(totalfilesize, a_kilobyte_is_1024_bytes=True), hashsize
-        )
+    logger.debug(
+        "Total file size: %s, hashsize (-s): %d",
+        human_size(totalfilesize, a_kilobyte_is_1024_bytes=True),
+        hashsize,
     )
 
     jfpf = "{0}-K{1}".format(pf, K)
     jfdb = jfpf
     fastqfiles = " ".join(fastqfiles)
 
     jfcmd = op.join(opts.jellyfish_home, "jellyfish")
@@ -1152,28 +1159,14 @@
     jfhisto = jfpf + ".histogram"
     cmd = jfcmd + " histo -t 64 {0} -o {1}".format(jfdb, jfhisto)
 
     if need_update(jfdb, jfhisto):
         sh(cmd)
 
 
-def merylhistogram(merylfile):
-    """
-    Run meryl to dump histogram to be used in kmer.histogram(). The merylfile
-    are the files ending in .mcidx or .mcdat.
-    """
-    pf, sf = op.splitext(merylfile)
-    outfile = pf + ".histogram"
-    if need_update(merylfile, outfile):
-        cmd = "meryl -Dh -s {0}".format(pf)
-        sh(cmd, outfile=outfile)
-
-    return outfile
-
-
 def multihistogram(args):
     """
     %prog multihistogram *.histogram species
 
     Plot the histogram based on a set of K-mer hisotograms. The method is based
     on Star et al.'s method (Atlantic Cod genome paper).
     """
@@ -1186,17 +1179,17 @@
 
     if len(args) < 1:
         sys.exit(not p.print_help())
 
     histfiles = args[:-1]
     species = args[-1]
     fig = plt.figure(1, (iopts.w, iopts.h))
-    root = fig.add_axes([0, 0, 1, 1])
-    A = fig.add_axes([0.08, 0.12, 0.38, 0.76])
-    B = fig.add_axes([0.58, 0.12, 0.38, 0.76])
+    root = fig.add_axes((0, 0, 1, 1))
+    A = fig.add_axes((0.08, 0.12, 0.38, 0.76))
+    B = fig.add_axes((0.58, 0.12, 0.38, 0.76))
 
     lines = []
     legends = []
     genomesizes = []
     for histfile in histfiles:
         ks = KmerSpectrum(histfile)
         x, y = ks.get_xy(opts.vmin, opts.vmax)
@@ -1237,47 +1230,149 @@
     panel_labels(root, labels)
 
     normalize_axes(root)
     imagename = species + ".multiK.pdf"
     savefig(imagename, dpi=iopts.dpi, iopts=iopts)
 
 
+def plot_nbinom_fit(ax, ks: KmerSpectrum, ymax: float, method_info: dict):
+    """
+    Plot the negative binomial fit.
+    """
+    generative_model = method_info["generative_model"]
+    GG = method_info["Gbins"]
+    ll = method_info["lambda"]
+    rr = method_info["rho"]
+    kf_range = method_info["kf_range"]
+    stacked = generative_model(GG, ll, rr)
+    ax.plot(
+        kf_range,
+        stacked,
+        ":",
+        color="#6a3d9a",
+        lw=2,
+    )
+    # Plot multiple CN locations, CN1, CN2, ... up to ploidy
+    cn_color = "#a6cee3"
+    for i in range(1, ks.ploidy + 1):
+        x = i * ks.lambda_
+        ax.plot((x, x), (0, ymax), "-.", color=cn_color)
+        ax.text(
+            x,
+            ymax * 0.95,
+            f"CN{i}",
+            ha="right",
+            va="center",
+            color=cn_color,
+            rotation=90,
+        )
+
+
+def draw_ks_histogram(
+    ax,
+    histfile: str,
+    method: str,
+    coverage: int,
+    vmin: int,
+    vmax: int,
+    species: str,
+    K: int,
+    maxiter: int,
+    peaks: bool,
+) -> int:
+    """
+    Draw the K-mer histogram.
+    """
+    ks = KmerSpectrum(histfile)
+    method_info = ks.analyze(K=K, maxiter=maxiter, method=method)
+
+    Total_Kmers = int(ks.totalKmers)
+    Kmer_coverage = ks.lambda_ if not coverage else coverage
+    Genome_size = int(round(Total_Kmers * 1.0 / Kmer_coverage))
+
+    Total_Kmers_msg = f"Total {K}-mers: {thousands(Total_Kmers)}"
+    Kmer_coverage_msg = f"{K}-mer coverage: {Kmer_coverage:.1f}x"
+    Genome_size_msg = f"Estimated genome size: {Genome_size / 1e6:.1f} Mb"
+    Repetitive_msg = ks.repetitive
+    SNPrate_msg = ks.snprate
+
+    messages = [
+        Total_Kmers_msg,
+        Kmer_coverage_msg,
+        Genome_size_msg,
+        Repetitive_msg,
+        SNPrate_msg,
+    ]
+    for msg in messages:
+        print(msg, file=sys.stderr)
+
+    x, y = ks.get_xy(vmin, vmax)
+    title = f"{species} {K}-mer histogram"
+
+    ax.bar(x, y, fc="#b2df8a", lw=0)
+
+    if peaks:  # Only works for method 'allpaths'
+        t = (ks.min1, ks.max1, ks.min2, ks.max2, ks.min3)
+        tcounts = [(x, y) for x, y in ks.counts if x in t]
+        if tcounts:
+            x, y = zip(*tcounts)
+            tcounts = dict(tcounts)
+            ax.plot(x, y, "ko", lw=3, mec="k", mfc="w")
+            ax.text(ks.max1, tcounts[ks.max1], "SNP peak")
+            ax.text(ks.max2, tcounts[ks.max2], "Main peak")
+
+    _, ymax = ax.get_ylim()
+    ymax *= 7 / 6
+    # Plot the negative binomial fit
+    if method == "nbinom":
+        plot_nbinom_fit(ax, ks, ymax, method_info)
+        messages += [ks.ploidy_message] + ks.copy_messages
+
+    write_messages(ax, messages)
+
+    ax.set_title(markup(title))
+    ax.set_xlim((0, vmax))
+    ax.set_ylim((0, ymax))
+    adjust_spines(ax, ["left", "bottom"], outward=True)
+    xlabel, ylabel = "Coverage (X)", "Counts"
+    ax.set_xlabel(xlabel)
+    ax.set_ylabel(ylabel)
+    set_human_axis(ax)
+
+    return Genome_size
+
+
 def histogram(args):
     """
     %prog histogram meryl.histogram species K
 
-    Plot the histogram based on meryl K-mer distribution, species and N are
+    Plot the histogram based on Jellyfish or meryl K-mer distribution, species and N are
     only used to annotate the graphic.
     """
     p = OptionParser(histogram.__doc__)
     p.add_option(
         "--vmin",
         dest="vmin",
-        default=1,
+        default=2,
         type="int",
         help="minimum value, inclusive",
     )
     p.add_option(
         "--vmax",
         dest="vmax",
-        default=100,
+        default=200,
         type="int",
         help="maximum value, inclusive",
     )
     p.add_option(
-        "--pdf",
-        default=False,
-        action="store_true",
-        help="Print PDF instead of ASCII plot",
-    )
-    p.add_option(
         "--method",
         choices=("nbinom", "allpaths"),
         default="nbinom",
-        help="'nbinom' - slow but more accurate for het or polyploid genome; 'allpaths' - fast and works for homozygous enomes",
+        help="'nbinom' - slow but more accurate for het or polyploid genome; "
+        + "'allpaths' - fast and works for homozygous enomes",
     )
     p.add_option(
         "--maxiter",
         default=100,
         type="int",
         help="Max iterations for optimization. Only used with --method nbinom",
     )
@@ -1294,113 +1389,23 @@
 
     if len(args) != 3:
         sys.exit(not p.print_help())
 
     histfile, species, N = args
     method = opts.method
     vmin, vmax = opts.vmin, opts.vmax
-    ascii = not opts.pdf
     peaks = not opts.nopeaks and method == "allpaths"
     N = int(N)
 
-    if histfile.rsplit(".", 1)[-1] in ("mcdat", "mcidx"):
-        logging.debug("CA kmer index found")
-        histfile = merylhistogram(histfile)
-
-    ks = KmerSpectrum(histfile)
-    method_info = ks.analyze(K=N, maxiter=opts.maxiter, method=method)
-
-    Total_Kmers = int(ks.totalKmers)
-    coverage = opts.coverage
-    Kmer_coverage = ks.lambda_ if not coverage else coverage
-    Genome_size = int(round(Total_Kmers * 1.0 / Kmer_coverage))
-
-    Total_Kmers_msg = "Total {0}-mers: {1}".format(N, thousands(Total_Kmers))
-    Kmer_coverage_msg = "{0}-mer coverage: {1:.1f}x".format(N, Kmer_coverage)
-    Genome_size_msg = "Estimated genome size: {0:.1f} Mb".format(Genome_size / 1e6)
-    Repetitive_msg = ks.repetitive
-    SNPrate_msg = ks.snprate
-
-    for msg in (Total_Kmers_msg, Kmer_coverage_msg, Genome_size_msg):
-        print(msg, file=sys.stderr)
-
-    x, y = ks.get_xy(vmin, vmax)
-    title = "{0} {1}-mer histogram".format(species, N)
-
-    if ascii:
-        asciiplot(x, y, title=title)
-        return Genome_size
-
-    plt.figure(1, (iopts.w, iopts.h))
-    plt.bar(x, y, fc="#b2df8a", lw=0)
-    # Plot the negative binomial fit
-    if method == "nbinom":
-        generative_model = method_info["generative_model"]
-        GG = method_info["Gbins"]
-        ll = method_info["lambda"]
-        rr = method_info["rho"]
-        kf_range = method_info["kf_range"]
-        stacked = generative_model(GG, ll, rr)
-        plt.plot(
-            kf_range,
-            stacked,
-            ":",
-            color="#6a3d9a",
-            lw=2,
-        )
-
-    ax = plt.gca()
-
-    if peaks:  # Only works for method 'allpaths'
-        t = (ks.min1, ks.max1, ks.min2, ks.max2, ks.min3)
-        tcounts = [(x, y) for x, y in ks.counts if x in t]
-        if tcounts:
-            x, y = zip(*tcounts)
-            tcounts = dict(tcounts)
-            plt.plot(x, y, "ko", lw=3, mec="k", mfc="w")
-            ax.text(ks.max1, tcounts[ks.max1], "SNP peak")
-            ax.text(ks.max2, tcounts[ks.max2], "Main peak")
-
-    ymin, ymax = ax.get_ylim()
-    ymax = ymax * 7 / 6
-    if method == "nbinom":
-        # Plot multiple CN locations, CN1, CN2, ... up to ploidy
-        cn_color = "#a6cee3"
-        for i in range(1, ks.ploidy + 1):
-            x = i * ks.lambda_
-            plt.plot((x, x), (0, ymax), "-.", color=cn_color)
-            plt.text(
-                x,
-                ymax * 0.95,
-                "CN{}".format(i),
-                ha="right",
-                va="center",
-                color=cn_color,
-                rotation=90,
-            )
-
-    messages = [
-        Total_Kmers_msg,
-        Kmer_coverage_msg,
-        Genome_size_msg,
-        Repetitive_msg,
-        SNPrate_msg,
-    ]
-    if method == "nbinom":
-        messages += [ks.ploidy_message] + ks.copy_messages
-    write_messages(ax, messages)
+    fig = plt.figure(1, (iopts.w, iopts.h))
+    ax = fig.add_axes((0.1, 0.1, 0.8, 0.8))
 
-    ax.set_title(markup(title))
-    ax.set_xlim((0, vmax))
-    ax.set_ylim((0, ymax))
-    adjust_spines(ax, ["left", "bottom"], outward=True)
-    xlabel, ylabel = "Coverage (X)", "Counts"
-    ax.set_xlabel(xlabel)
-    ax.set_ylabel(ylabel)
-    set_human_axis(ax)
+    Genome_size = draw_ks_histogram(
+        ax, histfile, method, opts.coverage, vmin, vmax, species, N, opts.maxiter, peaks
+    )
 
     imagename = histfile.split(".")[0] + "." + iopts.format
     savefig(imagename, dpi=100)
 
     return Genome_size
```

### Comparing `jcvi-1.4.2/jcvi/assembly/opticalmap.py` & `jcvi-1.4.5/jcvi/assembly/opticalmap.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/assembly/patch.py` & `jcvi-1.4.5/jcvi/assembly/patch.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/assembly/postprocess.py` & `jcvi-1.4.5/jcvi/assembly/postprocess.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/assembly/preprocess.py` & `jcvi-1.4.5/jcvi/assembly/preprocess.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,17 +28,17 @@
     def __init__(self, filename, human=False):
         super(FastQCdata, self).__init__(filename)
         if not op.exists(filename):
             logging.debug("File `{0}` not found.".format(filename))
             # Sample_RF37-1/RF37-1_GATCAG_L008_R2_fastqc =>
             # RF37-1_GATCAG_L008_R2
             self["Filename"] = op.basename(op.split(filename)[0]).rsplit("_", 1)[0]
-            self["Total Sequences"] = self["Sequence length"] = self[
-                "Total Bases"
-            ] = "na"
+            self["Total Sequences"] = self["Sequence length"] = self["Total Bases"] = (
+                "na"
+            )
             return
 
         fp = open(filename)
         for row in fp:
             atoms = row.rstrip().split("\t")
             if atoms[0] in ("#", ">"):
                 continue
```

### Comparing `jcvi-1.4.2/jcvi/assembly/sim.py` & `jcvi-1.4.5/jcvi/assembly/sim.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/assembly/soap.py` & `jcvi-1.4.5/jcvi/assembly/soap.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/assembly/syntenypath.py` & `jcvi-1.4.5/jcvi/assembly/syntenypath.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/assembly/trinity.py` & `jcvi-1.4.5/jcvi/assembly/trinity.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/compara/base.py` & `jcvi-1.4.5/jcvi/compara/base.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/compara/blastfilter.py` & `jcvi-1.4.5/jcvi/compara/blastfilter.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/compara/catalog.py` & `jcvi-1.4.5/jcvi/compara/catalog.py`

 * *Files 5% similar despite different names*

```diff
@@ -605,26 +605,28 @@
     The pipeline runs LAST and generate .lifted.anchors.
 
     `--full` mode would assume 1-to-1 quota synteny blocks as the backbone of
     such predictions. Extra orthologs will be recruited from reciprocal best
     match (RBH).
     """
     from jcvi.apps.align import last as last_main
+    from jcvi.apps.align import diamond_blastp_main, blast_main
     from jcvi.compara.blastfilter import main as blastfilter_main
     from jcvi.compara.quota import main as quota_main
     from jcvi.compara.synteny import scan, mcscan, liftover
     from jcvi.formats.blast import cscore, filter, filtered_blastfile_name
 
     p = OptionParser(ortholog.__doc__)
     p.add_option(
         "--dbtype",
         default="nucl",
         choices=("nucl", "prot"),
         help="Molecule type of subject database",
     )
+
     p.add_option(
         "--full",
         default=False,
         action="store_true",
         help="Run in full 1x1 mode, including blocks and RBH",
     )
     p.add_option("--cscore", default=0.7, type="float", help="C-score cutoff")
@@ -666,15 +668,22 @@
     dotplot_group.add_option(
         "--no_dotplot", default=False, action="store_true", help="Do not make dotplot"
     )
     p.add_option(
         "--ignore_zero_anchor",
         default=False,
         action="store_true",
-        help="Ignore this pair of ortholog identification instead of throwing an error when performing many pairs of cataloging."
+        help="Ignore this pair of ortholog identification instead of throwing an error when performing many pairs of cataloging.",
+    )
+
+    p.add_option(
+        "--align_soft",
+        default="last",
+        choices=("last", "blast", "diamond_blastp"),
+        help="Sequence alignment software. Default <last> for both <nucl> and <prot>. Users could also use <blast> for both <nucl> and <prot>, or <diamond_blastp> for <prot>.",
     )
 
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
@@ -686,22 +695,28 @@
     bbed, bfasta = b + ".bed", b + suffix
     ccscore = opts.cscore
     quota = opts.quota
     exclude = opts.exclude
     dist = "--dist={0}".format(opts.dist)
     minsize_flag = "--min_size={}".format(opts.n)
     cpus_flag = "--cpus={}".format(opts.cpus)
+    align_soft = opts.align_soft
 
     aprefix = op.basename(a)
     bprefix = op.basename(b)
     pprefix = ".".join((aprefix, bprefix))
     qprefix = ".".join((bprefix, aprefix))
     last = pprefix + ".last"
     if need_update((afasta, bfasta), last, warn=True):
-        last_main([bfasta, afasta, cpus_flag], dbtype)
+        if align_soft == "blast":
+            blast_main([bfasta, afasta, cpus_flag], dbtype)
+        elif dbtype == "prot" and align_soft == "diamond_blastp":
+            diamond_blastp_main([bfasta, afasta, cpus_flag], dbtype)
+        else:
+            last_main([bfasta, afasta, cpus_flag], dbtype)
 
     self_remove = opts.self_remove
     if a == b:
         lastself = filtered_blastfile_name(last, self_remove, 0, inverse=True)
         if need_update(last, lastself, warn=True):
             filter(
                 [last, "--hitlen=0", f"--pctid={self_remove}", "--inverse", "--noself"]
```

### Comparing `jcvi-1.4.2/jcvi/compara/fractionation.py` & `jcvi-1.4.5/jcvi/compara/fractionation.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/compara/pad.py` & `jcvi-1.4.5/jcvi/compara/pad.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/compara/phylogeny.py` & `jcvi-1.4.5/jcvi/compara/phylogeny.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/compara/quota.py` & `jcvi-1.4.5/jcvi/compara/quota.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/compara/reconstruct.py` & `jcvi-1.4.5/jcvi/compara/reconstruct.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/compara/synfind.py` & `jcvi-1.4.5/jcvi/compara/synfind.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/compara/synteny.py` & `jcvi-1.4.5/jcvi/compara/synteny.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/formats/agp.py` & `jcvi-1.4.5/jcvi/formats/agp.py`

 * *Files 0% similar despite different names*

```diff
@@ -310,15 +310,15 @@
 
     @property
     def order(self):
         """
         Returns a dict with component_id => (i, agpline)
         """
         d = {}
-        for (i, x) in enumerate(self):
+        for i, x in enumerate(self):
             if x.is_gap:
                 continue
             xid = x.component_id
             d[xid] = (i, x)
 
             xid = xid.rsplit(".", 1)[0]  # Remove Genbank version
             if xid not in d:
@@ -1289,17 +1289,17 @@
             if opts.warn and span < 50:
                 logging.error("component span too small ({0}):\n{1}".format(span, a))
 
     table = dict()
     for label, lengths in zip(("Gaps", "Components"), (gap_lengths, component_lengths)):
 
         if not lengths:
-            table[(label, "Min")] = table[(label, "Max")] = table[
-                (label, "Sum")
-            ] = "n.a."
+            table[(label, "Min")] = table[(label, "Max")] = table[(label, "Sum")] = (
+                "n.a."
+            )
             continue
 
         table[(label, "Min")] = "{0} ({1})".format(*min(lengths))
         table[(label, "Max")] = "{0} ({1})".format(*max(lengths))
         table[(label, "Sum")] = sum(x[0] for x in lengths)
 
     print(tabulate(table), file=sys.stderr)
```

### Comparing `jcvi-1.4.2/jcvi/formats/base.py` & `jcvi-1.4.5/jcvi/formats/base.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/formats/bed.py` & `jcvi-1.4.5/jcvi/formats/bed.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Classes to handle the .bed files
 """
+
 import logging
 import math
 import numpy as np
 import os
 import os.path as op
 import shutil
 import sys
@@ -147,15 +148,19 @@
         self.nullkey = lambda x: (natsort_key(x.seqid), x.start, x.accn)
         self.key = key or self.nullkey
 
         if not filename:
             return
 
         for line in must_open(filename):
-            if line[0] == "#" or (juncs and line.startswith("track name")) or line.strip()=="":
+            if (
+                line[0] == "#"
+                or (juncs and line.startswith("track name"))
+                or line.strip() == ""
+            ):
                 continue
             b = BedLine(line)
             if include and b.accn not in include:
                 continue
             self.append(b)
 
         if sorted:
```

### Comparing `jcvi-1.4.2/jcvi/formats/blast.py` & `jcvi-1.4.5/jcvi/formats/blast.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/formats/cblast.pyx` & `jcvi-1.4.5/jcvi/formats/cblast.pyx`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/formats/cdt.py` & `jcvi-1.4.5/jcvi/formats/cdt.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/formats/chain.py` & `jcvi-1.4.5/jcvi/formats/chain.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/formats/contig.py` & `jcvi-1.4.5/jcvi/formats/contig.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/formats/coords.py` & `jcvi-1.4.5/jcvi/formats/coords.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,15 +166,14 @@
         else:
             type = 0
 
         return type
 
 
 class Coords(LineFile):
-
     """
     when parsing the .coords file, first skip first 5 lines
     [S1] [E1] | [S2] [E2] | [LEN 1] [LEN 2] | [% IDY] | [TAGS]
 
     then each row would be composed as this
     """
```

### Comparing `jcvi-1.4.2/jcvi/formats/excel.py` & `jcvi-1.4.5/jcvi/formats/excel.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/formats/fasta.py` & `jcvi-1.4.5/jcvi/formats/fasta.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Wrapper for biopython Fasta, add option to parse sequence headers
 """
+
 import re
 import sys
 import os
 import os.path as op
 import shutil
 import logging
 import string
```

### Comparing `jcvi-1.4.2/jcvi/formats/fastq.py` & `jcvi-1.4.5/jcvi/formats/fastq.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/formats/genbank.py` & `jcvi-1.4.5/jcvi/formats/genbank.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,24 +137,24 @@
 
         if filenames is not None:
             self.accessions = [op.basename(f).split(".")[0] for f in filenames]
             d = dict(
                 next(iter(SeqIO.to_dict(SeqIO.parse(f, "gb")).items()))
                 for f in filenames
             )
-            for (k, v) in d.items():
+            for k, v in d.items():
                 self[k.split(".")[0]] = v
 
         elif idfile is not None:
             gbdir = self._get_records()
             d = dict(
                 next(iter(SeqIO.to_dict(SeqIO.parse(f, "gb")).items()))
                 for f in glob(gbdir + "/*.gb")
             )
-            for (k, v) in d.items():
+            for k, v in d.items():
                 self[k.split(".")[0]] = v
 
         else:
             sys.exit(
                 "GenBank object is initiated from either gb files or " "accession IDs."
             )
```

### Comparing `jcvi-1.4.2/jcvi/formats/gff.py` & `jcvi-1.4.5/jcvi/formats/gff.py`

 * *Files 0% similar despite different names*

```diff
@@ -3052,15 +3052,14 @@
     ensembl_cds = opts.ensembl_cds
     if opts.type:
         type = set(x.strip() for x in opts.type.split(","))
     if opts.source:
         source = set(x.strip() for x in opts.source.split(","))
     if ensembl_cds:
         type = {"CDS"}
-        source = {"protein_coding"}
 
     gff = Gff(
         gffile,
         key=key,
         parent_key=parent_key,
         append_source=opts.append_source,
         append_ftype=opts.append_ftype,
@@ -3091,14 +3090,16 @@
         if span:
             bl.score = bl.span
         if human_chr:
             if bl.seqid not in VALID_HUMAN_CHROMOSMES:
                 continue
             bl.seqid = "chr" + bl.seqid
         if ensembl_cds:
+            if g.get_attr("gene_biotype") != "protein_coding":
+                continue
             bl.accn = "{0}.{1}".format(
                 g.get_attr("transcript_name"), g.get_attr("exon_number")
             )
             position = (bl.seqid, bl.start, bl.end)
             if position in seen:
                 skipped_identical_range += 1
                 continue
```

### Comparing `jcvi-1.4.2/jcvi/formats/html.py` & `jcvi-1.4.5/jcvi/formats/html.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/formats/maf.py` & `jcvi-1.4.5/jcvi/formats/maf.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/formats/obo.py` & `jcvi-1.4.5/jcvi/formats/obo.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/formats/paf.py` & `jcvi-1.4.5/jcvi/formats/paf.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/formats/pdf.py` & `jcvi-1.4.5/jcvi/formats/pdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     filename_page_ranges = parse_filename_page_ranges(args)
     verbose = opts.verbose
     fw = must_open(outfile, "wb")
 
     merger = PdfFileMerger()
     in_fs = {}
     try:
-        for (filename, page_range) in filename_page_ranges:
+        for filename, page_range in filename_page_ranges:
             if verbose:
                 print(filename, page_range, file=sys.stderr)
             if filename not in in_fs:
                 in_fs[filename] = open(filename, "rb")
             merger.append(in_fs[filename], pages=page_range)
     except:
         print(traceback.format_exc(), file=sys.stderr)
```

### Comparing `jcvi-1.4.2/jcvi/formats/psl.py` & `jcvi-1.4.5/jcvi/formats/psl.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/formats/pyblast.py` & `jcvi-1.4.5/jcvi/formats/pyblast.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/formats/sam.py` & `jcvi-1.4.5/jcvi/formats/sam.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/formats/sizes.py` & `jcvi-1.4.5/jcvi/formats/sizes.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/formats/vcf.py` & `jcvi-1.4.5/jcvi/formats/vcf.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/graphics/align.py` & `jcvi-1.4.5/jcvi/graphics/align.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/graphics/assembly.py` & `jcvi-1.4.5/jcvi/graphics/assembly.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/graphics/base.py` & `jcvi-1.4.5/jcvi/graphics/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,50 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 
 import copy
 import os.path as op
 from os import remove
+
 import sys
 import logging
 
 logging.getLogger("matplotlib").setLevel(logging.WARNING)
 logging.getLogger("numexpr").setLevel(logging.WARNING)
 logging.getLogger("PIL").setLevel(logging.INFO)
 
-
 from functools import partial
+from typing import Optional, List, Tuple, Union
 
 import numpy as np
 import matplotlib as mpl
+import seaborn as sns
 
 mpl.use("Agg")
 
 import matplotlib.pyplot as plt
 import matplotlib.ticker as ticker
 
 from brewer2mpl import get_map
 from matplotlib import cm, rc, rcParams
+from matplotlib.colors import Colormap
 from matplotlib.patches import (
     Rectangle,
     Polygon,
     CirclePolygon,
     Ellipse,
     PathPatch,
     FancyArrow,
     FancyArrowPatch,
     FancyBboxPatch,
 )
-from typing import Optional
 
 from ..apps.base import datadir, glob, listify, logger, sample_N, which
 from ..formats.base import LineFile
+from ..utils.cbook import human_size
 
 
 CHARS = {
     "&": r"\&",
     "%": r"\%",
     "$": r"\$",
     "#": r"\#",
@@ -269,22 +272,28 @@
     return blues_r, reds, blue_red, green_purple, red_purple
 
 
 blues_r, reds, blue_red, green_purple, red_purple = prettyplot()
 
 
 def normalize_axes(axes):
+    """
+    Normalize the axes to have the same scale.
+    """
     axes = listify(axes)
     for ax in axes:
         ax.set_xlim(0, 1)
         ax.set_ylim(0, 1)
         ax.set_axis_off()
 
 
-def panel_labels(ax, labels, size=16):
+def panel_labels(ax, labels, size: int = 16):
+    """
+    Add panel labels (A, B, ...) to a figure.
+    """
     for xx, yy, panel_label in labels:
         if rcParams["text.usetex"]:
             panel_label = r"$\textbf{{{0}}}$".format(panel_label)
         ax.text(xx, yy, panel_label, size=size, ha="center", va="center")
 
 
 def update_figname(figname: str, format: str) -> str:
@@ -328,15 +337,15 @@
     logger.debug(msg)
 
     if cleanup:
         plt.rcdefaults()
 
 
 # human readable size (Kb, Mb, Gb)
-def human_readable(x, pos, base=False):
+def human_readable(x: Union[str, int], _, base=False):
     x = str(int(x))
     if x.endswith("000000000"):
         x = x[:-9] + "G"
     elif x.endswith("000000"):
         x = x[:-6] + "M"
     elif x.endswith("000"):
         x = x[:-3] + "K"
@@ -414,22 +423,20 @@
     context="notebook",
     style="darkgrid",
     palette="deep",
     font="Helvetica",
     usetex: bool = True,
 ):
     try:
-        import seaborn as sns
-
         extra_rc = {
             "lines.linewidth": 1,
             "lines.markeredgewidth": 1,
             "patch.edgecolor": "k",
         }
-        sns.set(context=context, style=style, palette=palette, rc=extra_rc)
+        sns.set_theme(context=context, style=style, palette=palette, rc=extra_rc)
     except (ImportError, SyntaxError):
         pass
 
     if usetex:
         rc("text", usetex=True)
     else:
         logger.info("Set text.usetex=%s. Font styles may be inconsistent.", usetex)
@@ -495,14 +502,75 @@
     ax.set_ylim(0, 20)
     ax.set_xlim(0, xmax)
     ax.set_axis_off()
 
     savefig(outfile)
 
 
+def plot_heatmap(
+    ax,
+    M: np.array,
+    breaks: List[int],
+    groups: List[Tuple[int, int, List[Tuple[int, str]], str]] = [],
+    plot_breaks: bool = False,
+    cmap: Optional[Union[str, Colormap]] = None,
+    binsize: Optional[int] = None,
+):
+    """Plot heatmap illustrating the contact probabilities in Hi-C data.
+
+    Args:
+        ax (pyplot.axes): Matplotlib axis
+        M (np.array): 2D numpy-array
+        breaks (List[int]): Positions of chromosome starts. Can be None.
+        iopts (OptionParser options): Graphical options passed in from commandline
+        groups (List, optional): [(start, end, [(position, seqid)], color)]. Defaults to [].
+        plot_breaks (bool): Whether to plot white breaks. Defaults to False.
+        cmap (str | Colormap, optional): Colormap. Defaults to None, which uses cubehelix.
+        binsize (int, optional): Resolution of the heatmap.
+    """
+    cmap = cmap or sns.cubehelix_palette(rot=0.5, as_cmap=True)
+    ax.imshow(M, cmap=cmap, interpolation="none")
+    _, xmax = ax.get_xlim()
+    xlim = (0, xmax)
+    if plot_breaks:
+        for b in breaks[:-1]:
+            ax.plot([b, b], xlim, "w-")
+            ax.plot(xlim, [b, b], "w-")
+
+    def simplify_seqid(seqid):
+        seqid = seqid.replace("_", "")
+        if seqid[:3].lower() == "chr":
+            seqid = seqid[3:]
+        return seqid.lstrip("0")
+
+    for start, end, position_seqids, color in groups:
+        # Plot a square
+        ax.plot([start, start], [start, end], "-", color=color)
+        ax.plot([start, end], [start, start], "-", color=color)
+        ax.plot([start, end], [end, end], "-", color=color)
+        ax.plot([end, end], [start, end], "-", color=color)
+        for position, seqid in position_seqids:
+            seqid = simplify_seqid(seqid)
+            ax.text(position, end, seqid, ha="center", va="top")
+
+    ax.set_xlim(xlim)
+    ax.set_ylim((xlim[1], xlim[0]))  # Flip the y-axis so the origin is at the top
+    ax.set_xticklabels(ax.get_xticks(), family="Helvetica", color="gray")
+    ax.set_yticklabels(ax.get_yticks(), family="Helvetica", color="gray", rotation=90)
+    ax.tick_params(left=True, bottom=True, labelleft=True, labelbottom=True)
+    if binsize is not None:
+        formatter = ticker.FuncFormatter(
+            lambda x, pos: human_readable(int(x) * binsize, pos, base=True)
+        )
+        ax.xaxis.set_major_formatter(formatter)
+        ax.yaxis.set_major_formatter(formatter)
+        title = f"Resolution = {human_size(binsize, precision=0)} per bin"
+        ax.set_xlabel(title)
+
+
 def discrete_rainbow(N=7, cmap=cm.Set1, usepreset=True, shuffle=False, plot=False):
     """
     Return a discrete colormap and the set of colors.
 
     modified from
     <http://www.scipy.org/Cookbook/Matplotlib/ColormapTransformations>
```

### Comparing `jcvi-1.4.2/jcvi/graphics/blastplot.py` & `jcvi-1.4.5/jcvi/graphics/blastplot.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,24 +122,24 @@
 
     xchr_labels, ychr_labels = [], []
     ignore = True  # tag to mark whether to plot chr name (skip small ones)
     ignore_size_x = ignore_size_y = 0
 
     # plot the chromosome breaks
     logging.debug("xbreaks={0} ybreaks={1}".format(len(qsizes), len(ssizes)))
-    for (seqid, beg, end) in qsizes.get_breaks():
+    for seqid, beg, end in qsizes.get_breaks():
         ignore = abs(end - beg) < ignore_size_x
         if ignore:
             continue
         seqid = rename_seqid(seqid)
 
         xchr_labels.append((seqid, (beg + end) / 2, ignore))
         ax.plot([end, end], ylim, "-", lw=1, color="grey")
 
-    for (seqid, beg, end) in ssizes.get_breaks():
+    for seqid, beg, end in ssizes.get_breaks():
         ignore = abs(end - beg) < ignore_size_y
         if ignore:
             continue
         seqid = rename_seqid(seqid)
 
         ychr_labels.append((seqid, (beg + end) / 2, ignore))
         ax.plot(xlim, [end, end], "-", lw=1, color="grey")
```

### Comparing `jcvi-1.4.2/jcvi/graphics/chromosome.py` & `jcvi-1.4.5/jcvi/graphics/chromosome.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 # -*- coding: UTF-8 -*-
 
 """
 Legacy script to plot distribution of certain classes onto chromosomes. Adapted
 from the script used in the Tang et al. PNAS 2010 paper, sigma figure.
 """
 import sys
+
 from itertools import groupby
 from math import ceil
-from typing import Tuple
+from typing import Optional, Tuple
 
 import numpy as np
 
 from natsort import natsorted
 
 from ..apps.base import OptionGroup, OptionParser, datafile, logger, sample_N
 from ..formats.base import DictFile, get_number
@@ -20,14 +21,15 @@
 from ..formats.sizes import Sizes
 from ..graphics.base import (
     CirclePolygon,
     Polygon,
     Rectangle,
     latex,
     markup,
+    normalize_axes,
     plt,
     savefig,
     set1_n,
     set3_n,
 )
 from ..graphics.glyph import BaseGlyph, plot_cap
 
@@ -476,15 +478,15 @@
 
     bedfile = args[0]
     mappingfile = None
     if len(args) == 2:
         mappingfile = args[1]
 
     fig = plt.figure(1, (iopts.w, iopts.h))
-    root = fig.add_axes([0, 0, 1, 1])
+    root = fig.add_axes((0, 0, 1, 1))
 
     draw_chromosomes(
         root,
         bedfile,
         sizes=opts.sizes,
         iopts=iopts,
         mergedist=opts.mergedist,
@@ -493,36 +495,34 @@
         mappingfile=mappingfile,
         gauge=opts.gauge,
         legend=opts.legend,
         empty=opts.empty,
         title=opts.title,
     )
 
-    root.set_xlim(0, 1)
-    root.set_ylim(0, 1)
-    root.set_axis_off()
+    normalize_axes(root)
 
     prefix = bedfile.rsplit(".", 1)[0]
     figname = prefix + "." + opts.format
     savefig(figname, dpi=iopts.dpi, iopts=iopts)
 
 
 def draw_chromosomes(
     root,
     bedfile,
     sizes,
     iopts,
-    mergedist,
-    winsize,
-    imagemap,
-    mappingfile=None,
-    gauge=False,
-    legend=True,
-    empty=False,
-    title=None,
+    mergedist: int,
+    winsize: int,
+    imagemap: bool = False,
+    mappingfile: Optional[str] = None,
+    gauge: bool = False,
+    legend: bool = True,
+    empty: bool = False,
+    title: Optional[str] = None,
 ):
     bed = Bed(bedfile)
     prefix = bedfile.rsplit(".", 1)[0]
 
     if imagemap:
         imgmapfile = prefix + ".map"
         mapfh = open(imgmapfile, "w")
```

### Comparing `jcvi-1.4.2/jcvi/graphics/coverage.py` & `jcvi-1.4.5/jcvi/graphics/coverage.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/graphics/dotplot.py` & `jcvi-1.4.5/jcvi/graphics/dotplot.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/graphics/glyph.py` & `jcvi-1.4.5/jcvi/graphics/glyph.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/graphics/grabseeds.py` & `jcvi-1.4.5/jcvi/graphics/grabseeds.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,139 +2,168 @@
 # -*- coding: UTF-8 -*-
 
 """
 Image processing pipelines for phenotyping projects.
 """
 import json
 import os.path as op
-import sys
 import string
-import logging
-from math import sin, cos, pi
+import sys
 
 from collections import Counter
+from math import cos, pi, sin
+from typing import Any, List, Optional, Tuple
 
 import numpy as np
-from jcvi.graphics.base import (
-    plt,
-    savefig,
-    normalize_axes,
-    Rectangle,
-    latex,
-    load_image,
-)
 
 from PIL.Image import open as iopen
+from pyefd import elliptic_fourier_descriptors
 from pytesseract import image_to_string
-
-from wand.image import Image
-from webcolors import rgb_to_hex, normalize_integer_triplet
 from scipy.ndimage import binary_fill_holes, distance_transform_edt
 from scipy.optimize import fmin_bfgs as fmin
 from skimage.color import gray2rgb, rgb2gray
-from skimage.filters import roberts, sobel
 from skimage.feature import canny, peak_local_max
-from skimage.measure import regionprops, label
+from skimage.filters import roberts, sobel
+from skimage.measure import find_contours, regionprops, label
 from skimage.morphology import disk, closing
-from skimage.segmentation import watershed
-from skimage.segmentation import clear_border
+from skimage.segmentation import clear_border, watershed
+from wand.image import Image
+from webcolors import rgb_to_hex, normalize_integer_triplet
 
-from jcvi.utils.webcolors import closest_color
-from jcvi.formats.base import must_open
-from jcvi.algorithms.formula import reject_outliers, get_kmeans
-from jcvi.apps.base import (
+from .base import (
+    Rectangle,
+    latex,
+    load_image,
+    normalize_axes,
+    plt,
+    savefig,
+    set_helvetica_axis,
+)
+from ..algorithms.formula import get_kmeans, reject_outliers
+from ..apps.base import (
     OptionParser,
     OptionGroup,
     ActionDispatcher,
+    datadir,
+    logger,
     iglob,
     mkdir,
-    datadir,
 )
-
+from ..formats.base import must_open
+from ..formats.pdf import cat
+from ..utils.webcolors import closest_color
 
 np.seterr(all="ignore")
 
+RGBTuple = Tuple[int, int, int]
+
 
 class Seed(object):
-    def __init__(self, imagename, accession, seedno, rgb, props, exif):
+    """
+    Seed object with metrics.
+    """
+
+    def __init__(
+        self,
+        imagename: str,
+        accession: str,
+        seedno: int,
+        rgb: RGBTuple,
+        props: Any,
+        efds: np.ndarray,
+        exif: dict,
+    ):
         self.imagename = imagename
         self.accession = accession
         self.seedno = seedno
         y, x = props.centroid
         self.x, self.y = int(round(x)), int(round(y))
-        self.location = "{0}|{1}".format(self.x, self.y)
+        self.location = f"{self.x}|{self.y}"
         self.area = int(round(props.area))
         self.length = int(round(props.major_axis_length))
         self.width = int(round(props.minor_axis_length))
         self.props = props
+        self.efds = efds
         self.circularity = 4 * pi * props.area / props.perimeter**2
         self.rgb = rgb
         self.colorname = closest_color(rgb)
         self.datetime = exif.get("exif:DateTimeOriginal", "none")
         self.rgbtag = triplet_to_rgb(rgb)
-        self.pixeltag = "length={0} width={1} area={2}".format(
-            self.length, self.width, self.area
-        )
+        self.pixeltag = f"length={self.length} width={self.width} area={self.area}"
         self.hashtag = " ".join((self.rgbtag, self.colorname))
         self.calibrated = False
 
     def __str__(self):
         fields = [
             self.imagename,
             self.datetime,
             self.accession,
             self.seedno,
             self.location,
             self.area,
-            "{0:.2f}".format(self.circularity),
+            f"{self.circularity:.2f}",
             self.length,
             self.width,
             self.colorname,
             self.rgbtag,
         ]
         if self.calibrated:
             fields += [
                 self.pixelcmratio,
                 self.rgbtransform,
                 self.correctedlength,
                 self.correctedwidth,
                 self.correctedcolorname,
                 self.correctedrgb,
             ]
+        fields += [",".join(f"{x:.3f}" for x in self.efds)]
         return "\t".join(str(x) for x in fields)
 
     @classmethod
-    def header(cls, calibrate=False):
+    def header(cls, calibrated: bool = False) -> str:
+        """
+        Return header line for the TSV file.
+        """
         fields = (
             "ImageName DateTime Accession SeedNum Location "
             "Area Circularity Length(px) Width(px) ColorName RGB".split()
         )
-        if calibrate:
+        if calibrated:
             fields += (
                 "PixelCMratio RGBtransform Length(cm)"
                 " Width(cm) CorrectedColorName CorrectedRGB".split()
             )
+        fields += ["EllipticFourierDescriptors"]
         return "\t".join(fields)
 
-    def calibrate(self, pixel_cm_ratio, tr):
-        self.pixelcmratio = "{0:.2f}".format(pixel_cm_ratio)
-        self.rgbtransform = ",".join(["{0:.2f}".format(x) for x in tr.flatten()])
-        self.correctedlength = "{0:.2f}".format(self.length / pixel_cm_ratio)
-        self.correctedwidth = "{0:.2f}".format(self.width / pixel_cm_ratio)
+    def calibrate(self, pixel_cm_ratio: float, tr: np.ndarray):
+        """
+        Calibrate pixel-inch ratio and color adjustment.
+        """
+        self.pixelcmratio = f"{pixel_cm_ratio:.2f}"
+        self.rgbtransform = ",".join([f"{x:.2f}" for x in tr.flatten()])
+        self.correctedlength = f"{self.length / pixel_cm_ratio:.2f}"
+        self.correctedwidth = f"{self.width / pixel_cm_ratio:.2f}"
         correctedrgb = np.dot(tr, np.array(self.rgb))
         self.correctedrgb = triplet_to_rgb(correctedrgb)
         self.correctedcolorname = closest_color(correctedrgb)
         self.calibrated = True
 
 
-def rgb_to_triplet(rgb):
-    return tuple([int(x) for x in rgb.split(",")])
+def rgb_to_triplet(rgb: str) -> RGBTuple:
+    """
+    Convert RGB string to triplet.
+    """
+    return tuple([int(x) for x in rgb.split(",")][:3])
 
 
-def triplet_to_rgb(triplet):
+def triplet_to_rgb(triplet: RGBTuple) -> str:
+    """
+    Convert triplet to RGB string.
+    """
     triplet = normalize_integer_triplet(triplet)
     return ",".join(str(int(round(x))) for x in triplet)
 
 
 def main():
 
     actions = (
@@ -142,66 +171,68 @@
         ("seeds", "extract seed metrics from one image"),
         ("calibrate", "calibrate pixel-inch ratio and color adjustment"),
     )
     p = ActionDispatcher(actions)
     p.dispatch(globals())
 
 
-def total_error(x, colormap):
+def total_error(x: np.ndarray, colormap: Tuple[Tuple[np.ndarray, np.ndarray]]) -> float:
+    """
+    Calculate total error between observed and expected colors.
+    """
     xs = np.reshape(x, (3, 3))
-    error_squared = sum([np.linalg.norm(np.dot(xs, o) - e) ** 2 for o, e in colormap])
+    error_squared = sum(np.linalg.norm(np.dot(xs, o) - e) ** 2 for o, e in colormap)
     return error_squared**0.5
 
 
 def calibrate(args):
     """
     %prog calibrate calibrate.JPG boxsize
 
     Calibrate pixel-inch ratio and color adjustment.
     - `calibrate.JPG` is the photo containig a colorchecker
     - `boxsize` is the measured size for the boxes on printed colorchecker, in
       squared centimeter (cm2) units
     """
     xargs = args[2:]
     p = OptionParser(calibrate.__doc__)
-    opts, args, iopts = add_seeds_options(p, args)
+    _, args, _ = add_seeds_options(p, args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     imagefile, boxsize = args
     boxsize = float(boxsize)
 
     # Read in color checker
     colorcheckerfile = op.join(datadir, "colorchecker.txt")
     colorchecker = []
     expected = 0
-    for row in open(colorcheckerfile):
-        boxes = row.split()
-        colorchecker.append(boxes)
-        expected += len(boxes)
+    with open(colorcheckerfile, encoding="utf-8") as file:
+        for row in file:
+            boxes = row.split()
+            colorchecker.append(boxes)
+            expected += len(boxes)
 
     folder = op.split(imagefile)[0]
-    objects = seeds([imagefile, "--outdir={0}".format(folder)] + xargs)
+    objects = seeds([imagefile, f"--outdir={folder}"] + xargs)
     nseeds = len(objects)
-    logging.debug("Found {0} boxes (expected={1})".format(nseeds, expected))
+    logger.debug("Found %d boxes (expected=%d)", nseeds, expected)
     assert (
         expected - 4 <= nseeds <= expected + 4
-    ), "Number of boxes drastically different from {0}".format(expected)
+    ), f"Number of boxes drastically different from {expected}"
 
     # Calculate pixel-cm ratio
     boxes = [t.area for t in objects]
     reject = reject_outliers(boxes)
     retained_boxes = [b for r, b in zip(reject, boxes) if not r]
     mbox = np.median(retained_boxes)  # in pixels
     pixel_cm_ratio = (mbox / boxsize) ** 0.5
-    logging.debug(
-        "Median box size: {0} pixels. Measured box size: {1} cm2".format(mbox, boxsize)
-    )
-    logging.debug("Pixel-cm ratio: {0}".format(pixel_cm_ratio))
+    logger.debug("Median box size: %d pixels. Measured box size: %d cm2", mbox, boxsize)
+    logger.debug("Pixel-cm ratio: %.2f", pixel_cm_ratio)
 
     xs = [t.x for t in objects]
     ys = [t.y for t in objects]
     xs = [float(itemx) for itemx in xs]
     ys = [float(itemy) for itemy in ys]
     idx_xs = get_kmeans(xs, 6)
     idx_ys = get_kmeans(ys, 4)
@@ -224,20 +255,23 @@
     print("RGB linear transform:\n", tr, file=sys.stderr)
     calib = {"PixelCMratio": pixel_cm_ratio, "RGBtransform": tr.tolist()}
 
     jsonfile = op.join(folder, "calibrate.json")
     fw = must_open(jsonfile, "w")
     print(json.dumps(calib, indent=4), file=fw)
     fw.close()
-    logging.debug("Calibration specs written to `{0}`.".format(jsonfile))
+    logger.debug("Calibration specs written to `%s`.", jsonfile)
 
     return jsonfile
 
 
 def add_seeds_options(p, args):
+    """
+    Add options to the OptionParser for seeds() and batchseeds() functions.
+    """
     g1 = OptionGroup(p, "Image manipulation")
     g1.add_option("--rotate", default=0, type="int", help="Rotate degrees clockwise")
     g1.add_option(
         "--rows", default=":", help="Crop rows e.g. `:800` from first 800 rows"
     )
     g1.add_option(
         "--cols", default=":", help="Crop cols e.g. `-800:` from last 800 cols"
@@ -322,19 +356,17 @@
 
 def batchseeds(args):
     """
     %prog batchseeds folder
 
     Extract seed metrics for each image in a directory.
     """
-    from jcvi.formats.pdf import cat
-
     xargs = args[1:]
     p = OptionParser(batchseeds.__doc__)
-    opts, args, iopts = add_seeds_options(p, args)
+    opts, args, _ = add_seeds_options(p, args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (folder,) = args
     folder = folder.rstrip("/")
     outdir = folder + "-debug"
@@ -348,95 +380,105 @@
         if im.endswith((".resize.jpg", ".main.jpg", ".label.jpg")):
             continue
         if op.basename(im).startswith("calibrate"):
             continue
         images.append(im)
 
     fw = must_open(outfile, "w")
-    print(Seed.header(calibrate=jsonfile), file=fw)
+    print(Seed.header(calibrated=bool(jsonfile)), file=fw)
     nseeds = 0
     for im in images:
-        imargs = [im, "--noheader", "--outdir={0}".format(outdir)] + xargs
+        imargs = [im, "--noheader", f"--outdir={outdir}"] + xargs
         if jsonfile:
-            imargs += ["--calibrate={0}".format(jsonfile)]
+            imargs += [f"--calibrate={jsonfile}"]
         objects = seeds(imargs)
         for o in objects:
             print(o, file=fw)
         nseeds += len(objects)
     fw.close()
-    logging.debug("Processed {0} images.".format(len(images)))
-    logging.debug("A total of {0} objects written to `{1}`.".format(nseeds, outfile))
+    logger.debug("Processed %d images.", len(images))
+    logger.debug("A total of %d objects written to `%s`.", nseeds, outfile)
 
     pdfs = iglob(outdir, "*.pdf")
     outpdf = folder + "-output.pdf"
-    cat(pdfs + ["--outfile={0}".format(outpdf)])
+    cat(pdfs + [f"--outfile={outpdf}"])
 
-    logging.debug("Debugging information written to `{0}`.".format(outpdf))
+    logger.debug("Debugging information written to `%s`.", outpdf)
     return outfile
 
 
-def p_round(n, precision=5):
+def p_round(n: int, precision: int = 5) -> int:
+    """
+    Round to the nearest precision.
+    """
     precision = int(precision)
     return int(round(n / float(precision))) * precision
 
 
-def pixel_stats(img):
+def pixel_stats(img: List[RGBTuple]) -> RGBTuple:
+    """
+    Get the most common pixel color.
+    """
     img = [(p_round(r), p_round(g), p_round(b)) for r, g, b in img]
     c = Counter(img)
-    imgx, count = c.most_common(1)[0]
+    imgx, _ = c.most_common(1)[0]
     return imgx
 
 
-def slice(s, m):
+def slice_to_ints(s: str, m: int) -> Tuple[int, int]:
+    """
+    Parse slice string.
+    """
     assert ":" in s
     ra, rb = s.split(":")
     ra = 0 if ra == "" else int(ra)
     rb = m if rb == "" else int(rb)
     return ra, rb
 
 
-def convert_background(pngfile, new_background):
-    """Replace the background color with the specified background color, default is blue"""
+def convert_background(pngfile: str, new_background: str):
+    """
+    Replace the background color with the specified background color, default is
+    blue.
+    """
     if new_background:
         _name, _ext = op.splitext(op.basename(pngfile))
         _name += "_bgxform"
         newfile = op.join(op.dirname(pngfile), _name + _ext)
 
         img = iopen(pngfile)
         pixels = list(img.getdata())
-        h, w = img.size
 
         # Get Standard Deviation of RGB
-        rgbArray = []
+        rgb_array = []
         for x in range(255):
-            rgbArray.append(x)
-        stdRGB = np.std(rgbArray) * 0.8
+            rgb_array.append(x)
+        std_rgb = np.std(rgb_array) * 0.8
 
         # Get average color
-        obcolor = [None, None, None]
+        obcolor = [0, 0, 0]
         pixel_values = []
         for t in range(3):
             pixel_color = img.getdata(band=t)
             for pixel in pixel_color:
-                if pixel > stdRGB:
+                if pixel > std_rgb:
                     pixel_values.append(pixel)
             obcolor[t] = sum(pixel_values) // len(pixel_values)
 
         # Get background color using average color and standard deviation
         for t in range(3):
             pixel_color = img.getdata(band=t)
             seed_pixel_values = []
             for i in pixel_color:
-                if (i > (obcolor[t] - stdRGB)) and (i < (obcolor[t] + stdRGB)):
+                if obcolor[t] - std_rgb < i < obcolor[t] + std_rgb:
                     seed_pixel_values.append(i)
             obcolor[t] = sum(seed_pixel_values) // len(seed_pixel_values)
         # Selection of colors based on option parser
-        nbcolor = [None, None, None]
+        nbcolor = [0, 0, 0]
         if new_background == "INVERSE":
-            nbcolor = [None, None, None]
             for t in range(3):
                 nbcolor[t] = 255 - obcolor[t]
         elif new_background == "red":
             nbcolor = [255, 0, 0]
 
         elif new_background == "green":
             nbcolor = [0, 255, 0]
@@ -452,104 +494,116 @@
 
         elif new_background == "orange":
             nbcolor = [255, 165, 0]
 
         # Change Background Color
         obcolor = tuple(obcolor)
         nbcolor = tuple(nbcolor)
-        for i in range(len(pixels)):
-            r, g, b = pixels[i]
-            if (obcolor[0] - stdRGB) <= r <= (obcolor[0] + stdRGB):
-                if (obcolor[1] - stdRGB) <= g <= (obcolor[1] + stdRGB):
-                    if (obcolor[2] - stdRGB) <= b <= (obcolor[2] + stdRGB):
-                        pixels[i] = nbcolor
+        for idx, pixel in enumerate(pixels):
+            if all(o - std_rgb <= p <= o + std_rgb for o, p in zip(obcolor, pixel)):
+                pixels[idx] = nbcolor
         img.putdata(pixels)
         img.save(newfile, "PNG")
         return newfile
     return pngfile
 
 
 def convert_image(
-    pngfile,
-    pf,
-    outdir=".",
-    resize=1000,
-    format="jpeg",
-    rotate=0,
-    rows=":",
-    cols=":",
-    labelrows=None,
-    labelcols=None,
-):
+    pngfile: str,
+    pf: str,
+    outdir: str = ".",
+    resize: int = 1000,
+    img_format: str = "jpeg",
+    rotate: int = 0,
+    rows: str = ":",
+    cols: str = ":",
+    labelrows: Optional[str] = None,
+    labelcols: Optional[str] = None,
+) -> Tuple[str, str, Optional[str], dict]:
+    """
+    Convert image to JPEG format and resize it.
+    """
     resizefile = op.join(outdir, pf + ".resize.jpg")
     mainfile = op.join(outdir, pf + ".main.jpg")
     labelfile = op.join(outdir, pf + ".label.jpg")
     img = Image(filename=pngfile)
-    exif = dict((k, v) for k, v in img.metadata.items() if k.startswith("exif:"))
+    exif = dict((k, img.metadata[k]) for k in img.metadata if k.startswith("exif:"))
 
     # Rotation, slicing and cropping of main image
     if rotate:
         img.rotate(rotate)
     if resize:
         w, h = img.size
         if min(w, h) > resize:
             if w < h:
                 nw, nh = resize, resize * h // w
             else:
                 nw, nh = resize * w // h, resize
             img.resize(nw, nh)
-            logging.debug(
-                "Image `{0}` resized from {1}px:{2}px to {3}px:{4}px".format(
-                    pngfile, w, h, nw, nh
-                )
+            logger.debug(
+                "Image `%s` resized from %dpx:%dpx to %dpx:%dpx", pngfile, w, h, nw, nh
             )
-    img.format = format
+    img.format = img_format
     img.save(filename=resizefile)
 
     rimg = img.clone()
     if rows != ":" or cols != ":":
         w, h = img.size
-        ra, rb = slice(rows, h)
-        ca, cb = slice(cols, w)
+        ra, rb = slice_to_ints(rows, h)
+        ca, cb = slice_to_ints(cols, w)
         # left, top, right, bottom
-        logging.debug("Crop image to {0}:{1} {2}:{3}".format(ra, rb, ca, cb))
+        logger.debug("Crop image to %d:%d %d:%d", ra, rb, ca, cb)
         img.crop(ca, ra, cb, rb)
-        img.format = format
+        img.format = img_format
         img.save(filename=mainfile)
     else:
         mainfile = resizefile
 
     # Extract text labels from image
     if labelrows or labelcols:
         w, h = rimg.size
         if labelrows and not labelcols:
             labelcols = ":"
         if labelcols and not labelrows:
             labelrows = ":"
-        ra, rb = slice(labelrows, h)
-        ca, cb = slice(labelcols, w)
-        logging.debug("Extract label from {0}:{1} {2}:{3}".format(ra, rb, ca, cb))
+        ra, rb = slice_to_ints(labelrows, h)
+        ca, cb = slice_to_ints(labelcols, w)
+        logger.debug("Extract label from %d:%d %d:%d", ra, rb, ca, cb)
         rimg.crop(ca, ra, cb, rb)
-        rimg.format = format
+        rimg.format = img_format
         rimg.save(filename=labelfile)
     else:
         labelfile = None
 
     return resizefile, mainfile, labelfile, exif
 
 
-def extract_label(labelfile):
+def extract_label(labelfile: str) -> str:
+    """
+    Extract accession number from label image.
+    """
     accession = image_to_string(iopen(labelfile))
     accession = " ".join(accession.split())  # normalize spaces
     accession = "".join(x for x in accession if x in string.printable)
     if not accession:
         accession = "none"
     return accession
 
 
+def efd_feature(contour: np.ndarray) -> np.ndarray:
+    """
+    To use EFD as features, one can write a small wrapper function.
+
+    Based on: https://pyefd.readthedocs.io/en/latest
+    """
+    coeffs = elliptic_fourier_descriptors(contour, normalize=True)
+    # skip the first three coefficients, which are always 1, 0, 0
+    return coeffs.flatten()[3:]
+
+
 def seeds(args):
     """
     %prog seeds [pngfile|jpgfile]
 
     Extract seed metrics from [pngfile|jpgfile]. Use --rows and --cols to crop image.
     """
     p = OptionParser(seeds.__doc__)
@@ -584,20 +638,18 @@
         cols=cols,
         labelrows=labelrows,
         labelcols=labelcols,
     )
     oimg = load_image(resizefile)
     img = load_image(mainfile)
 
-    fig, (ax1, ax2, ax3, ax4) = plt.subplots(
-        ncols=4, nrows=1, figsize=(iopts.w, iopts.h)
-    )
+    _, (ax1, ax2, ax3, ax4) = plt.subplots(ncols=4, nrows=1, figsize=(iopts.w, iopts.h))
     # Edge detection
     img_gray = rgb2gray(img)
-    logging.debug("Running {0} edge detection ...".format(ff))
+    logger.debug("Running %s edge detection ...", ff)
     if ff == "canny":
         edges = canny(img_gray, sigma=opts.sigma)
     elif ff == "roberts":
         edges = roberts(img_gray)
     elif ff == "sobel":
         edges = sobel(img_gray)
     edges = clear_border(edges, buffer_size=opts.border)
@@ -607,38 +659,40 @@
 
     # Watershed algorithm
     if opts.watershed:
         distance = distance_transform_edt(filled)
         local_maxi = peak_local_max(distance, threshold_rel=0.05, indices=False)
         coordinates = peak_local_max(distance, threshold_rel=0.05)
         markers, nmarkers = label(local_maxi, return_num=True)
-        logging.debug("Identified {0} watershed markers".format(nmarkers))
+        logger.debug("Identified %d watershed markers", nmarkers)
         labels = watershed(closed, markers, mask=filled)
     else:
         labels = label(filled)
 
     # Object size filtering
     w, h = img_gray.shape
     canvas_size = w * h
     min_size = int(round(canvas_size * opts.minsize / 100))
     max_size = int(round(canvas_size * opts.maxsize / 100))
-    logging.debug(
-        "Find objects with pixels between {0} ({1}%) and {2} ({3}%)".format(
-            min_size, opts.minsize, max_size, opts.maxsize
-        )
+    logger.debug(
+        "Find objects with pixels between %d (%d%%) and %d (%d%%)",
+        min_size,
+        opts.minsize,
+        max_size,
+        opts.maxsize,
     )
 
     # Plotting
     ax1.set_title("Original picture")
     ax1.imshow(oimg)
 
-    params = r"{0}, $\sigma$={1}, $k$={2}".format(ff, sigma, kernel)
+    params = rf"{ff}, $\sigma$={sigma}, $k$={kernel}"
     if opts.watershed:
         params += ", watershed"
-    ax2.set_title("Edge detection\n({0})".format(params))
+    ax2.set_title(f"Edge detection\n({params})")
     closed = gray2rgb(closed)
     ax2_img = labels
     if opts.edges:
         ax2_img = closed
     elif opts.watershed:
         ax2.plot(coordinates[:, 1], coordinates[:, 0], "g.")
     ax2.imshow(ax2_img, cmap=iopts.cmap)
@@ -652,66 +706,71 @@
     else:
         accession = pf
 
     # Calculate region properties
     rp = regionprops(labels)
     rp = [x for x in rp if min_size <= x.area <= max_size]
     nb_labels = len(rp)
-    logging.debug("A total of {0} objects identified.".format(nb_labels))
+    logger.debug("A total of %d objects identified.", nb_labels)
     objects = []
     for i, props in enumerate(rp):
         i += 1
         if i > opts.count:
             break
 
+        contour = find_contours(labels == props.label, 0.5)[0]
+        efds = efd_feature(contour)
         y0, x0 = props.centroid
         orientation = props.orientation
         major, minor = props.major_axis_length, props.minor_axis_length
-        major_dx = cos(orientation) * major / 2
-        major_dy = sin(orientation) * major / 2
-        minor_dx = sin(orientation) * minor / 2
-        minor_dy = cos(orientation) * minor / 2
-        ax2.plot((x0 - major_dx, x0 + major_dx), (y0 + major_dy, y0 - major_dy), "r-")
+        major_dx = sin(orientation) * major / 2
+        major_dy = cos(orientation) * major / 2
+        minor_dx = cos(orientation) * minor / 2
+        minor_dy = -sin(orientation) * minor / 2
+        ax2.plot((x0 - major_dx, x0 + major_dx), (y0 - major_dy, y0 + major_dy), "r-")
         ax2.plot((x0 - minor_dx, x0 + minor_dx), (y0 - minor_dy, y0 + minor_dy), "r-")
+        ax2.plot(contour[:, 1], contour[:, 0], "y-")
 
         npixels = int(props.area)
         # Sample the center of the blob for color
         d = min(int(round(minor / 2 * 0.35)) + 1, 50)
         x0d, y0d = int(round(x0)), int(round(y0))
         square = img[(y0d - d) : (y0d + d), (x0d - d) : (x0d + d)]
         pixels = []
         for row in square:
             pixels.extend(row)
-        logging.debug(
-            "Seed #{0}: {1} pixels ({2} sampled) - {3:.2f}%".format(
-                i, npixels, len(pixels), 100.0 * npixels / canvas_size
-            )
+        logger.debug(
+            "Seed #%d: %d pixels (%d sampled) - %.2f%%",
+            i,
+            npixels,
+            len(pixels),
+            100.0 * npixels / canvas_size,
         )
 
         rgb = pixel_stats(pixels)
-        objects.append(Seed(filename, accession, i, rgb, props, exif))
+        objects.append(Seed(filename, accession, i, rgb, props, efds, exif))
         minr, minc, maxr, maxc = props.bbox
         rect = Rectangle(
             (minc, minr), maxc - minc, maxr - minr, fill=False, ec="w", lw=1
         )
         ax3.add_patch(rect)
         mc, mr = (minc + maxc) // 2, (minr + maxr) // 2
-        ax3.text(mc, mr, "{0}".format(i), color="w", ha="center", va="center", size=6)
+        ax3.text(mc, mr, f"{i}", color="w", ha="center", va="center", size=6)
 
     for ax in (ax2, ax3):
         ax.set_xlim(0, h)
         ax.set_ylim(w, 0)
 
     # Output identified seed stats
-    ax4.text(0.1, 0.92, "File: {0}".format(latex(filename)), color="g")
-    ax4.text(0.1, 0.86, "Label: {0}".format(latex(accession)), color="m")
+    ax4.text(0.1, 0.92, f"File: {latex(filename)}", color="g")
+    ax4.text(0.1, 0.86, f"Label: {latex(accession)}", color="m")
     yy = 0.8
     fw = must_open(opts.outfile, "w")
     if not opts.noheader:
-        print(Seed.header(calibrate=calib), file=fw)
+        print(Seed.header(calibrated=calib), file=fw)
     for o in objects:
         if calib:
             o.calibrate(pixel_cm_ratio, tr)
         print(o, file=fw)
         i = o.seedno
         if i > 7:
             continue
@@ -722,24 +781,21 @@
             Rectangle((0.1, yy - 0.025), 0.12, 0.05, lw=0, fc=rgb_to_hex(o.rgb))
         )
         ax4.text(0.27, yy, o.hashtag, va="center")
         yy -= 0.06
     ax4.text(
         0.1,
         yy,
-        "(A total of {0} objects displayed)".format(nb_labels),
+        f"(A total of {nb_labels} objects displayed)",
         color="darkslategray",
     )
     normalize_axes(ax4)
 
     for ax in (ax1, ax2, ax3):
-        xticklabels = [int(x) for x in ax.get_xticks()]
-        yticklabels = [int(x) for x in ax.get_yticks()]
-        ax.set_xticklabels(xticklabels, family="Helvetica", size=8)
-        ax.set_yticklabels(yticklabels, family="Helvetica", size=8)
+        set_helvetica_axis(ax)
 
     image_name = op.join(outdir, pf + "." + iopts.format)
     savefig(image_name, dpi=iopts.dpi, iopts=iopts)
     return objects
 
 
 if __name__ == "__main__":
```

### Comparing `jcvi-1.4.2/jcvi/graphics/heatmap.py` & `jcvi-1.4.5/jcvi/graphics/heatmap.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/graphics/histogram.py` & `jcvi-1.4.5/jcvi/graphics/histogram.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     bins = defaultdict(int)
     for d in data:
         logd = int(log(d, base))
         bins[logd] += 1
 
     x, y = [], []
     for size, number in sorted(bins.items()):
-        lb, ub = base ** size, base ** (size + 1)
+        lb, ub = base**size, base ** (size + 1)
         x.append((lb, ub))
         y.append(number)
 
     asciiplot(x, y, title=title)
 
 
 def get_data(filename, vmin=None, vmax=None, skip=0, col=0):
```

### Comparing `jcvi-1.4.2/jcvi/graphics/karyotype.py` & `jcvi-1.4.5/jcvi/graphics/karyotype.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/graphics/landscape.py` & `jcvi-1.4.5/jcvi/graphics/landscape.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,39 +5,40 @@
 Create chromosome landscape plots that are similar to the ones used in soybean
 and sorghum paper.
 """
 
 
 import os.path as op
 import sys
-import logging
+
+from collections import Counter, OrderedDict, defaultdict
+from typing import List, Optional
 
 import numpy as np
 
-from collections import defaultdict, OrderedDict
+from ..algorithms.matrix import moving_sum
+from ..apps.base import OptionParser, ActionDispatcher, logger
+from ..formats.base import BaseFile, DictFile, LineFile, must_open
+from ..formats.bed import Bed, bins
+from ..formats.sizes import Sizes
+from ..utils.cbook import human_size, autoscale
 
-from jcvi.formats.sizes import Sizes
-from jcvi.formats.base import BaseFile, DictFile, LineFile, must_open
-from jcvi.formats.bed import Bed, bins
-from jcvi.algorithms.matrix import moving_sum
-from jcvi.graphics.base import (
-    plt,
-    Rectangle,
+from .base import (
     CirclePolygon,
-    savefig,
-    ticker,
+    Rectangle,
+    adjust_spines,
     human_readable_base,
     latex,
     markup,
-    set_human_axis,
     normalize_axes,
-    adjust_spines,
+    plt,
+    savefig,
+    set_human_axis,
+    ticker,
 )
-from jcvi.utils.cbook import human_size, autoscale
-from jcvi.apps.base import OptionParser, ActionDispatcher
 
 
 # Colors picked from Schmutz soybean genome paper using ColorPic
 palette = ["#ACABD5", "#DBF0F5", "#3EA77A", "#FBF5AB", "#C162A6"] + list("rgbymck")
 gray = "#CCCCCB"
 Registration = {
     "Gypsy": "LTR-RT/Gypsy",
@@ -88,15 +89,15 @@
         else:
             self.new_name = self.name
 
 
 class ChrInfoFile(BaseFile, OrderedDict):
     def __init__(self, filename, delimiter=","):
         super(ChrInfoFile, self).__init__(filename)
-        with open(filename) as fp:
+        with open(filename, encoding="utf-8") as fp:
             for row in fp:
                 if row[0] == "#":
                     continue
                 line = ChrInfoLine(row, delimiter=delimiter)
                 self[line.name] = line
 
 
@@ -109,15 +110,15 @@
         if len(args) > 2:
             self.subtitle = args[2]
 
 
 class TitleInfoFile(BaseFile, OrderedDict):
     def __init__(self, filename, delimiter=","):
         super(TitleInfoFile, self).__init__(filename)
-        with open(filename) as fp:
+        with open(filename, encoding="utf-8") as fp:
             for row in fp:
                 if row[0] == "#":
                     continue
                 line = TitleInfoLine(row, delimiter=delimiter)
                 self[line.name] = line
 
 
@@ -144,23 +145,21 @@
     chr01A  50000   100000  36.00
     chr01A  100000  150000  280.00
     chr01A  150000  200000  190.00
 
     Args:
         filename (str): Path to the file.
     """
-    from collections import defaultdict, Counter
-
     dists = defaultdict(Counter)
     with must_open(filename) as fp:
         for row in fp:
             chromosome, start, end, depth = row.split()
             depth = int(float(depth))
             dists[chromosome][depth] += 1
-    logging.debug("Loaded {} seqids".format(len(dists)))
+    logger.debug("Loaded %d seqids", len(dists))
     return dists
 
 
 def parse_groupsfile(filename):
     """Parse groupsfile, which contains the tracks to be plotted
     in the vertically stacked mosdepth plot.
 
@@ -172,15 +171,15 @@
         filename (str): Path to the groups file.
     """
     groups = []
     with open(filename) as fp:
         for row in fp:
             chrs, colors = row.split()
             groups.append((chrs.split(","), colors.split(",")))
-    logging.debug("Loaded {} groups".format(len(groups)))
+    logger.debug("Loaded %d groups", len(groups))
     return groups
 
 
 def cumarray_to_array(ar):
     """Convert cumulative array to normal array.
 
     Args:
@@ -217,27 +216,27 @@
     distfile, groupsfile = args
     dists = parse_distfile(distfile)
     groups = parse_groupsfile(groupsfile)
     logscale = opts.logscale
 
     # Construct a composite figure with N tracks indicated in the groups
     fig = plt.figure(1, (iopts.w, iopts.h))
-    root = fig.add_axes([0, 0, 1, 1])
+    root = fig.add_axes((0, 0, 1, 1))
 
     rows = len(groups)
     ypad = 0.05
     yinterval = (1 - 2 * ypad) / (rows + 1)
     yy = 1 - ypad
 
     for group_idx, (chrs, colors) in enumerate(groups):
         yy -= yinterval
-        ax = fig.add_axes([0.15, yy, 0.7, yinterval * 0.85])
+        ax = fig.add_axes((0.15, yy, 0.7, yinterval * 0.85))
         for c, color in zip(chrs, colors):
             cdata = dists[c].items()
-            logging.debug("Importing {} records for {}".format(len(cdata), c))
+            logger.debug("Importing %d records for %s", len(cdata), c)
             cx, cy = zip(*sorted(cdata))
             ax.plot(cx, cy, "-", color=color)
         if logscale:
             ax.set_xscale("log", basex=2)
         ax.set_xlim(1 if logscale else 0, opts.maxdepth)
         ax.get_yaxis().set_visible(False)
         if group_idx != rows - 1:
@@ -267,33 +266,33 @@
     image_name = pf + "." + iopts.format
     savefig(image_name, dpi=iopts.dpi, iopts=iopts)
 
 
 def draw_depth(
     root,
     ax,
-    bed,
-    chrinfo={},
-    defaultcolor="k",
-    sepcolor="w",
-    ylim=100,
-    logscale=False,
-    title=None,
-    subtitle=None,
+    bed: Bed,
+    chrinfo: dict = {},
+    defaultcolor: str = "k",
+    sepcolor: str = "w",
+    maxdepth: int = 100,
+    logscale: bool = False,
+    title: Optional[str] = None,
+    subtitle: Optional[str] = None,
 ):
     """Draw depth plot on the given axes, using data from bed
 
     Args:
         root (matplotlib.Axes): Canvas axes
         ax (matplotlib.Axes): Axes to plot data on
         bed (Bed): Bed data from mosdepth
         chrinfo (ChrInfoFile): seqid => color, new name
         defaultcolor (str): matplotlib-compatible color for data points
         sepcolor (str): matplotlib-compatible color for chromosome breaks
-        ylim (int): Upper limit of the y-axis (depth)
+        maxdepth (int): Upper limit of the y-axis (depth)
         title (str): Title of the figure, to the right of the axis
         subtitle (str): Subtitle of the figure, just below title
     """
     if chrinfo is None:
         chrinfo = {}
     sizes = bed.max_bp_in_chr
     seqids = chrinfo.keys() if chrinfo else sizes.keys()
@@ -330,15 +329,15 @@
         x,
         y,
         c=c,
         edgecolors="none",
         s=8,
         lw=0,
     )
-    logging.debug("Obtained {} data points with depth data".format(len(data)))
+    logger.debug("Obtained %d data points with depth data", len(data))
 
     # Per seqid median
     medians = {}
     for seqid, values in data_by_seqid.items():
         c = chrinfo[seqid].color if seqid in chrinfo else defaultcolor
         seqid_start = starts[seqid]
         seqid_end = ends[seqid]
@@ -349,19 +348,19 @@
             (seqid_median, seqid_median),
             "-",
             lw=4,
             color=c,
             alpha=0.5,
         )
 
-    # vertical lines for all the breaks
+    # Vertical lines for all the breaks
     for pos in starts.values():
-        ax.plot((pos, pos), (0, ylim), "-", lw=1, color=sepcolor)
+        ax.plot((pos, pos), (0, maxdepth), "-", lw=1, color=sepcolor)
 
-    # beautify the numeric axis
+    # Beautify the numeric axis
     for tick in ax.get_xticklines() + ax.get_yticklines():
         tick.set_visible(False)
 
     median_depth_y = 0.88
     chr_label_y = 0.08
     for seqid, position in label_positions:
         xpos = 0.1 + position * 0.8 / xsize
@@ -376,14 +375,23 @@
             median_depth_y,
             str(int(seqid_median)),
             color=c,
             ha="center",
             va="center",
         )
 
+    # Add an arrow to the right of the plot, indicating these are median depths
+    root.text(
+        0.91,
+        0.88,
+        r"$\leftarrow$median",
+        color="lightslategray",
+        va="center",
+    )
+
     if title:
         root.text(
             0.95,
             0.5,
             markup(title),
             color="darkslategray",
             ha="center",
@@ -401,22 +409,68 @@
             size=15,
         )
 
     ax.set_xticks([])
     ax.set_xlim(0, xsize)
     if logscale:
         ax.set_yscale("log", basey=2)
-    ax.set_ylim(1 if logscale else 0, ylim)
+    ax.set_ylim(1 if logscale else 0, maxdepth)
     ax.set_ylabel("Depth")
 
     set_human_axis(ax)
     plt.setp(ax.get_xticklabels() + ax.get_yticklabels(), color="gray", size=10)
     normalize_axes(root)
 
 
+def draw_multi_depth(
+    root,
+    panel_roots,
+    panel_axes,
+    bedfiles: List[str],
+    chrinfo_file: str,
+    titleinfo_file: str,
+    maxdepth: int,
+    logscale: bool,
+):
+    """
+    Draw multiple depth plots on the same canvas.
+    """
+    chrinfo = ChrInfoFile(chrinfo_file) if chrinfo_file else {}
+    titleinfo = TitleInfoFile(titleinfo_file) if titleinfo_file else {}
+    npanels = len(bedfiles)
+    yinterval = 1.0 / npanels
+    ypos = 1 - yinterval
+    for bedfile, panel_root, panel_ax in zip(bedfiles, panel_roots, panel_axes):
+        pf = op.basename(bedfile).split(".", 1)[0]
+        bed = Bed(bedfile)
+
+        if ypos > 0.001:
+            root.plot((0.02, 0.98), (ypos, ypos), "-", lw=2, color="lightslategray")
+
+        title = titleinfo.get(bedfile, pf.split("_", 1)[0])
+        subtitle = None
+        if isinstance(title, TitleInfoLine):
+            subtitle = title.subtitle
+            title = title.title
+
+        draw_depth(
+            panel_root,
+            panel_ax,
+            bed,
+            chrinfo=chrinfo,
+            maxdepth=maxdepth,
+            logscale=logscale,
+            title=title,
+            subtitle=subtitle,
+        )
+        ypos -= yinterval
+
+    normalize_axes(root)
+
+
 def depth(args):
     """
     %prog depth *.regions.bed.gz
 
     Plot the mosdepth regions BED file. We recommend to generate this BED file
     by (please adjust the --by parameter to your required resolution):
 
@@ -451,51 +505,39 @@
     )
     opts, args, iopts = p.set_image_options(args, style="dark", figsize="14x4")
 
     if len(args) < 1:
         sys.exit(not p.print_help())
 
     bedfiles = args
-    chrinfo = ChrInfoFile(opts.chrinfo) if opts.chrinfo else {}
-    titleinfo = TitleInfoFile(opts.titleinfo) if opts.titleinfo else {}
 
     fig = plt.figure(1, (iopts.w, iopts.h))
-    root = fig.add_axes([0, 0, 1, 1])
+    root = fig.add_axes((0, 0, 1, 1))
 
     npanels = len(bedfiles)
     yinterval = 1.0 / npanels
     ypos = 1 - yinterval
-    for bedfile in bedfiles:
-        pf = op.basename(bedfile).split(".", 1)[0]
-        bed = Bed(bedfile)
-
-        panel_root = root if npanels == 1 else fig.add_axes([0, ypos, 1, yinterval])
-        panel_ax = fig.add_axes([0.1, ypos + 0.2 * yinterval, 0.8, 0.65 * yinterval])
-        if ypos > 0.001:
-            root.plot((0, 1), (ypos, ypos), "-", lw=2, color="lightslategray")
-
-        title = titleinfo.get(bedfile, pf.split("_", 1)[0])
-        subtitle = None
-        if isinstance(title, TitleInfoLine):
-            subtitle = title.subtitle
-            title = title.title
-
-        draw_depth(
-            panel_root,
-            panel_ax,
-            bed,
-            chrinfo=chrinfo,
-            ylim=opts.maxdepth,
-            logscale=opts.logscale,
-            title=title,
-            subtitle=subtitle,
-        )
+    panel_roots, panel_axes = [], []
+    for _ in range(npanels):
+        panel_root = root if npanels == 1 else fig.add_axes((0, ypos, 1, yinterval))
+        panel_ax = fig.add_axes((0.1, ypos + 0.2 * yinterval, 0.8, 0.65 * yinterval))
+        panel_roots.append(panel_root)
+        panel_axes.append(panel_ax)
         ypos -= yinterval
 
-    normalize_axes(root)
+    draw_multi_depth(
+        root,
+        panel_roots,
+        panel_axes,
+        bedfiles,
+        opts.chrinfo,
+        opts.titleinfo,
+        opts.maxdepth,
+        opts.logscale,
+    )
 
     if npanels > 1:
         pf = op.commonprefix(bedfiles)
     pf = pf or "depth"
     image_name = pf + "." + iopts.format
     savefig(image_name, dpi=iopts.dpi, iopts=iopts)
 
@@ -510,18 +552,19 @@
 
 
 def check_window_options(opts):
     window = opts.window
     shift = opts.shift
     subtract = opts.subtract
     assert window % shift == 0, "--window must be divisible by --shift"
-    logging.debug(
-        "Line/stack-plot options: window={0} shift={1} subtract={2}".format(
-            window, shift, subtract
-        )
+    logger.debug(
+        "Line/stack-plot options: window=%d shift=%d subtract=%d",
+        window,
+        shift,
+        subtract,
     )
     merge = not opts.nomerge
 
     return window, shift, subtract, merge
 
 
 def get_beds(s, binned=False):
@@ -637,23 +680,23 @@
     clen = Sizes(fastafile).mapping[chr]
     nbins = get_nbins(clen, shift)
 
     plt.rcParams["xtick.major.size"] = 0
     plt.rcParams["ytick.major.size"] = 0
 
     fig = plt.figure(1, (iopts.w, iopts.h))
-    root = fig.add_axes([0, 0, 1, 1])
+    root = fig.add_axes((0, 0, 1, 1))
 
     root.text(0.5, 0.95, chr, ha="center", color="darkslategray")
 
     xstart, xend = margin, 1 - margin
     xlen = xend - xstart
     ratio = xlen / clen
     # Line plots
-    ax = fig.add_axes([xstart, 0.6, xlen, 0.3])
+    ax = fig.add_axes((xstart, 0.6, xlen, 0.3))
     lineplot(ax, linebins, nbins, chr, window, shift)
 
     # Bar plots
     yy = 0.5
     yinterval = 0.08
     xs = lambda x: xstart + ratio * x
     r = 0.01
@@ -818,30 +861,30 @@
     )
 
     margin = 0.06
     inner = 0.015
     clen = Sizes(fastafile).mapping[chr]
 
     fig = plt.figure(1, (iopts.w, iopts.h))
-    root = fig.add_axes([0, 0, 1, 1])
+    root = fig.add_axes((0, 0, 1, 1))
 
     # Gauge
     ratio = draw_gauge(root, margin, clen, rightmargin=4 * margin)
     yinterval = 0.3
     xx = margin
     yy = 1 - margin
     yy -= yinterval
     xlen = clen / ratio
     cc = chr
     if "_" in chr:
         ca, cb = chr.split("_")
         cc = ca[0].upper() + cb
 
     root.add_patch(Rectangle((xx, yy), xlen, yinterval - inner, color=gray))
-    ax = fig.add_axes([xx, yy, xlen, yinterval - inner])
+    ax = fig.add_axes((xx, yy, xlen, yinterval - inner))
 
     nbins = get_nbins(clen, shift)
 
     owindow = clen / 100
     if owindow > window:
         window = owindow / shift * shift
 
@@ -1024,15 +1067,15 @@
     s = list(sizes.iter_sizes())[:top]
     maxl = max(x[1] for x in s)
     margin = 0.08
     inner = 0.02  # y distance between tracks
 
     pf = fastafile.rsplit(".", 1)[0]
     fig = plt.figure(1, (iopts.w, iopts.h))
-    root = fig.add_axes([0, 0, 1, 1])
+    root = fig.add_axes((0, 0, 1, 1))
 
     # Gauge
     ratio = draw_gauge(root, margin, maxl)
 
     # Per chromosome
     yinterval = (1 - 2 * margin) / (top + 1)
     xx = margin
@@ -1045,15 +1088,15 @@
             ca, cb = chr.split("_")
             cc = ca[0].upper() + cb
 
         if switch and cc in switch:
             cc = "\n".join((cc, "({0})".format(switch[cc])))
 
         root.add_patch(Rectangle((xx, yy), xlen, yinterval - inner, color=gray))
-        ax = fig.add_axes([xx, yy, xlen, yinterval - inner])
+        ax = fig.add_axes((xx, yy, xlen, yinterval - inner))
 
         nbins = clen / shift
         if clen % shift:
             nbins += 1
 
         stackplot(ax, binfiles, nbins, palette, chr, window, shift)
         root.text(
```

### Comparing `jcvi-1.4.2/jcvi/graphics/mummerplot.py` & `jcvi-1.4.5/jcvi/graphics/mummerplot.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/graphics/synteny.py` & `jcvi-1.4.5/jcvi/graphics/synteny.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/graphics/table.py` & `jcvi-1.4.5/jcvi/graphics/table.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/graphics/tree.py` & `jcvi-1.4.5/jcvi/graphics/tree.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/graphics/wheel.py` & `jcvi-1.4.5/jcvi/graphics/wheel.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/projects/age.py` & `jcvi-1.4.5/jcvi/projects/age.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/projects/allmaps.py` & `jcvi-1.4.5/jcvi/projects/allmaps.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/projects/bites.py` & `jcvi-1.4.5/jcvi/projects/bites.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/projects/ies.py` & `jcvi-1.4.5/jcvi/projects/ies.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/projects/misc.py` & `jcvi-1.4.5/jcvi/projects/misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
         ("amborella", "plot amborella macro- and micro-synteny (requires data)"),
         # Mt4.0 paper (Tang et al., 2014 BMC Genomics)
         ("mtdotplots", "plot Mt3.5 and Mt4.0 side-by-side"),
         # Oropetium paper (Vanburen et al., 2015 Nature)
         ("oropetium", "plot oropetium micro-synteny (requires data)"),
         # Pomegranate paper (Qin et al., 2017 Plant Journal)
         ("pomegranate", "plot pomegranate macro- and micro-synteny (requires data)"),
-        # Unpublished
         ("birch", "plot birch macro-synteny (requires data)"),
         ("litchi", "plot litchi micro-synteny (requires data)"),
         ("utricularia", "plot utricularia micro-synteny (requires data)"),
         (
             "waterlilyGOM",
             "waterlily phylogeny and related infographics (requires data)",
         ),
@@ -72,15 +71,15 @@
 
     logging.debug("Load tree file `{0}`".format(datafile))
     t, hpd = parse_tree(datafile)
 
     pf = datafile.rsplit(".", 1)[0]
 
     fig = plt.figure(1, (iopts.w, iopts.h))
-    root = fig.add_axes([0, 0, 1, 1])
+    root = fig.add_axes((0, 0, 1, 1))
 
     margin, rmargin = 0.15, 0.19  # Left and right margin
     leafinfo = LeafInfoFile("leafinfo.csv").cache
     wgdinfo = WGDInfoFile("wgdinfo.csv").cache
     groups = "Monocots,Eudicots,ANA-grade,Gymnosperms"
 
     draw_tree(
```

### Comparing `jcvi-1.4.2/jcvi/projects/napus.py` & `jcvi-1.4.5/jcvi/projects/napus.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/projects/pineapple.py` & `jcvi-1.4.5/jcvi/projects/pineapple.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/projects/str.py` & `jcvi-1.4.5/jcvi/projects/str.py`

 * *Files 0% similar despite different names*

```diff
@@ -352,15 +352,15 @@
         for proband, proband_sex, p1, p1_sex, p2, p2_sex in trios:
             tp1 = tredcall(p1)
             tp2 = tredcall(p2)
             tpp = tredcall(proband)
             m = mendelian_check(tp1, tp2, tpp, is_xlinked=is_xlinked)
             counts[m] += 1
             if is_xlinked:
-                for (p, p_sex) in ((tp1, p1_sex), (tp2, p2_sex), (tpp, proband_sex)):
+                for p, p_sex in ((tp1, p1_sex), (tp2, p2_sex), (tpp, proband_sex)):
                     if p[1].startswith("-"):
                         p[1] = "n.a."
             cells = [shorten(p1), p1_sex] + tp1[1:]
             cells += [shorten(p2), p2_sex] + tp2[1:]
             cells += [shorten(proband), proband_sex] + tpp[1:]
             print("\t".join([m] + cells), file=fw)
         fw.close()
@@ -587,15 +587,15 @@
         ncols=2, nrows=2, figsize=(iopts.w, iopts.h)
     )
     plt.tight_layout(pad=6)
 
     data = pd.read_csv(tsvfile, sep="\t", low_memory=False)
 
     ids, treds = read_treds()
-    for (dp, ax, title) in zip(
+    for dp, ax, title in zip(
         ("FDP", "PDP", "RDP", "PEDP"),
         (ax1, ax2, ax3, ax4),
         ("Spanning reads", "Partial reads", "Repeat-only reads", "Paired-end reads"),
     ):
         logging.debug("Build {}".format(title))
         # Construct related data structure
         xd = []  # (tred, dp)
```

### Comparing `jcvi-1.4.2/jcvi/projects/sugarcane.py` & `jcvi-1.4.5/jcvi/projects/sugarcane.py`

 * *Files 0% similar despite different names*

```diff
@@ -693,15 +693,15 @@
     SPECIES_CONFIG = {
         "SS": {"label": "S. spontaneum", "pos": (0.5, 0.67)},
         "SR": {"label": "S. robustum", "pos": (0.2, 0.3)},
         "SO": {"label": "S. officinarum", "pos": (0.8, 0.3)},
     }
     # Get median for each genome pair
     medians = {}
-    for (g1, g2) in product(SPECIES_CONFIG.keys(), repeat=2):
+    for g1, g2 in product(SPECIES_CONFIG.keys(), repeat=2):
         g1, g2 = sorted((g1, g2))
         d = data_by_genomes[(g1, g2)]
         medians[(g1, g2)] = np.median(d)
     for g, config in SPECIES_CONFIG.items():
         x, y = config["pos"]
         text = f'*{config["label"]}*' + f"\n{medians[(g, g)]:.1f} %"
         text = markup(text)
```

### Comparing `jcvi-1.4.2/jcvi/projects/synfind.py` & `jcvi-1.4.5/jcvi/projects/synfind.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/projects/tgbs.py` & `jcvi-1.4.5/jcvi/projects/tgbs.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/projects/vanilla.py` & `jcvi-1.4.5/jcvi/projects/vanilla.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/utils/aws.py` & `jcvi-1.4.5/jcvi/utils/aws.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/utils/cbook.py` & `jcvi-1.4.5/jcvi/utils/cbook.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Useful recipes from various internet sources (thanks)
 mostly decorator patterns
 """
+
 import os.path as op
 import re
 import sys
 import logging
 
 from collections import defaultdict
```

### Comparing `jcvi-1.4.2/jcvi/utils/data/Airswing.ttf` & `jcvi-1.4.5/jcvi/utils/data/Airswing.ttf`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/utils/data/Collegia.ttf` & `jcvi-1.4.5/jcvi/utils/data/Collegia.ttf`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/utils/data/HookedUp.ttf` & `jcvi-1.4.5/jcvi/utils/data/HookedUp.ttf`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/utils/data/Humor-Sans.ttf` & `jcvi-1.4.5/jcvi/utils/data/Humor-Sans.ttf`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/utils/data/TREDs.meta.csv` & `jcvi-1.4.5/jcvi/utils/data/TREDs.meta.csv`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/utils/data/adapters.fasta` & `jcvi-1.4.5/jcvi/utils/data/adapters.fasta`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/utils/data/blosum80.mat` & `jcvi-1.4.5/jcvi/utils/data/blosum80.mat`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/utils/data/chrY.hg38.unique_ccn.gc` & `jcvi-1.4.5/jcvi/utils/data/chrY.hg38.unique_ccn.gc`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/utils/data/hg38.band.txt` & `jcvi-1.4.5/jcvi/utils/data/hg38.band.txt`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/utils/data/hg38.chrom.sizes` & `jcvi-1.4.5/jcvi/utils/data/hg38.chrom.sizes`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/utils/data/instance.json` & `jcvi-1.4.5/jcvi/utils/data/instance.json`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/utils/db.py` & `jcvi-1.4.5/jcvi/utils/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from jcvi.formats.base import must_open
 from jcvi.apps.base import OptionParser, ActionDispatcher, sh, getusername
 from jcvi.utils.cbook import AutoVivification
 
 
 # set up valid database connection params
 valid_dbconn = AutoVivification()
-for (dbconn, port, module, host) in zip(
+for dbconn, port, module, host in zip(
     ("Sybase", "MySQL", "PostgreSQL", "Oracle"),
     (2025, 3306, 5432, 1521),
     ("Sybase", "MySQLdb", "psycopg2", "cx_Oracle"),
     ("SYBPROD", "mysql-lan-dev", "pgsql-lan-dev", "DBNAME.tacc.utexas.edu"),
 ):
     valid_dbconn[dbconn]["port"] = port
     valid_dbconn[dbconn]["module"] = module
```

### Comparing `jcvi-1.4.2/jcvi/utils/ez_setup.py` & `jcvi-1.4.5/jcvi/utils/ez_setup.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/utils/grouper.py` & `jcvi-1.4.5/jcvi/utils/grouper.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/utils/orderedcollections.py` & `jcvi-1.4.5/jcvi/utils/orderedcollections.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/utils/range.py` & `jcvi-1.4.5/jcvi/utils/range.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/utils/table.py` & `jcvi-1.4.5/jcvi/utils/table.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/utils/taxonomy.py` & `jcvi-1.4.5/jcvi/utils/taxonomy.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/utils/validator.py` & `jcvi-1.4.5/jcvi/utils/validator.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/utils/webcolors.py` & `jcvi-1.4.5/jcvi/utils/webcolors.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/variation/cnv.py` & `jcvi-1.4.5/jcvi/variation/cnv.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/variation/deconvolute.py` & `jcvi-1.4.5/jcvi/variation/deconvolute.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/variation/delly.py` & `jcvi-1.4.5/jcvi/variation/delly.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/variation/impute.py` & `jcvi-1.4.5/jcvi/variation/impute.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/variation/phase.py` & `jcvi-1.4.5/jcvi/variation/phase.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/variation/snp.py` & `jcvi-1.4.5/jcvi/variation/snp.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi/variation/str.py` & `jcvi-1.4.5/jcvi/variation/str.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.2/jcvi.egg-info/PKG-INFO` & `jcvi-1.4.5/jcvi.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,24 @@
 Metadata-Version: 2.1
 Name: jcvi
-Version: 1.4.2
+Version: 1.4.5
 Summary: Python utility libraries on genome assembly, annotation and comparative genomics
 Home-page: http://github.com/tanghaibao/jcvi
 Author: Haibao Tang, Vivek Krishnakumar, Jingping Li
 Author-email: tanghaibao@gmail.com
 License: BSD
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: CrossMap
-Requires-Dist: PyPDF2
-Requires-Dist: biopython
-Requires-Dist: boto3
-Requires-Dist: brewer2mpl
-Requires-Dist: deap
-Requires-Dist: ete3
-Requires-Dist: ftpretty
-Requires-Dist: gffutils
-Requires-Dist: goatools
-Requires-Dist: genomepy
-Requires-Dist: graphviz
-Requires-Dist: jinja2
-Requires-Dist: matplotlib
-Requires-Dist: more-itertools
-Requires-Dist: natsort
-Requires-Dist: networkx
-Requires-Dist: numpy
-Requires-Dist: ortools
-Requires-Dist: pybedtools
-Requires-Dist: rich
-Requires-Dist: scikit-image
-Requires-Dist: scipy
-Requires-Dist: seaborn
-Requires-Dist: webcolors
 
 # JCVI utility libraries
 
 [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.31631.svg)](https://doi.org/10.5281/zenodo.594205)
 [![Latest PyPI version](https://img.shields.io/pypi/v/jcvi.svg)](https://pypi.python.org/pypi/jcvi)
 [![bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/jcvi/README.html?highlight=jcvi)
 [![Github Actions](https://github.com/tanghaibao/jcvi/workflows/build/badge.svg)](https://github.com/tanghaibao/jcvi/actions)
@@ -246,7 +222,9 @@
 **Feel free to check out other scripts in the package, it is not just
 for FASTA.**
 
 ## Star History
 
 [![Star History
 Chart](https://api.star-history.com/svg?repos=tanghaibao/jcvi&type=Date)](https://star-history.com/#tanghaibao/jcvi&Date)
+
+
```

### Comparing `jcvi-1.4.2/jcvi.egg-info/SOURCES.txt` & `jcvi-1.4.5/jcvi.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 jcvi/algorithms/ec.py
 jcvi/algorithms/formula.py
 jcvi/algorithms/graph.py
 jcvi/algorithms/lis.py
 jcvi/algorithms/lpsolve.py
 jcvi/algorithms/matrix.py
 jcvi/algorithms/maxsum.py
-jcvi/algorithms/ml.py
 jcvi/algorithms/supermap.py
 jcvi/algorithms/tsp.py
 jcvi/annotation/__init__.py
 jcvi/annotation/__main__.py
 jcvi/annotation/ahrd.py
 jcvi/annotation/automaton.py
 jcvi/annotation/depth.py
@@ -46,21 +45,19 @@
 jcvi/apps/bwa.py
 jcvi/apps/cdhit.py
 jcvi/apps/emboss.py
 jcvi/apps/fetch.py
 jcvi/apps/gbsubmit.py
 jcvi/apps/gmap.py
 jcvi/apps/grid.py
-jcvi/apps/ks.py
 jcvi/apps/lastz.py
 jcvi/apps/mask.py
 jcvi/apps/phylo.py
 jcvi/apps/r.py
 jcvi/apps/restriction.py
-jcvi/apps/script.py
 jcvi/apps/softlink.py
 jcvi/apps/uclust.py
 jcvi/apps/uniprot.py
 jcvi/apps/vecscreen.py
 jcvi/assembly/__init__.py
 jcvi/assembly/__main__.py
 jcvi/assembly/allmaps.py
@@ -85,15 +82,17 @@
 jcvi/assembly/trinity.py
 jcvi/compara/__init__.py
 jcvi/compara/__main__.py
 jcvi/compara/base.py
 jcvi/compara/blastfilter.py
 jcvi/compara/catalog.py
 jcvi/compara/fractionation.py
+jcvi/compara/ks.py
 jcvi/compara/pad.py
+jcvi/compara/pedigree.py
 jcvi/compara/phylogeny.py
 jcvi/compara/quota.py
 jcvi/compara/reconstruct.py
 jcvi/compara/synfind.py
 jcvi/compara/synteny.py
 jcvi/formats/__init__.py
 jcvi/formats/__main__.py
@@ -128,38 +127,33 @@
 jcvi/graphics/base.py
 jcvi/graphics/blastplot.py
 jcvi/graphics/chromosome.py
 jcvi/graphics/coverage.py
 jcvi/graphics/dotplot.py
 jcvi/graphics/glyph.py
 jcvi/graphics/grabseeds.py
-jcvi/graphics/graph.py
 jcvi/graphics/heatmap.py
 jcvi/graphics/histogram.py
 jcvi/graphics/karyotype.py
 jcvi/graphics/landscape.py
-jcvi/graphics/logo.py
 jcvi/graphics/mummerplot.py
 jcvi/graphics/synteny.py
 jcvi/graphics/table.py
 jcvi/graphics/tree.py
 jcvi/graphics/wheel.py
-jcvi/graphics/whisker.py
 jcvi/projects/__init__.py
 jcvi/projects/__main__.py
 jcvi/projects/age.py
-jcvi/projects/alfalfa.py
 jcvi/projects/allmaps.py
 jcvi/projects/bites.py
-jcvi/projects/heterosis.py
 jcvi/projects/ies.py
+jcvi/projects/jcvi.py
 jcvi/projects/misc.py
 jcvi/projects/napus.py
 jcvi/projects/pineapple.py
-jcvi/projects/pistachio.py
 jcvi/projects/str.py
 jcvi/projects/sugarcane.py
 jcvi/projects/synfind.py
 jcvi/projects/tgbs.py
 jcvi/projects/vanilla.py
 jcvi/utils/__init__.py
 jcvi/utils/__main__.py
@@ -192,9 +186,8 @@
 jcvi/variation/__main__.py
 jcvi/variation/cnv.py
 jcvi/variation/deconvolute.py
 jcvi/variation/delly.py
 jcvi/variation/impute.py
 jcvi/variation/phase.py
 jcvi/variation/snp.py
-jcvi/variation/str.py
-jcvi/variation/tassel.py
+jcvi/variation/str.py
```

### Comparing `jcvi-1.4.2/setup.cfg` & `jcvi-1.4.5/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 	matplotlib
 	more-itertools
 	natsort
 	networkx
 	numpy
 	ortools
 	pybedtools
+	pyefd
 	rich
 	scikit-image
 	scipy
 	seaborn
 	webcolors
 include_package_data = True
 tests_require = PyYAML; pytest; pytest-cov; pytest-benchmark; mock
```

### Comparing `jcvi-1.4.2/setup.py` & `jcvi-1.4.5/setup.py`

 * *Files identical despite different names*

