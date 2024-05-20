# Comparing `tmp/bioframe-0.6.4.tar.gz` & `tmp/bioframe-0.7.0.tar.gz`

## Comparing `bioframe-0.6.4.tar` & `bioframe-0.7.0.tar`

### file list

```diff
@@ -1,99 +1,111 @@
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 bioframe-0.6.4/.readthedocs.yaml
--rw-r--r--   0        0        0     8742 2020-02-02 00:00:00.000000 bioframe-0.6.4/CHANGES.md
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 bioframe-0.6.4/CITATION.cff
--rw-r--r--   0        0        0     4865 2020-02-02 00:00:00.000000 bioframe-0.6.4/CONTRIBUTING.md
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 bioframe-0.6.4/.github/workflows/ci.yml
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 bioframe-0.6.4/.github/workflows/publish.yml
--rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/__init__.py
--rw-r--r--   0        0        0    16583 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/extras.py
--rw-r--r--   0        0        0    64680 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/ops.py
--rw-r--r--   0        0        0     6495 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/vis.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/core/__init__.py
--rw-r--r--   0        0        0    25601 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/core/arrops.py
--rw-r--r--   0        0        0    15578 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/core/checks.py
--rw-r--r--   0        0        0    11535 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/core/construction.py
--rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/core/specs.py
--rw-r--r--   0        0        0     7009 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/core/stringops.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/__init__.py
--rw-r--r--   0        0        0     5667 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/assembly.py
--rw-r--r--   0        0        0    18716 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/fileops.py
--rw-r--r--   0        0        0     8639 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/resources.py
--rw-r--r--   0        0        0     5223 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/schemas.py
--rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/data/_assemblies.yml
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/data/ce10.seqinfo.tsv
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/data/ce11.seqinfo.tsv
--rw-r--r--   0        0        0    70878 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/data/danRer10.seqinfo.tsv
--rw-r--r--   0        0        0    66339 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/data/danRer11.seqinfo.tsv
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/data/dm3.seqinfo.tsv
--rw-r--r--   0        0        0   161973 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/data/dm6.seqinfo.tsv
--rw-r--r--   0        0        0    30781 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/data/hg19.cytoband.tsv
--rw-r--r--   0        0        0     6881 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/data/hg19.seqinfo.tsv
--rw-r--r--   0        0        0    30775 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/data/hg38.cytoband.tsv
--rw-r--r--   0        0        0    16501 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/data/hg38.seqinfo.tsv
--rw-r--r--   0        0        0    30780 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/data/hs1.cytoband.tsv
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/data/hs1.seqinfo.tsv
--rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/data/mm10.seqinfo.tsv
--rw-r--r--   0        0        0     4802 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/data/mm39.seqinfo.tsv
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/data/mm9.seqinfo.tsv
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/data/sacCer3.seqinfo.tsv
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/io/data/wuhCor1.seqinfo.tsv
--rw-r--r--   0        0        0     5776 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/sandbox/clients.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/sandbox/gtf_io.py
--rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 bioframe-0.6.4/bioframe/sandbox/parquet_io.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/Makefile
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/api-construction.rst
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/api-extras.rst
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/api-fileops.rst
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/api-intervalops.rst
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/api-lowlevel.md
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/api-resources.rst
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/api-validation.rst
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/api-vis.rst
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/conf.py
--rw-r--r--   0        0        0     4847 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/guide-definitions.rst
--rw-r--r--   0        0        0    16241 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/guide-intervalops.md
--rw-r--r--   0        0        0    13704 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/guide-io.ipynb
--rw-r--r--   0        0        0   374027 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/guide-performance.ipynb
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/guide-quickstart.rst
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/guide-recipes.md
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/guide-specifications.rst
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/index.rst
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/make.bat
--rw-r--r--   0        0        0    38715 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/times100.bw
--rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/figs/._bioframe-logo.png
--rw-r--r--   0        0        0    68759 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/figs/bioframe-logo.png
--rw-r--r--   0        0        0    65297 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/figs/bioframe_closest.pdf
--rw-r--r--   0        0        0    21587 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/figs/closest0.png
--rw-r--r--   0        0        0    56069 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/figs/closest1.png
--rw-r--r--   0        0        0    50871 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/figs/closest2.png
--rw-r--r--   0        0        0    44726 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/figs/closest3.png
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/figs/df1.png
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/figs/df2.png
--rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/figs/df@.png
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/figs/merge_df1.png
--rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/figs/overlap_inner_0.png
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/figs/overlap_inner_1.png
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/lowlevel/arrops.rst
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/lowlevel/specs.rst
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/lowlevel/stringops.rst
--rw-r--r--   0        0        0   272664 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/tutorials/tutorial_assign_motifs_to_peaks.ipynb
--rw-r--r--   0        0        0    72730 2020-02-02 00:00:00.000000 bioframe-0.6.4/docs/tutorials/tutorial_assign_peaks_to_genes.ipynb
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 bioframe-0.6.4/tests/test_assembly_info.py
--rw-r--r--   0        0        0    14096 2020-02-02 00:00:00.000000 bioframe-0.6.4/tests/test_core_checks.py
--rw-r--r--   0        0        0     7474 2020-02-02 00:00:00.000000 bioframe-0.6.4/tests/test_core_construction.py
--rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 bioframe-0.6.4/tests/test_core_specs.py
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 bioframe-0.6.4/tests/test_core_stringops.py
--rw-r--r--   0        0        0     8990 2020-02-02 00:00:00.000000 bioframe-0.6.4/tests/test_extras.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 bioframe-0.6.4/tests/test_fileops.py
--rw-r--r--   0        0        0    69553 2020-02-02 00:00:00.000000 bioframe-0.6.4/tests/test_ops.py
--rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 bioframe-0.6.4/tests/test_ops_select.py
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 bioframe-0.6.4/tests/test_resources.py
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 bioframe-0.6.4/tests/test_vis.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 bioframe-0.6.4/tests/test_data/test.chrom.sizes
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 bioframe-0.6.4/tests/test_data/test.fa
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 bioframe-0.6.4/tests/test_data/test.fa.fai
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 bioframe-0.6.4/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 bioframe-0.6.4/LICENSE
--rw-r--r--   0        0        0     5217 2020-02-02 00:00:00.000000 bioframe-0.6.4/README.md
--rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 bioframe-0.6.4/pyproject.toml
--rw-r--r--   0        0        0     7190 2020-02-02 00:00:00.000000 bioframe-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 bioframe-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 bioframe-0.7.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     9513 2020-02-02 00:00:00.000000 bioframe-0.7.0/CHANGES.md
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 bioframe-0.7.0/CITATION.cff
+-rw-r--r--   0        0        0     5517 2020-02-02 00:00:00.000000 bioframe-0.7.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 bioframe-0.7.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 bioframe-0.7.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 bioframe-0.7.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 bioframe-0.7.0/bioframe/__init__.py
+-rw-r--r--   0        0        0    16589 2020-02-02 00:00:00.000000 bioframe-0.7.0/bioframe/extras.py
+-rw-r--r--   0        0        0    64681 2020-02-02 00:00:00.000000 bioframe-0.7.0/bioframe/ops.py
+-rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 bioframe-0.7.0/bioframe/vis.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 bioframe-0.7.0/bioframe/core/__init__.py
+-rw-r--r--   0        0        0    25606 2020-02-02 00:00:00.000000 bioframe-0.7.0/bioframe/core/arrops.py
+-rw-r--r--   0        0        0    15075 2020-02-02 00:00:00.000000 bioframe-0.7.0/bioframe/core/checks.py
+-rw-r--r--   0        0        0    11535 2020-02-02 00:00:00.000000 bioframe-0.7.0/bioframe/core/construction.py
+-rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 bioframe-0.7.0/bioframe/core/specs.py
+-rw-r--r--   0        0        0     6906 2020-02-02 00:00:00.000000 bioframe-0.7.0/bioframe/core/stringops.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 bioframe-0.7.0/bioframe/io/__init__.py
+-rw-r--r--   0        0        0     5667 2020-02-02 00:00:00.000000 bioframe-0.7.0/bioframe/io/assembly.py
+-rw-r--r--   0        0        0    23399 2020-02-02 00:00:00.000000 bioframe-0.7.0/bioframe/io/bed.py
+-rw-r--r--   0        0        0    19327 2020-02-02 00:00:00.000000 bioframe-0.7.0/bioframe/io/fileops.py
+-rw-r--r--   0        0        0     8630 2020-02-02 00:00:00.000000 bioframe-0.7.0/bioframe/io/resources.py
+-rw-r--r--   0        0        0     5232 2020-02-02 00:00:00.000000 bioframe-0.7.0/bioframe/io/schemas.py
+-rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 bioframe-0.7.0/bioframe/io/data/_assemblies.yml
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 bioframe-0.7.0/bioframe/io/data/ce10.seqinfo.tsv
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 bioframe-0.7.0/bioframe/io/data/ce11.seqinfo.tsv
+-rw-r--r--   0        0        0    70878 2020-02-02 00:00:00.000000 bioframe-0.7.0/bioframe/io/data/danRer10.seqinfo.tsv
+-rw-r--r--   0        0        0    66339 2020-02-02 00:00:00.000000 bioframe-0.7.0/bioframe/io/data/danRer11.seqinfo.tsv
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 bioframe-0.7.0/bioframe/io/data/dm3.seqinfo.tsv
+-rw-r--r--   0        0        0   161973 2020-02-02 00:00:00.000000 bioframe-0.7.0/bioframe/io/data/dm6.seqinfo.tsv
+-rw-r--r--   0        0        0    30781 2020-02-02 00:00:00.000000 bioframe-0.7.0/bioframe/io/data/hg19.cytoband.tsv
+-rw-r--r--   0        0        0     6881 2020-02-02 00:00:00.000000 bioframe-0.7.0/bioframe/io/data/hg19.seqinfo.tsv
+-rw-r--r--   0        0        0    30775 2020-02-02 00:00:00.000000 bioframe-0.7.0/bioframe/io/data/hg38.cytoband.tsv
+-rw-r--r--   0        0        0    16501 2020-02-02 00:00:00.000000 bioframe-0.7.0/bioframe/io/data/hg38.seqinfo.tsv
+-rw-r--r--   0        0        0    30780 2020-02-02 00:00:00.000000 bioframe-0.7.0/bioframe/io/data/hs1.cytoband.tsv
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 bioframe-0.7.0/bioframe/io/data/hs1.seqinfo.tsv
+-rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 bioframe-0.7.0/bioframe/io/data/mm10.seqinfo.tsv
+-rw-r--r--   0        0        0     4801 2020-02-02 00:00:00.000000 bioframe-0.7.0/bioframe/io/data/mm39.seqinfo.tsv
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 bioframe-0.7.0/bioframe/io/data/mm9.seqinfo.tsv
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 bioframe-0.7.0/bioframe/io/data/sacCer3.seqinfo.tsv
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 bioframe-0.7.0/bioframe/io/data/wuhCor1.seqinfo.tsv
+-rw-r--r--   0        0        0     5774 2020-02-02 00:00:00.000000 bioframe-0.7.0/bioframe/sandbox/clients.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 bioframe-0.7.0/bioframe/sandbox/gtf_io.py
+-rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 bioframe-0.7.0/bioframe/sandbox/parquet_io.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 bioframe-0.7.0/docs/Makefile
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 bioframe-0.7.0/docs/api-construction.rst
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 bioframe-0.7.0/docs/api-extras.rst
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 bioframe-0.7.0/docs/api-fileops.rst
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 bioframe-0.7.0/docs/api-intervalops.rst
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 bioframe-0.7.0/docs/api-lowlevel.md
+-rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 bioframe-0.7.0/docs/api-resources.rst
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 bioframe-0.7.0/docs/api-validation.rst
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 bioframe-0.7.0/docs/api-vis.rst
+-rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 bioframe-0.7.0/docs/conf.py
+-rw-r--r--   0        0        0     5211 2020-02-02 00:00:00.000000 bioframe-0.7.0/docs/guide-bedtools.md
+-rw-r--r--   0        0        0     4804 2020-02-02 00:00:00.000000 bioframe-0.7.0/docs/guide-definitions.rst
+-rw-r--r--   0        0        0    16197 2020-02-02 00:00:00.000000 bioframe-0.7.0/docs/guide-intervalops.md
+-rw-r--r--   0        0        0    13720 2020-02-02 00:00:00.000000 bioframe-0.7.0/docs/guide-io.ipynb
+-rw-r--r--   0        0        0   374211 2020-02-02 00:00:00.000000 bioframe-0.7.0/docs/guide-performance.ipynb
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 bioframe-0.7.0/docs/guide-quickstart.rst
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 bioframe-0.7.0/docs/guide-recipes.md
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 bioframe-0.7.0/docs/guide-specifications.rst
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 bioframe-0.7.0/docs/index.rst
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 bioframe-0.7.0/docs/make.bat
+-rw-r--r--   0        0        0    38715 2020-02-02 00:00:00.000000 bioframe-0.7.0/docs/times100.bw
+-rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 bioframe-0.7.0/docs/figs/._bioframe-logo.png
+-rw-r--r--   0        0        0    68759 2020-02-02 00:00:00.000000 bioframe-0.7.0/docs/figs/bioframe-logo.png
+-rw-r--r--   0        0        0    65297 2020-02-02 00:00:00.000000 bioframe-0.7.0/docs/figs/bioframe_closest.pdf
+-rw-r--r--   0        0        0    21587 2020-02-02 00:00:00.000000 bioframe-0.7.0/docs/figs/closest0.png
+-rw-r--r--   0        0        0    56069 2020-02-02 00:00:00.000000 bioframe-0.7.0/docs/figs/closest1.png
+-rw-r--r--   0        0        0    50871 2020-02-02 00:00:00.000000 bioframe-0.7.0/docs/figs/closest2.png
+-rw-r--r--   0        0        0    44726 2020-02-02 00:00:00.000000 bioframe-0.7.0/docs/figs/closest3.png
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 bioframe-0.7.0/docs/figs/df1.png
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 bioframe-0.7.0/docs/figs/df2.png
+-rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 bioframe-0.7.0/docs/figs/df@.png
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 bioframe-0.7.0/docs/figs/merge_df1.png
+-rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 bioframe-0.7.0/docs/figs/overlap_inner_0.png
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 bioframe-0.7.0/docs/figs/overlap_inner_1.png
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 bioframe-0.7.0/docs/lowlevel/arrops.rst
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 bioframe-0.7.0/docs/lowlevel/specs.rst
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 bioframe-0.7.0/docs/lowlevel/stringops.rst
+-rw-r--r--   0        0        0   273298 2020-02-02 00:00:00.000000 bioframe-0.7.0/docs/tutorials/tutorial_assign_motifs_to_peaks.ipynb
+-rw-r--r--   0        0        0    73212 2020-02-02 00:00:00.000000 bioframe-0.7.0/docs/tutorials/tutorial_assign_peaks_to_genes.ipynb
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 bioframe-0.7.0/tests/test_assembly_info.py
+-rw-r--r--   0        0        0     7027 2020-02-02 00:00:00.000000 bioframe-0.7.0/tests/test_bed.py
+-rw-r--r--   0        0        0    14094 2020-02-02 00:00:00.000000 bioframe-0.7.0/tests/test_core_checks.py
+-rw-r--r--   0        0        0     7472 2020-02-02 00:00:00.000000 bioframe-0.7.0/tests/test_core_construction.py
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 bioframe-0.7.0/tests/test_core_specs.py
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 bioframe-0.7.0/tests/test_core_stringops.py
+-rw-r--r--   0        0        0     8988 2020-02-02 00:00:00.000000 bioframe-0.7.0/tests/test_extras.py
+-rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 bioframe-0.7.0/tests/test_fileops.py
+-rw-r--r--   0        0        0    69539 2020-02-02 00:00:00.000000 bioframe-0.7.0/tests/test_ops.py
+-rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 bioframe-0.7.0/tests/test_ops_select.py
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 bioframe-0.7.0/tests/test_resources.py
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 bioframe-0.7.0/tests/test_vis.py
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 bioframe-0.7.0/tests/test_data/bed12.bed
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 bioframe-0.7.0/tests/test_data/bed9.bed
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 bioframe-0.7.0/tests/test_data/jaspar.bed
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 bioframe-0.7.0/tests/test_data/narrowPeak.bed
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 bioframe-0.7.0/tests/test_data/test.chrom.sizes
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 bioframe-0.7.0/tests/test_data/test.fa
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 bioframe-0.7.0/tests/test_data/test.fa.fai
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 bioframe-0.7.0/tests/test_data/toy.bam
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 bioframe-0.7.0/tests/test_data/toy.bam.bai
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 bioframe-0.7.0/tests/test_data/toy.sam
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 bioframe-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 bioframe-0.7.0/LICENSE
+-rw-r--r--   0        0        0     5364 2020-02-02 00:00:00.000000 bioframe-0.7.0/README.md
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 bioframe-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     7300 2020-02-02 00:00:00.000000 bioframe-0.7.0/PKG-INFO
```

### Comparing `bioframe-0.6.4/.readthedocs.yaml` & `bioframe-0.7.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.4/CHANGES.md` & `bioframe-0.7.0/CHANGES.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,28 @@
 # Release notes
 
-## [Upcoming release](https://github.com/open2c/bioframe/compare/v0.6.4...HEAD)
+## [Upcoming release](https://github.com/open2c/bioframe/compare/v0.7.0...HEAD)
+
+## [v0.6.4](https://github.com/open2c/bioframe/compare/v0.6.4...v0.7.0)
+Date 2024-05-20
+
+API changes:
+* Add `to_bed` function to validate and write standard BED files @gamazeps in https://github.com/open2c/bioframe/pull/203
+* `read_bam` deprecated in favor of `read_alignments` @gamazeps in https://github.com/open2c/bioframe/pull/206
+
+Documentation:
+* Add "bioframe for bedtools users" guide to docs by @gamazeps in https://github.com/open2c/bioframe/pull/198
+
+Bug fixes:
+* Fix contig name and JSON isses in read_bam implementation by @gamazeps in https://github.com/open2c/bioframe/pull/206
+
+New Contributors:
+* @gamazeps made their first contribution in https://github.com/open2c/bioframe/pull/203
+
+**Full Changelog**: https://github.com/open2c/bioframe/compare/v0.6.4...v0.7.0
 
 ## [v0.6.4](https://github.com/open2c/bioframe/compare/v0.6.3...v0.6.4)
 Date 2024-04-06
 
 Maintenance:
 * Migrate from setuptools `pkg_resources` to `importlib.resources` by @nvictus in https://github.com/open2c/bioframe/pull/194
 * Use `importlib.metadata` for versioning by @nvictus in https://github.com/open2c/bioframe/pull/195
@@ -37,18 +55,18 @@
 * Update to new UCSC hgdownload url by @golobor and @nvictus in https://github.com/open2c/bioframe/pull/187
 
 ## [v0.6.1](https://github.com/open2c/bioframe/compare/v0.6.0...v0.6.1)
 Date 2024-01-08
 
 API changes:
 
-Default behavior of `ensure_nullable` option in `overlap` was modified to minimize the possibility of regressions in libraries that depend on legacy behavior. 
+Default behavior of `ensure_nullable` option in `overlap` was modified to minimize the possibility of regressions in libraries that depend on legacy behavior.
 
-* The new option was renamed `ensure_int` and is `True` by default. It ensures that output coordinate columns are always returned with an integer dtype, as was the case in prior versions. This is achieved by converting columns having non-nullable NumPy dtypes to Pandas nullable ones in the specific case where the result of an **outer join** generates missing values; otherwise, column dtypes are preserved unchanged in the output. 
-* Unlike previous minor versions of bioframe, the nullable dtype chosen will have the **same underlying type** as the corresponding column from the input (i.e, an input dataframe using `np.uint32` start coordinates may yield a `pd.UInt32` start column in the output). 
+* The new option was renamed `ensure_int` and is `True` by default. It ensures that output coordinate columns are always returned with an integer dtype, as was the case in prior versions. This is achieved by converting columns having non-nullable NumPy dtypes to Pandas nullable ones in the specific case where the result of an **outer join** generates missing values; otherwise, column dtypes are preserved unchanged in the output.
+* Unlike previous minor versions of bioframe, the nullable dtype chosen will have the **same underlying type** as the corresponding column from the input (i.e, an input dataframe using `np.uint32` start coordinates may yield a `pd.UInt32` start column in the output).
 * This behavior can be turned off by setting `ensure_int` to `False`, in which case outer joins on dataframes using NumPy dtypes may produce floating point output columns when missing values are introduced (stored as `NaN`), following the native casting behavior of such columns.
 
 ## [v0.6.0](https://github.com/open2c/bioframe/compare/v0.5.1...v0.6.0)
 Date 2024-01-04
 
 API changes:
 * `overlap`: In previous versions, output coordinate columns were always converted to Pandas "nullable" `Int64` dtype before returning outer join results. In the interest of flexibility, memory efficiency, and least surprise, the coordinate columns returned in the output dataframe now preserve dtype from the input dataframes, following native type casting rules if missing data are introduced. We introduce the `ensure_nullable` argument to force Pandas nullable dtypes in the output coordinates. See the [docs](https://bioframe.readthedocs.io/en/latest/api-intervalops.html#bioframe.ops.overlap) for more details. (#178)
@@ -137,35 +155,35 @@
 * `bioframe.sort_bedframe` does not append columns or modify their dtypes.
 
 ## [v0.3.0](https://github.com/open2c/bioframe/compare/v0.2.0...v0.3.0)
 
 Date : 2021-08-31
 
 Conceptual changes:
-* we formulated strict definitions for genomic intervals, dataframes, and 
+* we formulated strict definitions for genomic intervals, dataframes, and
     their various properties. All bioframe functions are expected to follow
-    to these definitions tightly.  
+    to these definitions tightly.
 
 API changes:
-* reorganize modules: 
-    * ops - operations on genomic interval dataframes 
+* reorganize modules:
+    * ops - operations on genomic interval dataframes
     * extras - miscellaneous operations, most involving
         genomic sequences and gene annotations
     * vis - visualizations of genomic interval dataframes
     * core.arrops - operations on genomic interval arrays
     * core.checks - tests for definitions of genomic interval dataframes
     * core.construction - construction and sanitation of genomic interval dataframes
-    * core.specs - specifications for the implementation of genomic intervals in pandas.dataframes 
+    * core.specs - specifications for the implementation of genomic intervals in pandas.dataframes
         (i.e. column names, datatypes, etc)
     * core.stringops - operations on genomic interval strings
     * io.fileops - I/O on common file formats for genomic data
     * io.schemas - schemas for standard tabular formats for genomic data storage
-    * io.resources - interfaces to popular online genomic data resources 
+    * io.resources - interfaces to popular online genomic data resources
 
-* new functions: extras.pair_by_distance, ops.sort_bedframe, ops.assign_view, 
+* new functions: extras.pair_by_distance, ops.sort_bedframe, ops.assign_view,
     dataframe constructors
 
 * existing functions:
     * expand: take negative values and fractional values
     * overlap: change default suffixes, keep_order=True
     * subtract: add return_index and keep_order
```

### Comparing `bioframe-0.6.4/CITATION.cff` & `bioframe-0.7.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.4/CONTRIBUTING.md` & `bioframe-0.7.0/CONTRIBUTING.md`

 * *Files 11% similar despite different names*

```diff
@@ -22,69 +22,86 @@
 
 This project uses the [hatch](https://hatch.pypa.io/latest/) project manager and build system. We recommend you install `hatch` as a global isolated application using [pipx](https://pipx.pypa.io/stable/). See other installation options [here](https://hatch.pypa.io/latest/install/).
 
 ```sh
 pipx install hatch
 ```
 
-> [!TIP]  
-> If you prefer to store your virtual environments in your working directory (like classic virtualenvs) rather than in a centralized location (similar to conda), configure hatch as follows:
-> 
-> ```sh
-> hatch config set dirs.env.virtual .venv
-> ```
->
-> This will make hatch set up its environments within the current working directory under `.venv`.
+> [!NOTE]
+> Many custom command shortcuts are accessible through hatch (and shown below). See `tool.hatch.envs.default.scripts` in our project's `pyproject.toml` configuration file.
 
 After forking and cloning the repository, you can create an isolated Python development environment and install the package in "editable" (i.e. development) mode as follows:
 
 ```sh
 git clone https://github.com/open2c/bioframe.git
+cd bioframe
 hatch shell
 ```
 
-The first time you run `hatch shell` the environment will be created and activated, and the package will be installed. In future sessions, running `hatch shell` will reactivate your development environment. If you prefer to manage your virtual environments differently, you can install the package for development using:
+The first time you run `hatch shell` the environment will be created and activated, and the package will be installed. In future sessions, running `hatch shell` will reactivate your development environment.
+
+> [!TIP]
+> If you prefer to store your virtual environments in your working directory (like classic virtualenvs) rather than in a centralized location (similar to conda), configure hatch as follows:
+>
+> ```sh
+> hatch config set dirs.env.virtual .venv
+> ```
+>
+> This will make hatch set up its environments within the current working directory under `.venv`.
+
+Alternatively, if you prefer to manage your virtual environments yourself, you can install the package for development using, for example:
 
 ```sh
+python -m venv .venv
+source .venv/bin/activate
 pip install -e '.[dev,test,docs]'
 ```
 
 For all pull requests, linting and unit tests are automatically run using the [GitHub Actions](https://docs.github.com/en/actions) Continuous Integration service. However, you are still encouraged to run these checks locally before pushing code to a PR.
 
-> [!NOTE]
-> Many custom command shortcuts are accessible through hatch (and shown below). See `tool.hatch.envs.default.scripts` in our project's `pyproject.toml` configuration file.
-
-## Linting
+## Linting and Formatting
 
-We use [ruff](https://docs.astral.sh/ruff/) for style checking. Run `ruff .` or:
+We use [ruff](https://docs.astral.sh/ruff/) for style checking. Run `ruff check .` or:
 
 ```sh
 hatch run lint
 ```
 
-Ruff can fix a lot of errors itself. Run `ruff --fix .` or:
+Ruff can fix a lot of errors itself. Run `ruff check --fix .` or:
 
 ```sh
 hatch run fix
 ```
 
-You can also use tools like [black](https://black.readthedocs.io/en/stable/) to reformat your code.
+Ruff includes a formatter that mimics [black](https://black.readthedocs.io/en/stable/). To automatically reformat your code, you can use `ruff format {source_file}`.
+
+We use [pre-commit](https://github.com/pre-commit/pre-commit) to make sure the coding style is enforced. You first need to install pre-commit and the corresponding git commit hooks:
 
+```sh
+pip install pre-commit
+pre-commit install
+```
+
+The last command installs the hooks listed in `.pre-commit-config.yaml` locally into your git repo. If you do this, the checks will run automatically before every commit. You can also manually make sure your code satisfies the coding style:
+
+```sh
+pre-commit run --all-files
+```
 
-## Running/Adding Unit Tests
+## Testing
 
 It is best if all new functionality and/or bug fixes have unit tests added with each use-case.
 
 We use [pytest](https://docs.pytest.org/en/latest) as our unit testing framework. Once you've configured your environment, you can just `cd` to the root of your repository and run `pytest` or:
 
 ```sh
 hatch run test
 ```
 
-## Adding/Building the Documentation
+## Documentation
 
 If a feature is stable and relatively finalized, it is time to add it to the documentation. If you are adding any private/public functions, it is best to add docstrings, to aid in reviewing code and also for the API reference.
 
 We use [Numpy style docstrings](https://numpydoc.readthedocs.io/en/latest/format.html>) and [Sphinx](http://www.sphinx-doc.org/en/stable) to document this library. Sphinx, in turn, uses [reStructuredText](http://www.sphinx-doc.org/en/stable/rest.html) as its markup language for adding code.
 
 We use the [Sphinx Autosummary extension](http://www.sphinx-doc.org/en/stable/ext/autosummary.html) to generate API references. You may want to look at `docs/api-*.rst` files to see how they look and where to add new functions, classes or modules. We also use the [myst_nb extension](https://myst-nb.readthedocs.io/en/latest/) to render Jupyter notebooks in the documentation.
```

### Comparing `bioframe-0.6.4/.github/workflows/ci.yml` & `bioframe-0.7.0/.github/workflows/ci.yml`

 * *Files 15% similar despite different names*

```diff
@@ -9,33 +9,33 @@
 
 
 jobs:
 
   Lint:
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: "3.x"
     - run: |
         python -m pip install --upgrade pip hatch
         pip install -e .[dev]
         hatch run lint
 
   Test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: [ "3.8", "3.9", "3.10", "3.11" ]
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
       - run: |
           python -m pip install --upgrade pip hatch
           pip install -e .[dev]
           # Stop the build if there are Python syntax errors or undefined names
           ruff . --select=E9,F63,F7,F82 --show-source
```

### Comparing `bioframe-0.6.4/.github/workflows/publish.yml` & `bioframe-0.7.0/.github/workflows/publish.yml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       id-token: write
 
     steps:
       - name: Checkout
         uses: actions/checkout@v4
 
       - name: Setup Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.x"
 
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install build
```

### Comparing `bioframe-0.6.4/bioframe/__init__.py` & `bioframe-0.7.0/bioframe/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,21 +41,23 @@
     "SCHEMAS",
     "UCSCClient",
     "assemblies_available",
     "assembly_info",
     "fetch_centromeres",
     "fetch_chromsizes",
     "load_fasta",
+    "read_alignment",
     "read_bam",
     "read_bigbed",
     "read_bigwig",
     "read_chromsizes",
     "read_pairix",
     "read_tabix",
     "read_table",
+    "to_bed",
     "to_bigbed",
     "to_bigwig",
     "assign_view",
     "closest",
     "cluster",
     "complement",
     "count_overlaps",
@@ -112,21 +114,23 @@
     SCHEMAS,
     UCSCClient,
     assemblies_available,
     assembly_info,
     fetch_centromeres,
     fetch_chromsizes,
     load_fasta,
+    read_alignment,
     read_bam,
     read_bigbed,
     read_bigwig,
     read_chromsizes,
     read_pairix,
     read_tabix,
     read_table,
+    to_bed,
     to_bigbed,
     to_bigwig,
 )
 from .ops import (
     assign_view,
     closest,
     cluster,
```

### Comparing `bioframe-0.6.4/bioframe/extras.py` & `bioframe-0.7.0/bioframe/extras.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,19 +57,19 @@
     if len(cols_chroms) == 2:
         ck1, sk1 = cols_chroms
     elif len(cols_chroms) == 3:
         ck1, sk1, ek1 = cols_chroms
 
     if isinstance(chromsizes, (pd.Series, dict)):
         chromsizes = dict(chromsizes)
-        df_chroms = (
-            pd.DataFrame({
+        df_chroms = pd.DataFrame(
+            {
                 ck1: list(chromsizes.keys()),
                 "length": list(chromsizes.values()),
-            })
+            }
         )
     elif isinstance(chromsizes, pd.DataFrame):
         df_chroms = chromsizes.copy()
     else:
         raise ValueError("unknown input type for chromsizes")
 
     if len(cols_chroms) == 2:
@@ -508,16 +508,17 @@
 
     # Select only the pairs that are separated by
     # at least min_intervening intervals and no more than max_intervening intervals
     idxs["intervening"] = (
         np.abs(idxs[f"index{suffixes[0]}"] - idxs[f"index{suffixes[1]}"]) - 1
     )
     idxs = idxs[
-        (idxs['intervening']<=max_intervening) & (idxs['intervening']>=min_intervening)
-        ]
+        (idxs["intervening"] <= max_intervening)
+        & (idxs["intervening"] >= min_intervening)
+    ]
 
     left_ivals = (
         df.iloc[idxs[f"index{suffixes[0]}"].values]
         .rename(columns=lambda x: x + suffixes[0])
         .reset_index(drop=True)
     )
     right_ivals = (
```

### Comparing `bioframe-0.6.4/bioframe/ops.py` & `bioframe-0.7.0/bioframe/ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -819,15 +819,15 @@
         (
             cluster_ids_group,
             cluster_starts_group,
             cluster_ends_group,
         ) = arrops.merge_intervals(
             df_group[sk].values.astype(np.int64),
             df_group[ek].values.astype(np.int64),
-            min_dist=min_dist
+            min_dist=min_dist,
             # df_group[sk].values, df_group[ek].values, min_dist=min_dist
         )
         interval_counts = np.bincount(cluster_ids_group)
         n_clusters = cluster_starts_group.shape[0]
 
         ## Storing chromosome names causes a 2x slowdown. :(
         if isinstance(group_keys, str):
```

### Comparing `bioframe-0.6.4/bioframe/vis.py` & `bioframe-0.7.0/bioframe/vis.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     chr1   10     20   blue   0,0,255
     chr2   0      10   green  0,128,0
     chr2   10     20   None   0
     """
     if pd.isnull(color):
         return "0"
     else:
-        return ",".join(str(int(x*255)) for x in to_rgb(color))
+        return ",".join(str(int(x * 255)) for x in to_rgb(color))
 
 
 def _plot_interval(
     start, end, level, facecolor=None, edgecolor=None, height=0.6, ax=None
 ):
     facecolor = DEFAULT_FACECOLOR if facecolor is None else facecolor
     edgecolor = DEFAULT_EDGECOLOR if edgecolor is None else edgecolor
@@ -135,15 +135,14 @@
         labels = itertools.cycle([labels])
     else:
         labels = itertools.cycle(labels)
 
     for i, (start, end, level, color, label) in enumerate(
         zip(starts, ends, levels, colors, labels)
     ):
-
         _plot_interval(start, end, level, facecolor=color)
         if label is not None:
             plt.text(
                 (start + end) / 2,
                 level,
                 label,
                 horizontalalignment="center",
```

### Comparing `bioframe-0.6.4/bioframe/core/__init__.py` & `bioframe-0.7.0/bioframe/core/__init__.py`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.4/bioframe/core/arrops.py` & `bioframe-0.7.0/bioframe/core/arrops.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,14 +260,15 @@
 
     # Sort overlaps according to the 1st
     if sort:
         overlap_ids = overlap_ids[np.lexsort([overlap_ids[:, 1], overlap_ids[:, 0]])]
 
     return overlap_ids
 
+
 def _convert_points_to_len1_segments(starts, ends):
     """
     Convert points to len1 segments for internal use in overlap().
     This enables desired overlap behavior for points and preserves
     behavior for semi-open intervals of len>=1.
     Parameters
     ----------
@@ -278,14 +279,15 @@
     pseudo_ends : numpy.ndarray
     An array of pseudo-ends for overlapping intervals.
     """
     pseudo_ends = ends.copy()
     pseudo_ends[ends == starts] += 1
     return [starts, pseudo_ends]
 
+
 def overlap_intervals(starts1, ends1, starts2, ends2, closed=False, sort=False):
     """
     Take two sets of intervals and return the indices of pairs of overlapping intervals.
 
     Parameters
     ----------
     starts1, ends1, starts2, ends2 : numpy.ndarray
@@ -725,16 +727,16 @@
     right_dists = starts2[right_ids[:, 1]] - ends1[right_ids[:, 0]] + 1
 
     closest_ids = np.vstack([left_ids, right_ids, overlap_ids])
     closest_dists = np.concatenate(
         [left_dists, right_dists, np.zeros(overlap_ids.shape[0])]
     )
 
-    if len(closest_ids)==0:
-        return np.empty((0,2), dtype=int)
+    if len(closest_ids) == 0:
+        return np.empty((0, 2), dtype=int)
 
     # Sort by distance to set 1 intervals and, if present, by the tie-breaking
     # data array.
     if tie_arr is None:
         order = np.lexsort([closest_ids[:, 1], closest_dists, closest_ids[:, 0]])
     else:
         order = np.lexsort(
```

### Comparing `bioframe-0.6.4/bioframe/core/checks.py` & `bioframe-0.7.0/bioframe/core/checks.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,16 +58,15 @@
     ck1, sk1, ek1 = _get_default_colnames() if cols is None else cols
 
     if not _verify_columns(df, [ck1, sk1, ek1], return_as_bool=True):
         if raise_errors:
             raise TypeError("Invalid bedFrame: Invalid column names")
         return False
 
-    if not _verify_column_dtypes(df, cols=[ck1, sk1, ek1],
-                                 return_as_bool=True):
+    if not _verify_column_dtypes(df, cols=[ck1, sk1, ek1], return_as_bool=True):
         if raise_errors:
             raise TypeError("Invalid bedFrame: Invalid column dtypes")
         return False
 
     nan_intervals = pd.isnull(df[[ck1, sk1, ek1]])
     if (~(~nan_intervals.any(axis=1) | nan_intervals.all(axis=1))).any():
         if raise_errors:
@@ -75,26 +74,26 @@
                 "Invalid bedFrame: Invalid null values "
                 "(if any of chrom, start, end are null, then all must be null)"
             )
         return False
 
     if ((df[ek1] - df[sk1]) < 0).any():
         if raise_errors:
-            raise ValueError(f"Invalid bedframe: starts exceed ends for "
-                             f"{sum((df[ek1] - df[sk1]) < 0)} intervals")
+            raise ValueError(
+                f"Invalid bedframe: starts exceed ends for "
+                f"{sum((df[ek1] - df[sk1]) < 0)} intervals"
+            )
         return False
 
     return True
 
 
-def is_cataloged(df,
-                 view_df,
-                 raise_errors=False,
-                 df_view_col="view_region",
-                 view_name_col="name"):
+def is_cataloged(
+    df, view_df, raise_errors=False, df_view_col="view_region", view_name_col="name"
+):
     """
     Tests if all region names in `df[df_view_col]` are present in
     `view_df[view_name_col]`.
 
     Parameters
     ----------
     df : pandas.DataFrame
@@ -129,21 +128,24 @@
         if raise_errors:
             raise ValueError(f"Could not find \
                 `{view_name_col}` \
                 column in view_df")
         return False
 
     if not set(df[df_view_col].copy().dropna().values).issubset(
-            set(view_df[view_name_col].values)):
+        set(view_df[view_name_col].values)
+    ):
         if raise_errors:
             missing_regions = set(df[df_view_col].values).difference(
-                set(view_df[view_name_col].values))
+                set(view_df[view_name_col].values)
+            )
             raise ValueError(
                 f"The following regions in df[df_view_col] not in "
-                f"view_df[view_name_col]: \n{missing_regions}")
+                f"view_df[view_name_col]: \n{missing_regions}"
+            )
         return False
 
     return True
 
 
 def is_overlapping(df, cols=None):
     """
@@ -168,27 +170,23 @@
     from ..ops import merge
 
     ck1, sk1, ek1 = _get_default_colnames() if cols is None else cols
 
     df_merged = merge(df, cols=cols)
 
     total_interval_len = np.sum((df[ek1] - df[sk1]).values)
-    total_interval_len_merged = np.sum(
-        (df_merged[ek1] - df_merged[sk1]).values)
+    total_interval_len_merged = np.sum((df_merged[ek1] - df_merged[sk1]).values)
 
     if total_interval_len > total_interval_len_merged:
         return True
     else:
         return False
 
 
-def is_viewframe(region_df,
-                 raise_errors=False,
-                 view_name_col="name",
-                 cols=None):
+def is_viewframe(region_df, raise_errors=False, view_name_col="name", cols=None):
     """
     Checks that `region_df` is a valid viewFrame.
 
     This includes:
 
     - it satisfies requirements for a bedframe, including columns for
       ('chrom', 'start', 'end')
@@ -219,35 +217,37 @@
     -------
     is_viewframe:bool
 
     """
 
     ck1, sk1, ek1 = _get_default_colnames() if cols is None else cols
 
-    if not _verify_columns(region_df, [ck1, sk1, ek1, view_name_col],
-                           return_as_bool=True):
+    if not _verify_columns(
+        region_df, [ck1, sk1, ek1, view_name_col], return_as_bool=True
+    ):
         if raise_errors:
             raise TypeError("Invalid view: invalid column names")
         return False
 
     if not is_bedframe(region_df, cols=cols):
         if raise_errors:
             raise ValueError("Invalid view: not a bedframe")
         return False
 
     if pd.isna(region_df).values.any():
         if raise_errors:
             raise ValueError("Invalid view: cannot contain NAs")
         return False
 
-    if len(set(region_df[view_name_col])) < \
-       len(region_df[view_name_col].values):
+    if len(set(region_df[view_name_col])) < len(region_df[view_name_col].values):
         if raise_errors:
-            raise ValueError("Invalid view: entries in \
-                region_df[view_name_col] must be unique")
+            raise ValueError(
+                "Invalid view: entries in \
+                region_df[view_name_col] must be unique"
+            )
         return False
 
     if is_overlapping(region_df, cols=cols):
         if raise_errors:
             raise ValueError("Invalid view: entries must be non-overlapping")
         return False
 
@@ -292,22 +292,20 @@
 
     Returns
     -------
     is_contained:bool
 
     """
     from ..ops import trim
+
     ck1, sk1, ek1 = _get_default_colnames() if cols is None else cols
     ck2, sk2, ek2 = _get_default_colnames() if cols_view is None else cols_view
     if df_view_col is None:
         try:
-            df_view_assigned = ops.overlap(df,
-                                           view_df,
-                                           cols1=cols,
-                                           cols2=cols_view)
+            df_view_assigned = ops.overlap(df, view_df, cols1=cols, cols2=cols_view)
             # ek2 = end_ is the default value
             assert (df_view_assigned[ek2 + "_"].isna()).sum() == 0
             # sk2 = start_ is the default value
             assert (df_view_assigned[sk2 + "_"].isna()).sum() == 0
             assert (df_view_assigned[ek1] <= df_view_assigned[ek2 + "_"]).all()
             # ek1 = end is the default value
             # sk1 = start is the default value
@@ -316,25 +314,28 @@
             if raise_errors:
                 raise AssertionError("df not contained in view_df")
             else:
                 return False
         return True
 
     if not is_cataloged(
-            df, view_df, df_view_col=df_view_col, view_name_col=view_name_col):
+        df, view_df, df_view_col=df_view_col, view_name_col=view_name_col
+    ):
         if raise_errors:
             raise ValueError("df not cataloged in view_df")
         return False
 
-    df_trim = trim(df,
-                   view_df=view_df,
-                   df_view_col=df_view_col,
-                   view_name_col=view_name_col,
-                   cols=cols,
-                   cols_view=cols_view)
+    df_trim = trim(
+        df,
+        view_df=view_df,
+        df_view_col=df_view_col,
+        view_name_col=view_name_col,
+        cols=cols,
+        cols_view=cols_view,
+    )
 
     is_start_trimmed = np.any(df[sk1].values != df_trim[sk1].values)
     is_end_trimmed = np.any(df[ek1].values != df_trim[ek1].values)
 
     if is_start_trimmed or is_end_trimmed:
         if raise_errors:
             raise ValueError("df not contained in view_df")
@@ -377,19 +378,19 @@
     -------
     is_covering:bool
 
     """
     from ..ops import complement
 
     if complement(
-            df,
-            view_df=view_df,
-            view_name_col=view_name_col,
-            cols=cols,
-            cols_view=cols_view,
+        df,
+        view_df=view_df,
+        view_name_col=view_name_col,
+        cols=cols,
+        cols_view=cols_view,
     ).empty:
         return True
     else:
         return False
 
 
 def is_tiling(
@@ -440,36 +441,36 @@
 
     Returns
     -------
     is_tiling:bool
 
     """
 
-    view_df = construction.make_viewframe(view_df,
-                                          view_name_col=view_name_col,
-                                          cols=cols_view)
+    view_df = construction.make_viewframe(
+        view_df, view_name_col=view_name_col, cols=cols_view
+    )
 
     if is_overlapping(df, cols=cols):
         if raise_errors:
             raise ValueError("overlaps")
         return False
-    if not is_covering(df,
-                       view_df,
-                       view_name_col=view_name_col,
-                       cols=cols,
-                       cols_view=cols_view):
+    if not is_covering(
+        df, view_df, view_name_col=view_name_col, cols=cols, cols_view=cols_view
+    ):
         if raise_errors:
             raise ValueError("not covered")
         return False
-    if not is_contained(df,
-                        view_df,
-                        df_view_col=df_view_col,
-                        view_name_col=view_name_col,
-                        cols=cols,
-                        cols_view=cols_view):
+    if not is_contained(
+        df,
+        view_df,
+        df_view_col=df_view_col,
+        view_name_col=view_name_col,
+        cols=cols,
+        cols_view=cols_view,
+    ):
         if raise_errors:
             raise ValueError("not contained")
         return False
     return True
 
 
 def is_sorted(
```

### Comparing `bioframe-0.6.4/bioframe/core/construction.py` & `bioframe-0.7.0/bioframe/core/construction.py`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.4/bioframe/core/specs.py` & `bioframe-0.7.0/bioframe/core/specs.py`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.4/bioframe/core/stringops.py` & `bioframe-0.7.0/bioframe/core/stringops.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,18 +15,16 @@
 RANGE_TOKEN_SPEC = [
     ("HYPHEN", r"-"),
     ("COORD", r"[0-9,]+(\.[0-9]*)?(?:[a-z]+)?"),
     ("OTHER", r".+"),
 ]
 
 RANGE_REGEX = re.compile(
-    r"\s*" + r"|\s*".join(
-        rf"(?P<{name}>{token})" for name, token in RANGE_TOKEN_SPEC
-    ),
-    re.IGNORECASE
+    r"\s*" + r"|\s*".join(rf"(?P<{name}>{token})" for name, token in RANGE_TOKEN_SPEC),
+    re.IGNORECASE,
 )
 
 
 def to_ucsc_string(grange: Tuple[str, int, int]) -> str:
     """
     Convert a grange to a UCSC string.
 
@@ -110,34 +108,28 @@
         for match in RANGE_REGEX.finditer(s):
             name = match.lastgroup
             yield name, match.group(name)
 
     def _parse_range(token_stream):
         name, token = next(token_stream, (None, None))
         if name != "COORD":
-            raise ValueError(
-                f"Expected COORD; got unexpected token: {name}: {token}"
-            )
+            raise ValueError(f"Expected COORD; got unexpected token: {name}: {token}")
         start = _parse_humanized_int(token)
 
         name, token = next(token_stream, (None, None))
         if name != "HYPHEN":
-            raise ValueError(
-                f"Expected HYPHEN; got unexpected token: {name}: {token}"
-            )
+            raise ValueError(f"Expected HYPHEN; got unexpected token: {name}: {token}")
 
         name, token = next(token_stream, (None, None))
         if name is None:  # No end coordinate
             end = None
         elif name == "COORD":
             end = _parse_humanized_int(token)
         else:
-            raise ValueError(
-                f"Expected COORD; got unexpected token: {name}: {token}"
-            )
+            raise ValueError(f"Expected COORD; got unexpected token: {name}: {token}")
 
         return start, end
 
     parts = s.split(":")
 
     chrom = parts[0].strip()
     if not len(chrom):
```

### Comparing `bioframe-0.6.4/bioframe/io/__init__.py` & `bioframe-0.7.0/bioframe/io/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from .assembly import assemblies_available, assembly_info
+from .bed import to_bed
 from .fileops import (
     load_fasta,
+    read_alignment,
     read_bam,
     read_bigbed,
     read_bigwig,
     read_chromsizes,
     read_pairix,
     read_tabix,
     read_table,
@@ -18,16 +20,18 @@
     "assemblies_available",
     "assembly_info",
     "read_table",
     "read_chromsizes",
     "read_tabix",
     "read_pairix",
     "read_bam",
+    "read_alignment",
     "load_fasta",
     "read_bigwig",
+    "to_bed",
     "to_bigwig",
     "read_bigbed",
     "to_bigbed",
     "UCSCClient",
     "fetch_centromeres",
     "fetch_chromsizes",
     "SCHEMAS",
```

### Comparing `bioframe-0.6.4/bioframe/io/assembly.py` & `bioframe-0.7.0/bioframe/io/assembly.py`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.4/bioframe/io/fileops.py` & `bioframe-0.7.0/bioframe/io/fileops.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import array
 import io
 import json
 import os
 import shutil
 import subprocess
 import tempfile
 from collections import OrderedDict
@@ -84,15 +85,15 @@
 
 def read_chromsizes(
     filepath_or,
     filter_chroms=True,
     chrom_patterns=(r"^chr[0-9]+$", r"^chr[XY]$", r"^chrM$"),
     natsort=True,
     as_bed=False,
-    **kwargs
+    **kwargs,
 ):
     """
     Read a ``<db>.chrom.sizes`` or ``<db>.chromInfo.txt`` file from the UCSC
     database, where ``db`` is a genome assembly name, as a `pandas.Series`.
 
     Parameters
     ----------
@@ -128,15 +129,15 @@
 
     chromtable = pd.read_csv(
         filepath_or,
         sep="\t",
         usecols=[0, 1],
         names=["name", "length"],
         dtype={"name": str},
-        **kwargs
+        **kwargs,
     )
 
     if filter_chroms:
         parts = []
         for pattern in chrom_patterns:
             if not len(pattern):
                 continue
@@ -180,15 +181,15 @@
     fp,
     region1,
     region2=None,
     chromsizes=None,
     columns=None,
     usecols=None,
     dtypes=None,
-    **kwargs
+    **kwargs,
 ):
     """
     Read a pairix-indexed file into DataFrame.
     """
     import cytoolz as toolz
     import pypairix
 
@@ -227,43 +228,63 @@
             if col in dtypes:
                 df[col] = df[col].astype(dtypes[col])
             else:
                 df[col] = pd.to_numeric(df[col], "ignore")
     return df
 
 
-def read_bam(fp, chrom=None, start=None, end=None):
+def read_alignment(fp, chrom=None, start=None, end=None):
     """
-    Read bam records into a DataFrame.
+    Read alignment records into a DataFrame.
     """
     import pysam
 
-    with closing(pysam.AlignmentFile(fp, "rb")) as f:
-        bam_iter = f.fetch(chrom, start, end)
-        records = [
-            (
-                s.qname,
-                s.flag,
-                s.rname,
-                s.pos,
-                s.mapq,
-                s.cigarstring if s.mapq != 0 else np.nan,
-                s.rnext,
-                s.pnext,
-                s.tlen,
-                s.seq,
-                s.qual,
-                json.dumps(OrderedDict(s.tags)),
+    ext = os.path.splitext(fp)[1]
+    if ext == '.sam':
+        mode = 'r'
+    elif ext == '.bam':
+        mode = 'rb'
+    elif ext == '.cram':
+        mode = 'rc'
+    else:
+        raise ValueError(f'{ext} is not a supported filetype')
+
+    with closing(pysam.AlignmentFile(fp, mode)) as f:
+        records = []
+        for s in f.fetch(chrom, start, end):
+            # Needed because array.array is not json serializable
+            tags = [(k, v.tolist() if type(v) == array.array else v) for k, v in s.tags]
+            records.append(
+                (
+                    s.qname,
+                    s.flag,
+                    s.reference_name,
+                    s.pos,
+                    s.mapq,
+                    s.cigarstring if s.mapq != 0 else np.nan,
+                    s.rnext,
+                    s.pnext,
+                    s.tlen,
+                    s.seq,
+                    s.qual,
+                    json.dumps(dict(tags)),
+                )
             )
-            for s in bam_iter
-        ]
         df = pd.DataFrame(records, columns=BAM_FIELDS)
     return df
 
 
+def read_bam(fp, chrom=None, start=None, end=None):
+    """
+    Deprecated: use `read_alignment` instead.
+    Read bam file into dataframe,
+    """
+    return read_alignment(fp, chrom, start, end)
+
+
 class PysamFastaRecord:
     def __init__(self, ff, ref):
         self.ff = ff
         if ref not in ff.references:
             raise KeyError(f"Reference name '{ref}' not found in '{ff}'")
         self.ref = ref
 
@@ -393,17 +414,15 @@
         if end is None:
             end = f.chroms()[chrom]
         ivals = f.intervals(chrom, start, end)
         df = pd.DataFrame(ivals, columns=["start", "end", "value"])
         df.insert(0, "chrom", chrom)
 
     else:
-        raise ValueError(
-            f"engine must be 'auto', 'pybbi' or 'pybigwig'; got {engine}"
-        )
+        raise ValueError(f"engine must be 'auto', 'pybbi' or 'pybigwig'; got {engine}")
 
     return df
 
 
 def read_bigbed(path, chrom, start=None, end=None, engine="auto"):
     """
     Read intervals from a bigBed file.
@@ -450,17 +469,15 @@
         if end is None:
             end = f.chroms()[chrom]
         ivals = f.entries(chrom, start, end)
         df = pd.DataFrame(ivals, columns=["start", "end", "rest"])
         df.insert(0, "chrom", chrom)
 
     else:
-        raise ValueError(
-            f"engine must be 'auto', 'pybbi' or 'pybigwig'; got {engine}"
-        )
+        raise ValueError(f"engine must be 'auto', 'pybbi' or 'pybigwig'; got {engine}")
 
     return df
 
 
 def to_bigwig(df, chromsizes, outpath, value_field=None, path_to_binary=None):
     """
     Save a bedGraph-like dataframe as a binary BigWig track.
@@ -512,29 +529,26 @@
     for col in ["chrom", "start", "end"]:
         if col not in df.columns:
             is_bedgraph = False
     if len(df.columns) < 4:
         is_bedgraph = False
 
     if not is_bedgraph:
-        raise ValueError(
-            f"A bedGraph-like DataFrame is required, got {df.columns}"
-        )
+        raise ValueError(f"A bedGraph-like DataFrame is required, got {df.columns}")
 
     if value_field is None:
         value_field = df.columns[3]
 
     columns = ["chrom", "start", "end", value_field]
     bg = df[columns].copy()
     bg["chrom"] = bg["chrom"].astype(str)
     bg = bg.sort_values(["chrom", "start", "end"])
 
     with tempfile.NamedTemporaryFile(suffix=".bg") as f, \
-         tempfile.NamedTemporaryFile("wt", suffix=".chrom.sizes") as cs: # fmt: skip
-
+         tempfile.NamedTemporaryFile("wt", suffix=".chrom.sizes") as cs:  # fmt: skip
         chromsizes.to_csv(cs, sep="\t", header=False)
         cs.flush()
 
         bg.to_csv(
             f.name, sep="\t", columns=columns, index=False, header=False, na_rep="nan"
         )
 
@@ -606,15 +620,14 @@
     bed = df[columns].copy()
     bed["chrom"] = bed["chrom"].astype(str)
     bed = bed.sort_values(["chrom", "start", "end"])
 
     with tempfile.NamedTemporaryFile(suffix=".bed") as f, tempfile.NamedTemporaryFile(
         "wt", suffix=".chrom.sizes"
     ) as cs:
-
         chromsizes.to_csv(cs, sep="\t", header=False)
         cs.flush()
 
         bed.to_csv(
             f.name, sep="\t", columns=columns, index=False, header=False, na_rep="nan"
         )
```

### Comparing `bioframe-0.6.4/bioframe/io/resources.py` & `bioframe-0.7.0/bioframe/io/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,24 +125,24 @@
         A dataframe with columns 'chrom', 'start', 'end', 'mid'.
     """
     cyb = cyb[cyb[band_col] == "acen"]
     grouped = cyb.groupby("chrom", sort=False)
     cens = []
     for chrom, group in grouped:
         if not len(group) == 2:
-            raise ValueError(
-                f"Expected 2 'acen' bands for {chrom}, found {len(group)}"
-            )
+            raise ValueError(f"Expected 2 'acen' bands for {chrom}, found {len(group)}")
         acens = group.sort_values("start")
-        cens.append({
-            "chrom": chrom,
-            "start": acens.iloc[0]["start"],
-            "end": acens.iloc[1]["end"],
-            "mid": acens.iloc[0]["end"],
-        })
+        cens.append(
+            {
+                "chrom": chrom,
+                "start": acens.iloc[0]["start"],
+                "end": acens.iloc[1]["end"],
+                "mid": acens.iloc[0]["end"],
+            }
+        )
     return pd.DataFrame.from_records(cens)
 
 
 def _origins_from_ucsccentromeres(cens: pd.DataFrame) -> pd.DataFrame:
     """
     Extract chromosomal origin positions from UCSC centromeres.txt table
     describing centromere model sequences. Takes the midpoint of all
@@ -154,18 +154,15 @@
         DataFrame with centromeres.txt data.
 
     Returns
     -------
     pandas.DataFrame
         A dataframe with columns 'chrom', 'start', 'end', 'mid'.
     """
-    cens = cens.groupby("chrom").agg({
-        "start": np.min,
-        "end": np.max
-    }).reset_index()
+    cens = cens.groupby("chrom").agg({"start": np.min, "end": np.max}).reset_index()
     cens["mid"] = (cens["start"] + cens["end"]) // 2
     cens = (
         cens[["chrom", "start", "end", "mid"]]
         .sort_values("chrom")
         .reset_index(drop=True)
     )
     return cens
@@ -229,15 +226,15 @@
             try:
                 df = fetcher()
                 break
             except urllib.error.HTTPError:
                 pass
         else:
             raise ValueError(
-               f"No source for centromere data found from provider '{provider}'."
+                f"No source for centromere data found from provider '{provider}'."
             )
 
         if schema == "centromeres":
             return _origins_from_ucsccentromeres(df)
         else:
             return _origins_from_cytoband(df)
```

### Comparing `bioframe-0.6.4/bioframe/io/schemas.py` & `bioframe-0.7.0/bioframe/io/schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """
 Field names for various genomic tabular files
 
 """
+
 __all__ = ["SCHEMAS"]
 
 
 # UCSC File Formats
 # https://genome.ucsc.edu/FAQ/FAQformat.html
 BED12_FIELDS = [
     "chrom",
     "start",
     "end",
     "name",
     "score",
     "strand",
     "thickStart",
     "thickEnd",
-    "rgb",
+    "itemRgb",
     "blockCount",
     "blockSizes",
     "blockStarts",
 ]
 
 BED_FIELDS = BED12_FIELDS[:6]
 
@@ -103,15 +104,15 @@
     "start",
     "end",
     "name",
     "score",
     "strand",
     "thickStart",
     "thickEnd",
-    "rgb",
+    "itemRgb",
     "blockCount",
     "blockSizes",
     "blockStarts",
     "fc",
     "-log10p",
     "-log10q",
 ]
```

### Comparing `bioframe-0.6.4/bioframe/io/data/_assemblies.yml` & `bioframe-0.7.0/bioframe/io/data/_assemblies.yml`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.4/bioframe/io/data/danRer10.seqinfo.tsv` & `bioframe-0.7.0/bioframe/io/data/danRer10.seqinfo.tsv`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.4/bioframe/io/data/danRer11.seqinfo.tsv` & `bioframe-0.7.0/bioframe/io/data/danRer11.seqinfo.tsv`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.4/bioframe/io/data/dm3.seqinfo.tsv` & `bioframe-0.7.0/bioframe/io/data/dm3.seqinfo.tsv`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 chr2LHet	368872	unlocalized	chr2	primary	2LHet,NW_001848855.1,CM000456.1
 chr2RHet	3288761	unlocalized	chr2	primary	2RHet,NW_001848856.1,CM000457.1
 chr3LHet	2555491	unlocalized	chr3	primary	3LHet,NW_001848857.1,CM000458.1
 chr3RHet	2517507	unlocalized	chr3	primary	3RHet,NW_001848858.1,CM000459.1
 chrXHet	204112	unlocalized	chrX	primary	XHet,NW_001848859.1,CM000460.1
 chrYHet	347038	unlocalized	chrY	primary	YHet,NW_001848860.1,CM000461.1
 chrU	10049037	unplaced		primary	Un,NC_001709.1
-chrUextra	29004656	unplaced		primary	
+chrUextra	29004656	unplaced		primary
```

### Comparing `bioframe-0.6.4/bioframe/io/data/dm6.seqinfo.tsv` & `bioframe-0.7.0/bioframe/io/data/dm6.seqinfo.tsv`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.4/bioframe/io/data/hg19.cytoband.tsv` & `bioframe-0.7.0/bioframe/io/data/hg19.cytoband.tsv`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.4/bioframe/io/data/hg19.seqinfo.tsv` & `bioframe-0.7.0/bioframe/io/data/hg19.seqinfo.tsv`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.4/bioframe/io/data/hg38.cytoband.tsv` & `bioframe-0.7.0/bioframe/io/data/hg38.cytoband.tsv`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.4/bioframe/io/data/hg38.seqinfo.tsv` & `bioframe-0.7.0/bioframe/io/data/hg38.seqinfo.tsv`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.4/bioframe/io/data/hs1.cytoband.tsv` & `bioframe-0.7.0/bioframe/io/data/hs1.cytoband.tsv`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.4/bioframe/io/data/hs1.seqinfo.tsv` & `bioframe-0.7.0/bioframe/io/data/hs1.seqinfo.tsv`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.4/bioframe/io/data/mm10.seqinfo.tsv` & `bioframe-0.7.0/bioframe/io/data/mm10.seqinfo.tsv`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.4/bioframe/io/data/mm39.seqinfo.tsv` & `bioframe-0.7.0/bioframe/io/data/mm39.seqinfo.tsv`

 * *Files 0% similar despite different names*

```diff
@@ -56,8 +56,7 @@
 chrUn_GL456389v1	28772	unplaced		primary	GL456389.1,MSCHRUN_CTG18,NT_166473.1
 chrUn_GL456390v1	24668	unplaced		primary	GL456390.1,MSCHRUN_CTG9,NT_166474.1
 chrUn_GL456392v1	23629	unplaced		primary	GL456392.1,MSCHRUN_CTG10,NT_166476.1
 chrUn_GL456394v1	24323	unplaced		primary	GL456394.1,MSCHRUN_CTG12,NT_166478.1
 chrUn_GL456396v1	21240	unplaced		primary	GL456396.1,MSCHRUN_CTG15,NT_166480.1
 chrUn_JH584304v1	114452	unplaced		primary	JH584304.1,MSCHRUN_CTG23,NT_187064.1
 chrUn_MU069435v1	31129	unplaced		primary	MU069435.1,MSCHRUN_CTG24,NW_023337853.1
-
```

### Comparing `bioframe-0.6.4/bioframe/io/data/mm9.seqinfo.tsv` & `bioframe-0.7.0/bioframe/io/data/mm9.seqinfo.tsv`

 * *Files 13% similar despite different names*

```diff
@@ -17,20 +17,20 @@
 chr16	98319150	assembled	chr16	primary	16,CM001009.1,NC_000082.5
 chr17	95272651	assembled	chr17	primary	17,CM001010.1,NC_000083.5
 chr18	90772031	assembled	chr18	primary	18,CM001011.1,NC_000084.5
 chr19	61342430	assembled	chr19	primary	19,CM001012.1,NC_000085.5
 chrX	166650296	assembled	chrX	primary	X,CM001013.1,NC_000086.6
 chrY	15902555	assembled	chrY	primary	Y,CM001014.1,NC_000087.6
 chrM	16299	assembled	chrM	non-nuclear	MT,AY172335.1,NC_005089.1
-chr1_random	1231697	unlocalized	chr1	primary	
-chr3_random	41899	unlocalized	chr3	primary	
-chr4_random	160594	unlocalized	chr4	primary	
-chr5_random	357350	unlocalized	chr5	primary	
-chr7_random	362490	unlocalized	chr7	primary	
-chr8_random	849593	unlocalized	chr8	primary	
-chr9_random	449403	unlocalized	chr9	primary	
-chr13_random	400311	unlocalized	chr13	primary	
-chr16_random	3994	unlocalized	chr16	primary	
-chr17_random	628739	unlocalized	chr17	primary	
-chrX_random	1785075	unlocalized	chrX	primary	
-chrY_random	58682461	unlocalized	chrY	primary	
-chrUn_random	5900358	unplaced		primary	
+chr1_random	1231697	unlocalized	chr1	primary
+chr3_random	41899	unlocalized	chr3	primary
+chr4_random	160594	unlocalized	chr4	primary
+chr5_random	357350	unlocalized	chr5	primary
+chr7_random	362490	unlocalized	chr7	primary
+chr8_random	849593	unlocalized	chr8	primary
+chr9_random	449403	unlocalized	chr9	primary
+chr13_random	400311	unlocalized	chr13	primary
+chr16_random	3994	unlocalized	chr16	primary
+chr17_random	628739	unlocalized	chr17	primary
+chrX_random	1785075	unlocalized	chrX	primary
+chrY_random	58682461	unlocalized	chrY	primary
+chrUn_random	5900358	unplaced		primary
```

### Comparing `bioframe-0.6.4/bioframe/io/data/sacCer3.seqinfo.tsv` & `bioframe-0.7.0/bioframe/io/data/sacCer3.seqinfo.tsv`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.4/bioframe/sandbox/clients.py` & `bioframe-0.7.0/bioframe/sandbox/clients.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from urllib.parse import urlencode, urljoin
 
 import pandas as pd
 import requests
 
 
 class EncodeClient:
-
     BASE_URL = "http://www.encodeproject.org/"
 
     # 2020-05-15 compatible with ENCODE Metadata at:
     METADATA_URL = "https://www.encodeproject.org/metadata/type=Experiment&status=released/metadata.tsv"
 
     KNOWN_ASSEMBLIES = (
         "GRCh38",
@@ -37,15 +36,14 @@
         if not op.isdir(self.cachedir):
             os.makedirs(self.cachedir, exist_ok=True)
 
         if metadata is None:
             metadata_path = op.join(cachedir, "metadata.tsv")
 
             if not op.exists(metadata_path):
-
                 print(
                     "getting metadata from ENCODE, please wait while "
                     "(~240Mb) file downloads"
                 )
                 with requests.get(self.METADATA_URL, stream=True) as r:
                     r.raise_for_status()
                     with open(metadata_path, "wb") as f:
```

### Comparing `bioframe-0.6.4/bioframe/sandbox/gtf_io.py` & `bioframe-0.7.0/bioframe/sandbox/gtf_io.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,14 +5,12 @@
     item_lists = attrs.str.split(item_sep)
     item_lists = item_lists.apply(
         lambda items: [item.strip().split(kv_sep) for item in items]
     )
     stripchars = quotechar + " "
     item_lists = item_lists.apply(
         lambda items: [
-            [x.strip(stripchars) for x in item]
-            for item in items
-            if len(item) == 2
+            [x.strip(stripchars) for x in item] for item in items if len(item) == 2
         ]
     )
     kv_records = item_lists.apply(dict)
     return pd.DataFrame.from_records(kv_records, **kwargs)
```

### Comparing `bioframe-0.6.4/bioframe/sandbox/parquet_io.py` & `bioframe-0.7.0/bioframe/sandbox/parquet_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def to_parquet(
     pieces,
     outpath,
     row_group_size=None,
     compression="snappy",
     use_dictionary=True,
     version=2.0,
-    **kwargs
+    **kwargs,
 ):
     """
     Save an iterable of dataframe chunks to a single Apache Parquet file. For
     more info about Parquet, see https://arrow.apache.org/docs/python/parquet.html.
 
     Parameters
     ----------
@@ -51,15 +51,15 @@
             if i == 0:
                 writer = pa.parquet.ParquetWriter(
                     outpath,
                     table.schema,
                     compression=compression,
                     use_dictionary=use_dictionary,
                     version=version,
-                    **kwargs
+                    **kwargs,
                 )
             writer.write_table(table, row_group_size=row_group_size)
     finally:
         writer.close()
 
 
 def read_parquet(filepath, columns=None, iterator=False, **kwargs):
```

### Comparing `bioframe-0.6.4/docs/Makefile` & `bioframe-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.4/docs/api-lowlevel.md` & `bioframe-0.7.0/docs/api-lowlevel.md`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
    lowlevel/arrops
    lowlevel/specs
    lowlevel/stringops
 
 ```
 
-Low level array-based operations are used to implement the genomic interval operations on dataframes. 
+Low level array-based operations are used to implement the genomic interval operations on dataframes.
 
 ```{code-cell} ipython3
 import itertools
 
 import numpy as np
 import matplotlib
 import matplotlib.pyplot as plt
```

### Comparing `bioframe-0.6.4/docs/api-resources.rst` & `bioframe-0.7.0/docs/api-resources.rst`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 Bioframe provides a collection of genome assembly metadata for commonly used
 genomes. These are accessible through a convenient dataclass interface via :func:`bioframe.assembly_info`.
 
 The assemblies are listed in a manifest YAML file, and each assembly
 has a mandatory companion file called `seqinfo` that contains the sequence
 names, lengths, and other information. The records in the manifest file contain
-the following fields:   
+the following fields:
 
 - ``organism``: the organism name
 - ``provider``: the genome assembly provider (e.g, ucsc, ncbi)
 - ``provider_build``: the genome assembly build name (e.g., hg19, GRCh37)
 - ``release_year``: the year of the assembly release
 - ``seqinfo``: path to the seqinfo file
 - ``cytobands``: path to the cytoband file, if available
@@ -27,16 +27,16 @@
 - ``name``: canonical sequence name
 - ``length``: sequence length
 - ``role``: role of the sequence or scaffold (e.g., "assembled", "unlocalized", "unplaced")
 - ``molecule``: name of the molecule that the sequence belongs to, if placed
 - ``unit``: assembly unit of the chromosome (e.g., "primary", "non-nuclear", "decoy")
 - ``aliases``: comma-separated list of aliases for the sequence name
 
-We currently do not include sequences with "alt" or "patch" roles in `seqinfo` files, but we 
-do support the inclusion of additional decoy sequences (as used by so-called NGS *analysis 
+We currently do not include sequences with "alt" or "patch" roles in `seqinfo` files, but we
+do support the inclusion of additional decoy sequences (as used by so-called NGS *analysis
 sets* for human genome assemblies) by marking them as members of a "decoy" assembly unit.
 
 The `cytoband` file is an optional TSV file with the following columns (with header):
 
 - ``chrom``: chromosome name
 - ``start``: start position
 - ``end``: end position
@@ -57,13 +57,13 @@
 .. autoclass:: bioframe.io.assembly.GenomeAssembly
    :members:
    :undoc-members:
 
 
 Remote resources
 ----------------
-These functions now default to using the local data store, but can be used to obtain chromsizes or 
+These functions now default to using the local data store, but can be used to obtain chromsizes or
 centromere positions from UCSC by setting ``provider="ucsc"``.
 
 .. automodule:: bioframe.io.resources
    :autosummary:
-   :members:
+   :members:
```

### Comparing `bioframe-0.6.4/docs/conf.py` & `bioframe-0.7.0/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # list see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
 # -- Path setup --------------------------------------------------------------
 # import sys
 from datetime import datetime
 from importlib.metadata import metadata
-from pathlib import Path
+
 # autodoc_mock_imports = ["numpy", "pandas", "matplotlib", "requests"]
 
 
 # -- Project information -----------------------------------------------------
 # NOTE: If you installed your project in editable mode, this might be stale.
 #       If this is the case, reinstall it to refresh the metadata
 info = metadata("bioframe")
@@ -45,15 +45,15 @@
 ]
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
-exclude_patterns = ["_build", "Thumbs.db", ".DS_Store", '**.ipynb_checkpoints']
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store", "**.ipynb_checkpoints"]
 
 # nbsphinx_custom_formats = {
 #     '.md': ['jupytext.reads', {'fmt': 'MyST'}],
 # }
 
 # -- Options for HTML output -------------------------------------------------
 
@@ -72,8 +72,8 @@
 autosummary_generate = True
 
 # Don't include fully qualified name prefixes in autodoc
 add_module_names = False
 
 # Cache MyST (.md or .ipynb) notebook outputs if unmodified
 jupyter_execute_notebooks = "cache"
-execution_excludepatterns = ['guide-performance.ipynb']
+execution_excludepatterns = ["guide-performance.ipynb"]
```

### Comparing `bioframe-0.6.4/docs/guide-definitions.rst` & `bioframe-0.7.0/docs/guide-definitions.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,45 @@
 .. _Definitions:
 
 Definitions
 ===========
-        
+
 Interval:
-    - An *interval* is a tuple of integers (start, end) with start <= end.  
-    - Coordinates are assumed to be 0-based and intervals half-open (1-based ends) i.e. [start, end). 
-    - An interval has a *length* equal to (end - start). 
-    - A special case where start and end are the same, i.e. [X, X), is interpreted as a *point* (aka an *empty interval*, i.e. an edge between 1-bp bins). A point has zero length. 
+    - An *interval* is a tuple of integers (start, end) with start <= end.
+    - Coordinates are assumed to be 0-based and intervals half-open (1-based ends) i.e. [start, end).
+    - An interval has a *length* equal to (end - start).
+    - A special case where start and end are the same, i.e. [X, X), is interpreted as a *point* (aka an *empty interval*, i.e. an edge between 1-bp bins). A point has zero length.
     - Negative coordinates are permissible for both ends of an interval.
-    
+
 Properties of a pair of intervals:
     - Two intervals can either *overlap*, or not. The overlap length = max(0, min(end1, end2) - max(start1, start2)). Empty intervals can have overlap length = 0.
-    - When two intervals overlap, the shorter of the two intervals is said to be *contained* in the longer one if the length of their overlap equals the length of the shorter interval. This property is often referred to as nestedness, but we use the term “contained” as it is less ambiguous when describing the relationship of sets of intervals to one interval. 
-    - If two intervals do not overlap, they have a *distance* = max(0, max(start1, start2) - min(end1, end2)). 
-    - If two intervals have overlap=0 and distance=0, they are said to be *abutting*. 
-    
+    - When two intervals overlap, the shorter of the two intervals is said to be *contained* in the longer one if the length of their overlap equals the length of the shorter interval. This property is often referred to as nestedness, but we use the term “contained” as it is less ambiguous when describing the relationship of sets of intervals to one interval.
+    - If two intervals do not overlap, they have a *distance* = max(0, max(start1, start2) - min(end1, end2)).
+    - If two intervals have overlap=0 and distance=0, they are said to be *abutting*.
+
 Scaffold:
     - A chromosome, contig or, more generally, a *scaffold* is an interval defined by a unique string and has a length>=0, with start=0 and end=length, implicitly defining an interval [0, length).
-    
-Genome assembly: 
+
+Genome assembly:
     - The complete set of scaffolds associated with a genome is called an *assembly* (e.g. defined by the reference sequence from NCBI, etc.).
-    
+
 Genomic interval:
-    - A *genomic interval* is an interval with an associated scaffold, or chromosome, defined by a string, i.e. a triple (chrom, start, end). 
-    - Genomic intervals on different scaffolds never overlap and do not have a defined distance. 
+    - A *genomic interval* is an interval with an associated scaffold, or chromosome, defined by a string, i.e. a triple (chrom, start, end).
+    - Genomic intervals on different scaffolds never overlap and do not have a defined distance.
     - Genomic intervals can extend beyond their associated scaffold (e.g. with negative values or values greater than the scaffold length), as this can be useful in downstream applications. If they do, they are not contained by their associated scaffold.
     - A *base-pair* is a special case of a genomic interval with length=1, i.e. (chrom, start, start+1)
     - *strand* is an (optional) property of a genomic interval which specifies an interval’s orientation on its scaffold. Note start and end are still defined with respect to the scaffold’s reference orientation (positive strand), even if the interval lies on the negative strand. Intervals on different strands can either be allowed to overlap or not.
-    
+
 View (i.e. a set of Genomic Regions):
-    - A genomic *view* is an ordered set of non-overlapping genomic intervals each having a unique name defined by a string. Individual named intervals in a view are *regions*, defined by a quadruple, e.g. (chrom, start, end, name). 
+    - A genomic *view* is an ordered set of non-overlapping genomic intervals each having a unique name defined by a string. Individual named intervals in a view are *regions*, defined by a quadruple, e.g. (chrom, start, end, name).
     - A view thus specifies a unified 1D coordinate system, i.e. a projection of multiple genomic regions onto a single axis.
     - We define views separately from the scaffolds that make up a genome assembly, as a set of more constrained and ordered genomic regions are often useful for downstream analysis and visualization.
     - An assembly is a special case of a view, where the individual regions correspond to the assembly’s entire scaffolds.
 
 Associating genomic intervals with views
     - Similarly to how genomic intervals are associated with a scaffold, they can also be associated with a region from a view with an additional string, making a quadruple (chrom, start, end, view_region). This string must be *cataloged* in the view, i.e. it must match the name of a region in the view. Typically the interval would be contained in its associated view region, or, at the minimum, have a greater overlap with that region than other view regions.
     - If each interval in a set is contained in their associated view region, the set is *contained* in the view.
     - A set of intervals *covers* a view if each region in the view is contained by the union of its associated intervals. Conversely, if a set does not cover all of view regions, the interval set will have *gaps* relative to that view (stretches of bases not covered by an interval).
 
 Properties of sets of genomic intervals:
     - A set of genomic intervals may have overlaps or not. If it does not, it is said to be *overlap-free*.
-    - A set of genomic intervals is *tiling* if it: (i) covers the associated view, (ii) is contained in that view, and (iii) is overlap-free. Equivalently, a tiling set of intervals (a) has an initial interval that begins at the start of each region and (b) a final interval that terminates at the end of each region, and (c) every base pair is associated with a unique interval. 
-
-
+    - A set of genomic intervals is *tiling* if it: (i) covers the associated view, (ii) is contained in that view, and (iii) is overlap-free. Equivalently, a tiling set of intervals (a) has an initial interval that begins at the start of each region and (b) a final interval that terminates at the end of each region, and (c) every base pair is associated with a unique interval.
```

### Comparing `bioframe-0.6.4/docs/guide-intervalops.md` & `bioframe-0.7.0/docs/guide-intervalops.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     jupytext_version: 1.11.3
 kernelspec:
   display_name: Python 3
   language: python
   name: python3
 ---
 
-# Genomic interval operations 
+# Genomic interval operations
 
 ```{eval-rst}
 This guide provides an introdution into how to use bioframe to perform genomic interval operations. For the full list of genomic interval operations, see the :ref:`API reference<API_ops>`.
 
 The following modules are used in this guide:
 ```
 ```{code-cell} ipython3
@@ -47,28 +47,28 @@
 ```
 ```{eval-rst}
 Or via functions in :mod:`bioframe.core.construction`, e.g.:
 ```
 ```{code-cell} ipython3
 df2 = bioframe.from_any(
     [['chr1', 4, 8],
-     ['chr1', 10, 11]], 
+     ['chr1', 10, 11]],
     name_col='chrom')
 ```
 ```{eval-rst}
 Or ingested from datasets and databases with functions in :mod:`bioframe.io.fileops` and :mod:`bioframe.io.resources`.
 ```
 
 ```{eval-rst}
-BedFrames satisfy the following properties:  
+BedFrames satisfy the following properties:
 
-- chrom, start, end columns  
-- columns have valid dtypes (object/string/categorical, int/pd.Int64Dtype(), int/pd.Int64Dtype())  
+- chrom, start, end columns
+- columns have valid dtypes (object/string/categorical, int/pd.Int64Dtype(), int/pd.Int64Dtype())
 - for each interval, if any of chrom, start, end are null, then all are null
-- all starts <= ends.  
+- all starts <= ends.
 
 Whether a dataframe satisfies these properties can be checked with :func:`bioframe.core.checks.is_bedframe`:
 ```
 ```{code-cell} ipython3
 bioframe.is_bedframe(df2)
 ```
 ```{eval-rst}
@@ -94,15 +94,15 @@
 Using :func:`bioframe.overlap`, we can see the two dataframes defined above, ``df1`` and ``df2``, contain two pairs of overlapping intervals:
 ```
 ```{code-cell} ipython3
 overlapping_intervals = bf.overlap(df1, df2, how='inner', suffixes=('_1','_2'))
 display(overlapping_intervals)
 ```
 ```{code-cell} ipython3
-for i, reg_pair in overlapping_intervals.iterrows(): 
+for i, reg_pair in overlapping_intervals.iterrows():
     bf.vis.plot_intervals_arr(
         starts = [reg_pair.start_1,reg_pair.start_2],
         ends = [reg_pair.end_1,reg_pair.end_2],
         colors = ['skyblue', 'lightpink'],
         levels = [2,1],
         xlim = (0,16),
         show_coords = True)
@@ -154,15 +154,15 @@
 df_annotated = bf.cluster(df1, min_dist=2)
 display(df_annotated)
 bf.vis.plot_intervals(df_annotated, labels=df_annotated['cluster'], show_coords=True, xlim=(0,16))
 ```
 
 ## Merge
 ```{eval-rst}
-Instead of returning cluster assignments, :func:`bioframe.merge` returns a new dataframe of merged genomic intervals. As with :func:`bioframe.cluster`, using ``min_dist=0`` and ``min_dist=None`` gives different results. 
+Instead of returning cluster assignments, :func:`bioframe.merge` returns a new dataframe of merged genomic intervals. As with :func:`bioframe.cluster`, using ``min_dist=0`` and ``min_dist=None`` gives different results.
 
 If ``min_dist=0``, this returns a dataframe of two intervals:
 ```
 ```{code-cell} ipython3
 df_merged = bf.merge(df1, min_dist=0)
 
 display(df_merged)
@@ -181,67 +181,67 @@
 In genomics, it is often useful not only to find features that overlap, but also features that are nearby along the genome. In bioframe, this is achieved using :func:`bioframe.closest`.
 ```
 ```{code-cell} ipython3
 closest_intervals = bf.closest(df1, df2, suffixes=('_1','_2'))
 display(closest_intervals)
 ```
 ```{code-cell} ipython3
-for i, reg_pair in closest_intervals.iterrows(): 
+for i, reg_pair in closest_intervals.iterrows():
     bf.vis.plot_intervals_arr(
         starts = [reg_pair.start_1,reg_pair.start_2],
         ends = [reg_pair.end_1,reg_pair.end_2],
         colors = ['skyblue', 'lightpink'],
         levels = [2,1],
         xlim = (0,16),
         show_coords = True)
     plt.title(f'closest pair #{i}')
 ```
 
 ```{eval-rst}
-By default, :func:`bioframe.closest` reports overlapping intervals. This can be modified by passing ``ignore_overlap=True``. Note the closest pair #2 and #3, which did not overlap, remain the same: 
+By default, :func:`bioframe.closest` reports overlapping intervals. This can be modified by passing ``ignore_overlap=True``. Note the closest pair #2 and #3, which did not overlap, remain the same:
 ```
 ```{code-cell} ipython3
 closest_intervals = bf.closest(df1, df2, ignore_overlaps=True, suffixes=('_1','_2'))
-for i, reg_pair in closest_intervals.iterrows(): 
+for i, reg_pair in closest_intervals.iterrows():
     bf.vis.plot_intervals_arr(
         starts = [reg_pair.start_1,reg_pair.start_2],
         ends = [reg_pair.end_1,reg_pair.end_2],
         colors = ['skyblue', 'lightpink'],
         levels = [2,1],
         xlim = (0,16),
         show_coords = True)
     plt.title(f'closest pair #{i}')
 ```
 
 ```{eval-rst}
-Closest intervals within a single DataFrame can be found simply by passing a single dataframe to :func:`bioframe.closest`. The number of closest intervals to report per query interval can be adjusted with ``k``. 
+Closest intervals within a single DataFrame can be found simply by passing a single dataframe to :func:`bioframe.closest`. The number of closest intervals to report per query interval can be adjusted with ``k``.
 ```
 ```{code-cell} ipython3
 bf.closest(df1, k=2)
 ```
 
 ```{eval-rst}
-Closest intervals upstream of the features in df1 can be found by ignoring downstream and overlaps. 
+Closest intervals upstream of the features in df1 can be found by ignoring downstream and overlaps.
 Upstream/downstream direction is defined by genomic coordinates by default (smaller coordinate is upstream).
 ```
 ```{code-cell} ipython3
-bf.closest(df1, df2, 
-    ignore_overlaps=True, 
+bf.closest(df1, df2,
+    ignore_overlaps=True,
     ignore_downstream=True)
 ```
 
 ```{eval-rst}
 If the features in df1 have direction (e.g., genes have transcription direction), then the definition of upstream/downstream
 direction can be changed to the direction of the features by `direction_col`:
 ```
 ```{code-cell} ipython3
 df1["strand"] = np.where(np.random.rand(len(df1)) > 0.5, "+", "-")
-bf.closest(df1, df2, 
-    ignore_overlaps=True, 
-    ignore_downstream=True, 
+bf.closest(df1, df2,
+    ignore_overlaps=True,
+    ignore_downstream=True,
     direction_col='strand')
 ```
 
 
 ## Coverage & Count Overlaps
 ```{eval-rst}
 For two sets of genomic features, it is often useful to calculate the number of basepairs covered and the number of overlapping intervals. While these are fairly straightforward to compute from the output of :func:`bioframe.overlap` with :func:`pandas.groupby` and column renaming, since these are very frequently used, they are provided as core bioframe functions.
@@ -255,17 +255,17 @@
 df1_coverage_and_count = bf.count_overlaps(df1_coverage, df2)
 display(df1_coverage_and_count)
 ```
 
 This plot shows the coverage and number of overlaps for intervals in ``df1`` by ``df2``:
 ```{code-cell} ipython3
 bf.vis.plot_intervals(
-    df1_coverage_and_count, 
-    show_coords=True, xlim=(0,16), 
-    labels = [f'{cov} bp, {n} intervals' 
+    df1_coverage_and_count,
+    show_coords=True, xlim=(0,16),
+    labels = [f'{cov} bp, {n} intervals'
               for cov, n in zip(df1_coverage_and_count.coverage, df1_coverage_and_count['count'])])
 
 bf.vis.plot_intervals(df2, show_coords=True, xlim=(0,16), colors='lightpink')
 ```
 
 ## Subtract & Set Difference
 ```{eval-rst}
@@ -290,19 +290,19 @@
 ```
 ```{code-cell} ipython3
 bf.vis.plot_intervals(setdiff_intervals, show_coords=True, xlim=(0,16))
 ```
 
 ## Expand
 ```{eval-rst}
-:func:`bioframe.expand` enables quick resizing of intervals. 
+:func:`bioframe.expand` enables quick resizing of intervals.
 
 
-Expand supports additive resizing, with ``pad``. 
-Note that unless subsequently trimmed (with :func:`bioframe.trim`), 
+Expand supports additive resizing, with ``pad``.
+Note that unless subsequently trimmed (with :func:`bioframe.trim`),
 expanded intervals can have negative values:
 ```
 ```{code-cell} ipython3
 expanded_intervals = bf.expand(df1, pad=2)
 display(expanded_intervals)
 ```
 ```{code-cell} ipython3
@@ -320,31 +320,31 @@
 bf.vis.plot_intervals(expanded_intervals, show_coords=True, xlim=(0,16))
 ```
 
 ## Genomic Views
 ```{eval-rst}
 Certain interval operations are often used relative to a set of reference intervals, whether those are chromosomes, scaffolds, or sub-intervals of either. Bioframe formalizes this with the concept of a `genomic view`, implemented as pandas dataframes, termed viewFrames, that satisfy the following:
 
-- all requirements for bedFrames, including columns for ('chrom', 'start', 'end')  
-- it has an additional column, ``view_name_col``, with default 'name'  
-- entries in the view_name_col are unique 
-- intervals are non-overlapping  
-- it does not contain null values  
+- all requirements for bedFrames, including columns for ('chrom', 'start', 'end')
+- it has an additional column, ``view_name_col``, with default 'name'
+- entries in the view_name_col are unique
+- intervals are non-overlapping
+- it does not contain null values
 
-Importanly a `genomic view` specifies a global coordinate axis, i.e. a conversion from a genomic coordinate system to a single axis. See :ref:`Technical Notes<Technical_Notes>` for more details. 
+Importanly a `genomic view` specifies a global coordinate axis, i.e. a conversion from a genomic coordinate system to a single axis. See :ref:`Technical Notes<Technical_Notes>` for more details.
 
 Bioframe provides a function to assign intervals to corresponding intervals in a view, :func:`bioframe.assign_view`, a function to construct views from various input formats, :func:`bioframe.core.construction.make_viewframe`, and a function check that viewframe requirements are met, :func:`bioframe.core.checks.is_viewframe`.
 
-The following genomic interval operations make use of views, though also have useful default behavior if no view is provided: :func:`bioframe.complement`, :func:`bioframe.trim`, :func:`bioframe.sort_bedframe`.  
+The following genomic interval operations make use of views, though also have useful default behavior if no view is provided: :func:`bioframe.complement`, :func:`bioframe.trim`, :func:`bioframe.sort_bedframe`.
 
 ```
 
 ## Complement
 ```{eval-rst}
-Equally important to finding which genomic features overlap is finding those that do not. :func:`bioframe.complement` returns a BedFrame of intervals not covered by any intervals in an input BedFrame. 
+Equally important to finding which genomic features overlap is finding those that do not. :func:`bioframe.complement` returns a BedFrame of intervals not covered by any intervals in an input BedFrame.
 
 Complments are defined relative to a `genomic view`. Here this is provided as a dictionary with a single chromosome of length 15:
 ```
 
 ```{code-cell} ipython3
 df_complemented = bf.complement(df1, view_df={'chr1':15})
 display(df_complemented)
@@ -418,17 +418,17 @@
 display( bioframe.select(df_unsorted,'chrX:8-14') )
 ```
 
 ## Flexible column naming
 
 +++
 
-Genomic analyses often deal with dataframes with inhomogeneously named columns. Bioframe offers a way to set the default column names that are most convenient for your analyses. 
+Genomic analyses often deal with dataframes with inhomogeneously named columns. Bioframe offers a way to set the default column names that are most convenient for your analyses.
 
-Default bedframe column names are stored in ``bioframe.core.specs_rc``. 
+Default bedframe column names are stored in ``bioframe.core.specs_rc``.
 
 ```{code-cell} ipython3
 bf.core.specs._rc
 ```
 
 If the dataframes we wish to work with have `['CHROMOSOME', 'LEFT', 'RIGHT']`, we can either pass cols to operations in ``bioframe.ops``:
 
@@ -464,8 +464,7 @@
 ```
 
 ```{code-cell} ipython3
 # setting colnames back to default.
 bf.core.specs.update_default_colnames(['chrom', 'start', 'end'])
 bf.core.specs._rc
 ```
-
```

### Comparing `bioframe-0.6.4/docs/guide-io.ipynb` & `bioframe-0.7.0/docs/guide-io.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.996062421679198%*

 * *Differences: {"'cells'": "{5: {'source': {insert: [(1, '    "*

 * *            '"https://www.encodeproject.org/files/ENCFF001XKR/@@download/ENCFF001XKR.bed.gz",\\n\'), '*

 * *            '(2, \'    schema="bed9",\\n\')], delete: [2, 1]}}, 6: {\'source\': {insert: [(1, '*

 * *            "'    "*

 * *            '"https://www.encodeproject.org/files/ENCFF401MQL/@@download/ENCFF401MQL.bed.gz",\\n\'), '*

 * *            '(2, \'    schema="narrowPeak",\\n\'), (3, \')\\n\')], delete: [2, 1]}}, 7: '*

 * *            "{'source': {insert: [(1, '    "*

 * *       […]*

```diff
@@ -47,41 +47,42 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "df = bioframe.read_table(\n",
-                "    'https://www.encodeproject.org/files/ENCFF001XKR/@@download/ENCFF001XKR.bed.gz', \n",
-                "    schema='bed9'\n",
+                "    \"https://www.encodeproject.org/files/ENCFF001XKR/@@download/ENCFF001XKR.bed.gz\",\n",
+                "    schema=\"bed9\",\n",
                 ")\n",
                 "display(df[0:3])"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "df = bioframe.read_table(\n",
-                "    \"https://www.encodeproject.org/files/ENCFF401MQL/@@download/ENCFF401MQL.bed.gz\", \n",
-                "     schema='narrowPeak')\n",
+                "    \"https://www.encodeproject.org/files/ENCFF401MQL/@@download/ENCFF401MQL.bed.gz\",\n",
+                "    schema=\"narrowPeak\",\n",
+                ")\n",
                 "display(df[0:3])"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "df = bioframe.read_table(\n",
-                "    'https://www.encodeproject.org/files/ENCFF001VRS/@@download/ENCFF001VRS.bed.gz', \n",
-                "     schema='bed12'\n",
+                "    \"https://www.encodeproject.org/files/ENCFF001VRS/@@download/ENCFF001VRS.bed.gz\",\n",
+                "    schema=\"bed12\",\n",
                 ")\n",
                 "display(df[0:3])"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
@@ -92,15 +93,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "bioframe.SCHEMAS['bed6']"
+                "bioframe.SCHEMAS[\"bed6\"]"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -111,49 +112,49 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "bw_url = 'http://genome.ucsc.edu/goldenPath/help/examples/bigWigExample.bw'\n",
+                "bw_url = \"http://genome.ucsc.edu/goldenPath/help/examples/bigWigExample.bw\"\n",
                 "df = bioframe.read_bigwig(bw_url, \"chr21\", start=10_000_000, end=10_010_000)\n",
                 "df.head(5)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "df['value'] *= 100\n",
+                "df[\"value\"] *= 100\n",
                 "df.head(5)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "chromsizes = bioframe.fetch_chromsizes('hg19')\n",
-                "# bioframe.to_bigwig(df, chromsizes, 'times100.bw')  \n",
+                "chromsizes = bioframe.fetch_chromsizes(\"hg19\")\n",
+                "# bioframe.to_bigwig(df, chromsizes, 'times100.bw')\n",
                 "\n",
                 "# note: requires UCSC bedGraphToBigWig binary, which can be installed as\n",
                 "# !conda install -y -c bioconda ucsc-bedgraphtobigwig"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "bb_url = 'http://genome.ucsc.edu/goldenPath/help/examples/bigBedExample.bb'\n",
+                "bb_url = \"http://genome.ucsc.edu/goldenPath/help/examples/bigBedExample.bb\"\n",
                 "bioframe.read_bigbed(bb_url, \"chr21\", start=48000000).head()"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
@@ -182,56 +183,61 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "bioframe.read_chromsizes(\n",
-                "    'https://hgdownload.soe.ucsc.edu/goldenPath/hg38/bigZips/hg38.chrom.sizes'\n",
+                "    \"https://hgdownload.soe.ucsc.edu/goldenPath/hg38/bigZips/hg38.chrom.sizes\"\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "bioframe.read_chromsizes('https://hgdownload.soe.ucsc.edu/goldenPath/hg38/bigZips/hg38.chrom.sizes',\n",
-                "                         filter_chroms=False)"
+                "bioframe.read_chromsizes(\n",
+                "    \"https://hgdownload.soe.ucsc.edu/goldenPath/hg38/bigZips/hg38.chrom.sizes\",\n",
+                "    filter_chroms=False,\n",
+                ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "dm6_url = 'https://hgdownload.soe.ucsc.edu/goldenPath/dm6/database/chromInfo.txt.gz'"
+                "dm6_url = \"https://hgdownload.soe.ucsc.edu/goldenPath/dm6/database/chromInfo.txt.gz\""
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "bioframe.read_chromsizes(dm6_url,\n",
-                "                         filter_chroms=True, \n",
-                "                         chrom_patterns=(\"^chr2L$\", \"^chr2R$\", \"^chr3L$\", \"^chr3R$\", \"^chr4$\", \"^chrX$\")\n",
+                "bioframe.read_chromsizes(\n",
+                "    dm6_url,\n",
+                "    filter_chroms=True,\n",
+                "    chrom_patterns=(\"^chr2L$\", \"^chr2R$\", \"^chr3L$\", \"^chr3R$\", \"^chr4$\", \"^chrX$\"),\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "bioframe.read_chromsizes(dm6_url, chrom_patterns=[\"^chr\\d+L$\", \"^chr\\d+R$\", \"^chr4$\", \"^chrX$\", \"^chrM$\"])"
+                "bioframe.read_chromsizes(\n",
+                "    dm6_url, chrom_patterns=[r\"^chr\\d+L$\", r\"^chr\\d+R$\", \"^chr4$\", \"^chrX$\", \"^chrM$\"]\n",
+                ")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -240,15 +246,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "chromsizes = bioframe.fetch_chromsizes('hg38')\n",
+                "chromsizes = bioframe.fetch_chromsizes(\"hg38\")\n",
                 "chromsizes[-5:]"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
@@ -258,17 +264,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "display(\n",
-                "    bioframe.fetch_centromeres('hg38')[:3]\n",
-                ")"
+                "display(bioframe.fetch_centromeres(\"hg38\")[:3])"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -277,15 +281,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "client = bioframe.UCSCClient('hg38')\n",
+                "client = bioframe.UCSCClient(\"hg38\")\n",
                 "client.fetch_cytoband()"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
```

### Comparing `bioframe-0.6.4/docs/guide-performance.ipynb` & `bioframe-0.7.0/docs/guide-performance.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9974303508401792%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(1, '## Optional:\\n')], delete: [1]}}, 3: {'source': "*

 * *            "{insert: [(2, 'import matplotlib.pyplot as plt\\n'), (5, 'import psutil\\n'), (6, "*

 * *            '\'import pyranges\\n\'), (9, \'\\n\'), (10, \'plt.rcParams["figure.facecolor"] = '*

 * *            '"white"\\n\'), (11, \'plt.rcParams["font.size"] = 16\\n\'), (16, \'if '*

 * *            "include_pybedtools:\\n'), (18, '\\n'), (19, '    "*

 * *            'pybedtools.helpers.set_bedtools_path(\\n\'), (20, \'        pat […]*

```diff
@@ -17,43 +17,47 @@
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# ! pip install pyranges\n",
-                "## Optional: \n",
+                "## Optional:\n",
                 "# ! conda install -c bioconda bedtools\n",
                 "# ! pip install pybedtools"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import platform\n",
-                "import psutil\n",
                 "\n",
+                "import matplotlib.pyplot as plt\n",
                 "import numpy as np\n",
                 "import pandas as pd\n",
-                "import matplotlib.pyplot as plt\n",
-                "plt.rcParams['figure.facecolor']='white'\n",
-                "plt.rcParams['font.size']=16\n",
+                "import psutil\n",
+                "import pyranges\n",
                 "\n",
                 "import bioframe\n",
-                "import pyranges\n",
+                "\n",
+                "plt.rcParams[\"figure.facecolor\"] = \"white\"\n",
+                "plt.rcParams[\"font.size\"] = 16\n",
                 "\n",
                 "# Note that by default we switch off the demo of pybedtools.\n",
                 "# It runs for minutes for 10^5 intervals\n",
                 "include_pybedtools = False\n",
-                "if include_pybedtools: \n",
+                "if include_pybedtools:\n",
                 "    import pybedtools\n",
-                "    pybedtools.helpers.set_bedtools_path(path='/usr/bin/') # Set the path to bedtools CLI"
+                "\n",
+                "    pybedtools.helpers.set_bedtools_path(\n",
+                "        path=\"/usr/bin/\"\n",
+                "    )  # Set the path to bedtools CLI"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {},
             "outputs": [
@@ -67,19 +71,19 @@
                         "24 CPUs at 3040 GHz\n"
                     ]
                 }
             ],
             "source": [
                 "print(f\"Bioframe v.{bioframe.__version__}\")\n",
                 "print(f\"PyRanges v.{pyranges.__version__}\")\n",
-                "if include_pybedtools: \n",
+                "if include_pybedtools:\n",
                 "    print(f\"Pybedtools v.{pybedtools.__version__}\")\n",
                 "\n",
                 "print(f\"System Platform: {platform.platform()}\")\n",
-                "print(f\"{psutil.cpu_count()} CPUs at {psutil.cpu_freq().current:.0f} GHz\") "
+                "print(f\"{psutil.cpu_count()} CPUs at {psutil.cpu_freq().current:.0f} GHz\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Below we define a function to generate random intervals with various properties, returning a dataframe of intervals."
@@ -88,45 +92,41 @@
         {
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {},
             "outputs": [],
             "source": [
                 "def make_random_intervals(\n",
-                "        n=1e5, \n",
-                "        n_chroms=1, \n",
-                "        max_coord=None, \n",
-                "        max_length=10, \n",
-                "        sort=False,\n",
-                "        categorical_chroms=False,\n",
-                "        \n",
-                "    ):\n",
+                "    n=1e5,\n",
+                "    n_chroms=1,\n",
+                "    max_coord=None,\n",
+                "    max_length=10,\n",
+                "    sort=False,\n",
+                "    categorical_chroms=False,\n",
+                "):\n",
                 "    n = int(n)\n",
                 "    n_chroms = int(n_chroms)\n",
                 "    max_coord = (n // n_chroms) if max_coord is None else int(max_coord)\n",
                 "    max_length = int(max_length)\n",
-                "    \n",
-                "    chroms = np.array(['chr'+str(i+1) for i in range(n_chroms)])[\n",
-                "        np.random.randint(0, n_chroms, n)]\n",
+                "\n",
+                "    chroms = np.array([\"chr\" + str(i + 1) for i in range(n_chroms)])[\n",
+                "        np.random.randint(0, n_chroms, n)\n",
+                "    ]\n",
                 "    starts = np.random.randint(0, max_coord, n)\n",
                 "    ends = starts + np.random.randint(1, max_length, n)\n",
                 "\n",
-                "    df = pd.DataFrame({\n",
-                "        'chrom':chroms,\n",
-                "        'start':starts,\n",
-                "        'end':ends\n",
-                "    })\n",
-                "    \n",
+                "    df = pd.DataFrame({\"chrom\": chroms, \"start\": starts, \"end\": ends})\n",
+                "\n",
                 "    if categorical_chroms:\n",
-                "        df['chrom'] = df['chrom'].astype('category')\n",
+                "        df[\"chrom\"] = df[\"chrom\"].astype(\"category\")\n",
                 "\n",
                 "    if sort:\n",
-                "        df = df.sort_values(['chrom','start','end']).reset_index(drop=True)\n",
-                "        \n",
-                "    return df\n"
+                "        df = df.sort_values([\"chrom\", \"start\", \"end\"]).reset_index(drop=True)\n",
+                "\n",
+                "    return df"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Overlap"
@@ -191,18 +191,18 @@
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "plt.loglog(\n",
                 "    list(timings.keys()),\n",
                 "    list([r.average for r in timings.values()]),\n",
-                "    'o-',\n",
+                "    \"o-\",\n",
                 ")\n",
-                "plt.xlabel('N intervals')\n",
-                "plt.ylabel('time, seconds')\n",
+                "plt.xlabel(\"N intervals\")\n",
+                "plt.ylabel(\"time, seconds\")\n",
                 "plt.gca().set_aspect(1.0)\n",
                 "plt.grid()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -235,16 +235,16 @@
                 }
             ],
             "source": [
                 "timings = {}\n",
                 "n_intersections = {}\n",
                 "n = 1e4\n",
                 "for avg_interval_len in [3, 1e1, 3e1, 1e2, 3e2]:\n",
-                "    df = make_random_intervals(n=n, n_chroms=1, max_length=avg_interval_len*2)\n",
-                "    df2 = make_random_intervals(n=n, n_chroms=1, max_length=avg_interval_len*2)\n",
+                "    df = make_random_intervals(n=n, n_chroms=1, max_length=avg_interval_len * 2)\n",
+                "    df2 = make_random_intervals(n=n, n_chroms=1, max_length=avg_interval_len * 2)\n",
                 "    timings[avg_interval_len] = %timeit -o -r 1 bioframe.overlap(df, df2)\n",
                 "    n_intersections[avg_interval_len] = bioframe.overlap(df, df2).shape[0]"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 8,
@@ -261,18 +261,18 @@
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "plt.loglog(\n",
                 "    list(n_intersections.values()),\n",
                 "    list([r.average for r in timings.values()]),\n",
-                "    'o-',\n",
+                "    \"o-\",\n",
                 ")\n",
-                "plt.xlabel('N intersections')\n",
-                "plt.ylabel('time, seconds')\n",
+                "plt.xlabel(\"N intersections\")\n",
+                "plt.ylabel(\"time, seconds\")\n",
                 "plt.gca().set_aspect(1.0)\n",
                 "plt.grid()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -310,15 +310,15 @@
                 "timings = {}\n",
                 "n_intersections = {}\n",
                 "n = 1e5\n",
                 "for n_chroms in [1, 3, 10, 30, 100, 300, 1000]:\n",
                 "    df = make_random_intervals(n, n_chroms)\n",
                 "    df2 = make_random_intervals(n, n_chroms)\n",
                 "    timings[n_chroms] = %timeit -o -r 1 bioframe.overlap(df, df2)\n",
-                "    n_intersections[n_chroms] = bioframe.overlap(df, df2).shape[0]\n"
+                "    n_intersections[n_chroms] = bioframe.overlap(df, df2).shape[0]"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Note this test preserves the number of intersections, which is likely why performance remains similar over the considered range."
@@ -366,19 +366,19 @@
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "plt.loglog(\n",
                 "    list(timings.keys()),\n",
                 "    list([r.average for r in timings.values()]),\n",
-                "    'o-',\n",
+                "    \"o-\",\n",
                 ")\n",
                 "plt.ylim([1e-1, 10])\n",
-                "plt.xlabel('# chromosomes')\n",
-                "plt.ylabel('time, seconds')\n",
+                "plt.xlabel(\"# chromosomes\")\n",
+                "plt.ylabel(\"time, seconds\")\n",
                 "# plt.gca().set_aspect(1.0)\n",
                 "plt.grid()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -496,34 +496,34 @@
                         "Categorical chromosomes (outer/inner joins):\n",
                         "333 ms \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 1 loop each)\n",
                         "90 ms \u00b1 0 ns per loop (mean \u00b1 std. dev. of 1 run, 10 loops each)\n"
                     ]
                 }
             ],
             "source": [
-                "print('Default inputs (outer/inner joins):')\n",
+                "print(\"Default inputs (outer/inner joins):\")\n",
                 "df = make_random_intervals()\n",
                 "df2 = make_random_intervals()\n",
                 "\n",
                 "%timeit -r 1 bioframe.overlap(df, df2)\n",
                 "%timeit -r 1 bioframe.overlap(df, df2, how='inner')\n",
                 "\n",
-                "print('Sorted inputs (outer/inner joins):')\n",
+                "print(\"Sorted inputs (outer/inner joins):\")\n",
                 "df_sorted = make_random_intervals(sort=True)\n",
                 "df2_sorted = make_random_intervals(sort=True)\n",
                 "\n",
                 "%timeit -r 1 bioframe.overlap(df_sorted, df2_sorted)\n",
                 "%timeit -r 1 bioframe.overlap(df_sorted, df2_sorted, how='inner')\n",
                 "\n",
-                "print('Categorical chromosomes (outer/inner joins):')\n",
+                "print(\"Categorical chromosomes (outer/inner joins):\")\n",
                 "df_cat = make_random_intervals(categorical_chroms=True)\n",
                 "df2_cat = make_random_intervals(categorical_chroms=True)\n",
                 "\n",
                 "%timeit -r 1 bioframe.overlap(df_cat, df2_cat)\n",
-                "%timeit -r 1 bioframe.overlap(df_cat, df2_cat, how='inner')\n"
+                "%timeit -r 1 bioframe.overlap(df_cat, df2_cat, how='inner')"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Vs Pyranges (and, optionally, pybedtools)"
@@ -547,17 +547,17 @@
             "cell_type": "code",
             "execution_count": 16,
             "metadata": {},
             "outputs": [],
             "source": [
                 "def df2pr(df):\n",
                 "    return pyranges.PyRanges(\n",
-                "    chromosomes=df.chrom,\n",
-                "    starts=df.start,\n",
-                "    ends=df.end,\n",
+                "        chromosomes=df.chrom,\n",
+                "        starts=df.start,\n",
+                "        ends=df.end,\n",
                 "    )"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 17,
             "metadata": {},
@@ -586,16 +586,15 @@
                 "timings_pr = {}\n",
                 "for n in [1e2, 1e3, 1e4, 1e5, 1e6, 3e6]:\n",
                 "    df = make_random_intervals(n=n, n_chroms=1)\n",
                 "    df2 = make_random_intervals(n=n, n_chroms=1)\n",
                 "    pr = df2pr(df)\n",
                 "    pr2 = df2pr(df2)\n",
                 "    timings_bf[n] = %timeit -o -r 1 bioframe.overlap(df, df2,how='inner')\n",
-                "    timings_pr[n] = %timeit -o -r 1 pr.join(pr2)\n",
-                "    "
+                "    timings_pr[n] = %timeit -o -r 1 pr.join(pr2)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 18,
             "metadata": {},
             "outputs": [
@@ -620,29 +619,29 @@
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "plt.loglog(\n",
                 "    list(timings_bf.keys()),\n",
                 "    list([r.average for r in timings_bf.values()]),\n",
-                "    'o-',\n",
-                "    label='bioframe'\n",
+                "    \"o-\",\n",
+                "    label=\"bioframe\",\n",
                 ")\n",
                 "plt.loglog(\n",
                 "    list(timings_pr.keys()),\n",
                 "    list([r.average for r in timings_pr.values()]),\n",
-                "    'o-',\n",
-                "    label='pyranges'\n",
+                "    \"o-\",\n",
+                "    label=\"pyranges\",\n",
                 ")\n",
                 "\n",
                 "plt.gca().set(\n",
-                "    xlabel='N intervals',\n",
-                "    ylabel='time, seconds',\n",
+                "    xlabel=\"N intervals\",\n",
+                "    ylabel=\"time, seconds\",\n",
                 "    aspect=1.0,\n",
-                "    xticks=10**np.arange(2,6.1)\n",
+                "    xticks=10 ** np.arange(2, 6.1),\n",
                 ")\n",
                 "plt.grid()\n",
                 "plt.legend()"
             ]
         },
         {
             "cell_type": "markdown",
@@ -663,15 +662,17 @@
             "execution_count": 19,
             "metadata": {},
             "outputs": [],
             "source": [
                 "def pyranges_intersect_dfs(df, df2):\n",
                 "    return df2pr(df).intersect(df2pr(df2)).as_df()\n",
                 "\n",
+                "\n",
                 "if include_pybedtools:\n",
+                "\n",
                 "    def pybedtools_intersect_dfs(bed1, bed2):\n",
                 "        return bed1.intersect(bed2).to_dataframe()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 20,
@@ -697,15 +698,15 @@
                 }
             ],
             "source": [
                 "timings_bf = {}\n",
                 "timings_pr = {}\n",
                 "if include_pybedtools:\n",
                 "    timings_pb = {}\n",
-                "    \n",
+                "\n",
                 "for n in [1e2, 1e3, 1e4, 1e5, 1e6, 3e6]:\n",
                 "    df = make_random_intervals(n=n, n_chroms=1)\n",
                 "    df2 = make_random_intervals(n=n, n_chroms=1)\n",
                 "    timings_bf[n] = %timeit -o -r 1 bioframe.overlap(df, df2, how='inner')\n",
                 "    timings_pr[n] = %timeit -o -r 1 pyranges_intersect_dfs(df, df2)\n",
                 "    if include_pybedtools:\n",
                 "        bed1 = pybedtools.BedTool.from_dataframe(df)\n",
@@ -739,35 +740,31 @@
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "plt.loglog(\n",
                 "    list(timings_bf.keys()),\n",
                 "    list([r.average for r in timings_bf.values()]),\n",
-                "    'o-',\n",
-                "    label='bioframe'\n",
+                "    \"o-\",\n",
+                "    label=\"bioframe\",\n",
                 ")\n",
                 "plt.loglog(\n",
                 "    list(timings_pr.keys()),\n",
                 "    list([r.average for r in timings_pr.values()]),\n",
-                "    'o-',\n",
-                "    label='pyranges'\n",
+                "    \"o-\",\n",
+                "    label=\"pyranges\",\n",
                 ")\n",
                 "if include_pybedtools:\n",
                 "    plt.loglog(\n",
                 "        list(timings_pb.keys()),\n",
                 "        list([r.average for r in timings_pb.values()]),\n",
-                "        'o-',\n",
-                "        label='pybedtools'\n",
+                "        \"o-\",\n",
+                "        label=\"pybedtools\",\n",
                 "    )\n",
-                "plt.gca().set(\n",
-                "    xlabel='N intervals',\n",
-                "    ylabel='time, seconds',\n",
-                "    aspect=1.0\n",
-                ")\n",
+                "plt.gca().set(xlabel=\"N intervals\", ylabel=\"time, seconds\", aspect=1.0)\n",
                 "plt.grid()\n",
                 "plt.legend()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -777,56 +774,63 @@
         },
         {
             "cell_type": "code",
             "execution_count": 23,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from memory_profiler import memory_usage\n",
                 "import time\n",
                 "\n",
+                "from memory_profiler import memory_usage\n",
+                "\n",
+                "\n",
                 "def sleep_before_after(func, sleep_sec=0.5):\n",
-                "    \"\"\" \n",
-                "    Wrapper that allows to report background interpreter's memory consumption \n",
+                "    \"\"\"\n",
+                "    Wrapper that allows to report background interpreter's memory consumption\n",
                 "    for the first 5 time intervals (if increment is 0.1 abd sleep_sec=0.5):\n",
-                "    https://github.com/pythonprofilers/memory_profiler#api \n",
+                "    https://github.com/pythonprofilers/memory_profiler#api\n",
                 "    \"\"\"\n",
+                "\n",
                 "    def _f(*args, **kwargs):\n",
                 "        time.sleep(sleep_sec)\n",
                 "        func(*args, **kwargs)\n",
                 "        time.sleep(sleep_sec)\n",
+                "\n",
                 "    return _f\n",
                 "\n",
+                "\n",
                 "mem_usage_bf = {}\n",
                 "mem_usage_pr = {}\n",
                 "if include_pybedtools:\n",
                 "    mem_usage_pb = {}\n",
                 "\n",
                 "for n in [1e2, 1e3, 1e4, 1e5, 1e6, 3e6]:\n",
                 "    df = make_random_intervals(n=n, n_chroms=1)\n",
                 "    df2 = make_random_intervals(n=n, n_chroms=1)\n",
                 "    mem_usage_bf[n] = memory_usage(\n",
-                "        (sleep_before_after(bioframe.overlap), (df, df2), dict( how='inner')), \n",
-                "        backend='psutil_pss', \n",
+                "        (sleep_before_after(bioframe.overlap), (df, df2), dict(how=\"inner\")),\n",
+                "        backend=\"psutil_pss\",\n",
                 "        include_children=True,\n",
-                "        interval=0.1)\n",
+                "        interval=0.1,\n",
+                "    )\n",
                 "    mem_usage_pr[n] = memory_usage(\n",
-                "        (sleep_before_after(pyranges_intersect_dfs), (df, df2), dict()), \n",
-                "        backend='psutil_pss', \n",
+                "        (sleep_before_after(pyranges_intersect_dfs), (df, df2), dict()),\n",
+                "        backend=\"psutil_pss\",\n",
                 "        include_children=True,\n",
-                "        interval=0.1)\n",
+                "        interval=0.1,\n",
+                "    )\n",
                 "    if include_pybedtools:\n",
                 "        bed1 = pybedtools.BedTool.from_dataframe(df)\n",
                 "        bed2 = pybedtools.BedTool.from_dataframe(df2)\n",
                 "        mem_usage_pb[n] = memory_usage(\n",
-                "            (sleep_before_after(pybedtools_intersect_dfs), (bed1, bed2), dict()), \n",
-                "            backend='psutil_pss', \n",
+                "            (sleep_before_after(pybedtools_intersect_dfs), (bed1, bed2), dict()),\n",
+                "            backend=\"psutil_pss\",\n",
                 "            include_children=True,\n",
-                "            interval=0.1)\n",
-                "    "
+                "            interval=0.1,\n",
+                "        )"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 24,
             "metadata": {},
             "outputs": [
@@ -848,44 +852,41 @@
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
-                "# Note that r[4] is the background memory usage of Python interpreter, \n",
-                "# and max(r) is the maximum memory usage (that must be from the bioframe/pyranges functions)\n",
-                "plt.figure(figsize=(8,6))\n",
+                "# Note that r[4] is the background memory usage of Python interpreter,\n",
+                "# and max(r) is the maximum memory usage (that must be from the\n",
+                "# bioframe/pyranges functions)\n",
+                "plt.figure(figsize=(8, 6))\n",
                 "plt.loglog(\n",
                 "    list(mem_usage_bf.keys()),\n",
                 "    list([max(r) - r[4] for r in mem_usage_bf.values()]),\n",
-                "    'o-',\n",
-                "    label='bioframe'\n",
+                "    \"o-\",\n",
+                "    label=\"bioframe\",\n",
                 ")\n",
                 "\n",
                 "plt.loglog(\n",
                 "    list(mem_usage_pr.keys()),\n",
                 "    list([max(r) - r[4] for r in mem_usage_pr.values()]),\n",
-                "    'o-',\n",
-                "    label='pyranges'\n",
+                "    \"o-\",\n",
+                "    label=\"pyranges\",\n",
                 ")\n",
                 "\n",
                 "if include_pybedtools:\n",
                 "    plt.loglog(\n",
                 "        list(mem_usage_pb.keys()),\n",
                 "        list([max(r) - r[4] for r in mem_usage_pb.values()]),\n",
-                "        'o-',\n",
-                "        label='pybedtools'\n",
+                "        \"o-\",\n",
+                "        label=\"pybedtools\",\n",
                 "    )\n",
                 "\n",
-                "plt.gca().set(\n",
-                "    xlabel='N intervals',\n",
-                "    ylabel='Memory usage, Mb',\n",
-                "    aspect=1.0\n",
-                ")\n",
+                "plt.gca().set(xlabel=\"N intervals\", ylabel=\"Memory usage, Mb\", aspect=1.0)\n",
                 "plt.grid()\n",
                 "plt.legend()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 25,
@@ -928,23 +929,23 @@
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
-                "print('Bioframe dtypes:')\n",
+                "print(\"Bioframe dtypes:\")\n",
                 "display(df.dtypes)\n",
                 "print()\n",
                 "\n",
-                "print('Pyranges dtypes:')\n",
+                "print(\"Pyranges dtypes:\")\n",
                 "display(df2pr(df).dtypes)\n",
                 "\n",
                 "if include_pybedtools:\n",
-                "    print('Pybedtools dtypes:')\n",
+                "    print(\"Pybedtools dtypes:\")\n",
                 "    bed1 = pybedtools.BedTool.from_dataframe(df)\n",
                 "    display(bed1.to_dataframe().dtypes)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 26,
@@ -970,92 +971,101 @@
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "### Combined performance figure.\n",
                 "\n",
-                "fig, axs = plt.subplot_mosaic(\n",
-                "    'AAA.BBB',\n",
-                "    figsize=(9.0,4))\n",
-                "\n",
-                "plt.sca(axs['A'])                   \n",
-                "\n",
-                "plt.text(-0.25, 1.0, 'A', horizontalalignment='center',\n",
-                "    verticalalignment='center', transform=plt.gca().transAxes,\n",
-                "        fontsize=19)\n",
+                "fig, axs = plt.subplot_mosaic(\"AAA.BBB\", figsize=(9.0, 4))\n",
+                "\n",
+                "plt.sca(axs[\"A\"])\n",
+                "\n",
+                "plt.text(\n",
+                "    -0.25,\n",
+                "    1.0,\n",
+                "    \"A\",\n",
+                "    horizontalalignment=\"center\",\n",
+                "    verticalalignment=\"center\",\n",
+                "    transform=plt.gca().transAxes,\n",
+                "    fontsize=19,\n",
+                ")\n",
                 "\n",
                 "plt.loglog(\n",
                 "    list(timings_bf.keys()),\n",
                 "    list([r.average for r in timings_bf.values()]),\n",
-                "    'o-',\n",
-                "    color='k',\n",
-                "    label='bioframe'\n",
+                "    \"o-\",\n",
+                "    color=\"k\",\n",
+                "    label=\"bioframe\",\n",
                 ")\n",
                 "plt.loglog(\n",
                 "    list(timings_pr.keys()),\n",
                 "    list([r.average for r in timings_pr.values()]),\n",
-                "    'o-',\n",
-                "    color='gray',\n",
-                "    label='pyranges'\n",
+                "    \"o-\",\n",
+                "    color=\"gray\",\n",
+                "    label=\"pyranges\",\n",
                 ")\n",
                 "if include_pybedtools:\n",
                 "    plt.loglog(\n",
                 "        list(timings_pb.keys()),\n",
                 "        list([r.average for r in timings_pb.values()]),\n",
-                "        'o-',\n",
-                "        color='lightgray',\n",
-                "        label='pybedtools'\n",
-                ")\n",
+                "        \"o-\",\n",
+                "        color=\"lightgray\",\n",
+                "        label=\"pybedtools\",\n",
+                "    )\n",
                 "\n",
                 "plt.gca().set(\n",
-                "    xlabel='N intervals',\n",
-                "    ylabel='time, s',\n",
+                "    xlabel=\"N intervals\",\n",
+                "    ylabel=\"time, s\",\n",
                 "    aspect=1.0,\n",
-                "    xticks=10**np.arange(2,6.1),\n",
-                "    yticks=10**np.arange(-3,0.1),\n",
-                "\n",
+                "    xticks=10 ** np.arange(2, 6.1),\n",
+                "    yticks=10 ** np.arange(-3, 0.1),\n",
                 ")\n",
                 "\n",
                 "plt.grid()\n",
                 "plt.legend()\n",
                 "\n",
-                "plt.sca(axs['B'])\n",
-                "plt.text(-0.33, 1.0, 'B', horizontalalignment='center',\n",
-                "    verticalalignment='center', transform=plt.gca().transAxes,\n",
-                "        fontsize=19)\n",
+                "plt.sca(axs[\"B\"])\n",
+                "plt.text(\n",
+                "    -0.33,\n",
+                "    1.0,\n",
+                "    \"B\",\n",
+                "    horizontalalignment=\"center\",\n",
+                "    verticalalignment=\"center\",\n",
+                "    transform=plt.gca().transAxes,\n",
+                "    fontsize=19,\n",
+                ")\n",
                 "plt.loglog(\n",
                 "    list(mem_usage_bf.keys()),\n",
                 "    list([max(r) - r[4] for r in mem_usage_bf.values()]),\n",
-                "    'o-',\n",
-                "    color='k',\n",
-                "    label='bioframe'\n",
+                "    \"o-\",\n",
+                "    color=\"k\",\n",
+                "    label=\"bioframe\",\n",
                 ")\n",
                 "\n",
                 "plt.loglog(\n",
                 "    list(mem_usage_pr.keys()),\n",
                 "    list([max(r) - r[4] for r in mem_usage_pr.values()]),\n",
-                "    'o-',\n",
-                "    color='gray',\n",
-                "    label='pyranges'\n",
+                "    \"o-\",\n",
+                "    color=\"gray\",\n",
+                "    label=\"pyranges\",\n",
                 ")\n",
                 "if include_pybedtools:\n",
                 "    plt.loglog(\n",
                 "        list(mem_usage_pb.keys()),\n",
                 "        list([max(r) - r[4] for r in mem_usage_pb.values()]),\n",
-                "        'o-',\n",
-                "        color='lightgray',\n",
-                "        label='pybedtools'\n",
+                "        \"o-\",\n",
+                "        color=\"lightgray\",\n",
+                "        label=\"pybedtools\",\n",
                 "    )\n",
                 "\n",
                 "plt.gca().set(\n",
-                "    xlabel='N intervals',\n",
-                "    ylabel='Memory usage, Mb',\n",
+                "    xlabel=\"N intervals\",\n",
+                "    ylabel=\"Memory usage, Mb\",\n",
                 "    aspect=1.0,\n",
-                "    xticks=10**np.arange(2,6.1),\n",
+                "    xticks=10 ** np.arange(2, 6.1),\n",
                 ")\n",
                 "\n",
                 "plt.grid()\n",
                 "plt.legend()"
             ]
         },
         {
@@ -1094,16 +1104,15 @@
                 "timings_slicing_pr = {}\n",
                 "\n",
                 "\n",
                 "for n in [1e2, 1e3, 1e4, 1e5, 1e6, 3e6]:\n",
                 "    df = make_random_intervals(n=n, n_chroms=1)\n",
                 "    timings_slicing_bf[n] = %timeit -o -r 1 bioframe.select(df, ('chr1', n//2, n//4*3))\n",
                 "    pr = df2pr(df)\n",
-                "    timings_slicing_pr[n] = %timeit -o -r 1 pr['chr1', n//2:n//4*3]\n",
-                "    \n"
+                "    timings_slicing_pr[n] = %timeit -o -r 1 pr['chr1', n//2:n//4*3]"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 28,
             "metadata": {},
             "outputs": [
@@ -1128,29 +1137,25 @@
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "plt.loglog(\n",
                 "    list(timings_slicing_bf.keys()),\n",
                 "    list([r.average for r in timings_bf.values()]),\n",
-                "    'o-',\n",
-                "    label='bioframe'\n",
+                "    \"o-\",\n",
+                "    label=\"bioframe\",\n",
                 ")\n",
                 "\n",
                 "plt.loglog(\n",
                 "    list(timings_slicing_pr.keys()),\n",
                 "    list([r.average for r in timings_pr.values()]),\n",
-                "    'o-',\n",
-                "    label='pyranges'\n",
-                ")\n",
-                "plt.gca().set(\n",
-                "    xlabel='N intervals',\n",
-                "    ylabel='time, s',\n",
-                "    aspect=1.0\n",
+                "    \"o-\",\n",
+                "    label=\"pyranges\",\n",
                 ")\n",
+                "plt.gca().set(xlabel=\"N intervals\", ylabel=\"time, s\", aspect=1.0)\n",
                 "plt.grid()\n",
                 "plt.legend()"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
```

### Comparing `bioframe-0.6.4/docs/guide-quickstart.rst` & `bioframe-0.7.0/docs/guide-quickstart.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Quickstart
 ==========
 
 Installation
 ------------
- 
+
 ::
 
     $ pip install bioframe
 
 To install the latest development version of `bioframe` from
 github, first make a local clone of the github repository:
 
 .. code-block:: bash
 
-    $ git clone https://github.com/open2c/bioframe 
+    $ git clone https://github.com/open2c/bioframe
 
-Then, compile and install `bioframe` in 
+Then, compile and install `bioframe` in
 `development mode <https://setuptools.readthedocs.io/en/latest/setuptools.html#development-mode>`_. This installs the package without moving it to a system folder, and thus allows for testing changes to the python code on the fly.
 
 .. code-block:: bash
 
     $ cd bioframe
     $ pip install -e ./
-
-
```

### Comparing `bioframe-0.6.4/docs/guide-recipes.md` & `bioframe-0.7.0/docs/guide-recipes.md`

 * *Files 12% similar despite different names*

```diff
@@ -10,35 +10,35 @@
   display_name: Python 3
   language: python
   name: python3
 ---
 
 # How do I
 
-## Obtain overlapping intervals with matching strandedness? 
+## Obtain overlapping intervals with matching strandedness?
 Use overlap with the ``on`` argument:
 ```
 df = bf.overlap(df1, df2, on=[‘strand’])
 ```
 
-## Obtain overlapping intervals with opposite strandedness? 
+## Obtain overlapping intervals with opposite strandedness?
 Overlap then filter pairs of opposite strandedness:
 ```
 df = bf.overlap(df1, df2)
 df = df.loc[df["strand"]!=df["strand_"]]
 ```
 ## Obtain intervals that exceed 50% coverage by another set of intervals?
 Coverage, then filter pairs by fractional coverage:
 ```
 df = bf.coverage(df1, df2)
 df = df[ ( df["coverage"] / (df["end"]-df["start"]) ) >=0.50]
 ```
 
 ## Shift all intervals on the positive strand by 10bp?
-Use pandas indexing: 
+Use pandas indexing:
 ```
 df.loc[df.strand=="+",["start", "end"]] += 10
 ```
 
 ## Obtain intervals overlapped by at least 2 intervals from another set?
 Count overlaps, then filter:
 ```
@@ -48,22 +48,18 @@
 
 ## Find strand-specific downstream genomic features?
 Use closest after filtering by strand, and passing the `ignore_upsream=True` argument.
 ```
 bioframe.closest(df1.loc[df1['strand']=='+'], df2, ignore_upstream=True)
 ```
 
-For gener, the upstream/downstream direction might be defined by the direction of transcription. 
-Use `direction_col='strand'` to set up the direction: 
+For gener, the upstream/downstream direction might be defined by the direction of transcription.
+Use `direction_col='strand'` to set up the direction:
 ```
 bioframe.closest(df1, df2, ignore_upstream=True, direction_col='strand')
 ```
 
 ## Drop non-autosomes from a bedframe?
 Use pandas DataFrame.isin(values):
 ```
 df[ ~df.chrom.isin(['chrX','chrY'])]
 ```
-
-
-
-
```

### Comparing `bioframe-0.6.4/docs/guide-specifications.rst` & `bioframe-0.7.0/docs/guide-specifications.rst`

 * *Files 3% similar despite different names*

```diff
@@ -5,32 +5,32 @@
 
 BedFrame (i.e. genomic intervals stored in a pandas dataframe):
     - In a BedFrame, three required columns specify the set of genomic intervals (default column names = (‘chrom’, ‘start’, ‘end’)).
     - Other reserved but not required column names: (‘strand’, ‘name’, ‘view_region’).
 
         - entries in column ‘name’ are expected to be unique
         - ‘view_region’ is expected to point to an associated region in a view with a matching name
-        - ‘strand’ is expected to be encoded with strings (‘+’, ‘-’, ‘.’). 
+        - ‘strand’ is expected to be encoded with strings (‘+’, ‘-’, ‘.’).
 
     - Additional columns are allowed: ‘zodiac_sign’, ‘soundcloud’, ‘twitter_name’, etc.
     - Repeated intervals are allowed.
-    - The native pandas DataFrame index is not intended to be used as an immutable lookup table for genomic intervals in BedFrame. This is because many common genomic interval operations change the number of intervals stored in a BedFrame. 
-   - Two useful sorting schemes for BedFrames are: 
+    - The native pandas DataFrame index is not intended to be used as an immutable lookup table for genomic intervals in BedFrame. This is because many common genomic interval operations change the number of intervals stored in a BedFrame.
+   - Two useful sorting schemes for BedFrames are:
 
         - scaffold-sorted: on (chrom, start, end), where chrom is sorted lexicographically.
         - view-sorted: on (view_region, start, end) where view_region is sorted by order in the view.
-        
+
     - Null values are allowed, but only as pd.NA (using np.nan is discouraged as it results in unwanted type re-casting).
    - Note if no ‘view_region’ is assigned to a genomic interval, then ‘chrom’ implicitly defines an associated region
     - Note the BedFrame specification is a natural extension of the BED format ( ​​https://samtools.github.io/hts-specs/BEDv1.pdf ) for pandas DataFrames.
 
 ViewFrames (a genomic view stored in a pandas dataframe)
     - BedFrame where:
-         
+
            - intervals are non-overlapping
-           - “name” column is mandatory and contains a set of unique strings. 
+           - “name” column is mandatory and contains a set of unique strings.
 
     - Note that a ViewFrame can potentially be indexed by the name column to serve as a lookup table. This functionality is currently not implemented, because within the current Pandas implementation indexing by a column removes the column from the table.
-    - Note that views can be defined by: 
-        
+    - Note that views can be defined by:
+
         - dictionary of string:ints (start=0 assumed) or string:tuples (start,end)
         - pandas series of chromsizes (start=0, name=chrom)
```

### Comparing `bioframe-0.6.4/docs/index.rst` & `bioframe-0.7.0/docs/index.rst`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,15 @@
    guide-quickstart
    guide-intervalops.md
    guide-io.ipynb
    guide-performance.ipynb
    guide-recipes.md
    guide-definitions
    guide-specifications
+   guide-bedtools
 
 .. toctree::
    :maxdepth: 1
    :caption: Tutorials
 
    tutorials/tutorial_assign_motifs_to_peaks.ipynb
    tutorials/tutorial_assign_peaks_to_genes.ipynb
```

### Comparing `bioframe-0.6.4/docs/make.bat` & `bioframe-0.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.4/docs/times100.bw` & `bioframe-0.7.0/docs/times100.bw`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.4/docs/figs/._bioframe-logo.png` & `bioframe-0.7.0/docs/figs/._bioframe-logo.png`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.4/docs/figs/bioframe-logo.png` & `bioframe-0.7.0/docs/figs/bioframe-logo.png`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.4/docs/figs/bioframe_closest.pdf` & `bioframe-0.7.0/docs/figs/bioframe_closest.pdf`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.4/docs/figs/closest0.png` & `bioframe-0.7.0/docs/figs/closest0.png`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.4/docs/figs/closest1.png` & `bioframe-0.7.0/docs/figs/closest1.png`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.4/docs/figs/closest2.png` & `bioframe-0.7.0/docs/figs/closest2.png`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.4/docs/figs/closest3.png` & `bioframe-0.7.0/docs/figs/closest3.png`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.4/docs/figs/df1.png` & `bioframe-0.7.0/docs/figs/df1.png`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.4/docs/figs/df2.png` & `bioframe-0.7.0/docs/figs/df2.png`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.4/docs/figs/df@.png` & `bioframe-0.7.0/docs/figs/df@.png`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.4/docs/figs/merge_df1.png` & `bioframe-0.7.0/docs/figs/merge_df1.png`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.4/docs/figs/overlap_inner_0.png` & `bioframe-0.7.0/docs/figs/overlap_inner_0.png`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.4/docs/figs/overlap_inner_1.png` & `bioframe-0.7.0/docs/figs/overlap_inner_1.png`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.4/docs/tutorials/tutorial_assign_motifs_to_peaks.ipynb` & `bioframe-0.7.0/docs/tutorials/tutorial_assign_motifs_to_peaks.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99421388507326%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(0, 'import matplotlib.pyplot as plt\\n'), (2, 'import "*

 * *            "pandas as pd\\n'), (3, '\\n'), (4, 'import bioframe')], delete: [3, 2, 0]}}, 2: "*

 * *            '{\'source\': [\'base_dir = "/tmp/bioframe_tutorial_data/"\\n\', \'assembly = '*

 * *            '"GRCh38"\']}, 4: {\'source\': {insert: [(0, \'ctcf_peaks = '*

 * *            "bioframe.read_table(\\n'), (1, '    "*

 * *            '"https://www.encodeproject.org/files/ENCFF401MQL/@@download/ENCFF401MQL.bed.gz",\\n\'), '*

 * *   […]*

```diff
@@ -11,28 +11,29 @@
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import bioframe\n",
+                "import matplotlib.pyplot as plt\n",
                 "import numpy as np\n",
-                "import pandas as pd \n",
-                "import matplotlib.pyplot as plt"
+                "import pandas as pd\n",
+                "\n",
+                "import bioframe"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [],
             "source": [
-                "base_dir = '/tmp/bioframe_tutorial_data/'\n",
-                "assembly = 'GRCh38'"
+                "base_dir = \"/tmp/bioframe_tutorial_data/\"\n",
+                "assembly = \"GRCh38\""
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Load CTCF ChIP-seq peaks for HFF from ENCODE\n",
@@ -166,15 +167,18 @@
                     },
                     "execution_count": 3,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "ctcf_peaks = bioframe.read_table(\"https://www.encodeproject.org/files/ENCFF401MQL/@@download/ENCFF401MQL.bed.gz\", schema='narrowPeak')\n",
+                "ctcf_peaks = bioframe.read_table(\n",
+                "    \"https://www.encodeproject.org/files/ENCFF401MQL/@@download/ENCFF401MQL.bed.gz\",\n",
+                "    schema=\"narrowPeak\",\n",
+                ")\n",
                 "ctcf_peaks[0:5]"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -272,17 +276,19 @@
                     "execution_count": 4,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "### CTCF motif: http://jaspar.genereg.net/matrix/MA0139.1/\n",
-                "jaspar_url = 'http://expdata.cmmt.ubc.ca/JASPAR/downloads/UCSC_tracks/2022/hg38/'\n",
-                "jaspar_motif_file = 'MA0139.1.tsv.gz'\n",
-                "ctcf_motifs = bioframe.read_table(jaspar_url+jaspar_motif_file,schema='jaspar',skiprows=1)    \n",
+                "jaspar_url = \"http://expdata.cmmt.ubc.ca/JASPAR/downloads/UCSC_tracks/2022/hg38/\"\n",
+                "jaspar_motif_file = \"MA0139.1.tsv.gz\"\n",
+                "ctcf_motifs = bioframe.read_table(\n",
+                "    jaspar_url + jaspar_motif_file, schema=\"jaspar\", skiprows=1\n",
+                ")\n",
                 "ctcf_motifs[0:4]"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -291,15 +297,17 @@
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {},
             "outputs": [],
             "source": [
-                "df_peaks_motifs = bioframe.overlap(ctcf_peaks,ctcf_motifs, suffixes=('_1','_2'), return_index=True)"
+                "df_peaks_motifs = bioframe.overlap(\n",
+                "    ctcf_peaks, ctcf_motifs, suffixes=(\"_1\", \"_2\"), return_index=True\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "There are often multiple motifs overlapping one ChIP-seq peak, and a substantial number of peaks without motifs:"
@@ -315,34 +323,38 @@
                     "output_type": "stream",
                     "text": [
                         "fraction of peaks without motifs 0.14\n"
                     ]
                 },
                 {
                     "data": {
-                        "image/png": "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DBjgdAHdunW765ANI0aM0IgRI5xu+06Sk5OVnJysvLw8l7YLAABKD5txcmCoa9euycfH55bLzp49W+aGX8jJyVFgYKAuXLiggIAAl7Zd0mcf4Hqc0QGA0qmwf7+d7oz8u9/9Tvn5+QXm/+c//1G3bt2cbQ4AAMBtnA46p0+f1tChQx3mnTlzRt26dVOzZs1cVhgAAEBxOR10UlNTtXPnTvvdVqdOnVLXrl3VqlUrvffeey4v0F14jg4AANbndGfkGjVqaMOGDercubMkaf369WrXrp1WrFihChVK9dBZDhITE5WYmGi/xgcAAKynSGNd1atXT2lpaercubN69Oihv//97wWGaQAAAPC0QgWd6tWr3zLIXLp0SWvXrrXfYi5J586dc111AAAAxVCooLNgwQI3lwEAAOB6hQo6Q4YMcXcdJY4HBgIAYH3F6j18+fJl5eTkOLzKCgb1BADA+pwOOhcvXtTIkSNVq1YtVa1aVdWrV3d4AQAAlBZOB50JEybo448/1qJFi+Tr66ulS5dq+vTpCgkJ0ZtvvumOGgEAAIrE6dvL165dqzfffFPdunXTk08+qS5duqhRo0YKDw/XihUrNGjQIHfUCQAA4DSnz+icO3dODRo0kCQFBATYbyfv3Lmztm3b5trqAAAAisHpoNOwYUMdP35ckhQREWEf9mHt2rWqVq2aK2tzK4aAAADA+pwOOv/93/+tL7/8UpI0efJke1+dcePGafz48S4v0F246woAAOtzuo/OzcE8Jal79+765ptvlJ6erl/96leKjIx0aXEAAADFUaSxrm66cuWKwsLCFBYW5qp6AAAAXMbpS1d5eXl68cUXVbduXVWtWlXffvutJOn555/X66+/7vICAQAAisrpoPPSSy9p+fLlmjt3rnx8fOzzW7VqpaVLl7q0OAAAgOJwOui8+eabSklJ0aBBg+Tl5WWf37p1a33zzTcuLQ4AAKA4nA46p06dUqNGjQrMz8/P1/Xr111SVEng9nIAAKzP6aDTokULbd++vcD8999/X23btnVJUSWB28sBALA+p++6mjp1qhISEnTq1Cnl5+dr9erVOnTokN58802tW7fOHTUCAAAUidNndPr06aOVK1cqNTVVNptNL7zwgg4ePKi1a9eqR48e7qgRAACgSIr0HJ1evXqpV69erq4FAADApYr8wMD09HQdPHhQNptNzZs3V1RUlCvrAgAAKDang87Jkyc1YMAAffrpp/ZBPM+fP6+4uDi98847Cg0NdXWNAAAAReJ0H50nn3xS169f18GDB3Xu3DmdO3dOBw8elDFGQ4cOdUeNAAAAReL0GZ3t27drx44datq0qX1e06ZN9eqrr6pTp04uLQ4AAKA4nD6jExYWdssHA964cUN169Z1SVEAAACu4HTQmTt3rkaNGqX09HQZYyT91DF5zJgx+vOf/+zyAt2FJyMDAGB9NnMzrRRS9erVdenSJd24cUPe3j9d+br531WqVHFY99y5c66r1E1ycnIUGBioCxcuKCAgwKVt15+03qXtoeQdn9Pb0yUAAG6hsH+/ne6js2DBguLUBQAAUGKcDjpDhgxxRx0AAAAu53QfHQAAgLKCoAMAACyLoAMAACyrUEFn3759ys/Pd3ctAAAALlWooNO2bVudPXtWktSwYUNlZ2e7tSgAAABXKFTQqVatmo4dOyZJOn78OGd3AABAmVCo28t/+9vfqmvXrqpTp45sNpuio6Pl5eV1y3W//fZblxYIAABQVIUKOikpKerXr5+OHDmi0aNH66mnnpK/v7+7awMAACiWQj8w8IEHHpAkZWRkaMyYMQQdAABQ6jl9e/myZcvsIefkyZM6deqUy4sqCQzqCQCA9TkddPLz8zVjxgwFBgYqPDxcYWFhqlatml588cUy1Uk5MTFRBw4c0K5duzxdCgAAcBOnx7qaMmWKXn/9dc2ZM0edOnWSMUaffvqppk2bpitXruill15yR50AAABOczrovPHGG1q6dKn69u1rnxcZGam6detqxIgRBB0AAFBqOH3p6ty5c2rWrFmB+c2aNdO5c+dcUhQAAIArOB10IiMjtXDhwgLzFy5cqMjISJcUBQAA4ApOX7qaO3euevfurU2bNik2NlY2m007duxQZmamUlNT3VEjAABAkTh9Rqdr1646fPiwHn74YZ0/f17nzp1Tv379dOjQIXXp0sUdNQIAABSJ02d0JCkkJIROxwAAoNRz+owOAABAWUHQAQAAlkXQAQAAluVU0DHG6LvvvtPly5fdVQ8AAIDLOB10GjdurJMnT7qrHgAAAJdxKuhUqFBBjRs3VnZ2trvqAQAAcBmn++jMnTtX48eP19dff+2OegAAAFzG6efoPP7447p06ZIiIyPl4+OjSpUqOSxnvCsAAFBaOB10FixY4IYygNKp/qT1Jbq943N6l+j2AMDqnA46Q4YMcUcdRZaZmamEhARlZWXJ29tbzz//vB599FFPlwUAAEqBIj1H5+jRo3ruuec0YMAAZWVlSZI+/PBD7d+/36XFFYa3t7cWLFigAwcOaNOmTRo3bpwuXrxY4nUAAIDSx+mgs3XrVrVq1UpffPGFVq9erdzcXEnSvn37NHXqVJcXeDd16tRRmzZtJEm1atVSUFAQ/YQAAICkIgSdSZMmaebMmUpLS5OPj499fvfu3fXZZ585XcC2bdvUp08fhYSEyGazac2aNQXWWbRokRo0aCA/Pz9FRUVp+/btt2wrPT1d+fn5Cg0NdboOAABgPU4Hna+++koPP/xwgfn33HNPkZ6vc/HiRUVGRmrhwoW3XL5y5UqNHTtWU6ZM0Z49e9SlSxfFx8frxIkTDutlZ2dr8ODBSklJueP2rl69qpycHIcXAACwJqeDTrVq1XT69OkC8/fs2aO6des6XUB8fLxmzpypfv363XL5/PnzNXToUA0bNkzNmzfXggULFBoaqsWLF9vXuXr1qh5++GFNnjxZcXFxd9ze7NmzFRgYaH9x9gcAAOtyOugMHDhQEydO1JkzZ2Sz2ZSfn69PP/1Uzz77rAYPHuzS4q5du6aMjAz17NnTYX7Pnj21Y8cOST8NS/HEE0/ovvvuU0JCwl3bnDx5si5cuGB/ZWZmurRmAABQejgddF566SWFhYWpbt26ys3NVUREhO69917FxcXpueeec2lxZ8+eVV5enoKDgx3mBwcH68yZM5KkTz/9VCtXrtSaNWvUpk0btWnTRl999dVt2/T19VVAQIDDCwAAWJPTz9GpWLGiVqxYoRkzZmjPnj3Kz89X27Zt1bhxY3fUJ0my2WwO08YY+7zOnTsrPz/f6TaTk5OVnJysvLw8l9QIAABKH6eDzk2/+tWv1LBhQ0kFg4ir1KxZU15eXvazNzdlZWUVOMvjrMTERCUmJionJ0eBgYHFagsAAJRORXpg4Ouvv66WLVvKz89Pfn5+atmypZYuXerq2uTj46OoqCilpaU5zE9LS7trp2MAAACnz+g8//zzevnllzVq1CjFxsZKkj777DONGzdOx48f18yZM51qLzc3V0eOHLFPHzt2THv37lVQUJDCwsKUlJSkhIQERUdHKzY2VikpKTpx4oSGDx/ubOkAAKCccTroLF68WK+99poGDBhgn9e3b1+1bt1ao0aNcjropKenq3v37vbppKQkST+NqbV8+XL1799f2dnZmjFjhk6fPq2WLVsqNTVV4eHhzpbugD46AABYn80YY5x5Q/Xq1bVz584CnY8PHz6s9u3b6/z5866sz+1u9tG5cOGCy+/AKumRr1H2MXo5ABROYf9+O91H5/HHH3d4WN9NKSkpGjRokLPNAQAAuE2hLl3dvJwk/XSH1dKlS7Vx40Z17NhRkvT5558rMzPT5Q8MBAAAKI5CBZ09e/Y4TEdFRUmSjh49Kumnca7uuece7d+/38XlAQAAFF2hgs7mzZvdXUeJozMyAADWV6Tn6FhBYmKiDhw4oF27dnm6FAAA4CZO315+5coVvfrqq9q8ebOysrIKDL+we/dulxUHAABQHE4HnSeffFJpaWl65JFH1L59e7cN/wAAAFBcTged9evXKzU1VZ06dXJHPQAAAC7jdB+dunXryt/f3x21lKjk5GRFREQoJibG06UAAAA3cTrozJs3TxMnTtR3333njnpKDJ2RAQCwPqcvXUVHR+vKlStq2LChKleurIoVKzosP3funMuKAwAAKA6ng86AAQN06tQpzZo1S8HBwXRGBgAApZbTQWfHjh367LPPFBkZ6Y56AAAAXMbpPjrNmjXT5cuX3VELAACASzkddObMmaNnnnlGW7ZsUXZ2tnJychxeZQV3XQEAYH02Y4xx5g0VKvyUjX7ZN8cYI5vNVubGjsrJyVFgYKAuXLiggIAAl7Zdf9J6l7YH6zs+p7enSwCAMqGwf7+d7qNjxQE+AQCANTkddLp27eqOOgAAAFzO6aCzbdu2Oy6/9957i1wMAACAKzkddLp161Zg3s/765S1PjoAAMC6nL7r6ocffnB4ZWVl6cMPP1RMTIw2btzojhoBAACKxOkzOoGBgQXm9ejRQ76+vho3bpwyMjJcUpi7JScnKzk5mTNQAABYmNNndG7nnnvu0aFDh1zVnNsxqCcAANbn9Bmdffv2OUwbY3T69GnNmTOHYSEAAECp4nTQadOmjWw2m375nMGOHTvqb3/7m8sKAwAAKC6ng86xY8ccpitUqKB77rlHfn5+LisKAADAFZwOOuHh4e6oAwAAwOWcDjqS9NFHH+mjjz5SVlaW8vPzHZZx+QoAAJQWTged6dOna8aMGYqOjladOnUKDO4JAABQWjgddJYsWaLly5crISHBHfUAAAC4jNPP0bl27Zri4uLcUUuJSk5OVkREhGJiYjxdCgAAcBOng86wYcP09ttvu6OWEsUDAwEAsD6nL11duXJFKSkp2rRpk1q3bq2KFSs6LJ8/f77LigMAACiOIj0ZuU2bNpKkr7/+2mEZHZMBAEBp4nTQ2bx5szvqAAAAcDmXDeoJAABQ2hB0AACAZRF0AACAZRF0AACAZRF0AACAZRF0AACAZRVp9HIA7lF/0voS3d7xOb1LdHsAUNI4owMAACyLoAMAACyr3AYdRi8HAMD6ym3QYfRyAACsr9wGHQAAYH0EHQAAYFkEHQAAYFkEHQAAYFkEHQAAYFkEHQAAYFkEHQAAYFkEHQAAYFkEHQAAYFkEHQAAYFkEHQAAYFkEHQAAYFkEHQAAYFkEHQAAYFkEHQAAYFmWCDoPP/ywqlevrkceecTTpQAAgFLEEkFn9OjRevPNNz1dBgAAKGUsEXS6d+8uf39/T5cBAABKGY8HnW3btqlPnz4KCQmRzWbTmjVrCqyzaNEiNWjQQH5+foqKitL27dtLvlAAAFDmeDzoXLx4UZGRkVq4cOEtl69cuVJjx47VlClTtGfPHnXp0kXx8fE6ceJEkbZ39epV5eTkOLwAAIA1eTzoxMfHa+bMmerXr98tl8+fP19Dhw7VsGHD1Lx5cy1YsEChoaFavHhxkbY3e/ZsBQYG2l+hoaHFKR8AAJRiHg86d3Lt2jVlZGSoZ8+eDvN79uypHTt2FKnNyZMn68KFC/ZXZmamK0oFAAClkLenC7iTs2fPKi8vT8HBwQ7zg4ODdebMGft0r169tHv3bl28eFH16tXTBx98oJiYmFu26evrK19fX7fWDQAASodSHXRustlsDtPGGId5GzZsKOmSAABAGVCqL13VrFlTXl5eDmdvJCkrK6vAWR5nJScnKyIi4rZnfgAAQNlXqoOOj4+PoqKilJaW5jA/LS1NcXFxxWo7MTFRBw4c0K5du4rVDgAAKL08fukqNzdXR44csU8fO3ZMe/fuVVBQkMLCwpSUlKSEhARFR0crNjZWKSkpOnHihIYPH+7BqgEAQFng8aCTnp6u7t2726eTkpIkSUOGDNHy5cvVv39/ZWdna8aMGTp9+rRatmyp1NRUhYeHe6pkAABQRng86HTr1k3GmDuuM2LECI0YMcKl201OTlZycrLy8vJc2i4AACg9SnUfHXeijw4AANZXboMOAACwPoIOAACwLI/30fEU+ugAUv1J60t0e8fn9C7R7QFAuT2jQx8dAACsr9wGHQAAYH0EHQAAYFkEHQAAYFnlNugwqCcAANZXboMOnZEBALC+cht0AACA9RF0AACAZRF0AACAZRF0AACAZTEEBENAAJbGMBdA+VZuz+hw1xUAANZXboMOAACwPoIOAACwLIIOAACwLIIOAACwLIIOAACwLG4v5/ZyoMSU9K3eAFBuz+hwezkAANZXboMOAACwPoIOAACwLIIOAACwLIIOAACwLIIOAACwLIIOAACwLIIOAACwLIIOAACwLJ6MzJORAQA/U9JP8D4+p3eJbq+8KbdndHgyMgAA1ldugw4AALA+gg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsBvVkUE8AZRgDUAJ3Vm7P6DCoJwAA1ldugw4AALA+gg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsSwSddevWqWnTpmrcuLGWLl3q6XIAAEAp4e3pAorrxo0bSkpK0ubNmxUQEKB27dqpX79+CgoK8nRpAADAw8r8GZ2dO3eqRYsWqlu3rvz9/fXggw9qw4YNni4LAACUAh4POtu2bVOfPn0UEhIim82mNWvWFFhn0aJFatCggfz8/BQVFaXt27fbl33//feqW7eufbpevXo6depUSZQOAABKOY8HnYsXLyoyMlILFy685fKVK1dq7NixmjJlivbs2aMuXbooPj5eJ06ckCQZYwq8x2az3XZ7V69eVU5OjsMLAABYk8f76MTHxys+Pv62y+fPn6+hQ4dq2LBhkqQFCxZow4YNWrx4sWbPnq26des6nME5efKkOnTocNv2Zs+erenTp7tuBwDgZ+pPWu/pEtzK6vvnCVb/TI/P6e3R7Xv8jM6dXLt2TRkZGerZs6fD/J49e2rHjh2SpPbt2+vrr7/WqVOn9OOPPyo1NVW9evW6bZuTJ0/WhQsX7K/MzEy37gMAAPAcj5/RuZOzZ88qLy9PwcHBDvODg4N15swZSZK3t7fmzZun7t27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FAAAQMmjjw4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsgg5QDN26ddPYsWM9XYadMUZPP/20goKCZLPZtHfvXk+X5GD58uWqVq1aiW/3+PHjpfLzKK5ffv8uXbqk3/72twoICJDNZtP58+c9VltpUr9+fS1YsMDTZcBDGOsKsJAPP/xQy5cv15YtW9SwYUPVrFnT0yWVCqGhoTp9+nSZ/Ty2bNmi7t2764cffnAIiqtXr1bFihXt02+88Ya2b9+uHTt2qGbNmgoMDPRAtUDpQtABSpm8vDzZbLYCI3AXxtGjR1WnTp1SOWr19evXPbZtLy8v1a5d22Pbd5egoCCH6aNHj6p58+albgDa69evOwQyoCRx6QplXrdu3TR69GhNmDBBQUFBql27tqZNm2ZffqvLFufPn5fNZrOPnLtlyxbZbDZt2LBBbdu2VaVKlXTfffcpKytL//rXv9S8eXMFBARowIABunTpksP2b9y4oZEjR6patWqqUaOGnnvuOf18CLlr165pwoQJqlu3rqpUqaIOHTo4jNh783LOunXrFBERIV9fX3333Xe33NetW7eqffv28vX1VZ06dTRp0iTduHFDkvTEE09o1KhROnHihGw2m+rXr3/bz2zVqlVq0aKFfH19Vb9+fc2bN8++bPLkyerYsWOB97Ru3VpTp061Ty9btkzNmzeXn5+fmjVrpkWLFhX4zN977z1169ZNfn5+euuttwq0efToUf3mN79RcHCwqlatqpiYGG3atMlhnfr16+vFF1/UwIEDVbVqVYWEhOjVV191WMdms2nx4sWKj49XpUqV1KBBA73//vsF6rn5Hbh5vD/66CNFR0ercuXKiouL06FDhxzanTlzpmrVqiV/f38NGzZMkyZNUps2bW77uRb1e3T16lWNHj1atWrVkp+fnzp37qxdu3bZa+/evbskqXr16rLZbHriiSckOV666tatm+bNm6dt27bJZrOpW7dukqRFixapcePG8vPzU3BwsB555JHb1n/zu7hmzRo1adJEfn5+6tGjhzIzMx3WW7t2raKiouTn56eGDRtq+vTp9u/hzeOxZMkS/eY3v1GVKlU0c+bMW26vMMf2woULevrpp1WrVi0FBATovvvu05dffmlfXpjv0C8tW7ZMgYGBSktLu+N6sIgSGToUcKOu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h2vo0KFOh7Z27drpvffe07vvvquWLVvqhRde0IwZM+y3LN/06KOPKjs7W5cuXdJDDz3ksGzYsGFaunSpli9frlatWqlr165avny5GjRo4FQtL7/8sqpXr664uDj16dNHvXr1Urt27Qqs98wzzygjI0Nt27bViy++qHnz5qlXr14O60yfPl3vvvuuWrdurTfeeEMrVqxQRESEU/X83KBBgzR58mQ9++yzateunY4dO6YnnnjC4fKMq8yZM0e//e1vlZCQoHbt2unIkSPasGGDqlevLumnYz99+nRNmjRJwcHBGjlyZKHarVatmlavXq377rtPzZs315IlS/TOO++oRYsWt31P5cqVNXHiRA0cOFCxsbGqVKmS3n33XfvyXr16ad26dUpLS1NMTIw6duyo+fPnKzw8vEj7fqdja7PZlJqaqnvvvVdPPvmkmjRposcee0zHjx+3n2Es7Hfopk6dOmn9+vV6/vnn9corrxSpZpQtNlPYi84A4AH169fX2LFj7zjUhs1m0wcffFAgkLlajx49VLt2bf39739363Y8Zfny5Ro7dmyJDR1RmGMLFBeXrgDgFi5duqQlS5bY+3S888472rRpEw+ZA8oYgg4A3MLNyyYzZ87U1atX1bRpU61atUr333+/p0sD4AQuXQEAAMuiMzIAALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALCs/wM2yc43oc2ldQAAAABJRU5ErkJggg==\n",
+                        "image/png": "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DBjgdAHdunW765ANI0aM0IgRI5xu+06Sk5OVnJysvLw8l7YLAABKD5txcmCoa9euycfH55bLzp49W+aGX8jJyVFgYKAuXLiggIAAl7Zd0mcf4Hqc0QGA0qmwf7+d7oz8u9/9Tvn5+QXm/+c//1G3bt2cbQ4AAMBtnA46p0+f1tChQx3mnTlzRt26dVOzZs1cVhgAAEBxOR10UlNTtXPnTvvdVqdOnVLXrl3VqlUrvffeey4v0F14jg4AANbndGfkGjVqaMOGDercubMkaf369WrXrp1WrFihChVK9dBZDhITE5WYmGi/xgcAAKynSGNd1atXT2lpaercubN69Oihv//97wWGaQAAAPC0QgWd6tWr3zLIXLp0SWvXrrXfYi5J586dc111AAAAxVCooLNgwQI3lwEAAOB6hQo6Q4YMcXcdJY4HBgIAYH3F6j18+fJl5eTkOLzKCgb1BADA+pwOOhcvXtTIkSNVq1YtVa1aVdWrV3d4AQAAlBZOB50JEybo448/1qJFi+Tr66ulS5dq+vTpCgkJ0ZtvvumOGgEAAIrE6dvL165dqzfffFPdunXTk08+qS5duqhRo0YKDw/XihUrNGjQIHfUCQAA4DSnz+icO3dODRo0kCQFBATYbyfv3Lmztm3b5trqAAAAisHpoNOwYUMdP35ckhQREWEf9mHt2rWqVq2aK2tzK4aAAADA+pwOOv/93/+tL7/8UpI0efJke1+dcePGafz48S4v0F246woAAOtzuo/OzcE8Jal79+765ptvlJ6erl/96leKjIx0aXEAAADFUaSxrm66cuWKwsLCFBYW5qp6AAAAXMbpS1d5eXl68cUXVbduXVWtWlXffvutJOn555/X66+/7vICAQAAisrpoPPSSy9p+fLlmjt3rnx8fOzzW7VqpaVLl7q0OAAAgOJwOui8+eabSklJ0aBBg+Tl5WWf37p1a33zzTcuLQ4AAKA4nA46p06dUqNGjQrMz8/P1/Xr111SVEng9nIAAKzP6aDTokULbd++vcD8999/X23btnVJUSWB28sBALA+p++6mjp1qhISEnTq1Cnl5+dr9erVOnTokN58802tW7fOHTUCAAAUidNndPr06aOVK1cqNTVVNptNL7zwgg4ePKi1a9eqR48e7qgRAACgSIr0HJ1evXqpV69erq4FAADApYr8wMD09HQdPHhQNptN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crLy8vJc2i4AACg9SnUfHXeijw4AANZXboMOAACwPoIOAACwLI/30fEU+ugAUv1J60t0e8fn9C7R7QFAuT2jQx8dAACsr9wGHQAAYH0EHQAAYFkEHQAAYFnlNugwqCcAANZXboMOnZEBALC+cht0AACA9RF0AACAZRF0AACAZRF0AACAZTEEBENAAJbGMBdA+VZuz+hw1xUAANZXboMOAACwPoIOAACwLIIOAACwLIIOAACwLIIOAACwLG4v5/ZyoMSU9K3eAFBuz+hwezkAANZXboMOAACwPoIOAACwLIIOAACwLIIOAACwLIIOAACwLIIOAACwLIIOAACwLIIOAACwLJ6MzJORAQA/U9JP8D4+p3eJbq+8KbdndHgyMgAA1ldugw4AALA+gg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsBvVkUE8AZRgDUAJ3Vm7P6DCoJwAA1ldugw4AALA+gg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsSwSddevWqWnTpmrcuLGWLl3q6XIAAEAp4e3pAorrxo0bSkpK0ubNmxUQEKB27dqpX79+CgoK8nRpAADAw8r8GZ2dO3eqRYsWqlu3rvz9/fXggw9qw4YNni4LAACUAh4POtu2bVOfPn0UEhIim82mNWvWFFhn0aJFatCggfz8/BQVFaXt27fbl33//feqW7eufbpevXo6depUSZQOAABKOY8HnYsXLyoyMlILFy685fKVK1dq7NixmjJlivbs2aMuXbooPj5eJ06ckCQZYwq8x2az3XZ7V69eVU5OjsMLAABYk8f76MTHxys+Pv62y+fPn6+hQ4dq2LBhkqQFCxZow4YNWrx4sWbPnq26des6nME5efKkOnTocNv2Zs+erenTp7tuBwDgZ+pPWu/pEtzK6vvnCVb/TI/P6e3R7Xv8jM6dXLt2TRkZGerZs6fD/J49e2rHjh2SpPbt2+vrr7/WqVOn9OOPPyo1NVW9evW6bZuTJ0/WhQsX7K/MzEy37gMAAPAcj5/RuZOzZ88qLy9PwcHBDvODg4N15swZSZK3t7fmzZun7t27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FAAAQMmjjw4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsgg5QDN26ddPYsWM9XYadMUZPP/20goKCZLPZtHfvXk+X5GD58uWqVq1aiW/3+PHjpfLzKK5ffv8uXbqk3/72twoICJDNZtP58+c9VltpUr9+fS1YsMDTZcBDGOsKsJAPP/xQy5cv15YtW9SwYUPVrFnT0yWVCqGhoTp9+nSZ/Ty2bNmi7t2764cffnAIiqtXr1bFihXt02+88Ya2b9+uHTt2qGbNmgoMDPRAtUDpQtABSpm8vDzZbLYCI3AXxtGjR1WnTp1SOWr19evXPbZtLy8v1a5d22Pbd5egoCCH6aNHj6p58+albgDa69evOwQyoCRx6QplXrdu3TR69GhNmDBBQUFBql27tqZNm2ZffqvLFufPn5fNZrOPnLtlyxbZbDZt2LBBbdu2VaVKlXTfffcpKytL//rXv9S8eXMFBARowIABunTpksP2b9y4oZEjR6patWqqUaOGnnvuOf18CLlr165pwoQJqlu3rqpUqaIOHTo4jNh783LOunXrFBERIV9fX3333Xe33NetW7eqffv28vX1VZ06dTRp0iTduHFDkvTEE09o1KhROnHihGw2m+rXr3/bz2zVqlVq0aKFfH19Vb9+fc2bN8++bPLkyerYsWOB97Ru3VpTp061Ty9btkzNmzeXn5+fmjVrpkWLFhX4zN977z1169ZNfn5+euuttwq0efToUf3mN79RcHCwqlatqpiYGG3atMlhnfr16+vFF1/UwIEDVbVqVYWEhOjVV191WMdms2nx4sWKj49XpUqV1KBBA73//vsF6rn5Hbh5vD/66CNFR0ercuXKiouL06FDhxzanTlzpmrVqiV/f38NGzZMkyZNUps2bW77uRb1e3T16lWNHj1atWrVkp+fnzp37qxdu3bZa+/evbskqXr16rLZbHriiSckOV666tatm+bNm6dt27bJZrOpW7dukqRFixapcePG8vPzU3BwsB555JHb1n/zu7hmzRo1adJEfn5+6tGjhzIzMx3WW7t2raKiouTn56eGDRtq+vTp9u/hzeOxZMkS/eY3v1GVKlU0c+bMW26vMMf2woULevrpp1WrVi0FBATovvvu05dffmlfXpjv0C8tW7ZMgYGBSktLu+N6sIgSGToUcKOu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h2vo0KFOh7Z27drpvffe07vvvquWLVvqhRde0IwZM+y3LN/06KOPKjs7W5cuXdJDDz3ksGzYsGFaunSpli9frlatWqlr165avny5GjRo4FQtL7/8sqpXr664uDj16dNHvXr1Urt27Qqs98wzzygjI0Nt27bViy++qHnz5qlXr14O60yfPl3vvvuuWrdurTfeeEMrVqxQRESEU/X83KBBgzR58mQ9++yzateunY4dO6YnnnjC4fKMq8yZM0e//e1vlZCQoHbt2unIkSPasGGDqlevLumnYz99+nRNmjRJwcHBGjlyZKHarVatmlavXq377rtPzZs315IlS/TOO++oRYsWt31P5cqVNXHiRA0cOFCxsbGqVKmS3n33XfvyXr16ad26dUpLS1NMTIw6duyo+fPnKzw8vEj7fqdja7PZlJqaqnvvvVdPPvmkmjRposcee0zHjx+3n2Es7Hfopk6dOmn9+vV6/vnn9corrxSpZpQtNlPYi84A4AH169fX2LFj7zjUhs1m0wcffFAgkLlajx49VLt2bf39739363Y8Zfny5Ro7dmyJDR1RmGMLFBeXrgDgFi5duqQlS5bY+3S888472rRpEw+ZA8oYgg4A3MLNyyYzZ87U1atX1bRpU61atUr333+/p0sD4AQuXQEAAMuiMzIAALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALAsgg4AALCs/wM2yc43oc2ldQAAAABJRU5ErkJggg==",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
-                "# note that counting motifs per peak can also be handled directly with bioframe.count_overlaps\n",
-                "# but since we re-use df_peaks_motifs below we instead use the pandas operations directly\n",
+                "# note that counting motifs per peak can also be handled directly with\n",
+                "# bioframe.count_overlaps but since we re-use df_peaks_motifs below we\n",
+                "# instead use the pandas operations directly\n",
                 "motifs_per_peak = df_peaks_motifs.groupby([\"index_1\"])[\"index_2\"].count().values\n",
                 "\n",
-                "plt.hist(motifs_per_peak,np.arange(0,np.max(motifs_per_peak)))\n",
-                "plt.xlabel('number of overlapping motifs per peak')\n",
-                "plt.ylabel('number of peaks')\n",
-                "plt.semilogy();\n",
+                "plt.hist(motifs_per_peak, np.arange(0, np.max(motifs_per_peak)))\n",
+                "plt.xlabel(\"number of overlapping motifs per peak\")\n",
+                "plt.ylabel(\"number of peaks\")\n",
+                "plt.semilogy()\n",
                 "\n",
-                "print(f'fraction of peaks without motifs {np.round(np.sum(motifs_per_peak==0)/len(motifs_per_peak),2)}')"
+                "print(\n",
+                "    f\"fraction of peaks without motifs \"\n",
+                "    f\"{np.round(np.sum(motifs_per_peak==0)/len(motifs_per_peak), 2)}\"\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Assign the strongest motif to each peak"
@@ -351,18 +363,20 @@
         {
             "cell_type": "code",
             "execution_count": 7,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# since idxmax does not currently take NA, fill with -1\n",
-                "df_peaks_motifs['pval_2'] = df_peaks_motifs['pval_2'].fillna(-1) \n",
-                "idxmax_peaks_motifs = df_peaks_motifs.groupby([\"chrom_1\", \"start_1\",\"end_1\"])[\"pval_2\"].idxmax().values\n",
+                "df_peaks_motifs[\"pval_2\"] = df_peaks_motifs[\"pval_2\"].fillna(-1)\n",
+                "idxmax_peaks_motifs = (\n",
+                "    df_peaks_motifs.groupby([\"chrom_1\", \"start_1\", \"end_1\"])[\"pval_2\"].idxmax().values\n",
+                ")\n",
                 "df_peaks_maxmotif = df_peaks_motifs.loc[idxmax_peaks_motifs]\n",
-                "df_peaks_maxmotif['pval_2'].replace(-1,np.nan,inplace=True)"
+                "df_peaks_maxmotif[\"pval_2\"].replace(-1, np.nan, inplace=True)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "stronger peaks tend to have stronger motifs:"
@@ -371,31 +385,39 @@
         {
             "cell_type": "code",
             "execution_count": 8,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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\n",
+                        "image/png": "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",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
-                "plt.rcParams['font.size']=12\n",
-                "df_peaks_maxmotif['fc_1']  = df_peaks_maxmotif['fc_1'].values.astype('float')\n",
-                "plt.scatter(df_peaks_maxmotif['fc_1'].values, \n",
-                "            df_peaks_maxmotif['pval_2'].values, 5, alpha=0.5,lw=0)\n",
-                "plt.xlabel('ENCODE CTCF peak strength, fc')\n",
-                "plt.ylabel('JASPAR CTCF motif strength \\n (-log10 pval *100)')\n",
-                "plt.title('corr: '+str(np.round(df_peaks_maxmotif['fc_1'].corr(df_peaks_maxmotif['pval_2']),2)));"
+                "plt.rcParams[\"font.size\"] = 12\n",
+                "df_peaks_maxmotif[\"fc_1\"] = df_peaks_maxmotif[\"fc_1\"].values.astype(\"float\")\n",
+                "plt.scatter(\n",
+                "    df_peaks_maxmotif[\"fc_1\"].values,\n",
+                "    df_peaks_maxmotif[\"pval_2\"].values,\n",
+                "    5,\n",
+                "    alpha=0.5,\n",
+                "    lw=0,\n",
+                ")\n",
+                "plt.xlabel(\"ENCODE CTCF peak strength, fc\")\n",
+                "plt.ylabel(\"JASPAR CTCF motif strength \\n (-log10 pval *100)\")\n",
+                "plt.title(\n",
+                "    \"corr: \"\n",
+                "    + str(np.round(df_peaks_maxmotif[\"fc_1\"].corr(df_peaks_maxmotif[\"pval_2\"]), 2))\n",
+                ");"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We can also ask the reverse question: how many motifs overlap a ChIP-seq peak?"
@@ -403,39 +425,43 @@
         },
         {
             "cell_type": "code",
             "execution_count": 9,
             "metadata": {},
             "outputs": [],
             "source": [
-                "df_motifs_peaks = bioframe.overlap(ctcf_motifs,ctcf_peaks,how='left', suffixes=('_1','_2'))"
+                "df_motifs_peaks = bioframe.overlap(\n",
+                "    ctcf_motifs, ctcf_peaks, how=\"left\", suffixes=(\"_1\", \"_2\")\n",
+                ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 10,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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\n",
+                        "image/png": "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",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
-                "m = df_motifs_peaks.sort_values('pval_1')\n",
-                "plt.plot( m['pval_1'].values[::-1] ,\n",
-                "    np.cumsum(pd.isnull(m['chrom_2'].values[::-1])==0)/np.arange(1,len(m)+1))\n",
-                "plt.xlabel('pval')\n",
-                "plt.ylabel('probability motif overlaps a peak');\n"
+                "m = df_motifs_peaks.sort_values(\"pval_1\")\n",
+                "plt.plot(\n",
+                "    m[\"pval_1\"].values[::-1],\n",
+                "    np.cumsum(pd.isnull(m[\"chrom_2\"].values[::-1]) == 0) / np.arange(1, len(m) + 1),\n",
+                ")\n",
+                "plt.xlabel(\"pval\")\n",
+                "plt.ylabel(\"probability motif overlaps a peak\");"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### filter peaks overlapping blacklisted regions\n",
@@ -506,16 +532,18 @@
                     },
                     "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "blacklist = bioframe.read_table('https://www.encodeproject.org/files/ENCFF356LFX/@@download/ENCFF356LFX.bed.gz',\n",
-                "                                schema='bed3')\n",
+                "blacklist = bioframe.read_table(\n",
+                "    \"https://www.encodeproject.org/files/ENCFF356LFX/@@download/ENCFF356LFX.bed.gz\",\n",
+                "    schema=\"bed3\",\n",
+                ")\n",
                 "blacklist[0:3]"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -525,26 +553,29 @@
         {
             "cell_type": "code",
             "execution_count": 12,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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AgBkJ0AAgOwECACQnQABALITIABAdgIEAMhOgAAA2QkQACA7AQIAZCdAAIDsBAgAkJ0AAQCyEyAAQHYCBADIToAAANkJEAAgOwECAGQnQACA7AQIAJCdAAEAshMgAEB2AgQAyE6AAADZCRAAIDsBAgBkJ0AAgOwECACQXVEB8rOf/SzOOOOMGDlyZPTp0yeGDBkSJ510UqxZs6ar5gcAlKHKYgbv3r07RowYEV/60pfi6KOPjr1798batWvjK1/5Smzbti2uvfbarponAFBGigqQqVOnxtSpU1ttmz17drzyyiuxatUqAQIAHJCSvAdk2LBhUVlZVMsAAD1Yh6qhubk5mpub4+23345169bFww8/HP/4j/+43/FNTU3R1NTUcr6hoaEjuwUAykSHAuTSSy+N7373uxER0bt37/iHf/iHuPjii/c7ftmyZVFbW9uxGfYQxy5a32bbtuVndMNMSq+7j+1A9p9zjge6r4+OK5fHQ3t60rF+VO5/HwfbWnfl8bd32121L4rXoZdgrr766vjJT34S69evjwsuuCAuu+yy+Na3vrXf8TU1NVFfX99yqqur6/CEAYBDX4eeARk5cmSMHDkyIiJmzZoVEb+KjHPPPTeGDx/eZnyhUIhCodCJaQIA5aQkb0KdPHlyfPDBB/Hyyy+X4uYAgDJXkgDZsmVL9OrVK37nd36nFDcHAJS5ol6Cueiii2LAgAExefLkOPLII2Pnzp2xbt26uOeee+KKK65o9+UXAICPKipATjrppPjnf/7n+P73vx+7d++O/v37x6c//em444474k//9E+7ao4AQJkpKkDOP//8OP/887tqLgBAD+HbcAGA7AQIAJCdAAEAshMgAEB2AgQAyE6AAADZCRAAIDsBAgBkJ0AAgOwECACQnQABALITIABAdgIEAMhOgAAA2QkQACA7AQIAZCdAAIDsBAgAkJ0AAQCyEyAAQHYCBADIToAAANkJEAAgOwECAGQnQACA7AQIAJCdAAEAshMgAEB2AgQAyE6AAADZCRAAIDsBAgBkJ0AAgOwECACQnQABALITIABAdgIEAMiuqADZvHlzXHDBBTFmzJjo169fHH300TF37tz46U9/2lXzAwDKUFEBcsstt8S2bdvi8ssvjw0bNsRNN90UO3bsiClTpsTmzZu7ao4AQJmpLGbwt7/97TjiiCNabTvttNPi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PvromDt3bvz0pz9tM/bpp5+OU089Nfr37x+DBg2Kz3/+8/Hyyy+3e7s333xzjBkzJgqFQnzyk5+M2traeP/999uM27FjR5x33nkxbNiw6Nu3b5x00kmxadOmkh/nwerWW2+NioqK6N+/f5vLrHfnPf744zFr1qwYPHhw9OnTJ0aNGhXXX399qzHWufOeeeaZOPPMM6O6ujr69u0bY8aMieuuuy7eeaf1x4Nb6+Ls2bMnrrzyypgxY0YMHz48KioqYsmSJe2O7e61ffTRR+Okk06Kvn37xrBhw+K8886LHTt2FHfAnf4s1YPE9OnT06BBg9J3vvOdtHnz5nThhRemiEhr167t7qkdVP74j/84TZs2La1cuTJt3bo1rVu3Lk2ZMiVVVlamTZs2tYx74YUX0uGHH55+//d/P61fvz7dd999ady4cam6ujrt2LGj1W3ecMMNqaKiItXU1KQtW7akv/3bv029e/dOX/va11qN27dvXxo/fnw65phj0po1a9IjjzyS5s6dmyorK9PWrVuzHH93eu2119LAgQNTdXV16tevX6vLrHfnrV27NvXq1Sudc8456T/+4z/S5s2b0z/90z+l2traljHWufOef/75VFVVlT796U+ne+65J23atCktXrw4HXbYYemP/uiPWsZZ6+K98soraeDAgenkk09u+R22ePHiNuO6e223bt2aKisr09y5c9MjjzyS1qxZk44++ug0fvz4tG/fvgM+3rIIkPXr16eISHfeeWer7dOnT0/V1dXpgw8+6KaZHXzeeOONNtv27NmTjjzyyHTKKae0bJs3b14aNmxYqq+vb9m2bdu29Fu/9VvpyiuvbNm2c+fOVFVVlS666KJWt7l06dJUUVGRnn/++ZZt3/72t1NEpP/6r/9q2fb++++nsWPHpsmTJ5fk+A5ms2fPTnPmzEnnnntumwCx3p3z2muvpX79+qX58+d/7Djr3HnXXHNNioj04osvttp+0UUXpYhIu3btSilZ645obm5Ozc3NKaWU3nzzzf0GSHev7YknnpjGjh2b3n///ZZtP/rRj1JEpJUrVx7w8ZZFgFx44YWpf//+rRYjpZTuvPPOFBHpRz/6UTfN7NAxbdq0NHr06JTSrx50ffr0SRdffHGbcTNmzEijRo1qOb9mzZoUEemJJ55oNe7DLyhcunRpy7ZTTz01nXDCCW1u88Ybb0wRkV577bVSHc5B54477kiHH354qquraxMg1rvzlixZkiIibdu2bb9jrHNpfLjWb775ZqvtV155ZerVq1dqbGy01iWwvwDp7rV97bXXUkSkZcuWtRk7evToNH369AM+xrJ4D8hzzz0Xn/rUp6KysvXnqk2cOLHlcvavvr4+nn766Rg3blxERLz00kvx7rvvtqzfr5s4cWK8+OKLsW/fvoj4v7WdMGFCq3G//du/HcOGDWu19s8999x+bzMi4vnnny/NAR1kduzYEQsXLozly5fHMccc0+Zy6915P/zhD2PIkCHxi1/8IiZNmhSVlZVxxBFHxCWXXNLy9eHWuTTOPffcGDRoUMyfPz9efvnl2LNnT/zgBz+I7373u7FgwYLo16+fte5C3b22H15nf2OL+X1bFgHy1ltvtftFeB9ua+8L9Pg/CxYsiL1798Y111wTEf+3Xvtb05RSvP322y1jC4VC9OvXr92xv772PfV+uvTSS+OEE06I+fPnt3u59e68119/Pd55552YN29enH322fHoo4/GFVdcEbfffnvMmjUrUkrWuUSOPfbYeOKJJ+K5556L4447LgYMGBBz5syJc889N2666aaI8JjuSt29tr9p/8XcB0V9FPvBrKKiokOX9XTf+MY3Yu3atXHzzTfHZz7zmVaXHeiaFrP2Pe1+uu++++KBBx6IZ5555jcen/XuuObm5ti3b18sXrw4Fi1aFBERU6dOjd69e8fChQtj06ZN0bdv34iwzp21bdu2mDNnThx55JFx7733xvDhw+PHP/5x3HDDDdHY2BirV69uGWutu053r+3+xhZzH5TFMyBDhw5tt7p27doVEe2XGhG1tbVxww03xNKlS+Oyyy5r2T506NCIaP//Jnbt2hUVFRUxaNCglrH79u1r8+d3H4799bXvafdTY2NjLFiwIL7+9a9HdXV17N69O3bv3h3vvfdeRETs3r079u7da71L4MM1nDlzZqvtp59+ekT86k8WrXNpLFq0KBoaGuLhhx+OL3zhC3HyySfHFVdcEX//938f3/ve9+Kxxx6z1l2ou9f2N+2/mPugLAJkwoQJ8cILL8QHH3zQavuzzz4bERHjx4/vjmkd1Gpra2PJkiWxZMmSuPrqq1tddtxxx0WfPn1a1u/XPfvss3H88cdHVVVVRPzfa4sfHfvLX/4ydu7c2WrtJ0yYsN/bjCi/+2nnzp3xxhtvxIoVK2Lw4MEtp7vuuiv27t0bgwcPjj/5kz+x3iXQ3uvRERHp/3/TRK9evaxzifzsZz+LsWPHtnla/8QTT4yIaHlpxlp3je5e2w//u7+xRd0HB/x21YPYhg0bUkSku+++u9X20047zZ/htuO6665LEZGuvfba/Y754he/mI444ojU0NDQsu3VV19NvXv3TldddVXLtrfeeitVVVWlSy65pNX1ly1b1ubPvFauXJkiIj355JMt295///00bty49NnPfrYUh3ZQeffdd9OWLVvanGbOnJmqqqrSli1b0rPPPptSst6d9fDDD7d5V39KKf3d3/1dioj0n//5nykl61wK06ZNS8OHD0979uxptX3VqlUpItL999+fUrLWnfVxf4bb3Ws7efLkNH78+Fa/W5944okUEemWW2454GMsiwBJ6Vef+TF48OC0atWqtHnz5vS1r30tRURas2ZNd0/toPKtb30rRUQ67bTT0hNPPNHm9KEXXngh9e/fP5188slpw4YN6V//9V/T+PHjP/aDbq6++uq0devW9M1vfjMVCoV2P+hm3LhxacSIEWnt2rVp48aN6ayzziqbDxE6UO19Doj17rw5c+akQqGQrr/++rRx48a0bNmyVFVVlWbPnt0yxjp33r//+7+nioqKNGXKlJYPIlu6dGnq379/Gjt2bGpqakopWeuO2rBhQ1q3bl363ve+lyIizZs3L61bty6tW7cu7d27N6XU/Wu7ZcuWVFlZmc4666y0cePGtHbt2jRixIie+UFkKf3qw7T+/M//PB111FGpd+/eaeLEiemuu+7q7mkddP7gD/4gRcR+T7/uqaeeSqecckrq27dvGjBgQDrzzDPbfPjQh2666aY0evTo1Lt37zRy5Mi0ePHi9N5777UZ98tf/jJ99atfTUOGDElVVVVpypQpaePGjV1yrAer9gIkJevdWe+880666qqr0ogRI1JlZWUaOXJkqqmpafMD0Tp33ubNm9OMGTPSUUcdlfr06ZNGjx6d/uqv/irt3Lmz1ThrXbxPfOIT+/35/Morr7SM6+61feSRR9KUKVNSVVVVGjJkSPrqV7/a7gddfpyKlP7/i6QAAJmUxZtQAYBDiwABALITIABAdgIEAMhOgAAA2QkQACA7AQIAZCdAAIDsBAgAkJ0AAQCyEyAAQHYCBADI7v8B5af2nsavP4AAAAAASUVORK5CYII=\n",
+                        "image/png": "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AgBkJ0AAgOwECACQnQABALITIABAdgIEAMhOgAAA2QkQACA7AQIAZCdAAIDsBAgAkJ0AAQCyEyAAQHYCBADIToAAANkJEAAgOwECAGQnQACA7AQIAJCdAAEAshMgAEB2AgQAyE6AAADZCRAAIDsBAgBkJ0AAgOwECACQXVEB8rOf/SzOOOOMGDlyZPTp0yeGDBkSJ510UqxZs6ar5gcAlKHKYgbv3r07RowYEV/60pfi6KOPjr1798batWvjK1/5Smzbti2uvfbarponAFBGigqQqVOnxtSpU1ttmz17drzyyiuxatUqAQIAHJCSvAdk2LBhUVlZVMsAAD1Yh6qhubk5mpub4+23345169bFww8/HP/4j/+43/FNTU3R1NTUcr6hoaEjuwUAykSHAuTSSy+N7373uxER0bt37/iHf/iHuPjii/c7ftmyZVFbW9uxGfYQxy5a32bbtuVndMNMSq+7j+1A9p9zjge6r4+OK5fHQ3t60rF+VO5/HwfbWnfl8bd32121L4rXoZdgrr766vjJT34S69evjwsuuCAuu+yy+Na3vrXf8TU1NVFfX99yqqur6/CEAYBDX4eeARk5cmSMHDkyIiJmzZoVEb+KjHPPPTeGDx/eZnyhUIhCodCJaQIA5aQkb0KdPHlyfPDBB/Hyyy+X4uYAgDJXkgDZsmVL9OrVK37nd36nFDcHAJS5ol6Cueiii2LAgAExefLkOPLII2Pnzp2xbt26uOeee+KKK65o9+UXAICPKipATjrppPjnf/7n+P73vx+7d++O/v37x6c//em444474k//9E+7ao4AQJkpKkDOP//8OP/887tqLgBAD+HbcAGA7AQIAJCdAAEAshMgAEB2AgQAyE6AAADZCRAAIDsBAgBkJ0AAgOwECACQnQABALITIABAdgIEAMhOgAAA2QkQACA7AQIAZCdAAIDsBAgAkJ0AAQCyEyAAQHYCBADIToAAANkJEAAgOwECAGQnQACA7AQIAJCdAAEAshMgAEB2AgQAyE6AAADZCRAAIDsBAgBkJ0AAgOwECACQnQABALITIABAdgIEAMiuqADZvHlzXHDBBTFmzJjo169fHH300TF37tz46U9/2lXzAwDKUFEBcsstt8S2bdvi8ssvjw0bNsRNN90UO3bsiClTpsTmzZu7ao4AQJmpLGbwt7/97TjiiCNabTvttNPi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PvromDt3bvz0pz9tM/bpp5+OU089Nfr37x+DBg2Kz3/+8/Hyyy+3e7s333xzjBkzJgqFQnzyk5+M2traeP/999uM27FjR5x33nkxbNiw6Nu3b5x00kmxadOmkh/nwerWW2+NioqK6N+/f5vLrHfnPf744zFr1qwYPHhw9OnTJ0aNGhXXX399qzHWufOeeeaZOPPMM6O6ujr69u0bY8aMieuuuy7eeaf1x4Nb6+Ls2bMnrrzyypgxY0YMHz48KioqYsmSJe2O7e61ffTRR+Okk06Kvn37xrBhw+K8886LHTt2FHfAnf4s1YPE9OnT06BBg9J3vvOdtHnz5nThhRemiEhr167t7qkdVP74j/84TZs2La1cuTJt3bo1rVu3Lk2ZMiVVVlamTZs2tYx74YUX0uGHH55+//d/P61fvz7dd999ady4cam6ujrt2LGj1W3ecMMNqaKiItXU1KQtW7akv/3bv029e/dOX/va11qN27dvXxo/fnw65phj0po1a9IjjzyS5s6dmyorK9PWrVuzHH93eu2119LAgQNTdXV16tevX6vLrHfnrV27NvXq1Sudc8456T/+4z/S5s2b0z/90z+l2traljHWufOef/75VFVVlT796U+ne+65J23atCktXrw4HXbYYemP/uiPWsZZ6+K98soraeDAgenkk09u+R22ePHiNuO6e223bt2aKisr09y5c9MjjzyS1qxZk44++ug0fvz4tG/fvgM+3rIIkPXr16eISHfeeWer7dOnT0/V1dXpgw8+6KaZHXzeeOONNtv27NmTjjzyyHTKKae0bJs3b14aNmxYqq+vb9m2bdu29Fu/9VvpyiuvbNm2c+fOVFVVlS666KJWt7l06dJUUVGRnn/++ZZt3/72t1NEpP/6r/9q2fb++++nsWPHpsmTJ5fk+A5ms2fPTnPmzEnnnntumwCx3p3z2muvpX79+qX58+d/7Djr3HnXXHNNioj04osvttp+0UUXpYhIu3btSilZ645obm5Ozc3NKaWU3nzzzf0GSHev7YknnpjGjh2b3n///ZZtP/rRj1JEpJUrVx7w8ZZFgFx44YWpf//+rRYjpZTuvPPOFBHpRz/6UTfN7NAxbdq0NHr06JTSrx50ffr0SRdffHGbcTNmzEijRo1qOb9mzZoUEemJJ55oNe7DLyhcunRpy7ZTTz01nXDCCW1u88Ybb0wRkV577bVSHc5B54477kiHH354qquraxMg1rvzlixZkiIibdu2bb9jrHNpfLjWb775ZqvtV155ZerVq1dqbGy01iWwvwDp7rV97bXXUkSkZcuWtRk7evToNH369AM+xrJ4D8hzzz0Xn/rUp6KysvXnqk2cOLHlcvavvr4+nn766Rg3blxERLz00kvx7rvvtqzfr5s4cWK8+OKLsW/fvoj4v7WdMGFCq3G//du/HcOGDWu19s8999x+bzMi4vnnny/NAR1kduzYEQsXLozly5fHMccc0+Zy6915P/zhD2PIkCHxi1/8IiZNmhSVlZVxxBFHxCWXXNLy9eHWuTTOPffcGDRoUMyfPz9efvnl2LNnT/zgBz+I7373u7FgwYLo16+fte5C3b22H15nf2OL+X1bFgHy1ltvtftFeB9ua+8L9Pg/CxYsiL1798Y111wTEf+3Xvtb05RSvP322y1jC4VC9OvXr92xv772PfV+uvTSS+OEE06I+fPnt3u59e68119/Pd55552YN29enH322fHoo4/GFVdcEbfffnvMmjUrUkrWuUSOPfbYeOKJJ+K5556L4447LgYMGBBz5syJc889N2666aaI8JjuSt29tr9p/8XcB0V9FPvBrKKiokOX9XTf+MY3Yu3atXHzzTfHZz7zmVaXHeiaFrP2Pe1+uu++++KBBx6IZ5555jcen/XuuObm5ti3b18sXrw4Fi1aFBERU6dOjd69e8fChQtj06ZN0bdv34iwzp21bdu2mDNnThx55JFx7733xvDhw+PHP/5x3HDDDdHY2BirV69uGWutu053r+3+xhZzH5TFMyBDhw5tt7p27doVEe2XGhG1tbVxww03xNKlS+Oyyy5r2T506NCIaP//Jnbt2hUVFRUxaNCglrH79u1r8+d3H4799bXvafdTY2NjLFiwIL7+9a9HdXV17N69O3bv3h3vvfdeRETs3r079u7da71L4MM1nDlzZqvtp59+ekT86k8WrXNpLFq0KBoaGuLhhx+OL3zhC3HyySfHFVdcEX//938f3/ve9+Kxxx6z1l2ou9f2N+2/mPugLAJkwoQJ8cILL8QHH3zQavuzzz4bERHjx4/vjmkd1Gpra2PJkiWxZMmSuPrqq1tddtxxx0WfPn1a1u/XPfvss3H88cdHVVVVRPzfa4sfHfvLX/4ydu7c2WrtJ0yYsN/bjCi/+2nnzp3xxhtvxIoVK2Lw4MEtp7vuuiv27t0bgwcPjj/5kz+x3iXQ3uvRERHp/3/TRK9evaxzifzsZz+LsWPHtnla/8QTT4yIaHlpxlp3je5e2w//u7+xRd0HB/x21YPYhg0bUkSku+++u9X20047zZ/htuO6665LEZGuvfba/Y754he/mI444ojU0NDQsu3VV19NvXv3TldddVXLtrfeeitVVVWlSy65pNX1ly1b1ubPvFauXJkiIj355JMt295///00bty49NnPfrYUh3ZQeffdd9OWLVvanGbOnJmqqqrSli1b0rPPPptSst6d9fDDD7d5V39KKf3d3/1dioj0n//5nykl61wK06ZNS8OHD0979uxptX3VqlUpItL999+fUrLWnfVxf4bb3Ws7efLkNH78+Fa/W5944okUEemWW2454GMsiwBJ6Vef+TF48OC0atWqtHnz5vS1r30tRURas2ZNd0/toPKtb30rRUQ67bTT0hNPPNHm9KEXXngh9e/fP5188slpw4YN6V//9V/T+PHjP/aDbq6++uq0devW9M1vfjMVCoV2P+hm3LhxacSIEWnt2rVp48aN6ayzziqbDxE6UO19Doj17rw5c+akQqGQrr/++rRx48a0bNmyVFVVlWbPnt0yxjp33r//+7+nioqKNGXKlJYPIlu6dGnq379/Gjt2bGpqakopWeuO2rBhQ1q3bl363ve+lyIizZs3L61bty6tW7cu7d27N6XU/Wu7ZcuWVFlZmc4666y0cePGtHbt2jRixIie+UFkKf3qw7T+/M//PB111FGpd+/eaeLEiemuu+7q7mkddP7gD/4gRcR+T7/uqaeeSqecckrq27dvGjBgQDrzzDPbfPjQh2666aY0evTo1Lt37zRy5Mi0ePHi9N5777UZ98tf/jJ99atfTUOGDElVVVVpypQpaePGjV1yrAer9gIkJevdWe+880666qqr0ogRI1JlZWUaOXJkqqmpafMD0Tp33ubNm9OMGTPSUUcdlfr06ZNGjx6d/uqv/irt3Lmz1ThrXbxPfOIT+/35/Morr7SM6+61feSRR9KUKVNSVVVVGjJkSPrqV7/a7gddfpyKlP7/i6QAAJmUxZtQAYBDiwABALITIABAdgIEAMhOgAAA2QkQACA7AQIAZCdAAIDsBAgAkJ0AAQCyEyAAQHYCBADI7v8B5af2nsavP4AAAAAASUVORK5CYII=",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
-                "closest_to_blacklist = bioframe.closest(ctcf_peaks,blacklist)\n",
-                "plt.hist(closest_to_blacklist['distance'].astype('Float64').astype('float'),np.arange(0,1e4,100));"
+                "closest_to_blacklist = bioframe.closest(ctcf_peaks, blacklist)\n",
+                "plt.hist(\n",
+                "    closest_to_blacklist[\"distance\"].astype(\"Float64\").astype(\"float\"),\n",
+                "    np.arange(0, 1e4, 100),\n",
+                ");"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "to be safe, let's remove anything +/- 1kb from a blacklisted region"
@@ -552,24 +583,38 @@
         },
         {
             "cell_type": "code",
             "execution_count": 13,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# first let's select the columns we want for our final dataframe of peaks with motifs\n",
+                "# first let's select the columns we want for our final dataframe of peaks\n",
+                "# with motifs\n",
                 "df_peaks_maxmotif = df_peaks_maxmotif[\n",
-                "                            ['chrom_1','start_1','end_1','fc_1',\n",
-                "                             'chrom_2','start_2','end_2','pval_2','strand_2']]\n",
+                "    [\n",
+                "        \"chrom_1\",\n",
+                "        \"start_1\",\n",
+                "        \"end_1\",\n",
+                "        \"fc_1\",\n",
+                "        \"chrom_2\",\n",
+                "        \"start_2\",\n",
+                "        \"end_2\",\n",
+                "        \"pval_2\",\n",
+                "        \"strand_2\",\n",
+                "    ]\n",
+                "]\n",
                 "#  then rename columns for convenience when subtracting\n",
                 "for i in df_peaks_maxmotif.keys():\n",
-                "    if '_1' in i: df_peaks_maxmotif.rename(columns={i:i.split('_')[0]},inplace=True)\n",
+                "    if \"_1\" in i:\n",
+                "        df_peaks_maxmotif.rename(columns={i: i.split(\"_\")[0]}, inplace=True)\n",
                 "\n",
-                "# now subtract, expanding the blacklist by 1kb        \n",
-                "df_peaks_maxmotif_clean = bioframe.subtract(df_peaks_maxmotif,bioframe.expand(blacklist,1000))"
+                "# now subtract, expanding the blacklist by 1kb\n",
+                "df_peaks_maxmotif_clean = bioframe.subtract(\n",
+                "    df_peaks_maxmotif, bioframe.expand(blacklist, 1000)\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "there it is! we now have a dataframe containing positions of CTCF ChIP peaks, \n",
```

### Comparing `bioframe-0.6.4/docs/tutorials/tutorial_assign_peaks_to_genes.ipynb` & `bioframe-0.7.0/docs/tutorials/tutorial_assign_peaks_to_genes.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9959429752188703%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(0, 'import matplotlib.pyplot as plt\\n'), (2, '\\n'), (3, "*

 * *            "'import bioframe')], delete: [3, 2, 0]}}, 2: {'source': ['base_dir = "*

 * *            '"/tmp/bioframe_tutorial_data/"\\n\', \'assembly = "hg38"\']}, 7: {\'source\': '*

 * *            "{insert: [(0, 'ctcf_peaks = bioframe.read_table(\\n'), (1, '    "*

 * *            '"https://www.encodeproject.org/files/ENCFF401MQL/@@download/ENCFF401MQL.bed.gz",\\n\'), '*

 * *            '(2, \'    schema="narrowPeak",\\n\'), (3, […]*

```diff
@@ -13,29 +13,29 @@
         {
             "cell_type": "code",
             "execution_count": 1,
             "id": "ad9ab941",
             "metadata": {},
             "outputs": [],
             "source": [
-                "import bioframe\n",
+                "import matplotlib.pyplot as plt\n",
                 "import numpy as np\n",
-                "import pandas as pd \n",
-                "import matplotlib.pyplot as plt"
+                "\n",
+                "import bioframe"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 72,
             "id": "562865cc",
             "metadata": {},
             "outputs": [],
             "source": [
-                "base_dir = '/tmp/bioframe_tutorial_data/'\n",
-                "assembly = 'hg38'"
+                "base_dir = \"/tmp/bioframe_tutorial_data/\"\n",
+                "assembly = \"hg38\""
             ]
         },
         {
             "cell_type": "markdown",
             "id": "d3dae5c3",
             "metadata": {},
             "source": [
@@ -216,27 +216,32 @@
                     },
                     "execution_count": 3,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "ctcf_peaks = bioframe.read_table(\"https://www.encodeproject.org/files/ENCFF401MQL/@@download/ENCFF401MQL.bed.gz\", schema='narrowPeak')\n",
+                "ctcf_peaks = bioframe.read_table(\n",
+                "    \"https://www.encodeproject.org/files/ENCFF401MQL/@@download/ENCFF401MQL.bed.gz\",\n",
+                "    schema=\"narrowPeak\",\n",
+                ")\n",
                 "ctcf_peaks.head()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 83,
             "id": "5a228b72",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Filter for selected chromosomes:\n",
-                "ctcf_peaks = bioframe.overlap(ctcf_peaks, chromosomes).dropna(subset=['name_'])[ctcf_peaks.columns]"
+                "ctcf_peaks = bioframe.overlap(ctcf_peaks, chromosomes).dropna(subset=[\"name_\"])[\n",
+                "    ctcf_peaks.columns\n",
+                "]"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "e39fca85",
             "metadata": {},
             "source": [
@@ -366,33 +371,35 @@
                     },
                     "execution_count": 4,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "genes_url = 'https://hgdownload.soe.ucsc.edu/goldenpath/hg38/bigZips/genes/hg38.ensGene.gtf.gz'\n",
-                "genes = bioframe.read_table(genes_url, schema='gtf').query('feature==\"CDS\"')\n",
+                "genes_url = (\n",
+                "    \"https://hgdownload.soe.ucsc.edu/goldenpath/hg38/bigZips/genes/hg38.ensGene.gtf.gz\"\n",
+                ")\n",
+                "genes = bioframe.read_table(genes_url, schema=\"gtf\").query('feature==\"CDS\"')\n",
                 "\n",
-                "genes.head() \n",
+                "genes.head()\n",
                 "\n",
                 "## Note this functions to parse the attributes of the genes:\n",
                 "# import bioframe.sandbox.gtf_io\n",
                 "# genes_attr = bioframe.sandbox.gtf_io.parse_gtf_attributes(genes['attributes'])"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 84,
             "id": "84b4226f",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Filter for selected chromosomes:\n",
-                "genes = bioframe.overlap(genes, chromosomes).dropna(subset=['name_'])[genes.columns]"
+                "genes = bioframe.overlap(genes, chromosomes).dropna(subset=[\"name_\"])[genes.columns]"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "111ff194",
             "metadata": {},
             "source": [
@@ -439,17 +446,17 @@
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
-                "# Plot the distribution of distances from peaks to genes: \n",
-                "plt.hist( peaks_closest['distance'], np.arange(0, 1e3, 10));\n",
-                "plt.xlim( [0, 1e3] )"
+                "# Plot the distribution of distances from peaks to genes:\n",
+                "plt.hist(peaks_closest[\"distance\"], np.arange(0, 1e3, 10))\n",
+                "plt.xlim([0, 1e3])"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "8cec3987",
             "metadata": {},
             "source": [
@@ -465,25 +472,31 @@
         {
             "cell_type": "code",
             "execution_count": 88,
             "id": "e99e5213",
             "metadata": {},
             "outputs": [],
             "source": [
-                "peaks_closest_upstream_nodir = bioframe.closest(genes, ctcf_peaks, \n",
+                "peaks_closest_upstream_nodir = bioframe.closest(\n",
+                "    genes,\n",
+                "    ctcf_peaks,\n",
                 "    ignore_overlaps=False,\n",
                 "    ignore_upstream=False,\n",
                 "    ignore_downstream=True,\n",
-                "    direction_col=None)\n",
+                "    direction_col=None,\n",
+                ")\n",
                 "\n",
-                "peaks_closest_downstream_nodir = bioframe.closest(genes, ctcf_peaks, \n",
+                "peaks_closest_downstream_nodir = bioframe.closest(\n",
+                "    genes,\n",
+                "    ctcf_peaks,\n",
                 "    ignore_overlaps=False,\n",
                 "    ignore_upstream=True,\n",
                 "    ignore_downstream=False,\n",
-                "    direction_col=None)"
+                "    direction_col=None,\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "2fa693c9",
             "metadata": {},
             "source": [
@@ -514,17 +527,27 @@
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
-                "plt.hist( peaks_closest_upstream_nodir['distance'], np.arange(0, 1e4, 100), alpha=0.5, label=\"upstream\");\n",
-                "plt.hist( peaks_closest_downstream_nodir['distance'], np.arange(0, 1e4, 100), alpha=0.5, label=\"downstream\");\n",
-                "plt.xlim( [0, 1e4] )\n",
+                "plt.hist(\n",
+                "    peaks_closest_upstream_nodir[\"distance\"],\n",
+                "    np.arange(0, 1e4, 100),\n",
+                "    alpha=0.5,\n",
+                "    label=\"upstream\",\n",
+                ")\n",
+                "plt.hist(\n",
+                "    peaks_closest_downstream_nodir[\"distance\"],\n",
+                "    np.arange(0, 1e4, 100),\n",
+                "    alpha=0.5,\n",
+                "    label=\"downstream\",\n",
+                ")\n",
+                "plt.xlim([0, 1e4])\n",
                 "plt.legend()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "4f130a50",
             "metadata": {},
@@ -543,25 +566,31 @@
             "cell_type": "code",
             "execution_count": 90,
             "id": "b47d83fa",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Note that \"strand\" here is the column name in genes table:\n",
-                "peaks_closest_upstream_dir = bioframe.closest(genes, ctcf_peaks, \n",
+                "peaks_closest_upstream_dir = bioframe.closest(\n",
+                "    genes,\n",
+                "    ctcf_peaks,\n",
                 "    ignore_overlaps=False,\n",
                 "    ignore_upstream=False,\n",
                 "    ignore_downstream=True,\n",
-                "    direction_col='strand')\n",
+                "    direction_col=\"strand\",\n",
+                ")\n",
                 "\n",
-                "peaks_closest_downstream_dir = bioframe.closest(genes, ctcf_peaks, \n",
+                "peaks_closest_downstream_dir = bioframe.closest(\n",
+                "    genes,\n",
+                "    ctcf_peaks,\n",
                 "    ignore_overlaps=False,\n",
                 "    ignore_upstream=True,\n",
                 "    ignore_downstream=False,\n",
-                "    direction_col='strand')"
+                "    direction_col=\"strand\",\n",
+                ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 96,
             "id": "f18e706a",
             "metadata": {},
@@ -584,17 +613,27 @@
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
-                "plt.hist( peaks_closest_upstream_dir['distance'], np.arange(0, 1e4, 100), alpha=0.5, label=\"upstream\");\n",
-                "plt.hist( peaks_closest_downstream_dir['distance'], np.arange(0, 1e4, 100), alpha=0.5, label=\"downstream\");\n",
-                "plt.xlim( [0, 1e4] )\n",
+                "plt.hist(\n",
+                "    peaks_closest_upstream_dir[\"distance\"],\n",
+                "    np.arange(0, 1e4, 100),\n",
+                "    alpha=0.5,\n",
+                "    label=\"upstream\",\n",
+                ")\n",
+                "plt.hist(\n",
+                "    peaks_closest_downstream_dir[\"distance\"],\n",
+                "    np.arange(0, 1e4, 100),\n",
+                "    alpha=0.5,\n",
+                "    label=\"downstream\",\n",
+                ")\n",
+                "plt.xlim([0, 1e4])\n",
                 "plt.legend()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "65b4a264",
             "metadata": {},
```

### Comparing `bioframe-0.6.4/tests/test_assembly_info.py` & `bioframe-0.7.0/tests/test_assembly_info.py`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.4/tests/test_core_checks.py` & `bioframe-0.7.0/tests/test_core_checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,14 @@
     )
     assert is_cataloged(
         df, view_df, df_view_col="funny_view_region", view_name_col="funny_name"
     )
 
 
 def test_is_contained():
-
     view_df = pd.DataFrame(
         [
             ["chr1", 0, 20, "chr1p"],
             ["chr1", 21, 30, "chr1q"],
             ["chrX", 1, 10, "chrX_0"],
         ],
         columns=["chrom", "start", "end", "name"],
@@ -430,15 +429,14 @@
         ],
         columns=["chrom", "start", "end", "name"],
     )
     assert is_viewframe(df1)
 
 
 def test_is_sorted():
-
     view_df = pd.DataFrame(
         [
             ["chrX", 1, 8, "oranges"],
             ["chrX", 8, 20, "grapefruit"],
             ["chr1", 0, 10, "apples"],
         ],
         columns=["chrom", "start", "end", "fruit"],
```

### Comparing `bioframe-0.6.4/tests/test_core_construction.py` & `bioframe-0.7.0/tests/test_core_construction.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
         pd.Series(
             data=["chr0:1-4", "chr1:2-5", "chr2:3-6"], index=[0, 1, 2], name="name"
         ),
     )
 
 
 def test_any():
-
     ### tests copied from old parse_regions
     # main functionality: convert to dataframe and create name
     df = pd.DataFrame(
         {"chrom": [f"chr{i}" for i in range(3)], "start": [1, 2, 3], "end": [4, 5, 6]}
     )
     parsed = from_any(df)
     assert "name" not in parsed.columns
@@ -166,15 +165,14 @@
     )
     assert construction.sanitize_bedframe(
         df1, start_exceed_end_action="drop", drop_null=True
     ).empty
 
 
 def test_make_viewframe():
-
     # test dict input
     view_df = pd.DataFrame(
         [
             ["chrTESTX", 0, 10, "chrTESTX:0-10"],
             ["chrTESTX_p", 0, 12, "chrTESTX_p:0-12"],
         ],
         columns=["chrom", "start", "end", "name"],
```

### Comparing `bioframe-0.6.4/tests/test_core_specs.py` & `bioframe-0.7.0/tests/test_core_specs.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,14 @@
         specs.update_default_colnames(["chromosome", "start", "end", "extrasuff"])
 
     # reset to default
     specs.update_default_colnames(("chrom", "start", "end"))
 
 
 def test_verify_columns():
-
     new_names = ("C", "chromStart", "chromStop")
     df1 = pd.DataFrame(
         [["chr1", 1, 5], ["chr1", 3, 8], ["chr1", 8, 10], ["chr1", 12, 14]],
         columns=list(new_names),
     )
 
     with pytest.raises(ValueError):
@@ -67,15 +66,14 @@
 
     # no repeated column names
     with pytest.raises(ValueError):
         specs._verify_columns(df1, ["chromStart", "chromStart"], unique_cols=True)
 
 
 def test_verify_column_dtypes():
-
     new_names = ("C", "chromStart", "chromStop")
     df1 = pd.DataFrame(
         [["chr1", 1, 5], ["chr1", 3, 8], ["chr1", 8, 10], ["chr1", 12, 14]],
         columns=list(new_names),
     )
 
     with pytest.raises(ValueError):
```

### Comparing `bioframe-0.6.4/tests/test_core_stringops.py` & `bioframe-0.7.0/tests/test_core_stringops.py`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.4/tests/test_extras.py` & `bioframe-0.7.0/tests/test_extras.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 import bioframe
 
 testdir = op.realpath(op.dirname(__file__))
 
 
 def test_make_chromarms():
-
     ### test the case where columns have different names
     df = pd.DataFrame(
         [["chrX", 0, 8]],
         columns=["chromosome", "lo", "hi"],
     )
     mids = pd.DataFrame([["chrX", 4]], columns=["chromosome", "loc"])
     arms = pd.DataFrame(
@@ -188,15 +187,14 @@
             return_input=False,
             mapped_only=False,
         ).values
     ).all()
 
 
 def test_seq_gc():
-
     assert 0 == bioframe.seq_gc("AT")
     assert np.isnan(bioframe.seq_gc("NNN"))
     assert 1 == bioframe.seq_gc("NGnC")
     assert 0.5 == bioframe.seq_gc("GTCA")
     assert 0.25 == bioframe.seq_gc("nnnNgTCa", mapped_only=False)
     with pytest.raises(ValueError):
         bioframe.seq_gc(["A", "T"])
```

### Comparing `bioframe-0.6.4/tests/test_ops.py` & `bioframe-0.7.0/tests/test_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -2024,17 +2024,15 @@
     counts_nans_inserted_after = (
         pd.concat([pd.DataFrame([pd.NA]), counts_no_nans, pd.DataFrame([pd.NA])])
     ).astype(
         {
             "start": pd.Int64Dtype(),
             "end": pd.Int64Dtype(),
         }
-    )[
-        ["chrom1", "start", "end", "strand", "animal", "count"]
-    ]
+    )[["chrom1", "start", "end", "strand", "animal", "count"]]
 
     counts_nans = bioframe.count_overlaps(
         df1_na,
         df2_na,
         on=None,
         cols1=("chrom1", "start", "end"),
         cols2=("chrom2", "start2", "end2"),
```

### Comparing `bioframe-0.6.4/tests/test_ops_select.py` & `bioframe-0.7.0/tests/test_ops_select.py`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.4/tests/test_resources.py` & `bioframe-0.7.0/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.4/tests/test_vis.py` & `bioframe-0.7.0/tests/test_vis.py`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.4/LICENSE` & `bioframe-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bioframe-0.6.4/README.md` & `bioframe-0.7.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # Bioframe: Operations on Genomic Interval Dataframes
 
-<img src="https://github.com/open2c/bioframe/raw/main/docs/figs/bioframe-logo.png" width=75%> 
+<img src="https://github.com/open2c/bioframe/raw/main/docs/figs/bioframe-logo.png" width=75%>
 
 ![CI](https://github.com/open2c/bioframe/actions/workflows/ci.yml/badge.svg)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/open2c/bioframe/main.svg)](https://results.pre-commit.ci/latest/github/open2c/bioframe/main)
 [![Docs status](https://readthedocs.org/projects/bioframe/badge/)](https://bioframe.readthedocs.io/en/latest/)
 [![Paper](https://img.shields.io/badge/DOI-10.1093%2Fbioinformatics%2Fbtae088-blue)](https://doi.org/10.1093/bioinformatics/btae088)
 [![Zenodo](https://zenodo.org/badge/69901992.svg)](https://zenodo.org/badge/latestdoi/69901992)
 [![Slack](https://img.shields.io/badge/chat-slack-%233F0F3F?logo=slack)](https://bit.ly/open2c-slack)
 [![NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](https://www.numfocus.org)
 
-Bioframe enables flexible and scalable operations on genomic interval dataframes in Python. 
+Bioframe enables flexible and scalable operations on genomic interval dataframes in Python.
 
-Bioframe is built directly on top of [Pandas](https://pandas.pydata.org/). Bioframe provides: 
+Bioframe is built directly on top of [Pandas](https://pandas.pydata.org/). Bioframe provides:
 
 * A variety of genomic interval operations that work directly on dataframes.
 * Operations for special classes of genomic intervals, including chromosome arms and fixed-size bins.
 * Conveniences for diverse tabular genomic data formats and loading genome assembly summary information.
 
 Read the [docs](https://bioframe.readthedocs.io/en/latest/), including the [guide](https://bioframe.readthedocs.io/en/latest/guide-intervalops.html), as well as the [bioframe preprint](https://doi.org/10.1101/2022.02.16.480748) for more information.
 
@@ -34,71 +35,71 @@
 Interested in contributing to bioframe? That's great! To get started, check out the [contributing guide](https://github.com/open2c/bioframe/blob/main/CONTRIBUTING.md). Discussions about the project roadmap take place on the [Open2C Slack](https://bit.ly/open2c-slack) and regular developer meetings scheduled there. Anyone can join and participate!
 
 
 ## Interval operations
 
 Key genomic interval operations in bioframe include:
 - `overlap`: Find pairs of overlapping genomic intervals between two dataframes.
-- `closest`: For every interval in a dataframe, find the closest intervals in a second dataframe. 
+- `closest`: For every interval in a dataframe, find the closest intervals in a second dataframe.
 - `cluster`: Group overlapping intervals in a dataframe into clusters.
 - `complement`: Find genomic intervals that are not covered by any interval from a dataframe.
- 
+
 Bioframe additionally has functions that are frequently used for genomic interval operations and can be expressed as combinations of these core operations and dataframe operations, including: `coverage`, `expand`, `merge`, `select`, and `subtract`.
 
 To `overlap` two dataframes, call:
 ```python
 import bioframe as bf
 
 bf.overlap(df1, df2)
 ```
 
 For these two input dataframes, with intervals all on the same chromosome:
 
-<img src="https://github.com/open2c/bioframe/raw/main/docs/figs/df1.png" width=60%> 
-<img src="https://github.com/open2c/bioframe/raw/main/docs/figs/df2.png" width=60%> 
+<img src="https://github.com/open2c/bioframe/raw/main/docs/figs/df1.png" width=60%>
+<img src="https://github.com/open2c/bioframe/raw/main/docs/figs/df2.png" width=60%>
 
 `overlap` will return the following interval pairs as overlaps:
 
-<img src="https://github.com/open2c/bioframe/raw/main/docs/figs/overlap_inner_0.png" width=60%> 
-<img src="https://github.com/open2c/bioframe/raw/main/docs/figs/overlap_inner_1.png" width=60%> 
+<img src="https://github.com/open2c/bioframe/raw/main/docs/figs/overlap_inner_0.png" width=60%>
+<img src="https://github.com/open2c/bioframe/raw/main/docs/figs/overlap_inner_1.png" width=60%>
 
 
 To `merge` all overlapping intervals in a dataframe, call:
 ```python
 import bioframe as bf
 
 bf.merge(df1)
 ```
 
 For this input dataframe, with intervals all on the same chromosome:
 
-<img src="https://github.com/open2c/bioframe/raw/main/docs/figs/df1.png" width=60%> 
+<img src="https://github.com/open2c/bioframe/raw/main/docs/figs/df1.png" width=60%>
 
 `merge` will return a new dataframe with these merged intervals:
 
-<img src="https://github.com/open2c/bioframe/raw/main/docs/figs/merge_df1.png" width=60%> 
+<img src="https://github.com/open2c/bioframe/raw/main/docs/figs/merge_df1.png" width=60%>
 
 See the [guide](https://bioframe.readthedocs.io/en/latest/guide-intervalops.html) for visualizations of other interval operations in bioframe.
 
 ## File I/O
 
 Bioframe includes utilities for reading genomic file formats into dataframes and vice versa. One handy function is `read_table` which mirrors pandas’s read_csv/read_table but provides a [`schema`](https://github.com/open2c/bioframe/blob/main/bioframe/io/schemas.py) argument to populate column names for common tabular file formats.
 
 ```python
 jaspar_url = 'http://expdata.cmmt.ubc.ca/JASPAR/downloads/UCSC_tracks/2022/hg38/MA0139.1.tsv.gz'
 ctcf_motif_calls = bioframe.read_table(jaspar_url, schema='jaspar', skiprows=1)
 ```
 
 ## Tutorials
-See this [jupyter notebook](https://github.com/open2c/bioframe/tree/master/docs/tutorials/tutorial_assign_motifs_to_peaks.ipynb) for an example of how to assign TF motifs to ChIP-seq peaks using bioframe. 
+See this [jupyter notebook](https://github.com/open2c/bioframe/tree/master/docs/tutorials/tutorial_assign_motifs_to_peaks.ipynb) for an example of how to assign TF motifs to ChIP-seq peaks using bioframe.
 
 
 ## Citing
 
-If you use ***bioframe*** in your work, please cite:  
+If you use ***bioframe*** in your work, please cite:
 
 ```bibtex
 @article{bioframe_2024,
 author = {Open2C and Abdennur, Nezar and Fudenberg, Geoffrey and Flyamer, Ilya M and Galitsyna, Aleksandra A and Goloborodko, Anton and Imakaev, Maxim and Venev, Sergey},
 doi = {10.1093/bioinformatics/btae088},
 journal = {Bioinformatics},
 title = {{Bioframe: Operations on Genomic Intervals in Pandas Dataframes}},
```

### Comparing `bioframe-0.6.4/pyproject.toml` & `bioframe-0.7.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-vcs"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bioframe"
-version = "0.6.4"
+version = "0.7.0"
 description = "Operations and utilities for Genomic Interval Dataframes."
 license = {text = "MIT"}
 authors = [
   {name = "Open2C", email = "open.chromosome.collective@gmail.com"},
 ]
 keywords = [
     "pandas",
@@ -45,15 +45,14 @@
     "importlib-metadata ; python_version<'3.8'",
     "importlib-resources ; python_version<'3.9'",
 ]
 
 [project.optional-dependencies]
 dev = [
     "biopython",
-    "isort",
     "pysam",
     "pybbi",
     "pytest",
     "ruff",
 ]
 test = [
     "pytest",
@@ -69,41 +68,45 @@
 
 [project.urls]
 homepage = "https://github.com/open2c/bioframe"
 documentation = "https://bioframe.readthedocs.io/en/latest"
 repository = "https://github.com/open2c/bioframe"
 changelog = "https://github.com/open2c/bioframe/blob/main/CHANGES.md"
 
-[tool.isort]
-profile = "black"
-skip_gitignore = true
-known_first_party = "bioframe"
-
 [tool.ruff]
 target-version = "py37"
 exclude = [
     ".venv",
 ]
-lint.extend-select = [
+
+[tool.ruff.lint]
+extend-select = [
     # "C",  # mccabe complexity
     # "D",  # pydocstyle
     "E",  # style errors
     "F",  # pyflakes
     "I",  # isort
     "RUF", # ruff-specific rules
     "UP", # pyupgrade
     "W",  # style  warnings
 ]
 
+[tool.ruff.lint.isort]
+known-first-party = ["bioframe"]
+
+[tool.ruff.lint.pydocstyle]
+convention = "numpy"
+
 [tool.hatch.envs.default]
 features = ["dev", "test", "docs"]
 
 [tool.hatch.envs.default.scripts]
 fix = "ruff check --fix ."
 lint = "ruff check bioframe tests"
+format = "ruff format bioframe tests"
 test = "pytest ."
 docs = "sphinx-autobuild docs docs/_build/html"
 
 [tool.hatch.envs.test]
 features = ["dev", "test"]
 
 [[tool.hatch.envs.test.matrix]]
```

### Comparing `bioframe-0.6.4/PKG-INFO` & `bioframe-0.7.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bioframe
-Version: 0.6.4
+Version: 0.7.0
 Summary: Operations and utilities for Genomic Interval Dataframes.
 Project-URL: homepage, https://github.com/open2c/bioframe
 Project-URL: documentation, https://bioframe.readthedocs.io/en/latest
 Project-URL: repository, https://github.com/open2c/bioframe
 Project-URL: changelog, https://github.com/open2c/bioframe/blob/main/CHANGES.md
 Author-email: Open2C <open.chromosome.collective@gmail.com>
 License: MIT
@@ -25,15 +25,14 @@
 Requires-Dist: numpy>=1.10
 Requires-Dist: pandas>=1.3
 Requires-Dist: pyyaml
 Requires-Dist: requests
 Requires-Dist: typing-extensions; python_version < '3.9'
 Provides-Extra: dev
 Requires-Dist: biopython; extra == 'dev'
-Requires-Dist: isort; extra == 'dev'
 Requires-Dist: pybbi; extra == 'dev'
 Requires-Dist: pysam; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: autodocsumm; extra == 'docs'
 Requires-Dist: jinja2; extra == 'docs'
@@ -43,26 +42,27 @@
 Requires-Dist: sphinx-rtd-theme; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Bioframe: Operations on Genomic Interval Dataframes
 
-<img src="https://github.com/open2c/bioframe/raw/main/docs/figs/bioframe-logo.png" width=75%> 
+<img src="https://github.com/open2c/bioframe/raw/main/docs/figs/bioframe-logo.png" width=75%>
 
 ![CI](https://github.com/open2c/bioframe/actions/workflows/ci.yml/badge.svg)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/open2c/bioframe/main.svg)](https://results.pre-commit.ci/latest/github/open2c/bioframe/main)
 [![Docs status](https://readthedocs.org/projects/bioframe/badge/)](https://bioframe.readthedocs.io/en/latest/)
 [![Paper](https://img.shields.io/badge/DOI-10.1093%2Fbioinformatics%2Fbtae088-blue)](https://doi.org/10.1093/bioinformatics/btae088)
 [![Zenodo](https://zenodo.org/badge/69901992.svg)](https://zenodo.org/badge/latestdoi/69901992)
 [![Slack](https://img.shields.io/badge/chat-slack-%233F0F3F?logo=slack)](https://bit.ly/open2c-slack)
 [![NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](https://www.numfocus.org)
 
-Bioframe enables flexible and scalable operations on genomic interval dataframes in Python. 
+Bioframe enables flexible and scalable operations on genomic interval dataframes in Python.
 
-Bioframe is built directly on top of [Pandas](https://pandas.pydata.org/). Bioframe provides: 
+Bioframe is built directly on top of [Pandas](https://pandas.pydata.org/). Bioframe provides:
 
 * A variety of genomic interval operations that work directly on dataframes.
 * Operations for special classes of genomic intervals, including chromosome arms and fixed-size bins.
 * Conveniences for diverse tabular genomic data formats and loading genome assembly summary information.
 
 Read the [docs](https://bioframe.readthedocs.io/en/latest/), including the [guide](https://bioframe.readthedocs.io/en/latest/guide-intervalops.html), as well as the [bioframe preprint](https://doi.org/10.1101/2022.02.16.480748) for more information.
 
@@ -81,71 +81,71 @@
 Interested in contributing to bioframe? That's great! To get started, check out the [contributing guide](https://github.com/open2c/bioframe/blob/main/CONTRIBUTING.md). Discussions about the project roadmap take place on the [Open2C Slack](https://bit.ly/open2c-slack) and regular developer meetings scheduled there. Anyone can join and participate!
 
 
 ## Interval operations
 
 Key genomic interval operations in bioframe include:
 - `overlap`: Find pairs of overlapping genomic intervals between two dataframes.
-- `closest`: For every interval in a dataframe, find the closest intervals in a second dataframe. 
+- `closest`: For every interval in a dataframe, find the closest intervals in a second dataframe.
 - `cluster`: Group overlapping intervals in a dataframe into clusters.
 - `complement`: Find genomic intervals that are not covered by any interval from a dataframe.
- 
+
 Bioframe additionally has functions that are frequently used for genomic interval operations and can be expressed as combinations of these core operations and dataframe operations, including: `coverage`, `expand`, `merge`, `select`, and `subtract`.
 
 To `overlap` two dataframes, call:
 ```python
 import bioframe as bf
 
 bf.overlap(df1, df2)
 ```
 
 For these two input dataframes, with intervals all on the same chromosome:
 
-<img src="https://github.com/open2c/bioframe/raw/main/docs/figs/df1.png" width=60%> 
-<img src="https://github.com/open2c/bioframe/raw/main/docs/figs/df2.png" width=60%> 
+<img src="https://github.com/open2c/bioframe/raw/main/docs/figs/df1.png" width=60%>
+<img src="https://github.com/open2c/bioframe/raw/main/docs/figs/df2.png" width=60%>
 
 `overlap` will return the following interval pairs as overlaps:
 
-<img src="https://github.com/open2c/bioframe/raw/main/docs/figs/overlap_inner_0.png" width=60%> 
-<img src="https://github.com/open2c/bioframe/raw/main/docs/figs/overlap_inner_1.png" width=60%> 
+<img src="https://github.com/open2c/bioframe/raw/main/docs/figs/overlap_inner_0.png" width=60%>
+<img src="https://github.com/open2c/bioframe/raw/main/docs/figs/overlap_inner_1.png" width=60%>
 
 
 To `merge` all overlapping intervals in a dataframe, call:
 ```python
 import bioframe as bf
 
 bf.merge(df1)
 ```
 
 For this input dataframe, with intervals all on the same chromosome:
 
-<img src="https://github.com/open2c/bioframe/raw/main/docs/figs/df1.png" width=60%> 
+<img src="https://github.com/open2c/bioframe/raw/main/docs/figs/df1.png" width=60%>
 
 `merge` will return a new dataframe with these merged intervals:
 
-<img src="https://github.com/open2c/bioframe/raw/main/docs/figs/merge_df1.png" width=60%> 
+<img src="https://github.com/open2c/bioframe/raw/main/docs/figs/merge_df1.png" width=60%>
 
 See the [guide](https://bioframe.readthedocs.io/en/latest/guide-intervalops.html) for visualizations of other interval operations in bioframe.
 
 ## File I/O
 
 Bioframe includes utilities for reading genomic file formats into dataframes and vice versa. One handy function is `read_table` which mirrors pandas’s read_csv/read_table but provides a [`schema`](https://github.com/open2c/bioframe/blob/main/bioframe/io/schemas.py) argument to populate column names for common tabular file formats.
 
 ```python
 jaspar_url = 'http://expdata.cmmt.ubc.ca/JASPAR/downloads/UCSC_tracks/2022/hg38/MA0139.1.tsv.gz'
 ctcf_motif_calls = bioframe.read_table(jaspar_url, schema='jaspar', skiprows=1)
 ```
 
 ## Tutorials
-See this [jupyter notebook](https://github.com/open2c/bioframe/tree/master/docs/tutorials/tutorial_assign_motifs_to_peaks.ipynb) for an example of how to assign TF motifs to ChIP-seq peaks using bioframe. 
+See this [jupyter notebook](https://github.com/open2c/bioframe/tree/master/docs/tutorials/tutorial_assign_motifs_to_peaks.ipynb) for an example of how to assign TF motifs to ChIP-seq peaks using bioframe.
 
 
 ## Citing
 
-If you use ***bioframe*** in your work, please cite:  
+If you use ***bioframe*** in your work, please cite:
 
 ```bibtex
 @article{bioframe_2024,
 author = {Open2C and Abdennur, Nezar and Fudenberg, Geoffrey and Flyamer, Ilya M and Galitsyna, Aleksandra A and Goloborodko, Anton and Imakaev, Maxim and Venev, Sergey},
 doi = {10.1093/bioinformatics/btae088},
 journal = {Bioinformatics},
 title = {{Bioframe: Operations on Genomic Intervals in Pandas Dataframes}},
```

